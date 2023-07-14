# Comparing `tmp/mapel-core-2.0.5.tar.gz` & `tmp/mapel-core-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapel-core-2.0.5.tar", last modified: Fri May 26 20:06:45 2023, max compression
+gzip compressed data, was "mapel-core-2.0.6.tar", last modified: Fri Jul 14 09:02:34 2023, max compression
```

## Comparing `mapel-core-2.0.5.tar` & `mapel-core-2.0.6.tar`

### file list

```diff
@@ -1,50 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:45.573657 mapel-core-2.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-26 20:06:23.000000 mapel-core-2.0.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-26 20:06:45.573657 mapel-core-2.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-26 20:06:23.000000 mapel-core-2.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-26 20:06:23.000000 mapel-core-2.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-26 20:06:23.000000 mapel-core-2.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 20:06:45.573657 mapel-core-2.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:45.557657 mapel-core-2.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:45.553657 mapel-core-2.0.5/src/mapel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:45.561657 mapel-core-2.0.5/src/mapel/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:23.000000 mapel-core-2.0.5/src/mapel/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:45.561657 mapel-core-2.0.5/src/mapel/core/embedding/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:23.000000 mapel-core-2.0.5/src/mapel/core/embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-26 20:06:23.000000 mapel-core-2.0.5/src/mapel/core/embedding/initial_positions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:45.565657 mapel-core-2.0.5/src/mapel/core/embedding/kamada_kawai/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:23.000000 mapel-core-2.0.5/src/mapel/core/embedding/kamada_kawai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-05-26 20:06:23.000000 mapel-core-2.0.5/src/mapel/core/embedding/kamada_kawai/energy_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-05-26 20:06:23.000000 mapel-core-2.0.5/src/mapel/core/embedding/kamada_kawai/kamada_kawai.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-26 20:06:23.000000 mapel-core-2.0.5/src/mapel/core/embedding/kamada_kawai/optimization_algorithms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:45.565657 mapel-core-2.0.5/src/mapel/core/embedding/simulated_annealing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:23.000000 mapel-core-2.0.5/src/mapel/core/embedding/simulated_annealing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-05-26 20:06:23.000000 mapel-core-2.0.5/src/mapel/core/embedding/simulated_annealing/simulated_annealing.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-26 20:06:23.000000 mapel-core-2.0.5/src/mapel/core/embedding/simulated_annealing/simulated_annealing_energy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:45.565657 mapel-core-2.0.5/src/mapel/core/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:23.000000 mapel-core-2.0.5/src/mapel/core/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-26 20:06:23.000000 mapel-core-2.0.5/src/mapel/core/features/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-05-26 20:06:23.000000 mapel-core-2.0.5/src/mapel/core/features/distortion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-05-26 20:06:23.000000 mapel-core-2.0.5/src/mapel/core/features/monotonicity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-26 20:06:23.000000 mapel-core-2.0.5/src/mapel/core/features/stability.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-26 20:06:23.000000 mapel-core-2.0.5/src/mapel/core/features_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-05-26 20:06:23.000000 mapel-core-2.0.5/src/mapel/core/glossary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-26 20:06:23.000000 mapel-core-2.0.5/src/mapel/core/inner_distances.py
--rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-05-26 20:06:23.000000 mapel-core-2.0.5/src/mapel/core/matchings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:45.569657 mapel-core-2.0.5/src/mapel/core/objects/
--rw-r--r--   0 runner    (1001) docker     (123)    24483 2023-05-26 20:06:23.000000 mapel-core-2.0.5/src/mapel/core/objects/Experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-26 20:06:23.000000 mapel-core-2.0.5/src/mapel/core/objects/Family.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-26 20:06:23.000000 mapel-core-2.0.5/src/mapel/core/objects/Instance.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:23.000000 mapel-core-2.0.5/src/mapel/core/objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:45.569657 mapel-core-2.0.5/src/mapel/core/persistence/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:23.000000 mapel-core-2.0.5/src/mapel/core/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-05-26 20:06:23.000000 mapel-core-2.0.5/src/mapel/core/persistence/experiment_exports.py
--rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-05-26 20:06:23.000000 mapel-core-2.0.5/src/mapel/core/persistence/experiment_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)    62604 2023-05-26 20:06:23.000000 mapel-core-2.0.5/src/mapel/core/printing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-26 20:06:23.000000 mapel-core-2.0.5/src/mapel/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:45.573657 mapel-core-2.0.5/src/mapel_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-26 20:06:45.000000 mapel-core-2.0.5/src/mapel_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-26 20:06:45.000000 mapel-core-2.0.5/src/mapel_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 20:06:45.000000 mapel-core-2.0.5/src/mapel_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-26 20:06:45.000000 mapel-core-2.0.5/src/mapel_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 20:06:45.000000 mapel-core-2.0.5/src/mapel_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:34.121503 mapel-core-2.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-14 09:02:16.000000 mapel-core-2.0.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-14 09:02:34.121503 mapel-core-2.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-14 09:02:16.000000 mapel-core-2.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-14 09:02:16.000000 mapel-core-2.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-14 09:02:16.000000 mapel-core-2.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 09:02:34.121503 mapel-core-2.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:34.117503 mapel-core-2.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:34.117503 mapel-core-2.0.6/src/mapel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:34.117503 mapel-core-2.0.6/src/mapel/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:34.117503 mapel-core-2.0.6/src/mapel/core/embedding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/embedding/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/embedding/initial_positions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:34.117503 mapel-core-2.0.6/src/mapel/core/embedding/kamada_kawai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/embedding/kamada_kawai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/embedding/kamada_kawai/energy_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/embedding/kamada_kawai/kamada_kawai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/embedding/kamada_kawai/optimization_algorithms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:34.117503 mapel-core-2.0.6/src/mapel/core/embedding/simulated_annealing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/embedding/simulated_annealing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/embedding/simulated_annealing/simulated_annealing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/embedding/simulated_annealing/simulated_annealing_energy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:34.121503 mapel-core-2.0.6/src/mapel/core/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/features/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/features/distortion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/features/mallows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/features/monotonicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/features/stability.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/features_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/glossary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/inner_distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/matchings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:34.121503 mapel-core-2.0.6/src/mapel/core/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)    16676 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/objects/Experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/objects/Family.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/objects/Instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:34.121503 mapel-core-2.0.6/src/mapel/core/persistence/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/persistence/experiment_exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/persistence/experiment_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62429 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-14 09:02:16.000000 mapel-core-2.0.6/src/mapel/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:02:34.121503 mapel-core-2.0.6/src/mapel_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-14 09:02:34.000000 mapel-core-2.0.6/src/mapel_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-14 09:02:34.000000 mapel-core-2.0.6/src/mapel_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 09:02:34.000000 mapel-core-2.0.6/src/mapel_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-14 09:02:34.000000 mapel-core-2.0.6/src/mapel_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 09:02:34.000000 mapel-core-2.0.6/src/mapel_core.egg-info/top_level.txt
```

### Comparing `mapel-core-2.0.5/LICENSE.txt` & `mapel-core-2.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.5/PKG-INFO` & `mapel-core-2.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-core
-Version: 2.0.5
+Version: 2.0.6
 Summary: Map of Elections---essential parts
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>, Andrzej Kaczmarczyk <andrzej.kaczmarczyk@agh.edu.pl>, Kasper Sapala <kasper.sapala@gmail.com>, Tomasz Was <tomasz.t.was@gmail.com>
 License: Copyright (c) 2018-2022 Stanisław Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-core-2.0.5/README.md` & `mapel-core-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.5/pyproject.toml` & `mapel-core-2.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65", "wheel", "pybind11>=2.6.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mapel-core"
