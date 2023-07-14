# Comparing `tmp/mapel-marriages-2.0.5.tar.gz` & `tmp/mapel-marriages-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapel-marriages-2.0.5.tar", last modified: Fri May 26 20:07:11 2023, max compression
+gzip compressed data, was "mapel-marriages-2.0.6.tar", last modified: Fri Jul 14 09:02:55 2023, max compression
```

## Comparing `mapel-marriages-2.0.5.tar` & `mapel-marriages-2.0.6.tar`

### file list

```diff
@@ -1,40 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:07:11.298081 mapel-marriages-2.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-26 20:06:23.000000 mapel-marriages-2.0.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-26 20:07:11.298081 mapel-marriages-2.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-26 20:06:23.000000 mapel-marriages-2.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-26 20:06:23.000000 mapel-marriages-2.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 20:06:23.000000 mapel-marriages-2.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 20:07:11.298081 mapel-marriages-2.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:07:11.290081 mapel-marriages-2.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:07:11.290081 mapel-marriages-2.0.5/src/mapel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:07:11.290081 mapel-marriages-2.0.5/src/mapel/marriages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:23.000000 mapel-marriages-2.0.5/src/mapel/marriages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:07:11.294081 mapel-marriages-2.0.5/src/mapel/marriages/cultures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:23.000000 mapel-marriages-2.0.5/src/mapel/marriages/cultures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-26 20:06:23.000000 mapel-marriages-2.0.5/src/mapel/marriages/cultures/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16557 2023-05-26 20:06:23.000000 mapel-marriages-2.0.5/src/mapel/marriages/cultures/euclidean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-26 20:06:23.000000 mapel-marriages-2.0.5/src/mapel/marriages/cultures/impartial.py
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-05-26 20:06:23.000000 mapel-marriages-2.0.5/src/mapel/marriages/cultures/mallows.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-26 20:06:23.000000 mapel-marriages-2.0.5/src/mapel/marriages/cultures/urn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-26 20:06:23.000000 mapel-marriages-2.0.5/src/mapel/marriages/cultures_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:07:11.294081 mapel-marriages-2.0.5/src/mapel/marriages/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:23.000000 mapel-marriages-2.0.5/src/mapel/marriages/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9917 2023-05-26 20:06:23.000000 mapel-marriages-2.0.5/src/mapel/marriages/features/basic_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-05-26 20:06:23.000000 mapel-marriages-2.0.5/src/mapel/marriages/features/distance_to_stability_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-26 20:06:23.000000 mapel-marriages-2.0.5/src/mapel/marriages/features/experiments_marriage.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-26 20:06:23.000000 mapel-marriages-2.0.5/src/mapel/marriages/features_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:07:11.294081 mapel-marriages-2.0.5/src/mapel/marriages/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:23.000000 mapel-marriages-2.0.5/src/mapel/marriages/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-05-26 20:06:23.000000 mapel-marriages-2.0.5/src/mapel/marriages/metrics/main_marriages_distances.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-05-26 20:06:23.000000 mapel-marriages-2.0.5/src/mapel/marriages/metrics_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:07:11.294081 mapel-marriages-2.0.5/src/mapel/marriages/objects/
--rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-05-26 20:06:23.000000 mapel-marriages-2.0.5/src/mapel/marriages/objects/Marriages.py
--rw-r--r--   0 runner    (1001) docker     (123)    16617 2023-05-26 20:06:23.000000 mapel-marriages-2.0.5/src/mapel/marriages/objects/MarriagesExperiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-26 20:06:23.000000 mapel-marriages-2.0.5/src/mapel/marriages/objects/MarriagesFamily.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:23.000000 mapel-marriages-2.0.5/src/mapel/marriages/objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:07:11.298081 mapel-marriages-2.0.5/src/mapel_marriages.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-26 20:07:11.000000 mapel-marriages-2.0.5/src/mapel_marriages.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-26 20:07:11.000000 mapel-marriages-2.0.5/src/mapel_marriages.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 20:07:11.000000 mapel-marriages-2.0.5/src/mapel_marriages.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 20:07:11.000000 mapel-marriages-2.0.5/src/mapel_marriages.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 20:07:11.000000 mapel-marriages-2.0.5/src/mapel_marriages.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:55.349771 mapel-marriages-2.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-14 09:02:16.000000 mapel-marriages-2.0.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-07-14 09:02:55.349771 mapel-marriages-2.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-14 09:02:16.000000 mapel-marriages-2.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-14 09:02:16.000000 mapel-marriages-2.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 09:02:16.000000 mapel-marriages-2.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 09:02:55.349771 mapel-marriages-2.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:55.345771 mapel-marriages-2.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:55.341771 mapel-marriages-2.0.6/src/mapel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:55.345771 mapel-marriages-2.0.6/src/mapel/marriages/
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-14 09:02:16.000000 mapel-marriages-2.0.6/src/mapel/marriages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:55.345771 mapel-marriages-2.0.6/src/mapel/marriages/cultures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:16.000000 mapel-marriages-2.0.6/src/mapel/marriages/cultures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-14 09:02:16.000000 mapel-marriages-2.0.6/src/mapel/marriages/cultures/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-07-14 09:02:16.000000 mapel-marriages-2.0.6/src/mapel/marriages/cultures/euclidean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-07-14 09:02:16.000000 mapel-marriages-2.0.6/src/mapel/marriages/cultures/impartial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-14 09:02:16.000000 mapel-marriages-2.0.6/src/mapel/marriages/cultures/mallows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-14 09:02:16.000000 mapel-marriages-2.0.6/src/mapel/marriages/cultures/urn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-14 09:02:16.000000 mapel-marriages-2.0.6/src/mapel/marriages/cultures_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:55.345771 mapel-marriages-2.0.6/src/mapel/marriages/distances/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:16.000000 mapel-marriages-2.0.6/src/mapel/marriages/distances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-07-14 09:02:16.000000 mapel-marriages-2.0.6/src/mapel/marriages/distances/main_marriages_distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-07-14 09:02:16.000000 mapel-marriages-2.0.6/src/mapel/marriages/distances_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:55.345771 mapel-marriages-2.0.6/src/mapel/marriages/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:16.000000 mapel-marriages-2.0.6/src/mapel/marriages/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-07-14 09:02:16.000000 mapel-marriages-2.0.6/src/mapel/marriages/features/basic_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-07-14 09:02:16.000000 mapel-marriages-2.0.6/src/mapel/marriages/features/distance_to_stability_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-14 09:02:16.000000 mapel-marriages-2.0.6/src/mapel/marriages/features/experiments_marriage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-14 09:02:16.000000 mapel-marriages-2.0.6/src/mapel/marriages/features_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:55.345771 mapel-marriages-2.0.6/src/mapel/marriages/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-07-14 09:02:16.000000 mapel-marriages-2.0.6/src/mapel/marriages/objects/Marriages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15855 2023-07-14 09:02:16.000000 mapel-marriages-2.0.6/src/mapel/marriages/objects/MarriagesExperiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-14 09:02:16.000000 mapel-marriages-2.0.6/src/mapel/marriages/objects/MarriagesFamily.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:16.000000 mapel-marriages-2.0.6/src/mapel/marriages/objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:55.345771 mapel-marriages-2.0.6/src/mapel/marriages/persistence/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:16.000000 mapel-marriages-2.0.6/src/mapel/marriages/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-14 09:02:16.000000 mapel-marriages-2.0.6/src/mapel/marriages/persistence/instance_exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-14 09:02:16.000000 mapel-marriages-2.0.6/src/mapel/marriages/persistence/instance_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:55.349771 mapel-marriages-2.0.6/src/mapel_marriages.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-07-14 09:02:55.000000 mapel-marriages-2.0.6/src/mapel_marriages.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-14 09:02:55.000000 mapel-marriages-2.0.6/src/mapel_marriages.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 09:02:55.000000 mapel-marriages-2.0.6/src/mapel_marriages.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 09:02:55.000000 mapel-marriages-2.0.6/src/mapel_marriages.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 09:02:55.000000 mapel-marriages-2.0.6/src/mapel_marriages.egg-info/top_level.txt
```

### Comparing `mapel-marriages-2.0.5/LICENSE.txt` & `mapel-marriages-2.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.5/PKG-INFO` & `mapel-marriages-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-marriages
-Version: 2.0.5
+Version: 2.0.6
 Summary: Map of Marriages
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>
 License: Copyright (c) 2018-2022 Stanislaw Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-marriages-2.0.5/README.md` & `mapel-marriages-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.5/pyproject.toml` & `mapel-marriages-2.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65", "wheel", "pybind11>=2.6.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mapel-marriages"
