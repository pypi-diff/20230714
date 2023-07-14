# Comparing `tmp/ohdsi-sqlrender-0.2.1.tar.gz` & `tmp/ohdsi-sqlrender-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohdsi-sqlrender-0.2.1.tar", last modified: Tue Jul 11 14:30:34 2023, max compression
+gzip compressed data, was "ohdsi-sqlrender-0.2.2.tar", last modified: Fri Jul 14 10:13:54 2023, max compression
```

## Comparing `ohdsi-sqlrender-0.2.1.tar` & `ohdsi-sqlrender-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:34.728854 ohdsi-sqlrender-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-11 14:30:34.728854 ohdsi-sqlrender-0.2.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:34.728854 ohdsi-sqlrender-0.2.1/ohdsi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:34.728854 ohdsi-sqlrender-0.2.1/ohdsi/sqlrender/
--rw-r--r--   0 runner    (1001) docker     (123)    12125 2023-07-11 14:30:22.000000 ohdsi-sqlrender-0.2.1/ohdsi/sqlrender/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:34.728854 ohdsi-sqlrender-0.2.1/ohdsi_sqlrender.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-11 14:30:34.000000 ohdsi-sqlrender-0.2.1/ohdsi_sqlrender.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-11 14:30:34.000000 ohdsi-sqlrender-0.2.1/ohdsi_sqlrender.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:30:34.000000 ohdsi-sqlrender-0.2.1/ohdsi_sqlrender.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-11 14:30:34.000000 ohdsi-sqlrender-0.2.1/ohdsi_sqlrender.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 14:30:34.000000 ohdsi-sqlrender-0.2.1/ohdsi_sqlrender.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 14:30:34.728854 ohdsi-sqlrender-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-11 14:30:22.000000 ohdsi-sqlrender-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:54.322689 ohdsi-sqlrender-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-14 10:13:54.322689 ohdsi-sqlrender-0.2.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:54.318689 ohdsi-sqlrender-0.2.2/ohdsi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:54.318689 ohdsi-sqlrender-0.2.2/ohdsi/sqlrender/
+-rw-r--r--   0 runner    (1001) docker     (123)    12498 2023-07-14 10:13:44.000000 ohdsi-sqlrender-0.2.2/ohdsi/sqlrender/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:54.322689 ohdsi-sqlrender-0.2.2/ohdsi_sqlrender.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-14 10:13:54.000000 ohdsi-sqlrender-0.2.2/ohdsi_sqlrender.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-14 10:13:54.000000 ohdsi-sqlrender-0.2.2/ohdsi_sqlrender.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:13:54.000000 ohdsi-sqlrender-0.2.2/ohdsi_sqlrender.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-14 10:13:54.000000 ohdsi-sqlrender-0.2.2/ohdsi_sqlrender.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 10:13:54.000000 ohdsi-sqlrender-0.2.2/ohdsi_sqlrender.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 10:13:54.322689 ohdsi-sqlrender-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-14 10:13:44.000000 ohdsi-sqlrender-0.2.2/setup.py
```

### Comparing `ohdsi-sqlrender-0.2.1/ohdsi/sqlrender/__init__.py` & `ohdsi-sqlrender-0.2.2/ohdsi/sqlrender/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import os
+
 from pathlib import Path
 from rpy2.robjects.methods import RS4
 from rpy2.robjects.vectors import StrVector
 
 from rpy2.robjects.packages import importr
 
 #
@@ -11,16 +13,27 @@
 # def _py_none_to_null(py_obj):
 #     return robjects.null
 
 
 #
 # r interface
 #
-sql_render_r = importr('SqlRender')
-base_r = importr('base')
+# When building documentation for the project, the following import will fail
+# as the package is not installed. In this case, we set the variable to None
+# so that the documentation can be built.
+if os.environ.get('IGNORE_R_IMPORTS', False):
+    sql_render_r = None
+else:
+    sql_render_r = importr('SqlRender')
+
+try:
+    base_r = importr('base')
+except ImportError:
+    # TODO we should notify the user
+    base_r = None
 
 
 #
 # python wrappers
 #
 class SparkSql:
```

### Comparing `ohdsi-sqlrender-0.2.1/setup.py` & `ohdsi-sqlrender-0.2.2/setup.py`

 * *Files identical despite different names*

