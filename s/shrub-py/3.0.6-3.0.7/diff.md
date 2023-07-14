# Comparing `tmp/shrub_py-3.0.6.tar.gz` & `tmp/shrub_py-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shrub_py-3.0.6.tar", max compression
+gzip compressed data, was "shrub_py-3.0.7.tar", max compression
```

## Comparing `shrub_py-3.0.6.tar` & `shrub_py-3.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11536 2023-06-27 23:15:07.085320 shrub_py-3.0.6/LICENSE
--rw-r--r--   0        0        0     1285 2023-06-27 23:15:07.085320 shrub_py-3.0.6/README.md
--rw-r--r--   0        0        0      817 2023-06-27 23:15:07.089320 shrub_py-3.0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-27 23:15:07.089320 shrub_py-3.0.6/src/shrub/__init__.py
--rw-r--r--   0        0        0     1723 2023-06-27 23:15:07.089320 shrub_py-3.0.6/src/shrub/base.py
--rw-r--r--   0        0        0     6189 2023-06-27 23:15:07.089320 shrub_py-3.0.6/src/shrub/command.py
--rw-r--r--   0        0        0     7208 2023-06-27 23:15:07.089320 shrub_py-3.0.6/src/shrub/config.py
--rw-r--r--   0        0        0    28873 2023-06-27 23:15:07.089320 shrub_py-3.0.6/src/shrub/operations.py
--rw-r--r--   0        0        0        0 2023-06-27 23:15:07.089320 shrub_py-3.0.6/src/shrub/py.typed
--rw-r--r--   0        0        0     9305 2023-06-27 23:15:07.089320 shrub_py-3.0.6/src/shrub/task.py
--rw-r--r--   0        0        0      266 2023-06-27 23:15:07.089320 shrub_py-3.0.6/src/shrub/v2/__init__.py
--rw-r--r--   0        0        0    22752 2023-06-27 23:15:07.089320 shrub_py-3.0.6/src/shrub/v2/command.py
--rw-r--r--   0        0        0      992 2023-06-27 23:15:07.089320 shrub_py-3.0.6/src/shrub/v2/dict_creation_util.py
--rw-r--r--   0        0        0     2386 2023-06-27 23:15:07.089320 shrub_py-3.0.6/src/shrub/v2/project.py
--rw-r--r--   0        0        0     5561 2023-06-27 23:15:07.089320 shrub_py-3.0.6/src/shrub/v2/task.py
--rw-r--r--   0        0        0     9495 2023-06-27 23:15:07.089320 shrub_py-3.0.6/src/shrub/v2/variant.py
--rw-r--r--   0        0        0        0 2023-06-27 23:15:07.089320 shrub_py-3.0.6/src/shrub/v3/__init__.py
--rw-r--r--   0        0        0     1439 2023-06-27 23:15:07.089320 shrub_py-3.0.6/src/shrub/v3/evg_build_variant.py
--rw-r--r--   0        0        0    33152 2023-06-27 23:15:07.089320 shrub_py-3.0.6/src/shrub/v3/evg_command.py
--rw-r--r--   0        0        0     3187 2023-06-27 23:15:07.089320 shrub_py-3.0.6/src/shrub/v3/evg_project.py
--rw-r--r--   0        0        0     1663 2023-06-27 23:15:07.089320 shrub_py-3.0.6/src/shrub/v3/evg_task.py
--rw-r--r--   0        0        0     1968 2023-06-27 23:15:07.089320 shrub_py-3.0.6/src/shrub/v3/evg_task_group.py
--rw-r--r--   0        0        0      921 2023-06-27 23:15:07.089320 shrub_py-3.0.6/src/shrub/v3/shrub_service.py
--rw-r--r--   0        0        0    10210 2023-06-27 23:15:07.089320 shrub_py-3.0.6/src/shrub/variant.py
--rw-r--r--   0        0        0     2228 1970-01-01 00:00:00.000000 shrub_py-3.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11536 2023-07-14 20:00:24.977757 shrub_py-3.0.7/LICENSE
+-rw-r--r--   0        0        0     1285 2023-07-14 20:00:24.977757 shrub_py-3.0.7/README.md
+-rw-r--r--   0        0        0      837 2023-07-14 20:00:24.981757 shrub_py-3.0.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/__init__.py
+-rw-r--r--   0        0        0     1723 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/base.py
+-rw-r--r--   0        0        0     6189 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/command.py
+-rw-r--r--   0        0        0     7769 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/config.py
+-rw-r--r--   0        0        0    28873 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/operations.py
+-rw-r--r--   0        0        0        0 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/py.typed
+-rw-r--r--   0        0        0     9305 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/task.py
+-rw-r--r--   0        0        0      266 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/v2/__init__.py
+-rw-r--r--   0        0        0    22752 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/v2/command.py
+-rw-r--r--   0        0        0      992 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/v2/dict_creation_util.py
+-rw-r--r--   0        0        0     2386 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/v2/project.py
+-rw-r--r--   0        0        0     5561 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/v2/task.py
+-rw-r--r--   0        0        0     9669 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/v2/variant.py
+-rw-r--r--   0        0        0        0 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/v3/__init__.py
+-rw-r--r--   0        0        0     1535 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/v3/evg_build_variant.py
+-rw-r--r--   0        0        0    33152 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/v3/evg_command.py
+-rw-r--r--   0        0        0     3187 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/v3/evg_project.py
+-rw-r--r--   0        0        0     1663 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/v3/evg_task.py
+-rw-r--r--   0        0        0     1968 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/v3/evg_task_group.py
+-rw-r--r--   0        0        0      921 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/v3/shrub_service.py
+-rw-r--r--   0        0        0    10210 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/variant.py
+-rw-r--r--   0        0        0     2269 1970-01-01 00:00:00.000000 shrub_py-3.0.7/PKG-INFO
```

### Comparing `shrub_py-3.0.6/LICENSE` & `shrub_py-3.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `shrub_py-3.0.6/README.md` & `shrub_py-3.0.7/README.md`

 * *Files identical despite different names*