-version = "2.0.5"
+version = "2.0.6"
 authors = [
  {name = "Stanislaw Szufa", email = "s.szufa@gmail.com"},
  {name = "Niclas Boehmer", email = "niclas.boehmer@tu-berlin.de"},
  {name = "Andrzej Kaczmarczyk", email = "andrzej.kaczmarczyk@agh.edu.pl"},
  {name = "Kasper Sapala", email = "kasper.sapala@gmail.com"},
  {name = "Tomasz Was", email = "tomasz.t.was@gmail.com"},
 ]
```

### Comparing `mapel-core-2.0.5/src/mapel/core/embedding/initial_positions.py` & `mapel-core-2.0.6/src/mapel/core/embedding/initial_positions.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.5/src/mapel/core/embedding/kamada_kawai/energy_functions.py` & `mapel-core-2.0.6/src/mapel/core/embedding/kamada_kawai/energy_functions.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.5/src/mapel/core/embedding/kamada_kawai/kamada_kawai.py` & `mapel-core-2.0.6/src/mapel/core/embedding/kamada_kawai/kamada_kawai.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.5/src/mapel/core/embedding/kamada_kawai/optimization_algorithms.py` & `mapel-core-2.0.6/src/mapel/core/embedding/kamada_kawai/optimization_algorithms.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.5/src/mapel/core/embedding/simulated_annealing/simulated_annealing.py` & `mapel-core-2.0.6/src/mapel/core/embedding/simulated_annealing/simulated_annealing.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.5/src/mapel/core/embedding/simulated_annealing/simulated_annealing_energy.py` & `mapel-core-2.0.6/src/mapel/core/embedding/simulated_annealing/simulated_annealing_energy.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.5/src/mapel/core/features/common.py` & `mapel-core-2.0.6/src/mapel/core/features/common.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.5/src/mapel/core/features/distortion.py` & `mapel-core-2.0.6/src/mapel/core/features/distortion.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.5/src/mapel/core/features/monotonicity.py` & `mapel-core-2.0.6/src/mapel/core/features/monotonicity.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.5/src/mapel/core/features/stability.py` & `mapel-core-2.0.6/src/mapel/core/features/stability.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.5/src/mapel/core/features_main.py` & `mapel-core-2.0.6/src/mapel/core/features_main.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.5/src/mapel/core/glossary.py` & `mapel-core-2.0.6/src/mapel/core/glossary.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 MAIN_LOCAL_FEATUERS = []
 
 MAIN_GLOBAL_FEATUERS = ['distortion', 'monotonicity']
 
 ELECTION_GLOBAL_FEATURES = {'clustering', 'clustering_kmeans', 'distortion_from_all',
                             'id_vs_un', 'an_vs_st', }
 
