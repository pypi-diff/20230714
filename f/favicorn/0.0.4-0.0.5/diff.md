# Comparing `tmp/favicorn-0.0.4.tar.gz` & `tmp/favicorn-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "favicorn-0.0.4.tar", last modified: Sat Apr 29 10:02:31 2023, max compression
+gzip compressed data, was "favicorn-0.0.5.tar", last modified: Fri Jul 14 08:14:43 2023, max compression
```

## Comparing `favicorn-0.0.4.tar` & `favicorn-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:02:31.743806 favicorn-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-29 10:02:31.743806 favicorn-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-29 10:02:02.000000 favicorn-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:02:31.743806 favicorn-0.0.4/favicorn/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-29 10:02:02.000000 favicorn-0.0.4/favicorn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-29 10:02:02.000000 favicorn-0.0.4/favicorn/connection_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-29 10:02:02.000000 favicorn-0.0.4/favicorn/iconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-29 10:02:02.000000 favicorn-0.0.4/favicorn/isocket_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:02:02.000000 favicorn-0.0.4/favicorn/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-29 10:02:02.000000 favicorn-0.0.4/favicorn/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-29 10:02:02.000000 favicorn-0.0.4/favicorn/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-29 10:02:02.000000 favicorn-0.0.4/favicorn/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-29 10:02:02.000000 favicorn-0.0.4/favicorn/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:02:31.743806 favicorn-0.0.4/favicorn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-29 10:02:31.000000 favicorn-0.0.4/favicorn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-29 10:02:31.000000 favicorn-0.0.4/favicorn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 10:02:31.000000 favicorn-0.0.4/favicorn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-29 10:02:31.000000 favicorn-0.0.4/favicorn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-29 10:02:31.000000 favicorn-0.0.4/favicorn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-29 10:02:02.000000 favicorn-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 10:02:31.743806 favicorn-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-29 10:02:02.000000 favicorn-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:14:43.634646 favicorn-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-14 08:14:43.634646 favicorn-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-14 08:14:34.000000 favicorn-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:14:43.626645 favicorn-0.0.5/favicorn/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:14:43.630645 favicorn-0.0.5/favicorn/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/builders/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/connection_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:14:43.630645 favicorn-0.0.5/favicorn/connections/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/connections/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:14:43.630645 favicorn-0.0.5/favicorn/connections/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/connections/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/connections/tcp/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:14:43.630645 favicorn-0.0.5/favicorn/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/controllers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:14:43.630645 favicorn-0.0.5/favicorn/controllers/asgi/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/controllers/asgi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/controllers/asgi/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/controllers/asgi/event_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/controllers/asgi/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/controllers/asgi/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/controllers/asgi/scope_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:14:43.630645 favicorn-0.0.5/favicorn/event_buses/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/event_buses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/event_buses/deque.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:14:43.630645 favicorn-0.0.5/favicorn/i/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/i/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/i/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/i/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/i/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/i/event_bus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:14:43.630645 favicorn-0.0.5/favicorn/i/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/i/protocols/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:14:43.630645 favicorn-0.0.5/favicorn/i/protocols/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/i/protocols/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/i/protocols/http/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/i/protocols/http/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/i/protocols/http/request_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/i/protocols/http/response_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/i/protocols/http/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:14:43.634646 favicorn-0.0.5/favicorn/i/protocols/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/i/protocols/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/i/protocols/websocket/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/i/protocols/websocket/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/i/protocols/websocket/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/i/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/i/socket_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:14:43.634646 favicorn-0.0.5/favicorn/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/protocols/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:14:43.634646 favicorn-0.0.5/favicorn/protocols/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/protocols/http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:14:43.634646 favicorn-0.0.5/favicorn/protocols/http/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/protocols/http/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:14:43.634646 favicorn-0.0.5/favicorn/protocols/http/parsers/h11_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/protocols/http/parsers/h11_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/protocols/http/parsers/h11_parser/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:14:43.634646 favicorn-0.0.5/favicorn/protocols/http/parsers/httptools_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/protocols/http/parsers/httptools_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/protocols/http/parsers/httptools_parser/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/protocols/http/parsers/httptools_parser/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:14:43.634646 favicorn-0.0.5/favicorn/protocols/http/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/protocols/http/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/protocols/http/serializers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:14:43.634646 favicorn-0.0.5/favicorn/protocols/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/protocols/websocket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:14:43.634646 favicorn-0.0.5/favicorn/protocols/websocket/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/protocols/websocket/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/protocols/websocket/parsers/wsproto_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:14:43.634646 favicorn-0.0.5/favicorn/protocols/websocket/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/protocols/websocket/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/protocols/websocket/serializers/wsproto_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:14:43.634646 favicorn-0.0.5/favicorn/socket_providers/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/socket_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/socket_providers/inet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/socket_providers/unix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-14 08:14:34.000000 favicorn-0.0.5/favicorn/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:14:43.630645 favicorn-0.0.5/favicorn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-14 08:14:43.000000 favicorn-0.0.5/favicorn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-07-14 08:14:43.000000 favicorn-0.0.5/favicorn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 08:14:43.000000 favicorn-0.0.5/favicorn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 08:14:43.000000 favicorn-0.0.5/favicorn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-14 08:14:34.000000 favicorn-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 08:14:43.634646 favicorn-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-14 08:14:34.000000 favicorn-0.0.5/setup.py
```

### Comparing `favicorn-0.0.4/favicorn/connection_manager.py` & `favicorn-0.0.5/favicorn/connection_manager.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import asyncio
 