-version = "2.0.5"
+version = "2.0.6"
 authors = [
  {name = "Stanislaw Szufa", email = "s.szufa@gmail.com"},
  {name = "Niclas Boehmer", email = "niclas.boehmer@tu-berlin.de"},
 ]
 description = "Map of Marriages"
 classifiers=[
     "Programming Language :: Python :: 3",
```

### Comparing `mapel-marriages-2.0.5/src/mapel/marriages/cultures/euclidean.py` & `mapel-marriages-2.0.6/src/mapel/marriages/cultures/euclidean.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,89 +1,96 @@
 import numpy as np
 import math
 from numpy import linalg
 from mapel.marriages.cultures.mallows import mallows_votes
 
+
 ################################################################
 
 def get_range(params):
     if params['p_dist'] == 'beta':
         return np.random.beta(params['a'], params['b'])
     elif params['p_dist'] == 'uniform':
         return np.random.uniform(low=params['a'], high=params['b'])
 
+
 def weighted_l1(a1, a2, w):
     total = 0
     for i in range(len(a1)):
-        total += abs(a1[i]-a2[i])*w[i]
+        total += abs(a1[i] - a2[i]) * w[i]
     return total
 
-def generate_euclidean_votes(num_agents: int = None, params: dict = None):
 
-    name = f'{params["dim"]}d_{params["space"]}'
+def generate_euclidean_votes(num_agents: int = None,
+                             dim=2,
+                             space='uniform',
+                             **kwargs):
+    name = f'{dim}d_{space}'
 
     left = np.array([get_rand(name, i=i, num_agents=num_agents) for i in range(num_agents)])
     right = np.array([get_rand(name, i=i, num_agents=num_agents) for i in range(num_agents)])
 
     left_votes = np.zeros([num_agents, num_agents], dtype=int)
     right_votes = np.zeros([num_agents, num_agents], dtype=int)
     distances = np.zeros([num_agents, num_agents], dtype=float)
 
     for v in range(num_agents):
         for c in range(num_agents):
-
             left_votes[v][c] = c
             distances[v][c] = np.linalg.norm(left[v] - right[c])
         left_votes[v] = [x for _, x in sorted(zip(distances[v], left_votes[v]))]
 
     for v in range(num_agents):
         for c in range(num_agents):
-
             right_votes[v][c] = c
             distances[v][c] = np.linalg.norm(right[v] - left[c])
         right_votes[v] = [x for _, x in sorted(zip(distances[v], right_votes[v]))]
 
     return [left_votes, right_votes]
 
 
-def generate_mallows_euclidean_votes(num_agents: int = None, params: dict = None):
-    print(params)
-
-    name = f'{params["dim"]}d_{params["space"]}'
+def generate_mallows_euclidean_votes(num_agents: int = None,
+                                     dim=2,
+                                     space='uniform',
+                                     phi=0.5,
+                                     **kwargs):
+    name = f'{dim}d_{space}'
 
     left = np.array([get_rand(name, i=i, num_agents=num_agents) for i in range(num_agents)])
     right = np.array([get_rand(name, i=i, num_agents=num_agents) for i in range(num_agents)])
 
     left_votes = np.zeros([num_agents, num_agents], dtype=int)
     right_votes = np.zeros([num_agents, num_agents], dtype=int)
     distances = np.zeros([num_agents, num_agents], dtype=float)
 
     for v in range(num_agents):
         for c in range(num_agents):
-
             left_votes[v][c] = c
             distances[v][c] = np.linalg.norm(left[v] - right[c])
         left_votes[v] = [x for _, x in sorted(zip(distances[v], left_votes[v]))]
 
     for v in range(num_agents):
         for c in range(num_agents):
-
             right_votes[v][c] = c
             distances[v][c] = np.linalg.norm(right[v] - left[c])
         right_votes[v] = [x for _, x in sorted(zip(distances[v], right_votes[v]))]
 
-    left_votes = mallows_votes(left_votes, params['phi'])
-    right_votes = mallows_votes(right_votes, params['phi'])
+    left_votes = mallows_votes(left_votes, phi)
+    right_votes = mallows_votes(right_votes, phi)
 
     return [left_votes, right_votes]
 
 
-def generate_reverse_euclidean_votes(num_agents: int = None, params: dict = None):
-
-    name = f'{params["dim"]}d_{params["space"]}'
+def generate_reverse_euclidean_votes(num_agents: int = None,
+                                     dim=2,
+                                     space='uniform',
+                                     phi=0.5,
+                                    proportion: float = 0.5,
+                                     **kwargs):
+    name = f'{dim}d_{space}'
 
     left = np.array([get_rand(name, i=i, num_agents=num_agents) for i in range(num_agents)])
     right = np.array([get_rand(name, i=i, num_agents=num_agents) for i in range(num_agents)])
 
     left_votes = np.zeros([num_agents, num_agents], dtype=int)
     right_votes = np.zeros([num_agents, num_agents], dtype=int)
     distances = np.zeros([num_agents, num_agents], dtype=float)
@@ -96,251 +103,251 @@
 
     for v in range(num_agents):
         for c in range(num_agents):
             right_votes[v][c] = c
             distances[v][c] = np.linalg.norm(right[v] - left[c])
         right_votes[v] = [x for _, x in sorted(zip(distances[v], right_votes[v]))]
 
-    if 'proportion' in params:
-        p = params['proportion']
-    else:
-        p = 0.5
-
-    for i in range(int(num_agents * (1.-p))):
+    p = proportion
+    for i in range(int(num_agents * (1. - p))):
         tmp = list(left_votes[i])
         tmp.reverse()
         left_votes[i] = tmp
 
         tmp = list(right_votes[i])
         tmp.reverse()
         right_votes[i] = tmp
 
     return [left_votes, right_votes]
 
 
-def generate_expectation_votes(num_agents: int = None, params: dict = None):
-    name = f'{params["dim"]}d_{params["space"]}'
+def generate_expectation_votes(num_agents: int = None,
+                               dim=2,
+                               space='uniform',
+                               std=0.1,
+                               phi=0.5,
+                               **kwargs):
+    name = f'{dim}d_{space}'
 
     left_agents_reality = np.array([get_rand(name) for _ in range(num_agents)])
     left_agents_wishes = np.zeros([num_agents, 2])
 
     right_agents_reality = np.array([get_rand(name) for _ in range(num_agents)])
     right_agents_wishes = np.zeros([num_agents, 2])
 
     for v in range(num_agents):
         # while agents_wishes[v][0] <= 0 or agents_wishes[v][0] >= 1:
-        left_agents_wishes[v][0] = np.random.normal(left_agents_reality[v][0], params['std'])
+        left_agents_wishes[v][0] = np.random.normal(left_agents_reality[v][0], std)
         # while agents_wishes[v][1] <= 0 or agents_wishes[v][1] >= 1:
-        left_agents_wishes[v][1] = np.random.normal(left_agents_reality[v][1], params['std'])
+        left_agents_wishes[v][1] = np.random.normal(left_agents_reality[v][1], std)
 
         # while agents_wishes[v][0] <= 0 or agents_wishes[v][0] >= 1:
-        right_agents_wishes[v][0] = np.random.normal(right_agents_reality[v][0], params['std'])
+        right_agents_wishes[v][0] = np.random.normal(right_agents_reality[v][0], std)
         # while agents_wishes[v][1] <= 0 or agents_wishes[v][1] >= 1:
-        right_agents_wishes[v][1] = np.random.normal(right_agents_reality[v][1], params['std'])
+        right_agents_wishes[v][1] = np.random.normal(right_agents_reality[v][1], std)
 
     left_votes = np.zeros([num_agents, num_agents], dtype=int)
     right_votes = np.zeros([num_agents, num_agents], dtype=int)
     distances = np.zeros([num_agents, num_agents], dtype=float)
 
     for v in range(num_agents):
         for c in range(num_agents):
-
             left_votes[v][c] = c
             distances[v][c] = np.linalg.norm(right_agents_reality[c] - left_agents_wishes[v])
         left_votes[v] = [x for _, x in sorted(zip(distances[v], left_votes[v]))]
 
     for v in range(num_agents):
         for c in range(num_agents):
-
             right_votes[v][c] = c
             distances[v][c] = np.linalg.norm(left_agents_reality[c] - right_agents_wishes[v])
         right_votes[v] = [x for _, x in sorted(zip(distances[v], right_votes[v]))]
 
     return [left_votes, right_votes]
 
 
-def generate_fame_votes(num_agents: int = None, params: dict = None):
-    name = f'{params["dim"]}d_{params["space"]}'
+def generate_fame_votes(num_agents: int = None,
+                        dim=2,
+                        space='uniform',
+                        radius=0.1,
+                        **kwargs):
+
+    name = f'{dim}d_{space}'
 
     left = np.array([get_rand(name, i=i, num_agents=num_agents) for i in range(num_agents)])
     right = np.array([get_rand(name, i=i, num_agents=num_agents) for i in range(num_agents)])
 
-    left_rays = np.array([np.random.uniform(0, params['radius']) for _ in range(num_agents)])
-    right_rays = np.array([np.random.uniform(0, params['radius']) for _ in range(num_agents)])
+    left_rays = np.array([np.random.uniform(0, radius) for _ in range(num_agents)])
+    right_rays = np.array([np.random.uniform(0, radius) for _ in range(num_agents)])
 
     left_votes = np.zeros([num_agents, num_agents], dtype=int)
     right_votes = np.zeros([num_agents, num_agents], dtype=int)
     distances = np.zeros([num_agents, num_agents], dtype=float)
 
     for v in range(num_agents):
         for c in range(num_agents):
-
             left_votes[v][c] = c
             distances[v][c] = np.linalg.norm(left[v] - right[c])
             distances[v][c] = distances[v][c] - right_rays[c]
         left_votes[v] = [x for _, x in sorted(zip(distances[v], left_votes[v]))]
 
     for v in range(num_agents):
         for c in range(num_agents):
-
             right_votes[v][c] = c
             distances[v][c] = np.linalg.norm(right[v] - left[c])
             distances[v][c] = distances[v][c] - left_rays[c]
         right_votes[v] = [x for _, x in sorted(zip(distances[v], right_votes[v]))]
 
     return [left_votes, right_votes]
 
 
-def generate_attributes_votes(num_agents: int = None, params: dict = None):
-    name = f'{params["dim"]}d_{params["space"]}'
+def generate_attributes_votes(num_agents: int = None,
+                              dim: int = 2,
+                              space: str = 'uniform',
+                              **kwargs):
+    name = f'{dim}d_{space}'
 
     left_agents_skills = np.array([get_rand(name) for _ in range(num_agents)])
     left_agents_weights = np.array([get_rand(name) for _ in range(num_agents)])
     right_agents_skills = np.array([get_rand(name) for _ in range(num_agents)])
     right_agents_weights = np.array([get_rand(name) for _ in range(num_agents)])
 
     votes = np.zeros([num_agents, num_agents], dtype=int)
     left_votes = np.zeros([num_agents, num_agents], dtype=int)
     right_votes = np.zeros([num_agents, num_agents], dtype=int)
     distances = np.zeros([num_agents, num_agents], dtype=float)
-    ones = np.ones([params["dim"]], dtype=float)
+    ones = np.ones([dim], dtype=float)
 
     for v in range(num_agents):
         for c in range(num_agents):
             left_votes[v][c] = c
-            if params["dim"] == 1:
+            if dim == 1:
                 distances[v][c] = (1. - right_agents_skills[c]) * left_agents_weights[v]
             else:
                 distances[v][c] = weighted_l1(ones, right_agents_skills[c], left_agents_weights[v])
         left_votes[v] = [x for _, x in sorted(zip(distances[v], left_votes[v]))]
 
     for v in range(num_agents):
         for c in range(num_agents):
             right_votes[v][c] = c
-            if params["dim"] == 1:
+            if dim == 1:
                 distances[v][c] = (1. - left_agents_skills[c]) * right_agents_weights[v]
             else:
                 distances[v][c] = weighted_l1(ones, left_agents_skills[c], right_agents_weights[v])
         right_votes[v] = [x for _, x in sorted(zip(distances[v], right_votes[v]))]
 
     return [left_votes, right_votes]
 
 
 #################
 def generate_roommates_radius_votes(num_agents: int = None, params: dict = None):
-
     dim = params['dim']
 
     name = f'{dim}d_{params["space"]}'
 
     agents = np.array([get_rand(name) for _ in range(num_agents)])
 
     votes = np.zeros([num_agents, num_agents], dtype=int)
     distances = np.zeros([num_agents, num_agents], dtype=float)
 
-    rays = np.array([np.random.random()/2. for _ in range(num_agents)])
+    rays = np.array([np.random.random() / 2. for _ in range(num_agents)])
 
     # a_power = np.array([get_range(params) for _ in range(num_agents)])
 
     for v in range(num_agents):
         for c in range(num_agents):
-
             # if v_range[v] + c_range[c] >= np.linalg.norm(voters[v] - candidates[c]):
             #     votes[v].add(c)
             votes[v][c] = c
             distances[v][c] = np.linalg.norm(agents[v] - agents[c])
             distances[v][c] = abs(distances[v][c] - rays[c])
         votes[v] = [x for _, x in sorted(zip(distances[v], votes[v]))]
 
     return convert(votes)
 
 
-
-
 def generate_roommates_double_votes(num_agents: int = None, params: dict = None):
-
     dim = params['dim']
 
     name = f'{dim}d_{params["space"]}'
 
     agents_reality = np.array([get_rand(name) for _ in range(num_agents)])
     agents_wishes = np.array([get_rand(name) for _ in range(num_agents)])
 
     for v in range(num_agents):
-        agents_wishes[v][0] = agents_reality[v][0] + (agents_wishes[v][0]-0.5)*1.
-        agents_wishes[v][1] = agents_reality[v][1] + (agents_wishes[v][1]-0.5)*1.
+        agents_wishes[v][0] = agents_reality[v][0] + (agents_wishes[v][0] - 0.5) * 1.
+        agents_wishes[v][1] = agents_reality[v][1] + (agents_wishes[v][1] - 0.5) * 1.
 
     votes = np.zeros([num_agents, num_agents], dtype=int)
     distances = np.zeros([num_agents, num_agents], dtype=float)
 
     for v in range(num_agents):
         for c in range(num_agents):
-
             votes[v][c] = c
             distances[v][c] = np.linalg.norm(agents_reality[v] - agents_wishes[c])
         votes[v] = [x for _, x in sorted(zip(distances[v], votes[v]))]
 
     return convert(votes)
 
 
 def generate_roommates_mallows_euclidean_votes(num_agents: int = None, params: dict = None):
-
     name = f'{params["dim"]}d_{params["space"]}'
     # print(name)
 
     agents = np.array([get_rand(name, i=i, num_agents=num_agents) for i in range(num_agents)])
 
     votes = np.zeros([num_agents, num_agents], dtype=int)
     distances = np.zeros([num_agents, num_agents], dtype=float)
 
     # a_power = np.array([get_range(params) for _ in range(num_agents)])
 
     for v in range(num_agents):
         for c in range(num_agents):
-
             # if v_range[v] + c_range[c] >= np.linalg.norm(voters[v] - candidates[c]):
             #     votes[v].add(c)
             votes[v][c] = c
             distances[v][c] = np.linalg.norm(agents[v] - agents[c])
         votes[v] = [x for _, x in sorted(zip(distances[v], votes[v]))]
 
     votes = mallows_votes(votes, 0.05)
 
     return convert(votes)
 
+
 # AUXILIARY
 def random_ball(dimension, num_points=1, radius=1):
     random_directions = np.random.normal(size=(dimension, num_points))
     random_directions /= linalg.norm(random_directions, axis=0)
     random_radii = np.random.random(num_points) ** (1 / dimension)
     return radius * (random_directions * random_radii).T
 
 
 GEN_CTR = 0
 
+
 def get_rand(model: str, i: int = 0, num_agents: int = 0, cat: str = "voters") -> list:
     """ generate random values"""
     # print(model ==  "1d_uniform")
 
     point = [0]
-    if model in {"1d_uniform",  "1d_interval"}:
+    if model in {"1d_uniform", "1d_interval"}:
         return np.random.rand()
     elif model in {'1d_asymmetric'}:
         if np.random.rand() < 0.3:
             return np.random.normal(loc=0.25, scale=0.15, size=1)
         else:
             return np.random.normal(loc=0.75, scale=0.15, size=1)
     elif model in {"1d_gaussian"}:
         point = np.random.normal(0.5, 0.15)
         while point > 1 or point < 0:
             point = np.random.normal(0.5, 0.15)
     elif model == "1d_one_sided_triangle":
         point = np.random.uniform(0, 1) ** 0.5
     elif model == "1d_full_triangle":
-        point = np.random.choice([np.random.uniform(0, 1) ** 0.5, 2 - np.random.uniform(0, 1) ** 0.5])
+        point = np.random.choice(
+            [np.random.uniform(0, 1) ** 0.5, 2 - np.random.uniform(0, 1) ** 0.5])
     elif model == "1d_two_party":
         point = np.random.choice([np.random.uniform(0, 1), np.random.uniform(2, 3)])
     elif model in {"2d_disc", "2d_range_disc"}:
         phi = 2.0 * 180.0 * np.random.random()
         radius = math.sqrt(np.random.random()) * 0.5
         point = [0.5 + radius * math.cos(phi), 0.5 + radius * math.sin(phi)]
     elif model == "2d_range_overlapping":
@@ -401,22 +408,22 @@
     elif model == "4d_cube":
         dim = 4
         point = [np.random.random() for _ in range(dim)]
     elif model == "5d_cube":
         dim = 5
         point = [np.random.random() for _ in range(dim)]
     elif model == '1d_extreme':
-        if i%2 == 1:
+        if i % 2 == 1:
             i -= 0.1
         point = i
     elif model == '2d_extreme':
         if i % 2 == 1:
-            alpha = 2 * math.pi * ((i-np.random.random()/100) / num_agents)
+            alpha = 2 * math.pi * ((i - np.random.random() / 100) / num_agents)
         else:
-            alpha = 2 * math.pi * ((i+np.random.random()/100) / num_agents)
+            alpha = 2 * math.pi * ((i + np.random.random() / 100) / num_agents)
         x = 1. * math.cos(alpha)
         y = 1. * math.sin(alpha)
         point = [x, y]
     else:
         print('unknown culture_id', model)
         point = [0, 0]
     return point
```

### Comparing `mapel-marriages-2.0.5/src/mapel/marriages/cultures/impartial.py` & `mapel-marriages-2.0.6/src/mapel/marriages/cultures/impartial.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,67 +1,48 @@
 import numpy as np
 
 
-def generate_ic_votes(num_agents: int = None, params=None):
+def generate_ic_votes(num_agents: int = None, **kwargs):
 
     return [list(np.random.permutation(num_agents)) for _ in range(num_agents)]
 
 
-def generate_id_votes(num_agents: int = None, params=None):
+def generate_id_votes(num_agents: int = None, **kwargs):
 
     return [list(range(num_agents)) for _ in range(num_agents)]
 
 
-def generate_asymmetric_votes(num_agents: int = None, params=None):
+def generate_asymmetric_votes(num_agents: int = None, **kwargs):
     votes = [list(range(num_agents)) for _ in range(num_agents)]
     votes_left = [rotate(vote, shift+1) for shift, vote in enumerate(votes)]
     votes = [list(range(num_agents)) for _ in range(num_agents)]
     votes_right = [rotate(vote, shift) for shift, vote in enumerate(votes)]
     return [votes_left, votes_right]
 
 
-def generate_group_ic_votes(num_agents: int = None, params: dict = None):
+def generate_group_ic_votes(num_agents: int = None, proportion: int = 0.5, **kwargs):
     """ Impartial Culture with two groups """
 
-    if 'proportion' not in params:
-        params['proportion'] = 0.5
-
-    size_1 = int(params['proportion'] * num_agents)
+    size_1 = int(proportion * num_agents)
     size_2 = int(num_agents - size_1)
 
     votes_1 = [list(np.random.permutation(size_1)) +
                list(np.random.permutation([j for j in range(size_1, num_agents)]))
                for _ in range(size_1)]
 
     votes_2 = [list(np.random.permutation([j for j in range(size_1, num_agents)])) +
                list(np.random.permutation(size_1))
                for _ in range(size_2)]
 
     votes = votes_1 + votes_2
 
     return votes
 
-# def generate_ic__id_votes(num_agents: int = None, params=None):
-#
-#     votes_1 = [list(np.random.permutation(num_agents)) for _ in range(num_agents)]
-#     votes_2 = [list(range(num_agents)) for _ in range(num_agents)]
-#
-#     return [votes_1, votes_2]
-#
-#
-# def generate_asymmetric__id_votes(num_agents: int = None, params=None):
-#     votes = [list(range(num_agents)) for _ in range(num_agents)]
-#
-#     votes_1 = [rotate(vote, is_shifted) for is_shifted, vote in enumerate(votes)]
-#     votes_2 = [list(range(num_agents)) for _ in range(num_agents)]
-#
-#     return [votes_1, votes_2]
-
 
-def generate_symmetric_votes(num_agents: int = None, params=None):
+def generate_symmetric_votes(num_agents: int = None, **kwargs):
 
     num_rounds = num_agents - 1
 
     def next(agents):
         first = agents[0]
         last = agents[-1]
         middle = agents[1:-1]
```

### Comparing `mapel-marriages-2.0.5/src/mapel/marriages/cultures_.py` & `mapel-marriages-2.0.6/src/mapel/marriages/cultures_.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 
 import mapel.marriages.cultures.euclidean as euclidean
 import mapel.marriages.cultures.impartial as impartial
 import mapel.marriages.cultures.mallows as mallows
 import mapel.marriages.cultures.urn as urn
 
 
-def generate_votes(model_id: str = None, num_agents: int = None,
+def generate_votes(culture_id: str = None,
+                   num_agents: int = None,
                    params: dict = None) -> Union[list, np.ndarray]:
     independent_models = {
         'ic': impartial.generate_ic_votes,
         'id': impartial.generate_id_votes,
         'symmetric': impartial.generate_symmetric_votes,
         'norm-mallows': mallows.generate_norm_mallows_votes,
         'urn': urn.generate_urn_votes,
@@ -27,22 +28,22 @@
         'reverse_euclidean': euclidean.generate_reverse_euclidean_votes,
         'mallows_euclidean': euclidean.generate_mallows_euclidean_votes,
         'expectation': euclidean.generate_expectation_votes,
         'attributes': euclidean.generate_attributes_votes,
         'fame': euclidean.generate_fame_votes,
     }
 
-    if model_id in independent_models:
-        votes_1 = independent_models.get(model_id)(num_agents=num_agents, params=params)
-        votes_2 = independent_models.get(model_id)(num_agents=num_agents, params=params)
+    if culture_id in independent_models:
+        votes_1 = independent_models.get(culture_id)(num_agents=num_agents, **params)
+        votes_2 = independent_models.get(culture_id)(num_agents=num_agents, **params)
         return [votes_1, votes_2]
 
-    elif model_id in dependent_models:
-        return dependent_models.get(model_id)(num_agents=num_agents, params=params)
+    elif culture_id in dependent_models:
+        return dependent_models.get(culture_id)(num_agents=num_agents, **params)
 
     else:
-        logging.warning(f'No such model id: {model_id}')
+        logging.warning(f'No such culture id: {culture_id}')
         return []
 
 # # # # # # # # # # # # # # # #
 # LAST CLEANUP ON: 22.10.2021 #
 # # # # # # # # # # # # # # # #
```

### Comparing `mapel-marriages-2.0.5/src/mapel/marriages/features/basic_features.py` & `mapel-marriages-2.0.6/src/mapel/marriages/features/basic_features.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 import gurobipy as gp
 from gurobipy import GRB
-# from mapel.roommates.matching.games import StableRoommates
-try:
-    from mapel.roommates.matching.games import StableRoommates
-except:
-    pass
+
 
 from random import shuffle
 import statistics
 import warnings
 import sys
 import time
 import networkx as nx
@@ -36,30 +32,14 @@
                 partnerj_index = instance[j].index(partner_j)
                 if instance[i].index(j)<partneri_index:
                     if instance[j].index(i) < partnerj_index:
                         bps+=1
     return bps
 
 
-def compute_stable_SR(votes):
-    dict_instance={}
-    num_agents=len(votes)
-    for i in range(num_agents):
-        dict_instance[i]=votes[i]
-    game = StableRoommates.create_from_dictionary(dict_instance)
-    try:
-        matching = game.solve()
-        usable_matching = {}
-        for m in matching:
-            usable_matching[m.name] = matching[m].name
-        return usable_matching
-    except:
-        return None
-
-
 
 def spear_distance(instance1,instance2):
     num_agents=len(instance1)
     m = gp.Model("qp")
     #m.setParam('Threads', 6)
     #m.setParam('OutputFlag', False)
     x = m.addVars(num_agents, num_agents, lb=0, ub=1, vtype=GRB.BINARY)
```

### Comparing `mapel-marriages-2.0.5/src/mapel/marriages/features/distance_to_stability_features.py` & `mapel-marriages-2.0.6/src/mapel/marriages/features/distance_to_stability_features.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.5/src/mapel/marriages/features/experiments_marriage.py` & `mapel-marriages-2.0.6/src/mapel/marriages/features/experiments_marriage.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.5/src/mapel/marriages/features_.py` & `mapel-marriages-2.0.6/src/mapel/marriages/features_.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.5/src/mapel/marriages/metrics/main_marriages_distances.py` & `mapel-marriages-2.0.6/src/mapel/marriages/distances/main_marriages_distances.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,20 +14,20 @@
         cost_table_1, cost_table_2 = get_matching_cost_retrospective(
             instance_1, instance_2, inner_distance, crossing=crossing)
 
         a, _ = solve_matching_vectors(cost_table_1)
         b, _ = solve_matching_vectors(cost_table_2)
         results.append(a+b)
 
-    return min(results)
+    return min(results), None
 
 
 def compute_positionwise_distance(instance_1, instance_2, inner_distance):
     cost_table = get_matching_cost_positionwise(instance_1, instance_2, inner_distance)
-    return solve_matching_vectors(cost_table)
+    return solve_matching_vectors(cost_table), None
 
 
 def compute_pos_swap_distance(instance_1: Marriages, instance_2: Marriages,
                               inner_distance: Callable) -> (float, list):
     """ Compute Positionwise distance between ordinal elections """
     cost_table = get_matching_cost_positionwise(instance_1, instance_2, inner_distance)
     obj_val, matching = solve_matching_vectors(cost_table)
```

### Comparing `mapel-marriages-2.0.5/src/mapel/marriages/metrics_.py` & `mapel-marriages-2.0.6/src/mapel/marriages/distances_.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 import copy
 import os
 import csv
 import numpy as np
 
 from mapel.core.inner_distances import map_str_to_func
 from mapel.core.objects.Experiment import Experiment
-from mapel.marriages.metrics import main_marriages_distances as mrd
+from mapel.marriages.distances import main_marriages_distances as mrd
 from mapel.marriages.objects.Marriages import Marriages
 
 
 def get_distance(election_1: Marriages, election_2: Marriages,
-                 distance_id: str = None) -> float or (float, list):
+                 distance_id: str = None) -> (float, list):
     """ Return: distance between ordinal elections, (if applicable) optimal matching """
     inner_distance, main_distance = extract_distance_id(distance_id)
 
     metrics_without_params = {
 
     }
```

### Comparing `mapel-marriages-2.0.5/src/mapel/marriages/objects/MarriagesExperiment.py` & `mapel-marriages-2.0.6/src/mapel/marriages/objects/MarriagesExperiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/usr/bin/env python
 import ast
-import copy
 import csv
 import itertools
 import os
 from multiprocessing import Process
 from time import sleep
 
 from mapel.core.objects.Experiment import Experiment
 from mapel.marriages.objects.MarriagesFamily import MarriagesFamily
 from mapel.marriages.objects.Marriages import Marriages
-import mapel.marriages.models_main as models_main
-import mapel.marriages.metrics_main as metr
+import mapel.marriages.distances as metr
 import mapel.marriages.features.basic_features as basic
-import mapel.marriages.features_main as features
-from mapel.core.printing import get_values_from_csv_file
+import mapel.marriages.features as features
+from mapel.core.persistence.experiment_imports import get_values_from_csv_file
 from mapel.core.utils import make_folder_if_do_not_exist
+import mapel.core.persistence.experiment_exports as exports
+
 try:
     from sklearn.manifold import MDS
     from sklearn.manifold import TSNE
     from sklearn.manifold import SpectralEmbedding
     from sklearn.manifold import LocallyLinearEmbedding
     from sklearn.manifold import Isomap
 except ImportError as error:
@@ -145,34 +145,20 @@
 
                     for row in reader:
                         distances[row['instance_id_1']][row['instance_id_2']] = float(
                             row['distance'])
                         times[row['instance_id_1']][row['instance_id_2']] = float(row['time'])
 
         if self.is_exported:
-            self._store_distances_to_file(distance_id, distances, times)
+            exports.export_distances_to_file(self, distance_id, distances, times)
 
         self.distances = distances
         self.times = times
         self.matchings = matchings
 
-    def _store_distances_to_file(self, distance_id, distances, times):
-        path_to_folder = os.path.join(os.getcwd(), "election", self.experiment_id, "distances")
-        make_folder_if_do_not_exist(path_to_folder)
-        path_to_file = os.path.join(path_to_folder, f'{distance_id}.csv')
-
-        with open(path_to_file, 'w', newline='') as csv_file:
-            writer = csv.writer(csv_file, delimiter=';')
-            writer.writerow(["instance_id_1", "instance_id_2", "distance", "time"])
-
-            for election_1, election_2 in itertools.combinations(self.instances, 2):
-                distance = str(distances[election_1][election_2])
-                time_ = str(times[election_1][election_2])
-                writer.writerow([election_1, election_2, distance, time_])
-
     def import_controllers(self):
         """ Import controllers from a file """
 
         families = {}
 
         path = os.path.join(os.getcwd(), 'election', self.experiment_id, 'map.csv')
         file_ = open(path, 'r')
```

### Comparing `mapel-marriages-2.0.5/src/mapel/marriages/objects/MarriagesFamily.py` & `mapel-marriages-2.0.6/src/mapel/marriages/objects/MarriagesFamily.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,16 +89,16 @@
                                                         relphi=params['norm-phi'])
 
             if self.single:
                 instance_id = self.family_id
             else:
                 instance_id = self.family_id + '_' + str(j)
 
