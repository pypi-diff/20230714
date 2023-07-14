# Comparing `tmp/packg-0.2.23.tar.gz` & `tmp/packg-0.2.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packg-0.2.23.tar", last modified: Fri Jul 14 12:42:20 2023, max compression
+gzip compressed data, was "packg-0.2.24.tar", last modified: Fri Jul 14 12:43:23 2023, max compression
```

## Comparing `packg-0.2.23.tar` & `packg-0.2.24.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-14 12:42:20.777480 packg-0.2.23/
--rw-------   0 gings    (14999) lmb-mit   (1061)    11336 2023-04-24 08:52:38.000000 packg-0.2.23/LICENSE
--rw-------   0 gings    (14999) lmb-mit   (1061)     2091 2023-07-14 12:42:20.777480 packg-0.2.23/PKG-INFO
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1295 2023-07-14 12:39:32.000000 packg-0.2.23/README.md
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     2337 2023-07-06 08:44:58.000000 packg-0.2.23/pyproject.toml
--rw-------   0 gings    (14999) lmb-mit   (1061)       96 2023-07-14 12:39:32.000000 packg-0.2.23/requirements.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       38 2023-07-14 12:42:20.781480 packg-0.2.23/setup.cfg
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-14 12:42:20.669477 packg-0.2.23/src/
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-14 12:42:20.729479 packg-0.2.23/src/packg/
--rw-------   0 gings    (14999) lmb-mit   (1061)      130 2023-07-14 12:42:00.000000 packg-0.2.23/src/packg/__init__.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      120 2023-07-14 12:39:32.000000 packg-0.2.23/src/packg/__main__.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     3107 2023-07-14 12:39:32.000000 packg-0.2.23/src/packg/caching.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     5770 2023-07-14 12:39:32.000000 packg-0.2.23/src/packg/constclass.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      530 2023-07-14 12:39:32.000000 packg-0.2.23/src/packg/debugging.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      470 2023-07-14 12:39:32.000000 packg-0.2.23/src/packg/dtime.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     8349 2023-07-14 12:39:32.000000 packg-0.2.23/src/packg/import_from_source.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-14 12:42:20.769479 packg-0.2.23/src/packg/iotools/
--rw-------   0 gings    (14999) lmb-mit   (1061)      707 2023-07-14 12:39:32.000000 packg-0.2.23/src/packg/iotools/__init__.py
--rw-------   0 gings    (14999) lmb-mit   (1061)      420 2023-07-14 12:39:32.000000 packg-0.2.23/src/packg/iotools/compressed.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      457 2023-07-14 12:39:32.000000 packg-0.2.23/src/packg/iotools/gitmatcher.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     6028 2023-07-14 12:39:32.000000 packg-0.2.23/src/packg/iotools/jsonext.py
--rw-------   0 gings    (14999) lmb-mit   (1061)    10555 2023-07-14 12:39:32.000000 packg-0.2.23/src/packg/iotools/jsonext_encoder.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     4014 2023-07-14 12:39:32.000000 packg-0.2.23/src/packg/iotools/misc.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     4840 2023-07-14 12:39:32.000000 packg-0.2.23/src/packg/iotools/yamlext.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     5915 2023-07-14 12:39:32.000000 packg-0.2.23/src/packg/log.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      394 2023-07-14 12:39:32.000000 packg-0.2.23/src/packg/misc.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     2420 2023-07-14 12:39:32.000000 packg-0.2.23/src/packg/packaging.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     2698 2023-07-14 12:39:32.000000 packg-0.2.23/src/packg/paths.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-14 12:42:20.773480 packg-0.2.23/src/packg/run/
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     3522 2023-07-14 12:39:32.000000 packg-0.2.23/src/packg/run/syncjupytext.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     5464 2023-07-14 12:39:32.000000 packg-0.2.23/src/packg/strings.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1988 2023-07-14 12:39:32.000000 packg-0.2.23/src/packg/system.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     1328 2023-07-14 12:39:32.000000 packg-0.2.23/src/packg/tensors.py
--rw-------   0 gings    (14999) lmb-mit   (1061)      527 2023-07-14 12:39:32.000000 packg-0.2.23/src/packg/typext.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-14 12:42:20.749479 packg-0.2.23/src/packg.egg-info/
--rw-------   0 gings    (14999) lmb-mit   (1061)     2091 2023-07-14 12:42:20.000000 packg-0.2.23/src/packg.egg-info/PKG-INFO
--rw-------   0 gings    (14999) lmb-mit   (1061)      808 2023-07-14 12:42:20.000000 packg-0.2.23/src/packg.egg-info/SOURCES.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-07-14 12:42:20.000000 packg-0.2.23/src/packg.egg-info/dependency_links.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       96 2023-07-14 12:42:20.000000 packg-0.2.23/src/packg.egg-info/requires.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        6 2023-07-14 12:42:20.000000 packg-0.2.23/src/packg.egg-info/top_level.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-28 06:28:28.000000 packg-0.2.23/src/packg.egg-info/zip-safe
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-14 12:43:23.518693 packg-0.2.24/
+-rw-------   0 gings    (14999) lmb-mit   (1061)    11336 2023-04-24 08:52:38.000000 packg-0.2.24/LICENSE
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2091 2023-07-14 12:43:23.518693 packg-0.2.24/PKG-INFO
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1295 2023-07-14 12:42:57.000000 packg-0.2.24/README.md
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     2337 2023-07-06 08:44:58.000000 packg-0.2.24/pyproject.toml
+-rw-------   0 gings    (14999) lmb-mit   (1061)       96 2023-07-14 12:42:57.000000 packg-0.2.24/requirements.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       38 2023-07-14 12:43:23.518693 packg-0.2.24/setup.cfg
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-14 12:43:23.430691 packg-0.2.24/src/
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-14 12:43:23.474692 packg-0.2.24/src/packg/
+-rw-------   0 gings    (14999) lmb-mit   (1061)      129 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/__init__.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      120 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/__main__.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     3097 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/caching.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     5871 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/constclass.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      544 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/debugging.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      470 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/dtime.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     8439 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/import_from_source.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-14 12:43:23.510693 packg-0.2.24/src/packg/iotools/
+-rw-------   0 gings    (14999) lmb-mit   (1061)      794 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/iotools/__init__.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)      420 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/iotools/compressed.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      457 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/iotools/gitmatcher.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     6252 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/iotools/jsonext.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)    10990 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/iotools/jsonext_encoder.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     4027 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/iotools/misc.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     4890 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/iotools/yamlext.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     5948 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/log.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      394 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/misc.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     2394 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/packaging.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2698 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/paths.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-14 12:43:23.514693 packg-0.2.24/src/packg/run/
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     3626 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/run/syncjupytext.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     5507 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/strings.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1968 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/system.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     1407 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/tensors.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)      527 2023-07-14 12:42:57.000000 packg-0.2.24/src/packg/typext.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-14 12:43:23.494692 packg-0.2.24/src/packg.egg-info/
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2091 2023-07-14 12:43:23.000000 packg-0.2.24/src/packg.egg-info/PKG-INFO
+-rw-------   0 gings    (14999) lmb-mit   (1061)      808 2023-07-14 12:43:23.000000 packg-0.2.24/src/packg.egg-info/SOURCES.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-07-14 12:43:23.000000 packg-0.2.24/src/packg.egg-info/dependency_links.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       96 2023-07-14 12:43:23.000000 packg-0.2.24/src/packg.egg-info/requires.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        6 2023-07-14 12:43:23.000000 packg-0.2.24/src/packg.egg-info/top_level.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-28 06:28:28.000000 packg-0.2.24/src/packg.egg-info/zip-safe
```

### Comparing `packg-0.2.23/LICENSE` & `packg-0.2.24/LICENSE`

 * *Files identical despite different names*

### Comparing `packg-0.2.23/PKG-INFO` & `packg-0.2.24/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packg
-Version: 0.2.23
+Version: 0.2.24
 Summary: Collection of utilities used in other python projects.
 Author: gingsi
 License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/packg
 Keywords: attrs,typing,dict,attr
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: packg Version: 0.2.23 Summary: Collection of
+Metadata-Version: 2.1 Name: packg Version: 0.2.24 Summary: Collection of
 utilities used in other python projects. Author: gingsi License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/packg Keywords:
 attrs,typing,dict,attr Platform: any Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `packg-0.2.23/README.md` & `packg-0.2.24/README.md`

 * *Files identical despite different names*

