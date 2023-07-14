# Comparing `tmp/planbee-0.1.4.tar.gz` & `tmp/planbee-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planbee-0.1.4.tar", last modified: Fri Jul 14 09:51:10 2023, max compression
+gzip compressed data, was "planbee-0.1.5.tar", last modified: Fri Jul 14 10:08:03 2023, max compression
```

## Comparing `planbee-0.1.4.tar` & `planbee-0.1.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:51:10.024327 planbee-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-14 09:51:06.000000 planbee-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-14 09:51:10.024327 planbee-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-14 09:51:06.000000 planbee-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-14 09:51:10.024327 planbee-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-14 09:51:06.000000 planbee-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:51:10.016327 planbee-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:51:10.024327 planbee-0.1.4/src/planbee/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-14 09:51:06.000000 planbee-0.1.4/src/planbee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-14 09:51:10.024327 planbee-0.1.4/src/planbee/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:51:10.020327 planbee-0.1.4/src/planbee/models/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-14 09:51:06.000000 planbee-0.1.4/src/planbee/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-14 09:51:06.000000 planbee-0.1.4/src/planbee/models/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-14 09:51:06.000000 planbee-0.1.4/src/planbee/models/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:51:10.024327 planbee-0.1.4/src/planbee/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:51:06.000000 planbee-0.1.4/src/planbee/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-14 09:51:06.000000 planbee-0.1.4/src/planbee/scheduler/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:51:10.024327 planbee-0.1.4/src/planbee/scheduler/heuristic_solver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:51:06.000000 planbee-0.1.4/src/planbee/scheduler/heuristic_solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-07-14 09:51:06.000000 planbee-0.1.4/src/planbee/scheduler/heuristic_solver/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-07-14 09:51:06.000000 planbee-0.1.4/src/planbee/scheduler/heuristic_solver/task_allocator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-07-14 09:51:06.000000 planbee-0.1.4/src/planbee/scheduler/heuristic_solver/window_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-14 09:51:06.000000 planbee-0.1.4/src/planbee/scheduler/scheduler_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-07-14 09:51:06.000000 planbee-0.1.4/src/planbee/scheduler/task_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-14 09:51:06.000000 planbee-0.1.4/src/planbee/scheduler/task_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-14 09:51:06.000000 planbee-0.1.4/src/planbee/scheduler/visualizations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:51:10.020327 planbee-0.1.4/src/planbee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-14 09:51:10.000000 planbee-0.1.4/src/planbee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-14 09:51:10.000000 planbee-0.1.4/src/planbee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 09:51:10.000000 planbee-0.1.4/src/planbee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 09:51:10.000000 planbee-0.1.4/src/planbee.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-14 09:51:10.000000 planbee-0.1.4/src/planbee.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 09:51:10.000000 planbee-0.1.4/src/planbee.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:08:03.381983 planbee-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-14 10:07:58.000000 planbee-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-14 10:08:03.381983 planbee-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-14 10:07:58.000000 planbee-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-14 10:08:03.381983 planbee-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-14 10:07:58.000000 planbee-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:08:03.381983 planbee-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:08:03.381983 planbee-0.1.5/src/planbee/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-14 10:07:58.000000 planbee-0.1.5/src/planbee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-14 10:08:03.381983 planbee-0.1.5/src/planbee/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:08:03.381983 planbee-0.1.5/src/planbee/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-14 10:07:58.000000 planbee-0.1.5/src/planbee/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-14 10:07:58.000000 planbee-0.1.5/src/planbee/models/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-14 10:07:58.000000 planbee-0.1.5/src/planbee/models/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:08:03.381983 planbee-0.1.5/src/planbee/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:07:58.000000 planbee-0.1.5/src/planbee/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-14 10:07:58.000000 planbee-0.1.5/src/planbee/scheduler/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:08:03.381983 planbee-0.1.5/src/planbee/scheduler/heuristic_solver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:07:58.000000 planbee-0.1.5/src/planbee/scheduler/heuristic_solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-07-14 10:07:58.000000 planbee-0.1.5/src/planbee/scheduler/heuristic_solver/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-07-14 10:07:58.000000 planbee-0.1.5/src/planbee/scheduler/heuristic_solver/task_allocator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-07-14 10:07:58.000000 planbee-0.1.5/src/planbee/scheduler/heuristic_solver/window_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-14 10:07:58.000000 planbee-0.1.5/src/planbee/scheduler/scheduler_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-07-14 10:07:58.000000 planbee-0.1.5/src/planbee/scheduler/task_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-14 10:07:58.000000 planbee-0.1.5/src/planbee/scheduler/task_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-14 10:07:58.000000 planbee-0.1.5/src/planbee/scheduler/visualizations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:08:03.381983 planbee-0.1.5/src/planbee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-14 10:08:03.000000 planbee-0.1.5/src/planbee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-14 10:08:03.000000 planbee-0.1.5/src/planbee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:08:03.000000 planbee-0.1.5/src/planbee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:08:03.000000 planbee-0.1.5/src/planbee.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-14 10:08:03.000000 planbee-0.1.5/src/planbee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 10:08:03.000000 planbee-0.1.5/src/planbee.egg-info/top_level.txt
```

### Comparing `planbee-0.1.4/LICENSE` & `planbee-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `planbee-0.1.4/PKG-INFO` & `planbee-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planbee
-Version: 0.1.4
+Version: 0.1.5
 Summary: production / job shop / resource scheduler for Python
 Home-page: https://github.com/Yacobolo/PlanBee
 Author: Jacob Østergaard Nielsen
 Author-email: jaoe@oestergaard-as.dk
 License: UNKNOWN
 Description: # PlanBee 🐝
```

