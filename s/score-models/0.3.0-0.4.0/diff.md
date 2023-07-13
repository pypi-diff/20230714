# Comparing `tmp/score_models-0.3.0.tar.gz` & `tmp/score_models-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "score_models-0.3.0.tar", last modified: Thu Jul  6 14:09:29 2023, max compression
+gzip compressed data, was "score_models-0.4.0.tar", last modified: Thu Jul 13 23:07:47 2023, max compression
```

## Comparing `score_models-0.3.0.tar` & `score_models-0.4.0.tar`

### file list

```diff
@@ -1,60 +1,62 @@
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-06 14:09:29.392583 score_models-0.3.0/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6213 2023-07-06 14:09:29.392583 score_models-0.3.0/PKG-INFO
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     5325 2023-07-06 13:52:29.000000 score_models-0.3.0/README.md
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       90 2023-07-06 13:52:30.000000 score_models-0.3.0/pyproject.toml
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-06 14:09:29.388583 score_models-0.3.0/score_models/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       94 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/__init__.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-06 14:09:29.392583 score_models-0.3.0/score_models/architectures/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       71 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/architectures/__init__.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     4923 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/architectures/ddpm.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3557 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/architectures/mlp.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)    15113 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/architectures/ncsnpp.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)    16600 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/base.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2035 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/definitions.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-06 14:09:29.392583 score_models-0.3.0/score_models/layers/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      686 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/layers/__init__.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3574 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/layers/attention_block.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      601 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/layers/combine.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2766 2023-03-05 17:43:23.000000 score_models-0.3.0/score_models/layers/conditional_batchnorm2d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2279 2023-03-05 17:43:23.000000 score_models-0.3.0/score_models/layers/conditional_instancenorm2d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2980 2023-03-05 17:43:23.000000 score_models-0.3.0/score_models/layers/conditional_instancenorm2d_plus.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2903 2023-03-05 17:43:23.000000 score_models-0.3.0/score_models/layers/conv1dsame.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3120 2023-03-05 17:43:23.000000 score_models-0.3.0/score_models/layers/conv2dsame.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3134 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/layers/conv3dsame.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1111 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/layers/conv_layers.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3354 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/layers/ddpm_resnet_block.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1950 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/layers/downsample.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3543 2023-03-05 17:43:23.000000 score_models-0.3.0/score_models/layers/ncsn_resnet_block.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      611 2023-03-05 17:43:23.000000 score_models-0.3.0/score_models/layers/projection_embedding.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3232 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/layers/resnet_block_biggan.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2447 2023-03-05 17:43:23.000000 score_models-0.3.0/score_models/layers/spectral_normalization.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      862 2023-03-05 17:43:23.000000 score_models-0.3.0/score_models/layers/squeeze_and_excitation.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2123 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/layers/style_gan_conv.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1957 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/layers/up_or_downsampling.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6493 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/layers/up_or_downsampling1d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     7626 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/layers/up_or_downsampling2d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     7507 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/layers/up_or_downsampling3d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1485 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/layers/upfirdn1d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1720 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/layers/upfirdn2d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2053 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/layers/upfirdn3d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1558 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/layers/upsample.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1590 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/score_model.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-06 14:09:29.392583 score_models-0.3.0/score_models/sde/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       71 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/sde/__init__.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1268 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/sde/sde.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1653 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/sde/vesde.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1504 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/sde/vpsde.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3672 2023-07-06 13:52:30.000000 score_models-0.3.0/score_models/utils.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-06 14:09:29.388583 score_models-0.3.0/score_models.egg-info/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6213 2023-07-06 14:09:29.000000 score_models-0.3.0/score_models.egg-info/PKG-INFO
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1715 2023-07-06 14:09:29.000000 score_models-0.3.0/score_models.egg-info/SOURCES.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)        1 2023-07-06 14:09:29.000000 score_models-0.3.0/score_models.egg-info/dependency_links.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       43 2023-07-06 14:09:29.000000 score_models-0.3.0/score_models.egg-info/requires.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       13 2023-07-06 14:09:29.000000 score_models-0.3.0/score_models.egg-info/top_level.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       38 2023-07-06 14:09:29.392583 score_models-0.3.0/setup.cfg
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      880 2023-07-06 14:07:37.000000 score_models-0.3.0/setup.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-06 14:09:29.392583 score_models-0.3.0/tests/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1231 2023-07-06 13:52:30.000000 score_models-0.3.0/tests/test_architectures.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6839 2023-07-06 13:52:30.000000 score_models-0.3.0/tests/test_layers.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1384 2023-07-06 13:52:30.000000 score_models-0.3.0/tests/test_loading_score.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3090 2023-07-06 13:52:30.000000 score_models-0.3.0/tests/test_training.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-13 23:07:47.130668 score_models-0.4.0/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1081 2023-07-06 14:56:40.000000 score_models-0.4.0/LICENSE.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6233 2023-07-13 23:07:47.130668 score_models-0.4.0/PKG-INFO
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     5617 2023-07-13 16:06:46.000000 score_models-0.4.0/README.md
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       90 2023-07-06 13:52:30.000000 score_models-0.4.0/pyproject.toml
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-13 23:07:47.126669 score_models-0.4.0/score_models/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       94 2023-07-06 13:52:30.000000 score_models-0.4.0/score_models/__init__.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-13 23:07:47.126669 score_models-0.4.0/score_models/architectures/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       71 2023-07-06 13:52:30.000000 score_models-0.4.0/score_models/architectures/__init__.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     4940 2023-07-13 16:30:47.000000 score_models-0.4.0/score_models/architectures/ddpm.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3557 2023-07-06 13:52:30.000000 score_models-0.4.0/score_models/architectures/mlp.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)    15113 2023-07-06 13:52:30.000000 score_models-0.4.0/score_models/architectures/ncsnpp.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)    20511 2023-07-13 22:53:22.000000 score_models-0.4.0/score_models/base.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2035 2023-07-06 13:52:30.000000 score_models-0.4.0/score_models/definitions.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-13 23:07:47.130668 score_models-0.4.0/score_models/layers/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      686 2023-07-06 13:52:30.000000 score_models-0.4.0/score_models/layers/__init__.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3574 2023-07-06 13:52:30.000000 score_models-0.4.0/score_models/layers/attention_block.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      601 2023-07-06 13:52:30.000000 score_models-0.4.0/score_models/layers/combine.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2766 2023-03-05 17:43:23.000000 score_models-0.4.0/score_models/layers/conditional_batchnorm2d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2279 2023-03-05 17:43:23.000000 score_models-0.4.0/score_models/layers/conditional_instancenorm2d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2980 2023-03-05 17:43:23.000000 score_models-0.4.0/score_models/layers/conditional_instancenorm2d_plus.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2903 2023-03-05 17:43:23.000000 score_models-0.4.0/score_models/layers/conv1dsame.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3120 2023-03-05 17:43:23.000000 score_models-0.4.0/score_models/layers/conv2dsame.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3134 2023-07-06 13:52:30.000000 score_models-0.4.0/score_models/layers/conv3dsame.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1111 2023-07-06 13:52:30.000000 score_models-0.4.0/score_models/layers/conv_layers.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3354 2023-07-06 13:52:30.000000 score_models-0.4.0/score_models/layers/ddpm_resnet_block.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1950 2023-07-06 13:52:30.000000 score_models-0.4.0/score_models/layers/downsample.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3543 2023-03-05 17:43:23.000000 score_models-0.4.0/score_models/layers/ncsn_resnet_block.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      611 2023-03-05 17:43:23.000000 score_models-0.4.0/score_models/layers/projection_embedding.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3232 2023-07-06 13:52:30.000000 score_models-0.4.0/score_models/layers/resnet_block_biggan.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2447 2023-03-05 17:43:23.000000 score_models-0.4.0/score_models/layers/spectral_normalization.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      862 2023-03-05 17:43:23.000000 score_models-0.4.0/score_models/layers/squeeze_and_excitation.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2123 2023-07-06 13:52:30.000000 score_models-0.4.0/score_models/layers/style_gan_conv.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1957 2023-07-06 13:52:30.000000 score_models-0.4.0/score_models/layers/up_or_downsampling.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6493 2023-07-06 13:52:30.000000 score_models-0.4.0/score_models/layers/up_or_downsampling1d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     7626 2023-07-06 13:52:30.000000 score_models-0.4.0/score_models/layers/up_or_downsampling2d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     7507 2023-07-06 13:52:30.000000 score_models-0.4.0/score_models/layers/up_or_downsampling3d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1485 2023-07-06 13:52:30.000000 score_models-0.4.0/score_models/layers/upfirdn1d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1720 2023-07-06 13:52:30.000000 score_models-0.4.0/score_models/layers/upfirdn2d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2053 2023-07-06 13:52:30.000000 score_models-0.4.0/score_models/layers/upfirdn3d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1558 2023-07-06 13:52:30.000000 score_models-0.4.0/score_models/layers/upsample.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1590 2023-07-13 20:33:56.000000 score_models-0.4.0/score_models/score_model.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-13 23:07:47.130668 score_models-0.4.0/score_models/sde/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       71 2023-07-06 13:52:30.000000 score_models-0.4.0/score_models/sde/__init__.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1348 2023-07-13 16:04:19.000000 score_models-0.4.0/score_models/sde/sde.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2110 2023-07-13 20:33:46.000000 score_models-0.4.0/score_models/sde/vesde.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1577 2023-07-13 22:41:55.000000 score_models-0.4.0/score_models/sde/vpsde.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3101 2023-07-13 20:57:29.000000 score_models-0.4.0/score_models/sliced_score_matching.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3672 2023-07-06 13:52:30.000000 score_models-0.4.0/score_models/utils.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-13 23:07:47.126669 score_models-0.4.0/score_models.egg-info/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6233 2023-07-13 23:07:47.000000 score_models-0.4.0/score_models.egg-info/PKG-INFO
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1764 2023-07-13 23:07:47.000000 score_models-0.4.0/score_models.egg-info/SOURCES.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)        1 2023-07-13 23:07:47.000000 score_models-0.4.0/score_models.egg-info/dependency_links.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       43 2023-07-13 23:07:47.000000 score_models-0.4.0/score_models.egg-info/requires.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       13 2023-07-13 23:07:47.000000 score_models-0.4.0/score_models.egg-info/top_level.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       38 2023-07-13 23:07:47.130668 score_models-0.4.0/setup.cfg
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      880 2023-07-13 23:06:39.000000 score_models-0.4.0/setup.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-13 23:07:47.130668 score_models-0.4.0/tests/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1231 2023-07-06 13:52:30.000000 score_models-0.4.0/tests/test_architectures.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6839 2023-07-06 13:52:30.000000 score_models-0.4.0/tests/test_layers.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2361 2023-07-13 22:54:03.000000 score_models-0.4.0/tests/test_score_models.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2888 2023-07-13 16:45:56.000000 score_models-0.4.0/tests/test_training.py
```

### Comparing `score_models-0.3.0/PKG-INFO` & `score_models-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: score_models
-Version: 0.3.0
+Version: 0.4.0
 Summary: A simple pytorch interface for score model and basic diffusion.
 Home-page: https://github.com/AlexandreAdam/torch_score_models
 Author: Alexandre Adam
 Author-email: alexandre.adam@umontreal.ca
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
+License-File: LICENSE.txt
 
 =========================
 Score Models for Pytorch
 =========================
 
 .. image:: https://badge.fury.io/py/score_models.svg
    :target: https://badge.fury.io/py/score_models
