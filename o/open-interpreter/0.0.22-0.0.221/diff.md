# Comparing `tmp/open_interpreter-0.0.22.tar.gz` & `tmp/open_interpreter-0.0.221.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.22.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.221.tar", max compression
```

## Comparing `open_interpreter-0.0.22.tar` & `open_interpreter-0.0.221.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.22/LICENSE
--rw-r--r--   0        0        0      246 2023-07-14 08:56:06.552917 open_interpreter-0.0.22/README.md
--rw-r--r--   0        0        0      135 2023-07-14 08:44:08.027686 open_interpreter-0.0.22/interpreter/__init__.py
--rw-r--r--   0        0        0     4723 2023-07-14 17:03:06.697651 open_interpreter-0.0.22/interpreter/exec.py
--rw-r--r--   0        0        0     6241 2023-07-14 08:45:19.160956 open_interpreter-0.0.22/interpreter/interpreter.py
--rw-r--r--   0        0        0     2735 2023-07-14 07:41:45.322446 open_interpreter-0.0.22/interpreter/json_utils.py
--rw-r--r--   0        0        0     3810 2023-07-14 07:24:41.161431 open_interpreter-0.0.22/interpreter/openai_utils.py
--rw-r--r--   0        0        0     3322 2023-07-14 07:41:46.414527 open_interpreter-0.0.22/interpreter/view.py
--rw-r--r--   0        0        0      489 2023-07-14 17:03:58.962526 open_interpreter-0.0.22/pyproject.toml
--rw-r--r--   0        0        0      830 1970-01-01 00:00:00.000000 open_interpreter-0.0.22/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.221/LICENSE
+-rw-r--r--   0        0        0      246 2023-07-14 08:56:06.552917 open_interpreter-0.0.221/README.md
+-rw-r--r--   0        0        0      135 2023-07-14 08:44:08.027686 open_interpreter-0.0.221/interpreter/__init__.py
+-rw-r--r--   0        0        0     5239 2023-07-14 17:35:57.437462 open_interpreter-0.0.221/interpreter/exec.py
+-rw-r--r--   0        0        0     6241 2023-07-14 08:45:19.160956 open_interpreter-0.0.221/interpreter/interpreter.py
+-rw-r--r--   0        0        0     2735 2023-07-14 07:41:45.322446 open_interpreter-0.0.221/interpreter/json_utils.py
+-rw-r--r--   0        0        0     3810 2023-07-14 07:24:41.161431 open_interpreter-0.0.221/interpreter/openai_utils.py
+-rw-r--r--   0        0        0     3322 2023-07-14 07:41:46.414527 open_interpreter-0.0.221/interpreter/view.py
+-rw-r--r--   0        0        0      490 2023-07-14 17:36:30.520548 open_interpreter-0.0.221/pyproject.toml
+-rw-r--r--   0        0        0      831 1970-01-01 00:00:00.000000 open_interpreter-0.0.221/PKG-INFO
```

### Comparing `open_interpreter-0.0.22/LICENSE` & `open_interpreter-0.0.221/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.22/interpreter/exec.py` & `open_interpreter-0.0.221/interpreter/exec.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,29 @@
 def check_for_syntax_errors(code):
     # Needs to happen before we execute.
     lines = code.split('\n')
     filtered_lines = [line for line in lines if not re.match(r'^[!%]', line.strip())]
     cleaned_code = '\n'.join(filtered_lines)
     compile(cleaned_code, '<string>', 'exec')
 
+
+def truncate_output(data):
+    max_length = 7000
+    message = f'Output truncated. Showing the last {max_length} characters:\n\n'
+
+    # Remove previous truncation message if it exists
+    if data.startswith(message):
+        data = data[len(message):]
+
+    # If data exceeds max length, truncate it and add message
+    if len(data) > max_length:
+        data = message + data[-max_length:]
+    return data
+  
+
 class RichOutStream:
 
     def __init__(self, live):
         self.live = live
         self.data = ""
 
     def write(self, data):
@@ -31,15 +46,18 @@
 
         # Clean ANSI color codes
         self.data = re.sub(r'\x1b\[[0-9;]*m', '', self.data)
       
         # Clean ANSI escape sequences
         ansi_escape = re.compile(r'\x1B(?:[@-Z\\-_]|\[[0-?]*[ -/]*[@-~])')
         self.data = ansi_escape.sub('', self.data)
-      
+
+        # Truncate and prepend a message if truncated
+        self.data = truncate_output(self.data)
+        
         panel = Panel(self.data.strip(), box=MINIMAL, style="#FFFFFF on #3b3b37")
         self.live.update(panel, refresh=True)
 
     def flush(self):
         pass
 
 def exec_and_capture_output(code):
```

### Comparing `open_interpreter-0.0.22/interpreter/interpreter.py` & `open_interpreter-0.0.221/interpreter/interpreter.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.22/interpreter/json_utils.py` & `open_interpreter-0.0.221/interpreter/json_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.22/interpreter/openai_utils.py` & `open_interpreter-0.0.221/interpreter/openai_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.22/interpreter/view.py` & `open_interpreter-0.0.221/interpreter/view.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.22/PKG-INFO` & `open_interpreter-0.0.221/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.22
+Version: 0.0.221
 Summary: Ask GPT-4 to run code locally
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

