# Comparing `tmp/open_interpreter-0.0.1.tar.gz` & `tmp/open_interpreter-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.1.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.2.tar", max compression
```

## Comparing `open_interpreter-0.0.1.tar` & `open_interpreter-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2023-07-14 07:11:47.541275 open_interpreter-0.0.1/LICENSE
--rw-r--r--   0        0        0       81 2023-07-14 07:11:47.541275 open_interpreter-0.0.1/README.md
--rw-r--r--   0        0        0      373 2023-07-14 07:41:43.650322 open_interpreter-0.0.1/interpreter/__init__.py
--rw-r--r--   0        0        0     4546 2023-07-14 07:41:44.774405 open_interpreter-0.0.1/interpreter/exec.py
--rw-r--r--   0        0        0     6255 2023-07-14 07:41:44.186362 open_interpreter-0.0.1/interpreter/interpreter.py
--rw-r--r--   0        0        0     2735 2023-07-14 07:41:45.322446 open_interpreter-0.0.1/interpreter/json_utils.py
--rw-r--r--   0        0        0     3810 2023-07-14 07:24:41.161431 open_interpreter-0.0.1/interpreter/openai_utils.py
--rw-r--r--   0        0        0     3322 2023-07-14 07:41:46.414527 open_interpreter-0.0.1/interpreter/view.py
--rw-r--r--   0        0        0      488 2023-07-14 08:00:29.113690 open_interpreter-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      664 1970-01-01 00:00:00.000000 open_interpreter-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-14 07:11:47.541275 open_interpreter-0.0.2/LICENSE
+-rw-r--r--   0        0        0       81 2023-07-14 07:11:47.541275 open_interpreter-0.0.2/README.md
+-rw-r--r--   0        0        0      524 2023-07-14 08:09:42.222661 open_interpreter-0.0.2/interpreter/__init__.py
+-rw-r--r--   0        0        0     4546 2023-07-14 07:41:44.774405 open_interpreter-0.0.2/interpreter/exec.py
+-rw-r--r--   0        0        0     6255 2023-07-14 07:41:44.186362 open_interpreter-0.0.2/interpreter/interpreter.py
+-rw-r--r--   0        0        0     2735 2023-07-14 07:41:45.322446 open_interpreter-0.0.2/interpreter/json_utils.py
+-rw-r--r--   0        0        0     3810 2023-07-14 07:24:41.161431 open_interpreter-0.0.2/interpreter/openai_utils.py
+-rw-r--r--   0        0        0     3322 2023-07-14 07:41:46.414527 open_interpreter-0.0.2/interpreter/view.py
+-rw-r--r--   0        0        0      488 2023-07-14 08:10:33.658471 open_interpreter-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      664 1970-01-01 00:00:00.000000 open_interpreter-0.0.2/PKG-INFO
```

### Comparing `open_interpreter-0.0.1/LICENSE` & `open_interpreter-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.1/interpreter/exec.py` & `open_interpreter-0.0.2/interpreter/exec.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.1/interpreter/interpreter.py` & `open_interpreter-0.0.2/interpreter/interpreter.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.1/interpreter/json_utils.py` & `open_interpreter-0.0.2/interpreter/json_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.1/interpreter/openai_utils.py` & `open_interpreter-0.0.2/interpreter/openai_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.1/interpreter/view.py` & `open_interpreter-0.0.2/interpreter/view.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.1/PKG-INFO` & `open_interpreter-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.1
+Version: 0.0.2
 Summary: Ask GPT-4 to run code locally
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

