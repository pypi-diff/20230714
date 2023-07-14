# Comparing `tmp/protloc_mex1-0.0.8.tar.gz` & `tmp/protloc_mex1-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protloc_mex1-0.0.8.tar", last modified: Fri Jul  7 03:53:16 2023, max compression
+gzip compressed data, was "protloc_mex1-0.0.9.tar", last modified: Fri Jul 14 03:42:09 2023, max compression
```

## Comparing `protloc_mex1-0.0.8.tar` & `protloc_mex1-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 03:53:16.362831 protloc_mex1-0.0.8/
--rw-rw-rw-   0        0        0     1091 2023-04-25 08:38:35.000000 protloc_mex1-0.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0     7733 2023-07-07 03:53:16.361831 protloc_mex1-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     6953 2023-05-15 09:50:59.000000 protloc_mex1-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 03:53:16.327175 protloc_mex1-0.0.8/protloc_mex1/
--rw-rw-rw-   0        0        0    19901 2023-06-12 12:11:40.000000 protloc_mex1-0.0.8/protloc_mex1/AA_count.py
--rw-rw-rw-   0        0        0     8014 2023-04-29 12:40:52.000000 protloc_mex1-0.0.8/protloc_mex1/GO_count.py
--rw-rw-rw-   0        0        0    10510 2023-04-28 13:10:04.000000 protloc_mex1-0.0.8/protloc_mex1/SHAP_conduct.py
--rw-rw-rw-   0        0        0    33141 2023-07-03 03:39:28.000000 protloc_mex1-0.0.8/protloc_mex1/SHAP_plus.py
--rw-rw-rw-   0        0        0       39 2023-04-29 12:25:34.000000 protloc_mex1-0.0.8/protloc_mex1/__init__.py
--rw-rw-rw-   0        0        0    14425 2023-06-22 02:36:30.000000 protloc_mex1-0.0.8/protloc_mex1/classifier_evalute.py
-drwxrwxrwx   0        0        0        0 2023-07-07 03:53:16.360330 protloc_mex1-0.0.8/protloc_mex1.egg-info/
--rw-rw-rw-   0        0        0     7733 2023-07-07 03:53:16.000000 protloc_mex1-0.0.8/protloc_mex1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      380 2023-07-07 03:53:16.000000 protloc_mex1-0.0.8/protloc_mex1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 03:53:16.000000 protloc_mex1-0.0.8/protloc_mex1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2023-07-07 03:53:16.000000 protloc_mex1-0.0.8/protloc_mex1.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-07 03:53:16.000000 protloc_mex1-0.0.8/protloc_mex1.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      859 2023-07-07 03:47:35.000000 protloc_mex1-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-07 03:53:16.362831 protloc_mex1-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-14 03:42:09.484559 protloc_mex1-0.0.9/
+-rw-rw-rw-   0        0        0     1091 2023-04-25 08:38:35.000000 protloc_mex1-0.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     7733 2023-07-14 03:42:09.483560 protloc_mex1-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     6953 2023-05-15 09:50:59.000000 protloc_mex1-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 03:42:09.471730 protloc_mex1-0.0.9/protloc_mex1/
+-rw-rw-rw-   0        0        0    19901 2023-06-12 12:11:40.000000 protloc_mex1-0.0.9/protloc_mex1/AA_count.py
+-rw-rw-rw-   0        0        0     8019 2023-07-13 04:13:20.000000 protloc_mex1-0.0.9/protloc_mex1/GO_count.py
+-rw-rw-rw-   0        0        0     4006 2023-07-13 14:50:38.000000 protloc_mex1-0.0.9/protloc_mex1/IG_calculator.py
+-rw-rw-rw-   0        0        0    14849 2023-07-12 10:44:12.000000 protloc_mex1-0.0.9/protloc_mex1/SHAP_conduct.py
+-rw-rw-rw-   0        0        0    33141 2023-07-03 03:39:28.000000 protloc_mex1-0.0.9/protloc_mex1/SHAP_plus.py
+-rw-rw-rw-   0        0        0      167 2023-07-13 03:52:08.000000 protloc_mex1-0.0.9/protloc_mex1/__init__.py
+-rw-rw-rw-   0        0        0    14425 2023-06-22 02:36:30.000000 protloc_mex1-0.0.9/protloc_mex1/classifier_evalute.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:42:09.482560 protloc_mex1-0.0.9/protloc_mex1.egg-info/
+-rw-rw-rw-   0        0        0     7733 2023-07-14 03:42:09.000000 protloc_mex1-0.0.9/protloc_mex1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2023-07-14 03:42:09.000000 protloc_mex1-0.0.9/protloc_mex1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 03:42:09.000000 protloc_mex1-0.0.9/protloc_mex1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      105 2023-07-14 03:42:09.000000 protloc_mex1-0.0.9/protloc_mex1.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-14 03:42:09.000000 protloc_mex1-0.0.9/protloc_mex1.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      882 2023-07-14 03:40:27.000000 protloc_mex1-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-14 03:42:09.484559 protloc_mex1-0.0.9/setup.cfg
```

### Comparing `protloc_mex1-0.0.8/LICENSE.txt` & `protloc_mex1-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `protloc_mex1-0.0.8/PKG-INFO` & `protloc_mex1-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: protloc_mex1
-Version: 0.0.8
+Version: 0.0.9
 Summary: ...
 Author-email: Ze Yu Luo <1024226968@qq.com>
 Project-URL: Homepage, https://github.com/yujuan-zhang/ProtLoc-mexl
 Project-URL: Bug Tracker, https://github.com/yujuan-zhang/ProtLoc-mexl/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: ==3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # ProtLoc-Mex1
 
 ## Introduction ProtLoc-Mex1
```

