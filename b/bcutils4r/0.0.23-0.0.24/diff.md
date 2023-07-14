# Comparing `tmp/bcutils4r-0.0.23.tar.gz` & `tmp/bcutils4r-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcutils4r-0.0.23.tar", last modified: Fri Jul 14 01:36:32 2023, max compression
+gzip compressed data, was "bcutils4r-0.0.24.tar", last modified: Fri Jul 14 01:42:38 2023, max compression
```

## Comparing `bcutils4r-0.0.23.tar` & `bcutils4r-0.0.24.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-14 01:36:32.673217 bcutils4r-0.0.23/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    35128 2022-07-24 06:54:15.000000 bcutils4r-0.0.23/LICENSE
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     4387 2023-07-14 01:36:32.673217 bcutils4r-0.0.23/PKG-INFO
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     3739 2023-07-14 01:34:31.000000 bcutils4r-0.0.23/README.md
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      678 2023-07-14 01:36:04.000000 bcutils4r-0.0.23/pyproject.toml
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       38 2023-07-14 01:36:32.673217 bcutils4r-0.0.23/setup.cfg
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      998 2023-07-14 01:36:00.000000 bcutils4r-0.0.23/setup.py
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-14 01:36:32.673217 bcutils4r-0.0.23/src/
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-14 01:36:32.673217 bcutils4r-0.0.23/src/bcutils4r/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        0 2022-07-24 06:54:15.000000 bcutils4r-0.0.23/src/bcutils4r/__init__.py
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    16996 2023-07-14 01:21:43.000000 bcutils4r-0.0.23/src/bcutils4r/eval_classification.py
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-14 01:36:32.673217 bcutils4r-0.0.23/src/bcutils4r.egg-info/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     4387 2023-07-14 01:36:32.000000 bcutils4r-0.0.23/src/bcutils4r.egg-info/PKG-INFO
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      288 2023-07-14 01:36:32.000000 bcutils4r-0.0.23/src/bcutils4r.egg-info/SOURCES.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        1 2023-07-14 01:36:32.000000 bcutils4r-0.0.23/src/bcutils4r.egg-info/dependency_links.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       45 2023-07-14 01:36:32.000000 bcutils4r-0.0.23/src/bcutils4r.egg-info/requires.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       10 2023-07-14 01:36:32.000000 bcutils4r-0.0.23/src/bcutils4r.egg-info/top_level.txt
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-14 01:42:38.494657 bcutils4r-0.0.24/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    35128 2022-07-24 06:54:15.000000 bcutils4r-0.0.24/LICENSE
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     4373 2023-07-14 01:42:38.494657 bcutils4r-0.0.24/PKG-INFO
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     3725 2023-07-14 01:41:30.000000 bcutils4r-0.0.24/README.md
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      678 2023-07-14 01:42:05.000000 bcutils4r-0.0.24/pyproject.toml
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       38 2023-07-14 01:42:38.494657 bcutils4r-0.0.24/setup.cfg
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      998 2023-07-14 01:41:59.000000 bcutils4r-0.0.24/setup.py
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-14 01:42:38.494657 bcutils4r-0.0.24/src/
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-14 01:42:38.494657 bcutils4r-0.0.24/src/bcutils4r/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        0 2022-07-24 06:54:15.000000 bcutils4r-0.0.24/src/bcutils4r/__init__.py
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    16996 2023-07-14 01:21:43.000000 bcutils4r-0.0.24/src/bcutils4r/eval_classification.py
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-14 01:42:38.494657 bcutils4r-0.0.24/src/bcutils4r.egg-info/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     4373 2023-07-14 01:42:38.000000 bcutils4r-0.0.24/src/bcutils4r.egg-info/PKG-INFO
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      288 2023-07-14 01:42:38.000000 bcutils4r-0.0.24/src/bcutils4r.egg-info/SOURCES.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        1 2023-07-14 01:42:38.000000 bcutils4r-0.0.24/src/bcutils4r.egg-info/dependency_links.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       45 2023-07-14 01:42:38.000000 bcutils4r-0.0.24/src/bcutils4r.egg-info/requires.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       10 2023-07-14 01:42:38.000000 bcutils4r-0.0.24/src/bcutils4r.egg-info/top_level.txt
```

### Comparing `bcutils4r-0.0.23/LICENSE` & `bcutils4r-0.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `bcutils4r-0.0.23/PKG-INFO` & `bcutils4r-0.0.24/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcutils4r
-Version: 0.0.23
+Version: 0.0.24
 Summary: Wrapper around some basic sklearn and scikit-plot utilities for binary classification.
 Home-page: https://github.com/rutujagurav/bcutils4r
 Author: Rutuja Gurav
 Author-email: Rutuja Gurav <rutujagurav100@gmail.com>
 Project-URL: Homepage, https://github.com/rutujagurav/bcutils4r
 Project-URL: Bug Tracker, https://github.com/rutujagurav/bcutils4r/issues
 Classifier: Programming Language :: Python :: 3
@@ -81,33 +81,33 @@
                     X=X, y=y, 
                     y_test=y_test, y_pred=y_pred, y_pred_proba=y_pred_proba, 
                     save=False, RESULTS_DIR=None,
                     show=True)
 
 ```
 <!-- ### Confusion Matrix -->
