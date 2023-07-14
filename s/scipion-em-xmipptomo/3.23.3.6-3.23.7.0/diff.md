# Comparing `tmp/scipion-em-xmipptomo-3.23.3.6.tar.gz` & `tmp/scipion-em-xmipptomo-3.23.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-xmipptomo-3.23.3.6.tar", last modified: Tue Apr 25 08:38:29 2023, max compression
+gzip compressed data, was "scipion-em-xmipptomo-3.23.7.0.tar", last modified: Fri Jul 14 07:54:40 2023, max compression
```

## Comparing `scipion-em-xmipptomo-3.23.3.6.tar` & `scipion-em-xmipptomo-3.23.7.0.tar`

### file list

```diff
@@ -1,64 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:29.447014 scipion-em-xmipptomo-3.23.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-25 08:38:29.447014 scipion-em-xmipptomo-3.23.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:29.443014 scipion-em-xmipptomo-3.23.3.6/scipion_em_xmipptomo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-25 08:38:29.000000 scipion-em-xmipptomo-3.23.3.6/scipion_em_xmipptomo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-25 08:38:29.000000 scipion-em-xmipptomo-3.23.3.6/scipion_em_xmipptomo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:38:29.000000 scipion-em-xmipptomo-3.23.3.6/scipion_em_xmipptomo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-25 08:38:29.000000 scipion-em-xmipptomo-3.23.3.6/scipion_em_xmipptomo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-25 08:38:29.000000 scipion-em-xmipptomo-3.23.3.6/scipion_em_xmipptomo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-25 08:38:29.000000 scipion-em-xmipptomo-3.23.3.6/scipion_em_xmipptomo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 08:38:29.447014 scipion-em-xmipptomo-3.23.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:29.443014 scipion-em-xmipptomo-3.23.3.6/xmipptomo/
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/bibtex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:29.447014 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_align_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_applyAlignmentTS.py
--rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_apply_alignment_subtomo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11036 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_cltomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_connected_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_coords_roi.py
--rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_crop_resize_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_crop_tomograms.py
--rw-r--r--   0 runner    (1001) docker     (123)    11300 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_extract_subtomos.py
--rw-r--r--   0 runner    (1001) docker     (123)    11376 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_filter_coordinates_by_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_flexalign.py
--rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_half_maps_subtomos.py
--rw-r--r--   0 runner    (1001) docker     (123)    25953 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_phantom_subtomo.py
--rw-r--r--   0 runner    (1001) docker     (123)    14307 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_phantom_tomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_project_top.py
--rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_resizeTS.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_resize_tomograms.py
--rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_resolution_local_monotomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_roiIJ.py
--rw-r--r--   0 runner    (1001) docker     (123)    12420 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_score_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_score_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     9287 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_splitTS.py
--rw-r--r--   0 runner    (1001) docker     (123)    17366 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_subtomo_map_back.py
--rw-r--r--   0 runner    (1001) docker     (123)    13484 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_subtraction_subtomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:29.447014 scipion-em-xmipptomo-3.23.3.6/xmipptomo/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/tests/test_protocol_extract_subtomos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/tests/test_protocol_monotomo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/tests/test_protocol_phantom_subtomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/tests/test_protocols_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/tests/test_protocols_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)    26723 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/tests/test_protocols_xmipptomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:29.447014 scipion-em-xmipptomo-3.23.3.6/xmipptomo/viewers/
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/viewers/monotomo_tree_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/viewers/viewer_cltomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/viewers/viewer_phantom_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    10075 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/viewers/viewer_resolution_local_monotomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/viewers/viewer_score_subtomos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/wizards.py
--rw-r--r--   0 runner    (1001) docker     (123)    72615 2023-04-25 08:36:19.000000 scipion-em-xmipptomo-3.23.3.6/xmipptomo/xmipp_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:54:40.251429 scipion-em-xmipptomo-3.23.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-14 07:54:40.251429 scipion-em-xmipptomo-3.23.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:54:40.247429 scipion-em-xmipptomo-3.23.7.0/scipion_em_xmipptomo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-14 07:54:40.000000 scipion-em-xmipptomo-3.23.7.0/scipion_em_xmipptomo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-07-14 07:54:40.000000 scipion-em-xmipptomo-3.23.7.0/scipion_em_xmipptomo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 07:54:40.000000 scipion-em-xmipptomo-3.23.7.0/scipion_em_xmipptomo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-14 07:54:40.000000 scipion-em-xmipptomo-3.23.7.0/scipion_em_xmipptomo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-14 07:54:40.000000 scipion-em-xmipptomo-3.23.7.0/scipion_em_xmipptomo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-14 07:54:40.000000 scipion-em-xmipptomo-3.23.7.0/scipion_em_xmipptomo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 07:54:40.251429 scipion-em-xmipptomo-3.23.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:54:40.247429 scipion-em-xmipptomo-3.23.7.0/xmipptomo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:54:40.251429 scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_align_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_applyAlignmentTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_apply_alignment_subtomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11036 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_cltomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_connected_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_coords_roi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_crop_resize_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_crop_tomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19092 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_deep_misalignment_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10647 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_denoising_confidence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_dose_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_extract_particlestacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_extract_subtomos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11376 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_filter_coordinates_by_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_flexalign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_half_maps_subtomos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11482 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_peak_high_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25953 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_phantom_subtomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14307 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_phantom_tomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15885 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_project_subtomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8770 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_project_top.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_reconstruct_tomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_resizeTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_resize_tomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_resolution_local_monotomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_roiIJ.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12420 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_score_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_score_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9288 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_splitTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17371 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_subtomo_map_back.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13484 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_subtraction_subtomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:54:40.251429 scipion-em-xmipptomo-3.23.7.0/xmipptomo/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/tests/test_protocol_extract_subtomos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/tests/test_protocol_monotomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/tests/test_protocol_phantom_subtomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/tests/test_protocol_project_subtomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/tests/test_protocols_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/tests/test_protocols_deep_misalignment_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/tests/test_protocols_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26735 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/tests/test_protocols_xmipptomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:54:40.251429 scipion-em-xmipptomo-3.23.7.0/xmipptomo/viewers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/viewers/monotomo_tree_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/viewers/viewer_cltomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/viewers/viewer_phantom_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10075 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/viewers/viewer_resolution_local_monotomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/viewers/viewer_score_subtomos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/wizards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72615 2023-07-14 07:52:48.000000 scipion-em-xmipptomo-3.23.7.0/xmipptomo/xmipp_logo.png
```

### Comparing `scipion-em-xmipptomo-3.23.3.6/LICENSE` & `scipion-em-xmipptomo-3.23.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.6/PKG-INFO` & `scipion-em-xmipptomo-3.23.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: scipion-em-xmipptomo
-Version: 3.23.3.6
+Version: 3.23.7.0
 Summary: Scipion plugin to deal with xmipp tomography protocols.
 Home-page: https://github.com/i2pc/scipion-em-xmipptomo
 Author: I2PC
 Author-email: scipion@cnb.csic.es
 License: UNKNOWN
 Description: ========================
         Scipion xmipptomo plugin
