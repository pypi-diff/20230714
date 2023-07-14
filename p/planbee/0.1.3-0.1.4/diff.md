# Comparing `tmp/planbee-0.1.3.tar.gz` & `tmp/planbee-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planbee-0.1.3.tar", last modified: Tue Jul 11 11:10:29 2023, max compression
+gzip compressed data, was "planbee-0.1.4.tar", last modified: Fri Jul 14 09:51:10 2023, max compression
```

## Comparing `planbee-0.1.3.tar` & `planbee-0.1.4.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:10:29.385908 planbee-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-11 11:10:26.000000 planbee-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-11 11:10:29.385908 planbee-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-11 11:10:26.000000 planbee-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-11 11:10:29.385908 planbee-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-11 11:10:26.000000 planbee-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:10:29.377908 planbee-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:10:29.385908 planbee-0.1.3/src/planbee/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-11 11:10:26.000000 planbee-0.1.3/src/planbee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-11 11:10:29.385908 planbee-0.1.3/src/planbee/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:10:29.381908 planbee-0.1.3/src/planbee/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:10:26.000000 planbee-0.1.3/src/planbee/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-11 11:10:26.000000 planbee-0.1.3/src/planbee/models/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-11 11:10:26.000000 planbee-0.1.3/src/planbee/models/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:10:29.381908 planbee-0.1.3/src/planbee/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:10:26.000000 planbee-0.1.3/src/planbee/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-11 11:10:26.000000 planbee-0.1.3/src/planbee/scheduler/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:10:29.381908 planbee-0.1.3/src/planbee/scheduler/heuristic_solver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:10:26.000000 planbee-0.1.3/src/planbee/scheduler/heuristic_solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-07-11 11:10:26.000000 planbee-0.1.3/src/planbee/scheduler/heuristic_solver/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    10798 2023-07-11 11:10:26.000000 planbee-0.1.3/src/planbee/scheduler/heuristic_solver/task_allocator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-07-11 11:10:26.000000 planbee-0.1.3/src/planbee/scheduler/heuristic_solver/task_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-07-11 11:10:26.000000 planbee-0.1.3/src/planbee/scheduler/heuristic_solver/window_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-11 11:10:26.000000 planbee-0.1.3/src/planbee/scheduler/scheduler_result.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-11 11:10:26.000000 planbee-0.1.3/src/planbee/scheduler/visualizations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:10:29.381908 planbee-0.1.3/src/planbee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-11 11:10:29.000000 planbee-0.1.3/src/planbee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-11 11:10:29.000000 planbee-0.1.3/src/planbee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 11:10:29.000000 planbee-0.1.3/src/planbee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 11:10:29.000000 planbee-0.1.3/src/planbee.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-11 11:10:29.000000 planbee-0.1.3/src/planbee.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 11:10:29.000000 planbee-0.1.3/src/planbee.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:51:10.024327 planbee-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-14 09:51:06.000000 planbee-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-14 09:51:10.024327 planbee-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-14 09:51:06.000000 planbee-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-14 09:51:10.024327 planbee-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-14 09:51:06.000000 planbee-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:51:10.016327 planbee-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:51:10.024327 planbee-0.1.4/src/planbee/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-14 09:51:06.000000 planbee-0.1.4/src/planbee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-14 09:51:10.024327 planbee-0.1.4/src/planbee/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:51:10.020327 planbee-0.1.4/src/planbee/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-14 09:51:06.000000 planbee-0.1.4/src/planbee/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-14 09:51:06.000000 planbee-0.1.4/src/planbee/models/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-14 09:51:06.000000 planbee-0.1.4/src/planbee/models/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:51:10.024327 planbee-0.1.4/src/planbee/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:51:06.000000 planbee-0.1.4/src/planbee/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-14 09:51:06.000000 planbee-0.1.4/src/planbee/scheduler/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:51:10.024327 planbee-0.1.4/src/planbee/scheduler/heuristic_solver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:51:06.000000 planbee-0.1.4/src/planbee/scheduler/heuristic_solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-07-14 09:51:06.000000 planbee-0.1.4/src/planbee/scheduler/heuristic_solver/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-07-14 09:51:06.000000 planbee-0.1.4/src/planbee/scheduler/heuristic_solver/task_allocator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-07-14 09:51:06.000000 planbee-0.1.4/src/planbee/scheduler/heuristic_solver/window_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-14 09:51:06.000000 planbee-0.1.4/src/planbee/scheduler/scheduler_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-07-14 09:51:06.000000 planbee-0.1.4/src/planbee/scheduler/task_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-14 09:51:06.000000 planbee-0.1.4/src/planbee/scheduler/task_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-14 09:51:06.000000 planbee-0.1.4/src/planbee/scheduler/visualizations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:51:10.020327 planbee-0.1.4/src/planbee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-14 09:51:10.000000 planbee-0.1.4/src/planbee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-14 09:51:10.000000 planbee-0.1.4/src/planbee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 09:51:10.000000 planbee-0.1.4/src/planbee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 09:51:10.000000 planbee-0.1.4/src/planbee.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-14 09:51:10.000000 planbee-0.1.4/src/planbee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 09:51:10.000000 planbee-0.1.4/src/planbee.egg-info/top_level.txt
```

### Comparing `planbee-0.1.3/LICENSE` & `planbee-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `planbee-0.1.3/PKG-INFO` & `planbee-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planbee
-Version: 0.1.3
+Version: 0.1.4
 Summary: production / job shop / resource scheduler for Python
 Home-page: https://github.com/Yacobolo/PlanBee
 Author: Jacob Østergaard Nielsen
 Author-email: jaoe@oestergaard-as.dk
 License: UNKNOWN
 Description: # PlanBee 🐝
```

