# Comparing `tmp/cro-0.0.5.1.tar.gz` & `tmp/cro-0.0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cro-0.0.5.1.tar", last modified: Fri Nov 12 11:24:05 2021, max compression
+gzip compressed data, was "dist\cro-0.0.5.2.tar", last modified: Fri Jul 14 09:41:17 2023, max compression
```

## Comparing `cro-0.0.5.1.tar` & `cro-0.0.5.2.tar`

### file list

```diff
@@ -1,28 +1,35 @@
-drwxrwxrwx   0        0        0        0 2021-11-12 11:24:05.000000 cro-0.0.5.1/
--rw-rw-rw-   0        0        0       51 2021-11-12 11:21:49.000000 cro-0.0.5.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1240 2021-11-12 11:24:05.000000 cro-0.0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0      243 2021-11-12 11:02:22.000000 cro-0.0.5.1/README.txt
-drwxrwxrwx   0        0        0        0 2021-11-12 11:24:05.000000 cro-0.0.5.1/cro/
--rw-rw-rw-   0        0        0     1365 2021-11-12 11:23:30.000000 cro-0.0.5.1/cro/__init__.py
-drwxrwxrwx   0        0        0        0 2021-11-12 11:24:05.000000 cro-0.0.5.1/cro/assets/
-drwxrwxrwx   0        0        0        0 2021-11-12 11:24:05.000000 cro-0.0.5.1/cro/assets/data/
--rw-rw-rw-   0        0        0  1068550 2021-11-12 11:02:22.000000 cro-0.0.5.1/cro/assets/data/voice.csv
--rw-rw-rw-   0        0        0    15502 2021-11-12 11:21:49.000000 cro-0.0.5.1/cro/cro.py
--rw-rw-rw-   0        0        0     1994 2021-11-12 11:02:22.000000 cro-0.0.5.1/cro/fitness.py
--rw-rw-rw-   0        0        0     3243 2021-11-12 11:02:22.000000 cro-0.0.5.1/cro/larvaemutation.py
--rw-rw-rw-   0        0        0     2955 2021-11-12 11:02:22.000000 cro-0.0.5.1/cro/reef_initialization.py
--rw-rw-rw-   0        0        0     1348 2021-11-12 11:02:22.000000 cro-0.0.5.1/cro/report.py
--rw-rw-rw-   0        0        0     1167 2021-11-12 11:21:49.000000 cro-0.0.5.1/cro/utils.py
-drwxrwxrwx   0        0        0        0 2021-11-12 11:24:05.000000 cro-0.0.5.1/cro.egg-info/
--rw-rw-rw-   0        0        0     1240 2021-11-12 11:24:05.000000 cro-0.0.5.1/cro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      415 2021-11-12 11:24:05.000000 cro-0.0.5.1/cro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-11-12 11:24:05.000000 cro-0.0.5.1/cro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2021-11-12 11:24:05.000000 cro-0.0.5.1/cro.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2021-11-12 11:24:05.000000 cro-0.0.5.1/cro.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2021-11-12 11:24:05.000000 cro-0.0.5.1/examples/
--rw-rw-rw-   0        0        0     1253 2021-11-12 11:02:22.000000 cro-0.0.5.1/examples/__init__.py
--rw-rw-rw-   0        0        0      231 2021-11-12 11:02:22.000000 cro-0.0.5.1/examples/context.py
--rw-rw-rw-   0        0        0     4729 2021-11-12 11:02:22.000000 cro-0.0.5.1/examples/example_advanced.py
--rw-rw-rw-   0        0        0     3155 2021-11-12 11:02:22.000000 cro-0.0.5.1/examples/example_basic.py
--rw-rw-rw-   0        0        0      115 2021-11-12 11:24:05.000000 cro-0.0.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1959 2021-11-12 11:21:49.000000 cro-0.0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:41:17.000000 cro-0.0.5.2/
+-rw-rw-rw-   0        0        0       51 2023-07-14 09:13:13.000000 cro-0.0.5.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1240 2023-07-14 09:41:17.000000 cro-0.0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2017-10-12 15:50:46.000000 cro-0.0.5.2/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 09:41:17.000000 cro-0.0.5.2/cro/
+-rw-rw-rw-   0        0        0     1365 2023-07-14 09:13:13.000000 cro-0.0.5.2/cro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:41:16.000000 cro-0.0.5.2/cro/assets/
+drwxrwxrwx   0        0        0        0 2023-07-14 09:41:17.000000 cro-0.0.5.2/cro/assets/data/
+-rw-rw-rw-   0        0        0  1068550 2017-10-12 15:50:46.000000 cro-0.0.5.2/cro/assets/data/voice.csv
+-rw-rw-rw-   0        0        0    15690 2023-07-14 09:13:13.000000 cro-0.0.5.2/cro/cro.py
+-rw-rw-rw-   0        0        0     1994 2023-07-14 08:54:33.000000 cro-0.0.5.2/cro/fitness.py
+-rw-rw-rw-   0        0        0     3243 2023-07-14 08:54:34.000000 cro-0.0.5.2/cro/larvaemutation.py
+-rw-rw-rw-   0        0        0     2955 2023-07-14 08:54:34.000000 cro-0.0.5.2/cro/reef_initialization.py
+-rw-rw-rw-   0        0        0     1348 2017-12-16 09:26:55.000000 cro-0.0.5.2/cro/report.py
+-rw-rw-rw-   0        0        0     1164 2023-07-14 09:18:49.000000 cro-0.0.5.2/cro/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:41:17.000000 cro-0.0.5.2/cro.egg-info/
+-rw-rw-rw-   0        0        0     1240 2023-07-14 09:41:16.000000 cro-0.0.5.2/cro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      677 2023-07-14 09:41:16.000000 cro-0.0.5.2/cro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 09:41:16.000000 cro-0.0.5.2/cro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-07-14 09:41:16.000000 cro-0.0.5.2/cro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-14 09:41:16.000000 cro-0.0.5.2/cro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 09:41:17.000000 cro-0.0.5.2/examples/
+drwxrwxrwx   0        0        0        0 2023-07-14 09:41:17.000000 cro-0.0.5.2/examples/.ipynb_checkpoints/
+-rw-rw-rw-   0        0        0   126818 2017-11-09 12:27:42.000000 cro-0.0.5.2/examples/.ipynb_checkpoints/cro_notebook_examples-checkpoint.ipynb
+-rw-rw-rw-   0        0        0     1253 2017-12-16 09:26:55.000000 cro-0.0.5.2/examples/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:41:17.000000 cro-0.0.5.2/examples/__pycache__/
+-rw-rw-rw-   0        0        0      232 2017-11-11 17:26:12.000000 cro-0.0.5.2/examples/__pycache__/__init__.cpython-36.pyc
+-rw-rw-rw-   0        0        0      313 2017-11-26 19:25:58.000000 cro-0.0.5.2/examples/__pycache__/context.cpython-36.pyc
+-rw-rw-rw-   0        0        0      317 2023-07-14 08:53:07.000000 cro-0.0.5.2/examples/__pycache__/context.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1210 2017-11-11 17:26:16.000000 cro-0.0.5.2/examples/__pycache__/test_example_basic.cpython-36-PYTEST.pyc
+-rw-rw-rw-   0        0        0      231 2017-11-26 17:14:27.000000 cro-0.0.5.2/examples/context.py
+-rw-rw-rw-   0        0        0     3622 2023-07-14 09:13:13.000000 cro-0.0.5.2/examples/example_advanced.py
+-rw-rw-rw-   0        0        0     3155 2023-07-14 08:54:34.000000 cro-0.0.5.2/examples/example_basic.py
+-rw-rw-rw-   0        0        0      115 2023-07-14 09:41:17.000000 cro-0.0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1959 2023-07-14 09:13:13.000000 cro-0.0.5.2/setup.py
```

### Comparing `cro-0.0.5.1/PKG-INFO` & `cro-0.0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: cro
-Version: 0.0.5.1
+Version: 0.0.5.2
 Summary: Coral Reef Optimization (CRO) Algorithm
 Home-page: https://github.com/VictorPelaez/coral-reef-optimization-algorithm
 Author: CRO Team
 Author-email: cro_developers@googlegroups.com
 License: MIT
 Description: Coral Reefs Optimization (CRO) algorithm artificially simulates a coral reef, where different corals (which are the solutions for the considered optimization problem) grow and reproduce in a coral-reef, fighting with other corals for space.
