# Comparing `tmp/langsmith-0.0.5.tar.gz` & `tmp/langsmith-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langsmith-0.0.5.tar", max compression
+gzip compressed data, was "langsmith-0.0.6.tar", max compression
```

## Comparing `langsmith-0.0.5.tar` & `langsmith-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     8031 2023-07-12 19:21:57.969036 langsmith-0.0.5/README.md
--rw-r--r--   0        0        0      478 2023-07-12 19:21:57.969036 langsmith-0.0.5/langsmith/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 19:21:57.969036 langsmith-0.0.5/langsmith/cli/__init__.py
--rw-r--r--   0        0        0      363 2023-07-12 19:21:57.969036 langsmith-0.0.5/langsmith/cli/conf/nginx.conf
--rw-r--r--   0        0        0      143 2023-07-12 19:21:57.969036 langsmith-0.0.5/langsmith/cli/docker-compose.dev.yaml
--rw-r--r--   0        0        0      315 2023-07-12 19:21:57.969036 langsmith-0.0.5/langsmith/cli/docker-compose.ngrok.yaml
--rw-r--r--   0        0        0     1186 2023-07-12 19:21:57.969036 langsmith-0.0.5/langsmith/cli/docker-compose.yaml
--rw-r--r--   0        0        0    14432 2023-07-12 19:21:57.969036 langsmith-0.0.5/langsmith/cli/main.py
--rw-r--r--   0        0        0    30429 2023-07-12 19:21:57.969036 langsmith-0.0.5/langsmith/client.py
--rw-r--r--   0        0        0      234 2023-07-12 19:21:57.969036 langsmith-0.0.5/langsmith/evaluation/__init__.py
--rw-r--r--   0        0        0     1411 2023-07-12 19:21:57.969036 langsmith-0.0.5/langsmith/evaluation/evaluator.py
--rw-r--r--   0        0        0     1529 2023-07-12 19:21:57.969036 langsmith-0.0.5/langsmith/evaluation/string_evaluator.py
--rw-r--r--   0        0        0     9462 2023-07-12 19:21:57.969036 langsmith-0.0.5/langsmith/run_helpers.py
--rw-r--r--   0        0        0     6116 2023-07-12 19:21:57.969036 langsmith-0.0.5/langsmith/run_trees.py
--rw-r--r--   0        0        0     6499 2023-07-12 19:21:57.969036 langsmith-0.0.5/langsmith/schemas.py
--rw-r--r--   0        0        0     2185 2023-07-12 19:21:57.969036 langsmith-0.0.5/langsmith/utils.py
--rw-r--r--   0        0        0      858 2023-07-12 19:21:57.969036 langsmith-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     8593 1970-01-01 00:00:00.000000 langsmith-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     8031 2023-07-14 06:11:43.024263 langsmith-0.0.6/README.md
+-rw-r--r--   0        0        0      478 2023-07-14 06:11:43.024263 langsmith-0.0.6/langsmith/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-14 06:11:43.024263 langsmith-0.0.6/langsmith/cli/__init__.py
+-rw-r--r--   0        0        0      363 2023-07-14 06:11:43.024263 langsmith-0.0.6/langsmith/cli/conf/nginx.conf
+-rw-r--r--   0        0        0      143 2023-07-14 06:11:43.024263 langsmith-0.0.6/langsmith/cli/docker-compose.dev.yaml
+-rw-r--r--   0        0        0      315 2023-07-14 06:11:43.024263 langsmith-0.0.6/langsmith/cli/docker-compose.ngrok.yaml
+-rw-r--r--   0        0        0     1186 2023-07-14 06:11:43.024263 langsmith-0.0.6/langsmith/cli/docker-compose.yaml
+-rw-r--r--   0        0        0    14283 2023-07-14 06:11:43.024263 langsmith-0.0.6/langsmith/cli/main.py
+-rw-r--r--   0        0        0    31862 2023-07-14 06:11:43.024263 langsmith-0.0.6/langsmith/client.py
+-rw-r--r--   0        0        0      234 2023-07-14 06:11:43.024263 langsmith-0.0.6/langsmith/evaluation/__init__.py
+-rw-r--r--   0        0        0     1411 2023-07-14 06:11:43.024263 langsmith-0.0.6/langsmith/evaluation/evaluator.py
+-rw-r--r--   0        0        0     1529 2023-07-14 06:11:43.024263 langsmith-0.0.6/langsmith/evaluation/string_evaluator.py
+-rw-r--r--   0        0        0     9462 2023-07-14 06:11:43.024263 langsmith-0.0.6/langsmith/run_helpers.py
+-rw-r--r--   0        0        0     6116 2023-07-14 06:11:43.024263 langsmith-0.0.6/langsmith/run_trees.py
+-rw-r--r--   0        0        0     6499 2023-07-14 06:11:43.024263 langsmith-0.0.6/langsmith/schemas.py
+-rw-r--r--   0        0        0     4180 2023-07-14 06:11:43.024263 langsmith-0.0.6/langsmith/utils.py
+-rw-r--r--   0        0        0      858 2023-07-14 06:11:43.024263 langsmith-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     8593 1970-01-01 00:00:00.000000 langsmith-0.0.6/PKG-INFO
```

### Comparing `langsmith-0.0.5/README.md` & `langsmith-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.5/langsmith/cli/docker-compose.yaml` & `langsmith-0.0.6/langsmith/cli/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.5/langsmith/cli/main.py` & `langsmith-0.0.6/langsmith/cli/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,20 +2,23 @@
 import json
 import logging
 import os
 import shutil
 import subprocess
 from contextlib import contextmanager
 from pathlib import Path