-![cm](tests/example_classification/results/confusion_matrix.png)
-<!-- ![cm](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/confusion_matrix.png) -->
+<!-- ![cm](tests/example_classification/results/confusion_matrix.png) -->
+![cm](https://github.com/rutujagurav/bcutils4r/blob/main/tests/example_classification/results/confusion_matrix.png)
 
 <!-- ### Class-wise ROC curve -->
-![roc](tests/example_classification/results/classwise_roc_curve.png)
-<!-- ![roc](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/classwise_roc_curve.png) -->
+<!-- ![roc](tests/example_classification/results/classwise_roc_curve.png) -->
+![roc](https://github.com/rutujagurav/bcutils4r/blob/main/tests/example_classification/results/classwise_roc_curve.png)
 
 <!-- ### Class-wise PR curve -->
-![pr](tests/example_classification/results/classwise_pr_curve.png)
-<!-- ![pr](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/classwise_pr_curve.png) -->
+<!-- ![pr](tests/example_classification/results/classwise_pr_curve.png) -->
+![pr](https://github.com/rutujagurav/bcutils4r/blob/main/tests/example_classification/results/classwise_pr_curve.png)
 
 <!-- ### KS statistic  -->
-![ks_stat](tests/example_classification/results/ks_stat.png)
-<!-- ![ks_stat](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/ks_stat.png) -->
+<!-- ![ks_stat](tests/example_classification/results/ks_stat.png) -->
+![ks_stat](https://github.com/rutujagurav/bcutils4r/blob/main/tests/example_classification/results/ks_stat.png)
 
 <!-- ### Lift Curve  -->
-![lift](tests/example_classification/results/lift_curve.png)
-<!-- ![lift](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/lift_curve.png) -->
+<!-- ![lift](tests/example_classification/results/lift_curve.png) -->
+![lift](https://github.com/rutujagurav/bcutils4r/blob/main/tests/example_classification/results/lift_curve.png)
 
 <!-- ### Cross-validated ROC curves -->
-![cv_roc](tests/example_classification/results/crossvalidation_roc_curve.png)
-<!-- ![cv_roc](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/crossvalidation_roc_curve.png) -->
+<!-- ![cv_roc](tests/example_classification/results/crossvalidation_roc_curve.png) -->
+![cv_roc](https://github.com/rutujagurav/bcutils4r/blob/main/tests/example_classification/results/crossvalidation_roc_curve.png)
 
 <!-- ### Cross-validated PR curves -->
-![cv_pr](tests/example_classification/results/crossvalidation_pr_curve.png)
-<!-- ![cv_pr](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/crossvalidation_pr_curve.png) -->
+<!-- ![cv_pr](tests/example_classification/results/crossvalidation_pr_curve.png) -->
+![cv_pr](https://github.com/rutujagurav/bcutils4r/blob/main/tests/example_classification/results/crossvalidation_pr_curve.png)
```

### Comparing `bcutils4r-0.0.23/README.md` & `bcutils4r-0.0.24/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -65,33 +65,33 @@
                     X=X, y=y, 
                     y_test=y_test, y_pred=y_pred, y_pred_proba=y_pred_proba, 
                     save=False, RESULTS_DIR=None,
                     show=True)
 
 ```
 <!-- ### Confusion Matrix -->
-![cm](tests/example_classification/results/confusion_matrix.png)
-<!-- ![cm](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/confusion_matrix.png) -->
+<!-- ![cm](tests/example_classification/results/confusion_matrix.png) -->
+![cm](https://github.com/rutujagurav/bcutils4r/blob/main/tests/example_classification/results/confusion_matrix.png)
 
 <!-- ### Class-wise ROC curve -->
-![roc](tests/example_classification/results/classwise_roc_curve.png)
-<!-- ![roc](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/classwise_roc_curve.png) -->
+<!-- ![roc](tests/example_classification/results/classwise_roc_curve.png) -->
+![roc](https://github.com/rutujagurav/bcutils4r/blob/main/tests/example_classification/results/classwise_roc_curve.png)
 
 <!-- ### Class-wise PR curve -->
-![pr](tests/example_classification/results/classwise_pr_curve.png)
-<!-- ![pr](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/classwise_pr_curve.png) -->
+<!-- ![pr](tests/example_classification/results/classwise_pr_curve.png) -->
+![pr](https://github.com/rutujagurav/bcutils4r/blob/main/tests/example_classification/results/classwise_pr_curve.png)
 
 <!-- ### KS statistic  -->
-![ks_stat](tests/example_classification/results/ks_stat.png)
-<!-- ![ks_stat](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/ks_stat.png) -->
+<!-- ![ks_stat](tests/example_classification/results/ks_stat.png) -->
+![ks_stat](https://github.com/rutujagurav/bcutils4r/blob/main/tests/example_classification/results/ks_stat.png)
 
 <!-- ### Lift Curve  -->
-![lift](tests/example_classification/results/lift_curve.png)
-<!-- ![lift](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/lift_curve.png) -->
+<!-- ![lift](tests/example_classification/results/lift_curve.png) -->
+![lift](https://github.com/rutujagurav/bcutils4r/blob/main/tests/example_classification/results/lift_curve.png)
 
 <!-- ### Cross-validated ROC curves -->
-![cv_roc](tests/example_classification/results/crossvalidation_roc_curve.png)
-<!-- ![cv_roc](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/crossvalidation_roc_curve.png) -->
+<!-- ![cv_roc](tests/example_classification/results/crossvalidation_roc_curve.png) -->
+![cv_roc](https://github.com/rutujagurav/bcutils4r/blob/main/tests/example_classification/results/crossvalidation_roc_curve.png)
 
 <!-- ### Cross-validated PR curves -->
-![cv_pr](tests/example_classification/results/crossvalidation_pr_curve.png)
-<!-- ![cv_pr](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/crossvalidation_pr_curve.png) -->
+<!-- ![cv_pr](tests/example_classification/results/crossvalidation_pr_curve.png) -->
+![cv_pr](https://github.com/rutujagurav/bcutils4r/blob/main/tests/example_classification/results/crossvalidation_pr_curve.png)
```

### Comparing `bcutils4r-0.0.23/pyproject.toml` & `bcutils4r-0.0.24/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bcutils4r"
-version = "0.0.23"
+version = "0.0.24"
 authors = [
   { name="Rutuja Gurav", email="rutujagurav100@gmail.com" },
 ]
 description = "Wrapper around some basic sklearn and scikit-plot utilities for binary classification."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers=[
```

### Comparing `bcutils4r-0.0.23/setup.py` & `bcutils4r-0.0.24/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="bcutils4r", # Replace with your own username
-    version="0.0.23",
+    version="0.0.24",
     author="Rutuja Gurav",
     author_email="rutujagurav100@gmail.com",
     description="Wrapper around some basic sklearn and scikit-plot utilities for binary classification.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rutujagurav/bcutils4r",
     project_urls={
```

### Comparing `bcutils4r-0.0.23/src/bcutils4r/eval_classification.py` & `bcutils4r-0.0.24/src/bcutils4r/eval_classification.py`

 * *Files identical despite different names*

### Comparing `bcutils4r-0.0.23/src/bcutils4r.egg-info/PKG-INFO` & `bcutils4r-0.0.24/src/bcutils4r.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcutils4r
-Version: 0.0.23
+Version: 0.0.24
 Summary: Wrapper around some basic sklearn and scikit-plot utilities for binary classification.
 Home-page: https://github.com/rutujagurav/bcutils4r
 Author: Rutuja Gurav
 Author-email: Rutuja Gurav <rutujagurav100@gmail.com>
 Project-URL: Homepage, https://github.com/rutujagurav/bcutils4r
 Project-URL: Bug Tracker, https://github.com/rutujagurav/bcutils4r/issues
 Classifier: Programming Language :: Python :: 3
@@ -81,33 +81,33 @@
                     X=X, y=y, 
                     y_test=y_test, y_pred=y_pred, y_pred_proba=y_pred_proba, 
                     save=False, RESULTS_DIR=None,
                     show=True)
 
 ```
 <!-- ### Confusion Matrix -->
-![cm](tests/example_classification/results/confusion_matrix.png)
-<!-- ![cm](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/confusion_matrix.png) -->
+<!-- ![cm](tests/example_classification/results/confusion_matrix.png) -->
+![cm](https://github.com/rutujagurav/bcutils4r/blob/main/tests/example_classification/results/confusion_matrix.png)
 
 <!-- ### Class-wise ROC curve -->
-![roc](tests/example_classification/results/classwise_roc_curve.png)
-<!-- ![roc](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/classwise_roc_curve.png) -->
+<!-- ![roc](tests/example_classification/results/classwise_roc_curve.png) -->
+![roc](https://github.com/rutujagurav/bcutils4r/blob/main/tests/example_classification/results/classwise_roc_curve.png)
 
 <!-- ### Class-wise PR curve -->
-![pr](tests/example_classification/results/classwise_pr_curve.png)
-<!-- ![pr](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/classwise_pr_curve.png) -->
+<!-- ![pr](tests/example_classification/results/classwise_pr_curve.png) -->
+![pr](https://github.com/rutujagurav/bcutils4r/blob/main/tests/example_classification/results/classwise_pr_curve.png)
 
 <!-- ### KS statistic  -->
-![ks_stat](tests/example_classification/results/ks_stat.png)
-<!-- ![ks_stat](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/ks_stat.png) -->
+<!-- ![ks_stat](tests/example_classification/results/ks_stat.png) -->
+![ks_stat](https://github.com/rutujagurav/bcutils4r/blob/main/tests/example_classification/results/ks_stat.png)
 
 <!-- ### Lift Curve  -->
-![lift](tests/example_classification/results/lift_curve.png)
-<!-- ![lift](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/lift_curve.png) -->
+<!-- ![lift](tests/example_classification/results/lift_curve.png) -->
+![lift](https://github.com/rutujagurav/bcutils4r/blob/main/tests/example_classification/results/lift_curve.png)
 
 <!-- ### Cross-validated ROC curves -->
-![cv_roc](tests/example_classification/results/crossvalidation_roc_curve.png)
-<!-- ![cv_roc](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/crossvalidation_roc_curve.png) -->
+<!-- ![cv_roc](tests/example_classification/results/crossvalidation_roc_curve.png) -->
+![cv_roc](https://github.com/rutujagurav/bcutils4r/blob/main/tests/example_classification/results/crossvalidation_roc_curve.png)
 
 <!-- ### Cross-validated PR curves -->
-![cv_pr](tests/example_classification/results/crossvalidation_pr_curve.png)
-<!-- ![cv_pr](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/crossvalidation_pr_curve.png) -->
+<!-- ![cv_pr](tests/example_classification/results/crossvalidation_pr_curve.png) -->
+![cv_pr](https://github.com/rutujagurav/bcutils4r/blob/main/tests/example_classification/results/crossvalidation_pr_curve.png)
```

