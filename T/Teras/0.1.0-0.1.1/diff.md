# Comparing `tmp/Teras-0.1.0.tar.gz` & `tmp/Teras-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Teras-0.1.0.tar", last modified: Thu Jul 13 20:58:34 2023, max compression
+gzip compressed data, was "Teras-0.1.1.tar", last modified: Fri Jul 14 19:44:00 2023, max compression
```

## Comparing `Teras-0.1.0.tar` & `Teras-0.1.1.tar`

### file list

```diff
@@ -1,143 +1,150 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:34.458654 Teras-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-07-13 20:57:25.000000 Teras-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-07-13 20:58:34.458654 Teras-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-07-13 20:57:25.000000 Teras-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:34.438654 Teras-0.1.0/Teras.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-07-13 20:58:34.000000 Teras-0.1.0/Teras.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-07-13 20:58:34.000000 Teras-0.1.0/Teras.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 20:58:34.000000 Teras-0.1.0/Teras.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-13 20:58:34.000000 Teras-0.1.0/Teras.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-13 20:58:34.000000 Teras-0.1.0/Teras.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-13 20:57:25.000000 Teras-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 20:58:34.458654 Teras-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-13 20:57:25.000000 Teras-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:34.438654 Teras-0.1.0/teras/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/activations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:34.438654 Teras-0.1.0/teras/config/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/config/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/config/saint.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/config/tabnet.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/config/tabtransformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:34.438654 Teras-0.1.0/teras/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/ensemble/bagging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/ensemble/stacking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:34.442654 Teras-0.1.0/teras/generative/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/generative/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:34.442654 Teras-0.1.0/teras/impute/
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/impute/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:34.442654 Teras-0.1.0/teras/layerflow/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layerflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:34.442654 Teras-0.1.0/teras/layerflow/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layerflow/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:34.442654 Teras-0.1.0/teras/layerflow/layers/common/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layerflow/layers/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layerflow/layers/common/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layerflow/layers/ctgan.py
--rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layerflow/layers/dnfnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layerflow/layers/ft_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layerflow/layers/gain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layerflow/layers/node.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layerflow/layers/pcgain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layerflow/layers/rtdl_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12570 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layerflow/layers/saint.py
--rw-r--r--   0 runner    (1001) docker     (123)    13271 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layerflow/layers/tabnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layerflow/layers/tabtransformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:34.446654 Teras-0.1.0/teras/layerflow/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layerflow/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layerflow/models/ctgan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layerflow/models/dnfnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12785 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layerflow/models/ft_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11602 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layerflow/models/gain.py
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layerflow/models/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    11671 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layerflow/models/pcgain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layerflow/models/rtdl_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    16088 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layerflow/models/saint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layerflow/models/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)    15114 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layerflow/models/tabnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    15468 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layerflow/models/tabtransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layerflow/models/tvae.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:34.450654 Teras-0.1.0/teras/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layers/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layers/activations_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:34.454654 Teras-0.1.0/teras/layers/common/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layers/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layers/common/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layers/common/head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layers/common/head_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layers/common/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layers/common/transformer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layers/ctgan.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layers/ctgan_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19482 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layers/dnfnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layers/dnfnet_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layers/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layers/embedding_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6230 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layers/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layers/encoding_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layers/ft_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layers/ft_transformer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layers/gain.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layers/gain_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12804 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layers/node.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layers/node_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layers/oenf.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layers/oenf_test.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layers/pcgain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layers/regularization.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layers/regularization_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layers/rtdl_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layers/rtdl_resnet_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    33470 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layers/saint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layers/saint_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    34959 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layers/tabnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layers/tabnet_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layers/tabtransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layers/tabtransformer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layers/tvae.py
--rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/layers/vime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:34.454654 Teras-0.1.0/teras/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/losses/ctgan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/losses/gain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/losses/pcgain.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/losses/saint.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/losses/tabnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/losses/tvae.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/losses/vime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:34.454654 Teras-0.1.0/teras/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26887 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/models/ctgan.py
--rw-r--r--   0 runner    (1001) docker     (123)    12347 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/models/dnfnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    18400 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/models/ft_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    24556 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/models/gain.py
--rw-r--r--   0 runner    (1001) docker     (123)    16994 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/models/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    23895 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/models/pcgain.py
--rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/models/rtdl_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    38387 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/models/saint.py
--rw-r--r--   0 runner    (1001) docker     (123)    39859 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/models/tabnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    37919 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/models/tabtransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13092 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/models/tvae.py
--rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/models/vime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:34.458654 Teras-0.1.0/teras/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:34.458654 Teras-0.1.0/teras/preprocessing/base/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/preprocessing/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/preprocessing/base/base_data_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    34509 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/preprocessing/ctgan.py
--rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/preprocessing/gain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/preprocessing/oenf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/preprocessing/pcgain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/preprocessing/tvae.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:34.458654 Teras-0.1.0/teras/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/utils/dnfnet.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/utils/gain.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/utils/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/utils/pcgain.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/utils/tabtransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12379 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-07-13 20:57:25.000000 Teras-0.1.0/teras/utils/vime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:44:00.869325 Teras-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-07-14 19:43:02.000000 Teras-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-07-14 19:44:00.869325 Teras-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-07-14 19:43:02.000000 Teras-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:44:00.853325 Teras-0.1.1/Teras.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-07-14 19:44:00.000000 Teras-0.1.1/Teras.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-07-14 19:44:00.000000 Teras-0.1.1/Teras.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 19:44:00.000000 Teras-0.1.1/Teras.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-14 19:44:00.000000 Teras-0.1.1/Teras.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 19:44:00.000000 Teras-0.1.1/Teras.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-14 19:43:02.000000 Teras-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 19:44:00.869325 Teras-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-14 19:43:02.000000 Teras-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:44:00.853325 Teras-0.1.1/teras/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/activations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:44:00.857325 Teras-0.1.1/teras/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/config/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/config/saint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/config/tabnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/config/tabtransformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:44:00.857325 Teras-0.1.1/teras/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/ensemble/bagging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/ensemble/stacking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:44:00.857325 Teras-0.1.1/teras/generative/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/generative/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:44:00.857325 Teras-0.1.1/teras/impute/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/impute/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:44:00.857325 Teras-0.1.1/teras/layerflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:44:00.857325 Teras-0.1.1/teras/layerflow/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:44:00.857325 Teras-0.1.1/teras/layerflow/layers/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/layers/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/layers/common/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/layers/ctgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/layers/dnfnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/layers/ft_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/layers/gain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/layers/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/layers/pcgain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/layers/rtdl_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12570 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/layers/saint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13271 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/layers/tabnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/layers/tabtransformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:44:00.861325 Teras-0.1.1/teras/layerflow/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/ctgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/dnfnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/dnfnet_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13412 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/ft_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/ft_transformer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11602 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/gain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/node_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11671 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/pcgain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/rtdl_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/rtdl_resnet_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16327 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/saint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/saint_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15754 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/tabnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/tabnet_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16123 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/tabtransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/tabtransformer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layerflow/models/tvae.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:44:00.865325 Teras-0.1.1/teras/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/activations_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:44:00.865325 Teras-0.1.1/teras/layers/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/common/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/common/head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/common/head_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/common/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/common/transformer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/ctgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/ctgan_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19482 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/dnfnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/dnfnet_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/embedding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6230 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/encoding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/ft_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/ft_transformer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/gain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/gain_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12804 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/node_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/oenf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/oenf_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/pcgain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/regularization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/regularization_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/rtdl_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/rtdl_resnet_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33470 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/saint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/saint_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34959 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/tabnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/tabnet_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/tabtransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/tabtransformer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/tvae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/layers/vime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:44:00.865325 Teras-0.1.1/teras/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/losses/ctgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/losses/gain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/losses/pcgain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/losses/saint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/losses/tabnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/losses/tvae.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/losses/vime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:44:00.865325 Teras-0.1.1/teras/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26887 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/models/ctgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12347 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/models/dnfnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18400 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/models/ft_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24556 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/models/gain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16994 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/models/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23895 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/models/pcgain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/models/rtdl_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38395 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/models/saint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39859 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/models/tabnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37919 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/models/tabtransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13092 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/models/tvae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/models/vime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:44:00.869325 Teras-0.1.1/teras/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:44:00.869325 Teras-0.1.1/teras/preprocessing/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/preprocessing/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/preprocessing/base/base_data_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34509 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/preprocessing/ctgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/preprocessing/gain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/preprocessing/oenf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/preprocessing/pcgain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/preprocessing/tvae.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:44:00.869325 Teras-0.1.1/teras/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/utils/dnfnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/utils/gain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/utils/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/utils/pcgain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/utils/tabtransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13046 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-07-14 19:43:02.000000 Teras-0.1.1/teras/utils/vime.py
```

### Comparing `Teras-0.1.0/LICENSE` & `Teras-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/PKG-INFO` & `Teras-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,45 +1,56 @@
 Metadata-Version: 2.1
 Name: Teras
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Unified Deep Learning Library for Tabular Data
 Author: Khawaja Abaid
 Author-email: Khawaja Abaid <khawaja.abaid@gmail.com>
 Project-URL: Homepage, https://github.com/KhawajaAbaid/teras
 Project-URL: Bug Tracker, https://github.com/KhawajaAbaid/teras/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Teras — A Unified Deep Learning Library for Tabualr Data
