# Comparing `tmp/cjm-yolox-pytorch-0.0.92.tar.gz` & `tmp/cjm-yolox-pytorch-0.0.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cjm-yolox-pytorch-0.0.92.tar", last modified: Thu Jul 13 20:17:06 2023, max compression
+gzip compressed data, was "cjm-yolox-pytorch-0.0.93.tar", last modified: Fri Jul 14 18:29:30 2023, max compression
```

## Comparing `cjm-yolox-pytorch-0.0.92.tar` & `cjm-yolox-pytorch-0.0.93.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-13 20:17:06.823843 cjm-yolox-pytorch-0.0.92/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1075 2023-06-22 23:01:16.000000 cjm-yolox-pytorch-0.0.92/LICENSE
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      111 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.92/MANIFEST.in
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1816 2023-07-13 20:17:06.823621 cjm-yolox-pytorch-0.0.92/PKG-INFO
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1050 2023-07-13 20:16:56.000000 cjm-yolox-pytorch-0.0.92/README.md
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-13 20:17:06.820885 cjm-yolox-pytorch-0.0.92/cjm_yolox_pytorch/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       23 2023-07-13 20:16:52.000000 cjm-yolox-pytorch-0.0.92/cjm_yolox_pytorch/__init__.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    12406 2023-07-13 20:16:52.000000 cjm-yolox-pytorch-0.0.92/cjm_yolox_pytorch/_modidx.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    17558 2023-07-13 20:16:52.000000 cjm-yolox-pytorch-0.0.92/cjm_yolox_pytorch/loss.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    35626 2023-07-13 20:16:52.000000 cjm-yolox-pytorch-0.0.92/cjm_yolox_pytorch/model.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    15312 2023-07-13 20:16:52.000000 cjm-yolox-pytorch-0.0.92/cjm_yolox_pytorch/simota.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2618 2023-07-13 20:16:52.000000 cjm-yolox-pytorch-0.0.92/cjm_yolox_pytorch/utils.py
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-13 20:17:06.823288 cjm-yolox-pytorch-0.0.92/cjm_yolox_pytorch.egg-info/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1816 2023-07-13 20:17:06.000000 cjm-yolox-pytorch-0.0.92/cjm_yolox_pytorch.egg-info/PKG-INFO
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      506 2023-07-13 20:17:06.000000 cjm-yolox-pytorch-0.0.92/cjm_yolox_pytorch.egg-info/SOURCES.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-07-13 20:17:06.000000 cjm-yolox-pytorch-0.0.92/cjm_yolox_pytorch.egg-info/dependency_links.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       56 2023-07-13 20:17:06.000000 cjm-yolox-pytorch-0.0.92/cjm_yolox_pytorch.egg-info/entry_points.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-06-23 01:14:13.000000 cjm-yolox-pytorch-0.0.92/cjm_yolox_pytorch.egg-info/not-zip-safe
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       45 2023-07-13 20:17:06.000000 cjm-yolox-pytorch-0.0.92/cjm_yolox_pytorch.egg-info/requires.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       18 2023-07-13 20:17:06.000000 cjm-yolox-pytorch-0.0.92/cjm_yolox_pytorch.egg-info/top_level.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1067 2023-07-13 20:16:47.000000 cjm-yolox-pytorch-0.0.92/settings.ini
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       38 2023-07-13 20:17:06.823912 cjm-yolox-pytorch-0.0.92/setup.cfg
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2596 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.92/setup.py
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-14 18:29:30.819090 cjm-yolox-pytorch-0.0.93/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1075 2023-06-22 23:01:16.000000 cjm-yolox-pytorch-0.0.93/LICENSE
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      111 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.93/MANIFEST.in
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1816 2023-07-14 18:29:30.818762 cjm-yolox-pytorch-0.0.93/PKG-INFO
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1050 2023-07-13 20:16:56.000000 cjm-yolox-pytorch-0.0.93/README.md
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-14 18:29:30.814763 cjm-yolox-pytorch-0.0.93/cjm_yolox_pytorch/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       23 2023-07-14 18:25:27.000000 cjm-yolox-pytorch-0.0.93/cjm_yolox_pytorch/__init__.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    12639 2023-07-14 18:25:27.000000 cjm-yolox-pytorch-0.0.93/cjm_yolox_pytorch/_modidx.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    22521 2023-07-14 18:25:27.000000 cjm-yolox-pytorch-0.0.93/cjm_yolox_pytorch/loss.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    35626 2023-07-14 18:25:27.000000 cjm-yolox-pytorch-0.0.93/cjm_yolox_pytorch/model.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    15312 2023-07-14 18:25:27.000000 cjm-yolox-pytorch-0.0.93/cjm_yolox_pytorch/simota.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     3149 2023-07-14 18:25:27.000000 cjm-yolox-pytorch-0.0.93/cjm_yolox_pytorch/utils.py
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-14 18:29:30.818233 cjm-yolox-pytorch-0.0.93/cjm_yolox_pytorch.egg-info/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1816 2023-07-14 18:29:30.000000 cjm-yolox-pytorch-0.0.93/cjm_yolox_pytorch.egg-info/PKG-INFO
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      506 2023-07-14 18:29:30.000000 cjm-yolox-pytorch-0.0.93/cjm_yolox_pytorch.egg-info/SOURCES.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-07-14 18:29:30.000000 cjm-yolox-pytorch-0.0.93/cjm_yolox_pytorch.egg-info/dependency_links.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       56 2023-07-14 18:29:30.000000 cjm-yolox-pytorch-0.0.93/cjm_yolox_pytorch.egg-info/entry_points.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-06-23 01:14:13.000000 cjm-yolox-pytorch-0.0.93/cjm_yolox_pytorch.egg-info/not-zip-safe
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       45 2023-07-14 18:29:30.000000 cjm-yolox-pytorch-0.0.93/cjm_yolox_pytorch.egg-info/requires.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       18 2023-07-14 18:29:30.000000 cjm-yolox-pytorch-0.0.93/cjm_yolox_pytorch.egg-info/top_level.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1067 2023-07-14 18:24:43.000000 cjm-yolox-pytorch-0.0.93/settings.ini
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       38 2023-07-14 18:29:30.819169 cjm-yolox-pytorch-0.0.93/setup.cfg
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2596 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.93/setup.py
```

### Comparing `cjm-yolox-pytorch-0.0.92/LICENSE` & `cjm-yolox-pytorch-0.0.93/LICENSE`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.92/PKG-INFO` & `cjm-yolox-pytorch-0.0.93/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjm-yolox-pytorch
-Version: 0.0.92
+Version: 0.0.93
 Summary: A PyTorch implementation of the YOLOX object detection model based on the mmdetection implementation.
 Home-page: https://github.com/cj-mills/cjm-yolox-pytorch
 Author: cj-mills
 Author-email: millscj.mills2@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python torch
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cjm-yolox-pytorch-0.0.92/README.md` & `cjm-yolox-pytorch-0.0.93/README.md`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.92/cjm_yolox_pytorch/_modidx.py` & `cjm-yolox-pytorch-0.0.93/cjm_yolox_pytorch/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,10 +94,12 @@
                                                                                                 'cjm_yolox_pytorch/simota.py'),
                                           'cjm_yolox_pytorch.simota.SimOTAAssigner.assign': ( 'simota.html#simotaassigner.assign',
                                                                                               'cjm_yolox_pytorch/simota.py'),
                                           'cjm_yolox_pytorch.simota.SimOTAAssigner.dynamic_k_matching': ( 'simota.html#simotaassigner.dynamic_k_matching',
                                                                                                           'cjm_yolox_pytorch/simota.py'),
                                           'cjm_yolox_pytorch.simota.SimOTAAssigner.get_in_gt_and_in_center_info': ( 'simota.html#simotaassigner.get_in_gt_and_in_center_info',
                                                                                                                     'cjm_yolox_pytorch/simota.py')},
