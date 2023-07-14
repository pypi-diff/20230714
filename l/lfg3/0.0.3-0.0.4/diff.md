# Comparing `tmp/lfg3-0.0.3.tar.gz` & `tmp/lfg3-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfg3-0.0.3.tar", max compression
+gzip compressed data, was "lfg3-0.0.4.tar", max compression
```

## Comparing `lfg3-0.0.3.tar` & `lfg3-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1064 2023-07-14 17:53:09.614185 lfg3-0.0.3/LICENSE
--rw-r--r--   0        0        0     2385 2023-07-14 20:15:32.577555 lfg3-0.0.3/README.md
--rw-r--r--   0        0        0        0 2023-07-14 17:53:09.638329 lfg3-0.0.3/lfg3/__init__.py
--rw-r--r--   0        0        0      183 2023-07-14 20:15:44.376799 lfg3-0.0.3/lfg3/utils.py
--rw-r--r--   0        0        0     1548 2023-07-14 20:16:08.591573 lfg3-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2912 1970-01-01 00:00:00.000000 lfg3-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-14 17:53:09.614185 lfg3-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2385 2023-07-14 20:15:32.577555 lfg3-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-07-14 17:53:09.638329 lfg3-0.0.4/lfg3/__init__.py
+-rw-r--r--   0        0        0      183 2023-07-14 20:15:44.376799 lfg3-0.0.4/lfg3/utils.py
+-rw-r--r--   0        0        0     1529 2023-07-14 20:17:13.302869 lfg3-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2881 1970-01-01 00:00:00.000000 lfg3-0.0.4/PKG-INFO
```

### Comparing `lfg3-0.0.3/LICENSE` & `lfg3-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lfg3-0.0.3/README.md` & `lfg3-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `lfg3-0.0.3/pyproject.toml` & `lfg3-0.0.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "lfg3"
-version = "0.0.3"
+version = "0.0.4"
 description = "ether"
-authors = ["monokh <mnokhb@gmail.com>"]
+authors = ["monokh"]
 repository = "https://github.com/monokh/lfg3"
 readme = "README.md"
 packages = [
   {include = "lfg3"}
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `lfg3-0.0.3/PKG-INFO` & `lfg3-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: lfg3
-Version: 0.0.3
+Version: 0.0.4
 Summary: ether
 Home-page: https://github.com/monokh/lfg3
 Author: monokh
-Author-email: mnokhb@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Project-URL: Repository, https://github.com/monokh/lfg3
```

