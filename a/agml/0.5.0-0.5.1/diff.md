# Comparing `tmp/agml-0.5.0.tar.gz` & `tmp/agml-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agml-0.5.0.tar", last modified: Tue May 23 14:13:41 2023, max compression
+gzip compressed data, was "agml-0.5.1.tar", last modified: Fri Jul 14 20:16:47 2023, max compression
```

## Comparing `agml-0.5.0.tar` & `agml-0.5.1.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-05-23 14:13:41.640323 agml-0.5.0/
--rw-r--r--   0 amoghjoshi   (501) staff       (20)       81 2022-03-29 13:30:39.000000 agml-0.5.0/AUTHORS
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    11357 2022-05-19 21:35:28.000000 agml-0.5.0/LICENSE
--rw-r--r--   0 amoghjoshi   (501) staff       (20)      210 2023-05-23 14:06:53.000000 agml-0.5.0/MANIFEST.in
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    11924 2023-05-23 14:13:41.636637 agml-0.5.0/PKG-INFO
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    10944 2023-05-23 14:06:53.000000 agml-0.5.0/README.md
-drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-05-23 14:13:41.402754 agml-0.5.0/agml/
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     1367 2023-05-23 14:13:20.000000 agml-0.5.0/agml/__init__.py
-drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-05-23 14:13:41.422173 agml-0.5.0/agml/_assets/
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     6398 2022-10-06 00:40:28.000000 agml-0.5.0/agml/_assets/model_benchmarks.json
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    38010 2023-05-23 14:06:53.000000 agml-0.5.0/agml/_assets/public_datasources.json
--rw-r--r--   0 amoghjoshi   (501) staff       (20)   481599 2023-05-23 14:06:53.000000 agml-0.5.0/agml/_assets/shape_info.pickle
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    29899 2023-05-23 14:06:53.000000 agml-0.5.0/agml/_assets/source_citations.json
--rw-r--r--   0 amoghjoshi   (501) staff       (20)      318 2022-10-23 01:02:40.000000 agml-0.5.0/agml/_assets/viz_colormaps.json
-drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-05-23 14:13:41.423099 agml-0.5.0/agml/_helios/
--rwxr-xr-x   0 amoghjoshi   (501) staff       (20)     1098 2022-10-06 00:40:28.000000 agml-0.5.0/agml/_helios/helios_install.sh
-drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-05-23 14:13:41.432109 agml-0.5.0/agml/backend/
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     1371 2022-10-06 00:40:28.000000 agml-0.5.0/agml/backend/__init__.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     7975 2023-05-23 14:06:53.000000 agml-0.5.0/agml/backend/config.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     2252 2022-10-06 00:40:28.000000 agml-0.5.0/agml/backend/experimental.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)      983 2023-05-18 17:36:50.000000 agml-0.5.0/agml/backend/random.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    10087 2023-05-23 14:06:53.000000 agml-0.5.0/agml/backend/tftorch.py
-drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-05-23 14:13:41.453503 agml-0.5.0/agml/data/
--rw-r--r--   0 amoghjoshi   (501) staff       (20)      900 2023-05-23 14:06:53.000000 agml-0.5.0/agml/data/__init__.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    15429 2023-05-23 14:06:53.000000 agml-0.5.0/agml/data/builder.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     3748 2022-03-29 13:30:39.000000 agml-0.5.0/agml/data/experimental.py
-drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-05-23 14:13:41.458346 agml-0.5.0/agml/data/exporters/
--rw-r--r--   0 amoghjoshi   (501) staff       (20)        0 2022-03-29 13:30:39.000000 agml-0.5.0/agml/data/exporters/__init__.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     9639 2022-05-19 21:43:54.000000 agml-0.5.0/agml/data/exporters/tensorflow.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     5737 2023-05-23 14:06:53.000000 agml-0.5.0/agml/data/image_loader.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    73721 2023-05-23 14:06:53.000000 agml-0.5.0/agml/data/loader.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    16197 2023-05-23 14:06:53.000000 agml-0.5.0/agml/data/manager.py
-drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-05-23 14:13:41.473743 agml-0.5.0/agml/data/managers/
--rw-r--r--   0 amoghjoshi   (501) staff       (20)      600 2022-03-29 13:30:39.000000 agml-0.5.0/agml/data/managers/__init__.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    14583 2022-10-06 00:40:28.000000 agml-0.5.0/agml/data/managers/resize.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    15928 2023-05-17 13:59:46.000000 agml-0.5.0/agml/data/managers/training.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     6074 2023-05-23 14:06:53.000000 agml-0.5.0/agml/data/managers/transform_helpers.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    26516 2023-05-23 14:06:53.000000 agml-0.5.0/agml/data/managers/transforms.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    13454 2023-05-11 17:51:20.000000 agml-0.5.0/agml/data/metadata.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    66025 2022-10-06 00:40:28.000000 agml-0.5.0/agml/data/multi_loader.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     9127 2022-10-06 00:40:28.000000 agml-0.5.0/agml/data/object.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     8528 2023-05-23 14:06:53.000000 agml-0.5.0/agml/data/point_cloud.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     6681 2022-10-06 00:40:28.000000 agml-0.5.0/agml/data/public.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     7351 2022-10-06 00:40:28.000000 agml-0.5.0/agml/data/tools.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     3137 2022-10-06 00:40:28.000000 agml-0.5.0/agml/framework.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     3504 2023-05-23 14:06:53.000000 agml-0.5.0/agml/io.py
-drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-05-23 14:13:41.518995 agml-0.5.0/agml/models/
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     1690 2023-05-23 14:06:53.000000 agml-0.5.0/agml/models/__init__.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     6551 2022-10-06 00:40:28.000000 agml-0.5.0/agml/models/base.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     2624 2022-10-06 00:40:28.000000 agml-0.5.0/agml/models/benchmarks.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     8921 2023-05-23 14:06:53.000000 agml-0.5.0/agml/models/classification.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    22088 2023-05-23 14:06:53.000000 agml-0.5.0/agml/models/detection.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     2104 2022-10-06 00:40:28.000000 agml-0.5.0/agml/models/losses.py
-drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-05-23 14:13:41.532491 agml-0.5.0/agml/models/metrics/
--rw-r--r--   0 amoghjoshi   (501) staff       (20)      729 2022-10-06 00:40:28.000000 agml-0.5.0/agml/models/metrics/__init__.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     2632 2022-10-06 00:40:28.000000 agml-0.5.0/agml/models/metrics/accuracy.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     9795 2022-10-31 22:25:12.000000 agml-0.5.0/agml/models/metrics/map.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     8321 2022-10-31 22:25:12.000000 agml-0.5.0/agml/models/preprocessing.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    14008 2023-05-23 14:06:53.000000 agml-0.5.0/agml/models/segmentation.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     4452 2023-05-23 14:06:53.000000 agml-0.5.0/agml/models/tools.py
-drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-05-23 14:13:41.575788 agml-0.5.0/agml/synthetic/
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     1052 2023-05-23 14:06:53.000000 agml-0.5.0/agml/synthetic/__init__.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    10891 2023-05-23 14:06:53.000000 agml-0.5.0/agml/synthetic/compilation.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    12123 2023-05-23 14:06:53.000000 agml-0.5.0/agml/synthetic/config.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    16172 2023-05-11 17:51:20.000000 agml-0.5.0/agml/synthetic/converter.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    20631 2023-05-23 14:06:53.000000 agml-0.5.0/agml/synthetic/generator.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     3519 2023-05-23 14:06:53.000000 agml-0.5.0/agml/synthetic/lidar_loader.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    13066 2023-01-12 19:08:43.000000 agml-0.5.0/agml/synthetic/manual.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    16844 2023-05-23 14:06:53.000000 agml-0.5.0/agml/synthetic/options.py
-drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-05-23 14:13:41.581311 agml-0.5.0/agml/synthetic/synthetic_data_generation/
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     1740 2023-05-23 14:06:53.000000 agml-0.5.0/agml/synthetic/synthetic_data_generation/CMakeLists.txt
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    10067 2023-05-23 14:06:53.000000 agml-0.5.0/agml/synthetic/synthetic_data_generation/generate.cpp
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     7806 2023-01-12 19:08:43.000000 agml-0.5.0/agml/synthetic/tools.py
-drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-05-23 14:13:41.608640 agml-0.5.0/agml/utils/
--rw-r--r--   0 amoghjoshi   (501) staff       (20)      600 2021-10-22 20:11:12.000000 agml-0.5.0/agml/utils/__init__.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     4429 2022-10-06 00:40:28.000000 agml-0.5.0/agml/utils/data.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     6589 2022-10-06 00:40:28.000000 agml-0.5.0/agml/utils/downloads.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     4734 2023-05-23 14:06:53.000000 agml-0.5.0/agml/utils/general.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     3586 2023-05-23 14:06:53.000000 agml-0.5.0/agml/utils/image.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     3831 2023-05-23 14:06:53.000000 agml-0.5.0/agml/utils/io.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     2688 2022-10-06 00:40:28.000000 agml-0.5.0/agml/utils/logging.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     2371 2022-10-06 00:40:28.000000 agml-0.5.0/agml/utils/random.py
-drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-05-23 14:13:41.634073 agml-0.5.0/agml/viz/
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     1365 2023-05-23 14:06:53.000000 agml-0.5.0/agml/viz/__init__.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    14220 2023-05-23 14:06:53.000000 agml-0.5.0/agml/viz/boxes.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     2309 2023-05-23 14:06:53.000000 agml-0.5.0/agml/viz/display.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     4786 2023-05-23 14:06:53.000000 agml-0.5.0/agml/viz/general.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     5345 2023-05-23 14:06:53.000000 agml-0.5.0/agml/viz/inspection.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     5095 2023-05-23 14:06:53.000000 agml-0.5.0/agml/viz/labels.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    10434 2023-05-23 14:06:53.000000 agml-0.5.0/agml/viz/masks.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     2404 2023-05-23 14:06:53.000000 agml-0.5.0/agml/viz/point_clouds.py
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     6828 2023-05-23 14:06:53.000000 agml-0.5.0/agml/viz/tools.py
-drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-05-23 14:13:41.408998 agml-0.5.0/agml.egg-info/
--rw-r--r--   0 amoghjoshi   (501) staff       (20)    11924 2023-05-23 14:13:40.000000 agml-0.5.0/agml.egg-info/PKG-INFO
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     2074 2023-05-23 14:13:40.000000 agml-0.5.0/agml.egg-info/SOURCES.txt
--rw-r--r--   0 amoghjoshi   (501) staff       (20)        1 2023-05-23 14:13:40.000000 agml-0.5.0/agml.egg-info/dependency_links.txt
--rw-r--r--   0 amoghjoshi   (501) staff       (20)      318 2023-05-23 14:13:40.000000 agml-0.5.0/agml.egg-info/requires.txt
--rw-r--r--   0 amoghjoshi   (501) staff       (20)        5 2023-05-23 14:13:40.000000 agml-0.5.0/agml.egg-info/top_level.txt
--rw-r--r--   0 amoghjoshi   (501) staff       (20)       38 2023-05-23 14:13:41.640992 agml-0.5.0/setup.cfg
--rw-r--r--   0 amoghjoshi   (501) staff       (20)     2551 2022-10-14 14:32:05.000000 agml-0.5.0/setup.py
+drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-07-14 20:16:47.971303 agml-0.5.1/
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)       81 2022-03-29 13:30:39.000000 agml-0.5.1/AUTHORS
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    11357 2022-05-19 21:35:28.000000 agml-0.5.1/LICENSE
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)      210 2023-05-23 14:06:53.000000 agml-0.5.1/MANIFEST.in
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    12081 2023-07-14 20:16:47.970569 agml-0.5.1/PKG-INFO
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    11101 2023-07-14 20:16:30.000000 agml-0.5.1/README.md
+drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-07-14 20:16:47.748164 agml-0.5.1/agml/
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     1367 2023-07-14 20:16:13.000000 agml-0.5.1/agml/__init__.py
+drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-07-14 20:16:47.778521 agml-0.5.1/agml/_assets/
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     6398 2022-10-06 00:40:28.000000 agml-0.5.1/agml/_assets/model_benchmarks.json
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    39224 2023-07-14 20:16:30.000000 agml-0.5.1/agml/_assets/public_datasources.json
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)   481766 2023-07-14 20:16:30.000000 agml-0.5.1/agml/_assets/shape_info.pickle
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    30005 2023-07-14 19:58:36.000000 agml-0.5.1/agml/_assets/source_citations.json
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)      318 2022-10-23 01:02:40.000000 agml-0.5.1/agml/_assets/viz_colormaps.json
+drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-07-14 20:16:47.782952 agml-0.5.1/agml/_helios/
+-rwxr-xr-x   0 amoghjoshi   (501) staff       (20)     1098 2022-10-06 00:40:28.000000 agml-0.5.1/agml/_helios/helios_install.sh
+drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-07-14 20:16:47.788765 agml-0.5.1/agml/backend/
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     1371 2022-10-06 00:40:28.000000 agml-0.5.1/agml/backend/__init__.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     7975 2023-05-23 14:06:53.000000 agml-0.5.1/agml/backend/config.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     2252 2022-10-06 00:40:28.000000 agml-0.5.1/agml/backend/experimental.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)      983 2023-05-18 17:36:50.000000 agml-0.5.1/agml/backend/random.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    10087 2023-05-23 14:06:53.000000 agml-0.5.1/agml/backend/tftorch.py
+drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-07-14 20:16:47.828419 agml-0.5.1/agml/data/
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)      900 2023-05-23 14:06:53.000000 agml-0.5.1/agml/data/__init__.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    15429 2023-05-23 14:06:53.000000 agml-0.5.1/agml/data/builder.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     3748 2022-03-29 13:30:39.000000 agml-0.5.1/agml/data/experimental.py
+drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-07-14 20:16:47.839719 agml-0.5.1/agml/data/exporters/
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)        0 2022-03-29 13:30:39.000000 agml-0.5.1/agml/data/exporters/__init__.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     9639 2022-05-19 21:43:54.000000 agml-0.5.1/agml/data/exporters/tensorflow.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     5737 2023-05-23 14:06:53.000000 agml-0.5.1/agml/data/image_loader.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    75355 2023-06-05 14:07:06.000000 agml-0.5.1/agml/data/loader.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    16197 2023-05-23 14:06:53.000000 agml-0.5.1/agml/data/manager.py
+drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-07-14 20:16:47.851578 agml-0.5.1/agml/data/managers/
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)      600 2022-03-29 13:30:39.000000 agml-0.5.1/agml/data/managers/__init__.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    14583 2022-10-06 00:40:28.000000 agml-0.5.1/agml/data/managers/resize.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    15928 2023-05-17 13:59:46.000000 agml-0.5.1/agml/data/managers/training.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     6074 2023-05-23 14:06:53.000000 agml-0.5.1/agml/data/managers/transform_helpers.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    26516 2023-05-23 14:06:53.000000 agml-0.5.1/agml/data/managers/transforms.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    13454 2023-05-11 17:51:20.000000 agml-0.5.1/agml/data/metadata.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    66025 2022-10-06 00:40:28.000000 agml-0.5.1/agml/data/multi_loader.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     9127 2022-10-06 00:40:28.000000 agml-0.5.1/agml/data/object.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     8528 2023-05-23 14:06:53.000000 agml-0.5.1/agml/data/point_cloud.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     6681 2022-10-06 00:40:28.000000 agml-0.5.1/agml/data/public.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     7351 2022-10-06 00:40:28.000000 agml-0.5.1/agml/data/tools.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     3137 2022-10-06 00:40:28.000000 agml-0.5.1/agml/framework.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     3796 2023-06-08 14:31:07.000000 agml-0.5.1/agml/io.py
+drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-07-14 20:16:47.888201 agml-0.5.1/agml/models/
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     1690 2023-05-23 14:06:53.000000 agml-0.5.1/agml/models/__init__.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     6551 2022-10-06 00:40:28.000000 agml-0.5.1/agml/models/base.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     2624 2022-10-06 00:40:28.000000 agml-0.5.1/agml/models/benchmarks.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     8921 2023-05-23 14:06:53.000000 agml-0.5.1/agml/models/classification.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    22088 2023-05-23 14:06:53.000000 agml-0.5.1/agml/models/detection.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     2104 2022-10-06 00:40:28.000000 agml-0.5.1/agml/models/losses.py
+drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-07-14 20:16:47.903008 agml-0.5.1/agml/models/metrics/
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)      729 2022-10-06 00:40:28.000000 agml-0.5.1/agml/models/metrics/__init__.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     2632 2022-10-06 00:40:28.000000 agml-0.5.1/agml/models/metrics/accuracy.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     9795 2022-10-31 22:25:12.000000 agml-0.5.1/agml/models/metrics/map.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     8321 2022-10-31 22:25:12.000000 agml-0.5.1/agml/models/preprocessing.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    14006 2023-06-05 18:39:24.000000 agml-0.5.1/agml/models/segmentation.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     4452 2023-05-23 14:06:53.000000 agml-0.5.1/agml/models/tools.py
+drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-07-14 20:16:47.932529 agml-0.5.1/agml/synthetic/
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     1052 2023-05-23 14:06:53.000000 agml-0.5.1/agml/synthetic/__init__.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    10891 2023-05-23 14:06:53.000000 agml-0.5.1/agml/synthetic/compilation.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    12123 2023-05-23 14:06:53.000000 agml-0.5.1/agml/synthetic/config.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    16172 2023-05-11 17:51:20.000000 agml-0.5.1/agml/synthetic/converter.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    20832 2023-06-05 14:56:01.000000 agml-0.5.1/agml/synthetic/generator.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     3519 2023-05-23 14:06:53.000000 agml-0.5.1/agml/synthetic/lidar_loader.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    13066 2023-01-12 19:08:43.000000 agml-0.5.1/agml/synthetic/manual.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    16872 2023-06-05 14:56:01.000000 agml-0.5.1/agml/synthetic/options.py
+drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-07-14 20:16:47.943087 agml-0.5.1/agml/synthetic/synthetic_data_generation/
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     1740 2023-05-23 14:06:53.000000 agml-0.5.1/agml/synthetic/synthetic_data_generation/CMakeLists.txt
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    10553 2023-06-05 14:56:01.000000 agml-0.5.1/agml/synthetic/synthetic_data_generation/generate.cpp
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     7806 2023-01-12 19:08:43.000000 agml-0.5.1/agml/synthetic/tools.py
+drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-07-14 20:16:47.959672 agml-0.5.1/agml/utils/
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)      600 2021-10-22 20:11:12.000000 agml-0.5.1/agml/utils/__init__.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     4429 2022-10-06 00:40:28.000000 agml-0.5.1/agml/utils/data.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     6589 2022-10-06 00:40:28.000000 agml-0.5.1/agml/utils/downloads.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     4734 2023-05-23 14:06:53.000000 agml-0.5.1/agml/utils/general.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     3586 2023-05-23 14:06:53.000000 agml-0.5.1/agml/utils/image.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     3831 2023-05-23 14:06:53.000000 agml-0.5.1/agml/utils/io.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     2688 2022-10-06 00:40:28.000000 agml-0.5.1/agml/utils/logging.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     2371 2022-10-06 00:40:28.000000 agml-0.5.1/agml/utils/random.py
+drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-07-14 20:16:47.968819 agml-0.5.1/agml/viz/
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     1365 2023-05-23 14:06:53.000000 agml-0.5.1/agml/viz/__init__.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    14278 2023-06-08 14:34:48.000000 agml-0.5.1/agml/viz/boxes.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     2309 2023-05-23 14:06:53.000000 agml-0.5.1/agml/viz/display.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     4786 2023-05-23 14:06:53.000000 agml-0.5.1/agml/viz/general.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     5345 2023-05-23 14:06:53.000000 agml-0.5.1/agml/viz/inspection.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     5095 2023-05-23 14:06:53.000000 agml-0.5.1/agml/viz/labels.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    10434 2023-05-23 14:06:53.000000 agml-0.5.1/agml/viz/masks.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     2404 2023-05-23 14:06:53.000000 agml-0.5.1/agml/viz/point_clouds.py
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     6828 2023-05-23 14:06:53.000000 agml-0.5.1/agml/viz/tools.py
+drwxr-xr-x   0 amoghjoshi   (501) staff       (20)        0 2023-07-14 20:16:47.755929 agml-0.5.1/agml.egg-info/
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)    12081 2023-07-14 20:16:47.000000 agml-0.5.1/agml.egg-info/PKG-INFO
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     2074 2023-07-14 20:16:47.000000 agml-0.5.1/agml.egg-info/SOURCES.txt
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)        1 2023-07-14 20:16:47.000000 agml-0.5.1/agml.egg-info/dependency_links.txt
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)      318 2023-07-14 20:16:47.000000 agml-0.5.1/agml.egg-info/requires.txt
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)        5 2023-07-14 20:16:47.000000 agml-0.5.1/agml.egg-info/top_level.txt
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)       38 2023-07-14 20:16:47.971692 agml-0.5.1/setup.cfg
+-rw-r--r--   0 amoghjoshi   (501) staff       (20)     2551 2022-10-14 14:32:05.000000 agml-0.5.1/setup.py
```

### Comparing `agml-0.5.0/LICENSE` & `agml-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/PKG-INFO` & `agml-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agml
-Version: 0.5.0
+Version: 0.5.1
 Summary: A comprehensive library for agricultural deep learning
 Home-page: https://github.com/plant-ai-biophysics-lab/AgML
 Author: UC Davis Plant AI and Biophysics Lab
 Author-email: jmearles@ucdavis.edu
 Maintainer: Amogh Joshi
 Maintainer-email: amnjoshi@ucdavis.edu
 License: UNKNOWN
