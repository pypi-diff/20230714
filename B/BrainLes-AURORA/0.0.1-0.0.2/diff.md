# Comparing `tmp/BrainLes_AURORA-0.0.1.tar.gz` & `tmp/BrainLes_AURORA-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BrainLes_AURORA-0.0.1.tar", last modified: Tue Jul 11 15:00:38 2023, max compression
+gzip compressed data, was "BrainLes_AURORA-0.0.2.tar", last modified: Fri Jul 14 18:51:24 2023, max compression
```

## Comparing `BrainLes_AURORA-0.0.1.tar` & `BrainLes_AURORA-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 florian   (1001) florian   (1001)        0 2023-07-11 15:00:38.066943 BrainLes_AURORA-0.0.1/
-drwxrwxr-x   0 florian   (1001) florian   (1001)        0 2023-07-11 15:00:38.062943 BrainLes_AURORA-0.0.1/BrainLes_AURORA.egg-info/
--rw-rw-r--   0 florian   (1001) florian   (1001)     8222 2023-07-11 15:00:38.000000 BrainLes_AURORA-0.0.1/BrainLes_AURORA.egg-info/PKG-INFO
--rw-rw-r--   0 florian   (1001) florian   (1001)      370 2023-07-11 15:00:38.000000 BrainLes_AURORA-0.0.1/BrainLes_AURORA.egg-info/SOURCES.txt
--rw-rw-r--   0 florian   (1001) florian   (1001)        1 2023-07-11 15:00:38.000000 BrainLes_AURORA-0.0.1/BrainLes_AURORA.egg-info/dependency_links.txt
--rw-rw-r--   0 florian   (1001) florian   (1001)      103 2023-07-11 15:00:38.000000 BrainLes_AURORA-0.0.1/BrainLes_AURORA.egg-info/requires.txt
--rw-rw-r--   0 florian   (1001) florian   (1001)       16 2023-07-11 15:00:38.000000 BrainLes_AURORA-0.0.1/BrainLes_AURORA.egg-info/top_level.txt
--rw-rw-r--   0 florian   (1001) florian   (1001)    34523 2023-07-11 13:37:21.000000 BrainLes_AURORA-0.0.1/LICENSE
--rw-rw-r--   0 florian   (1001) florian   (1001)     8222 2023-07-11 15:00:38.066943 BrainLes_AURORA-0.0.1/PKG-INFO
--rw-rw-r--   0 florian   (1001) florian   (1001)     7586 2023-07-11 13:37:21.000000 BrainLes_AURORA-0.0.1/README.md
-drwxrwxr-x   0 florian   (1001) florian   (1001)        0 2023-07-11 15:00:38.066943 BrainLes_AURORA-0.0.1/brainles_aurora/
--rw-rw-r--   0 florian   (1001) florian   (1001)    17453 2023-07-11 14:54:39.000000 BrainLes_AURORA-0.0.1/brainles_aurora/lib.py
--rw-rw-r--   0 florian   (1001) florian   (1001)     6352 2023-07-11 13:37:23.000000 BrainLes_AURORA-0.0.1/brainles_aurora/modlib.py
--rw-rw-r--   0 florian   (1001) florian   (1001)     1201 2023-07-11 13:37:23.000000 BrainLes_AURORA-0.0.1/brainles_aurora/run_inference.py
--rw-rw-r--   0 florian   (1001) florian   (1001)     2924 2023-07-11 13:37:23.000000 BrainLes_AURORA-0.0.1/brainles_aurora/run_inference_cli.py
--rw-rw-r--   0 florian   (1001) florian   (1001)     1483 2023-07-11 14:56:35.000000 BrainLes_AURORA-0.0.1/brainles_aurora/utils.py
--rw-rw-r--   0 florian   (1001) florian   (1001)     1219 2023-07-11 14:36:54.000000 BrainLes_AURORA-0.0.1/pyproject.toml
--rw-rw-r--   0 florian   (1001) florian   (1001)       38 2023-07-11 15:00:38.066943 BrainLes_AURORA-0.0.1/setup.cfg
+drwxrwxr-x   0 florian   (1001) florian   (1001)        0 2023-07-14 18:51:24.258277 BrainLes_AURORA-0.0.2/
+drwxrwxr-x   0 florian   (1001) florian   (1001)        0 2023-07-14 18:51:24.258277 BrainLes_AURORA-0.0.2/BrainLes_AURORA.egg-info/
+-rw-rw-r--   0 florian   (1001) florian   (1001)     8222 2023-07-14 18:51:24.000000 BrainLes_AURORA-0.0.2/BrainLes_AURORA.egg-info/PKG-INFO
+-rw-rw-r--   0 florian   (1001) florian   (1001)      370 2023-07-14 18:51:24.000000 BrainLes_AURORA-0.0.2/BrainLes_AURORA.egg-info/SOURCES.txt
+-rw-rw-r--   0 florian   (1001) florian   (1001)        1 2023-07-14 18:51:24.000000 BrainLes_AURORA-0.0.2/BrainLes_AURORA.egg-info/dependency_links.txt
+-rw-rw-r--   0 florian   (1001) florian   (1001)      103 2023-07-14 18:51:24.000000 BrainLes_AURORA-0.0.2/BrainLes_AURORA.egg-info/requires.txt
+-rw-rw-r--   0 florian   (1001) florian   (1001)       16 2023-07-14 18:51:24.000000 BrainLes_AURORA-0.0.2/BrainLes_AURORA.egg-info/top_level.txt
+-rw-rw-r--   0 florian   (1001) florian   (1001)    34523 2023-07-11 13:37:21.000000 BrainLes_AURORA-0.0.2/LICENSE
+-rw-rw-r--   0 florian   (1001) florian   (1001)     8222 2023-07-14 18:51:24.258277 BrainLes_AURORA-0.0.2/PKG-INFO
+-rw-rw-r--   0 florian   (1001) florian   (1001)     7586 2023-07-11 13:37:21.000000 BrainLes_AURORA-0.0.2/README.md
+drwxrwxr-x   0 florian   (1001) florian   (1001)        0 2023-07-14 18:51:24.258277 BrainLes_AURORA-0.0.2/brainles_aurora/
+-rw-rw-r--   0 florian   (1001) florian   (1001)      216 2023-07-12 14:42:43.000000 BrainLes_AURORA-0.0.2/brainles_aurora/aux.py
+-rw-rw-r--   0 florian   (1001) florian   (1001)     1483 2023-07-12 14:05:44.000000 BrainLes_AURORA-0.0.2/brainles_aurora/download.py
+-rw-rw-r--   0 florian   (1001) florian   (1001)    17445 2023-07-12 14:42:57.000000 BrainLes_AURORA-0.0.2/brainles_aurora/lib.py
+-rw-rw-r--   0 florian   (1001) florian   (1001)     1201 2023-07-11 15:21:02.000000 BrainLes_AURORA-0.0.2/brainles_aurora/run_inference.py
+-rw-rw-r--   0 florian   (1001) florian   (1001)     2924 2023-07-11 15:21:02.000000 BrainLes_AURORA-0.0.2/brainles_aurora/run_inference_cli.py
+-rw-rw-r--   0 florian   (1001) florian   (1001)     1219 2023-07-14 18:46:45.000000 BrainLes_AURORA-0.0.2/pyproject.toml
+-rw-rw-r--   0 florian   (1001) florian   (1001)       38 2023-07-14 18:51:24.258277 BrainLes_AURORA-0.0.2/setup.cfg
```

### Comparing `BrainLes_AURORA-0.0.1/BrainLes_AURORA.egg-info/PKG-INFO` & `BrainLes_AURORA-0.0.2/BrainLes_AURORA.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BrainLes-AURORA
-Version: 0.0.1
+Version: 0.0.2
 Summary: TODO.
 Author-email: Florian Kofler <florian.kofler@tum.de>, Isra Mekki <isra.mekki@helmholtz-muenchen.de>
 Maintainer-email: Florian Kofler <florian.kofler@tum.de>, Isra Mekki <isra.mekki@helmholtz-muenchen.de>
 Project-URL: repository, https://github.com/neuronflow/BrainLes
 Keywords: Brain metastasis segmentation
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `BrainLes_AURORA-0.0.1/LICENSE` & `BrainLes_AURORA-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `BrainLes_AURORA-0.0.1/PKG-INFO` & `BrainLes_AURORA-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BrainLes_AURORA
-Version: 0.0.1
+Version: 0.0.2
 Summary: TODO.
 Author-email: Florian Kofler <florian.kofler@tum.de>, Isra Mekki <isra.mekki@helmholtz-muenchen.de>
 Maintainer-email: Florian Kofler <florian.kofler@tum.de>, Isra Mekki <isra.mekki@helmholtz-muenchen.de>
 Project-URL: repository, https://github.com/neuronflow/BrainLes
 Keywords: Brain metastasis segmentation
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `BrainLes_AURORA-0.0.1/README.md` & `BrainLes_AURORA-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `BrainLes_AURORA-0.0.1/brainles_aurora/lib.py` & `BrainLes_AURORA-0.0.2/brainles_aurora/lib.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,33 +23,24 @@
     LoadImageD,
     Lambdad,
     ToTensord,
     ScaleIntensityRangePercentilesd,
     EnsureChannelFirstd,
 )
 
