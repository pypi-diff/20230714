# Comparing `tmp/BrainLes_AURORA-0.0.2.tar.gz` & `tmp/BrainLes_AURORA-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BrainLes_AURORA-0.0.2.tar", last modified: Fri Jul 14 18:51:24 2023, max compression
+gzip compressed data, was "BrainLes_AURORA-0.0.3.tar", last modified: Fri Jul 14 19:03:30 2023, max compression
```

## Comparing `BrainLes_AURORA-0.0.2.tar` & `BrainLes_AURORA-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 florian   (1001) florian   (1001)        0 2023-07-14 18:51:24.258277 BrainLes_AURORA-0.0.2/
-drwxrwxr-x   0 florian   (1001) florian   (1001)        0 2023-07-14 18:51:24.258277 BrainLes_AURORA-0.0.2/BrainLes_AURORA.egg-info/
--rw-rw-r--   0 florian   (1001) florian   (1001)     8222 2023-07-14 18:51:24.000000 BrainLes_AURORA-0.0.2/BrainLes_AURORA.egg-info/PKG-INFO
--rw-rw-r--   0 florian   (1001) florian   (1001)      370 2023-07-14 18:51:24.000000 BrainLes_AURORA-0.0.2/BrainLes_AURORA.egg-info/SOURCES.txt
--rw-rw-r--   0 florian   (1001) florian   (1001)        1 2023-07-14 18:51:24.000000 BrainLes_AURORA-0.0.2/BrainLes_AURORA.egg-info/dependency_links.txt
--rw-rw-r--   0 florian   (1001) florian   (1001)      103 2023-07-14 18:51:24.000000 BrainLes_AURORA-0.0.2/BrainLes_AURORA.egg-info/requires.txt
--rw-rw-r--   0 florian   (1001) florian   (1001)       16 2023-07-14 18:51:24.000000 BrainLes_AURORA-0.0.2/BrainLes_AURORA.egg-info/top_level.txt
--rw-rw-r--   0 florian   (1001) florian   (1001)    34523 2023-07-11 13:37:21.000000 BrainLes_AURORA-0.0.2/LICENSE
--rw-rw-r--   0 florian   (1001) florian   (1001)     8222 2023-07-14 18:51:24.258277 BrainLes_AURORA-0.0.2/PKG-INFO
--rw-rw-r--   0 florian   (1001) florian   (1001)     7586 2023-07-11 13:37:21.000000 BrainLes_AURORA-0.0.2/README.md
-drwxrwxr-x   0 florian   (1001) florian   (1001)        0 2023-07-14 18:51:24.258277 BrainLes_AURORA-0.0.2/brainles_aurora/
--rw-rw-r--   0 florian   (1001) florian   (1001)      216 2023-07-12 14:42:43.000000 BrainLes_AURORA-0.0.2/brainles_aurora/aux.py
--rw-rw-r--   0 florian   (1001) florian   (1001)     1483 2023-07-12 14:05:44.000000 BrainLes_AURORA-0.0.2/brainles_aurora/download.py
--rw-rw-r--   0 florian   (1001) florian   (1001)    17445 2023-07-12 14:42:57.000000 BrainLes_AURORA-0.0.2/brainles_aurora/lib.py
--rw-rw-r--   0 florian   (1001) florian   (1001)     1201 2023-07-11 15:21:02.000000 BrainLes_AURORA-0.0.2/brainles_aurora/run_inference.py
--rw-rw-r--   0 florian   (1001) florian   (1001)     2924 2023-07-11 15:21:02.000000 BrainLes_AURORA-0.0.2/brainles_aurora/run_inference_cli.py
--rw-rw-r--   0 florian   (1001) florian   (1001)     1219 2023-07-14 18:46:45.000000 BrainLes_AURORA-0.0.2/pyproject.toml
--rw-rw-r--   0 florian   (1001) florian   (1001)       38 2023-07-14 18:51:24.258277 BrainLes_AURORA-0.0.2/setup.cfg
+drwxrwxr-x   0 florian   (1001) florian   (1001)        0 2023-07-14 19:03:30.046508 BrainLes_AURORA-0.0.3/
+drwxrwxr-x   0 florian   (1001) florian   (1001)        0 2023-07-14 19:03:30.042508 BrainLes_AURORA-0.0.3/BrainLes_AURORA.egg-info/
+-rw-rw-r--   0 florian   (1001) florian   (1001)     8222 2023-07-14 19:03:30.000000 BrainLes_AURORA-0.0.3/BrainLes_AURORA.egg-info/PKG-INFO
+-rw-rw-r--   0 florian   (1001) florian   (1001)      370 2023-07-14 19:03:30.000000 BrainLes_AURORA-0.0.3/BrainLes_AURORA.egg-info/SOURCES.txt
+-rw-rw-r--   0 florian   (1001) florian   (1001)        1 2023-07-14 19:03:30.000000 BrainLes_AURORA-0.0.3/BrainLes_AURORA.egg-info/dependency_links.txt
+-rw-rw-r--   0 florian   (1001) florian   (1001)      103 2023-07-14 19:03:30.000000 BrainLes_AURORA-0.0.3/BrainLes_AURORA.egg-info/requires.txt
+-rw-rw-r--   0 florian   (1001) florian   (1001)       16 2023-07-14 19:03:30.000000 BrainLes_AURORA-0.0.3/BrainLes_AURORA.egg-info/top_level.txt
+-rw-rw-r--   0 florian   (1001) florian   (1001)    34523 2023-07-11 13:37:21.000000 BrainLes_AURORA-0.0.3/LICENSE
+-rw-rw-r--   0 florian   (1001) florian   (1001)     8222 2023-07-14 19:03:30.046508 BrainLes_AURORA-0.0.3/PKG-INFO
+-rw-rw-r--   0 florian   (1001) florian   (1001)     7586 2023-07-11 13:37:21.000000 BrainLes_AURORA-0.0.3/README.md
+drwxrwxr-x   0 florian   (1001) florian   (1001)        0 2023-07-14 19:03:30.046508 BrainLes_AURORA-0.0.3/brainles_aurora/
+-rw-rw-r--   0 florian   (1001) florian   (1001)      216 2023-07-12 14:42:43.000000 BrainLes_AURORA-0.0.3/brainles_aurora/aux.py
+-rw-rw-r--   0 florian   (1001) florian   (1001)     1483 2023-07-12 14:05:44.000000 BrainLes_AURORA-0.0.3/brainles_aurora/download.py
+-rw-rw-r--   0 florian   (1001) florian   (1001)    17431 2023-07-14 19:02:21.000000 BrainLes_AURORA-0.0.3/brainles_aurora/lib.py
+-rw-rw-r--   0 florian   (1001) florian   (1001)     1201 2023-07-11 15:21:02.000000 BrainLes_AURORA-0.0.3/brainles_aurora/run_inference.py
+-rw-rw-r--   0 florian   (1001) florian   (1001)     2924 2023-07-11 15:21:02.000000 BrainLes_AURORA-0.0.3/brainles_aurora/run_inference_cli.py
+-rw-rw-r--   0 florian   (1001) florian   (1001)     1219 2023-07-14 19:02:51.000000 BrainLes_AURORA-0.0.3/pyproject.toml
+-rw-rw-r--   0 florian   (1001) florian   (1001)       38 2023-07-14 19:03:30.046508 BrainLes_AURORA-0.0.3/setup.cfg
```

### Comparing `BrainLes_AURORA-0.0.2/BrainLes_AURORA.egg-info/PKG-INFO` & `BrainLes_AURORA-0.0.3/BrainLes_AURORA.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BrainLes-AURORA
-Version: 0.0.2
+Version: 0.0.3
 Summary: TODO.
 Author-email: Florian Kofler <florian.kofler@tum.de>, Isra Mekki <isra.mekki@helmholtz-muenchen.de>
 Maintainer-email: Florian Kofler <florian.kofler@tum.de>, Isra Mekki <isra.mekki@helmholtz-muenchen.de>
 Project-URL: repository, https://github.com/neuronflow/BrainLes
 Keywords: Brain metastasis segmentation
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `BrainLes_AURORA-0.0.2/LICENSE` & `BrainLes_AURORA-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `BrainLes_AURORA-0.0.2/PKG-INFO` & `BrainLes_AURORA-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BrainLes_AURORA
-Version: 0.0.2
+Version: 0.0.3
 Summary: TODO.
 Author-email: Florian Kofler <florian.kofler@tum.de>, Isra Mekki <isra.mekki@helmholtz-muenchen.de>
 Maintainer-email: Florian Kofler <florian.kofler@tum.de>, Isra Mekki <isra.mekki@helmholtz-muenchen.de>
 Project-URL: repository, https://github.com/neuronflow/BrainLes
 Keywords: Brain metastasis segmentation
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `BrainLes_AURORA-0.0.2/README.md` & `BrainLes_AURORA-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `BrainLes_AURORA-0.0.2/brainles_aurora/download.py` & `BrainLes_AURORA-0.0.3/brainles_aurora/download.py`

 * *Files identical despite different names*

### Comparing `BrainLes_AURORA-0.0.2/brainles_aurora/lib.py` & `BrainLes_AURORA-0.0.3/brainles_aurora/lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     LoadImageD,
     Lambdad,
     ToTensord,
     ScaleIntensityRangePercentilesd,
     EnsureChannelFirstd,
 )
 