```

### Comparing `scipion-em-xmipptomo-3.23.3.6/scipion_em_xmipptomo.egg-info/PKG-INFO` & `scipion-em-xmipptomo-3.23.7.0/scipion_em_xmipptomo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: scipion-em-xmipptomo
-Version: 3.23.3.6
+Version: 3.23.7.0
 Summary: Scipion plugin to deal with xmipp tomography protocols.
 Home-page: https://github.com/i2pc/scipion-em-xmipptomo
 Author: I2PC
 Author-email: scipion@cnb.csic.es
 License: UNKNOWN
 Description: ========================
         Scipion xmipptomo plugin
```

### Comparing `scipion-em-xmipptomo-3.23.3.6/scipion_em_xmipptomo.egg-info/SOURCES.txt` & `scipion-em-xmipptomo-3.23.7.0/scipion_em_xmipptomo.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,64 @@
-CHANGES.txt
 LICENSE
 MANIFEST.in
 README.rst
 requirements.txt
 setup.py
 scipion_em_xmipptomo.egg-info/PKG-INFO
 scipion_em_xmipptomo.egg-info/SOURCES.txt
 scipion_em_xmipptomo.egg-info/dependency_links.txt
 scipion_em_xmipptomo.egg-info/entry_points.txt
 scipion_em_xmipptomo.egg-info/requires.txt
 scipion_em_xmipptomo.egg-info/top_level.txt
 xmipptomo/__init__.py
 xmipptomo/bibtex.py
+xmipptomo/objects.py
 xmipptomo/protocols.conf
 xmipptomo/utils.py
 xmipptomo/wizards.py
 xmipptomo/xmipp_logo.png
 xmipptomo/protocols/__init__.py
 xmipptomo/protocols/protocol_align_transform.py
 xmipptomo/protocols/protocol_applyAlignmentTS.py
 xmipptomo/protocols/protocol_apply_alignment_subtomo.py
 xmipptomo/protocols/protocol_cltomo.py
 xmipptomo/protocols/protocol_connected_components.py
 xmipptomo/protocols/protocol_coords_roi.py
 xmipptomo/protocols/protocol_crop_resize_base.py
 xmipptomo/protocols/protocol_crop_tomograms.py
+xmipptomo/protocols/protocol_deep_misalignment_detection.py
+xmipptomo/protocols/protocol_denoising_confidence.py
+xmipptomo/protocols/protocol_dose_filter.py
+xmipptomo/protocols/protocol_extract_particlestacks.py
 xmipptomo/protocols/protocol_extract_subtomos.py
 xmipptomo/protocols/protocol_filter_coordinates_by_map.py
 xmipptomo/protocols/protocol_flexalign.py
 xmipptomo/protocols/protocol_half_maps_subtomos.py
+xmipptomo/protocols/protocol_peak_high_contrast.py
 xmipptomo/protocols/protocol_phantom_subtomo.py
 xmipptomo/protocols/protocol_phantom_tomo.py
+xmipptomo/protocols/protocol_project_subtomograms.py
 xmipptomo/protocols/protocol_project_top.py
+xmipptomo/protocols/protocol_reconstruct_tomograms.py
 xmipptomo/protocols/protocol_resizeTS.py
 xmipptomo/protocols/protocol_resize_tomograms.py
 xmipptomo/protocols/protocol_resolution_local_monotomo.py
 xmipptomo/protocols/protocol_roiIJ.py
 xmipptomo/protocols/protocol_score_coordinates.py
 xmipptomo/protocols/protocol_score_transform.py
 xmipptomo/protocols/protocol_splitTS.py
 xmipptomo/protocols/protocol_subtomo_map_back.py
 xmipptomo/protocols/protocol_subtraction_subtomo.py
 xmipptomo/tests/__init__.py
 xmipptomo/tests/test_protocol_extract_subtomos.py
 xmipptomo/tests/test_protocol_monotomo.py
 xmipptomo/tests/test_protocol_phantom_subtomo.py
+xmipptomo/tests/test_protocol_project_subtomograms.py
 xmipptomo/tests/test_protocols_crop.py
+xmipptomo/tests/test_protocols_deep_misalignment_detection.py
 xmipptomo/tests/test_protocols_resize.py
 xmipptomo/tests/test_protocols_xmipptomo.py
 xmipptomo/viewers/__init__.py
 xmipptomo/viewers/monotomo_tree_provider.py
 xmipptomo/viewers/viewer_cltomo.py
 xmipptomo/viewers/viewer_phantom_create.py
 xmipptomo/viewers/viewer_resolution_local_monotomo.py
```

### Comparing `scipion-em-xmipptomo-3.23.3.6/setup.py` & `scipion-em-xmipptomo-3.23.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/__init__.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 # *
 # **************************************************************************
 import xmipp3
 import subprocess, os
 import pyworkflow.utils as pwutils
 
 _logo = "xmipp_logo.png"
-_references = ['delaRosaTrevin2013']
-__version__ = "3.23.03.6" #X.YY.MM.sv
+_references = ['delaRosaTrevin2013', 'Jimenez2022']
+__version__ = "3.23.07.0" #X.YY.MM.sv
         # X.Y.M = version of the xmipp release associated.
         # sv = Set this to ".0" on each xmipp  release.
         # For not release version (hotfix) increase it --> ".1", ".2", ...
 
 class Plugin(xmipp3.Plugin):
 
     @classmethod