-from brainles_aurora.utils import download_model_weights
+from AURORA.brainles_aurora.download import download_model_weights
+from AURORA.brainles_aurora.aux import turbo_path
 
 lib_abspath = os.path.dirname(os.path.abspath(__file__))
 
 model_weights_dir = lib_abspath + "/model_weights"
 if not os.path.exists(model_weights_dir):
     download_model_weights(target_folder=lib_abspath)
     
 
-def _turbo_path(the_path):
-    turbo_path = Path(
-        os.path.normpath(
-            os.path.abspath(
-                the_path,
-            )
-        )
-    )
-    return turbo_path
-
 
 def _create_nifti_seg(
     threshold,
     reference_file,
     onehot_model_outputs_CHWD,
     output_file,
     whole_network_output_file,
@@ -290,17 +281,19 @@
             in_channels=4,
             out_channels=2,
             features=(32, 32, 64, 128, 256, 32),
             dropout=0.1,
             act="mish",
         )
         if model_selection == "best":
-            weights = _turbo_path(lib_abspath + "/model_weights/t1-t1c-t1-fla/t1-t1c-t1-fla_best.tar")
+            weights = turbo_path(lib_abspath + "/model_weights/t1-t1c-t2-fla/t1-t1c-t2-fla_best.tar")
         elif model_selection == "last":
