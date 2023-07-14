# Comparing `tmp/LongNet-0.3.8.tar.gz` & `tmp/LongNet-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LongNet-0.3.8.tar", last modified: Fri Jul 14 03:36:57 2023, max compression
+gzip compressed data, was "LongNet-0.3.9.tar", last modified: Fri Jul 14 19:13:33 2023, max compression
```

## Comparing `LongNet-0.3.8.tar` & `LongNet-0.3.9.tar`

### file list

```diff
@@ -1,31 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:36:57.590338 LongNet-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-14 03:36:46.000000 LongNet-0.3.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:36:57.586338 LongNet-0.3.8/LongNet/
--rw-r--r--   0 runner    (1001) docker     (123)    13807 2023-07-14 03:36:46.000000 LongNet-0.3.8/LongNet/Transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-14 03:36:46.000000 LongNet-0.3.8/LongNet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-07-14 03:36:46.000000 LongNet-0.3.8/LongNet/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-07-14 03:36:46.000000 LongNet-0.3.8/LongNet/attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:36:57.590338 LongNet-0.3.8/LongNet/iterations/
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-14 03:36:46.000000 LongNet-0.3.8/LongNet/iterations/BlocksparseDilatedAttention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-14 03:36:46.000000 LongNet-0.3.8/LongNet/iterations/DilatedAttentionOP.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-07-14 03:36:46.000000 LongNet-0.3.8/LongNet/iterations/DilatedAttentionOld.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-14 03:36:46.000000 LongNet-0.3.8/LongNet/iterations/DistributedDilatedAttention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-14 03:36:46.000000 LongNet-0.3.8/LongNet/iterations/DynamicDilatedAttention.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-07-14 03:36:46.000000 LongNet-0.3.8/LongNet/iterations/MultiModal.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-14 03:36:46.000000 LongNet-0.3.8/LongNet/iterations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-07-14 03:36:46.000000 LongNet-0.3.8/LongNet/iterations/topk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-07-14 03:36:46.000000 LongNet-0.3.8/LongNet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    23040 2023-07-14 03:36:46.000000 LongNet-0.3.8/LongNet/training.py
--rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-07-14 03:36:46.000000 LongNet-0.3.8/LongNet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:36:57.590338 LongNet-0.3.8/LongNet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-14 03:36:57.000000 LongNet-0.3.8/LongNet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-14 03:36:57.000000 LongNet-0.3.8/LongNet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 03:36:57.000000 LongNet-0.3.8/LongNet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-14 03:36:57.000000 LongNet-0.3.8/LongNet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 03:36:57.000000 LongNet-0.3.8/LongNet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-14 03:36:57.590338 LongNet-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-07-14 03:36:46.000000 LongNet-0.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 03:36:57.590338 LongNet-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-14 03:36:46.000000 LongNet-0.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:36:57.590338 LongNet-0.3.8/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-14 03:36:46.000000 LongNet-0.3.8/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.923536 LongNet-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-14 19:13:22.000000 LongNet-0.3.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.907535 LongNet-0.3.9/LongNet/
+-rw-r--r--   0 runner    (1001) docker     (123)    13807 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/Transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.911535 LongNet-0.3.9/LongNet/iterations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/iterations/BlocksparseDilatedAttention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/iterations/DilatedAttentionOP.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/iterations/DilatedAttentionOld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/iterations/DistributedDilatedAttention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/iterations/DynamicDilatedAttention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/iterations/MultiModal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/iterations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/iterations/topk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.911535 LongNet-0.3.9/LongNet/torchscale/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.915536 LongNet-0.3.9/LongNet/torchscale/architecture/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/architecture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/architecture/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15919 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/architecture/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13806 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/architecture/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/architecture/encoder_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/architecture/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.919536 LongNet-0.3.9/LongNet/torchscale/component/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/component/droppath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/component/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/component/feedforward_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/component/multihead_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/component/multiway_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/component/relative_position_bias.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.919536 LongNet-0.3.9/LongNet/torchscale/component/xmoe/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/component/xmoe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/component/xmoe/global_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12079 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/component/xmoe/moe_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18530 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/component/xmoe/routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/component/xpos_relative_position.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.919536 LongNet-0.3.9/LongNet/torchscale/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/model/BEiT3.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/torchscale/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23040 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-07-14 19:13:22.000000 LongNet-0.3.9/LongNet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.911535 LongNet-0.3.9/LongNet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-14 19:13:33.000000 LongNet-0.3.9/LongNet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-14 19:13:33.000000 LongNet-0.3.9/LongNet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 19:13:33.000000 LongNet-0.3.9/LongNet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-14 19:13:33.000000 LongNet-0.3.9/LongNet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 19:13:33.000000 LongNet-0.3.9/LongNet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-14 19:13:33.923536 LongNet-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-07-14 19:13:22.000000 LongNet-0.3.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 19:13:33.923536 LongNet-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-14 19:13:22.000000 LongNet-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.923536 LongNet-0.3.9/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-14 19:13:22.000000 LongNet-0.3.9/test/test.py
```

### Comparing `LongNet-0.3.8/LICENSE` & `LongNet-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.8/LongNet/Transformer.py` & `LongNet-0.3.9/LongNet/Transformer.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.8/LongNet/attend.py` & `LongNet-0.3.9/LongNet/attend.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,15 @@
                 mask = mask & ~causal_mask
                 causal = False
 
         # handle alibi positional bias
         # convert from bool to float
 
         if exists(attn_bias):
