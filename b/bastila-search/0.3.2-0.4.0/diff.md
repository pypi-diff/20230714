# Comparing `tmp/bastila_search-0.3.2.tar.gz` & `tmp/bastila_search-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bastila_search-0.3.2.tar", last modified: Fri Jul  7 04:52:36 2023, max compression
+gzip compressed data, was "bastila_search-0.4.0.tar", last modified: Fri Jul 14 19:03:31 2023, max compression
```

## Comparing `bastila_search-0.3.2.tar` & `bastila_search-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2023-07-07 04:52:36.292474 bastila_search-0.3.2/
--rw-rw-r--   0 joe       (1000) joe       (1000)     1064 2023-07-07 03:39:14.000000 bastila_search-0.3.2/LICENSE
--rw-rw-r--   0 joe       (1000) joe       (1000)      287 2023-07-07 04:52:36.292474 bastila_search-0.3.2/PKG-INFO
--rw-rw-r--   0 joe       (1000) joe       (1000)        0 2023-07-07 03:28:42.000000 bastila_search-0.3.2/README.md
-drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2023-07-07 04:52:36.292474 bastila_search-0.3.2/bastila_search/
--rw-rw-r--   0 joe       (1000) joe       (1000)        0 2023-07-07 03:29:31.000000 bastila_search-0.3.2/bastila_search/__init__.py
--rw-rw-r--   0 joe       (1000) joe       (1000)     4178 2023-07-07 04:22:49.000000 bastila_search-0.3.2/bastila_search/bastila_search.py
--rw-rw-r--   0 joe       (1000) joe       (1000)      437 2023-07-07 04:15:04.000000 bastila_search-0.3.2/bastila_search/setup_config.py
-drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2023-07-07 04:52:36.292474 bastila_search-0.3.2/bastila_search.egg-info/
--rw-rw-r--   0 joe       (1000) joe       (1000)      287 2023-07-07 04:52:36.000000 bastila_search-0.3.2/bastila_search.egg-info/PKG-INFO
--rw-rw-r--   0 joe       (1000) joe       (1000)      384 2023-07-07 04:52:36.000000 bastila_search-0.3.2/bastila_search.egg-info/SOURCES.txt
--rw-rw-r--   0 joe       (1000) joe       (1000)        1 2023-07-07 04:52:36.000000 bastila_search-0.3.2/bastila_search.egg-info/dependency_links.txt
--rw-rw-r--   0 joe       (1000) joe       (1000)      115 2023-07-07 04:52:36.000000 bastila_search-0.3.2/bastila_search.egg-info/entry_points.txt
--rw-rw-r--   0 joe       (1000) joe       (1000)        1 2023-07-07 03:41:59.000000 bastila_search-0.3.2/bastila_search.egg-info/not-zip-safe
--rw-rw-r--   0 joe       (1000) joe       (1000)        9 2023-07-07 04:52:36.000000 bastila_search-0.3.2/bastila_search.egg-info/requires.txt
--rw-rw-r--   0 joe       (1000) joe       (1000)       15 2023-07-07 04:52:36.000000 bastila_search-0.3.2/bastila_search.egg-info/top_level.txt
--rw-rw-r--   0 joe       (1000) joe       (1000)       38 2023-07-07 04:52:36.292474 bastila_search-0.3.2/setup.cfg
--rw-rw-r--   0 joe       (1000) joe       (1000)      611 2023-07-07 04:52:29.000000 bastila_search-0.3.2/setup.py
+drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2023-07-14 19:03:31.263542 bastila_search-0.4.0/
+-rw-rw-r--   0 joe       (1000) joe       (1000)     1064 2023-07-07 03:39:14.000000 bastila_search-0.4.0/LICENSE
+-rw-rw-r--   0 joe       (1000) joe       (1000)      287 2023-07-14 19:03:31.263542 bastila_search-0.4.0/PKG-INFO
+-rw-rw-r--   0 joe       (1000) joe       (1000)        0 2023-07-07 03:28:42.000000 bastila_search-0.4.0/README.md
+drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2023-07-14 19:03:31.263542 bastila_search-0.4.0/bastila_search/
+-rw-rw-r--   0 joe       (1000) joe       (1000)        0 2023-07-07 03:29:31.000000 bastila_search-0.4.0/bastila_search/__init__.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)     5155 2023-07-11 00:58:56.000000 bastila_search-0.4.0/bastila_search/bastila_search.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)      444 2023-07-11 00:59:13.000000 bastila_search-0.4.0/bastila_search/setup_config.py
+drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2023-07-14 19:03:31.263542 bastila_search-0.4.0/bastila_search.egg-info/
+-rw-rw-r--   0 joe       (1000) joe       (1000)      287 2023-07-14 19:03:31.000000 bastila_search-0.4.0/bastila_search.egg-info/PKG-INFO
+-rw-rw-r--   0 joe       (1000) joe       (1000)      384 2023-07-14 19:03:31.000000 bastila_search-0.4.0/bastila_search.egg-info/SOURCES.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)        1 2023-07-14 19:03:31.000000 bastila_search-0.4.0/bastila_search.egg-info/dependency_links.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)      115 2023-07-14 19:03:31.000000 bastila_search-0.4.0/bastila_search.egg-info/entry_points.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)        1 2023-07-07 03:41:59.000000 bastila_search-0.4.0/bastila_search.egg-info/not-zip-safe
+-rw-rw-r--   0 joe       (1000) joe       (1000)        9 2023-07-14 19:03:31.000000 bastila_search-0.4.0/bastila_search.egg-info/requires.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)       15 2023-07-14 19:03:31.000000 bastila_search-0.4.0/bastila_search.egg-info/top_level.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)       38 2023-07-14 19:03:31.263542 bastila_search-0.4.0/setup.cfg
+-rw-rw-r--   0 joe       (1000) joe       (1000)      611 2023-07-14 19:02:00.000000 bastila_search-0.4.0/setup.py
```

### Comparing `bastila_search-0.3.2/LICENSE` & `bastila_search-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bastila_search-0.3.2/bastila_search/bastila_search.py` & `bastila_search-0.4.0/bastila_search/bastila_search.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 import requests
 import json
 import re