### Comparing `packg-0.2.23/pyproject.toml` & `packg-0.2.24/pyproject.toml`

 * *Files identical despite different names*

### Comparing `packg-0.2.23/src/packg/caching.py` & `packg-0.2.24/src/packg/caching.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,43 +7,47 @@
 
 
 class StoreNoNumpy(FileSystemStoreBackend):
     """
     Backend for joblib with pickle instead of numpy_pickle.
     Faster than the original backend for non-numpy objects (e.g. dicts).
     """
+
     NAME = "no_numpy"
 
     def load_item(self, path, verbose=1, msg=None):
         full_path = os.path.join(self.location, *path)
 
         if verbose > 1:
             if verbose < 10:
-                print(f'{msg}...')
+                print(f"{msg}...")
             else:
-                print(f'{msg} from {full_path}')
+                print(f"{msg} from {full_path}")
 
-        mmap_mode = (None if not hasattr(self, 'mmap_mode')
-                     else self.mmap_mode)
+        mmap_mode = None if not hasattr(self, "mmap_mode") else self.mmap_mode
 
-        filename = os.path.join(full_path, 'output.pkl')
+        filename = os.path.join(full_path, "output.pkl")
         if not self._item_exists(filename):
-            raise KeyError(f"Non-existing item (may have been cleared).\n"
-                           f"File {filename} does not exist")
+            raise KeyError(
+                f"Non-existing item (may have been cleared).\n"
+                f"File {filename} does not exist"
+            )
 
         assert mmap_mode is None, "Standard pickle does not support mmap_mode"
         with self._open_item(filename, "rb") as fh:
             item = pickle.load(fh)
         return item
 
 
 register_store_backend(StoreNoNumpy.NAME, StoreNoNumpy)
 
 
-def get_joblib_memory(location="cache_joblib", verbose=1, numpy_capable=False) -> joblib.Memory:
+def get_joblib_memory(
+    location="cache_joblib", verbose=1, numpy_capable=False
+) -> joblib.Memory:
     """
     Wrapper for joblib.Memory which uses the StoreNoNumpy backend by default.
 
     Args:
         location: cache dir
         verbose: higher = more verbose
         numpy_capable: keep False unless needed, it makes loading alot slower for e.g. dicts
@@ -68,16 +72,15 @@
         data_again = memory_cache.apply_memory_caching(cache_key, load_json, file)
         # Function is called once, then data is loaded from memory since cache_key exists.
     """
 
     def __init__(self):
         self._cache_dict = {}
 
-    def apply_memory_caching(
-            self, cache_key, func, *args, **kwargs):
+    def apply_memory_caching(self, cache_key, func, *args, **kwargs):
         cache_dict = self._cache_dict
         if cache_key is None:
             cache_key = joblib.hash((args, kwargs))
         if cache_key not in cache_dict:
             func_result = func(*args, **kwargs)
             cache_dict[cache_key] = func_result
         return cache_dict[cache_key]
```

### Comparing `packg-0.2.23/src/packg/constclass.py` & `packg-0.2.24/src/packg/constclass.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 import inspect
 from abc import ABCMeta, abstractmethod
 from typing import (
-    Iterator, Optional, List, ItemsView, KeysView, ValuesView, Any, Dict, Tuple, Union)
+    Iterator,
+    Optional,
+    List,
+    ItemsView,
+    KeysView,
+    ValuesView,
+    Any,
+    Dict,
+    Tuple,
+    Union,
+)
 
 
 class InstanceToClassDelegator(ABCMeta):
     """Metaclass to delegate instance methods to class methods, e.g.:
     __str__(MyClass) will call MyClass._class_str()."""
 
     def __str__(cls):
@@ -17,15 +27,17 @@
     def __iter__(cls):
         return cls._class_iter()  # noqa  # pylint: disable=no-value-for-parameter
 
     def __len__(cls):
         return cls._class_len()  # noqa  # pylint: disable=no-value-for-parameter
 
     def __instancecheck__(cls, instance):
-        return cls._class_instancecheck()  # noqa  # pylint: disable=no-value-for-parameter
+        return (
+            cls._class_instancecheck()
+        )  # noqa  # pylint: disable=no-value-for-parameter
 
     @abstractmethod
     def _class_str(cls):
         pass
 
     @abstractmethod
     def _class_repr(cls):
