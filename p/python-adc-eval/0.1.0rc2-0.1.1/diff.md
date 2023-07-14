# Comparing `tmp/python-adc-eval-0.1.0rc2.tar.gz` & `tmp/python-adc-eval-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-adc-eval-0.1.0rc2.tar", last modified: Thu Jul 13 20:48:54 2023, max compression
+gzip compressed data, was "python-adc-eval-0.1.1.tar", last modified: Fri Jul 14 14:22:53 2023, max compression
```

## Comparing `python-adc-eval-0.1.0rc2.tar` & `python-adc-eval-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:48:54.225708 python-adc-eval-0.1.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-13 20:48:37.000000 python-adc-eval-0.1.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 20:48:37.000000 python-adc-eval-0.1.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-13 20:48:54.225708 python-adc-eval-0.1.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-13 20:48:37.000000 python-adc-eval-0.1.0rc2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:48:54.225708 python-adc-eval-0.1.0rc2/adc_eval/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 20:48:37.000000 python-adc-eval-0.1.0rc2/adc_eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-13 20:48:37.000000 python-adc-eval-0.1.0rc2/adc_eval/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-13 20:48:37.000000 python-adc-eval-0.1.0rc2/adc_eval/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10545 2023-07-13 20:48:37.000000 python-adc-eval-0.1.0rc2/adc_eval/spectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-13 20:48:37.000000 python-adc-eval-0.1.0rc2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:48:54.225708 python-adc-eval-0.1.0rc2/python_adc_eval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-13 20:48:54.000000 python-adc-eval-0.1.0rc2/python_adc_eval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-13 20:48:54.000000 python-adc-eval-0.1.0rc2/python_adc_eval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 20:48:54.000000 python-adc-eval-0.1.0rc2/python_adc_eval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-13 20:48:54.000000 python-adc-eval-0.1.0rc2/python_adc_eval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 20:48:54.000000 python-adc-eval-0.1.0rc2/python_adc_eval.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-13 20:48:37.000000 python-adc-eval-0.1.0rc2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 20:48:54.225708 python-adc-eval-0.1.0rc2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:22:53.717265 python-adc-eval-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-14 14:22:33.000000 python-adc-eval-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-14 14:22:33.000000 python-adc-eval-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-14 14:22:53.717265 python-adc-eval-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-14 14:22:33.000000 python-adc-eval-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:22:53.713266 python-adc-eval-0.1.1/adc_eval/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-14 14:22:33.000000 python-adc-eval-0.1.1/adc_eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-14 14:22:33.000000 python-adc-eval-0.1.1/adc_eval/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-14 14:22:33.000000 python-adc-eval-0.1.1/adc_eval/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10545 2023-07-14 14:22:33.000000 python-adc-eval-0.1.1/adc_eval/spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-07-14 14:22:33.000000 python-adc-eval-0.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:22:53.713266 python-adc-eval-0.1.1/python_adc_eval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-14 14:22:53.000000 python-adc-eval-0.1.1/python_adc_eval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-14 14:22:53.000000 python-adc-eval-0.1.1/python_adc_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 14:22:53.000000 python-adc-eval-0.1.1/python_adc_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 14:22:53.000000 python-adc-eval-0.1.1/python_adc_eval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 14:22:53.000000 python-adc-eval-0.1.1/python_adc_eval.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 14:22:33.000000 python-adc-eval-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 14:22:53.717265 python-adc-eval-0.1.1/setup.cfg
```

### Comparing `python-adc-eval-0.1.0rc2/LICENSE` & `python-adc-eval-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-adc-eval-0.1.0rc2/PKG-INFO` & `python-adc-eval-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-adc-eval
-Version: 0.1.0rc2
+Version: 0.1.1
 Summary: ADC Evaluation Library
 Author-email: Kevin Fronczak <kfronczak@gmail.com>
 License: MIT
 Project-URL: Source Code, https://github.com/fronzbot/python-adc-eval
 Project-URL: Bug Reports, https://github.com/fronzbot/python-adc-eval/issues
 Keywords: adc,analog-to-digital,evaluation,eval,spectrum
 Platform: any
```

### Comparing `python-adc-eval-0.1.0rc2/README.rst` & `python-adc-eval-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `python-adc-eval-0.1.0rc2/adc_eval/converters.py` & `python-adc-eval-0.1.1/adc_eval/converters.py`

 * *Files identical despite different names*

### Comparing `python-adc-eval-0.1.0rc2/adc_eval/spectrum.py` & `python-adc-eval-0.1.1/adc_eval/spectrum.py`

 * *Files identical despite different names*

### Comparing `python-adc-eval-0.1.0rc2/pyproject.toml` & `python-adc-eval-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=68.0", "wheel~=0.40.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-adc-eval"
-version = "0.1.0rc2"
+version = "0.1.1"
 license = {text = "MIT"}
 description = "ADC Evaluation Library"
 readme = "README.rst"
 authors = [{name = "Kevin Fronczak", email = "kfronczak@gmail.com"}]
 keywords = ["adc", "analog-to-digital", "evaluation", "eval", "spectrum"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -75,14 +75,16 @@
     "PLR2004",  # Magic value used in comparison, consider replacing {value} with a constant variable
     "PLW2901", # Outer {outer_kind} variable {name} overwritten by inner {inner_kind} target
     "UP006", # keep type annotation style as is
     "UP007", # keep type annotation style as is
     # Ignored due to performance: https://github.com/charliermarsh/ruff/issues/2923
     "UP038", # Use `X | Y` in `isinstance` call instead of `(X, Y)`
 ]
-
+exclude = [
+    "__init__.py",
+]
 line-length = 88
 
 target-version = "py39"
 
 [tool.ruff.mccabe]
 max-complexity = 10
```

### Comparing `python-adc-eval-0.1.0rc2/python_adc_eval.egg-info/PKG-INFO` & `python-adc-eval-0.1.1/python_adc_eval.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-adc-eval
-Version: 0.1.0rc2
+Version: 0.1.1
 Summary: ADC Evaluation Library
 Author-email: Kevin Fronczak <kfronczak@gmail.com>
 License: MIT
 Project-URL: Source Code, https://github.com/fronzbot/python-adc-eval
 Project-URL: Bug Reports, https://github.com/fronzbot/python-adc-eval/issues
 Keywords: adc,analog-to-digital,evaluation,eval,spectrum
 Platform: any
```

