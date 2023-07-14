# Comparing `tmp/sphinx-sql-1.3.4.tar.gz` & `tmp/sphinx-sql-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-sql-1.3.4.tar", last modified: Sun Aug  7 19:54:20 2022, max compression
+gzip compressed data, was "sphinx-sql-1.3.5.tar", last modified: Fri Jul 14 03:07:02 2023, max compression
```

## Comparing `sphinx-sql-1.3.4.tar` & `sphinx-sql-1.3.5.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-07 19:54:20.981740 sphinx-sql-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (121)    35148 2022-08-07 19:54:04.000000 sphinx-sql-1.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-07 19:54:04.000000 sphinx-sql-1.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6109 2022-08-07 19:54:20.981740 sphinx-sql-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5853 2022-08-07 19:54:04.000000 sphinx-sql-1.3.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-07 19:54:20.981740 sphinx-sql-1.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-08-07 19:54:04.000000 sphinx-sql-1.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-07 19:54:20.977740 sphinx-sql-1.3.4/sphinx_sql/
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-08-07 19:54:04.000000 sphinx-sql-1.3.4/sphinx_sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22992 2022-08-07 19:54:04.000000 sphinx-sql-1.3.4/sphinx_sql/sphinx_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-07 19:54:20.981740 sphinx-sql-1.3.4/sphinx_sql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6109 2022-08-07 19:54:20.000000 sphinx-sql-1.3.4/sphinx_sql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      256 2022-08-07 19:54:20.000000 sphinx-sql-1.3.4/sphinx_sql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-07 19:54:20.000000 sphinx-sql-1.3.4/sphinx_sql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-08-07 19:54:20.000000 sphinx-sql-1.3.4/sphinx_sql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-08-07 19:54:20.000000 sphinx-sql-1.3.4/sphinx_sql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:07:02.282540 sphinx-sql-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-14 03:06:52.000000 sphinx-sql-1.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 03:06:52.000000 sphinx-sql-1.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-07-14 03:07:02.282540 sphinx-sql-1.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-07-14 03:06:52.000000 sphinx-sql-1.3.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 03:07:02.282540 sphinx-sql-1.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-14 03:06:52.000000 sphinx-sql-1.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:07:02.282540 sphinx-sql-1.3.5/sphinx_sql/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-14 03:06:52.000000 sphinx-sql-1.3.5/sphinx_sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23135 2023-07-14 03:06:52.000000 sphinx-sql-1.3.5/sphinx_sql/sphinx_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:07:02.282540 sphinx-sql-1.3.5/sphinx_sql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-07-14 03:07:02.000000 sphinx-sql-1.3.5/sphinx_sql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-14 03:07:02.000000 sphinx-sql-1.3.5/sphinx_sql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 03:07:02.000000 sphinx-sql-1.3.5/sphinx_sql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-14 03:07:02.000000 sphinx-sql-1.3.5/sphinx_sql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-14 03:07:02.000000 sphinx-sql-1.3.5/sphinx_sql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:07:02.282540 sphinx-sql-1.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-07-14 03:06:52.000000 sphinx-sql-1.3.5/tests/test_sphinx_sql.py
```

### Comparing `sphinx-sql-1.3.4/LICENSE` & `sphinx-sql-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-sql-1.3.4/PKG-INFO` & `sphinx-sql-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-sql
-Version: 1.3.4
+Version: 1.3.5
 Summary: Sphinx extension for autodoc of SQL files.
 Home-page: https://github.com/jackscodemonkey/sphinx-sql
 Author: Marcus Robb
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `sphinx-sql-1.3.4/README.rst` & `sphinx-sql-1.3.5/README.rst`

 * *Files identical despite different names*

### Comparing `sphinx-sql-1.3.4/setup.py` & `sphinx-sql-1.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `sphinx-sql-1.3.4/sphinx_sql/sphinx_sql.py` & `sphinx-sql-1.3.5/sphinx_sql/sphinx_sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 ]
 
 
 class SqlDirective(Directive):
     has_content = False
     option_spec = {"sqlsource": directives.unchanged}
 
-    # Most of these regex strings should be case insensitive lookups
+    # Most of these regex strings should be case-insensitive lookups
     closing_regex = (
         r"((?=return:)|(?=purpose:)|(?=dependent objects:)|"
         r"(?=changelog:)|(?=parameters)|(?=\*/))"
     )
     regex_dict = {
         # Full comment block
         "top_sql_block_comments": r"(?s)/*.*?\*/",
@@ -61,15 +61,15 @@
         # in cluster and catalog objects (e.g. database, role; extension,
         #  schema)
         "object_cluster_catalog": r"(?<=create)\s+(\w+)\s*(if not exists)*\s"
         r'?("?[^\s*;]*"?)\s*',
         # Match Group 2 (a defined special object type, e.g. "materialized")
         # and Group 3 for Object Type, Group 5 for Object Name
         # in schema objects (e.g. table, view, function)
-        "object_schema": rf"(?<=create)\s*(or replace)?\s*("
+        "object_schema": rf"(?:(?<=create)|(?<=alter))\s*(or replace|or alter)?\s*("
         rf"{'|'.join(special_obj_type)}"
         rf")?\s*(\w+)\s*(if not exists)*\s?((\w*)\.(\"?[^\s*\(]*\"?))",
         # Match Group 2 for distribution key, comma separated for multiple keys
         "distributed_by": r"distributed by \(.*?\)",
         # Match Group 2 for partition type (range) Group 3 for partition key.
         "partition_by": r"partition by \(.*?\)",
         # Match Group 1 for language
@@ -264,14 +264,17 @@
                     "",
                 )
             try:
                 if "sql_type" in locals():
                     # DDL file
                     # Read name and type from ANSI92 SQL objects first
                     object_details["type"] = str(sql_type[0]).upper().strip()
+                    if object_details["type"] == "PROC":
+                        object_details["type"] = "PROCEDURE"
+
                     object_details["name"] = (
                         str(sql_type[1]).lower().strip().replace('"', "")
                     )
 
                     if object_details["type"] in TABLE_TYPES:
                         dist = self.objdist.findall(contents)
                         part = self.objpart.findall(contents)
```

### Comparing `sphinx-sql-1.3.4/sphinx_sql.egg-info/PKG-INFO` & `sphinx-sql-1.3.5/sphinx_sql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-sql
-Version: 1.3.4
+Version: 1.3.5
 Summary: Sphinx extension for autodoc of SQL files.
 Home-page: https://github.com/jackscodemonkey/sphinx-sql
 Author: Marcus Robb
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

