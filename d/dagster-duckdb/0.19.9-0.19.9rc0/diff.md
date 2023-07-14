# Comparing `tmp/dagster-duckdb-0.19.9.tar.gz` & `tmp/dagster-duckdb-0.19.9rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-duckdb-0.19.9.tar", last modified: Thu Jun  8 18:52:54 2023, max compression
+gzip compressed data, was "dagster-duckdb-0.19.9rc0.tar", last modified: Thu Jun  8 18:28:18 2023, max compression
```

## Comparing `dagster-duckdb-0.19.9.tar` & `dagster-duckdb-0.19.9rc0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:52:54.299859 dagster-duckdb-0.19.9/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 18:43:17.000000 dagster-duckdb-0.19.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       48 2023-06-08 18:43:17.000000 dagster-duckdb-0.19.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-08 18:52:54.303859 dagster-duckdb-0.19.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      128 2023-06-08 18:43:17.000000 dagster-duckdb-0.19.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:52:54.299859 dagster-duckdb-0.19.9/dagster_duckdb/
--rw-r--r--   0 root         (0) root         (0)      336 2023-06-08 18:43:17.000000 dagster-duckdb-0.19.9/dagster_duckdb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9444 2023-06-08 18:43:17.000000 dagster-duckdb-0.19.9/dagster_duckdb/io_manager.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-08 18:43:17.000000 dagster-duckdb-0.19.9/dagster_duckdb/py.typed
--rw-r--r--   0 root         (0) root         (0)     1280 2023-06-08 18:43:17.000000 dagster-duckdb-0.19.9/dagster_duckdb/resource.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-08 18:43:17.000000 dagster-duckdb-0.19.9/dagster_duckdb/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:52:54.299859 dagster-duckdb-0.19.9/dagster_duckdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-08 18:52:54.000000 dagster-duckdb-0.19.9/dagster_duckdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      407 2023-06-08 18:52:54.000000 dagster-duckdb-0.19.9/dagster_duckdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:52:54.000000 dagster-duckdb-0.19.9/dagster_duckdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:52:54.000000 dagster-duckdb-0.19.9/dagster_duckdb.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      149 2023-06-08 18:52:54.000000 dagster-duckdb-0.19.9/dagster_duckdb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-08 18:52:54.000000 dagster-duckdb-0.19.9/dagster_duckdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      125 2023-06-08 18:52:54.303859 dagster-duckdb-0.19.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1544 2023-06-08 18:43:17.000000 dagster-duckdb-0.19.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:18.362675 dagster-duckdb-0.19.9rc0/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 18:20:46.000000 dagster-duckdb-0.19.9rc0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       48 2023-06-08 18:20:46.000000 dagster-duckdb-0.19.9rc0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      695 2023-06-08 18:28:18.362675 dagster-duckdb-0.19.9rc0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      128 2023-06-08 18:20:46.000000 dagster-duckdb-0.19.9rc0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:18.362675 dagster-duckdb-0.19.9rc0/dagster_duckdb/
+-rw-r--r--   0 root         (0) root         (0)      336 2023-06-08 18:20:46.000000 dagster-duckdb-0.19.9rc0/dagster_duckdb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9444 2023-06-08 18:20:46.000000 dagster-duckdb-0.19.9rc0/dagster_duckdb/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-08 18:20:46.000000 dagster-duckdb-0.19.9rc0/dagster_duckdb/py.typed
+-rw-r--r--   0 root         (0) root         (0)     1280 2023-06-08 18:20:46.000000 dagster-duckdb-0.19.9rc0/dagster_duckdb/resource.py
+-rw-r--r--   0 root         (0) root         (0)       26 2023-06-08 18:20:46.000000 dagster-duckdb-0.19.9rc0/dagster_duckdb/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:18.362675 dagster-duckdb-0.19.9rc0/dagster_duckdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      695 2023-06-08 18:28:18.000000 dagster-duckdb-0.19.9rc0/dagster_duckdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      407 2023-06-08 18:28:18.000000 dagster-duckdb-0.19.9rc0/dagster_duckdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:28:18.000000 dagster-duckdb-0.19.9rc0/dagster_duckdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:28:18.000000 dagster-duckdb-0.19.9rc0/dagster_duckdb.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      152 2023-06-08 18:28:18.000000 dagster-duckdb-0.19.9rc0/dagster_duckdb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-08 18:28:18.000000 dagster-duckdb-0.19.9rc0/dagster_duckdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      125 2023-06-08 18:28:18.366675 dagster-duckdb-0.19.9rc0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1547 2023-06-08 18:20:46.000000 dagster-duckdb-0.19.9rc0/setup.py
```

### Comparing `dagster-duckdb-0.19.9/LICENSE` & `dagster-duckdb-0.19.9rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-0.19.9/PKG-INFO` & `dagster-duckdb-0.19.9rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb
-Version: 0.19.9
+Version: 0.19.9rc0
 Summary: Package for DuckDB-specific Dagster framework op and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-duckdb-0.19.9/dagster_duckdb/io_manager.py` & `dagster-duckdb-0.19.9rc0/dagster_duckdb/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-0.19.9/dagster_duckdb/resource.py` & `dagster-duckdb-0.19.9rc0/dagster_duckdb/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-0.19.9/dagster_duckdb.egg-info/PKG-INFO` & `dagster-duckdb-0.19.9rc0/dagster_duckdb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb
-Version: 0.19.9
+Version: 0.19.9rc0
 Summary: Package for DuckDB-specific Dagster framework op and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-duckdb-0.19.9/setup.py` & `dagster-duckdb-0.19.9rc0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_duckdb_tests*"]),
     include_package_data=True,
     install_requires=[
         "duckdb",
-        "dagster==1.3.9",
+        "dagster==1.3.9rc0",
     ],
     extras_require={
         "pandas": ["pandas"],
         # Pyspark 2.x is incompatible with Python 3.8+
         "pyspark": [
             'pyspark>=3.0.0; python_version >= "3.8"',
             'pyspark>=2.0.2; python_version < "3.8"',
```

