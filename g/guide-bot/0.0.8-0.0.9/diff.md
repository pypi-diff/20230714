# Comparing `tmp/guide_bot-0.0.8.tar.gz` & `tmp/guide_bot-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/guide_bot-0.0.8.tar", last modified: Tue May 11 19:24:19 2021, max compression
+gzip compressed data, was "dist/guide_bot-0.0.9.tar", last modified: Wed May 12 07:05:01 2021, max compression
```

## Comparing `guide_bot-0.0.8.tar` & `guide_bot-0.0.9.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 madsbertelsen (1083417152) 14964212        0 2021-05-11 19:24:19.000000 guide_bot-0.0.8/
--rw-r--r--   0 madsbertelsen (1083417152) 14964212       33 2021-05-11 13:43:49.000000 guide_bot-0.0.8/MANIFEST.in
--rw-r--r--   0 madsbertelsen (1083417152) 14964212    15143 2021-05-11 19:24:19.000000 guide_bot-0.0.8/PKG-INFO
--rw-r--r--   0 madsbertelsen (1083417152) 14964212    12738 2021-05-11 09:33:08.000000 guide_bot-0.0.8/README.md
-drwxr-xr-x   0 madsbertelsen (1083417152) 14964212        0 2021-05-11 19:24:19.000000 guide_bot-0.0.8/examples/
--rw-r--r--   0 madsbertelsen (1083417152) 14964212     9968 2021-05-11 10:38:12.000000 guide_bot-0.0.8/examples/simple_scan.ipynb
-drwxr-xr-x   0 madsbertelsen (1083417152) 14964212        0 2021-05-11 19:24:19.000000 guide_bot-0.0.8/guide_bot/
--rw-r--r--   0 madsbertelsen (1083417152) 14964212        0 2021-01-05 10:43:56.000000 guide_bot-0.0.8/guide_bot/__init__.py
-drwxr-xr-x   0 madsbertelsen (1083417152) 14964212        0 2021-05-11 19:24:19.000000 guide_bot-0.0.8/guide_bot/base_elements/
--rw-r--r--   0 madsbertelsen (1083417152) 14964212        0 2021-01-05 10:43:56.000000 guide_bot-0.0.8/guide_bot/base_elements/__init__.py
--rw-r--r--   0 madsbertelsen (1083417152) 14964212     8720 2021-05-10 15:20:44.000000 guide_bot-0.0.8/guide_bot/base_elements/element_group.py
--rw-r--r--   0 madsbertelsen (1083417152) 14964212    12880 2021-01-05 10:43:56.000000 guide_bot-0.0.8/guide_bot/base_elements/guide_elements.py
-drwxr-xr-x   0 madsbertelsen (1083417152) 14964212        0 2021-05-11 19:24:19.000000 guide_bot-0.0.8/guide_bot/cluster/
--rw-r--r--   0 madsbertelsen (1083417152) 14964212     1469 2021-05-11 12:11:24.000000 guide_bot-0.0.8/guide_bot/cluster/Base.py
--rw-r--r--   0 madsbertelsen (1083417152) 14964212     6362 2021-05-11 09:31:37.000000 guide_bot-0.0.8/guide_bot/cluster/SLURM.py
--rw-r--r--   0 madsbertelsen (1083417152) 14964212        0 2021-03-17 14:38:59.000000 guide_bot-0.0.8/guide_bot/cluster/__init__.py
-drwxr-xr-x   0 madsbertelsen (1083417152) 14964212        0 2021-05-11 19:24:19.000000 guide_bot-0.0.8/guide_bot/cluster_config/
--rw-r--r--   0 madsbertelsen (1083417152) 14964212     1149 2021-03-17 14:38:59.000000 guide_bot-0.0.8/guide_bot/cluster_config/DMSC.yaml
-drwxr-xr-x   0 madsbertelsen (1083417152) 14964212        0 2021-05-11 19:24:19.000000 guide_bot-0.0.8/guide_bot/elements/
--rw-r--r--   0 madsbertelsen (1083417152) 14964212    12569 2021-05-06 07:36:22.000000 guide_bot-0.0.8/guide_bot/elements/Element_elliptic.py
--rw-r--r--   0 madsbertelsen (1083417152) 14964212     3031 2021-01-05 10:43:56.000000 guide_bot-0.0.8/guide_bot/elements/Element_gap.py
--rw-r--r--   0 madsbertelsen (1083417152) 14964212     3881 2021-05-10 15:20:44.000000 guide_bot-0.0.8/guide_bot/elements/Element_straight.py
--rw-r--r--   0 madsbertelsen (1083417152) 14964212       91 2021-01-05 10:43:56.000000 guide_bot-0.0.8/guide_bot/elements/__init__.py
-drwxr-xr-x   0 madsbertelsen (1083417152) 14964212        0 2021-05-11 19:24:19.000000 guide_bot-0.0.8/guide_bot/logic/
--rw-r--r--   0 madsbertelsen (1083417152) 14964212        0 2021-01-05 10:43:56.000000 guide_bot-0.0.8/guide_bot/logic/__init__.py
--rw-r--r--   0 madsbertelsen (1083417152) 14964212    21764 2021-05-10 15:20:44.000000 guide_bot-0.0.8/guide_bot/logic/guide_bot_main.py
--rw-r--r--   0 madsbertelsen (1083417152) 14964212     8692 2021-05-10 15:20:44.000000 guide_bot-0.0.8/guide_bot/logic/length_system.py
--rw-r--r--   0 madsbertelsen (1083417152) 14964212    10976 2021-05-10 15:20:44.000000 guide_bot-0.0.8/guide_bot/logic/runner.py
-drwxr-xr-x   0 madsbertelsen (1083417152) 14964212        0 2021-05-11 19:24:19.000000 guide_bot-0.0.8/guide_bot/optimizer/
--rw-r--r--   0 madsbertelsen (1083417152) 14964212        0 2021-01-05 10:43:56.000000 guide_bot-0.0.8/guide_bot/optimizer/__init__.py
--rw-r--r--   0 madsbertelsen (1083417152) 14964212     7796 2021-05-10 15:20:44.000000 guide_bot-0.0.8/guide_bot/optimizer/optimizer.py
-drwxr-xr-x   0 madsbertelsen (1083417152) 14964212        0 2021-05-11 19:24:19.000000 guide_bot-0.0.8/guide_bot/parameters/
--rw-r--r--   0 madsbertelsen (1083417152) 14964212        0 2021-01-05 10:43:56.000000 guide_bot-0.0.8/guide_bot/parameters/__init__.py
--rw-r--r--   0 madsbertelsen (1083417152) 14964212     3792 2021-01-05 10:43:56.000000 guide_bot-0.0.8/guide_bot/parameters/constraints.py
--rw-r--r--   0 madsbertelsen (1083417152) 14964212    15043 2021-01-05 10:43:56.000000 guide_bot-0.0.8/guide_bot/parameters/instrument_parameter_container.py
--rw-r--r--   0 madsbertelsen (1083417152) 14964212    13226 2021-01-05 10:43:56.000000 guide_bot-0.0.8/guide_bot/parameters/instrument_parameters.py
-drwxr-xr-x   0 madsbertelsen (1083417152) 14964212        0 2021-05-11 19:24:19.000000 guide_bot-0.0.8/guide_bot/requirements/
--rw-r--r--   0 madsbertelsen (1083417152) 14964212    33457 2021-05-10 15:20:44.000000 guide_bot-0.0.8/guide_bot/requirements/Sample.py
--rw-r--r--   0 madsbertelsen (1083417152) 14964212    21753 2021-05-10 15:20:44.000000 guide_bot-0.0.8/guide_bot/requirements/Source.py
--rw-r--r--   0 madsbertelsen (1083417152) 14964212        0 2021-01-05 10:43:56.000000 guide_bot-0.0.8/guide_bot/requirements/__init__.py
--rw-r--r--   0 madsbertelsen (1083417152) 14964212    16828 2021-05-10 15:20:44.000000 guide_bot-0.0.8/guide_bot/requirements/requirement_parameters.py
-drwxr-xr-x   0 madsbertelsen (1083417152) 14964212        0 2021-05-11 19:24:19.000000 guide_bot-0.0.8/guide_bot/scan_visualization/
--rw-r--r--   0 madsbertelsen (1083417152) 14964212        0 2021-05-11 19:21:47.000000 guide_bot-0.0.8/guide_bot/scan_visualization/__init__.py
--rw-r--r--   0 madsbertelsen (1083417152) 14964212    35663 2021-05-10 15:20:44.000000 guide_bot-0.0.8/guide_bot/scan_visualization/jb_interface.py
--rw-r--r--   0 madsbertelsen (1083417152) 14964212    18022 2021-05-10 15:20:44.000000 guide_bot-0.0.8/guide_bot/scan_visualization/overview.py
-drwxr-xr-x   0 madsbertelsen (1083417152) 14964212        0 2021-05-11 19:24:19.000000 guide_bot-0.0.8/guide_bot/tests/
--rw-r--r--   0 madsbertelsen (1083417152) 14964212        0 2021-01-05 10:43:56.000000 guide_bot-0.0.8/guide_bot/tests/__init__.py
--rw-r--r--   0 madsbertelsen (1083417152) 14964212      997 2021-01-05 10:43:56.000000 guide_bot-0.0.8/guide_bot/tests/short_requirement_parameters.py
--rw-r--r--   0 madsbertelsen (1083417152) 14964212     2038 2021-01-05 10:43:56.000000 guide_bot-0.0.8/guide_bot/tests/test_Constraints.py
--rw-r--r--   0 madsbertelsen (1083417152) 14964212    10954 2021-01-05 10:43:56.000000 guide_bot-0.0.8/guide_bot/tests/test_guide_elements.py
--rw-r--r--   0 madsbertelsen (1083417152) 14964212     2081 2021-01-05 10:43:56.000000 guide_bot-0.0.8/guide_bot/tests/test_instrument_parameter_container.py
--rw-r--r--   0 madsbertelsen (1083417152) 14964212     5968 2021-01-05 10:43:56.000000 guide_bot-0.0.8/guide_bot/tests/test_instrument_parameters.py
--rw-r--r--   0 madsbertelsen (1083417152) 14964212    12607 2021-01-05 10:43:56.000000 guide_bot-0.0.8/guide_bot/tests/test_requirement_parameters.py
-drwxr-xr-x   0 madsbertelsen (1083417152) 14964212        0 2021-05-11 19:24:19.000000 guide_bot-0.0.8/guide_bot.egg-info/
--rw-r--r--   0 madsbertelsen (1083417152) 14964212    15143 2021-05-11 19:24:19.000000 guide_bot-0.0.8/guide_bot.egg-info/PKG-INFO
--rw-r--r--   0 madsbertelsen (1083417152) 14964212     1555 2021-05-11 19:24:19.000000 guide_bot-0.0.8/guide_bot.egg-info/SOURCES.txt
--rw-r--r--   0 madsbertelsen (1083417152) 14964212        1 2021-05-11 19:24:19.000000 guide_bot-0.0.8/guide_bot.egg-info/dependency_links.txt
--rw-r--r--   0 madsbertelsen (1083417152) 14964212       68 2021-05-11 19:24:19.000000 guide_bot-0.0.8/guide_bot.egg-info/requires.txt
--rw-r--r--   0 madsbertelsen (1083417152) 14964212       10 2021-05-11 19:24:19.000000 guide_bot-0.0.8/guide_bot.egg-info/top_level.txt
--rw-r--r--   0 madsbertelsen (1083417152) 14964212       38 2021-05-11 19:24:19.000000 guide_bot-0.0.8/setup.cfg
--rw-r--r--   0 madsbertelsen (1083417152) 14964212      816 2021-05-11 19:24:18.000000 guide_bot-0.0.8/setup.py
+drwxr-xr-x   0 madsbertelsen (1083417152) 14964212        0 2021-05-12 07:05:01.000000 guide_bot-0.0.9/
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212       33 2021-05-11 13:43:49.000000 guide_bot-0.0.9/MANIFEST.in
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212    15142 2021-05-12 07:05:01.000000 guide_bot-0.0.9/PKG-INFO
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212    12737 2021-05-12 06:46:30.000000 guide_bot-0.0.9/README.md
+drwxr-xr-x   0 madsbertelsen (1083417152) 14964212        0 2021-05-12 07:05:01.000000 guide_bot-0.0.9/examples/
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212     9968 2021-05-11 10:38:12.000000 guide_bot-0.0.9/examples/simple_scan.ipynb
+drwxr-xr-x   0 madsbertelsen (1083417152) 14964212        0 2021-05-12 07:05:01.000000 guide_bot-0.0.9/guide_bot/
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212        0 2021-01-05 10:43:56.000000 guide_bot-0.0.9/guide_bot/__init__.py
+drwxr-xr-x   0 madsbertelsen (1083417152) 14964212        0 2021-05-12 07:05:01.000000 guide_bot-0.0.9/guide_bot/base_elements/
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212        0 2021-01-05 10:43:56.000000 guide_bot-0.0.9/guide_bot/base_elements/__init__.py
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212     8720 2021-05-10 15:20:44.000000 guide_bot-0.0.9/guide_bot/base_elements/element_group.py
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212    12880 2021-01-05 10:43:56.000000 guide_bot-0.0.9/guide_bot/base_elements/guide_elements.py
+drwxr-xr-x   0 madsbertelsen (1083417152) 14964212        0 2021-05-12 07:05:01.000000 guide_bot-0.0.9/guide_bot/cluster/
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212     1469 2021-05-11 12:11:24.000000 guide_bot-0.0.9/guide_bot/cluster/Base.py
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212     6362 2021-05-11 09:31:37.000000 guide_bot-0.0.9/guide_bot/cluster/SLURM.py
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212        0 2021-03-17 14:38:59.000000 guide_bot-0.0.9/guide_bot/cluster/__init__.py
+drwxr-xr-x   0 madsbertelsen (1083417152) 14964212        0 2021-05-12 07:05:01.000000 guide_bot-0.0.9/guide_bot/cluster_config/
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212     1149 2021-03-17 14:38:59.000000 guide_bot-0.0.9/guide_bot/cluster_config/DMSC.yaml
+drwxr-xr-x   0 madsbertelsen (1083417152) 14964212        0 2021-05-12 07:05:01.000000 guide_bot-0.0.9/guide_bot/elements/
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212    12569 2021-05-06 07:36:22.000000 guide_bot-0.0.9/guide_bot/elements/Element_elliptic.py
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212     3031 2021-01-05 10:43:56.000000 guide_bot-0.0.9/guide_bot/elements/Element_gap.py
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212     3881 2021-05-10 15:20:44.000000 guide_bot-0.0.9/guide_bot/elements/Element_straight.py
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212       91 2021-01-05 10:43:56.000000 guide_bot-0.0.9/guide_bot/elements/__init__.py
+drwxr-xr-x   0 madsbertelsen (1083417152) 14964212        0 2021-05-12 07:05:01.000000 guide_bot-0.0.9/guide_bot/logic/
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212        0 2021-01-05 10:43:56.000000 guide_bot-0.0.9/guide_bot/logic/__init__.py
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212    21764 2021-05-10 15:20:44.000000 guide_bot-0.0.9/guide_bot/logic/guide_bot_main.py
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212     8692 2021-05-10 15:20:44.000000 guide_bot-0.0.9/guide_bot/logic/length_system.py
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212    10976 2021-05-10 15:20:44.000000 guide_bot-0.0.9/guide_bot/logic/runner.py
+drwxr-xr-x   0 madsbertelsen (1083417152) 14964212        0 2021-05-12 07:05:01.000000 guide_bot-0.0.9/guide_bot/optimizer/
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212        0 2021-01-05 10:43:56.000000 guide_bot-0.0.9/guide_bot/optimizer/__init__.py
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212     7796 2021-05-10 15:20:44.000000 guide_bot-0.0.9/guide_bot/optimizer/optimizer.py
+drwxr-xr-x   0 madsbertelsen (1083417152) 14964212        0 2021-05-12 07:05:01.000000 guide_bot-0.0.9/guide_bot/parameters/
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212        0 2021-01-05 10:43:56.000000 guide_bot-0.0.9/guide_bot/parameters/__init__.py
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212     3792 2021-01-05 10:43:56.000000 guide_bot-0.0.9/guide_bot/parameters/constraints.py
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212    15043 2021-01-05 10:43:56.000000 guide_bot-0.0.9/guide_bot/parameters/instrument_parameter_container.py
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212    13226 2021-01-05 10:43:56.000000 guide_bot-0.0.9/guide_bot/parameters/instrument_parameters.py
+drwxr-xr-x   0 madsbertelsen (1083417152) 14964212        0 2021-05-12 07:05:01.000000 guide_bot-0.0.9/guide_bot/requirements/
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212    33457 2021-05-10 15:20:44.000000 guide_bot-0.0.9/guide_bot/requirements/Sample.py
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212    21753 2021-05-10 15:20:44.000000 guide_bot-0.0.9/guide_bot/requirements/Source.py
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212        0 2021-01-05 10:43:56.000000 guide_bot-0.0.9/guide_bot/requirements/__init__.py
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212    16828 2021-05-10 15:20:44.000000 guide_bot-0.0.9/guide_bot/requirements/requirement_parameters.py
+drwxr-xr-x   0 madsbertelsen (1083417152) 14964212        0 2021-05-12 07:05:01.000000 guide_bot-0.0.9/guide_bot/scan_visualization/
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212        0 2021-05-11 19:21:47.000000 guide_bot-0.0.9/guide_bot/scan_visualization/__init__.py
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212    36634 2021-05-12 06:56:50.000000 guide_bot-0.0.9/guide_bot/scan_visualization/jb_interface.py
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212    18917 2021-05-12 06:26:02.000000 guide_bot-0.0.9/guide_bot/scan_visualization/overview.py
+drwxr-xr-x   0 madsbertelsen (1083417152) 14964212        0 2021-05-12 07:05:01.000000 guide_bot-0.0.9/guide_bot/tests/
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212        0 2021-01-05 10:43:56.000000 guide_bot-0.0.9/guide_bot/tests/__init__.py
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212      997 2021-01-05 10:43:56.000000 guide_bot-0.0.9/guide_bot/tests/short_requirement_parameters.py
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212     2038 2021-01-05 10:43:56.000000 guide_bot-0.0.9/guide_bot/tests/test_Constraints.py
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212    10954 2021-01-05 10:43:56.000000 guide_bot-0.0.9/guide_bot/tests/test_guide_elements.py
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212     2081 2021-01-05 10:43:56.000000 guide_bot-0.0.9/guide_bot/tests/test_instrument_parameter_container.py
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212     5968 2021-01-05 10:43:56.000000 guide_bot-0.0.9/guide_bot/tests/test_instrument_parameters.py
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212    12607 2021-01-05 10:43:56.000000 guide_bot-0.0.9/guide_bot/tests/test_requirement_parameters.py
+drwxr-xr-x   0 madsbertelsen (1083417152) 14964212        0 2021-05-12 07:05:01.000000 guide_bot-0.0.9/guide_bot.egg-info/
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212    15142 2021-05-12 07:05:01.000000 guide_bot-0.0.9/guide_bot.egg-info/PKG-INFO
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212     1555 2021-05-12 07:05:01.000000 guide_bot-0.0.9/guide_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212        1 2021-05-12 07:05:01.000000 guide_bot-0.0.9/guide_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212       68 2021-05-12 07:05:01.000000 guide_bot-0.0.9/guide_bot.egg-info/requires.txt
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212       10 2021-05-12 07:05:01.000000 guide_bot-0.0.9/guide_bot.egg-info/top_level.txt
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212       38 2021-05-12 07:05:01.000000 guide_bot-0.0.9/setup.cfg
+-rw-r--r--   0 madsbertelsen (1083417152) 14964212      816 2021-05-12 07:01:47.000000 guide_bot-0.0.9/setup.py
```

### Comparing `guide_bot-0.0.8/PKG-INFO` & `guide_bot-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guide_bot
-Version: 0.0.8
+Version: 0.0.9
 Summary: Neutron guide optimization package
 Home-page: https://git.esss.dk/highness/guide_bot
 Author: Mads Bertelsen
 Author-email: Mads.Bertelsen@ess.eu
 License: UNKNOWN
 Description: # Early version of guide_bot in python
         
