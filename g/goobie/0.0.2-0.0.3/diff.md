# Comparing `tmp/goobie-0.0.2.tar.gz` & `tmp/goobie-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goobie-0.0.2.tar", last modified: Fri Jul 14 01:42:04 2023, max compression
+gzip compressed data, was "goobie-0.0.3.tar", last modified: Fri Jul 14 01:51:51 2023, max compression
```

## Comparing `goobie-0.0.2.tar` & `goobie-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,19 @@
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-14 01:42:04.705935 goobie-0.0.2/
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      505 2023-07-14 01:42:04.689935 goobie-0.0.2/PKG-INFO
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-14 01:42:04.689935 goobie-0.0.2/goobie/
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-14 01:42:04.689935 goobie-0.0.2/goobie/stubs/
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       19 2023-07-14 01:26:37.000000 goobie-0.0.2/goobie/stubs/__init__.pyi
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       63 2023-07-14 01:26:50.000000 goobie-0.0.2/goobie/stubs/core.pyi
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       17 2023-07-14 01:25:25.000000 goobie-0.0.2/goobie/stubs/handler.pyi
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-14 01:42:04.689935 goobie-0.0.2/goobie.egg-info/
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      505 2023-07-14 01:42:04.000000 goobie-0.0.2/goobie.egg-info/PKG-INFO
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      201 2023-07-14 01:42:04.000000 goobie-0.0.2/goobie.egg-info/SOURCES.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        1 2023-07-14 01:42:04.000000 goobie-0.0.2/goobie.egg-info/dependency_links.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       20 2023-07-14 01:42:04.000000 goobie-0.0.2/goobie.egg-info/top_level.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       38 2023-07-14 01:42:04.705935 goobie-0.0.2/setup.cfg
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      873 2023-07-14 01:41:51.000000 goobie-0.0.2/setup.py
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-14 01:51:51.397352 goobie-0.0.3/
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      505 2023-07-14 01:51:51.397352 goobie-0.0.3/PKG-INFO
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-14 01:51:51.393352 goobie-0.0.3/goobie/
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       40 2023-07-14 01:27:03.000000 goobie-0.0.3/goobie/__init__.py
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       91 2023-07-14 01:22:58.000000 goobie-0.0.3/goobie/core.py
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-14 01:51:51.397352 goobie-0.0.3/goobie/stubs/
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       19 2023-07-14 01:26:37.000000 goobie-0.0.3/goobie/stubs/__init__.pyi
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       63 2023-07-14 01:26:50.000000 goobie-0.0.3/goobie/stubs/core.pyi
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       17 2023-07-14 01:25:25.000000 goobie-0.0.3/goobie/stubs/handler.pyi
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-14 01:51:51.397352 goobie-0.0.3/goobie/utils/
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       27 2023-07-14 01:24:30.000000 goobie-0.0.3/goobie/utils/__init__.py
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       39 2023-07-14 01:21:39.000000 goobie-0.0.3/goobie/utils/handler.py
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-14 01:51:51.397352 goobie-0.0.3/goobie.egg-info/
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      505 2023-07-14 01:51:51.000000 goobie-0.0.3/goobie.egg-info/PKG-INFO
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      284 2023-07-14 01:51:51.000000 goobie-0.0.3/goobie.egg-info/SOURCES.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        1 2023-07-14 01:51:51.000000 goobie-0.0.3/goobie.egg-info/dependency_links.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       33 2023-07-14 01:51:51.000000 goobie-0.0.3/goobie.egg-info/top_level.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       38 2023-07-14 01:51:51.397352 goobie-0.0.3/setup.cfg
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     1026 2023-07-14 01:51:05.000000 goobie-0.0.3/setup.py
```

### Comparing `goobie-0.0.2/setup.py` & `goobie-0.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = ''
 KEYWORDS = ['test']
 
 
 CLASSIFIERS = [
     'Development Status :: 3 - Alpha',
     'Environment :: Console',
@@ -22,15 +22,18 @@
     name="goobie",
     version=VERSION,
     author="Erasmus A. Junior",
     author_email="eirasmx@pm.me",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     licence='GNU LGPLv3',
-    packages=['goobie/stubs'],
-    package_data={'goobie/stubs': ['__init__.pyi', 'core.pyi', 'handler.pyi']},
+    packages=['goobie', 'goobie/utils','goobie/stubs'],
+    package_data={
+        'goobie/stubs': ['__init__.pyi', 'core.pyi', 'handler.pyi'],
+        'goobie/utils': ['__init__.py', 'handler.py'],
+        'goobie': ['core.py', '__init__.py']
+                  },
     python_requires='>=3.7',
     keywords=KEYWORDS,
     classifiers=CLASSIFIERS,
     py_modules=['goobie'],
 )
-
```

