# Comparing `tmp/resoto-plugin-digitalocean-3.6.0.tar.gz` & `tmp/resoto-plugin-digitalocean-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-digitalocean-3.6.0.tar", last modified: Fri Jun 30 19:22:29 2023, max compression
+gzip compressed data, was "resoto-plugin-digitalocean-3.6.1.tar", last modified: Fri Jul 14 17:04:19 2023, max compression
```

## Comparing `resoto-plugin-digitalocean-3.6.0.tar` & `resoto-plugin-digitalocean-3.6.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:22:29.950440 resoto-plugin-digitalocean-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-30 19:22:29.950440 resoto-plugin-digitalocean-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:22:29.942439 resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean/
--rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15431 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    43858 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    20282 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:22:29.946439 resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-30 19:22:29.000000 resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-30 19:22:29.000000 resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:22:29.000000 resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-30 19:22:29.000000 resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:19:01.000000 resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-30 19:22:29.000000 resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-30 19:22:29.000000 resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-30 19:22:29.950440 resoto-plugin-digitalocean-3.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:22:29.946439 resoto-plugin-digitalocean-3.6.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:22:29.950440 resoto-plugin-digitalocean-3.6.0/test/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/cdns.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/domain_records.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/domains.py
--rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/droplets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/firewalls.py
--rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/floatingip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/k8s.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/loadbalancers.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/neighbor_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/projectresources.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/regions.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/registry_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/registry_repository_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/spaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/ssh_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/volumes.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/fixtures/vpcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25525 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-30 19:17:38.000000 resoto-plugin-digitalocean-3.6.0/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:04:19.017918 resoto-plugin-digitalocean-3.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 16:58:26.000000 resoto-plugin-digitalocean-3.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-14 17:04:19.017918 resoto-plugin-digitalocean-3.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-14 16:58:26.000000 resoto-plugin-digitalocean-3.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-14 16:58:26.000000 resoto-plugin-digitalocean-3.6.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:04:19.013918 resoto-plugin-digitalocean-3.6.1/resoto_plugin_digitalocean/
+-rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-07-14 16:58:26.000000 resoto-plugin-digitalocean-3.6.1/resoto_plugin_digitalocean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15431 2023-07-14 16:58:26.000000 resoto-plugin-digitalocean-3.6.1/resoto_plugin_digitalocean/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43858 2023-07-14 16:58:26.000000 resoto-plugin-digitalocean-3.6.1/resoto_plugin_digitalocean/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-14 16:58:26.000000 resoto-plugin-digitalocean-3.6.1/resoto_plugin_digitalocean/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20282 2023-07-14 16:58:26.000000 resoto-plugin-digitalocean-3.6.1/resoto_plugin_digitalocean/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-07-14 16:58:26.000000 resoto-plugin-digitalocean-3.6.1/resoto_plugin_digitalocean/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:04:19.013918 resoto-plugin-digitalocean-3.6.1/resoto_plugin_digitalocean.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-14 17:04:19.000000 resoto-plugin-digitalocean-3.6.1/resoto_plugin_digitalocean.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-14 17:04:19.000000 resoto-plugin-digitalocean-3.6.1/resoto_plugin_digitalocean.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:04:19.000000 resoto-plugin-digitalocean-3.6.1/resoto_plugin_digitalocean.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-14 17:04:19.000000 resoto-plugin-digitalocean-3.6.1/resoto_plugin_digitalocean.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:00:14.000000 resoto-plugin-digitalocean-3.6.1/resoto_plugin_digitalocean.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-14 17:04:19.000000 resoto-plugin-digitalocean-3.6.1/resoto_plugin_digitalocean.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-14 17:04:19.000000 resoto-plugin-digitalocean-3.6.1/resoto_plugin_digitalocean.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-14 17:04:19.021918 resoto-plugin-digitalocean-3.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:04:19.013918 resoto-plugin-digitalocean-3.6.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:58:26.000000 resoto-plugin-digitalocean-3.6.1/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:04:19.017918 resoto-plugin-digitalocean-3.6.1/test/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-14 16:58:26.000000 resoto-plugin-digitalocean-3.6.1/test/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-14 16:58:26.000000 resoto-plugin-digitalocean-3.6.1/test/fixtures/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-14 16:58:26.000000 resoto-plugin-digitalocean-3.6.1/test/fixtures/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-14 16:58:26.000000 resoto-plugin-digitalocean-3.6.1/test/fixtures/cdns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-14 16:58:26.000000 resoto-plugin-digitalocean-3.6.1/test/fixtures/certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-14 16:58:26.000000 resoto-plugin-digitalocean-3.6.1/test/fixtures/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-14 16:58:26.000000 resoto-plugin-digitalocean-3.6.1/test/fixtures/domain_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-14 16:58:26.000000 resoto-plugin-digitalocean-3.6.1/test/fixtures/domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-07-14 16:58:26.000000 resoto-plugin-digitalocean-3.6.1/test/fixtures/droplets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-14 16:58:26.000000 resoto-plugin-digitalocean-3.6.1/test/fixtures/firewalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-07-14 16:58:26.000000 resoto-plugin-digitalocean-3.6.1/test/fixtures/floatingip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-14 16:58:26.000000 resoto-plugin-digitalocean-3.6.1/test/fixtures/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-07-14 16:58:26.000000 resoto-plugin-digitalocean-3.6.1/test/fixtures/loadbalancers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-14 16:58:26.000000 resoto-plugin-digitalocean-3.6.1/test/fixtures/neighbor_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-14 16:58:26.000000 resoto-plugin-digitalocean-3.6.1/test/fixtures/projectresources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-14 16:58:26.000000 resoto-plugin-digitalocean-3.6.1/test/fixtures/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-07-14 16:58:26.000000 resoto-plugin-digitalocean-3.6.1/test/fixtures/regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-14 16:58:26.000000 resoto-plugin-digitalocean-3.6.1/test/fixtures/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-14 16:58:26.000000 resoto-plugin-digitalocean-3.6.1/test/fixtures/registry_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-14 16:58:26.000000 resoto-plugin-digitalocean-3.6.1/test/fixtures/registry_repository_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-14 16:58:26.000000 resoto-plugin-digitalocean-3.6.1/test/fixtures/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-14 16:58:26.000000 resoto-plugin-digitalocean-3.6.1/test/fixtures/spaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-14 16:58:26.000000 resoto-plugin-digitalocean-3.6.1/test/fixtures/ssh_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-14 16:58:26.000000 resoto-plugin-digitalocean-3.6.1/test/fixtures/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-14 16:58:26.000000 resoto-plugin-digitalocean-3.6.1/test/fixtures/volumes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-14 16:58:26.000000 resoto-plugin-digitalocean-3.6.1/test/fixtures/vpcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25525 2023-07-14 16:58:26.000000 resoto-plugin-digitalocean-3.6.1/test/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-14 16:58:26.000000 resoto-plugin-digitalocean-3.6.1/test/test_config.py
```

### Comparing `resoto-plugin-digitalocean-3.6.0/PKG-INFO` & `resoto-plugin-digitalocean-3.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-digitalocean
-Version: 3.6.0
+Version: 3.6.1
 Summary: Resoto DigitalOcean Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/digitalocean
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-digitalocean-3.6.0/pyproject.toml` & `resoto-plugin-digitalocean-3.6.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-digitalocean"
 description = "Resoto DigitalOcean Collector Plugin"
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
     "boto3",
     "requests",
     "botocore",
     "retrying"
 ]
 
 [project.optional-dependencies]
