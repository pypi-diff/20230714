# Comparing `tmp/threads-api-1.1.5.tar.gz` & `tmp/threads-api-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threads-api-1.1.5.tar", last modified: Thu Jul 13 21:53:15 2023, max compression
+gzip compressed data, was "threads-api-1.1.6.tar", last modified: Thu Jul 13 22:08:36 2023, max compression
```

## Comparing `threads-api-1.1.5.tar` & `threads-api-1.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-13 21:53:15.006703 threads-api-1.1.5/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1068 2023-07-06 22:22:29.000000 threads-api-1.1.5/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    15004 2023-07-13 21:53:15.006703 threads-api-1.1.5/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    14474 2023-07-13 21:53:08.000000 threads-api-1.1.5/README.md
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      472 2023-07-13 21:53:08.000000 threads-api-1.1.5/pyproject.toml
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-13 21:53:15.006703 threads-api-1.1.5/setup.cfg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      768 2023-07-13 21:53:08.000000 threads-api-1.1.5/setup.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-13 21:53:15.002703 threads-api-1.1.5/threads_api/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 20:59:49.000000 threads-api-1.1.5/threads_api/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-13 21:53:15.006703 threads-api-1.1.5/threads_api/src/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:13:21.000000 threads-api-1.1.5/threads_api/src/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    41169 2023-07-13 21:53:08.000000 threads-api-1.1.5/threads_api/src/threads_api.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-13 21:53:15.006703 threads-api-1.1.5/threads_api/tests/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:19:18.000000 threads-api-1.1.5/threads_api/tests/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      305 2023-07-13 17:43:17.000000 threads-api-1.1.5/threads_api/tests/get_post_id_test.py
--rwxrwxr-x   0 daniel    (1000) daniel    (1000)      592 2023-07-13 21:53:08.000000 threads-api-1.1.5/threads_api/tests/get_threads_test.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-13 21:53:15.006703 threads-api-1.1.5/threads_api.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    15004 2023-07-13 21:53:14.000000 threads-api-1.1.5/threads_api.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      404 2023-07-13 21:53:14.000000 threads-api-1.1.5/threads_api.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-13 21:53:14.000000 threads-api-1.1.5/threads_api.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        8 2023-07-13 21:53:14.000000 threads-api-1.1.5/threads_api.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       12 2023-07-13 21:53:14.000000 threads-api-1.1.5/threads_api.egg-info/top_level.txt
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-13 22:08:36.547629 threads-api-1.1.6/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1068 2023-07-06 22:22:29.000000 threads-api-1.1.6/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    15089 2023-07-13 22:08:36.547629 threads-api-1.1.6/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    14474 2023-07-13 21:53:08.000000 threads-api-1.1.6/README.md
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      472 2023-07-13 22:08:34.000000 threads-api-1.1.6/pyproject.toml
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-13 22:08:36.547629 threads-api-1.1.6/setup.cfg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      853 2023-07-13 22:08:34.000000 threads-api-1.1.6/setup.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-13 22:08:36.543629 threads-api-1.1.6/threads_api/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 20:59:49.000000 threads-api-1.1.6/threads_api/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-13 22:08:36.543629 threads-api-1.1.6/threads_api/src/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:13:21.000000 threads-api-1.1.6/threads_api/src/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    41169 2023-07-13 21:53:08.000000 threads-api-1.1.6/threads_api/src/threads_api.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-13 22:08:36.547629 threads-api-1.1.6/threads_api/tests/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:19:18.000000 threads-api-1.1.6/threads_api/tests/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      305 2023-07-13 17:43:17.000000 threads-api-1.1.6/threads_api/tests/get_post_id_test.py
+-rwxrwxr-x   0 daniel    (1000) daniel    (1000)      592 2023-07-13 21:53:08.000000 threads-api-1.1.6/threads_api/tests/get_threads_test.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-13 22:08:36.543629 threads-api-1.1.6/threads_api.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    15089 2023-07-13 22:08:36.000000 threads-api-1.1.6/threads_api.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      404 2023-07-13 22:08:36.000000 threads-api-1.1.6/threads_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-13 22:08:36.000000 threads-api-1.1.6/threads_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        8 2023-07-13 22:08:36.000000 threads-api-1.1.6/threads_api.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       12 2023-07-13 22:08:36.000000 threads-api-1.1.6/threads_api.egg-info/top_level.txt
```

### Comparing `threads-api-1.1.5/LICENSE` & `threads-api-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `threads-api-1.1.5/PKG-INFO` & `threads-api-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: threads-api
-Version: 1.1.5
+Version: 1.1.6
 Summary: Unofficial Python client for Meta Threads.net API
 Home-page: https://github.com/danie1/threads-api
-Author: Danie1
-Author-email: 
+Author: Daniel Saad
+Author-email: danielsaad777@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # [<img src="https://raw.githubusercontent.com/danie1/threads-api/main/.github/logo.jpg" width="36" height="36" />](https://github.com/danie1) Meta's Threads.net API
 
 [![Downdloads](https://pepy.tech/badge/threads-api)](https://pypi.org/project/threads-api/)
 [![Version](https://img.shields.io/pypi/v/threads-api.svg?style=flat)](https://pypi.org/project/threads-api/)
```

### Comparing `threads-api-1.1.5/README.md` & `threads-api-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `threads-api-1.1.5/setup.py` & `threads-api-1.1.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='threads-api',
-    version='1.1.5',
+    version='1.1.6',
     description='Unofficial Python client for Meta Threads.net API',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    author='Danie1',
-    author_email='',
+    author='Daniel Saad',
+    author_email='danielsaad777@gmail.com',
     url='https://github.com/danie1/threads-api',
     packages=find_packages(),
     install_requires=[
         'aiohttp'
     ],
     classifiers=[
-        'Development Status :: 3 - Alpha',
+        'Operating System :: OS Independent',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3',
+
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
 )
```

### Comparing `threads-api-1.1.5/threads_api/src/threads_api.py` & `threads-api-1.1.6/threads_api/src/threads_api.py`

 * *Files identical despite different names*

### Comparing `threads-api-1.1.5/threads_api/tests/get_threads_test.py` & `threads-api-1.1.6/threads_api/tests/get_threads_test.py`

 * *Files identical despite different names*

### Comparing `threads-api-1.1.5/threads_api.egg-info/PKG-INFO` & `threads-api-1.1.6/threads_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: threads-api
-Version: 1.1.5
+Version: 1.1.6
 Summary: Unofficial Python client for Meta Threads.net API
 Home-page: https://github.com/danie1/threads-api
-Author: Danie1
-Author-email: 
+Author: Daniel Saad
+Author-email: danielsaad777@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # [<img src="https://raw.githubusercontent.com/danie1/threads-api/main/.github/logo.jpg" width="36" height="36" />](https://github.com/danie1) Meta's Threads.net API
 
 [![Downdloads](https://pepy.tech/badge/threads-api)](https://pypi.org/project/threads-api/)
 [![Version](https://img.shields.io/pypi/v/threads-api.svg?style=flat)](https://pypi.org/project/threads-api/)
```

