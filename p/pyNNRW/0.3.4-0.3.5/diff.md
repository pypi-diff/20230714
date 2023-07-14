# Comparing `tmp/pyNNRW-0.3.4.tar.gz` & `tmp/pyNNRW-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyNNRW-0.3.4.tar", last modified: Wed Jul  5 11:01:17 2023, max compression
+gzip compressed data, was "pyNNRW-0.3.5.tar", last modified: Fri Jul 14 03:00:37 2023, max compression
```

## Comparing `pyNNRW-0.3.4.tar` & `pyNNRW-0.3.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 11:01:17.274625 pyNNRW-0.3.4/
--rw-rw-rw-   0        0        0      214 2022-03-26 07:50:46.000000 pyNNRW-0.3.4/LICENCE
--rw-rw-rw-   0        0        0     4106 2023-07-05 11:01:17.277629 pyNNRW-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     3458 2022-05-10 04:41:05.000000 pyNNRW-0.3.4/README.md
--rw-rw-rw-   0        0        0      108 2022-01-07 07:21:30.000000 pyNNRW-0.3.4/pyproject.toml
--rw-rw-rw-   0        0        0      906 2023-07-05 11:01:17.286623 pyNNRW-0.3.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-05 11:01:16.817922 pyNNRW-0.3.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-05 11:01:17.254623 pyNNRW-0.3.4/src/pyNNRW/
--rw-rw-rw-   0        0        0     2044 2023-04-07 01:49:33.000000 pyNNRW-0.3.4/src/pyNNRW/__init__.py
--rw-rw-rw-   0        0        0      239 2022-05-20 11:56:20.000000 pyNNRW-0.3.4/src/pyNNRW/aerw.py
--rw-rw-rw-   0        0        0      777 2022-05-20 11:56:20.000000 pyNNRW-0.3.4/src/pyNNRW/dtc.py
--rw-rw-rw-   0        0        0    18109 2023-07-03 09:13:36.000000 pyNNRW-0.3.4/src/pyNNRW/elm.py
--rw-rw-rw-   0        0        0      128 2022-05-20 11:56:20.000000 pyNNRW-0.3.4/src/pyNNRW/knn.py
--rw-rw-rw-   0        0        0    13110 2023-07-03 09:52:09.000000 pyNNRW-0.3.4/src/pyNNRW/knnrw.py
--rw-rw-rw-   0        0        0      509 2022-05-20 11:56:20.000000 pyNNRW-0.3.4/src/pyNNRW/lr.py
--rw-rw-rw-   0        0        0     7233 2022-05-20 11:56:20.000000 pyNNRW-0.3.4/src/pyNNRW/mlp.py
--rw-rw-rw-   0        0        0    24246 2023-07-05 10:32:40.000000 pyNNRW-0.3.4/src/pyNNRW/nnrw.py
--rw-rw-rw-   0        0        0     8033 2022-05-20 11:56:20.000000 pyNNRW-0.3.4/src/pyNNRW/rbfnn.py
--rw-rw-rw-   0        0        0     8632 2022-05-20 11:56:20.000000 pyNNRW-0.3.4/src/pyNNRW/rbm.py
--rw-rw-rw-   0        0        0    17215 2023-07-05 05:52:42.000000 pyNNRW-0.3.4/src/pyNNRW/rvfl.py
--rw-rw-rw-   0        0        0     1436 2022-05-20 11:56:20.000000 pyNNRW-0.3.4/src/pyNNRW/wann.py
-drwxrwxrwx   0        0        0        0 2023-07-05 11:01:17.269621 pyNNRW-0.3.4/src/pyNNRW.egg-info/
--rw-rw-rw-   0        0        0     4106 2023-07-05 11:01:16.000000 pyNNRW-0.3.4/src/pyNNRW.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      457 2023-07-05 11:01:16.000000 pyNNRW-0.3.4/src/pyNNRW.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 11:01:16.000000 pyNNRW-0.3.4/src/pyNNRW.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-07-05 11:01:16.000000 pyNNRW-0.3.4/src/pyNNRW.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-05 11:01:16.000000 pyNNRW-0.3.4/src/pyNNRW.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 03:00:37.692155 pyNNRW-0.3.5/
+-rw-rw-rw-   0        0        0      214 2022-03-26 07:50:46.000000 pyNNRW-0.3.5/LICENCE
+-rw-rw-rw-   0        0        0     4106 2023-07-14 03:00:37.693125 pyNNRW-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3458 2022-05-10 04:41:05.000000 pyNNRW-0.3.5/README.md
+-rw-rw-rw-   0        0        0      108 2022-01-07 07:21:30.000000 pyNNRW-0.3.5/pyproject.toml
+-rw-rw-rw-   0        0        0      906 2023-07-14 03:00:37.703119 pyNNRW-0.3.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-14 03:00:37.409797 pyNNRW-0.3.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-14 03:00:37.658585 pyNNRW-0.3.5/src/pyNNRW/
+-rw-rw-rw-   0        0        0     2044 2023-04-07 01:49:33.000000 pyNNRW-0.3.5/src/pyNNRW/__init__.py
+-rw-rw-rw-   0        0        0      239 2022-05-20 11:56:20.000000 pyNNRW-0.3.5/src/pyNNRW/aerw.py
+-rw-rw-rw-   0        0        0      777 2022-05-20 11:56:20.000000 pyNNRW-0.3.5/src/pyNNRW/dtc.py
+-rw-rw-rw-   0        0        0    18109 2023-07-03 09:13:36.000000 pyNNRW-0.3.5/src/pyNNRW/elm.py
+-rw-rw-rw-   0        0        0      128 2022-05-20 11:56:20.000000 pyNNRW-0.3.5/src/pyNNRW/knn.py
+-rw-rw-rw-   0        0        0    13110 2023-07-03 09:52:09.000000 pyNNRW-0.3.5/src/pyNNRW/knnrw.py
+-rw-rw-rw-   0        0        0      509 2022-05-20 11:56:20.000000 pyNNRW-0.3.5/src/pyNNRW/lr.py
+-rw-rw-rw-   0        0        0     7233 2022-05-20 11:56:20.000000 pyNNRW-0.3.5/src/pyNNRW/mlp.py
+-rw-rw-rw-   0        0        0    24607 2023-07-14 02:26:04.000000 pyNNRW-0.3.5/src/pyNNRW/nnrw.py
+-rw-rw-rw-   0        0        0     8033 2022-05-20 11:56:20.000000 pyNNRW-0.3.5/src/pyNNRW/rbfnn.py
+-rw-rw-rw-   0        0        0     8632 2022-05-20 11:56:20.000000 pyNNRW-0.3.5/src/pyNNRW/rbm.py
+-rw-rw-rw-   0        0        0    17369 2023-07-14 02:21:08.000000 pyNNRW-0.3.5/src/pyNNRW/rvfl.py
+-rw-rw-rw-   0        0        0     1436 2022-05-20 11:56:20.000000 pyNNRW-0.3.5/src/pyNNRW/wann.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:00:37.689111 pyNNRW-0.3.5/src/pyNNRW.egg-info/
+-rw-rw-rw-   0        0        0     4106 2023-07-14 03:00:37.000000 pyNNRW-0.3.5/src/pyNNRW.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2023-07-14 03:00:37.000000 pyNNRW-0.3.5/src/pyNNRW.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 03:00:37.000000 pyNNRW-0.3.5/src/pyNNRW.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-07-14 03:00:37.000000 pyNNRW-0.3.5/src/pyNNRW.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-14 03:00:37.000000 pyNNRW-0.3.5/src/pyNNRW.egg-info/top_level.txt
```

### Comparing `pyNNRW-0.3.4/PKG-INFO` & `pyNNRW-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyNNRW
-Version: 0.3.4
+Version: 0.3.5
 Summary: A Python library for NNRW (neural network with random weights)
 Home-page: https://github.com/zhangys11/pyNNRW
 Author: Yinsheng Zhang (Ph.D.)
 Author-email: oo@zju.edu.cn
 Project-URL: Bug Tracker, https://github.com/zhangys11/pyNNRW/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `pyNNRW-0.3.4/README.md` & `pyNNRW-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `pyNNRW-0.3.4/setup.cfg` & `pyNNRW-0.3.5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 794e 4e52 570d 0a76 6572 7369   = pyNNRW..versi
