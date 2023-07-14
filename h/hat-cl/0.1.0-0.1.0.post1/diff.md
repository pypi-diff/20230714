# Comparing `tmp/hat_cl-0.1.0.tar.gz` & `tmp/hat_cl-0.1.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hat_cl-0.1.0.tar", max compression
+gzip compressed data, was "hat_cl-0.1.0.post1.tar", max compression
```

## Comparing `hat_cl-0.1.0.tar` & `hat_cl-0.1.0.post1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      289 2023-07-08 21:36:59.367351 hat_cl-0.1.0/hat/__init__.py
--rw-r--r--   0        0        0      739 2023-03-10 21:53:59.498628 hat_cl-0.1.0/hat/_base.py
--rw-r--r--   0        0        0      670 2023-04-30 13:56:25.471519 hat_cl-0.1.0/hat/constants.py
--rw-r--r--   0        0        0     1306 2023-03-20 22:26:30.881305 hat_cl-0.1.0/hat/exceptions.py
--rw-r--r--   0        0        0      626 2023-07-07 16:34:16.699858 hat_cl-0.1.0/hat/modules/__init__.py
--rw-r--r--   0        0        0    23654 2023-07-06 23:02:52.022599 hat_cl-0.1.0/hat/modules/_base.py
--rw-r--r--   0        0        0     5303 2023-07-06 22:37:53.251619 hat_cl-0.1.0/hat/modules/batchnorm.py
--rw-r--r--   0        0        0    10333 2023-04-06 16:12:14.785307 hat_cl-0.1.0/hat/modules/conv.py
--rw-r--r--   0        0        0     3799 2023-03-16 12:06:23.689102 hat_cl-0.1.0/hat/modules/linear.py
--rw-r--r--   0        0        0      201 2023-03-15 22:46:20.733492 hat_cl-0.1.0/hat/modules/maskers/__init__.py
--rw-r--r--   0        0        0     4890 2023-04-06 16:12:14.786754 hat_cl-0.1.0/hat/modules/maskers/_base.py
--rw-r--r--   0        0        0     4278 2023-03-16 23:17:27.119883 hat_cl-0.1.0/hat/modules/maskers/attention_masker.py
--rw-r--r--   0        0        0     2216 2023-03-15 23:08:19.830720 hat_cl-0.1.0/hat/modules/maskers/constant_masker.py
--rw-r--r--   0        0        0    28742 2023-07-13 19:23:14.300466 hat_cl-0.1.0/hat/modules/maskers/hat_masker.py
--rw-r--r--   0        0        0     4203 2023-07-06 22:59:31.786664 hat_cl-0.1.0/hat/modules/normalization.py
--rw-r--r--   0        0        0      793 2023-07-06 22:55:22.706413 hat_cl-0.1.0/hat/modules/utils.py
--rw-r--r--   0        0        0     1166 2023-07-12 15:36:44.437379 hat_cl-0.1.0/hat/parameter.py
--rw-r--r--   0        0        0    12772 2023-07-13 19:17:35.308775 hat_cl-0.1.0/hat/payload.py
--rw-r--r--   0        0        0      446 2023-07-08 17:47:42.673708 hat_cl-0.1.0/hat/timm_models/__init__.py
--rw-r--r--   0        0        0      113 2023-07-08 20:05:21.869773 hat_cl-0.1.0/hat/timm_models/layers/__init__.py
--rw-r--r--   0        0        0     1769 2023-07-09 19:06:03.701806 hat_cl-0.1.0/hat/timm_models/layers/mlp.py
--rw-r--r--   0        0        0     2742 2023-07-13 19:14:59.122973 hat_cl-0.1.0/hat/timm_models/layers/patch_embed.py
--rw-r--r--   0        0        0    13453 2023-07-12 16:14:40.458425 hat_cl-0.1.0/hat/timm_models/resnet.py
--rw-r--r--   0        0        0      132 2023-07-08 17:50:19.031793 hat_cl-0.1.0/hat/timm_models/utils/__init__.py
--rw-r--r--   0        0        0     1595 2023-07-08 22:38:44.855800 hat_cl-0.1.0/hat/timm_models/utils/conversion.py
--rw-r--r--   0        0        0    29933 2023-07-14 16:17:45.419209 hat_cl-0.1.0/hat/timm_models/vision_transformer.py
--rw-r--r--   0        0        0     5807 2023-04-30 13:59:33.537756 hat_cl-0.1.0/hat/types_.py
--rw-r--r--   0        0        0      556 2023-04-18 23:05:59.580507 hat_cl-0.1.0/hat/utils/__init__.py
--rw-r--r--   0        0        0     4339 2023-03-15 23:04:08.822439 hat_cl-0.1.0/hat/utils/conversion.py
--rw-r--r--   0        0        0     3070 2023-04-06 16:12:14.764344 hat_cl-0.1.0/hat/utils/forgetting.py
--rw-r--r--   0        0        0     4292 2023-03-15 23:05:48.394260 hat_cl-0.1.0/hat/utils/forward.py
--rw-r--r--   0        0        0     2337 2023-07-05 19:16:11.219615 hat_cl-0.1.0/hat/utils/inspection.py
--rw-r--r--   0        0        0     1679 2023-03-16 16:57:58.028942 hat_cl-0.1.0/hat/utils/pruning.py
--rw-r--r--   0        0        0      938 2023-07-06 22:55:56.728696 hat_cl-0.1.0/hat/utils/regularization.py
--rw-r--r--   0        0        0     4946 2023-04-30 13:47:28.331687 hat_cl-0.1.0/hat/utils/scaling.py
--rw-r--r--   0        0        0     1627 2023-03-27 16:25:51.502678 hat_cl-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1304 2023-07-14 18:16:14.952595 hat_cl-0.1.0/readme.md
--rw-r--r--   0        0        0     1875 1970-01-01 00:00:00.000000 hat_cl-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      289 2023-07-08 21:36:59.367351 hat_cl-0.1.0.post1/hat/__init__.py
+-rw-r--r--   0        0        0      739 2023-03-10 21:53:59.498628 hat_cl-0.1.0.post1/hat/_base.py
+-rw-r--r--   0        0        0      670 2023-04-30 13:56:25.471519 hat_cl-0.1.0.post1/hat/constants.py
+-rw-r--r--   0        0        0     1306 2023-03-20 22:26:30.881305 hat_cl-0.1.0.post1/hat/exceptions.py
+-rw-r--r--   0        0        0      626 2023-07-07 16:34:16.699858 hat_cl-0.1.0.post1/hat/modules/__init__.py
+-rw-r--r--   0        0        0    23654 2023-07-06 23:02:52.022599 hat_cl-0.1.0.post1/hat/modules/_base.py
+-rw-r--r--   0        0        0     5303 2023-07-06 22:37:53.251619 hat_cl-0.1.0.post1/hat/modules/batchnorm.py
+-rw-r--r--   0        0        0    10333 2023-04-06 16:12:14.785307 hat_cl-0.1.0.post1/hat/modules/conv.py
+-rw-r--r--   0        0        0     3799 2023-03-16 12:06:23.689102 hat_cl-0.1.0.post1/hat/modules/linear.py
+-rw-r--r--   0        0        0      201 2023-03-15 22:46:20.733492 hat_cl-0.1.0.post1/hat/modules/maskers/__init__.py
+-rw-r--r--   0        0        0     4890 2023-04-06 16:12:14.786754 hat_cl-0.1.0.post1/hat/modules/maskers/_base.py
+-rw-r--r--   0        0        0     4278 2023-03-16 23:17:27.119883 hat_cl-0.1.0.post1/hat/modules/maskers/attention_masker.py
+-rw-r--r--   0        0        0     2216 2023-03-15 23:08:19.830720 hat_cl-0.1.0.post1/hat/modules/maskers/constant_masker.py
+-rw-r--r--   0        0        0    28742 2023-07-13 19:23:14.300466 hat_cl-0.1.0.post1/hat/modules/maskers/hat_masker.py
+-rw-r--r--   0        0        0     4203 2023-07-06 22:59:31.786664 hat_cl-0.1.0.post1/hat/modules/normalization.py
+-rw-r--r--   0        0        0      793 2023-07-06 22:55:22.706413 hat_cl-0.1.0.post1/hat/modules/utils.py
+-rw-r--r--   0        0        0     1166 2023-07-12 15:36:44.437379 hat_cl-0.1.0.post1/hat/parameter.py
+-rw-r--r--   0        0        0    12772 2023-07-13 19:17:35.308775 hat_cl-0.1.0.post1/hat/payload.py
+-rw-r--r--   0        0        0      446 2023-07-08 17:47:42.673708 hat_cl-0.1.0.post1/hat/timm_models/__init__.py
+-rw-r--r--   0        0        0      113 2023-07-08 20:05:21.869773 hat_cl-0.1.0.post1/hat/timm_models/layers/__init__.py
+-rw-r--r--   0        0        0     1769 2023-07-09 19:06:03.701806 hat_cl-0.1.0.post1/hat/timm_models/layers/mlp.py
+-rw-r--r--   0        0        0     2742 2023-07-13 19:14:59.122973 hat_cl-0.1.0.post1/hat/timm_models/layers/patch_embed.py
+-rw-r--r--   0        0        0    13453 2023-07-12 16:14:40.458425 hat_cl-0.1.0.post1/hat/timm_models/resnet.py
+-rw-r--r--   0        0        0      132 2023-07-08 17:50:19.031793 hat_cl-0.1.0.post1/hat/timm_models/utils/__init__.py
+-rw-r--r--   0        0        0     1595 2023-07-08 22:38:44.855800 hat_cl-0.1.0.post1/hat/timm_models/utils/conversion.py
+-rw-r--r--   0        0        0    29933 2023-07-14 16:17:45.419209 hat_cl-0.1.0.post1/hat/timm_models/vision_transformer.py
+-rw-r--r--   0        0        0     5807 2023-04-30 13:59:33.537756 hat_cl-0.1.0.post1/hat/types_.py
+-rw-r--r--   0        0        0      556 2023-04-18 23:05:59.580507 hat_cl-0.1.0.post1/hat/utils/__init__.py
+-rw-r--r--   0        0        0     4339 2023-03-15 23:04:08.822439 hat_cl-0.1.0.post1/hat/utils/conversion.py
+-rw-r--r--   0        0        0     3070 2023-04-06 16:12:14.764344 hat_cl-0.1.0.post1/hat/utils/forgetting.py
+-rw-r--r--   0        0        0     4292 2023-03-15 23:05:48.394260 hat_cl-0.1.0.post1/hat/utils/forward.py
+-rw-r--r--   0        0        0     2337 2023-07-05 19:16:11.219615 hat_cl-0.1.0.post1/hat/utils/inspection.py
+-rw-r--r--   0        0        0     1679 2023-03-16 16:57:58.028942 hat_cl-0.1.0.post1/hat/utils/pruning.py
+-rw-r--r--   0        0        0      938 2023-07-06 22:55:56.728696 hat_cl-0.1.0.post1/hat/utils/regularization.py
+-rw-r--r--   0        0        0     4946 2023-04-30 13:47:28.331687 hat_cl-0.1.0.post1/hat/utils/scaling.py
+-rw-r--r--   0        0        0     1633 2023-07-14 20:56:54.996072 hat_cl-0.1.0.post1/pyproject.toml
+-rw-r--r--   0        0        0     5850 2023-07-14 20:52:47.260287 hat_cl-0.1.0.post1/readme.md
+-rw-r--r--   0        0        0     6427 1970-01-01 00:00:00.000000 hat_cl-0.1.0.post1/PKG-INFO
```

### Comparing `hat_cl-0.1.0/hat/_base.py` & `hat_cl-0.1.0.post1/hat/_base.py`

 * *Files identical despite different names*

### Comparing `hat_cl-0.1.0/hat/constants.py` & `hat_cl-0.1.0.post1/hat/constants.py`

 * *Files identical despite different names*

### Comparing `hat_cl-0.1.0/hat/exceptions.py` & `hat_cl-0.1.0.post1/hat/exceptions.py`

 * *Files identical despite different names*

### Comparing `hat_cl-0.1.0/hat/modules/__init__.py` & `hat_cl-0.1.0.post1/hat/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `hat_cl-0.1.0/hat/modules/_base.py` & `hat_cl-0.1.0.post1/hat/modules/_base.py`

 * *Files identical despite different names*