-from pathlib import Path
 import sys
 import os
 import fnmatch
 
+from pathlib import Path
+
 base_url = 'https://bastila.dev'
 
+
 def load_config():
     try:
         with open("config.json", "r") as file:
             return json.load(file)
     except FileNotFoundError:
         return None
 
+
+def handle_exception(error):
+    print(error)
+    sys.exit(1)
+
+
 def fetch_patterns(session):
     response = session.get(f'{base_url}/api/check/standard-changes/')
     response.raise_for_status()
     standards = response.json()
 
     return standards['results']
 
@@ -102,58 +110,76 @@
     response.raise_for_status()
     return response.json()
 
 
 def main():
     config = load_config()
 
-    if config is None:
-        print("Configuration not found. Please run setup_config.py to set up the necessary parameters.")
-        sys.exit(1)
-    else:
-        bastila_key = config["BASTILA_KEY"]
-        block_on_failure = config["BLOCK_ON_FAILURE"]
+    BASTILA_KEY = os.getenv("BASTILA_KEY", None)
+    POST_RESULTS = os.getenv('POST_RESULTS', 'false').lower() == 'true'
+    PREVENT_REGRESSION = os.getenv("PREVENT_REGRESSION", 'false').lower() == 'true'
+
+    if config is None and BASTILA_KEY is None:
+        print("Configuration not found. Please run the command bastila_setup or setup an environment file to set up the necessary parameters.")
+        handle_exception()
+    elif config is not None:
+        BASTILA_KEY = config["BASTILA_KEY"]
+        PREVENT_REGRESSION = config["PREVENT_REGRESSION"]
 
     session = requests.Session()
     session.headers.update({
-        'Authorization': f'Api-Key {bastila_key}',
+        'Authorization': f'Api-Key {BASTILA_KEY}',
         'Content-Type': 'application/json'
     })
     print('Starting Bastila Search')
 
     try:
+        print('Starting check')
         check = create_check(session)
     except Exception as e:
-        sys.exit(e)
-
-    print('Started Check')
+        print('Create check failed')
+        handle_exception(e)
 
     try:
+        print('Fetching patterns')
         patterns = fetch_patterns(session)
     except Exception as e:
-        sys.exit(e)
-
-    print('Patterns Fetched')
+        print('Fetch patterns failed')
+        handle_exception(e)
 
     try:
+        print('Searching files')
         results = search_files(patterns)
     except Exception as e:
-        sys.exit(e)
+        print('Fetch patterns failed')
+        handle_exception(e)
 
-    print('Code Searched')
+    if POST_RESULTS:
+        try:
+            print('Posting results')
+            post_results(session, {
+              'check': check['id'],
+              'results': results
+            })
+        except Exception as e:
+            print('Posting results failed')
+            handle_exception(e)
 
     is_regression = False
     for result in results:
         if not result['is_successful']:
             print(result['fix_recommendation'])
             is_regression = True
 
     if is_regression:
         print('Check Failed')
-        if block_on_failure:
+        if PREVENT_REGRESSION:
             sys.exit(1)
-
-    print('Success')
+        else:
+            print('You are allowing regressions so we did not throw an error')
+    else:
+        print('Bastila check succeeded')
+    print('Bastila check complete')
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `bastila_search-0.3.2/setup.py` & `bastila_search-0.4.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='bastila_search',
-    version='0.3.2',
+    version='0.4.0',
     description='A python script that catches commits that introduce predefined deprecated patterns',
     url='https://github.com/GetBastila/bastila-hook',
     author='Bastila',
     author_email='hello@bastila.app',
     license='MIT',
     packages=['bastila_search'],
     install_requires=[
```

