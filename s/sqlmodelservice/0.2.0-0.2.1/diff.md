# Comparing `tmp/sqlmodelservice-0.2.0.tar.gz` & `tmp/sqlmodelservice-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlmodelservice-0.2.0.tar", max compression
+gzip compressed data, was "sqlmodelservice-0.2.1.tar", max compression
```

## Comparing `sqlmodelservice-0.2.0.tar` & `sqlmodelservice-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1067 2023-07-12 09:20:54.866634 sqlmodelservice-0.2.0/LICENSE
--rw-r--r--   0        0        0      576 2023-07-12 11:17:33.572050 sqlmodelservice-0.2.0/README.md
--rw-r--r--   0        0        0     2262 2023-07-12 11:21:36.700418 sqlmodelservice-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      190 2023-07-12 11:21:21.352388 sqlmodelservice-0.2.0/sqlmodelservice/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 09:26:53.250669 sqlmodelservice-0.2.0/sqlmodelservice/py.typed
--rw-r--r--   0        0        0     9318 2023-07-12 09:52:04.659296 sqlmodelservice-0.2.0/sqlmodelservice/service.py
--rw-r--r--   0        0        0     1305 1970-01-01 00:00:00.000000 sqlmodelservice-0.2.0/setup.py
--rw-r--r--   0        0        0     1062 1970-01-01 00:00:00.000000 sqlmodelservice-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-12 09:20:54.866634 sqlmodelservice-0.2.1/LICENSE
+-rw-r--r--   0        0        0      714 2023-07-12 21:04:10.450474 sqlmodelservice-0.2.1/README.md
+-rw-r--r--   0        0        0     2287 2023-07-14 09:39:44.771106 sqlmodelservice-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      190 2023-07-12 11:21:21.352388 sqlmodelservice-0.2.1/sqlmodelservice/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 09:26:53.250669 sqlmodelservice-0.2.1/sqlmodelservice/py.typed
+-rw-r--r--   0        0        0     9300 2023-07-14 09:39:07.166960 sqlmodelservice-0.2.1/sqlmodelservice/service.py
+-rw-r--r--   0        0        0     1445 1970-01-01 00:00:00.000000 sqlmodelservice-0.2.1/setup.py
+-rw-r--r--   0        0        0     1200 1970-01-01 00:00:00.000000 sqlmodelservice-0.2.1/PKG-INFO
```

### Comparing `sqlmodelservice-0.2.0/LICENSE` & `sqlmodelservice-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlmodelservice-0.2.0/README.md` & `sqlmodelservice-0.2.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # SQLModelService
 
