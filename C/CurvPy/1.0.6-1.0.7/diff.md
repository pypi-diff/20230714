# Comparing `tmp/CurvPy-1.0.6.tar.gz` & `tmp/CurvPy-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CurvPy-1.0.6.tar", last modified: Fri Jul 14 14:12:01 2023, max compression
+gzip compressed data, was "CurvPy-1.0.7.tar", last modified: Fri Jul 14 14:20:37 2023, max compression
```

## Comparing `CurvPy-1.0.6.tar` & `CurvPy-1.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 14:12:01.787729 CurvPy-1.0.6/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 14:12:01.787729 CurvPy-1.0.6/CurvPy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5264 2023-07-14 14:12:01.000000 CurvPy-1.0.6/CurvPy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      203 2023-07-14 14:12:01.000000 CurvPy-1.0.6/CurvPy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 14:12:01.000000 CurvPy-1.0.6/CurvPy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       36 2023-07-14 14:12:01.000000 CurvPy-1.0.6/CurvPy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-14 14:12:01.000000 CurvPy-1.0.6/CurvPy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5264 2023-07-14 14:12:01.787729 CurvPy-1.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5143 2023-07-14 14:01:17.000000 CurvPy-1.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 14:12:01.787729 CurvPy-1.0.6/curvpy/
--rw-r--r--   0 root         (0) root         (0)       91 2023-07-05 19:13:20.000000 CurvPy-1.0.6/curvpy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8078 2023-07-05 19:20:26.000000 CurvPy-1.0.6/curvpy/curvpy.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 14:12:01.787729 CurvPy-1.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      549 2023-07-14 14:11:10.000000 CurvPy-1.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 14:20:37.907738 CurvPy-1.0.7/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 14:20:37.897738 CurvPy-1.0.7/CurvPy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5464 2023-07-14 14:20:37.000000 CurvPy-1.0.7/CurvPy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      203 2023-07-14 14:20:37.000000 CurvPy-1.0.7/CurvPy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 14:20:37.000000 CurvPy-1.0.7/CurvPy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-07-14 14:20:37.000000 CurvPy-1.0.7/CurvPy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-14 14:20:37.000000 CurvPy-1.0.7/CurvPy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5464 2023-07-14 14:20:37.907738 CurvPy-1.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5346 2023-07-14 14:19:02.000000 CurvPy-1.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 14:20:37.907738 CurvPy-1.0.7/curvpy/
+-rw-r--r--   0 root         (0) root         (0)       91 2023-07-05 19:13:20.000000 CurvPy-1.0.7/curvpy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8078 2023-07-05 19:20:26.000000 CurvPy-1.0.7/curvpy/curvpy.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 14:20:37.907738 CurvPy-1.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      549 2023-07-14 14:20:04.000000 CurvPy-1.0.7/setup.py
```

### Comparing `CurvPy-1.0.6/CurvPy.egg-info/PKG-INFO` & `CurvPy-1.0.7/CurvPy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CurvPy
-Version: 1.0.6
+Version: 1.0.7
 Summary: A regression analysis library
 Home-page: UNKNOWN
 Author: sidharth
 Author-email: sidharthss2690@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -127,8 +127,11 @@
 
 The number of function evaluations determines the maximum number of times the model function is called during the optimization process. The optimization algorithm iteratively adjusts the parameters of the model function to minimize the difference between the predicted values and the actual data. The purpose of it is to set an upper limit on the computational time for the optimization process. If the algorithm reaches the maximum number of function evaluations specified by "maximum evaluation" before converging to a solution, it will terminate and return the current best estimate of the parameters.
 ## Bound parameters
 
 The bounds parameter allows you to set lower and upper bounds for the parameters of the model function. It helps restrict the parameter search space during the optimization process. By setting bounds, you can constrain the parameters to specific ranges that make sense for your problem. The bounds parameter is a tuple of two arrays: the lower bounds and the upper bounds. For each parameter, specify the lower and upper bounds in the corresponding arrays. Setting a lower bound to -np.inf (negative infinity) means there is no lower constraint, while setting an upper bound to np.inf (positive infinity) means there is no upper constraint. Using bounds can help prevent unrealistic or invalid parameter values during optimization, improving the stability and reliability of the results.
 
 
