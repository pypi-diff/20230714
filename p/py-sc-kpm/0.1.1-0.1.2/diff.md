# Comparing `tmp/py-sc-kpm-0.1.1.tar.gz` & `tmp/py-sc-kpm-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-sc-kpm-0.1.1.tar", last modified: Fri Jul 14 11:12:34 2023, max compression
+gzip compressed data, was "py-sc-kpm-0.1.2.tar", last modified: Fri Jul 14 13:44:26 2023, max compression
```

## Comparing `py-sc-kpm-0.1.1.tar` & `py-sc-kpm-0.1.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:12:34.857563 py-sc-kpm-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    27598 2023-07-14 11:12:34.857563 py-sc-kpm-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26739 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-14 11:12:34.857563 py-sc-kpm-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:12:34.853563 py-sc-kpm-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:12:34.853563 py-sc-kpm-0.1.1/src/py_sc_kpm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27598 2023-07-14 11:12:34.000000 py-sc-kpm-0.1.1/src/py_sc_kpm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-14 11:12:34.000000 py-sc-kpm-0.1.1/src/py_sc_kpm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 11:12:34.000000 py-sc-kpm-0.1.1/src/py_sc_kpm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-14 11:12:34.000000 py-sc-kpm-0.1.1/src/py_sc_kpm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 11:12:34.000000 py-sc-kpm-0.1.1/src/py_sc_kpm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:12:34.857563 py-sc-kpm-0.1.1/src/sc_kpm/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/src/sc_kpm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/src/sc_kpm/identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/src/sc_kpm/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/src/sc_kpm/sc_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/src/sc_kpm/sc_keynodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/src/sc_kpm/sc_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/src/sc_kpm/sc_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/src/sc_kpm/sc_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:12:34.857563 py-sc-kpm-0.1.1/src/sc_kpm/sc_sets/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/src/sc_kpm/sc_sets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/src/sc_kpm/sc_sets/sc_numbered_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/src/sc_kpm/sc_sets/sc_oriented_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/src/sc_kpm/sc_sets/sc_set.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/src/sc_kpm/sc_sets/sc_structure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:12:34.857563 py-sc-kpm-0.1.1/src/sc_kpm/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/src/sc_kpm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/src/sc_kpm/utils/action_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/src/sc_kpm/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/src/sc_kpm/utils/iteration_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:12:34.857563 py-sc-kpm-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/tests/test_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/tests/test_keynodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:44:26.585687 py-sc-kpm-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-14 13:44:17.000000 py-sc-kpm-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    27598 2023-07-14 13:44:26.585687 py-sc-kpm-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26739 2023-07-14 13:44:17.000000 py-sc-kpm-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-14 13:44:26.585687 py-sc-kpm-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-14 13:44:17.000000 py-sc-kpm-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:44:26.581687 py-sc-kpm-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:44:26.581687 py-sc-kpm-0.1.2/src/py_sc_kpm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27598 2023-07-14 13:44:26.000000 py-sc-kpm-0.1.2/src/py_sc_kpm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-14 13:44:26.000000 py-sc-kpm-0.1.2/src/py_sc_kpm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 13:44:26.000000 py-sc-kpm-0.1.2/src/py_sc_kpm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-14 13:44:26.000000 py-sc-kpm-0.1.2/src/py_sc_kpm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 13:44:26.000000 py-sc-kpm-0.1.2/src/py_sc_kpm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:44:26.581687 py-sc-kpm-0.1.2/src/sc_kpm/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-14 13:44:17.000000 py-sc-kpm-0.1.2/src/sc_kpm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-07-14 13:44:17.000000 py-sc-kpm-0.1.2/src/sc_kpm/identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-14 13:44:17.000000 py-sc-kpm-0.1.2/src/sc_kpm/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-07-14 13:44:17.000000 py-sc-kpm-0.1.2/src/sc_kpm/sc_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-14 13:44:17.000000 py-sc-kpm-0.1.2/src/sc_kpm/sc_keynodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-07-14 13:44:17.000000 py-sc-kpm-0.1.2/src/sc_kpm/sc_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-14 13:44:17.000000 py-sc-kpm-0.1.2/src/sc_kpm/sc_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-07-14 13:44:17.000000 py-sc-kpm-0.1.2/src/sc_kpm/sc_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:44:26.581687 py-sc-kpm-0.1.2/src/sc_kpm/sc_sets/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-14 13:44:17.000000 py-sc-kpm-0.1.2/src/sc_kpm/sc_sets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-14 13:44:17.000000 py-sc-kpm-0.1.2/src/sc_kpm/sc_sets/sc_numbered_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-07-14 13:44:17.000000 py-sc-kpm-0.1.2/src/sc_kpm/sc_sets/sc_oriented_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-07-14 13:44:17.000000 py-sc-kpm-0.1.2/src/sc_kpm/sc_sets/sc_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-14 13:44:17.000000 py-sc-kpm-0.1.2/src/sc_kpm/sc_sets/sc_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:44:26.585687 py-sc-kpm-0.1.2/src/sc_kpm/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-14 13:44:17.000000 py-sc-kpm-0.1.2/src/sc_kpm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6363 2023-07-14 13:44:17.000000 py-sc-kpm-0.1.2/src/sc_kpm/utils/action_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-07-14 13:44:17.000000 py-sc-kpm-0.1.2/src/sc_kpm/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-14 13:44:17.000000 py-sc-kpm-0.1.2/src/sc_kpm/utils/iteration_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:44:26.585687 py-sc-kpm-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-07-14 13:44:17.000000 py-sc-kpm-0.1.2/tests/test_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-14 13:44:17.000000 py-sc-kpm-0.1.2/tests/test_keynodes.py
```

### Comparing `py-sc-kpm-0.1.1/LICENSE` & `py-sc-kpm-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py-sc-kpm-0.1.1/PKG-INFO` & `py-sc-kpm-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-sc-kpm
-Version: 0.1.1
+Version: 0.1.2
 Summary: The Python implementation of the knowledge processing module for knowledge manipulations
 Home-page: https://github.com/ostis-ai/py-sc-kpm
 Author: ostis-ai
 License: MIT
 Project-URL: Bug Reports, https://github.com/ostis-ai/py-sc-kpm/issues
 Project-URL: Source, https://github.com/ostis-ai/py-sc-kpm
 Keywords: sc-kpm,kpm,knowledge processing