-from .iconnection import IConnectionFactory
+from .i.connection import IConnectionFactory
 from .reader import SocketReader
 from .writer import SocketWriter
 
 
 class ConnectionManager:
     def __init__(
         self,
@@ -13,19 +13,17 @@
         self.connection_factory = connection_factory
 
     async def handler(
         self,
         stream_reader: asyncio.StreamReader,
         stream_writer: asyncio.StreamWriter,
     ) -> None:
-        reader = SocketReader(
-            stream_reader=stream_reader, default_read_count=4028
-        )
-        writer = SocketWriter(stream_writer=stream_writer)
         connection = self.connection_factory.build(
-            reader,
-            writer,
+            reader=SocketReader(
+                stream_reader=stream_reader, default_read_count=4028
+            ),
+            writer=SocketWriter(stream_writer=stream_writer),
         )
         try:
             await connection.main()
         finally:
             await connection.close()
```

### Comparing `favicorn-0.0.4/favicorn/reader.py` & `favicorn-0.0.5/favicorn/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,12 +33,12 @@
         if count is None:
             count = self.default_read_count
         data = await self.stream_reader.read(count)
         if self.stream_reader.at_eof():
             return None
         return data
 
-    async def wait(self, timeout: int | None = None) -> bool:
+    async def wait(self, timeout: float | None = None) -> bool:
         if data := await self.read(timeout=timeout, count=None):
             self.buffered_data = data
             return True
         return False
```

### Comparing `favicorn-0.0.4/favicorn/server.py` & `favicorn-0.0.5/favicorn/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import asyncio
 import logging
 
 from .connection_manager import ConnectionManager
-from .iconnection import IConnectionFactory
-from .isocket_provider import ISocketProvider
+from .i.connection import IConnectionFactory
+from .i.server import IServer
+from .i.socket_provider import ISocketProvider
 
 
-class Server:
+class Server(IServer):
     logger: logging.Logger
     socket_provider: ISocketProvider
     connection_factory: IConnectionFactory
 
     def __init__(
         self,
         socket_provider: ISocketProvider,
```

### Comparing `favicorn-0.0.4/favicorn/writer.py` & `favicorn-0.0.5/favicorn/writer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import asyncio
 
-from .utils import get_remote_addr
-
 
 class SocketWriter:
     stream_writer: asyncio.StreamWriter
 
     def __init__(self, stream_writer: asyncio.StreamWriter) -> None:
         self.stream_writer = stream_writer
 
@@ -17,15 +15,20 @@
         if not self.stream_writer.is_closing():
             await self.stream_writer.drain()
 
     def is_closing(self) -> bool:
         return self.stream_writer.is_closing()
 
     def get_address(self) -> tuple[str, int] | None:
-        return get_remote_addr(self.stream_writer)
+        if socket_info := self.stream_writer.get_extra_info("socket"):
+            if info := socket_info.getpeername():
+                return (str(info[0]), int(info[1]))
+        if info := self.stream_writer.get_extra_info("peername"):
+            return (str(info[0]), int(info[1]))
+        return None
 
     async def close(self) -> None:
         if self.stream_writer.is_closing():
             return
         if self.stream_writer.can_write_eof():
             self.stream_writer.write_eof()
         self.stream_writer.close()
```

### Comparing `favicorn-0.0.4/setup.py` & `favicorn-0.0.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 import os
 from pathlib import Path
 
-from setuptools import setup  # type: ignore [import]
+from setuptools import find_packages, setup  # type: ignore [import]
 
 
 setup(
     name="favicorn",
     version=os.environ["GITHUB_REF_NAME"],
     description="ASGI webserver",
     author="Vladimir Vojtenko",
     author_email="vladimirdev635@gmail.com",
     license="MIT",
-    packages=[
-        "favicorn",
-    ],
-    package_data={
-        "favicorn": ["py.typed"],
-    },
-    install_requires=["httptools", "asgiref"],
+    packages=find_packages(exclude=["__tests__*"]),
+    include_package_data=True,
     long_description=(Path(__file__).parent / "README.md").read_text(),
     long_description_content_type="text/markdown",
 )
```

