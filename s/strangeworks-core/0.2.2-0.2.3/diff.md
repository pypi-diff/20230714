# Comparing `tmp/strangeworks_core-0.2.2.tar.gz` & `tmp/strangeworks_core-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_core-0.2.2.tar", max compression
+gzip compressed data, was "strangeworks_core-0.2.3.tar", max compression
```

## Comparing `strangeworks_core-0.2.2.tar` & `strangeworks_core-0.2.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      655 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/README.md
--rw-r--r--   0        0        0      914 2023-07-14 18:30:40.408649 strangeworks_core-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      109 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/__init__.py
--rw-r--r--   0        0        0       19 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/batch/__init__.py
--rw-r--r--   0        0        0    12246 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/batch/utils.py
--rw-r--r--   0        0        0       19 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/config/__init__.py
--rw-r--r--   0        0        0      647 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/config/base.py
--rw-r--r--   0        0        0     3340 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/config/config.py
--rw-r--r--   0        0        0      874 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/config/defaults.py
--rw-r--r--   0        0        0     1846 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/config/env.py
--rw-r--r--   0        0        0     6262 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/config/file.py
--rw-r--r--   0        0        0       19 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/errors/__init__.py
--rw-r--r--   0        0        0     2613 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/errors/error.py
--rw-r--r--   0        0        0       19 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/platform/__init__.py
--rw-r--r--   0        0        0     2457 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/platform/auth.py
--rw-r--r--   0        0        0     4880 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/platform/gql.py
--rw-r--r--   0        0        0    10844 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/platform/rest_client.py
--rw-r--r--   0        0        0     3275 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/platform/transport.py
--rw-r--r--   0        0        0       19 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/types/__init__.py
--rw-r--r--   0        0        0     3572 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/types/backend.py
--rw-r--r--   0        0        0     2024 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/types/file.py
--rw-r--r--   0        0        0      647 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/types/func.py
--rw-r--r--   0        0        0     6517 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/types/job.py
--rw-r--r--   0        0        0      760 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/types/machine.py
--rw-r--r--   0        0        0     1088 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/types/product.py
--rw-r--r--   0        0        0     2732 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/types/resource.py
--rw-r--r--   0        0        0      553 2023-07-14 18:30:25.584603 strangeworks_core-0.2.2/strangeworks_core/utils.py
--rw-r--r--   0        0        0     1464 1970-01-01 00:00:00.000000 strangeworks_core-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      655 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/README.md
+-rw-r--r--   0        0        0      914 2023-07-14 19:18:43.994335 strangeworks_core-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      109 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/__init__.py
+-rw-r--r--   0        0        0       19 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/batch/__init__.py
+-rw-r--r--   0        0        0    13255 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/batch/utils.py
+-rw-r--r--   0        0        0       19 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/config/__init__.py
+-rw-r--r--   0        0        0      647 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/config/base.py
+-rw-r--r--   0        0        0     3340 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/config/config.py
+-rw-r--r--   0        0        0      874 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/config/defaults.py
+-rw-r--r--   0        0        0     1846 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/config/env.py
+-rw-r--r--   0        0        0     6262 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/config/file.py
+-rw-r--r--   0        0        0       19 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/errors/__init__.py
+-rw-r--r--   0        0        0     2613 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/errors/error.py
+-rw-r--r--   0        0        0       19 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/platform/__init__.py
+-rw-r--r--   0        0        0     2457 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/platform/auth.py
+-rw-r--r--   0        0        0     4880 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/platform/gql.py
+-rw-r--r--   0        0        0    10844 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/platform/rest_client.py
+-rw-r--r--   0        0        0     3275 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/platform/transport.py
+-rw-r--r--   0        0        0       19 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/types/__init__.py
+-rw-r--r--   0        0        0     3572 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/types/backend.py
+-rw-r--r--   0        0        0     2024 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/types/file.py
+-rw-r--r--   0        0        0      647 2023-07-14 19:18:26.517321 strangeworks_core-0.2.3/strangeworks_core/types/func.py
+-rw-r--r--   0        0        0     6749 2023-07-14 19:18:26.521322 strangeworks_core-0.2.3/strangeworks_core/types/job.py
+-rw-r--r--   0        0        0      760 2023-07-14 19:18:26.521322 strangeworks_core-0.2.3/strangeworks_core/types/machine.py
+-rw-r--r--   0        0        0     1088 2023-07-14 19:18:26.521322 strangeworks_core-0.2.3/strangeworks_core/types/product.py
+-rw-r--r--   0        0        0     2732 2023-07-14 19:18:26.521322 strangeworks_core-0.2.3/strangeworks_core/types/resource.py
+-rw-r--r--   0        0        0      553 2023-07-14 19:18:26.521322 strangeworks_core-0.2.3/strangeworks_core/utils.py
+-rw-r--r--   0        0        0     1464 1970-01-01 00:00:00.000000 strangeworks_core-0.2.3/PKG-INFO
```

### Comparing `strangeworks_core-0.2.2/README.md` & `strangeworks_core-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.2/pyproject.toml` & `strangeworks_core-0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "strangeworks-core"
-version = "0.2.2"
+version = "0.2.3"
 
 description = "Strangeworks Core provides the infrastructure to interact with the platform."
 authors = ["Strange Devs <hello@strangeworks.com>"]
 readme = "README.md"
 packages = [{include = "strangeworks_core"}]
 license = "Apache-2.0"