@@ -44,8 +44,8 @@
             "TF_FORCE_GPU_ALLOW_GROWTH": "'true'"
         }, position=pwutils.Environ.BEGIN)
         return environ
 
     @classmethod
     def defineBinaries(cls, env):
 
-        pass
+        pass
```

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/bibtex.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/viewers/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# -*- coding: utf-8 -*-
 # **************************************************************************
 # *
-# * Authors:     Estrella Fernandez Gimenez (me.fernandez@cnb.csic.es)
+# * Authors:     J.M. De la Rosa Trevin (delarosatrevin@scilifelab.se) [1]
 # *
-# *  BCU, Centro Nacional de Biotecnologia, CSIC
+# * [1] SciLifeLab, Stockholm University
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 2 of the License, or
 # * (at your option) any later version.
 # *
 # * This program is distributed in the hope that it will be useful,
@@ -21,23 +20,12 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
-"""
-@article{delaRosaTrevin2013,
-title = "Xmipp 3.0: An improved software suite for image processing in electron microscopy ",
-journal = "JSB",
-volume = "184",
-number = "2",
-pages = "321 - 328",
-year = "2013",
-issn = "1047-8477",
-doi = "http://dx.doi.org/10.1016/j.jsb.2013.09.015",
-url = "http://www.sciencedirect.com/science/article/pii/S1047847713002566",
-author = "de la Rosa-Trevín, J.M.  and Oton, J. and R. Marabini and A. Zaldívar and J. Vargas and J.M. Carazo and Sorzano, C.O.S.",
-keywords = "Electron microscopy, Single particles analysis, Image processing, Software package "
-}
+from .viewer_cltomo import XmippCLTomoViewer, XmippProtTsFlexAlignViewer
+from .viewer_resolution_local_monotomo import XmippMonoTomoViewer
+from .viewer_phantom_create import XmippPhantomSubtomoViewer
+from .viewer_score_subtomos import XmippTomoScoreSubtomoViewer
 
-"""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/__init__.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,40 +21,37 @@
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 # Please keep the alphabetical order
-
 from .protocol_align_transform import XmippProtAlignTransform
 from .protocol_apply_alignment_subtomo import XmippProtApplyTransformSubtomo
 from .protocol_applyAlignmentTS import XmippProtApplyTransformationMatrixTS
 from .protocol_cltomo import XmippProtCLTomo
 from .protocol_connected_components import XmippProtConnectedComponents
 from .protocol_coords_roi import XmippProtCCroi
+from .protocol_deep_misalignment_detection import XmippProtDeepDetectMisalignment
+from .protocol_dose_filter import XmippProtDoseFilter
 from .protocol_filter_coordinates_by_map import XmippProtFilterCoordinatesByMap
 from .protocol_crop_tomograms import XmippProtCropTomograms
+from .protocol_denoising_confidence import XmippProtConfTomo
+from .protocol_extract_particlestacks import XmippProtExtractParticleStacks
 from .protocol_extract_subtomos import XmippProtExtractSubtomos
 from .protocol_flexalign import XmippProtTsFlexAlign
+from .protocol_peak_high_contrast import XmippProtPeakHighContrast
 from .protocol_phantom_subtomo import XmippProtPhantomSubtomo
 from .protocol_phantom_tomo import XmippProtPhantomTomo
 from .protocol_project_top import XmippProtSubtomoProject
+from .protocol_reconstruct_tomograms import XmippProtReconstructTomograms
 from .protocol_resizeTS import XmippProtResizeTiltSeries
 from .protocol_resize_tomograms import XmippProtResizeTomograms
 from .protocol_resolution_local_monotomo import XmippProtMonoTomo
 from .protocol_roiIJ import XmippProtRoiIJ
 from .protocol_score_coordinates import XmippProtScoreCoordinates
 from .protocol_score_transform import XmippProtScoreTransform
 from .protocol_splitTS import XmippProtSplitTiltSeries
 from .protocol_subtraction_subtomo import XmippProtSubtractionSubtomo
 from .protocol_subtomo_map_back import XmippProtSubtomoMapBack
 from .protocol_half_maps_subtomos import XmippProtHalfMapsSubtomo
-
-
-
-
-
-
-
-
-
+from .protocol_project_subtomograms import XmippProtProjectSubtomograms
```

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_align_transform.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_align_transform.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_applyAlignmentTS.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_applyAlignmentTS.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # **************************************************************************
 # *
-# * Authors:     Federico P. de Isidro Gomez (fp.deisidro@cnb.csi.es) [1]
+# * Authors:     Federico P. de Isidro Gomez (fp.deisidro@cnb.csic.es) [1]
 # *
 # * [1] Centro Nacional de Biotecnologia, CSIC, Spain
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 2 of the License, or
 # * (at your option) any later version.
```

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_apply_alignment_subtomo.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_apply_alignment_subtomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_cltomo.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_cltomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_connected_components.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_connected_components.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_coords_roi.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_coords_roi.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_crop_resize_base.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_crop_resize_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,14 @@
 # **************************************************************************
 
 from pwem.protocols import EMProtocol
 from pyworkflow import BETA
 from pyworkflow.protocol.params import EnumParam, FloatParam, IntParam, BooleanParam, PointerParam
 import pyworkflow.protocol.constants as const
 from tomo.protocols import ProtTomoBase
-import os
-from pyworkflow.object import Set
-import tomo.objects as tomoObj
 
 
 class XmippProtResizeBase(EMProtocol, ProtTomoBase):
     """
     Base class to resize 2D and 3D objects in tomography
     """
```

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_crop_tomograms.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_crop_tomograms.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,25 +20,19 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # *********************************************************************
 
-from pwem.protocols import EMProtocol
 from pyworkflow import BETA
-from pyworkflow.protocol.params import EnumParam, FloatParam, IntParam, BooleanParam, PointerParam
-import pyworkflow.protocol.constants as const
-from tomo.protocols import ProtTomoBase
-from tomo.objects import SetOfTomograms, Tomogram
+from pyworkflow.protocol.params import PointerParam
+from tomo.objects import Tomogram
 import os
