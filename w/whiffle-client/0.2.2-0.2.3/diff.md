# Comparing `tmp/whiffle_client-0.2.2.tar.gz` & `tmp/whiffle_client-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/builds/whiffle/hindcasting/whiffle-client/dist/.tmp-r_roxn_j/whiffle_client-0.2.2.tar", last modified: Thu Jul 13 16:52:54 2023, max compression
+gzip compressed data, was "/builds/whiffle/hindcasting/whiffle-client/dist/.tmp-nptz5x6_/whiffle_client-0.2.3.tar", last modified: Fri Jul 14 10:23:48 2023, max compression
```

## Comparing `whiffle_client-0.2.2.tar` & `whiffle_client-0.2.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 16:52:54.000000 whiffle_client-0.2.2/
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-07-13 16:52:48.000000 whiffle_client-0.2.2/LICENCE.txt
--rw-rw-rw-   0 root         (0) root         (0)      121 2023-07-13 16:52:48.000000 whiffle_client-0.2.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1567 2023-07-13 16:52:54.000000 whiffle_client-0.2.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      780 2023-07-13 16:52:48.000000 whiffle_client-0.2.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1228 2023-07-13 16:52:48.000000 whiffle_client-0.2.2/USER_README.md
--rw-rw-rw-   0 root         (0) root         (0)      834 2023-07-13 16:52:48.000000 whiffle_client-0.2.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 16:52:54.000000 whiffle_client-0.2.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 16:52:54.000000 whiffle_client-0.2.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3935 2023-07-13 16:52:48.000000 whiffle_client-0.2.2/tests/test_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 16:52:54.000000 whiffle_client-0.2.2/whiffle_client/
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-07-13 16:52:48.000000 whiffle_client-0.2.2/whiffle_client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7093 2023-07-13 16:52:48.000000 whiffle_client-0.2.2/whiffle_client/client.py
--rw-rw-rw-   0 root         (0) root         (0)     3092 2023-07-13 16:52:48.000000 whiffle_client-0.2.2/whiffle_client/entrypoints.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 16:52:54.000000 whiffle_client-0.2.2/whiffle_client/resources/
--rw-rw-rw-   0 root         (0) root         (0)     2624 2023-07-13 16:52:48.000000 whiffle_client-0.2.2/whiffle_client/resources/example_generic_params.json
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-07-13 16:52:48.000000 whiffle_client-0.2.2/whiffle_client/resources/whiffle_config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 16:52:54.000000 whiffle_client-0.2.2/whiffle_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1567 2023-07-13 16:52:54.000000 whiffle_client-0.2.2/whiffle_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      494 2023-07-13 16:52:54.000000 whiffle_client-0.2.2/whiffle_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 16:52:54.000000 whiffle_client-0.2.2/whiffle_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-07-13 16:52:54.000000 whiffle_client-0.2.2/whiffle_client.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-07-13 16:52:54.000000 whiffle_client-0.2.2/whiffle_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-13 16:52:54.000000 whiffle_client-0.2.2/whiffle_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:23:48.000000 whiffle_client-0.2.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-07-14 10:23:42.000000 whiffle_client-0.2.3/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)      121 2023-07-14 10:23:42.000000 whiffle_client-0.2.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1577 2023-07-14 10:23:48.000000 whiffle_client-0.2.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      780 2023-07-14 10:23:42.000000 whiffle_client-0.2.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1238 2023-07-14 10:23:42.000000 whiffle_client-0.2.3/USER_README.md
+-rw-rw-rw-   0 root         (0) root         (0)      834 2023-07-14 10:23:42.000000 whiffle_client-0.2.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 10:23:48.000000 whiffle_client-0.2.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:23:48.000000 whiffle_client-0.2.3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3943 2023-07-14 10:23:42.000000 whiffle_client-0.2.3/tests/test_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:23:48.000000 whiffle_client-0.2.3/whiffle_client/
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-07-14 10:23:42.000000 whiffle_client-0.2.3/whiffle_client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7093 2023-07-14 10:23:42.000000 whiffle_client-0.2.3/whiffle_client/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     3088 2023-07-14 10:23:42.000000 whiffle_client-0.2.3/whiffle_client/entrypoints.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:23:48.000000 whiffle_client-0.2.3/whiffle_client/resources/
+-rw-rw-rw-   0 root         (0) root         (0)     2624 2023-07-14 10:23:42.000000 whiffle_client-0.2.3/whiffle_client/resources/example_generic_params.json
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-07-14 10:23:42.000000 whiffle_client-0.2.3/whiffle_client/resources/whiffle_config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:23:48.000000 whiffle_client-0.2.3/whiffle_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1577 2023-07-14 10:23:48.000000 whiffle_client-0.2.3/whiffle_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      494 2023-07-14 10:23:48.000000 whiffle_client-0.2.3/whiffle_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 10:23:48.000000 whiffle_client-0.2.3/whiffle_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-07-14 10:23:48.000000 whiffle_client-0.2.3/whiffle_client.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-07-14 10:23:48.000000 whiffle_client-0.2.3/whiffle_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-14 10:23:48.000000 whiffle_client-0.2.3/whiffle_client.egg-info/top_level.txt
```

### Comparing `whiffle_client-0.2.2/LICENCE.txt` & `whiffle_client-0.2.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.2.2/PKG-INFO` & `whiffle_client-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: whiffle_client
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python based web client to interact with Whiffle services
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 # Whiffle client
 
 This client allows running atmospheric large-eddy simulations (LES) with Whiffle's GPU-resident model <https://whiffle.nl/>. 
 The client requires an access token, which you can configure with the command line interface by executing,
 