-from subprocess import CalledProcessError
 from typing import Dict, Generator, List, Mapping, Optional, Union, cast
 
 import requests
 
-from langsmith.utils import get_runtime_environment
+from langsmith.utils import (
+    get_docker_compose_command,
+    get_docker_environment,
+    get_runtime_environment,
+)
 
 logging.basicConfig(level=logging.INFO, format="%(message)s")
 logger = logging.getLogger(__name__)
 
 _DIR = Path(__file__).parent
 
 
@@ -59,40 +62,14 @@
         " in your LangChain application:"
         "\nLANGCHAIN_TRACING_V2=true"
         f"\nLANGCHAIN_ENDPOINT={langchain_endpoint}"
     )
     logger.info("\n".join(service_message))
 
 
-def get_docker_compose_command() -> List[str]:
-    """Get the correct docker compose command for this system."""
-    try:
-        subprocess.check_call(
-            ["docker", "compose", "--version"],
-            stdout=subprocess.DEVNULL,
-            stderr=subprocess.DEVNULL,
-        )
-        return ["docker", "compose"]
-    except (CalledProcessError, FileNotFoundError):
-        try:
-            subprocess.check_call(
-                ["docker-compose", "--version"],
-                stdout=subprocess.DEVNULL,
-                stderr=subprocess.DEVNULL,
-            )
-            return ["docker-compose"]
-        except (CalledProcessError, FileNotFoundError):
-            raise ValueError(
-                "Neither 'docker compose' nor 'docker-compose'"
-                " commands are available. Please install the Docker"
-                " server following the instructions for your operating"
-                " system at https://docs.docker.com/engine/install/"
-            )
-
-
 def get_ngrok_url(auth_token: Optional[str]) -> str:
     """Get the ngrok URL for the LangSmith server."""
     ngrok_url = "http://localhost:4040/api/tunnels"
     try:
         response = requests.get(ngrok_url)
         response.raise_for_status()
         exposed_url = response.json()["tunnels"][0]["public_url"]
@@ -156,23 +133,26 @@
     config_path.unlink(missing_ok=True)
 
 
 class LangSmithCommand:
     """Manage the LangSmith Tracing server."""
 
     def __init__(self) -> None:
-        self.docker_compose_command = get_docker_compose_command()
         self.docker_compose_file = (
             Path(__file__).absolute().parent / "docker-compose.yaml"
         )
         self.docker_compose_dev_file = (
             Path(__file__).absolute().parent / "docker-compose.dev.yaml"
         )
         self.ngrok_path = Path(__file__).absolute().parent / "docker-compose.ngrok.yaml"
 
+    @property
+    def docker_compose_command(self) -> List[str]:
+        return get_docker_compose_command()
+
     def _open_browser(self, url: str) -> None:
         try:
             subprocess.run(["open", url])
         except FileNotFoundError:
             pass
 
     def _start_local(self, dev: bool) -> None:
@@ -282,26 +262,36 @@
             os.environ["OPENAI_API_KEY"] = openai_api_key
         self.pull(dev=dev)
         if expose:
             self._start_and_expose(auth_token=auth_token, dev=dev)
         else:
             self._start_local(dev=dev)
 
-    def stop(self) -> None:
+    def stop(self, clear_volumes: bool = False) -> None:
         """Stop the LangSmith server."""
-        subprocess.run(
-            [
-                *self.docker_compose_command,
-                "-f",
-                str(self.docker_compose_file),
-                "-f",
-                str(self.ngrok_path),
-                "down",
-            ]
-        )
+        cmd = [
+            *self.docker_compose_command,
+            "-f",
+            str(self.docker_compose_file),
+            "-f",
+            str(self.ngrok_path),
+            "down",
+        ]
+        if clear_volumes:
+            confirm = input(
+                "You are about to delete all the locally cached "
+                "LangSmith containers and volumes. "
+                "This operation cannot be undone. Are you sure? [y/N]"
+            )
+            if confirm.lower() != "y":
+                print("Aborting.")
+                return
+            cmd.append("--volumes")
+
+        subprocess.run(cmd)
 
     def logs(self) -> None:
         """Print the logs from the LangSmith server."""
         subprocess.run(
             [
                 *self.docker_compose_command,
                 "-f",
@@ -342,16 +332,22 @@
             logger.info("The LangSmith server is not running.")
             return
 
 
 def env() -> None:
     """Print the runtime environment information."""
     env = get_runtime_environment()
+    env.update(get_docker_environment())
+
+    # calculate the max length of keys
+    max_key_length = max(len(key) for key in env.keys())
+
     logger.info("LangChain Environment:")
-    logger.info("\n".join(f"{k}:{v}" for k, v in env.items()))
+    for k, v in env.items():
+        logger.info(f"{k:{max_key_length}}: {v}")
 
 
 def main() -> None:
     """Main entrypoint for the CLI."""
     parser = argparse.ArgumentParser()
     subparsers = parser.add_subparsers(description="LangSmith CLI commands")
 
@@ -391,15 +387,22 @@
             openai_api_key=args.openai_api_key,
         )
     )
 
     server_stop_parser = subparsers.add_parser(
         "stop", description="Stop the LangSmith server."
     )
