# Comparing `tmp/integrate-ai-9.5.0.tar.gz` & `tmp/integrate-ai-9.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "integrate-ai-9.5.0.tar", last modified: Wed May 17 20:51:48 2023, max compression
+gzip compressed data, was "integrate-ai-9.6.0.tar", last modified: Fri Jul 14 18:09:16 2023, max compression
```

## Comparing `integrate-ai-9.5.0.tar` & `integrate-ai-9.6.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 20:51:48.924935 integrate-ai-9.5.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-05-17 20:51:47.000000 integrate-ai-9.5.0/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1075 2023-05-17 20:51:48.924935 integrate-ai-9.5.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      750 2023-05-17 20:51:47.000000 integrate-ai-9.5.0/backend_shim.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 20:51:48.920935 integrate-ai-9.5.0/integrate_ai/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-17 20:51:47.000000 integrate-ai-9.5.0/integrate_ai/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      657 2023-05-17 20:51:47.000000 integrate-ai-9.5.0/integrate_ai/cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20910 2023-05-17 20:51:47.000000 integrate-ai-9.5.0/integrate_ai/client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1081 2023-05-17 20:51:47.000000 integrate-ai-9.5.0/integrate_ai/main.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2692 2023-05-17 20:51:47.000000 integrate-ai-9.5.0/integrate_ai/sdk.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5678 2023-05-17 20:51:47.000000 integrate-ai-9.5.0/integrate_ai/server.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 20:51:48.924935 integrate-ai-9.5.0/integrate_ai/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-17 20:51:47.000000 integrate-ai-9.5.0/integrate_ai/utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8291 2023-05-17 20:51:47.000000 integrate-ai-9.5.0/integrate_ai/utils/docker_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1105 2023-05-17 20:51:47.000000 integrate-ai-9.5.0/integrate_ai/utils/error_handling.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      664 2023-05-17 20:51:47.000000 integrate-ai-9.5.0/integrate_ai/utils/logger.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      859 2023-05-17 20:51:47.000000 integrate-ai-9.5.0/integrate_ai/utils/path_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6025 2023-05-17 20:51:47.000000 integrate-ai-9.5.0/integrate_ai/utils/rest_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2840 2023-05-17 20:51:47.000000 integrate-ai-9.5.0/integrate_ai/utils/typer_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-17 20:51:48.924935 integrate-ai-9.5.0/integrate_ai.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1075 2023-05-17 20:51:48.000000 integrate-ai-9.5.0/integrate_ai.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      665 2023-05-17 20:51:48.000000 integrate-ai-9.5.0/integrate_ai.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-17 20:51:48.000000 integrate-ai-9.5.0/integrate_ai.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       46 2023-05-17 20:51:48.000000 integrate-ai-9.5.0/integrate_ai.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-17 20:51:48.000000 integrate-ai-9.5.0/integrate_ai.egg-info/namespace_packages.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2023-05-17 20:51:48.000000 integrate-ai-9.5.0/integrate_ai.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-17 20:51:48.000000 integrate-ai-9.5.0/integrate_ai.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-17 20:51:48.924935 integrate-ai-9.5.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1753 2023-05-17 20:51:47.000000 integrate-ai-9.5.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 18:09:16.485332 integrate-ai-9.6.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-07-14 18:09:15.000000 integrate-ai-9.6.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1075 2023-07-14 18:09:16.485332 integrate-ai-9.6.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      750 2023-07-14 18:09:15.000000 integrate-ai-9.6.0/backend_shim.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 18:09:16.481331 integrate-ai-9.6.0/integrate_ai/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 18:09:15.000000 integrate-ai-9.6.0/integrate_ai/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      657 2023-07-14 18:09:15.000000 integrate-ai-9.6.0/integrate_ai/cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21146 2023-07-14 18:09:15.000000 integrate-ai-9.6.0/integrate_ai/client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1081 2023-07-14 18:09:15.000000 integrate-ai-9.6.0/integrate_ai/main.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2692 2023-07-14 18:09:15.000000 integrate-ai-9.6.0/integrate_ai/sdk.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5678 2023-07-14 18:09:15.000000 integrate-ai-9.6.0/integrate_ai/server.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 18:09:16.485332 integrate-ai-9.6.0/integrate_ai/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-14 18:09:15.000000 integrate-ai-9.6.0/integrate_ai/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8291 2023-07-14 18:09:15.000000 integrate-ai-9.6.0/integrate_ai/utils/docker_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1105 2023-07-14 18:09:15.000000 integrate-ai-9.6.0/integrate_ai/utils/error_handling.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      664 2023-07-14 18:09:15.000000 integrate-ai-9.6.0/integrate_ai/utils/logger.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      859 2023-07-14 18:09:15.000000 integrate-ai-9.6.0/integrate_ai/utils/path_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6025 2023-07-14 18:09:15.000000 integrate-ai-9.6.0/integrate_ai/utils/rest_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2840 2023-07-14 18:09:15.000000 integrate-ai-9.6.0/integrate_ai/utils/typer_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-14 18:09:16.485332 integrate-ai-9.6.0/integrate_ai.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1075 2023-07-14 18:09:16.000000 integrate-ai-9.6.0/integrate_ai.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      665 2023-07-14 18:09:16.000000 integrate-ai-9.6.0/integrate_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-14 18:09:16.000000 integrate-ai-9.6.0/integrate_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       46 2023-07-14 18:09:16.000000 integrate-ai-9.6.0/integrate_ai.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-14 18:09:16.000000 integrate-ai-9.6.0/integrate_ai.egg-info/namespace_packages.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2023-07-14 18:09:16.000000 integrate-ai-9.6.0/integrate_ai.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-07-14 18:09:16.000000 integrate-ai-9.6.0/integrate_ai.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-07-14 18:09:16.485332 integrate-ai-9.6.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1748 2023-07-14 18:09:15.000000 integrate-ai-9.6.0/setup.py
```

### Comparing `integrate-ai-9.5.0/PKG-INFO` & `integrate-ai-9.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: integrate-ai
-Version: 9.5.0
+Version: 9.6.0
 Summary: integrate.ai
 Author: integrate.ai
 License: Copyright (C) 2022 integrate.ai, Inc. All rights reserved.
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7.5
 Description-Content-Type: text/markdown
