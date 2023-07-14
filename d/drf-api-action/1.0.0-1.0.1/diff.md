# Comparing `tmp/drf_api_action-1.0.0.tar.gz` & `tmp/drf_api_action-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_api_action-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "drf_api_action-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `drf_api_action-1.0.0.tar` & `drf_api_action-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     4662 2023-06-30 15:08:23.928144 drf_api_action-1.0.0/README.md
--rw-r--r--   0        0        0        0 2023-06-30 15:08:23.929499 drf_api_action-1.0.0/drf_api_action/__init__.py
--rw-r--r--   0        0        0     3850 2023-06-30 15:08:23.930489 drf_api_action-1.0.0/drf_api_action/decorators.py
--rw-r--r--   0        0        0       50 2023-06-30 15:08:23.930847 drf_api_action-1.0.0/drf_api_action/exceptions.py
--rw-r--r--   0        0        0      856 2023-06-30 15:08:23.931045 drf_api_action-1.0.0/drf_api_action/mixins.py
--rw-r--r--   0        0        0      693 2023-06-30 15:08:23.931279 drf_api_action-1.0.0/drf_api_action/utils.py
--rw-r--r--   0        0        0     4491 2023-06-30 15:08:23.931998 drf_api_action-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     5217 1970-01-01 00:00:00.000000 drf_api_action-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     4662 2023-06-30 15:08:23.928144 drf_api_action-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 15:08:23.929499 drf_api_action-1.0.1/drf_api_action/__init__.py
+-rw-r--r--   0        0        0     3850 2023-06-30 15:08:23.930489 drf_api_action-1.0.1/drf_api_action/decorators.py
+-rw-r--r--   0        0        0       50 2023-06-30 15:08:23.930847 drf_api_action-1.0.1/drf_api_action/exceptions.py
+-rw-r--r--   0        0        0      856 2023-06-30 15:08:23.931045 drf_api_action-1.0.1/drf_api_action/mixins.py
+-rw-r--r--   0        0        0      693 2023-06-30 15:08:23.931279 drf_api_action-1.0.1/drf_api_action/utils.py
+-rw-r--r--   0        0        0     4491 2023-07-13 10:23:29.533830 drf_api_action-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5217 1970-01-01 00:00:00.000000 drf_api_action-1.0.1/PKG-INFO
```

### Comparing `drf_api_action-1.0.0/README.md` & `drf_api_action-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `drf_api_action-1.0.0/drf_api_action/decorators.py` & `drf_api_action-1.0.1/drf_api_action/decorators.py`

 * *Files identical despite different names*

### Comparing `drf_api_action-1.0.0/drf_api_action/mixins.py` & `drf_api_action-1.0.1/drf_api_action/mixins.py`

 * *Files identical despite different names*

### Comparing `drf_api_action-1.0.0/drf_api_action/utils.py` & `drf_api_action-1.0.1/drf_api_action/utils.py`

 * *Files identical despite different names*

### Comparing `drf_api_action-1.0.0/pyproject.toml` & `drf_api_action-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "drf_api_action"
 description = "use the power of restframework also as a library functions"
-version = "1.0.0"
+version = "1.0.1"
 readme = "README.md"
-dependencies = ["Django>=4.2.2", "djangorestframework>=3.14.0", "pytest-django>=4.5.2"]
+dependencies = ["Django>=4.2.3", "djangorestframework>=3.14.0", "pytest-django>=4.5.2"]
 authors = [
   { name="Ori Roza", email="ori75660@gmail.com" },
 ]
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `drf_api_action-1.0.0/PKG-INFO` & `drf_api_action-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: drf_api_action
-Version: 1.0.0
+Version: 1.0.1
 Summary: use the power of restframework also as a library functions
 Author-email: Ori Roza <ori75660@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Dist: Django>=4.2.2
+Requires-Dist: Django>=4.2.3
 Requires-Dist: djangorestframework>=3.14.0
 Requires-Dist: pytest-django>=4.5.2
 Project-URL: Homepage, https://github.com/Ori-Roza/drf-api-action
 
 # drf-api-action
 
 [![python - 3.8 | 3.9 | 3.10 | 3.11](https://img.shields.io/badge/python-3.8_|_3.9_|_3.10_|_3.11-blue)](https://)[![CI](https://github.com/Ori-Roza/drf-api-action/actions/workflows/tests.yaml/badge.svg?branch=master)](https://github.com/Ori-Roza/drf-api-action/actions/workflows/tests.yaml)
```