-            weights = _turbo_path(lib_abspath + "/model_weights/t1-t1c-t1-fla/t1-t1c-t1-fla_last.tar")
+            weights = turbo_path(lib_abspath + "/model_weights/t1-t1c-t2-fla/t1-t1c-t2-fla_last.tar")
+        elif model_selection == "vanilla":
+            weights = turbo_path(lib_abspath + "/model_weights/t1-t1c-t2-fla/vanilla.tar")
         else:
             raise NotImplementedError(
                 "no checkpoint implemented for this selection strategy."
             )
 
     elif mode == "t1c-t1-fla":
         model = BasicUNet(
@@ -309,17 +302,17 @@
             out_channels=2,
             features=(32, 32, 64, 128, 256, 32),
             dropout=0.1,
             act="mish",
         )
 
         if model_selection == "best":
-            weights = _turbo_path(lib_abspath + "/model_weights/t1c-t1-fla/t1c-t1-fla_best.tar")
+            weights = turbo_path(lib_abspath + "/model_weights/t1c-t1-fla/t1c-t1-fla_best.tar")
         elif model_selection == "last":
-            weights = _turbo_path(lib_abspath + "/model_weights/t1c-t1-fla/t1c-t1-fla_last.tar")
+            weights = turbo_path(lib_abspath + "/model_weights/t1c-t1-fla/t1c-t1-fla_last.tar")
         else:
             raise NotImplementedError(
                 "no checkpoint implemented for this selection strategy."
             )
 
     elif mode == "t1c-t1":
         model = BasicUNet(
@@ -328,17 +321,17 @@
             out_channels=2,
             features=(32, 32, 64, 128, 256, 32),
             dropout=0.1,
             act="mish",
         )
 
         if model_selection == "best":
-            weights = _turbo_path(lib_abspath + "/model_weights/t1c-t1/t1c-t1_best.tar")
+            weights = turbo_path(lib_abspath + "/model_weights/t1c-t1/t1c-t1_best.tar")
         elif model_selection == "last":
-            weights = _turbo_path(lib_abspath + "/model_weights/t1c-t1/t1c-t1_last.tar")
+            weights = turbo_path(lib_abspath + "/model_weights/t1c-t1/t1c-t1_last.tar")
         else:
             raise NotImplementedError(
                 "no checkpoint implemented for this selection strategy."
             )
 
     elif mode == "t1c-fla":
         model = BasicUNet(
@@ -347,17 +340,17 @@
             out_channels=2,
             features=(32, 32, 64, 128, 256, 32),
             dropout=0.1,
             act="mish",
         )
 
         if model_selection == "best":
-            weights = _turbo_path(lib_abspath + "/model_weights/t1c-fla/t1c-fla_best.tar")
+            weights = turbo_path(lib_abspath + "/model_weights/t1c-fla/t1c-fla_best.tar")
         elif model_selection == "last":
-            weights = _turbo_path(lib_abspath + "/model_weights/t1c-fla/t1c-fla_last.tar")
+            weights = turbo_path(lib_abspath + "/model_weights/t1c-fla/t1c-fla_last.tar")
         else:
             raise NotImplementedError(
                 "no checkpoint implemented for this selection strategy."
             )
 
     elif mode == "t1c-o":
         model = BasicUNet(
@@ -366,17 +359,17 @@
             out_channels=2,
             features=(32, 32, 64, 128, 256, 32),
             dropout=0.1,
             act="mish",
         )
 
         if model_selection == "best":