```

### Comparing `resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean/__init__.py` & `resoto-plugin-digitalocean-3.6.1/resoto_plugin_digitalocean/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, List, Tuple, cast
+from typing import Optional, List, Tuple, cast, Any
 
 from resoto_plugin_digitalocean.client import StreamingWrapper, get_team_credentials
 from resoto_plugin_digitalocean.collector import DigitalOceanTeamCollector
 from resoto_plugin_digitalocean.resources import DigitalOceanResource, DigitalOceanTeam
 from resoto_plugin_digitalocean.config import (
     DigitalOceanCollectorConfig,
     DigitalOceanTeamCredentials,
@@ -17,16 +17,16 @@
 from resotolib.baseresources import BaseResource
 import time
 
 
 class DigitalOceanCollectorPlugin(BaseCollectorPlugin):
     cloud = "digitalocean"
 
-    def __init__(self) -> None:
-        super().__init__()
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
+        super().__init__(*args, **kwargs)
         self.core_feedback: Optional[CoreFeedback] = None
 
     def collect(self) -> None:
         """This method is being called by resoto whenever the collector runs
 
         It is responsible for querying the cloud APIs for remote resources and adding
         them to the plugin graph.
@@ -83,15 +83,15 @@
             client = StreamingWrapper(
                 c.api_token,
                 c.spaces_keys.access_key if c.spaces_keys else None,
                 c.spaces_keys.secret_key if c.spaces_keys else None,
             )
             team_graph = self.collect_team(client, self.core_feedback.with_context("digitalocean"))
             if team_graph:
-                self.graph.merge(team_graph)
+                self.send_account_graph(team_graph)
 
     def collect_team(self, client: StreamingWrapper, feedback: CoreFeedback) -> Optional[Graph]:
         """Collects an individual team."""
         team_id = client.get_team_id()
         team = DigitalOceanTeam(id=team_id, tags={}, urn=f"do:team:{team_id}")
 
         try:
```

### Comparing `resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean/client.py` & `resoto-plugin-digitalocean-3.6.1/resoto_plugin_digitalocean/client.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean/collector.py` & `resoto-plugin-digitalocean-3.6.1/resoto_plugin_digitalocean/collector.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean/config.py` & `resoto-plugin-digitalocean-3.6.1/resoto_plugin_digitalocean/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean/resources.py` & `resoto-plugin-digitalocean-3.6.1/resoto_plugin_digitalocean/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean/utils.py` & `resoto-plugin-digitalocean-3.6.1/resoto_plugin_digitalocean/utils.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean.egg-info/PKG-INFO` & `resoto-plugin-digitalocean-3.6.1/resoto_plugin_digitalocean.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-digitalocean
-Version: 3.6.0
+Version: 3.6.1
 Summary: Resoto DigitalOcean Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/digitalocean
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-digitalocean-3.6.0/resoto_plugin_digitalocean.egg-info/SOURCES.txt` & `resoto-plugin-digitalocean-3.6.1/resoto_plugin_digitalocean.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.6.0/test/fixtures/__init__.py` & `resoto-plugin-digitalocean-3.6.1/test/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.6.0/test/fixtures/apps.py` & `resoto-plugin-digitalocean-3.6.1/test/fixtures/apps.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.6.0/test/fixtures/databases.py` & `resoto-plugin-digitalocean-3.6.1/test/fixtures/databases.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.6.0/test/fixtures/domain_records.py` & `resoto-plugin-digitalocean-3.6.1/test/fixtures/domain_records.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.6.0/test/fixtures/droplets.py` & `resoto-plugin-digitalocean-3.6.1/test/fixtures/droplets.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.6.0/test/fixtures/firewalls.py` & `resoto-plugin-digitalocean-3.6.1/test/fixtures/firewalls.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.6.0/test/fixtures/floatingip.py` & `resoto-plugin-digitalocean-3.6.1/test/fixtures/floatingip.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.6.0/test/fixtures/k8s.py` & `resoto-plugin-digitalocean-3.6.1/test/fixtures/k8s.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.6.0/test/fixtures/loadbalancers.py` & `resoto-plugin-digitalocean-3.6.1/test/fixtures/loadbalancers.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.6.0/test/fixtures/projectresources.py` & `resoto-plugin-digitalocean-3.6.1/test/fixtures/projectresources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.6.0/test/fixtures/projects.py` & `resoto-plugin-digitalocean-3.6.1/test/fixtures/projects.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.6.0/test/fixtures/regions.py` & `resoto-plugin-digitalocean-3.6.1/test/fixtures/regions.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.6.0/test/fixtures/registry_repositories.py` & `resoto-plugin-digitalocean-3.6.1/test/fixtures/registry_repositories.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.6.0/test/fixtures/tags.py` & `resoto-plugin-digitalocean-3.6.1/test/fixtures/tags.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.6.0/test/fixtures/volumes.py` & `resoto-plugin-digitalocean-3.6.1/test/fixtures/volumes.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.6.0/test/test_collector.py` & `resoto-plugin-digitalocean-3.6.1/test/test_collector.py`

 * *Files identical despite different names*

