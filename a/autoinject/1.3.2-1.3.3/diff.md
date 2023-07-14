# Comparing `tmp/autoinject-1.3.2.tar.gz` & `tmp/autoinject-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoinject-1.3.2.tar", last modified: Mon May 15 21:32:18 2023, max compression
+gzip compressed data, was "autoinject-1.3.3.tar", last modified: Fri Jul 14 14:03:08 2023, max compression
```

## Comparing `autoinject-1.3.2.tar` & `autoinject-1.3.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 21:32:18.034031 autoinject-1.3.2/
--rw-rw-rw-   0        0        0     1058 2023-05-15 17:40:59.000000 autoinject-1.3.2/LICENSE
--rw-rw-rw-   0        0        0     9942 2023-05-15 21:32:18.035024 autoinject-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     9324 2023-05-15 20:58:54.000000 autoinject-1.3.2/README.md
--rw-rw-rw-   0        0        0       88 2023-05-15 17:40:59.000000 autoinject-1.3.2/pyproject.toml
--rw-rw-rw-   0        0        0      809 2023-05-15 21:32:18.036023 autoinject-1.3.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-15 21:32:18.006023 autoinject-1.3.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-15 21:32:18.018087 autoinject-1.3.2/src/autoinject/
--rw-rw-rw-   0        0        0      496 2023-05-15 21:31:49.000000 autoinject-1.3.2/src/autoinject/__init__.py
--rw-rw-rw-   0        0        0      227 2023-05-15 17:40:59.000000 autoinject-1.3.2/src/autoinject/_tests.py
--rw-rw-rw-   0        0        0     7138 2023-05-15 20:33:47.000000 autoinject-1.3.2/src/autoinject/class_registry.py
--rw-rw-rw-   0        0        0     7469 2023-05-15 18:15:47.000000 autoinject-1.3.2/src/autoinject/context_manager.py
--rw-rw-rw-   0        0        0    11411 2023-05-15 19:37:38.000000 autoinject-1.3.2/src/autoinject/informants.py
--rw-rw-rw-   0        0        0    23632 2023-05-15 21:28:17.000000 autoinject-1.3.2/src/autoinject/injection.py
-drwxrwxrwx   0        0        0        0 2023-05-15 21:32:18.025023 autoinject-1.3.2/src/autoinject.egg-info/
--rw-rw-rw-   0        0        0     9942 2023-05-15 21:32:17.000000 autoinject-1.3.2/src/autoinject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      560 2023-05-15 21:32:18.000000 autoinject-1.3.2/src/autoinject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 21:32:17.000000 autoinject-1.3.2/src/autoinject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-15 21:32:17.000000 autoinject-1.3.2/src/autoinject.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-15 21:32:17.000000 autoinject-1.3.2/src/autoinject.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-15 21:32:18.033022 autoinject-1.3.2/tests/
--rw-rw-rw-   0        0        0    14330 2023-05-15 17:40:59.000000 autoinject-1.3.2/tests/test_context_manager.py
--rw-rw-rw-   0        0        0     1436 2023-05-15 18:38:39.000000 autoinject-1.3.2/tests/test_ep.py
--rw-rw-rw-   0        0        0    18157 2023-05-15 21:31:41.000000 autoinject-1.3.2/tests/test_injector.py
--rw-rw-rw-   0        0        0     2701 2023-05-15 17:40:59.000000 autoinject-1.3.2/tests/test_non_standard_injection.py
--rw-rw-rw-   0        0        0     3446 2023-05-15 20:18:25.000000 autoinject-1.3.2/tests/test_registry.py
--rw-rw-rw-   0        0        0     5175 2023-05-15 17:40:59.000000 autoinject-1.3.2/tests/test_threaded.py
+drwxrwxrwx   0        0        0        0 2023-07-14 14:03:08.238316 autoinject-1.3.3/
+-rw-rw-rw-   0        0        0     1058 2023-05-15 17:40:59.000000 autoinject-1.3.3/LICENSE
+-rw-rw-rw-   0        0        0    10142 2023-07-14 14:03:08.239275 autoinject-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     9524 2023-07-14 14:02:53.000000 autoinject-1.3.3/README.md
+-rw-rw-rw-   0        0        0       88 2023-05-15 17:40:59.000000 autoinject-1.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0      809 2023-07-14 14:03:08.240273 autoinject-1.3.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-14 14:03:08.207273 autoinject-1.3.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-14 14:03:08.222276 autoinject-1.3.3/src/autoinject/
+-rw-rw-rw-   0        0        0      496 2023-07-14 14:01:11.000000 autoinject-1.3.3/src/autoinject/__init__.py
+-rw-rw-rw-   0        0        0      227 2023-05-15 17:40:59.000000 autoinject-1.3.3/src/autoinject/_tests.py
+-rw-rw-rw-   0        0        0     7153 2023-07-14 14:00:35.000000 autoinject-1.3.3/src/autoinject/class_registry.py
+-rw-rw-rw-   0        0        0     7469 2023-05-15 18:15:47.000000 autoinject-1.3.3/src/autoinject/context_manager.py
+-rw-rw-rw-   0        0        0    11411 2023-05-15 19:37:38.000000 autoinject-1.3.3/src/autoinject/informants.py
+-rw-rw-rw-   0        0        0    24191 2023-07-14 14:02:09.000000 autoinject-1.3.3/src/autoinject/injection.py
+drwxrwxrwx   0        0        0        0 2023-07-14 14:03:08.228274 autoinject-1.3.3/src/autoinject.egg-info/
+-rw-rw-rw-   0        0        0    10142 2023-07-14 14:03:08.000000 autoinject-1.3.3/src/autoinject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      560 2023-07-14 14:03:08.000000 autoinject-1.3.3/src/autoinject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 14:03:08.000000 autoinject-1.3.3/src/autoinject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-07-14 14:03:08.000000 autoinject-1.3.3/src/autoinject.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-14 14:03:08.000000 autoinject-1.3.3/src/autoinject.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 14:03:08.237320 autoinject-1.3.3/tests/
+-rw-rw-rw-   0        0        0    14330 2023-05-15 17:40:59.000000 autoinject-1.3.3/tests/test_context_manager.py
+-rw-rw-rw-   0        0        0     1436 2023-05-15 18:38:39.000000 autoinject-1.3.3/tests/test_ep.py
+-rw-rw-rw-   0        0        0    18157 2023-05-15 21:31:41.000000 autoinject-1.3.3/tests/test_injector.py
+-rw-rw-rw-   0        0        0     2701 2023-05-15 17:40:59.000000 autoinject-1.3.3/tests/test_non_standard_injection.py
+-rw-rw-rw-   0        0        0     3446 2023-05-15 20:18:25.000000 autoinject-1.3.3/tests/test_registry.py
+-rw-rw-rw-   0        0        0     5175 2023-05-15 17:40:59.000000 autoinject-1.3.3/tests/test_threaded.py
```

### Comparing `autoinject-1.3.2/LICENSE` & `autoinject-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `autoinject-1.3.2/PKG-INFO` & `autoinject-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoinject
-Version: 1.3.2
+Version: 1.3.3
 Summary: Automated dependency injection for Python
 Home-page: https://github.com/turnbullerin/autoinject
 Author: Erin Turnbull
 Author-email: erin.a.turnbull@gmail.com
 Project-URL: Bug Tracker, https://github.com/turnbullerin/autoinject/issues
 Project-URL: Documentation, https://autoinject.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
@@ -150,14 +150,18 @@
 
 ```
 
 Read the [full documentation](https://autoinject.readthedocs.io/en/latest/?) for more details.
 
 ## Changelog
 
+### v1.3.3
+- Member lists of objects are now cached to prevent multiple calls to ``inspect.getmembers()`` when the 
+same class is created many times. This results in significant speed increases.
+
 ### v1.3.0
 - The new `@injector.test_case()` decorator is available for use with unit testing frameworks. It executes the decorated
   function with a different global and non-global context to ensure the independence of test functions. In addition, one
   can override the injected classes to provide specific test fixtures. These are passed as a dict of either `type` objects 
   or fully qualified class names as strings as keys and either the `type` or class name as string (to create the object), 
   or an object or function to use as the injected object.
 - A bug was fixed where exceptions within a context caused issues with the new contextvars integration.
```

### Comparing `autoinject-1.3.2/README.md` & `autoinject-1.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,18 @@
 
 ```
 
 Read the [full documentation](https://autoinject.readthedocs.io/en/latest/?) for more details.
 
 ## Changelog
 
+### v1.3.3
+- Member lists of objects are now cached to prevent multiple calls to ``inspect.getmembers()`` when the 
+same class is created many times. This results in significant speed increases.
+
 ### v1.3.0
 - The new `@injector.test_case()` decorator is available for use with unit testing frameworks. It executes the decorated
   function with a different global and non-global context to ensure the independence of test functions. In addition, one
   can override the injected classes to provide specific test fixtures. These are passed as a dict of either `type` objects 
   or fully qualified class names as strings as keys and either the `type` or class name as string (to create the object), 
   or an object or function to use as the injected object.
 - A bug was fixed where exceptions within a context caused issues with the new contextvars integration.
```

### Comparing `autoinject-1.3.2/setup.cfg` & `autoinject-1.3.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 7574 6f69 6e6a 6563 740d 0a76   = autoinject..v
-00000020: 6572 7369 6f6e 203d 2031 2e33 2e32 0d0a  ersion = 1.3.2..
+00000020: 6572 7369 6f6e 203d 2031 2e33 2e33 0d0a  ersion = 1.3.3..
 00000030: 6175 7468 6f72 203d 2045 7269 6e20 5475  author = Erin Tu
 00000040: 726e 6275 6c6c 0d0a 6175 7468 6f72 5f65  rnbull..author_e
 00000050: 6d61 696c 203d 2065 7269 6e2e 612e 7475  mail = erin.a.tu
 00000060: 726e 6275 6c6c 4067 6d61 696c 2e63 6f6d  rnbull@gmail.com
 00000070: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000080: 4175 746f 6d61 7465 6420 6465 7065 6e64  Automated depend
 00000090: 656e 6379 2069 6e6a 6563 7469 6f6e 2066  ency injection f
```

### Comparing `autoinject-1.3.2/src/autoinject/class_registry.py` & `autoinject-1.3.3/src/autoinject/class_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         """ Converts a type to a string that represents the fully-qualified name of the class.
         :param cls: Either a type to convert or a string representing the fully-qualified name of the class.
         :type cls: type OR str
         :return: Returns a string that could be used to import the class
         :rtype: str
         """
         info = str(cls)
-        if info.startswith("<class '"):
+        if len(info) > 10 and info[0:8] == "<class '":
             info = info[8:-2]
         return info
 
     def is_injectable(self, cls: type) -> bool:
         """ Checks if the given class is injectable
 
             :param cls: The class that is being checked
```

### Comparing `autoinject-1.3.2/src/autoinject/context_manager.py` & `autoinject-1.3.3/src/autoinject/context_manager.py`

 * *Files identical despite different names*

### Comparing `autoinject-1.3.2/src/autoinject/informants.py` & `autoinject-1.3.3/src/autoinject/informants.py`

 * *Files identical despite different names*

### Comparing `autoinject-1.3.2/src/autoinject/injection.py` & `autoinject-1.3.3/src/autoinject/injection.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,15 @@
         :meth:`autoinject.injection.InjectionManager.construct` decorator on the class's ``__init__()`` method. It will
         search for CLASS attributes with an injectable type-hint and inject the objects into the INSTANCE attributes
         as required.
     """
 
     def __init__(self, include_entry_points=True):
         """ Constructor """
+        self._members_cache = {}
         self.cls_registry = ClassRegistry(self)
         self.context_manager = ContextManager(self.cls_registry)
         # Register the class registry for injection, using the local instance
         self.cls_registry.register(
             ClassRegistry,
             constructor=lambda: self.cls_registry,
             caching_strategy=CacheStrategy.GLOBAL_CACHE
@@ -216,14 +217,15 @@
 
     def register_constructor(self, cls_name, constructor, *args, **kwargs):
         """ Wrapper around :meth:`autoinject.class_registry.ClassRegistry.register_class` """
         clear_cache = self.cls_registry.is_injectable(cls_name)
         self.cls_registry.register(cls_name, *args, constructor=constructor, **kwargs)
         if clear_cache:
             self.context_manager.clear_cache(cls_name)
+        self._members_cache = {}
 
     def get(self, cls_name):
         """ Wrapper around :meth:`autoinject.context_manager.ContextManager.get_object` """
         return self.context_manager.get_object(cls_name)
 
     def override(self, cls_name, new_constructor, *args, **kwargs):
         """ Override one class with another. """
@@ -377,24 +379,35 @@
                 def __init__(self):
                     pass
 
         """
         @wraps(func)
         def wrapper(*args, **kwargs):
             obj = args[0]  # self
-            type_map = self._get_bindable_attributes(obj.__class__)
-            for name, val in inspect.getmembers(obj.__class__):
-                if name[0:2] == "__":
-                    continue
-                if name in type_map and getattr(obj, name) is None:
-                    if self.cls_registry.is_injectable(type_map[name]):
-                        setattr(obj, name, self.context_manager.get_object(type_map[name]))
+            for attr_name, attr_type in self._get_bindable_members(obj.__class__):
+                if getattr(obj, attr_name) is None:
+                    setattr(obj, attr_name, self.context_manager.get_object(attr_type))
             return func(*args, **kwargs)
         return wrapper
 
+    def _get_bindable_members(self, cls: type) -> list[str, t.Union[type, str]]:
+        """Given a type, find all members we should check"""
+        if cls not in self._members_cache:
+            self._members_cache[cls] = []
+            type_map = self._get_bindable_attributes(cls)
+            for name, _ in inspect.getmembers(cls):
+                if name[0:2] == "__":
+                    continue
+                if name not in type_map:
+                    continue
+                if not self.cls_registry.is_injectable(type_map[name]):
+                    continue
+                self._members_cache[cls].append((name, type_map[name]))
+        return self._members_cache[cls]
+
     def _get_bindable_attributes(self, cls: type) -> dict:
         """Given a type, find all the bindable attributes using the annotations."""
         type_map = {}
         check_me = [cls, *cls.__mro__]
         for check_cls in check_me:
             if hasattr(check_cls, "__annotations__"):
                 for k in check_cls.__annotations__:
```

### Comparing `autoinject-1.3.2/src/autoinject.egg-info/PKG-INFO` & `autoinject-1.3.3/src/autoinject.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoinject
-Version: 1.3.2
+Version: 1.3.3
 Summary: Automated dependency injection for Python
 Home-page: https://github.com/turnbullerin/autoinject
 Author: Erin Turnbull
 Author-email: erin.a.turnbull@gmail.com
 Project-URL: Bug Tracker, https://github.com/turnbullerin/autoinject/issues
 Project-URL: Documentation, https://autoinject.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
@@ -150,14 +150,18 @@
 
 ```
 
 Read the [full documentation](https://autoinject.readthedocs.io/en/latest/?) for more details.
 
 ## Changelog
 
+### v1.3.3
+- Member lists of objects are now cached to prevent multiple calls to ``inspect.getmembers()`` when the 
+same class is created many times. This results in significant speed increases.
+
 ### v1.3.0
 - The new `@injector.test_case()` decorator is available for use with unit testing frameworks. It executes the decorated
   function with a different global and non-global context to ensure the independence of test functions. In addition, one
   can override the injected classes to provide specific test fixtures. These are passed as a dict of either `type` objects 
   or fully qualified class names as strings as keys and either the `type` or class name as string (to create the object), 
   or an object or function to use as the injected object.
 - A bug was fixed where exceptions within a context caused issues with the new contextvars integration.
```

### Comparing `autoinject-1.3.2/src/autoinject.egg-info/SOURCES.txt` & `autoinject-1.3.3/src/autoinject.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autoinject-1.3.2/tests/test_context_manager.py` & `autoinject-1.3.3/tests/test_context_manager.py`

 * *Files identical despite different names*

### Comparing `autoinject-1.3.2/tests/test_ep.py` & `autoinject-1.3.3/tests/test_ep.py`

 * *Files identical despite different names*

### Comparing `autoinject-1.3.2/tests/test_injector.py` & `autoinject-1.3.3/tests/test_injector.py`

 * *Files identical despite different names*

### Comparing `autoinject-1.3.2/tests/test_non_standard_injection.py` & `autoinject-1.3.3/tests/test_non_standard_injection.py`

 * *Files identical despite different names*

### Comparing `autoinject-1.3.2/tests/test_registry.py` & `autoinject-1.3.3/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `autoinject-1.3.2/tests/test_threaded.py` & `autoinject-1.3.3/tests/test_threaded.py`

 * *Files identical despite different names*

