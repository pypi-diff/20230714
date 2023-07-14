# Comparing `tmp/siibra-0.4a59.tar.gz` & `tmp/siibra-0.4a61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siibra-0.4a59.tar", last modified: Mon Jul  3 11:01:32 2023, max compression
+gzip compressed data, was "siibra-0.4a61.tar", last modified: Fri Jul 14 11:18:58 2023, max compression
```

## Comparing `siibra-0.4a59.tar` & `siibra-0.4a61.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:01:32.949725 siibra-0.4a59/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 11:00:14.000000 siibra-0.4a59/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-03 11:00:14.000000 siibra-0.4a59/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-07-03 11:01:32.949725 siibra-0.4a59/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-07-03 11:00:14.000000 siibra-0.4a59/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 11:01:32.949725 siibra-0.4a59/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-03 11:00:14.000000 siibra-0.4a59/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:01:32.937725 siibra-0.4a59/siibra/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25127 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/commons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:01:32.941725 siibra-0.4a59/siibra/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/configuration/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    19110 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/configuration/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:01:32.941725 siibra-0.4a59/siibra/core/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/core/atlas.py
--rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/core/concept.py
--rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/core/parcellation.py
--rw-r--r--   0 runner    (1001) docker     (123)    24623 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/core/region.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/core/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:01:32.941725 siibra-0.4a59/siibra/features/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16109 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/anchor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:01:32.941725 siibra-0.4a59/siibra/features/connectivity/
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/connectivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/connectivity/functional_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/connectivity/regional_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/connectivity/streamline_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/connectivity/streamline_lengths.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/connectivity/tracer_connectivity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:01:32.941725 siibra-0.4a59/siibra/features/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/dataset/ebrains.py
--rw-r--r--   0 runner    (1001) docker     (123)    16210 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:01:32.941725 siibra-0.4a59/siibra/features/image/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/image/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/image/sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/image/volume_of_interest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:01:32.945725 siibra-0.4a59/siibra/features/tabular/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/tabular/bigbrain_intensity_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/tabular/cell_density_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/tabular/cortical_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/tabular/gene_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/tabular/layerwise_bigbrain_intensities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/tabular/layerwise_cell_density.py
--rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/tabular/receptor_density_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/tabular/receptor_density_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/tabular/regional_timeseries_activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/features/tabular/tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:01:32.945725 siibra-0.4a59/siibra/livequeries/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/livequeries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/livequeries/allen.py
--rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/livequeries/bigbrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/livequeries/ebrains.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/livequeries/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:01:32.945725 siibra-0.4a59/siibra/locations/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/locations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16822 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/locations/boundingbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/locations/location.py
--rw-r--r--   0 runner    (1001) docker     (123)    12586 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/locations/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/locations/pointset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:01:32.945725 siibra-0.4a59/siibra/retrieval/
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/retrieval/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/retrieval/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:01:32.945725 siibra-0.4a59/siibra/retrieval/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/retrieval/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26557 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/retrieval/repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)    20780 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/retrieval/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:01:32.949725 siibra-0.4a59/siibra/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/vocabularies/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)  1647972 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/vocabularies/gene_names.json
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/vocabularies/receptor_symbols.json
--rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/vocabularies/region_aliases.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:01:32.949725 siibra-0.4a59/siibra/volumes/
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/volumes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/volumes/gifti.py
--rw-r--r--   0 runner    (1001) docker     (123)    24048 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/volumes/neuroglancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/volumes/nifti.py
--rw-r--r--   0 runner    (1001) docker     (123)    43140 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/volumes/parcellationmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    21681 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/volumes/sparsemap.py
--rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-07-03 11:00:14.000000 siibra-0.4a59/siibra/volumes/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:01:32.941725 siibra-0.4a59/siibra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-07-03 11:01:32.000000 siibra-0.4a59/siibra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-07-03 11:01:32.000000 siibra-0.4a59/siibra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 11:01:32.000000 siibra-0.4a59/siibra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-03 11:01:32.000000 siibra-0.4a59/siibra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 11:01:32.000000 siibra-0.4a59/siibra.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:01:32.949725 siibra-0.4a59/test/
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-03 11:00:14.000000 siibra-0.4a59/test/test_siibra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:18:58.920182 siibra-0.4a61/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-14 11:17:30.000000 siibra-0.4a61/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-14 11:17:30.000000 siibra-0.4a61/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-07-14 11:18:58.916182 siibra-0.4a61/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-07-14 11:17:30.000000 siibra-0.4a61/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 11:18:58.920182 siibra-0.4a61/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-14 11:17:30.000000 siibra-0.4a61/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:18:58.904182 siibra-0.4a61/siibra/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25127 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/commons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:18:58.908182 siibra-0.4a61/siibra/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/configuration/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19112 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/configuration/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:18:58.908182 siibra-0.4a61/siibra/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/core/atlas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/core/concept.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/core/parcellation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24623 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/core/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/core/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:18:58.908182 siibra-0.4a61/siibra/features/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16109 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/features/anchor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:18:58.908182 siibra-0.4a61/siibra/features/connectivity/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/features/connectivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/features/connectivity/functional_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/features/connectivity/regional_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/features/connectivity/streamline_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/features/connectivity/streamline_lengths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/features/connectivity/tracing_connectivity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:18:58.908182 siibra-0.4a61/siibra/features/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/features/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/features/dataset/ebrains.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16210 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/features/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:18:58.912182 siibra-0.4a61/siibra/features/image/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/features/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/features/image/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/features/image/sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/features/image/volume_of_interest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:18:58.912182 siibra-0.4a61/siibra/features/tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/features/tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/features/tabular/bigbrain_intensity_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/features/tabular/cell_density_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/features/tabular/cortical_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/features/tabular/gene_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/features/tabular/layerwise_bigbrain_intensities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/features/tabular/layerwise_cell_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/features/tabular/receptor_density_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/features/tabular/receptor_density_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/features/tabular/regional_timeseries_activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/features/tabular/tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:18:58.912182 siibra-0.4a61/siibra/livequeries/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/livequeries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/livequeries/allen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/livequeries/bigbrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/livequeries/ebrains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/livequeries/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:18:58.912182 siibra-0.4a61/siibra/locations/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/locations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16822 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/locations/boundingbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/locations/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12586 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/locations/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/locations/pointset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:18:58.912182 siibra-0.4a61/siibra/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/retrieval/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/retrieval/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:18:58.916182 siibra-0.4a61/siibra/retrieval/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/retrieval/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26557 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/retrieval/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21377 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/retrieval/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:18:58.916182 siibra-0.4a61/siibra/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/vocabularies/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1647972 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/vocabularies/gene_names.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/vocabularies/receptor_symbols.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/vocabularies/region_aliases.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:18:58.916182 siibra-0.4a61/siibra/volumes/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/volumes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/volumes/gifti.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24048 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/volumes/neuroglancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/volumes/nifti.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43140 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/volumes/parcellationmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21682 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/volumes/sparsemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-07-14 11:17:30.000000 siibra-0.4a61/siibra/volumes/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:18:58.908182 siibra-0.4a61/siibra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-07-14 11:18:58.000000 siibra-0.4a61/siibra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-14 11:18:58.000000 siibra-0.4a61/siibra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 11:18:58.000000 siibra-0.4a61/siibra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-14 11:18:58.000000 siibra-0.4a61/siibra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 11:18:58.000000 siibra-0.4a61/siibra.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:18:58.916182 siibra-0.4a61/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-14 11:17:30.000000 siibra-0.4a61/test/test_siibra.py
```

### Comparing `siibra-0.4a59/LICENSE` & `siibra-0.4a61/LICENSE`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/PKG-INFO` & `siibra-0.4a61/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siibra
-Version: 0.4a59
+Version: 0.4a61
 Summary: siibra - Software interfaces for interacting with brain atlases
 Home-page: https://github.com/FZJ-INM1-BDA/siibra-python
 Author: Big Data Analytics Group, Forschungszentrum Juelich, Institute of Neuroscience and Medicine (INM-1)
 Author-email: inm1-bda@fz-juelich.de
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `siibra-0.4a59/README.rst` & `siibra-0.4a61/README.rst`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/setup.py` & `siibra-0.4a61/setup.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/__init__.py` & `siibra-0.4a61/siibra/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/commons.py` & `siibra-0.4a61/siibra/commons.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/configuration/__init__.py` & `siibra-0.4a61/siibra/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/configuration/configuration.py` & `siibra-0.4a61/siibra/configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/configuration/factory.py` & `siibra-0.4a61/siibra/configuration/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -439,16 +439,16 @@
             return connectivity.StreamlineLengths(**kwargs)
         elif modality == "Functional":
             kwargs["paradigm"] = spec.get("paradigm")
             return connectivity.FunctionalConnectivity(**kwargs)
         elif modality == "RestingState":
             kwargs["paradigm"] = spec.get("paradigm", "RestingState")
             return connectivity.FunctionalConnectivity(**kwargs)
-        elif modality == "Tracer":
-            return connectivity.TracerConnectivity(**kwargs)
+        elif modality == "Tracing":
+            return connectivity.TracingConnectivity(**kwargs)
         else:
             raise ValueError(f"No method for building connectivity matrix of type {modality}.")
 
     @classmethod
     def build_activity_timeseries(cls, spec):
         modality = spec["modality"]
         kwargs = {
```

