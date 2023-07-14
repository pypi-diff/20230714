# Comparing `tmp/ms-mint-app-0.3.0.tar.gz` & `tmp/ms-mint-app-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms-mint-app-0.3.0.tar", last modified: Wed Jul 12 16:39:53 2023, max compression
+gzip compressed data, was "ms-mint-app-0.3.1.tar", last modified: Fri Jul 14 21:12:04 2023, max compression
```

## Comparing `ms-mint-app-0.3.0.tar` & `ms-mint-app-0.3.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:53.311085 ms-mint-app-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-07-12 16:39:53.311085 ms-mint-app-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:53.311085 ms-mint-app-0.3.0/ms_mint_app/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-12 16:39:53.311085 ms-mint-app-0.3.0/ms_mint_app/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    13453 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/filelock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/plugin_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/plugin_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:53.299085 ms-mint-app-0.3.0/ms_mint_app/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/plugins/add_metabolites.py
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/plugins/analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:53.299085 ms-mint-app-0.3.0/ms_mint_app/plugins/analysis_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/plugins/analysis_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/plugins/analysis_tools/distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/plugins/analysis_tools/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/plugins/analysis_tools/hierachical_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/plugins/analysis_tools/pca.py
--rw-r--r--   0 runner    (1001) docker     (123)    12468 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/plugins/analysis_tools/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/plugins/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/plugins/ms_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/plugins/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/plugins/quality_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    20693 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/plugins/target_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/plugins/targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/plugins/workspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:53.307085 ms-mint-app-0.3.0/ms_mint_app/static/
--rw-r--r--   0 runner    (1001) docker     (123)  9253590 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/static/ChEBI-Chem.parquet
--rw-r--r--   0 runner    (1001) docker     (123)  1058677 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/static/ChEBI-Groups.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/static/Standard_Peaklist.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22254 2023-07-12 16:39:38.000000 ms-mint-app-0.3.0/ms_mint_app/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:53.295085 ms-mint-app-0.3.0/ms_mint_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-07-12 16:39:53.000000 ms-mint-app-0.3.0/ms_mint_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-12 16:39:53.000000 ms-mint-app-0.3.0/ms_mint_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 16:39:53.000000 ms-mint-app-0.3.0/ms_mint_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-12 16:39:53.000000 ms-mint-app-0.3.0/ms_mint_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-12 16:39:53.000000 ms-mint-app-0.3.0/ms_mint_app.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:53.307085 ms-mint-app-0.3.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-07-12 16:39:38.000000 ms-mint-app-0.3.0/scripts/Mint.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-12 16:39:53.311085 ms-mint-app-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-12 16:39:38.000000 ms-mint-app-0.3.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68751 2023-07-12 16:39:38.000000 ms-mint-app-0.3.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:12:04.169942 ms-mint-app-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-07-14 21:12:04.169942 ms-mint-app-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:12:04.169942 ms-mint-app-0.3.1/ms_mint_app/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-14 21:12:04.169942 ms-mint-app-0.3.1/ms_mint_app/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13453 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/filelock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/plugin_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/plugin_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:12:04.157940 ms-mint-app-0.3.1/ms_mint_app/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/plugins/add_metabolites.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/plugins/analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:12:04.157940 ms-mint-app-0.3.1/ms_mint_app/plugins/analysis_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/plugins/analysis_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/plugins/analysis_tools/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/plugins/analysis_tools/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/plugins/analysis_tools/hierachical_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/plugins/analysis_tools/pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13504 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/plugins/analysis_tools/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/plugins/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/plugins/ms_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/plugins/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/plugins/quality_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20693 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/plugins/target_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/plugins/targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/plugins/workspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:12:04.169942 ms-mint-app-0.3.1/ms_mint_app/static/
+-rw-r--r--   0 runner    (1001) docker     (123)  9253590 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/static/ChEBI-Chem.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)  1058677 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/static/ChEBI-Groups.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/static/Standard_Peaklist.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23723 2023-07-14 21:11:53.000000 ms-mint-app-0.3.1/ms_mint_app/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:12:04.157940 ms-mint-app-0.3.1/ms_mint_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-07-14 21:12:04.000000 ms-mint-app-0.3.1/ms_mint_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-14 21:12:04.000000 ms-mint-app-0.3.1/ms_mint_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 21:12:04.000000 ms-mint-app-0.3.1/ms_mint_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-14 21:12:04.000000 ms-mint-app-0.3.1/ms_mint_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 21:12:04.000000 ms-mint-app-0.3.1/ms_mint_app.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:12:04.169942 ms-mint-app-0.3.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-07-14 21:11:53.000000 ms-mint-app-0.3.1/scripts/Mint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-14 21:12:04.169942 ms-mint-app-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-14 21:11:53.000000 ms-mint-app-0.3.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68751 2023-07-14 21:11:53.000000 ms-mint-app-0.3.1/versioneer.py
```

### Comparing `ms-mint-app-0.3.0/LICENSE` & `ms-mint-app-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.0/PKG-INFO` & `ms-mint-app-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-mint-app
-Version: 0.3.0
+Version: 0.3.1
 Summary: Metabolomics Integrator (Mint)
 Home-page: https://github.com/LewisResearchGroup/ms-mint-app
 Author: Soren Wacker
 Author-email: swacker@ucalgary.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ms-mint-app-0.3.0/README.md` & `ms-mint-app-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.0/ms_mint_app/app.py` & `ms-mint-app-0.3.1/ms_mint_app/app.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.0/ms_mint_app/auth.py` & `ms-mint-app-0.3.1/ms_mint_app/auth.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.0/ms_mint_app/database.py` & `ms-mint-app-0.3.1/ms_mint_app/database.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.0/ms_mint_app/filelock.py` & `ms-mint-app-0.3.1/ms_mint_app/filelock.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.0/ms_mint_app/messages.py` & `ms-mint-app-0.3.1/ms_mint_app/messages.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.0/ms_mint_app/plugin_manager.py` & `ms-mint-app-0.3.1/ms_mint_app/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.0/ms_mint_app/plugins/add_metabolites.py` & `ms-mint-app-0.3.1/ms_mint_app/plugins/add_metabolites.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.0/ms_mint_app/plugins/analysis.py` & `ms-mint-app-0.3.1/ms_mint_app/plugins/analysis.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from dash import html, dcc
 from dash.dependencies import Input, Output, State
 from dash.exceptions import PreventUpdate
 import dash_bootstrap_components as dbc
 