-`whiffle config-edit user.token <your_token>`
+`whiffle config edit user.token <your_token>`
 
 You can create a new task by executing,
 
-`whiffle run <path_to_the_task_specification.[json|yaml]>`
+`whiffle task run <path_to_the_task_specification.[json|yaml]>`
 
 The client polls the progress of the task until it has finished. The task will run in the background if you abort the client.
 You can list the most recent tasks by executing,
 
 `whiffle task list`
 
 If you need an access token or you have any questions, please reach out to <support@whiffle.nl>.
@@ -30,19 +30,19 @@
 
 ### List the configuration
 
 `whiffle config list`
 
 ### Change the token in the configuration
 
-`whiffle config-edit user.token <your_token>`
+`whiffle config edit user.token <your_token>`
 
 ### Run a task
 
-`whiffle run <path_to_the_task_specification.[json|yaml]>`
+`whiffle task run <path_to_the_task_specification.[json|yaml]>`
 
 ### List tasks
 
 `whiffle task list <number of tasks>`
 
 ### Download a task
```

### Comparing `whiffle_client-0.2.2/README.md` & `whiffle_client-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.2.2/USER_README.md` & `whiffle_client-0.2.3/whiffle_client.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,27 @@
+Metadata-Version: 2.1
+Name: whiffle-client
+Version: 0.2.3
+Summary: Python based web client to interact with Whiffle services
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENCE.txt
+
 # Whiffle client
 
 This client allows running atmospheric large-eddy simulations (LES) with Whiffle's GPU-resident model <https://whiffle.nl/>. 
 The client requires an access token, which you can configure with the command line interface by executing,
 
-`whiffle config-edit user.token <your_token>`
+`whiffle config edit user.token <your_token>`
 
 You can create a new task by executing,
 
-`whiffle run <path_to_the_task_specification.[json|yaml]>`
+`whiffle task run <path_to_the_task_specification.[json|yaml]>`
 
 The client polls the progress of the task until it has finished. The task will run in the background if you abort the client.
 You can list the most recent tasks by executing,
 
 `whiffle task list`
 
 If you need an access token or you have any questions, please reach out to <support@whiffle.nl>.
@@ -20,26 +30,26 @@
 
 ### List the configuration
 
 `whiffle config list`
 
 ### Change the token in the configuration
 
-`whiffle config-edit user.token <your_token>`
+`whiffle config edit user.token <your_token>`
 
 ### Run a task
 
-`whiffle run <path_to_the_task_specification.[json|yaml]>`
+`whiffle task run <path_to_the_task_specification.[json|yaml]>`
 
 ### List tasks
 
 `whiffle task list <number of tasks>`
 
 ### Download a task
 
 `whiffle task download <task_id>`
 
 ### Attach a task
 
 You can monitor the progress of a task and it will be automatically downloaded once the task has been successfully completed. 
 
-`whiffle task attach <task_id>`
+`whiffle task attach <task_id>`
```

### Comparing `whiffle_client-0.2.2/pyproject.toml` & `whiffle_client-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.2.2/tests/test_client.py` & `whiffle_client-0.2.3/tests/test_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         assert token in res.output
         res = runner.invoke(whiffle, ["config", "list"])
         assert token in res.output
 
     def test_run_task(self, mocker):
         mock_new_task_response(mocker)
         mock = mocker.patch("whiffle_client.Client.process")
-        runner.invoke(whiffle, ["run", default_task_path])
+        runner.invoke(whiffle, ["task", "run", default_task_path])
         mock.assert_called_once()
 
     def test_task_list(self, mocker):
         mock_new_task_response(mocker)
         mock = mocker.patch("whiffle_client.Client.get_tasks")
         runner.invoke(whiffle, ["task", "list"])
         mock.assert_called_once()
```

### Comparing `whiffle_client-0.2.2/whiffle_client/client.py` & `whiffle_client-0.2.3/whiffle_client/client.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.2.2/whiffle_client/entrypoints.py` & `whiffle_client-0.2.3/whiffle_client/entrypoints.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 @click.group()
 def whiffle():
     pass
 
 
 @whiffle.group()
 def task():
-    """task commands"""
+    """Task commands"""
     pass
 
 
 @whiffle.group()
 def config():
-    """edit config"""
+    """Edit config"""
     pass
 
 
 @task.command()
 @click.argument("number_of_tasks", default=10)
 def list(number_of_tasks):
-    """List tasks."""
+    """List tasks"""
 
     number_of_tasks = int(number_of_tasks)
     client = Client()
     tasks = client.get_tasks()
     click.echo(
         "{:33}{:11}{:16} {:16} progress".format(
             "task id", "status", "start time", "finish time"
@@ -41,15 +41,15 @@
         click.echo(
             "{task_id:33}{task_status:11}{received:17.16}{finished:17.16}{processed_steps}/{total_steps}".format(
                 **task
             )
         )
 
 
-@whiffle.command()
+@task.command()
 @click.argument("file_path")
 def run(file_path) -> str:
     """Run task type given a set of parameters.
 
     \b
     Parameters
     ----------
```

### Comparing `whiffle_client-0.2.2/whiffle_client/resources/example_generic_params.json` & `whiffle_client-0.2.3/whiffle_client/resources/example_generic_params.json`

 * *Files identical despite different names*

