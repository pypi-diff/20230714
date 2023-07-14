# Comparing `tmp/TDCRPy-0.0.4.tar.gz` & `tmp/TDCRPy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\TDCRPy-0.0.4.tar", last modified: Fri Jul 14 12:48:20 2023, max compression
+gzip compressed data, was "dist\TDCRPy-0.0.5.tar", last modified: Fri Jul 14 12:50:02 2023, max compression
```

## Comparing `TDCRPy-0.0.4.tar` & `TDCRPy-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 12:48:20.000000 TDCRPy-0.0.4/
-drwxrwxrwx   0        0        0        0 2023-07-14 12:48:20.000000 TDCRPy-0.0.4/Code/
--rw-rw-rw-   0        0        0    11530 2023-07-05 06:46:32.000000 TDCRPy-0.0.4/Code/Activity_TDCR.py
--rw-rw-rw-   0        0        0     4829 2023-07-05 09:18:15.000000 TDCRPy-0.0.4/Code/EfficiencyProfils.py
--rw-rw-rw-   0        0        0    23202 2023-07-13 12:37:29.000000 TDCRPy-0.0.4/Code/TDCRPy.py
--rw-rw-rw-   0        0        0    79115 2023-07-13 12:37:29.000000 TDCRPy-0.0.4/Code/TDCR_model_lib.py
--rw-rw-rw-   0        0        0     3171 2023-07-13 14:12:55.000000 TDCRPy-0.0.4/Code/TDCRoptimize.py
--rw-rw-rw-   0        0        0       25 2023-07-14 12:37:52.000000 TDCRPy-0.0.4/Code/__init__.py
--rw-rw-rw-   0        0        0      817 2023-05-23 08:42:51.000000 TDCRPy-0.0.4/Code/decay.py
--rw-rw-rw-   0        0        0      210 2023-07-14 12:11:28.000000 TDCRPy-0.0.4/Code/test.py
--rw-rw-rw-   0        0        0     3250 2023-05-23 08:42:51.000000 TDCRPy-0.0.4/Code/test1.py
--rw-rw-rw-   0        0        0        0 2023-07-13 12:54:56.000000 TDCRPy-0.0.4/LICENCE
--rw-rw-rw-   0        0        0      659 2023-07-14 12:48:20.000000 TDCRPy-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     4737 2023-05-23 08:42:51.000000 TDCRPy-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 12:48:20.000000 TDCRPy-0.0.4/TDCRPy.egg-info/
--rw-rw-rw-   0        0        0      659 2023-07-14 12:48:19.000000 TDCRPy-0.0.4/TDCRPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-07-14 12:48:20.000000 TDCRPy-0.0.4/TDCRPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 12:48:19.000000 TDCRPy-0.0.4/TDCRPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-14 12:48:19.000000 TDCRPy-0.0.4/TDCRPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-14 12:48:19.000000 TDCRPy-0.0.4/TDCRPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 12:48:20.000000 TDCRPy-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      818 2023-07-14 12:48:08.000000 TDCRPy-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 12:50:01.000000 TDCRPy-0.0.5/
+drwxrwxrwx   0        0        0        0 2023-07-14 12:50:01.000000 TDCRPy-0.0.5/Code/
+-rw-rw-rw-   0        0        0    11530 2023-07-05 06:46:32.000000 TDCRPy-0.0.5/Code/Activity_TDCR.py
+-rw-rw-rw-   0        0        0     4829 2023-07-05 09:18:15.000000 TDCRPy-0.0.5/Code/EfficiencyProfils.py
+-rw-rw-rw-   0        0        0    23202 2023-07-13 12:37:29.000000 TDCRPy-0.0.5/Code/TDCRPy.py
+-rw-rw-rw-   0        0        0    79115 2023-07-13 12:37:29.000000 TDCRPy-0.0.5/Code/TDCR_model_lib.py
+-rw-rw-rw-   0        0        0     3171 2023-07-13 14:12:55.000000 TDCRPy-0.0.5/Code/TDCRoptimize.py
+-rw-rw-rw-   0        0        0       93 2023-07-14 12:49:39.000000 TDCRPy-0.0.5/Code/__init__.py
+-rw-rw-rw-   0        0        0      817 2023-05-23 08:42:51.000000 TDCRPy-0.0.5/Code/decay.py
+-rw-rw-rw-   0        0        0      210 2023-07-14 12:11:28.000000 TDCRPy-0.0.5/Code/test.py
+-rw-rw-rw-   0        0        0     3250 2023-05-23 08:42:51.000000 TDCRPy-0.0.5/Code/test1.py
+-rw-rw-rw-   0        0        0        0 2023-07-13 12:54:56.000000 TDCRPy-0.0.5/LICENCE
+-rw-rw-rw-   0        0        0      659 2023-07-14 12:50:02.000000 TDCRPy-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4737 2023-05-23 08:42:51.000000 TDCRPy-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 12:50:01.000000 TDCRPy-0.0.5/TDCRPy.egg-info/
+-rw-rw-rw-   0        0        0      659 2023-07-14 12:50:01.000000 TDCRPy-0.0.5/TDCRPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-07-14 12:50:01.000000 TDCRPy-0.0.5/TDCRPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 12:50:01.000000 TDCRPy-0.0.5/TDCRPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-14 12:50:01.000000 TDCRPy-0.0.5/TDCRPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-14 12:50:01.000000 TDCRPy-0.0.5/TDCRPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 12:50:02.000000 TDCRPy-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      818 2023-07-14 12:49:51.000000 TDCRPy-0.0.5/setup.py
```

### Comparing `TDCRPy-0.0.4/Code/Activity_TDCR.py` & `TDCRPy-0.0.5/Code/Activity_TDCR.py`

 * *Files identical despite different names*

### Comparing `TDCRPy-0.0.4/Code/EfficiencyProfils.py` & `TDCRPy-0.0.5/Code/EfficiencyProfils.py`

 * *Files identical despite different names*

### Comparing `TDCRPy-0.0.4/Code/TDCRPy.py` & `TDCRPy-0.0.5/Code/TDCRPy.py`

 * *Files identical despite different names*

### Comparing `TDCRPy-0.0.4/Code/TDCR_model_lib.py` & `TDCRPy-0.0.5/Code/TDCR_model_lib.py`

 * *Files identical despite different names*

### Comparing `TDCRPy-0.0.4/Code/TDCRoptimize.py` & `TDCRPy-0.0.5/Code/TDCRoptimize.py`

 * *Files identical despite different names*

### Comparing `TDCRPy-0.0.4/Code/decay.py` & `TDCRPy-0.0.5/Code/decay.py`

 * *Files identical despite different names*

### Comparing `TDCRPy-0.0.4/Code/test1.py` & `TDCRPy-0.0.5/Code/test1.py`

 * *Files identical despite different names*

### Comparing `TDCRPy-0.0.4/PKG-INFO` & `TDCRPy-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TDCRPy
-Version: 0.0.4
+Version: 0.0.5
 Summary: TDCR model
 Home-page: UNKNOWN
 Author: RomainCoulon (Romain Coulon)
 Author-email: <romain.coulon@bipm.org>
 License: UNKNOWN
 Keywords: python,TDCR,Monte-Carlo,radionuclide,scintillation,counting
 Platform: UNKNOWN
```

### Comparing `TDCRPy-0.0.4/README.md` & `TDCRPy-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `TDCRPy-0.0.4/TDCRPy.egg-info/PKG-INFO` & `TDCRPy-0.0.5/TDCRPy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TDCRPy
-Version: 0.0.4
+Version: 0.0.5
 Summary: TDCR model
 Home-page: UNKNOWN
 Author: RomainCoulon (Romain Coulon)
 Author-email: <romain.coulon@bipm.org>
 License: UNKNOWN
 Keywords: python,TDCR,Monte-Carlo,radionuclide,scintillation,counting
 Platform: UNKNOWN
```

### Comparing `TDCRPy-0.0.4/setup.py` & `TDCRPy-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = "0.0.4"
+VERSION = "0.0.5"
 DESCRIPTION = "TDCR model"
 
 setup(
     name = "TDCRPy",
     version = VERSION,
     author = "RomainCoulon (Romain Coulon)",
     author_email = "<romain.coulon@bipm.org>",
```