-            weights = _turbo_path(lib_abspath + "/model_weights/t1c-o/t1c-o_best.tar")
+            weights = turbo_path(lib_abspath + "/model_weights/t1c-o/t1c-o_best.tar")
         elif model_selection == "last":
-            weights = _turbo_path(lib_abspath + "/model_weights/t1c-o/t1c-o_last.tar")
+            weights = turbo_path(lib_abspath + "/model_weights/t1c-o/t1c-o_last.tar")
         else:
             raise NotImplementedError(
                 "no checkpoint implemented for this selection strategy."
             )
 
     elif mode == "t1-o":
         model = BasicUNet(
@@ -385,17 +378,17 @@
             out_channels=2,
             features=(32, 32, 64, 128, 256, 32),
             dropout=0.1,
             act="mish",
         )
 
         if model_selection == "best":
-            weights = _turbo_path(lib_abspath + "/model_weights/t1-o/t1-o_best.tar")
+            weights = turbo_path(lib_abspath + "/model_weights/t1-o/t1-o_best.tar")
         elif model_selection == "last":
-            weights = _turbo_path(lib_abspath + "/model_weights/t1-o/t1-o_last.tar")
+            weights = turbo_path(lib_abspath + "/model_weights/t1-o/t1-o_last.tar")
         else:
             raise NotImplementedError(
                 "no checkpoint implemented for this selection strategy."
             )
 
     elif mode == "fla-o":
         model = BasicUNet(
@@ -404,17 +397,17 @@
             out_channels=2,
             features=(32, 32, 64, 128, 256, 32),
             dropout=0.1,
             act="mish",
         )
 
         if model_selection == "best":
-            weights = _turbo_path(lib_abspath + "/model_weights/fla-o/fla-o_best.tar")
+            weights = turbo_path(lib_abspath + "/model_weights/fla-o/fla-o_best.tar")
         elif model_selection == "last":
-            weights = _turbo_path(lib_abspath + "/model_weights/fla-o/fla-o_last.tar")
+            weights = turbo_path(lib_abspath + "/model_weights/fla-o/fla-o_last.tar")
         else:
             raise NotImplementedError(
                 "no checkpoint implemented for this selection strategy."
             )
     else:
         raise NotImplementedError("no model implemented for this combination of files")
 
@@ -455,24 +448,24 @@
     sw_batch_size: batch size for the sliding window inference
     overlap: overlap used in the sliding window inference
 
     see the above function definition for meaningful defaults.
     """
     # ~~<< I N P U T S >>~~
     if t1_file is not None:
-        t1_file = _turbo_path(t1_file)
+        t1_file = turbo_path(t1_file)
 
     if t1c_file is not None:
-        t1c_file = _turbo_path(t1c_file)
+        t1c_file = turbo_path(t1c_file)
 
     if t2_file is not None:
-        t2_file = _turbo_path(t2_file)
+        t2_file = turbo_path(t2_file)
 
     if fla_file is not None:
-        fla_file = _turbo_path(fla_file)
+        fla_file = turbo_path(fla_file)
 
     # ~~<< M O D E >>~~
     mode = _get_mode(
         t1_file=t1_file,
         t1c_file=t1c_file,
         t2_file=t2_file,
         fla_file=fla_file,
```

### Comparing `BrainLes_AURORA-0.0.1/brainles_aurora/run_inference.py` & `BrainLes_AURORA-0.0.2/brainles_aurora/run_inference.py`

 * *Files identical despite different names*

### Comparing `BrainLes_AURORA-0.0.1/brainles_aurora/run_inference_cli.py` & `BrainLes_AURORA-0.0.2/brainles_aurora/run_inference_cli.py`

 * *Files identical despite different names*

### Comparing `BrainLes_AURORA-0.0.1/brainles_aurora/utils.py` & `BrainLes_AURORA-0.0.2/brainles_aurora/download.py`

 * *Files identical despite different names*

### Comparing `BrainLes_AURORA-0.0.1/pyproject.toml` & `BrainLes_AURORA-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 [tool.setuptools_scm]
 write_to = "brainles_aurora/_version.py"
 
 [project]
 name = "BrainLes_AURORA"
 # dynamic = ["version"]
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   {name="Florian Kofler", email="florian.kofler@tum.de"},
   {name="Isra Mekki", email="isra.mekki@helmholtz-muenchen.de"},
 ]
 maintainers = [
   {name="Florian Kofler", email="florian.kofler@tum.de"},
   {name="Isra Mekki", email="isra.mekki@helmholtz-muenchen.de"},
```

