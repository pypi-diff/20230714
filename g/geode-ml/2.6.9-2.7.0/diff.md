# Comparing `tmp/geode-ml-2.6.9.tar.gz` & `tmp/geode-ml-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geode-ml-2.6.9.tar", last modified: Tue May  2 16:20:09 2023, max compression
+gzip compressed data, was "geode-ml-2.7.0.tar", last modified: Fri Jul 14 14:29:59 2023, max compression
```

## Comparing `geode-ml-2.6.9.tar` & `geode-ml-2.7.0.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 16:20:09.836173 geode-ml-2.6.9/
--rw-rw-rw-   0        0        0     1089 2022-08-12 21:19:04.000000 geode-ml-2.6.9/LICENSE
--rw-rw-rw-   0        0        0     3803 2023-05-02 16:20:09.834206 geode-ml-2.6.9/PKG-INFO
--rw-rw-rw-   0        0        0     1909 2023-02-21 17:44:50.000000 geode-ml-2.6.9/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 16:20:09.816170 geode-ml-2.6.9/geode/
--rw-rw-rw-   0        0        0       74 2023-05-02 16:15:26.000000 geode-ml-2.6.9/geode/__init__.py
--rw-rw-rw-   0        0        0    21109 2023-04-04 21:38:51.000000 geode-ml-2.6.9/geode/datasets.py
--rw-rw-rw-   0        0        0     3727 2023-04-04 20:48:50.000000 geode-ml-2.6.9/geode/losses.py
--rw-rw-rw-   0        0        0     6703 2023-04-04 20:48:50.000000 geode-ml-2.6.9/geode/metrics.py
--rw-rw-rw-   0        0        0    22374 2023-05-02 16:18:39.000000 geode-ml-2.6.9/geode/models.py
--rw-rw-rw-   0        0        0    17934 2023-04-04 21:51:54.000000 geode-ml-2.6.9/geode/utilities.py
-drwxrwxrwx   0        0        0        0 2023-05-02 16:20:09.831172 geode-ml-2.6.9/geode_ml.egg-info/
--rw-rw-rw-   0        0        0     3803 2023-05-02 16:20:09.000000 geode-ml-2.6.9/geode_ml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2023-05-02 16:20:09.000000 geode-ml-2.6.9/geode_ml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 16:20:09.000000 geode-ml-2.6.9/geode_ml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2023-05-02 16:20:09.000000 geode-ml-2.6.9/geode_ml.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-02 16:20:09.000000 geode-ml-2.6.9/geode_ml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      960 2023-05-02 16:15:26.000000 geode-ml-2.6.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-02 16:20:09.836173 geode-ml-2.6.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-14 14:29:59.829506 geode-ml-2.7.0/
+-rw-rw-rw-   0        0        0     1089 2022-08-12 21:19:04.000000 geode-ml-2.7.0/LICENSE
+-rw-rw-rw-   0        0        0     3676 2023-07-14 14:29:59.828503 geode-ml-2.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1782 2023-07-14 14:25:42.000000 geode-ml-2.7.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 14:29:59.809054 geode-ml-2.7.0/geode/
+-rw-rw-rw-   0        0        0       74 2023-07-14 14:27:11.000000 geode-ml-2.7.0/geode/__init__.py
+-rw-rw-rw-   0        0        0    21111 2023-05-02 21:04:51.000000 geode-ml-2.7.0/geode/datasets.py
+-rw-rw-rw-   0        0        0     2522 2023-05-09 16:10:45.000000 geode-ml-2.7.0/geode/losses.py
+-rw-rw-rw-   0        0        0    22548 2023-07-14 14:25:16.000000 geode-ml-2.7.0/geode/models.py
+-rw-rw-rw-   0        0        0    17934 2023-04-04 21:51:54.000000 geode-ml-2.7.0/geode/utilities.py
+drwxrwxrwx   0        0        0        0 2023-07-14 14:29:59.825508 geode-ml-2.7.0/geode_ml.egg-info/
+-rw-rw-rw-   0        0        0     3676 2023-07-14 14:29:59.000000 geode-ml-2.7.0/geode_ml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-07-14 14:29:59.000000 geode-ml-2.7.0/geode_ml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 14:29:59.000000 geode-ml-2.7.0/geode_ml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      129 2023-07-14 14:29:59.000000 geode-ml-2.7.0/geode_ml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-14 14:29:59.000000 geode-ml-2.7.0/geode_ml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      981 2023-07-14 14:26:47.000000 geode-ml-2.7.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-14 14:29:59.829506 geode-ml-2.7.0/setup.cfg
```

### Comparing `geode-ml-2.6.9/LICENSE` & `geode-ml-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geode-ml-2.6.9/PKG-INFO` & `geode-ml-2.7.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geode-ml
-Version: 2.6.9
+Version: 2.7.0
 Summary: Clases and methods to help with the creation of geospatial training datasets and deep-learning models.
 Author-email: Matt Reichenbach <matthew.reichenbach@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 mpreichenbach
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -67,19 +67,14 @@
 
 The geode.losses module
 --------------------
 
 The losses module contains custom loss functions for model training; these may be removed in the future when implemented
 in Tensorflow.
 
