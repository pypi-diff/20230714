# Comparing `tmp/py4web-debug-tools-0.2.1.tar.gz` & `tmp/py4web-debug-tools-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py4web-debug-tools-0.2.1.tar", last modified: Thu Mar 23 14:07:54 2023, max compression
+gzip compressed data, was "py4web-debug-tools-0.2.2.tar", last modified: Fri Jul 14 13:59:15 2023, max compression
```

## Comparing `py4web-debug-tools-0.2.1.tar` & `py4web-debug-tools-0.2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-23 14:07:54.379701 py4web-debug-tools-0.2.1/
--rw-rw-r--   0 robin     (1000) robin     (1000)     3687 2023-03-23 14:07:54.379701 py4web-debug-tools-0.2.1/PKG-INFO
--rw-rw-r--   0 robin     (1000) robin     (1000)     3393 2023-03-02 16:27:24.000000 py4web-debug-tools-0.2.1/README.md
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-23 14:07:54.379701 py4web-debug-tools-0.2.1/py4web_debug/
--rw-rw-r--   0 robin     (1000) robin     (1000)      131 2023-03-02 15:39:55.000000 py4web-debug-tools-0.2.1/py4web_debug/__init__.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     3073 2023-03-23 14:06:41.000000 py4web-debug-tools-0.2.1/py4web_debug/core.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     7232 2023-03-23 14:06:31.000000 py4web-debug-tools-0.2.1/py4web_debug/debugbar.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     3496 2023-02-21 12:42:44.000000 py4web-debug-tools-0.2.1/py4web_debug/dumping.py
--rw-rw-r--   0 robin     (1000) robin     (1000)       82 2023-02-21 11:17:08.000000 py4web-debug-tools-0.2.1/py4web_debug/env.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     4316 2023-03-02 16:15:42.000000 py4web-debug-tools-0.2.1/py4web_debug/internals.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-23 14:07:54.379701 py4web-debug-tools-0.2.1/py4web_debug/templates/
--rw-rw-r--   0 robin     (1000) robin     (1000)     7169 2023-03-23 14:06:31.000000 py4web-debug-tools-0.2.1/py4web_debug/templates/debugbar.html
--rw-rw-r--   0 robin     (1000) robin     (1000)       60 2023-02-21 12:22:35.000000 py4web-debug-tools-0.2.1/py4web_debug/templates/dumpdie.html
--rw-rw-r--   0 robin     (1000) robin     (1000)      868 2023-02-21 12:22:15.000000 py4web-debug-tools-0.2.1/py4web_debug/templates/error_default.html
--rw-rw-r--   0 robin     (1000) robin     (1000)      532 2023-02-21 12:23:06.000000 py4web-debug-tools-0.2.1/py4web_debug/templates/fancy_dumpdie.html
--rw-rw-r--   0 robin     (1000) robin     (1000)      207 2023-03-02 15:42:15.000000 py4web-debug-tools-0.2.1/py4web_debug/wsgi.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-23 14:07:54.379701 py4web-debug-tools-0.2.1/py4web_debug_tools.egg-info/
--rw-rw-r--   0 robin     (1000) robin     (1000)     3687 2023-03-23 14:07:54.000000 py4web-debug-tools-0.2.1/py4web_debug_tools.egg-info/PKG-INFO
--rw-rw-r--   0 robin     (1000) robin     (1000)      546 2023-03-23 14:07:54.000000 py4web-debug-tools-0.2.1/py4web_debug_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)        1 2023-03-23 14:07:54.000000 py4web-debug-tools-0.2.1/py4web_debug_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)       36 2023-03-23 14:07:54.000000 py4web-debug-tools-0.2.1/py4web_debug_tools.egg-info/requires.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)       13 2023-03-23 14:07:54.000000 py4web-debug-tools-0.2.1/py4web_debug_tools.egg-info/top_level.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)       38 2023-03-23 14:07:54.379701 py4web-debug-tools-0.2.1/setup.cfg
--rw-rw-r--   0 robin     (1000) robin     (1000)      671 2023-03-23 14:07:16.000000 py4web-debug-tools-0.2.1/setup.py
+drwxrwxr-x   0 eddie     (1001) eddie     (1001)        0 2023-07-14 13:59:15.885692 py4web-debug-tools-0.2.2/
+-rw-rw-r--   0 eddie     (1001) eddie     (1001)     3687 2023-07-14 13:59:15.881692 py4web-debug-tools-0.2.2/PKG-INFO
+-rw-rw-r--   0 eddie     (1001) eddie     (1001)     3393 2023-07-14 13:53:10.000000 py4web-debug-tools-0.2.2/README.md
+drwxrwxr-x   0 eddie     (1001) eddie     (1001)        0 2023-07-14 13:59:15.881692 py4web-debug-tools-0.2.2/py4web_debug/
+-rw-rw-r--   0 eddie     (1001) eddie     (1001)      157 2023-07-14 13:53:47.000000 py4web-debug-tools-0.2.2/py4web_debug/__init__.py
+-rw-rw-r--   0 eddie     (1001) eddie     (1001)     3073 2023-07-14 13:53:10.000000 py4web-debug-tools-0.2.2/py4web_debug/core.py
+-rw-rw-r--   0 eddie     (1001) eddie     (1001)     7232 2023-07-14 13:53:10.000000 py4web-debug-tools-0.2.2/py4web_debug/debugbar.py
+-rw-rw-r--   0 eddie     (1001) eddie     (1001)     3496 2023-07-14 13:53:10.000000 py4web-debug-tools-0.2.2/py4web_debug/dumping.py
+-rw-rw-r--   0 eddie     (1001) eddie     (1001)       82 2023-07-14 13:53:10.000000 py4web-debug-tools-0.2.2/py4web_debug/env.py
+-rw-rw-r--   0 eddie     (1001) eddie     (1001)     4316 2023-07-14 13:53:10.000000 py4web-debug-tools-0.2.2/py4web_debug/internals.py
+drwxrwxr-x   0 eddie     (1001) eddie     (1001)        0 2023-07-14 13:59:15.881692 py4web-debug-tools-0.2.2/py4web_debug/templates/
+-rw-rw-r--   0 eddie     (1001) eddie     (1001)     7169 2023-07-14 13:53:10.000000 py4web-debug-tools-0.2.2/py4web_debug/templates/debugbar.html
+-rw-rw-r--   0 eddie     (1001) eddie     (1001)       60 2023-07-14 13:53:10.000000 py4web-debug-tools-0.2.2/py4web_debug/templates/dumpdie.html
+-rw-rw-r--   0 eddie     (1001) eddie     (1001)      868 2023-07-14 13:53:10.000000 py4web-debug-tools-0.2.2/py4web_debug/templates/error_default.html
+-rw-rw-r--   0 eddie     (1001) eddie     (1001)      532 2023-07-14 13:53:10.000000 py4web-debug-tools-0.2.2/py4web_debug/templates/fancy_dumpdie.html
+-rw-rw-r--   0 eddie     (1001) eddie     (1001)      207 2023-07-14 13:53:10.000000 py4web-debug-tools-0.2.2/py4web_debug/wsgi.py
+drwxrwxr-x   0 eddie     (1001) eddie     (1001)        0 2023-07-14 13:59:15.881692 py4web-debug-tools-0.2.2/py4web_debug_tools.egg-info/
+-rw-rw-r--   0 eddie     (1001) eddie     (1001)     3687 2023-07-14 13:59:15.000000 py4web-debug-tools-0.2.2/py4web_debug_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 eddie     (1001) eddie     (1001)      546 2023-07-14 13:59:15.000000 py4web-debug-tools-0.2.2/py4web_debug_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 eddie     (1001) eddie     (1001)        1 2023-07-14 13:59:15.000000 py4web-debug-tools-0.2.2/py4web_debug_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 eddie     (1001) eddie     (1001)       36 2023-07-14 13:59:15.000000 py4web-debug-tools-0.2.2/py4web_debug_tools.egg-info/requires.txt
+-rw-rw-r--   0 eddie     (1001) eddie     (1001)       13 2023-07-14 13:59:15.000000 py4web-debug-tools-0.2.2/py4web_debug_tools.egg-info/top_level.txt
+-rw-rw-r--   0 eddie     (1001) eddie     (1001)       38 2023-07-14 13:59:15.885692 py4web-debug-tools-0.2.2/setup.cfg
+-rw-rw-r--   0 eddie     (1001) eddie     (1001)      671 2023-07-14 13:54:29.000000 py4web-debug-tools-0.2.2/setup.py
```

### Comparing `py4web-debug-tools-0.2.1/PKG-INFO` & `py4web-debug-tools-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py4web-debug-tools
-Version: 0.2.1
+Version: 0.2.2
 Summary: Debug Tools for py4web
 Home-page: https://github.com/trialandsuccess/py4web-debug-tools
 Author: Robin van der Noord
 Author-email: contact@trialandsuccess.nl
 Requires-Python: >3.10.0
 Description-Content-Type: text/markdown
