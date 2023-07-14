# Comparing `tmp/syscoloringsaddition-1.0.0.tar.gz` & `tmp/syscoloringsaddition-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syscoloringsaddition-1.0.0.tar", last modified: Fri Jul 14 10:36:54 2023, max compression
+gzip compressed data, was "syscoloringsaddition-1.1.0.tar", last modified: Fri Jul 14 10:39:01 2023, max compression
```

## Comparing `syscoloringsaddition-1.0.0.tar` & `syscoloringsaddition-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:36:54.663688 syscoloringsaddition-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      353 2023-07-14 10:36:54.663688 syscoloringsaddition-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 10:36:54.663688 syscoloringsaddition-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      566 2023-07-14 10:36:54.000000 syscoloringsaddition-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:36:54.663688 syscoloringsaddition-1.0.0/syscoloringsaddition/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-14 10:36:54.000000 syscoloringsaddition-1.0.0/syscoloringsaddition/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:36:54.663688 syscoloringsaddition-1.0.0/syscoloringsaddition.egg-info/
--rw-r--r--   0 root         (0) root         (0)      353 2023-07-14 10:36:54.000000 syscoloringsaddition-1.0.0/syscoloringsaddition.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      217 2023-07-14 10:36:54.000000 syscoloringsaddition-1.0.0/syscoloringsaddition.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 10:36:54.000000 syscoloringsaddition-1.0.0/syscoloringsaddition.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-14 10:36:54.000000 syscoloringsaddition-1.0.0/syscoloringsaddition.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:39:01.459342 syscoloringsaddition-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      353 2023-07-14 10:39:01.459342 syscoloringsaddition-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 10:39:01.459342 syscoloringsaddition-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      566 2023-07-14 10:39:00.000000 syscoloringsaddition-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:39:01.455342 syscoloringsaddition-1.1.0/syscoloringsaddition/
+-rw-r--r--   0 root         (0) root         (0)    96773 2023-07-14 10:39:00.000000 syscoloringsaddition-1.1.0/syscoloringsaddition/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:39:01.459342 syscoloringsaddition-1.1.0/syscoloringsaddition.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      353 2023-07-14 10:39:01.000000 syscoloringsaddition-1.1.0/syscoloringsaddition.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      217 2023-07-14 10:39:01.000000 syscoloringsaddition-1.1.0/syscoloringsaddition.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 10:39:01.000000 syscoloringsaddition-1.1.0/syscoloringsaddition.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-14 10:39:01.000000 syscoloringsaddition-1.1.0/syscoloringsaddition.egg-info/top_level.txt
```

### Comparing `syscoloringsaddition-1.0.0/setup.py` & `syscoloringsaddition-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="syscoloringsaddition",
     version=VERSION,
```

