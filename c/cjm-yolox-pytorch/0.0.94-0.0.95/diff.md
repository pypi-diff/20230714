# Comparing `tmp/cjm-yolox-pytorch-0.0.94.tar.gz` & `tmp/cjm-yolox-pytorch-0.0.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cjm-yolox-pytorch-0.0.94.tar", last modified: Fri Jul 14 20:44:47 2023, max compression
+gzip compressed data, was "cjm-yolox-pytorch-0.0.95.tar", last modified: Fri Jul 14 21:41:22 2023, max compression
```

## Comparing `cjm-yolox-pytorch-0.0.94.tar` & `cjm-yolox-pytorch-0.0.95.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-14 20:44:47.878891 cjm-yolox-pytorch-0.0.94/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1075 2023-06-22 23:01:16.000000 cjm-yolox-pytorch-0.0.94/LICENSE
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      111 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.94/MANIFEST.in
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1816 2023-07-14 20:44:47.878717 cjm-yolox-pytorch-0.0.94/PKG-INFO
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1050 2023-07-13 20:16:56.000000 cjm-yolox-pytorch-0.0.94/README.md
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-14 20:44:47.876296 cjm-yolox-pytorch-0.0.94/cjm_yolox_pytorch/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       23 2023-07-14 20:44:11.000000 cjm-yolox-pytorch-0.0.94/cjm_yolox_pytorch/__init__.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    12639 2023-07-14 20:44:11.000000 cjm-yolox-pytorch-0.0.94/cjm_yolox_pytorch/_modidx.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    23438 2023-07-14 20:44:11.000000 cjm-yolox-pytorch-0.0.94/cjm_yolox_pytorch/loss.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    35626 2023-07-14 20:44:11.000000 cjm-yolox-pytorch-0.0.94/cjm_yolox_pytorch/model.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    15312 2023-07-14 20:44:11.000000 cjm-yolox-pytorch-0.0.94/cjm_yolox_pytorch/simota.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     3149 2023-07-14 20:44:11.000000 cjm-yolox-pytorch-0.0.94/cjm_yolox_pytorch/utils.py
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-14 20:44:47.878382 cjm-yolox-pytorch-0.0.94/cjm_yolox_pytorch.egg-info/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1816 2023-07-14 20:44:47.000000 cjm-yolox-pytorch-0.0.94/cjm_yolox_pytorch.egg-info/PKG-INFO
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      506 2023-07-14 20:44:47.000000 cjm-yolox-pytorch-0.0.94/cjm_yolox_pytorch.egg-info/SOURCES.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-07-14 20:44:47.000000 cjm-yolox-pytorch-0.0.94/cjm_yolox_pytorch.egg-info/dependency_links.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       56 2023-07-14 20:44:47.000000 cjm-yolox-pytorch-0.0.94/cjm_yolox_pytorch.egg-info/entry_points.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-06-23 01:14:13.000000 cjm-yolox-pytorch-0.0.94/cjm_yolox_pytorch.egg-info/not-zip-safe
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       45 2023-07-14 20:44:47.000000 cjm-yolox-pytorch-0.0.94/cjm_yolox_pytorch.egg-info/requires.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       18 2023-07-14 20:44:47.000000 cjm-yolox-pytorch-0.0.94/cjm_yolox_pytorch.egg-info/top_level.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1067 2023-07-14 20:43:45.000000 cjm-yolox-pytorch-0.0.94/settings.ini
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       38 2023-07-14 20:44:47.878943 cjm-yolox-pytorch-0.0.94/setup.cfg
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2596 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.94/setup.py
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-14 21:41:22.152891 cjm-yolox-pytorch-0.0.95/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1075 2023-06-22 23:01:16.000000 cjm-yolox-pytorch-0.0.95/LICENSE
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      111 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.95/MANIFEST.in
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1816 2023-07-14 21:41:22.152736 cjm-yolox-pytorch-0.0.95/PKG-INFO
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1050 2023-07-13 20:16:56.000000 cjm-yolox-pytorch-0.0.95/README.md
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-14 21:41:22.150404 cjm-yolox-pytorch-0.0.95/cjm_yolox_pytorch/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       23 2023-07-14 21:41:06.000000 cjm-yolox-pytorch-0.0.95/cjm_yolox_pytorch/__init__.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    12639 2023-07-14 21:41:06.000000 cjm-yolox-pytorch-0.0.95/cjm_yolox_pytorch/_modidx.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    24714 2023-07-14 21:41:06.000000 cjm-yolox-pytorch-0.0.95/cjm_yolox_pytorch/loss.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    35626 2023-07-14 21:41:06.000000 cjm-yolox-pytorch-0.0.95/cjm_yolox_pytorch/model.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    15312 2023-07-14 21:41:06.000000 cjm-yolox-pytorch-0.0.95/cjm_yolox_pytorch/simota.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     3149 2023-07-14 21:41:06.000000 cjm-yolox-pytorch-0.0.95/cjm_yolox_pytorch/utils.py
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-14 21:41:22.152415 cjm-yolox-pytorch-0.0.95/cjm_yolox_pytorch.egg-info/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1816 2023-07-14 21:41:22.000000 cjm-yolox-pytorch-0.0.95/cjm_yolox_pytorch.egg-info/PKG-INFO
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      506 2023-07-14 21:41:22.000000 cjm-yolox-pytorch-0.0.95/cjm_yolox_pytorch.egg-info/SOURCES.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-07-14 21:41:22.000000 cjm-yolox-pytorch-0.0.95/cjm_yolox_pytorch.egg-info/dependency_links.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       56 2023-07-14 21:41:22.000000 cjm-yolox-pytorch-0.0.95/cjm_yolox_pytorch.egg-info/entry_points.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-06-23 01:14:13.000000 cjm-yolox-pytorch-0.0.95/cjm_yolox_pytorch.egg-info/not-zip-safe
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       45 2023-07-14 21:41:22.000000 cjm-yolox-pytorch-0.0.95/cjm_yolox_pytorch.egg-info/requires.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       18 2023-07-14 21:41:22.000000 cjm-yolox-pytorch-0.0.95/cjm_yolox_pytorch.egg-info/top_level.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1067 2023-07-14 21:40:24.000000 cjm-yolox-pytorch-0.0.95/settings.ini
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       38 2023-07-14 21:41:22.152940 cjm-yolox-pytorch-0.0.95/setup.cfg
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2596 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.95/setup.py
```

### Comparing `cjm-yolox-pytorch-0.0.94/LICENSE` & `cjm-yolox-pytorch-0.0.95/LICENSE`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.94/PKG-INFO` & `cjm-yolox-pytorch-0.0.95/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjm-yolox-pytorch
-Version: 0.0.94
+Version: 0.0.95
 Summary: A PyTorch implementation of the YOLOX object detection model based on the mmdetection implementation.
 Home-page: https://github.com/cj-mills/cjm-yolox-pytorch
 Author: cj-mills
 Author-email: millscj.mills2@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python torch
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cjm-yolox-pytorch-0.0.94/README.md` & `cjm-yolox-pytorch-0.0.95/README.md`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.94/cjm_yolox_pytorch/_modidx.py` & `cjm-yolox-pytorch-0.0.95/cjm_yolox_pytorch/_modidx.py`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.94/cjm_yolox_pytorch/loss.py` & `cjm-yolox-pytorch-0.0.95/cjm_yolox_pytorch/loss.py`

 * *Files 5% similar despite different names*

