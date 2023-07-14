# Comparing `tmp/bcutils4r-0.0.21.tar.gz` & `tmp/bcutils4r-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcutils4r-0.0.21.tar", last modified: Fri Jun  2 03:58:06 2023, max compression
+gzip compressed data, was "bcutils4r-0.0.22.tar", last modified: Fri Jul 14 01:28:35 2023, max compression
```

## Comparing `bcutils4r-0.0.21.tar` & `bcutils4r-0.0.22.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-06-02 03:58:06.363577 bcutils4r-0.0.21/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    35128 2022-07-24 06:54:15.000000 bcutils4r-0.0.21/LICENSE
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     4279 2023-06-02 03:58:06.363577 bcutils4r-0.0.21/PKG-INFO
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     3631 2023-01-31 08:14:46.000000 bcutils4r-0.0.21/README.md
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      678 2023-06-02 03:56:22.000000 bcutils4r-0.0.21/pyproject.toml
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       38 2023-06-02 03:58:06.363577 bcutils4r-0.0.21/setup.cfg
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      982 2023-06-02 03:54:04.000000 bcutils4r-0.0.21/setup.py
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-06-02 03:58:06.359577 bcutils4r-0.0.21/src/
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-06-02 03:58:06.359577 bcutils4r-0.0.21/src/bcutils4r/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        0 2022-07-24 06:54:15.000000 bcutils4r-0.0.21/src/bcutils4r/__init__.py
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    16286 2023-01-31 07:24:25.000000 bcutils4r-0.0.21/src/bcutils4r/eval_model.py
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-06-02 03:58:06.363577 bcutils4r-0.0.21/src/bcutils4r.egg-info/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     4279 2023-06-02 03:58:06.000000 bcutils4r-0.0.21/src/bcutils4r.egg-info/PKG-INFO
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      289 2023-06-02 03:58:06.000000 bcutils4r-0.0.21/src/bcutils4r.egg-info/SOURCES.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        1 2023-06-02 03:58:06.000000 bcutils4r-0.0.21/src/bcutils4r.egg-info/dependency_links.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       32 2023-06-02 03:58:06.000000 bcutils4r-0.0.21/src/bcutils4r.egg-info/requires.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       10 2023-06-02 03:58:06.000000 bcutils4r-0.0.21/src/bcutils4r.egg-info/top_level.txt
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-14 01:28:35.442121 bcutils4r-0.0.22/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    35128 2022-07-24 06:54:15.000000 bcutils4r-0.0.22/LICENSE
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     4300 2023-07-14 01:28:35.442121 bcutils4r-0.0.22/PKG-INFO
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     3652 2023-07-14 00:55:07.000000 bcutils4r-0.0.22/README.md
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      678 2023-07-14 01:24:22.000000 bcutils4r-0.0.22/pyproject.toml
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       38 2023-07-14 01:28:35.442121 bcutils4r-0.0.22/setup.cfg
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      998 2023-07-14 01:25:42.000000 bcutils4r-0.0.22/setup.py
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-14 01:28:35.442121 bcutils4r-0.0.22/src/
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-14 01:28:35.442121 bcutils4r-0.0.22/src/bcutils4r/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        0 2022-07-24 06:54:15.000000 bcutils4r-0.0.22/src/bcutils4r/__init__.py
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    16996 2023-07-14 01:21:43.000000 bcutils4r-0.0.22/src/bcutils4r/eval_classification.py
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-14 01:28:35.442121 bcutils4r-0.0.22/src/bcutils4r.egg-info/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     4300 2023-07-14 01:28:35.000000 bcutils4r-0.0.22/src/bcutils4r.egg-info/PKG-INFO
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      288 2023-07-14 01:28:35.000000 bcutils4r-0.0.22/src/bcutils4r.egg-info/SOURCES.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        1 2023-07-14 01:28:35.000000 bcutils4r-0.0.22/src/bcutils4r.egg-info/dependency_links.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       45 2023-07-14 01:28:35.000000 bcutils4r-0.0.22/src/bcutils4r.egg-info/requires.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       10 2023-07-14 01:28:35.000000 bcutils4r-0.0.22/src/bcutils4r.egg-info/top_level.txt
```

### Comparing `bcutils4r-0.0.21/LICENSE` & `bcutils4r-0.0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `bcutils4r-0.0.21/PKG-INFO` & `bcutils4r-0.0.22/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcutils4r
-Version: 0.0.21
+Version: 0.0.22
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
-<!-- ![cm](tests/DetectPulsarStar/results/confusion_matrix.png) -->
-<!-- ![cm](https://github.com/rutujagurav/bcutils4r/blob/master/tests/DetectPulsarStar/results/confusion_matrix.png) -->
+![cm](tests/example_classification/results/confusion_matrix.png)
+<!-- ![cm](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/confusion_matrix.png) -->
 
 <!-- ### Class-wise ROC curve -->
-<!-- ![roc](tests/DetectPulsarStar/results/classwise_roc_curve.png) -->
-<!-- ![roc](https://github.com/rutujagurav/bcutils4r/blob/master/tests/DetectPulsarStar/results/classwise_roc_curve.png) -->
+![roc](tests/example_classification/results/classwise_roc_curve.png)
+<!-- ![roc](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/classwise_roc_curve.png) -->
 
 <!-- ### Class-wise PR curve -->
-<!-- ![pr](tests/DetectPulsarStar/results/classwise_pr_curve.png) -->
-<!-- ![pr](https://github.com/rutujagurav/bcutils4r/blob/master/tests/DetectPulsarStar/results/classwise_pr_curve.png) -->
+![pr](tests/example_classification/results/classwise_pr_curve.png)
+<!-- ![pr](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/classwise_pr_curve.png) -->
 
 <!-- ### KS statistic  -->
-<!-- ![ks_stat](tests/DetectPulsarStar/results/ks_stat.png) -->
-<!-- ![ks_stat](https://github.com/rutujagurav/bcutils4r/blob/master/tests/DetectPulsarStar/results/ks_stat.png) -->
+![ks_stat](tests/example_classification/results/ks_stat.png)
+<!-- ![ks_stat](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/ks_stat.png) -->
 
 <!-- ### Lift Curve  -->
-<!-- ![lift](tests/DetectPulsarStar/results/lift_curve.png) -->
-<!-- ![lift](https://github.com/rutujagurav/bcutils4r/blob/master/tests/DetectPulsarStar/results/lift_curve.png) -->
+![lift](tests/example_classification/results/lift_curve.png)
+<!-- ![lift](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/lift_curve.png) -->
 
 <!-- ### Cross-validated ROC curves -->
-<!-- ![cv_roc](tests/DetectPulsarStar/results/crossvalidation_roc_curve.png) -->
-<!-- ![cv_roc](https://github.com/rutujagurav/bcutils4r/blob/master/tests/DetectPulsarStar/results/crossvalidation_roc_curve.png) -->
+![cv_roc](tests/example_classification/results/crossvalidation_roc_curve.png)
+<!-- ![cv_roc](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/crossvalidation_roc_curve.png) -->
 
 <!-- ### Cross-validated PR curves -->
-<!-- ![cv_pr](tests/DetectPulsarStar/results/crossvalidation_pr_curve.png) -->
-<!-- ![cv_pr](https://github.com/rutujagurav/bcutils4r/blob/master/tests/DetectPulsarStar/results/crossvalidation_pr_curve.png) -->
+![cv_pr](tests/example_classification/results/crossvalidation_pr_curve.png)
+<!-- ![cv_pr](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/crossvalidation_pr_curve.png) -->
```

