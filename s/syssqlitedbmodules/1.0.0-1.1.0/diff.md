# Comparing `tmp/syssqlitedbmodules-1.0.0.tar.gz` & `tmp/syssqlitedbmodules-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syssqlitedbmodules-1.0.0.tar", last modified: Fri Jul 14 18:44:36 2023, max compression
+gzip compressed data, was "syssqlitedbmodules-1.1.0.tar", last modified: Fri Jul 14 18:46:41 2023, max compression
```

## Comparing `syssqlitedbmodules-1.0.0.tar` & `syssqlitedbmodules-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:44:36.202010 syssqlitedbmodules-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      351 2023-07-14 18:44:36.202010 syssqlitedbmodules-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 18:44:36.202010 syssqlitedbmodules-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      564 2023-07-14 18:44:35.000000 syssqlitedbmodules-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:44:36.202010 syssqlitedbmodules-1.0.0/syssqlitedbmodules/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-14 18:44:35.000000 syssqlitedbmodules-1.0.0/syssqlitedbmodules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:44:36.202010 syssqlitedbmodules-1.0.0/syssqlitedbmodules.egg-info/
--rw-r--r--   0 root         (0) root         (0)      351 2023-07-14 18:44:36.000000 syssqlitedbmodules-1.0.0/syssqlitedbmodules.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      207 2023-07-14 18:44:36.000000 syssqlitedbmodules-1.0.0/syssqlitedbmodules.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 18:44:36.000000 syssqlitedbmodules-1.0.0/syssqlitedbmodules.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-07-14 18:44:36.000000 syssqlitedbmodules-1.0.0/syssqlitedbmodules.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:46:41.289607 syssqlitedbmodules-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      351 2023-07-14 18:46:41.289607 syssqlitedbmodules-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 18:46:41.289607 syssqlitedbmodules-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      564 2023-07-14 18:46:40.000000 syssqlitedbmodules-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:46:41.289607 syssqlitedbmodules-1.1.0/syssqlitedbmodules/
+-rw-r--r--   0 root         (0) root         (0)    96773 2023-07-14 18:46:40.000000 syssqlitedbmodules-1.1.0/syssqlitedbmodules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:46:41.289607 syssqlitedbmodules-1.1.0/syssqlitedbmodules.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      351 2023-07-14 18:46:41.000000 syssqlitedbmodules-1.1.0/syssqlitedbmodules.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      207 2023-07-14 18:46:41.000000 syssqlitedbmodules-1.1.0/syssqlitedbmodules.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 18:46:41.000000 syssqlitedbmodules-1.1.0/syssqlitedbmodules.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-14 18:46:41.000000 syssqlitedbmodules-1.1.0/syssqlitedbmodules.egg-info/top_level.txt
```

### Comparing `syssqlitedbmodules-1.0.0/setup.py` & `syssqlitedbmodules-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="syssqlitedbmodules",
     version=VERSION,
```

