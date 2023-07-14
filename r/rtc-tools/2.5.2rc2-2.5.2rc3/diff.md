# Comparing `tmp/rtc-tools-2.5.2rc2.tar.gz` & `tmp/rtc-tools-2.5.2rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtc-tools-2.5.2rc2.tar", last modified: Tue Jun  6 08:39:48 2023, max compression
+gzip compressed data, was "rtc-tools-2.5.2rc3.tar", last modified: Fri Jul 14 11:16:51 2023, max compression
```

## Comparing `rtc-tools-2.5.2rc2.tar` & `rtc-tools-2.5.2rc3.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:39:48.261309 rtc-tools-2.5.2rc2/
--rw-rw-rw-   0 root         (0) root         (0)     7652 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/COPYING.LESSER
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1185 2023-06-06 08:39:48.261309 rtc-tools-2.5.2rc2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      750 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      388 2023-06-06 08:39:48.262308 rtc-tools-2.5.2rc2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2016 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:39:48.248309 rtc-tools-2.5.2rc2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:39:48.251309 rtc-tools-2.5.2rc2/src/rtc_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1185 2023-06-06 08:39:48.000000 rtc-tools-2.5.2rc2/src/rtc_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2071 2023-06-06 08:39:48.000000 rtc-tools-2.5.2rc2/src/rtc_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 08:39:48.000000 rtc-tools-2.5.2rc2/src/rtc_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      151 2023-06-06 08:39:48.000000 rtc-tools-2.5.2rc2/src/rtc_tools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      130 2023-06-06 08:39:48.000000 rtc-tools-2.5.2rc2/src/rtc_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-06 08:39:48.000000 rtc-tools-2.5.2rc2/src/rtc_tools.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:39:48.262308 rtc-tools-2.5.2rc2/src/rtctools/
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:39:48.253309 rtc-tools-2.5.2rc2/src/rtctools/_internal/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/_internal/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5336 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/_internal/alias_tools.py
--rw-rw-rw-   0 root         (0) root         (0)      903 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/_internal/caching.py
--rw-rw-rw-   0 root         (0) root         (0)     2243 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/_internal/casadi_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     1084 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/_internal/debug_check_helpers.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-06-06 08:39:48.262308 rtc-tools-2.5.2rc2/src/rtctools/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:39:48.255308 rtc-tools-2.5.2rc2/src/rtctools/data/
--rw-rw-rw-   0 root         (0) root         (0)      157 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4947 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/data/csv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:39:48.255308 rtc-tools-2.5.2rc2/src/rtctools/data/interpolation/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/data/interpolation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      958 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/data/interpolation/bspline.py
--rw-rw-rw-   0 root         (0) root         (0)     5985 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/data/interpolation/bspline1d.py
--rw-rw-rw-   0 root         (0) root         (0)     1607 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/data/interpolation/bspline2d.py
--rw-rw-rw-   0 root         (0) root         (0)    18692 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/data/netcdf.py
--rw-rw-rw-   0 root         (0) root         (0)    43530 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/data/pi.py
--rw-rw-rw-   0 root         (0) root         (0)     8853 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/data/rtc.py
--rw-rw-rw-   0 root         (0) root         (0)    13011 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/data/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:39:48.260309 rtc-tools-2.5.2rc2/src/rtctools/optimization/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/optimization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   117456 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/optimization/collocated_integrated_optimization_problem.py
--rw-rw-rw-   0 root         (0) root         (0)     9026 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/optimization/control_tree_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    16651 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/optimization/csv_lookup_table_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    11624 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/optimization/csv_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    31608 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/optimization/goal_programming_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    41999 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/optimization/goal_programming_mixin_base.py
--rw-rw-rw-   0 root         (0) root         (0)     6782 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/optimization/homotopy_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     3126 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/optimization/initial_state_estimation_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    12558 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/optimization/io_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     1019 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/optimization/linearization_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     8736 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/optimization/linearized_order_goal_programming_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    13293 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/optimization/min_abs_goal_programming_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    16198 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/optimization/modelica_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     7259 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/optimization/netcdf_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    43494 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/optimization/optimization_problem.py
--rw-rw-rw-   0 root         (0) root         (0)    10783 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/optimization/pi_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    25126 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/optimization/single_pass_goal_programming_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     1753 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/optimization/timeseries.py
--rw-rw-rw-   0 root         (0) root         (0)     4193 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/rtctoolsapp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 08:39:48.261309 rtc-tools-2.5.2rc2/src/rtctools/simulation/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/simulation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6606 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/simulation/csv_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     6163 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/simulation/io_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     8922 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/simulation/pi_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    35419 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/simulation/simulation_problem.py
--rw-rw-rw-   0 root         (0) root         (0)     8905 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/src/rtctools/util.py
--rw-rw-rw-   0 root         (0) root         (0)    68611 2023-06-06 08:39:43.000000 rtc-tools-2.5.2rc2/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:16:51.032525 rtc-tools-2.5.2rc3/
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/COPYING.LESSER
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1185 2023-07-14 11:16:51.032525 rtc-tools-2.5.2rc3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      750 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      388 2023-07-14 11:16:51.033525 rtc-tools-2.5.2rc3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2016 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:16:51.022525 rtc-tools-2.5.2rc3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:16:51.024525 rtc-tools-2.5.2rc3/src/rtc_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1185 2023-07-14 11:16:51.000000 rtc-tools-2.5.2rc3/src/rtc_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2071 2023-07-14 11:16:51.000000 rtc-tools-2.5.2rc3/src/rtc_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 11:16:51.000000 rtc-tools-2.5.2rc3/src/rtc_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      151 2023-07-14 11:16:51.000000 rtc-tools-2.5.2rc3/src/rtc_tools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      130 2023-07-14 11:16:51.000000 rtc-tools-2.5.2rc3/src/rtc_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-14 11:16:51.000000 rtc-tools-2.5.2rc3/src/rtc_tools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:16:51.033525 rtc-tools-2.5.2rc3/src/rtctools/
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:16:51.026525 rtc-tools-2.5.2rc3/src/rtctools/_internal/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/_internal/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5336 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/_internal/alias_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)      903 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/_internal/caching.py
+-rw-rw-rw-   0 root         (0) root         (0)     2243 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/_internal/casadi_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1084 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/_internal/debug_check_helpers.py
+-rw-r--r--   0 root         (0) root         (0)      500 2023-07-14 11:16:51.033525 rtc-tools-2.5.2rc3/src/rtctools/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:16:51.027525 rtc-tools-2.5.2rc3/src/rtctools/data/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4947 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/data/csv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:16:51.028525 rtc-tools-2.5.2rc3/src/rtctools/data/interpolation/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/data/interpolation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      958 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/data/interpolation/bspline.py
+-rw-rw-rw-   0 root         (0) root         (0)     5985 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/data/interpolation/bspline1d.py
+-rw-rw-rw-   0 root         (0) root         (0)     1607 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/data/interpolation/bspline2d.py
+-rw-rw-rw-   0 root         (0) root         (0)    18692 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/data/netcdf.py
+-rw-rw-rw-   0 root         (0) root         (0)    43530 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/data/pi.py
+-rw-rw-rw-   0 root         (0) root         (0)     8853 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/data/rtc.py
+-rw-rw-rw-   0 root         (0) root         (0)    13011 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/data/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:16:51.031525 rtc-tools-2.5.2rc3/src/rtctools/optimization/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/optimization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   117456 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/optimization/collocated_integrated_optimization_problem.py
+-rw-rw-rw-   0 root         (0) root         (0)     9026 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/optimization/control_tree_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    16651 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/optimization/csv_lookup_table_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    11624 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/optimization/csv_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    31608 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/optimization/goal_programming_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    41999 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/optimization/goal_programming_mixin_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6782 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/optimization/homotopy_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     3126 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/optimization/initial_state_estimation_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    11817 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/optimization/io_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1019 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/optimization/linearization_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     8736 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/optimization/linearized_order_goal_programming_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    13293 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/optimization/min_abs_goal_programming_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    16198 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/optimization/modelica_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     7259 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/optimization/netcdf_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    43624 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/optimization/optimization_problem.py
+-rw-rw-rw-   0 root         (0) root         (0)    10783 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/optimization/pi_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    25126 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/optimization/single_pass_goal_programming_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1753 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/optimization/timeseries.py
+-rw-rw-rw-   0 root         (0) root         (0)     4193 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/rtctoolsapp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 11:16:51.032525 rtc-tools-2.5.2rc3/src/rtctools/simulation/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/simulation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6606 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/simulation/csv_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     6163 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/simulation/io_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     8922 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/simulation/pi_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    35419 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/simulation/simulation_problem.py
+-rw-rw-rw-   0 root         (0) root         (0)     8905 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/src/rtctools/util.py
+-rw-rw-rw-   0 root         (0) root         (0)    68611 2023-07-14 11:16:46.000000 rtc-tools-2.5.2rc3/versioneer.py
```

### Comparing `rtc-tools-2.5.2rc2/COPYING.LESSER` & `rtc-tools-2.5.2rc3/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2rc2/PKG-INFO` & `rtc-tools-2.5.2rc3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtc-tools
-Version: 2.5.2rc2
+Version: 2.5.2rc3
 Summary: Toolbox for control and optimization of water systems.
 Home-page: https://oss.deltares.nl/web/rtc-tools/home
 Author: Deltares
 Maintainer: Deltares
 License: UNKNOWN
 Download-URL: http://gitlab.com/deltares/rtc-tools/
 Platform: Windows