```diff
@@ -412,47 +412,76 @@
         else:
             objectness_targets = torch.cat(objectness_targets, 0)
 
         if len(bbox_targets) == 0:
             bbox_targets = torch.empty((0, 4), dtype=torch.float32, device=class_scores[0].device)
         else:
             bbox_targets = torch.cat(bbox_targets, 0)
+            
+            
+        # Compute bounding box loss
+        if positive_masks.shape[0] > 0:
+            loss_bbox = self.bbox_loss_func(flatten_decoded_bboxes.view(-1, 4)[positive_masks], bbox_targets)
+        else:
+            loss_bbox = torch.tensor(0.).to(class_scores[0].device)
+
+        # Compute objectness loss
+        loss_obj = self.objectness_loss_func(flatten_objectness_scores.view(-1, 1), objectness_targets)
+
+        # Compute class loss
+        if positive_masks.shape[0] > 0:
+            loss_cls = self.class_loss_func(flatten_class_preds.view(-1, self.num_classes)[positive_masks], class_targets)
+        else:
+            loss_cls = torch.tensor(0.).to(class_scores[0].device)
+
+        # For L1 loss, do the same
+        if self.use_l1:
+            if positive_masks.shape[0] > 0:
+                l1_targets = torch.cat(l1_targets, 0)
+                loss_l1 = self.l1_loss_func(
+                    flatten_bbox_preds.view(-1, 4)[positive_masks],
+                    l1_targets) / num_total_samples
+                loss_l1 *= self.l1_loss_weight
+                loss_dict.update(loss_l1=loss_l1)
+            else:
+                loss_dict.update(loss_l1=torch.tensor(0.).to(class_scores[0].device))
+
 
         # ---------------------------
 
 #         # Concatenate all positive masks, class targets, objectness targets, and bounding box targets
 #         positive_masks = torch.cat(positive_masks, 0)
 #         class_targets = torch.cat(class_targets, 0)
 #         objectness_targets = torch.cat(objectness_targets, 0)
 #         bbox_targets = torch.cat(bbox_targets, 0)
 
-        # Compute bounding box loss
-        loss_bbox = self.bbox_loss_func(flatten_decoded_bboxes.view(-1, 4)[positive_masks], bbox_targets)
+#         # Compute bounding box loss
+#         loss_bbox = self.bbox_loss_func(flatten_decoded_bboxes.view(-1, 4)[positive_masks], bbox_targets)
 
-        # Compute objectness loss
-        loss_obj = self.objectness_loss_func(flatten_objectness_scores.view(-1, 1), objectness_targets)
+#         # Compute objectness loss
+#         loss_obj = self.objectness_loss_func(flatten_objectness_scores.view(-1, 1), objectness_targets)
 
-        # Compute class loss
-        loss_cls = self.class_loss_func(flatten_class_preds.view(-1, self.num_classes)[positive_masks],class_targets)
+#         # Compute class loss
+#         loss_cls = self.class_loss_func(flatten_class_preds.view(-1, self.num_classes)[positive_masks],class_targets)
         
-        # Calculate total number of samples
-        num_total_samples = max(sum(num_positive_images), 1)
+#         # Calculate total number of samples
+#         num_total_samples = max(sum(num_positive_images), 1)
         
-        # Scale losses
-        loss_bbox = (loss_bbox * self.bbox_loss_weight) / num_total_samples
-        loss_obj = (loss_obj * self.objectness_loss_weight) / num_total_samples
-        loss_cls = (loss_cls * self.class_loss_weight) / num_total_samples
+#         # Scale losses
+#         loss_bbox = (loss_bbox * self.bbox_loss_weight) / num_total_samples
+#         loss_obj = (loss_obj * self.objectness_loss_weight) / num_total_samples
+#         loss_cls = (loss_cls * self.class_loss_weight) / num_total_samples
         
-        # Initialize loss dictionary
-        loss_dict = dict(loss_cls=loss_cls, loss_bbox=loss_bbox, loss_obj=loss_obj)
+#         # Initialize loss dictionary
+#         loss_dict = dict(loss_cls=loss_cls, loss_bbox=loss_bbox, loss_obj=loss_obj)
 
-        # If use_l1 is True, concatenate l1 targets, compute L1 loss and add it to the loss dictionary
-        if self.use_l1:
-            l1_targets = torch.cat(l1_targets, 0)
-            loss_l1 = self.l1_loss_func(
-                flatten_bbox_preds.view(-1, 4)[positive_masks],
-                l1_targets) / num_total_samples
-            loss_l1 *= self.l1_loss_weight
-            loss_dict.update(loss_l1=loss_l1)
+#         # If use_l1 is True, concatenate l1 targets, compute L1 loss and add it to the loss dictionary
+#         if self.use_l1:
+#             l1_targets = torch.cat(l1_targets, 0)
+#             loss_l1 = self.l1_loss_func(
+#                 flatten_bbox_preds.view(-1, 4)[positive_masks],
+#                 l1_targets) / num_total_samples
+#             loss_l1 *= self.l1_loss_weight
+#             loss_dict.update(loss_l1=loss_l1)
 
         # Return loss dictionary
         return loss_dict
```

