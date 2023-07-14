# Comparing `tmp/flee-3.0.tar.gz` & `tmp/flee-3.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flee-3.0.tar", last modified: Fri Jul 14 16:40:06 2023, max compression
+gzip compressed data, was "flee-3.0a0.tar", last modified: Mon Jul 25 10:06:54 2022, max compression
```

## Comparing `flee-3.0.tar` & `flee-3.0a0.tar`

### file list

```diff
@@ -1,68 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:40:06.043820 flee-3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-14 16:39:52.000000 flee-3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-14 16:39:52.000000 flee-3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-14 16:40:06.043820 flee-3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-14 16:39:52.000000 flee-3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:40:06.043820 flee-3.0/flee/
--rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-07-14 16:39:52.000000 flee-3.0/flee/Diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (123)    14348 2023-07-14 16:39:52.000000 flee-3.0/flee/InputGeography.py
--rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-07-14 16:39:52.000000 flee-3.0/flee/SimulationSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-14 16:39:52.000000 flee-3.0/flee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-14 16:40:06.043820 flee-3.0/flee/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    29790 2023-07-14 16:39:52.000000 flee-3.0/flee/coupling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:40:06.035821 flee-3.0/flee/datamanager/
--rw-r--r--   0 runner    (1001) docker     (123)    16669 2023-07-14 16:39:52.000000 flee-3.0/flee/datamanager/DataTable.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:39:52.000000 flee-3.0/flee/datamanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-14 16:39:52.000000 flee-3.0/flee/datamanager/calc_date_difference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-07-14 16:39:52.000000 flee-3.0/flee/datamanager/handle_refugee_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-14 16:39:52.000000 flee-3.0/flee/datamanager/read_period.py
--rw-r--r--   0 runner    (1001) docker     (123)    52678 2023-07-14 16:39:52.000000 flee-3.0/flee/flee.py
--rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-07-14 16:39:52.000000 flee-3.0/flee/micro_InputGeography.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-07-14 16:39:52.000000 flee-3.0/flee/moving.py
--rw-r--r--   0 runner    (1001) docker     (123)    22946 2023-07-14 16:39:52.000000 flee-3.0/flee/pflee.py
--rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-07-14 16:39:52.000000 flee-3.0/flee/pmicro_flee.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:40:06.039821 flee-3.0/flee/postprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-07-14 16:39:52.000000 flee-3.0/flee/postprocessing/CalculateDiagnostics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-14 16:39:52.000000 flee-3.0/flee/postprocessing/FormatPyplotFigures.py
--rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-07-14 16:39:52.000000 flee-3.0/flee/postprocessing/PlotRedirectionComparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-14 16:39:52.000000 flee-3.0/flee/postprocessing/StoreDiagnostics.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:39:52.000000 flee-3.0/flee/postprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18445 2023-07-14 16:39:52.000000 flee-3.0/flee/postprocessing/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-07-14 16:39:52.000000 flee-3.0/flee/postprocessing/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-14 16:39:52.000000 flee-3.0/flee/postprocessing/analyze_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-14 16:39:52.000000 flee-3.0/flee/postprocessing/compare_out.py
--rw-r--r--   0 runner    (1001) docker     (123)    10957 2023-07-14 16:39:52.000000 flee-3.0/flee/postprocessing/extract-validation-results.py
--rw-r--r--   0 runner    (1001) docker     (123)    29288 2023-07-14 16:39:52.000000 flee-3.0/flee/postprocessing/plot-flee-uq-output-more.py
--rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-07-14 16:39:52.000000 flee-3.0/flee/postprocessing/plot_flee_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-07-14 16:39:52.000000 flee-3.0/flee/postprocessing/plot_flee_forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)    13625 2023-07-14 16:39:52.000000 flee-3.0/flee/postprocessing/plot_flee_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    23262 2023-07-14 16:39:52.000000 flee-3.0/flee/postprocessing/plot_flee_uq_output.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-14 16:39:52.000000 flee-3.0/flee/postprocessing/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-14 16:39:52.000000 flee-3.0/flee/scoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-07-14 16:39:52.000000 flee-3.0/flee/spawning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:40:06.035821 flee-3.0/flee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-14 16:40:06.000000 flee-3.0/flee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-14 16:40:06.000000 flee-3.0/flee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:40:06.000000 flee-3.0/flee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:40:05.000000 flee-3.0/flee.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-14 16:40:06.000000 flee-3.0/flee.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-14 16:40:06.000000 flee-3.0/flee.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-14 16:39:53.000000 flee-3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-14 16:40:06.043820 flee-3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-14 16:39:53.000000 flee-3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:40:06.043820 flee-3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-14 16:39:53.000000 flee-3.0/tests/test_1_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-14 16:39:53.000000 flee-3.0/tests/test_awareness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-14 16:39:53.000000 flee-3.0/tests/test_camp_sink.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-14 16:39:53.000000 flee-3.0/tests/test_close_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-14 16:39:53.000000 flee-3.0/tests/test_conflict_driven_spawning.py
--rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-07-14 16:39:53.000000 flee-3.0/tests/test_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-14 16:39:53.000000 flee-3.0/tests/test_datatable.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-14 16:39:53.000000 flee-3.0/tests/test_load_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-14 16:39:53.000000 flee-3.0/tests/test_micro_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-14 16:39:53.000000 flee-3.0/tests/test_moving.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-14 16:39:53.000000 flee-3.0/tests/test_path_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-14 16:39:53.000000 flee-3.0/tests/test_removelink.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-14 16:39:53.000000 flee-3.0/tests/test_tiny_closure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-14 16:39:53.000000 flee-3.0/tests/test_toy_escape.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-14 16:39:53.000000 flee-3.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-25 10:06:53.996894 flee-3.0a0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1515 2022-07-25 10:06:39.000000 flee-3.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       71 2022-07-25 10:06:39.000000 flee-3.0a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2674 2022-07-25 10:06:53.996894 flee-3.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1856 2022-07-25 10:06:39.000000 flee-3.0a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-25 10:06:53.996894 flee-3.0a0/flee/
+-rw-r--r--   0 runner    (1001) docker     (121)     2416 2022-07-25 10:06:39.000000 flee-3.0a0/flee/Diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11345 2022-07-25 10:06:39.000000 flee-3.0a0/flee/InputGeography.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8661 2022-07-25 10:06:39.000000 flee-3.0a0/flee/SimulationSettings.py
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2022-07-25 10:06:39.000000 flee-3.0a0/flee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      497 2022-07-25 10:06:53.996894 flee-3.0a0/flee/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29790 2022-07-25 10:06:39.000000 flee-3.0a0/flee/coupling.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-25 10:06:53.992894 flee-3.0a0/flee/datamanager/
+-rw-r--r--   0 runner    (1001) docker     (121)    16669 2022-07-25 10:06:39.000000 flee-3.0a0/flee/datamanager/DataTable.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-25 10:06:39.000000 flee-3.0a0/flee/datamanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      326 2022-07-25 10:06:39.000000 flee-3.0a0/flee/datamanager/calc_date_difference.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3513 2022-07-25 10:06:39.000000 flee-3.0a0/flee/datamanager/handle_refugee_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)      981 2022-07-25 10:06:39.000000 flee-3.0a0/flee/datamanager/read_period.py
+-rw-r--r--   0 runner    (1001) docker     (121)    45432 2022-07-25 10:06:39.000000 flee-3.0a0/flee/flee.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6338 2022-07-25 10:06:39.000000 flee-3.0a0/flee/micro_InputGeography.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6059 2022-07-25 10:06:39.000000 flee-3.0a0/flee/moving.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21899 2022-07-25 10:06:39.000000 flee-3.0a0/flee/pflee.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13174 2022-07-25 10:06:39.000000 flee-3.0a0/flee/pmicro_flee.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-25 10:06:53.996894 flee-3.0a0/flee/postprocessing/
+-rw-r--r--   0 runner    (1001) docker     (121)     4061 2022-07-25 10:06:39.000000 flee-3.0a0/flee/postprocessing/CalculateDiagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1464 2022-07-25 10:06:39.000000 flee-3.0a0/flee/postprocessing/FormatPyplotFigures.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6923 2022-07-25 10:06:39.000000 flee-3.0a0/flee/postprocessing/PlotRedirectionComparison.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1740 2022-07-25 10:06:39.000000 flee-3.0a0/flee/postprocessing/StoreDiagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-25 10:06:39.000000 flee-3.0a0/flee/postprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18445 2022-07-25 10:06:39.000000 flee-3.0a0/flee/postprocessing/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4056 2022-07-25 10:06:39.000000 flee-3.0a0/flee/postprocessing/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1297 2022-07-25 10:06:39.000000 flee-3.0a0/flee/postprocessing/analyze_graph.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2128 2022-07-25 10:06:39.000000 flee-3.0a0/flee/postprocessing/compare_out.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10957 2022-07-25 10:06:39.000000 flee-3.0a0/flee/postprocessing/extract-validation-results.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29288 2022-07-25 10:06:39.000000 flee-3.0a0/flee/postprocessing/plot-flee-uq-output-more.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6531 2022-07-25 10:06:39.000000 flee-3.0a0/flee/postprocessing/plot_flee_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13614 2022-07-25 10:06:39.000000 flee-3.0a0/flee/postprocessing/plot_flee_output.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23262 2022-07-25 10:06:39.000000 flee-3.0a0/flee/postprocessing/plot_flee_uq_output.py
+-rw-r--r--   0 runner    (1001) docker     (121)      856 2022-07-25 10:06:39.000000 flee-3.0a0/flee/postprocessing/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2332 2022-07-25 10:06:39.000000 flee-3.0a0/flee/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6778 2022-07-25 10:06:39.000000 flee-3.0a0/flee/spawning.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-25 10:06:53.992894 flee-3.0a0/flee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2674 2022-07-25 10:06:53.000000 flee-3.0a0/flee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1260 2022-07-25 10:06:53.000000 flee-3.0a0/flee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-25 10:06:53.000000 flee-3.0a0/flee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-25 10:06:53.000000 flee-3.0a0/flee.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       72 2022-07-25 10:06:53.000000 flee-3.0a0/flee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-07-25 10:06:53.000000 flee-3.0a0/flee.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       72 2022-07-25 10:06:39.000000 flee-3.0a0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      168 2022-07-25 10:06:53.996894 flee-3.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1875 2022-07-25 10:06:39.000000 flee-3.0a0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)    68611 2022-07-25 10:06:39.000000 flee-3.0a0/versioneer.py
```

### Comparing `flee-3.0/LICENSE` & `flee-3.0a0/LICENSE`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 Copyright (c) 2015-2017, Brunel University London
+All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
     * Redistributions of source code must retain the above copyright
       notice, this list of conditions and the following disclaimer.
     * Redistributions in binary form must reproduce the above copyright
       notice, this list of conditions and the following disclaimer in the
@@ -16,8 +17,8 @@
 WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 DISCLAIMED. IN NO EVENT SHALL <COPYRIGHT HOLDER> BE LIABLE FOR ANY
 DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
 (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
 ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `flee-3.0/PKG-INFO` & `flee-3.0a0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,37 @@
 Metadata-Version: 2.1
 Name: flee