@@ -134,15 +146,15 @@
 
     @classmethod
     def _class_instancecheck(cls, instance):
         return isinstance(instance, str)
 
     @classmethod
     def __init_subclass__(
-            cls, allowed_types: Optional[Union[type, List[type], Tuple[type, ...]]] = None
+        cls, allowed_types: Optional[Union[type, List[type], Tuple[type, ...]]] = None
     ) -> None:
         """
         Setup properties for the public interface when this class is inherited.
 
         This will be called on nested inheritance as well.
 
         Args:
@@ -175,14 +187,17 @@
             # if allowed types is specified, make sure the value types are allowed
             if allowed_types is not None:
                 # isinstance errors when fed lists instead of tuple, so convert lists to tuples
                 if isinstance(allowed_types, list):
                     allowed_types = tuple(allowed_types)
                 if not isinstance(value, allowed_types):
                     raise TypeError(
-                        f"Constant: {key} in class: {cls.__name__} must be of type {allowed_types}")
+                        f"Constant: {key} in class: {cls.__name__} must be of type {allowed_types}"
+                    )
 
             # update class properties
             cls._dict[cls.__name__][key] = value
 
     def __init__(self) -> None:
-        raise RuntimeError(f"Do not instance this class, it's a Const: {type(self).__name__}")
+        raise RuntimeError(
+            f"Do not instance this class, it's a Const: {type(self).__name__}"
+        )
```

### Comparing `packg-0.2.23/src/packg/debugging.py` & `packg-0.2.24/src/packg/debugging.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import time
 
 
 def connect_to_debug_server(host=None, port=None):
     if host is None:
         return
     import pydevd_pycharm  # noqa  # pylint: disable=import-error
+
     if port is None:
         port = 12345
     while True:
         try:
             pydevd_pycharm.settrace(
-                host, port=port, stdoutToServer=True, stderrToServer=True, suspend=False)
+                host, port=port, stdoutToServer=True, stderrToServer=True, suspend=False
+            )
             break
         except ConnectionRefusedError:
             print(f"Debug server connection refused: {host}:{port}. Retrying...")
             time.sleep(2)
```

### Comparing `packg-0.2.23/src/packg/import_from_source.py` & `packg-0.2.24/src/packg/import_from_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,17 @@
     return len(components) >= 2 and components[1] == "tests"
 
 
 def _is_package(module_spec: ModuleSpec) -> bool:
     return module_spec.origin is not None and module_spec.origin.endswith("__init__.py")
 
 
-def _recurse_modules(module_name: str, ignore_tests: bool, packages_only: bool) -> Iterator[str]:
+def _recurse_modules(
+    module_name: str, ignore_tests: bool, packages_only: bool
+) -> Iterator[str]:
     if ignore_tests and _is_test_module(module_name):
         return
 
     module_spec = import_util.find_spec(module_name)
 
     if module_spec is not None and module_spec.origin is not None:
         if not (packages_only and not _is_package(module_spec)):
@@ -75,19 +77,23 @@
                     packages_only=packages_only,
                 )
             elif not packages_only:
                 yield f"{module_name}.{child.name}"
 
 
 class _ImportFromSourceChecker(NodeVisitor):
-    def __init__(self, module: str, module_list_to_ignore_not_found: Optional[List] = None):
+    def __init__(
+        self, module: str, module_list_to_ignore_not_found: Optional[List] = None
+    ):
         module_spec = import_util.find_spec(module)
-        is_pkg = (module_spec is not None
-                  and module_spec.origin is not None
-                  and module_spec.origin.endswith("__init__.py"))
+        is_pkg = (
+            module_spec is not None
+            and module_spec.origin is not None
+            and module_spec.origin.endswith("__init__.py")
+        )
 
         self._module = module if is_pkg else ".".join(module.split(".")[:-1])
         self._top_level_module = self._module.split(".")[0]
         self._module_list_to_ignore_not_found = module_list_to_ignore_not_found
 
     def visit_ImportFrom(self, node: ImportFrom) -> Any:
         # Check that there are no relative imports that attempt to read from a parent module. We've found that there
@@ -140,15 +146,17 @@
             if isinstance(attr, type) or callable(attr):
                 attribute_module = attr.__module__
             else:
                 continue
 
             # Figure out where we should be importing this class from, and assert that the *actual* import we found
             # matches the place we *should* import from.
-            should_import_from = self._get_module_should_import(module_to_import=attribute_module)
+            should_import_from = self._get_module_should_import(
+                module_to_import=attribute_module
+            )
             if module_to_import != should_import_from:
                 logging.warning(
                     f"(Potential false positive) "
                     f"Imported {alias.name} from {module_to_import}, "
                     f"which is not the public module where this object "
                     f"is defined. Please import from {should_import_from} instead."
                 )
@@ -160,15 +168,17 @@
         to actually take into account the fact that some submodules can be "private" (ie: start with an "_"), in
         which case we should only import from them if self._module is internal to that private module.
         """
         module_components = module_to_import.split(".")
         result: List[str] = []
 
         for component in module_components:
-            if component.startswith("_") and not self._module.startswith(".".join(result)):
+            if component.startswith("_") and not self._module.startswith(
+                ".".join(result)
+            ):
                 break
             result.append(component)
 
         return ".".join(result)
 
 
 def _apply_visitor(module: str, visitor: NodeVisitor) -> None:
```

### Comparing `packg-0.2.23/src/packg/iotools/jsonext.py` & `packg-0.2.24/src/packg/iotools/jsonext.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 
 from packg.iotools.compressed import load_xz
 from packg.iotools.jsonext_encoder import CustomJSONEncoder
 from packg.iotools.misc import open_file_or_io, read_text_from_file_or_io
 from packg.typext import PathOrIO, PathType
 
 
-def load_json(file_or_io: PathOrIO, verbose: bool = False, encoding: str = "utf-8") -> Any:
+def load_json(
+    file_or_io: PathOrIO, verbose: bool = False, encoding: str = "utf-8"
+) -> Any:
     """Load data from json file or file object"""
     start_timer = timer()
     data_str = read_text_from_file_or_io(file_or_io, encoding=encoding)
     try:
         obj = loads_json(data_str)
     except Exception as e:
         raise RuntimeError(f"Error loading json file {file_or_io}") from e
