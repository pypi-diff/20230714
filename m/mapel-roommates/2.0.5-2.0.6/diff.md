# Comparing `tmp/mapel-roommates-2.0.5.tar.gz` & `tmp/mapel-roommates-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapel-roommates-2.0.5.tar", last modified: Fri May 26 20:07:02 2023, max compression
+gzip compressed data, was "mapel-roommates-2.0.6.tar", last modified: Fri Jul 14 09:02:48 2023, max compression
```

## Comparing `mapel-roommates-2.0.5.tar` & `mapel-roommates-2.0.6.tar`

### file list

```diff
@@ -1,40 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:07:02.765950 mapel-roommates-2.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-26 20:06:23.000000 mapel-roommates-2.0.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-26 20:07:02.765950 mapel-roommates-2.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-26 20:06:23.000000 mapel-roommates-2.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-26 20:06:23.000000 mapel-roommates-2.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 20:06:23.000000 mapel-roommates-2.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 20:07:02.765950 mapel-roommates-2.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:07:02.761949 mapel-roommates-2.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:07:02.757949 mapel-roommates-2.0.5/src/mapel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:07:02.761949 mapel-roommates-2.0.5/src/mapel/roommates/
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-26 20:06:23.000000 mapel-roommates-2.0.5/src/mapel/roommates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:07:02.761949 mapel-roommates-2.0.5/src/mapel/roommates/cultures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:23.000000 mapel-roommates-2.0.5/src/mapel/roommates/cultures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-26 20:06:23.000000 mapel-roommates-2.0.5/src/mapel/roommates/cultures/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-05-26 20:06:23.000000 mapel-roommates-2.0.5/src/mapel/roommates/cultures/euclidean.py
--rw-r--r--   0 runner    (1001) docker     (123)    18776 2023-05-26 20:06:23.000000 mapel-roommates-2.0.5/src/mapel/roommates/cultures/group_separable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-05-26 20:06:23.000000 mapel-roommates-2.0.5/src/mapel/roommates/cultures/impartial.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-26 20:06:23.000000 mapel-roommates-2.0.5/src/mapel/roommates/cultures/mallows.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-26 20:06:23.000000 mapel-roommates-2.0.5/src/mapel/roommates/cultures/urn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-26 20:06:23.000000 mapel-roommates-2.0.5/src/mapel/roommates/cultures_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:07:02.761949 mapel-roommates-2.0.5/src/mapel/roommates/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:23.000000 mapel-roommates-2.0.5/src/mapel/roommates/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-05-26 20:06:23.000000 mapel-roommates-2.0.5/src/mapel/roommates/features/basic_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-05-26 20:06:23.000000 mapel-roommates-2.0.5/src/mapel/roommates/features/distance_to_stability_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-26 20:06:23.000000 mapel-roommates-2.0.5/src/mapel/roommates/features_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:07:02.761949 mapel-roommates-2.0.5/src/mapel/roommates/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:23.000000 mapel-roommates-2.0.5/src/mapel/roommates/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-26 20:06:23.000000 mapel-roommates-2.0.5/src/mapel/roommates/metrics/main_distances.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-26 20:06:23.000000 mapel-roommates-2.0.5/src/mapel/roommates/metrics_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:07:02.765950 mapel-roommates-2.0.5/src/mapel/roommates/objects/
--rw-r--r--   0 runner    (1001) docker     (123)     7735 2023-05-26 20:06:23.000000 mapel-roommates-2.0.5/src/mapel/roommates/objects/Roommates.py
--rw-r--r--   0 runner    (1001) docker     (123)    19801 2023-05-26 20:06:23.000000 mapel-roommates-2.0.5/src/mapel/roommates/objects/RoommatesExperiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-26 20:06:23.000000 mapel-roommates-2.0.5/src/mapel/roommates/objects/RoommatesFamily.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:23.000000 mapel-roommates-2.0.5/src/mapel/roommates/objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:07:02.765950 mapel-roommates-2.0.5/src/mapel_roommates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-26 20:07:02.000000 mapel-roommates-2.0.5/src/mapel_roommates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-26 20:07:02.000000 mapel-roommates-2.0.5/src/mapel_roommates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 20:07:02.000000 mapel-roommates-2.0.5/src/mapel_roommates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 20:07:02.000000 mapel-roommates-2.0.5/src/mapel_roommates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 20:07:02.000000 mapel-roommates-2.0.5/src/mapel_roommates.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:48.313692 mapel-roommates-2.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-14 09:02:48.313692 mapel-roommates-2.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 09:02:48.313692 mapel-roommates-2.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:48.309692 mapel-roommates-2.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:48.309692 mapel-roommates-2.0.6/src/mapel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:48.309692 mapel-roommates-2.0.6/src/mapel/roommates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:48.309692 mapel-roommates-2.0.6/src/mapel/roommates/cultures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/cultures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/cultures/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10974 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/cultures/euclidean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18776 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/cultures/group_separable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/cultures/impartial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/cultures/mallows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/cultures/urn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/cultures_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:48.309692 mapel-roommates-2.0.6/src/mapel/roommates/distances/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/distances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/distances/main_distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/distances_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:48.309692 mapel-roommates-2.0.6/src/mapel/roommates/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/features/basic_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/features/distance_to_stability_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/features_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:48.313692 mapel-roommates-2.0.6/src/mapel/roommates/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/objects/Roommates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18739 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/objects/RoommatesExperiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/objects/RoommatesFamily.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:48.313692 mapel-roommates-2.0.6/src/mapel/roommates/persistence/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/persistence/instance_exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-14 09:02:16.000000 mapel-roommates-2.0.6/src/mapel/roommates/persistence/instance_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:48.313692 mapel-roommates-2.0.6/src/mapel_roommates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-14 09:02:48.000000 mapel-roommates-2.0.6/src/mapel_roommates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-14 09:02:48.000000 mapel-roommates-2.0.6/src/mapel_roommates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 09:02:48.000000 mapel-roommates-2.0.6/src/mapel_roommates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 09:02:48.000000 mapel-roommates-2.0.6/src/mapel_roommates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 09:02:48.000000 mapel-roommates-2.0.6/src/mapel_roommates.egg-info/top_level.txt
```

### Comparing `mapel-roommates-2.0.5/LICENSE.txt` & `mapel-roommates-2.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.5/PKG-INFO` & `mapel-roommates-2.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-roommates
-Version: 2.0.5
+Version: 2.0.6
 Summary: Map of Roommates
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>
 License: Copyright (c) 2018-2022 Stanislaw Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-roommates-2.0.5/README.md` & `mapel-roommates-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.5/pyproject.toml` & `mapel-roommates-2.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65", "wheel", "pybind11>=2.6.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mapel-roommates"