### Comparing `siibra-0.4a59/siibra/core/__init__.py` & `siibra-0.4a61/siibra/core/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/core/atlas.py` & `siibra-0.4a61/siibra/core/atlas.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/core/concept.py` & `siibra-0.4a61/siibra/core/concept.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/core/parcellation.py` & `siibra-0.4a61/siibra/core/parcellation.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/core/region.py` & `siibra-0.4a61/siibra/core/region.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/core/space.py` & `siibra-0.4a61/siibra/core/space.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/features/__init__.py` & `siibra-0.4a61/siibra/features/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/features/anchor.py` & `siibra-0.4a61/siibra/features/anchor.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/features/connectivity/__init__.py` & `siibra-0.4a61/siibra/features/connectivity/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .functional_connectivity import FunctionalConnectivity
 from .streamline_counts import StreamlineCounts
 from .streamline_lengths import StreamlineLengths
-from .tracer_connectivity import TracerConnectivity
+from .tracing_connectivity import TracingConnectivity
 
 
 def __dir__():
     return [
         "FunctionalConnectivity",
         "StreamlineCounts",
         "StreamlineLengths",
-        "TracerConnectivity"
+        "TracingConnectivity"
     ]
```

### Comparing `siibra-0.4a59/siibra/features/connectivity/functional_connectivity.py` & `siibra-0.4a61/siibra/features/connectivity/functional_connectivity.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/features/connectivity/regional_connectivity.py` & `siibra-0.4a61/siibra/features/connectivity/regional_connectivity.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/features/connectivity/streamline_counts.py` & `siibra-0.4a61/siibra/features/connectivity/streamline_counts.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/features/connectivity/streamline_lengths.py` & `siibra-0.4a61/siibra/features/connectivity/streamline_lengths.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/features/connectivity/tracer_connectivity.py` & `siibra-0.4a61/siibra/features/connectivity/tracing_connectivity.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from . import regional_connectivity
 
 
-class TracerConnectivity(
+class TracingConnectivity(
     regional_connectivity.RegionalConnectivity,
-    configuration_folder="features/connectivity/regional/tracer",
+    configuration_folder="features/connectivity/regional/tracing",
     category="connectivity"
 ):
     """
     Connectivity matrix obtained in a semi-quantitative manner and grouped by a
     parcellation.
     """
```

### Comparing `siibra-0.4a59/siibra/features/dataset/__init__.py` & `siibra-0.4a61/siibra/features/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/features/dataset/ebrains.py` & `siibra-0.4a61/siibra/features/dataset/ebrains.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/features/feature.py` & `siibra-0.4a61/siibra/features/feature.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/features/image/__init__.py` & `siibra-0.4a61/siibra/features/image/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/features/image/image.py` & `siibra-0.4a61/siibra/features/image/image.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/features/image/sections.py` & `siibra-0.4a61/siibra/features/image/sections.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/features/image/volume_of_interest.py` & `siibra-0.4a61/siibra/features/image/volume_of_interest.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/features/tabular/__init__.py` & `siibra-0.4a61/siibra/features/tabular/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/features/tabular/bigbrain_intensity_profile.py` & `siibra-0.4a61/siibra/features/tabular/bigbrain_intensity_profile.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/features/tabular/cell_density_profile.py` & `siibra-0.4a61/siibra/features/tabular/cell_density_profile.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/features/tabular/cortical_profile.py` & `siibra-0.4a61/siibra/features/tabular/cortical_profile.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/features/tabular/gene_expression.py` & `siibra-0.4a61/siibra/features/tabular/gene_expression.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/features/tabular/layerwise_bigbrain_intensities.py` & `siibra-0.4a61/siibra/features/tabular/layerwise_bigbrain_intensities.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/features/tabular/layerwise_cell_density.py` & `siibra-0.4a61/siibra/features/tabular/layerwise_cell_density.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/features/tabular/receptor_density_fingerprint.py` & `siibra-0.4a61/siibra/features/tabular/receptor_density_fingerprint.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/features/tabular/receptor_density_profile.py` & `siibra-0.4a61/siibra/features/tabular/receptor_density_profile.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/features/tabular/regional_timeseries_activity.py` & `siibra-0.4a61/siibra/features/tabular/regional_timeseries_activity.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/features/tabular/tabular.py` & `siibra-0.4a61/siibra/features/tabular/tabular.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/livequeries/__init__.py` & `siibra-0.4a61/siibra/livequeries/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/livequeries/allen.py` & `siibra-0.4a61/siibra/livequeries/allen.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/livequeries/bigbrain.py` & `siibra-0.4a61/siibra/livequeries/bigbrain.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/livequeries/ebrains.py` & `siibra-0.4a61/siibra/livequeries/ebrains.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/livequeries/query.py` & `siibra-0.4a61/siibra/livequeries/query.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/locations/__init__.py` & `siibra-0.4a61/siibra/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/locations/boundingbox.py` & `siibra-0.4a61/siibra/locations/boundingbox.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/locations/location.py` & `siibra-0.4a61/siibra/locations/location.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/locations/point.py` & `siibra-0.4a61/siibra/locations/point.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/locations/pointset.py` & `siibra-0.4a61/siibra/locations/pointset.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/retrieval/__init__.py` & `siibra-0.4a61/siibra/retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/retrieval/cache.py` & `siibra-0.4a61/siibra/retrieval/cache.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/retrieval/datasets.py` & `siibra-0.4a61/siibra/retrieval/datasets.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/retrieval/repositories.py` & `siibra-0.4a61/siibra/retrieval/repositories.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/retrieval/requests.py` & `siibra-0.4a61/siibra/retrieval/requests.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .cache import CACHE
 from .exceptions import EbrainsAuthenticationError
-from ..commons import logger, HBP_AUTH_TOKEN, KEYCLOAK_CLIENT_ID, KEYCLOAK_CLIENT_SECRET, siibra_tqdm, SIIBRA_USE_LOCAL_SNAPSPOT
+from ..commons import (
+    logger,
+    HBP_AUTH_TOKEN,
+    KEYCLOAK_CLIENT_ID,
+    KEYCLOAK_CLIENT_SECRET,
+    siibra_tqdm,
+    SIIBRA_USE_LOCAL_SNAPSPOT,
+)
 from .. import __version__
 
 import json
 from zipfile import ZipFile
 import requests
 import os
 from nibabel import Nifti1Image, GiftiImage, streamlines
@@ -52,30 +59,27 @@
     ".json": lambda b: json.loads(b.decode()),
     ".tck": lambda b: streamlines.load(BytesIO(b)),
     ".csv": lambda b: pd.read_csv(BytesIO(b)),
     ".tsv": lambda b: pd.read_csv(BytesIO(b), delimiter="\t").dropna(axis=0, how="all"),
     ".txt": lambda b: pd.read_csv(BytesIO(b), delimiter=" ", header=None),
     ".zip": lambda b: ZipFile(BytesIO(b)),
     ".png": lambda b: skimage_io.imread(BytesIO(b)),
-    ".npy": lambda b: np.load(BytesIO(b))
+    ".npy": lambda b: np.load(BytesIO(b)),
 }
 
 
 class SiibraHttpRequestError(Exception):