-Version: 3.0
+Version: 3.0a0
 Summary: Flee is an agent-based modelling toolkit which is purpose-built for simulating the movement of individuals across geographical locations.
 Home-page: https://flee.readthedocs.io
 Author: Derek Groen
 Author-email: Derek.Groen@brunel.ac.uk
 License: BSD-3-Clause
 Keywords: flee
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Flee
 [![Build Status](https://travis-ci.com/djgroen/flee.svg?branch=master)](https://travis-ci.com/djgroen/flee)
 [![GitHub Issues](https://img.shields.io/github/issues/djgroen/flee.svg)](https://github.com/djgroen/flee/issues)
 [![GitHub last-commit](https://img.shields.io/github/last-commit/djgroen/flee.svg)](https://github.com/djgroen/flee/commits/master)
 
 
-Flee is an agent-based modelling toolkit which is purpose-built for simulating
-the movement of individuals across geographical locations. Flee is currently
-used primarily for modelling the movements of forcibly displaced
-persons (FDPs).
+Flee is an agent-based modelling toolkit which is purpose-built for simulating the movement of individuals across geographical locations. Flee is currently used primarily for modelling the movements of refugees and internally displaces persons (IDPs).
 
-Full documentation of Flee is available at https://flee.readthedocs.io.
-
-Official releases will be done on https://www.github.com/djgroen/flee. (flee-release is deprecated and will be removed in due course.)
+Flee is currently is released periodically under a BSD 3-clause license once the first journal paper is accepted.
 
 ## Parallel performance testing
 
 Parallel tests can be performed using test_par.py. The interface is as follows:
 
 mpirun -np <cores> python3 tests/test_par.py [options]
```

### Comparing `flee-3.0/README.md` & `flee-3.0a0/flee.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,37 @@
+Metadata-Version: 2.1
+Name: flee
+Version: 3.0a0
+Summary: Flee is an agent-based modelling toolkit which is purpose-built for simulating the movement of individuals across geographical locations.
+Home-page: https://flee.readthedocs.io
+Author: Derek Groen
+Author-email: Derek.Groen@brunel.ac.uk
+License: BSD-3-Clause
+Keywords: flee
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Flee
 [![Build Status](https://travis-ci.com/djgroen/flee.svg?branch=master)](https://travis-ci.com/djgroen/flee)
 [![GitHub Issues](https://img.shields.io/github/issues/djgroen/flee.svg)](https://github.com/djgroen/flee/issues)
 [![GitHub last-commit](https://img.shields.io/github/last-commit/djgroen/flee.svg)](https://github.com/djgroen/flee/commits/master)
 
 
-Flee is an agent-based modelling toolkit which is purpose-built for simulating
-the movement of individuals across geographical locations. Flee is currently
-used primarily for modelling the movements of forcibly displaced
-persons (FDPs).
-
-Full documentation of Flee is available at https://flee.readthedocs.io.
+Flee is an agent-based modelling toolkit which is purpose-built for simulating the movement of individuals across geographical locations. Flee is currently used primarily for modelling the movements of refugees and internally displaces persons (IDPs).
 
-Official releases will be done on https://www.github.com/djgroen/flee. (flee-release is deprecated and will be removed in due course.)
+Flee is currently is released periodically under a BSD 3-clause license once the first journal paper is accepted.
 
 ## Parallel performance testing
 
 Parallel tests can be performed using test_par.py. The interface is as follows:
 
 mpirun -np <cores> python3 tests/test_par.py [options]
```

### Comparing `flee-3.0/flee/Diagnostics.py` & `flee-3.0a0/flee/micro_InputGeography.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,214 +1,191 @@
-from __future__ import annotations, print_function
-
+import csv
 import os
 import sys
 from functools import wraps
+
+# from flee import flee
+from flee.InputGeography import InputGeography as based_InputGeography_class
 from flee.SimulationSettings import SimulationSettings
 
 if os.getenv("FLEE_TYPE_CHECK") is not None and os.environ["FLEE_TYPE_CHECK"].lower() == "true":
     from beartype import beartype as check_args_type
 else:
-    def check_args_type(func):
-        return func
-
-
-def print_attribute_keys(a):
-    out = ""
-    for k in a.attributes.keys():
-        out += str(k)
-        out += ","
-    return out
-
-
-def print_attribute_values(a):
-    out = ""
-    for k in a.attributes.values():
-        out += str(k)
-        out += ","
-    return out
-
-
-@check_args_type
-def write_agents_par(
-    rank: int, agents, time: int, max_written: int = -1, timestep_interval: int = 1
-) -> None:
-    """
-    Write agent data to file. Write only up to <max_written> agents each time step,
-    and only write a file every <timestep_interval> time steps.
 
-    Args:
-        rank (int): Description
-        agents (List[Person]): Description
-        time (int): Description
-        max_written (int, optional): Description
-        timestep_interval (int, optional): Description
-    """
-
-    my_file = None
-    if time == 0:
-        my_file = open("agents.out.%s" % rank, "w", encoding="utf-8")
-        print(
-            "#time,rank-agentid,original_location,current_location,gps_x,gps_y,is_travelling,distance_travelled,"
-            "places_travelled,distance_moved_this_timestep,{}".format(print_attribute_keys(agents[0])),
-            file=my_file,
-        )
-    else:
-        my_file = open("agents.out.%s" % rank, "a", encoding="utf-8")
-
-    if max_written < 0:
-        max_written = len(agents)
-
-    if time % timestep_interval == 0:
-        for k in range(0, max_written):
-            a = agents[k]
-
-            if a.location is None: #Do not write agent logs for agents that are removed from the simulation.
-                continue
-
-            print(
-                    "{},{}-{},{},{},{},{},{},{},{},{},{}".format(
-                    time,
-                    rank,
-                    k,
-                    a.home_location.name,
-                    a.location.name,
-                    a.location.x,
-                    a.location.y,
-                    a.travelling,
-                    a.distance_travelled,
-                    a.places_travelled,
-                    a.distance_moved_this_timestep,
-                    print_attribute_values(a),
-                    ),
-                file=my_file,
-            )
-
-            if SimulationSettings.log_levels["agent"] > 1:
-                if SimulationSettings.log_levels["agent"] > 2:
-                    hop_number = 1 # hop counter starts at 1 to indicate second hop in time step.
-                    for l in a.locations_visited:
-                        print(
-                            "{}-{},{}-{},{},{},{},{},{},{},{},{},{}".format(
-                                time,
-                                hop_number,
-                                rank,
-                                k,
-                                a.home_location.name,
-                                l.name,
-                                l.x,
-                                l.y,
-                                a.travelling,
-                                a.distance_travelled,
-                                a.places_travelled,
-                                a.distance_moved_this_timestep,
-                                print_attribute_values(a),
-                            ),
-                            file=my_file,
-                        )
-                        hop_number += 1
+    def check_args_type(func):
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            return func(*args, **kwargs)
+
+        return wrapper
+
+
+class InputGeography(based_InputGeography_class):
+    """
+    Class which reads in Geographic information.
+    """
+
+    def __init__(self):
+        super().__init__()
+
+    @check_args_type
+    def ReadLinksFromCSV(
+        self,
+        csv_name: str,
+        name1_col: int = 0,
+        name2_col: int = 1,
+        dist_col: int = 2,
+        forced_redirection: int = 3,
+        link_type_col: int = 4,
+    ) -> None:
+        """
+        Converts a CSV file to a locations information table
+
+        Args:
+            csv_name (str): Description
+            name1_col (int, optional): Description
+            name2_col (int, optional): Description
+            dist_col (int, optional): Description
+            forced_redirection (int, optional): Description
+            link_type_col (int, optional): Description
+        """
+        self.links = []
+
+        with open(csv_name, newline="", encoding="utf-8") as csvfile:
+            values = csv.reader(csvfile)
+
+            for row in values:
+                if row[0][0] == "#":
+                    pass
                 else:
-                    for l in a.locations_visited:
-                        print(
-                            "{},{}-{},{},{},{},{},{},{},{},{},{}".format(
-                                time,
-                                rank,
-                                k,
-                                a.home_location.name,
-                                l.name,
-                                l.x,
-                                l.y,
-                                a.travelling,
-                                a.distance_travelled,
-                                a.places_travelled,
-                                a.distance_moved_this_timestep,
-                                print_attribute_values(a),
-                            ),
-                            file=my_file,
-                        )
-
-
-
-@check_args_type
-def write_agents(agents, time: int, max_written: int = -1, timestep_interval: int = 1) -> None:
-    """
-    Summary
-
-    Args:
-        agents (List[Person]): Description
-        time (int): Description
-        max_written (int, optional): Description
-        timestep_interval (int, optional): Description
-    """
-    write_agents_par(rank=0, agents=agents, time=time, max_written=-1, timestep_interval=1)
-
-
-@check_args_type
-def write_links_par(
-    rank: int, locations, time: int, timestep_interval: int = 1
-) -> None:
-    """
-    Write agent data to file. Write only up to <max_written> agents each time step,
-    and only write a file every <timestep_interval> time steps.
-
-    Args:
-        rank (int): Description
-        agents (List[Person]): Description
-        time (int): Description
-        max_written (int, optional): Description
-        timestep_interval (int, optional): Description
-    """
-
-    my_file = None
-    if time == 0:
-        my_file = open("links.out.%s" % rank, "w", encoding="utf-8")
-        print(
-            "#time,start_location,end_location,cum_num_agents,attribute",
-            file=my_file,
-        )
-    else:
-        my_file = open("links.out.%s" % rank, "a", encoding="utf-8")
-
-    if time % timestep_interval == 0:
-        for i in range(0, len(locations)):
-            for l in locations[i].links:
+                    # print(row)
+                    self.links.append(
+                        [
+                            row[name1_col],
+                            row[name2_col],
+                            row[dist_col],
+                            row[forced_redirection],
+                            row[link_type_col],
+                        ]
+                    )
+
+        """
+        if isinstance(row[link_type_col], str):
+            if "drive" in row[link_type_col].lower():
+                flee.SimulationSettings.move_rules["MaxMoveSpeed"] = flee.SimulationSettings.move_rules["MaxMoveSpeed"]
+            elif "walk" in row[link_type_col].lower():
+                flee.SimulationSettings.move_rules["MaxMoveSpeed"] = flee.SimulationSettings.MaxWalkSpeed
+            elif "crossing" in row[link_type_col].lower():
+                flee.SimulationSettings.move_rules["MaxMoveSpeed"] = flee.SimulationSettings.move_rules["MaxCrossingSpeed"]
+            else:
                 print(
-                    "{},{},{},{},total".format(
-                    time,
-                    l.startpoint.name,
-                    l.endpoint.name,
-                    l.cumNumAgents,
-                    ),
-                file=my_file,
+                    "Error in identifying link_type() object: cannot parse the type of link {}"
+                    " {} for location object with name.".format(link_type_col, name1_col)
                 )
+                sys.exit()
+        """
 
-                if SimulationSettings.log_levels["link"] > 1:
-                    for a in l.cumNumAgentsByAttribute:
-                        for v in l.cumNumAgentsByAttribute[a]:
-                            print(
-                                "{},{},{},{},{}:{}".format(
-                                time,
-                                l.startpoint.name,
-                                l.endpoint.name,
-                                l.cumNumAgentsByAttribute[a][v],
-                                a,
-                                v,
-                                ),
-                            file=my_file,
-                            )
-
-
+    @check_args_type
+    def StoreInputGeographyInEcosystem(self, e):
+        """
+        Store the geographic information in this class in a FLEE simulation,
+        overwriting existing entries.
+
+        Args:
+            e (Ecosystem): Description
+
+        Returns:
+            Tuple[Ecosystem, Dict]: Description
+        """
+        lm = {}
+        num_conflict_zones = 0
+
+        for loc in self.locations:
+            name = loc[0]
+
+            # if population field is empty, just set it to 0.
+            if len(loc[1]) < 1:
+                population = 0
+            else:
+                population = int(loc[1]) // SimulationSettings.optimisations["PopulationScaleDownFactor"]
+
+            x = float(loc[2]) if len(loc[2]) > 0 else 0.0
+            y = float(loc[3]) if len(loc[3]) > 0 else 0.0
+
+            # if population field is empty, just set it to 0.
+            if len(loc[7]) < 1:
+                country = "unknown"
+            else:
+                country = loc[7]
+
+            # print(loc, file=sys.stderr)
+            location_type = loc[4]
+            if "conflict" in location_type.lower():
+                num_conflict_zones += 1
+                if int(loc[5]) > 0:
+                    location_type = "town"
+
+            if "camp" in loc[4].lower():
+                lm[name] = e.addLocation(
+                    name=name,
+                    location_type=location_type,
+                    capacity=population,
+                    x=x,
+                    y=y,
+                    country=country,
+                )
+            else:
+                lm[name] = e.addLocation(
+                    name=name,
+                    location_type=location_type,
+                    pop=population,
+                    x=x,
+                    y=y,
+                    country=country,
+                )
 
+        for link in self.links:
+            if len(link) > 4:
+                if int(link[3]) == 1:
+                    e.linkUp(
+                        endpoint1=link[0],
+                        endpoint2=link[1],
+                        distance=float(link[2]),
+                        forced_redirection=True,
+                        link_type=str(link[4]),
+                    )
+                if int(link[3]) == 2:
+                    e.linkUp(
+                        endpoint1=link[1],
+                        endpoint2=link[0],
+                        distance=float(link[2]),
+                        forced_redirection=True,
+                        link_type=str(link[4]),
+                    )
+                else:
+                    e.linkUp(
+                        endpoint1=link[0],
+                        endpoint2=link[1],
+                        distance=float(link[2]),
+                        forced_redirection=False,
+                        link_type=str(link[4]),
+                    )
+            else:
+                e.linkUp(
+                    endpoint1=link[0],
+                    endpoint2=link[1],
+                    distance=float(link[2]),
+                    forced_redirection=False,
+                    link_type=str(link[4]),
+                )
 
-@check_args_type
-def write_links(locations, time: int, timestep_interval: int = 1) -> None:
-    """
-    Summary
+        e.closures = []
+        for link in self.closures:
+            e.closures.append([link[0], link[1], link[2], int(link[3]), int(link[4])])
 
-    Args:
-        agents (List[Person]): Description
-        time (int): Description
-        max_written (int, optional): Description
-        timestep_interval (int, optional): Description
-    """
-    write_links_par(rank=0, locations=locations, time=time, timestep_interval=1)
+        if num_conflict_zones < 1:
+            print(
+                "Warning: location graph has 0 conflict zones (ignore if conflicts.csv is used).",
+                file=sys.stderr,
+            )
 
+        return e, lm
```

### Comparing `flee-3.0/flee/InputGeography.py` & `flee-3.0a0/flee/InputGeography.py`

 * *Files 18% similar despite different names*

```diff
@@ -50,15 +50,15 @@
                     for i in range(1, len(headers)):  # field 0 is day.
                         headers[i] = headers[i].strip()
                         if len(headers[i]) > 0:
                             self.conflicts[headers[i]] = []
                 else:
                     for i in range(1, len(row)):  # field 0 is day.
                         # print(row[0])
-                        self.conflicts[headers[i]].append(float(row[i].strip()))
+                        self.conflicts[headers[i]].append(int(row[i].strip()))
                 row_count += 1
 
         # print(self.conflicts)
         # TODO: make test verifying this in test_csv.py
 
     @check_args_type
     def getConflictLocationNames(self) -> List[str]:
@@ -110,52 +110,43 @@
                     if len(row) > 8:
                         # First 8 columns have hard-coded names, other columns can be added to include custom (static) attributes
                         for i in range(8, len(row)):
                             print("appending", file=sys.stderr)
                             columns.append(row[i])
                         self.columns = columns
                     print("header", columns, row, len(row), file=sys.stderr)
+                    pass
                 else:
                     # print(row)
                     self.locations.append(row)
 
     @check_args_type
-    def MakeLocationList(self) -> dict:
-        loc_list = {}
-        for l in self.locations:
-            loc_list[l[0]] = [float(l[3]),float(l[4])]
-        return loc_list
-
-    @check_args_type
-    def ReadLinksFromCSV(self, csv_name: str) -> None:
+    def ReadLinksFromCSV(
+        self, csv_name: str, name1_col: int = 0, name2_col: int = 1, dist_col: int = 2
+    ) -> None:
         """
         Converts a CSV file to a locations information table
 
         Args:
             csv_name (str): Description
+            name1_col (int, optional): Description
+            name2_col (int, optional): Description
+            dist_col (int, optional): Description
         """
         self.links = []
 
         with open(csv_name, newline="", encoding="utf-8") as csvfile:
             values = csv.reader(csvfile)
 
-            link_columns = ["name1","name2","distance","forced_redirection"]
             for row in values:
                 if len(row) == 0 or row[0][0] == "#":
-                    if len(row) > 4:
-                        # First 8 columns have hard-coded names, other columns can be added to include custom (static) attributes
-                        for i in range(4, len(row)):
-                            print("appending", file=sys.stderr)
-                            link_columns.append(row[i])
-                    self.link_columns = link_columns
-                    print("link header", link_columns, row, len(row), file=sys.stderr)
                     pass
                 else:
                     # print(row)
-                    self.links.append(row)
+                    self.links.append([row[name1_col], row[name2_col], row[dist_col]])
 
     @check_args_type
     def ReadClosuresFromCSV(self, csv_name: str) -> None:
         """
         Read the closures.csv file. Format is:
         closure_type,name1,name2,closure_start,closure_end
 
@@ -170,53 +161,14 @@
             for row in values:
                 if len(row) == 0 or row[0][0] == "#":
                     pass
                 else:
                     # print(row)
                     self.closures.append(row)
 
-
-    def ReadAgentsFromCSV(self, e, csv_name: str) -> None:
-        """
-        Read the agents.csv file. Format is:
-        location,attributes
-
-        Args:
-            csv_name (str): Description
-        """
-
-        self.agents = []
-
-        with open(csv_name, newline="", encoding="utf-8") as csvfile:
-            values = csv.reader(csvfile)
-
-            i = 0
-            for row in values:
-                if len(row) == 0 or row[0][0] == "#":
-                    pass
-                elif i == 0:
-                    headers = row[1:]
-                    print(headers)
-                else:
-                    print(row)
-                    attr = {}
-                    for i in range (1, len(row)):
-                        attr[headers[i-1]] = row[i]
-
-                    loc_found = False
-                    for i in range(0, len(e.locationNames)):
-                        if e.locationNames[i] == row[0]:
-                            e.addAgent(e.locations[i], attributes=attr)
-                            loc_found= True
-
-                    if not loc_found:
-                        print("could not map location to CSV-loaded agent on line. (not count commented lines or empty lines)", sys.stderr)
-                i += 1
-
-
     def StoreInputGeographyInEcosystem(self, e):
         """
         Store the geographic information in this class in a FLEE simulation,
         overwriting existing entries.
 
         Args:
             e (Ecosystem): Description
@@ -226,21 +178,14 @@
         """
 
         #0"name",1"region",2"country",3"gps_x",4"gps_y",5"location_type",6"conflict_date",7"pop/cap"
 
 
         lm = {}
         num_conflict_zones = 0
-
-        # Home country is assumed to be the country of the first location.
-        home_country = self.locations[0][2]
-        print("Home country set to: ", home_country, file=sys.stderr)
-        if len(home_country) < 1:
-            home_country = "unknown"
-
         for loc in self.locations:
 
             name = loc[0]
             # if population field is empty, just set it to 0.
             if len(loc[7]) < 1:
                 population = 0
             else:
@@ -251,18 +196,14 @@
 
             # if country field is empty, just set it to unknown.
             if len(loc[2]) < 1:
                 country = "unknown"
             else:
                 country = loc[2]
 
-            foreign = True
-            if country == home_country:
-                foreign = False
-
             # print(loc, file=sys.stderr)
             location_type = loc[5]
             if "conflict" in location_type.lower():
                 num_conflict_zones += 1
                 if int(loc[6]) > 0:
                     location_type = "town"
 
@@ -274,72 +215,57 @@
             if "camp" in location_type.lower():
                 lm[name] = e.addLocation(
                     name=name,
                     location_type=location_type,
                     capacity=population,
                     x=x,
                     y=y,
-                    foreign=foreign,
                     country=country,
                     attributes=attributes
                 )
             else:
                 lm[name] = e.addLocation(
                     name=name,
                     location_type=location_type,
                     pop=population,
                     x=x,
                     y=y,
-                    foreign=foreign,
                     country=country,
                     attributes=attributes
                 )
 
         for link in self.links:
-            attributes = {}
-            if len(link) > 4:
-                for i in range(4, len(link)):
-                    attributes[self.link_columns[i]] = link[i]
-
             if len(link) > 3:
-                l3 = link[3]
-                if len(l3) == 0:
-                    l3 = 0
-
-                if int(l3) == 1:
+                if int(link[3]) == 1:
                     e.linkUp(
                         endpoint1=link[0],
                         endpoint2=link[1],
                         distance=float(link[2]),
                         forced_redirection=True,
-                        attributes=attributes,
                     )
-                if int(l3) == 2:
+                if int(link[3]) == 2:
                     e.linkUp(
                         endpoint1=link[1],
                         endpoint2=link[0],
                         distance=float(link[2]),
                         forced_redirection=True,
-                        attributes=attributes,
                     )
                 else:
                     e.linkUp(
                         endpoint1=link[0],
                         endpoint2=link[1],
                         distance=float(link[2]),
                         forced_redirection=False,
-                        attributes=attributes,
                     )
             else:
                 e.linkUp(
                     endpoint1=link[0],
                     endpoint2=link[1],
                     distance=float(link[2]),
                     forced_redirection=False,
-                    attributes = {},
                 )
 
         e.closures = []
         for link in self.closures:
             e.closures.append([link[0], link[1], link[2], int(link[3]), int(link[4])])
 
         if num_conflict_zones < 1:
@@ -362,47 +288,44 @@
             e (Ecosystem): Description
             time (int): Description
             Debug (bool, optional): Description
         """
         if len(SimulationSettings.FlareConflictInputFile) == 0:
             for loc in self.locations:
                 if "conflict" in loc[4].lower() and int(loc[5]) == time:
-                    conflict_intensity = 1.0
                     if e.print_location_output:
                         print(
-                            "Time = {}. Adding a new conflict zone [{}] with pop. {} and intensity {}".format(
-                                time, loc[0], int(loc[1]), conflict_intensity
+                            "Time = {}. Adding a new conflict zone [{}] with pop. {}".format(
+                                time, loc[0], int(loc[1])
                             ),
                             file=sys.stderr,
                         )
-                    e.add_conflict_zone(name=loc[0], conflict_intensity=conflict_intensity)
+                    e.add_conflict_zone(name=loc[0])
         else:
-            conflict_names = self.getConflictLocationNames()
+            conflic_names = self.getConflictLocationNames()
             # print(confl_names)
-            for conflict_name in conflict_names:
+            for conflic_name in conflic_names:
                 if Debug:
-                    print("L:", conflict_name, self.conflicts[conflict_name], time, file=sys.stderr)
-                if self.conflicts[conflict_name][time] > 0.000001:
+                    print("L:", conflic_name, self.conflicts[conflic_name], time, file=sys.stderr)
+                if self.conflicts[conflic_name][time] == 1:
                     if time > 0:
-                        if self.conflicts[conflict_name][time - 1] < 0.000001:
+                        if self.conflicts[conflic_name][time - 1] == 0:
                             print(
-                                "Time = {}. Adding a new conflict zone [{}] with intensity {}".format(
-                                    time, conflict_name, self.conflicts[conflict_name][time]
+                                "Time = {}. Adding a new conflict zone [{}]".format(
+                                    time, conflic_name
                                 ),
                                 file=sys.stderr,
                             )
-                            e.add_conflict_zone(name=conflict_name, conflict_intensity=self.conflicts[conflict_name][time])
+                            e.add_conflict_zone(name=conflic_name)
                     else:
                         print(
-                            "Time = {}. Adding a new conflict zone [{}] with intensity {}".format(
-                                time, conflict_name, self.conflicts[conflict_name][time]
-                            ),
+                            "Time = {}. Adding a new conflict zone [{}]".format(time, conflic_name),
                             file=sys.stderr,
                         )
-                        e.add_conflict_zone(name=conflict_name,conflict_intensity=self.conflicts[conflict_name][time])
-                if self.conflicts[conflict_name][time] < 0.000001 and time > 0:
-                    if self.conflicts[conflict_name][time - 1] == 1:
+                        e.add_conflict_zone(name=conflic_name)
+                if self.conflicts[conflic_name][time] == 0 and time > 0:
+                    if self.conflicts[conflic_name][time - 1] == 1:
                         print(
-                            "Time = {}. Removing conflict zone [{}]".format(time, conflict_name),
+                            "Time = {}. Removing conflict zone [{}]".format(time, conflic_name),
                             file=sys.stderr,
                         )
-                        e.remove_conflict_zone(name=conflict_name)
+                        e.remove_conflict_zone(name=conflic_name)
```

### Comparing `flee-3.0/flee/SimulationSettings.py` & `flee-3.0a0/flee/SimulationSettings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+import csv
 import sys
 import yaml
 import os
 
 # pylint: skip-file
 
+from typing import List, Optional, Tuple
+
 if os.getenv("FLEE_TYPE_CHECK") is not None and os.environ["FLEE_TYPE_CHECK"].lower() == "true":
     from beartype import beartype as check_args_type
 else:
     def check_args_type(func):
         return func
 
 
@@ -32,45 +35,42 @@
     spawn_rules = {} # ABM spawning rules
     move_rules = {} # ABM movement rules
     optimisations = {} # Settings to improve runtime performance
 
     sqrt_ten = 3.16227766017  # square root of ten (10^0.5).
 
 
-    @staticmethod
+    @check_args_type
     def get_conflict_decay(time_since_conflict: int):
 
-        if SimulationSettings.spawn_rules["conflict_spawn_decay"] is None:
-            return 1.0
-
         spawn_len = len(SimulationSettings.spawn_rules["conflict_spawn_decay"])
 
         if spawn_len < 1:
             print("Warning: no conflict spawn decay set. Defaulting to no decay", file=sys.stderr)
             return 1.0
         else:
             i = min(int(time_since_conflict / 30), spawn_len-1)
             if SimulationSettings.log_levels["conflict"] > 0:
               print("Conflict zone spawn status: time elapsed {}, decay factor {}".format(time_since_conflict, float(SimulationSettings.spawn_rules["conflict_spawn_decay"][i])), file=sys.stderr)
             return float(SimulationSettings.spawn_rules["conflict_spawn_decay"][i])
 
 
-    @staticmethod
+    @check_args_type
     def get_location_conflict_decay(time: int, loc):
         """
 
         time: e.time (time in simulation)
         loc: location for which to calculate the decay multiplier.
         """
         time_since_conflict = time - loc.time_of_conflict
         multiplier = SimulationSettings.get_conflict_decay(time_since_conflict)
         return multiplier
 
 
-    @staticmethod
+    @check_args_type
     def ReadFromYML(ymlfile: str):
 
         print("YAML file:", ymlfile, file=sys.stderr)
         with open(ymlfile) as f:
             dp = yaml.safe_load(f)
 
         number_of_steps = float(fetchss(dp,"number_of_steps",-1))
@@ -78,26 +78,21 @@
 
         print("YAML:", dp, file=sys.stderr)
 
         dpll = fetchss(dp,"log_levels",None)
 
         SimulationSettings.log_levels["agent"] = int(fetchss(dpll,"agent",0))
         # set to 1 to obtain average times for agents to reach camps at any time
-        # set to 2 to obtain duplicate entries when agents do multiple hops in one timestep.
-        # step (aggregate info).
-        SimulationSettings.log_levels["link"] = int(fetchss(dpll,"link",0))
-        # set to 1 to obtain cumulative agent counts on links at any time
         # step (aggregate info).
         SimulationSettings.log_levels["camp"] = int(fetchss(dpll,"camp",0))
         # set to 1 for basic information on locations added and conflict zones
         # assigned.
         SimulationSettings.log_levels["init"] = int(fetchss(dpll,"init",0))
         # set to 1 for information on conflict zone spawning
         SimulationSettings.log_levels["conflict"] = int(fetchss(dpll,"conflict",0))
-        SimulationSettings.log_levels["idp_totals"] = int(fetchss(dpll,"idp_totals",0))
 
 
 
         dps = fetchss(dp,"spawn_rules",None)
 
         # Spawned agents are subtracted from populations. This can lead to crashes if the number of spawned agents
         # exceeds the total population in conflict zones.
@@ -106,17 +101,14 @@
         SimulationSettings.spawn_rules["TakeFromPopulation"] = bool(fetchss(dps, "take_from_population", False))
         # Advanced settings
         SimulationSettings.spawn_rules["InsertDayZeroRefugeesInCamps"] = bool(fetchss(dps, "insert_day0", True))
 
 
         SimulationSettings.spawn_rules["conflict_zone_spawning_only"] = bool(fetchss(dps, "conflict_zone_spawning_only", True)) # Only spawn agents from conflict zones.
 
-        SimulationSettings.spawn_rules["camps_are_sinks"] = bool(fetchss(dps, "camps_are_sicks", False)) # Camps can deactivate agents.
-        SimulationSettings.spawn_rules["read_from_agents_csv_file"] = bool(fetchss(dps, "read_from_agents_csv_file", False)) # Load agents from agents.csv file.
-
         dpsc = fetchss(dps,"conflict_driven_spawning",None)
         if dpsc is not None:
           SimulationSettings.spawn_rules["conflict_driven_spawning"] = True # Conflicts provide a direct push factor.
           
           SimulationSettings.spawn_rules["conflict_spawn_mode"] = fetchss(dpsc,"spawn_mode","constant") # constant, Poisson, pop_ratio
 
           if SimulationSettings.spawn_rules["conflict_spawn_mode"] == "pop_ratio":
@@ -141,30 +133,28 @@
         SimulationSettings.move_rules["MaxWalkSpeed"] = float(fetchss(dpr,"max_walk_speed", 35.0))
 
         # most number of km that we expect refugees to traverse per time step on
         # boat/walk to cross river (2 km/h * 10 hours).
         SimulationSettings.move_rules["MaxCrossingSpeed"] = float(fetchss(dpr,"max_crossing_speed", 20.0))
 
 
-        SimulationSettings.move_rules["ForeignWeight"] = float(fetchss(dpr,"foreign_weight", 1.0)) # attraction multiplier for foreign locations (stacks with camp multiplier).
         SimulationSettings.move_rules["CampWeight"] = float(fetchss(dpr,"camp_weight", 1.0)) # attraction multiplier for camps.
         SimulationSettings.move_rules["ConflictWeight"] = float(fetchss(dpr,"conflict_weight", 1.0 / SimulationSettings.sqrt_ten)) #attraction multiplier for source zones (conflict zones)
 
 
         SimulationSettings.move_rules["ConflictMoveChance"] = float(fetchss(dpr,"conflict_movechance", 1.0)) # chance of persons leaving a conflict zone per day.
         SimulationSettings.move_rules["CampMoveChance"] = float(fetchss(dpr,"camp_movechance", 0.001)) # chance of persons leaving a camp.
-        SimulationSettings.move_rules["IDPCampMoveChance"] = float(fetchss(dpr,"idpcamp_movechance", 0.1)) # chance of persons leaving a camp.
         SimulationSettings.move_rules["DefaultMoveChance"] = float(fetchss(dpr,"default_movechance", 0.3)) # chance of persons leaving a regular location per day.
         
 
-        SimulationSettings.move_rules["AwarenessLevel"] = int(fetchss(dpr,"awareness_level", 1)) # awareness of locations X link steps away by agents.
+        SimulationSettings.move_rules["AwarenessLevel"] = float(fetchss(dpr,"awareness_level", 1)) # awareness of locations X link steps away by agents.
         # -1, no weighting at all, 0 = road only, 1 = location, 2 = neighbours, 3 = region.
        
-        # A location or camp is beginning to be considered full if the number of agents there exceeds (capacity OR pop) * CapacityBuffer.
-        SimulationSettings.move_rules["CapacityBuffer"] = float(fetchss(dpr,"capacity_buffer", 0.9)) # awareness of locations X link steps away by agents.
+        # A location or camp is considered full if the number of agents there exceeds (capacity OR pop) * CapacityBuffer.
+        SimulationSettings.move_rules["CapacityBuffer"] = float(fetchss(dpr,"capacity_buffer", 1.0)) # awareness of locations X link steps away by agents.
 
         # Displaced people will not take a break unless they at least travelled
         # for a full day's distance in the last two days.
         SimulationSettings.move_rules["AvoidShortStints"] = bool(fetchss(dpr,"avoid_short_stints",False))
       
         # Agents traverse first link on foot.
         SimulationSettings.move_rules["StartOnFoot"] = bool(fetchss(dpr,"start_on_foot",False))
@@ -179,23 +169,21 @@
         # Flee 3.0 Prototyping conditionals (see design focument)
         # TODO: embed these in a more flexible/powerful framework of conditionals
         for a in ["ChildrenAvoidHazards", "BoysTakeRisk", "MatchCampEthnicity", "MatchTownEthnicity", "MatchConflictEthnicity"]:
             SimulationSettings.move_rules[a] = bool(fetchss(dpr,a,False))
 
 
         dpo = fetchss(dp, "optimisations", None)
-        SimulationSettings.optimisations["PopulationScaleDownFactor"] = int(fetchss(dpo,"hasten",1))
+        SimulationSettings.optimisations["PopulationScaleDownFactor"] = float(fetchss(dpo,"hasten",1.0))
 
         if SimulationSettings.UseV1Rules is True:
             SimulationSettings.move_rules["MaxMoveSpeed"] = 200
             SimulationSettings.move_rules["StartOnFoot"] = False
             # Displaced people will not take a break unless they at least travelled
             # for a full day's distance in the last two days.
             SimulationSettings.move_rules["AvoidShortStints"] = False
             SimulationSettings.move_rules["CampWeight"] = 2.0  # attraction factor for camps.
             # reduction factor for refugees entering conflict zones.
             SimulationSettings.move_rules["ConflictWeight"] = 0.25
 
-        print("Move rules set to:", SimulationSettings.move_rules, file=sys.stderr)
-
         return number_of_steps
```

### Comparing `flee-3.0/flee/coupling.py` & `flee-3.0a0/flee/coupling.py`

 * *Files identical despite different names*

### Comparing `flee-3.0/flee/datamanager/DataTable.py` & `flee-3.0a0/flee/datamanager/DataTable.py`

 * *Files identical despite different names*

### Comparing `flee-3.0/flee/datamanager/handle_refugee_data.py` & `flee-3.0a0/flee/datamanager/handle_refugee_data.py`

 * *Files identical despite different names*

### Comparing `flee-3.0/flee/datamanager/read_period.py` & `flee-3.0a0/flee/datamanager/read_period.py`

 * *Files identical despite different names*

### Comparing `flee-3.0/flee/flee.py` & `flee-3.0a0/flee/flee.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import copy
 import os
 import random
 import sys
 from typing import List, Optional, Tuple
 
 import numpy as np
-from flee.Diagnostics import write_agents, write_links
+from flee.Diagnostics import write_agents
 from flee.SimulationSettings import SimulationSettings
 import flee.moving as moving
 import flee.spawning as spawning
 import flee.scoring as scoring
 
 if os.getenv("FLEE_TYPE_CHECK") is not None and os.environ["FLEE_TYPE_CHECK"].lower() == "true":
     from beartype import beartype as check_args_type
@@ -31,23 +31,24 @@
         "home_location",
         "timesteps_since_departure",
         "places_travelled",
         "recent_travel_distance",
         "distance_moved_this_timestep",
         "travelling",
         "distance_travelled_on_link",
+        "age",
+        "gender",
         "attributes",
-        "locations_visited",
-        "route",
     ]
 
     @check_args_type
-    def __init__(self, location, attributes):
+    def __init__(self, location, age, gender, attributes):
         self.location = location
         self.home_location = location
+        self.location.IncrementNumAgents()
         self.timesteps_since_departure = 0
         self.places_travelled = 1
 
         # An index of how much the agent has recently traveled
         # (range : 0.0-1.0).
         self.recent_travel_distance = 0.0
         # Number of km moved this timestep.
@@ -56,135 +57,83 @@
         # Set to true when an agent resides on a link.
         self.travelling = False
 
         # Tracks how much distance a Person has been able to travel on the
         # current link.
         self.distance_travelled_on_link = 0
 
+        self.age=age
+        self.gender=gender
         self.attributes=attributes
-        self.route = []
 
         if SimulationSettings.log_levels["agent"] > 0:
-            self.distance_travelled = 0 
-            # track total distance travelled.
-        if SimulationSettings.log_levels["agent"] > 1:
-            self.locations_visited = [] 
-            # track and write locations visited before final one in timestep.
-
-        self.location.IncrementNumAgents(self)
-
-    @check_args_type
-    def getBaseEndPointScore(self, link) -> float:
-        """
-        Serial base endpoint score retrieval.
-
-        Args:
-            link (Link) : Description
-
-        Returns:
-            float: Description
-        """
-        return link.endpoint.scores[1]
+            self.distance_travelled = 0
 
 
     @check_args_type
     def handle_travel(self, location, travelling) -> None:
         """
         Summary
 
         Args:
             location: location to travel to (can be Location of Link type).
             travelling: set to True if location is a Link, False if it is a Location object.
         """
         self.location.DecrementNumAgents()
         self.location = location
-        self.location.IncrementNumAgents(self)
+        self.location.IncrementNumAgents()
         self.travelling = travelling
         self.distance_travelled_on_link = 0
 
 
-    def check_dest_is_full_camp(self,e):
-        for i in range(0, len(e.locationNames)):
-            if e.locationNames[i] == self.route[-1]:
-                if e.locations[i].camp and moving.getCapMultiplier(e.locations[i],1) < 0.5:
-                    #print(e.time, e.locationNames[i], self.route[-1], file=sys.stderr)
-                    return True
-                else: 
-                    return False
-
-
-    def take_next_step(self,e):
-        for l in self.location.links:
-            if l.endpoint.name == self.route[0]:
-                if self.check_dest_is_full_camp(e):
-                    self.route = []
-                    return None
-                self.route = self.route[1:]
-                return l
-
-        # Link has vanished, remove route.
-        self.route = []
-        return None
-
     @check_args_type
-    def evolve(self, e, time: int, ForceTownMove: bool = False) -> None:
+    def evolve(self, time: int, ForceTownMove: bool = False) -> None:
         """
         Summary
 
         Args:
             time (int): Description
             ForceTownMove (bool, optional): Description
         """
-
         if self.travelling is False:
-            if self.location.town and ForceTownMove: # called through evolveMore
+            if self.location.town and ForceTownMove:
                 movechance = 1.0
-            else: # called first time in loop
+            else:
                 movechance = self.location.movechance
 
             outcome = random.random()
             # print(movechance)
 
             if outcome < movechance:
-                #only plan a route if the agent has no existing route.
-                if len(self.route) == 0:
-                    # determine here which route to take
-                    self.route = moving.selectRoute(self, time=time)
-
-                # attempt to follow route. Return None if fail.    
-                chosenDest = self.take_next_step(e)
+                # determine here which route to take?
+                chosenRoute = moving.selectRoute(self, time=time)
 
                 # if there is a viable route to a different location.
-                if chosenDest:
+                if chosenRoute:
                     # update location to link endpoint
-                    self.handle_travel(chosenDest, travelling=True)
+                    self.handle_travel(chosenRoute, travelling=True)
 
 
     @check_args_type
-    def finish_travel(self, e, time: int) -> None:
+    def finish_travel(self, time: int) -> None:
         """
         Summary
 
         Args:
             time (int): Description
         """
         if self.travelling:
 
-            todays_travel_speed = float(self.location.attributes.get("max_move_speed", SimulationSettings.move_rules["MaxMoveSpeed"]))
-
             if self.places_travelled == 1 and SimulationSettings.move_rules["StartOnFoot"]:
-                todays_travel_speed = SimulationSettings.move_rules["MaxWalkSpeed"]
-
-            # Flee 3.0: support for walk_probability attribute on links.
-            walk_probability = float(self.location.attributes.get("walk_probability","0.0"))
-            if random.random() < walk_probability:
-                todays_travel_speed = SimulationSettings.move_rules["MaxWalkSpeed"]
-
-            self.distance_travelled_on_link += todays_travel_speed
-            self.distance_moved_this_timestep += todays_travel_speed
+                # First journey
+                self.distance_travelled_on_link += SimulationSettings.move_rules["MaxWalkSpeed"]
+                self.distance_moved_this_timestep += SimulationSettings.move_rules["MaxWalkSpeed"]
+            else:
+                self.distance_travelled_on_link += SimulationSettings.move_rules["MaxMoveSpeed"]
+                self.distance_moved_this_timestep += SimulationSettings.move_rules["MaxMoveSpeed"]
 
             # If destination has been reached.
             if self.distance_travelled_on_link > self.location.get_distance():
 
                 self.places_travelled += 1
                 # remove the excess km tracked by the
                 # distance_moved_this_timestep var.
@@ -202,46 +151,43 @@
                     self.handle_travel(self.location.startpoint, travelling=False)
 
                 else:
                     # if the person has moved less than the MaxMoveSpeed, it
                     # should go through another evolve() step in the new
                     # location.
                     evolveMore = False
-                    if self.distance_moved_this_timestep < todays_travel_speed:
-                        if SimulationSettings.log_levels["agent"] > 1:
-                            self.locations_visited.append(self.location)
+                    if self.distance_moved_this_timestep < SimulationSettings.move_rules["MaxMoveSpeed"]:
                         evolveMore = True
 
                     # update location (which is on a link) to link endpoint
                     self.handle_travel(self.location.endpoint, travelling=False)
 
                     if SimulationSettings.log_levels["camp"] > 0:
-                        if self.location.camp is True:
+                        if self.location.Camp is True:
                             self.location.incoming_journey_lengths += [
                                 self.timesteps_since_departure
                             ]
 
                     # Perform another evolve step if needed. And if it results
                     # in travel, then the current traveled distance needs
                     # to be taken into account.
-                    # Note MaxMoveSpeed is used here, not todays_travel_speed.
                     if evolveMore is True:
                         ForceTownMove = False
                         if SimulationSettings.move_rules["AvoidShortStints"]:
                             # Flee 2.0 Changeset 1, factor 2.
                             if (
                                 self.recent_travel_distance
                                 + (
                                     self.distance_moved_this_timestep
                                     / SimulationSettings.move_rules["MaxMoveSpeed"]
                                 )
                             ) / 2.0 < 0.5:
                                 ForceTownMove = True
-                        self.evolve(e, time=time, ForceTownMove=ForceTownMove)
-                        self.finish_travel(e, time=time)
+                        self.evolve(time=time, ForceTownMove=ForceTownMove)
+                        self.finish_travel(time=time)
 
 
 class Location:
     """
     The Location class
     """
 
@@ -269,50 +215,46 @@
         self.numAgents = 0  # refugee population
         # refugee population on current rank (for pflee).
         self.numAgentsOnRank = 0
         self.capacity = capacity  # refugee capacity
         self.pop = pop  # non-refugee population
         self.foreign = foreign
         self.country = country
-        self.conflict = -1.0
+        self.conflict = False
         self.conflict_date = -1 # date that last conflict erupted.
         self.camp = False
-        self.idpcamp = False
         self.town = False
         self.forward = False
         self.marker = False
         self.time_of_conflict = -1 # Time that a major conflict event last took place.
         self.numAgentsSpawned = 0
 
         self.attributes = attributes # This will store a range of attributes that are read from file.
 
         if location_type is not None:
             if "camp" in location_type.lower():
                 self.movechance = SimulationSettings.move_rules["CampMoveChance"]
                 self.camp = True
-                if "idp" in location_type.lower():
-                    self.idpcamp = True
-                    self.movechance = SimulationSettings.move_rules["IDPCampMoveChance"]
+                self.foreign = True
             elif "conflict" in location_type.lower():
                 self.movechance = SimulationSettings.move_rules["ConflictMoveChance"]
-                self.conflict = float(self.attributes.get("conflict_intensity",1.0))
+                self.conflict = True
             elif "forward" in location_type.lower():
                 self.movechance = 1.0
                 self.forward = True
             elif "marker" in location_type.lower():
                 self.movechance = 1.0
                 self.marker = True
             elif "default" in location_type.lower() or "town" in location_type.lower():
                 self.town = True
                 self.movechance = SimulationSettings.move_rules["DefaultMoveChance"]
             else:
                 print(
                     "Error in creating Location() object: cannot parse location_type value of"
-                    " {} for location object with name {}".format(location_type, name),
-                    file=sys.stderr
+                    " {} for location object with name {}".format(location_type, name)
                 )
 
         # Automatically tags a location as a Camp if refugees are less than 2%
         # likely to move out on a given day.
         if self.movechance < 0.005 and not self.camp:
             print(
                 "Warning: automatically setting location {} to camp, "
@@ -321,90 +263,66 @@
             )
             self.camp = True
             self.town = False
 
         self.scores = np.array([1.0, 1.0, 1.0, 1.0])
 
         scoring.updateLocationScore(0,self)
+        scoring.updateNeighbourhoodScore(self)
+        scoring.updateRegionScore(self)
 
         if SimulationSettings.log_levels["camp"] > 0:
             # reinitializes every time step. Contains individual journey
             # lengths from incoming agents.
             self.incoming_journey_lengths = []
 
         self.print()
 
     @check_args_type
-    def open_camp(self, IDP=False) -> None:
+    def SetCamp(self) -> None:
         """
-        Summary: change location type to camp or IDP camp.
+        Summary
         """
-        self.movechance = SimulationSettings.move_rules["CampMoveChance"]
+        self.movechance = SimulationSettings.CampMoveChance
         self.camp = True
-        self.conflict = -1.0
+        self.foreign = True
+        self.conflict = False
         self.town = False
-        self.forward = False
-        self.marker = False
-        if IDP:
-            self.idpcamp = True
-            self.movechance = SimulationSettings.move_rules["IDPCampMoveChance"]
-
-
-    @check_args_type
-    def setAttribute(self, name: str, value) -> None:
-        self.attributes[name] = value
-
-
-    @check_args_type
-    def close_camp(self, IDP=False) -> None:
-        """
-        Summary: change location type to town.
-        """
-        self.movechance = SimulationSettings.move_rules["DefaultMoveChance"]
-        self.camp = False
-        self.idpcamp = False
-        self.conflict = -1.0
-        self.town = True
-        self.forward = False
-        self.marker = False
-
 
     @check_args_type
     def DecrementNumAgents(self) -> None:
         """
         Summary
         """
         self.numAgents -= 1
 
     @check_args_type
-    def IncrementNumAgents(self, agent) -> None:
+    def IncrementNumAgents(self) -> None:
         """
         Summary
         """
         self.numAgents += 1
 
     @check_args_type
     def print(self) -> None:
         """
         Summary
         """
         print(
             "Location name: {}, X: {}, Y: {}, movechance: {}, cap: {}, "
-            "pop: {}, country: {}, conflict? {}, camp? {}, foreign? {}, attributes: {}".format(
+            "pop: {}, country: {}, conflict? {}, camp? {}".format(
                 self.name,
                 self.x,
                 self.y,
                 self.movechance,
                 self.capacity,
                 self.pop,
                 self.country,
                 self.conflict,
                 self.camp,
-                self.foreign,
-                self.attributes,
             ),
             file=sys.stderr,
         )
         for link in self.links:
             print(
                 "Link from {} to {}, dist: {}, pop. {}".format(
                     self.name, link.endpoint.name, link.get_distance(), link.numAgents
@@ -454,67 +372,46 @@
 
 class Link:
     """
     the Link class
     """
 
     @check_args_type
-    def __init__(self, startpoint, endpoint, distance: float, forced_redirection: bool = False, attributes: dict = {}):
-        self.name = "L:{}:{}".format(startpoint.name, endpoint.name)
+    def __init__(self, startpoint, endpoint, distance: float, forced_redirection: bool = False):
+        self.name = "__link__"
         self.closed = False
 
         # distance in km.
         self.__distance = distance
 
         # links for now always connect two endpoints
         self.startpoint = startpoint
         self.endpoint = endpoint
-        self.x = (self.startpoint.x + self.endpoint.x) / 2.0
-        self.y = (self.startpoint.y + self.endpoint.y) / 2.0
 
         # number of agents that are in transit.
         self.numAgents = 0
-        self.cumNumAgents = 0 # cumulative # of agents
-        if SimulationSettings.log_levels["link"] > 1:
-            self.cumNumAgentsByAttribute = {}
         # refugee population on current rank (for pflee).
         self.numAgentsOnRank = 0
 
         # if True, then all Persons will go down this link.
         self.forced_redirection = forced_redirection
 
-        self.attributes = attributes
-
     @check_args_type
     def DecrementNumAgents(self) -> None:
         """
         Summary
         """
         self.numAgents -= 1
 
     @check_args_type
-    def IncrementNumAgents(self, agent) -> None:
+    def IncrementNumAgents(self) -> None:
         """
         Summary
         """
         self.numAgents += 1
-        self.cumNumAgents += 1
-
-        if SimulationSettings.log_levels["link"] > 1:
-            for a in agent.attributes:
-                category = self.cumNumAgentsByAttribute.get(a, {})
-                category[agent.attributes[a]] = category.get(agent.attributes[a], 0) + 1
-                self.cumNumAgentsByAttribute[a] = category
-            #print(category, file=sys.stderr)
-
-
-    @check_args_type
-    def setAttribute(self, name: str, value) -> None:
-        self.attributes[name] = value
-
 
     def get_distance(self) -> float:
         """
         Summary
 
         Args:
 
@@ -586,15 +483,15 @@
         total number of camp arrivals.
         """
         if SimulationSettings.log_levels["camp"] > 0:
             arrival_total = 0
             tmp_num_arrivals = 0
 
             for loc in self.locations:
-                if loc.camp is True:
+                if loc.Camp is True:
                     arrival_total += np.sum(loc.incoming_journey_lengths)
                     tmp_num_arrivals += len(loc.incoming_journey_lengths)
                     loc.incoming_journey_lengths = []
 
             self.num_arrivals += [tmp_num_arrivals]
 
             if tmp_num_arrivals > 0:
@@ -623,45 +520,31 @@
                         if Debug:
                             print(
                                 "Time = {}. Closing Border between "
                                 "[{}] and [{}]".format(time, c[1], c[2]),
                                 file=sys.stderr,
                             )
                         self.close_border(source_country=c[1], dest_country=c[2], twoway=twoway)
-                    elif c[0] == "location":
+                    if c[0] == "location":
                         self.close_location(location_name=c[1], twoway=twoway)
-                    elif c[0] == "link":
+                    if c[0] == "link":
                         self.close_link(startpoint=c[1], endpoint=c[2], twoway=twoway)
-                    elif c[0] == "camp":
-                        self.close_camp(c[1], IDP=False)
-                    elif c[0] == "idpcamp":
-                        self.close_camp(c[1], IDP=True)
-                    elif c[0] == "remove_forced_redirection":
-                        self.set_forced_redirection(c[1], c[2], False)
-
                 if time == c[4]:
                     if c[0] == "country":
                         if Debug:
                             print(
                                 "Time = {}. Reopening Border between "
                                 "[{}] and [{}]".format(time, c[1], c[2]),
                                 file=sys.stderr,
                             )
                         self.reopen_border(source_country=c[1], dest_country=c[2], twoway=twoway)
-                    elif c[0] == "location":
+                    if c[0] == "location":
                         self.reopen_location(location_name=c[1], twoway=twoway)
-                    elif c[0] == "link":
+                    if c[0] == "link":
                         self.reopen_link(startpoint=c[1], endpoint=c[2], twoway=twoway)
-                    elif c[0] == "camp":
-                        self.open_camp(c[1], IDP=False)
-                    elif c[0] == "idpcamp":
-                        self.open_camp(c[1], IDP=True)
-                    elif c[0] == "remove_forced_redirection":
-                        self.set_forced_redirection(c[1], c[2], True)
-
 
     @check_args_type
     def _convert_location_name_to_index(self, name: str) -> int:
         """
         Convert a location name to an index number
 
         Args:
@@ -677,15 +560,15 @@
                 x = i
 
         # for i in range(0, len(self.locations)):
         #     if self.locations[i].name == name:
         #         x = i
 
         if x < 0:
-            print("#Warning: location not found in remove_link", file=sys.stderr)
+            print("#Warning: location not found in remove_link")
             return False
 
         return x
 
     @check_args_type
     def _remove_link_1way(self, startpoint: str, endpoint: str, close_only: bool = False) -> bool:
         """
@@ -1049,40 +932,14 @@
             source_country=source_country, dest_country=dest_country, mode="reopen", Debug=Debug
         )
         if twoway:
             self._change_border_1way(
                 source_country=dest_country, dest_country=source_country, mode="reopen", Debug=Debug
             )
 
-
-    @check_args_type
-    def close_camp(self, location_name: str, IDP: bool):
-        self.locations[self._convert_location_name_to_index(location_name)].close_camp(IDP)
-        print("Time = {}. Close camp {}, IDP: {}.".format(self.time, location_name, IDP), file=sys.stderr)
-
-
-    @check_args_type
-    def open_camp(self, location_name: str, IDP: bool):
-        self.locations[self._convert_location_name_to_index(location_name)].open_camp(IDP)
-        print("Time = {}. Open camp {}, IDP: {}.".format(self.time, location_name, IDP), file=sys.stderr)
-
-
-    @check_args_type
-    def set_forced_redirection(self, loc1_name: str, loc2_name: str, value: bool):
-        id1 = self._convert_location_name_to_index(loc1_name)
-        for i in range(0, len(self.locations[id1].links)):
-            if self.locations[id1].links[i].endpoint.name == loc2_name:
-                old_val = self.locations[id1].links[i].forced_redirection
-                self.locations[id1].links[i].forced_redirection = value
-                print("Time = {}. Redirection {}-{} changed from {} to {}.".format(self.time, loc1_name, loc2_name, old_val, value), file=sys.stderr)
-
-
- 
-
-
     @check_args_type
     def close_location(self, location_name: str, twoway: bool = True, Debug: bool = False) -> bool:
         """
         Close in- and outgoing links for a location.
 
         Args:
             location_name (str): Description
@@ -1115,15 +972,15 @@
             return self._change_location_1way(
                 location_name, mode="reopen", direction="both", Debug=Debug
             )
 
         return self._change_location_1way(location_name, mode="reopen", direction="in", Debug=Debug)
 
     @check_args_type
-    def add_conflict_zone(self, name: str, conflict_intensity: float = 1.0, change_movechance: bool = True) -> None:
+    def add_conflict_zone(self, name: str, change_movechance: bool = True) -> None:
         """
         Adds a conflict zone. Default weight is equal to
         population of the location.
 
         Args:
             name (str): Description
             change_movechance (bool, optional): Description
@@ -1131,23 +988,23 @@
         Returns:
             None: Description
         """
         for i in range(0, len(self.locationNames)):
             if self.locationNames[i] == name:
                 if change_movechance:
                     self.locations[i].movechance = SimulationSettings.move_rules["ConflictMoveChance"]
-                    self.locations[i].conflict = conflict_intensity
+                    self.locations[i].conflict = True
                     self.locations[i].town = False
 
                 self.locations[i].time_of_conflict = self.time                  
                 spawning.refresh_spawn_weights(self)
 
                 if SimulationSettings.log_levels["init"] > 0:
-                    print("Added conflict zone: {}, pop. {}, intensity: {}".format(name, self.locations[i].pop, conflict_intensity), file=sys.stderr)
-                    print("New total spawn weight: ", sum(self.spawn_weights), file=sys.stderr)
+                    print("Added conflict zone:", name, ", pop. ", self.locations[i].pop)
+                    print("New total spawn weight: ", sum(self.spawn_weights))
                 return
 
         print("Diagnostic: self.locationNames: ", self.locationNames, file=sys.stderr)
         print(
             "ERROR in flee.add_conflict_zone: location with name [{}] "
             "appears not to exist in the FLEE ecosystem "
             "(see diagnostic above).".format(name),
@@ -1160,20 +1017,19 @@
         Shorthand function to remove a conflict zone from the list.
         (not used yet)
 
         Args:
             name (str): Description
             change_movechance (bool, optional): Description
         """
-        for i in range(0, len(self.locationNames)):
-            if self.locationNames[i] == name:
-                if change_movechance:
-                    self.locations[i].movechance = SimulationSettings.move_rules["DefaultMoveChance"]
-                self.locations[i].conflict = -1.0
-                self.locations[i].town = True
+        for i in range(0, len(self.conflict_zones)):
+            if change_movechance:
+                self.conflict_zones[i].movechance = SimulationSettings.move_rules["DefaultMoveChance"]
+            self.conflict_zones[i].conflict = False
+            self.conflict_zones[i].town = True
 
         spawning.refresh_spawn_weights(self)
 
     @check_args_type
     def pick_spawn_location(self):
         """
         Summary
@@ -1196,75 +1052,62 @@
 
         Args:
             number (int, optional): Description
 
         Returns:
             list: Description
         """
-        spawn_weight_total = sum(self.spawn_weights)
+        swtotal = sum(self.spawn_weights)
 
-        assert spawn_weight_total > 0
+        assert swtotal > 0
 
         return np.random.choice(
-            self.locations, number, p=self.spawn_weights / spawn_weight_total
+            self.locations, number, p=self.spawn_weights / swtotal
         ).tolist()
 
 
     @check_args_type
     def evolve(self) -> None:
         """
         Summary
         """
-
         spawning.refresh_spawn_weights(self) # Required to correctly incorporate TakeFromPopulation and ConflictSpawnDecay.
 
         # update level 1, 2 and 3 location scores
         for loc in self.locations:
             scoring.updateLocationScore(self.time, loc)
 
+        for loc in self.locations:
+            scoring.updateNeighbourhoodScore(loc)
+
+        for loc in self.locations:
+            scoring.updateRegionScore(loc)
+
         # update agent locations
         for a in self.agents:
-            if SimulationSettings.log_levels["agent"] > 1:
-                a.locations_visited = []
-            if a.location is not None:
-                a.evolve(self, time=self.time)
+            a.evolve(time=self.time)
 
         for a in self.agents:
-            if a.location is not None:
-                a.finish_travel(self, time=self.time)
-                a.timesteps_since_departure += 1
-        
+            a.finish_travel(time=self.time)
+            a.timesteps_since_departure += 1
 
         if SimulationSettings.log_levels["agent"] > 0:
             write_agents(agents=self.agents, time=self.time)
 
-        if SimulationSettings.log_levels["link"] > 0:
-            write_links(locations=self.locations, time=self.time)
-
         for a in self.agents:
             a.recent_travel_distance = (
                 a.recent_travel_distance
                 + (a.distance_moved_this_timestep / SimulationSettings.move_rules["MaxMoveSpeed"])
             ) / 2.0
             a.distance_moved_this_timestep = 0
 
         # update link properties
         if SimulationSettings.log_levels["camp"] > 0:
             self._aggregate_arrivals()
 
-        # Deactivate agents in camps with a certain probability.
-        if SimulationSettings.spawn_rules["camps_are_sinks"] == True:
-            for a in self.agents:
-                if a.travelling == False:
-                    if a.location is not None:
-                        if a.location.camp == True:
-                            outcome = random.random()
-                            if outcome < a.location.attributes.get("deactivation_probability", 0.0):
-                                a.location = None
-
         self.time += 1
 
     @check_args_type
     def addLocation(
         self,
         name: str,
         x: float = 0.0,
@@ -1305,45 +1148,45 @@
             capacity=capacity,
             pop=pop,
             foreign=foreign,
             country=country,
             attributes=attributes,
         )
         if SimulationSettings.log_levels["init"] > 0 and self.print_location_output:
-            print("Location:", name, x, y, loc.movechance, capacity, ", pop. ", pop, foreign, ", attrib. ", attributes, file=sys.stderr)
+            print("Location:", name, x, y, loc.movechance, capacity, ", pop. ", pop, foreign, ", attrib. ",attributes)
 
         self.locations.append(loc)
         self.spawn_weights = np.append(self.spawn_weights, [0.0])
         self.locationNames.append(loc.name)
 
         spawning.refresh_spawn_weights(self)
         return loc
 
     @check_args_type
-    def addAgent(self, location, attributes) -> None:
+    def addAgent(self, location, age, gender, attributes) -> None:
         """
         Summary
 
         Args:
             location (Location): Description
         """
         if SimulationSettings.spawn_rules["TakeFromPopulation"]:
-            if location.conflict > 0.0:
+            if location.conflict:
                 if location.pop > 0:
                     location.pop -= 1
                     location.numAgentsSpawned += 1
                 else:
                     print(
                         "ERROR: Number of agents in the simulation is larger than the combined "
                         "population of the conflict zones. Please amend locations.csv."
                     )
                     location.print()
                     assert location.pop > 1
 
-        self.agents.append(Person(location=location, attributes=attributes))
+        self.agents.append(Person(location=location, age=age, gender=gender, attributes=attributes))
 
     @check_args_type
     def insertAgent(self, location) -> None:
         """
         Note: insert Agent does NOT take from Population.
 
         Args:
@@ -1378,56 +1221,31 @@
                 new_agents += self.agents[i]  # agent is preserved in ecosystem
             else:
                 # agent is removed from the ecosystem and number of agents
                 # drops by one.
                 self.agents[i].location.DecrementNumAgents()
         self.agents = new_agents
 
-
-    @check_args_type
-    def setAttribute(self, name: str, value) -> None:
-        self.attributes[name] = value
-
-
     @check_args_type
     def numAgents(self) -> int:
         """
         Summary
 
         Returns:
             int: Description
         """
         return len(self.agents)
 
-
-    @check_args_type
-    def numIDPs(self) -> int:
-        """
-        Aggregates number of IDPs across locations
-
-        Returns:
-            int: total # of IDPs.
-        """
-        num_idps = 0
-
-        for l in self.locations:
-            if l.idpcamp:
-                num_idps += l.numAgents
-
-        return num_idps
-
-
     @check_args_type
     def linkUp(
         self,
         endpoint1: str,
         endpoint2: str,
         distance: float = 1.0,
         forced_redirection: bool = False,
-        attributes: dict = {},
     ) -> None:
         """
         Creates a link between two endpoint locations
 
         Args:
             endpoint1 (str): Description
             endpoint2 (str): Description
@@ -1439,45 +1257,43 @@
         for i in range(0, len(self.locationNames)):
             if self.locationNames[i] == endpoint1:
                 endpoint1_index = i
             if self.locationNames[i] == endpoint2:
                 endpoint2_index = i
 
         if endpoint1_index < 0:
-            print("Diagnostic: Ecosystem.locationNames: ", self.locationNames, file=sys.stderr)
+            print("Diagnostic: Ecosystem.locationNames: ", self.locationNames)
             print(
                 "Error: link created to non-existent source: {}  with dest {}".format(
-                    endpoint1, endpoint2, file=sys.stderr
+                    endpoint1, endpoint2
                 )
             )
             sys.exit()
         if endpoint2_index < 0:
-            print("Diagnostic: Ecosystem.locationNames: ", self.locationNames, file=sys.stderr)
+            print("Diagnostic: Ecosystem.locationNames: ", self.locationNames)
             print(
                 "Error: link created to non-existent destination: {} with source {}".format(
-                    endpoint2, endpoint1, file=sys.stderr
+                    endpoint2, endpoint1
                 )
             )
             sys.exit()
 
         self.locations[endpoint1_index].links.append(
             Link(
                 startpoint=self.locations[endpoint1_index],
                 endpoint=self.locations[endpoint2_index],
                 distance=distance,
                 forced_redirection=forced_redirection,
-                attributes=attributes,
             )
         )
         self.locations[endpoint2_index].links.append(
             Link(
                 startpoint=self.locations[endpoint2_index],
                 endpoint=self.locations[endpoint1_index],
                 distance=distance,
-                attributes=attributes,
             )
         )
 
     @check_args_type
     def printInfo(self) -> None:
         """
         Summary
```

### Comparing `flee-3.0/flee/moving.py` & `flee-3.0a0/flee/moving.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import sys
 import numpy as np
 import random
-from beartype.typing import List, Optional, Tuple
+from typing import List, Optional, Tuple
 from flee.SimulationSettings import SimulationSettings
 
 if os.getenv("FLEE_TYPE_CHECK") is not None and os.environ["FLEE_TYPE_CHECK"].lower() == "true":
     from beartype import beartype as check_args_type
 else:
     def check_args_type(func):
         return func
@@ -22,34 +22,31 @@
         agent (Person): agent making the decision
         link (Link): Description
 
     Returns:
         float: Description
     """
     # print(link.endpoint.name, link.endpoint.scores)
-    base = agent.getBaseEndPointScore(link) # called externally because serial and parallel implementations differ.
-
+    base = link.endpoint.scores[1]
     # The base score is derived from the perceived level of safety and security.
     # E.g. Conflict zones have lower scores, camps have higher scores.
     # Location effects like high/low GDP, food security or weather effects could later also alter this score.
 
     #["ChildrenAvoidHazards", "BoysTakeRisk", "MatchCampEthnicity", "MatchTownEthnicity", "MatchConflictEthnicity"]
-    if SimulationSettings.move_rules["ChildrenAvoidHazards"]:
-        if agent.attributes["age"]<19:
-            # For children the safety of the destination is more important than for adults.
-            base = base*base
-        if SimulationSettings.move_rules["BoysTakeRisk"]:
-            if agent.attributes["gender"]=="male" and agent.attributes["age"]>14:
-                # Hypothesis that perceived safety does not affect routing decisions for teenage boys.
-                base = 1 
+    if SimulationSettings.move_rules["ChildrenAvoidHazards"] and agent.age <19:
+        # For children the safety of the destination is more important than for adults.
+        base = base*base
+        if SimulationSettings.move_rules["BoysTakeRisk"] and agent.gender=="male" and agent.age>14:
+            # Hypothesis that perceived safety does not affect routing decisions for teenage boys.
+            base = 1 
 
     if link.endpoint.camp == True:
         if SimulationSettings.move_rules["MatchCampEthnicity"]:
             base *= (spawning.getAttributeRatio(link.endpoint, "ethnicity") * 10.0)
-    elif link.endpoint.conflict > 0.0:
+    elif link.endpoint.conflict == True:
         if SimulationSettings.move_rules["MatchConflictEthnicity"]:
             base *= (spawning.getAttributeRatio(link.endpoint, "ethnicity") * 10.0)
     else:
         if SimulationSettings.move_rules["MatchTownEthnicity"]:
             base *= (spawning.getAttributeRatio(link.endpoint, "ethnicity") * 10.0)
 
     return base
@@ -68,32 +65,33 @@
         float: return
 
         - 1.0 if occupancy < nearly_full_occ (0.9).
         - 0.0 if occupancy >= 1.0.
         - a value in between for intermediate values
     """
 
-    nearly_full_occ = SimulationSettings.move_rules["CapacityBuffer"]  # occupancy rate to be considered nearly full.
+    nearly_full_occ = 0.9  # occupancy rate to be considered nearly full.
     # full occupancy limit (should be equal to self.capacity).
+    cap_limit = location.capacity * SimulationSettings.move_rules["CapacityBuffer"]
 
-    if location.capacity < 1:
+    if location.capacity < 0:
         return 1.0
 
-    if location.numAgents <= nearly_full_occ * location.capacity:
+    if location.numAgents <= nearly_full_occ * cap_limit:
         return 1.0
 
-    if location.numAgents >= 1.0 * location.capacity:
+    if location.numAgents >= 1.0 * cap_limit:
         return 0.0
 
     # should be a number equal in range [0 to 0.1*self.numAgents].
-    residual = location.numAgents - (nearly_full_occ * location.capacity)
+    residual = location.numAgents - (nearly_full_occ * cap_limit)
 
     # Calculate the residual weighting factor, when pop is between 0.9 and
     # 1.0 of capacity (with default settings).
-    weight = 1.0 - (residual / (location.capacity * (1.0 - nearly_full_occ)))
+    weight = 1.0 - (residual / (cap_limit * (1.0 - nearly_full_occ)))
 
     assert weight >= 0.0
     assert weight <= 1.0
 
     return weight
 
 
@@ -103,15 +101,15 @@
   agent,
   link,
   prior_distance: float,
   origin_names: List[str],
   step: int,
   time: int,
   debug: bool = False,
-) -> Tuple[List[float],List[List[str]]]:
+) -> float:
   """
   Calculates Link Weights recursively based on awareness level.
   Loops are avoided.
 
   Args:
   a: agent
   link (Link): Description
@@ -123,80 +121,75 @@
   """
 
 
 
   weight = float(getEndPointScore(agent=agent, link=link)
           / float(SimulationSettings.move_rules["Softening"] + link.get_distance() + prior_distance)) * getCapMultiplier(link.endpoint, numOnLink=int(link.numAgents))
 
-  weights = [weight]
-  routes = [origin_names + [link.endpoint.name]]
 
   if SimulationSettings.move_rules["AwarenessLevel"] > step:
     # Traverse the tree one step further.
-    for lel in link.endpoint.links:
-      if lel.endpoint.name in origin_names:
+    for e in link.endpoint.links:
+      if e.endpoint.name in origin_names:
         # Link points back to an origin, so ignore.
         pass
       else:
-        wgt, rts = calculateLinkWeight(agent=agent,
-              link=lel,
+        weight = max(
+          weight,
+          calculateLinkWeight(agent=agent,
+              link=e,
               prior_distance=prior_distance + link.get_distance(),
               origin_names=origin_names + [link.endpoint.name],
               step=step + 1,
               time=time,
               debug=debug,
-              )
-        weights = weights + wgt
-        routes = routes + rts
+              ),
+          )
 
   if debug:
-    print("step {}, total weight returned {}, routes {}".format(step, weights, routes), file=sys.stderr)
-  return weights, routes
+    print("step {}, total weight returned {}".format(step, weight))
+  return weight
 
 
 @check_args_type
-def normalizeWeights(weights: List[float]) -> List[float]:
+def normalizeWeights(weights) -> list:
   """
   Summary
 
   Args:
     weights (List[float]): Description
 
   Returns:
     list: Description
   """
-
   if np.sum(weights) > 0.0:
-    weights = [x/float(sum(weights)) for x in weights]
-    #weights = weights.tolist()
-  else:  # if all have zero weight, then we do equal weighting
-    weights = [(x+1)/float(len(weights)) for x in weights]
-    
-
-  return weights
+    weights /= np.sum(weights)
+  else:  # if all have zero weight, then we do equal weighting.
+    weights += 1.0 / float(len(weights))
+  return weights.tolist()
 
 
 
 @check_args_type
-def chooseFromWeights(weights, routes):
+def chooseFromWeights(weights, linklist):
   """
   Summary
 
   Args:
-    weights (List[float]): Weights for each route
-    routes (List[List[str]]]): List of possible routes
+    weights (List[float]): Description
+    linklist (List[Link]): Description
 
   Returns:
     float: Description
   """
   if len(weights) == 0:
     return None
 
   weights = normalizeWeights(weights=weights)
-  result = random.choices(routes, weights=weights)
+  result = random.choices(linklist, weights=weights)
   return result[0]
 
 
 @check_args_type
 def selectRoute(a, time: int, debug: bool = False):
   """
   Summary
@@ -205,35 +198,26 @@
   a: Agent
   time (int): Description
   debug (bool, optional): Description
 
   Returns:
   int: Description
   """
-  weights = []
-  routes = []
+  linklen = len(a.location.links)
+  weights = np.zeros(linklen)
 
   if SimulationSettings.move_rules["AwarenessLevel"] == 0:
-    linklen = len(a.location.links)
-    return [np.random.randint(0, linklen)]
+    return np.random.randint(0, linklen)
 
   for k, e in enumerate(a.location.links):
-    wgt, rts = calculateLinkWeight(
+    weights[k] = calculateLinkWeight(
          a,
          link=e,
          prior_distance=0.0,
-         origin_names=[],
+         origin_names=[a.location.name],
          step=1,
          time=time,
          debug=debug,
     )
 
-    weights = weights + wgt
-    routes = routes + rts
-
-  if debug:
-    print("selectRoute: ",routes, weights, file=sys.stderr)
-  route = chooseFromWeights(weights=weights, routes=routes)
-
-
-  return route
+  return chooseFromWeights(weights=weights, linklist=a.location.links)
```

### Comparing `flee-3.0/flee/pflee.py` & `flee-3.0a0/flee/pflee.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 import os
 import sys
 from functools import wraps
 from typing import List, Optional
 
 import numpy as np
-from flee import flee,scoring,spawning
-from flee.Diagnostics import write_agents_par,write_links_par
+from flee import flee,scoring
+from flee.Diagnostics import write_agents_par
 from flee.SimulationSettings import SimulationSettings
 from mpi4py import MPI
 
 if os.getenv("FLEE_TYPE_CHECK") is not None and os.environ["FLEE_TYPE_CHECK"].lower() == "true":
     from beartype import beartype as check_args_type
 else:
 
@@ -68,42 +68,44 @@
         "timesteps_since_departure",
         "places_travelled",
         "recent_travel_distance",
         "distance_moved_this_timestep",
         "travelling",
         "distance_travelled_on_link",
         "e",
+        "age",
+        "gender",
         "attributes",
     ]
 
     @check_args_type
-    def __init__(self, e, location, attributes):
-        super().__init__(location, attributes)
+    def __init__(self, e, location, age, gender, attributes):
+        super().__init__(location, age, gender, attributes)
         self.e = e
 
     @check_args_type
-    def evolve(self, e, time: int, ForceTownMove: bool = False) -> None:
+    def evolve(self, time: int, ForceTownMove: bool = False) -> None:
         """
         Summary
 
         Args:
             time (int): Description
-            ForceTownMove (bool, optional): towns have a move chance of 1.0.
+            ForceTownMove (bool, optional): Description
         """
-        super().evolve(e, time=time, ForceTownMove=ForceTownMove)
+        super().evolve(time=time, ForceTownMove=ForceTownMove)
 
     @check_args_type
-    def finish_travel(self, e, time: int) -> None:
+    def finish_travel(self, time: int) -> None:
         """
         Summary
 
         Args:
             time (int): Description
         """
-        super().finish_travel(e, time=time)
+        super().finish_travel(time=time)
 
     @check_args_type
     def getLinkWeightV1(self, link, awareness_level: int) -> float:
         """
         Calculate the weight of an adjacent link. Weight = probability that
         it will be chosen.
 
@@ -120,15 +122,15 @@
 
         return float(
             self.e.scores[(link.endpoint.id * 4) + awareness_level]
             / float(SimulationSettings.move_rules["Softening"] + link.get_distance())
         )
 
     @check_args_type
-    def getBaseEndPointScore(self, link) -> float:
+    def getEndPointScore(self, link) -> float:
         """
         Overwrite serial function because we have a different data structure
         for endpoint scores.
 
         Args:
             link (Link) : Description
 
@@ -183,15 +185,15 @@
     def DecrementNumAgents(self) -> None:
         """
         Summary
         """
         self.numAgentsOnRank -= 1
 
     @check_args_type
-    def IncrementNumAgents(self, agent) -> None:
+    def IncrementNumAgents(self) -> None:
         """
         Summary
         """
         self.numAgentsOnRank += 1
 
     @check_args_type
     def print(self) -> None:
@@ -231,15 +233,17 @@
         Updates all scores of a particular location. Different to
         Serial Flee, due to the reversed order there.
 
         Args:
             time (int): Description
         """
         self.time = time
-        scoring.updateLocationScore(time, self)
+        scoring.updateRegionScore(loc)
+        scoring.updateNeighbourhoodScore(loc)
+        scoring.updateLocationScore(time, loc)
 
 
 class Link(flee.Link):
     """
     The Link class
     """
 
@@ -248,24 +252,22 @@
         super().__init__(startpoint, endpoint, distance, forced_redirection)
 
     @check_args_type
     def DecrementNumAgents(self) -> None:
         """
         Summary
         """
-        self.numAgentsOnRank -= 1
-        super().DecrementNumAgents()
+        self.numAgents -= 1
 
     @check_args_type
-    def IncrementNumAgents(self, agent) -> None:
+    def IncrementNumAgents(self) -> None:
         """
         Summary
         """
-        self.numAgentsOnRank += 1
-        super().IncrementNumAgents(agent)
+        self.numAgents += 1
 
 
 class Ecosystem(flee.Ecosystem):
     """
     The Ecosystem class
     """
 
@@ -322,32 +324,14 @@
         # N = t % self.mpi.size
         # if self.mpi.rank == N:
         if self.mpi.rank == 0:
             return True
         return False
 
     @check_args_type
-    def numIDPs(self) -> int:
-        """
-        Aggregates number of IDPs across locations
-
-        Returns:
-            int: total # of IDPs.
-        """
-        num_idps = 0
-
-        for loc in self.locations:
-            if loc.idpcamp:
-                num_idps += loc.numAgents
-
-        num_idps_all = self.mpi.CalcCommWorldTotalSingle(num_idps)
-        return num_idps_all
-
-
-    @check_args_type
     def updateNumAgents(self, CountClosed: bool = False, log: bool = True) -> None:
         """
         Summary
 
         Args:
             CountClosed (bool, optional): Description
             log (bool, optional): Description
@@ -420,37 +404,37 @@
     """
     Add & insert agent functions.
     TODO: make addAgent function smarter, to prevent large load imbalances
     over time due to removals by clearLocationFromAgents?
     """
 
     @check_args_type
-    def addAgent(self, location, attributes) -> None:
+    def addAgent(self, location, age, gender, attributes) -> None:
         """
         Summary
 
         Args:
             location (Location): Description
         """
-        if SimulationSettings.spawn_rules["TakeFromPopulation"]:
-            if location.conflict > 0.0:
+        if SimulationSettings.move_rules["TakeFromPopulation"]:
+            if location.conflict:
                 if location.pop > 1:
                     location.pop -= 1
                     location.numAgentsSpawnedOnRank += 1
                     location.numAgentsSpawned += 1
                 else:
                     print(
                         "ERROR: Number of agents in the simulation is larger than the combined "
                         "population of the conflict zones. Please amend locations.csv."
                     )
                     location.print()
                     assert location.pop > 1
         self.total_agents += 1
         if self.total_agents % self.mpi.size == self.mpi.rank:
-            self.agents.append(Person(self, location=location, attributes=attributes))
+            self.agents.append(Person(self, location=location, age=age, gender=gender, attributes=attributes))
 
 
     @check_args_type
     def insertAgent(self, location) -> None:
         """
         Note: insert Agent does NOT take from Population.
 
@@ -564,33 +548,37 @@
             print("end of synchronize_locations", file=sys.stderr)
 
     @check_args_type
     def evolve(self) -> None:
         """
         Summary
         """
-
-
         if self.time == 0:
             # print("rank, num_agents:", self.mpi.rank, len(self.agents))
 
             # Update all scores three times to ensure code starts with updated
             # scores.
             for _ in range(0, 3):
                 for i, loc in enumerate(self.locations):
                     if i % self.mpi.size == self.mpi.rank:
                         loc.updateAllScores(time=self.time)
 
         if self.parallel_mode == "classic":
-            # update level 1 location scores (2 and 3 are obsolete).
+            # update level 1, 2 and 3 location scores.
             # Scores remain perfectly updated in classic mode.
             for loc in self.locations:
                 loc.time = self.time
                 scoring.updateLocationScore(loc)
 
+            for loc in self.locations:
+                scoring.updateNeighbourhoodScore(loc)
+
+            for loc in self.locations:
+                scoring.updateRegionScore(loc)
+
         elif self.parallel_mode == "loc-par":
             # update scores in reverse order for efficiency.
             # Neighbourhood and Region score will be outdated by 1 and 2 time
             # steps resp.
 
             loc_per_rank = int(len(self.locations) / self.mpi.size)
             lpr_remainder = int(len(self.locations) % self.mpi.size)
@@ -618,67 +606,54 @@
 
         # update location spawn total.
         for i, le in enumerate(self.locations):
             le.numAgentsSpawned = spawn_totals[i]
 
         # update agent locations
         for a in self.agents:
-            a.evolve(self, time=self.time)
+            a.evolve(time=self.time)
 
         # print("NumAgents after evolve:", file=sys.stderr)
         self.updateNumAgents(CountClosed=True, log=False)
 
         for a in self.agents:
-            a.finish_travel(self, time=self.time)
+            a.finish_travel(time=self.time)
             a.timesteps_since_departure += 1
 
         if SimulationSettings.log_levels["agent"] > 0:
             write_agents_par(rank=self.mpi.rank, agents=self.agents, time=self.time)
 
-        if SimulationSettings.log_levels["link"] > 0:
-            write_links_par(rank=self.mpi.rank, locations=self.locations, time=self.time)
-
         for a in self.agents:
             a.recent_travel_distance = (
                 a.recent_travel_distance
                 + (a.distance_moved_this_timestep / SimulationSettings.move_rules["MaxMoveSpeed"])
             ) / 2.0
             a.distance_moved_this_timestep = 0
 
         # print("NumAgents after finish_travel:", file=sys.stderr)
         self.updateNumAgents(log=False)
 
         # update link properties
         if SimulationSettings.log_levels["camp"] > 0:
             self._aggregate_arrivals()
 
-        # Deactivate agents in camps with a certain probability.
-        if SimulationSettings.spawn_rules["camps_are_sinks"] == True:
-            for a in self.agents:
-                if a.travelling == False:
-                    if a.location.camp == True:
-                        outcome = random.random()
-                        if outcome < a.location.attributes.get("deactivation_probability", 0.0):
-                            a.location = None
-
         self.time += 1
 
     @check_args_type
     def addLocation(
         self,
         name: str,
         x: float = 0.0,
         y: float = 0.0,
         location_type: Optional[str] = None,
-        movechance: float = -1.0,
+        movechance: float = SimulationSettings.move_rules["DefaultMoveChance"],
         capacity: int = -1,
         pop: int = 0,
         foreign: bool = False,
         country: str = "unknown",
-        attributes: dict = {},
     ):
         """
         Add a location to the ABM network graph
 
         Args:
             name (str): Description
             x (float, optional): Description
@@ -691,17 +666,14 @@
             country (str, optional): Description
 
         No Longer Returned:
             Location: Description
 
         """
 
-        if movechance < 0.0:
-            movechance = SimulationSettings.move_rules["DefaultMoveChance"]
-
         # Enlarge the scores array in Ecosystem to reflect the new location.
         # Pflee only.
         if self.cur_loc_id > 0:
             self.scores = np.append(self.scores, np.array([1.0, 1.0, 1.0, 1.0]))
         # print(len(self.scores))
 
         loc = Location(
@@ -724,20 +696,15 @@
             print(
                 "Location: {} {} {} {} {} , pop. {} {}".format(
                     name, x, y, loc.movechance, capacity, pop, foreign
                 ),
                 file=sys.stderr,
             )
         self.locations.append(loc)
-        self.spawn_weights = np.append(self.spawn_weights, [0.0])
         self.locationNames.append(loc.name)
-
-        spawning.refresh_spawn_weights(self)
-
-
         return loc
 
     @check_args_type
     def printComplete(self) -> None:
         """
         Summary
         """
```

### Comparing `flee-3.0/flee/pmicro_flee.py` & `flee-3.0a0/flee/pmicro_flee.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,15 @@
         self,
         startpoint,
         endpoint,
         distance: float,
         forced_redirection: bool = False,
         link_type: Optional[str] = None,
     ):
-        self.name = "L:{}:{}".format(startpoint.name, endpoint.name)
+        self.name = "__link__"
         self.closed = False
 
         # distance in km.
         self.__distance = float(distance)
 
         # links for now always connect two endpoints
         self.startpoint = startpoint
```

### Comparing `flee-3.0/flee/postprocessing/CalculateDiagnostics.py` & `flee-3.0a0/flee/postprocessing/CalculateDiagnostics.py`

 * *Files identical despite different names*

### Comparing `flee-3.0/flee/postprocessing/FormatPyplotFigures.py` & `flee-3.0a0/flee/postprocessing/FormatPyplotFigures.py`

 * *Files identical despite different names*

### Comparing `flee-3.0/flee/postprocessing/PlotRedirectionComparison.py` & `flee-3.0a0/flee/postprocessing/PlotRedirectionComparison.py`

 * *Files identical despite different names*

### Comparing `flee-3.0/flee/postprocessing/StoreDiagnostics.py` & `flee-3.0a0/flee/postprocessing/StoreDiagnostics.py`

 * *Files identical despite different names*

### Comparing `flee-3.0/flee/postprocessing/_version.py` & `flee-3.0a0/flee/postprocessing/_version.py`

 * *Files identical despite different names*

### Comparing `flee-3.0/flee/postprocessing/analysis.py` & `flee-3.0a0/flee/postprocessing/analysis.py`

 * *Files identical despite different names*

### Comparing `flee-3.0/flee/postprocessing/analyze_graph.py` & `flee-3.0a0/flee/postprocessing/analyze_graph.py`

 * *Files identical despite different names*

### Comparing `flee-3.0/flee/postprocessing/compare_out.py` & `flee-3.0a0/flee/postprocessing/compare_out.py`

 * *Files identical despite different names*

### Comparing `flee-3.0/flee/postprocessing/extract-validation-results.py` & `flee-3.0a0/flee/postprocessing/extract-validation-results.py`

 * *Files identical despite different names*

### Comparing `flee-3.0/flee/postprocessing/plot-flee-uq-output-more.py` & `flee-3.0a0/flee/postprocessing/plot-flee-uq-output-more.py`

 * *Files identical despite different names*

### Comparing `flee-3.0/flee/postprocessing/plot_flee_forecast.py` & `flee-3.0a0/flee/postprocessing/plot_flee_forecast.py`

 * *Files identical despite different names*

### Comparing `flee-3.0/flee/postprocessing/plot_flee_output.py` & `flee-3.0a0/flee/postprocessing/plot_flee_output.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,29 +277,29 @@
         ", rescaled: ",
         np.mean(diffdata_rescaled),
         ", len: ",
         len(diffdata),
     )
 
     (labeldiff_rescaled,) = plt.plot(
-        np.arange(len(diffdata_rescaled)), diffdata_rescaled, linewidth=5, label="Error (rescaled)"
+        np.arange(len(diffdata_rescaled)), diffdata_rescaled, linewidth=5, label="Error"
     )
 
     plt.legend(handles=[labeldiff_rescaled], loc=7, prop={"size": 14})
 
     set_margins()
 
     plt.savefig("{}/error.png".format(output), bbox_inches = 'tight')
 
     ###############################################
     #               ERROR COMPARISON              #
     ###############################################
 
     (labeldiff,) = plt.plot(
-        np.arange(len(diffdata)), diffdata, linewidth=5, label="Error (non-rescaled)"
+        np.arange(len(diffdata)), diffdata, linewidth=5, label="error (not rescaled)"
     )
 
     plt.legend(handles=[labeldiff, labeldiff_rescaled], loc=1, prop={"size": 14})
 
     set_margins()
 
     plt.savefig("{}/error_comparison.png".format(output), bbox_inches = 'tight')
```

### Comparing `flee-3.0/flee/postprocessing/plot_flee_uq_output.py` & `flee-3.0a0/flee/postprocessing/plot_flee_uq_output.py`

 * *Files identical despite different names*

### Comparing `flee-3.0/flee/postprocessing/plotter.py` & `flee-3.0a0/flee/postprocessing/plotter.py`

 * *Files identical despite different names*

### Comparing `flee-3.0/flee/spawning.py` & `flee-3.0a0/flee/spawning.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,22 +42,22 @@
         # First reset weight to 0.0.
         e.spawn_weights[i] = 0.0
 
         # Conflict-driven spawning
         if not SimulationSettings.spawn_rules["conflict_driven_spawning"]: # This branch should be skipped if conflicts spawn fixed numbers of agents.
 
             if SimulationSettings.spawn_rules["conflict_zone_spawning_only"]: # This option reduces spawning to 0 in non-conflict zones.
-                if e.locations[i].conflict <= 0.0:
+                if e.locations[i].conflict == False:
                     continue
 
-            if e.locations[i].conflict > 0.0: # Adding conflict-based weighting for spawning.
+            if e.locations[i].conflict == True: # Adding conflict-based weighting for spawning.
                 # Conflict decay multiplier
-                multiplier = e.locations[i].conflict
+                multiplier = 1.0
                 if SimulationSettings.spawn_rules["conflict_spawn_decay"]:
-                    multiplier = e.locations[i].conflict * SimulationSettings.get_location_conflict_decay(e.time, e.locations[i])
+                    multiplier = SimulationSettings.get_location_conflict_decay(e.time, e.locations[i])
 
                 # Pop+conflict weight
                 e.spawn_weights[i] = e.locations[i].pop * conflict_pop_weight * multiplier
 
 
     e.spawn_weight_total = sum(e.spawn_weights)
 
@@ -65,15 +65,15 @@
 
 def read_demographic_csv(e, csvname):
   """
   Attribute CSV files have the following format:
   Value,Default,LocA,LocB,...
   ValueA,weight for that value by Default, ...
   """
-  attribute = (csvname.split(os.sep)[1].split('.')[0]).split('_')[1]
+  attribute = (csvname.split('/')[1].split('.')[0]).split('_')[1]
 
   if not os.path.exists(csvname):
       return
 
   df = pd.read_csv(csvname)
 
   if SimulationSettings.log_levels["init"] > -1:
@@ -82,106 +82,107 @@
   __demographics[attribute] = df
 
 
 def read_demographics(e):
   if not os.path.exists("input_csv"):
       return
 
-  csv_list = glob.glob(os.path.join("input_csv","demographics_*.csv"))
+  csv_list = glob.glob("input_csv/demographics_*.csv")
 
   for csvname in csv_list:
       read_demographic_csv(e, csvname)
   
 
 
 def draw_sample(e, loc, attribute):
   #print(__demographics[attribute], file=sys.stderr)
   #print(__demographics[attribute].iloc[0]['Default'], file=sys.stderr)
 
   if attribute in __demographics:
     if loc.name in __demographics[attribute].columns:
-      a = __demographics[attribute].sample(n=1,weights=loc.name)
+      a = __demographics[attribute].sample(n=1,weights=loc)
     else:
       a = __demographics[attribute].sample(n=1,weights='Default')
   else:
     return -1
 
   return a.iloc[0][attribute]
 
 
 def draw_samples(e,loc):
     """
-    Draw samples from all optional attributes.
+    Draw samples from all optional attributes, except age and gender (which are always provided).
     """
     samples = {}
     for a in __demographics.keys():
-        samples[a] = draw_sample(e, loc, a)
+        if a == "age" or a == "gender":
+            continue
+        else:
+            samples[a] = draw_sample(e, loc, a)
     return samples
 
 
 def add_initial_refugees(e, d, loc):
   """ Add the initial refugees to a location, using the location name"""
 
   # Only initialize demographics when first called.
   if len(__demographics) == 0:
       read_demographics(e)
 
 
   if SimulationSettings.spawn_rules["InsertDayZeroRefugeesInCamps"]:
       num_refugees = int(d.get_field(loc.name, 0, FullInterpolation=True))
       for i in range(0, num_refugees):
+          age = draw_sample(e, loc, 'age')
+          gender = draw_sample(e, loc, 'gender')
           attributes = draw_samples(e, loc)
-          e.addAgent(location=loc, attributes=attributes) # Parallelization is incorporated *inside* the addAgent function.
+          e.addAgent(location=loc, age=age, gender=gender, attributes=attributes) # Parallelization is incorporated *inside* the addAgent function.
 
 
-def spawn_daily_displaced(e, t, d, SumFromCamps=False):
+def spawn_daily_displaced(e, t, d):
     global __refugees_raw, __refugee_debt
     """
     t = time
     e = Ecosystem object
     d = DataTable object
     refugees_raw = raw refugee count
     """
-    new_refs = 0
 
     if SimulationSettings.spawn_rules["conflict_driven_spawning"]:
 
       for i in range(0, len(e.locations)):
  
         ## BASE RATES  
         if SimulationSettings.spawn_rules["conflict_spawn_mode"] == "constant":
-            if e.locations[i].conflict > 0.0:
-                num_spawned = int(SimulationSettings.spawn_rules["displaced_per_conflict_day"] * e.locations[i].conflict)
-            else:
-                num_spawned = 0
+            num_spawned = SimulationSettings.spawn_rules["displaced_per_conflict_day"]
 
         elif SimulationSettings.spawn_rules["conflict_spawn_mode"] == "pop_ratio":
-            if e.locations[i].conflict > 0.0:  
-                num_spawned = int(SimulationSettings.spawn_rules["displaced_per_conflict_day"] * e.locations[i].pop * e.locations[i].conflict)
+            if e.locations[i].conflict:  
+                num_spawned = int(SimulationSettings.spawn_rules["displaced_per_conflict_day"] * e.locations[i].pop)
             else: 
                 num_spawned = 0
 
         elif SimulationSettings.spawn_rules["conflict_spawn_mode"].lower() == "Poisson":
-            if e.locations[i].conflict > 0.0:  
-                num_spawned = np.random.poisson(SimulationSettings.spawn_rules["displaced_per_conflict_day"] * e.locations[i].conflict)
+            if e.locations[i].conflict:  
+                num_spawned = np.random.poisson(SimulationSettings.spawn_rules["displaced_per_conflict_day"])
             else: 
                 num_spawned = 0
 
         ## Doing the actual spawning here.
         for j in range(0, num_spawned):
-            attributes = draw_samples(e, e.locations[i])
-            e.addAgent(location=e.locations[i], attributes=attributes) # Parallelization is incorporated *inside* the addAgent function.
-
-        new_refs = num_spawned
+            age = draw_sample(e, e.locations[i], 'age')
+            gender = draw_sample(e, e.locations[i], 'gender')
+            attributes = draw_samples(e, loc)
+            e.addAgent(location=e.locations[i], age=age, gender=gender, attributes=attributes) # Parallelization is incorporated *inside* the addAgent function.
 
     else:
 
       # Determine number of new refugees to insert into the system.
-      new_refs = d.get_daily_difference(t, FullInterpolation=True, SumFromCamps=SumFromCamps) - __refugee_debt
-      __refugees_raw += d.get_daily_difference(t, FullInterpolation=True, SumFromCamps=SumFromCamps)
+      new_refs = d.get_daily_difference(t, FullInterpolation=True, SumFromCamps=False) - __refugee_debt
+      __refugees_raw += d.get_daily_difference(t, FullInterpolation=True, SumFromCamps=False)
 
       #Refugees are pre-placed in Mali, so set new_refs to 0 on Day 0.
       if SimulationSettings.spawn_rules["InsertDayZeroRefugeesInCamps"]:
         if t == 0:
           new_refs = 0
           #refugees_raw = 0
 
@@ -190,21 +191,13 @@
         new_refs = 0
       elif __refugee_debt > 0:
         __refugee_debt = 0
 
       #Insert refugee agents
       for i in range(0, new_refs):
         loc = e.pick_spawn_location()
+        age = draw_sample(e, loc, 'age')
+        gender = draw_sample(e, loc, 'gender')
         attributes = draw_samples(e, loc)
-        e.addAgent(location=loc, attributes=attributes) # Parallelization is incorporated *inside* the addAgent function.
+        e.addAgent(location=loc, age=age, gender=gender, attributes=attributes) # Parallelization is incorporated *inside* the addAgent function.
 
     return new_refs, __refugees_raw, __refugee_debt
-
-
-def spawn_agents(e, number):
-
-    #Insert refugee agents
-    for i in range(0, number):
-        loc = e.pick_spawn_location()
-        attributes = draw_samples(e, loc)
-        e.addAgent(location=loc, attributes=attributes) # Parallelization is incorporated *inside* the addAgent function.
-
```

### Comparing `flee-3.0/flee.egg-info/SOURCES.txt` & `flee-3.0a0/flee.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -36,26 +36,11 @@
 flee/postprocessing/__init__.py
 flee/postprocessing/_version.py
 flee/postprocessing/analysis.py
 flee/postprocessing/analyze_graph.py
 flee/postprocessing/compare_out.py
 flee/postprocessing/extract-validation-results.py
 flee/postprocessing/plot-flee-uq-output-more.py
-flee/postprocessing/plot_flee_compare.py
 flee/postprocessing/plot_flee_forecast.py
 flee/postprocessing/plot_flee_output.py
 flee/postprocessing/plot_flee_uq_output.py
-flee/postprocessing/plotter.py
-tests/test_1_agent.py
-tests/test_awareness.py
-tests/test_camp_sink.py
-tests/test_close_location.py
-tests/test_conflict_driven_spawning.py
-tests/test_csv.py
-tests/test_datatable.py
-tests/test_load_agent.py
-tests/test_micro_model.py
-tests/test_moving.py
-tests/test_path_choice.py
-tests/test_removelink.py
-tests/test_tiny_closure.py
-tests/test_toy_escape.py
+flee/postprocessing/plotter.py
```

### Comparing `flee-3.0/setup.py` & `flee-3.0a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,25 +28,25 @@
 test_requirements = ["pytest>=3", ]
 
 cmdclass = versioneer.get_cmdclass()
 
 setup(
     author="Derek Groen",
     author_email="Derek.Groen@brunel.ac.uk",
-    python_requires=">=3.8",
+    python_requires=">=3.6",
     classifiers=[
         # list of classifiers -> https://pypi.org/classifiers/
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
     ],
     description="Flee is an agent-based modelling toolkit which is "
     "purpose-built for simulating the movement of individuals "
     "across geographical locations.",
     install_requires=install_requires,
     license="BSD-3-Clause",
     long_description=long_description,
@@ -57,8 +57,8 @@
     packages=find_packages(include=["flee", "flee.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://flee.readthedocs.io",
     version=versioneer.get_version(),
     cmdclass=cmdclass,
     zip_safe=False,
-    )
+)
```

### Comparing `flee-3.0/versioneer.py` & `flee-3.0a0/versioneer.py`

 * *Files identical despite different names*

