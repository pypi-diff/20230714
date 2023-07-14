# Comparing `tmp/apispec_pydantic_plugin-0.2.2.tar.gz` & `tmp/apispec_pydantic_plugin-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apispec_pydantic_plugin-0.2.2.tar", max compression
+gzip compressed data, was "apispec_pydantic_plugin-0.3.0.tar", max compression
```

## Comparing `apispec_pydantic_plugin-0.2.2.tar` & `apispec_pydantic_plugin-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0      354 2023-01-27 18:49:59.069929 apispec_pydantic_plugin-0.2.2/README.md
--rw-r--r--   0        0        0     1631 2023-01-30 20:42:28.283313 apispec_pydantic_plugin-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      668 2023-01-31 02:45:06.844285 apispec_pydantic_plugin-0.2.2/src/apispec_pydantic_plugin/__init__.py
--rw-r--r--   0        0        0      310 2023-01-26 19:27:54.736758 apispec_pydantic_plugin-0.2.2/src/apispec_pydantic_plugin/errors.py
--rw-r--r--   0        0        0      547 2023-01-27 15:17:28.537048 apispec_pydantic_plugin-0.2.2/src/apispec_pydantic_plugin/models.py
--rw-r--r--   0        0        0        0 2023-01-26 14:55:59.355774 apispec_pydantic_plugin-0.2.2/src/apispec_pydantic_plugin/py.typed
--rw-r--r--   0        0        0     2307 2023-01-31 18:32:30.083348 apispec_pydantic_plugin-0.2.2/src/apispec_pydantic_plugin/pydantic_plugin.py
--rw-r--r--   0        0        0      896 2023-01-27 15:17:28.538407 apispec_pydantic_plugin-0.2.2/src/apispec_pydantic_plugin/registry.py
--rw-r--r--   0        0        0     9366 2023-01-31 18:32:30.084317 apispec_pydantic_plugin-0.2.2/src/apispec_pydantic_plugin/resolver.py
--rw-r--r--   0        0        0     1076 1970-01-01 00:00:00.000000 apispec_pydantic_plugin-0.2.2/setup.py
--rw-r--r--   0        0        0      792 1970-01-01 00:00:00.000000 apispec_pydantic_plugin-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      354 2023-07-14 18:50:40.271135 apispec_pydantic_plugin-0.3.0/README.md
+-rw-r--r--   0        0        0     1633 2023-07-14 19:09:58.637873 apispec_pydantic_plugin-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      628 2023-07-14 19:04:58.074159 apispec_pydantic_plugin-0.3.0/src/apispec_pydantic_plugin/__init__.py
+-rw-r--r--   0        0        0      310 2023-07-14 18:50:40.273116 apispec_pydantic_plugin-0.3.0/src/apispec_pydantic_plugin/errors.py
+-rw-r--r--   0        0        0      318 2023-07-14 19:04:58.075026 apispec_pydantic_plugin-0.3.0/src/apispec_pydantic_plugin/models.py
+-rw-r--r--   0        0        0        0 2023-07-14 18:50:40.273840 apispec_pydantic_plugin-0.3.0/src/apispec_pydantic_plugin/py.typed
+-rw-r--r--   0        0        0     2305 2023-07-14 19:04:58.076359 apispec_pydantic_plugin-0.3.0/src/apispec_pydantic_plugin/pydantic_plugin.py
+-rw-r--r--   0        0        0      896 2023-07-14 18:50:40.274630 apispec_pydantic_plugin-0.3.0/src/apispec_pydantic_plugin/registry.py
+-rw-r--r--   0        0        0     9366 2023-07-14 18:50:40.274943 apispec_pydantic_plugin-0.3.0/src/apispec_pydantic_plugin/resolver.py
+-rw-r--r--   0        0        0      789 1970-01-01 00:00:00.000000 apispec_pydantic_plugin-0.3.0/PKG-INFO
```

### Comparing `apispec_pydantic_plugin-0.2.2/pyproject.toml` & `apispec_pydantic_plugin-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [tool.poetry]
 name = "apispec-pydantic-plugin"
-version = "0.2.2"
+version = "0.3.0"
 description = ""
 authors = ["Kevin Kirsche <kevin.kirsche@one.verizon.com>"]
 readme = "README.md"
 packages = [{ include = "apispec_pydantic_plugin", from = "src" }]
 include = ["src/apispec_pydantic_plugin/py.typed"]
 
 [tool.poetry.dependencies]