```

### Comparing `strangeworks_core-0.2.2/strangeworks_core/batch/utils.py` & `strangeworks_core-0.2.3/strangeworks_core/batch/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -255,31 +255,64 @@
 
     return program
 
 
 def _get_imports(file_path: str) -> list[str]:
     """Get a list of the imports in a file.
 
+    Parse imports using ast (https://docs.python.org/3/library/ast.html)
+    in order to properly handle most if not all import cases such as:
+    ```python
+    import module
+    import module as m
+    from module import name
+    from module import name as n
+    from module import (
+        name1,
+        name2,
+        name3,
+        name4 as n4,
+    )
+    ```
+
     Parameters
     ----------
     file_path: str
         The path to the file of the function.
 
     Returns
     -------
     imports: list[str]
         A list of the imports in the file.
     """
-    with open(file_path) as f:
-        lines = f.readlines()
-        return [
-            line.strip()
-            for line in lines
-            if line.startswith("import") or line.startswith("from")
-        ]
+    with open(file_path, "r") as file:
+        tree = ast.parse(file.read())
+
+    imports = []
+    for node in ast.walk(tree):
+        if isinstance(node, ast.Import):
+            imports.extend(
+                [
+                    f"import {name.name}"
+                    if not name.asname
+                    else f"import {name.name} as {name.asname}"
+                    for name in node.names
+                ]
+            )
+        elif isinstance(node, ast.ImportFrom):
+            module = node.module if node.module else ""
+            imports.extend(
+                [
+                    f"from {module} import {alias.name}"
+                    if not alias.asname
+                    else f"from {module} import {alias.name} as {alias.asname}"
+                    for alias in node.names
+                ]
+            )
+    return imports
 
 
 def _get_source(f: Callable[..., Any], decorator_name: str) -> str:
     """Get the source code of a function, removing the decorator.
 
     Parameters
     ----------
```

### Comparing `strangeworks_core-0.2.2/strangeworks_core/config/base.py` & `strangeworks_core-0.2.3/strangeworks_core/config/base.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.2/strangeworks_core/config/config.py` & `strangeworks_core-0.2.3/strangeworks_core/config/config.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.2/strangeworks_core/config/defaults.py` & `strangeworks_core-0.2.3/strangeworks_core/config/defaults.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.2/strangeworks_core/config/env.py` & `strangeworks_core-0.2.3/strangeworks_core/config/env.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.2/strangeworks_core/config/file.py` & `strangeworks_core-0.2.3/strangeworks_core/config/file.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.2/strangeworks_core/errors/error.py` & `strangeworks_core-0.2.3/strangeworks_core/errors/error.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.2/strangeworks_core/platform/auth.py` & `strangeworks_core-0.2.3/strangeworks_core/platform/auth.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.2/strangeworks_core/platform/gql.py` & `strangeworks_core-0.2.3/strangeworks_core/platform/gql.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.2/strangeworks_core/platform/rest_client.py` & `strangeworks_core-0.2.3/strangeworks_core/platform/rest_client.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.2/strangeworks_core/platform/transport.py` & `strangeworks_core-0.2.3/strangeworks_core/platform/transport.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.2/strangeworks_core/types/backend.py` & `strangeworks_core-0.2.3/strangeworks_core/types/backend.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.2/strangeworks_core/types/file.py` & `strangeworks_core-0.2.3/strangeworks_core/types/file.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.2/strangeworks_core/types/func.py` & `strangeworks_core-0.2.3/strangeworks_core/types/func.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.2/strangeworks_core/types/job.py` & `strangeworks_core-0.2.3/strangeworks_core/types/job.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,25 @@
     QUEUED = "QUEUED"
     RUNNING = "RUNNING"
     COMPLETED = "COMPLETED"
     FAILED = "FAILED"
     CANCELLING = "CANCELLING"
     CANCELLED = "CANCELLED"
 
+    @property
+    def is_terminal_state(self):
+        """Check if status is corresponds to a terminal state.
+
+        Returns
+        -------
+        return True if self is in [Status.CANCELLED, Status.COMPLETED, Status.FAILED],
+        False otherwise.
+        """
+        return self in [Status.CANCELLED, Status.COMPLETED, Status.FAILED]
+
 
 class Job:
     """Object representing a Strangeworks platform job entry."""
 
     def __init__(
         self,
         slug: str,
@@ -137,22 +148,21 @@
         """
         return self._is_terminal_state
 
     @property
     def is_terminal_state(self) -> bool:
         """Return if job is in terminal state.
 
-        If _is_terminal_state was set, return that value. Otherwise, return True if
-        self.status is in [Status.CANCELLED, Status.COMPLETED, Status.FAILED],
-        otherwise False.
+        If _is_terminal_state was set, return that value. Otherwise, return
+        self.status.is_terminal_state
         """
         return (
             self._is_terminal_state
             if self._is_terminal_state is not None
-            else self.status in [Status.CANCELLED, Status.COMPLETED, Status.FAILED]
+            else self.status.is_terminal_state
         )
 
 
 class JobFile:
     """Object which represents a Strangeworks platform job file entry."""
 
     def __init__(
```

### Comparing `strangeworks_core-0.2.2/strangeworks_core/types/machine.py` & `strangeworks_core-0.2.3/strangeworks_core/types/machine.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.2/strangeworks_core/types/product.py` & `strangeworks_core-0.2.3/strangeworks_core/types/product.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.2/strangeworks_core/types/resource.py` & `strangeworks_core-0.2.3/strangeworks_core/types/resource.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.2/strangeworks_core/utils.py` & `strangeworks_core-0.2.3/strangeworks_core/utils.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.2/PKG-INFO` & `strangeworks_core-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strangeworks-core
-Version: 0.2.2
+Version: 0.2.3
 Summary: Strangeworks Core provides the infrastructure to interact with the platform.
 License: Apache-2.0
 Author: Strange Devs
 Author-email: hello@strangeworks.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

