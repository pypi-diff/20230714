# Comparing `tmp/bw_libs-0.1.0.tar.gz` & `tmp/bw_libs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw_libs-0.1.0.tar", last modified: Thu Jul 13 19:37:53 2023, max compression
+gzip compressed data, was "bw_libs-0.1.1.tar", last modified: Fri Jul 14 07:52:59 2023, max compression
```

## Comparing `bw_libs-0.1.0.tar` & `bw_libs-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2023-07-13 19:37:53.146793 bw_libs-0.1.0/
--rw-r--r--   0 admin      (502) staff       (20)     1067 2021-03-30 20:46:26.000000 bw_libs-0.1.0/LICENSE
--rw-r--r--   0 admin      (502) staff       (20)     1283 2023-07-13 19:37:53.146505 bw_libs-0.1.0/PKG-INFO
--rw-r--r--   0 admin      (502) staff       (20)      798 2023-07-13 19:27:37.000000 bw_libs-0.1.0/README.md
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2023-07-13 19:37:53.143908 bw_libs-0.1.0/bw_libs/
--rw-r--r--   0 admin      (502) staff       (20)       29 2023-07-13 19:35:20.000000 bw_libs-0.1.0/bw_libs/__init__.py
--rw-r--r--   0 admin      (502) staff       (20)       31 2023-07-13 19:32:56.000000 bw_libs-0.1.0/bw_libs/main.py
-drwxr-xr-x   0 admin      (502) staff       (20)        0 2023-07-13 19:37:53.145978 bw_libs-0.1.0/bw_libs.egg-info/
--rw-r--r--   0 admin      (502) staff       (20)     1283 2023-07-13 19:37:53.000000 bw_libs-0.1.0/bw_libs.egg-info/PKG-INFO
--rw-r--r--   0 admin      (502) staff       (20)      186 2023-07-13 19:37:53.000000 bw_libs-0.1.0/bw_libs.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (502) staff       (20)        1 2023-07-13 19:37:53.000000 bw_libs-0.1.0/bw_libs.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (502) staff       (20)        8 2023-07-13 19:37:53.000000 bw_libs-0.1.0/bw_libs.egg-info/top_level.txt
--rw-r--r--   0 admin      (502) staff       (20)       38 2023-07-13 19:37:53.146938 bw_libs-0.1.0/setup.cfg
--rw-r--r--   0 admin      (502) staff       (20)      944 2023-07-13 19:37:25.000000 bw_libs-0.1.0/setup.py
+drwxr-xr-x   0 admin      (502) staff       (20)        0 2023-07-14 07:52:59.985014 bw_libs-0.1.1/
+-rw-r--r--   0 admin      (502) staff       (20)     1067 2021-03-30 20:46:26.000000 bw_libs-0.1.1/LICENSE
+-rw-r--r--   0 admin      (502) staff       (20)     1283 2023-07-14 07:52:59.984747 bw_libs-0.1.1/PKG-INFO
+-rw-r--r--   0 admin      (502) staff       (20)      798 2023-07-13 19:27:37.000000 bw_libs-0.1.1/README.md
+drwxr-xr-x   0 admin      (502) staff       (20)        0 2023-07-14 07:52:59.982119 bw_libs-0.1.1/bw_libs/
+-rw-r--r--   0 admin      (502) staff       (20)       29 2023-07-13 19:35:20.000000 bw_libs-0.1.1/bw_libs/__init__.py
+-rw-r--r--   0 admin      (502) staff       (20)      180 2023-07-14 07:51:04.000000 bw_libs-0.1.1/bw_libs/main.py
+drwxr-xr-x   0 admin      (502) staff       (20)        0 2023-07-14 07:52:59.984265 bw_libs-0.1.1/bw_libs.egg-info/
+-rw-r--r--   0 admin      (502) staff       (20)     1283 2023-07-14 07:52:59.000000 bw_libs-0.1.1/bw_libs.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (502) staff       (20)      216 2023-07-14 07:52:59.000000 bw_libs-0.1.1/bw_libs.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (502) staff       (20)        1 2023-07-14 07:52:59.000000 bw_libs-0.1.1/bw_libs.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (502) staff       (20)        9 2023-07-14 07:52:59.000000 bw_libs-0.1.1/bw_libs.egg-info/requires.txt
+-rw-r--r--   0 admin      (502) staff       (20)        8 2023-07-14 07:52:59.000000 bw_libs-0.1.1/bw_libs.egg-info/top_level.txt
+-rw-r--r--   0 admin      (502) staff       (20)       38 2023-07-14 07:52:59.985131 bw_libs-0.1.1/setup.cfg
+-rw-r--r--   0 admin      (502) staff       (20)      954 2023-07-14 07:52:58.000000 bw_libs-0.1.1/setup.py
```

### Comparing `bw_libs-0.1.0/LICENSE` & `bw_libs-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bw_libs-0.1.0/PKG-INFO` & `bw_libs-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw_libs
-Version: 0.1.0
+Version: 0.1.1
 Summary: DESCRIPTION
 Author: Sargis
 Author-email: <sargis@bridgewise.com>
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bw_libs-0.1.0/README.md` & `bw_libs-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `bw_libs-0.1.0/bw_libs.egg-info/PKG-INFO` & `bw_libs-0.1.1/bw_libs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw-libs
-Version: 0.1.0
+Version: 0.1.1
 Summary: DESCRIPTION
 Author: Sargis
 Author-email: <sargis@bridgewise.com>
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bw_libs-0.1.0/setup.py` & `bw_libs-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 DESCRIPTION = 'DESCRIPTION'
 LONG_DESCRIPTION = 'LONG_DESCRIPTION'
 
 # Setting up
 setup(
     name="bw_libs",
     version=VERSION,
     author="Sargis",
     author_email="<sargis@bridgewise.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=[],
+    install_requires=['pydantic'],
     keywords=['python'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