### Comparing `planbee-0.1.3/README.md` & `planbee-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `planbee-0.1.3/setup.py` & `planbee-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `planbee-0.1.3/src/planbee/models/resource.py` & `planbee-0.1.4/src/planbee/models/resource.py`

 * *Files identical despite different names*

### Comparing `planbee-0.1.3/src/planbee/models/task.py` & `planbee-0.1.4/src/planbee/models/task.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,21 +3,24 @@
 
 from pydantic import BaseModel, validator
 
 from .resource import Resource
 
 
 class Task(BaseModel):
-    id: int
+    id: Union[int, str]
     duration: int
     priority: int
     resources: list[list[Resource]]
     resource_count: Union[int, str] = 1
     predecessors: Optional[list["Task"]] = []
     predecessor_delay: int = 0
+    batch_size: Optional[int] = None
+    quantity: Optional[int] = None
+    batch_id: Optional[int] = None
 
     @validator("resources", pre=True)
     def ensure_list(cls, v):
         if not isinstance(v, list):  # if a single resource object is passed
             return [[v]]  # make it a list of list
         if (
             isinstance(v, list) and len(v) > 0 and not isinstance(v[0], list)
```

### Comparing `planbee-0.1.3/src/planbee/scheduler/core.py` & `planbee-0.1.4/src/planbee/scheduler/core.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,27 @@
+from ..models import Task
 from .heuristic_solver.main import HeuristicSolver
 from .scheduler_result import SchedulerResult
+from .task_graph import TaskGraph
 
 
 class Scheduler:
-    def __init__(self, tasks):
+    def __init__(self, tasks: list[Task]):
         self.tasks = tasks
         self.resources = set(
             [resource for task in tasks for resource in task.get_resources()]
         )
+        self.task_graph = TaskGraph(tasks)
+
+    def schedule(self):
+        # merge intervals for all resources
         for resource in self.resources:
             resource.merge_intervals()
 
-    def schedule(self):
-        heuristic_solver = HeuristicSolver(self.tasks, self.resources)
+        # schedule tasks
+        task_order = self.task_graph.get_task_order()
+        heuristic_solver = HeuristicSolver(self.tasks, self.resources, task_order)
         result = heuristic_solver.solve()
 
         scheduler_result = SchedulerResult(result)
         print(scheduler_result.summary())
         return scheduler_result
-        return scheduler_result
```

### Comparing `planbee-0.1.3/src/planbee/scheduler/heuristic_solver/main.py` & `planbee-0.1.4/src/planbee/scheduler/heuristic_solver/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 import numpy as np
 
 from .task_allocator import TaskAllocator
-from .task_graph import TaskGraph
 from .window_manager import WindowManager
 
 
 class HeuristicSolver:
-    def __init__(self, tasks, resources):
+    def __init__(self, tasks, resources, task_order):
         self.task_allocator = TaskAllocator()
-        self.task_graph = TaskGraph(tasks)
+        self.task_order = task_order
         self.window_manager = WindowManager(resources)
         self.task_vars = {
             task.id: {
                 "task_id": task.id,
                 "assigned_resource_ids": None,
                 "task_start": None,
                 "task_end": None,
                 "resource_intervals": None,
             }
             for task in tasks
         }
         self.task_dict = {task.id: task for task in tasks}
 
     def solve(self):
-        task_order = self.task_graph.get_task_order()
         unscheduled_tasks = []
 
-        for task_id in task_order:
+        for task_id in self.task_order:
             task = self.task_dict[task_id]
 
             # get task resources and windows dict
-            task_resource_ids = [resource.id for resource in task.get_resources()]
+            task_resource_ids = np.array(
+                [resource.id for resource in task.get_resources()]
+            )
+
             task_earliest_start = self._get_task_earliest_start(task)
 
             if task_earliest_start is None:
                 unscheduled_tasks.append(task_id)
                 continue
 
-            task_resource_windows_dict = (
-                self.window_manager.get_task_resource_windows_dict(
-                    task_resource_ids, task_earliest_start
-                )
+            task_resource_windows = self.window_manager.get_task_resource_windows(
+                task_resource_ids, task_earliest_start
             )
-            if not task_resource_windows_dict:
+            if not task_resource_windows:
                 unscheduled_tasks.append(task_id)
                 continue
 
             # allocate task
             allocated_resource_windows_dict = self.task_allocator.allocate_task(
-                resource_windows_dict=task_resource_windows_dict,
+                resource_windows=task_resource_windows,
+                resource_ids=task_resource_ids,
                 task_duration=task.duration,
                 resource_count=task.resource_count,
                 resource_group_indices=task.get_resource_group_indices(),
             )
 
             if not allocated_resource_windows_dict:
                 unscheduled_tasks.append(task_id)
@@ -99,8 +99,7 @@
 
         for key, value_list in d.items():
             min_val = np.min([x[0] for x in value_list])
             max_val = np.max([x[1] for x in value_list])
             result[key] = (min_val, max_val)
 
         return result
-        return result
```

### Comparing `planbee-0.1.3/src/planbee/scheduler/heuristic_solver/task_allocator.py` & `planbee-0.1.4/src/planbee/scheduler/heuristic_solver/task_allocator.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 import numpy as np
 
 
 class TaskAllocator:
     def allocate_task(
         self,
-        resource_windows_dict: np.array,
+        resource_windows: list[np.array],
+        resource_ids: np.array,
         task_duration: float,
         resource_count: int,
         resource_group_indices: list[list[int]],
     ) -> Optional[dict[int, np.array]]:
-        windows = list(resource_windows_dict.values())
-        matrix = self.create_matrix(windows)
-        resource_ids = np.array(list(resource_windows_dict.keys()))
+        matrix = self.create_matrix(resource_windows)
+
         solution_matrix, solution_resource_ids = self.solve_matrix(
             matrix=matrix,
             task_duration=task_duration,
             resource_ids=resource_ids,
             resource_count=resource_count,
             resource_group_indices=resource_group_indices,
         )
```

### Comparing `planbee-0.1.3/src/planbee/scheduler/heuristic_solver/task_graph.py` & `planbee-0.1.4/src/planbee/scheduler/task_graph.py`

 * *Files identical despite different names*

### Comparing `planbee-0.1.3/src/planbee/scheduler/heuristic_solver/window_manager.py` & `planbee-0.1.4/src/planbee/scheduler/heuristic_solver/window_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,32 +13,32 @@
         Creates a dictionary mapping resource IDs to numpy arrays representing windows.
         """
         return {
             resource.id: self.windows_to_numpy(resource.available_windows)
             for resource in self.resources
         }
 
-    def get_task_resource_windows_dict(
+    def get_task_resource_windows(
         self, task_resource_ids: list[int], task_earliest_start: int
-    ) -> dict[int, np.ndarray]:
+    ) -> list[np.ndarray]:
         """
-        Returns a subset of the resource windows dict for the given resource IDs.
+        Returns the resource windows for the resource ids.
         The windows are trimmed to the min_task_start.
         """
-        return {
-            resource_id: trimmed_window
+        return [
+            trimmed_window
             for resource_id in task_resource_ids
             if (
                 trimmed_window := self.trim_window(
                     window=self.resource_windows_dict[resource_id],
                     trim_interval=(0, task_earliest_start),
                 )
             ).size
             > 0
-        }
+        ]
 
     def windows_to_numpy(self, windows: list[tuple[int, int]]) -> np.ndarray:
         """
         Converts a list of windows to a numpy array.
         """
         arr = np.array(windows)
         return np.concatenate([arr, np.diff(arr), np.zeros((arr.shape[0], 1))], axis=1)
```

### Comparing `planbee-0.1.3/src/planbee/scheduler/scheduler_result.py` & `planbee-0.1.4/src/planbee/scheduler/scheduler_result.py`

 * *Files identical despite different names*

### Comparing `planbee-0.1.3/src/planbee.egg-info/PKG-INFO` & `planbee-0.1.4/src/planbee.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planbee
-Version: 0.1.3
+Version: 0.1.4
 Summary: production / job shop / resource scheduler for Python
 Home-page: https://github.com/Yacobolo/PlanBee
 Author: Jacob Østergaard Nielsen
 Author-email: jaoe@oestergaard-as.dk
 License: UNKNOWN
 Description: # PlanBee 🐝
```

### Comparing `planbee-0.1.3/src/planbee.egg-info/SOURCES.txt` & `planbee-0.1.4/src/planbee.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -12,13 +12,14 @@
 src/planbee.egg-info/top_level.txt
 src/planbee/models/__init__.py
 src/planbee/models/resource.py
 src/planbee/models/task.py
 src/planbee/scheduler/__init__.py
 src/planbee/scheduler/core.py
 src/planbee/scheduler/scheduler_result.py
+src/planbee/scheduler/task_graph.py
+src/planbee/scheduler/task_preprocessor.py
 src/planbee/scheduler/visualizations.py
 src/planbee/scheduler/heuristic_solver/__init__.py
 src/planbee/scheduler/heuristic_solver/main.py
 src/planbee/scheduler/heuristic_solver/task_allocator.py
-src/planbee/scheduler/heuristic_solver/task_graph.py
 src/planbee/scheduler/heuristic_solver/window_manager.py
```

