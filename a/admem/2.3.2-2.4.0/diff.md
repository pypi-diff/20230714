# Comparing `tmp/admem-2.3.2.tar.gz` & `tmp/admem-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "admem-2.3.2.tar", last modified: Tue May  2 21:09:52 2023, max compression
+gzip compressed data, was "admem-2.4.0.tar", last modified: Thu Jul 13 23:18:32 2023, max compression
```

## Comparing `admem-2.3.2.tar` & `admem-2.4.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 21:09:52.276428 admem-2.3.2/
--rw-rw-rw-   0 root         (0) root         (0)     1059 2023-05-02 14:46:08.000000 admem-2.3.2/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      351 2023-05-02 21:09:52.276428 admem-2.3.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      980 2023-05-02 21:09:52.276428 admem-2.3.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      144 2022-07-30 13:12:02.000000 admem-2.3.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 21:09:52.260427 admem-2.3.2/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 21:09:52.272428 admem-2.3.2/source/admem/
--rw-rw-rw-   0 root         (0) root         (0)      584 2023-05-02 21:02:37.000000 admem-2.3.2/source/admem/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1212 2023-05-02 14:46:09.000000 admem-2.3.2/source/admem/_backend_manager_proxy.py
--rw-rw-rw-   0 root         (0) root         (0)     6684 2023-05-02 14:46:09.000000 admem-2.3.2/source/admem/_create_django_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1575 2023-05-02 14:46:09.000000 admem-2.3.2/source/admem/_decorator.py
--rw-rw-rw-   0 root         (0) root         (0)     8282 2023-05-02 21:02:37.000000 admem-2.3.2/source/admem/_django_store.py
--rw-rw-rw-   0 root         (0) root         (0)     2350 2023-05-02 14:46:09.000000 admem-2.3.2/source/admem/_inspect_dataclass.py
--rw-rw-rw-   0 root         (0) root         (0)     2301 2023-05-02 21:02:37.000000 admem-2.3.2/source/admem/_path_proxy.py
--rw-rw-rw-   0 root         (0) root         (0)      641 2023-05-02 14:46:09.000000 admem-2.3.2/source/admem/_protocols.py
--rw-rw-rw-   0 root         (0) root         (0)     2960 2023-05-02 14:46:09.000000 admem-2.3.2/source/admem/_store_setup.py
--rw-rw-rw-   0 root         (0) root         (0)     2242 2023-05-02 14:46:09.000000 admem-2.3.2/source/admem/_sync_store.py
--rw-rw-rw-   0 root         (0) root         (0)      498 2023-05-02 14:46:09.000000 admem-2.3.2/source/admem/_util.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 14:46:09.000000 admem-2.3.2/source/admem/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 21:09:52.276428 admem-2.3.2/source/admem.egg-info/
--rw-r--r--   0 root         (0) root         (0)      351 2023-05-02 21:09:52.000000 admem-2.3.2/source/admem.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      593 2023-05-02 21:09:52.000000 admem-2.3.2/source/admem.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 21:09:52.000000 admem-2.3.2/source/admem.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 21:09:44.000000 admem-2.3.2/source/admem.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      232 2023-05-02 21:09:52.000000 admem-2.3.2/source/admem.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-02 21:09:52.000000 admem-2.3.2/source/admem.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 23:18:32.680537 admem-2.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1059 2023-07-13 22:37:10.000000 admem-2.4.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      351 2023-07-13 23:18:32.680537 admem-2.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      983 2023-07-13 23:18:32.684538 admem-2.4.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      144 2022-07-30 13:12:02.000000 admem-2.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 23:18:32.668537 admem-2.4.0/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 23:18:32.676537 admem-2.4.0/source/admem/
+-rw-rw-rw-   0 root         (0) root         (0)      584 2023-07-13 22:37:11.000000 admem-2.4.0/source/admem/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1792 2023-07-13 22:56:56.000000 admem-2.4.0/source/admem/_backend_manager_proxy.py
+-rw-rw-rw-   0 root         (0) root         (0)     6684 2023-07-13 22:37:11.000000 admem-2.4.0/source/admem/_create_django_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1575 2023-07-13 22:37:11.000000 admem-2.4.0/source/admem/_decorator.py
+-rw-rw-rw-   0 root         (0) root         (0)     9429 2023-07-13 22:53:28.000000 admem-2.4.0/source/admem/_django_store.py
+-rw-rw-rw-   0 root         (0) root         (0)     2350 2023-07-13 22:37:11.000000 admem-2.4.0/source/admem/_inspect_dataclass.py
+-rw-rw-rw-   0 root         (0) root         (0)     2301 2023-07-13 22:37:11.000000 admem-2.4.0/source/admem/_path_proxy.py
+-rw-rw-rw-   0 root         (0) root         (0)      747 2023-07-13 22:37:11.000000 admem-2.4.0/source/admem/_protocols.py
+-rw-rw-rw-   0 root         (0) root         (0)     2960 2023-07-13 22:37:11.000000 admem-2.4.0/source/admem/_store_setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     2242 2023-07-13 22:37:11.000000 admem-2.4.0/source/admem/_sync_store.py
+-rw-rw-rw-   0 root         (0) root         (0)      498 2023-07-13 22:37:11.000000 admem-2.4.0/source/admem/_util.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-13 22:37:11.000000 admem-2.4.0/source/admem/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 23:18:32.680537 admem-2.4.0/source/admem.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      351 2023-07-13 23:18:32.000000 admem-2.4.0/source/admem.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      593 2023-07-13 23:18:32.000000 admem-2.4.0/source/admem.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 23:18:32.000000 admem-2.4.0/source/admem.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 23:18:09.000000 admem-2.4.0/source/admem.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      235 2023-07-13 23:18:32.000000 admem-2.4.0/source/admem.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-07-13 23:18:32.000000 admem-2.4.0/source/admem.egg-info/top_level.txt
```

### Comparing `admem-2.3.2/LICENSE.txt` & `admem-2.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `admem-2.3.2/setup.cfg` & `admem-2.4.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -26,26 +26,26 @@
 [options.package_data]
 * = *.typed
 admem = 
 	source/admem/py.typed
 
 [options.extras_require]
 dev = 
-	adaux==2.4.4
-	pre-commit>=2.20
-	mypy==1.1.1
-	pylint==2.17.1
+	adaux==2.6.1
+	pre-commit>=3.3.3
+	mypy==1.4.1
+	pylint==2.17.4
 	django-stubs==1.12.0
 test = 
-	pytest>=7.2
+	pytest>=7.4
 	pytest-cov~=4.0
 docs = 
-	sphinx>=5.3.0
-	sphinx-rtd-theme>=1.0.0
-	sphinx-click>=4.3
+	sphinx>=6.2.1
+	sphinx-rtd-theme>=1.2.2
+	sphinx-click>=4.4.0
 	jupyter-sphinx>=0.4
 	bash_kernel>=0.8
 
 [tool:pytest]
 markers = 
 	merge_only: run test only on merge request
 addopts = --strict-markers -m "not merge_only"
```

