# Comparing `tmp/factorio-0.2.0.tar.gz` & `tmp/factorio-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "factorio-0.2.0.tar", max compression
+gzip compressed data, was "factorio-0.3.0.tar", max compression
```

## Comparing `factorio-0.2.0.tar` & `factorio-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     7652 2023-03-10 22:07:08.021389 factorio-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0     1628 2023-04-27 20:50:15.037000 factorio-0.2.0/README.rst
--rw-r--r--   0        0        0     2621 2023-06-08 15:36:26.218108 factorio-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-10 22:07:08.023760 factorio-0.2.0/src/factorio/__init__.py
--rw-r--r--   0        0        0      539 2023-04-28 08:43:44.957572 factorio-0.2.0/src/factorio/factories.py
--rw-r--r--   0        0        0     1667 2023-04-28 08:43:44.957758 factorio-0.2.0/src/factorio/fields.py
--rw-r--r--   0        0        0        0 2023-03-10 22:07:08.033431 factorio-0.2.0/src/factorio/py.typed
--rw-r--r--   0        0        0     2533 1970-01-01 00:00:00.000000 factorio-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-03-10 22:07:08.021389 factorio-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     1628 2023-04-27 20:50:15.037000 factorio-0.3.0/README.rst
+-rw-r--r--   0        0        0     2612 2023-07-14 10:26:21.422628 factorio-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-10 22:07:08.023760 factorio-0.3.0/src/factorio/__init__.py
+-rw-r--r--   0        0        0      616 2023-07-14 10:10:11.033681 factorio-0.3.0/src/factorio/factories.py
+-rw-r--r--   0        0        0     1667 2023-07-14 09:23:41.843038 factorio-0.3.0/src/factorio/fields.py
+-rw-r--r--   0        0        0        0 2023-03-10 22:07:08.033431 factorio-0.3.0/src/factorio/py.typed
+-rw-r--r--   0        0        0     2533 1970-01-01 00:00:00.000000 factorio-0.3.0/PKG-INFO
```

### Comparing `factorio-0.2.0/LICENSE.txt` & `factorio-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `factorio-0.2.0/README.rst` & `factorio-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `factorio-0.2.0/pyproject.toml` & `factorio-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
 skip_empty = true
 
 [tool.poetry]
 name = "factorio"
-version = "0.2.0"
+version = "0.3.0"
 description = "A fixtures replacement tool"
 authors = [
     "Stephanos Kuma <stephanos@kuma.ai>",
 ]
 
 license = "LGPL-3.0+"
 readme = "README.rst"
@@ -122,15 +122,15 @@
 ]
 
 [tool.poetry.dependencies]
 # python version
 python = "^3.8"
 
 # dependencies
-Faker = "^18.0"
+Faker = "^19.0"
 
 [tool.poetry.group.dev.dependencies]
 ipdb = {version = "^0.13", python = "^3.9"}
 ipython = {version = "^8.12", python = "^3.9"}
 pipdeptree = "^2.7"
 
 [tool.poetry.group.lint.dependencies]
@@ -139,9 +139,9 @@
 ruff = "^0.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3"
 pytest-cov = "^4.0"
 
 [tool.poetry.group.docs.dependencies]
-sphinx = "^6.2"
-sphinx-rtd-theme = "^1.2"
+furo = "^2023.5"
+sphinx = "^7.0"
```

### Comparing `factorio-0.2.0/src/factorio/factories.py` & `factorio-0.3.0/src/factorio/factories.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,21 +2,25 @@
 
 from typing import Any
 
 from factorio.fields import AbstractField
 
 
 class Factory:
+    Fields: type
+
     class Meta:
         model: type
-        fields: dict[str, Any]
 
     @classmethod
     def build(cls, **kwargs: Any) -> Any:
         fields: dict[str, Any] = {}
-        for key, value in cls.Meta.fields.items():
+        for key, value in cls.Fields.__dict__.items():
+            if key.startswith("__") and key.endswith("__"):
+                continue
+
             if key in kwargs:
                 value = kwargs[key]  # noqa: PLW2901
 
             fields[key] = value() if isinstance(value, AbstractField) else value
 
         return cls.Meta.model(**fields)
```

### Comparing `factorio-0.2.0/src/factorio/fields.py` & `factorio-0.3.0/src/factorio/fields.py`

 * *Files identical despite different names*

### Comparing `factorio-0.2.0/PKG-INFO` & `factorio-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: factorio
-Version: 0.2.0
+Version: 0.3.0
 Summary: A fixtures replacement tool
 Home-page: https://factorio.readthedocs.io/en/stable/
 License: LGPL-3.0+
 Keywords: tests
 Author: Stephanos Kuma
 Author-email: stephanos@kuma.ai
 Requires-Python: >=3.8,<4.0
@@ -12,15 +12,15 @@
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Faker (>=18.0,<19.0)
+Requires-Dist: Faker (>=19.0,<20.0)
 Project-URL: Documentation, https://factorio.readthedocs.io/en/stable/
 Project-URL: Repository, https://github.com/spapanik/factorio
 Description-Content-Type: text/x-rst
 
 =====================================
 factorio: A fixtures replacement tool
 =====================================
```

