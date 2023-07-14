# Comparing `tmp/apple-upscale-0.1.0.tar.gz` & `tmp/apple-upscale-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apple-upscale-0.1.0.tar", last modified: Wed Jul 12 22:47:52 2023, max compression
+gzip compressed data, was "apple-upscale-0.1.1.tar", last modified: Fri Jul 14 21:57:35 2023, max compression
```

## Comparing `apple-upscale-0.1.0.tar` & `apple-upscale-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 alvinwan   (501) staff       (20)        0 2023-07-12 22:47:52.697007 apple-upscale-0.1.0/
--rw-r--r--   0 alvinwan   (501) staff       (20)     2316 2023-06-16 03:39:27.000000 apple-upscale-0.1.0/LICENSE
--rw-r--r--   0 alvinwan   (501) staff       (20)     8550 2023-07-12 22:47:52.696812 apple-upscale-0.1.0/PKG-INFO
--rw-r--r--   0 alvinwan   (501) staff       (20)     4847 2023-07-12 22:45:57.000000 apple-upscale-0.1.0/README.md
--rw-r--r--   0 alvinwan   (501) staff       (20)     1508 2023-07-12 22:42:30.000000 apple-upscale-0.1.0/pyproject.toml
--rw-r--r--   0 alvinwan   (501) staff       (20)       38 2023-07-12 22:47:52.697058 apple-upscale-0.1.0/setup.cfg
-drwxr-xr-x   0 alvinwan   (501) staff       (20)        0 2023-07-12 22:47:52.692726 apple-upscale-0.1.0/src/
-drwxr-xr-x   0 alvinwan   (501) staff       (20)        0 2023-07-12 22:47:52.694165 apple-upscale-0.1.0/src/apple_upscale.egg-info/
--rw-r--r--   0 alvinwan   (501) staff       (20)     8550 2023-07-12 22:47:52.000000 apple-upscale-0.1.0/src/apple_upscale.egg-info/PKG-INFO
--rw-r--r--   0 alvinwan   (501) staff       (20)      642 2023-07-12 22:47:52.000000 apple-upscale-0.1.0/src/apple_upscale.egg-info/SOURCES.txt
--rw-r--r--   0 alvinwan   (501) staff       (20)        1 2023-07-12 22:47:52.000000 apple-upscale-0.1.0/src/apple_upscale.egg-info/dependency_links.txt
--rw-r--r--   0 alvinwan   (501) staff       (20)       99 2023-07-12 22:47:52.000000 apple-upscale-0.1.0/src/apple_upscale.egg-info/requires.txt
--rw-r--r--   0 alvinwan   (501) staff       (20)        8 2023-07-12 22:47:52.000000 apple-upscale-0.1.0/src/apple_upscale.egg-info/top_level.txt
-drwxr-xr-x   0 alvinwan   (501) staff       (20)        0 2023-07-12 22:47:52.694318 apple-upscale-0.1.0/src/upscale/
--rw-r--r--   0 alvinwan   (501) staff       (20)      103 2023-06-16 03:49:19.000000 apple-upscale-0.1.0/src/upscale/__init__.py
-drwxr-xr-x   0 alvinwan   (501) staff       (20)        0 2023-07-12 22:47:52.694805 apple-upscale-0.1.0/src/upscale/masking/
--rw-r--r--   0 alvinwan   (501) staff       (20)     6302 2023-06-16 05:22:21.000000 apple-upscale-0.1.0/src/upscale/masking/importance.py
--rw-r--r--   0 alvinwan   (501) staff       (20)    10335 2023-06-16 05:22:21.000000 apple-upscale-0.1.0/src/upscale/masking/mask.py
--rw-r--r--   0 alvinwan   (501) staff       (20)      671 2023-06-16 04:26:49.000000 apple-upscale-0.1.0/src/upscale/masking/utils.py
-drwxr-xr-x   0 alvinwan   (501) staff       (20)        0 2023-07-12 22:47:52.696427 apple-upscale-0.1.0/src/upscale/pruning/
--rw-r--r--   0 alvinwan   (501) staff       (20)      269 2023-06-16 04:26:49.000000 apple-upscale-0.1.0/src/upscale/pruning/__init__.py
--rw-r--r--   0 alvinwan   (501) staff       (20)     4694 2023-06-16 05:22:21.000000 apple-upscale-0.1.0/src/upscale/pruning/manager.py
--rw-r--r--   0 alvinwan   (501) staff       (20)     5352 2023-06-16 04:26:49.000000 apple-upscale-0.1.0/src/upscale/pruning/mock.py
--rw-r--r--   0 alvinwan   (501) staff       (20)     8514 2023-06-16 05:22:21.000000 apple-upscale-0.1.0/src/upscale/pruning/pruner.py
--rw-r--r--   0 alvinwan   (501) staff       (20)    21686 2023-06-16 04:26:49.000000 apple-upscale-0.1.0/src/upscale/pruning/reorder.py
--rw-r--r--   0 alvinwan   (501) staff       (20)    28935 2023-06-16 04:26:49.000000 apple-upscale-0.1.0/src/upscale/pruning/resolve.py
--rw-r--r--   0 alvinwan   (501) staff       (20)    11895 2023-06-16 04:26:49.000000 apple-upscale-0.1.0/src/upscale/pruning/trace.py
--rw-r--r--   0 alvinwan   (501) staff       (20)    17450 2023-06-16 04:26:49.000000 apple-upscale-0.1.0/src/upscale/pruning/tracing.py
--rw-r--r--   0 alvinwan   (501) staff       (20)     5502 2023-06-16 05:22:21.000000 apple-upscale-0.1.0/src/upscale/pruning/utils.py
-drwxr-xr-x   0 alvinwan   (501) staff       (20)        0 2023-07-12 22:47:52.696590 apple-upscale-0.1.0/tests/
--rw-r--r--   0 alvinwan   (501) staff       (20)    10714 2023-06-16 05:22:21.000000 apple-upscale-0.1.0/tests/test_core.py
+drwxr-xr-x   0 alvinwan   (501) staff       (20)        0 2023-07-14 21:57:35.510905 apple-upscale-0.1.1/
+-rw-r--r--   0 alvinwan   (501) staff       (20)     2316 2023-07-14 21:56:56.000000 apple-upscale-0.1.1/LICENSE
+-rw-r--r--   0 alvinwan   (501) staff       (20)     8544 2023-07-14 21:57:35.510710 apple-upscale-0.1.1/PKG-INFO
+-rw-r--r--   0 alvinwan   (501) staff       (20)     4841 2023-07-14 21:56:56.000000 apple-upscale-0.1.1/README.md
+-rw-r--r--   0 alvinwan   (501) staff       (20)     1508 2023-07-14 21:56:56.000000 apple-upscale-0.1.1/pyproject.toml
+-rw-r--r--   0 alvinwan   (501) staff       (20)       38 2023-07-14 21:57:35.510950 apple-upscale-0.1.1/setup.cfg
+drwxr-xr-x   0 alvinwan   (501) staff       (20)        0 2023-07-14 21:57:35.506472 apple-upscale-0.1.1/src/
+drwxr-xr-x   0 alvinwan   (501) staff       (20)        0 2023-07-14 21:57:35.508233 apple-upscale-0.1.1/src/apple_upscale.egg-info/
+-rw-r--r--   0 alvinwan   (501) staff       (20)     8544 2023-07-14 21:57:35.000000 apple-upscale-0.1.1/src/apple_upscale.egg-info/PKG-INFO
+-rw-r--r--   0 alvinwan   (501) staff       (20)      660 2023-07-14 21:57:35.000000 apple-upscale-0.1.1/src/apple_upscale.egg-info/SOURCES.txt
+-rw-r--r--   0 alvinwan   (501) staff       (20)        1 2023-07-14 21:57:35.000000 apple-upscale-0.1.1/src/apple_upscale.egg-info/dependency_links.txt
+-rw-r--r--   0 alvinwan   (501) staff       (20)       99 2023-07-14 21:57:35.000000 apple-upscale-0.1.1/src/apple_upscale.egg-info/requires.txt
+-rw-r--r--   0 alvinwan   (501) staff       (20)        8 2023-07-14 21:57:35.000000 apple-upscale-0.1.1/src/apple_upscale.egg-info/top_level.txt
+drwxr-xr-x   0 alvinwan   (501) staff       (20)        0 2023-07-14 21:57:35.508381 apple-upscale-0.1.1/src/upscale/
+-rw-r--r--   0 alvinwan   (501) staff       (20)      189 2023-07-14 21:56:56.000000 apple-upscale-0.1.1/src/upscale/__init__.py
+drwxr-xr-x   0 alvinwan   (501) staff       (20)        0 2023-07-14 21:57:35.508831 apple-upscale-0.1.1/src/upscale/masking/
+-rw-r--r--   0 alvinwan   (501) staff       (20)     6327 2023-07-14 21:56:56.000000 apple-upscale-0.1.1/src/upscale/masking/importance.py
+-rw-r--r--   0 alvinwan   (501) staff       (20)    10335 2023-07-14 21:56:56.000000 apple-upscale-0.1.1/src/upscale/masking/mask.py
+-rw-r--r--   0 alvinwan   (501) staff       (20)      671 2023-07-14 21:56:56.000000 apple-upscale-0.1.1/src/upscale/masking/utils.py
+drwxr-xr-x   0 alvinwan   (501) staff       (20)        0 2023-07-14 21:57:35.510193 apple-upscale-0.1.1/src/upscale/pruning/
+-rw-r--r--   0 alvinwan   (501) staff       (20)      269 2023-07-14 21:56:56.000000 apple-upscale-0.1.1/src/upscale/pruning/__init__.py
+-rw-r--r--   0 alvinwan   (501) staff       (20)     4742 2023-07-14 21:56:56.000000 apple-upscale-0.1.1/src/upscale/pruning/manager.py
+-rw-r--r--   0 alvinwan   (501) staff       (20)     5352 2023-07-14 21:56:56.000000 apple-upscale-0.1.1/src/upscale/pruning/mock.py
+-rw-r--r--   0 alvinwan   (501) staff       (20)     8486 2023-07-14 21:56:56.000000 apple-upscale-0.1.1/src/upscale/pruning/pruner.py
+-rw-r--r--   0 alvinwan   (501) staff       (20)    21648 2023-07-14 21:56:56.000000 apple-upscale-0.1.1/src/upscale/pruning/reorder.py
+-rw-r--r--   0 alvinwan   (501) staff       (20)    28935 2023-07-14 21:56:56.000000 apple-upscale-0.1.1/src/upscale/pruning/resolve.py
+-rw-r--r--   0 alvinwan   (501) staff       (20)    11895 2023-07-14 21:56:56.000000 apple-upscale-0.1.1/src/upscale/pruning/trace.py
+-rw-r--r--   0 alvinwan   (501) staff       (20)    17340 2023-07-14 21:56:56.000000 apple-upscale-0.1.1/src/upscale/pruning/tracing.py
+-rw-r--r--   0 alvinwan   (501) staff       (20)     5502 2023-07-14 21:56:56.000000 apple-upscale-0.1.1/src/upscale/pruning/utils.py
+drwxr-xr-x   0 alvinwan   (501) staff       (20)        0 2023-07-14 21:57:35.510480 apple-upscale-0.1.1/tests/
+-rw-r--r--   0 alvinwan   (501) staff       (20)      488 2023-07-14 21:56:56.000000 apple-upscale-0.1.1/tests/test_api.py
+-rw-r--r--   0 alvinwan   (501) staff       (20)    10293 2023-07-14 21:56:56.000000 apple-upscale-0.1.1/tests/test_core.py
```

### Comparing `apple-upscale-0.1.0/LICENSE` & `apple-upscale-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `apple-upscale-0.1.0/PKG-INFO` & `apple-upscale-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apple-upscale
-Version: 0.1.0
+Version: 0.1.1
 Summary: Export utility for unconstrained channel pruned models
 Author-email: Alvin Wan <alvinwan@apple.com>
 License: Copyright (C) 2023 Apple Inc. All Rights Reserved.
         
         IMPORTANT:  This Apple software is supplied to you by Apple
         Inc. ("Apple") in consideration of your agreement to the following
         terms, and your use, installation, modification or redistribution of
@@ -58,17 +58,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-# Unconstrained Channel Pruning · [Paper](https://machinelearning.apple.com/research/unconstrained-channel-pruning)
+# Unconstrained Channel Pruning · [Paper](https://openreview.net/forum?id=25fe54GXLo)
 
-**UPSCALE: Unconstrained Channel Pruning** @ [ICML 2023](https://icml.cc/virtual/2023/poster/25215)<br/>
+**UPSCALE: Unconstrained Channel Pruning** @ [ICML 2023](https://openreview.net/forum?id=25fe54GXLo)<br/>
 [Alvin Wan](https://alvinwan.com), [Hanxiang Hao](https://scholar.google.com/citations?user=IMn1m2sAAAAJ&hl=en&oi=ao), [Kaushik Patnaik](https://openreview.net/profile?id=~Kaushik_Patnaik1), [Yueyang Xu](https://github.com/inSam), [Omer Hadad](https://scholar.google.com/citations?user=cHZBEjQAAAAJ&hl=en), [David Güera](https://davidguera.com), [Zhile Ren](https://jrenzhile.com), [Qi Shan](https://scholar.google.com/citations?user=0FbnKXwAAAAJ&hl=en)
 
 By removing constraints from existing pruners, we improve ImageNet accuracy for post-training pruned models by 2.1 points on average - benefiting DenseNet (+16.9), EfficientNetV2 (+7.9), and ResNet (+6.2). Furthermore, for these unconstrained pruned models, UPSCALE improves inference speeds by up to 2x over a baseline export.
 
 ## Quick Start
 
 Install our package.
@@ -76,18 +76,18 @@
 ```bash
 pip install apple-upscale
 ```
 
 Mask and prune channels, using the default magnitude pruner.
 
 ```python