-version = "2.0.5"
+version = "2.0.6"
 authors = [
  {name = "Stanislaw Szufa", email = "s.szufa@gmail.com"},
  {name = "Niclas Boehmer", email = "niclas.boehmer@tu-berlin.de"},
 ]
 description = "Map of Roommates"
 classifiers=[
     "Programming Language :: Python :: 3",
```

### Comparing `mapel-roommates-2.0.5/src/mapel/roommates/cultures/euclidean.py` & `mapel-roommates-2.0.6/src/mapel/roommates/cultures/euclidean.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,196 +1,203 @@
 import numpy as np
 import math
 from numpy import linalg
 from mapel.roommates.cultures._utils import convert
 from mapel.roommates.cultures.mallows import mallows_votes
 
-################################################################
-
 def get_range(params):
     if params['p_dist'] == 'beta':
         return np.random.beta(params['a'], params['b'])
     elif params['p_dist'] == 'uniform':
         return np.random.uniform(low=params['a'], high=params['b'])
 
 
 def weighted_l1(a1, a2, w):
     total = 0
     for i in range(len(a1)):
-        total += abs(a1[i]-a2[i])*w[i]
+        total += abs(a1[i] - a2[i]) * w[i]
     return total
 
 
-def generate_attributes_votes(num_agents: int = None, params: dict = None):
-
-    name = f'{params["dim"]}d_{params["space"]}'
+def generate_roommates_attributes_votes(num_agents: int = None,
+                                        dim: int = 2,
+                                        space='uniform',
+                                        **kwargs):
+    name = f'{dim}d_{space}'
 
     agents_skills = np.array([get_rand(name) for _ in range(num_agents)])
     agents_weights = np.array([get_rand(name) for _ in range(num_agents)])
 
     votes = np.zeros([num_agents, num_agents], dtype=int)
     distances = np.zeros([num_agents, num_agents], dtype=float)
-    ones = np.ones([params["dim"]], dtype=float)
+    ones = np.ones([dim], dtype=float)
 
     for v in range(num_agents):
         for c in range(num_agents):
             votes[v][c] = c
-            if params["dim"] == 1:
+            if dim == 1:
                 distances[v][c] = abs(1. - agents_skills[c]) * agents_weights[v]
             else:
                 distances[v][c] = weighted_l1(ones, agents_skills[c], agents_weights[v])
         votes[v] = [x for _, x in sorted(zip(distances[v], votes[v]))]
 
     return convert(votes)
 
 
-def generate_roommates_euclidean_votes(num_agents: int = None, params: dict = None):
-
-    name = f'{params["dim"]}d_{params["space"]}'
+def generate_roommates_euclidean_votes(num_agents: int = None,
+                                       dim: int = 2,
+                                       space='uniform',
+                                       **kwargs):
+    name = f'{dim}d_{space}'
 
     agents = np.array([get_rand(name, i=i, num_agents=num_agents) for i in range(num_agents)])
 
     votes = np.zeros([num_agents, num_agents], dtype=int)
     distances = np.zeros([num_agents, num_agents], dtype=float)
 
     for v in range(num_agents):
         for c in range(num_agents):
-
             votes[v][c] = c
             distances[v][c] = np.linalg.norm(agents[v] - agents[c])
         votes[v] = [x for _, x in sorted(zip(distances[v], votes[v]))]
 
     return convert(votes)
 
 
-def generate_roommates_reverse_euclidean_votes(num_agents: int = None, params: dict = None):
-
-    name = f'{params["dim"]}d_{params["space"]}'
+def generate_roommates_reverse_euclidean_votes(num_agents: int = None,
+                                               dim: int = 2,
+                                               space='uniform',
+                                               proportion=0.5,
+                                               **kwargs):
+    name = f'{dim}d_{space}'
 
     agents = np.array([get_rand(name, i=i, num_agents=num_agents) for i in range(num_agents)])
 
     votes = np.zeros([num_agents, num_agents], dtype=int)
     distances = np.zeros([num_agents, num_agents], dtype=float)
 
     for v in range(num_agents):
         for c in range(num_agents):
-
             votes[v][c] = c
             distances[v][c] = np.linalg.norm(agents[v] - agents[c])
         votes[v] = [x for _, x in sorted(zip(distances[v], votes[v]))]
 
-    if 'proportion' in params:
-        p = params['proportion']
-    else:
-        p = 0.5
+    p = proportion
 
-    for i in range(int(num_agents * (1.-p))):
+    for i in range(int(num_agents * (1. - p))):
         tmp = list(votes[i])
         tmp.reverse()
         votes[i] = tmp
 
     return convert(votes)
 
 
-def generate_expectation_votes(num_agents: int = None, params: dict = None):
-
-    name = f'{params["dim"]}d_{params["space"]}'
+def generate_roommates_expectation_votes(num_agents: int = None,
+                                         dim: int = 2,
+                                         space='uniform',
+                                         std=0.1,
+                                         **kwargs):
+    name = f'{dim}d_{space}'
 
     agents_reality = np.array([get_rand(name) for _ in range(num_agents)])
     agents_wishes = np.zeros([num_agents, 2])
 
     for v in range(num_agents):
         # while agents_wishes[v][0] <= 0 or agents_wishes[v][0] >= 1:
-        agents_wishes[v][0] = np.random.normal(agents_reality[v][0], params['std'])
+        agents_wishes[v][0] = np.random.normal(agents_reality[v][0], std)
         # while agents_wishes[v][1] <= 0 or agents_wishes[v][1] >= 1:
-        agents_wishes[v][1] = np.random.normal(agents_reality[v][1], params['std'])
+        agents_wishes[v][1] = np.random.normal(agents_reality[v][1], std)
 
     votes = np.zeros([num_agents, num_agents], dtype=int)
     distances = np.zeros([num_agents, num_agents], dtype=float)
 
     for v in range(num_agents):
         for c in range(num_agents):
-
             votes[v][c] = c
             distances[v][c] = np.linalg.norm(agents_reality[c] - agents_wishes[v])
         votes[v] = [x for _, x in sorted(zip(distances[v], votes[v]))]
 
     return convert(votes)
 
 
-def generate_fame_votes(num_agents: int = None, params: dict = None):
+def generate_roommates_fame_votes(num_agents: int = None,
+                                  dim: int = 2,
+                                  space='uniform',
+                                  radius=0.1,
+                                  **kwargs):
     # Also known as radius model
 
-    name = f'{params["dim"]}d_{params["space"]}'
+    name = f'{dim}d_{space}'
 
     agents = np.array([get_rand(name) for _ in range(num_agents)])
     votes = np.zeros([num_agents, num_agents], dtype=int)
     distances = np.zeros([num_agents, num_agents], dtype=float)
-    rays = np.array([np.random.uniform(0, params['radius']) for _ in range(num_agents)])
+    rays = np.array([np.random.uniform(0, radius) for _ in range(num_agents)])
 
     for v in range(num_agents):
         for c in range(num_agents):
             votes[v][c] = c
             distances[v][c] = np.linalg.norm(agents[v] - agents[c])
             distances[v][c] = distances[v][c] - rays[c]
         votes[v] = [x for _, x in sorted(zip(distances[v], votes[v]))]
 
     return convert(votes)
 
 
-def generate_roommates_mallows_euclidean_votes(num_agents: int = None, params: dict = None):
-
-    name = f'{params["dim"]}d_{params["space"]}'
+def generate_roommates_mallows_euclidean_votes(num_agents: int = None,
+                                               dim: int = 2,
+                                               space='uniform',
+                                               phi=0.5,
+                                               **kwargs):
+    name = f'{dim}d_{space}'
 
     agents = np.array([get_rand(name, i=i, num_agents=num_agents) for i in range(num_agents)])
 
     votes = np.zeros([num_agents, num_agents], dtype=int)
     distances = np.zeros([num_agents, num_agents], dtype=float)
 
     for v in range(num_agents):
         for c in range(num_agents):
-
             votes[v][c] = c
             distances[v][c] = np.linalg.norm(agents[v] - agents[c])
         votes[v] = [x for _, x in sorted(zip(distances[v], votes[v]))]
 
-    votes = mallows_votes(votes, params['phi'])
+    votes = mallows_votes(votes, phi)
 
     return convert(votes)
 
 # AUXILIARY
 def random_ball(dimension, num_points=1, radius=1):
     random_directions = np.random.normal(size=(dimension, num_points))
     random_directions /= linalg.norm(random_directions, axis=0)
     random_radii = np.random.random(num_points) ** (1 / dimension)
     return radius * (random_directions * random_radii).T
 
-
 GEN_CTR = 0
-
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
@@ -251,22 +258,22 @@
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

### Comparing `mapel-roommates-2.0.5/src/mapel/roommates/cultures/group_separable.py` & `mapel-roommates-2.0.6/src/mapel/roommates/cultures/group_separable.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.5/src/mapel/roommates/cultures/impartial.py` & `mapel-roommates-2.0.6/src/mapel/roommates/cultures/impartial.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 
 
 import numpy as np
 from mapel.roommates.cultures._utils import convert
 from mapel.core.utils import *
 import logging
 
-def generate_roommates_ic_votes(num_agents: int = None):
+
+def generate_roommates_ic_votes(num_agents: int = None, **kwargs):
     """ Impartial Culture """
 
     votes = [list(np.random.permutation(num_agents)) for _ in range(num_agents)]
 
     return convert(votes)
 
 
-def generate_roommates_group_ic_votes(num_agents: int = None, params: dict = None):
+def generate_roommates_group_ic_votes(num_agents: int = None,
+                                      proportion=0.5,
+                                      **kwargs):
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
@@ -31,32 +31,32 @@
                for _ in range(size_2)]
 
     votes = votes_1 + votes_2
 
     return convert(votes)
 
 
