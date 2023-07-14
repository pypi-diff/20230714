# Comparing `tmp/scientific_plots-1.7.0.tar.gz` & `tmp/scientific_plots-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scientific_plots-1.7.0.tar", last modified: Wed Jul 12 15:55:48 2023, max compression
+gzip compressed data, was "scientific_plots-1.7.1.tar", last modified: Fri Jul 14 13:44:17 2023, max compression
```

## Comparing `scientific_plots-1.7.0.tar` & `scientific_plots-1.7.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:55:48.619552 scientific_plots-1.7.0/
--rw-rw-rw-   0 root         (0) root         (0)     7652 2023-06-25 08:00:18.000000 scientific_plots-1.7.0/COPYING.LESSER
--rw-r--r--   0 root         (0) root         (0)    11607 2023-07-12 15:55:48.619552 scientific_plots-1.7.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1683 2023-06-25 08:15:40.000000 scientific_plots-1.7.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     2103 2023-06-23 08:33:51.000000 scientific_plots-1.7.0/readme.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 15:55:48.619552 scientific_plots-1.7.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:55:48.611552 scientific_plots-1.7.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:55:48.611552 scientific_plots-1.7.0/src/cycler-stubs/
--rw-rw-rw-   0 root         (0) root         (0)      713 2023-04-02 22:54:17.000000 scientific_plots-1.7.0/src/cycler-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:55:48.611552 scientific_plots-1.7.0/src/hurst-stubs/
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-04-02 22:54:17.000000 scientific_plots-1.7.0/src/hurst-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:55:48.615552 scientific_plots-1.7.0/src/matplotlib-stubs/
--rw-rw-rw-   0 root         (0) root         (0)     1580 2023-06-30 21:18:04.000000 scientific_plots-1.7.0/src/matplotlib-stubs/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      377 2023-04-02 22:54:17.000000 scientific_plots-1.7.0/src/matplotlib-stubs/animation.pyi
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-23 09:07:22.000000 scientific_plots-1.7.0/src/matplotlib-stubs/cm.pyi
--rw-rw-rw-   0 root         (0) root         (0)      757 2023-04-02 22:54:17.000000 scientific_plots-1.7.0/src/matplotlib-stubs/colors.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1464 2023-07-12 15:45:02.000000 scientific_plots-1.7.0/src/matplotlib-stubs/figure.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:55:48.615552 scientific_plots-1.7.0/src/matplotlib-stubs/pyplot/
--rw-rw-rw-   0 root         (0) root         (0)     8988 2023-07-12 15:45:02.000000 scientific_plots-1.7.0/src/matplotlib-stubs/pyplot/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      298 2023-04-02 22:54:17.000000 scientific_plots-1.7.0/src/matplotlib-stubs/pyplot/style.pyi
--rw-rw-rw-   0 root         (0) root         (0)      528 2023-06-24 21:33:21.000000 scientific_plots-1.7.0/src/matplotlib-stubs/ticker.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:55:48.615552 scientific_plots-1.7.0/src/mpl_toolkits-stubs/
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-23 09:07:22.000000 scientific_plots-1.7.0/src/mpl_toolkits-stubs/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-06-23 09:07:22.000000 scientific_plots-1.7.0/src/mpl_toolkits-stubs/mplot.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:55:48.615552 scientific_plots-1.7.0/src/numba-stubs/
--rw-rw-rw-   0 root         (0) root         (0)     1092 2023-04-02 22:54:17.000000 scientific_plots-1.7.0/src/numba-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:55:48.615552 scientific_plots-1.7.0/src/python_translator-stubs/
--rw-rw-rw-   0 root         (0) root         (0)      251 2023-04-02 22:54:17.000000 scientific_plots-1.7.0/src/python_translator-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:55:48.615552 scientific_plots-1.7.0/src/scientific_plots/
--rw-rw-rw-   0 root         (0) root         (0)      305 2023-07-11 17:08:49.000000 scientific_plots-1.7.0/src/scientific_plots/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1298 2023-04-02 22:54:17.000000 scientific_plots-1.7.0/src/scientific_plots/data_analysis.py
--rw-rw-rw-   0 root         (0) root         (0)    18907 2023-06-25 08:00:18.000000 scientific_plots-1.7.0/src/scientific_plots/default_plots.py
--rw-rw-rw-   0 root         (0) root         (0)    19709 2023-07-12 15:45:02.000000 scientific_plots-1.7.0/src/scientific_plots/plot_settings.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-12 15:55:22.000000 scientific_plots-1.7.0/src/scientific_plots/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     5485 2023-04-02 22:54:17.000000 scientific_plots-1.7.0/src/scientific_plots/two_d_plot.py
--rw-rw-rw-   0 root         (0) root         (0)      883 2023-04-02 22:54:17.000000 scientific_plots-1.7.0/src/scientific_plots/types_.py
--rw-rw-rw-   0 root         (0) root         (0)     8954 2023-06-25 09:05:46.000000 scientific_plots-1.7.0/src/scientific_plots/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:55:48.619552 scientific_plots-1.7.0/src/scientific_plots.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11607 2023-07-12 15:55:48.000000 scientific_plots-1.7.0/src/scientific_plots.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1363 2023-07-12 15:55:48.000000 scientific_plots-1.7.0/src/scientific_plots.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 15:55:48.000000 scientific_plots-1.7.0/src/scientific_plots.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      189 2023-07-12 15:55:48.000000 scientific_plots-1.7.0/src/scientific_plots.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      126 2023-07-12 15:55:48.000000 scientific_plots-1.7.0/src/scientific_plots.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:55:48.619552 scientific_plots-1.7.0/src/scipy-stubs/
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-04-02 22:54:17.000000 scientific_plots-1.7.0/src/scipy-stubs/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      615 2023-04-02 22:54:17.000000 scientific_plots-1.7.0/src/scipy-stubs/fft.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1134 2023-07-07 14:38:21.000000 scientific_plots-1.7.0/src/scipy-stubs/integrate.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3032 2023-07-07 14:38:21.000000 scientific_plots-1.7.0/src/scipy-stubs/interpolate.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1006 2023-04-02 22:54:17.000000 scientific_plots-1.7.0/src/scipy-stubs/optimize.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:55:48.619552 scientific_plots-1.7.0/src/scipy-stubs/signal/
--rw-rw-rw-   0 root         (0) root         (0)     1022 2023-04-02 22:54:17.000000 scientific_plots-1.7.0/src/scipy-stubs/signal/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      271 2023-04-02 22:54:17.000000 scientific_plots-1.7.0/src/scipy-stubs/signal/windows.pyi
--rw-rw-rw-   0 root         (0) root         (0)      373 2023-04-02 22:54:17.000000 scientific_plots-1.7.0/src/scipy-stubs/special.pyi
--rw-rw-rw-   0 root         (0) root         (0)      301 2023-04-02 22:54:17.000000 scientific_plots-1.7.0/src/scipy-stubs/stats.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:55:48.619552 scientific_plots-1.7.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2372 2023-06-22 14:06:06.000000 scientific_plots-1.7.0/tests/test_plot_manual.py
--rw-rw-rw-   0 root         (0) root         (0)     3783 2023-07-12 15:45:02.000000 scientific_plots-1.7.0/tests/test_plots.py
--rw-rw-rw-   0 root         (0) root         (0)      710 2023-04-02 22:54:17.000000 scientific_plots-1.7.0/tests/test_types.py
--rw-rw-rw-   0 root         (0) root         (0)      807 2023-04-02 22:54:17.000000 scientific_plots-1.7.0/tests/test_utilties.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 13:44:17.160221 scientific_plots-1.7.1/
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2023-06-25 08:00:18.000000 scientific_plots-1.7.1/COPYING.LESSER
+-rw-r--r--   0 root         (0) root         (0)    11607 2023-07-14 13:44:17.160221 scientific_plots-1.7.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1683 2023-06-25 08:15:40.000000 scientific_plots-1.7.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     2103 2023-06-23 08:33:51.000000 scientific_plots-1.7.1/readme.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 13:44:17.160221 scientific_plots-1.7.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 13:44:17.148221 scientific_plots-1.7.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 13:44:17.152221 scientific_plots-1.7.1/src/cycler-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)      713 2023-04-02 22:54:17.000000 scientific_plots-1.7.1/src/cycler-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 13:44:17.152221 scientific_plots-1.7.1/src/hurst-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-04-02 22:54:17.000000 scientific_plots-1.7.1/src/hurst-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 13:44:17.152221 scientific_plots-1.7.1/src/matplotlib-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)     1580 2023-06-30 21:18:04.000000 scientific_plots-1.7.1/src/matplotlib-stubs/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      377 2023-04-02 22:54:17.000000 scientific_plots-1.7.1/src/matplotlib-stubs/animation.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-23 09:07:22.000000 scientific_plots-1.7.1/src/matplotlib-stubs/cm.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      757 2023-04-02 22:54:17.000000 scientific_plots-1.7.1/src/matplotlib-stubs/colors.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1464 2023-07-12 15:45:02.000000 scientific_plots-1.7.1/src/matplotlib-stubs/figure.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 13:44:17.152221 scientific_plots-1.7.1/src/matplotlib-stubs/pyplot/
+-rw-rw-rw-   0 root         (0) root         (0)     8988 2023-07-12 15:45:02.000000 scientific_plots-1.7.1/src/matplotlib-stubs/pyplot/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      298 2023-04-02 22:54:17.000000 scientific_plots-1.7.1/src/matplotlib-stubs/pyplot/style.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      528 2023-06-24 21:33:21.000000 scientific_plots-1.7.1/src/matplotlib-stubs/ticker.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 13:44:17.152221 scientific_plots-1.7.1/src/mpl_toolkits-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-23 09:07:22.000000 scientific_plots-1.7.1/src/mpl_toolkits-stubs/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-06-23 09:07:22.000000 scientific_plots-1.7.1/src/mpl_toolkits-stubs/mplot.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 13:44:17.152221 scientific_plots-1.7.1/src/numba-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)     1092 2023-04-02 22:54:17.000000 scientific_plots-1.7.1/src/numba-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 13:44:17.152221 scientific_plots-1.7.1/src/python_translator-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)      251 2023-04-02 22:54:17.000000 scientific_plots-1.7.1/src/python_translator-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 13:44:17.156221 scientific_plots-1.7.1/src/scientific_plots/
+-rw-rw-rw-   0 root         (0) root         (0)      305 2023-07-14 12:17:58.000000 scientific_plots-1.7.1/src/scientific_plots/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1298 2023-04-02 22:54:17.000000 scientific_plots-1.7.1/src/scientific_plots/data_analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    18907 2023-06-25 08:00:18.000000 scientific_plots-1.7.1/src/scientific_plots/default_plots.py
+-rw-rw-rw-   0 root         (0) root         (0)    20586 2023-07-14 13:33:18.000000 scientific_plots-1.7.1/src/scientific_plots/plot_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-14 13:43:50.000000 scientific_plots-1.7.1/src/scientific_plots/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     5485 2023-04-02 22:54:17.000000 scientific_plots-1.7.1/src/scientific_plots/two_d_plot.py
+-rw-rw-rw-   0 root         (0) root         (0)      883 2023-04-02 22:54:17.000000 scientific_plots-1.7.1/src/scientific_plots/types_.py
+-rw-rw-rw-   0 root         (0) root         (0)     8954 2023-06-25 09:05:46.000000 scientific_plots-1.7.1/src/scientific_plots/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 13:44:17.156221 scientific_plots-1.7.1/src/scientific_plots.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11607 2023-07-14 13:44:17.000000 scientific_plots-1.7.1/src/scientific_plots.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1363 2023-07-14 13:44:17.000000 scientific_plots-1.7.1/src/scientific_plots.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 13:44:17.000000 scientific_plots-1.7.1/src/scientific_plots.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      189 2023-07-14 13:44:17.000000 scientific_plots-1.7.1/src/scientific_plots.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      126 2023-07-14 13:44:17.000000 scientific_plots-1.7.1/src/scientific_plots.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 13:44:17.156221 scientific_plots-1.7.1/src/scipy-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-04-02 22:54:17.000000 scientific_plots-1.7.1/src/scipy-stubs/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      615 2023-04-02 22:54:17.000000 scientific_plots-1.7.1/src/scipy-stubs/fft.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1134 2023-07-07 14:38:21.000000 scientific_plots-1.7.1/src/scipy-stubs/integrate.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3032 2023-07-07 14:38:21.000000 scientific_plots-1.7.1/src/scipy-stubs/interpolate.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1006 2023-04-02 22:54:17.000000 scientific_plots-1.7.1/src/scipy-stubs/optimize.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 13:44:17.156221 scientific_plots-1.7.1/src/scipy-stubs/signal/
+-rw-rw-rw-   0 root         (0) root         (0)     1022 2023-04-02 22:54:17.000000 scientific_plots-1.7.1/src/scipy-stubs/signal/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-04-02 22:54:17.000000 scientific_plots-1.7.1/src/scipy-stubs/signal/windows.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      373 2023-04-02 22:54:17.000000 scientific_plots-1.7.1/src/scipy-stubs/special.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      301 2023-04-02 22:54:17.000000 scientific_plots-1.7.1/src/scipy-stubs/stats.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 13:44:17.160221 scientific_plots-1.7.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3116 2023-07-14 13:19:44.000000 scientific_plots-1.7.1/tests/test_plot_manual.py
+-rw-rw-rw-   0 root         (0) root         (0)     3783 2023-07-12 15:45:02.000000 scientific_plots-1.7.1/tests/test_plots.py
+-rw-rw-rw-   0 root         (0) root         (0)      710 2023-04-02 22:54:17.000000 scientific_plots-1.7.1/tests/test_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      807 2023-04-02 22:54:17.000000 scientific_plots-1.7.1/tests/test_utilties.py
```

### Comparing `scientific_plots-1.7.0/COPYING.LESSER` & `scientific_plots-1.7.1/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.0/PKG-INFO` & `scientific_plots-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scientific_plots
-Version: 1.7.0
+Version: 1.7.1
 Summary: Useful methods for plots used in science
 Author-email: Felix Fischer <f.fischer@ifas.rwth-aachen.de>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scientific_plots-1.7.0/pyproject.toml` & `scientific_plots-1.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.0/readme.md` & `scientific_plots-1.7.1/readme.md`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.0/src/cycler-stubs/__init__.pyi` & `scientific_plots-1.7.1/src/cycler-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.0/src/matplotlib-stubs/__init__.pyi` & `scientific_plots-1.7.1/src/matplotlib-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.0/src/matplotlib-stubs/colors.pyi` & `scientific_plots-1.7.1/src/matplotlib-stubs/colors.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.0/src/matplotlib-stubs/figure.pyi` & `scientific_plots-1.7.1/src/matplotlib-stubs/figure.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.0/src/matplotlib-stubs/pyplot/__init__.pyi` & `scientific_plots-1.7.1/src/matplotlib-stubs/pyplot/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.0/src/matplotlib-stubs/ticker.pyi` & `scientific_plots-1.7.1/src/matplotlib-stubs/ticker.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.0/src/numba-stubs/__init__.pyi` & `scientific_plots-1.7.1/src/numba-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.0/src/scientific_plots/data_analysis.py` & `scientific_plots-1.7.1/src/scientific_plots/data_analysis.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.0/src/scientific_plots/default_plots.py` & `scientific_plots-1.7.1/src/scientific_plots/default_plots.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.0/src/scientific_plots/plot_settings.py` & `scientific_plots-1.7.1/src/scientific_plots/plot_settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from .utilities import translate
 from .types_ import Vector
 
 mpl.use("Agg")
 plt.rcParams["axes.unicode_minus"] = False
 
 SPINE_COLOR = "black"
-FIGSIZE = (4.4, 3.0)
+FIGSIZE = (3.15, 2.35)
 FIGSIZE_SMALL = (2.2, 2.1)
 _savefig = copy(plt.savefig)  # backup the old save-function
 
 
 def linestyles() -> Generator[str, None, None]:
     """get the line-stiles as an iterator"""
     yield "-"
@@ -242,15 +242,15 @@
     mpl.rcParams["text.latex.preamble"] = [
         r"\usepackage{helvet}",  # set the normal font here
         r"\usepackage{sansmath}",  # load up the sansmath so that math
         # -> helvet
         r"\sansmath",  # <- tricky! -- gotta actually tell tex to use!
     ]
     mpl.rc("font", family="sans-serif")
-    mpl.rc("text", usetex=True)
+    mpl.rc("text", usetex=False)
     font = {"size": 30}
 
     mpl.rc("font", **font)
     plt.set_cmap("rwth_list")
     try:
         yield ax
     except Exception as e:
@@ -406,28 +406,34 @@
 
 
 def set_serif() -> None:
     """Set the plot to use a style with serifs."""
     mpl.rcParams["font.family"] = "serif"
     mpl.rcParams["font.serif"] = [
         "cmr10", "stix", "Times New Roman"]
+    mpl.rcParams["mathtext.fontset"] = "cm"
 
 
 def set_sans_serif() -> None:
     """Set matplotlib to use a sans-serif font."""
     mpl.rcParams["font.family"] = "sans-serif"
     mpl.rcParams["font.sans-serif"] = [
         "Arial", "Helvetica", "DejaVu Sans"]
 
 
 class ThreeDPlotException(Exception):
     """This exception is called when a 3D plot is drawn. This is used to exit
     the plotting function with the science-style."""
 
 
+class FallBackException(Exception):
+    """This is excaption is thrown when the fallback-style is selected.
+    Only for debug purposes."""
+
+
 def check_3d(three_d: bool) -> None:
     """This function checks if the current plot is a 3d plot. In that case, an
     exception is thrown, which can be used to stop the creation of the default
     plot."""
     if three_d:
         raise ThreeDPlotException
     if isinstance(plt.gca(), mpl_toolkits.mplot3d.axes3d.Axes3D):
@@ -435,69 +441,84 @@
 
 
 PlotFunction = Callable[..., None]
 
 
 @overload
 def apply_styles(plot_function: PlotFunction, *,
-                 three_d: bool = False) -> PlotFunction:
+                 three_d: bool = False,
+                 _fallback: bool = False) -> PlotFunction:
     ...
 
 
 @overload
-def apply_styles(plot_function: None, *, three_d: bool = False)\
+def apply_styles(plot_function: None, *, three_d: bool = False,
+                 _fallback: bool = False)\
         -> Callable[[PlotFunction], PlotFunction]:
     ...
 
 
 @overload
-def apply_styles(*, three_d: bool = False)\
+def apply_styles(*, three_d: bool = False,
+                 _fallback: bool = False)\
         -> Callable[[PlotFunction], PlotFunction]:
     ...
 
 
 def apply_styles(plot_function: Optional[PlotFunction] = None, *,
-                 three_d: bool = False)\
+                 three_d: bool = False, _fallback: bool = False)\
         -> Union[Callable[[PlotFunction], PlotFunction], PlotFunction]:
-    """Apply the newly defined styles to a function, which creates a plot."""
+    """
+    Apply the newly defined styles to a function, which creates a plot.
+    The new plots are saved into different subdirectories and multiple
+    variants of every plot will be created.
+
+    Arguments
+    --------
+    three_d: Create a use this option for 3D-plots
+    fallback: switch directly to the fallback-style (for debug)
+    """
     # pylint: disable=too-many-statements
 
     def _decorator(_plot_function: PlotFunction) -> PlotFunction:
         """This is the  actual decorator. Thus, the outer function
         'apply_styles' is actually a decorator-factory."""
 
         @wraps(_plot_function)
         def new_plot_function(*args: Any, **kwargs: Any) -> None:
             """
             New plotting function, with applied styles.
             """
             # default plot
             plt.set_cmap("rwth_list")
-            plt.savefig = new_save_simple()
+            plt.savefig = new_save_simple(png=False)
             _plot_function(*args, **kwargs)
 
-            errors = (OSError, FileNotFoundError, ThreeDPlotException)
+            errors = (OSError, FileNotFoundError, ThreeDPlotException,
+                      FallBackException)
 
             def journal() -> None:
                 """Create a plot for journals."""
                 set_rwth_colors(three_d)
                 set_serif()
                 plt.savefig = new_save_simple("journal", png=False,
                                               small=not three_d)
                 _plot_function(*args, **kwargs)
+                plt.close("all")
 
             def sans_serif() -> None:
                 """
                 Create a plot for journals with sans-serif-fonts.
                 """
                 set_rwth_colors(three_d)
                 set_sans_serif()
                 plt.savefig = new_save_simple("sans_serif", german=True,
                                               small=not three_d)
                 _plot_function(*args, **kwargs)
+                plt.close("all")
 
             def grayscale() -> None:
                 """
                 Create a plot in grayscales for disserations.
                 """
                 mpl.rcParams["text.usetex"] = False
                 set_serif()
@@ -506,14 +527,15 @@
                     new_kwargs = copy(kwargs)
                     new_kwargs["colorscheme"] = "Greys"
                 else:
                     new_kwargs = kwargs
                 plt.savefig = new_save_simple("grayscale", png=False,
                                               small=not three_d)
                 _plot_function(*args, **new_kwargs)
+                plt.close("all")
 
             def presentation() -> None:
                 """
                 Create a plot for presentations.
                 """
                 if three_d:
                     new_kwargs = copy(kwargs)
@@ -524,19 +546,23 @@
                     new_kwargs = kwargs
                 set_rwth_colors(three_d)
                 presentation_settings()
                 set_sans_serif()
                 plt.savefig = new_save_simple("presentation",
                                               german=True, pdf=False)
                 _plot_function(*args, **new_kwargs)
+                plt.close("all")
 
             try:
+                plt.close("all")
+
                 check_3d(three_d)
+                if _fallback:
+                    raise FallBackException
 
-                # test if this context is available
                 plt.close("all")
 
                 # journal
                 with plt.style.context(["science", "ieee"]):
                     journal()
 
                 # sans-serif
@@ -552,33 +578,35 @@
                     presentation()
 
             except errors:
                 if not three_d:
                     warn(dedent(""""Could not found style 'science'.
                                 The package was probably installed incorrectly.
                                 Using a fallback-style."""), ImportWarning)
+
+                plt.close("all")
                 # journal
                 with plt.style.context("fast"):
                     if not three_d:
                         mpl.rcParams["figure.figsize"] = FIGSIZE
-                        mpl.rcParams["font.size"] = 10
+                        mpl.rcParams["font.size"] = 8
                     journal()
 
                 # sans-serif
                 with plt.style.context("fast"):
                     if not three_d:
                         mpl.rcParams["figure.figsize"] = FIGSIZE
-                        mpl.rcParams["font.size"] = 10
+                        mpl.rcParams["font.size"] = 8
                     sans_serif()
 
                 # grayscale
                 with plt.style.context("grayscale"):
                     if not three_d:
                         mpl.rcParams["figure.figsize"] = FIGSIZE
-                        mpl.rcParams["font.size"] = 10
+                        mpl.rcParams["font.size"] = 8
                     grayscale()
 
                 # presentation
                 with plt.style.context("fast"):
                     presentation()
 
             plt.savefig = old_save
```

