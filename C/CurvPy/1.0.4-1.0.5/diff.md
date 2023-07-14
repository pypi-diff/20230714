# Comparing `tmp/CurvPy-1.0.4.tar.gz` & `tmp/CurvPy-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CurvPy-1.0.4.tar", last modified: Wed Jul  5 19:21:44 2023, max compression
+gzip compressed data, was "CurvPy-1.0.5.tar", last modified: Fri Jul 14 14:05:35 2023, max compression
```

## Comparing `CurvPy-1.0.4.tar` & `CurvPy-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 19:21:44.729824 CurvPy-1.0.4/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 19:21:44.719824 CurvPy-1.0.4/CurvPy.egg-info/
--rw-r--r--   0 root         (0) root         (0)      209 2023-07-05 19:21:44.000000 CurvPy-1.0.4/CurvPy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      193 2023-07-05 19:21:44.000000 CurvPy-1.0.4/CurvPy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 19:21:44.000000 CurvPy-1.0.4/CurvPy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       36 2023-07-05 19:21:44.000000 CurvPy-1.0.4/CurvPy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-05 19:21:44.000000 CurvPy-1.0.4/CurvPy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      209 2023-07-05 19:21:44.719824 CurvPy-1.0.4/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 19:21:44.719824 CurvPy-1.0.4/curvpy/
--rw-r--r--   0 root         (0) root         (0)       91 2023-07-05 19:13:20.000000 CurvPy-1.0.4/curvpy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8078 2023-07-05 19:20:26.000000 CurvPy-1.0.4/curvpy/curvpy.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 19:21:44.729824 CurvPy-1.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      347 2023-07-05 19:20:46.000000 CurvPy-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 14:05:35.447723 CurvPy-1.0.5/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 14:05:35.447723 CurvPy-1.0.5/CurvPy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      209 2023-07-14 14:05:35.000000 CurvPy-1.0.5/CurvPy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      203 2023-07-14 14:05:35.000000 CurvPy-1.0.5/CurvPy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 14:05:35.000000 CurvPy-1.0.5/CurvPy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-07-14 14:05:35.000000 CurvPy-1.0.5/CurvPy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-14 14:05:35.000000 CurvPy-1.0.5/CurvPy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      209 2023-07-14 14:05:35.447723 CurvPy-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5143 2023-07-14 14:01:17.000000 CurvPy-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 14:05:35.447723 CurvPy-1.0.5/curvpy/
+-rw-r--r--   0 root         (0) root         (0)       91 2023-07-05 19:13:20.000000 CurvPy-1.0.5/curvpy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8078 2023-07-05 19:20:26.000000 CurvPy-1.0.5/curvpy/curvpy.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 14:05:35.447723 CurvPy-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      347 2023-07-14 14:04:25.000000 CurvPy-1.0.5/setup.py
```

### Comparing `CurvPy-1.0.4/curvpy/curvpy.py` & `CurvPy-1.0.5/curvpy/curvpy.py`

 * *Files identical despite different names*

