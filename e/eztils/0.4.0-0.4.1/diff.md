# Comparing `tmp/eztils-0.4.0.tar.gz` & `tmp/eztils-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eztils-0.4.0.tar", max compression
+gzip compressed data, was "eztils-0.4.1.tar", max compression
```

## Comparing `eztils-0.4.0.tar` & `eztils-0.4.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1075 2023-07-14 01:17:51.780650 eztils-0.4.0/LICENSE
--rw-r--r--   0        0        0    12710 2023-07-14 01:52:52.320035 eztils-0.4.0/README.md
--rw-r--r--   0        0        0      542 2023-07-14 02:09:17.596159 eztils-0.4.0/eztils/__init__.py
--rw-r--r--   0        0        0      808 2023-07-14 02:09:17.600159 eztils-0.4.0/eztils/default/__init__.py
--rw-r--r--   0        0        0     2341 2023-07-14 01:58:12.724178 eztils-0.4.0/eztils/default/logging.py
--rw-r--r--   0        0        0      112 2023-07-14 02:09:16.540172 eztils-0.4.0/eztils/default/math.py
--rw-r--r--   0        0        0     1091 2023-07-14 01:58:12.704178 eztils-0.4.0/eztils/default/structures.py
--rw-r--r--   0        0        0      265 2023-07-14 02:09:16.960167 eztils-0.4.0/eztils/torch/__init__.py
--rw-r--r--   0        0        0      688 2023-07-14 02:09:17.632159 eztils-0.4.0/eztils/torch/utils/__init__.py
--rw-r--r--   0        0        0     5667 2023-07-14 02:09:17.640159 eztils-0.4.0/eztils/torch/utils/arrays.py
--rw-r--r--   0        0        0      962 2023-07-14 01:17:51.780650 eztils-0.4.0/eztils/torch/utils/model_wrappers.py
--rw-r--r--   0        0        0     3457 2023-07-14 02:09:10.176249 eztils-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    13743 1970-01-01 00:00:00.000000 eztils-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-14 01:17:51.780650 eztils-0.4.1/LICENSE
+-rw-r--r--   0        0        0    12710 2023-07-14 01:52:52.320035 eztils-0.4.1/README.md
+-rw-r--r--   0        0        0      542 2023-07-14 02:09:17.596159 eztils-0.4.1/eztils/__init__.py
+-rw-r--r--   0        0        0      879 2023-07-14 02:29:30.133442 eztils-0.4.1/eztils/default/__init__.py
+-rw-r--r--   0        0        0     2341 2023-07-14 01:58:12.724178 eztils-0.4.1/eztils/default/logging.py
+-rw-r--r--   0        0        0      112 2023-07-14 02:09:16.540172 eztils-0.4.1/eztils/default/math.py
+-rw-r--r--   0        0        0     1091 2023-07-14 01:58:12.704178 eztils-0.4.1/eztils/default/structures.py
+-rw-r--r--   0        0        0      265 2023-07-14 02:09:16.960167 eztils-0.4.1/eztils/torch/__init__.py
+-rw-r--r--   0        0        0      688 2023-07-14 02:09:17.632159 eztils-0.4.1/eztils/torch/utils/__init__.py
+-rw-r--r--   0        0        0     5667 2023-07-14 02:09:17.640159 eztils-0.4.1/eztils/torch/utils/arrays.py
+-rw-r--r--   0        0        0      962 2023-07-14 01:17:51.780650 eztils-0.4.1/eztils/torch/utils/model_wrappers.py
+-rw-r--r--   0        0        0     3457 2023-07-14 02:29:08.441706 eztils-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0    13743 1970-01-01 00:00:00.000000 eztils-0.4.1/PKG-INFO
```

### Comparing `eztils-0.4.0/LICENSE` & `eztils-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eztils-0.4.0/README.md` & `eztils-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `eztils-0.4.0/eztils/__init__.py` & `eztils-0.4.1/eztils/__init__.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.0/eztils/default/logging.py` & `eztils-0.4.1/eztils/default/logging.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.0/eztils/default/structures.py` & `eztils-0.4.1/eztils/default/structures.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.0/eztils/torch/utils/__init__.py` & `eztils-0.4.1/eztils/torch/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.0/eztils/torch/utils/arrays.py` & `eztils-0.4.1/eztils/torch/utils/arrays.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.0/eztils/torch/utils/model_wrappers.py` & `eztils-0.4.1/eztils/torch/utils/model_wrappers.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.0/pyproject.toml` & `eztils-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 authors = ["ezhang7423 <ezhang7423@student.palomar.edu>"]
 description = "eds utilities"
 homepage = "https://github.com/ezhang7423/eztils"
 license = "MIT"
 name = "eztils"
 readme = "README.md"
 repository = "https://github.com/ezhang7423/eztils"
-version = "0.4.0"
+version = "0.4.1"
 
 # Keywords description https://python-poetry.org/docs/pyproject/#keywords
 keywords = [] #! Update me
 
 # Pypi classifiers: https://pypi.org/classifiers/
 classifiers = [
   #! Update me
```

### Comparing `eztils-0.4.0/PKG-INFO` & `eztils-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eztils
-Version: 0.4.0
+Version: 0.4.1
 Summary: eds utilities
 Home-page: https://github.com/ezhang7423/eztils
 License: MIT
 Author: ezhang7423
 Author-email: ezhang7423@student.palomar.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