### Comparing `admem-2.3.2/source/admem/__init__.py` & `admem-2.4.0/source/admem/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,8 +19,8 @@
     + _sync_store.__all__
     + _store_setup.__all__
     + _create_django_model.__all__
     + _inspect_dataclass.__all__
 )
 
 
-__version__ = "2.3.2"
+__version__ = "2.4.0"
```

### Comparing `admem-2.3.2/source/admem/_backend_manager_proxy.py` & `admem-2.4.0/source/admem/_backend_manager_proxy.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,29 +10,44 @@
 
 @dc.dataclass
 class BackendManagerProxy:
     backend: BackendStoreProtocol
     internal: tp.Any
     calls: list[str] = dc.field(default_factory=list)
 
+    _collect_only: tuple[str, ...] = tuple()
+    _collect_defer: tuple[str, ...] = tuple()
+
     def __getattr__(self, key: str) -> "BackendManagerProxy":
         self.calls.append(key)
         return self
 
     def __call__(self, *args: tp.Any, **kwgs: tp.Any) -> "BackendManagerProxy":
         assert self.calls
+        if self.calls[-1] == "only":
+            self._collect_defer = tuple()
+            self._collect_only = args
+        elif self.calls[-1] == "defer":
+            if len(args) == 1 and args[0] is None:
+                self._collect_defer = tuple()
+            else:
+                self._collect_defer += args
         self.internal = getattr(self.internal, self.calls[-1])(*args, **kwgs)
         return self
 
     def dci(self) -> tp.Iterator[tp.Any]:  # dataclass iterator
         if isinstance(self.internal, Iterable):
             for obj in self.internal:
-                yield self.backend.parse(obj)
+                yield self.backend.parse(
+                    obj, defer=self._collect_defer, only=self._collect_only
+                )
         else:
-            yield self.backend.parse(self.internal)
+            yield self.backend.parse(
+                self.internal, defer=self._collect_defer, only=self._collect_only
+            )
 
     def dcl(self) -> tp.Any | list[tp.Any]:  # dataclass list
         res = list(self.dci())
         if not isinstance(self.internal, Iterable):
             return res[0]
         return res