-
     def __init__(self, url: str, status_code: int, msg="Cannot execute http request."):
         self.url = url
         self.status_code = status_code
         self.msg = msg
         Exception.__init__(self)
 
     def __str__(self):
-        return (
-            f"{self.msg}\n\tStatus code: {self.status_code}\n\tUrl: {self.url:76.76}"
-        )
+        return f"{self.msg}\n\tStatus code: {self.status_code}\n\tUrl: {self.url:76.76}"
 
 
 class HttpRequest:
     def __init__(
         self,
         url: str,
         func: Callable = None,
@@ -113,22 +117,26 @@
         self.msg_if_not_cached = msg_if_not_cached
         self.refresh = refresh
         self.post = post
 
     @staticmethod
     def find_suitiable_decoder(url: str):
         urlpath = urllib.parse.urlsplit(url).path
-        if urlpath.endswith('.gz'):
+        if urlpath.endswith(".gz"):
             dec = HttpRequest.find_suitiable_decoder(urlpath[:-3])
             return lambda b: dec(gzip.decompress(b))
 
-        suitable_decoders = [dec for sfx, dec in DECODERS.items() if urlpath.endswith(sfx)]
+        suitable_decoders = [
+            dec for sfx, dec in DECODERS.items() if urlpath.endswith(sfx)
+        ]
         if len(suitable_decoders) > 0:
             assert len(suitable_decoders) == 1
             return suitable_decoders[0]
+        else:
+            return None
 
     def _set_decoder_func(self, func):
         self.func = func or self.find_suitiable_decoder(self.url)
 
     @property
     def cached(self):
         return os.path.isfile(self.cachefile)
@@ -142,32 +150,42 @@
         if self.cached and not self.refresh:
             return
 
         # not yet in cache, perform http request.
         if self.msg_if_not_cached is not None:
             logger.debug(self.msg_if_not_cached)
 
-        headers = self.kwargs.get('headers', {})
-        other_kwargs = {key: self.kwargs[key] for key in self.kwargs if key != "headers"}
+        headers = self.kwargs.get("headers", {})
+        other_kwargs = {
+            key: self.kwargs[key] for key in self.kwargs if key != "headers"
+        }
 
         http_method = requests.post if self.post else requests.get
-        r = http_method(self.url, headers={
-            **USER_AGENT_HEADER,
-            **headers,
-        }, **other_kwargs, stream=True)
+        r = http_method(
+            self.url,
+            headers={
+                **USER_AGENT_HEADER,
+                **headers,
+            },
+            **other_kwargs,
+            stream=True,
+        )
 
         if not r.ok:
             raise SiibraHttpRequestError(status_code=r.status_code, url=self.url)
 
-        size_bytes = int(r.headers.get('content-length', 0))
+        size_bytes = int(r.headers.get("content-length", 0))
         if size_bytes > min_bytesize_with_no_progress_info:
             progress_bar = siibra_tqdm(
-                total=size_bytes, unit='iB', unit_scale=True,
-                position=0, leave=True,
-                desc=f"Downloading {os.path.split(self.url)[-1]} ({size_bytes / 1024**2:.1f} MiB)"
+                total=size_bytes,
+                unit="iB",
+                unit_scale=True,
+                position=0,
+                leave=True,
+                desc=f"Downloading {os.path.split(self.url)[-1]} ({size_bytes / 1024**2:.1f} MiB)",
             )
         temp_cachefile = f"{self.cachefile}_temp"
         lock = Lock(f"{temp_cachefile}.lock")
 
         with lock:
             with open(temp_cachefile, "wb") as f:
                 for data in r.iter_content(block_size):
@@ -200,18 +218,19 @@
     @property
     def data(self):
         # for backward compatibility with old LazyHttpRequest class
         return self.get()
 
 
 class ZipfileRequest(HttpRequest):
-    def __init__(self, url, filename, func=None):
-        HttpRequest.__init__(self, url, func=func)
+    def __init__(self, url, filename, func=None, refresh=False):
+        HttpRequest.__init__(self, url, refresh=refresh,
+            func=func or self.find_suitiable_decoder(filename)
+        )
         self.filename = filename
-        self._set_decoder_func(self.find_suitiable_decoder(self.filename))
 
     def get(self):
         self._retrieve()
         zipfile = ZipFile(self.cachefile)
         filenames = zipfile.namelist()
         matches = [fn for fn in filenames if fn.endswith(self.filename)]
         if len(matches) == 0:
@@ -255,43 +274,57 @@
         HttpRequest.__init__(self, url, decoder, msg_if_not_cached, post=post)
 
     @classmethod
     def init_oidc(cls):
         resp = requests.get(f"{cls._IAM_ENDPOINT}/.well-known/openid-configuration")
         json_resp = resp.json()
         if "token_endpoint" in json_resp:
-            logger.debug(f"token_endpoint exists in .well-known/openid-configuration. Setting _IAM_TOKEN_ENDPOINT to {json_resp.get('token_endpoint')}")
+            logger.debug(
+                f"token_endpoint exists in .well-known/openid-configuration. Setting _IAM_TOKEN_ENDPOINT to {json_resp.get('token_endpoint')}"
+            )
             cls._IAM_TOKEN_ENDPOINT = json_resp.get("token_endpoint")
         else:
-            logger.warning("expect token endpoint in .well-known/openid-configuration, but was not present")
+            logger.warning(
+                "expect token endpoint in .well-known/openid-configuration, but was not present"
+            )
 
         if "device_authorization_endpoint" in json_resp:
-            logger.debug(f"device_authorization_endpoint exists in .well-known/openid-configuration. setting _IAM_DEVICE_ENDPOINT to {json_resp.get('device_authorization_endpoint')}")
+            logger.debug(
+                f"device_authorization_endpoint exists in .well-known/openid-configuration. setting _IAM_DEVICE_ENDPOINT to {json_resp.get('device_authorization_endpoint')}"
+            )
             cls._IAM_DEVICE_ENDPOINT = json_resp.get("device_authorization_endpoint")
         else:
-            logger.warning("expected device_authorization_endpoint in .well-known/openid-configuration, but was not present")
+            logger.warning(
+                "expected device_authorization_endpoint in .well-known/openid-configuration, but was not present"
+            )
 
     @classmethod
     def fetch_token(cls, **kwargs):
         """
         Fetch an EBRAINS token using commandline-supplied username/password
         using the data proxy endpoint.
 
 
         :ref:`Details on how to access EBRAINS are here.<accessEBRAINS>`
         """
         cls.device_flow(**kwargs)
 
     @classmethod
     def device_flow(cls, **kwargs):
-        if all([
-            not sys.__stdout__.isatty(),  # if is tty, do not raise
-            not any(k in ['JPY_INTERRUPT_EVENT', "JPY_PARENT_PID"] for k in os.environ),  # if is notebook environment, do not raise
-            not os.getenv("SIIBRA_ENABLE_DEVICE_FLOW"),  # if explicitly enabled by env var, do not raise
-        ]):
+        if all(
+            [
+                not sys.__stdout__.isatty(),  # if is tty, do not raise
+                not any(
+                    k in ["JPY_INTERRUPT_EVENT", "JPY_PARENT_PID"] for k in os.environ
+                ),  # if is notebook environment, do not raise
+                not os.getenv(
+                    "SIIBRA_ENABLE_DEVICE_FLOW"
+                ),  # if explicitly enabled by env var, do not raise
+            ]
+        ):
             raise EbrainsAuthenticationError(
                 "sys.stdout is not tty, SIIBRA_ENABLE_DEVICE_FLOW is not set,"
                 "and not running in a notebook. Are you running in batch mode?"
             )
 
         cls.init_oidc()
 
@@ -302,30 +335,25 @@
             if not isinstance(scopes, list):
                 logger.warning("scopes needs to be a list, is but is not... skipping")
                 return None
             if not all(isinstance(scope, str) for scope in scopes):
                 logger.warning("scopes needs to be all str, but is not")
                 return None
             if len(scopes) == 0:
-                logger.warning('provided empty list as scopes... skipping')
+                logger.warning("provided empty list as scopes... skipping")
                 return None
             return "+".join(scopes)
 
         scopes = get_scopes()
 
-        data = {
-            'client_id': cls._IAM_DEVICE_FLOW_CLIENTID
-        }
+        data = {"client_id": cls._IAM_DEVICE_FLOW_CLIENTID}
 
         if scopes:
-            data['scopes'] = scopes
-        resp = requests.post(
-            url=cls._IAM_DEVICE_ENDPOINT,
-            data=data
-        )
+            data["scopes"] = scopes
+        resp = requests.post(url=cls._IAM_DEVICE_ENDPOINT, data=data)
         resp.raise_for_status()
         resp_json = resp.json()
         logger.debug("device flow, request full json:", resp_json)
 
         assert "verification_uri_complete" in resp_json
         assert "device_code" in resp_json
 
@@ -340,25 +368,27 @@
         while True:
             # TODO the polling is a little busted at the moment.
             # need to speak to axel to shorten the polling duration
             sleep(sleep_timer)
 
             logger.debug("Calling endpoint")
             if attempt_number > cls._IAM_DEVICE_MAXTRIES:
-                message = f"exceeded max attempts: {cls._IAM_DEVICE_MAXTRIES}, aborting..."
+                message = (
+                    f"exceeded max attempts: {cls._IAM_DEVICE_MAXTRIES}, aborting..."
+                )
                 logger.error(message)
                 raise EbrainsAuthenticationError(message)
             attempt_number += 1
             resp = requests.post(
                 url=cls._IAM_TOKEN_ENDPOINT,
                 data={
-                    'grant_type': "urn:ietf:params:oauth:grant-type:device_code",
-                    'client_id': cls._IAM_DEVICE_FLOW_CLIENTID,
-                    'device_code': device_code
-                }
+                    "grant_type": "urn:ietf:params:oauth:grant-type:device_code",
+                    "client_id": cls._IAM_DEVICE_FLOW_CLIENTID,
+                    "device_code": device_code,
+                },
             )
 
             if resp.status_code == 200:
                 json_resp = resp.json()
                 logger.debug("Device flow sucessful:", json_resp)
                 cls._KG_API_TOKEN = json_resp.get("access_token")
                 print("ebrains token successfuly set.")