@@ -49,67 +51,105 @@
         This is inefficient for large files. In that case, iterate the file lines
         and use loads_json on each line.
     """
     data_str = read_text_from_file_or_io(file_or_io, encoding=encoding)
     try:
         data = loads_jsonl(data_str)
     except Exception as e:
-        raise RuntimeError(f"Error loading json file {file_or_io} (see reraised error)") from e
+        raise RuntimeError(
+            f"Error loading json file {file_or_io} (see reraised error)"
+        ) from e
     return data
 
 
 def loads_jsonl(s: str) -> List[Any]:
     data = []
     for i, line in enumerate(s.splitlines()):
         try:
             data.append(loads_json(line))
         except Exception as e:
             raise RuntimeError(f"Error loading json line {i}: {line}") from e
     return data
 
 
-def dump_json(obj: Any, file_or_io: PathOrIO, ensure_ascii: bool = False,
-              check_circular: bool = False, allow_nan=False, indent=None, separators=None,
-              sort_keys=False, verbose: bool = True, create_parent=False,
-              float_precision=None) -> None:
+def dump_json(
+    obj: Any,
+    file_or_io: PathOrIO,
+    ensure_ascii: bool = False,
+    check_circular: bool = False,
+    allow_nan=False,
+    indent=None,
+    separators=None,
+    sort_keys=False,
+    verbose: bool = True,
+    create_parent=False,
+    float_precision=None,
+) -> None:
     """Write data to json file or file object using the custom json encoder"""
     start_timer = timer()
-    with open_file_or_io(file_or_io, "wt", encoding="utf8", create_parent=create_parent) as fh:
+    with open_file_or_io(
+        file_or_io, "wt", encoding="utf8", create_parent=create_parent
+    ) as fh:
         if indent is None and separators is None:
             separators = (",", ":")
 
-        json.dump(obj, fh, cls=CustomJSONEncoder, ensure_ascii=ensure_ascii,
-                  check_circular=check_circular,
-                  allow_nan=allow_nan, indent=indent, separators=separators, sort_keys=sort_keys,
-                  float_precision=float_precision)
+        json.dump(
+            obj,
+            fh,
+            cls=CustomJSONEncoder,
+            ensure_ascii=ensure_ascii,
+            check_circular=check_circular,
+            allow_nan=allow_nan,
+            indent=indent,
+            separators=separators,
+            sort_keys=sort_keys,
+            float_precision=float_precision,
+        )
 
     if verbose:
         print(f"Wrote json file {file_or_io} in {timer() - start_timer:.3f} seconds")
 
 
-def dumps_json(obj: Any, ensure_ascii: bool = False,
-               check_circular: bool = False, allow_nan=False, indent=None, separators=None,
-               sort_keys=False, float_precision=None) -> str:
+def dumps_json(
+    obj: Any,
+    ensure_ascii: bool = False,
+    check_circular: bool = False,
+    allow_nan=False,
+    indent=None,
+    separators=None,
+    sort_keys=False,
+    float_precision=None,
+) -> str:
     """Write data to json string using the custom json encoder"""
-    return json.dumps(obj, cls=CustomJSONEncoder, ensure_ascii=ensure_ascii,
-                      check_circular=check_circular,
-                      allow_nan=allow_nan, indent=indent, separators=separators,
-                      sort_keys=sort_keys, float_precision=float_precision)
-
-
-def dump_jsonl(data: Iterable[Any], file_or_io: PathOrIO, verbose: bool = True,
-               create_parent=False) -> None:
+    return json.dumps(
+        obj,
+        cls=CustomJSONEncoder,
+        ensure_ascii=ensure_ascii,
+        check_circular=check_circular,
+        allow_nan=allow_nan,
+        indent=indent,
+        separators=separators,
+        sort_keys=sort_keys,
+        float_precision=float_precision,
+    )
+
+
+def dump_jsonl(
+    data: Iterable[Any], file_or_io: PathOrIO, verbose: bool = True, create_parent=False
+) -> None:
     """Write lines of data to jsonl (list of json strings) file or file object
     using the custom json encoder"""
     start_timer = timer()
     err_msg = f"data must be a list/sequence but is {type(data)}"
     assert not isinstance(data, str), err_msg
     assert isinstance(data, Sequence), err_msg
 
-    with open_file_or_io(file_or_io, "wt", encoding="utf8", create_parent=create_parent) as fh:
+    with open_file_or_io(
+        file_or_io, "wt", encoding="utf8", create_parent=create_parent
+    ) as fh:
         for d in data:
             fh.write(f"{dumps_json(d)}\n")
 
     if verbose:
         print(f"Wrote jsonl file {file_or_io} in {timer() - start_timer:.3f} seconds")
 
 
@@ -128,28 +168,44 @@
     except Exception as e:
         raise RuntimeError(f"Error loading json file {file}") from e
     if verbose:
         print(f"Loaded json file {file} in {timer() - start_timer:.3f} seconds")
     return obj
 
 
-def dump_json_xz(obj: Any, file: PathType, ensure_ascii: bool = False,
-                 check_circular: bool = False, allow_nan=False, indent=None, separators=None,
-                 sort_keys=False, verbose: bool = True, create_parent=False,
-                 float_precision=None) -> None:
+def dump_json_xz(
+    obj: Any,
+    file: PathType,
+    ensure_ascii: bool = False,
+    check_circular: bool = False,
+    allow_nan=False,
+    indent=None,
+    separators=None,
+    sort_keys=False,
+    verbose: bool = True,
+    create_parent=False,
+    float_precision=None,
+) -> None:
     start_timer = timer()
     file = Path(file)
     if create_parent:
         os.makedirs(file.parent, exist_ok=True)
     with lzma.open(file, "wt", encoding="utf8") as fh:
         try:
-            dump_json(obj, fh, ensure_ascii=ensure_ascii,
-                      check_circular=check_circular,
-                      allow_nan=allow_nan, indent=indent, separators=separators,
-                      sort_keys=sort_keys,
-                      verbose=verbose, create_parent=create_parent,
-                      float_precision=float_precision)
+            dump_json(
+                obj,
+                fh,
+                ensure_ascii=ensure_ascii,
+                check_circular=check_circular,
+                allow_nan=allow_nan,
+                indent=indent,
+                separators=separators,
+                sort_keys=sort_keys,
+                verbose=verbose,
+                create_parent=create_parent,
+                float_precision=float_precision,
+            )
         except Exception as e:
             raise RuntimeError(f"Error dumping json xz file {file}") from e
 
     if verbose:
         print(f"Wrote json xz file {file} in {timer() - start_timer:.3f} seconds")
```

### Comparing `packg-0.2.23/src/packg/iotools/jsonext_encoder.py` & `packg-0.2.24/src/packg/iotools/jsonext_encoder.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,35 @@
 """JSON encoder implementation for jsonext.py"""
 # pylint: skip-file
 import json
-from json.encoder import c_make_encoder, encode_basestring_ascii, encode_basestring, INFINITY
+from json.encoder import (
+    c_make_encoder,
+    encode_basestring_ascii,
+    encode_basestring,
+    INFINITY,
+)
 from pathlib import Path
 
 import numpy as np
 
 
 class CustomJSONEncoder(json.JSONEncoder):
-    def __init__(self, *, skipkeys=False, ensure_ascii=False,
-                 check_circular=True, allow_nan=False, sort_keys=False,
-                 indent=None, separators=None, default=None, float_precision=None):
+    def __init__(
+        self,
+        *,
+        skipkeys=False,
+        ensure_ascii=False,
+        check_circular=True,
+        allow_nan=False,
+        sort_keys=False,
+        indent=None,
+        separators=None,
+        default=None,
+        float_precision=None,
+    ):
         self.skipkeys = skipkeys
         self.ensure_ascii = ensure_ascii
         self.check_circular = check_circular
         self.allow_nan = allow_nan
         self.sort_keys = sort_keys
         self.indent = indent
         self.float_precision = float_precision
@@ -36,108 +51,148 @@
         if isinstance(o, np.ndarray):
             return o.tolist()
         if hasattr(o, "detach"):  # torch
             return o.detach().cpu().numpy().tolist()
         class_name = o.__class__.__name__
         if class_name.lower() == "devicearray":  # jax
             return o.tolist()
-        raise TypeError(f'Object of type {class_name} is not JSON serializable')
+        raise TypeError(f"Object of type {class_name} is not JSON serializable")
 
     def iterencode(self, o, _one_shot=False):
         # change: custom iterencode function called
         if self.check_circular:
             markers = {}
         else:
             markers = None
         if self.ensure_ascii:
             _encoder = encode_basestring_ascii
         else:
             _encoder = encode_basestring
 
-        def floatstr(obj, allow_nan=self.allow_nan,
-                     _repr=float.__repr__, _inf=INFINITY, _neginf=-INFINITY):
+        def floatstr(
+            obj,
+            allow_nan=self.allow_nan,
+            _repr=float.__repr__,
+            _inf=INFINITY,
+            _neginf=-INFINITY,
+        ):
             if obj != obj:
-                text = 'NaN'
+                text = "NaN"
             elif obj == _inf:
-                text = 'Infinity'
+                text = "Infinity"
             elif obj == _neginf:
-                text = '-Infinity'
+                text = "-Infinity"
             elif self.float_precision is not None:
-                return f'{obj:.{self.float_precision}f}'
+                return f"{obj:.{self.float_precision}f}"
             else:
                 return _repr(obj)
             if not allow_nan:
                 raise ValueError(
-                        "Out of range float values are not JSON compliant: " +
-                        repr(obj))
+                    "Out of range float values are not JSON compliant: " + repr(obj)
+                )
 
             return text
 
-        if (_one_shot and c_make_encoder is not None
-                and self.indent is None and self.float_precision is None):
+        if (
+            _one_shot
+            and c_make_encoder is not None
+            and self.indent is None
+            and self.float_precision is None
+        ):
             # only call the original c encoder if available and no custom iterencode logic is needed
             _iterencode = c_make_encoder(
-                    markers, self.default, _encoder, self.indent,
-                    self.key_separator, self.item_separator, self.sort_keys,
-                    self.skipkeys, self.allow_nan)
+                markers,
+                self.default,
+                _encoder,
+                self.indent,
+                self.key_separator,
+                self.item_separator,
+                self.sort_keys,
+                self.skipkeys,
+                self.allow_nan,
+            )
         else:
             _iterencode = _make_custom_iterencode(
-                    markers, self.default, _encoder, self.indent, floatstr,
-                    self.key_separator, self.item_separator, self.sort_keys,
-                    self.skipkeys, _one_shot)
+                markers,
+                self.default,
+                _encoder,
+                self.indent,
+                floatstr,
+                self.key_separator,
+                self.item_separator,
+                self.sort_keys,
+                self.skipkeys,
+                _one_shot,
+            )
         return _iterencode(o, 0)
 
 
 def _make_custom_iterencode(
-        markers, _default, _encoder, _indent, _floatstr, _key_separator, _item_separator,
-        _sort_keys, _skipkeys,
-        _one_shot,
-        # HACK: hand-optimized bytecode; turn globals into locals
-        ValueError=ValueError, dict=dict, float=float, id=id, int=int, isinstance=isinstance,
-        list=list, str=str,
-        tuple=tuple, _intstr=int.__repr__, indent_list: bool = False):
+    markers,
+    _default,
+    _encoder,
+    _indent,
+    _floatstr,
+    _key_separator,
+    _item_separator,
+    _sort_keys,
+    _skipkeys,
+    _one_shot,
+    # HACK: hand-optimized bytecode; turn globals into locals
+    ValueError=ValueError,
+    dict=dict,
+    float=float,
+    id=id,
+    int=int,
+    isinstance=isinstance,
+    list=list,
+    str=str,
+    tuple=tuple,
+    _intstr=int.__repr__,
+    indent_list: bool = False,
+):
     if _indent is not None and not isinstance(_indent, str):
-        _indent = ' ' * _indent
+        _indent = " " * _indent
 
     # change: no spaces at the end of lines
     _item_separator_eol = _item_separator.rstrip()
 
     def _iterencode_list(lst, _current_indent_level):
         if not lst:
-            yield '[]'
+            yield "[]"
             return
         if markers is not None:
             markerid = id(lst)
             if markerid in markers:
                 raise ValueError("Circular reference detected")
             markers[markerid] = lst
-        buf = '['
+        buf = "["
         # # change: use indent_list flag, use eol separator
         if _indent is not None and indent_list:
             _current_indent_level += 1
-            newline_indent = '\n' + _indent * _current_indent_level
+            newline_indent = "\n" + _indent * _current_indent_level
             separator = _item_separator_eol + newline_indent
             buf += newline_indent
         else:
             newline_indent = None
             separator = _item_separator
         first = True
         for value in lst:
             if first:
                 first = False
             else:
                 buf = separator
             if isinstance(value, str):
                 yield buf + _encoder(value)
             elif value is None:
-                yield buf + 'null'
+                yield buf + "null"
             elif value is True:
-                yield buf + 'true'
+                yield buf + "true"
             elif value is False:
-                yield buf + 'false'
+                yield buf + "false"
             elif isinstance(value, int):
                 # Subclasses of int/float may override __repr__, but we still
                 # want to encode them as integers/floats in JSON. One example
                 # within the standard library is IntEnum.
                 yield buf + _intstr(value)
             elif isinstance(value, float):
                 # see comment above for int
@@ -149,32 +204,32 @@
                 elif isinstance(value, dict):
                     chunks = _iterencode_dict(value, _current_indent_level)
                 else:
                     chunks = _iterencode(value, _current_indent_level)
                 yield from chunks
         if newline_indent is not None:
             _current_indent_level -= 1
-            yield '\n' + _indent * _current_indent_level
-        yield ']'
+            yield "\n" + _indent * _current_indent_level
+        yield "]"
         if markers is not None:
             del markers[markerid]
 
     def _iterencode_dict(dct, _current_indent_level):
         if not dct:
-            yield '{}'
+            yield "{}"
             return
         if markers is not None:
             markerid = id(dct)
             if markerid in markers:
                 raise ValueError("Circular reference detected")
             markers[markerid] = dct
-        yield '{'
+        yield "{"
         if _indent is not None:
             _current_indent_level += 1
-            newline_indent = '\n' + _indent * _current_indent_level
+            newline_indent = "\n" + _indent * _current_indent_level
             item_separator = _item_separator_eol + newline_indent
             yield newline_indent
         else:
             newline_indent = None
             item_separator = _item_separator
         first = True
         if _sort_keys:
@@ -186,41 +241,43 @@
                 pass
             # JavaScript is weakly typed for these, so it makes sense to
             # also allow them.  Many encoders seem to do something like this.
             elif isinstance(key, float):
                 # see comment for int/float in _make_iterencode
                 key = _floatstr(key)
             elif key is True:
-                key = 'true'
+                key = "true"
             elif key is False:
-                key = 'false'
+                key = "false"
             elif key is None:
-                key = 'null'
+                key = "null"
             elif isinstance(key, int):
                 # see comment for int/float in _make_iterencode
                 key = _intstr(key)
             elif _skipkeys:
                 continue
             else:
-                raise TypeError(f'keys must be str, int, float, bool or None, '
-                                f'not {key.__class__.__name__}')
+                raise TypeError(
+                    f"keys must be str, int, float, bool or None, "
+                    f"not {key.__class__.__name__}"
+                )
             if first:
                 first = False
             else:
                 yield item_separator
             yield _encoder(key)
             yield _key_separator
             if isinstance(value, str):
                 yield _encoder(value)
             elif value is None:
-                yield 'null'
+                yield "null"
             elif value is True:
-                yield 'true'
+                yield "true"
             elif value is False:
-                yield 'false'
+                yield "false"
             elif isinstance(value, int):
                 # see comment for int/float in _make_iterencode
                 yield _intstr(value)
             elif isinstance(value, float):
                 # see comment for int/float in _make_iterencode
                 yield _floatstr(value)
             else:
@@ -229,28 +286,28 @@
                 elif isinstance(value, dict):
                     chunks = _iterencode_dict(value, _current_indent_level)
                 else:
                     chunks = _iterencode(value, _current_indent_level)
                 yield from chunks
         if newline_indent is not None:
             _current_indent_level -= 1
-            yield '\n' + _indent * _current_indent_level
-        yield '}'
+            yield "\n" + _indent * _current_indent_level
+        yield "}"
         if markers is not None:
             del markers[markerid]
 
     def _iterencode(o, _current_indent_level):
         if isinstance(o, str):
             yield _encoder(o)
         elif o is None:
-            yield 'null'
+            yield "null"
         elif o is True:
-            yield 'true'
+            yield "true"
         elif o is False:
-            yield 'false'
+            yield "false"
         elif isinstance(o, int):
             # see comment for int/float in _make_iterencode
             yield _intstr(o)
         elif isinstance(o, float):
             # see comment for int/float in _make_iterencode
             yield _floatstr(o)
         elif isinstance(o, (list, tuple)):
```

### Comparing `packg-0.2.23/src/packg/iotools/misc.py` & `packg-0.2.24/src/packg/iotools/misc.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,24 +6,28 @@
 
 import natsort
 from packg.typext import PathOrIO, PathTypeCls, PathType
 
 
 @contextmanager
 def set_working_directory(path: Path):
-    """Change directory temporarily within in the context manager.
-    """
+    """Change directory temporarily within in the context manager."""
     origin = Path(os.getcwd()).absolute()
     os.chdir(path)
     yield
     os.chdir(origin)
 
 
 @contextmanager
-def open_file_or_io(file_or_io: PathOrIO, mode="r", encoding="utf-8", create_parent=False, ):
+def open_file_or_io(
+    file_or_io: PathOrIO,
+    mode="r",
+    encoding="utf-8",
+    create_parent=False,
+):
     should_close = False
     if isinstance(file_or_io, (str, PathTypeCls)):
         file_or_io = Path(file_or_io)
         if create_parent:
             os.makedirs(file_or_io.parent, exist_ok=True)
         fh = file_or_io.open(mode, encoding=encoding)
         should_close = True
@@ -58,15 +62,17 @@
         bytes content
     """
     if isinstance(file_or_io, PathTypeCls):
         return Path(file_or_io).read_bytes()
     return file_or_io.read()
 
 