-def generate_roommates_id_votes(num_agents: int = None):
+def generate_roommates_id_votes(num_agents: int = None, **kwargs):
     """ One of four extreme points for Compass """
 
     votes = [list(range(num_agents)) for _ in range(num_agents)]
 
     return convert(votes)
 
 
-def generate_roommates_asymmetric_votes(num_agents: int = None):
+def generate_roommates_asymmetric_votes(num_agents: int = None, **kwargs):
     """ One of four extreme points for Compass """
     votes = [list(range(num_agents)) for _ in range(num_agents)]
 
     votes = [rotate(vote, shift) for shift, vote in enumerate(votes)]
 
     return convert(votes)
 
 
-def generate_roommates_symmetric_votes(num_agents: int = None):
+def generate_roommates_symmetric_votes(num_agents: int = None, **kwargs):
     """ One of four extreme points for Compass """
 
     num_rounds = num_agents - 1
 
     def next(agents):
         first = agents[0]
         last = agents[-1]
@@ -83,15 +83,15 @@
         for x, y in partition:
             votes[x][pos] = y
             votes[y][pos] = x
 
     return votes
 
 
-def generate_roommates_chaos_votes(num_agents: int = None):
+def generate_roommates_chaos_votes(num_agents: int = None, **kwargs):
     """ One of four extreme points for Compass """
 
     if num_agents-1 % 3 == 0:
         logging.warning("Incorrect realization of Chaos instance")
 
     num_rooms = num_agents // 2
     matrix = np.zeros([num_agents, num_agents - 1], dtype=int)