+from ms_mint.standards import RESULTS_COLUMNS
+
 from .analysis_tools import heatmap
 from .analysis_tools import pca
 from .analysis_tools import distributions
 from .analysis_tools import hierachical_clustering
 from .analysis_tools import plotting
 
 
@@ -31,27 +33,32 @@
     
 
 
 _modules = [heatmap, distributions, pca, hierachical_clustering, plotting]
 
 modules = {module._label: module for module in _modules}
 
-groupby_options = [
-    {"label": "plate", "value": "plate"},
+colorby_options = [
     {"label": "label", "value": "label"},
+    {"label": "plate", "value": "plate"},
     {"label": "sample_type", "value": "sample_type"},
-    {"label": "color", "value": "color"},
 ]
 
-ana_normalization_cols = [
-    {"label": "plate", "value": "plate"},
-    {"label": "peak_label", "value": "peak_label"},
-    {"label": "ms_file_id", "value": "ms_file_id"},
+apply_options = [{"label": "log10(x+1)", "value": "log1p"}, 
+                 {"label": "log2(x+1)" , "value": "log2p1"}]
+
+var_name_options = T.list_to_options(RESULTS_COLUMNS)
+
+scaler_options = [
+    {"value": "standard", "label": "Standard Scaling (z-scores)"},
+    #{"value": "minmax", "label": "MinMax Scaling"},
+    {"value": "robust", "label": "Robust Scaling"}
 ]
 
+
 _layout = html.Div(
     [
         dcc.Tabs(
             id="ana-secondary-tab",
             value=_modules[0]._label,
             vertical=False,
             children=[
@@ -78,35 +85,54 @@
                 ),
                 dcc.Dropdown(
                     id="ana-peak-labels-exclude",
                     options=[],
                     placeholder="Exclude peak_labels",
                     multi=True,
                 ),
+                dcc.Dropdown(
+                    id="ana-var-name",
+                    options=var_name_options,
+                    value='peak_max',
+                    placeholder="Variable to plot",
+                )
             ]),
             dbc.Col([
                 dcc.Dropdown(
                     id="ana-ms-order", options=[], placeholder="MS-file sorting", multi=True
                 ),
                 dcc.Dropdown(
-                    id="ana-groupby",
-                    options=groupby_options,
+                    id="ana-colorby",
+                    options=colorby_options,
                     value=None,
-                    placeholder="Group by column",
+                    placeholder="Color by",
                 ),
                 dcc.Dropdown(
-                    id="ana-normalization-cols",
-                    options=ana_normalization_cols,
+                    id="ana-apply",
+                    options=apply_options,
+                    value=None,
+                    placeholder="Transformation",
+                    multi=False,
+                ),  
+                dcc.Dropdown(
+                    id="ana-groupby",
+                    options=[],
                     value=None,
                     placeholder="Normalize by",
                     multi=True,
                 ),
+                dcc.Dropdown(
+                    id="ana-scaler",
+                    options=scaler_options,
+                    value=[],
+                    placeholder="Scaler",
+                    multi=False,
+                ),                                 
             ]),
         ]),
-
         html.Div(id="ana-secondary-tab-content"),
     ]
 )
 
 
 _label = "Analysis"
 
@@ -161,16 +187,18 @@
     )
     def ms_order_options(tab, wdir):
         cols = T.get_metadata(wdir).dropna(how="all", axis=1).columns.to_list()
         if "index" in cols:
             cols.remove("index")
         if "use_for_optimization" in cols:
             cols.remove("use_for_optimization")
-        options = [{"value": i, "label": i} for i in cols]
-        return options, options
+        options_without_peak_label = [{"value": i, "label": i} for i in cols]
+        cols.append('peak_label')
+        options_with_peak_label = [{"value": i, "label": i} for i in cols]
+        return options_without_peak_label, options_with_peak_label
 
     @app.callback(
         Output("ana-peak-labels-include", "options"),
         Output("ana-peak-labels-exclude", "options"),
         Input("tab", "value"),
         State("wdir", "children"),
     )
