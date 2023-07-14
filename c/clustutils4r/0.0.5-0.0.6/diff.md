# Comparing `tmp/clustutils4r-0.0.5.tar.gz` & `tmp/clustutils4r-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clustutils4r-0.0.5.tar", last modified: Fri Jul 14 00:29:24 2023, max compression
+gzip compressed data, was "clustutils4r-0.0.6.tar", last modified: Fri Jul 14 02:13:39 2023, max compression
```

## Comparing `clustutils4r-0.0.5.tar` & `clustutils4r-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-14 00:29:24.681324 clustutils4r-0.0.5/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    35128 2023-07-13 07:56:53.000000 clustutils4r-0.0.5/LICENSE
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     3823 2023-07-14 00:29:24.681324 clustutils4r-0.0.5/PKG-INFO
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     3191 2023-07-14 00:24:10.000000 clustutils4r-0.0.5/README.md
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      659 2023-07-14 00:28:49.000000 clustutils4r-0.0.5/pyproject.toml
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       38 2023-07-14 00:29:24.681324 clustutils4r-0.0.5/setup.cfg
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      978 2023-07-14 00:28:53.000000 clustutils4r-0.0.5/setup.py
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-14 00:29:24.681324 clustutils4r-0.0.5/src/
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-14 00:29:24.681324 clustutils4r-0.0.5/src/clustutils4r/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        0 2023-07-13 05:33:28.000000 clustutils4r-0.0.5/src/clustutils4r/__init__.py
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    25231 2023-07-14 00:18:19.000000 clustutils4r-0.0.5/src/clustutils4r/eval_clustering.py
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-14 00:29:24.681324 clustutils4r-0.0.5/src/clustutils4r.egg-info/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     3823 2023-07-14 00:29:24.000000 clustutils4r-0.0.5/src/clustutils4r.egg-info/PKG-INFO
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      305 2023-07-14 00:29:24.000000 clustutils4r-0.0.5/src/clustutils4r.egg-info/SOURCES.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        1 2023-07-14 00:29:24.000000 clustutils4r-0.0.5/src/clustutils4r.egg-info/dependency_links.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       44 2023-07-14 00:29:24.000000 clustutils4r-0.0.5/src/clustutils4r.egg-info/requires.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       13 2023-07-14 00:29:24.000000 clustutils4r-0.0.5/src/clustutils4r.egg-info/top_level.txt
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-14 02:13:39.458328 clustutils4r-0.0.6/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    35128 2023-07-13 07:56:53.000000 clustutils4r-0.0.6/LICENSE
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     4905 2023-07-14 02:13:39.458328 clustutils4r-0.0.6/PKG-INFO
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     4273 2023-07-14 02:12:15.000000 clustutils4r-0.0.6/README.md
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      659 2023-07-14 02:13:08.000000 clustutils4r-0.0.6/pyproject.toml
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       38 2023-07-14 02:13:39.458328 clustutils4r-0.0.6/setup.cfg
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      978 2023-07-14 02:13:12.000000 clustutils4r-0.0.6/setup.py
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-14 02:13:39.458328 clustutils4r-0.0.6/src/
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-14 02:13:39.458328 clustutils4r-0.0.6/src/clustutils4r/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        0 2023-07-13 05:33:28.000000 clustutils4r-0.0.6/src/clustutils4r/__init__.py
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    26853 2023-07-14 02:01:24.000000 clustutils4r-0.0.6/src/clustutils4r/eval_clustering.py
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-14 02:13:39.458328 clustutils4r-0.0.6/src/clustutils4r.egg-info/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     4905 2023-07-14 02:13:39.000000 clustutils4r-0.0.6/src/clustutils4r.egg-info/PKG-INFO
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      305 2023-07-14 02:13:39.000000 clustutils4r-0.0.6/src/clustutils4r.egg-info/SOURCES.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        1 2023-07-14 02:13:39.000000 clustutils4r-0.0.6/src/clustutils4r.egg-info/dependency_links.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       44 2023-07-14 02:13:39.000000 clustutils4r-0.0.6/src/clustutils4r.egg-info/requires.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       13 2023-07-14 02:13:39.000000 clustutils4r-0.0.6/src/clustutils4r.egg-info/top_level.txt
```

### Comparing `clustutils4r-0.0.5/LICENSE` & `clustutils4r-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `clustutils4r-0.0.5/README.md` & `clustutils4r-0.0.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: clustutils4r
+Version: 0.0.6
+Summary: Wrapper around some basic sklearn utilities for clustering.
+Home-page: https://github.com/rutujagurav/clustutils4r
+Author: Rutuja Gurav
+Author-email: Rutuja Gurav <rutujagurav100@gmail.com>
+Project-URL: Homepage, https://github.com/rutujagurav/clustutils4r
+Project-URL: Bug Tracker, https://github.com/rutujagurav/clustutils4r/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Clustering Utilities
 
 This packages provides a simple convenience wrapper around some basic sklearn utilities for clustering. The only function available is `eval_clustering()`.
 
 ## Installation
 `pip install clustutils4r`
 
@@ -60,18 +76,31 @@
                         make_metrics_plots=True,
                         make_silhoutte_plots=True, embed_data_in_2d=True,
                         show=True, 
                         save=True, RESULTS_DIR=os.getcwd()+'/results',
                     )
 
 ```