@@ -377,15 +407,14 @@
     @classmethod
     def set_token(cls, token):
         logger.info(f"Setting EBRAINS Knowledge Graph authentication token: {token}")
         cls._KG_API_TOKEN = token
 
     @property
     def kg_token(self):
-
         # token is available, return it
         if self.__class__._KG_API_TOKEN is not None:
             return self.__class__._KG_API_TOKEN
 
         # See if a token is directly provided in  $HBP_AUTH_TOKEN
         if HBP_AUTH_TOKEN:
             self.__class__._KG_API_TOKEN = HBP_AUTH_TOKEN
@@ -444,89 +473,103 @@
         self.kwargs = {"headers": self.auth_headers, "params": self.params}
         return super().get()
 
 
 def try_all_connectors():
     def outer(fn):
         @wraps(fn)
-        def inner(self: 'GitlabProxyEnum', *args, **kwargs):
+        def inner(self: "GitlabProxyEnum", *args, **kwargs):
             exceptions = []
             for connector in self.connectors:
                 try:
                     return fn(self, *args, connector=connector, **kwargs)
                 except Exception as e:
                     exceptions.append(e)
             else:
                 for exc in exceptions:
                     logger.error(exc)
                 raise Exception("try_all_connectors failed")
+
         return inner
+
     return outer
 
 
 class GitlabProxyEnum(Enum):
     DATASET_V1 = "DATASET_V1"
     PARCELLATIONREGION_V1 = "PARCELLATIONREGION_V1"
     DATASET_V3 = "DATASET_V3"
     DATASETVERSION_V3 = "DATASETVERSION_V3"
 
     @property