```

### Comparing `rtc-tools-2.5.2rc2/README.md` & `rtc-tools-2.5.2rc3/README.md`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2rc2/setup.py` & `rtc-tools-2.5.2rc3/setup.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2rc2/src/rtc_tools.egg-info/PKG-INFO` & `rtc-tools-2.5.2rc3/src/rtc_tools.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtc-tools
-Version: 2.5.2rc2
+Version: 2.5.2rc3
 Summary: Toolbox for control and optimization of water systems.
 Home-page: https://oss.deltares.nl/web/rtc-tools/home
 Author: Deltares
 Maintainer: Deltares
 License: UNKNOWN
 Download-URL: http://gitlab.com/deltares/rtc-tools/
 Platform: Windows
```

### Comparing `rtc-tools-2.5.2rc2/src/rtc_tools.egg-info/SOURCES.txt` & `rtc-tools-2.5.2rc3/src/rtc_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2rc2/src/rtctools/_internal/alias_tools.py` & `rtc-tools-2.5.2rc3/src/rtctools/_internal/alias_tools.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2rc2/src/rtctools/_internal/caching.py` & `rtc-tools-2.5.2rc3/src/rtctools/_internal/caching.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2rc2/src/rtctools/_internal/casadi_helpers.py` & `rtc-tools-2.5.2rc3/src/rtctools/_internal/casadi_helpers.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2rc2/src/rtctools/_internal/debug_check_helpers.py` & `rtc-tools-2.5.2rc3/src/rtctools/_internal/debug_check_helpers.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2rc2/src/rtctools/data/csv.py` & `rtc-tools-2.5.2rc3/src/rtctools/data/csv.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2rc2/src/rtctools/data/interpolation/bspline.py` & `rtc-tools-2.5.2rc3/src/rtctools/data/interpolation/bspline.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2rc2/src/rtctools/data/interpolation/bspline1d.py` & `rtc-tools-2.5.2rc3/src/rtctools/data/interpolation/bspline1d.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2rc2/src/rtctools/data/interpolation/bspline2d.py` & `rtc-tools-2.5.2rc3/src/rtctools/data/interpolation/bspline2d.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2rc2/src/rtctools/data/netcdf.py` & `rtc-tools-2.5.2rc3/src/rtctools/data/netcdf.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2rc2/src/rtctools/data/pi.py` & `rtc-tools-2.5.2rc3/src/rtctools/data/pi.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2rc2/src/rtctools/data/rtc.py` & `rtc-tools-2.5.2rc3/src/rtctools/data/rtc.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2rc2/src/rtctools/data/storage.py` & `rtc-tools-2.5.2rc3/src/rtctools/data/storage.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2rc2/src/rtctools/optimization/collocated_integrated_optimization_problem.py` & `rtc-tools-2.5.2rc3/src/rtctools/optimization/collocated_integrated_optimization_problem.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2rc2/src/rtctools/optimization/control_tree_mixin.py` & `rtc-tools-2.5.2rc3/src/rtctools/optimization/control_tree_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2rc2/src/rtctools/optimization/csv_lookup_table_mixin.py` & `rtc-tools-2.5.2rc3/src/rtctools/optimization/csv_lookup_table_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2rc2/src/rtctools/optimization/csv_mixin.py` & `rtc-tools-2.5.2rc3/src/rtctools/optimization/csv_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2rc2/src/rtctools/optimization/goal_programming_mixin.py` & `rtc-tools-2.5.2rc3/src/rtctools/optimization/goal_programming_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2rc2/src/rtctools/optimization/goal_programming_mixin_base.py` & `rtc-tools-2.5.2rc3/src/rtctools/optimization/goal_programming_mixin_base.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2rc2/src/rtctools/optimization/homotopy_mixin.py` & `rtc-tools-2.5.2rc3/src/rtctools/optimization/homotopy_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2rc2/src/rtctools/optimization/initial_state_estimation_mixin.py` & `rtc-tools-2.5.2rc3/src/rtctools/optimization/initial_state_estimation_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2rc2/src/rtctools/optimization/io_mixin.py` & `rtc-tools-2.5.2rc3/src/rtctools/optimization/io_mixin.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,42 +55,23 @@
     @abstractmethod
     def write(self) -> None:
         """"
         Writes output data to files
         """
         pass
 
