# Comparing `tmp/LongNet-0.3.9.tar.gz` & `tmp/LongNet-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LongNet-0.3.9.tar", last modified: Fri Jul 14 19:13:33 2023, max compression
+gzip compressed data, was "LongNet-0.4.0.tar", last modified: Fri Jul 14 20:16:25 2023, max compression
```

## Comparing `LongNet-0.3.9.tar` & `LongNet-0.4.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.923536 LongNet-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-14 19:13:22.000000 LongNet-0.3.9/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.907535 LongNet-0.3.9/LongNet/
--rw-r--r--   0 runner    (1001) docker     (123)    13807 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/Transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.911535 LongNet-0.3.9/LongNet/iterations/
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/iterations/BlocksparseDilatedAttention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/iterations/DilatedAttentionOP.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/iterations/DilatedAttentionOld.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/iterations/DistributedDilatedAttention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/iterations/DynamicDilatedAttention.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/iterations/MultiModal.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/iterations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/iterations/topk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.911535 LongNet-0.3.9/LongNet/torchscale/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.915536 LongNet-0.3.9/LongNet/torchscale/architecture/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/architecture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/architecture/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    15919 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/architecture/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    13806 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/architecture/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/architecture/encoder_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/architecture/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.919536 LongNet-0.3.9/LongNet/torchscale/component/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/component/droppath.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/component/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/component/feedforward_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/component/multihead_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/component/multiway_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/component/relative_position_bias.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.919536 LongNet-0.3.9/LongNet/torchscale/component/xmoe/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/component/xmoe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/component/xmoe/global_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    12079 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/component/xmoe/moe_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18530 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/component/xmoe/routing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/component/xpos_relative_position.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.919536 LongNet-0.3.9/LongNet/torchscale/model/
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/model/BEiT3.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23040 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/training.py
--rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.911535 LongNet-0.3.9/LongNet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-14 19:13:33.000000 LongNet-0.3.9/LongNet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-14 19:13:33.000000 LongNet-0.3.9/LongNet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 19:13:33.000000 LongNet-0.3.9/LongNet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-14 19:13:33.000000 LongNet-0.3.9/LongNet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 19:13:33.000000 LongNet-0.3.9/LongNet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-14 19:13:33.923536 LongNet-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-07-14 19:13:22.000000 LongNet-0.3.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 19:13:33.923536 LongNet-0.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-14 19:13:22.000000 LongNet-0.3.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.923536 LongNet-0.3.9/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-14 19:13:22.000000 LongNet-0.3.9/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:16:25.610744 LongNet-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-14 20:16:14.000000 LongNet-0.4.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:16:25.602744 LongNet-0.4.0/LongNet/
+-rw-r--r--   0 runner    (1001) docker     (123)    13807 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/Transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:16:25.606744 LongNet-0.4.0/LongNet/iterations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/iterations/BlocksparseDilatedAttention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/iterations/DilatedAttentionOP.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/iterations/DilatedAttentionOld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/iterations/DistributedDilatedAttention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/iterations/DynamicDilatedAttention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/iterations/MultiModal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/iterations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/iterations/topk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:16:25.606744 LongNet-0.4.0/LongNet/torchscale/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:16:25.606744 LongNet-0.4.0/LongNet/torchscale/architecture/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/architecture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/architecture/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15919 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/architecture/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13806 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/architecture/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/architecture/encoder_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/architecture/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:16:25.610744 LongNet-0.4.0/LongNet/torchscale/component/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/component/droppath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/component/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/component/feedforward_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/component/multihead_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/component/multiway_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/component/relative_position_bias.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:16:25.610744 LongNet-0.4.0/LongNet/torchscale/component/xmoe/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/component/xmoe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/component/xmoe/global_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12079 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/component/xmoe/moe_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18530 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/component/xmoe/routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/component/xpos_relative_position.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:16:25.610744 LongNet-0.4.0/LongNet/torchscale/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/model/BEiT3.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23040 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:16:25.602744 LongNet-0.4.0/LongNet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-14 20:16:25.000000 LongNet-0.4.0/LongNet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-14 20:16:25.000000 LongNet-0.4.0/LongNet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 20:16:25.000000 LongNet-0.4.0/LongNet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-14 20:16:25.000000 LongNet-0.4.0/LongNet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 20:16:25.000000 LongNet-0.4.0/LongNet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-14 20:16:25.610744 LongNet-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-07-14 20:16:14.000000 LongNet-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 20:16:25.610744 LongNet-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-14 20:16:14.000000 LongNet-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:16:25.610744 LongNet-0.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-14 20:16:14.000000 LongNet-0.4.0/test/test.py
```

### Comparing `LongNet-0.3.9/LICENSE` & `LongNet-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.9/LongNet/Transformer.py` & `LongNet-0.4.0/LongNet/Transformer.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.9/LongNet/attend.py` & `LongNet-0.4.0/LongNet/attend.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.9/LongNet/attention.py` & `LongNet-0.4.0/LongNet/attention.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import torch 
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.nn.parallel import DataParallel
 
 from LongNet.utils import XPOS, RelativePositionBias
 