-    def connectors(self) -> List['GitlabConnector']:
+    def connectors(self) -> List["GitlabConnector"]:
         servers = [
             ("https://jugit.fz-juelich.de", 7846),
             ("https://gitlab.ebrains.eu", 421),
         ]
         from .repositories import GitlabConnector, LocalFileRepository
+
         if SIIBRA_USE_LOCAL_SNAPSPOT:
             logger.info(f"Using localsnapshot at {SIIBRA_USE_LOCAL_SNAPSPOT}")
             return [LocalFileRepository(SIIBRA_USE_LOCAL_SNAPSPOT)]
-        return [GitlabConnector(server[0], server[1], "master", archive_mode=True) for server in servers]
+        return [
+            GitlabConnector(server[0], server[1], "master", archive_mode=True)
+            for server in servers
+        ]
 
     @try_all_connectors()
-    def search_files(self, folder: str, suffix=None, recursive=True, *, connector: 'GitlabConnector' = None) -> List[str]:
+    def search_files(
+        self,
+        folder: str,
+        suffix=None,
+        recursive=True,
+        *,
+        connector: "GitlabConnector" = None,
+    ) -> List[str]:
         assert connector
         return connector.search_files(folder, suffix=suffix, recursive=recursive)
 
     @try_all_connectors()