```

### Comparing `mapel-roommates-2.0.5/src/mapel/roommates/cultures/urn.py` & `mapel-roommates-2.0.6/src/mapel/roommates/cultures/urn.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import numpy as np
 from mapel.roommates.cultures._utils import convert
 
 
-def generate_roommates_urn_votes(num_agents: int = None, params=None):
+def generate_roommates_urn_votes(num_agents: int = None,
+                                 alpha: int = 0.1,
+                                 **kwargs):
+
     votes = np.zeros([num_agents, num_agents], dtype=int)
     urn_size = 1.
     for j in range(num_agents):
         rho = np.random.uniform(0, urn_size)
         if rho <= 1.:
             votes[j] = np.random.permutation(num_agents)
         else:
             votes[j] = votes[np.random.randint(0, j)]
-        urn_size += params['alpha']
+        urn_size += alpha
 
     return convert(votes)
 
 # # # # # # # # # # # # # # # #
-# LAST CLEANUP ON: 16.03.2022 #
+# LAST CLEANUP ON:  9.06.2023 #
 # # # # # # # # # # # # # # # #
```

### Comparing `mapel-roommates-2.0.5/src/mapel/roommates/cultures_.py` & `mapel-roommates-2.0.6/src/mapel/roommates/cultures_.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,53 +4,43 @@
 
 import numpy as np
 
 import mapel.roommates.cultures.euclidean as euclidean
 import mapel.roommates.cultures.impartial as impartial
 import mapel.roommates.cultures.mallows as mallows
 import mapel.roommates.cultures.urn as urn
-import mapel.roommates.cultures.group_separable as group_separable
 
 
-def generate_votes(culture_id: str = None, num_agents: int = None,
-                   params: dict = None) -> Union[list, np.ndarray]:
+registered_roommates_culture = {
+    'ic': impartial.generate_roommates_ic_votes,
+    'id': impartial.generate_roommates_id_votes,
+    'chaos': impartial.generate_roommates_chaos_votes,
+    'symmetric': impartial.generate_roommates_symmetric_votes,
+    'asymmetric': impartial.generate_roommates_asymmetric_votes,
+    'urn': urn.generate_roommates_urn_votes,
+    'fame': euclidean.generate_roommates_fame_votes,
+    'expectation': euclidean.generate_roommates_expectation_votes,
+    'attributes': euclidean.generate_roommates_attributes_votes,
+    'euclidean': euclidean.generate_roommates_euclidean_votes,
+    'reverse_euclidean': euclidean.generate_roommates_reverse_euclidean_votes,
+    'group_ic': impartial.generate_roommates_group_ic_votes,
+    'norm-mallows': mallows.generate_roommates_norm_mallows_votes,
+    'mallows_euclidean': euclidean.generate_roommates_mallows_euclidean_votes,
+    'malasym': mallows.generate_roommates_malasym_votes,
+}
 
-    main_models_with_params = {
-        'roommates_norm-mallows': mallows.generate_roommates_norm_mallows_votes,
-        'roommates_urn': urn.generate_roommates_urn_votes,
-        'roommates_euclidean': euclidean.generate_roommates_euclidean_votes,
-        'roommates_reverse_euclidean': euclidean.generate_roommates_reverse_euclidean_votes,
-        'roommates_gs': group_separable.generate_roommates_gs_votes,
-        'roommates_radius': euclidean.generate_fame_votes,  # deprecated
-        'fame': euclidean.generate_fame_votes,
-        'roommates_double': euclidean.generate_expectation_votes,  # deprecated
-        'expectation': euclidean.generate_expectation_votes,
-        'roommates_mallows_euclidean': euclidean.generate_roommates_mallows_euclidean_votes,
-        'roommates_vectors': euclidean.generate_attributes_votes,  # deprecated
-        'attributes': euclidean.generate_attributes_votes,
-        'roommates_malasym': mallows.generate_roommates_malasym_votes,
-        'roommates_group_ic': impartial.generate_roommates_group_ic_votes,
-    }
-
-    main_models_without_params = {
-        'roommates_ic': impartial.generate_roommates_ic_votes,
-        'roommates_id': impartial.generate_roommates_id_votes,
-        'roommates_chaos': impartial.generate_roommates_chaos_votes,
-        'roommates_symmetric': impartial.generate_roommates_symmetric_votes,
-        'roommates_asymmetric': impartial.generate_roommates_asymmetric_votes,
-    }
 