-`SQLModelService` is a generic service layer on top of `SQLModel` for conveniently creating APIs with frameworks like [FastAPI](https://fastapi.tiangolo.com/).
+`SQLModelService` is a generic service layer on top of [SQLModel](https://sqlmodel.tiangolo.com/) for conveniently creating APIs with frameworks like [FastAPI](https://fastapi.tiangolo.com/).
+
+See the [documentation](https://volfpeter.github.io/sqlmodelservice) for examples and the API reference.
 
 ## Installation
 
 The library is available on PyPI and can be installed with:
 
 ```console
 $ pip install sqlmodelservice
```

### Comparing `sqlmodelservice-0.2.0/pyproject.toml` & `sqlmodelservice-0.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 [project]
+name = "sqlmodelservice"
 readme = "README.md"
 license = { text = "MIT" }
 classifiers = [
     "Intended Audience :: Information Technology",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
@@ -19,15 +20,15 @@
 
 [project.urls]
 Homepage = "https://github.com/volfpeter/sqlmodelservice"
 Documentation = "https://volfpeter.github.io/sqlmodelservice"
 
 [tool.poetry]
 name = "sqlmodelservice"
-version = "0.2.0"
+version = "0.2.1"
 description = "A generic service layer on top of SQLModel for conveniently creating APIs with frameworks like FastAPI."
 authors = ["Peter Volf <do.volfp@gmail.com>"]
 readme = "README.md"
 packages = [{include = "sqlmodelservice"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `sqlmodelservice-0.2.0/sqlmodelservice/service.py` & `sqlmodelservice-0.2.1/sqlmodelservice/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,15 @@
 from typing import Any, Generic, Type, TypeVar, overload
 
 from sqlmodel import Session, SQLModel, select
 from sqlmodel.engine.result import Result, ScalarResult
 from sqlmodel.sql.expression import SelectOfScalar
 
 AtomicPrimaryKey = int | str
-PrimaryKey = (
-    AtomicPrimaryKey
-    | tuple[AtomicPrimaryKey, ...]
-    | list[AtomicPrimaryKey]
-    | Mapping[str, AtomicPrimaryKey]
-)
+PrimaryKey = AtomicPrimaryKey | tuple[AtomicPrimaryKey, ...] | list[AtomicPrimaryKey] | Mapping[str, AtomicPrimaryKey]
 
 T = TypeVar("T")
 TM_1 = TypeVar("TM_1", bound=SQLModel)
 TM_2 = TypeVar("TM_2", bound=SQLModel)
 TM_3 = TypeVar("TM_3", bound=SQLModel)
 TM_4 = TypeVar("TM_4", bound=SQLModel)
 
@@ -150,17 +145,15 @@
         ...
 
     @overload
     def select(self, joined_1: Type[TM_1], /) -> SelectOfScalar[tuple[TModel, TM_1]]:
         ...
 
     @overload
-    def select(
-        self, joined_1: Type[TM_1], joined_2: Type[TM_2], /
-    ) -> SelectOfScalar[tuple[TModel, TM_1, TM_2]]:
+    def select(self, joined_1: Type[TM_1], joined_2: Type[TM_2], /) -> SelectOfScalar[tuple[TModel, TM_1, TM_2]]:
         ...
 
     @overload
     def select(
         self, joined_1: Type[TM_1], joined_2: Type[TM_2], joined_3: Type[TM_3], /
     ) -> SelectOfScalar[tuple[TModel, TM_1, TM_2, TM_3]]:
         ...
@@ -249,15 +242,15 @@
 
         Raises:
             ValueError: If formatting fails.
         """
         if isinstance(pk, (str, int)):
             return str(pk)
         elif isinstance(pk, (tuple, list)):
-            return "|".join(pk)
+            return "|".join(str(i) for i in pk)
         elif isinstance(pk, dict):
             return "|".join(f"{k}:{v}" for k, v in pk.items())
 
         raise ValueError("Unrecognized primary key type.")
 
     def _prepare_for_create(self, data: TCreate) -> TModel:
         """
```

### Comparing `sqlmodelservice-0.2.0/setup.py` & `sqlmodelservice-0.2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['sqlmodel>=0.0.8,<0.0.9']
 
 setup_kwargs = {
     'name': 'sqlmodelservice',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'A generic service layer on top of SQLModel for conveniently creating APIs with frameworks like FastAPI.',
-    'long_description': '# SQLModelService\n\n`SQLModelService` is a generic service layer on top of `SQLModel` for conveniently creating APIs with frameworks like [FastAPI](https://fastapi.tiangolo.com/).\n\n## Installation\n\nThe library is available on PyPI and can be installed with:\n\n```console\n$ pip install sqlmodelservice\n```\n\n## Dependencies\n\nThe only direct dependency of the project -- as the name suggests -- is `SQLModel`.\n\n## Contributing\n\nContributions are welcome.\n\n## License\n\nThe library is open-sourced under the conditions of the [MIT license](https://choosealicense.com/licenses/mit/).\n',
+    'long_description': '# SQLModelService\n\n`SQLModelService` is a generic service layer on top of [SQLModel](https://sqlmodel.tiangolo.com/) for conveniently creating APIs with frameworks like [FastAPI](https://fastapi.tiangolo.com/).\n\nSee the [documentation](https://volfpeter.github.io/sqlmodelservice) for examples and the API reference.\n\n## Installation\n\nThe library is available on PyPI and can be installed with:\n\n```console\n$ pip install sqlmodelservice\n```\n\n## Dependencies\n\nThe only direct dependency of the project -- as the name suggests -- is `SQLModel`.\n\n## Contributing\n\nContributions are welcome.\n\n## License\n\nThe library is open-sourced under the conditions of the [MIT license](https://choosealicense.com/licenses/mit/).\n',
     'author': 'Peter Volf',
     'author_email': 'do.volfp@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `sqlmodelservice-0.2.0/PKG-INFO` & `sqlmodelservice-0.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: sqlmodelservice
-Version: 0.2.0
+Version: 0.2.1
 Summary: A generic service layer on top of SQLModel for conveniently creating APIs with frameworks like FastAPI.
 Author: Peter Volf
 Author-email: do.volfp@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: sqlmodel (>=0.0.8,<0.0.9)
 Description-Content-Type: text/markdown
 
 # SQLModelService
 
-`SQLModelService` is a generic service layer on top of `SQLModel` for conveniently creating APIs with frameworks like [FastAPI](https://fastapi.tiangolo.com/).
+`SQLModelService` is a generic service layer on top of [SQLModel](https://sqlmodel.tiangolo.com/) for conveniently creating APIs with frameworks like [FastAPI](https://fastapi.tiangolo.com/).
+
+See the [documentation](https://volfpeter.github.io/sqlmodelservice) for examples and the API reference.
 
 ## Installation
 
 The library is available on PyPI and can be installed with:
 
 ```console
 $ pip install sqlmodelservice
```

