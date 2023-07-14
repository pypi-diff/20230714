# Comparing `tmp/clustutils4r-0.0.3.tar.gz` & `tmp/clustutils4r-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clustutils4r-0.0.3.tar", last modified: Thu Jul 13 09:03:56 2023, max compression
+gzip compressed data, was "clustutils4r-0.0.4.tar", last modified: Fri Jul 14 00:22:25 2023, max compression
```

## Comparing `clustutils4r-0.0.3.tar` & `clustutils4r-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-13 09:03:56.231658 clustutils4r-0.0.3/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    35128 2023-07-13 07:56:53.000000 clustutils4r-0.0.3/LICENSE
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     3495 2023-07-13 09:03:56.231658 clustutils4r-0.0.3/PKG-INFO
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     2863 2023-07-13 08:52:52.000000 clustutils4r-0.0.3/README.md
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      659 2023-07-13 09:03:19.000000 clustutils4r-0.0.3/pyproject.toml
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       38 2023-07-13 09:03:56.231658 clustutils4r-0.0.3/setup.cfg
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      978 2023-07-13 09:03:15.000000 clustutils4r-0.0.3/setup.py
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-13 09:03:56.227658 clustutils4r-0.0.3/src/
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-13 09:03:56.231658 clustutils4r-0.0.3/src/clustutils4r/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        0 2023-07-13 05:33:28.000000 clustutils4r-0.0.3/src/clustutils4r/__init__.py
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    25402 2023-07-13 08:55:31.000000 clustutils4r-0.0.3/src/clustutils4r/eval_clustering.py
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-13 09:03:56.231658 clustutils4r-0.0.3/src/clustutils4r.egg-info/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     3495 2023-07-13 09:03:56.000000 clustutils4r-0.0.3/src/clustutils4r.egg-info/PKG-INFO
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      305 2023-07-13 09:03:56.000000 clustutils4r-0.0.3/src/clustutils4r.egg-info/SOURCES.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        1 2023-07-13 09:03:56.000000 clustutils4r-0.0.3/src/clustutils4r.egg-info/dependency_links.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       44 2023-07-13 09:03:56.000000 clustutils4r-0.0.3/src/clustutils4r.egg-info/requires.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       13 2023-07-13 09:03:56.000000 clustutils4r-0.0.3/src/clustutils4r.egg-info/top_level.txt
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-14 00:22:25.811096 clustutils4r-0.0.4/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    35128 2023-07-13 07:56:53.000000 clustutils4r-0.0.4/LICENSE
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     3779 2023-07-14 00:22:25.811096 clustutils4r-0.0.4/PKG-INFO
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     3147 2023-07-14 00:17:31.000000 clustutils4r-0.0.4/README.md
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      659 2023-07-14 00:21:40.000000 clustutils4r-0.0.4/pyproject.toml
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       38 2023-07-14 00:22:25.811096 clustutils4r-0.0.4/setup.cfg
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      978 2023-07-14 00:21:34.000000 clustutils4r-0.0.4/setup.py
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-14 00:22:25.811096 clustutils4r-0.0.4/src/
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-14 00:22:25.811096 clustutils4r-0.0.4/src/clustutils4r/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        0 2023-07-13 05:33:28.000000 clustutils4r-0.0.4/src/clustutils4r/__init__.py
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    25231 2023-07-14 00:18:19.000000 clustutils4r-0.0.4/src/clustutils4r/eval_clustering.py
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-14 00:22:25.811096 clustutils4r-0.0.4/src/clustutils4r.egg-info/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     3779 2023-07-14 00:22:25.000000 clustutils4r-0.0.4/src/clustutils4r.egg-info/PKG-INFO
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      305 2023-07-14 00:22:25.000000 clustutils4r-0.0.4/src/clustutils4r.egg-info/SOURCES.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        1 2023-07-14 00:22:25.000000 clustutils4r-0.0.4/src/clustutils4r.egg-info/dependency_links.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       44 2023-07-14 00:22:25.000000 clustutils4r-0.0.4/src/clustutils4r.egg-info/requires.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       13 2023-07-14 00:22:25.000000 clustutils4r-0.0.4/src/clustutils4r.egg-info/top_level.txt
```

### Comparing `clustutils4r-0.0.3/LICENSE` & `clustutils4r-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `clustutils4r-0.0.3/PKG-INFO` & `clustutils4r-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clustutils4r
-Version: 0.0.3
+Version: 0.0.4
 Summary: Wrapper around some basic sklearn utilities for clustering.
 Home-page: https://github.com/rutujagurav/clustutils4r
 Author: Rutuja Gurav
 Author-email: Rutuja Gurav <rutujagurav100@gmail.com>
 Project-URL: Homepage, https://github.com/rutujagurav/clustutils4r
 Project-URL: Bug Tracker, https://github.com/rutujagurav/clustutils4r/issues
 Classifier: Programming Language :: Python :: 3
@@ -16,19 +16,19 @@
 
 # Clustering Utilities
 
 This packages provides a simple convenience wrapper around some basic sklearn utilities for clustering. The only function available is `eval_clustering()`.
 
 ## Available Parameters
 
-`model`: clustering model object (untrained)
+`model`: Clustering model object (untrained)
 
-`X`: Pandas DataFrame containing preprocessed, normalized, complete dataset features
+`X`: Numpy array containing preprocessed, normalized, complete dataset features
 
-`gt_labels`: Pandas Series containing encoded ground-truth labels for `X` (often not available)
+`gt_labels`: Numpy array containing encoded ground-truth labels for `X` (often not available)
 
 `num_clusters`: Range of no. of clusters to grid search over.
 
 `num_runs`: No. of runs per no. of cluster (defaults = 10).
 
 `make_metrics_plots`: Plot various clustering evaluation metrics. Depending on whether `gt_labels` are provided, you will get one or more plots - one for non-ground truth-based metrics and another for ground truth-based metrics. (default = `True`).
 
@@ -48,39 +48,43 @@
 
 ## Example Usage
 ```python
 import os
 from sklearn import datasets
 
 # Load the iris dataset