@@ -232,15 +232,15 @@
         ```
         The run_status method shows the status of all runs, check if any failed.
         
         After the scan_overview have loaded the data, its possible to visualize with 4 different widgets:
         
         - PlotAnyMonitor: Plots any single monitor
         - CompareMonitors: Compare 1D monitors for any number of guides
-        - CompareMonitorsScans: Compare 1D monitors over a scan
+        - CompareMonitorsScan: Compare 1D monitors over a scan
         - PlotSum: Shows sum of any monitor as function of scan
         
         They are all displayed with the same setup, for example here with PlotAnyMonitor as example
         ```
         scan_interface = jb_interface.PlotSum(scan_overview)
         scan_interface.show_interface()
         ```
```

### Comparing `guide_bot-0.0.8/README.md` & `guide_bot-0.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
 ```
 The run_status method shows the status of all runs, check if any failed.
 
 After the scan_overview have loaded the data, its possible to visualize with 4 different widgets:
 
 - PlotAnyMonitor: Plots any single monitor
 - CompareMonitors: Compare 1D monitors for any number of guides
-- CompareMonitorsScans: Compare 1D monitors over a scan
+- CompareMonitorsScan: Compare 1D monitors over a scan
 - PlotSum: Shows sum of any monitor as function of scan
 
 They are all displayed with the same setup, for example here with PlotAnyMonitor as example
 ```
 scan_interface = jb_interface.PlotSum(scan_overview)
 scan_interface.show_interface()
 ```
```