-COLORS = ['blue', 'green', 'black', 'red', 'orange', 'purple', 'brown', 'lime', 'cyan', 'grey']
-
 RULE_NAME_MATRIX = {
     "av": "AV",
     "sav": "SAV",
     "pav": "PAV",
     "slav": "SLAV",
     "cc": "CC",
     "seqpav": "seq-PAV",
@@ -141,14 +139,18 @@
 'Norm-Mallows (uniform)': 'N-Mallows',
 'GS Balanced': 'GS (Bal.)',
 'GS Caterpillar': 'GS (Cat.)',
 'ID': 'ID',
 'AN': 'AN',
 'ST': 'ST',
 'UN': 'UN',
+'1D Uniform': '1D',
+'2D Uniform': '2D',
+'3D Uniform': '3D',
+'2D Sphere': 'Circle',
 }
 
 LIST_OF_PREFLIB_MODELS = {'sushi', 'irish', 'glasgow', 'skate', 'formula',
                           'tshirt', 'cities_survey', 'aspen', 'ers',
                           'marble', 'cycling_tdf', 'cycling_gdi',
                           'ice_races', 'grenoble', 'speed_skating',
                           'irish_bis', 'speed_skating_bis', 'skate_bis'}
@@ -160,43 +162,30 @@
                        'single-crossing_matrix', 'gs_caterpillar_matrix',
                        'norm-mallows_matrix', 'sushi_matrix',
                        'walsh_path', 'conitzer_path', 'from_approval'}
 
 PATHS = {'unid', 'stan', 'anid', 'stid', 'anun', 'stun',
          'mallows_matrix_path', 'walsh_path', 'conitzer_path', }
 