```

### Comparing `cro-0.0.5.1/cro/__init__.py` & `cro-0.0.5.2/cro/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 from .utils import *
 from .fitness import *
 from .larvaemutation import *
 
 __author__ = "CRO Team"
 __email__ = "cro_developers@googlegroups.com"
 # version must be in the last line 
-__version__ = "0.0.5.1"
+__version__ = "0.0.5.2"
```

### Comparing `cro-0.0.5.1/cro/assets/data/voice.csv` & `cro-0.0.5.2/cro/assets/data/voice.csv`

 * *Files identical despite different names*

### Comparing `cro-0.0.5.1/cro/cro.py` & `cro-0.0.5.2/cro/cro.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 #!/usr/bin/env python
 # coding=utf-8
 ###############################################################################
 from __future__ import division, print_function
 import sys
 import logging
+from multiprocess import Pool, cpu_count
+
 import numpy as np
 
 from .reef_initialization import get_reefinit_function
 from .larvaemutation import get_larvaemutation_function
 
 class CRO(object):
     def __init__(self, Ngen, N, M, Fb, Fa, Fd, r0, k, Pd, fitness_coral, opt, L=None,
-                 ke=0.2, npolyps=1, seed=None, mode='bin', param_grid={}, verbose=False):
+                 ke=0.2, npolyps=1, seed=None, mode='bin', param_grid={}, n_jobs=-1,
+                 verbose=False):
         
         # Set logging configuration
         logging_level = logging.INFO if verbose else logging.WARNING
         logging.basicConfig(stream=sys.stdout,
                             format="%(message)s")
         logging.getLogger().setLevel(logging_level)
 