### Comparing `protloc_mex1-0.0.8/README.md` & `protloc_mex1-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `protloc_mex1-0.0.8/protloc_mex1/AA_count.py` & `protloc_mex1-0.0.9/protloc_mex1/AA_count.py`

 * *Files identical despite different names*

### Comparing `protloc_mex1-0.0.8/protloc_mex1/GO_count.py` & `protloc_mex1-0.0.9/protloc_mex1/GO_count.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,18 +16,17 @@
 import warnings
 try:
     import gensim
     if version.parse(gensim.__version__) < version.parse('4.2.0'):
         warnings.warn("Your gensim version is older than 4.2.0  +\
                       and may be not operation correct.")
 except ImportError:
-    raise ValueError('gensim is not installed so this module is not available! Run `pip install gensim` " \
+    raise ValueError('gensim is not installed so this module is not available! Run `pip install gensim==4.2.0` " \
                              "to fix this ')
 
-
 ## Building sentence processing functions
 def read_corpus(sequence_input, tokens_only=False):
     '''
     
     
     Reads input text data and yields tokenized sentences or tagged sentences.
```

### Comparing `protloc_mex1-0.0.8/protloc_mex1/SHAP_conduct.py` & `protloc_mex1-0.0.9/protloc_mex1/SHAP_conduct.py`

 * *Files 16% similar despite different names*

```diff
@@ -257,7 +257,123 @@
 
         X_random = X_input.sample(frac=self.frac_num, replace=False, random_state=0, axis=0)
         shap_interaction_values = self.explainer.shap_interaction_values(X_random, tree_limit=self.tree_limit_num)
 
         self.save_shap_interaction_index(shap_interaction_values, X_random, file_name, save_path,type_class)
 
 
+
+class DeepSHAPValueConduct:
+    '''
+    A class used to analyze Deep SHAP values.
+    
+    Attributes:
+    ----------
+    explainer : SHAP DeepExplainer 
+        The explainer used to calculate SHAP values.
+    X_input : DataFrame
+        Input features.
+    y_input : Series, DataFrame
+        Target values.
+    '''
+    def __init__(self, explainer , X_input, X_input_tensor,y_input):
+        
+        
+        # Randomly select samples from X_input to form the background dataset
+        
+        self.explainer = explainer 
+        self.X_input = X_input
+        self.X_input_tensor=X_input_tensor
+        self.y_input = y_input
+    
+    def shap_value_conduct(self):
+        '''
+        Calculate the SHAP values of X_input using explainer.
+
+        Returns
+        -------
+        shap_values : list
+            SHAP values for each sample in X_input for each localization.
+        '''
+        self.shap_values = self.explainer.shap_values(self.X_input_tensor)  # Convert DataFrame to numpy array
+        return self.shap_values
+
+    def save_shap_values(self, X_predict_input,shap_value_input,X_input,y_input, type_class,save_path,file_name,gene_ID):
+        '''
+        
+
+        Save SHAP values, input features, target values and predictions to CSV file.  
+
+        Parameters
+        ----------
+        X_predict_input : DataFrame
+            Model predictions for X_input. 
+        shap_value_input : list
+            SHAP values for each sample in X_input for One localization.
+        X_input : DataFrame
+            Input features.
+        y_input : Series, DataFrame
+            Target values.
+        type_class : str
+            One target class name.               
+        save_path : str
+            input is file or plot save path way with no contain file name.
+        file_name : str
+            only indicate test or train but not specific file name, 
+            such as input can't be classification_report.csv.
+        gene_ID : str
+            Name of the index column.
+
+        Returns
+        -------
+        X_shap_save : DataFrame
+            Combined information of SHAP values, inputs, targets and predictions.
+
+        '''
+                
+        X_shap_save = pd.DataFrame(shap_value_input, columns=X_input.columns, index=X_input.index)
+        X_shap_save = X_shap_save.join(y_input, how="inner")
+        X_shap_save = X_shap_save.join(X_predict_input, how="inner")
+        file_path = f"{save_path}/{file_name}_{type_class}_shap_value.csv"
+        X_shap_save.to_csv(file_path, index_label=gene_ID)
+        return X_shap_save
+        
+
+    def Shapley_value_save(self,X_predict_input,type_class,save_path,file_name="train",gene_ID='ID'):
+        '''
+        
+
+        Save SHAP values for different classes.
+        
+        Parameters
+        ----------
+        X_predict_input : DataFrame
+            Model predictions for X_input.  
+        type_class : list
+            Names of the target classes.                 
+        save_path : str
+            input is file or plot save path way with no contain file name.
+        file_name : str, optional
+            only indicate test or train but not specific file name, The default is "train".
+        gene_ID : str, optional
+            Name of the index column. The default is 'ID'.
+        
+        Returns
+        -------
+        X_shap_save : dict
+            Saved information of SHAP values (SHAP values, inputs, targets and predictions) for each class.
+        
+        Note
+        -------
+        Please ensure that the type entered for the type_class parameter matches 
+        the type of the model default classification,
+        otherwise the results may be inaccurate!
+        '''
+        logging.warning('Please ensure that the type entered for the type_class parameter matches the type of the model default classification,\
+                        otherwise the results may be inaccurate!')
+        X_shap_save=list(map(lambda x,y:self.save_shap_values(X_predict_input,\
+                                    self.shap_values[y],self.X_input,self.y_input,x,save_path,file_name,gene_ID),type_class,range(len(type_class))))
+        X_shap_save=dict(zip(type_class,X_shap_save))
+        return X_shap_save
+    
+    
+
```

### Comparing `protloc_mex1-0.0.8/protloc_mex1/SHAP_plus.py` & `protloc_mex1-0.0.9/protloc_mex1/SHAP_plus.py`

 * *Files identical despite different names*

### Comparing `protloc_mex1-0.0.8/protloc_mex1/classifier_evalute.py` & `protloc_mex1-0.0.9/protloc_mex1/classifier_evalute.py`

 * *Files identical despite different names*

### Comparing `protloc_mex1-0.0.8/protloc_mex1.egg-info/PKG-INFO` & `protloc_mex1-0.0.9/protloc_mex1.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: protloc-mex1
-Version: 0.0.8
+Version: 0.0.9
 Summary: ...
 Author-email: Ze Yu Luo <1024226968@qq.com>
 Project-URL: Homepage, https://github.com/yujuan-zhang/ProtLoc-mexl
 Project-URL: Bug Tracker, https://github.com/yujuan-zhang/ProtLoc-mexl/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: ==3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # ProtLoc-Mex1
 
 ## Introduction ProtLoc-Mex1
```

### Comparing `protloc_mex1-0.0.8/pyproject.toml` & `protloc_mex1-0.0.9/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "protloc_mex1"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Ze Yu Luo", email="1024226968@qq.com" },
 ]
 description = "..."
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = "==3.9"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
         "biopython~=1.79",
         "numpy>=1.20.3",
         "pandas>=1.4.1",
         "seaborn>=0.11.2",
         "matplotlib>=3.5.1",
-        "shap~=0.41.0",
+        "shap==0.41.0",
+        "gensim==4.2.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/yujuan-zhang/ProtLoc-mexl"
 "Bug Tracker" = "https://github.com/yujuan-zhang/ProtLoc-mexl/issues"
-
```