```

### Comparing `ms-mint-app-0.3.0/ms_mint_app/plugins/analysis_tools/distributions.py` & `ms-mint-app-0.3.1/ms_mint_app/plugins/analysis_tools/distributions.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,40 +7,44 @@
 import seaborn as sns
 
 from dash import html, dcc
 import dash_bootstrap_components as dbc
 from dash.exceptions import PreventUpdate
 from dash.dependencies import Input, Output, State
 
+from ms_mint.Mint import Mint
+from ms_mint.standards import MINT_RESULTS_COLUMNS
 from ... import tools as T
 
+
 graph_options = [
     {"label": "Histograms", "value": "hist"},
     {"label": "Boxplots", "value": "boxplot"},
     {"label": "Probability Density", "value": "density"},
 ]
 
 _label = "Distributions"
 
 _layout = html.Div(
     [
-        html.H3("Quality Control"),
+        html.H3("Distributions"),
         dbc.Button("Update", id="dist-update"),
         dcc.Dropdown(
             id="dist-graphs",
             options=graph_options,
             value=["hist"],
             multi=True,
             placeholder="Kinds of graphs",
         ),
         dcc.Checklist(
             id="dist-select",
             options=[{"label": "Dense", "value": "Dense"}],
             value=["Dense"],
         ),
+        html.Center(html.H4("", id='description'), style={'marginTop': "200px"}),
         html.Div(id="dist-figures", style={"float": "center"}),
     ]
 )
 
 
 layout_no_data = html.Div(
     [
@@ -58,28 +62,37 @@
 def layout():
     return _layout
 
 
 def callbacks(app, fsc, cache):
     @app.callback(
         Output("dist-figures", "children"),
+        Output("description", "children"),
         Input("dist-update", "n_clicks"),
         State("tab", "value"),
+        State("ana-var-name", "value"),
+        State("ana-colorby", "value"),
         State("ana-groupby", "value"),
+        State("ana-scaler", "value"),
+        State("ana-apply", "value"),
         State("dist-graphs", "value"),
         State("dist-select", "value"),
         State("ana-file-types", "value"),
         State("ana-peak-labels-include", "value"),
         State("ana-peak-labels-exclude", "value"),
         State("wdir", "children"),
     )
     def qc_figures(
         n_clicks,
         tab,
+        var_name,
+        colorby,
         groupby,
+        scaler,
+        apply,
         kinds,
         options,
         file_types,
         include_labels,
         exclude_labels,
         wdir,
     ):
@@ -90,111 +103,89 @@
         df = T.get_complete_results(
             wdir,
             include_labels=include_labels,
             exclude_labels=exclude_labels,
             file_types=file_types,
         )
 
-        if len(df) == 0:
-            return "No results yet. First run MINT."
-
-        if "boxplot" in kinds:
-            if groupby is None or len(groupby) == 0:
-                return dbc.Alert(
-                    'For boxplots a "Group-by" column has to be set', color="info"
-                )
-            if len(df[groupby].drop_duplicates()) <= 1:
-                return dbc.Alert(
-                    'For boxplots at least two groups have to be defined in selected "Group-by" column in metadata sheet.',
-                    color="info",
-                )
-
-        sns.set_context("paper")
+        mint = Mint()
+        mint.results = df[MINT_RESULTS_COLUMNS]
+        mint.load_metadata(T.get_metadata_fn(wdir))
 
-        sort_by_col = "plate"
-        quant_col = "log(peak_max+1)"
+        df = mint.crosstab(var_name=var_name, index=['ms_file_label', colorby], 
+                           groupby=groupby, apply=apply, scaler=scaler).stack().to_frame().reset_index().rename(columns={0: var_name})
 
-        if sort_by_col is not None:
-            df = df.sort_values(["peak_label", sort_by_col])
-
-        if options is None:
-            options = []
+        desc = T.describe_transformation(var_name=var_name, apply=apply, groupby=groupby, scaler=scaler)
+        desc_short = desc.split(" (")[0]
 
         figures = []
         n_total = len(df.peak_label.drop_duplicates())
         for i, (peak_label, grp) in tqdm(
             enumerate(df.groupby("peak_label")), total=n_total
         ):
 
             if not "Dense" in options:
                 figures.append(
                     dcc.Markdown(f"#### `{peak_label}`", style={"float": "center"})
                 )
             fsc.set("progress", int(100 * (i + 1) / n_total))
 
-            # Sorting to ensure similar legends
-            if sort_by_col is not None:
-                grp = grp.sort_values(sort_by_col).reset_index(drop=True)
-
-            # if len(grp) < 1:
-            #    continue
             if "hist" in kinds:
-                # define your figure and axis
                 fig, ax = plt.subplots(figsize=(3, 3))
                 
-                sns.histplot(data=grp, x=quant_col, hue=groupby, ax=ax)
+                sns.histplot(data=grp, x=var_name, hue=colorby, ax=ax)
+                ax.set_xlabel(desc_short)
                 ax.set_title(peak_label)
-                fig_label = f"by-{groupby}__{quant_col}__{peak_label}"
+                fig_label = f"by-{colorby}__{var_name}__{peak_label}"
                 #T.savefig(fig, kind="hist", wdir=wdir, label=fig_label)
                 src = T.fig_to_src(fig, dpi=150)
                 figures.append(html.Img(src=src, style={"width": "300px"}))
 
             if "density" in kinds:
                 # define your figure and axis
                 fig, ax = plt.subplots(figsize=(3, 3))
 
-                for label, group_df in grp.groupby(groupby):
+                for label, group_df in grp.groupby(colorby):
                     sns.kdeplot(
                         data=group_df,
-                        x=quant_col,
+                        x=var_name,
                         ax=ax,
                         label=label,
                         common_norm=False,
                     )
+                ax.set_xlabel(desc_short)
                 ax.set_title(peak_label)
                 ax.legend()
-                fig_label = f"by-{groupby}__{quant_col}__{peak_label}"
+                fig_label = f"by-{colorby}__{var_name}__{peak_label}"
                 #T.savefig(fig, kind="density", wdir=wdir, label=fig_label)
                 src = T.fig_to_src(fig, dpi=150)
                 figures.append(html.Img(src=src, style={"width": "300px"}))
 
             if "boxplot" in kinds:
-                n_groups = len(grp[groupby].drop_duplicates())
+                n_groups = len(grp[colorby].drop_duplicates())
                 aspect = max(1, n_groups / 10)
                 
                 # define your figure and axis
                 fig, ax = plt.subplots(figsize=(aspect*3, 3))
 
                 sns.boxplot(
                     data=grp,
-                    y=quant_col,
-                    x=groupby,
+                    y=var_name,
+                    x=colorby,
                     color="w",
                     ax=ax
                 )
 
-                if quant_col in ["peak_max", "peak_area"]:
+                if var_name in ["peak_max", "peak_area"]:
                     ax.ticklabel_format(axis="y", style="sci", scilimits=(0, 0))
-
+                ax.set_ylabel(desc_short)
                 ax.set_title(peak_label)
                 plt.xticks(rotation=90)
-                fig_label = f"by-{groupby}__{quant_col}__{peak_label}"
+                fig_label = f"by-{colorby}__{var_name}__{peak_label}"
                 #T.savefig(fig, kind="boxplot", wdir=wdir, label=fig_label)
                 src = T.fig_to_src(fig, dpi=150)
                 figures.append(html.Img(src=src, style={"width": "300px"}))
 
             if not "Dense" in options:
                 figures.append(dcc.Markdown("---"))
 
-            # if i == 3: break
-
-        return figures
+        return figures, desc
```

### Comparing `ms-mint-app-0.3.0/ms_mint_app/plugins/analysis_tools/heatmap.py` & `ms-mint-app-0.3.1/ms_mint_app/plugins/analysis_tools/heatmap.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,38 +3,37 @@
 from dash import html, dcc
 from dash.dependencies import Input, Output, State
 from dash.exceptions import PreventUpdate
 import dash_bootstrap_components as dbc
 
 from ms_mint.Mint import Mint
 from ms_mint.plotly_tools import plotly_heatmap
+from ms_mint.standards import MINT_RESULTS_COLUMNS
 
 from ... import tools as T
 
 _label = "Heatmap"
 
 
 heatmap_options = [
-    {"label": "Normalized by biomarker", "value": "normed_by_cols"},
     {"label": "Cluster", "value": "clustered"},
     {"label": "Dendrogram", "value": "add_dendrogram"},
     {"label": "Transposed", "value": "transposed"},
     {"label": "Correlation", "value": "correlation"},
     {"label": "Show in new tab", "value": "call_show"},
-    {"label": "log1p", "value": "log1p"},
 ]
 
 
 _layout = html.Div(
     [
         html.H3("Heatmap"),
         dbc.Button("Update", id="heatmap-update"),
         dcc.Dropdown(
             id="heatmap-options",
-            value=["normed_by_cols"],
+            value=[],
             options=heatmap_options,
             multi=True,
         ),
         dcc.Loading(
             html.Div(
                 [dcc.Graph(id="heatmap-figure")],
                 style={"height": "100vh", "marginTop": "50px"},
@@ -58,24 +57,32 @@
         if tab != _label:
             raise PreventUpdate
         return _layout
 
     @app.callback(
         Output("heatmap-figure", "figure"),
         Input("heatmap-update", "n_clicks"),
+        State("ana-var-name", "value"),
+        State("ana-groupby", "value"),
+        State("ana-scaler", "value"),
+        State("ana-apply", "value"),
         State("ana-file-types", "value"),
         State("ana-peak-labels-include", "value"),
         State("ana-peak-labels-exclude", "value"),
         State("ana-ms-order", "value"),
         State("heatmap-options", "value"),
         State("viewport-container", "children"),
         State("wdir", "children"),
     )
     def heat_heatmap(
         n_clicks,
+        var_name,
+        groupby,
+        scaler,
+        apply,
         file_types,
         include_labels,
         exclude_labels,
         ms_order,
         options,
         viewport,
         wdir,
@@ -90,40 +97,33 @@
             exclude_labels=exclude_labels,
             file_types=file_types,
         )
 
         if len(df) == 0:
             return "No results yet. First run MINT."
 
-        mint.results = df
+        mint.results = df[MINT_RESULTS_COLUMNS]
         mint.load_metadata(T.get_metadata_fn(wdir))
         
-        var_name = "peak_max"
-        data = mint.crosstab(var_name)
-        data.index = [T.Basename(i) for i in data.index]
-
-        if ms_order is not None and len(ms_order) > 0:
-            df = df.sort_values(ms_order)
-            ms_files = df["ms_file_id"].drop_duplicates()
-            data = data.loc[ms_files]
-
-        data.fillna(0, inplace=True)
-
-        name = var_name
-        if "log1p" in options:
-            data = data.apply(np.log1p)
-            name = f"log( {var_name}+1 )"
+        df = mint.crosstab(var_name=var_name, apply=apply, groupby=groupby, scaler=scaler)
+
+        if ms_order:
+            # ms_order might contain 'ms_file_label' which is the index of the dataframe
+            ndx = mint.meta.reset_index().sort_values(ms_order).set_index('ms_file_label').index.to_list()
+            df = df.reindex(ndx)
+
+        desc = T.describe_transformation(var_name=var_name, apply=apply, groupby=groupby, scaler=scaler)
 
         fig = plotly_heatmap(
-            data,
+            df,
             height=height,
             width=width,
-            normed_by_cols="normed_by_cols" in options,
+            #normed_by_cols="normed_by_cols" in options,
             transposed="transposed" in options,
             clustered="clustered" in options,
             add_dendrogram="add_dendrogram" in options,
             correlation="correlation" in options,
             call_show="call_show" in options,
-            name=name,
+            name=desc,
         )
 
         return fig
```

### Comparing `ms-mint-app-0.3.0/ms_mint_app/plugins/analysis_tools/hierachical_clustering.py` & `ms-mint-app-0.3.1/ms_mint_app/plugins/analysis_tools/hierachical_clustering.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from dash import html, dcc
 from dash.dependencies import Input, Output, State
 from dash.exceptions import PreventUpdate
 import dash_bootstrap_components as dbc
 
 from ms_mint.notebook import Mint
+from ms_mint.standards import MINT_RESULTS_COLUMNS
 
 from ... import tools as T
 
 
 _label = "Hierachical Clustering"
 
 _options = ["Transposed"]
@@ -77,31 +78,39 @@
         Output("hc-figures", "children"),
         Input("hc-update", "n_clicks"),
         State("hc-metric-x", "value"),
         State("hc-metric-y", "value"),        
         State("hc-figsize-x", "value"),
         State("hc-figsize-y", "value"),
         State("hc-options", "value"),
+        State("ana-var-name", "value"),
+        State("ana-colorby", "value"),
+        State("ana-groupby", "value"),
+        State("ana-scaler", "value"),
+        State("ana-apply", "value"),
         State("ana-file-types", "value"),
         State("ana-peak-labels-include", "value"),
         State("ana-peak-labels-exclude", "value"),
-        State("ana-ms-order", "value"),
         State("wdir", "children"),
     )
     def create_figure(
         n_clicks,
         metrix_x,
         metrix_y,
         fig_size_x,
         fig_size_y,
         options,
+        var_name,
+        colorby,
+        groupby,
+        scaler,
+        apply,
         file_types,
         include_labels,
         exclude_labels,
-        ms_order,
         wdir,
     ):
 
         if n_clicks is None:
             raise PreventUpdate
 
         if options is None: 
@@ -120,18 +129,22 @@
         df = T.get_complete_results(
             wdir,
             include_labels=include_labels,
             exclude_labels=exclude_labels,
             file_types=file_types,
         )
     
-        df["ms_file"] = df["ms_file_label"]
-        mint.results = df
+        mint.results = df[MINT_RESULTS_COLUMNS]
         mint.load_metadata(T.get_metadata_fn(wdir))
 
         fig = mint.plot.hierarchical_clustering(
-            figsize=(fig_size_x, fig_size_y), transposed="Transposed" in options, metric=(metrix_x, metrix_y)
+            figsize=(fig_size_x, fig_size_y), 
+            transposed="Transposed" in options, 
+            metric=(metrix_x, metrix_y), 
+            groupby=groupby, 
+            scaler=scaler,
+            apply=apply
         )
 
         src = T.fig_to_src(fig.figure)
 
         return html.Img(src=src, style={"maxWidth": "80%"})
```

### Comparing `ms-mint-app-0.3.0/ms_mint_app/plugins/analysis_tools/pca.py` & `ms-mint-app-0.3.1/ms_mint_app/plugins/analysis_tools/pca.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,25 @@
+import logging
+
 import numpy as np
 import seaborn as sns
 import plotly.express as px
 
 from dash import html, dcc
 from dash.dependencies import Input, Output, State
 from dash.exceptions import PreventUpdate
 
 import dash_bootstrap_components as dbc
 
 from ms_mint import Mint
+from ms_mint.standards import MINT_RESULTS_COLUMNS
 
 from ... import tools as T
 
-options = [{"value": i, "label": i} for i in ["Standard scaling", "Corner"]]
+options = []
 
 _layout = html.Div(
     [
         html.H3("Principal Components Analysis"),
         dbc.Button("Run PCA", id="pca-update"),
         dcc.Dropdown(
             id="pca-options",
@@ -71,98 +74,87 @@
 def callbacks(app, fsc, cache):
     @app.callback(
         Output("pca-figure-pairplot", "figure"),
         Output("pca-figure-explained-variance", "figure"),
         Output("pca-figure-contrib", "figure"),
         Input("pca-update", "n_clicks"),
         State("pca-nvars", "value"),
+        State("ana-var-name", "value"),
+        State("ana-colorby", "value"),
         State("ana-groupby", "value"),
+        State("ana-scaler", "value"),
+        State("ana-apply", "value"),
         State("ana-peak-labels-include", "value"),
         State("ana-peak-labels-exclude", "value"),
-        State("ana-normalization-cols", "value"),
         State("ana-file-types", "value"),
         State("pca-options", "value"),
+        State("viewport-container", "children"),
         State("wdir", "children"),
     )
     def create_pca(
         n_clicks,
         n_components,
+        var_name,
+        colorby,
         groupby,
+        scaler,
+        apply,
         include_labels,
         exclude_labels,
-        norm_cols,
         file_types,
         options,
+        viewport,
         wdir,
     ):
+        
+        width, height = [int(e) for e in viewport.split(",")]
+
         if n_clicks is None:
             raise PreventUpdate
-        if norm_cols is None:
-            norm_cols = []
+        if groupby is None:
+            groupby = []
 
         df = T.get_complete_results(
             wdir,
             include_labels=include_labels,
             exclude_labels=exclude_labels,
             file_types=file_types,
         )
 
-        if file_types is not None and len(file_types) > 0:
-            df = df[df["sample_type"].isin(file_types)]
-
-        if groupby is not None and len(groupby) > 0:
-            labels = (
-                df[["ms_file_label", groupby]].drop_duplicates().set_index("ms_file_label")
-            )
-        else:
-            labels = None
-            groupby = None
-
-        if len(norm_cols) != 0:
-            if ("peak_label" in norm_cols) and ("ms_file" in norm_cols):
-                return dbc.Alert(
-                    "'peak_label' and 'ms_file' should not be used together for normalization!",
-                    color="danger",
-                )
-
-            df = df[df.Batch.notna()]
-            cols = ["peak_max"]
-            df.loc[:, cols] = (
-                (
-                    df[cols]
-                    - df[cols + norm_cols]
-                    .groupby(norm_cols)
-                    .transform("median")[cols]
-                    .values
-                )
-                / df[cols + norm_cols].groupby(norm_cols).transform("std")[cols].values
-            ).reset_index()
-
         figures = []
         mint = Mint()
-        mint.results = df
+        mint.results = df[MINT_RESULTS_COLUMNS]
         mint.load_metadata(T.get_metadata_fn(wdir))
 
-        mint.pca.run(n_components=n_components)
+        n_peak_labels = len(mint.results.peak_label.drop_duplicates())
+
+        desc = T.describe_transformation(var_name=var_name, apply=apply, groupby=groupby, scaler=scaler)
+        desc_short = desc.split(" (")[0]
+
+        try:
+            mint.pca.run(var_name=var_name, n_components=n_components, groupby=groupby, scaler=scaler, apply=apply)
+        except RuntimeWarning as e:
+            logging.error(e)
+            return dbc.Alert(str(e), color="warning")
 
         fig_scattermatrix = mint.pca.plot.pairplot(
                 n_components=n_components,
-                hue=groupby,
+                hue=colorby,
                 interactive=True,
-                height=n_components*200+100,
-                width=n_components*200+100,
-                title='Principal components scatter plot',
+                height=min(n_components*200+100, width),
+                width=min(n_components*200+100, width),
+                title=f'Principal components scatter plot ({var_name})',
                 diag='box'
             )
 
-        fig_cumvar = mint.pca.plot.cumulative_variance(interactive=True, width=n_components*20+500)
+        fig_cumvar = mint.pca.plot.cumulative_variance(interactive=True, width=min(n_components*20+500, width))
 
         fig_contrib = mint.pca.plot.loadings(interactive=True, 
                                              height=n_components*200+100, 
-                                             width=len(mint.targets)*20+500,
-                                             title='Principal component loadings')
+                                             width=min(n_peak_labels*50+350, width),
+                                             title=f'Principal component loadings ({var_name})')
 
         fig_scattermatrix.update_layout(autosize=True)
         fig_cumvar.update_layout(autosize=True)        
         fig_contrib.update_layout(autosize=True)
 
         return fig_scattermatrix, fig_cumvar, fig_contrib
```

### Comparing `ms-mint-app-0.3.0/ms_mint_app/plugins/analysis_tools/plotting.py` & `ms-mint-app-0.3.1/ms_mint_app/plugins/analysis_tools/plotting.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+import logging
+
 from dash import html, dcc
 from dash.dependencies import Input, Output, State
 from dash.exceptions import PreventUpdate
 import dash_bootstrap_components as dbc
 
 from matplotlib import pyplot as plt
 
 import seaborn as sns
 
 plt.rcParams["figure.autolayout"] = False
 
+from ms_mint.Mint import Mint
+from ms_mint.standards import MINT_RESULTS_COLUMNS
 
 from ... import tools as T
-
+import pandas as pd
 
 _label = "Plotting"
 
 _kinds = [
     "bar",
     "violin",
     "box",
@@ -233,50 +237,49 @@
                 html.Label("Figure kind"),
                 dcc.Dropdown(id="plot-kind", options=kind_options, value="box"),
                 
                 dbc.Row([
                     html.Label("Facet width (inches):"),
                     dcc.Input( id="plot-fig-height", placeholder="Facet height", value=2.5, type="number"),
                     html.Label("Facet aspect ratio:"),
-                    dcc.Input( id="plot-fig-aspect", placeholder="Facet aspect", value=1, type="number"),   
+                    dcc.Input( id="plot-fig-aspect", placeholder="Facet aspect", value=2, type="number"),   
                 ]),
 
                 html.Label("Column wrap"),
-                dcc.Slider(id="plot-col-wrap", step=1, min=0, max=30, value=3),                 
+                dcc.Slider(id="plot-col-wrap", step=1, min=0, max=20, value=3),                 
             ]),
             dbc.Col([                
-                              
                 html.Label("x- and y-axes"),
-                dcc.Dropdown(id="plot-x", options=[{"value": "MS-file", "label": "MS-file"}], value=None, placeholder="X"),
+                dcc.Dropdown(id="plot-x", options=[{"value": "peak_label", "label": "peak_label"}], value='peak_label', placeholder="X"),
                 dcc.Dropdown(id="plot-y", options=[{"value": "peak_area_top3", "label": "peak_area_top3"}], value="peak_area_top3", placeholder="Y"),  
 
                 html.Label("Row and column facets:"),
                 dcc.Dropdown(id="plot-col", options=[{"value": "peak_label", "label": "peak_label"}], value=None, placeholder="Columns"),
                 dcc.Dropdown(id="plot-row", options=[], value=None, placeholder="Rows"), 
 
             ]),
             dbc.Col([
-
                 html.Label("Marker style and size:"),
                 dcc.Dropdown(id="plot-style", options=[], value=None, placeholder="Style"),
                 dcc.Dropdown(id="plot-size", options=[], value=None, placeholder="Size"),       
 
                 html.Label("Colors"),
                 dcc.Dropdown(id="plot-hue", options=[], value=None, placeholder="Color"),
                 dcc.Dropdown(id="plot-palette", options=palette_options, value=None, placeholder="Palette (Colors)",),
             ]),
             dbc.Col([                
-
                 html.Label("Figure title"),
                 dcc.Input(id="plot-title", placeholder="Figure title", value=None, style={'width': '100%'}),                  
             ]),
         ]),
         html.Label("Options"),
         dcc.Dropdown(id="plot-options", value=["sci", "share-x", "rot-x-ticks", "log-y"], options=options, multi=True),    
         dbc.Button("Update", id="plot-update"),
+
+        html.Center(html.H4("", id='plot-description'), style={'marginTop': "200px"}),
         dcc.Loading(
             html.Div(
                 id="plot-figures",
                 style={
                     "margin": "auto",
                     "marginTop": "10%",
                     "text-align": "center",
@@ -308,20 +311,22 @@
         State("wdir", "children"),
     )
     def fill_options(tab, wdir):
         if tab != _label:
             raise PreventUpdate
         results = T.get_complete_results(wdir)
         results = results.dropna(axis=1, how="all")
-        cols = results.columns
+        cols = results.columns.to_list()
+        cols.append('x')
         options = [{"value": x, "label": x} for x in cols]
         return [options] * 7
 
     @app.callback(
         Output("plot-figures", "children"),
+        Output("plot-description", "children"),
         Input("plot-update", "n_clicks"),
         State("plot-kind", "value"),
         State("plot-fig-height", "value"),
         State("plot-fig-aspect", "value"),
         State("plot-x", "value"),
         State("plot-y", "value"),
         State("plot-hue", "value"),
@@ -330,14 +335,18 @@
         State("plot-col-wrap", "value"),
         State("plot-style", "value"),
         State("plot-size", "value"),
         State("plot-title", "value"),
         State("ana-file-types", "value"),
         State("ana-peak-labels-include", "value"),
         State("ana-peak-labels-exclude", "value"),
+        State("ana-var-name", "value"),
+        State("ana-groupby", "value"),
+        State("ana-scaler", "value"),
+        State("ana-apply", "value"),
         State("ana-ms-order", "value"),
         State("plot-palette", "value"),
         State("plot-options", "value"),
         State("wdir", "children"),
         cancel=[Input("plot-update", "n_clicks")],
     )
     def create_figure(
@@ -353,14 +362,18 @@
         col_wrap,
         style,
         size,
         title,
         file_types,
         include_labels,
         exclude_labels,
+        var_name,
+        groupby,
+        scaler,
+        apply,
         ms_order,
         palette,
         options,
         wdir,
     ):
 
         if n_clicks is None:
@@ -374,26 +387,40 @@
         if aspect is None:
             aspect = 1
         if 'talk' in options:
             sns.set_context("talk")
         else:
             sns.set_context("paper")
 
+        if row is not None:
+            col_wrap = None
+
         height = min(float(height), 100)
         height = max(height, 1)
         aspect = max(0.01, float(aspect))
         aspect = min(aspect, 100)
 
         df = T.get_complete_results(
             wdir,
             include_labels=include_labels,
             exclude_labels=exclude_labels,
             file_types=file_types,
         )
 
+        mint = Mint()
+        mint.results = df[MINT_RESULTS_COLUMNS]
+        mint.load_metadata(T.get_metadata_fn(wdir))
+
+        df_2 = mint.crosstab(var_name=var_name, apply=apply, groupby=groupby, scaler=scaler)
+        df_2 = df_2.stack().to_frame().reset_index().rename(columns={0: 'x'})
+
+        desc = T.describe_transformation(var_name=var_name, apply=apply, groupby=groupby, scaler=scaler)
+
+        df = pd.merge(df, df_2, how='outer')
+
         df = df[(df.peak_n_datapoints > 0) & (df.peak_max > 0)]
 
         if ms_order is None or len(ms_order) == 0:
             df = df.sort_values(
                 [i for i in [col, row, hue, x, y, style, size] if i is not None]
             )
         else:
@@ -457,14 +484,15 @@
                 kind=kind,
                 height=height,
                 aspect=aspect,
                 palette=palette,
                 **kwargs
             )
         except Exception as e:
+            logging.error(e)
             return dbc.Alert(str(e), color="danger")
 
         g.fig.subplots_adjust(top=0.9)
         g.set_titles(col_template="{col_name}", row_template="{row_name}", y=1.05)
 
         if "log-x" in options:
             g.set(xscale="log")
@@ -488,8 +516,8 @@
         if title is not None:
             g.fig.suptitle(title, y=1.01)
 
         g.tight_layout(w_pad=0)
 
         src = T.fig_to_src(g.fig, dpi=300 if "HQ" in options else None)
 
-        return html.Img(src=src, style={"maxWidth": "80%"})
+        return html.Img(src=src, style={"maxWidth": "80%"}), f"x = {desc}"
```

### Comparing `ms-mint-app-0.3.0/ms_mint_app/plugins/metadata.py` & `ms-mint-app-0.3.1/ms_mint_app/plugins/metadata.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.0/ms_mint_app/plugins/ms_files.py` & `ms-mint-app-0.3.1/ms_mint_app/plugins/ms_files.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.0/ms_mint_app/plugins/processing.py` & `ms-mint-app-0.3.1/ms_mint_app/plugins/processing.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.0/ms_mint_app/plugins/quality_control.py` & `ms-mint-app-0.3.1/ms_mint_app/plugins/quality_control.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.0/ms_mint_app/plugins/target_optimization.py` & `ms-mint-app-0.3.1/ms_mint_app/plugins/target_optimization.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.0/ms_mint_app/plugins/targets.py` & `ms-mint-app-0.3.1/ms_mint_app/plugins/targets.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.0/ms_mint_app/plugins/workspaces.py` & `ms-mint-app-0.3.1/ms_mint_app/plugins/workspaces.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.0/ms_mint_app/static/ChEBI-Chem.parquet` & `ms-mint-app-0.3.1/ms_mint_app/static/ChEBI-Chem.parquet`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.0/ms_mint_app/static/ChEBI-Groups.parquet` & `ms-mint-app-0.3.1/ms_mint_app/static/ChEBI-Groups.parquet`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.0/ms_mint_app/tools.py` & `ms-mint-app-0.3.1/ms_mint_app/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,18 @@
 from ms_mint.standards import TARGETS_COLUMNS
 
 from datetime import date
 
 from .filelock import FileLock
 
 
+def list_to_options(x):
+    return [{"label": e, "value": e} for e in x]
+
+
 def lock(fn):
     return FileLock(f"{fn}.lock", timeout=1)
 
 
 def today():
     return date.today().strftime("%y%m%d")
 
@@ -790,7 +794,49 @@
     # Check if the first line is an empty line (contains only newline character)
     if lines[0] == "\n":
         logging.warning(f'Empty first line detected in {file_path}. Removing it.')
         lines.pop(0)
         
         with open(file_path, 'w') as file:
             file.writelines(lines)
+
+
+def describe_transformation(var_name, apply, groupby, scaler):
+
+    # Only apply the function if it's provided
+    if apply is not None:
+        apply_desc = transformations[apply]['description']
+        apply_desc = apply_desc.replace('x', var_name)
+    else:
+        apply_desc = var_name
+    
+    # If scaler or groupby is None, no scaling applied so return just the transformed variable
+    if groupby is None or scaler is None:
+        return apply_desc
+
+    if not scaler:
+        return apply_desc
+
+    # Define human-readable names for known scalers
+    scaler_mapping = {"standard": "Standard scaling", "robust": "Robust scaling", '': ''}  # expand as needed
+    if isinstance(scaler, str):
+        scaler_description = scaler_mapping.get(scaler.lower(), scaler)
+    else:
+        scaler_description = scaler.__name__
+    
+    # Groupby can be a list or a string, so make sure it's a list for consistent handling
+    if isinstance(groupby, str):
+        groupby = [groupby]
+    
+    groupby_description = ", ".join(groupby)
+    
+    # Scaling was applied, so return the description in < >
+    return f"<{apply_desc}> ({scaler_description}, grouped by {groupby_description})"
+
+
+log2p1 = lambda x: np.log2(1 + x)
+log1p = np.log1p
+
+transformations = {
+    "log1p":  {'function': log1p,  'description': 'log10(x + 1)'},
+    "log2p1": {'function': log2p1, 'description': 'log2(x + 1)' }
+}
```

### Comparing `ms-mint-app-0.3.0/ms_mint_app.egg-info/PKG-INFO` & `ms-mint-app-0.3.1/ms_mint_app.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-mint-app
-Version: 0.3.0
+Version: 0.3.1
 Summary: Metabolomics Integrator (Mint)
 Home-page: https://github.com/LewisResearchGroup/ms-mint-app
 Author: Soren Wacker
 Author-email: swacker@ucalgary.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ms-mint-app-0.3.0/ms_mint_app.egg-info/SOURCES.txt` & `ms-mint-app-0.3.1/ms_mint_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.0/scripts/Mint.py` & `ms-mint-app-0.3.1/scripts/Mint.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.0/setup.py` & `ms-mint-app-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.0/versioneer.py` & `ms-mint-app-0.3.1/versioneer.py`

 * *Files identical despite different names*

