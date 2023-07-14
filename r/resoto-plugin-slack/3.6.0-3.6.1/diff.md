# Comparing `tmp/resoto-plugin-slack-3.6.0.tar.gz` & `tmp/resoto-plugin-slack-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-slack-3.6.0.tar", last modified: Fri Jun 30 19:21:51 2023, max compression
+gzip compressed data, was "resoto-plugin-slack-3.6.1.tar", last modified: Fri Jul 14 17:00:06 2023, max compression
```

## Comparing `resoto-plugin-slack-3.6.0.tar` & `resoto-plugin-slack-3.6.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:51.175455 resoto-plugin-slack-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 19:18:31.000000 resoto-plugin-slack-3.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-30 19:21:51.175455 resoto-plugin-slack-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-30 19:18:31.000000 resoto-plugin-slack-3.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-30 19:18:31.000000 resoto-plugin-slack-3.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:51.175455 resoto-plugin-slack-3.6.0/resoto_plugin_slack/
--rw-r--r--   0 runner    (1001) docker     (123)    11689 2023-06-30 19:18:31.000000 resoto-plugin-slack-3.6.0/resoto_plugin_slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-30 19:18:31.000000 resoto-plugin-slack-3.6.0/resoto_plugin_slack/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-06-30 19:18:31.000000 resoto-plugin-slack-3.6.0/resoto_plugin_slack/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:51.175455 resoto-plugin-slack-3.6.0/resoto_plugin_slack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-30 19:21:51.000000 resoto-plugin-slack-3.6.0/resoto_plugin_slack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-30 19:21:51.000000 resoto-plugin-slack-3.6.0/resoto_plugin_slack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:21:51.000000 resoto-plugin-slack-3.6.0/resoto_plugin_slack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-30 19:21:51.000000 resoto-plugin-slack-3.6.0/resoto_plugin_slack.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:19:50.000000 resoto-plugin-slack-3.6.0/resoto_plugin_slack.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-30 19:21:51.000000 resoto-plugin-slack-3.6.0/resoto_plugin_slack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-30 19:21:51.000000 resoto-plugin-slack-3.6.0/resoto_plugin_slack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-30 19:21:51.175455 resoto-plugin-slack-3.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:51.175455 resoto-plugin-slack-3.6.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-30 19:18:31.000000 resoto-plugin-slack-3.6.0/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:00:06.174583 resoto-plugin-slack-3.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 16:56:01.000000 resoto-plugin-slack-3.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-14 17:00:06.174583 resoto-plugin-slack-3.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-14 16:56:01.000000 resoto-plugin-slack-3.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-14 16:56:01.000000 resoto-plugin-slack-3.6.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:00:06.174583 resoto-plugin-slack-3.6.1/resoto_plugin_slack/
+-rw-r--r--   0 runner    (1001) docker     (123)    11736 2023-07-14 16:56:01.000000 resoto-plugin-slack-3.6.1/resoto_plugin_slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-14 16:56:01.000000 resoto-plugin-slack-3.6.1/resoto_plugin_slack/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-07-14 16:56:01.000000 resoto-plugin-slack-3.6.1/resoto_plugin_slack/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:00:06.174583 resoto-plugin-slack-3.6.1/resoto_plugin_slack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-14 17:00:06.000000 resoto-plugin-slack-3.6.1/resoto_plugin_slack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-14 17:00:06.000000 resoto-plugin-slack-3.6.1/resoto_plugin_slack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:00:06.000000 resoto-plugin-slack-3.6.1/resoto_plugin_slack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-14 17:00:06.000000 resoto-plugin-slack-3.6.1/resoto_plugin_slack.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:57:38.000000 resoto-plugin-slack-3.6.1/resoto_plugin_slack.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-14 17:00:06.000000 resoto-plugin-slack-3.6.1/resoto_plugin_slack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-14 17:00:06.000000 resoto-plugin-slack-3.6.1/resoto_plugin_slack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-14 17:00:06.178583 resoto-plugin-slack-3.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:00:06.174583 resoto-plugin-slack-3.6.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-14 16:56:01.000000 resoto-plugin-slack-3.6.1/test/test_config.py
```

### Comparing `resoto-plugin-slack-3.6.0/PKG-INFO` & `resoto-plugin-slack-3.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-slack
-Version: 3.6.0
+Version: 3.6.1
 Summary: Resoto Slack Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/slack
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-slack-3.6.0/pyproject.toml` & `resoto-plugin-slack-3.6.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-slack"
 description = "Resoto Slack Plugin"
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
     "slack-sdk",
     "retrying",
 ]
 
 [project.entry-points."resoto.plugins"]
 slack_bot = "resoto_plugin_slack:SlackBotPlugin"
 slack_collector = "resoto_plugin_slack:SlackCollectorPlugin"
```

### Comparing `resoto-plugin-slack-3.6.0/resoto_plugin_slack/__init__.py` & `resoto-plugin-slack-3.6.1/resoto_plugin_slack/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import resotolib.logger
 import threading
 import time
 import ssl
 import slack_sdk
-from typing import List
+from typing import List, Any
 from retrying import retry
 
 from resotolib.utils import utc_str
 from .resources import (
     SlackRegion,
     SlackTeam,
     SlackUser,
@@ -38,16 +38,16 @@
             return True
     return False
 
 
 class SlackCollectorPlugin(BaseCollectorPlugin):
     cloud = "slack"
 
-    def __init__(self):
-        super().__init__()
+    def __init__(self, *args: Any, **kwargs: Any):
+        super().__init__(*args, **kwargs)
         self.client = None
 
     def collect(self) -> None:
         if not Config.slack.bot_token:
             log.info("Slack Collector Plugin: plugin loaded but no bot token provided")
             return
```

### Comparing `resoto-plugin-slack-3.6.0/resoto_plugin_slack/resources.py` & `resoto-plugin-slack-3.6.1/resoto_plugin_slack/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-slack-3.6.0/resoto_plugin_slack.egg-info/PKG-INFO` & `resoto-plugin-slack-3.6.1/resoto_plugin_slack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-slack
-Version: 3.6.0
+Version: 3.6.1
 Summary: Resoto Slack Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/slack
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

