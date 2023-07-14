# Comparing `tmp/percy-selenium-2.0.0a0.tar.gz` & `tmp/percy-selenium-2.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "percy-selenium-2.0.0a0.tar", last modified: Mon Jul  3 13:57:04 2023, max compression
+gzip compressed data, was "percy-selenium-2.0.0b0.tar", last modified: Fri Jul 14 14:22:34 2023, max compression
```

## Comparing `percy-selenium-2.0.0a0.tar` & `percy-selenium-2.0.0b0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:57:04.629859 percy-selenium-2.0.0a0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-03 13:56:39.000000 percy-selenium-2.0.0a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-03 13:57:04.629859 percy-selenium-2.0.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-03 13:56:39.000000 percy-selenium-2.0.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:57:04.629859 percy-selenium-2.0.0a0/percy/
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-03 13:56:39.000000 percy-selenium-2.0.0a0/percy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-03 13:56:39.000000 percy-selenium-2.0.0a0/percy/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-07-03 13:56:39.000000 percy-selenium-2.0.0a0/percy/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-03 13:56:39.000000 percy-selenium-2.0.0a0/percy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:57:04.629859 percy-selenium-2.0.0a0/percy_selenium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-03 13:57:04.000000 percy-selenium-2.0.0a0/percy_selenium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-03 13:57:04.000000 percy-selenium-2.0.0a0/percy_selenium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 13:57:04.000000 percy-selenium-2.0.0a0/percy_selenium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 13:57:04.000000 percy-selenium-2.0.0a0/percy_selenium.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 13:57:04.000000 percy-selenium-2.0.0a0/percy_selenium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-03 13:57:04.000000 percy-selenium-2.0.0a0/percy_selenium.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 13:57:04.629859 percy-selenium-2.0.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-03 13:56:39.000000 percy-selenium-2.0.0a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:57:04.629859 percy-selenium-2.0.0a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13135 2023-07-03 13:56:39.000000 percy-selenium-2.0.0a0/tests/test_snapshot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:22:34.912308 percy-selenium-2.0.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-14 14:22:07.000000 percy-selenium-2.0.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-14 14:22:34.912308 percy-selenium-2.0.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-14 14:22:07.000000 percy-selenium-2.0.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:22:34.912308 percy-selenium-2.0.0b0/percy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-14 14:22:07.000000 percy-selenium-2.0.0b0/percy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-14 14:22:07.000000 percy-selenium-2.0.0b0/percy/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-07-14 14:22:07.000000 percy-selenium-2.0.0b0/percy/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-14 14:22:07.000000 percy-selenium-2.0.0b0/percy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:22:34.912308 percy-selenium-2.0.0b0/percy_selenium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-14 14:22:34.000000 percy-selenium-2.0.0b0/percy_selenium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-14 14:22:34.000000 percy-selenium-2.0.0b0/percy_selenium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 14:22:34.000000 percy-selenium-2.0.0b0/percy_selenium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 14:22:34.000000 percy-selenium-2.0.0b0/percy_selenium.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-14 14:22:34.000000 percy-selenium-2.0.0b0/percy_selenium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 14:22:34.000000 percy-selenium-2.0.0b0/percy_selenium.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 14:22:34.912308 percy-selenium-2.0.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-14 14:22:07.000000 percy-selenium-2.0.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:22:34.912308 percy-selenium-2.0.0b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13135 2023-07-14 14:22:07.000000 percy-selenium-2.0.0b0/tests/test_snapshot.py
```

### Comparing `percy-selenium-2.0.0a0/LICENSE` & `percy-selenium-2.0.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `percy-selenium-2.0.0a0/PKG-INFO` & `percy-selenium-2.0.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: percy-selenium
-Version: 2.0.0a0
+Version: 2.0.0b0
 Summary: Python client for visual testing with Percy
 Home-page: https://github.com/percy/percy-selenium-python
 Author: Perceptual Inc.
 Author-email: team@percy.io
 License: MIT
 Keywords: selenium percy visual testing
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `percy-selenium-2.0.0a0/README.md` & `percy-selenium-2.0.0b0/README.md`

 * *Files identical despite different names*

### Comparing `percy-selenium-2.0.0a0/percy/__init__.py` & `percy-selenium-2.0.0b0/percy/__init__.py`

 * *Files identical despite different names*

### Comparing `percy-selenium-2.0.0a0/percy/snapshot.py` & `percy-selenium-2.0.0b0/percy/snapshot.py`

 * *Files identical despite different names*

### Comparing `percy-selenium-2.0.0a0/percy_selenium.egg-info/PKG-INFO` & `percy-selenium-2.0.0b0/percy_selenium.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: percy-selenium
-Version: 2.0.0a0
+Version: 2.0.0b0
 Summary: Python client for visual testing with Percy
 Home-page: https://github.com/percy/percy-selenium-python
 Author: Perceptual Inc.
 Author-email: team@percy.io
 License: MIT
 Keywords: selenium percy visual testing
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `percy-selenium-2.0.0a0/setup.py` & `percy-selenium-2.0.0b0/setup.py`

 * *Files identical despite different names*

### Comparing `percy-selenium-2.0.0a0/tests/test_snapshot.py` & `percy-selenium-2.0.0b0/tests/test_snapshot.py`

 * *Files identical despite different names*