### Comparing `shrub_py-3.0.6/pyproject.toml` & `shrub_py-3.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shrub.py"
-version = "3.0.6"
+version = "3.0.7"
 description = "Library for creating evergreen configurations"
 authors = [
     "David Bradford <david.bradford@mongodb.com>",
     "Lydia Stepanek <lydia.stepanek@mongodb.com>",
     "Tausif Rahman <tausif.rahman@mongodb.com>"
 ]
 license = "Apache-2.0"
@@ -17,14 +17,15 @@
 [tool.poetry.dependencies]
 python = ">3.7.0"
 PyYaml = "^5.1"
 dataclasses = {version = "^0.7", python = "3.6.*"}
 pydantic = "^1.8"
 git-url-parse = "^1"
 typing-extensions = "^4"
+croniter = "^1.4.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.0"
 pytest-black = "^0.3"
 pytest-flake8 = "^1.0"
 pytest-mypy = "^0.8.0"
 black = "^23.3.0"
```

### Comparing `shrub_py-3.0.6/src/shrub/base.py` & `shrub_py-3.0.7/src/shrub/base.py`

 * *Files identical despite different names*

### Comparing `shrub_py-3.0.6/src/shrub/command.py` & `shrub_py-3.0.7/src/shrub/command.py`

 * *Files identical despite different names*

### Comparing `shrub_py-3.0.6/src/shrub/config.py` & `shrub_py-3.0.7/src/shrub/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from shrub.base import EvergreenBuilder
 from shrub.base import NAME_KEY
 from shrub.base import RECURSE_KEY
 from shrub.command import CommandSequence
 from shrub.task import Task
 from shrub.task import TaskGroup
 from shrub.variant import Variant
+from croniter import croniter
 
 
 def _find_name_in_list(name_list, name):
     """Call get_name() on all items in the given list to find a match."""
     for l in name_list:  # noqa: E741
         if l.get_name() == name:
             return l
@@ -29,28 +30,30 @@
         self._variants = []
         self._pre = None
         self._post = None
         self._timeout = None
 
         self._exec_timeout_secs = None
         self._batch_time_secs = None