```

### Comparing `py4web-debug-tools-0.2.1/README.md` & `py4web-debug-tools-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `py4web-debug-tools-0.2.1/py4web_debug/core.py` & `py4web-debug-tools-0.2.2/py4web_debug/core.py`

 * *Files identical despite different names*

### Comparing `py4web-debug-tools-0.2.1/py4web_debug/debugbar.py` & `py4web-debug-tools-0.2.2/py4web_debug/debugbar.py`

 * *Files identical despite different names*

### Comparing `py4web-debug-tools-0.2.1/py4web_debug/dumping.py` & `py4web-debug-tools-0.2.2/py4web_debug/dumping.py`

 * *Files identical despite different names*

### Comparing `py4web-debug-tools-0.2.1/py4web_debug/internals.py` & `py4web-debug-tools-0.2.2/py4web_debug/internals.py`

 * *Files identical despite different names*

### Comparing `py4web-debug-tools-0.2.1/py4web_debug/templates/debugbar.html` & `py4web-debug-tools-0.2.2/py4web_debug/templates/debugbar.html`

 * *Files identical despite different names*

### Comparing `py4web-debug-tools-0.2.1/py4web_debug/templates/error_default.html` & `py4web-debug-tools-0.2.2/py4web_debug/templates/error_default.html`

 * *Files identical despite different names*