-def yield_chunked_bytes(file_or_io: PathOrIO, chunk_size=1024 * 1024) -> Iterable[bytes]:
+def yield_chunked_bytes(
+    file_or_io: PathOrIO, chunk_size=1024 * 1024
+) -> Iterable[bytes]:
     """
 
     Args:
         file_or_io: file name or open file-like object
         chunk_size: chunk size in bytes, default 1MB
 
     Returns:
@@ -76,15 +82,17 @@
         while True:
             data = fh.read(chunk_size)
             if len(data) == 0:
                 break
             yield data
 
 
-def yield_nonempty_stripped_lines(lines_obj: Union[PathOrIO, Iterable[str]]) -> Iterable[str]:
+def yield_nonempty_stripped_lines(
+    lines_obj: Union[PathOrIO, Iterable[str]]
+) -> Iterable[str]:
     """
     Read lines from input, strip whitespaces, skip empty lines, yield lines.
 
     Args:
         lines_obj: Can be any of:
             - iterable of str (list, opened file)
             - filepath str or Path
@@ -103,16 +111,16 @@
             line = line.strip()
             if line == "":
                 continue
             yield line
 
 
 def sort_file_paths_with_dirs_separated(
-        file_paths: List[PathType], natsorted: bool = False,
-        dirs_first: bool = True) -> List[Path]:
+    file_paths: List[PathType], natsorted: bool = False, dirs_first: bool = True
+) -> List[Path]:
     """
     Sort a list of file paths, separating files inside subdirectories from files in the root.
 
     Only works for file paths (not directory paths) - input "dir/" will be treated like "dir"
     since in pathlib, Path("dir/") and Path("dir") are the same thing.
 
     Args:
```

### Comparing `packg-0.2.23/src/packg/iotools/yamlext.py` & `packg-0.2.24/src/packg/iotools/yamlext.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,30 +19,39 @@
     return loads_yaml(yaml_str)
 
 
 def loads_yaml(yaml_str: str) -> Any:
     return yaml.load(yaml_str, Loader=yaml.SafeLoader)
 
 
-def dump_yaml(obj: Any, file_or_io: PathOrIO, standard_format: bool = True,
-              check_roundtrip: bool = True, create_parent=False, **kwargs) -> None:
+def dump_yaml(
+    obj: Any,
+    file_or_io: PathOrIO,
+    standard_format: bool = True,
+    check_roundtrip: bool = True,
+    create_parent=False,
+    **kwargs,
+) -> None:
     """
     convert python object to yaml string and write to file. see dumps_yaml for details.
     """
-    s = dumps_yaml(obj, standard_format=standard_format, check_roundtrip=check_roundtrip, **kwargs)
+    s = dumps_yaml(
+        obj, standard_format=standard_format, check_roundtrip=check_roundtrip, **kwargs
+    )
     if isinstance(file_or_io, PathTypeCls):
         if create_parent:
             os.makedirs(Path(file_or_io).parent, exist_ok=True)
         Path(file_or_io).write_text(s, encoding="utf8")
         return
     file_or_io.write(s)
 
 
-def dumps_yaml(obj: Any, standard_format: bool = True, check_roundtrip: bool = True,
-               **kwargs) -> str:
+def dumps_yaml(
+    obj: Any, standard_format: bool = True, check_roundtrip: bool = True, **kwargs
+) -> str:
     """
     convert python object to yaml string
 
     Args:
         obj:
         standard_format:
             if True, use the standard yaml format