-    def get(self, filename, decode_func=None, *, connector: 'GitlabConnector' = None):
+    def get(self, filename, decode_func=None, *, connector: "GitlabConnector" = None):
         assert connector
         return connector.get(filename, "", decode_func)
 
 
 class GitlabProxy(HttpRequest):
-
     folder_dict = {
         GitlabProxyEnum.DATASET_V1: "ebrainsquery/v1/dataset",
         GitlabProxyEnum.DATASET_V3: "ebrainsquery/v3/Dataset",
         GitlabProxyEnum.DATASETVERSION_V3: "ebrainsquery/v3/DatasetVersion",
         GitlabProxyEnum.PARCELLATIONREGION_V1: "ebrainsquery/v1/parcellationregions",
     }
 
     def __init__(
         self,
         flavour: GitlabProxyEnum,
         instance_id=None,
-        postprocess: Callable[['GitlabProxy', Any], Any] = (
+        postprocess: Callable[["GitlabProxy", Any], Any] = (
             lambda proxy, obj: obj
             if hasattr(proxy, "instance_id") and proxy.instance_id
             else {"results": obj}
-        )
+        ),
     ):
         if flavour not in GitlabProxyEnum:
             raise RuntimeError("Can only proxy enum members")
 
         self.flavour = flavour
         self.folder = self.folder_dict[flavour]
         self.postprocess = postprocess
         self.instance_id = instance_id
         self._cached_files = None
 
     def get(self):
         if self.instance_id:
-            return self.postprocess(self, self.flavour.get(f"{self.folder}/{self.instance_id}.json"))
+            return self.postprocess(
+                self, self.flavour.get(f"{self.folder}/{self.instance_id}.json")
+            )
         return self.postprocess(self, self.flavour.get(f"{self.folder}/_all.json"))
 
 
 class MultiSourceRequestException(Exception):
     pass
 
 
@@ -540,12 +583,14 @@
         exceptions = []
         for req in self.requests:
             try:
                 return req.get()
             except Exception as e:
                 exceptions.append(e)
         else:
-            raise MultiSourceRequestException("All requests failed:\n" + "\n".join(str(exc) for exc in exceptions))
+            raise MultiSourceRequestException(
+                "All requests failed:\n" + "\n".join(str(exc) for exc in exceptions)
+            )
 
     @property
     def data(self):
         return self.get()
```

### Comparing `siibra-0.4a59/siibra/vocabularies/__init__.py` & `siibra-0.4a61/siibra/vocabularies/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/vocabularies/gene_names.json` & `siibra-0.4a61/siibra/vocabularies/gene_names.json`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/vocabularies/receptor_symbols.json` & `siibra-0.4a61/siibra/vocabularies/receptor_symbols.json`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/vocabularies/region_aliases.json` & `siibra-0.4a61/siibra/vocabularies/region_aliases.json`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/volumes/__init__.py` & `siibra-0.4a61/siibra/volumes/__init__.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/volumes/gifti.py` & `siibra-0.4a61/siibra/volumes/gifti.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/volumes/neuroglancer.py` & `siibra-0.4a61/siibra/volumes/neuroglancer.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/volumes/nifti.py` & `siibra-0.4a61/siibra/volumes/nifti.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/volumes/parcellationmap.py` & `siibra-0.4a61/siibra/volumes/parcellationmap.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra/volumes/sparsemap.py` & `siibra-0.4a61/siibra/volumes/sparsemap.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,22 +107,22 @@
         # returns the x, y, and z coordinates of nonzero voxels for the map
         # with the given index, together with their corresponding values v.
         assert volume in range(self.num_volumes)
         x, y, z = [v.squeeze() for v in np.split(self.coords(volume), 3)]
         v = [self.probs[i][volume] for i in self.voxels[x, y, z]]
         return x, y, z, v
 
-    def _to_local_cache(self):
+    def _to_local_cache(self, cache_prefix: str):
         """
         Serialize this index to the cache, using the given prefix for the cache
         filenames.
         """
-        probsfile = cache.CACHE.build_filename(f"{self._cache_prefix}", suffix="probs.txt.gz")
-        bboxfile = cache.CACHE.build_filename(f"{self._cache_prefix}", suffix="bboxes.txt.gz")
-        voxelfile = cache.CACHE.build_filename(f"{self._cache_prefix}", suffix="voxels.nii.gz")
+        probsfile = cache.CACHE.build_filename(f"{cache_prefix}", suffix="probs.txt.gz")
+        bboxfile = cache.CACHE.build_filename(f"{cache_prefix}", suffix="bboxes.txt.gz")
+        voxelfile = cache.CACHE.build_filename(f"{cache_prefix}", suffix="voxels.nii.gz")
         Nifti1Image(self.voxels, self.affine).to_filename(voxelfile)
         with gzip.open(probsfile, 'wt') as f:
             for D in self.probs:
                 f.write("{}\n".format(" ".join(f"{i} {p}" for i, p in D.items())))
         with gzip.open(bboxfile, "wt") as f:
             for bbox in self.bboxes:
                 f.write(
```

