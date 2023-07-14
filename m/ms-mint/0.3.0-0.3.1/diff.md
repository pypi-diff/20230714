# Comparing `tmp/ms-mint-0.3.0.tar.gz` & `tmp/ms-mint-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms-mint-0.3.0.tar", last modified: Wed Jul 12 16:23:58 2023, max compression
+gzip compressed data, was "ms-mint-0.3.1.tar", last modified: Fri Jul 14 21:05:01 2023, max compression
```

## Comparing `ms-mint-0.3.0.tar` & `ms-mint-0.3.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:23:58.521733 ms-mint-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11301 2023-07-12 16:23:41.000000 ms-mint-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-12 16:23:41.000000 ms-mint-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-07-12 16:23:58.521733 ms-mint-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17628 2023-07-12 16:23:41.000000 ms-mint-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:23:58.525733 ms-mint-0.3.0/ms_mint/
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-07-12 16:23:41.000000 ms-mint-0.3.0/ms_mint/Chromatogram.py
--rw-r--r--   0 runner    (1001) docker     (123)    18153 2023-07-12 16:23:41.000000 ms-mint-0.3.0/ms_mint/Mint.py
--rw-r--r--   0 runner    (1001) docker     (123)    11735 2023-07-12 16:23:41.000000 ms-mint-0.3.0/ms_mint/MintPlotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-07-12 16:23:41.000000 ms-mint-0.3.0/ms_mint/TargetOptimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-12 16:23:41.000000 ms-mint-0.3.0/ms_mint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-12 16:23:58.525733 ms-mint-0.3.0/ms_mint/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13298 2023-07-12 16:23:41.000000 ms-mint-0.3.0/ms_mint/filelock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-12 16:23:41.000000 ms-mint-0.3.0/ms_mint/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    11415 2023-07-12 16:23:41.000000 ms-mint-0.3.0/ms_mint/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-07-12 16:23:41.000000 ms-mint-0.3.0/ms_mint/matplotlib_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-12 16:23:41.000000 ms-mint-0.3.0/ms_mint/notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     8231 2023-07-12 16:23:41.000000 ms-mint-0.3.0/ms_mint/pca.py
--rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-07-12 16:23:41.000000 ms-mint-0.3.0/ms_mint/plotly_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-07-12 16:23:41.000000 ms-mint-0.3.0/ms_mint/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-12 16:23:41.000000 ms-mint-0.3.0/ms_mint/standards.py
--rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-07-12 16:23:41.000000 ms-mint-0.3.0/ms_mint/targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-07-12 16:23:41.000000 ms-mint-0.3.0/ms_mint/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:23:58.521733 ms-mint-0.3.0/ms_mint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-07-12 16:23:58.000000 ms-mint-0.3.0/ms_mint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-12 16:23:58.000000 ms-mint-0.3.0/ms_mint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 16:23:58.000000 ms-mint-0.3.0/ms_mint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-12 16:23:58.000000 ms-mint-0.3.0/ms_mint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 16:23:58.000000 ms-mint-0.3.0/ms_mint.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:23:58.521733 ms-mint-0.3.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-12 16:23:41.000000 ms-mint-0.3.0/scripts/ms-mint-convert.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      450 2023-07-12 16:23:58.521733 ms-mint-0.3.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1348 2023-07-12 16:23:41.000000 ms-mint-0.3.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68780 2023-07-12 16:23:42.000000 ms-mint-0.3.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:05:01.618117 ms-mint-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11301 2023-07-14 21:04:45.000000 ms-mint-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-14 21:04:45.000000 ms-mint-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-07-14 21:05:01.618117 ms-mint-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17628 2023-07-14 21:04:45.000000 ms-mint-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:05:01.618117 ms-mint-0.3.1/ms_mint/
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-07-14 21:04:45.000000 ms-mint-0.3.1/ms_mint/Chromatogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20582 2023-07-14 21:04:45.000000 ms-mint-0.3.1/ms_mint/Mint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10662 2023-07-14 21:04:45.000000 ms-mint-0.3.1/ms_mint/MintPlotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-07-14 21:04:45.000000 ms-mint-0.3.1/ms_mint/TargetOptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-14 21:04:45.000000 ms-mint-0.3.1/ms_mint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-14 21:05:01.618117 ms-mint-0.3.1/ms_mint/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13298 2023-07-14 21:04:45.000000 ms-mint-0.3.1/ms_mint/filelock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-14 21:04:45.000000 ms-mint-0.3.1/ms_mint/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-07-14 21:04:45.000000 ms-mint-0.3.1/ms_mint/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-07-14 21:04:45.000000 ms-mint-0.3.1/ms_mint/matplotlib_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-14 21:04:45.000000 ms-mint-0.3.1/ms_mint/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-07-14 21:04:45.000000 ms-mint-0.3.1/ms_mint/pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-07-14 21:04:45.000000 ms-mint-0.3.1/ms_mint/plotly_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10713 2023-07-14 21:04:45.000000 ms-mint-0.3.1/ms_mint/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-14 21:04:45.000000 ms-mint-0.3.1/ms_mint/standards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-07-14 21:04:45.000000 ms-mint-0.3.1/ms_mint/targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-07-14 21:04:45.000000 ms-mint-0.3.1/ms_mint/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:05:01.618117 ms-mint-0.3.1/ms_mint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-07-14 21:05:01.000000 ms-mint-0.3.1/ms_mint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-14 21:05:01.000000 ms-mint-0.3.1/ms_mint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 21:05:01.000000 ms-mint-0.3.1/ms_mint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-14 21:05:01.000000 ms-mint-0.3.1/ms_mint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 21:05:01.000000 ms-mint-0.3.1/ms_mint.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:05:01.618117 ms-mint-0.3.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-14 21:04:45.000000 ms-mint-0.3.1/scripts/ms-mint-convert.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      450 2023-07-14 21:05:01.618117 ms-mint-0.3.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1348 2023-07-14 21:04:45.000000 ms-mint-0.3.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68780 2023-07-14 21:04:46.000000 ms-mint-0.3.1/versioneer.py
```

### Comparing `ms-mint-0.3.0/LICENSE` & `ms-mint-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ms-mint-0.3.0/PKG-INFO` & `ms-mint-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-mint
-Version: 0.3.0
+Version: 0.3.1
 Summary: Metabolomics Integrator (Mint)
 Home-page: https://github.com/LewisResearchGroup/ms-mint
 Author: Soren Wacker
 Author-email: swacker@ucalgary.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ms-mint-0.3.0/README.md` & `ms-mint-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ms-mint-0.3.0/ms_mint/Chromatogram.py` & `ms-mint-0.3.1/ms_mint/Chromatogram.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.3.0/ms_mint/Mint.py` & `ms-mint-0.3.1/ms_mint/Mint.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,26 +6,29 @@
 import time
 import logging
 
 from pathlib import Path as P
 from multiprocessing import Pool, Manager, cpu_count
 from glob import glob
 
