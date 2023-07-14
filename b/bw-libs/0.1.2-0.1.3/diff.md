# Comparing `tmp/bw_libs-0.1.2.tar.gz` & `tmp/bw_libs-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw_libs-0.1.2.tar", last modified: Fri Jul 14 07:55:08 2023, max compression
+gzip compressed data, was "bw_libs-0.1.3.tar", last modified: Fri Jul 14 07:56:26 2023, max compression
```

## Comparing `bw_libs-0.1.2.tar` & `bw_libs-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2023-07-14 07:55:08.605009 bw_libs-0.1.2/
--rw-r--r--   0 admin      (502) staff       (20)     1067 2021-03-30 20:46:26.000000 bw_libs-0.1.2/LICENSE
--rw-r--r--   0 admin      (502) staff       (20)     1283 2023-07-14 07:55:08.604706 bw_libs-0.1.2/PKG-INFO
--rw-r--r--   0 admin      (502) staff       (20)      798 2023-07-13 19:27:37.000000 bw_libs-0.1.2/README.md
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2023-07-14 07:55:08.601572 bw_libs-0.1.2/bw_libs/
--rw-r--r--   0 admin      (502) staff       (20)       71 2023-07-14 07:54:27.000000 bw_libs-0.1.2/bw_libs/__init__.py
--rw-r--r--   0 admin      (502) staff       (20)      180 2023-07-14 07:51:04.000000 bw_libs-0.1.2/bw_libs/main.py
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2023-07-14 07:55:08.604145 bw_libs-0.1.2/bw_libs.egg-info/
--rw-r--r--   0 admin      (502) staff       (20)     1283 2023-07-14 07:55:08.000000 bw_libs-0.1.2/bw_libs.egg-info/PKG-INFO
--rw-r--r--   0 admin      (502) staff       (20)      216 2023-07-14 07:55:08.000000 bw_libs-0.1.2/bw_libs.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (502) staff       (20)        1 2023-07-14 07:55:08.000000 bw_libs-0.1.2/bw_libs.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (502) staff       (20)        9 2023-07-14 07:55:08.000000 bw_libs-0.1.2/bw_libs.egg-info/requires.txt
--rw-r--r--   0 admin      (502) staff       (20)        8 2023-07-14 07:55:08.000000 bw_libs-0.1.2/bw_libs.egg-info/top_level.txt
--rw-r--r--   0 admin      (502) staff       (20)       38 2023-07-14 07:55:08.605142 bw_libs-0.1.2/setup.cfg
--rw-r--r--   0 admin      (502) staff       (20)      954 2023-07-14 07:55:05.000000 bw_libs-0.1.2/setup.py
+drwxr-xr-x   0 admin      (502) staff       (20)        0 2023-07-14 07:56:26.301741 bw_libs-0.1.3/
+-rw-r--r--   0 admin      (502) staff       (20)     1067 2021-03-30 20:46:26.000000 bw_libs-0.1.3/LICENSE
+-rw-r--r--   0 admin      (502) staff       (20)     1283 2023-07-14 07:56:26.301431 bw_libs-0.1.3/PKG-INFO
+-rw-r--r--   0 admin      (502) staff       (20)      798 2023-07-13 19:27:37.000000 bw_libs-0.1.3/README.md
+drwxr-xr-x   0 admin      (502) staff       (20)        0 2023-07-14 07:56:26.298703 bw_libs-0.1.3/bw_libs/
+-rw-r--r--   0 admin      (502) staff       (20)       70 2023-07-14 07:56:21.000000 bw_libs-0.1.3/bw_libs/__init__.py
+-rw-r--r--   0 admin      (502) staff       (20)      180 2023-07-14 07:51:04.000000 bw_libs-0.1.3/bw_libs/main.py
+drwxr-xr-x   0 admin      (502) staff       (20)        0 2023-07-14 07:56:26.300863 bw_libs-0.1.3/bw_libs.egg-info/
+-rw-r--r--   0 admin      (502) staff       (20)     1283 2023-07-14 07:56:26.000000 bw_libs-0.1.3/bw_libs.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (502) staff       (20)      216 2023-07-14 07:56:26.000000 bw_libs-0.1.3/bw_libs.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (502) staff       (20)        1 2023-07-14 07:56:26.000000 bw_libs-0.1.3/bw_libs.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (502) staff       (20)        9 2023-07-14 07:56:26.000000 bw_libs-0.1.3/bw_libs.egg-info/requires.txt
+-rw-r--r--   0 admin      (502) staff       (20)        8 2023-07-14 07:56:26.000000 bw_libs-0.1.3/bw_libs.egg-info/top_level.txt
+-rw-r--r--   0 admin      (502) staff       (20)       38 2023-07-14 07:56:26.301869 bw_libs-0.1.3/setup.cfg
+-rw-r--r--   0 admin      (502) staff       (20)      954 2023-07-14 07:56:21.000000 bw_libs-0.1.3/setup.py
```

### Comparing `bw_libs-0.1.2/LICENSE` & `bw_libs-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bw_libs-0.1.2/PKG-INFO` & `bw_libs-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw_libs
-Version: 0.1.2
+Version: 0.1.3
 Summary: DESCRIPTION
 Author: Sargis
 Author-email: <sargis@bridgewise.com>
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bw_libs-0.1.2/README.md` & `bw_libs-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `bw_libs-0.1.2/bw_libs.egg-info/PKG-INFO` & `bw_libs-0.1.3/bw_libs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw-libs
-Version: 0.1.2
+Version: 0.1.3
 Summary: DESCRIPTION
 Author: Sargis
 Author-email: <sargis@bridgewise.com>
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bw_libs-0.1.2/setup.py` & `bw_libs-0.1.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.2'
+VERSION = '0.1.3'
 DESCRIPTION = 'DESCRIPTION'
 LONG_DESCRIPTION = 'LONG_DESCRIPTION'
 
 # Setting up
 setup(
     name="bw_libs",
     version=VERSION,
```

