# Comparing `tmp/open_interpreter-0.0.2.tar.gz` & `tmp/open_interpreter-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.2.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.21.tar", max compression
```

## Comparing `open_interpreter-0.0.2.tar` & `open_interpreter-0.0.21.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2023-07-14 07:11:47.541275 open_interpreter-0.0.2/LICENSE
--rw-r--r--   0        0        0       81 2023-07-14 07:11:47.541275 open_interpreter-0.0.2/README.md
--rw-r--r--   0        0        0      524 2023-07-14 08:09:42.222661 open_interpreter-0.0.2/interpreter/__init__.py
--rw-r--r--   0        0        0     4546 2023-07-14 07:41:44.774405 open_interpreter-0.0.2/interpreter/exec.py
--rw-r--r--   0        0        0     6255 2023-07-14 07:41:44.186362 open_interpreter-0.0.2/interpreter/interpreter.py
--rw-r--r--   0        0        0     2735 2023-07-14 07:41:45.322446 open_interpreter-0.0.2/interpreter/json_utils.py
--rw-r--r--   0        0        0     3810 2023-07-14 07:24:41.161431 open_interpreter-0.0.2/interpreter/openai_utils.py
--rw-r--r--   0        0        0     3322 2023-07-14 07:41:46.414527 open_interpreter-0.0.2/interpreter/view.py
--rw-r--r--   0        0        0      488 2023-07-14 08:10:33.658471 open_interpreter-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      664 1970-01-01 00:00:00.000000 open_interpreter-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-14 07:11:47.541275 open_interpreter-0.0.21/LICENSE
+-rw-r--r--   0        0        0       81 2023-07-14 07:11:47.541275 open_interpreter-0.0.21/README.md
+-rw-r--r--   0        0        0      135 2023-07-14 08:44:08.027686 open_interpreter-0.0.21/interpreter/__init__.py
+-rw-r--r--   0        0        0     4546 2023-07-14 07:41:44.774405 open_interpreter-0.0.21/interpreter/exec.py
+-rw-r--r--   0        0        0     6241 2023-07-14 08:45:19.160956 open_interpreter-0.0.21/interpreter/interpreter.py
+-rw-r--r--   0        0        0     2735 2023-07-14 07:41:45.322446 open_interpreter-0.0.21/interpreter/json_utils.py
+-rw-r--r--   0        0        0     3810 2023-07-14 07:24:41.161431 open_interpreter-0.0.21/interpreter/openai_utils.py
+-rw-r--r--   0        0        0     3322 2023-07-14 07:41:46.414527 open_interpreter-0.0.21/interpreter/view.py
+-rw-r--r--   0        0        0      489 2023-07-14 08:46:35.930643 open_interpreter-0.0.21/pyproject.toml
+-rw-r--r--   0        0        0      665 1970-01-01 00:00:00.000000 open_interpreter-0.0.21/PKG-INFO
```

### Comparing `open_interpreter-0.0.2/LICENSE` & `open_interpreter-0.0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.2/interpreter/exec.py` & `open_interpreter-0.0.21/interpreter/exec.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.2/interpreter/interpreter.py` & `open_interpreter-0.0.21/interpreter/interpreter.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 """.strip()
 
 class Interpreter:
     def __init__(self):
         self.messages = []
         self._logs = []
         self.system_message = system_message
-        self.openai_api_key = None
+        self.api_key = None
 
     def reset(self):
         self.messages = []
         self._logs = []
 
     def load(self, messages):
         self.messages = messages
@@ -88,15 +88,15 @@
             # make openai call
             gpt_functions = [{k: v for k, v in d.items() if k != 'function'} for d in functions]
             response = openai_streaming_response(
                 self.messages,
                 gpt_functions,
                 self.system_message,
                 "gpt-4-0613",
-                self.openai_api_key
+                self.api_key
             )
 
             base_event = {
                 "role": "assistant",
                 "content": ""
             }
             event = base_event
```

### Comparing `open_interpreter-0.0.2/interpreter/json_utils.py` & `open_interpreter-0.0.21/interpreter/json_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.2/interpreter/openai_utils.py` & `open_interpreter-0.0.21/interpreter/openai_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.2/interpreter/view.py` & `open_interpreter-0.0.21/interpreter/view.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.2/PKG-INFO` & `open_interpreter-0.0.21/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.2
+Version: 0.0.21
 Summary: Ask GPT-4 to run code locally
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