```

### Comparing `integrate-ai-9.5.0/backend_shim.py` & `integrate-ai-9.6.0/backend_shim.py`

 * *Files identical despite different names*

### Comparing `integrate-ai-9.5.0/integrate_ai/cli.py` & `integrate-ai-9.6.0/integrate_ai/cli.py`

 * *Files identical despite different names*

### Comparing `integrate-ai-9.5.0/integrate_ai/client.py` & `integrate-ai-9.6.0/integrate_ai/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -421,15 +421,15 @@
                     "environment": {"IAI_LOG_SAVE_PATH": container_log_path},
                     "extra_hosts": {"localhost": "host-gateway"},
                 },
             )
             assert response
         except Exception as e:
             progress.console.print(e, style="red")
-            raise typer.Exit(0)
+            raise typer.Exit(1)
 
         progress.update(task_id=start_container_task, completed=True)
         progress.console.print(f"Container {container_name} is started.", style="green")
     return mounted_data_path, local_log_path
 
 
 def mount_data_for_train(mount_path, volumes, **kwargs):
@@ -514,41 +514,44 @@
         verbose: Log verbose for container
 
     """
     set_env_var(environment, "IAI_DEBUG_LOCAL_GATEWAY")
     set_env_var(environment, "IAI_FLOUR_LOG_LEVEL")
     with Progress(SpinnerColumn(), TextColumn("[progress.description]{task.description}")) as progress:
         task = progress.add_task(description="Processing...", total=1)
-        response = container.exec_run(
-            cmd,
-            stdout=verbose,
+        exec_id = container.client.api.exec_create(container.id, cmd, stdout=verbose, environment=environment)
+        response = container.client.api.exec_start(
+            exec_id,
             stream=True,
             demux=True,
-            environment=environment,
         )
         if response:
-            for (output, error) in response.output:  # type: ignore
+            for (output, error) in response:  # type: ignore
                 if error:
                     progress.console.print(error.decode("utf-8"))
                 else:
                     progress.console.print(output.decode("utf-8"))
 
         progress.update(task_id=task, completed=True)
 
-    progress.console.print("Finished processing.", style="green")
+    exec_result = container.client.api.exec_inspect(exec_id)
+    exit_code = exec_result["ExitCode"]
+    progress.console.print(
+        f"Finished processing with exit code {exit_code}.", style="green" if exit_code == 0 else "red"
+    )
     progress.console.print("Logs are saved in {local_log_path} and can be found with iai client log", style="blue")
 
     with Progress(SpinnerColumn(), TextColumn("[progress.description]{task.description}")) as progress:
         closing_task = progress.add_task(description="Closing container...", total=1)
         container.stop()
         if remove_after_complete:
             container.remove()
         progress.update(task_id=closing_task, completed=True)
 
-        raise typer.Exit(0)
+        raise typer.Exit(exit_code)
 
 
 @app.callback()
 def main():
     """
     Sub command for managing client related operations.
     """
```

### Comparing `integrate-ai-9.5.0/integrate_ai/main.py` & `integrate-ai-9.6.0/integrate_ai/main.py`

 * *Files identical despite different names*

### Comparing `integrate-ai-9.5.0/integrate_ai/sdk.py` & `integrate-ai-9.6.0/integrate_ai/sdk.py`

 * *Files identical despite different names*

### Comparing `integrate-ai-9.5.0/integrate_ai/server.py` & `integrate-ai-9.6.0/integrate_ai/server.py`

 * *Files identical despite different names*

### Comparing `integrate-ai-9.5.0/integrate_ai/utils/docker_client.py` & `integrate-ai-9.6.0/integrate_ai/utils/docker_client.py`

 * *Files identical despite different names*

### Comparing `integrate-ai-9.5.0/integrate_ai/utils/error_handling.py` & `integrate-ai-9.6.0/integrate_ai/utils/error_handling.py`

 * *Files identical despite different names*

### Comparing `integrate-ai-9.5.0/integrate_ai/utils/logger.py` & `integrate-ai-9.6.0/integrate_ai/utils/logger.py`

 * *Files identical despite different names*

### Comparing `integrate-ai-9.5.0/integrate_ai/utils/path_utils.py` & `integrate-ai-9.6.0/integrate_ai/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `integrate-ai-9.5.0/integrate_ai/utils/rest_client.py` & `integrate-ai-9.6.0/integrate_ai/utils/rest_client.py`

 * *Files identical despite different names*

### Comparing `integrate-ai-9.5.0/integrate_ai/utils/typer_utils.py` & `integrate-ai-9.6.0/integrate_ai/utils/typer_utils.py`

 * *Files identical despite different names*

### Comparing `integrate-ai-9.5.0/integrate_ai.egg-info/PKG-INFO` & `integrate-ai-9.6.0/integrate_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: integrate-ai
-Version: 9.5.0
+Version: 9.6.0
 Summary: integrate.ai
 Author: integrate.ai
 License: Copyright (C) 2022 integrate.ai, Inc. All rights reserved.
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7.5
 Description-Content-Type: text/markdown
```

### Comparing `integrate-ai-9.5.0/integrate_ai.egg-info/SOURCES.txt` & `integrate-ai-9.6.0/integrate_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `integrate-ai-9.5.0/setup.py` & `integrate-ai-9.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,10 +66,9 @@
     'package_data': {
     },
     'packages': (
         'integrate_ai',
         'integrate_ai.utils',
     ),
     'python_requires': '>=3.7.5',
-    'version': """9.5.0
-""",
+    'version': '9.6.0',
 })
```