### Comparing `py4web-debug-tools-0.2.1/py4web_debug/templates/fancy_dumpdie.html` & `py4web-debug-tools-0.2.2/py4web_debug/templates/fancy_dumpdie.html`

 * *Files identical despite different names*

### Comparing `py4web-debug-tools-0.2.1/py4web_debug_tools.egg-info/PKG-INFO` & `py4web-debug-tools-0.2.2/py4web_debug_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py4web-debug-tools
-Version: 0.2.1
+Version: 0.2.2
 Summary: Debug Tools for py4web
 Home-page: https://github.com/trialandsuccess/py4web-debug-tools
 Author: Robin van der Noord
 Author-email: contact@trialandsuccess.nl
 Requires-Python: >3.10.0
 Description-Content-Type: text/markdown
```

### Comparing `py4web-debug-tools-0.2.1/py4web_debug_tools.egg-info/SOURCES.txt` & `py4web-debug-tools-0.2.2/py4web_debug_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py4web-debug-tools-0.2.1/setup.py` & `py4web-debug-tools-0.2.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md") as f:
     long_desc = f.read()
 
 dependencies = ["py4web", "yatl", "pydal", "configurable-json"]
 
 setup(
     name="py4web-debug-tools",
-    version="0.2.1",
+    version="0.2.2",
     description="Debug Tools for py4web",
     author="Robin van der Noord",
     author_email="contact@trialandsuccess.nl",
     url="https://github.com/trialandsuccess/py4web-debug-tools",
     packages=["py4web_debug"],
     include_package_data=True,
     package_data={"py4web_debug": ["templates/*.html"]},
```