### Comparing `hat_cl-0.1.0/hat/modules/batchnorm.py` & `hat_cl-0.1.0.post1/hat/modules/batchnorm.py`

 * *Files identical despite different names*

### Comparing `hat_cl-0.1.0/hat/modules/conv.py` & `hat_cl-0.1.0.post1/hat/modules/conv.py`

 * *Files identical despite different names*

### Comparing `hat_cl-0.1.0/hat/modules/linear.py` & `hat_cl-0.1.0.post1/hat/modules/linear.py`

 * *Files identical despite different names*

### Comparing `hat_cl-0.1.0/hat/modules/maskers/_base.py` & `hat_cl-0.1.0.post1/hat/modules/maskers/_base.py`

 * *Files identical despite different names*

### Comparing `hat_cl-0.1.0/hat/modules/maskers/attention_masker.py` & `hat_cl-0.1.0.post1/hat/modules/maskers/attention_masker.py`

 * *Files identical despite different names*

### Comparing `hat_cl-0.1.0/hat/modules/maskers/constant_masker.py` & `hat_cl-0.1.0.post1/hat/modules/maskers/constant_masker.py`

 * *Files identical despite different names*

### Comparing `hat_cl-0.1.0/hat/modules/maskers/hat_masker.py` & `hat_cl-0.1.0.post1/hat/modules/maskers/hat_masker.py`

 * *Files identical despite different names*

