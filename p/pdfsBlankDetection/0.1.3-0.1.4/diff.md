# Comparing `tmp/pdfsBlankDetection-0.1.3.tar.gz` & `tmp/pdfsBlankDetection-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfsBlankDetection-0.1.3.tar", last modified: Wed Jul  5 03:38:04 2023, max compression
+gzip compressed data, was "pdfsBlankDetection-0.1.4.tar", last modified: Fri Jul 14 02:02:38 2023, max compression
```

## Comparing `pdfsBlankDetection-0.1.3.tar` & `pdfsBlankDetection-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 03:38:04.082728 pdfsBlankDetection-0.1.3/
--rw-rw-rw-   0        0        0       19 2023-07-05 02:27:45.000000 pdfsBlankDetection-0.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 pdfsBlankDetection-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0      410 2023-07-05 03:38:04.082728 pdfsBlankDetection-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       30 2023-07-05 02:45:05.000000 pdfsBlankDetection-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-05 03:38:04.066730 pdfsBlankDetection-0.1.3/pdfsBlankDetection/
--rw-rw-rw-   0        0        0        0 2023-06-25 05:47:26.000000 pdfsBlankDetection-0.1.3/pdfsBlankDetection/__init__.py
--rw-rw-rw-   0        0        0   109056 2023-07-05 03:27:35.000000 pdfsBlankDetection-0.1.3/pdfsBlankDetection/pdf_blank_detection_f.pyd
--rw-rw-rw-   0        0        0    66560 2023-07-05 03:27:42.000000 pdfsBlankDetection-0.1.3/pdfsBlankDetection/pdf_blank_detection_ui.pyd
--rw-rw-rw-   0        0        0   102400 2023-07-05 03:37:10.000000 pdfsBlankDetection-0.1.3/pdfsBlankDetection/pdfsBlankDetection.pyd
-drwxrwxrwx   0        0        0        0 2023-07-05 03:38:04.080728 pdfsBlankDetection-0.1.3/pdfsBlankDetection.egg-info/
--rw-rw-rw-   0        0        0      410 2023-07-05 03:38:03.000000 pdfsBlankDetection-0.1.3/pdfsBlankDetection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      384 2023-07-05 03:38:04.000000 pdfsBlankDetection-0.1.3/pdfsBlankDetection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 03:38:03.000000 pdfsBlankDetection-0.1.3/pdfsBlankDetection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-05 03:38:03.000000 pdfsBlankDetection-0.1.3/pdfsBlankDetection.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      136 2023-07-05 03:38:04.085731 pdfsBlankDetection-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1028 2023-07-05 03:37:15.000000 pdfsBlankDetection-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 02:02:38.145462 pdfsBlankDetection-0.1.4/
+-rw-rw-rw-   0        0        0       19 2023-07-05 02:27:45.000000 pdfsBlankDetection-0.1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 pdfsBlankDetection-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      410 2023-07-14 02:02:38.145462 pdfsBlankDetection-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2023-07-05 02:45:05.000000 pdfsBlankDetection-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 02:02:38.122460 pdfsBlankDetection-0.1.4/pdfsBlankDetection/
+-rw-rw-rw-   0        0        0        0 2023-06-25 05:47:26.000000 pdfsBlankDetection-0.1.4/pdfsBlankDetection/__init__.py
+-rw-rw-rw-   0        0        0   110080 2023-07-14 01:34:39.000000 pdfsBlankDetection-0.1.4/pdfsBlankDetection/pdf_blank_detection_f.pyd
+-rw-rw-rw-   0        0        0    79360 2023-07-14 01:34:43.000000 pdfsBlankDetection-0.1.4/pdfsBlankDetection/pdf_blank_detection_ui_v2.pyd
+-rw-rw-rw-   0        0        0    44032 2023-07-14 01:34:47.000000 pdfsBlankDetection-0.1.4/pdfsBlankDetection/pdf_blank_detection_ui_v2_result_windows2.pyd
+-rw-rw-rw-   0        0        0   115200 2023-07-14 01:34:34.000000 pdfsBlankDetection-0.1.4/pdfsBlankDetection/pdfsBlankDetection.pyd
+drwxrwxrwx   0        0        0        0 2023-07-14 02:02:38.141460 pdfsBlankDetection-0.1.4/pdfsBlankDetection.egg-info/
+-rw-rw-rw-   0        0        0      410 2023-07-14 02:02:38.000000 pdfsBlankDetection-0.1.4/pdfsBlankDetection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      452 2023-07-14 02:02:38.000000 pdfsBlankDetection-0.1.4/pdfsBlankDetection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 02:02:38.000000 pdfsBlankDetection-0.1.4/pdfsBlankDetection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-14 02:02:38.000000 pdfsBlankDetection-0.1.4/pdfsBlankDetection.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      136 2023-07-14 02:02:38.147462 pdfsBlankDetection-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1028 2023-07-14 02:01:07.000000 pdfsBlankDetection-0.1.4/setup.py
```

### Comparing `pdfsBlankDetection-0.1.3/setup.py` & `pdfsBlankDetection-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 1
-PATCH = 3
+PATCH = 4
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "pdfsBlankDetection",
```