-import torchvision
+import torch, torchvision
 from upscale import MaskingManager, PruningManager
 
-x = torch.rand((1, 3, 224, 224)).cuda()
+x = torch.rand((1, 3, 224, 224), device='cuda')
 model = torchvision.models.get_model('resnet18', pretrained=True).cuda()  # get any pytorch model
 MaskingManager(model).importance().mask()
 PruningManager(model).compute([x]).prune()
 ```
 
 ## Customize Pruning
 
@@ -126,15 +126,15 @@
     # prune each segment in the network independently
     for layer in segment.layers:
         # layers in the segment
 ```
 
 ## Development
 
-> **NOTE:** See [upscale/pruning/README.md](upscale/pruning/README.md) for more details on how the core export algorithm code is organized.
+> **NOTE:** See [src/upscale/pruning/README.md](src/upscale/pruning/README.md) for more details on how the core export algorithm code is organized.
 
 Clone and setup.
 
 ```bash
 git clone git@github.com:apple/ml-upscale.git
 cd upscale
 pip install -e .
```

### Comparing `apple-upscale-0.1.0/README.md` & `apple-upscale-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# Unconstrained Channel Pruning · [Paper](https://machinelearning.apple.com/research/unconstrained-channel-pruning)
+# Unconstrained Channel Pruning · [Paper](https://openreview.net/forum?id=25fe54GXLo)
 
