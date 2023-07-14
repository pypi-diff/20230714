# Comparing `tmp/fastMONAI-0.3.2.tar.gz` & `tmp/fastMONAI-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastMONAI-0.3.2.tar", last modified: Thu Jul 13 09:17:04 2023, max compression
+gzip compressed data, was "fastMONAI-0.3.3.tar", last modified: Fri Jul 14 13:46:06 2023, max compression
```

## Comparing `fastMONAI-0.3.2.tar` & `fastMONAI-0.3.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 sathiesh  (1001) sathiesh  (1001)        0 2023-07-13 09:17:04.690129 fastMONAI-0.3.2/
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     1101 2023-07-12 10:04:27.000000 fastMONAI-0.3.2/CONTRIBUTING.md
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)    11337 2022-08-29 15:09:22.000000 fastMONAI-0.3.2/LICENSE
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      111 2022-08-29 15:09:22.000000 fastMONAI-0.3.2/MANIFEST.in
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     5428 2023-07-13 09:17:04.690129 fastMONAI-0.3.2/PKG-INFO
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     4664 2023-03-31 13:03:15.000000 fastMONAI-0.3.2/README.md
-drwxrwxr-x   0 sathiesh  (1001) sathiesh  (1001)        0 2023-07-13 09:17:04.690129 fastMONAI-0.3.2/fastMONAI/
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)       22 2023-07-13 09:11:37.000000 fastMONAI-0.3.2/fastMONAI/__init__.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)    27510 2023-07-13 09:11:37.000000 fastMONAI-0.3.2/fastMONAI/_modidx.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     4948 2023-07-13 09:11:36.000000 fastMONAI-0.3.2/fastMONAI/dataset_info.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)    10970 2023-07-13 09:11:36.000000 fastMONAI-0.3.2/fastMONAI/external_data.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      590 2022-12-13 11:40:31.000000 fastMONAI-0.3.2/fastMONAI/research_utils.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     1406 2023-07-13 09:11:36.000000 fastMONAI-0.3.2/fastMONAI/utils.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      360 2022-12-13 12:10:38.000000 fastMONAI-0.3.2/fastMONAI/vision_all.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     9070 2023-07-13 09:11:36.000000 fastMONAI-0.3.2/fastMONAI/vision_augmentation.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     7428 2023-07-13 09:11:36.000000 fastMONAI-0.3.2/fastMONAI/vision_core.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)    10530 2023-07-13 09:11:36.000000 fastMONAI-0.3.2/fastMONAI/vision_data.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     3699 2023-07-13 09:11:36.000000 fastMONAI-0.3.2/fastMONAI/vision_inference.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     3591 2023-07-13 09:11:36.000000 fastMONAI-0.3.2/fastMONAI/vision_loss.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     3549 2023-07-13 09:11:36.000000 fastMONAI-0.3.2/fastMONAI/vision_metrics.py
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     3095 2023-07-13 09:11:36.000000 fastMONAI-0.3.2/fastMONAI/vision_plot.py
-drwxrwxr-x   0 sathiesh  (1001) sathiesh  (1001)        0 2023-07-13 09:17:04.690129 fastMONAI-0.3.2/fastMONAI.egg-info/
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     5428 2023-07-13 09:17:04.000000 fastMONAI-0.3.2/fastMONAI.egg-info/PKG-INFO
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      657 2023-07-13 09:17:04.000000 fastMONAI-0.3.2/fastMONAI.egg-info/SOURCES.txt
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)        1 2023-07-13 09:17:04.000000 fastMONAI-0.3.2/fastMONAI.egg-info/dependency_links.txt
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)       40 2023-07-13 09:17:04.000000 fastMONAI-0.3.2/fastMONAI.egg-info/entry_points.txt
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)        1 2022-08-29 15:24:47.000000 fastMONAI-0.3.2/fastMONAI.egg-info/not-zip-safe
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      133 2023-07-13 09:17:04.000000 fastMONAI-0.3.2/fastMONAI.egg-info/requires.txt
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)       10 2023-07-13 09:17:04.000000 fastMONAI-0.3.2/fastMONAI.egg-info/top_level.txt
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     1218 2023-07-12 08:55:41.000000 fastMONAI-0.3.2/settings.ini
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)       38 2023-07-13 09:17:04.690129 fastMONAI-0.3.2/setup.cfg
--rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     2541 2022-08-29 15:09:22.000000 fastMONAI-0.3.2/setup.py
+drwxrwxr-x   0 sathiesh  (1001) sathiesh  (1001)        0 2023-07-14 13:46:06.873309 fastMONAI-0.3.3/
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     1101 2023-07-12 10:04:27.000000 fastMONAI-0.3.3/CONTRIBUTING.md
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)    11337 2022-08-29 15:09:22.000000 fastMONAI-0.3.3/LICENSE
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      111 2022-08-29 15:09:22.000000 fastMONAI-0.3.3/MANIFEST.in
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     5428 2023-07-14 13:46:06.873309 fastMONAI-0.3.3/PKG-INFO
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     4664 2023-03-31 13:03:15.000000 fastMONAI-0.3.3/README.md
+drwxrwxr-x   0 sathiesh  (1001) sathiesh  (1001)        0 2023-07-14 13:46:06.873309 fastMONAI-0.3.3/fastMONAI/
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)       22 2023-07-14 13:40:49.000000 fastMONAI-0.3.3/fastMONAI/__init__.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)    27510 2023-07-14 13:40:49.000000 fastMONAI-0.3.3/fastMONAI/_modidx.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     4948 2023-07-14 13:40:49.000000 fastMONAI-0.3.3/fastMONAI/dataset_info.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)    11016 2023-07-14 13:40:49.000000 fastMONAI-0.3.3/fastMONAI/external_data.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      590 2022-12-13 11:40:31.000000 fastMONAI-0.3.3/fastMONAI/research_utils.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     1406 2023-07-14 13:40:49.000000 fastMONAI-0.3.3/fastMONAI/utils.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      360 2022-12-13 12:10:38.000000 fastMONAI-0.3.3/fastMONAI/vision_all.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     9070 2023-07-14 13:40:49.000000 fastMONAI-0.3.3/fastMONAI/vision_augmentation.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     7428 2023-07-14 13:40:49.000000 fastMONAI-0.3.3/fastMONAI/vision_core.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)    10491 2023-07-14 13:40:49.000000 fastMONAI-0.3.3/fastMONAI/vision_data.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     3744 2023-07-14 13:40:49.000000 fastMONAI-0.3.3/fastMONAI/vision_inference.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     3591 2023-07-14 13:40:49.000000 fastMONAI-0.3.3/fastMONAI/vision_loss.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     3549 2023-07-14 13:40:49.000000 fastMONAI-0.3.3/fastMONAI/vision_metrics.py
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     3095 2023-07-14 13:40:49.000000 fastMONAI-0.3.3/fastMONAI/vision_plot.py
+drwxrwxr-x   0 sathiesh  (1001) sathiesh  (1001)        0 2023-07-14 13:46:06.873309 fastMONAI-0.3.3/fastMONAI.egg-info/
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     5428 2023-07-14 13:46:06.000000 fastMONAI-0.3.3/fastMONAI.egg-info/PKG-INFO
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      657 2023-07-14 13:46:06.000000 fastMONAI-0.3.3/fastMONAI.egg-info/SOURCES.txt
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)        1 2023-07-14 13:46:06.000000 fastMONAI-0.3.3/fastMONAI.egg-info/dependency_links.txt
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)       40 2023-07-14 13:46:06.000000 fastMONAI-0.3.3/fastMONAI.egg-info/entry_points.txt
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)        1 2022-08-29 15:24:47.000000 fastMONAI-0.3.3/fastMONAI.egg-info/not-zip-safe
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)      133 2023-07-14 13:46:06.000000 fastMONAI-0.3.3/fastMONAI.egg-info/requires.txt
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)       10 2023-07-14 13:46:06.000000 fastMONAI-0.3.3/fastMONAI.egg-info/top_level.txt
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     1218 2023-07-14 13:40:38.000000 fastMONAI-0.3.3/settings.ini
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)       38 2023-07-14 13:46:06.873309 fastMONAI-0.3.3/setup.cfg
+-rw-rw-r--   0 sathiesh  (1001) sathiesh  (1001)     2541 2022-08-29 15:09:22.000000 fastMONAI-0.3.3/setup.py
```

### Comparing `fastMONAI-0.3.2/CONTRIBUTING.md` & `fastMONAI-0.3.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.2/LICENSE` & `fastMONAI-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.2/PKG-INFO` & `fastMONAI-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastMONAI
-Version: 0.3.2
+Version: 0.3.3
 Summary: fastMONAI library
 Home-page: https://github.com/MMIV-ML/fastMONAI
 Author: Satheshkumar Kaliyugarasan
 Author-email: skka@hvl.no
 License: Apache Software License 2.0
 Keywords: deep learning,medical imaging
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `fastMONAI-0.3.2/README.md` & `fastMONAI-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.2/fastMONAI/_modidx.py` & `fastMONAI-0.3.3/fastMONAI/_modidx.py`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.2/fastMONAI/dataset_info.py` & `fastMONAI-0.3.3/fastMONAI/dataset_info.py`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.2/fastMONAI/external_data.py` & `fastMONAI-0.3.3/fastMONAI/external_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,14 +253,15 @@
         Two pandas DataFrames. The first DataFrame combines training and validation 
         data, and the second DataFrame contains the testing data.
     """
     path = Path(path) / study
     dataset_file_path = path / f'{study}.npz'
 
     try:
+        #todo: check if dataset is downloaded
         download_url(url=MURLs.MEDMNIST_DICT[study], filepath=dataset_file_path)
     except:
         raise ValueError(f"Dataset '{study}' does not exist.")
 
     data = load(dataset_file_path)
     keys = ['train_images', 'val_images', 'test_images']
```

