# Comparing `tmp/gaussianutility-0.1.1.tar.gz` & `tmp/gaussianutility-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaussianutility-0.1.1.tar", last modified: Fri Jul  7 17:26:50 2023, max compression
+gzip compressed data, was "gaussianutility-0.1.2.tar", last modified: Fri Jul 14 16:55:37 2023, max compression
```

## Comparing `gaussianutility-0.1.1.tar` & `gaussianutility-0.1.2.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 sungil    (1000) sungil    (1000)        0 2023-07-07 17:26:50.662551 gaussianutility-0.1.1/
--rw-r--r--   0 sungil    (1000) sungil    (1000)     1799 2023-06-28 19:04:07.000000 gaussianutility-0.1.1/.gitignore
--rw-r--r--   0 sungil    (1000) sungil    (1000)     1068 2023-06-28 19:04:07.000000 gaussianutility-0.1.1/LICENSE
--rw-r--r--   0 sungil    (1000) sungil    (1000)     5038 2023-07-07 17:26:50.652551 gaussianutility-0.1.1/PKG-INFO
--rw-r--r--   0 sungil    (1000) sungil    (1000)     4570 2023-07-07 16:22:21.000000 gaussianutility-0.1.1/README.md
-drwxr-xr-x   0 sungil    (1000) sungil    (1000)        0 2023-07-07 17:26:50.632552 gaussianutility-0.1.1/gaussianutility/
--rw-r--r--   0 sungil    (1000) sungil    (1000)        1 2023-06-28 19:04:07.000000 gaussianutility-0.1.1/gaussianutility/__init__.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)     2595 2023-07-03 20:00:20.000000 gaussianutility-0.1.1/gaussianutility/com2vasp.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)     1202 2023-07-03 20:00:20.000000 gaussianutility-0.1.1/gaussianutility/com2xyz.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)     2194 2023-07-03 20:00:20.000000 gaussianutility-0.1.1/gaussianutility/freezeLayer.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)     6161 2023-07-03 20:31:32.000000 gaussianutility-0.1.1/gaussianutility/gibbsTemp.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)     1494 2023-07-03 20:00:20.000000 gaussianutility-0.1.1/gaussianutility/out2com.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)     1578 2023-07-03 20:00:20.000000 gaussianutility-0.1.1/gaussianutility/out2xyz.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)     2146 2023-07-03 20:00:20.000000 gaussianutility-0.1.1/gaussianutility/printE.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)     7563 2023-07-03 20:00:20.000000 gaussianutility-0.1.1/gaussianutility/sortInput.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)    10666 2023-07-03 20:00:20.000000 gaussianutility-0.1.1/gaussianutility/spectrum.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)     9331 2023-07-03 20:00:20.000000 gaussianutility-0.1.1/gaussianutility/utilities.py
--rw-r--r--   0 sungil    (1000) sungil    (1000)     2794 2023-07-03 20:00:20.000000 gaussianutility-0.1.1/gaussianutility/vasp2com.py
-drwxr-xr-x   0 sungil    (1000) sungil    (1000)        0 2023-07-07 17:26:50.642552 gaussianutility-0.1.1/gaussianutility.egg-info/
--rw-r--r--   0 sungil    (1000) sungil    (1000)     5038 2023-07-07 17:26:50.000000 gaussianutility-0.1.1/gaussianutility.egg-info/PKG-INFO
--rw-r--r--   0 sungil    (1000) sungil    (1000)      995 2023-07-07 17:26:50.000000 gaussianutility-0.1.1/gaussianutility.egg-info/SOURCES.txt
--rw-r--r--   0 sungil    (1000) sungil    (1000)        1 2023-07-07 17:26:50.000000 gaussianutility-0.1.1/gaussianutility.egg-info/dependency_links.txt
--rw-r--r--   0 sungil    (1000) sungil    (1000)      428 2023-07-07 17:26:50.000000 gaussianutility-0.1.1/gaussianutility.egg-info/entry_points.txt
--rw-r--r--   0 sungil    (1000) sungil    (1000)      103 2023-07-07 17:26:50.000000 gaussianutility-0.1.1/gaussianutility.egg-info/requires.txt
--rw-r--r--   0 sungil    (1000) sungil    (1000)       16 2023-07-07 17:26:50.000000 gaussianutility-0.1.1/gaussianutility.egg-info/top_level.txt
--rw-r--r--   0 sungil    (1000) sungil    (1000)      472 2023-07-07 17:22:57.000000 gaussianutility-0.1.1/pyproject.toml
--rw-r--r--   0 sungil    (1000) sungil    (1000)       38 2023-07-07 17:26:50.662551 gaussianutility-0.1.1/setup.cfg
--rw-r--r--   0 sungil    (1000) sungil    (1000)     1622 2023-07-07 17:22:57.000000 gaussianutility-0.1.1/setup.py
-drwxr-xr-x   0 sungil    (1000) sungil    (1000)        0 2023-07-07 17:26:50.652551 gaussianutility-0.1.1/test/
--rw-r--r--   0 sungil    (1000) sungil    (1000)     1187 2023-06-28 19:04:07.000000 gaussianutility-0.1.1/test/3trimerPrism.SiAl.geom.com
--rw-r--r--   0 sungil    (1000) sungil    (1000)  2499899 2023-06-28 19:04:07.000000 gaussianutility-0.1.1/test/3trimerPrism.SiAl.out
--rw-r--r--   0 sungil    (1000) sungil    (1000)     1596 2023-06-28 19:04:07.000000 gaussianutility-0.1.1/test/4tetramerPrism.SiAl.geom.com
--rw-r--r--   0 sungil    (1000) sungil    (1000)  6317153 2023-06-28 19:04:07.000000 gaussianutility-0.1.1/test/4tetramerPrism.SiAl.out
--rw-r--r--   0 sungil    (1000) sungil    (1000)     1929 2023-06-28 19:04:07.000000 gaussianutility-0.1.1/test/5pentamerPrism.SiAl.geom.com
--rw-r--r--   0 sungil    (1000) sungil    (1000)   702306 2023-06-28 19:04:07.000000 gaussianutility-0.1.1/test/5pentamerPrism.SiAl.out
--rw-r--r--   0 sungil    (1000) sungil    (1000)     2335 2023-06-28 19:04:07.000000 gaussianutility-0.1.1/test/6hexamerPrism.SiAl.geom.com
--rw-r--r--   0 sungil    (1000) sungil    (1000)  4029103 2023-06-28 19:04:07.000000 gaussianutility-0.1.1/test/6hexamerPrism.SiAl.out
--rw-r--r--   0 sungil    (1000) sungil    (1000)     2676 2023-06-28 19:04:07.000000 gaussianutility-0.1.1/test/7heptamerPrism.SiAl.geom.com
--rw-r--r--   0 sungil    (1000) sungil    (1000)  4193531 2023-06-28 19:04:07.000000 gaussianutility-0.1.1/test/7heptamerPrism.SiAl.out
--rw-r--r--   0 sungil    (1000) sungil    (1000)     3082 2023-06-28 19:04:07.000000 gaussianutility-0.1.1/test/8octamerPrism.SiAl.geom.com
--rw-r--r--   0 sungil    (1000) sungil    (1000) 10170069 2023-06-28 19:04:07.000000 gaussianutility-0.1.1/test/8octamerPrism.SiAl.out
+drwxr-xr-x   0 sungil    (1000) sungil    (1000)        0 2023-07-14 16:55:37.235970 gaussianutility-0.1.2/
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     1799 2023-06-28 19:04:07.000000 gaussianutility-0.1.2/.gitignore
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     1068 2023-06-28 19:04:07.000000 gaussianutility-0.1.2/LICENSE
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     5750 2023-07-14 16:55:37.235970 gaussianutility-0.1.2/PKG-INFO
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     5282 2023-07-13 14:06:36.000000 gaussianutility-0.1.2/README.md
+drwxr-xr-x   0 sungil    (1000) sungil    (1000)        0 2023-07-14 16:55:37.165971 gaussianutility-0.1.2/gaussianutility/
+-rw-r--r--   0 sungil    (1000) sungil    (1000)        1 2023-06-28 19:04:07.000000 gaussianutility-0.1.2/gaussianutility/__init__.py
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     2595 2023-07-03 20:00:20.000000 gaussianutility-0.1.2/gaussianutility/com2vasp.py
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     1202 2023-07-03 20:00:20.000000 gaussianutility-0.1.2/gaussianutility/com2xyz.py
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     2194 2023-07-03 20:00:20.000000 gaussianutility-0.1.2/gaussianutility/freezeLayer.py
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     6161 2023-07-03 20:31:32.000000 gaussianutility-0.1.2/gaussianutility/gibbsTemp.py
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     1494 2023-07-03 20:00:20.000000 gaussianutility-0.1.2/gaussianutility/out2com.py
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     1578 2023-07-03 20:00:20.000000 gaussianutility-0.1.2/gaussianutility/out2xyz.py
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     2146 2023-07-03 20:00:20.000000 gaussianutility-0.1.2/gaussianutility/printE.py
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     7563 2023-07-03 20:00:20.000000 gaussianutility-0.1.2/gaussianutility/sortInput.py
+-rw-r--r--   0 sungil    (1000) sungil    (1000)    10666 2023-07-03 20:00:20.000000 gaussianutility-0.1.2/gaussianutility/spectrum.py
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     9331 2023-07-03 20:00:20.000000 gaussianutility-0.1.2/gaussianutility/utilities.py
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     2794 2023-07-03 20:00:20.000000 gaussianutility-0.1.2/gaussianutility/vasp2com.py
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     1713 2023-07-14 16:47:10.000000 gaussianutility-0.1.2/gaussianutility/xyz2com.py
+drwxr-xr-x   0 sungil    (1000) sungil    (1000)        0 2023-07-14 16:55:37.165971 gaussianutility-0.1.2/gaussianutility.egg-info/
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     5750 2023-07-14 16:55:37.000000 gaussianutility-0.1.2/gaussianutility.egg-info/PKG-INFO
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     1022 2023-07-14 16:55:37.000000 gaussianutility-0.1.2/gaussianutility.egg-info/SOURCES.txt
+-rw-r--r--   0 sungil    (1000) sungil    (1000)        1 2023-07-14 16:55:37.000000 gaussianutility-0.1.2/gaussianutility.egg-info/dependency_links.txt
+-rw-r--r--   0 sungil    (1000) sungil    (1000)      467 2023-07-14 16:55:37.000000 gaussianutility-0.1.2/gaussianutility.egg-info/entry_points.txt
+-rw-r--r--   0 sungil    (1000) sungil    (1000)      103 2023-07-14 16:55:37.000000 gaussianutility-0.1.2/gaussianutility.egg-info/requires.txt
+-rw-r--r--   0 sungil    (1000) sungil    (1000)       16 2023-07-14 16:55:37.000000 gaussianutility-0.1.2/gaussianutility.egg-info/top_level.txt
+-rw-r--r--   0 sungil    (1000) sungil    (1000)      472 2023-07-13 21:38:45.000000 gaussianutility-0.1.2/pyproject.toml
+-rw-r--r--   0 sungil    (1000) sungil    (1000)       38 2023-07-14 16:55:37.235970 gaussianutility-0.1.2/setup.cfg
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     1682 2023-07-13 21:38:37.000000 gaussianutility-0.1.2/setup.py
+drwxr-xr-x   0 sungil    (1000) sungil    (1000)        0 2023-07-14 16:55:37.215970 gaussianutility-0.1.2/test/
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     1187 2023-06-28 19:04:07.000000 gaussianutility-0.1.2/test/3trimerPrism.SiAl.geom.com
+-rw-r--r--   0 sungil    (1000) sungil    (1000)  2499899 2023-06-28 19:04:07.000000 gaussianutility-0.1.2/test/3trimerPrism.SiAl.out
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     1596 2023-06-28 19:04:07.000000 gaussianutility-0.1.2/test/4tetramerPrism.SiAl.geom.com
+-rw-r--r--   0 sungil    (1000) sungil    (1000)  6317153 2023-06-28 19:04:07.000000 gaussianutility-0.1.2/test/4tetramerPrism.SiAl.out
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     1929 2023-06-28 19:04:07.000000 gaussianutility-0.1.2/test/5pentamerPrism.SiAl.geom.com
+-rw-r--r--   0 sungil    (1000) sungil    (1000)   702306 2023-06-28 19:04:07.000000 gaussianutility-0.1.2/test/5pentamerPrism.SiAl.out
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     2335 2023-06-28 19:04:07.000000 gaussianutility-0.1.2/test/6hexamerPrism.SiAl.geom.com
+-rw-r--r--   0 sungil    (1000) sungil    (1000)  4029103 2023-06-28 19:04:07.000000 gaussianutility-0.1.2/test/6hexamerPrism.SiAl.out
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     2676 2023-06-28 19:04:07.000000 gaussianutility-0.1.2/test/7heptamerPrism.SiAl.geom.com
+-rw-r--r--   0 sungil    (1000) sungil    (1000)  4193531 2023-06-28 19:04:07.000000 gaussianutility-0.1.2/test/7heptamerPrism.SiAl.out
+-rw-r--r--   0 sungil    (1000) sungil    (1000)     3082 2023-06-28 19:04:07.000000 gaussianutility-0.1.2/test/8octamerPrism.SiAl.geom.com
+-rw-r--r--   0 sungil    (1000) sungil    (1000) 10170069 2023-06-28 19:04:07.000000 gaussianutility-0.1.2/test/8octamerPrism.SiAl.out
```

### Comparing `gaussianutility-0.1.1/.gitignore` & `gaussianutility-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.1/LICENSE` & `gaussianutility-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.1/PKG-INFO` & `gaussianutility-0.1.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,26 @@
-Metadata-Version: 2.1
-Name: gaussianutility
-Version: 0.1.1
-Summary: Useful utilities to use Gaussian09/16 software
-Home-page: https://github.com/Sungil-Hong/gaussianutility
-Author: Sungil Hong
-Author-email: Sungil Hong <suh33@pitt.edu>
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Gaussian Utility
 
