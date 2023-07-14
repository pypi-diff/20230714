# Comparing `tmp/VGPY-1.0.0.tar.gz` & `tmp/VGPY-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VGPY-1.0.0.tar", last modified: Fri Jul 14 05:23:03 2023, max compression
+gzip compressed data, was "VGPY-1.0.1.tar", last modified: Fri Jul 14 07:13:48 2023, max compression
```

## Comparing `VGPY-1.0.0.tar` & `VGPY-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,12 @@
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-14 05:23:03.849782 VGPY-1.0.0/
--rw-r--r--   0 jan        (501) staff       (20)      268 2023-07-14 05:23:03.849530 VGPY-1.0.0/PKG-INFO
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-14 05:23:03.849175 VGPY-1.0.0/VGPY.egg-info/
--rw-r--r--   0 jan        (501) staff       (20)      268 2023-07-14 05:23:03.000000 VGPY-1.0.0/VGPY.egg-info/PKG-INFO
--rw-r--r--   0 jan        (501) staff       (20)      120 2023-07-14 05:23:03.000000 VGPY-1.0.0/VGPY.egg-info/SOURCES.txt
--rw-r--r--   0 jan        (501) staff       (20)        1 2023-07-14 05:23:03.000000 VGPY-1.0.0/VGPY.egg-info/dependency_links.txt
--rw-r--r--   0 jan        (501) staff       (20)        1 2023-07-14 05:23:03.000000 VGPY-1.0.0/VGPY.egg-info/top_level.txt
--rw-r--r--   0 jan        (501) staff       (20)       38 2023-07-14 05:23:03.849861 VGPY-1.0.0/setup.cfg
--rw-r--r--   0 jan        (501) staff       (20)      522 2023-07-14 03:55:23.000000 VGPY-1.0.0/setup.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-14 07:13:48.389458 VGPY-1.0.1/
+-rw-r--r--   0 jan        (501) staff       (20)      268 2023-07-14 07:13:48.389200 VGPY-1.0.1/PKG-INFO
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-14 07:13:48.387182 VGPY-1.0.1/VGPY/
+-rw-r--r--   0 jan        (501) staff       (20)       28 2023-07-14 07:12:13.000000 VGPY-1.0.1/VGPY/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)     1848 2023-07-13 12:55:09.000000 VGPY-1.0.1/VGPY/vango_openapi.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-07-14 07:13:48.388772 VGPY-1.0.1/VGPY.egg-info/
+-rw-r--r--   0 jan        (501) staff       (20)      268 2023-07-14 07:13:48.000000 VGPY-1.0.1/VGPY.egg-info/PKG-INFO
+-rw-r--r--   0 jan        (501) staff       (20)      159 2023-07-14 07:13:48.000000 VGPY-1.0.1/VGPY.egg-info/SOURCES.txt
+-rw-r--r--   0 jan        (501) staff       (20)        1 2023-07-14 07:13:48.000000 VGPY-1.0.1/VGPY.egg-info/dependency_links.txt
+-rw-r--r--   0 jan        (501) staff       (20)        5 2023-07-14 07:13:48.000000 VGPY-1.0.1/VGPY.egg-info/top_level.txt
+-rw-r--r--   0 jan        (501) staff       (20)       38 2023-07-14 07:13:48.389590 VGPY-1.0.1/setup.cfg
+-rw-r--r--   0 jan        (501) staff       (20)      522 2023-07-14 07:13:44.000000 VGPY-1.0.1/setup.py
```

### Comparing `VGPY-1.0.0/setup.py` & `VGPY-1.0.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 
 from setuptools import setup, find_packages
 
 setup(
     name='VGPY',
-    version='1.0.0',
+    version='1.0.1',
     description='van_go open api',
     author='JanVee',
     author_email='814107539@qq.com',
     packages=find_packages(),
     install_requires=[],
     keywords = ("vango", "VGPY"),
     long_description = "An feature extraction algorithm, van_go open api",
```

