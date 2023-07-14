# Comparing `tmp/pycones-0.1.2.tar.gz` & `tmp/pycones-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycones-0.1.2.tar", max compression
+gzip compressed data, was "pycones-0.1.3.tar", max compression
```

## Comparing `pycones-0.1.2.tar` & `pycones-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      373 2023-06-24 09:08:37.437746 pycones-0.1.2/README.md
--rw-r--r--   0        0        0      435 2023-06-24 09:07:55.327757 pycones-0.1.2/pycones/__init__.py
--rw-r--r--   0        0        0      676 2023-06-24 09:07:55.327757 pycones-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      992 1970-01-01 00:00:00.000000 pycones-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      479 2023-07-14 08:32:36.973848 pycones-0.1.3/README.md
+-rw-r--r--   0        0        0     1843 2023-07-14 08:31:55.873855 pycones-0.1.3/pycones/__init__.py
+-rw-r--r--   0        0        0      676 2023-07-14 08:28:06.063893 pycones-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1098 1970-01-01 00:00:00.000000 pycones-0.1.3/PKG-INFO
```

### Comparing `pycones-0.1.2/pyproject.toml` & `pycones-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pycones"
-version = "0.1.2"
+version = "0.1.3"
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
-current_version = "0.1.2"
+current_version = "0.1.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
     'version = "{version}"',
 ]
```

### Comparing `pycones-0.1.2/PKG-INFO` & `pycones-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycones
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: william
 Author-email: william_swl@163.com
 Requires-Python: >=3.6
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -41,7 +41,13 @@
 - join lists into a string
 
 ```python
 list_join(list("abc"), list("def"), sep=",")
 # "a,b,c,d,e,f"
 ```
 
+- switch jupyter kernel into python or r
+
+```python
+nb_kernel_switch(notebook_path, kernel='python')
+```
+
```

