# Comparing `tmp/prolog_primitives-1.1.1.tar.gz` & `tmp/prolog_primitives-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prolog_primitives-1.1.1.tar", last modified: Thu Jul 13 17:47:00 2023, max compression
+gzip compressed data, was "prolog_primitives-1.1.2.tar", last modified: Fri Jul 14 18:08:17 2023, max compression
```

## Comparing `prolog_primitives-1.1.1.tar` & `prolog_primitives-1.1.2.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:47:00.951640 prolog_primitives-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-13 17:47:00.951640 prolog_primitives-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-13 17:47:00.000000 prolog_primitives-1.1.1/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:47:00.935640 prolog_primitives-1.1.1/prolog_primitives/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-13 17:46:35.000000 prolog_primitives-1.1.1/prolog_primitives/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:47:00.943640 prolog_primitives-1.1.1/prolog_primitives/basic/
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/basic/DBManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/basic/DistributedElements.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/basic/PrimitiveWrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/basic/Session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/basic/SubRequestEvent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/basic/Utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/basic/filterKbPrimitive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/basic/nt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:47:00.947640 prolog_primitives-1.1.1/prolog_primitives/generatedProto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:46:35.000000 prolog_primitives-1.1.1/prolog_primitives/generatedProto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-07-13 17:46:35.000000 prolog_primitives-1.1.1/prolog_primitives/generatedProto/basicMessages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-13 17:46:35.000000 prolog_primitives-1.1.1/prolog_primitives/generatedProto/basicMessages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-07-13 17:46:35.000000 prolog_primitives-1.1.1/prolog_primitives/generatedProto/errorsMessages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-13 17:46:35.000000 prolog_primitives-1.1.1/prolog_primitives/generatedProto/errorsMessages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-07-13 17:46:35.000000 prolog_primitives-1.1.1/prolog_primitives/generatedProto/primitiveService_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-13 17:46:35.000000 prolog_primitives-1.1.1/prolog_primitives/generatedProto/primitiveService_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-07-13 17:46:35.000000 prolog_primitives-1.1.1/prolog_primitives/generatedProto/sideEffectsMessages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-13 17:46:35.000000 prolog_primitives-1.1.1/prolog_primitives/generatedProto/sideEffectsMessages_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:47:00.947640 prolog_primitives-1.1.1/prolog_primitives/ml_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/collections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:47:00.947640 prolog_primitives-1.1.1/prolog_primitives/ml_lib/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/dataset/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/dataset/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/dataset/fold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/dataset/randomSplit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/dataset/row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/dataset/theoryToDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:47:00.947640 prolog_primitives-1.1.1/prolog_primitives/ml_lib/neuralNetwork/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/neuralNetwork/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:47:00.951640 prolog_primitives-1.1.1/prolog_primitives/ml_lib/predictors/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/predictors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/predictors/classify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/predictors/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/predictors/score.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/predictors/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:47:00.951640 prolog_primitives-1.1.1/prolog_primitives/ml_lib/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/schema/schemaClass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/schema/theoryToSchema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:47:00.951640 prolog_primitives-1.1.1/prolog_primitives/ml_lib/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/transformations/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/transformations/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/transformations/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/transformations/one_hot_encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/transformations/schema_trasformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/transformations/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/prolog_primitives/ml_lib/transformations/transformationClass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:47:00.935640 prolog_primitives-1.1.1/prolog_primitives.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-13 17:47:00.000000 prolog_primitives-1.1.1/prolog_primitives.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-13 17:47:00.000000 prolog_primitives-1.1.1/prolog_primitives.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:47:00.000000 prolog_primitives-1.1.1/prolog_primitives.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:47:00.000000 prolog_primitives-1.1.1/prolog_primitives.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-13 17:47:00.000000 prolog_primitives-1.1.1/prolog_primitives.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-13 17:47:00.000000 prolog_primitives-1.1.1/prolog_primitives.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 17:47:00.951640 prolog_primitives-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-07-13 17:45:27.000000 prolog_primitives-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:08:17.694581 prolog_primitives-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-14 18:08:17.694581 prolog_primitives-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-14 18:08:17.000000 prolog_primitives-1.1.2/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:08:17.682581 prolog_primitives-1.1.2/prolog_primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-14 18:07:51.000000 prolog_primitives-1.1.2/prolog_primitives/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:08:17.686581 prolog_primitives-1.1.2/prolog_primitives/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/basic/DBManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/basic/DistributedElements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/basic/PrimitiveWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/basic/Session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/basic/SubRequestEvent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/basic/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/basic/filterKbPrimitive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/basic/nt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:08:17.686581 prolog_primitives-1.1.2/prolog_primitives/generatedProto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 18:07:51.000000 prolog_primitives-1.1.2/prolog_primitives/generatedProto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-07-14 18:07:51.000000 prolog_primitives-1.1.2/prolog_primitives/generatedProto/basicMessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-14 18:07:51.000000 prolog_primitives-1.1.2/prolog_primitives/generatedProto/basicMessages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-07-14 18:07:51.000000 prolog_primitives-1.1.2/prolog_primitives/generatedProto/errorsMessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-14 18:07:51.000000 prolog_primitives-1.1.2/prolog_primitives/generatedProto/errorsMessages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-07-14 18:07:51.000000 prolog_primitives-1.1.2/prolog_primitives/generatedProto/primitiveService_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-14 18:07:51.000000 prolog_primitives-1.1.2/prolog_primitives/generatedProto/primitiveService_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-07-14 18:07:51.000000 prolog_primitives-1.1.2/prolog_primitives/generatedProto/sideEffectsMessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-14 18:07:51.000000 prolog_primitives-1.1.2/prolog_primitives/generatedProto/sideEffectsMessages_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:08:17.686581 prolog_primitives-1.1.2/prolog_primitives/ml_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/collections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:08:17.690581 prolog_primitives-1.1.2/prolog_primitives/ml_lib/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/dataset/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/dataset/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/dataset/fold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/dataset/randomSplit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/dataset/row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/dataset/theoryToDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:08:17.690581 prolog_primitives-1.1.2/prolog_primitives/ml_lib/neuralNetwork/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/neuralNetwork/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:08:17.690581 prolog_primitives-1.1.2/prolog_primitives/ml_lib/predictors/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/predictors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/predictors/classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/predictors/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/predictors/score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/predictors/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:08:17.694581 prolog_primitives-1.1.2/prolog_primitives/ml_lib/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/schema/schemaClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/schema/theoryToSchema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:08:17.694581 prolog_primitives-1.1.2/prolog_primitives/ml_lib/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/transformations/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/transformations/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/transformations/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/transformations/one_hot_encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/transformations/schema_trasformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/transformations/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/transformations/transformationClass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:08:17.682581 prolog_primitives-1.1.2/prolog_primitives.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-14 18:08:17.000000 prolog_primitives-1.1.2/prolog_primitives.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-14 18:08:17.000000 prolog_primitives-1.1.2/prolog_primitives.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 18:08:17.000000 prolog_primitives-1.1.2/prolog_primitives.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 18:08:17.000000 prolog_primitives-1.1.2/prolog_primitives.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-14 18:08:17.000000 prolog_primitives-1.1.2/prolog_primitives.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-14 18:08:17.000000 prolog_primitives-1.1.2/prolog_primitives.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 18:08:17.694581 prolog_primitives-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/setup.py
```

### Comparing `prolog_primitives-1.1.1/LICENSE` & `prolog_primitives-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.1/PKG-INFO` & `prolog_primitives-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prolog_primitives
-Version: 1.1.1
+Version: 1.1.2
 Summary: description here
 Home-page: https://github.com/lorenzo-osimani/prolog_primitives/
 Author: Lorenzo Osimani
 Author-email: lorenzo.osimani@studio.unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/lorenzo-osimani/prolog_primitives/issues
 Project-URL: Source, https://github.com/lorenzo-osimani/prolog_primitives/