### Comparing `fastMONAI-0.3.2/fastMONAI/research_utils.py` & `fastMONAI-0.3.3/fastMONAI/research_utils.py`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.2/fastMONAI/utils.py` & `fastMONAI-0.3.3/fastMONAI/utils.py`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.2/fastMONAI/vision_augmentation.py` & `fastMONAI-0.3.3/fastMONAI/vision_augmentation.py`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.2/fastMONAI/vision_core.py` & `fastMONAI-0.3.3/fastMONAI/vision_core.py`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.2/fastMONAI/vision_data.py` & `fastMONAI-0.3.3/fastMONAI/vision_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,38 +106,38 @@
         )
 
         return cls.from_dblock(dblock, df, **kwargs)
 
 # %% ../nbs/02_vision_data.ipynb 16
 @typedispatch
 def show_batch(x: MedImage, y, samples, ctxs=None, max_n=6, nrows=None, 
-               ncols=None, figsize=None, channel: int = 0, indices=None, 
-               anatomical_plane: int = 0, **kwargs):
-    """Showing a batch of samples for classification and regression tasks."""
-    
+               ncols=None, figsize=None, channel=0, indices=None,
+               anatomical_plane=0, **kwargs):
+    '''Showing a batch of samples for classification and regression tasks.'''
+
     if ctxs is None: 
         ctxs = get_grid(min(len(samples), max_n), nrows=nrows, ncols=ncols, figsize=figsize)
