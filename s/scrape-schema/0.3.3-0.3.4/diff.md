# Comparing `tmp/scrape_schema-0.3.3.tar.gz` & `tmp/scrape_schema-0.3.4.tar.gz`

## Comparing `scrape_schema-0.3.3.tar` & `scrape_schema-0.3.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 scrape_schema-0.3.3/scrape_schema/__init__.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 scrape_schema-0.3.3/scrape_schema/_logger.py
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 scrape_schema-0.3.3/scrape_schema/_protocols.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 scrape_schema-0.3.3/scrape_schema/_typing.py
--rw-r--r--   0        0        0    12988 2020-02-02 00:00:00.000000 scrape_schema-0.3.3/scrape_schema/base.py
--rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 scrape_schema-0.3.3/scrape_schema/field.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 scrape_schema-0.3.3/scrape_schema/nested.py
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 scrape_schema-0.3.3/scrape_schema/type_caster.py
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 scrape_schema-0.3.3/scrape_schema/special_methods/__init__.py
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 scrape_schema-0.3.3/scrape_schema/special_methods/base.py
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 scrape_schema-0.3.3/scrape_schema/special_methods/methods.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scrape_schema-0.3.3/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 scrape_schema-0.3.3/LICENSE
--rw-r--r--   0        0        0    10563 2020-02-02 00:00:00.000000 scrape_schema-0.3.3/README.md
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 scrape_schema-0.3.3/pyproject.toml
--rw-r--r--   0        0        0    12494 2020-02-02 00:00:00.000000 scrape_schema-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 scrape_schema-0.3.4/scrape_schema/__init__.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 scrape_schema-0.3.4/scrape_schema/_logger.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 scrape_schema-0.3.4/scrape_schema/_protocols.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 scrape_schema-0.3.4/scrape_schema/_typing.py
+-rw-r--r--   0        0        0    13216 2020-02-02 00:00:00.000000 scrape_schema-0.3.4/scrape_schema/base.py
+-rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 scrape_schema-0.3.4/scrape_schema/field.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 scrape_schema-0.3.4/scrape_schema/nested.py
+-rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 scrape_schema-0.3.4/scrape_schema/type_caster.py
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 scrape_schema-0.3.4/scrape_schema/special_methods/__init__.py
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 scrape_schema-0.3.4/scrape_schema/special_methods/base.py
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 scrape_schema-0.3.4/scrape_schema/special_methods/methods.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scrape_schema-0.3.4/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 scrape_schema-0.3.4/LICENSE
+-rw-r--r--   0        0        0    10563 2020-02-02 00:00:00.000000 scrape_schema-0.3.4/README.md
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 scrape_schema-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0    12494 2020-02-02 00:00:00.000000 scrape_schema-0.3.4/PKG-INFO
```

### Comparing `scrape_schema-0.3.3/scrape_schema/_typing.py` & `scrape_schema-0.3.4/scrape_schema/_typing.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.3/scrape_schema/base.py` & `scrape_schema-0.3.4/scrape_schema/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,33 +15,32 @@
     SpecialMethodsHandler,
 )
 from scrape_schema.type_caster import TypeCaster
 
 
 class sc_param(property):
     """Shortcut for adding property-like descriptors in BaseSchema"""
-
-    pass
+    pass  # pragma: no cover
 
 
 class BaseField:
     def __init__(self, auto_type: bool = True, default: Any = ..., **kwargs):
         self._stack_methods: List[MarkupMethod] = []
         self.default = default
         self.auto_type = auto_type
         self.is_default = False  # flag check failed parsed value
         self._spec_method_handler: SpecialMethodsHandler = DEFAULT_SPEC_METHOD_HANDLER
 
     @abstractmethod
     def _prepare_markup(self, markup):
-        pass
+        pass  # pragma: no cover
 
     @abstractmethod
     def sc_parse(self, markup: Any):
-        pass
+        pass  # pragma: no cover
 
 
 class Field(BaseField):
     def _prepare_markup(self, markup: Union[str, bytes, Selector, SelectorList]):
         """convert string/bytes to parser class context"""
         if isinstance(markup, (Selector, SelectorList)):
             return markup
@@ -223,15 +222,15 @@
             return cls_schema
 
         # localns={} kwarg avoid TypeError 'function' object is not subscriptable
         for name, value in get_type_hints(
             cls_schema, localns={}, include_extras=True
         ).items():
             if name in ("__schema_fields__", "__schema_annotations__", "__parsers__"):