-data = datasets.load_iris()
+data = datasets.load_digits()
 
 # Split the data into features and labels
 X = data.data
 y = data.target
 
 # Define clustering model
 from sklearn.cluster import KMeans
 kmeans_model = KMeans()
 
 # Run the evaluation
 from clustutils4r.eval_clustering import eval_clustering
-range_clusters = list(range(2,10+1))
+range_clusters = list(range(3,15+1))
 labelled_datapoints, nongt_metrics, gt_metrics \
     = eval_clustering(X=X, gt_labels=y,
-                        model=kmeans_model,
+                        model=KMeans(),
                         num_clusters=range_clusters, num_runs=10,
                         annotate_topN_best_scores=True, annotN=3,
                         make_metrics_plots=True,
-                        make_silhoutte_plots=False,
-                        show=True, save=True, 
-                        RESULTS_DIR=os.getcwd()+'/results',
+                        make_silhoutte_plots=True, embed_data_in_2d=True,
+                        show=True, 
+                        save=True, RESULTS_DIR=os.getcwd()+'/results',
                     )
 
 ```
 <!-- ### GT Metrics-->
-![cm](tests/example_clustering/results/feats_clustering_gt_metrics.png)
-<!-- ![cm](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/confusion_matrix.png) -->
+![gt](tests/example_clustering/results/feats_clustering_gt_metrics.png)
+<!-- ![gt](https://github.com/rutujagurav/clustutils4r/blob/master/tests/example_clustering/results/feats_clustering_gt_metrics.png) -->
 
 <!-- ### Non GT Metrics -->
-![roc](tests/example_clustering/results/feats_clustering_nongt_metrics.png)
-<!-- ![roc](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/classwise_roc_curve.png) -->
+![ngt](tests/example_clustering/results/feats_clustering_nongt_metrics.png)
+<!-- ![ngt](https://github.com/rutujagurav/clustutils4r/blob/master/tests/example_clustering/results/feats_clustering_nongt_metrics.png) -->
+
+<!-- ### Sil Plots -->
+![sil](tests/example_clustering/results/silhouette_plots/10_silhouette_plot.png)
+<!-- ![sil](https://github.com/rutujagurav/clustutils4r/blob/master/tests/example_clustering/results/silhouette_plots/10_silhouette_plot.png) -->
```

### Comparing `clustutils4r-0.0.3/README.md` & `clustutils4r-0.0.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Clustering Utilities
 
 This packages provides a simple convenience wrapper around some basic sklearn utilities for clustering. The only function available is `eval_clustering()`.
 
 ## Available Parameters
 
-`model`: clustering model object (untrained)
+`model`: Clustering model object (untrained)
 
-`X`: Pandas DataFrame containing preprocessed, normalized, complete dataset features
+`X`: Numpy array containing preprocessed, normalized, complete dataset features
 
-`gt_labels`: Pandas Series containing encoded ground-truth labels for `X` (often not available)
+`gt_labels`: Numpy array containing encoded ground-truth labels for `X` (often not available)
 
 `num_clusters`: Range of no. of clusters to grid search over.
 
 `num_runs`: No. of runs per no. of cluster (defaults = 10).
 
 `make_metrics_plots`: Plot various clustering evaluation metrics. Depending on whether `gt_labels` are provided, you will get one or more plots - one for non-ground truth-based metrics and another for ground truth-based metrics. (default = `True`).
 