### Comparing `guide_bot-0.0.8/examples/simple_scan.ipynb` & `guide_bot-0.0.9/examples/simple_scan.ipynb`

 * *Files identical despite different names*

### Comparing `guide_bot-0.0.8/guide_bot/base_elements/element_group.py` & `guide_bot-0.0.9/guide_bot/base_elements/element_group.py`

 * *Files identical despite different names*

### Comparing `guide_bot-0.0.8/guide_bot/base_elements/guide_elements.py` & `guide_bot-0.0.9/guide_bot/base_elements/guide_elements.py`

 * *Files identical despite different names*

### Comparing `guide_bot-0.0.8/guide_bot/cluster/Base.py` & `guide_bot-0.0.9/guide_bot/cluster/Base.py`

 * *Files identical despite different names*

### Comparing `guide_bot-0.0.8/guide_bot/cluster/SLURM.py` & `guide_bot-0.0.9/guide_bot/cluster/SLURM.py`

 * *Files identical despite different names*

### Comparing `guide_bot-0.0.8/guide_bot/cluster_config/DMSC.yaml` & `guide_bot-0.0.9/guide_bot/cluster_config/DMSC.yaml`

 * *Files identical despite different names*

### Comparing `guide_bot-0.0.8/guide_bot/elements/Element_elliptic.py` & `guide_bot-0.0.9/guide_bot/elements/Element_elliptic.py`

 * *Files identical despite different names*

