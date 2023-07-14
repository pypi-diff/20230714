# Comparing `tmp/resoto-plugin-k8s-3.6.0.tar.gz` & `tmp/resoto-plugin-k8s-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-k8s-3.6.0.tar", last modified: Fri Jun 30 19:29:03 2023, max compression
+gzip compressed data, was "resoto-plugin-k8s-3.6.1.tar", last modified: Fri Jul 14 17:05:59 2023, max compression
```

## Comparing `resoto-plugin-k8s-3.6.0.tar` & `resoto-plugin-k8s-3.6.1.tar`

### file list

```diff
@@ -1,19 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:03.405045 resoto-plugin-k8s-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 19:24:06.000000 resoto-plugin-k8s-3.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-30 19:29:03.405045 resoto-plugin-k8s-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-30 19:24:06.000000 resoto-plugin-k8s-3.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-30 19:24:06.000000 resoto-plugin-k8s-3.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:03.405045 resoto-plugin-k8s-3.6.0/resoto_plugin_k8s/
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-06-30 19:24:06.000000 resoto-plugin-k8s-3.6.0/resoto_plugin_k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19406 2023-06-30 19:24:06.000000 resoto-plugin-k8s-3.6.0/resoto_plugin_k8s/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-30 19:24:06.000000 resoto-plugin-k8s-3.6.0/resoto_plugin_k8s/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)   106651 2023-06-30 19:24:06.000000 resoto-plugin-k8s-3.6.0/resoto_plugin_k8s/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:03.405045 resoto-plugin-k8s-3.6.0/resoto_plugin_k8s.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-30 19:29:03.000000 resoto-plugin-k8s-3.6.0/resoto_plugin_k8s.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-30 19:29:03.000000 resoto-plugin-k8s-3.6.0/resoto_plugin_k8s.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:29:03.000000 resoto-plugin-k8s-3.6.0/resoto_plugin_k8s.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-30 19:29:03.000000 resoto-plugin-k8s-3.6.0/resoto_plugin_k8s.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:25:36.000000 resoto-plugin-k8s-3.6.0/resoto_plugin_k8s.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-30 19:29:03.000000 resoto-plugin-k8s-3.6.0/resoto_plugin_k8s.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 19:29:03.000000 resoto-plugin-k8s-3.6.0/resoto_plugin_k8s.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-30 19:29:03.405045 resoto-plugin-k8s-3.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:59.821883 resoto-plugin-k8s-3.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 17:01:23.000000 resoto-plugin-k8s-3.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-14 17:05:59.821883 resoto-plugin-k8s-3.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-14 17:01:23.000000 resoto-plugin-k8s-3.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-14 17:01:23.000000 resoto-plugin-k8s-3.6.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:59.821883 resoto-plugin-k8s-3.6.1/resoto_plugin_k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-07-14 17:01:23.000000 resoto-plugin-k8s-3.6.1/resoto_plugin_k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19406 2023-07-14 17:01:23.000000 resoto-plugin-k8s-3.6.1/resoto_plugin_k8s/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-14 17:01:23.000000 resoto-plugin-k8s-3.6.1/resoto_plugin_k8s/collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:59.821883 resoto-plugin-k8s-3.6.1/resoto_plugin_k8s/deferred_edges/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-14 17:01:23.000000 resoto-plugin-k8s-3.6.1/resoto_plugin_k8s/deferred_edges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-07-14 17:01:23.000000 resoto-plugin-k8s-3.6.1/resoto_plugin_k8s/deferred_edges/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-14 17:01:23.000000 resoto-plugin-k8s-3.6.1/resoto_plugin_k8s/deferred_edges/digitalocean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-14 17:01:23.000000 resoto-plugin-k8s-3.6.1/resoto_plugin_k8s/deferred_edges/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   106651 2023-07-14 17:01:23.000000 resoto-plugin-k8s-3.6.1/resoto_plugin_k8s/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:59.821883 resoto-plugin-k8s-3.6.1/resoto_plugin_k8s.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-14 17:05:59.000000 resoto-plugin-k8s-3.6.1/resoto_plugin_k8s.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-14 17:05:59.000000 resoto-plugin-k8s-3.6.1/resoto_plugin_k8s.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:05:59.000000 resoto-plugin-k8s-3.6.1/resoto_plugin_k8s.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-14 17:05:59.000000 resoto-plugin-k8s-3.6.1/resoto_plugin_k8s.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:02:43.000000 resoto-plugin-k8s-3.6.1/resoto_plugin_k8s.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-14 17:05:59.000000 resoto-plugin-k8s-3.6.1/resoto_plugin_k8s.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 17:05:59.000000 resoto-plugin-k8s-3.6.1/resoto_plugin_k8s.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-14 17:05:59.821883 resoto-plugin-k8s-3.6.1/setup.cfg
```

### Comparing `resoto-plugin-k8s-3.6.0/PKG-INFO` & `resoto-plugin-k8s-3.6.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-k8s
-Version: 3.6.0
+Version: 3.6.1
 Summary: Resoto Kubernetes Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/k8s
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-k8s-3.6.0/pyproject.toml` & `resoto-plugin-k8s-3.6.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-k8s"
 description = "Resoto Kubernetes Collector Plugin"
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
     "kubernetes",
 ]
 
 [project.entry-points."resoto.plugins"]
 k8s_collector = "resoto_plugin_k8s:KubernetesCollectorPlugin"
 
 [project.urls]
