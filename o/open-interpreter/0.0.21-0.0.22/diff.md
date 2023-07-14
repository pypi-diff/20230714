# Comparing `tmp/open_interpreter-0.0.21.tar.gz` & `tmp/open_interpreter-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.21.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.22.tar", max compression
```

## Comparing `open_interpreter-0.0.21.tar` & `open_interpreter-0.0.22.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2023-07-14 07:11:47.541275 open_interpreter-0.0.21/LICENSE
--rw-r--r--   0        0        0       81 2023-07-14 07:11:47.541275 open_interpreter-0.0.21/README.md
--rw-r--r--   0        0        0      135 2023-07-14 08:44:08.027686 open_interpreter-0.0.21/interpreter/__init__.py
--rw-r--r--   0        0        0     4546 2023-07-14 07:41:44.774405 open_interpreter-0.0.21/interpreter/exec.py
--rw-r--r--   0        0        0     6241 2023-07-14 08:45:19.160956 open_interpreter-0.0.21/interpreter/interpreter.py
--rw-r--r--   0        0        0     2735 2023-07-14 07:41:45.322446 open_interpreter-0.0.21/interpreter/json_utils.py
--rw-r--r--   0        0        0     3810 2023-07-14 07:24:41.161431 open_interpreter-0.0.21/interpreter/openai_utils.py
--rw-r--r--   0        0        0     3322 2023-07-14 07:41:46.414527 open_interpreter-0.0.21/interpreter/view.py
--rw-r--r--   0        0        0      489 2023-07-14 08:46:35.930643 open_interpreter-0.0.21/pyproject.toml
--rw-r--r--   0        0        0      665 1970-01-01 00:00:00.000000 open_interpreter-0.0.21/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.22/LICENSE
+-rw-r--r--   0        0        0      246 2023-07-14 08:56:06.552917 open_interpreter-0.0.22/README.md
+-rw-r--r--   0        0        0      135 2023-07-14 08:44:08.027686 open_interpreter-0.0.22/interpreter/__init__.py
+-rw-r--r--   0        0        0     4723 2023-07-14 17:03:06.697651 open_interpreter-0.0.22/interpreter/exec.py
+-rw-r--r--   0        0        0     6241 2023-07-14 08:45:19.160956 open_interpreter-0.0.22/interpreter/interpreter.py
+-rw-r--r--   0        0        0     2735 2023-07-14 07:41:45.322446 open_interpreter-0.0.22/interpreter/json_utils.py
+-rw-r--r--   0        0        0     3810 2023-07-14 07:24:41.161431 open_interpreter-0.0.22/interpreter/openai_utils.py
+-rw-r--r--   0        0        0     3322 2023-07-14 07:41:46.414527 open_interpreter-0.0.22/interpreter/view.py
+-rw-r--r--   0        0        0      489 2023-07-14 17:03:58.962526 open_interpreter-0.0.22/pyproject.toml
+-rw-r--r--   0        0        0      830 1970-01-01 00:00:00.000000 open_interpreter-0.0.22/PKG-INFO
```

### Comparing `open_interpreter-0.0.21/LICENSE` & `open_interpreter-0.0.22/LICENSE`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 killian
+Copyright (c) 2023 Killian Lucas
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `open_interpreter-0.0.21/interpreter/exec.py` & `open_interpreter-0.0.22/interpreter/exec.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,19 @@
         self.data = ""
 
     def write(self, data):
         self.data += data
 
         # Clean ANSI color codes
         self.data = re.sub(r'\x1b\[[0-9;]*m', '', self.data)
-
+      
+        # Clean ANSI escape sequences
+        ansi_escape = re.compile(r'\x1B(?:[@-Z\\-_]|\[[0-?]*[ -/]*[@-~])')
+        self.data = ansi_escape.sub('', self.data)
+      
         panel = Panel(self.data.strip(), box=MINIMAL, style="#FFFFFF on #3b3b37")
         self.live.update(panel, refresh=True)
 
     def flush(self):
         pass
 
 def exec_and_capture_output(code):
```

### Comparing `open_interpreter-0.0.21/interpreter/interpreter.py` & `open_interpreter-0.0.22/interpreter/interpreter.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.21/interpreter/json_utils.py` & `open_interpreter-0.0.22/interpreter/json_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.21/interpreter/openai_utils.py` & `open_interpreter-0.0.22/interpreter/openai_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.21/interpreter/view.py` & `open_interpreter-0.0.22/interpreter/view.py`

 * *Files identical despite different names*