-    if culture_id in main_models_with_params:
-        return main_models_with_params.get(culture_id)(num_agents=num_agents, params=params)
+def generate_votes(culture_id: str = None, num_agents: int = None,
+                   params: dict = None) -> Union[list, np.ndarray]:
 
-    if culture_id in main_models_without_params:
-        return main_models_without_params.get(culture_id)(num_agents=num_agents)
+    if culture_id in registered_roommates_culture:
+        return registered_roommates_culture.get(culture_id)(num_agents=num_agents, **params)
 
     else:
         print("No such election culture_id!", culture_id)
         return []
 
 
 # # # # # # # # # # # # # # # #
-# LAST CLEANUP ON: 16.03.2022 #
+# LAST CLEANUP ON:  9.06.2023 #
 # # # # # # # # # # # # # # # #
```

### Comparing `mapel-roommates-2.0.5/src/mapel/roommates/features/basic_features.py` & `mapel-roommates-2.0.6/src/mapel/roommates/features/basic_features.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     for i in range(num_agents):
         pref = [x for x in range(num_agents) if x != i]
         shuffle(pref)
         instance.append(pref)
     return instance
 
 def number_blockingPairs(instance,matching):
-    # print(matching)
     bps=0
     num_agents=len(instance)
     for i in range(num_agents):
         for j in range(i+1,num_agents):
             if i!=j:
                 partner_i=matching[i]
                 partneri_index=instance[i].index(partner_i)
```

### Comparing `mapel-roommates-2.0.5/src/mapel/roommates/features/distance_to_stability_features.py` & `mapel-roommates-2.0.6/src/mapel/roommates/features/distance_to_stability_features.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.5/src/mapel/roommates/features_.py` & `mapel-roommates-2.0.6/src/mapel/roommates/features_.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 #!/usr/bin/env python
 
 import mapel.roommates.features.basic_features as basic
-from mapel.core.glossary import MAIN_LOCAL_FEATUERS, MAIN_GLOBAL_FEATUERS
-from mapel.core.features_main import get_main_local_feature, get_main_global_feature
+from mapel.core.glossary import MAIN_GLOBAL_FEATUERS
+from mapel.core.features_main import get_main_global_feature
 import numpy as np
 from itertools import combinations
 from mapel.core.inner_distances import l2
 
+registered_roommates_features = {
+    'summed_rank_minimal_matching': basic.summed_rank_minimal_matching,
+    'summed_rank_maximal_matching': basic.summed_rank_maximal_matching,
+    'minimal_rank_maximizing_matching': basic.minimal_rank_maximizing_matching,
+    'min_num_bps_matching': basic.min_num_bps_matching,
+    'num_of_bps_min_weight': basic.num_of_bps_maximumWeight,
+    'avg_num_of_bps_for_rand_matching': basic.avg_num_of_bps_for_random_matching,
+    'mutuality': basic.mutuality,
+    'dist_from_id_1': basic.dist_from_id_1,
+    'dist_from_id_2': basic.dist_from_id_2,
+}
 
-def get_local_feature(feature_id):
-    if feature_id in MAIN_LOCAL_FEATUERS:
-        return get_main_local_feature(feature_id)
 
-    return {'summed_rank_minimal_matching': basic.summed_rank_minimal_matching,
-            'summed_rank_maximal_matching': basic.summed_rank_maximal_matching,
-            'minimal_rank_maximizing_matching': basic.minimal_rank_maximizing_matching,
-            'min_num_bps_matching': basic.min_num_bps_matching,
-            'num_of_bps_min_weight': basic.num_of_bps_maximumWeight,
-            'avg_num_of_bps_for_rand_matching': basic.avg_num_of_bps_for_random_matching,
-            'mutuality': basic.mutuality,
-            'dist_from_id_1': basic.dist_from_id_1,
-            'dist_from_id_2': basic.dist_from_id_2,
-            }.get(feature_id)
+def get_local_feature(feature_id):
+    if feature_id in registered_roommates_features:
+        return registered_roommates_features.get(feature_id)
+    return {
+    }.get(feature_id)
 
 
 def get_global_feature(feature_id):
     if feature_id in MAIN_GLOBAL_FEATUERS:
         return get_main_global_feature(feature_id)
 
     return {'monotonicity': monotonicity,
             'distortion_from_all': distortion_from_all,
             }.get(feature_id)
 
-
 # TMP FUNCS
 def monotonicity(experiment, instance) -> float:
     e0 = instance.instance_id
     c0 = np.array(experiment.coordinates[e0])
     distortion = 0
     for e1, e2 in combinations(experiment.instances, 2):
         if e1 != e0 and e2 != e0:
@@ -47,43 +49,31 @@
             embedded_d2 = np.linalg.norm(c0 - experiment.coordinates[e2])
             embedded_proportion = embedded_d1 / embedded_d2
             _max = max(original_proportion, embedded_proportion)
             _min = min(original_proportion, embedded_proportion)
             distortion += _max / _min
     return distortion
 