-    
+        
     n = 1 if y is None else 2
     
     for i in range(n):
         ctxs = [
-            b.show(ctx=c, channel=channel, indices=indices, anatomical_plane=anatomical_plane, **kwargs) 
-            for b, c, _ in zip(samples.itemgot(i), ctxs, range(max_n))
+            b.show(ctx=c, channel=channel, indices=indices, anatomical_plane=anatomical_plane, **kwargs)
+            for b,c,_ in zip(samples.itemgot(i),ctxs,range(max_n))
         ]
 
     plt.tight_layout()
     
     return ctxs
 
 # %% ../nbs/02_vision_data.ipynb 17
 @typedispatch
-def show_batch(x: MedImage, y: MedMask, samples, ctxs=None, max_n=6, nrows: int = None,
-               ncols: int = None, figsize=None, channel: int = 0, indices: int = None,
-               anatomical_plane: int = 0, **kwargs):
+def show_batch(x: MedImage, y: MedMask, samples, ctxs=None, max_n=6, nrows=None,
+               ncols=None, figsize=None, channel=0, indices=None,
+               anatomical_plane=0, **kwargs):
     """Showing a batch of decoded segmentation samples."""
 
     nrows, ncols = min(len(samples), max_n), x.shape[1] + 1
     imgs = []
 
     fig, axs = subplots(nrows, ncols, figsize=figsize, **kwargs)
     axs = axs.flatten()
@@ -222,15 +222,15 @@
                              anatomical_plane=anatomical_plane, **kwargs) 
                       for b, c, _ in zip(o.itemgot(0), ctxs[1::2], range(2 * max_n))]
 
     return ctxs
 
 # %% ../nbs/02_vision_data.ipynb 23
 @typedispatch
