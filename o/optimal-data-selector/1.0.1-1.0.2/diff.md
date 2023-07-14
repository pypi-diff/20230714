# Comparing `tmp/optimal_data_selector-1.0.1.tar.gz` & `tmp/optimal_data_selector-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimal_data_selector-1.0.1.tar", last modified: Thu Jul 13 15:53:30 2023, max compression
+gzip compressed data, was "optimal_data_selector-1.0.2.tar", last modified: Fri Jul 14 06:26:58 2023, max compression
```

## Comparing `optimal_data_selector-1.0.1.tar` & `optimal_data_selector-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 15:53:30.769884 optimal_data_selector-1.0.1/
--rw-rw-rw-   0        0        0        0 2023-07-13 10:41:27.000000 optimal_data_selector-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      860 2023-07-13 15:53:30.767885 optimal_data_selector-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-13 15:53:30.678940 optimal_data_selector-1.0.1/optimal_data_selector/
--rw-rw-rw-   0        0        0        0 2023-07-13 09:41:50.000000 optimal_data_selector-1.0.1/optimal_data_selector/__init__.py
--rw-rw-rw-   0        0        0     9647 2023-07-13 14:26:26.000000 optimal_data_selector-1.0.1/optimal_data_selector/optimal.py
--rw-rw-rw-   0        0        0        0 2023-07-13 09:28:13.000000 optimal_data_selector-1.0.1/optimal_data_selector/optimal_2.py
-drwxrwxrwx   0        0        0        0 2023-07-13 15:53:30.764888 optimal_data_selector-1.0.1/optimal_data_selector.egg-info/
--rw-rw-rw-   0        0        0      860 2023-07-13 15:53:26.000000 optimal_data_selector-1.0.1/optimal_data_selector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-07-13 15:53:26.000000 optimal_data_selector-1.0.1/optimal_data_selector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 15:53:26.000000 optimal_data_selector-1.0.1/optimal_data_selector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-07-13 15:53:26.000000 optimal_data_selector-1.0.1/optimal_data_selector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 15:53:30.770884 optimal_data_selector-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1157 2023-07-13 15:49:39.000000 optimal_data_selector-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 06:26:58.473168 optimal_data_selector-1.0.2/
+-rw-rw-rw-   0        0        0        0 2023-07-13 10:41:27.000000 optimal_data_selector-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      899 2023-07-14 06:26:58.471170 optimal_data_selector-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-14 06:26:58.329643 optimal_data_selector-1.0.2/optimal_data_selector/
+-rw-rw-rw-   0        0        0        0 2023-07-13 09:41:50.000000 optimal_data_selector-1.0.2/optimal_data_selector/__init__.py
+-rw-rw-rw-   0        0        0     9647 2023-07-13 14:26:26.000000 optimal_data_selector-1.0.2/optimal_data_selector/optimal.py
+-rw-rw-rw-   0        0        0        0 2023-07-13 09:28:13.000000 optimal_data_selector-1.0.2/optimal_data_selector/optimal_2.py
+drwxrwxrwx   0        0        0        0 2023-07-14 06:26:58.456892 optimal_data_selector-1.0.2/optimal_data_selector.egg-info/
+-rw-rw-rw-   0        0        0      899 2023-07-14 06:26:56.000000 optimal_data_selector-1.0.2/optimal_data_selector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-07-14 06:26:56.000000 optimal_data_selector-1.0.2/optimal_data_selector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 06:26:56.000000 optimal_data_selector-1.0.2/optimal_data_selector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-14 06:26:56.000000 optimal_data_selector-1.0.2/optimal_data_selector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 06:26:58.474167 optimal_data_selector-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1199 2023-07-14 06:23:11.000000 optimal_data_selector-1.0.2/setup.py
```

### Comparing `optimal_data_selector-1.0.1/PKG-INFO` & `optimal_data_selector-1.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: optimal_data_selector
-Version: 1.0.1
+Version: 1.0.2
 Summary: A function for selecting optimal data combinations
 Author: Rohan Majumder
 Author-email: majumderrohan2001@gmail.com
-Keywords: get_best_data_combination,optimise_accuracy,lock_data_combination,gives_best_result,best_data_for_ML_models
+Keywords: get_best_data_combination,optimise_accuracy,lock_data_combination,gives_best_result,best_data_for_ML_models,works on text data
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-A package to increase the accuracy of ML models, gives you the best data for model training
+A package to increase the accuracy of ML models, gives you the best data for model training, works on text data
```

### Comparing `optimal_data_selector-1.0.1/optimal_data_selector/optimal.py` & `optimal_data_selector-1.0.2/optimal_data_selector/optimal.py`

 * *Files identical despite different names*

### Comparing `optimal_data_selector-1.0.1/optimal_data_selector.egg-info/PKG-INFO` & `optimal_data_selector-1.0.2/optimal_data_selector.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: optimal-data-selector
-Version: 1.0.1
+Version: 1.0.2
 Summary: A function for selecting optimal data combinations
 Author: Rohan Majumder
 Author-email: majumderrohan2001@gmail.com
-Keywords: get_best_data_combination,optimise_accuracy,lock_data_combination,gives_best_result,best_data_for_ML_models
+Keywords: get_best_data_combination,optimise_accuracy,lock_data_combination,gives_best_result,best_data_for_ML_models,works on text data
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-A package to increase the accuracy of ML models, gives you the best data for model training
+A package to increase the accuracy of ML models, gives you the best data for model training, works on text data
```

### Comparing `optimal_data_selector-1.0.1/setup.py` & `optimal_data_selector-1.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.0.1'
+VERSION = '1.0.2'
 DESCRIPTION = 'A function for selecting optimal data combinations'
-LONG_DESCRIPTION = 'A package to increase the accuracy of ML models, gives you the best data for model training'
+LONG_DESCRIPTION = 'A package to increase the accuracy of ML models, gives you the best data for model training, works on text data'
 
 # Setting up
 setup(
     name="optimal_data_selector",
     version=VERSION,
     author="Rohan Majumder",
     author_email="majumderrohan2001@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[],
-    keywords=['get_best_data_combination', 'optimise_accuracy', 'lock_data_combination', 'gives_best_result', 'best_data_for_ML_models'],
+    keywords=['get_best_data_combination', 'optimise_accuracy', 'lock_data_combination', 'gives_best_result', 'best_data_for_ML_models', 'works on text data'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         "Operating System :: Unix",
```

