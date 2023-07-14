# Comparing `tmp/resotoworker-3.6.0.tar.gz` & `tmp/resotoworker-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotoworker-3.6.0.tar", last modified: Fri Jun 30 19:24:16 2023, max compression
+gzip compressed data, was "resotoworker-3.6.1.tar", last modified: Fri Jul 14 17:02:11 2023, max compression
```

## Comparing `resotoworker-3.6.0.tar` & `resotoworker-3.6.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:16.857830 resotoworker-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 19:18:37.000000 resotoworker-3.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-30 19:24:16.857830 resotoworker-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-06-30 19:18:37.000000 resotoworker-3.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-30 19:18:37.000000 resotoworker-3.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:16.853830 resotoworker-3.6.0/resotoworker/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-30 19:18:37.000000 resotoworker-3.6.0/resotoworker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12171 2023-06-30 19:18:37.000000 resotoworker-3.6.0/resotoworker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-06-30 19:18:37.000000 resotoworker-3.6.0/resotoworker/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-06-30 19:18:37.000000 resotoworker-3.6.0/resotoworker/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-06-30 19:18:37.000000 resotoworker-3.6.0/resotoworker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-30 19:18:37.000000 resotoworker-3.6.0/resotoworker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-06-30 19:18:37.000000 resotoworker-3.6.0/resotoworker/pluginloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-30 19:18:37.000000 resotoworker-3.6.0/resotoworker/resotocore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-30 19:18:37.000000 resotoworker-3.6.0/resotoworker/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-30 19:18:37.000000 resotoworker-3.6.0/resotoworker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:16.857830 resotoworker-3.6.0/resotoworker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-30 19:24:16.000000 resotoworker-3.6.0/resotoworker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-30 19:24:16.000000 resotoworker-3.6.0/resotoworker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:24:16.000000 resotoworker-3.6.0/resotoworker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-30 19:24:16.000000 resotoworker-3.6.0/resotoworker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:20:15.000000 resotoworker-3.6.0/resotoworker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-30 19:24:16.000000 resotoworker-3.6.0/resotoworker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 19:24:16.000000 resotoworker-3.6.0/resotoworker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-30 19:24:16.857830 resotoworker-3.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:16.857830 resotoworker-3.6.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:18:37.000000 resotoworker-3.6.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-30 19:18:37.000000 resotoworker-3.6.0/test/fakeconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-30 19:18:37.000000 resotoworker-3.6.0/test/test_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-30 19:18:37.000000 resotoworker-3.6.0/test/test_collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-30 19:18:37.000000 resotoworker-3.6.0/test/test_resotocore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-06-30 19:18:37.000000 resotoworker-3.6.0/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:02:10.993684 resotoworker-3.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 16:56:59.000000 resotoworker-3.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-07-14 17:02:10.993684 resotoworker-3.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-07-14 16:56:59.000000 resotoworker-3.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-14 16:56:59.000000 resotoworker-3.6.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:02:10.993684 resotoworker-3.6.1/resotoworker/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-14 16:56:59.000000 resotoworker-3.6.1/resotoworker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-07-14 16:56:59.000000 resotoworker-3.6.1/resotoworker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-07-14 16:56:59.000000 resotoworker-3.6.1/resotoworker/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-07-14 16:56:59.000000 resotoworker-3.6.1/resotoworker/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-07-14 16:56:59.000000 resotoworker-3.6.1/resotoworker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-14 16:56:59.000000 resotoworker-3.6.1/resotoworker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-14 16:56:59.000000 resotoworker-3.6.1/resotoworker/pluginloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-07-14 16:56:59.000000 resotoworker-3.6.1/resotoworker/resotocore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-14 16:56:59.000000 resotoworker-3.6.1/resotoworker/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-14 16:56:59.000000 resotoworker-3.6.1/resotoworker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:02:10.993684 resotoworker-3.6.1/resotoworker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-07-14 17:02:10.000000 resotoworker-3.6.1/resotoworker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-14 17:02:10.000000 resotoworker-3.6.1/resotoworker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:02:10.000000 resotoworker-3.6.1/resotoworker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-14 17:02:10.000000 resotoworker-3.6.1/resotoworker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:58:37.000000 resotoworker-3.6.1/resotoworker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-14 17:02:10.000000 resotoworker-3.6.1/resotoworker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 17:02:10.000000 resotoworker-3.6.1/resotoworker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-14 17:02:10.993684 resotoworker-3.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:02:10.993684 resotoworker-3.6.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:56:59.000000 resotoworker-3.6.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-14 16:56:59.000000 resotoworker-3.6.1/test/fakeconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-14 16:56:59.000000 resotoworker-3.6.1/test/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-14 16:56:59.000000 resotoworker-3.6.1/test/test_collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-14 16:56:59.000000 resotoworker-3.6.1/test/test_resotocore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-14 16:56:59.000000 resotoworker-3.6.1/test/test_utils.py
```

### Comparing `resotoworker-3.6.0/PKG-INFO` & `resotoworker-3.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoworker
-Version: 3.6.0
+Version: 3.6.1
 Summary: Runs collector plugins and sends the result to resotocore.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotoworker
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `resotoworker-3.6.0/README.md` & `resotoworker-3.6.1/README.md`

 * *Files identical despite different names*