+        self._cron = None
         self._stepback = None
         self._command_type = None
         self._ignore_files = []
 
     def _yaml_map(self):
         return {
             "_tasks": {NAME_KEY: "tasks", RECURSE_KEY: True},
             "_groups": {NAME_KEY: "task_groups", RECURSE_KEY: True},
             "_variants": {NAME_KEY: "buildvariants", RECURSE_KEY: True},
             "_pre": {NAME_KEY: "pre", RECURSE_KEY: True},
             "_post": {NAME_KEY: "post", RECURSE_KEY: True},
             "_timeout": {NAME_KEY: "timeout", RECURSE_KEY: False},
             "_exec_timeout_secs": {NAME_KEY: "exec_timeout_secs", RECURSE_KEY: False},
             "_batch_time_secs": {NAME_KEY: "batchtime", RECURSE_KEY: False},
+            "_cron": {NAME_KEY: "cron", RECURSE_KEY: False},
             "_stepback": {NAME_KEY: "stepback", RECURSE_KEY: False},
             "_command_type": {NAME_KEY: "command_type", RECURSE_KEY: False},
             "_ignore_files": {NAME_KEY: "ignore", RECURSE_KEY: False},
         }
 
     def task(self, name):
         """
@@ -178,14 +181,30 @@
         """
         if not isinstance(duration, int):
             raise TypeError("batch_time only accepts an int")
 
         self._batch_time_secs = duration
         return self
 
+    def cron(self, cron_schedule):
+        """
+        Sets the cron schedule.
+
+        :param cron_schedule: cron schedule to set.
+        :return: instance of config.
+        """
+        if not isinstance(cron_schedule, str):
+            raise TypeError("cron only accepts strings")
+
+        if not croniter.is_valid(cron_schedule):
+            raise ValueError("Invalid cron syntax")
+
+        self._cron = cron_schedule
+        return self
+
     def stepback(self):
         """
         Enables stepback for this config.
 
         :return: instance of config.
         """
         self._stepback = True
```

### Comparing `shrub_py-3.0.6/src/shrub/operations.py` & `shrub_py-3.0.7/src/shrub/operations.py`

 * *Files identical despite different names*

### Comparing `shrub_py-3.0.6/src/shrub/task.py` & `shrub_py-3.0.7/src/shrub/task.py`

 * *Files identical despite different names*

### Comparing `shrub_py-3.0.6/src/shrub/v2/command.py` & `shrub_py-3.0.7/src/shrub/v2/command.py`

 * *Files identical despite different names*

### Comparing `shrub_py-3.0.6/src/shrub/v2/dict_creation_util.py` & `shrub_py-3.0.7/src/shrub/v2/dict_creation_util.py`

 * *Files identical despite different names*

### Comparing `shrub_py-3.0.6/src/shrub/v2/project.py` & `shrub_py-3.0.7/src/shrub/v2/project.py`

 * *Files identical despite different names*

### Comparing `shrub_py-3.0.6/src/shrub/v2/task.py` & `shrub_py-3.0.7/src/shrub/v2/task.py`

 * *Files identical despite different names*

### Comparing `shrub_py-3.0.6/src/shrub/v2/variant.py` & `shrub_py-3.0.7/src/shrub/v2/variant.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,34 +26,37 @@
     """Representation of a Build Variant."""
 
     def __init__(
         self,
         name: str,
         display_name: Optional[str] = None,
         batch_time: Optional[int] = None,
+        cron: Optional[str] = None,
         expansions: Optional[Dict[str, Any]] = None,
         run_on: Optional[Sequence[str]] = None,
         modules: Optional[Sequence[str]] = None,
         activate: Optional[bool] = None,
     ) -> None:
         """
         Create a new build variant.
 
         :param name: Name of build variant.
         :param display_name: Display name of build variant.
         :param batch_time: Interval of time in minutes that evergreen should wait before activating
             this variant.
+        :param cron: Schedule in cron syntax that this variant should run on.
         :param expansions: A set of key-value expansions pairs.
         :param run_on: Which distros the tasks should run on.
         :param modules: Which modules to include in this build variant.
         :param activate: Should the build variant be scheduled by default.
         """
         self.name = name
         self.display_name = display_name
         self.batch_time = batch_time
