# Comparing `tmp/checkatlas-0.3.0.tar.gz` & `tmp/checkatlas-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkatlas-0.3.0.tar", max compression
+gzip compressed data, was "checkatlas-0.3.1.tar", max compression
```

## Comparing `checkatlas-0.3.0.tar` & `checkatlas-0.3.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1506 2023-07-11 21:43:46.215059 checkatlas-0.3.0/LICENSE
--rw-r--r--   0        0        0     4452 2023-07-11 21:43:46.215059 checkatlas-0.3.0/README.md
--rw-r--r--   0        0        0      111 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/__init__.py
--rw-r--r--   0        0        0     4648 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/__main__.py
--rw-r--r--   0        0        0    24191 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/atlas.py
--rw-r--r--   0        0        0     4715 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/cellranger.py
--rw-r--r--   0        0        0     4236 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/checkatlas.py
--rw-r--r--   0        0        0       45 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/__init__.py
--rw-r--r--   0        0        0      192 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/annot/__init__.py
--rw-r--r--   0        0        0      242 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/annot/adj_mutual_info.py
--rw-r--r--   0        0        0      153 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/annot/dunn_index.py
--rw-r--r--   0        0        0      232 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/annot/fowlkes_mallow.py
--rw-r--r--   0        0        0      228 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/annot/rand_index.py
--rw-r--r--   0        0        0      220 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/annot/vmeasure.py
--rw-r--r--   0        0        0      125 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/cluster/__init__.py
--rw-r--r--   0        0        0      225 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/cluster/calinski_harabasz.py
--rw-r--r--   0        0        0      219 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/cluster/davies_bouldin.py
--rw-r--r--   0        0        0      211 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/cluster/silhouette.py
--rw-r--r--   0        0        0       89 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/dimred/__init__.py
--rw-r--r--   0        0        0      602 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/dimred/kruskal_stress.py
--rw-r--r--   0        0        0      162 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/dimred/spearman_rho.py
--rw-r--r--   0        0        0     4108 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/metrics.py
--rw-r--r--   0        0        0        0 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/specificity/__init__.py
--rw-r--r--   0        0        0     6278 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/specificity/analysis.py
--rw-r--r--   0        0        0     8417 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/specificity/compute.py
--rw-r--r--   0        0        0     4107 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/specificity/get_data.py
--rw-r--r--   0        0        0     9993 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/metrics/specificity/plot.py
--rw-r--r--   0        0        0    20167 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/seurat.py
--rw-r--r--   0        0        0      107 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/utils/__init__.py
--rw-r--r--   0        0        0     4544 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/utils/checkatlas_arguments.py
--rw-r--r--   0        0        0     2230 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/utils/files.py
--rw-r--r--   0        0        0     1960 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/utils/folders.py
--rw-r--r--   0        0        0     6267 2023-07-11 21:43:46.215059 checkatlas-0.3.0/checkatlas/utils/obsolete_arguments.py
--rw-r--r--   0        0        0     1350 2023-07-11 21:43:46.399061 checkatlas-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5726 1970-01-01 00:00:00.000000 checkatlas-0.3.0/setup.py
--rw-r--r--   0        0        0     5395 1970-01-01 00:00:00.000000 checkatlas-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1506 2023-07-14 13:45:51.118752 checkatlas-0.3.1/LICENSE
+-rw-r--r--   0        0        0     4452 2023-07-14 13:45:51.118752 checkatlas-0.3.1/README.md
+-rw-r--r--   0        0        0      111 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/__init__.py
+-rw-r--r--   0        0        0     4648 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/__main__.py
+-rw-r--r--   0        0        0    24201 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/atlas.py
+-rw-r--r--   0        0        0     4715 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/cellranger.py
+-rw-r--r--   0        0        0     8494 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/checkatlas.py
+-rw-r--r--   0        0        0       45 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/__init__.py
+-rw-r--r--   0        0        0      192 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/annot/__init__.py
+-rw-r--r--   0        0        0      242 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/annot/adj_mutual_info.py
+-rw-r--r--   0        0        0      153 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/annot/dunn_index.py
+-rw-r--r--   0        0        0      232 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/annot/fowlkes_mallow.py
+-rw-r--r--   0        0        0      228 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/annot/rand_index.py
+-rw-r--r--   0        0        0      220 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/annot/vmeasure.py
+-rw-r--r--   0        0        0      125 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/cluster/__init__.py
+-rw-r--r--   0        0        0      225 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/cluster/calinski_harabasz.py
+-rw-r--r--   0        0        0      219 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/cluster/davies_bouldin.py
+-rw-r--r--   0        0        0      211 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/cluster/silhouette.py
+-rw-r--r--   0        0        0       89 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/dimred/__init__.py
+-rw-r--r--   0        0        0      602 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/dimred/kruskal_stress.py
+-rw-r--r--   0        0        0      162 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/dimred/spearman_rho.py
+-rw-r--r--   0        0        0     4108 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/metrics.py
+-rw-r--r--   0        0        0        0 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/specificity/__init__.py
+-rw-r--r--   0        0        0     6278 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/specificity/analysis.py
+-rw-r--r--   0        0        0     8417 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/specificity/compute.py
+-rw-r--r--   0        0        0     4107 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/specificity/get_data.py
+-rw-r--r--   0        0        0     9993 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/metrics/specificity/plot.py
+-rw-r--r--   0        0        0    20177 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/seurat.py
+-rw-r--r--   0        0        0      107 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/utils/__init__.py
+-rw-r--r--   0        0        0     4544 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/utils/checkatlas_arguments.py
+-rw-r--r--   0        0        0     2230 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/utils/files.py
+-rw-r--r--   0        0        0     2065 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/utils/folders.py
+-rw-r--r--   0        0        0     6267 2023-07-14 13:45:51.118752 checkatlas-0.3.1/checkatlas/utils/obsolete_arguments.py
+-rw-r--r--   0        0        0     1350 2023-07-14 13:45:51.342770 checkatlas-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5726 1970-01-01 00:00:00.000000 checkatlas-0.3.1/setup.py
+-rw-r--r--   0        0        0     5395 1970-01-01 00:00:00.000000 checkatlas-0.3.1/PKG-INFO
```

### Comparing `checkatlas-0.3.0/LICENSE` & `checkatlas-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.0/README.md` & `checkatlas-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.0/checkatlas/__main__.py` & `checkatlas-0.3.1/checkatlas/__main__.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.0/checkatlas/atlas.py` & `checkatlas-0.3.1/checkatlas/atlas.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,15 +301,15 @@
         args (argparse.Namespace): list of arguments from checkatlas workflow
     """
     atlas_name = atlas_info[checkatlas.ATLAS_NAME_KEY]
     atlas_type = atlas_info[checkatlas.ATLAS_TYPE_KEY]
     atlas_path = atlas_info[checkatlas.ATLAS_PATH_KEY]
     logger.debug(f"Create Summary table for {atlas_name}")
     csv_path = files.get_file_path(
-        atlas_name, folders.SUMMARY, checkatlas.SUMMARY_EXTENSION, args.path
+        atlas_name, folders.SUMMARY, checkatlas.TSV_EXTENSION, args.path
     )
     # Create summary table
     header = [
         "AtlasFileType",
         "NbCells",
         "NbGenes",
         "AnnData.raw",
@@ -339,25 +339,25 @@
         atlas_info (dict): info on the atlas
         args (argparse.Namespace): list of arguments from checkatlas workflow
     """
     atlas_name = atlas_info[checkatlas.ATLAS_NAME_KEY]
 
     logger.debug(f"Create Adata table for {atlas_name}")
     csv_path = files.get_file_path(
-        atlas_name, folders.ANNDATA, checkatlas.ADATA_EXTENSION, args.path
+        atlas_name, folders.ANNDATA, checkatlas.TSV_EXTENSION, args.path
     )
     # Create AnnData table