-<!-- ### GT Metrics-->
-![gt](tests/example_clustering/results/feats_clustering_gt_metrics.png)
-<!-- ![gt](https://github.com/rutujagurav/clustutils4r/blob/master/tests/example_clustering/results/feats_clustering_gt_metrics.png) -->
-
-<!-- ### Non GT Metrics -->
-![ngt](tests/example_clustering/results/feats_clustering_nongt_metrics.png)
-<!-- ![ngt](https://github.com/rutujagurav/clustutils4r/blob/master/tests/example_clustering/results/feats_clustering_nongt_metrics.png) -->
-
-<!-- ### Sil Plots -->
-![sil](tests/example_clustering/results/silhouette_plots/10_silhouette_plot.png)
-<!-- ![sil](https://github.com/rutujagurav/clustutils4r/blob/master/tests/example_clustering/results/silhouette_plots/10_silhouette_plot.png) -->
+
+![ch](tests/example_clustering/results/nongt_metrics_plots/cal_har.png)
+![sil](tests/example_clustering/results/nongt_metrics_plots/dav_bou.png)
+![sil](tests/example_clustering/results/nongt_metrics_plots/hopkn.png)
+![sil](tests/example_clustering/results/nongt_metrics_plots/sil.png)
+
+<!-- ![ch](https://github.com/rutujagurav/clustutils4r/blob/main/tests/example_clustering/results/nongt_metrics_plots/cal_har.png)
+![sil](https://github.com/rutujagurav/clustutils4r/blob/main/tests/example_clustering/results/nongt_metrics_plots/dav_bou.png)
+![sil](https://github.com/rutujagurav/clustutils4r/blob/main/tests/example_clustering/results/nongt_metrics_plots/hopkn.png)
+![sil](https://github.com/rutujagurav/clustutils4r/blob/main/tests/example_clustering/results/nongt_metrics_plots/sil.png) -->
+
+![fmi](tests/example_clustering/results/gt_metrics_plots/fmi.png)
+![mi](tests/example_clustering/results/gt_metrics_plots/mutual_info.png)
+![hcv](tests/example_clustering/results/gt_metrics_plots/hcv.png)
+![ri](tests/example_clustering/results/gt_metrics_plots/rand_index.png)
+
+<!-- ![fmi](https://github.com/rutujagurav/clustutils4r/blob/main/tests/example_clustering/results/gt_metrics_plots/fmi.png)
+![mi](https://github.com/rutujagurav/clustutils4r/blob/main/tests/example_clustering/results/gt_metrics_plots/mutual_info.png)
+![hcv](https://github.com/rutujagurav/clustutils4r/blob/main/tests/example_clustering/results/gt_metrics_plots/hcv.png)
+![ri](https://github.com/rutujagurav/clustutils4r/blob/main/tests/example_clustering/results/gt_metrics_plots/rand_index.png) -->
+
+![silplt](tests/example_clustering/results/silhouette_plots/10_silhouette_plot.png)
+
+<!-- ![silplt](https://github.com/rutujagurav/clustutils4r/blob/main/tests/example_clustering/results/silhouette_plots/10_silhouette_plot.png) -->
```

### Comparing `clustutils4r-0.0.5/pyproject.toml` & `clustutils4r-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clustutils4r"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Rutuja Gurav", email="rutujagurav100@gmail.com" },
 ]
 description = "Wrapper around some basic sklearn utilities for clustering."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers=[
```

### Comparing `clustutils4r-0.0.5/setup.py` & `clustutils4r-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="clustutils4r", # Replace with your own username
-    version="0.0.5",
+    version="0.0.6",
     author="Rutuja Gurav",
     author_email="rutujagurav100@gmail.com",
     description="Wrapper around some basic sklearn utilities for clustering.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rutujagurav/clustutils4r",
     project_urls={
```

### Comparing `clustutils4r-0.0.5/src/clustutils4r/eval_clustering.py` & `clustutils4r-0.0.6/src/clustutils4r/eval_clustering.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,126 +102,157 @@
         ami_scores_std = [0*0]*len(ami_scores_mean)
         nmi_scores_std = [0*0]*len(nmi_scores_mean)
         homogeneity_scores_std = [0*0]*len(homogeneity_scores_mean)
         completeness_scores_std = [0*0]*len(completeness_scores_mean)
         v_measure_scores_std = [0*0]*len(v_measure_scores_mean)
         fmi_scores_std = [0*0]*len(fmi_scores_mean)
     
-    fig, axs = plt.subplots(2, 2, figsize=(10,10))
-
+    # fig, axs = plt.subplots(2, 2, figsize=(10,10))
+    fig, ax = plt.subplots(1, 1, figsize=(5,5))
     ## RI
-    axs[0,0].plot(num_clusters, ri_scores_mean, label='RI')
-    axs[0,0].fill_between(num_clusters, 
+    ax.plot(num_clusters, ri_scores_mean, label='RI')
+    ax.fill_between(num_clusters, 
                         ri_scores_mean - ri_scores_std, 
                         ri_scores_mean + ri_scores_std, 
                         alpha=0.2)
     # axs[0,0].set_title("Rand Index")
     # axs[0,0].set_xlabel("No. of Clusters")
 
     ## ARI
-    axs[0,0].plot(num_clusters, ari_scores_mean, label='ARI')
-    axs[0,0].fill_between(num_clusters,
+    ax.plot(num_clusters, ari_scores_mean, label='ARI')
+    ax.fill_between(num_clusters,
                         ari_scores_mean - ari_scores_std,
                         ari_scores_mean + ari_scores_std,
                         alpha=0.2)
-    # axs[0,0].set_title("Adjusted Rand Index")
-    axs[0,0].set_xlabel("No. of Clusters")
+    ax.set_title("Rand Index")
+    ax.set_xlabel("No. of Clusters")
     # axs[0,0].set_ylim(0,1)
     if annotate_topN_best_scores:
         top_k_indices = np.array(ari_scores_mean).argsort()[-annotN:][::-1]
         for i in top_k_indices:
             value = ari_scores_mean[i]
-            axs[0,0].text(i+num_clusters[0], value, f'{num_clusters[i]}', color='red')
+            ax.text(i+num_clusters[0], value, f'{num_clusters[i]}', color='red')
+
+    ax.legend(title='Metric', loc='best')
+
+    plt.tight_layout()    
+    if save:
+        plt.savefig(os.path.join(save_dir, 'gt_metrics_plots/rand_index.png'), dpi=300)
+    if show:
+        plt.show()
+    plt.close()    
 
-    axs[0,0].legend(title='Metric', loc='best')
 
+    fig, ax = plt.subplots(1, 1, figsize=(5,5))
     ## MI
     # axs[0,1].plot(num_clusters, mi_scores_mean, label='MI')
     # axs[0,1].fill_between(num_clusters,
     #                     mi_scores_mean - mi_scores_std,
     #                     mi_scores_mean + mi_scores_std,
     #                     alpha=0.2)
 
     ## AMI
-    axs[0,1].plot(num_clusters, ami_scores_mean, label='AMI')
-    axs[0,1].fill_between(num_clusters,
+    ax.plot(num_clusters, ami_scores_mean, label='AMI')
+    ax.fill_between(num_clusters,
                         ami_scores_mean - ami_scores_std,
                         ami_scores_mean + ami_scores_std,
                         alpha=0.2)
 
     ## NMI
-    axs[0,1].plot(num_clusters, nmi_scores_mean, label='NMI')
-    axs[0,1].fill_between(num_clusters,
+    ax.plot(num_clusters, nmi_scores_mean, label='NMI')
+    ax.fill_between(num_clusters,
                         nmi_scores_mean - nmi_scores_std,
                         nmi_scores_mean + nmi_scores_std,
                         alpha=0.2)
     
-    axs[0,1].set_xlabel("No. of Clusters")
+    ax.set_xlabel("No. of Clusters")
     # axs[0,1].set_ylim(0,1)
     if annotate_topN_best_scores:
         top_k_indices = np.array(nmi_scores_mean).argsort()[-annotN:][::-1]
         for i in top_k_indices:
             value = nmi_scores_mean[i]
-            axs[0,1].text(i+num_clusters[0], value, f'{num_clusters[i]}', color='red')
-    axs[0,1].legend(title='Metric', loc='best')
+            ax.text(i+num_clusters[0], value, f'{num_clusters[i]}', color='red')
+    ax.legend(title='Metric', loc='best')
+
+    plt.tight_layout()    
+    if save:
+        plt.savefig(os.path.join(save_dir, 'gt_metrics_plots/mutual_info.png'), dpi=300)
+    if show:
+        plt.show()
+    plt.close()
 
+    fig, ax = plt.subplots(1, 1, figsize=(5,5))
     ## Homogeneity
-    axs[1,0].plot(num_clusters, homogeneity_scores_mean, label='Homogeneity')
-    axs[1,0].fill_between(num_clusters,
+    ax.plot(num_clusters, homogeneity_scores_mean, label='Homogeneity')
+    ax.fill_between(num_clusters,
                         homogeneity_scores_mean - homogeneity_scores_std,
                         homogeneity_scores_mean + homogeneity_scores_std,
                         alpha=0.2)
 
     ## Completeness
-    axs[1,0].plot(num_clusters, completeness_scores_mean, label='Completeness')
-    axs[1,0].fill_between(num_clusters,
+    ax.plot(num_clusters, completeness_scores_mean, label='Completeness')
+    ax.fill_between(num_clusters,
                         completeness_scores_mean - completeness_scores_std,
                         completeness_scores_mean + completeness_scores_std,
                         alpha=0.2)
 
     ## V-Measure
-    axs[1,0].plot(num_clusters, v_measure_scores_mean, label='V-Measure')
-    axs[1,0].fill_between(num_clusters,
+    ax.plot(num_clusters, v_measure_scores_mean, label='V-Measure')
+    ax.fill_between(num_clusters,
                         v_measure_scores_mean - v_measure_scores_std,
                         v_measure_scores_mean + v_measure_scores_std,
                         alpha=0.2)
     
-    axs[1,0].set_xlabel("No. of Clusters")
-    # axs[1,0].set_ylim(0,1)
+    ax.set_xlabel("No. of Clusters")
+    # ax.set_ylim(0,1)
     if annotate_topN_best_scores:
         top_k_indices = np.array(v_measure_scores_mean).argsort()[-annotN:][::-1]
         for i in top_k_indices:
             value = v_measure_scores_mean[i]
-            axs[1,0].text(i+num_clusters[0], value, f'{num_clusters[i]}', color='red')
-    axs[1,0].legend(title='Metric', loc='best')
+            ax.text(i+num_clusters[0], value, f'{num_clusters[i]}', color='red')
+    ax.legend(title='Metric', loc='best')
+
+    plt.tight_layout()    
+    if save:
+        plt.savefig(os.path.join(save_dir, 'gt_metrics_plots/hcv.png'), dpi=300)
+    if show:
+        plt.show()
+    plt.close()
 
+    fig, ax = plt.subplots(1, 1, figsize=(5,5))
     ## FMI
-    axs[1,1].plot(num_clusters, fmi_scores_mean, label='FMI')
-    axs[1,1].fill_between(num_clusters,
+    ax.plot(num_clusters, fmi_scores_mean, label='FMI')
+    ax.fill_between(num_clusters,
                         fmi_scores_mean - fmi_scores_std,
                         fmi_scores_mean + fmi_scores_std,
                         alpha=0.2)
-    # axs[1,1].set_title("Fowlkes-Mallows Index")
-    axs[1,1].set_xlabel("No. of Clusters")
-    # axs[1,1].set_ylim(0,1)
+    ax.set_title("Fowlkes-Mallows Index")
+    ax.set_xlabel("No. of Clusters")
+    # ax.set_ylim(0,1)
     if annotate_topN_best_scores:
         top_k_indices = np.array(fmi_scores_mean).argsort()[-annotN:][::-1]
         for i in top_k_indices:
             value = fmi_scores_mean[i]
-            axs[1,1].text(i+num_clusters[0], value, f'{num_clusters[i]}', color='red')
-    axs[1,1].legend(title='Metric', loc='best')
-
-
+            ax.text(i+num_clusters[0], value, f'{num_clusters[i]}', color='red')
+    # axs[1,1].legend(title='Metric', loc='best')
     plt.tight_layout()    
     if save:
-        print("Saving ground truth-based clustering metrics plot at {}".format(os.path.join(save_dir, 'feats_clustering_metrics.png')))
-        plt.savefig(os.path.join(save_dir, 'feats_clustering_gt_metrics.png'), dpi=300)
+        plt.savefig(os.path.join(save_dir, 'gt_metrics_plots/fmi.png'), dpi=300)
     if show:
         plt.show()
-    plt.close()    
+    plt.close()
+
+
+    # plt.tight_layout()    
+    # if save:
+    #     print("Saving ground truth-based clustering metrics plot at {}".format(os.path.join(save_dir, 'feats_clustering_metrics.png')))
+    #     plt.savefig(os.path.join(save_dir, 'feats_clustering_gt_metrics.png'), dpi=300)
+    # if show:
+    #     plt.show()
+    # plt.close()    
 
 
 def plot_nongt_metrics(nongt_metrics=None, 
                        num_clusters=None, annotate_topN_best_scores=False, annotN=3,
                        show=False, save=False, save_dir=None):
     if isinstance(nongt_metrics, dict):
         sil_scores_mean = nongt_metrics['mean']['Silhouette'].values
@@ -241,76 +272,110 @@
         hpkn_scores_mean = nongt_metrics['Hopkins'].values
 
         sil_scores_std = [0.0]*len(sil_scores_mean)
         ch_scores_std = [0.0]*len(ch_scores_mean)
         db_scores_std = [0.0]*len(db_scores_mean)
         hpkn_scores_std = [0.0]*len(hpkn_scores_mean)
     
-    fig, axs = plt.subplots(2,2, figsize=(10,10))
+    # fig, axs = plt.subplots(2,2, figsize=(10,10))
 
+    fig, ax = plt.subplots(1, 1, figsize=(5,5))
     ## Silhouette
-    axs[0,0].plot(num_clusters, sil_scores_mean)
-    axs[0,0].fill_between(num_clusters, 
+    ax.plot(num_clusters, sil_scores_mean)
+    ax.fill_between(num_clusters, 
                         sil_scores_mean - sil_scores_std, 
                         sil_scores_mean + sil_scores_std, 
                         color='b', alpha=0.2)
-    axs[0,0].set_title("Avg. Silhoutte Score\n(-1=incorrect, 0=overlap, 1=dense)")
-    axs[0,0].set_xlabel("No. of Clusters")
-    axs[0,0].set_ylim(-1.1,1.1)
+    ax.set_title("Avg. Silhoutte Score\n(-1=incorrect, 0=overlap, 1=dense)")
+    ax.set_xlabel("No. of Clusters")
+    ax.set_ylim(-1.1,1.1)
 
+    plt.tight_layout()    
+    if save:
+        plt.savefig(os.path.join(save_dir, 'nongt_metrics_plots/sil.png'), dpi=300)
+    if show:
+        plt.show()
+    plt.close()
+    
+    
+    fig, ax = plt.subplots(1, 1, figsize=(5,5))
     ## Calinski-Harabasz
-    axs[1,0].plot(num_clusters, ch_scores_mean)
-    axs[1,0].fill_between(num_clusters, 
+    ax.plot(num_clusters, ch_scores_mean)
+    ax.fill_between(num_clusters, 
                         ch_scores_mean - ch_scores_std, 
                         ch_scores_mean + ch_scores_std, 
                         color='b', alpha=0.2)
-    axs[1,0].set_title("Calinski Harabasz Score\n(higher=dense,well-separated)")
-    axs[1,0].set_xlabel("No. of Clusters")
+    ax.set_title("Calinski Harabasz Score\n(higher=dense,well-separated)")
+    ax.set_xlabel("No. of Clusters")
     
     if annotate_topN_best_scores:
         # # top_k_indices = sorted(range(len(ch_scores)), key=lambda i: ch_scores[i], reverse=True)[:k]
         top_k_indices = np.array(ch_scores_mean).argsort()[-annotN:][::-1]
         for i in top_k_indices:
             value = ch_scores_mean[i]
-            axs[1,0].text(i+num_clusters[0], value, f'{num_clusters[i]}', color='red')
+            ax.text(i+num_clusters[0], value, f'{num_clusters[i]}', color='red')
 
+    plt.tight_layout()    
+    if save:
+        plt.savefig(os.path.join(save_dir, 'nongt_metrics_plots/cal_har.png'), dpi=300)
+    if show:
+        plt.show()
+    plt.close()
+
+
+    fig, ax = plt.subplots(1, 1, figsize=(5,5))
     ## Davies-Bouldin
-    axs[1,1].plot(num_clusters, db_scores_mean)
-    axs[1,1].fill_between(num_clusters, 
+    ax.plot(num_clusters, db_scores_mean)
+    ax.fill_between(num_clusters, 
                         db_scores_mean - db_scores_std, 
                         db_scores_mean + db_scores_std, 
                         color='b', alpha=0.2)
-    axs[1,1].set_title("Davies Bouldin Score\n(lower=better)")
-    axs[1,1].set_xlabel("No. of Clusters") 
+    ax.set_title("Davies Bouldin Score\n(lower=better)")
+    ax.set_xlabel("No. of Clusters") 
     
     if annotate_topN_best_scores:
         # # top_k_indices = sorted(range(len(db_scores)), key=lambda i: db_scores[i], reverse=False)[:k]
         top_k_indices = np.array(db_scores_mean).argsort()[:annotN]
         for i in top_k_indices:
             value = db_scores_mean[i]
-            axs[1,1].text(i+num_clusters[0], value, f'{num_clusters[i]}', color='red')
+            ax.text(i+num_clusters[0], value, f'{num_clusters[i]}', color='red')
     
+    plt.tight_layout()    
+    if save:
+        plt.savefig(os.path.join(save_dir, 'nongt_metrics_plots/dav_bou.png'), dpi=300)
+    if show:
+        plt.show()
+    plt.close()
+    
+    fig, ax = plt.subplots(1, 1, figsize=(5,5))
     ## Hopkins
-    axs[0,1].plot(num_clusters, hpkn_scores_mean)
-    axs[0,1].fill_between(num_clusters, 
+    ax.plot(num_clusters, hpkn_scores_mean)
+    ax.fill_between(num_clusters, 
                         hpkn_scores_mean - hpkn_scores_std, 
                         hpkn_scores_mean + hpkn_scores_std, 
                         color='b', alpha=0.2)
-    axs[0,1].set_title("Hopkins Statistic\n(1=clustered, 0.5=random, 0=uniforrm)")
-    axs[0,1].set_xlabel("No. of Clusters")
-    axs[0,1].set_ylim(-0.1,1.1) 
+    ax.set_title("Hopkins Statistic\n(1=clustered, 0.5=random, 0=uniforrm)")
+    ax.set_xlabel("No. of Clusters")
+    ax.set_ylim(-0.1,1.1) 
 
     plt.tight_layout()    
     if save:
-        print("Saving non-ground truth-based clustering metrics plot at {}".format(os.path.join(save_dir, 'feats_clustering_metrics.png')))
-        plt.savefig(os.path.join(save_dir, 'feats_clustering_nongt_metrics.png'), dpi=300)
+        plt.savefig(os.path.join(save_dir, 'nongt_metrics_plots/hopkn.png'), dpi=300)
     if show:
         plt.show()
     plt.close()
 
+    # plt.tight_layout()    
+    # if save:
+    #     print("Saving non-ground truth-based clustering metrics plot at {}".format(os.path.join(save_dir, 'feats_clustering_metrics.png')))
+    #     plt.savefig(os.path.join(save_dir, 'feats_clustering_nongt_metrics.png'), dpi=300)
+    # if show:
+    #     plt.show()
+    # plt.close()
+
 def cluster_feats(X=None, gt_labels=[],
                 #   algorithm='k-Means',
                   model=None,
                   num_clusters = [2,3,5,10], num_runs=10, 
                   make_metrics_plots=True, annotate_topN_best_scores=False, annotN=3,
                   make_silhoutte_plots=True, embed_data_in_2d = False,
                   show=False, save=False, save_dir=None):
@@ -535,14 +600,16 @@
                     distance_metric='euclidean',
                     show=False, save=False, RESULTS_DIR=None, 
                     make_metrics_plots=True, annotate_topN_best_scores=True, annotN=3,
                     make_silhoutte_plots=False, embed_data_in_2d=False):
     
     if not os.path.exists(RESULTS_DIR):
         os.makedirs(RESULTS_DIR+'/silhouette_plots')
+        os.makedirs(RESULTS_DIR+'/gt_metrics_plots')
+        os.makedirs(RESULTS_DIR+'/nongt_metrics_plots')
     
     # if dataset_type == 'features':
     return cluster_feats(X=X, gt_labels=gt_labels, 
                         model=model,
                         # algorithm=algorithm,
                         num_clusters=num_clusters, num_runs=num_runs,
                         show=show, save=save, save_dir=RESULTS_DIR,
```