+# UI-based version of CurvPy
+### CurvPy also have a UI based repository-[https://github.com/sidhu2690/CurvPy]
+### More details about curvpy can be found here- [https://sidhu2690.github.io/curvpy_v2/]
```

### Comparing `CurvPy-1.0.6/PKG-INFO` & `CurvPy-1.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CurvPy
-Version: 1.0.6
+Version: 1.0.7
 Summary: A regression analysis library
 Home-page: UNKNOWN
 Author: sidharth
 Author-email: sidharthss2690@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -127,8 +127,11 @@
 
 The number of function evaluations determines the maximum number of times the model function is called during the optimization process. The optimization algorithm iteratively adjusts the parameters of the model function to minimize the difference between the predicted values and the actual data. The purpose of it is to set an upper limit on the computational time for the optimization process. If the algorithm reaches the maximum number of function evaluations specified by "maximum evaluation" before converging to a solution, it will terminate and return the current best estimate of the parameters.
 ## Bound parameters
 
 The bounds parameter allows you to set lower and upper bounds for the parameters of the model function. It helps restrict the parameter search space during the optimization process. By setting bounds, you can constrain the parameters to specific ranges that make sense for your problem. The bounds parameter is a tuple of two arrays: the lower bounds and the upper bounds. For each parameter, specify the lower and upper bounds in the corresponding arrays. Setting a lower bound to -np.inf (negative infinity) means there is no lower constraint, while setting an upper bound to np.inf (positive infinity) means there is no upper constraint. Using bounds can help prevent unrealistic or invalid parameter values during optimization, improving the stability and reliability of the results.
 
 
+# UI-based version of CurvPy
+### CurvPy also have a UI based repository-[https://github.com/sidhu2690/CurvPy]
+### More details about curvpy can be found here- [https://sidhu2690.github.io/curvpy_v2/]
```

### Comparing `CurvPy-1.0.6/README.md` & `CurvPy-1.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -115,7 +115,11 @@
 ## Number of evaluations
 
 The number of function evaluations determines the maximum number of times the model function is called during the optimization process. The optimization algorithm iteratively adjusts the parameters of the model function to minimize the difference between the predicted values and the actual data. The purpose of it is to set an upper limit on the computational time for the optimization process. If the algorithm reaches the maximum number of function evaluations specified by "maximum evaluation" before converging to a solution, it will terminate and return the current best estimate of the parameters.
 ## Bound parameters
 
 The bounds parameter allows you to set lower and upper bounds for the parameters of the model function. It helps restrict the parameter search space during the optimization process. By setting bounds, you can constrain the parameters to specific ranges that make sense for your problem. The bounds parameter is a tuple of two arrays: the lower bounds and the upper bounds. For each parameter, specify the lower and upper bounds in the corresponding arrays. Setting a lower bound to -np.inf (negative infinity) means there is no lower constraint, while setting an upper bound to np.inf (positive infinity) means there is no upper constraint. Using bounds can help prevent unrealistic or invalid parameter values during optimization, improving the stability and reliability of the results.
 
+
+# UI-based version of CurvPy
+### CurvPy also have a UI based repository-[https://github.com/sidhu2690/CurvPy]
+### More details about curvpy can be found here- [https://sidhu2690.github.io/curvpy_v2/]
```

### Comparing `CurvPy-1.0.6/curvpy/curvpy.py` & `CurvPy-1.0.7/curvpy/curvpy.py`

 * *Files identical despite different names*

### Comparing `CurvPy-1.0.6/setup.py` & `CurvPy-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='CurvPy',
-    version='1.0.6',
+    version='1.0.7',
     author='sidharth',
     author_email='sidharthss2690@gmail.com',
     description='A regression analysis library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