-                continue
+                continue  # pragma: no cover
             if mcs.__is_type_field(value):
                 field_type, field = mcs.__parse_annotated_field(value)
                 __schema_fields__[name] = field
                 __schema_annotations__[name] = field_type
 
         setattr(cls_schema, "__schema_fields__", __schema_fields__)
         setattr(cls_schema, "__schema_annotations__", __schema_annotations__)
@@ -241,15 +240,19 @@
 
 class BaseSchema(metaclass=SchemaMeta):
     class Config:
         selector_kwargs: Dict[str, Any] = {}
         type_caster: Optional[TypeCaster] = TypeCaster()  # TODO make interface
 
     @property
-    def __parser__(self) -> Union[Selector, SelectorList]:
+    def __sc_params__(self) -> Dict[str, Any]:
+        return {k: v for k, v in self.__dict__.items() if isinstance(v, sc_param)}
+
+    @property
+    def __selector__(self) -> Union[Selector, SelectorList]:
         return self._cached_parser
 
     @property
     def __raw__(self) -> str:
         return self._markup
 
     def __init__(self, markup: Any):
@@ -281,15 +284,15 @@
         for name, field in self.__schema_fields__.items():
             field_type = self.__schema_annotations__[name]
             _logger.debug("%s.%s start parse", self.__schema_name__, name)
             if field.__class__.__name__ == "Nested":  # todo fix
                 field.type_ = field_type
 
             # todo refactoring
-            value = field.sc_parse(self.__parser__)
+            value = field.sc_parse(self.__selector__)
 
             if self.Config.type_caster and field.auto_type and not field.is_default:
                 value = self.Config.type_caster.cast(field_type, value)
             # disable default value flag
             if field.is_default:
                 field.is_default = False
```

### Comparing `scrape_schema-0.3.3/scrape_schema/field.py` & `scrape_schema-0.3.4/scrape_schema/field.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.3/scrape_schema/nested.py` & `scrape_schema-0.3.4/scrape_schema/nested.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.3/scrape_schema/type_caster.py` & `scrape_schema-0.3.4/scrape_schema/type_caster.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,14 @@
+# pragma: no cover
 import sys
 from typing import Any, Type, Union
-
+from scrape_schema._typing import NoneType
 from scrape_schema._logger import _logger
 from scrape_schema._typing import get_args, get_origin
 
-NoneType = type(None)
-
 
 class TypeCaster:
     def _typing_to_builtin(self, type_hint: Type) -> Type:
         origin = get_origin(type_hint)
         args = get_args(type_hint)
 
         if origin is not None and args:
```

### Comparing `scrape_schema-0.3.3/scrape_schema/special_methods/__init__.py` & `scrape_schema-0.3.4/scrape_schema/special_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.3/scrape_schema/special_methods/base.py` & `scrape_schema-0.3.4/scrape_schema/special_methods/base.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.3/scrape_schema/special_methods/methods.py` & `scrape_schema-0.3.4/scrape_schema/special_methods/methods.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.3/.gitignore` & `scrape_schema-0.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.3/LICENSE` & `scrape_schema-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.3/README.md` & `scrape_schema-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.3/pyproject.toml` & `scrape_schema-0.3.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -83,15 +83,18 @@
 
 [tool.coverage.run]
 branch = true
 parallel = true
 omit = [
   "scrape_schema/__about__.py",
   "scrape_schema/factory/__init__.py",
-  "scrape_schema/_logger.py"
+  "scrape_schema/_logger.py",
+  "scrape_schema/_typing.py",
+  "scrape_schema/_protocols.py",
+  "scrape_schema/type_caster.py"
 ]
 
 [tool.coverage.report]
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
```

### Comparing `scrape_schema-0.3.3/PKG-INFO` & `scrape_schema-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrape-schema
-Version: 0.3.3
+Version: 0.3.4
 Summary: A library for converting any text (xml, html, plain text, stdout, etc) to python datatypes
 Project-URL: Documentation, https://github.com/vypivshiy/scrape-schema#readme
 Project-URL: Issues, https://github.com/vypivshiy/scrape-schema/issues
 Project-URL: Source, https://github.com/vypivshiy/scrape-schema
 Project-URL: Examples, https://github.com/vypivshiy/scrape-schema/examples
 Author: vypivshiy
 License-Expression: MIT
```

