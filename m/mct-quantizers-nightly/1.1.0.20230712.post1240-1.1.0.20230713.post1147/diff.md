# Comparing `tmp/mct-quantizers-nightly-1.1.0.20230712.post1240.tar.gz` & `tmp/mct-quantizers-nightly-1.1.0.20230713.post1147.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mct-quantizers-nightly-1.1.0.20230712.post1240.tar", last modified: Wed Jul 12 00:12:41 2023, max compression
+gzip compressed data, was "mct-quantizers-nightly-1.1.0.20230713.post1147.tar", last modified: Thu Jul 13 00:11:47 2023, max compression
```

## Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240.tar` & `mct-quantizers-nightly-1.1.0.20230713.post1147.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:12:41.371537 mct-quantizers-nightly-1.1.0.20230712.post1240/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-12 00:12:41.371537 mct-quantizers-nightly-1.1.0.20230712.post1240/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:12:41.367537 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:12:41.367537 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/common/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/common/base_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/common/get_all_subclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/common/get_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/common/quant_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/common/quant_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:12:41.367537 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/activation_quantization_holder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/load_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:12:41.367537 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:12:41.367537 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/quantizers/activation_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8074 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:12:41.367537 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/quantizers/weights_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/validation_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:12:41.367537 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/activation_quantization_holder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/load_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:12:41.371537 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:12:41.371537 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:12:41.371537 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-07-12 00:12:25.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:12:41.371537 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-12 00:12:41.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-12 00:12:41.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 00:12:41.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 00:12:41.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-12 00:12:41.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-12 00:12:41.371537 mct-quantizers-nightly-1.1.0.20230712.post1240/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-12 00:12:40.000000 mct-quantizers-nightly-1.1.0.20230712.post1240/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:11:47.900499 mct-quantizers-nightly-1.1.0.20230713.post1147/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-13 00:11:47.900499 mct-quantizers-nightly-1.1.0.20230713.post1147/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:11:47.896499 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:11:47.896499 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/common/base_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/common/get_all_subclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/common/get_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/common/quant_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/common/quant_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:11:47.896499 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/activation_quantization_holder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantize_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:11:47.896499 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:11:47.896499 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/activation_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8074 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:11:47.900499 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/weights_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/validation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:11:47.900499 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/activation_quantization_holder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantize_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:11:47.900499 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:11:47.900499 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:11:47.900499 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:11:47.900499 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-13 00:11:47.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-13 00:11:47.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 00:11:47.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-13 00:11:47.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 00:11:47.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-13 00:11:47.900499 mct-quantizers-nightly-1.1.0.20230713.post1147/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-13 00:11:47.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/setup.py
```

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/LICENSE.md` & `mct-quantizers-nightly-1.1.0.20230713.post1147/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/PKG-INFO` & `mct-quantizers-nightly-1.1.0.20230713.post1147/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-quantizers-nightly
-Version: 1.1.0.20230712.post1240
+Version: 1.1.0.20230713.post1147
 Summary: Infrastructure for support neural networks compression
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT) Quantizers
         
         The MCT Quantizers library is an open-source library developed by researchers and engineers working at Sony Semiconductor Israel.
```

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/README.md` & `mct-quantizers-nightly-1.1.0.20230713.post1147/README.md`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/__init__.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/common/__init__.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/common/base_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/common/base_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/common/constants.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/common/constants.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/common/get_all_subclasses.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/common/get_all_subclasses.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/common/get_quantizers.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/common/get_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/common/quant_info.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/common/quant_info.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/common/quant_utils.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/common/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/__init__.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/activation_quantization_holder.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/activation_quantization_holder.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,24 +9,23 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-
 from mct_quantizers.common.base_inferable_quantizer import BaseInferableQuantizer
 from mct_quantizers.common.constants import ACTIVATION_HOLDER_QUANTIZER, FOUND_TF, TRAINING, STEPS
 from mct_quantizers.common.get_all_subclasses import get_all_subclasses
 from mct_quantizers.logger import Logger
 
 if FOUND_TF:
     import tensorflow as tf
     from tensorflow.python.util import tf_inspect
-    from keras.utils.control_flow_util import smart_cond
+    from tensorflow.python.keras.utils.control_flow_util import smart_cond
     from mct_quantizers.keras.quantizers import BaseKerasInferableQuantizer
 
     keras = tf.keras
 
 
     def _make_quantizer_fn(quantizer, x, training):
         """Use currying to return True/False specialized fns to the cond."""
```

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/load_model.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/load_model.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/quantize_wrapper.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantize_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from mct_quantizers.common.constants import FOUND_TF, WEIGHTS_QUANTIZERS, STEPS, LAYER, TRAINING
 from mct_quantizers.logger import Logger
 from mct_quantizers.common.get_all_subclasses import get_all_subclasses
 
 if FOUND_TF:
     import tensorflow as tf
     from tensorflow.python.util import tf_inspect
-    from keras.utils.control_flow_util import smart_cond
+    from tensorflow.python.keras.utils.control_flow_util import smart_cond
 
     from mct_quantizers.keras.quantizers import BaseKerasInferableQuantizer
 
     keras = tf.keras
 
     def _make_quantizer_fn(quantizer, x, training):
         """Use currying to return True/False specialized fns to the cond."""
```

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/quantizer_utils.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/quantizers/__init__.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/keras/validation_functions.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/validation_functions.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/logger.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/logger.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/__init__.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/activation_quantization_holder.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/activation_quantization_holder.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/load_model.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/load_model.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/quantize_wrapper.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantize_wrapper.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/quantizer_utils.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/quantizers/__init__.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers_nightly.egg-info/PKG-INFO` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-quantizers-nightly
-Version: 1.1.0.20230712.post1240
+Version: 1.1.0.20230713.post1147
 Summary: Infrastructure for support neural networks compression
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT) Quantizers
         
         The MCT Quantizers library is an open-source library developed by researchers and engineers working at Sony Semiconductor Israel.
```

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/mct_quantizers_nightly.egg-info/SOURCES.txt` & `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230712.post1240/setup.py` & `mct-quantizers-nightly-1.1.0.20230713.post1147/setup.py`

 * *Files identical despite different names*