-The geode.metrics module
---------------------
-
-The metrics module contains useful metrics for testing model performance.
-
 The geode.models module
 --------------------
 
 The models module contains the classes:
 
 1. Segmentation
 	* subclass of the tensorflow.keras.Model class to be used for image segmentation
```

### Comparing `geode-ml-2.6.9/README.md` & `geode-ml-2.7.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -31,19 +31,14 @@
 
 The geode.losses module
 --------------------
 
 The losses module contains custom loss functions for model training; these may be removed in the future when implemented
 in Tensorflow.
 
-The geode.metrics module
---------------------
-
-The metrics module contains useful metrics for testing model performance.
-
 The geode.models module
 --------------------
 
 The models module contains the classes:
 
 1. Segmentation
 	* subclass of the tensorflow.keras.Model class to be used for image segmentation
```

### Comparing `geode-ml-2.6.9/geode/datasets.py` & `geode-ml-2.7.0/geode/datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 class SegmentationDataset:
 
     def __init__(self, source_path: str = '',
                  polygons_path: str = '',
                  labels_path: str = '',
                  tiles_path: str = '',
                  n_channels: int = 3,
-                 tile_dimension: int = 0):
+                 tile_dimension: int = 512):
 
         """A class for defining and manipulating semantic segmentation datasets.
 
         Attributes:
             source_path: the directory containing source imagery;
             polygons_path: the directory containing subdirectories of polygon shapefiles;
             labels_path: the directory to contain label rasters;
```

### Comparing `geode-ml-2.6.9/geode/losses.py` & `geode-ml-2.7.0/geode/losses.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,52 +1,14 @@
 # losses.py
 
 from numpy import asarray, ndarray
 import tensorflow as tf
 from tensorflow.keras import backend as K
 
 
-def dice_loss(y_true: ndarray,
-              y_pred: ndarray,
-              smooth: float = 100.) -> float:
-    """Computes the dice-loss between one-hot encoded arrays, then returns a score between [0, 1].
-
-    Args:
-        y_true: tensor of ground-truth values of size (batch, height, width, n_classes);
-        y_pred: tensor of model predictions of size (batch, height, width, n_classes);
-        smooth: a value to avoid division by zero (among other things).
-
-    Returns:
-        The dice-loss score.
-
-    Raises:
-        ValueError: if smooth is less than zero.
-    """
-
-    # coerce arguments to the correct type
-    y_true = asarray(y_true)
-    y_pred = asarray(y_pred)
-    smooth = float(smooth)
-
-    # check for the correct float range
-    if smooth < 0:
-        raise ValueError("Argument smooth must be greater than or equal to zero.")
-
-    y_true = K.cast(y_true, dtype=tf.float32)
-    y_pred = K.cast(y_pred, dtype=tf.float32)
-
-    y_true_f = K.flatten(y_true)
-    y_pred_f = K.flatten(y_pred)
-    intersection = K.sum(y_true_f * y_pred_f)
-
-    dice = (2 * intersection + smooth) / (K.sum(y_true_f) + K.sum(y_pred_f) + smooth)
-
-    return 1 - dice
-
-
 def iou_loss(y_true: ndarray,
              y_pred: ndarray,
              smooth: float = 100.) -> float:
     """Computes the IoU-loss between one-hot encoded arrays, then return a loss score between [0, 1].
 
     Args:
         y_true: tensor of ground-truth values of size (batch, height, width);
```

### Comparing `geode-ml-2.6.9/geode/models.py` & `geode-ml-2.7.0/geode/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # models.py
 
-import geode.metrics as gm
 from geode.utilities import predict_raster
-from numpy import mean, unique
+from numpy import mean
 from os import listdir, makedirs
 from os.path import isdir, join
 from osgeo.gdal import Open