-python = "^3.10"
-pydantic = ">=1.10.4,<2"
+python = ">=3.10,<4"
+pydantic = ">=2.0.3,<3"
 apispec = ">=6.0.2,<7"
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.12.0"
 example-isort-formatting-plugin = "^0.1.1"
 example-isort-sorting-plugin = "^0.1.0"
-black = {extras = ["toml"], version = "^22.12.0"}
-mypy = "^0.991"
-bandit = "^1.7.4"
+black = {extras = ["toml"], version = "^23.7.0"}
+mypy = "^1.4.1"
+bandit = "^1.7.5"
 flake8 = "^6.0.0"
-flake8-bugbear = "^23.1.20"
-flake8-pyi = "^23.1.1"
-codespell = "^2.2.2"
-pyupgrade = "^3.3.1"
-pytest = "^7.2.1"
+flake8-bugbear = "^23.7.10"
+flake8-pyi = "^23.6.0"
+codespell = "^2.2.5"
+pyupgrade = "^3.9.0"
+pytest = "^7.4.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 formatter = "example"
```

### Comparing `apispec_pydantic_plugin-0.2.2/src/apispec_pydantic_plugin/__init__.py` & `apispec_pydantic_plugin-0.3.0/src/apispec_pydantic_plugin/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from apispec_pydantic_plugin.errors import (
     ApispecPydanticPluginError,
     ApiSpecPydanticPluginKeyError,
     ApiSpecPydanticPluginValueError,
     ModelNotFoundError,
     ResolverNotFound,
 )
-from apispec_pydantic_plugin.models import ApiBaseModel, ApiGenericModel
+from apispec_pydantic_plugin.models import ApiBaseModel
 from apispec_pydantic_plugin.pydantic_plugin import PydanticPlugin
 from apispec_pydantic_plugin.registry import Registry
 
 # isort: unique-list
 __all__ = [
     "ApiBaseModel",
-    "ApiGenericModel",
     "ApiSpecPydanticPluginKeyError",
     "ApiSpecPydanticPluginValueError",
     "ApispecPydanticPluginError",
     "ModelNotFoundError",
     "PydanticPlugin",
     "Registry",
     "ResolverNotFound",
```

### Comparing `apispec_pydantic_plugin-0.2.2/src/apispec_pydantic_plugin/pydantic_plugin.py` & `apispec_pydantic_plugin-0.3.0/src/apispec_pydantic_plugin/pydantic_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             kwargs: All additional keyword arguments sent to `APISpec.schema()`
         """
         model: BaseModelAlias | None = kwargs.pop("model", None)
         if model:
             schema = model.schema(ref_template="#/components/schemas/{model}")
 
             if self.spec and "definitions" in schema:
-                for (k, v) in schema["definitions"].items():
+                for k, v in schema["definitions"].items():
                     with suppress(DuplicateComponentNameError):
                         self.spec.components.schema(k, v)
 
             if "definitions" in schema:
                 del schema["definitions"]
 
             return schema
```

### Comparing `apispec_pydantic_plugin-0.2.2/src/apispec_pydantic_plugin/registry.py` & `apispec_pydantic_plugin-0.3.0/src/apispec_pydantic_plugin/registry.py`

 * *Files identical despite different names*

### Comparing `apispec_pydantic_plugin-0.2.2/src/apispec_pydantic_plugin/resolver.py` & `apispec_pydantic_plugin-0.3.0/src/apispec_pydantic_plugin/resolver.py`

 * *Files identical despite different names*

### Comparing `apispec_pydantic_plugin-0.2.2/PKG-INFO` & `apispec_pydantic_plugin-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: apispec-pydantic-plugin
-Version: 0.2.2
+Version: 0.3.0
 Summary: 
 Author: Kevin Kirsche
 Author-email: kevin.kirsche@one.verizon.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.10,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: apispec (>=6.0.2,<7)
-Requires-Dist: pydantic (>=1.10.4,<2)
+Requires-Dist: pydantic (>=2.0.3,<3)
 Description-Content-Type: text/markdown
 
 
 # APISpec Pydantic Plugin
 
 This is a plugin that replaces `apispec.ext.marshmallow:MarshmallowPlugin` with an equivalent plugin for use with Pydantic.
```