### Comparing `resotoworker-3.6.0/pyproject.toml` & `resotoworker-3.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 name = "resotoworker"
-version = "3.6.0"
+version = "3.6.1"
 authors = [{name="Some Engineering Inc."}]
 description = "Runs collector plugins and sends the result to resotocore."
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [ "Programming Language :: Python :: 3" ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "resotolib==3.6.0",
+    "resotolib==3.6.1",
     "tenacity",
     "CherryPy",
 ]
 
 [project.scripts]
 resotoworker = "resotoworker.__main__:main"
```

### Comparing `resotoworker-3.6.0/resotoworker/__main__.py` & `resotoworker-3.6.1/resotoworker/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from signal import SIGTERM
 from typing import List, Dict, Type, Optional, Any, Callable
 
 import requests
 
 import resotolib.proc
 from resotolib.args import ArgumentParser
-from resotolib.baseplugin import BaseActionPlugin, BasePostCollectPlugin, BaseCollectorPlugin, PluginType
+from resotolib.baseplugin import BaseActionPlugin, BaseCollectorPlugin, PluginType
 from resotolib.config import Config
 from resotolib.core import add_args as core_add_args, resotocore, wait_for_resotocore
 from resotolib.core.actions import CoreActions, CoreFeedback
 from resotolib.core.ca import TLSData
 from resotolib.core.tasks import CoreTasks, CoreTaskHandler
 from resotolib.event import (
     add_event_listener,
@@ -114,15 +114,15 @@
 
     core = Resotocore(send_request, config)
 
     # the multiprocessing manager is used to share data between processes
     mp_manager = multiprocessing.Manager()
     core_messages: Queue[Json] = mp_manager.Queue()
 
-    collector = Collector(config, core.send_to_resotocore, core_messages)
+    collector = Collector(config, core, core_messages)
 
     # Handle Ctrl+c and other means of termination/shutdown
     resotolib.proc.initializer()
     add_event_listener(EventType.SHUTDOWN, shutdown, blocking=False)
 
     # Try to increase nofile and nproc limits
     increase_limits()
@@ -220,38 +220,38 @@
     config: Config,
     plugin_loader: PluginLoader,
     tls_data: Optional[TLSData],
     collector: Collector,
     message: Dict[str, Any],
 ) -> Optional[Dict[str, Any]]:
     collectors: List[Type[BaseCollectorPlugin]] = plugin_loader.plugins(PluginType.COLLECTOR)  # type: ignore
-    post_collectors: List[Type[BasePostCollectPlugin]] = plugin_loader.plugins(PluginType.POST_COLLECT)  # type: ignore
     # todo: clean this up
     if not isinstance(message, dict):
         log.error(f"Invalid message: {message}")
         return None
     kind = message.get("kind")
     message_type = message.get("message_type")
     data = message.get("data") or {}
     task_id: str = data.get("task")  # type: ignore
     step_name: str = data.get("step")  # type: ignore
+
     log.debug(f"Received message of kind {kind}, type {message_type}, data: {data}")
     if kind == "action":
         try:
             if message_type == "collect":
                 start_time = time.time()
-                collector.collect_and_send(collectors, post_collectors, task_id=task_id, step_name=step_name)
+                collector.collect_and_send(collectors, task_data=data)
                 run_time = int(time.time() - start_time)
                 log.info(f"Collect ran for {run_time} seconds")
             elif message_type == "cleanup":
                 if not Config.resotoworker.cleanup:
-                    log.info("Cleanup called but disabled in config" " (resotoworker.cleanup) - skipping")
+                    log.info("Cleanup called but disabled in config (resotoworker.cleanup) - skipping")
                 else:
                     if Config.resotoworker.cleanup_dry_run:
-                        log.info("Cleanup called with dry run configured" " (resotoworker.cleanup_dry_run)")
+                        log.info("Cleanup called with dry run configured (resotoworker.cleanup_dry_run)")
                     start_time = time.time()
                     feedback = CoreFeedback(task_id, step_name, "cleanup", collector.core_messages)
                     cleanup(
                         config,
                         {p.cloud: p for p in collectors},
                         feedback,
                         tls_data=tls_data,
```

### Comparing `resotoworker-3.6.0/resotoworker/cleanup.py` & `resotoworker-3.6.1/resotoworker/cleanup.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.6.0/resotoworker/collect.py` & `resotoworker-3.6.1/resotoworker/collect.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,59 +1,102 @@
 import multiprocessing
+import threading
+from tempfile import mkdtemp
+from shutil import rmtree
 from queue import Queue
-
 import resotolib.proc
 from time import time
 from concurrent import futures
 from threading import Lock
 from resotoworker.exceptions import DuplicateMessageError
-from resotolib.baseplugin import BaseCollectorPlugin, BasePostCollectPlugin
-from resotolib.baseresources import GraphRoot
+from resotoworker.resotocore import Resotocore
+from resotolib.baseplugin import BaseCollectorPlugin
+from resotolib.baseresources import GraphRoot, BaseCloud, BaseAccount, BaseResource
 from resotolib.core.actions import CoreFeedback
-from resotolib.graph import Graph, sanitize
+from resotolib.graph import Graph, sanitize, GraphMergeKind
 from resotolib.logger import log, setup_logger
 from resotolib.args import ArgumentParser
 from argparse import Namespace
-from typing import List, Optional, Callable, Type, Dict, Any, Set
+from typing import List, Optional, Type, Dict, Any, Set
 from resotolib.config import Config, RunningConfig
 from resotolib.types import Json
 
 TaskId = str
 
 
 class Collector:
-    def __init__(
-        self, config: Config, send_to_resotocore: Callable[[Graph, TaskId], None], core_messages: Queue[Json]
-    ) -> None:
-        self._send_to_resotocore = send_to_resotocore
+    def __init__(self, config: Config, resotocore: Resotocore, core_messages: Queue[Json]) -> None:
+        self._resotocore = resotocore
         self._config = config
         self.core_messages = core_messages
         self.processing: Set[str] = set()
         self.processing_lock = Lock()
 
+    def graph_sender(self, graph_queue: Queue[Optional[Graph]], task_id: TaskId, tempdir: str) -> None:
+        log.debug("Waiting for collector graphs")
+        start_time = time()
+        while True:
+            collector_graph = graph_queue.get()
+            if collector_graph is None:
+                run_time = time() - start_time
+                log.debug(f"Ending graph sender thread for task id {task_id} after {run_time} seconds")
+                break
+
+            graph = Graph(root=GraphRoot(id="root", tags={}))
+            graph.merge(collector_graph)
+            del collector_graph
+            sanitize(graph)
+
+            graph_info = ""
+            assert isinstance(graph.root, BaseResource)
+            for cloud in graph.successors(graph.root):
+                if isinstance(cloud, BaseCloud):
+                    graph_info += f" {cloud.kdname}"
+                for account in graph.successors(cloud):
+                    if isinstance(account, BaseAccount):
+                        graph_info += f" {account.kdname}"
+
+            log.info(f"Received collector graph for{graph_info}")
+
+            if (cycle := graph.find_cycle()) is not None:
+                desc = ", ".join, [f"{key.edge_type}: {key.src.kdname}-->{key.dst.kdname}" for key in cycle]
+                log.error(f"Graph of {graph_info} is not acyclic - ignoring. Cycle {desc}")
+                continue
+
+            try:
+                self._resotocore.send_to_resotocore(graph, task_id, tempdir)
+            except Exception as e:
+                log.error(f"Error sending graph of {graph_info} to resotocore: {e}")
+            del graph
+
     def collect_and_send(
         self,
         collectors: List[Type[BaseCollectorPlugin]],
-        post_collectors: List[Type[BasePostCollectPlugin]],
-        task_id: str,
-        step_name: str,
+        task_data: Json,
     ) -> None:
+        task_id = task_data["task"]
+        step_name = task_data["step"]
         core_feedback = CoreFeedback(task_id, step_name, "collect", self.core_messages)
 
-        def collect(collectors: List[Type[BaseCollectorPlugin]]) -> Optional[Graph]:
-            graph = Graph(root=GraphRoot(id="root", tags={}))
+        def collect(
+            collectors: List[Type[BaseCollectorPlugin]],
+            graph_queue: Queue[Optional[Graph]],
+            task_data: Json,
+        ) -> bool:
+            all_success = True
+            graph_merge_kind = self._config.resotoworker.graph_merge_kind
 
             max_workers = (
                 len(collectors)
                 if len(collectors) < self._config.resotoworker.pool_size
                 else self._config.resotoworker.pool_size
             )
             if max_workers == 0:
                 log.error("No workers configured or no collector plugins loaded - skipping collect")
-                return None
+                return False
             pool_args = {"max_workers": max_workers}
             pool_executor: Type[futures.Executor]
             collect_args: Dict[str, Any]
             if self._config.resotoworker.fork_process:
                 pool_args["mp_context"] = multiprocessing.get_context("spawn")
                 pool_args["initializer"] = resotolib.proc.initializer
                 pool_executor = futures.ProcessPoolExecutor
@@ -67,125 +110,80 @@
 
             with pool_executor(**pool_args) as executor:
                 wait_for = [
                     executor.submit(
                         collect_plugin_graph,
                         collector,
                         core_feedback,
+                        graph_queue,
+                        graph_merge_kind,
+                        task_data=task_data,
                         **collect_args,
                     )
                     for collector in collectors
                 ]
                 for future in futures.as_completed(wait_for):
-                    collector_graph = future.result()
-                    if not isinstance(collector_graph, Graph):
-                        log.error(f"Skipping invalid collector graph {type(collector_graph)}")
-                        continue
-                    graph.merge(collector_graph)
-            sanitize(graph)
-            return graph
-
-        def post_collect(graph: Graph, post_collectors: List[Type[BasePostCollectPlugin]]) -> Graph:
-            if len(post_collectors) == 0:
-                log.info("No post-collect plugins loaded - skipping")
-                return graph
-            pool_args: Dict[str, Any] = {"max_workers": 1}
-            pool_executor: Type[futures.Executor]
-            collect_args: Dict[str, Any] = {}
-            if self._config.resotoworker.fork_process:
-                pool_args["mp_context"] = multiprocessing.get_context("spawn")
-                pool_args["initializer"] = resotolib.proc.initializer
-                pool_executor = futures.ProcessPoolExecutor
-                collect_args = {
-                    "args": ArgumentParser.args,
-                    "running_config": self._config.running_config,
-                }
-            else:
-                pool_executor = futures.ThreadPoolExecutor
-
-            with pool_executor(**pool_args) as executor:
-                for post_collector in post_collectors:
-                    future = executor.submit(
-                        run_post_collect_plugin, post_collector, graph, core_feedback, **collect_args
-                    )
-                    try:
-                        new_graph = future.result(Config.resotoworker.timeout)
-                    except TimeoutError as e:
-                        log.exception(f"Unhandled exception in {post_collector}: {e} - ignoring plugin")
-                        continue
-                    except Exception as e:
-                        log.exception(f"Unhandled exception in {post_collector}: {e} - ignoring plugin")
-                        continue
-
-                    if new_graph is None:
-                        continue
-                    graph = new_graph
-
-                sanitize(graph)
-                return graph
+                    collector_success = future.result()
+                    if not collector_success:
+                        all_success = False
+            return all_success
 
         processing_id = f"{task_id}:{step_name}"
         try:
             with self.processing_lock:
                 if processing_id in self.processing:
                     raise DuplicateMessageError(f"Already processing {processing_id} - ignoring message")
                 self.processing.add(processing_id)
 
-            collected = collect(collectors)
+            mp_manager = multiprocessing.Manager()
+            graph_queue: Queue[Optional[Graph]] = mp_manager.Queue()
+            graph_sender_threads = []
+            graph_sender_pool_size = self._config.resotoworker.graph_sender_pool_size
+            tempdir = mkdtemp(prefix=f"resoto-{task_id}", dir=self._config.resotoworker.tempdir)
+            try:
+                for i in range(graph_sender_pool_size):
+                    graph_sender_t = threading.Thread(
+                        target=self.graph_sender,
+                        args=(graph_queue, task_id, tempdir),
+                        name=f"graph_sender_{i}",
+                    )
+                    graph_sender_t.daemon = True
+                    graph_sender_t.start()
+                    graph_sender_threads.append(graph_sender_t)
+
+                self._resotocore.create_graph_and_update_model(tempdir=tempdir)
+                collect(collectors, graph_queue, task_data)
+            finally:
+                log.debug("Telling graph sender threads to end")
+                for _ in range(graph_sender_pool_size):
+                    graph_queue.put(None)
+                for t in graph_sender_threads:
+                    t.join(self._config.resotoworker.timeout)
+                if not self._config.resotoworker.debug_dump_json:
+                    rmtree(tempdir, ignore_errors=True)
 
-            if collected:
-                collected = post_collect(collected, post_collectors)
-                self._send_to_resotocore(collected, task_id)
         finally:
             with self.processing_lock:
                 if processing_id in self.processing:
                     self.processing.remove(processing_id)
 
 
-def run_post_collect_plugin(
-    post_collector_plugin: Type[BasePostCollectPlugin],
-    graph: Graph,
-    core_feedback: CoreFeedback,
-    args: Optional[Namespace] = None,
-    running_config: Optional[RunningConfig] = None,
-) -> Optional[Graph]:
-    try:
-        post_collector: BasePostCollectPlugin = post_collector_plugin()
-        if core_feedback and hasattr(post_collector, "core_feedback"):
-            setattr(post_collector, "core_feedback", core_feedback)
-
-        if args is not None:
-            ArgumentParser.args = args  # type: ignore
-            setup_logger("resotoworker")
-        if running_config is not None:
-            Config.running_config.apply(running_config)
-
-        log.debug(f"starting new post-collect process for {post_collector.name}")
-        start_time = time()
-        post_collector.post_collect(graph)
-        elapsed = time() - start_time
-        if (cycle := graph.find_cycle()) is not None:
-            desc = ", ".join, [f"{key.edge_type}: {key.src.kdname}-->{key.dst.kdname}" for key in cycle]
-            log.error(f"Graph of plugin {post_collector.name} is not acyclic - ignoring plugin results. Cycle {desc}")
-            return None
-        log.info(f"Collector of plugin {post_collector.name} finished in {elapsed:.4f}s")
-        return graph
-    except Exception as e:
-        log.exception(f"Unhandled exception in {post_collector_plugin}: {e} - ignoring plugin")
-        return None
-
-
 def collect_plugin_graph(
     collector_plugin: Type[BaseCollectorPlugin],
     core_feedback: CoreFeedback,
+    graph_queue: Queue[Optional[Graph]],
+    graph_merge_kind: GraphMergeKind,
+    task_data: Json,
     args: Optional[Namespace] = None,
     running_config: Optional[RunningConfig] = None,
-) -> Optional[Graph]:
+) -> bool:
     try:
-        collector: BaseCollectorPlugin = collector_plugin()
+        collector: BaseCollectorPlugin = collector_plugin(
+            graph_queue=graph_queue, graph_merge_kind=graph_merge_kind, task_data=task_data
+        )
         core_feedback.progress_done(collector.cloud, 0, 1)
         if core_feedback and hasattr(collector, "core_feedback"):
             setattr(collector, "core_feedback", core_feedback)
         collector_name = f"collector_{collector.cloud}"
         resotolib.proc.set_thread_name(collector_name)
 
         if args is not None:
@@ -199,20 +197,16 @@
         collector.start()
         collector.join(Config.resotoworker.timeout)
         core_feedback.progress_done(collector.cloud, 1, 1)
         elapsed = time() - start_time
         if not collector.is_alive():  # The plugin has finished its work
             if not collector.finished:
                 log.error(f"Plugin {collector.cloud} did not finish collection" " - ignoring plugin results")
-                return None
-            if (cycle := collector.graph.find_cycle()) is not None:
-                desc = ", ".join, [f"{key.edge_type}: {key.src.kdname}-->{key.dst.kdname}" for key in cycle]
-                log.error(f"Graph of plugin {collector.cloud} is not acyclic - ignoring plugin results. Cycle {desc}")
-                return None
+                return False
             log.info(f"Collector of plugin {collector.cloud} finished in {elapsed:.4f}s")