+[![License Badge](https://img.shields.io/github/license/Sungil-Hong/gaussianutility)](https://github.com/loevlie/GPT4Readability/blob/main/LICENSE)
+[![Issues Badge](https://img.shields.io/github/issues/Sungil-Hong/gaussianutility)](https://github.com/loevlie/GPT4Readability/issues)
+[![Pull Requests Badge](https://img.shields.io/github/issues-pr/Sungil-Hong/gaussianutility)](https://github.com/loevlie/GPT4Readability/pulls)
+[![Contributors Badge](https://img.shields.io/github/contributors/Sungil-Hong/gaussianutility)](https://github.com/loevlie/GPT4Readability/graphs/contributors)
+[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/dwyl/esta/issues)
+
 The Gaussian Utility is a Python package that provides useful utilities for working with Gaussian 09/16 software. 
 
 Gaussian is a computer program used by chemists, chemical engineers, biochemists, physicists, and other scientists for performing quantum chemistry calculations.
 
-## Purpose and Functionalities
-
 The Gaussian Utility package offers several functionalities to enhance the usage of Gaussian software.
 Especially, this package can address ONIOM-type Gaussian input/output files, which is not widely available in ASE.
 
 Most of the scripts that work on a Gaussian output file are written based Density Functional Theory calculations.
 Hence, the compatibility with different types of calculations, e.g., coupled cluster, Hartree-Fock, semi-empirical, and Møller–Plesset perturbation methodes has not been confirmed yet.
 
-These functionalities include:
+The package includes the following scripts:
 
 1. Convert input structure file type:
    - `com2vasp`: Converts Gaussian input files (.com) to VASP input files (.vasp).
    - `com2xyz`: Converts Gaussian input files (.com) to XYZ coordinate files (.xyz).
    - `vasp2com`: Converts VASP input files (.vasp) to Gaussian input files (.com).
    
 2. Extract structure from output file:
```

### Comparing `gaussianutility-0.1.1/gaussianutility/com2vasp.py` & `gaussianutility-0.1.2/gaussianutility/com2vasp.py`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.1/gaussianutility/com2xyz.py` & `gaussianutility-0.1.2/gaussianutility/com2xyz.py`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.1/gaussianutility/freezeLayer.py` & `gaussianutility-0.1.2/gaussianutility/freezeLayer.py`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.1/gaussianutility/gibbsTemp.py` & `gaussianutility-0.1.2/gaussianutility/gibbsTemp.py`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.1/gaussianutility/out2com.py` & `gaussianutility-0.1.2/gaussianutility/out2com.py`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.1/gaussianutility/out2xyz.py` & `gaussianutility-0.1.2/gaussianutility/out2xyz.py`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.1/gaussianutility/printE.py` & `gaussianutility-0.1.2/gaussianutility/printE.py`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.1/gaussianutility/sortInput.py` & `gaussianutility-0.1.2/gaussianutility/sortInput.py`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.1/gaussianutility/spectrum.py` & `gaussianutility-0.1.2/gaussianutility/spectrum.py`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.1/gaussianutility/utilities.py` & `gaussianutility-0.1.2/gaussianutility/utilities.py`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.1/gaussianutility/vasp2com.py` & `gaussianutility-0.1.2/gaussianutility/vasp2com.py`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.1/gaussianutility.egg-info/PKG-INFO` & `gaussianutility-0.1.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 Metadata-Version: 2.1
 Name: gaussianutility
-Version: 0.1.1
+Version: 0.1.2
 Summary: Useful utilities to use Gaussian09/16 software
 Home-page: https://github.com/Sungil-Hong/gaussianutility
 Author: Sungil Hong
 Author-email: Sungil Hong <suh33@pitt.edu>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Gaussian Utility
 
+[![License Badge](https://img.shields.io/github/license/Sungil-Hong/gaussianutility)](https://github.com/loevlie/GPT4Readability/blob/main/LICENSE)
+[![Issues Badge](https://img.shields.io/github/issues/Sungil-Hong/gaussianutility)](https://github.com/loevlie/GPT4Readability/issues)
+[![Pull Requests Badge](https://img.shields.io/github/issues-pr/Sungil-Hong/gaussianutility)](https://github.com/loevlie/GPT4Readability/pulls)
+[![Contributors Badge](https://img.shields.io/github/contributors/Sungil-Hong/gaussianutility)](https://github.com/loevlie/GPT4Readability/graphs/contributors)
+[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/dwyl/esta/issues)
+
 The Gaussian Utility is a Python package that provides useful utilities for working with Gaussian 09/16 software. 
 
 Gaussian is a computer program used by chemists, chemical engineers, biochemists, physicists, and other scientists for performing quantum chemistry calculations.
 
-## Purpose and Functionalities
-
 The Gaussian Utility package offers several functionalities to enhance the usage of Gaussian software.
 Especially, this package can address ONIOM-type Gaussian input/output files, which is not widely available in ASE.
 
 Most of the scripts that work on a Gaussian output file are written based Density Functional Theory calculations.
 Hence, the compatibility with different types of calculations, e.g., coupled cluster, Hartree-Fock, semi-empirical, and Møller–Plesset perturbation methodes has not been confirmed yet.
 
-These functionalities include:
+The package includes the following scripts:
 
 1. Convert input structure file type:
    - `com2vasp`: Converts Gaussian input files (.com) to VASP input files (.vasp).
    - `com2xyz`: Converts Gaussian input files (.com) to XYZ coordinate files (.xyz).
    - `vasp2com`: Converts VASP input files (.vasp) to Gaussian input files (.com).
    
 2. Extract structure from output file:
```

### Comparing `gaussianutility-0.1.1/gaussianutility.egg-info/SOURCES.txt` & `gaussianutility-0.1.2/gaussianutility.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 gaussianutility/out2com.py
 gaussianutility/out2xyz.py
 gaussianutility/printE.py
 gaussianutility/sortInput.py
 gaussianutility/spectrum.py
 gaussianutility/utilities.py
 gaussianutility/vasp2com.py
+gaussianutility/xyz2com.py
 gaussianutility.egg-info/PKG-INFO
 gaussianutility.egg-info/SOURCES.txt
 gaussianutility.egg-info/dependency_links.txt
 gaussianutility.egg-info/entry_points.txt
 gaussianutility.egg-info/requires.txt
 gaussianutility.egg-info/top_level.txt
 test/3trimerPrism.SiAl.geom.com
```

### Comparing `gaussianutility-0.1.1/setup.py` & `gaussianutility-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="gaussianutility",
-    version="0.1.1",
+    version="0.1.2",
     author="Sungil Hong",
     author_email="suh33@pitt.edu",
     description="Useful utilities to use Gaussian09/16 software",
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points={'console_scripts': [
                   'com2vasp = gaussianutility.com2vasp:main',
                   'com2xyz = gaussianutility.com2xyz:main',
+                  'xyz2com = gaussianutility.xyz2com:main',
                   'freezeLayer = gaussianutility.freezeLayer:main',
                   'gibbsTemp = gaussianutility.gibbsTemp:main',
                   'out2com = gaussianutility.out2com:main',
                   'out2xyz = gaussianutility.out2xyz:main',
                   'printE = gaussianutility.printE:main',
                   'sortInput = gaussianutility.sortInput:main',
                   'spectrum = gaussianutility.spectrum:main',
```

### Comparing `gaussianutility-0.1.1/test/3trimerPrism.SiAl.geom.com` & `gaussianutility-0.1.2/test/3trimerPrism.SiAl.geom.com`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.1/test/3trimerPrism.SiAl.out` & `gaussianutility-0.1.2/test/3trimerPrism.SiAl.out`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.1/test/4tetramerPrism.SiAl.geom.com` & `gaussianutility-0.1.2/test/4tetramerPrism.SiAl.geom.com`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.1/test/4tetramerPrism.SiAl.out` & `gaussianutility-0.1.2/test/4tetramerPrism.SiAl.out`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.1/test/5pentamerPrism.SiAl.geom.com` & `gaussianutility-0.1.2/test/5pentamerPrism.SiAl.geom.com`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.1/test/5pentamerPrism.SiAl.out` & `gaussianutility-0.1.2/test/5pentamerPrism.SiAl.out`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.1/test/6hexamerPrism.SiAl.geom.com` & `gaussianutility-0.1.2/test/6hexamerPrism.SiAl.geom.com`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.1/test/6hexamerPrism.SiAl.out` & `gaussianutility-0.1.2/test/6hexamerPrism.SiAl.out`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.1/test/7heptamerPrism.SiAl.geom.com` & `gaussianutility-0.1.2/test/7heptamerPrism.SiAl.geom.com`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.1/test/7heptamerPrism.SiAl.out` & `gaussianutility-0.1.2/test/7heptamerPrism.SiAl.out`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.1/test/8octamerPrism.SiAl.geom.com` & `gaussianutility-0.1.2/test/8octamerPrism.SiAl.geom.com`

 * *Files identical despite different names*

### Comparing `gaussianutility-0.1.1/test/8octamerPrism.SiAl.out` & `gaussianutility-0.1.2/test/8octamerPrism.SiAl.out`

 * *Files identical despite different names*

