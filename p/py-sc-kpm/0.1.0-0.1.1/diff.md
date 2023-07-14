# Comparing `tmp/py-sc-kpm-0.1.0.tar.gz` & `tmp/py-sc-kpm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-sc-kpm-0.1.0.tar", last modified: Sat May 13 08:47:06 2023, max compression
+gzip compressed data, was "py-sc-kpm-0.1.1.tar", last modified: Fri Jul 14 11:12:34 2023, max compression
```

## Comparing `py-sc-kpm-0.1.0.tar` & `py-sc-kpm-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 08:47:06.073975 py-sc-kpm-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-13 08:46:53.000000 py-sc-kpm-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25873 2023-05-13 08:47:06.073975 py-sc-kpm-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25014 2023-05-13 08:46:53.000000 py-sc-kpm-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-13 08:47:06.073975 py-sc-kpm-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-13 08:46:53.000000 py-sc-kpm-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 08:47:06.069975 py-sc-kpm-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 08:47:06.069975 py-sc-kpm-0.1.0/src/py_sc_kpm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25873 2023-05-13 08:47:06.000000 py-sc-kpm-0.1.0/src/py_sc_kpm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-13 08:47:06.000000 py-sc-kpm-0.1.0/src/py_sc_kpm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 08:47:06.000000 py-sc-kpm-0.1.0/src/py_sc_kpm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-13 08:47:06.000000 py-sc-kpm-0.1.0/src/py_sc_kpm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-13 08:47:06.000000 py-sc-kpm-0.1.0/src/py_sc_kpm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 08:47:06.069975 py-sc-kpm-0.1.0/src/sc_kpm/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-13 08:46:53.000000 py-sc-kpm-0.1.0/src/sc_kpm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-13 08:46:53.000000 py-sc-kpm-0.1.0/src/sc_kpm/identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-13 08:46:53.000000 py-sc-kpm-0.1.0/src/sc_kpm/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-05-13 08:46:53.000000 py-sc-kpm-0.1.0/src/sc_kpm/sc_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-13 08:46:53.000000 py-sc-kpm-0.1.0/src/sc_kpm/sc_keynodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-13 08:46:53.000000 py-sc-kpm-0.1.0/src/sc_kpm/sc_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-13 08:46:53.000000 py-sc-kpm-0.1.0/src/sc_kpm/sc_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-05-13 08:46:53.000000 py-sc-kpm-0.1.0/src/sc_kpm/sc_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 08:47:06.069975 py-sc-kpm-0.1.0/src/sc_kpm/sc_sets/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-13 08:46:53.000000 py-sc-kpm-0.1.0/src/sc_kpm/sc_sets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-13 08:46:53.000000 py-sc-kpm-0.1.0/src/sc_kpm/sc_sets/sc_numbered_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-05-13 08:46:53.000000 py-sc-kpm-0.1.0/src/sc_kpm/sc_sets/sc_oriented_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-05-13 08:46:53.000000 py-sc-kpm-0.1.0/src/sc_kpm/sc_sets/sc_set.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-13 08:46:53.000000 py-sc-kpm-0.1.0/src/sc_kpm/sc_sets/sc_structure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 08:47:06.073975 py-sc-kpm-0.1.0/src/sc_kpm/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-13 08:46:53.000000 py-sc-kpm-0.1.0/src/sc_kpm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-05-13 08:46:53.000000 py-sc-kpm-0.1.0/src/sc_kpm/utils/action_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-05-13 08:46:53.000000 py-sc-kpm-0.1.0/src/sc_kpm/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-13 08:46:53.000000 py-sc-kpm-0.1.0/src/sc_kpm/utils/iteration_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 08:47:06.073975 py-sc-kpm-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-05-13 08:46:53.000000 py-sc-kpm-0.1.0/tests/test_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-13 08:46:53.000000 py-sc-kpm-0.1.0/tests/test_keynodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:12:34.857563 py-sc-kpm-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    27598 2023-07-14 11:12:34.857563 py-sc-kpm-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26739 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-14 11:12:34.857563 py-sc-kpm-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:12:34.853563 py-sc-kpm-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:12:34.853563 py-sc-kpm-0.1.1/src/py_sc_kpm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27598 2023-07-14 11:12:34.000000 py-sc-kpm-0.1.1/src/py_sc_kpm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-14 11:12:34.000000 py-sc-kpm-0.1.1/src/py_sc_kpm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 11:12:34.000000 py-sc-kpm-0.1.1/src/py_sc_kpm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-14 11:12:34.000000 py-sc-kpm-0.1.1/src/py_sc_kpm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 11:12:34.000000 py-sc-kpm-0.1.1/src/py_sc_kpm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:12:34.857563 py-sc-kpm-0.1.1/src/sc_kpm/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/src/sc_kpm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/src/sc_kpm/identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/src/sc_kpm/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/src/sc_kpm/sc_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/src/sc_kpm/sc_keynodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/src/sc_kpm/sc_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/src/sc_kpm/sc_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/src/sc_kpm/sc_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:12:34.857563 py-sc-kpm-0.1.1/src/sc_kpm/sc_sets/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/src/sc_kpm/sc_sets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/src/sc_kpm/sc_sets/sc_numbered_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/src/sc_kpm/sc_sets/sc_oriented_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/src/sc_kpm/sc_sets/sc_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/src/sc_kpm/sc_sets/sc_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:12:34.857563 py-sc-kpm-0.1.1/src/sc_kpm/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/src/sc_kpm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/src/sc_kpm/utils/action_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/src/sc_kpm/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/src/sc_kpm/utils/iteration_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:12:34.857563 py-sc-kpm-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/tests/test_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-14 11:12:20.000000 py-sc-kpm-0.1.1/tests/test_keynodes.py
```

### Comparing `py-sc-kpm-0.1.0/LICENSE` & `py-sc-kpm-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py-sc-kpm-0.1.0/PKG-INFO` & `py-sc-kpm-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: py-sc-kpm
-Version: 0.1.0
-Summary: The Python implementation of the knowledge processing module for knowledge manipulations
-Home-page: https://github.com/ostis-ai/py-sc-kpm
-Author: ostis-ai
-License: MIT
-Project-URL: Bug Reports, https://github.com/ostis-ai/py-sc-kpm/issues
-Project-URL: Source, https://github.com/ostis-ai/py-sc-kpm
-Keywords: sc-kpm,kpm,knowledge processing
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8, <4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # py-sc-kpm
 
 The python implementation of the knowledge processing machine (kpm)
 for [sc-machine](https://github.com/ostis-ai/sc-machine).
 Library provides tools for interacting with knowledge bases.
 Communication with server is implemented in separate library
 named [py-sc-client](https://github.com/ostis-ai/py-sc-client).
@@ -752,17 +731,18 @@
         arguments: Dict[ScAddr, IsDynamic],
         concepts: List[Idtf],
         initiation: Idtf = QuestionStatus.QUESTION_INITIATED,
 ) -> ScAddr: ...
 ```
 
 Agent wait function: Waits for creation of edge to reaction node for some seconds.
+Default reaction_node is `question_finished`.
 
 ```python
-def wait_agent(seconds: float, question_node: ScAddr, reaction_node: ScAddr) -> None: ...
+def wait_agent(seconds: float, question_node: ScAddr, reaction_node: ScAddr = None) -> None: ...
 ```
 
 Agent execute function: combines two previous functions -- calls, waits and returns question node and **True** if success
 
 ```python
 def execute_agent(
         arguments: Dict[ScAddr, IsDynamic],
@@ -793,14 +773,71 @@
 
 question = call_agent(**kwargs)  # ScAddr(...)
 wait_agent(3, question, ScKeynodes[QuestionStatus.QUESTION_FINISHED])
 # or
 question, is_successfully = execute_agent(**kwargs, wait_time=3)  # ScAddr(...), bool
 ```
 
+### Create, call and execute action
+
+Functions that allow to create action and add arguments and call later.
+
+Function that creates action with concepts and return its ScAddr.
+
+```python
+def create_action(*concepts: Idtf) -> ScAddr: ...
+```
+
+Function that creates arguments of action
+
+```python
+def add_action_arguments(action_node: ScAddr, arguments: Dict[ScAddr, IsDynamic]) -> None: ...
+```
+
+Now you can call or execute action.
+Action call functions don't return action_node because it's parameter to them.
+
+```python
+def call_action(
+        action_node: ScAddr, initiation: Idtf = QuestionStatus.QUESTION_INITIATED
+) -> None: ...
+```
+
+```python
+def execute_action(
+        action_node: ScAddr,
+        initiation: Idtf = QuestionStatus.QUESTION_INITIATED,
+        reaction: Idtf = QuestionStatus.QUESTION_FINISHED_SUCCESSFULLY,
+        wait_time: float = COMMON_WAIT_TIME,
+) -> bool: ...
+```
+
+Example:
+
+```python
+from sc_client.models import ScLinkContentType
+from sc_kpm import ScKeynodes
+from sc_kpm.identifiers import CommonIdentifiers, QuestionStatus
+from sc_kpm.utils import create_link
+from sc_kpm.utils.action_utils import add_action_arguments, call_action, create_action, execute_action, wait_agent
+
+arg1 = create_link(2, ScLinkContentType.INT)
+arg2 = create_link(3, ScLinkContentType.INT)
+
+action_node = create_action(CommonIdentifiers.QUESTION, "some_class_name")  # ScAddr(...)
+# Do something here
+arguments = {arg1: False, arg2: False}
+
+add_action_arguments(action_node, arguments)
+call_action(action_node)
+wait_agent(3, action_node, ScKeynodes[QuestionStatus.QUESTION_FINISHED])
+# or
+is_successful = execute_action(action_node, wait_time=3)  # bool
+```
+
 ### Finish action
 
 Function `finish_action` connects status class to action node:
 
 ```python
 def finish_action(action_node: ScAddr, status: Idtf = QuestionStatus.QUESTION_FINISHED) -> ScAddr: ...
 ```
```

### Comparing `py-sc-kpm-0.1.0/README.md` & `py-sc-kpm-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: py-sc-kpm
+Version: 0.1.1
+Summary: The Python implementation of the knowledge processing module for knowledge manipulations
+Home-page: https://github.com/ostis-ai/py-sc-kpm
+Author: ostis-ai
+License: MIT
+Project-URL: Bug Reports, https://github.com/ostis-ai/py-sc-kpm/issues
+Project-URL: Source, https://github.com/ostis-ai/py-sc-kpm
+Keywords: sc-kpm,kpm,knowledge processing
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8, <4
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # py-sc-kpm
 
 The python implementation of the knowledge processing machine (kpm)
 for [sc-machine](https://github.com/ostis-ai/sc-machine).
 Library provides tools for interacting with knowledge bases.
 Communication with server is implemented in separate library
 named [py-sc-client](https://github.com/ostis-ai/py-sc-client).
@@ -731,17 +752,18 @@
         arguments: Dict[ScAddr, IsDynamic],
         concepts: List[Idtf],
         initiation: Idtf = QuestionStatus.QUESTION_INITIATED,
 ) -> ScAddr: ...
 ```
 
 Agent wait function: Waits for creation of edge to reaction node for some seconds.
+Default reaction_node is `question_finished`.
 
 ```python
-def wait_agent(seconds: float, question_node: ScAddr, reaction_node: ScAddr) -> None: ...
+def wait_agent(seconds: float, question_node: ScAddr, reaction_node: ScAddr = None) -> None: ...
 ```
 
 Agent execute function: combines two previous functions -- calls, waits and returns question node and **True** if success
 
 ```python
 def execute_agent(
         arguments: Dict[ScAddr, IsDynamic],
@@ -772,14 +794,71 @@
 
 question = call_agent(**kwargs)  # ScAddr(...)
 wait_agent(3, question, ScKeynodes[QuestionStatus.QUESTION_FINISHED])
 # or
 question, is_successfully = execute_agent(**kwargs, wait_time=3)  # ScAddr(...), bool
 ```
 
+### Create, call and execute action
+
+Functions that allow to create action and add arguments and call later.
+
+Function that creates action with concepts and return its ScAddr.
+
+```python
+def create_action(*concepts: Idtf) -> ScAddr: ...
+```
+
+Function that creates arguments of action
+
+```python
+def add_action_arguments(action_node: ScAddr, arguments: Dict[ScAddr, IsDynamic]) -> None: ...
+```
+
+Now you can call or execute action.
+Action call functions don't return action_node because it's parameter to them.
+
+```python
+def call_action(
+        action_node: ScAddr, initiation: Idtf = QuestionStatus.QUESTION_INITIATED
+) -> None: ...
+```
+
+```python
+def execute_action(
+        action_node: ScAddr,
+        initiation: Idtf = QuestionStatus.QUESTION_INITIATED,
+        reaction: Idtf = QuestionStatus.QUESTION_FINISHED_SUCCESSFULLY,
+        wait_time: float = COMMON_WAIT_TIME,
+) -> bool: ...
+```
+
+Example:
+
+```python
+from sc_client.models import ScLinkContentType
+from sc_kpm import ScKeynodes
+from sc_kpm.identifiers import CommonIdentifiers, QuestionStatus
+from sc_kpm.utils import create_link
+from sc_kpm.utils.action_utils import add_action_arguments, call_action, create_action, execute_action, wait_agent
+
+arg1 = create_link(2, ScLinkContentType.INT)
+arg2 = create_link(3, ScLinkContentType.INT)
+
+action_node = create_action(CommonIdentifiers.QUESTION, "some_class_name")  # ScAddr(...)
+# Do something here
+arguments = {arg1: False, arg2: False}
+
+add_action_arguments(action_node, arguments)
+call_action(action_node)
+wait_agent(3, action_node, ScKeynodes[QuestionStatus.QUESTION_FINISHED])
+# or
+is_successful = execute_action(action_node, wait_time=3)  # bool
+```
+
 ### Finish action
 
 Function `finish_action` connects status class to action node:
 
 ```python
 def finish_action(action_node: ScAddr, status: Idtf = QuestionStatus.QUESTION_FINISHED) -> ScAddr: ...
 ```
```

### Comparing `py-sc-kpm-0.1.0/setup.py` & `py-sc-kpm-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 DIRECTORY_PATH = Path(__file__).parent
 README = (DIRECTORY_PATH / "README.md").read_text()
 
-VERSION = "0.1.0"
+VERSION = "0.1.1"
 INSTALL_REQUIRES = ["py-sc-client>=0.2.6"]
 CURRENT_PYTHON = sys.version_info[:2]
 REQUIRED_PYTHON = (3, 8)
 
 
 if CURRENT_PYTHON < REQUIRED_PYTHON:
     sys.stderr.write(
```

### Comparing `py-sc-kpm-0.1.0/src/py_sc_kpm.egg-info/PKG-INFO` & `py-sc-kpm-0.1.1/src/py_sc_kpm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-sc-kpm
-Version: 0.1.0
+Version: 0.1.1
 Summary: The Python implementation of the knowledge processing module for knowledge manipulations
 Home-page: https://github.com/ostis-ai/py-sc-kpm
 Author: ostis-ai
 License: MIT
 Project-URL: Bug Reports, https://github.com/ostis-ai/py-sc-kpm/issues
 Project-URL: Source, https://github.com/ostis-ai/py-sc-kpm
 Keywords: sc-kpm,kpm,knowledge processing
@@ -752,17 +752,18 @@
         arguments: Dict[ScAddr, IsDynamic],
         concepts: List[Idtf],
         initiation: Idtf = QuestionStatus.QUESTION_INITIATED,
 ) -> ScAddr: ...
 ```
 
 Agent wait function: Waits for creation of edge to reaction node for some seconds.
+Default reaction_node is `question_finished`.
 
 ```python
-def wait_agent(seconds: float, question_node: ScAddr, reaction_node: ScAddr) -> None: ...
+def wait_agent(seconds: float, question_node: ScAddr, reaction_node: ScAddr = None) -> None: ...
 ```
 
 Agent execute function: combines two previous functions -- calls, waits and returns question node and **True** if success
 
 ```python
 def execute_agent(
         arguments: Dict[ScAddr, IsDynamic],
@@ -793,14 +794,71 @@
 
 question = call_agent(**kwargs)  # ScAddr(...)
 wait_agent(3, question, ScKeynodes[QuestionStatus.QUESTION_FINISHED])
 # or
 question, is_successfully = execute_agent(**kwargs, wait_time=3)  # ScAddr(...), bool
 ```
 
+### Create, call and execute action
+
+Functions that allow to create action and add arguments and call later.
+
+Function that creates action with concepts and return its ScAddr.
+
+```python
+def create_action(*concepts: Idtf) -> ScAddr: ...
+```
+
+Function that creates arguments of action
+
+```python
+def add_action_arguments(action_node: ScAddr, arguments: Dict[ScAddr, IsDynamic]) -> None: ...
+```
+
+Now you can call or execute action.
+Action call functions don't return action_node because it's parameter to them.
+
+```python
+def call_action(
+        action_node: ScAddr, initiation: Idtf = QuestionStatus.QUESTION_INITIATED
+) -> None: ...
+```
+
+```python
+def execute_action(
+        action_node: ScAddr,
+        initiation: Idtf = QuestionStatus.QUESTION_INITIATED,
+        reaction: Idtf = QuestionStatus.QUESTION_FINISHED_SUCCESSFULLY,
+        wait_time: float = COMMON_WAIT_TIME,
+) -> bool: ...
+```
+
+Example:
+
+```python
+from sc_client.models import ScLinkContentType
+from sc_kpm import ScKeynodes
+from sc_kpm.identifiers import CommonIdentifiers, QuestionStatus
+from sc_kpm.utils import create_link
+from sc_kpm.utils.action_utils import add_action_arguments, call_action, create_action, execute_action, wait_agent
+
+arg1 = create_link(2, ScLinkContentType.INT)
+arg2 = create_link(3, ScLinkContentType.INT)
+
+action_node = create_action(CommonIdentifiers.QUESTION, "some_class_name")  # ScAddr(...)
+# Do something here
+arguments = {arg1: False, arg2: False}
+
+add_action_arguments(action_node, arguments)
+call_action(action_node)
+wait_agent(3, action_node, ScKeynodes[QuestionStatus.QUESTION_FINISHED])
+# or
+is_successful = execute_action(action_node, wait_time=3)  # bool
+```
+
 ### Finish action
 
 Function `finish_action` connects status class to action node:
 
 ```python
 def finish_action(action_node: ScAddr, status: Idtf = QuestionStatus.QUESTION_FINISHED) -> ScAddr: ...
 ```
```

### Comparing `py-sc-kpm-0.1.0/src/py_sc_kpm.egg-info/SOURCES.txt` & `py-sc-kpm-0.1.1/src/py_sc_kpm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-sc-kpm-0.1.0/src/sc_kpm/__init__.py` & `py-sc-kpm-0.1.1/src/sc_kpm/__init__.py`

 * *Files identical despite different names*

### Comparing `py-sc-kpm-0.1.0/src/sc_kpm/identifiers.py` & `py-sc-kpm-0.1.1/src/sc_kpm/identifiers.py`

 * *Files identical despite different names*

### Comparing `py-sc-kpm-0.1.0/src/sc_kpm/sc_agent.py` & `py-sc-kpm-0.1.1/src/sc_kpm/sc_agent.py`

 * *Files identical despite different names*

### Comparing `py-sc-kpm-0.1.0/src/sc_kpm/sc_keynodes.py` & `py-sc-kpm-0.1.1/src/sc_kpm/sc_keynodes.py`

 * *Files identical despite different names*

### Comparing `py-sc-kpm-0.1.0/src/sc_kpm/sc_module.py` & `py-sc-kpm-0.1.1/src/sc_kpm/sc_module.py`

 * *Files identical despite different names*

### Comparing `py-sc-kpm-0.1.0/src/sc_kpm/sc_result.py` & `py-sc-kpm-0.1.1/src/sc_kpm/sc_result.py`

 * *Files identical despite different names*

### Comparing `py-sc-kpm-0.1.0/src/sc_kpm/sc_server.py` & `py-sc-kpm-0.1.1/src/sc_kpm/sc_server.py`

 * *Files identical despite different names*

### Comparing `py-sc-kpm-0.1.0/src/sc_kpm/sc_sets/sc_numbered_set.py` & `py-sc-kpm-0.1.1/src/sc_kpm/sc_sets/sc_numbered_set.py`

 * *Files identical despite different names*

### Comparing `py-sc-kpm-0.1.0/src/sc_kpm/sc_sets/sc_oriented_set.py` & `py-sc-kpm-0.1.1/src/sc_kpm/sc_sets/sc_oriented_set.py`

 * *Files identical despite different names*

### Comparing `py-sc-kpm-0.1.0/src/sc_kpm/sc_sets/sc_set.py` & `py-sc-kpm-0.1.1/src/sc_kpm/sc_sets/sc_set.py`

 * *Files identical despite different names*

### Comparing `py-sc-kpm-0.1.0/src/sc_kpm/sc_sets/sc_structure.py` & `py-sc-kpm-0.1.1/src/sc_kpm/sc_sets/sc_structure.py`

 * *Files identical despite different names*

### Comparing `py-sc-kpm-0.1.0/src/sc_kpm/utils/__init__.py` & `py-sc-kpm-0.1.1/src/sc_kpm/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `py-sc-kpm-0.1.0/src/sc_kpm/utils/action_utils.py` & `py-sc-kpm-0.1.1/src/sc_kpm/utils/action_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """
 This source file is part of an OSTIS project. For the latest info, see https://github.com/ostis-ai
 Distributed under the MIT License
 (See an accompanying file LICENSE or a copy at https://opensource.org/licenses/MIT)
 """
 
-import time
-from datetime import datetime, timedelta
+from threading import Event
 from typing import Dict, List, Tuple, Union
 
 from sc_client import client
+from sc_client.client import events_create, events_destroy
 from sc_client.constants import sc_types
-from sc_client.models import ScAddr, ScConstruction, ScTemplate
+from sc_client.constants.common import ScEventType
+from sc_client.models import ScAddr, ScConstruction, ScEventParams, ScTemplate
 
 from sc_kpm.identifiers import CommonIdentifiers, QuestionStatus, ScAlias
 from sc_kpm.sc_keynodes import Idtf, ScKeynodes
+from sc_kpm.sc_result import ScResult
 from sc_kpm.sc_sets.sc_structure import ScStructure
 from sc_kpm.utils.common_utils import (
     check_edge,
     create_edge,
     create_node,
     create_norole_relation,
     create_role_relation,
@@ -70,65 +72,88 @@
     arguments: Dict[ScAddr, IsDynamic],
     concepts: List[Idtf],
     initiation: Idtf = QuestionStatus.QUESTION_INITIATED,
     reaction: Idtf = QuestionStatus.QUESTION_FINISHED_SUCCESSFULLY,
     wait_time: float = COMMON_WAIT_TIME,
 ) -> Tuple[ScAddr, bool]:
     question = call_agent(arguments, concepts, initiation)
-    wait_agent(wait_time, question, ScKeynodes[QuestionStatus.QUESTION_FINISHED])
+    wait_agent(wait_time, question)
     result = check_edge(sc_types.EDGE_ACCESS_VAR_POS_PERM, ScKeynodes[reaction], question)
     return question, result
 
 
 def call_agent(
     arguments: Dict[ScAddr, IsDynamic],
     concepts: List[Idtf],
     initiation: Idtf = QuestionStatus.QUESTION_INITIATED,
 ) -> ScAddr:
-    question = _create_action_with_arguments(arguments, concepts)
-    initiation_node = ScKeynodes.resolve(initiation, sc_types.NODE_CONST_CLASS)
-    create_edge(sc_types.EDGE_ACCESS_CONST_POS_PERM, initiation_node, question)
+    question = create_action(*concepts)
+    add_action_arguments(question, arguments)
+    call_action(question, initiation)
     return question
 
 
-def _create_action_with_arguments(arguments: Dict[ScAddr, IsDynamic], concepts: List[Idtf]) -> ScAddr:
-    action_node = _create_action(concepts)
-    rrel_dynamic_arg = ScKeynodes[CommonIdentifiers.RREL_DYNAMIC_ARGUMENT]
+def create_action(*concepts: Idtf) -> ScAddr:
+    construction = ScConstruction()
+    construction.create_node(sc_types.NODE_CONST, ScAlias.ACTION_NODE)
+    for concept in concepts:
+        construction.create_edge(
+            sc_types.EDGE_ACCESS_CONST_POS_PERM,
+            ScKeynodes.resolve(concept, sc_types.NODE_CONST_CLASS),
+            ScAlias.ACTION_NODE,
+        )
+    action_node = client.create_elements(construction)[0]
+    return action_node
 
+
+def add_action_arguments(action_node: ScAddr, arguments: Dict[ScAddr, IsDynamic]) -> None:
+    rrel_dynamic_arg = ScKeynodes[CommonIdentifiers.RREL_DYNAMIC_ARGUMENT]
     argument: ScAddr
     for index, (argument, is_dynamic) in enumerate(arguments.items(), 1):
         if argument.is_valid():
             rrel_i = ScKeynodes.rrel_index(index)
             if is_dynamic:
                 dynamic_node = create_node(sc_types.NODE_CONST)
                 create_role_relation(action_node, dynamic_node, rrel_dynamic_arg, rrel_i)
                 create_edge(sc_types.EDGE_ACCESS_CONST_POS_TEMP, dynamic_node, argument)
             else:
                 create_role_relation(action_node, argument, rrel_i)
-    return action_node
 
 
-def _create_action(concepts: List[Idtf]) -> ScAddr:
-    construction = ScConstruction()
-    construction.create_node(sc_types.NODE_CONST, ScAlias.ACTION_NODE)
-    for concept in concepts:
-        construction.create_edge(
-            sc_types.EDGE_ACCESS_CONST_POS_PERM,
-            ScKeynodes.resolve(concept, sc_types.NODE_CONST_CLASS),
-            ScAlias.ACTION_NODE,
-        )
-    action_node = client.create_elements(construction)[0]
-    return action_node
+def execute_action(
+    action_node: ScAddr,
+    initiation: Idtf = QuestionStatus.QUESTION_INITIATED,
+    reaction: Idtf = QuestionStatus.QUESTION_FINISHED_SUCCESSFULLY,
+    wait_time: float = COMMON_WAIT_TIME,
+) -> bool:
+    call_action(action_node, initiation)
+    wait_agent(wait_time, action_node)
+    result = check_edge(sc_types.EDGE_ACCESS_VAR_POS_PERM, ScKeynodes[reaction], action_node)
+    return result
+
+
+def call_action(action_node: ScAddr, initiation: Idtf = QuestionStatus.QUESTION_INITIATED) -> None:
+    initiation_node = ScKeynodes.resolve(initiation, sc_types.NODE_CONST_CLASS)
+    create_edge(sc_types.EDGE_ACCESS_CONST_POS_PERM, initiation_node, action_node)
 
 
-# TODO rewrite to event
-def wait_agent(seconds: float, question_node: ScAddr, reaction_node: ScAddr) -> None:
-    finish = datetime.now() + timedelta(seconds=seconds)
-    while not check_edge(sc_types.EDGE_ACCESS_VAR_POS_PERM, reaction_node, question_node) and datetime.now() < finish:
-        time.sleep(0.1)
+def wait_agent(seconds: float, question_node: ScAddr, reaction_node: ScAddr = None) -> None:
+    reaction_node = reaction_node or ScKeynodes[QuestionStatus.QUESTION_FINISHED]
+    finish_event = Event()
+
+    def event_callback(_: ScAddr, __: ScAddr, trg: ScAddr) -> ScResult:
+        if trg != reaction_node:
+            return ScResult.SKIP
+        finish_event.set()
+        return ScResult.OK
+
+    event_params = ScEventParams(question_node, ScEventType.ADD_INGOING_EDGE, event_callback)
+    sc_event = events_create(event_params)[0]
+    finish_event.wait(seconds)  # TODO: return status in 0.2.0
+    events_destroy(sc_event)
 
 
 def finish_action(action_node: ScAddr, status: Idtf = QuestionStatus.QUESTION_FINISHED) -> ScAddr:
     return create_edge(sc_types.EDGE_ACCESS_CONST_POS_PERM, ScKeynodes[status], action_node)
 
 
 def finish_action_with_status(action_node: ScAddr, is_success: bool = True) -> None:
```

### Comparing `py-sc-kpm-0.1.0/src/sc_kpm/utils/common_utils.py` & `py-sc-kpm-0.1.1/src/sc_kpm/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `py-sc-kpm-0.1.0/src/sc_kpm/utils/iteration_utils.py` & `py-sc-kpm-0.1.1/src/sc_kpm/utils/iteration_utils.py`

 * *Files identical despite different names*

### Comparing `py-sc-kpm-0.1.0/tests/test_classes.py` & `py-sc-kpm-0.1.1/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `py-sc-kpm-0.1.0/tests/test_keynodes.py` & `py-sc-kpm-0.1.1/tests/test_keynodes.py`

 * *Files identical despite different names*

