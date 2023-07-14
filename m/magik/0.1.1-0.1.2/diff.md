# Comparing `tmp/magik-0.1.1.tar.gz` & `tmp/magik-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magik-0.1.1.tar", last modified: Thu Jul 13 00:34:40 2023, max compression
+gzip compressed data, was "magik-0.1.2.tar", last modified: Fri Jul 14 12:30:16 2023, max compression
```

## Comparing `magik-0.1.1.tar` & `magik-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-13 00:34:40.831130 magik-0.1.1/
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     3210 2023-07-13 00:34:40.831009 magik-0.1.1/PKG-INFO
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     2840 2023-07-11 14:25:41.000000 magik-0.1.1/README.md
-drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-13 00:34:40.825345 magik-0.1.1/magik.egg-info/
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     3210 2023-07-13 00:34:40.000000 magik-0.1.1/magik.egg-info/PKG-INFO
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      600 2023-07-13 00:34:40.000000 magik-0.1.1/magik.egg-info/SOURCES.txt
--rw-r--r--   0 shivsakhuja   (501) staff       (20)        1 2023-07-13 00:34:40.000000 magik-0.1.1/magik.egg-info/dependency_links.txt
--rw-r--r--   0 shivsakhuja   (501) staff       (20)       52 2023-07-13 00:34:40.000000 magik-0.1.1/magik.egg-info/entry_points.txt
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      246 2023-07-13 00:34:40.000000 magik-0.1.1/magik.egg-info/requires.txt
--rw-r--r--   0 shivsakhuja   (501) staff       (20)       17 2023-07-13 00:34:40.000000 magik-0.1.1/magik.egg-info/top_level.txt
-drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-13 00:34:40.830525 magik-0.1.1/magik_prompt_sdk/
--rw-r--r--   0 shivsakhuja   (501) staff       (20)       34 2023-07-11 15:55:34.000000 magik-0.1.1/magik_prompt_sdk/__init__.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1301 2023-07-11 14:06:10.000000 magik-0.1.1/magik_prompt_sdk/cli.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      477 2023-07-11 13:50:13.000000 magik-0.1.1/magik_prompt_sdk/config.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      515 2023-07-11 13:26:16.000000 magik-0.1.1/magik_prompt_sdk/constants.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1392 2023-07-11 13:46:49.000000 magik-0.1.1/magik_prompt_sdk/deploy.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     7014 2023-07-11 15:55:38.000000 magik-0.1.1/magik_prompt_sdk/evaluators.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      746 2023-07-08 22:47:12.000000 magik-0.1.1/magik_prompt_sdk/generate.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1711 2023-07-08 22:46:41.000000 magik-0.1.1/magik_prompt_sdk/initialize.py
-drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-13 00:34:40.830735 magik-0.1.1/magik_prompt_sdk/logger/
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1922 2023-07-06 18:14:00.000000 magik-0.1.1/magik_prompt_sdk/logger/__init__.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      390 2023-07-08 20:18:24.000000 magik-0.1.1/magik_prompt_sdk/matchers.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     4382 2023-07-13 00:02:48.000000 magik-0.1.1/magik_prompt_sdk/openai_helper.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     5733 2023-07-11 15:55:39.000000 magik-0.1.1/magik_prompt_sdk/run.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     2992 2023-07-08 22:49:32.000000 magik-0.1.1/magik_prompt_sdk/sys_exec.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      299 2023-07-06 16:24:21.000000 magik-0.1.1/magik_prompt_sdk/utils.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)       38 2023-07-13 00:34:40.831162 magik-0.1.1/setup.cfg
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      834 2023-07-13 00:32:47.000000 magik-0.1.1/setup.py
+drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-14 12:30:16.803346 magik-0.1.2/
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     3210 2023-07-14 12:30:16.803185 magik-0.1.2/PKG-INFO
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     2840 2023-07-11 14:25:41.000000 magik-0.1.2/README.md
+drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-14 12:30:16.801602 magik-0.1.2/magik/
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)        0 2023-07-14 11:51:21.000000 magik-0.1.2/magik/__init__.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     2374 2023-07-14 12:27:41.000000 magik-0.1.2/magik/cli.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      455 2023-07-14 12:27:41.000000 magik-0.1.2/magik/config.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      583 2023-07-14 12:27:11.000000 magik-0.1.2/magik/constants.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1365 2023-07-14 12:27:39.000000 magik-0.1.2/magik/deploy.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     6992 2023-07-14 12:27:41.000000 magik-0.1.2/magik/evaluators.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      711 2023-07-14 12:27:41.000000 magik-0.1.2/magik/generate.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1676 2023-07-14 12:27:41.000000 magik-0.1.2/magik/initialize.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1922 2023-07-14 11:50:58.000000 magik-0.1.2/magik/internal_logger.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      608 2023-07-14 12:27:41.000000 magik-0.1.2/magik/logger.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      390 2023-07-08 20:18:24.000000 magik-0.1.2/magik/matchers.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1043 2023-07-14 12:27:41.000000 magik-0.1.2/magik/openai_helper.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     6146 2023-07-14 12:27:41.000000 magik-0.1.2/magik/run.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     2990 2023-07-14 12:27:41.000000 magik-0.1.2/magik/sys_exec.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      299 2023-07-06 16:24:21.000000 magik-0.1.2/magik/utils.py
+drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-14 12:30:16.802950 magik-0.1.2/magik.egg-info/
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     3210 2023-07-14 12:30:16.000000 magik-0.1.2/magik.egg-info/PKG-INFO
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      462 2023-07-14 12:30:16.000000 magik-0.1.2/magik.egg-info/SOURCES.txt
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)        1 2023-07-14 12:30:16.000000 magik-0.1.2/magik.egg-info/dependency_links.txt
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)       45 2023-07-14 12:30:16.000000 magik-0.1.2/magik.egg-info/entry_points.txt
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      234 2023-07-14 12:30:16.000000 magik-0.1.2/magik.egg-info/requires.txt
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)        6 2023-07-14 12:30:16.000000 magik-0.1.2/magik.egg-info/top_level.txt
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)       38 2023-07-14 12:30:16.803388 magik-0.1.2/setup.cfg
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      827 2023-07-14 12:29:44.000000 magik-0.1.2/setup.py
```

### Comparing `magik-0.1.1/PKG-INFO` & `magik-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magik
-Version: 0.1.1
+Version: 0.1.2
 Summary: SDK to write and run tests for your LLM app
 Author: Magik Labs Team
 Author-email: hello@magiklabs.app
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `magik-0.1.1/README.md` & `magik-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `magik-0.1.1/magik.egg-info/PKG-INFO` & `magik-0.1.2/magik.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magik
-Version: 0.1.1
+Version: 0.1.2
 Summary: SDK to write and run tests for your LLM app
 Author: Magik Labs Team
 Author-email: hello@magiklabs.app
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `magik-0.1.1/magik_prompt_sdk/deploy.py` & `magik-0.1.2/magik/deploy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import os
 import requests
-from magik_prompt_sdk.logger import logger
-from magik_prompt_sdk.constants import CONFIG_FILE_PATH, DEPLOY_URL
-from magik_prompt_sdk.config import get_magik_api_key
+from magik.internal_logger import logger
+from magik.constants import CONFIG_FILE_PATH, DEPLOY_URL, TEST_DIR
+from magik.config import get_magik_api_key
 
 
 def deploy_test(test_name: str):
     api_key = get_magik_api_key()
     if api_key == None:
         logger.error(f"No API key found. Please add your API key to {CONFIG_FILE_PATH}")
 
     # construct the file path
-    file_path = f"./magik/tests/{test_name}/assertions.py"
+    file_path = f"{TEST_DIR}/{test_name}/assertions.py"
 
     # check if the file exists
     if not os.path.isfile(file_path):
         logger.info(f"No assertions.py file found for test_name {test_name}")
         return
 
     # read file
@@ -36,12 +36,12 @@
     else:
         logger.info(
             f"Failed to upload {file_path}. Status code: {response.status_code}"
         )
 
 
 def deploy_all(api_key: str):
-    # find all test_ids in ./magik/tests
-    test_names = os.listdir("./magik/tests")
+    # find all test_ids in {TEST_DIR}
+    test_names = os.listdir(TEST_DIR)
 
     for test_name in test_names:
         deploy_test(test_name, api_key)
```