```

### Comparing `prolog_primitives-1.1.1/prolog_primitives/basic/DBManager.py` & `prolog_primitives-1.1.2/prolog_primitives/basic/DBManager.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.1/prolog_primitives/basic/DistributedElements.py` & `prolog_primitives-1.1.2/prolog_primitives/basic/DistributedElements.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.1/prolog_primitives/basic/PrimitiveWrapper.py` & `prolog_primitives-1.1.2/prolog_primitives/basic/PrimitiveWrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,14 @@
     service = GenericPrimitive(primitive.primitive, primitive.functor, primitive.arity, executor)
     server = grpc.server(executor)
     Server.add_GenericPrimitiveServiceServicer_to_server(service, server)
     server.add_insecure_port('[::]:' + str(port))
     server.start()
     if(withDB):
         DBManager.addPrimitive(service.functor, service.arity, libraryName, "localhost", port)
-    print("Server started, listening on " + str(port))
+    print(f"Server of {primitive.functor}\{primitive.arity} started, listening on {port}", flush=True)
     return server
```

### Comparing `prolog_primitives-1.1.1/prolog_primitives/basic/Session.py` & `prolog_primitives-1.1.2/prolog_primitives/basic/Session.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.1/prolog_primitives/basic/SubRequestEvent.py` & `prolog_primitives-1.1.2/prolog_primitives/basic/SubRequestEvent.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.1/prolog_primitives/basic/Utils.py` & `prolog_primitives-1.1.2/prolog_primitives/basic/Utils.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.1/prolog_primitives/basic/filterKbPrimitive.py` & `prolog_primitives-1.1.2/prolog_primitives/basic/filterKbPrimitive.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.1/prolog_primitives/basic/nt.py` & `prolog_primitives-1.1.2/prolog_primitives/basic/nt.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.1/prolog_primitives/generatedProto/basicMessages_pb2.py` & `prolog_primitives-1.1.2/prolog_primitives/generatedProto/basicMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.1/prolog_primitives/generatedProto/errorsMessages_pb2.py` & `prolog_primitives-1.1.2/prolog_primitives/generatedProto/errorsMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.1/prolog_primitives/generatedProto/primitiveService_pb2.py` & `prolog_primitives-1.1.2/prolog_primitives/generatedProto/primitiveService_pb2.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.1/prolog_primitives/generatedProto/primitiveService_pb2_grpc.py` & `prolog_primitives-1.1.2/prolog_primitives/generatedProto/primitiveService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.1/prolog_primitives/generatedProto/sideEffectsMessages_pb2.py` & `prolog_primitives-1.1.2/prolog_primitives/generatedProto/sideEffectsMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.1/prolog_primitives/ml_lib/collections.py` & `prolog_primitives-1.1.2/prolog_primitives/ml_lib/collections.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.1/prolog_primitives/ml_lib/dataset/cell.py` & `prolog_primitives-1.1.2/prolog_primitives/ml_lib/dataset/cell.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.1/prolog_primitives/ml_lib/dataset/column.py` & `prolog_primitives-1.1.2/prolog_primitives/ml_lib/dataset/column.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.1/prolog_primitives/ml_lib/dataset/fold.py` & `prolog_primitives-1.1.2/prolog_primitives/ml_lib/dataset/fold.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.1/prolog_primitives/ml_lib/dataset/randomSplit.py` & `prolog_primitives-1.1.2/prolog_primitives/ml_lib/dataset/randomSplit.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.1/prolog_primitives/ml_lib/dataset/row.py` & `prolog_primitives-1.1.2/prolog_primitives/ml_lib/dataset/row.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.1/prolog_primitives/ml_lib/dataset/theoryToDataset.py` & `prolog_primitives-1.1.2/prolog_primitives/ml_lib/dataset/theoryToDataset.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.1/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py` & `prolog_primitives-1.1.2/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.1/prolog_primitives/ml_lib/launcher.py` & `prolog_primitives-1.1.2/prolog_primitives/ml_lib/launcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     executor = ThreadPoolExecutor(max_workers=len(primitives))
 
     for primitive in primitives:
         #future = executor.submit(launchPrimitive, primitive, port)
         launchPrimitive(primitive, port)
         port += 1
 