+        self.cron = cron
         self.tasks: Set[Task] = set()
         self.task_groups: Set[TaskGroup] = set()
         self.existing_tasks: Set[ExistingTask] = set()
         self.display_tasks: Set[_DisplayTask] = set()
         self.expansions: Dict[str, Any] = expansions if expansions else {}
         self.run_on = run_on
         self.modules = modules
@@ -241,12 +244,13 @@
             obj,
             {
                 "expansions": self.expansions,
                 "run_on": self.run_on,
                 "modules": self.modules,
                 "display_name": self.display_name,
                 "batch_time": self.batch_time,
+                "cron": self.cron,
                 "activate": self.activate,
             },
         )
 
         return obj
```

### Comparing `shrub_py-3.0.6/src/shrub/v3/evg_build_variant.py` & `shrub_py-3.0.7/src/shrub/v3/evg_build_variant.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,22 +24,24 @@
 
     * name: ID of build variant.
     * tasks: List of tasks to run on this build variant.
     * display_name: Name of build variant.
     * run_on: Distros that tasks should be run on.
     * display_tasks: Display tasks that are part of the build variant.
     * batchtime: How frequent this build variant should be run.
+    * cron: What cron schedule this build variant should run on.
     * expansions: Definition of expansions for this build variant.
     * stepback: If stepback should be run on this build variant.
     * module: List of modules to include in this build variant.
     """
 
     name: str
     tasks: List[EvgTaskRef]
     display_name: Optional[str] = None
     run_on: Optional[List[str]] = None
     display_tasks: Optional[List[DisplayTask]] = None
     batchtime: Optional[int] = None
+    cron: Optional[str] = None
     expansions: Optional[Dict[str, str]] = None
     stepback: Optional[bool] = None
     modules: Optional[List[str]] = None
     tags: Optional[List[str]] = None
```

### Comparing `shrub_py-3.0.6/src/shrub/v3/evg_command.py` & `shrub_py-3.0.7/src/shrub/v3/evg_command.py`

 * *Files identical despite different names*

### Comparing `shrub_py-3.0.6/src/shrub/v3/evg_project.py` & `shrub_py-3.0.7/src/shrub/v3/evg_project.py`

 * *Files identical despite different names*

### Comparing `shrub_py-3.0.6/src/shrub/v3/evg_task.py` & `shrub_py-3.0.7/src/shrub/v3/evg_task.py`

 * *Files identical despite different names*

### Comparing `shrub_py-3.0.6/src/shrub/v3/evg_task_group.py` & `shrub_py-3.0.7/src/shrub/v3/evg_task_group.py`

 * *Files identical despite different names*

### Comparing `shrub_py-3.0.6/src/shrub/v3/shrub_service.py` & `shrub_py-3.0.7/src/shrub/v3/shrub_service.py`

 * *Files identical despite different names*

### Comparing `shrub_py-3.0.6/src/shrub/variant.py` & `shrub_py-3.0.7/src/shrub/variant.py`

 * *Files identical despite different names*

### Comparing `shrub_py-3.0.6/PKG-INFO` & `shrub_py-3.0.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: shrub-py
-Version: 3.0.6
+Version: 3.0.7
 Summary: Library for creating evergreen configurations
 Home-page: https://github.com/evergreen-ci/shrub.py
 License: Apache-2.0
 Author: David Bradford
 Author-email: david.bradford@mongodb.com
 Requires-Python: >3.7.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYaml (>=5.1,<6.0)
+Requires-Dist: croniter (>=1.4.1,<2.0.0)
 Requires-Dist: dataclasses (>=0.7,<0.8) ; python_version >= "3.6.dev0" and python_version < "3.7.dev0"
 Requires-Dist: git-url-parse (>=1,<2)
 Requires-Dist: pydantic (>=1.8,<2.0)
 Requires-Dist: typing-extensions (>=4,<5)
 Project-URL: Repository, https://github.com/evergreen-ci/shrub.py
 Description-Content-Type: text/markdown
```