@@ -65,55 +74,59 @@
     if check_roundtrip:
         re_obj = loads_yaml(yaml_str)
 
         if re_obj != obj:
             print(f"---------- Original object:\n{obj}\n", file=sys.stderr)
             print(f"---------- Reconstructed object:\n{re_obj}\n", file=sys.stderr)
             raise RuntimeError(
-                "roundtrip failed (original object cannot be reconstructed from yaml, see stderr)")
+                "roundtrip failed (original object cannot be reconstructed from yaml, see stderr)"
+            )
     return yaml_str
 
 
 def _dumps_yaml_recursive(
-        obj: Any, indent: int = 4, _indent_level: int = 0,
-        _is_inside_list: bool = False) -> str:
+    obj: Any, indent: int = 4, _indent_level: int = 0, _is_inside_list: bool = False
+) -> str:
     """
     Modified version of yaml.dump with abbreviated lists and dicts.
     """
     # setup key-value collector and indent level
     indent = " " * (_indent_level * indent)
 
     # check type
     if isinstance(obj, (bool, int, float, type(None))):
         # by yaml standard, if there is only a single objects in the file, append "..." (eod)
         return _convert_single_object_to_yaml_str(
-            obj, remove_eod=_indent_level > 0 or _is_inside_list)
+            obj, remove_eod=_indent_level > 0 or _is_inside_list
+        )
     if isinstance(obj, str):
         # put quotes around strings
-        return f"\"{obj}\""
+        return f'"{obj}"'
     if is_any_mapping(obj):
         if _is_inside_list:
             # short: dicts inside lists will be kept in the abbreviated form: {key: "value"}
             if len(obj) == 0:
                 return "{}"
             dct_strs = ["{"]
             for sub_key, sub_val in obj.items():
-                dct_strs.append(f"{sub_key}: "
-                                f"{_dumps_yaml_recursive(sub_val, _is_inside_list=True)}")
+                dct_strs.append(
+                    f"{sub_key}: "
+                    f"{_dumps_yaml_recursive(sub_val, _is_inside_list=True)}"
+                )
                 dct_strs.append(", ")
             dct_strs.pop()
             dct_strs.append("}")
             return "".join(dct_strs)
         # long: build the dict line by line
         ret_list = []
         for k, v in obj.items():
             kv_sep = "\n" if isinstance(v, abc.Mapping) else " "
             recursive_result = _dumps_yaml_recursive(
-                v, _indent_level=_indent_level + 1,
-                _is_inside_list=_is_inside_list)
+                v, _indent_level=_indent_level + 1, _is_inside_list=_is_inside_list
+            )
             ret_list.append(f"{indent}{k}:{kv_sep}{recursive_result}")
         return "\n".join(ret_list)
     if is_any_iterable(obj):
         # iterate lists
         return f"[{', '.join((_dumps_yaml_recursive(v, _is_inside_list=True) for v in obj))}]"
     raise ValueError(f"dict to yaml, value type not understood: {obj}")