+from sklearn.preprocessing import StandardScaler, RobustScaler
+
 from .standards import MINT_RESULTS_COLUMNS, TARGETS_COLUMNS, DEPRECATED_LABELS
 from .processing import process_ms1_files_in_parallel, extract_chromatogram_from_ms1
 from .io import export_to_excel, ms_file_to_df
 from .TargetOptimizer import TargetOptimizer
 from .targets import read_targets, check_targets, standardize_targets
 from .tools import (
     is_ms_file,
     get_ms_files_from_results,
     get_targets_from_results,
     scale_dataframe,
     init_metadata,
-    fn_to_label
+    fn_to_label,
+    log2p1
 )
 from .pca import PrincipalComponentsAnalyser
 from .MintPlotter import MintPlotter
 from .Chromatogram import Chromatogram
 
 import ms_mint
 
@@ -55,15 +58,16 @@
         verbose: bool = False,
         progress_callback: Callable = None,
         time_unit: str = "s",
         wdir: str = None
     ):
         self.verbose = verbose
         self._version = ms_mint.__version__
-        print("Mint version:", self.version, "\n")
+        if verbose: 
+            print("Mint version:", self.version, "\n")
         self.progress_callback = progress_callback
         self.reset()
         self.plot = MintPlotter(mint=self)
         self.opt = TargetOptimizer(mint=self)
         self.pca = PrincipalComponentsAnalyser(self)
         self.tqdm = tqdm
 
@@ -377,48 +381,90 @@
         """
         return self._results
 
     @results.setter
     def results(self, df):
         self._results = df
 
-    def crosstab(self, values: str = "peak_max", index: str = None, column: str = None, aggfunc: str = 'mean', apply: Callable = None, scaler: Callable = None):
+    def crosstab(self, var_name: str = None, index: str = None, column: str = None, aggfunc: str = 'mean', 
+                 apply: Callable = None, scaler: Callable = None, groupby: str = None):
         """
         Create condensed representation of the results.
         More specifically, a cross-table with filenames as index and target labels.
         The values in the cells are determined by *col_name*.
 