-PARTY_MODELS = {'2d_gaussian_party', '1d_gaussian_party', 'ic_party',
-                'walsh_party', 'conitzer_party', 'mallows_party'}
-
 APPROVAL_MODELS = {'impartial_culture', 'ic', 'resampling', 'id',
                    'empty', 'full', 'truncated_urn',
                    'urn', 'euclidean', 'noise',
                    'zeros', 'ones',
                    'id_0.5', 'ic_0.5',
                    'half_1', 'half_2', 'disjoint_resampling',
                    'simplex_resampling',
                    'vcr', 'truncated_mallows', 'moving_resampling',
                    'jaccard', 'skeleton', 'anti_pjr',
                    'partylist'}
 
 APPROVAL_FAKE_MODELS = {'approval_half_1', 'approval_half_2', 'approval_skeleton'}
 
-GRAPH_MODELS = {'erdos_renyi_graph', 'watts_strogatz_graph', 'barabasi_albert_graph',
-                'random_geometric_graph', 'random_tree',
-                'cycle_graph', 'wheel_graph', 'star_graph', 'ladder_graph', 'circular_ladder_graph',
-                'erdos_renyi_graph_path'}
 
-NOT_ABCVOTING_RULES = {'borda_c4', 'random'}
+NOT_ABCVOTING_RULES = {'borda_c4',
+                       'random'}
 
 EMBEDDING_RELATED_FEATURE = ['monotonicity_triplets', 'distortion_from_all']
 
-ROOMMATES_PROBLEM_MODELS = {'roommates_ic'}
-
-FEATURES_WITH_DISSAT = {'highest_cc_score', 'highest_hb_score', 'highest_pav_score',
-                        'greedy_approx_cc_score', 'removal_approx_cc_score',
-                        'greedy_approx_hb_score', 'removal_approx_hb_score',
-                        'greedy_approx_pav_score', 'removal_approx_pav_score',
-                        'banzhaf_cc_score', 'ranging_cc_score'}
 
 # # # # # # # # # # # # # # # #
 # LAST CLEANUP ON: 12.10.2021 #
 # # # # # # # # # # # # # # # #
```

### Comparing `mapel-core-2.0.5/src/mapel/core/inner_distances.py` & `mapel-core-2.0.6/src/mapel/core/inner_distances.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,16 +31,14 @@
 def wl1(vector_1: np.ndarray, vector_2: np.ndarray) -> float:
     """ Return: L1 distance """
     return sum([len(vector_1)-i*abs(vector_1[i] - vector_2[i]) for i in range(len(vector_1))])
 
 
 def l1(vector_1: np.ndarray, vector_2: np.ndarray) -> float:
     """ Return: L1 distance """
-    # vector_1 = np.ndarray(vector_1)
-    # vector_2 = np.ndarray(vector_2)
     return np.linalg.norm(vector_1 - vector_2, ord=1)
 
 
 def l2(vector_1: np.ndarray, vector_2: np.ndarray) -> float:
     """ Return: L2 distance """
     return np.linalg.norm(vector_1 - vector_2, ord=2)
```

### Comparing `mapel-core-2.0.5/src/mapel/core/objects/Family.py` & `mapel-core-2.0.6/src/mapel/core/objects/Family.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,54 +1,51 @@
 #!/usr/bin/env python
 
+
 class Family:
-    """ Family of elections: a set of elections from the same election culture_id """
+    """ Family of elections: a set of instances from the same culture """
 
     def __init__(self,
                  culture_id: str = None,
-                 family_id='none',
+                 family_id: str = 'none',
                  params: dict = None,
-                 # printing_params: dict = None,
                  size: int = 1,
                  label: str = None,
                  color: str = "black",
                  alpha: float = 1.,
                  ms: int = 20,
-                 show=True,
-                 marker='o',
+                 show: bool = True,
+                 marker: str = 'o',
                  starting_from: int = 0,
                  single: bool = False,
                  instance_ids: list = None,
                  path: dict = None,
                  **kwargs):
 
         if path is None:
             path = {}