### Comparing `scientific_plots-1.7.0/src/scientific_plots/two_d_plot.py` & `scientific_plots-1.7.1/src/scientific_plots/two_d_plot.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.0/src/scientific_plots/types_.py` & `scientific_plots-1.7.1/src/scientific_plots/types_.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.0/src/scientific_plots/utilities.py` & `scientific_plots-1.7.1/src/scientific_plots/utilities.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.0/src/scientific_plots.egg-info/PKG-INFO` & `scientific_plots-1.7.1/src/scientific_plots.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scientific-plots
-Version: 1.7.0
+Version: 1.7.1
 Summary: Useful methods for plots used in science
 Author-email: Felix Fischer <f.fischer@ifas.rwth-aachen.de>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scientific_plots-1.7.0/src/scientific_plots.egg-info/SOURCES.txt` & `scientific_plots-1.7.1/src/scientific_plots.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.0/src/scipy-stubs/fft.pyi` & `scientific_plots-1.7.1/src/scipy-stubs/fft.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.0/src/scipy-stubs/integrate.pyi` & `scientific_plots-1.7.1/src/scipy-stubs/integrate.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.0/src/scipy-stubs/interpolate.pyi` & `scientific_plots-1.7.1/src/scipy-stubs/interpolate.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.0/src/scipy-stubs/optimize.pyi` & `scientific_plots-1.7.1/src/scipy-stubs/optimize.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.0/src/scipy-stubs/signal/__init__.pyi` & `scientific_plots-1.7.1/src/scipy-stubs/signal/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.0/tests/test_plot_manual.py` & `scientific_plots-1.7.1/tests/test_plot_manual.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 #!/usr/bin/env python3
 """
 Test the design of the created plots by eye and by hand. For this, the plots
 are placed in a persistent directory.
 """
 from pathlib import Path
 
