# Comparing `tmp/genomap-1.0.4.tar.gz` & `tmp/genomap-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genomap-1.0.4.tar", last modified: Mon Jul 10 18:27:47 2023, max compression
+gzip compressed data, was "genomap-1.0.5.tar", last modified: Fri Jul 14 21:26:22 2023, max compression
```

## Comparing `genomap-1.0.4.tar` & `genomap-1.0.5.tar`

### file list

```diff
@@ -1,25 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:27:47.092911 genomap-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-10 18:27:06.000000 genomap-1.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-10 18:27:06.000000 genomap-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-07-10 18:27:47.092911 genomap-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-10 18:27:06.000000 genomap-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:27:47.088911 genomap-1.0.4/data/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-10 18:27:06.000000 genomap-1.0.4/data/TM_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:27:47.088911 genomap-1.0.4/genomap/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-10 18:27:06.000000 genomap-1.0.4/genomap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:27:47.092911 genomap-1.0.4/genomap/bregman_genomap/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-10 18:27:06.000000 genomap-1.0.4/genomap/bregman_genomap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   125058 2023-07-10 18:27:06.000000 genomap-1.0.4/genomap/bregman_genomap/bregman_genomap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-07-10 18:27:06.000000 genomap-1.0.4/genomap/genomap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:27:47.092911 genomap-1.0.4/genomap/genomapOPT/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-10 18:27:06.000000 genomap-1.0.4/genomap/genomapOPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-10 18:27:06.000000 genomap-1.0.4/genomap/genomapOPT/genomapOPT.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:27:47.088911 genomap-1.0.4/genomap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-07-10 18:27:47.000000 genomap-1.0.4/genomap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-10 18:27:47.000000 genomap-1.0.4/genomap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 18:27:47.000000 genomap-1.0.4/genomap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-10 18:27:47.000000 genomap-1.0.4/genomap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 18:27:47.000000 genomap-1.0.4/genomap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-10 18:27:06.000000 genomap-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 18:27:47.092911 genomap-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-10 18:27:06.000000 genomap-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:26:22.305258 genomap-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-14 21:24:47.000000 genomap-1.0.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-14 21:24:47.000000 genomap-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-07-14 21:26:22.305258 genomap-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-14 21:24:47.000000 genomap-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:26:22.301258 genomap-1.0.5/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-14 21:24:47.000000 genomap-1.0.5/data/TM_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:26:22.301258 genomap-1.0.5/genomap/
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/ConvDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/ConvIDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13513 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/FcDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/FcIDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:26:22.305258 genomap-1.0.5/genomap/bregman_genomap/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/bregman_genomap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125058 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/bregman_genomap/bregman_genomap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/class_discriminative_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/gTraj_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:26:22.305258 genomap-1.0.5/genomap/genoMOI/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/genoMOI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/genoMOI/genoMOI.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:26:22.305258 genomap-1.0.5/genomap/genoTraj/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/genoTraj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/genoTraj/genoTraj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:26:22.305258 genomap-1.0.5/genomap/genoVis/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/genoVis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/genoVis/genoVis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/genomap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:26:22.305258 genomap-1.0.5/genomap/genomapOPT/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/genomapOPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/genomapOPT/genomapOPT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/group_centroid_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/utils_MOI.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:26:22.305258 genomap-1.0.5/genomap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-07-14 21:26:22.000000 genomap-1.0.5/genomap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-14 21:26:22.000000 genomap-1.0.5/genomap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 21:26:22.000000 genomap-1.0.5/genomap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-14 21:26:22.000000 genomap-1.0.5/genomap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 21:26:22.000000 genomap-1.0.5/genomap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-14 21:24:47.000000 genomap-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 21:26:22.305258 genomap-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-14 21:24:47.000000 genomap-1.0.5/setup.py
```

### Comparing `genomap-1.0.4/LICENSE.txt` & `genomap-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `genomap-1.0.4/PKG-INFO` & `genomap-1.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomap
-Version: 1.0.4
+Version: 1.0.5
 Summary: Genomap converts tabular gene expression data into spatially meaningful images.
 Home-page: https://github.com/xinglab-ai/genomap
 Author: Md Tauhidul Islam
 Author-email: tauhid@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -19,14 +19,19 @@
 
 scipy, scikit-learn, pot, numpy
 
 If you face any issues with packages, please check the environment section of our Code-Ocean capsule (https://doi.org/10.24433/CO.0640398.v1), where you can check the package versions.
 
 # How to use genomap
 
+The easiest way to start with genomap is to install it from pypi using 
+
+```python
+pip install genomap
+```
 The data should be in cell (row) x gene (column) format. Genomap construction needs only one parameter: the size of the genomap (row and column number). The row and column number can be any number starting from 1. You can create square or rectangular genomaps. The number of genes in your dataset should be less than or equal to the number of pixels in the genomap. Genomap construction is very fast and you should get the genomaps within a few seconds.
 
 # Sample data
 
 To run the example code below, you will need to download the required data file. You can download it from [here](https://drive.google.com/file/d/1kkbI9_6zD80Jr5OhMkGlcdMOeWcRfz7b/view?usp=drive_link).
 
 # Example code
```

