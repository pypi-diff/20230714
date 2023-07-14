# Comparing `tmp/botocore-a-la-carte-wellarchitected-1.31.2.tar.gz` & `tmp/botocore-a-la-carte-wellarchitected-1.31.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-wellarchitected-1.31.2.tar", last modified: Wed Jul 12 01:45:02 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-wellarchitected-1.31.3.tar", last modified: Fri Jul 14 01:46:45 2023, max compression
```

## Comparing `botocore-a-la-carte-wellarchitected-1.31.2.tar` & `botocore-a-la-carte-wellarchitected-1.31.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:45:02.587524 botocore-a-la-carte-wellarchitected-1.31.2/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-12 01:45:02.000000 botocore-a-la-carte-wellarchitected-1.31.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-12 01:45:02.587524 botocore-a-la-carte-wellarchitected-1.31.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:45:02.587524 botocore-a-la-carte-wellarchitected-1.31.2/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:45:02.587524 botocore-a-la-carte-wellarchitected-1.31.2/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:45:02.587524 botocore-a-la-carte-wellarchitected-1.31.2/botocore/data/wellarchitected/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:45:02.587524 botocore-a-la-carte-wellarchitected-1.31.2/botocore/data/wellarchitected/2020-03-31/
--rw-r--r--   0 runner    (1001) docker     (123)    17660 2023-07-12 01:44:12.000000 botocore-a-la-carte-wellarchitected-1.31.2/botocore/data/wellarchitected/2020-03-31/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-12 01:44:12.000000 botocore-a-la-carte-wellarchitected-1.31.2/botocore/data/wellarchitected/2020-03-31/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-12 01:44:12.000000 botocore-a-la-carte-wellarchitected-1.31.2/botocore/data/wellarchitected/2020-03-31/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   156541 2023-07-12 01:44:12.000000 botocore-a-la-carte-wellarchitected-1.31.2/botocore/data/wellarchitected/2020-03-31/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:45:02.587524 botocore-a-la-carte-wellarchitected-1.31.2/botocore_a_la_carte_wellarchitected.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-12 01:45:02.000000 botocore-a-la-carte-wellarchitected-1.31.2/botocore_a_la_carte_wellarchitected.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-12 01:45:02.000000 botocore-a-la-carte-wellarchitected-1.31.2/botocore_a_la_carte_wellarchitected.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 01:45:02.000000 botocore-a-la-carte-wellarchitected-1.31.2/botocore_a_la_carte_wellarchitected.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 01:45:02.000000 botocore-a-la-carte-wellarchitected-1.31.2/botocore_a_la_carte_wellarchitected.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 01:45:02.587524 botocore-a-la-carte-wellarchitected-1.31.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-12 01:45:02.000000 botocore-a-la-carte-wellarchitected-1.31.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:45.187025 botocore-a-la-carte-wellarchitected-1.31.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-14 01:46:44.000000 botocore-a-la-carte-wellarchitected-1.31.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-14 01:46:45.187025 botocore-a-la-carte-wellarchitected-1.31.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:45.183025 botocore-a-la-carte-wellarchitected-1.31.3/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:45.183025 botocore-a-la-carte-wellarchitected-1.31.3/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:45.187025 botocore-a-la-carte-wellarchitected-1.31.3/botocore/data/wellarchitected/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:45.187025 botocore-a-la-carte-wellarchitected-1.31.3/botocore/data/wellarchitected/2020-03-31/
+-rw-r--r--   0 runner    (1001) docker     (123)    17660 2023-07-14 01:45:45.000000 botocore-a-la-carte-wellarchitected-1.31.3/botocore/data/wellarchitected/2020-03-31/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-14 01:45:45.000000 botocore-a-la-carte-wellarchitected-1.31.3/botocore/data/wellarchitected/2020-03-31/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-14 01:45:45.000000 botocore-a-la-carte-wellarchitected-1.31.3/botocore/data/wellarchitected/2020-03-31/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   156541 2023-07-14 01:45:45.000000 botocore-a-la-carte-wellarchitected-1.31.3/botocore/data/wellarchitected/2020-03-31/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:45.187025 botocore-a-la-carte-wellarchitected-1.31.3/botocore_a_la_carte_wellarchitected.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-14 01:46:45.000000 botocore-a-la-carte-wellarchitected-1.31.3/botocore_a_la_carte_wellarchitected.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-14 01:46:45.000000 botocore-a-la-carte-wellarchitected-1.31.3/botocore_a_la_carte_wellarchitected.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 01:46:45.000000 botocore-a-la-carte-wellarchitected-1.31.3/botocore_a_la_carte_wellarchitected.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 01:46:45.000000 botocore-a-la-carte-wellarchitected-1.31.3/botocore_a_la_carte_wellarchitected.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 01:46:45.187025 botocore-a-la-carte-wellarchitected-1.31.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-14 01:46:44.000000 botocore-a-la-carte-wellarchitected-1.31.3/setup.py
```

### Comparing `botocore-a-la-carte-wellarchitected-1.31.2/LICENSE.txt` & `botocore-a-la-carte-wellarchitected-1.31.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-wellarchitected-1.31.2/PKG-INFO` & `botocore-a-la-carte-wellarchitected-1.31.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-wellarchitected
-Version: 1.31.2
+Version: 1.31.3
 Summary: wellarchitected data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-wellarchitected-1.31.2/botocore/data/wellarchitected/2020-03-31/endpoint-rule-set-1.json` & `botocore-a-la-carte-wellarchitected-1.31.3/botocore/data/wellarchitected/2020-03-31/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-wellarchitected-1.31.2/botocore/data/wellarchitected/2020-03-31/service-2.json` & `botocore-a-la-carte-wellarchitected-1.31.3/botocore/data/wellarchitected/2020-03-31/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-wellarchitected-1.31.2/botocore_a_la_carte_wellarchitected.egg-info/PKG-INFO` & `botocore-a-la-carte-wellarchitected-1.31.3/botocore_a_la_carte_wellarchitected.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-wellarchitected
-Version: 1.31.2
+Version: 1.31.3
 Summary: wellarchitected data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-wellarchitected-1.31.2/setup.py` & `botocore-a-la-carte-wellarchitected-1.31.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-wellarchitected',
-    version="1.31.2",
+    version="1.31.3",
     description='wellarchitected data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/wellarchitected/*/*.json'],
```

