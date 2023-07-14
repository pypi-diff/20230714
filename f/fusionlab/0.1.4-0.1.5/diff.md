# Comparing `tmp/fusionlab-0.1.4.tar.gz` & `tmp/fusionlab-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusionlab-0.1.4.tar", last modified: Sat Jul  8 09:26:21 2023, max compression
+gzip compressed data, was "fusionlab-0.1.5.tar", last modified: Fri Jul 14 03:52:39 2023, max compression
```

## Comparing `fusionlab-0.1.4.tar` & `fusionlab-0.1.5.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.854576 fusionlab-0.1.4/
--rw-r--r--   0 cyli       (502) staff       (20)     1060 2022-12-31 04:40:09.000000 fusionlab-0.1.4/LICENSE
--rw-r--r--   0 cyli       (502) staff       (20)     3730 2023-07-08 09:26:21.854421 fusionlab-0.1.4/PKG-INFO
--rw-r--r--   0 cyli       (502) staff       (20)     3267 2023-07-08 09:17:08.000000 fusionlab-0.1.4/README.md
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.838028 fusionlab-0.1.4/fusionlab/
--rw-r--r--   0 cyli       (502) staff       (20)      993 2023-06-02 08:43:17.000000 fusionlab-0.1.4/fusionlab/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)       63 2023-07-08 09:19:32.000000 fusionlab-0.1.4/fusionlab/__version__.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.840314 fusionlab-0.1.4/fusionlab/classification/
--rw-r--r--   0 cyli       (502) staff       (20)      387 2023-07-01 03:49:33.000000 fusionlab-0.1.4/fusionlab/classification/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     3353 2023-07-01 03:49:33.000000 fusionlab-0.1.4/fusionlab/classification/base.py
--rw-r--r--   0 cyli       (502) staff       (20)      711 2023-07-01 03:49:33.000000 fusionlab-0.1.4/fusionlab/classification/lstm.py
--rw-r--r--   0 cyli       (502) staff       (20)     1473 2023-07-01 03:49:33.000000 fusionlab-0.1.4/fusionlab/classification/vgg.py
--rw-r--r--   0 cyli       (502) staff       (20)       32 2023-06-02 08:43:17.000000 fusionlab-0.1.4/fusionlab/configs.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.841619 fusionlab-0.1.4/fusionlab/datasets/
--rw-r--r--   0 cyli       (502) staff       (20)      558 2023-07-01 03:49:44.000000 fusionlab-0.1.4/fusionlab/datasets/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     1181 2023-05-20 16:17:41.000000 fusionlab-0.1.4/fusionlab/datasets/a12lead.py
--rw-r--r--   0 cyli       (502) staff       (20)     5456 2023-06-02 08:43:17.000000 fusionlab-0.1.4/fusionlab/datasets/cinc2017.py
--rw-r--r--   0 cyli       (502) staff       (20)      325 2023-06-02 08:43:17.000000 fusionlab-0.1.4/fusionlab/datasets/csvread.py
--rw-r--r--   0 cyli       (502) staff       (20)    13273 2023-07-01 03:49:33.000000 fusionlab-0.1.4/fusionlab/datasets/ludb.py
--rw-r--r--   0 cyli       (502) staff       (20)    12053 2023-05-20 16:17:41.000000 fusionlab-0.1.4/fusionlab/datasets/muse.py
--rw-r--r--   0 cyli       (502) staff       (20)     4586 2023-07-01 03:49:44.000000 fusionlab-0.1.4/fusionlab/datasets/utils.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.841885 fusionlab-0.1.4/fusionlab/encoders/
--rw-r--r--   0 cyli       (502) staff       (20)      906 2023-07-08 09:17:08.000000 fusionlab-0.1.4/fusionlab/encoders/__init__.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.842345 fusionlab-0.1.4/fusionlab/encoders/alexnet/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.4/fusionlab/encoders/alexnet/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     1751 2023-07-01 03:49:33.000000 fusionlab-0.1.4/fusionlab/encoders/alexnet/alexnet.py
--rw-r--r--   0 cyli       (502) staff       (20)     1186 2022-12-31 04:40:09.000000 fusionlab-0.1.4/fusionlab/encoders/alexnet/tfalexnet.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.842682 fusionlab-0.1.4/fusionlab/encoders/convnext/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-07-08 09:17:08.000000 fusionlab-0.1.4/fusionlab/encoders/convnext/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     8194 2023-07-08 09:17:08.000000 fusionlab-0.1.4/fusionlab/encoders/convnext/convnext.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.843025 fusionlab-0.1.4/fusionlab/encoders/efficientnet/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-07-08 09:17:08.000000 fusionlab-0.1.4/fusionlab/encoders/efficientnet/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)    12573 2023-07-08 09:19:15.000000 fusionlab-0.1.4/fusionlab/encoders/efficientnet/efficientnet.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.843740 fusionlab-0.1.4/fusionlab/encoders/inceptionv1/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.4/fusionlab/encoders/inceptionv1/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     3650 2023-07-01 03:49:33.000000 fusionlab-0.1.4/fusionlab/encoders/inceptionv1/inceptionv1.py
--rw-r--r--   0 cyli       (502) staff       (20)     3029 2023-01-03 10:19:18.000000 fusionlab-0.1.4/fusionlab/encoders/inceptionv1/tfinceptionv1.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.844359 fusionlab-0.1.4/fusionlab/encoders/resnetv1/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.4/fusionlab/encoders/resnetv1/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     4838 2023-07-01 03:49:33.000000 fusionlab-0.1.4/fusionlab/encoders/resnetv1/resnetv1.py
--rw-r--r--   0 cyli       (502) staff       (20)     4183 2023-01-05 10:15:54.000000 fusionlab-0.1.4/fusionlab/encoders/resnetv1/tfresnetv1.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.845000 fusionlab-0.1.4/fusionlab/encoders/vgg/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.4/fusionlab/encoders/vgg/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     4206 2022-12-31 04:40:09.000000 fusionlab-0.1.4/fusionlab/encoders/vgg/tfvgg.py
--rw-r--r--   0 cyli       (502) staff       (20)     4753 2023-07-01 03:49:33.000000 fusionlab-0.1.4/fusionlab/encoders/vgg/vgg.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.846444 fusionlab-0.1.4/fusionlab/functional/
--rw-r--r--   0 cyli       (502) staff       (20)      347 2023-05-20 16:17:41.000000 fusionlab-0.1.4/fusionlab/functional/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)      420 2023-05-20 16:17:41.000000 fusionlab-0.1.4/fusionlab/functional/dice.py
--rw-r--r--   0 cyli       (502) staff       (20)      486 2023-05-20 16:17:41.000000 fusionlab-0.1.4/fusionlab/functional/iou.py
--rw-r--r--   0 cyli       (502) staff       (20)      661 2023-05-20 16:17:41.000000 fusionlab-0.1.4/fusionlab/functional/tfdice.py
--rw-r--r--   0 cyli       (502) staff       (20)      718 2023-05-20 16:17:41.000000 fusionlab-0.1.4/fusionlab/functional/tfiou.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.847036 fusionlab-0.1.4/fusionlab/layers/
--rw-r--r--   0 cyli       (502) staff       (20)      289 2023-07-08 09:17:08.000000 fusionlab-0.1.4/fusionlab/layers/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     3604 2023-07-08 09:17:08.000000 fusionlab-0.1.4/fusionlab/layers/base.py
--rw-r--r--   0 cyli       (502) staff       (20)    17832 2023-07-08 09:17:08.000000 fusionlab-0.1.4/fusionlab/layers/factories.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.847987 fusionlab-0.1.4/fusionlab/layers/squeeze_excitation/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-07-07 10:44:19.000000 fusionlab-0.1.4/fusionlab/layers/squeeze_excitation/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     2187 2023-07-08 09:17:08.000000 fusionlab-0.1.4/fusionlab/layers/squeeze_excitation/se.py
--rw-r--r--   0 cyli       (502) staff       (20)      748 2023-01-05 10:57:39.000000 fusionlab-0.1.4/fusionlab/layers/squeeze_excitation/tfse.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.848273 fusionlab-0.1.4/fusionlab/losses/
--rw-r--r--   0 cyli       (502) staff       (20)      405 2023-05-20 16:17:41.000000 fusionlab-0.1.4/fusionlab/losses/__init__.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.848756 fusionlab-0.1.4/fusionlab/losses/diceloss/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-31 09:07:31.000000 fusionlab-0.1.4/fusionlab/losses/diceloss/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     3650 2023-01-31 09:07:31.000000 fusionlab-0.1.4/fusionlab/losses/diceloss/dice.py
--rw-r--r--   0 cyli       (502) staff       (20)     4142 2023-05-21 07:24:23.000000 fusionlab-0.1.4/fusionlab/losses/diceloss/tfdice.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.849377 fusionlab-0.1.4/fusionlab/losses/iouloss/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-31 09:07:31.000000 fusionlab-0.1.4/fusionlab/losses/iouloss/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     2773 2023-01-31 09:07:31.000000 fusionlab-0.1.4/fusionlab/losses/iouloss/iou.py
--rw-r--r--   0 cyli       (502) staff       (20)     3102 2023-05-21 07:24:23.000000 fusionlab-0.1.4/fusionlab/losses/iouloss/tfiou.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.849972 fusionlab-0.1.4/fusionlab/losses/tversky/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-04-13 01:08:31.000000 fusionlab-0.1.4/fusionlab/losses/tversky/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     4440 2023-04-13 01:08:31.000000 fusionlab-0.1.4/fusionlab/losses/tversky/tftversky.py
--rw-r--r--   0 cyli       (502) staff       (20)     3897 2023-04-13 01:08:31.000000 fusionlab-0.1.4/fusionlab/losses/tversky/tversky.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.850205 fusionlab-0.1.4/fusionlab/metrics/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-31 09:07:31.000000 fusionlab-0.1.4/fusionlab/metrics/__init__.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.851218 fusionlab-0.1.4/fusionlab/segmentation/
--rw-r--r--   0 cyli       (502) staff       (20)      420 2023-07-01 03:49:33.000000 fusionlab-0.1.4/fusionlab/segmentation/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     1770 2023-07-01 03:49:33.000000 fusionlab-0.1.4/fusionlab/segmentation/base.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.851621 fusionlab-0.1.4/fusionlab/segmentation/resunet/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-14 03:30:01.000000 fusionlab-0.1.4/fusionlab/segmentation/resunet/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     5271 2023-07-01 03:49:33.000000 fusionlab-0.1.4/fusionlab/segmentation/resunet/resunet.py
--rw-r--r--   0 cyli       (502) staff       (20)     4476 2023-05-20 16:17:41.000000 fusionlab-0.1.4/fusionlab/segmentation/resunet/tfresunet.py
--rw-r--r--   0 cyli       (502) staff       (20)      683 2023-05-20 16:17:41.000000 fusionlab-0.1.4/fusionlab/segmentation/tfbase.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.851994 fusionlab-0.1.4/fusionlab/segmentation/unet/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-07 18:27:01.000000 fusionlab-0.1.4/fusionlab/segmentation/unet/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     4168 2023-05-20 16:17:41.000000 fusionlab-0.1.4/fusionlab/segmentation/unet/tfunet.py
--rw-r--r--   0 cyli       (502) staff       (20)     5414 2023-07-01 03:49:33.000000 fusionlab-0.1.4/fusionlab/segmentation/unet/unet.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.852353 fusionlab-0.1.4/fusionlab/segmentation/unet2plus/
--rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-12 08:11:48.000000 fusionlab-0.1.4/fusionlab/segmentation/unet2plus/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     4622 2023-05-20 16:17:41.000000 fusionlab-0.1.4/fusionlab/segmentation/unet2plus/tfunet2plus.py
--rw-r--r--   0 cyli       (502) staff       (20)     5662 2023-07-01 03:49:33.000000 fusionlab-0.1.4/fusionlab/segmentation/unet2plus/unet2plus.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.853102 fusionlab-0.1.4/fusionlab/trainers/
--rw-r--r--   0 cyli       (502) staff       (20)      224 2023-05-20 16:17:41.000000 fusionlab-0.1.4/fusionlab/trainers/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)     6521 2023-06-02 08:43:17.000000 fusionlab-0.1.4/fusionlab/trainers/dcgan.py
--rw-r--r--   0 cyli       (502) staff       (20)       72 2023-05-20 16:17:48.000000 fusionlab-0.1.4/fusionlab/trainers/test.py
--rw-r--r--   0 cyli       (502) staff       (20)     4784 2023-06-02 08:43:17.000000 fusionlab-0.1.4/fusionlab/trainers/trainer.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.854111 fusionlab-0.1.4/fusionlab/utils/
--rw-r--r--   0 cyli       (502) staff       (20)       93 2023-07-01 03:49:44.000000 fusionlab-0.1.4/fusionlab/utils/__init__.py
--rw-r--r--   0 cyli       (502) staff       (20)      218 2022-12-31 04:40:09.000000 fusionlab-0.1.4/fusionlab/utils/basic.py
--rw-r--r--   0 cyli       (502) staff       (20)      406 2023-07-01 03:49:44.000000 fusionlab-0.1.4/fusionlab/utils/plots.py
--rw-r--r--   0 cyli       (502) staff       (20)      825 2023-06-02 08:43:17.000000 fusionlab-0.1.4/fusionlab/utils/trace.py
-drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-08 09:26:21.839044 fusionlab-0.1.4/fusionlab.egg-info/
--rw-r--r--   0 cyli       (502) staff       (20)     3730 2023-07-08 09:26:21.000000 fusionlab-0.1.4/fusionlab.egg-info/PKG-INFO
--rw-r--r--   0 cyli       (502) staff       (20)     2723 2023-07-08 09:26:21.000000 fusionlab-0.1.4/fusionlab.egg-info/SOURCES.txt
--rw-r--r--   0 cyli       (502) staff       (20)        1 2023-07-08 09:26:21.000000 fusionlab-0.1.4/fusionlab.egg-info/dependency_links.txt
--rw-r--r--   0 cyli       (502) staff       (20)      191 2023-07-08 09:26:21.000000 fusionlab-0.1.4/fusionlab.egg-info/requires.txt
--rw-r--r--   0 cyli       (502) staff       (20)       10 2023-07-08 09:26:21.000000 fusionlab-0.1.4/fusionlab.egg-info/top_level.txt
--rw-r--r--   0 cyli       (502) staff       (20)       38 2023-07-08 09:26:21.854619 fusionlab-0.1.4/setup.cfg
--rw-r--r--   0 cyli       (502) staff       (20)     3989 2023-05-21 07:24:23.000000 fusionlab-0.1.4/setup.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.859478 fusionlab-0.1.5/
+-rw-r--r--   0 cyli       (502) staff       (20)     1060 2022-12-31 04:40:09.000000 fusionlab-0.1.5/LICENSE
+-rw-r--r--   0 cyli       (502) staff       (20)     3730 2023-07-14 03:52:39.859354 fusionlab-0.1.5/PKG-INFO
+-rw-r--r--   0 cyli       (502) staff       (20)     3267 2023-07-08 09:17:08.000000 fusionlab-0.1.5/README.md
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.844439 fusionlab-0.1.5/fusionlab/
+-rw-r--r--   0 cyli       (502) staff       (20)      993 2023-06-02 08:43:17.000000 fusionlab-0.1.5/fusionlab/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)       63 2023-07-14 03:50:01.000000 fusionlab-0.1.5/fusionlab/__version__.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.846464 fusionlab-0.1.5/fusionlab/classification/
+-rw-r--r--   0 cyli       (502) staff       (20)      387 2023-07-01 03:49:33.000000 fusionlab-0.1.5/fusionlab/classification/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     3353 2023-07-01 03:49:33.000000 fusionlab-0.1.5/fusionlab/classification/base.py
+-rw-r--r--   0 cyli       (502) staff       (20)      711 2023-07-01 03:49:33.000000 fusionlab-0.1.5/fusionlab/classification/lstm.py
+-rw-r--r--   0 cyli       (502) staff       (20)     1473 2023-07-01 03:49:33.000000 fusionlab-0.1.5/fusionlab/classification/vgg.py
+-rw-r--r--   0 cyli       (502) staff       (20)       32 2023-06-02 08:43:17.000000 fusionlab-0.1.5/fusionlab/configs.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.847878 fusionlab-0.1.5/fusionlab/datasets/
+-rw-r--r--   0 cyli       (502) staff       (20)      558 2023-07-01 03:49:44.000000 fusionlab-0.1.5/fusionlab/datasets/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     1181 2023-05-20 16:17:41.000000 fusionlab-0.1.5/fusionlab/datasets/a12lead.py
+-rw-r--r--   0 cyli       (502) staff       (20)     5456 2023-06-02 08:43:17.000000 fusionlab-0.1.5/fusionlab/datasets/cinc2017.py
+-rw-r--r--   0 cyli       (502) staff       (20)      325 2023-06-02 08:43:17.000000 fusionlab-0.1.5/fusionlab/datasets/csvread.py
+-rw-r--r--   0 cyli       (502) staff       (20)    13273 2023-07-01 03:49:33.000000 fusionlab-0.1.5/fusionlab/datasets/ludb.py
+-rw-r--r--   0 cyli       (502) staff       (20)    12053 2023-05-20 16:17:41.000000 fusionlab-0.1.5/fusionlab/datasets/muse.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4586 2023-07-01 03:49:44.000000 fusionlab-0.1.5/fusionlab/datasets/utils.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.848113 fusionlab-0.1.5/fusionlab/encoders/
+-rw-r--r--   0 cyli       (502) staff       (20)      906 2023-07-08 09:17:08.000000 fusionlab-0.1.5/fusionlab/encoders/__init__.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.848607 fusionlab-0.1.5/fusionlab/encoders/alexnet/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.5/fusionlab/encoders/alexnet/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     1751 2023-07-01 03:49:33.000000 fusionlab-0.1.5/fusionlab/encoders/alexnet/alexnet.py
+-rw-r--r--   0 cyli       (502) staff       (20)     1186 2022-12-31 04:40:09.000000 fusionlab-0.1.5/fusionlab/encoders/alexnet/tfalexnet.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.848914 fusionlab-0.1.5/fusionlab/encoders/convnext/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-07-08 09:17:08.000000 fusionlab-0.1.5/fusionlab/encoders/convnext/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     8194 2023-07-08 09:17:08.000000 fusionlab-0.1.5/fusionlab/encoders/convnext/convnext.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.849256 fusionlab-0.1.5/fusionlab/encoders/efficientnet/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-07-08 09:17:08.000000 fusionlab-0.1.5/fusionlab/encoders/efficientnet/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)    12573 2023-07-08 09:19:15.000000 fusionlab-0.1.5/fusionlab/encoders/efficientnet/efficientnet.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.849865 fusionlab-0.1.5/fusionlab/encoders/inceptionv1/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.5/fusionlab/encoders/inceptionv1/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     3650 2023-07-01 03:49:33.000000 fusionlab-0.1.5/fusionlab/encoders/inceptionv1/inceptionv1.py
+-rw-r--r--   0 cyli       (502) staff       (20)     3029 2023-01-03 10:19:18.000000 fusionlab-0.1.5/fusionlab/encoders/inceptionv1/tfinceptionv1.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.850516 fusionlab-0.1.5/fusionlab/encoders/resnetv1/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.5/fusionlab/encoders/resnetv1/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4838 2023-07-01 03:49:33.000000 fusionlab-0.1.5/fusionlab/encoders/resnetv1/resnetv1.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4183 2023-01-05 10:15:54.000000 fusionlab-0.1.5/fusionlab/encoders/resnetv1/tfresnetv1.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.851205 fusionlab-0.1.5/fusionlab/encoders/vgg/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-05-20 16:17:41.000000 fusionlab-0.1.5/fusionlab/encoders/vgg/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4206 2022-12-31 04:40:09.000000 fusionlab-0.1.5/fusionlab/encoders/vgg/tfvgg.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4753 2023-07-01 03:49:33.000000 fusionlab-0.1.5/fusionlab/encoders/vgg/vgg.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.852383 fusionlab-0.1.5/fusionlab/functional/
+-rw-r--r--   0 cyli       (502) staff       (20)      347 2023-05-20 16:17:41.000000 fusionlab-0.1.5/fusionlab/functional/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)      420 2023-05-20 16:17:41.000000 fusionlab-0.1.5/fusionlab/functional/dice.py
+-rw-r--r--   0 cyli       (502) staff       (20)      486 2023-05-20 16:17:41.000000 fusionlab-0.1.5/fusionlab/functional/iou.py
+-rw-r--r--   0 cyli       (502) staff       (20)      661 2023-05-20 16:17:41.000000 fusionlab-0.1.5/fusionlab/functional/tfdice.py
+-rw-r--r--   0 cyli       (502) staff       (20)      718 2023-05-20 16:17:41.000000 fusionlab-0.1.5/fusionlab/functional/tfiou.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.852927 fusionlab-0.1.5/fusionlab/layers/
+-rw-r--r--   0 cyli       (502) staff       (20)      289 2023-07-08 09:17:08.000000 fusionlab-0.1.5/fusionlab/layers/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     3599 2023-07-14 03:24:02.000000 fusionlab-0.1.5/fusionlab/layers/base.py
+-rw-r--r--   0 cyli       (502) staff       (20)    17832 2023-07-08 09:17:08.000000 fusionlab-0.1.5/fusionlab/layers/factories.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.853623 fusionlab-0.1.5/fusionlab/layers/squeeze_excitation/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-07-07 10:44:19.000000 fusionlab-0.1.5/fusionlab/layers/squeeze_excitation/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     2187 2023-07-08 09:17:08.000000 fusionlab-0.1.5/fusionlab/layers/squeeze_excitation/se.py
+-rw-r--r--   0 cyli       (502) staff       (20)      748 2023-01-05 10:57:39.000000 fusionlab-0.1.5/fusionlab/layers/squeeze_excitation/tfse.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.853878 fusionlab-0.1.5/fusionlab/losses/
+-rw-r--r--   0 cyli       (502) staff       (20)      405 2023-05-20 16:17:41.000000 fusionlab-0.1.5/fusionlab/losses/__init__.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.854330 fusionlab-0.1.5/fusionlab/losses/diceloss/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-31 09:07:31.000000 fusionlab-0.1.5/fusionlab/losses/diceloss/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     3650 2023-01-31 09:07:31.000000 fusionlab-0.1.5/fusionlab/losses/diceloss/dice.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4142 2023-05-21 07:24:23.000000 fusionlab-0.1.5/fusionlab/losses/diceloss/tfdice.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.854881 fusionlab-0.1.5/fusionlab/losses/iouloss/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-31 09:07:31.000000 fusionlab-0.1.5/fusionlab/losses/iouloss/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     2773 2023-01-31 09:07:31.000000 fusionlab-0.1.5/fusionlab/losses/iouloss/iou.py
+-rw-r--r--   0 cyli       (502) staff       (20)     3102 2023-05-21 07:24:23.000000 fusionlab-0.1.5/fusionlab/losses/iouloss/tfiou.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.855500 fusionlab-0.1.5/fusionlab/losses/tversky/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-04-13 01:08:31.000000 fusionlab-0.1.5/fusionlab/losses/tversky/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4440 2023-04-13 01:08:31.000000 fusionlab-0.1.5/fusionlab/losses/tversky/tftversky.py
+-rw-r--r--   0 cyli       (502) staff       (20)     3897 2023-04-13 01:08:31.000000 fusionlab-0.1.5/fusionlab/losses/tversky/tversky.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.855739 fusionlab-0.1.5/fusionlab/metrics/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-31 09:07:31.000000 fusionlab-0.1.5/fusionlab/metrics/__init__.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.856330 fusionlab-0.1.5/fusionlab/segmentation/
+-rw-r--r--   0 cyli       (502) staff       (20)      420 2023-07-01 03:49:33.000000 fusionlab-0.1.5/fusionlab/segmentation/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     1770 2023-07-01 03:49:33.000000 fusionlab-0.1.5/fusionlab/segmentation/base.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.856730 fusionlab-0.1.5/fusionlab/segmentation/resunet/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-14 03:30:01.000000 fusionlab-0.1.5/fusionlab/segmentation/resunet/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     5271 2023-07-01 03:49:33.000000 fusionlab-0.1.5/fusionlab/segmentation/resunet/resunet.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4476 2023-05-20 16:17:41.000000 fusionlab-0.1.5/fusionlab/segmentation/resunet/tfresunet.py
+-rw-r--r--   0 cyli       (502) staff       (20)      683 2023-05-20 16:17:41.000000 fusionlab-0.1.5/fusionlab/segmentation/tfbase.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.857104 fusionlab-0.1.5/fusionlab/segmentation/unet/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-07 18:27:01.000000 fusionlab-0.1.5/fusionlab/segmentation/unet/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4168 2023-05-20 16:17:41.000000 fusionlab-0.1.5/fusionlab/segmentation/unet/tfunet.py
+-rw-r--r--   0 cyli       (502) staff       (20)     5414 2023-07-01 03:49:33.000000 fusionlab-0.1.5/fusionlab/segmentation/unet/unet.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.857443 fusionlab-0.1.5/fusionlab/segmentation/unet2plus/
+-rw-r--r--   0 cyli       (502) staff       (20)        0 2023-01-12 08:11:48.000000 fusionlab-0.1.5/fusionlab/segmentation/unet2plus/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4622 2023-05-20 16:17:41.000000 fusionlab-0.1.5/fusionlab/segmentation/unet2plus/tfunet2plus.py
+-rw-r--r--   0 cyli       (502) staff       (20)     5662 2023-07-01 03:49:33.000000 fusionlab-0.1.5/fusionlab/segmentation/unet2plus/unet2plus.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.858153 fusionlab-0.1.5/fusionlab/trainers/
+-rw-r--r--   0 cyli       (502) staff       (20)      224 2023-05-20 16:17:41.000000 fusionlab-0.1.5/fusionlab/trainers/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)     6521 2023-06-02 08:43:17.000000 fusionlab-0.1.5/fusionlab/trainers/dcgan.py
+-rw-r--r--   0 cyli       (502) staff       (20)       72 2023-05-20 16:17:48.000000 fusionlab-0.1.5/fusionlab/trainers/test.py
+-rw-r--r--   0 cyli       (502) staff       (20)     4784 2023-06-02 08:43:17.000000 fusionlab-0.1.5/fusionlab/trainers/trainer.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.859069 fusionlab-0.1.5/fusionlab/utils/
+-rw-r--r--   0 cyli       (502) staff       (20)      106 2023-07-14 03:23:23.000000 fusionlab-0.1.5/fusionlab/utils/__init__.py
+-rw-r--r--   0 cyli       (502) staff       (20)      789 2023-07-14 03:23:06.000000 fusionlab-0.1.5/fusionlab/utils/basic.py
+-rw-r--r--   0 cyli       (502) staff       (20)      406 2023-07-01 03:49:44.000000 fusionlab-0.1.5/fusionlab/utils/plots.py
+-rw-r--r--   0 cyli       (502) staff       (20)      825 2023-06-02 08:43:17.000000 fusionlab-0.1.5/fusionlab/utils/trace.py
+drwxr-xr-x   0 cyli       (502) staff       (20)        0 2023-07-14 03:52:39.845280 fusionlab-0.1.5/fusionlab.egg-info/
+-rw-r--r--   0 cyli       (502) staff       (20)     3730 2023-07-14 03:52:39.000000 fusionlab-0.1.5/fusionlab.egg-info/PKG-INFO
+-rw-r--r--   0 cyli       (502) staff       (20)     2723 2023-07-14 03:52:39.000000 fusionlab-0.1.5/fusionlab.egg-info/SOURCES.txt
+-rw-r--r--   0 cyli       (502) staff       (20)        1 2023-07-14 03:52:39.000000 fusionlab-0.1.5/fusionlab.egg-info/dependency_links.txt
+-rw-r--r--   0 cyli       (502) staff       (20)      177 2023-07-14 03:52:39.000000 fusionlab-0.1.5/fusionlab.egg-info/requires.txt
+-rw-r--r--   0 cyli       (502) staff       (20)       10 2023-07-14 03:52:39.000000 fusionlab-0.1.5/fusionlab.egg-info/top_level.txt
+-rw-r--r--   0 cyli       (502) staff       (20)       38 2023-07-14 03:52:39.859518 fusionlab-0.1.5/setup.cfg
+-rw-r--r--   0 cyli       (502) staff       (20)     3989 2023-05-21 07:24:23.000000 fusionlab-0.1.5/setup.py
```

### Comparing `fusionlab-0.1.4/LICENSE` & `fusionlab-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/PKG-INFO` & `fusionlab-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusionlab
-Version: 0.1.4
+Version: 0.1.5
 Summary: Useful packages for DL
 Home-page: https://github.com/taipingeric/fusionlab
 Author: Chih-Yang Li
 Author-email: taipingeric@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fusionlab-0.1.4/README.md` & `fusionlab-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/__init__.py` & `fusionlab-0.1.5/fusionlab/__init__.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/classification/base.py` & `fusionlab-0.1.5/fusionlab/classification/base.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/classification/lstm.py` & `fusionlab-0.1.5/fusionlab/classification/lstm.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/classification/vgg.py` & `fusionlab-0.1.5/fusionlab/classification/vgg.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/datasets/__init__.py` & `fusionlab-0.1.5/fusionlab/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/datasets/a12lead.py` & `fusionlab-0.1.5/fusionlab/datasets/a12lead.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/datasets/cinc2017.py` & `fusionlab-0.1.5/fusionlab/datasets/cinc2017.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/datasets/ludb.py` & `fusionlab-0.1.5/fusionlab/datasets/ludb.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/datasets/muse.py` & `fusionlab-0.1.5/fusionlab/datasets/muse.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/datasets/utils.py` & `fusionlab-0.1.5/fusionlab/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/encoders/__init__.py` & `fusionlab-0.1.5/fusionlab/encoders/__init__.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/encoders/alexnet/alexnet.py` & `fusionlab-0.1.5/fusionlab/encoders/alexnet/alexnet.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/encoders/alexnet/tfalexnet.py` & `fusionlab-0.1.5/fusionlab/encoders/alexnet/tfalexnet.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/encoders/convnext/convnext.py` & `fusionlab-0.1.5/fusionlab/encoders/convnext/convnext.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/encoders/efficientnet/efficientnet.py` & `fusionlab-0.1.5/fusionlab/encoders/efficientnet/efficientnet.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/encoders/inceptionv1/inceptionv1.py` & `fusionlab-0.1.5/fusionlab/encoders/inceptionv1/inceptionv1.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/encoders/inceptionv1/tfinceptionv1.py` & `fusionlab-0.1.5/fusionlab/encoders/inceptionv1/tfinceptionv1.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/encoders/resnetv1/resnetv1.py` & `fusionlab-0.1.5/fusionlab/encoders/resnetv1/resnetv1.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/encoders/resnetv1/tfresnetv1.py` & `fusionlab-0.1.5/fusionlab/encoders/resnetv1/tfresnetv1.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/encoders/vgg/tfvgg.py` & `fusionlab-0.1.5/fusionlab/encoders/vgg/tfvgg.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/encoders/vgg/vgg.py` & `fusionlab-0.1.5/fusionlab/encoders/vgg/vgg.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/functional/tfdice.py` & `fusionlab-0.1.5/fusionlab/functional/tfdice.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/functional/tfiou.py` & `fusionlab-0.1.5/fusionlab/functional/tfiou.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/layers/base.py` & `fusionlab-0.1.5/fusionlab/layers/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch.nn as nn
