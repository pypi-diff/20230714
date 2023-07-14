# Comparing `tmp/QRcodeTracking-0.1.1.tar.gz` & `tmp/QRcodeTracking-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QRcodeTracking-0.1.1.tar", last modified: Fri Jul 14 03:50:55 2023, max compression
+gzip compressed data, was "QRcodeTracking-0.1.2.tar", last modified: Fri Jul 14 07:31:06 2023, max compression
```

## Comparing `QRcodeTracking-0.1.1.tar` & `QRcodeTracking-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 03:50:55.187439 QRcodeTracking-0.1.1/
--rw-rw-rw-   0        0        0       19 2023-07-05 02:27:45.000000 QRcodeTracking-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 QRcodeTracking-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      373 2023-07-14 03:50:55.188401 QRcodeTracking-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-14 03:50:55.164399 QRcodeTracking-0.1.1/QRcodeTracking/
--rw-rw-rw-   0        0        0    76800 2023-07-14 03:35:22.000000 QRcodeTracking-0.1.1/QRcodeTracking/QR_codefunction.pyd
--rw-rw-rw-   0        0        0   114176 2023-07-14 03:35:17.000000 QRcodeTracking-0.1.1/QRcodeTracking/QRcodeTracking.pyd
--rw-rw-rw-   0        0        0        0 2023-07-13 02:44:59.000000 QRcodeTracking-0.1.1/QRcodeTracking/__init__.py
--rw-rw-rw-   0        0        0    64000 2023-07-14 03:35:10.000000 QRcodeTracking-0.1.1/QRcodeTracking/erwewima_ui.pyd
-drwxrwxrwx   0        0        0        0 2023-07-14 03:50:55.184405 QRcodeTracking-0.1.1/QRcodeTracking.egg-info/
--rw-rw-rw-   0        0        0      373 2023-07-14 03:50:55.000000 QRcodeTracking-0.1.1/QRcodeTracking.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2023-07-14 03:50:55.000000 QRcodeTracking-0.1.1/QRcodeTracking.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 03:50:55.000000 QRcodeTracking-0.1.1/QRcodeTracking.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-14 03:50:55.000000 QRcodeTracking-0.1.1/QRcodeTracking.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       15 2023-07-14 03:40:50.000000 QRcodeTracking-0.1.1/README.md
--rw-rw-rw-   0        0        0      136 2023-07-14 03:50:55.189436 QRcodeTracking-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1006 2023-07-14 03:37:31.000000 QRcodeTracking-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:31:06.967717 QRcodeTracking-0.1.2/
+-rw-rw-rw-   0        0        0       19 2023-07-05 02:27:45.000000 QRcodeTracking-0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 QRcodeTracking-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      373 2023-07-14 07:31:06.967717 QRcodeTracking-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-14 07:31:06.943718 QRcodeTracking-0.1.2/QRcodeTracking/
+-rw-rw-rw-   0        0        0    76800 2023-07-14 07:14:48.000000 QRcodeTracking-0.1.2/QRcodeTracking/QR_codefunction.pyd
+-rw-rw-rw-   0        0        0   115712 2023-07-14 07:14:40.000000 QRcodeTracking-0.1.2/QRcodeTracking/QRcodeTracking.pyd
+-rw-rw-rw-   0        0        0        0 2023-07-13 02:44:59.000000 QRcodeTracking-0.1.2/QRcodeTracking/__init__.py
+-rw-rw-rw-   0        0        0    64000 2023-07-14 07:14:30.000000 QRcodeTracking-0.1.2/QRcodeTracking/erwewima_ui.pyd
+drwxrwxrwx   0        0        0        0 2023-07-14 07:31:06.963721 QRcodeTracking-0.1.2/QRcodeTracking.egg-info/
+-rw-rw-rw-   0        0        0      373 2023-07-14 07:31:06.000000 QRcodeTracking-0.1.2/QRcodeTracking.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2023-07-14 07:31:06.000000 QRcodeTracking-0.1.2/QRcodeTracking.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 07:31:06.000000 QRcodeTracking-0.1.2/QRcodeTracking.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-14 07:31:06.000000 QRcodeTracking-0.1.2/QRcodeTracking.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       15 2023-07-14 03:40:50.000000 QRcodeTracking-0.1.2/README.md
+-rw-rw-rw-   0        0        0      136 2023-07-14 07:31:06.970716 QRcodeTracking-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1006 2023-07-14 07:29:23.000000 QRcodeTracking-0.1.2/setup.py
```

### Comparing `QRcodeTracking-0.1.1/setup.py` & `QRcodeTracking-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 1
-PATCH = 1
+PATCH = 2
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "QRcodeTracking",
```

