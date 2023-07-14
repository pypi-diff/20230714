# Comparing `tmp/easy_ge-0.1.7.tar.gz` & `tmp/easy_ge-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_ge-0.1.7.tar", max compression
+gzip compressed data, was "easy_ge-0.1.8.tar", max compression
```

## Comparing `easy_ge-0.1.7.tar` & `easy_ge-0.1.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1059 2023-07-14 04:13:27.522821 easy_ge-0.1.7/LICENSE
--rw-r--r--   0        0        0       88 2023-07-14 04:13:27.522821 easy_ge-0.1.7/easy_ge/__init__.py
--rw-r--r--   0        0        0      308 2023-07-14 04:13:27.522821 easy_ge-0.1.7/easy_ge/docker_entry.py
--rw-r--r--   0        0        0     6290 2023-07-14 04:13:27.522821 easy_ge-0.1.7/easy_ge/expectation_manager.py
--rw-r--r--   0        0        0     4468 2023-07-14 04:13:27.522821 easy_ge-0.1.7/easy_ge/helpers.py
--rw-r--r--   0        0        0     2321 2023-07-14 04:13:27.526821 easy_ge-0.1.7/easy_ge/main.py
--rw-r--r--   0        0        0      908 2023-07-14 04:13:27.526821 easy_ge-0.1.7/easy_ge/templates/checkpoint.tpl
--rw-r--r--   0        0        0     4535 2023-07-14 04:13:27.526821 easy_ge-0.1.7/easy_ge/templates/great_expectations.tpl
--rw-r--r--   0        0        0     5091 2023-07-14 04:13:27.526821 easy_ge-0.1.7/easy_ge/templates/schema.json
--rw-r--r--   0        0        0     1137 2023-07-14 04:13:48.503285 easy_ge-0.1.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-14 04:13:27.526821 easy_ge-0.1.7/readme.md
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 easy_ge-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-07-14 04:28:31.312322 easy_ge-0.1.8/LICENSE
+-rw-r--r--   0        0        0       95 2023-07-14 04:28:31.312322 easy_ge-0.1.8/easy_ge/__init__.py
+-rw-r--r--   0        0        0      308 2023-07-14 04:28:31.312322 easy_ge-0.1.8/easy_ge/docker_entry.py
+-rw-r--r--   0        0        0     6297 2023-07-14 04:28:31.312322 easy_ge-0.1.8/easy_ge/expectation_manager.py
+-rw-r--r--   0        0        0     4468 2023-07-14 04:28:31.312322 easy_ge-0.1.8/easy_ge/helpers.py
+-rw-r--r--   0        0        0     2335 2023-07-14 04:28:31.312322 easy_ge-0.1.8/easy_ge/main.py
+-rw-r--r--   0        0        0      908 2023-07-14 04:28:31.312322 easy_ge-0.1.8/easy_ge/templates/checkpoint.tpl
+-rw-r--r--   0        0        0     4535 2023-07-14 04:28:31.312322 easy_ge-0.1.8/easy_ge/templates/great_expectations.tpl
+-rw-r--r--   0        0        0     5091 2023-07-14 04:28:31.312322 easy_ge-0.1.8/easy_ge/templates/schema.json
+-rw-r--r--   0        0        0     1137 2023-07-14 04:28:31.316322 easy_ge-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-14 04:28:31.316322 easy_ge-0.1.8/readme.md
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 easy_ge-0.1.8/PKG-INFO
```

### Comparing `easy_ge-0.1.7/LICENSE` & `easy_ge-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.7/easy_ge/expectation_manager.py` & `easy_ge-0.1.8/easy_ge/expectation_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import pandas as pd
 from great_expectations.data_context import (AbstractDataContext,
                                              BaseDataContext)
 from great_expectations.data_context.types.base import DataContextConfig
 
 try:
-    from .helpers import TemplateHandler
+    from easy_ge.helpers import TemplateHandler
 except:
     from helpers import TemplateHandler
 
 import logging
 
 logging.basicConfig(
     level=logging.INFO,
```

### Comparing `easy_ge-0.1.7/easy_ge/helpers.py` & `easy_ge-0.1.8/easy_ge/helpers.py`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.7/easy_ge/main.py` & `easy_ge-0.1.8/easy_ge/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import logging
 from datetime import datetime
 
 try:
     from expectation_manager import ExpectationManager
     from helpers import ConfigLoader, TemplateHandler
 except:
-    from .expectation_manager import ExpectationManager
-    from .helpers import ConfigLoader, TemplateHandler  
+    from easy_ge.expectation_manager import ExpectationManager
+    from easy_ge.helpers import ConfigLoader, TemplateHandler  
 
 ###############################
 # ONLY FOR LOCAL Testing
 ###############################
 GCP_KEY_PATH = "gcp_key_spark.json"
 JAVA_HOME = "/usr/lib/jvm/java-11-openjdk-amd64"
 import os
```

### Comparing `easy_ge-0.1.7/easy_ge/templates/checkpoint.tpl` & `easy_ge-0.1.8/easy_ge/templates/checkpoint.tpl`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.7/easy_ge/templates/great_expectations.tpl` & `easy_ge-0.1.8/easy_ge/templates/great_expectations.tpl`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.7/easy_ge/templates/schema.json` & `easy_ge-0.1.8/easy_ge/templates/schema.json`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.7/pyproject.toml` & `easy_ge-0.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easy_ge"
-version = "0.1.7"
+version = "0.1.8"
 description = "A package that abstracts the complexity of Great Expectations away. At least for straight forward use cases."
 authors = ["Elsayed91 <elsayed.is@outlook.com>"]
 readme = "readme.md"
 packages = [{include = "easy_ge"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `easy_ge-0.1.7/PKG-INFO` & `easy_ge-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-ge
-Version: 0.1.7
+Version: 0.1.8
 Summary: A package that abstracts the complexity of Great Expectations away. At least for straight forward use cases.
 Author: Elsayed91
 Author-email: elsayed.is@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

