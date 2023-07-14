# Comparing `tmp/botocore-a-la-carte-dax-1.31.2.tar.gz` & `tmp/botocore-a-la-carte-dax-1.31.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-dax-1.31.2.tar", last modified: Wed Jul 12 01:44:28 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-dax-1.31.3.tar", last modified: Fri Jul 14 01:46:04 2023, max compression
```

## Comparing `botocore-a-la-carte-dax-1.31.2.tar` & `botocore-a-la-carte-dax-1.31.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:28.739164 botocore-a-la-carte-dax-1.31.2/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-12 01:44:28.000000 botocore-a-la-carte-dax-1.31.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-12 01:44:28.739164 botocore-a-la-carte-dax-1.31.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:28.735164 botocore-a-la-carte-dax-1.31.2/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:28.735164 botocore-a-la-carte-dax-1.31.2/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:28.735164 botocore-a-la-carte-dax-1.31.2/botocore/data/dax/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:28.735164 botocore-a-la-carte-dax-1.31.2/botocore/data/dax/2017-04-19/
--rw-r--r--   0 runner    (1001) docker     (123)    13118 2023-07-12 01:44:12.000000 botocore-a-la-carte-dax-1.31.2/botocore/data/dax/2017-04-19/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-12 01:44:12.000000 botocore-a-la-carte-dax-1.31.2/botocore/data/dax/2017-04-19/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-12 01:44:12.000000 botocore-a-la-carte-dax-1.31.2/botocore/data/dax/2017-04-19/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    68163 2023-07-12 01:44:12.000000 botocore-a-la-carte-dax-1.31.2/botocore/data/dax/2017-04-19/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:28.735164 botocore-a-la-carte-dax-1.31.2/botocore_a_la_carte_dax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-12 01:44:28.000000 botocore-a-la-carte-dax-1.31.2/botocore_a_la_carte_dax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-12 01:44:28.000000 botocore-a-la-carte-dax-1.31.2/botocore_a_la_carte_dax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 01:44:28.000000 botocore-a-la-carte-dax-1.31.2/botocore_a_la_carte_dax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 01:44:28.000000 botocore-a-la-carte-dax-1.31.2/botocore_a_la_carte_dax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 01:44:28.739164 botocore-a-la-carte-dax-1.31.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-12 01:44:28.000000 botocore-a-la-carte-dax-1.31.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:04.822601 botocore-a-la-carte-dax-1.31.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-14 01:46:04.000000 botocore-a-la-carte-dax-1.31.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-14 01:46:04.822601 botocore-a-la-carte-dax-1.31.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:04.822601 botocore-a-la-carte-dax-1.31.3/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:04.822601 botocore-a-la-carte-dax-1.31.3/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:04.822601 botocore-a-la-carte-dax-1.31.3/botocore/data/dax/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:04.822601 botocore-a-la-carte-dax-1.31.3/botocore/data/dax/2017-04-19/
+-rw-r--r--   0 runner    (1001) docker     (123)    13118 2023-07-14 01:45:45.000000 botocore-a-la-carte-dax-1.31.3/botocore/data/dax/2017-04-19/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-14 01:45:45.000000 botocore-a-la-carte-dax-1.31.3/botocore/data/dax/2017-04-19/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-14 01:45:45.000000 botocore-a-la-carte-dax-1.31.3/botocore/data/dax/2017-04-19/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    68163 2023-07-14 01:45:45.000000 botocore-a-la-carte-dax-1.31.3/botocore/data/dax/2017-04-19/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:04.822601 botocore-a-la-carte-dax-1.31.3/botocore_a_la_carte_dax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-14 01:46:04.000000 botocore-a-la-carte-dax-1.31.3/botocore_a_la_carte_dax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-14 01:46:04.000000 botocore-a-la-carte-dax-1.31.3/botocore_a_la_carte_dax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 01:46:04.000000 botocore-a-la-carte-dax-1.31.3/botocore_a_la_carte_dax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 01:46:04.000000 botocore-a-la-carte-dax-1.31.3/botocore_a_la_carte_dax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 01:46:04.822601 botocore-a-la-carte-dax-1.31.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-14 01:46:04.000000 botocore-a-la-carte-dax-1.31.3/setup.py
```

### Comparing `botocore-a-la-carte-dax-1.31.2/LICENSE.txt` & `botocore-a-la-carte-dax-1.31.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-dax-1.31.2/PKG-INFO` & `botocore-a-la-carte-dax-1.31.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-dax
-Version: 1.31.2
+Version: 1.31.3
 Summary: dax data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-dax-1.31.2/botocore/data/dax/2017-04-19/endpoint-rule-set-1.json` & `botocore-a-la-carte-dax-1.31.3/botocore/data/dax/2017-04-19/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-dax-1.31.2/botocore/data/dax/2017-04-19/paginators-1.json` & `botocore-a-la-carte-dax-1.31.3/botocore/data/dax/2017-04-19/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-dax-1.31.2/botocore/data/dax/2017-04-19/service-2.json` & `botocore-a-la-carte-dax-1.31.3/botocore/data/dax/2017-04-19/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-dax-1.31.2/botocore_a_la_carte_dax.egg-info/PKG-INFO` & `botocore-a-la-carte-dax-1.31.3/botocore_a_la_carte_dax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-dax
-Version: 1.31.2
+Version: 1.31.3
 Summary: dax data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-dax-1.31.2/setup.py` & `botocore-a-la-carte-dax-1.31.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-dax',
-    version="1.31.2",
+    version="1.31.3",
     description='dax data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/dax/*/*.json'],
```