-    def times_from_input(self) -> np.ndarray:
-        """
-        Returns the times in seconds from the reference datetime onwards.
-
-        The times are based on the input data.
-        """
-        times_sec = self.io.times_sec
-        time_index = bisect.bisect_left(times_sec, 0.0)
-        times = times_sec[time_index:]
-        return times
-
     def times(self, variable=None) -> np.ndarray:
         """
         Returns the times in seconds from the reference datetime onwards.
 
-        The number of times is based on the number of timesteps to optimize for.
-
-        :param variable: variable name
+        :param variable:
         """
-        all_times = self.times_from_input()
-        max_number_of_times = len(all_times)
-        if self._number_of_timesteps_to_optimize is not None:
-            number_of_times = self._number_of_timesteps_to_optimize + 1
-        else:
-            number_of_times = max_number_of_times
-        number_of_times = min(number_of_times, max_number_of_times)
-        times = all_times[:number_of_times]
-        return times
+        times_sec = self.io.times_sec
+        t_idx = bisect.bisect_left(times_sec, 0.0)
+        return times_sec[t_idx:]
 
     @property
     def equidistant(self):
         return self.__equidistant
 
     @property
     def ensemble_size(self):
```

### Comparing `rtc-tools-2.5.2rc2/src/rtctools/optimization/linearization_mixin.py` & `rtc-tools-2.5.2rc3/src/rtctools/optimization/linearization_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2rc2/src/rtctools/optimization/linearized_order_goal_programming_mixin.py` & `rtc-tools-2.5.2rc3/src/rtctools/optimization/linearized_order_goal_programming_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2rc2/src/rtctools/optimization/min_abs_goal_programming_mixin.py` & `rtc-tools-2.5.2rc3/src/rtctools/optimization/min_abs_goal_programming_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2rc2/src/rtctools/optimization/modelica_mixin.py` & `rtc-tools-2.5.2rc3/src/rtctools/optimization/modelica_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2rc2/src/rtctools/optimization/netcdf_mixin.py` & `rtc-tools-2.5.2rc3/src/rtctools/optimization/netcdf_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2rc2/src/rtctools/optimization/optimization_problem.py` & `rtc-tools-2.5.2rc3/src/rtctools/optimization/optimization_problem.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,17 +40,14 @@
 
 
 class OptimizationProblem(DataStoreAccessor, metaclass=ABCMeta):
     """
     Base class for all optimization problems.
     """
 