-from torchvision.utils import _make_ntuple
 from typing import Union, Sequence, Optional, Callable
 
 from fusionlab.layers import ConvND, BatchNorm
+from fusionlab.utils import make_ntuple
 
 class ConvNormAct(nn.Module):
     '''
     ref: 
     https://pytorch.org/vision/main/generated/torchvision.ops.Conv2dNormActivation.html
     https://github.com/pytorch/vision/blob/main/torchvision/ops/misc.py#L68
 
@@ -48,16 +48,16 @@
         super().__init__()
         # padding 
         if padding is None:
             if isinstance(kernel_size, int) and isinstance(dilation, int):
                 padding = (kernel_size - 1) // 2 * dilation
             else:
                 _conv_dim = spatial_dims
-                kernel_size = _make_ntuple(kernel_size, _conv_dim)
-                dilation = _make_ntuple(dilation, _conv_dim)
+                kernel_size = make_ntuple(kernel_size, _conv_dim)
+                dilation = make_ntuple(dilation, _conv_dim)
                 padding = tuple((kernel_size[i] - 1) // 2 * dilation[i] for i in range(_conv_dim))
         # bias
         if bias is None:
             bias = norm_layer is None
 
         self.conv = ConvND(
             spatial_dims,
```

### Comparing `fusionlab-0.1.4/fusionlab/layers/factories.py` & `fusionlab-0.1.5/fusionlab/layers/factories.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/layers/squeeze_excitation/se.py` & `fusionlab-0.1.5/fusionlab/layers/squeeze_excitation/se.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/layers/squeeze_excitation/tfse.py` & `fusionlab-0.1.5/fusionlab/layers/squeeze_excitation/tfse.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/losses/diceloss/dice.py` & `fusionlab-0.1.5/fusionlab/losses/diceloss/dice.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/losses/diceloss/tfdice.py` & `fusionlab-0.1.5/fusionlab/losses/diceloss/tfdice.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/losses/iouloss/iou.py` & `fusionlab-0.1.5/fusionlab/losses/iouloss/iou.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/losses/iouloss/tfiou.py` & `fusionlab-0.1.5/fusionlab/losses/iouloss/tfiou.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/losses/tversky/tftversky.py` & `fusionlab-0.1.5/fusionlab/losses/tversky/tftversky.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/losses/tversky/tversky.py` & `fusionlab-0.1.5/fusionlab/losses/tversky/tversky.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/segmentation/base.py` & `fusionlab-0.1.5/fusionlab/segmentation/base.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/segmentation/resunet/resunet.py` & `fusionlab-0.1.5/fusionlab/segmentation/resunet/resunet.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/segmentation/resunet/tfresunet.py` & `fusionlab-0.1.5/fusionlab/segmentation/resunet/tfresunet.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/segmentation/tfbase.py` & `fusionlab-0.1.5/fusionlab/segmentation/tfbase.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/segmentation/unet/tfunet.py` & `fusionlab-0.1.5/fusionlab/segmentation/unet/tfunet.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/segmentation/unet/unet.py` & `fusionlab-0.1.5/fusionlab/segmentation/unet/unet.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/segmentation/unet2plus/tfunet2plus.py` & `fusionlab-0.1.5/fusionlab/segmentation/unet2plus/tfunet2plus.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/segmentation/unet2plus/unet2plus.py` & `fusionlab-0.1.5/fusionlab/segmentation/unet2plus/unet2plus.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/trainers/dcgan.py` & `fusionlab-0.1.5/fusionlab/trainers/dcgan.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/trainers/trainer.py` & `fusionlab-0.1.5/fusionlab/trainers/trainer.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab/utils/trace.py` & `fusionlab-0.1.5/fusionlab/utils/trace.py`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/fusionlab.egg-info/PKG-INFO` & `fusionlab-0.1.5/fusionlab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusionlab
-Version: 0.1.4
+Version: 0.1.5
 Summary: Useful packages for DL
 Home-page: https://github.com/taipingeric/fusionlab
 Author: Chih-Yang Li
 Author-email: taipingeric@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fusionlab-0.1.4/fusionlab.egg-info/SOURCES.txt` & `fusionlab-0.1.5/fusionlab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fusionlab-0.1.4/setup.py` & `fusionlab-0.1.5/setup.py`

 * *Files identical despite different names*