### Comparing `siibra-0.4a59/siibra/volumes/volume.py` & `siibra-0.4a61/siibra/volumes/volume.py`

 * *Files identical despite different names*

### Comparing `siibra-0.4a59/siibra.egg-info/PKG-INFO` & `siibra-0.4a61/siibra.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siibra
-Version: 0.4a59
+Version: 0.4a61
 Summary: siibra - Software interfaces for interacting with brain atlases
 Home-page: https://github.com/FZJ-INM1-BDA/siibra-python
 Author: Big Data Analytics Group, Forschungszentrum Juelich, Institute of Neuroscience and Medicine (INM-1)
 Author-email: inm1-bda@fz-juelich.de
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `siibra-0.4a59/siibra.egg-info/SOURCES.txt` & `siibra-0.4a61/siibra.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 siibra/features/anchor.py
 siibra/features/feature.py
 siibra/features/connectivity/__init__.py
 siibra/features/connectivity/functional_connectivity.py
 siibra/features/connectivity/regional_connectivity.py
 siibra/features/connectivity/streamline_counts.py
 siibra/features/connectivity/streamline_lengths.py
-siibra/features/connectivity/tracer_connectivity.py
+siibra/features/connectivity/tracing_connectivity.py
 siibra/features/dataset/__init__.py
 siibra/features/dataset/ebrains.py
 siibra/features/image/__init__.py
 siibra/features/image/image.py
 siibra/features/image/sections.py
 siibra/features/image/volume_of_interest.py
 siibra/features/tabular/__init__.py
```

### Comparing `siibra-0.4a59/test/test_siibra.py` & `siibra-0.4a61/test/test_siibra.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from unittest.mock import patch, MagicMock
 from siibra import _parcellation
 from siibra import get_region
 
 Parcellation = _parcellation.Parcellation
 
+
 def test_get_region():
     class DummyCls:
         def get_region(self):
             raise NotImplementedError
+
     dummy_obj = DummyCls()
     mock_region = DummyCls()
     dummy_obj.get_region = MagicMock(return_value=mock_region)
-    with patch.object(Parcellation, 'get_instance', return_value=dummy_obj) as mock_get_instance:
+    with patch.object(
+        Parcellation, "get_instance", return_value=dummy_obj
+    ) as mock_get_instance:
         actual_got_region = get_region("boo-buz", "foo-bar")
 
         mock_get_instance.assert_called_once_with("boo-buz")
         dummy_obj.get_region.assert_called_once_with("foo-bar")
         assert actual_got_region is mock_region
```