### Comparing `hat_cl-0.1.0/hat/modules/normalization.py` & `hat_cl-0.1.0.post1/hat/modules/normalization.py`

 * *Files identical despite different names*

### Comparing `hat_cl-0.1.0/hat/modules/utils.py` & `hat_cl-0.1.0.post1/hat/modules/utils.py`

 * *Files identical despite different names*

### Comparing `hat_cl-0.1.0/hat/parameter.py` & `hat_cl-0.1.0.post1/hat/parameter.py`

 * *Files identical despite different names*

### Comparing `hat_cl-0.1.0/hat/payload.py` & `hat_cl-0.1.0.post1/hat/payload.py`

 * *Files identical despite different names*

### Comparing `hat_cl-0.1.0/hat/timm_models/layers/mlp.py` & `hat_cl-0.1.0.post1/hat/timm_models/layers/mlp.py`

 * *Files identical despite different names*

### Comparing `hat_cl-0.1.0/hat/timm_models/layers/patch_embed.py` & `hat_cl-0.1.0.post1/hat/timm_models/layers/patch_embed.py`

 * *Files identical despite different names*

### Comparing `hat_cl-0.1.0/hat/timm_models/resnet.py` & `hat_cl-0.1.0.post1/hat/timm_models/resnet.py`

 * *Files identical despite different names*