-import pyworkflow.utils.path as path
 from pyworkflow.object import Set
-import tomo.objects as tomoObj
-from pwem.emlib.image import ImageHandler
 from xmipptomo.protocols.protocol_crop_resize_base import XmippProtCropBase3D
 
 SUFIXCROPPED = '_cropped.mrc'
 
 class XmippProtCropTomograms(XmippProtCropBase3D):
     """
     Protocol to crop tomograms using xmipp_transform_window.
```

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_extract_subtomos.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_extract_subtomos.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # **************************************************************************
 # *
 # * Authors:     J.L. Vilas (jlvilas@cnb.csic.es)
+# *              Federico P. de Isidro Gomez (fp.deisidro@cnb.csic.es)
 # *
 # * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 2 of the License, or
 # * (at your option) any later version.
@@ -23,65 +24,82 @@
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 import os
 import glob
 from pwem.emlib import lib
-from pwem.objects import Particle, Volume, Transform, String, SetOfVolumes, SetOfParticles
+from pwem.objects import Transform
 from pwem.protocols import EMProtocol
 from pwem import ALIGN_PROJ
 import pwem.emlib.metadata as md
 
 from pyworkflow import BETA
 from pyworkflow import utils as pwutils
-from pyworkflow.protocol.params import PointerParam, EnumParam, IntParam, BooleanParam
+from pyworkflow.protocol.params import PointerParam, FloatParam, IntParam, BooleanParam
 
-from tomo.objects import SetOfTomograms, SetOfSubTomograms, SubTomogram, SetOfCoordinates3D, TomoAcquisition, MATRIX_CONVERSION
+from tomo.objects import SetOfTomograms, SetOfSubTomograms, SubTomogram, SetOfCoordinates3D, TomoAcquisition, \
+    MATRIX_CONVERSION
 import tomo.constants as const
 
 from tomo.protocols import ProtTomoBase
 from xmipp3.convert import alignmentToRow
 
-
 COORD_BASE_FN = 'coords'
 
 # Tomogram type constants for particle extraction
 OUTPUTATTRIBUTE = 'Subtomograms'
 
 
 class XmippProtExtractSubtomos(EMProtocol, ProtTomoBase):
     """
     Extract a set of subtomograms from a set of tomograms given a set of coordinates.
     """
     _label = 'extract subtomos'
     _devStatus = BETA
-    _possibleOutputs = {OUTPUTATTRIBUTE:SetOfSubTomograms}
+    _possibleOutputs = {OUTPUTATTRIBUTE: SetOfSubTomograms}
     lines = []
     tomoFiles = []
 
     # --------------------------- DEFINE param functions ------------------------
     def _defineParams(self, form):
         form.addSection(label='Parameters')
 
-        form.addParam('coords', PointerParam, pointerClass=SetOfCoordinates3D,
-                  label='Coordinates', help='3D coordinates to use in the extraction process.'
-                                            'The coordinate denotes the center of the subtomogram')
-
-        form.addParam('tomograms', PointerParam, pointerClass=SetOfTomograms,
+        form.addParam('coords',
+                      PointerParam,
+                      pointerClass=SetOfCoordinates3D,
+                      label='Coordinates',
+                      help='3D coordinates to use in the extraction process.'
+                           'The coordinate denotes the center of the subtomogram')
+
+        form.addParam('tomograms',
+                      PointerParam,
+                      pointerClass=SetOfTomograms,
                       allowsNull=True,
-                      label='Tomograms (Optional)', help='The subtomograms will be extracted from this set.')
+                      label='Tomograms (Optional)',
+                      help='The subtomograms will be extracted from this set.')
 
-        form.addParam('boxSize', IntParam,
+        form.addParam('boxSize',
+                      IntParam,
                       label='Box size',
+                      help='The subtomograms are extracted as a cube. The box size defines the edge of the cube. '
+                           'This is the final size of the boxsize if downsampling is applied. The wizard selects same '
+                           'box size as picking')
+
+        form.addParam('dowsamplingFactor',
+                      FloatParam,
+                      label='Dowsampling factor',
+                      default=1.0,
                       help='The subtomograms are extracted as a cube. The box size defines the edge of the cube'
                            'The wizard selects same box size as picking')
 
-        form.addParam('invertContrast', BooleanParam,
-                      label='Invert Contrast',  default=True,
+        form.addParam('invertContrast',
+                      BooleanParam,
+                      label='Invert Contrast',
+                      default=True,
                       help='Normally, tomograms has the contrast inverted with respect to standard for subtomograms. '
                            'It means, in the tomograms the structure is black and the noise is white. Generally, the'
                            'subtomograms are white with a black background. This means that the subtomograms has the '
                            'contrast inverted with respect to the tomograms. Put this flag as True if the contrast'
                            'need to be inverted.')
 
     # --------------------------- INSERT steps functions ------------------------
@@ -106,15 +124,14 @@
         coordDict = []
 
         for item in self.coords.get().iterCoordinates(volume=tomo):
             coord = item
             transform = Transform(matrix=item.getMatrix(convention=MATRIX_CONVERSION.XMIPP))
 
             if coord.getTomoId() == tsid:
-
                 nRow = md.Row()
                 nRow.setValue(lib.MDL_ITEM_ID, int(coord.getObjId()))
                 coord.setVolume(tomo)
 
                 nRow.setValue(lib.MDL_XCOOR, int(coord.getX(const.BOTTOM_LEFT_CORNER)))
                 nRow.setValue(lib.MDL_YCOOR, int(coord.getY(const.BOTTOM_LEFT_CORNER)))
                 nRow.setValue(lib.MDL_ZCOOR, int(coord.getZ(const.BOTTOM_LEFT_CORNER)))
@@ -135,34 +152,32 @@
     def getTomograms(self):
         """
             Returns the set of tomograms that will be used for extracting the coordinates.
 
             If the unique input is the set of coordinates the output will be their corresponding tomograms
             If a set of tomograms is provided in the form, then the output will be such set of tomograms
         """
-        inTomograms = None
         if self.tomograms.get() is None:
             inTomograms = self.coords.get().getPrecedents()
         else:
             inTomograms = self.tomograms.get()
         return inTomograms
 
-
     def extractStep(self, tsId):
         """
             This function executes xmipp_tomo_extract_subtomos. To do that
             1) It defines the set of tomograms to be used (self.getTomograms)
             2) A folder where the subtomograms will be stored is created. The name of this folder is the tsId
             3) Lanches the xmipp_tomo_extract_subtomos
 
         """
 
         inTomograms = self.getTomograms()
 
-        tomo = inTomograms[{'_tsId':tsId}]
+        tomo = inTomograms[{'_tsId': tsId}]
 
         if tomo is None:
             self.warning('Tomogram not found for tsId %s' % tsId)
             return
 
         # Defining the output folder
         tomoPath = self._getExtraPath(tsId)
@@ -175,32 +190,37 @@
         params = ' --tomogram %s' % tomoFn
         params += ' --coordinates %s' % fnCoords
         params += ' --boxsize %i' % self.boxSize.get()
         if self.invertContrast.get():
             params += ' --invertContrast'
         params += ' --subtomo'
         params += ' --threads %i' % 1
-
-        params += ' -o %s' % tomoPath
+        if self.dowsamplingFactor.get() != 1:
+            params += ' --downsample %f' % self.dowsamplingFactor.get()
+        params += ' -o %s ' % tomoPath
         self.runJob('xmipp_tomo_extract_subtomograms', params)
 
         self.tomoFiles.append(tomoFn)
 
     def createOutputStep(self):
         """
             This function creates the output of the protocol
         """
+
         precedents = self.getTomograms()
         firstItem = precedents.getFirstItem()
         acquisitonInfo = firstItem.getAcquisition()
-        #TODO: Check the sampling if the tomograms are different than the picked ones
-        #TODO: Check the sampling rate if a downsampling option is implemented
+        # TODO: Check the sampling if the tomograms are different than the picked ones
+        # TODO: Check the sampling rate if a downsampling option is implemented
         outputSet = None
+
+        newSamplingRate = precedents.getSamplingRate() * self.dowsamplingFactor.get()
+
         self.outputSubTomogramsSet = self._createSetOfSubTomograms(self._getOutputSuffix(SetOfSubTomograms))
-        self.outputSubTomogramsSet.setSamplingRate(precedents.getSamplingRate())
+        self.outputSubTomogramsSet.setSamplingRate(newSamplingRate)
         self.outputSubTomogramsSet.setCoordinates3D(self.coords)
         if firstItem.getAcquisition():
             acquisition = TomoAcquisition()
             acquisition.setAngleMin(acquisitonInfo.getAngleMin())
             acquisition.setAngleMax(acquisitonInfo.getAngleMax())
             acquisition.setStep(acquisitonInfo.getStep())
             self.outputSubTomogramsSet.setAcquisition(acquisition)
@@ -210,43 +230,47 @@
         for item in precedents.iterItems():
             for ind, tomoFile in enumerate(self.tomoFiles):
                 if os.path.basename(tomoFile) == os.path.basename(item.getFileName()):
                     coordSet = self.lines[ind]
                     tsId = item.getTsId()
                     outputSet, counter = self.readSetOfSubTomograms(tomoFile,
                                                                     self.outputSubTomogramsSet,
-                                                                    coordSet, 1, counter, tsId)
+                                                                    coordSet,
+                                                                    1,
+                                                                    counter,
+                                                                    tsId,
+                                                                    newSamplingRate)
 
-        self._defineOutputs(**{OUTPUTATTRIBUTE:outputSet})
+        self._defineOutputs(**{OUTPUTATTRIBUTE: outputSet})
         self._defineSourceRelation(self.coords, outputSet)
 
-    def readSetOfSubTomograms(self, tomoFile, outputSubTomogramsSet, coordSet, factor, counter, tsId):
+    def readSetOfSubTomograms(self, tomoFile, outputSubTomogramsSet, coordSet, factor, counter, tsId, newSamplingRate):
         """
             This function set the corresponing attributes to each subtomogram. Coordinates and transformation matrix
             The output is the set of Subtomograms
         """
         self.info("Registering subtomograms for %s" % tomoFile)
 
-        outRegex = os.path.join(self._getExtraPath(tsId), pwutils.removeBaseExt(tomoFile)+'-*.mrc')
+        outRegex = os.path.join(self._getExtraPath(tsId), pwutils.removeBaseExt(tomoFile) + '-*.mrc')
 
         subtomoFileList = sorted(glob.glob(outRegex))
 
         for idx, subtomoFile in enumerate(subtomoFileList):
-
             self.debug("Registering subtomogram %s - %s" % (counter, subtomoFile))
 
             subtomogram = SubTomogram()
             subtomogram.cleanObjId()
             subtomogram.setLocation(subtomoFile)
             subtomogram.setCoordinate3D(coordSet[idx])
             transformation = coordSet[idx]._eulerMatrix
             shift_x, shift_y, shift_z = transformation.getShifts()
             transformation.setShifts(factor * shift_x,
                                      factor * shift_y,
                                      factor * shift_z)
+            subtomogram.setSamplingRate(newSamplingRate)
             subtomogram.setTransform(transformation)
             subtomogram.setVolName(tsId)
             outputSubTomogramsSet.append(subtomogram)
             counter += 1
         return outputSubTomogramsSet, counter
 
     # --------------------------- INFO functions ------------------------------
@@ -255,18 +279,16 @@
         return ["A set of %d subtomograms with dimensions %s was obtained."
                 % (toms.getSize(), toms.getDimensions())]
 
     def _validate(self):
         errors = []
         inTomograms = self.tomograms.get()
         if inTomograms is not None:
-            if abs(self.coords.get().getPrecedents().getSamplingRate() - inTomograms.getSamplingRate())> 0.01: #0.01A/px is an aceptable error
+            if abs(self.coords.get().getPrecedents().getSamplingRate() - inTomograms.getSamplingRate()) > 0.01:  # 0.01A/px is an aceptable error
                 errors.append("The coordinates has a different sampling rate than the selected tomograms."
                               "Tomograms and coordinates must be at the same scale. Please ensure a matching in the "
                               "sample rate")
         return errors
 
     def _summary(self):
         summary = []
         return summary
-
-
```

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_filter_coordinates_by_map.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_filter_coordinates_by_map.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_flexalign.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_flexalign.py`

 * *Files 17% similar despite different names*

```diff
@@ -34,17 +34,17 @@
     """
     Simple protocol to average TiltSeries movies as basic
     motion correction. It is used mainly for testing purposes.
     """
     _label = 'tiltseries FlexAlign'
     _devStatus = BETA
     evenOddCapable = True
-    
+
     def _defineParams(self, form):
-        ProtTsCorrectMotion._defineParams(self, form)
+        ProtTsCorrectMotion._defineParams(self, form, addEvenOddParam = False)
         form.addSection(label="FlexAlign")
         XmippProtFlexAlign._defineAlignmentParams(self, form)
 
     def _getOutputMicName(self, movie):
         return self._getTiltImageMRoot(movie) + ".mrc"
 
     def _processTiltImageM(self, workingFolder, tiltImageM, *args):
@@ -62,7 +62,22 @@
 
         self._processMovie(tiltImageM)
 
         # Restore user decision about saving movies
         self.doSaveMovie.set(doSaveMovie)
 
         self.inputMovies = None
+
+    def _validate(self):
+        errors = []
+        #TODO: If protocol_ts_correct_motion is refactored, then this validate should be
+        # the one of flexalign (scipion-em-xmipp).
+        if self.doLocalAlignment.get() and not self.useGpu.get():
+            errors.append("GPU is needed to do local alignment.")
+
+        if (self.binFactor.get() < 1):
+            errors.append("Bin factor must be >= 1")
+
+        return errors
+
+    def _citations(self):
+        return XmippProtFlexAlign._citations(self)
```

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_half_maps_subtomos.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_half_maps_subtomos.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_phantom_subtomo.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_phantom_subtomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_phantom_tomo.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_phantom_tomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_project_top.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_project_top.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,18 +25,18 @@
 # *
 # **************************************************************************
 import enum
 
 import numpy as np
 from pwem.emlib.image import ImageHandler as ih
 from pwem.emlib import lib
-from pwem.objects import Particle, Volume, Transform, String, SetOfVolumes, SetOfParticles
+from pwem.objects import Particle, Transform, String, SetOfVolumes, SetOfParticles
 from pwem.protocols import ProtAnalysis3D
 from pyworkflow import BETA
-from pyworkflow.protocol.params import PointerParam, EnumParam, IntParam, BooleanParam
+from pyworkflow.protocol.params import PointerParam, EnumParam, IntParam, BooleanParam, Form, LEVEL_ADVANCED
 from tomo.objects import SetOfSubTomograms
 
 class SubtomoProjectOutput(enum.Enum):
     particles = SetOfParticles
     average = Particle
 
 class XmippProtSubtomoProject(ProtAnalysis3D):
@@ -46,15 +46,15 @@
     _label = 'subtomo projection'
     _devStatus = BETA
     _possibleOutputs = SubtomoProjectOutput
 
     _dirChoices = ['X', 'Y', 'Z']
 
     # --------------------------- DEFINE param functions ------------------------
-    def _defineParams(self, form):
+    def _defineParams(self, form:Form):
         form.addSection(label='General parameters')
         form.addParam('input', PointerParam, pointerClass=[SetOfSubTomograms, SetOfVolumes],
                       label='Input Volumes', help='This protocol can *not* work with .em files *if* the input is a set'
                                                   ' of tomograms or a set of volumes, ')
         form.addParam('radAvg', BooleanParam, default=False, label='Compute radial average?',
                       help='Compute the radial average with respect to Z of the input volumes and from them, '
                            'it computes their projections in the desired direction')
@@ -62,27 +62,30 @@
                       label='Projection direction', condition='radAvg == False')
         form.addParam('rangeParam', EnumParam, choices=['All', 'Range'], default=0, display=EnumParam.DISPLAY_HLIST,
                       label='Range of slices', condition='radAvg == False',
                       help='Range of slices used to compute the projection, where 0 is the central slice.')
         form.addParam('cropParam', IntParam, default=10, label='Slices', condition="rangeParam == 1",
                       help='Crop this amount of voxels in each side of the selected direction.')
 
+        form.addBooleanParam('ignoreOrientations', label="Ignore orientations",
+                             help="Activate to ignore particle orientation information.",
+                             default=False, expertLevel=LEVEL_ADVANCED)
+
     # --------------------------- INSERT steps functions ------------------------
     def _insertAllSteps(self):
 
         self._insertFunctionStep(self.projectStep)
         self._insertFunctionStep(self.createOutputStep)
 
     # --------------------------- STEPS functions -------------------------------
     def projectStep(self):
         input = self.input.get()
         x, y, z = input.getDim()
 
-        print("Dimensions (x,y,z) are: %s, %s, %s." % (x,y,z))
-
+        self.info("Dimensions (x,y,z) are: %s, %s, %s." % (x,y,z))
 
         dir = self.dirParam.get()
         partialProjection = self.rangeParam.get() == 1
 
         if partialProjection:
             bottomSlice = int(x/2 - self.cropParam.get())
             topSlice = int(x/2 + self.cropParam.get())
@@ -95,15 +98,15 @@
 
         for subtomo in input.iterItems():
 
             fn = "%s@%s" % subtomo.getLocation()
             if fn.endswith('.mrc'):
                 fn += ':mrc'
 
-            if subtomo.hasTransform():
+            if subtomo.hasTransform() and not self.ignoreOrientations:
 
                 ih().rotateVolume(fn, tmpOrientedSubtomoFn, subtomo.getTransform())
                 fn = tmpOrientedSubtomoFn
 
             vol = ih().read(fn)
             img = ih().createImage()
```

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_resizeTS.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_resizeTS.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # **************************************************************************
 # *
-# * Authors:     Federico P. de Isidro Gomez (fp.deisidro@cnb.csi.es) [1]
+# * Authors:     Federico P. de Isidro Gomez (fp.deisidro@cnb.csic.es) [1]
 # *
 # * [1] Centro Nacional de Biotecnologia, CSIC, Spain
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 2 of the License, or
 # * (at your option) any later version.
@@ -20,19 +20,16 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
-from pwem.protocols import EMProtocol
 from pyworkflow import BETA
-from pyworkflow.protocol.params import EnumParam, FloatParam, IntParam, BooleanParam, PointerParam
-import pyworkflow.protocol.constants as const
-from tomo.protocols import ProtTomoBase
+from pyworkflow.protocol.params import PointerParam
 import os
 import pyworkflow.utils.path as path
 from pyworkflow.object import Set
 import tomo.objects as tomoObj
 from pwem.emlib.image import ImageHandler
 from xmipptomo.protocols.protocol_crop_resize_base import XmippProtResizeBase
```

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_resize_tomograms.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_resize_tomograms.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,25 +20,19 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # *********************************************************************
 
-from pwem.protocols import EMProtocol
 from pyworkflow import BETA
-from pyworkflow.protocol.params import EnumParam, FloatParam, IntParam, BooleanParam, PointerParam
-import pyworkflow.protocol.constants as const
-from tomo.protocols import ProtTomoBase
-from tomo.objects import SetOfTomograms, Tomogram
+from pyworkflow.protocol.params import PointerParam
+from tomo.objects import Tomogram
 import os
-import pyworkflow.utils.path as path
 from pyworkflow.object import Set
-import tomo.objects as tomoObj
-from pwem.emlib.image import ImageHandler
 from xmipptomo.protocols.protocol_crop_resize_base import XmippProtResizeBase
 
 
 
 class XmippProtResizeTomograms(XmippProtResizeBase):
     """
     Protocol to to resize tomograms using xmipp_image_resize.
