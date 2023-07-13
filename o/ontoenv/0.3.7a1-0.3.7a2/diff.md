# Comparing `tmp/ontoenv-0.3.7a1.tar.gz` & `tmp/ontoenv-0.3.7a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ontoenv-0.3.7a1.tar", max compression
+gzip compressed data, was "ontoenv-0.3.7a2.tar", max compression
```

## Comparing `ontoenv-0.3.7a1.tar` & `ontoenv-0.3.7a2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1519 2023-04-20 23:37:22.604572 ontoenv-0.3.7a1/LICENSE
--rw-r--r--   0        0        0    12565 2023-07-13 23:36:29.662858 ontoenv-0.3.7a1/ontoenv/__init__.py
--rw-r--r--   0        0        0     2065 2023-04-20 23:37:22.605017 ontoenv-0.3.7a1/ontoenv/cli.py
--rw-r--r--   0        0        0      529 2023-07-13 23:36:40.716858 ontoenv-0.3.7a1/pyproject.toml
--rw-r--r--   0        0        0      813 1970-01-01 00:00:00.000000 ontoenv-0.3.7a1/PKG-INFO
+-rw-r--r--   0        0        0     1519 2023-04-20 23:37:22.604572 ontoenv-0.3.7a2/LICENSE
+-rw-r--r--   0        0        0    12565 2023-07-13 23:36:29.662858 ontoenv-0.3.7a2/ontoenv/__init__.py
+-rw-r--r--   0        0        0     2065 2023-04-20 23:37:22.605017 ontoenv-0.3.7a2/ontoenv/cli.py
+-rw-r--r--   0        0        0      529 2023-07-13 23:40:01.900826 ontoenv-0.3.7a2/pyproject.toml
+-rw-r--r--   0        0        0      813 1970-01-01 00:00:00.000000 ontoenv-0.3.7a2/PKG-INFO
```

### Comparing `ontoenv-0.3.7a1/LICENSE` & `ontoenv-0.3.7a2/LICENSE`

 * *Files identical despite different names*

### Comparing `ontoenv-0.3.7a1/ontoenv/__init__.py` & `ontoenv-0.3.7a2/ontoenv/__init__.py`

 * *Files identical despite different names*

### Comparing `ontoenv-0.3.7a1/ontoenv/cli.py` & `ontoenv-0.3.7a2/ontoenv/cli.py`

 * *Files identical despite different names*

### Comparing `ontoenv-0.3.7a1/pyproject.toml` & `ontoenv-0.3.7a2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ontoenv"
-version = "0.3.7a1"
+version = "0.3.7a2"
 description = "Manages owl:imports statements for multi-file development"
 authors = ["Gabe Fierro <gtfierro@mines.edu>"]
 license = "BSD 3-Clause"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 rdflib = "^6.0.0"
```

### Comparing `ontoenv-0.3.7a1/PKG-INFO` & `ontoenv-0.3.7a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ontoenv
-Version: 0.3.7a1
+Version: 0.3.7a2
 Summary: Manages owl:imports statements for multi-file development
 License: BSD 3-Clause
 Author: Gabe Fierro
 Author-email: gtfierro@mines.edu
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

