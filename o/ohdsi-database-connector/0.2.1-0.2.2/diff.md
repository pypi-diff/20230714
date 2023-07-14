# Comparing `tmp/ohdsi-database-connector-0.2.1.tar.gz` & `tmp/ohdsi-database-connector-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohdsi-database-connector-0.2.1.tar", last modified: Tue Jul 11 14:30:34 2023, max compression
+gzip compressed data, was "ohdsi-database-connector-0.2.2.tar", last modified: Fri Jul 14 10:13:53 2023, max compression
```

## Comparing `ohdsi-database-connector-0.2.1.tar` & `ohdsi-database-connector-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:34.252861 ohdsi-database-connector-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-11 14:30:34.252861 ohdsi-database-connector-0.2.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:34.252861 ohdsi-database-connector-0.2.1/ohdsi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:34.252861 ohdsi-database-connector-0.2.1/ohdsi/database_connector/
--rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-07-11 14:30:22.000000 ohdsi-database-connector-0.2.1/ohdsi/database_connector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:34.252861 ohdsi-database-connector-0.2.1/ohdsi/database_connector/java/
--rw-r--r--   0 runner    (1001) docker     (123)  1004719 2023-07-11 14:30:22.000000 ohdsi-database-connector-0.2.1/ohdsi/database_connector/java/postgresql-42.2.18.jar
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:34.252861 ohdsi-database-connector-0.2.1/ohdsi_database_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-11 14:30:34.000000 ohdsi-database-connector-0.2.1/ohdsi_database_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-11 14:30:34.000000 ohdsi-database-connector-0.2.1/ohdsi_database_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:30:34.000000 ohdsi-database-connector-0.2.1/ohdsi_database_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-11 14:30:34.000000 ohdsi-database-connector-0.2.1/ohdsi_database_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 14:30:34.000000 ohdsi-database-connector-0.2.1/ohdsi_database_connector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 14:30:34.252861 ohdsi-database-connector-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-11 14:30:22.000000 ohdsi-database-connector-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:53.834680 ohdsi-database-connector-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-14 10:13:53.834680 ohdsi-database-connector-0.2.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:53.834680 ohdsi-database-connector-0.2.2/ohdsi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:53.834680 ohdsi-database-connector-0.2.2/ohdsi/database_connector/
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-07-14 10:13:44.000000 ohdsi-database-connector-0.2.2/ohdsi/database_connector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:53.834680 ohdsi-database-connector-0.2.2/ohdsi/database_connector/java/
+-rw-r--r--   0 runner    (1001) docker     (123)  1004719 2023-07-14 10:13:44.000000 ohdsi-database-connector-0.2.2/ohdsi/database_connector/java/postgresql-42.2.18.jar
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:53.834680 ohdsi-database-connector-0.2.2/ohdsi_database_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-14 10:13:53.000000 ohdsi-database-connector-0.2.2/ohdsi_database_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-14 10:13:53.000000 ohdsi-database-connector-0.2.2/ohdsi_database_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:13:53.000000 ohdsi-database-connector-0.2.2/ohdsi_database_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-14 10:13:53.000000 ohdsi-database-connector-0.2.2/ohdsi_database_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 10:13:53.000000 ohdsi-database-connector-0.2.2/ohdsi_database_connector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 10:13:53.834680 ohdsi-database-connector-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-14 10:13:44.000000 ohdsi-database-connector-0.2.2/setup.py
```

### Comparing `ohdsi-database-connector-0.2.1/ohdsi/database_connector/__init__.py` & `ohdsi-database-connector-0.2.2/ohdsi/database_connector/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,22 @@
+import os
+
 from importlib.resources import files
 
 from rpy2.robjects.packages import importr
 from rpy2.robjects.vectors import ListVector
 from rpy2.robjects.methods import RS4
 
-
-database_connector_r = importr('DatabaseConnector')
+# When building documentation for the project, the following import will fail
+# as the package is not installed. In this case, we set the variable to None
+# so that the documentation can be built.
+if os.environ.get('IGNORE_R_IMPORTS', False):
+    database_connector_r = None
+else:
+    database_connector_r = importr('DatabaseConnector')
 
 
 class Connect:
 
     @staticmethod
     def create_connection_details(
         dbms: str, user: str | None = None, password: str | None = None,
```

### Comparing `ohdsi-database-connector-0.2.1/ohdsi/database_connector/java/postgresql-42.2.18.jar` & `ohdsi-database-connector-0.2.2/ohdsi/database_connector/java/postgresql-42.2.18.jar`

 * *Files identical despite different names*

### Comparing `ohdsi-database-connector-0.2.1/setup.py` & `ohdsi-database-connector-0.2.2/setup.py`

 * *Files identical despite different names*