-#
+
 def distortion_from_all(experiment, election):
     values = np.array([])
     one_side_values = np.array([])
     election_id_1 = election.instance_id
 
     for election_id_2 in experiment.instances:
-        # if election_id_2 in {'identity_10_100_0', 'uniformity_10_100_0',
-        #                      'antagonism_10_100_0', 'stratification_10_100_0'}:
         if election_id_1 != election_id_2:
-            # m = election.instances[election_id_1].num_candidates
-            # print(election_id_1, election_id_2)
             true_distance = experiment.distances[election_id_1][election_id_2]
             true_distance /= experiment.distances['MD']['MA']
             embedded_distance = l2(np.array(experiment.coordinates[election_id_1]),
                                    np.array(experiment.coordinates[election_id_2]))
 
             embedded_distance /= \
                 l2(np.array(experiment.coordinates['MD']),
                    np.array(experiment.coordinates['MA']))
-            # try:
-            #     ratio = float(embedded_distance) / float(true_distance)
-            # except:
-            #     ratio = 1.
             one_side_ratio = embedded_distance / true_distance
             one_side_values = np.append(one_side_values, one_side_ratio)
 
             ratio = max(embedded_distance, true_distance) / min(embedded_distance, true_distance)
 
             values = np.append(values, ratio)
 
-    # print(min(one_side_values), max(one_side_values))
-    # if election_id_1 == 'IC_0':
-    #     print(values)
-
     return np.mean(values)
```

### Comparing `mapel-roommates-2.0.5/src/mapel/roommates/metrics/main_distances.py` & `mapel-roommates-2.0.6/src/mapel/roommates/distances/main_distances.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.5/src/mapel/roommates/metrics_.py` & `mapel-roommates-2.0.6/src/mapel/roommates/distances_.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,64 @@
 #!/usr/bin/env python
 import copy
 import csv
-import itertools
 from time import time
 import logging
 import os
 from typing import Callable
 
 import numpy as np
 
 from mapel.core.inner_distances import map_str_to_func
 from mapel.core.objects.Experiment import Experiment
-from mapel.roommates.metrics import main_distances as mrd
+from mapel.roommates.distances import main_distances as mrd
 from mapel.roommates.objects.Roommates import Roommates
 
+registered_roommates_distances = {
+    'mutual_attraction': mrd.compute_retrospective_distance,
+
+    'positionwise': mrd.compute_positionwise_distance,  # unsupported distance
+    'pos_swap': mrd.compute_pos_swap_distance,  # unsupported distance
+    'swap_bf': mrd.compute_swap_bf_distance,  # unsupported distance
+    'pairwise': mrd.compute_pairwise_distance,  # unsupported distance
+}
+
 
 def get_distance(election_1: Roommates, election_2: Roommates,
                  distance_id: str = None) -> float or (float, list):
     """ Return: distance between ordinal elections, (if applicable) optimal matching """
 
     inner_distance, main_distance = extract_distance_id(distance_id)
 
-    metrics_without_params = {
-    }
-
-    metrics_with_inner_distance = {
-        'mutual_attraction': mrd.compute_retrospective_distance,
-        'positionwise': mrd.compute_positionwise_distance,
-        'pos_swap': mrd.compute_pos_swap_distance,
-        'swap_bf': mrd.compute_swap_bf_distance,
-        'pairwise': mrd.compute_pairwise_distance,
-    }
-
-    if main_distance in metrics_without_params:
-        return metrics_without_params.get(main_distance)(election_1, election_2)
-
-    elif main_distance in metrics_with_inner_distance:
-        return metrics_with_inner_distance.get(main_distance)(election_1, election_2,
-                                                              inner_distance)
+    if main_distance in registered_roommates_distances:
+        return registered_roommates_distances.get(main_distance)(election_1,
+                                                                 election_2,
+                                                                 inner_distance)
     else:
         logging.warning('No such metric!')
 
 
 def extract_distance_id(distance_id: str) -> (Callable, str):
     if '-' in distance_id:
         inner_distance, main_distance = distance_id.split('-')
         inner_distance = map_str_to_func(inner_distance)
     else:
         main_distance = distance_id
         inner_distance = None
     return inner_distance, main_distance
 
 
-def run_single_thread(experiment: Experiment, thread_ids: list,
-                      distances: dict, times: dict, matchings: dict,
-                      printing: bool, t) -> None:
+def run_single_thread(experiment: Experiment,
+                      thread_ids: list,
+                      distances: dict,
+                      times: dict,
+                      matchings: dict,
+                      t) -> None:
     """ Single thread for computing distances """
     for election_id_1, election_id_2 in thread_ids:
-        if t == 0 and printing:
-            print(election_id_1, election_id_2)
         start_time = time()
 
         distance = get_distance(copy.deepcopy(experiment.instances[election_id_1]),
                                 copy.deepcopy(experiment.instances[election_id_2]),
                                 distance_id=copy.deepcopy(experiment.distance_id),
                                 )
         if type(distance) is tuple:
@@ -87,11 +83,10 @@
                 ["instance_id_1", "instance_id_2", "distance", "time"])
 
             for election_id_1, election_id_2 in thread_ids:
                 distance = float(distances[election_id_1][election_id_2])
                 time_ = float(times[election_id_1][election_id_2])
                 writer.writerow([election_id_1, election_id_2, distance, time_])
 
-
 # # # # # # # # # # # # # # # #
 # LAST CLEANUP ON: 13.10.2021 #
 # # # # # # # # # # # # # # # #
