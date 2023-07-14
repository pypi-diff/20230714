# Comparing `tmp/quri_parts_tket-0.11.0.tar.gz` & `tmp/quri_parts_tket-0.12.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quri_parts_tket-0.11.0.tar", max compression
+gzip compressed data, was "quri_parts_tket-0.12.0.post1.tar", max compression
```

## Comparing `quri_parts_tket-0.11.0.tar` & `quri_parts_tket-0.12.0.post1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11358 2023-05-30 10:40:14.643340 quri_parts_tket-0.11.0/LICENSE
--rw-r--r--   0        0        0      341 2023-05-30 10:40:14.643340 quri_parts_tket-0.11.0/README.md
--rw-r--r--   0        0        0     1103 2023-05-30 10:40:32.832048 quri_parts_tket-0.11.0/pyproject.toml
--rw-r--r--   0        0        0       34 2023-05-30 10:40:31.976011 quri_parts_tket-0.11.0/quri_parts/tket/NOTICE
--rw-r--r--   0        0        0        0 2023-05-30 10:40:14.643340 quri_parts_tket-0.11.0/quri_parts/tket/__init__.py
--rw-r--r--   0        0        0      725 2023-05-30 10:40:14.643340 quri_parts_tket-0.11.0/quri_parts/tket/circuit/__init__.py
--rw-r--r--   0        0        0     5592 2023-05-30 10:40:14.643340 quri_parts_tket-0.11.0/quri_parts/tket/circuit/circuit_converter.py
--rw-r--r--   0        0        0     4521 2023-05-30 10:40:14.643340 quri_parts_tket-0.11.0/quri_parts/tket/circuit/tket_circuit_converter.py
--rw-r--r--   0        0        0     1213 1970-01-01 00:00:00.000000 quri_parts_tket-0.11.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-07-14 07:25:35.450371 quri_parts_tket-0.12.0.post1/LICENSE
+-rw-r--r--   0        0        0      341 2023-07-14 07:25:35.450371 quri_parts_tket-0.12.0.post1/README.md
+-rw-r--r--   0        0        0     1109 2023-07-14 07:26:24.194692 quri_parts_tket-0.12.0.post1/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-07-14 07:26:23.350687 quri_parts_tket-0.12.0.post1/quri_parts/tket/NOTICE
+-rw-r--r--   0        0        0        0 2023-07-14 07:25:35.450371 quri_parts_tket-0.12.0.post1/quri_parts/tket/__init__.py
+-rw-r--r--   0        0        0      725 2023-07-14 07:25:35.450371 quri_parts_tket-0.12.0.post1/quri_parts/tket/circuit/__init__.py
+-rw-r--r--   0        0        0     5592 2023-07-14 07:25:35.450371 quri_parts_tket-0.12.0.post1/quri_parts/tket/circuit/circuit_converter.py
+-rw-r--r--   0        0        0     4521 2023-07-14 07:25:35.450371 quri_parts_tket-0.12.0.post1/quri_parts/tket/circuit/tket_circuit_converter.py
+-rw-r--r--   0        0        0     1219 1970-01-01 00:00:00.000000 quri_parts_tket-0.12.0.post1/PKG-INFO
```

### Comparing `quri_parts_tket-0.11.0/LICENSE` & `quri_parts_tket-0.12.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `quri_parts_tket-0.11.0/pyproject.toml` & `quri_parts_tket-0.12.0.post1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning", "setuptools"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "quri-parts-tket"
-version = "0.11.0"
+version = "0.12.0.post1"
 description = "A plugin to use tket with QURI Parts"
 license = "Apache-2.0"
 authors = ["QURI Parts Authors <opensource@qunasys.com>"]
 readme = "README.md"
 repository = "https://github.com/QunaSys/quri-parts"
 documentation = "https://quri-parts.qunasys.com"
 keywords = ["quantum", "quantum computing"]
```

### Comparing `quri_parts_tket-0.11.0/quri_parts/tket/circuit/__init__.py` & `quri_parts_tket-0.12.0.post1/quri_parts/tket/circuit/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_tket-0.11.0/quri_parts/tket/circuit/circuit_converter.py` & `quri_parts_tket-0.12.0.post1/quri_parts/tket/circuit/circuit_converter.py`

 * *Files identical despite different names*

### Comparing `quri_parts_tket-0.11.0/quri_parts/tket/circuit/tket_circuit_converter.py` & `quri_parts_tket-0.12.0.post1/quri_parts/tket/circuit/tket_circuit_converter.py`

 * *Files identical despite different names*

### Comparing `quri_parts_tket-0.11.0/PKG-INFO` & `quri_parts_tket-0.12.0.post1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quri-parts-tket
-Version: 0.11.0
+Version: 0.12.0.post1
 Summary: A plugin to use tket with QURI Parts
 Home-page: https://github.com/QunaSys/quri-parts
 License: Apache-2.0
 Keywords: quantum,quantum computing
 Author: QURI Parts Authors
 Author-email: opensource@qunasys.com
 Requires-Python: >=3.9.8,<4.0.0
```