### Comparing `guide_bot-0.0.8/guide_bot/elements/Element_gap.py` & `guide_bot-0.0.9/guide_bot/elements/Element_gap.py`

 * *Files identical despite different names*

### Comparing `guide_bot-0.0.8/guide_bot/elements/Element_straight.py` & `guide_bot-0.0.9/guide_bot/elements/Element_straight.py`

 * *Files identical despite different names*

### Comparing `guide_bot-0.0.8/guide_bot/logic/guide_bot_main.py` & `guide_bot-0.0.9/guide_bot/logic/guide_bot_main.py`

 * *Files identical despite different names*

### Comparing `guide_bot-0.0.8/guide_bot/logic/length_system.py` & `guide_bot-0.0.9/guide_bot/logic/length_system.py`

 * *Files identical despite different names*

### Comparing `guide_bot-0.0.8/guide_bot/logic/runner.py` & `guide_bot-0.0.9/guide_bot/logic/runner.py`

 * *Files identical despite different names*

### Comparing `guide_bot-0.0.8/guide_bot/optimizer/optimizer.py` & `guide_bot-0.0.9/guide_bot/optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `guide_bot-0.0.8/guide_bot/parameters/constraints.py` & `guide_bot-0.0.9/guide_bot/parameters/constraints.py`

 * *Files identical despite different names*