+import matplotlib.pyplot as plt
 from pytest import mark
 from numpy import linspace, meshgrid
 from scientific_plots.default_plots import (
     two_plots, three_axis_plots, plot, plot_surface)
+from scientific_plots.plot_settings import apply_styles
 from scientific_plots.types_ import Vector
 
 
 LOCATION = Path("tests/plots/test_plot.pdf")
 LOCATION2 = Path("tests/plots/test_plot2.pdf")
 LOCATION3 = Path("tests/plots/test_plot3.pdf")
 LOCATION4 = Path("tests/plots/test_plot_surface.pdf")
+LOCATION5 = Path("tests/plots/test_plot_fallback.pdf")
 
 
 @mark.use_style
 def test_two_plots() -> None:
     """Test the creation of a twin-plot."""
     x_test: Vector = linspace(1., 100., 100)
     y_test1: Vector = x_test**2
@@ -54,15 +57,15 @@
 @mark.use_style
 def test_skip_color() -> None:
     """Test the skipping of a color in the cycle."""
     x_test: Vector = linspace(1., 2., 100)
     y_test1: Vector = x_test**2
     filename = LOCATION3
     filename.parent.mkdir(exist_ok=True)
-    plot(x_test, y_test1, "x", "y", filename, cycler=1)
+    plot(x_test, y_test1, "$x_2$", r"$\sqrt{y_c}$", filename, cycler=1)
     assert filename.exists()
 
 
 @mark.use_style
 def test_two_d_plot() -> None:
     """Test the creation of a two dimensional surface plot."""
     x_test: Vector = linspace(-10, 10, 100)