@@ -32,39 +32,43 @@
 
 ## Example Usage
 ```python
 import os
 from sklearn import datasets
 
 # Load the iris dataset
-data = datasets.load_iris()
+data = datasets.load_digits()
 
 # Split the data into features and labels
 X = data.data
 y = data.target
 
 # Define clustering model
 from sklearn.cluster import KMeans
 kmeans_model = KMeans()
 
 # Run the evaluation
 from clustutils4r.eval_clustering import eval_clustering
-range_clusters = list(range(2,10+1))
+range_clusters = list(range(3,15+1))
 labelled_datapoints, nongt_metrics, gt_metrics \
     = eval_clustering(X=X, gt_labels=y,
-                        model=kmeans_model,
+                        model=KMeans(),
                         num_clusters=range_clusters, num_runs=10,
                         annotate_topN_best_scores=True, annotN=3,
                         make_metrics_plots=True,
-                        make_silhoutte_plots=False,
-                        show=True, save=True, 
-                        RESULTS_DIR=os.getcwd()+'/results',
+                        make_silhoutte_plots=True, embed_data_in_2d=True,
+                        show=True, 
+                        save=True, RESULTS_DIR=os.getcwd()+'/results',
                     )
 
 ```
 <!-- ### GT Metrics-->
-![cm](tests/example_clustering/results/feats_clustering_gt_metrics.png)
-<!-- ![cm](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/confusion_matrix.png) -->
+![gt](tests/example_clustering/results/feats_clustering_gt_metrics.png)
+<!-- ![gt](https://github.com/rutujagurav/clustutils4r/blob/master/tests/example_clustering/results/feats_clustering_gt_metrics.png) -->
 
 <!-- ### Non GT Metrics -->
-![roc](tests/example_clustering/results/feats_clustering_nongt_metrics.png)
-<!-- ![roc](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/classwise_roc_curve.png) -->
+![ngt](tests/example_clustering/results/feats_clustering_nongt_metrics.png)
+<!-- ![ngt](https://github.com/rutujagurav/clustutils4r/blob/master/tests/example_clustering/results/feats_clustering_nongt_metrics.png) -->
+
+<!-- ### Sil Plots -->
+![sil](tests/example_clustering/results/silhouette_plots/10_silhouette_plot.png)
+<!-- ![sil](https://github.com/rutujagurav/clustutils4r/blob/master/tests/example_clustering/results/silhouette_plots/10_silhouette_plot.png) -->
```

### Comparing `clustutils4r-0.0.3/pyproject.toml` & `clustutils4r-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clustutils4r"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Rutuja Gurav", email="rutujagurav100@gmail.com" },
 ]
 description = "Wrapper around some basic sklearn utilities for clustering."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers=[
```

### Comparing `clustutils4r-0.0.3/setup.py` & `clustutils4r-0.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="clustutils4r", # Replace with your own username
-    version="0.0.3",
+    version="0.0.4",
     author="Rutuja Gurav",
     author_email="rutujagurav100@gmail.com",
     description="Wrapper around some basic sklearn utilities for clustering.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rutujagurav/clustutils4r",
     project_urls={
```

### Comparing `clustutils4r-0.0.3/src/clustutils4r/eval_clustering.py` & `clustutils4r-0.0.4/src/clustutils4r/eval_clustering.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,8 @@
-from cProfile import label
-from turtle import title
 import warnings
-
-from torch import gt, le
 warnings.simplefilter(action='ignore', category=FutureWarning)
 import matplotlib.pyplot as plt
 plt.rcParams['font.family'] = 'serif'
 plt.rcParams['font.serif'] = ['Times New Roman'] + plt.rcParams['font.serif']
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 import seaborn as sns
 from sklearn.manifold import Isomap, SpectralEmbedding
@@ -316,15 +312,15 @@
                   model=None,
                   num_clusters = [2,3,5,10], num_runs=10, 
                   make_metrics_plots=True, annotate_topN_best_scores=False, annotN=3,
                   make_silhoutte_plots=True, embed_data_in_2d = False,
                   show=False, save=False, save_dir=None):
     
     if len(gt_labels)!=0:
-        print("Ground truth labels provided. Computing ground truth-based clustering metrics algon with non-ground truth based metrics.") 
+        print("Ground truth labels provided. Computing ground truth-based clustering metrics along with non-ground truth based metrics.") 
     
     labels = []
     gt_metrics = {}
     nongt_metrics = {}
 
     gt_metrics_mean, gt_metrics_std = {}, {}
     nongt_metrics_mean, nongt_metrics_std = {}, {}
@@ -351,15 +347,14 @@
 
             if nongt_metrics_[best_run_metric_] > best_score_:
                 best_run_id_ = run
                 best_score_ = nongt_metrics_[best_run_metric_]
                 best_run_sil_score_ = nongt_metrics_['Silhouette']
                 best_run_lbls_ = run_lbls_
             
-        ## This is using the last run's labels. TODO: Replace this with "best" score labels.
         print("[k={}] Best run is {} (out of {}) with {} score = {}"\
               .format(n_clusters, best_run_id_, num_runs, best_run_metric_, best_score_))
         cluster_labels = best_run_lbls_
         silhouette_avg = best_run_sil_score_
         labels.append(cluster_labels) 
         
         if len(gt_labels)!=0:
```

### Comparing `clustutils4r-0.0.3/src/clustutils4r.egg-info/PKG-INFO` & `clustutils4r-0.0.4/src/clustutils4r.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clustutils4r
-Version: 0.0.3
+Version: 0.0.4
 Summary: Wrapper around some basic sklearn utilities for clustering.
 Home-page: https://github.com/rutujagurav/clustutils4r
 Author: Rutuja Gurav
 Author-email: Rutuja Gurav <rutujagurav100@gmail.com>
 Project-URL: Homepage, https://github.com/rutujagurav/clustutils4r
 Project-URL: Bug Tracker, https://github.com/rutujagurav/clustutils4r/issues
 Classifier: Programming Language :: Python :: 3
@@ -16,19 +16,19 @@
 
 # Clustering Utilities
 
 This packages provides a simple convenience wrapper around some basic sklearn utilities for clustering. The only function available is `eval_clustering()`.
 
 ## Available Parameters
 
-`model`: clustering model object (untrained)
+`model`: Clustering model object (untrained)
 
-`X`: Pandas DataFrame containing preprocessed, normalized, complete dataset features
+`X`: Numpy array containing preprocessed, normalized, complete dataset features
 
-`gt_labels`: Pandas Series containing encoded ground-truth labels for `X` (often not available)
+`gt_labels`: Numpy array containing encoded ground-truth labels for `X` (often not available)
 
 `num_clusters`: Range of no. of clusters to grid search over.
 
 `num_runs`: No. of runs per no. of cluster (defaults = 10).
 
 `make_metrics_plots`: Plot various clustering evaluation metrics. Depending on whether `gt_labels` are provided, you will get one or more plots - one for non-ground truth-based metrics and another for ground truth-based metrics. (default = `True`).
 
@@ -48,39 +48,43 @@
 
 ## Example Usage
 ```python
 import os
 from sklearn import datasets
 
 # Load the iris dataset
-data = datasets.load_iris()
+data = datasets.load_digits()
 
 # Split the data into features and labels
 X = data.data
 y = data.target
 
 # Define clustering model
 from sklearn.cluster import KMeans
 kmeans_model = KMeans()
 
 # Run the evaluation
 from clustutils4r.eval_clustering import eval_clustering
-range_clusters = list(range(2,10+1))
+range_clusters = list(range(3,15+1))
 labelled_datapoints, nongt_metrics, gt_metrics \
     = eval_clustering(X=X, gt_labels=y,
-                        model=kmeans_model,
+                        model=KMeans(),
                         num_clusters=range_clusters, num_runs=10,
                         annotate_topN_best_scores=True, annotN=3,
                         make_metrics_plots=True,
-                        make_silhoutte_plots=False,
-                        show=True, save=True, 
-                        RESULTS_DIR=os.getcwd()+'/results',
+                        make_silhoutte_plots=True, embed_data_in_2d=True,
+                        show=True, 
+                        save=True, RESULTS_DIR=os.getcwd()+'/results',
                     )
 
 ```
 <!-- ### GT Metrics-->
-![cm](tests/example_clustering/results/feats_clustering_gt_metrics.png)
-<!-- ![cm](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/confusion_matrix.png) -->
+![gt](tests/example_clustering/results/feats_clustering_gt_metrics.png)
+<!-- ![gt](https://github.com/rutujagurav/clustutils4r/blob/master/tests/example_clustering/results/feats_clustering_gt_metrics.png) -->
 
 <!-- ### Non GT Metrics -->
-![roc](tests/example_clustering/results/feats_clustering_nongt_metrics.png)
-<!-- ![roc](https://github.com/rutujagurav/bcutils4r/blob/master/tests/example_classification/results/classwise_roc_curve.png) -->
+![ngt](tests/example_clustering/results/feats_clustering_nongt_metrics.png)
+<!-- ![ngt](https://github.com/rutujagurav/clustutils4r/blob/master/tests/example_clustering/results/feats_clustering_nongt_metrics.png) -->
+
+<!-- ### Sil Plots -->
+![sil](tests/example_clustering/results/silhouette_plots/10_silhouette_plot.png)
+<!-- ![sil](https://github.com/rutujagurav/clustutils4r/blob/master/tests/example_clustering/results/silhouette_plots/10_silhouette_plot.png) -->
```