-        :param col_name: Name of the column from *mint.results* table that is used for the cell values.
-        :type col_name: str
+        :param var_name: Name of the column from *mint.results* table that is used for the cell values. If None, defaults to 'peak_area_top3'.
+        :type var_name: str, optional
+
+        :param index: Name of the column to be used as index in the resulting cross-tabulation. If None, defaults to 'ms_file_label'.
+        :type index: str, optional
+
+        :param column: Name of the column to be used as columns in the resulting cross-tabulation. If None, defaults to 'peak_label'.
+        :type column: str, optional
+
+        :param aggfunc: Aggregation function to be used for aggregating values. Defaults to 'mean'.
+        :type aggfunc: str, optional
+
+        :param apply: Function to be applied to the resulting cross-tabulation. If None, no function is applied.
+        :type apply: Callable, optional
 
-        cells of the returned table.
+        :param scaler: Function to scale the data in the resulting cross-tabulation. If None, no scaling is performed.
+        :type scaler: Callable, optional
+
+        :param groupby: Name of the column to group data before scaling. If None, scaling is applied to the whole data, not group-wise.
+        :type groupby: str, optional
+
+        :return: DataFrame representing the cross-tabulation.
+        :rtype: pandas.DataFrame
         """
-        
         df_meta = pd.merge(self.meta, self.results, left_index=True, right_on='ms_file_label')
-
+        # Remove None if in index
+        if isinstance(index, list):
+            if None in index:
+                index.remove(None)
+        if isinstance(groupby, str):
+            groupby = [groupby]
+            
         if index is None:
             index = 'ms_file_label'
         if column is None:
             column = 'peak_label'
-        if values is None:
-            values = 'peak_area_top3'
+        if var_name is None:
+            var_name = 'peak_area_top3'
+        if apply:
+            if apply == 'log2p1':
+                apply = log2p1
+            if apply == 'logp1':
+                apply = np.log1p
+            df_meta[var_name] = df_meta[var_name].apply(apply)
+        if isinstance(scaler, str):
+            scaler_dict = {'standard': StandardScaler(),
+                           'robust': RobustScaler()}
 
-        df = pd.crosstab(
-            df_meta[index],
-            df_meta[column],
-            df_meta[values],
-            aggfunc=aggfunc,
-        ).astype(np.float64)
+            if scaler not in scaler_dict:
+                raise ValueError(f"Unsupported scaler: {scaler}")
 
-        if apply:
-            df = df.apply(apply)
+            scaler = scaler_dict[scaler]
+            
         if scaler:
-            df = scale_dataframe(df, scaler=scaler)
+            if groupby:          
+                groupby_cols = groupby + [column]
+                df_meta[var_name] = df_meta.groupby(groupby_cols)[var_name].transform(lambda x: self._scale_group(x, scaler))
+            else:
+                df_meta[var_name] = df_meta.groupby(column)[var_name].transform(lambda x: self._scale_group(x, scaler))
+                
+        df = pd.pivot_table(
+            df_meta,
+            index=index,
+            columns=column,
+            values=var_name,
+            aggfunc=aggfunc,
+        ).astype(np.float64)
         return df
-
+    
     @property
     def progress(self):
         """
         Shows the current progress.
 
         :getter: Returns the current progress value.
         :setter: Set the progress to a value between 0 and 100 and calls the progress callback function.
@@ -560,7 +606,13 @@
         if fn is None:
             fn = self.wdir/METADATA_DEFAUT_FN
         if str(fn).endswith('.csv'):
             self.meta.to_csv(fn, na_filter=False)
         elif str(fn).endswith('.parquet'):
             self.meta.to_parquet(fn)
         return self
+
+    def _scale_group(self, group, scaler):
+        """
+        Helper function to scale groups individually.
+        """
+        return scaler.fit_transform(group.to_numpy().reshape(-1, 1)).flatten()
```

### Comparing `ms-mint-0.3.0/ms_mint/MintPlotter.py` & `ms-mint-0.3.1/ms_mint/MintPlotter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 import numpy as np
 import seaborn as sns
+import warnings
 
-from warnings import simplefilter
 from scipy.cluster.hierarchy import ClusterWarning
 
 from pathlib import Path as P
+
+import matplotlib
 from matplotlib import pyplot as plt
 
+from typing import Optional, List, Tuple
+
 from .plotly_tools import plotly_heatmap, plotly_peak_shapes
 from .matplotlib_tools import (
     plot_peak_shapes,
     hierarchical_clustering,
     plot_metabolomics_hist2d,
 )
 