### Comparing `bcutils4r-0.0.21/pyproject.toml` & `bcutils4r-0.0.22/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bcutils4r"
-version = "0.0.21"
+version = "0.0.22"
 authors = [
   { name="Rutuja Gurav", email="rutujagurav100@gmail.com" },
 ]
 description = "Wrapper around some basic sklearn and scikit-plot utilities for binary classification."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers=[
```

### Comparing `bcutils4r-0.0.21/setup.py` & `bcutils4r-0.0.22/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="bcutils4r", # Replace with your own username
-    version="0.0.21",
+    version="0.0.22",
     author="Rutuja Gurav",
     author_email="rutujagurav100@gmail.com",
     description="Wrapper around some basic sklearn and scikit-plot utilities for binary classification.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rutujagurav/bcutils4r",
     project_urls={
@@ -17,13 +17,13 @@
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
-          'deprecation', 'seaborn', 'scikit-plot'
+          'deprecation', 'seaborn', 'scikit-learn', 'scikit-plot'
       ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.6",
 )
```

### Comparing `bcutils4r-0.0.21/src/bcutils4r/eval_model.py` & `bcutils4r-0.0.22/src/bcutils4r/eval_classification.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import matplotlib.pyplot as plt
 plt.rcParams['font.family'] = 'serif'
 plt.rcParams['font.serif'] = ['Times New Roman'] + plt.rcParams['font.serif']
+plt.rcParams['axes.facecolor'] = 'white'
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 import seaborn as sns
 
 import pandas as pd
 import numpy as np
 import os
 
@@ -128,58 +129,78 @@
     #     ax.set_text(j, i, cm[i, j], horizontalalignment="center", color=color)
     # ax.set_ylabel('True Label', fontsize=15)
     # ax.set_xlabel('Predicted Label', fontsize=15)
 
     s.set_ylabel('True Label') #, fontsize=15
     s.set_xlabel('Predicted Label')
     
+    plt.tight_layout()
     if save:
         plt.savefig(RESULTS_DIR+'/confusion_matrix.png', bbox_inches='tight',dpi=dpi)
     if show:
         plt.show()
     plt.close()
         
 def plot_ks_stat(y_test=None, y_pred=None, RESULTS_DIR='', show=False, save=False, dpi=300):
     fig, ax = plt.subplots()
     ax = scikitplot.metrics.plot_ks_statistic(y_test, y_pred, ax=ax)
+    ax.set_xlim([-0.05, 1.05])
+    ax.set_ylim([-0.05, 1.05])
+    ax.set_facecolor('white')
     for l in ax.lines:
-        l.set_lw(1)
+        l.set_lw(2)
+    
+    plt.tight_layout()
     if save:
         plt.savefig(RESULTS_DIR+'/ks_stat.png', bbox_inches='tight',dpi=dpi)
     if show:
         plt.show()
     plt.close()
 
 def plot_lift_curve(y_test=None, y_pred=None, RESULTS_DIR='', show=False, save=False, dpi=300):
     fig, ax = plt.subplots()
     ax = scikitplot.metrics.plot_lift_curve(y_test, y_pred, ax=ax)
+    ax.set_facecolor('white')
     for l in ax.lines:
-        l.set_lw(1)
+        l.set_lw(2)
+    
+    plt.tight_layout()
+    plt.legend(loc='best')
     if save:
         plt.savefig(RESULTS_DIR+'/lift_curve.png', bbox_inches='tight',dpi=dpi)
     if show:
         plt.show()    
     plt.close()
 
 def plot_classwise_pr_curve(y_test=None, y_pred=None, RESULTS_DIR='', show=False, save=False, dpi=300):
     fig, ax = plt.subplots()
     ax = scikitplot.metrics.plot_precision_recall(y_test, y_pred, ax=ax)
+    ax.set_xlim([-0.05, 1.05])
+    ax.set_ylim([-0.05, 1.05])
+    ax.set_facecolor('white')
     for l in ax.lines:
-        l.set_lw(1)
+        l.set_lw(2)
+    
+    plt.tight_layout()
     if save:
         plt.savefig(RESULTS_DIR+'/classwise_pr_curve.png', bbox_inches='tight',dpi=dpi)
     if show:
         plt.show()    
     plt.close()
 
 def plot_classwise_roc_curve(y_test=None, y_pred=None, RESULTS_DIR='', show=False, save=False, dpi=300):
     fig, ax = plt.subplots()
     ax = scikitplot.metrics.plot_roc(y_test, y_pred, ax=ax)
+    ax.set_xlim([-0.05, 1.05])
+    ax.set_ylim([-0.05, 1.05])
+    ax.set_facecolor('white')
     for l in ax.lines:
-        l.set_lw(1)
+        l.set_lw(2)
+    
+    plt.tight_layout()
     if save:
         plt.savefig(RESULTS_DIR+'/classwise_roc_curve.png', bbox_inches='tight', dpi=dpi)
     if show:
         plt.show() 
     plt.close()
 
 def generate_classification_report(y_test=None, y_pred=None, RESULTS_DIR='', labels=[], show=False, save=False):
@@ -187,14 +208,15 @@
         report = classification_report(y_test, 
                                         y_pred, 
                                         target_names=[cl+'(class '+str(i)+')' for i, cl in enumerate(labels)], 
                                         output_dict=True)
     else:
         report = classification_report(y_test, y_pred, output_dict=True)
     report_df = pd.DataFrame(report).transpose()
+    
     if save:
         report_df.to_csv(RESULTS_DIR+'/classification_report.csv')
     if show:
         print(report_df)
 
 def plot_cv_roc_curve(classifier=None, cv=None, n_splits=10, X=None, y=None, RESULTS_DIR='', title='Cross-Validated ROC Curve', show=False, save=False, dpi=300):
     """
@@ -244,14 +266,16 @@
 
     plt.xlim([-0.05, 1.05])
     plt.ylim([-0.05, 1.05])
     plt.xlabel('False Positive Rate')
     plt.ylabel('True Positive Rate')
     plt.title(title)
     plt.legend(bbox_to_anchor=(1, 1))
+    # plt.tight_layout()
+    plt.grid()
     if(save):
         plt.savefig(RESULTS_DIR+'/crossvalidation_roc_curve.png', bbox_inches='tight',dpi=dpi)
     if(show):
         plt.show()
     plt.close()
 
 def plot_cv_pr_curve(classifier=None, cv=None, n_splits=10, X=None, y=None, RESULTS_DIR='', title='Cross-Validated PR Curve', show=False, save=False, dpi=300):
@@ -294,14 +318,16 @@
 
     plt.xlim([-0.05, 1.05])
     plt.ylim([-0.05, 1.05])
     plt.xlabel('Recall')
     plt.ylabel('Precision')
     plt.title(title)
     plt.legend(bbox_to_anchor=(1, 1))
+    # plt.tight_layout()
+    plt.grid()
     if save:
         plt.savefig(RESULTS_DIR+'/crossvalidation_pr_curve.png', bbox_inches='tight',dpi=dpi)   
     if show:
         plt.show()
     plt.close()
 
 # def plot_shap_summary(model=None, X_train=None, X_test=None, show=False, save=False, RESULTS_DIR=None):
@@ -310,15 +336,15 @@
 #     shap.summary_plot(shap_values=shap_values, features=X_test, matplotlib=True, show=False)
 #     if save:
 #         plt.savefig(RESULTS_DIR+'/shap_summary_plot.png', bbox_inches='tight',dpi=dpi)   
 #     if show:
 #         plt.show()
 #     plt.close()
     
-def eval_model( trained_model=None, untrained_model=None,
+def eval_classification( trained_model=None, untrained_model=None, n_splits=10,
                 X=None, y=None, X_train=None, X_test=None, 
                 y_train=None, y_test=None, y_pred=None, y_pred_proba=None, 
                 class_names=None, 
                 save=False, RESULTS_DIR=None,
                 show=False, dpi=300):
 
     if save:
@@ -381,21 +407,23 @@
                                     save=save)
 
     if untrained_model is not None and X is not None and y is not None:
         assert len(X) == len(y), "[Length Mismatch]: Number of samples not equal to number of class labels"    
         plot_cv_roc_curve(classifier=untrained_model, 
                             X=X, 
                             y=pd.Series(y), 
+                            n_splits=n_splits,
                             RESULTS_DIR=RESULTS_DIR, 
                             title='Cross Validated ROC Curve', 
                             dpi=dpi,
                             show=show, 
                             save=save)
         
         plot_cv_pr_curve(classifier=untrained_model,  
                             X=X, 
                             y=pd.Series(y), 
+                            n_splits=n_splits,
                             RESULTS_DIR=RESULTS_DIR, 
                             title='Cross Validated PR Curve', 
                             dpi=dpi,
                             show=show, 
                             save=save)
```

### Comparing `bcutils4r-0.0.21/src/bcutils4r.egg-info/PKG-INFO` & `bcutils4r-0.0.22/src/bcutils4r.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcutils4r
-Version: 0.0.21
+Version: 0.0.22
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
-<!-- ![cm](tests/DetectPulsarStar/results/confusion_matrix.png) -->
-<!-- ![cm](https://github.com/rutujagurav/bcutils4r/blob/master/tests/DetectPulsarStar/results/confusion_matrix.png) -->
+![cm](tests/example_classification/results/confusion_matrix.png)
+<!-- ![cm](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/confusion_matrix.png) -->
 
 <!-- ### Class-wise ROC curve -->
-<!-- ![roc](tests/DetectPulsarStar/results/classwise_roc_curve.png) -->
-<!-- ![roc](https://github.com/rutujagurav/bcutils4r/blob/master/tests/DetectPulsarStar/results/classwise_roc_curve.png) -->
+![roc](tests/example_classification/results/classwise_roc_curve.png)
+<!-- ![roc](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/classwise_roc_curve.png) -->
 
 <!-- ### Class-wise PR curve -->
-<!-- ![pr](tests/DetectPulsarStar/results/classwise_pr_curve.png) -->
-<!-- ![pr](https://github.com/rutujagurav/bcutils4r/blob/master/tests/DetectPulsarStar/results/classwise_pr_curve.png) -->
+![pr](tests/example_classification/results/classwise_pr_curve.png)
+<!-- ![pr](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/classwise_pr_curve.png) -->
 
 <!-- ### KS statistic  -->
-<!-- ![ks_stat](tests/DetectPulsarStar/results/ks_stat.png) -->
-<!-- ![ks_stat](https://github.com/rutujagurav/bcutils4r/blob/master/tests/DetectPulsarStar/results/ks_stat.png) -->
+![ks_stat](tests/example_classification/results/ks_stat.png)
+<!-- ![ks_stat](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/ks_stat.png) -->
 
 <!-- ### Lift Curve  -->
-<!-- ![lift](tests/DetectPulsarStar/results/lift_curve.png) -->
-<!-- ![lift](https://github.com/rutujagurav/bcutils4r/blob/master/tests/DetectPulsarStar/results/lift_curve.png) -->
+![lift](tests/example_classification/results/lift_curve.png)
+<!-- ![lift](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/lift_curve.png) -->
 
 <!-- ### Cross-validated ROC curves -->
-<!-- ![cv_roc](tests/DetectPulsarStar/results/crossvalidation_roc_curve.png) -->
-<!-- ![cv_roc](https://github.com/rutujagurav/bcutils4r/blob/master/tests/DetectPulsarStar/results/crossvalidation_roc_curve.png) -->
+![cv_roc](tests/example_classification/results/crossvalidation_roc_curve.png)
+<!-- ![cv_roc](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/crossvalidation_roc_curve.png) -->
 
 <!-- ### Cross-validated PR curves -->
-<!-- ![cv_pr](tests/DetectPulsarStar/results/crossvalidation_pr_curve.png) -->
-<!-- ![cv_pr](https://github.com/rutujagurav/bcutils4r/blob/master/tests/DetectPulsarStar/results/crossvalidation_pr_curve.png) -->
+![cv_pr](tests/example_classification/results/crossvalidation_pr_curve.png)
+<!-- ![cv_pr](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/crossvalidation_pr_curve.png) -->
```