@@ -161,14 +161,15 @@
 [white_grapes_and_leaves_segmentation](https://github.com/Project-AgML/AgML/blob/main/docs/datasets/white_grapes_and_leaves_segmentation.md) | Semantic Segmentation | 273 | 
 [ghai_romaine_detection](https://github.com/Project-AgML/AgML/blob/main/docs/datasets/ghai_romaine_detection.md) | Object Detection | 500 |
 [ghai_green_cabbage_detection](https://github.com/Project-AgML/AgML/blob/main/docs/datasets/ghai_green_cabbage_detection.md) | Object Detection | 500 |
 [ghai_iceberg_lettuce_detection](https://github.com/Project-AgML/AgML/blob/main/docs/datasets/ghai_iceberg_lettuce_detection.md) | Object Detection | 500 |
 [riseholme_strawberry_classification_2021](https://github.com/Project-AgML/AgML/blob/main/docs/datasets/riseholme_strawberry_classification_2021.md) | Image Classification | 3520 |
 [ghai_broccoli_detection](https://github.com/Project-AgML/AgML/blob/main/docs/datasets/ghai_broccoli_detection.md) | Object Detection | 500 |
 [bean_synthetic_earlygrowth_aerial](https://github.com/Project-AgML/AgML/blob/main/docs/datasets/bean_synthetic_earlygrowth_aerial.md) | Semantic Segmentation | 2500 |
+[ghai_strawberry_fruit_detection](https://github.com/Project-AgML/AgML/blob/main/docs/datasets/ghai_strawberry_fruit_detection.md) | Object Detection | 500 |
 
 ## Usage Information
 
 ### Using Public Agricultural Data
 
 AgML aims to provide easy access to a range of existing public agricultural datasets The core of AgML's public data pipeline is 
 [`AgMLDataLoader`](/agml/data/loader.py). You can use the `AgMLDataLoader` or `agml.data.download_public_dataset()` to download 
@@ -191,9 +192,9 @@
 ## Contributions
 
 We welcome contributions! If you would like to contribute a new feature, fix an issue that you've noticed, or even just mention
 a bug or feature that you would like to see implemented, please don't hesitate to use the *Issues* tab to bring it to our attention.
 See the [contributing guidelines](/CONTRIBUTING.md) for more information.
 
 ## Funding
-This project is partly funded by the [National AI Institute for Food Systems (AIFS)](https://aifs.ucdavis.edu
+This project is partly funded by the [National AI Institute for Food Systems (AIFS)](https://aifs.ucdavis.ed
```

### Comparing `agml-0.5.0/README.md` & `agml-0.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -133,14 +133,15 @@
 [white_grapes_and_leaves_segmentation](https://github.com/Project-AgML/AgML/blob/main/docs/datasets/white_grapes_and_leaves_segmentation.md) | Semantic Segmentation | 273 | 
 [ghai_romaine_detection](https://github.com/Project-AgML/AgML/blob/main/docs/datasets/ghai_romaine_detection.md) | Object Detection | 500 |
 [ghai_green_cabbage_detection](https://github.com/Project-AgML/AgML/blob/main/docs/datasets/ghai_green_cabbage_detection.md) | Object Detection | 500 |
 [ghai_iceberg_lettuce_detection](https://github.com/Project-AgML/AgML/blob/main/docs/datasets/ghai_iceberg_lettuce_detection.md) | Object Detection | 500 |
 [riseholme_strawberry_classification_2021](https://github.com/Project-AgML/AgML/blob/main/docs/datasets/riseholme_strawberry_classification_2021.md) | Image Classification | 3520 |
 [ghai_broccoli_detection](https://github.com/Project-AgML/AgML/blob/main/docs/datasets/ghai_broccoli_detection.md) | Object Detection | 500 |
 [bean_synthetic_earlygrowth_aerial](https://github.com/Project-AgML/AgML/blob/main/docs/datasets/bean_synthetic_earlygrowth_aerial.md) | Semantic Segmentation | 2500 |
+[ghai_strawberry_fruit_detection](https://github.com/Project-AgML/AgML/blob/main/docs/datasets/ghai_strawberry_fruit_detection.md) | Object Detection | 500 |
 
 ## Usage Information
 
 ### Using Public Agricultural Data
 
 AgML aims to provide easy access to a range of existing public agricultural datasets The core of AgML's public data pipeline is 
 [`AgMLDataLoader`](/agml/data/loader.py). You can use the `AgMLDataLoader` or `agml.data.download_public_dataset()` to download 
@@ -163,8 +164,8 @@
 ## Contributions
 
 We welcome contributions! If you would like to contribute a new feature, fix an issue that you've noticed, or even just mention
 a bug or feature that you would like to see implemented, please don't hesitate to use the *Issues* tab to bring it to our attention.
 See the [contributing guidelines](/CONTRIBUTING.md) for more information.
 
 ## Funding
-This project is partly funded by the [National AI Institute for Food Systems (AIFS)](https://aifs.ucdavis.edu
+This project is partly funded by the [National AI Institute for Food Systems (AIFS)](https://aifs.ucdavis.ed
```

### Comparing `agml-0.5.0/agml/__init__.py` & `agml-0.5.1/agml/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = '0.5.0'
+__version__ = '0.5.1'
 __all__ = ['data', 'synthetic', 'backend', 'viz', 'io']
 
 
 # If AgML is being imported for the first time, then we need to setup
 # the module, namely prepping the config file.
 def _setup():
     import os as _os
```

### Comparing `agml-0.5.0/agml/_assets/model_benchmarks.json` & `agml-0.5.1/agml/_assets/model_benchmarks.json`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/_assets/public_datasources.json` & `agml-0.5.1/agml/_assets/public_datasources.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722222222222222%*

 * *Differences: {"'ghai_strawberry_fruit_detection'": "OrderedDict([('classes', OrderedDict([('1', 'Bud'), ('2', "*

 * *                                      "'Calyx'), ('3', 'Detached Fruit'), ('4', 'Flower'), ('5', "*

 * *                                      "'Large green'), ('6', 'Leaf'), ('7', 'Ripe fruit'), ('8', "*

 * *                                      "'Small Green'), ('9', 'Stem'), ('10', 'Unripe fruit')])), "*

 * *                                      "('ml_task', 'object_detection'), ('ag_task', "*

 * *                               […]*

```diff
@@ -481,14 +481,54 @@
             "std": [
                 0.253168523311615,
                 0.26515713334083557,
                 0.2393222600221634
             ]
         }
     },
+    "ghai_strawberry_fruit_detection": {
+        "ag_task": "crop_detection",
+        "annotation_format": "coco_json",
+        "classes": {
+            "1": "Bud",
+            "10": "Unripe fruit",
+            "2": "Calyx",
+            "3": "Detached Fruit",
+            "4": "Flower",
+            "5": "Large green",
+            "6": "Leaf",
+            "7": "Ripe fruit",
+            "8": "Small Green",
+            "9": "Stem"
+        },
+        "docs_url": "https://github.com/AxisAg/GHAIDatasets/blob/main/datasets/strawberry.md",
+        "external_image_sources": [],
+        "input_data_format": "jpg",
+        "location": {
+            "continent": "north_america",
+            "country": "usa"
+        },
+        "ml_task": "object_detection",
+        "n_images": "500",
+        "platform": "handheld/ground",
+        "real_synthetic": "real",
+        "sensor_modality": "rgb",
+        "stats": {
+            "mean": [
+                0.49159616231918335,
+                0.5238277316093445,
+                0.4485996663570404
+            ],
+            "std": [
+                0.18163496255874634,
+                0.16137710213661194,
+                0.18042609095573425
+            ]
+        }
+    },
     "grape_detection_californiaday": {
         "ag_task": "fruit_detection",
         "annotation_format": "image",
         "classes": {
             "1": "grape"
         },
         "docs_url": "",
```

### Comparing `agml-0.5.0/agml/_assets/shape_info.pickle` & `agml-0.5.1/agml/_assets/shape_info.pickle`

 * *Files 0% similar despite different names*

```diff
@@ -29020,15 +29020,15 @@
 000715b0: 0067 0000 0000 0000 0003 0000 0000 0000  .g..............
 000715c0: 009c 0000 0000 0000 007b 0000 0000 0000  .........{......
 000715d0: 0003 0000 0000 0000 009d 0000 0000 0000  ................
 000715e0: 0067 0000 0000 0000 0003 0000 0000 0000  .g..............
 000715f0: 00a1 0000 0000 0000 0061 0000 0000 0000  .........a......
 00071600: 0003 0000 0000 0000 00b5 0000 0000 0000  ................
 00071610: 007e 0000 0000 0000 0003 0000 0000 0000  .~..............
-00071620: 0094 7494 6295 1143 0000 0000 0000 6804  ..t.b..C......h.
+00071620: 0094 7494 6295 b843 0000 0000 0000 6804  ..t.b..C......h.
 00071630: 6807 4b00 8594 6809 8794 5294 284b 014d  h.K...h...R.(K.M
 00071640: 3408 8594 6a14 0200 0089 42a0 4100 0001  4...j.....B.A...
 00071650: 0000 0000 0000 0001 0000 0000 0000 0001  ................
 00071660: 0000 0000 0000 0001 0000 0000 0000 0001  ................
 00071670: 0000 0000 0000 0001 0000 0000 0000 0001  ................
 00071680: 0000 0000 0000 0002 0000 0000 0000 0001  ................
 00071690: 0000 0000 0000 0002 0000 0000 0000 0001  ................
@@ -30093,8 +30093,19 @@
 000758c0: 6809 8794 5294 284b 014b 014b 0386 9468  h...R.(K.K.K...h
 000758d0: 0e8c 0269 3894 8988 8794 5294 284b 0368  ...i8.....R.(K.h
 000758e0: 124e 4e4e 4aff ffff ff4a ffff ffff 4b00  .NNNJ....J....K.
 000758f0: 7494 6289 4318 0002 0000 0000 0000 0002  t.b.C...........
 00075900: 0000 0000 0000 0300 0000 0000 0000 9474  ...............t
 00075910: 9462 6804 6807 4b00 8594 6809 8794 5294  .bh.h.K...h...R.
 00075920: 284b 014b 0185 946a 3802 0000 8943 08c4  (K.K...j8....C..
-00075930: 0900 0000 0000 0094 7494 6286 9475 2e    ........t.b..u.
+00075930: 0900 0000 0000 0094 7494 6286 948c 1f67  ........t.b....g
+00075940: 6861 695f 7374 7261 7762 6572 7279 5f66  hai_strawberry_f
+00075950: 7275 6974 5f64 6574 6563 7469 6f6e 9468  ruit_detection.h
+00075960: 0468 074b 0085 9468 0987 9452 9428 4b01  .h.K...h...R.(K.
+00075970: 4b01 4b03 8694 680e 8c02 6938 9489 8887  K.K...h...i8....
+00075980: 9452 9428 4b03 6812 4e4e 4e4a ffff ffff  .R.(K.h.NNNJ....
+00075990: 4aff ffff ff4b 0074 9462 8943 1838 0400  J....K.t.b.C.8..
+000759a0: 0000 0000 0080 0700 0000 0000 0003 0000  ................
+000759b0: 0000 0000 0094 7494 6268 0468 074b 0085  ......t.bh.h.K..
+000759c0: 9468 0987 9452 9428 4b01 4b01 8594 6a4a  .h...R.(K.K...jJ
+000759d0: 0200 0089 4308 f401 0000 0000 0000 9474  ....C..........t
+000759e0: 9462 8694 752e                           .b..u.
```

### Comparing `agml-0.5.0/agml/_assets/source_citations.json` & `agml-0.5.1/agml/_assets/source_citations.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722222222222222%*

 * *Differences: {"'ghai_strawberry_fruit_detection'": "OrderedDict([('license', 'CC BY-SA 4.0'), ('citation', "*

 * *                                      "'')])"}*

```diff
@@ -55,14 +55,18 @@
         "citation": "",
         "license": "CC BY-SA 4.0"
     },
     "ghai_romaine_detection": {
         "citation": "",
         "license": "CC BY-SA 4.0"
     },
+    "ghai_strawberry_fruit_detection": {
+        "citation": "",
+        "license": "CC BY-SA 4.0"
+    },
     "grape_detection_californiaday": {
         "citation": "@misc{GrapeDay,\n  author    = {Plant AI and Biophysics Lab},\n  title     = {Grape Detection 2019 Day},\n  year      = {2019},\n  url       = {https://github.com/plant-ai-biophysics-lab/AgML} \n ",
         "license": ""
     },
     "grape_detection_californianight": {
         "citation": "@misc{GrapeNight,\n  author    = {Plant AI and Biophysics Lab},\n  title     = {Grape Detection 2020 Night},\n  year      = {2020},\n  url       = {https://github.com/plant-ai-biophysics-lab/AgML} \n ",
         "license": ""
```

### Comparing `agml-0.5.0/agml/_helios/helios_install.sh` & `agml-0.5.1/agml/_helios/helios_install.sh`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/backend/__init__.py` & `agml-0.5.1/agml/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/backend/config.py` & `agml-0.5.1/agml/backend/config.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/backend/experimental.py` & `agml-0.5.1/agml/backend/experimental.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/backend/random.py` & `agml-0.5.1/agml/backend/random.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/backend/tftorch.py` & `agml-0.5.1/agml/backend/tftorch.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/data/__init__.py` & `agml-0.5.1/agml/data/__init__.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/data/builder.py` & `agml-0.5.1/agml/data/builder.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/data/experimental.py` & `agml-0.5.1/agml/data/experimental.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/data/exporters/tensorflow.py` & `agml-0.5.1/agml/data/exporters/tensorflow.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/data/image_loader.py` & `agml-0.5.1/agml/data/image_loader.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/data/loader.py` & `agml-0.5.1/agml/data/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 import json
 import copy
+import glob
 from typing import Union
 from collections.abc import Sequence
 from decimal import getcontext, Decimal
 
 import numpy as np
 
 from agml.framework import AgMLSerializable
@@ -292,14 +293,46 @@
         Given the path to a Helios-generated (and converted) dataset, this method
         will generate an `AgMLDataLoader` which is constructed using similar
         semantics to the regular instantiation. This method is largely similar to
         `AgMLDataLoader.custom()`, but also takes into account the extra
         information which is provided in the `.metadata` directory of the Helios
         generated dataset, allowing it to contain potentially even more info.
         """
+        # Instantiate from a list of datasets.
+        if isinstance(name, (list, tuple)):
+            if dataset_path is None:
+                dataset_path = [None] * len(name)
+            elif isinstance(dataset_path, str):
+                dataset_path = [dataset_path] * len(name)
+            else:
+                if not len(dataset_path) == len(name):
+                    raise ValueError("The number of dataset paths must be "
+                                     "the same as the number of dataset names.")
+            datasets = [cls.helios(n, dataset_path = dp)
+                        for n, dp in zip(name, dataset_path)]
+            return cls.merge(*datasets)
+
+        # Instantiate from a wildcard pattern.
+        if isinstance(name, str) and '*' in name:
+            if dataset_path is None:
+                dataset_path = os.path.abspath(synthetic_data_save_path())
+            elif not os.path.exists(dataset_path):
+                raise NotADirectoryError(
+                    f"Existing directory '{dataset_path}' for dataset of name "
+                    f"{name} not found, pass a custom path if you want to use "
+                    f"a custom dataset path for the dataset.")
+
+            # Get the list of datasets.
+            possible_datasets = glob.glob(os.path.join(dataset_path, name))
+            if len(possible_datasets) == 0:
+                raise ValueError(f"No datasets found for pattern: {name}.")
+            datasets = [cls.helios(os.path.basename(p), dataset_path = dataset_path)
+                        for p in sorted(possible_datasets)]
+            return cls.merge(*datasets)
+
         # Locate the path to the dataset, using synthetic semantics.
         if dataset_path is None:
             dataset_path = os.path.abspath(
                 os.path.join(synthetic_data_save_path(), name))
             if not os.path.exists(dataset_path):
                 raise NotADirectoryError(
                     f"Existing directory '{dataset_path}' for dataset of name "
```

### Comparing `agml-0.5.0/agml/data/manager.py` & `agml-0.5.1/agml/data/manager.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/data/managers/__init__.py` & `agml-0.5.1/agml/data/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/data/managers/resize.py` & `agml-0.5.1/agml/data/managers/resize.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/data/managers/training.py` & `agml-0.5.1/agml/data/managers/training.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/data/managers/transform_helpers.py` & `agml-0.5.1/agml/data/managers/transform_helpers.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/data/managers/transforms.py` & `agml-0.5.1/agml/data/managers/transforms.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/data/metadata.py` & `agml-0.5.1/agml/data/metadata.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/data/multi_loader.py` & `agml-0.5.1/agml/data/multi_loader.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/data/object.py` & `agml-0.5.1/agml/data/object.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/data/point_cloud.py` & `agml-0.5.1/agml/data/point_cloud.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/data/public.py` & `agml-0.5.1/agml/data/public.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/data/tools.py` & `agml-0.5.1/agml/data/tools.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/framework.py` & `agml-0.5.1/agml/framework.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/io.py` & `agml-0.5.1/agml/io.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import random
 import inspect
 
+import cv2
+
 from agml.utils.io import (
     get_file_list as _get_file_list,
     get_dir_list as _get_dir_list,
     nested_file_list as _get_nested_file_list,
     nested_dir_list as _get_nested_dir_list,
     recursive_dirname as _recursive_dirname
 )
@@ -108,9 +110,19 @@
 
     Returns:
         str: The path to the random file.
     """
     return random.choice(get_file_list(path, **kwargs))
 
 
+def read_image(path, **kwargs):
+    """Reads an image from a file.
+
+    Args:
+        path (str): The path to the image file.
+        **kwargs: Keyword arguments to pass to `cv2.imread`.
 
+    Returns:
+        numpy.ndarray: The image.
+    """
+    return cv2.imread(path, **kwargs)
```

### Comparing `agml-0.5.0/agml/models/__init__.py` & `agml-0.5.1/agml/models/__init__.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/models/base.py` & `agml-0.5.1/agml/models/base.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/models/benchmarks.py` & `agml-0.5.1/agml/models/benchmarks.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/models/classification.py` & `agml-0.5.1/agml/models/classification.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/models/detection.py` & `agml-0.5.1/agml/models/detection.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/models/losses.py` & `agml-0.5.1/agml/models/losses.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/models/metrics/__init__.py` & `agml-0.5.1/agml/models/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/models/metrics/accuracy.py` & `agml-0.5.1/agml/models/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/models/metrics/map.py` & `agml-0.5.1/agml/models/metrics/map.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/models/preprocessing.py` & `agml-0.5.1/agml/models/preprocessing.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/models/segmentation.py` & `agml-0.5.1/agml/models/segmentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 from agml.models.base import AgMLModelBase
 from agml.models.benchmarks import BenchmarkMetadata
 from agml.models.tools import auto_move_data, imagenet_style_process
 from agml.data.public import source
 from agml.utils.general import resolve_list_value
 from agml.utils.image import resolve_image_size
-from agml.viz.masks import show_image_with_overlaid_mask, show_image_and_mask
+from agml.viz.masks import show_image_and_overlaid_mask, show_image_and_mask
 
 # This is last since `agml.models.base` will check for PyTorch Lightning,
 # and PyTorch Lightning automatically installed torchmetrics with it.
 from torchmetrics import JaccardIndex as IoU
 
 
 class DeepLabV3Transfer(nn.Module):
@@ -246,15 +246,15 @@
         Returns
         -------
         The matplotlib figure containing the image.
         """
         image = self._expand_input_images(image)[0]
         mask = self.predict(image, **kwargs)
         if overlay:
-            return show_image_with_overlaid_mask(image, mask, **kwargs)
+            return show_image_and_overlaid_mask(image, mask, **kwargs)
         return show_image_and_mask(image, mask, **kwargs)
 
     def load_benchmark(self, dataset):
         """Loads a benchmark for the given semantic segmentation dataset.
 
         This method is used to load pretrained weights for a specific AgML dataset.
         In essence, it serves as a wrapper for `load_state_dict`, directly getting
```

### Comparing `agml-0.5.0/agml/models/tools.py` & `agml-0.5.1/agml/models/tools.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/synthetic/__init__.py` & `agml-0.5.1/agml/synthetic/__init__.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/synthetic/compilation.py` & `agml-0.5.1/agml/synthetic/compilation.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/synthetic/config.py` & `agml-0.5.1/agml/synthetic/config.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/synthetic/converter.py` & `agml-0.5.1/agml/synthetic/converter.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/synthetic/generator.py` & `agml-0.5.1/agml/synthetic/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,15 +151,15 @@
 
         # Generate the ground parameters.
         ground_params = self._load_ground_parameters()
         parameters['Ground'] = ground_params
 
         # The `scan` tag is used for LiDAR generation. This must be added later
         # because there can be multiple origins and thus multiple `scan` tags.
-        if self._generation_options.simulation_type == SimulationType.LiDAR:
+        if self._generation_options.simulation_type == SimulationType.LiDAR or self._generation_options.simulation_type == SimulationType.Both:
             scan_tags = []
             if isinstance(parameters['lidar']['origin'][0], list):
                 for origin in parameters['lidar']['origin']:
                     scan_tag = parameters['lidar']
                     scan_tag['origin'] = origin
                     scan_tags.append(scan_tag)
             else:
@@ -169,23 +169,23 @@
         self._convert_dict_params_to_string(parameters)
 
         # Create a fresh dictionary and put all of the parameters in it.
         canopy_parameters = {
             self._canopy + "Parameters": parameters['canopy'],
             'Ground': parameters['Ground']}
         xml_params = {'canopygenerator': canopy_parameters}
-        if self._generation_options.simulation_type == SimulationType.RGB:
+        if self._generation_options.simulation_type == SimulationType.RGB or self._generation_options.simulation_type == SimulationType.Both:
             xml_params[''] = parameters['camera']
 
         # Convert all of the parameters to XML format.
         tree = ET.parse(io.StringIO(dict2xml({'helios': xml_params})))
         root = tree.getroot()
 
         # Add the `scan` tags if necessary for LiDAR generation.
-        if self._generation_options.simulation_type == SimulationType.LiDAR:
+        if self._generation_options.simulation_type == SimulationType.LiDAR or self._generation_options.simulation_type == SimulationType.Both:
             for scan_tag in scan_tags: # noqa
                 scan_tag_contents = ET.parse(
                     io.StringIO(dict2xml({'scan': scan_tag}))).getroot()
                 ET.indent(scan_tag_contents)
                 root.append(scan_tag_contents)
 
         # Update the camera tags.
```

### Comparing `agml-0.5.0/agml/synthetic/lidar_loader.py` & `agml-0.5.1/agml/synthetic/lidar_loader.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/synthetic/manual.py` & `agml-0.5.1/agml/synthetic/manual.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/synthetic/options.py` & `agml-0.5.1/agml/synthetic/options.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     none: str = "none"
 
 
 class SimulationType(Enum):
     """The simulation render (RGB vs. LiDAR) that is generated."""
     RGB: str = "rgb"
     LiDAR: str = "lidar"
+    Both: str = "rgb lidar"
 
 
 NumberOrMaybeList = TypeVar('NumberOrMaybeList', Number, List[Number])
 
 
 @dataclass(repr = False)
 class Parameters:
```

### Comparing `agml-0.5.0/agml/synthetic/synthetic_data_generation/CMakeLists.txt` & `agml-0.5.1/agml/synthetic/synthetic_data_generation/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/synthetic/synthetic_data_generation/generate.cpp` & `agml-0.5.1/agml/synthetic/synthetic_data_generation/generate.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 using namespace helios;
 
 
 struct SyntheticAnnotationConfig {
 public:
     int num_images;
     vector<string> annotation_type;
-    string simulation_type;
+    vector<string> simulation_type;
     vector<string> labels;
     string xml_path;
     string output_path;
     void load_config(const char* path);
 };
 
 
@@ -49,15 +49,22 @@
             vector<string> annotation_types;
             while ((pos = line.find(' ')) != string::npos) {
                 this -> annotation_type.push_back(line.substr(0, pos));
                 line.erase(0, pos + delimeter.length());
             }
             this->annotation_type.push_back(line);
         } else if (i == 2) {
-            this->simulation_type = line;
+            string delimeter = " "; size_t pos;
+            vector<string> simulation_type;
+            while ((pos = line.find(' ')) != string::npos)
+            {
+                this -> simulation_type.push_back(line.substr(0,pos));
+                line.erase(0, pos + delimeter.length());
+            }
+            this->simulation_type.push_back(line);
         } else if (i == 3) {
             string delimeter = " "; size_t pos;
             vector<string> labels;
             while ((pos = line.find(' ')) != string::npos) {
                 labels.push_back(line.substr(0, pos));
                 line.erase(0, pos + delimeter.length());
             }
@@ -146,15 +153,15 @@
         CanopyGenerator cgen(&context);
         cgen.loadXML(config.xml_path.c_str());
 
         // Declare the Synthetic Annotation class.
         SyntheticAnnotation annotation(&context);
 
         // Choose either the LiDAR or RGB image simulation.
-        if (config.simulation_type == "lidar") {
+        if (!config.simulation_type.empty() && config.simulation_type[1] == "lidar") {
             // Get the UUID of all the elements on the scene
             vector<uint> UUID_trunk = cgen.getTrunkUUIDs();
             vector<uint> UUID_shoot = cgen.getBranchUUIDs();
             vector<uint> UUID_leaf = cgen.getLeafUUIDs();
             vector<uint> UUID_fruit = cgen.getFruitUUIDs();
             vector<uint> UUID_ground = cgen.getGroundUUIDs();
 
@@ -186,15 +193,17 @@
             // Export point cloud data.
             string this_image_dir = config.output_path + "/" + string("image" + to_string(i));
             system(("mkdir -p " + this_image_dir).c_str());
             std::this_thread::sleep_for(std::chrono::milliseconds(100)); // wait until folder is made
             string cloud_export = this_image_dir + "/" + string("point_cloud_" + to_string(i) + ".xyz");
             std::cout << "Writing LiDAR Point cloud to " << cloud_export << " " << std::endl;
             lidarcloud.exportPointCloud(cloud_export.c_str());
-        } else {
+        }
+        if (!config.simulation_type.empty() && config.simulation_type[0] == "rgb")
+        {
             if (!config.annotation_type.empty() && config.annotation_type[0] != "none") {
                 // Set the annotation type based on the configuration.
                 vector<string> va = config.annotation_type;
                 if (!contains(va, "semantic_segmentation")) {
                     annotation.disableSemanticSegmentation();
                 }
                 if (!contains(va, "object_detection")) {
@@ -203,15 +212,15 @@
                 if (!contains(va, "instance_segmentation")) {
                     annotation.disableInstanceSegmentation();
                 }
 
                 // Add labels according to whatever scheme we want.
                 vector<string> vl = config.labels;
                 for (int p = 0; p < cgen.getPlantCount(); p++) { // loop over vines
-                    if (config.simulation_type == "rgb") {
+                    if (!config.simulation_type.empty() && config.simulation_type[0] == "rgb") {
                         if (contains(vl, "trunks")) {
                             annotation.labelPrimitives(cgen.getTrunkUUIDs(p), "trunks");
                         }
                         if (contains(vl, "branches")) {
                             annotation.labelPrimitives(cgen.getBranchUUIDs(p), "branches");
                         }
                         if (contains(vl, "leaves")) {
```

### Comparing `agml-0.5.0/agml/synthetic/tools.py` & `agml-0.5.1/agml/synthetic/tools.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/utils/__init__.py` & `agml-0.5.1/agml/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/utils/data.py` & `agml-0.5.1/agml/utils/data.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/utils/downloads.py` & `agml-0.5.1/agml/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/utils/general.py` & `agml-0.5.1/agml/utils/general.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/utils/image.py` & `agml-0.5.1/agml/utils/image.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/utils/io.py` & `agml-0.5.1/agml/utils/io.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/utils/logging.py` & `agml-0.5.1/agml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/utils/random.py` & `agml-0.5.1/agml/utils/random.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/viz/__init__.py` & `agml-0.5.1/agml/viz/__init__.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/viz/boxes.py` & `agml-0.5.1/agml/viz/boxes.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,14 +106,16 @@
             except KeyError:
                 raise ValueError(
                     "Unexpected COCO JSON format found in input `bboxes` "
                     "dictionary, got {list(bboxes.keys())} but expected "
                     "either `bbox` or `bboxes` for bounding boxes.")
     if bbox_format is not None:
         bboxes = convert_bbox_format(bboxes, bbox_format)
+    if labels is None:
+        labels = [0] * len(bboxes)
 
     # Run a few final checks in order to ensure data is formatted properly.
     image = format_image(image, mask = False)
     if not inplace:
         image = image.copy()
     bboxes = weak_squeeze(bboxes, ndims = 2)
     labels = weak_squeeze(labels, ndims = 1)
```

### Comparing `agml-0.5.0/agml/viz/display.py` & `agml-0.5.1/agml/viz/display.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/viz/general.py` & `agml-0.5.1/agml/viz/general.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/viz/inspection.py` & `agml-0.5.1/agml/viz/inspection.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/viz/labels.py` & `agml-0.5.1/agml/viz/labels.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/viz/masks.py` & `agml-0.5.1/agml/viz/masks.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/viz/point_clouds.py` & `agml-0.5.1/agml/viz/point_clouds.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml/viz/tools.py` & `agml-0.5.1/agml/viz/tools.py`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/agml.egg-info/PKG-INFO` & `agml-0.5.1/agml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agml
-Version: 0.5.0
+Version: 0.5.1
 Summary: A comprehensive library for agricultural deep learning
 Home-page: https://github.com/plant-ai-biophysics-lab/AgML
 Author: UC Davis Plant AI and Biophysics Lab
 Author-email: jmearles@ucdavis.edu
 Maintainer: Amogh Joshi
 Maintainer-email: amnjoshi@ucdavis.edu
 License: UNKNOWN
@@ -161,14 +161,15 @@
 [white_grapes_and_leaves_segmentation](https://github.com/Project-AgML/AgML/blob/main/docs/datasets/white_grapes_and_leaves_segmentation.md) | Semantic Segmentation | 273 | 
 [ghai_romaine_detection](https://github.com/Project-AgML/AgML/blob/main/docs/datasets/ghai_romaine_detection.md) | Object Detection | 500 |
 [ghai_green_cabbage_detection](https://github.com/Project-AgML/AgML/blob/main/docs/datasets/ghai_green_cabbage_detection.md) | Object Detection | 500 |
 [ghai_iceberg_lettuce_detection](https://github.com/Project-AgML/AgML/blob/main/docs/datasets/ghai_iceberg_lettuce_detection.md) | Object Detection | 500 |
 [riseholme_strawberry_classification_2021](https://github.com/Project-AgML/AgML/blob/main/docs/datasets/riseholme_strawberry_classification_2021.md) | Image Classification | 3520 |
 [ghai_broccoli_detection](https://github.com/Project-AgML/AgML/blob/main/docs/datasets/ghai_broccoli_detection.md) | Object Detection | 500 |
 [bean_synthetic_earlygrowth_aerial](https://github.com/Project-AgML/AgML/blob/main/docs/datasets/bean_synthetic_earlygrowth_aerial.md) | Semantic Segmentation | 2500 |
+[ghai_strawberry_fruit_detection](https://github.com/Project-AgML/AgML/blob/main/docs/datasets/ghai_strawberry_fruit_detection.md) | Object Detection | 500 |
 
 ## Usage Information
 
 ### Using Public Agricultural Data
 
 AgML aims to provide easy access to a range of existing public agricultural datasets The core of AgML's public data pipeline is 
 [`AgMLDataLoader`](/agml/data/loader.py). You can use the `AgMLDataLoader` or `agml.data.download_public_dataset()` to download 
@@ -191,9 +192,9 @@
 ## Contributions
 
 We welcome contributions! If you would like to contribute a new feature, fix an issue that you've noticed, or even just mention
 a bug or feature that you would like to see implemented, please don't hesitate to use the *Issues* tab to bring it to our attention.
 See the [contributing guidelines](/CONTRIBUTING.md) for more information.
 
 ## Funding
-This project is partly funded by the [National AI Institute for Food Systems (AIFS)](https://aifs.ucdavis.edu
+This project is partly funded by the [National AI Institute for Food Systems (AIFS)](https://aifs.ucdavis.ed
```

### Comparing `agml-0.5.0/agml.egg-info/SOURCES.txt` & `agml-0.5.1/agml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agml-0.5.0/setup.py` & `agml-0.5.1/setup.py`

 * *Files identical despite different names*

