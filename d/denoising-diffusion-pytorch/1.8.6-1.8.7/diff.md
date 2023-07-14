# Comparing `tmp/denoising-diffusion-pytorch-1.8.6.tar.gz` & `tmp/denoising-diffusion-pytorch-1.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denoising-diffusion-pytorch-1.8.6.tar", last modified: Thu Jul 13 14:45:22 2023, max compression
+gzip compressed data, was "denoising-diffusion-pytorch-1.8.7.tar", last modified: Fri Jul 14 14:14:41 2023, max compression
```

## Comparing `denoising-diffusion-pytorch-1.8.6.tar` & `denoising-diffusion-pytorch-1.8.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:45:22.221145 denoising-diffusion-pytorch-1.8.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-13 14:45:06.000000 denoising-diffusion-pytorch-1.8.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-13 14:45:22.221145 denoising-diffusion-pytorch-1.8.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-07-13 14:45:06.000000 denoising-diffusion-pytorch-1.8.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:45:22.217145 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-13 14:45:06.000000 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-13 14:45:06.000000 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    27920 2023-07-13 14:45:06.000000 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/classifier_free_guidance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-07-13 14:45:06.000000 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    36981 2023-07-13 14:45:06.000000 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    30027 2023-07-13 14:45:06.000000 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-07-13 14:45:06.000000 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/elucidated_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-13 14:45:06.000000 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/fid_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    35629 2023-07-13 14:45:06.000000 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/guided_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-07-13 14:45:06.000000 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    21236 2023-07-13 14:45:06.000000 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/simple_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-07-13 14:45:06.000000 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 14:45:06.000000 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-13 14:45:06.000000 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:45:22.221145 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-13 14:45:22.000000 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-13 14:45:22.000000 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 14:45:22.000000 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-13 14:45:22.000000 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-13 14:45:22.000000 denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 14:45:22.221145 denoising-diffusion-pytorch-1.8.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-13 14:45:06.000000 denoising-diffusion-pytorch-1.8.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:14:41.844280 denoising-diffusion-pytorch-1.8.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-14 14:14:32.000000 denoising-diffusion-pytorch-1.8.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-14 14:14:41.844280 denoising-diffusion-pytorch-1.8.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-07-14 14:14:32.000000 denoising-diffusion-pytorch-1.8.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:14:41.844280 denoising-diffusion-pytorch-1.8.7/denoising_diffusion_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-14 14:14:32.000000 denoising-diffusion-pytorch-1.8.7/denoising_diffusion_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-14 14:14:32.000000 denoising-diffusion-pytorch-1.8.7/denoising_diffusion_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27920 2023-07-14 14:14:32.000000 denoising-diffusion-pytorch-1.8.7/denoising_diffusion_pytorch/classifier_free_guidance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-07-14 14:14:32.000000 denoising-diffusion-pytorch-1.8.7/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37278 2023-07-14 14:14:32.000000 denoising-diffusion-pytorch-1.8.7/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30027 2023-07-14 14:14:32.000000 denoising-diffusion-pytorch-1.8.7/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-07-14 14:14:32.000000 denoising-diffusion-pytorch-1.8.7/denoising_diffusion_pytorch/elucidated_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-14 14:14:32.000000 denoising-diffusion-pytorch-1.8.7/denoising_diffusion_pytorch/fid_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35629 2023-07-14 14:14:32.000000 denoising-diffusion-pytorch-1.8.7/denoising_diffusion_pytorch/guided_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-07-14 14:14:32.000000 denoising-diffusion-pytorch-1.8.7/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21236 2023-07-14 14:14:32.000000 denoising-diffusion-pytorch-1.8.7/denoising_diffusion_pytorch/simple_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-07-14 14:14:32.000000 denoising-diffusion-pytorch-1.8.7/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 14:14:32.000000 denoising-diffusion-pytorch-1.8.7/denoising_diffusion_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-14 14:14:32.000000 denoising-diffusion-pytorch-1.8.7/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:14:41.844280 denoising-diffusion-pytorch-1.8.7/denoising_diffusion_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-14 14:14:41.000000 denoising-diffusion-pytorch-1.8.7/denoising_diffusion_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-14 14:14:41.000000 denoising-diffusion-pytorch-1.8.7/denoising_diffusion_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 14:14:41.000000 denoising-diffusion-pytorch-1.8.7/denoising_diffusion_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-14 14:14:41.000000 denoising-diffusion-pytorch-1.8.7/denoising_diffusion_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-14 14:14:41.000000 denoising-diffusion-pytorch-1.8.7/denoising_diffusion_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 14:14:41.844280 denoising-diffusion-pytorch-1.8.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-14 14:14:32.000000 denoising-diffusion-pytorch-1.8.7/setup.py
```

### Comparing `denoising-diffusion-pytorch-1.8.6/LICENSE` & `denoising-diffusion-pytorch-1.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.6/PKG-INFO` & `denoising-diffusion-pytorch-1.8.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.8.6
+Version: 1.8.7
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.8.6/README.md` & `denoising-diffusion-pytorch-1.8.7/README.md`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/__init__.py` & `denoising-diffusion-pytorch-1.8.7/denoising_diffusion_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/attend.py` & `denoising-diffusion-pytorch-1.8.7/denoising_diffusion_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/classifier_free_guidance.py` & `denoising-diffusion-pytorch-1.8.7/denoising_diffusion_pytorch/classifier_free_guidance.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.8.7/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py` & `denoising-diffusion-pytorch-1.8.7/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,51 +310,55 @@
             nn.Linear(fourier_dim, time_dim),
             nn.GELU(),
             nn.Linear(time_dim, time_dim)
         )
 
         # attention
 
-        full_attn = cast_tuple(full_attn, length = len(dim_mults))
+        num_stages = len(dim_mults)
+        full_attn  = cast_tuple(full_attn, num_stages)
+        attn_heads = cast_tuple(attn_heads, num_stages)
+        attn_dim_head = cast_tuple(attn_dim_head, num_stages)
+
         assert len(full_attn) == len(dim_mults)
 
         FullAttention = partial(Attention, flash = flash_attn)
 
         # layers
 
         self.downs = nn.ModuleList([])
         self.ups = nn.ModuleList([])
         num_resolutions = len(in_out)
 
-        for ind, ((dim_in, dim_out), layer_full_attn) in enumerate(zip(in_out, full_attn)):
+        for ind, ((dim_in, dim_out), layer_full_attn, layer_attn_heads, layer_attn_dim_head) in enumerate(zip(in_out, full_attn, attn_heads, attn_dim_head)):
             is_last = ind >= (num_resolutions - 1)
 
             attn_klass = FullAttention if layer_full_attn else LinearAttention
 
             self.downs.append(nn.ModuleList([
                 block_klass(dim_in, dim_in, time_emb_dim = time_dim),
                 block_klass(dim_in, dim_in, time_emb_dim = time_dim),
-                attn_klass(dim_in, dim_head = attn_dim_head, heads = attn_heads),
+                attn_klass(dim_in, dim_head = layer_attn_dim_head, heads = layer_attn_heads),
                 Downsample(dim_in, dim_out) if not is_last else nn.Conv2d(dim_in, dim_out, 3, padding = 1)
             ]))
 
         mid_dim = dims[-1]
         self.mid_block1 = block_klass(mid_dim, mid_dim, time_emb_dim = time_dim)
         self.mid_attn = FullAttention(mid_dim)
         self.mid_block2 = block_klass(mid_dim, mid_dim, time_emb_dim = time_dim)
 
-        for ind, ((dim_in, dim_out), layer_full_attn) in enumerate(zip(reversed(in_out), reversed(full_attn))):
+        for ind, ((dim_in, dim_out), layer_full_attn, layer_attn_heads, layer_attn_dim_head) in enumerate(zip(*map(reversed, (in_out, full_attn, attn_heads, attn_dim_head)))):
             is_last = ind == (len(in_out) - 1)
 
             attn_klass = FullAttention if layer_full_attn else LinearAttention
 
             self.ups.append(nn.ModuleList([
                 block_klass(dim_out + dim_in, dim_out, time_emb_dim = time_dim),
                 block_klass(dim_out + dim_in, dim_out, time_emb_dim = time_dim),
-                attn_klass(dim_out, dim_head = attn_dim_head, heads = attn_heads),
+                attn_klass(dim_out, dim_head = layer_attn_dim_head, heads = layer_attn_heads),
                 Upsample(dim_out, dim_in) if not is_last else  nn.Conv2d(dim_out, dim_in, 3, padding = 1)
             ]))
 
         default_out_dim = channels * (1 if not learned_variance else 2)
         self.out_dim = default(out_dim, default_out_dim)
 
         self.final_res_block = block_klass(dim * 2, dim, time_emb_dim = time_dim)
```

### Comparing `denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py` & `denoising-diffusion-pytorch-1.8.7/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/elucidated_diffusion.py` & `denoising-diffusion-pytorch-1.8.7/denoising_diffusion_pytorch/elucidated_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/fid_evaluation.py` & `denoising-diffusion-pytorch-1.8.7/denoising_diffusion_pytorch/fid_evaluation.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/guided_diffusion.py` & `denoising-diffusion-pytorch-1.8.7/denoising_diffusion_pytorch/guided_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/learned_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.8.7/denoising_diffusion_pytorch/learned_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/simple_diffusion.py` & `denoising-diffusion-pytorch-1.8.7/denoising_diffusion_pytorch/simple_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.8.7/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.8.7/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch.egg-info/PKG-INFO` & `denoising-diffusion-pytorch-1.8.7/denoising_diffusion_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.8.6
+Version: 1.8.7
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.8.6/denoising_diffusion_pytorch.egg-info/SOURCES.txt` & `denoising-diffusion-pytorch-1.8.7/denoising_diffusion_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.6/setup.py` & `denoising-diffusion-pytorch-1.8.7/setup.py`

 * *Files identical despite different names*