@@ -33,14 +36,15 @@
         self.opt_multiplier = -1 if opt == "max" else 1
         self.L    = L                          
         self.ke   = ke
         self.npolyps = npolyps
         self.seed = seed
         self.mode = mode
         self.param_grid = param_grid
+        self.n_jobs = cpu_count() if n_jobs == -1 else max(int(n_jobs), 1) # at least 1
         self.verbose = verbose
 
         self.reefinit_function = get_reefinit_function(mode)
         self.larvaemutation_function = get_larvaemutation_function(mode)
         logging.info("Running Initialization: %s", self.opt) 
         
     def reefinitialization (self):   
@@ -61,18 +65,19 @@
         return REEF, REEFpob
 
     def fitness(self, REEFpob):
         """
         Description:
             This function calculates the health function for each coral in the reef
         """
-        REEF_fitness = []
-        for coral in REEFpob:
-            coral_fitness = self.fitness_coral(coral)
-            REEF_fitness.append(coral_fitness)
+        try:
+            p = self.parallel
+        except AttributeError:
+            p = self.parallel = Pool(self.n_jobs)
+        REEF_fitness = p.map(self.fitness_coral, REEFpob)
 
         return self.opt_multiplier*np.array(REEF_fitness)
 
     def broadcastspawning(self, REEF, REEFpob): 
         """
         Description:
             Create new larvae by external sexual reproduction. Cross-over operation
```

### Comparing `cro-0.0.5.1/cro/fitness.py` & `cro-0.0.5.2/cro/fitness.py`

 * *Files identical despite different names*

### Comparing `cro-0.0.5.1/cro/larvaemutation.py` & `cro-0.0.5.2/cro/larvaemutation.py`

 * *Files identical despite different names*

### Comparing `cro-0.0.5.1/cro/reef_initialization.py` & `cro-0.0.5.2/cro/reef_initialization.py`

 * *Files identical despite different names*

### Comparing `cro-0.0.5.1/cro/report.py` & `cro-0.0.5.2/cro/report.py`

 * *Files identical despite different names*

### Comparing `cro-0.0.5.1/cro/utils.py` & `cro-0.0.5.2/cro/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import numpy as np
 from sklearn.utils import Bunch
 
 # https://www.kaggle.com/adhok93/feature-importance-and-pca
 
 def load_data(name):
     # csv file
-    data = pd.read_csv('../cro/assets/data/' + name + '.csv')
+    data = pd.read_csv('cro/assets/data/' + name + '.csv')
     if name=='voice':
         data['label'] = data.label.apply(lambda x: 1 if x=='female' else 0) #one means female class
          
     feature_cols = [x for x in data.columns if (x!='label') & (x!='target')]
     
     # Add noisy features
     noisy_features = 10
```

### Comparing `cro-0.0.5.1/cro.egg-info/PKG-INFO` & `cro-0.0.5.2/cro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: cro
-Version: 0.0.5.1
+Version: 0.0.5.2
 Summary: Coral Reef Optimization (CRO) Algorithm
 Home-page: https://github.com/VictorPelaez/coral-reef-optimization-algorithm
 Author: CRO Team
 Author-email: cro_developers@googlegroups.com
 License: MIT
 Description: Coral Reefs Optimization (CRO) algorithm artificially simulates a coral reef, where different corals (which are the solutions for the considered optimization problem) grow and reproduce in a coral-reef, fighting with other corals for space.
```

### Comparing `cro-0.0.5.1/examples/__init__.py` & `cro-0.0.5.2/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `cro-0.0.5.1/examples/example_advanced.py` & `cro-0.0.5.2/examples/example_advanced.py`

 * *Files 26% similar despite different names*

```diff
@@ -73,31 +73,8 @@
     M  = 10                    # MxN: reef size
     Fb = 0.8                   # Broadcast prob.
     Fa = 0.2                   # Asexual reproduction prob.
     Fd = 0.1                   # Fraction of the corals to be eliminated in the depredation operator.
     r0 = 0.7                   # Free/total initial proportion
     k  = 3                     # Number of opportunities for a new coral to settle in the reef
     Pd = 0.1                   # Depredation prob.
-    opt= 'min'                 # flag: 'max' for maximizing and 'min' for minimizing
-    
-    ## ------------------------------------------------------
-    
-    dataset = datasets.load_boston()
-    L = dataset.data.shape[1] # number of features
-    X = dataset.data
-    y = dataset.target
-    
-    params = {'n_estimators': 60, 'max_depth': 4, 'min_samples_split': 2}
-    gbr = ensemble.GradientBoostingRegressor(**params)  
-    
-    fitness_coral = partial(feature_selection, X=X, y=y, model=gbr,
-                            get_prediction=lambda gbr, X: gbr.predict(X), 
-                            metric=mean_squared_error)
-    start = time.time()
-    cro = CRO(Ngen, N, M, Fb, Fa, Fd, r0, k, Pd, fitness_coral, opt, L, seed=13, verbose=True)
-    (REEF, REEFpob, REEFfitness, ind_best, Bestfitness, Meanfitness) = cro.fit(X, y, gbr)
-    print("Example II: feature selection, regression (min mse): ", time.time() - start, "seconds.")
-
-    plot_results(Bestfitness, Meanfitness, cro, filename=None)
-    
-    names = np.array(['CRIM', 'ZN', 'INDUS', 'CHAS', 'NOX', 'RM', 'AGE', 'DIS', 'RAD', 'TAX', 'PTRATIO', 'B', 'LSTAT'])
-    print(names[REEFpob[ind_best, :]>0])
+    opt= 'min'                 # flag: 'max' for maximizing and 'min' for minimizing
```

### Comparing `cro-0.0.5.1/examples/example_basic.py` & `cro-0.0.5.2/examples/example_basic.py`

 * *Files identical despite different names*

### Comparing `cro-0.0.5.1/setup.py` & `cro-0.0.5.2/setup.py`

 * *Files identical despite different names*

