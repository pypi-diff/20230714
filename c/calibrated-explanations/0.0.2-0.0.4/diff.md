# Comparing `tmp/calibrated-explanations-0.0.2.tar.gz` & `tmp/calibrated-explanations-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calibrated-explanations-0.0.2.tar", last modified: Fri Jul 14 09:45:06 2023, max compression
+gzip compressed data, was "calibrated-explanations-0.0.4.tar", last modified: Fri Jul 14 11:50:44 2023, max compression
```

## Comparing `calibrated-explanations-0.0.2.tar` & `calibrated-explanations-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 rryy      (1000) rryy      (1000)        0 2023-07-14 09:45:06.733500 calibrated-explanations-0.0.2/
--rw-r--r--   0 rryy      (1000) rryy      (1000)     1064 2023-07-10 15:03:28.000000 calibrated-explanations-0.0.2/LICENSE
--rw-r--r--   0 rryy      (1000) rryy      (1000)     2258 2023-07-14 09:45:06.733500 calibrated-explanations-0.0.2/PKG-INFO
--rw-r--r--   0 rryy      (1000) rryy      (1000)     1630 2023-07-14 09:41:13.000000 calibrated-explanations-0.0.2/README.md
-drwxr-xr-x   0 rryy      (1000) rryy      (1000)        0 2023-07-14 09:45:06.730166 calibrated-explanations-0.0.2/calibrated_explanations/
-drwxr-xr-x   0 rryy      (1000) rryy      (1000)        0 2023-07-14 09:45:06.733500 calibrated-explanations-0.0.2/calibrated_explanations/calibrated_explanations.egg-info/
--rw-r--r--   0 rryy      (1000) rryy      (1000)     2258 2023-07-14 09:45:06.000000 calibrated-explanations-0.0.2/calibrated_explanations/calibrated_explanations.egg-info/PKG-INFO
--rw-r--r--   0 rryy      (1000) rryy      (1000)      449 2023-07-14 09:45:06.000000 calibrated-explanations-0.0.2/calibrated_explanations/calibrated_explanations.egg-info/SOURCES.txt
--rw-r--r--   0 rryy      (1000) rryy      (1000)        1 2023-07-14 09:45:06.000000 calibrated-explanations-0.0.2/calibrated_explanations/calibrated_explanations.egg-info/dependency_links.txt
--rw-r--r--   0 rryy      (1000) rryy      (1000)       78 2023-07-14 09:45:06.000000 calibrated-explanations-0.0.2/calibrated_explanations/calibrated_explanations.egg-info/requires.txt
--rw-r--r--   0 rryy      (1000) rryy      (1000)        1 2023-07-14 09:45:06.000000 calibrated-explanations-0.0.2/calibrated_explanations/calibrated_explanations.egg-info/top_level.txt
--rw-r--r--   0 rryy      (1000) rryy      (1000)      833 2023-07-14 09:41:13.000000 calibrated-explanations-0.0.2/pyproject.toml
--rw-r--r--   0 rryy      (1000) rryy      (1000)       38 2023-07-14 09:45:06.733500 calibrated-explanations-0.0.2/setup.cfg
--rw-r--r--   0 rryy      (1000) rryy      (1000)      170 2023-07-12 09:59:43.000000 calibrated-explanations-0.0.2/setup.py
-drwxr-xr-x   0 rryy      (1000) rryy      (1000)        0 2023-07-14 09:45:06.733500 calibrated-explanations-0.0.2/tests/
--rw-r--r--   0 rryy      (1000) rryy      (1000)     8488 2023-07-14 09:40:31.000000 calibrated-explanations-0.0.2/tests/test_classification.py
--rw-r--r--   0 rryy      (1000) rryy      (1000)    15237 2023-07-14 09:40:31.000000 calibrated-explanations-0.0.2/tests/test_regression.py
+drwxr-xr-x   0 rudy      (1080) rudy      (1080)        0 2023-07-14 11:50:44.663289 calibrated-explanations-0.0.4/
+-rw-r--r--   0 rudy      (1080) rudy      (1080)     1064 2023-07-05 15:11:26.000000 calibrated-explanations-0.0.4/LICENSE
+-rw-r--r--   0 rudy      (1080) rudy      (1080)     2535 2023-07-14 11:50:44.663289 calibrated-explanations-0.0.4/PKG-INFO
+-rw-r--r--   0 rudy      (1080) rudy      (1080)     1907 2023-07-14 11:46:58.000000 calibrated-explanations-0.0.4/README.md
+drwxr-xr-x   0 rudy      (1080) rudy      (1080)        0 2023-07-14 11:50:44.656623 calibrated-explanations-0.0.4/calibrated_explanations/
+drwxr-xr-x   0 rudy      (1080) rudy      (1080)        0 2023-07-14 11:50:44.659956 calibrated-explanations-0.0.4/calibrated_explanations/calibrated_explanations.egg-info/
+-rw-r--r--   0 rudy      (1080) rudy      (1080)     2535 2023-07-14 11:50:44.000000 calibrated-explanations-0.0.4/calibrated_explanations/calibrated_explanations.egg-info/PKG-INFO
+-rw-r--r--   0 rudy      (1080) rudy      (1080)      449 2023-07-14 11:50:44.000000 calibrated-explanations-0.0.4/calibrated_explanations/calibrated_explanations.egg-info/SOURCES.txt
+-rw-r--r--   0 rudy      (1080) rudy      (1080)        1 2023-07-14 11:50:44.000000 calibrated-explanations-0.0.4/calibrated_explanations/calibrated_explanations.egg-info/dependency_links.txt
+-rw-r--r--   0 rudy      (1080) rudy      (1080)       67 2023-07-14 11:50:44.000000 calibrated-explanations-0.0.4/calibrated_explanations/calibrated_explanations.egg-info/requires.txt
+-rw-r--r--   0 rudy      (1080) rudy      (1080)        1 2023-07-14 11:50:44.000000 calibrated-explanations-0.0.4/calibrated_explanations/calibrated_explanations.egg-info/top_level.txt
+-rw-r--r--   0 rudy      (1080) rudy      (1080)      812 2023-07-14 11:50:35.000000 calibrated-explanations-0.0.4/pyproject.toml
+-rw-r--r--   0 rudy      (1080) rudy      (1080)       38 2023-07-14 11:50:44.663289 calibrated-explanations-0.0.4/setup.cfg
+-rw-r--r--   0 rudy      (1080) rudy      (1080)      170 2023-07-12 11:33:21.000000 calibrated-explanations-0.0.4/setup.py
+drwxr-xr-x   0 rudy      (1080) rudy      (1080)        0 2023-07-14 11:50:44.663289 calibrated-explanations-0.0.4/tests/
+-rw-r--r--   0 rudy      (1080) rudy      (1080)     8488 2023-07-12 15:02:18.000000 calibrated-explanations-0.0.4/tests/test_classification.py
+-rw-r--r--   0 rudy      (1080) rudy      (1080)    15237 2023-07-12 15:02:18.000000 calibrated-explanations-0.0.4/tests/test_regression.py
```

### Comparing `calibrated-explanations-0.0.2/LICENSE` & `calibrated-explanations-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `calibrated-explanations-0.0.2/PKG-INFO` & `calibrated-explanations-0.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calibrated-explanations
-Version: 0.0.2
+Version: 0.0.4
 Summary: Extract calibrated explanations from machine learning models.
 Author-email: Helena Löfström <helena.lofstrom@ju.se>
 Project-URL: Homepage, https://github.com/Moffran/calibrated_explanations
 Project-URL: Bug Tracker, https://github.com/Moffran/calibrated_explanations/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,14 +12,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Calibrated Explanations
 =======================
 
+[![Calibrated Explanations PyPI version][pypi-version]][calibrated-explanations-on-pypi]
 [![Build Status for Calibrated Explanations][build-status]][build-log]
 
 Calibrated Explanations is a Python library
 that is able to explain predictions of a black-box model
 using Venn Abers predictors (classification)
 or conformal predictive systems (regression) and perturbations.
 
@@ -66,16 +67,18 @@
 
 Further reading
 ---------------
 
 The calibrated explanations library is based on the paper
 "Calibrated Explanations for Black-Box Predictions"
 by
-Helena Löfström,
+[Helena Löfström](https://github.com/Moffran),
 [Tuwe Löfström](https://github.com/tuvelofstrom),
 Ulf Johansson and
 Cecilia Sönströd.
 
 If you would like to cite this work, please cite the above paper.
 
-[build-log]:    https://github.com/Moffran/calibrated_explanations/actions/workflows/ce.yml
-[build-status]: https://github.com/Moffran/calibrated_explanations/actions/workflows/ce.yml/badge.svg
+[build-log]:    https://github.com/Moffran/calibrated_explanations/actions/workflows/test.yml
+[build-status]: https://github.com/Moffran/calibrated_explanations/actions/workflows/test.yml/badge.svg
+[pypi-version]: https://img.shields.io/pypi/v/calibrated-explanations
+[calibrated-explanations-on-pypi]: https://pypi.org/project/calibrated-explanations
```