+import pandas as pd
 import plotly.express as px
 
 from .tools import scale_dataframe, mz_mean_width_to_min_max
 from .io import ms_file_to_df
 
 
 class MintPlotter:
@@ -32,124 +37,90 @@
         """
         Plot generator for mint.results.
 
         :param mint: Mint instance
         :type mint: ms_mint.Mint.Mint
         """
         self.mint = mint
-
+        
+        
     def hierarchical_clustering(
         self,
-        data=None,
-        peak_labels=None,
-        ms_files=None,
-        title=None,
-        figsize=(8, 8),
-        targets_var="peak_max",
-        vmin=-3,
-        vmax=3,
-        xmaxticks=None,
-        ymaxticks=None,
-        transform_func="log2p1",
-        scaler_ms_file=None,
-        scaler_peak_label="standard",
-        metric="cosine",
-        transform_filenames_func="basename",
-        transposed=False,
+        data: Optional[pd.DataFrame] = None,
+        peak_labels: Optional[List[str]] = None,
+        ms_files: Optional[List[str]] = None,
+        title: Optional[str] = None,
+        figsize: Tuple[int, int] = (8, 8),
+        targets_var: Optional[str] = None,
+        var_name: str = "peak_max",
+        vmin: int = -3,
+        vmax: int = 3,
+        xmaxticks: Optional[int] = None,
+        ymaxticks: Optional[int] = None,
+        apply: str = "log2p1",
+        metric: str = "cosine",
+        scaler: str = "standard",
+        groupby: Optional[str] = None,
+        transposed: bool = False,
         **kwargs,
-    ):
+    ) -> matplotlib.figure.Figure:
         """
         Performs a cluster analysis and plots a heatmap. If no data is provided,
-        data is taken form self.mint.crosstab(targets_var).
+        data is taken from self.mint.crosstab(var_name).
         The clustered non-transformed non-scaled data is stored in `self.mint.clustered`.
 
-        :param transform_func: default 'log2p1', values: [None, 'log1p', 'log2p1', 'log10p1']
-            - None: no transformation
-            - log1p: tranform data with lambda x: np.log1p(x)
-            - log2p1: transform data with lambda x: log2(x+1)
-            - log10p1: transform data with lambda x: log10(x+1)
-
-        :param scaler_ms_file: default None, values: [None, 'standard', 'robust']
-            - scaler used to scale along ms_file axis
-            - if None no scaling is applied
-            - if 'standard' use scikit learn StandardScaler()
-            - if 'robust' use scikit learn RobustScaler()
-
-        :param scaler_peak_label: default 'standard'
-            - like scaler_ms_file, but scaling along peak_label axis
-
-        :param metric: default 'cosine', can be string or a list of two values:
-            if two values are provided e.g. ('cosine', 'euclidean') the first
-            will be used to cluster the x-axis and the second for the y-axis.
-
-            'braycurtis', 'canberra', 'chebyshev', 'cityblock', 'correlation', 'cosine',
-            'dice', 'euclidean', 'hamming', 'jaccard', 'jensenshannon', 'kulsinski', 'mahalanobis',
-            'matching', 'minkowski', 'rogerstanimoto', 'russellrao', 'seuclidean',
-            'sokalmichener', 'sokalsneath', 'sqeuclidean', 'yule'.
-            More information:
-            https://docs.scipy.org/doc/scipy/reference/generated/scipy.spatial.distance.pdist.html
+        :param data: DataFrame with data to be used for clustering. If None, crosstab of mint instance is used.
+        :type data: pandas.DataFrame, optional
 
-        :param transpose: bool, default False
-            - True: transpose the figure
-        """
-        if len(self.mint.results) == 0:
-            return None
+        :param var_name: Name of the column from data to be used for cell values in the heatmap. Defaults to "peak_max".
+        :type var_name: str
 
-        simplefilter("ignore", ClusterWarning)
-        if data is None:
-            data = self.mint.crosstab(targets_var).copy()
+        :param apply: Transformation to be applied on the data. Can be "log1p", "log2p1", "log10p1" or None. Defaults to "log2p1".
+        :type apply: str, optional
+
+        :param scaler: Method to scale data along both axes. Can be "standard", "robust" or None. Defaults to "standard".
+        :type scaler: str, optional
 
-        if peak_labels is not None:
-            data = data[peak_labels]
+        :param groupby: Name of the column to group data before scaling. If None, scaling is applied to the whole data, not group-wise.
+        :type groupby: str, optional
 