-    # Number of time steps to optimize for. If None, optimize for all timesteps.
-    _number_of_timesteps_to_optimize = None
-    # Options for debug checks.
     _debug_check_level = DebugLevel.MEDIUM
     _debug_check_options = {}
 
     def __init__(self, **kwargs):
         # Call parent class first for default behaviour.
         super().__init__(**kwargs)
 
@@ -150,14 +147,18 @@
         logger.info("Calling solver")
 
         results = solver(x0=x0, lbx=lbx, ubx=ubx, lbg=ca.veccat(*lbg), ubg=ca.veccat(*ubg))
 
         # Extract relevant stats
         self.__objective_value = float(results['f'])
         self.__solver_output = np.array(results['x']).ravel()
+        self.__transcribed_problem = {"lbx": lbx, "ubx": ubx, "lbg": lbg, "ubg": ubg, "x0": x0, "nlp": nlp}
+        self.__lam_g = results.get("lam_g")
+        self.__lam_x = results.get("lam_x")
+
         self.__solver_stats = solver.stats()
 
         success, log_level = self.solver_success(self.__solver_stats, log_solver_failure_as_error)
 
         return_status = self.__solver_stats['return_status']
         if 'secondary_return_status' in self.__solver_stats:
             return_status = "{}: {}".format(return_status, self.__solver_stats['secondary_return_status'])
