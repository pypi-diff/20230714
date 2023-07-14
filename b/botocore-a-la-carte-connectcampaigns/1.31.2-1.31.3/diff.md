# Comparing `tmp/botocore-a-la-carte-connectcampaigns-1.31.2.tar.gz` & `tmp/botocore-a-la-carte-connectcampaigns-1.31.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-connectcampaigns-1.31.2.tar", last modified: Wed Jul 12 01:44:26 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-connectcampaigns-1.31.3.tar", last modified: Fri Jul 14 01:46:01 2023, max compression
```

## Comparing `botocore-a-la-carte-connectcampaigns-1.31.2.tar` & `botocore-a-la-carte-connectcampaigns-1.31.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:26.071133 botocore-a-la-carte-connectcampaigns-1.31.2/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-12 01:44:25.000000 botocore-a-la-carte-connectcampaigns-1.31.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-12 01:44:26.071133 botocore-a-la-carte-connectcampaigns-1.31.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:26.067133 botocore-a-la-carte-connectcampaigns-1.31.2/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:26.071133 botocore-a-la-carte-connectcampaigns-1.31.2/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:26.071133 botocore-a-la-carte-connectcampaigns-1.31.2/botocore/data/connectcampaigns/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:26.071133 botocore-a-la-carte-connectcampaigns-1.31.2/botocore/data/connectcampaigns/2021-01-30/
--rw-r--r--   0 runner    (1001) docker     (123)    13174 2023-07-12 01:44:12.000000 botocore-a-la-carte-connectcampaigns-1.31.2/botocore/data/connectcampaigns/2021-01-30/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-12 01:44:12.000000 botocore-a-la-carte-connectcampaigns-1.31.2/botocore/data/connectcampaigns/2021-01-30/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    43506 2023-07-12 01:44:12.000000 botocore-a-la-carte-connectcampaigns-1.31.2/botocore/data/connectcampaigns/2021-01-30/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:26.071133 botocore-a-la-carte-connectcampaigns-1.31.2/botocore_a_la_carte_connectcampaigns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-12 01:44:26.000000 botocore-a-la-carte-connectcampaigns-1.31.2/botocore_a_la_carte_connectcampaigns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-12 01:44:26.000000 botocore-a-la-carte-connectcampaigns-1.31.2/botocore_a_la_carte_connectcampaigns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 01:44:26.000000 botocore-a-la-carte-connectcampaigns-1.31.2/botocore_a_la_carte_connectcampaigns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 01:44:26.000000 botocore-a-la-carte-connectcampaigns-1.31.2/botocore_a_la_carte_connectcampaigns.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 01:44:26.071133 botocore-a-la-carte-connectcampaigns-1.31.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-12 01:44:25.000000 botocore-a-la-carte-connectcampaigns-1.31.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:01.698569 botocore-a-la-carte-connectcampaigns-1.31.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-14 01:46:01.000000 botocore-a-la-carte-connectcampaigns-1.31.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-14 01:46:01.698569 botocore-a-la-carte-connectcampaigns-1.31.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:01.698569 botocore-a-la-carte-connectcampaigns-1.31.3/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:01.698569 botocore-a-la-carte-connectcampaigns-1.31.3/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:01.698569 botocore-a-la-carte-connectcampaigns-1.31.3/botocore/data/connectcampaigns/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:01.698569 botocore-a-la-carte-connectcampaigns-1.31.3/botocore/data/connectcampaigns/2021-01-30/
+-rw-r--r--   0 runner    (1001) docker     (123)    13174 2023-07-14 01:45:45.000000 botocore-a-la-carte-connectcampaigns-1.31.3/botocore/data/connectcampaigns/2021-01-30/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-14 01:45:45.000000 botocore-a-la-carte-connectcampaigns-1.31.3/botocore/data/connectcampaigns/2021-01-30/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    43506 2023-07-14 01:45:45.000000 botocore-a-la-carte-connectcampaigns-1.31.3/botocore/data/connectcampaigns/2021-01-30/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:01.698569 botocore-a-la-carte-connectcampaigns-1.31.3/botocore_a_la_carte_connectcampaigns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-14 01:46:01.000000 botocore-a-la-carte-connectcampaigns-1.31.3/botocore_a_la_carte_connectcampaigns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-14 01:46:01.000000 botocore-a-la-carte-connectcampaigns-1.31.3/botocore_a_la_carte_connectcampaigns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 01:46:01.000000 botocore-a-la-carte-connectcampaigns-1.31.3/botocore_a_la_carte_connectcampaigns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 01:46:01.000000 botocore-a-la-carte-connectcampaigns-1.31.3/botocore_a_la_carte_connectcampaigns.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 01:46:01.698569 botocore-a-la-carte-connectcampaigns-1.31.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-14 01:46:01.000000 botocore-a-la-carte-connectcampaigns-1.31.3/setup.py
```

### Comparing `botocore-a-la-carte-connectcampaigns-1.31.2/LICENSE.txt` & `botocore-a-la-carte-connectcampaigns-1.31.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-connectcampaigns-1.31.2/PKG-INFO` & `botocore-a-la-carte-connectcampaigns-1.31.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-connectcampaigns
-Version: 1.31.2
+Version: 1.31.3
 Summary: connectcampaigns data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-connectcampaigns-1.31.2/botocore/data/connectcampaigns/2021-01-30/endpoint-rule-set-1.json` & `botocore-a-la-carte-connectcampaigns-1.31.3/botocore/data/connectcampaigns/2021-01-30/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-connectcampaigns-1.31.2/botocore/data/connectcampaigns/2021-01-30/service-2.json` & `botocore-a-la-carte-connectcampaigns-1.31.3/botocore/data/connectcampaigns/2021-01-30/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-connectcampaigns-1.31.2/botocore_a_la_carte_connectcampaigns.egg-info/PKG-INFO` & `botocore-a-la-carte-connectcampaigns-1.31.3/botocore_a_la_carte_connectcampaigns.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-connectcampaigns
-Version: 1.31.2
+Version: 1.31.3
 Summary: connectcampaigns data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-connectcampaigns-1.31.2/setup.py` & `botocore-a-la-carte-connectcampaigns-1.31.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-connectcampaigns',
-    version="1.31.2",
+    version="1.31.3",
     description='connectcampaigns data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/connectcampaigns/*/*.json'],
```

