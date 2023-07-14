# Comparing `tmp/SMACT-2.5.1.tar.gz` & `tmp/SMACT-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SMACT-2.5.1.tar", last modified: Tue May  2 12:17:57 2023, max compression
+gzip compressed data, was "SMACT-2.5.2.tar", last modified: Fri Jul 14 15:25:14 2023, max compression
```

## Comparing `SMACT-2.5.1.tar` & `SMACT-2.5.2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:17:57.055828 SMACT-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-02 12:17:42.000000 SMACT-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-02 12:17:42.000000 SMACT-2.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12439 2023-05-02 12:17:57.055828 SMACT-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11531 2023-05-02 12:17:42.000000 SMACT-2.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:17:57.043828 SMACT-2.5.1/SMACT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12439 2023-05-02 12:17:57.000000 SMACT-2.5.1/SMACT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-02 12:17:57.000000 SMACT-2.5.1/SMACT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 12:17:57.000000 SMACT-2.5.1/SMACT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 12:17:56.000000 SMACT-2.5.1/SMACT.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-02 12:17:57.000000 SMACT-2.5.1/SMACT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 12:17:57.000000 SMACT-2.5.1/SMACT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-02 12:17:42.000000 SMACT-2.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 12:17:57.055828 SMACT-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-02 12:17:42.000000 SMACT-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:17:57.047828 SMACT-2.5.1/smact/
--rw-r--r--   0 runner    (1001) docker     (123)    17669 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:17:57.051828 SMACT-2.5.1/smact/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data/Covalent_radii.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data/HHIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data/SSE.csv
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data/SSE_2015.csv
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data/SSE_Pauling.csv
--rw-r--r--   0 runner    (1001) docker     (123)    17321 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data/element_data.txt
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data/ionic_radii.csv
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data/ordered_periodic.txt
--rw-r--r--   0 runner    (1001) docker     (123)    37149 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data/oxidation_state_probability_table.json
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data/oxidation_states.txt
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data/oxidation_states_SP.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data/oxidation_states_icsd.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data/oxidation_states_pmg.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data/oxidation_states_wiki.txt
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data/oxidationstates.data
--rw-r--r--   0 runner    (1001) docker     (123)    11433 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data/shannon_radii.csv
--rw-r--r--   0 runner    (1001) docker     (123)    29754 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data/shannon_radii_ML_extended.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data/solid_properties.txt
--rw-r--r--   0 runner    (1001) docker     (123)    43658 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data/solid_properties.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    24651 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/distorter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:17:57.051828 SMACT-2.5.1/smact/dopant_prediction/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/dopant_prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/dopant_prediction/doper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1587 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/lattice_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/mainpage.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/oxidation_states.py
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    15175 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/screening.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:17:57.055828 SMACT-2.5.1/smact/structure_prediction/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/structure_prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9573 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/structure_prediction/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    14853 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/structure_prediction/mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10052 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/structure_prediction/prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/structure_prediction/probability_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    22383 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/structure_prediction/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/structure_prediction/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:17:57.055828 SMACT-2.5.1/smact/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12333 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/tests/test_doper.py
--rw-r--r--   0 runner    (1001) docker     (123)    22153 2023-05-02 12:17:42.000000 SMACT-2.5.1/smact/tests/test_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:25:14.678125 SMACT-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-14 15:25:06.000000 SMACT-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-14 15:25:06.000000 SMACT-2.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12331 2023-07-14 15:25:14.678125 SMACT-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11423 2023-07-14 15:25:06.000000 SMACT-2.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:25:14.674126 SMACT-2.5.2/SMACT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12331 2023-07-14 15:25:14.000000 SMACT-2.5.2/SMACT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-14 15:25:14.000000 SMACT-2.5.2/SMACT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 15:25:14.000000 SMACT-2.5.2/SMACT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 15:25:14.000000 SMACT-2.5.2/SMACT.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-14 15:25:14.000000 SMACT-2.5.2/SMACT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 15:25:14.000000 SMACT-2.5.2/SMACT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-14 15:25:06.000000 SMACT-2.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 15:25:14.678125 SMACT-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-14 15:25:06.000000 SMACT-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:25:14.674126 SMACT-2.5.2/smact/
+-rw-r--r--   0 runner    (1001) docker     (123)    17669 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:25:14.678125 SMACT-2.5.2/smact/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/data/Covalent_radii.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/data/HHIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/data/SSE.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/data/SSE_2015.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/data/SSE_Pauling.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    17321 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/data/element_data.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/data/ionic_radii.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/data/ordered_periodic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    37149 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/data/oxidation_state_probability_table.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/data/oxidation_states.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/data/oxidation_states_SP.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/data/oxidation_states_icsd.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/data/oxidation_states_pmg.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/data/oxidation_states_wiki.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/data/oxidationstates.data
+-rw-r--r--   0 runner    (1001) docker     (123)    11433 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/data/shannon_radii.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    29754 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/data/shannon_radii_ML_extended.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/data/solid_properties.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    43658 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/data/solid_properties.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    24651 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/distorter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:25:14.678125 SMACT-2.5.2/smact/dopant_prediction/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/dopant_prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/dopant_prediction/doper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1587 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/lattice_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/mainpage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/oxidation_states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15276 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/screening.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:25:14.678125 SMACT-2.5.2/smact/structure_prediction/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/structure_prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9573 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/structure_prediction/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14864 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/structure_prediction/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10052 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/structure_prediction/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/structure_prediction/probability_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22383 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/structure_prediction/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/structure_prediction/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:25:14.678125 SMACT-2.5.2/smact/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13099 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/tests/test_doper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22159 2023-07-14 15:25:06.000000 SMACT-2.5.2/smact/tests/test_structure.py
```

### Comparing `SMACT-2.5.1/LICENSE` & `SMACT-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.1/PKG-INFO` & `SMACT-2.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SMACT
-Version: 2.5.1
+Version: 2.5.2
 Summary: Semiconducting Materials by Analogy and Chemical Theory
 Home-page: https://github.com/WMD-group/SMACT
 Author: Daniel W. Davies
 Author-email: d.w.davies@imperial.ac.uk
 Maintainer: Anthony O. Onwuli
 Maintainer-email: anthony.onwuli16@imperial.ac.uk
 License: MIT