-def plot_top_losses(x: MedImage, y, samples, outs, raws, losses, nrows: int = None, 
+def plot_top_losses(x: MedImage, y: TensorCategory, samples, outs, raws, losses, nrows: int = None, 
                     ncols: int = None, figsize=None, channel: int = 0, indices: int = None, 
                     anatomical_plane: int = 0, **kwargs):
     """Show images in top_losses along with their prediction, actual, loss, and probability of actual class."""
 
     title = 'Prediction/Actual/Loss' if isinstance(y, torch.Tensor) else 'Prediction/Actual/Loss/Probability'
     axs = get_grid(len(samples), nrows=nrows, ncols=ncols, figsize=figsize, title=title)
```

### Comparing `fastMONAI-0.3.2/fastMONAI/vision_inference.py` & `fastMONAI-0.3.3/fastMONAI/vision_inference.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/06_vision_inference.ipynb.
 
 # %% auto 0
 __all__ = ['inference', 'refine_binary_pred_mask']
 
 # %% ../nbs/06_vision_inference.ipynb 1
-import numpy as np
+from copy import copy
 from pathlib import Path
-from torchio import Resize
+import torch
+import numpy as np
 from scipy.ndimage import label
-from .vision_core import *
-from .vision_augmentation import do_pad_or_crop
 from skimage.morphology import remove_small_objects
 from SimpleITK import DICOMOrient, GetArrayFromImage
-from copy import copy
+from torchio import Resize
+from .vision_core import *
+from .vision_augmentation import do_pad_or_crop
 
 # %% ../nbs/06_vision_inference.ipynb 3
 def _to_original_orientation(input_img, org_orientation):
     """Reorients the image to its original orientation."""
     
     orientation_itk = DICOMOrient(input_img, org_orientation)
     reoriented_array =  GetArrayFromImage(orientation_itk).transpose()
@@ -70,15 +71,15 @@
     
     return org_img
 
 # %% ../nbs/06_vision_inference.ipynb 7
 def refine_binary_pred_mask(pred_mask, 
                             remove_size: (int, float) = None,
                             percentage: float = 0.2,
-                            verbose: bool = False) -> np.ndarray:
+                            verbose: bool = False) -> torch.Tensor:
     """Removes small objects from the predicted binary mask.
 
     Args:
         pred_mask: The predicted mask from which small objects are to be removed.
         remove_size: The size under which objects are considered 'small'.
         percentage: The percentage of the remove_size to be used as threshold. 
             Defaults to 0.2.
@@ -98,8 +99,8 @@
         max_label = sizes[1:].argmax() + 1
         remove_size = sizes[max_label]
 
     small_objects_threshold = remove_size * percentage
     processed_mask = remove_small_objects(
         labeled_mask, min_size=small_objects_threshold)
 
-    return np.where(processed_mask > 0, 1., 0.)
+    return torch.Tensor(processed_mask > 0).float()
```

### Comparing `fastMONAI-0.3.2/fastMONAI/vision_loss.py` & `fastMONAI-0.3.3/fastMONAI/vision_loss.py`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.2/fastMONAI/vision_metrics.py` & `fastMONAI-0.3.3/fastMONAI/vision_metrics.py`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.2/fastMONAI/vision_plot.py` & `fastMONAI-0.3.3/fastMONAI/vision_plot.py`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.2/fastMONAI.egg-info/PKG-INFO` & `fastMONAI-0.3.3/fastMONAI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastMONAI
-Version: 0.3.2
+Version: 0.3.3
 Summary: fastMONAI library
 Home-page: https://github.com/MMIV-ML/fastMONAI
 Author: Satheshkumar Kaliyugarasan
 Author-email: skka@hvl.no
 License: Apache Software License 2.0
 Keywords: deep learning,medical imaging
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `fastMONAI-0.3.2/fastMONAI.egg-info/SOURCES.txt` & `fastMONAI-0.3.3/fastMONAI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastMONAI-0.3.2/settings.ini` & `fastMONAI-0.3.3/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified
 # see https://github.com/fastai/nbdev/blob/master/settings.ini for examples
 
 ### Python Library ###
 lib_name = fastMONAI
 min_python = 3.7
-version = 0.3.2
+version = 0.3.3
 ### OPTIONAL ###
 
 requirements = fastai==2.7.12 monai==1.2.0 torchio==0.18.91 xlrd>=1.2.0 scikit-image==0.19.3 huggingface-hub gdown
 dev_requirements = ipywidgets nbdev tabulate
 
 ### nbdev ###
 nbs_path = nbs
```

### Comparing `fastMONAI-0.3.2/setup.py` & `fastMONAI-0.3.3/setup.py`

 * *Files identical despite different names*

