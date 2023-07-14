# Comparing `tmp/TDCRPy-0.0.1.tar.gz` & `tmp/TDCRPy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\TDCRPy-0.0.1.tar", last modified: Thu Jul 13 17:11:15 2023, max compression
+gzip compressed data, was "dist\TDCRPy-0.0.2.tar", last modified: Fri Jul 14 12:24:16 2023, max compression
```

## Comparing `TDCRPy-0.0.1.tar` & `TDCRPy-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 17:11:14.000000 TDCRPy-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-07-13 17:11:14.000000 TDCRPy-0.0.1/Code/
--rw-rw-rw-   0        0        0    11530 2023-07-05 06:46:32.000000 TDCRPy-0.0.1/Code/Activity_TDCR.py
--rw-rw-rw-   0        0        0     4829 2023-07-05 09:18:15.000000 TDCRPy-0.0.1/Code/EfficiencyProfils.py
--rw-rw-rw-   0        0        0    23202 2023-07-13 12:37:29.000000 TDCRPy-0.0.1/Code/TDCRPy.py
--rw-rw-rw-   0        0        0    79115 2023-07-13 12:37:29.000000 TDCRPy-0.0.1/Code/TDCR_model_lib.py
--rw-rw-rw-   0        0        0     3171 2023-07-13 14:12:55.000000 TDCRPy-0.0.1/Code/TDCRoptimize.py
--rw-rw-rw-   0        0        0       25 2023-07-13 16:42:15.000000 TDCRPy-0.0.1/Code/__init__.py
--rw-rw-rw-   0        0        0      817 2023-05-23 08:42:51.000000 TDCRPy-0.0.1/Code/decay.py
--rw-rw-rw-   0        0        0     3250 2023-05-23 08:42:51.000000 TDCRPy-0.0.1/Code/test1.py
--rw-rw-rw-   0        0        0        0 2023-07-13 12:54:56.000000 TDCRPy-0.0.1/LICENCE
--rw-rw-rw-   0        0        0      552 2023-07-13 17:11:15.000000 TDCRPy-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4737 2023-05-23 08:42:51.000000 TDCRPy-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 17:11:14.000000 TDCRPy-0.0.1/TDCRPy.egg-info/
--rw-rw-rw-   0        0        0      552 2023-07-13 17:11:14.000000 TDCRPy-0.0.1/TDCRPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      327 2023-07-13 17:11:14.000000 TDCRPy-0.0.1/TDCRPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 17:11:14.000000 TDCRPy-0.0.1/TDCRPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-13 17:11:14.000000 TDCRPy-0.0.1/TDCRPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-13 17:11:14.000000 TDCRPy-0.0.1/TDCRPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 17:11:15.000000 TDCRPy-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      710 2023-07-13 17:11:04.000000 TDCRPy-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 12:24:15.000000 TDCRPy-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-07-14 12:24:15.000000 TDCRPy-0.0.2/Code/
+-rw-rw-rw-   0        0        0    11530 2023-07-05 06:46:32.000000 TDCRPy-0.0.2/Code/Activity_TDCR.py
+-rw-rw-rw-   0        0        0     4829 2023-07-05 09:18:15.000000 TDCRPy-0.0.2/Code/EfficiencyProfils.py
+-rw-rw-rw-   0        0        0    23202 2023-07-13 12:37:29.000000 TDCRPy-0.0.2/Code/TDCRPy.py
+-rw-rw-rw-   0        0        0    79115 2023-07-13 12:37:29.000000 TDCRPy-0.0.2/Code/TDCR_model_lib.py
+-rw-rw-rw-   0        0        0     3171 2023-07-13 14:12:55.000000 TDCRPy-0.0.2/Code/TDCRoptimize.py
+-rw-rw-rw-   0        0        0       25 2023-07-13 16:42:15.000000 TDCRPy-0.0.2/Code/__init__.py
+-rw-rw-rw-   0        0        0      817 2023-05-23 08:42:51.000000 TDCRPy-0.0.2/Code/decay.py
+-rw-rw-rw-   0        0        0      210 2023-07-14 12:11:28.000000 TDCRPy-0.0.2/Code/test.py
+-rw-rw-rw-   0        0        0     3250 2023-05-23 08:42:51.000000 TDCRPy-0.0.2/Code/test1.py
+-rw-rw-rw-   0        0        0        0 2023-07-13 12:54:56.000000 TDCRPy-0.0.2/LICENCE
+-rw-rw-rw-   0        0        0      640 2023-07-14 12:24:16.000000 TDCRPy-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4737 2023-05-23 08:42:51.000000 TDCRPy-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 12:24:15.000000 TDCRPy-0.0.2/TDCRPy.egg-info/
+-rw-rw-rw-   0        0        0      640 2023-07-14 12:24:15.000000 TDCRPy-0.0.2/TDCRPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-07-14 12:24:15.000000 TDCRPy-0.0.2/TDCRPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 12:24:15.000000 TDCRPy-0.0.2/TDCRPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-14 12:24:15.000000 TDCRPy-0.0.2/TDCRPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-14 12:24:15.000000 TDCRPy-0.0.2/TDCRPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 12:24:16.000000 TDCRPy-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      799 2023-07-14 12:24:04.000000 TDCRPy-0.0.2/setup.py
```

### Comparing `TDCRPy-0.0.1/Code/Activity_TDCR.py` & `TDCRPy-0.0.2/Code/Activity_TDCR.py`

 * *Files identical despite different names*

### Comparing `TDCRPy-0.0.1/Code/EfficiencyProfils.py` & `TDCRPy-0.0.2/Code/EfficiencyProfils.py`

 * *Files identical despite different names*

### Comparing `TDCRPy-0.0.1/Code/TDCRPy.py` & `TDCRPy-0.0.2/Code/TDCRPy.py`

 * *Files identical despite different names*

### Comparing `TDCRPy-0.0.1/Code/TDCR_model_lib.py` & `TDCRPy-0.0.2/Code/TDCR_model_lib.py`

 * *Files identical despite different names*

### Comparing `TDCRPy-0.0.1/Code/TDCRoptimize.py` & `TDCRPy-0.0.2/Code/TDCRoptimize.py`

 * *Files identical despite different names*

### Comparing `TDCRPy-0.0.1/Code/decay.py` & `TDCRPy-0.0.2/Code/decay.py`

 * *Files identical despite different names*

### Comparing `TDCRPy-0.0.1/Code/test1.py` & `TDCRPy-0.0.2/Code/test1.py`

 * *Files identical despite different names*

### Comparing `TDCRPy-0.0.1/PKG-INFO` & `TDCRPy-0.0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: TDCRPy
-Version: 0.0.1
+Version: 0.0.2
 Summary: TDCR model
 Home-page: UNKNOWN
 Author: RomainCoulon (Romain Coulon)
 Author-email: <romain.coulon@bipm.org>
 License: UNKNOWN