### Comparing `guide_bot-0.0.8/guide_bot/parameters/instrument_parameter_container.py` & `guide_bot-0.0.9/guide_bot/parameters/instrument_parameter_container.py`

 * *Files identical despite different names*

### Comparing `guide_bot-0.0.8/guide_bot/parameters/instrument_parameters.py` & `guide_bot-0.0.9/guide_bot/parameters/instrument_parameters.py`

 * *Files identical despite different names*

### Comparing `guide_bot-0.0.8/guide_bot/requirements/Sample.py` & `guide_bot-0.0.9/guide_bot/requirements/Sample.py`

 * *Files identical despite different names*

### Comparing `guide_bot-0.0.8/guide_bot/requirements/Source.py` & `guide_bot-0.0.9/guide_bot/requirements/Source.py`

 * *Files identical despite different names*

### Comparing `guide_bot-0.0.8/guide_bot/requirements/requirement_parameters.py` & `guide_bot-0.0.9/guide_bot/requirements/requirement_parameters.py`

 * *Files identical despite different names*

### Comparing `guide_bot-0.0.8/guide_bot/scan_visualization/jb_interface.py` & `guide_bot-0.0.9/guide_bot/scan_visualization/jb_interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,22 @@
 
         self.guide_names = self.scan_overview.get_guide_names()
         self.guide_enable = {}
         for guide in self.guide_names:
             self.guide_enable[guide] = True
 
         n_pars = self.scan_overview.get_n_scanned_parameters()
