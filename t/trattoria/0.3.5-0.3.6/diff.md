# Comparing `tmp/trattoria-0.3.5.tar.gz` & `tmp/trattoria-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trattoria-0.3.5.tar", max compression
+gzip compressed data, was "trattoria-0.3.6.tar", max compression
```

## Comparing `trattoria-0.3.5.tar` & `trattoria-0.3.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3045 2023-07-13 16:18:55.310579 trattoria-0.3.5/README.md
--rw-r--r--   0        0        0      583 2023-07-14 09:46:33.110667 trattoria-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      347 2023-07-13 09:43:14.854450 trattoria-0.3.5/trattoria/__init__.py
--rw-r--r--   0        0        0    16141 2023-07-13 09:43:14.854570 trattoria-0.3.5/trattoria/core.py
--rw-r--r--   0        0        0     3033 2023-07-13 09:43:14.854629 trattoria-0.3.5/trattoria/postselection.py
--rw-r--r--   0        0        0     3833 1970-01-01 00:00:00.000000 trattoria-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     3045 2023-07-13 16:18:55.310579 trattoria-0.3.6/README.md
+-rw-r--r--   0        0        0      583 2023-07-14 09:57:28.624923 trattoria-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0      347 2023-07-13 09:43:14.854450 trattoria-0.3.6/trattoria/__init__.py
+-rw-r--r--   0        0        0    16141 2023-07-13 09:43:14.854570 trattoria-0.3.6/trattoria/core.py
+-rw-r--r--   0        0        0     3033 2023-07-13 09:43:14.854629 trattoria-0.3.6/trattoria/postselection.py
+-rw-r--r--   0        0        0     3833 1970-01-01 00:00:00.000000 trattoria-0.3.6/PKG-INFO
```

### Comparing `trattoria-0.3.5/README.md` & `trattoria-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `trattoria-0.3.5/pyproject.toml` & `trattoria-0.3.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "trattoria"
-version = "0.3.5"
+version = "0.3.6"
 description = "The fastest streaming algorithms for your TTTR data"
 authors = ["Guillem Ballesteros <dev+pypi@maxwellrules.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/GCBallesteros/trattoria"
 repository = "https://github.com/GCBallesteros/trattoria"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 numpy = ">=1.20"
 scipy = ">=1.8"
-trattoria-core = "0.4.4"
+trattoria-core = "0.4.3"
 
 [tool.poetry.dev-dependencies]
 black = "^20.8b1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `trattoria-0.3.5/trattoria/core.py` & `trattoria-0.3.6/trattoria/core.py`

 * *Files identical despite different names*

### Comparing `trattoria-0.3.5/trattoria/postselection.py` & `trattoria-0.3.6/trattoria/postselection.py`

 * *Files identical despite different names*

### Comparing `trattoria-0.3.5/PKG-INFO` & `trattoria-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: trattoria
-Version: 0.3.5
+Version: 0.3.6
 Summary: The fastest streaming algorithms for your TTTR data
 Home-page: https://github.com/GCBallesteros/trattoria
 License: MIT
 Author: Guillem Ballesteros
 Author-email: dev+pypi@maxwellrules.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.20)
 Requires-Dist: scipy (>=1.8)
-Requires-Dist: trattoria-core (==0.4.4)
+Requires-Dist: trattoria-core (==0.4.3)
 Project-URL: Repository, https://github.com/GCBallesteros/trattoria
 Description-Content-Type: text/markdown
 
 # 🍕 Trattoria 🍕
 Trattoria delivers you the fastest streaming algorithms to analyze your TTTR data. We
 currenlty support the following algorithms:
 - __Second order autocorrelations__: Calculate the autocorrelation between two channels of
```