```

### Comparing `py-sc-kpm-0.1.1/README.md` & `py-sc-kpm-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `py-sc-kpm-0.1.1/setup.py` & `py-sc-kpm-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 DIRECTORY_PATH = Path(__file__).parent
 README = (DIRECTORY_PATH / "README.md").read_text()
 
-VERSION = "0.1.1"
+VERSION = "0.1.2"
 INSTALL_REQUIRES = ["py-sc-client>=0.2.6"]
 CURRENT_PYTHON = sys.version_info[:2]
 REQUIRED_PYTHON = (3, 8)
 
 
 if CURRENT_PYTHON < REQUIRED_PYTHON:
     sys.stderr.write(
```

### Comparing `py-sc-kpm-0.1.1/src/py_sc_kpm.egg-info/PKG-INFO` & `py-sc-kpm-0.1.2/src/py_sc_kpm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-sc-kpm
-Version: 0.1.1
+Version: 0.1.2
 Summary: The Python implementation of the knowledge processing module for knowledge manipulations
 Home-page: https://github.com/ostis-ai/py-sc-kpm
 Author: ostis-ai
 License: MIT
 Project-URL: Bug Reports, https://github.com/ostis-ai/py-sc-kpm/issues
 Project-URL: Source, https://github.com/ostis-ai/py-sc-kpm
 Keywords: sc-kpm,kpm,knowledge processing
