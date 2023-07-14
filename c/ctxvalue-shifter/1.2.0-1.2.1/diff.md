# Comparing `tmp/ctxvalue_shifter-1.2.0-py3-none-any.whl.zip` & `tmp/ctxvalue_shifter-1.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 15649 bytes, number of entries: 9
+Zip file size: 16030 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat       53 b- defN 23-Jul-14 10:12 cxvshifter/__init__.py
--rw-rw-rw-  2.0 fat     1413 b- defN 23-Jul-14 10:23 cxvshifter/cxvshifter.py
+-rw-rw-rw-  2.0 fat     2591 b- defN 23-Jul-14 11:00 cxvshifter/cxvshifter.py
 -rw-rw-rw-  2.0 fat       50 b- defN 23-Jul-14 09:32 shifter/__init__.py
 -rw-rw-rw-  2.0 fat     1396 b- defN 23-Jul-14 09:59 shifter/shifter.py
--rw-rw-rw-  2.0 fat    35149 b- defN 23-Jul-14 10:26 ctxvalue_shifter-1.2.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      908 b- defN 23-Jul-14 10:26 ctxvalue_shifter-1.2.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-14 10:26 ctxvalue_shifter-1.2.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Jul-14 10:26 ctxvalue_shifter-1.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      738 b- defN 23-Jul-14 10:26 ctxvalue_shifter-1.2.0.dist-info/RECORD
-9 files, 39810 bytes uncompressed, 14369 bytes compressed:  63.9%
+-rw-rw-rw-  2.0 fat    35149 b- defN 23-Jul-14 11:01 ctxvalue_shifter-1.2.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      908 b- defN 23-Jul-14 11:01 ctxvalue_shifter-1.2.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-14 11:01 ctxvalue_shifter-1.2.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Jul-14 11:01 ctxvalue_shifter-1.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      738 b- defN 23-Jul-14 11:01 ctxvalue_shifter-1.2.1.dist-info/RECORD
+9 files, 40988 bytes uncompressed, 14750 bytes compressed:  64.0%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: shifter/__init__.py
 Comment: 
 
 Filename: shifter/shifter.py
 Comment: 
 
-Filename: ctxvalue_shifter-1.2.0.dist-info/LICENSE
+Filename: ctxvalue_shifter-1.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: ctxvalue_shifter-1.2.0.dist-info/METADATA
+Filename: ctxvalue_shifter-1.2.1.dist-info/METADATA
 Comment: 
 
-Filename: ctxvalue_shifter-1.2.0.dist-info/WHEEL
+Filename: ctxvalue_shifter-1.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: ctxvalue_shifter-1.2.0.dist-info/top_level.txt
+Filename: ctxvalue_shifter-1.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: ctxvalue_shifter-1.2.0.dist-info/RECORD
+Filename: ctxvalue_shifter-1.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cxvshifter/cxvshifter.py

```diff
@@ -1,13 +1,65 @@
 """
 Contextual Value Shifter - A Python module that implements a contextual "shift" function. 
 """
 
+import inspect
 import subprocess
 
+class ContextualActions():
+    """
+    Defines the contextual actions for ctxvalue-shifter.
+    """
+    def __init__(self):
+        warning_msg = """WARNING: This class isn't supposed to be used directly.
+        Use `cxvshifter.shift()`."""
+        caller_module = inspect.getmodule(inspect.currentframe().f_back)
+        module_name = caller_module.__name__ if caller_module else '<unknown>'
+        if module_name != '__main__':
+            print(warning_msg)
+
+    def stdout(self, data):
+        """
+        Prints to stdout.
+
+        Used if `destination` is `'stdout'`.
+        """
+        print(data)
+
+    def exec(self, cmd):
+        """
+        Runs a command.
+
+        Used if `destination` is `'exec'`.
+        """
+        # If cmd isn't str, that probably isn't good
+        if not isinstance(cmd, str):
+            raise TypeError("'exec' specified, but `origin` is not a string.")
+        subprocess.run(cmd, shell=True, check=True)
+
+    def filec(self, data, filename):
+        """
+        Writes a file.
+
+        Used if `destination` is `'file'`.
+        """
+        if filename is None:
+            raise ValueError("Missing 'file' parameter.")
+
+        with open(filename, 'w', encoding="UTF-8") as file:
+            file.write(str(data))
+
+    def assign(self, origin, destination):
+        """
+        Assigns a variable.
+
+        Used if `destination` is not a special value.
+        """
+        globals()[destination] = origin
+
 def shift(origin, destination, filename=None):
     """
     Shifts the value of `origin` to the specified `destination`.
 
     `destination` options:
     - `'stdout'`: Prints `origin` to standard output.
     - `'exec'`: Executes `origin` as a command using subprocess.
@@ -17,34 +69,24 @@
     If `destination` is `'return'`, shift returns `origin`.
 
     Otherwise, shift returns `None`.
     """
 
     # We make sure destination is str, to prevent abuse
     # and to make sure they're doing it right
-    if destination is not str:
+    if not isinstance(destination, str):
         raise TypeError("`destination` is not string.")
 
-    if destination == 'stdout':
-        print(origin)
+    action = ContextualActions()
 
+    if destination == 'stdout':
+        action.stdout(origin)
     elif destination == 'exec':
-        # If origin isn't str, that probably isn't good
-        if origin is not str:
-            raise TypeError("'exec' specified, but `origin` is not a string.")
-
-        subprocess.run(origin, shell=True, check=True)
-
+        action.exec(origin)
     elif destination == 'file':
-        if filename is None:
-            raise ValueError("Missing 'file' parameter.")
-
-        with open(filename, 'w', encoding="UTF-8") as file:
-            file.write(str(origin))
-
+        action.filec(origin, filename)
     elif destination == 'return':
         return origin
-
     else:
-        globals()[destination] = origin
+        action.assign(origin, destination)
 
     return None
```

## Comparing `ctxvalue_shifter-1.2.0.dist-info/LICENSE` & `ctxvalue_shifter-1.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ctxvalue_shifter-1.2.0.dist-info/METADATA` & `ctxvalue_shifter-1.2.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctxvalue-shifter
-Version: 1.2.0
+Version: 1.2.1
 Summary: Contextual Value Shifter, a module for shifting values to different destinations.
 Author: Arsalan Kazmi
 Author-email: sonicspeed848@gmail.com
 Requires-Python: >=3.6
 License-File: LICENSE
 
 Contextual Value Shifter is a Python module that implements a contextual "shift" function.
```