```

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_resolution_local_monotomo.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_resolution_local_monotomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_roiIJ.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_roiIJ.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_score_coordinates.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_score_coordinates.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,16 +70,16 @@
                       label="Outliers distance threshold", condition='outliers == True and filter == 1',
                       help='Z-Score value from 0 to infinite. Only coordinates with a Z-Score smaller than '
                            'or equal to the threshold will be kept in the output')
         form.addParam('carbon', params.BooleanParam, default=True,
                       label="Score carbon closeness?")
         form.addParam('carbonThreshold', params.FloatParam, default=0.8,
                       label="Carbon distance threshold", condition='carbon == True and filter == 1',
-                      help='Score value between 0 and 1. Only coordinates with a score largen than or equal '
-                           'to the tresghold will be kept in the output')
+                      help='Score value between 0 and 1. Only coordinates with a score larger than or equal '
+                           'to the threshold will be kept in the output')
 
     # --------------------------- INSERT steps functions ----------------------
     def _insertAllSteps(self):
         pwutils.makePath(self._getExtraPath('inputCoords'))
         pwutils.makePath(self._getExtraPath('outputCoords'))
         coordinates = self.inputCoordinates.get()
         self.tomos = coordinates.getPrecedents()
```

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_score_transform.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_score_transform.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_splitTS.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_splitTS.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # **************************************************************************
 # *
