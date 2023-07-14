# Comparing `tmp/resoto-plugin-gcp-3.6.0.tar.gz` & `tmp/resoto-plugin-gcp-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-gcp-3.6.0.tar", last modified: Fri Jun 30 19:31:54 2023, max compression
+gzip compressed data, was "resoto-plugin-gcp-3.6.1.tar", last modified: Fri Jul 14 17:02:09 2023, max compression
```

## Comparing `resoto-plugin-gcp-3.6.0.tar` & `resoto-plugin-gcp-3.6.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:31:54.380810 resoto-plugin-gcp-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-30 19:31:54.380810 resoto-plugin-gcp-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:31:54.372810 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/gcp_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:31:54.376810 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25320 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12979 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/resources/billing.py
--rw-r--r--   0 runner    (1001) docker     (123)   284432 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/resources/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    49819 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/resources/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    40556 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/resources/sqladmin.py
--rw-r--r--   0 runner    (1001) docker     (123)    15271 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/resources/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:31:54.372810 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-30 19:31:54.000000 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-30 19:31:54.000000 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:31:54.000000 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-30 19:31:54.000000 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:26:13.000000 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-30 19:31:54.000000 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-30 19:31:54.000000 resoto-plugin-gcp-3.6.0/resoto_plugin_gcp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-30 19:31:54.380810 resoto-plugin-gcp-3.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:31:54.380810 resoto-plugin-gcp-3.6.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/test/random_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/test/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/test/test_billing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/test/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)    12850 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/test/test_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/test/test_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/test/test_sqladmin.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-30 19:24:28.000000 resoto-plugin-gcp-3.6.0/test/test_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:02:09.617871 resoto-plugin-gcp-3.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-14 17:02:09.617871 resoto-plugin-gcp-3.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:02:09.617871 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/gcp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:02:09.617871 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25320 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12979 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/resources/billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)   284432 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/resources/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49819 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/resources/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40556 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/resources/sqladmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15271 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/resources/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:02:09.617871 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-14 17:02:09.000000 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-14 17:02:09.000000 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:02:09.000000 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-14 17:02:09.000000 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:57:50.000000 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-14 17:02:09.000000 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-14 17:02:09.000000 resoto-plugin-gcp-3.6.1/resoto_plugin_gcp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-14 17:02:09.621871 resoto-plugin-gcp-3.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:02:09.617871 resoto-plugin-gcp-3.6.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/test/random_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/test/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/test/test_billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/test/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12850 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/test/test_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/test/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/test/test_sqladmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-14 16:56:30.000000 resoto-plugin-gcp-3.6.1/test/test_storage.py
```

### Comparing `resoto-plugin-gcp-3.6.0/PKG-INFO` & `resoto-plugin-gcp-3.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-gcp
-Version: 3.6.0
+Version: 3.6.1
 Summary: Resoto GCP Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/gcp
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-gcp-3.6.0/pyproject.toml` & `resoto-plugin-gcp-3.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-gcp"
 description = "Resoto GCP Collector Plugin"
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
     "google-api-python-client",
     "oauth2client",
     "retrying",
     "tenacity",
 ]
 
 [project.entry-points."resoto.plugins"]
```

### Comparing `resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/__init__.py` & `resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 
     Gets instantiated in resoto's Processor thread. The collect() method
     is run during a resource collection loop.
     """
 
     cloud = "gcp"
 
-    def __init__(self) -> None:
-        super().__init__()
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
+        super().__init__(*args, **kwargs)
         self.core_feedback: Optional[CoreFeedback] = None
 
     def collect(self) -> None:
         """Run by resoto during the global collect() run.
 
         This method kicks off code that adds GCP resources to `self.graph`.
         When collect() finishes the parent thread will take `self.graph` and merge
@@ -75,15 +75,16 @@
                 for project_id in credentials.keys()
             ]
             for future in futures.as_completed(wait_for):
                 project_graph = future.result()
                 if not isinstance(project_graph, Graph):
                     log.error(f"Skipping invalid project_graph {type(project_graph)}")
                     continue
-                self.graph.merge(project_graph)
+                self.send_account_graph(project_graph)
+                del project_graph
 
     @staticmethod
     def collect_project(
         project_id: str,
         core_feedback: CoreFeedback,
         cloud: Cloud,
         args: Optional[Namespace] = None,
@@ -129,15 +130,15 @@
     @staticmethod
     def add_config(config: Config) -> None:
         """Called by resoto upon startup to populate the Config store"""
         config.add_config(GcpConfig)
 
 
 def collect_project_proxy(*args, queue: multiprocessing.Queue, **kwargs) -> None:  # type: ignore
-    resotolib.proc.initializer()
+    resotolib.proc.collector_initializer()
     queue.put(GCPCollectorPlugin.collect_project(*args, **kwargs))
 
 
 def collect_in_process(*args, **kwargs) -> Optional[Graph]:  # type: ignore
     ctx = multiprocessing.get_context("spawn")
     queue = ctx.Queue()
     kwargs["queue"] = queue
```

### Comparing `resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/collector.py` & `resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/collector.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/config.py` & `resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/gcp_client.py` & `resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/gcp_client.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/resources/base.py` & `resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/resources/base.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/resources/billing.py` & `resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/resources/billing.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/resources/compute.py` & `resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/resources/compute.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/resources/container.py` & `resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/resources/container.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/resources/sqladmin.py` & `resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/resources/sqladmin.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/resources/storage.py` & `resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/resources/storage.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.0/resoto_plugin_gcp/utils.py` & `resoto-plugin-gcp-3.6.1/resoto_plugin_gcp/utils.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.0/resoto_plugin_gcp.egg-info/PKG-INFO` & `resoto-plugin-gcp-3.6.1/resoto_plugin_gcp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-gcp
-Version: 3.6.0
+Version: 3.6.1
 Summary: Resoto GCP Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/gcp
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-gcp-3.6.0/resoto_plugin_gcp.egg-info/SOURCES.txt` & `resoto-plugin-gcp-3.6.1/resoto_plugin_gcp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.0/test/conftest.py` & `resoto-plugin-gcp-3.6.1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.0/test/random_client.py` & `resoto-plugin-gcp-3.6.1/test/random_client.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.0/test/test_base.py` & `resoto-plugin-gcp-3.6.1/test/test_base.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.0/test/test_billing.py` & `resoto-plugin-gcp-3.6.1/test/test_billing.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.0/test/test_collector.py` & `resoto-plugin-gcp-3.6.1/test/test_collector.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.0/test/test_compute.py` & `resoto-plugin-gcp-3.6.1/test/test_compute.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.0/test/test_config.py` & `resoto-plugin-gcp-3.6.1/test/test_config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.0/test/test_container.py` & `resoto-plugin-gcp-3.6.1/test/test_container.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.6.0/test/test_sqladmin.py` & `resoto-plugin-gcp-3.6.1/test/test_sqladmin.py`

 * *Files identical despite different names*

