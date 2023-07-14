# Comparing `tmp/threads-api-1.1.7.tar.gz` & `tmp/threads-api-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threads-api-1.1.7.tar", last modified: Fri Jul 14 16:26:41 2023, max compression
+gzip compressed data, was "threads-api-1.1.8.tar", last modified: Fri Jul 14 16:34:23 2023, max compression
```

## Comparing `threads-api-1.1.7.tar` & `threads-api-1.1.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-14 16:26:41.924255 threads-api-1.1.7/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1068 2023-07-06 22:22:29.000000 threads-api-1.1.7/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    15158 2023-07-14 16:26:41.924255 threads-api-1.1.7/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    14543 2023-07-14 16:25:20.000000 threads-api-1.1.7/README.md
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      472 2023-07-14 16:22:15.000000 threads-api-1.1.7/pyproject.toml
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-14 16:26:41.924255 threads-api-1.1.7/setup.cfg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      853 2023-07-14 16:22:11.000000 threads-api-1.1.7/setup.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-14 16:26:41.924255 threads-api-1.1.7/threads_api/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 20:59:49.000000 threads-api-1.1.7/threads_api/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-14 16:26:41.924255 threads-api-1.1.7/threads_api/src/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:13:21.000000 threads-api-1.1.7/threads_api/src/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    43668 2023-07-14 16:23:48.000000 threads-api-1.1.7/threads_api/src/threads_api.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-14 16:26:41.924255 threads-api-1.1.7/threads_api/tests/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:19:18.000000 threads-api-1.1.7/threads_api/tests/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      305 2023-07-13 17:43:17.000000 threads-api-1.1.7/threads_api/tests/get_post_id_test.py
--rwxrwxr-x   0 daniel    (1000) daniel    (1000)      592 2023-07-13 21:53:08.000000 threads-api-1.1.7/threads_api/tests/get_threads_test.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-14 16:26:41.924255 threads-api-1.1.7/threads_api.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    15158 2023-07-14 16:26:41.000000 threads-api-1.1.7/threads_api.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      404 2023-07-14 16:26:41.000000 threads-api-1.1.7/threads_api.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-14 16:26:41.000000 threads-api-1.1.7/threads_api.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        8 2023-07-14 16:26:41.000000 threads-api-1.1.7/threads_api.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       12 2023-07-14 16:26:41.000000 threads-api-1.1.7/threads_api.egg-info/top_level.txt
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-14 16:34:23.902443 threads-api-1.1.8/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1068 2023-07-06 22:22:29.000000 threads-api-1.1.8/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    15158 2023-07-14 16:34:23.902443 threads-api-1.1.8/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    14543 2023-07-14 16:25:20.000000 threads-api-1.1.8/README.md
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      472 2023-07-14 16:29:40.000000 threads-api-1.1.8/pyproject.toml
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-14 16:34:23.902443 threads-api-1.1.8/setup.cfg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      853 2023-07-14 16:29:34.000000 threads-api-1.1.8/setup.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-14 16:34:23.894443 threads-api-1.1.8/threads_api/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 20:59:49.000000 threads-api-1.1.8/threads_api/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-14 16:34:23.898443 threads-api-1.1.8/threads_api/src/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:13:21.000000 threads-api-1.1.8/threads_api/src/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    43640 2023-07-14 16:28:49.000000 threads-api-1.1.8/threads_api/src/threads_api.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-14 16:34:23.898443 threads-api-1.1.8/threads_api/tests/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:19:18.000000 threads-api-1.1.8/threads_api/tests/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      305 2023-07-13 17:43:17.000000 threads-api-1.1.8/threads_api/tests/get_post_id_test.py
+-rwxrwxr-x   0 daniel    (1000) daniel    (1000)      592 2023-07-13 21:53:08.000000 threads-api-1.1.8/threads_api/tests/get_threads_test.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-14 16:34:23.898443 threads-api-1.1.8/threads_api.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    15158 2023-07-14 16:34:23.000000 threads-api-1.1.8/threads_api.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      404 2023-07-14 16:34:23.000000 threads-api-1.1.8/threads_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-14 16:34:23.000000 threads-api-1.1.8/threads_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        8 2023-07-14 16:34:23.000000 threads-api-1.1.8/threads_api.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       12 2023-07-14 16:34:23.000000 threads-api-1.1.8/threads_api.egg-info/top_level.txt
```

### Comparing `threads-api-1.1.7/LICENSE` & `threads-api-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `threads-api-1.1.7/PKG-INFO` & `threads-api-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threads-api
-Version: 1.1.7
+Version: 1.1.8
 Summary: Unofficial Python client for Meta Threads.net API
 Home-page: https://github.com/danie1/threads-api
 Author: Daniel Saad
 Author-email: danielsaad777@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `threads-api-1.1.7/README.md` & `threads-api-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `threads-api-1.1.7/setup.py` & `threads-api-1.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='threads-api',
-    version='1.1.7',
+    version='1.1.8',
     description='Unofficial Python client for Meta Threads.net API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Daniel Saad',
     author_email='danielsaad777@gmail.com',
     url='https://github.com/danie1/threads-api',
     packages=find_packages(),
```

### Comparing `threads-api-1.1.7/threads_api/src/threads_api.py` & `threads-api-1.1.8/threads_api/src/threads_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,15 +212,15 @@
             except LoggedOutException as e:
                 print(f"[Error] {e}. Attempting to re-login.")
                 pass
 
         try:
             
             self.logger.info("Attempting to login")
-            self.instagrapi_client.login(username, password, relogin, verification_code)
+            self.instagrapi_client.login(username, password)
             token = self.instagrapi_client.private.headers['Authorization'].split("Bearer IGT:2:")[1]
             
             await _set_logged_in_state(username, token)
                     
             if cached_token_path is not None:
                 _save_token_to_cache(cached_token_path, token, password)
         except Exception as e:
```

### Comparing `threads-api-1.1.7/threads_api/tests/get_threads_test.py` & `threads-api-1.1.8/threads_api/tests/get_threads_test.py`

 * *Files identical despite different names*

### Comparing `threads-api-1.1.7/threads_api.egg-info/PKG-INFO` & `threads-api-1.1.8/threads_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threads-api
-Version: 1.1.7
+Version: 1.1.8
 Summary: Unofficial Python client for Meta Threads.net API
 Home-page: https://github.com/danie1/threads-api
 Author: Daniel Saad
 Author-email: danielsaad777@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

