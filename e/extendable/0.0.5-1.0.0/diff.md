# Comparing `tmp/extendable-0.0.5.tar.gz` & `tmp/extendable-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extendable-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "extendable-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `extendable-0.0.5.tar` & `extendable-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1081 2023-07-13 15:24:28.911025 extendable-0.0.5/LICENSE
--rw-r--r--   0        0        0     3245 2023-07-13 15:24:28.911025 extendable-0.0.5/README.md
--rw-r--r--   0        0        0     1457 2023-07-13 15:24:28.911025 extendable-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      393 2023-07-13 15:24:28.915025 extendable-0.0.5/src/extendable/__init__.py
--rw-r--r--   0        0        0      298 2023-07-13 15:24:28.915025 extendable-0.0.5/src/extendable/context.py
--rw-r--r--   0        0        0     9418 2023-07-13 15:24:28.915025 extendable-0.0.5/src/extendable/main.py
--rw-r--r--   0        0        0        0 2023-07-13 15:24:28.915025 extendable-0.0.5/src/extendable/py.typed
--rw-r--r--   0        0        0     8212 2023-07-13 15:24:28.915025 extendable-0.0.5/src/extendable/registry.py
--rw-r--r--   0        0        0     1059 2023-07-13 15:24:28.915025 extendable-0.0.5/src/extendable/utils.py
--rw-r--r--   0        0        0       22 2023-07-13 15:24:28.915025 extendable-0.0.5/src/extendable/version.py
--rw-r--r--   0        0        0     4248 1970-01-01 00:00:00.000000 extendable-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-07-14 16:30:24.882046 extendable-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3245 2023-07-14 16:30:24.882046 extendable-1.0.0/README.md
+-rw-r--r--   0        0        0     1457 2023-07-14 16:30:24.882046 extendable-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      393 2023-07-14 16:30:24.882046 extendable-1.0.0/src/extendable/__init__.py
+-rw-r--r--   0        0        0      332 2023-07-14 16:30:24.882046 extendable-1.0.0/src/extendable/context.py
+-rw-r--r--   0        0        0       55 2023-07-14 16:30:24.882046 extendable-1.0.0/src/extendable/exceptions.py
+-rw-r--r--   0        0        0     9975 2023-07-14 16:30:24.882046 extendable-1.0.0/src/extendable/main.py
+-rw-r--r--   0        0        0        0 2023-07-14 16:30:24.882046 extendable-1.0.0/src/extendable/py.typed
+-rw-r--r--   0        0        0     8212 2023-07-14 16:30:24.882046 extendable-1.0.0/src/extendable/registry.py
+-rw-r--r--   0        0        0     1059 2023-07-14 16:30:24.882046 extendable-1.0.0/src/extendable/utils.py
+-rw-r--r--   0        0        0       22 2023-07-14 16:30:24.882046 extendable-1.0.0/src/extendable/version.py
+-rw-r--r--   0        0        0     4248 1970-01-01 00:00:00.000000 extendable-1.0.0/PKG-INFO
```

### Comparing `extendable-0.0.5/LICENSE` & `extendable-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `extendable-0.0.5/README.md` & `extendable-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `extendable-0.0.5/pyproject.toml` & `extendable-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `extendable-0.0.5/src/extendable/main.py` & `extendable-1.0.0/src/extendable/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,22 @@
     from typing import OrderedDict
 else:
     from typing_extensions import OrderedDict
 
 from abc import ABCMeta
 
 from .context import extendable_registry
+from .exceptions import RegistryNotInitializedError
 
 _registry_build_mode = False
 if TYPE_CHECKING:
     from .registry import ExtendableClassesRegistry
 
+    AnyClassMethod = classmethod[Any, Any, Any]
+
 
 class ExtendableClassDef:
     name: str
     base_names: List[str]
     namespace: Dict[str, Any]
     original_name: str
     others_bases: List[Any]
@@ -186,44 +189,52 @@
     @classmethod
     def _wrap_class_methods(metacls, namespace: Dict[str, Any]) -> Dict[str, Any]:
         """Wrap classmethods defined into the namespace to delegate the call to the
         final class."""
         new_namespace: Dict[str, Any] = {}
         for key, value in namespace.items():
             if isinstance(value, classmethod):
-                func = value.__func__
-
-                @no_type_check
-                def new_method(
-                    cls, *args, _method_name=None, _initial_func=None, **kwargs
-                ):
-                    # ensure that arggs and kwargs are conform to the
-                    # initial signature
-                    inspect.signature(_initial_func).bind(cls, *args, **kwargs)
-                    try:
-                        return getattr(cls._get_assembled_cls(), _method_name)(
-                            *args, **kwargs
-                        )
-                    except KeyError:
-                        return _initial_func(cls, *args, **kwargs)
-
-                new_method_def = functools.partial(
-                    new_method, _method_name=key, _initial_func=func
-                )
-                # preserve signature for IDE
-                functools.update_wrapper(new_method_def, func)
-                new_namespace[key] = classmethod(new_method_def)
+                new_namespace[key] = metacls._wrap_class_method(value, key)
             else:
                 new_namespace[key] = value
         return new_namespace
 
     @classmethod
     def _is_extendable(metacls, cls: Type[Any]) -> bool:
         return issubclass(type(cls), ExtendableMeta)
 
+    @classmethod
+    def _wrap_class_method(
+        metacls, method: "AnyClassMethod", method_name: str
+    ) -> "AnyClassMethod":
+        """Wrap a class method to delegate the call to the final class.
+
+        In addition to preserve the signature and the docstring, this
+        method will also preserve the validation of args and kwargs
+        against the signature of the initial method at method call.
+        """
+        func = method.__func__
+
+        @no_type_check
+        def new_method(cls, *args, _method_name=None, _initial_func=None, **kwargs):
+            # ensure that args and kwargs are conform to the
+            # initial signature
+            inspect.signature(_initial_func).bind(cls, *args, **kwargs)
+            try:
+                return getattr(cls._get_assembled_cls(), _method_name)(*args, **kwargs)
+            except (RegistryNotInitializedError, KeyError):
+                return _initial_func(cls, *args, **kwargs)
+
+        new_method_def = functools.partial(
+            new_method, _method_name=method_name, _initial_func=func
+        )
+        # preserve signature for IDE
+        functools.update_wrapper(new_method_def, func)
+        return classmethod(new_method_def)
+
     @no_type_check
     def __call__(cls, *args, **kwargs) -> "ExtendableMeta":
         """Create the aggregated class in place of the original class definition.
 
         This method called at instance creation. The resulted instance
         will be an instance of the aggregated class not an instance of
         the original class definition since this definition could have
@@ -245,8 +256,12 @@
 
     def _get_assembled_cls(
         cls, registry: Optional["ExtendableClassesRegistry"] = None
     ) -> "ExtendableMeta":
         """An helper method to get the final class (the aggregated one) for the current
         class."""
         registry = registry if registry else extendable_registry.get()
+        if not registry:
+            raise RegistryNotInitializedError(
+                "Extendable classes registry is not initialized"
+            )
         return registry[cls.__xreg_name__]
```

### Comparing `extendable-0.0.5/src/extendable/registry.py` & `extendable-1.0.0/src/extendable/registry.py`

 * *Files identical despite different names*

### Comparing `extendable-0.0.5/src/extendable/utils.py` & `extendable-1.0.0/src/extendable/utils.py`

 * *Files identical despite different names*

### Comparing `extendable-0.0.5/PKG-INFO` & `extendable-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extendable
-Version: 0.0.5
+Version: 1.0.0
 Summary: A lib to define class extendable at runtime.
 Author-email: Laurent Mignon <laurent.mignon@acsone.eu>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