```

### Comparing `admem-2.3.2/source/admem/_create_django_model.py` & `admem-2.4.0/source/admem/_create_django_model.py`

 * *Files identical despite different names*

### Comparing `admem-2.3.2/source/admem/_decorator.py` & `admem-2.4.0/source/admem/_decorator.py`

 * *Files identical despite different names*

### Comparing `admem-2.3.2/source/admem/_django_store.py` & `admem-2.4.0/source/admem/_django_store.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (c) 2022-2023 Mario S. Könz; License: MIT
+import collections
 import dataclasses as dc
 import enum
 import types
 import typing as tp
 from pathlib import Path
 
 from django.core.files import File
@@ -137,22 +138,52 @@
         def inner(fieldfile: FieldFile) -> DjangoPath:
             assert fieldfile.name
             res = DjangoPath(fieldfile.name, prefix=prefix)
             return res
 
         return inner
 
-    def django_to_dataclass(self, dj_obj: models.Model) -> tp.Any:
+    @classmethod
+    def _true_key_and_subkey(
+        cls, keylist: tp.Iterable[str], is_only: bool = False
+    ) -> tuple[set[str], dict[str, set[str]]]:
+        subkeys = collections.defaultdict(set)
+        truekeys = set()
+        for key in keylist:
+            if "__" in key:
+                tkey, skey = key.split("__", 1)
+                if is_only:
+                    truekeys.add(tkey)
+                subkeys[tkey].add(skey)
+            else:
+                truekeys.add(key)
+        return truekeys, subkeys
+
+    def django_to_dataclass(  # pylint: disable=too-many-locals
+        self,
+        dj_obj: models.Model,
+        defer: tp.Iterable[str] = tuple(),
+        only: tp.Iterable[str] = tuple(),
+    ) -> tp.Any:
         dataclass = BACKEND_LINKER.backend_to_dc[type(dj_obj)]
-        obj_kwgs = {}
+        obj_kwgs: dict[str, tp.Any] = {}
+        true_defer, sub_defer = self._true_key_and_subkey(defer)
+        true_only, sub_only = self._true_key_and_subkey(only, is_only=True)
         for field in dc.fields(dataclass):
             key = field.name
+            if key in true_defer or (true_only and key not in true_only):
+                obj_kwgs[field.name] = None
+                continue
             val = getattr(dj_obj, key)
             if type(val) in BACKEND_LINKER.backend_to_dc:
-                val = self.django_to_dataclass(val)
+                val = self.django_to_dataclass(
+                    val,
+                    defer=sub_defer.get(field.name, set()),
+                    only=sub_only.get(field.name, set()),
+                )
 
             field_type = field.type
             origin = tp.get_origin(field_type)
             if origin:
                 # pylint: disable=protected-access
                 dj_field = dj_obj._meta.get_field(key)
                 if origin == types.UnionType:
```

### Comparing `admem-2.3.2/source/admem/_inspect_dataclass.py` & `admem-2.4.0/source/admem/_inspect_dataclass.py`

 * *Files identical despite different names*

### Comparing `admem-2.3.2/source/admem/_path_proxy.py` & `admem-2.4.0/source/admem/_path_proxy.py`

 * *Files identical despite different names*

### Comparing `admem-2.3.2/source/admem/_protocols.py` & `admem-2.4.0/source/admem/_protocols.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,15 +7,20 @@
 class BackendStoreProtocol(tp.Protocol):
     def dump(self, obj: T) -> tp.Any:
         pass  # pragma: no cover
 
     def load_all(self, dataclass: type[T], **filter_kwgs: tp.Any) -> tp.Iterator[T]:
         pass  # pragma: no cover
 
-    def parse(self, backend_obj: tp.Any) -> tp.Any:
+    def parse(
+        self,
+        backend_obj: tp.Any,
+        defer: tuple[str, ...] = tuple(),
+        only: tuple[str, ...] = tuple(),
+    ) -> tp.Any:
         pass  # pragma: no cover
 
     def backend_manager(self, dataclass: type[T]) -> tp.Any:
         pass  # pragma: no cover
 
     def reverse_set(self, obj: T, relation: str) -> set[tp.Any]:
         pass  # pragma: no cover
```

### Comparing `admem-2.3.2/source/admem/_store_setup.py` & `admem-2.4.0/source/admem/_store_setup.py`

 * *Files identical despite different names*

### Comparing `admem-2.3.2/source/admem/_sync_store.py` & `admem-2.4.0/source/admem/_sync_store.py`

 * *Files identical despite different names*

### Comparing `admem-2.3.2/source/admem.egg-info/SOURCES.txt` & `admem-2.4.0/source/admem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

