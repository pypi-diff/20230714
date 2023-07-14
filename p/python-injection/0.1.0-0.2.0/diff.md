# Comparing `tmp/python_injection-0.1.0.tar.gz` & `tmp/python_injection-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_injection-0.1.0.tar", max compression
+gzip compressed data, was "python_injection-0.2.0.tar", max compression
```

## Comparing `python_injection-0.1.0.tar` & `python_injection-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0     1907 2023-07-14 16:22:33.385524 python_injection-0.1.0/README.md
--rw-r--r--   0        0        0       38 2023-07-14 16:22:33.385524 python_injection-0.1.0/injection/__init__.py
--rw-r--r--   0        0        0     3621 2023-07-14 16:22:33.385524 python_injection-0.1.0/injection/core.py
--rw-r--r--   0        0        0      381 2023-07-14 16:22:33.385524 python_injection-0.1.0/injection/core.pyi
--rw-r--r--   0        0        0      561 2023-07-14 16:23:01.138872 python_injection-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2472 1970-01-01 00:00:00.000000 python_injection-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2538 2023-07-14 21:21:08.690746 python_injection-0.2.0/README.md
+-rw-r--r--   0        0        0       38 2023-07-14 21:21:08.690746 python_injection-0.2.0/injection/__init__.py
+-rw-r--r--   0        0        0     3621 2023-07-14 21:21:08.690746 python_injection-0.2.0/injection/core.py
+-rw-r--r--   0        0        0      381 2023-07-14 21:21:08.690746 python_injection-0.2.0/injection/core.pyi
+-rw-r--r--   0        0        0      461 2023-07-14 21:21:08.690746 python_injection-0.2.0/injection/utils.py
+-rw-r--r--   0        0        0       81 2023-07-14 21:21:08.690746 python_injection-0.2.0/injection/utils.pyi
+-rw-r--r--   0        0        0      561 2023-07-14 21:21:33.231213 python_injection-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3103 1970-01-01 00:00:00.000000 python_injection-0.2.0/PKG-INFO
```

### Comparing `python_injection-0.1.0/injection/core.py` & `python_injection-0.2.0/injection/core.py`

 * *Files identical despite different names*

### Comparing `python_injection-0.1.0/pyproject.toml` & `python_injection-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-injection"
-version = "0.1.0"
+version = "0.2.0"
 description = "Fast and easy dependency injection framework."
 authors = ["remimd"]
 keywords = ["dependencies", "inject", "injection"]
 license = "MIT"
 packages = [{ include = "injection" }]
 readme = "README.md"
 repository = "https://github.com/soon-app/injection"
```

### Comparing `python_injection-0.1.0/PKG-INFO` & `python_injection-0.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,11 @@
-Metadata-Version: 2.1
-Name: python-injection
-Version: 0.1.0
-Summary: Fast and easy dependency injection framework.
-Home-page: https://github.com/soon-app/injection
-License: MIT
-Keywords: dependencies,inject,injection
-Author: remimd
-Requires-Python: >=3.10,<4
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Project-URL: Repository, https://github.com/soon-app/injection
-Description-Content-Type: text/markdown
-
 # Injection
 
 [![CI](https://github.com/soon-app/injection/actions/workflows/ci.yml/badge.svg)](https://github.com/soon-app/injection)
+[![PyPI](https://badge.fury.io/py/python-injection.svg)](https://pypi.org/project/python-injection/)
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Fast and easy dependency injection framework.
 
 ## Quick start
 
 ⚠️ _Requires Python 3.10 or higher_
@@ -68,14 +53,15 @@
 
 ### Inheritance
 
 In the case of inheritance, you can use the decorator parameters `reference` or `references` to link the injection to 
 one or several other classes.
 
 **Warning: if the child class is in another file, make sure that file is imported before injection.**
+[_See `load_package` function._](#load_package)
 
 _`reference` parameter example:_
 
 ```python
 from injection import unique
 
 class A:
@@ -111,7 +97,33 @@
 from injection import unique
 
 @unique(reference=MyClass)
 def my_recipe() -> MyClass:
     """ recipe implementation """
 ```
 
+## Utils
+
+### load_package
+
+Useful for put in memory injectables hidden deep within a package. Example:
+
+```
+package
+├── sub_package
+│   ├── __init__.py
+│   └── module2.py
+│       └── class Injectable1
+├── __init__.py
+└── module1.py
+    └── class Injectable2
+```
+
+To load Injectable1 and Injectable2 into memory you can do the following:
+
+```python
+from injection.utils import load_package
+
+import package
+
+load_package(package)
+```
```

