# Comparing `tmp/pycones-0.1.4.tar.gz` & `tmp/pycones-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycones-0.1.4.tar", max compression
+gzip compressed data, was "pycones-0.1.5.tar", max compression
```

## Comparing `pycones-0.1.4.tar` & `pycones-0.1.5.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      479 2023-07-14 08:32:36.973848 pycones-0.1.4/README.md
--rw-r--r--   0        0        0     1875 2023-07-14 08:50:40.913668 pycones-0.1.4/pycones/__init__.py
--rw-r--r--   0        0        0      676 2023-07-14 08:50:40.913668 pycones-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1098 1970-01-01 00:00:00.000000 pycones-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      479 2023-07-14 08:32:36.973848 pycones-0.1.5/README.md
+-rw-r--r--   0        0        0     1880 2023-07-14 08:54:30.503629 pycones-0.1.5/pycones/__init__.py
+-rw-r--r--   0        0        0      676 2023-07-14 08:54:30.503629 pycones-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1098 1970-01-01 00:00:00.000000 pycones-0.1.5/PKG-INFO
```

### Comparing `pycones-0.1.4/pycones/__init__.py` & `pycones-0.1.5/pycones/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 The pycones package provides useful functions
 """
 import json
 
-__version__ = "0.1.4"
+__version__ = "0.1.5"
 
 
 def flatten(lst):
     """
     flatten a list
     """
     result = []
@@ -23,15 +23,15 @@
     """
     join lists into a string
     """
     res = sep.join(flatten(args))
     return res
 
 
-def nb_kernel_switch(notebook_path, kernel="python"):
+def nb_kernel_switch(notebook_path, out_path, kernel="python"):
     """
     switch jupyter kernel into python or r
     """
     assert notebook_path.endswith(".ipynb"), "please input a .ipynb file"
     kernel = kernel.lower()
     assert kernel in ["python", "r"], "please switch to python or r kernel"
 
@@ -56,9 +56,9 @@
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
         }
 
-    with open(notebook_path, 'w') as f:
+    with open(out_path, 'w') as f:
         json.dump(notebook, f)
```

### Comparing `pycones-0.1.4/pyproject.toml` & `pycones-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pycones"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["william <william_swl@163.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.6"
 matplotlib = ">=3.0"
@@ -16,15 +16,15 @@
 tox = "^4.6.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.bumpver]
-current_version = "0.1.4"
+current_version = "0.1.5"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
     'version = "{version}"',
 ]
```

### Comparing `pycones-0.1.4/PKG-INFO` & `pycones-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycones
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: william
 Author-email: william_swl@163.com
 Requires-Python: >=3.6
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

