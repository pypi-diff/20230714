# Comparing `tmp/x-unet-0.3.0.tar.gz` & `tmp/x-unet-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "x-unet-0.3.0.tar", last modified: Thu Jan  5 18:47:30 2023, max compression
+gzip compressed data, was "x-unet-0.3.1.tar", last modified: Fri Jul 14 14:42:29 2023, max compression
```

## Comparing `x-unet-0.3.0.tar` & `x-unet-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 18:47:30.973292 x-unet-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-01-05 18:47:18.000000 x-unet-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-01-05 18:47:30.973292 x-unet-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-01-05 18:47:18.000000 x-unet-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-05 18:47:30.973292 x-unet-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-01-05 18:47:18.000000 x-unet-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 18:47:30.973292 x-unet-0.3.0/x_unet/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-01-05 18:47:18.000000 x-unet-0.3.0/x_unet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18874 2023-01-05 18:47:18.000000 x-unet-0.3.0/x_unet/x_unet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 18:47:30.973292 x-unet-0.3.0/x_unet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-01-05 18:47:30.000000 x-unet-0.3.0/x_unet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-01-05 18:47:30.000000 x-unet-0.3.0/x_unet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 18:47:30.000000 x-unet-0.3.0/x_unet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-05 18:47:30.000000 x-unet-0.3.0/x_unet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-05 18:47:30.000000 x-unet-0.3.0/x_unet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:42:29.186716 x-unet-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-14 14:42:17.000000 x-unet-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-14 14:42:29.186716 x-unet-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-14 14:42:17.000000 x-unet-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 14:42:29.186716 x-unet-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-14 14:42:17.000000 x-unet-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:42:29.182716 x-unet-0.3.1/x_unet/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-14 14:42:17.000000 x-unet-0.3.1/x_unet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19339 2023-07-14 14:42:17.000000 x-unet-0.3.1/x_unet/x_unet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:42:29.182716 x-unet-0.3.1/x_unet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-14 14:42:29.000000 x-unet-0.3.1/x_unet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-14 14:42:29.000000 x-unet-0.3.1/x_unet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 14:42:29.000000 x-unet-0.3.1/x_unet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-14 14:42:29.000000 x-unet-0.3.1/x_unet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 14:42:29.000000 x-unet-0.3.1/x_unet.egg-info/top_level.txt
```

### Comparing `x-unet-0.3.0/LICENSE` & `x-unet-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `x-unet-0.3.0/PKG-INFO` & `x-unet-0.3.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x-unet
-Version: 0.3.0
+Version: 0.3.1
 Summary: X-Unet
 Home-page: https://github.com/lucidrains/x-unet
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,biomedical segmentation,medical deep learning,unets
 Classifier: Development Status :: 4 - Beta
```

### Comparing `x-unet-0.3.0/README.md` & `x-unet-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `x-unet-0.3.0/setup.py` & `x-unet-0.3.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'x-unet',
   packages = find_packages(exclude=[]),