```

### Comparing `resoto-plugin-k8s-3.6.0/resoto_plugin_k8s/__init__.py` & `resoto-plugin-k8s-3.6.1/resoto_plugin_k8s/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,28 +9,29 @@
 import resotolib.proc
 from kubernetes.client import ApiException
 from kubernetes.client import Configuration
 
 from resoto_plugin_k8s.base import K8sApiClient, K8sClient
 from resoto_plugin_k8s.collector import KubernetesCollector
 from resoto_plugin_k8s.base import K8sConfig
+from resoto_plugin_k8s.deferred_edges import create_deferred_edges
 from resotolib.args import ArgumentParser, Namespace
 from resotolib.baseplugin import BaseCollectorPlugin
 from resotolib.config import Config, RunningConfig
 from resotolib.core.actions import CoreFeedback
 from resotolib.graph import Graph
 
 log = logging.getLogger("resoto.plugins.k8s")
 
 
 class KubernetesCollectorPlugin(BaseCollectorPlugin):
     cloud = "k8s"
 
-    def __init__(self) -> None:
-        super().__init__()
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
+        super().__init__(*args, **kwargs)
         # once defined, it will be set by the worker
         self.core_feedback: Optional[CoreFeedback] = None
 
     def collect(self, **kwargs: Any) -> None:
         log.debug("plugin: Kubernetes collecting resources")
         assert self.core_feedback, "core_feedback is not set"
 
@@ -42,15 +43,15 @@
                 log.warning("Kubernetes plugin enabled, but no clusters configured. Ignore.")
                 return
 
             max_workers = len(cluster_access) if len(cluster_access) < k8s.pool_size else k8s.pool_size
             pool_args: Dict[str, Any] = {"max_workers": max_workers}
             if k8s.fork_process:
                 pool_args["mp_context"] = multiprocessing.get_context("spawn")
-                pool_args["initializer"] = resotolib.proc.initializer
+                pool_args["initializer"] = resotolib.proc.collector_initializer
                 pool_executor: Type[Executor] = futures.ProcessPoolExecutor
             else:
                 pool_executor = futures.ThreadPoolExecutor
 
             with pool_executor(**pool_args) as executor:
                 wait_for = [
                     executor.submit(
@@ -65,15 +66,15 @@
                     for cluster_id, cluster_config in cluster_access.items()
                 ]
                 for future in futures.as_completed(wait_for):
                     cluster_graph = future.result()
                     if not isinstance(cluster_graph, Graph):
                         log.error(f"Skipping invalid cluster_graph {type(cluster_graph)}")
                         continue
-                    self.graph.merge(cluster_graph)
+                    self.send_account_graph(cluster_graph)
 
     @staticmethod
     def collect_cluster(
         cluster_id: str,
         cluster_config: Configuration,
         args: Namespace,
         running_config: RunningConfig,
@@ -94,14 +95,15 @@
 
         try:
             k8s_client: K8sClient = kwargs.get("client_factory", K8sApiClient.from_config)(
                 cluster_id, cluster_config
             ).with_feedback(core_feedback)
             kc = KubernetesCollector(Config.k8s, k8s_client)
             kc.collect()
+            create_deferred_edges(kc.graph)
         except ApiException as e:
             if e.reason == "Unauthorized":
                 core_feedback.error(f"Unable to authenticate with {cluster_id}", log)
             else:
                 core_feedback.error(f"An unhandled error occurred while collecting {cluster_id}: {e}", log)
             raise
         except Exception as e:
```

### Comparing `resoto-plugin-k8s-3.6.0/resoto_plugin_k8s/base.py` & `resoto-plugin-k8s-3.6.1/resoto_plugin_k8s/base.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-k8s-3.6.0/resoto_plugin_k8s/collector.py` & `resoto-plugin-k8s-3.6.1/resoto_plugin_k8s/collector.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-k8s-3.6.0/resoto_plugin_k8s/resources.py` & `resoto-plugin-k8s-3.6.1/resoto_plugin_k8s/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-k8s-3.6.0/resoto_plugin_k8s.egg-info/PKG-INFO` & `resoto-plugin-k8s-3.6.1/resoto_plugin_k8s.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-k8s
-Version: 3.6.0
+Version: 3.6.1
 Summary: Resoto Kubernetes Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/k8s
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