-        if instance_ids is None:
-            instance_ids = {}
         if params is None:
             params = {}
-        # if printing_params is None:
-        #     printing_params = {}
         if label is None:
             label = family_id
+        if instance_ids is None:
+            instance_ids = {}
 
         self.family_id = family_id
         self.culture_id = culture_id
         self.params = params
-        # self.printing_params = params
         self.size = size
         self.label = label
         self.color = color
         self.alpha = alpha
         self.show = show
         self.marker = marker
         self.ms = ms
         self.starting_from = starting_from
         self.single = single
         self.path = path
         self.instance_ids = instance_ids
 
 
 # # # # # # # # # # # # # # # #
-# LAST CLEANUP ON: 12.10.2021 #
+# LAST CLEANUP ON: 11.07.2023 #
 # # # # # # # # # # # # # # # #
```

### Comparing `mapel-core-2.0.5/src/mapel/core/persistence/experiment_imports.py` & `mapel-core-2.0.6/src/mapel/core/persistence/experiment_imports.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import os
 
 import numpy as np
 from mapel.core.glossary import *
 
 
 # Distances
-def import_distances(experiment, distance_id):
+def import_distances_from_file(experiment, distance_id):
+    """ Import distances between each pair of instances from a file """
 
     distances = {}
 
     file_name = f'{distance_id}.csv'
     path = os.path.join(os.getcwd(), 'experiments', experiment.experiment_id,
                         'distances', file_name)
 
@@ -47,18 +48,23 @@
             except KeyError:
                 pass
 
     return distances
 
 
 def add_distances_to_experiment(experiment) -> (dict, dict, dict):
-    """ Import precomputed distances between each pair of instances from a file """
+    """ Import precomputed distances between each pair of instances from a file
+        while preparing an experiment """
     try:
         file_name = f'{experiment.distance_id}.csv'
-        path = os.path.join(os.getcwd(), 'experiments', experiment.experiment_id, 'distances', file_name)
+        path = os.path.join(os.getcwd(),
+                            'experiments',
+                            experiment.experiment_id,
+                            'distances',
+                            file_name)
 
         distances = {}
         times = {}
         stds = {}
         mappings = {}
         with open(path, 'r', newline='') as csv_file:
 
@@ -126,79 +132,63 @@
                 if instance_id_1 not in experiment.instances:
                     warn = True
 
             if warn:
                 text = f'Possibly outdated distances are imported!'
                 logging.warning(text)
 
-        print('=== Distances imported successfully! ===')
         return distances, times, stds, mappings
 
     except FileNotFoundError:
-        print('=== Distances not found! ===')
         return None, None, None, None
 
 
 # Features
 def get_values_from_csv_file(experiment, feature_id, feature_long_id=None,
                              upper_limit=np.infty,
                              lower_limit=-np.infty,
                              column_id='value') -> dict:
     """ Import values for a feature_id from a .csv file """
-    if feature_long_id is None:
-        feature_long_id = feature_id
 
-    if feature_id in EMBEDDING_RELATED_FEATURE:
-        path = os.path.join(os.getcwd(), "experiments", experiment.experiment_id,
-                            "features", f'{feature_long_id}.csv')
-    else:
-        path = os.path.join(os.getcwd(), "experiments", experiment.experiment_id,
-                            "features", f'{feature_long_id}.csv')
+    feature_long_id = feature_id if feature_long_id is None else feature_long_id
+
+    path = os.path.join(os.getcwd(), "experiments", experiment.experiment_id, "features",
+                        f'{feature_long_id}.csv')
+
     values = {}
     with open(path, 'r', newline='') as csv_file:
         reader = csv.DictReader(csv_file, delimiter=';')
 
         for row in reader:
-            try:
-                election_id = row['instance_id']
-            except:
-                try:
-                    election_id = row['election_id']
-                except:
-                    pass
+            election_id = row.get('instance_id', row.get('election_id'))
             value = row[column_id]