@@ -73,7 +76,31 @@
     filename = LOCATION4
     filename.parent.mkdir(exist_ok=True)
     plot_surface(
         x_test_grid, y_test_grid, z_grid,
         "x-label", "y-label", "z-label",
         LOCATION4)
     assert filename.exists()
+
+
+@mark.use_style
+def test_fallback() -> None:
+    """Test plot creation using the fallback-style."""
+    filename = LOCATION4
+    filename.parent.mkdir(exist_ok=True)
+
+    x_test: Vector = linspace(-10, 10, 100)
+    y_test = x_test**2
+
+    @apply_styles(_fallback=True)
+    def simple_plot() -> None:
+        """Create a simple plot."""
+        plt.plot(x_test, y_test, label="test")
+        plt.xlabel("$x$ [m]")
+        plt.ylabel(r"$\sqrt{y_c}$ [1/m]")
+        plt.legend()
+        plt.tight_layout()
+        plt.savefig(LOCATION5)
+
+    simple_plot()
+
+    assert filename.exists()
```

### Comparing `scientific_plots-1.7.0/tests/test_plots.py` & `scientific_plots-1.7.1/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.0/tests/test_types.py` & `scientific_plots-1.7.1/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.7.0/tests/test_utilties.py` & `scientific_plots-1.7.1/tests/test_utilties.py`

 * *Files identical despite different names*