-# * Authors:     Federico P. de Isidro Gomez (fp.deisidro@cnb.csi.es) [1]
+# * Authors:     Federico P. de Isidro Gomez (fp.deisidro@cnb.csic.es) [1]
 # *
 # * [1] Centro Nacional de Biotecnologia, CSIC, Spain
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 2 of the License, or
 # * (at your option) any later version.
```

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_subtomo_map_back.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_subtomo_map_back.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         form.addParam('inputTomograms', PointerParam, pointerClass="SetOfTomograms",
                       label='Original tomograms', help="Original tomograms from which the subtomograms were extracted", allowsNull=True)
         form.addParam('invertContrast', BooleanParam, default=False, label='Invert reference contrast',
                       help="Invert the contrast if the reference is black over a white background.  Xmipp, Spider, "
                            "Relion and Eman require white particles over a black background. ")
         form.addParam('paintingType', EnumParam,
                       choices=['Copy', 'Average', 'Highlight', 'Binarize'],
-                      default=PAINTING_TYPES.COPY, important=True,
+                      default=PAINTING_TYPES.HIGHLIGHT, important=True,
                       display=EnumParam.DISPLAY_HLIST,
                       label='Painting mode',
                       help='The program has several painting options:\n*Copy*: Copying the reference onto the tomogram.'
                            '\n*Average*: Setting the region occupied by the reference in the tomogram to the average '
                            'value of that region.\n*Highlight*: Add the reference multiplied by a constant to the '
                            'location specified.\n*Binarize*: Copy a binarized version of the reference onto the '
                            'tomogram.')
```

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols/protocol_subtraction_subtomo.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols/protocol_subtraction_subtomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/protocols.conf` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/protocols.conf`

 * *Files 5% similar despite different names*