+from sklearn.metrics import precision_score, recall_score, jaccard_score, f1_score
 import tensorflow as tf
 from tensorflow.keras.layers import Add, BatchNormalization, Concatenate, Conv2D, Dropout, Input, MaxPooling2D, \
     UpSampling2D
 from tensorflow.keras.layers.experimental.preprocessing import Rescaling
 
 
 class SegmentationModel:
@@ -95,41 +95,44 @@
 
             # create metrics dictionary
             metrics_dict = {}
 
             # create lists for each metric
             f1_scores = []
             jaccard_scores = []
-            acc_scores = []
+            precision_scores = []
+            recall_scores = []
 
             # loop through the test subset
             for fname in sub_filenames:
                 if verbose:
                     print(fname)
 
                 # open the relevant datasets
                 y_true = Open(join(self.test_labels_path, fname)).ReadAsArray()
                 y_pred = Open(join(self.test_predictions_path, fname)).ReadAsArray()
 
                 # compute metrics
-                f1_scores.append(gm.f1(y_true=y_true,
-                                       y_pred=y_pred,
-                                       pos_label=pos_label))
-
-                jaccard_scores.append(gm.jaccard(y_true=y_true,
-                                                 y_pred=y_pred,
-                                                 pos_label=pos_label))
+                f1_scores.append(f1_score(y_true=y_true,
+                                          y_pred=y_pred))
 
-                acc_scores.append(gm.total_accuracy(y_true=y_true,
+                jaccard_scores.append(jaccard_score(y_true=y_true,
                                                     y_pred=y_pred))
 
+                precision_scores.append(precision_score(y_true=y_true,
+                                                        y_pred=y_pred))
+
+                recall_scores.append(recall_score(y_true=y_true,
+                                                  y_pred=y_true))
+
             # add scores to the metrics dictionary
             metrics_dict['f1'] = mean(f1_scores)
             metrics_dict['jaccard'] = mean(jaccard_scores)
-            metrics_dict['accuracy'] = mean(acc_scores)
+            metrics_dict['precision'] = mean(precision_scores)
+            metrics_dict['recall'] = mean(recall_scores)
 
             dname_metrics[dname] = metrics_dict
 
         # write the dictionary to a file
         if output_path is not None:
             with open(output_path, 'w') as f:
                 for key, value in dname_metrics.items():
```

### Comparing `geode-ml-2.6.9/geode/utilities.py` & `geode-ml-2.7.0/geode/utilities.py`

 * *Files identical despite different names*

### Comparing `geode-ml-2.6.9/geode_ml.egg-info/PKG-INFO` & `geode-ml-2.7.0/geode_ml.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geode-ml
-Version: 2.6.9
+Version: 2.7.0
 Summary: Clases and methods to help with the creation of geospatial training datasets and deep-learning models.
 Author-email: Matt Reichenbach <matthew.reichenbach@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 mpreichenbach
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -67,19 +67,14 @@
 
 The geode.losses module
 --------------------
 
 The losses module contains custom loss functions for model training; these may be removed in the future when implemented
 in Tensorflow.
 
-The geode.metrics module
---------------------
-
-The metrics module contains useful metrics for testing model performance.
-
 The geode.models module
 --------------------
 
 The models module contains the classes:
 
 1. Segmentation
 	* subclass of the tensorflow.keras.Model class to be used for image segmentation
```

### Comparing `geode-ml-2.6.9/pyproject.toml` & `geode-ml-2.7.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ['setuptools>=61.0.0', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'geode-ml'
-version = '2.6.9'
+version = '2.7.0'
 description = "Clases and methods to help with the creation of geospatial training datasets and deep-learning models."
 readme = 'README.md'
 license = {file='LICENSE'}
 authors = [
     {name = 'Matt Reichenbach', email='matthew.reichenbach@gmail.com'},
 ]
 requires-python = '>=3.7'
@@ -21,13 +21,14 @@
     'Operating System :: OS Independent',
 ]
 
 keywords = ['deep-learning', 'training', 'dataset', 'geospatial']
 dependencies = [
     'gdal >= 3.4',
     'numpy',
+    'scikit-learn',
     "tensorflow-gpu >= 2.7; platform_system=='Windows'",
     "tensorflow >= 2.7; platform_system=='Linux'"
 ]
 
 [project.urls]
 'Homepage' = 'https://github.com/mpreichenbach/geode-ml'
```