-            if value == 'None' or value is None:
-                value = None
-            elif column_id == 'time' and float(value) == 0.:
-                value = None
-            else:
-                value = float(value)
-                if value >= upper_limit:
-                    value = upper_limit
-                if value <= lower_limit:
-                    value = lower_limit
 
-            values[election_id] = value
+            if value in {'None', 'Blank'} or column_id == 'time' and float(value) == 0.:
+                values[election_id] = None
+                continue
+
+            value = float(value)
+            values[election_id] = min(max(value, lower_limit), upper_limit)
 
     return values
 
 
 # Coordinates
 def add_coordinates_to_experiment(experiment, dim=2, file_name=None) -> dict:
     """ Import from a file precomputed coordinates of all the points --
-    each point refer to one instance """
+        each point refer to one instance """
 
     coordinates = {}
     if file_name is None:
         file_name = f'{experiment.embedding_id}_{experiment.distance_id}_{dim}d.csv'
     path = os.path.join(os.getcwd(), "experiments", experiment.experiment_id,
                         "coordinates", file_name)
+
     with open(path, 'r', newline='') as csv_file:
 
-        # ORIGINAL
         reader = csv.DictReader(csv_file, delimiter=';')
 
         warn = False
 
         for row in reader:
             try:
                 instance_id = row['instance_id']
@@ -219,7 +209,11 @@
                 warn = True
 
         if warn:
             text = f'Possibly outdated coordinates are imported!'
             logging.warning(text)
 
     return coordinates
+
+# # # # # # # # # # # # # # # #
+# LAST CLEANUP ON: 11.07.2023 #
+# # # # # # # # # # # # # # # #
```

### Comparing `mapel-core-2.0.5/src/mapel/core/printing.py` & `mapel-core-2.0.6/src/mapel/core/printing.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,26 +10,14 @@
 except ImportError:
     tikzplotlib = None
 
 from mapel.core.glossary import *
 import mapel.core.persistence.experiment_imports as imports
 
 
-def print_approvals_histogram(election):
-    plt.title(election.election_id, size=20)
-    bins = np.linspace(0, 100, 51)
-    plt.hist([len(vote) for vote in election.votes], bins=bins)
-    # x_axis = np.arange(0, 100, 0.01)
-    # plt.plot(x_axis, norm.pdf(x_axis, 50, 2)*2000)
-    plt.ylim([0, election.num_voters])
-    plt.xlim([-1, election.num_candidates + 1])
-    plt.savefig("images/histograms/" + election.election_id + ".png")
-    plt.show()
-
-
 # New 1d map printing
 def print_map_1d(experiment, saveas=None):
     experiment.compute_coordinates_by_families()
     all_values = [0]
     for family in experiment.families.values():
         x = float(experiment.coordinates_by_families[family.family_id][0][0])
         all_values.append(x)
@@ -51,15 +39,14 @@
     # plt.axis("off")
     if saveas:
         plt.savefig(saveas)
     plt.show()
 
 
 # Main functions
-#DIV-MERGE
 def print_map_2d(experiment,
                  xlabel=None,
                  shading=False,
                  legend_pos=None,
                  title_pos=None,
                  angle=0,
                  reverse=False,
@@ -150,15 +137,16 @@
                                     feature_labelsize=14,
                                     dpi=250,
                                     title_size=16,
                                     ticks_pos=None,
                                     omit=None,
                                     textual_size=16,
                                     figsize=(6.4, 6.4),
-                                    strech=None) -> None:
+                                    strech=None,
+                                    colors=None) -> None:
     if textual is None:
         textual = []
 
     if omit is None:
         omit = []
 
     experiment.compute_coordinates_by_families()
@@ -180,15 +168,16 @@
                                               upper_limit=upper_limit,
                                               lower_limit=lower_limit,
                                               scale=scale,
                                               xticklabels=xticklabels, ms=ms, cmap=cmap,
                                               omit=omit,
                                               ticks=ticks, column_id=column_id,
                                               feature_labelsize=feature_labelsize,
-                                              strech=strech)
+                                              strech=strech,
+                                              colors=colors)
     _add_textual(experiment=experiment, textual=textual, ax=ax, size=textual_size,
                  shades_dict=shades_dict, cmap=cmap, column_id=column_id, feature_id=feature_id)
 
     # BACKGROUND
     _basic_background(ax=ax, legend=False,
                       saveas=saveas, xlabel=xlabel, bbox_inches=bbox_inches,
                       title=title, legend_pos=legend_pos, title_size=title_size,
@@ -358,15 +347,15 @@
 
 
 def _import_values_for_feature(experiment, feature_id=None, upper_limit=None,
                                lower_limit=None, normalizing_func=None,
                                marker_func=None, dim=2, column_id='value', omit=None,
                                scale='default'):
     """ Import values for a feature_id """
-
+    print(upper_limit)
     if isinstance(feature_id, str):
         if feature_id in experiment.features:
             values = experiment.features[feature_id][column_id]
             if column_id == 'time':
                 values = {k: convert_none_time(v) for k, v in values.items()}
             else:
                 values = {k: convert_none(v) for k, v in values.items()}
@@ -389,14 +378,15 @@
     _max = max(x for x in values.values() if x is not None)
 
     shades = []
     xx = []
     yy = []
     zz = []
     markers = []
+    none_xx, none_yy = [], []
     blank_xx, blank_yy = [], []
 
     ctr = 0
 
     my_shade = {}
     for family_id in experiment.families:
         for k in range(experiment.families[family_id].size):
@@ -622,24 +612,27 @@
 
 
 def _color_map_by_feature(experiment=None, fig=None, ax=None, feature_id=None,
                           upper_limit=np.infty, lower_limit=-np.infty,
                           normalizing_func=None, marker_func=None, xticklabels=None, ms=None,
                           cmap=None, ticks=None, dim=2, rounding=1, column_id='value',
                           feature_labelsize=14, ticks_pos=None, omit=None, scale='default',
-                          strech=None):
+                          strech=None, colors=None):
     xx, yy, zz, shades, markers, mses, _min, _max, blank_xx, blank_yy, names = \
         _import_values_for_feature(
             experiment, feature_id=feature_id, upper_limit=upper_limit, lower_limit=lower_limit,
             normalizing_func=normalizing_func,
             marker_func=marker_func, dim=dim, column_id=column_id, omit=omit, scale=scale)
 
     vmin = 0
     vmax = 1
     # strech=[1.0,2.0]
+    print(strech)
+    print(_min)
+    print(_max)
     if strech is not None:
         length = _max - _min
         vmin = 0 - (_min - strech[0]) / length
         vmax = 1 + (strech[1] - _max) / length
     print(vmin, vmax)
 
     unique_markers = set(markers)
@@ -650,15 +643,18 @@
 
     if cmap is None:
         if rounding == 0:
             num_colors = int(min(_max - _min + 1, 101))
             if num_colors < 10:
                 xticklabels = [str(q) for q in range(num_colors)]
                 ticks_pos = [(2 * q + 1) / num_colors / 2 for q in range(num_colors)]
-            cmap = custom_div_cmap(num_colors=num_colors)
+            if colors is None:
+                cmap = custom_div_cmap(num_colors=num_colors)
+            else:
+                cmap = custom_div_cmap(colors=colors, num_colors=num_colors)
         else:
             cmap = custom_div_cmap()
 
     for um in unique_markers:
         masks = (markers == um)
         if um == '.':
             images.append(ax.scatter(xx[masks], yy[masks],
@@ -973,15 +969,15 @@
                     color = (0.75 - 0.75 * alpha + 0.125 * tint + 0.875 * alpha * tint,
                              0.75 - 0.75 * alpha,
                              0.75 - 0.75 * alpha + 0.125 * (1 - tint) + 0.875 * alpha * (1- tint))
                     alpha = 1
 
                 elif 'Urn' in label:
 
-                    color, alpha = get_color_alpha_for_urn(color, alpha, urn_orangered)
+                    color, alpha = get_color_alpha_for_urn(alpha, urn_orangered)
 
                 else:
 
                     if alpha is None or alpha > 1:
                         alpha = 1
 
                     if '1D _path' in label:
@@ -1055,15 +1051,15 @@
         pass
     file_name = saveas + ".tex"
     path = os.path.join(os.getcwd(), "images", "tex", file_name)
     tikzplotlib.save(path)
 
 
 # MAIN FUNCTIONS
-def print_matrix(experiment=None, scale=1., rounding=1, distance_name='',
+def print_matrix(experiment=None, scale=1., rounding=1,
                  saveas=None, show=True, ms=8, title=None, omit=None,
                  self_distances=False, yticks='left', with_std=False, time=False, dpi=100,
                  vmin=None, vmax=None):
     """Print the matrix with average distances between each pair of election """
 
     if omit is None:
         omit = []
@@ -1640,19 +1636,18 @@
         alpha = math.atan(d_x / d_y)
         experiment.rotate(alpha)
         if experiment.coordinates['all_0'][1] < experiment.coordinates['all_1'][1]:
             experiment.rotate(math.pi)
     except:
         print('Cannot adjust!')
 
-#DIV-MERGE
-def get_color_alpha_for_urn(color, alpha, orangered=True):
-    # return 'red', min(alpha, 1)
 
-    if orangered:
+def get_color_alpha_for_urn(alpha, urn_orangered=True):
+
+    if urn_orangered:
         if alpha > 1.07:
             return 'red', 0.9
         elif alpha > 0.53:
             return 'orangered', 0.9
         elif alpha > 0.22:
             return 'orange', 0.9
         else:
```

### Comparing `mapel-core-2.0.5/src/mapel/core/utils.py` & `mapel-core-2.0.6/src/mapel/core/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 
-
 def make_folder_if_do_not_exist(path):
     is_exist = os.path.exists(path)
     if not is_exist:
         os.makedirs(path)
 
 def is_module_loaded(module_import_name):
    '''
```

### Comparing `mapel-core-2.0.5/src/mapel_core.egg-info/PKG-INFO` & `mapel-core-2.0.6/src/mapel_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-core
-Version: 2.0.5
+Version: 2.0.6
 Summary: Map of Elections---essential parts
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>, Andrzej Kaczmarczyk <andrzej.kaczmarczyk@agh.edu.pl>, Kasper Sapala <kasper.sapala@gmail.com>, Tomasz Was <tomasz.t.was@gmail.com>
 License: Copyright (c) 2018-2022 Stanisław Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-core-2.0.5/src/mapel_core.egg-info/SOURCES.txt` & `mapel-core-2.0.6/src/mapel_core.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -6,25 +6,27 @@
 src/mapel/core/features_main.py
 src/mapel/core/glossary.py
 src/mapel/core/inner_distances.py
 src/mapel/core/matchings.py
 src/mapel/core/printing.py
 src/mapel/core/utils.py
 src/mapel/core/embedding/__init__.py
+src/mapel/core/embedding/embed.py
 src/mapel/core/embedding/initial_positions.py
 src/mapel/core/embedding/kamada_kawai/__init__.py
 src/mapel/core/embedding/kamada_kawai/energy_functions.py
 src/mapel/core/embedding/kamada_kawai/kamada_kawai.py
 src/mapel/core/embedding/kamada_kawai/optimization_algorithms.py
 src/mapel/core/embedding/simulated_annealing/__init__.py
 src/mapel/core/embedding/simulated_annealing/simulated_annealing.py
 src/mapel/core/embedding/simulated_annealing/simulated_annealing_energy.py
 src/mapel/core/features/__init__.py
 src/mapel/core/features/common.py
 src/mapel/core/features/distortion.py
+src/mapel/core/features/mallows.py
 src/mapel/core/features/monotonicity.py
 src/mapel/core/features/stability.py
 src/mapel/core/objects/Experiment.py
 src/mapel/core/objects/Family.py
 src/mapel/core/objects/Instance.py
 src/mapel/core/objects/__init__.py
 src/mapel/core/persistence/__init__.py
```