```diff
@@ -11,19 +11,21 @@
             ]}
 	]},
 	{"tag": "section", "text": "Tomograms", "children": [
 	    {"tag": "protocol_group", "text": "Preprocess", "openItem": "False", "children": [
                 {"tag": "protocol", "value": "XmippProtResizeTomograms", "text": "default"}
 	    ]},
 	    {"tag": "protocol_group", "text": "Quality Analysis", "openItem": "False", "children": [
-                {"tag": "protocol", "value": "XmippProtMonoTomo", "text": "default"}
+                {"tag": "protocol", "value": "XmippProtMonoTomo", "text": "default"},
+                {"tag": "protocol", "value": "XmippProtDeepDetectMisalignment",   "text": "default"}
 	    ]}
 	]},
 	{"tag": "section", "text": "Particles", "children": [
 	    {"tag": "protocol_group", "text": "Picking", "openItem": "False", "children": [
+            {"tag": "protocol", "value": "XmippProtPeakHighContrast",   "text": "default"},
 	        {"tag": "protocol", "value": "XmippProtConnectedComponents", "text": "default"},
 	        {"tag": "protocol", "value": "XmippProtRoiIJ",   "text": "default"},
 		    {"tag": "protocol", "value": "XmippProtCCroi",   "text": "default"},
             {"tag": "protocol", "value": "XmippProtScoreCoordinates",   "text": "default"}
             ]}
         ]},
 	{"tag": "section", "text": "Subtomogram averaging", "children": [
```

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/tests/__init__.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/tests/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,13 +23,20 @@
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 from pyworkflow.tests import DataSet
 
