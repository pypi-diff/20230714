# Comparing `tmp/funpymodeling-0.1.7.tar.gz` & `tmp/funpymodeling-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funpymodeling-0.1.7.tar", last modified: Wed Sep 16 14:29:28 2020, max compression
+gzip compressed data, was "funpymodeling-0.1.8.tar", max compression
```

## Comparing `funpymodeling-0.1.7.tar` & `funpymodeling-0.1.8.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0      113 2020-08-10 20:46:00.421946 funpymodeling-0.1.7/README.md
--rw-r--r--   0        0        0      181 2020-09-16 14:29:24.824993 funpymodeling-0.1.7/funpymodeling/__init__.py
--rw-r--r--   0        0        0     1426 2020-09-01 23:44:47.673357 funpymodeling-0.1.7/funpymodeling/data_prep.py
--rw-r--r--   0        0        0     7912 2020-09-01 23:44:47.673708 funpymodeling-0.1.7/funpymodeling/exploratory.py
--rw-r--r--   0        0        0     1792 2020-09-01 23:44:47.674010 funpymodeling-0.1.7/funpymodeling/model_validation.py
--rw-r--r--   0        0        0        0 2020-09-01 23:44:47.674214 funpymodeling-0.1.7/funpymodeling/test/__init__.py
--rw-r--r--   0        0        0       94 2020-09-01 23:44:47.674723 funpymodeling-0.1.7/funpymodeling/test/test_funpymodeling.py
--rw-r--r--   0        0        0      845 2020-09-16 14:29:21.444049 funpymodeling-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1161 2020-09-16 14:29:28.477957 funpymodeling-0.1.7/setup.py
--rw-r--r--   0        0        0     1143 2020-09-16 14:29:28.478298 funpymodeling-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      113 2023-06-28 15:10:52.000000 funpymodeling-0.1.8/README.md
+-rw-r--r--   0        0        0      181 2023-06-28 15:10:52.000000 funpymodeling-0.1.8/funpymodeling/__init__.py
+-rw-r--r--   0        0        0     1426 2023-06-28 15:10:52.000000 funpymodeling-0.1.8/funpymodeling/data_prep.py
+-rw-r--r--   0        0        0     7912 2023-06-28 15:10:52.000000 funpymodeling-0.1.8/funpymodeling/exploratory.py
+-rw-r--r--   0        0        0     1792 2023-06-28 15:10:52.000000 funpymodeling-0.1.8/funpymodeling/model_validation.py
+-rw-r--r--   0        0        0        0 2023-06-28 15:10:52.000000 funpymodeling-0.1.8/funpymodeling/test/__init__.py
+-rw-r--r--   0        0        0       94 2023-06-28 15:10:52.000000 funpymodeling-0.1.8/funpymodeling/test/test_funpymodeling.py
+-rw-r--r--   0        0        0      779 2023-07-13 23:34:56.694732 funpymodeling-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1339 1970-01-01 00:00:00.000000 funpymodeling-0.1.8/PKG-INFO
```

### Comparing `funpymodeling-0.1.7/funpymodeling/data_prep.py` & `funpymodeling-0.1.8/funpymodeling/data_prep.py`

 * *Files identical despite different names*

### Comparing `funpymodeling-0.1.7/funpymodeling/exploratory.py` & `funpymodeling-0.1.8/funpymodeling/exploratory.py`

 * *Files identical despite different names*

### Comparing `funpymodeling-0.1.7/funpymodeling/model_validation.py` & `funpymodeling-0.1.8/funpymodeling/model_validation.py`

 * *Files identical despite different names*

### Comparing `funpymodeling-0.1.7/pyproject.toml` & `funpymodeling-0.1.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 [tool.poetry]
 name = "funpymodeling"
-version = "0.1.7"
+version = "0.1.8"
 description = "A package designed for data scientists and teachers, to speed up their ML projects, focused on exploratory data analysis, data preparation, and model performance."
 license="MIT"
 authors = ["Pablo Casas <pcasas.biz@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/pablo14/funPyModeling"
 documentation = "https://github.com/pablo14/funPyModeling"
 
 [tool.poetry.dependencies]
-python = "^3.6.1"
-pandas = "^1.0.5"
-numpy = "^1.18.5"
-matplotlib = "^3.2.2"
-typing-extensions = { version = "^3.7.4", python = "<3.8" }
-sklearn = "^0.0"
-seaborn = "^0.10.1"
-
-[tool.poetry.dev-dependencies]
-flake8 = "^3.8.1"
+python = ">=3.8.1,<4.0"
+pandas = "^2.0.2"
+numpy = "^1.24.3"
+matplotlib = "^3.7.1"
+typing-extensions = "^4.6.3"
+scikit-learn = "^1.2.2"
+seaborn = "^0.12.2"
+flake8 = "^6.0.0"
 jupyter = "^1.0.0"
-pre-commit = "^2.4.0"
-pytest = "^5.4.2"
-coveralls = "^2.0.0"
+pre-commit = "^3.3.2"
+pytest = "^7.3.1"
+
 
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