-            return collector.graph
+            return True
         else:
             log.error(f"Plugin {collector.cloud} timed out - discarding plugin graph")
-            return None
+            return False
     except Exception as e:
         log.exception(f"Unhandled exception in {collector_plugin}: {e} - ignoring plugin")
-        return None
+        return False
```

### Comparing `resotoworker-3.6.0/resotoworker/config.py` & `resotoworker-3.6.1/resotoworker/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,17 +54,20 @@
     )
     graph: str = field(
         default="resoto",
         metadata={"description": "Name of the graph to import data into and run searches on"},
     )
     timeout: int = field(default=10800, metadata={"description": "Collection/cleanup timeout in seconds"})
     pool_size: int = field(default=5, metadata={"description": "Collector thread/process pool size"})
+    graph_sender_pool_size: int = field(
+        default=5, metadata={"description": "Maximum number of graphs to send to the core concurrently"}
+    )
     fork_process: bool = field(default=True, metadata={"description": "Use forked process instead of threads"})
     graph_merge_kind: GraphMergeKind = field(
-        default=GraphMergeKind.cloud,
+        default=GraphMergeKind.account,
         metadata={"description": "Resource kind to merge graph at (cloud or account)"},
     )
     debug_dump_json: bool = field(default=False, metadata={"description": "Dump the generated JSON data to disk"})
     tempdir: Optional[str] = field(default=None, metadata={"description": "Directory to create temporary files in"})
     cleanup: bool = field(default=False, metadata={"description": "Enable cleanup of resources"})
     cleanup_pool_size: int = field(
         factory=lambda: num_default_threads() * 2,
```

### Comparing `resotoworker-3.6.0/resotoworker/pluginloader.py` & `resotoworker-3.6.1/resotoworker/pluginloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pkg_resources
 import inspect
 from resotolib.logger import log
 from typing import List, Optional, Type, Union, Dict, cast, Set
 from resotolib.args import ArgumentParser
 from resotolib.config import Config
-from resotolib.baseplugin import BaseCollectorPlugin, BasePostCollectPlugin, BasePlugin, BaseActionPlugin, PluginType
+from resotolib.baseplugin import BaseCollectorPlugin, BasePlugin, BaseActionPlugin, PluginType
 
 
 class PluginLoader:
     """resoto plugin loader"""
 
     def __init__(self, plugin_type: Optional[PluginType] = None) -> None:
         # self.__plugins is a dict with key PluginType and value List
@@ -47,50 +47,41 @@
         self._initialized = True
 
     def add_plugin(self, plugin: Union[Type[BasePlugin], Type[BaseActionPlugin]]) -> bool:
         """Adds a Plugin class to the list of Plugins"""
         if (
             inspect.isclass(plugin)
             and not inspect.isabstract(plugin)
-            and issubclass(plugin, (BasePlugin, BaseActionPlugin, BasePostCollectPlugin))
+            and issubclass(plugin, (BasePlugin, BaseActionPlugin))
             and plugin.plugin_type in self._plugins
         ):
             log.debug(f"Found plugin {plugin} ({plugin.plugin_type.name})")
             if plugin not in self._plugins[plugin.plugin_type]:
                 self._plugins[plugin.plugin_type].append(plugin)
         return True
 
-    def plugins(
-        self, plugin_type: PluginType
-    ) -> List[Union[Type[BasePlugin], Type[BaseActionPlugin], Type[BasePostCollectPlugin]]]:
+    def plugins(self, plugin_type: PluginType) -> List[Union[Type[BasePlugin], Type[BaseActionPlugin]]]:
         """Returns the list of Plugins of a certain PluginType"""
         if not self._initialized:
             self.find_plugins()
         configured_collectors: Set[str] = set(Config.resotoworker.collector)
 
-        if plugin_type == PluginType.POST_COLLECT:
-            post_collect_plugins = cast(List[Type[BasePostCollectPlugin]], self._plugins.get(plugin_type, []))
-            return [
-                plugin
-                for plugin in post_collect_plugins
-                if plugin.activate_with.issubset(configured_collectors) or plugin.name in configured_collectors
-            ]
-        elif plugin_type == PluginType.COLLECTOR:
+        if plugin_type == PluginType.COLLECTOR:
             plugins: List[Type[BaseCollectorPlugin]] = self._plugins.get(plugin_type, [])  # type: ignore
             return [plugin for plugin in plugins if plugin.cloud in configured_collectors]
 
-        return self._plugins.get(plugin_type, [])  # type: ignore
+        return self._plugins.get(plugin_type, [])
 
     def all_plugins(
         self, plugin_type: Optional[PluginType] = None
-    ) -> List[Union[Type[BasePlugin], Type[BaseActionPlugin], Type[BasePostCollectPlugin]]]:
+    ) -> List[Union[Type[BasePlugin], Type[BaseActionPlugin]]]:
         if not self._initialized:
             self.find_plugins()
         if plugin_type is not None:
-            return self._plugins.get(plugin_type, [])  # type: ignore
+            return self._plugins.get(plugin_type, [])
         return [plugin for plugins in self._plugins.values() for plugin in plugins]
 
     def all_collector_plugins(self) -> List[Type[BaseCollectorPlugin]]:
         return cast(List[Type[BaseCollectorPlugin]], self.all_plugins(plugin_type=PluginType.COLLECTOR))
 
     def add_plugin_args(self, arg_parser: ArgumentParser) -> None:
         """Add args to the arg parser"""
```

### Comparing `resotoworker-3.6.0/resotoworker/resotocore.py` & `resotoworker-3.6.1/resotoworker/resotocore.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import requests
 import tempfile
 from datetime import datetime
 from resotolib.args import ArgumentParser
 from resotolib.logger import log
 from resotolib.jwt import encode_jwt_to_headers
-from resotolib.graph import Graph, GraphExportIterator
+from resotolib.graph import Graph, GraphExportIterator, export_model
 from resotolib.config import Config
 from resotolib.core import resotocore
 from typing import Callable, Optional
 from tenacity import Retrying
 from tenacity.stop import stop_after_attempt
 from tenacity.wait import wait_fixed
 
@@ -19,29 +19,30 @@
         self,
         send_request: Callable[[requests.Request], requests.Response],
         config: Config,
     ) -> None:
         self._send_request = send_request
         self._config = config
 
-    def send_to_resotocore(self, graph: Graph, task_id: str) -> None:
+    def create_graph_and_update_model(self, tempdir: str) -> None:
+        base_uri = resotocore.http_uri
+        resotocore_graph = self._config.resotoworker.graph
+        dump_json = self._config.resotoworker.debug_dump_json
+        self.create_graph(base_uri, resotocore_graph)
+        self.update_model(base_uri, dump_json=dump_json, tempdir=tempdir)
+
+    def send_to_resotocore(self, graph: Graph, task_id: str, tempdir: str) -> None:
         if not ArgumentParser.args.resotocore_uri:
             return None
 
-        log.info("resotocore Event Handler called")
-
         base_uri = resotocore.http_uri
         resotocore_graph = self._config.resotoworker.graph
         dump_json = self._config.resotoworker.debug_dump_json