-from AURORA.brainles_aurora.download import download_model_weights
-from AURORA.brainles_aurora.aux import turbo_path
+from brainles_aurora.download import download_model_weights
+from brainles_aurora.aux import turbo_path
 
 lib_abspath = os.path.dirname(os.path.abspath(__file__))
 
 model_weights_dir = lib_abspath + "/model_weights"
 if not os.path.exists(model_weights_dir):
     download_model_weights(target_folder=lib_abspath)
```

### Comparing `BrainLes_AURORA-0.0.2/brainles_aurora/run_inference.py` & `BrainLes_AURORA-0.0.3/brainles_aurora/run_inference.py`

 * *Files identical despite different names*

### Comparing `BrainLes_AURORA-0.0.2/brainles_aurora/run_inference_cli.py` & `BrainLes_AURORA-0.0.3/brainles_aurora/run_inference_cli.py`

 * *Files identical despite different names*

### Comparing `BrainLes_AURORA-0.0.2/pyproject.toml` & `BrainLes_AURORA-0.0.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 [tool.setuptools_scm]
 write_to = "brainles_aurora/_version.py"
 
 [project]
 name = "BrainLes_AURORA"
 # dynamic = ["version"]
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   {name="Florian Kofler", email="florian.kofler@tum.de"},
   {name="Isra Mekki", email="isra.mekki@helmholtz-muenchen.de"},
 ]
 maintainers = [
   {name="Florian Kofler", email="florian.kofler@tum.de"},
   {name="Isra Mekki", email="isra.mekki@helmholtz-muenchen.de"},
```