### Comparing `magik-0.1.1/magik_prompt_sdk/evaluators.py` & `magik-0.1.2/magik/evaluators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Contains functions to evaluate assertions.
 import re
 import ast
-from magik_prompt_sdk.openai_helper import OpenAI
-from magik_prompt_sdk.constants import OPEN_AI_DEFAULT_MODEL
+from magik.openai_helper import OpenAI
+from magik.constants import OPEN_AI_DEFAULT_MODEL
 
 
 def generate_grading_prompt(output_to_evaluate, grading_criteria):
     return (
         """
     You are grading a response string according to a grading criteria given to you.
```

### Comparing `magik-0.1.1/magik_prompt_sdk/initialize.py` & `magik-0.1.2/magik/initialize.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
-from magik_prompt_sdk.logger import logger
-from magik_prompt_sdk.sys_exec import write_to_file
-from magik_prompt_sdk.constants import (
+from magik.internal_logger import logger
+from magik.sys_exec import write_to_file
+from magik.constants import (
     TESTRUNS_DIR,
     TEST_DIR,
     CONFIG_FILE_PATH,
     EXAMPLE_CONFIG_PATH,
 )
-from magik_prompt_sdk.sys_exec import read_from_file
+from magik.sys_exec import read_from_file
 
 
 # Create magik_tests directory
 # Create magik_test_runs directory
 # Create magik_config.json
 def initialize():
     create_magik_tests_dir()
```

### Comparing `magik-0.1.1/magik_prompt_sdk/logger/__init__.py` & `magik-0.1.2/magik/internal_logger.py`

 * *Files identical despite different names*

### Comparing `magik-0.1.1/magik_prompt_sdk/run.py` & `magik-0.1.2/magik/run.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,44 @@
 import os
+import requests
 import sys
 import importlib.util
 from datetime import datetime
-from magik_prompt_sdk.logger import logger
-from magik_prompt_sdk.utils import substitute_vars
-from magik_prompt_sdk.openai_helper import OpenAI
-from magik_prompt_sdk.sys_exec import read_from_file, create_file
-from magik_prompt_sdk.config import get_open_ai_default_model
-from magik_prompt_sdk.constants import TESTRUNS_DIR, TEST_DIR
+from magik.internal_logger import logger
+from magik.utils import substitute_vars
+from magik.openai_helper import OpenAI
+from magik.sys_exec import read_from_file, create_file
+from magik.config import get_open_ai_default_model, get_magik_api_key
+from magik.constants import TESTRUNS_DIR, TEST_DIR, RUN_URL
 
 
 def run_tests(test_name):
     tests = _load_tests(test_name)
     raw_prompt = _load_prompt(test_name)
     log_file_path = _log_file_path(test_name)
     _run_tests_for_prompt(test_name, tests, raw_prompt, log_file_path=log_file_path)
 
 
+def run_tests_in_prod(start_date, end_date, prompt_slug):
+    request_data = {
+        "source": "CLI",
+        "startDate": start_date,
+        "endDate": end_date,
+        "promptSlug": prompt_slug,
+    }
+    print(f"Sending request to {RUN_URL} with data: {request_data}")
+    requests.post(
+        RUN_URL,
+        json=request_data,
+        headers={
+            "magik-api-key": get_magik_api_key(),
+        },
+    )
+
+
 def _run_tests_for_prompt(test_name, tests, raw_prompt, log_file_path):
     _log_to_file_and_console("---------------")
     _log_to_file_and_console("TEST RESULTS")
     _log_to_file_and_console("---------------")
     _log_to_file_and_console("\n")
 
     num_tests_passed = 0
```

### Comparing `magik-0.1.1/magik_prompt_sdk/sys_exec.py` & `magik-0.1.2/magik/sys_exec.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 import os
 import json
 import subprocess
-from magik_prompt_sdk.logger import logger
+from magik.internal_logger import logger
 
 
 def execute_command(command, confirm=True, log=True):
     if confirm:
         confirmation = input(f"Run '{command}'? (y/n)")
         if confirmation != "y":
             return
```

### Comparing `magik-0.1.1/setup.py` & `magik-0.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,27 +4,27 @@
     long_description = fh.read()
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="magik",
-    version="0.1.1",
+    version="0.1.2",
     author="Magik Labs Team",
     author_email="hello@magiklabs.app",
     description="SDK to write and run tests for your LLM app",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     install_requires=requirements,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     entry_points={
         "console_scripts": [
-            "magik=magik_prompt_sdk.cli:main",
+            "magik=magik_sdk.cli:main",
         ],
     },
     python_requires=">=3.6",
 )
```

