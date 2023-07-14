# Comparing `tmp/cipromote-1.1.0.tar.gz` & `tmp/cipromote-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cipromote-1.1.0.tar", max compression
+gzip compressed data, was "cipromote-1.2.0.tar", max compression
```

## Comparing `cipromote-1.1.0.tar` & `cipromote-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       68 2023-03-13 15:43:49.230739 cipromote-1.1.0/README.md
--rw-r--r--   0        0        0      548 2023-07-13 21:37:44.536819 cipromote-1.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-01 21:23:03.887994 cipromote-1.1.0/src/cipromote/__init__.py
--rw-r--r--   0        0        0    25204 2023-03-01 22:01:52.712793 cipromote-1.1.0/src/cipromote/ci-cli.py
--rw-r--r--   0        0        0     9801 2023-07-13 21:37:03.560306 cipromote-1.1.0/src/cipromote/cli.py
--rw-r--r--   0        0        0      114 2023-03-01 22:01:52.717793 cipromote-1.1.0/src/cipromote/constants.py
--rw-r--r--   0        0        0     1680 2023-03-02 20:06:52.453096 cipromote-1.1.0/src/cipromote/instances.py
--rw-r--r--   0        0        0     5708 2023-03-02 21:27:59.317150 cipromote-1.1.0/src/cipromote/label_versions.py
--rw-r--r--   0        0        0     3889 2023-03-02 20:55:55.574572 cipromote-1.1.0/src/cipromote/labels.py
--rw-r--r--   0        0        0      387 2023-03-02 15:58:17.336622 cipromote-1.1.0/src/cipromote/login.py
--rw-r--r--   0        0        0     3510 2023-03-02 15:12:46.158566 cipromote-1.1.0/src/cipromote/loginInput.py
--rw-r--r--   0        0        0     2981 2023-03-02 19:49:52.016215 cipromote-1.1.0/src/cipromote/projects.py
--rw-r--r--   0        0        0    11691 2023-03-01 22:01:52.726793 cipromote-1.1.0/src/cipromote/queries.py
--rw-r--r--   0        0        0     2158 2023-03-01 22:01:52.728793 cipromote-1.1.0/src/cipromote/versioned_items.py
--rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 cipromote-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0       68 2023-03-13 15:43:49.230739 cipromote-1.2.0/README.md
+-rw-r--r--   0        0        0      548 2023-07-14 11:50:44.367941 cipromote-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-01 21:23:03.887994 cipromote-1.2.0/src/cipromote/__init__.py
+-rw-r--r--   0        0        0    25204 2023-03-01 22:01:52.712793 cipromote-1.2.0/src/cipromote/ci-cli.py
+-rw-r--r--   0        0        0    10721 2023-07-14 11:50:00.910215 cipromote-1.2.0/src/cipromote/cli.py
+-rw-r--r--   0        0        0      114 2023-03-01 22:01:52.717793 cipromote-1.2.0/src/cipromote/constants.py
+-rw-r--r--   0        0        0     1680 2023-03-02 20:06:52.453096 cipromote-1.2.0/src/cipromote/instances.py
+-rw-r--r--   0        0        0     5708 2023-03-02 21:27:59.317150 cipromote-1.2.0/src/cipromote/label_versions.py
+-rw-r--r--   0        0        0     3889 2023-03-02 20:55:55.574572 cipromote-1.2.0/src/cipromote/labels.py
+-rw-r--r--   0        0        0      387 2023-03-02 15:58:17.336622 cipromote-1.2.0/src/cipromote/login.py
+-rw-r--r--   0        0        0     3510 2023-03-02 15:12:46.158566 cipromote-1.2.0/src/cipromote/loginInput.py
+-rw-r--r--   0        0        0     2981 2023-03-02 19:49:52.016215 cipromote-1.2.0/src/cipromote/projects.py
+-rw-r--r--   0        0        0    11691 2023-03-01 22:01:52.726793 cipromote-1.2.0/src/cipromote/queries.py
+-rw-r--r--   0        0        0     2158 2023-03-01 22:01:52.728793 cipromote-1.2.0/src/cipromote/versioned_items.py
+-rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 cipromote-1.2.0/PKG-INFO
```

### Comparing `cipromote-1.1.0/pyproject.toml` & `cipromote-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cipromote"
-version = "1.1.0"
+version = "1.2.0"
 description = "Promote MotionCI Labels"
 authors = ["Michael MacKenna <mmackenna@ufginsurance.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^8.1.3"
```

### Comparing `cipromote-1.1.0/src/cipromote/ci-cli.py` & `cipromote-1.2.0/src/cipromote/ci-cli.py`

 * *Files identical despite different names*

### Comparing `cipromote-1.1.0/src/cipromote/cli.py` & `cipromote-1.2.0/src/cipromote/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """ Core module with cli """
 import click
 import json
 import sys
 import os
+import time
 import requests
 import cipromote.constants as constants
 import cipromote.instances as instances
 import cipromote.queries as queries
 import cipromote.loginInput as loginInput
 import cipromote.login as login
 import cipromote.labels as labels
@@ -82,14 +83,34 @@
     for instance in instance_object:
         if instance['node']['name'].lower() == instance_name.lower():
             target_instance = instance['node']
             print(f"The target instance is {target_instance['name']}")
             pprint(target_instance)
     return target_instance
 
+@main.command("monitor-instance", short_help="Check an instance by name every X seconds")
+@click.argument("instance-name")
+@click.argument("seconds")
+def get_instance(instance_name, seconds):
+    """ Check a particular instance by name every X seconds """
+    server_url = os.getenv("MOTIOCI_SERVERURL")
+    constants.CI_URL = server_url
+    constants.GRAPH_URL = constants.CI_URL + constants.GRAPH_URL
+    print('Sending query to the following url')
+    print(constants.GRAPH_URL)
+    while True:
+        instance_object = instances.get_instances_default()
+        for instance in instance_object:
+            if instance['node']['name'].lower() == instance_name.lower():
+                target_instance = instance['node']
+                print(f"The target instance is {target_instance['name']}")
+                pprint(target_instance)
+                time.sleep(int(seconds))
+    return target_instance
+
 @main.command("check-instance-namespace", short_help="Check if a particular namespace is present")
 @click.argument("instance-name")
 @click.argument("namespace-name")
 def check_instance_namespace(instance_name, namespace_name):
     """ Check if a particular namespace is present in a particular instance """
     server_url = os.getenv("MOTIOCI_SERVERURL")
     constants.CI_URL = server_url
```

### Comparing `cipromote-1.1.0/src/cipromote/instances.py` & `cipromote-1.2.0/src/cipromote/instances.py`

 * *Files identical despite different names*

### Comparing `cipromote-1.1.0/src/cipromote/label_versions.py` & `cipromote-1.2.0/src/cipromote/label_versions.py`

 * *Files identical despite different names*

### Comparing `cipromote-1.1.0/src/cipromote/labels.py` & `cipromote-1.2.0/src/cipromote/labels.py`

 * *Files identical despite different names*

### Comparing `cipromote-1.1.0/src/cipromote/loginInput.py` & `cipromote-1.2.0/src/cipromote/loginInput.py`

 * *Files identical despite different names*

### Comparing `cipromote-1.1.0/src/cipromote/projects.py` & `cipromote-1.2.0/src/cipromote/projects.py`

 * *Files identical despite different names*

### Comparing `cipromote-1.1.0/src/cipromote/queries.py` & `cipromote-1.2.0/src/cipromote/queries.py`

 * *Files identical despite different names*

### Comparing `cipromote-1.1.0/src/cipromote/versioned_items.py` & `cipromote-1.2.0/src/cipromote/versioned_items.py`

 * *Files identical despite different names*

### Comparing `cipromote-1.1.0/PKG-INFO` & `cipromote-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cipromote
-Version: 1.1.0
+Version: 1.2.0
 Summary: Promote MotionCI Labels
 Author: Michael MacKenna
 Author-email: mmackenna@ufginsurance.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

