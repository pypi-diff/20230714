# Comparing `tmp/resoto-plugin-dockerhub-3.6.0.tar.gz` & `tmp/resoto-plugin-dockerhub-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-dockerhub-3.6.0.tar", last modified: Fri Jun 30 19:26:40 2023, max compression
+gzip compressed data, was "resoto-plugin-dockerhub-3.6.1.tar", last modified: Fri Jul 14 17:05:19 2023, max compression
```

## Comparing `resoto-plugin-dockerhub-3.6.0.tar` & `resoto-plugin-dockerhub-3.6.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:26:40.202747 resoto-plugin-dockerhub-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 19:23:24.000000 resoto-plugin-dockerhub-3.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-30 19:26:40.202747 resoto-plugin-dockerhub-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-30 19:23:24.000000 resoto-plugin-dockerhub-3.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-30 19:23:24.000000 resoto-plugin-dockerhub-3.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:26:40.202747 resoto-plugin-dockerhub-3.6.0/resoto_plugin_dockerhub/
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-30 19:23:24.000000 resoto-plugin-dockerhub-3.6.0/resoto_plugin_dockerhub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-30 19:23:24.000000 resoto-plugin-dockerhub-3.6.0/resoto_plugin_dockerhub/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-30 19:23:24.000000 resoto-plugin-dockerhub-3.6.0/resoto_plugin_dockerhub/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:26:40.202747 resoto-plugin-dockerhub-3.6.0/resoto_plugin_dockerhub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-30 19:26:40.000000 resoto-plugin-dockerhub-3.6.0/resoto_plugin_dockerhub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-30 19:26:40.000000 resoto-plugin-dockerhub-3.6.0/resoto_plugin_dockerhub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:26:40.000000 resoto-plugin-dockerhub-3.6.0/resoto_plugin_dockerhub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-30 19:26:40.000000 resoto-plugin-dockerhub-3.6.0/resoto_plugin_dockerhub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:24:40.000000 resoto-plugin-dockerhub-3.6.0/resoto_plugin_dockerhub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-30 19:26:40.000000 resoto-plugin-dockerhub-3.6.0/resoto_plugin_dockerhub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-30 19:26:40.000000 resoto-plugin-dockerhub-3.6.0/resoto_plugin_dockerhub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-30 19:26:40.202747 resoto-plugin-dockerhub-3.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:26:40.202747 resoto-plugin-dockerhub-3.6.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-30 19:23:24.000000 resoto-plugin-dockerhub-3.6.0/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:19.033009 resoto-plugin-dockerhub-3.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 17:01:44.000000 resoto-plugin-dockerhub-3.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-14 17:05:19.033009 resoto-plugin-dockerhub-3.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-14 17:01:44.000000 resoto-plugin-dockerhub-3.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-14 17:01:44.000000 resoto-plugin-dockerhub-3.6.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:19.033009 resoto-plugin-dockerhub-3.6.1/resoto_plugin_dockerhub/
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-14 17:01:44.000000 resoto-plugin-dockerhub-3.6.1/resoto_plugin_dockerhub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-14 17:01:44.000000 resoto-plugin-dockerhub-3.6.1/resoto_plugin_dockerhub/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-14 17:01:44.000000 resoto-plugin-dockerhub-3.6.1/resoto_plugin_dockerhub/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:19.033009 resoto-plugin-dockerhub-3.6.1/resoto_plugin_dockerhub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-14 17:05:19.000000 resoto-plugin-dockerhub-3.6.1/resoto_plugin_dockerhub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-14 17:05:19.000000 resoto-plugin-dockerhub-3.6.1/resoto_plugin_dockerhub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:05:19.000000 resoto-plugin-dockerhub-3.6.1/resoto_plugin_dockerhub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-14 17:05:19.000000 resoto-plugin-dockerhub-3.6.1/resoto_plugin_dockerhub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:03:09.000000 resoto-plugin-dockerhub-3.6.1/resoto_plugin_dockerhub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-14 17:05:19.000000 resoto-plugin-dockerhub-3.6.1/resoto_plugin_dockerhub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-14 17:05:19.000000 resoto-plugin-dockerhub-3.6.1/resoto_plugin_dockerhub.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-14 17:05:19.033009 resoto-plugin-dockerhub-3.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:19.033009 resoto-plugin-dockerhub-3.6.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-14 17:01:44.000000 resoto-plugin-dockerhub-3.6.1/test/test_config.py
```

### Comparing `resoto-plugin-dockerhub-3.6.0/PKG-INFO` & `resoto-plugin-dockerhub-3.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-dockerhub
-Version: 3.6.0
+Version: 3.6.1
 Summary: Resoto Docker Hub Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/dockerhub
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-dockerhub-3.6.0/README.md` & `resoto-plugin-dockerhub-3.6.1/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-dockerhub-3.6.0/pyproject.toml` & `resoto-plugin-dockerhub-3.6.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-dockerhub"
 description = "Resoto Docker Hub Collector Plugin"
-version = "3.6.0"
+version = "3.6.1"
 authors = [{name="Some Engineering Inc."}]
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
     # Audience
@@ -23,15 +23,15 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "resotolib==3.6.0",
+    "resotolib==3.6.1",
     "requests",
 
 ]
 
 [project.entry-points."resoto.plugins"]
 dockerhub = "resoto_plugin_dockerhub:DockerHubCollectorPlugin"
```

### Comparing `resoto-plugin-dockerhub-3.6.0/resoto_plugin_dockerhub/__init__.py` & `resoto-plugin-dockerhub-3.6.1/resoto_plugin_dockerhub/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import requests
 from resotolib.logger import log
 from resotolib.baseplugin import BaseCollectorPlugin
 from resotolib.config import Config
 from .config import DockerHubConfig
-from typing import Optional
+from typing import Optional, Any
 from .resources import (
     DockerHubNamespace,
     DockerHubRepository,
 )
 
 
 class DockerHubCollectorPlugin(BaseCollectorPlugin):
     cloud = "dockerhub"
 
-    def __init__(self, *args, **kwargs) -> None:
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
         self.dockerhub_uri = "https://hub.docker.com/v2/repositories/"
 
     def collect(self) -> None:
         log.debug("plugin: collecting Docker Hub resources")
 
         for namespace in Config.dockerhub.namespaces:
```

### Comparing `resoto-plugin-dockerhub-3.6.0/resoto_plugin_dockerhub/resources.py` & `resoto-plugin-dockerhub-3.6.1/resoto_plugin_dockerhub/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-dockerhub-3.6.0/resoto_plugin_dockerhub.egg-info/PKG-INFO` & `resoto-plugin-dockerhub-3.6.1/resoto_plugin_dockerhub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-dockerhub
-Version: 3.6.0
+Version: 3.6.1
 Summary: Resoto Docker Hub Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/dockerhub
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