-        self.list_indicies = [0] * n_pars
+        #self.list_indicies = [0] * n_pars
+
+        if len(self.scan_overview.succesful_indices) == 0:
+            raise RuntimeError("No succesful runs found. Run load_all_guide_information in overview object.")
+        else:
+            self.guides_with_at_least_one_run = list(self.scan_overview.succesful_indices.keys())
+            succesful_guide = self.guides_with_at_least_one_run[0]
+            self.list_indicies = list(self.scan_overview.succesful_indices[succesful_guide][0])
 
         self.moderator = self.get_moderator_list()[0]
         self.run_name = self.get_run_name_list()[0]
         self.monitor = self.get_monitor_list()[0]
 
         self.moderator_scan_labels = None
         self.moderator_scan_sliders = None
@@ -60,15 +67,15 @@
             if self.guide_enable[guide]:
                 enabled_guides.append(guide)
         return enabled_guides
 
     def get_monitor_list(self):
         shape = self.scan_overview.get_shape()
         indicies = tuple(self.list_indicies)
-        guide = self.guide_names[0]
+        guide = self.guides_with_at_least_one_run[0]
         moderator = self.get_moderator_list()[0]
 
         if self.scan_overview.data[guide][indicies][moderator] is not None:
             runs = self.scan_overview.data[guide][indicies][moderator].runs
             return runs[self.run_name].get_monitor_list()
         else:
             return []
@@ -78,24 +85,27 @@
             raise KeyError("Monitor named " + monitor + " not available.")
 
         self.monitor = monitor
 
     def get_run_name_list(self):
         shape = self.scan_overview.get_shape()
         indicies = tuple(self.list_indicies)
-        guide = self.guide_names[0]
+        guide = self.guides_with_at_least_one_run[0]
         moderator = self.get_moderator_list()[0]
 
         if self.scan_overview.data[guide][indicies][moderator] is not None:
             runs = self.scan_overview.data[guide][indicies][moderator].runs
             return list(runs.keys())
         else:
             return []
 
     def set_run_name(self, run_name):
+        if run_name is None:
+            return
+
         if run_name not in self.get_run_name_list():
             raise KeyError("Run named " + str(run_name) + " not available.")
 
         self.run_name = run_name
 
     def get_moderator_list(self):
         return self.scan_overview.get_moderators()
@@ -223,22 +233,25 @@
         sample_sliders = []
         sample_labels = []
         full_sample_sliders = []
         self.sample_scan_sliders = {}
         self.sample_scan_labels = {}
         for sample_par in self.get_scanned_sample_parameters():
             max_index = self.get_par_max_index(sample_par, "sample")