-            instance = Marriages(experiment_id, instance_id, _import=False,
-                                 model_id=self.model_id, num_agents=self.num_agents)
+            instance = Marriages(experiment_id, instance_id, is_imported=False,
+                                 culture_id=self.model_id, num_agents=self.num_agents)
 
             instance.prepare_instance(store=store, params=params)
 
             instances[instance_id] = instance
 
             _keys.append(instance_id)
```

### Comparing `mapel-marriages-2.0.5/src/mapel_marriages.egg-info/PKG-INFO` & `mapel-marriages-2.0.6/src/mapel_marriages.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-marriages
-Version: 2.0.5
+Version: 2.0.6
 Summary: Map of Marriages
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>
 License: Copyright (c) 2018-2022 Stanislaw Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-marriages-2.0.5/src/mapel_marriages.egg-info/SOURCES.txt` & `mapel-marriages-2.0.6/src/mapel_marriages.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 LICENSE.txt
 README.md
 pyproject.toml
 requirements.txt
 src/mapel/marriages/__init__.py
 src/mapel/marriages/cultures_.py
+src/mapel/marriages/distances_.py
 src/mapel/marriages/features_.py
-src/mapel/marriages/metrics_.py
 src/mapel/marriages/cultures/__init__.py
 src/mapel/marriages/cultures/_utils.py
 src/mapel/marriages/cultures/euclidean.py
 src/mapel/marriages/cultures/impartial.py
 src/mapel/marriages/cultures/mallows.py
 src/mapel/marriages/cultures/urn.py
+src/mapel/marriages/distances/__init__.py
+src/mapel/marriages/distances/main_marriages_distances.py
 src/mapel/marriages/features/__init__.py
 src/mapel/marriages/features/basic_features.py
 src/mapel/marriages/features/distance_to_stability_features.py
 src/mapel/marriages/features/experiments_marriage.py
-src/mapel/marriages/metrics/__init__.py
-src/mapel/marriages/metrics/main_marriages_distances.py
 src/mapel/marriages/objects/Marriages.py
 src/mapel/marriages/objects/MarriagesExperiment.py
 src/mapel/marriages/objects/MarriagesFamily.py
 src/mapel/marriages/objects/__init__.py
+src/mapel/marriages/persistence/__init__.py
+src/mapel/marriages/persistence/instance_exports.py
+src/mapel/marriages/persistence/instance_imports.py
 src/mapel_marriages.egg-info/PKG-INFO
 src/mapel_marriages.egg-info/SOURCES.txt
 src/mapel_marriages.egg-info/dependency_links.txt
 src/mapel_marriages.egg-info/requires.txt
 src/mapel_marriages.egg-info/top_level.txt
```