-    print(f"Servers listening from {initialport} to {port-1}")
+    print(f"Servers listening from {initialport} to {port-1}", flush=True)
 
     try:
         for server in servers:
             server.wait_for_termination()
     except (Exception, KeyboardInterrupt, SystemExit) as inst:
         executor.shutdown(wait=False, cancel_futures=True)
         for server in servers:
```

### Comparing `prolog_primitives-1.1.1/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py` & `prolog_primitives-1.1.2/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.1/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py` & `prolog_primitives-1.1.2/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.1/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py` & `prolog_primitives-1.1.2/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.1/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py` & `prolog_primitives-1.1.2/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.1/prolog_primitives/ml_lib/predictors/classify.py` & `prolog_primitives-1.1.2/prolog_primitives/ml_lib/predictors/classify.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.1/prolog_primitives/ml_lib/predictors/predict.py` & `prolog_primitives-1.1.2/prolog_primitives/ml_lib/predictors/predict.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.1/prolog_primitives/ml_lib/predictors/score.py` & `prolog_primitives-1.1.2/prolog_primitives/ml_lib/predictors/score.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.1/prolog_primitives/ml_lib/predictors/train.py` & `prolog_primitives-1.1.2/prolog_primitives/ml_lib/predictors/train.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             output = tf.stack(output, axis = 1)
             input = tf.stack(input, axis = 1)
             optimizer = tf.keras.optimizers.Adam(learning_rate=params["learning_rate"])
             
             model.compile(
                 loss = params["loss"],
                 optimizer=optimizer,
-                metrics=["mse"],
+                metrics=['mae', 'mse'],
             )
             model.fit(x=input,y=output, batch_size=params["batch"], epochs=params["epoch"])
             id = SharedCollections().addModel(model)
             yield request.replySuccess(substitutions={
                 predictor_out_ref.var: Utils.buildConstantArgumentMsg(id)
                 }, hasNext=False)
         else:
```

### Comparing `prolog_primitives-1.1.1/prolog_primitives/ml_lib/schema/schema.py` & `prolog_primitives-1.1.2/prolog_primitives/ml_lib/schema/schema.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.1/prolog_primitives/ml_lib/schema/schemaClass.py` & `prolog_primitives-1.1.2/prolog_primitives/ml_lib/schema/schemaClass.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.1/prolog_primitives/ml_lib/schema/theoryToSchema.py` & `prolog_primitives-1.1.2/prolog_primitives/ml_lib/schema/theoryToSchema.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.1/prolog_primitives/ml_lib/transformations/drop.py` & `prolog_primitives-1.1.2/prolog_primitives/ml_lib/transformations/drop.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.1/prolog_primitives/ml_lib/transformations/fit.py` & `prolog_primitives-1.1.2/prolog_primitives/ml_lib/transformations/fit.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.1/prolog_primitives/ml_lib/transformations/normalization.py` & `prolog_primitives-1.1.2/prolog_primitives/ml_lib/transformations/normalization.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.1/prolog_primitives/ml_lib/transformations/one_hot_encode.py` & `prolog_primitives-1.1.2/prolog_primitives/ml_lib/transformations/one_hot_encode.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.1/prolog_primitives/ml_lib/transformations/schema_trasformation.py` & `prolog_primitives-1.1.2/prolog_primitives/ml_lib/transformations/schema_trasformation.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.1/prolog_primitives/ml_lib/transformations/transform.py` & `prolog_primitives-1.1.2/prolog_primitives/ml_lib/transformations/transform.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.1/prolog_primitives/ml_lib/transformations/transformationClass.py` & `prolog_primitives-1.1.2/prolog_primitives/ml_lib/transformations/transformationClass.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,17 @@
     
     @abstractmethod
     def copy(self):
         pass
     
 class Normalization(Transformation):
     