### Comparing `calibrated-explanations-0.0.2/README.md` & `calibrated-explanations-0.0.4/calibrated_explanations/calibrated_explanations.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,26 @@
+Metadata-Version: 2.1
+Name: calibrated-explanations
+Version: 0.0.4
+Summary: Extract calibrated explanations from machine learning models.
+Author-email: Helena Löfström <helena.lofstrom@ju.se>
+Project-URL: Homepage, https://github.com/Moffran/calibrated_explanations
+Project-URL: Bug Tracker, https://github.com/Moffran/calibrated_explanations/issues
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 Calibrated Explanations
 =======================
 
+[![Calibrated Explanations PyPI version][pypi-version]][calibrated-explanations-on-pypi]
 [![Build Status for Calibrated Explanations][build-status]][build-log]
 
 Calibrated Explanations is a Python library
 that is able to explain predictions of a black-box model
 using Venn Abers predictors (classification)
 or conformal predictive systems (regression) and perturbations.
 
@@ -51,16 +67,18 @@
 
 Further reading
 ---------------
 
 The calibrated explanations library is based on the paper
 "Calibrated Explanations for Black-Box Predictions"
 by
-Helena Löfström,
+[Helena Löfström](https://github.com/Moffran),
 [Tuwe Löfström](https://github.com/tuvelofstrom),
 Ulf Johansson and
 Cecilia Sönströd.
 
 If you would like to cite this work, please cite the above paper.
 
-[build-log]:    https://github.com/Moffran/calibrated_explanations/actions/workflows/ce.yml
-[build-status]: https://github.com/Moffran/calibrated_explanations/actions/workflows/ce.yml/badge.svg
+[build-log]:    https://github.com/Moffran/calibrated_explanations/actions/workflows/test.yml
+[build-status]: https://github.com/Moffran/calibrated_explanations/actions/workflows/test.yml/badge.svg
+[pypi-version]: https://img.shields.io/pypi/v/calibrated-explanations
+[calibrated-explanations-on-pypi]: https://pypi.org/project/calibrated-explanations
```

### Comparing `calibrated-explanations-0.0.2/pyproject.toml` & `calibrated-explanations-0.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 [project]
 name = "calibrated-explanations"
-version = "0.0.2"
+version = "0.0.4"
 authors = [
   { name="Helena Löfström", email="helena.lofstrom@ju.se" },
 ]
 description = "Extract calibrated explanations from machine learning models."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
+  'crepes',
+  'ipython',
+  'lime',
+  'matplotlib',
   'numpy',
   'pandas',
   'scikit-learn',
-  'matplotlib',
-  'lime',
   'shap',
-  'crepes',
-  'typing',
   'tqdm',
-  'random',
-  'copy',
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `calibrated-explanations-0.0.2/tests/test_classification.py` & `calibrated-explanations-0.0.4/tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `calibrated-explanations-0.0.2/tests/test_regression.py` & `calibrated-explanations-0.0.4/tests/test_regression.py`

 * *Files identical despite different names*

