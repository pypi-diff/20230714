# Comparing `tmp/python-adc-eval-0.1.2rc0.tar.gz` & `tmp/python-adc-eval-0.1.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-adc-eval-0.1.2rc0.tar", last modified: Fri Jul 14 20:08:02 2023, max compression
+gzip compressed data, was "python-adc-eval-0.1.2rc1.tar", last modified: Fri Jul 14 20:14:30 2023, max compression
```

## Comparing `python-adc-eval-0.1.2rc0.tar` & `python-adc-eval-0.1.2rc1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:08:02.094678 python-adc-eval-0.1.2rc0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-14 20:07:43.000000 python-adc-eval-0.1.2rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-14 20:07:43.000000 python-adc-eval-0.1.2rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-14 20:08:02.094678 python-adc-eval-0.1.2rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-14 20:07:43.000000 python-adc-eval-0.1.2rc0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:08:02.094678 python-adc-eval-0.1.2rc0/adc_eval/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-14 20:07:43.000000 python-adc-eval-0.1.2rc0/adc_eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-14 20:07:43.000000 python-adc-eval-0.1.2rc0/adc_eval/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-14 20:07:43.000000 python-adc-eval-0.1.2rc0/adc_eval/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10545 2023-07-14 20:07:43.000000 python-adc-eval-0.1.2rc0/adc_eval/spectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-07-14 20:07:43.000000 python-adc-eval-0.1.2rc0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:08:02.094678 python-adc-eval-0.1.2rc0/python_adc_eval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-14 20:08:02.000000 python-adc-eval-0.1.2rc0/python_adc_eval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-14 20:08:02.000000 python-adc-eval-0.1.2rc0/python_adc_eval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 20:08:02.000000 python-adc-eval-0.1.2rc0/python_adc_eval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 20:08:02.000000 python-adc-eval-0.1.2rc0/python_adc_eval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 20:08:02.000000 python-adc-eval-0.1.2rc0/python_adc_eval.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 20:07:43.000000 python-adc-eval-0.1.2rc0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 20:08:02.094678 python-adc-eval-0.1.2rc0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:14:30.439318 python-adc-eval-0.1.2rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-14 20:14:11.000000 python-adc-eval-0.1.2rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-14 20:14:11.000000 python-adc-eval-0.1.2rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-14 20:14:30.439318 python-adc-eval-0.1.2rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-14 20:14:11.000000 python-adc-eval-0.1.2rc1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:14:30.439318 python-adc-eval-0.1.2rc1/adc_eval/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-14 20:14:11.000000 python-adc-eval-0.1.2rc1/adc_eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-14 20:14:11.000000 python-adc-eval-0.1.2rc1/adc_eval/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-14 20:14:11.000000 python-adc-eval-0.1.2rc1/adc_eval/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-07-14 20:14:11.000000 python-adc-eval-0.1.2rc1/adc_eval/spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-07-14 20:14:11.000000 python-adc-eval-0.1.2rc1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:14:30.439318 python-adc-eval-0.1.2rc1/python_adc_eval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-14 20:14:30.000000 python-adc-eval-0.1.2rc1/python_adc_eval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-14 20:14:30.000000 python-adc-eval-0.1.2rc1/python_adc_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 20:14:30.000000 python-adc-eval-0.1.2rc1/python_adc_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 20:14:30.000000 python-adc-eval-0.1.2rc1/python_adc_eval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 20:14:30.000000 python-adc-eval-0.1.2rc1/python_adc_eval.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 20:14:11.000000 python-adc-eval-0.1.2rc1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 20:14:30.439318 python-adc-eval-0.1.2rc1/setup.cfg
```

### Comparing `python-adc-eval-0.1.2rc0/LICENSE` & `python-adc-eval-0.1.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-adc-eval-0.1.2rc0/PKG-INFO` & `python-adc-eval-0.1.2rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-adc-eval
-Version: 0.1.2rc0
+Version: 0.1.2rc1
 Summary: ADC Evaluation Library
 Author-email: Kevin Fronczak <kfronczak@gmail.com>
 License: MIT
 Project-URL: Source Code, https://github.com/fronzbot/python-adc-eval
 Project-URL: Bug Reports, https://github.com/fronzbot/python-adc-eval/issues
 Keywords: adc,analog-to-digital,evaluation,eval,spectrum
 Platform: any
```

### Comparing `python-adc-eval-0.1.2rc0/README.rst` & `python-adc-eval-0.1.2rc1/README.rst`

 * *Files identical despite different names*

### Comparing `python-adc-eval-0.1.2rc0/adc_eval/converters.py` & `python-adc-eval-0.1.2rc1/adc_eval/converters.py`

 * *Files identical despite different names*

### Comparing `python-adc-eval-0.1.2rc0/adc_eval/spectrum.py` & `python-adc-eval-0.1.2rc1/adc_eval/spectrum.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,19 +57,19 @@
         "hamming": {"cg": 0.54, "npb": 1.36},
         "blackman": {"cg": 0.42, "npb": 1.73},
     }[window]
     fft_n = len(psp) * 2  # one side spectrum provided
     df = sample_freq / fft_n
     # calculate fundamental frequency
     fund_bin = np.argmax(psp)
-    fund_freq = np.sum(
-        [psp[i] * i * df for i in range(fund_bin - leak, fund_bin + leak + 1)]
-    ) / np.sum(psp[fund_bin - leak : fund_bin + leak + 1])
-    if np.isinf:
-        fund_freq = fund_bin * df
+    fund_freq = fund_bin * df
+    num = np.sum([psp[i] * i * df for i in range(fund_bin - leak, fund_bin + leak + 1)])
+    den = np.sum(psp[fund_bin - leak : fund_bin + leak + 1])
+    if den > 0:
+        fund_freq = num / den
 
     # calculate harmonics info
     h = []
     for i in range(1, n + 1):
         h_i = {"num": i}
         zone_freq = (fund_freq * i) % sample_freq
         h_i["freq"] = (
```

### Comparing `python-adc-eval-0.1.2rc0/pyproject.toml` & `python-adc-eval-0.1.2rc1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=68.0", "wheel~=0.40.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-adc-eval"
-version = "0.1.2.rc0"
+version = "0.1.2rc1"
 license = {text = "MIT"}
 description = "ADC Evaluation Library"
 readme = "README.rst"
 authors = [{name = "Kevin Fronczak", email = "kfronczak@gmail.com"}]
 keywords = ["adc", "analog-to-digital", "evaluation", "eval", "spectrum"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `python-adc-eval-0.1.2rc0/python_adc_eval.egg-info/PKG-INFO` & `python-adc-eval-0.1.2rc1/python_adc_eval.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-adc-eval
-Version: 0.1.2rc0
+Version: 0.1.2rc1
 Summary: ADC Evaluation Library
 Author-email: Kevin Fronczak <kfronczak@gmail.com>
 License: MIT
 Project-URL: Source Code, https://github.com/fronzbot/python-adc-eval
 Project-URL: Bug Reports, https://github.com/fronzbot/python-adc-eval/issues
 Keywords: adc,analog-to-digital,evaluation,eval,spectrum
 Platform: any
```