-    server_stop_parser.set_defaults(func=lambda args: server_command.stop())
+    server_stop_parser.add_argument(
+        "--clear-volumes",
+        action="store_true",
+        help="Delete all the locally cached LangSmith containers and volumes.",
+    )
+    server_stop_parser.set_defaults(
+        func=lambda args: server_command.stop(clear_volumes=args.clear_volumes)
+    )
 
     server_pull_parser = subparsers.add_parser(
         "pull", description="Pull the latest LangSmith images."
     )
     server_pull_parser.add_argument(
         "--dev",
         action="store_true",
```

### Comparing `langsmith-0.0.5/langsmith/client.py` & `langsmith-0.0.6/langsmith/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -348,15 +348,15 @@
         )
         run_create = {
             **kwargs,
             "session_name": project_name,
             "name": name,
             "inputs": inputs,
             "run_type": run_type,
-            "execution_order": execution_order,
+            "execution_order": execution_order if execution_order is not None else 1,
         }
         run_extra = cast(dict, run_create.setdefault("extra", {}))
         runtime = run_extra.setdefault("runtime", {})
         runtime_env = get_runtime_environment()
         run_extra["runtime"] = {**runtime_env, **runtime}
         headers = {**self._headers, "Accept": "application/json"}
         self.request_with_retries(
@@ -421,34 +421,67 @@
         *,
         project_id: Optional[ID_TYPE] = None,
         project_name: Optional[str] = None,
         run_type: Optional[str] = None,
         dataset_name: Optional[str] = None,
         dataset_id: Optional[ID_TYPE] = None,
         reference_example_id: Optional[ID_TYPE] = None,
+        query: Optional[str] = None,
+        filter: Optional[str] = None,
+        execution_order: Optional[int] = None,
+        parent_run_id: Optional[ID_TYPE] = None,
+        start_time: Optional[datetime] = None,
+        end_time: Optional[datetime] = None,
+        error: Optional[bool] = None,
+        run_ids: Optional[List[ID_TYPE]] = None,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
+        order_by: Optional[Sequence[str]] = None,
         **kwargs: Any,
     ) -> Iterator[Run]:
         """List runs from the LangSmith API."""
         if project_name is not None:
             if project_id is not None:
                 raise ValueError("Only one of project_id or project_name may be given")
             project_id = self.read_project(project_name=project_name).id
         if dataset_name is not None:
             if dataset_id is not None:
                 raise ValueError("Only one of dataset_id or dataset_name may be given")
             dataset_id = self.read_dataset(dataset_name=dataset_name).id
-        query_params = {
+        query_params: Dict[str, Any] = {
             "session": project_id,
             "run_type": run_type,
             **kwargs,
         }
         if reference_example_id is not None:
             query_params["reference_example"] = reference_example_id
         if dataset_id is not None:
             query_params["dataset"] = dataset_id
+        if query is not None:
+            query_params["query"] = query
+        if filter is not None:
+            query_params["filter"] = filter
+        if execution_order is not None:
+            query_params["execution_order"] = execution_order
+        if parent_run_id is not None:
+            query_params["parent_run"] = parent_run_id
+        if start_time is not None:
+            query_params["start_time"] = start_time.isoformat()
+        if end_time is not None:
+            query_params["end_time"] = end_time.isoformat()
+        if error is not None:
+            query_params["error"] = error
+        if run_ids is not None:
+            query_params["id"] = run_ids
+        if limit is not None:
+            query_params["limit"] = limit
+        if offset is not None:
+            query_params["offset"] = offset
+        if order_by is not None:
+            query_params["order"] = order_by
         yield from (
             Run(**run) for run in self._get_paginated_list("/runs", params=query_params)
         )
 
     def delete_run(self, run_id: ID_TYPE) -> None:
         """Delete a run from the LangSmith API."""
         response = self.session.delete(
```

### Comparing `langsmith-0.0.5/langsmith/evaluation/evaluator.py` & `langsmith-0.0.6/langsmith/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.5/langsmith/evaluation/string_evaluator.py` & `langsmith-0.0.6/langsmith/evaluation/string_evaluator.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.5/langsmith/run_helpers.py` & `langsmith-0.0.6/langsmith/run_helpers.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.5/langsmith/run_trees.py` & `langsmith-0.0.6/langsmith/run_trees.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.5/langsmith/schemas.py` & `langsmith-0.0.6/langsmith/schemas.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.5/pyproject.toml` & `langsmith-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langsmith"
-version = "0.0.5"
+version = "0.0.6"
 description = "Client library to connect to the LangSmith LLM Tracing and Evaluation Platform."
 authors = ["LangChain"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "langsmith"}]
 
 [tool.poetry.scripts]
```

### Comparing `langsmith-0.0.5/PKG-INFO` & `langsmith-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langsmith
-Version: 0.0.5
+Version: 0.0.6
 Summary: Client library to connect to the LangSmith LLM Tracing and Evaluation Platform.
 License: MIT
 Author: LangChain
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