-            widget = widgets.IntSlider(value=0, min=0, max=max_index, step=1,
+            global_index = self.scan_overview.get_global_index_from_sample_parameter(sample_par)
+            current_index = self.list_indicies[global_index]
+
+            widget = widgets.IntSlider(value=current_index, min=0, max=max_index, step=1,
                                        description=sample_par, readout=False,
                                        layout=widgets.Layout(width="80%"))
             self.sample_scan_sliders[sample_par] = widget
             sample_sliders.append(widget)
 
 
-            initial_value = self.get_scanned_sample_parameter_values(sample_par)[0]
+            initial_value = self.get_scanned_sample_parameter_values(sample_par)[current_index]
             unit = self.get_scanned_sample_parameter_unit(sample_par)
             if unit is not None:
                 value_string = str(initial_value) + " [" + str(unit) + "]"
             else:
                 value_string = str(initial_value)
 
             widget_label = widgets.Label(value=value_string)
@@ -271,35 +284,37 @@
         current_run_name = self.dropdown_run_name.value
         new_options = tuple(self.get_run_name_list())
 
         self.dropdown_run_name.options = new_options
         if current_run_name in new_options:
             self.set_run_name(current_run_name)
             self.dropdown_run_name.value = current_run_name
-        else:
+        elif len(new_options) > 0:
             self.set_run_name(new_options[0])
             self.dropdown_run_name.value = new_options[0]
 
         self.update_plot()
 
     def make_moderator_scan_sliders(self):
         moderator_sliders = []
         moderator_labels = []
         full_moderator_sliders = []
         self.moderator_scan_sliders = {}
         self.moderator_scan_labels = {}
         for moderator_par in self.get_scanned_moderator_parameters():
             max_index = self.get_par_max_index(moderator_par, "moderator")
-            widget = widgets.IntSlider(value=0, min=0, max=max_index, step=1,
+            global_index = self.scan_overview.get_global_index_from_moderator_parameter(moderator_par)
+            current_index = self.list_indicies[global_index]
+            widget = widgets.IntSlider(value=current_index, min=0, max=max_index, step=1,
                                        description=moderator_par, readout=False,
                                        layout=widgets.Layout(width="80%"))
             moderator_sliders.append(widget)
             self.moderator_scan_sliders[moderator_par] = widget
 
-            initial_value = self.get_scanned_moderator_parameter_values(moderator_par)[0]
+            initial_value = self.get_scanned_moderator_parameter_values(moderator_par)[current_index]
             unit = self.get_scanned_moderator_parameter_unit(moderator_par)
             if unit is not None:
                 value_string = str(initial_value) + " [" + str(unit) + "]"
             else:
                 value_string = str(initial_value)
             widget_label = widgets.Label(value=value_string)
             moderator_labels.append(widget_label)
@@ -348,15 +363,15 @@
         self.sample_scan_labels = None
         self.moderator_scan_labels = None
 
     def get_monitor_list(self):
         # Overwrite get_monitor_list to only allow 1D monitors
         shape = self.scan_overview.get_shape()
         indicies = tuple(self.list_indicies)
-        guide = self.guide_names[0]
+        guide = self.guides_with_at_least_one_run[0]
         moderator = self.get_moderator_list()[0]
 
         runs = self.scan_overview.data[guide][indicies][moderator].runs
 
         return runs[self.run_name].get_1D_monitor_list()
 
     def get_plot_data(self):
@@ -452,15 +467,15 @@
         self.dropdown_monitor = None
         self.dropdown_run_name = None
         self.dropdown_moderator = None
 
         self.sample_scan_labels = None
         self.moderator_scan_labels = None
 
-        self.selected_guide = self.get_guide_names()[0]
+        self.selected_guide = self.guides_with_at_least_one_run[0]
 
         self.scan_par = None
         self.target = None
 
         sample_scan = self.get_scanned_sample_parameters()
         if len(sample_scan) > 0:
             self.target = "sample"
@@ -478,15 +493,15 @@
             raise KeyError("Need to select a guide available in the dataset!")
 
         self.selected_guide = guide
 
     def make_guide_selector(self):
 
         widget = widgets.RadioButtons(options=self.get_guide_names(),
-                                      #description="guide choices",
+                                      value=self.selected_guide,
                                       disabled=False, indent=True)
 
         widget.observe(self.update_guide_selector, "value")
 
         return widget
 
     def update_guide_selector(self, change):
@@ -569,15 +584,15 @@
 
         self.update_plot()
 
     def get_monitor_list(self):
         # Overwrite get_monitor_list to only allow 1D monitors
         shape = self.scan_overview.get_shape()
         indicies = tuple(self.list_indicies)
-        guide = self.guide_names[0]
+        guide = self.guides_with_at_least_one_run[0]
         moderator = self.get_moderator_list()[0]
 
         runs = self.scan_overview.data[guide][indicies][moderator].runs
 
         return runs[self.run_name].get_1D_monitor_list()
 
     def get_plot_data(self):
@@ -690,28 +705,28 @@
         self.dropdown_monitor = None
         self.dropdown_run_name = None
         self.dropdown_moderator = None
 
         self.sample_scan_labels = None
         self.moderator_scan_labels = None
 
-        self.selected_guide = self.get_guide_names()[0]
+        self.selected_guide = self.guides_with_at_least_one_run[0]
 
 
     def set_guide(self, guide):
 
         if guide not in self.get_guide_names():
             raise KeyError("Need to select a guide available in the dataset!")
 
         self.selected_guide = guide
 
     def make_guide_selector(self):
 
         widget = widgets.RadioButtons(options=self.get_guide_names(),
-                                      #description="guide choices",
+                                      value=self.selected_guide,
                                       disabled=False, indent=True)
 
         widget.observe(self.update_guide_selector, "value")
 
         return widget
 
     def update_guide_selector(self, change):
```

### Comparing `guide_bot-0.0.8/guide_bot/scan_visualization/overview.py` & `guide_bot-0.0.9/guide_bot/scan_visualization/overview.py`

 * *Files 5% similar despite different names*

```diff
@@ -317,14 +317,16 @@
         self.moderator_list = []
         self.moderator_list.append(self.overview["moderator"]["moderator_name"])
         self.moderator_list += self.overview["analysis_moderators"]
 
         self.guide_status = {}
         self.data = {}
 
+        self.succesful_indices = {}
+
     def get_guide_names(self):
         return self.overview["guide_names"]
 
     def get_moderators(self):
         return self.moderator_list
 
     def get_shape(self):
@@ -345,14 +347,21 @@
     def get_scanned_sample_unit(self, par):
         if self.sample_scan_units is not None:
             if par in self.sample_scan_units:
                 return self.sample_scan_units[par]
 
         return None
 
+    def get_global_index_from_sample_index(self, index):
+        return index
+
+    def get_global_index_from_sample_parameter(self, parameter):
+        index = self.get_scanned_sample_parameters().index(parameter)
+        return self.get_global_index_from_sample_index(index)
+
     def get_scanned_moderator_parameters(self):
         return self.scan_list_moderator
 
     def get_par_index_moderator(self, parameter):
         if parameter not in self.scan_list_moderator:
             raise KeyError("Parameter name not found in moderator scan list")
 
@@ -364,14 +373,21 @@
     def get_scanned_moderator_unit(self, par):
         if self.moderator_scan_units is not None:
             if par in self.moderator_scan_units:
                 return self.moderator_scan_units[par]
 
         return None
 
+    def get_global_index_from_moderator_index(self, index):
+        return index + self.scan_list_cut
+
+    def get_global_index_from_moderator_parameter(self, parameter):
+        index = self.get_scanned_moderator_parameters().index(parameter)
+        return self.get_global_index_from_moderator_index(index)
+
     def get_n_scanned_parameters(self):
         return self.total_scan_pars
 
     def get_scanned_parameters(self):
         return self.scan_list
 
     def get_type_from_index(self, index):
@@ -494,21 +510,28 @@
             try:
                 state = next(scan)
             except StopIteration:
                 break
 
             self.data[guide][state] = {}
 
+            any_success = False
             for mod in self.moderator_list:
                 path = self.get_data_location(guide, state, analysis_moderator=mod)
 
                 if self.path_is_data_directory(path):
                     self.data[guide][state][mod] = SourceAnalysis(path)
+                    any_success = True
                 else:
                     self.data[guide][state][mod] = None
 
+            if any_success:
+                if guide not in self.succesful_indices:
+                    self.succesful_indices[guide] = []
+                self.succesful_indices[guide].append(state)
+
     def load_run_information(self):
         for guide in self.get_guide_names():
             self.load_guide_run_information(guide)
```

### Comparing `guide_bot-0.0.8/guide_bot/tests/short_requirement_parameters.py` & `guide_bot-0.0.9/guide_bot/tests/short_requirement_parameters.py`

 * *Files identical despite different names*

### Comparing `guide_bot-0.0.8/guide_bot/tests/test_Constraints.py` & `guide_bot-0.0.9/guide_bot/tests/test_Constraints.py`

 * *Files identical despite different names*

### Comparing `guide_bot-0.0.8/guide_bot/tests/test_guide_elements.py` & `guide_bot-0.0.9/guide_bot/tests/test_guide_elements.py`

 * *Files identical despite different names*

### Comparing `guide_bot-0.0.8/guide_bot/tests/test_instrument_parameter_container.py` & `guide_bot-0.0.9/guide_bot/tests/test_instrument_parameter_container.py`

 * *Files identical despite different names*

### Comparing `guide_bot-0.0.8/guide_bot/tests/test_instrument_parameters.py` & `guide_bot-0.0.9/guide_bot/tests/test_instrument_parameters.py`

 * *Files identical despite different names*

### Comparing `guide_bot-0.0.8/guide_bot/tests/test_requirement_parameters.py` & `guide_bot-0.0.9/guide_bot/tests/test_requirement_parameters.py`

 * *Files identical despite different names*

### Comparing `guide_bot-0.0.8/guide_bot.egg-info/PKG-INFO` & `guide_bot-0.0.9/guide_bot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guide-bot
-Version: 0.0.8
+Version: 0.0.9
 Summary: Neutron guide optimization package
 Home-page: https://git.esss.dk/highness/guide_bot
 Author: Mads Bertelsen
 Author-email: Mads.Bertelsen@ess.eu
 License: UNKNOWN
 Description: # Early version of guide_bot in python
         
@@ -232,15 +232,15 @@
         ```
         The run_status method shows the status of all runs, check if any failed.
         
         After the scan_overview have loaded the data, its possible to visualize with 4 different widgets:
         
         - PlotAnyMonitor: Plots any single monitor
         - CompareMonitors: Compare 1D monitors for any number of guides
-        - CompareMonitorsScans: Compare 1D monitors over a scan
+        - CompareMonitorsScan: Compare 1D monitors over a scan
         - PlotSum: Shows sum of any monitor as function of scan
         
         They are all displayed with the same setup, for example here with PlotAnyMonitor as example
         ```
         scan_interface = jb_interface.PlotSum(scan_overview)
         scan_interface.show_interface()
         ```
```

### Comparing `guide_bot-0.0.8/guide_bot.egg-info/SOURCES.txt` & `guide_bot-0.0.9/guide_bot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `guide_bot-0.0.8/setup.py` & `guide_bot-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='guide_bot',
-    version='0.0.8',
+    version='0.0.9',
     author="Mads Bertelsen",
     author_email="Mads.Bertelsen@ess.eu",
     description="Neutron guide optimization package",
     include_package_data=True,
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://git.esss.dk/highness/guide_bot",
```

