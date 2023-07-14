# Comparing `tmp/LongNet-0.3.7.tar.gz` & `tmp/LongNet-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LongNet-0.3.7.tar", last modified: Wed Jul 12 21:56:59 2023, max compression
+gzip compressed data, was "LongNet-0.3.8.tar", last modified: Fri Jul 14 03:36:57 2023, max compression
```

## Comparing `LongNet-0.3.7.tar` & `LongNet-0.3.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:56:59.763195 LongNet-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 21:56:50.000000 LongNet-0.3.7/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:56:59.763195 LongNet-0.3.7/LongNet/
--rw-r--r--   0 runner    (1001) docker     (123)    13807 2023-07-12 21:56:50.000000 LongNet-0.3.7/LongNet/Transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-12 21:56:50.000000 LongNet-0.3.7/LongNet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-07-12 21:56:50.000000 LongNet-0.3.7/LongNet/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-07-12 21:56:50.000000 LongNet-0.3.7/LongNet/attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:56:59.763195 LongNet-0.3.7/LongNet/iterations/
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-12 21:56:50.000000 LongNet-0.3.7/LongNet/iterations/BlocksparseDilatedAttention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-12 21:56:50.000000 LongNet-0.3.7/LongNet/iterations/DilatedAttentionOP.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-07-12 21:56:50.000000 LongNet-0.3.7/LongNet/iterations/DilatedAttentionOld.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-12 21:56:50.000000 LongNet-0.3.7/LongNet/iterations/DistributedDilatedAttention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-12 21:56:50.000000 LongNet-0.3.7/LongNet/iterations/DynamicDilatedAttention.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-07-12 21:56:50.000000 LongNet-0.3.7/LongNet/iterations/MultiModal.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-12 21:56:50.000000 LongNet-0.3.7/LongNet/iterations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-07-12 21:56:50.000000 LongNet-0.3.7/LongNet/iterations/topk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-07-12 21:56:50.000000 LongNet-0.3.7/LongNet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    23040 2023-07-12 21:56:50.000000 LongNet-0.3.7/LongNet/training.py
--rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-07-12 21:56:50.000000 LongNet-0.3.7/LongNet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:56:59.763195 LongNet-0.3.7/LongNet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-12 21:56:59.000000 LongNet-0.3.7/LongNet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-12 21:56:59.000000 LongNet-0.3.7/LongNet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 21:56:59.000000 LongNet-0.3.7/LongNet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-12 21:56:59.000000 LongNet-0.3.7/LongNet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 21:56:59.000000 LongNet-0.3.7/LongNet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-12 21:56:59.763195 LongNet-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-07-12 21:56:50.000000 LongNet-0.3.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 21:56:59.763195 LongNet-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-12 21:56:50.000000 LongNet-0.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:56:59.763195 LongNet-0.3.7/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-12 21:56:50.000000 LongNet-0.3.7/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:36:57.590338 LongNet-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-14 03:36:46.000000 LongNet-0.3.8/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:36:57.586338 LongNet-0.3.8/LongNet/
+-rw-r--r--   0 runner    (1001) docker     (123)    13807 2023-07-14 03:36:46.000000 LongNet-0.3.8/LongNet/Transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-14 03:36:46.000000 LongNet-0.3.8/LongNet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-07-14 03:36:46.000000 LongNet-0.3.8/LongNet/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-07-14 03:36:46.000000 LongNet-0.3.8/LongNet/attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:36:57.590338 LongNet-0.3.8/LongNet/iterations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-14 03:36:46.000000 LongNet-0.3.8/LongNet/iterations/BlocksparseDilatedAttention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-14 03:36:46.000000 LongNet-0.3.8/LongNet/iterations/DilatedAttentionOP.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-07-14 03:36:46.000000 LongNet-0.3.8/LongNet/iterations/DilatedAttentionOld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-14 03:36:46.000000 LongNet-0.3.8/LongNet/iterations/DistributedDilatedAttention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-14 03:36:46.000000 LongNet-0.3.8/LongNet/iterations/DynamicDilatedAttention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-07-14 03:36:46.000000 LongNet-0.3.8/LongNet/iterations/MultiModal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-14 03:36:46.000000 LongNet-0.3.8/LongNet/iterations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-07-14 03:36:46.000000 LongNet-0.3.8/LongNet/iterations/topk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-07-14 03:36:46.000000 LongNet-0.3.8/LongNet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23040 2023-07-14 03:36:46.000000 LongNet-0.3.8/LongNet/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-07-14 03:36:46.000000 LongNet-0.3.8/LongNet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:36:57.590338 LongNet-0.3.8/LongNet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-14 03:36:57.000000 LongNet-0.3.8/LongNet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-14 03:36:57.000000 LongNet-0.3.8/LongNet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 03:36:57.000000 LongNet-0.3.8/LongNet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-14 03:36:57.000000 LongNet-0.3.8/LongNet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 03:36:57.000000 LongNet-0.3.8/LongNet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-14 03:36:57.590338 LongNet-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-07-14 03:36:46.000000 LongNet-0.3.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 03:36:57.590338 LongNet-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-14 03:36:46.000000 LongNet-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:36:57.590338 LongNet-0.3.8/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-14 03:36:46.000000 LongNet-0.3.8/test/test.py
```

### Comparing `LongNet-0.3.7/LICENSE` & `LongNet-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.7/LongNet/Transformer.py` & `LongNet-0.3.8/LongNet/Transformer.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.7/LongNet/attend.py` & `LongNet-0.3.8/LongNet/attend.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.7/LongNet/attention.py` & `LongNet-0.3.8/LongNet/attention.py`

 * *Files 3% similar despite different names*

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
@@ -30,31 +30,29 @@
         assert isinstance(use_rel_pos_bias, bool), 'use_rel_pos_bias should be a boolean value'
         
         # Initialize parameters
         self.d_model = d_model               # model dimension
         self.num_heads = num_heads           # number of attention heads
         self.dilation_rate = dilation_rate   # dilation rate
         self.segment_size = segment_size     # segment size
-        
         self.dropout = nn.Dropout(dropout)
         # If casual attention is used
         self.casual = casual
         # If using positional encoding
         self.use_xpos = use_xpos
         # If using relative positional bias
         self.use_rel_pos_bias = use_rel_pos_bias
         self.distributed = Distributed
 
+
         # Initialize attention for each head with dilation
-        # Initialize the attention heads with or without DataParallel based on the value of 'distributed'
         if self.distributed:
-            self.attentions = nn.ModuleList([DataParallel(FlashMHA(embed_dim=d_model, num_heads=num_heads, device=device, dtype=dtype)) for _ in range(self.dilation_rate)])
+            self.attentions = nn.ModuleList([DataParallel(FlashAttention(causal=self.casual, dropout=dropout)) for _ in range(self.dilation_rate)])
         else:
-            self.attentions = nn.ModuleList([FlashMHA(embed_dim=d_model, num_heads=num_heads, device=device, dtype=dtype) for _ in range(self.dilation_rate)])
-
+            self.attentions = nn.ModuleList([FlashAttention(causal=self.casual, dropout=dropout) for _ in range(self.dilation_rate)])
 
         # If using positional encoding, initialize it
         if use_xpos:
             self.xpos = XPOS(head_dim=d_model//num_heads)
 
         # If using relative positional bias, initialize it
         if use_rel_pos_bias:
@@ -100,16 +98,14 @@
 
             attn_output = torch.cat(elements_attns, dim=1)
 
 
             #option2
             # elements_attns = [attention(element.to(dtype), element.to(dtype), element.to(dtype)) for element in x_]
             # attn_output = torch.cat(elements_attns, dim=1)
-
-
             
             # If using relative positional bias, add it
             if self.use_rel_pos_bias:
                 attn_output += self.relative_bias(batch_size, attn_output.size(1), attn_output.size(1))
 
             # If using casual attention, apply mask
             if self.casual:
@@ -133,14 +129,19 @@
         outputs_weighted = sum(w * out for w, out in zip(weights, all_head_outputs))
 
         # Return the weighted outputs
         return outputs_weighted
 
 
 
+class MultiHeadDilatedAttention:
+    def __init__():
+        pass
+
+
 
 
 
 
 
 class LongNetTransformer(nn.Module):
     def __init__(self, d_model, num_heads, dilation_rates, segment_sizes):
```