@@ -18,28 +18,26 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![DOI](http://joss.theoj.org/papers/10.21105/joss.01361/status.svg)](https://doi.org/10.21105/joss.01361)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5553202.svg)](https://doi.org/10.5281/zenodo.5553202)
 [![Documentation Status](https://readthedocs.org/projects/smact/badge/?version=latest)](http://smact.readthedocs.org/en/latest/?badge=latest)
-[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![DOI](http://joss.theoj.org/papers/10.21105/joss.01361/status.svg)](https://doi.org/10.21105/joss.01361)
+![python version](https://img.shields.io/pypi/pyversions/smact)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPi](https://img.shields.io/pypi/v/smact)](https://pypi.org/project/SMACT/)
 [![GitHub issues](https://img.shields.io/github/issues-raw/WMD-Group/SMACT)](https://github.com/WMD-group/SMACT/issues)
 ![dependencies](https://img.shields.io/librariesio/release/pypi/smact)
 [![CI Status](https://github.com/WMD-group/SMACT/actions/workflows/ci.yml/badge.svg)](https://github.com/WMD-group/SMACT/actions/workflows/ci.yml)
-![python version](https://img.shields.io/pypi/pyversions/smact)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/smact)
 [![codecov](https://codecov.io/gh/WMD-group/SMACT/branch/master/graph/badge.svg?token=UtgVxjoYNP)](https://codecov.io/gh/WMD-group/SMACT)
-
+![PyPI - Downloads](https://img.shields.io/pypi/dm/smact)
 
 SMACT
 =====
 
 **Semiconducting Materials from Analogy and Chemical Theory** (SMACT) is a collection of rapid screening tools that uses data about chemical elements.
 
 - **Documentation:** https://smact.readthedocs.io/en/latest/
```

### Comparing `SMACT-2.5.1/README.md` & `SMACT-2.5.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,19 @@
+[![DOI](http://joss.theoj.org/papers/10.21105/joss.01361/status.svg)](https://doi.org/10.21105/joss.01361)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5553202.svg)](https://doi.org/10.5281/zenodo.5553202)
 [![Documentation Status](https://readthedocs.org/projects/smact/badge/?version=latest)](http://smact.readthedocs.org/en/latest/?badge=latest)
-[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![DOI](http://joss.theoj.org/papers/10.21105/joss.01361/status.svg)](https://doi.org/10.21105/joss.01361)
+![python version](https://img.shields.io/pypi/pyversions/smact)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPi](https://img.shields.io/pypi/v/smact)](https://pypi.org/project/SMACT/)
 [![GitHub issues](https://img.shields.io/github/issues-raw/WMD-Group/SMACT)](https://github.com/WMD-group/SMACT/issues)
 ![dependencies](https://img.shields.io/librariesio/release/pypi/smact)
 [![CI Status](https://github.com/WMD-group/SMACT/actions/workflows/ci.yml/badge.svg)](https://github.com/WMD-group/SMACT/actions/workflows/ci.yml)
-![python version](https://img.shields.io/pypi/pyversions/smact)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/smact)
 [![codecov](https://codecov.io/gh/WMD-group/SMACT/branch/master/graph/badge.svg?token=UtgVxjoYNP)](https://codecov.io/gh/WMD-group/SMACT)
-
+![PyPI - Downloads](https://img.shields.io/pypi/dm/smact)
 
 SMACT
 =====
 
 **Semiconducting Materials from Analogy and Chemical Theory** (SMACT) is a collection of rapid screening tools that uses data about chemical elements.
 
 - **Documentation:** https://smact.readthedocs.io/en/latest/
```

### Comparing `SMACT-2.5.1/SMACT.egg-info/PKG-INFO` & `SMACT-2.5.2/SMACT.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SMACT
-Version: 2.5.1
+Version: 2.5.2
 Summary: Semiconducting Materials by Analogy and Chemical Theory
 Home-page: https://github.com/WMD-group/SMACT
 Author: Daniel W. Davies
 Author-email: d.w.davies@imperial.ac.uk
 Maintainer: Anthony O. Onwuli
 Maintainer-email: anthony.onwuli16@imperial.ac.uk
 License: MIT
@@ -18,28 +18,26 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![DOI](http://joss.theoj.org/papers/10.21105/joss.01361/status.svg)](https://doi.org/10.21105/joss.01361)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5553202.svg)](https://doi.org/10.5281/zenodo.5553202)
 [![Documentation Status](https://readthedocs.org/projects/smact/badge/?version=latest)](http://smact.readthedocs.org/en/latest/?badge=latest)
-[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![DOI](http://joss.theoj.org/papers/10.21105/joss.01361/status.svg)](https://doi.org/10.21105/joss.01361)
+![python version](https://img.shields.io/pypi/pyversions/smact)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPi](https://img.shields.io/pypi/v/smact)](https://pypi.org/project/SMACT/)
 [![GitHub issues](https://img.shields.io/github/issues-raw/WMD-Group/SMACT)](https://github.com/WMD-group/SMACT/issues)
 ![dependencies](https://img.shields.io/librariesio/release/pypi/smact)
 [![CI Status](https://github.com/WMD-group/SMACT/actions/workflows/ci.yml/badge.svg)](https://github.com/WMD-group/SMACT/actions/workflows/ci.yml)
-![python version](https://img.shields.io/pypi/pyversions/smact)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/smact)
 [![codecov](https://codecov.io/gh/WMD-group/SMACT/branch/master/graph/badge.svg?token=UtgVxjoYNP)](https://codecov.io/gh/WMD-group/SMACT)
-
+![PyPI - Downloads](https://img.shields.io/pypi/dm/smact)
 
 SMACT
 =====
 
 **Semiconducting Materials from Analogy and Chemical Theory** (SMACT) is a collection of rapid screening tools that uses data about chemical elements.
 
 - **Documentation:** https://smact.readthedocs.io/en/latest/
```

### Comparing `SMACT-2.5.1/SMACT.egg-info/SOURCES.txt` & `SMACT-2.5.2/SMACT.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.1/setup.py` & `SMACT-2.5.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python
 
 __author__ = "Daniel W. Davies"
 __author_email__ = "d.w.davies@imperial.ac.uk"
 __copyright__ = (
     "Copyright Daniel W. Davies, Adam J. Jackson, Keith T. Butler (2019)"
 )
-__version__ = "2.5.1"
+__version__ = "2.5.2"
 __maintainer__ = "Anthony O. Onwuli"
 __maintaier_email__ = "anthony.onwuli16@imperial.ac.uk"
-__date__ = "May 2 2023"
+__date__ = "July 13 2023"
 
 import os
 import unittest
 
 from setuptools import Extension, setup
 
 module_dir = os.path.dirname(os.path.abspath(__file__))
```

### Comparing `SMACT-2.5.1/smact/__init__.py` & `SMACT-2.5.2/smact/__init__.py`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.1/smact/builder.py` & `SMACT-2.5.2/smact/builder.py`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.1/smact/data/Covalent_radii.csv` & `SMACT-2.5.2/smact/data/Covalent_radii.csv`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.1/smact/data/HHIs.txt` & `SMACT-2.5.2/smact/data/HHIs.txt`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.1/smact/data/SSE.csv` & `SMACT-2.5.2/smact/data/SSE.csv`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.1/smact/data/SSE_2015.csv` & `SMACT-2.5.2/smact/data/SSE_2015.csv`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.1/smact/data/SSE_Pauling.csv` & `SMACT-2.5.2/smact/data/SSE_Pauling.csv`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.1/smact/data/element_data.txt` & `SMACT-2.5.2/smact/data/element_data.txt`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.1/smact/data/ionic_radii.csv` & `SMACT-2.5.2/smact/data/ionic_radii.csv`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.1/smact/data/oxidation_state_probability_table.json` & `SMACT-2.5.2/smact/data/oxidation_state_probability_table.json`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.1/smact/data/oxidation_states.txt` & `SMACT-2.5.2/smact/data/oxidation_states.txt`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.1/smact/data/oxidation_states_SP.txt` & `SMACT-2.5.2/smact/data/oxidation_states_SP.txt`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.1/smact/data/oxidation_states_icsd.txt` & `SMACT-2.5.2/smact/data/oxidation_states_icsd.txt`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.1/smact/data/oxidation_states_pmg.txt` & `SMACT-2.5.2/smact/data/oxidation_states_pmg.txt`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.1/smact/data/oxidation_states_wiki.txt` & `SMACT-2.5.2/smact/data/oxidation_states_wiki.txt`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.1/smact/data/oxidationstates.data` & `SMACT-2.5.2/smact/data/oxidationstates.data`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.1/smact/data/shannon_radii.csv` & `SMACT-2.5.2/smact/data/shannon_radii.csv`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.1/smact/data/shannon_radii_ML_extended.csv` & `SMACT-2.5.2/smact/data/shannon_radii_ML_extended.csv`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.1/smact/data/solid_properties.txt` & `SMACT-2.5.2/smact/data/solid_properties.txt`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.1/smact/data/solid_properties.xlsx` & `SMACT-2.5.2/smact/data/solid_properties.xlsx`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.1/smact/data_loader.py` & `SMACT-2.5.2/smact/data_loader.py`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.1/smact/distorter.py` & `SMACT-2.5.2/smact/distorter.py`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.1/smact/dopant_prediction/doper.py` & `SMACT-2.5.2/smact/dopant_prediction/doper.py`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.1/smact/lattice.py` & `SMACT-2.5.2/smact/lattice.py`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.1/smact/lattice_parameters.py` & `SMACT-2.5.2/smact/lattice_parameters.py`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.1/smact/oxidation_states.py` & `SMACT-2.5.2/smact/oxidation_states.py`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.1/smact/properties.py` & `SMACT-2.5.2/smact/properties.py`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.1/smact/screening.py` & `SMACT-2.5.2/smact/screening.py`

 * *Files 6% similar despite different names*

```diff
@@ -309,48 +309,50 @@
 
 def smact_filter(
     els: Union[Tuple[Element], List[Element]],
     threshold: Optional[int] = 8,
     stoichs: Optional[List[List[int]]] = None,
     species_unique: bool = True,
     oxidation_states_set: str = "default",
+    comp_tuple: bool = False,
 ) -> Union[List[Tuple[str, int, int]], List[Tuple[str, int]]]:
     """Function that applies the charge neutrality and electronegativity
     tests in one go for simple application in external scripts that
     wish to apply the general 'smact test'.
 
     Args:
         els (tuple/list): A list of smact.Element objects
         threshold (int): Threshold for stoichiometry limit, default = 8
         stoichs (list[int]): A selection of valid stoichiometric ratios for each site.
         species_unique (bool): Whether or not to consider elements in different oxidation states as unique in the results.
         oxidation_states_set (string): A string to choose which set of oxidation states should be chosen. Options are 'default', 'icsd', 'pymatgen' and 'wiki' for the default, icsd, pymatgen structure predictor and Wikipedia (https://en.wikipedia.org/wiki/Template:List_of_oxidation_states_of_the_elements) oxidation states respectively.
+        comp_tuple (bool): Whether or not to return the results as a named tuple of elements and stoichiometries (True) or as a normal tuple of elements and stoichiometries (False).
     Returns:
         allowed_comps (list): Allowed compositions for that chemical system
         in the form [(elements), (oxidation states), (ratios)] if species_unique=True
         or in the form [(elements), (ratios)] if species_unique=False.
 
     Example usage:
         >>> from smact.screening import smact_filter
         >>> from smact import Element
         >>> els = (Element('Cs'), Element('Pb'), Element('I'))
         >>> comps = smact_filter(els, threshold =5 )
         >>> for comp in comps:
         >>>     print(comp)
-        Composition(element_symbols=('Cs', 'Pb', 'I'), oxidation_states=(1, -4, -1), stoichiometries=(5, 1, 1))
-        Composition(element_symbols=('Cs', 'Pb', 'I'), oxidation_states=(1, 2, -1), stoichiometries=(1, 1, 3))
-        Composition(element_symbols=('Cs', 'Pb', 'I'), oxidation_states=(1, 2, -1), stoichiometries=(1, 2, 5))
-        Composition(element_symbols=('Cs', 'Pb', 'I'), oxidation_states=(1, 2, -1), stoichiometries=(2, 1, 4))
-        Composition(element_symbols=('Cs', 'Pb', 'I'), oxidation_states=(1, 2, -1), stoichiometries=(3, 1, 5))
-        Composition(element_symbols=('Cs', 'Pb', 'I'), oxidation_states=(1, 4, -1), stoichiometries=(1, 1, 5))
+        [('Cs', 'Pb', 'I'), (1, -4, -1), (5, 1, 1)]
+        [('Cs', 'Pb', 'I'), (1, 2, -1), (1, 1, 3)]
+        [('Cs', 'Pb', 'I'), (1, 2, -1), (1, 2, 5)]
+        [('Cs', 'Pb', 'I'), (1, 2, -1), (2, 1, 4)]
+        [('Cs', 'Pb', 'I'), (1, 2, -1), (3, 1, 5)]
+        [('Cs', 'Pb', 'I'), (1, 4, -1), (1, 1, 5)]
 
     Example (using stoichs):
         >>> from smact.screening import smact_filter
         >>> from smact import Element
-        >>> comps = smact_filter(els, stoichs = [[1],[1],[3]] )
+        >>> comps = smact_filter(els, stoichs = [[1],[1],[3]], comp_tuple=True )
         >>> for comp in comps:
         >>>     print(comp)
         Composition(element_symbols=('Cs', 'Pb', 'I'), oxidation_states=(1, 2, -1), stoichiometries=(1, 1, 3))
 
 
     """
 
@@ -389,19 +391,25 @@
         # Electronegativity test
         if cn_e:
             electroneg_OK = pauling_test(ox_states, electronegs)
             if electroneg_OK:
                 for ratio in cn_r:
                     compositions.append(
                         _allowed_compositions(symbols, ox_states, ratio)
+                        if comp_tuple
+                        else (symbols, ox_states, ratio)
                     )
 
     # Return list depending on whether we are interested in unique species combinations
     # or just unique element combinations.
     if species_unique:
         return compositions
     else:
-        compositions = [
-            _allowed_compositions_nonunique(i[0], i[2]) for i in compositions
-        ]
+        if comp_tuple:
+            compositions = [
+                _allowed_compositions_nonunique(i[0], i[2])
+                for i in compositions
+            ]
+        else:
+            compositions = [(i[0], i[2]) for i in compositions]
         compositions = list(set(compositions))
         return compositions
```

### Comparing `SMACT-2.5.1/smact/structure_prediction/database.py` & `SMACT-2.5.2/smact/structure_prediction/database.py`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.1/smact/structure_prediction/mutation.py` & `SMACT-2.5.2/smact/structure_prediction/mutation.py`

 * *Files 0% similar despite different names*

```diff
@@ -335,15 +335,15 @@
         corr = self.complete_sub_probs()
 
         # Sum each row (symmetry means this is the same as column sums)
         sums = corr.sum(axis=0)
         # Stack into matrix
         mat_sums = np.vstack([sums] * len(sums))
         # Make each element the product of (row_sum * col_sum)
-        mat_sums *= sums[:, None]
+        mat_sums *= sums.to_numpy()[:, None]
 
         corr /= mat_sums
 
         return corr
 
     def same_spec_probs(self) -> pd.Series:
         """Calculate the same species substiution probabilities."""
```

### Comparing `SMACT-2.5.1/smact/structure_prediction/prediction.py` & `SMACT-2.5.2/smact/structure_prediction/prediction.py`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.1/smact/structure_prediction/probability_models.py` & `SMACT-2.5.2/smact/structure_prediction/probability_models.py`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.1/smact/structure_prediction/structure.py` & `SMACT-2.5.2/smact/structure_prediction/structure.py`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.1/smact/structure_prediction/utilities.py` & `SMACT-2.5.2/smact/structure_prediction/utilities.py`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.1/smact/tests/test_core.py` & `SMACT-2.5.2/smact/tests/test_core.py`

 * *Files 8% similar despite different names*

```diff
@@ -342,14 +342,36 @@
         self.assertEqual(
             [(r[0], r[1], r[2]) for r in result],
             [
                 (("Na", "Fe", "Cl"), (1, -1, -1), (2, 1, 1)),
                 (("Na", "Fe", "Cl"), (1, 1, -1), (1, 1, 2)),
             ],
         )
+        result_comp_tuple = smact.screening.smact_filter(
+            [Na, Fe, Cl], threshold=2, comp_tuple=True
+        )
+        self.assertTupleEqual(
+            result_comp_tuple[0].element_symbols, ("Na", "Fe", "Cl")
+        )
+        self.assertTupleEqual(result_comp_tuple[0].stoichiometries, (2, 1, 1))
+        self.assertTupleEqual(
+            result_comp_tuple[0].oxidation_states, (1, -1, -1)
+        )
+        self.assertEqual(
+            set(
+                smact.screening.smact_filter(
+                    [Na, Fe, Cl], threshold=2, species_unique=False
+                )
+            ),
+            {
+                (("Na", "Fe", "Cl"), (2, 1, 1)),
+                (("Na", "Fe", "Cl"), (1, 1, 2)),
+            },
+        )
+
         self.assertEqual(
             len(smact.screening.smact_filter([Na, Fe, Cl], threshold=8)), 77
         )
 
         result = smact.screening.smact_filter(
             [Na, Fe, Cl], stoichs=[[1], [1], [4]]
         )
```

### Comparing `SMACT-2.5.1/smact/tests/test_doper.py` & `SMACT-2.5.2/smact/tests/test_doper.py`

 * *Files identical despite different names*

### Comparing `SMACT-2.5.1/smact/tests/test_structure.py` & `SMACT-2.5.2/smact/tests/test_structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -367,15 +367,15 @@
             lambda_json=TEST_LAMBDA_JSON
         )
         cls.test_pymatgen_mutator = CationMutator.from_json(
             lambda_json=None, alpha=lambda x, y: -5
         )
 
         # 5 random test species -> 5! test pairs
-        cls.test_species = sample(cls.test_pymatgen_mutator.specs, 5)
+        cls.test_species = sample(list(cls.test_pymatgen_mutator.specs), 5)
         cls.test_pairs = list(
             itertools.combinations_with_replacement(cls.test_species, 2)
         )
 
         cls.pymatgen_sp = SubstitutionProbability(lambda_table=None, alpha=-5)
 
     def test_lambda_tab_pop(self):
```