-        tempdir = self._config.resotoworker.tempdir
         graph_merge_kind = self._config.resotoworker.graph_merge_kind
 
-        self.create_graph(base_uri, resotocore_graph)
-        self.update_model(graph, base_uri, dump_json=dump_json, tempdir=tempdir)
-
         graph_export_iterator = GraphExportIterator(
             graph,
             delete_tempfile=not dump_json,
             tempdir=tempdir,
             graph_merge_kind=graph_merge_kind,
         )
         #  The graph is not required any longer and can be released.
@@ -70,24 +71,23 @@
                 r = self._send_request(request)
                 if r.status_code != 200:
                     log.error(r.content)
                     raise RuntimeError(f"Failed to create graph: {r.content}")  # type: ignore
 
     def update_model(
         self,
-        graph: Graph,
         resotocore_base_uri: str,
         dump_json: bool = False,
         tempdir: Optional[str] = None,
     ) -> None:
         model_uri = f"{resotocore_base_uri}/model"
 
         log.debug(f"Updating model via {model_uri}")
 
-        model_json = json.dumps(graph.export_model(), indent=4)
+        model_json = json.dumps(export_model(), indent=4)
 
         if dump_json:
             ts = datetime.now().strftime("%Y-%m-%d-%H-%M")
             with tempfile.NamedTemporaryFile(
                 prefix=f"resoto-model-{ts}-",
                 suffix=".json",
                 delete=not dump_json,
@@ -121,19 +121,21 @@
 
         headers = {
             "Content-Type": "application/x-ndjson",
             "Resoto-Worker-Nodes": str(graph_export_iterator.number_of_nodes),
             "Resoto-Worker-Edges": str(graph_export_iterator.number_of_edges),
             "Resoto-Worker-Task-Id": task_id,
         }
+        params = dict(wait_for_result=False)
         if getattr(ArgumentParser.args, "psk", None):
             encode_jwt_to_headers(headers, {}, ArgumentParser.args.psk)
 
         for attempt in Retrying(reraise=True, stop=stop_after_attempt(3), wait=wait_fixed(10)):
             with attempt:
-                request = requests.Request(method="POST", url=merge_uri, data=graph_export_iterator, headers=headers)
+                request = requests.Request(
+                    method="POST", url=merge_uri, data=graph_export_iterator, params=params, headers=headers
+                )
                 r = self._send_request(request)
-                if r.status_code != 200:
+                if r.status_code not in (200, 204):
                     log.error(r.content)
                     raise RuntimeError(f"Failed to send graph: {r.content}")  # type: ignore
-                log.debug(f"resotocore reply: {r.content.decode()}")
         log.debug(f"Sent {graph_export_iterator.total_lines} items to resotocore")
```

### Comparing `resotoworker-3.6.0/resotoworker/tag.py` & `resotoworker-3.6.1/resotoworker/tag.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.6.0/resotoworker/utils.py` & `resotoworker-3.6.1/resotoworker/utils.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.6.0/resotoworker.egg-info/PKG-INFO` & `resotoworker-3.6.1/resotoworker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoworker
-Version: 3.6.0
+Version: 3.6.1
 Summary: Runs collector plugins and sends the result to resotocore.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotoworker
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `resotoworker-3.6.0/resotoworker.egg-info/SOURCES.txt` & `resotoworker-3.6.1/resotoworker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resotoworker-3.6.0/test/test_args.py` & `resotoworker-3.6.1/test/test_args.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.6.0/test/test_collect.py` & `resotoworker-3.6.1/test/test_resotocore.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
+import json
 from argparse import ArgumentParser
-from queue import Queue
-
-from resotoworker.collect import Collector
-from typing import Optional, cast
+from typing import Dict, cast
 from resotolib.graph import Graph
-from resotolib.config import Config
+from resotoworker.resotocore import Resotocore
+import requests
 from test.fakeconfig import FakeConfig
+from resotolib.config import Config
+from resotolib.baseresources import BaseAccount, GraphRoot
 from resotolib.baseplugin import BaseCollectorPlugin
-from resotolib.baseresources import BaseAccount
 from typing import ClassVar
 from attrs import define
 
 
 @define(eq=False)
 class ExampleAccount(BaseAccount):
     kind: ClassVar[str] = "example_account"
@@ -32,29 +32,44 @@
         pass
 
     @staticmethod
     def add_config(config: Config) -> None:
         pass
 
 
-def test_collect_and_send() -> None:
-    sent_task_id: Optional[str] = None
+def test_resotocore() -> None:
+    recorded_headers: Dict[str, str] = {}
 
-    def send_to_resotocore(graph: Graph, task_id: str) -> None:
-        nonlocal sent_task_id
-        sent_task_id = task_id
+    def make_query(request: requests.Request) -> requests.Response:
+        nonlocal recorded_headers
+        recorded_headers = request.headers
+        resp = requests.Response()
+        resp.status_code = 200
+        resp._content = str.encode(json.dumps("OK"))
+        return resp
 
     config = cast(
         Config,
         FakeConfig(
             values={
-                "resotoworker": {"pool_size": 1, "fork_process": False},
+                "resotoworker": {
+                    "graph": "resoto",
+                    "debug_dump_json": False,
+                    "tempdir": None,
+                    "graph_merge_kind": "foo_kind",
+                },
                 "running_config": None,
             }
         ),
     )
 
-    collector = Collector(config, send_to_resotocore, Queue())
+    core = Resotocore(make_query, config)
+
+    collector = ExampleCollectorPlugin()
+    collector.collect()
+    graph = Graph(root=GraphRoot(id="graph_root"))
+    graph.merge(collector.graph)
 
-    collector.collect_and_send([ExampleCollectorPlugin], [], "task_123", "collect")
+    core.send_to_resotocore(graph, "task_123", "/tmp")
+    print(recorded_headers)
 
-    assert sent_task_id == "task_123"
+    assert recorded_headers["Resoto-Worker-Task-Id"] == "task_123"
```

### Comparing `resotoworker-3.6.0/test/test_resotocore.py` & `resotoworker-3.6.1/test/test_collect.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,26 @@
-import json
+import requests
 from argparse import ArgumentParser
-from typing import Dict, cast
-from resotolib.graph import Graph
+from queue import Queue
+
+from resotoworker.collect import Collector
+from resotoworker.config import ResotoWorkerConfig
 from resotoworker.resotocore import Resotocore
-import requests
-from test.fakeconfig import FakeConfig
+from typing import Optional, cast, Any
+from resotolib.graph import Graph, GraphMergeKind
 from resotolib.config import Config
-from resotolib.baseresources import BaseAccount, GraphRoot
+from test.fakeconfig import FakeConfig
 from resotolib.baseplugin import BaseCollectorPlugin
+from resotolib.baseresources import BaseAccount
 from typing import ClassVar
 from attrs import define
 
+Config.add_config(ResotoWorkerConfig)
+Config.init_default_config()
+
 
 @define(eq=False)
 class ExampleAccount(BaseAccount):
     kind: ClassVar[str] = "example_account"
 
     def delete(self, graph: Graph) -> bool:
         return NotImplemented
@@ -32,44 +38,52 @@
         pass
 
     @staticmethod
     def add_config(config: Config) -> None:
         pass
 
 
-def test_resotocore() -> None:
-    recorded_headers: Dict[str, str] = {}
+def make_query(request: requests.Request) -> requests.Response:
+    resp = requests.Response()
+    resp.status_code = 200
+    resp._content = b""
+    return resp
+
+
+class TestResotocore(Resotocore):
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
+        super().__init__(*args, **kwargs)
+        self.sent_task_id: Optional[str] = None
 
-    def make_query(request: requests.Request) -> requests.Response:
-        nonlocal recorded_headers
-        recorded_headers = request.headers
-        resp = requests.Response()
-        resp.status_code = 200
-        resp._content = str.encode(json.dumps("OK"))
-        return resp
+    def send_to_resotocore(self, graph: Graph, task_id: str, tempdir: str) -> None:
+        self.sent_task_id = task_id
+
+    def create_graph_and_update_model(self, tempdir: str) -> None:
+        pass
+
+
+def test_collect_and_send() -> None:
+    resotocore = TestResotocore(make_query, Config)
 
     config = cast(
         Config,
         FakeConfig(
             values={
                 "resotoworker": {
-                    "graph": "resoto",
+                    "pool_size": 1,
+                    "fork_process": False,
                     "debug_dump_json": False,
-                    "tempdir": "/tmp",
-                    "graph_merge_kind": "foo_kind",
+                    "graph_merge_kind": GraphMergeKind.cloud,
+                    "graph_sender_pool_size": 5,
+                    "timeout": 10800,
+                    "tempdir": None,
                 },
                 "running_config": None,
             }
         ),
     )
 
-    core = Resotocore(make_query, config)
-
-    collector = ExampleCollectorPlugin()
-    collector.collect()
-    graph = Graph(root=GraphRoot(id="graph_root"))
-    graph.merge(collector.graph)
+    collector = Collector(config, resotocore, Queue())
 
-    core.send_to_resotocore(graph, "task_123")
-    print(recorded_headers)
+    collector.collect_and_send([ExampleCollectorPlugin], {"task": "task_123", "step": "collect"})
 
-    assert recorded_headers["Resoto-Worker-Task-Id"] == "task_123"
+    assert resotocore.sent_task_id == "task_123"
```

### Comparing `resotoworker-3.6.0/test/test_utils.py` & `resotoworker-3.6.1/test/test_utils.py`

 * *Files identical despite different names*