### Comparing `LongNet-0.3.7/LongNet/iterations/BlocksparseDilatedAttention.py` & `LongNet-0.3.8/LongNet/iterations/BlocksparseDilatedAttention.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.7/LongNet/iterations/DilatedAttentionOP.py` & `LongNet-0.3.8/LongNet/iterations/DilatedAttentionOP.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.7/LongNet/iterations/DilatedAttentionOld.py` & `LongNet-0.3.8/LongNet/iterations/DilatedAttentionOld.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.7/LongNet/iterations/DistributedDilatedAttention.py` & `LongNet-0.3.8/LongNet/iterations/DistributedDilatedAttention.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.7/LongNet/iterations/DynamicDilatedAttention.py` & `LongNet-0.3.8/LongNet/iterations/DynamicDilatedAttention.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.7/LongNet/iterations/MultiModal.py` & `LongNet-0.3.8/LongNet/iterations/MultiModal.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.7/LongNet/iterations/topk.py` & `LongNet-0.3.8/LongNet/iterations/topk.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.7/LongNet/model.py` & `LongNet-0.3.8/LongNet/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,12 +87,12 @@
             segment_size = 0,               # segment size for DilatedAttention
             casual = False,                 # whether to use causal attention for DilatedAttention
             use_xpos = False,               # whether to use absolute positional embeddings for DilatedAttention
             use_rel_pos_bias = False,       # whether to use relative positional bias for DilatedAttention
             distributed = False             # whether to distribute attention for DilatedAttention
         )
 
-    def forward(self, text_tokens, temperature: int = None, filter_thres: int = None, **kwargs):
+    def generate(self, text_tokens, temperature: int = None, filter_thres: int = None, **kwargs):
         sampled = self.model.generate(temperature=temperature, filter_thres=filter_thres)
         return sampled
```

### Comparing `LongNet-0.3.7/LongNet/training.py` & `LongNet-0.3.8/LongNet/training.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.7/LongNet/utils.py` & `LongNet-0.3.8/LongNet/utils.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.7/LongNet.egg-info/PKG-INFO` & `LongNet-0.3.8/LongNet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LongNet
-Version: 0.3.7
+Version: 0.3.8
 Summary: LongNet - Pytorch
 Home-page: https://github.com/kyegomez/LongNet
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LongNet-0.3.7/LongNet.egg-info/SOURCES.txt` & `LongNet-0.3.8/LongNet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.7/PKG-INFO` & `LongNet-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LongNet
-Version: 0.3.7
+Version: 0.3.8
 Summary: LongNet - Pytorch
 Home-page: https://github.com/kyegomez/LongNet
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LongNet-0.3.7/README.md` & `LongNet-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `LongNet-0.3.7/setup.py` & `LongNet-0.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 # 
 
 setup(
   name = 'LongNet',
   packages = find_packages(exclude=[]),
-  version = '0.3.7',
+  version = '0.3.8',
   license='MIT',
   description = 'LongNet - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/LongNet',
   keywords = [
```

### Comparing `LongNet-0.3.7/test/test.py` & `LongNet-0.3.8/test/test.py`

 * *Files identical despite different names*