-        if ms_files is not None:
-            data = data.loc[ms_files]
+        :param metric: The distance metric to use for the tree. Can be any metric supported by scipy.spatial.distance.pdist.
+        :type metric: str, optional
 
-        tmp_data = data.copy()
-
-        if transform_func == "log1p":
-            transform_func = np.log1p
-        if transform_func == "log2p1":
-            transform_func = lambda x: np.log2(x + 1)
-        if transform_func == "log10p1":
-            transform_func = lambda x: np.log10(x + 1)
-        if transform_func is not None:
-            tmp_data = tmp_data.apply(transform_func)
-
-        if transform_filenames_func == "basename":
-            transform_filenames_func = lambda x: P(x).with_suffix("").name
-        if transform_filenames_func is not None:
-            tmp_data.index = [transform_filenames_func(i) for i in tmp_data.index]
-
-        # Scale along ms-files
-        if scaler_ms_file is not None:
-            tmp_data = scale_dataframe(tmp_data.T, scaler_ms_file).T
-
-        # Scale along peak_labels
-        if scaler_peak_label is not None:
-            tmp_data = scale_dataframe(tmp_data, scaler_peak_label)
+        :param transposed: Whether to transpose the figure or not. Defaults to False.
+        :type transposed: bool, optional
+
+        :return: Matplotlib figure representing the clustered heatmap.
+        :rtype: matplotlib.figure.Figure
+        """
+
+        if targets_var is not None:
+            warnings.warn("targets_var is depricated use var_name instead", DeprecationWarning)
+            var_name = targets_var
+
+        warnings.simplefilter("ignore", ClusterWarning)
+        if data is None:
+            data = self.mint.crosstab(var_name=var_name, apply=apply, scaler=scaler, groupby=groupby)
 
         if transposed:
-            tmp_data = tmp_data.T
+            data = data.T
 
         _, fig, ndx_x, ndx_y = hierarchical_clustering(
-            tmp_data,
+            data,
             vmin=vmin,
             vmax=vmax,
             figsize=figsize,
             xmaxticks=xmaxticks,
             ymaxticks=ymaxticks,
             metric=metric,
             **kwargs,
         )
 
-        if not transposed:
-            self.mint.clustered = data.iloc[ndx_x, ndx_y]
-        else:
-            self.mint.clustered = data.iloc[ndx_y, ndx_x]
+        self.mint.clustered = data.iloc[ndx_x, ndx_y]
+        
         return fig
     
 
     def peak_shapes(self, fns=None, peak_labels=None, interactive=False, **kwargs):
         """Plot peak shapes.
 
         :return: Figure with peak shapes.
```

### Comparing `ms-mint-0.3.0/ms_mint/TargetOptimizer.py` & `ms-mint-0.3.1/ms_mint/TargetOptimizer.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.3.0/ms_mint/filelock.py` & `ms-mint-0.3.1/ms_mint/filelock.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.3.0/ms_mint/filters.py` & `ms-mint-0.3.1/ms_mint/filters.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.3.0/ms_mint/io.py` & `ms-mint-0.3.1/ms_mint/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,26 +60,32 @@
         elif fn.lower().endswith(".mzmlb"):
             df = mzmlb_to_df__pyteomics(fn, read_only=read_only)
         else:
             logging.error(f"Cannot read file {fn} of type {type(fn)}")
     except IndexError as e:
         logging.warning(f"{e}: {fn}")
         return None
-    if not read_only:
+    
+    if read_only:
+        return df
+    else:
         # Compatibility with old schema
         df = df.rename(
             columns={
                 "retentionTime": "scan_time",
                 "intensity array": "intensity",
                 "m/z array": "mz",
             }
         )
+        if 'scan_id' not in df.columns:
+            df['scan_id'] = 0
+        if 'ms_level' not in df.columns:
+            df['ms_level'] = 1
         # Set datatypes
         set_dtypes(df)
