# Comparing `tmp/move_ugc_python-0.7.4.tar.gz` & `tmp/move_ugc_python-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "move_ugc_python-0.7.4.tar", max compression
+gzip compressed data, was "move_ugc_python-0.7.5.tar", max compression
```

## Comparing `move_ugc_python-0.7.4.tar` & `move_ugc_python-0.7.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1307 2023-07-13 15:43:59.281768 move_ugc_python-0.7.4/README.md
--rw-r--r--   0        0        0       90 2023-07-13 15:43:59.285769 move_ugc_python-0.7.4/move_ugc/__init__.py
--rw-r--r--   0        0        0       56 2023-07-13 15:43:59.285769 move_ugc_python-0.7.4/move_ugc/gql_requests/__init__.py
--rw-r--r--   0        0        0      306 2023-07-13 15:43:59.285769 move_ugc_python-0.7.4/move_ugc/gql_requests/additional_file.py
--rw-r--r--   0        0        0      116 2023-07-13 15:43:59.285769 move_ugc_python-0.7.4/move_ugc/gql_requests/client.py
--rw-r--r--   0        0        0     1067 2023-07-13 15:43:59.285769 move_ugc_python-0.7.4/move_ugc/gql_requests/file.py
--rw-r--r--   0        0        0     1102 2023-07-13 15:43:59.285769 move_ugc_python-0.7.4/move_ugc/gql_requests/job.py
--rw-r--r--   0        0        0     1334 2023-07-13 15:43:59.285769 move_ugc_python-0.7.4/move_ugc/gql_requests/take.py
--rw-r--r--   0        0        0        0 2023-07-13 15:43:59.285769 move_ugc_python-0.7.4/move_ugc/py.typed
--rw-r--r--   0        0        0       36 2023-07-13 15:43:59.285769 move_ugc_python-0.7.4/move_ugc/schemas/__init__.py
--rw-r--r--   0        0        0     2165 2023-07-13 15:43:59.285769 move_ugc_python-0.7.4/move_ugc/schemas/additional_file.py
--rw-r--r--   0        0        0      709 2023-07-13 15:43:59.285769 move_ugc_python-0.7.4/move_ugc/schemas/client.py
--rw-r--r--   0        0        0      250 2023-07-13 15:43:59.285769 move_ugc_python-0.7.4/move_ugc/schemas/constants.py
--rw-r--r--   0        0        0     1489 2023-07-13 15:43:59.285769 move_ugc_python-0.7.4/move_ugc/schemas/file.py
--rw-r--r--   0        0        0      866 2023-07-13 15:43:59.285769 move_ugc_python-0.7.4/move_ugc/schemas/gql.py
--rw-r--r--   0        0        0     1937 2023-07-13 15:43:59.285769 move_ugc_python-0.7.4/move_ugc/schemas/job.py
--rw-r--r--   0        0        0     1198 2023-07-13 15:43:59.285769 move_ugc_python-0.7.4/move_ugc/schemas/metaclient.py
--rw-r--r--   0        0        0     1827 2023-07-13 15:43:59.285769 move_ugc_python-0.7.4/move_ugc/schemas/take.py
--rw-r--r--   0        0        0      998 2023-07-13 15:43:59.285769 move_ugc_python-0.7.4/move_ugc/schemas/transport.py
--rw-r--r--   0        0        0       54 2023-07-13 15:43:59.285769 move_ugc_python-0.7.4/move_ugc/services/__init__.py
--rw-r--r--   0        0        0     1618 2023-07-13 15:43:59.285769 move_ugc_python-0.7.4/move_ugc/services/base.py
--rw-r--r--   0        0        0     2296 2023-07-13 15:43:59.285769 move_ugc_python-0.7.4/move_ugc/services/file.py
--rw-r--r--   0        0        0     2432 2023-07-13 15:43:59.285769 move_ugc_python-0.7.4/move_ugc/services/job.py
--rw-r--r--   0        0        0     3239 2023-07-13 15:43:59.285769 move_ugc_python-0.7.4/move_ugc/services/take.py
--rw-r--r--   0        0        0      592 2023-07-13 15:43:59.285769 move_ugc_python-0.7.4/move_ugc/settings.py
--rw-r--r--   0        0        0      886 2023-07-13 15:43:59.285769 move_ugc_python-0.7.4/move_ugc/ugc_client.py
--rw-r--r--   0        0        0     1279 2023-07-13 15:43:59.285769 move_ugc_python-0.7.4/pyproject.toml
--rw-r--r--   0        0        0     1803 1970-01-01 00:00:00.000000 move_ugc_python-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1339 2023-07-14 08:16:28.847084 move_ugc_python-0.7.5/README.md
+-rw-r--r--   0        0        0       90 2023-07-14 08:16:28.847084 move_ugc_python-0.7.5/move_ugc/__init__.py
+-rw-r--r--   0        0        0       56 2023-07-14 08:16:28.847084 move_ugc_python-0.7.5/move_ugc/gql_requests/__init__.py
+-rw-r--r--   0        0        0      306 2023-07-14 08:16:28.847084 move_ugc_python-0.7.5/move_ugc/gql_requests/additional_file.py
+-rw-r--r--   0        0        0      116 2023-07-14 08:16:28.847084 move_ugc_python-0.7.5/move_ugc/gql_requests/client.py
+-rw-r--r--   0        0        0     1067 2023-07-14 08:16:28.847084 move_ugc_python-0.7.5/move_ugc/gql_requests/file.py
+-rw-r--r--   0        0        0     1102 2023-07-14 08:16:28.847084 move_ugc_python-0.7.5/move_ugc/gql_requests/job.py
+-rw-r--r--   0        0        0     1334 2023-07-14 08:16:28.847084 move_ugc_python-0.7.5/move_ugc/gql_requests/take.py
+-rw-r--r--   0        0        0        0 2023-07-14 08:16:28.847084 move_ugc_python-0.7.5/move_ugc/py.typed
+-rw-r--r--   0        0        0       36 2023-07-14 08:16:28.847084 move_ugc_python-0.7.5/move_ugc/schemas/__init__.py
+-rw-r--r--   0        0        0     2165 2023-07-14 08:16:28.847084 move_ugc_python-0.7.5/move_ugc/schemas/additional_file.py
+-rw-r--r--   0        0        0      709 2023-07-14 08:16:28.847084 move_ugc_python-0.7.5/move_ugc/schemas/client.py
+-rw-r--r--   0        0        0      250 2023-07-14 08:16:28.847084 move_ugc_python-0.7.5/move_ugc/schemas/constants.py
+-rw-r--r--   0        0        0     1489 2023-07-14 08:16:28.847084 move_ugc_python-0.7.5/move_ugc/schemas/file.py
+-rw-r--r--   0        0        0      866 2023-07-14 08:16:28.847084 move_ugc_python-0.7.5/move_ugc/schemas/gql.py
+-rw-r--r--   0        0        0     1937 2023-07-14 08:16:28.847084 move_ugc_python-0.7.5/move_ugc/schemas/job.py
+-rw-r--r--   0        0        0     1198 2023-07-14 08:16:28.847084 move_ugc_python-0.7.5/move_ugc/schemas/metaclient.py
+-rw-r--r--   0        0        0     1827 2023-07-14 08:16:28.847084 move_ugc_python-0.7.5/move_ugc/schemas/take.py
+-rw-r--r--   0        0        0      998 2023-07-14 08:16:28.847084 move_ugc_python-0.7.5/move_ugc/schemas/transport.py
+-rw-r--r--   0        0        0       54 2023-07-14 08:16:28.847084 move_ugc_python-0.7.5/move_ugc/services/__init__.py
+-rw-r--r--   0        0        0     1618 2023-07-14 08:16:28.847084 move_ugc_python-0.7.5/move_ugc/services/base.py
+-rw-r--r--   0        0        0     2296 2023-07-14 08:16:28.847084 move_ugc_python-0.7.5/move_ugc/services/file.py
+-rw-r--r--   0        0        0     2432 2023-07-14 08:16:28.847084 move_ugc_python-0.7.5/move_ugc/services/job.py
+-rw-r--r--   0        0        0     3239 2023-07-14 08:16:28.847084 move_ugc_python-0.7.5/move_ugc/services/take.py
+-rw-r--r--   0        0        0      592 2023-07-14 08:16:28.847084 move_ugc_python-0.7.5/move_ugc/settings.py
+-rw-r--r--   0        0        0      886 2023-07-14 08:16:28.847084 move_ugc_python-0.7.5/move_ugc/ugc_client.py
+-rw-r--r--   0        0        0     1279 2023-07-14 08:16:28.847084 move_ugc_python-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0     1835 1970-01-01 00:00:00.000000 move_ugc_python-0.7.5/PKG-INFO
```

### Comparing `move_ugc_python-0.7.4/README.md` & `move_ugc_python-0.7.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ![Tests](./badges/tests.svg)
 ![Coverage](./badges/coverage.svg)
 [![CI](https://github.com/move-ai/move-ugc-python/actions/workflows/ci.yml/badge.svg)](https://github.com/move-ai/move-ugc-python/actions/workflows/ci.yml)
 ![Documentation Style](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)
 
 ## Full documentation
 
-The full documentation is available at https://move-ai.github.io/move-ugc-python/
+The full documentation is available at https://move-ai.github.io/move-ugc-python/latest/
 
 ## Installation
 
 ### With pip:
 
 ```bash
 pip install move-ugc-python
@@ -43,8 +43,8 @@
 
 ```python
 video_file = ugc.files.retrieve(file_id="<FILE_ID>")
 ```
 
 ## Contribution Guide
 
-Information for how someone can contribute to this project can be found in our [documentation](/move-ugc-python/latest/contributing)
+Information for how someone can contribute to this project can be found in our [documentation](https://move-ai.github.io/move-ugc-python/latest/contributing)
```

### Comparing `move_ugc_python-0.7.4/move_ugc/gql_requests/file.py` & `move_ugc_python-0.7.5/move_ugc/gql_requests/file.py`

 * *Files identical despite different names*

### Comparing `move_ugc_python-0.7.4/move_ugc/gql_requests/job.py` & `move_ugc_python-0.7.5/move_ugc/gql_requests/job.py`

 * *Files identical despite different names*

### Comparing `move_ugc_python-0.7.4/move_ugc/gql_requests/take.py` & `move_ugc_python-0.7.5/move_ugc/gql_requests/take.py`

 * *Files identical despite different names*

### Comparing `move_ugc_python-0.7.4/move_ugc/schemas/additional_file.py` & `move_ugc_python-0.7.5/move_ugc/schemas/additional_file.py`

 * *Files identical despite different names*

### Comparing `move_ugc_python-0.7.4/move_ugc/schemas/client.py` & `move_ugc_python-0.7.5/move_ugc/schemas/client.py`

 * *Files identical despite different names*

### Comparing `move_ugc_python-0.7.4/move_ugc/schemas/file.py` & `move_ugc_python-0.7.5/move_ugc/schemas/file.py`

 * *Files identical despite different names*

### Comparing `move_ugc_python-0.7.4/move_ugc/schemas/gql.py` & `move_ugc_python-0.7.5/move_ugc/schemas/gql.py`

 * *Files identical despite different names*

### Comparing `move_ugc_python-0.7.4/move_ugc/schemas/job.py` & `move_ugc_python-0.7.5/move_ugc/schemas/job.py`

 * *Files identical despite different names*

### Comparing `move_ugc_python-0.7.4/move_ugc/schemas/metaclient.py` & `move_ugc_python-0.7.5/move_ugc/schemas/metaclient.py`

 * *Files identical despite different names*

### Comparing `move_ugc_python-0.7.4/move_ugc/schemas/take.py` & `move_ugc_python-0.7.5/move_ugc/schemas/take.py`

 * *Files identical despite different names*

### Comparing `move_ugc_python-0.7.4/move_ugc/schemas/transport.py` & `move_ugc_python-0.7.5/move_ugc/schemas/transport.py`

 * *Files identical despite different names*

### Comparing `move_ugc_python-0.7.4/move_ugc/services/base.py` & `move_ugc_python-0.7.5/move_ugc/services/base.py`

 * *Files identical despite different names*

### Comparing `move_ugc_python-0.7.4/move_ugc/services/file.py` & `move_ugc_python-0.7.5/move_ugc/services/file.py`

 * *Files identical despite different names*

### Comparing `move_ugc_python-0.7.4/move_ugc/services/job.py` & `move_ugc_python-0.7.5/move_ugc/services/job.py`

 * *Files identical despite different names*

### Comparing `move_ugc_python-0.7.4/move_ugc/services/take.py` & `move_ugc_python-0.7.5/move_ugc/services/take.py`

 * *Files identical despite different names*

### Comparing `move_ugc_python-0.7.4/move_ugc/settings.py` & `move_ugc_python-0.7.5/move_ugc/settings.py`

 * *Files identical despite different names*

### Comparing `move_ugc_python-0.7.4/move_ugc/ugc_client.py` & `move_ugc_python-0.7.5/move_ugc/ugc_client.py`

 * *Files identical despite different names*

### Comparing `move_ugc_python-0.7.4/pyproject.toml` & `move_ugc_python-0.7.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "move-ugc-python"
-version = "0.7.4"
+version = "0.7.5"
 description = ""
 authors = ["Move.ai"]
 readme = "README.md"
 packages = [{include = "move_ugc"}, {include = "move_ugc/py.typed"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
```

### Comparing `move_ugc_python-0.7.4/PKG-INFO` & `move_ugc_python-0.7.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: move-ugc-python
-Version: 0.7.4
+Version: 0.7.5
 Summary: 
 Author: Move.ai
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -20,15 +20,15 @@
 ![Tests](./badges/tests.svg)
 ![Coverage](./badges/coverage.svg)
 [![CI](https://github.com/move-ai/move-ugc-python/actions/workflows/ci.yml/badge.svg)](https://github.com/move-ai/move-ugc-python/actions/workflows/ci.yml)
 ![Documentation Style](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)
 
 ## Full documentation
 
-The full documentation is available at https://move-ai.github.io/move-ugc-python/
+The full documentation is available at https://move-ai.github.io/move-ugc-python/latest/
 
 ## Installation
 
 ### With pip:
 
 ```bash
 pip install move-ugc-python
@@ -58,8 +58,8 @@
 
 ```python
 video_file = ugc.files.retrieve(file_id="<FILE_ID>")
 ```
 
 ## Contribution Guide
 
-Information for how someone can contribute to this project can be found in our [documentation](/move-ugc-python/latest/contributing)
+Information for how someone can contribute to this project can be found in our [documentation](https://move-ai.github.io/move-ugc-python/latest/contributing)
```