```

### Comparing `mapel-roommates-2.0.5/src/mapel/roommates/objects/RoommatesExperiment.py` & `mapel-roommates-2.0.6/src/mapel/roommates/objects/RoommatesExperiment.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 #!/usr/bin/env python
 import ast
 import copy
 import csv
 import itertools
-import os
 from multiprocessing import Process
 from time import sleep
 import time
 
 from mapel.core.objects.Experiment import Experiment
 from mapel.roommates.objects.RoommatesFamily import RoommatesFamily
 from mapel.roommates.objects.Roommates import Roommates
 import mapel.roommates.cultures_ as models_main
-import mapel.roommates.metrics_ as metr
+import mapel.roommates.distances_ as metr
 import mapel.roommates.features.basic_features as basic
 import mapel.roommates.features_ as features
 from mapel.core.utils import *
 from mapel.core.glossary import *
-from mapel.core.printing import get_values_from_csv_file
+from mapel.core.persistence.experiment_imports import get_values_from_csv_file
 
 try:
     from sklearn.manifold import MDS
     from sklearn.manifold import TSNE
     from sklearn.manifold import SpectralEmbedding
     from sklearn.manifold import LocallyLinearEmbedding
     from sklearn.manifold import Isomap
@@ -121,17 +120,18 @@
         self.num_instances = sum([self.families[family_id].size for family_id in self.families])
 
         models_main.prepare_instances(experiment=self,
                                     culture_id=self.families[family_id].culture_id,
                                     family_id=family_id,
                                     params=copy.deepcopy(self.families[family_id].params))
 
-
-    def compute_distances(self, distance_id: str = 'emd-positionwise', num_threads: int = 1,
-                          self_distances: bool = False, printing: bool = False) -> None:
+    def compute_distances(self,
+                          distance_id: str = 'emd-positionwise',
+                          num_threads: int = 1,
+                          self_distances: bool = False) -> None:
 
         self.distance_id = distance_id
 
         if '-pairwise' in distance_id:
             for instance in self.instances.values():
                 instance.votes_to_pairwise_matrix()
 
@@ -145,27 +145,29 @@
                 if i == j:
                     if self_distances:
                         ids.append((instance_1, instance_2))
                 elif i < j:
                     ids.append((instance_1, instance_2))
 
         num_distances = len(ids)
-
         processes =[]
 
         for t in range(num_threads):
             print(f'Starting thread: {t}')
             sleep(0.1)
             start = int(t * num_distances / num_threads)
             stop = int((t + 1) * num_distances / num_threads)
             thread_ids = ids[start:stop]
 
-            process = Process(target=metr.run_single_thread, args=(self, thread_ids,
-                                                                     distances, times, matchings,
-                                                                     printing, t ))
+            process = Process(target=metr.run_single_thread, args=(self,
+                                                                   thread_ids,
+                                                                     distances,
+                                                                   times,
+                                                                   matchings,
+                                                                     t ))
 
             process.start()
             processes.append(process)
 
         for process in processes:
             process.join()
 
@@ -203,25 +205,25 @@
 
         self.distances = distances
         self.times = times
         self.matchings = matchings
 
         for instance_id_1 in self.distances:
             for instance_id_2 in self.distances[instance_id_1]:
-                self.distances[instance_id_2][instance_id_1] = self.distances[instance_id_1][instance_id_2]
-                self.times[instance_id_2][instance_id_1] = self.times[instance_id_1][instance_id_2]
-
-
+                self.distances[instance_id_2][instance_id_1] = \
+                    self.distances[instance_id_1][instance_id_2]
+                self.times[instance_id_2][instance_id_1] = \
+                    self.times[instance_id_1][instance_id_2]
 
     def import_controllers(self):
         """ Import controllers from a file """
 
         families = {}
 
-        path = os.path.join(os.getcwd(), 'election', self.experiment_id, 'map.csv')
+        path = os.path.join(os.getcwd(), 'experiments', self.experiment_id, 'map.csv')
         file_ = open(path, 'r')
 
         header = [h.strip() for h in file_.readline().split(';')]
         reader = csv.DictReader(file_, fieldnames=header, delimiter=';')
 
         starting_from = 0
         for row in reader:
@@ -293,15 +295,15 @@
 
         if self.instances is None:
             self.instances = {}
 
         for family_id in self.families:
 
             new_instances = self.families[family_id].prepare_family(
-                store=self.is_exported,
+                is_exported=self.is_exported,
                 experiment_id=self.experiment_id)
 
             for instance_id in new_instances:
                 self.instances[instance_id] = new_instances[instance_id]
 
     def compute_stable_sr(self):
         for instance_id in self.instances:
@@ -324,15 +326,17 @@
                 writer.writerow(
                     ["instance_id", "matching"])
 
                 for instance_id in self.instances:
                     usable_matching = self.matchings[instance_id]
                     writer.writerow([instance_id, usable_matching])
 
-    def compute_feature(self, feature_id: str = None, feature_params=None, printing=False) -> dict:
+    def compute_feature(self,
+                        feature_id: str = None,
+                        feature_params=None) -> dict:
 
         if feature_params is None:
             feature_params = {}
 
         feature_dict = {'value': {}, 'time': {}, 'std': {}}
 
         features_with_std = {'avg_num_of_bps_for_rand_matching'}
@@ -370,17 +374,14 @@
                     else:
                         value = abs(maximal[instance_id] - minimal[instance_id])
                     feature_dict['value'][instance_id] = value
                     feature_dict['time'][instance_id] = 0
 
             else:
                 for instance_id in self.instances:
-                    if printing:
-                        print(instance_id)
-                    feature = features.get_local_feature(feature_id)
                     feature = features.get_local_feature(feature_id)
                     instance = self.instances[instance_id]
 
                     start = time.time()
 
                     for _ in range(num_iterations):
 
@@ -393,34 +394,14 @@
                         else:
                             value = feature(instance)
 
                         print(value)
 
                     total_time = time.time() - start
                     total_time /= num_iterations
-                    #
-                    # elif feature_id in ['largest_cohesive_group', 'number_of_cohesive_groups',
-                    #                     'number_of_cohesive_groups_brute',
-                    #                     'proportionality_degree_pav',
-                    #                     'proportionality_degree_av',
-                    #                     'proportionality_degree_cc',
-                    #                     'justified_ratio',
-                    #                     'cohesiveness',
-                    #                     'partylist',
-                    #                     'highest_cc_score',
-                    #                     'highest_hb_score']:
-                    #     value = feature(election, feature_params)
-                    #
-                    # elif feature_id in {'avg_distortion_from_guardians',
-                    #                     'worst_distortion_from_guardians',
-                    #                     'distortion_from_all',
-                    #                     'distortion_from_top_100'}:
-                    #     value = feature(election, election_id)
-                    # else:
-                    #     value = feature(election)
 
                     if feature_id in features_with_std:
                         feature_dict['value'][instance_id] = value[0]
                         feature_dict['time'][instance_id] = total_time
                         feature_dict['std'][instance_id] = value[1]
                     else:
                         feature_dict['value'][instance_id] = value
```

### Comparing `mapel-roommates-2.0.5/src/mapel/roommates/objects/RoommatesFamily.py` & `mapel-roommates-2.0.6/src/mapel/roommates/objects/RoommatesFamily.py`

 * *Files 11% similar despite different names*

```diff
@@ -66,38 +66,38 @@
             path['start'] = 0.
 
         if 'step' in path:
             params[variable] = path['start'] + j * path['step']
 
         return params, variable
 
-    def prepare_family(self, experiment_id=None, store=None):
+    def prepare_family(self, experiment_id=None, is_exported=None):
 
         instances = {}
 
         _keys = []
         for j in range(self.size):
 
             params = copy.deepcopy(self.params)
 
             path = self.path
             if path is not None and 'variable' in path:
                 new_params, variable = self._get_params_for_paths(j)
                 params = {**params, **new_params}
 
-            if params is not None and 'norm-phi' in params:
-                params['phi'] = mallows.phi_from_relphi(self.num_agents,
-                                                        relphi=params['norm-phi'])
+            if params is not None and 'normphi' in params:
+                params['phi'] = mallows.phi_from_normphi(self.num_agents,
+                                                        relphi=params['normphi'])
 
             instance_id = get_instance_id(self.single, self.family_id, j)
 
-            instance = Roommates(experiment_id, instance_id, _import=False,
+            instance = Roommates(experiment_id, instance_id, is_imported=False,
                                  culture_id=self.culture_id, num_agents=self.num_agents)
 
-            instance.prepare_instance(store=store, params=params)
+            instance.prepare_instance(is_exported=is_exported, params=params)
 
             instances[instance_id] = instance
 
             _keys.append(instance_id)
 
         self.instance_ids = _keys
```

### Comparing `mapel-roommates-2.0.5/src/mapel_roommates.egg-info/PKG-INFO` & `mapel-roommates-2.0.6/src/mapel_roommates.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-roommates
-Version: 2.0.5
+Version: 2.0.6
 Summary: Map of Roommates
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>
 License: Copyright (c) 2018-2022 Stanislaw Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-roommates-2.0.5/src/mapel_roommates.egg-info/SOURCES.txt` & `mapel-roommates-2.0.6/src/mapel_roommates.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 LICENSE.txt
 README.md
 pyproject.toml
 requirements.txt
 src/mapel/roommates/__init__.py
 src/mapel/roommates/cultures_.py
+src/mapel/roommates/distances_.py
 src/mapel/roommates/features_.py
-src/mapel/roommates/metrics_.py
 src/mapel/roommates/cultures/__init__.py
 src/mapel/roommates/cultures/_utils.py
 src/mapel/roommates/cultures/euclidean.py
 src/mapel/roommates/cultures/group_separable.py
 src/mapel/roommates/cultures/impartial.py
 src/mapel/roommates/cultures/mallows.py
 src/mapel/roommates/cultures/urn.py
+src/mapel/roommates/distances/__init__.py
+src/mapel/roommates/distances/main_distances.py
 src/mapel/roommates/features/__init__.py
 src/mapel/roommates/features/basic_features.py
 src/mapel/roommates/features/distance_to_stability_features.py
-src/mapel/roommates/metrics/__init__.py
-src/mapel/roommates/metrics/main_distances.py
 src/mapel/roommates/objects/Roommates.py
 src/mapel/roommates/objects/RoommatesExperiment.py
 src/mapel/roommates/objects/RoommatesFamily.py
 src/mapel/roommates/objects/__init__.py
+src/mapel/roommates/persistence/__init__.py
+src/mapel/roommates/persistence/instance_exports.py
+src/mapel/roommates/persistence/instance_imports.py
 src/mapel_roommates.egg-info/PKG-INFO
 src/mapel_roommates.egg-info/SOURCES.txt
 src/mapel_roommates.egg-info/dependency_links.txt
 src/mapel_roommates.egg-info/requires.txt
 src/mapel_roommates.egg-info/top_level.txt
```