-    print(df.columns)
     return df
 
 
 def mzxml_to_df(
     fn: Union[str, pathlib.Path],
     read_only: bool = False,
     time_unit_in_file: str = "min",
```

### Comparing `ms-mint-0.3.0/ms_mint/matplotlib_tools.py` & `ms-mint-0.3.1/ms_mint/matplotlib_tools.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.3.0/ms_mint/notebook.py` & `ms-mint-0.3.1/ms_mint/notebook.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.3.0/ms_mint/pca.py` & `ms-mint-0.3.1/ms_mint/pca.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 import seaborn as sns
+import warnings
+
 import plotly.figure_factory as ff
 from plotly import express as px
 
 from sklearn.decomposition import PCA
 from .tools import scale_dataframe
 
 
@@ -21,41 +23,43 @@
         :param mint: Mint instance, defaults to None
         :type mint: ms_mint.Mint.Mint, optional
         """
         self.mint = mint
         self.results = None
         self.plot = PCA_Plotter(self)
 
-    def run(self, n_components=3, on="peak_max", fillna="median", scaler="standard"):
+    def run(self, n_components=3, on=None, var_name="peak_max", fillna="median", apply=None, groupby=None, scaler="standard"):
         """
         Run Principal Component Analysis on current results. Results are stored in
         self.decomposition_results.
 
         :param on: Column name to use for pca, defaults to "peak_max"
         :type on: str, optional
         :param n_components: Number of PCA components to return, defaults to 3
         :type n_components: int, optional
         :param fillna: Method to fill missing values, defaults to "median"
         :type fillna: str, optional
         :param scaler: Method to scale the columns, defaults to "standard"
         :type scaler: str, optional
         """
-
-        df = self.mint.crosstab(on).fillna(fillna)
+        
+        if on is not None:
+            warnings.warn("on is depricated use var_name instead", DeprecationWarning)            
+            var_name = on            
+        
+        df = self.mint.crosstab(var_name=var_name, apply=apply, scaler=scaler, groupby=groupby)
 
         if fillna == "median":
             fillna = df.median()
         elif fillna == "mean":
             fillna = df.mean()
         elif fillna == "zero":
             fillna = 0
 
         df = df.fillna(fillna)
-        if scaler is not None:
-            df = scale_dataframe(df, scaler)
 
         min_dim = min(df.shape)
         n_components = min(n_components, min_dim)
         pca = PCA(n_components)
         X_projected = pca.fit_transform(df)
         # Convert to dataframe
         df_projected = pd.DataFrame(X_projected, index=df.index.get_level_values(0))
```

### Comparing `ms-mint-0.3.0/ms_mint/plotly_tools.py` & `ms-mint-0.3.1/ms_mint/plotly_tools.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.3.0/ms_mint/processing.py` & `ms-mint-0.3.1/ms_mint/processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     """
     df = ms_file_to_df(filename)
     results = process_ms1(df, targets)
     results["total_intensity"] = df["intensity"].sum()
     results["ms_file"] = filename
     results["ms_file_label"] = P(filename).with_suffix('').name
     results["ms_file_size_MB"] = os.path.getsize(filename) / 1024 / 1024
-    results["peak_score"] = score_peaks(results)
+    results["peak_score"] = 0 #  score_peaks(results)
     return results[MINT_RESULTS_COLUMNS]
 
 
 def process_ms1(df, targets):
     """
     Process MS-1 data with a target list.
```

### Comparing `ms-mint-0.3.0/ms_mint/standards.py` & `ms-mint-0.3.1/ms_mint/standards.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.3.0/ms_mint/targets.py` & `ms-mint-0.3.1/ms_mint/targets.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.3.0/ms_mint/tools.py` & `ms-mint-0.3.1/ms_mint/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 from scipy.signal import find_peaks, peak_widths
 
 from .standards import M_PROTON, TARGETS_COLUMNS
 from .filelock import FileLock
 from .matplotlib_tools import plot_peaks
 
 
+def log2p1(x):
+    return np.log2(x+1)
+
+
 def lock(fn):
     """
     File lock to ensure safe writing to file.
 
     :param fn: Filename to lock.
     :type fn: str or PosixPath
     :return: File lock object.
```

### Comparing `ms-mint-0.3.0/ms_mint.egg-info/PKG-INFO` & `ms-mint-0.3.1/ms_mint.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-mint
-Version: 0.3.0
+Version: 0.3.1
 Summary: Metabolomics Integrator (Mint)
 Home-page: https://github.com/LewisResearchGroup/ms-mint
 Author: Soren Wacker
 Author-email: swacker@ucalgary.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ms-mint-0.3.0/ms_mint.egg-info/SOURCES.txt` & `ms-mint-0.3.1/ms_mint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ms-mint-0.3.0/scripts/ms-mint-convert.py` & `ms-mint-0.3.1/scripts/ms-mint-convert.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.3.0/setup.py` & `ms-mint-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.3.0/versioneer.py` & `ms-mint-0.3.1/versioneer.py`

 * *Files identical despite different names*