-00000020: 6f6e 203d 2030 2e33 2e34 0d0a 6175 7468  on = 0.3.4..auth
+00000020: 6f6e 203d 2030 2e33 2e35 0d0a 6175 7468  on = 0.3.5..auth
 00000030: 6f72 203d 2059 696e 7368 656e 6720 5a68  or = Yinsheng Zh
 00000040: 616e 6720 2850 682e 442e 290d 0a61 7574  ang (Ph.D.)..aut
 00000050: 686f 725f 656d 6169 6c20 3d20 6f6f 407a  hor_email = oo@z
 00000060: 6a75 2e65 6475 2e63 6e0d 0a64 6573 6372  ju.edu.cn..descr
 00000070: 6970 7469 6f6e 203d 2041 2050 7974 686f  iption = A Pytho
 00000080: 6e20 6c69 6272 6172 7920 666f 7220 4e4e  n library for NN
 00000090: 5257 2028 6e65 7572 616c 206e 6574 776f  RW (neural netwo
```

### Comparing `pyNNRW-0.3.4/src/pyNNRW/__init__.py` & `pyNNRW-0.3.5/src/pyNNRW/__init__.py`

 * *Files identical despite different names*

### Comparing `pyNNRW-0.3.4/src/pyNNRW/dtc.py` & `pyNNRW-0.3.5/src/pyNNRW/dtc.py`

 * *Files identical despite different names*

### Comparing `pyNNRW-0.3.4/src/pyNNRW/elm.py` & `pyNNRW-0.3.5/src/pyNNRW/elm.py`

 * *Files identical despite different names*

### Comparing `pyNNRW-0.3.4/src/pyNNRW/knnrw.py` & `pyNNRW-0.3.5/src/pyNNRW/knnrw.py`

 * *Files identical despite different names*

### Comparing `pyNNRW-0.3.4/src/pyNNRW/mlp.py` & `pyNNRW-0.3.5/src/pyNNRW/mlp.py`

 * *Files identical despite different names*

### Comparing `pyNNRW-0.3.4/src/pyNNRW/nnrw.py` & `pyNNRW-0.3.5/src/pyNNRW/nnrw.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-import warnings
-warnings.filterwarnings("ignore")
-
 import time
+import warnings
 import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib.ticker as mticker
 from sklearn.base import BaseEstimator, ClassifierMixin
 from sklearn.model_selection import train_test_split
-from sklearn.linear_model import LogisticRegression
+from sklearn.linear_model import LogisticRegression, LogisticRegressionCV
 from sklearn.ensemble import StackingClassifier #,HistGradientBoostingClassifier
 from sklearn.tree import DecisionTreeClassifier
 from sklearn.svm import SVC
 from sklearn.multiclass import OneVsOneClassifier
 from sklearn.metrics import r2_score
 
 from . import to_categorical
 
+warnings.filterwarnings("ignore")
+
 #region Performance Test. Compare NNRW with mainstream classifier models.
 
 def ELMClf(X, y, L = 100, verbose = False):
     '''
     A wrapper for ELM.
     L represents the number of hidden layer nodes.
     '''
@@ -522,28 +522,35 @@
         plt.ylim(YLIM) # e.g., (.4, 1.05)
     plt.show()
 
     print('best test accuracy: ', max(dic_acc.values()), 'N, L = ', [key for key, value in dic_acc.items() if value == max(dic_acc.values())])
 
     return dic_acc
     
-def hetero_stacking(X, y, estimators, repeat = 10, WITH_CONTEXT = True):
+def hetero_stacking(X, y, estimators,
+                    test_size = .3, random_state = None,
+                    WITH_CONTEXT = False, repeat = 5):
     '''
     estimators: a batch of base learners. Each learner should be derived from the BaseEstimator type.    
     '''
     acc = 0
+    repeat = 1
     
-    for iter in range(repeat):
+    for _ in range(repeat):
 
         X_train, X_test, y_train, y_test = train_test_split(
-            X, y
+            X, y, stratify=y,
+            test_size= test_size,
+            random_state=random_state
         )
 
         clf = StackingClassifier(
-            estimators=estimators, final_estimator=LogisticRegressionCV(), passthrough = WITH_CONTEXT
+            estimators=estimators, 
+            final_estimator=LogisticRegressionCV(),
+            passthrough = WITH_CONTEXT
         )
 
         acc = acc + clf.fit(X_train, y_train).score(X_test, y_test)
     
     return acc / repeat
 
 class FSSE(BaseEstimator, ClassifierMixin):
@@ -565,51 +572,52 @@
     
     '''
     def __init__(self, create_base_estimator_cv, feature_split = 'all', meta_l1_ratios = [0.5,0.6,0.7,0.8,0.9,1.0]):
 
         self.create_base_estimator_cv = create_base_estimator_cv
         self.feature_split = feature_split
         self.meta_l1_ratios = meta_l1_ratios
+        self.base_learners = {}
+        self.meta_learner = None
 
-    def fit(self, X, y):     
+    def fit(self, X, y):
         
         if isinstance(self.feature_split, int):
             self.feature_split = abs(self.feature_split)
 
         if (self.feature_split == 'all' or self.feature_split >= X.shape[1]):
             self.feature_split = X.shape[1] 
 
-        X_train, X_test, y_train, y_test = train_test_split(X, y)
-        
-        self.base_learners = {}
+        X_train, X_test, y_train, y_test = train_test_split(X, y, stratify=y)
+                
         predicts = []
         for i in range(0, X.shape[1], self.feature_split): # TODO: padding to N*feature_split, or special treatment for the last group.
             clfcv = self.create_base_estimator_cv().fit(X_train[:,i:i+ self.feature_split], y_train)
             self.base_learners[(i, i + self.feature_split)] = clfcv.clf.best_estimator_ # the inner best model
             predicts.append( clfcv.predict(X_test[:,i:i+ self.feature_split]) )
 
         predicts = np.array(predicts).T
         # print(predicts.shape)
         # print(X_test.shape, y_test.shape)
         self.meta_learner = LogisticRegressionCV(penalty = 'elasticnet',  # use elasticnet penalty to get sparse result
                                             l1_ratios = self.meta_l1_ratios, # require at least 0.5 L1 ratio for sparsity
                                            solver = 'saga' # only saga support elasticnet penalty
-                                           ).fit(predicts ,y_test)  
+                                           ).fit(predicts ,y_test)
         # print(meta_learner.l1_ratio_)
         # plt.plot(meta_learner.coef_[0])
         # return base_learners, meta_learner  
 
     def base_predict(self, X):
         '''
         base leaners' prediction, used as the input for meta-learner
         '''
         predicts = []
-        for b in self.base_learners:
-            FS = X[:,b[0]:b[1]]
-            yhat = self.base_learners[b].predict(FS)
+        for k, b in self.base_learners.items():
+            FS = X[:,k[0]:k[1]]
+            yhat = b.predict(FS)
             predicts.append(yhat)
 
         return np.array(predicts).T
 
     def predict(self, X):
 
         predicts = self.base_predict(X)
@@ -676,36 +684,38 @@
         for w in self.meta_learner.coef_[0]:
             fs_importance = fs_importance + [w]*self.feature_split
     
         fs_importance = np.array(fs_importance)
 
         return biggest_fsse_fs, fs_importance
 
-def fsse_homo_stacking(X, y, create_base_estimator_cv, split_range = range(1, 20), repeat = 3, summary = 'median'):
+def fsse_homo_stacking(X, y, create_base_estimator_cv, split_range = range(1, 20), repeat = 3, summary = 'median', display = False):
 
-    accs = []
+    dic_accs = {}
     r = split_range
     N = repeat
 
     for split in r:
 
         for i in range(N):
 
             accs_repeat = []
 
             fsse = FSSE(create_base_estimator_cv, feature_split = split)
             fsse.fit(X, y)
             accs_repeat.append(fsse.evaluate(X, y))
 
         if summary == 'median':
-            accs.append( np.median(accs_repeat) )
+            dic_accs[split] = np.median(accs_repeat)
         else:
-            accs.append( np.mean(accs_repeat) ) # otherwise, mean
+            dic_accs[split] = np.mean(accs_repeat) # otherwise, mean
 
-    plt.figure(figsize = (12,3))
-    plt.scatter(r,accs)
-    plt.plot(r, accs)
-    plt.show()
+    if display:
+
+        plt.figure(figsize = (12,3))
+        plt.scatter(r, list(dic_accs.values()))
+        plt.plot(r, list(dic_accs.values()))
+        plt.show()
     
-    return accs
+    return dic_accs
 
 #endregion
```

### Comparing `pyNNRW-0.3.4/src/pyNNRW/rbfnn.py` & `pyNNRW-0.3.5/src/pyNNRW/rbfnn.py`

 * *Files identical despite different names*

### Comparing `pyNNRW-0.3.4/src/pyNNRW/rbm.py` & `pyNNRW-0.3.5/src/pyNNRW/rbm.py`

 * *Files identical despite different names*

### Comparing `pyNNRW-0.3.4/src/pyNNRW/rvfl.py` & `pyNNRW-0.3.5/src/pyNNRW/rvfl.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,16 @@
         beta: A Numpy array shape is [n_feature + n_nodes, n_class], the projection matrix.
         activation: A string of activation name.
         data_std: A list, store normalization parameters for each layer.
         data_mean: A list, store normalization parameters for each layer.
         same_feature: A bool, the true means all the features have same meaning and boundary for example: images.
         task_type: A string of ML task type, 'classification' or 'regression'.
     """
-    def __init__(self, n_nodes, lam, w_random_vec_range = [-1, 1], 
-                 b_random_vec_range = [0, 1], activation = 'sigmoid', 
+    def __init__(self, n_nodes, lam, w_random_vec_range = [-1, 1],
+                 b_random_vec_range = [0, 1], activation = 'sigmoid',
                  same_feature=False,
                  task_type='classification'):
         assert task_type in ['classification', 'regression'], 'task_type should be "classification" or "regression".'
         self.n_nodes = n_nodes
         self.lam = lam # controls the direct-link strength
         self.w_random_range = w_random_vec_range
         self.b_random_range = b_random_vec_range
@@ -229,15 +229,15 @@
     Reference: A new learning paradigm for random vector functional-link network: RVFL+. Neural Networks 122 (2020) pp.94-105
 
     Parameters
     ----------
     hidden_nodes : default 50, the number of enhancement node between the input layer and the hidden layer
     random_type :default = 'uniform', please select random type from "uniform" or "gaussian"
     activation_name : default = 'sigmoid', please select an activation function from the below set: {'sigmoid', 'tanh',
-                     'sin', 'hardlim', 'softlim', 'gaussianRBF', 'multiquadricRBF', 'inv_multiquadricRBF', 'tribas',
+                     'sine', 'hardlim', 'softlim', 'gaussianRBF', 'multiquadricRBF', 'inv_multiquadricRBF', 'tribas',
                        'inv_tribas'}
     type: default='classification', classification or regression
     Example
     --------
     model = RVFL()
     model.fit(train_x, train_y)
     y_hat = model.predict(test_x)
@@ -248,15 +248,15 @@
                  type="classification"):
 
         self.hidden_nodes = hidden_nodes
         self.random_type = random_type
         self.activation_name = activation_name
         self.type = type
         self._activation_dict = {'sigmoid': lambda x : 1.0 / (1.0 + np.exp(-x)),
-                                 "sin": lambda x: np.sin(x),
+                                 "sine": lambda x: np.sin(x),
                                  "tanh": lambda x: np.tanh(x),
                                  "hardlim": lambda x:np.array(x > 0.0, dtype=float),
                                  "softlim":lambda x:np.clip(x, 0.0, 1.0),
                                  "gaussianRBF": lambda x:np.exp(-pow(x, 2.0)),
                                  "multiquadricRBF": lambda x:np.sqrt(1.0 + pow(x, 2.0)),
                                  "inv_multiquadricRBF": lambda x : 1.0 / (np.sqrt(1.0 + pow(x, 2.0))),
                                  "tribas": lambda x: np.clip(1.0 - np.fabs(x), 0.0, 1.0),
@@ -403,22 +403,27 @@
     def evaluate(self, X, y, metrics=['loss', 'accuracy', 'precision', 'recall']):
         '''
         Return loss, accuracy, precision, recall by default
         '''
         return self.model.evaluate(X, y, metrics=metrics)
 
 class RVFLClassifierCV():
+    '''
+    Encapsulate RVFL as a sklearn estimator and use CV to optimize its hyper-parameters
+    '''
 
-    def __init__(self, hparams = {'n_hidden_nodes': [1, 10], 'activation': ['sigmoid', 'tanh', 'sin'] }):        
+    def __init__(self, hparams = {'n_hidden_nodes': [1, 10], 'activation': ['sigmoid', 'tanh', 'sine'] }):      
         '''
         parameters  
         ----------
         hparams : hyper-parameter candidate values to be grid-searched
         '''
         self.parameters =hparams
+        self.clf = None
+        self.classes_ = []
        
     def fit(self, X, y):
         rvflc = RVFLClassifier()
         self.clf = GridSearchCV(rvflc, self.parameters, scoring = 'accuracy') # 'neg_log_loss'
         self.clf.fit(X, y)
         # print( sorted(clf.cv_results_.keys()) )
         self.classes_ = np.unique(y)
```

### Comparing `pyNNRW-0.3.4/src/pyNNRW/wann.py` & `pyNNRW-0.3.5/src/pyNNRW/wann.py`

 * *Files identical despite different names*

### Comparing `pyNNRW-0.3.4/src/pyNNRW.egg-info/PKG-INFO` & `pyNNRW-0.3.5/src/pyNNRW.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyNNRW
-Version: 0.3.4
+Version: 0.3.5
 Summary: A Python library for NNRW (neural network with random weights)
 Home-page: https://github.com/zhangys11/pyNNRW
 Author: Yinsheng Zhang (Ph.D.)
 Author-email: oo@zju.edu.cn
 Project-URL: Bug Tracker, https://github.com/zhangys11/pyNNRW/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