-    applier = tf.keras.layers.Normalization()
-    inverter = tf.keras.layers.Normalization(invert=True)
+    def __init__(self):
+        self.applier = tf.keras.layers.Normalization()
+        self.inverter = tf.keras.layers.Normalization(invert=True)
         
     def adapt(self, inputs):
         self.applier.adapt(inputs)
         self.inverter.adapt(inputs)
         
     def copy(self):
         return Normalization()
@@ -55,52 +56,50 @@
     def __init__(self,
                  originalSchema: str,
                  layers: dict = {}):
         self.originalSchemaId = originalSchema 
         self.originalSchema = SharedCollections().getSchema(originalSchema)
         self.__layers = {}
         for attr in self.originalSchema.attributes:
-            self.__layers[attr.name] = [] + layers.get(attr.name, [])
+            self.__layers[attr.name] = layers.get(attr.name, [])
         
     def append(self, pipeline: dict):
         new_pipeline = {}
         for attr, layers in self.__layers.items():
             new_pipeline[attr] = layers + pipeline.get(attr, [])
         return Pipeline(self.originalSchemaId, new_pipeline)    
     
     def adapt(self, inputs):
         newLayers = dict.fromkeys(self.__layers.keys())
         for attr, layers in self.__layers.items():
-            data = tf.reshape(inputs[attr], (len(inputs[attr]), -1))
+            data = tf.reshape(inputs[attr], (len(inputs[attr]), 1))
             newLayers[attr] = []
             for layer in layers:
                 copied = layer.copy()
                 if(type(copied) == Normalization):
                     copied.adapt(data)
                 data = copied.applier(data)
                 newLayers[attr].append(copied)
+
         return Pipeline(self.originalSchemaId, newLayers)
         
     def apply(self, inputs):
         output = {}
         for attr, layers in self.__layers.items():
-            output[attr] = tf.reshape(inputs[attr], (len(inputs[attr]), -1))
+            output[attr] = tf.reshape(inputs[attr], (len(inputs[attr]), 1))
             for layer in layers:  
                 output[attr] = layer.applier(output[attr])
-
-            
-            
         return Dataset.from_dict(output)
         
     def invert(self, inputs):
         output = {}
         for attr, layers in self.__layers.items():
             reversedList = list(layers)
             reversedList.reverse()
-            output[attr] = tf.reshape(inputs[attr], (len(inputs[attr]), -1))
+            output[attr] = tf.reshape(inputs[attr], (len(inputs[attr]), 1))
             for layer in reversedList:  
                 output[attr] = layer.inverter(output[attr])
         return Dataset.from_dict(output)
     
     def computeFinalSchema(self) -> Schema:
         from ..schema.schemaClass import Attribute, Schema
         data = {}
```

### Comparing `prolog_primitives-1.1.1/prolog_primitives.egg-info/PKG-INFO` & `prolog_primitives-1.1.2/prolog_primitives.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prolog-primitives
-Version: 1.1.1
+Version: 1.1.2
 Summary: description here
 Home-page: https://github.com/lorenzo-osimani/prolog_primitives/
 Author: Lorenzo Osimani
 Author-email: lorenzo.osimani@studio.unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/lorenzo-osimani/prolog_primitives/issues
 Project-URL: Source, https://github.com/lorenzo-osimani/prolog_primitives/
```

### Comparing `prolog_primitives-1.1.1/prolog_primitives.egg-info/SOURCES.txt` & `prolog_primitives-1.1.2/prolog_primitives.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.1/setup.py` & `prolog_primitives-1.1.2/setup.py`

 * *Files identical despite different names*

