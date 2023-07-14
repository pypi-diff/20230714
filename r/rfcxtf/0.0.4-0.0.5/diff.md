# Comparing `tmp/rfcxtf-0.0.4.tar.gz` & `tmp/rfcxtf-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfcxtf-0.0.4.tar", last modified: Thu Jul 13 17:42:23 2023, max compression
+gzip compressed data, was "rfcxtf-0.0.5.tar", last modified: Fri Jul 14 11:13:09 2023, max compression
```

## Comparing `rfcxtf-0.0.4.tar` & `rfcxtf-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 17:42:23.487449 rfcxtf-0.0.4/
--rw-r--r--   0 root         (0) root         (0)      482 2023-07-13 17:42:23.486313 rfcxtf-0.0.4/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 17:42:23.436553 rfcxtf-0.0.4/rfcxtf/
--rw-r--r--   0 root         (0) root         (0)      593 2023-05-04 09:58:45.000000 rfcxtf-0.0.4/rfcxtf/ClassifierBase.py
--rw-r--r--   0 root         (0) root         (0)     2602 2023-05-04 10:33:29.000000 rfcxtf-0.0.4/rfcxtf/ClassifierTF2.py
--rw-r--r--   0 root         (0) root         (0)       58 2023-05-04 10:26:02.000000 rfcxtf-0.0.4/rfcxtf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 17:42:23.481461 rfcxtf-0.0.4/rfcxtf/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 11:11:18.000000 rfcxtf-0.0.4/rfcxtf/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)       48 2023-05-04 09:05:14.000000 rfcxtf-0.0.4/rfcxtf/utils/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      272 2023-05-04 09:05:14.000000 rfcxtf-0.0.4/rfcxtf/utils/io.py
--rw-r--r--   0 root         (0) root         (0)      321 2023-05-04 09:05:14.000000 rfcxtf-0.0.4/rfcxtf/utils/postprocessor.py
--rw-r--r--   0 root         (0) root         (0)     3492 2023-07-08 19:32:57.000000 rfcxtf-0.0.4/rfcxtf/validate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 17:42:23.462453 rfcxtf-0.0.4/rfcxtf.egg-info/
--rw-r--r--   0 root         (0) root         (0)      482 2023-07-13 17:42:23.000000 rfcxtf-0.0.4/rfcxtf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      345 2023-07-13 17:42:23.000000 rfcxtf-0.0.4/rfcxtf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 17:42:23.000000 rfcxtf-0.0.4/rfcxtf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-13 17:42:23.000000 rfcxtf-0.0.4/rfcxtf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-13 17:42:23.000000 rfcxtf-0.0.4/rfcxtf.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 17:42:23.488033 rfcxtf-0.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      778 2023-07-13 17:41:19.000000 rfcxtf-0.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:13:09.716534 rfcxtf-0.0.5/
+-rw-r--r--   0 root         (0) root         (0)      482 2023-07-14 11:13:09.715026 rfcxtf-0.0.5/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:13:09.666554 rfcxtf-0.0.5/rfcxtf/
+-rw-r--r--   0 root         (0) root         (0)      593 2023-05-04 09:58:45.000000 rfcxtf-0.0.5/rfcxtf/ClassifierBase.py
+-rw-r--r--   0 root         (0) root         (0)     2602 2023-05-04 10:33:29.000000 rfcxtf-0.0.5/rfcxtf/ClassifierTF2.py
+-rw-r--r--   0 root         (0) root         (0)       58 2023-05-04 10:26:02.000000 rfcxtf-0.0.5/rfcxtf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:13:09.710232 rfcxtf-0.0.5/rfcxtf/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 11:11:18.000000 rfcxtf-0.0.5/rfcxtf/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       48 2023-05-04 09:05:14.000000 rfcxtf-0.0.5/rfcxtf/utils/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      272 2023-05-04 09:05:14.000000 rfcxtf-0.0.5/rfcxtf/utils/io.py
+-rw-r--r--   0 root         (0) root         (0)      321 2023-05-04 09:05:14.000000 rfcxtf-0.0.5/rfcxtf/utils/postprocessor.py
+-rw-r--r--   0 root         (0) root         (0)     3501 2023-07-13 21:45:45.000000 rfcxtf-0.0.5/rfcxtf/validate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:13:09.689797 rfcxtf-0.0.5/rfcxtf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      482 2023-07-14 11:13:09.000000 rfcxtf-0.0.5/rfcxtf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      345 2023-07-14 11:13:09.000000 rfcxtf-0.0.5/rfcxtf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 11:13:09.000000 rfcxtf-0.0.5/rfcxtf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-14 11:13:09.000000 rfcxtf-0.0.5/rfcxtf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-14 11:13:09.000000 rfcxtf-0.0.5/rfcxtf.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 11:13:09.717250 rfcxtf-0.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      778 2023-07-14 11:12:45.000000 rfcxtf-0.0.5/setup.py
```

### Comparing `rfcxtf-0.0.4/rfcxtf/ClassifierBase.py` & `rfcxtf-0.0.5/rfcxtf/ClassifierBase.py`

 * *Files identical despite different names*

### Comparing `rfcxtf-0.0.4/rfcxtf/ClassifierTF2.py` & `rfcxtf-0.0.5/rfcxtf/ClassifierTF2.py`

 * *Files identical despite different names*

### Comparing `rfcxtf-0.0.4/rfcxtf/validate.py` & `rfcxtf-0.0.5/rfcxtf/validate.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import numpy as np
 import tarfile
 import tempfile
 import tensorflow as tf
 from typing import Optional
 from .utils.io import read_wav
 
-def validate(saved_model_package_path: str) -> Optional[str]:
+def validate(saved_model_package_path: str, audio_file_path: str) -> Optional[str]:
     # Must have tar.gz extension
     if not saved_model_package_path.endswith('.tar.gz'):
         return 'Package must be a .tar.gz file'
     
     # Must be able to extract tar.gz
     temp_folder = tempfile.mkdtemp()
     try:
@@ -62,15 +62,15 @@
         return 'Signature `score` must have 1 output as a 3-element tuple'
     (expected_classes,) = metadata['class_names'].get_shape()
     (_, _, actual_classes) = score_fn.outputs[0].get_shape()
     if expected_classes != actual_classes:
         return 'Length of `class_names` in `metadata` must match size of `score` output'
 
     # Can score an input
-    data, _ = read_wav('example/guardian_audio.wav')
+    data, _ = read_wav(audio_file_path)
     waveform_values = np.array(data, dtype=np.float32).reshape((1, len(data), 1)) 
     try:
         _ = next(iter(score_fn(
             waveform=tf.constant(waveform_values),
             context_step_samples=tf.constant(int(metadata['input_sample_rate']), tf.int64),
         ).values())).numpy()
     except Exception as e:
```

### Comparing `rfcxtf-0.0.4/setup.py` & `rfcxtf-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 REQUIRED_PACKAGES = ['tensorflow', 'pysndfile', 'numpy']
 
 setup(name='rfcxtf',
-      version='0.0.4',
+      version='0.0.5',
       url='https://github.com/rfcx/rfcx-sdk-python',
       license='None',
       author='Rainforest Connection',
       author_email='antony@rfcx.org',
       install_requires=REQUIRED_PACKAGES,
       description='Support for building TensorFlow classifiers on Arbimon and Guardian platforms',
       packages=find_packages(exclude=['tests']),
```