### Comparing `planbee-0.1.4/README.md` & `planbee-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `planbee-0.1.4/setup.py` & `planbee-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `planbee-0.1.4/src/planbee/models/resource.py` & `planbee-0.1.5/src/planbee/models/resource.py`

 * *Files identical despite different names*

### Comparing `planbee-0.1.4/src/planbee/models/task.py` & `planbee-0.1.5/src/planbee/models/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .resource import Resource
 
 
 class Task(BaseModel):
     id: Union[int, str]
     duration: int
     priority: int
-    resources: list[list[Resource]]
+    resources: list[set[Resource]]
     resource_count: Union[int, str] = 1
     predecessors: Optional[list["Task"]] = []
     predecessor_delay: int = 0
     batch_size: Optional[int] = None
     quantity: Optional[int] = None
     batch_id: Optional[int] = None
```

### Comparing `planbee-0.1.4/src/planbee/scheduler/core.py` & `planbee-0.1.5/src/planbee/scheduler/core.py`

 * *Files identical despite different names*

### Comparing `planbee-0.1.4/src/planbee/scheduler/heuristic_solver/main.py` & `planbee-0.1.5/src/planbee/scheduler/heuristic_solver/main.py`

 * *Files identical despite different names*

### Comparing `planbee-0.1.4/src/planbee/scheduler/heuristic_solver/task_allocator.py` & `planbee-0.1.5/src/planbee/scheduler/heuristic_solver/task_allocator.py`

 * *Files identical despite different names*

### Comparing `planbee-0.1.4/src/planbee/scheduler/heuristic_solver/window_manager.py` & `planbee-0.1.5/src/planbee/scheduler/heuristic_solver/window_manager.py`

 * *Files identical despite different names*

### Comparing `planbee-0.1.4/src/planbee/scheduler/scheduler_result.py` & `planbee-0.1.5/src/planbee/scheduler/scheduler_result.py`

 * *Files identical despite different names*

### Comparing `planbee-0.1.4/src/planbee/scheduler/task_graph.py` & `planbee-0.1.5/src/planbee/scheduler/task_graph.py`

 * *Files identical despite different names*

### Comparing `planbee-0.1.4/src/planbee/scheduler/task_preprocessor.py` & `planbee-0.1.5/src/planbee/scheduler/task_preprocessor.py`

 * *Files identical despite different names*

### Comparing `planbee-0.1.4/src/planbee.egg-info/PKG-INFO` & `planbee-0.1.5/src/planbee.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planbee
-Version: 0.1.4
+Version: 0.1.5
 Summary: production / job shop / resource scheduler for Python
 Home-page: https://github.com/Yacobolo/PlanBee
 Author: Jacob Østergaard Nielsen
 Author-email: jaoe@oestergaard-as.dk
 License: UNKNOWN
 Description: # PlanBee 🐝
```

### Comparing `planbee-0.1.4/src/planbee.egg-info/SOURCES.txt` & `planbee-0.1.5/src/planbee.egg-info/SOURCES.txt`

 * *Files identical despite different names*