### Comparing `genomap-1.0.4/README.md` & `genomap-1.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,19 @@
 
 scipy, scikit-learn, pot, numpy
 
 If you face any issues with packages, please check the environment section of our Code-Ocean capsule (https://doi.org/10.24433/CO.0640398.v1), where you can check the package versions.
 
 # How to use genomap
 
+The easiest way to start with genomap is to install it from pypi using 
+
+```python
+pip install genomap
+```
 The data should be in cell (row) x gene (column) format. Genomap construction needs only one parameter: the size of the genomap (row and column number). The row and column number can be any number starting from 1. You can create square or rectangular genomaps. The number of genes in your dataset should be less than or equal to the number of pixels in the genomap. Genomap construction is very fast and you should get the genomaps within a few seconds.
 
 # Sample data
 
 To run the example code below, you will need to download the required data file. You can download it from [here](https://drive.google.com/file/d/1kkbI9_6zD80Jr5OhMkGlcdMOeWcRfz7b/view?usp=drive_link).
 
 # Example code
```

### Comparing `genomap-1.0.4/genomap/bregman_genomap/bregman_genomap.py` & `genomap-1.0.5/genomap/bregman_genomap/bregman_genomap.py`

 * *Files identical despite different names*

### Comparing `genomap-1.0.4/genomap/genomap.py` & `genomap-1.0.5/genomap/genomap.py`

 * *Files identical despite different names*

### Comparing `genomap-1.0.4/genomap/genomapOPT/genomapOPT.py` & `genomap-1.0.5/genomap/genomapOPT/genomapOPT.py`

 * *Files identical despite different names*

### Comparing `genomap-1.0.4/genomap.egg-info/PKG-INFO` & `genomap-1.0.5/genomap.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomap
-Version: 1.0.4
+Version: 1.0.5
 Summary: Genomap converts tabular gene expression data into spatially meaningful images.
 Home-page: https://github.com/xinglab-ai/genomap
 Author: Md Tauhidul Islam
 Author-email: tauhid@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -19,14 +19,19 @@
 
 scipy, scikit-learn, pot, numpy
 
 If you face any issues with packages, please check the environment section of our Code-Ocean capsule (https://doi.org/10.24433/CO.0640398.v1), where you can check the package versions.
 
 # How to use genomap
 
+The easiest way to start with genomap is to install it from pypi using 
+
+```python
+pip install genomap
+```
 The data should be in cell (row) x gene (column) format. Genomap construction needs only one parameter: the size of the genomap (row and column number). The row and column number can be any number starting from 1. You can create square or rectangular genomaps. The number of genes in your dataset should be less than or equal to the number of pixels in the genomap. Genomap construction is very fast and you should get the genomaps within a few seconds.
 
 # Sample data
 
 To run the example code below, you will need to download the required data file. You can download it from [here](https://drive.google.com/file/d/1kkbI9_6zD80Jr5OhMkGlcdMOeWcRfz7b/view?usp=drive_link).
 
 # Example code
```

### Comparing `genomap-1.0.4/setup.py` & `genomap-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="genomap",
-    version="1.0.4",
+    version="1.0.5",
     author="Md Tauhidul Islam",
     author_email="tauhid@stanford.edu",
     description="Genomap converts tabular gene expression data into spatially meaningful images.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xinglab-ai/genomap",
     classifiers=[
```