```

### Comparing `py-sc-kpm-0.1.1/src/py_sc_kpm.egg-info/SOURCES.txt` & `py-sc-kpm-0.1.2/src/py_sc_kpm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-sc-kpm-0.1.1/src/sc_kpm/__init__.py` & `py-sc-kpm-0.1.2/src/sc_kpm/__init__.py`

 * *Files identical despite different names*

### Comparing `py-sc-kpm-0.1.1/src/sc_kpm/identifiers.py` & `py-sc-kpm-0.1.2/src/sc_kpm/identifiers.py`

 * *Files identical despite different names*

### Comparing `py-sc-kpm-0.1.1/src/sc_kpm/sc_agent.py` & `py-sc-kpm-0.1.2/src/sc_kpm/sc_agent.py`

 * *Files identical despite different names*

### Comparing `py-sc-kpm-0.1.1/src/sc_kpm/sc_keynodes.py` & `py-sc-kpm-0.1.2/src/sc_kpm/sc_keynodes.py`

 * *Files identical despite different names*

### Comparing `py-sc-kpm-0.1.1/src/sc_kpm/sc_module.py` & `py-sc-kpm-0.1.2/src/sc_kpm/sc_module.py`

 * *Files identical despite different names*

### Comparing `py-sc-kpm-0.1.1/src/sc_kpm/sc_result.py` & `py-sc-kpm-0.1.2/src/sc_kpm/sc_result.py`

 * *Files identical despite different names*

### Comparing `py-sc-kpm-0.1.1/src/sc_kpm/sc_server.py` & `py-sc-kpm-0.1.2/src/sc_kpm/sc_server.py`

 * *Files identical despite different names*

### Comparing `py-sc-kpm-0.1.1/src/sc_kpm/sc_sets/sc_numbered_set.py` & `py-sc-kpm-0.1.2/src/sc_kpm/sc_sets/sc_numbered_set.py`

 * *Files identical despite different names*

### Comparing `py-sc-kpm-0.1.1/src/sc_kpm/sc_sets/sc_oriented_set.py` & `py-sc-kpm-0.1.2/src/sc_kpm/sc_sets/sc_oriented_set.py`

 * *Files identical despite different names*

### Comparing `py-sc-kpm-0.1.1/src/sc_kpm/sc_sets/sc_set.py` & `py-sc-kpm-0.1.2/src/sc_kpm/sc_sets/sc_set.py`

 * *Files identical despite different names*

### Comparing `py-sc-kpm-0.1.1/src/sc_kpm/sc_sets/sc_structure.py` & `py-sc-kpm-0.1.2/src/sc_kpm/sc_sets/sc_structure.py`

 * *Files identical despite different names*

### Comparing `py-sc-kpm-0.1.1/src/sc_kpm/utils/__init__.py` & `py-sc-kpm-0.1.2/src/sc_kpm/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `py-sc-kpm-0.1.1/src/sc_kpm/utils/action_utils.py` & `py-sc-kpm-0.1.2/src/sc_kpm/utils/action_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,16 +144,18 @@
         if trg != reaction_node:
             return ScResult.SKIP
         finish_event.set()
         return ScResult.OK
 
     event_params = ScEventParams(question_node, ScEventType.ADD_INGOING_EDGE, event_callback)
     sc_event = events_create(event_params)[0]
-    finish_event.wait(seconds)  # TODO: return status in 0.2.0
+    if not check_edge(sc_types.EDGE_ACCESS_VAR_POS_PERM, reaction_node, question_node):
+        finish_event.wait(seconds)
     events_destroy(sc_event)
+    # TODO: return status in 0.2.0
 
 
 def finish_action(action_node: ScAddr, status: Idtf = QuestionStatus.QUESTION_FINISHED) -> ScAddr:
     return create_edge(sc_types.EDGE_ACCESS_CONST_POS_PERM, ScKeynodes[status], action_node)
 
 
 def finish_action_with_status(action_node: ScAddr, is_success: bool = True) -> None:
```

### Comparing `py-sc-kpm-0.1.1/src/sc_kpm/utils/common_utils.py` & `py-sc-kpm-0.1.2/src/sc_kpm/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `py-sc-kpm-0.1.1/src/sc_kpm/utils/iteration_utils.py` & `py-sc-kpm-0.1.2/src/sc_kpm/utils/iteration_utils.py`

 * *Files identical despite different names*

### Comparing `py-sc-kpm-0.1.1/tests/test_classes.py` & `py-sc-kpm-0.1.2/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `py-sc-kpm-0.1.1/tests/test_keynodes.py` & `py-sc-kpm-0.1.2/tests/test_keynodes.py`

 * *Files identical despite different names*

