# Comparing `tmp/bcirisktools-0.3.4.tar.gz` & `tmp/bcirisktools-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcirisktools-0.3.4.tar", last modified: Tue Jun  6 19:27:45 2023, max compression
+gzip compressed data, was "bcirisktools-0.3.5.tar", last modified: Fri Jul 14 16:10:34 2023, max compression
```

## Comparing `bcirisktools-0.3.4.tar` & `bcirisktools-0.3.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-06-06 19:27:45.338000 bcirisktools-0.3.4/
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     1063 2022-10-12 10:00:20.000000 bcirisktools-0.3.4/LICENCE
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      573 2023-06-06 19:27:45.333000 bcirisktools-0.3.4/PKG-INFO
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     4265 2022-12-02 15:48:25.000000 bcirisktools-0.3.4/README.md
-drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-06-06 19:27:45.207000 bcirisktools-0.3.4/bcirisktools/
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      308 2023-03-02 03:02:45.000000 bcirisktools-0.3.4/bcirisktools/__init__.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     5638 2023-06-06 19:27:22.000000 bcirisktools-0.3.4/bcirisktools/input_filters.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     1480 2023-03-02 03:02:45.000000 bcirisktools-0.3.4/bcirisktools/metrics_bci.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     7528 2023-03-02 03:02:45.000000 bcirisktools-0.3.4/bcirisktools/modeling.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)    10025 2023-03-23 00:01:50.000000 bcirisktools-0.3.4/bcirisktools/shapley_report.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     5783 2023-05-09 16:19:37.000000 bcirisktools-0.3.4/bcirisktools/stability.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)    19187 2023-05-09 13:13:17.000000 bcirisktools-0.3.4/bcirisktools/tree_crt.py
-drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-06-06 19:27:45.311000 bcirisktools-0.3.4/bcirisktools.egg-info/
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      573 2023-06-06 19:27:44.000000 bcirisktools-0.3.4/bcirisktools.egg-info/PKG-INFO
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      410 2023-06-06 19:27:44.000000 bcirisktools-0.3.4/bcirisktools.egg-info/SOURCES.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)        1 2023-06-06 19:27:44.000000 bcirisktools-0.3.4/bcirisktools.egg-info/dependency_links.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       78 2023-06-06 19:27:44.000000 bcirisktools-0.3.4/bcirisktools.egg-info/requires.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       13 2023-06-06 19:27:44.000000 bcirisktools-0.3.4/bcirisktools.egg-info/top_level.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       62 2023-03-02 03:02:45.000000 bcirisktools-0.3.4/pyproject.toml
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       38 2023-06-06 19:27:45.342000 bcirisktools-0.3.4/setup.cfg
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     1018 2023-06-06 19:27:40.000000 bcirisktools-0.3.4/setup.py
+drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-07-14 16:10:34.751000 bcirisktools-0.3.5/
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     1063 2022-10-12 10:00:20.000000 bcirisktools-0.3.5/LICENCE
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      573 2023-07-14 16:10:34.744000 bcirisktools-0.3.5/PKG-INFO
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     4265 2022-12-02 15:48:25.000000 bcirisktools-0.3.5/README.md
+drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-07-14 16:10:34.604000 bcirisktools-0.3.5/bcirisktools/
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      308 2023-03-02 03:02:45.000000 bcirisktools-0.3.5/bcirisktools/__init__.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     5638 2023-06-06 19:27:22.000000 bcirisktools-0.3.5/bcirisktools/input_filters.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     1480 2023-03-02 03:02:45.000000 bcirisktools-0.3.5/bcirisktools/metrics_bci.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     7528 2023-03-02 03:02:45.000000 bcirisktools-0.3.5/bcirisktools/modeling.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)    10038 2023-07-14 16:08:21.000000 bcirisktools-0.3.5/bcirisktools/shapley_report.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     5783 2023-05-09 16:19:37.000000 bcirisktools-0.3.5/bcirisktools/stability.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)    19187 2023-05-09 13:13:17.000000 bcirisktools-0.3.5/bcirisktools/tree_crt.py
+drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-07-14 16:10:34.725000 bcirisktools-0.3.5/bcirisktools.egg-info/
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      573 2023-07-14 16:10:34.000000 bcirisktools-0.3.5/bcirisktools.egg-info/PKG-INFO
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      410 2023-07-14 16:10:34.000000 bcirisktools-0.3.5/bcirisktools.egg-info/SOURCES.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)        1 2023-07-14 16:10:34.000000 bcirisktools-0.3.5/bcirisktools.egg-info/dependency_links.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       78 2023-07-14 16:10:34.000000 bcirisktools-0.3.5/bcirisktools.egg-info/requires.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       13 2023-07-14 16:10:34.000000 bcirisktools-0.3.5/bcirisktools.egg-info/top_level.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       62 2023-03-02 03:02:45.000000 bcirisktools-0.3.5/pyproject.toml
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       38 2023-07-14 16:10:34.755000 bcirisktools-0.3.5/setup.cfg
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     1018 2023-07-14 16:09:16.000000 bcirisktools-0.3.5/setup.py
```

### Comparing `bcirisktools-0.3.4/LICENCE` & `bcirisktools-0.3.5/LICENCE`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.3.4/PKG-INFO` & `bcirisktools-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcirisktools
-Version: 0.3.4
+Version: 0.3.5
 Summary: BCI risks tools
 Author: Mezosky
 Author-email: <imezadelajara@gmail.com>
 Keywords: python,risk,tools,bci
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bcirisktools-0.3.4/README.md` & `bcirisktools-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.3.4/bcirisktools/input_filters.py` & `bcirisktools-0.3.5/bcirisktools/input_filters.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.3.4/bcirisktools/metrics_bci.py` & `bcirisktools-0.3.5/bcirisktools/metrics_bci.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.3.4/bcirisktools/modeling.py` & `bcirisktools-0.3.5/bcirisktools/modeling.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.3.4/bcirisktools/shapley_report.py` & `bcirisktools-0.3.5/bcirisktools/shapley_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,18 +86,19 @@
             (self.predVar["KS"] > 0.01) & (self.predVar["ROC"] > 0.501), :
         ]
         self.variables_univariate = self.predVar["Features"]
 
     def _plot_shaps(self, study_var, x_label="", shap_nulls=False):
         if shap_nulls:
             cond = self.X_train[study_var].values >= self.min_value
-            shaps_values = self.shap_values.values[cond]
+            shaps_values = self.shap_values.values[... , -1][cond]
             inputs_x = self.X_train[cond]
         else:
-            shaps_values = self.shap_values.values
+            
+            shaps_values = self.shap_values.values[... , -1]
             inputs_x = self.X_train
 
         shap.dependence_plot(
             study_var,
             shaps_values,
             inputs_x,
             xmin="percentile(0.5)",
@@ -121,15 +122,15 @@
         # Univariate analysis
         print("/------------------------------------------------------/")
         print("Initializing univariate analysis...")
         print("/------------------------------------------------------/")
         self._univariate_analysis()
 
         # Redefine data
-        self.X_train = self.X_train[self.variables_univariate]
+        self.X_train = self.X_train
 
         # Get Shapley values
         print("\n/------------------------------------------------------/")
         print("Calculating Shapley values...")
         print("/------------------------------------------------------/")
         if self.model is None:
             self.dtrain = xgb.DMatrix(self.X_train, label=self.y_train)
@@ -137,15 +138,15 @@
         explainer = shap.TreeExplainer(self.model)
         self.shap_values = explainer(self.X_train)
 
         var_names = self.shap_values.feature_names
         var_shap = np.abs(self.shap_values.values).mean(axis=0)
 
         self.df_shap = pd.DataFrame(
-            zip(var_names, var_shap), columns=["Features", "Mean Shapley"]
+            zip(var_names, var_shap[:, -1]), columns=["Features", "Mean Shapley"]
         )
         self.df_shap = self.df_shap.sort_values(
             by="Mean Shapley", ascending=False
         ).reset_index(drop=True)
         self.df_shap_top = self.df_shap.head(10)
 
         # Final Dataframe
```

### Comparing `bcirisktools-0.3.4/bcirisktools/stability.py` & `bcirisktools-0.3.5/bcirisktools/stability.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.3.4/bcirisktools/tree_crt.py` & `bcirisktools-0.3.5/bcirisktools/tree_crt.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.3.4/bcirisktools.egg-info/PKG-INFO` & `bcirisktools-0.3.5/bcirisktools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcirisktools
-Version: 0.3.4
+Version: 0.3.5
 Summary: BCI risks tools
 Author: Mezosky
 Author-email: <imezadelajara@gmail.com>
 Keywords: python,risk,tools,bci
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bcirisktools-0.3.4/setup.py` & `bcirisktools-0.3.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = "0.3.4"
+VERSION = "0.3.5"
 DESCRIPTION = "BCI risks tools"
 LONG_DESCRIPTION = "A package that compiles different risk tools used by BCI bank."
 
 # Setting up
 setup(
     name="bcirisktools",
     version=VERSION,
```

