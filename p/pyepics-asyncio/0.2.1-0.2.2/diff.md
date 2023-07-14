# Comparing `tmp/pyepics_asyncio-0.2.1.tar.gz` & `tmp/pyepics_asyncio-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyepics_asyncio-0.2.1.tar", max compression
+gzip compressed data, was "pyepics_asyncio-0.2.2.tar", max compression
```

## Comparing `pyepics_asyncio-0.2.1.tar` & `pyepics_asyncio-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      638 2023-07-08 06:53:40.401654 pyepics_asyncio-0.2.1/README.md
--rw-r--r--   0        0        0     4037 2023-07-08 06:57:01.373994 pyepics_asyncio-0.2.1/pyepics_asyncio/__init__.py
--rw-r--r--   0        0        0        0 2022-04-06 12:17:54.769183 pyepics_asyncio-0.2.1/pyepics_asyncio/py.typed
--rw-r--r--   0        0        0      837 2023-07-08 06:59:14.374240 pyepics_asyncio-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1355 1970-01-01 00:00:00.000000 pyepics_asyncio-0.2.1/setup.py
--rw-r--r--   0        0        0     1526 1970-01-01 00:00:00.000000 pyepics_asyncio-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      929 2023-07-14 06:31:17.302665 pyepics_asyncio-0.2.2/README.md
+-rw-r--r--   0        0        0     5199 2023-07-14 08:38:44.330584 pyepics_asyncio-0.2.2/pyepics_asyncio/__init__.py
+-rw-r--r--   0        0        0        0 2022-04-06 12:17:54.769183 pyepics_asyncio-0.2.2/pyepics_asyncio/py.typed
+-rw-r--r--   0        0        0     2406 2023-07-14 08:01:03.568823 pyepics_asyncio-0.2.2/pyepics_asyncio/test_.py
+-rw-r--r--   0        0        0      882 2023-07-14 08:39:31.938786 pyepics_asyncio-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1657 1970-01-01 00:00:00.000000 pyepics_asyncio-0.2.2/setup.py
+-rw-r--r--   0        0        0     1817 1970-01-01 00:00:00.000000 pyepics_asyncio-0.2.2/PKG-INFO
```

### Comparing `pyepics_asyncio-0.2.1/pyepics_asyncio/__init__.py` & `pyepics_asyncio-0.2.2/pyepics_asyncio/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
-from typing import Any, AsyncIterable, AsyncIterator, Awaitable, TypeVar
+from typing import Any, List, AsyncIterable, AsyncIterator, Awaitable, TypeVar
 
 import asyncio
-from asyncio import AbstractEventLoop, Future, Queue
+from asyncio import AbstractEventLoop, Future, Event
+from threading import Lock
 
 import epics  # type: ignore
 
 
 class PvBase:
     def __init__(self, raw: epics.PV) -> None:
         self.raw = raw
@@ -28,19 +29,16 @@
 class Pv(PvBase):
     "Process variable"
 
     @staticmethod
     def connect(name: str) -> Awaitable[Pv]:
         return _Connect(name)
 
-    async def get(self) -> Any:
-        def caget() -> Any:
-            return self.raw.get(use_monitor=False)
-
-        await asyncio.get_running_loop().run_in_executor(None, caget)
+    def get(self) -> _GetFuture:
+        return _GetFuture(self)
 
 
 class PvMonitor(PvBase, AsyncIterable[Any]):
     "Process variable with monitor"
 
     def __init__(self, raw: epics.PV, monitor: _Monitor) -> None:
         super().__init__(raw)
@@ -68,81 +66,120 @@
             loop.call_soon_threadsafe(self._complete)
 
     def __init__(self, pv: PvBase, value: Any) -> None:
         super().__init__()
         pv.raw.put(value, wait=False, callback=self._callback)
 
 
+class _GetFuture(Future[Any]):
+    def _complete(self, value: Any) -> None:
+        if not self.done():
+            self.set_result(value)
+
+    def _clear(self) -> None:
+        self.raw.clear_auto_monitor()
+        self.raw.clear_callbacks()
+
+    def _callback(self, value: Any, **kw: Any) -> None:
+        self._clear()
+        loop = self.get_loop()
+        if not loop.is_closed():
+            loop.call_soon_threadsafe(lambda: self._complete(value))
+
+    def __init__(self, pv: PvBase) -> None:
+        super().__init__()
+        self.raw = pv.raw
+        self.raw.add_callback(self._callback)
+        self.add_done_callback(_GetFuture._clear)
+        self.raw.auto_monitor = epics.dbr.DBE_VALUE
+
+
 T = TypeVar("T", bound=PvBase)
 
 
 class _ConnectBase(Future[T]):
     def _cancel(self) -> None:
         self.raw.disconnect()
 
     def _complete(self) -> None:
         raise NotImplementedError()
 
     def _connection_callback(self, pvname: str = "", conn: bool = False, **kw: Any) -> None:
         assert pvname == self.name
         if conn:
+            self.raw.connection_callbacks.clear()
             assert self.remove_done_callback(_ConnectBase._cancel) == 1
             loop = self.get_loop()
             if not loop.is_closed():
                 loop.call_soon_threadsafe(self._complete)
 
-    def __init__(self, name: str, raw: epics.PV) -> None:
+    def __init__(self, name: str) -> None:
         super().__init__()
         self.name = name
-        self.raw = raw
+        self.raw = epics.PV.__new__(epics.PV)
         self.add_done_callback(_ConnectBase._cancel)
+        self.__init_raw__(self.raw)
+
+    def __init_raw__(self, raw: epics.PV) -> None:
+        raise NotImplementedError()
 
 
 class _Connect(_ConnectBase[Pv]):
     def _complete(self) -> None:
         self.set_result(Pv(self.raw))
 
-    def __init__(self, name: str) -> None:
-        super().__init__(
-            name,
-            epics.PV(
-                name,
-                form="native",
-                auto_monitor=False,
-                connection_callback=self._connection_callback,
-            ),
+    def __init_raw__(self, raw: epics.PV) -> None:
+        raw.__init__(
+            self.name,
+            form="native",
+            auto_monitor=False,
+            connection_callback=self._connection_callback,
         )
 
 
 class _ConnectMonitor(_ConnectBase[PvMonitor]):
     def _complete(self) -> None:
         self.set_result(PvMonitor(self.raw, self.values))
 
     def __init__(self, name: str) -> None:
         self.values = _Monitor(loop=asyncio.get_running_loop())
-        super().__init__(
-            name,
-            epics.PV(
-                name,
-                form="native",
-                auto_monitor=epics.dbr.DBE_VALUE,
-                connection_callback=self._connection_callback,
-                callback=self.values._callback,
-            ),
+        super().__init__(name)
+
+    def __init_raw__(self, raw: epics.PV) -> None:
+        raw.__init__(
+            self.name,
+            form="native",
+            auto_monitor=epics.dbr.DBE_VALUE,
+            connection_callback=self._connection_callback,
+            callback=self.values._callback,
         )
 
 
 class _Monitor(AsyncIterator[Any]):
     def __init__(self, loop: AbstractEventLoop) -> None:
         super().__init__()
         self._loop = loop
-        self._queue: Queue[Any] = Queue()
+        self._event = Event()
+        self._lock = Lock()
+        self._values: List[Any] = [None, None]
 
     def _callback(self, value: Any = None, **kw: Any) -> None:
+        with self._lock:
+            if self._values[0] is None:
+                self._values[0] = value
+            else:
+                self._values[1] = value
+
         if not self._loop.is_closed():
-            self._loop.call_soon_threadsafe(lambda: self._queue.put_nowait(value))
+            self._loop.call_soon_threadsafe(self._event.set)
 
     async def __anext__(self) -> Any:
-        return await self._queue.get()
+        while True:
+            with self._lock:
+                (value, *self._values) = (*self._values, None)
+                self._event.clear()
+            if value is not None:
+                return value
+            await self._event.wait()
 
     def __aiter__(self) -> _Monitor:
         return self
```

### Comparing `pyepics_asyncio-0.2.1/pyproject.toml` & `pyepics_asyncio-0.2.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyepics-asyncio"
-version = "0.2.1"
+version = "0.2.2"
 description = "Async/await wrapper for PyEpics"
 homepage = "https://github.com/agerasev/pyepics-asyncio"
 repository = "https://github.com/agerasev/pyepics-asyncio"
 authors = ["Alexey Gerasev <alexey.gerasev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["pyepics", "epics", "asyncio", "async", "await"]
@@ -18,14 +18,16 @@
 [tool.poetry.dependencies]
 python = "^3.9"
 pyepics = "^3.5.1"
 
 [tool.poetry.dev-dependencies]
 mypy = "^1.4.1"
 black = "^23.3.0"
+pytest = "^7.4.0"
+pytest-asyncio = "^0.21.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 128
```

### Comparing `pyepics_asyncio-0.2.1/PKG-INFO` & `pyepics_asyncio-0.2.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyepics-asyncio
-Version: 0.2.1
+Version: 0.2.2
 Summary: Async/await wrapper for PyEpics
 Home-page: https://github.com/agerasev/pyepics-asyncio
 License: MIT
 Keywords: pyepics,epics,asyncio,async,await
 Author: Alexey Gerasev
 Author-email: alexey.gerasev@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -54,7 +54,17 @@
 
 ### Write value to PV
 
 ```python
 await pv.put(3.1415)
 ```
 
+## Testing
+
+To run tests you need to have dummy IOC running (located in `ioc` dir):
+
++ Set appropriate `EPICS_BASE` path in `configure/RELEASE`.
++ Build with `make`.
++ Go to `iocBoot/iocTest/` and run script `st.cmd` and don't stop it.
+
+In separate shell run `poetry run pytest --verbose`.
+
```