-from LongNet.attend import FlashMHA
+from LongNet.attend import FlashAttention
 
 device = "cuda:0"
 dtype=torch.float16
 
 
 
 # Define the attention module
@@ -42,17 +42,17 @@
         self.use_xpos = use_xpos
         # If using relative positional bias
         self.use_rel_pos_bias = use_rel_pos_bias
         self.distributed = Distributed
 
         # Initialize the attention heads with or without DataParallel based on the value of 'distributed'
         if self.distributed:
-            self.attentions = nn.ModuleList([DataParallel(FlashMHA(embed_dim=d_model, num_heads=num_heads, device=device, dtype=dtype)) for _ in range(self.dilation_rate)])
+            self.attentions = nn.ModuleList([DataParallel(FlashAttention(causal=self.casual, dropout=dropout).to(device)) for _ in range(self.dilation_rate)])
         else:
-            self.attentions = nn.ModuleList([FlashMHA(embed_dim=d_model, num_heads=num_heads, device=device, dtype=dtype) for _ in range(self.dilation_rate)])
+            self.attentions = nn.ModuleList([FlashAttention(causal=self.casual, dropout=dropout).to(device) for _ in range(self.dilation_rate)])
 
 
         # If using positional encoding, initialize it
         if use_xpos:
             self.xpos = XPOS(head_dim=d_model//num_heads)
 
         # If using relative positional bias, initialize it
@@ -63,15 +63,14 @@
         self.softmax = nn.Softmax(dim=-1)
 
     # Function to get mask for casual attention
     def get_mask(self, i, j):
         return torch.ones((i, j), device=device, dtype=torch.bool).triu(j - i + 2)
 
 
-    # Forward function
     def forward(self, x):
         # Get batch size, sequence length and model dimension
         batch_size, seq_len, _ = x.shape
 
         # If using positional encoding, add it
         if self.use_xpos:
             x = self.xpos(x)
@@ -82,26 +81,25 @@
         # For each attention head
         for head_idx, attention in enumerate(self.attentions):
             # Calculate offset for this head
             offset = head_idx % self.dilation_rate
 
             # Apply offset and segment for this head
             x_ = x[:, offset::self.dilation_rate, :]
-            x_ = x_.contiguous().view(batch_size, -1, self.segment_size, self.d_model)
-            
+            x_ = x_.contiguous().view(batch_size, 1, -1, self.segment_size, self.d_model)  # Add an extra dimension for the number of heads
 
-            
+            # Process each segment separately
             elements_attns = []
-            for idx in range(x_.shape[1]):
-                element      = x_[:, idx, :, :].to(dtype)
+            for idx in range(x_.shape[2]):
+                element = x_[:, :, idx, :, :].to(dtype)
                 element_attn = attention(element, element, element)
-
                 elements_attns.append(element_attn)
 
-            attn_output = torch.cat(elements_attns, dim=1)
+            attn_output = torch.cat(elements_attns, dim=2)
+
 
 
             #option2
             # elements_attns = [attention(element.to(dtype), element.to(dtype), element.to(dtype)) for element in x_]
             # attn_output = torch.cat(elements_attns, dim=1)
```

### Comparing `LongNet-0.3.9/LongNet/iterations/BlocksparseDilatedAttention.py` & `LongNet-0.4.0/LongNet/iterations/BlocksparseDilatedAttention.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch 
 import torch.nn as nn
 import torch.nn.functional as F
 
 from LongNet.utils import XPOS, RelativePositionBias
-from LongNet.attention import FlashMHA
+from LongNet.attend import FlashMHA
 
 # Replace this with your correct GPU device
 device = "cuda:0"
 dtype=torch.float16
```

### Comparing `LongNet-0.3.9/LongNet/iterations/DilatedAttentionOP.py` & `LongNet-0.4.0/LongNet/iterations/DilatedAttentionOP.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import torch 
 import torch.nn as nn
 import torch.nn.functional as F
 
 from LongNet.utils import XPOS, RelativePositionBias
-from LongNet.attention import FlashMHA
+from LongNet.attend import FlashMHA
 
 # Replace this with your correct GPU device
 device = "cuda:0"
 dtype=torch.float16
```

### Comparing `LongNet-0.3.9/LongNet/iterations/DilatedAttentionOld.py` & `LongNet-0.4.0/LongNet/iterations/DilatedAttentionOld.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.9/LongNet/iterations/DistributedDilatedAttention.py` & `LongNet-0.4.0/LongNet/iterations/DistributedDilatedAttention.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #distributed dilated attention based on second iteration
 import torch.distributed as dist
 import torch 
 import torch.nn as nn
 import torch.nn.functional as F
 
 from LongNet.utils import XPOS, RelativePositionBias
-from LongNet.attention import FlashMHA
+from LongNet.attend import FlashMHA
 
 # Replace this with your correct GPU device
 device = "cuda:0"
 dtype=torch.float16
```

### Comparing `LongNet-0.3.9/LongNet/iterations/DynamicDilatedAttention.py` & `LongNet-0.4.0/LongNet/iterations/DynamicDilatedAttention.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import torch 
 import torch.nn as nn
 import torch.nn.functional as F
 
 from LongNet.utils import XPOS, RelativePositionBias
-from LongNet.attention import FlashMHA
+from LongNet.attend import FlashAttention
 
 # Replace this with your correct GPU device
 device = "cuda:0"
 dtype=torch.float16
 
 
 
 
 class DynamicDilatedAttention(nn.Module):
     def __init__(self, d_model, num_heads, num_rates, dropout=0.0, casual=False, use_xpos=False, use_rel_pos_bias=False):
         super(DynamicDilatedAttention, self).__init__()
         self.d_model = d_model
         self.num_heads = num_heads
+        self.casual = casual  # Define this before FlashAttention
 
         # Generate geometric sequences for dilation rates and segment sizes
         self.dilation_rates = torch.logspace(start=0, end=num_rates-1, steps=num_rates, base=2, dtype=torch.int, device=device)
         self.segment_sizes = torch.logspace(start=0, end=num_rates-1, steps=num_rates, base=2, dtype=torch.int, device=device)
 
-        self.attentions = nn.ModuleList([FlashMHA(embed_dim=d_model, num_heads=num_heads, device=device, dtype=dtype) for _ in range(num_rates)])
+        self.attention = [FlashAttention(causal=self.casual, dropout=dropout).to(device) for _ in range(num_rates)] # Corrected here]
         self.dropout = nn.Dropout(dropout)
-        self.casual = casual
 
         self.use_xpos = use_xpos
         self.use_rel_pos_bias = use_rel_pos_bias
 
         if use_xpos:
             self.xpos = XPOS(head_dim=d_model//num_heads)
         if use_rel_pos_bias:
@@ -41,47 +41,47 @@
 
     def forward(self, x):
         batch_size, seq_len, _ = x.shape
 
         if self.use_xpos:
             x = self.xpos(x)
 
-        #collect outputs from each attention head
-        all_head_outputs = []
-        all_softmax_denominators = []
-        for head_idx, attention in enumerate(self.attentions):
+        # Initialize tensor to store outputs
+        outputs = torch.zeros((batch_size, seq_len, self.d_model), device=device, dtype=dtype)
+
+        # Initialize tensor to store softmax denominators
+        softmax_denominators = torch.zeros((batch_size, seq_len, self.num_heads), device=device, dtype=dtype)
+
+        for head_idx, attention in enumerate(self.attention):
             dilation_rate = self.dilation_rates[head_idx]
             segment_size = self.segment_sizes[head_idx]
 
             for offset in range(dilation_rate):
                 x_ = x[:, offset::dilation_rate, :]  # Apply offset for each head
                 x_ = x_.contiguous().view(batch_size, -1, segment_size, self.d_model)
 
-                attn_output, attn_weights = attention(x_, x_, x_)
+                attn_output, attn_weights, *_ = attention(x_, x_, x_)  # Collect all additional return values into a list
+                
                 if self.use_rel_pos_bias:
                     attn_output += self.relative_bias(batch_size, attn_output.size(1), attn_output.size(1))
 
                 if self.casual:
                     mask = self.get_mask(attn_output.size(1), attn_output.size(1))
                     attn_output = attn_output.masked_fill(mask, float('-inf'))
 
                 attn_output = self.dropout(attn_output)
 
-                #resize back to original size
-                attn_output_resized = torch.zeros((batch_size, seq_len, self.d_model), device=device, dtype=dtype)
-                attn_output_resized[:, offset::dilation_rate, :] = attn_output.contiguous().view(batch_size, -1, self.d_model)
+                # Add output to the corresponding positions in the outputs tensor
+                outputs[:, offset::dilation_rate, :] += attn_output.contiguous().view(batch_size, -1, self.d_model)
                 
-                all_head_outputs.append(attn_output_resized)
-                all_softmax_denominators.append(attn_weights.sum(dim=-1))
+                # Add softmax denominators to the corresponding positions in the softmax_denominators tensor
+                softmax_denominators[:, offset::dilation_rate, :] += attn_weights.sum(dim=-1)
 
-        #calculate the weights for the different dilated attentions
-        weights = self.softmax(torch.stack(all_softmax_denominators, dim=-1))
+        # Calculate the weights for the different dilated attentions
+        weights = self.softmax(softmax_denominators)
 
-        #apply the weights to the outputs of the different heads
-        outputs_weighted = sum(w.unsqueeze(-1) * out for w, out in zip(weights, all_head_outputs))
+        # Apply the weights to the outputs
+        outputs_weighted = weights * outputs
 
         return outputs_weighted
 
 
-
-
-
```

### Comparing `LongNet-0.3.9/LongNet/iterations/MultiModal.py` & `LongNet-0.4.0/LongNet/iterations/MultiModal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch 
 import torch.nn as nn
 import torch.nn.functional as F
 
 from LongNet.utils import XPOS, RelativePositionBias
-from LongNet.attention import FlashMHA
+from LongNet.attend import FlashMHA
 
 device = "cuda:0"
 dtype=torch.float16
 
 
 #second iteration the weighted sum of the different dilated + offsets for the different heads
 class DilatedAttention(nn.Module):
```

### Comparing `LongNet-0.3.9/LongNet/iterations/topk.py` & `LongNet-0.4.0/LongNet/iterations/topk.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch 
 import torch.nn as nn
 import torch.nn.functional as F
 
 from LongNet.utils import XPOS, RelativePositionBias
-from LongNet.attention import FlashMHA
+from LongNet.attend import FlashMHA
 
 
 # Replace this with your correct GPU device
 device = "cuda:0"
 dtype=torch.float16
```

### Comparing `LongNet-0.3.9/LongNet/model.py` & `LongNet-0.4.0/LongNet/model.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.9/LongNet/torchscale/architecture/config.py` & `LongNet-0.4.0/LongNet/torchscale/architecture/config.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.9/LongNet/torchscale/architecture/decoder.py` & `LongNet-0.4.0/LongNet/torchscale/architecture/decoder.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.9/LongNet/torchscale/architecture/encoder.py` & `LongNet-0.4.0/LongNet/torchscale/architecture/encoder.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.9/LongNet/torchscale/architecture/encoder_decoder.py` & `LongNet-0.4.0/LongNet/torchscale/architecture/encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.9/LongNet/torchscale/architecture/utils.py` & `LongNet-0.4.0/LongNet/torchscale/architecture/utils.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.9/LongNet/torchscale/component/droppath.py` & `LongNet-0.4.0/LongNet/torchscale/component/droppath.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.9/LongNet/torchscale/component/embedding.py` & `LongNet-0.4.0/LongNet/torchscale/component/embedding.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.9/LongNet/torchscale/component/feedforward_network.py` & `LongNet-0.4.0/LongNet/torchscale/component/feedforward_network.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.9/LongNet/torchscale/component/multihead_attention.py` & `LongNet-0.4.0/LongNet/torchscale/component/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.9/LongNet/torchscale/component/multiway_network.py` & `LongNet-0.4.0/LongNet/torchscale/component/multiway_network.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.9/LongNet/torchscale/component/relative_position_bias.py` & `LongNet-0.4.0/LongNet/torchscale/component/relative_position_bias.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.9/LongNet/torchscale/component/xmoe/global_groups.py` & `LongNet-0.4.0/LongNet/torchscale/component/xmoe/global_groups.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.9/LongNet/torchscale/component/xmoe/moe_layer.py` & `LongNet-0.4.0/LongNet/torchscale/component/xmoe/moe_layer.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.9/LongNet/torchscale/component/xmoe/routing.py` & `LongNet-0.4.0/LongNet/torchscale/component/xmoe/routing.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.9/LongNet/torchscale/component/xpos_relative_position.py` & `LongNet-0.4.0/LongNet/torchscale/component/xpos_relative_position.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.9/LongNet/torchscale/model/BEiT3.py` & `LongNet-0.4.0/LongNet/torchscale/model/BEiT3.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.9/LongNet/training.py` & `LongNet-0.4.0/LongNet/training.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.9/LongNet/utils.py` & `LongNet-0.4.0/LongNet/utils.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.9/LongNet.egg-info/PKG-INFO` & `LongNet-0.4.0/LongNet.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LongNet
-Version: 0.3.9
+Version: 0.4.0
 Summary: LongNet - Pytorch
 Home-page: https://github.com/kyegomez/LongNet
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LongNet-0.3.9/LongNet.egg-info/SOURCES.txt` & `LongNet-0.4.0/LongNet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.9/PKG-INFO` & `LongNet-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LongNet
-Version: 0.3.9
+Version: 0.4.0
 Summary: LongNet - Pytorch
 Home-page: https://github.com/kyegomez/LongNet
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LongNet-0.3.9/README.md` & `LongNet-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.9/setup.py` & `LongNet-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 # 
 
 setup(
   name = 'LongNet',
   packages = find_packages(exclude=[]),
-  version = '0.3.9',
+  version = '0.4.0',
   license='MIT',
   description = 'LongNet - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/LongNet',
   keywords = [
```

### Comparing `LongNet-0.3.9/test/test.py` & `LongNet-0.4.0/test/test.py`

 * *Files identical despite different names*