```

### Comparing `packg-0.2.23/src/packg/log.py` & `packg-0.2.24/src/packg/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,42 +19,44 @@
 
 from loguru import logger
 
 LevelType = Union[str, int]  # either "DEBUG" or 10
 DEFAULT_LOGURU_FORMAT = (
     "<green>{time:YYYY-MM-DD HH:mm:ss.SSS}</green> | <level>{level: <8}</level> | "
     "<cyan>{name}</cyan>:<cyan>{function}</cyan>:<cyan>{line}</cyan> - "
-    "<level>{message}</level>")
+    "<level>{message}</level>"
+)
 SHORTER_FORMAT = (
     "<green>{time:YYYYMMDD HH:mm:ss}</green> <level>{level: <4.4}</level> "
     "<cyan>{name}</cyan>:<cyan>{function}</cyan>:<cyan>{line}</cyan> "
-    "<level>{message}</level>")
+    "<level>{message}</level>"
+)
 SHORTEST_FORMAT = (
     "<green>{time:YYYYMMDD HH:mm:ss}</green> <level>{level: <4.4}</level> "
-    "<level>{message}</level>")
+    "<level>{message}</level>"
+)
 BRIGHTBG_FORMAT = (
     "<green>{time:YYYYMMDD HH:mm:ss}</green> <level>{level: <4.4}</level> "
     "<blue>{name}</blue>:<blue>{function}</blue>:<blue>{line}</blue> "
-    "<level>{message}</level>")
-TIMELESS_FORMAT = (
-    "<level>{level: <4.4}</level> "
-    "<level>{message}</level>")
+    "<level>{message}</level>"
+)
+TIMELESS_FORMAT = "<level>{level: <4.4}</level> " "<level>{message}</level>"
 
 
 global_logger_config = None
 
 
 def configure_logger(
-        level: LevelType = "DEBUG",
-        sink=sys.stderr,
-        format=SHORTEST_FORMAT,  # noqa # pylint: disable=redefined-builtin
-        colorize=True,
-        add_sinks: Optional[List[Any]] = None,
-        kwargs_handler: Optional[Dict[str, Any]] = None,
-        **kwargs: Any
+    level: LevelType = "DEBUG",
+    sink=sys.stderr,
+    format=SHORTEST_FORMAT,  # noqa # pylint: disable=redefined-builtin
+    colorize=True,
+    add_sinks: Optional[List[Any]] = None,
+    kwargs_handler: Optional[Dict[str, Any]] = None,
+    **kwargs: Any,
 ) -> Dict[str, Any]:
     """
     Configure the loguru logger. For more complex usages, use logger.configure() directly.
 
     Args:
         level: minimum level to log
         sink: where to write the logs to
@@ -73,36 +75,44 @@
 
     """
     add_sinks = add_sinks if add_sinks is not None else []
     kwargs_handler = kwargs_handler if kwargs_handler is not None else {}
     sinks = [sink] + add_sinks
     handlers = []
     for lsink in sinks:
-        params = {"sink": lsink, "format": format, "colorize": colorize,
-                  "level": get_level_as_str(level)}
+        params = {
+            "sink": lsink,
+            "format": format,
+            "colorize": colorize,
+            "level": get_level_as_str(level),
+        }
         assert "sink" not in kwargs_handler, f"sink is a reserved key, got {params}"
         params.update(deepcopy(kwargs_handler))
         if isinstance(lsink, str):
             # automatically disable color codes for files
             params["colorize"] = False
         handlers.append(params)
 
     # fix bug when combining colorama and loguru in conemu console on windows
-    if (colorize and os.name == "nt" and os.environ.get("CONEMUANSI") == "ON"
-            and sink in (sys.stderr, sys.stdout)):
+    if (
+        colorize
+        and os.name == "nt"
+        and os.environ.get("CONEMUANSI") == "ON"
+        and sink in (sys.stderr, sys.stdout)
+    ):
         print("\r", end="")  # the invisible print here magically fixes the color
 
     logger_config = {"handlers": handlers, **kwargs}
     logger.configure(**logger_config)
     global global_logger_config
     global_logger_config = logger_config
     return logger_config
 
 
-def reroute_logger(new_sink, logger_config=None,  handler_num: int = 0) -> None:
+def reroute_logger(new_sink, logger_config=None, handler_num: int = 0) -> None:
     """
     Reroute a sink from one target to another. Useful for proper logging inside
     a tqdm progressbar without having to recreate the entire logger.
 
     Args:
         new_sink: new target
         logger_config: config created by configure_logger() function above.
@@ -155,14 +165,15 @@
 def get_terminal_size() -> int:
     try:
         n_cols = os.get_terminal_size().columns
     except OSError:
         n_cols = 80
     return n_cols
 
+
 # # catch logs - code below will raise exceptions for logs. helpful for debugging where
 # # random logs are coming from
 # import logging
 #
 #
 # class CustomHandler(logging.Handler):
 #     def __init__(self):
```

### Comparing `packg-0.2.23/src/packg/packaging.py` & `packg-0.2.24/src/packg/packaging.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,20 +23,23 @@
     """
     main_file = Path(main_file)
     print(f"main_file: {main_file}")
     package_dir = main_file.parent
     package_name = package_dir.name
     package_scripts_dir = package_dir / run_dir
     glob_str = "**/*.py" if recursive else "*.py"
-    package_scripts = [f.relative_to(package_scripts_dir)
-                       for f in package_scripts_dir.glob(glob_str)
-                       if not f.name.startswith("__")]
-    sorted_scripts = sort_file_paths_with_dirs_separated(package_scripts, dirs_first=False)
-    package_scripts = [f.as_posix()[:-3].replace("/", ".")
-                       for f in sorted_scripts]
+    package_scripts = [
+        f.relative_to(package_scripts_dir)
+        for f in package_scripts_dir.glob(glob_str)
+        if not f.name.startswith("__")
+    ]
+    sorted_scripts = sort_file_paths_with_dirs_separated(
+        package_scripts, dirs_first=False
+    )
+    package_scripts = [f.as_posix()[:-3].replace("/", ".") for f in sorted_scripts]
     abbrevs = create_nested_abbreviations(package_scripts)
 
     args = sys.argv[1:]
     if len(args) > 0:
         abbrev_arg = args[0]
         if abbrev_arg in abbrevs:
             script = abbrevs[abbrev_arg]
@@ -67,8 +70,7 @@
 
 def run_script(target, args):
     print(f"Running {target}")
     module = importlib.import_module(target)
     main = getattr(module, "main")
     sys.argv = [sys.argv[0]] + args[1:]
     main()
-
```

### Comparing `packg-0.2.23/src/packg/paths.py` & `packg-0.2.24/src/packg/paths.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.23/src/packg/run/syncjupytext.py` & `packg-0.2.24/src/packg/run/syncjupytext.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,19 +17,22 @@
 from packg.log import SHORTEST_FORMAT, configure_logger, get_logger_level_from_args
 import time
 
 
 @define
 class Args(VerboseQuietArgs):
     base_dir: Optional[Path] = add_argument(
-        shortcut="-b", type=str, help="Source base dir", default=".")
+        shortcut="-b", type=str, help="Source base dir", default="."
+    )
     continuous: bool = add_argument(
-        shortcut="-c", action="store_true", help="Continuous mode")
+        shortcut="-c", action="store_true", help="Continuous mode"
+    )
     notebooks: bool = add_argument(
-        shortcut="-n", action="store_true", help="Create notebooks from scripts")
+        shortcut="-n", action="store_true", help="Create notebooks from scripts"
+    )
 
 
 def main():
     parser = TypedParser.create_parser(Args, description=__doc__)
     args: Args = parser.parse_args()
     configure_logger(level=get_logger_level_from_args(args), format=SHORTEST_FORMAT)
     logger.info(f"{args}")
@@ -67,15 +70,18 @@
                 files_to_update.append(file)
 
             current_time_str = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime())
             time_delta = timer() - start_timer
             current_timedelta_str = time.strftime("%H:%M:%S", time.gmtime(time_delta))
             tstr = f"{current_time_str} running for {current_timedelta_str} (round {n_rounds:4d})"
             if len(files_to_update) == 0:
-                print(f"{tstr}: Nothing to update.", end="\n" if n_rounds % 100 == 0 else "\r")
+                print(
+                    f"{tstr}: Nothing to update.",
+                    end="\n" if n_rounds % 100 == 0 else "\r",
+                )
             else:
                 print()
                 for file in files_to_update:
                     # convert to
                     logger.info(f"---------- Update {file}")
                     os.system(f"jupytext --to py:percent {file}")
                 os.makedirs(last_sync_file.parent, exist_ok=True)
@@ -85,13 +91,15 @@
                 print()
                 logger.info(f"Done updating {len(files_to_update)} files.")
             if not args.continuous:
                 break
             time.sleep(sleep)
 
         except (KeyboardInterrupt, AssertionError) as e:
-            logger.warning(f"\nInterrupted by user or file changes: {format_exception(e)}")
+            logger.warning(
+                f"\nInterrupted by user or file changes: {format_exception(e)}"
+            )
             break
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `packg-0.2.23/src/packg/strings.py` & `packg-0.2.24/src/packg/strings.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,21 @@
     """
 
     quoted = urllib.parse.quote(sentence, safe="")
     return f"{prefix}{quoted}"
 
 
 def unquote_with_urlparse(sentence: str, prefix="q") -> str:
-    sentence_no_prefix = sentence[len(prefix):]
+    sentence_no_prefix = sentence[len(prefix) :]
     return urllib.parse.unquote(sentence_no_prefix)
 
 
-def create_unique_abbreviations(input_strings: List[str], seps=("_", ".")) -> Dict[str, str]:
+def create_unique_abbreviations(
+    input_strings: List[str], seps=("_", ".")
+) -> Dict[str, str]:
     """
 
     Old version, splits input strings at "_" and "." and takes first letter of each word.
 
     lg         run.list_gpus
     pcbs       run.packaging.create_build_scripts
 
@@ -60,15 +62,17 @@
                     abbreviation = new_abbreviation
                     break
                 i += 1
         abbreviations[abbreviation] = name
     return abbreviations
 
 
-def create_nested_abbreviations(input_strings: List[str], sep_dir=".") -> Dict[str, str]:
+def create_nested_abbreviations(
+    input_strings: List[str], sep_dir="."
+) -> Dict[str, str]:
     """
     New version, keep the directory nesting and use minimal amount of letters
 
     l          run.list_gpus
     p.c        run.packaging.create_build_scripts
 
     Args:
@@ -141,13 +145,15 @@
             sub_stem_short = f"{stem_short}.{short_key}"
             sub_stem_long = f"{stem_long}.{long_key}"
             if key_is_leaf[long_key]:
                 # leaf node, return the short and long total stems
                 return_strs.append((sub_stem_short, sub_stem_long))
                 continue
             # non-leaf node, recurse
-            sub_strs = _recursive_shortcuts(dct_in[long_key], sub_stem_short, sub_stem_long)
+            sub_strs = _recursive_shortcuts(
+                dct_in[long_key], sub_stem_short, sub_stem_long
+            )
             return_strs.extend(sub_strs)
         return return_strs
 
     # finally cut the first "." and return the dict
     return {s[1:]: l[1:] for s, l in _recursive_shortcuts(dct)}
```

### Comparing `packg-0.2.23/src/packg/system.py` & `packg-0.2.24/src/packg/system.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,24 +14,25 @@
     Returns:
         stdout, stderr, returncode
     """
     pipe = subprocess.PIPE
     with subprocess.Popen(call, stdout=pipe, stderr=pipe, shell=True) as process:
         out, err = process.communicate()
         retcode = process.poll()
-    charset = 'utf-8'
+    charset = "utf-8"
     out = out.decode(charset)
     err = err.decode(charset)
     if verbose:
         print(f"out {out} err {err} ret {retcode}")
     return out, err, retcode
 
 
 def assert_command_worked(
-        errmsg: str, cmd: str, out: str, err: str, retcode: int) -> None:
+    errmsg: str, cmd: str, out: str, err: str, retcode: int
+) -> None:
     """Process the output of a systemcall and assert that the command worked.
 
     Args:
         errmsg: additional error info to display
         cmd: original command that was run (for display purposes)
         out: stdout of the command
         err: stderr of the command
@@ -40,19 +41,21 @@
     Returns:
         None
 
     """
     assert retcode == 0, (
         f"command failed: {cmd}\nout: {out}\nerr: {err}\n"
         f"retcode: {retcode}\n"
-        f"additional error info: {errmsg}")
+        f"additional error info: {errmsg}"
+    )
 
 
-def systemcall_with_assert(call: str, errmsg: str = "none", verbose: bool = False
-                           ) -> Tuple[str, str, int]:
+def systemcall_with_assert(
+    call: str, errmsg: str = "none", verbose: bool = False
+) -> Tuple[str, str, int]:
     """Run a command and assert it worked
 
     Args:
         call: command to run
         errmsg: additional error info to display when the command fails
         verbose: verbosity of the command
```

### Comparing `packg-0.2.23/src/packg/tensors.py` & `packg-0.2.24/src/packg/tensors.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,19 +8,20 @@
     if isinstance(inp, np.ndarray):
         return inp
     if hasattr(inp, "numpy"):
         return inp.numpy()
     return np.array(inp)
 
 
-def describe_stats(arr: TensorType,
-                   name: str = "",
-                   format_str: str = "{:.2f}",
-                   table_sep: Optional[str] = None,
-                   ) -> str:
+def describe_stats(
+    arr: TensorType,
+    name: str = "",
+    format_str: str = "{:.2f}",
+    table_sep: Optional[str] = None,
+) -> str:
     """
     See also lovely-tensors package for things like this
 
     Args:
         arr: array or tensor
         name: name of the tensor
         format_str: format string for printing
@@ -29,13 +30,26 @@
     """
     arr = ensure_numpy(arr)
     out_strs = []
     if table_sep is not None:
         fmt_str = table_sep.join([format_str] * 5)
         out_strs.append(f"{name}{table_sep}{len(arr)}{table_sep}")
     else:
-        fmt_str = ("Range: " + format_str + " to " + format_str + ", mean: " + format_str +
-                   ", std: " + format_str + ", median: " + format_str)
+        fmt_str = (
+            "Range: "
+            + format_str
+            + " to "
+            + format_str
+            + ", mean: "
+            + format_str
+            + ", std: "
+            + format_str
+            + ", median: "
+            + format_str
+        )
         out_strs.append(f"{name}: #{len(arr)}, ")
     out_strs.append(
-        fmt_str.format(np.min(arr), np.max(arr), np.mean(arr), np.std(arr), np.median(arr)))
+        fmt_str.format(
+            np.min(arr), np.max(arr), np.mean(arr), np.std(arr), np.median(arr)
+        )
+    )
     return "".join(out_strs)
```

### Comparing `packg-0.2.23/src/packg/typext.py` & `packg-0.2.24/src/packg/typext.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.23/src/packg.egg-info/PKG-INFO` & `packg-0.2.24/src/packg.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packg
-Version: 0.2.23
+Version: 0.2.24
 Summary: Collection of utilities used in other python projects.
 Author: gingsi
 License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/packg
 Keywords: attrs,typing,dict,attr
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: packg Version: 0.2.23 Summary: Collection of
+Metadata-Version: 2.1 Name: packg Version: 0.2.24 Summary: Collection of
 utilities used in other python projects. Author: gingsi License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/packg Keywords:
 attrs,typing,dict,attr Platform: any Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `packg-0.2.23/src/packg.egg-info/SOURCES.txt` & `packg-0.2.24/src/packg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