@@ -67,15 +68,15 @@
    model = ScoreModelBase(model=net, beta_min=1e-2, beta_max=20, device="cuda")
 
    # NN Architectures support a Unet with 1D convolutions for time series input data
    net = NCSNpp(channels=1, nf=128, ch_mult=[2, 2, 2, 2], dimensions=1)
    # ... or 3D convolutions for videos/voxels
    net = NCSNpp(channels=1, nf=128, ch_mult=[2, 2, 2, 2], attention=False, dimensions=3)
    # You can also use a simpler MLP architecture
-   net = MLP(input_dimensions=dim, layers=4, units=100)
+   net = MLP(dimensions=dim, layers=4, units=100)
    # ... or Jonathan Ho's DDPM architecture
    net = DDPM(channels=1, dimensions=2, nf=128, ch_mult=[2, 2, 2, 2])
 
    # Train the model
    model.fit(dataset=your_dataset, epochs=100, learning_rate=1e-4)
 
    # Generate samples from the trained model
```

### Comparing `score_models-0.3.0/README.md` & `score_models-0.4.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 # Score Models for Pytorch
 
 [![PyPI version](https://badge.fury.io/py/score_models.svg)](https://badge.fury.io/py/score_models)
 [![codecov](https://codecov.io/gh/AlexandreAdam/torch_score_models/branch/dev/graph/badge.svg)](https://codecov.io/gh/AlexandreAdam/torch_score_models)
 
 A storage for score-based models. The `ScoreModel` interface gives access to the following utilities
 - Simple initialisation of MLP, NCSN++ and DDPM neural network architectures
-- A fit method to train the score model on a dataset using Denoising Score Matching (DSM).
+- A fit method to train the score model on a dataset using Denoising Score Matching (DSM: see [Vincent 2011](https://www.iro.umontreal.ca/~vincentp/Publications/DenoisingScoreMatching_NeuralComp2011.pdf)).
 - A sampling method based on an Euler-Maruyama discretisation of an SDE. 
 - A simple interface to train an energy model using DSM
 
 This repository is mainly intended for personal use. 
 You might also want to refer to the original implementation at [https://github.com/yang-song/score_sde](https://github.com/yang-song/score_sde).
 
 ## Installation
 
 To install the package, you can use pip:
 
 ```bash
-pip install torch-score-models
+pip install score_models
 ```
 
 ## Usage
 
 
 ### ScoreModel
 
 The `ScoreModel` class is the main interface for training and using score models, defined as
-$$
-    \mathbf{s}_\theta(t, \mathbf{x}) = \frac{1}{\sigma(t)} \nabla_\mathbf{x} \log p_t(\mathbf{x})
-$$
-where $\sigma(t)$ is the standard deviation of the perturbation kernel $p_t(\mathbf{x} \mid \mathbf{x}_0)$ 
-of an SDE.
+
+```math
+\mathbf{s}_\theta(t, \mathbf{x}) \equiv \nabla_\mathbf{x} \log p_t(\mathbf{x}) = \frac{1}{\sigma(t)} f_\theta (t, \mathbf{x})$$
+```
+
+where $\sigma(t)$ is the standard deviation of the perturbation kernel $`p_t(\mathbf{x} \mid \mathbf{x}_0)`$
+of an SDE and $f_\theta : [0, 1] \times\mathbb{R}^d \to \mathbb{R}^d$ is a neural network for $\mathbf{x} \in \mathbb{R}^d$. 
 
 The `ScoreModel` class extends the `torch.nn.Module` class. Example usage:
 
 ```python
 from score_models import ScoreModel, EnergyModel, NCSNpp, MLP, DDPM
 
 # Create a ScoreModelBase instance with Yang Song's NCSN++ architecture and the VESDE
@@ -44,15 +46,15 @@
 model = ScoreModelBase(model=net, beta_min=1e-2, beta_max=20, device="cuda")
 
 # NN Architectures support a Unet with 1D convolutions for time series input data
 net = NCSNpp(channels=1, nf=128, ch_mult=[2, 2, 2, 2], dimensions=1)
 # ... or 3D convolutions for videos/voxels
 net = NCSNpp(channels=1, nf=128, ch_mult=[2, 2, 2, 2], attention=False, dimensions=3)
 # You can also use a simpler MLP architecture 
-net = MLP(input_dimensions=dim, layers=4, units=100)
+net = MLP(dimensions=dim, layers=4, units=100)
 # ... or Jonathan Ho's DDPM architecture
 net = DDPM(channels=1, dimensions=2, nf=128, ch_mult=[2, 2, 2, 2])
 
 # Train the model
 model.fit(dataset=your_dataset, epochs=100, learning_rate=1e-4)
 
 # Generate samples from the trained model
@@ -65,25 +67,27 @@
 score = ScoreModel(checkpoint_directory)
 ```
 
 ### EnergyModel
 
 The `EnergyModel` class works in pretty much the same way as `ScoreModel`, but implements the score via the 
 automatic differentation of an energy model
-$$
-    E_\theta(t, \mathbf{x}) = \frac{1}{2 \sigma(t)} \lVert \mathbf{x} - f_\theta(t, \mathbf{x}) \rVert_2^ 2
-$$
+```math
+E_\theta(t, \mathbf{x}) = \frac{1}{2 \sigma(t)} \lVert \mathbf{x} - f_\theta (t, \mathbf{x}) \rVert_2^ 2
+```
+
 This is to say that the score is defined as
-$$
-    \mathbf{s}_\theta(t, \mathbf{x}) = - \nabla_\mathbf{x} E_\theta(t, \mathbf{x})
-$$
+```math
+\mathbf{s}_\theta (t, \mathbf{x}) = - \nabla_\mathbf{x} E_\theta(t, \mathbf{x}) 
+```
+
 
 **Note**: When using the MLP architecture, the energy model can be constructed more efficiently as the output of the
 neural network by specifying `nn_is_energy` in the hyperparameters of the MLP, which will modify the neural network 
-architecture to be a function $f_\theta: \mathbb{R}^d \to \mathbb{R}$ instead of $f_\theta: \mathbb{R}^d \to \mathbb{R}^d$. An `output_activation` like `relu` 
+architecture to be a function $f_\theta: [0, 1] \times\mathbb{R}^d \to \mathbb{R}$ instead of $f_\theta: [0, 1] \times\mathbb{R}^d \to \mathbb{R}^d$. An `output_activation` like `relu` 
 can also be specified to make the energy positive or bounded from below.
 
 
 ### Training Parameters
 
 When training the model using the `fit` method, you can provide various parameters to customize the training process. Some important parameters include:
```

### Comparing `score_models-0.3.0/score_models/architectures/ddpm.py` & `score_models-0.4.0/score_models/architectures/ddpm.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
                 out_ch = nf * ch_mult[i_level]
                 modules.append(ResnetBlock(in_ch=in_ch + hs_c.pop(), out_ch=out_ch))
                 in_ch = out_ch
             if i_level != 0:
                 modules.append(Upsample(in_ch=in_ch, with_conv=resample_with_conv))
 
         assert not hs_c
-        modules.append(nn.GroupNorm(num_channels=in_ch, num_groups=32, eps=1e-6))
+        modules.append(nn.GroupNorm(num_channels=in_ch, num_groups=min(in_ch // 4, 32), eps=1e-6))
         modules.append(conv3x3(in_ch, channels))
         self.all_modules = nn.ModuleList(modules)
 
     def forward(self, t, x):
         modules = self.all_modules
         m_idx = 0
         temb = t
```

### Comparing `score_models-0.3.0/score_models/architectures/mlp.py` & `score_models-0.4.0/score_models/architectures/mlp.py`

 * *Files identical despite different names*

### Comparing `score_models-0.3.0/score_models/architectures/ncsnpp.py` & `score_models-0.4.0/score_models/architectures/ncsnpp.py`

 * *Files identical despite different names*

### Comparing `score_models-0.3.0/score_models/definitions.py` & `score_models-0.4.0/score_models/definitions.py`

 * *Files identical despite different names*

### Comparing `score_models-0.3.0/score_models/layers/__init__.py` & `score_models-0.4.0/score_models/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `score_models-0.3.0/score_models/layers/attention_block.py` & `score_models-0.4.0/score_models/layers/attention_block.py`

 * *Files identical despite different names*

### Comparing `score_models-0.3.0/score_models/layers/combine.py` & `score_models-0.4.0/score_models/layers/combine.py`

 * *Files identical despite different names*

### Comparing `score_models-0.3.0/score_models/layers/conditional_batchnorm2d.py` & `score_models-0.4.0/score_models/layers/conditional_batchnorm2d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.3.0/score_models/layers/conditional_instancenorm2d.py` & `score_models-0.4.0/score_models/layers/conditional_instancenorm2d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.3.0/score_models/layers/conditional_instancenorm2d_plus.py` & `score_models-0.4.0/score_models/layers/conditional_instancenorm2d_plus.py`

 * *Files identical despite different names*

### Comparing `score_models-0.3.0/score_models/layers/conv1dsame.py` & `score_models-0.4.0/score_models/layers/conv1dsame.py`

 * *Files identical despite different names*

### Comparing `score_models-0.3.0/score_models/layers/conv2dsame.py` & `score_models-0.4.0/score_models/layers/conv2dsame.py`

 * *Files identical despite different names*

### Comparing `score_models-0.3.0/score_models/layers/conv3dsame.py` & `score_models-0.4.0/score_models/layers/conv3dsame.py`

 * *Files identical despite different names*

### Comparing `score_models-0.3.0/score_models/layers/conv_layers.py` & `score_models-0.4.0/score_models/layers/conv_layers.py`

 * *Files identical despite different names*

### Comparing `score_models-0.3.0/score_models/layers/ddpm_resnet_block.py` & `score_models-0.4.0/score_models/layers/ddpm_resnet_block.py`

 * *Files identical despite different names*

### Comparing `score_models-0.3.0/score_models/layers/downsample.py` & `score_models-0.4.0/score_models/layers/downsample.py`

 * *Files identical despite different names*

### Comparing `score_models-0.3.0/score_models/layers/ncsn_resnet_block.py` & `score_models-0.4.0/score_models/layers/ncsn_resnet_block.py`

 * *Files identical despite different names*

### Comparing `score_models-0.3.0/score_models/layers/projection_embedding.py` & `score_models-0.4.0/score_models/layers/projection_embedding.py`

 * *Files identical despite different names*

### Comparing `score_models-0.3.0/score_models/layers/resnet_block_biggan.py` & `score_models-0.4.0/score_models/layers/resnet_block_biggan.py`

 * *Files identical despite different names*

### Comparing `score_models-0.3.0/score_models/layers/spectral_normalization.py` & `score_models-0.4.0/score_models/layers/spectral_normalization.py`

 * *Files identical despite different names*

### Comparing `score_models-0.3.0/score_models/layers/squeeze_and_excitation.py` & `score_models-0.4.0/score_models/layers/squeeze_and_excitation.py`

 * *Files identical despite different names*

### Comparing `score_models-0.3.0/score_models/layers/style_gan_conv.py` & `score_models-0.4.0/score_models/layers/style_gan_conv.py`

 * *Files identical despite different names*

### Comparing `score_models-0.3.0/score_models/layers/up_or_downsampling.py` & `score_models-0.4.0/score_models/layers/up_or_downsampling.py`

 * *Files identical despite different names*

### Comparing `score_models-0.3.0/score_models/layers/up_or_downsampling1d.py` & `score_models-0.4.0/score_models/layers/up_or_downsampling1d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.3.0/score_models/layers/up_or_downsampling2d.py` & `score_models-0.4.0/score_models/layers/up_or_downsampling2d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.3.0/score_models/layers/up_or_downsampling3d.py` & `score_models-0.4.0/score_models/layers/up_or_downsampling3d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.3.0/score_models/layers/upfirdn1d.py` & `score_models-0.4.0/score_models/layers/upfirdn1d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.3.0/score_models/layers/upfirdn2d.py` & `score_models-0.4.0/score_models/layers/upfirdn2d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.3.0/score_models/layers/upfirdn3d.py` & `score_models-0.4.0/score_models/layers/upfirdn3d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.3.0/score_models/layers/upsample.py` & `score_models-0.4.0/score_models/layers/upsample.py`

 * *Files identical despite different names*

### Comparing `score_models-0.3.0/score_models/score_model.py` & `score_models-0.4.0/score_models/score_model.py`

 * *Files identical despite different names*

### Comparing `score_models-0.3.0/score_models/sde/sde.py` & `score_models-0.4.0/score_models/sde/sde.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 from abc import ABC, abstractmethod
 from typing import Tuple
 
-import torch
+from torch.distributions import Normal, Independent
+from torch.distributions import Distribution
 from torch import Tensor
 
 class SDE(ABC):
     """
     Abstract class for some SDE info important for the score models
     """
     def __init__(self):
         super().__init__()
     
     @abstractmethod
     def sigma(self, t) -> Tensor:
         ...
     
     @abstractmethod
-    def prior(self, dimensions) -> Tensor:
+    def prior(self, shape) -> Distribution:
         """
-        Sample from the high temperature prior
+        High temperature distribution
         """
         ...
-
+    
     @abstractmethod
     def diffusion(self, t:Tensor, x: Tensor) -> Tensor:
         ...
 
     @abstractmethod
     def drift(self, t, x) -> Tensor:
         ...
     
     @abstractmethod
-    def marginal(self, x0: Tensor, t: Tensor) -> Tensor:
+    def marginal(self, t: Tensor, x0: Tensor) -> Tensor:
         """
         Sample from the marginal at time t given some initial condition x0
         """
         ...
 
     @abstractmethod
     def marginal_prob_scalars(self, t) -> Tuple[Tensor, Tensor]:
```

### Comparing `score_models-0.3.0/score_models/sde/vesde.py` & `score_models-0.4.0/score_models/sde/vesde.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import torch
 from .sde import SDE
 from torch import Tensor
 import numpy as np
+from torch.distributions import Normal, Independent
 
 
 class VESDE(SDE):
     def __init__(
             self,
             sigma_min: float,
             sigma_max: float,
@@ -22,18 +23,27 @@
         super().__init__()
         self.sigma_min = sigma_min
         self.sigma_max = sigma_max
 
     def sigma(self, t: Tensor) -> Tensor:
         return self.sigma_min * (self.sigma_max / self.sigma_min) ** t
     
-    def prior(self, dimensions):
-        return torch.randn(dimensions) * self.sigma_max
+    def prior(self, shape, mu=None):
+        """
+        Technically, VESDE does not change the mean of the 0 temperature distribution, 
+        so I give the option to provide for more accuracy. In practice, 
+        sigma_max is chosen large enough to make this choice irrelevant
+        """
+        if mu is None:
+            mu = torch.zeros(shape)
+        else:
+            assert mu.shape == shape 
+        return Independent(Normal(loc=mu, scale=self.sigma_max, validate_args=False), 1)
     
-    def marginal(self, x0: Tensor, t: Tensor) -> Tensor:
+    def marginal(self, t: Tensor, x0: Tensor) -> Tensor:
         _, *D = x0.shape
         z = torch.randn_like(x0)
         _, sigma_t = self.marginal_prob_scalars(t)
         return x0 + sigma_t.view(-1, *[1]*len(D)) * z
     
     def marginal_prob_scalars(self, t) -> tuple[Tensor, Tensor]:
         return torch.ones_like(t), self.sigma(t)
```

### Comparing `score_models-0.3.0/score_models/utils.py` & `score_models-0.4.0/score_models/utils.py`

 * *Files identical despite different names*

### Comparing `score_models-0.3.0/score_models.egg-info/PKG-INFO` & `score_models-0.4.0/score_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: score-models
-Version: 0.3.0
+Version: 0.4.0
 Summary: A simple pytorch interface for score model and basic diffusion.
 Home-page: https://github.com/AlexandreAdam/torch_score_models
 Author: Alexandre Adam
 Author-email: alexandre.adam@umontreal.ca
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
+License-File: LICENSE.txt
 
 =========================
 Score Models for Pytorch
 =========================
 
 .. image:: https://badge.fury.io/py/score_models.svg
    :target: https://badge.fury.io/py/score_models
@@ -67,15 +68,15 @@
    model = ScoreModelBase(model=net, beta_min=1e-2, beta_max=20, device="cuda")
 
    # NN Architectures support a Unet with 1D convolutions for time series input data
    net = NCSNpp(channels=1, nf=128, ch_mult=[2, 2, 2, 2], dimensions=1)
    # ... or 3D convolutions for videos/voxels
    net = NCSNpp(channels=1, nf=128, ch_mult=[2, 2, 2, 2], attention=False, dimensions=3)
    # You can also use a simpler MLP architecture
-   net = MLP(input_dimensions=dim, layers=4, units=100)
+   net = MLP(dimensions=dim, layers=4, units=100)
    # ... or Jonathan Ho's DDPM architecture
    net = DDPM(channels=1, dimensions=2, nf=128, ch_mult=[2, 2, 2, 2])
 
    # Train the model
    model.fit(dataset=your_dataset, epochs=100, learning_rate=1e-4)
 
    # Generate samples from the trained model
```

### Comparing `score_models-0.3.0/score_models.egg-info/SOURCES.txt` & `score_models-0.4.0/score_models.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+LICENSE.txt
 README.md
 pyproject.toml
 setup.py
 score_models/__init__.py
 score_models/base.py
 score_models/definitions.py
 score_models/score_model.py
+score_models/sliced_score_matching.py
 score_models/utils.py
 score_models.egg-info/PKG-INFO
 score_models.egg-info/SOURCES.txt
 score_models.egg-info/dependency_links.txt
 score_models.egg-info/requires.txt
 score_models.egg-info/top_level.txt
 score_models/architectures/__init__.py
@@ -43,9 +45,9 @@
 score_models/layers/upsample.py
 score_models/sde/__init__.py
 score_models/sde/sde.py
 score_models/sde/vesde.py
 score_models/sde/vpsde.py
 tests/test_architectures.py
 tests/test_layers.py
-tests/test_loading_score.py
+tests/test_score_models.py
 tests/test_training.py
```

### Comparing `score_models-0.3.0/setup.py` & `score_models-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of the README file
 with open("long_description.rst", "r") as fh:
     long_description = fh.read()
 
 setup(
 	name="score_models",
-	version="0.3.0",
+	version="0.4.0",
     description="A simple pytorch interface for score model and basic diffusion.",
     long_description=long_description,
     author="Alexandre Adam",
     author_email="alexandre.adam@umontreal.ca",
     url="https://github.com/AlexandreAdam/torch_score_models",
     packages=find_packages(),
     install_requires=[
```

### Comparing `score_models-0.3.0/tests/test_architectures.py` & `score_models-0.4.0/tests/test_architectures.py`

 * *Files identical despite different names*

### Comparing `score_models-0.3.0/tests/test_layers.py` & `score_models-0.4.0/tests/test_layers.py`

 * *Files identical despite different names*

### Comparing `score_models-0.3.0/tests/test_loading_score.py` & `score_models-0.4.0/tests/test_score_models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+from score_models.architectures.ddpm import DDPM
 import torch
 from score_models.utils import load_architecture
 from score_models import ScoreModel, EnergyModel
 from score_models.architectures import MLP, NCSNpp
 import pytest
 
 
-def local_test_loading_model():
+def local_test_loading_model_and_score_fn():
     # local test only
     path = "/home/alexandre/Desktop/Projects/data/score_models/ncsnpp_ct_g_220912024942"
     model, hparams = load_architecture(path)
     
     score = ScoreModel(checkpoints_directory=path)
     print(score.sde)
     x = torch.randn(1, 1, 256, 256)
@@ -45,12 +46,38 @@
     t = torch.ones(1)
     score(t, x)
 
 def test_init_score():
     net = MLP(10)
     with pytest.raises(KeyError):
         score = ScoreModel(net)
-    
+
+def test_log_likelihood():
+    net = MLP(dimensions=2)
+    score = ScoreModel(net, beta_min=1e-2, beta_max=10)
+    print(score.sde)
+    x = torch.randn(3, 2)
+    ll = score.log_likelihood(x, ode_steps=10, verbose=1, epsilon=1e-5)
+    print(ll)
+    assert ll.shape == torch.Size([3])
+
+def test_score_at_zero_t():
+    net = MLP(dimensions=2)
+    score = ScoreModel(net, beta_min=1e-2, beta_max=10)
+    print(score.sde)
+    x = torch.randn(3, 2)
+    ll, vjp_func = torch.func.vjp(lambda x: score.log_likelihood(x, ode_steps=10, epsilon=1e-5), x)
+    grad = vjp_func(torch.ones_like(ll))
+    print(grad)
+
+def test_sample_fn():
+    net = NCSNpp(1, nf=8, ch_mult=(2, 2))
+    score = ScoreModel(net, sigma_min=1e-2, sigma_max=10)
+    score.sample(5, shape=[1, 16, 16], steps=10)
+
+    net = DDPM(1, nf=32, ch_mult=(2, 2))
+    score = ScoreModel(net, beta_min=1e-2, beta_max=10)
+    score.sample(5, shape=[1, 16, 16], steps=10)
```

### Comparing `score_models-0.3.0/tests/test_training.py` & `score_models-0.4.0/tests/test_training.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import torch
 from torch.utils.data import TensorDataset
 from score_models import ScoreModel, EnergyModel, MLP
 
 def test_training_score():
     # Create a dummy dataset
-    # Assuming you have input features 'X' and target values 'y'
-    X = torch.randn(10, 10)  # Replace with your input features
+    X = torch.randn(10, 10)
 
     # Convert the data into a TensorDataset
     dataset = TensorDataset(X)
 
     hyperparameters = {
         "dimensions": 10,
         "units": 10,
@@ -52,16 +51,15 @@
         checkpoints_directory=checkpoints_directory, 
         seed=seed
         )
     print(losses)
 
 def test_training_energy():
     # Create a dummy dataset
-    # Assuming you have input features 'X' and target values 'y'
-    X = torch.randn(10, 10)  # Replace with your input features
+    X = torch.randn(10, 10)
 
     # Convert the data into a TensorDataset
     dataset = TensorDataset(X)
 
     hyperparameters = {
         "dimensions": 10,
         "units": 10,
```

