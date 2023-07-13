# Comparing `tmp/ontoenv-0.3.7a3.tar.gz` & `tmp/ontoenv-0.3.7a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ontoenv-0.3.7a3.tar", max compression
+gzip compressed data, was "ontoenv-0.3.7a4.tar", max compression
```

## Comparing `ontoenv-0.3.7a3.tar` & `ontoenv-0.3.7a4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1519 2023-04-20 23:37:22.604572 ontoenv-0.3.7a3/LICENSE
--rw-r--r--   0        0        0    12627 2023-07-13 23:43:29.773713 ontoenv-0.3.7a3/ontoenv/__init__.py
--rw-r--r--   0        0        0     2065 2023-04-20 23:37:22.605017 ontoenv-0.3.7a3/ontoenv/cli.py
--rw-r--r--   0        0        0      529 2023-07-13 23:43:35.088586 ontoenv-0.3.7a3/pyproject.toml
--rw-r--r--   0        0        0      813 1970-01-01 00:00:00.000000 ontoenv-0.3.7a3/PKG-INFO
+-rw-r--r--   0        0        0     1519 2023-04-20 23:37:22.604572 ontoenv-0.3.7a4/LICENSE
+-rw-r--r--   0        0        0    12672 2023-07-13 23:46:05.111025 ontoenv-0.3.7a4/ontoenv/__init__.py
+-rw-r--r--   0        0        0     2065 2023-04-20 23:37:22.605017 ontoenv-0.3.7a4/ontoenv/cli.py
+-rw-r--r--   0        0        0      529 2023-07-13 23:46:09.544483 ontoenv-0.3.7a4/pyproject.toml
+-rw-r--r--   0        0        0      813 1970-01-01 00:00:00.000000 ontoenv-0.3.7a4/PKG-INFO
```

### Comparing `ontoenv-0.3.7a3/LICENSE` & `ontoenv-0.3.7a4/LICENSE`

 * *Files identical despite different names*

### Comparing `ontoenv-0.3.7a3/ontoenv/__init__.py` & `ontoenv-0.3.7a4/ontoenv/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -273,14 +273,15 @@
             cache.add(uri)
         if (recursive or recursive_limit > 0) and new_imports:
             self.import_dependencies(
                 graph,
                 cache=cache,
                 recursive=recursive,
                 recursive_limit=recursive_limit - 1,
+                keep_matching=keep_matching,
             )
 
 
 def find_root_file(start=None) -> Optional[Path]:
     """
     Starting at the current directory, traverse upwards until it finds a .ontoenv directory
     """
```

### Comparing `ontoenv-0.3.7a3/ontoenv/cli.py` & `ontoenv-0.3.7a4/ontoenv/cli.py`

 * *Files identical despite different names*

### Comparing `ontoenv-0.3.7a3/pyproject.toml` & `ontoenv-0.3.7a4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ontoenv"
-version = "0.3.7a3"
+version = "0.3.7a4"
 description = "Manages owl:imports statements for multi-file development"
 authors = ["Gabe Fierro <gtfierro@mines.edu>"]
 license = "BSD 3-Clause"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 rdflib = "^6.0.0"
```

### Comparing `ontoenv-0.3.7a3/PKG-INFO` & `ontoenv-0.3.7a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ontoenv
-Version: 0.3.7a3
+Version: 0.3.7a4
 Summary: Manages owl:imports statements for multi-file development
 License: BSD 3-Clause
 Author: Gabe Fierro
 Author-email: gtfierro@mines.edu
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