-            attn_bias = rearrange(attn_bias, 'h i j -> 1 h i j').expand(batch, -1, -1, -1)
+            attn_bias = rearrange(attn_bias, 'h i j -> 1 h i j').expand(batch, heads, -1, -1)
 
             # if mask given, the mask would already contain the causal mask from above logic
             # otherwise, if no mask given but still causal, mask out alibi positional bias to a large negative number
 
             mask_value = -torch.finfo(q.dtype).max
 
             if exists(mask):
```

### Comparing `LongNet-0.3.8/LongNet/attention.py` & `LongNet-0.3.9/LongNet/attention.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import torch 
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.nn.parallel import DataParallel
 
 from LongNet.utils import XPOS, RelativePositionBias
 
-from LongNet.attend import FlashAttention
+from LongNet.attend import FlashMHA
 
 device = "cuda:0"
 dtype=torch.float16
 
 
 
 # Define the attention module
@@ -30,29 +30,30 @@
         assert isinstance(use_rel_pos_bias, bool), 'use_rel_pos_bias should be a boolean value'
         
         # Initialize parameters
         self.d_model = d_model               # model dimension
         self.num_heads = num_heads           # number of attention heads
         self.dilation_rate = dilation_rate   # dilation rate
         self.segment_size = segment_size     # segment size
+        
         self.dropout = nn.Dropout(dropout)
         # If casual attention is used
         self.casual = casual
         # If using positional encoding
         self.use_xpos = use_xpos
         # If using relative positional bias
         self.use_rel_pos_bias = use_rel_pos_bias
         self.distributed = Distributed
 
-
-        # Initialize attention for each head with dilation
+        # Initialize the attention heads with or without DataParallel based on the value of 'distributed'
         if self.distributed:
-            self.attentions = nn.ModuleList([DataParallel(FlashAttention(causal=self.casual, dropout=dropout)) for _ in range(self.dilation_rate)])
+            self.attentions = nn.ModuleList([DataParallel(FlashMHA(embed_dim=d_model, num_heads=num_heads, device=device, dtype=dtype)) for _ in range(self.dilation_rate)])
         else:
-            self.attentions = nn.ModuleList([FlashAttention(causal=self.casual, dropout=dropout) for _ in range(self.dilation_rate)])
+            self.attentions = nn.ModuleList([FlashMHA(embed_dim=d_model, num_heads=num_heads, device=device, dtype=dtype) for _ in range(self.dilation_rate)])
+
 
         # If using positional encoding, initialize it
         if use_xpos:
             self.xpos = XPOS(head_dim=d_model//num_heads)
 
         # If using relative positional bias, initialize it
         if use_rel_pos_bias:
@@ -98,14 +99,16 @@
 
             attn_output = torch.cat(elements_attns, dim=1)
 
 
             #option2
             # elements_attns = [attention(element.to(dtype), element.to(dtype), element.to(dtype)) for element in x_]
             # attn_output = torch.cat(elements_attns, dim=1)
+
+
             
             # If using relative positional bias, add it
             if self.use_rel_pos_bias:
                 attn_output += self.relative_bias(batch_size, attn_output.size(1), attn_output.size(1))
 
             # If using casual attention, apply mask
             if self.casual:
```

### Comparing `LongNet-0.3.8/LongNet/iterations/BlocksparseDilatedAttention.py` & `LongNet-0.3.9/LongNet/iterations/BlocksparseDilatedAttention.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.8/LongNet/iterations/DilatedAttentionOP.py` & `LongNet-0.3.9/LongNet/iterations/DilatedAttentionOP.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.8/LongNet/iterations/DilatedAttentionOld.py` & `LongNet-0.3.9/LongNet/iterations/DilatedAttentionOld.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import torch 
 import torch.nn as nn
 import torch.nn.functional as F
 
 from LongNet.utils import XPOS, RelativePositionBias
-from LongNet.attention import FlashMHA
+from LongNet.attend import FlashAttention
 
 # Replace this with your correct GPU device
 device = "cuda:0"
 dtype=torch.float16
 
 
 
@@ -41,21 +41,22 @@
         super(DilatedAttentionold, self).__init__()
         self.d_model = d_model
         self.num_heads = num_heads
 
         self.dilation_rate = dilation_rate
         self.segment_size = segment_size
 
-        self.attention = FlashMHA(embed_dim=d_model, num_heads=num_heads, device=device, dtype=dtype)
         self.dropout = nn.Dropout(dropout)
         self.casual = casual
 
         self.use_xpos = use_xpos
         self.use_rel_pos_bias = use_rel_pos_bias
 
+        self.attention = FlashAttention(causal=self.casual, dropout=dropout).to(device)
+
         if use_xpos:
             self.xpos = XPOS(head_dim=d_model//num_heads)
         if use_rel_pos_bias:
             self.relative_bias = RelativePositionBias(num_buckets=32, max_distance=128, n_heads=num_heads)
 
         #head offsets
         self.head_offsets = nn.Parameter(torch.randn(num_heads, d_model))
@@ -70,24 +71,24 @@
             x = self.xpos(x)
         
         # Split and sparsify
         x = x.view(batch_size, -1, self.segment_size, self.d_model)
         x = x[:, :, :: self.dilation_rate, :]
 
         # Perform attention
-        attn_output, _ = self.attention(x, x, x)
+        attn_output = self.attention(x, x, x)
 
         #if use rel pos => apply relative positioning bias 
         if self.use_rel_pos_bias:
             attn_output += self.relative_bias(batch_size, attn_output.size(1), attn_output.size(1))
 
         # if casual create a mask and apply to the output
         if self.casual:
             mask = self.get_mask(attn_output.size(1), attn_output.size(1))
             attn_output = attn_output.masked_fill(mask, float('-inf'))
 
         # apply dropout
         attn_output = self.dropout(attn_output)
 
         # Scatter and concatenate 
-        attn_output = attn_output.view(batch_size, -1, self.d_model)
+        attn_output = attn_output.reshape(batch_size, -1, self.d_model)
         return attn_output
```

### Comparing `LongNet-0.3.8/LongNet/iterations/DistributedDilatedAttention.py` & `LongNet-0.3.9/LongNet/iterations/DistributedDilatedAttention.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.8/LongNet/iterations/DynamicDilatedAttention.py` & `LongNet-0.3.9/LongNet/iterations/DynamicDilatedAttention.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.8/LongNet/iterations/MultiModal.py` & `LongNet-0.3.9/LongNet/iterations/MultiModal.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.8/LongNet/iterations/topk.py` & `LongNet-0.3.9/LongNet/iterations/topk.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.8/LongNet/model.py` & `LongNet-0.3.9/LongNet/model.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.8/LongNet/training.py` & `LongNet-0.3.9/LongNet/training.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.8/LongNet/utils.py` & `LongNet-0.3.9/LongNet/utils.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.8/LongNet.egg-info/PKG-INFO` & `LongNet-0.3.9/LongNet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LongNet
-Version: 0.3.8
+Version: 0.3.9
 Summary: LongNet - Pytorch
 Home-page: https://github.com/kyegomez/LongNet
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LongNet-0.3.8/PKG-INFO` & `LongNet-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LongNet
-Version: 0.3.8
+Version: 0.3.9
 Summary: LongNet - Pytorch
 Home-page: https://github.com/kyegomez/LongNet
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LongNet-0.3.8/README.md` & `LongNet-0.3.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 3. Its dilated attention is a drop-in replacement for standard attention, which can be seamlessly integrated with the existing Transformer-based optimization.
 
 Experiment results demonstrate that LongNet yields strong performance on both long-sequence modeling and general language tasks. Their work opens up new possibilities for modeling very long sequences, e.g., treating a whole corpus or even the entire Internet as a sequence.
 
 Here's the updated usage and installation section with two methods: git clone or pip install LongNet:
 
 ## Installation
-c
+
 You can install LongNet using one of the following methods:
 
 ### Method 1: Git Clone
 
 1. Clone the LongNet repository from GitHub:
 
 ```shell
@@ -37,27 +37,15 @@
 
 2. Navigate to the cloned directory:
 
 ```shell
 cd LongNet
 ```
 
-3. Prepare `flash_attn` library
-
-```bash
-
-cd flash_attn
-
-python setup.py install
-
-cd ..
-
-```
-
-4. Install the required dependencies:
+3. Install the required dependencies:
 
 ```shell
 pip install -r requirements.txt
 ```
 
 
 ### Method 2: Pip Install
@@ -107,16 +95,20 @@
 # Forward pass
 outputs = attention(inputs)
 
 # Print the output shape
 print(outputs.shape)  # Expected: [batch_size, seq_len, d_model]
 ```
 
+# Documentation
+
+* [Click here for the model documentation](docs/DOCUMENTATION.md)
+
 # Training the Model
-There are 2 methods, one is `accelerate` and the other `from LongNet import Train`
+* We're still working on the model configuation as closely in the paper as possible. There are 2 methods, one is `accelerate` and the other `from LongNet import Train`
 
 ### Method 1 
 
 * Git clone installation
 
 * Init your parameters `accelerate config`
```

### Comparing `LongNet-0.3.8/setup.py` & `LongNet-0.3.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 # 
 
 setup(
   name = 'LongNet',
   packages = find_packages(exclude=[]),
-  version = '0.3.8',
+  version = '0.3.9',
   license='MIT',
   description = 'LongNet - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/LongNet',
   keywords = [
@@ -23,14 +23,15 @@
         'torchscale',
         'transformers',
         'accelerate',
         'bitsandbytes',
         'fairscale',
         'timm',
         'dataclasses',
+        'beartype'
     ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.6',
```

### Comparing `LongNet-0.3.8/test/test.py` & `LongNet-0.3.9/test/test.py`

 * *Files identical despite different names*