### Comparing `hat_cl-0.1.0/hat/timm_models/utils/conversion.py` & `hat_cl-0.1.0.post1/hat/timm_models/utils/conversion.py`

 * *Files identical despite different names*

### Comparing `hat_cl-0.1.0/hat/timm_models/vision_transformer.py` & `hat_cl-0.1.0.post1/hat/timm_models/vision_transformer.py`

 * *Files identical despite different names*

### Comparing `hat_cl-0.1.0/hat/types_.py` & `hat_cl-0.1.0.post1/hat/types_.py`

 * *Files identical despite different names*

### Comparing `hat_cl-0.1.0/hat/utils/__init__.py` & `hat_cl-0.1.0.post1/hat/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hat_cl-0.1.0/hat/utils/conversion.py` & `hat_cl-0.1.0.post1/hat/utils/conversion.py`

 * *Files identical despite different names*

### Comparing `hat_cl-0.1.0/hat/utils/forgetting.py` & `hat_cl-0.1.0.post1/hat/utils/forgetting.py`

 * *Files identical despite different names*

### Comparing `hat_cl-0.1.0/hat/utils/forward.py` & `hat_cl-0.1.0.post1/hat/utils/forward.py`

 * *Files identical despite different names*

### Comparing `hat_cl-0.1.0/hat/utils/inspection.py` & `hat_cl-0.1.0.post1/hat/utils/inspection.py`

 * *Files identical despite different names*

### Comparing `hat_cl-0.1.0/hat/utils/pruning.py` & `hat_cl-0.1.0.post1/hat/utils/pruning.py`

 * *Files identical despite different names*

### Comparing `hat_cl-0.1.0/hat/utils/regularization.py` & `hat_cl-0.1.0.post1/hat/utils/regularization.py`

 * *Files identical despite different names*

### Comparing `hat_cl-0.1.0/hat/utils/scaling.py` & `hat_cl-0.1.0.post1/hat/utils/scaling.py`

 * *Files identical despite different names*

### Comparing `hat_cl-0.1.0/pyproject.toml` & `hat_cl-0.1.0.post1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hat-cl"
-version = "0.1.0"
+version = "0.1.0.post1"
 description = "HAT (Hard Attention to the Task) Modules for Continual Learning"
 authors = ["Xiaotian Duan <xduan7@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 packages = [{include = "hat"}]
 
 [tool.poetry.dependencies]
```