### Comparing `cjm-yolox-pytorch-0.0.94/cjm_yolox_pytorch/model.py` & `cjm-yolox-pytorch-0.0.95/cjm_yolox_pytorch/model.py`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.94/cjm_yolox_pytorch/simota.py` & `cjm-yolox-pytorch-0.0.95/cjm_yolox_pytorch/simota.py`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.94/cjm_yolox_pytorch/utils.py` & `cjm-yolox-pytorch-0.0.95/cjm_yolox_pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.94/cjm_yolox_pytorch.egg-info/PKG-INFO` & `cjm-yolox-pytorch-0.0.95/cjm_yolox_pytorch.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjm-yolox-pytorch
-Version: 0.0.94
+Version: 0.0.95
 Summary: A PyTorch implementation of the YOLOX object detection model based on the mmdetection implementation.
 Home-page: https://github.com/cj-mills/cjm-yolox-pytorch
 Author: cj-mills
 Author-email: millscj.mills2@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python torch
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cjm-yolox-pytorch-0.0.94/settings.ini` & `cjm-yolox-pytorch-0.0.95/settings.ini`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = cjm-yolox-pytorch
 lib_name = %(repo)s
-version = 0.0.94
+version = 0.0.95
 min_python = 3.9
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = cjm_yolox_pytorch
```

### Comparing `cjm-yolox-pytorch-0.0.94/setup.py` & `cjm-yolox-pytorch-0.0.95/setup.py`

 * *Files identical despite different names*