-            'cjm_yolox_pytorch.utils': { 'cjm_yolox_pytorch.utils.generate_output_grids': ( 'utils.html#generate_output_grids',
+            'cjm_yolox_pytorch.utils': { 'cjm_yolox_pytorch.utils.apply_to_inputs': ( 'utils.html#apply_to_inputs',
+                                                                                      'cjm_yolox_pytorch/utils.py'),
+                                         'cjm_yolox_pytorch.utils.generate_output_grids': ( 'utils.html#generate_output_grids',
                                                                                             'cjm_yolox_pytorch/utils.py'),
                                          'cjm_yolox_pytorch.utils.multi_apply': ('utils.html#multi_apply', 'cjm_yolox_pytorch/utils.py')}}}
```

### Comparing `cjm-yolox-pytorch-0.0.92/cjm_yolox_pytorch/loss.py` & `cjm-yolox-pytorch-0.0.93/cjm_yolox_pytorch/loss.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import numpy as np
 
 import torch
 import torch.nn.functional as F
 import torchvision
 
 # %% ../nbs/02_loss.ipynb 5
-from .utils import multi_apply, generate_output_grids
+from .utils import multi_apply, generate_output_grids, apply_to_inputs
 from .simota import AssignResult, SimOTAAssigner
 
 # %% ../nbs/02_loss.ipynb 7
 @dataclass
 class SamplingResult:
     """
     Bounding box sampling result.
@@ -259,14 +259,93 @@
     
     
     def flatten_and_concat(self, tensors, batch_size, reshape_dims=None):
         new_shape = (batch_size, -1, reshape_dims) if reshape_dims else (batch_size, -1)
         return torch.cat([t.permute(0, 2, 3, 1).reshape(*new_shape) for t in tensors], dim=1)
 
     
+#     def __call__(self, class_scores, predicted_bboxes, objectness_scores, ground_truth_bboxes, ground_truth_labels):
+#         """
+#         Main method to compute the YOLOX loss.
+
+#         Args:
+#             class_scores (List[torch.Tensor]): A list of class scores for each scale.
+#             predicted_bboxes (List[torch.Tensor]): A list of predicted bounding boxes for each scale.
+#             objectness_scores (List[torch.Tensor]): A list of objectness scores for each scale.
+#             ground_truth_bboxes (List[torch.Tensor]): A list of ground truth bounding boxes for each image.
+#             ground_truth_labels (List[torch.Tensor]): A list of ground truth labels for each image.
+
+#         Returns:
+#             Dict: A dictionary with the classification, bounding box, objectness, and optionally, L1 loss.
+#         """
+        
+#         # Get the number of images in the batch
+#         batch_size = class_scores[0].shape[0]
+        
+#         # Generate box coordinates for all grid priors.
+#         output_grid_boxes = generate_output_grids(*[s*self.strides[0] for s in class_scores[0].shape[-2:]], self.strides)
+#         output_grid_boxes[:, :2] *= output_grid_boxes[:, 2].unsqueeze(1)
+#         flatten_output_grid_boxes = torch.cat([output_grid_boxes, output_grid_boxes[:, 2:].clone()], dim=1)
+        
+#         # Flatten and concatenate class predictions, bounding box predictions, and objectness scores
+#         flatten_class_preds = self.flatten_and_concat(class_scores, batch_size, self.num_classes)
+#         flatten_bbox_preds = self.flatten_and_concat(predicted_bboxes, batch_size, 4)
+#         flatten_objectness_scores = self.flatten_and_concat(objectness_scores, batch_size)
+                    
+#         # Concatenate and decode box predictions
+#         flatten_output_grid_boxes = flatten_output_grid_boxes.to(flatten_bbox_preds.device)
+#         flatten_decoded_bboxes = self.bbox_decode(flatten_output_grid_boxes, flatten_bbox_preds)
+
+#         # Compute targets
+#         (positive_masks, class_targets, objectness_targets, bbox_targets, l1_targets,
+#          num_positive_images) = multi_apply(
+#              self.get_target_single, flatten_class_preds.detach(),
+#              flatten_objectness_scores.detach(),
+#              flatten_output_grid_boxes.unsqueeze(0).repeat(batch_size, 1, 1),
+#              flatten_decoded_bboxes.detach(), ground_truth_bboxes, ground_truth_labels)
+
+#         # Concatenate all positive masks, class targets, objectness targets, and bounding box targets
+#         positive_masks = torch.cat(positive_masks, 0)
+#         class_targets = torch.cat(class_targets, 0)
+#         objectness_targets = torch.cat(objectness_targets, 0)
+#         bbox_targets = torch.cat(bbox_targets, 0)
+
+#         # Compute bounding box loss
+#         loss_bbox = self.bbox_loss_func(flatten_decoded_bboxes.view(-1, 4)[positive_masks], bbox_targets)
+
+#         # Compute objectness loss
+#         loss_obj = self.objectness_loss_func(flatten_objectness_scores.view(-1, 1), objectness_targets)
+
+#         # Compute class loss
+#         loss_cls = self.class_loss_func(flatten_class_preds.view(-1, self.num_classes)[positive_masks],class_targets)
+        
+#         # Calculate total number of samples
+#         num_total_samples = max(sum(num_positive_images), 1)
+        
+#         # Scale losses
+#         loss_bbox = (loss_bbox * self.bbox_loss_weight) / num_total_samples
+#         loss_obj = (loss_obj * self.objectness_loss_weight) / num_total_samples
+#         loss_cls = (loss_cls * self.class_loss_weight) / num_total_samples
+        
+#         # Initialize loss dictionary
+#         loss_dict = dict(loss_cls=loss_cls, loss_bbox=loss_bbox, loss_obj=loss_obj)
+
+#         # If use_l1 is True, concatenate l1 targets, compute L1 loss and add it to the loss dictionary
+#         if self.use_l1:
+#             l1_targets = torch.cat(l1_targets, 0)
+#             loss_l1 = self.l1_loss_func(
+#                 flatten_bbox_preds.view(-1, 4)[positive_masks],
+#                 l1_targets) / num_total_samples
+#             loss_l1 *= self.l1_loss_weight
+#             loss_dict.update(loss_l1=loss_l1)
+
+#         # Return loss dictionary
+#         return loss_dict
+    
+    
     def __call__(self, class_scores, predicted_bboxes, objectness_scores, ground_truth_bboxes, ground_truth_labels):
         """
         Main method to compute the YOLOX loss.
 
         Args:
             class_scores (List[torch.Tensor]): A list of class scores for each scale.
             predicted_bboxes (List[torch.Tensor]): A list of predicted bounding boxes for each scale.
@@ -291,21 +370,38 @@
         flatten_bbox_preds = self.flatten_and_concat(predicted_bboxes, batch_size, 4)
         flatten_objectness_scores = self.flatten_and_concat(objectness_scores, batch_size)
                     
         # Concatenate and decode box predictions
         flatten_output_grid_boxes = flatten_output_grid_boxes.to(flatten_bbox_preds.device)
         flatten_decoded_bboxes = self.bbox_decode(flatten_output_grid_boxes, flatten_bbox_preds)
 
-        # Compute targets
-        (positive_masks, class_targets, objectness_targets, bbox_targets, l1_targets,
-         num_positive_images) = multi_apply(
-             self.get_target_single, flatten_class_preds.detach(),
-             flatten_objectness_scores.detach(),
-             flatten_output_grid_boxes.unsqueeze(0).repeat(batch_size, 1, 1),
-             flatten_decoded_bboxes.detach(), ground_truth_bboxes, ground_truth_labels)
+        
+        # ---------------------------
+        
+        # Prepare inputs for self.get_target_single
+        inputs = zip(flatten_class_preds.detach(), flatten_objectness_scores.detach(),
+                     flatten_output_grid_boxes.unsqueeze(0).repeat(batch_size, 1, 1),
+                     flatten_decoded_bboxes.detach(), ground_truth_bboxes, ground_truth_labels)
+
+        # Apply self.get_target_single to each input, handling errors and collecting the results
+        target_results = apply_to_inputs(self.get_target_single, inputs)
+
+        # Process the target results
+        positive_masks, class_targets, objectness_targets, bbox_targets, l1_targets, num_positive_images = [], [], [], [], [], []
+        for result in target_results:
+            if result is not None:
+                positive_masks.append(result[0])
+                class_targets.append(result[1])
+                objectness_targets.append(result[2])
+                bbox_targets.append(result[3])
+                l1_targets.append(result[4])
+                num_positive_images.append(result[5])
+        
+        
+        # ---------------------------
 
         # Concatenate all positive masks, class targets, objectness targets, and bounding box targets
         positive_masks = torch.cat(positive_masks, 0)
         class_targets = torch.cat(class_targets, 0)
         objectness_targets = torch.cat(objectness_targets, 0)
         bbox_targets = torch.cat(bbox_targets, 0)
```

### Comparing `cjm-yolox-pytorch-0.0.92/cjm_yolox_pytorch/model.py` & `cjm-yolox-pytorch-0.0.93/cjm_yolox_pytorch/model.py`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.92/cjm_yolox_pytorch/simota.py` & `cjm-yolox-pytorch-0.0.93/cjm_yolox_pytorch/simota.py`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.92/cjm_yolox_pytorch/utils.py` & `cjm-yolox-pytorch-0.0.93/cjm_yolox_pytorch/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/01_utils.ipynb.
 
 # %% auto 0
-__all__ = ['multi_apply', 'generate_output_grids']
+__all__ = ['multi_apply', 'generate_output_grids', 'apply_to_inputs']
 
 # %% ../nbs/01_utils.ipynb 4
 from pathlib import Path
 
 from typing import Any, Type, List, Optional, Callable, Tuple
 from functools import partial
 
@@ -68,7 +68,22 @@
             # Append to the list
             all_coordinates.append(coordinates)
 
         # Concatenate all tensors in the list along the first dimension
         output_grids = torch.cat(all_coordinates, dim=0)
 
         return output_grids
+
+# %% ../nbs/01_utils.ipynb 12
+def apply_to_inputs(func, inputs):
+    """
+    Apply the function `func` to each input in `inputs`, handling errors and returning a list of results.
+    """
+    results = []
+    for input_ in inputs:
+        try:
+            result = func(*input_)
+            results.append(result)
+        except Exception as e:
+            print(f"Error occurred: {str(e)}")
+            results.append(None)  # or raise the exception if you want to stop execution immediately
+    return results
```

### Comparing `cjm-yolox-pytorch-0.0.92/cjm_yolox_pytorch.egg-info/PKG-INFO` & `cjm-yolox-pytorch-0.0.93/cjm_yolox_pytorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjm-yolox-pytorch
-Version: 0.0.92
+Version: 0.0.93
 Summary: A PyTorch implementation of the YOLOX object detection model based on the mmdetection implementation.
 Home-page: https://github.com/cj-mills/cjm-yolox-pytorch
 Author: cj-mills
 Author-email: millscj.mills2@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python torch
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cjm-yolox-pytorch-0.0.92/settings.ini` & `cjm-yolox-pytorch-0.0.93/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = cjm-yolox-pytorch
 lib_name = %(repo)s
-version = 0.0.92
+version = 0.0.93
 min_python = 3.9
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = cjm_yolox_pytorch
```

### Comparing `cjm-yolox-pytorch-0.0.92/setup.py` & `cjm-yolox-pytorch-0.0.93/setup.py`

 * *Files identical despite different names*