-  version = '0.3.0',
+  version = '0.3.1',
   license='MIT',
   description = 'X-Unet',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/x-unet',
   keywords = [
     'artificial intelligence',
     'deep learning',
     'biomedical segmentation',
     'medical deep learning',
     'unets',
   ],
   install_requires=[
+    'beartype',
     'einops>=0.4',
     'torch>=1.6',
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
```

### Comparing `x-unet-0.3.0/x_unet/x_unet.py` & `x-unet-0.3.1/x_unet/x_unet.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 import torch
 from torch import nn, einsum
 import torch.nn.functional as F
 
 from einops import rearrange, repeat, reduce
 from einops.layers.torch import Rearrange
 
+from beartype import beartype
+from beartype.typing import Tuple, Union, Optional
+
 # helper functions
 
 def exists(val):
     return val is not None
 
 def default(val, d):
     return val if exists(val) else d
@@ -287,38 +290,43 @@
         if self.resize_fmap_before:
             outs = self.resize_fmaps(outs, target_height, target_width)
 
         return torch.cat((x, *outs), dim = 1)
 
 # unet
 
+def MaybeTuple(type):
+    return Union[type, Tuple[type, ...]]
+
 def kernel_and_same_pad(*kernel_size):
     paddings = tuple(map(lambda k: k // 2, kernel_size))
     return dict(kernel_size = kernel_size, padding = paddings)
 
 class XUnet(nn.Module):
+
+    @beartype
     def __init__(
         self,
         dim,
         init_dim = None,
         out_dim = None,
         frame_kernel_size = 1,
-        dim_mults = (1, 2, 4, 8),
-        num_blocks_per_stage = (2, 2, 2, 2),
-        num_self_attn_per_stage = (0, 0, 0, 1),
-        nested_unet_depths = (0, 0, 0, 0),
+        dim_mults: MaybeTuple(int) = (1, 2, 4, 8),
+        num_blocks_per_stage: MaybeTuple(int) = (2, 2, 2, 2),
+        num_self_attn_per_stage: MaybeTuple(int) = (0, 0, 0, 1),
+        nested_unet_depths: MaybeTuple(int) = (0, 0, 0, 0),
         nested_unet_dim = 32,
         channels = 3,
         use_convnext = False,
         resnet_groups = 8,
         consolidate_upsample_fmaps = True,
         skip_scale = 2 ** -0.5,
         weight_standardize = False,
-        attn_heads = 8,
-        attn_dim_head = 32
+        attn_heads: MaybeTuple(int) = 8,
+        attn_dim_head: MaybeTuple(int) = 32
     ):
         super().__init__()
 
         self.train_as_images = frame_kernel_size == 1
 
         self.skip_scale = skip_scale
         self.channels = channels
@@ -350,65 +358,65 @@
         # number of self attention blocks per stage
 
         num_self_attn_per_stage = cast_tuple(num_self_attn_per_stage, num_resolutions)
         assert all([num_self_attn_blocks >= 0 for num_self_attn_blocks in num_self_attn_per_stage])
 
         # attn kwargs
 
-        attn_kwargs = dict(
-            heads = attn_heads,
-            dim_head = attn_dim_head
-        )
+        attn_heads = cast_tuple(attn_heads, num_resolutions)
+        attn_dim_head = cast_tuple(attn_dim_head, num_resolutions)
 
         # modules for all layers
 
         skip_dims = []
 
         down_stage_parameters = [
             in_out,
             nested_unet_depths,
             num_blocks_per_stage,
-            num_self_attn_per_stage
+            num_self_attn_per_stage,
+            attn_heads,
+            attn_dim_head
         ]
 
         up_stage_parameters = [reversed(params[:-1]) for params in down_stage_parameters]
 
         # downs
 
-        for ind, ((dim_in, dim_out), nested_unet_depth, num_blocks, self_attn_blocks) in enumerate(zip(*down_stage_parameters)):
+        for ind, ((dim_in, dim_out), nested_unet_depth, num_blocks, self_attn_blocks, heads, dim_head) in enumerate(zip(*down_stage_parameters)):
             is_last = ind >= (num_resolutions - 1)
             skip_dims.append(dim_in)
 
             self.downs.append(nn.ModuleList([
                 blocks(dim_in, dim_in, nested_unet_depth = nested_unet_depth, nested_unet_dim = nested_unet_dim),
                 nn.ModuleList([blocks(dim_in, dim_in, nested_unet_depth = nested_unet_depth, nested_unet_dim = nested_unet_dim) for _ in range(num_blocks - 1)]),
-                nn.ModuleList([TransformerBlock(dim_in, depth = self_attn_blocks, **attn_kwargs) for _ in range(self_attn_blocks)]),
+                nn.ModuleList([TransformerBlock(dim_in, depth = self_attn_blocks, heads = heads, dim_head = dim_head) for _ in range(self_attn_blocks)]),
                 Downsample(dim_in, dim_out)
             ]))
 
         # middle
 
         mid_dim = dims[-1]
         mid_nested_unet_depth = nested_unet_depths[-1]
 
         self.mid = blocks(mid_dim, mid_dim, nested_unet_depth = mid_nested_unet_depth, nested_unet_dim = nested_unet_dim)
-        self.mid_attn = Attention(mid_dim)
+        self.mid_attn = Attention(mid_dim, heads = attn_heads[-1], dim_head = attn_dim_head[-1])
         self.mid_after = blocks(mid_dim, mid_dim, nested_unet_depth = mid_nested_unet_depth, nested_unet_dim = nested_unet_dim)
 
         self.mid_upsample = Upsample(mid_dim, dims[-2])
 
         # ups
 
-        for ind, ((dim_in, dim_out), nested_unet_depth, num_blocks, self_attn_blocks) in enumerate(zip(*up_stage_parameters)):
+        for ind, ((dim_in, dim_out), nested_unet_depth, num_blocks, self_attn_blocks, heads, dim_head) in enumerate(zip(*up_stage_parameters)):
             is_last = ind >= (num_resolutions - 1)
 
             self.ups.append(nn.ModuleList([
                 blocks(dim_out + skip_dims.pop(), dim_out, nested_unet_depth = nested_unet_depth, nested_unet_dim = nested_unet_dim),
                 nn.ModuleList([blocks(dim_out, dim_out, nested_unet_depth = nested_unet_depth, nested_unet_dim = nested_unet_dim) for _ in range(num_blocks - 1)]),
-                nn.ModuleList([TransformerBlock(dim_out, depth = self_attn_blocks, **attn_kwargs) for _ in range(self_attn_blocks)]),
+                nn.ModuleList([TransformerBlock(dim_out, depth = self_attn_blocks, heads = heads, dim_head = dim_head) for _ in range(self_attn_blocks)]),
                 Upsample(dim_out, dim_in) if not is_last else nn.Identity()
             ]))
 
 
         out_dim = default(out_dim, channels)
 
         if consolidate_upsample_fmaps:
```

### Comparing `x-unet-0.3.0/x_unet.egg-info/PKG-INFO` & `x-unet-0.3.1/x_unet.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x-unet
-Version: 0.3.0
+Version: 0.3.1
 Summary: X-Unet
 Home-page: https://github.com/lucidrains/x-unet
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,biomedical segmentation,medical deep learning,unets
 Classifier: Development Status :: 4 - Beta
```