-**UPSCALE: Unconstrained Channel Pruning** @ [ICML 2023](https://icml.cc/virtual/2023/poster/25215)<br/>
+**UPSCALE: Unconstrained Channel Pruning** @ [ICML 2023](https://openreview.net/forum?id=25fe54GXLo)<br/>
 [Alvin Wan](https://alvinwan.com), [Hanxiang Hao](https://scholar.google.com/citations?user=IMn1m2sAAAAJ&hl=en&oi=ao), [Kaushik Patnaik](https://openreview.net/profile?id=~Kaushik_Patnaik1), [Yueyang Xu](https://github.com/inSam), [Omer Hadad](https://scholar.google.com/citations?user=cHZBEjQAAAAJ&hl=en), [David Güera](https://davidguera.com), [Zhile Ren](https://jrenzhile.com), [Qi Shan](https://scholar.google.com/citations?user=0FbnKXwAAAAJ&hl=en)
 
 By removing constraints from existing pruners, we improve ImageNet accuracy for post-training pruned models by 2.1 points on average - benefiting DenseNet (+16.9), EfficientNetV2 (+7.9), and ResNet (+6.2). Furthermore, for these unconstrained pruned models, UPSCALE improves inference speeds by up to 2x over a baseline export.
 
 ## Quick Start
 
 Install our package.
@@ -12,18 +12,18 @@
 ```bash
 pip install apple-upscale
 ```
 
 Mask and prune channels, using the default magnitude pruner.
 
 ```python
-import torchvision
+import torch, torchvision
 from upscale import MaskingManager, PruningManager
 
-x = torch.rand((1, 3, 224, 224)).cuda()
+x = torch.rand((1, 3, 224, 224), device='cuda')
 model = torchvision.models.get_model('resnet18', pretrained=True).cuda()  # get any pytorch model
 MaskingManager(model).importance().mask()
 PruningManager(model).compute([x]).prune()
 ```
 
 ## Customize Pruning
 
@@ -62,15 +62,15 @@
     # prune each segment in the network independently
     for layer in segment.layers:
         # layers in the segment
 ```
 
 ## Development
 
-> **NOTE:** See [upscale/pruning/README.md](upscale/pruning/README.md) for more details on how the core export algorithm code is organized.
+> **NOTE:** See [src/upscale/pruning/README.md](src/upscale/pruning/README.md) for more details on how the core export algorithm code is organized.
 
 Clone and setup.
 
 ```bash
 git clone git@github.com:apple/ml-upscale.git
 cd upscale
 pip install -e .
```

### Comparing `apple-upscale-0.1.0/pyproject.toml` & `apple-upscale-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
 # For licensing see accompanying LICENSE file.
 # Copyright (C) 2023 Apple Inc. All Rights Reserved.
 #
 
 [project]
 name = "apple-upscale"  # Required
-version = "0.1.0"  # Required
+version = "0.1.1"  # Required
 description = "Export utility for unconstrained channel pruned models"  # Optional
 readme = "README.md" # Optional
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 keywords = ["pruning", "export", "unconstrained pruning"]  # Optional
 authors = [
   {name = "Alvin Wan", email = "alvinwan@apple.com" } # Optional
```

### Comparing `apple-upscale-0.1.0/src/apple_upscale.egg-info/PKG-INFO` & `apple-upscale-0.1.1/src/apple_upscale.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apple-upscale
-Version: 0.1.0
+Version: 0.1.1
 Summary: Export utility for unconstrained channel pruned models
 Author-email: Alvin Wan <alvinwan@apple.com>
 License: Copyright (C) 2023 Apple Inc. All Rights Reserved.
         
         IMPORTANT:  This Apple software is supplied to you by Apple
         Inc. ("Apple") in consideration of your agreement to the following
         terms, and your use, installation, modification or redistribution of
@@ -58,17 +58,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-# Unconstrained Channel Pruning · [Paper](https://machinelearning.apple.com/research/unconstrained-channel-pruning)
+# Unconstrained Channel Pruning · [Paper](https://openreview.net/forum?id=25fe54GXLo)
 
-**UPSCALE: Unconstrained Channel Pruning** @ [ICML 2023](https://icml.cc/virtual/2023/poster/25215)<br/>
+**UPSCALE: Unconstrained Channel Pruning** @ [ICML 2023](https://openreview.net/forum?id=25fe54GXLo)<br/>
 [Alvin Wan](https://alvinwan.com), [Hanxiang Hao](https://scholar.google.com/citations?user=IMn1m2sAAAAJ&hl=en&oi=ao), [Kaushik Patnaik](https://openreview.net/profile?id=~Kaushik_Patnaik1), [Yueyang Xu](https://github.com/inSam), [Omer Hadad](https://scholar.google.com/citations?user=cHZBEjQAAAAJ&hl=en), [David Güera](https://davidguera.com), [Zhile Ren](https://jrenzhile.com), [Qi Shan](https://scholar.google.com/citations?user=0FbnKXwAAAAJ&hl=en)
 
 By removing constraints from existing pruners, we improve ImageNet accuracy for post-training pruned models by 2.1 points on average - benefiting DenseNet (+16.9), EfficientNetV2 (+7.9), and ResNet (+6.2). Furthermore, for these unconstrained pruned models, UPSCALE improves inference speeds by up to 2x over a baseline export.
 
 ## Quick Start
 
 Install our package.
@@ -76,18 +76,18 @@
 ```bash
 pip install apple-upscale
 ```
 
 Mask and prune channels, using the default magnitude pruner.
 
 ```python
-import torchvision
+import torch, torchvision
 from upscale import MaskingManager, PruningManager
 
-x = torch.rand((1, 3, 224, 224)).cuda()
+x = torch.rand((1, 3, 224, 224), device='cuda')
 model = torchvision.models.get_model('resnet18', pretrained=True).cuda()  # get any pytorch model
 MaskingManager(model).importance().mask()
 PruningManager(model).compute([x]).prune()
 ```
 
 ## Customize Pruning
 
@@ -126,15 +126,15 @@
     # prune each segment in the network independently
     for layer in segment.layers:
         # layers in the segment
 ```
 
 ## Development
 
-> **NOTE:** See [upscale/pruning/README.md](upscale/pruning/README.md) for more details on how the core export algorithm code is organized.
+> **NOTE:** See [src/upscale/pruning/README.md](src/upscale/pruning/README.md) for more details on how the core export algorithm code is organized.
 
 Clone and setup.
 
 ```bash
 git clone git@github.com:apple/ml-upscale.git
 cd upscale
 pip install -e .
```

### Comparing `apple-upscale-0.1.0/src/apple_upscale.egg-info/SOURCES.txt` & `apple-upscale-0.1.1/src/apple_upscale.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -15,8 +15,9 @@
 src/upscale/pruning/mock.py
 src/upscale/pruning/pruner.py
 src/upscale/pruning/reorder.py
 src/upscale/pruning/resolve.py
 src/upscale/pruning/trace.py
 src/upscale/pruning/tracing.py
 src/upscale/pruning/utils.py
+tests/test_api.py
 tests/test_core.py
```

### Comparing `apple-upscale-0.1.0/src/upscale/masking/importance.py` & `apple-upscale-0.1.1/src/upscale/masking/importance.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,14 +147,15 @@
                 torch.save(mean, path)
 
                 logging.info(f"Computed rank for {module._name} ({x.shape}) in {round(end - start, 2)}s")
             else:
                 logging.debug(f"Loaded precomputed rank for {module._name})")
 
         model._handles = []
+        model._name = ''
         is_hook_registered = False
         for name, module in model.named_modules():
             if isinstance(module, nn.Conv2d):
                 module._name = name
                 path = self.get_rank_path(model, module)
                 if not path.exists():
                     model._handles.append(module.register_forward_hook(hook))
```

### Comparing `apple-upscale-0.1.0/src/upscale/masking/mask.py` & `apple-upscale-0.1.1/src/upscale/masking/mask.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     def get_weights(self, layers):
         return [getattr(layer, self.name).transpose(0, self.dim).detach() for layer in layers]
 
     def set_weights(self, layers, weights):
         for layer, weight in zip(layers, weights):
             param = nn.Parameter(weight.transpose(0, self.dim))
             old = getattr(layer, self.name)
-            param.tensor_id = getattr(old, 'tensor_id', None)  # TODO: hack to preserve op ids in trace
+            param.tensor_id = getattr(old, 'tensor_id', None)  # NOTE: hack to preserve op ids in trace
             setattr(layer, self.name, param)
 
     def importance(self, heuristic=Magnitude()):
         if heuristic.name == 'weight':
             # TODO: broken in general (e.g., for densenet, need to use trace)
             unpruneds = [weight.reshape(weight.shape[0], -1) for weight in self.get_weights(self.layers)]
         else:
```

### Comparing `apple-upscale-0.1.0/src/upscale/masking/utils.py` & `apple-upscale-0.1.1/src/upscale/masking/utils.py`

 * *Files identical despite different names*

### Comparing `apple-upscale-0.1.0/src/upscale/pruning/manager.py` & `apple-upscale-0.1.1/src/upscale/pruning/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,26 +28,26 @@
     >>> net = resnet18()
     >>> x = torch.rand((1, 3, 224, 224))
 
     Compute pruning parameters using a set of pruned input channel indices.
 
     >>> manager = PruningManager(net)
     >>> pruned_inputs = [('layer1.1.conv1.weight', 5)]
-    >>> manager.compute([x], pruned_inputs=pruned_inputs)
+    >>> _ = manager.compute([x], pruned_inputs=pruned_inputs)
 
     Then, during training, you can use the mock-pruned model. This mock-pruned
     model applies masks instead of modifying the model itself.
 
     >>> net_mock = manager.get_mock_model()
     >>> y_mock = net_mock(x)
 
     Finally, actually prune the model. Then run inference using the *original
     (now modified, in place) model.
 
-    >>> manager.prune()
+    >>> _ = manager.prune()
     >>> y_pruned = net(x)
 
     Check that both the mocked and pruned outputs match.
 
     >>> (y_pruned - y_mock).abs().max() < 1e-5
     tensor(True)
 
@@ -101,14 +101,15 @@
         """
         if self.spec is None or force:
             traced = self.trace(inputs, force)
             if pruned_inputs is None and pruned_outputs is None:
                 pruned_inputs, pruned_outputs = get_mask_indices(traced.tensor_to_metadata)
             self.spec = generate_pruning_spec(
                 traced, pruned_outputs, pruned_inputs, net=self.net, **kwargs)
+        return self
 
     def get_mock_model(self):
         """
         Obtain a model you can run normally, just like any other PyTorch model.
         Emulates a pruned model.
         """
         assert self.spec is not None, (
@@ -124,8 +125,9 @@
         Note that the wrapped model, after pruning, can't be reloaded after
         saving. The architecture will differ, so attempting to load a pruned
         checkpoint will result in errors. After this step, the only path
         forward is to fully export the model, e.g., using torchscript.
         """
         prune_model(self.spec, is_not_ane=is_not_ane, baseline=baseline)
         self.spec = None  # NOTE: clear pruning params, which are now invalid
+        return self
```

### Comparing `apple-upscale-0.1.0/src/upscale/pruning/mock.py` & `apple-upscale-0.1.1/src/upscale/pruning/mock.py`

 * *Files identical despite different names*

### Comparing `apple-upscale-0.1.0/src/upscale/pruning/pruner.py` & `apple-upscale-0.1.1/src/upscale/pruning/pruner.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,14 @@
         ('conv' in module_name or 'linear' in module_name)
     is_depthwise = (
         'conv' in module.__class__.__name__.lower()
         and getattr(module, 'groups', 0) > 1
     )
     # or (input_weight_indices is not None and max(input_weight_indices) > 1
     # and len(weight.shape) > 1 and weight.shape[1] == 1):
-    # TODO: do we need this
     if ('transpose' in module_name and not is_bias):
         output_weight_indices, input_weight_indices = \
             input_weight_indices, output_weight_indices
     if is_depthwise or (is_constant and not is_bias):
         output_weight_indices, input_weight_indices = \
             input_weight_indices, None
     if is_depthwise and output_weight_indices is not None:
```

### Comparing `apple-upscale-0.1.0/src/upscale/pruning/reorder.py` & `apple-upscale-0.1.1/src/upscale/pruning/reorder.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,15 +245,15 @@
     >>> compute_reordering(
     ...     {1, 2, 3, 4}, {1: {0,}, 2: {0, 1,}, 3: {0, 1, 2}, 4: {0, 1, 2}}
     ... )  # order should not change
     [0, 1, 2]
     >>> compute_reordering({2, 3}, {2: [(1, 2), (1, 3), (4, 0)], 3: [(1, 1)]})
     [(1, 2), (1, 3), (4, 0), (1, 1)]
     """
-    # 1. Find all sub-nodes.  # TODO: figure out subset optimality
+    # 1. Find all sub-nodes.
     parent_to_children = group_child_nodes(nodes, node_to_members)
     node_to_ordered_members = compute_child_node_reordering(
         parent_to_children, node_to_members)
     nodes = parent_to_children.keys()
 
     # 2. Construct adjacency and cost matrices.
     adj, cost = build_adjacency_cost(nodes, node_to_members)
```

### Comparing `apple-upscale-0.1.0/src/upscale/pruning/resolve.py` & `apple-upscale-0.1.1/src/upscale/pruning/resolve.py`

 * *Files identical despite different names*

### Comparing `apple-upscale-0.1.0/src/upscale/pruning/trace.py` & `apple-upscale-0.1.1/src/upscale/pruning/trace.py`

 * *Files identical despite different names*

### Comparing `apple-upscale-0.1.0/src/upscale/pruning/tracing.py` & `apple-upscale-0.1.1/src/upscale/pruning/tracing.py`

 * *Files 0% similar despite different names*

```diff
@@ -422,16 +422,14 @@
             channel_axis - dimension for the channel axis
 
         >>> x, traces = torch.rand(1, 3, 12, 12), [trace_from_n_channels(0, 3)]
         >>> k = {'input': x, 'dim': (0, 2, 3, 1)}
         >>> Tracer.compute_new_channels(0, traces, torch.permute, k, x, 1)[2]
         3
         """
-        # TODO: support view, reshape by tracking channel axes
-        # TODO: support pad with a n/a source?
         is_trace_reset = False
         is_convolution = func in (
             torch.conv1d,
             torch.conv2d,
             torch.conv3d,
             torch.conv_transpose1d,
             torch.conv_transpose2d,
```

### Comparing `apple-upscale-0.1.0/src/upscale/pruning/utils.py` & `apple-upscale-0.1.1/src/upscale/pruning/utils.py`

 * *Files identical despite different names*

### Comparing `apple-upscale-0.1.0/tests/test_core.py` & `apple-upscale-0.1.1/tests/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,28 +228,14 @@
         y1 = self.linear0(x)
         y2 = self.linear1(y1)
         y3 = self.linear2(y2)
         y4 = self.linear3(y3)
         return y4
 
 
-class Permute(nn.Module):
-    def __init__(self):
-        super().__init__()
-        self.conv0 = nn.Conv2d(3, 5, 3, padding=1)
-        self.conv1 = nn.Conv2d(5, 5, 3, padding=1)
-
-    def forward(self, x):
-        y = self.conv0(x)
-        y = y.permute(0, 2, 3, 1)
-        y = y.permute(0, 3, 1, 2)
-        y = self.conv1(y)
-        return y
-
-
 def check_pruning_correctness(
     net, inputs=None, input_shapes=[(1, 3, 224, 224)], threshold=1e-14, Manager=PyTorchPruningManager, **kwargs
 ):      
     if inputs is None:
         inputs = [torch.rand(input_shape) for input_shape in input_shapes]
 
     if torch.cuda.is_available():
@@ -289,15 +275,14 @@
     (Depthwise, [('conv2.weight', 3)], [], [(1, 3, 224, 224)]),
     (ConcatProducers, [('conv2.weight', 3)], [], [(1, 3, 224, 224)]),
     (MultipleProducersConsumers, [('conv2.weight', 3), ('conv4.weight', 3)], [], [(1, 3, 224, 224)]),
     (Deconv, [('conv2.weight', 3)], [], [(1, 3, 224, 224)]),
     (ConvBNReluLumpy, [], [('1.weight', 1)], [(1, 3, 224, 224)]),
     (UnbiasedConv, [], [('0.weight', 1)], [(1, 3, 5, 5)]),        # 'small' input size (anything >= 10 will pass)
     (MLP, [('linear2.weight', 2)], [], [(1, 3)]),
-    # (Permute, [], [('conv1.weight', 2)], [(1, 3, 5, 5)]), # TODO: restore
 ))
 def test_pruning_core_pytorch_constrained(Net, pruned_inputs, pruned_outputs, input_shapes):
     """Test core pytorch pruning implementation.
 
     These tests are designed to catch specific edge cases in e2e tests. For randomized tests on more
     realistic models, see `test_pruning_core_random`.
     """
```