-DataSet(name='monotomo', folder='monotomo',
+DataSet(name='monotomo',
+        folder='monotomo',
         files={'even1': 'even_tomogram_rx1.mrc',
                'even2': 'even_tomogram_rx2.mrc',
                'odd1': 'even_tomogram_rx1.mrc',
                'odd2': 'even_tomogram_rx2.mrc',
                })
+
+DataSet(name='deepMisaliTomo',
+        folder='monotomo',
+        files={
+            'tomo1': 'even_tomogram_rx1.mrc'
+        })
```

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/tests/test_protocol_extract_subtomos.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/tests/test_protocol_extract_subtomos.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,23 +19,22 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
-from pyworkflow.tests import BaseTest, DataSet, setupTestProject
+from pyworkflow.tests import BaseTest, setupTestProject
 from tomo.protocols.protocol_import_coordinates import IMPORT_FROM_EMAN
 from ..protocols import *
 import tomo.protocols
 
 from xmipptomo.protocols.protocol_extract_subtomos import OUTPUTATTRIBUTE
 from xmipptomo.protocols import XmippProtExtractSubtomos
 
-
 class TestXmippProtExtractSubtomosBase(BaseTest):
     @classmethod
     def setUpClass(cls):
         setupTestProject(cls)
 
     @classmethod
     def setData(cls, projectData='tomo-em'):
@@ -43,24 +42,23 @@
         cls.dataset = DataSet.getDataSet(projectData)
         cls.tomogram = cls.dataset.getFile('tomo1')
         cls.coords3D = cls.dataset.getFile('overview_wbp.txt')
         cls.coords3D_Large = cls.dataset.getFile('overview_wbp_large.txt')
         cls.inputSetOfSubTomogram = cls.dataset.getFile('subtomo')
         cls.smallTomogram = cls.dataset.getFile('coremask_normcorona.mrc')
 
-
-class TestXmippProtExtractSubtomos(TestXmippProtExtractSubtomosBase):
-    """This class check if the protocol to extract subtomograms in Xmipptomo works properly.
+class TestXmippProtExtractSubtomosProts(TestXmippProtExtractSubtomosBase):
+    """
+    This prepares the protocols to perform the necessary tests.
     """
-
     @classmethod
     def setUpClass(cls):
         setupTestProject(cls)
-        TestXmippProtExtractSubtomosBase.setData()
-
+        TestXmippProtExtractSubtomosProts.setData()
+        
     def _runImportCoordinatesAndTomograms(self):
         protImportTomogram = self.newProtocol(tomo.protocols.ProtImportTomograms,
                                               filesPath=self.tomogram,
                                               samplingRate=5)
 
         self.launchProtocol(protImportTomogram)
 
@@ -92,30 +90,29 @@
                                                   invertContrast=doInvert,
                                                   boxSize=boxSize)
         self.launchProtocol(protTomoExtraction)
         self.assertSetSize(getattr(protTomoExtraction, OUTPUTATTRIBUTE), 5,
                            "There was a problem with SetOfSubtomogram output")
         return protTomoExtraction
 
-
+class TestXmippProtExtractSubtomos(TestXmippProtExtractSubtomosProts):
+    """
+    This class check if the protocol to extract subtomograms in Xmipptomo works properly.
+    """
     def test_extractParticlesWithDoInvert(self):
         protTomoExtraction = self._runXmippTomoExtraction(doInvert=True)
         output = getattr(protTomoExtraction, OUTPUTATTRIBUTE)
         self.assessOutput(output)
 
-
     def test_extractParticlesModifiedBoxSize(self):
         protTomoExtraction = self._runXmippTomoExtraction(boxSize=64)
         output =getattr(protTomoExtraction, OUTPUTATTRIBUTE)
         self.assessOutput(output)
 
     def test_extractParticlesFromDifferentTomogram(self):
         protTomoExtraction = self._runXmippTomoExtraction(differenttomogram=True)
         output =getattr(protTomoExtraction, OUTPUTATTRIBUTE)
         self.assessOutput(output)
 
-
     def assessOutput(self, outputSet, size=5):
-
         self.assertSetSize(outputSet, size)
-        self.assertTrue(outputSet.hasCoordinates3D())
-
+        self.assertTrue(outputSet.hasCoordinates3D())
```

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/tests/test_protocol_monotomo.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/tests/test_protocol_monotomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/tests/test_protocol_phantom_subtomo.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/tests/test_protocol_phantom_subtomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/tests/test_protocols_crop.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/tests/test_protocols_crop.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/tests/test_protocols_resize.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/tests/test_protocols_resize.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/tests/test_protocols_xmipptomo.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/tests/test_protocols_xmipptomo.py`

 * *Files 0% similar despite different names*

```diff
@@ -518,15 +518,16 @@
 class TestXmipptomoSplitTS(BaseTest):
     """This class check if the protocol split tilt-series works properly."""
 
     @classmethod
     def setUpClass(cls):
         setupTestProject(cls)
         cls.inputDataSet = DataSet.getDataSet('tomo-em')
-        cls.inputSoTS = cls.inputDataSet.getFile('ts1_imod')
+        cls.inputSoTS = cls.inputDataSet.getFile('tutorialData/BB*.st')
+
 
     def runWorkflow(self):
         protImportTS = self.newProtocol(ProtImportTs,
                                         filesPath=os.path.split(self.inputSoTS)[0],
                                         filesPattern="BB{TS}.st",
                                         voltage=300,
                                         anglesFrom=0,
```

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/viewers/monotomo_tree_provider.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/viewers/monotomo_tree_provider.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/viewers/viewer_cltomo.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/viewers/viewer_cltomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/viewers/viewer_phantom_create.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/viewers/viewer_phantom_create.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/viewers/viewer_resolution_local_monotomo.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/viewers/viewer_resolution_local_monotomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/viewers/viewer_score_subtomos.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/viewers/viewer_score_subtomos.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/wizards.py` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/wizards.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipptomo-3.23.3.6/xmipptomo/xmipp_logo.png` & `scipion-em-xmipptomo-3.23.7.0/xmipptomo/xmipp_logo.png`

 * *Files identical despite different names*