-Keywords: python,TDCR
+Keywords: python,TDCR,Monte-Carlo,radionuclide,scintillation,counting
 Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: Freeware
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 License-File: LICENCE
 
 UNKNOWN
```

### Comparing `TDCRPy-0.0.1/README.md` & `TDCRPy-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `TDCRPy-0.0.1/TDCRPy.egg-info/PKG-INFO` & `TDCRPy-0.0.2/TDCRPy.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: TDCRPy
-Version: 0.0.1
+Version: 0.0.2
 Summary: TDCR model
 Home-page: UNKNOWN
 Author: RomainCoulon (Romain Coulon)
 Author-email: <romain.coulon@bipm.org>
 License: UNKNOWN
-Keywords: python,TDCR
+Keywords: python,TDCR,Monte-Carlo,radionuclide,scintillation,counting
 Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: Freeware
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 License-File: LICENCE
 
 UNKNOWN
```

### Comparing `TDCRPy-0.0.1/setup.py` & `TDCRPy-0.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 DESCRIPTION = "TDCR model"
 
 setup(
     name = "TDCRPy",
     version = VERSION,
     author = "RomainCoulon (Romain Coulon)",
     author_email = "<romain.coulon@bipm.org>",
     description = DESCRIPTION,
     packages = find_packages(),
     install_requires = ["numpy"],
-    keywords = ["python","TDCR"],
+    keywords = ["python","TDCR","Monte-Carlo","radionuclide","scintillation","counting"],
     classifiers=[
-        "Development Status :: 1 - Planning",
-        "Intended Audience :: Developers",
+        "Development Status :: 2 - Pre-Alpha",
+        "Intended Audience :: Science/Research",
+		"License :: Freeware",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
 )
```

