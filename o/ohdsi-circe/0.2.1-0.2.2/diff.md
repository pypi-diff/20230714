# Comparing `tmp/ohdsi-circe-0.2.1.tar.gz` & `tmp/ohdsi-circe-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohdsi-circe-0.2.1.tar", last modified: Tue Jul 11 14:30:33 2023, max compression
+gzip compressed data, was "ohdsi-circe-0.2.2.tar", last modified: Fri Jul 14 10:13:52 2023, max compression
```

## Comparing `ohdsi-circe-0.2.1.tar` & `ohdsi-circe-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:33.372873 ohdsi-circe-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-11 14:30:33.372873 ohdsi-circe-0.2.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:33.372873 ohdsi-circe-0.2.1/ohdsi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:33.372873 ohdsi-circe-0.2.1/ohdsi/circe/
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-07-11 14:30:22.000000 ohdsi-circe-0.2.1/ohdsi/circe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:33.372873 ohdsi-circe-0.2.1/ohdsi/circe/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-11 14:30:22.000000 ohdsi-circe-0.2.1/ohdsi/circe/data/conceptSet.json
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-11 14:30:22.000000 ohdsi-circe-0.2.1/ohdsi/circe/data/conceptSetList.json
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-11 14:30:22.000000 ohdsi-circe-0.2.1/ohdsi/circe/data/simpleCohort.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:33.372873 ohdsi-circe-0.2.1/ohdsi_circe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-11 14:30:33.000000 ohdsi-circe-0.2.1/ohdsi_circe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-11 14:30:33.000000 ohdsi-circe-0.2.1/ohdsi_circe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:30:33.000000 ohdsi-circe-0.2.1/ohdsi_circe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-11 14:30:33.000000 ohdsi-circe-0.2.1/ohdsi_circe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 14:30:33.000000 ohdsi-circe-0.2.1/ohdsi_circe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 14:30:33.372873 ohdsi-circe-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-11 14:30:22.000000 ohdsi-circe-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:52.986669 ohdsi-circe-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-14 10:13:52.986669 ohdsi-circe-0.2.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:52.986669 ohdsi-circe-0.2.2/ohdsi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:52.986669 ohdsi-circe-0.2.2/ohdsi/circe/
+-rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-07-14 10:13:44.000000 ohdsi-circe-0.2.2/ohdsi/circe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:52.986669 ohdsi-circe-0.2.2/ohdsi/circe/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-14 10:13:44.000000 ohdsi-circe-0.2.2/ohdsi/circe/data/conceptSet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-14 10:13:44.000000 ohdsi-circe-0.2.2/ohdsi/circe/data/conceptSetList.json
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-14 10:13:44.000000 ohdsi-circe-0.2.2/ohdsi/circe/data/simpleCohort.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:52.986669 ohdsi-circe-0.2.2/ohdsi_circe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-14 10:13:52.000000 ohdsi-circe-0.2.2/ohdsi_circe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-14 10:13:52.000000 ohdsi-circe-0.2.2/ohdsi_circe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:13:52.000000 ohdsi-circe-0.2.2/ohdsi_circe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-14 10:13:52.000000 ohdsi-circe-0.2.2/ohdsi_circe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 10:13:52.000000 ohdsi-circe-0.2.2/ohdsi_circe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 10:13:52.986669 ohdsi-circe-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-14 10:13:44.000000 ohdsi-circe-0.2.2/setup.py
```

### Comparing `ohdsi-circe-0.2.1/ohdsi/circe/__init__.py` & `ohdsi-circe-0.2.2/ohdsi/circe/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 import json
+import os
+
+from pathlib import Path
 
 from rpy2 import robjects
 from rpy2.robjects.methods import RS4
 from rpy2.robjects.vectors import StrVector
 
 from rpy2.robjects.packages import importr
 
@@ -11,18 +14,29 @@
 # Converters
 #
 @robjects.default_converter.py2rpy.register(type(None))
 def _py_none_to_null(py_obj):
     return robjects.NULL
 
 
+@robjects.default_converter.py2rpy.register(Path)
+def _py_path_to_str(py_obj):
+    return robjects.StrVector(str(py_obj))
+
+
 #
 # R interface
 #
-circe_r = importr('CirceR')
+# When building documentation for the project, the following import will fail
+# as the package is not installed. In this case, we set the variable to None
+# so that the documentation can be built.
+if os.environ.get('IGNORE_R_IMPORTS', False):
+    circe_r = None
+else:
+    circe_r = importr('CirceR')
 
 
 #
 # Python wrappers
 #
 class CohortExpression:
```

### Comparing `ohdsi-circe-0.2.1/ohdsi/circe/data/conceptSet.json` & `ohdsi-circe-0.2.2/ohdsi/circe/data/conceptSet.json`

 * *Files identical despite different names*

### Comparing `ohdsi-circe-0.2.1/ohdsi/circe/data/conceptSetList.json` & `ohdsi-circe-0.2.2/ohdsi/circe/data/conceptSetList.json`

 * *Files identical despite different names*

### Comparing `ohdsi-circe-0.2.1/ohdsi/circe/data/simpleCohort.json` & `ohdsi-circe-0.2.2/ohdsi/circe/data/simpleCohort.json`

 * *Files identical despite different names*

### Comparing `ohdsi-circe-0.2.1/setup.py` & `ohdsi-circe-0.2.2/setup.py`

 * *Files identical despite different names*