+# Teras — A Unified Deep Learning Library for Tabular Data
 
 Teras (short for Tabular Keras) is a unified deep learning library for Tabular Data that aims to be your one stop for everything related to deep learing with tabular data.
 
-It provides state of the art layers, models and arhitectures for all purposes, be it classificaiton, regression or even data generation and imputation using state of the art deep learning architectures. 
+It provides state of the art layers, models and arhitectures for all purposes, be it classification, regression or even data generation and imputation using state of the art deep learning architectures. 
 
 It also includes Preprocessing, Encoding and (Categorical and Numerical) Embedding layers. 
 
-While these state of the art architectures can be quite sophisticated, Teras, thanks to the increidble design of Keras, abstracts away all the complications and sophistication and makes it easy as ever to access those models and put them to use.
+While these state of the art architectures can be quite sophisticated, Teras, thanks to the incredible design of Keras, abstracts away all the complications and sophistication and makes it easy as ever to access those models and put them to use.
 
 Not only that, everything available is highly customizable and modular, allowing for all variety of use cases.
 
+## Installation:
+You can install Teras using pip as follows,
+```
+pip install teras
+```
+
 ## Getting Started
 Read our [Getting Started Guide](https://github.com/KhawajaAbaid/teras/blob/main/tutorials/getting_started.ipynb) to...*drum roll* get started with Teras.
 
+
+## Documentation:
+You can access the documentation on ReadTheDocs.io: https://teras.readthedocs.io/en/latest/index.html
+Only the front page is a little messy but rest of the documentation should be good — though a lot of works needs to be done in this regard.
+
 ## Usage
-Teras provieds two API for usage to satitate different levels of flexbility and accessbility needs:
+Teras provides two API for usage to satiate different levels of flexibility and accessibility needs:
 1. **Parametric API**: This is the default API, where user specifies values for parameters that are used in construction of any sub-layers or models within the architecture.
 ```
 from teras.models import TabNetClassifier
 
 model = TabNetClassifier(num_classes=2, features_metadata=features_metadata)
 ```
-2. **LayerFlow API**: It maximizes flexbility and minimizes interface. Here, the user can pass any sub-layers or models instances as arguments to the given architecture (model/layer). It can be accessed through `teras.layerflow`
+2. **LayerFlow API**: It maximizes flexibility and minimizes interface. Here, the user can pass any sub-layers or models instances as arguments to the given architecture (model/layer). It can be accessed through `teras.layerflow`
 ```
 from teras.layerflow.models import TabNetClassifier
 from teras.layerflow.layers import TabNetEncoder, TabNetClassificationHead
 
 encoder = TabNetEncoder()
 head = TabNetClassificationHead(num_classes=2)
 model = TabNetClassifier(features_metadata=features_metadata,
@@ -47,15 +58,15 @@
                          head=head)
 ```
 You can read more about the difference between the two in the Teras APIs section in the [Getting Started Guide](https://github.com/KhawajaAbaid/teras/blob/main/tutorials/getting_started.ipynb).
 
 ## Main Teras Modules
 Teras offers following main modules:
 
-1. `teras.layerflow`: It is the LayerFlow API, offering maximum flebility with minimal interface. It's an alternative to the default Parametric API. You can read more about the difference between the two in the Teras APIs section in the [Getting Started Guide](https://github.com/KhawajaAbaid/teras/blob/main/tutorials/getting_started.ipynb).
+1. `teras.layerflow`: It is the LayerFlow API, offering maximum flexibility with minimal interface. It's an alternative to the default Parametric API. You can read more about the difference between the two in the Teras APIs section in the [Getting Started Guide](https://github.com/KhawajaAbaid/teras/blob/main/tutorials/getting_started.ipynb).
 2. `teras.layers`: It contains all the layers for all of the architectures offered by Teras.
 3. `teras.models`: It contains all of the models of all the architectures types, be it Classificaiton, Regresssion etc offered by Teras.
 4. `teras.generative`: It contains state of the art models for Data Generation. (Currently it offers `CTGAN` and `TVAE`).
 5. `teras.impute`: It contains state of the art models for Data Imputation. (Currently it offers `GAIN` and `PCGAIN`)
 6. `teras.preprocessing`: It offers preprocessing classes for data transformation and data sampling that are required by highly sophisticated models specifically the data generation and imputation models.
 7. `teras.ensemble`: It is a work in progress and aims to offers ensembling techniques making it easier than ever to ensemble your deep learning models, such as using Bagging or Stacking. (Currently it offers very basic version of these.)
 8. `teras.utils`: It contains useful utility functions making life easier for Teras users
@@ -66,12 +77,12 @@
 1. Provide a uniform interface for all the different proposed architectures.
 2. Further bridge the gap between research and application.
 3. Be a one-stop for everything concerning deep learning for tabular data.
 4. Accelerate research in tabular domain of deep learning by making it easier for researchers to access, use and experiment with exisiting architectures — saving them lots of valuable time.
 
 
 ## Support
-If you find Teras useful, consider supporting the project. I've been working on this for the past ~3 months full time and plan to continue to do so. I also have many future plans for it but my currently laptop is quite old which makes it impossible for me to test highly demanding workflows let alone rapidly test and iterate. So your support will be very vital in the betterment of this project.
+If you find Teras useful, consider supporting the project. I've been working on this for the past ~3 months full time and plan to continue to do so. I also have many future plans for it but my current laptop is quite old which makes it impossible for me to test highly demanding workflows let alone rapidly test and iterate. So your support will be very vital in the betterment of this project.
 Thank you!
 
 [![BuyMeACoffee](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-ffdd00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black)](https://www.buymeacoffee.com/KhawajaAbaid)
 [![Patreon](https://img.shields.io/badge/Patreon-F96854?style=for-the-badge&logo=patreon&logoColor=white)](https://www.patreon.com/KhawajaAbaid)
```

### Comparing `Teras-0.1.0/README.md` & `Teras-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,42 @@
-# Teras — A Unified Deep Learning Library for Tabualr Data
+# Teras — A Unified Deep Learning Library for Tabular Data
 
 Teras (short for Tabular Keras) is a unified deep learning library for Tabular Data that aims to be your one stop for everything related to deep learing with tabular data.
 
-It provides state of the art layers, models and arhitectures for all purposes, be it classificaiton, regression or even data generation and imputation using state of the art deep learning architectures. 
+It provides state of the art layers, models and arhitectures for all purposes, be it classification, regression or even data generation and imputation using state of the art deep learning architectures. 
 
 It also includes Preprocessing, Encoding and (Categorical and Numerical) Embedding layers. 
 
-While these state of the art architectures can be quite sophisticated, Teras, thanks to the increidble design of Keras, abstracts away all the complications and sophistication and makes it easy as ever to access those models and put them to use.
+While these state of the art architectures can be quite sophisticated, Teras, thanks to the incredible design of Keras, abstracts away all the complications and sophistication and makes it easy as ever to access those models and put them to use.
 
 Not only that, everything available is highly customizable and modular, allowing for all variety of use cases.
 
+## Installation:
+You can install Teras using pip as follows,
+```
+pip install teras
+```
+
 ## Getting Started
 Read our [Getting Started Guide](https://github.com/KhawajaAbaid/teras/blob/main/tutorials/getting_started.ipynb) to...*drum roll* get started with Teras.
 
+
+## Documentation:
+You can access the documentation on ReadTheDocs.io: https://teras.readthedocs.io/en/latest/index.html
+Only the front page is a little messy but rest of the documentation should be good — though a lot of works needs to be done in this regard.
+
 ## Usage
-Teras provieds two API for usage to satitate different levels of flexbility and accessbility needs:
+Teras provides two API for usage to satiate different levels of flexibility and accessibility needs:
 1. **Parametric API**: This is the default API, where user specifies values for parameters that are used in construction of any sub-layers or models within the architecture.
 ```
 from teras.models import TabNetClassifier
 
 model = TabNetClassifier(num_classes=2, features_metadata=features_metadata)
 ```
-2. **LayerFlow API**: It maximizes flexbility and minimizes interface. Here, the user can pass any sub-layers or models instances as arguments to the given architecture (model/layer). It can be accessed through `teras.layerflow`
+2. **LayerFlow API**: It maximizes flexibility and minimizes interface. Here, the user can pass any sub-layers or models instances as arguments to the given architecture (model/layer). It can be accessed through `teras.layerflow`
 ```
 from teras.layerflow.models import TabNetClassifier
 from teras.layerflow.layers import TabNetEncoder, TabNetClassificationHead
 
 encoder = TabNetEncoder()
 head = TabNetClassificationHead(num_classes=2)
 model = TabNetClassifier(features_metadata=features_metadata,
@@ -33,15 +44,15 @@
                          head=head)
 ```
 You can read more about the difference between the two in the Teras APIs section in the [Getting Started Guide](https://github.com/KhawajaAbaid/teras/blob/main/tutorials/getting_started.ipynb).
 
 ## Main Teras Modules
 Teras offers following main modules:
 
-1. `teras.layerflow`: It is the LayerFlow API, offering maximum flebility with minimal interface. It's an alternative to the default Parametric API. You can read more about the difference between the two in the Teras APIs section in the [Getting Started Guide](https://github.com/KhawajaAbaid/teras/blob/main/tutorials/getting_started.ipynb).
+1. `teras.layerflow`: It is the LayerFlow API, offering maximum flexibility with minimal interface. It's an alternative to the default Parametric API. You can read more about the difference between the two in the Teras APIs section in the [Getting Started Guide](https://github.com/KhawajaAbaid/teras/blob/main/tutorials/getting_started.ipynb).
 2. `teras.layers`: It contains all the layers for all of the architectures offered by Teras.
 3. `teras.models`: It contains all of the models of all the architectures types, be it Classificaiton, Regresssion etc offered by Teras.
 4. `teras.generative`: It contains state of the art models for Data Generation. (Currently it offers `CTGAN` and `TVAE`).
 5. `teras.impute`: It contains state of the art models for Data Imputation. (Currently it offers `GAIN` and `PCGAIN`)
 6. `teras.preprocessing`: It offers preprocessing classes for data transformation and data sampling that are required by highly sophisticated models specifically the data generation and imputation models.
 7. `teras.ensemble`: It is a work in progress and aims to offers ensembling techniques making it easier than ever to ensemble your deep learning models, such as using Bagging or Stacking. (Currently it offers very basic version of these.)
 8. `teras.utils`: It contains useful utility functions making life easier for Teras users
@@ -52,12 +63,12 @@
 1. Provide a uniform interface for all the different proposed architectures.
 2. Further bridge the gap between research and application.
 3. Be a one-stop for everything concerning deep learning for tabular data.
 4. Accelerate research in tabular domain of deep learning by making it easier for researchers to access, use and experiment with exisiting architectures — saving them lots of valuable time.
 
 
 ## Support
-If you find Teras useful, consider supporting the project. I've been working on this for the past ~3 months full time and plan to continue to do so. I also have many future plans for it but my currently laptop is quite old which makes it impossible for me to test highly demanding workflows let alone rapidly test and iterate. So your support will be very vital in the betterment of this project.
+If you find Teras useful, consider supporting the project. I've been working on this for the past ~3 months full time and plan to continue to do so. I also have many future plans for it but my current laptop is quite old which makes it impossible for me to test highly demanding workflows let alone rapidly test and iterate. So your support will be very vital in the betterment of this project.
 Thank you!
 
 [![BuyMeACoffee](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-ffdd00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black)](https://www.buymeacoffee.com/KhawajaAbaid)
 [![Patreon](https://img.shields.io/badge/Patreon-F96854?style=for-the-badge&logo=patreon&logoColor=white)](https://www.patreon.com/KhawajaAbaid)
```

### Comparing `Teras-0.1.0/Teras.egg-info/PKG-INFO` & `Teras-0.1.1/Teras.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,45 +1,56 @@
 Metadata-Version: 2.1
 Name: Teras
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Unified Deep Learning Library for Tabular Data
 Author: Khawaja Abaid
 Author-email: Khawaja Abaid <khawaja.abaid@gmail.com>
 Project-URL: Homepage, https://github.com/KhawajaAbaid/teras
 Project-URL: Bug Tracker, https://github.com/KhawajaAbaid/teras/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Teras — A Unified Deep Learning Library for Tabualr Data
+# Teras — A Unified Deep Learning Library for Tabular Data
 
 Teras (short for Tabular Keras) is a unified deep learning library for Tabular Data that aims to be your one stop for everything related to deep learing with tabular data.
 
-It provides state of the art layers, models and arhitectures for all purposes, be it classificaiton, regression or even data generation and imputation using state of the art deep learning architectures. 
+It provides state of the art layers, models and arhitectures for all purposes, be it classification, regression or even data generation and imputation using state of the art deep learning architectures. 
 
 It also includes Preprocessing, Encoding and (Categorical and Numerical) Embedding layers. 
 
-While these state of the art architectures can be quite sophisticated, Teras, thanks to the increidble design of Keras, abstracts away all the complications and sophistication and makes it easy as ever to access those models and put them to use.
+While these state of the art architectures can be quite sophisticated, Teras, thanks to the incredible design of Keras, abstracts away all the complications and sophistication and makes it easy as ever to access those models and put them to use.
 
 Not only that, everything available is highly customizable and modular, allowing for all variety of use cases.
 
+## Installation:
+You can install Teras using pip as follows,
+```
+pip install teras
+```
+
 ## Getting Started
 Read our [Getting Started Guide](https://github.com/KhawajaAbaid/teras/blob/main/tutorials/getting_started.ipynb) to...*drum roll* get started with Teras.
 
+
+## Documentation:
+You can access the documentation on ReadTheDocs.io: https://teras.readthedocs.io/en/latest/index.html
+Only the front page is a little messy but rest of the documentation should be good — though a lot of works needs to be done in this regard.
+
 ## Usage
-Teras provieds two API for usage to satitate different levels of flexbility and accessbility needs:
+Teras provides two API for usage to satiate different levels of flexibility and accessibility needs:
 1. **Parametric API**: This is the default API, where user specifies values for parameters that are used in construction of any sub-layers or models within the architecture.
 ```
 from teras.models import TabNetClassifier
 
 model = TabNetClassifier(num_classes=2, features_metadata=features_metadata)
 ```
-2. **LayerFlow API**: It maximizes flexbility and minimizes interface. Here, the user can pass any sub-layers or models instances as arguments to the given architecture (model/layer). It can be accessed through `teras.layerflow`
+2. **LayerFlow API**: It maximizes flexibility and minimizes interface. Here, the user can pass any sub-layers or models instances as arguments to the given architecture (model/layer). It can be accessed through `teras.layerflow`
 ```
 from teras.layerflow.models import TabNetClassifier
 from teras.layerflow.layers import TabNetEncoder, TabNetClassificationHead
 
 encoder = TabNetEncoder()
 head = TabNetClassificationHead(num_classes=2)
 model = TabNetClassifier(features_metadata=features_metadata,
@@ -47,15 +58,15 @@
                          head=head)
 ```
 You can read more about the difference between the two in the Teras APIs section in the [Getting Started Guide](https://github.com/KhawajaAbaid/teras/blob/main/tutorials/getting_started.ipynb).
 
 ## Main Teras Modules
 Teras offers following main modules:
 
-1. `teras.layerflow`: It is the LayerFlow API, offering maximum flebility with minimal interface. It's an alternative to the default Parametric API. You can read more about the difference between the two in the Teras APIs section in the [Getting Started Guide](https://github.com/KhawajaAbaid/teras/blob/main/tutorials/getting_started.ipynb).
+1. `teras.layerflow`: It is the LayerFlow API, offering maximum flexibility with minimal interface. It's an alternative to the default Parametric API. You can read more about the difference between the two in the Teras APIs section in the [Getting Started Guide](https://github.com/KhawajaAbaid/teras/blob/main/tutorials/getting_started.ipynb).
 2. `teras.layers`: It contains all the layers for all of the architectures offered by Teras.
 3. `teras.models`: It contains all of the models of all the architectures types, be it Classificaiton, Regresssion etc offered by Teras.
 4. `teras.generative`: It contains state of the art models for Data Generation. (Currently it offers `CTGAN` and `TVAE`).
 5. `teras.impute`: It contains state of the art models for Data Imputation. (Currently it offers `GAIN` and `PCGAIN`)
 6. `teras.preprocessing`: It offers preprocessing classes for data transformation and data sampling that are required by highly sophisticated models specifically the data generation and imputation models.
 7. `teras.ensemble`: It is a work in progress and aims to offers ensembling techniques making it easier than ever to ensemble your deep learning models, such as using Bagging or Stacking. (Currently it offers very basic version of these.)
 8. `teras.utils`: It contains useful utility functions making life easier for Teras users
@@ -66,12 +77,12 @@
 1. Provide a uniform interface for all the different proposed architectures.
 2. Further bridge the gap between research and application.
 3. Be a one-stop for everything concerning deep learning for tabular data.
 4. Accelerate research in tabular domain of deep learning by making it easier for researchers to access, use and experiment with exisiting architectures — saving them lots of valuable time.
 
 
 ## Support
-If you find Teras useful, consider supporting the project. I've been working on this for the past ~3 months full time and plan to continue to do so. I also have many future plans for it but my currently laptop is quite old which makes it impossible for me to test highly demanding workflows let alone rapidly test and iterate. So your support will be very vital in the betterment of this project.
+If you find Teras useful, consider supporting the project. I've been working on this for the past ~3 months full time and plan to continue to do so. I also have many future plans for it but my current laptop is quite old which makes it impossible for me to test highly demanding workflows let alone rapidly test and iterate. So your support will be very vital in the betterment of this project.
 Thank you!
 
 [![BuyMeACoffee](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-ffdd00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black)](https://www.buymeacoffee.com/KhawajaAbaid)
 [![Patreon](https://img.shields.io/badge/Patreon-F96854?style=for-the-badge&logo=patreon&logoColor=white)](https://www.patreon.com/KhawajaAbaid)
```

### Comparing `Teras-0.1.0/Teras.egg-info/SOURCES.txt` & `Teras-0.1.1/Teras.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -32,23 +32,30 @@
 teras/layerflow/layers/tabnet.py
 teras/layerflow/layers/tabtransformer.py
 teras/layerflow/layers/common/__init__.py
 teras/layerflow/layers/common/transformer.py
 teras/layerflow/models/__init__.py
 teras/layerflow/models/ctgan.py
 teras/layerflow/models/dnfnet.py
+teras/layerflow/models/dnfnet_test.py
 teras/layerflow/models/ft_transformer.py
+teras/layerflow/models/ft_transformer_test.py
 teras/layerflow/models/gain.py
 teras/layerflow/models/node.py
+teras/layerflow/models/node_test.py
 teras/layerflow/models/pcgain.py
 teras/layerflow/models/rtdl_resnet.py
+teras/layerflow/models/rtdl_resnet_test.py
 teras/layerflow/models/saint.py
+teras/layerflow/models/saint_test.py
 teras/layerflow/models/simple.py
 teras/layerflow/models/tabnet.py
+teras/layerflow/models/tabnet_test.py
 teras/layerflow/models/tabtransformer.py
+teras/layerflow/models/tabtransformer_test.py
 teras/layerflow/models/tvae.py
 teras/layers/__init__.py
 teras/layers/activations.py
 teras/layers/activations_test.py
 teras/layers/ctgan.py
 teras/layers/ctgan_test.py
 teras/layers/dnfnet.py
```

### Comparing `Teras-0.1.0/pyproject.toml` & `Teras-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0", "tensorflow", "tensorflow-probability",
             "tensorflow-addons", "pandas", "numpy", "tqdm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Teras"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Khawaja Abaid", email="khawaja.abaid@gmail.com" },
 ]
 description = "A Unified Deep Learning Library for Tabular Data"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `Teras-0.1.0/teras/__init__.py` & `Teras-0.1.1/teras/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/config/__init__.py` & `Teras-0.1.1/teras/config/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/config/base.py` & `Teras-0.1.1/teras/config/base.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/config/saint.py` & `Teras-0.1.1/teras/config/saint.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/config/tabnet.py` & `Teras-0.1.1/teras/config/tabnet.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/ensemble/__init__.py` & `Teras-0.1.1/teras/ensemble/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/ensemble/bagging.py` & `Teras-0.1.1/teras/ensemble/bagging.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/ensemble/stacking.py` & `Teras-0.1.1/teras/ensemble/stacking.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/generative/__init__.py` & `Teras-0.1.1/teras/generative/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/impute/__init__.py` & `Teras-0.1.1/teras/impute/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layerflow/__init__.py` & `Teras-0.1.1/teras/layerflow/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layerflow/layers/__init__.py` & `Teras-0.1.1/teras/layerflow/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layerflow/layers/common/__init__.py` & `Teras-0.1.1/teras/layerflow/layers/common/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layerflow/layers/common/transformer.py` & `Teras-0.1.1/teras/layerflow/layers/common/transformer.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layerflow/layers/dnfnet.py` & `Teras-0.1.1/teras/layerflow/layers/dnfnet.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layerflow/layers/ft_transformer.py` & `Teras-0.1.1/teras/layerflow/layers/ft_transformer.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layerflow/layers/node.py` & `Teras-0.1.1/teras/layerflow/layers/node.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layerflow/layers/rtdl_resnet.py` & `Teras-0.1.1/teras/layerflow/layers/rtdl_resnet.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layerflow/layers/saint.py` & `Teras-0.1.1/teras/layerflow/layers/saint.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layerflow/layers/tabnet.py` & `Teras-0.1.1/teras/layerflow/layers/tabnet.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layerflow/layers/tabtransformer.py` & `Teras-0.1.1/teras/layerflow/layers/tabtransformer.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layerflow/models/__init__.py` & `Teras-0.1.1/teras/layerflow/models/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layerflow/models/ctgan.py` & `Teras-0.1.1/teras/layerflow/models/ctgan.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layerflow/models/dnfnet.py` & `Teras-0.1.1/teras/layerflow/models/dnfnet.py`

 * *Files 16% similar despite different names*

```diff
@@ -85,15 +85,23 @@
                 >>> from teras.layerflow.layers import DNFNetClassificationHead
     """
     def __init__(self,
                  dnnf_layers: PACK_OF_LAYERS = None,
                  head: layers.Layer = None,
                  **kwargs):
         if head is None:
-            head = DNFNetClassificationHead()
+            num_classes = 2
+            activation_out = None
+            if "num_classes" in kwargs:
+                num_classes = kwargs.pop("num_classes")
+            if "activation_out" in kwargs:
+                activation_out = kwargs.pop("activation_out")
+            head = DNFNetClassificationHead(num_classes=num_classes,
+                                            activation_out=activation_out,
+                                            name="dnfnet_classification_head")
         super().__init__(dnnf_layers=dnnf_layers,
                          head=head,
                          **kwargs)
 
 
 class DNFNetRegressor(DNFNet):
     """
@@ -118,11 +126,15 @@
                 >>> from teras.layerflow.layers import DNFNetRegressionHead
     """
     def __init__(self,
                  dnnf_layers: PACK_OF_LAYERS = None,
                  head: layers.Layer = None,
                  **kwargs):
         if head is None:
-            head = DNFNetRegressionHead()
+            num_outputs = 1
+            if "num_outputs" in kwargs:
+                num_outputs = kwargs.pop("num_outputs")
+            head = DNFNetRegressionHead(num_outputs=num_outputs,
+                                        name="dnfnet_regression_head")
         super().__init__(dnnf_layers=dnnf_layers,
                          head=head,
                          **kwargs)
```

### Comparing `Teras-0.1.0/teras/layerflow/models/ft_transformer.py` & `Teras-0.1.1/teras/layerflow/models/ft_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
                       'encoder': keras.layers.serialize(self.encoder),
                       'head': keras.layers.serialize(self.head),
                       }
         config.update(new_config)
         return config
 
 
-class FTTransformerClassifier(_BaseFTTransformerClassifier):
+class FTTransformerClassifier(FTTransformer):
     """
     FTTransformerClassifier architecture with LayrFlow design.
     It is based on the FT-Transformer architecture proposed by Yury Gorishniy et al.
     in the paper Revisiting Deep Learning Models for Tabular Data
     in their FTTransformer architecture.
 
     Reference(s):
@@ -148,25 +148,33 @@
                  categorical_feature_embedding: layers.Layer = None,
                  numerical_feature_embedding: layers.Layer = None,
                  cls_token: layers.Layer = None,
                  encoder: layers.Layer = None,
                  head: layers.Layer = None,
                  **kwargs):
         if head is None:
-            head = ClassificationHead()
+            num_classes = 2
+            activation_out = None
+            if "num_classes" in kwargs:
+                num_classes = kwargs.pop("num_classes")
+            if "activation_out" in kwargs:
+                activation_out = kwargs.pop("activation_out")
+            head = ClassificationHead(num_classes=num_classes,
+                                      activation_out=activation_out,
+                                      name="ft_transformer_classification_head")
         super().__init__(features_metadata=features_metadata,
                          categorical_feature_embedding=categorical_feature_embedding,
                          numerical_feature_embedding=numerical_feature_embedding,
                          cls_token=cls_token,
                          encoder=encoder,
                          head=head,
                          **kwargs)
 
 
-class FTTransformerRegressor(_BaseFTTransformerRegressor):
+class FTTransformerRegressor(FTTransformer):
     """
     FTTransformerRegressor architecture with LayrFlow design.
     It is based on the FT-Transformer architecture proposed by Yury Gorishniy et al.
     in the paper Revisiting Deep Learning Models for Tabular Data
     in their FTTransformer architecture.
 
     Reference(s):
@@ -218,15 +226,19 @@
                  categorical_feature_embedding: layers.Layer = None,
                  numerical_feature_embedding: layers.Layer = None,
                  cls_token: layers.Layer = None,
                  encoder: layers.Layer = None,
                  head: layers.Layer = None,
                  **kwargs):
         if head is None:
-            head = RegressionHead()
+            num_outputs = 1
+            if "num_outputs" in kwargs:
+                num_outputs = kwargs.pop("num_outputs")
+            head = RegressionHead(num_outputs=num_outputs,
+                                  name="ft_transformer_regression_head")
         super().__init__(features_metadata=features_metadata,
                          categorical_feature_embedding=categorical_feature_embedding,
                          numerical_feature_embedding=numerical_feature_embedding,
                          cls_token=cls_token,
                          encoder=encoder,
                          head=head,
                          **kwargs)
```

### Comparing `Teras-0.1.0/teras/layerflow/models/gain.py` & `Teras-0.1.1/teras/layerflow/models/gain.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layerflow/models/node.py` & `Teras-0.1.1/teras/layerflow/models/node.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from tensorflow import keras
 from tensorflow.keras import layers, models
 from teras.models import NODE as _BaseNODE
-from teras.layerflow.layers import NODEClassificationHead, NODERegressionHead
+from teras.layers import NODEClassificationHead, NODERegressionHead
 from typing import List
 from teras.utils import serialize_layers_collection
 
 LIST_OF_LAYERS = List[layers.Layer]
 
 
 class NODE(_BaseNODE):
@@ -95,15 +95,23 @@
     def __init__(self,
                  tree_layers: LIST_OF_LAYERS = None,
                  head: layers.Layer = None,
                  max_features: int = None,
                  input_dropout: float = 0.,
                  **kwargs):
         if head is None:
-            head = NODEClassificationHead()
+            num_classes = 2
+            activation_out = None
+            if "num_classes" in kwargs:
+                num_classes = kwargs.pop("num_classes")
+            if "activation_out" in kwargs:
+                activation_out = kwargs.pop("activation_out")
+            head = NODEClassificationHead(num_classes=num_classes,
+                                          activation_out=activation_out,
+                                          name="node_classification_head")
         super().__init__(tree_layers=tree_layers,
                          head=head,
                          max_features=max_features,
                          input_dropout=input_dropout,
                          **kwargs)
 
 
@@ -139,13 +147,17 @@
     def __init__(self,
                  tree_layers: LIST_OF_LAYERS = None,
                  head: layers.Layer = None,
                  max_features: int = None,
                  input_dropout: float = 0.,
                  **kwargs):
         if head is None:
-            head = NODERegressionHead()
+            num_outputs = 1
+            if "num_outputs" in kwargs:
+                num_outputs = kwargs.pop("num_outputs")
+            head = NODERegressionHead(num_outputs=num_outputs,
+                                      name="node_regression_head")
         super().__init__(tree_layers=tree_layers,
                          head=head,
                          max_features=max_features,
                          input_dropout=input_dropout,
                          **kwargs)
```

### Comparing `Teras-0.1.0/teras/layerflow/models/pcgain.py` & `Teras-0.1.1/teras/layerflow/models/pcgain.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layerflow/models/rtdl_resnet.py` & `Teras-0.1.1/teras/layerflow/models/rtdl_resnet.py`

 * *Files 22% similar despite different names*

```diff
@@ -79,15 +79,23 @@
                 >>> from teras.layerflow.layers import RTDLResNetClassificationHead
     """
     def __init__(self,
                  resnet_blocks: LAYER_OR_MODEL = None,
                  head: layers.Layer = None,
                  **kwargs):
         if head is None:
-            head = RTDLResNetClassificationHead()
+            num_classes = 2
+            activation_out = None
+            if "num_classes" in kwargs:
+                num_classes = kwargs.pop("num_classes")
+            if "activation_out" in kwargs:
+                activation_out = kwargs.pop("activation_out")
+            head = RTDLResNetClassificationHead(num_classes=num_classes,
+                                          activation_out=activation_out,
+                                          name="rtdl_resnet_classification_head")
         super().__init__(resnet_blocks=resnet_blocks,
                          head=head,
                          **kwargs)
 
 
 class RTDLResNetRegressor(RTDLResNet):
     """
@@ -113,11 +121,15 @@
                 >>> from teras.layerflow.layers import RTDLResNetRegressionHead
     """
     def __init__(self,
                  resnet_blocks: LAYER_OR_MODEL = None,
                  head: layers.Layer = None,
                  **kwargs):
         if head is None:
-            head = RTDLResNetRegressionHead()
+            num_outputs = 1
+            if "num_outputs" in kwargs:
+                num_outputs = kwargs.pop("num_outputs")
+            head = RTDLResNetRegressionHead(num_outputs=num_outputs,
+                                            name="rtdl_resnet_regression_head")
         super().__init__(resnet_blocks=resnet_blocks,
                          head=head,
                          **kwargs)
```

### Comparing `Teras-0.1.0/teras/layerflow/models/saint.py` & `Teras-0.1.1/teras/layerflow/models/saint.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from tensorflow import keras
 from tensorflow.keras import layers, models
 from teras.models import (SAINT as _BaseSAINT,
-                          SAINTClassifier as _BaseSAINTClassifier,
-                          SAINTRegressor as _BaseSAINTRegressor,
                           SAINTPretrainer as _BaseSAINTPretrainer)
 from teras.layerflow.layers.saint import ClassificationHead, RegressionHead
 
 
 class SAINT(_BaseSAINT):
     """
     SAINT architecture with LayerFlow design.
@@ -56,44 +54,44 @@
         head: `layers.Layer`,
             An instance of ClassificationHead or RegressionHead layer for final outputs,
             or any layer that can work in place of a Head layer for that purpose.
     """
     def __init__(self,
                  features_metadata: dict,
                  categorical_feature_embedding: layers.Layer = None,
-                 saint_numerical_feature_embedding: layers.Layer = None,
-                 saint_encoder: layers.Layer = None,
+                 numerical_feature_embedding: layers.Layer = None,
+                 encoder: layers.Layer = None,
                  head: layers.Layer = None,
                  **kwargs):
         super().__init__(features_metadata=features_metadata,
                          **kwargs)
         if categorical_feature_embedding is not None:
             self.categorical_feature_embedding = categorical_feature_embedding
 
-        if saint_numerical_feature_embedding is not None:
-            self.numerical_feature_embedding = saint_numerical_feature_embedding
+        if numerical_feature_embedding is not None:
+            self.numerical_feature_embedding = numerical_feature_embedding
 
-        if saint_encoder is not None:
-            self.saint_encoder = saint_encoder
+        if encoder is not None:
+            self.encoder = encoder
 
         if head is not None:
             self.head = head
 
     def get_config(self):
         config = super().get_config()
         new_config = {'categorical_feature_embedding': keras.layers.serialize(self.categorical_feature_embedding),
-                      'saint_numerical_feature_embedding': keras.layers.serialize(self.saint_numerical_feature_embedding),
-                      'saint_encoder': keras.layers.serialize(self.saint_encoder),
+                      'numerical_feature_embedding': keras.layers.serialize(self.numerical_feature_embedding),
+                      'encoder': keras.layers.serialize(self.encoder),
                       'head': keras.layers.serialize(self.head),
                       }
         config.update(new_config)
         return config
 
 
-class SAINTClassifier(_BaseSAINTClassifier):
+class SAINTClassifier(SAINT):
     """
     SAINTClassifier with LayerFlow design.
     It is based on the SAINT architecture proposed by Gowthami Somepalli et al.
     in the paper,
     SAINT: Improved Neural Networks for Tabular Data
     via Row Attention and Contrastive Pre-Training.
 
@@ -143,28 +141,35 @@
             You can import the `SAINTClassificationHead` layer as follows,
                 >>> from teras.layerflow.layers import SAINTClassificationHead
     """
     def __init__(self,
                  features_metadata: dict,
                  categorical_feature_embedding: layers.Layer = None,
                  numerical_feature_embedding: layers.Layer = None,
-                 saint_encoder: layers.Layer = None,
+                 encoder: layers.Layer = None,
                  head: layers.Layer = None,
                  **kwargs):
         if head is None:
-            head = ClassificationHead()
+            num_classes = 2
+            activation_out = None
+            if "num_classes" in kwargs:
+                num_classes = kwargs.pop("num_classes")
+            if "activation_out" in kwargs:
+                activation_out = kwargs.pop("activation_out")
+            head = ClassificationHead(num_classes=num_classes,
+                                      activation_out=activation_out)
         super().__init__(features_metadata=features_metadata,
                          categorical_feature_embedding=categorical_feature_embedding,
                          numerical_feature_embedding=numerical_feature_embedding,
-                         saint_encoder=saint_encoder,
+                         encoder=encoder,
                          head=head,
                          **kwargs)
 
 
-class SAINTRegressor(_BaseSAINTRegressor):
+class SAINTRegressor(SAINT):
     """
     SAINTClassifier with LayerFlow design.
     It is based on the SAINT architecture proposed by Gowthami Somepalli et al.
     in the paper,
     SAINT: Improved Neural Networks for Tabular Data
     via Row Attention and Contrastive Pre-Training.
 
@@ -215,23 +220,26 @@
                 >>> from teras.layerflow.layers import SAINTRegressionHead
 
     """
     def __init__(self,
                  features_metadata: dict,
                  categorical_feature_embedding: layers.Layer = None,
                  numerical_feature_embedding: layers.Layer = None,
-                 saint_encoder: layers.Layer = None,
+                 encoder: layers.Layer = None,
                  head: layers.Layer = None,
                  **kwargs):
         if head is None:
-            head = RegressionHead()
+            num_outputs = 1
+            if "num_outputs" in kwargs:
+                num_outputs = kwargs.pop("num_outputs")
+            head = RegressionHead(num_outputs=num_outputs)
         super().__init__(features_metadata=features_metadata,
                          categorical_feature_embedding=categorical_feature_embedding,
                          numerical_feature_embedding=numerical_feature_embedding,
-                         saint_encoder=saint_encoder,
+                         encoder=encoder,
                          head=head,
                          **kwargs)
 
 
 class SAINTPretrainer(_BaseSAINTPretrainer):
     """
     SAINTPretrainer model with LayerFlow design.
```

### Comparing `Teras-0.1.0/teras/layerflow/models/simple.py` & `Teras-0.1.1/teras/layerflow/models/simple.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layerflow/models/tabnet.py` & `Teras-0.1.1/teras/layerflow/models/tabnet.py`

 * *Files 5% similar despite different names*

```diff
@@ -134,15 +134,23 @@
     def __init__(self,
                  features_metadata: dict,
                  categorical_features_embedding: layers.Layer = None,
                  encoder: layers.Layer = None,
                  head: layers.Layer = None,
                  **kwargs):
         if head is None:
-            head = ClassificationHead()
+            num_classes = 2
+            activation_out = None
+            if "num_classes" in kwargs:
+                num_classes = kwargs.pop("num_classes")
+            if "activation_out" in kwargs:
+                activation_out = kwargs.pop("activation_out")
+            head = ClassificationHead(num_classes=num_classes,
+                                      activation_out=activation_out,
+                                      name="tabnet_classification_head")
         super().__init__(features_metadata=features_metadata,
                          categorical_features_embedding=categorical_features_embedding,
                          encoder=encoder,
                          head=head,
                          **kwargs)
 
     @classmethod
@@ -229,15 +237,19 @@
     def __init__(self,
                  features_metadata: dict,
                  categorical_features_embedding: layers.Layer = None,
                  encoder: layers.Layer = None,
                  head: layers.Layer = None,
                  **kwargs):
         if head is None:
-            head = RegressionHead()
+            num_outputs = 1
+            if "num_outputs" in kwargs:
+                num_outputs = kwargs.pop("num_outputs")
+            head = RegressionHead(num_outputs=num_outputs,
+                                  name="tabnet_regression_head")
         super().__init__(features_metadata=features_metadata,
                          categorical_features_embedding=categorical_features_embedding,
                          encoder=encoder,
                          head=head,
                          **kwargs)
 
     @classmethod
```

### Comparing `Teras-0.1.0/teras/layerflow/models/tabtransformer.py` & `Teras-0.1.1/teras/layerflow/models/tabtransformer.py`

 * *Files 9% similar despite different names*

```diff
@@ -155,15 +155,23 @@
                  features_metadata: dict,
                  categorical_feature_embedding: layers.Layer = None,
                  column_embedding: layers.Layer = None,
                  encoder: layers.Layer = None,
                  head: layers.Layer = None,
                  **kwargs):
         if head is None:
-            head = ClassificationHead()
+            num_classes = 2
+            activation_out = None
+            if "num_classes" in kwargs:
+                num_classes = kwargs.pop("num_classes")
+            if "activation_out" in kwargs:
+                activation_out = kwargs.pop("activation_out")
+            head = ClassificationHead(num_classes=num_classes,
+                                      activation_out=activation_out,
+                                      name="tabtransformer_classification_head")
         super().__init__(features_metadata=features_metadata,
                          categorical_feature_embedding=categorical_feature_embedding,
                          column_embedding=column_embedding,
                          encoder=encoder,
                          head=head,
                          **kwargs)
 
@@ -258,15 +266,19 @@
                  features_metadata: dict,
                  categorical_feature_embedding: layers.Layer = None,
                  column_embedding: layers.Layer = None,
                  encoder: layers.Layer = None,
                  head: layers.Layer = None,
                  **kwargs):
         if head is None:
-            head = RegressionHead()
+            num_outputs = 1
+            if "num_outputs" in kwargs:
+                num_outputs = kwargs.pop("num_outputs")
+            head = RegressionHead(num_outputs=num_outputs,
+                                  name="tatransformer_regression_head")
         super().__init__(features_metadata=features_metadata,
                          categorical_feature_embedding=categorical_feature_embedding,
                          column_embedding=column_embedding,
                          encoder=encoder,
                          head=head,
                          **kwargs)
```

### Comparing `Teras-0.1.0/teras/layerflow/models/tvae.py` & `Teras-0.1.1/teras/layerflow/models/tvae.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layers/__init__.py` & `Teras-0.1.1/teras/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layers/activations.py` & `Teras-0.1.1/teras/layers/activations.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layers/activations_test.py` & `Teras-0.1.1/teras/layers/activations_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layers/common/__init__.py` & `Teras-0.1.1/teras/layers/common/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layers/common/gan.py` & `Teras-0.1.1/teras/layers/common/gan.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layers/common/head.py` & `Teras-0.1.1/teras/layers/common/head.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layers/common/head_test.py` & `Teras-0.1.1/teras/layers/common/head_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layers/common/transformer.py` & `Teras-0.1.1/teras/layers/common/transformer.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layers/common/transformer_test.py` & `Teras-0.1.1/teras/layers/common/transformer_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layers/ctgan.py` & `Teras-0.1.1/teras/layers/ctgan.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layers/ctgan_test.py` & `Teras-0.1.1/teras/layers/ctgan_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layers/dnfnet.py` & `Teras-0.1.1/teras/layers/dnfnet.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layers/dnfnet_test.py` & `Teras-0.1.1/teras/layers/dnfnet_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layers/embedding.py` & `Teras-0.1.1/teras/layers/embedding.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layers/embedding_test.py` & `Teras-0.1.1/teras/layers/embedding_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layers/encoding.py` & `Teras-0.1.1/teras/layers/encoding.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layers/encoding_test.py` & `Teras-0.1.1/teras/layers/encoding_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layers/ft_transformer.py` & `Teras-0.1.1/teras/layers/ft_transformer.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layers/ft_transformer_test.py` & `Teras-0.1.1/teras/layers/ft_transformer_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layers/gain.py` & `Teras-0.1.1/teras/layers/gain.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layers/gain_test.py` & `Teras-0.1.1/teras/layers/gain_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layers/node.py` & `Teras-0.1.1/teras/layers/node.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layers/node_test.py` & `Teras-0.1.1/teras/layers/node_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layers/oenf.py` & `Teras-0.1.1/teras/layers/oenf.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layers/regularization.py` & `Teras-0.1.1/teras/layers/regularization.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layers/regularization_test.py` & `Teras-0.1.1/teras/layers/regularization_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layers/rtdl_resnet.py` & `Teras-0.1.1/teras/layers/rtdl_resnet.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layers/saint.py` & `Teras-0.1.1/teras/layers/saint.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layers/saint_test.py` & `Teras-0.1.1/teras/layers/saint_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layers/tabnet.py` & `Teras-0.1.1/teras/layers/tabnet.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layers/tabnet_test.py` & `Teras-0.1.1/teras/layers/tabnet_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layers/tabtransformer.py` & `Teras-0.1.1/teras/layers/tabtransformer.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/layers/vime.py` & `Teras-0.1.1/teras/layers/vime.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/losses/__init__.py` & `Teras-0.1.1/teras/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/losses/ctgan.py` & `Teras-0.1.1/teras/losses/ctgan.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/losses/gain.py` & `Teras-0.1.1/teras/losses/gain.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/losses/pcgain.py` & `Teras-0.1.1/teras/losses/pcgain.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/losses/saint.py` & `Teras-0.1.1/teras/losses/saint.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/losses/tabnet.py` & `Teras-0.1.1/teras/losses/tabnet.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/losses/tvae.py` & `Teras-0.1.1/teras/losses/tvae.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/losses/vime.py` & `Teras-0.1.1/teras/losses/vime.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/models/__init__.py` & `Teras-0.1.1/teras/models/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/models/ctgan.py` & `Teras-0.1.1/teras/models/ctgan.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/models/dnfnet.py` & `Teras-0.1.1/teras/models/dnfnet.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/models/ft_transformer.py` & `Teras-0.1.1/teras/models/ft_transformer.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/models/gain.py` & `Teras-0.1.1/teras/models/gain.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/models/node.py` & `Teras-0.1.1/teras/models/node.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/models/pcgain.py` & `Teras-0.1.1/teras/models/pcgain.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/models/rtdl_resnet.py` & `Teras-0.1.1/teras/models/rtdl_resnet.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/models/saint.py` & `Teras-0.1.1/teras/models/saint.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,27 +142,27 @@
             # If categorical features exist, then they must be embedded
             self.categorical_feature_embedding = CategoricalFeatureEmbedding(
                                                     categorical_features_metadata=self._categorical_features_metadata,
                                                     embedding_dim=self.embedding_dim,
                                                     encode=self.encode_categorical_values)
             self._num_embedded_features += self._num_categorical_features
 
-        self.saint_encoder = SAINTEncoder(num_transformer_layers=self.num_transformer_layers,
-                                          embedding_dim=self.embedding_dim,
-                                          num_attention_heads=self.num_attention_heads,
-                                          num_inter_sample_attention_heads=self.num_inter_sample_attention_heads,
-                                          attention_dropout=self.attention_dropout,
-                                          inter_sample_attention_dropout=self.inter_sample_attention_dropout,
-                                          feedforward_dropout=self.feedforward_dropout,
-                                          feedforward_multiplier=self.feedforward_multiplier,
-                                          norm_epsilon=self.norm_epsilon,
-                                          apply_attention_to_features=self.apply_attention_to_features,
-                                          apply_attention_to_rows=self.apply_attention_to_rows,
-                                          num_embedded_features=self._num_embedded_features,
-                                          )
+        self.encoder = SAINTEncoder(num_transformer_layers=self.num_transformer_layers,
+                                    embedding_dim=self.embedding_dim,
+                                    num_attention_heads=self.num_attention_heads,
+                                    num_inter_sample_attention_heads=self.num_inter_sample_attention_heads,
+                                    attention_dropout=self.attention_dropout,
+                                    inter_sample_attention_dropout=self.inter_sample_attention_dropout,
+                                    feedforward_dropout=self.feedforward_dropout,
+                                    feedforward_multiplier=self.feedforward_multiplier,
+                                    norm_epsilon=self.norm_epsilon,
+                                    apply_attention_to_features=self.apply_attention_to_features,
+                                    apply_attention_to_rows=self.apply_attention_to_rows,
+                                    num_embedded_features=self._num_embedded_features,
+                                    )
         self.flatten = layers.Flatten()
         self.norm = layers.LayerNormalization(epsilon=self.norm_epsilon)
 
         self.head = None
         self._is_first_batch = True
         self._is_data_in_dict_format = False
 
@@ -184,16 +184,19 @@
             numerical_features = self.numerical_feature_embedding(inputs)
             if features is not None:
                 features = tf.concat([features, numerical_features],
                                      axis=1)
             else:
                 features = numerical_features
 
+        # Set features shape
+        features.set_shape((None, self.num_features, self.embedding_dim))
+
         # Contextualize the embedded features
-        features = self.saint_encoder(features)
+        features = self.encoder(features)
 
         # Flatten the contextualized embeddings of the features
         features = self.flatten(features)
 
         outputs = features
         if self.head is not None:
             outputs = self.head(outputs)
@@ -605,16 +608,16 @@
                 p = numerical_features
                 p_prime = numerical_features_prime
 
         # Apply mixup on the embedding space -- only to the augment data
         p_prime = self.mixup(p_prime)
 
         # Pass these embeddings through saint encoder
-        r = self.model.saint_encoder(p)
-        r_prime = self.model.saint_encoder(p_prime)
+        r = self.model.encoder(p)
+        r_prime = self.model.encoder(p_prime)
 
         # Pass the encoded features through projection heads
         z = self.projection_head_1(r)
         z_prime = self.projection_head_2(r_prime)
         # Normalize
         z = z / tf.norm(z, axis=-1, keepdims=True)
         z_prime = z_prime / tf.norm(z_prime, axis=-1, keepdims=True)
```

### Comparing `Teras-0.1.0/teras/models/tabnet.py` & `Teras-0.1.1/teras/models/tabnet.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/models/tabtransformer.py` & `Teras-0.1.1/teras/models/tabtransformer.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/models/tvae.py` & `Teras-0.1.1/teras/models/tvae.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/models/vime.py` & `Teras-0.1.1/teras/models/vime.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/preprocessing/__init__.py` & `Teras-0.1.1/teras/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/preprocessing/base/__init__.py` & `Teras-0.1.1/teras/preprocessing/base/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/preprocessing/base/base_data_transformer.py` & `Teras-0.1.1/teras/preprocessing/base/base_data_transformer.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/preprocessing/ctgan.py` & `Teras-0.1.1/teras/preprocessing/ctgan.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/preprocessing/gain.py` & `Teras-0.1.1/teras/preprocessing/gain.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/preprocessing/oenf.py` & `Teras-0.1.1/teras/preprocessing/oenf.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/preprocessing/pcgain.py` & `Teras-0.1.1/teras/preprocessing/pcgain.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/preprocessing/tvae.py` & `Teras-0.1.1/teras/preprocessing/tvae.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/utils/__init__.py` & `Teras-0.1.1/teras/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/utils/dnfnet.py` & `Teras-0.1.1/teras/utils/dnfnet.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/utils/pcgain.py` & `Teras-0.1.1/teras/utils/pcgain.py`

 * *Files identical despite different names*

### Comparing `Teras-0.1.0/teras/utils/utils.py` & `Teras-0.1.1/teras/utils/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -178,49 +178,66 @@
     features_meta_data["categorical"] = categorical_features_metadata
     features_meta_data["numerical"] = numerical_features_metadata
     return features_meta_data
 
 
 def dataframe_to_tf_dataset(
         dataframe: pd.DataFrame,
-        target: str = None,
+        target: Union[str, list] = None,
         shuffle: bool = True,
         batch_size: int = 1024,
         as_dict: bool = False,
 ):
     """
     Builds a tf.data.Dataset from a given pandas dataframe
 
     Args:
-        dataframe: A pandas dataframe
-        target: Name of the target column
-        shuffle: Whether to shuffle the dataset
-        batch_size: Batch size
-        as_dict: Whether to make a tensorflow dataset in a dictionary format
+        dataframe: `pd.DataFrame`,
+            A pandas dataframe
+        target: `str` or `list`,
+            Name of the target column or list of names of the target columns.
+        shuffle: `bool`, default True
+            Whether to shuffle the dataset
+        batch_size: `int`, default 1024,
+            Batch size
+        as_dict: `bool`, default False,
+            Whether to make a tensorflow dataset in a dictionary format
             where each record is a mapping of features names against their values.
 
             SOME GUIDELINES on when to create dataset in dictionary format and when not:
             1. If your dataset is composed of heterogeneous data formats, i.e. it contains
                 features where some features contain integers/floats AND others contain strings,
                 and you don't want to manually encode the string values into integers/floats,
                 then your dataset must be in dictionary format, which you can get by setting
                 the `as_dict` parameter to `True`.
 
 
     Returns:
          A tf.data.Dataset dataset
     """
     df = dataframe.copy()
-    if target:
-        labels = df.pop(target)
+    if target is not None:
+        if isinstance(target, (list, tuple, set)):
+            if as_dict:
+                labels = dict()
+                for feat in target:
+                    labels[feat] = df.pop(feat).values
+            else:
+                labels = []
+                for feat in target:
+                    labels.append(df.pop(feat).values)
+                labels = tf.transpose(tf.constant(labels))
+        else:
+            labels = df.pop(target)
+            if not as_dict:
+                labels = labels.values
         if as_dict:
             dataset = tf.data.Dataset.from_tensor_slices((dict(df), labels))
         else:
             df = df.values
-            labels = labels.values
             dataset = tf.data.Dataset.from_tensor_slices((df, labels))
     else:
         if as_dict:
             dataset = tf.data.Dataset.from_tensor_slices(dict(df))
         else:
             dataset = tf.data.Dataset.from_tensor_slices(df.values)
     if shuffle:
```

### Comparing `Teras-0.1.0/teras/utils/vime.py` & `Teras-0.1.1/teras/utils/vime.py`

 * *Files identical despite different names*