@@ -195,21 +196,14 @@
                 'Skipping Postprocessing in OptimizationProblem.optimize()')
 
         # Done
         logger.info("Done with optimize()")
 
         return success
 
-    @classmethod
-    def set_number_of_timesteps_to_optimize(cls, number_of_timesteps_to_optimize):
-        """
-        Set the number of timesteps for which to optimize.
-        """
-        cls._number_of_timesteps_to_optimize = number_of_timesteps_to_optimize
-
     def __check_bounds_control_input(self) -> None:
         # Checks if at the control inputs have bounds, log warning when a control input is not bounded.
         bounds = self.bounds()
 
         for variable in self.dae_variables['control_inputs']:
             variable = variable.name()
             if variable not in bounds:
@@ -329,14 +323,28 @@
     @property
     def solver_stats(self) -> Dict[str, Any]:
         """
         The stats from the last NLP solver run.
         """
         return self.__solver_stats
 
+    @property
+    def lagrange_multipliers(self) -> Tuple[Any, Any]:
+        """
+        The lagrange multipliers at the solution.
+        """
+        return self.__lam_g, self.__lam_x
+
+    @property
+    def transcribed_problem(self) -> Dict[str, Any]:
+        """
+        The transcribed problem.
+        """
+        return self.__transcribed_problem
+
     def pre(self) -> None:
         """
         Preprocessing logic is performed here.
         """
         pass
 
     @abstractproperty
```

### Comparing `rtc-tools-2.5.2rc2/src/rtctools/optimization/pi_mixin.py` & `rtc-tools-2.5.2rc3/src/rtctools/optimization/pi_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2rc2/src/rtctools/optimization/single_pass_goal_programming_mixin.py` & `rtc-tools-2.5.2rc3/src/rtctools/optimization/single_pass_goal_programming_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2rc2/src/rtctools/optimization/timeseries.py` & `rtc-tools-2.5.2rc3/src/rtctools/optimization/timeseries.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2rc2/src/rtctools/rtctoolsapp.py` & `rtc-tools-2.5.2rc3/src/rtctools/rtctoolsapp.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2rc2/src/rtctools/simulation/csv_mixin.py` & `rtc-tools-2.5.2rc3/src/rtctools/simulation/csv_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2rc2/src/rtctools/simulation/io_mixin.py` & `rtc-tools-2.5.2rc3/src/rtctools/simulation/io_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2rc2/src/rtctools/simulation/pi_mixin.py` & `rtc-tools-2.5.2rc3/src/rtctools/simulation/pi_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2rc2/src/rtctools/simulation/simulation_problem.py` & `rtc-tools-2.5.2rc3/src/rtctools/simulation/simulation_problem.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2rc2/src/rtctools/util.py` & `rtc-tools-2.5.2rc3/src/rtctools/util.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2rc2/versioneer.py` & `rtc-tools-2.5.2rc3/versioneer.py`

 * *Files identical despite different names*