-    header = ["obs", "obsm", "var", "varm", "uns"]
+    header = ["atlas_obs", "obsm", "var", "varm", "uns"]
     df_summary = pd.DataFrame(index=[atlas_name], columns=header)
     # html_element = "<span class=\"label label-primary\">"
     # new_line = ''
     # for value in list(adata.obs.columns):
     #     new_line += html_element + value + "</span><br>"
     #     print(new_line)
-    df_summary["obs"][atlas_name] = (
+    df_summary["atlas_obs"][atlas_name] = (
         "<code>"
         + "</code><br><code>".join(list(adata.obs.columns))
         + "</code>"
     )
     df_summary["obsm"][atlas_name] = (
         "<code>"
         + "</code><br><code>".join(list(adata.obsm_keys()))
@@ -388,15 +388,15 @@
     Args:
         adata (AnnData): atlas to analyse
         atlas_info (dict): info on the atlas
         args (argparse.Namespace): list of arguments from checkatlas workflow
     """
     atlas_name = atlas_info[checkatlas.ATLAS_NAME_KEY]
     qc_path = files.get_file_path(
-        atlas_name, folders.QC, checkatlas.QC_EXTENSION, args.path
+        atlas_name, folders.QC, checkatlas.TSV_EXTENSION, args.path
     )
     logger.debug(f"Create QC tables for {atlas_name}")
     qc_genes = []
     # mitochondrial genes
     adata.var["mt"] = adata.var_names.str.startswith("MT-")
     if len(adata.var[adata.var["mt"]]) != 0:
         qc_genes.append("mt")
@@ -569,27 +569,27 @@
         atlas_info (dict): path of the atlas
         args (argparse.Namespace): list of arguments from checkatlas workflow
     """
     atlas_name = atlas_info[checkatlas.ATLAS_NAME_KEY]
     csv_path = files.get_file_path(
         atlas_name,
         folders.CLUSTER,
-        checkatlas.METRIC_CLUSTER_EXTENSION,
+        checkatlas.TSV_EXTENSION,
         args.path,
     )
-    header = ["Sample", "obs"] + args.metric_cluster
+    header = ["Clust_Sample", "obs"] + args.metric_cluster
     df_cluster = pd.DataFrame(columns=header)
     obs_keys = get_viable_obs_annot(adata, args)
     obsm_key_representation = "X_umap"
 
     if len(obs_keys) > 0:
         logger.debug(f"Calc clustering metrics for {atlas_name}")
         for obs_key in obs_keys:
             dict_line = {
-                "Sample": [atlas_name + "_" + obs_key],
+                "Clust_Sample": [atlas_name + "_" + obs_key],
                 "obs": [obs_key],
             }
             for metric in args.metric_cluster:
                 logger.debug(
                     f"Calc {metric} for {atlas_name} "
                     f"with obs {obs_key} and obsm {obsm_key_representation}"
                 )
@@ -617,27 +617,27 @@
         atlas_path (dict): path of the atlas
         args (argparse.Namespace): list of arguments from checkatlas workflow
     """
     atlas_name = atlas_info[checkatlas.ATLAS_NAME_KEY]
     csv_path = files.get_file_path(
         atlas_name,
         folders.ANNOTATION,
-        checkatlas.METRIC_ANNOTATION_EXTENSION,
+        checkatlas.TSV_EXTENSION,
         args.path,
     )
-    header = ["Sample", "Reference", "obs"] + args.metric_annot
+    header = ["Annot_Sample", "Reference", "obs"] + args.metric_annot
     df_annot = pd.DataFrame(columns=header)
     obs_keys = get_viable_obs_annot(adata, args)
     if len(obs_keys) > 1:
         logger.debug(f"Calc annotation metrics for {atlas_name}")
         ref_obs = obs_keys[0]
         for i in range(1, len(obs_keys)):
             obs_key = obs_keys[i]
             dict_line = {
-                "Sample": [atlas_name + "_" + obs_key],
+                "Annot_Sample": [atlas_name + "_" + obs_key],
                 "Reference": [ref_obs],
                 "obs": [obs_key],
             }
             for metric in args.metric_annot:
                 logger.debug(
                     f"Calc {metric} for {atlas_name} "
                     f"with obs {obs_key} vs ref_obs {ref_obs}"
@@ -666,25 +666,25 @@
         atlas_info (dict): path of the atlas
         args (argparse.Namespace): list of arguments from checkatlas workflow
     """
     atlas_name = atlas_info[checkatlas.ATLAS_NAME_KEY]
     csv_path = files.get_file_path(
         atlas_name,
         folders.DIMRED,
-        checkatlas.METRIC_DIMRED_EXTENSION,
+        checkatlas.TSV_EXTENSION,
         args.path,
     )
-    header = ["Sample", "obsm"] + args.metric_dimred
+    header = ["Dimred_Sample", "obsm"] + args.metric_dimred
     df_dimred = pd.DataFrame(columns=header)
     obsm_keys = get_viable_obsm(adata, args)
     if len(obsm_keys) > 0:
         logger.debug(f"Calc dim red metrics for {atlas_name}")
         for obsm_key in obsm_keys:
             dict_line = {
-                "Sample": [atlas_name + "_" + obsm_key],
+                "Dimred_Sample": [atlas_name + "_" + obsm_key],
                 "obsm": [obsm_key],
             }
             for metric in args.metric_dimred:
                 logger.debug(
                     f"Calc {metric} for {atlas_name} with obsm {obsm_key}"
                 )
                 metric_value = metrics.calc_metric_dimred(
```

### Comparing `checkatlas-0.3.0/checkatlas/cellranger.py` & `checkatlas-0.3.1/checkatlas/cellranger.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.0/checkatlas/metrics/dimred/kruskal_stress.py` & `checkatlas-0.3.1/checkatlas/metrics/dimred/kruskal_stress.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.0/checkatlas/metrics/metrics.py` & `checkatlas-0.3.1/checkatlas/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.0/checkatlas/metrics/specificity/analysis.py` & `checkatlas-0.3.1/checkatlas/metrics/specificity/analysis.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.0/checkatlas/metrics/specificity/compute.py` & `checkatlas-0.3.1/checkatlas/metrics/specificity/compute.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.0/checkatlas/metrics/specificity/get_data.py` & `checkatlas-0.3.1/checkatlas/metrics/specificity/get_data.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.0/checkatlas/metrics/specificity/plot.py` & `checkatlas-0.3.1/checkatlas/metrics/specificity/plot.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.0/checkatlas/seurat.py` & `checkatlas-0.3.1/checkatlas/seurat.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,15 +208,15 @@
     :param csv_path:
     :return:
     """
     atlas_name = atlas_info[checkatlas.ATLAS_NAME_KEY]
     logger.debug(f"Create Summary table for {atlas_name}")
     csv_path = os.path.join(
         folders.get_folder(args.path, folders.SUMMARY),
-        atlas_name + checkatlas.SUMMARY_EXTENSION,
+        atlas_name + checkatlas.TSV_EXTENSION,
     )
     # Create summary table
     header = [
         "AtlasFileType",
         "NbCells",
         "NbGenes",
         "AnnData.raw",
@@ -255,18 +255,18 @@
     :param atlas_path:
     :return:
     """
     atlas_name = atlas_info[checkatlas.ATLAS_NAME_KEY]
     logger.debug(f"Create Adata table for {atlas_name}")
     csv_path = os.path.join(
         folders.get_folder(args.path, folders.ANNDATA),
-        atlas_name + checkatlas.ADATA_EXTENSION,
+        atlas_name + checkatlas.TSV_EXTENSION,
     )
     # Create AnnData table
-    header = ["obs", "obsm", "var", "varm", "uns"]
+    header = ["atlas_obs", "obsm", "var", "varm", "uns"]
     df_summary = pd.DataFrame(index=[atlas_name], columns=header)
 
     # Create r_functions
     r_obs = robjects.r(
         "obs <- function(seurat){ return(colnames(seurat@meta.data))}"
     )
     r_obsm = robjects.r(
@@ -280,15 +280,15 @@
     obsm_list = r_obsm(seurat)
     var_list = [""]
     varm_list = [""]
     uns_list = [""]
     if not isinstance(r_uns(seurat), NULLType):
         uns_list = r_uns(seurat)
 
-    df_summary["obs"][atlas_name] = (
+    df_summary["atlas_obs"][atlas_name] = (
         "<code>" + "</code><br><code>".join(obs_list) + "</code>"
     )
     df_summary["obsm"][atlas_name] = (
         "<code>" + "</code><br><code>".join(obsm_list) + "</code>"
     )
     df_summary["var"][atlas_name] = (
         "<code>" + "</code><br><code>".join(var_list) + "</code>"
@@ -314,15 +314,15 @@
     :param atlas_name:
     :param atlas_path:
     :return:
     """
     atlas_name = atlas_info[checkatlas.ATLAS_NAME_KEY]
     qc_path = os.path.join(
         folders.get_folder(args.path, folders.QC),
-        atlas_name + checkatlas.QC_EXTENSION,
+        atlas_name + checkatlas.TSV_EXTENSION,
     )
     logger.debug(f"Create QC tables for {atlas_name}")
     obs_keys = get_viable_obs_qc(seurat, args)
     r_meta = robjects.r("obs <- function(seurat){ return(seurat@meta.data)}")
     r_metadata = r_meta(seurat)
     with (ro.default_converter + pandas2ri.converter).context():
         df_metadata = ro.conversion.get_conversion().rpy2py(r_metadata)
@@ -464,25 +464,25 @@
     :param atlas_info:
     :param args:
     :return:
     """
     atlas_name = atlas_info[checkatlas.ATLAS_NAME_KEY]
     csv_path = os.path.join(
         folders.get_folder(args.path, folders.CLUSTER),
-        atlas_name + checkatlas.METRIC_CLUSTER_EXTENSION,
+        atlas_name + checkatlas.TSV_EXTENSION,
     )
-    header = ["Sample", "obs"] + args.metric_cluster
+    header = ["Clust_Sample", "obs"] + args.metric_cluster
     df_cluster = pd.DataFrame(columns=header)
     obs_keys = get_viable_obs_annot(seurat, args)
     obsm_key_representation = "umap"
     if len(obs_keys) > 0:
         logger.debug(f"Calc clustering metrics for {atlas_name}")
         for obs_key in obs_keys:
             dict_line = {
-                "Sample": [atlas_name + "_" + obs_key],
+                "Clust_Sample": [atlas_name + "_" + obs_key],
                 "obs": [obs_key],
             }
             for metric in args.metric_cluster:
                 logger.debug(
                     f"Calc {metric} for {atlas_name} "
                     f"with obs {obs_key} and obsm {obsm_key_representation}"
                 )
@@ -509,27 +509,27 @@
     :param atlas_info:
     :param args:
     :return:
     """
     atlas_name = atlas_info[checkatlas.ATLAS_NAME_KEY]
     csv_path = os.path.join(
         folders.get_folder(args.path, folders.ANNOTATION),
-        atlas_name + checkatlas.METRIC_ANNOTATION_EXTENSION,
+        atlas_name + checkatlas.TSV_EXTENSION,
     )
-    header = ["Sample", "Reference", "obs"] + args.metric_annot
+    header = ["Annot_Sample", "Reference", "obs"] + args.metric_annot
     df_annot = pd.DataFrame(columns=header)
     obs_keys = get_viable_obs_annot(seurat, args)
     if len(obs_keys) > 1:
         logger.debug(f"Calc annotation metrics for {atlas_name}")
         if len(obs_keys) != 0:
             ref_obs = obs_keys[0]
             for i in range(1, len(obs_keys)):
                 obs_key = obs_keys[i]
                 dict_line = {
-                    "Sample": [atlas_name + "_" + obs_key],
+                    "Annot_Sample": [atlas_name + "_" + obs_key],
                     "Reference": [ref_obs],
                     "obs": [obs_key],
                 }
                 for metric in args.metric_annot:
                     logger.debug(
                         f"Calc {metric} for {atlas_name} "
                         f"with obs {obs_key} vs ref_obs {ref_obs}"
@@ -557,28 +557,28 @@
     :param atlas_info:
     :param args:
     :return:
     """
     atlas_name = atlas_info[checkatlas.ATLAS_NAME_KEY]
     csv_path = os.path.join(
         folders.get_folder(args.path, folders.DIMRED),
-        atlas_name + checkatlas.METRIC_DIMRED_EXTENSION,
+        atlas_name + checkatlas.TSV_EXTENSION,
     )
-    header = ["Sample", "obsm"] + args.metric_dimred
+    header = ["Dimred_Sample", "obsm"] + args.metric_dimred
     df_dimred = pd.DataFrame(columns=header)
     # r_reduction = robjects.r(
     #     "reduc <- function(seurat, obsm_key){"
     #     " return(Embeddings(object = seurat, reduction = obsm_key))}"
     # )
     obsm_keys = get_viable_obsm(seurat, args)
     if len(obsm_keys) > 0:
         logger.debug(f"Calc dim red metrics for {atlas_name}")
         for obsm_key in obsm_keys:
             dict_line = {
-                "Sample": [atlas_name + "_" + obsm_key],
+                "Dimred_Sample": [atlas_name + "_" + obsm_key],
                 "obsm": [obsm_key],
             }
             for metric in args.metric_dimred:
                 logger.debug(
                     f"Calc {metric} for {atlas_name} with obsm {obsm_key}"
                 )
                 # r_countmatrix = robjects.r(
```

### Comparing `checkatlas-0.3.0/checkatlas/utils/checkatlas_arguments.py` & `checkatlas-0.3.1/checkatlas/utils/checkatlas_arguments.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,16 +119,16 @@
         f"   Example: --metric_annot rand_index"
         f"   List of annotation metrics: {annot.__all__}",
     )
     metric_options.add_argument(
         "--metric_dimred",
         nargs="+",
         type=str,
-        # default=["kruskal_stress"],
-        default=[],
+        default=["kruskal_stress"],
+        # default=[],
         help="Specify the list of dimensionality reduction "
         "metrics to calculate.\n"
         "   Example: --metric_dimred kruskal_stress\n"
         f"   List of dim. red. metrics: {dimred.__all__}",
     )
     return parser
```

### Comparing `checkatlas-0.3.0/checkatlas/utils/files.py` & `checkatlas-0.3.1/checkatlas/utils/files.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.0/checkatlas/utils/folders.py` & `checkatlas-0.3.1/checkatlas/utils/folders.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,27 +11,28 @@
 CLUSTER = "cluster"
 ANNOTATION = "annotation"
 DIMRED = "dimred"
 SPECI = "specificity"
 TEMP = "temp"
 NEXTFLOW = "temp/nextflow"
 
+MULTIQC_FOLDER = "CheckAtlas_MultiQC"
+
 DICT_FOLDER = {
     SUMMARY: SUMMARY,
     ANNDATA: ANNDATA,
     QC: QC,
     QC_FIG: QC_FIG,
     UMAP: UMAP,
     TSNE: TSNE,
     CLUSTER: CLUSTER,
     ANNOTATION: ANNOTATION,
     DIMRED: DIMRED,
     SPECI: SPECI,
     TEMP: TEMP,
-    NEXTFLOW: NEXTFLOW,
 }
 
 logger = logging.getLogger("checkatlas")
 
 
 def get_workingdir(path: str) -> str:
     """Return the working_dir = path of search
@@ -78,7 +79,11 @@
         os.mkdir(global_path)
 
     for key_folder in DICT_FOLDER.keys():
         temp_path = os.path.join(global_path, key_folder)
         if not os.path.exists(temp_path):
             logger.debug(f"Create folder: {temp_path}")
             os.mkdir(temp_path)
+
+
+def get_multiqc_folder(path: str) -> str:
+    return os.path.join(path, MULTIQC_FOLDER)
```

### Comparing `checkatlas-0.3.0/checkatlas/utils/obsolete_arguments.py` & `checkatlas-0.3.1/checkatlas/utils/obsolete_arguments.py`

 * *Files identical despite different names*

### Comparing `checkatlas-0.3.0/pyproject.toml` & `checkatlas-0.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "checkatlas"
-version = "0.3.0"
+version = "0.3.1"
 description="One liner tool to check the quality of your single-cell atlases."
 authors = ["becavin-lab"]
 readme = "README.md"
 license = "BSD 3-Clause"
 packages = [{include = "checkatlas"}]
 include = ["checkatlas/checkatlas_workflow.nf"]
 exclude = ["tests/", ".github", "*dask-worker-space*"]
```

### Comparing `checkatlas-0.3.0/setup.py` & `checkatlas-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
  'types-pyyaml>=6.0.12.6,<7.0.0.0']
 
 entry_points = \
 {'console_scripts': ['checkatlas = checkatlas.__main__:main']}
 
 setup_kwargs = {
     'name': 'checkatlas',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'One liner tool to check the quality of your single-cell atlases.',
     'long_description': "# ![CheckAtlas](docs/images/checkatlas_logo.png) \n\n\n![PyPI](https://img.shields.io/pypi/v/checkatlas)\n![PyPI - Downloads](https://img.shields.io/pypi/dw/checkatlas)\n![PyPI - License](https://img.shields.io/pypi/l/checkatlas)\n![Conda](https://img.shields.io/conda/pn/bioconda/checkatlas)\n\n[![codecov](https://codecov.io/gh/becavin-lab/checkatlas/branch/main/graph/badge.svg?token=checkatlas_token_here)](https://codecov.io/gh/becavin-lab/checkatlas)\n[![CI](https://github.com/becavin-lab/checkatlas/actions/workflows/tests.yml/badge.svg)](https://github.com/becavin-lab/checkatlas/actions/workflows/tests.yml)\n[![Documentation Status](https://readthedocs.org/projects/checkatlas/badge/?version=latest)](https://checkatlas.readthedocs.io/en/latest/?badge=latest)\n[![Gitter](https://badges.gitter.im/checkatlas/checkatlas.svg)](https://app.gitter.im/#/room/!KpJcsVTOlGjwJgtLwF:gitter.im)\n\n![Static Badge](https://img.shields.io/badge/Packaging-Poetry-blue)\n![Static Badge](https://img.shields.io/badge/Docs-Mkdocs-red)\n![Static Badge](https://img.shields.io/badge/Linting-flake8%20black%20mypy-yellow)\n\nCheckAtlas is a one liner tool to check the quality of your single-cell atlases. For every atlas, it produces the\nquality control tables and figures which can be then processed by multiqc. CheckAtlas is able to load Scanpy, Seurat,\nand CellRanger files.\n\n\n## Summary\n\n### Parse Scanpy, Seurat and CellRanger objects\n\nThe checkatlas pipeline start with a fast crawl through your working directory. It detects Seurat (.rds), Scanpy (.h5ad) or cellranger (.h5) atlas files.\n\n\n### Create checkatlas summary files\n\nGo through all atlas files and produce summary information:\n\n- All basic QC (nRNA, nFeature, ratio_mito)\n- General information (nbcells, nbgenes, nblayers)\n- All elements in atlas files (obs, obsm, uns, var, varm)\n- Reductions (pca, umap, tsne)\n- All metrics (clustering, annotation, dimreduction, specificity)\n\n### Parse checkatlas files in MultiQC\n\n   Update MultiQC project to add checkatlas parsing. Dev project in: https://github.com/becavin-lab/MultiQC/tree/checkatlas\n\nhttps://checkatlas.readthedocs.io/en/latest/\n\n## Examples\n\n1. Evaluate and compare different atlases: https://github.com/becavin-lab/checkatlas/blob/3a4f88e94716c09a3b9c86010f570743a5855461/examples/Atlas_comparison.ipynb\n\nhttps://checkatlas.readthedocs.io/en/stable/CheckAtlas_example_1/CheckAtlas_example_1.html\n\n2. Evaluate different version of your atlas: https://github.com/becavin-lab/checkatlas/blob/3a4f88e94716c09a3b9c86010f570743a5855461/examples/Version_comparison.ipynb\n\nhttps://checkatlas.readthedocs.io/en/stable/CheckAtlas_example_2/CheckAtlas_example_2.html\n\n3. Explore Scanpy, Seurat and CellRanger objects in your folder: https://github.com/becavin-lab/checkatlas/blob/main/examples/AtlasType_comparison.ipynb\n\nhttps://checkatlas.readthedocs.io/en/stable/CheckAtlas_example_3/CheckAtlas_example_3.html\n\n## Installation\n\nCheckAtlas can be downloaded from PyPI. However, the project is in an early development phase. We strongly recommend to use the developmental version.\n\n### Install checkatlas development version\n\n```bash\ngit clone git@github.com:becavin-lab/checkatlas.git\npip install checkatlas/.\n```\n\nInstall MultiQC with checkatlas file management. This version of MultiQC is available at checkatlas branch of github.com:becavin-lab/MultiQC.\n\n```bash\ngit clone git@github.com:becavin-lab/MultiQC.git\ncd MultiQC/\ngit checkout checkatlas\npip install .\n```\n\n### Install it from PyPI\n\n```bash\npip install checkatlas\n```\n\n### Install Seurat\n\nTo be able to manage seurat file, rpy2 should have Seurat installed. The easiest way is to put all checkatlas requirements in a conda environment and add r-seurat.\n\n```bash\nconda create -n checkatlas python=3.9\npip install checkatlas\nconda install -c bioconda r-seurat\n```\n\nOr, open R in checkatlas environment (the one where you ran 'pip install') and install Seurat.\n\n```bash\n% R\n> install.packages('Seurat')\n> library(Seurat)\n```\n\n\n## Usage\n\nThe one liner way to run checkatlas is the following: \n\n```bash\n$ cd your_search_folder/\n$ python -m checkatlas .\n#or\n$ checkatlas .\n```\n\nOr run it inside your python workflow.\n\n```py\nfrom checkatlas import checkatlas\ncheckatlas.run(path, atlas_list, multithread, n_cpus)\n```\n\n\n## Development\n\nRead the [CONTRIBUTING.md](docs/contributing.md) file.\n\nProject developed thanks to the project template : (https://github.com/rochacbruno/python-project-template/)\n\n",
     'author': 'becavin-lab',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://checkatlas.readthedocs.io/',
```

### Comparing `checkatlas-0.3.0/PKG-INFO` & `checkatlas-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checkatlas
-Version: 0.3.0
+Version: 0.3.1
 Summary: One liner tool to check the quality of your single-cell atlases.
 Home-page: https://checkatlas.readthedocs.io/
 License: BSD 3-Clause
 Author: becavin-lab
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

