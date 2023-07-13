# Comparing `tmp/pegasusio-0.8.0.tar.gz` & `tmp/pegasusio-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pegasusio-0.8.0.tar", last modified: Wed Feb  8 07:39:47 2023, max compression
+gzip compressed data, was "pegasusio-0.8.1.tar", last modified: Thu Jul 13 22:31:29 2023, max compression
```

## Comparing `pegasusio-0.8.0.tar` & `pegasusio-0.8.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-02-08 07:39:47.614255 pegasusio-0.8.0/
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-02-08 07:39:47.581286 pegasusio-0.8.0/.github/
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-02-08 07:39:47.584838 pegasusio-0.8.0/.github/workflows/
--rw-r--r--   0 yangy197   (501) staff       (20)     1281 2022-05-18 21:24:30.000000 pegasusio-0.8.0/.github/workflows/ci-test.yml
--rw-r--r--   0 yangy197   (501) staff       (20)     1515 2022-03-11 05:10:26.000000 pegasusio-0.8.0/LICENSE
--rw-r--r--   0 yangy197   (501) staff       (20)      178 2022-03-11 05:10:26.000000 pegasusio-0.8.0/MANIFEST.in
--rw-r--r--   0 yangy197   (501) staff       (20)     2391 2023-02-08 07:39:47.613942 pegasusio-0.8.0/PKG-INFO
--rw-r--r--   0 yangy197   (501) staff       (20)     1260 2022-05-18 21:24:30.000000 pegasusio-0.8.0/README.rst
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-02-08 07:39:47.592820 pegasusio-0.8.0/ext_modules/
--rw-r--r--   0 yangy197   (501) staff       (20)   868155 2023-02-08 07:39:46.000000 pegasusio-0.8.0/ext_modules/fast_funcs.c
--rw-r--r--   0 yangy197   (501) staff       (20)     2710 2023-02-08 07:30:28.000000 pegasusio-0.8.0/ext_modules/fast_funcs.pyx
--rw-r--r--   0 yangy197   (501) staff       (20)  1955517 2022-12-15 07:29:55.000000 pegasusio-0.8.0/ext_modules/io_funcs.c
--rw-r--r--   0 yangy197   (501) staff       (20)    19047 2022-07-05 17:51:08.000000 pegasusio-0.8.0/ext_modules/io_funcs.pyx
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-02-08 07:39:47.608434 pegasusio-0.8.0/pegasusio/
--rw-r--r--   0 yangy197   (501) staff       (20)     1337 2022-03-11 05:10:26.000000 pegasusio-0.8.0/pegasusio/__init__.py
--rw-r--r--   0 yangy197   (501) staff       (20)     1221 2022-03-11 05:10:26.000000 pegasusio-0.8.0/pegasusio/__main__.py
--rw-r--r--   0 yangy197   (501) staff       (20)     9347 2023-02-08 07:30:28.000000 pegasusio-0.8.0/pegasusio/aggr_data.py
--rw-r--r--   0 yangy197   (501) staff       (20)     4906 2022-07-16 18:23:29.000000 pegasusio-0.8.0/pegasusio/citeseq_data.py
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-02-08 07:39:47.612920 pegasusio-0.8.0/pegasusio/commands/
--rw-r--r--   0 yangy197   (501) staff       (20)     5127 2022-03-11 05:10:26.000000 pegasusio-0.8.0/pegasusio/commands/AggregateMatrix.py
--rw-r--r--   0 yangy197   (501) staff       (20)      624 2022-03-11 05:10:26.000000 pegasusio-0.8.0/pegasusio/commands/Base.py
--rw-r--r--   0 yangy197   (501) staff       (20)       65 2022-03-11 05:10:26.000000 pegasusio-0.8.0/pegasusio/commands/__init__.py
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-02-08 07:39:47.613325 pegasusio-0.8.0/pegasusio/cylib/
--rw-r--r--   0 yangy197   (501) staff       (20)       48 2022-03-11 05:10:26.000000 pegasusio-0.8.0/pegasusio/cylib/README.rst
--rw-r--r--   0 yangy197   (501) staff       (20)     4647 2022-03-11 05:10:26.000000 pegasusio-0.8.0/pegasusio/cyto_data.py
--rw-r--r--   0 yangy197   (501) staff       (20)     1277 2022-03-11 05:10:26.000000 pegasusio-0.8.0/pegasusio/cyto_utils.py
--rw-r--r--   0 yangy197   (501) staff       (20)    12028 2022-05-18 21:24:30.000000 pegasusio-0.8.0/pegasusio/data_aggregation.py
--rw-r--r--   0 yangy197   (501) staff       (20)     3709 2022-03-11 05:10:26.000000 pegasusio-0.8.0/pegasusio/datadict.py
--rw-r--r--   0 yangy197   (501) staff       (20)      755 2022-03-11 05:10:26.000000 pegasusio-0.8.0/pegasusio/decorators.py
--rw-r--r--   0 yangy197   (501) staff       (20)    14596 2022-07-16 18:23:29.000000 pegasusio-0.8.0/pegasusio/hdf5_utils.py
--rw-r--r--   0 yangy197   (501) staff       (20)    24650 2022-03-11 05:10:26.000000 pegasusio-0.8.0/pegasusio/multimodal_data.py
--rw-r--r--   0 yangy197   (501) staff       (20)     3618 2022-03-11 05:10:26.000000 pegasusio-0.8.0/pegasusio/nanostring_data.py
--rw-r--r--   0 yangy197   (501) staff       (20)     5557 2022-03-11 05:10:26.000000 pegasusio-0.8.0/pegasusio/nanostring_utils.py
--rw-r--r--   0 yangy197   (501) staff       (20)     7380 2022-07-17 05:38:56.000000 pegasusio-0.8.0/pegasusio/qc_utils.py
--rw-r--r--   0 yangy197   (501) staff       (20)    10870 2022-12-13 21:19:51.000000 pegasusio-0.8.0/pegasusio/readwrite.py
--rw-r--r--   0 yangy197   (501) staff       (20)     1922 2022-03-11 05:10:26.000000 pegasusio-0.8.0/pegasusio/spatial_data.py
--rw-r--r--   0 yangy197   (501) staff       (20)     4156 2022-12-13 21:11:39.000000 pegasusio-0.8.0/pegasusio/spatial_utils.py
--rw-r--r--   0 yangy197   (501) staff       (20)    23280 2023-02-08 07:30:28.000000 pegasusio-0.8.0/pegasusio/text_utils.py
--rw-r--r--   0 yangy197   (501) staff       (20)    27874 2022-08-07 20:31:31.000000 pegasusio-0.8.0/pegasusio/unimodal_data.py
--rw-r--r--   0 yangy197   (501) staff       (20)     6234 2022-03-11 05:10:26.000000 pegasusio-0.8.0/pegasusio/vdj_data.py
--rw-r--r--   0 yangy197   (501) staff       (20)     3414 2022-03-11 05:10:26.000000 pegasusio-0.8.0/pegasusio/vdj_utils.py
--rw-r--r--   0 yangy197   (501) staff       (20)      142 2023-02-08 07:39:47.000000 pegasusio-0.8.0/pegasusio/version.py
--rw-r--r--   0 yangy197   (501) staff       (20)    17284 2022-03-11 05:10:26.000000 pegasusio-0.8.0/pegasusio/views.py
--rw-r--r--   0 yangy197   (501) staff       (20)    20754 2022-05-18 21:24:30.000000 pegasusio-0.8.0/pegasusio/zarr_utils.py
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-02-08 07:39:47.611790 pegasusio-0.8.0/pegasusio.egg-info/
--rw-r--r--   0 yangy197   (501) staff       (20)     2391 2023-02-08 07:39:47.000000 pegasusio-0.8.0/pegasusio.egg-info/PKG-INFO
--rw-r--r--   0 yangy197   (501) staff       (20)     1142 2023-02-08 07:39:47.000000 pegasusio-0.8.0/pegasusio.egg-info/SOURCES.txt
--rw-r--r--   0 yangy197   (501) staff       (20)        1 2023-02-08 07:39:47.000000 pegasusio-0.8.0/pegasusio.egg-info/dependency_links.txt
--rw-r--r--   0 yangy197   (501) staff       (20)       54 2023-02-08 07:39:47.000000 pegasusio-0.8.0/pegasusio.egg-info/entry_points.txt
--rw-r--r--   0 yangy197   (501) staff       (20)        1 2022-05-12 21:04:51.000000 pegasusio-0.8.0/pegasusio.egg-info/not-zip-safe
--rw-r--r--   0 yangy197   (501) staff       (20)      149 2023-02-08 07:39:47.000000 pegasusio-0.8.0/pegasusio.egg-info/requires.txt
--rw-r--r--   0 yangy197   (501) staff       (20)       10 2023-02-08 07:39:47.000000 pegasusio-0.8.0/pegasusio.egg-info/top_level.txt
--rw-r--r--   0 yangy197   (501) staff       (20)      150 2022-03-11 05:10:26.000000 pegasusio-0.8.0/pyproject.toml
--rw-r--r--   0 yangy197   (501) staff       (20)      146 2022-05-18 21:24:30.000000 pegasusio-0.8.0/requirements.txt
--rw-r--r--   0 yangy197   (501) staff       (20)       38 2023-02-08 07:39:47.614373 pegasusio-0.8.0/setup.cfg
--rw-r--r--   0 yangy197   (501) staff       (20)     2073 2022-08-08 04:23:27.000000 pegasusio-0.8.0/setup.py
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-07-13 22:31:29.515760 pegasusio-0.8.1/
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-07-13 22:31:29.463389 pegasusio-0.8.1/.github/
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-07-13 22:31:29.467709 pegasusio-0.8.1/.github/workflows/
+-rw-r--r--   0 yangy197   (501) staff       (20)     1281 2022-05-18 21:24:30.000000 pegasusio-0.8.1/.github/workflows/ci-test.yml
+-rw-r--r--   0 yangy197   (501) staff       (20)     1515 2022-03-11 05:10:26.000000 pegasusio-0.8.1/LICENSE
+-rw-r--r--   0 yangy197   (501) staff       (20)      178 2022-03-11 05:10:26.000000 pegasusio-0.8.1/MANIFEST.in
+-rw-r--r--   0 yangy197   (501) staff       (20)     2391 2023-07-13 22:31:29.515121 pegasusio-0.8.1/PKG-INFO
+-rw-r--r--   0 yangy197   (501) staff       (20)     1260 2022-05-18 21:24:30.000000 pegasusio-0.8.1/README.rst
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-07-13 22:31:29.477816 pegasusio-0.8.1/ext_modules/
+-rw-r--r--   0 yangy197   (501) staff       (20)   868155 2023-02-08 07:39:46.000000 pegasusio-0.8.1/ext_modules/fast_funcs.c
+-rw-r--r--   0 yangy197   (501) staff       (20)     2710 2023-02-08 07:30:28.000000 pegasusio-0.8.1/ext_modules/fast_funcs.pyx
+-rw-r--r--   0 yangy197   (501) staff       (20)  1961835 2023-07-13 22:31:28.000000 pegasusio-0.8.1/ext_modules/io_funcs.c
+-rw-r--r--   0 yangy197   (501) staff       (20)    19240 2023-06-20 21:16:48.000000 pegasusio-0.8.1/ext_modules/io_funcs.pyx
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-07-13 22:31:29.502152 pegasusio-0.8.1/pegasusio/
+-rw-r--r--   0 yangy197   (501) staff       (20)     1337 2022-03-11 05:10:26.000000 pegasusio-0.8.1/pegasusio/__init__.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     1221 2022-03-11 05:10:26.000000 pegasusio-0.8.1/pegasusio/__main__.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     9347 2023-02-08 07:30:28.000000 pegasusio-0.8.1/pegasusio/aggr_data.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     4906 2022-07-16 18:23:29.000000 pegasusio-0.8.1/pegasusio/citeseq_data.py
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-07-13 22:31:29.511685 pegasusio-0.8.1/pegasusio/commands/
+-rw-r--r--   0 yangy197   (501) staff       (20)     5127 2022-03-11 05:10:26.000000 pegasusio-0.8.1/pegasusio/commands/AggregateMatrix.py
+-rw-r--r--   0 yangy197   (501) staff       (20)      624 2022-03-11 05:10:26.000000 pegasusio-0.8.1/pegasusio/commands/Base.py
+-rw-r--r--   0 yangy197   (501) staff       (20)       65 2022-03-11 05:10:26.000000 pegasusio-0.8.1/pegasusio/commands/__init__.py
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-07-13 22:31:29.513162 pegasusio-0.8.1/pegasusio/cylib/
+-rw-r--r--   0 yangy197   (501) staff       (20)       48 2022-03-11 05:10:26.000000 pegasusio-0.8.1/pegasusio/cylib/README.rst
+-rw-r--r--   0 yangy197   (501) staff       (20)     4647 2022-03-11 05:10:26.000000 pegasusio-0.8.1/pegasusio/cyto_data.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     1277 2022-03-11 05:10:26.000000 pegasusio-0.8.1/pegasusio/cyto_utils.py
+-rw-r--r--   0 yangy197   (501) staff       (20)    12028 2022-05-18 21:24:30.000000 pegasusio-0.8.1/pegasusio/data_aggregation.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     3709 2022-03-11 05:10:26.000000 pegasusio-0.8.1/pegasusio/datadict.py
+-rw-r--r--   0 yangy197   (501) staff       (20)      755 2022-03-11 05:10:26.000000 pegasusio-0.8.1/pegasusio/decorators.py
+-rw-r--r--   0 yangy197   (501) staff       (20)    14596 2022-07-16 18:23:29.000000 pegasusio-0.8.1/pegasusio/hdf5_utils.py
+-rw-r--r--   0 yangy197   (501) staff       (20)    24767 2023-06-20 21:16:48.000000 pegasusio-0.8.1/pegasusio/multimodal_data.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     3618 2022-03-11 05:10:26.000000 pegasusio-0.8.1/pegasusio/nanostring_data.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     5557 2022-03-11 05:10:26.000000 pegasusio-0.8.1/pegasusio/nanostring_utils.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     7380 2022-07-17 05:38:56.000000 pegasusio-0.8.1/pegasusio/qc_utils.py
+-rw-r--r--   0 yangy197   (501) staff       (20)    10870 2022-12-13 21:19:51.000000 pegasusio-0.8.1/pegasusio/readwrite.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     1922 2022-03-11 05:10:26.000000 pegasusio-0.8.1/pegasusio/spatial_data.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     4156 2022-12-13 21:11:39.000000 pegasusio-0.8.1/pegasusio/spatial_utils.py
+-rw-r--r--   0 yangy197   (501) staff       (20)    23515 2023-06-20 21:16:48.000000 pegasusio-0.8.1/pegasusio/text_utils.py
+-rw-r--r--   0 yangy197   (501) staff       (20)    27915 2023-07-13 22:25:44.000000 pegasusio-0.8.1/pegasusio/unimodal_data.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     6234 2022-03-11 05:10:26.000000 pegasusio-0.8.1/pegasusio/vdj_data.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     3414 2022-03-11 05:10:26.000000 pegasusio-0.8.1/pegasusio/vdj_utils.py
+-rw-r--r--   0 yangy197   (501) staff       (20)      142 2023-07-13 22:31:28.000000 pegasusio-0.8.1/pegasusio/version.py
+-rw-r--r--   0 yangy197   (501) staff       (20)    17284 2022-03-11 05:10:26.000000 pegasusio-0.8.1/pegasusio/views.py
+-rw-r--r--   0 yangy197   (501) staff       (20)    20760 2023-06-20 21:16:48.000000 pegasusio-0.8.1/pegasusio/zarr_utils.py
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-07-13 22:31:29.508603 pegasusio-0.8.1/pegasusio.egg-info/
+-rw-r--r--   0 yangy197   (501) staff       (20)     2391 2023-07-13 22:31:29.000000 pegasusio-0.8.1/pegasusio.egg-info/PKG-INFO
+-rw-r--r--   0 yangy197   (501) staff       (20)     1142 2023-07-13 22:31:29.000000 pegasusio-0.8.1/pegasusio.egg-info/SOURCES.txt
+-rw-r--r--   0 yangy197   (501) staff       (20)        1 2023-07-13 22:31:29.000000 pegasusio-0.8.1/pegasusio.egg-info/dependency_links.txt
+-rw-r--r--   0 yangy197   (501) staff       (20)       54 2023-07-13 22:31:29.000000 pegasusio-0.8.1/pegasusio.egg-info/entry_points.txt
+-rw-r--r--   0 yangy197   (501) staff       (20)        1 2022-05-12 21:04:51.000000 pegasusio-0.8.1/pegasusio.egg-info/not-zip-safe
+-rw-r--r--   0 yangy197   (501) staff       (20)      149 2023-07-13 22:31:29.000000 pegasusio-0.8.1/pegasusio.egg-info/requires.txt
+-rw-r--r--   0 yangy197   (501) staff       (20)       10 2023-07-13 22:31:29.000000 pegasusio-0.8.1/pegasusio.egg-info/top_level.txt
+-rw-r--r--   0 yangy197   (501) staff       (20)      150 2022-03-11 05:10:26.000000 pegasusio-0.8.1/pyproject.toml
+-rw-r--r--   0 yangy197   (501) staff       (20)      146 2022-05-18 21:24:30.000000 pegasusio-0.8.1/requirements.txt
+-rw-r--r--   0 yangy197   (501) staff       (20)       38 2023-07-13 22:31:29.515986 pegasusio-0.8.1/setup.cfg
+-rw-r--r--   0 yangy197   (501) staff       (20)     2073 2022-08-08 04:23:27.000000 pegasusio-0.8.1/setup.py
```

### Comparing `pegasusio-0.8.0/.github/workflows/ci-test.yml` & `pegasusio-0.8.1/.github/workflows/ci-test.yml`

 * *Files identical despite different names*

### Comparing `pegasusio-0.8.0/LICENSE` & `pegasusio-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pegasusio-0.8.0/PKG-INFO` & `pegasusio-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pegasusio
-Version: 0.8.0
+Version: 0.8.1
 Summary: Pegasusio is a Python package for reading / writing single-cell genomics data
 Home-page: https://github.com/lilab-bcb/pegasusio
 Author: Yiming Yang, Rimte Rocher, Joshua Gould and Bo Li
 Author-email: cumulus-support@googlegroups.com
 Keywords: single cell/nucleus genomics data reading and writing
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Jupyter
```

### Comparing `pegasusio-0.8.0/README.rst` & `pegasusio-0.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `pegasusio-0.8.0/ext_modules/fast_funcs.c` & `pegasusio-0.8.1/ext_modules/fast_funcs.c`

 * *Files identical despite different names*

### Comparing `pegasusio-0.8.0/ext_modules/fast_funcs.pyx` & `pegasusio-0.8.1/ext_modules/fast_funcs.pyx`

 * *Files identical despite different names*

### Comparing `pegasusio-0.8.0/ext_modules/io_funcs.c` & `pegasusio-0.8.1/ext_modules/io_funcs.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.33 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "name": "pegasusio.cylib.io",
         "sources": [
@@ -18,16 +18,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_33"
+#define CYTHON_HEX_VERSION 0x001D21F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -96,15 +96,15 @@
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -561,35 +561,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -1191,15 +1191,15 @@
   int precision;
 };
 struct __pyx_fuse_3_1_1__pyx_opt_args_9pegasusio_5cylib_2io_write_mtx {
   int __pyx_n;
   int precision;
 };
 
-/* "ext_modules/io_funcs.pyx":197
+/* "ext_modules/io_funcs.pyx":201
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef void write_dense(char* output_file, str[:] barcodes, str[:] features, data_type[:] data, indices_type[:] indices, indptr_type[:] indptr, int M, int N, int precision = 2):             # <<<<<<<<<<<<<<
  *     """ Input must be csr_matrix internal representation, gene by cell (X.T.tocsr()); Output will be gene by cell
  *     """
  */
 struct __pyx_fuse_0_0_0__pyx_opt_args_9pegasusio_5cylib_2io_write_dense {
@@ -1582,26 +1582,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1796,14 +1796,31 @@
 /* CIntToPyUnicode.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_From_int(int value, Py_ssize_t width, char padding_char, char format_char);
 
 /* JoinPyUnicode.proto */
 static PyObject* __Pyx_PyUnicode_Join(PyObject* value_tuple, Py_ssize_t value_count, Py_ssize_t result_ulength,
                                       Py_UCS4 max_char);
 
+/* UnpackUnboundCMethod.proto */
+typedef struct {
+    PyObject *type;
+    PyObject **method_name;
+    PyCFunction func;
+    PyObject *method;
+    int flag;
+} __Pyx_CachedCFunction;
+
+/* CallUnboundCMethod1.proto */
+static PyObject* __Pyx__CallUnboundCMethod1(__Pyx_CachedCFunction* cfunc, PyObject* self, PyObject* arg);
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_CallUnboundCMethod1(__Pyx_CachedCFunction* cfunc, PyObject* self, PyObject* arg);
+#else
+#define __Pyx_CallUnboundCMethod1(cfunc, self, arg)  __Pyx__CallUnboundCMethod1(cfunc, self, arg)
+#endif
+
 /* PyObjectFormatSimple.proto */
 #if CYTHON_COMPILING_IN_PYPY
     #define __Pyx_PyObject_FormatSimple(s, f) (\
         likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
         PyObject_Format(s, f))
 #elif PY_MAJOR_VERSION < 3
     #define __Pyx_PyObject_FormatSimple(s, f) (\
@@ -1871,39 +1888,22 @@
 
 /* PyUnicode_Unicode.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_Unicode(PyObject *obj);
 
 /* py_dict_pop.proto */
 static CYTHON_INLINE PyObject *__Pyx_PyDict_Pop(PyObject *d, PyObject *key, PyObject *default_value);
 
-/* UnpackUnboundCMethod.proto */
-typedef struct {
-    PyObject *type;
-    PyObject **method_name;
-    PyCFunction func;
-    PyObject *method;
-    int flag;
-} __Pyx_CachedCFunction;
-
 /* CallUnboundCMethod2.proto */
 static PyObject* __Pyx__CallUnboundCMethod2(__Pyx_CachedCFunction* cfunc, PyObject* self, PyObject* arg1, PyObject* arg2);
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030600B1
 static CYTHON_INLINE PyObject *__Pyx_CallUnboundCMethod2(__Pyx_CachedCFunction *cfunc, PyObject *self, PyObject *arg1, PyObject *arg2);
 #else
 #define __Pyx_CallUnboundCMethod2(cfunc, self, arg1, arg2)  __Pyx__CallUnboundCMethod2(cfunc, self, arg1, arg2)
 #endif
 
-/* CallUnboundCMethod1.proto */
-static PyObject* __Pyx__CallUnboundCMethod1(__Pyx_CachedCFunction* cfunc, PyObject* self, PyObject* arg);
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_CallUnboundCMethod1(__Pyx_CachedCFunction* cfunc, PyObject* self, PyObject* arg);
-#else
-#define __Pyx_CallUnboundCMethod1(cfunc, self, arg)  __Pyx__CallUnboundCMethod1(cfunc, self, arg)
-#endif
-
 /* CIntToPyUnicode.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_From_char(char value, Py_ssize_t width, char padding_char, char format_char);
 
 /* CIntToPyUnicode.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_From_Py_ssize_t(Py_ssize_t value, Py_ssize_t width, char padding_char, char format_char);
 
 /* pyobject_as_double.proto */
@@ -2481,26 +2481,27 @@
 static const char __pyx_k_np[] = "np";
 static const char __pyx_k_to[] = " to ";
 static const char __pyx_k_2_1[] = "2,1";
 static const char __pyx_k_E_2[] = "E = ";
 static const char __pyx_k_E_3[] = "E/";
 static const char __pyx_k_PAR[] = "$PAR";
 static const char __pyx_k_TOT[] = "$TOT";
-static const char __pyx_k__22[] = "\n\r";
-static const char __pyx_k__23[] = "\r\n";
-static const char __pyx_k__25[] = "\t%.";
-static const char __pyx_k__41[] = "'!";
-static const char __pyx_k__42[] = ", ";
-static const char __pyx_k__43[] = "]!";
-static const char __pyx_k__54[] = ".";
-static const char __pyx_k__55[] = ",";
-static const char __pyx_k__56[] = "*";
-static const char __pyx_k__57[] = " = *!";
-static const char __pyx_k__58[] = " = ";
-static const char __pyx_k__59[] = ")!";
+static const char __pyx_k__22[] = "\"'";
+static const char __pyx_k__23[] = "\n\r";
+static const char __pyx_k__24[] = "\r\n";
+static const char __pyx_k__26[] = "\t%.";
+static const char __pyx_k__42[] = "'!";
+static const char __pyx_k__43[] = ", ";
+static const char __pyx_k__44[] = "]!";
+static const char __pyx_k__55[] = ".";
+static const char __pyx_k__56[] = ",";
+static const char __pyx_k__57[] = "*";
+static const char __pyx_k__58[] = " = *!";
+static const char __pyx_k__59[] = " = ";
+static const char __pyx_k__60[] = ")!";
 static const char __pyx_k_big[] = "big";
 static const char __pyx_k_d_d[] = "%d %d %.";
 static const char __pyx_k_f_2[] = "f";
 static const char __pyx_k_int[] = "int";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_obj[] = "obj";
 static const char __pyx_k_pop[] = "pop";
@@ -2813,25 +2814,26 @@
 static PyObject *__pyx_kp_u_Warning_Detected_more_than_one_d;
 static PyObject *__pyx_kp_u_Warning_P;
 static PyObject *__pyx_kp_u_Warning_detected_f2_0_for_P;
 static PyObject *__pyx_kp_u_We_require_f1_0_for_PnE_f1_f2;
 static PyObject *__pyx_kp_s__2;
 static PyObject *__pyx_kp_u__22;
 static PyObject *__pyx_kp_u__23;
-static PyObject *__pyx_kp_u__25;
-static PyObject *__pyx_kp_u__41;
+static PyObject *__pyx_kp_u__24;
+static PyObject *__pyx_kp_u__26;
 static PyObject *__pyx_kp_u__42;
 static PyObject *__pyx_kp_u__43;
+static PyObject *__pyx_kp_u__44;
 static PyObject *__pyx_kp_u__5;
-static PyObject *__pyx_kp_u__54;
 static PyObject *__pyx_kp_u__55;
 static PyObject *__pyx_kp_u__56;
 static PyObject *__pyx_kp_u__57;
 static PyObject *__pyx_kp_u__58;
 static PyObject *__pyx_kp_u__59;
+static PyObject *__pyx_kp_u__60;
 static PyObject *__pyx_n_s_allocate_buffer;
 static PyObject *__pyx_n_s_args;
 static PyObject *__pyx_n_s_array;
 static PyObject *__pyx_n_s_barcodes;
 static PyObject *__pyx_n_s_base;
 static PyObject *__pyx_kp_u_be_no_more_than_4_bytes_for_DAT;
 static PyObject *__pyx_n_u_big;
@@ -3088,14 +3090,15 @@
 static PyObject *__pyx_pf___pyx_memoryviewslice_2__setstate_cython__(CYTHON_UNUSED struct __pyx_memoryviewslice_obj *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView___pyx_unpickle_Enum(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static __Pyx_CachedCFunction __pyx_umethod_PyDict_Type_pop = {0, &__pyx_n_s_pop, 0, 0, 0};
+static __Pyx_CachedCFunction __pyx_umethod_PyUnicode_Type_strip = {0, &__pyx_n_s_strip, 0, 0, 0};
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_1;
 static PyObject *__pyx_int_2;
 static PyObject *__pyx_int_6;
 static PyObject *__pyx_int_8;
 static PyObject *__pyx_int_100000;
 static PyObject *__pyx_int_112105877;
@@ -3114,72 +3117,72 @@
 static int __pyx_k__15;
 static int __pyx_k__16;
 static int __pyx_k__17;
 static int __pyx_k__18;
 static int __pyx_k__19;
 static int __pyx_k__20;
 static int __pyx_k__21;
-static int __pyx_k__24;
-static int __pyx_k__26;
+static int __pyx_k__25;
 static int __pyx_k__27;
 static int __pyx_k__28;
 static int __pyx_k__29;
 static int __pyx_k__30;
 static int __pyx_k__31;
 static int __pyx_k__32;
 static int __pyx_k__33;
 static int __pyx_k__34;
 static int __pyx_k__35;
 static int __pyx_k__36;
 static int __pyx_k__37;
 static int __pyx_k__38;
 static int __pyx_k__39;
 static int __pyx_k__40;
+static int __pyx_k__41;
 static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_tuple__4;
-static PyObject *__pyx_slice__74;
-static PyObject *__pyx_tuple__44;
+static PyObject *__pyx_slice__75;
 static PyObject *__pyx_tuple__45;
 static PyObject *__pyx_tuple__46;
 static PyObject *__pyx_tuple__47;
 static PyObject *__pyx_tuple__48;
 static PyObject *__pyx_tuple__49;
 static PyObject *__pyx_tuple__50;
 static PyObject *__pyx_tuple__51;
 static PyObject *__pyx_tuple__52;
 static PyObject *__pyx_tuple__53;
-static PyObject *__pyx_tuple__60;
+static PyObject *__pyx_tuple__54;
 static PyObject *__pyx_tuple__61;
 static PyObject *__pyx_tuple__62;
 static PyObject *__pyx_tuple__63;
 static PyObject *__pyx_tuple__64;
 static PyObject *__pyx_tuple__65;
 static PyObject *__pyx_tuple__66;
 static PyObject *__pyx_tuple__67;
 static PyObject *__pyx_tuple__68;
 static PyObject *__pyx_tuple__69;
 static PyObject *__pyx_tuple__70;
 static PyObject *__pyx_tuple__71;
 static PyObject *__pyx_tuple__72;
 static PyObject *__pyx_tuple__73;
-static PyObject *__pyx_tuple__75;
+static PyObject *__pyx_tuple__74;
 static PyObject *__pyx_tuple__76;
 static PyObject *__pyx_tuple__77;
 static PyObject *__pyx_tuple__78;
 static PyObject *__pyx_tuple__79;
-static PyObject *__pyx_tuple__81;
-static PyObject *__pyx_tuple__83;
+static PyObject *__pyx_tuple__80;
+static PyObject *__pyx_tuple__82;
 static PyObject *__pyx_tuple__84;
 static PyObject *__pyx_tuple__85;
 static PyObject *__pyx_tuple__86;
 static PyObject *__pyx_tuple__87;
 static PyObject *__pyx_tuple__88;
-static PyObject *__pyx_codeobj__80;
-static PyObject *__pyx_codeobj__82;
-static PyObject *__pyx_codeobj__89;
+static PyObject *__pyx_tuple__89;
+static PyObject *__pyx_codeobj__81;
+static PyObject *__pyx_codeobj__83;
+static PyObject *__pyx_codeobj__90;
 /* Late includes */
 
 /* "ext_modules/io_funcs.pyx":37
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef tuple read_mtx(char* mtx_file):             # <<<<<<<<<<<<<<
  *     cdef FILE* fi = fopen(mtx_file, "r")
@@ -10621,23 +10624,23 @@
   Py_ssize_t __pyx_v_i;
   PyObject *__pyx_v_data = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_t_3;
-  Py_ssize_t __pyx_t_4;
-  Py_UCS4 __pyx_t_5;
-  PyObject *__pyx_t_6 = NULL;
-  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  Py_ssize_t __pyx_t_6;
+  Py_UCS4 __pyx_t_7;
   long __pyx_t_8;
-  int __pyx_t_9;
+  PyObject *__pyx_t_9 = NULL;
   int __pyx_t_10;
   int __pyx_t_11;
-  PyObject *__pyx_t_12 = NULL;
+  int __pyx_t_12;
   PyObject *__pyx_t_13 = NULL;
   PyObject *__pyx_t_14 = NULL;
   PyObject *__pyx_t_15 = NULL;
   PyObject *__pyx_t_16 = NULL;
   PyObject *__pyx_t_17 = NULL;
   PyObject *__pyx_t_18 = NULL;
   PyObject *__pyx_t_19 = NULL;
@@ -10762,680 +10765,792 @@
   #endif
 
   /* "ext_modules/io_funcs.pyx":148
  *     assert pch != NULL
  * 
  *     if strchr(delimiters, line[0]) != NULL:             # <<<<<<<<<<<<<<
  *         row_key = ""
- *         N = 1
+ *         colnames.append(pch)
  */
   __pyx_t_2 = ((strchr(__pyx_v_delimiters, (__pyx_v_line[0])) != NULL) != 0);
   if (__pyx_t_2) {
 
     /* "ext_modules/io_funcs.pyx":149
  * 
  *     if strchr(delimiters, line[0]) != NULL:
  *         row_key = ""             # <<<<<<<<<<<<<<
- *         N = 1
  *         colnames.append(pch)
+ *         colnames[N] = colnames[N].strip("\"'")
  */
     __Pyx_INCREF(__pyx_kp_u__5);
     __pyx_v_row_key = __pyx_kp_u__5;
 
     /* "ext_modules/io_funcs.pyx":150
  *     if strchr(delimiters, line[0]) != NULL:
  *         row_key = ""
- *         N = 1             # <<<<<<<<<<<<<<
- *         colnames.append(pch)
- *     else:
+ *         colnames.append(pch)             # <<<<<<<<<<<<<<
+ *         colnames[N] = colnames[N].strip("\"'")
+ *         N = 1
  */
-    __pyx_v_N = 1;
+    __pyx_t_1 = __Pyx_PyStr_FromString(__pyx_v_pch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 150, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_3 = __Pyx_PyList_Append(__pyx_v_colnames, __pyx_t_1); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 150, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
     /* "ext_modules/io_funcs.pyx":151
  *         row_key = ""
+ *         colnames.append(pch)
+ *         colnames[N] = colnames[N].strip("\"'")             # <<<<<<<<<<<<<<
  *         N = 1
- *         colnames.append(pch)             # <<<<<<<<<<<<<<
  *     else:
- *         row_key = pch
  */
-    __pyx_t_1 = __Pyx_PyStr_FromString(__pyx_v_pch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 151, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(PyList_GET_ITEM(__pyx_v_colnames, __pyx_v_N), __pyx_n_s_strip); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 151, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_5 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
+      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
+      if (likely(__pyx_t_5)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+        __Pyx_INCREF(__pyx_t_5);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_4, function);
+      }
+    }
+    __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_kp_u__22) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u__22);
+    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 151, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyList_Append(__pyx_v_colnames, __pyx_t_1); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 151, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    if (unlikely(__Pyx_SetItemInt(__pyx_v_colnames, __pyx_v_N, __pyx_t_1, int, 1, __Pyx_PyInt_From_int, 1, 0, 0) < 0)) __PYX_ERR(0, 151, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
+    /* "ext_modules/io_funcs.pyx":152
+ *         colnames.append(pch)
+ *         colnames[N] = colnames[N].strip("\"'")
+ *         N = 1             # <<<<<<<<<<<<<<
+ *     else:
+ *         row_key = pch
+ */
+    __pyx_v_N = 1;
+
     /* "ext_modules/io_funcs.pyx":148
  *     assert pch != NULL
  * 
  *     if strchr(delimiters, line[0]) != NULL:             # <<<<<<<<<<<<<<
  *         row_key = ""
- *         N = 1
+ *         colnames.append(pch)
  */
     goto __pyx_L3;
   }
 
-  /* "ext_modules/io_funcs.pyx":153
- *         colnames.append(pch)
+  /* "ext_modules/io_funcs.pyx":154
+ *         N = 1
  *     else:
  *         row_key = pch             # <<<<<<<<<<<<<<
+ *         row_key = row_key.strip("\"'")
  * 
- *     pch = strtok(NULL, delimiters)
  */
   /*else*/ {
-    __pyx_t_1 = __Pyx_PyUnicode_FromString(__pyx_v_pch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 153, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyUnicode_FromString(__pyx_v_pch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 154, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_row_key = ((PyObject*)__pyx_t_1);
     __pyx_t_1 = 0;
+
+    /* "ext_modules/io_funcs.pyx":155
+ *     else:
+ *         row_key = pch
+ *         row_key = row_key.strip("\"'")             # <<<<<<<<<<<<<<
+ * 
+ *     pch = strtok(NULL, delimiters)
+ */
+    __pyx_t_1 = __Pyx_CallUnboundCMethod1(&__pyx_umethod_PyUnicode_Type_strip, __pyx_v_row_key, __pyx_kp_u__22); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 155, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 155, __pyx_L1_error)
+    __Pyx_DECREF_SET(__pyx_v_row_key, ((PyObject*)__pyx_t_1));
+    __pyx_t_1 = 0;
   }
   __pyx_L3:;
 
-  /* "ext_modules/io_funcs.pyx":155
- *         row_key = pch
+  /* "ext_modules/io_funcs.pyx":157
+ *         row_key = row_key.strip("\"'")
  * 
  *     pch = strtok(NULL, delimiters)             # <<<<<<<<<<<<<<
  *     while pch != NULL:
  *         colnames.append(pch)
  */
   __pyx_v_pch = strtok(NULL, __pyx_v_delimiters);
 
-  /* "ext_modules/io_funcs.pyx":156
+  /* "ext_modules/io_funcs.pyx":158
  * 
  *     pch = strtok(NULL, delimiters)
  *     while pch != NULL:             # <<<<<<<<<<<<<<
  *         colnames.append(pch)
- *         N += 1
+ *         colnames[N] = colnames[N].strip("\"'")
  */
   while (1) {
     __pyx_t_2 = ((__pyx_v_pch != NULL) != 0);
     if (!__pyx_t_2) break;
 
-    /* "ext_modules/io_funcs.pyx":157
+    /* "ext_modules/io_funcs.pyx":159
  *     pch = strtok(NULL, delimiters)
  *     while pch != NULL:
  *         colnames.append(pch)             # <<<<<<<<<<<<<<
+ *         colnames[N] = colnames[N].strip("\"'")
  *         N += 1
- *         pch = strtok(NULL, delimiters)
  */
-    __pyx_t_1 = __Pyx_PyStr_FromString(__pyx_v_pch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 157, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyStr_FromString(__pyx_v_pch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 159, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyList_Append(__pyx_v_colnames, __pyx_t_1); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 157, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyList_Append(__pyx_v_colnames, __pyx_t_1); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 159, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "ext_modules/io_funcs.pyx":158
+    /* "ext_modules/io_funcs.pyx":160
  *     while pch != NULL:
  *         colnames.append(pch)
+ *         colnames[N] = colnames[N].strip("\"'")             # <<<<<<<<<<<<<<
+ *         N += 1
+ *         pch = strtok(NULL, delimiters)
+ */
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(PyList_GET_ITEM(__pyx_v_colnames, __pyx_v_N), __pyx_n_s_strip); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 160, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_5 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
+      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
+      if (likely(__pyx_t_5)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+        __Pyx_INCREF(__pyx_t_5);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_4, function);
+      }
+    }
+    __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_kp_u__22) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u__22);
+    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 160, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    if (unlikely(__Pyx_SetItemInt(__pyx_v_colnames, __pyx_v_N, __pyx_t_1, int, 1, __Pyx_PyInt_From_int, 1, 0, 0) < 0)) __PYX_ERR(0, 160, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+    /* "ext_modules/io_funcs.pyx":161
+ *         colnames.append(pch)
+ *         colnames[N] = colnames[N].strip("\"'")
  *         N += 1             # <<<<<<<<<<<<<<
  *         pch = strtok(NULL, delimiters)
  * 
  */
     __pyx_v_N = (__pyx_v_N + 1);
 
-    /* "ext_modules/io_funcs.pyx":159
- *         colnames.append(pch)
+    /* "ext_modules/io_funcs.pyx":162
+ *         colnames[N] = colnames[N].strip("\"'")
  *         N += 1
  *         pch = strtok(NULL, delimiters)             # <<<<<<<<<<<<<<
  * 
  *     if N == 0:
  */
     __pyx_v_pch = strtok(NULL, __pyx_v_delimiters);
   }
 
-  /* "ext_modules/io_funcs.pyx":161
+  /* "ext_modules/io_funcs.pyx":164
  *         pch = strtok(NULL, delimiters)
  * 
  *     if N == 0:             # <<<<<<<<<<<<<<
  *         raise ValueError(f"File {csv_file} contains no columns!")
  * 
  */
   __pyx_t_2 = ((__pyx_v_N == 0) != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "ext_modules/io_funcs.pyx":162
+    /* "ext_modules/io_funcs.pyx":165
  * 
  *     if N == 0:
  *         raise ValueError(f"File {csv_file} contains no columns!")             # <<<<<<<<<<<<<<
  * 
- *     colnames[N - 1] = colnames[N - 1].rstrip("\n\r")
+ *     colnames[N - 1] = colnames[N - 1].rstrip("\n\r").strip("\"'")
  */
-    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 162, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 165, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = 0;
-    __pyx_t_5 = 127;
+    __pyx_t_6 = 0;
+    __pyx_t_7 = 127;
     __Pyx_INCREF(__pyx_kp_u_File);
-    __pyx_t_4 += 5;
+    __pyx_t_6 += 5;
     __Pyx_GIVEREF(__pyx_kp_u_File);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_File);
-    __pyx_t_6 = __Pyx_PyStr_FromString(__pyx_v_csv_file); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 162, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_7 = __Pyx_PyObject_FormatSimple(__pyx_t_6, __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 162, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) : __pyx_t_5;
-    __pyx_t_4 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
-    __Pyx_GIVEREF(__pyx_t_7);
-    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_7);
-    __pyx_t_7 = 0;
+    __pyx_t_4 = __Pyx_PyStr_FromString(__pyx_v_csv_file); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 165, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 165, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_7 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_7) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_7;
+    __pyx_t_6 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
+    __Pyx_GIVEREF(__pyx_t_5);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_5);
+    __pyx_t_5 = 0;
     __Pyx_INCREF(__pyx_kp_u_contains_no_columns);
-    __pyx_t_4 += 21;
+    __pyx_t_6 += 21;
     __Pyx_GIVEREF(__pyx_kp_u_contains_no_columns);
     PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u_contains_no_columns);
-    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_1, 3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 162, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_5 = __Pyx_PyUnicode_Join(__pyx_t_1, 3, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 165, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 162, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 165, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 162, __pyx_L1_error)
+    __PYX_ERR(0, 165, __pyx_L1_error)
 
-    /* "ext_modules/io_funcs.pyx":161
+    /* "ext_modules/io_funcs.pyx":164
  *         pch = strtok(NULL, delimiters)
  * 
  *     if N == 0:             # <<<<<<<<<<<<<<
  *         raise ValueError(f"File {csv_file} contains no columns!")
  * 
  */
   }
 
-  /* "ext_modules/io_funcs.pyx":164
+  /* "ext_modules/io_funcs.pyx":167
  *         raise ValueError(f"File {csv_file} contains no columns!")
  * 
- *     colnames[N - 1] = colnames[N - 1].rstrip("\n\r")             # <<<<<<<<<<<<<<
+ *     colnames[N - 1] = colnames[N - 1].rstrip("\n\r").strip("\"'")             # <<<<<<<<<<<<<<
  * 
  *     while getline(&line, &size, fi) >=0:
  */
   __pyx_t_8 = (__pyx_v_N - 1);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(PyList_GET_ITEM(__pyx_v_colnames, __pyx_t_8), __pyx_n_s_rstrip); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 164, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_6 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
-    __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_7);
-    if (likely(__pyx_t_6)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
-      __Pyx_INCREF(__pyx_t_6);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(PyList_GET_ITEM(__pyx_v_colnames, __pyx_t_8), __pyx_n_s_rstrip); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 167, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_9 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
+    __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_4);
+    if (likely(__pyx_t_9)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+      __Pyx_INCREF(__pyx_t_9);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_7, function);
+      __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_6, __pyx_kp_u__22) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_kp_u__22);
-  __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 164, __pyx_L1_error)
+  __pyx_t_5 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_9, __pyx_kp_u__23) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u__23);
+  __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 167, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_strip); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 167, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+      __Pyx_INCREF(__pyx_t_5);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_4, function);
+    }
+  }
+  __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_kp_u__22) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u__22);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 167, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_8 = (__pyx_v_N - 1);
-  if (unlikely(__Pyx_SetItemInt(__pyx_v_colnames, __pyx_t_8, __pyx_t_1, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 164, __pyx_L1_error)
+  if (unlikely(__Pyx_SetItemInt(__pyx_v_colnames, __pyx_t_8, __pyx_t_1, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 167, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "ext_modules/io_funcs.pyx":166
- *     colnames[N - 1] = colnames[N - 1].rstrip("\n\r")
+  /* "ext_modules/io_funcs.pyx":169
+ *     colnames[N - 1] = colnames[N - 1].rstrip("\n\r").strip("\"'")
  * 
  *     while getline(&line, &size, fi) >=0:             # <<<<<<<<<<<<<<
  *         if line[0] < 32 or line[0] == 127:
  *             continue
  */
   while (1) {
     __pyx_t_2 = ((getline((&__pyx_v_line), (&__pyx_v_size), __pyx_v_fi) >= 0) != 0);
     if (!__pyx_t_2) break;
 
-    /* "ext_modules/io_funcs.pyx":167
+    /* "ext_modules/io_funcs.pyx":170
  * 
  *     while getline(&line, &size, fi) >=0:
  *         if line[0] < 32 or line[0] == 127:             # <<<<<<<<<<<<<<
  *             continue
  *         pch = strtok(line, delimiters)
  */
-    __pyx_t_9 = (((__pyx_v_line[0]) < 32) != 0);
-    if (!__pyx_t_9) {
+    __pyx_t_10 = (((__pyx_v_line[0]) < 32) != 0);
+    if (!__pyx_t_10) {
     } else {
-      __pyx_t_2 = __pyx_t_9;
+      __pyx_t_2 = __pyx_t_10;
       goto __pyx_L10_bool_binop_done;
     }
-    __pyx_t_9 = (((__pyx_v_line[0]) == 0x7F) != 0);
-    __pyx_t_2 = __pyx_t_9;
+    __pyx_t_10 = (((__pyx_v_line[0]) == 0x7F) != 0);
+    __pyx_t_2 = __pyx_t_10;
     __pyx_L10_bool_binop_done:;
     if (__pyx_t_2) {
 
-      /* "ext_modules/io_funcs.pyx":168
+      /* "ext_modules/io_funcs.pyx":171
  *     while getline(&line, &size, fi) >=0:
  *         if line[0] < 32 or line[0] == 127:
  *             continue             # <<<<<<<<<<<<<<
  *         pch = strtok(line, delimiters)
  *         assert pch != NULL
  */
       goto __pyx_L7_continue;
 
-      /* "ext_modules/io_funcs.pyx":167
+      /* "ext_modules/io_funcs.pyx":170
  * 
  *     while getline(&line, &size, fi) >=0:
  *         if line[0] < 32 or line[0] == 127:             # <<<<<<<<<<<<<<
  *             continue
  *         pch = strtok(line, delimiters)
  */
     }
 
-    /* "ext_modules/io_funcs.pyx":169
+    /* "ext_modules/io_funcs.pyx":172
  *         if line[0] < 32 or line[0] == 127:
  *             continue
  *         pch = strtok(line, delimiters)             # <<<<<<<<<<<<<<
  *         assert pch != NULL
  *         rownames.append(pch)
  */
     __pyx_v_pch = strtok(__pyx_v_line, __pyx_v_delimiters);
 
-    /* "ext_modules/io_funcs.pyx":170
+    /* "ext_modules/io_funcs.pyx":173
  *             continue
  *         pch = strtok(line, delimiters)
  *         assert pch != NULL             # <<<<<<<<<<<<<<
  *         rownames.append(pch)
- *         for i in range(N):
+ *         rownames[M] = rownames[M].strip("\"'")
  */
     #ifndef CYTHON_WITHOUT_ASSERTIONS
     if (unlikely(!Py_OptimizeFlag)) {
       if (unlikely(!((__pyx_v_pch != NULL) != 0))) {
         PyErr_SetNone(PyExc_AssertionError);
-        __PYX_ERR(0, 170, __pyx_L1_error)
+        __PYX_ERR(0, 173, __pyx_L1_error)
       }
     }
     #endif
 
-    /* "ext_modules/io_funcs.pyx":171
+    /* "ext_modules/io_funcs.pyx":174
  *         pch = strtok(line, delimiters)
  *         assert pch != NULL
  *         rownames.append(pch)             # <<<<<<<<<<<<<<
+ *         rownames[M] = rownames[M].strip("\"'")
  *         for i in range(N):
- *             pch = strtok(NULL, delimiters)
  */
-    __pyx_t_1 = __Pyx_PyStr_FromString(__pyx_v_pch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 171, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyStr_FromString(__pyx_v_pch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 174, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyList_Append(__pyx_v_rownames, __pyx_t_1); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 171, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyList_Append(__pyx_v_rownames, __pyx_t_1); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 174, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "ext_modules/io_funcs.pyx":172
+    /* "ext_modules/io_funcs.pyx":175
  *         assert pch != NULL
  *         rownames.append(pch)
+ *         rownames[M] = rownames[M].strip("\"'")             # <<<<<<<<<<<<<<
+ *         for i in range(N):
+ *             pch = strtok(NULL, delimiters)
+ */
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(PyList_GET_ITEM(__pyx_v_rownames, __pyx_v_M), __pyx_n_s_strip); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 175, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_5 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
+      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
+      if (likely(__pyx_t_5)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+        __Pyx_INCREF(__pyx_t_5);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_4, function);
+      }
+    }
+    __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_kp_u__22) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u__22);
+    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 175, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    if (unlikely(__Pyx_SetItemInt(__pyx_v_rownames, __pyx_v_M, __pyx_t_1, int, 1, __Pyx_PyInt_From_int, 1, 0, 0) < 0)) __PYX_ERR(0, 175, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+    /* "ext_modules/io_funcs.pyx":176
+ *         rownames.append(pch)
+ *         rownames[M] = rownames[M].strip("\"'")
  *         for i in range(N):             # <<<<<<<<<<<<<<
  *             pch = strtok(NULL, delimiters)
  *             assert pch != NULL
  */
-    __pyx_t_10 = __pyx_v_N;
-    __pyx_t_11 = __pyx_t_10;
-    for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_11; __pyx_t_4+=1) {
-      __pyx_v_i = __pyx_t_4;
+    __pyx_t_11 = __pyx_v_N;
+    __pyx_t_12 = __pyx_t_11;
+    for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_12; __pyx_t_6+=1) {
+      __pyx_v_i = __pyx_t_6;
 
-      /* "ext_modules/io_funcs.pyx":173
- *         rownames.append(pch)
+      /* "ext_modules/io_funcs.pyx":177
+ *         rownames[M] = rownames[M].strip("\"'")
  *         for i in range(N):
  *             pch = strtok(NULL, delimiters)             # <<<<<<<<<<<<<<
  *             assert pch != NULL
  *             if is_zero(pch) == 0:
  */
       __pyx_v_pch = strtok(NULL, __pyx_v_delimiters);
 
-      /* "ext_modules/io_funcs.pyx":174
+      /* "ext_modules/io_funcs.pyx":178
  *         for i in range(N):
  *             pch = strtok(NULL, delimiters)
  *             assert pch != NULL             # <<<<<<<<<<<<<<
  *             if is_zero(pch) == 0:
  *                 row_ind.append(M)
  */
       #ifndef CYTHON_WITHOUT_ASSERTIONS
       if (unlikely(!Py_OptimizeFlag)) {
         if (unlikely(!((__pyx_v_pch != NULL) != 0))) {
           PyErr_SetNone(PyExc_AssertionError);
-          __PYX_ERR(0, 174, __pyx_L1_error)
+          __PYX_ERR(0, 178, __pyx_L1_error)
         }
       }
       #endif
 
-      /* "ext_modules/io_funcs.pyx":175
+      /* "ext_modules/io_funcs.pyx":179
  *             pch = strtok(NULL, delimiters)
  *             assert pch != NULL
  *             if is_zero(pch) == 0:             # <<<<<<<<<<<<<<
  *                 row_ind.append(M)
  *                 col_ind.append(i)
  */
       __pyx_t_2 = ((__pyx_f_9pegasusio_5cylib_2io_is_zero(__pyx_v_pch) == 0) != 0);
       if (__pyx_t_2) {
 
-        /* "ext_modules/io_funcs.pyx":176
+        /* "ext_modules/io_funcs.pyx":180
  *             assert pch != NULL
  *             if is_zero(pch) == 0:
  *                 row_ind.append(M)             # <<<<<<<<<<<<<<
  *                 col_ind.append(i)
  *                 data_list.append(pch)
  */
-        __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_M); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 176, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_M); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 180, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_3 = __Pyx_PyList_Append(__pyx_v_row_ind, __pyx_t_1); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 176, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyList_Append(__pyx_v_row_ind, __pyx_t_1); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 180, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-        /* "ext_modules/io_funcs.pyx":177
+        /* "ext_modules/io_funcs.pyx":181
  *             if is_zero(pch) == 0:
  *                 row_ind.append(M)
  *                 col_ind.append(i)             # <<<<<<<<<<<<<<
  *                 data_list.append(pch)
  *                 if i == N - 1:
  */
-        __pyx_t_1 = PyInt_FromSsize_t(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error)
+        __pyx_t_1 = PyInt_FromSsize_t(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 181, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_3 = __Pyx_PyList_Append(__pyx_v_col_ind, __pyx_t_1); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 177, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyList_Append(__pyx_v_col_ind, __pyx_t_1); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 181, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-        /* "ext_modules/io_funcs.pyx":178
+        /* "ext_modules/io_funcs.pyx":182
  *                 row_ind.append(M)
  *                 col_ind.append(i)
  *                 data_list.append(pch)             # <<<<<<<<<<<<<<
  *                 if i == N - 1:
  *                     data_list[L] = data_list[L].rstrip("\r\n")
  */
-        __pyx_t_1 = __Pyx_PyStr_FromString(__pyx_v_pch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 178, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyStr_FromString(__pyx_v_pch); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 182, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_3 = __Pyx_PyList_Append(__pyx_v_data_list, __pyx_t_1); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 178, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyList_Append(__pyx_v_data_list, __pyx_t_1); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 182, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-        /* "ext_modules/io_funcs.pyx":179
+        /* "ext_modules/io_funcs.pyx":183
  *                 col_ind.append(i)
  *                 data_list.append(pch)
  *                 if i == N - 1:             # <<<<<<<<<<<<<<
  *                     data_list[L] = data_list[L].rstrip("\r\n")
  *                 L += 1
  */
         __pyx_t_2 = ((__pyx_v_i == (__pyx_v_N - 1)) != 0);
         if (__pyx_t_2) {
 
-          /* "ext_modules/io_funcs.pyx":180
+          /* "ext_modules/io_funcs.pyx":184
  *                 data_list.append(pch)
  *                 if i == N - 1:
  *                     data_list[L] = data_list[L].rstrip("\r\n")             # <<<<<<<<<<<<<<
  *                 L += 1
  *         M += 1
  */
-          __pyx_t_7 = __Pyx_PyObject_GetAttrStr(PyList_GET_ITEM(__pyx_v_data_list, __pyx_v_L), __pyx_n_s_rstrip); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 180, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_7);
-          __pyx_t_6 = NULL;
-          if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
-            __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_7);
-            if (likely(__pyx_t_6)) {
-              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
-              __Pyx_INCREF(__pyx_t_6);
+          __pyx_t_4 = __Pyx_PyObject_GetAttrStr(PyList_GET_ITEM(__pyx_v_data_list, __pyx_v_L), __pyx_n_s_rstrip); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 184, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_4);
+          __pyx_t_5 = NULL;
+          if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
+            __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
+            if (likely(__pyx_t_5)) {
+              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+              __Pyx_INCREF(__pyx_t_5);
               __Pyx_INCREF(function);
-              __Pyx_DECREF_SET(__pyx_t_7, function);
+              __Pyx_DECREF_SET(__pyx_t_4, function);
             }
           }
-          __pyx_t_1 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_6, __pyx_kp_u__23) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_kp_u__23);
-          __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-          if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 180, __pyx_L1_error)
+          __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_kp_u__24) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u__24);
+          __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+          if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 184, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_1);
-          __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-          if (unlikely(__Pyx_SetItemInt(__pyx_v_data_list, __pyx_v_L, __pyx_t_1, size_t, 0, __Pyx_PyInt_FromSize_t, 1, 0, 0) < 0)) __PYX_ERR(0, 180, __pyx_L1_error)
+          __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+          if (unlikely(__Pyx_SetItemInt(__pyx_v_data_list, __pyx_v_L, __pyx_t_1, size_t, 0, __Pyx_PyInt_FromSize_t, 1, 0, 0) < 0)) __PYX_ERR(0, 184, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-          /* "ext_modules/io_funcs.pyx":179
+          /* "ext_modules/io_funcs.pyx":183
  *                 col_ind.append(i)
  *                 data_list.append(pch)
  *                 if i == N - 1:             # <<<<<<<<<<<<<<
  *                     data_list[L] = data_list[L].rstrip("\r\n")
  *                 L += 1
  */
         }
 
-        /* "ext_modules/io_funcs.pyx":181
+        /* "ext_modules/io_funcs.pyx":185
  *                 if i == N - 1:
  *                     data_list[L] = data_list[L].rstrip("\r\n")
  *                 L += 1             # <<<<<<<<<<<<<<
  *         M += 1
  * 
  */
         __pyx_v_L = (__pyx_v_L + 1);
 
-        /* "ext_modules/io_funcs.pyx":175
+        /* "ext_modules/io_funcs.pyx":179
  *             pch = strtok(NULL, delimiters)
  *             assert pch != NULL
  *             if is_zero(pch) == 0:             # <<<<<<<<<<<<<<
  *                 row_ind.append(M)
  *                 col_ind.append(i)
  */
       }
     }
 
-    /* "ext_modules/io_funcs.pyx":182
+    /* "ext_modules/io_funcs.pyx":186
  *                     data_list[L] = data_list[L].rstrip("\r\n")
  *                 L += 1
  *         M += 1             # <<<<<<<<<<<<<<
  * 
  *     free(line)
  */
     __pyx_v_M = (__pyx_v_M + 1);
     __pyx_L7_continue:;
   }
 
-  /* "ext_modules/io_funcs.pyx":184
+  /* "ext_modules/io_funcs.pyx":188
  *         M += 1
  * 
  *     free(line)             # <<<<<<<<<<<<<<
  *     fclose(fi)
  * 
  */
   free(__pyx_v_line);
 
-  /* "ext_modules/io_funcs.pyx":185
+  /* "ext_modules/io_funcs.pyx":189
  * 
  *     free(line)
  *     fclose(fi)             # <<<<<<<<<<<<<<
  * 
  *     try:
  */
   (void)(fclose(__pyx_v_fi));
 
-  /* "ext_modules/io_funcs.pyx":187
+  /* "ext_modules/io_funcs.pyx":191
  *     fclose(fi)
  * 
  *     try:             # <<<<<<<<<<<<<<
  *         data = np.array(data_list, dtype = np.intc)
  *     except ValueError:
  */
   {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
-    __Pyx_ExceptionSave(&__pyx_t_12, &__pyx_t_13, &__pyx_t_14);
-    __Pyx_XGOTREF(__pyx_t_12);
+    __Pyx_ExceptionSave(&__pyx_t_13, &__pyx_t_14, &__pyx_t_15);
     __Pyx_XGOTREF(__pyx_t_13);
     __Pyx_XGOTREF(__pyx_t_14);
+    __Pyx_XGOTREF(__pyx_t_15);
     /*try:*/ {
 
-      /* "ext_modules/io_funcs.pyx":188
+      /* "ext_modules/io_funcs.pyx":192
  * 
  *     try:
  *         data = np.array(data_list, dtype = np.intc)             # <<<<<<<<<<<<<<
  *     except ValueError:
  *         data = np.array(data_list, dtype = np.float32)
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 188, __pyx_L16_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 192, __pyx_L16_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_array); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 188, __pyx_L16_error)
-      __Pyx_GOTREF(__pyx_t_7);
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_array); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 192, __pyx_L16_error)
+      __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 188, __pyx_L16_error)
+      __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 192, __pyx_L16_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_INCREF(__pyx_v_data_list);
       __Pyx_GIVEREF(__pyx_v_data_list);
       PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_data_list);
-      __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 188, __pyx_L16_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_GetModuleGlobalName(__pyx_t_15, __pyx_n_s_np); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 188, __pyx_L16_error)
-      __Pyx_GOTREF(__pyx_t_15);
-      __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_intc); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 188, __pyx_L16_error)
+      __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 192, __pyx_L16_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_np); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 192, __pyx_L16_error)
+      __Pyx_GOTREF(__pyx_t_9);
+      __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_intc); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 192, __pyx_L16_error)
       __Pyx_GOTREF(__pyx_t_16);
-      __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-      if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_16) < 0) __PYX_ERR(0, 188, __pyx_L16_error)
+      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+      if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_16) < 0) __PYX_ERR(0, 192, __pyx_L16_error)
       __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-      __pyx_t_16 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_1, __pyx_t_6); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 188, __pyx_L16_error)
+      __pyx_t_16 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_1, __pyx_t_5); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 192, __pyx_L16_error)
       __Pyx_GOTREF(__pyx_t_16);
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_v_data = __pyx_t_16;
       __pyx_t_16 = 0;
 
-      /* "ext_modules/io_funcs.pyx":187
+      /* "ext_modules/io_funcs.pyx":191
  *     fclose(fi)
  * 
  *     try:             # <<<<<<<<<<<<<<
  *         data = np.array(data_list, dtype = np.intc)
  *     except ValueError:
  */
     }
-    __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
     __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
     __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
+    __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
     goto __pyx_L21_try_end;
     __pyx_L16_error:;
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
     __Pyx_XDECREF(__pyx_t_16); __pyx_t_16 = 0;
-    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-    /* "ext_modules/io_funcs.pyx":189
+    /* "ext_modules/io_funcs.pyx":193
  *     try:
  *         data = np.array(data_list, dtype = np.intc)
  *     except ValueError:             # <<<<<<<<<<<<<<
  *         data = np.array(data_list, dtype = np.float32)
  * 
  */
-    __pyx_t_10 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_ValueError);
-    if (__pyx_t_10) {
+    __pyx_t_11 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_ValueError);
+    if (__pyx_t_11) {
       __Pyx_AddTraceback("pegasusio.cylib.io.read_csv", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_16, &__pyx_t_6, &__pyx_t_1) < 0) __PYX_ERR(0, 189, __pyx_L18_except_error)
+      if (__Pyx_GetException(&__pyx_t_16, &__pyx_t_5, &__pyx_t_1) < 0) __PYX_ERR(0, 193, __pyx_L18_except_error)
       __Pyx_GOTREF(__pyx_t_16);
-      __Pyx_GOTREF(__pyx_t_6);
+      __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_1);
 
-      /* "ext_modules/io_funcs.pyx":190
+      /* "ext_modules/io_funcs.pyx":194
  *         data = np.array(data_list, dtype = np.intc)
  *     except ValueError:
  *         data = np.array(data_list, dtype = np.float32)             # <<<<<<<<<<<<<<
  * 
  *     return row_ind, col_ind, data, (M, N), row_key, rownames, colnames
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 190, __pyx_L18_except_error)
-      __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_array); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 190, __pyx_L18_except_error)
-      __Pyx_GOTREF(__pyx_t_15);
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 190, __pyx_L18_except_error)
-      __Pyx_GOTREF(__pyx_t_7);
+      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 194, __pyx_L18_except_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_array); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 194, __pyx_L18_except_error)
+      __Pyx_GOTREF(__pyx_t_9);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 194, __pyx_L18_except_error)
+      __Pyx_GOTREF(__pyx_t_4);
       __Pyx_INCREF(__pyx_v_data_list);
       __Pyx_GIVEREF(__pyx_v_data_list);
-      PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_v_data_list);
-      __pyx_t_17 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 190, __pyx_L18_except_error)
+      PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_data_list);
+      __pyx_t_17 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 194, __pyx_L18_except_error)
       __Pyx_GOTREF(__pyx_t_17);
-      __Pyx_GetModuleGlobalName(__pyx_t_18, __pyx_n_s_np); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 190, __pyx_L18_except_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_18, __pyx_n_s_np); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 194, __pyx_L18_except_error)
       __Pyx_GOTREF(__pyx_t_18);
-      __pyx_t_19 = __Pyx_PyObject_GetAttrStr(__pyx_t_18, __pyx_n_s_float32); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 190, __pyx_L18_except_error)
+      __pyx_t_19 = __Pyx_PyObject_GetAttrStr(__pyx_t_18, __pyx_n_s_float32); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 194, __pyx_L18_except_error)
       __Pyx_GOTREF(__pyx_t_19);
       __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
-      if (PyDict_SetItem(__pyx_t_17, __pyx_n_s_dtype, __pyx_t_19) < 0) __PYX_ERR(0, 190, __pyx_L18_except_error)
+      if (PyDict_SetItem(__pyx_t_17, __pyx_n_s_dtype, __pyx_t_19) < 0) __PYX_ERR(0, 194, __pyx_L18_except_error)
       __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
-      __pyx_t_19 = __Pyx_PyObject_Call(__pyx_t_15, __pyx_t_7, __pyx_t_17); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 190, __pyx_L18_except_error)
+      __pyx_t_19 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_4, __pyx_t_17); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 194, __pyx_L18_except_error)
       __Pyx_GOTREF(__pyx_t_19);
-      __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
       __Pyx_XDECREF_SET(__pyx_v_data, __pyx_t_19);
       __pyx_t_19 = 0;
       __Pyx_XDECREF(__pyx_t_16); __pyx_t_16 = 0;
-      __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
       goto __pyx_L17_exception_handled;
     }
     goto __pyx_L18_except_error;
     __pyx_L18_except_error:;
 
-    /* "ext_modules/io_funcs.pyx":187
+    /* "ext_modules/io_funcs.pyx":191
  *     fclose(fi)
  * 
  *     try:             # <<<<<<<<<<<<<<
  *         data = np.array(data_list, dtype = np.intc)
  *     except ValueError:
  */
-    __Pyx_XGIVEREF(__pyx_t_12);
     __Pyx_XGIVEREF(__pyx_t_13);
     __Pyx_XGIVEREF(__pyx_t_14);
-    __Pyx_ExceptionReset(__pyx_t_12, __pyx_t_13, __pyx_t_14);
+    __Pyx_XGIVEREF(__pyx_t_15);
+    __Pyx_ExceptionReset(__pyx_t_13, __pyx_t_14, __pyx_t_15);
     goto __pyx_L1_error;
     __pyx_L17_exception_handled:;
-    __Pyx_XGIVEREF(__pyx_t_12);
     __Pyx_XGIVEREF(__pyx_t_13);
     __Pyx_XGIVEREF(__pyx_t_14);
-    __Pyx_ExceptionReset(__pyx_t_12, __pyx_t_13, __pyx_t_14);
+    __Pyx_XGIVEREF(__pyx_t_15);
+    __Pyx_ExceptionReset(__pyx_t_13, __pyx_t_14, __pyx_t_15);
     __pyx_L21_try_end:;
   }
 
-  /* "ext_modules/io_funcs.pyx":192
+  /* "ext_modules/io_funcs.pyx":196
  *         data = np.array(data_list, dtype = np.float32)
  * 
  *     return row_ind, col_ind, data, (M, N), row_key, rownames, colnames             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_M); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 192, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_M); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_N); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 192, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_16 = PyTuple_New(2); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 192, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_N); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_16 = PyTuple_New(2); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_16);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_16, 0, __pyx_t_1);
-  __Pyx_GIVEREF(__pyx_t_6);
-  PyTuple_SET_ITEM(__pyx_t_16, 1, __pyx_t_6);
+  __Pyx_GIVEREF(__pyx_t_5);
+  PyTuple_SET_ITEM(__pyx_t_16, 1, __pyx_t_5);
   __pyx_t_1 = 0;
-  __pyx_t_6 = 0;
-  __pyx_t_6 = PyTuple_New(7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 192, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_5 = 0;
+  __pyx_t_5 = PyTuple_New(7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_v_row_ind);
   __Pyx_GIVEREF(__pyx_v_row_ind);
-  PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_v_row_ind);
+  PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_row_ind);
   __Pyx_INCREF(__pyx_v_col_ind);
   __Pyx_GIVEREF(__pyx_v_col_ind);
-  PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_v_col_ind);
+  PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_v_col_ind);
   __Pyx_INCREF(__pyx_v_data);
   __Pyx_GIVEREF(__pyx_v_data);
-  PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_v_data);
+  PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_v_data);
   __Pyx_GIVEREF(__pyx_t_16);
-  PyTuple_SET_ITEM(__pyx_t_6, 3, __pyx_t_16);
+  PyTuple_SET_ITEM(__pyx_t_5, 3, __pyx_t_16);
   __Pyx_INCREF(__pyx_v_row_key);
   __Pyx_GIVEREF(__pyx_v_row_key);
-  PyTuple_SET_ITEM(__pyx_t_6, 4, __pyx_v_row_key);
+  PyTuple_SET_ITEM(__pyx_t_5, 4, __pyx_v_row_key);
   __Pyx_INCREF(__pyx_v_rownames);
   __Pyx_GIVEREF(__pyx_v_rownames);
-  PyTuple_SET_ITEM(__pyx_t_6, 5, __pyx_v_rownames);
+  PyTuple_SET_ITEM(__pyx_t_5, 5, __pyx_v_rownames);
   __Pyx_INCREF(__pyx_v_colnames);
   __Pyx_GIVEREF(__pyx_v_colnames);
-  PyTuple_SET_ITEM(__pyx_t_6, 6, __pyx_v_colnames);
+  PyTuple_SET_ITEM(__pyx_t_5, 6, __pyx_v_colnames);
   __pyx_t_16 = 0;
-  __pyx_r = ((PyObject*)__pyx_t_6);
-  __pyx_t_6 = 0;
+  __pyx_r = ((PyObject*)__pyx_t_5);
+  __pyx_t_5 = 0;
   goto __pyx_L0;
 
   /* "ext_modules/io_funcs.pyx":132
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef tuple read_csv(char* csv_file, char* delimiters):             # <<<<<<<<<<<<<<
  *     cdef FILE* fi = fopen(csv_file, "r")
  *     cdef char* line = NULL
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_15);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_9);
   __Pyx_XDECREF(__pyx_t_16);
   __Pyx_XDECREF(__pyx_t_17);
   __Pyx_XDECREF(__pyx_t_18);
   __Pyx_XDECREF(__pyx_t_19);
   __Pyx_AddTraceback("pegasusio.cylib.io.read_csv", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
@@ -11537,15 +11652,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ext_modules/io_funcs.pyx":197
+/* "ext_modules/io_funcs.pyx":201
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef void write_dense(char* output_file, str[:] barcodes, str[:] features, data_type[:] data, indices_type[:] indices, indptr_type[:] indptr, int M, int N, int precision = 2):             # <<<<<<<<<<<<<<
  *     """ Input must be csr_matrix internal representation, gene by cell (X.T.tocsr()); Output will be gene by cell
  *     """
  */
 
@@ -11587,31 +11702,31 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_signatures)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_args)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fused_cpdef", 1, 4, 4, 1); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fused_cpdef", 1, 4, 4, 1); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_kwargs)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fused_cpdef", 1, 4, 4, 2); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fused_cpdef", 1, 4, 4, 2); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_defaults)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fused_cpdef", 1, 4, 4, 3); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fused_cpdef", 1, 4, 4, 3); __PYX_ERR(0, 201, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fused_cpdef") < 0)) __PYX_ERR(0, 197, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fused_cpdef") < 0)) __PYX_ERR(0, 201, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -11620,15 +11735,15 @@
     __pyx_v_signatures = values[0];
     __pyx_v_args = values[1];
     __pyx_v_kwargs = values[2];
     __pyx_v_defaults = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__pyx_fused_cpdef", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 197, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__pyx_fused_cpdef", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 201, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pegasusio.cylib.io.__pyx_fused_cpdef", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9pegasusio_5cylib_2io_6write_dense(__pyx_self, __pyx_v_signatures, __pyx_v_args, __pyx_v_kwargs, __pyx_v_defaults);
 
@@ -11676,15 +11791,15 @@
   Py_ssize_t __pyx_t_17;
   int __pyx_t_18;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("write_dense", 0);
   __Pyx_INCREF(__pyx_v_kwargs);
-  __pyx_t_1 = PyList_New(1 * 3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(1 * 3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   { Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < 3; __pyx_temp++) {
       __Pyx_INCREF(Py_None);
       __Pyx_GIVEREF(Py_None);
       PyList_SET_ITEM(__pyx_t_1, __pyx_temp, Py_None);
     }
@@ -11694,39 +11809,39 @@
   __pyx_t_3 = (__pyx_v_kwargs != Py_None);
   __pyx_t_4 = (__pyx_t_3 != 0);
   if (__pyx_t_4) {
   } else {
     __pyx_t_2 = __pyx_t_4;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_kwargs); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_kwargs); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 201, __pyx_L1_error)
   __pyx_t_3 = ((!__pyx_t_4) != 0);
   __pyx_t_2 = __pyx_t_3;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_2) {
     __Pyx_INCREF(Py_None);
     __Pyx_DECREF_SET(__pyx_v_kwargs, Py_None);
   }
-  __pyx_t_1 = ((PyObject *)__Pyx_ImportNumPyArrayTypeIfAvailable()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__Pyx_ImportNumPyArrayTypeIfAvailable()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_ndarray = ((PyTypeObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   __pyx_v_itemsize = -1L;
   __pyx_v_int_is_signed = (!((((int)-1L) > 0) != 0));
   __pyx_v_long_is_signed = (!((((long)-1L) > 0) != 0));
   if (unlikely(__pyx_v_args == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 197, __pyx_L1_error)
+    __PYX_ERR(0, 201, __pyx_L1_error)
   }
-  __pyx_t_5 = PyTuple_GET_SIZE(((PyObject*)__pyx_v_args)); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_GET_SIZE(((PyObject*)__pyx_v_args)); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 201, __pyx_L1_error)
   __pyx_t_2 = ((3 < __pyx_t_5) != 0);
   if (__pyx_t_2) {
     if (unlikely(__pyx_v_args == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 197, __pyx_L1_error)
+      __PYX_ERR(0, 201, __pyx_L1_error)
     }
     __pyx_t_1 = PyTuple_GET_ITEM(((PyObject*)__pyx_v_args), 3);
     __Pyx_INCREF(__pyx_t_1);
     __pyx_v_arg = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L6;
   }
@@ -11735,85 +11850,85 @@
   if (__pyx_t_4) {
   } else {
     __pyx_t_2 = __pyx_t_4;
     goto __pyx_L7_bool_binop_done;
   }
   if (unlikely(__pyx_v_kwargs == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(0, 197, __pyx_L1_error)
+    __PYX_ERR(0, 201, __pyx_L1_error)
   }
-  __pyx_t_4 = (__Pyx_PyDict_ContainsTF(__pyx_n_s_data, ((PyObject*)__pyx_v_kwargs), Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PyDict_ContainsTF(__pyx_n_s_data, ((PyObject*)__pyx_v_kwargs), Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 201, __pyx_L1_error)
   __pyx_t_3 = (__pyx_t_4 != 0);
   __pyx_t_2 = __pyx_t_3;
   __pyx_L7_bool_binop_done:;
   if (__pyx_t_2) {
     if (unlikely(__pyx_v_kwargs == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 197, __pyx_L1_error)
+      __PYX_ERR(0, 201, __pyx_L1_error)
     }
-    __pyx_t_1 = __Pyx_PyDict_GetItem(((PyObject*)__pyx_v_kwargs), __pyx_n_s_data); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyDict_GetItem(((PyObject*)__pyx_v_kwargs), __pyx_n_s_data); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_arg = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L6;
   }
   /*else*/ {
     if (unlikely(__pyx_v_args == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-      __PYX_ERR(0, 197, __pyx_L1_error)
+      __PYX_ERR(0, 201, __pyx_L1_error)
     }
-    __pyx_t_5 = PyTuple_GET_SIZE(((PyObject*)__pyx_v_args)); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 197, __pyx_L1_error)
-    __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_GET_SIZE(((PyObject*)__pyx_v_args)); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 201, __pyx_L1_error)
+    __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 201, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_INCREF(__pyx_int_8);
     __Pyx_GIVEREF(__pyx_int_8);
     PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_int_8);
     __Pyx_INCREF(__pyx_n_s_s);
     __Pyx_GIVEREF(__pyx_n_s_s);
     PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_n_s_s);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_t_1);
     __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyString_Format(__pyx_kp_s_Expected_at_least_d_argument_s_g, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyString_Format(__pyx_kp_s_Expected_at_least_d_argument_s_g, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 201, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_6, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __PYX_ERR(0, 197, __pyx_L1_error)
+    __PYX_ERR(0, 201, __pyx_L1_error)
   }
   __pyx_L6:;
   while (1) {
     __pyx_t_2 = (__pyx_v_ndarray != ((PyTypeObject*)Py_None));
     __pyx_t_3 = (__pyx_t_2 != 0);
     if (__pyx_t_3) {
       __pyx_t_3 = __Pyx_TypeCheck(__pyx_v_arg, __pyx_v_ndarray); 
       __pyx_t_2 = (__pyx_t_3 != 0);
       if (__pyx_t_2) {
-        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_dtype); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 197, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_dtype); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 201, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __pyx_v_dtype = __pyx_t_6;
         __pyx_t_6 = 0;
         goto __pyx_L12;
       }
       __pyx_t_2 = __pyx_memoryview_check(__pyx_v_arg); 
       __pyx_t_3 = (__pyx_t_2 != 0);
       if (__pyx_t_3) {
-        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_base); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 197, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_base); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 201, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __pyx_v_arg_base = __pyx_t_6;
         __pyx_t_6 = 0;
         __pyx_t_3 = __Pyx_TypeCheck(__pyx_v_arg_base, __pyx_v_ndarray); 
         __pyx_t_2 = (__pyx_t_3 != 0);
         if (__pyx_t_2) {
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg_base, __pyx_n_s_dtype); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 197, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg_base, __pyx_n_s_dtype); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 201, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
           __pyx_v_dtype = __pyx_t_6;
           __pyx_t_6 = 0;
           goto __pyx_L13;
         }
         /*else*/ {
           __Pyx_INCREF(Py_None);
@@ -11827,108 +11942,108 @@
         __pyx_v_dtype = Py_None;
       }
       __pyx_L12:;
       __pyx_v_itemsize = -1L;
       __pyx_t_2 = (__pyx_v_dtype != Py_None);
       __pyx_t_3 = (__pyx_t_2 != 0);
       if (__pyx_t_3) {
-        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_dtype, __pyx_n_s_itemsize); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 197, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_dtype, __pyx_n_s_itemsize); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 201, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __pyx_v_itemsize = __pyx_t_5;
-        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_dtype, __pyx_n_s_kind); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 197, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_dtype, __pyx_n_s_kind); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 201, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_7 = __Pyx_PyObject_Ord(__pyx_t_6); if (unlikely(__pyx_t_7 == ((long)(long)(Py_UCS4)-1))) __PYX_ERR(0, 197, __pyx_L1_error)
+        __pyx_t_7 = __Pyx_PyObject_Ord(__pyx_t_6); if (unlikely(__pyx_t_7 == ((long)(long)(Py_UCS4)-1))) __PYX_ERR(0, 201, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __pyx_v_kind = __pyx_t_7;
         __pyx_v_dtype_signed = (__pyx_v_kind == 'i');
         switch (__pyx_v_kind) {
           case 'i':
           case 'u':
           __pyx_t_2 = (((sizeof(int)) == __pyx_v_itemsize) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L16_bool_binop_done;
           }
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 197, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 201, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __pyx_t_2 = ((((Py_ssize_t)__pyx_t_5) == 1) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L16_bool_binop_done;
           }
           __pyx_t_2 = ((!((__pyx_v_int_is_signed ^ __pyx_v_dtype_signed) != 0)) != 0);
           __pyx_t_3 = __pyx_t_2;
           __pyx_L16_bool_binop_done:;
           if (__pyx_t_3) {
-            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 197, __pyx_L1_error)
+            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 201, __pyx_L1_error)
             goto __pyx_L10_break;
           }
           __pyx_t_2 = (((sizeof(long)) == __pyx_v_itemsize) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L20_bool_binop_done;
           }
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 197, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 201, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __pyx_t_2 = ((((Py_ssize_t)__pyx_t_5) == 1) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L20_bool_binop_done;
           }
           __pyx_t_2 = ((!((__pyx_v_long_is_signed ^ __pyx_v_dtype_signed) != 0)) != 0);
           __pyx_t_3 = __pyx_t_2;
           __pyx_L20_bool_binop_done:;
           if (__pyx_t_3) {
-            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_long, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 197, __pyx_L1_error)
+            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_long, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 201, __pyx_L1_error)
             goto __pyx_L10_break;
           }
           break;
           case 'f':
           __pyx_t_2 = (((sizeof(float)) == __pyx_v_itemsize) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L24_bool_binop_done;
           }
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 197, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 201, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __pyx_t_2 = ((((Py_ssize_t)__pyx_t_5) == 1) != 0);
           __pyx_t_3 = __pyx_t_2;
           __pyx_L24_bool_binop_done:;
           if (__pyx_t_3) {
-            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_float, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 197, __pyx_L1_error)
+            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_float, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 201, __pyx_L1_error)
             goto __pyx_L10_break;
           }
           __pyx_t_2 = (((sizeof(double)) == __pyx_v_itemsize) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L27_bool_binop_done;
           }
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 197, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 201, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __pyx_t_2 = ((((Py_ssize_t)__pyx_t_5) == 1) != 0);
           __pyx_t_3 = __pyx_t_2;
           __pyx_L27_bool_binop_done:;
           if (__pyx_t_3) {
-            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_double, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 197, __pyx_L1_error)
+            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_double, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 201, __pyx_L1_error)
             goto __pyx_L10_break;
           }
           break;
           case 'c':
           break;
           case 'O':
           break;
@@ -11947,15 +12062,15 @@
     __pyx_L30_bool_binop_done:;
     if (__pyx_t_3) {
       __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_ds_int(__pyx_v_arg, 0); 
       __pyx_v_memslice = __pyx_t_8;
       __pyx_t_3 = (__pyx_v_memslice.memview != 0);
       if (__pyx_t_3) {
         __PYX_XDEC_MEMVIEW((&__pyx_v_memslice), 1); 
-        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 197, __pyx_L1_error)
+        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 201, __pyx_L1_error)
         goto __pyx_L10_break;
       }
       /*else*/ {
         PyErr_Clear(); 
       }
     }
     __pyx_t_2 = ((__pyx_v_itemsize == -1L) != 0);
@@ -11969,15 +12084,15 @@
     __pyx_L34_bool_binop_done:;
     if (__pyx_t_3) {
       __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_ds_long(__pyx_v_arg, 0); 
       __pyx_v_memslice = __pyx_t_8;
       __pyx_t_3 = (__pyx_v_memslice.memview != 0);
       if (__pyx_t_3) {
         __PYX_XDEC_MEMVIEW((&__pyx_v_memslice), 1); 
-        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_long, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 197, __pyx_L1_error)
+        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_long, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 201, __pyx_L1_error)
         goto __pyx_L10_break;
       }
       /*else*/ {
         PyErr_Clear(); 
       }
     }
     __pyx_t_2 = ((__pyx_v_itemsize == -1L) != 0);
@@ -11991,15 +12106,15 @@
     __pyx_L38_bool_binop_done:;
     if (__pyx_t_3) {
       __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(__pyx_v_arg, 0); 
       __pyx_v_memslice = __pyx_t_8;
       __pyx_t_3 = (__pyx_v_memslice.memview != 0);
       if (__pyx_t_3) {
         __PYX_XDEC_MEMVIEW((&__pyx_v_memslice), 1); 
-        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_float, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 197, __pyx_L1_error)
+        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_float, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 201, __pyx_L1_error)
         goto __pyx_L10_break;
       }
       /*else*/ {
         PyErr_Clear(); 
       }
     }
     __pyx_t_2 = ((__pyx_v_itemsize == -1L) != 0);
@@ -12013,35 +12128,35 @@
     __pyx_L42_bool_binop_done:;
     if (__pyx_t_3) {
       __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_ds_double(__pyx_v_arg, 0); 
       __pyx_v_memslice = __pyx_t_8;
       __pyx_t_3 = (__pyx_v_memslice.memview != 0);
       if (__pyx_t_3) {
         __PYX_XDEC_MEMVIEW((&__pyx_v_memslice), 1); 
-        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_double, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 197, __pyx_L1_error)
+        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_double, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 201, __pyx_L1_error)
         goto __pyx_L10_break;
       }
       /*else*/ {
         PyErr_Clear(); 
       }
     }
-    if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, Py_None, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 197, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, Py_None, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 201, __pyx_L1_error)
     goto __pyx_L10_break;
   }
   __pyx_L10_break:;
   if (unlikely(__pyx_v_args == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 197, __pyx_L1_error)
+    __PYX_ERR(0, 201, __pyx_L1_error)
   }
-  __pyx_t_5 = PyTuple_GET_SIZE(((PyObject*)__pyx_v_args)); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_GET_SIZE(((PyObject*)__pyx_v_args)); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 201, __pyx_L1_error)
   __pyx_t_3 = ((4 < __pyx_t_5) != 0);
   if (__pyx_t_3) {
     if (unlikely(__pyx_v_args == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 197, __pyx_L1_error)
+      __PYX_ERR(0, 201, __pyx_L1_error)
     }
     __pyx_t_6 = PyTuple_GET_ITEM(((PyObject*)__pyx_v_args), 4);
     __Pyx_INCREF(__pyx_t_6);
     __Pyx_DECREF_SET(__pyx_v_arg, __pyx_t_6);
     __pyx_t_6 = 0;
     goto __pyx_L45;
   }
@@ -12050,85 +12165,85 @@
   if (__pyx_t_4) {
   } else {
     __pyx_t_3 = __pyx_t_4;
     goto __pyx_L46_bool_binop_done;
   }
   if (unlikely(__pyx_v_kwargs == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(0, 197, __pyx_L1_error)
+    __PYX_ERR(0, 201, __pyx_L1_error)
   }
-  __pyx_t_4 = (__Pyx_PyDict_ContainsTF(__pyx_n_s_indices, ((PyObject*)__pyx_v_kwargs), Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PyDict_ContainsTF(__pyx_n_s_indices, ((PyObject*)__pyx_v_kwargs), Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 201, __pyx_L1_error)
   __pyx_t_2 = (__pyx_t_4 != 0);
   __pyx_t_3 = __pyx_t_2;
   __pyx_L46_bool_binop_done:;
   if (__pyx_t_3) {
     if (unlikely(__pyx_v_kwargs == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 197, __pyx_L1_error)
+      __PYX_ERR(0, 201, __pyx_L1_error)
     }
-    __pyx_t_6 = __Pyx_PyDict_GetItem(((PyObject*)__pyx_v_kwargs), __pyx_n_s_indices); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyDict_GetItem(((PyObject*)__pyx_v_kwargs), __pyx_n_s_indices); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 201, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF_SET(__pyx_v_arg, __pyx_t_6);
     __pyx_t_6 = 0;
     goto __pyx_L45;
   }
   /*else*/ {
     if (unlikely(__pyx_v_args == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-      __PYX_ERR(0, 197, __pyx_L1_error)
+      __PYX_ERR(0, 201, __pyx_L1_error)
     }
-    __pyx_t_5 = PyTuple_GET_SIZE(((PyObject*)__pyx_v_args)); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 197, __pyx_L1_error)
-    __pyx_t_6 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_GET_SIZE(((PyObject*)__pyx_v_args)); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 201, __pyx_L1_error)
+    __pyx_t_6 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 201, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_int_8);
     __Pyx_GIVEREF(__pyx_int_8);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_8);
     __Pyx_INCREF(__pyx_n_s_s);
     __Pyx_GIVEREF(__pyx_n_s_s);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_n_s_s);
     __Pyx_GIVEREF(__pyx_t_6);
     PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_t_6);
     __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyString_Format(__pyx_kp_s_Expected_at_least_d_argument_s_g, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyString_Format(__pyx_kp_s_Expected_at_least_d_argument_s_g, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 201, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 197, __pyx_L1_error)
+    __PYX_ERR(0, 201, __pyx_L1_error)
   }
   __pyx_L45:;
   while (1) {
     __pyx_t_3 = (__pyx_v_ndarray != ((PyTypeObject*)Py_None));
     __pyx_t_2 = (__pyx_t_3 != 0);
     if (__pyx_t_2) {
       __pyx_t_2 = __Pyx_TypeCheck(__pyx_v_arg, __pyx_v_ndarray); 
       __pyx_t_3 = (__pyx_t_2 != 0);
       if (__pyx_t_3) {
-        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_dtype); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_dtype); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_XDECREF_SET(__pyx_v_dtype, __pyx_t_1);
         __pyx_t_1 = 0;
         goto __pyx_L51;
       }
       __pyx_t_3 = __pyx_memoryview_check(__pyx_v_arg); 
       __pyx_t_2 = (__pyx_t_3 != 0);
       if (__pyx_t_2) {
-        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_XDECREF_SET(__pyx_v_arg_base, __pyx_t_1);
         __pyx_t_1 = 0;
         __pyx_t_2 = __Pyx_TypeCheck(__pyx_v_arg_base, __pyx_v_ndarray); 
         __pyx_t_3 = (__pyx_t_2 != 0);
         if (__pyx_t_3) {
-          __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg_base, __pyx_n_s_dtype); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+          __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg_base, __pyx_n_s_dtype); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_XDECREF_SET(__pyx_v_dtype, __pyx_t_1);
           __pyx_t_1 = 0;
           goto __pyx_L52;
         }
         /*else*/ {
           __Pyx_INCREF(Py_None);
@@ -12142,72 +12257,72 @@
         __Pyx_XDECREF_SET(__pyx_v_dtype, Py_None);
       }
       __pyx_L51:;
       __pyx_v_itemsize = -1L;
       __pyx_t_3 = (__pyx_v_dtype != Py_None);
       __pyx_t_2 = (__pyx_t_3 != 0);
       if (__pyx_t_2) {
-        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_dtype, __pyx_n_s_itemsize); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_dtype, __pyx_n_s_itemsize); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_1); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_1); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __pyx_v_itemsize = __pyx_t_5;
-        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_dtype, __pyx_n_s_kind); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_dtype, __pyx_n_s_kind); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_7 = __Pyx_PyObject_Ord(__pyx_t_1); if (unlikely(__pyx_t_7 == ((long)(long)(Py_UCS4)-1))) __PYX_ERR(0, 197, __pyx_L1_error)
+        __pyx_t_7 = __Pyx_PyObject_Ord(__pyx_t_1); if (unlikely(__pyx_t_7 == ((long)(long)(Py_UCS4)-1))) __PYX_ERR(0, 201, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __pyx_v_kind = __pyx_t_7;
         __pyx_v_dtype_signed = (__pyx_v_kind == 'i');
         switch (__pyx_v_kind) {
           case 'i':
           case 'u':
           __pyx_t_3 = (((sizeof(int)) == __pyx_v_itemsize) != 0);
           if (__pyx_t_3) {
           } else {
             __pyx_t_2 = __pyx_t_3;
             goto __pyx_L55_bool_binop_done;
           }
-          __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+          __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_1); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_1); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           __pyx_t_3 = ((((Py_ssize_t)__pyx_t_5) == 1) != 0);
           if (__pyx_t_3) {
           } else {
             __pyx_t_2 = __pyx_t_3;
             goto __pyx_L55_bool_binop_done;
           }
           __pyx_t_3 = ((!((__pyx_v_int_is_signed ^ __pyx_v_dtype_signed) != 0)) != 0);
           __pyx_t_2 = __pyx_t_3;
           __pyx_L55_bool_binop_done:;
           if (__pyx_t_2) {
-            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 1, __pyx_n_s_int, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 197, __pyx_L1_error)
+            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 1, __pyx_n_s_int, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 201, __pyx_L1_error)
             goto __pyx_L49_break;
           }
           __pyx_t_3 = (((sizeof(long)) == __pyx_v_itemsize) != 0);
           if (__pyx_t_3) {
           } else {
             __pyx_t_2 = __pyx_t_3;
             goto __pyx_L59_bool_binop_done;
           }
-          __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+          __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_1); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_1); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           __pyx_t_3 = ((((Py_ssize_t)__pyx_t_5) == 1) != 0);
           if (__pyx_t_3) {
           } else {
             __pyx_t_2 = __pyx_t_3;
             goto __pyx_L59_bool_binop_done;
           }
           __pyx_t_3 = ((!((__pyx_v_long_is_signed ^ __pyx_v_dtype_signed) != 0)) != 0);
           __pyx_t_2 = __pyx_t_3;
           __pyx_L59_bool_binop_done:;
           if (__pyx_t_2) {
-            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 1, __pyx_n_s_long, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 197, __pyx_L1_error)
+            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 1, __pyx_n_s_long, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 201, __pyx_L1_error)
             goto __pyx_L49_break;
           }
           break;
           case 'f':
           break;
           case 'c':
           break;
@@ -12228,15 +12343,15 @@
     __pyx_L63_bool_binop_done:;
     if (__pyx_t_2) {
       __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_ds_int(__pyx_v_arg, 0); 
       __pyx_v_memslice = __pyx_t_8;
       __pyx_t_2 = (__pyx_v_memslice.memview != 0);
       if (__pyx_t_2) {
         __PYX_XDEC_MEMVIEW((&__pyx_v_memslice), 1); 
-        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 1, __pyx_n_s_int, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 197, __pyx_L1_error)
+        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 1, __pyx_n_s_int, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 201, __pyx_L1_error)
         goto __pyx_L49_break;
       }
       /*else*/ {
         PyErr_Clear(); 
       }
     }
     __pyx_t_3 = ((__pyx_v_itemsize == -1L) != 0);
@@ -12250,35 +12365,35 @@
     __pyx_L67_bool_binop_done:;
     if (__pyx_t_2) {
       __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_ds_long(__pyx_v_arg, 0); 
       __pyx_v_memslice = __pyx_t_8;
       __pyx_t_2 = (__pyx_v_memslice.memview != 0);
       if (__pyx_t_2) {
         __PYX_XDEC_MEMVIEW((&__pyx_v_memslice), 1); 
-        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 1, __pyx_n_s_long, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 197, __pyx_L1_error)
+        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 1, __pyx_n_s_long, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 201, __pyx_L1_error)
         goto __pyx_L49_break;
       }
       /*else*/ {
         PyErr_Clear(); 
       }
     }
-    if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 1, Py_None, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 197, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 1, Py_None, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 201, __pyx_L1_error)
     goto __pyx_L49_break;
   }
   __pyx_L49_break:;
   if (unlikely(__pyx_v_args == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 197, __pyx_L1_error)
+    __PYX_ERR(0, 201, __pyx_L1_error)
   }
-  __pyx_t_5 = PyTuple_GET_SIZE(((PyObject*)__pyx_v_args)); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_GET_SIZE(((PyObject*)__pyx_v_args)); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 201, __pyx_L1_error)
   __pyx_t_2 = ((5 < __pyx_t_5) != 0);
   if (__pyx_t_2) {
     if (unlikely(__pyx_v_args == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 197, __pyx_L1_error)
+      __PYX_ERR(0, 201, __pyx_L1_error)
     }
     __pyx_t_1 = PyTuple_GET_ITEM(((PyObject*)__pyx_v_args), 5);
     __Pyx_INCREF(__pyx_t_1);
     __Pyx_DECREF_SET(__pyx_v_arg, __pyx_t_1);
     __pyx_t_1 = 0;
     goto __pyx_L70;
   }
@@ -12287,85 +12402,85 @@
   if (__pyx_t_4) {
   } else {
     __pyx_t_2 = __pyx_t_4;
     goto __pyx_L71_bool_binop_done;
   }
   if (unlikely(__pyx_v_kwargs == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(0, 197, __pyx_L1_error)
+    __PYX_ERR(0, 201, __pyx_L1_error)
   }
-  __pyx_t_4 = (__Pyx_PyDict_ContainsTF(__pyx_n_s_indptr, ((PyObject*)__pyx_v_kwargs), Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PyDict_ContainsTF(__pyx_n_s_indptr, ((PyObject*)__pyx_v_kwargs), Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 201, __pyx_L1_error)
   __pyx_t_3 = (__pyx_t_4 != 0);
   __pyx_t_2 = __pyx_t_3;
   __pyx_L71_bool_binop_done:;
   if (__pyx_t_2) {
     if (unlikely(__pyx_v_kwargs == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 197, __pyx_L1_error)
+      __PYX_ERR(0, 201, __pyx_L1_error)
     }
-    __pyx_t_1 = __Pyx_PyDict_GetItem(((PyObject*)__pyx_v_kwargs), __pyx_n_s_indptr); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyDict_GetItem(((PyObject*)__pyx_v_kwargs), __pyx_n_s_indptr); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF_SET(__pyx_v_arg, __pyx_t_1);
     __pyx_t_1 = 0;
     goto __pyx_L70;
   }
   /*else*/ {
     if (unlikely(__pyx_v_args == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-      __PYX_ERR(0, 197, __pyx_L1_error)
+      __PYX_ERR(0, 201, __pyx_L1_error)
     }
-    __pyx_t_5 = PyTuple_GET_SIZE(((PyObject*)__pyx_v_args)); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 197, __pyx_L1_error)
-    __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_GET_SIZE(((PyObject*)__pyx_v_args)); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 201, __pyx_L1_error)
+    __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 201, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_INCREF(__pyx_int_8);
     __Pyx_GIVEREF(__pyx_int_8);
     PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_int_8);
     __Pyx_INCREF(__pyx_n_s_s);
     __Pyx_GIVEREF(__pyx_n_s_s);
     PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_n_s_s);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_t_1);
     __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyString_Format(__pyx_kp_s_Expected_at_least_d_argument_s_g, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyString_Format(__pyx_kp_s_Expected_at_least_d_argument_s_g, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 201, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_6, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __PYX_ERR(0, 197, __pyx_L1_error)
+    __PYX_ERR(0, 201, __pyx_L1_error)
   }
   __pyx_L70:;
   while (1) {
     __pyx_t_2 = (__pyx_v_ndarray != ((PyTypeObject*)Py_None));
     __pyx_t_3 = (__pyx_t_2 != 0);
     if (__pyx_t_3) {
       __pyx_t_3 = __Pyx_TypeCheck(__pyx_v_arg, __pyx_v_ndarray); 
       __pyx_t_2 = (__pyx_t_3 != 0);
       if (__pyx_t_2) {
-        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_dtype); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 197, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_dtype); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 201, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_XDECREF_SET(__pyx_v_dtype, __pyx_t_6);
         __pyx_t_6 = 0;
         goto __pyx_L76;
       }
       __pyx_t_2 = __pyx_memoryview_check(__pyx_v_arg); 
       __pyx_t_3 = (__pyx_t_2 != 0);
       if (__pyx_t_3) {
-        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_base); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 197, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_base); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 201, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_XDECREF_SET(__pyx_v_arg_base, __pyx_t_6);
         __pyx_t_6 = 0;
         __pyx_t_3 = __Pyx_TypeCheck(__pyx_v_arg_base, __pyx_v_ndarray); 
         __pyx_t_2 = (__pyx_t_3 != 0);
         if (__pyx_t_2) {
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg_base, __pyx_n_s_dtype); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 197, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg_base, __pyx_n_s_dtype); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 201, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
           __Pyx_XDECREF_SET(__pyx_v_dtype, __pyx_t_6);
           __pyx_t_6 = 0;
           goto __pyx_L77;
         }
         /*else*/ {
           __Pyx_INCREF(Py_None);
@@ -12379,72 +12494,72 @@
         __Pyx_XDECREF_SET(__pyx_v_dtype, Py_None);
       }
       __pyx_L76:;
       __pyx_v_itemsize = -1L;
       __pyx_t_2 = (__pyx_v_dtype != Py_None);
       __pyx_t_3 = (__pyx_t_2 != 0);
       if (__pyx_t_3) {
-        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_dtype, __pyx_n_s_itemsize); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 197, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_dtype, __pyx_n_s_itemsize); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 201, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __pyx_v_itemsize = __pyx_t_5;
-        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_dtype, __pyx_n_s_kind); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 197, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_dtype, __pyx_n_s_kind); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 201, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_7 = __Pyx_PyObject_Ord(__pyx_t_6); if (unlikely(__pyx_t_7 == ((long)(long)(Py_UCS4)-1))) __PYX_ERR(0, 197, __pyx_L1_error)
+        __pyx_t_7 = __Pyx_PyObject_Ord(__pyx_t_6); if (unlikely(__pyx_t_7 == ((long)(long)(Py_UCS4)-1))) __PYX_ERR(0, 201, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __pyx_v_kind = __pyx_t_7;
         __pyx_v_dtype_signed = (__pyx_v_kind == 'i');
         switch (__pyx_v_kind) {
           case 'i':
           case 'u':
           __pyx_t_2 = (((sizeof(int)) == __pyx_v_itemsize) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L80_bool_binop_done;
           }
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 197, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 201, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __pyx_t_2 = ((((Py_ssize_t)__pyx_t_5) == 1) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L80_bool_binop_done;
           }
           __pyx_t_2 = ((!((__pyx_v_int_is_signed ^ __pyx_v_dtype_signed) != 0)) != 0);
           __pyx_t_3 = __pyx_t_2;
           __pyx_L80_bool_binop_done:;
           if (__pyx_t_3) {
-            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 2, __pyx_n_s_int, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 197, __pyx_L1_error)
+            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 2, __pyx_n_s_int, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 201, __pyx_L1_error)
             goto __pyx_L74_break;
           }
           __pyx_t_2 = (((sizeof(long)) == __pyx_v_itemsize) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L84_bool_binop_done;
           }
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 197, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 201, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
-          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __pyx_t_2 = ((((Py_ssize_t)__pyx_t_5) == 1) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L84_bool_binop_done;
           }
           __pyx_t_2 = ((!((__pyx_v_long_is_signed ^ __pyx_v_dtype_signed) != 0)) != 0);
           __pyx_t_3 = __pyx_t_2;
           __pyx_L84_bool_binop_done:;
           if (__pyx_t_3) {
-            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 2, __pyx_n_s_long, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 197, __pyx_L1_error)
+            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 2, __pyx_n_s_long, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 201, __pyx_L1_error)
             goto __pyx_L74_break;
           }
           break;
           case 'f':
           break;
           case 'c':
           break;
@@ -12465,15 +12580,15 @@
     __pyx_L88_bool_binop_done:;
     if (__pyx_t_3) {
       __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_ds_int(__pyx_v_arg, 0); 
       __pyx_v_memslice = __pyx_t_8;
       __pyx_t_3 = (__pyx_v_memslice.memview != 0);
       if (__pyx_t_3) {
         __PYX_XDEC_MEMVIEW((&__pyx_v_memslice), 1); 
-        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 2, __pyx_n_s_int, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 197, __pyx_L1_error)
+        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 2, __pyx_n_s_int, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 201, __pyx_L1_error)
         goto __pyx_L74_break;
       }
       /*else*/ {
         PyErr_Clear(); 
       }
     }
     __pyx_t_2 = ((__pyx_v_itemsize == -1L) != 0);
@@ -12487,100 +12602,100 @@
     __pyx_L92_bool_binop_done:;
     if (__pyx_t_3) {
       __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_ds_long(__pyx_v_arg, 0); 
       __pyx_v_memslice = __pyx_t_8;
       __pyx_t_3 = (__pyx_v_memslice.memview != 0);
       if (__pyx_t_3) {
         __PYX_XDEC_MEMVIEW((&__pyx_v_memslice), 1); 
-        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 2, __pyx_n_s_long, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 197, __pyx_L1_error)
+        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 2, __pyx_n_s_long, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 201, __pyx_L1_error)
         goto __pyx_L74_break;
       }
       /*else*/ {
         PyErr_Clear(); 
       }
     }
-    if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 2, Py_None, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 197, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 2, Py_None, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 201, __pyx_L1_error)
     goto __pyx_L74_break;
   }
   __pyx_L74_break:;
-  __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_v_candidates = ((PyObject*)__pyx_t_6);
   __pyx_t_6 = 0;
   __pyx_t_5 = 0;
   if (unlikely(__pyx_v_signatures == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(0, 197, __pyx_L1_error)
+    __PYX_ERR(0, 201, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_dict_iterator(((PyObject*)__pyx_v_signatures), 1, ((PyObject *)NULL), (&__pyx_t_9), (&__pyx_t_10)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_dict_iterator(((PyObject*)__pyx_v_signatures), 1, ((PyObject *)NULL), (&__pyx_t_9), (&__pyx_t_10)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_6);
   __pyx_t_6 = __pyx_t_1;
   __pyx_t_1 = 0;
   while (1) {
     __pyx_t_11 = __Pyx_dict_iter_next(__pyx_t_6, __pyx_t_9, &__pyx_t_5, &__pyx_t_1, NULL, NULL, __pyx_t_10);
     if (unlikely(__pyx_t_11 == 0)) break;
-    if (unlikely(__pyx_t_11 == -1)) __PYX_ERR(0, 197, __pyx_L1_error)
+    if (unlikely(__pyx_t_11 == -1)) __PYX_ERR(0, 201, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_XDECREF_SET(__pyx_v_sig, __pyx_t_1);
     __pyx_t_1 = 0;
     __pyx_v_match_found = 0;
-    __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_v_sig, __pyx_n_s_strip); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_v_sig, __pyx_n_s_strip); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 201, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_13);
     __pyx_t_14 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_13))) {
       __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_13);
       if (likely(__pyx_t_14)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_13);
         __Pyx_INCREF(__pyx_t_14);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_13, function);
       }
     }
     __pyx_t_12 = (__pyx_t_14) ? __Pyx_PyObject_Call2Args(__pyx_t_13, __pyx_t_14, __pyx_kp_s_) : __Pyx_PyObject_CallOneArg(__pyx_t_13, __pyx_kp_s_);
     __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
-    if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 197, __pyx_L1_error)
+    if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 201, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_12);
     __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-    __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_split); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_split); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 201, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_13);
     __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
     __pyx_t_12 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_13))) {
       __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_13);
       if (likely(__pyx_t_12)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_13);
         __Pyx_INCREF(__pyx_t_12);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_13, function);
       }
     }
     __pyx_t_1 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_13, __pyx_t_12, __pyx_kp_s__2) : __Pyx_PyObject_CallOneArg(__pyx_t_13, __pyx_kp_s__2);
     __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
     __Pyx_XDECREF_SET(__pyx_v_src_sig, __pyx_t_1);
     __pyx_t_1 = 0;
-    __pyx_t_15 = PyList_GET_SIZE(__pyx_v_dest_sig); if (unlikely(__pyx_t_15 == ((Py_ssize_t)-1))) __PYX_ERR(0, 197, __pyx_L1_error)
+    __pyx_t_15 = PyList_GET_SIZE(__pyx_v_dest_sig); if (unlikely(__pyx_t_15 == ((Py_ssize_t)-1))) __PYX_ERR(0, 201, __pyx_L1_error)
     __pyx_t_16 = __pyx_t_15;
     for (__pyx_t_17 = 0; __pyx_t_17 < __pyx_t_16; __pyx_t_17+=1) {
       __pyx_v_i = __pyx_t_17;
       __pyx_t_1 = PyList_GET_ITEM(__pyx_v_dest_sig, __pyx_v_i);
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_XDECREF_SET(__pyx_v_dst_type, __pyx_t_1);
       __pyx_t_1 = 0;
       __pyx_t_3 = (__pyx_v_dst_type != Py_None);
       __pyx_t_2 = (__pyx_t_3 != 0);
       if (__pyx_t_2) {
-        __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_src_sig, __pyx_v_i, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_src_sig, __pyx_v_i, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_13 = PyObject_RichCompare(__pyx_t_1, __pyx_v_dst_type, Py_EQ); __Pyx_XGOTREF(__pyx_t_13); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 197, __pyx_L1_error)
+        __pyx_t_13 = PyObject_RichCompare(__pyx_t_1, __pyx_v_dst_type, Py_EQ); __Pyx_XGOTREF(__pyx_t_13); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 201, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_13); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 197, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_13); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 201, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
         if (__pyx_t_2) {
           __pyx_v_match_found = 1;
           goto __pyx_L100;
         }
         /*else*/ {
           __pyx_v_match_found = 0;
@@ -12588,43 +12703,43 @@
         }
         __pyx_L100:;
       }
     }
     __pyx_L98_break:;
     __pyx_t_2 = (__pyx_v_match_found != 0);
     if (__pyx_t_2) {
-      __pyx_t_18 = __Pyx_PyList_Append(__pyx_v_candidates, __pyx_v_sig); if (unlikely(__pyx_t_18 == ((int)-1))) __PYX_ERR(0, 197, __pyx_L1_error)
+      __pyx_t_18 = __Pyx_PyList_Append(__pyx_v_candidates, __pyx_v_sig); if (unlikely(__pyx_t_18 == ((int)-1))) __PYX_ERR(0, 201, __pyx_L1_error)
     }
   }
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_2 = (PyList_GET_SIZE(__pyx_v_candidates) != 0);
   __pyx_t_3 = ((!__pyx_t_2) != 0);
   if (__pyx_t_3) {
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 201, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_Raise(__pyx_t_6, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __PYX_ERR(0, 197, __pyx_L1_error)
+    __PYX_ERR(0, 201, __pyx_L1_error)
   }
-  __pyx_t_9 = PyList_GET_SIZE(__pyx_v_candidates); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_9 = PyList_GET_SIZE(__pyx_v_candidates); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 201, __pyx_L1_error)
   __pyx_t_3 = ((__pyx_t_9 > 1) != 0);
   if (__pyx_t_3) {
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 201, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_Raise(__pyx_t_6, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __PYX_ERR(0, 197, __pyx_L1_error)
+    __PYX_ERR(0, 201, __pyx_L1_error)
   }
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     if (unlikely(__pyx_v_signatures == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 197, __pyx_L1_error)
+      __PYX_ERR(0, 201, __pyx_L1_error)
     }
-    __pyx_t_6 = __Pyx_PyDict_GetItem(((PyObject*)__pyx_v_signatures), PyList_GET_ITEM(__pyx_v_candidates, 0)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyDict_GetItem(((PyObject*)__pyx_v_signatures), PyList_GET_ITEM(__pyx_v_candidates, 0)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 201, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_r = __pyx_t_6;
     __pyx_t_6 = 0;
     goto __pyx_L0;
   }
 
   /* function exit code */
@@ -12651,15 +12766,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pw_9pegasusio_5cylib_2io_45__pyx_fuse_0_0_0write_dense(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_pw_9pegasusio_5cylib_2io_7write_dense(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static void __pyx_fuse_0_0_0__pyx_f_9pegasusio_5cylib_2io_write_dense(char *__pyx_v_output_file, __Pyx_memviewslice __pyx_v_barcodes, __Pyx_memviewslice __pyx_v_features, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_indices, __Pyx_memviewslice __pyx_v_indptr, int __pyx_v_M, int __pyx_v_N, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_fuse_0_0_0__pyx_opt_args_9pegasusio_5cylib_2io_write_dense *__pyx_optional_args) {
-  int __pyx_v_precision = __pyx_k__24;
+  int __pyx_v_precision = __pyx_k__25;
   FILE *__pyx_v_fo;
   PyObject *__pyx_v_fmt_str = 0;
   char const *__pyx_v_fmt;
   Py_ssize_t __pyx_v_i;
   Py_ssize_t __pyx_v_j;
   CYTHON_UNUSED Py_ssize_t __pyx_v_k;
   Py_ssize_t __pyx_v_fr;
@@ -12689,24 +12804,24 @@
   __Pyx_RefNannySetupContext("__pyx_fuse_0_0_0write_dense", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_precision = __pyx_optional_args->precision;
     }
   }
 
-  /* "ext_modules/io_funcs.pyx":200
+  /* "ext_modules/io_funcs.pyx":204
  *     """ Input must be csr_matrix internal representation, gene by cell (X.T.tocsr()); Output will be gene by cell
  *     """
  *     cdef FILE* fo = fopen(output_file, "w")             # <<<<<<<<<<<<<<
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"
  * 
  */
   __pyx_v_fo = fopen(__pyx_v_output_file, ((char const *)"w"));
 
-  /* "ext_modules/io_funcs.pyx":201
+  /* "ext_modules/io_funcs.pyx":205
  *     """
  *     cdef FILE* fo = fopen(output_file, "w")
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"             # <<<<<<<<<<<<<<
  * 
  *     cdef const char* fmt = fmt_str
  */
   __pyx_t_3 = (0 != 0);
@@ -12715,236 +12830,236 @@
     __pyx_t_2 = __pyx_t_3;
     goto __pyx_L3_bool_binop_done;
   }
   __pyx_t_3 = (0 != 0);
   __pyx_t_2 = __pyx_t_3;
   __pyx_L3_bool_binop_done:;
   if (__pyx_t_2) {
-    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = 0;
     __pyx_t_6 = 127;
-    __Pyx_INCREF(__pyx_kp_u__25);
+    __Pyx_INCREF(__pyx_kp_u__26);
     __pyx_t_5 += 3;
-    __Pyx_GIVEREF(__pyx_kp_u__25);
-    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u__25);
-    __pyx_t_7 = __Pyx_PyUnicode_From_int(__pyx_v_precision, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __Pyx_GIVEREF(__pyx_kp_u__26);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u__26);
+    __pyx_t_7 = __Pyx_PyUnicode_From_int(__pyx_v_precision, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_INCREF(__pyx_n_u_f_2);
     __pyx_t_5 += 1;
     __Pyx_GIVEREF(__pyx_n_u_f_2);
     PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_n_u_f_2);
-    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_1 = __pyx_t_7;
     __pyx_t_7 = 0;
   } else {
     __Pyx_INCREF(__pyx_kp_u_d);
     __pyx_t_1 = __pyx_kp_u_d;
   }
   __pyx_v_fmt_str = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "ext_modules/io_funcs.pyx":203
+  /* "ext_modules/io_funcs.pyx":207
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"
  * 
  *     cdef const char* fmt = fmt_str             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t i, j, k, fr
  * 
  */
-  __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_v_fmt_str); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 203, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_v_fmt_str); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 207, __pyx_L1_error)
   __pyx_v_fmt = __pyx_t_8;
 
-  /* "ext_modules/io_funcs.pyx":206
+  /* "ext_modules/io_funcs.pyx":210
  *     cdef Py_ssize_t i, j, k, fr
  * 
  *     fprintf(fo, "GENE");             # <<<<<<<<<<<<<<
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  */
   (void)(fprintf(__pyx_v_fo, ((char const *)"GENE")));
 
-  /* "ext_modules/io_funcs.pyx":207
+  /* "ext_modules/io_funcs.pyx":211
  * 
  *     fprintf(fo, "GENE");
  *     for i in range(N):             # <<<<<<<<<<<<<<
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  *     fprintf(fo, "\n")
  */
   __pyx_t_9 = __pyx_v_N;
   __pyx_t_10 = __pyx_t_9;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_10; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "ext_modules/io_funcs.pyx":208
+    /* "ext_modules/io_funcs.pyx":212
  *     fprintf(fo, "GENE");
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])             # <<<<<<<<<<<<<<
  *     fprintf(fo, "\n")
  * 
  */
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_1 = (PyObject *) *((PyObject * *) ( /* dim=0 */ (__pyx_v_barcodes.data + __pyx_t_11 * __pyx_v_barcodes.strides[0]) ));
     if (unlikely(__pyx_t_1 == NULL)) __pyx_t_1 = Py_None;
     __Pyx_INCREF((PyObject*)__pyx_t_1);
-    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 208, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 212, __pyx_L1_error)
     (void)(fprintf(__pyx_v_fo, ((char const *)"\t%s"), ((char *)__pyx_t_12)));
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
 
-  /* "ext_modules/io_funcs.pyx":209
+  /* "ext_modules/io_funcs.pyx":213
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  *     fprintf(fo, "\n")             # <<<<<<<<<<<<<<
  * 
  *     for i in range(M):
  */
   (void)(fprintf(__pyx_v_fo, ((char const *)"\n")));
 
-  /* "ext_modules/io_funcs.pyx":211
+  /* "ext_modules/io_funcs.pyx":215
  *     fprintf(fo, "\n")
  * 
  *     for i in range(M):             # <<<<<<<<<<<<<<
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0
  */
   __pyx_t_9 = __pyx_v_M;
   __pyx_t_10 = __pyx_t_9;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_10; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "ext_modules/io_funcs.pyx":212
+    /* "ext_modules/io_funcs.pyx":216
  * 
  *     for i in range(M):
  *         fprintf(fo, "%s", <char*>features[i]);             # <<<<<<<<<<<<<<
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):
  */
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_1 = (PyObject *) *((PyObject * *) ( /* dim=0 */ (__pyx_v_features.data + __pyx_t_11 * __pyx_v_features.strides[0]) ));
     if (unlikely(__pyx_t_1 == NULL)) __pyx_t_1 = Py_None;
     __Pyx_INCREF((PyObject*)__pyx_t_1);
-    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 212, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 216, __pyx_L1_error)
     (void)(fprintf(__pyx_v_fo, ((char const *)"%s"), ((char *)__pyx_t_12)));
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "ext_modules/io_funcs.pyx":213
+    /* "ext_modules/io_funcs.pyx":217
  *     for i in range(M):
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0             # <<<<<<<<<<<<<<
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):
  */
     __pyx_v_fr = 0;
 
-    /* "ext_modules/io_funcs.pyx":214
+    /* "ext_modules/io_funcs.pyx":218
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):             # <<<<<<<<<<<<<<
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")
  */
     __pyx_t_11 = (__pyx_v_i + 1);
     __pyx_t_13 = (*((int *) ( /* dim=0 */ (__pyx_v_indptr.data + __pyx_t_11 * __pyx_v_indptr.strides[0]) )));
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = (*((int *) ( /* dim=0 */ (__pyx_v_indptr.data + __pyx_t_11 * __pyx_v_indptr.strides[0]) ))); __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_j = __pyx_t_15;
 
-      /* "ext_modules/io_funcs.pyx":215
+      /* "ext_modules/io_funcs.pyx":219
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):             # <<<<<<<<<<<<<<
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])
  */
       __pyx_t_16 = __pyx_v_j;
       __pyx_t_17 = (*((int *) ( /* dim=0 */ (__pyx_v_indices.data + __pyx_t_16 * __pyx_v_indices.strides[0]) )));
       __pyx_t_18 = __pyx_t_17;
       for (__pyx_t_19 = __pyx_v_fr; __pyx_t_19 < __pyx_t_18; __pyx_t_19+=1) {
         __pyx_v_k = __pyx_t_19;
 
-        /* "ext_modules/io_funcs.pyx":216
+        /* "ext_modules/io_funcs.pyx":220
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")             # <<<<<<<<<<<<<<
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1
  */
         (void)(fprintf(__pyx_v_fo, ((char const *)"\t0")));
       }
 
-      /* "ext_modules/io_funcs.pyx":217
+      /* "ext_modules/io_funcs.pyx":221
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])             # <<<<<<<<<<<<<<
  *             fr = indices[j] + 1
  *         for k in range(fr, N):
  */
       __pyx_t_16 = __pyx_v_j;
       (void)(fprintf(__pyx_v_fo, __pyx_v_fmt, (*((int *) ( /* dim=0 */ (__pyx_v_data.data + __pyx_t_16 * __pyx_v_data.strides[0]) )))));
 
-      /* "ext_modules/io_funcs.pyx":218
+      /* "ext_modules/io_funcs.pyx":222
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1             # <<<<<<<<<<<<<<
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")
  */
       __pyx_t_16 = __pyx_v_j;
       __pyx_v_fr = ((*((int *) ( /* dim=0 */ (__pyx_v_indices.data + __pyx_t_16 * __pyx_v_indices.strides[0]) ))) + 1);
     }
 
-    /* "ext_modules/io_funcs.pyx":219
+    /* "ext_modules/io_funcs.pyx":223
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1
  *         for k in range(fr, N):             # <<<<<<<<<<<<<<
  *             fprintf(fo, "\t0")
  *         fprintf(fo, "\n")
  */
     __pyx_t_13 = __pyx_v_N;
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = __pyx_v_fr; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_k = __pyx_t_15;
 
-      /* "ext_modules/io_funcs.pyx":220
+      /* "ext_modules/io_funcs.pyx":224
  *             fr = indices[j] + 1
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")             # <<<<<<<<<<<<<<
  *         fprintf(fo, "\n")
  * 
  */
       (void)(fprintf(__pyx_v_fo, ((char const *)"\t0")));
     }
 
-    /* "ext_modules/io_funcs.pyx":221
+    /* "ext_modules/io_funcs.pyx":225
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")
  *         fprintf(fo, "\n")             # <<<<<<<<<<<<<<
  * 
  *     fclose(fo)
  */
     (void)(fprintf(__pyx_v_fo, ((char const *)"\n")));
   }
 
-  /* "ext_modules/io_funcs.pyx":223
+  /* "ext_modules/io_funcs.pyx":227
  *         fprintf(fo, "\n")
  * 
  *     fclose(fo)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   (void)(fclose(__pyx_v_fo));
 
-  /* "ext_modules/io_funcs.pyx":197
+  /* "ext_modules/io_funcs.pyx":201
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef void write_dense(char* output_file, str[:] barcodes, str[:] features, data_type[:] data, indices_type[:] indices, indptr_type[:] indptr, int M, int N, int precision = 2):             # <<<<<<<<<<<<<<
  *     """ Input must be csr_matrix internal representation, gene by cell (X.T.tocsr()); Output will be gene by cell
  *     """
  */
 
@@ -13012,61 +13127,61 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_output_file)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_barcodes)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_0_0write_dense", 0, 8, 9, 1); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_0_0write_dense", 0, 8, 9, 1); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_features)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_0_0write_dense", 0, 8, 9, 2); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_0_0write_dense", 0, 8, 9, 2); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_0_0write_dense", 0, 8, 9, 3); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_0_0write_dense", 0, 8, 9, 3); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_indices)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_0_0write_dense", 0, 8, 9, 4); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_0_0write_dense", 0, 8, 9, 4); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_indptr)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_0_0write_dense", 0, 8, 9, 5); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_0_0write_dense", 0, 8, 9, 5); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (likely((values[6] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_M)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_0_0write_dense", 0, 8, 9, 6); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_0_0write_dense", 0, 8, 9, 6); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  7:
         if (likely((values[7] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_N)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_0_0write_dense", 0, 8, 9, 7); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_0_0write_dense", 0, 8, 9, 7); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  8:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_precision);
           if (value) { values[8] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_0_0_0write_dense") < 0)) __PYX_ERR(0, 197, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_0_0_0write_dense") < 0)) __PYX_ERR(0, 201, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  9: values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
         CYTHON_FALLTHROUGH;
         case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
         values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
@@ -13076,31 +13191,31 @@
         values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_output_file = __Pyx_PyObject_AsWritableString(values[0]); if (unlikely((!__pyx_v_output_file) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_barcodes = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_barcodes.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_features = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_features.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_data = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_data.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_indices = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indices.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_indptr = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indptr.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_M = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_M == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_N = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_N == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
+    __pyx_v_output_file = __Pyx_PyObject_AsWritableString(values[0]); if (unlikely((!__pyx_v_output_file) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_barcodes = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_barcodes.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_features = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_features.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_data = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_data.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_indices = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indices.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_indptr = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indptr.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_M = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_M == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_N = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_N == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
     if (values[8]) {
-      __pyx_v_precision = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_precision == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
+      __pyx_v_precision = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_precision == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
     } else {
-      __pyx_v_precision = __pyx_k__24;
+      __pyx_v_precision = __pyx_k__25;
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_0_0write_dense", 0, 8, 9, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 197, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_0_0write_dense", 0, 8, 9, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 201, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pegasusio.cylib.io.__pyx_fuse_0_0_0write_dense", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9pegasusio_5cylib_2io_44__pyx_fuse_0_0_0write_dense(__pyx_self, __pyx_v_output_file, __pyx_v_barcodes, __pyx_v_features, __pyx_v_data, __pyx_v_indices, __pyx_v_indptr, __pyx_v_M, __pyx_v_N, __pyx_v_precision);
 
@@ -13115,23 +13230,23 @@
   struct __pyx_fuse_0_0_0__pyx_opt_args_9pegasusio_5cylib_2io_write_dense __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_0_0_0write_dense", 0);
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_barcodes.memview)) { __Pyx_RaiseUnboundLocalError("barcodes"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_features.memview)) { __Pyx_RaiseUnboundLocalError("features"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_data.memview)) { __Pyx_RaiseUnboundLocalError("data"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_indices.memview)) { __Pyx_RaiseUnboundLocalError("indices"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_indptr.memview)) { __Pyx_RaiseUnboundLocalError("indptr"); __PYX_ERR(0, 197, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_barcodes.memview)) { __Pyx_RaiseUnboundLocalError("barcodes"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_features.memview)) { __Pyx_RaiseUnboundLocalError("features"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_data.memview)) { __Pyx_RaiseUnboundLocalError("data"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_indices.memview)) { __Pyx_RaiseUnboundLocalError("indices"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_indptr.memview)) { __Pyx_RaiseUnboundLocalError("indptr"); __PYX_ERR(0, 201, __pyx_L1_error) }
   __pyx_t_1.__pyx_n = 1;
   __pyx_t_1.precision = __pyx_v_precision;
   __pyx_fuse_0_0_0__pyx_f_9pegasusio_5cylib_2io_write_dense(__pyx_v_output_file, __pyx_v_barcodes, __pyx_v_features, __pyx_v_data, __pyx_v_indices, __pyx_v_indptr, __pyx_v_M, __pyx_v_N, 0, &__pyx_t_1); 
-  __pyx_t_2 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -13148,15 +13263,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pw_9pegasusio_5cylib_2io_47__pyx_fuse_0_0_1write_dense(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_pw_9pegasusio_5cylib_2io_7write_dense(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static void __pyx_fuse_0_0_1__pyx_f_9pegasusio_5cylib_2io_write_dense(char *__pyx_v_output_file, __Pyx_memviewslice __pyx_v_barcodes, __Pyx_memviewslice __pyx_v_features, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_indices, __Pyx_memviewslice __pyx_v_indptr, int __pyx_v_M, int __pyx_v_N, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_fuse_0_0_1__pyx_opt_args_9pegasusio_5cylib_2io_write_dense *__pyx_optional_args) {
-  int __pyx_v_precision = __pyx_k__26;
+  int __pyx_v_precision = __pyx_k__27;
   FILE *__pyx_v_fo;
   PyObject *__pyx_v_fmt_str = 0;
   char const *__pyx_v_fmt;
   Py_ssize_t __pyx_v_i;
   Py_ssize_t __pyx_v_j;
   CYTHON_UNUSED Py_ssize_t __pyx_v_k;
   Py_ssize_t __pyx_v_fr;
@@ -13186,24 +13301,24 @@
   __Pyx_RefNannySetupContext("__pyx_fuse_0_0_1write_dense", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_precision = __pyx_optional_args->precision;
     }
   }
 
-  /* "ext_modules/io_funcs.pyx":200
+  /* "ext_modules/io_funcs.pyx":204
  *     """ Input must be csr_matrix internal representation, gene by cell (X.T.tocsr()); Output will be gene by cell
  *     """
  *     cdef FILE* fo = fopen(output_file, "w")             # <<<<<<<<<<<<<<
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"
  * 
  */
   __pyx_v_fo = fopen(__pyx_v_output_file, ((char const *)"w"));
 
-  /* "ext_modules/io_funcs.pyx":201
+  /* "ext_modules/io_funcs.pyx":205
  *     """
  *     cdef FILE* fo = fopen(output_file, "w")
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"             # <<<<<<<<<<<<<<
  * 
  *     cdef const char* fmt = fmt_str
  */
   __pyx_t_3 = (0 != 0);
@@ -13212,236 +13327,236 @@
     __pyx_t_2 = __pyx_t_3;
     goto __pyx_L3_bool_binop_done;
   }
   __pyx_t_3 = (0 != 0);
   __pyx_t_2 = __pyx_t_3;
   __pyx_L3_bool_binop_done:;
   if (__pyx_t_2) {
-    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = 0;
     __pyx_t_6 = 127;
-    __Pyx_INCREF(__pyx_kp_u__25);
+    __Pyx_INCREF(__pyx_kp_u__26);
     __pyx_t_5 += 3;
-    __Pyx_GIVEREF(__pyx_kp_u__25);
-    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u__25);
-    __pyx_t_7 = __Pyx_PyUnicode_From_int(__pyx_v_precision, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __Pyx_GIVEREF(__pyx_kp_u__26);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u__26);
+    __pyx_t_7 = __Pyx_PyUnicode_From_int(__pyx_v_precision, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_INCREF(__pyx_n_u_f_2);
     __pyx_t_5 += 1;
     __Pyx_GIVEREF(__pyx_n_u_f_2);
     PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_n_u_f_2);
-    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_1 = __pyx_t_7;
     __pyx_t_7 = 0;
   } else {
     __Pyx_INCREF(__pyx_kp_u_d);
     __pyx_t_1 = __pyx_kp_u_d;
   }
   __pyx_v_fmt_str = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "ext_modules/io_funcs.pyx":203
+  /* "ext_modules/io_funcs.pyx":207
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"
  * 
  *     cdef const char* fmt = fmt_str             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t i, j, k, fr
  * 
  */
-  __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_v_fmt_str); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 203, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_v_fmt_str); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 207, __pyx_L1_error)
   __pyx_v_fmt = __pyx_t_8;
 
-  /* "ext_modules/io_funcs.pyx":206
+  /* "ext_modules/io_funcs.pyx":210
  *     cdef Py_ssize_t i, j, k, fr
  * 
  *     fprintf(fo, "GENE");             # <<<<<<<<<<<<<<
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  */
   (void)(fprintf(__pyx_v_fo, ((char const *)"GENE")));
 
-  /* "ext_modules/io_funcs.pyx":207
+  /* "ext_modules/io_funcs.pyx":211
  * 
  *     fprintf(fo, "GENE");
  *     for i in range(N):             # <<<<<<<<<<<<<<
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  *     fprintf(fo, "\n")
  */
   __pyx_t_9 = __pyx_v_N;
   __pyx_t_10 = __pyx_t_9;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_10; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "ext_modules/io_funcs.pyx":208
+    /* "ext_modules/io_funcs.pyx":212
  *     fprintf(fo, "GENE");
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])             # <<<<<<<<<<<<<<
  *     fprintf(fo, "\n")
  * 
  */
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_1 = (PyObject *) *((PyObject * *) ( /* dim=0 */ (__pyx_v_barcodes.data + __pyx_t_11 * __pyx_v_barcodes.strides[0]) ));
     if (unlikely(__pyx_t_1 == NULL)) __pyx_t_1 = Py_None;
     __Pyx_INCREF((PyObject*)__pyx_t_1);
-    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 208, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 212, __pyx_L1_error)
     (void)(fprintf(__pyx_v_fo, ((char const *)"\t%s"), ((char *)__pyx_t_12)));
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
 
-  /* "ext_modules/io_funcs.pyx":209
+  /* "ext_modules/io_funcs.pyx":213
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  *     fprintf(fo, "\n")             # <<<<<<<<<<<<<<
  * 
  *     for i in range(M):
  */
   (void)(fprintf(__pyx_v_fo, ((char const *)"\n")));
 
-  /* "ext_modules/io_funcs.pyx":211
+  /* "ext_modules/io_funcs.pyx":215
  *     fprintf(fo, "\n")
  * 
  *     for i in range(M):             # <<<<<<<<<<<<<<
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0
  */
   __pyx_t_9 = __pyx_v_M;
   __pyx_t_10 = __pyx_t_9;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_10; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "ext_modules/io_funcs.pyx":212
+    /* "ext_modules/io_funcs.pyx":216
  * 
  *     for i in range(M):
  *         fprintf(fo, "%s", <char*>features[i]);             # <<<<<<<<<<<<<<
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):
  */
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_1 = (PyObject *) *((PyObject * *) ( /* dim=0 */ (__pyx_v_features.data + __pyx_t_11 * __pyx_v_features.strides[0]) ));
     if (unlikely(__pyx_t_1 == NULL)) __pyx_t_1 = Py_None;
     __Pyx_INCREF((PyObject*)__pyx_t_1);
-    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 212, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 216, __pyx_L1_error)
     (void)(fprintf(__pyx_v_fo, ((char const *)"%s"), ((char *)__pyx_t_12)));
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "ext_modules/io_funcs.pyx":213
+    /* "ext_modules/io_funcs.pyx":217
  *     for i in range(M):
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0             # <<<<<<<<<<<<<<
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):
  */
     __pyx_v_fr = 0;
 
-    /* "ext_modules/io_funcs.pyx":214
+    /* "ext_modules/io_funcs.pyx":218
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):             # <<<<<<<<<<<<<<
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")
  */
     __pyx_t_11 = (__pyx_v_i + 1);
     __pyx_t_13 = (*((long *) ( /* dim=0 */ (__pyx_v_indptr.data + __pyx_t_11 * __pyx_v_indptr.strides[0]) )));
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = (*((long *) ( /* dim=0 */ (__pyx_v_indptr.data + __pyx_t_11 * __pyx_v_indptr.strides[0]) ))); __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_j = __pyx_t_15;
 
-      /* "ext_modules/io_funcs.pyx":215
+      /* "ext_modules/io_funcs.pyx":219
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):             # <<<<<<<<<<<<<<
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])
  */
       __pyx_t_16 = __pyx_v_j;
       __pyx_t_17 = (*((int *) ( /* dim=0 */ (__pyx_v_indices.data + __pyx_t_16 * __pyx_v_indices.strides[0]) )));
       __pyx_t_18 = __pyx_t_17;
       for (__pyx_t_19 = __pyx_v_fr; __pyx_t_19 < __pyx_t_18; __pyx_t_19+=1) {
         __pyx_v_k = __pyx_t_19;
 
-        /* "ext_modules/io_funcs.pyx":216
+        /* "ext_modules/io_funcs.pyx":220
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")             # <<<<<<<<<<<<<<
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1
  */
         (void)(fprintf(__pyx_v_fo, ((char const *)"\t0")));
       }
 
-      /* "ext_modules/io_funcs.pyx":217
+      /* "ext_modules/io_funcs.pyx":221
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])             # <<<<<<<<<<<<<<
  *             fr = indices[j] + 1
  *         for k in range(fr, N):
  */
       __pyx_t_16 = __pyx_v_j;
       (void)(fprintf(__pyx_v_fo, __pyx_v_fmt, (*((int *) ( /* dim=0 */ (__pyx_v_data.data + __pyx_t_16 * __pyx_v_data.strides[0]) )))));
 
-      /* "ext_modules/io_funcs.pyx":218
+      /* "ext_modules/io_funcs.pyx":222
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1             # <<<<<<<<<<<<<<
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")
  */
       __pyx_t_16 = __pyx_v_j;
       __pyx_v_fr = ((*((int *) ( /* dim=0 */ (__pyx_v_indices.data + __pyx_t_16 * __pyx_v_indices.strides[0]) ))) + 1);
     }
 
-    /* "ext_modules/io_funcs.pyx":219
+    /* "ext_modules/io_funcs.pyx":223
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1
  *         for k in range(fr, N):             # <<<<<<<<<<<<<<
  *             fprintf(fo, "\t0")
  *         fprintf(fo, "\n")
  */
     __pyx_t_17 = __pyx_v_N;
     __pyx_t_18 = __pyx_t_17;
     for (__pyx_t_15 = __pyx_v_fr; __pyx_t_15 < __pyx_t_18; __pyx_t_15+=1) {
       __pyx_v_k = __pyx_t_15;
 
-      /* "ext_modules/io_funcs.pyx":220
+      /* "ext_modules/io_funcs.pyx":224
  *             fr = indices[j] + 1
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")             # <<<<<<<<<<<<<<
  *         fprintf(fo, "\n")
  * 
  */
       (void)(fprintf(__pyx_v_fo, ((char const *)"\t0")));
     }
 
-    /* "ext_modules/io_funcs.pyx":221
+    /* "ext_modules/io_funcs.pyx":225
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")
  *         fprintf(fo, "\n")             # <<<<<<<<<<<<<<
  * 
  *     fclose(fo)
  */
     (void)(fprintf(__pyx_v_fo, ((char const *)"\n")));
   }
 
-  /* "ext_modules/io_funcs.pyx":223
+  /* "ext_modules/io_funcs.pyx":227
  *         fprintf(fo, "\n")
  * 
  *     fclose(fo)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   (void)(fclose(__pyx_v_fo));
 
-  /* "ext_modules/io_funcs.pyx":197
+  /* "ext_modules/io_funcs.pyx":201
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef void write_dense(char* output_file, str[:] barcodes, str[:] features, data_type[:] data, indices_type[:] indices, indptr_type[:] indptr, int M, int N, int precision = 2):             # <<<<<<<<<<<<<<
  *     """ Input must be csr_matrix internal representation, gene by cell (X.T.tocsr()); Output will be gene by cell
  *     """
  */
 
@@ -13509,61 +13624,61 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_output_file)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_barcodes)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_0_1write_dense", 0, 8, 9, 1); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_0_1write_dense", 0, 8, 9, 1); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_features)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_0_1write_dense", 0, 8, 9, 2); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_0_1write_dense", 0, 8, 9, 2); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_0_1write_dense", 0, 8, 9, 3); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_0_1write_dense", 0, 8, 9, 3); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_indices)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_0_1write_dense", 0, 8, 9, 4); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_0_1write_dense", 0, 8, 9, 4); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_indptr)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_0_1write_dense", 0, 8, 9, 5); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_0_1write_dense", 0, 8, 9, 5); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (likely((values[6] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_M)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_0_1write_dense", 0, 8, 9, 6); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_0_1write_dense", 0, 8, 9, 6); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  7:
         if (likely((values[7] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_N)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_0_1write_dense", 0, 8, 9, 7); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_0_1write_dense", 0, 8, 9, 7); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  8:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_precision);
           if (value) { values[8] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_0_0_1write_dense") < 0)) __PYX_ERR(0, 197, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_0_0_1write_dense") < 0)) __PYX_ERR(0, 201, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  9: values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
         CYTHON_FALLTHROUGH;
         case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
         values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
@@ -13573,31 +13688,31 @@
         values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_output_file = __Pyx_PyObject_AsWritableString(values[0]); if (unlikely((!__pyx_v_output_file) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_barcodes = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_barcodes.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_features = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_features.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_data = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_data.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_indices = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indices.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_indptr = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indptr.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_M = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_M == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_N = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_N == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
+    __pyx_v_output_file = __Pyx_PyObject_AsWritableString(values[0]); if (unlikely((!__pyx_v_output_file) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_barcodes = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_barcodes.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_features = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_features.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_data = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_data.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_indices = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indices.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_indptr = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indptr.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_M = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_M == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_N = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_N == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
     if (values[8]) {
-      __pyx_v_precision = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_precision == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
+      __pyx_v_precision = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_precision == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
     } else {
-      __pyx_v_precision = __pyx_k__26;
+      __pyx_v_precision = __pyx_k__27;
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_0_1write_dense", 0, 8, 9, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 197, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_0_1write_dense", 0, 8, 9, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 201, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pegasusio.cylib.io.__pyx_fuse_0_0_1write_dense", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9pegasusio_5cylib_2io_46__pyx_fuse_0_0_1write_dense(__pyx_self, __pyx_v_output_file, __pyx_v_barcodes, __pyx_v_features, __pyx_v_data, __pyx_v_indices, __pyx_v_indptr, __pyx_v_M, __pyx_v_N, __pyx_v_precision);
 
@@ -13612,23 +13727,23 @@
   struct __pyx_fuse_0_0_1__pyx_opt_args_9pegasusio_5cylib_2io_write_dense __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_0_0_1write_dense", 0);
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_barcodes.memview)) { __Pyx_RaiseUnboundLocalError("barcodes"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_features.memview)) { __Pyx_RaiseUnboundLocalError("features"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_data.memview)) { __Pyx_RaiseUnboundLocalError("data"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_indices.memview)) { __Pyx_RaiseUnboundLocalError("indices"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_indptr.memview)) { __Pyx_RaiseUnboundLocalError("indptr"); __PYX_ERR(0, 197, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_barcodes.memview)) { __Pyx_RaiseUnboundLocalError("barcodes"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_features.memview)) { __Pyx_RaiseUnboundLocalError("features"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_data.memview)) { __Pyx_RaiseUnboundLocalError("data"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_indices.memview)) { __Pyx_RaiseUnboundLocalError("indices"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_indptr.memview)) { __Pyx_RaiseUnboundLocalError("indptr"); __PYX_ERR(0, 201, __pyx_L1_error) }
   __pyx_t_1.__pyx_n = 1;
   __pyx_t_1.precision = __pyx_v_precision;
   __pyx_fuse_0_0_1__pyx_f_9pegasusio_5cylib_2io_write_dense(__pyx_v_output_file, __pyx_v_barcodes, __pyx_v_features, __pyx_v_data, __pyx_v_indices, __pyx_v_indptr, __pyx_v_M, __pyx_v_N, 0, &__pyx_t_1); 
-  __pyx_t_2 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -13645,15 +13760,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pw_9pegasusio_5cylib_2io_49__pyx_fuse_0_1_0write_dense(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_pw_9pegasusio_5cylib_2io_7write_dense(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static void __pyx_fuse_0_1_0__pyx_f_9pegasusio_5cylib_2io_write_dense(char *__pyx_v_output_file, __Pyx_memviewslice __pyx_v_barcodes, __Pyx_memviewslice __pyx_v_features, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_indices, __Pyx_memviewslice __pyx_v_indptr, int __pyx_v_M, int __pyx_v_N, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_fuse_0_1_0__pyx_opt_args_9pegasusio_5cylib_2io_write_dense *__pyx_optional_args) {
-  int __pyx_v_precision = __pyx_k__27;
+  int __pyx_v_precision = __pyx_k__28;
   FILE *__pyx_v_fo;
   PyObject *__pyx_v_fmt_str = 0;
   char const *__pyx_v_fmt;
   Py_ssize_t __pyx_v_i;
   Py_ssize_t __pyx_v_j;
   CYTHON_UNUSED Py_ssize_t __pyx_v_k;
   Py_ssize_t __pyx_v_fr;
@@ -13683,24 +13798,24 @@
   __Pyx_RefNannySetupContext("__pyx_fuse_0_1_0write_dense", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_precision = __pyx_optional_args->precision;
     }
   }
 
-  /* "ext_modules/io_funcs.pyx":200
+  /* "ext_modules/io_funcs.pyx":204
  *     """ Input must be csr_matrix internal representation, gene by cell (X.T.tocsr()); Output will be gene by cell
  *     """
  *     cdef FILE* fo = fopen(output_file, "w")             # <<<<<<<<<<<<<<
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"
  * 
  */
   __pyx_v_fo = fopen(__pyx_v_output_file, ((char const *)"w"));
 
-  /* "ext_modules/io_funcs.pyx":201
+  /* "ext_modules/io_funcs.pyx":205
  *     """
  *     cdef FILE* fo = fopen(output_file, "w")
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"             # <<<<<<<<<<<<<<
  * 
  *     cdef const char* fmt = fmt_str
  */
   __pyx_t_3 = (0 != 0);
@@ -13709,236 +13824,236 @@
     __pyx_t_2 = __pyx_t_3;
     goto __pyx_L3_bool_binop_done;
   }
   __pyx_t_3 = (0 != 0);
   __pyx_t_2 = __pyx_t_3;
   __pyx_L3_bool_binop_done:;
   if (__pyx_t_2) {
-    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = 0;
     __pyx_t_6 = 127;
-    __Pyx_INCREF(__pyx_kp_u__25);
+    __Pyx_INCREF(__pyx_kp_u__26);
     __pyx_t_5 += 3;
-    __Pyx_GIVEREF(__pyx_kp_u__25);
-    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u__25);
-    __pyx_t_7 = __Pyx_PyUnicode_From_int(__pyx_v_precision, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __Pyx_GIVEREF(__pyx_kp_u__26);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u__26);
+    __pyx_t_7 = __Pyx_PyUnicode_From_int(__pyx_v_precision, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_INCREF(__pyx_n_u_f_2);
     __pyx_t_5 += 1;
     __Pyx_GIVEREF(__pyx_n_u_f_2);
     PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_n_u_f_2);
-    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_1 = __pyx_t_7;
     __pyx_t_7 = 0;
   } else {
     __Pyx_INCREF(__pyx_kp_u_d);
     __pyx_t_1 = __pyx_kp_u_d;
   }
   __pyx_v_fmt_str = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "ext_modules/io_funcs.pyx":203
+  /* "ext_modules/io_funcs.pyx":207
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"
  * 
  *     cdef const char* fmt = fmt_str             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t i, j, k, fr
  * 
  */
-  __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_v_fmt_str); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 203, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_v_fmt_str); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 207, __pyx_L1_error)
   __pyx_v_fmt = __pyx_t_8;
 
-  /* "ext_modules/io_funcs.pyx":206
+  /* "ext_modules/io_funcs.pyx":210
  *     cdef Py_ssize_t i, j, k, fr
  * 
  *     fprintf(fo, "GENE");             # <<<<<<<<<<<<<<
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  */
   (void)(fprintf(__pyx_v_fo, ((char const *)"GENE")));
 
-  /* "ext_modules/io_funcs.pyx":207
+  /* "ext_modules/io_funcs.pyx":211
  * 
  *     fprintf(fo, "GENE");
  *     for i in range(N):             # <<<<<<<<<<<<<<
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  *     fprintf(fo, "\n")
  */
   __pyx_t_9 = __pyx_v_N;
   __pyx_t_10 = __pyx_t_9;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_10; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "ext_modules/io_funcs.pyx":208
+    /* "ext_modules/io_funcs.pyx":212
  *     fprintf(fo, "GENE");
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])             # <<<<<<<<<<<<<<
  *     fprintf(fo, "\n")
  * 
  */
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_1 = (PyObject *) *((PyObject * *) ( /* dim=0 */ (__pyx_v_barcodes.data + __pyx_t_11 * __pyx_v_barcodes.strides[0]) ));
     if (unlikely(__pyx_t_1 == NULL)) __pyx_t_1 = Py_None;
     __Pyx_INCREF((PyObject*)__pyx_t_1);
-    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 208, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 212, __pyx_L1_error)
     (void)(fprintf(__pyx_v_fo, ((char const *)"\t%s"), ((char *)__pyx_t_12)));
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
 
-  /* "ext_modules/io_funcs.pyx":209
+  /* "ext_modules/io_funcs.pyx":213
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  *     fprintf(fo, "\n")             # <<<<<<<<<<<<<<
  * 
  *     for i in range(M):
  */
   (void)(fprintf(__pyx_v_fo, ((char const *)"\n")));
 
-  /* "ext_modules/io_funcs.pyx":211
+  /* "ext_modules/io_funcs.pyx":215
  *     fprintf(fo, "\n")
  * 
  *     for i in range(M):             # <<<<<<<<<<<<<<
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0
  */
   __pyx_t_9 = __pyx_v_M;
   __pyx_t_10 = __pyx_t_9;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_10; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "ext_modules/io_funcs.pyx":212
+    /* "ext_modules/io_funcs.pyx":216
  * 
  *     for i in range(M):
  *         fprintf(fo, "%s", <char*>features[i]);             # <<<<<<<<<<<<<<
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):
  */
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_1 = (PyObject *) *((PyObject * *) ( /* dim=0 */ (__pyx_v_features.data + __pyx_t_11 * __pyx_v_features.strides[0]) ));
     if (unlikely(__pyx_t_1 == NULL)) __pyx_t_1 = Py_None;
     __Pyx_INCREF((PyObject*)__pyx_t_1);
-    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 212, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 216, __pyx_L1_error)
     (void)(fprintf(__pyx_v_fo, ((char const *)"%s"), ((char *)__pyx_t_12)));
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "ext_modules/io_funcs.pyx":213
+    /* "ext_modules/io_funcs.pyx":217
  *     for i in range(M):
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0             # <<<<<<<<<<<<<<
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):
  */
     __pyx_v_fr = 0;
 
-    /* "ext_modules/io_funcs.pyx":214
+    /* "ext_modules/io_funcs.pyx":218
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):             # <<<<<<<<<<<<<<
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")
  */
     __pyx_t_11 = (__pyx_v_i + 1);
     __pyx_t_13 = (*((int *) ( /* dim=0 */ (__pyx_v_indptr.data + __pyx_t_11 * __pyx_v_indptr.strides[0]) )));
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = (*((int *) ( /* dim=0 */ (__pyx_v_indptr.data + __pyx_t_11 * __pyx_v_indptr.strides[0]) ))); __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_j = __pyx_t_15;
 
-      /* "ext_modules/io_funcs.pyx":215
+      /* "ext_modules/io_funcs.pyx":219
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):             # <<<<<<<<<<<<<<
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])
  */
       __pyx_t_16 = __pyx_v_j;
       __pyx_t_17 = (*((long *) ( /* dim=0 */ (__pyx_v_indices.data + __pyx_t_16 * __pyx_v_indices.strides[0]) )));
       __pyx_t_18 = __pyx_t_17;
       for (__pyx_t_19 = __pyx_v_fr; __pyx_t_19 < __pyx_t_18; __pyx_t_19+=1) {
         __pyx_v_k = __pyx_t_19;
 
-        /* "ext_modules/io_funcs.pyx":216
+        /* "ext_modules/io_funcs.pyx":220
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")             # <<<<<<<<<<<<<<
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1
  */
         (void)(fprintf(__pyx_v_fo, ((char const *)"\t0")));
       }
 
-      /* "ext_modules/io_funcs.pyx":217
+      /* "ext_modules/io_funcs.pyx":221
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])             # <<<<<<<<<<<<<<
  *             fr = indices[j] + 1
  *         for k in range(fr, N):
  */
       __pyx_t_16 = __pyx_v_j;
       (void)(fprintf(__pyx_v_fo, __pyx_v_fmt, (*((int *) ( /* dim=0 */ (__pyx_v_data.data + __pyx_t_16 * __pyx_v_data.strides[0]) )))));
 
-      /* "ext_modules/io_funcs.pyx":218
+      /* "ext_modules/io_funcs.pyx":222
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1             # <<<<<<<<<<<<<<
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")
  */
       __pyx_t_16 = __pyx_v_j;
       __pyx_v_fr = ((*((long *) ( /* dim=0 */ (__pyx_v_indices.data + __pyx_t_16 * __pyx_v_indices.strides[0]) ))) + 1);
     }
 
-    /* "ext_modules/io_funcs.pyx":219
+    /* "ext_modules/io_funcs.pyx":223
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1
  *         for k in range(fr, N):             # <<<<<<<<<<<<<<
  *             fprintf(fo, "\t0")
  *         fprintf(fo, "\n")
  */
     __pyx_t_13 = __pyx_v_N;
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = __pyx_v_fr; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_k = __pyx_t_15;
 
-      /* "ext_modules/io_funcs.pyx":220
+      /* "ext_modules/io_funcs.pyx":224
  *             fr = indices[j] + 1
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")             # <<<<<<<<<<<<<<
  *         fprintf(fo, "\n")
  * 
  */
       (void)(fprintf(__pyx_v_fo, ((char const *)"\t0")));
     }
 
-    /* "ext_modules/io_funcs.pyx":221
+    /* "ext_modules/io_funcs.pyx":225
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")
  *         fprintf(fo, "\n")             # <<<<<<<<<<<<<<
  * 
  *     fclose(fo)
  */
     (void)(fprintf(__pyx_v_fo, ((char const *)"\n")));
   }
 
-  /* "ext_modules/io_funcs.pyx":223
+  /* "ext_modules/io_funcs.pyx":227
  *         fprintf(fo, "\n")
  * 
  *     fclose(fo)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   (void)(fclose(__pyx_v_fo));
 
-  /* "ext_modules/io_funcs.pyx":197
+  /* "ext_modules/io_funcs.pyx":201
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef void write_dense(char* output_file, str[:] barcodes, str[:] features, data_type[:] data, indices_type[:] indices, indptr_type[:] indptr, int M, int N, int precision = 2):             # <<<<<<<<<<<<<<
  *     """ Input must be csr_matrix internal representation, gene by cell (X.T.tocsr()); Output will be gene by cell
  *     """
  */
 
@@ -14006,61 +14121,61 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_output_file)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_barcodes)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_1_0write_dense", 0, 8, 9, 1); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_1_0write_dense", 0, 8, 9, 1); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_features)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_1_0write_dense", 0, 8, 9, 2); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_1_0write_dense", 0, 8, 9, 2); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_1_0write_dense", 0, 8, 9, 3); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_1_0write_dense", 0, 8, 9, 3); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_indices)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_1_0write_dense", 0, 8, 9, 4); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_1_0write_dense", 0, 8, 9, 4); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_indptr)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_1_0write_dense", 0, 8, 9, 5); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_1_0write_dense", 0, 8, 9, 5); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (likely((values[6] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_M)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_1_0write_dense", 0, 8, 9, 6); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_1_0write_dense", 0, 8, 9, 6); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  7:
         if (likely((values[7] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_N)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_1_0write_dense", 0, 8, 9, 7); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_1_0write_dense", 0, 8, 9, 7); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  8:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_precision);
           if (value) { values[8] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_0_1_0write_dense") < 0)) __PYX_ERR(0, 197, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_0_1_0write_dense") < 0)) __PYX_ERR(0, 201, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  9: values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
         CYTHON_FALLTHROUGH;
         case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
         values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
@@ -14070,31 +14185,31 @@
         values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_output_file = __Pyx_PyObject_AsWritableString(values[0]); if (unlikely((!__pyx_v_output_file) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_barcodes = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_barcodes.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_features = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_features.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_data = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_data.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_indices = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indices.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_indptr = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indptr.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_M = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_M == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_N = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_N == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
+    __pyx_v_output_file = __Pyx_PyObject_AsWritableString(values[0]); if (unlikely((!__pyx_v_output_file) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_barcodes = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_barcodes.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_features = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_features.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_data = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_data.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_indices = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indices.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_indptr = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indptr.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_M = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_M == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_N = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_N == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
     if (values[8]) {
-      __pyx_v_precision = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_precision == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
+      __pyx_v_precision = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_precision == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
     } else {
-      __pyx_v_precision = __pyx_k__27;
+      __pyx_v_precision = __pyx_k__28;
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_1_0write_dense", 0, 8, 9, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 197, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_1_0write_dense", 0, 8, 9, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 201, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pegasusio.cylib.io.__pyx_fuse_0_1_0write_dense", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9pegasusio_5cylib_2io_48__pyx_fuse_0_1_0write_dense(__pyx_self, __pyx_v_output_file, __pyx_v_barcodes, __pyx_v_features, __pyx_v_data, __pyx_v_indices, __pyx_v_indptr, __pyx_v_M, __pyx_v_N, __pyx_v_precision);
 
@@ -14109,23 +14224,23 @@
   struct __pyx_fuse_0_1_0__pyx_opt_args_9pegasusio_5cylib_2io_write_dense __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_0_1_0write_dense", 0);
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_barcodes.memview)) { __Pyx_RaiseUnboundLocalError("barcodes"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_features.memview)) { __Pyx_RaiseUnboundLocalError("features"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_data.memview)) { __Pyx_RaiseUnboundLocalError("data"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_indices.memview)) { __Pyx_RaiseUnboundLocalError("indices"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_indptr.memview)) { __Pyx_RaiseUnboundLocalError("indptr"); __PYX_ERR(0, 197, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_barcodes.memview)) { __Pyx_RaiseUnboundLocalError("barcodes"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_features.memview)) { __Pyx_RaiseUnboundLocalError("features"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_data.memview)) { __Pyx_RaiseUnboundLocalError("data"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_indices.memview)) { __Pyx_RaiseUnboundLocalError("indices"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_indptr.memview)) { __Pyx_RaiseUnboundLocalError("indptr"); __PYX_ERR(0, 201, __pyx_L1_error) }
   __pyx_t_1.__pyx_n = 1;
   __pyx_t_1.precision = __pyx_v_precision;
   __pyx_fuse_0_1_0__pyx_f_9pegasusio_5cylib_2io_write_dense(__pyx_v_output_file, __pyx_v_barcodes, __pyx_v_features, __pyx_v_data, __pyx_v_indices, __pyx_v_indptr, __pyx_v_M, __pyx_v_N, 0, &__pyx_t_1); 
-  __pyx_t_2 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -14142,15 +14257,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pw_9pegasusio_5cylib_2io_51__pyx_fuse_0_1_1write_dense(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_pw_9pegasusio_5cylib_2io_7write_dense(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static void __pyx_fuse_0_1_1__pyx_f_9pegasusio_5cylib_2io_write_dense(char *__pyx_v_output_file, __Pyx_memviewslice __pyx_v_barcodes, __Pyx_memviewslice __pyx_v_features, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_indices, __Pyx_memviewslice __pyx_v_indptr, int __pyx_v_M, int __pyx_v_N, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_fuse_0_1_1__pyx_opt_args_9pegasusio_5cylib_2io_write_dense *__pyx_optional_args) {
-  int __pyx_v_precision = __pyx_k__28;
+  int __pyx_v_precision = __pyx_k__29;
   FILE *__pyx_v_fo;
   PyObject *__pyx_v_fmt_str = 0;
   char const *__pyx_v_fmt;
   Py_ssize_t __pyx_v_i;
   Py_ssize_t __pyx_v_j;
   CYTHON_UNUSED Py_ssize_t __pyx_v_k;
   Py_ssize_t __pyx_v_fr;
@@ -14182,24 +14297,24 @@
   __Pyx_RefNannySetupContext("__pyx_fuse_0_1_1write_dense", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_precision = __pyx_optional_args->precision;
     }
   }
 
-  /* "ext_modules/io_funcs.pyx":200
+  /* "ext_modules/io_funcs.pyx":204
  *     """ Input must be csr_matrix internal representation, gene by cell (X.T.tocsr()); Output will be gene by cell
  *     """
  *     cdef FILE* fo = fopen(output_file, "w")             # <<<<<<<<<<<<<<
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"
  * 
  */
   __pyx_v_fo = fopen(__pyx_v_output_file, ((char const *)"w"));
 
-  /* "ext_modules/io_funcs.pyx":201
+  /* "ext_modules/io_funcs.pyx":205
  *     """
  *     cdef FILE* fo = fopen(output_file, "w")
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"             # <<<<<<<<<<<<<<
  * 
  *     cdef const char* fmt = fmt_str
  */
   __pyx_t_3 = (0 != 0);
@@ -14208,236 +14323,236 @@
     __pyx_t_2 = __pyx_t_3;
     goto __pyx_L3_bool_binop_done;
   }
   __pyx_t_3 = (0 != 0);
   __pyx_t_2 = __pyx_t_3;
   __pyx_L3_bool_binop_done:;
   if (__pyx_t_2) {
-    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = 0;
     __pyx_t_6 = 127;
-    __Pyx_INCREF(__pyx_kp_u__25);
+    __Pyx_INCREF(__pyx_kp_u__26);
     __pyx_t_5 += 3;
-    __Pyx_GIVEREF(__pyx_kp_u__25);
-    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u__25);
-    __pyx_t_7 = __Pyx_PyUnicode_From_int(__pyx_v_precision, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __Pyx_GIVEREF(__pyx_kp_u__26);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u__26);
+    __pyx_t_7 = __Pyx_PyUnicode_From_int(__pyx_v_precision, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_INCREF(__pyx_n_u_f_2);
     __pyx_t_5 += 1;
     __Pyx_GIVEREF(__pyx_n_u_f_2);
     PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_n_u_f_2);
-    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_1 = __pyx_t_7;
     __pyx_t_7 = 0;
   } else {
     __Pyx_INCREF(__pyx_kp_u_d);
     __pyx_t_1 = __pyx_kp_u_d;
   }
   __pyx_v_fmt_str = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "ext_modules/io_funcs.pyx":203
+  /* "ext_modules/io_funcs.pyx":207
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"
  * 
  *     cdef const char* fmt = fmt_str             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t i, j, k, fr
  * 
  */
-  __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_v_fmt_str); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 203, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_v_fmt_str); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 207, __pyx_L1_error)
   __pyx_v_fmt = __pyx_t_8;
 
-  /* "ext_modules/io_funcs.pyx":206
+  /* "ext_modules/io_funcs.pyx":210
  *     cdef Py_ssize_t i, j, k, fr
  * 
  *     fprintf(fo, "GENE");             # <<<<<<<<<<<<<<
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  */
   (void)(fprintf(__pyx_v_fo, ((char const *)"GENE")));
 
-  /* "ext_modules/io_funcs.pyx":207
+  /* "ext_modules/io_funcs.pyx":211
  * 
  *     fprintf(fo, "GENE");
  *     for i in range(N):             # <<<<<<<<<<<<<<
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  *     fprintf(fo, "\n")
  */
   __pyx_t_9 = __pyx_v_N;
   __pyx_t_10 = __pyx_t_9;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_10; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "ext_modules/io_funcs.pyx":208
+    /* "ext_modules/io_funcs.pyx":212
  *     fprintf(fo, "GENE");
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])             # <<<<<<<<<<<<<<
  *     fprintf(fo, "\n")
  * 
  */
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_1 = (PyObject *) *((PyObject * *) ( /* dim=0 */ (__pyx_v_barcodes.data + __pyx_t_11 * __pyx_v_barcodes.strides[0]) ));
     if (unlikely(__pyx_t_1 == NULL)) __pyx_t_1 = Py_None;
     __Pyx_INCREF((PyObject*)__pyx_t_1);
-    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 208, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 212, __pyx_L1_error)
     (void)(fprintf(__pyx_v_fo, ((char const *)"\t%s"), ((char *)__pyx_t_12)));
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
 
-  /* "ext_modules/io_funcs.pyx":209
+  /* "ext_modules/io_funcs.pyx":213
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  *     fprintf(fo, "\n")             # <<<<<<<<<<<<<<
  * 
  *     for i in range(M):
  */
   (void)(fprintf(__pyx_v_fo, ((char const *)"\n")));
 
-  /* "ext_modules/io_funcs.pyx":211
+  /* "ext_modules/io_funcs.pyx":215
  *     fprintf(fo, "\n")
  * 
  *     for i in range(M):             # <<<<<<<<<<<<<<
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0
  */
   __pyx_t_9 = __pyx_v_M;
   __pyx_t_10 = __pyx_t_9;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_10; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "ext_modules/io_funcs.pyx":212
+    /* "ext_modules/io_funcs.pyx":216
  * 
  *     for i in range(M):
  *         fprintf(fo, "%s", <char*>features[i]);             # <<<<<<<<<<<<<<
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):
  */
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_1 = (PyObject *) *((PyObject * *) ( /* dim=0 */ (__pyx_v_features.data + __pyx_t_11 * __pyx_v_features.strides[0]) ));
     if (unlikely(__pyx_t_1 == NULL)) __pyx_t_1 = Py_None;
     __Pyx_INCREF((PyObject*)__pyx_t_1);
-    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 212, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 216, __pyx_L1_error)
     (void)(fprintf(__pyx_v_fo, ((char const *)"%s"), ((char *)__pyx_t_12)));
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "ext_modules/io_funcs.pyx":213
+    /* "ext_modules/io_funcs.pyx":217
  *     for i in range(M):
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0             # <<<<<<<<<<<<<<
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):
  */
     __pyx_v_fr = 0;
 
-    /* "ext_modules/io_funcs.pyx":214
+    /* "ext_modules/io_funcs.pyx":218
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):             # <<<<<<<<<<<<<<
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")
  */
     __pyx_t_11 = (__pyx_v_i + 1);
     __pyx_t_13 = (*((long *) ( /* dim=0 */ (__pyx_v_indptr.data + __pyx_t_11 * __pyx_v_indptr.strides[0]) )));
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = (*((long *) ( /* dim=0 */ (__pyx_v_indptr.data + __pyx_t_11 * __pyx_v_indptr.strides[0]) ))); __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_j = __pyx_t_15;
 
-      /* "ext_modules/io_funcs.pyx":215
+      /* "ext_modules/io_funcs.pyx":219
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):             # <<<<<<<<<<<<<<
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])
  */
       __pyx_t_16 = __pyx_v_j;
       __pyx_t_17 = (*((long *) ( /* dim=0 */ (__pyx_v_indices.data + __pyx_t_16 * __pyx_v_indices.strides[0]) )));
       __pyx_t_18 = __pyx_t_17;
       for (__pyx_t_19 = __pyx_v_fr; __pyx_t_19 < __pyx_t_18; __pyx_t_19+=1) {
         __pyx_v_k = __pyx_t_19;
 
-        /* "ext_modules/io_funcs.pyx":216
+        /* "ext_modules/io_funcs.pyx":220
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")             # <<<<<<<<<<<<<<
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1
  */
         (void)(fprintf(__pyx_v_fo, ((char const *)"\t0")));
       }
 
-      /* "ext_modules/io_funcs.pyx":217
+      /* "ext_modules/io_funcs.pyx":221
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])             # <<<<<<<<<<<<<<
  *             fr = indices[j] + 1
  *         for k in range(fr, N):
  */
       __pyx_t_16 = __pyx_v_j;
       (void)(fprintf(__pyx_v_fo, __pyx_v_fmt, (*((int *) ( /* dim=0 */ (__pyx_v_data.data + __pyx_t_16 * __pyx_v_data.strides[0]) )))));
 
-      /* "ext_modules/io_funcs.pyx":218
+      /* "ext_modules/io_funcs.pyx":222
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1             # <<<<<<<<<<<<<<
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")
  */
       __pyx_t_16 = __pyx_v_j;
       __pyx_v_fr = ((*((long *) ( /* dim=0 */ (__pyx_v_indices.data + __pyx_t_16 * __pyx_v_indices.strides[0]) ))) + 1);
     }
 
-    /* "ext_modules/io_funcs.pyx":219
+    /* "ext_modules/io_funcs.pyx":223
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1
  *         for k in range(fr, N):             # <<<<<<<<<<<<<<
  *             fprintf(fo, "\t0")
  *         fprintf(fo, "\n")
  */
     __pyx_t_20 = __pyx_v_N;
     __pyx_t_21 = __pyx_t_20;
     for (__pyx_t_15 = __pyx_v_fr; __pyx_t_15 < __pyx_t_21; __pyx_t_15+=1) {
       __pyx_v_k = __pyx_t_15;
 
-      /* "ext_modules/io_funcs.pyx":220
+      /* "ext_modules/io_funcs.pyx":224
  *             fr = indices[j] + 1
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")             # <<<<<<<<<<<<<<
  *         fprintf(fo, "\n")
  * 
  */
       (void)(fprintf(__pyx_v_fo, ((char const *)"\t0")));
     }
 
-    /* "ext_modules/io_funcs.pyx":221
+    /* "ext_modules/io_funcs.pyx":225
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")
  *         fprintf(fo, "\n")             # <<<<<<<<<<<<<<
  * 
  *     fclose(fo)
  */
     (void)(fprintf(__pyx_v_fo, ((char const *)"\n")));
   }
 
-  /* "ext_modules/io_funcs.pyx":223
+  /* "ext_modules/io_funcs.pyx":227
  *         fprintf(fo, "\n")
  * 
  *     fclose(fo)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   (void)(fclose(__pyx_v_fo));
 
-  /* "ext_modules/io_funcs.pyx":197
+  /* "ext_modules/io_funcs.pyx":201
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef void write_dense(char* output_file, str[:] barcodes, str[:] features, data_type[:] data, indices_type[:] indices, indptr_type[:] indptr, int M, int N, int precision = 2):             # <<<<<<<<<<<<<<
  *     """ Input must be csr_matrix internal representation, gene by cell (X.T.tocsr()); Output will be gene by cell
  *     """
  */
 
@@ -14505,61 +14620,61 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_output_file)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_barcodes)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_1_1write_dense", 0, 8, 9, 1); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_1_1write_dense", 0, 8, 9, 1); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_features)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_1_1write_dense", 0, 8, 9, 2); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_1_1write_dense", 0, 8, 9, 2); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_1_1write_dense", 0, 8, 9, 3); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_1_1write_dense", 0, 8, 9, 3); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_indices)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_1_1write_dense", 0, 8, 9, 4); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_1_1write_dense", 0, 8, 9, 4); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_indptr)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_1_1write_dense", 0, 8, 9, 5); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_1_1write_dense", 0, 8, 9, 5); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (likely((values[6] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_M)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_1_1write_dense", 0, 8, 9, 6); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_1_1write_dense", 0, 8, 9, 6); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  7:
         if (likely((values[7] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_N)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_1_1write_dense", 0, 8, 9, 7); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_1_1write_dense", 0, 8, 9, 7); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  8:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_precision);
           if (value) { values[8] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_0_1_1write_dense") < 0)) __PYX_ERR(0, 197, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_0_1_1write_dense") < 0)) __PYX_ERR(0, 201, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  9: values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
         CYTHON_FALLTHROUGH;
         case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
         values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
@@ -14569,31 +14684,31 @@
         values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_output_file = __Pyx_PyObject_AsWritableString(values[0]); if (unlikely((!__pyx_v_output_file) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_barcodes = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_barcodes.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_features = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_features.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_data = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_data.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_indices = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indices.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_indptr = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indptr.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_M = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_M == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_N = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_N == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
+    __pyx_v_output_file = __Pyx_PyObject_AsWritableString(values[0]); if (unlikely((!__pyx_v_output_file) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_barcodes = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_barcodes.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_features = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_features.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_data = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_data.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_indices = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indices.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_indptr = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indptr.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_M = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_M == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_N = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_N == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
     if (values[8]) {
-      __pyx_v_precision = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_precision == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
+      __pyx_v_precision = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_precision == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
     } else {
-      __pyx_v_precision = __pyx_k__28;
+      __pyx_v_precision = __pyx_k__29;
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_1_1write_dense", 0, 8, 9, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 197, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_0_1_1write_dense", 0, 8, 9, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 201, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pegasusio.cylib.io.__pyx_fuse_0_1_1write_dense", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9pegasusio_5cylib_2io_50__pyx_fuse_0_1_1write_dense(__pyx_self, __pyx_v_output_file, __pyx_v_barcodes, __pyx_v_features, __pyx_v_data, __pyx_v_indices, __pyx_v_indptr, __pyx_v_M, __pyx_v_N, __pyx_v_precision);
 
@@ -14608,23 +14723,23 @@
   struct __pyx_fuse_0_1_1__pyx_opt_args_9pegasusio_5cylib_2io_write_dense __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_0_1_1write_dense", 0);
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_barcodes.memview)) { __Pyx_RaiseUnboundLocalError("barcodes"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_features.memview)) { __Pyx_RaiseUnboundLocalError("features"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_data.memview)) { __Pyx_RaiseUnboundLocalError("data"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_indices.memview)) { __Pyx_RaiseUnboundLocalError("indices"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_indptr.memview)) { __Pyx_RaiseUnboundLocalError("indptr"); __PYX_ERR(0, 197, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_barcodes.memview)) { __Pyx_RaiseUnboundLocalError("barcodes"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_features.memview)) { __Pyx_RaiseUnboundLocalError("features"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_data.memview)) { __Pyx_RaiseUnboundLocalError("data"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_indices.memview)) { __Pyx_RaiseUnboundLocalError("indices"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_indptr.memview)) { __Pyx_RaiseUnboundLocalError("indptr"); __PYX_ERR(0, 201, __pyx_L1_error) }
   __pyx_t_1.__pyx_n = 1;
   __pyx_t_1.precision = __pyx_v_precision;
   __pyx_fuse_0_1_1__pyx_f_9pegasusio_5cylib_2io_write_dense(__pyx_v_output_file, __pyx_v_barcodes, __pyx_v_features, __pyx_v_data, __pyx_v_indices, __pyx_v_indptr, __pyx_v_M, __pyx_v_N, 0, &__pyx_t_1); 
-  __pyx_t_2 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -14641,15 +14756,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pw_9pegasusio_5cylib_2io_53__pyx_fuse_1_0_0write_dense(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_pw_9pegasusio_5cylib_2io_7write_dense(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static void __pyx_fuse_1_0_0__pyx_f_9pegasusio_5cylib_2io_write_dense(char *__pyx_v_output_file, __Pyx_memviewslice __pyx_v_barcodes, __Pyx_memviewslice __pyx_v_features, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_indices, __Pyx_memviewslice __pyx_v_indptr, int __pyx_v_M, int __pyx_v_N, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_fuse_1_0_0__pyx_opt_args_9pegasusio_5cylib_2io_write_dense *__pyx_optional_args) {
-  int __pyx_v_precision = __pyx_k__29;
+  int __pyx_v_precision = __pyx_k__30;
   FILE *__pyx_v_fo;
   PyObject *__pyx_v_fmt_str = 0;
   char const *__pyx_v_fmt;
   Py_ssize_t __pyx_v_i;
   Py_ssize_t __pyx_v_j;
   CYTHON_UNUSED Py_ssize_t __pyx_v_k;
   Py_ssize_t __pyx_v_fr;
@@ -14679,24 +14794,24 @@
   __Pyx_RefNannySetupContext("__pyx_fuse_1_0_0write_dense", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_precision = __pyx_optional_args->precision;
     }
   }
 
-  /* "ext_modules/io_funcs.pyx":200
+  /* "ext_modules/io_funcs.pyx":204
  *     """ Input must be csr_matrix internal representation, gene by cell (X.T.tocsr()); Output will be gene by cell
  *     """
  *     cdef FILE* fo = fopen(output_file, "w")             # <<<<<<<<<<<<<<
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"
  * 
  */
   __pyx_v_fo = fopen(__pyx_v_output_file, ((char const *)"w"));
 
-  /* "ext_modules/io_funcs.pyx":201
+  /* "ext_modules/io_funcs.pyx":205
  *     """
  *     cdef FILE* fo = fopen(output_file, "w")
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"             # <<<<<<<<<<<<<<
  * 
  *     cdef const char* fmt = fmt_str
  */
   __pyx_t_3 = (0 != 0);
@@ -14705,236 +14820,236 @@
     __pyx_t_2 = __pyx_t_3;
     goto __pyx_L3_bool_binop_done;
   }
   __pyx_t_3 = (0 != 0);
   __pyx_t_2 = __pyx_t_3;
   __pyx_L3_bool_binop_done:;
   if (__pyx_t_2) {
-    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = 0;
     __pyx_t_6 = 127;
-    __Pyx_INCREF(__pyx_kp_u__25);
+    __Pyx_INCREF(__pyx_kp_u__26);
     __pyx_t_5 += 3;
-    __Pyx_GIVEREF(__pyx_kp_u__25);
-    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u__25);
-    __pyx_t_7 = __Pyx_PyUnicode_From_int(__pyx_v_precision, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __Pyx_GIVEREF(__pyx_kp_u__26);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u__26);
+    __pyx_t_7 = __Pyx_PyUnicode_From_int(__pyx_v_precision, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_INCREF(__pyx_n_u_f_2);
     __pyx_t_5 += 1;
     __Pyx_GIVEREF(__pyx_n_u_f_2);
     PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_n_u_f_2);
-    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_1 = __pyx_t_7;
     __pyx_t_7 = 0;
   } else {
     __Pyx_INCREF(__pyx_kp_u_d);
     __pyx_t_1 = __pyx_kp_u_d;
   }
   __pyx_v_fmt_str = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "ext_modules/io_funcs.pyx":203
+  /* "ext_modules/io_funcs.pyx":207
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"
  * 
  *     cdef const char* fmt = fmt_str             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t i, j, k, fr
  * 
  */
-  __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_v_fmt_str); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 203, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_v_fmt_str); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 207, __pyx_L1_error)
   __pyx_v_fmt = __pyx_t_8;
 
-  /* "ext_modules/io_funcs.pyx":206
+  /* "ext_modules/io_funcs.pyx":210
  *     cdef Py_ssize_t i, j, k, fr
  * 
  *     fprintf(fo, "GENE");             # <<<<<<<<<<<<<<
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  */
   (void)(fprintf(__pyx_v_fo, ((char const *)"GENE")));
 
-  /* "ext_modules/io_funcs.pyx":207
+  /* "ext_modules/io_funcs.pyx":211
  * 
  *     fprintf(fo, "GENE");
  *     for i in range(N):             # <<<<<<<<<<<<<<
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  *     fprintf(fo, "\n")
  */
   __pyx_t_9 = __pyx_v_N;
   __pyx_t_10 = __pyx_t_9;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_10; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "ext_modules/io_funcs.pyx":208
+    /* "ext_modules/io_funcs.pyx":212
  *     fprintf(fo, "GENE");
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])             # <<<<<<<<<<<<<<
  *     fprintf(fo, "\n")
  * 
  */
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_1 = (PyObject *) *((PyObject * *) ( /* dim=0 */ (__pyx_v_barcodes.data + __pyx_t_11 * __pyx_v_barcodes.strides[0]) ));
     if (unlikely(__pyx_t_1 == NULL)) __pyx_t_1 = Py_None;
     __Pyx_INCREF((PyObject*)__pyx_t_1);
-    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 208, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 212, __pyx_L1_error)
     (void)(fprintf(__pyx_v_fo, ((char const *)"\t%s"), ((char *)__pyx_t_12)));
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
 
-  /* "ext_modules/io_funcs.pyx":209
+  /* "ext_modules/io_funcs.pyx":213
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  *     fprintf(fo, "\n")             # <<<<<<<<<<<<<<
  * 
  *     for i in range(M):
  */
   (void)(fprintf(__pyx_v_fo, ((char const *)"\n")));
 
-  /* "ext_modules/io_funcs.pyx":211
+  /* "ext_modules/io_funcs.pyx":215
  *     fprintf(fo, "\n")
  * 
  *     for i in range(M):             # <<<<<<<<<<<<<<
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0
  */
   __pyx_t_9 = __pyx_v_M;
   __pyx_t_10 = __pyx_t_9;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_10; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "ext_modules/io_funcs.pyx":212
+    /* "ext_modules/io_funcs.pyx":216
  * 
  *     for i in range(M):
  *         fprintf(fo, "%s", <char*>features[i]);             # <<<<<<<<<<<<<<
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):
  */
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_1 = (PyObject *) *((PyObject * *) ( /* dim=0 */ (__pyx_v_features.data + __pyx_t_11 * __pyx_v_features.strides[0]) ));
     if (unlikely(__pyx_t_1 == NULL)) __pyx_t_1 = Py_None;
     __Pyx_INCREF((PyObject*)__pyx_t_1);
-    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 212, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 216, __pyx_L1_error)
     (void)(fprintf(__pyx_v_fo, ((char const *)"%s"), ((char *)__pyx_t_12)));
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "ext_modules/io_funcs.pyx":213
+    /* "ext_modules/io_funcs.pyx":217
  *     for i in range(M):
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0             # <<<<<<<<<<<<<<
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):
  */
     __pyx_v_fr = 0;
 
-    /* "ext_modules/io_funcs.pyx":214
+    /* "ext_modules/io_funcs.pyx":218
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):             # <<<<<<<<<<<<<<
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")
  */
     __pyx_t_11 = (__pyx_v_i + 1);
     __pyx_t_13 = (*((int *) ( /* dim=0 */ (__pyx_v_indptr.data + __pyx_t_11 * __pyx_v_indptr.strides[0]) )));
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = (*((int *) ( /* dim=0 */ (__pyx_v_indptr.data + __pyx_t_11 * __pyx_v_indptr.strides[0]) ))); __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_j = __pyx_t_15;
 
-      /* "ext_modules/io_funcs.pyx":215
+      /* "ext_modules/io_funcs.pyx":219
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):             # <<<<<<<<<<<<<<
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])
  */
       __pyx_t_16 = __pyx_v_j;
       __pyx_t_17 = (*((int *) ( /* dim=0 */ (__pyx_v_indices.data + __pyx_t_16 * __pyx_v_indices.strides[0]) )));
       __pyx_t_18 = __pyx_t_17;
       for (__pyx_t_19 = __pyx_v_fr; __pyx_t_19 < __pyx_t_18; __pyx_t_19+=1) {
         __pyx_v_k = __pyx_t_19;
 
-        /* "ext_modules/io_funcs.pyx":216
+        /* "ext_modules/io_funcs.pyx":220
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")             # <<<<<<<<<<<<<<
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1
  */
         (void)(fprintf(__pyx_v_fo, ((char const *)"\t0")));
       }
 
-      /* "ext_modules/io_funcs.pyx":217
+      /* "ext_modules/io_funcs.pyx":221
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])             # <<<<<<<<<<<<<<
  *             fr = indices[j] + 1
  *         for k in range(fr, N):
  */
       __pyx_t_16 = __pyx_v_j;
       (void)(fprintf(__pyx_v_fo, __pyx_v_fmt, (*((long *) ( /* dim=0 */ (__pyx_v_data.data + __pyx_t_16 * __pyx_v_data.strides[0]) )))));
 
-      /* "ext_modules/io_funcs.pyx":218
+      /* "ext_modules/io_funcs.pyx":222
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1             # <<<<<<<<<<<<<<
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")
  */
       __pyx_t_16 = __pyx_v_j;
       __pyx_v_fr = ((*((int *) ( /* dim=0 */ (__pyx_v_indices.data + __pyx_t_16 * __pyx_v_indices.strides[0]) ))) + 1);
     }
 
-    /* "ext_modules/io_funcs.pyx":219
+    /* "ext_modules/io_funcs.pyx":223
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1
  *         for k in range(fr, N):             # <<<<<<<<<<<<<<
  *             fprintf(fo, "\t0")
  *         fprintf(fo, "\n")
  */
     __pyx_t_13 = __pyx_v_N;
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = __pyx_v_fr; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_k = __pyx_t_15;
 
-      /* "ext_modules/io_funcs.pyx":220
+      /* "ext_modules/io_funcs.pyx":224
  *             fr = indices[j] + 1
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")             # <<<<<<<<<<<<<<
  *         fprintf(fo, "\n")
  * 
  */
       (void)(fprintf(__pyx_v_fo, ((char const *)"\t0")));
     }
 
-    /* "ext_modules/io_funcs.pyx":221
+    /* "ext_modules/io_funcs.pyx":225
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")
  *         fprintf(fo, "\n")             # <<<<<<<<<<<<<<
  * 
  *     fclose(fo)
  */
     (void)(fprintf(__pyx_v_fo, ((char const *)"\n")));
   }
 
-  /* "ext_modules/io_funcs.pyx":223
+  /* "ext_modules/io_funcs.pyx":227
  *         fprintf(fo, "\n")
  * 
  *     fclose(fo)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   (void)(fclose(__pyx_v_fo));
 
-  /* "ext_modules/io_funcs.pyx":197
+  /* "ext_modules/io_funcs.pyx":201
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef void write_dense(char* output_file, str[:] barcodes, str[:] features, data_type[:] data, indices_type[:] indices, indptr_type[:] indptr, int M, int N, int precision = 2):             # <<<<<<<<<<<<<<
  *     """ Input must be csr_matrix internal representation, gene by cell (X.T.tocsr()); Output will be gene by cell
  *     """
  */
 
@@ -15002,61 +15117,61 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_output_file)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_barcodes)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_0_0write_dense", 0, 8, 9, 1); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_0_0write_dense", 0, 8, 9, 1); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_features)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_0_0write_dense", 0, 8, 9, 2); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_0_0write_dense", 0, 8, 9, 2); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_0_0write_dense", 0, 8, 9, 3); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_0_0write_dense", 0, 8, 9, 3); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_indices)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_0_0write_dense", 0, 8, 9, 4); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_0_0write_dense", 0, 8, 9, 4); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_indptr)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_0_0write_dense", 0, 8, 9, 5); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_0_0write_dense", 0, 8, 9, 5); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (likely((values[6] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_M)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_0_0write_dense", 0, 8, 9, 6); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_0_0write_dense", 0, 8, 9, 6); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  7:
         if (likely((values[7] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_N)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_0_0write_dense", 0, 8, 9, 7); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_0_0write_dense", 0, 8, 9, 7); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  8:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_precision);
           if (value) { values[8] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_1_0_0write_dense") < 0)) __PYX_ERR(0, 197, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_1_0_0write_dense") < 0)) __PYX_ERR(0, 201, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  9: values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
         CYTHON_FALLTHROUGH;
         case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
         values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
@@ -15066,31 +15181,31 @@
         values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_output_file = __Pyx_PyObject_AsWritableString(values[0]); if (unlikely((!__pyx_v_output_file) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_barcodes = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_barcodes.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_features = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_features.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_data = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_data.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_indices = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indices.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_indptr = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indptr.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_M = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_M == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_N = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_N == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
+    __pyx_v_output_file = __Pyx_PyObject_AsWritableString(values[0]); if (unlikely((!__pyx_v_output_file) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_barcodes = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_barcodes.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_features = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_features.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_data = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_data.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_indices = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indices.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_indptr = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indptr.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_M = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_M == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_N = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_N == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
     if (values[8]) {
-      __pyx_v_precision = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_precision == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
+      __pyx_v_precision = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_precision == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
     } else {
-      __pyx_v_precision = __pyx_k__29;
+      __pyx_v_precision = __pyx_k__30;
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_0_0write_dense", 0, 8, 9, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 197, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_0_0write_dense", 0, 8, 9, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 201, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pegasusio.cylib.io.__pyx_fuse_1_0_0write_dense", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9pegasusio_5cylib_2io_52__pyx_fuse_1_0_0write_dense(__pyx_self, __pyx_v_output_file, __pyx_v_barcodes, __pyx_v_features, __pyx_v_data, __pyx_v_indices, __pyx_v_indptr, __pyx_v_M, __pyx_v_N, __pyx_v_precision);
 
@@ -15105,23 +15220,23 @@
   struct __pyx_fuse_1_0_0__pyx_opt_args_9pegasusio_5cylib_2io_write_dense __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_1_0_0write_dense", 0);
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_barcodes.memview)) { __Pyx_RaiseUnboundLocalError("barcodes"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_features.memview)) { __Pyx_RaiseUnboundLocalError("features"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_data.memview)) { __Pyx_RaiseUnboundLocalError("data"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_indices.memview)) { __Pyx_RaiseUnboundLocalError("indices"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_indptr.memview)) { __Pyx_RaiseUnboundLocalError("indptr"); __PYX_ERR(0, 197, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_barcodes.memview)) { __Pyx_RaiseUnboundLocalError("barcodes"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_features.memview)) { __Pyx_RaiseUnboundLocalError("features"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_data.memview)) { __Pyx_RaiseUnboundLocalError("data"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_indices.memview)) { __Pyx_RaiseUnboundLocalError("indices"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_indptr.memview)) { __Pyx_RaiseUnboundLocalError("indptr"); __PYX_ERR(0, 201, __pyx_L1_error) }
   __pyx_t_1.__pyx_n = 1;
   __pyx_t_1.precision = __pyx_v_precision;
   __pyx_fuse_1_0_0__pyx_f_9pegasusio_5cylib_2io_write_dense(__pyx_v_output_file, __pyx_v_barcodes, __pyx_v_features, __pyx_v_data, __pyx_v_indices, __pyx_v_indptr, __pyx_v_M, __pyx_v_N, 0, &__pyx_t_1); 
-  __pyx_t_2 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -15138,15 +15253,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pw_9pegasusio_5cylib_2io_55__pyx_fuse_1_0_1write_dense(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_pw_9pegasusio_5cylib_2io_7write_dense(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static void __pyx_fuse_1_0_1__pyx_f_9pegasusio_5cylib_2io_write_dense(char *__pyx_v_output_file, __Pyx_memviewslice __pyx_v_barcodes, __Pyx_memviewslice __pyx_v_features, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_indices, __Pyx_memviewslice __pyx_v_indptr, int __pyx_v_M, int __pyx_v_N, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_fuse_1_0_1__pyx_opt_args_9pegasusio_5cylib_2io_write_dense *__pyx_optional_args) {
-  int __pyx_v_precision = __pyx_k__30;
+  int __pyx_v_precision = __pyx_k__31;
   FILE *__pyx_v_fo;
   PyObject *__pyx_v_fmt_str = 0;
   char const *__pyx_v_fmt;
   Py_ssize_t __pyx_v_i;
   Py_ssize_t __pyx_v_j;
   CYTHON_UNUSED Py_ssize_t __pyx_v_k;
   Py_ssize_t __pyx_v_fr;
@@ -15176,24 +15291,24 @@
   __Pyx_RefNannySetupContext("__pyx_fuse_1_0_1write_dense", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_precision = __pyx_optional_args->precision;
     }
   }
 
-  /* "ext_modules/io_funcs.pyx":200
+  /* "ext_modules/io_funcs.pyx":204
  *     """ Input must be csr_matrix internal representation, gene by cell (X.T.tocsr()); Output will be gene by cell
  *     """
  *     cdef FILE* fo = fopen(output_file, "w")             # <<<<<<<<<<<<<<
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"
  * 
  */
   __pyx_v_fo = fopen(__pyx_v_output_file, ((char const *)"w"));
 
-  /* "ext_modules/io_funcs.pyx":201
+  /* "ext_modules/io_funcs.pyx":205
  *     """
  *     cdef FILE* fo = fopen(output_file, "w")
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"             # <<<<<<<<<<<<<<
  * 
  *     cdef const char* fmt = fmt_str
  */
   __pyx_t_3 = (0 != 0);
@@ -15202,236 +15317,236 @@
     __pyx_t_2 = __pyx_t_3;
     goto __pyx_L3_bool_binop_done;
   }
   __pyx_t_3 = (0 != 0);
   __pyx_t_2 = __pyx_t_3;
   __pyx_L3_bool_binop_done:;
   if (__pyx_t_2) {
-    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = 0;
     __pyx_t_6 = 127;
-    __Pyx_INCREF(__pyx_kp_u__25);
+    __Pyx_INCREF(__pyx_kp_u__26);
     __pyx_t_5 += 3;
-    __Pyx_GIVEREF(__pyx_kp_u__25);
-    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u__25);
-    __pyx_t_7 = __Pyx_PyUnicode_From_int(__pyx_v_precision, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __Pyx_GIVEREF(__pyx_kp_u__26);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u__26);
+    __pyx_t_7 = __Pyx_PyUnicode_From_int(__pyx_v_precision, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_INCREF(__pyx_n_u_f_2);
     __pyx_t_5 += 1;
     __Pyx_GIVEREF(__pyx_n_u_f_2);
     PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_n_u_f_2);
-    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_1 = __pyx_t_7;
     __pyx_t_7 = 0;
   } else {
     __Pyx_INCREF(__pyx_kp_u_d);
     __pyx_t_1 = __pyx_kp_u_d;
   }
   __pyx_v_fmt_str = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "ext_modules/io_funcs.pyx":203
+  /* "ext_modules/io_funcs.pyx":207
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"
  * 
  *     cdef const char* fmt = fmt_str             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t i, j, k, fr
  * 
  */
-  __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_v_fmt_str); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 203, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_v_fmt_str); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 207, __pyx_L1_error)
   __pyx_v_fmt = __pyx_t_8;
 
-  /* "ext_modules/io_funcs.pyx":206
+  /* "ext_modules/io_funcs.pyx":210
  *     cdef Py_ssize_t i, j, k, fr
  * 
  *     fprintf(fo, "GENE");             # <<<<<<<<<<<<<<
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  */
   (void)(fprintf(__pyx_v_fo, ((char const *)"GENE")));
 
-  /* "ext_modules/io_funcs.pyx":207
+  /* "ext_modules/io_funcs.pyx":211
  * 
  *     fprintf(fo, "GENE");
  *     for i in range(N):             # <<<<<<<<<<<<<<
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  *     fprintf(fo, "\n")
  */
   __pyx_t_9 = __pyx_v_N;
   __pyx_t_10 = __pyx_t_9;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_10; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "ext_modules/io_funcs.pyx":208
+    /* "ext_modules/io_funcs.pyx":212
  *     fprintf(fo, "GENE");
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])             # <<<<<<<<<<<<<<
  *     fprintf(fo, "\n")
  * 
  */
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_1 = (PyObject *) *((PyObject * *) ( /* dim=0 */ (__pyx_v_barcodes.data + __pyx_t_11 * __pyx_v_barcodes.strides[0]) ));
     if (unlikely(__pyx_t_1 == NULL)) __pyx_t_1 = Py_None;
     __Pyx_INCREF((PyObject*)__pyx_t_1);
-    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 208, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 212, __pyx_L1_error)
     (void)(fprintf(__pyx_v_fo, ((char const *)"\t%s"), ((char *)__pyx_t_12)));
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
 
-  /* "ext_modules/io_funcs.pyx":209
+  /* "ext_modules/io_funcs.pyx":213
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  *     fprintf(fo, "\n")             # <<<<<<<<<<<<<<
  * 
  *     for i in range(M):
  */
   (void)(fprintf(__pyx_v_fo, ((char const *)"\n")));
 
-  /* "ext_modules/io_funcs.pyx":211
+  /* "ext_modules/io_funcs.pyx":215
  *     fprintf(fo, "\n")
  * 
  *     for i in range(M):             # <<<<<<<<<<<<<<
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0
  */
   __pyx_t_9 = __pyx_v_M;
   __pyx_t_10 = __pyx_t_9;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_10; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "ext_modules/io_funcs.pyx":212
+    /* "ext_modules/io_funcs.pyx":216
  * 
  *     for i in range(M):
  *         fprintf(fo, "%s", <char*>features[i]);             # <<<<<<<<<<<<<<
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):
  */
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_1 = (PyObject *) *((PyObject * *) ( /* dim=0 */ (__pyx_v_features.data + __pyx_t_11 * __pyx_v_features.strides[0]) ));
     if (unlikely(__pyx_t_1 == NULL)) __pyx_t_1 = Py_None;
     __Pyx_INCREF((PyObject*)__pyx_t_1);
-    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 212, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 216, __pyx_L1_error)
     (void)(fprintf(__pyx_v_fo, ((char const *)"%s"), ((char *)__pyx_t_12)));
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "ext_modules/io_funcs.pyx":213
+    /* "ext_modules/io_funcs.pyx":217
  *     for i in range(M):
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0             # <<<<<<<<<<<<<<
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):
  */
     __pyx_v_fr = 0;
 
-    /* "ext_modules/io_funcs.pyx":214
+    /* "ext_modules/io_funcs.pyx":218
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):             # <<<<<<<<<<<<<<
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")
  */
     __pyx_t_11 = (__pyx_v_i + 1);
     __pyx_t_13 = (*((long *) ( /* dim=0 */ (__pyx_v_indptr.data + __pyx_t_11 * __pyx_v_indptr.strides[0]) )));
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = (*((long *) ( /* dim=0 */ (__pyx_v_indptr.data + __pyx_t_11 * __pyx_v_indptr.strides[0]) ))); __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_j = __pyx_t_15;
 
-      /* "ext_modules/io_funcs.pyx":215
+      /* "ext_modules/io_funcs.pyx":219
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):             # <<<<<<<<<<<<<<
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])
  */
       __pyx_t_16 = __pyx_v_j;
       __pyx_t_17 = (*((int *) ( /* dim=0 */ (__pyx_v_indices.data + __pyx_t_16 * __pyx_v_indices.strides[0]) )));
       __pyx_t_18 = __pyx_t_17;
       for (__pyx_t_19 = __pyx_v_fr; __pyx_t_19 < __pyx_t_18; __pyx_t_19+=1) {
         __pyx_v_k = __pyx_t_19;
 
-        /* "ext_modules/io_funcs.pyx":216
+        /* "ext_modules/io_funcs.pyx":220
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")             # <<<<<<<<<<<<<<
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1
  */
         (void)(fprintf(__pyx_v_fo, ((char const *)"\t0")));
       }
 
-      /* "ext_modules/io_funcs.pyx":217
+      /* "ext_modules/io_funcs.pyx":221
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])             # <<<<<<<<<<<<<<
  *             fr = indices[j] + 1
  *         for k in range(fr, N):
  */
       __pyx_t_16 = __pyx_v_j;
       (void)(fprintf(__pyx_v_fo, __pyx_v_fmt, (*((long *) ( /* dim=0 */ (__pyx_v_data.data + __pyx_t_16 * __pyx_v_data.strides[0]) )))));
 
-      /* "ext_modules/io_funcs.pyx":218
+      /* "ext_modules/io_funcs.pyx":222
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1             # <<<<<<<<<<<<<<
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")
  */
       __pyx_t_16 = __pyx_v_j;
       __pyx_v_fr = ((*((int *) ( /* dim=0 */ (__pyx_v_indices.data + __pyx_t_16 * __pyx_v_indices.strides[0]) ))) + 1);
     }
 
-    /* "ext_modules/io_funcs.pyx":219
+    /* "ext_modules/io_funcs.pyx":223
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1
  *         for k in range(fr, N):             # <<<<<<<<<<<<<<
  *             fprintf(fo, "\t0")
  *         fprintf(fo, "\n")
  */
     __pyx_t_17 = __pyx_v_N;
     __pyx_t_18 = __pyx_t_17;
     for (__pyx_t_15 = __pyx_v_fr; __pyx_t_15 < __pyx_t_18; __pyx_t_15+=1) {
       __pyx_v_k = __pyx_t_15;
 
-      /* "ext_modules/io_funcs.pyx":220
+      /* "ext_modules/io_funcs.pyx":224
  *             fr = indices[j] + 1
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")             # <<<<<<<<<<<<<<
  *         fprintf(fo, "\n")
  * 
  */
       (void)(fprintf(__pyx_v_fo, ((char const *)"\t0")));
     }
 
-    /* "ext_modules/io_funcs.pyx":221
+    /* "ext_modules/io_funcs.pyx":225
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")
  *         fprintf(fo, "\n")             # <<<<<<<<<<<<<<
  * 
  *     fclose(fo)
  */
     (void)(fprintf(__pyx_v_fo, ((char const *)"\n")));
   }
 
-  /* "ext_modules/io_funcs.pyx":223
+  /* "ext_modules/io_funcs.pyx":227
  *         fprintf(fo, "\n")
  * 
  *     fclose(fo)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   (void)(fclose(__pyx_v_fo));
 
-  /* "ext_modules/io_funcs.pyx":197
+  /* "ext_modules/io_funcs.pyx":201
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef void write_dense(char* output_file, str[:] barcodes, str[:] features, data_type[:] data, indices_type[:] indices, indptr_type[:] indptr, int M, int N, int precision = 2):             # <<<<<<<<<<<<<<
  *     """ Input must be csr_matrix internal representation, gene by cell (X.T.tocsr()); Output will be gene by cell
  *     """
  */
 
@@ -15499,61 +15614,61 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_output_file)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_barcodes)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_0_1write_dense", 0, 8, 9, 1); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_0_1write_dense", 0, 8, 9, 1); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_features)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_0_1write_dense", 0, 8, 9, 2); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_0_1write_dense", 0, 8, 9, 2); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_0_1write_dense", 0, 8, 9, 3); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_0_1write_dense", 0, 8, 9, 3); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_indices)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_0_1write_dense", 0, 8, 9, 4); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_0_1write_dense", 0, 8, 9, 4); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_indptr)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_0_1write_dense", 0, 8, 9, 5); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_0_1write_dense", 0, 8, 9, 5); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (likely((values[6] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_M)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_0_1write_dense", 0, 8, 9, 6); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_0_1write_dense", 0, 8, 9, 6); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  7:
         if (likely((values[7] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_N)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_0_1write_dense", 0, 8, 9, 7); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_0_1write_dense", 0, 8, 9, 7); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  8:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_precision);
           if (value) { values[8] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_1_0_1write_dense") < 0)) __PYX_ERR(0, 197, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_1_0_1write_dense") < 0)) __PYX_ERR(0, 201, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  9: values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
         CYTHON_FALLTHROUGH;
         case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
         values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
@@ -15563,31 +15678,31 @@
         values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_output_file = __Pyx_PyObject_AsWritableString(values[0]); if (unlikely((!__pyx_v_output_file) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_barcodes = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_barcodes.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_features = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_features.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_data = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_data.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_indices = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indices.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_indptr = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indptr.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_M = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_M == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_N = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_N == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
+    __pyx_v_output_file = __Pyx_PyObject_AsWritableString(values[0]); if (unlikely((!__pyx_v_output_file) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_barcodes = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_barcodes.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_features = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_features.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_data = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_data.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_indices = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indices.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_indptr = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indptr.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_M = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_M == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_N = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_N == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
     if (values[8]) {
-      __pyx_v_precision = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_precision == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
+      __pyx_v_precision = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_precision == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
     } else {
-      __pyx_v_precision = __pyx_k__30;
+      __pyx_v_precision = __pyx_k__31;
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_0_1write_dense", 0, 8, 9, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 197, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_0_1write_dense", 0, 8, 9, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 201, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pegasusio.cylib.io.__pyx_fuse_1_0_1write_dense", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9pegasusio_5cylib_2io_54__pyx_fuse_1_0_1write_dense(__pyx_self, __pyx_v_output_file, __pyx_v_barcodes, __pyx_v_features, __pyx_v_data, __pyx_v_indices, __pyx_v_indptr, __pyx_v_M, __pyx_v_N, __pyx_v_precision);
 
@@ -15602,23 +15717,23 @@
   struct __pyx_fuse_1_0_1__pyx_opt_args_9pegasusio_5cylib_2io_write_dense __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_1_0_1write_dense", 0);
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_barcodes.memview)) { __Pyx_RaiseUnboundLocalError("barcodes"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_features.memview)) { __Pyx_RaiseUnboundLocalError("features"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_data.memview)) { __Pyx_RaiseUnboundLocalError("data"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_indices.memview)) { __Pyx_RaiseUnboundLocalError("indices"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_indptr.memview)) { __Pyx_RaiseUnboundLocalError("indptr"); __PYX_ERR(0, 197, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_barcodes.memview)) { __Pyx_RaiseUnboundLocalError("barcodes"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_features.memview)) { __Pyx_RaiseUnboundLocalError("features"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_data.memview)) { __Pyx_RaiseUnboundLocalError("data"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_indices.memview)) { __Pyx_RaiseUnboundLocalError("indices"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_indptr.memview)) { __Pyx_RaiseUnboundLocalError("indptr"); __PYX_ERR(0, 201, __pyx_L1_error) }
   __pyx_t_1.__pyx_n = 1;
   __pyx_t_1.precision = __pyx_v_precision;
   __pyx_fuse_1_0_1__pyx_f_9pegasusio_5cylib_2io_write_dense(__pyx_v_output_file, __pyx_v_barcodes, __pyx_v_features, __pyx_v_data, __pyx_v_indices, __pyx_v_indptr, __pyx_v_M, __pyx_v_N, 0, &__pyx_t_1); 
-  __pyx_t_2 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -15635,15 +15750,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pw_9pegasusio_5cylib_2io_57__pyx_fuse_1_1_0write_dense(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_pw_9pegasusio_5cylib_2io_7write_dense(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static void __pyx_fuse_1_1_0__pyx_f_9pegasusio_5cylib_2io_write_dense(char *__pyx_v_output_file, __Pyx_memviewslice __pyx_v_barcodes, __Pyx_memviewslice __pyx_v_features, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_indices, __Pyx_memviewslice __pyx_v_indptr, int __pyx_v_M, int __pyx_v_N, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_fuse_1_1_0__pyx_opt_args_9pegasusio_5cylib_2io_write_dense *__pyx_optional_args) {
-  int __pyx_v_precision = __pyx_k__31;
+  int __pyx_v_precision = __pyx_k__32;
   FILE *__pyx_v_fo;
   PyObject *__pyx_v_fmt_str = 0;
   char const *__pyx_v_fmt;
   Py_ssize_t __pyx_v_i;
   Py_ssize_t __pyx_v_j;
   CYTHON_UNUSED Py_ssize_t __pyx_v_k;
   Py_ssize_t __pyx_v_fr;
@@ -15673,24 +15788,24 @@
   __Pyx_RefNannySetupContext("__pyx_fuse_1_1_0write_dense", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_precision = __pyx_optional_args->precision;
     }
   }
 
-  /* "ext_modules/io_funcs.pyx":200
+  /* "ext_modules/io_funcs.pyx":204
  *     """ Input must be csr_matrix internal representation, gene by cell (X.T.tocsr()); Output will be gene by cell
  *     """
  *     cdef FILE* fo = fopen(output_file, "w")             # <<<<<<<<<<<<<<
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"
  * 
  */
   __pyx_v_fo = fopen(__pyx_v_output_file, ((char const *)"w"));
 
-  /* "ext_modules/io_funcs.pyx":201
+  /* "ext_modules/io_funcs.pyx":205
  *     """
  *     cdef FILE* fo = fopen(output_file, "w")
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"             # <<<<<<<<<<<<<<
  * 
  *     cdef const char* fmt = fmt_str
  */
   __pyx_t_3 = (0 != 0);
@@ -15699,236 +15814,236 @@
     __pyx_t_2 = __pyx_t_3;
     goto __pyx_L3_bool_binop_done;
   }
   __pyx_t_3 = (0 != 0);
   __pyx_t_2 = __pyx_t_3;
   __pyx_L3_bool_binop_done:;
   if (__pyx_t_2) {
-    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = 0;
     __pyx_t_6 = 127;
-    __Pyx_INCREF(__pyx_kp_u__25);
+    __Pyx_INCREF(__pyx_kp_u__26);
     __pyx_t_5 += 3;
-    __Pyx_GIVEREF(__pyx_kp_u__25);
-    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u__25);
-    __pyx_t_7 = __Pyx_PyUnicode_From_int(__pyx_v_precision, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __Pyx_GIVEREF(__pyx_kp_u__26);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u__26);
+    __pyx_t_7 = __Pyx_PyUnicode_From_int(__pyx_v_precision, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_INCREF(__pyx_n_u_f_2);
     __pyx_t_5 += 1;
     __Pyx_GIVEREF(__pyx_n_u_f_2);
     PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_n_u_f_2);
-    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_1 = __pyx_t_7;
     __pyx_t_7 = 0;
   } else {
     __Pyx_INCREF(__pyx_kp_u_d);
     __pyx_t_1 = __pyx_kp_u_d;
   }
   __pyx_v_fmt_str = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "ext_modules/io_funcs.pyx":203
+  /* "ext_modules/io_funcs.pyx":207
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"
  * 
  *     cdef const char* fmt = fmt_str             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t i, j, k, fr
  * 
  */
-  __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_v_fmt_str); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 203, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_v_fmt_str); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 207, __pyx_L1_error)
   __pyx_v_fmt = __pyx_t_8;
 
-  /* "ext_modules/io_funcs.pyx":206
+  /* "ext_modules/io_funcs.pyx":210
  *     cdef Py_ssize_t i, j, k, fr
  * 
  *     fprintf(fo, "GENE");             # <<<<<<<<<<<<<<
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  */
   (void)(fprintf(__pyx_v_fo, ((char const *)"GENE")));
 
-  /* "ext_modules/io_funcs.pyx":207
+  /* "ext_modules/io_funcs.pyx":211
  * 
  *     fprintf(fo, "GENE");
  *     for i in range(N):             # <<<<<<<<<<<<<<
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  *     fprintf(fo, "\n")
  */
   __pyx_t_9 = __pyx_v_N;
   __pyx_t_10 = __pyx_t_9;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_10; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "ext_modules/io_funcs.pyx":208
+    /* "ext_modules/io_funcs.pyx":212
  *     fprintf(fo, "GENE");
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])             # <<<<<<<<<<<<<<
  *     fprintf(fo, "\n")
  * 
  */
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_1 = (PyObject *) *((PyObject * *) ( /* dim=0 */ (__pyx_v_barcodes.data + __pyx_t_11 * __pyx_v_barcodes.strides[0]) ));
     if (unlikely(__pyx_t_1 == NULL)) __pyx_t_1 = Py_None;
     __Pyx_INCREF((PyObject*)__pyx_t_1);
-    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 208, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 212, __pyx_L1_error)
     (void)(fprintf(__pyx_v_fo, ((char const *)"\t%s"), ((char *)__pyx_t_12)));
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
 
-  /* "ext_modules/io_funcs.pyx":209
+  /* "ext_modules/io_funcs.pyx":213
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  *     fprintf(fo, "\n")             # <<<<<<<<<<<<<<
  * 
  *     for i in range(M):
  */
   (void)(fprintf(__pyx_v_fo, ((char const *)"\n")));
 
-  /* "ext_modules/io_funcs.pyx":211
+  /* "ext_modules/io_funcs.pyx":215
  *     fprintf(fo, "\n")
  * 
  *     for i in range(M):             # <<<<<<<<<<<<<<
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0
  */
   __pyx_t_9 = __pyx_v_M;
   __pyx_t_10 = __pyx_t_9;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_10; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "ext_modules/io_funcs.pyx":212
+    /* "ext_modules/io_funcs.pyx":216
  * 
  *     for i in range(M):
  *         fprintf(fo, "%s", <char*>features[i]);             # <<<<<<<<<<<<<<
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):
  */
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_1 = (PyObject *) *((PyObject * *) ( /* dim=0 */ (__pyx_v_features.data + __pyx_t_11 * __pyx_v_features.strides[0]) ));
     if (unlikely(__pyx_t_1 == NULL)) __pyx_t_1 = Py_None;
     __Pyx_INCREF((PyObject*)__pyx_t_1);
-    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 212, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 216, __pyx_L1_error)
     (void)(fprintf(__pyx_v_fo, ((char const *)"%s"), ((char *)__pyx_t_12)));
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "ext_modules/io_funcs.pyx":213
+    /* "ext_modules/io_funcs.pyx":217
  *     for i in range(M):
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0             # <<<<<<<<<<<<<<
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):
  */
     __pyx_v_fr = 0;
 
-    /* "ext_modules/io_funcs.pyx":214
+    /* "ext_modules/io_funcs.pyx":218
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):             # <<<<<<<<<<<<<<
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")
  */
     __pyx_t_11 = (__pyx_v_i + 1);
     __pyx_t_13 = (*((int *) ( /* dim=0 */ (__pyx_v_indptr.data + __pyx_t_11 * __pyx_v_indptr.strides[0]) )));
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = (*((int *) ( /* dim=0 */ (__pyx_v_indptr.data + __pyx_t_11 * __pyx_v_indptr.strides[0]) ))); __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_j = __pyx_t_15;
 
-      /* "ext_modules/io_funcs.pyx":215
+      /* "ext_modules/io_funcs.pyx":219
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):             # <<<<<<<<<<<<<<
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])
  */
       __pyx_t_16 = __pyx_v_j;
       __pyx_t_17 = (*((long *) ( /* dim=0 */ (__pyx_v_indices.data + __pyx_t_16 * __pyx_v_indices.strides[0]) )));
       __pyx_t_18 = __pyx_t_17;
       for (__pyx_t_19 = __pyx_v_fr; __pyx_t_19 < __pyx_t_18; __pyx_t_19+=1) {
         __pyx_v_k = __pyx_t_19;
 
-        /* "ext_modules/io_funcs.pyx":216
+        /* "ext_modules/io_funcs.pyx":220
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")             # <<<<<<<<<<<<<<
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1
  */
         (void)(fprintf(__pyx_v_fo, ((char const *)"\t0")));
       }
 
-      /* "ext_modules/io_funcs.pyx":217
+      /* "ext_modules/io_funcs.pyx":221
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])             # <<<<<<<<<<<<<<
  *             fr = indices[j] + 1
  *         for k in range(fr, N):
  */
       __pyx_t_16 = __pyx_v_j;
       (void)(fprintf(__pyx_v_fo, __pyx_v_fmt, (*((long *) ( /* dim=0 */ (__pyx_v_data.data + __pyx_t_16 * __pyx_v_data.strides[0]) )))));
 
-      /* "ext_modules/io_funcs.pyx":218
+      /* "ext_modules/io_funcs.pyx":222
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1             # <<<<<<<<<<<<<<
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")
  */
       __pyx_t_16 = __pyx_v_j;
       __pyx_v_fr = ((*((long *) ( /* dim=0 */ (__pyx_v_indices.data + __pyx_t_16 * __pyx_v_indices.strides[0]) ))) + 1);
     }
 
-    /* "ext_modules/io_funcs.pyx":219
+    /* "ext_modules/io_funcs.pyx":223
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1
  *         for k in range(fr, N):             # <<<<<<<<<<<<<<
  *             fprintf(fo, "\t0")
  *         fprintf(fo, "\n")
  */
     __pyx_t_13 = __pyx_v_N;
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = __pyx_v_fr; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_k = __pyx_t_15;
 
-      /* "ext_modules/io_funcs.pyx":220
+      /* "ext_modules/io_funcs.pyx":224
  *             fr = indices[j] + 1
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")             # <<<<<<<<<<<<<<
  *         fprintf(fo, "\n")
  * 
  */
       (void)(fprintf(__pyx_v_fo, ((char const *)"\t0")));
     }
 
-    /* "ext_modules/io_funcs.pyx":221
+    /* "ext_modules/io_funcs.pyx":225
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")
  *         fprintf(fo, "\n")             # <<<<<<<<<<<<<<
  * 
  *     fclose(fo)
  */
     (void)(fprintf(__pyx_v_fo, ((char const *)"\n")));
   }
 
-  /* "ext_modules/io_funcs.pyx":223
+  /* "ext_modules/io_funcs.pyx":227
  *         fprintf(fo, "\n")
  * 
  *     fclose(fo)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   (void)(fclose(__pyx_v_fo));
 
-  /* "ext_modules/io_funcs.pyx":197
+  /* "ext_modules/io_funcs.pyx":201
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef void write_dense(char* output_file, str[:] barcodes, str[:] features, data_type[:] data, indices_type[:] indices, indptr_type[:] indptr, int M, int N, int precision = 2):             # <<<<<<<<<<<<<<
  *     """ Input must be csr_matrix internal representation, gene by cell (X.T.tocsr()); Output will be gene by cell
  *     """
  */
 
@@ -15996,61 +16111,61 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_output_file)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_barcodes)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_1_0write_dense", 0, 8, 9, 1); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_1_0write_dense", 0, 8, 9, 1); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_features)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_1_0write_dense", 0, 8, 9, 2); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_1_0write_dense", 0, 8, 9, 2); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_1_0write_dense", 0, 8, 9, 3); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_1_0write_dense", 0, 8, 9, 3); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_indices)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_1_0write_dense", 0, 8, 9, 4); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_1_0write_dense", 0, 8, 9, 4); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_indptr)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_1_0write_dense", 0, 8, 9, 5); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_1_0write_dense", 0, 8, 9, 5); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (likely((values[6] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_M)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_1_0write_dense", 0, 8, 9, 6); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_1_0write_dense", 0, 8, 9, 6); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  7:
         if (likely((values[7] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_N)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_1_0write_dense", 0, 8, 9, 7); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_1_0write_dense", 0, 8, 9, 7); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  8:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_precision);
           if (value) { values[8] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_1_1_0write_dense") < 0)) __PYX_ERR(0, 197, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_1_1_0write_dense") < 0)) __PYX_ERR(0, 201, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  9: values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
         CYTHON_FALLTHROUGH;
         case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
         values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
@@ -16060,31 +16175,31 @@
         values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_output_file = __Pyx_PyObject_AsWritableString(values[0]); if (unlikely((!__pyx_v_output_file) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_barcodes = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_barcodes.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_features = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_features.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_data = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_data.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_indices = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indices.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_indptr = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indptr.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_M = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_M == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_N = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_N == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
+    __pyx_v_output_file = __Pyx_PyObject_AsWritableString(values[0]); if (unlikely((!__pyx_v_output_file) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_barcodes = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_barcodes.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_features = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_features.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_data = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_data.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_indices = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indices.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_indptr = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indptr.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_M = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_M == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_N = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_N == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
     if (values[8]) {
-      __pyx_v_precision = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_precision == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
+      __pyx_v_precision = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_precision == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
     } else {
-      __pyx_v_precision = __pyx_k__31;
+      __pyx_v_precision = __pyx_k__32;
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_1_0write_dense", 0, 8, 9, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 197, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_1_0write_dense", 0, 8, 9, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 201, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pegasusio.cylib.io.__pyx_fuse_1_1_0write_dense", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9pegasusio_5cylib_2io_56__pyx_fuse_1_1_0write_dense(__pyx_self, __pyx_v_output_file, __pyx_v_barcodes, __pyx_v_features, __pyx_v_data, __pyx_v_indices, __pyx_v_indptr, __pyx_v_M, __pyx_v_N, __pyx_v_precision);
 
@@ -16099,23 +16214,23 @@
   struct __pyx_fuse_1_1_0__pyx_opt_args_9pegasusio_5cylib_2io_write_dense __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_1_1_0write_dense", 0);
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_barcodes.memview)) { __Pyx_RaiseUnboundLocalError("barcodes"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_features.memview)) { __Pyx_RaiseUnboundLocalError("features"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_data.memview)) { __Pyx_RaiseUnboundLocalError("data"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_indices.memview)) { __Pyx_RaiseUnboundLocalError("indices"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_indptr.memview)) { __Pyx_RaiseUnboundLocalError("indptr"); __PYX_ERR(0, 197, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_barcodes.memview)) { __Pyx_RaiseUnboundLocalError("barcodes"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_features.memview)) { __Pyx_RaiseUnboundLocalError("features"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_data.memview)) { __Pyx_RaiseUnboundLocalError("data"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_indices.memview)) { __Pyx_RaiseUnboundLocalError("indices"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_indptr.memview)) { __Pyx_RaiseUnboundLocalError("indptr"); __PYX_ERR(0, 201, __pyx_L1_error) }
   __pyx_t_1.__pyx_n = 1;
   __pyx_t_1.precision = __pyx_v_precision;
   __pyx_fuse_1_1_0__pyx_f_9pegasusio_5cylib_2io_write_dense(__pyx_v_output_file, __pyx_v_barcodes, __pyx_v_features, __pyx_v_data, __pyx_v_indices, __pyx_v_indptr, __pyx_v_M, __pyx_v_N, 0, &__pyx_t_1); 
-  __pyx_t_2 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -16132,15 +16247,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pw_9pegasusio_5cylib_2io_59__pyx_fuse_1_1_1write_dense(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_pw_9pegasusio_5cylib_2io_7write_dense(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static void __pyx_fuse_1_1_1__pyx_f_9pegasusio_5cylib_2io_write_dense(char *__pyx_v_output_file, __Pyx_memviewslice __pyx_v_barcodes, __Pyx_memviewslice __pyx_v_features, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_indices, __Pyx_memviewslice __pyx_v_indptr, int __pyx_v_M, int __pyx_v_N, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_fuse_1_1_1__pyx_opt_args_9pegasusio_5cylib_2io_write_dense *__pyx_optional_args) {
-  int __pyx_v_precision = __pyx_k__32;
+  int __pyx_v_precision = __pyx_k__33;
   FILE *__pyx_v_fo;
   PyObject *__pyx_v_fmt_str = 0;
   char const *__pyx_v_fmt;
   Py_ssize_t __pyx_v_i;
   Py_ssize_t __pyx_v_j;
   CYTHON_UNUSED Py_ssize_t __pyx_v_k;
   Py_ssize_t __pyx_v_fr;
@@ -16172,24 +16287,24 @@
   __Pyx_RefNannySetupContext("__pyx_fuse_1_1_1write_dense", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_precision = __pyx_optional_args->precision;
     }
   }
 
-  /* "ext_modules/io_funcs.pyx":200
+  /* "ext_modules/io_funcs.pyx":204
  *     """ Input must be csr_matrix internal representation, gene by cell (X.T.tocsr()); Output will be gene by cell
  *     """
  *     cdef FILE* fo = fopen(output_file, "w")             # <<<<<<<<<<<<<<
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"
  * 
  */
   __pyx_v_fo = fopen(__pyx_v_output_file, ((char const *)"w"));
 
-  /* "ext_modules/io_funcs.pyx":201
+  /* "ext_modules/io_funcs.pyx":205
  *     """
  *     cdef FILE* fo = fopen(output_file, "w")
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"             # <<<<<<<<<<<<<<
  * 
  *     cdef const char* fmt = fmt_str
  */
   __pyx_t_3 = (0 != 0);
@@ -16198,236 +16313,236 @@
     __pyx_t_2 = __pyx_t_3;
     goto __pyx_L3_bool_binop_done;
   }
   __pyx_t_3 = (0 != 0);
   __pyx_t_2 = __pyx_t_3;
   __pyx_L3_bool_binop_done:;
   if (__pyx_t_2) {
-    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = 0;
     __pyx_t_6 = 127;
-    __Pyx_INCREF(__pyx_kp_u__25);
+    __Pyx_INCREF(__pyx_kp_u__26);
     __pyx_t_5 += 3;
-    __Pyx_GIVEREF(__pyx_kp_u__25);
-    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u__25);
-    __pyx_t_7 = __Pyx_PyUnicode_From_int(__pyx_v_precision, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __Pyx_GIVEREF(__pyx_kp_u__26);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u__26);
+    __pyx_t_7 = __Pyx_PyUnicode_From_int(__pyx_v_precision, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_INCREF(__pyx_n_u_f_2);
     __pyx_t_5 += 1;
     __Pyx_GIVEREF(__pyx_n_u_f_2);
     PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_n_u_f_2);
-    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_1 = __pyx_t_7;
     __pyx_t_7 = 0;
   } else {
     __Pyx_INCREF(__pyx_kp_u_d);
     __pyx_t_1 = __pyx_kp_u_d;
   }
   __pyx_v_fmt_str = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "ext_modules/io_funcs.pyx":203
+  /* "ext_modules/io_funcs.pyx":207
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"
  * 
  *     cdef const char* fmt = fmt_str             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t i, j, k, fr
  * 
  */
-  __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_v_fmt_str); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 203, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_v_fmt_str); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 207, __pyx_L1_error)
   __pyx_v_fmt = __pyx_t_8;
 
-  /* "ext_modules/io_funcs.pyx":206
+  /* "ext_modules/io_funcs.pyx":210
  *     cdef Py_ssize_t i, j, k, fr
  * 
  *     fprintf(fo, "GENE");             # <<<<<<<<<<<<<<
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  */
   (void)(fprintf(__pyx_v_fo, ((char const *)"GENE")));
 
-  /* "ext_modules/io_funcs.pyx":207
+  /* "ext_modules/io_funcs.pyx":211
  * 
  *     fprintf(fo, "GENE");
  *     for i in range(N):             # <<<<<<<<<<<<<<
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  *     fprintf(fo, "\n")
  */
   __pyx_t_9 = __pyx_v_N;
   __pyx_t_10 = __pyx_t_9;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_10; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "ext_modules/io_funcs.pyx":208
+    /* "ext_modules/io_funcs.pyx":212
  *     fprintf(fo, "GENE");
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])             # <<<<<<<<<<<<<<
  *     fprintf(fo, "\n")
  * 
  */
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_1 = (PyObject *) *((PyObject * *) ( /* dim=0 */ (__pyx_v_barcodes.data + __pyx_t_11 * __pyx_v_barcodes.strides[0]) ));
     if (unlikely(__pyx_t_1 == NULL)) __pyx_t_1 = Py_None;
     __Pyx_INCREF((PyObject*)__pyx_t_1);
-    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 208, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 212, __pyx_L1_error)
     (void)(fprintf(__pyx_v_fo, ((char const *)"\t%s"), ((char *)__pyx_t_12)));
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
 
-  /* "ext_modules/io_funcs.pyx":209
+  /* "ext_modules/io_funcs.pyx":213
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  *     fprintf(fo, "\n")             # <<<<<<<<<<<<<<
  * 
  *     for i in range(M):
  */
   (void)(fprintf(__pyx_v_fo, ((char const *)"\n")));
 
-  /* "ext_modules/io_funcs.pyx":211
+  /* "ext_modules/io_funcs.pyx":215
  *     fprintf(fo, "\n")
  * 
  *     for i in range(M):             # <<<<<<<<<<<<<<
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0
  */
   __pyx_t_9 = __pyx_v_M;
   __pyx_t_10 = __pyx_t_9;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_10; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "ext_modules/io_funcs.pyx":212
+    /* "ext_modules/io_funcs.pyx":216
  * 
  *     for i in range(M):
  *         fprintf(fo, "%s", <char*>features[i]);             # <<<<<<<<<<<<<<
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):
  */
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_1 = (PyObject *) *((PyObject * *) ( /* dim=0 */ (__pyx_v_features.data + __pyx_t_11 * __pyx_v_features.strides[0]) ));
     if (unlikely(__pyx_t_1 == NULL)) __pyx_t_1 = Py_None;
     __Pyx_INCREF((PyObject*)__pyx_t_1);
-    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 212, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 216, __pyx_L1_error)
     (void)(fprintf(__pyx_v_fo, ((char const *)"%s"), ((char *)__pyx_t_12)));
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "ext_modules/io_funcs.pyx":213
+    /* "ext_modules/io_funcs.pyx":217
  *     for i in range(M):
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0             # <<<<<<<<<<<<<<
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):
  */
     __pyx_v_fr = 0;
 
-    /* "ext_modules/io_funcs.pyx":214
+    /* "ext_modules/io_funcs.pyx":218
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):             # <<<<<<<<<<<<<<
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")
  */
     __pyx_t_11 = (__pyx_v_i + 1);
     __pyx_t_13 = (*((long *) ( /* dim=0 */ (__pyx_v_indptr.data + __pyx_t_11 * __pyx_v_indptr.strides[0]) )));
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = (*((long *) ( /* dim=0 */ (__pyx_v_indptr.data + __pyx_t_11 * __pyx_v_indptr.strides[0]) ))); __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_j = __pyx_t_15;
 
-      /* "ext_modules/io_funcs.pyx":215
+      /* "ext_modules/io_funcs.pyx":219
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):             # <<<<<<<<<<<<<<
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])
  */
       __pyx_t_16 = __pyx_v_j;
       __pyx_t_17 = (*((long *) ( /* dim=0 */ (__pyx_v_indices.data + __pyx_t_16 * __pyx_v_indices.strides[0]) )));
       __pyx_t_18 = __pyx_t_17;
       for (__pyx_t_19 = __pyx_v_fr; __pyx_t_19 < __pyx_t_18; __pyx_t_19+=1) {
         __pyx_v_k = __pyx_t_19;
 
-        /* "ext_modules/io_funcs.pyx":216
+        /* "ext_modules/io_funcs.pyx":220
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")             # <<<<<<<<<<<<<<
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1
  */
         (void)(fprintf(__pyx_v_fo, ((char const *)"\t0")));
       }
 
-      /* "ext_modules/io_funcs.pyx":217
+      /* "ext_modules/io_funcs.pyx":221
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])             # <<<<<<<<<<<<<<
  *             fr = indices[j] + 1
  *         for k in range(fr, N):
  */
       __pyx_t_16 = __pyx_v_j;
       (void)(fprintf(__pyx_v_fo, __pyx_v_fmt, (*((long *) ( /* dim=0 */ (__pyx_v_data.data + __pyx_t_16 * __pyx_v_data.strides[0]) )))));
 
-      /* "ext_modules/io_funcs.pyx":218
+      /* "ext_modules/io_funcs.pyx":222
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1             # <<<<<<<<<<<<<<
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")
  */
       __pyx_t_16 = __pyx_v_j;
       __pyx_v_fr = ((*((long *) ( /* dim=0 */ (__pyx_v_indices.data + __pyx_t_16 * __pyx_v_indices.strides[0]) ))) + 1);
     }
 
-    /* "ext_modules/io_funcs.pyx":219
+    /* "ext_modules/io_funcs.pyx":223
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1
  *         for k in range(fr, N):             # <<<<<<<<<<<<<<
  *             fprintf(fo, "\t0")
  *         fprintf(fo, "\n")
  */
     __pyx_t_20 = __pyx_v_N;
     __pyx_t_21 = __pyx_t_20;
     for (__pyx_t_15 = __pyx_v_fr; __pyx_t_15 < __pyx_t_21; __pyx_t_15+=1) {
       __pyx_v_k = __pyx_t_15;
 
-      /* "ext_modules/io_funcs.pyx":220
+      /* "ext_modules/io_funcs.pyx":224
  *             fr = indices[j] + 1
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")             # <<<<<<<<<<<<<<
  *         fprintf(fo, "\n")
  * 
  */
       (void)(fprintf(__pyx_v_fo, ((char const *)"\t0")));
     }
 
-    /* "ext_modules/io_funcs.pyx":221
+    /* "ext_modules/io_funcs.pyx":225
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")
  *         fprintf(fo, "\n")             # <<<<<<<<<<<<<<
  * 
  *     fclose(fo)
  */
     (void)(fprintf(__pyx_v_fo, ((char const *)"\n")));
   }
 
-  /* "ext_modules/io_funcs.pyx":223
+  /* "ext_modules/io_funcs.pyx":227
  *         fprintf(fo, "\n")
  * 
  *     fclose(fo)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   (void)(fclose(__pyx_v_fo));
 
-  /* "ext_modules/io_funcs.pyx":197
+  /* "ext_modules/io_funcs.pyx":201
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef void write_dense(char* output_file, str[:] barcodes, str[:] features, data_type[:] data, indices_type[:] indices, indptr_type[:] indptr, int M, int N, int precision = 2):             # <<<<<<<<<<<<<<
  *     """ Input must be csr_matrix internal representation, gene by cell (X.T.tocsr()); Output will be gene by cell
  *     """
  */
 
@@ -16495,61 +16610,61 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_output_file)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_barcodes)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_1_1write_dense", 0, 8, 9, 1); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_1_1write_dense", 0, 8, 9, 1); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_features)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_1_1write_dense", 0, 8, 9, 2); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_1_1write_dense", 0, 8, 9, 2); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_1_1write_dense", 0, 8, 9, 3); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_1_1write_dense", 0, 8, 9, 3); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_indices)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_1_1write_dense", 0, 8, 9, 4); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_1_1write_dense", 0, 8, 9, 4); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_indptr)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_1_1write_dense", 0, 8, 9, 5); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_1_1write_dense", 0, 8, 9, 5); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (likely((values[6] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_M)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_1_1write_dense", 0, 8, 9, 6); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_1_1write_dense", 0, 8, 9, 6); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  7:
         if (likely((values[7] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_N)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_1_1write_dense", 0, 8, 9, 7); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_1_1write_dense", 0, 8, 9, 7); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  8:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_precision);
           if (value) { values[8] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_1_1_1write_dense") < 0)) __PYX_ERR(0, 197, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_1_1_1write_dense") < 0)) __PYX_ERR(0, 201, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  9: values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
         CYTHON_FALLTHROUGH;
         case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
         values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
@@ -16559,31 +16674,31 @@
         values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_output_file = __Pyx_PyObject_AsWritableString(values[0]); if (unlikely((!__pyx_v_output_file) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_barcodes = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_barcodes.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_features = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_features.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_data = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_data.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_indices = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indices.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_indptr = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indptr.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_M = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_M == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_N = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_N == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
+    __pyx_v_output_file = __Pyx_PyObject_AsWritableString(values[0]); if (unlikely((!__pyx_v_output_file) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_barcodes = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_barcodes.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_features = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_features.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_data = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_data.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_indices = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indices.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_indptr = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indptr.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_M = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_M == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_N = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_N == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
     if (values[8]) {
-      __pyx_v_precision = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_precision == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
+      __pyx_v_precision = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_precision == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
     } else {
-      __pyx_v_precision = __pyx_k__32;
+      __pyx_v_precision = __pyx_k__33;
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_1_1write_dense", 0, 8, 9, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 197, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_1_1_1write_dense", 0, 8, 9, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 201, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pegasusio.cylib.io.__pyx_fuse_1_1_1write_dense", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9pegasusio_5cylib_2io_58__pyx_fuse_1_1_1write_dense(__pyx_self, __pyx_v_output_file, __pyx_v_barcodes, __pyx_v_features, __pyx_v_data, __pyx_v_indices, __pyx_v_indptr, __pyx_v_M, __pyx_v_N, __pyx_v_precision);
 
@@ -16598,23 +16713,23 @@
   struct __pyx_fuse_1_1_1__pyx_opt_args_9pegasusio_5cylib_2io_write_dense __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_1_1_1write_dense", 0);
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_barcodes.memview)) { __Pyx_RaiseUnboundLocalError("barcodes"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_features.memview)) { __Pyx_RaiseUnboundLocalError("features"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_data.memview)) { __Pyx_RaiseUnboundLocalError("data"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_indices.memview)) { __Pyx_RaiseUnboundLocalError("indices"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_indptr.memview)) { __Pyx_RaiseUnboundLocalError("indptr"); __PYX_ERR(0, 197, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_barcodes.memview)) { __Pyx_RaiseUnboundLocalError("barcodes"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_features.memview)) { __Pyx_RaiseUnboundLocalError("features"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_data.memview)) { __Pyx_RaiseUnboundLocalError("data"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_indices.memview)) { __Pyx_RaiseUnboundLocalError("indices"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_indptr.memview)) { __Pyx_RaiseUnboundLocalError("indptr"); __PYX_ERR(0, 201, __pyx_L1_error) }
   __pyx_t_1.__pyx_n = 1;
   __pyx_t_1.precision = __pyx_v_precision;
   __pyx_fuse_1_1_1__pyx_f_9pegasusio_5cylib_2io_write_dense(__pyx_v_output_file, __pyx_v_barcodes, __pyx_v_features, __pyx_v_data, __pyx_v_indices, __pyx_v_indptr, __pyx_v_M, __pyx_v_N, 0, &__pyx_t_1); 
-  __pyx_t_2 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -16631,15 +16746,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pw_9pegasusio_5cylib_2io_61__pyx_fuse_2_0_0write_dense(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_pw_9pegasusio_5cylib_2io_7write_dense(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static void __pyx_fuse_2_0_0__pyx_f_9pegasusio_5cylib_2io_write_dense(char *__pyx_v_output_file, __Pyx_memviewslice __pyx_v_barcodes, __Pyx_memviewslice __pyx_v_features, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_indices, __Pyx_memviewslice __pyx_v_indptr, int __pyx_v_M, int __pyx_v_N, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_fuse_2_0_0__pyx_opt_args_9pegasusio_5cylib_2io_write_dense *__pyx_optional_args) {
-  int __pyx_v_precision = __pyx_k__33;
+  int __pyx_v_precision = __pyx_k__34;
   FILE *__pyx_v_fo;
   PyObject *__pyx_v_fmt_str = 0;
   char const *__pyx_v_fmt;
   Py_ssize_t __pyx_v_i;
   Py_ssize_t __pyx_v_j;
   CYTHON_UNUSED Py_ssize_t __pyx_v_k;
   Py_ssize_t __pyx_v_fr;
@@ -16669,24 +16784,24 @@
   __Pyx_RefNannySetupContext("__pyx_fuse_2_0_0write_dense", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_precision = __pyx_optional_args->precision;
     }
   }
 
-  /* "ext_modules/io_funcs.pyx":200
+  /* "ext_modules/io_funcs.pyx":204
  *     """ Input must be csr_matrix internal representation, gene by cell (X.T.tocsr()); Output will be gene by cell
  *     """
  *     cdef FILE* fo = fopen(output_file, "w")             # <<<<<<<<<<<<<<
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"
  * 
  */
   __pyx_v_fo = fopen(__pyx_v_output_file, ((char const *)"w"));
 
-  /* "ext_modules/io_funcs.pyx":201
+  /* "ext_modules/io_funcs.pyx":205
  *     """
  *     cdef FILE* fo = fopen(output_file, "w")
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"             # <<<<<<<<<<<<<<
  * 
  *     cdef const char* fmt = fmt_str
  */
   __pyx_t_3 = (1 != 0);
@@ -16695,236 +16810,236 @@
     __pyx_t_2 = __pyx_t_3;
     goto __pyx_L3_bool_binop_done;
   }
   __pyx_t_3 = (0 != 0);
   __pyx_t_2 = __pyx_t_3;
   __pyx_L3_bool_binop_done:;
   if (__pyx_t_2) {
-    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = 0;
     __pyx_t_6 = 127;
-    __Pyx_INCREF(__pyx_kp_u__25);
+    __Pyx_INCREF(__pyx_kp_u__26);
     __pyx_t_5 += 3;
-    __Pyx_GIVEREF(__pyx_kp_u__25);
-    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u__25);
-    __pyx_t_7 = __Pyx_PyUnicode_From_int(__pyx_v_precision, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __Pyx_GIVEREF(__pyx_kp_u__26);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u__26);
+    __pyx_t_7 = __Pyx_PyUnicode_From_int(__pyx_v_precision, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_INCREF(__pyx_n_u_f_2);
     __pyx_t_5 += 1;
     __Pyx_GIVEREF(__pyx_n_u_f_2);
     PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_n_u_f_2);
-    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_1 = __pyx_t_7;
     __pyx_t_7 = 0;
   } else {
     __Pyx_INCREF(__pyx_kp_u_d);
     __pyx_t_1 = __pyx_kp_u_d;
   }
   __pyx_v_fmt_str = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "ext_modules/io_funcs.pyx":203
+  /* "ext_modules/io_funcs.pyx":207
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"
  * 
  *     cdef const char* fmt = fmt_str             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t i, j, k, fr
  * 
  */
-  __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_v_fmt_str); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 203, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_v_fmt_str); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 207, __pyx_L1_error)
   __pyx_v_fmt = __pyx_t_8;
 
-  /* "ext_modules/io_funcs.pyx":206
+  /* "ext_modules/io_funcs.pyx":210
  *     cdef Py_ssize_t i, j, k, fr
  * 
  *     fprintf(fo, "GENE");             # <<<<<<<<<<<<<<
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  */
   (void)(fprintf(__pyx_v_fo, ((char const *)"GENE")));
 
-  /* "ext_modules/io_funcs.pyx":207
+  /* "ext_modules/io_funcs.pyx":211
  * 
  *     fprintf(fo, "GENE");
  *     for i in range(N):             # <<<<<<<<<<<<<<
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  *     fprintf(fo, "\n")
  */
   __pyx_t_9 = __pyx_v_N;
   __pyx_t_10 = __pyx_t_9;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_10; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "ext_modules/io_funcs.pyx":208
+    /* "ext_modules/io_funcs.pyx":212
  *     fprintf(fo, "GENE");
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])             # <<<<<<<<<<<<<<
  *     fprintf(fo, "\n")
  * 
  */
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_1 = (PyObject *) *((PyObject * *) ( /* dim=0 */ (__pyx_v_barcodes.data + __pyx_t_11 * __pyx_v_barcodes.strides[0]) ));
     if (unlikely(__pyx_t_1 == NULL)) __pyx_t_1 = Py_None;
     __Pyx_INCREF((PyObject*)__pyx_t_1);
-    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 208, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 212, __pyx_L1_error)
     (void)(fprintf(__pyx_v_fo, ((char const *)"\t%s"), ((char *)__pyx_t_12)));
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
 
-  /* "ext_modules/io_funcs.pyx":209
+  /* "ext_modules/io_funcs.pyx":213
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  *     fprintf(fo, "\n")             # <<<<<<<<<<<<<<
  * 
  *     for i in range(M):
  */
   (void)(fprintf(__pyx_v_fo, ((char const *)"\n")));
 
-  /* "ext_modules/io_funcs.pyx":211
+  /* "ext_modules/io_funcs.pyx":215
  *     fprintf(fo, "\n")
  * 
  *     for i in range(M):             # <<<<<<<<<<<<<<
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0
  */
   __pyx_t_9 = __pyx_v_M;
   __pyx_t_10 = __pyx_t_9;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_10; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "ext_modules/io_funcs.pyx":212
+    /* "ext_modules/io_funcs.pyx":216
  * 
  *     for i in range(M):
  *         fprintf(fo, "%s", <char*>features[i]);             # <<<<<<<<<<<<<<
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):
  */
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_1 = (PyObject *) *((PyObject * *) ( /* dim=0 */ (__pyx_v_features.data + __pyx_t_11 * __pyx_v_features.strides[0]) ));
     if (unlikely(__pyx_t_1 == NULL)) __pyx_t_1 = Py_None;
     __Pyx_INCREF((PyObject*)__pyx_t_1);
-    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 212, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 216, __pyx_L1_error)
     (void)(fprintf(__pyx_v_fo, ((char const *)"%s"), ((char *)__pyx_t_12)));
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "ext_modules/io_funcs.pyx":213
+    /* "ext_modules/io_funcs.pyx":217
  *     for i in range(M):
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0             # <<<<<<<<<<<<<<
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):
  */
     __pyx_v_fr = 0;
 
-    /* "ext_modules/io_funcs.pyx":214
+    /* "ext_modules/io_funcs.pyx":218
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):             # <<<<<<<<<<<<<<
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")
  */
     __pyx_t_11 = (__pyx_v_i + 1);
     __pyx_t_13 = (*((int *) ( /* dim=0 */ (__pyx_v_indptr.data + __pyx_t_11 * __pyx_v_indptr.strides[0]) )));
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = (*((int *) ( /* dim=0 */ (__pyx_v_indptr.data + __pyx_t_11 * __pyx_v_indptr.strides[0]) ))); __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_j = __pyx_t_15;
 
-      /* "ext_modules/io_funcs.pyx":215
+      /* "ext_modules/io_funcs.pyx":219
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):             # <<<<<<<<<<<<<<
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])
  */
       __pyx_t_16 = __pyx_v_j;
       __pyx_t_17 = (*((int *) ( /* dim=0 */ (__pyx_v_indices.data + __pyx_t_16 * __pyx_v_indices.strides[0]) )));
       __pyx_t_18 = __pyx_t_17;
       for (__pyx_t_19 = __pyx_v_fr; __pyx_t_19 < __pyx_t_18; __pyx_t_19+=1) {
         __pyx_v_k = __pyx_t_19;
 
-        /* "ext_modules/io_funcs.pyx":216
+        /* "ext_modules/io_funcs.pyx":220
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")             # <<<<<<<<<<<<<<
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1
  */
         (void)(fprintf(__pyx_v_fo, ((char const *)"\t0")));
       }
 
-      /* "ext_modules/io_funcs.pyx":217
+      /* "ext_modules/io_funcs.pyx":221
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])             # <<<<<<<<<<<<<<
  *             fr = indices[j] + 1
  *         for k in range(fr, N):
  */
       __pyx_t_16 = __pyx_v_j;
       (void)(fprintf(__pyx_v_fo, __pyx_v_fmt, (*((float *) ( /* dim=0 */ (__pyx_v_data.data + __pyx_t_16 * __pyx_v_data.strides[0]) )))));
 
-      /* "ext_modules/io_funcs.pyx":218
+      /* "ext_modules/io_funcs.pyx":222
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1             # <<<<<<<<<<<<<<
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")
  */
       __pyx_t_16 = __pyx_v_j;
       __pyx_v_fr = ((*((int *) ( /* dim=0 */ (__pyx_v_indices.data + __pyx_t_16 * __pyx_v_indices.strides[0]) ))) + 1);
     }
 
-    /* "ext_modules/io_funcs.pyx":219
+    /* "ext_modules/io_funcs.pyx":223
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1
  *         for k in range(fr, N):             # <<<<<<<<<<<<<<
  *             fprintf(fo, "\t0")
  *         fprintf(fo, "\n")
  */
     __pyx_t_13 = __pyx_v_N;
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = __pyx_v_fr; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_k = __pyx_t_15;
 
-      /* "ext_modules/io_funcs.pyx":220
+      /* "ext_modules/io_funcs.pyx":224
  *             fr = indices[j] + 1
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")             # <<<<<<<<<<<<<<
  *         fprintf(fo, "\n")
  * 
  */
       (void)(fprintf(__pyx_v_fo, ((char const *)"\t0")));
     }
 
-    /* "ext_modules/io_funcs.pyx":221
+    /* "ext_modules/io_funcs.pyx":225
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")
  *         fprintf(fo, "\n")             # <<<<<<<<<<<<<<
  * 
  *     fclose(fo)
  */
     (void)(fprintf(__pyx_v_fo, ((char const *)"\n")));
   }
 
-  /* "ext_modules/io_funcs.pyx":223
+  /* "ext_modules/io_funcs.pyx":227
  *         fprintf(fo, "\n")
  * 
  *     fclose(fo)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   (void)(fclose(__pyx_v_fo));
 
-  /* "ext_modules/io_funcs.pyx":197
+  /* "ext_modules/io_funcs.pyx":201
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef void write_dense(char* output_file, str[:] barcodes, str[:] features, data_type[:] data, indices_type[:] indices, indptr_type[:] indptr, int M, int N, int precision = 2):             # <<<<<<<<<<<<<<
  *     """ Input must be csr_matrix internal representation, gene by cell (X.T.tocsr()); Output will be gene by cell
  *     """
  */
 
@@ -16992,61 +17107,61 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_output_file)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_barcodes)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_0_0write_dense", 0, 8, 9, 1); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_0_0write_dense", 0, 8, 9, 1); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_features)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_0_0write_dense", 0, 8, 9, 2); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_0_0write_dense", 0, 8, 9, 2); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_0_0write_dense", 0, 8, 9, 3); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_0_0write_dense", 0, 8, 9, 3); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_indices)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_0_0write_dense", 0, 8, 9, 4); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_0_0write_dense", 0, 8, 9, 4); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_indptr)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_0_0write_dense", 0, 8, 9, 5); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_0_0write_dense", 0, 8, 9, 5); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (likely((values[6] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_M)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_0_0write_dense", 0, 8, 9, 6); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_0_0write_dense", 0, 8, 9, 6); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  7:
         if (likely((values[7] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_N)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_0_0write_dense", 0, 8, 9, 7); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_0_0write_dense", 0, 8, 9, 7); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  8:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_precision);
           if (value) { values[8] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_2_0_0write_dense") < 0)) __PYX_ERR(0, 197, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_2_0_0write_dense") < 0)) __PYX_ERR(0, 201, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  9: values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
         CYTHON_FALLTHROUGH;
         case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
         values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
@@ -17056,31 +17171,31 @@
         values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_output_file = __Pyx_PyObject_AsWritableString(values[0]); if (unlikely((!__pyx_v_output_file) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_barcodes = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_barcodes.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_features = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_features.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_data = __Pyx_PyObject_to_MemoryviewSlice_ds_float(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_data.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_indices = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indices.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_indptr = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indptr.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_M = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_M == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_N = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_N == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
+    __pyx_v_output_file = __Pyx_PyObject_AsWritableString(values[0]); if (unlikely((!__pyx_v_output_file) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_barcodes = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_barcodes.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_features = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_features.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_data = __Pyx_PyObject_to_MemoryviewSlice_ds_float(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_data.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_indices = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indices.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_indptr = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indptr.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_M = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_M == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_N = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_N == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
     if (values[8]) {
-      __pyx_v_precision = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_precision == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
+      __pyx_v_precision = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_precision == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
     } else {
-      __pyx_v_precision = __pyx_k__33;
+      __pyx_v_precision = __pyx_k__34;
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_0_0write_dense", 0, 8, 9, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 197, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_0_0write_dense", 0, 8, 9, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 201, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pegasusio.cylib.io.__pyx_fuse_2_0_0write_dense", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9pegasusio_5cylib_2io_60__pyx_fuse_2_0_0write_dense(__pyx_self, __pyx_v_output_file, __pyx_v_barcodes, __pyx_v_features, __pyx_v_data, __pyx_v_indices, __pyx_v_indptr, __pyx_v_M, __pyx_v_N, __pyx_v_precision);
 
@@ -17095,23 +17210,23 @@
   struct __pyx_fuse_2_0_0__pyx_opt_args_9pegasusio_5cylib_2io_write_dense __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_2_0_0write_dense", 0);
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_barcodes.memview)) { __Pyx_RaiseUnboundLocalError("barcodes"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_features.memview)) { __Pyx_RaiseUnboundLocalError("features"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_data.memview)) { __Pyx_RaiseUnboundLocalError("data"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_indices.memview)) { __Pyx_RaiseUnboundLocalError("indices"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_indptr.memview)) { __Pyx_RaiseUnboundLocalError("indptr"); __PYX_ERR(0, 197, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_barcodes.memview)) { __Pyx_RaiseUnboundLocalError("barcodes"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_features.memview)) { __Pyx_RaiseUnboundLocalError("features"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_data.memview)) { __Pyx_RaiseUnboundLocalError("data"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_indices.memview)) { __Pyx_RaiseUnboundLocalError("indices"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_indptr.memview)) { __Pyx_RaiseUnboundLocalError("indptr"); __PYX_ERR(0, 201, __pyx_L1_error) }
   __pyx_t_1.__pyx_n = 1;
   __pyx_t_1.precision = __pyx_v_precision;
   __pyx_fuse_2_0_0__pyx_f_9pegasusio_5cylib_2io_write_dense(__pyx_v_output_file, __pyx_v_barcodes, __pyx_v_features, __pyx_v_data, __pyx_v_indices, __pyx_v_indptr, __pyx_v_M, __pyx_v_N, 0, &__pyx_t_1); 
-  __pyx_t_2 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -17128,15 +17243,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pw_9pegasusio_5cylib_2io_63__pyx_fuse_2_0_1write_dense(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_pw_9pegasusio_5cylib_2io_7write_dense(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static void __pyx_fuse_2_0_1__pyx_f_9pegasusio_5cylib_2io_write_dense(char *__pyx_v_output_file, __Pyx_memviewslice __pyx_v_barcodes, __Pyx_memviewslice __pyx_v_features, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_indices, __Pyx_memviewslice __pyx_v_indptr, int __pyx_v_M, int __pyx_v_N, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_fuse_2_0_1__pyx_opt_args_9pegasusio_5cylib_2io_write_dense *__pyx_optional_args) {
-  int __pyx_v_precision = __pyx_k__34;
+  int __pyx_v_precision = __pyx_k__35;
   FILE *__pyx_v_fo;
   PyObject *__pyx_v_fmt_str = 0;
   char const *__pyx_v_fmt;
   Py_ssize_t __pyx_v_i;
   Py_ssize_t __pyx_v_j;
   CYTHON_UNUSED Py_ssize_t __pyx_v_k;
   Py_ssize_t __pyx_v_fr;
@@ -17166,24 +17281,24 @@
   __Pyx_RefNannySetupContext("__pyx_fuse_2_0_1write_dense", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_precision = __pyx_optional_args->precision;
     }
   }
 
-  /* "ext_modules/io_funcs.pyx":200
+  /* "ext_modules/io_funcs.pyx":204
  *     """ Input must be csr_matrix internal representation, gene by cell (X.T.tocsr()); Output will be gene by cell
  *     """
  *     cdef FILE* fo = fopen(output_file, "w")             # <<<<<<<<<<<<<<
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"
  * 
  */
   __pyx_v_fo = fopen(__pyx_v_output_file, ((char const *)"w"));
 
-  /* "ext_modules/io_funcs.pyx":201
+  /* "ext_modules/io_funcs.pyx":205
  *     """
  *     cdef FILE* fo = fopen(output_file, "w")
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"             # <<<<<<<<<<<<<<
  * 
  *     cdef const char* fmt = fmt_str
  */
   __pyx_t_3 = (1 != 0);
@@ -17192,236 +17307,236 @@
     __pyx_t_2 = __pyx_t_3;
     goto __pyx_L3_bool_binop_done;
   }
   __pyx_t_3 = (0 != 0);
   __pyx_t_2 = __pyx_t_3;
   __pyx_L3_bool_binop_done:;
   if (__pyx_t_2) {
-    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = 0;
     __pyx_t_6 = 127;
-    __Pyx_INCREF(__pyx_kp_u__25);
+    __Pyx_INCREF(__pyx_kp_u__26);
     __pyx_t_5 += 3;
-    __Pyx_GIVEREF(__pyx_kp_u__25);
-    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u__25);
-    __pyx_t_7 = __Pyx_PyUnicode_From_int(__pyx_v_precision, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __Pyx_GIVEREF(__pyx_kp_u__26);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u__26);
+    __pyx_t_7 = __Pyx_PyUnicode_From_int(__pyx_v_precision, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_INCREF(__pyx_n_u_f_2);
     __pyx_t_5 += 1;
     __Pyx_GIVEREF(__pyx_n_u_f_2);
     PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_n_u_f_2);
-    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_1 = __pyx_t_7;
     __pyx_t_7 = 0;
   } else {
     __Pyx_INCREF(__pyx_kp_u_d);
     __pyx_t_1 = __pyx_kp_u_d;
   }
   __pyx_v_fmt_str = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "ext_modules/io_funcs.pyx":203
+  /* "ext_modules/io_funcs.pyx":207
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"
  * 
  *     cdef const char* fmt = fmt_str             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t i, j, k, fr
  * 
  */
-  __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_v_fmt_str); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 203, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_v_fmt_str); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 207, __pyx_L1_error)
   __pyx_v_fmt = __pyx_t_8;
 
-  /* "ext_modules/io_funcs.pyx":206
+  /* "ext_modules/io_funcs.pyx":210
  *     cdef Py_ssize_t i, j, k, fr
  * 
  *     fprintf(fo, "GENE");             # <<<<<<<<<<<<<<
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  */
   (void)(fprintf(__pyx_v_fo, ((char const *)"GENE")));
 
-  /* "ext_modules/io_funcs.pyx":207
+  /* "ext_modules/io_funcs.pyx":211
  * 
  *     fprintf(fo, "GENE");
  *     for i in range(N):             # <<<<<<<<<<<<<<
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  *     fprintf(fo, "\n")
  */
   __pyx_t_9 = __pyx_v_N;
   __pyx_t_10 = __pyx_t_9;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_10; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "ext_modules/io_funcs.pyx":208
+    /* "ext_modules/io_funcs.pyx":212
  *     fprintf(fo, "GENE");
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])             # <<<<<<<<<<<<<<
  *     fprintf(fo, "\n")
  * 
  */
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_1 = (PyObject *) *((PyObject * *) ( /* dim=0 */ (__pyx_v_barcodes.data + __pyx_t_11 * __pyx_v_barcodes.strides[0]) ));
     if (unlikely(__pyx_t_1 == NULL)) __pyx_t_1 = Py_None;
     __Pyx_INCREF((PyObject*)__pyx_t_1);
-    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 208, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 212, __pyx_L1_error)
     (void)(fprintf(__pyx_v_fo, ((char const *)"\t%s"), ((char *)__pyx_t_12)));
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
 
-  /* "ext_modules/io_funcs.pyx":209
+  /* "ext_modules/io_funcs.pyx":213
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  *     fprintf(fo, "\n")             # <<<<<<<<<<<<<<
  * 
  *     for i in range(M):
  */
   (void)(fprintf(__pyx_v_fo, ((char const *)"\n")));
 
-  /* "ext_modules/io_funcs.pyx":211
+  /* "ext_modules/io_funcs.pyx":215
  *     fprintf(fo, "\n")
  * 
  *     for i in range(M):             # <<<<<<<<<<<<<<
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0
  */
   __pyx_t_9 = __pyx_v_M;
   __pyx_t_10 = __pyx_t_9;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_10; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "ext_modules/io_funcs.pyx":212
+    /* "ext_modules/io_funcs.pyx":216
  * 
  *     for i in range(M):
  *         fprintf(fo, "%s", <char*>features[i]);             # <<<<<<<<<<<<<<
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):
  */
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_1 = (PyObject *) *((PyObject * *) ( /* dim=0 */ (__pyx_v_features.data + __pyx_t_11 * __pyx_v_features.strides[0]) ));
     if (unlikely(__pyx_t_1 == NULL)) __pyx_t_1 = Py_None;
     __Pyx_INCREF((PyObject*)__pyx_t_1);
-    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 212, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 216, __pyx_L1_error)
     (void)(fprintf(__pyx_v_fo, ((char const *)"%s"), ((char *)__pyx_t_12)));
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "ext_modules/io_funcs.pyx":213
+    /* "ext_modules/io_funcs.pyx":217
  *     for i in range(M):
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0             # <<<<<<<<<<<<<<
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):
  */
     __pyx_v_fr = 0;
 
-    /* "ext_modules/io_funcs.pyx":214
+    /* "ext_modules/io_funcs.pyx":218
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):             # <<<<<<<<<<<<<<
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")
  */
     __pyx_t_11 = (__pyx_v_i + 1);
     __pyx_t_13 = (*((long *) ( /* dim=0 */ (__pyx_v_indptr.data + __pyx_t_11 * __pyx_v_indptr.strides[0]) )));
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = (*((long *) ( /* dim=0 */ (__pyx_v_indptr.data + __pyx_t_11 * __pyx_v_indptr.strides[0]) ))); __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_j = __pyx_t_15;
 
-      /* "ext_modules/io_funcs.pyx":215
+      /* "ext_modules/io_funcs.pyx":219
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):             # <<<<<<<<<<<<<<
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])
  */
       __pyx_t_16 = __pyx_v_j;
       __pyx_t_17 = (*((int *) ( /* dim=0 */ (__pyx_v_indices.data + __pyx_t_16 * __pyx_v_indices.strides[0]) )));
       __pyx_t_18 = __pyx_t_17;
       for (__pyx_t_19 = __pyx_v_fr; __pyx_t_19 < __pyx_t_18; __pyx_t_19+=1) {
         __pyx_v_k = __pyx_t_19;
 
-        /* "ext_modules/io_funcs.pyx":216
+        /* "ext_modules/io_funcs.pyx":220
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")             # <<<<<<<<<<<<<<
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1
  */
         (void)(fprintf(__pyx_v_fo, ((char const *)"\t0")));
       }
 
-      /* "ext_modules/io_funcs.pyx":217
+      /* "ext_modules/io_funcs.pyx":221
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])             # <<<<<<<<<<<<<<
  *             fr = indices[j] + 1
  *         for k in range(fr, N):
  */
       __pyx_t_16 = __pyx_v_j;
       (void)(fprintf(__pyx_v_fo, __pyx_v_fmt, (*((float *) ( /* dim=0 */ (__pyx_v_data.data + __pyx_t_16 * __pyx_v_data.strides[0]) )))));
 
-      /* "ext_modules/io_funcs.pyx":218
+      /* "ext_modules/io_funcs.pyx":222
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1             # <<<<<<<<<<<<<<
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")
  */
       __pyx_t_16 = __pyx_v_j;
       __pyx_v_fr = ((*((int *) ( /* dim=0 */ (__pyx_v_indices.data + __pyx_t_16 * __pyx_v_indices.strides[0]) ))) + 1);
     }
 
-    /* "ext_modules/io_funcs.pyx":219
+    /* "ext_modules/io_funcs.pyx":223
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1
  *         for k in range(fr, N):             # <<<<<<<<<<<<<<
  *             fprintf(fo, "\t0")
  *         fprintf(fo, "\n")
  */
     __pyx_t_17 = __pyx_v_N;
     __pyx_t_18 = __pyx_t_17;
     for (__pyx_t_15 = __pyx_v_fr; __pyx_t_15 < __pyx_t_18; __pyx_t_15+=1) {
       __pyx_v_k = __pyx_t_15;
 
-      /* "ext_modules/io_funcs.pyx":220
+      /* "ext_modules/io_funcs.pyx":224
  *             fr = indices[j] + 1
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")             # <<<<<<<<<<<<<<
  *         fprintf(fo, "\n")
  * 
  */
       (void)(fprintf(__pyx_v_fo, ((char const *)"\t0")));
     }
 
-    /* "ext_modules/io_funcs.pyx":221
+    /* "ext_modules/io_funcs.pyx":225
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")
  *         fprintf(fo, "\n")             # <<<<<<<<<<<<<<
  * 
  *     fclose(fo)
  */
     (void)(fprintf(__pyx_v_fo, ((char const *)"\n")));
   }
 
-  /* "ext_modules/io_funcs.pyx":223
+  /* "ext_modules/io_funcs.pyx":227
  *         fprintf(fo, "\n")
  * 
  *     fclose(fo)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   (void)(fclose(__pyx_v_fo));
 
-  /* "ext_modules/io_funcs.pyx":197
+  /* "ext_modules/io_funcs.pyx":201
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef void write_dense(char* output_file, str[:] barcodes, str[:] features, data_type[:] data, indices_type[:] indices, indptr_type[:] indptr, int M, int N, int precision = 2):             # <<<<<<<<<<<<<<
  *     """ Input must be csr_matrix internal representation, gene by cell (X.T.tocsr()); Output will be gene by cell
  *     """
  */
 
@@ -17489,61 +17604,61 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_output_file)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_barcodes)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_0_1write_dense", 0, 8, 9, 1); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_0_1write_dense", 0, 8, 9, 1); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_features)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_0_1write_dense", 0, 8, 9, 2); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_0_1write_dense", 0, 8, 9, 2); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_0_1write_dense", 0, 8, 9, 3); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_0_1write_dense", 0, 8, 9, 3); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_indices)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_0_1write_dense", 0, 8, 9, 4); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_0_1write_dense", 0, 8, 9, 4); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_indptr)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_0_1write_dense", 0, 8, 9, 5); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_0_1write_dense", 0, 8, 9, 5); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (likely((values[6] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_M)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_0_1write_dense", 0, 8, 9, 6); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_0_1write_dense", 0, 8, 9, 6); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  7:
         if (likely((values[7] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_N)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_0_1write_dense", 0, 8, 9, 7); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_0_1write_dense", 0, 8, 9, 7); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  8:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_precision);
           if (value) { values[8] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_2_0_1write_dense") < 0)) __PYX_ERR(0, 197, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_2_0_1write_dense") < 0)) __PYX_ERR(0, 201, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  9: values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
         CYTHON_FALLTHROUGH;
         case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
         values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
@@ -17553,31 +17668,31 @@
         values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_output_file = __Pyx_PyObject_AsWritableString(values[0]); if (unlikely((!__pyx_v_output_file) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_barcodes = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_barcodes.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_features = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_features.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_data = __Pyx_PyObject_to_MemoryviewSlice_ds_float(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_data.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_indices = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indices.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_indptr = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indptr.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_M = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_M == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_N = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_N == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
+    __pyx_v_output_file = __Pyx_PyObject_AsWritableString(values[0]); if (unlikely((!__pyx_v_output_file) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_barcodes = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_barcodes.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_features = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_features.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_data = __Pyx_PyObject_to_MemoryviewSlice_ds_float(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_data.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_indices = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indices.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_indptr = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indptr.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_M = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_M == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_N = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_N == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
     if (values[8]) {
-      __pyx_v_precision = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_precision == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
+      __pyx_v_precision = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_precision == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
     } else {
-      __pyx_v_precision = __pyx_k__34;
+      __pyx_v_precision = __pyx_k__35;
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_0_1write_dense", 0, 8, 9, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 197, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_0_1write_dense", 0, 8, 9, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 201, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pegasusio.cylib.io.__pyx_fuse_2_0_1write_dense", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9pegasusio_5cylib_2io_62__pyx_fuse_2_0_1write_dense(__pyx_self, __pyx_v_output_file, __pyx_v_barcodes, __pyx_v_features, __pyx_v_data, __pyx_v_indices, __pyx_v_indptr, __pyx_v_M, __pyx_v_N, __pyx_v_precision);
 
@@ -17592,23 +17707,23 @@
   struct __pyx_fuse_2_0_1__pyx_opt_args_9pegasusio_5cylib_2io_write_dense __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_2_0_1write_dense", 0);
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_barcodes.memview)) { __Pyx_RaiseUnboundLocalError("barcodes"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_features.memview)) { __Pyx_RaiseUnboundLocalError("features"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_data.memview)) { __Pyx_RaiseUnboundLocalError("data"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_indices.memview)) { __Pyx_RaiseUnboundLocalError("indices"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_indptr.memview)) { __Pyx_RaiseUnboundLocalError("indptr"); __PYX_ERR(0, 197, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_barcodes.memview)) { __Pyx_RaiseUnboundLocalError("barcodes"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_features.memview)) { __Pyx_RaiseUnboundLocalError("features"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_data.memview)) { __Pyx_RaiseUnboundLocalError("data"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_indices.memview)) { __Pyx_RaiseUnboundLocalError("indices"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_indptr.memview)) { __Pyx_RaiseUnboundLocalError("indptr"); __PYX_ERR(0, 201, __pyx_L1_error) }
   __pyx_t_1.__pyx_n = 1;
   __pyx_t_1.precision = __pyx_v_precision;
   __pyx_fuse_2_0_1__pyx_f_9pegasusio_5cylib_2io_write_dense(__pyx_v_output_file, __pyx_v_barcodes, __pyx_v_features, __pyx_v_data, __pyx_v_indices, __pyx_v_indptr, __pyx_v_M, __pyx_v_N, 0, &__pyx_t_1); 
-  __pyx_t_2 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -17625,15 +17740,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pw_9pegasusio_5cylib_2io_65__pyx_fuse_2_1_0write_dense(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_pw_9pegasusio_5cylib_2io_7write_dense(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static void __pyx_fuse_2_1_0__pyx_f_9pegasusio_5cylib_2io_write_dense(char *__pyx_v_output_file, __Pyx_memviewslice __pyx_v_barcodes, __Pyx_memviewslice __pyx_v_features, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_indices, __Pyx_memviewslice __pyx_v_indptr, int __pyx_v_M, int __pyx_v_N, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_fuse_2_1_0__pyx_opt_args_9pegasusio_5cylib_2io_write_dense *__pyx_optional_args) {
-  int __pyx_v_precision = __pyx_k__35;
+  int __pyx_v_precision = __pyx_k__36;
   FILE *__pyx_v_fo;
   PyObject *__pyx_v_fmt_str = 0;
   char const *__pyx_v_fmt;
   Py_ssize_t __pyx_v_i;
   Py_ssize_t __pyx_v_j;
   CYTHON_UNUSED Py_ssize_t __pyx_v_k;
   Py_ssize_t __pyx_v_fr;
@@ -17663,24 +17778,24 @@
   __Pyx_RefNannySetupContext("__pyx_fuse_2_1_0write_dense", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_precision = __pyx_optional_args->precision;
     }
   }
 
-  /* "ext_modules/io_funcs.pyx":200
+  /* "ext_modules/io_funcs.pyx":204
  *     """ Input must be csr_matrix internal representation, gene by cell (X.T.tocsr()); Output will be gene by cell
  *     """
  *     cdef FILE* fo = fopen(output_file, "w")             # <<<<<<<<<<<<<<
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"
  * 
  */
   __pyx_v_fo = fopen(__pyx_v_output_file, ((char const *)"w"));
 
-  /* "ext_modules/io_funcs.pyx":201
+  /* "ext_modules/io_funcs.pyx":205
  *     """
  *     cdef FILE* fo = fopen(output_file, "w")
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"             # <<<<<<<<<<<<<<
  * 
  *     cdef const char* fmt = fmt_str
  */
   __pyx_t_3 = (1 != 0);
@@ -17689,236 +17804,236 @@
     __pyx_t_2 = __pyx_t_3;
     goto __pyx_L3_bool_binop_done;
   }
   __pyx_t_3 = (0 != 0);
   __pyx_t_2 = __pyx_t_3;
   __pyx_L3_bool_binop_done:;
   if (__pyx_t_2) {
-    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = 0;
     __pyx_t_6 = 127;
-    __Pyx_INCREF(__pyx_kp_u__25);
+    __Pyx_INCREF(__pyx_kp_u__26);
     __pyx_t_5 += 3;
-    __Pyx_GIVEREF(__pyx_kp_u__25);
-    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u__25);
-    __pyx_t_7 = __Pyx_PyUnicode_From_int(__pyx_v_precision, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __Pyx_GIVEREF(__pyx_kp_u__26);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u__26);
+    __pyx_t_7 = __Pyx_PyUnicode_From_int(__pyx_v_precision, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_INCREF(__pyx_n_u_f_2);
     __pyx_t_5 += 1;
     __Pyx_GIVEREF(__pyx_n_u_f_2);
     PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_n_u_f_2);
-    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_1 = __pyx_t_7;
     __pyx_t_7 = 0;
   } else {
     __Pyx_INCREF(__pyx_kp_u_d);
     __pyx_t_1 = __pyx_kp_u_d;
   }
   __pyx_v_fmt_str = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "ext_modules/io_funcs.pyx":203
+  /* "ext_modules/io_funcs.pyx":207
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"
  * 
  *     cdef const char* fmt = fmt_str             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t i, j, k, fr
  * 
  */
-  __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_v_fmt_str); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 203, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_v_fmt_str); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 207, __pyx_L1_error)
   __pyx_v_fmt = __pyx_t_8;
 
-  /* "ext_modules/io_funcs.pyx":206
+  /* "ext_modules/io_funcs.pyx":210
  *     cdef Py_ssize_t i, j, k, fr
  * 
  *     fprintf(fo, "GENE");             # <<<<<<<<<<<<<<
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  */
   (void)(fprintf(__pyx_v_fo, ((char const *)"GENE")));
 
-  /* "ext_modules/io_funcs.pyx":207
+  /* "ext_modules/io_funcs.pyx":211
  * 
  *     fprintf(fo, "GENE");
  *     for i in range(N):             # <<<<<<<<<<<<<<
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  *     fprintf(fo, "\n")
  */
   __pyx_t_9 = __pyx_v_N;
   __pyx_t_10 = __pyx_t_9;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_10; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "ext_modules/io_funcs.pyx":208
+    /* "ext_modules/io_funcs.pyx":212
  *     fprintf(fo, "GENE");
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])             # <<<<<<<<<<<<<<
  *     fprintf(fo, "\n")
  * 
  */
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_1 = (PyObject *) *((PyObject * *) ( /* dim=0 */ (__pyx_v_barcodes.data + __pyx_t_11 * __pyx_v_barcodes.strides[0]) ));
     if (unlikely(__pyx_t_1 == NULL)) __pyx_t_1 = Py_None;
     __Pyx_INCREF((PyObject*)__pyx_t_1);
-    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 208, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 212, __pyx_L1_error)
     (void)(fprintf(__pyx_v_fo, ((char const *)"\t%s"), ((char *)__pyx_t_12)));
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
 
-  /* "ext_modules/io_funcs.pyx":209
+  /* "ext_modules/io_funcs.pyx":213
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  *     fprintf(fo, "\n")             # <<<<<<<<<<<<<<
  * 
  *     for i in range(M):
  */
   (void)(fprintf(__pyx_v_fo, ((char const *)"\n")));
 
-  /* "ext_modules/io_funcs.pyx":211
+  /* "ext_modules/io_funcs.pyx":215
  *     fprintf(fo, "\n")
  * 
  *     for i in range(M):             # <<<<<<<<<<<<<<
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0
  */
   __pyx_t_9 = __pyx_v_M;
   __pyx_t_10 = __pyx_t_9;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_10; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "ext_modules/io_funcs.pyx":212
+    /* "ext_modules/io_funcs.pyx":216
  * 
  *     for i in range(M):
  *         fprintf(fo, "%s", <char*>features[i]);             # <<<<<<<<<<<<<<
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):
  */
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_1 = (PyObject *) *((PyObject * *) ( /* dim=0 */ (__pyx_v_features.data + __pyx_t_11 * __pyx_v_features.strides[0]) ));
     if (unlikely(__pyx_t_1 == NULL)) __pyx_t_1 = Py_None;
     __Pyx_INCREF((PyObject*)__pyx_t_1);
-    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 212, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 216, __pyx_L1_error)
     (void)(fprintf(__pyx_v_fo, ((char const *)"%s"), ((char *)__pyx_t_12)));
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "ext_modules/io_funcs.pyx":213
+    /* "ext_modules/io_funcs.pyx":217
  *     for i in range(M):
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0             # <<<<<<<<<<<<<<
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):
  */
     __pyx_v_fr = 0;
 
-    /* "ext_modules/io_funcs.pyx":214
+    /* "ext_modules/io_funcs.pyx":218
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):             # <<<<<<<<<<<<<<
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")
  */
     __pyx_t_11 = (__pyx_v_i + 1);
     __pyx_t_13 = (*((int *) ( /* dim=0 */ (__pyx_v_indptr.data + __pyx_t_11 * __pyx_v_indptr.strides[0]) )));
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = (*((int *) ( /* dim=0 */ (__pyx_v_indptr.data + __pyx_t_11 * __pyx_v_indptr.strides[0]) ))); __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_j = __pyx_t_15;
 
-      /* "ext_modules/io_funcs.pyx":215
+      /* "ext_modules/io_funcs.pyx":219
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):             # <<<<<<<<<<<<<<
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])
  */
       __pyx_t_16 = __pyx_v_j;
       __pyx_t_17 = (*((long *) ( /* dim=0 */ (__pyx_v_indices.data + __pyx_t_16 * __pyx_v_indices.strides[0]) )));
       __pyx_t_18 = __pyx_t_17;
       for (__pyx_t_19 = __pyx_v_fr; __pyx_t_19 < __pyx_t_18; __pyx_t_19+=1) {
         __pyx_v_k = __pyx_t_19;
 
-        /* "ext_modules/io_funcs.pyx":216
+        /* "ext_modules/io_funcs.pyx":220
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")             # <<<<<<<<<<<<<<
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1
  */
         (void)(fprintf(__pyx_v_fo, ((char const *)"\t0")));
       }
 
-      /* "ext_modules/io_funcs.pyx":217
+      /* "ext_modules/io_funcs.pyx":221
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])             # <<<<<<<<<<<<<<
  *             fr = indices[j] + 1
  *         for k in range(fr, N):
  */
       __pyx_t_16 = __pyx_v_j;
       (void)(fprintf(__pyx_v_fo, __pyx_v_fmt, (*((float *) ( /* dim=0 */ (__pyx_v_data.data + __pyx_t_16 * __pyx_v_data.strides[0]) )))));
 
-      /* "ext_modules/io_funcs.pyx":218
+      /* "ext_modules/io_funcs.pyx":222
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1             # <<<<<<<<<<<<<<
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")
  */
       __pyx_t_16 = __pyx_v_j;
       __pyx_v_fr = ((*((long *) ( /* dim=0 */ (__pyx_v_indices.data + __pyx_t_16 * __pyx_v_indices.strides[0]) ))) + 1);
     }
 
-    /* "ext_modules/io_funcs.pyx":219
+    /* "ext_modules/io_funcs.pyx":223
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1
  *         for k in range(fr, N):             # <<<<<<<<<<<<<<
  *             fprintf(fo, "\t0")
  *         fprintf(fo, "\n")
  */
     __pyx_t_13 = __pyx_v_N;
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = __pyx_v_fr; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_k = __pyx_t_15;
 
-      /* "ext_modules/io_funcs.pyx":220
+      /* "ext_modules/io_funcs.pyx":224
  *             fr = indices[j] + 1
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")             # <<<<<<<<<<<<<<
  *         fprintf(fo, "\n")
  * 
  */
       (void)(fprintf(__pyx_v_fo, ((char const *)"\t0")));
     }
 
-    /* "ext_modules/io_funcs.pyx":221
+    /* "ext_modules/io_funcs.pyx":225
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")
  *         fprintf(fo, "\n")             # <<<<<<<<<<<<<<
  * 
  *     fclose(fo)
  */
     (void)(fprintf(__pyx_v_fo, ((char const *)"\n")));
   }
 
-  /* "ext_modules/io_funcs.pyx":223
+  /* "ext_modules/io_funcs.pyx":227
  *         fprintf(fo, "\n")
  * 
  *     fclose(fo)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   (void)(fclose(__pyx_v_fo));
 
-  /* "ext_modules/io_funcs.pyx":197
+  /* "ext_modules/io_funcs.pyx":201
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef void write_dense(char* output_file, str[:] barcodes, str[:] features, data_type[:] data, indices_type[:] indices, indptr_type[:] indptr, int M, int N, int precision = 2):             # <<<<<<<<<<<<<<
  *     """ Input must be csr_matrix internal representation, gene by cell (X.T.tocsr()); Output will be gene by cell
  *     """
  */
 
@@ -17986,61 +18101,61 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_output_file)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_barcodes)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_1_0write_dense", 0, 8, 9, 1); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_1_0write_dense", 0, 8, 9, 1); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_features)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_1_0write_dense", 0, 8, 9, 2); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_1_0write_dense", 0, 8, 9, 2); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_1_0write_dense", 0, 8, 9, 3); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_1_0write_dense", 0, 8, 9, 3); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_indices)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_1_0write_dense", 0, 8, 9, 4); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_1_0write_dense", 0, 8, 9, 4); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_indptr)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_1_0write_dense", 0, 8, 9, 5); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_1_0write_dense", 0, 8, 9, 5); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (likely((values[6] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_M)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_1_0write_dense", 0, 8, 9, 6); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_1_0write_dense", 0, 8, 9, 6); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  7:
         if (likely((values[7] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_N)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_1_0write_dense", 0, 8, 9, 7); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_1_0write_dense", 0, 8, 9, 7); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  8:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_precision);
           if (value) { values[8] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_2_1_0write_dense") < 0)) __PYX_ERR(0, 197, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_2_1_0write_dense") < 0)) __PYX_ERR(0, 201, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  9: values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
         CYTHON_FALLTHROUGH;
         case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
         values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
@@ -18050,31 +18165,31 @@
         values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_output_file = __Pyx_PyObject_AsWritableString(values[0]); if (unlikely((!__pyx_v_output_file) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_barcodes = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_barcodes.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_features = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_features.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_data = __Pyx_PyObject_to_MemoryviewSlice_ds_float(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_data.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_indices = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indices.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_indptr = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indptr.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_M = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_M == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_N = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_N == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
+    __pyx_v_output_file = __Pyx_PyObject_AsWritableString(values[0]); if (unlikely((!__pyx_v_output_file) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_barcodes = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_barcodes.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_features = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_features.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_data = __Pyx_PyObject_to_MemoryviewSlice_ds_float(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_data.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_indices = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indices.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_indptr = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indptr.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_M = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_M == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_N = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_N == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
     if (values[8]) {
-      __pyx_v_precision = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_precision == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
+      __pyx_v_precision = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_precision == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
     } else {
-      __pyx_v_precision = __pyx_k__35;
+      __pyx_v_precision = __pyx_k__36;
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_1_0write_dense", 0, 8, 9, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 197, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_1_0write_dense", 0, 8, 9, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 201, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pegasusio.cylib.io.__pyx_fuse_2_1_0write_dense", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9pegasusio_5cylib_2io_64__pyx_fuse_2_1_0write_dense(__pyx_self, __pyx_v_output_file, __pyx_v_barcodes, __pyx_v_features, __pyx_v_data, __pyx_v_indices, __pyx_v_indptr, __pyx_v_M, __pyx_v_N, __pyx_v_precision);
 
@@ -18089,23 +18204,23 @@
   struct __pyx_fuse_2_1_0__pyx_opt_args_9pegasusio_5cylib_2io_write_dense __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_2_1_0write_dense", 0);
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_barcodes.memview)) { __Pyx_RaiseUnboundLocalError("barcodes"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_features.memview)) { __Pyx_RaiseUnboundLocalError("features"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_data.memview)) { __Pyx_RaiseUnboundLocalError("data"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_indices.memview)) { __Pyx_RaiseUnboundLocalError("indices"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_indptr.memview)) { __Pyx_RaiseUnboundLocalError("indptr"); __PYX_ERR(0, 197, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_barcodes.memview)) { __Pyx_RaiseUnboundLocalError("barcodes"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_features.memview)) { __Pyx_RaiseUnboundLocalError("features"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_data.memview)) { __Pyx_RaiseUnboundLocalError("data"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_indices.memview)) { __Pyx_RaiseUnboundLocalError("indices"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_indptr.memview)) { __Pyx_RaiseUnboundLocalError("indptr"); __PYX_ERR(0, 201, __pyx_L1_error) }
   __pyx_t_1.__pyx_n = 1;
   __pyx_t_1.precision = __pyx_v_precision;
   __pyx_fuse_2_1_0__pyx_f_9pegasusio_5cylib_2io_write_dense(__pyx_v_output_file, __pyx_v_barcodes, __pyx_v_features, __pyx_v_data, __pyx_v_indices, __pyx_v_indptr, __pyx_v_M, __pyx_v_N, 0, &__pyx_t_1); 
-  __pyx_t_2 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -18122,15 +18237,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pw_9pegasusio_5cylib_2io_67__pyx_fuse_2_1_1write_dense(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_pw_9pegasusio_5cylib_2io_7write_dense(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static void __pyx_fuse_2_1_1__pyx_f_9pegasusio_5cylib_2io_write_dense(char *__pyx_v_output_file, __Pyx_memviewslice __pyx_v_barcodes, __Pyx_memviewslice __pyx_v_features, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_indices, __Pyx_memviewslice __pyx_v_indptr, int __pyx_v_M, int __pyx_v_N, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_fuse_2_1_1__pyx_opt_args_9pegasusio_5cylib_2io_write_dense *__pyx_optional_args) {
-  int __pyx_v_precision = __pyx_k__36;
+  int __pyx_v_precision = __pyx_k__37;
   FILE *__pyx_v_fo;
   PyObject *__pyx_v_fmt_str = 0;
   char const *__pyx_v_fmt;
   Py_ssize_t __pyx_v_i;
   Py_ssize_t __pyx_v_j;
   CYTHON_UNUSED Py_ssize_t __pyx_v_k;
   Py_ssize_t __pyx_v_fr;
@@ -18162,24 +18277,24 @@
   __Pyx_RefNannySetupContext("__pyx_fuse_2_1_1write_dense", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_precision = __pyx_optional_args->precision;
     }
   }
 
-  /* "ext_modules/io_funcs.pyx":200
+  /* "ext_modules/io_funcs.pyx":204
  *     """ Input must be csr_matrix internal representation, gene by cell (X.T.tocsr()); Output will be gene by cell
  *     """
  *     cdef FILE* fo = fopen(output_file, "w")             # <<<<<<<<<<<<<<
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"
  * 
  */
   __pyx_v_fo = fopen(__pyx_v_output_file, ((char const *)"w"));
 
-  /* "ext_modules/io_funcs.pyx":201
+  /* "ext_modules/io_funcs.pyx":205
  *     """
  *     cdef FILE* fo = fopen(output_file, "w")
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"             # <<<<<<<<<<<<<<
  * 
  *     cdef const char* fmt = fmt_str
  */
   __pyx_t_3 = (1 != 0);
@@ -18188,236 +18303,236 @@
     __pyx_t_2 = __pyx_t_3;
     goto __pyx_L3_bool_binop_done;
   }
   __pyx_t_3 = (0 != 0);
   __pyx_t_2 = __pyx_t_3;
   __pyx_L3_bool_binop_done:;
   if (__pyx_t_2) {
-    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = 0;
     __pyx_t_6 = 127;
-    __Pyx_INCREF(__pyx_kp_u__25);
+    __Pyx_INCREF(__pyx_kp_u__26);
     __pyx_t_5 += 3;
-    __Pyx_GIVEREF(__pyx_kp_u__25);
-    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u__25);
-    __pyx_t_7 = __Pyx_PyUnicode_From_int(__pyx_v_precision, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __Pyx_GIVEREF(__pyx_kp_u__26);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u__26);
+    __pyx_t_7 = __Pyx_PyUnicode_From_int(__pyx_v_precision, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_INCREF(__pyx_n_u_f_2);
     __pyx_t_5 += 1;
     __Pyx_GIVEREF(__pyx_n_u_f_2);
     PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_n_u_f_2);
-    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_1 = __pyx_t_7;
     __pyx_t_7 = 0;
   } else {
     __Pyx_INCREF(__pyx_kp_u_d);
     __pyx_t_1 = __pyx_kp_u_d;
   }
   __pyx_v_fmt_str = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "ext_modules/io_funcs.pyx":203
+  /* "ext_modules/io_funcs.pyx":207
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"
  * 
  *     cdef const char* fmt = fmt_str             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t i, j, k, fr
  * 
  */
-  __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_v_fmt_str); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 203, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_v_fmt_str); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 207, __pyx_L1_error)
   __pyx_v_fmt = __pyx_t_8;
 
-  /* "ext_modules/io_funcs.pyx":206
+  /* "ext_modules/io_funcs.pyx":210
  *     cdef Py_ssize_t i, j, k, fr
  * 
  *     fprintf(fo, "GENE");             # <<<<<<<<<<<<<<
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  */
   (void)(fprintf(__pyx_v_fo, ((char const *)"GENE")));
 
-  /* "ext_modules/io_funcs.pyx":207
+  /* "ext_modules/io_funcs.pyx":211
  * 
  *     fprintf(fo, "GENE");
  *     for i in range(N):             # <<<<<<<<<<<<<<
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  *     fprintf(fo, "\n")
  */
   __pyx_t_9 = __pyx_v_N;
   __pyx_t_10 = __pyx_t_9;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_10; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "ext_modules/io_funcs.pyx":208
+    /* "ext_modules/io_funcs.pyx":212
  *     fprintf(fo, "GENE");
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])             # <<<<<<<<<<<<<<
  *     fprintf(fo, "\n")
  * 
  */
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_1 = (PyObject *) *((PyObject * *) ( /* dim=0 */ (__pyx_v_barcodes.data + __pyx_t_11 * __pyx_v_barcodes.strides[0]) ));
     if (unlikely(__pyx_t_1 == NULL)) __pyx_t_1 = Py_None;
     __Pyx_INCREF((PyObject*)__pyx_t_1);
-    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 208, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 212, __pyx_L1_error)
     (void)(fprintf(__pyx_v_fo, ((char const *)"\t%s"), ((char *)__pyx_t_12)));
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
 
-  /* "ext_modules/io_funcs.pyx":209
+  /* "ext_modules/io_funcs.pyx":213
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  *     fprintf(fo, "\n")             # <<<<<<<<<<<<<<
  * 
  *     for i in range(M):
  */
   (void)(fprintf(__pyx_v_fo, ((char const *)"\n")));
 
-  /* "ext_modules/io_funcs.pyx":211
+  /* "ext_modules/io_funcs.pyx":215
  *     fprintf(fo, "\n")
  * 
  *     for i in range(M):             # <<<<<<<<<<<<<<
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0
  */
   __pyx_t_9 = __pyx_v_M;
   __pyx_t_10 = __pyx_t_9;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_10; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "ext_modules/io_funcs.pyx":212
+    /* "ext_modules/io_funcs.pyx":216
  * 
  *     for i in range(M):
  *         fprintf(fo, "%s", <char*>features[i]);             # <<<<<<<<<<<<<<
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):
  */
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_1 = (PyObject *) *((PyObject * *) ( /* dim=0 */ (__pyx_v_features.data + __pyx_t_11 * __pyx_v_features.strides[0]) ));
     if (unlikely(__pyx_t_1 == NULL)) __pyx_t_1 = Py_None;
     __Pyx_INCREF((PyObject*)__pyx_t_1);
-    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 212, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 216, __pyx_L1_error)
     (void)(fprintf(__pyx_v_fo, ((char const *)"%s"), ((char *)__pyx_t_12)));
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "ext_modules/io_funcs.pyx":213
+    /* "ext_modules/io_funcs.pyx":217
  *     for i in range(M):
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0             # <<<<<<<<<<<<<<
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):
  */
     __pyx_v_fr = 0;
 
-    /* "ext_modules/io_funcs.pyx":214
+    /* "ext_modules/io_funcs.pyx":218
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):             # <<<<<<<<<<<<<<
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")
  */
     __pyx_t_11 = (__pyx_v_i + 1);
     __pyx_t_13 = (*((long *) ( /* dim=0 */ (__pyx_v_indptr.data + __pyx_t_11 * __pyx_v_indptr.strides[0]) )));
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = (*((long *) ( /* dim=0 */ (__pyx_v_indptr.data + __pyx_t_11 * __pyx_v_indptr.strides[0]) ))); __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_j = __pyx_t_15;
 
-      /* "ext_modules/io_funcs.pyx":215
+      /* "ext_modules/io_funcs.pyx":219
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):             # <<<<<<<<<<<<<<
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])
  */
       __pyx_t_16 = __pyx_v_j;
       __pyx_t_17 = (*((long *) ( /* dim=0 */ (__pyx_v_indices.data + __pyx_t_16 * __pyx_v_indices.strides[0]) )));
       __pyx_t_18 = __pyx_t_17;
       for (__pyx_t_19 = __pyx_v_fr; __pyx_t_19 < __pyx_t_18; __pyx_t_19+=1) {
         __pyx_v_k = __pyx_t_19;
 
-        /* "ext_modules/io_funcs.pyx":216
+        /* "ext_modules/io_funcs.pyx":220
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")             # <<<<<<<<<<<<<<
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1
  */
         (void)(fprintf(__pyx_v_fo, ((char const *)"\t0")));
       }
 
-      /* "ext_modules/io_funcs.pyx":217
+      /* "ext_modules/io_funcs.pyx":221
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])             # <<<<<<<<<<<<<<
  *             fr = indices[j] + 1
  *         for k in range(fr, N):
  */
       __pyx_t_16 = __pyx_v_j;
       (void)(fprintf(__pyx_v_fo, __pyx_v_fmt, (*((float *) ( /* dim=0 */ (__pyx_v_data.data + __pyx_t_16 * __pyx_v_data.strides[0]) )))));
 
-      /* "ext_modules/io_funcs.pyx":218
+      /* "ext_modules/io_funcs.pyx":222
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1             # <<<<<<<<<<<<<<
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")
  */
       __pyx_t_16 = __pyx_v_j;
       __pyx_v_fr = ((*((long *) ( /* dim=0 */ (__pyx_v_indices.data + __pyx_t_16 * __pyx_v_indices.strides[0]) ))) + 1);
     }
 
-    /* "ext_modules/io_funcs.pyx":219
+    /* "ext_modules/io_funcs.pyx":223
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1
  *         for k in range(fr, N):             # <<<<<<<<<<<<<<
  *             fprintf(fo, "\t0")
  *         fprintf(fo, "\n")
  */
     __pyx_t_20 = __pyx_v_N;
     __pyx_t_21 = __pyx_t_20;
     for (__pyx_t_15 = __pyx_v_fr; __pyx_t_15 < __pyx_t_21; __pyx_t_15+=1) {
       __pyx_v_k = __pyx_t_15;
 
-      /* "ext_modules/io_funcs.pyx":220
+      /* "ext_modules/io_funcs.pyx":224
  *             fr = indices[j] + 1
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")             # <<<<<<<<<<<<<<
  *         fprintf(fo, "\n")
  * 
  */
       (void)(fprintf(__pyx_v_fo, ((char const *)"\t0")));
     }
 
-    /* "ext_modules/io_funcs.pyx":221
+    /* "ext_modules/io_funcs.pyx":225
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")
  *         fprintf(fo, "\n")             # <<<<<<<<<<<<<<
  * 
  *     fclose(fo)
  */
     (void)(fprintf(__pyx_v_fo, ((char const *)"\n")));
   }
 
-  /* "ext_modules/io_funcs.pyx":223
+  /* "ext_modules/io_funcs.pyx":227
  *         fprintf(fo, "\n")
  * 
  *     fclose(fo)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   (void)(fclose(__pyx_v_fo));
 
-  /* "ext_modules/io_funcs.pyx":197
+  /* "ext_modules/io_funcs.pyx":201
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef void write_dense(char* output_file, str[:] barcodes, str[:] features, data_type[:] data, indices_type[:] indices, indptr_type[:] indptr, int M, int N, int precision = 2):             # <<<<<<<<<<<<<<
  *     """ Input must be csr_matrix internal representation, gene by cell (X.T.tocsr()); Output will be gene by cell
  *     """
  */
 
@@ -18485,61 +18600,61 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_output_file)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_barcodes)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_1_1write_dense", 0, 8, 9, 1); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_1_1write_dense", 0, 8, 9, 1); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_features)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_1_1write_dense", 0, 8, 9, 2); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_1_1write_dense", 0, 8, 9, 2); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_1_1write_dense", 0, 8, 9, 3); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_1_1write_dense", 0, 8, 9, 3); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_indices)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_1_1write_dense", 0, 8, 9, 4); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_1_1write_dense", 0, 8, 9, 4); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_indptr)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_1_1write_dense", 0, 8, 9, 5); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_1_1write_dense", 0, 8, 9, 5); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (likely((values[6] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_M)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_1_1write_dense", 0, 8, 9, 6); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_1_1write_dense", 0, 8, 9, 6); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  7:
         if (likely((values[7] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_N)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_1_1write_dense", 0, 8, 9, 7); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_1_1write_dense", 0, 8, 9, 7); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  8:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_precision);
           if (value) { values[8] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_2_1_1write_dense") < 0)) __PYX_ERR(0, 197, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_2_1_1write_dense") < 0)) __PYX_ERR(0, 201, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  9: values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
         CYTHON_FALLTHROUGH;
         case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
         values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
@@ -18549,31 +18664,31 @@
         values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_output_file = __Pyx_PyObject_AsWritableString(values[0]); if (unlikely((!__pyx_v_output_file) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_barcodes = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_barcodes.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_features = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_features.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_data = __Pyx_PyObject_to_MemoryviewSlice_ds_float(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_data.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_indices = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indices.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_indptr = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indptr.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_M = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_M == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_N = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_N == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
+    __pyx_v_output_file = __Pyx_PyObject_AsWritableString(values[0]); if (unlikely((!__pyx_v_output_file) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_barcodes = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_barcodes.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_features = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_features.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_data = __Pyx_PyObject_to_MemoryviewSlice_ds_float(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_data.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_indices = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indices.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_indptr = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indptr.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_M = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_M == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_N = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_N == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
     if (values[8]) {
-      __pyx_v_precision = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_precision == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
+      __pyx_v_precision = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_precision == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
     } else {
-      __pyx_v_precision = __pyx_k__36;
+      __pyx_v_precision = __pyx_k__37;
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_1_1write_dense", 0, 8, 9, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 197, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_2_1_1write_dense", 0, 8, 9, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 201, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pegasusio.cylib.io.__pyx_fuse_2_1_1write_dense", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9pegasusio_5cylib_2io_66__pyx_fuse_2_1_1write_dense(__pyx_self, __pyx_v_output_file, __pyx_v_barcodes, __pyx_v_features, __pyx_v_data, __pyx_v_indices, __pyx_v_indptr, __pyx_v_M, __pyx_v_N, __pyx_v_precision);
 
@@ -18588,23 +18703,23 @@
   struct __pyx_fuse_2_1_1__pyx_opt_args_9pegasusio_5cylib_2io_write_dense __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_2_1_1write_dense", 0);
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_barcodes.memview)) { __Pyx_RaiseUnboundLocalError("barcodes"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_features.memview)) { __Pyx_RaiseUnboundLocalError("features"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_data.memview)) { __Pyx_RaiseUnboundLocalError("data"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_indices.memview)) { __Pyx_RaiseUnboundLocalError("indices"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_indptr.memview)) { __Pyx_RaiseUnboundLocalError("indptr"); __PYX_ERR(0, 197, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_barcodes.memview)) { __Pyx_RaiseUnboundLocalError("barcodes"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_features.memview)) { __Pyx_RaiseUnboundLocalError("features"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_data.memview)) { __Pyx_RaiseUnboundLocalError("data"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_indices.memview)) { __Pyx_RaiseUnboundLocalError("indices"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_indptr.memview)) { __Pyx_RaiseUnboundLocalError("indptr"); __PYX_ERR(0, 201, __pyx_L1_error) }
   __pyx_t_1.__pyx_n = 1;
   __pyx_t_1.precision = __pyx_v_precision;
   __pyx_fuse_2_1_1__pyx_f_9pegasusio_5cylib_2io_write_dense(__pyx_v_output_file, __pyx_v_barcodes, __pyx_v_features, __pyx_v_data, __pyx_v_indices, __pyx_v_indptr, __pyx_v_M, __pyx_v_N, 0, &__pyx_t_1); 
-  __pyx_t_2 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -18621,15 +18736,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pw_9pegasusio_5cylib_2io_69__pyx_fuse_3_0_0write_dense(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_pw_9pegasusio_5cylib_2io_7write_dense(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static void __pyx_fuse_3_0_0__pyx_f_9pegasusio_5cylib_2io_write_dense(char *__pyx_v_output_file, __Pyx_memviewslice __pyx_v_barcodes, __Pyx_memviewslice __pyx_v_features, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_indices, __Pyx_memviewslice __pyx_v_indptr, int __pyx_v_M, int __pyx_v_N, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_fuse_3_0_0__pyx_opt_args_9pegasusio_5cylib_2io_write_dense *__pyx_optional_args) {
-  int __pyx_v_precision = __pyx_k__37;
+  int __pyx_v_precision = __pyx_k__38;
   FILE *__pyx_v_fo;
   PyObject *__pyx_v_fmt_str = 0;
   char const *__pyx_v_fmt;
   Py_ssize_t __pyx_v_i;
   Py_ssize_t __pyx_v_j;
   CYTHON_UNUSED Py_ssize_t __pyx_v_k;
   Py_ssize_t __pyx_v_fr;
@@ -18659,24 +18774,24 @@
   __Pyx_RefNannySetupContext("__pyx_fuse_3_0_0write_dense", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_precision = __pyx_optional_args->precision;
     }
   }
 
-  /* "ext_modules/io_funcs.pyx":200
+  /* "ext_modules/io_funcs.pyx":204
  *     """ Input must be csr_matrix internal representation, gene by cell (X.T.tocsr()); Output will be gene by cell
  *     """
  *     cdef FILE* fo = fopen(output_file, "w")             # <<<<<<<<<<<<<<
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"
  * 
  */
   __pyx_v_fo = fopen(__pyx_v_output_file, ((char const *)"w"));
 
-  /* "ext_modules/io_funcs.pyx":201
+  /* "ext_modules/io_funcs.pyx":205
  *     """
  *     cdef FILE* fo = fopen(output_file, "w")
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"             # <<<<<<<<<<<<<<
  * 
  *     cdef const char* fmt = fmt_str
  */
   __pyx_t_3 = (0 != 0);
@@ -18685,236 +18800,236 @@
     __pyx_t_2 = __pyx_t_3;
     goto __pyx_L3_bool_binop_done;
   }
   __pyx_t_3 = (1 != 0);
   __pyx_t_2 = __pyx_t_3;
   __pyx_L3_bool_binop_done:;
   if (__pyx_t_2) {
-    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = 0;
     __pyx_t_6 = 127;
-    __Pyx_INCREF(__pyx_kp_u__25);
+    __Pyx_INCREF(__pyx_kp_u__26);
     __pyx_t_5 += 3;
-    __Pyx_GIVEREF(__pyx_kp_u__25);
-    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u__25);
-    __pyx_t_7 = __Pyx_PyUnicode_From_int(__pyx_v_precision, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __Pyx_GIVEREF(__pyx_kp_u__26);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u__26);
+    __pyx_t_7 = __Pyx_PyUnicode_From_int(__pyx_v_precision, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_INCREF(__pyx_n_u_f_2);
     __pyx_t_5 += 1;
     __Pyx_GIVEREF(__pyx_n_u_f_2);
     PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_n_u_f_2);
-    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_1 = __pyx_t_7;
     __pyx_t_7 = 0;
   } else {
     __Pyx_INCREF(__pyx_kp_u_d);
     __pyx_t_1 = __pyx_kp_u_d;
   }
   __pyx_v_fmt_str = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "ext_modules/io_funcs.pyx":203
+  /* "ext_modules/io_funcs.pyx":207
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"
  * 
  *     cdef const char* fmt = fmt_str             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t i, j, k, fr
  * 
  */
-  __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_v_fmt_str); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 203, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_v_fmt_str); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 207, __pyx_L1_error)
   __pyx_v_fmt = __pyx_t_8;
 
-  /* "ext_modules/io_funcs.pyx":206
+  /* "ext_modules/io_funcs.pyx":210
  *     cdef Py_ssize_t i, j, k, fr
  * 
  *     fprintf(fo, "GENE");             # <<<<<<<<<<<<<<
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  */
   (void)(fprintf(__pyx_v_fo, ((char const *)"GENE")));
 
-  /* "ext_modules/io_funcs.pyx":207
+  /* "ext_modules/io_funcs.pyx":211
  * 
  *     fprintf(fo, "GENE");
  *     for i in range(N):             # <<<<<<<<<<<<<<
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  *     fprintf(fo, "\n")
  */
   __pyx_t_9 = __pyx_v_N;
   __pyx_t_10 = __pyx_t_9;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_10; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "ext_modules/io_funcs.pyx":208
+    /* "ext_modules/io_funcs.pyx":212
  *     fprintf(fo, "GENE");
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])             # <<<<<<<<<<<<<<
  *     fprintf(fo, "\n")
  * 
  */
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_1 = (PyObject *) *((PyObject * *) ( /* dim=0 */ (__pyx_v_barcodes.data + __pyx_t_11 * __pyx_v_barcodes.strides[0]) ));
     if (unlikely(__pyx_t_1 == NULL)) __pyx_t_1 = Py_None;
     __Pyx_INCREF((PyObject*)__pyx_t_1);
-    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 208, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 212, __pyx_L1_error)
     (void)(fprintf(__pyx_v_fo, ((char const *)"\t%s"), ((char *)__pyx_t_12)));
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
 
-  /* "ext_modules/io_funcs.pyx":209
+  /* "ext_modules/io_funcs.pyx":213
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  *     fprintf(fo, "\n")             # <<<<<<<<<<<<<<
  * 
  *     for i in range(M):
  */
   (void)(fprintf(__pyx_v_fo, ((char const *)"\n")));
 
-  /* "ext_modules/io_funcs.pyx":211
+  /* "ext_modules/io_funcs.pyx":215
  *     fprintf(fo, "\n")
  * 
  *     for i in range(M):             # <<<<<<<<<<<<<<
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0
  */
   __pyx_t_9 = __pyx_v_M;
   __pyx_t_10 = __pyx_t_9;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_10; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "ext_modules/io_funcs.pyx":212
+    /* "ext_modules/io_funcs.pyx":216
  * 
  *     for i in range(M):
  *         fprintf(fo, "%s", <char*>features[i]);             # <<<<<<<<<<<<<<
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):
  */
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_1 = (PyObject *) *((PyObject * *) ( /* dim=0 */ (__pyx_v_features.data + __pyx_t_11 * __pyx_v_features.strides[0]) ));
     if (unlikely(__pyx_t_1 == NULL)) __pyx_t_1 = Py_None;
     __Pyx_INCREF((PyObject*)__pyx_t_1);
-    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 212, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 216, __pyx_L1_error)
     (void)(fprintf(__pyx_v_fo, ((char const *)"%s"), ((char *)__pyx_t_12)));
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "ext_modules/io_funcs.pyx":213
+    /* "ext_modules/io_funcs.pyx":217
  *     for i in range(M):
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0             # <<<<<<<<<<<<<<
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):
  */
     __pyx_v_fr = 0;
 
-    /* "ext_modules/io_funcs.pyx":214
+    /* "ext_modules/io_funcs.pyx":218
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):             # <<<<<<<<<<<<<<
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")
  */
     __pyx_t_11 = (__pyx_v_i + 1);
     __pyx_t_13 = (*((int *) ( /* dim=0 */ (__pyx_v_indptr.data + __pyx_t_11 * __pyx_v_indptr.strides[0]) )));
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = (*((int *) ( /* dim=0 */ (__pyx_v_indptr.data + __pyx_t_11 * __pyx_v_indptr.strides[0]) ))); __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_j = __pyx_t_15;
 
-      /* "ext_modules/io_funcs.pyx":215
+      /* "ext_modules/io_funcs.pyx":219
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):             # <<<<<<<<<<<<<<
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])
  */
       __pyx_t_16 = __pyx_v_j;
       __pyx_t_17 = (*((int *) ( /* dim=0 */ (__pyx_v_indices.data + __pyx_t_16 * __pyx_v_indices.strides[0]) )));
       __pyx_t_18 = __pyx_t_17;
       for (__pyx_t_19 = __pyx_v_fr; __pyx_t_19 < __pyx_t_18; __pyx_t_19+=1) {
         __pyx_v_k = __pyx_t_19;
 
-        /* "ext_modules/io_funcs.pyx":216
+        /* "ext_modules/io_funcs.pyx":220
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")             # <<<<<<<<<<<<<<
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1
  */
         (void)(fprintf(__pyx_v_fo, ((char const *)"\t0")));
       }
 
-      /* "ext_modules/io_funcs.pyx":217
+      /* "ext_modules/io_funcs.pyx":221
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])             # <<<<<<<<<<<<<<
  *             fr = indices[j] + 1
  *         for k in range(fr, N):
  */
       __pyx_t_16 = __pyx_v_j;
       (void)(fprintf(__pyx_v_fo, __pyx_v_fmt, (*((double *) ( /* dim=0 */ (__pyx_v_data.data + __pyx_t_16 * __pyx_v_data.strides[0]) )))));
 
-      /* "ext_modules/io_funcs.pyx":218
+      /* "ext_modules/io_funcs.pyx":222
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1             # <<<<<<<<<<<<<<
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")
  */
       __pyx_t_16 = __pyx_v_j;
       __pyx_v_fr = ((*((int *) ( /* dim=0 */ (__pyx_v_indices.data + __pyx_t_16 * __pyx_v_indices.strides[0]) ))) + 1);
     }
 
-    /* "ext_modules/io_funcs.pyx":219
+    /* "ext_modules/io_funcs.pyx":223
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1
  *         for k in range(fr, N):             # <<<<<<<<<<<<<<
  *             fprintf(fo, "\t0")
  *         fprintf(fo, "\n")
  */
     __pyx_t_13 = __pyx_v_N;
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = __pyx_v_fr; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_k = __pyx_t_15;
 
-      /* "ext_modules/io_funcs.pyx":220
+      /* "ext_modules/io_funcs.pyx":224
  *             fr = indices[j] + 1
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")             # <<<<<<<<<<<<<<
  *         fprintf(fo, "\n")
  * 
  */
       (void)(fprintf(__pyx_v_fo, ((char const *)"\t0")));
     }
 
-    /* "ext_modules/io_funcs.pyx":221
+    /* "ext_modules/io_funcs.pyx":225
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")
  *         fprintf(fo, "\n")             # <<<<<<<<<<<<<<
  * 
  *     fclose(fo)
  */
     (void)(fprintf(__pyx_v_fo, ((char const *)"\n")));
   }
 
-  /* "ext_modules/io_funcs.pyx":223
+  /* "ext_modules/io_funcs.pyx":227
  *         fprintf(fo, "\n")
  * 
  *     fclose(fo)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   (void)(fclose(__pyx_v_fo));
 
-  /* "ext_modules/io_funcs.pyx":197
+  /* "ext_modules/io_funcs.pyx":201
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef void write_dense(char* output_file, str[:] barcodes, str[:] features, data_type[:] data, indices_type[:] indices, indptr_type[:] indptr, int M, int N, int precision = 2):             # <<<<<<<<<<<<<<
  *     """ Input must be csr_matrix internal representation, gene by cell (X.T.tocsr()); Output will be gene by cell
  *     """
  */
 
@@ -18982,61 +19097,61 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_output_file)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_barcodes)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_0_0write_dense", 0, 8, 9, 1); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_0_0write_dense", 0, 8, 9, 1); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_features)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_0_0write_dense", 0, 8, 9, 2); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_0_0write_dense", 0, 8, 9, 2); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_0_0write_dense", 0, 8, 9, 3); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_0_0write_dense", 0, 8, 9, 3); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_indices)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_0_0write_dense", 0, 8, 9, 4); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_0_0write_dense", 0, 8, 9, 4); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_indptr)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_0_0write_dense", 0, 8, 9, 5); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_0_0write_dense", 0, 8, 9, 5); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (likely((values[6] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_M)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_0_0write_dense", 0, 8, 9, 6); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_0_0write_dense", 0, 8, 9, 6); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  7:
         if (likely((values[7] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_N)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_0_0write_dense", 0, 8, 9, 7); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_0_0write_dense", 0, 8, 9, 7); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  8:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_precision);
           if (value) { values[8] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_3_0_0write_dense") < 0)) __PYX_ERR(0, 197, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_3_0_0write_dense") < 0)) __PYX_ERR(0, 201, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  9: values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
         CYTHON_FALLTHROUGH;
         case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
         values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
@@ -19046,31 +19161,31 @@
         values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_output_file = __Pyx_PyObject_AsWritableString(values[0]); if (unlikely((!__pyx_v_output_file) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_barcodes = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_barcodes.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_features = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_features.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_data = __Pyx_PyObject_to_MemoryviewSlice_ds_double(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_data.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_indices = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indices.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_indptr = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indptr.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_M = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_M == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_N = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_N == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
+    __pyx_v_output_file = __Pyx_PyObject_AsWritableString(values[0]); if (unlikely((!__pyx_v_output_file) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_barcodes = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_barcodes.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_features = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_features.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_data = __Pyx_PyObject_to_MemoryviewSlice_ds_double(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_data.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_indices = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indices.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_indptr = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indptr.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_M = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_M == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_N = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_N == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
     if (values[8]) {
-      __pyx_v_precision = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_precision == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
+      __pyx_v_precision = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_precision == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
     } else {
-      __pyx_v_precision = __pyx_k__37;
+      __pyx_v_precision = __pyx_k__38;
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_0_0write_dense", 0, 8, 9, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 197, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_0_0write_dense", 0, 8, 9, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 201, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pegasusio.cylib.io.__pyx_fuse_3_0_0write_dense", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9pegasusio_5cylib_2io_68__pyx_fuse_3_0_0write_dense(__pyx_self, __pyx_v_output_file, __pyx_v_barcodes, __pyx_v_features, __pyx_v_data, __pyx_v_indices, __pyx_v_indptr, __pyx_v_M, __pyx_v_N, __pyx_v_precision);
 
@@ -19085,23 +19200,23 @@
   struct __pyx_fuse_3_0_0__pyx_opt_args_9pegasusio_5cylib_2io_write_dense __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_3_0_0write_dense", 0);
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_barcodes.memview)) { __Pyx_RaiseUnboundLocalError("barcodes"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_features.memview)) { __Pyx_RaiseUnboundLocalError("features"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_data.memview)) { __Pyx_RaiseUnboundLocalError("data"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_indices.memview)) { __Pyx_RaiseUnboundLocalError("indices"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_indptr.memview)) { __Pyx_RaiseUnboundLocalError("indptr"); __PYX_ERR(0, 197, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_barcodes.memview)) { __Pyx_RaiseUnboundLocalError("barcodes"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_features.memview)) { __Pyx_RaiseUnboundLocalError("features"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_data.memview)) { __Pyx_RaiseUnboundLocalError("data"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_indices.memview)) { __Pyx_RaiseUnboundLocalError("indices"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_indptr.memview)) { __Pyx_RaiseUnboundLocalError("indptr"); __PYX_ERR(0, 201, __pyx_L1_error) }
   __pyx_t_1.__pyx_n = 1;
   __pyx_t_1.precision = __pyx_v_precision;
   __pyx_fuse_3_0_0__pyx_f_9pegasusio_5cylib_2io_write_dense(__pyx_v_output_file, __pyx_v_barcodes, __pyx_v_features, __pyx_v_data, __pyx_v_indices, __pyx_v_indptr, __pyx_v_M, __pyx_v_N, 0, &__pyx_t_1); 
-  __pyx_t_2 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -19118,15 +19233,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pw_9pegasusio_5cylib_2io_71__pyx_fuse_3_0_1write_dense(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_pw_9pegasusio_5cylib_2io_7write_dense(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static void __pyx_fuse_3_0_1__pyx_f_9pegasusio_5cylib_2io_write_dense(char *__pyx_v_output_file, __Pyx_memviewslice __pyx_v_barcodes, __Pyx_memviewslice __pyx_v_features, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_indices, __Pyx_memviewslice __pyx_v_indptr, int __pyx_v_M, int __pyx_v_N, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_fuse_3_0_1__pyx_opt_args_9pegasusio_5cylib_2io_write_dense *__pyx_optional_args) {
-  int __pyx_v_precision = __pyx_k__38;
+  int __pyx_v_precision = __pyx_k__39;
   FILE *__pyx_v_fo;
   PyObject *__pyx_v_fmt_str = 0;
   char const *__pyx_v_fmt;
   Py_ssize_t __pyx_v_i;
   Py_ssize_t __pyx_v_j;
   CYTHON_UNUSED Py_ssize_t __pyx_v_k;
   Py_ssize_t __pyx_v_fr;
@@ -19156,24 +19271,24 @@
   __Pyx_RefNannySetupContext("__pyx_fuse_3_0_1write_dense", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_precision = __pyx_optional_args->precision;
     }
   }
 
-  /* "ext_modules/io_funcs.pyx":200
+  /* "ext_modules/io_funcs.pyx":204
  *     """ Input must be csr_matrix internal representation, gene by cell (X.T.tocsr()); Output will be gene by cell
  *     """
  *     cdef FILE* fo = fopen(output_file, "w")             # <<<<<<<<<<<<<<
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"
  * 
  */
   __pyx_v_fo = fopen(__pyx_v_output_file, ((char const *)"w"));
 
-  /* "ext_modules/io_funcs.pyx":201
+  /* "ext_modules/io_funcs.pyx":205
  *     """
  *     cdef FILE* fo = fopen(output_file, "w")
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"             # <<<<<<<<<<<<<<
  * 
  *     cdef const char* fmt = fmt_str
  */
   __pyx_t_3 = (0 != 0);
@@ -19182,236 +19297,236 @@
     __pyx_t_2 = __pyx_t_3;
     goto __pyx_L3_bool_binop_done;
   }
   __pyx_t_3 = (1 != 0);
   __pyx_t_2 = __pyx_t_3;
   __pyx_L3_bool_binop_done:;
   if (__pyx_t_2) {
-    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = 0;
     __pyx_t_6 = 127;
-    __Pyx_INCREF(__pyx_kp_u__25);
+    __Pyx_INCREF(__pyx_kp_u__26);
     __pyx_t_5 += 3;
-    __Pyx_GIVEREF(__pyx_kp_u__25);
-    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u__25);
-    __pyx_t_7 = __Pyx_PyUnicode_From_int(__pyx_v_precision, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __Pyx_GIVEREF(__pyx_kp_u__26);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u__26);
+    __pyx_t_7 = __Pyx_PyUnicode_From_int(__pyx_v_precision, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_INCREF(__pyx_n_u_f_2);
     __pyx_t_5 += 1;
     __Pyx_GIVEREF(__pyx_n_u_f_2);
     PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_n_u_f_2);
-    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_1 = __pyx_t_7;
     __pyx_t_7 = 0;
   } else {
     __Pyx_INCREF(__pyx_kp_u_d);
     __pyx_t_1 = __pyx_kp_u_d;
   }
   __pyx_v_fmt_str = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "ext_modules/io_funcs.pyx":203
+  /* "ext_modules/io_funcs.pyx":207
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"
  * 
  *     cdef const char* fmt = fmt_str             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t i, j, k, fr
  * 
  */
-  __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_v_fmt_str); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 203, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_v_fmt_str); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 207, __pyx_L1_error)
   __pyx_v_fmt = __pyx_t_8;
 
-  /* "ext_modules/io_funcs.pyx":206
+  /* "ext_modules/io_funcs.pyx":210
  *     cdef Py_ssize_t i, j, k, fr
  * 
  *     fprintf(fo, "GENE");             # <<<<<<<<<<<<<<
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  */
   (void)(fprintf(__pyx_v_fo, ((char const *)"GENE")));
 
-  /* "ext_modules/io_funcs.pyx":207
+  /* "ext_modules/io_funcs.pyx":211
  * 
  *     fprintf(fo, "GENE");
  *     for i in range(N):             # <<<<<<<<<<<<<<
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  *     fprintf(fo, "\n")
  */
   __pyx_t_9 = __pyx_v_N;
   __pyx_t_10 = __pyx_t_9;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_10; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "ext_modules/io_funcs.pyx":208
+    /* "ext_modules/io_funcs.pyx":212
  *     fprintf(fo, "GENE");
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])             # <<<<<<<<<<<<<<
  *     fprintf(fo, "\n")
  * 
  */
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_1 = (PyObject *) *((PyObject * *) ( /* dim=0 */ (__pyx_v_barcodes.data + __pyx_t_11 * __pyx_v_barcodes.strides[0]) ));
     if (unlikely(__pyx_t_1 == NULL)) __pyx_t_1 = Py_None;
     __Pyx_INCREF((PyObject*)__pyx_t_1);
-    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 208, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 212, __pyx_L1_error)
     (void)(fprintf(__pyx_v_fo, ((char const *)"\t%s"), ((char *)__pyx_t_12)));
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
 
-  /* "ext_modules/io_funcs.pyx":209
+  /* "ext_modules/io_funcs.pyx":213
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  *     fprintf(fo, "\n")             # <<<<<<<<<<<<<<
  * 
  *     for i in range(M):
  */
   (void)(fprintf(__pyx_v_fo, ((char const *)"\n")));
 
-  /* "ext_modules/io_funcs.pyx":211
+  /* "ext_modules/io_funcs.pyx":215
  *     fprintf(fo, "\n")
  * 
  *     for i in range(M):             # <<<<<<<<<<<<<<
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0
  */
   __pyx_t_9 = __pyx_v_M;
   __pyx_t_10 = __pyx_t_9;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_10; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "ext_modules/io_funcs.pyx":212
+    /* "ext_modules/io_funcs.pyx":216
  * 
  *     for i in range(M):
  *         fprintf(fo, "%s", <char*>features[i]);             # <<<<<<<<<<<<<<
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):
  */
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_1 = (PyObject *) *((PyObject * *) ( /* dim=0 */ (__pyx_v_features.data + __pyx_t_11 * __pyx_v_features.strides[0]) ));
     if (unlikely(__pyx_t_1 == NULL)) __pyx_t_1 = Py_None;
     __Pyx_INCREF((PyObject*)__pyx_t_1);
-    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 212, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 216, __pyx_L1_error)
     (void)(fprintf(__pyx_v_fo, ((char const *)"%s"), ((char *)__pyx_t_12)));
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "ext_modules/io_funcs.pyx":213
+    /* "ext_modules/io_funcs.pyx":217
  *     for i in range(M):
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0             # <<<<<<<<<<<<<<
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):
  */
     __pyx_v_fr = 0;
 
-    /* "ext_modules/io_funcs.pyx":214
+    /* "ext_modules/io_funcs.pyx":218
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):             # <<<<<<<<<<<<<<
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")
  */
     __pyx_t_11 = (__pyx_v_i + 1);
     __pyx_t_13 = (*((long *) ( /* dim=0 */ (__pyx_v_indptr.data + __pyx_t_11 * __pyx_v_indptr.strides[0]) )));
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = (*((long *) ( /* dim=0 */ (__pyx_v_indptr.data + __pyx_t_11 * __pyx_v_indptr.strides[0]) ))); __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_j = __pyx_t_15;
 
-      /* "ext_modules/io_funcs.pyx":215
+      /* "ext_modules/io_funcs.pyx":219
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):             # <<<<<<<<<<<<<<
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])
  */
       __pyx_t_16 = __pyx_v_j;
       __pyx_t_17 = (*((int *) ( /* dim=0 */ (__pyx_v_indices.data + __pyx_t_16 * __pyx_v_indices.strides[0]) )));
       __pyx_t_18 = __pyx_t_17;
       for (__pyx_t_19 = __pyx_v_fr; __pyx_t_19 < __pyx_t_18; __pyx_t_19+=1) {
         __pyx_v_k = __pyx_t_19;
 
-        /* "ext_modules/io_funcs.pyx":216
+        /* "ext_modules/io_funcs.pyx":220
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")             # <<<<<<<<<<<<<<
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1
  */
         (void)(fprintf(__pyx_v_fo, ((char const *)"\t0")));
       }
 
-      /* "ext_modules/io_funcs.pyx":217
+      /* "ext_modules/io_funcs.pyx":221
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])             # <<<<<<<<<<<<<<
  *             fr = indices[j] + 1
  *         for k in range(fr, N):
  */
       __pyx_t_16 = __pyx_v_j;
       (void)(fprintf(__pyx_v_fo, __pyx_v_fmt, (*((double *) ( /* dim=0 */ (__pyx_v_data.data + __pyx_t_16 * __pyx_v_data.strides[0]) )))));
 
-      /* "ext_modules/io_funcs.pyx":218
+      /* "ext_modules/io_funcs.pyx":222
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1             # <<<<<<<<<<<<<<
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")
  */
       __pyx_t_16 = __pyx_v_j;
       __pyx_v_fr = ((*((int *) ( /* dim=0 */ (__pyx_v_indices.data + __pyx_t_16 * __pyx_v_indices.strides[0]) ))) + 1);
     }
 
-    /* "ext_modules/io_funcs.pyx":219
+    /* "ext_modules/io_funcs.pyx":223
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1
  *         for k in range(fr, N):             # <<<<<<<<<<<<<<
  *             fprintf(fo, "\t0")
  *         fprintf(fo, "\n")
  */
     __pyx_t_17 = __pyx_v_N;
     __pyx_t_18 = __pyx_t_17;
     for (__pyx_t_15 = __pyx_v_fr; __pyx_t_15 < __pyx_t_18; __pyx_t_15+=1) {
       __pyx_v_k = __pyx_t_15;
 
-      /* "ext_modules/io_funcs.pyx":220
+      /* "ext_modules/io_funcs.pyx":224
  *             fr = indices[j] + 1
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")             # <<<<<<<<<<<<<<
  *         fprintf(fo, "\n")
  * 
  */
       (void)(fprintf(__pyx_v_fo, ((char const *)"\t0")));
     }
 
-    /* "ext_modules/io_funcs.pyx":221
+    /* "ext_modules/io_funcs.pyx":225
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")
  *         fprintf(fo, "\n")             # <<<<<<<<<<<<<<
  * 
  *     fclose(fo)
  */
     (void)(fprintf(__pyx_v_fo, ((char const *)"\n")));
   }
 
-  /* "ext_modules/io_funcs.pyx":223
+  /* "ext_modules/io_funcs.pyx":227
  *         fprintf(fo, "\n")
  * 
  *     fclose(fo)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   (void)(fclose(__pyx_v_fo));
 
-  /* "ext_modules/io_funcs.pyx":197
+  /* "ext_modules/io_funcs.pyx":201
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef void write_dense(char* output_file, str[:] barcodes, str[:] features, data_type[:] data, indices_type[:] indices, indptr_type[:] indptr, int M, int N, int precision = 2):             # <<<<<<<<<<<<<<
  *     """ Input must be csr_matrix internal representation, gene by cell (X.T.tocsr()); Output will be gene by cell
  *     """
  */
 
@@ -19479,61 +19594,61 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_output_file)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_barcodes)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_0_1write_dense", 0, 8, 9, 1); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_0_1write_dense", 0, 8, 9, 1); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_features)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_0_1write_dense", 0, 8, 9, 2); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_0_1write_dense", 0, 8, 9, 2); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_0_1write_dense", 0, 8, 9, 3); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_0_1write_dense", 0, 8, 9, 3); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_indices)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_0_1write_dense", 0, 8, 9, 4); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_0_1write_dense", 0, 8, 9, 4); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_indptr)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_0_1write_dense", 0, 8, 9, 5); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_0_1write_dense", 0, 8, 9, 5); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (likely((values[6] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_M)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_0_1write_dense", 0, 8, 9, 6); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_0_1write_dense", 0, 8, 9, 6); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  7:
         if (likely((values[7] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_N)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_0_1write_dense", 0, 8, 9, 7); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_0_1write_dense", 0, 8, 9, 7); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  8:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_precision);
           if (value) { values[8] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_3_0_1write_dense") < 0)) __PYX_ERR(0, 197, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_3_0_1write_dense") < 0)) __PYX_ERR(0, 201, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  9: values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
         CYTHON_FALLTHROUGH;
         case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
         values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
@@ -19543,31 +19658,31 @@
         values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_output_file = __Pyx_PyObject_AsWritableString(values[0]); if (unlikely((!__pyx_v_output_file) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_barcodes = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_barcodes.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_features = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_features.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_data = __Pyx_PyObject_to_MemoryviewSlice_ds_double(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_data.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_indices = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indices.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_indptr = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indptr.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_M = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_M == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_N = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_N == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
+    __pyx_v_output_file = __Pyx_PyObject_AsWritableString(values[0]); if (unlikely((!__pyx_v_output_file) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_barcodes = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_barcodes.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_features = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_features.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_data = __Pyx_PyObject_to_MemoryviewSlice_ds_double(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_data.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_indices = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indices.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_indptr = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indptr.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_M = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_M == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_N = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_N == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
     if (values[8]) {
-      __pyx_v_precision = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_precision == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
+      __pyx_v_precision = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_precision == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
     } else {
-      __pyx_v_precision = __pyx_k__38;
+      __pyx_v_precision = __pyx_k__39;
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_0_1write_dense", 0, 8, 9, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 197, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_0_1write_dense", 0, 8, 9, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 201, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pegasusio.cylib.io.__pyx_fuse_3_0_1write_dense", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9pegasusio_5cylib_2io_70__pyx_fuse_3_0_1write_dense(__pyx_self, __pyx_v_output_file, __pyx_v_barcodes, __pyx_v_features, __pyx_v_data, __pyx_v_indices, __pyx_v_indptr, __pyx_v_M, __pyx_v_N, __pyx_v_precision);
 
@@ -19582,23 +19697,23 @@
   struct __pyx_fuse_3_0_1__pyx_opt_args_9pegasusio_5cylib_2io_write_dense __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_3_0_1write_dense", 0);
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_barcodes.memview)) { __Pyx_RaiseUnboundLocalError("barcodes"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_features.memview)) { __Pyx_RaiseUnboundLocalError("features"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_data.memview)) { __Pyx_RaiseUnboundLocalError("data"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_indices.memview)) { __Pyx_RaiseUnboundLocalError("indices"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_indptr.memview)) { __Pyx_RaiseUnboundLocalError("indptr"); __PYX_ERR(0, 197, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_barcodes.memview)) { __Pyx_RaiseUnboundLocalError("barcodes"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_features.memview)) { __Pyx_RaiseUnboundLocalError("features"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_data.memview)) { __Pyx_RaiseUnboundLocalError("data"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_indices.memview)) { __Pyx_RaiseUnboundLocalError("indices"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_indptr.memview)) { __Pyx_RaiseUnboundLocalError("indptr"); __PYX_ERR(0, 201, __pyx_L1_error) }
   __pyx_t_1.__pyx_n = 1;
   __pyx_t_1.precision = __pyx_v_precision;
   __pyx_fuse_3_0_1__pyx_f_9pegasusio_5cylib_2io_write_dense(__pyx_v_output_file, __pyx_v_barcodes, __pyx_v_features, __pyx_v_data, __pyx_v_indices, __pyx_v_indptr, __pyx_v_M, __pyx_v_N, 0, &__pyx_t_1); 
-  __pyx_t_2 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -19615,15 +19730,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pw_9pegasusio_5cylib_2io_73__pyx_fuse_3_1_0write_dense(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_pw_9pegasusio_5cylib_2io_7write_dense(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static void __pyx_fuse_3_1_0__pyx_f_9pegasusio_5cylib_2io_write_dense(char *__pyx_v_output_file, __Pyx_memviewslice __pyx_v_barcodes, __Pyx_memviewslice __pyx_v_features, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_indices, __Pyx_memviewslice __pyx_v_indptr, int __pyx_v_M, int __pyx_v_N, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_fuse_3_1_0__pyx_opt_args_9pegasusio_5cylib_2io_write_dense *__pyx_optional_args) {
-  int __pyx_v_precision = __pyx_k__39;
+  int __pyx_v_precision = __pyx_k__40;
   FILE *__pyx_v_fo;
   PyObject *__pyx_v_fmt_str = 0;
   char const *__pyx_v_fmt;
   Py_ssize_t __pyx_v_i;
   Py_ssize_t __pyx_v_j;
   CYTHON_UNUSED Py_ssize_t __pyx_v_k;
   Py_ssize_t __pyx_v_fr;
@@ -19653,24 +19768,24 @@
   __Pyx_RefNannySetupContext("__pyx_fuse_3_1_0write_dense", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_precision = __pyx_optional_args->precision;
     }
   }
 
-  /* "ext_modules/io_funcs.pyx":200
+  /* "ext_modules/io_funcs.pyx":204
  *     """ Input must be csr_matrix internal representation, gene by cell (X.T.tocsr()); Output will be gene by cell
  *     """
  *     cdef FILE* fo = fopen(output_file, "w")             # <<<<<<<<<<<<<<
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"
  * 
  */
   __pyx_v_fo = fopen(__pyx_v_output_file, ((char const *)"w"));
 
-  /* "ext_modules/io_funcs.pyx":201
+  /* "ext_modules/io_funcs.pyx":205
  *     """
  *     cdef FILE* fo = fopen(output_file, "w")
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"             # <<<<<<<<<<<<<<
  * 
  *     cdef const char* fmt = fmt_str
  */
   __pyx_t_3 = (0 != 0);
@@ -19679,236 +19794,236 @@
     __pyx_t_2 = __pyx_t_3;
     goto __pyx_L3_bool_binop_done;
   }
   __pyx_t_3 = (1 != 0);
   __pyx_t_2 = __pyx_t_3;
   __pyx_L3_bool_binop_done:;
   if (__pyx_t_2) {
-    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = 0;
     __pyx_t_6 = 127;
-    __Pyx_INCREF(__pyx_kp_u__25);
+    __Pyx_INCREF(__pyx_kp_u__26);
     __pyx_t_5 += 3;
-    __Pyx_GIVEREF(__pyx_kp_u__25);
-    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u__25);
-    __pyx_t_7 = __Pyx_PyUnicode_From_int(__pyx_v_precision, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __Pyx_GIVEREF(__pyx_kp_u__26);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u__26);
+    __pyx_t_7 = __Pyx_PyUnicode_From_int(__pyx_v_precision, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_INCREF(__pyx_n_u_f_2);
     __pyx_t_5 += 1;
     __Pyx_GIVEREF(__pyx_n_u_f_2);
     PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_n_u_f_2);
-    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_1 = __pyx_t_7;
     __pyx_t_7 = 0;
   } else {
     __Pyx_INCREF(__pyx_kp_u_d);
     __pyx_t_1 = __pyx_kp_u_d;
   }
   __pyx_v_fmt_str = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "ext_modules/io_funcs.pyx":203
+  /* "ext_modules/io_funcs.pyx":207
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"
  * 
  *     cdef const char* fmt = fmt_str             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t i, j, k, fr
  * 
  */
-  __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_v_fmt_str); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 203, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_v_fmt_str); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 207, __pyx_L1_error)
   __pyx_v_fmt = __pyx_t_8;
 
-  /* "ext_modules/io_funcs.pyx":206
+  /* "ext_modules/io_funcs.pyx":210
  *     cdef Py_ssize_t i, j, k, fr
  * 
  *     fprintf(fo, "GENE");             # <<<<<<<<<<<<<<
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  */
   (void)(fprintf(__pyx_v_fo, ((char const *)"GENE")));
 
-  /* "ext_modules/io_funcs.pyx":207
+  /* "ext_modules/io_funcs.pyx":211
  * 
  *     fprintf(fo, "GENE");
  *     for i in range(N):             # <<<<<<<<<<<<<<
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  *     fprintf(fo, "\n")
  */
   __pyx_t_9 = __pyx_v_N;
   __pyx_t_10 = __pyx_t_9;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_10; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "ext_modules/io_funcs.pyx":208
+    /* "ext_modules/io_funcs.pyx":212
  *     fprintf(fo, "GENE");
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])             # <<<<<<<<<<<<<<
  *     fprintf(fo, "\n")
  * 
  */
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_1 = (PyObject *) *((PyObject * *) ( /* dim=0 */ (__pyx_v_barcodes.data + __pyx_t_11 * __pyx_v_barcodes.strides[0]) ));
     if (unlikely(__pyx_t_1 == NULL)) __pyx_t_1 = Py_None;
     __Pyx_INCREF((PyObject*)__pyx_t_1);
-    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 208, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 212, __pyx_L1_error)
     (void)(fprintf(__pyx_v_fo, ((char const *)"\t%s"), ((char *)__pyx_t_12)));
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
 
-  /* "ext_modules/io_funcs.pyx":209
+  /* "ext_modules/io_funcs.pyx":213
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  *     fprintf(fo, "\n")             # <<<<<<<<<<<<<<
  * 
  *     for i in range(M):
  */
   (void)(fprintf(__pyx_v_fo, ((char const *)"\n")));
 
-  /* "ext_modules/io_funcs.pyx":211
+  /* "ext_modules/io_funcs.pyx":215
  *     fprintf(fo, "\n")
  * 
  *     for i in range(M):             # <<<<<<<<<<<<<<
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0
  */
   __pyx_t_9 = __pyx_v_M;
   __pyx_t_10 = __pyx_t_9;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_10; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "ext_modules/io_funcs.pyx":212
+    /* "ext_modules/io_funcs.pyx":216
  * 
  *     for i in range(M):
  *         fprintf(fo, "%s", <char*>features[i]);             # <<<<<<<<<<<<<<
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):
  */
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_1 = (PyObject *) *((PyObject * *) ( /* dim=0 */ (__pyx_v_features.data + __pyx_t_11 * __pyx_v_features.strides[0]) ));
     if (unlikely(__pyx_t_1 == NULL)) __pyx_t_1 = Py_None;
     __Pyx_INCREF((PyObject*)__pyx_t_1);
-    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 212, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 216, __pyx_L1_error)
     (void)(fprintf(__pyx_v_fo, ((char const *)"%s"), ((char *)__pyx_t_12)));
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "ext_modules/io_funcs.pyx":213
+    /* "ext_modules/io_funcs.pyx":217
  *     for i in range(M):
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0             # <<<<<<<<<<<<<<
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):
  */
     __pyx_v_fr = 0;
 
-    /* "ext_modules/io_funcs.pyx":214
+    /* "ext_modules/io_funcs.pyx":218
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):             # <<<<<<<<<<<<<<
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")
  */
     __pyx_t_11 = (__pyx_v_i + 1);
     __pyx_t_13 = (*((int *) ( /* dim=0 */ (__pyx_v_indptr.data + __pyx_t_11 * __pyx_v_indptr.strides[0]) )));
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = (*((int *) ( /* dim=0 */ (__pyx_v_indptr.data + __pyx_t_11 * __pyx_v_indptr.strides[0]) ))); __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_j = __pyx_t_15;
 
-      /* "ext_modules/io_funcs.pyx":215
+      /* "ext_modules/io_funcs.pyx":219
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):             # <<<<<<<<<<<<<<
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])
  */
       __pyx_t_16 = __pyx_v_j;
       __pyx_t_17 = (*((long *) ( /* dim=0 */ (__pyx_v_indices.data + __pyx_t_16 * __pyx_v_indices.strides[0]) )));
       __pyx_t_18 = __pyx_t_17;
       for (__pyx_t_19 = __pyx_v_fr; __pyx_t_19 < __pyx_t_18; __pyx_t_19+=1) {
         __pyx_v_k = __pyx_t_19;
 
-        /* "ext_modules/io_funcs.pyx":216
+        /* "ext_modules/io_funcs.pyx":220
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")             # <<<<<<<<<<<<<<
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1
  */
         (void)(fprintf(__pyx_v_fo, ((char const *)"\t0")));
       }
 
-      /* "ext_modules/io_funcs.pyx":217
+      /* "ext_modules/io_funcs.pyx":221
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])             # <<<<<<<<<<<<<<
  *             fr = indices[j] + 1
  *         for k in range(fr, N):
  */
       __pyx_t_16 = __pyx_v_j;
       (void)(fprintf(__pyx_v_fo, __pyx_v_fmt, (*((double *) ( /* dim=0 */ (__pyx_v_data.data + __pyx_t_16 * __pyx_v_data.strides[0]) )))));
 
-      /* "ext_modules/io_funcs.pyx":218
+      /* "ext_modules/io_funcs.pyx":222
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1             # <<<<<<<<<<<<<<
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")
  */
       __pyx_t_16 = __pyx_v_j;
       __pyx_v_fr = ((*((long *) ( /* dim=0 */ (__pyx_v_indices.data + __pyx_t_16 * __pyx_v_indices.strides[0]) ))) + 1);
     }
 
-    /* "ext_modules/io_funcs.pyx":219
+    /* "ext_modules/io_funcs.pyx":223
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1
  *         for k in range(fr, N):             # <<<<<<<<<<<<<<
  *             fprintf(fo, "\t0")
  *         fprintf(fo, "\n")
  */
     __pyx_t_13 = __pyx_v_N;
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = __pyx_v_fr; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_k = __pyx_t_15;
 
-      /* "ext_modules/io_funcs.pyx":220
+      /* "ext_modules/io_funcs.pyx":224
  *             fr = indices[j] + 1
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")             # <<<<<<<<<<<<<<
  *         fprintf(fo, "\n")
  * 
  */
       (void)(fprintf(__pyx_v_fo, ((char const *)"\t0")));
     }
 
-    /* "ext_modules/io_funcs.pyx":221
+    /* "ext_modules/io_funcs.pyx":225
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")
  *         fprintf(fo, "\n")             # <<<<<<<<<<<<<<
  * 
  *     fclose(fo)
  */
     (void)(fprintf(__pyx_v_fo, ((char const *)"\n")));
   }
 
-  /* "ext_modules/io_funcs.pyx":223
+  /* "ext_modules/io_funcs.pyx":227
  *         fprintf(fo, "\n")
  * 
  *     fclose(fo)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   (void)(fclose(__pyx_v_fo));
 
-  /* "ext_modules/io_funcs.pyx":197
+  /* "ext_modules/io_funcs.pyx":201
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef void write_dense(char* output_file, str[:] barcodes, str[:] features, data_type[:] data, indices_type[:] indices, indptr_type[:] indptr, int M, int N, int precision = 2):             # <<<<<<<<<<<<<<
  *     """ Input must be csr_matrix internal representation, gene by cell (X.T.tocsr()); Output will be gene by cell
  *     """
  */
 
@@ -19976,61 +20091,61 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_output_file)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_barcodes)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_1_0write_dense", 0, 8, 9, 1); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_1_0write_dense", 0, 8, 9, 1); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_features)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_1_0write_dense", 0, 8, 9, 2); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_1_0write_dense", 0, 8, 9, 2); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_1_0write_dense", 0, 8, 9, 3); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_1_0write_dense", 0, 8, 9, 3); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_indices)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_1_0write_dense", 0, 8, 9, 4); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_1_0write_dense", 0, 8, 9, 4); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_indptr)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_1_0write_dense", 0, 8, 9, 5); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_1_0write_dense", 0, 8, 9, 5); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (likely((values[6] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_M)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_1_0write_dense", 0, 8, 9, 6); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_1_0write_dense", 0, 8, 9, 6); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  7:
         if (likely((values[7] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_N)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_1_0write_dense", 0, 8, 9, 7); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_1_0write_dense", 0, 8, 9, 7); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  8:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_precision);
           if (value) { values[8] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_3_1_0write_dense") < 0)) __PYX_ERR(0, 197, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_3_1_0write_dense") < 0)) __PYX_ERR(0, 201, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  9: values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
         CYTHON_FALLTHROUGH;
         case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
         values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
@@ -20040,31 +20155,31 @@
         values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_output_file = __Pyx_PyObject_AsWritableString(values[0]); if (unlikely((!__pyx_v_output_file) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_barcodes = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_barcodes.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_features = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_features.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_data = __Pyx_PyObject_to_MemoryviewSlice_ds_double(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_data.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_indices = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indices.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_indptr = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indptr.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_M = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_M == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_N = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_N == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
+    __pyx_v_output_file = __Pyx_PyObject_AsWritableString(values[0]); if (unlikely((!__pyx_v_output_file) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_barcodes = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_barcodes.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_features = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_features.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_data = __Pyx_PyObject_to_MemoryviewSlice_ds_double(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_data.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_indices = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indices.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_indptr = __Pyx_PyObject_to_MemoryviewSlice_ds_int(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indptr.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_M = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_M == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_N = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_N == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
     if (values[8]) {
-      __pyx_v_precision = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_precision == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
+      __pyx_v_precision = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_precision == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
     } else {
-      __pyx_v_precision = __pyx_k__39;
+      __pyx_v_precision = __pyx_k__40;
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_1_0write_dense", 0, 8, 9, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 197, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_1_0write_dense", 0, 8, 9, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 201, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pegasusio.cylib.io.__pyx_fuse_3_1_0write_dense", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9pegasusio_5cylib_2io_72__pyx_fuse_3_1_0write_dense(__pyx_self, __pyx_v_output_file, __pyx_v_barcodes, __pyx_v_features, __pyx_v_data, __pyx_v_indices, __pyx_v_indptr, __pyx_v_M, __pyx_v_N, __pyx_v_precision);
 
@@ -20079,23 +20194,23 @@
   struct __pyx_fuse_3_1_0__pyx_opt_args_9pegasusio_5cylib_2io_write_dense __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_3_1_0write_dense", 0);
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_barcodes.memview)) { __Pyx_RaiseUnboundLocalError("barcodes"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_features.memview)) { __Pyx_RaiseUnboundLocalError("features"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_data.memview)) { __Pyx_RaiseUnboundLocalError("data"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_indices.memview)) { __Pyx_RaiseUnboundLocalError("indices"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_indptr.memview)) { __Pyx_RaiseUnboundLocalError("indptr"); __PYX_ERR(0, 197, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_barcodes.memview)) { __Pyx_RaiseUnboundLocalError("barcodes"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_features.memview)) { __Pyx_RaiseUnboundLocalError("features"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_data.memview)) { __Pyx_RaiseUnboundLocalError("data"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_indices.memview)) { __Pyx_RaiseUnboundLocalError("indices"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_indptr.memview)) { __Pyx_RaiseUnboundLocalError("indptr"); __PYX_ERR(0, 201, __pyx_L1_error) }
   __pyx_t_1.__pyx_n = 1;
   __pyx_t_1.precision = __pyx_v_precision;
   __pyx_fuse_3_1_0__pyx_f_9pegasusio_5cylib_2io_write_dense(__pyx_v_output_file, __pyx_v_barcodes, __pyx_v_features, __pyx_v_data, __pyx_v_indices, __pyx_v_indptr, __pyx_v_M, __pyx_v_N, 0, &__pyx_t_1); 
-  __pyx_t_2 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -20112,15 +20227,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pw_9pegasusio_5cylib_2io_75__pyx_fuse_3_1_1write_dense(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_pw_9pegasusio_5cylib_2io_7write_dense(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static void __pyx_fuse_3_1_1__pyx_f_9pegasusio_5cylib_2io_write_dense(char *__pyx_v_output_file, __Pyx_memviewslice __pyx_v_barcodes, __Pyx_memviewslice __pyx_v_features, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_indices, __Pyx_memviewslice __pyx_v_indptr, int __pyx_v_M, int __pyx_v_N, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_fuse_3_1_1__pyx_opt_args_9pegasusio_5cylib_2io_write_dense *__pyx_optional_args) {
-  int __pyx_v_precision = __pyx_k__40;
+  int __pyx_v_precision = __pyx_k__41;
   FILE *__pyx_v_fo;
   PyObject *__pyx_v_fmt_str = 0;
   char const *__pyx_v_fmt;
   Py_ssize_t __pyx_v_i;
   Py_ssize_t __pyx_v_j;
   CYTHON_UNUSED Py_ssize_t __pyx_v_k;
   Py_ssize_t __pyx_v_fr;
@@ -20152,24 +20267,24 @@
   __Pyx_RefNannySetupContext("__pyx_fuse_3_1_1write_dense", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_precision = __pyx_optional_args->precision;
     }
   }
 
-  /* "ext_modules/io_funcs.pyx":200
+  /* "ext_modules/io_funcs.pyx":204
  *     """ Input must be csr_matrix internal representation, gene by cell (X.T.tocsr()); Output will be gene by cell
  *     """
  *     cdef FILE* fo = fopen(output_file, "w")             # <<<<<<<<<<<<<<
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"
  * 
  */
   __pyx_v_fo = fopen(__pyx_v_output_file, ((char const *)"w"));
 
-  /* "ext_modules/io_funcs.pyx":201
+  /* "ext_modules/io_funcs.pyx":205
  *     """
  *     cdef FILE* fo = fopen(output_file, "w")
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"             # <<<<<<<<<<<<<<
  * 
  *     cdef const char* fmt = fmt_str
  */
   __pyx_t_3 = (0 != 0);
@@ -20178,236 +20293,236 @@
     __pyx_t_2 = __pyx_t_3;
     goto __pyx_L3_bool_binop_done;
   }
   __pyx_t_3 = (1 != 0);
   __pyx_t_2 = __pyx_t_3;
   __pyx_L3_bool_binop_done:;
   if (__pyx_t_2) {
-    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = 0;
     __pyx_t_6 = 127;
-    __Pyx_INCREF(__pyx_kp_u__25);
+    __Pyx_INCREF(__pyx_kp_u__26);
     __pyx_t_5 += 3;
-    __Pyx_GIVEREF(__pyx_kp_u__25);
-    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u__25);
-    __pyx_t_7 = __Pyx_PyUnicode_From_int(__pyx_v_precision, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __Pyx_GIVEREF(__pyx_kp_u__26);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u__26);
+    __pyx_t_7 = __Pyx_PyUnicode_From_int(__pyx_v_precision, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_INCREF(__pyx_n_u_f_2);
     __pyx_t_5 += 1;
     __Pyx_GIVEREF(__pyx_n_u_f_2);
     PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_n_u_f_2);
-    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_1 = __pyx_t_7;
     __pyx_t_7 = 0;
   } else {
     __Pyx_INCREF(__pyx_kp_u_d);
     __pyx_t_1 = __pyx_kp_u_d;
   }
   __pyx_v_fmt_str = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "ext_modules/io_funcs.pyx":203
+  /* "ext_modules/io_funcs.pyx":207
  *     cdef str fmt_str = f"\t%.{precision}f" if (data_type is float) or (data_type is double) else "\t%d"
  * 
  *     cdef const char* fmt = fmt_str             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t i, j, k, fr
  * 
  */
-  __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_v_fmt_str); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 203, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_v_fmt_str); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 207, __pyx_L1_error)
   __pyx_v_fmt = __pyx_t_8;
 
-  /* "ext_modules/io_funcs.pyx":206
+  /* "ext_modules/io_funcs.pyx":210
  *     cdef Py_ssize_t i, j, k, fr
  * 
  *     fprintf(fo, "GENE");             # <<<<<<<<<<<<<<
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  */
   (void)(fprintf(__pyx_v_fo, ((char const *)"GENE")));
 
-  /* "ext_modules/io_funcs.pyx":207
+  /* "ext_modules/io_funcs.pyx":211
  * 
  *     fprintf(fo, "GENE");
  *     for i in range(N):             # <<<<<<<<<<<<<<
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  *     fprintf(fo, "\n")
  */
   __pyx_t_9 = __pyx_v_N;
   __pyx_t_10 = __pyx_t_9;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_10; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "ext_modules/io_funcs.pyx":208
+    /* "ext_modules/io_funcs.pyx":212
  *     fprintf(fo, "GENE");
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])             # <<<<<<<<<<<<<<
  *     fprintf(fo, "\n")
  * 
  */
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_1 = (PyObject *) *((PyObject * *) ( /* dim=0 */ (__pyx_v_barcodes.data + __pyx_t_11 * __pyx_v_barcodes.strides[0]) ));
     if (unlikely(__pyx_t_1 == NULL)) __pyx_t_1 = Py_None;
     __Pyx_INCREF((PyObject*)__pyx_t_1);
-    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 208, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 212, __pyx_L1_error)
     (void)(fprintf(__pyx_v_fo, ((char const *)"\t%s"), ((char *)__pyx_t_12)));
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
 
-  /* "ext_modules/io_funcs.pyx":209
+  /* "ext_modules/io_funcs.pyx":213
  *     for i in range(N):
  *         fprintf(fo, "\t%s", <char*>barcodes[i])
  *     fprintf(fo, "\n")             # <<<<<<<<<<<<<<
  * 
  *     for i in range(M):
  */
   (void)(fprintf(__pyx_v_fo, ((char const *)"\n")));
 
-  /* "ext_modules/io_funcs.pyx":211
+  /* "ext_modules/io_funcs.pyx":215
  *     fprintf(fo, "\n")
  * 
  *     for i in range(M):             # <<<<<<<<<<<<<<
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0
  */
   __pyx_t_9 = __pyx_v_M;
   __pyx_t_10 = __pyx_t_9;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_10; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "ext_modules/io_funcs.pyx":212
+    /* "ext_modules/io_funcs.pyx":216
  * 
  *     for i in range(M):
  *         fprintf(fo, "%s", <char*>features[i]);             # <<<<<<<<<<<<<<
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):
  */
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_1 = (PyObject *) *((PyObject * *) ( /* dim=0 */ (__pyx_v_features.data + __pyx_t_11 * __pyx_v_features.strides[0]) ));
     if (unlikely(__pyx_t_1 == NULL)) __pyx_t_1 = Py_None;
     __Pyx_INCREF((PyObject*)__pyx_t_1);
-    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 212, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 216, __pyx_L1_error)
     (void)(fprintf(__pyx_v_fo, ((char const *)"%s"), ((char *)__pyx_t_12)));
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "ext_modules/io_funcs.pyx":213
+    /* "ext_modules/io_funcs.pyx":217
  *     for i in range(M):
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0             # <<<<<<<<<<<<<<
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):
  */
     __pyx_v_fr = 0;
 
-    /* "ext_modules/io_funcs.pyx":214
+    /* "ext_modules/io_funcs.pyx":218
  *         fprintf(fo, "%s", <char*>features[i]);
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):             # <<<<<<<<<<<<<<
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")
  */
     __pyx_t_11 = (__pyx_v_i + 1);
     __pyx_t_13 = (*((long *) ( /* dim=0 */ (__pyx_v_indptr.data + __pyx_t_11 * __pyx_v_indptr.strides[0]) )));
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = (*((long *) ( /* dim=0 */ (__pyx_v_indptr.data + __pyx_t_11 * __pyx_v_indptr.strides[0]) ))); __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_j = __pyx_t_15;
 
-      /* "ext_modules/io_funcs.pyx":215
+      /* "ext_modules/io_funcs.pyx":219
  *         fr = 0
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):             # <<<<<<<<<<<<<<
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])
  */
       __pyx_t_16 = __pyx_v_j;
       __pyx_t_17 = (*((long *) ( /* dim=0 */ (__pyx_v_indices.data + __pyx_t_16 * __pyx_v_indices.strides[0]) )));
       __pyx_t_18 = __pyx_t_17;
       for (__pyx_t_19 = __pyx_v_fr; __pyx_t_19 < __pyx_t_18; __pyx_t_19+=1) {
         __pyx_v_k = __pyx_t_19;
 
-        /* "ext_modules/io_funcs.pyx":216
+        /* "ext_modules/io_funcs.pyx":220
  *         for j in range(indptr[i], indptr[i + 1]):
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")             # <<<<<<<<<<<<<<
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1
  */
         (void)(fprintf(__pyx_v_fo, ((char const *)"\t0")));
       }
 
-      /* "ext_modules/io_funcs.pyx":217
+      /* "ext_modules/io_funcs.pyx":221
  *             for k in range(fr, indices[j]):
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])             # <<<<<<<<<<<<<<
  *             fr = indices[j] + 1
  *         for k in range(fr, N):
  */
       __pyx_t_16 = __pyx_v_j;
       (void)(fprintf(__pyx_v_fo, __pyx_v_fmt, (*((double *) ( /* dim=0 */ (__pyx_v_data.data + __pyx_t_16 * __pyx_v_data.strides[0]) )))));
 
-      /* "ext_modules/io_funcs.pyx":218
+      /* "ext_modules/io_funcs.pyx":222
  *                 fprintf(fo, "\t0")
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1             # <<<<<<<<<<<<<<
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")
  */
       __pyx_t_16 = __pyx_v_j;
       __pyx_v_fr = ((*((long *) ( /* dim=0 */ (__pyx_v_indices.data + __pyx_t_16 * __pyx_v_indices.strides[0]) ))) + 1);
     }
 
-    /* "ext_modules/io_funcs.pyx":219
+    /* "ext_modules/io_funcs.pyx":223
  *             fprintf(fo, fmt, data[j])
  *             fr = indices[j] + 1
  *         for k in range(fr, N):             # <<<<<<<<<<<<<<
  *             fprintf(fo, "\t0")
  *         fprintf(fo, "\n")
  */
     __pyx_t_20 = __pyx_v_N;
     __pyx_t_21 = __pyx_t_20;
     for (__pyx_t_15 = __pyx_v_fr; __pyx_t_15 < __pyx_t_21; __pyx_t_15+=1) {
       __pyx_v_k = __pyx_t_15;
 
-      /* "ext_modules/io_funcs.pyx":220
+      /* "ext_modules/io_funcs.pyx":224
  *             fr = indices[j] + 1
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")             # <<<<<<<<<<<<<<
  *         fprintf(fo, "\n")
  * 
  */
       (void)(fprintf(__pyx_v_fo, ((char const *)"\t0")));
     }
 
-    /* "ext_modules/io_funcs.pyx":221
+    /* "ext_modules/io_funcs.pyx":225
  *         for k in range(fr, N):
  *             fprintf(fo, "\t0")
  *         fprintf(fo, "\n")             # <<<<<<<<<<<<<<
  * 
  *     fclose(fo)
  */
     (void)(fprintf(__pyx_v_fo, ((char const *)"\n")));
   }
 
-  /* "ext_modules/io_funcs.pyx":223
+  /* "ext_modules/io_funcs.pyx":227
  *         fprintf(fo, "\n")
  * 
  *     fclose(fo)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   (void)(fclose(__pyx_v_fo));
 
-  /* "ext_modules/io_funcs.pyx":197
+  /* "ext_modules/io_funcs.pyx":201
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef void write_dense(char* output_file, str[:] barcodes, str[:] features, data_type[:] data, indices_type[:] indices, indptr_type[:] indptr, int M, int N, int precision = 2):             # <<<<<<<<<<<<<<
  *     """ Input must be csr_matrix internal representation, gene by cell (X.T.tocsr()); Output will be gene by cell
  *     """
  */
 
@@ -20475,61 +20590,61 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_output_file)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_barcodes)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_1_1write_dense", 0, 8, 9, 1); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_1_1write_dense", 0, 8, 9, 1); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_features)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_1_1write_dense", 0, 8, 9, 2); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_1_1write_dense", 0, 8, 9, 2); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_1_1write_dense", 0, 8, 9, 3); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_1_1write_dense", 0, 8, 9, 3); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_indices)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_1_1write_dense", 0, 8, 9, 4); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_1_1write_dense", 0, 8, 9, 4); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_indptr)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_1_1write_dense", 0, 8, 9, 5); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_1_1write_dense", 0, 8, 9, 5); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (likely((values[6] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_M)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_1_1write_dense", 0, 8, 9, 6); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_1_1write_dense", 0, 8, 9, 6); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  7:
         if (likely((values[7] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_N)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_1_1write_dense", 0, 8, 9, 7); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_1_1write_dense", 0, 8, 9, 7); __PYX_ERR(0, 201, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  8:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_precision);
           if (value) { values[8] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_3_1_1write_dense") < 0)) __PYX_ERR(0, 197, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_fuse_3_1_1write_dense") < 0)) __PYX_ERR(0, 201, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  9: values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
         CYTHON_FALLTHROUGH;
         case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
         values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
@@ -20539,31 +20654,31 @@
         values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_output_file = __Pyx_PyObject_AsWritableString(values[0]); if (unlikely((!__pyx_v_output_file) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_barcodes = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_barcodes.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_features = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_features.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_data = __Pyx_PyObject_to_MemoryviewSlice_ds_double(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_data.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_indices = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indices.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_indptr = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indptr.memview)) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_M = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_M == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
-    __pyx_v_N = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_N == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
+    __pyx_v_output_file = __Pyx_PyObject_AsWritableString(values[0]); if (unlikely((!__pyx_v_output_file) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_barcodes = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_barcodes.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_features = __Pyx_PyObject_to_MemoryviewSlice_ds_object(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_features.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_data = __Pyx_PyObject_to_MemoryviewSlice_ds_double(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_data.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_indices = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indices.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_indptr = __Pyx_PyObject_to_MemoryviewSlice_ds_long(values[5], PyBUF_WRITABLE); if (unlikely(!__pyx_v_indptr.memview)) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_M = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_M == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_N = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_N == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
     if (values[8]) {
-      __pyx_v_precision = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_precision == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
+      __pyx_v_precision = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_precision == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
     } else {
-      __pyx_v_precision = __pyx_k__40;
+      __pyx_v_precision = __pyx_k__41;
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_1_1write_dense", 0, 8, 9, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 197, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__pyx_fuse_3_1_1write_dense", 0, 8, 9, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 201, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pegasusio.cylib.io.__pyx_fuse_3_1_1write_dense", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9pegasusio_5cylib_2io_74__pyx_fuse_3_1_1write_dense(__pyx_self, __pyx_v_output_file, __pyx_v_barcodes, __pyx_v_features, __pyx_v_data, __pyx_v_indices, __pyx_v_indptr, __pyx_v_M, __pyx_v_N, __pyx_v_precision);
 
@@ -20578,23 +20693,23 @@
   struct __pyx_fuse_3_1_1__pyx_opt_args_9pegasusio_5cylib_2io_write_dense __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_3_1_1write_dense", 0);
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_barcodes.memview)) { __Pyx_RaiseUnboundLocalError("barcodes"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_features.memview)) { __Pyx_RaiseUnboundLocalError("features"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_data.memview)) { __Pyx_RaiseUnboundLocalError("data"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_indices.memview)) { __Pyx_RaiseUnboundLocalError("indices"); __PYX_ERR(0, 197, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_indptr.memview)) { __Pyx_RaiseUnboundLocalError("indptr"); __PYX_ERR(0, 197, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_barcodes.memview)) { __Pyx_RaiseUnboundLocalError("barcodes"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_features.memview)) { __Pyx_RaiseUnboundLocalError("features"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_data.memview)) { __Pyx_RaiseUnboundLocalError("data"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_indices.memview)) { __Pyx_RaiseUnboundLocalError("indices"); __PYX_ERR(0, 201, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_indptr.memview)) { __Pyx_RaiseUnboundLocalError("indptr"); __PYX_ERR(0, 201, __pyx_L1_error) }
   __pyx_t_1.__pyx_n = 1;
   __pyx_t_1.precision = __pyx_v_precision;
   __pyx_fuse_3_1_1__pyx_f_9pegasusio_5cylib_2io_write_dense(__pyx_v_output_file, __pyx_v_barcodes, __pyx_v_features, __pyx_v_data, __pyx_v_indices, __pyx_v_indptr, __pyx_v_M, __pyx_v_N, 0, &__pyx_t_1); 
-  __pyx_t_2 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -20608,15 +20723,15 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_indices, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_indptr, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ext_modules/io_funcs.pyx":228
+/* "ext_modules/io_funcs.pyx":232
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cdef swapbytes(uchar* bytes_buffer, int s):             # <<<<<<<<<<<<<<
  *     cdef int i, j
  *     cdef uchar tmp
  */
 
@@ -20627,79 +20742,79 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   long __pyx_t_1;
   long __pyx_t_2;
   int __pyx_t_3;
   __Pyx_RefNannySetupContext("swapbytes", 0);
 
-  /* "ext_modules/io_funcs.pyx":232
+  /* "ext_modules/io_funcs.pyx":236
  *     cdef uchar tmp
  * 
  *     for i in range(s >> 1):             # <<<<<<<<<<<<<<
  *         j = s - i - 1
  *         tmp = bytes_buffer[i]
  */
   __pyx_t_1 = (__pyx_v_s >> 1);
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_i = __pyx_t_3;
 
-    /* "ext_modules/io_funcs.pyx":233
+    /* "ext_modules/io_funcs.pyx":237
  * 
  *     for i in range(s >> 1):
  *         j = s - i - 1             # <<<<<<<<<<<<<<
  *         tmp = bytes_buffer[i]
  *         bytes_buffer[i] = bytes_buffer[j]
  */
     __pyx_v_j = ((__pyx_v_s - __pyx_v_i) - 1);
 
-    /* "ext_modules/io_funcs.pyx":234
+    /* "ext_modules/io_funcs.pyx":238
  *     for i in range(s >> 1):
  *         j = s - i - 1
  *         tmp = bytes_buffer[i]             # <<<<<<<<<<<<<<
  *         bytes_buffer[i] = bytes_buffer[j]
  *         bytes_buffer[j] = tmp
  */
     __pyx_v_tmp = (__pyx_v_bytes_buffer[__pyx_v_i]);
 
-    /* "ext_modules/io_funcs.pyx":235
+    /* "ext_modules/io_funcs.pyx":239
  *         j = s - i - 1
  *         tmp = bytes_buffer[i]
  *         bytes_buffer[i] = bytes_buffer[j]             # <<<<<<<<<<<<<<
  *         bytes_buffer[j] = tmp
  * 
  */
     (__pyx_v_bytes_buffer[__pyx_v_i]) = (__pyx_v_bytes_buffer[__pyx_v_j]);
 
-    /* "ext_modules/io_funcs.pyx":236
+    /* "ext_modules/io_funcs.pyx":240
  *         tmp = bytes_buffer[i]
  *         bytes_buffer[i] = bytes_buffer[j]
  *         bytes_buffer[j] = tmp             # <<<<<<<<<<<<<<
  * 
  * 
  */
     (__pyx_v_bytes_buffer[__pyx_v_j]) = __pyx_v_tmp;
   }
 
-  /* "ext_modules/io_funcs.pyx":228
+  /* "ext_modules/io_funcs.pyx":232
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cdef swapbytes(uchar* bytes_buffer, int s):             # <<<<<<<<<<<<<<
  *     cdef int i, j
  *     cdef uchar tmp
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ext_modules/io_funcs.pyx":241
+/* "ext_modules/io_funcs.pyx":245
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef tuple read_fcs(char* fcs_file):             # <<<<<<<<<<<<<<
  *     """ This function is inspired by the python package fcsparser (https://github.com/eyurtsev/fcsparser)
  *     """
  */
 
@@ -20804,50 +20919,50 @@
   int __pyx_t_36;
   float __pyx_t_37;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("read_fcs", 0);
 
-  /* "ext_modules/io_funcs.pyx":244
+  /* "ext_modules/io_funcs.pyx":248
  *     """ This function is inspired by the python package fcsparser (https://github.com/eyurtsev/fcsparser)
  *     """
  *     cdef FILE* fi = fopen(fcs_file, "rb")             # <<<<<<<<<<<<<<
  * 
  *     # parse HEADER segment
  */
   __pyx_v_fi = fopen(__pyx_v_fcs_file, ((char const *)"rb"));
 
-  /* "ext_modules/io_funcs.pyx":251
+  /* "ext_modules/io_funcs.pyx":255
  *     cdef size_t text_start, text_end, data_start, data_end, analysis_start, analysis_end
  * 
  *     fcs_format[6] = header_field[8] = 0             # <<<<<<<<<<<<<<
  *     assert fread(<void*>fcs_format, 1, 6, fi) == 6
  *     if strcmp(fcs_format, "FCS2.0") and strcmp(fcs_format, "FCS3.0") and strcmp(fcs_format, "FCS3.1"):
  */
   (__pyx_v_fcs_format[6]) = 0;
   (__pyx_v_header_field[8]) = 0;
 
-  /* "ext_modules/io_funcs.pyx":252
+  /* "ext_modules/io_funcs.pyx":256
  * 
  *     fcs_format[6] = header_field[8] = 0
  *     assert fread(<void*>fcs_format, 1, 6, fi) == 6             # <<<<<<<<<<<<<<
  *     if strcmp(fcs_format, "FCS2.0") and strcmp(fcs_format, "FCS3.0") and strcmp(fcs_format, "FCS3.1"):
  *         fclose(fi)
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(!Py_OptimizeFlag)) {
     if (unlikely(!((fread(((void *)__pyx_v_fcs_format), 1, 6, __pyx_v_fi) == 6) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(0, 252, __pyx_L1_error)
+      __PYX_ERR(0, 256, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "ext_modules/io_funcs.pyx":253
+  /* "ext_modules/io_funcs.pyx":257
  *     fcs_format[6] = header_field[8] = 0
  *     assert fread(<void*>fcs_format, 1, 6, fi) == 6
  *     if strcmp(fcs_format, "FCS2.0") and strcmp(fcs_format, "FCS3.0") and strcmp(fcs_format, "FCS3.1"):             # <<<<<<<<<<<<<<
  *         fclose(fi)
  *         raise ValueError(f"Detected unsupported FCS format '{fcs_format}'!")
  */
   __pyx_t_2 = (strcmp(__pyx_v_fcs_format, ((char const *)"FCS2.0")) != 0);
@@ -20863,238 +20978,238 @@
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_2 = (strcmp(__pyx_v_fcs_format, ((char const *)"FCS3.1")) != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (unlikely(__pyx_t_1)) {
 
-    /* "ext_modules/io_funcs.pyx":254
+    /* "ext_modules/io_funcs.pyx":258
  *     assert fread(<void*>fcs_format, 1, 6, fi) == 6
  *     if strcmp(fcs_format, "FCS2.0") and strcmp(fcs_format, "FCS3.0") and strcmp(fcs_format, "FCS3.1"):
  *         fclose(fi)             # <<<<<<<<<<<<<<
  *         raise ValueError(f"Detected unsupported FCS format '{fcs_format}'!")
  * 
  */
     (void)(fclose(__pyx_v_fi));
 
-    /* "ext_modules/io_funcs.pyx":255
+    /* "ext_modules/io_funcs.pyx":259
  *     if strcmp(fcs_format, "FCS2.0") and strcmp(fcs_format, "FCS3.0") and strcmp(fcs_format, "FCS3.1"):
  *         fclose(fi)
  *         raise ValueError(f"Detected unsupported FCS format '{fcs_format}'!")             # <<<<<<<<<<<<<<
  * 
  *     assert fseek(fi, 4, SEEK_CUR) == 0
  */
-    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 255, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 259, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = 0;
     __pyx_t_5 = 127;
     __Pyx_INCREF(__pyx_kp_u_Detected_unsupported_FCS_format);
     __pyx_t_4 += 33;
     __Pyx_GIVEREF(__pyx_kp_u_Detected_unsupported_FCS_format);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_kp_u_Detected_unsupported_FCS_format);
-    __pyx_t_6 = __Pyx_PyObject_FromString(__pyx_v_fcs_format); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 255, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_FromString(__pyx_v_fcs_format); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 259, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_7 = __Pyx_PyObject_FormatSimple(__pyx_t_6, __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 255, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_FormatSimple(__pyx_t_6, __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 259, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) : __pyx_t_5;
     __pyx_t_4 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_7);
     __pyx_t_7 = 0;
-    __Pyx_INCREF(__pyx_kp_u__41);
+    __Pyx_INCREF(__pyx_kp_u__42);
     __pyx_t_4 += 2;
-    __Pyx_GIVEREF(__pyx_kp_u__41);
-    PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_kp_u__41);
-    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_3, 3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 255, __pyx_L1_error)
+    __Pyx_GIVEREF(__pyx_kp_u__42);
+    PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_kp_u__42);
+    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_3, 3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 259, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 255, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 259, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 255, __pyx_L1_error)
+    __PYX_ERR(0, 259, __pyx_L1_error)
 
-    /* "ext_modules/io_funcs.pyx":253
+    /* "ext_modules/io_funcs.pyx":257
  *     fcs_format[6] = header_field[8] = 0
  *     assert fread(<void*>fcs_format, 1, 6, fi) == 6
  *     if strcmp(fcs_format, "FCS2.0") and strcmp(fcs_format, "FCS3.0") and strcmp(fcs_format, "FCS3.1"):             # <<<<<<<<<<<<<<
  *         fclose(fi)
  *         raise ValueError(f"Detected unsupported FCS format '{fcs_format}'!")
  */
   }
 
-  /* "ext_modules/io_funcs.pyx":257
+  /* "ext_modules/io_funcs.pyx":261
  *         raise ValueError(f"Detected unsupported FCS format '{fcs_format}'!")
  * 
  *     assert fseek(fi, 4, SEEK_CUR) == 0             # <<<<<<<<<<<<<<
  *     assert fread(<void*>header_field, 1, 8, fi) == 8
  *     text_start = atoi(header_field)
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(!Py_OptimizeFlag)) {
     if (unlikely(!((fseek(__pyx_v_fi, 4, SEEK_CUR) == 0) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(0, 257, __pyx_L1_error)
+      __PYX_ERR(0, 261, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "ext_modules/io_funcs.pyx":258
+  /* "ext_modules/io_funcs.pyx":262
  * 
  *     assert fseek(fi, 4, SEEK_CUR) == 0
  *     assert fread(<void*>header_field, 1, 8, fi) == 8             # <<<<<<<<<<<<<<
  *     text_start = atoi(header_field)
  *     assert fread(<void*>header_field, 1, 8, fi) == 8
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(!Py_OptimizeFlag)) {
     if (unlikely(!((fread(((void *)__pyx_v_header_field), 1, 8, __pyx_v_fi) == 8) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(0, 258, __pyx_L1_error)
+      __PYX_ERR(0, 262, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "ext_modules/io_funcs.pyx":259
+  /* "ext_modules/io_funcs.pyx":263
  *     assert fseek(fi, 4, SEEK_CUR) == 0
  *     assert fread(<void*>header_field, 1, 8, fi) == 8
  *     text_start = atoi(header_field)             # <<<<<<<<<<<<<<
  *     assert fread(<void*>header_field, 1, 8, fi) == 8
  *     text_end = atoi(header_field)
  */
   __pyx_v_text_start = atoi(__pyx_v_header_field);
 
-  /* "ext_modules/io_funcs.pyx":260
+  /* "ext_modules/io_funcs.pyx":264
  *     assert fread(<void*>header_field, 1, 8, fi) == 8
  *     text_start = atoi(header_field)
  *     assert fread(<void*>header_field, 1, 8, fi) == 8             # <<<<<<<<<<<<<<
  *     text_end = atoi(header_field)
  *     assert fread(<void*>header_field, 1, 8, fi) == 8
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(!Py_OptimizeFlag)) {
     if (unlikely(!((fread(((void *)__pyx_v_header_field), 1, 8, __pyx_v_fi) == 8) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(0, 260, __pyx_L1_error)
+      __PYX_ERR(0, 264, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "ext_modules/io_funcs.pyx":261
+  /* "ext_modules/io_funcs.pyx":265
  *     text_start = atoi(header_field)
  *     assert fread(<void*>header_field, 1, 8, fi) == 8
  *     text_end = atoi(header_field)             # <<<<<<<<<<<<<<
  *     assert fread(<void*>header_field, 1, 8, fi) == 8
  *     data_start = atoi(header_field)
  */
   __pyx_v_text_end = atoi(__pyx_v_header_field);
 
-  /* "ext_modules/io_funcs.pyx":262
+  /* "ext_modules/io_funcs.pyx":266
  *     assert fread(<void*>header_field, 1, 8, fi) == 8
  *     text_end = atoi(header_field)
  *     assert fread(<void*>header_field, 1, 8, fi) == 8             # <<<<<<<<<<<<<<
  *     data_start = atoi(header_field)
  *     assert fread(<void*>header_field, 1, 8, fi) == 8
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(!Py_OptimizeFlag)) {
     if (unlikely(!((fread(((void *)__pyx_v_header_field), 1, 8, __pyx_v_fi) == 8) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(0, 262, __pyx_L1_error)
+      __PYX_ERR(0, 266, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "ext_modules/io_funcs.pyx":263
+  /* "ext_modules/io_funcs.pyx":267
  *     text_end = atoi(header_field)
  *     assert fread(<void*>header_field, 1, 8, fi) == 8
  *     data_start = atoi(header_field)             # <<<<<<<<<<<<<<
  *     assert fread(<void*>header_field, 1, 8, fi) == 8
  *     data_end = atoi(header_field)
  */
   __pyx_v_data_start = atoi(__pyx_v_header_field);
 
-  /* "ext_modules/io_funcs.pyx":264
+  /* "ext_modules/io_funcs.pyx":268
  *     assert fread(<void*>header_field, 1, 8, fi) == 8
  *     data_start = atoi(header_field)
  *     assert fread(<void*>header_field, 1, 8, fi) == 8             # <<<<<<<<<<<<<<
  *     data_end = atoi(header_field)
  *     assert fread(<void*>header_field, 1, 8, fi) == 8
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(!Py_OptimizeFlag)) {
     if (unlikely(!((fread(((void *)__pyx_v_header_field), 1, 8, __pyx_v_fi) == 8) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(0, 264, __pyx_L1_error)
+      __PYX_ERR(0, 268, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "ext_modules/io_funcs.pyx":265
+  /* "ext_modules/io_funcs.pyx":269
  *     data_start = atoi(header_field)
  *     assert fread(<void*>header_field, 1, 8, fi) == 8
  *     data_end = atoi(header_field)             # <<<<<<<<<<<<<<
  *     assert fread(<void*>header_field, 1, 8, fi) == 8
  *     analysis_start = atoi(header_field)
  */
   __pyx_v_data_end = atoi(__pyx_v_header_field);
 
-  /* "ext_modules/io_funcs.pyx":266
+  /* "ext_modules/io_funcs.pyx":270
  *     assert fread(<void*>header_field, 1, 8, fi) == 8
  *     data_end = atoi(header_field)
  *     assert fread(<void*>header_field, 1, 8, fi) == 8             # <<<<<<<<<<<<<<
  *     analysis_start = atoi(header_field)
  *     assert fread(<void*>header_field, 1, 8, fi) == 8
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(!Py_OptimizeFlag)) {
     if (unlikely(!((fread(((void *)__pyx_v_header_field), 1, 8, __pyx_v_fi) == 8) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(0, 266, __pyx_L1_error)
+      __PYX_ERR(0, 270, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "ext_modules/io_funcs.pyx":267
+  /* "ext_modules/io_funcs.pyx":271
  *     data_end = atoi(header_field)
  *     assert fread(<void*>header_field, 1, 8, fi) == 8
  *     analysis_start = atoi(header_field)             # <<<<<<<<<<<<<<
  *     assert fread(<void*>header_field, 1, 8, fi) == 8
  *     analysis_end = atoi(header_field)
  */
   __pyx_v_analysis_start = atoi(__pyx_v_header_field);
 
-  /* "ext_modules/io_funcs.pyx":268
+  /* "ext_modules/io_funcs.pyx":272
  *     assert fread(<void*>header_field, 1, 8, fi) == 8
  *     analysis_start = atoi(header_field)
  *     assert fread(<void*>header_field, 1, 8, fi) == 8             # <<<<<<<<<<<<<<
  *     analysis_end = atoi(header_field)
  * 
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(!Py_OptimizeFlag)) {
     if (unlikely(!((fread(((void *)__pyx_v_header_field), 1, 8, __pyx_v_fi) == 8) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(0, 268, __pyx_L1_error)
+      __PYX_ERR(0, 272, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "ext_modules/io_funcs.pyx":269
+  /* "ext_modules/io_funcs.pyx":273
  *     analysis_start = atoi(header_field)
  *     assert fread(<void*>header_field, 1, 8, fi) == 8
  *     analysis_end = atoi(header_field)             # <<<<<<<<<<<<<<
  * 
  *     if text_start < 58 or text_start >= text_end:
  */
   __pyx_v_analysis_end = atoi(__pyx_v_header_field);
 
-  /* "ext_modules/io_funcs.pyx":271
+  /* "ext_modules/io_funcs.pyx":275
  *     analysis_end = atoi(header_field)
  * 
  *     if text_start < 58 or text_start >= text_end:             # <<<<<<<<<<<<<<
  *         fclose(fi)
  *         raise ValueError(f"Detected invalid TEXT segment start and end offsets: [{text_start}, {text_end}]!")
  */
   __pyx_t_2 = ((__pyx_v_text_start < 58) != 0);
@@ -21104,321 +21219,321 @@
     goto __pyx_L8_bool_binop_done;
   }
   __pyx_t_2 = ((__pyx_v_text_start >= __pyx_v_text_end) != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L8_bool_binop_done:;
   if (unlikely(__pyx_t_1)) {
 
-    /* "ext_modules/io_funcs.pyx":272
+    /* "ext_modules/io_funcs.pyx":276
  * 
  *     if text_start < 58 or text_start >= text_end:
  *         fclose(fi)             # <<<<<<<<<<<<<<
  *         raise ValueError(f"Detected invalid TEXT segment start and end offsets: [{text_start}, {text_end}]!")
  * 
  */
     (void)(fclose(__pyx_v_fi));
 
-    /* "ext_modules/io_funcs.pyx":273
+    /* "ext_modules/io_funcs.pyx":277
  *     if text_start < 58 or text_start >= text_end:
  *         fclose(fi)
  *         raise ValueError(f"Detected invalid TEXT segment start and end offsets: [{text_start}, {text_end}]!")             # <<<<<<<<<<<<<<
  * 
  *     if text_end == data_start:
  */
-    __pyx_t_3 = PyTuple_New(5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 273, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 277, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = 0;
     __pyx_t_5 = 127;
     __Pyx_INCREF(__pyx_kp_u_Detected_invalid_TEXT_segment_st);
     __pyx_t_4 += 54;
     __Pyx_GIVEREF(__pyx_kp_u_Detected_invalid_TEXT_segment_st);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_kp_u_Detected_invalid_TEXT_segment_st);
-    __pyx_t_7 = __Pyx_PyUnicode_From_size_t(__pyx_v_text_start, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 273, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyUnicode_From_size_t(__pyx_v_text_start, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 277, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_4 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_7);
     __pyx_t_7 = 0;
-    __Pyx_INCREF(__pyx_kp_u__42);
+    __Pyx_INCREF(__pyx_kp_u__43);
     __pyx_t_4 += 2;
-    __Pyx_GIVEREF(__pyx_kp_u__42);
-    PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_kp_u__42);
-    __pyx_t_7 = __Pyx_PyUnicode_From_size_t(__pyx_v_text_end, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 273, __pyx_L1_error)
+    __Pyx_GIVEREF(__pyx_kp_u__43);
+    PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_kp_u__43);
+    __pyx_t_7 = __Pyx_PyUnicode_From_size_t(__pyx_v_text_end, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 277, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_4 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_3, 3, __pyx_t_7);
     __pyx_t_7 = 0;
-    __Pyx_INCREF(__pyx_kp_u__43);
+    __Pyx_INCREF(__pyx_kp_u__44);
     __pyx_t_4 += 2;
-    __Pyx_GIVEREF(__pyx_kp_u__43);
-    PyTuple_SET_ITEM(__pyx_t_3, 4, __pyx_kp_u__43);
-    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_3, 5, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 273, __pyx_L1_error)
+    __Pyx_GIVEREF(__pyx_kp_u__44);
+    PyTuple_SET_ITEM(__pyx_t_3, 4, __pyx_kp_u__44);
+    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_3, 5, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 277, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 273, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 277, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 273, __pyx_L1_error)
+    __PYX_ERR(0, 277, __pyx_L1_error)
 
-    /* "ext_modules/io_funcs.pyx":271
+    /* "ext_modules/io_funcs.pyx":275
  *     analysis_end = atoi(header_field)
  * 
  *     if text_start < 58 or text_start >= text_end:             # <<<<<<<<<<<<<<
  *         fclose(fi)
  *         raise ValueError(f"Detected invalid TEXT segment start and end offsets: [{text_start}, {text_end}]!")
  */
   }
 
-  /* "ext_modules/io_funcs.pyx":275
+  /* "ext_modules/io_funcs.pyx":279
  *         raise ValueError(f"Detected invalid TEXT segment start and end offsets: [{text_start}, {text_end}]!")
  * 
  *     if text_end == data_start:             # <<<<<<<<<<<<<<
  *         text_end -= 1
  * 
  */
   __pyx_t_1 = ((__pyx_v_text_end == __pyx_v_data_start) != 0);
   if (__pyx_t_1) {
 
-    /* "ext_modules/io_funcs.pyx":276
+    /* "ext_modules/io_funcs.pyx":280
  * 
  *     if text_end == data_start:
  *         text_end -= 1             # <<<<<<<<<<<<<<
  * 
  *     # parse TEXT segment
  */
     __pyx_v_text_end = (__pyx_v_text_end - 1);
 
-    /* "ext_modules/io_funcs.pyx":275
+    /* "ext_modules/io_funcs.pyx":279
  *         raise ValueError(f"Detected invalid TEXT segment start and end offsets: [{text_start}, {text_end}]!")
  * 
  *     if text_end == data_start:             # <<<<<<<<<<<<<<
  *         text_end -= 1
  * 
  */
   }
 
-  /* "ext_modules/io_funcs.pyx":283
+  /* "ext_modules/io_funcs.pyx":287
  *     cdef uchar* text_segment
  * 
  *     unicode_source = np.zeros(100000, dtype = np.uint8)             # <<<<<<<<<<<<<<
  * 
  *     cdef uchar[:] sview = unicode_source
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 283, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 283, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 283, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 283, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_uint8); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 283, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_uint8); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_8) < 0) __PYX_ERR(0, 283, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_8) < 0) __PYX_ERR(0, 287, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_tuple__44, __pyx_t_3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 283, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_tuple__45, __pyx_t_3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_unicode_source = __pyx_t_8;
   __pyx_t_8 = 0;
 
-  /* "ext_modules/io_funcs.pyx":285
+  /* "ext_modules/io_funcs.pyx":289
  *     unicode_source = np.zeros(100000, dtype = np.uint8)
  * 
  *     cdef uchar[:] sview = unicode_source             # <<<<<<<<<<<<<<
  *     cdef int s_pos # unicode source position
  *     cdef dict metadata = {}
  */
-  __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_9pegasusio_5cylib_2io_uchar(__pyx_v_unicode_source, PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 285, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_9pegasusio_5cylib_2io_uchar(__pyx_v_unicode_source, PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 289, __pyx_L1_error)
   __pyx_v_sview = __pyx_t_9;
   __pyx_t_9.memview = NULL;
   __pyx_t_9.data = NULL;
 
-  /* "ext_modules/io_funcs.pyx":287
+  /* "ext_modules/io_funcs.pyx":291
  *     cdef uchar[:] sview = unicode_source
  *     cdef int s_pos # unicode source position
  *     cdef dict metadata = {}             # <<<<<<<<<<<<<<
  *     cdef bytes value_bytes
  *     cdef str key, value
  */
-  __pyx_t_8 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 287, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 291, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __pyx_v_metadata = ((PyObject*)__pyx_t_8);
   __pyx_t_8 = 0;
 
-  /* "ext_modules/io_funcs.pyx":291
+  /* "ext_modules/io_funcs.pyx":295
  *     cdef str key, value
  * 
  *     text_bytes = text_end - text_start + 1             # <<<<<<<<<<<<<<
  *     text_segment = <uchar*>malloc(text_bytes)
  *     assert text_segment != NULL
  */
   __pyx_v_text_bytes = ((__pyx_v_text_end - __pyx_v_text_start) + 1);
 
-  /* "ext_modules/io_funcs.pyx":292
+  /* "ext_modules/io_funcs.pyx":296
  * 
  *     text_bytes = text_end - text_start + 1
  *     text_segment = <uchar*>malloc(text_bytes)             # <<<<<<<<<<<<<<
  *     assert text_segment != NULL
  *     assert fseek(fi, text_start, SEEK_SET) == 0
  */
   __pyx_v_text_segment = ((__pyx_t_9pegasusio_5cylib_2io_uchar *)malloc(__pyx_v_text_bytes));
 
-  /* "ext_modules/io_funcs.pyx":293
+  /* "ext_modules/io_funcs.pyx":297
  *     text_bytes = text_end - text_start + 1
  *     text_segment = <uchar*>malloc(text_bytes)
  *     assert text_segment != NULL             # <<<<<<<<<<<<<<
  *     assert fseek(fi, text_start, SEEK_SET) == 0
  *     assert fread(<void*>text_segment, 1, text_bytes, fi) == text_bytes
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(!Py_OptimizeFlag)) {
     if (unlikely(!((__pyx_v_text_segment != NULL) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(0, 293, __pyx_L1_error)
+      __PYX_ERR(0, 297, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "ext_modules/io_funcs.pyx":294
+  /* "ext_modules/io_funcs.pyx":298
  *     text_segment = <uchar*>malloc(text_bytes)
  *     assert text_segment != NULL
  *     assert fseek(fi, text_start, SEEK_SET) == 0             # <<<<<<<<<<<<<<
  *     assert fread(<void*>text_segment, 1, text_bytes, fi) == text_bytes
  * 
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(!Py_OptimizeFlag)) {
     if (unlikely(!((fseek(__pyx_v_fi, __pyx_v_text_start, SEEK_SET) == 0) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(0, 294, __pyx_L1_error)
+      __PYX_ERR(0, 298, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "ext_modules/io_funcs.pyx":295
+  /* "ext_modules/io_funcs.pyx":299
  *     assert text_segment != NULL
  *     assert fseek(fi, text_start, SEEK_SET) == 0
  *     assert fread(<void*>text_segment, 1, text_bytes, fi) == text_bytes             # <<<<<<<<<<<<<<
  * 
  *     # determine the end position of text segment
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(!Py_OptimizeFlag)) {
     if (unlikely(!((fread(((void *)__pyx_v_text_segment), 1, __pyx_v_text_bytes, __pyx_v_fi) == __pyx_v_text_bytes) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(0, 295, __pyx_L1_error)
+      __PYX_ERR(0, 299, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "ext_modules/io_funcs.pyx":298
+  /* "ext_modules/io_funcs.pyx":302
  * 
  *     # determine the end position of text segment
  *     delim = text_segment[0]             # <<<<<<<<<<<<<<
  *     pos = text_bytes - 1
  *     while text_segment[pos] != delim:
  */
   __pyx_v_delim = (__pyx_v_text_segment[0]);
 
-  /* "ext_modules/io_funcs.pyx":299
+  /* "ext_modules/io_funcs.pyx":303
  *     # determine the end position of text segment
  *     delim = text_segment[0]
  *     pos = text_bytes - 1             # <<<<<<<<<<<<<<
  *     while text_segment[pos] != delim:
  *         pos -= 1
  */
   __pyx_v_pos = (__pyx_v_text_bytes - 1);
 
-  /* "ext_modules/io_funcs.pyx":300
+  /* "ext_modules/io_funcs.pyx":304
  *     delim = text_segment[0]
  *     pos = text_bytes - 1
  *     while text_segment[pos] != delim:             # <<<<<<<<<<<<<<
  *         pos -= 1
  *     text_bytes = pos + 1
  */
   while (1) {
     __pyx_t_1 = (((__pyx_v_text_segment[__pyx_v_pos]) != __pyx_v_delim) != 0);
     if (!__pyx_t_1) break;
 
-    /* "ext_modules/io_funcs.pyx":301
+    /* "ext_modules/io_funcs.pyx":305
  *     pos = text_bytes - 1
  *     while text_segment[pos] != delim:
  *         pos -= 1             # <<<<<<<<<<<<<<
  *     text_bytes = pos + 1
  * 
  */
     __pyx_v_pos = (__pyx_v_pos - 1);
   }
 
-  /* "ext_modules/io_funcs.pyx":302
+  /* "ext_modules/io_funcs.pyx":306
  *     while text_segment[pos] != delim:
  *         pos -= 1
  *     text_bytes = pos + 1             # <<<<<<<<<<<<<<
  * 
  *     # generate key:value dictionary
  */
   __pyx_v_text_bytes = (__pyx_v_pos + 1);
 
-  /* "ext_modules/io_funcs.pyx":305
+  /* "ext_modules/io_funcs.pyx":309
  * 
  *     # generate key:value dictionary
  *     pos = 1             # <<<<<<<<<<<<<<
  *     s_pos = 0
  *     key = ""
  */
   __pyx_v_pos = 1;
 
-  /* "ext_modules/io_funcs.pyx":306
+  /* "ext_modules/io_funcs.pyx":310
  *     # generate key:value dictionary
  *     pos = 1
  *     s_pos = 0             # <<<<<<<<<<<<<<
  *     key = ""
  *     while pos < text_bytes:
  */
   __pyx_v_s_pos = 0;
 
-  /* "ext_modules/io_funcs.pyx":307
+  /* "ext_modules/io_funcs.pyx":311
  *     pos = 1
  *     s_pos = 0
  *     key = ""             # <<<<<<<<<<<<<<
  *     while pos < text_bytes:
  *         if text_segment[pos] == delim:
  */
   __Pyx_INCREF(__pyx_kp_u__5);
   __pyx_v_key = __pyx_kp_u__5;
 
-  /* "ext_modules/io_funcs.pyx":308
+  /* "ext_modules/io_funcs.pyx":312
  *     s_pos = 0
  *     key = ""
  *     while pos < text_bytes:             # <<<<<<<<<<<<<<
  *         if text_segment[pos] == delim:
  *             if pos + 2 < text_bytes and text_segment[pos + 1] == delim: # delimiter escaping cannot happen at the end of the text segment
  */
   while (1) {
     __pyx_t_1 = ((__pyx_v_pos < __pyx_v_text_bytes) != 0);
     if (!__pyx_t_1) break;
 
-    /* "ext_modules/io_funcs.pyx":309
+    /* "ext_modules/io_funcs.pyx":313
  *     key = ""
  *     while pos < text_bytes:
  *         if text_segment[pos] == delim:             # <<<<<<<<<<<<<<
  *             if pos + 2 < text_bytes and text_segment[pos + 1] == delim: # delimiter escaping cannot happen at the end of the text segment
  *                 sview[s_pos] = text_segment[pos]
  */
     __pyx_t_1 = (((__pyx_v_text_segment[__pyx_v_pos]) == __pyx_v_delim) != 0);
     if (__pyx_t_1) {
 
-      /* "ext_modules/io_funcs.pyx":310
+      /* "ext_modules/io_funcs.pyx":314
  *     while pos < text_bytes:
  *         if text_segment[pos] == delim:
  *             if pos + 2 < text_bytes and text_segment[pos + 1] == delim: # delimiter escaping cannot happen at the end of the text segment             # <<<<<<<<<<<<<<
  *                 sview[s_pos] = text_segment[pos]
  *                 s_pos += 1
  */
       __pyx_t_2 = (((__pyx_v_pos + 2) < __pyx_v_text_bytes) != 0);
@@ -21428,119 +21543,119 @@
         goto __pyx_L17_bool_binop_done;
       }
       __pyx_t_2 = (((__pyx_v_text_segment[(__pyx_v_pos + 1)]) == __pyx_v_delim) != 0);
       __pyx_t_1 = __pyx_t_2;
       __pyx_L17_bool_binop_done:;
       if (__pyx_t_1) {
 
-        /* "ext_modules/io_funcs.pyx":311
+        /* "ext_modules/io_funcs.pyx":315
  *         if text_segment[pos] == delim:
  *             if pos + 2 < text_bytes and text_segment[pos + 1] == delim: # delimiter escaping cannot happen at the end of the text segment
  *                 sview[s_pos] = text_segment[pos]             # <<<<<<<<<<<<<<
  *                 s_pos += 1
  *                 pos += 1
  */
         __pyx_t_10 = __pyx_v_s_pos;
         *((__pyx_t_9pegasusio_5cylib_2io_uchar *) ( /* dim=0 */ (__pyx_v_sview.data + __pyx_t_10 * __pyx_v_sview.strides[0]) )) = (__pyx_v_text_segment[__pyx_v_pos]);
 
-        /* "ext_modules/io_funcs.pyx":312
+        /* "ext_modules/io_funcs.pyx":316
  *             if pos + 2 < text_bytes and text_segment[pos + 1] == delim: # delimiter escaping cannot happen at the end of the text segment
  *                 sview[s_pos] = text_segment[pos]
  *                 s_pos += 1             # <<<<<<<<<<<<<<
  *                 pos += 1
  *             else:
  */
         __pyx_v_s_pos = (__pyx_v_s_pos + 1);
 
-        /* "ext_modules/io_funcs.pyx":313
+        /* "ext_modules/io_funcs.pyx":317
  *                 sview[s_pos] = text_segment[pos]
  *                 s_pos += 1
  *                 pos += 1             # <<<<<<<<<<<<<<
  *             else:
  *                 if s_pos == 0:
  */
         __pyx_v_pos = (__pyx_v_pos + 1);
 
-        /* "ext_modules/io_funcs.pyx":310
+        /* "ext_modules/io_funcs.pyx":314
  *     while pos < text_bytes:
  *         if text_segment[pos] == delim:
  *             if pos + 2 < text_bytes and text_segment[pos + 1] == delim: # delimiter escaping cannot happen at the end of the text segment             # <<<<<<<<<<<<<<
  *                 sview[s_pos] = text_segment[pos]
  *                 s_pos += 1
  */
         goto __pyx_L16;
       }
 
-      /* "ext_modules/io_funcs.pyx":315
+      /* "ext_modules/io_funcs.pyx":319
  *                 pos += 1
  *             else:
  *                 if s_pos == 0:             # <<<<<<<<<<<<<<
  *                     free(text_segment)
  *                     fclose(fi)
  */
       /*else*/ {
         __pyx_t_1 = ((__pyx_v_s_pos == 0) != 0);
         if (unlikely(__pyx_t_1)) {
 
-          /* "ext_modules/io_funcs.pyx":316
+          /* "ext_modules/io_funcs.pyx":320
  *             else:
  *                 if s_pos == 0:
  *                     free(text_segment)             # <<<<<<<<<<<<<<
  *                     fclose(fi)
  *                     raise ValueError("Keywords and keyword values must have lengths greater than zero!")
  */
           free(__pyx_v_text_segment);
 
-          /* "ext_modules/io_funcs.pyx":317
+          /* "ext_modules/io_funcs.pyx":321
  *                 if s_pos == 0:
  *                     free(text_segment)
  *                     fclose(fi)             # <<<<<<<<<<<<<<
  *                     raise ValueError("Keywords and keyword values must have lengths greater than zero!")
  * 
  */
           (void)(fclose(__pyx_v_fi));
 
-          /* "ext_modules/io_funcs.pyx":318
+          /* "ext_modules/io_funcs.pyx":322
  *                     free(text_segment)
  *                     fclose(fi)
  *                     raise ValueError("Keywords and keyword values must have lengths greater than zero!")             # <<<<<<<<<<<<<<
  * 
  *                 value_bytes = bytes(unicode_source[0:s_pos])
  */
-          __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__45, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 318, __pyx_L1_error)
+          __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__46, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 322, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           __Pyx_Raise(__pyx_t_8, 0, 0, 0);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-          __PYX_ERR(0, 318, __pyx_L1_error)
+          __PYX_ERR(0, 322, __pyx_L1_error)
 
-          /* "ext_modules/io_funcs.pyx":315
+          /* "ext_modules/io_funcs.pyx":319
  *                 pos += 1
  *             else:
  *                 if s_pos == 0:             # <<<<<<<<<<<<<<
  *                     free(text_segment)
  *                     fclose(fi)
  */
         }
 
-        /* "ext_modules/io_funcs.pyx":320
+        /* "ext_modules/io_funcs.pyx":324
  *                     raise ValueError("Keywords and keyword values must have lengths greater than zero!")
  * 
  *                 value_bytes = bytes(unicode_source[0:s_pos])             # <<<<<<<<<<<<<<
  *                 try:
  *                     value = value_bytes.decode(encoding = 'utf-8')
  */
-        __pyx_t_8 = __Pyx_PyObject_GetSlice(__pyx_v_unicode_source, 0, __pyx_v_s_pos, NULL, NULL, NULL, 1, 1, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 320, __pyx_L1_error)
+        __pyx_t_8 = __Pyx_PyObject_GetSlice(__pyx_v_unicode_source, 0, __pyx_v_s_pos, NULL, NULL, NULL, 1, 1, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 324, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
-        __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 320, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 324, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_XDECREF_SET(__pyx_v_value_bytes, ((PyObject*)__pyx_t_3));
         __pyx_t_3 = 0;
 
-        /* "ext_modules/io_funcs.pyx":321
+        /* "ext_modules/io_funcs.pyx":325
  * 
  *                 value_bytes = bytes(unicode_source[0:s_pos])
  *                 try:             # <<<<<<<<<<<<<<
  *                     value = value_bytes.decode(encoding = 'utf-8')
  *                 except UnicodeDecodeError:
  */
         {
@@ -21548,35 +21663,35 @@
           __Pyx_PyThreadState_assign
           __Pyx_ExceptionSave(&__pyx_t_11, &__pyx_t_12, &__pyx_t_13);
           __Pyx_XGOTREF(__pyx_t_11);
           __Pyx_XGOTREF(__pyx_t_12);
           __Pyx_XGOTREF(__pyx_t_13);
           /*try:*/ {
 
-            /* "ext_modules/io_funcs.pyx":322
+            /* "ext_modules/io_funcs.pyx":326
  *                 value_bytes = bytes(unicode_source[0:s_pos])
  *                 try:
  *                     value = value_bytes.decode(encoding = 'utf-8')             # <<<<<<<<<<<<<<
  *                 except UnicodeDecodeError:
  *                     value = value_bytes.decode(encoding = 'latin-1')
  */
-            __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_value_bytes, __pyx_n_s_decode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 322, __pyx_L20_error)
+            __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_value_bytes, __pyx_n_s_decode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 326, __pyx_L20_error)
             __Pyx_GOTREF(__pyx_t_3);
-            __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 322, __pyx_L20_error)
+            __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 326, __pyx_L20_error)
             __Pyx_GOTREF(__pyx_t_8);
-            if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_encoding, __pyx_kp_u_utf_8) < 0) __PYX_ERR(0, 322, __pyx_L20_error)
-            __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 322, __pyx_L20_error)
+            if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_encoding, __pyx_kp_u_utf_8) < 0) __PYX_ERR(0, 326, __pyx_L20_error)
+            __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 326, __pyx_L20_error)
             __Pyx_GOTREF(__pyx_t_7);
             __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
             __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-            if (!(likely(PyUnicode_CheckExact(__pyx_t_7))||((__pyx_t_7) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_7)->tp_name), 0))) __PYX_ERR(0, 322, __pyx_L20_error)
+            if (!(likely(PyUnicode_CheckExact(__pyx_t_7))||((__pyx_t_7) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_7)->tp_name), 0))) __PYX_ERR(0, 326, __pyx_L20_error)
             __Pyx_XDECREF_SET(__pyx_v_value, ((PyObject*)__pyx_t_7));
             __pyx_t_7 = 0;
 
-            /* "ext_modules/io_funcs.pyx":321
+            /* "ext_modules/io_funcs.pyx":325
  * 
  *                 value_bytes = bytes(unicode_source[0:s_pos])
  *                 try:             # <<<<<<<<<<<<<<
  *                     value = value_bytes.decode(encoding = 'utf-8')
  *                 except UnicodeDecodeError:
  */
           }
@@ -21587,57 +21702,57 @@
           __pyx_L20_error:;
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
           __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
           __PYX_XDEC_MEMVIEW(&__pyx_t_9, 1);
 
-          /* "ext_modules/io_funcs.pyx":323
+          /* "ext_modules/io_funcs.pyx":327
  *                 try:
  *                     value = value_bytes.decode(encoding = 'utf-8')
  *                 except UnicodeDecodeError:             # <<<<<<<<<<<<<<
  *                     value = value_bytes.decode(encoding = 'latin-1')
  * 
  */
           __pyx_t_14 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_UnicodeDecodeError);
           if (__pyx_t_14) {
             __Pyx_AddTraceback("pegasusio.cylib.io.read_fcs", __pyx_clineno, __pyx_lineno, __pyx_filename);
-            if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_8, &__pyx_t_3) < 0) __PYX_ERR(0, 323, __pyx_L22_except_error)
+            if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_8, &__pyx_t_3) < 0) __PYX_ERR(0, 327, __pyx_L22_except_error)
             __Pyx_GOTREF(__pyx_t_7);
             __Pyx_GOTREF(__pyx_t_8);
             __Pyx_GOTREF(__pyx_t_3);
 
-            /* "ext_modules/io_funcs.pyx":324
+            /* "ext_modules/io_funcs.pyx":328
  *                     value = value_bytes.decode(encoding = 'utf-8')
  *                 except UnicodeDecodeError:
  *                     value = value_bytes.decode(encoding = 'latin-1')             # <<<<<<<<<<<<<<
  * 
  *                 s_pos = 0
  */
-            __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_value_bytes, __pyx_n_s_decode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 324, __pyx_L22_except_error)
+            __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_value_bytes, __pyx_n_s_decode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 328, __pyx_L22_except_error)
             __Pyx_GOTREF(__pyx_t_6);
-            __pyx_t_15 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 324, __pyx_L22_except_error)
+            __pyx_t_15 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 328, __pyx_L22_except_error)
             __Pyx_GOTREF(__pyx_t_15);
-            if (PyDict_SetItem(__pyx_t_15, __pyx_n_s_encoding, __pyx_kp_u_latin_1) < 0) __PYX_ERR(0, 324, __pyx_L22_except_error)
-            __pyx_t_16 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_empty_tuple, __pyx_t_15); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 324, __pyx_L22_except_error)
+            if (PyDict_SetItem(__pyx_t_15, __pyx_n_s_encoding, __pyx_kp_u_latin_1) < 0) __PYX_ERR(0, 328, __pyx_L22_except_error)
+            __pyx_t_16 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_empty_tuple, __pyx_t_15); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 328, __pyx_L22_except_error)
             __Pyx_GOTREF(__pyx_t_16);
             __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
             __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-            if (!(likely(PyUnicode_CheckExact(__pyx_t_16))||((__pyx_t_16) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_16)->tp_name), 0))) __PYX_ERR(0, 324, __pyx_L22_except_error)
+            if (!(likely(PyUnicode_CheckExact(__pyx_t_16))||((__pyx_t_16) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_16)->tp_name), 0))) __PYX_ERR(0, 328, __pyx_L22_except_error)
             __Pyx_XDECREF_SET(__pyx_v_value, ((PyObject*)__pyx_t_16));
             __pyx_t_16 = 0;
             __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
             __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
             __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
             goto __pyx_L21_exception_handled;
           }
           goto __pyx_L22_except_error;
           __pyx_L22_except_error:;
 
-          /* "ext_modules/io_funcs.pyx":321
+          /* "ext_modules/io_funcs.pyx":325
  * 
  *                 value_bytes = bytes(unicode_source[0:s_pos])
  *                 try:             # <<<<<<<<<<<<<<
  *                     value = value_bytes.decode(encoding = 'utf-8')
  *                 except UnicodeDecodeError:
  */
           __Pyx_XGIVEREF(__pyx_t_11);
@@ -21649,345 +21764,345 @@
           __Pyx_XGIVEREF(__pyx_t_11);
           __Pyx_XGIVEREF(__pyx_t_12);
           __Pyx_XGIVEREF(__pyx_t_13);
           __Pyx_ExceptionReset(__pyx_t_11, __pyx_t_12, __pyx_t_13);
           __pyx_L27_try_end:;
         }
 
-        /* "ext_modules/io_funcs.pyx":326
+        /* "ext_modules/io_funcs.pyx":330
  *                     value = value_bytes.decode(encoding = 'latin-1')
  * 
  *                 s_pos = 0             # <<<<<<<<<<<<<<
  *                 if key == "":
  *                     key = value.upper() # keywords are case insensitive; convert them to upper case
  */
         __pyx_v_s_pos = 0;
 
-        /* "ext_modules/io_funcs.pyx":327
+        /* "ext_modules/io_funcs.pyx":331
  * 
  *                 s_pos = 0
  *                 if key == "":             # <<<<<<<<<<<<<<
  *                     key = value.upper() # keywords are case insensitive; convert them to upper case
  *                 else:
  */
-        __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_key, __pyx_kp_u__5, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 327, __pyx_L1_error)
+        __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_key, __pyx_kp_u__5, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 331, __pyx_L1_error)
         __pyx_t_2 = (__pyx_t_1 != 0);
         if (__pyx_t_2) {
 
-          /* "ext_modules/io_funcs.pyx":328
+          /* "ext_modules/io_funcs.pyx":332
  *                 s_pos = 0
  *                 if key == "":
  *                     key = value.upper() # keywords are case insensitive; convert them to upper case             # <<<<<<<<<<<<<<
  *                 else:
  *                     metadata[key] = value
  */
-          __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_upper); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 328, __pyx_L1_error)
+          __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_upper); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 332, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           __pyx_t_7 = NULL;
           if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
             __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_8);
             if (likely(__pyx_t_7)) {
               PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
               __Pyx_INCREF(__pyx_t_7);
               __Pyx_INCREF(function);
               __Pyx_DECREF_SET(__pyx_t_8, function);
             }
           }
           __pyx_t_3 = (__pyx_t_7) ? __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_7) : __Pyx_PyObject_CallNoArg(__pyx_t_8);
           __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-          if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 328, __pyx_L1_error)
+          if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 332, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-          if (!(likely(PyUnicode_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(0, 328, __pyx_L1_error)
+          if (!(likely(PyUnicode_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(0, 332, __pyx_L1_error)
           __Pyx_DECREF_SET(__pyx_v_key, ((PyObject*)__pyx_t_3));
           __pyx_t_3 = 0;
 
-          /* "ext_modules/io_funcs.pyx":327
+          /* "ext_modules/io_funcs.pyx":331
  * 
  *                 s_pos = 0
  *                 if key == "":             # <<<<<<<<<<<<<<
  *                     key = value.upper() # keywords are case insensitive; convert them to upper case
  *                 else:
  */
           goto __pyx_L30;
         }
 
-        /* "ext_modules/io_funcs.pyx":330
+        /* "ext_modules/io_funcs.pyx":334
  *                     key = value.upper() # keywords are case insensitive; convert them to upper case
  *                 else:
  *                     metadata[key] = value             # <<<<<<<<<<<<<<
  *                     key = ""
  *         else:
  */
         /*else*/ {
-          if (unlikely(PyDict_SetItem(__pyx_v_metadata, __pyx_v_key, __pyx_v_value) < 0)) __PYX_ERR(0, 330, __pyx_L1_error)
+          if (unlikely(PyDict_SetItem(__pyx_v_metadata, __pyx_v_key, __pyx_v_value) < 0)) __PYX_ERR(0, 334, __pyx_L1_error)
 
-          /* "ext_modules/io_funcs.pyx":331
+          /* "ext_modules/io_funcs.pyx":335
  *                 else:
  *                     metadata[key] = value
  *                     key = ""             # <<<<<<<<<<<<<<
  *         else:
  *             sview[s_pos] = text_segment[pos]
  */
           __Pyx_INCREF(__pyx_kp_u__5);
           __Pyx_DECREF_SET(__pyx_v_key, __pyx_kp_u__5);
         }
         __pyx_L30:;
       }
       __pyx_L16:;
 
-      /* "ext_modules/io_funcs.pyx":309
+      /* "ext_modules/io_funcs.pyx":313
  *     key = ""
  *     while pos < text_bytes:
  *         if text_segment[pos] == delim:             # <<<<<<<<<<<<<<
  *             if pos + 2 < text_bytes and text_segment[pos + 1] == delim: # delimiter escaping cannot happen at the end of the text segment
  *                 sview[s_pos] = text_segment[pos]
  */
       goto __pyx_L15;
     }
 
-    /* "ext_modules/io_funcs.pyx":333
+    /* "ext_modules/io_funcs.pyx":337
  *                     key = ""
  *         else:
  *             sview[s_pos] = text_segment[pos]             # <<<<<<<<<<<<<<
  *             s_pos += 1
  * 
  */
     /*else*/ {
       __pyx_t_10 = __pyx_v_s_pos;
       *((__pyx_t_9pegasusio_5cylib_2io_uchar *) ( /* dim=0 */ (__pyx_v_sview.data + __pyx_t_10 * __pyx_v_sview.strides[0]) )) = (__pyx_v_text_segment[__pyx_v_pos]);
 
-      /* "ext_modules/io_funcs.pyx":334
+      /* "ext_modules/io_funcs.pyx":338
  *         else:
  *             sview[s_pos] = text_segment[pos]
  *             s_pos += 1             # <<<<<<<<<<<<<<
  * 
  *         pos += 1
  */
       __pyx_v_s_pos = (__pyx_v_s_pos + 1);
     }
     __pyx_L15:;
 
-    /* "ext_modules/io_funcs.pyx":336
+    /* "ext_modules/io_funcs.pyx":340
  *             s_pos += 1
  * 
  *         pos += 1             # <<<<<<<<<<<<<<
  * 
  *         if s_pos >= 100000:
  */
     __pyx_v_pos = (__pyx_v_pos + 1);
 
-    /* "ext_modules/io_funcs.pyx":338
+    /* "ext_modules/io_funcs.pyx":342
  *         pos += 1
  * 
  *         if s_pos >= 100000:             # <<<<<<<<<<<<<<
  *             free(text_segment)
  *             fclose(fi)
  */
     __pyx_t_2 = ((__pyx_v_s_pos >= 0x186A0) != 0);
     if (unlikely(__pyx_t_2)) {
 
-      /* "ext_modules/io_funcs.pyx":339
+      /* "ext_modules/io_funcs.pyx":343
  * 
  *         if s_pos >= 100000:
  *             free(text_segment)             # <<<<<<<<<<<<<<
  *             fclose(fi)
  *             raise NotImplementedError("Keyword or keyward value length cannot exceed 10,000!")
  */
       free(__pyx_v_text_segment);
 
-      /* "ext_modules/io_funcs.pyx":340
+      /* "ext_modules/io_funcs.pyx":344
  *         if s_pos >= 100000:
  *             free(text_segment)
  *             fclose(fi)             # <<<<<<<<<<<<<<
  *             raise NotImplementedError("Keyword or keyward value length cannot exceed 10,000!")
  * 
  */
       (void)(fclose(__pyx_v_fi));
 
-      /* "ext_modules/io_funcs.pyx":341
+      /* "ext_modules/io_funcs.pyx":345
  *             free(text_segment)
  *             fclose(fi)
  *             raise NotImplementedError("Keyword or keyward value length cannot exceed 10,000!")             # <<<<<<<<<<<<<<
  * 
  *     free(text_segment)
  */
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__46, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 341, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__47, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 345, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(0, 341, __pyx_L1_error)
+      __PYX_ERR(0, 345, __pyx_L1_error)
 
-      /* "ext_modules/io_funcs.pyx":338
+      /* "ext_modules/io_funcs.pyx":342
  *         pos += 1
  * 
  *         if s_pos >= 100000:             # <<<<<<<<<<<<<<
  *             free(text_segment)
  *             fclose(fi)
  */
     }
   }
 
-  /* "ext_modules/io_funcs.pyx":343
+  /* "ext_modules/io_funcs.pyx":347
  *             raise NotImplementedError("Keyword or keyward value length cannot exceed 10,000!")
  * 
  *     free(text_segment)             # <<<<<<<<<<<<<<
  * 
  *     if key != "":
  */
   free(__pyx_v_text_segment);
 
-  /* "ext_modules/io_funcs.pyx":345
+  /* "ext_modules/io_funcs.pyx":349
  *     free(text_segment)
  * 
  *     if key != "":             # <<<<<<<<<<<<<<
  *         fclose(fi)
  *         raise ValueError(f"Keyword {key} does not have a keyword value!")
  */
-  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_key, __pyx_kp_u__5, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 345, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_key, __pyx_kp_u__5, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 349, __pyx_L1_error)
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "ext_modules/io_funcs.pyx":346
+    /* "ext_modules/io_funcs.pyx":350
  * 
  *     if key != "":
  *         fclose(fi)             # <<<<<<<<<<<<<<
  *         raise ValueError(f"Keyword {key} does not have a keyword value!")
  * 
  */
     (void)(fclose(__pyx_v_fi));
 
-    /* "ext_modules/io_funcs.pyx":347
+    /* "ext_modules/io_funcs.pyx":351
  *     if key != "":
  *         fclose(fi)
  *         raise ValueError(f"Keyword {key} does not have a keyword value!")             # <<<<<<<<<<<<<<
  * 
  *     # sanity checks
  */
-    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 347, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 351, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = 0;
     __pyx_t_5 = 127;
     __Pyx_INCREF(__pyx_kp_u_Keyword);
     __pyx_t_4 += 8;
     __Pyx_GIVEREF(__pyx_kp_u_Keyword);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_kp_u_Keyword);
-    __pyx_t_8 = __Pyx_PyUnicode_Unicode(__pyx_v_key); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 347, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyUnicode_Unicode(__pyx_v_key); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 351, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) : __pyx_t_5;
     __pyx_t_4 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_8);
     __Pyx_GIVEREF(__pyx_t_8);
     PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_8);
     __pyx_t_8 = 0;
     __Pyx_INCREF(__pyx_kp_u_does_not_have_a_keyword_value);
     __pyx_t_4 += 31;
     __Pyx_GIVEREF(__pyx_kp_u_does_not_have_a_keyword_value);
     PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_kp_u_does_not_have_a_keyword_value);
-    __pyx_t_8 = __Pyx_PyUnicode_Join(__pyx_t_3, 3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 347, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyUnicode_Join(__pyx_t_3, 3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 351, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 347, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 351, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 347, __pyx_L1_error)
+    __PYX_ERR(0, 351, __pyx_L1_error)
 
-    /* "ext_modules/io_funcs.pyx":345
+    /* "ext_modules/io_funcs.pyx":349
  *     free(text_segment)
  * 
  *     if key != "":             # <<<<<<<<<<<<<<
  *         fclose(fi)
  *         raise ValueError(f"Keyword {key} does not have a keyword value!")
  */
   }
 
-  /* "ext_modules/io_funcs.pyx":352
+  /* "ext_modules/io_funcs.pyx":356
  *     cdef size_t _start, _end
  * 
  *     _start = _end = 0             # <<<<<<<<<<<<<<
  *     if "$BEGINDATA" in metadata:
  *         _start = int(metadata.pop("$BEGINDATA"))
  */
   __pyx_v__start = 0;
   __pyx_v__end = 0;
 
-  /* "ext_modules/io_funcs.pyx":353
+  /* "ext_modules/io_funcs.pyx":357
  * 
  *     _start = _end = 0
  *     if "$BEGINDATA" in metadata:             # <<<<<<<<<<<<<<
  *         _start = int(metadata.pop("$BEGINDATA"))
  *     if "$ENDDATA" in metadata:
  */
-  __pyx_t_1 = (__Pyx_PyDict_ContainsTF(__pyx_kp_u_BEGINDATA, __pyx_v_metadata, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 353, __pyx_L1_error)
+  __pyx_t_1 = (__Pyx_PyDict_ContainsTF(__pyx_kp_u_BEGINDATA, __pyx_v_metadata, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 357, __pyx_L1_error)
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "ext_modules/io_funcs.pyx":354
+    /* "ext_modules/io_funcs.pyx":358
  *     _start = _end = 0
  *     if "$BEGINDATA" in metadata:
  *         _start = int(metadata.pop("$BEGINDATA"))             # <<<<<<<<<<<<<<
  *     if "$ENDDATA" in metadata:
  *         _end = int(metadata.pop("$ENDDATA"))
  */
-    __pyx_t_3 = __Pyx_PyDict_Pop(__pyx_v_metadata, __pyx_kp_u_BEGINDATA, ((PyObject *)NULL)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 354, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_Pop(__pyx_v_metadata, __pyx_kp_u_BEGINDATA, ((PyObject *)NULL)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 358, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_8 = __Pyx_PyNumber_Int(__pyx_t_3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 354, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyNumber_Int(__pyx_t_3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 358, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_17 = __Pyx_PyInt_As_size_t(__pyx_t_8); if (unlikely((__pyx_t_17 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 354, __pyx_L1_error)
+    __pyx_t_17 = __Pyx_PyInt_As_size_t(__pyx_t_8); if (unlikely((__pyx_t_17 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 358, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __pyx_v__start = __pyx_t_17;
 
-    /* "ext_modules/io_funcs.pyx":353
+    /* "ext_modules/io_funcs.pyx":357
  * 
  *     _start = _end = 0
  *     if "$BEGINDATA" in metadata:             # <<<<<<<<<<<<<<
  *         _start = int(metadata.pop("$BEGINDATA"))
  *     if "$ENDDATA" in metadata:
  */
   }
 
-  /* "ext_modules/io_funcs.pyx":355
+  /* "ext_modules/io_funcs.pyx":359
  *     if "$BEGINDATA" in metadata:
  *         _start = int(metadata.pop("$BEGINDATA"))
  *     if "$ENDDATA" in metadata:             # <<<<<<<<<<<<<<
  *         _end = int(metadata.pop("$ENDDATA"))
  *     if data_start == 0 and data_end == 0:
  */
-  __pyx_t_2 = (__Pyx_PyDict_ContainsTF(__pyx_kp_u_ENDDATA, __pyx_v_metadata, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 355, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PyDict_ContainsTF(__pyx_kp_u_ENDDATA, __pyx_v_metadata, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 359, __pyx_L1_error)
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (__pyx_t_1) {
 
-    /* "ext_modules/io_funcs.pyx":356
+    /* "ext_modules/io_funcs.pyx":360
  *         _start = int(metadata.pop("$BEGINDATA"))
  *     if "$ENDDATA" in metadata:
  *         _end = int(metadata.pop("$ENDDATA"))             # <<<<<<<<<<<<<<
  *     if data_start == 0 and data_end == 0:
  *         data_start = _start
  */
-    __pyx_t_8 = __Pyx_PyDict_Pop(__pyx_v_metadata, __pyx_kp_u_ENDDATA, ((PyObject *)NULL)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 356, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyDict_Pop(__pyx_v_metadata, __pyx_kp_u_ENDDATA, ((PyObject *)NULL)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 360, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_3 = __Pyx_PyNumber_Int(__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 356, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyNumber_Int(__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 360, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_17 = __Pyx_PyInt_As_size_t(__pyx_t_3); if (unlikely((__pyx_t_17 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 356, __pyx_L1_error)
+    __pyx_t_17 = __Pyx_PyInt_As_size_t(__pyx_t_3); if (unlikely((__pyx_t_17 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 360, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v__end = __pyx_t_17;
 
-    /* "ext_modules/io_funcs.pyx":355
+    /* "ext_modules/io_funcs.pyx":359
  *     if "$BEGINDATA" in metadata:
  *         _start = int(metadata.pop("$BEGINDATA"))
  *     if "$ENDDATA" in metadata:             # <<<<<<<<<<<<<<
  *         _end = int(metadata.pop("$ENDDATA"))
  *     if data_start == 0 and data_end == 0:
  */
   }
 
-  /* "ext_modules/io_funcs.pyx":357
+  /* "ext_modules/io_funcs.pyx":361
  *     if "$ENDDATA" in metadata:
  *         _end = int(metadata.pop("$ENDDATA"))
  *     if data_start == 0 and data_end == 0:             # <<<<<<<<<<<<<<
  *         data_start = _start
  *         data_end = _end
  */
   __pyx_t_2 = ((__pyx_v_data_start == 0) != 0);
@@ -21997,154 +22112,154 @@
     goto __pyx_L36_bool_binop_done;
   }
   __pyx_t_2 = ((__pyx_v_data_end == 0) != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L36_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "ext_modules/io_funcs.pyx":358
+    /* "ext_modules/io_funcs.pyx":362
  *         _end = int(metadata.pop("$ENDDATA"))
  *     if data_start == 0 and data_end == 0:
  *         data_start = _start             # <<<<<<<<<<<<<<
  *         data_end = _end
  *     if data_start == 0:
  */
     __pyx_v_data_start = __pyx_v__start;
 
-    /* "ext_modules/io_funcs.pyx":359
+    /* "ext_modules/io_funcs.pyx":363
  *     if data_start == 0 and data_end == 0:
  *         data_start = _start
  *         data_end = _end             # <<<<<<<<<<<<<<
  *     if data_start == 0:
  *         print("Warning: Could not detect a DATA segment!")
  */
     __pyx_v_data_end = __pyx_v__end;
 
-    /* "ext_modules/io_funcs.pyx":357
+    /* "ext_modules/io_funcs.pyx":361
  *     if "$ENDDATA" in metadata:
  *         _end = int(metadata.pop("$ENDDATA"))
  *     if data_start == 0 and data_end == 0:             # <<<<<<<<<<<<<<
  *         data_start = _start
  *         data_end = _end
  */
   }
 
-  /* "ext_modules/io_funcs.pyx":360
+  /* "ext_modules/io_funcs.pyx":364
  *         data_start = _start
  *         data_end = _end
  *     if data_start == 0:             # <<<<<<<<<<<<<<
  *         print("Warning: Could not detect a DATA segment!")
  * 
  */
   __pyx_t_1 = ((__pyx_v_data_start == 0) != 0);
   if (__pyx_t_1) {
 
-    /* "ext_modules/io_funcs.pyx":361
+    /* "ext_modules/io_funcs.pyx":365
  *         data_end = _end
  *     if data_start == 0:
  *         print("Warning: Could not detect a DATA segment!")             # <<<<<<<<<<<<<<
  * 
  *     _start = _end = 0
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_print, __pyx_tuple__47, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 361, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_print, __pyx_tuple__48, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 365, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "ext_modules/io_funcs.pyx":360
+    /* "ext_modules/io_funcs.pyx":364
  *         data_start = _start
  *         data_end = _end
  *     if data_start == 0:             # <<<<<<<<<<<<<<
  *         print("Warning: Could not detect a DATA segment!")
  * 
  */
   }
 
-  /* "ext_modules/io_funcs.pyx":363
+  /* "ext_modules/io_funcs.pyx":367
  *         print("Warning: Could not detect a DATA segment!")
  * 
  *     _start = _end = 0             # <<<<<<<<<<<<<<
  *     if "$BEGINANALYSIS" in metadata:
  *         _start = int(metadata.pop("$BEGINANALYSIS"))
  */
   __pyx_v__start = 0;
   __pyx_v__end = 0;
 
-  /* "ext_modules/io_funcs.pyx":364
+  /* "ext_modules/io_funcs.pyx":368
  * 
  *     _start = _end = 0
  *     if "$BEGINANALYSIS" in metadata:             # <<<<<<<<<<<<<<
  *         _start = int(metadata.pop("$BEGINANALYSIS"))
  *     if "$ENDANALYSIS" in metadata:
  */
-  __pyx_t_1 = (__Pyx_PyDict_ContainsTF(__pyx_kp_u_BEGINANALYSIS, __pyx_v_metadata, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 364, __pyx_L1_error)
+  __pyx_t_1 = (__Pyx_PyDict_ContainsTF(__pyx_kp_u_BEGINANALYSIS, __pyx_v_metadata, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 368, __pyx_L1_error)
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "ext_modules/io_funcs.pyx":365
+    /* "ext_modules/io_funcs.pyx":369
  *     _start = _end = 0
  *     if "$BEGINANALYSIS" in metadata:
  *         _start = int(metadata.pop("$BEGINANALYSIS"))             # <<<<<<<<<<<<<<
  *     if "$ENDANALYSIS" in metadata:
  *         _end = int(metadata.pop("$ENDANALYSIS"))
  */
-    __pyx_t_3 = __Pyx_PyDict_Pop(__pyx_v_metadata, __pyx_kp_u_BEGINANALYSIS, ((PyObject *)NULL)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 365, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_Pop(__pyx_v_metadata, __pyx_kp_u_BEGINANALYSIS, ((PyObject *)NULL)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 369, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_8 = __Pyx_PyNumber_Int(__pyx_t_3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 365, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyNumber_Int(__pyx_t_3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 369, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_17 = __Pyx_PyInt_As_size_t(__pyx_t_8); if (unlikely((__pyx_t_17 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 365, __pyx_L1_error)
+    __pyx_t_17 = __Pyx_PyInt_As_size_t(__pyx_t_8); if (unlikely((__pyx_t_17 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 369, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __pyx_v__start = __pyx_t_17;
 
-    /* "ext_modules/io_funcs.pyx":364
+    /* "ext_modules/io_funcs.pyx":368
  * 
  *     _start = _end = 0
  *     if "$BEGINANALYSIS" in metadata:             # <<<<<<<<<<<<<<
  *         _start = int(metadata.pop("$BEGINANALYSIS"))
  *     if "$ENDANALYSIS" in metadata:
  */
   }
 
-  /* "ext_modules/io_funcs.pyx":366
+  /* "ext_modules/io_funcs.pyx":370
  *     if "$BEGINANALYSIS" in metadata:
  *         _start = int(metadata.pop("$BEGINANALYSIS"))
  *     if "$ENDANALYSIS" in metadata:             # <<<<<<<<<<<<<<
  *         _end = int(metadata.pop("$ENDANALYSIS"))
  *     if analysis_start == 0 and analysis_end == 0:
  */
-  __pyx_t_2 = (__Pyx_PyDict_ContainsTF(__pyx_kp_u_ENDANALYSIS, __pyx_v_metadata, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 366, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PyDict_ContainsTF(__pyx_kp_u_ENDANALYSIS, __pyx_v_metadata, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 370, __pyx_L1_error)
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (__pyx_t_1) {
 
-    /* "ext_modules/io_funcs.pyx":367
+    /* "ext_modules/io_funcs.pyx":371
  *         _start = int(metadata.pop("$BEGINANALYSIS"))
  *     if "$ENDANALYSIS" in metadata:
  *         _end = int(metadata.pop("$ENDANALYSIS"))             # <<<<<<<<<<<<<<
  *     if analysis_start == 0 and analysis_end == 0:
  *         analysis_start = _start
  */
-    __pyx_t_8 = __Pyx_PyDict_Pop(__pyx_v_metadata, __pyx_kp_u_ENDANALYSIS, ((PyObject *)NULL)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 367, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyDict_Pop(__pyx_v_metadata, __pyx_kp_u_ENDANALYSIS, ((PyObject *)NULL)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 371, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_3 = __Pyx_PyNumber_Int(__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 367, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyNumber_Int(__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 371, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_17 = __Pyx_PyInt_As_size_t(__pyx_t_3); if (unlikely((__pyx_t_17 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 367, __pyx_L1_error)
+    __pyx_t_17 = __Pyx_PyInt_As_size_t(__pyx_t_3); if (unlikely((__pyx_t_17 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 371, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v__end = __pyx_t_17;
 
-    /* "ext_modules/io_funcs.pyx":366
+    /* "ext_modules/io_funcs.pyx":370
  *     if "$BEGINANALYSIS" in metadata:
  *         _start = int(metadata.pop("$BEGINANALYSIS"))
  *     if "$ENDANALYSIS" in metadata:             # <<<<<<<<<<<<<<
  *         _end = int(metadata.pop("$ENDANALYSIS"))
  *     if analysis_start == 0 and analysis_end == 0:
  */
   }
 
-  /* "ext_modules/io_funcs.pyx":368
+  /* "ext_modules/io_funcs.pyx":372
  *     if "$ENDANALYSIS" in metadata:
  *         _end = int(metadata.pop("$ENDANALYSIS"))
  *     if analysis_start == 0 and analysis_end == 0:             # <<<<<<<<<<<<<<
  *         analysis_start = _start
  *         analysis_end = _end
  */
   __pyx_t_2 = ((__pyx_v_analysis_start == 0) != 0);
@@ -22154,392 +22269,392 @@
     goto __pyx_L42_bool_binop_done;
   }
   __pyx_t_2 = ((__pyx_v_analysis_end == 0) != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L42_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "ext_modules/io_funcs.pyx":369
+    /* "ext_modules/io_funcs.pyx":373
  *         _end = int(metadata.pop("$ENDANALYSIS"))
  *     if analysis_start == 0 and analysis_end == 0:
  *         analysis_start = _start             # <<<<<<<<<<<<<<
  *         analysis_end = _end
  *     if analysis_start > 0:
  */
     __pyx_v_analysis_start = __pyx_v__start;
 
-    /* "ext_modules/io_funcs.pyx":370
+    /* "ext_modules/io_funcs.pyx":374
  *     if analysis_start == 0 and analysis_end == 0:
  *         analysis_start = _start
  *         analysis_end = _end             # <<<<<<<<<<<<<<
  *     if analysis_start > 0:
  *         print("Warning: ANALYSIS segment would be omitted since current implementation does not support parsing of this segment.")
  */
     __pyx_v_analysis_end = __pyx_v__end;
 
-    /* "ext_modules/io_funcs.pyx":368
+    /* "ext_modules/io_funcs.pyx":372
  *     if "$ENDANALYSIS" in metadata:
  *         _end = int(metadata.pop("$ENDANALYSIS"))
  *     if analysis_start == 0 and analysis_end == 0:             # <<<<<<<<<<<<<<
  *         analysis_start = _start
  *         analysis_end = _end
  */
   }
 
-  /* "ext_modules/io_funcs.pyx":371
+  /* "ext_modules/io_funcs.pyx":375
  *         analysis_start = _start
  *         analysis_end = _end
  *     if analysis_start > 0:             # <<<<<<<<<<<<<<
  *         print("Warning: ANALYSIS segment would be omitted since current implementation does not support parsing of this segment.")
  * 
  */
   __pyx_t_1 = ((__pyx_v_analysis_start > 0) != 0);
   if (__pyx_t_1) {
 
-    /* "ext_modules/io_funcs.pyx":372
+    /* "ext_modules/io_funcs.pyx":376
  *         analysis_end = _end
  *     if analysis_start > 0:
  *         print("Warning: ANALYSIS segment would be omitted since current implementation does not support parsing of this segment.")             # <<<<<<<<<<<<<<
  * 
  *     if "$BEGINSTEXT" in metadata:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_print, __pyx_tuple__48, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 372, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_print, __pyx_tuple__49, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 376, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "ext_modules/io_funcs.pyx":371
+    /* "ext_modules/io_funcs.pyx":375
  *         analysis_start = _start
  *         analysis_end = _end
  *     if analysis_start > 0:             # <<<<<<<<<<<<<<
  *         print("Warning: ANALYSIS segment would be omitted since current implementation does not support parsing of this segment.")
  * 
  */
   }
 
-  /* "ext_modules/io_funcs.pyx":374
+  /* "ext_modules/io_funcs.pyx":378
  *         print("Warning: ANALYSIS segment would be omitted since current implementation does not support parsing of this segment.")
  * 
  *     if "$BEGINSTEXT" in metadata:             # <<<<<<<<<<<<<<
  *         if metadata.pop("$BEGINSTEXT") != "0":
  *             print("Warning: Detected a supplemental TEXT segment. This segment will be ignored under current implementation.")
  */
-  __pyx_t_1 = (__Pyx_PyDict_ContainsTF(__pyx_kp_u_BEGINSTEXT, __pyx_v_metadata, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 374, __pyx_L1_error)
+  __pyx_t_1 = (__Pyx_PyDict_ContainsTF(__pyx_kp_u_BEGINSTEXT, __pyx_v_metadata, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 378, __pyx_L1_error)
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "ext_modules/io_funcs.pyx":375
+    /* "ext_modules/io_funcs.pyx":379
  * 
  *     if "$BEGINSTEXT" in metadata:
  *         if metadata.pop("$BEGINSTEXT") != "0":             # <<<<<<<<<<<<<<
  *             print("Warning: Detected a supplemental TEXT segment. This segment will be ignored under current implementation.")
  *     if "$ENDSTEXT" in metadata:
  */
-    __pyx_t_3 = __Pyx_PyDict_Pop(__pyx_v_metadata, __pyx_kp_u_BEGINSTEXT, ((PyObject *)NULL)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 375, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_Pop(__pyx_v_metadata, __pyx_kp_u_BEGINSTEXT, ((PyObject *)NULL)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 379, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_3, __pyx_kp_u_0, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 375, __pyx_L1_error)
+    __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_3, __pyx_kp_u_0, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 379, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     if (__pyx_t_2) {
 
-      /* "ext_modules/io_funcs.pyx":376
+      /* "ext_modules/io_funcs.pyx":380
  *     if "$BEGINSTEXT" in metadata:
  *         if metadata.pop("$BEGINSTEXT") != "0":
  *             print("Warning: Detected a supplemental TEXT segment. This segment will be ignored under current implementation.")             # <<<<<<<<<<<<<<
  *     if "$ENDSTEXT" in metadata:
  *         del metadata["$ENDSTEXT"]
  */
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_print, __pyx_tuple__49, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 376, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_print, __pyx_tuple__50, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 380, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-      /* "ext_modules/io_funcs.pyx":375
+      /* "ext_modules/io_funcs.pyx":379
  * 
  *     if "$BEGINSTEXT" in metadata:
  *         if metadata.pop("$BEGINSTEXT") != "0":             # <<<<<<<<<<<<<<
  *             print("Warning: Detected a supplemental TEXT segment. This segment will be ignored under current implementation.")
  *     if "$ENDSTEXT" in metadata:
  */
     }
 
-    /* "ext_modules/io_funcs.pyx":374
+    /* "ext_modules/io_funcs.pyx":378
  *         print("Warning: ANALYSIS segment would be omitted since current implementation does not support parsing of this segment.")
  * 
  *     if "$BEGINSTEXT" in metadata:             # <<<<<<<<<<<<<<
  *         if metadata.pop("$BEGINSTEXT") != "0":
  *             print("Warning: Detected a supplemental TEXT segment. This segment will be ignored under current implementation.")
  */
   }
 
-  /* "ext_modules/io_funcs.pyx":377
+  /* "ext_modules/io_funcs.pyx":381
  *         if metadata.pop("$BEGINSTEXT") != "0":
  *             print("Warning: Detected a supplemental TEXT segment. This segment will be ignored under current implementation.")
  *     if "$ENDSTEXT" in metadata:             # <<<<<<<<<<<<<<
  *         del metadata["$ENDSTEXT"]
  * 
  */
-  __pyx_t_2 = (__Pyx_PyDict_ContainsTF(__pyx_kp_u_ENDSTEXT, __pyx_v_metadata, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 377, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PyDict_ContainsTF(__pyx_kp_u_ENDSTEXT, __pyx_v_metadata, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 381, __pyx_L1_error)
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (__pyx_t_1) {
 
-    /* "ext_modules/io_funcs.pyx":378
+    /* "ext_modules/io_funcs.pyx":382
  *             print("Warning: Detected a supplemental TEXT segment. This segment will be ignored under current implementation.")
  *     if "$ENDSTEXT" in metadata:
  *         del metadata["$ENDSTEXT"]             # <<<<<<<<<<<<<<
  * 
  *     # parse data segment
  */
-    if (unlikely(PyDict_DelItem(__pyx_v_metadata, __pyx_kp_u_ENDSTEXT) < 0)) __PYX_ERR(0, 378, __pyx_L1_error)
+    if (unlikely(PyDict_DelItem(__pyx_v_metadata, __pyx_kp_u_ENDSTEXT) < 0)) __PYX_ERR(0, 382, __pyx_L1_error)
 
-    /* "ext_modules/io_funcs.pyx":377
+    /* "ext_modules/io_funcs.pyx":381
  *         if metadata.pop("$BEGINSTEXT") != "0":
  *             print("Warning: Detected a supplemental TEXT segment. This segment will be ignored under current implementation.")
  *     if "$ENDSTEXT" in metadata:             # <<<<<<<<<<<<<<
  *         del metadata["$ENDSTEXT"]
  * 
  */
   }
 
-  /* "ext_modules/io_funcs.pyx":388
+  /* "ext_modules/io_funcs.pyx":392
  *     cdef str keyword, tmpstr
  * 
  *     for keyword in ["$NEXTDATA", "$MODE", "$PAR", "$TOT", "$BYTEORD", "$DATATYPE"]:             # <<<<<<<<<<<<<<
  *         if keyword not in metadata:
  *             fclose(fi)
  */
-  __pyx_t_3 = __pyx_tuple__50; __Pyx_INCREF(__pyx_t_3); __pyx_t_4 = 0;
+  __pyx_t_3 = __pyx_tuple__51; __Pyx_INCREF(__pyx_t_3); __pyx_t_4 = 0;
   for (;;) {
     if (__pyx_t_4 >= 6) break;
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_8 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_8); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 388, __pyx_L1_error)
+    __pyx_t_8 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_8); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 392, __pyx_L1_error)
     #else
-    __pyx_t_8 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 388, __pyx_L1_error)
+    __pyx_t_8 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 392, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     #endif
     __Pyx_XDECREF_SET(__pyx_v_keyword, ((PyObject*)__pyx_t_8));
     __pyx_t_8 = 0;
 
-    /* "ext_modules/io_funcs.pyx":389
+    /* "ext_modules/io_funcs.pyx":393
  * 
  *     for keyword in ["$NEXTDATA", "$MODE", "$PAR", "$TOT", "$BYTEORD", "$DATATYPE"]:
  *         if keyword not in metadata:             # <<<<<<<<<<<<<<
  *             fclose(fi)
  *             raise ValueError(f"Cannot detect requried keyword {keyword} in TEXT segment!")
  */
-    __pyx_t_1 = (__Pyx_PyDict_ContainsTF(__pyx_v_keyword, __pyx_v_metadata, Py_NE)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 389, __pyx_L1_error)
+    __pyx_t_1 = (__Pyx_PyDict_ContainsTF(__pyx_v_keyword, __pyx_v_metadata, Py_NE)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 393, __pyx_L1_error)
     __pyx_t_2 = (__pyx_t_1 != 0);
     if (unlikely(__pyx_t_2)) {
 
-      /* "ext_modules/io_funcs.pyx":390
+      /* "ext_modules/io_funcs.pyx":394
  *     for keyword in ["$NEXTDATA", "$MODE", "$PAR", "$TOT", "$BYTEORD", "$DATATYPE"]:
  *         if keyword not in metadata:
  *             fclose(fi)             # <<<<<<<<<<<<<<
  *             raise ValueError(f"Cannot detect requried keyword {keyword} in TEXT segment!")
  * 
  */
       (void)(fclose(__pyx_v_fi));
 
-      /* "ext_modules/io_funcs.pyx":391
+      /* "ext_modules/io_funcs.pyx":395
  *         if keyword not in metadata:
  *             fclose(fi)
  *             raise ValueError(f"Cannot detect requried keyword {keyword} in TEXT segment!")             # <<<<<<<<<<<<<<
  * 
  *     if metadata.pop("$NEXTDATA") != "0":
  */
-      __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 391, __pyx_L1_error)
+      __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 395, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __pyx_t_18 = 0;
       __pyx_t_5 = 127;
       __Pyx_INCREF(__pyx_kp_u_Cannot_detect_requried_keyword);
       __pyx_t_18 += 31;
       __Pyx_GIVEREF(__pyx_kp_u_Cannot_detect_requried_keyword);
       PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_kp_u_Cannot_detect_requried_keyword);
-      __pyx_t_7 = __Pyx_PyUnicode_Unicode(__pyx_v_keyword); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 391, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyUnicode_Unicode(__pyx_v_keyword); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 395, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) : __pyx_t_5;
       __pyx_t_18 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
       __Pyx_GIVEREF(__pyx_t_7);
       PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_7);
       __pyx_t_7 = 0;
       __Pyx_INCREF(__pyx_kp_u_in_TEXT_segment);
       __pyx_t_18 += 17;
       __Pyx_GIVEREF(__pyx_kp_u_in_TEXT_segment);
       PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_kp_u_in_TEXT_segment);
-      __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_8, 3, __pyx_t_18, __pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 391, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_8, 3, __pyx_t_18, __pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 395, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __pyx_t_8 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 391, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 395, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(0, 391, __pyx_L1_error)
+      __PYX_ERR(0, 395, __pyx_L1_error)
 
-      /* "ext_modules/io_funcs.pyx":389
+      /* "ext_modules/io_funcs.pyx":393
  * 
  *     for keyword in ["$NEXTDATA", "$MODE", "$PAR", "$TOT", "$BYTEORD", "$DATATYPE"]:
  *         if keyword not in metadata:             # <<<<<<<<<<<<<<
  *             fclose(fi)
  *             raise ValueError(f"Cannot detect requried keyword {keyword} in TEXT segment!")
  */
     }
 
-    /* "ext_modules/io_funcs.pyx":388
+    /* "ext_modules/io_funcs.pyx":392
  *     cdef str keyword, tmpstr
  * 
  *     for keyword in ["$NEXTDATA", "$MODE", "$PAR", "$TOT", "$BYTEORD", "$DATATYPE"]:             # <<<<<<<<<<<<<<
  *         if keyword not in metadata:
  *             fclose(fi)
  */
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "ext_modules/io_funcs.pyx":393
+  /* "ext_modules/io_funcs.pyx":397
  *             raise ValueError(f"Cannot detect requried keyword {keyword} in TEXT segment!")
  * 
  *     if metadata.pop("$NEXTDATA") != "0":             # <<<<<<<<<<<<<<
  *         print("Warning: Detected more than one data sets. Current implementation will only parse the first data set.")
  * 
  */
-  __pyx_t_3 = __Pyx_PyDict_Pop(__pyx_v_metadata, __pyx_kp_u_NEXTDATA, ((PyObject *)NULL)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 393, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_Pop(__pyx_v_metadata, __pyx_kp_u_NEXTDATA, ((PyObject *)NULL)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 397, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_3, __pyx_kp_u_0, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 393, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_3, __pyx_kp_u_0, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 397, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_2) {
 
-    /* "ext_modules/io_funcs.pyx":394
+    /* "ext_modules/io_funcs.pyx":398
  * 
  *     if metadata.pop("$NEXTDATA") != "0":
  *         print("Warning: Detected more than one data sets. Current implementation will only parse the first data set.")             # <<<<<<<<<<<<<<
  * 
  *     if metadata.pop("$MODE") != "L":
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_print, __pyx_tuple__51, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 394, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_print, __pyx_tuple__52, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 398, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "ext_modules/io_funcs.pyx":393
+    /* "ext_modules/io_funcs.pyx":397
  *             raise ValueError(f"Cannot detect requried keyword {keyword} in TEXT segment!")
  * 
  *     if metadata.pop("$NEXTDATA") != "0":             # <<<<<<<<<<<<<<
  *         print("Warning: Detected more than one data sets. Current implementation will only parse the first data set.")
  * 
  */
   }
 
-  /* "ext_modules/io_funcs.pyx":396
+  /* "ext_modules/io_funcs.pyx":400
  *         print("Warning: Detected more than one data sets. Current implementation will only parse the first data set.")
  * 
  *     if metadata.pop("$MODE") != "L":             # <<<<<<<<<<<<<<
  *         fclose(fi)
  *         raise NotImplementedError("Current implementation can only handle $MODE = L!")
  */
-  __pyx_t_3 = __Pyx_PyDict_Pop(__pyx_v_metadata, __pyx_kp_u_MODE, ((PyObject *)NULL)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 396, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_Pop(__pyx_v_metadata, __pyx_kp_u_MODE, ((PyObject *)NULL)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_3, __pyx_n_u_L, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 396, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_3, __pyx_n_u_L, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(__pyx_t_2)) {
 
-    /* "ext_modules/io_funcs.pyx":397
+    /* "ext_modules/io_funcs.pyx":401
  * 
  *     if metadata.pop("$MODE") != "L":
  *         fclose(fi)             # <<<<<<<<<<<<<<
  *         raise NotImplementedError("Current implementation can only handle $MODE = L!")
  * 
  */
     (void)(fclose(__pyx_v_fi));
 
-    /* "ext_modules/io_funcs.pyx":398
+    /* "ext_modules/io_funcs.pyx":402
  *     if metadata.pop("$MODE") != "L":
  *         fclose(fi)
  *         raise NotImplementedError("Current implementation can only handle $MODE = L!")             # <<<<<<<<<<<<<<
  * 
  *     endian = "little"
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__52, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 398, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__53, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 402, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 398, __pyx_L1_error)
+    __PYX_ERR(0, 402, __pyx_L1_error)
 
-    /* "ext_modules/io_funcs.pyx":396
+    /* "ext_modules/io_funcs.pyx":400
  *         print("Warning: Detected more than one data sets. Current implementation will only parse the first data set.")
  * 
  *     if metadata.pop("$MODE") != "L":             # <<<<<<<<<<<<<<
  *         fclose(fi)
  *         raise NotImplementedError("Current implementation can only handle $MODE = L!")
  */
   }
 
-  /* "ext_modules/io_funcs.pyx":400
+  /* "ext_modules/io_funcs.pyx":404
  *         raise NotImplementedError("Current implementation can only handle $MODE = L!")
  * 
  *     endian = "little"             # <<<<<<<<<<<<<<
  *     if metadata.pop("$BYTEORD") in ["4,3,2,1", "2,1"]:
  *         endian = "big"
  */
   __Pyx_INCREF(__pyx_n_u_little);
   __pyx_v_endian = __pyx_n_u_little;
 
-  /* "ext_modules/io_funcs.pyx":401
+  /* "ext_modules/io_funcs.pyx":405
  * 
  *     endian = "little"
  *     if metadata.pop("$BYTEORD") in ["4,3,2,1", "2,1"]:             # <<<<<<<<<<<<<<
  *         endian = "big"
  * 
  */
-  __pyx_t_3 = __Pyx_PyDict_Pop(__pyx_v_metadata, __pyx_kp_u_BYTEORD, ((PyObject *)NULL)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 401, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_Pop(__pyx_v_metadata, __pyx_kp_u_BYTEORD, ((PyObject *)NULL)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 405, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_t_3, __pyx_kp_u_4_3_2_1, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 401, __pyx_L1_error)
+  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_t_3, __pyx_kp_u_4_3_2_1, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 405, __pyx_L1_error)
   if (!__pyx_t_1) {
   } else {
     __pyx_t_2 = __pyx_t_1;
     goto __pyx_L54_bool_binop_done;
   }
-  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_t_3, __pyx_kp_u_2_1, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 401, __pyx_L1_error)
+  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_t_3, __pyx_kp_u_2_1, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 405, __pyx_L1_error)
   __pyx_t_2 = __pyx_t_1;
   __pyx_L54_bool_binop_done:;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (__pyx_t_1) {
 
-    /* "ext_modules/io_funcs.pyx":402
+    /* "ext_modules/io_funcs.pyx":406
  *     endian = "little"
  *     if metadata.pop("$BYTEORD") in ["4,3,2,1", "2,1"]:
  *         endian = "big"             # <<<<<<<<<<<<<<
  * 
  *     datatype = ord(metadata.pop("$DATATYPE")[0])
  */
     __Pyx_INCREF(__pyx_n_u_big);
     __Pyx_DECREF_SET(__pyx_v_endian, __pyx_n_u_big);
 
-    /* "ext_modules/io_funcs.pyx":401
+    /* "ext_modules/io_funcs.pyx":405
  * 
  *     endian = "little"
  *     if metadata.pop("$BYTEORD") in ["4,3,2,1", "2,1"]:             # <<<<<<<<<<<<<<
  *         endian = "big"
  * 
  */
   }
 
-  /* "ext_modules/io_funcs.pyx":404
+  /* "ext_modules/io_funcs.pyx":408
  *         endian = "big"
  * 
  *     datatype = ord(metadata.pop("$DATATYPE")[0])             # <<<<<<<<<<<<<<
  *     if datatype != b'I' and datatype != b'F' and datatype != b'D' and datatype != b'A':
  *         fclose(fi)
  */
-  __pyx_t_3 = __Pyx_PyDict_Pop(__pyx_v_metadata, __pyx_kp_u_DATATYPE, ((PyObject *)NULL)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 404, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_Pop(__pyx_v_metadata, __pyx_kp_u_DATATYPE, ((PyObject *)NULL)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 408, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_8 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 404, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 408, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_19 = __Pyx_PyObject_Ord(__pyx_t_8); if (unlikely(__pyx_t_19 == ((long)(long)(Py_UCS4)-1))) __PYX_ERR(0, 404, __pyx_L1_error)
+  __pyx_t_19 = __Pyx_PyObject_Ord(__pyx_t_8); if (unlikely(__pyx_t_19 == ((long)(long)(Py_UCS4)-1))) __PYX_ERR(0, 408, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __pyx_v_datatype = __pyx_t_19;
 
-  /* "ext_modules/io_funcs.pyx":405
+  /* "ext_modules/io_funcs.pyx":409
  * 
  *     datatype = ord(metadata.pop("$DATATYPE")[0])
  *     if datatype != b'I' and datatype != b'F' and datatype != b'D' and datatype != b'A':             # <<<<<<<<<<<<<<
  *         fclose(fi)
  *         raise ValueError(f"$DATATYPE {datatype} does not in 'IFDA'!")
  */
   switch (__pyx_v_datatype) {
@@ -22551,569 +22666,569 @@
     break;
     default:
     __pyx_t_1 = 1;
     break;
   }
   if (unlikely(__pyx_t_1)) {
 
-    /* "ext_modules/io_funcs.pyx":406
+    /* "ext_modules/io_funcs.pyx":410
  *     datatype = ord(metadata.pop("$DATATYPE")[0])
  *     if datatype != b'I' and datatype != b'F' and datatype != b'D' and datatype != b'A':
  *         fclose(fi)             # <<<<<<<<<<<<<<
  *         raise ValueError(f"$DATATYPE {datatype} does not in 'IFDA'!")
  * 
  */
     (void)(fclose(__pyx_v_fi));
 
-    /* "ext_modules/io_funcs.pyx":407
+    /* "ext_modules/io_funcs.pyx":411
  *     if datatype != b'I' and datatype != b'F' and datatype != b'D' and datatype != b'A':
  *         fclose(fi)
  *         raise ValueError(f"$DATATYPE {datatype} does not in 'IFDA'!")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 407, __pyx_L1_error)
+    __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 411, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __pyx_t_4 = 0;
     __pyx_t_5 = 127;
     __Pyx_INCREF(__pyx_kp_u_DATATYPE_2);
     __pyx_t_4 += 10;
     __Pyx_GIVEREF(__pyx_kp_u_DATATYPE_2);
     PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_kp_u_DATATYPE_2);
-    __pyx_t_3 = __Pyx_PyUnicode_From_char(__pyx_v_datatype, 0, ' ', 'd'); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 407, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyUnicode_From_char(__pyx_v_datatype, 0, ' ', 'd'); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 411, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_3);
     __pyx_t_3 = 0;
     __Pyx_INCREF(__pyx_kp_u_does_not_in_IFDA);
     __pyx_t_4 += 20;
     __Pyx_GIVEREF(__pyx_kp_u_does_not_in_IFDA);
     PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_kp_u_does_not_in_IFDA);
-    __pyx_t_3 = __Pyx_PyUnicode_Join(__pyx_t_8, 3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 407, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyUnicode_Join(__pyx_t_8, 3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 411, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_8 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 407, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 411, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_Raise(__pyx_t_8, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __PYX_ERR(0, 407, __pyx_L1_error)
+    __PYX_ERR(0, 411, __pyx_L1_error)
 
-    /* "ext_modules/io_funcs.pyx":405
+    /* "ext_modules/io_funcs.pyx":409
  * 
  *     datatype = ord(metadata.pop("$DATATYPE")[0])
  *     if datatype != b'I' and datatype != b'F' and datatype != b'D' and datatype != b'A':             # <<<<<<<<<<<<<<
  *         fclose(fi)
  *         raise ValueError(f"$DATATYPE {datatype} does not in 'IFDA'!")
  */
   }
 
-  /* "ext_modules/io_funcs.pyx":410
+  /* "ext_modules/io_funcs.pyx":414
  * 
  * 
  *     M = int(metadata.pop("$PAR"))             # <<<<<<<<<<<<<<
  *     N = int(metadata.pop("$TOT"))
  * 
  */
-  __pyx_t_8 = __Pyx_PyDict_Pop(__pyx_v_metadata, __pyx_kp_u_PAR, ((PyObject *)NULL)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 410, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyDict_Pop(__pyx_v_metadata, __pyx_kp_u_PAR, ((PyObject *)NULL)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 414, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_3 = __Pyx_PyNumber_Int(__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 410, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyNumber_Int(__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 414, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_14 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_14 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 410, __pyx_L1_error)
+  __pyx_t_14 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_14 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 414, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_M = __pyx_t_14;
 
-  /* "ext_modules/io_funcs.pyx":411
+  /* "ext_modules/io_funcs.pyx":415
  * 
  *     M = int(metadata.pop("$PAR"))
  *     N = int(metadata.pop("$TOT"))             # <<<<<<<<<<<<<<
  * 
  *     feature_metadata = {"featurekey": np.empty(M, dtype = object), "featureid": np.empty(M, dtype = object)}
  */
-  __pyx_t_3 = __Pyx_PyDict_Pop(__pyx_v_metadata, __pyx_kp_u_TOT, ((PyObject *)NULL)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 411, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_Pop(__pyx_v_metadata, __pyx_kp_u_TOT, ((PyObject *)NULL)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 415, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_8 = __Pyx_PyNumber_Int(__pyx_t_3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 411, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyNumber_Int(__pyx_t_3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 415, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_14 = __Pyx_PyInt_As_int(__pyx_t_8); if (unlikely((__pyx_t_14 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 411, __pyx_L1_error)
+  __pyx_t_14 = __Pyx_PyInt_As_int(__pyx_t_8); if (unlikely((__pyx_t_14 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 415, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __pyx_v_N = __pyx_t_14;
 
-  /* "ext_modules/io_funcs.pyx":413
+  /* "ext_modules/io_funcs.pyx":417
  *     N = int(metadata.pop("$TOT"))
  * 
  *     feature_metadata = {"featurekey": np.empty(M, dtype = object), "featureid": np.empty(M, dtype = object)}             # <<<<<<<<<<<<<<
  * 
  *     cdef str[:] fkview = feature_metadata["featurekey"]
  */
-  __pyx_t_8 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 413, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 417, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 413, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 417, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_empty); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 413, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_empty); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 417, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_M); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 413, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_M); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 417, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_16 = PyTuple_New(1); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 413, __pyx_L1_error)
+  __pyx_t_16 = PyTuple_New(1); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 417, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_16);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_16, 0, __pyx_t_3);
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 413, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 417, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_builtin_object) < 0) __PYX_ERR(0, 413, __pyx_L1_error)
-  __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_16, __pyx_t_3); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 413, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_builtin_object) < 0) __PYX_ERR(0, 417, __pyx_L1_error)
+  __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_16, __pyx_t_3); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 417, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_8, __pyx_n_u_featurekey, __pyx_t_15) < 0) __PYX_ERR(0, 413, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_8, __pyx_n_u_featurekey, __pyx_t_15) < 0) __PYX_ERR(0, 417, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_15, __pyx_n_s_np); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 413, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_15, __pyx_n_s_np); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 417, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 413, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 417, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-  __pyx_t_15 = __Pyx_PyInt_From_int(__pyx_v_M); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 413, __pyx_L1_error)
+  __pyx_t_15 = __Pyx_PyInt_From_int(__pyx_v_M); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 417, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
-  __pyx_t_16 = PyTuple_New(1); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 413, __pyx_L1_error)
+  __pyx_t_16 = PyTuple_New(1); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 417, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_16);
   __Pyx_GIVEREF(__pyx_t_15);
   PyTuple_SET_ITEM(__pyx_t_16, 0, __pyx_t_15);
   __pyx_t_15 = 0;
-  __pyx_t_15 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 413, __pyx_L1_error)
+  __pyx_t_15 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 417, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
-  if (PyDict_SetItem(__pyx_t_15, __pyx_n_s_dtype, __pyx_builtin_object) < 0) __PYX_ERR(0, 413, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_16, __pyx_t_15); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 413, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_15, __pyx_n_s_dtype, __pyx_builtin_object) < 0) __PYX_ERR(0, 417, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_16, __pyx_t_15); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 417, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-  if (PyDict_SetItem(__pyx_t_8, __pyx_n_u_featureid, __pyx_t_7) < 0) __PYX_ERR(0, 413, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_8, __pyx_n_u_featureid, __pyx_t_7) < 0) __PYX_ERR(0, 417, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_v_feature_metadata = ((PyObject*)__pyx_t_8);
   __pyx_t_8 = 0;
 
-  /* "ext_modules/io_funcs.pyx":415
+  /* "ext_modules/io_funcs.pyx":419
  *     feature_metadata = {"featurekey": np.empty(M, dtype = object), "featureid": np.empty(M, dtype = object)}
  * 
  *     cdef str[:] fkview = feature_metadata["featurekey"]             # <<<<<<<<<<<<<<
  *     cdef str[:] fiview = feature_metadata["featureid"]
  * 
  */
-  __pyx_t_8 = __Pyx_PyDict_GetItem(__pyx_v_feature_metadata, __pyx_n_u_featurekey); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 415, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyDict_GetItem(__pyx_v_feature_metadata, __pyx_n_u_featurekey); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 419, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_20 = __Pyx_PyObject_to_MemoryviewSlice_ds_object(__pyx_t_8, PyBUF_WRITABLE); if (unlikely(!__pyx_t_20.memview)) __PYX_ERR(0, 415, __pyx_L1_error)
+  __pyx_t_20 = __Pyx_PyObject_to_MemoryviewSlice_ds_object(__pyx_t_8, PyBUF_WRITABLE); if (unlikely(!__pyx_t_20.memview)) __PYX_ERR(0, 419, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __pyx_v_fkview = __pyx_t_20;
   __pyx_t_20.memview = NULL;
   __pyx_t_20.data = NULL;
 
-  /* "ext_modules/io_funcs.pyx":416
+  /* "ext_modules/io_funcs.pyx":420
  * 
  *     cdef str[:] fkview = feature_metadata["featurekey"]
  *     cdef str[:] fiview = feature_metadata["featureid"]             # <<<<<<<<<<<<<<
  * 
  *     PBs = np.zeros(M, dtype = np.intc)
  */
-  __pyx_t_8 = __Pyx_PyDict_GetItem(__pyx_v_feature_metadata, __pyx_n_u_featureid); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 416, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyDict_GetItem(__pyx_v_feature_metadata, __pyx_n_u_featureid); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 420, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_20 = __Pyx_PyObject_to_MemoryviewSlice_ds_object(__pyx_t_8, PyBUF_WRITABLE); if (unlikely(!__pyx_t_20.memview)) __PYX_ERR(0, 416, __pyx_L1_error)
+  __pyx_t_20 = __Pyx_PyObject_to_MemoryviewSlice_ds_object(__pyx_t_8, PyBUF_WRITABLE); if (unlikely(!__pyx_t_20.memview)) __PYX_ERR(0, 420, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __pyx_v_fiview = __pyx_t_20;
   __pyx_t_20.memview = NULL;
   __pyx_t_20.data = NULL;
 
-  /* "ext_modules/io_funcs.pyx":418
+  /* "ext_modules/io_funcs.pyx":422
  *     cdef str[:] fiview = feature_metadata["featureid"]
  * 
  *     PBs = np.zeros(M, dtype = np.intc)             # <<<<<<<<<<<<<<
  *     PRs = np.zeros(M, dtype = np.intc)
  *     PEs = np.empty(M, dtype = object)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 418, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 422, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_zeros); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 418, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_zeros); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 422, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_M); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 418, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_M); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 422, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_15 = PyTuple_New(1); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 418, __pyx_L1_error)
+  __pyx_t_15 = PyTuple_New(1); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 422, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
   __Pyx_GIVEREF(__pyx_t_8);
   PyTuple_SET_ITEM(__pyx_t_15, 0, __pyx_t_8);
   __pyx_t_8 = 0;
-  __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 418, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 422, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __Pyx_GetModuleGlobalName(__pyx_t_16, __pyx_n_s_np); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 418, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_16, __pyx_n_s_np); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 422, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_16);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_16, __pyx_n_s_intc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 418, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_16, __pyx_n_s_intc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 422, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-  if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 418, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 422, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_15, __pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 418, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_15, __pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 422, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __pyx_v_PBs = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "ext_modules/io_funcs.pyx":419
+  /* "ext_modules/io_funcs.pyx":423
  * 
  *     PBs = np.zeros(M, dtype = np.intc)
  *     PRs = np.zeros(M, dtype = np.intc)             # <<<<<<<<<<<<<<
  *     PEs = np.empty(M, dtype = object)
  *     log_decades = np.zeros(M, dtype = np.float32)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 419, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 423, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 419, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 423, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_M); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 419, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_M); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 423, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_15 = PyTuple_New(1); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 419, __pyx_L1_error)
+  __pyx_t_15 = PyTuple_New(1); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 423, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_15, 0, __pyx_t_3);
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 419, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 423, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 419, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 423, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_intc); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 419, __pyx_L1_error)
+  __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_intc); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 423, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_16);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_16) < 0) __PYX_ERR(0, 419, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_16) < 0) __PYX_ERR(0, 423, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-  __pyx_t_16 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_t_15, __pyx_t_3); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 419, __pyx_L1_error)
+  __pyx_t_16 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_t_15, __pyx_t_3); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 423, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_16);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_PRs = __pyx_t_16;
   __pyx_t_16 = 0;
 
-  /* "ext_modules/io_funcs.pyx":420
+  /* "ext_modules/io_funcs.pyx":424
  *     PBs = np.zeros(M, dtype = np.intc)
  *     PRs = np.zeros(M, dtype = np.intc)
  *     PEs = np.empty(M, dtype = object)             # <<<<<<<<<<<<<<
  *     log_decades = np.zeros(M, dtype = np.float32)
  *     linear_values = np.zeros(M, dtype = np.float32)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_16, __pyx_n_s_np); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 420, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_16, __pyx_n_s_np); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 424, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_16);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_16, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 420, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_16, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 424, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-  __pyx_t_16 = __Pyx_PyInt_From_int(__pyx_v_M); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 420, __pyx_L1_error)
+  __pyx_t_16 = __Pyx_PyInt_From_int(__pyx_v_M); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 424, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_16);
-  __pyx_t_15 = PyTuple_New(1); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 420, __pyx_L1_error)
+  __pyx_t_15 = PyTuple_New(1); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 424, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
   __Pyx_GIVEREF(__pyx_t_16);
   PyTuple_SET_ITEM(__pyx_t_15, 0, __pyx_t_16);
   __pyx_t_16 = 0;
-  __pyx_t_16 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 420, __pyx_L1_error)
+  __pyx_t_16 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 424, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_16);
-  if (PyDict_SetItem(__pyx_t_16, __pyx_n_s_dtype, __pyx_builtin_object) < 0) __PYX_ERR(0, 420, __pyx_L1_error)
-  __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_15, __pyx_t_16); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 420, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_16, __pyx_n_s_dtype, __pyx_builtin_object) < 0) __PYX_ERR(0, 424, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_15, __pyx_t_16); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 424, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
   __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
   __pyx_v_PEs = __pyx_t_8;
   __pyx_t_8 = 0;
 
-  /* "ext_modules/io_funcs.pyx":421
+  /* "ext_modules/io_funcs.pyx":425
  *     PRs = np.zeros(M, dtype = np.intc)
  *     PEs = np.empty(M, dtype = object)
  *     log_decades = np.zeros(M, dtype = np.float32)             # <<<<<<<<<<<<<<
  *     linear_values = np.zeros(M, dtype = np.float32)
  *     bit_masks = np.zeros(M, dtype = np.intc)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 421, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 425, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_zeros); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 421, __pyx_L1_error)
+  __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_zeros); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 425, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_16);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_M); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 421, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_M); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 425, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_15 = PyTuple_New(1); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 421, __pyx_L1_error)
+  __pyx_t_15 = PyTuple_New(1); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 425, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
   __Pyx_GIVEREF(__pyx_t_8);
   PyTuple_SET_ITEM(__pyx_t_15, 0, __pyx_t_8);
   __pyx_t_8 = 0;
-  __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 421, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 425, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 421, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 425, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float32); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 421, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float32); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 425, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 421, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 425, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_16, __pyx_t_15, __pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 421, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_16, __pyx_t_15, __pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 425, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __pyx_v_log_decades = __pyx_t_7;
   __pyx_t_7 = 0;
 
-  /* "ext_modules/io_funcs.pyx":422
+  /* "ext_modules/io_funcs.pyx":426
  *     PEs = np.empty(M, dtype = object)
  *     log_decades = np.zeros(M, dtype = np.float32)
  *     linear_values = np.zeros(M, dtype = np.float32)             # <<<<<<<<<<<<<<
  *     bit_masks = np.zeros(M, dtype = np.intc)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 422, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 426, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_zeros); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 422, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_zeros); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 426, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyInt_From_int(__pyx_v_M); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 422, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_From_int(__pyx_v_M); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 426, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_15 = PyTuple_New(1); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 422, __pyx_L1_error)
+  __pyx_t_15 = PyTuple_New(1); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 426, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
   __Pyx_GIVEREF(__pyx_t_7);
   PyTuple_SET_ITEM(__pyx_t_15, 0, __pyx_t_7);
   __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 422, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 426, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_GetModuleGlobalName(__pyx_t_16, __pyx_n_s_np); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 422, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_16, __pyx_n_s_np); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 426, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_16);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_16, __pyx_n_s_float32); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 422, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_16, __pyx_n_s_float32); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 426, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 422, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 426, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_t_15, __pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 422, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_t_15, __pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 426, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_v_linear_values = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "ext_modules/io_funcs.pyx":423
+  /* "ext_modules/io_funcs.pyx":427
  *     log_decades = np.zeros(M, dtype = np.float32)
  *     linear_values = np.zeros(M, dtype = np.float32)
  *     bit_masks = np.zeros(M, dtype = np.intc)             # <<<<<<<<<<<<<<
  * 
  *     cdef int[:] PBsview = PBs
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 423, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 427, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 423, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 427, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_M); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 423, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_M); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 427, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_15 = PyTuple_New(1); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 423, __pyx_L1_error)
+  __pyx_t_15 = PyTuple_New(1); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 427, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_15, 0, __pyx_t_3);
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 423, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 427, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 423, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 427, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_intc); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 423, __pyx_L1_error)
+  __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_intc); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 427, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_16);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_16) < 0) __PYX_ERR(0, 423, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_16) < 0) __PYX_ERR(0, 427, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-  __pyx_t_16 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_15, __pyx_t_3); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 423, __pyx_L1_error)
+  __pyx_t_16 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_15, __pyx_t_3); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 427, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_16);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_bit_masks = __pyx_t_16;
   __pyx_t_16 = 0;
 
-  /* "ext_modules/io_funcs.pyx":425
+  /* "ext_modules/io_funcs.pyx":429
  *     bit_masks = np.zeros(M, dtype = np.intc)
  * 
  *     cdef int[:] PBsview = PBs             # <<<<<<<<<<<<<<
  *     cdef int[:] PRsview = PRs
  *     cdef str[:] PEsview = PEs
  */
-  __pyx_t_21 = __Pyx_PyObject_to_MemoryviewSlice_ds_int(__pyx_v_PBs, PyBUF_WRITABLE); if (unlikely(!__pyx_t_21.memview)) __PYX_ERR(0, 425, __pyx_L1_error)
+  __pyx_t_21 = __Pyx_PyObject_to_MemoryviewSlice_ds_int(__pyx_v_PBs, PyBUF_WRITABLE); if (unlikely(!__pyx_t_21.memview)) __PYX_ERR(0, 429, __pyx_L1_error)
   __pyx_v_PBsview = __pyx_t_21;
   __pyx_t_21.memview = NULL;
   __pyx_t_21.data = NULL;
 
-  /* "ext_modules/io_funcs.pyx":426
+  /* "ext_modules/io_funcs.pyx":430
  * 
  *     cdef int[:] PBsview = PBs
  *     cdef int[:] PRsview = PRs             # <<<<<<<<<<<<<<
  *     cdef str[:] PEsview = PEs
  *     cdef float[:] ldview = log_decades
  */
-  __pyx_t_21 = __Pyx_PyObject_to_MemoryviewSlice_ds_int(__pyx_v_PRs, PyBUF_WRITABLE); if (unlikely(!__pyx_t_21.memview)) __PYX_ERR(0, 426, __pyx_L1_error)
+  __pyx_t_21 = __Pyx_PyObject_to_MemoryviewSlice_ds_int(__pyx_v_PRs, PyBUF_WRITABLE); if (unlikely(!__pyx_t_21.memview)) __PYX_ERR(0, 430, __pyx_L1_error)
   __pyx_v_PRsview = __pyx_t_21;
   __pyx_t_21.memview = NULL;
   __pyx_t_21.data = NULL;
 
-  /* "ext_modules/io_funcs.pyx":427
+  /* "ext_modules/io_funcs.pyx":431
  *     cdef int[:] PBsview = PBs
  *     cdef int[:] PRsview = PRs
  *     cdef str[:] PEsview = PEs             # <<<<<<<<<<<<<<
  *     cdef float[:] ldview = log_decades
  *     cdef float[:] lvview = linear_values
  */
-  __pyx_t_20 = __Pyx_PyObject_to_MemoryviewSlice_ds_object(__pyx_v_PEs, PyBUF_WRITABLE); if (unlikely(!__pyx_t_20.memview)) __PYX_ERR(0, 427, __pyx_L1_error)
+  __pyx_t_20 = __Pyx_PyObject_to_MemoryviewSlice_ds_object(__pyx_v_PEs, PyBUF_WRITABLE); if (unlikely(!__pyx_t_20.memview)) __PYX_ERR(0, 431, __pyx_L1_error)
   __pyx_v_PEsview = __pyx_t_20;
   __pyx_t_20.memview = NULL;
   __pyx_t_20.data = NULL;
 
-  /* "ext_modules/io_funcs.pyx":428
+  /* "ext_modules/io_funcs.pyx":432
  *     cdef int[:] PRsview = PRs
  *     cdef str[:] PEsview = PEs
  *     cdef float[:] ldview = log_decades             # <<<<<<<<<<<<<<
  *     cdef float[:] lvview = linear_values
  *     cdef int[:] bmview = bit_masks
  */
-  __pyx_t_22 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(__pyx_v_log_decades, PyBUF_WRITABLE); if (unlikely(!__pyx_t_22.memview)) __PYX_ERR(0, 428, __pyx_L1_error)
+  __pyx_t_22 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(__pyx_v_log_decades, PyBUF_WRITABLE); if (unlikely(!__pyx_t_22.memview)) __PYX_ERR(0, 432, __pyx_L1_error)
   __pyx_v_ldview = __pyx_t_22;
   __pyx_t_22.memview = NULL;
   __pyx_t_22.data = NULL;
 
-  /* "ext_modules/io_funcs.pyx":429
+  /* "ext_modules/io_funcs.pyx":433
  *     cdef str[:] PEsview = PEs
  *     cdef float[:] ldview = log_decades
  *     cdef float[:] lvview = linear_values             # <<<<<<<<<<<<<<
  *     cdef int[:] bmview = bit_masks
  * 
  */
-  __pyx_t_22 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(__pyx_v_linear_values, PyBUF_WRITABLE); if (unlikely(!__pyx_t_22.memview)) __PYX_ERR(0, 429, __pyx_L1_error)
+  __pyx_t_22 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(__pyx_v_linear_values, PyBUF_WRITABLE); if (unlikely(!__pyx_t_22.memview)) __PYX_ERR(0, 433, __pyx_L1_error)
   __pyx_v_lvview = __pyx_t_22;
   __pyx_t_22.memview = NULL;
   __pyx_t_22.data = NULL;
 
-  /* "ext_modules/io_funcs.pyx":430
+  /* "ext_modules/io_funcs.pyx":434
  *     cdef float[:] ldview = log_decades
  *     cdef float[:] lvview = linear_values
  *     cdef int[:] bmview = bit_masks             # <<<<<<<<<<<<<<
  * 
  *     cdef str ldstr, lvstr
  */
-  __pyx_t_21 = __Pyx_PyObject_to_MemoryviewSlice_ds_int(__pyx_v_bit_masks, PyBUF_WRITABLE); if (unlikely(!__pyx_t_21.memview)) __PYX_ERR(0, 430, __pyx_L1_error)
+  __pyx_t_21 = __Pyx_PyObject_to_MemoryviewSlice_ds_int(__pyx_v_bit_masks, PyBUF_WRITABLE); if (unlikely(!__pyx_t_21.memview)) __PYX_ERR(0, 434, __pyx_L1_error)
   __pyx_v_bmview = __pyx_t_21;
   __pyx_t_21.memview = NULL;
   __pyx_t_21.data = NULL;
 
-  /* "ext_modules/io_funcs.pyx":433
+  /* "ext_modules/io_funcs.pyx":437
  * 
  *     cdef str ldstr, lvstr
  *     cdef int total_bytes_per_row = 0             # <<<<<<<<<<<<<<
  * 
  *     for i in range(1, M + 1):
  */
   __pyx_v_total_bytes_per_row = 0;
 
-  /* "ext_modules/io_funcs.pyx":435
+  /* "ext_modules/io_funcs.pyx":439
  *     cdef int total_bytes_per_row = 0
  * 
  *     for i in range(1, M + 1):             # <<<<<<<<<<<<<<
  *         for tmpstr in ["B", "E", "N", "R"]:
  *             keyword = f"$P{i}{tmpstr}"
  */
   __pyx_t_19 = (__pyx_v_M + 1);
   __pyx_t_23 = __pyx_t_19;
   for (__pyx_t_4 = 1; __pyx_t_4 < __pyx_t_23; __pyx_t_4+=1) {
     __pyx_v_i = __pyx_t_4;
 
-    /* "ext_modules/io_funcs.pyx":436
+    /* "ext_modules/io_funcs.pyx":440
  * 
  *     for i in range(1, M + 1):
  *         for tmpstr in ["B", "E", "N", "R"]:             # <<<<<<<<<<<<<<
  *             keyword = f"$P{i}{tmpstr}"
  *             if keyword not in metadata:
  */
-    __pyx_t_16 = __pyx_tuple__53; __Pyx_INCREF(__pyx_t_16); __pyx_t_18 = 0;
+    __pyx_t_16 = __pyx_tuple__54; __Pyx_INCREF(__pyx_t_16); __pyx_t_18 = 0;
     for (;;) {
       if (__pyx_t_18 >= 4) break;
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-      __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_16, __pyx_t_18); __Pyx_INCREF(__pyx_t_3); __pyx_t_18++; if (unlikely(0 < 0)) __PYX_ERR(0, 436, __pyx_L1_error)
+      __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_16, __pyx_t_18); __Pyx_INCREF(__pyx_t_3); __pyx_t_18++; if (unlikely(0 < 0)) __PYX_ERR(0, 440, __pyx_L1_error)
       #else
-      __pyx_t_3 = PySequence_ITEM(__pyx_t_16, __pyx_t_18); __pyx_t_18++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 436, __pyx_L1_error)
+      __pyx_t_3 = PySequence_ITEM(__pyx_t_16, __pyx_t_18); __pyx_t_18++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 440, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       #endif
       __Pyx_XDECREF_SET(__pyx_v_tmpstr, ((PyObject*)__pyx_t_3));
       __pyx_t_3 = 0;
 
-      /* "ext_modules/io_funcs.pyx":437
+      /* "ext_modules/io_funcs.pyx":441
  *     for i in range(1, M + 1):
  *         for tmpstr in ["B", "E", "N", "R"]:
  *             keyword = f"$P{i}{tmpstr}"             # <<<<<<<<<<<<<<
  *             if keyword not in metadata:
  *                 fclose(fi)
  */
-      __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 437, __pyx_L1_error)
+      __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 441, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_24 = 0;
       __pyx_t_5 = 127;
       __Pyx_INCREF(__pyx_kp_u_P);
       __pyx_t_24 += 2;
       __Pyx_GIVEREF(__pyx_kp_u_P);
       PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_kp_u_P);
-      __pyx_t_15 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_v_i, 0, ' ', 'd'); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 437, __pyx_L1_error)
+      __pyx_t_15 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_v_i, 0, ' ', 'd'); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 441, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_15);
       __pyx_t_24 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_15);
       __Pyx_GIVEREF(__pyx_t_15);
       PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_15);
       __pyx_t_15 = 0;
-      __pyx_t_15 = __Pyx_PyUnicode_Unicode(__pyx_v_tmpstr); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 437, __pyx_L1_error)
+      __pyx_t_15 = __Pyx_PyUnicode_Unicode(__pyx_v_tmpstr); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 441, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_15);
       __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_15) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_15) : __pyx_t_5;
       __pyx_t_24 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_15);
       __Pyx_GIVEREF(__pyx_t_15);
       PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_t_15);
       __pyx_t_15 = 0;
-      __pyx_t_15 = __Pyx_PyUnicode_Join(__pyx_t_3, 3, __pyx_t_24, __pyx_t_5); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 437, __pyx_L1_error)
+      __pyx_t_15 = __Pyx_PyUnicode_Join(__pyx_t_3, 3, __pyx_t_24, __pyx_t_5); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 441, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_15);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_XDECREF_SET(__pyx_v_keyword, ((PyObject*)__pyx_t_15));
       __pyx_t_15 = 0;
 
-      /* "ext_modules/io_funcs.pyx":438
+      /* "ext_modules/io_funcs.pyx":442
  *         for tmpstr in ["B", "E", "N", "R"]:
  *             keyword = f"$P{i}{tmpstr}"
  *             if keyword not in metadata:             # <<<<<<<<<<<<<<
  *                 fclose(fi)
  *                 raise ValueError(f"Cannot detect requried keyword {keyword} in TEXT segment!")
  */
-      __pyx_t_1 = (__Pyx_PyDict_ContainsTF(__pyx_v_keyword, __pyx_v_metadata, Py_NE)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 438, __pyx_L1_error)
+      __pyx_t_1 = (__Pyx_PyDict_ContainsTF(__pyx_v_keyword, __pyx_v_metadata, Py_NE)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 442, __pyx_L1_error)
       __pyx_t_2 = (__pyx_t_1 != 0);
       if (unlikely(__pyx_t_2)) {
 
-        /* "ext_modules/io_funcs.pyx":439
+        /* "ext_modules/io_funcs.pyx":443
  *             keyword = f"$P{i}{tmpstr}"
  *             if keyword not in metadata:
  *                 fclose(fi)             # <<<<<<<<<<<<<<
  *                 raise ValueError(f"Cannot detect requried keyword {keyword} in TEXT segment!")
  * 
  */
         (void)(fclose(__pyx_v_fi));
 
-        /* "ext_modules/io_funcs.pyx":440
+        /* "ext_modules/io_funcs.pyx":444
  *             if keyword not in metadata:
  *                 fclose(fi)
  *                 raise ValueError(f"Cannot detect requried keyword {keyword} in TEXT segment!")             # <<<<<<<<<<<<<<
  * 
  *         pos = i - 1
  */
-        __pyx_t_15 = PyTuple_New(3); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 440, __pyx_L1_error)
+        __pyx_t_15 = PyTuple_New(3); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 444, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_15);
         __pyx_t_24 = 0;
         __pyx_t_5 = 127;
         __Pyx_INCREF(__pyx_kp_u_Cannot_detect_requried_keyword);
         __pyx_t_24 += 31;
         __Pyx_GIVEREF(__pyx_kp_u_Cannot_detect_requried_keyword);
         PyTuple_SET_ITEM(__pyx_t_15, 0, __pyx_kp_u_Cannot_detect_requried_keyword);
@@ -23122,213 +23237,213 @@
         __pyx_t_24 += __Pyx_PyUnicode_GET_LENGTH(__pyx_v_keyword);
         __Pyx_GIVEREF(__pyx_v_keyword);
         PyTuple_SET_ITEM(__pyx_t_15, 1, __pyx_v_keyword);
         __Pyx_INCREF(__pyx_kp_u_in_TEXT_segment);
         __pyx_t_24 += 17;
         __Pyx_GIVEREF(__pyx_kp_u_in_TEXT_segment);
         PyTuple_SET_ITEM(__pyx_t_15, 2, __pyx_kp_u_in_TEXT_segment);
-        __pyx_t_3 = __Pyx_PyUnicode_Join(__pyx_t_15, 3, __pyx_t_24, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 440, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyUnicode_Join(__pyx_t_15, 3, __pyx_t_24, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 444, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-        __pyx_t_15 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 440, __pyx_L1_error)
+        __pyx_t_15 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 444, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_15);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_Raise(__pyx_t_15, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-        __PYX_ERR(0, 440, __pyx_L1_error)
+        __PYX_ERR(0, 444, __pyx_L1_error)
 
-        /* "ext_modules/io_funcs.pyx":438
+        /* "ext_modules/io_funcs.pyx":442
  *         for tmpstr in ["B", "E", "N", "R"]:
  *             keyword = f"$P{i}{tmpstr}"
  *             if keyword not in metadata:             # <<<<<<<<<<<<<<
  *                 fclose(fi)
  *                 raise ValueError(f"Cannot detect requried keyword {keyword} in TEXT segment!")
  */
       }
 
-      /* "ext_modules/io_funcs.pyx":436
+      /* "ext_modules/io_funcs.pyx":440
  * 
  *     for i in range(1, M + 1):
  *         for tmpstr in ["B", "E", "N", "R"]:             # <<<<<<<<<<<<<<
  *             keyword = f"$P{i}{tmpstr}"
  *             if keyword not in metadata:
  */
     }
     __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
 
-    /* "ext_modules/io_funcs.pyx":442
+    /* "ext_modules/io_funcs.pyx":446
  *                 raise ValueError(f"Cannot detect requried keyword {keyword} in TEXT segment!")
  * 
  *         pos = i - 1             # <<<<<<<<<<<<<<
  *         fiview[pos] = metadata.pop(f"$P{i}N")
  *         fkview[pos] = metadata.pop(f"$P{i}S", fiview[pos])
  */
     __pyx_v_pos = (__pyx_v_i - 1);
 
-    /* "ext_modules/io_funcs.pyx":443
+    /* "ext_modules/io_funcs.pyx":447
  * 
  *         pos = i - 1
  *         fiview[pos] = metadata.pop(f"$P{i}N")             # <<<<<<<<<<<<<<
  *         fkview[pos] = metadata.pop(f"$P{i}S", fiview[pos])
  *         PEsview[pos] = metadata.pop(f"$P{i}E")
  */
-    __pyx_t_16 = PyTuple_New(3); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 443, __pyx_L1_error)
+    __pyx_t_16 = PyTuple_New(3); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 447, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_16);
     __pyx_t_18 = 0;
     __pyx_t_5 = 127;
     __Pyx_INCREF(__pyx_kp_u_P);
     __pyx_t_18 += 2;
     __Pyx_GIVEREF(__pyx_kp_u_P);
     PyTuple_SET_ITEM(__pyx_t_16, 0, __pyx_kp_u_P);
-    __pyx_t_15 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_v_i, 0, ' ', 'd'); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 443, __pyx_L1_error)
+    __pyx_t_15 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_v_i, 0, ' ', 'd'); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 447, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_15);
     __pyx_t_18 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_15);
     __Pyx_GIVEREF(__pyx_t_15);
     PyTuple_SET_ITEM(__pyx_t_16, 1, __pyx_t_15);
     __pyx_t_15 = 0;
     __Pyx_INCREF(__pyx_n_u_N);
     __pyx_t_18 += 1;
     __Pyx_GIVEREF(__pyx_n_u_N);
     PyTuple_SET_ITEM(__pyx_t_16, 2, __pyx_n_u_N);
-    __pyx_t_15 = __Pyx_PyUnicode_Join(__pyx_t_16, 3, __pyx_t_18, __pyx_t_5); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 443, __pyx_L1_error)
+    __pyx_t_15 = __Pyx_PyUnicode_Join(__pyx_t_16, 3, __pyx_t_18, __pyx_t_5); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 447, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_15);
     __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-    __pyx_t_16 = __Pyx_PyDict_Pop(__pyx_v_metadata, __pyx_t_15, ((PyObject *)NULL)); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 443, __pyx_L1_error)
+    __pyx_t_16 = __Pyx_PyDict_Pop(__pyx_v_metadata, __pyx_t_15, ((PyObject *)NULL)); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 447, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_16);
     __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-    if (!(likely(PyUnicode_CheckExact(__pyx_t_16))||((__pyx_t_16) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_16)->tp_name), 0))) __PYX_ERR(0, 443, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(__pyx_t_16))||((__pyx_t_16) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_16)->tp_name), 0))) __PYX_ERR(0, 447, __pyx_L1_error)
     __pyx_t_17 = __pyx_v_pos;
     __pyx_t_25 = ((PyObject * *) ( /* dim=0 */ (__pyx_v_fiview.data + __pyx_t_17 * __pyx_v_fiview.strides[0]) ));
     __Pyx_XGOTREF(*__pyx_t_25);
     __Pyx_INCREF(__pyx_t_16); __Pyx_XDECREF(*__pyx_t_25);
     *__pyx_t_25 = __pyx_t_16;
     __Pyx_XGIVEREF(*__pyx_t_25);
     __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
 
-    /* "ext_modules/io_funcs.pyx":444
+    /* "ext_modules/io_funcs.pyx":448
  *         pos = i - 1
  *         fiview[pos] = metadata.pop(f"$P{i}N")
  *         fkview[pos] = metadata.pop(f"$P{i}S", fiview[pos])             # <<<<<<<<<<<<<<
  *         PEsview[pos] = metadata.pop(f"$P{i}E")
  * 
  */
-    __pyx_t_16 = PyTuple_New(3); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 444, __pyx_L1_error)
+    __pyx_t_16 = PyTuple_New(3); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 448, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_16);
     __pyx_t_18 = 0;
     __pyx_t_5 = 127;
     __Pyx_INCREF(__pyx_kp_u_P);
     __pyx_t_18 += 2;
     __Pyx_GIVEREF(__pyx_kp_u_P);
     PyTuple_SET_ITEM(__pyx_t_16, 0, __pyx_kp_u_P);
-    __pyx_t_15 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_v_i, 0, ' ', 'd'); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 444, __pyx_L1_error)
+    __pyx_t_15 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_v_i, 0, ' ', 'd'); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 448, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_15);
     __pyx_t_18 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_15);
     __Pyx_GIVEREF(__pyx_t_15);
     PyTuple_SET_ITEM(__pyx_t_16, 1, __pyx_t_15);
     __pyx_t_15 = 0;
     __Pyx_INCREF(__pyx_n_u_S);
     __pyx_t_18 += 1;
     __Pyx_GIVEREF(__pyx_n_u_S);
     PyTuple_SET_ITEM(__pyx_t_16, 2, __pyx_n_u_S);
-    __pyx_t_15 = __Pyx_PyUnicode_Join(__pyx_t_16, 3, __pyx_t_18, __pyx_t_5); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 444, __pyx_L1_error)
+    __pyx_t_15 = __Pyx_PyUnicode_Join(__pyx_t_16, 3, __pyx_t_18, __pyx_t_5); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 448, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_15);
     __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
     __pyx_t_17 = __pyx_v_pos;
     __pyx_t_16 = (PyObject *) *((PyObject * *) ( /* dim=0 */ (__pyx_v_fiview.data + __pyx_t_17 * __pyx_v_fiview.strides[0]) ));
     if (unlikely(__pyx_t_16 == NULL)) __pyx_t_16 = Py_None;
     __Pyx_INCREF((PyObject*)__pyx_t_16);
-    __pyx_t_3 = __Pyx_PyDict_Pop(__pyx_v_metadata, __pyx_t_15, __pyx_t_16); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 444, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_Pop(__pyx_v_metadata, __pyx_t_15, __pyx_t_16); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 448, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
     __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-    if (!(likely(PyUnicode_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(0, 444, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(0, 448, __pyx_L1_error)
     __pyx_t_17 = __pyx_v_pos;
     __pyx_t_25 = ((PyObject * *) ( /* dim=0 */ (__pyx_v_fkview.data + __pyx_t_17 * __pyx_v_fkview.strides[0]) ));
     __Pyx_XGOTREF(*__pyx_t_25);
     __Pyx_INCREF(__pyx_t_3); __Pyx_XDECREF(*__pyx_t_25);
     *__pyx_t_25 = __pyx_t_3;
     __Pyx_XGIVEREF(*__pyx_t_25);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "ext_modules/io_funcs.pyx":445
+    /* "ext_modules/io_funcs.pyx":449
  *         fiview[pos] = metadata.pop(f"$P{i}N")
  *         fkview[pos] = metadata.pop(f"$P{i}S", fiview[pos])
  *         PEsview[pos] = metadata.pop(f"$P{i}E")             # <<<<<<<<<<<<<<
  * 
  *         tmpstr = metadata.pop(f"$P{i}R")
  */
-    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 445, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 449, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_18 = 0;
     __pyx_t_5 = 127;
     __Pyx_INCREF(__pyx_kp_u_P);
     __pyx_t_18 += 2;
     __Pyx_GIVEREF(__pyx_kp_u_P);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_kp_u_P);
-    __pyx_t_16 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_v_i, 0, ' ', 'd'); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 445, __pyx_L1_error)
+    __pyx_t_16 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_v_i, 0, ' ', 'd'); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 449, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_16);
     __pyx_t_18 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_16);
     __Pyx_GIVEREF(__pyx_t_16);
     PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_16);
     __pyx_t_16 = 0;
     __Pyx_INCREF(__pyx_n_u_E);
     __pyx_t_18 += 1;
     __Pyx_GIVEREF(__pyx_n_u_E);
     PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_n_u_E);
-    __pyx_t_16 = __Pyx_PyUnicode_Join(__pyx_t_3, 3, __pyx_t_18, __pyx_t_5); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 445, __pyx_L1_error)
+    __pyx_t_16 = __Pyx_PyUnicode_Join(__pyx_t_3, 3, __pyx_t_18, __pyx_t_5); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 449, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_16);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyDict_Pop(__pyx_v_metadata, __pyx_t_16, ((PyObject *)NULL)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 445, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_Pop(__pyx_v_metadata, __pyx_t_16, ((PyObject *)NULL)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 449, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-    if (!(likely(PyUnicode_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(0, 445, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(0, 449, __pyx_L1_error)
     __pyx_t_17 = __pyx_v_pos;
     __pyx_t_25 = ((PyObject * *) ( /* dim=0 */ (__pyx_v_PEsview.data + __pyx_t_17 * __pyx_v_PEsview.strides[0]) ));
     __Pyx_XGOTREF(*__pyx_t_25);
     __Pyx_INCREF(__pyx_t_3); __Pyx_XDECREF(*__pyx_t_25);
     *__pyx_t_25 = __pyx_t_3;
     __Pyx_XGIVEREF(*__pyx_t_25);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "ext_modules/io_funcs.pyx":447
+    /* "ext_modules/io_funcs.pyx":451
  *         PEsview[pos] = metadata.pop(f"$P{i}E")
  * 
  *         tmpstr = metadata.pop(f"$P{i}R")             # <<<<<<<<<<<<<<
  *         try:
  *             PRsview[pos] = int(tmpstr)
  */
-    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 447, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 451, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_18 = 0;
     __pyx_t_5 = 127;
     __Pyx_INCREF(__pyx_kp_u_P);
     __pyx_t_18 += 2;
     __Pyx_GIVEREF(__pyx_kp_u_P);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_kp_u_P);
-    __pyx_t_16 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_v_i, 0, ' ', 'd'); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 447, __pyx_L1_error)
+    __pyx_t_16 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_v_i, 0, ' ', 'd'); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 451, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_16);
     __pyx_t_18 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_16);
     __Pyx_GIVEREF(__pyx_t_16);
     PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_16);
     __pyx_t_16 = 0;
     __Pyx_INCREF(__pyx_n_u_R);
     __pyx_t_18 += 1;
     __Pyx_GIVEREF(__pyx_n_u_R);
     PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_n_u_R);
-    __pyx_t_16 = __Pyx_PyUnicode_Join(__pyx_t_3, 3, __pyx_t_18, __pyx_t_5); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 447, __pyx_L1_error)
+    __pyx_t_16 = __Pyx_PyUnicode_Join(__pyx_t_3, 3, __pyx_t_18, __pyx_t_5); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 451, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_16);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyDict_Pop(__pyx_v_metadata, __pyx_t_16, ((PyObject *)NULL)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 447, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_Pop(__pyx_v_metadata, __pyx_t_16, ((PyObject *)NULL)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 451, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-    if (!(likely(PyUnicode_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(0, 447, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(0, 451, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_tmpstr, ((PyObject*)__pyx_t_3));
     __pyx_t_3 = 0;
 
-    /* "ext_modules/io_funcs.pyx":448
+    /* "ext_modules/io_funcs.pyx":452
  * 
  *         tmpstr = metadata.pop(f"$P{i}R")
  *         try:             # <<<<<<<<<<<<<<
  *             PRsview[pos] = int(tmpstr)
  *         except ValueError:
  */
     {
@@ -23336,29 +23451,29 @@
       __Pyx_PyThreadState_assign
       __Pyx_ExceptionSave(&__pyx_t_13, &__pyx_t_12, &__pyx_t_11);
       __Pyx_XGOTREF(__pyx_t_13);
       __Pyx_XGOTREF(__pyx_t_12);
       __Pyx_XGOTREF(__pyx_t_11);
       /*try:*/ {
 
-        /* "ext_modules/io_funcs.pyx":449
+        /* "ext_modules/io_funcs.pyx":453
  *         tmpstr = metadata.pop(f"$P{i}R")
  *         try:
  *             PRsview[pos] = int(tmpstr)             # <<<<<<<<<<<<<<
  *         except ValueError:
  *             PRsview[pos] = int(float(tmpstr))
  */
-        __pyx_t_3 = __Pyx_PyNumber_Int(__pyx_v_tmpstr); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 449, __pyx_L62_error)
+        __pyx_t_3 = __Pyx_PyNumber_Int(__pyx_v_tmpstr); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 453, __pyx_L62_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_14 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_14 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 449, __pyx_L62_error)
+        __pyx_t_14 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_14 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 453, __pyx_L62_error)
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_t_17 = __pyx_v_pos;
         *((int *) ( /* dim=0 */ (__pyx_v_PRsview.data + __pyx_t_17 * __pyx_v_PRsview.strides[0]) )) = __pyx_t_14;
 
-        /* "ext_modules/io_funcs.pyx":448
+        /* "ext_modules/io_funcs.pyx":452
  * 
  *         tmpstr = metadata.pop(f"$P{i}R")
  *         try:             # <<<<<<<<<<<<<<
  *             PRsview[pos] = int(tmpstr)
  *         except ValueError:
  */
       }
@@ -23374,109 +23489,109 @@
       __PYX_XDEC_MEMVIEW(&__pyx_t_22, 1);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_XDEC_MEMVIEW(&__pyx_t_9, 1);
 
-      /* "ext_modules/io_funcs.pyx":450
+      /* "ext_modules/io_funcs.pyx":454
  *         try:
  *             PRsview[pos] = int(tmpstr)
  *         except ValueError:             # <<<<<<<<<<<<<<
  *             PRsview[pos] = int(float(tmpstr))
  *             print(f"Warning: $P{i}R should be an integer! Rounded {tmpstr} to {PRsview[pos]}.")
  */
       __pyx_t_14 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_ValueError);
       if (__pyx_t_14) {
         __Pyx_AddTraceback("pegasusio.cylib.io.read_fcs", __pyx_clineno, __pyx_lineno, __pyx_filename);
-        if (__Pyx_GetException(&__pyx_t_3, &__pyx_t_16, &__pyx_t_15) < 0) __PYX_ERR(0, 450, __pyx_L64_except_error)
+        if (__Pyx_GetException(&__pyx_t_3, &__pyx_t_16, &__pyx_t_15) < 0) __PYX_ERR(0, 454, __pyx_L64_except_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_GOTREF(__pyx_t_16);
         __Pyx_GOTREF(__pyx_t_15);
 
-        /* "ext_modules/io_funcs.pyx":451
+        /* "ext_modules/io_funcs.pyx":455
  *             PRsview[pos] = int(tmpstr)
  *         except ValueError:
  *             PRsview[pos] = int(float(tmpstr))             # <<<<<<<<<<<<<<
  *             print(f"Warning: $P{i}R should be an integer! Rounded {tmpstr} to {PRsview[pos]}.")
  * 
  */
-        __pyx_t_7 = __Pyx_PyNumber_Float(__pyx_v_tmpstr); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 451, __pyx_L64_except_error)
+        __pyx_t_7 = __Pyx_PyNumber_Float(__pyx_v_tmpstr); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 455, __pyx_L64_except_error)
         __Pyx_GOTREF(__pyx_t_7);
-        __pyx_t_8 = __Pyx_PyNumber_Int(__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 451, __pyx_L64_except_error)
+        __pyx_t_8 = __Pyx_PyNumber_Int(__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 455, __pyx_L64_except_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-        __pyx_t_14 = __Pyx_PyInt_As_int(__pyx_t_8); if (unlikely((__pyx_t_14 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 451, __pyx_L64_except_error)
+        __pyx_t_14 = __Pyx_PyInt_As_int(__pyx_t_8); if (unlikely((__pyx_t_14 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 455, __pyx_L64_except_error)
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         __pyx_t_17 = __pyx_v_pos;
         *((int *) ( /* dim=0 */ (__pyx_v_PRsview.data + __pyx_t_17 * __pyx_v_PRsview.strides[0]) )) = __pyx_t_14;
 
-        /* "ext_modules/io_funcs.pyx":452
+        /* "ext_modules/io_funcs.pyx":456
  *         except ValueError:
  *             PRsview[pos] = int(float(tmpstr))
  *             print(f"Warning: $P{i}R should be an integer! Rounded {tmpstr} to {PRsview[pos]}.")             # <<<<<<<<<<<<<<
  * 
  *         ldstr, lvstr = PEsview[pos].split(",")
  */
-        __pyx_t_8 = PyTuple_New(7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 452, __pyx_L64_except_error)
+        __pyx_t_8 = PyTuple_New(7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 456, __pyx_L64_except_error)
         __Pyx_GOTREF(__pyx_t_8);
         __pyx_t_18 = 0;
         __pyx_t_5 = 127;
         __Pyx_INCREF(__pyx_kp_u_Warning_P);
         __pyx_t_18 += 11;
         __Pyx_GIVEREF(__pyx_kp_u_Warning_P);
         PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_kp_u_Warning_P);
-        __pyx_t_7 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_v_i, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 452, __pyx_L64_except_error)
+        __pyx_t_7 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_v_i, 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 456, __pyx_L64_except_error)
         __Pyx_GOTREF(__pyx_t_7);
         __pyx_t_18 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
         __Pyx_GIVEREF(__pyx_t_7);
         PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_7);
         __pyx_t_7 = 0;
         __Pyx_INCREF(__pyx_kp_u_R_should_be_an_integer_Rounded);
         __pyx_t_18 += 32;
         __Pyx_GIVEREF(__pyx_kp_u_R_should_be_an_integer_Rounded);
         PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_kp_u_R_should_be_an_integer_Rounded);
-        __pyx_t_7 = __Pyx_PyUnicode_Unicode(__pyx_v_tmpstr); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 452, __pyx_L64_except_error)
+        __pyx_t_7 = __Pyx_PyUnicode_Unicode(__pyx_v_tmpstr); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 456, __pyx_L64_except_error)
         __Pyx_GOTREF(__pyx_t_7);
         __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) : __pyx_t_5;
         __pyx_t_18 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
         __Pyx_GIVEREF(__pyx_t_7);
         PyTuple_SET_ITEM(__pyx_t_8, 3, __pyx_t_7);
         __pyx_t_7 = 0;
         __Pyx_INCREF(__pyx_kp_u_to);
         __pyx_t_18 += 4;
         __Pyx_GIVEREF(__pyx_kp_u_to);
         PyTuple_SET_ITEM(__pyx_t_8, 4, __pyx_kp_u_to);
         __pyx_t_17 = __pyx_v_pos;
-        __pyx_t_7 = __Pyx_PyUnicode_From_int((*((int *) ( /* dim=0 */ (__pyx_v_PRsview.data + __pyx_t_17 * __pyx_v_PRsview.strides[0]) ))), 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 452, __pyx_L64_except_error)
+        __pyx_t_7 = __Pyx_PyUnicode_From_int((*((int *) ( /* dim=0 */ (__pyx_v_PRsview.data + __pyx_t_17 * __pyx_v_PRsview.strides[0]) ))), 0, ' ', 'd'); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 456, __pyx_L64_except_error)
         __Pyx_GOTREF(__pyx_t_7);
         __pyx_t_18 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
         __Pyx_GIVEREF(__pyx_t_7);
         PyTuple_SET_ITEM(__pyx_t_8, 5, __pyx_t_7);
         __pyx_t_7 = 0;
-        __Pyx_INCREF(__pyx_kp_u__54);
+        __Pyx_INCREF(__pyx_kp_u__55);
         __pyx_t_18 += 1;
-        __Pyx_GIVEREF(__pyx_kp_u__54);
-        PyTuple_SET_ITEM(__pyx_t_8, 6, __pyx_kp_u__54);
-        __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_8, 7, __pyx_t_18, __pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 452, __pyx_L64_except_error)
+        __Pyx_GIVEREF(__pyx_kp_u__55);
+        PyTuple_SET_ITEM(__pyx_t_8, 6, __pyx_kp_u__55);
+        __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_8, 7, __pyx_t_18, __pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 456, __pyx_L64_except_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-        __pyx_t_8 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 452, __pyx_L64_except_error)
+        __pyx_t_8 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 456, __pyx_L64_except_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_XDECREF(__pyx_t_16); __pyx_t_16 = 0;
         __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
         goto __pyx_L63_exception_handled;
       }
       goto __pyx_L64_except_error;
       __pyx_L64_except_error:;
 
-      /* "ext_modules/io_funcs.pyx":448
+      /* "ext_modules/io_funcs.pyx":452
  * 
  *         tmpstr = metadata.pop(f"$P{i}R")
  *         try:             # <<<<<<<<<<<<<<
  *             PRsview[pos] = int(tmpstr)
  *         except ValueError:
  */
       __Pyx_XGIVEREF(__pyx_t_13);
@@ -23488,83 +23603,83 @@
       __Pyx_XGIVEREF(__pyx_t_13);
       __Pyx_XGIVEREF(__pyx_t_12);
       __Pyx_XGIVEREF(__pyx_t_11);
       __Pyx_ExceptionReset(__pyx_t_13, __pyx_t_12, __pyx_t_11);
       __pyx_L69_try_end:;
     }
 
-    /* "ext_modules/io_funcs.pyx":454
+    /* "ext_modules/io_funcs.pyx":458
  *             print(f"Warning: $P{i}R should be an integer! Rounded {tmpstr} to {PRsview[pos]}.")
  * 
  *         ldstr, lvstr = PEsview[pos].split(",")             # <<<<<<<<<<<<<<
  *         ldview[pos] = float(ldstr)
  *         lvview[pos] = float(lvstr)
  */
     __pyx_t_17 = __pyx_v_pos;
     __pyx_t_15 = (PyObject *) *((PyObject * *) ( /* dim=0 */ (__pyx_v_PEsview.data + __pyx_t_17 * __pyx_v_PEsview.strides[0]) ));
     if (unlikely(__pyx_t_15 == NULL)) __pyx_t_15 = Py_None;
     __Pyx_INCREF((PyObject*)__pyx_t_15);
     if (unlikely(__pyx_t_15 == Py_None)) {
       PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "split");
-      __PYX_ERR(0, 454, __pyx_L1_error)
+      __PYX_ERR(0, 458, __pyx_L1_error)
     }
-    __pyx_t_16 = PyUnicode_Split(__pyx_t_15, __pyx_kp_u__55, -1L); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 454, __pyx_L1_error)
+    __pyx_t_16 = PyUnicode_Split(__pyx_t_15, __pyx_kp_u__56, -1L); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 458, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_16);
     __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
     if (1) {
       PyObject* sequence = __pyx_t_16;
       Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
       if (unlikely(size != 2)) {
         if (size > 2) __Pyx_RaiseTooManyValuesError(2);
         else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(0, 454, __pyx_L1_error)
+        __PYX_ERR(0, 458, __pyx_L1_error)
       }
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
       __pyx_t_15 = PyList_GET_ITEM(sequence, 0); 
       __pyx_t_3 = PyList_GET_ITEM(sequence, 1); 
       __Pyx_INCREF(__pyx_t_15);
       __Pyx_INCREF(__pyx_t_3);
       #else
-      __pyx_t_15 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 454, __pyx_L1_error)
+      __pyx_t_15 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 458, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_15);
-      __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 454, __pyx_L1_error)
+      __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 458, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       #endif
       __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
     }
-    if (!(likely(PyUnicode_CheckExact(__pyx_t_15))||((__pyx_t_15) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_15)->tp_name), 0))) __PYX_ERR(0, 454, __pyx_L1_error)
-    if (!(likely(PyUnicode_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(0, 454, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(__pyx_t_15))||((__pyx_t_15) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_15)->tp_name), 0))) __PYX_ERR(0, 458, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(0, 458, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_ldstr, ((PyObject*)__pyx_t_15));
     __pyx_t_15 = 0;
     __Pyx_XDECREF_SET(__pyx_v_lvstr, ((PyObject*)__pyx_t_3));
     __pyx_t_3 = 0;
 
-    /* "ext_modules/io_funcs.pyx":455
+    /* "ext_modules/io_funcs.pyx":459
  * 
  *         ldstr, lvstr = PEsview[pos].split(",")
  *         ldview[pos] = float(ldstr)             # <<<<<<<<<<<<<<
  *         lvview[pos] = float(lvstr)
  *         assert ldview[pos] >= 0.0 and lvview[pos] >= 0.0
  */
-    __pyx_t_26 = __Pyx_PyObject_AsDouble(__pyx_v_ldstr); if (unlikely(__pyx_t_26 == ((double)((double)-1)) && PyErr_Occurred())) __PYX_ERR(0, 455, __pyx_L1_error)
+    __pyx_t_26 = __Pyx_PyObject_AsDouble(__pyx_v_ldstr); if (unlikely(__pyx_t_26 == ((double)((double)-1)) && PyErr_Occurred())) __PYX_ERR(0, 459, __pyx_L1_error)
     __pyx_t_17 = __pyx_v_pos;
     *((float *) ( /* dim=0 */ (__pyx_v_ldview.data + __pyx_t_17 * __pyx_v_ldview.strides[0]) )) = __pyx_t_26;
 
-    /* "ext_modules/io_funcs.pyx":456
+    /* "ext_modules/io_funcs.pyx":460
  *         ldstr, lvstr = PEsview[pos].split(",")
  *         ldview[pos] = float(ldstr)
  *         lvview[pos] = float(lvstr)             # <<<<<<<<<<<<<<
  *         assert ldview[pos] >= 0.0 and lvview[pos] >= 0.0
  * 
  */
-    __pyx_t_26 = __Pyx_PyObject_AsDouble(__pyx_v_lvstr); if (unlikely(__pyx_t_26 == ((double)((double)-1)) && PyErr_Occurred())) __PYX_ERR(0, 456, __pyx_L1_error)
+    __pyx_t_26 = __Pyx_PyObject_AsDouble(__pyx_v_lvstr); if (unlikely(__pyx_t_26 == ((double)((double)-1)) && PyErr_Occurred())) __PYX_ERR(0, 460, __pyx_L1_error)
     __pyx_t_17 = __pyx_v_pos;
     *((float *) ( /* dim=0 */ (__pyx_v_lvview.data + __pyx_t_17 * __pyx_v_lvview.strides[0]) )) = __pyx_t_26;
 
-    /* "ext_modules/io_funcs.pyx":457
+    /* "ext_modules/io_funcs.pyx":461
  *         ldview[pos] = float(ldstr)
  *         lvview[pos] = float(lvstr)
  *         assert ldview[pos] >= 0.0 and lvview[pos] >= 0.0             # <<<<<<<<<<<<<<
  * 
  *         keyword = f"$P{i}B"
  */
     #ifndef CYTHON_WITHOUT_ASSERTIONS
@@ -23578,243 +23693,243 @@
       }
       __pyx_t_17 = __pyx_v_pos;
       __pyx_t_1 = (((*((float *) ( /* dim=0 */ (__pyx_v_lvview.data + __pyx_t_17 * __pyx_v_lvview.strides[0]) ))) >= 0.0) != 0);
       __pyx_t_2 = __pyx_t_1;
       __pyx_L72_bool_binop_done:;
       if (unlikely(!__pyx_t_2)) {
         PyErr_SetNone(PyExc_AssertionError);
-        __PYX_ERR(0, 457, __pyx_L1_error)
+        __PYX_ERR(0, 461, __pyx_L1_error)
       }
     }
     #endif
 
-    /* "ext_modules/io_funcs.pyx":459
+    /* "ext_modules/io_funcs.pyx":463
  *         assert ldview[pos] >= 0.0 and lvview[pos] >= 0.0
  * 
  *         keyword = f"$P{i}B"             # <<<<<<<<<<<<<<
  * 
  *         if metadata[keyword] == "*":
  */
-    __pyx_t_16 = PyTuple_New(3); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 459, __pyx_L1_error)
+    __pyx_t_16 = PyTuple_New(3); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 463, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_16);
     __pyx_t_18 = 0;
     __pyx_t_5 = 127;
     __Pyx_INCREF(__pyx_kp_u_P);
     __pyx_t_18 += 2;
     __Pyx_GIVEREF(__pyx_kp_u_P);
     PyTuple_SET_ITEM(__pyx_t_16, 0, __pyx_kp_u_P);
-    __pyx_t_3 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_v_i, 0, ' ', 'd'); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 459, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_v_i, 0, ' ', 'd'); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 463, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_18 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_16, 1, __pyx_t_3);
     __pyx_t_3 = 0;
     __Pyx_INCREF(__pyx_n_u_B);
     __pyx_t_18 += 1;
     __Pyx_GIVEREF(__pyx_n_u_B);
     PyTuple_SET_ITEM(__pyx_t_16, 2, __pyx_n_u_B);
-    __pyx_t_3 = __Pyx_PyUnicode_Join(__pyx_t_16, 3, __pyx_t_18, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 459, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyUnicode_Join(__pyx_t_16, 3, __pyx_t_18, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 463, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
     __Pyx_XDECREF_SET(__pyx_v_keyword, ((PyObject*)__pyx_t_3));
     __pyx_t_3 = 0;
 
-    /* "ext_modules/io_funcs.pyx":461
+    /* "ext_modules/io_funcs.pyx":465
  *         keyword = f"$P{i}B"
  * 
  *         if metadata[keyword] == "*":             # <<<<<<<<<<<<<<
  *             fclose(fi)
  *             if datatype == b'A':
  */
-    __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_metadata, __pyx_v_keyword); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 461, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_metadata, __pyx_v_keyword); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 465, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_3, __pyx_kp_u__56, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 461, __pyx_L1_error)
+    __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_3, __pyx_kp_u__57, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 465, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     if (__pyx_t_2) {
 
-      /* "ext_modules/io_funcs.pyx":462
+      /* "ext_modules/io_funcs.pyx":466
  * 
  *         if metadata[keyword] == "*":
  *             fclose(fi)             # <<<<<<<<<<<<<<
  *             if datatype == b'A':
  *                 raise NotImplementedError(f"Current implementation does not support {keyword} = *!")
  */
       (void)(fclose(__pyx_v_fi));
 
-      /* "ext_modules/io_funcs.pyx":463
+      /* "ext_modules/io_funcs.pyx":467
  *         if metadata[keyword] == "*":
  *             fclose(fi)
  *             if datatype == b'A':             # <<<<<<<<<<<<<<
  *                 raise NotImplementedError(f"Current implementation does not support {keyword} = *!")
  *             else:
  */
       __pyx_t_2 = ((__pyx_v_datatype == 'A') != 0);
       if (unlikely(__pyx_t_2)) {
 
-        /* "ext_modules/io_funcs.pyx":464
+        /* "ext_modules/io_funcs.pyx":468
  *             fclose(fi)
  *             if datatype == b'A':
  *                 raise NotImplementedError(f"Current implementation does not support {keyword} = *!")             # <<<<<<<<<<<<<<
  *             else:
  *                 raise ValueError(f"$DATATYPE '{datatype}' should have {keyword} = *!")
  */
-        __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 464, __pyx_L1_error)
+        __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 468, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __pyx_t_18 = 0;
         __pyx_t_5 = 127;
         __Pyx_INCREF(__pyx_kp_u_Current_implementation_does_not);
         __pyx_t_18 += 40;
         __Pyx_GIVEREF(__pyx_kp_u_Current_implementation_does_not);
         PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_kp_u_Current_implementation_does_not);
         __Pyx_INCREF(__pyx_v_keyword);
         __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_v_keyword) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_v_keyword) : __pyx_t_5;
         __pyx_t_18 += __Pyx_PyUnicode_GET_LENGTH(__pyx_v_keyword);
         __Pyx_GIVEREF(__pyx_v_keyword);
         PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_keyword);
-        __Pyx_INCREF(__pyx_kp_u__57);
+        __Pyx_INCREF(__pyx_kp_u__58);
         __pyx_t_18 += 5;
-        __Pyx_GIVEREF(__pyx_kp_u__57);
-        PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_kp_u__57);
-        __pyx_t_16 = __Pyx_PyUnicode_Join(__pyx_t_3, 3, __pyx_t_18, __pyx_t_5); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 464, __pyx_L1_error)
+        __Pyx_GIVEREF(__pyx_kp_u__58);
+        PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_kp_u__58);
+        __pyx_t_16 = __Pyx_PyUnicode_Join(__pyx_t_3, 3, __pyx_t_18, __pyx_t_5); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 468, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_16);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_NotImplementedError, __pyx_t_16); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 464, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_NotImplementedError, __pyx_t_16); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 468, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
         __Pyx_Raise(__pyx_t_3, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __PYX_ERR(0, 464, __pyx_L1_error)
+        __PYX_ERR(0, 468, __pyx_L1_error)
 
-        /* "ext_modules/io_funcs.pyx":463
+        /* "ext_modules/io_funcs.pyx":467
  *         if metadata[keyword] == "*":
  *             fclose(fi)
  *             if datatype == b'A':             # <<<<<<<<<<<<<<
  *                 raise NotImplementedError(f"Current implementation does not support {keyword} = *!")
  *             else:
  */
       }
 
-      /* "ext_modules/io_funcs.pyx":466
+      /* "ext_modules/io_funcs.pyx":470
  *                 raise NotImplementedError(f"Current implementation does not support {keyword} = *!")
  *             else:
  *                 raise ValueError(f"$DATATYPE '{datatype}' should have {keyword} = *!")             # <<<<<<<<<<<<<<
  * 
  *         PBsview[pos] = int(metadata.pop(keyword))
  */
       /*else*/ {
-        __pyx_t_3 = PyTuple_New(5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 466, __pyx_L1_error)
+        __pyx_t_3 = PyTuple_New(5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 470, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __pyx_t_18 = 0;
         __pyx_t_5 = 127;
         __Pyx_INCREF(__pyx_kp_u_DATATYPE_3);
         __pyx_t_18 += 11;
         __Pyx_GIVEREF(__pyx_kp_u_DATATYPE_3);
         PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_kp_u_DATATYPE_3);
-        __pyx_t_16 = __Pyx_PyUnicode_From_char(__pyx_v_datatype, 0, ' ', 'd'); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 466, __pyx_L1_error)
+        __pyx_t_16 = __Pyx_PyUnicode_From_char(__pyx_v_datatype, 0, ' ', 'd'); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 470, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_16);
         __pyx_t_18 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_16);
         __Pyx_GIVEREF(__pyx_t_16);
         PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_16);
         __pyx_t_16 = 0;
         __Pyx_INCREF(__pyx_kp_u_should_have);
         __pyx_t_18 += 14;
         __Pyx_GIVEREF(__pyx_kp_u_should_have);
         PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_kp_u_should_have);
         __Pyx_INCREF(__pyx_v_keyword);
         __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_v_keyword) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_v_keyword) : __pyx_t_5;
         __pyx_t_18 += __Pyx_PyUnicode_GET_LENGTH(__pyx_v_keyword);
         __Pyx_GIVEREF(__pyx_v_keyword);
         PyTuple_SET_ITEM(__pyx_t_3, 3, __pyx_v_keyword);
-        __Pyx_INCREF(__pyx_kp_u__57);
+        __Pyx_INCREF(__pyx_kp_u__58);
         __pyx_t_18 += 5;
-        __Pyx_GIVEREF(__pyx_kp_u__57);
-        PyTuple_SET_ITEM(__pyx_t_3, 4, __pyx_kp_u__57);
-        __pyx_t_16 = __Pyx_PyUnicode_Join(__pyx_t_3, 5, __pyx_t_18, __pyx_t_5); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 466, __pyx_L1_error)
+        __Pyx_GIVEREF(__pyx_kp_u__58);
+        PyTuple_SET_ITEM(__pyx_t_3, 4, __pyx_kp_u__58);
+        __pyx_t_16 = __Pyx_PyUnicode_Join(__pyx_t_3, 5, __pyx_t_18, __pyx_t_5); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 470, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_16);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_16); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 466, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_16); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 470, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
         __Pyx_Raise(__pyx_t_3, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __PYX_ERR(0, 466, __pyx_L1_error)
+        __PYX_ERR(0, 470, __pyx_L1_error)
       }
 
-      /* "ext_modules/io_funcs.pyx":461
+      /* "ext_modules/io_funcs.pyx":465
  *         keyword = f"$P{i}B"
  * 
  *         if metadata[keyword] == "*":             # <<<<<<<<<<<<<<
  *             fclose(fi)
  *             if datatype == b'A':
  */
     }
 
-    /* "ext_modules/io_funcs.pyx":468
+    /* "ext_modules/io_funcs.pyx":472
  *                 raise ValueError(f"$DATATYPE '{datatype}' should have {keyword} = *!")
  * 
  *         PBsview[pos] = int(metadata.pop(keyword))             # <<<<<<<<<<<<<<
  * 
  *         if datatype == b'F':
  */
-    __pyx_t_3 = __Pyx_PyDict_Pop(__pyx_v_metadata, __pyx_v_keyword, ((PyObject *)NULL)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 468, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_Pop(__pyx_v_metadata, __pyx_v_keyword, ((PyObject *)NULL)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 472, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_16 = __Pyx_PyNumber_Int(__pyx_t_3); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 468, __pyx_L1_error)
+    __pyx_t_16 = __Pyx_PyNumber_Int(__pyx_t_3); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 472, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_16);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_14 = __Pyx_PyInt_As_int(__pyx_t_16); if (unlikely((__pyx_t_14 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 468, __pyx_L1_error)
+    __pyx_t_14 = __Pyx_PyInt_As_int(__pyx_t_16); if (unlikely((__pyx_t_14 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 472, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
     __pyx_t_17 = __pyx_v_pos;
     *((int *) ( /* dim=0 */ (__pyx_v_PBsview.data + __pyx_t_17 * __pyx_v_PBsview.strides[0]) )) = __pyx_t_14;
 
-    /* "ext_modules/io_funcs.pyx":470
+    /* "ext_modules/io_funcs.pyx":474
  *         PBsview[pos] = int(metadata.pop(keyword))
  * 
  *         if datatype == b'F':             # <<<<<<<<<<<<<<
  *             if PBsview[pos] != 32:
  *                 fclose(fi)
  */
     switch (__pyx_v_datatype) {
       case 'F':
 
-      /* "ext_modules/io_funcs.pyx":471
+      /* "ext_modules/io_funcs.pyx":475
  * 
  *         if datatype == b'F':
  *             if PBsview[pos] != 32:             # <<<<<<<<<<<<<<
  *                 fclose(fi)
  *                 raise ValueError(f"$DATATYPE '{datatype}' must have {keyword} = 32 ({keyword} = {PBsview[pos]})!")
  */
       __pyx_t_17 = __pyx_v_pos;
       __pyx_t_2 = (((*((int *) ( /* dim=0 */ (__pyx_v_PBsview.data + __pyx_t_17 * __pyx_v_PBsview.strides[0]) ))) != 32) != 0);
       if (unlikely(__pyx_t_2)) {
 
-        /* "ext_modules/io_funcs.pyx":472
+        /* "ext_modules/io_funcs.pyx":476
  *         if datatype == b'F':
  *             if PBsview[pos] != 32:
  *                 fclose(fi)             # <<<<<<<<<<<<<<
  *                 raise ValueError(f"$DATATYPE '{datatype}' must have {keyword} = 32 ({keyword} = {PBsview[pos]})!")
  *             PBsview[pos] = PBsview[pos] // 8
  */
         (void)(fclose(__pyx_v_fi));
 
-        /* "ext_modules/io_funcs.pyx":473
+        /* "ext_modules/io_funcs.pyx":477
  *             if PBsview[pos] != 32:
  *                 fclose(fi)
  *                 raise ValueError(f"$DATATYPE '{datatype}' must have {keyword} = 32 ({keyword} = {PBsview[pos]})!")             # <<<<<<<<<<<<<<
  *             PBsview[pos] = PBsview[pos] // 8
  *             if ldview[pos] > 0.0 or lvview[pos] > 0.0:
  */
-        __pyx_t_16 = PyTuple_New(9); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 473, __pyx_L1_error)
+        __pyx_t_16 = PyTuple_New(9); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 477, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_16);
         __pyx_t_18 = 0;
         __pyx_t_5 = 127;
         __Pyx_INCREF(__pyx_kp_u_DATATYPE_3);
         __pyx_t_18 += 11;
         __Pyx_GIVEREF(__pyx_kp_u_DATATYPE_3);
         PyTuple_SET_ITEM(__pyx_t_16, 0, __pyx_kp_u_DATATYPE_3);
-        __pyx_t_3 = __Pyx_PyUnicode_From_char(__pyx_v_datatype, 0, ' ', 'd'); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 473, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyUnicode_From_char(__pyx_v_datatype, 0, ' ', 'd'); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 477, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __pyx_t_18 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_3);
         __Pyx_GIVEREF(__pyx_t_3);
         PyTuple_SET_ITEM(__pyx_t_16, 1, __pyx_t_3);
         __pyx_t_3 = 0;
         __Pyx_INCREF(__pyx_kp_u_must_have);
         __pyx_t_18 += 12;
@@ -23830,60 +23945,60 @@
         __Pyx_GIVEREF(__pyx_kp_u_32);
         PyTuple_SET_ITEM(__pyx_t_16, 4, __pyx_kp_u_32);
         __Pyx_INCREF(__pyx_v_keyword);
         __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_v_keyword) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_v_keyword) : __pyx_t_5;
         __pyx_t_18 += __Pyx_PyUnicode_GET_LENGTH(__pyx_v_keyword);
         __Pyx_GIVEREF(__pyx_v_keyword);
         PyTuple_SET_ITEM(__pyx_t_16, 5, __pyx_v_keyword);
-        __Pyx_INCREF(__pyx_kp_u__58);
+        __Pyx_INCREF(__pyx_kp_u__59);
         __pyx_t_18 += 3;
-        __Pyx_GIVEREF(__pyx_kp_u__58);
-        PyTuple_SET_ITEM(__pyx_t_16, 6, __pyx_kp_u__58);
+        __Pyx_GIVEREF(__pyx_kp_u__59);
+        PyTuple_SET_ITEM(__pyx_t_16, 6, __pyx_kp_u__59);
         __pyx_t_17 = __pyx_v_pos;
-        __pyx_t_3 = __Pyx_PyUnicode_From_int((*((int *) ( /* dim=0 */ (__pyx_v_PBsview.data + __pyx_t_17 * __pyx_v_PBsview.strides[0]) ))), 0, ' ', 'd'); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 473, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyUnicode_From_int((*((int *) ( /* dim=0 */ (__pyx_v_PBsview.data + __pyx_t_17 * __pyx_v_PBsview.strides[0]) ))), 0, ' ', 'd'); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 477, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __pyx_t_18 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_3);
         __Pyx_GIVEREF(__pyx_t_3);
         PyTuple_SET_ITEM(__pyx_t_16, 7, __pyx_t_3);
         __pyx_t_3 = 0;
-        __Pyx_INCREF(__pyx_kp_u__59);
+        __Pyx_INCREF(__pyx_kp_u__60);
         __pyx_t_18 += 2;
-        __Pyx_GIVEREF(__pyx_kp_u__59);
-        PyTuple_SET_ITEM(__pyx_t_16, 8, __pyx_kp_u__59);
-        __pyx_t_3 = __Pyx_PyUnicode_Join(__pyx_t_16, 9, __pyx_t_18, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 473, __pyx_L1_error)
+        __Pyx_GIVEREF(__pyx_kp_u__60);
+        PyTuple_SET_ITEM(__pyx_t_16, 8, __pyx_kp_u__60);
+        __pyx_t_3 = __Pyx_PyUnicode_Join(__pyx_t_16, 9, __pyx_t_18, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 477, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-        __pyx_t_16 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 473, __pyx_L1_error)
+        __pyx_t_16 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 477, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_16);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_Raise(__pyx_t_16, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-        __PYX_ERR(0, 473, __pyx_L1_error)
+        __PYX_ERR(0, 477, __pyx_L1_error)
 
-        /* "ext_modules/io_funcs.pyx":471
+        /* "ext_modules/io_funcs.pyx":475
  * 
  *         if datatype == b'F':
  *             if PBsview[pos] != 32:             # <<<<<<<<<<<<<<
  *                 fclose(fi)
  *                 raise ValueError(f"$DATATYPE '{datatype}' must have {keyword} = 32 ({keyword} = {PBsview[pos]})!")
  */
       }
 
-      /* "ext_modules/io_funcs.pyx":474
+      /* "ext_modules/io_funcs.pyx":478
  *                 fclose(fi)
  *                 raise ValueError(f"$DATATYPE '{datatype}' must have {keyword} = 32 ({keyword} = {PBsview[pos]})!")
  *             PBsview[pos] = PBsview[pos] // 8             # <<<<<<<<<<<<<<
  *             if ldview[pos] > 0.0 or lvview[pos] > 0.0:
  *                 fclose(fi)
  */
       __pyx_t_17 = __pyx_v_pos;
       __pyx_t_27 = __pyx_v_pos;
       *((int *) ( /* dim=0 */ (__pyx_v_PBsview.data + __pyx_t_27 * __pyx_v_PBsview.strides[0]) )) = __Pyx_div_long((*((int *) ( /* dim=0 */ (__pyx_v_PBsview.data + __pyx_t_17 * __pyx_v_PBsview.strides[0]) ))), 8);
 
-      /* "ext_modules/io_funcs.pyx":475
+      /* "ext_modules/io_funcs.pyx":479
  *                 raise ValueError(f"$DATATYPE '{datatype}' must have {keyword} = 32 ({keyword} = {PBsview[pos]})!")
  *             PBsview[pos] = PBsview[pos] // 8
  *             if ldview[pos] > 0.0 or lvview[pos] > 0.0:             # <<<<<<<<<<<<<<
  *                 fclose(fi)
  *                 raise ValueError(f"$DATATYPE '{datatype}' must have $P{i}E = 0,0 ($P{i}E = {PEsview[pos]})!")
  */
       __pyx_t_17 = __pyx_v_pos;
@@ -23895,149 +24010,149 @@
       }
       __pyx_t_17 = __pyx_v_pos;
       __pyx_t_1 = (((*((float *) ( /* dim=0 */ (__pyx_v_lvview.data + __pyx_t_17 * __pyx_v_lvview.strides[0]) ))) > 0.0) != 0);
       __pyx_t_2 = __pyx_t_1;
       __pyx_L78_bool_binop_done:;
       if (unlikely(__pyx_t_2)) {
 
-        /* "ext_modules/io_funcs.pyx":476
+        /* "ext_modules/io_funcs.pyx":480
  *             PBsview[pos] = PBsview[pos] // 8
  *             if ldview[pos] > 0.0 or lvview[pos] > 0.0:
  *                 fclose(fi)             # <<<<<<<<<<<<<<
  *                 raise ValueError(f"$DATATYPE '{datatype}' must have $P{i}E = 0,0 ($P{i}E = {PEsview[pos]})!")
  *         elif datatype == b'D':
  */
         (void)(fclose(__pyx_v_fi));
 
-        /* "ext_modules/io_funcs.pyx":477
+        /* "ext_modules/io_funcs.pyx":481
  *             if ldview[pos] > 0.0 or lvview[pos] > 0.0:
  *                 fclose(fi)
  *                 raise ValueError(f"$DATATYPE '{datatype}' must have $P{i}E = 0,0 ($P{i}E = {PEsview[pos]})!")             # <<<<<<<<<<<<<<
  *         elif datatype == b'D':
  *             if PBsview[pos] != 64:
  */
-        __pyx_t_16 = PyTuple_New(9); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 477, __pyx_L1_error)
+        __pyx_t_16 = PyTuple_New(9); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 481, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_16);
         __pyx_t_18 = 0;
         __pyx_t_5 = 127;
         __Pyx_INCREF(__pyx_kp_u_DATATYPE_3);
         __pyx_t_18 += 11;
         __Pyx_GIVEREF(__pyx_kp_u_DATATYPE_3);
         PyTuple_SET_ITEM(__pyx_t_16, 0, __pyx_kp_u_DATATYPE_3);
-        __pyx_t_3 = __Pyx_PyUnicode_From_char(__pyx_v_datatype, 0, ' ', 'd'); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 477, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyUnicode_From_char(__pyx_v_datatype, 0, ' ', 'd'); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 481, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __pyx_t_18 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_3);
         __Pyx_GIVEREF(__pyx_t_3);
         PyTuple_SET_ITEM(__pyx_t_16, 1, __pyx_t_3);
         __pyx_t_3 = 0;
         __Pyx_INCREF(__pyx_kp_u_must_have_P);
         __pyx_t_18 += 14;
         __Pyx_GIVEREF(__pyx_kp_u_must_have_P);
         PyTuple_SET_ITEM(__pyx_t_16, 2, __pyx_kp_u_must_have_P);
-        __pyx_t_3 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_v_i, 0, ' ', 'd'); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 477, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_v_i, 0, ' ', 'd'); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 481, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __pyx_t_18 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_3);
         __Pyx_GIVEREF(__pyx_t_3);
         PyTuple_SET_ITEM(__pyx_t_16, 3, __pyx_t_3);
         __pyx_t_3 = 0;
         __Pyx_INCREF(__pyx_kp_u_E_0_0_P);
         __pyx_t_18 += 11;
         __Pyx_GIVEREF(__pyx_kp_u_E_0_0_P);
         PyTuple_SET_ITEM(__pyx_t_16, 4, __pyx_kp_u_E_0_0_P);
-        __pyx_t_3 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_v_i, 0, ' ', 'd'); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 477, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_v_i, 0, ' ', 'd'); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 481, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __pyx_t_18 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_3);
         __Pyx_GIVEREF(__pyx_t_3);
         PyTuple_SET_ITEM(__pyx_t_16, 5, __pyx_t_3);
         __pyx_t_3 = 0;
         __Pyx_INCREF(__pyx_kp_u_E_2);
         __pyx_t_18 += 4;
         __Pyx_GIVEREF(__pyx_kp_u_E_2);
         PyTuple_SET_ITEM(__pyx_t_16, 6, __pyx_kp_u_E_2);
         __pyx_t_17 = __pyx_v_pos;
         __pyx_t_3 = (PyObject *) *((PyObject * *) ( /* dim=0 */ (__pyx_v_PEsview.data + __pyx_t_17 * __pyx_v_PEsview.strides[0]) ));
         if (unlikely(__pyx_t_3 == NULL)) __pyx_t_3 = Py_None;
         __Pyx_INCREF((PyObject*)__pyx_t_3);
-        __pyx_t_15 = __Pyx_PyUnicode_Unicode(__pyx_t_3); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 477, __pyx_L1_error)
+        __pyx_t_15 = __Pyx_PyUnicode_Unicode(__pyx_t_3); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 481, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_15);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_15) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_15) : __pyx_t_5;
         __pyx_t_18 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_15);
         __Pyx_GIVEREF(__pyx_t_15);
         PyTuple_SET_ITEM(__pyx_t_16, 7, __pyx_t_15);
         __pyx_t_15 = 0;
-        __Pyx_INCREF(__pyx_kp_u__59);
+        __Pyx_INCREF(__pyx_kp_u__60);
         __pyx_t_18 += 2;
-        __Pyx_GIVEREF(__pyx_kp_u__59);
-        PyTuple_SET_ITEM(__pyx_t_16, 8, __pyx_kp_u__59);
-        __pyx_t_15 = __Pyx_PyUnicode_Join(__pyx_t_16, 9, __pyx_t_18, __pyx_t_5); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 477, __pyx_L1_error)
+        __Pyx_GIVEREF(__pyx_kp_u__60);
+        PyTuple_SET_ITEM(__pyx_t_16, 8, __pyx_kp_u__60);
+        __pyx_t_15 = __Pyx_PyUnicode_Join(__pyx_t_16, 9, __pyx_t_18, __pyx_t_5); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 481, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_15);
         __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-        __pyx_t_16 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_15); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 477, __pyx_L1_error)
+        __pyx_t_16 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_15); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 481, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_16);
         __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
         __Pyx_Raise(__pyx_t_16, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-        __PYX_ERR(0, 477, __pyx_L1_error)
+        __PYX_ERR(0, 481, __pyx_L1_error)
 
-        /* "ext_modules/io_funcs.pyx":475
+        /* "ext_modules/io_funcs.pyx":479
  *                 raise ValueError(f"$DATATYPE '{datatype}' must have {keyword} = 32 ({keyword} = {PBsview[pos]})!")
  *             PBsview[pos] = PBsview[pos] // 8
  *             if ldview[pos] > 0.0 or lvview[pos] > 0.0:             # <<<<<<<<<<<<<<
  *                 fclose(fi)
  *                 raise ValueError(f"$DATATYPE '{datatype}' must have $P{i}E = 0,0 ($P{i}E = {PEsview[pos]})!")
  */
       }
 
-      /* "ext_modules/io_funcs.pyx":470
+      /* "ext_modules/io_funcs.pyx":474
  *         PBsview[pos] = int(metadata.pop(keyword))
  * 
  *         if datatype == b'F':             # <<<<<<<<<<<<<<
  *             if PBsview[pos] != 32:
  *                 fclose(fi)
  */
       break;
       case 'D':
 
-      /* "ext_modules/io_funcs.pyx":479
+      /* "ext_modules/io_funcs.pyx":483
  *                 raise ValueError(f"$DATATYPE '{datatype}' must have $P{i}E = 0,0 ($P{i}E = {PEsview[pos]})!")
  *         elif datatype == b'D':
  *             if PBsview[pos] != 64:             # <<<<<<<<<<<<<<
  *                 fclose(fi)
  *                 raise ValueError(f"$DATATYPE '{datatype}' must have {keyword} = 64 ({keyword} = {PBsview[pos]})!")
  */
       __pyx_t_17 = __pyx_v_pos;
       __pyx_t_2 = (((*((int *) ( /* dim=0 */ (__pyx_v_PBsview.data + __pyx_t_17 * __pyx_v_PBsview.strides[0]) ))) != 64) != 0);
       if (unlikely(__pyx_t_2)) {
 
-        /* "ext_modules/io_funcs.pyx":480
+        /* "ext_modules/io_funcs.pyx":484
  *         elif datatype == b'D':
  *             if PBsview[pos] != 64:
  *                 fclose(fi)             # <<<<<<<<<<<<<<
  *                 raise ValueError(f"$DATATYPE '{datatype}' must have {keyword} = 64 ({keyword} = {PBsview[pos]})!")
  *             PBsview[pos] = PBsview[pos] // 8
  */
         (void)(fclose(__pyx_v_fi));
 
-        /* "ext_modules/io_funcs.pyx":481
+        /* "ext_modules/io_funcs.pyx":485
  *             if PBsview[pos] != 64:
  *                 fclose(fi)
  *                 raise ValueError(f"$DATATYPE '{datatype}' must have {keyword} = 64 ({keyword} = {PBsview[pos]})!")             # <<<<<<<<<<<<<<
  *             PBsview[pos] = PBsview[pos] // 8
  *             if ldview[pos] > 0.0 or lvview[pos] > 0.0:
  */
-        __pyx_t_16 = PyTuple_New(9); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 481, __pyx_L1_error)
+        __pyx_t_16 = PyTuple_New(9); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 485, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_16);
         __pyx_t_18 = 0;
         __pyx_t_5 = 127;
         __Pyx_INCREF(__pyx_kp_u_DATATYPE_3);
         __pyx_t_18 += 11;
         __Pyx_GIVEREF(__pyx_kp_u_DATATYPE_3);
         PyTuple_SET_ITEM(__pyx_t_16, 0, __pyx_kp_u_DATATYPE_3);
-        __pyx_t_15 = __Pyx_PyUnicode_From_char(__pyx_v_datatype, 0, ' ', 'd'); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 481, __pyx_L1_error)
+        __pyx_t_15 = __Pyx_PyUnicode_From_char(__pyx_v_datatype, 0, ' ', 'd'); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 485, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_15);
         __pyx_t_18 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_15);
         __Pyx_GIVEREF(__pyx_t_15);
         PyTuple_SET_ITEM(__pyx_t_16, 1, __pyx_t_15);
         __pyx_t_15 = 0;
         __Pyx_INCREF(__pyx_kp_u_must_have);
         __pyx_t_18 += 12;
@@ -24053,60 +24168,60 @@
         __Pyx_GIVEREF(__pyx_kp_u_64);
         PyTuple_SET_ITEM(__pyx_t_16, 4, __pyx_kp_u_64);
         __Pyx_INCREF(__pyx_v_keyword);
         __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_v_keyword) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_v_keyword) : __pyx_t_5;
         __pyx_t_18 += __Pyx_PyUnicode_GET_LENGTH(__pyx_v_keyword);
         __Pyx_GIVEREF(__pyx_v_keyword);
         PyTuple_SET_ITEM(__pyx_t_16, 5, __pyx_v_keyword);
-        __Pyx_INCREF(__pyx_kp_u__58);
+        __Pyx_INCREF(__pyx_kp_u__59);
         __pyx_t_18 += 3;
-        __Pyx_GIVEREF(__pyx_kp_u__58);
-        PyTuple_SET_ITEM(__pyx_t_16, 6, __pyx_kp_u__58);
+        __Pyx_GIVEREF(__pyx_kp_u__59);
+        PyTuple_SET_ITEM(__pyx_t_16, 6, __pyx_kp_u__59);
         __pyx_t_17 = __pyx_v_pos;
-        __pyx_t_15 = __Pyx_PyUnicode_From_int((*((int *) ( /* dim=0 */ (__pyx_v_PBsview.data + __pyx_t_17 * __pyx_v_PBsview.strides[0]) ))), 0, ' ', 'd'); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 481, __pyx_L1_error)
+        __pyx_t_15 = __Pyx_PyUnicode_From_int((*((int *) ( /* dim=0 */ (__pyx_v_PBsview.data + __pyx_t_17 * __pyx_v_PBsview.strides[0]) ))), 0, ' ', 'd'); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 485, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_15);
         __pyx_t_18 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_15);
         __Pyx_GIVEREF(__pyx_t_15);
         PyTuple_SET_ITEM(__pyx_t_16, 7, __pyx_t_15);
         __pyx_t_15 = 0;
-        __Pyx_INCREF(__pyx_kp_u__59);
+        __Pyx_INCREF(__pyx_kp_u__60);
         __pyx_t_18 += 2;
-        __Pyx_GIVEREF(__pyx_kp_u__59);
-        PyTuple_SET_ITEM(__pyx_t_16, 8, __pyx_kp_u__59);
-        __pyx_t_15 = __Pyx_PyUnicode_Join(__pyx_t_16, 9, __pyx_t_18, __pyx_t_5); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 481, __pyx_L1_error)
+        __Pyx_GIVEREF(__pyx_kp_u__60);
+        PyTuple_SET_ITEM(__pyx_t_16, 8, __pyx_kp_u__60);
+        __pyx_t_15 = __Pyx_PyUnicode_Join(__pyx_t_16, 9, __pyx_t_18, __pyx_t_5); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 485, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_15);
         __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-        __pyx_t_16 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_15); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 481, __pyx_L1_error)
+        __pyx_t_16 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_15); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 485, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_16);
         __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
         __Pyx_Raise(__pyx_t_16, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-        __PYX_ERR(0, 481, __pyx_L1_error)
+        __PYX_ERR(0, 485, __pyx_L1_error)
 
-        /* "ext_modules/io_funcs.pyx":479
+        /* "ext_modules/io_funcs.pyx":483
  *                 raise ValueError(f"$DATATYPE '{datatype}' must have $P{i}E = 0,0 ($P{i}E = {PEsview[pos]})!")
  *         elif datatype == b'D':
  *             if PBsview[pos] != 64:             # <<<<<<<<<<<<<<
  *                 fclose(fi)
  *                 raise ValueError(f"$DATATYPE '{datatype}' must have {keyword} = 64 ({keyword} = {PBsview[pos]})!")
  */
       }
 
-      /* "ext_modules/io_funcs.pyx":482
+      /* "ext_modules/io_funcs.pyx":486
  *                 fclose(fi)
  *                 raise ValueError(f"$DATATYPE '{datatype}' must have {keyword} = 64 ({keyword} = {PBsview[pos]})!")
  *             PBsview[pos] = PBsview[pos] // 8             # <<<<<<<<<<<<<<
  *             if ldview[pos] > 0.0 or lvview[pos] > 0.0:
  *                 fclose(fi)
  */
       __pyx_t_17 = __pyx_v_pos;
       __pyx_t_27 = __pyx_v_pos;
       *((int *) ( /* dim=0 */ (__pyx_v_PBsview.data + __pyx_t_27 * __pyx_v_PBsview.strides[0]) )) = __Pyx_div_long((*((int *) ( /* dim=0 */ (__pyx_v_PBsview.data + __pyx_t_17 * __pyx_v_PBsview.strides[0]) ))), 8);
 
-      /* "ext_modules/io_funcs.pyx":483
+      /* "ext_modules/io_funcs.pyx":487
  *                 raise ValueError(f"$DATATYPE '{datatype}' must have {keyword} = 64 ({keyword} = {PBsview[pos]})!")
  *             PBsview[pos] = PBsview[pos] // 8
  *             if ldview[pos] > 0.0 or lvview[pos] > 0.0:             # <<<<<<<<<<<<<<
  *                 fclose(fi)
  *                 raise ValueError(f"$DATATYPE '{datatype}' must have $P{i}E = 0,0 ($P{i}E = {PEsview[pos]})!")
  */
       __pyx_t_17 = __pyx_v_pos;
@@ -24118,151 +24233,151 @@
       }
       __pyx_t_17 = __pyx_v_pos;
       __pyx_t_1 = (((*((float *) ( /* dim=0 */ (__pyx_v_lvview.data + __pyx_t_17 * __pyx_v_lvview.strides[0]) ))) > 0.0) != 0);
       __pyx_t_2 = __pyx_t_1;
       __pyx_L82_bool_binop_done:;
       if (unlikely(__pyx_t_2)) {
 
-        /* "ext_modules/io_funcs.pyx":484
+        /* "ext_modules/io_funcs.pyx":488
  *             PBsview[pos] = PBsview[pos] // 8
  *             if ldview[pos] > 0.0 or lvview[pos] > 0.0:
  *                 fclose(fi)             # <<<<<<<<<<<<<<
  *                 raise ValueError(f"$DATATYPE '{datatype}' must have $P{i}E = 0,0 ($P{i}E = {PEsview[pos]})!")
  *         else:
  */
         (void)(fclose(__pyx_v_fi));
 
-        /* "ext_modules/io_funcs.pyx":485
+        /* "ext_modules/io_funcs.pyx":489
  *             if ldview[pos] > 0.0 or lvview[pos] > 0.0:
  *                 fclose(fi)
  *                 raise ValueError(f"$DATATYPE '{datatype}' must have $P{i}E = 0,0 ($P{i}E = {PEsview[pos]})!")             # <<<<<<<<<<<<<<
  *         else:
  *             if datatype == b'I':
  */
-        __pyx_t_16 = PyTuple_New(9); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 485, __pyx_L1_error)
+        __pyx_t_16 = PyTuple_New(9); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 489, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_16);
         __pyx_t_18 = 0;
         __pyx_t_5 = 127;
         __Pyx_INCREF(__pyx_kp_u_DATATYPE_3);
         __pyx_t_18 += 11;
         __Pyx_GIVEREF(__pyx_kp_u_DATATYPE_3);
         PyTuple_SET_ITEM(__pyx_t_16, 0, __pyx_kp_u_DATATYPE_3);
-        __pyx_t_15 = __Pyx_PyUnicode_From_char(__pyx_v_datatype, 0, ' ', 'd'); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 485, __pyx_L1_error)
+        __pyx_t_15 = __Pyx_PyUnicode_From_char(__pyx_v_datatype, 0, ' ', 'd'); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 489, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_15);
         __pyx_t_18 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_15);
         __Pyx_GIVEREF(__pyx_t_15);
         PyTuple_SET_ITEM(__pyx_t_16, 1, __pyx_t_15);
         __pyx_t_15 = 0;
         __Pyx_INCREF(__pyx_kp_u_must_have_P);
         __pyx_t_18 += 14;
         __Pyx_GIVEREF(__pyx_kp_u_must_have_P);
         PyTuple_SET_ITEM(__pyx_t_16, 2, __pyx_kp_u_must_have_P);
-        __pyx_t_15 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_v_i, 0, ' ', 'd'); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 485, __pyx_L1_error)
+        __pyx_t_15 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_v_i, 0, ' ', 'd'); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 489, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_15);
         __pyx_t_18 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_15);
         __Pyx_GIVEREF(__pyx_t_15);
         PyTuple_SET_ITEM(__pyx_t_16, 3, __pyx_t_15);
         __pyx_t_15 = 0;
         __Pyx_INCREF(__pyx_kp_u_E_0_0_P);
         __pyx_t_18 += 11;
         __Pyx_GIVEREF(__pyx_kp_u_E_0_0_P);
         PyTuple_SET_ITEM(__pyx_t_16, 4, __pyx_kp_u_E_0_0_P);
-        __pyx_t_15 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_v_i, 0, ' ', 'd'); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 485, __pyx_L1_error)
+        __pyx_t_15 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_v_i, 0, ' ', 'd'); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 489, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_15);
         __pyx_t_18 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_15);
         __Pyx_GIVEREF(__pyx_t_15);
         PyTuple_SET_ITEM(__pyx_t_16, 5, __pyx_t_15);
         __pyx_t_15 = 0;
         __Pyx_INCREF(__pyx_kp_u_E_2);
         __pyx_t_18 += 4;
         __Pyx_GIVEREF(__pyx_kp_u_E_2);
         PyTuple_SET_ITEM(__pyx_t_16, 6, __pyx_kp_u_E_2);
         __pyx_t_17 = __pyx_v_pos;
         __pyx_t_15 = (PyObject *) *((PyObject * *) ( /* dim=0 */ (__pyx_v_PEsview.data + __pyx_t_17 * __pyx_v_PEsview.strides[0]) ));
         if (unlikely(__pyx_t_15 == NULL)) __pyx_t_15 = Py_None;
         __Pyx_INCREF((PyObject*)__pyx_t_15);
-        __pyx_t_3 = __Pyx_PyUnicode_Unicode(__pyx_t_15); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 485, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyUnicode_Unicode(__pyx_t_15); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 489, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
         __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_3) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_3) : __pyx_t_5;
         __pyx_t_18 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_3);
         __Pyx_GIVEREF(__pyx_t_3);
         PyTuple_SET_ITEM(__pyx_t_16, 7, __pyx_t_3);
         __pyx_t_3 = 0;
-        __Pyx_INCREF(__pyx_kp_u__59);
+        __Pyx_INCREF(__pyx_kp_u__60);
         __pyx_t_18 += 2;
-        __Pyx_GIVEREF(__pyx_kp_u__59);
-        PyTuple_SET_ITEM(__pyx_t_16, 8, __pyx_kp_u__59);
-        __pyx_t_3 = __Pyx_PyUnicode_Join(__pyx_t_16, 9, __pyx_t_18, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 485, __pyx_L1_error)
+        __Pyx_GIVEREF(__pyx_kp_u__60);
+        PyTuple_SET_ITEM(__pyx_t_16, 8, __pyx_kp_u__60);
+        __pyx_t_3 = __Pyx_PyUnicode_Join(__pyx_t_16, 9, __pyx_t_18, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 489, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-        __pyx_t_16 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 485, __pyx_L1_error)
+        __pyx_t_16 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 489, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_16);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_Raise(__pyx_t_16, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-        __PYX_ERR(0, 485, __pyx_L1_error)
+        __PYX_ERR(0, 489, __pyx_L1_error)
 
-        /* "ext_modules/io_funcs.pyx":483
+        /* "ext_modules/io_funcs.pyx":487
  *                 raise ValueError(f"$DATATYPE '{datatype}' must have {keyword} = 64 ({keyword} = {PBsview[pos]})!")
  *             PBsview[pos] = PBsview[pos] // 8
  *             if ldview[pos] > 0.0 or lvview[pos] > 0.0:             # <<<<<<<<<<<<<<
  *                 fclose(fi)
  *                 raise ValueError(f"$DATATYPE '{datatype}' must have $P{i}E = 0,0 ($P{i}E = {PEsview[pos]})!")
  */
       }
 
-      /* "ext_modules/io_funcs.pyx":478
+      /* "ext_modules/io_funcs.pyx":482
  *                 fclose(fi)
  *                 raise ValueError(f"$DATATYPE '{datatype}' must have $P{i}E = 0,0 ($P{i}E = {PEsview[pos]})!")
  *         elif datatype == b'D':             # <<<<<<<<<<<<<<
  *             if PBsview[pos] != 64:
  *                 fclose(fi)
  */
       break;
       default:
 
-      /* "ext_modules/io_funcs.pyx":487
+      /* "ext_modules/io_funcs.pyx":491
  *                 raise ValueError(f"$DATATYPE '{datatype}' must have $P{i}E = 0,0 ($P{i}E = {PEsview[pos]})!")
  *         else:
  *             if datatype == b'I':             # <<<<<<<<<<<<<<
  *                 if PBsview[pos] % 8 != 0:
  *                     fclose(fi)
  */
       __pyx_t_2 = ((__pyx_v_datatype == 'I') != 0);
       if (__pyx_t_2) {
 
-        /* "ext_modules/io_funcs.pyx":488
+        /* "ext_modules/io_funcs.pyx":492
  *         else:
  *             if datatype == b'I':
  *                 if PBsview[pos] % 8 != 0:             # <<<<<<<<<<<<<<
  *                     fclose(fi)
  *                     raise NotImplementedError(f"Current implementation requires that {keyword} must be a multiple of 8 ({keyword} = {PBsview[pos]}) for $DATATYPE '{datatype}'!")
  */
         __pyx_t_17 = __pyx_v_pos;
         __pyx_t_2 = ((__Pyx_mod_long((*((int *) ( /* dim=0 */ (__pyx_v_PBsview.data + __pyx_t_17 * __pyx_v_PBsview.strides[0]) ))), 8) != 0) != 0);
         if (unlikely(__pyx_t_2)) {
 
-          /* "ext_modules/io_funcs.pyx":489
+          /* "ext_modules/io_funcs.pyx":493
  *             if datatype == b'I':
  *                 if PBsview[pos] % 8 != 0:
  *                     fclose(fi)             # <<<<<<<<<<<<<<
  *                     raise NotImplementedError(f"Current implementation requires that {keyword} must be a multiple of 8 ({keyword} = {PBsview[pos]}) for $DATATYPE '{datatype}'!")
  *                 PBsview[pos] = PBsview[pos] // 8
  */
           (void)(fclose(__pyx_v_fi));
 
-          /* "ext_modules/io_funcs.pyx":490
+          /* "ext_modules/io_funcs.pyx":494
  *                 if PBsview[pos] % 8 != 0:
  *                     fclose(fi)
  *                     raise NotImplementedError(f"Current implementation requires that {keyword} must be a multiple of 8 ({keyword} = {PBsview[pos]}) for $DATATYPE '{datatype}'!")             # <<<<<<<<<<<<<<
  *                 PBsview[pos] = PBsview[pos] // 8
  *                 if PBsview[pos] > 4:
  */
-          __pyx_t_16 = PyTuple_New(9); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 490, __pyx_L1_error)
+          __pyx_t_16 = PyTuple_New(9); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 494, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_16);
           __pyx_t_18 = 0;
           __pyx_t_5 = 127;
           __Pyx_INCREF(__pyx_kp_u_Current_implementation_requires);
           __pyx_t_18 += 37;
           __Pyx_GIVEREF(__pyx_kp_u_Current_implementation_requires);
           PyTuple_SET_ITEM(__pyx_t_16, 0, __pyx_kp_u_Current_implementation_requires);
@@ -24276,97 +24391,97 @@
           __Pyx_GIVEREF(__pyx_kp_u_must_be_a_multiple_of_8);
           PyTuple_SET_ITEM(__pyx_t_16, 2, __pyx_kp_u_must_be_a_multiple_of_8);
           __Pyx_INCREF(__pyx_v_keyword);
           __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_v_keyword) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_v_keyword) : __pyx_t_5;
           __pyx_t_18 += __Pyx_PyUnicode_GET_LENGTH(__pyx_v_keyword);
           __Pyx_GIVEREF(__pyx_v_keyword);
           PyTuple_SET_ITEM(__pyx_t_16, 3, __pyx_v_keyword);
-          __Pyx_INCREF(__pyx_kp_u__58);
+          __Pyx_INCREF(__pyx_kp_u__59);
           __pyx_t_18 += 3;
-          __Pyx_GIVEREF(__pyx_kp_u__58);
-          PyTuple_SET_ITEM(__pyx_t_16, 4, __pyx_kp_u__58);
+          __Pyx_GIVEREF(__pyx_kp_u__59);
+          PyTuple_SET_ITEM(__pyx_t_16, 4, __pyx_kp_u__59);
           __pyx_t_17 = __pyx_v_pos;
-          __pyx_t_3 = __Pyx_PyUnicode_From_int((*((int *) ( /* dim=0 */ (__pyx_v_PBsview.data + __pyx_t_17 * __pyx_v_PBsview.strides[0]) ))), 0, ' ', 'd'); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 490, __pyx_L1_error)
+          __pyx_t_3 = __Pyx_PyUnicode_From_int((*((int *) ( /* dim=0 */ (__pyx_v_PBsview.data + __pyx_t_17 * __pyx_v_PBsview.strides[0]) ))), 0, ' ', 'd'); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 494, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_3);
           __pyx_t_18 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_3);
           __Pyx_GIVEREF(__pyx_t_3);
           PyTuple_SET_ITEM(__pyx_t_16, 5, __pyx_t_3);
           __pyx_t_3 = 0;
           __Pyx_INCREF(__pyx_kp_u_for_DATATYPE);
           __pyx_t_18 += 17;
           __Pyx_GIVEREF(__pyx_kp_u_for_DATATYPE);
           PyTuple_SET_ITEM(__pyx_t_16, 6, __pyx_kp_u_for_DATATYPE);
-          __pyx_t_3 = __Pyx_PyUnicode_From_char(__pyx_v_datatype, 0, ' ', 'd'); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 490, __pyx_L1_error)
+          __pyx_t_3 = __Pyx_PyUnicode_From_char(__pyx_v_datatype, 0, ' ', 'd'); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 494, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_3);
           __pyx_t_18 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_3);
           __Pyx_GIVEREF(__pyx_t_3);
           PyTuple_SET_ITEM(__pyx_t_16, 7, __pyx_t_3);
           __pyx_t_3 = 0;
-          __Pyx_INCREF(__pyx_kp_u__41);
+          __Pyx_INCREF(__pyx_kp_u__42);
           __pyx_t_18 += 2;
-          __Pyx_GIVEREF(__pyx_kp_u__41);
-          PyTuple_SET_ITEM(__pyx_t_16, 8, __pyx_kp_u__41);
-          __pyx_t_3 = __Pyx_PyUnicode_Join(__pyx_t_16, 9, __pyx_t_18, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 490, __pyx_L1_error)
+          __Pyx_GIVEREF(__pyx_kp_u__42);
+          PyTuple_SET_ITEM(__pyx_t_16, 8, __pyx_kp_u__42);
+          __pyx_t_3 = __Pyx_PyUnicode_Join(__pyx_t_16, 9, __pyx_t_18, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 494, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-          __pyx_t_16 = __Pyx_PyObject_CallOneArg(__pyx_builtin_NotImplementedError, __pyx_t_3); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 490, __pyx_L1_error)
+          __pyx_t_16 = __Pyx_PyObject_CallOneArg(__pyx_builtin_NotImplementedError, __pyx_t_3); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 494, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_16);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_Raise(__pyx_t_16, 0, 0, 0);
           __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-          __PYX_ERR(0, 490, __pyx_L1_error)
+          __PYX_ERR(0, 494, __pyx_L1_error)
 
-          /* "ext_modules/io_funcs.pyx":488
+          /* "ext_modules/io_funcs.pyx":492
  *         else:
  *             if datatype == b'I':
  *                 if PBsview[pos] % 8 != 0:             # <<<<<<<<<<<<<<
  *                     fclose(fi)
  *                     raise NotImplementedError(f"Current implementation requires that {keyword} must be a multiple of 8 ({keyword} = {PBsview[pos]}) for $DATATYPE '{datatype}'!")
  */
         }
 
-        /* "ext_modules/io_funcs.pyx":491
+        /* "ext_modules/io_funcs.pyx":495
  *                     fclose(fi)
  *                     raise NotImplementedError(f"Current implementation requires that {keyword} must be a multiple of 8 ({keyword} = {PBsview[pos]}) for $DATATYPE '{datatype}'!")
  *                 PBsview[pos] = PBsview[pos] // 8             # <<<<<<<<<<<<<<
  *                 if PBsview[pos] > 4:
  *                     fclose(fi)
  */
         __pyx_t_17 = __pyx_v_pos;
         __pyx_t_27 = __pyx_v_pos;
         *((int *) ( /* dim=0 */ (__pyx_v_PBsview.data + __pyx_t_27 * __pyx_v_PBsview.strides[0]) )) = __Pyx_div_long((*((int *) ( /* dim=0 */ (__pyx_v_PBsview.data + __pyx_t_17 * __pyx_v_PBsview.strides[0]) ))), 8);
 
-        /* "ext_modules/io_funcs.pyx":492
+        /* "ext_modules/io_funcs.pyx":496
  *                     raise NotImplementedError(f"Current implementation requires that {keyword} must be a multiple of 8 ({keyword} = {PBsview[pos]}) for $DATATYPE '{datatype}'!")
  *                 PBsview[pos] = PBsview[pos] // 8
  *                 if PBsview[pos] > 4:             # <<<<<<<<<<<<<<
  *                     fclose(fi)
  *                     raise NotImplementedError(f"Current implementation requires that {keyword} be no more than 4 bytes for $DATATYPE '{datatype}'!")
  */
         __pyx_t_17 = __pyx_v_pos;
         __pyx_t_2 = (((*((int *) ( /* dim=0 */ (__pyx_v_PBsview.data + __pyx_t_17 * __pyx_v_PBsview.strides[0]) ))) > 4) != 0);
         if (unlikely(__pyx_t_2)) {
 
-          /* "ext_modules/io_funcs.pyx":493
+          /* "ext_modules/io_funcs.pyx":497
  *                 PBsview[pos] = PBsview[pos] // 8
  *                 if PBsview[pos] > 4:
  *                     fclose(fi)             # <<<<<<<<<<<<<<
  *                     raise NotImplementedError(f"Current implementation requires that {keyword} be no more than 4 bytes for $DATATYPE '{datatype}'!")
  *                 bmview[pos] = 2 ** (PRsview[pos] - 1).bit_length() - 1
  */
           (void)(fclose(__pyx_v_fi));
 
-          /* "ext_modules/io_funcs.pyx":494
+          /* "ext_modules/io_funcs.pyx":498
  *                 if PBsview[pos] > 4:
  *                     fclose(fi)
  *                     raise NotImplementedError(f"Current implementation requires that {keyword} be no more than 4 bytes for $DATATYPE '{datatype}'!")             # <<<<<<<<<<<<<<
  *                 bmview[pos] = 2 ** (PRsview[pos] - 1).bit_length() - 1
  *             else:
  */
-          __pyx_t_16 = PyTuple_New(5); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 494, __pyx_L1_error)
+          __pyx_t_16 = PyTuple_New(5); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 498, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_16);
           __pyx_t_18 = 0;
           __pyx_t_5 = 127;
           __Pyx_INCREF(__pyx_kp_u_Current_implementation_requires);
           __pyx_t_18 += 37;
           __Pyx_GIVEREF(__pyx_kp_u_Current_implementation_requires);
           PyTuple_SET_ITEM(__pyx_t_16, 0, __pyx_kp_u_Current_implementation_requires);
@@ -24375,121 +24490,121 @@
           __pyx_t_18 += __Pyx_PyUnicode_GET_LENGTH(__pyx_v_keyword);
           __Pyx_GIVEREF(__pyx_v_keyword);
           PyTuple_SET_ITEM(__pyx_t_16, 1, __pyx_v_keyword);
           __Pyx_INCREF(__pyx_kp_u_be_no_more_than_4_bytes_for_DAT);
           __pyx_t_18 += 40;
           __Pyx_GIVEREF(__pyx_kp_u_be_no_more_than_4_bytes_for_DAT);
           PyTuple_SET_ITEM(__pyx_t_16, 2, __pyx_kp_u_be_no_more_than_4_bytes_for_DAT);
-          __pyx_t_3 = __Pyx_PyUnicode_From_char(__pyx_v_datatype, 0, ' ', 'd'); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 494, __pyx_L1_error)
+          __pyx_t_3 = __Pyx_PyUnicode_From_char(__pyx_v_datatype, 0, ' ', 'd'); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 498, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_3);
           __pyx_t_18 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_3);
           __Pyx_GIVEREF(__pyx_t_3);
           PyTuple_SET_ITEM(__pyx_t_16, 3, __pyx_t_3);
           __pyx_t_3 = 0;
-          __Pyx_INCREF(__pyx_kp_u__41);
+          __Pyx_INCREF(__pyx_kp_u__42);
           __pyx_t_18 += 2;
-          __Pyx_GIVEREF(__pyx_kp_u__41);
-          PyTuple_SET_ITEM(__pyx_t_16, 4, __pyx_kp_u__41);
-          __pyx_t_3 = __Pyx_PyUnicode_Join(__pyx_t_16, 5, __pyx_t_18, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 494, __pyx_L1_error)
+          __Pyx_GIVEREF(__pyx_kp_u__42);
+          PyTuple_SET_ITEM(__pyx_t_16, 4, __pyx_kp_u__42);
+          __pyx_t_3 = __Pyx_PyUnicode_Join(__pyx_t_16, 5, __pyx_t_18, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 498, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-          __pyx_t_16 = __Pyx_PyObject_CallOneArg(__pyx_builtin_NotImplementedError, __pyx_t_3); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 494, __pyx_L1_error)
+          __pyx_t_16 = __Pyx_PyObject_CallOneArg(__pyx_builtin_NotImplementedError, __pyx_t_3); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 498, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_16);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_Raise(__pyx_t_16, 0, 0, 0);
           __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-          __PYX_ERR(0, 494, __pyx_L1_error)
+          __PYX_ERR(0, 498, __pyx_L1_error)
 
-          /* "ext_modules/io_funcs.pyx":492
+          /* "ext_modules/io_funcs.pyx":496
  *                     raise NotImplementedError(f"Current implementation requires that {keyword} must be a multiple of 8 ({keyword} = {PBsview[pos]}) for $DATATYPE '{datatype}'!")
  *                 PBsview[pos] = PBsview[pos] // 8
  *                 if PBsview[pos] > 4:             # <<<<<<<<<<<<<<
  *                     fclose(fi)
  *                     raise NotImplementedError(f"Current implementation requires that {keyword} be no more than 4 bytes for $DATATYPE '{datatype}'!")
  */
         }
 
-        /* "ext_modules/io_funcs.pyx":495
+        /* "ext_modules/io_funcs.pyx":499
  *                     fclose(fi)
  *                     raise NotImplementedError(f"Current implementation requires that {keyword} be no more than 4 bytes for $DATATYPE '{datatype}'!")
  *                 bmview[pos] = 2 ** (PRsview[pos] - 1).bit_length() - 1             # <<<<<<<<<<<<<<
  *             else:
  *                 # datatype must be 'A'
  */
         __pyx_t_17 = __pyx_v_pos;
-        __pyx_t_3 = __Pyx_PyInt_From_long(((*((int *) ( /* dim=0 */ (__pyx_v_PRsview.data + __pyx_t_17 * __pyx_v_PRsview.strides[0]) ))) - 1)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 495, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyInt_From_long(((*((int *) ( /* dim=0 */ (__pyx_v_PRsview.data + __pyx_t_17 * __pyx_v_PRsview.strides[0]) ))) - 1)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 499, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_bit_length); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 495, __pyx_L1_error)
+        __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_bit_length); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 499, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_15);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_t_3 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_15))) {
           __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_15);
           if (likely(__pyx_t_3)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_15);
             __Pyx_INCREF(__pyx_t_3);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_15, function);
           }
         }
         __pyx_t_16 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_15);
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 495, __pyx_L1_error)
+        if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 499, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_16);
         __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-        __pyx_t_15 = __Pyx_PyNumber_PowerOf2(__pyx_int_2, __pyx_t_16, Py_None); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 495, __pyx_L1_error)
+        __pyx_t_15 = __Pyx_PyNumber_PowerOf2(__pyx_int_2, __pyx_t_16, Py_None); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 499, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_15);
         __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-        __pyx_t_16 = __Pyx_PyInt_SubtractObjC(__pyx_t_15, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 495, __pyx_L1_error)
+        __pyx_t_16 = __Pyx_PyInt_SubtractObjC(__pyx_t_15, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 499, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_16);
         __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-        __pyx_t_14 = __Pyx_PyInt_As_int(__pyx_t_16); if (unlikely((__pyx_t_14 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 495, __pyx_L1_error)
+        __pyx_t_14 = __Pyx_PyInt_As_int(__pyx_t_16); if (unlikely((__pyx_t_14 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 499, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
         __pyx_t_17 = __pyx_v_pos;
         *((int *) ( /* dim=0 */ (__pyx_v_bmview.data + __pyx_t_17 * __pyx_v_bmview.strides[0]) )) = __pyx_t_14;
 
-        /* "ext_modules/io_funcs.pyx":487
+        /* "ext_modules/io_funcs.pyx":491
  *                 raise ValueError(f"$DATATYPE '{datatype}' must have $P{i}E = 0,0 ($P{i}E = {PEsview[pos]})!")
  *         else:
  *             if datatype == b'I':             # <<<<<<<<<<<<<<
  *                 if PBsview[pos] % 8 != 0:
  *                     fclose(fi)
  */
         goto __pyx_L84;
       }
 
-      /* "ext_modules/io_funcs.pyx":498
+      /* "ext_modules/io_funcs.pyx":502
  *             else:
  *                 # datatype must be 'A'
  *                 if PBsview[pos] > 9:             # <<<<<<<<<<<<<<
  *                     fclose(fi)
  *                     raise NotImplementedError(f"Current implementation does not support {keyword} > 9 for $DATATYPE '{datatype}'!")
  */
       /*else*/ {
         __pyx_t_17 = __pyx_v_pos;
         __pyx_t_2 = (((*((int *) ( /* dim=0 */ (__pyx_v_PBsview.data + __pyx_t_17 * __pyx_v_PBsview.strides[0]) ))) > 9) != 0);
         if (unlikely(__pyx_t_2)) {
 
-          /* "ext_modules/io_funcs.pyx":499
+          /* "ext_modules/io_funcs.pyx":503
  *                 # datatype must be 'A'
  *                 if PBsview[pos] > 9:
  *                     fclose(fi)             # <<<<<<<<<<<<<<
  *                     raise NotImplementedError(f"Current implementation does not support {keyword} > 9 for $DATATYPE '{datatype}'!")
  * 
  */
           (void)(fclose(__pyx_v_fi));
 
-          /* "ext_modules/io_funcs.pyx":500
+          /* "ext_modules/io_funcs.pyx":504
  *                 if PBsview[pos] > 9:
  *                     fclose(fi)
  *                     raise NotImplementedError(f"Current implementation does not support {keyword} > 9 for $DATATYPE '{datatype}'!")             # <<<<<<<<<<<<<<
  * 
  *             if ldview[pos] > 0.0 or lvview[pos] > 0.0:
  */
-          __pyx_t_16 = PyTuple_New(5); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 500, __pyx_L1_error)
+          __pyx_t_16 = PyTuple_New(5); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 504, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_16);
           __pyx_t_18 = 0;
           __pyx_t_5 = 127;
           __Pyx_INCREF(__pyx_kp_u_Current_implementation_does_not);
           __pyx_t_18 += 40;
           __Pyx_GIVEREF(__pyx_kp_u_Current_implementation_does_not);
           PyTuple_SET_ITEM(__pyx_t_16, 0, __pyx_kp_u_Current_implementation_does_not);
@@ -24498,46 +24613,46 @@
           __pyx_t_18 += __Pyx_PyUnicode_GET_LENGTH(__pyx_v_keyword);
           __Pyx_GIVEREF(__pyx_v_keyword);
           PyTuple_SET_ITEM(__pyx_t_16, 1, __pyx_v_keyword);
           __Pyx_INCREF(__pyx_kp_u_9_for_DATATYPE);
           __pyx_t_18 += 20;
           __Pyx_GIVEREF(__pyx_kp_u_9_for_DATATYPE);
           PyTuple_SET_ITEM(__pyx_t_16, 2, __pyx_kp_u_9_for_DATATYPE);
-          __pyx_t_15 = __Pyx_PyUnicode_From_char(__pyx_v_datatype, 0, ' ', 'd'); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 500, __pyx_L1_error)
+          __pyx_t_15 = __Pyx_PyUnicode_From_char(__pyx_v_datatype, 0, ' ', 'd'); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 504, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_15);
           __pyx_t_18 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_15);
           __Pyx_GIVEREF(__pyx_t_15);
           PyTuple_SET_ITEM(__pyx_t_16, 3, __pyx_t_15);
           __pyx_t_15 = 0;
-          __Pyx_INCREF(__pyx_kp_u__41);
+          __Pyx_INCREF(__pyx_kp_u__42);
           __pyx_t_18 += 2;
-          __Pyx_GIVEREF(__pyx_kp_u__41);
-          PyTuple_SET_ITEM(__pyx_t_16, 4, __pyx_kp_u__41);
-          __pyx_t_15 = __Pyx_PyUnicode_Join(__pyx_t_16, 5, __pyx_t_18, __pyx_t_5); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 500, __pyx_L1_error)
+          __Pyx_GIVEREF(__pyx_kp_u__42);
+          PyTuple_SET_ITEM(__pyx_t_16, 4, __pyx_kp_u__42);
+          __pyx_t_15 = __Pyx_PyUnicode_Join(__pyx_t_16, 5, __pyx_t_18, __pyx_t_5); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 504, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_15);
           __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-          __pyx_t_16 = __Pyx_PyObject_CallOneArg(__pyx_builtin_NotImplementedError, __pyx_t_15); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 500, __pyx_L1_error)
+          __pyx_t_16 = __Pyx_PyObject_CallOneArg(__pyx_builtin_NotImplementedError, __pyx_t_15); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 504, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_16);
           __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
           __Pyx_Raise(__pyx_t_16, 0, 0, 0);
           __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-          __PYX_ERR(0, 500, __pyx_L1_error)
+          __PYX_ERR(0, 504, __pyx_L1_error)
 
-          /* "ext_modules/io_funcs.pyx":498
+          /* "ext_modules/io_funcs.pyx":502
  *             else:
  *                 # datatype must be 'A'
  *                 if PBsview[pos] > 9:             # <<<<<<<<<<<<<<
  *                     fclose(fi)
  *                     raise NotImplementedError(f"Current implementation does not support {keyword} > 9 for $DATATYPE '{datatype}'!")
  */
         }
       }
       __pyx_L84:;
 
-      /* "ext_modules/io_funcs.pyx":502
+      /* "ext_modules/io_funcs.pyx":506
  *                     raise NotImplementedError(f"Current implementation does not support {keyword} > 9 for $DATATYPE '{datatype}'!")
  * 
  *             if ldview[pos] > 0.0 or lvview[pos] > 0.0:             # <<<<<<<<<<<<<<
  *                 if ldview[pos] == 0.0:
  *                     fclose(fi)
  */
       __pyx_t_17 = __pyx_v_pos;
@@ -24549,262 +24664,262 @@
       }
       __pyx_t_17 = __pyx_v_pos;
       __pyx_t_1 = (((*((float *) ( /* dim=0 */ (__pyx_v_lvview.data + __pyx_t_17 * __pyx_v_lvview.strides[0]) ))) > 0.0) != 0);
       __pyx_t_2 = __pyx_t_1;
       __pyx_L89_bool_binop_done:;
       if (__pyx_t_2) {
 
-        /* "ext_modules/io_funcs.pyx":503
+        /* "ext_modules/io_funcs.pyx":507
  * 
  *             if ldview[pos] > 0.0 or lvview[pos] > 0.0:
  *                 if ldview[pos] == 0.0:             # <<<<<<<<<<<<<<
  *                     fclose(fi)
  *                     raise ValueError(f"We require f1 > 0 for $PnE/f1,f2/({PEsview[pos]})!")
  */
         __pyx_t_17 = __pyx_v_pos;
         __pyx_t_2 = (((*((float *) ( /* dim=0 */ (__pyx_v_ldview.data + __pyx_t_17 * __pyx_v_ldview.strides[0]) ))) == 0.0) != 0);
         if (unlikely(__pyx_t_2)) {
 
-          /* "ext_modules/io_funcs.pyx":504
+          /* "ext_modules/io_funcs.pyx":508
  *             if ldview[pos] > 0.0 or lvview[pos] > 0.0:
  *                 if ldview[pos] == 0.0:
  *                     fclose(fi)             # <<<<<<<<<<<<<<
  *                     raise ValueError(f"We require f1 > 0 for $PnE/f1,f2/({PEsview[pos]})!")
  *                 if lvview[pos] == 0.0:
  */
           (void)(fclose(__pyx_v_fi));
 
-          /* "ext_modules/io_funcs.pyx":505
+          /* "ext_modules/io_funcs.pyx":509
  *                 if ldview[pos] == 0.0:
  *                     fclose(fi)
  *                     raise ValueError(f"We require f1 > 0 for $PnE/f1,f2/({PEsview[pos]})!")             # <<<<<<<<<<<<<<
  *                 if lvview[pos] == 0.0:
  *                     lvview[pos] = 1.0
  */
-          __pyx_t_16 = PyTuple_New(3); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 505, __pyx_L1_error)
+          __pyx_t_16 = PyTuple_New(3); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 509, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_16);
           __pyx_t_18 = 0;
           __pyx_t_5 = 127;
           __Pyx_INCREF(__pyx_kp_u_We_require_f1_0_for_PnE_f1_f2);
           __pyx_t_18 += 34;
           __Pyx_GIVEREF(__pyx_kp_u_We_require_f1_0_for_PnE_f1_f2);
           PyTuple_SET_ITEM(__pyx_t_16, 0, __pyx_kp_u_We_require_f1_0_for_PnE_f1_f2);
           __pyx_t_17 = __pyx_v_pos;
           __pyx_t_15 = (PyObject *) *((PyObject * *) ( /* dim=0 */ (__pyx_v_PEsview.data + __pyx_t_17 * __pyx_v_PEsview.strides[0]) ));
           if (unlikely(__pyx_t_15 == NULL)) __pyx_t_15 = Py_None;
           __Pyx_INCREF((PyObject*)__pyx_t_15);
-          __pyx_t_3 = __Pyx_PyUnicode_Unicode(__pyx_t_15); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 505, __pyx_L1_error)
+          __pyx_t_3 = __Pyx_PyUnicode_Unicode(__pyx_t_15); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 509, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
           __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_3) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_3) : __pyx_t_5;
           __pyx_t_18 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_3);
           __Pyx_GIVEREF(__pyx_t_3);
           PyTuple_SET_ITEM(__pyx_t_16, 1, __pyx_t_3);
           __pyx_t_3 = 0;
-          __Pyx_INCREF(__pyx_kp_u__59);
+          __Pyx_INCREF(__pyx_kp_u__60);
           __pyx_t_18 += 2;
-          __Pyx_GIVEREF(__pyx_kp_u__59);
-          PyTuple_SET_ITEM(__pyx_t_16, 2, __pyx_kp_u__59);
-          __pyx_t_3 = __Pyx_PyUnicode_Join(__pyx_t_16, 3, __pyx_t_18, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 505, __pyx_L1_error)
+          __Pyx_GIVEREF(__pyx_kp_u__60);
+          PyTuple_SET_ITEM(__pyx_t_16, 2, __pyx_kp_u__60);
+          __pyx_t_3 = __Pyx_PyUnicode_Join(__pyx_t_16, 3, __pyx_t_18, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 509, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-          __pyx_t_16 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 505, __pyx_L1_error)
+          __pyx_t_16 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 509, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_16);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_Raise(__pyx_t_16, 0, 0, 0);
           __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-          __PYX_ERR(0, 505, __pyx_L1_error)
+          __PYX_ERR(0, 509, __pyx_L1_error)
 
-          /* "ext_modules/io_funcs.pyx":503
+          /* "ext_modules/io_funcs.pyx":507
  * 
  *             if ldview[pos] > 0.0 or lvview[pos] > 0.0:
  *                 if ldview[pos] == 0.0:             # <<<<<<<<<<<<<<
  *                     fclose(fi)
  *                     raise ValueError(f"We require f1 > 0 for $PnE/f1,f2/({PEsview[pos]})!")
  */
         }
 
-        /* "ext_modules/io_funcs.pyx":506
+        /* "ext_modules/io_funcs.pyx":510
  *                     fclose(fi)
  *                     raise ValueError(f"We require f1 > 0 for $PnE/f1,f2/({PEsview[pos]})!")
  *                 if lvview[pos] == 0.0:             # <<<<<<<<<<<<<<
  *                     lvview[pos] = 1.0
  *                     print(f"Warning: detected f2 = 0 for $P{i}E/{PEsview[pos]}/, which is not correct. Set f2 = 1 instead.")
  */
         __pyx_t_17 = __pyx_v_pos;
         __pyx_t_2 = (((*((float *) ( /* dim=0 */ (__pyx_v_lvview.data + __pyx_t_17 * __pyx_v_lvview.strides[0]) ))) == 0.0) != 0);
         if (__pyx_t_2) {
 
-          /* "ext_modules/io_funcs.pyx":507
+          /* "ext_modules/io_funcs.pyx":511
  *                     raise ValueError(f"We require f1 > 0 for $PnE/f1,f2/({PEsview[pos]})!")
  *                 if lvview[pos] == 0.0:
  *                     lvview[pos] = 1.0             # <<<<<<<<<<<<<<
  *                     print(f"Warning: detected f2 = 0 for $P{i}E/{PEsview[pos]}/, which is not correct. Set f2 = 1 instead.")
  * 
  */
           __pyx_t_17 = __pyx_v_pos;
           *((float *) ( /* dim=0 */ (__pyx_v_lvview.data + __pyx_t_17 * __pyx_v_lvview.strides[0]) )) = 1.0;
 
-          /* "ext_modules/io_funcs.pyx":508
+          /* "ext_modules/io_funcs.pyx":512
  *                 if lvview[pos] == 0.0:
  *                     lvview[pos] = 1.0
  *                     print(f"Warning: detected f2 = 0 for $P{i}E/{PEsview[pos]}/, which is not correct. Set f2 = 1 instead.")             # <<<<<<<<<<<<<<
  * 
  *         total_bytes_per_row += PBsview[pos]
  */
-          __pyx_t_16 = PyTuple_New(5); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 508, __pyx_L1_error)
+          __pyx_t_16 = PyTuple_New(5); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 512, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_16);
           __pyx_t_18 = 0;
           __pyx_t_5 = 127;
           __Pyx_INCREF(__pyx_kp_u_Warning_detected_f2_0_for_P);
           __pyx_t_18 += 31;
           __Pyx_GIVEREF(__pyx_kp_u_Warning_detected_f2_0_for_P);
           PyTuple_SET_ITEM(__pyx_t_16, 0, __pyx_kp_u_Warning_detected_f2_0_for_P);
-          __pyx_t_3 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_v_i, 0, ' ', 'd'); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 508, __pyx_L1_error)
+          __pyx_t_3 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_v_i, 0, ' ', 'd'); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 512, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_3);
           __pyx_t_18 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_3);
           __Pyx_GIVEREF(__pyx_t_3);
           PyTuple_SET_ITEM(__pyx_t_16, 1, __pyx_t_3);
           __pyx_t_3 = 0;
           __Pyx_INCREF(__pyx_kp_u_E_3);
           __pyx_t_18 += 2;
           __Pyx_GIVEREF(__pyx_kp_u_E_3);
           PyTuple_SET_ITEM(__pyx_t_16, 2, __pyx_kp_u_E_3);
           __pyx_t_17 = __pyx_v_pos;
           __pyx_t_3 = (PyObject *) *((PyObject * *) ( /* dim=0 */ (__pyx_v_PEsview.data + __pyx_t_17 * __pyx_v_PEsview.strides[0]) ));
           if (unlikely(__pyx_t_3 == NULL)) __pyx_t_3 = Py_None;
           __Pyx_INCREF((PyObject*)__pyx_t_3);
-          __pyx_t_15 = __Pyx_PyUnicode_Unicode(__pyx_t_3); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 508, __pyx_L1_error)
+          __pyx_t_15 = __Pyx_PyUnicode_Unicode(__pyx_t_3); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 512, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_15);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_15) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_15) : __pyx_t_5;
           __pyx_t_18 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_15);
           __Pyx_GIVEREF(__pyx_t_15);
           PyTuple_SET_ITEM(__pyx_t_16, 3, __pyx_t_15);
           __pyx_t_15 = 0;
           __Pyx_INCREF(__pyx_kp_u_which_is_not_correct_Set_f2_1_i);
           __pyx_t_18 += 44;
           __Pyx_GIVEREF(__pyx_kp_u_which_is_not_correct_Set_f2_1_i);
           PyTuple_SET_ITEM(__pyx_t_16, 4, __pyx_kp_u_which_is_not_correct_Set_f2_1_i);
-          __pyx_t_15 = __Pyx_PyUnicode_Join(__pyx_t_16, 5, __pyx_t_18, __pyx_t_5); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 508, __pyx_L1_error)
+          __pyx_t_15 = __Pyx_PyUnicode_Join(__pyx_t_16, 5, __pyx_t_18, __pyx_t_5); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 512, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_15);
           __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-          __pyx_t_16 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_15); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 508, __pyx_L1_error)
+          __pyx_t_16 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_15); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 512, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_16);
           __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
           __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
 
-          /* "ext_modules/io_funcs.pyx":506
+          /* "ext_modules/io_funcs.pyx":510
  *                     fclose(fi)
  *                     raise ValueError(f"We require f1 > 0 for $PnE/f1,f2/({PEsview[pos]})!")
  *                 if lvview[pos] == 0.0:             # <<<<<<<<<<<<<<
  *                     lvview[pos] = 1.0
  *                     print(f"Warning: detected f2 = 0 for $P{i}E/{PEsview[pos]}/, which is not correct. Set f2 = 1 instead.")
  */
         }
 
-        /* "ext_modules/io_funcs.pyx":502
+        /* "ext_modules/io_funcs.pyx":506
  *                     raise NotImplementedError(f"Current implementation does not support {keyword} > 9 for $DATATYPE '{datatype}'!")
  * 
  *             if ldview[pos] > 0.0 or lvview[pos] > 0.0:             # <<<<<<<<<<<<<<
  *                 if ldview[pos] == 0.0:
  *                     fclose(fi)
  */
       }
       break;
     }
 
-    /* "ext_modules/io_funcs.pyx":510
+    /* "ext_modules/io_funcs.pyx":514
  *                     print(f"Warning: detected f2 = 0 for $P{i}E/{PEsview[pos]}/, which is not correct. Set f2 = 1 instead.")
  * 
  *         total_bytes_per_row += PBsview[pos]             # <<<<<<<<<<<<<<
  * 
  * 
  */
     __pyx_t_17 = __pyx_v_pos;
     __pyx_v_total_bytes_per_row = (__pyx_v_total_bytes_per_row + (*((int *) ( /* dim=0 */ (__pyx_v_PBsview.data + __pyx_t_17 * __pyx_v_PBsview.strides[0]) ))));
   }
 
-  /* "ext_modules/io_funcs.pyx":514
+  /* "ext_modules/io_funcs.pyx":518
  * 
  *     # SEEK data start
  *     data = np.zeros((N, M), dtype = np.float32)             # <<<<<<<<<<<<<<
  *     cdef float[:, :] data_view = data
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_16, __pyx_n_s_np); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 514, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_16, __pyx_n_s_np); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 518, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_16);
-  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_16, __pyx_n_s_zeros); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 514, __pyx_L1_error)
+  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_16, __pyx_n_s_zeros); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 518, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
   __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-  __pyx_t_16 = __Pyx_PyInt_From_int(__pyx_v_N); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 514, __pyx_L1_error)
+  __pyx_t_16 = __Pyx_PyInt_From_int(__pyx_v_N); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 518, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_16);
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_M); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 514, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_M); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 518, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 514, __pyx_L1_error)
+  __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 518, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_GIVEREF(__pyx_t_16);
   PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_16);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_3);
   __pyx_t_16 = 0;
   __pyx_t_3 = 0;
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 514, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 518, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_8);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_8);
   __pyx_t_8 = 0;
-  __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 514, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 518, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __Pyx_GetModuleGlobalName(__pyx_t_16, __pyx_n_s_np); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 514, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_16, __pyx_n_s_np); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 518, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_16);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_16, __pyx_n_s_float32); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 514, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_16, __pyx_n_s_float32); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 518, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-  if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 514, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 518, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_15, __pyx_t_3, __pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 514, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_15, __pyx_t_3, __pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 518, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __pyx_v_data = __pyx_t_7;
   __pyx_t_7 = 0;
 
-  /* "ext_modules/io_funcs.pyx":515
+  /* "ext_modules/io_funcs.pyx":519
  *     # SEEK data start
  *     data = np.zeros((N, M), dtype = np.float32)
  *     cdef float[:, :] data_view = data             # <<<<<<<<<<<<<<
  * 
  *     cdef size_t buffer_size = (<size_t>N) * (<size_t>total_bytes_per_row)
  */
-  __pyx_t_28 = __Pyx_PyObject_to_MemoryviewSlice_dsds_float(__pyx_v_data, PyBUF_WRITABLE); if (unlikely(!__pyx_t_28.memview)) __PYX_ERR(0, 515, __pyx_L1_error)
+  __pyx_t_28 = __Pyx_PyObject_to_MemoryviewSlice_dsds_float(__pyx_v_data, PyBUF_WRITABLE); if (unlikely(!__pyx_t_28.memview)) __PYX_ERR(0, 519, __pyx_L1_error)
   __pyx_v_data_view = __pyx_t_28;
   __pyx_t_28.memview = NULL;
   __pyx_t_28.data = NULL;
 
-  /* "ext_modules/io_funcs.pyx":517
+  /* "ext_modules/io_funcs.pyx":521
  *     cdef float[:, :] data_view = data
  * 
  *     cdef size_t buffer_size = (<size_t>N) * (<size_t>total_bytes_per_row)             # <<<<<<<<<<<<<<
  *     cdef size_t data_size = data_end - data_start + 1
  *     if buffer_size != data_size and buffer_size != data_size - 1: # buffer_size == data_size - 1 because [data_start, data_end)
  */
   __pyx_v_buffer_size = (((size_t)__pyx_v_N) * ((size_t)__pyx_v_total_bytes_per_row));
 
-  /* "ext_modules/io_funcs.pyx":518
+  /* "ext_modules/io_funcs.pyx":522
  * 
  *     cdef size_t buffer_size = (<size_t>N) * (<size_t>total_bytes_per_row)
  *     cdef size_t data_size = data_end - data_start + 1             # <<<<<<<<<<<<<<
  *     if buffer_size != data_size and buffer_size != data_size - 1: # buffer_size == data_size - 1 because [data_start, data_end)
  *         print(f"Warning: Data size recorded in the DATA segment {data_end - data_start + 1} does not match the actual data size {buffer_size}.")
  */
   __pyx_v_data_size = ((__pyx_v_data_end - __pyx_v_data_start) + 1);
 
-  /* "ext_modules/io_funcs.pyx":519
+  /* "ext_modules/io_funcs.pyx":523
  *     cdef size_t buffer_size = (<size_t>N) * (<size_t>total_bytes_per_row)
  *     cdef size_t data_size = data_end - data_start + 1
  *     if buffer_size != data_size and buffer_size != data_size - 1: # buffer_size == data_size - 1 because [data_start, data_end)             # <<<<<<<<<<<<<<
  *         print(f"Warning: Data size recorded in the DATA segment {data_end - data_start + 1} does not match the actual data size {buffer_size}.")
  * 
  */
   __pyx_t_1 = ((__pyx_v_buffer_size != __pyx_v_data_size) != 0);
@@ -24814,191 +24929,191 @@
     goto __pyx_L94_bool_binop_done;
   }
   __pyx_t_1 = ((__pyx_v_buffer_size != (__pyx_v_data_size - 1)) != 0);
   __pyx_t_2 = __pyx_t_1;
   __pyx_L94_bool_binop_done:;
   if (__pyx_t_2) {
 
-    /* "ext_modules/io_funcs.pyx":520
+    /* "ext_modules/io_funcs.pyx":524
  *     cdef size_t data_size = data_end - data_start + 1
  *     if buffer_size != data_size and buffer_size != data_size - 1: # buffer_size == data_size - 1 because [data_start, data_end)
  *         print(f"Warning: Data size recorded in the DATA segment {data_end - data_start + 1} does not match the actual data size {buffer_size}.")             # <<<<<<<<<<<<<<
  * 
  *     cdef uchar* bytes_buffer = <uchar*>malloc(buffer_size + 1)
  */
-    __pyx_t_7 = PyTuple_New(5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 520, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 524, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_4 = 0;
     __pyx_t_5 = 127;
     __Pyx_INCREF(__pyx_kp_u_Warning_Data_size_recorded_in_th);
     __pyx_t_4 += 48;
     __Pyx_GIVEREF(__pyx_kp_u_Warning_Data_size_recorded_in_th);
     PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_kp_u_Warning_Data_size_recorded_in_th);
-    __pyx_t_8 = __Pyx_PyUnicode_From_size_t(((__pyx_v_data_end - __pyx_v_data_start) + 1), 0, ' ', 'd'); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 520, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyUnicode_From_size_t(((__pyx_v_data_end - __pyx_v_data_start) + 1), 0, ' ', 'd'); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 524, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __pyx_t_4 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_8);
     __Pyx_GIVEREF(__pyx_t_8);
     PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_8);
     __pyx_t_8 = 0;
     __Pyx_INCREF(__pyx_kp_u_does_not_match_the_actual_data);
     __pyx_t_4 += 37;
     __Pyx_GIVEREF(__pyx_kp_u_does_not_match_the_actual_data);
     PyTuple_SET_ITEM(__pyx_t_7, 2, __pyx_kp_u_does_not_match_the_actual_data);
-    __pyx_t_8 = __Pyx_PyUnicode_From_size_t(__pyx_v_buffer_size, 0, ' ', 'd'); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 520, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyUnicode_From_size_t(__pyx_v_buffer_size, 0, ' ', 'd'); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 524, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __pyx_t_4 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_8);
     __Pyx_GIVEREF(__pyx_t_8);
     PyTuple_SET_ITEM(__pyx_t_7, 3, __pyx_t_8);
     __pyx_t_8 = 0;
-    __Pyx_INCREF(__pyx_kp_u__54);
+    __Pyx_INCREF(__pyx_kp_u__55);
     __pyx_t_4 += 1;
-    __Pyx_GIVEREF(__pyx_kp_u__54);
-    PyTuple_SET_ITEM(__pyx_t_7, 4, __pyx_kp_u__54);
-    __pyx_t_8 = __Pyx_PyUnicode_Join(__pyx_t_7, 5, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 520, __pyx_L1_error)
+    __Pyx_GIVEREF(__pyx_kp_u__55);
+    PyTuple_SET_ITEM(__pyx_t_7, 4, __pyx_kp_u__55);
+    __pyx_t_8 = __Pyx_PyUnicode_Join(__pyx_t_7, 5, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 524, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 520, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 524, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "ext_modules/io_funcs.pyx":519
+    /* "ext_modules/io_funcs.pyx":523
  *     cdef size_t buffer_size = (<size_t>N) * (<size_t>total_bytes_per_row)
  *     cdef size_t data_size = data_end - data_start + 1
  *     if buffer_size != data_size and buffer_size != data_size - 1: # buffer_size == data_size - 1 because [data_start, data_end)             # <<<<<<<<<<<<<<
  *         print(f"Warning: Data size recorded in the DATA segment {data_end - data_start + 1} does not match the actual data size {buffer_size}.")
  * 
  */
   }
 
-  /* "ext_modules/io_funcs.pyx":522
+  /* "ext_modules/io_funcs.pyx":526
  *         print(f"Warning: Data size recorded in the DATA segment {data_end - data_start + 1} does not match the actual data size {buffer_size}.")
  * 
  *     cdef uchar* bytes_buffer = <uchar*>malloc(buffer_size + 1)             # <<<<<<<<<<<<<<
  *     assert bytes_buffer != NULL
  * 
  */
   __pyx_v_bytes_buffer = ((__pyx_t_9pegasusio_5cylib_2io_uchar *)malloc((__pyx_v_buffer_size + 1)));
 
-  /* "ext_modules/io_funcs.pyx":523
+  /* "ext_modules/io_funcs.pyx":527
  * 
  *     cdef uchar* bytes_buffer = <uchar*>malloc(buffer_size + 1)
  *     assert bytes_buffer != NULL             # <<<<<<<<<<<<<<
  * 
  *     cdef uchar* buf = bytes_buffer
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(!Py_OptimizeFlag)) {
     if (unlikely(!((__pyx_v_bytes_buffer != NULL) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(0, 523, __pyx_L1_error)
+      __PYX_ERR(0, 527, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "ext_modules/io_funcs.pyx":525
+  /* "ext_modules/io_funcs.pyx":529
  *     assert bytes_buffer != NULL
  * 
  *     cdef uchar* buf = bytes_buffer             # <<<<<<<<<<<<<<
  * 
  *     from sys import byteorder
  */
   __pyx_v_buf = __pyx_v_bytes_buffer;
 
-  /* "ext_modules/io_funcs.pyx":527
+  /* "ext_modules/io_funcs.pyx":531
  *     cdef uchar* buf = bytes_buffer
  * 
  *     from sys import byteorder             # <<<<<<<<<<<<<<
  *     cdef bint should_swap = endian != byteorder
  * 
  */
-  __pyx_t_7 = PyList_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 527, __pyx_L1_error)
+  __pyx_t_7 = PyList_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 531, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_INCREF(__pyx_n_s_byteorder);
   __Pyx_GIVEREF(__pyx_n_s_byteorder);
   PyList_SET_ITEM(__pyx_t_7, 0, __pyx_n_s_byteorder);
-  __pyx_t_8 = __Pyx_Import(__pyx_n_s_sys, __pyx_t_7, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 527, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_Import(__pyx_n_s_sys, __pyx_t_7, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 531, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_ImportFrom(__pyx_t_8, __pyx_n_s_byteorder); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 527, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_ImportFrom(__pyx_t_8, __pyx_n_s_byteorder); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 531, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_INCREF(__pyx_t_7);
   __pyx_v_byteorder = __pyx_t_7;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "ext_modules/io_funcs.pyx":528
+  /* "ext_modules/io_funcs.pyx":532
  * 
  *     from sys import byteorder
  *     cdef bint should_swap = endian != byteorder             # <<<<<<<<<<<<<<
  * 
  *     cdef int value_int
  */
-  __pyx_t_8 = PyObject_RichCompare(__pyx_v_endian, __pyx_v_byteorder, Py_NE); __Pyx_XGOTREF(__pyx_t_8); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 528, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_8); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 528, __pyx_L1_error)
+  __pyx_t_8 = PyObject_RichCompare(__pyx_v_endian, __pyx_v_byteorder, Py_NE); __Pyx_XGOTREF(__pyx_t_8); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 532, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_8); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 532, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __pyx_v_should_swap = __pyx_t_2;
 
-  /* "ext_modules/io_funcs.pyx":533
+  /* "ext_modules/io_funcs.pyx":537
  *     cdef double value_double
  * 
  *     assert fseek(fi, data_start, SEEK_SET) == 0             # <<<<<<<<<<<<<<
  *     assert fread(<void*>bytes_buffer, 1, buffer_size, fi) == buffer_size
  * 
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(!Py_OptimizeFlag)) {
     if (unlikely(!((fseek(__pyx_v_fi, __pyx_v_data_start, SEEK_SET) == 0) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(0, 533, __pyx_L1_error)
+      __PYX_ERR(0, 537, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "ext_modules/io_funcs.pyx":534
+  /* "ext_modules/io_funcs.pyx":538
  * 
  *     assert fseek(fi, data_start, SEEK_SET) == 0
  *     assert fread(<void*>bytes_buffer, 1, buffer_size, fi) == buffer_size             # <<<<<<<<<<<<<<
  * 
  *     for i in range(N):
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(!Py_OptimizeFlag)) {
     if (unlikely(!((fread(((void *)__pyx_v_bytes_buffer), 1, __pyx_v_buffer_size, __pyx_v_fi) == __pyx_v_buffer_size) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(0, 534, __pyx_L1_error)
+      __PYX_ERR(0, 538, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "ext_modules/io_funcs.pyx":536
+  /* "ext_modules/io_funcs.pyx":540
  *     assert fread(<void*>bytes_buffer, 1, buffer_size, fi) == buffer_size
  * 
  *     for i in range(N):             # <<<<<<<<<<<<<<
  *         for j in range(M):
  *             if datatype != b'A' and should_swap:
  */
   __pyx_t_14 = __pyx_v_N;
   __pyx_t_29 = __pyx_t_14;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_29; __pyx_t_4+=1) {
     __pyx_v_i = __pyx_t_4;
 
-    /* "ext_modules/io_funcs.pyx":537
+    /* "ext_modules/io_funcs.pyx":541
  * 
  *     for i in range(N):
  *         for j in range(M):             # <<<<<<<<<<<<<<
  *             if datatype != b'A' and should_swap:
  *                 swapbytes(buf, PBsview[j])
  */
     __pyx_t_30 = __pyx_v_M;
     __pyx_t_31 = __pyx_t_30;
     for (__pyx_t_18 = 0; __pyx_t_18 < __pyx_t_31; __pyx_t_18+=1) {
       __pyx_v_j = __pyx_t_18;
 
-      /* "ext_modules/io_funcs.pyx":538
+      /* "ext_modules/io_funcs.pyx":542
  *     for i in range(N):
  *         for j in range(M):
  *             if datatype != b'A' and should_swap:             # <<<<<<<<<<<<<<
  *                 swapbytes(buf, PBsview[j])
  * 
  */
       __pyx_t_1 = ((__pyx_v_datatype != 'A') != 0);
@@ -25008,187 +25123,187 @@
         goto __pyx_L101_bool_binop_done;
       }
       __pyx_t_1 = (__pyx_v_should_swap != 0);
       __pyx_t_2 = __pyx_t_1;
       __pyx_L101_bool_binop_done:;
       if (__pyx_t_2) {
 
-        /* "ext_modules/io_funcs.pyx":539
+        /* "ext_modules/io_funcs.pyx":543
  *         for j in range(M):
  *             if datatype != b'A' and should_swap:
  *                 swapbytes(buf, PBsview[j])             # <<<<<<<<<<<<<<
  * 
  *             if datatype == b'D':
  */
         __pyx_t_10 = __pyx_v_j;
-        __pyx_t_8 = __pyx_f_9pegasusio_5cylib_2io_swapbytes(__pyx_v_buf, (*((int *) ( /* dim=0 */ (__pyx_v_PBsview.data + __pyx_t_10 * __pyx_v_PBsview.strides[0]) )))); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 539, __pyx_L1_error)
+        __pyx_t_8 = __pyx_f_9pegasusio_5cylib_2io_swapbytes(__pyx_v_buf, (*((int *) ( /* dim=0 */ (__pyx_v_PBsview.data + __pyx_t_10 * __pyx_v_PBsview.strides[0]) )))); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 543, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-        /* "ext_modules/io_funcs.pyx":538
+        /* "ext_modules/io_funcs.pyx":542
  *     for i in range(N):
  *         for j in range(M):
  *             if datatype != b'A' and should_swap:             # <<<<<<<<<<<<<<
  *                 swapbytes(buf, PBsview[j])
  * 
  */
       }
 
-      /* "ext_modules/io_funcs.pyx":541
+      /* "ext_modules/io_funcs.pyx":545
  *                 swapbytes(buf, PBsview[j])
  * 
  *             if datatype == b'D':             # <<<<<<<<<<<<<<
  *                 memcpy(<void*>(&value_double), <void*>buf, PBsview[j])
  *                 data_view[i, j] = <float>value_double
  */
       switch (__pyx_v_datatype) {
         case 'D':
 
-        /* "ext_modules/io_funcs.pyx":542
+        /* "ext_modules/io_funcs.pyx":546
  * 
  *             if datatype == b'D':
  *                 memcpy(<void*>(&value_double), <void*>buf, PBsview[j])             # <<<<<<<<<<<<<<
  *                 data_view[i, j] = <float>value_double
  *             elif datatype == b'F':
  */
         __pyx_t_10 = __pyx_v_j;
         (void)(memcpy(((void *)(&__pyx_v_value_double)), ((void *)__pyx_v_buf), (*((int *) ( /* dim=0 */ (__pyx_v_PBsview.data + __pyx_t_10 * __pyx_v_PBsview.strides[0]) )))));
 
-        /* "ext_modules/io_funcs.pyx":543
+        /* "ext_modules/io_funcs.pyx":547
  *             if datatype == b'D':
  *                 memcpy(<void*>(&value_double), <void*>buf, PBsview[j])
  *                 data_view[i, j] = <float>value_double             # <<<<<<<<<<<<<<
  *             elif datatype == b'F':
  *                 memcpy(<void*>(&data_view[i, j]), <void*>buf, PBsview[j])
  */
         __pyx_t_10 = __pyx_v_i;
         __pyx_t_32 = __pyx_v_j;
         *((float *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_data_view.data + __pyx_t_10 * __pyx_v_data_view.strides[0]) ) + __pyx_t_32 * __pyx_v_data_view.strides[1]) )) = ((float)__pyx_v_value_double);
 
-        /* "ext_modules/io_funcs.pyx":541
+        /* "ext_modules/io_funcs.pyx":545
  *                 swapbytes(buf, PBsview[j])
  * 
  *             if datatype == b'D':             # <<<<<<<<<<<<<<
  *                 memcpy(<void*>(&value_double), <void*>buf, PBsview[j])
  *                 data_view[i, j] = <float>value_double
  */
         break;
         case 'F':
 
-        /* "ext_modules/io_funcs.pyx":545
+        /* "ext_modules/io_funcs.pyx":549
  *                 data_view[i, j] = <float>value_double
  *             elif datatype == b'F':
  *                 memcpy(<void*>(&data_view[i, j]), <void*>buf, PBsview[j])             # <<<<<<<<<<<<<<
  *             else:
  *                 if datatype == b'I':
  */
         __pyx_t_32 = __pyx_v_i;
         __pyx_t_10 = __pyx_v_j;
         __pyx_t_33 = __pyx_v_j;
         (void)(memcpy(((void *)(&(*((float *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_data_view.data + __pyx_t_32 * __pyx_v_data_view.strides[0]) ) + __pyx_t_10 * __pyx_v_data_view.strides[1]) ))))), ((void *)__pyx_v_buf), (*((int *) ( /* dim=0 */ (__pyx_v_PBsview.data + __pyx_t_33 * __pyx_v_PBsview.strides[0]) )))));
 
-        /* "ext_modules/io_funcs.pyx":544
+        /* "ext_modules/io_funcs.pyx":548
  *                 memcpy(<void*>(&value_double), <void*>buf, PBsview[j])
  *                 data_view[i, j] = <float>value_double
  *             elif datatype == b'F':             # <<<<<<<<<<<<<<
  *                 memcpy(<void*>(&data_view[i, j]), <void*>buf, PBsview[j])
  *             else:
  */
         break;
         default:
 
-        /* "ext_modules/io_funcs.pyx":547
+        /* "ext_modules/io_funcs.pyx":551
  *                 memcpy(<void*>(&data_view[i, j]), <void*>buf, PBsview[j])
  *             else:
  *                 if datatype == b'I':             # <<<<<<<<<<<<<<
  *                     memcpy(<void*>(&value_int), <void*>buf, PBsview[j])
  *                     value_int = value_int & bmview[j] # masking undefined bits
  */
         __pyx_t_2 = ((__pyx_v_datatype == 'I') != 0);
         if (__pyx_t_2) {
 
-          /* "ext_modules/io_funcs.pyx":548
+          /* "ext_modules/io_funcs.pyx":552
  *             else:
  *                 if datatype == b'I':
  *                     memcpy(<void*>(&value_int), <void*>buf, PBsview[j])             # <<<<<<<<<<<<<<
  *                     value_int = value_int & bmview[j] # masking undefined bits
  *                 else:
  */
           __pyx_t_33 = __pyx_v_j;
           (void)(memcpy(((void *)(&__pyx_v_value_int)), ((void *)__pyx_v_buf), (*((int *) ( /* dim=0 */ (__pyx_v_PBsview.data + __pyx_t_33 * __pyx_v_PBsview.strides[0]) )))));
 
-          /* "ext_modules/io_funcs.pyx":549
+          /* "ext_modules/io_funcs.pyx":553
  *                 if datatype == b'I':
  *                     memcpy(<void*>(&value_int), <void*>buf, PBsview[j])
  *                     value_int = value_int & bmview[j] # masking undefined bits             # <<<<<<<<<<<<<<
  *                 else:
  *                     # datatype must be 'A'
  */
           __pyx_t_33 = __pyx_v_j;
           __pyx_v_value_int = (__pyx_v_value_int & (*((int *) ( /* dim=0 */ (__pyx_v_bmview.data + __pyx_t_33 * __pyx_v_bmview.strides[0]) ))));
 
-          /* "ext_modules/io_funcs.pyx":547
+          /* "ext_modules/io_funcs.pyx":551
  *                 memcpy(<void*>(&data_view[i, j]), <void*>buf, PBsview[j])
  *             else:
  *                 if datatype == b'I':             # <<<<<<<<<<<<<<
  *                     memcpy(<void*>(&value_int), <void*>buf, PBsview[j])
  *                     value_int = value_int & bmview[j] # masking undefined bits
  */
           goto __pyx_L103;
         }
 
-        /* "ext_modules/io_funcs.pyx":552
+        /* "ext_modules/io_funcs.pyx":556
  *                 else:
  *                     # datatype must be 'A'
  *                     value_int = 0             # <<<<<<<<<<<<<<
  *                     for k in range(PBsview[j]):
  *                         value_int = value_int * 10 + ((<char>buf[k]) - b'0')
  */
         /*else*/ {
           __pyx_v_value_int = 0;
 
-          /* "ext_modules/io_funcs.pyx":553
+          /* "ext_modules/io_funcs.pyx":557
  *                     # datatype must be 'A'
  *                     value_int = 0
  *                     for k in range(PBsview[j]):             # <<<<<<<<<<<<<<
  *                         value_int = value_int * 10 + ((<char>buf[k]) - b'0')
  * 
  */
           __pyx_t_33 = __pyx_v_j;
           __pyx_t_34 = (*((int *) ( /* dim=0 */ (__pyx_v_PBsview.data + __pyx_t_33 * __pyx_v_PBsview.strides[0]) )));
           __pyx_t_35 = __pyx_t_34;
           for (__pyx_t_24 = 0; __pyx_t_24 < __pyx_t_35; __pyx_t_24+=1) {
             __pyx_v_k = __pyx_t_24;
 
-            /* "ext_modules/io_funcs.pyx":554
+            /* "ext_modules/io_funcs.pyx":558
  *                     value_int = 0
  *                     for k in range(PBsview[j]):
  *                         value_int = value_int * 10 + ((<char>buf[k]) - b'0')             # <<<<<<<<<<<<<<
  * 
  *                 if ldview[j] == 0.0 and lvview[j] == 0.0:
  */
-            __pyx_t_8 = __Pyx_PyInt_From_long((__pyx_v_value_int * 10)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 554, __pyx_L1_error)
+            __pyx_t_8 = __Pyx_PyInt_From_long((__pyx_v_value_int * 10)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 558, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_8);
-            __pyx_t_7 = __Pyx_PyInt_From_char(((char)(__pyx_v_buf[__pyx_v_k]))); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 554, __pyx_L1_error)
+            __pyx_t_7 = __Pyx_PyInt_From_char(((char)(__pyx_v_buf[__pyx_v_k]))); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 558, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_7);
-            __pyx_t_3 = PyNumber_Subtract(__pyx_t_7, __pyx_kp_b_0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 554, __pyx_L1_error)
+            __pyx_t_3 = PyNumber_Subtract(__pyx_t_7, __pyx_kp_b_0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 558, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_3);
             __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-            __pyx_t_7 = PyNumber_Add(__pyx_t_8, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 554, __pyx_L1_error)
+            __pyx_t_7 = PyNumber_Add(__pyx_t_8, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 558, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_7);
             __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
             __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-            __pyx_t_36 = __Pyx_PyInt_As_int(__pyx_t_7); if (unlikely((__pyx_t_36 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 554, __pyx_L1_error)
+            __pyx_t_36 = __Pyx_PyInt_As_int(__pyx_t_7); if (unlikely((__pyx_t_36 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 558, __pyx_L1_error)
             __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
             __pyx_v_value_int = __pyx_t_36;
           }
         }
         __pyx_L103:;
 
-        /* "ext_modules/io_funcs.pyx":556
+        /* "ext_modules/io_funcs.pyx":560
  *                         value_int = value_int * 10 + ((<char>buf[k]) - b'0')
  * 
  *                 if ldview[j] == 0.0 and lvview[j] == 0.0:             # <<<<<<<<<<<<<<
  *                     data_view[i, j] = <float>value_int
  *                 else:
  */
         __pyx_t_33 = __pyx_v_j;
@@ -25200,112 +25315,112 @@
         }
         __pyx_t_33 = __pyx_v_j;
         __pyx_t_1 = (((*((float *) ( /* dim=0 */ (__pyx_v_lvview.data + __pyx_t_33 * __pyx_v_lvview.strides[0]) ))) == 0.0) != 0);
         __pyx_t_2 = __pyx_t_1;
         __pyx_L107_bool_binop_done:;
         if (__pyx_t_2) {
 
-          /* "ext_modules/io_funcs.pyx":557
+          /* "ext_modules/io_funcs.pyx":561
  * 
  *                 if ldview[j] == 0.0 and lvview[j] == 0.0:
  *                     data_view[i, j] = <float>value_int             # <<<<<<<<<<<<<<
  *                 else:
  *                     data_view[i, j] = (<float>pow(10.0, ldview[j] * value_int / PRsview[j])) * lvview[j]
  */
           __pyx_t_33 = __pyx_v_i;
           __pyx_t_10 = __pyx_v_j;
           *((float *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_data_view.data + __pyx_t_33 * __pyx_v_data_view.strides[0]) ) + __pyx_t_10 * __pyx_v_data_view.strides[1]) )) = ((float)__pyx_v_value_int);
 
-          /* "ext_modules/io_funcs.pyx":556
+          /* "ext_modules/io_funcs.pyx":560
  *                         value_int = value_int * 10 + ((<char>buf[k]) - b'0')
  * 
  *                 if ldview[j] == 0.0 and lvview[j] == 0.0:             # <<<<<<<<<<<<<<
  *                     data_view[i, j] = <float>value_int
  *                 else:
  */
           goto __pyx_L106;
         }
 
-        /* "ext_modules/io_funcs.pyx":559
+        /* "ext_modules/io_funcs.pyx":563
  *                     data_view[i, j] = <float>value_int
  *                 else:
  *                     data_view[i, j] = (<float>pow(10.0, ldview[j] * value_int / PRsview[j])) * lvview[j]             # <<<<<<<<<<<<<<
  * 
  *             buf += PBsview[j]
  */
         /*else*/ {
           __pyx_t_10 = __pyx_v_j;
           __pyx_t_37 = ((*((float *) ( /* dim=0 */ (__pyx_v_ldview.data + __pyx_t_10 * __pyx_v_ldview.strides[0]) ))) * __pyx_v_value_int);
           __pyx_t_10 = __pyx_v_j;
           __pyx_t_34 = (*((int *) ( /* dim=0 */ (__pyx_v_PRsview.data + __pyx_t_10 * __pyx_v_PRsview.strides[0]) )));
           if (unlikely(__pyx_t_34 == 0)) {
             PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-            __PYX_ERR(0, 559, __pyx_L1_error)
+            __PYX_ERR(0, 563, __pyx_L1_error)
           }
           __pyx_t_10 = __pyx_v_j;
           __pyx_t_33 = __pyx_v_i;
           __pyx_t_32 = __pyx_v_j;
           *((float *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_data_view.data + __pyx_t_33 * __pyx_v_data_view.strides[0]) ) + __pyx_t_32 * __pyx_v_data_view.strides[1]) )) = (((float)pow(10.0, (__pyx_t_37 / ((float)__pyx_t_34)))) * (*((float *) ( /* dim=0 */ (__pyx_v_lvview.data + __pyx_t_10 * __pyx_v_lvview.strides[0]) ))));
         }
         __pyx_L106:;
         break;
       }
 
-      /* "ext_modules/io_funcs.pyx":561
+      /* "ext_modules/io_funcs.pyx":565
  *                     data_view[i, j] = (<float>pow(10.0, ldview[j] * value_int / PRsview[j])) * lvview[j]
  * 
  *             buf += PBsview[j]             # <<<<<<<<<<<<<<
  * 
  *     free(bytes_buffer)
  */
       __pyx_t_10 = __pyx_v_j;
       __pyx_v_buf = (__pyx_v_buf + (*((int *) ( /* dim=0 */ (__pyx_v_PBsview.data + __pyx_t_10 * __pyx_v_PBsview.strides[0]) ))));
     }
   }
 
-  /* "ext_modules/io_funcs.pyx":563
+  /* "ext_modules/io_funcs.pyx":567
  *             buf += PBsview[j]
  * 
  *     free(bytes_buffer)             # <<<<<<<<<<<<<<
  *     fclose(fi)
  * 
  */
   free(__pyx_v_bytes_buffer);
 
-  /* "ext_modules/io_funcs.pyx":564
+  /* "ext_modules/io_funcs.pyx":568
  * 
  *     free(bytes_buffer)
  *     fclose(fi)             # <<<<<<<<<<<<<<
  * 
  *     return feature_metadata, data, metadata
  */
   (void)(fclose(__pyx_v_fi));
 
-  /* "ext_modules/io_funcs.pyx":566
+  /* "ext_modules/io_funcs.pyx":570
  *     fclose(fi)
  * 
  *     return feature_metadata, data, metadata             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_7 = PyTuple_New(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 566, __pyx_L1_error)
+  __pyx_t_7 = PyTuple_New(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 570, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_INCREF(__pyx_v_feature_metadata);
   __Pyx_GIVEREF(__pyx_v_feature_metadata);
   PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_v_feature_metadata);
   __Pyx_INCREF(__pyx_v_data);
   __Pyx_GIVEREF(__pyx_v_data);
   PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_v_data);
   __Pyx_INCREF(__pyx_v_metadata);
   __Pyx_GIVEREF(__pyx_v_metadata);
   PyTuple_SET_ITEM(__pyx_t_7, 2, __pyx_v_metadata);
   __pyx_r = ((PyObject*)__pyx_t_7);
   __pyx_t_7 = 0;
   goto __pyx_L0;
 
-  /* "ext_modules/io_funcs.pyx":241
+  /* "ext_modules/io_funcs.pyx":245
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef tuple read_fcs(char* fcs_file):             # <<<<<<<<<<<<<<
  *     """ This function is inspired by the python package fcsparser (https://github.com/eyurtsev/fcsparser)
  *     """
  */
 
@@ -25367,15 +25482,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("read_fcs (wrapper)", 0);
   assert(__pyx_arg_fcs_file); {
-    __pyx_v_fcs_file = __Pyx_PyObject_AsWritableString(__pyx_arg_fcs_file); if (unlikely((!__pyx_v_fcs_file) && PyErr_Occurred())) __PYX_ERR(0, 241, __pyx_L3_error)
+    __pyx_v_fcs_file = __Pyx_PyObject_AsWritableString(__pyx_arg_fcs_file); if (unlikely((!__pyx_v_fcs_file) && PyErr_Occurred())) __PYX_ERR(0, 245, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("pegasusio.cylib.io.read_fcs", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -25391,15 +25506,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("read_fcs", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_9pegasusio_5cylib_2io_read_fcs(__pyx_v_fcs_file, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 241, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9pegasusio_5cylib_2io_read_fcs(__pyx_v_fcs_file, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 245, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -25611,15 +25726,15 @@
     /* "View.MemoryView":134
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if itemsize <= 0:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__60, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 134, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__61, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 134, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 134, __pyx_L1_error)
 
     /* "View.MemoryView":133
  *         self.itemsize = itemsize
@@ -25643,15 +25758,15 @@
     /* "View.MemoryView":137
  * 
  *         if itemsize <= 0:
  *             raise ValueError("itemsize <= 0 for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if not isinstance(format, bytes):
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__61, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 137, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__62, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 137, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 137, __pyx_L1_error)
 
     /* "View.MemoryView":136
  *             raise ValueError("Empty shape tuple for cython.array")
@@ -25712,15 +25827,15 @@
   /* "View.MemoryView":141
  *         if not isinstance(format, bytes):
  *             format = format.encode('ASCII')
  *         self._format = format  # keep a reference to the byte string             # <<<<<<<<<<<<<<
  *         self.format = self._format
  * 
  */
-  if (!(likely(PyBytes_CheckExact(__pyx_v_format))||((__pyx_v_format) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_v_format)->tp_name), 0))) __PYX_ERR(1, 141, __pyx_L1_error)
+  if (!(likely(PyBytes_CheckExact(__pyx_v_format))||((__pyx_v_format) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_v_format)->tp_name), 0))) __PYX_ERR(1, 141, __pyx_L1_error)
   __pyx_t_3 = __pyx_v_format;
   __Pyx_INCREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __Pyx_GOTREF(__pyx_v_self->_format);
   __Pyx_DECREF(__pyx_v_self->_format);
   __pyx_v_self->_format = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
@@ -25770,15 +25885,15 @@
     /* "View.MemoryView":149
  * 
  *         if not self._shape:
  *             raise MemoryError("unable to allocate shape and strides.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__62, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 149, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__63, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 149, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 149, __pyx_L1_error)
 
     /* "View.MemoryView":148
  *         self._strides = self._shape + self.ndim
@@ -26044,15 +26159,15 @@
       /* "View.MemoryView":177
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:
  *                 raise MemoryError("unable to allocate array data.")             # <<<<<<<<<<<<<<
  * 
  *             if self.dtype_is_object:
  */
-      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__63, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 177, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__64, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 177, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_Raise(__pyx_t_10, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __PYX_ERR(1, 177, __pyx_L1_error)
 
       /* "View.MemoryView":176
  * 
@@ -26288,15 +26403,15 @@
     /* "View.MemoryView":193
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")             # <<<<<<<<<<<<<<
  *         info.buf = self.data
  *         info.len = self.len
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__64, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 193, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__65, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 193, __pyx_L1_error)
 
     /* "View.MemoryView":192
  *         elif self.mode == u"fortran":
@@ -27022,15 +27137,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__65, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__66, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -27078,15 +27193,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__66, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__67, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -27690,15 +27805,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_Enum, (type(self), 0xb068931, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_Enum__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_unpickle_Enum__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_Enum, (type(self), 0xb068931, state)
@@ -28807,15 +28922,15 @@
     /* "View.MemoryView":420
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__67, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 420, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__68, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 420, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(1, 420, __pyx_L1_error)
 
     /* "View.MemoryView":419
  * 
@@ -29855,15 +29970,15 @@
       /* "View.MemoryView":497
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
-      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__68, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 497, __pyx_L5_except_error)
+      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__69, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 497, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __PYX_ERR(1, 497, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
@@ -29993,15 +30108,15 @@
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 512, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 512, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 512, __pyx_L1_error)
     __pyx_v_bytesvalue = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
 
     /* "View.MemoryView":511
  *         cdef Py_ssize_t i
  * 
  *         if isinstance(value, tuple):             # <<<<<<<<<<<<<<
@@ -30066,15 +30181,15 @@
       PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_v_value);
       __pyx_t_1 = 0;
       __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 514, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 514, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 514, __pyx_L1_error)
     __pyx_v_bytesvalue = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
   }
   __pyx_L3:;
 
   /* "View.MemoryView":516
  *             bytesvalue = struct.pack(self.view.format, value)
@@ -30217,15 +30332,15 @@
     /* "View.MemoryView":522
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__69, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 522, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__70, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 522, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 522, __pyx_L1_error)
 
     /* "View.MemoryView":521
  *     @cname('getbuffer')
@@ -30766,15 +30881,15 @@
     /* "View.MemoryView":572
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__70, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 572, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__71, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 572, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(1, 572, __pyx_L1_error)
 
     /* "View.MemoryView":570
  *     @property
@@ -30883,15 +30998,15 @@
  *             return (-1,) * self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__71, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 579, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__72, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
     /* "View.MemoryView":578
@@ -31921,15 +32036,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__72, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__73, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -31977,15 +32092,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__73, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__74, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -32334,17 +32449,17 @@
  *             else:
  */
         __pyx_t_8 = PyObject_Length(__pyx_v_tup); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(1, 684, __pyx_L1_error)
         __pyx_t_7 = PyList_New(1 * ((((__pyx_v_ndim - __pyx_t_8) + 1)<0) ? 0:((__pyx_v_ndim - __pyx_t_8) + 1))); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 684, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         { Py_ssize_t __pyx_temp;
           for (__pyx_temp=0; __pyx_temp < ((__pyx_v_ndim - __pyx_t_8) + 1); __pyx_temp++) {
-            __Pyx_INCREF(__pyx_slice__74);
-            __Pyx_GIVEREF(__pyx_slice__74);
-            PyList_SET_ITEM(__pyx_t_7, __pyx_temp, __pyx_slice__74);
+            __Pyx_INCREF(__pyx_slice__75);
+            __Pyx_GIVEREF(__pyx_slice__75);
+            PyList_SET_ITEM(__pyx_t_7, __pyx_temp, __pyx_slice__75);
           }
         }
         __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_7); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 684, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
         /* "View.MemoryView":685
  *             if not seen_ellipsis:
@@ -32369,15 +32484,15 @@
  *                 seen_ellipsis = True
  *             else:
  *                 result.append(slice(None))             # <<<<<<<<<<<<<<
  *             have_slices = True
  *         else:
  */
       /*else*/ {
-        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_slice__74); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 687, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_slice__75); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 687, __pyx_L1_error)
       }
       __pyx_L7:;
 
       /* "View.MemoryView":688
  *             else:
  *                 result.append(slice(None))
  *             have_slices = True             # <<<<<<<<<<<<<<
@@ -32509,17 +32624,17 @@
  * 
  *     return have_slices or nslices, tuple(result)
  */
     __pyx_t_3 = PyList_New(1 * ((__pyx_v_nslices<0) ? 0:__pyx_v_nslices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 698, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     { Py_ssize_t __pyx_temp;
       for (__pyx_temp=0; __pyx_temp < __pyx_v_nslices; __pyx_temp++) {
-        __Pyx_INCREF(__pyx_slice__74);
-        __Pyx_GIVEREF(__pyx_slice__74);
-        PyList_SET_ITEM(__pyx_t_3, __pyx_temp, __pyx_slice__74);
+        __Pyx_INCREF(__pyx_slice__75);
+        __Pyx_GIVEREF(__pyx_slice__75);
+        PyList_SET_ITEM(__pyx_t_3, __pyx_temp, __pyx_slice__75);
       }
     }
     __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_3); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 698, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     /* "View.MemoryView":697
  * 
@@ -32638,15 +32753,15 @@
       /* "View.MemoryView":705
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__75, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 705, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__76, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 705, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_Raise(__pyx_t_5, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __PYX_ERR(1, 705, __pyx_L1_error)
 
       /* "View.MemoryView":704
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
@@ -34822,15 +34937,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__76, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__77, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -34878,15 +34993,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__77, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__78, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -38155,15 +38270,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xb068931, 0x82a3537, 0x6ae9995):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__78, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__79, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xb068931, 0x82a3537, 0x6ae9995):
@@ -38269,15 +38384,15 @@
     /* "(tree fragment)":9
  *     __pyx_result = Enum.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Enum__set_state(<Enum> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_Enum__set_state(Enum __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
     __pyx_t_4 = __pyx_unpickle_Enum__set_state(((struct __pyx_MemviewEnum_obj *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
  *     __pyx_result = Enum.__new__(__pyx_type)
@@ -39311,25 +39426,26 @@
   {&__pyx_kp_u_Warning_Detected_more_than_one_d, __pyx_k_Warning_Detected_more_than_one_d, sizeof(__pyx_k_Warning_Detected_more_than_one_d), 0, 1, 0, 0},
   {&__pyx_kp_u_Warning_P, __pyx_k_Warning_P, sizeof(__pyx_k_Warning_P), 0, 1, 0, 0},
   {&__pyx_kp_u_Warning_detected_f2_0_for_P, __pyx_k_Warning_detected_f2_0_for_P, sizeof(__pyx_k_Warning_detected_f2_0_for_P), 0, 1, 0, 0},
   {&__pyx_kp_u_We_require_f1_0_for_PnE_f1_f2, __pyx_k_We_require_f1_0_for_PnE_f1_f2, sizeof(__pyx_k_We_require_f1_0_for_PnE_f1_f2), 0, 1, 0, 0},
   {&__pyx_kp_s__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 0, 1, 0},
   {&__pyx_kp_u__22, __pyx_k__22, sizeof(__pyx_k__22), 0, 1, 0, 0},
   {&__pyx_kp_u__23, __pyx_k__23, sizeof(__pyx_k__23), 0, 1, 0, 0},
-  {&__pyx_kp_u__25, __pyx_k__25, sizeof(__pyx_k__25), 0, 1, 0, 0},
-  {&__pyx_kp_u__41, __pyx_k__41, sizeof(__pyx_k__41), 0, 1, 0, 0},
+  {&__pyx_kp_u__24, __pyx_k__24, sizeof(__pyx_k__24), 0, 1, 0, 0},
+  {&__pyx_kp_u__26, __pyx_k__26, sizeof(__pyx_k__26), 0, 1, 0, 0},
   {&__pyx_kp_u__42, __pyx_k__42, sizeof(__pyx_k__42), 0, 1, 0, 0},
   {&__pyx_kp_u__43, __pyx_k__43, sizeof(__pyx_k__43), 0, 1, 0, 0},
+  {&__pyx_kp_u__44, __pyx_k__44, sizeof(__pyx_k__44), 0, 1, 0, 0},
   {&__pyx_kp_u__5, __pyx_k__5, sizeof(__pyx_k__5), 0, 1, 0, 0},
-  {&__pyx_kp_u__54, __pyx_k__54, sizeof(__pyx_k__54), 0, 1, 0, 0},
   {&__pyx_kp_u__55, __pyx_k__55, sizeof(__pyx_k__55), 0, 1, 0, 0},
   {&__pyx_kp_u__56, __pyx_k__56, sizeof(__pyx_k__56), 0, 1, 0, 0},
   {&__pyx_kp_u__57, __pyx_k__57, sizeof(__pyx_k__57), 0, 1, 0, 0},
   {&__pyx_kp_u__58, __pyx_k__58, sizeof(__pyx_k__58), 0, 1, 0, 0},
   {&__pyx_kp_u__59, __pyx_k__59, sizeof(__pyx_k__59), 0, 1, 0, 0},
+  {&__pyx_kp_u__60, __pyx_k__60, sizeof(__pyx_k__60), 0, 1, 0, 0},
   {&__pyx_n_s_allocate_buffer, __pyx_k_allocate_buffer, sizeof(__pyx_k_allocate_buffer), 0, 0, 1, 1},
   {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
   {&__pyx_n_s_array, __pyx_k_array, sizeof(__pyx_k_array), 0, 0, 1, 1},
   {&__pyx_n_s_barcodes, __pyx_k_barcodes, sizeof(__pyx_k_barcodes), 0, 0, 1, 1},
   {&__pyx_n_s_base, __pyx_k_base, sizeof(__pyx_k_base), 0, 0, 1, 1},
   {&__pyx_kp_u_be_no_more_than_4_bytes_for_DAT, __pyx_k_be_no_more_than_4_bytes_for_DAT, sizeof(__pyx_k_be_no_more_than_4_bytes_for_DAT), 0, 1, 0, 0},
   {&__pyx_n_u_big, __pyx_k_big, sizeof(__pyx_k_big), 0, 1, 0, 1},
@@ -39508,18 +39624,18 @@
   {&__pyx_n_s_zeros, __pyx_k_zeros, sizeof(__pyx_k_zeros), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 49, __pyx_L1_error)
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 74, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 94, __pyx_L1_error)
-  __pyx_builtin_UnicodeDecodeError = __Pyx_GetBuiltinName(__pyx_n_s_UnicodeDecodeError); if (!__pyx_builtin_UnicodeDecodeError) __PYX_ERR(0, 323, __pyx_L1_error)
-  __pyx_builtin_NotImplementedError = __Pyx_GetBuiltinName(__pyx_n_s_NotImplementedError); if (!__pyx_builtin_NotImplementedError) __PYX_ERR(0, 341, __pyx_L1_error)
-  __pyx_builtin_print = __Pyx_GetBuiltinName(__pyx_n_s_print); if (!__pyx_builtin_print) __PYX_ERR(0, 361, __pyx_L1_error)
-  __pyx_builtin_object = __Pyx_GetBuiltinName(__pyx_n_s_object); if (!__pyx_builtin_object) __PYX_ERR(0, 413, __pyx_L1_error)
+  __pyx_builtin_UnicodeDecodeError = __Pyx_GetBuiltinName(__pyx_n_s_UnicodeDecodeError); if (!__pyx_builtin_UnicodeDecodeError) __PYX_ERR(0, 327, __pyx_L1_error)
+  __pyx_builtin_NotImplementedError = __Pyx_GetBuiltinName(__pyx_n_s_NotImplementedError); if (!__pyx_builtin_NotImplementedError) __PYX_ERR(0, 345, __pyx_L1_error)
+  __pyx_builtin_print = __Pyx_GetBuiltinName(__pyx_n_s_print); if (!__pyx_builtin_print) __PYX_ERR(0, 365, __pyx_L1_error)
+  __pyx_builtin_object = __Pyx_GetBuiltinName(__pyx_n_s_object); if (!__pyx_builtin_object) __PYX_ERR(0, 417, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(1, 149, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(1, 152, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(1, 406, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(1, 615, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(1, 834, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
@@ -39540,417 +39656,418 @@
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_No_matching_signature_found); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
   __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_Function_call_with_ambiguous_arg); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "ext_modules/io_funcs.pyx":283
+  /* "ext_modules/io_funcs.pyx":287
  *     cdef uchar* text_segment
  * 
  *     unicode_source = np.zeros(100000, dtype = np.uint8)             # <<<<<<<<<<<<<<
  * 
  *     cdef uchar[:] sview = unicode_source
  */
-  __pyx_tuple__44 = PyTuple_Pack(1, __pyx_int_100000); if (unlikely(!__pyx_tuple__44)) __PYX_ERR(0, 283, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__44);
-  __Pyx_GIVEREF(__pyx_tuple__44);
+  __pyx_tuple__45 = PyTuple_Pack(1, __pyx_int_100000); if (unlikely(!__pyx_tuple__45)) __PYX_ERR(0, 287, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__45);
+  __Pyx_GIVEREF(__pyx_tuple__45);
 
-  /* "ext_modules/io_funcs.pyx":318
+  /* "ext_modules/io_funcs.pyx":322
  *                     free(text_segment)
  *                     fclose(fi)
  *                     raise ValueError("Keywords and keyword values must have lengths greater than zero!")             # <<<<<<<<<<<<<<
  * 
  *                 value_bytes = bytes(unicode_source[0:s_pos])
  */
-  __pyx_tuple__45 = PyTuple_Pack(1, __pyx_kp_u_Keywords_and_keyword_values_must); if (unlikely(!__pyx_tuple__45)) __PYX_ERR(0, 318, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__45);
-  __Pyx_GIVEREF(__pyx_tuple__45);
+  __pyx_tuple__46 = PyTuple_Pack(1, __pyx_kp_u_Keywords_and_keyword_values_must); if (unlikely(!__pyx_tuple__46)) __PYX_ERR(0, 322, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__46);
+  __Pyx_GIVEREF(__pyx_tuple__46);
 
-  /* "ext_modules/io_funcs.pyx":341
+  /* "ext_modules/io_funcs.pyx":345
  *             free(text_segment)
  *             fclose(fi)
  *             raise NotImplementedError("Keyword or keyward value length cannot exceed 10,000!")             # <<<<<<<<<<<<<<
  * 
  *     free(text_segment)
  */
-  __pyx_tuple__46 = PyTuple_Pack(1, __pyx_kp_u_Keyword_or_keyward_value_length); if (unlikely(!__pyx_tuple__46)) __PYX_ERR(0, 341, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__46);
-  __Pyx_GIVEREF(__pyx_tuple__46);
+  __pyx_tuple__47 = PyTuple_Pack(1, __pyx_kp_u_Keyword_or_keyward_value_length); if (unlikely(!__pyx_tuple__47)) __PYX_ERR(0, 345, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__47);
+  __Pyx_GIVEREF(__pyx_tuple__47);
 
-  /* "ext_modules/io_funcs.pyx":361
+  /* "ext_modules/io_funcs.pyx":365
  *         data_end = _end
  *     if data_start == 0:
  *         print("Warning: Could not detect a DATA segment!")             # <<<<<<<<<<<<<<
  * 
  *     _start = _end = 0
  */
-  __pyx_tuple__47 = PyTuple_Pack(1, __pyx_kp_u_Warning_Could_not_detect_a_DATA); if (unlikely(!__pyx_tuple__47)) __PYX_ERR(0, 361, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__47);
-  __Pyx_GIVEREF(__pyx_tuple__47);
+  __pyx_tuple__48 = PyTuple_Pack(1, __pyx_kp_u_Warning_Could_not_detect_a_DATA); if (unlikely(!__pyx_tuple__48)) __PYX_ERR(0, 365, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__48);
+  __Pyx_GIVEREF(__pyx_tuple__48);
 
-  /* "ext_modules/io_funcs.pyx":372
+  /* "ext_modules/io_funcs.pyx":376
  *         analysis_end = _end
  *     if analysis_start > 0:
  *         print("Warning: ANALYSIS segment would be omitted since current implementation does not support parsing of this segment.")             # <<<<<<<<<<<<<<
  * 
  *     if "$BEGINSTEXT" in metadata:
  */
-  __pyx_tuple__48 = PyTuple_Pack(1, __pyx_kp_u_Warning_ANALYSIS_segment_would_b); if (unlikely(!__pyx_tuple__48)) __PYX_ERR(0, 372, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__48);
-  __Pyx_GIVEREF(__pyx_tuple__48);
+  __pyx_tuple__49 = PyTuple_Pack(1, __pyx_kp_u_Warning_ANALYSIS_segment_would_b); if (unlikely(!__pyx_tuple__49)) __PYX_ERR(0, 376, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__49);
+  __Pyx_GIVEREF(__pyx_tuple__49);
 
-  /* "ext_modules/io_funcs.pyx":376
+  /* "ext_modules/io_funcs.pyx":380
  *     if "$BEGINSTEXT" in metadata:
  *         if metadata.pop("$BEGINSTEXT") != "0":
  *             print("Warning: Detected a supplemental TEXT segment. This segment will be ignored under current implementation.")             # <<<<<<<<<<<<<<
  *     if "$ENDSTEXT" in metadata:
  *         del metadata["$ENDSTEXT"]
  */
-  __pyx_tuple__49 = PyTuple_Pack(1, __pyx_kp_u_Warning_Detected_a_supplemental); if (unlikely(!__pyx_tuple__49)) __PYX_ERR(0, 376, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__49);
-  __Pyx_GIVEREF(__pyx_tuple__49);
+  __pyx_tuple__50 = PyTuple_Pack(1, __pyx_kp_u_Warning_Detected_a_supplemental); if (unlikely(!__pyx_tuple__50)) __PYX_ERR(0, 380, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__50);
+  __Pyx_GIVEREF(__pyx_tuple__50);
 
-  /* "ext_modules/io_funcs.pyx":388
+  /* "ext_modules/io_funcs.pyx":392
  *     cdef str keyword, tmpstr
  * 
  *     for keyword in ["$NEXTDATA", "$MODE", "$PAR", "$TOT", "$BYTEORD", "$DATATYPE"]:             # <<<<<<<<<<<<<<
  *         if keyword not in metadata:
  *             fclose(fi)
  */
-  __pyx_tuple__50 = PyTuple_Pack(6, __pyx_kp_u_NEXTDATA, __pyx_kp_u_MODE, __pyx_kp_u_PAR, __pyx_kp_u_TOT, __pyx_kp_u_BYTEORD, __pyx_kp_u_DATATYPE); if (unlikely(!__pyx_tuple__50)) __PYX_ERR(0, 388, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__50);
-  __Pyx_GIVEREF(__pyx_tuple__50);
+  __pyx_tuple__51 = PyTuple_Pack(6, __pyx_kp_u_NEXTDATA, __pyx_kp_u_MODE, __pyx_kp_u_PAR, __pyx_kp_u_TOT, __pyx_kp_u_BYTEORD, __pyx_kp_u_DATATYPE); if (unlikely(!__pyx_tuple__51)) __PYX_ERR(0, 392, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__51);
+  __Pyx_GIVEREF(__pyx_tuple__51);
 
-  /* "ext_modules/io_funcs.pyx":394
+  /* "ext_modules/io_funcs.pyx":398
  * 
  *     if metadata.pop("$NEXTDATA") != "0":
  *         print("Warning: Detected more than one data sets. Current implementation will only parse the first data set.")             # <<<<<<<<<<<<<<
  * 
  *     if metadata.pop("$MODE") != "L":
  */
-  __pyx_tuple__51 = PyTuple_Pack(1, __pyx_kp_u_Warning_Detected_more_than_one_d); if (unlikely(!__pyx_tuple__51)) __PYX_ERR(0, 394, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__51);
-  __Pyx_GIVEREF(__pyx_tuple__51);
+  __pyx_tuple__52 = PyTuple_Pack(1, __pyx_kp_u_Warning_Detected_more_than_one_d); if (unlikely(!__pyx_tuple__52)) __PYX_ERR(0, 398, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__52);
+  __Pyx_GIVEREF(__pyx_tuple__52);
 
-  /* "ext_modules/io_funcs.pyx":398
+  /* "ext_modules/io_funcs.pyx":402
  *     if metadata.pop("$MODE") != "L":
  *         fclose(fi)
  *         raise NotImplementedError("Current implementation can only handle $MODE = L!")             # <<<<<<<<<<<<<<
  * 
  *     endian = "little"
  */
-  __pyx_tuple__52 = PyTuple_Pack(1, __pyx_kp_u_Current_implementation_can_only); if (unlikely(!__pyx_tuple__52)) __PYX_ERR(0, 398, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__52);
-  __Pyx_GIVEREF(__pyx_tuple__52);
+  __pyx_tuple__53 = PyTuple_Pack(1, __pyx_kp_u_Current_implementation_can_only); if (unlikely(!__pyx_tuple__53)) __PYX_ERR(0, 402, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__53);
+  __Pyx_GIVEREF(__pyx_tuple__53);
 
-  /* "ext_modules/io_funcs.pyx":436
+  /* "ext_modules/io_funcs.pyx":440
  * 
  *     for i in range(1, M + 1):
  *         for tmpstr in ["B", "E", "N", "R"]:             # <<<<<<<<<<<<<<
  *             keyword = f"$P{i}{tmpstr}"
  *             if keyword not in metadata:
  */
-  __pyx_tuple__53 = PyTuple_Pack(4, __pyx_n_u_B, __pyx_n_u_E, __pyx_n_u_N, __pyx_n_u_R); if (unlikely(!__pyx_tuple__53)) __PYX_ERR(0, 436, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__53);
-  __Pyx_GIVEREF(__pyx_tuple__53);
+  __pyx_tuple__54 = PyTuple_Pack(4, __pyx_n_u_B, __pyx_n_u_E, __pyx_n_u_N, __pyx_n_u_R); if (unlikely(!__pyx_tuple__54)) __PYX_ERR(0, 440, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__54);
+  __Pyx_GIVEREF(__pyx_tuple__54);
 
   /* "View.MemoryView":134
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if itemsize <= 0:
  */
-  __pyx_tuple__60 = PyTuple_Pack(1, __pyx_kp_s_Empty_shape_tuple_for_cython_arr); if (unlikely(!__pyx_tuple__60)) __PYX_ERR(1, 134, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__60);
-  __Pyx_GIVEREF(__pyx_tuple__60);
+  __pyx_tuple__61 = PyTuple_Pack(1, __pyx_kp_s_Empty_shape_tuple_for_cython_arr); if (unlikely(!__pyx_tuple__61)) __PYX_ERR(1, 134, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__61);
+  __Pyx_GIVEREF(__pyx_tuple__61);
 
   /* "View.MemoryView":137
  * 
  *         if itemsize <= 0:
  *             raise ValueError("itemsize <= 0 for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if not isinstance(format, bytes):
  */
-  __pyx_tuple__61 = PyTuple_Pack(1, __pyx_kp_s_itemsize_0_for_cython_array); if (unlikely(!__pyx_tuple__61)) __PYX_ERR(1, 137, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__61);
-  __Pyx_GIVEREF(__pyx_tuple__61);
+  __pyx_tuple__62 = PyTuple_Pack(1, __pyx_kp_s_itemsize_0_for_cython_array); if (unlikely(!__pyx_tuple__62)) __PYX_ERR(1, 137, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__62);
+  __Pyx_GIVEREF(__pyx_tuple__62);
 
   /* "View.MemoryView":149
  * 
  *         if not self._shape:
  *             raise MemoryError("unable to allocate shape and strides.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__62 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_shape_and_str); if (unlikely(!__pyx_tuple__62)) __PYX_ERR(1, 149, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__62);
-  __Pyx_GIVEREF(__pyx_tuple__62);
+  __pyx_tuple__63 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_shape_and_str); if (unlikely(!__pyx_tuple__63)) __PYX_ERR(1, 149, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__63);
+  __Pyx_GIVEREF(__pyx_tuple__63);
 
   /* "View.MemoryView":177
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:
  *                 raise MemoryError("unable to allocate array data.")             # <<<<<<<<<<<<<<
  * 
  *             if self.dtype_is_object:
  */
-  __pyx_tuple__63 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_array_data); if (unlikely(!__pyx_tuple__63)) __PYX_ERR(1, 177, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__63);
-  __Pyx_GIVEREF(__pyx_tuple__63);
+  __pyx_tuple__64 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_array_data); if (unlikely(!__pyx_tuple__64)) __PYX_ERR(1, 177, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__64);
+  __Pyx_GIVEREF(__pyx_tuple__64);
 
   /* "View.MemoryView":193
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")             # <<<<<<<<<<<<<<
  *         info.buf = self.data
  *         info.len = self.len
  */
-  __pyx_tuple__64 = PyTuple_Pack(1, __pyx_kp_s_Can_only_create_a_buffer_that_is); if (unlikely(!__pyx_tuple__64)) __PYX_ERR(1, 193, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__64);
-  __Pyx_GIVEREF(__pyx_tuple__64);
+  __pyx_tuple__65 = PyTuple_Pack(1, __pyx_kp_s_Can_only_create_a_buffer_that_is); if (unlikely(!__pyx_tuple__65)) __PYX_ERR(1, 193, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__65);
+  __Pyx_GIVEREF(__pyx_tuple__65);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__65 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__65)) __PYX_ERR(1, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__65);
-  __Pyx_GIVEREF(__pyx_tuple__65);
+  __pyx_tuple__66 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__66)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__66);
+  __Pyx_GIVEREF(__pyx_tuple__66);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__66 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__66)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__66);
-  __Pyx_GIVEREF(__pyx_tuple__66);
+  __pyx_tuple__67 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__67)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__67);
+  __Pyx_GIVEREF(__pyx_tuple__67);
 
   /* "View.MemoryView":420
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
-  __pyx_tuple__67 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__67)) __PYX_ERR(1, 420, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__67);
-  __Pyx_GIVEREF(__pyx_tuple__67);
+  __pyx_tuple__68 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__68)) __PYX_ERR(1, 420, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__68);
+  __Pyx_GIVEREF(__pyx_tuple__68);
 
   /* "View.MemoryView":497
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
-  __pyx_tuple__68 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__68)) __PYX_ERR(1, 497, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__68);
-  __Pyx_GIVEREF(__pyx_tuple__68);
+  __pyx_tuple__69 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__69)) __PYX_ERR(1, 497, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__69);
+  __Pyx_GIVEREF(__pyx_tuple__69);
 
   /* "View.MemoryView":522
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
-  __pyx_tuple__69 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__69)) __PYX_ERR(1, 522, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__69);
-  __Pyx_GIVEREF(__pyx_tuple__69);
+  __pyx_tuple__70 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__70)) __PYX_ERR(1, 522, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__70);
+  __Pyx_GIVEREF(__pyx_tuple__70);
 
   /* "View.MemoryView":572
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
-  __pyx_tuple__70 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__70)) __PYX_ERR(1, 572, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__70);
-  __Pyx_GIVEREF(__pyx_tuple__70);
+  __pyx_tuple__71 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__71)) __PYX_ERR(1, 572, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__71);
+  __Pyx_GIVEREF(__pyx_tuple__71);
 
   /* "View.MemoryView":579
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
-  __pyx_tuple__71 = PyTuple_New(1); if (unlikely(!__pyx_tuple__71)) __PYX_ERR(1, 579, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__71);
+  __pyx_tuple__72 = PyTuple_New(1); if (unlikely(!__pyx_tuple__72)) __PYX_ERR(1, 579, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__72);
   __Pyx_INCREF(__pyx_int_neg_1);
   __Pyx_GIVEREF(__pyx_int_neg_1);
-  PyTuple_SET_ITEM(__pyx_tuple__71, 0, __pyx_int_neg_1);
-  __Pyx_GIVEREF(__pyx_tuple__71);
+  PyTuple_SET_ITEM(__pyx_tuple__72, 0, __pyx_int_neg_1);
+  __Pyx_GIVEREF(__pyx_tuple__72);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__72 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__72)) __PYX_ERR(1, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__72);
-  __Pyx_GIVEREF(__pyx_tuple__72);
+  __pyx_tuple__73 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__73)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__73);
+  __Pyx_GIVEREF(__pyx_tuple__73);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__73 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__73)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__73);
-  __Pyx_GIVEREF(__pyx_tuple__73);
+  __pyx_tuple__74 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__74)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__74);
+  __Pyx_GIVEREF(__pyx_tuple__74);
 
   /* "View.MemoryView":684
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))             # <<<<<<<<<<<<<<
  *                 seen_ellipsis = True
  *             else:
  */
-  __pyx_slice__74 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__74)) __PYX_ERR(1, 684, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_slice__74);
-  __Pyx_GIVEREF(__pyx_slice__74);
+  __pyx_slice__75 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__75)) __PYX_ERR(1, 684, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_slice__75);
+  __Pyx_GIVEREF(__pyx_slice__75);
 
   /* "View.MemoryView":705
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__75 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__75)) __PYX_ERR(1, 705, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__75);
-  __Pyx_GIVEREF(__pyx_tuple__75);
+  __pyx_tuple__76 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__76)) __PYX_ERR(1, 705, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__76);
+  __Pyx_GIVEREF(__pyx_tuple__76);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__76 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__76)) __PYX_ERR(1, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__76);
-  __Pyx_GIVEREF(__pyx_tuple__76);
+  __pyx_tuple__77 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__77)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__77);
+  __Pyx_GIVEREF(__pyx_tuple__77);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__77 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__77)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__77);
-  __Pyx_GIVEREF(__pyx_tuple__77);
-  __pyx_tuple__78 = PyTuple_Pack(3, __pyx_int_184977713, __pyx_int_136983863, __pyx_int_112105877); if (unlikely(!__pyx_tuple__78)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_tuple__78 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__78)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__78);
   __Pyx_GIVEREF(__pyx_tuple__78);
+  __pyx_tuple__79 = PyTuple_Pack(3, __pyx_int_184977713, __pyx_int_136983863, __pyx_int_112105877); if (unlikely(!__pyx_tuple__79)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__79);
+  __Pyx_GIVEREF(__pyx_tuple__79);
 
   /* "ext_modules/io_funcs.pyx":94
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef void write_mtx(char* mtx_file, data_type[:] data, indices_type[:] indices, indptr_type[:] indptr, int M, int N, int precision = 2):             # <<<<<<<<<<<<<<
  *     """ Input is csr_matrix internal representation, cell by gene; Output will be gene by cell
  *     """
  */
-  __pyx_tuple__79 = PyTuple_Pack(7, __pyx_n_s_mtx_file, __pyx_n_s_data, __pyx_n_s_indices, __pyx_n_s_indptr, __pyx_n_s_M, __pyx_n_s_N, __pyx_n_s_precision); if (unlikely(!__pyx_tuple__79)) __PYX_ERR(0, 94, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__79);
-  __Pyx_GIVEREF(__pyx_tuple__79);
-  __pyx_codeobj__80 = (PyObject*)__Pyx_PyCode_New(7, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__79, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_ext_modules_io_funcs_pyx, __pyx_n_s_pyx_fuse_0_0_0write_mtx, 94, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__80)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_tuple__80 = PyTuple_Pack(7, __pyx_n_s_mtx_file, __pyx_n_s_data, __pyx_n_s_indices, __pyx_n_s_indptr, __pyx_n_s_M, __pyx_n_s_N, __pyx_n_s_precision); if (unlikely(!__pyx_tuple__80)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__80);
+  __Pyx_GIVEREF(__pyx_tuple__80);
+  __pyx_codeobj__81 = (PyObject*)__Pyx_PyCode_New(7, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__80, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_ext_modules_io_funcs_pyx, __pyx_n_s_pyx_fuse_0_0_0write_mtx, 94, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__81)) __PYX_ERR(0, 94, __pyx_L1_error)
 
-  /* "ext_modules/io_funcs.pyx":197
+  /* "ext_modules/io_funcs.pyx":201
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef void write_dense(char* output_file, str[:] barcodes, str[:] features, data_type[:] data, indices_type[:] indices, indptr_type[:] indptr, int M, int N, int precision = 2):             # <<<<<<<<<<<<<<
  *     """ Input must be csr_matrix internal representation, gene by cell (X.T.tocsr()); Output will be gene by cell
  *     """
  */
-  __pyx_tuple__81 = PyTuple_Pack(9, __pyx_n_s_output_file, __pyx_n_s_barcodes, __pyx_n_s_features, __pyx_n_s_data, __pyx_n_s_indices, __pyx_n_s_indptr, __pyx_n_s_M, __pyx_n_s_N, __pyx_n_s_precision); if (unlikely(!__pyx_tuple__81)) __PYX_ERR(0, 197, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__81);
-  __Pyx_GIVEREF(__pyx_tuple__81);
-  __pyx_codeobj__82 = (PyObject*)__Pyx_PyCode_New(9, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__81, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_ext_modules_io_funcs_pyx, __pyx_n_s_pyx_fuse_0_0_0write_dense, 197, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__82)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_tuple__82 = PyTuple_Pack(9, __pyx_n_s_output_file, __pyx_n_s_barcodes, __pyx_n_s_features, __pyx_n_s_data, __pyx_n_s_indices, __pyx_n_s_indptr, __pyx_n_s_M, __pyx_n_s_N, __pyx_n_s_precision); if (unlikely(!__pyx_tuple__82)) __PYX_ERR(0, 201, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__82);
+  __Pyx_GIVEREF(__pyx_tuple__82);
+  __pyx_codeobj__83 = (PyObject*)__Pyx_PyCode_New(9, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__82, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_ext_modules_io_funcs_pyx, __pyx_n_s_pyx_fuse_0_0_0write_dense, 201, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__83)) __PYX_ERR(0, 201, __pyx_L1_error)
 
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_tuple__83 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__83)) __PYX_ERR(1, 287, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__83);
-  __Pyx_GIVEREF(__pyx_tuple__83);
+  __pyx_tuple__84 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__84)) __PYX_ERR(1, 287, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__84);
+  __Pyx_GIVEREF(__pyx_tuple__84);
 
   /* "View.MemoryView":288
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_tuple__84 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__84)) __PYX_ERR(1, 288, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__84);
-  __Pyx_GIVEREF(__pyx_tuple__84);
+  __pyx_tuple__85 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__85)) __PYX_ERR(1, 288, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__85);
+  __Pyx_GIVEREF(__pyx_tuple__85);
 
   /* "View.MemoryView":289
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__85 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__85)) __PYX_ERR(1, 289, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__85);
-  __Pyx_GIVEREF(__pyx_tuple__85);
+  __pyx_tuple__86 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__86)) __PYX_ERR(1, 289, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__86);
+  __Pyx_GIVEREF(__pyx_tuple__86);
 
   /* "View.MemoryView":292
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_tuple__86 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__86)) __PYX_ERR(1, 292, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__86);
-  __Pyx_GIVEREF(__pyx_tuple__86);
+  __pyx_tuple__87 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__87)) __PYX_ERR(1, 292, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__87);
+  __Pyx_GIVEREF(__pyx_tuple__87);
 
   /* "View.MemoryView":293
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__87 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__87)) __PYX_ERR(1, 293, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__87);
-  __Pyx_GIVEREF(__pyx_tuple__87);
+  __pyx_tuple__88 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__88)) __PYX_ERR(1, 293, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__88);
+  __Pyx_GIVEREF(__pyx_tuple__88);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__88 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__88)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__88);
-  __Pyx_GIVEREF(__pyx_tuple__88);
-  __pyx_codeobj__89 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__88, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__89)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__89 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__89)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__89);
+  __Pyx_GIVEREF(__pyx_tuple__89);
+  __pyx_codeobj__90 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__89, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__90)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   __pyx_umethod_PyDict_Type_pop.type = (PyObject*)&PyDict_Type;
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  __pyx_umethod_PyUnicode_Type_strip.type = (PyObject*)&PyUnicode_Type;
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_2 = PyInt_FromLong(2); if (unlikely(!__pyx_int_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_6 = PyInt_FromLong(6); if (unlikely(!__pyx_int_6)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_8 = PyInt_FromLong(8); if (unlikely(!__pyx_int_8)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_100000 = PyInt_FromLong(100000L); if (unlikely(!__pyx_int_100000)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_112105877 = PyInt_FromLong(112105877L); if (unlikely(!__pyx_int_112105877)) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -40253,15 +40370,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_pegasusio__cylib__io) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name_2, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -40374,122 +40491,120 @@
   __pyx_k__19 = 2;
   __pyx_k__20 = 2;
   __pyx_k__20 = 2;
   __pyx_k__21 = 2;
   __pyx_k__21 = 2;
   __pyx_t_1 = __Pyx_PyDict_NewPresized(16); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __pyx_FusedFunction_New(&__pyx_fuse_0_0_0__pyx_mdef_9pegasusio_5cylib_2io_11__pyx_fuse_0_0_0write_mtx, 0, __pyx_n_s_pyx_fuse_0_0_0write_mtx, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__80)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_3 = __pyx_FusedFunction_New(&__pyx_fuse_0_0_0__pyx_mdef_9pegasusio_5cylib_2io_11__pyx_fuse_0_0_0write_mtx, 0, __pyx_n_s_pyx_fuse_0_0_0write_mtx, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__81)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_t_2);
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_s_int_int_int, __pyx_t_3) < 0) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __pyx_FusedFunction_New(&__pyx_fuse_0_0_1__pyx_mdef_9pegasusio_5cylib_2io_13__pyx_fuse_0_0_1write_mtx, 0, __pyx_n_s_pyx_fuse_0_0_1write_mtx, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__80)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_3 = __pyx_FusedFunction_New(&__pyx_fuse_0_0_1__pyx_mdef_9pegasusio_5cylib_2io_13__pyx_fuse_0_0_1write_mtx, 0, __pyx_n_s_pyx_fuse_0_0_1write_mtx, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__81)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_t_2);
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_s_int_int_long, __pyx_t_3) < 0) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __pyx_FusedFunction_New(&__pyx_fuse_0_1_0__pyx_mdef_9pegasusio_5cylib_2io_15__pyx_fuse_0_1_0write_mtx, 0, __pyx_n_s_pyx_fuse_0_1_0write_mtx, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__80)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_3 = __pyx_FusedFunction_New(&__pyx_fuse_0_1_0__pyx_mdef_9pegasusio_5cylib_2io_15__pyx_fuse_0_1_0write_mtx, 0, __pyx_n_s_pyx_fuse_0_1_0write_mtx, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__81)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_t_2);
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_s_int_long_int, __pyx_t_3) < 0) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __pyx_FusedFunction_New(&__pyx_fuse_0_1_1__pyx_mdef_9pegasusio_5cylib_2io_17__pyx_fuse_0_1_1write_mtx, 0, __pyx_n_s_pyx_fuse_0_1_1write_mtx, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__80)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_3 = __pyx_FusedFunction_New(&__pyx_fuse_0_1_1__pyx_mdef_9pegasusio_5cylib_2io_17__pyx_fuse_0_1_1write_mtx, 0, __pyx_n_s_pyx_fuse_0_1_1write_mtx, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__81)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_t_2);
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_s_int_long_long, __pyx_t_3) < 0) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __pyx_FusedFunction_New(&__pyx_fuse_1_0_0__pyx_mdef_9pegasusio_5cylib_2io_19__pyx_fuse_1_0_0write_mtx, 0, __pyx_n_s_pyx_fuse_1_0_0write_mtx, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__80)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_3 = __pyx_FusedFunction_New(&__pyx_fuse_1_0_0__pyx_mdef_9pegasusio_5cylib_2io_19__pyx_fuse_1_0_0write_mtx, 0, __pyx_n_s_pyx_fuse_1_0_0write_mtx, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__81)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_t_2);
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_s_long_int_int, __pyx_t_3) < 0) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __pyx_FusedFunction_New(&__pyx_fuse_1_0_1__pyx_mdef_9pegasusio_5cylib_2io_21__pyx_fuse_1_0_1write_mtx, 0, __pyx_n_s_pyx_fuse_1_0_1write_mtx, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__80)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_3 = __pyx_FusedFunction_New(&__pyx_fuse_1_0_1__pyx_mdef_9pegasusio_5cylib_2io_21__pyx_fuse_1_0_1write_mtx, 0, __pyx_n_s_pyx_fuse_1_0_1write_mtx, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__81)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_t_2);
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_s_long_int_long, __pyx_t_3) < 0) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __pyx_FusedFunction_New(&__pyx_fuse_1_1_0__pyx_mdef_9pegasusio_5cylib_2io_23__pyx_fuse_1_1_0write_mtx, 0, __pyx_n_s_pyx_fuse_1_1_0write_mtx, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__80)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_3 = __pyx_FusedFunction_New(&__pyx_fuse_1_1_0__pyx_mdef_9pegasusio_5cylib_2io_23__pyx_fuse_1_1_0write_mtx, 0, __pyx_n_s_pyx_fuse_1_1_0write_mtx, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__81)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_t_2);
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_s_long_long_int, __pyx_t_3) < 0) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __pyx_FusedFunction_New(&__pyx_fuse_1_1_1__pyx_mdef_9pegasusio_5cylib_2io_25__pyx_fuse_1_1_1write_mtx, 0, __pyx_n_s_pyx_fuse_1_1_1write_mtx, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__80)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_3 = __pyx_FusedFunction_New(&__pyx_fuse_1_1_1__pyx_mdef_9pegasusio_5cylib_2io_25__pyx_fuse_1_1_1write_mtx, 0, __pyx_n_s_pyx_fuse_1_1_1write_mtx, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__81)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_t_2);
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_s_long_long_long, __pyx_t_3) < 0) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __pyx_FusedFunction_New(&__pyx_fuse_2_0_0__pyx_mdef_9pegasusio_5cylib_2io_27__pyx_fuse_2_0_0write_mtx, 0, __pyx_n_s_pyx_fuse_2_0_0write_mtx, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__80)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_3 = __pyx_FusedFunction_New(&__pyx_fuse_2_0_0__pyx_mdef_9pegasusio_5cylib_2io_27__pyx_fuse_2_0_0write_mtx, 0, __pyx_n_s_pyx_fuse_2_0_0write_mtx, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__81)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_t_2);
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_s_float_int_int, __pyx_t_3) < 0) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __pyx_FusedFunction_New(&__pyx_fuse_2_0_1__pyx_mdef_9pegasusio_5cylib_2io_29__pyx_fuse_2_0_1write_mtx, 0, __pyx_n_s_pyx_fuse_2_0_1write_mtx, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__80)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_3 = __pyx_FusedFunction_New(&__pyx_fuse_2_0_1__pyx_mdef_9pegasusio_5cylib_2io_29__pyx_fuse_2_0_1write_mtx, 0, __pyx_n_s_pyx_fuse_2_0_1write_mtx, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__81)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_t_2);
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_s_float_int_long, __pyx_t_3) < 0) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __pyx_FusedFunction_New(&__pyx_fuse_2_1_0__pyx_mdef_9pegasusio_5cylib_2io_31__pyx_fuse_2_1_0write_mtx, 0, __pyx_n_s_pyx_fuse_2_1_0write_mtx, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__80)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_3 = __pyx_FusedFunction_New(&__pyx_fuse_2_1_0__pyx_mdef_9pegasusio_5cylib_2io_31__pyx_fuse_2_1_0write_mtx, 0, __pyx_n_s_pyx_fuse_2_1_0write_mtx, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__81)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_t_2);
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_s_float_long_int, __pyx_t_3) < 0) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __pyx_FusedFunction_New(&__pyx_fuse_2_1_1__pyx_mdef_9pegasusio_5cylib_2io_33__pyx_fuse_2_1_1write_mtx, 0, __pyx_n_s_pyx_fuse_2_1_1write_mtx, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__80)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_3 = __pyx_FusedFunction_New(&__pyx_fuse_2_1_1__pyx_mdef_9pegasusio_5cylib_2io_33__pyx_fuse_2_1_1write_mtx, 0, __pyx_n_s_pyx_fuse_2_1_1write_mtx, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__81)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_t_2);
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_s_float_long_long, __pyx_t_3) < 0) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __pyx_FusedFunction_New(&__pyx_fuse_3_0_0__pyx_mdef_9pegasusio_5cylib_2io_35__pyx_fuse_3_0_0write_mtx, 0, __pyx_n_s_pyx_fuse_3_0_0write_mtx, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__80)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_3 = __pyx_FusedFunction_New(&__pyx_fuse_3_0_0__pyx_mdef_9pegasusio_5cylib_2io_35__pyx_fuse_3_0_0write_mtx, 0, __pyx_n_s_pyx_fuse_3_0_0write_mtx, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__81)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_t_2);
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_s_double_int_int, __pyx_t_3) < 0) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __pyx_FusedFunction_New(&__pyx_fuse_3_0_1__pyx_mdef_9pegasusio_5cylib_2io_37__pyx_fuse_3_0_1write_mtx, 0, __pyx_n_s_pyx_fuse_3_0_1write_mtx, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__80)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_3 = __pyx_FusedFunction_New(&__pyx_fuse_3_0_1__pyx_mdef_9pegasusio_5cylib_2io_37__pyx_fuse_3_0_1write_mtx, 0, __pyx_n_s_pyx_fuse_3_0_1write_mtx, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__81)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_t_2);
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_s_double_int_long, __pyx_t_3) < 0) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __pyx_FusedFunction_New(&__pyx_fuse_3_1_0__pyx_mdef_9pegasusio_5cylib_2io_39__pyx_fuse_3_1_0write_mtx, 0, __pyx_n_s_pyx_fuse_3_1_0write_mtx, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__80)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_3 = __pyx_FusedFunction_New(&__pyx_fuse_3_1_0__pyx_mdef_9pegasusio_5cylib_2io_39__pyx_fuse_3_1_0write_mtx, 0, __pyx_n_s_pyx_fuse_3_1_0write_mtx, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__81)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_t_2);
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_s_double_long_int, __pyx_t_3) < 0) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __pyx_FusedFunction_New(&__pyx_fuse_3_1_1__pyx_mdef_9pegasusio_5cylib_2io_41__pyx_fuse_3_1_1write_mtx, 0, __pyx_n_s_pyx_fuse_3_1_1write_mtx, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__80)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_3 = __pyx_FusedFunction_New(&__pyx_fuse_3_1_1__pyx_mdef_9pegasusio_5cylib_2io_41__pyx_fuse_3_1_1write_mtx, 0, __pyx_n_s_pyx_fuse_3_1_1write_mtx, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__81)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_t_2);
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_s_double_long_long, __pyx_t_3) < 0) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __pyx_FusedFunction_New(&__pyx_mdef_9pegasusio_5cylib_2io_3write_mtx, 0, __pyx_n_s_write_mtx, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__80)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_3 = __pyx_FusedFunction_New(&__pyx_mdef_9pegasusio_5cylib_2io_3write_mtx, 0, __pyx_n_s_write_mtx, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__81)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_t_2);
   ((__pyx_FusedFunctionObject *) __pyx_t_3)->__signatures__ = __pyx_t_1;
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_write_mtx, __pyx_t_3) < 0) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "ext_modules/io_funcs.pyx":197
+  /* "ext_modules/io_funcs.pyx":201
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef void write_dense(char* output_file, str[:] barcodes, str[:] features, data_type[:] data, indices_type[:] indices, indptr_type[:] indptr, int M, int N, int precision = 2):             # <<<<<<<<<<<<<<
  *     """ Input must be csr_matrix internal representation, gene by cell (X.T.tocsr()); Output will be gene by cell
  *     """
  */
-  __pyx_t_2 = __Pyx_PyInt_From_long(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_long(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_k__24 = 2;
-  __pyx_k__24 = 2;
-  __pyx_k__26 = 2;
-  __pyx_k__26 = 2;
+  __pyx_k__25 = 2;
+  __pyx_k__25 = 2;
   __pyx_k__27 = 2;
   __pyx_k__27 = 2;
   __pyx_k__28 = 2;
   __pyx_k__28 = 2;
   __pyx_k__29 = 2;
   __pyx_k__29 = 2;
   __pyx_k__30 = 2;
@@ -40510,103 +40625,105 @@
   __pyx_k__37 = 2;
   __pyx_k__38 = 2;
   __pyx_k__38 = 2;
   __pyx_k__39 = 2;
   __pyx_k__39 = 2;
   __pyx_k__40 = 2;
   __pyx_k__40 = 2;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(16); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_k__41 = 2;
+  __pyx_k__41 = 2;
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(16); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_0_0_0__pyx_mdef_9pegasusio_5cylib_2io_45__pyx_fuse_0_0_0write_dense, 0, __pyx_n_s_pyx_fuse_0_0_0write_dense, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__82)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_0_0_0__pyx_mdef_9pegasusio_5cylib_2io_45__pyx_fuse_0_0_0write_dense, 0, __pyx_n_s_pyx_fuse_0_0_0write_dense, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__83)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_int_int_int, __pyx_t_1) < 0) __PYX_ERR(0, 197, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_int_int_int, __pyx_t_1) < 0) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_0_0_1__pyx_mdef_9pegasusio_5cylib_2io_47__pyx_fuse_0_0_1write_dense, 0, __pyx_n_s_pyx_fuse_0_0_1write_dense, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__82)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_0_0_1__pyx_mdef_9pegasusio_5cylib_2io_47__pyx_fuse_0_0_1write_dense, 0, __pyx_n_s_pyx_fuse_0_0_1write_dense, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__83)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_int_int_long, __pyx_t_1) < 0) __PYX_ERR(0, 197, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_int_int_long, __pyx_t_1) < 0) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_0_1_0__pyx_mdef_9pegasusio_5cylib_2io_49__pyx_fuse_0_1_0write_dense, 0, __pyx_n_s_pyx_fuse_0_1_0write_dense, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__82)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_0_1_0__pyx_mdef_9pegasusio_5cylib_2io_49__pyx_fuse_0_1_0write_dense, 0, __pyx_n_s_pyx_fuse_0_1_0write_dense, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__83)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_int_long_int, __pyx_t_1) < 0) __PYX_ERR(0, 197, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_int_long_int, __pyx_t_1) < 0) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_0_1_1__pyx_mdef_9pegasusio_5cylib_2io_51__pyx_fuse_0_1_1write_dense, 0, __pyx_n_s_pyx_fuse_0_1_1write_dense, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__82)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_0_1_1__pyx_mdef_9pegasusio_5cylib_2io_51__pyx_fuse_0_1_1write_dense, 0, __pyx_n_s_pyx_fuse_0_1_1write_dense, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__83)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_int_long_long, __pyx_t_1) < 0) __PYX_ERR(0, 197, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_int_long_long, __pyx_t_1) < 0) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_1_0_0__pyx_mdef_9pegasusio_5cylib_2io_53__pyx_fuse_1_0_0write_dense, 0, __pyx_n_s_pyx_fuse_1_0_0write_dense, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__82)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_1_0_0__pyx_mdef_9pegasusio_5cylib_2io_53__pyx_fuse_1_0_0write_dense, 0, __pyx_n_s_pyx_fuse_1_0_0write_dense, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__83)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_long_int_int, __pyx_t_1) < 0) __PYX_ERR(0, 197, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_long_int_int, __pyx_t_1) < 0) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_1_0_1__pyx_mdef_9pegasusio_5cylib_2io_55__pyx_fuse_1_0_1write_dense, 0, __pyx_n_s_pyx_fuse_1_0_1write_dense, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__82)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_1_0_1__pyx_mdef_9pegasusio_5cylib_2io_55__pyx_fuse_1_0_1write_dense, 0, __pyx_n_s_pyx_fuse_1_0_1write_dense, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__83)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_long_int_long, __pyx_t_1) < 0) __PYX_ERR(0, 197, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_long_int_long, __pyx_t_1) < 0) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_1_1_0__pyx_mdef_9pegasusio_5cylib_2io_57__pyx_fuse_1_1_0write_dense, 0, __pyx_n_s_pyx_fuse_1_1_0write_dense, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__82)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_1_1_0__pyx_mdef_9pegasusio_5cylib_2io_57__pyx_fuse_1_1_0write_dense, 0, __pyx_n_s_pyx_fuse_1_1_0write_dense, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__83)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_long_long_int, __pyx_t_1) < 0) __PYX_ERR(0, 197, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_long_long_int, __pyx_t_1) < 0) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_1_1_1__pyx_mdef_9pegasusio_5cylib_2io_59__pyx_fuse_1_1_1write_dense, 0, __pyx_n_s_pyx_fuse_1_1_1write_dense, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__82)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_1_1_1__pyx_mdef_9pegasusio_5cylib_2io_59__pyx_fuse_1_1_1write_dense, 0, __pyx_n_s_pyx_fuse_1_1_1write_dense, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__83)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_long_long_long, __pyx_t_1) < 0) __PYX_ERR(0, 197, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_long_long_long, __pyx_t_1) < 0) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_2_0_0__pyx_mdef_9pegasusio_5cylib_2io_61__pyx_fuse_2_0_0write_dense, 0, __pyx_n_s_pyx_fuse_2_0_0write_dense, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__82)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_2_0_0__pyx_mdef_9pegasusio_5cylib_2io_61__pyx_fuse_2_0_0write_dense, 0, __pyx_n_s_pyx_fuse_2_0_0write_dense, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__83)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_float_int_int, __pyx_t_1) < 0) __PYX_ERR(0, 197, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_float_int_int, __pyx_t_1) < 0) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_2_0_1__pyx_mdef_9pegasusio_5cylib_2io_63__pyx_fuse_2_0_1write_dense, 0, __pyx_n_s_pyx_fuse_2_0_1write_dense, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__82)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_2_0_1__pyx_mdef_9pegasusio_5cylib_2io_63__pyx_fuse_2_0_1write_dense, 0, __pyx_n_s_pyx_fuse_2_0_1write_dense, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__83)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_float_int_long, __pyx_t_1) < 0) __PYX_ERR(0, 197, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_float_int_long, __pyx_t_1) < 0) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_2_1_0__pyx_mdef_9pegasusio_5cylib_2io_65__pyx_fuse_2_1_0write_dense, 0, __pyx_n_s_pyx_fuse_2_1_0write_dense, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__82)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_2_1_0__pyx_mdef_9pegasusio_5cylib_2io_65__pyx_fuse_2_1_0write_dense, 0, __pyx_n_s_pyx_fuse_2_1_0write_dense, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__83)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_float_long_int, __pyx_t_1) < 0) __PYX_ERR(0, 197, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_float_long_int, __pyx_t_1) < 0) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_2_1_1__pyx_mdef_9pegasusio_5cylib_2io_67__pyx_fuse_2_1_1write_dense, 0, __pyx_n_s_pyx_fuse_2_1_1write_dense, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__82)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_2_1_1__pyx_mdef_9pegasusio_5cylib_2io_67__pyx_fuse_2_1_1write_dense, 0, __pyx_n_s_pyx_fuse_2_1_1write_dense, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__83)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_float_long_long, __pyx_t_1) < 0) __PYX_ERR(0, 197, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_float_long_long, __pyx_t_1) < 0) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_3_0_0__pyx_mdef_9pegasusio_5cylib_2io_69__pyx_fuse_3_0_0write_dense, 0, __pyx_n_s_pyx_fuse_3_0_0write_dense, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__82)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_3_0_0__pyx_mdef_9pegasusio_5cylib_2io_69__pyx_fuse_3_0_0write_dense, 0, __pyx_n_s_pyx_fuse_3_0_0write_dense, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__83)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_double_int_int, __pyx_t_1) < 0) __PYX_ERR(0, 197, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_double_int_int, __pyx_t_1) < 0) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_3_0_1__pyx_mdef_9pegasusio_5cylib_2io_71__pyx_fuse_3_0_1write_dense, 0, __pyx_n_s_pyx_fuse_3_0_1write_dense, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__82)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_3_0_1__pyx_mdef_9pegasusio_5cylib_2io_71__pyx_fuse_3_0_1write_dense, 0, __pyx_n_s_pyx_fuse_3_0_1write_dense, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__83)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_double_int_long, __pyx_t_1) < 0) __PYX_ERR(0, 197, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_double_int_long, __pyx_t_1) < 0) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_3_1_0__pyx_mdef_9pegasusio_5cylib_2io_73__pyx_fuse_3_1_0write_dense, 0, __pyx_n_s_pyx_fuse_3_1_0write_dense, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__82)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_3_1_0__pyx_mdef_9pegasusio_5cylib_2io_73__pyx_fuse_3_1_0write_dense, 0, __pyx_n_s_pyx_fuse_3_1_0write_dense, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__83)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_double_long_int, __pyx_t_1) < 0) __PYX_ERR(0, 197, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_double_long_int, __pyx_t_1) < 0) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_3_1_1__pyx_mdef_9pegasusio_5cylib_2io_75__pyx_fuse_3_1_1write_dense, 0, __pyx_n_s_pyx_fuse_3_1_1write_dense, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__82)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_3_1_1__pyx_mdef_9pegasusio_5cylib_2io_75__pyx_fuse_3_1_1write_dense, 0, __pyx_n_s_pyx_fuse_3_1_1write_dense, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__83)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_double_long_long, __pyx_t_1) < 0) __PYX_ERR(0, 197, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_s_double_long_long, __pyx_t_1) < 0) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_mdef_9pegasusio_5cylib_2io_7write_dense, 0, __pyx_n_s_write_dense, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__82)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_mdef_9pegasusio_5cylib_2io_7write_dense, 0, __pyx_n_s_write_dense, NULL, __pyx_n_s_pegasusio_cylib_io, __pyx_d, ((PyObject *)__pyx_codeobj__83)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_t_3);
   ((__pyx_FusedFunctionObject *) __pyx_t_1)->__signatures__ = __pyx_t_2;
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_write_dense, __pyx_t_1) < 0) __PYX_ERR(0, 197, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_write_dense, __pyx_t_1) < 0) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "ext_modules/io_funcs.pyx":1
  * # cython: language_level=3, c_string_type=str, c_string_encoding=default             # <<<<<<<<<<<<<<
  * 
  * import numpy as np
@@ -40632,71 +40749,71 @@
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__83, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 287, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__84, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_XGOTREF(generic);
   __Pyx_DECREF_SET(generic, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __pyx_t_3 = 0;
 
   /* "View.MemoryView":288
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__84, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 288, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__85, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 288, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_XGOTREF(strided);
   __Pyx_DECREF_SET(strided, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __pyx_t_3 = 0;
 
   /* "View.MemoryView":289
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__85, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 289, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__86, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 289, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_XGOTREF(indirect);
   __Pyx_DECREF_SET(indirect, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __pyx_t_3 = 0;
 
   /* "View.MemoryView":292
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__86, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 292, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__87, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 292, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_XGOTREF(contiguous);
   __Pyx_DECREF_SET(contiguous, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __pyx_t_3 = 0;
 
   /* "View.MemoryView":293
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__87, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 293, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__88, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 293, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_XGOTREF(indirect_contiguous);
   __Pyx_DECREF_SET(indirect_contiguous, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __pyx_t_3 = 0;
 
   /* "View.MemoryView":317
@@ -41753,15 +41870,15 @@
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
 #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCall(func, NULL, 0);
     }
 #endif
-#ifdef __Pyx_CyFunction_USED
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
     if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
 #else
     if (likely(PyCFunction_Check(func)))
 #endif
     {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
             return __Pyx_PyObject_CallMethO(func, NULL);
@@ -41898,18 +42015,16 @@
 
 /* UnpackItemEndCheck */
 static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected) {
     if (unlikely(retval)) {
         Py_DECREF(retval);
         __Pyx_RaiseTooManyValuesError(expected);
         return -1;
-    } else {
-        return __Pyx_IterFinish();
     }
-    return 0;
+    return __Pyx_IterFinish();
 }
 
 /* RaiseNoneIterError */
 static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
 }
 
@@ -42212,17 +42327,15 @@
     PyObject *old_exc, *old_val, *old_tb;
     PyObject *ctx;
     __Pyx_PyThreadState_declare
 #ifdef WITH_THREAD
     PyGILState_STATE state;
     if (nogil)
         state = PyGILState_Ensure();
-#ifdef _MSC_VER
-    else state = (PyGILState_STATE)-1;
-#endif
+    else state = (PyGILState_STATE)0;
 #endif
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&old_exc, &old_val, &old_tb);
     if (full_traceback) {
         Py_XINCREF(old_exc);
         Py_XINCREF(old_val);
         Py_XINCREF(old_tb);
@@ -42487,14 +42600,86 @@
 #else
     result_ulength++;
     value_count++;
     return PyUnicode_Join(__pyx_empty_unicode, value_tuple);
 #endif
 }
 
+/* UnpackUnboundCMethod */
+static int __Pyx_TryUnpackUnboundCMethod(__Pyx_CachedCFunction* target) {
+    PyObject *method;
+    method = __Pyx_PyObject_GetAttrStr(target->type, *target->method_name);
+    if (unlikely(!method))
+        return -1;
+    target->method = method;
+#if CYTHON_COMPILING_IN_CPYTHON
+    #if PY_MAJOR_VERSION >= 3
+    if (likely(__Pyx_TypeCheck(method, &PyMethodDescr_Type)))
+    #endif
+    {
+        PyMethodDescrObject *descr = (PyMethodDescrObject*) method;
+        target->func = descr->d_method->ml_meth;
+        target->flag = descr->d_method->ml_flags & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_STACKLESS);
+    }
+#endif
+    return 0;
+}
+
+/* CallUnboundCMethod1 */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_CallUnboundCMethod1(__Pyx_CachedCFunction* cfunc, PyObject* self, PyObject* arg) {
+    if (likely(cfunc->func)) {
+        int flag = cfunc->flag;
+        if (flag == METH_O) {
+            return (*(cfunc->func))(self, arg);
+        } else if (PY_VERSION_HEX >= 0x030600B1 && flag == METH_FASTCALL) {
+            #if PY_VERSION_HEX >= 0x030700A0
+                return (*(__Pyx_PyCFunctionFast)(void*)(PyCFunction)cfunc->func)(self, &arg, 1);
+            #else
+                return (*(__Pyx_PyCFunctionFastWithKeywords)(void*)(PyCFunction)cfunc->func)(self, &arg, 1, NULL);
+            #endif
+        } else if (PY_VERSION_HEX >= 0x030700A0 && flag == (METH_FASTCALL | METH_KEYWORDS)) {
+            return (*(__Pyx_PyCFunctionFastWithKeywords)(void*)(PyCFunction)cfunc->func)(self, &arg, 1, NULL);
+        }
+    }
+    return __Pyx__CallUnboundCMethod1(cfunc, self, arg);
+}
+#endif
+static PyObject* __Pyx__CallUnboundCMethod1(__Pyx_CachedCFunction* cfunc, PyObject* self, PyObject* arg){
+    PyObject *args, *result = NULL;
+    if (unlikely(!cfunc->func && !cfunc->method) && unlikely(__Pyx_TryUnpackUnboundCMethod(cfunc) < 0)) return NULL;
+#if CYTHON_COMPILING_IN_CPYTHON
+    if (cfunc->func && (cfunc->flag & METH_VARARGS)) {
+        args = PyTuple_New(1);
+        if (unlikely(!args)) goto bad;
+        Py_INCREF(arg);
+        PyTuple_SET_ITEM(args, 0, arg);
+        if (cfunc->flag & METH_KEYWORDS)
+            result = (*(PyCFunctionWithKeywords)(void*)(PyCFunction)cfunc->func)(self, args, NULL);
+        else
+            result = (*cfunc->func)(self, args);
+    } else {
+        args = PyTuple_New(2);
+        if (unlikely(!args)) goto bad;
+        Py_INCREF(self);
+        PyTuple_SET_ITEM(args, 0, self);
+        Py_INCREF(arg);
+        PyTuple_SET_ITEM(args, 1, arg);
+        result = __Pyx_PyObject_Call(cfunc->method, args, NULL);
+    }
+#else
+    args = PyTuple_Pack(2, self, arg);
+    if (unlikely(!args)) goto bad;
+    result = __Pyx_PyObject_Call(cfunc->method, args, NULL);
+#endif
+bad:
+    Py_XDECREF(args);
+    return result;
+}
+
 /* GetTopmostException */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem *
 __Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
 {
     _PyErr_StackItem *exc_info = tstate->exc_info;
     while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
@@ -42970,34 +43155,14 @@
 /* PyUnicode_Unicode */
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_Unicode(PyObject *obj) {
     if (unlikely(obj == Py_None))
         obj = __pyx_kp_u_None;
     return __Pyx_NewRef(obj);
 }
 
-/* UnpackUnboundCMethod */
-static int __Pyx_TryUnpackUnboundCMethod(__Pyx_CachedCFunction* target) {
-    PyObject *method;
-    method = __Pyx_PyObject_GetAttrStr(target->type, *target->method_name);
-    if (unlikely(!method))
-        return -1;
-    target->method = method;
-#if CYTHON_COMPILING_IN_CPYTHON
-    #if PY_MAJOR_VERSION >= 3
-    if (likely(__Pyx_TypeCheck(method, &PyMethodDescr_Type)))
-    #endif
-    {
-        PyMethodDescrObject *descr = (PyMethodDescrObject*) method;
-        target->func = descr->d_method->ml_meth;
-        target->flag = descr->d_method->ml_flags & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_STACKLESS);
-    }
-#endif
-    return 0;
-}
-
 /* CallUnboundCMethod2 */
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030600B1
 static CYTHON_INLINE PyObject *__Pyx_CallUnboundCMethod2(__Pyx_CachedCFunction *cfunc, PyObject *self, PyObject *arg1, PyObject *arg2) {
     if (likely(cfunc->func)) {
         PyObject *args[2] = {arg1, arg2};
         if (cfunc->flag == METH_FASTCALL) {
             #if PY_VERSION_HEX >= 0x030700A0
@@ -43046,66 +43211,14 @@
     result = __Pyx_PyObject_Call(cfunc->method, args, NULL);
 #endif
 bad:
     Py_XDECREF(args);
     return result;
 }
 
-/* CallUnboundCMethod1 */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_CallUnboundCMethod1(__Pyx_CachedCFunction* cfunc, PyObject* self, PyObject* arg) {
-    if (likely(cfunc->func)) {
-        int flag = cfunc->flag;
-        if (flag == METH_O) {
-            return (*(cfunc->func))(self, arg);
-        } else if (PY_VERSION_HEX >= 0x030600B1 && flag == METH_FASTCALL) {
-            if (PY_VERSION_HEX >= 0x030700A0) {
-                return (*(__Pyx_PyCFunctionFast)(void*)(PyCFunction)cfunc->func)(self, &arg, 1);
-            } else {
-                return (*(__Pyx_PyCFunctionFastWithKeywords)(void*)(PyCFunction)cfunc->func)(self, &arg, 1, NULL);
-            }
-        } else if (PY_VERSION_HEX >= 0x030700A0 && flag == (METH_FASTCALL | METH_KEYWORDS)) {
-            return (*(__Pyx_PyCFunctionFastWithKeywords)(void*)(PyCFunction)cfunc->func)(self, &arg, 1, NULL);
-        }
-    }
-    return __Pyx__CallUnboundCMethod1(cfunc, self, arg);
-}
-#endif
-static PyObject* __Pyx__CallUnboundCMethod1(__Pyx_CachedCFunction* cfunc, PyObject* self, PyObject* arg){
-    PyObject *args, *result = NULL;
-    if (unlikely(!cfunc->func && !cfunc->method) && unlikely(__Pyx_TryUnpackUnboundCMethod(cfunc) < 0)) return NULL;
-#if CYTHON_COMPILING_IN_CPYTHON
-    if (cfunc->func && (cfunc->flag & METH_VARARGS)) {
-        args = PyTuple_New(1);
-        if (unlikely(!args)) goto bad;
-        Py_INCREF(arg);
-        PyTuple_SET_ITEM(args, 0, arg);
-        if (cfunc->flag & METH_KEYWORDS)
-            result = (*(PyCFunctionWithKeywords)(void*)(PyCFunction)cfunc->func)(self, args, NULL);
-        else
-            result = (*cfunc->func)(self, args);
-    } else {
-        args = PyTuple_New(2);
-        if (unlikely(!args)) goto bad;
-        Py_INCREF(self);
-        PyTuple_SET_ITEM(args, 0, self);
-        Py_INCREF(arg);
-        PyTuple_SET_ITEM(args, 1, arg);
-        result = __Pyx_PyObject_Call(cfunc->method, args, NULL);
-    }
-#else
-    args = PyTuple_Pack(2, self, arg);
-    if (unlikely(!args)) goto bad;
-    result = __Pyx_PyObject_Call(cfunc->method, args, NULL);
-#endif
-bad:
-    Py_XDECREF(args);
-    return result;
-}
-
 /* py_dict_pop */
 static CYTHON_INLINE PyObject *__Pyx_PyDict_Pop(PyObject *d, PyObject *key, PyObject *default_value) {
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX > 0x030600B3
     if ((1)) {
         return _PyDict_Pop(d, key, default_value);
     } else
 #endif
@@ -43616,15 +43729,15 @@
 #endif
     return PyObject_GetAttr(o, n);
 }
 
 /* ObjectGetItem */
 #if CYTHON_USE_TYPE_SLOTS
 static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
-    PyObject *runerr;
+    PyObject *runerr = NULL;
     Py_ssize_t key_value;
     PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
     if (unlikely(!(m && m->sq_item))) {
         PyErr_Format(PyExc_TypeError, "'%.200s' object is not subscriptable", Py_TYPE(obj)->tp_name);
         return NULL;
     }
     key_value = __Pyx_PyIndex_AsSsize_t(index);
@@ -44710,17 +44823,22 @@
         argc = PyTuple_GET_SIZE(args);
         new_args = PyTuple_GetSlice(args, 1, argc);
         if (unlikely(!new_args))
             return NULL;
         self = PyTuple_GetItem(args, 0);
         if (unlikely(!self)) {
             Py_DECREF(new_args);
+#if PY_MAJOR_VERSION > 2
             PyErr_Format(PyExc_TypeError,
                          "unbound method %.200S() needs an argument",
                          cyfunc->func_qualname);
+#else
+            PyErr_SetString(PyExc_TypeError,
+                            "unbound method needs an argument");
+#endif
             return NULL;
         }
         result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
         Py_DECREF(new_args);
     } else {
         result = __Pyx_CyFunction_Call(func, args, kw);
     }
@@ -45185,15 +45303,15 @@
         return -1;
     }
     return 0;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
```

### Comparing `pegasusio-0.8.0/ext_modules/io_funcs.pyx` & `pegasusio-0.8.1/ext_modules/io_funcs.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -143,36 +143,40 @@
 
     assert getline(&line, &size, fi) >= 0
     pch = strtok(line, delimiters)
     assert pch != NULL
 
     if strchr(delimiters, line[0]) != NULL:
         row_key = ""
-        N = 1
         colnames.append(pch)
+        colnames[N] = colnames[N].strip("\"'")
+        N = 1
     else:
         row_key = pch
+        row_key = row_key.strip("\"'")
 
     pch = strtok(NULL, delimiters)
     while pch != NULL:
         colnames.append(pch)
+        colnames[N] = colnames[N].strip("\"'")
         N += 1
         pch = strtok(NULL, delimiters)
 
     if N == 0:
         raise ValueError(f"File {csv_file} contains no columns!")
 
-    colnames[N - 1] = colnames[N - 1].rstrip("\n\r")
+    colnames[N - 1] = colnames[N - 1].rstrip("\n\r").strip("\"'")
 
     while getline(&line, &size, fi) >=0:
         if line[0] < 32 or line[0] == 127:
             continue
         pch = strtok(line, delimiters)
         assert pch != NULL
         rownames.append(pch)
+        rownames[M] = rownames[M].strip("\"'")
         for i in range(N):
             pch = strtok(NULL, delimiters)
             assert pch != NULL
             if is_zero(pch) == 0:
                 row_ind.append(M)
                 col_ind.append(i)
                 data_list.append(pch)
```

### Comparing `pegasusio-0.8.0/pegasusio/__init__.py` & `pegasusio-0.8.1/pegasusio/__init__.py`

 * *Files identical despite different names*

### Comparing `pegasusio-0.8.0/pegasusio/__main__.py` & `pegasusio-0.8.1/pegasusio/__main__.py`

 * *Files identical despite different names*

### Comparing `pegasusio-0.8.0/pegasusio/aggr_data.py` & `pegasusio-0.8.1/pegasusio/aggr_data.py`

 * *Files identical despite different names*

### Comparing `pegasusio-0.8.0/pegasusio/citeseq_data.py` & `pegasusio-0.8.1/pegasusio/citeseq_data.py`

 * *Files identical despite different names*

### Comparing `pegasusio-0.8.0/pegasusio/commands/AggregateMatrix.py` & `pegasusio-0.8.1/pegasusio/commands/AggregateMatrix.py`

 * *Files identical despite different names*

### Comparing `pegasusio-0.8.0/pegasusio/commands/Base.py` & `pegasusio-0.8.1/pegasusio/commands/Base.py`

 * *Files identical despite different names*

### Comparing `pegasusio-0.8.0/pegasusio/cyto_data.py` & `pegasusio-0.8.1/pegasusio/cyto_data.py`

 * *Files identical despite different names*

### Comparing `pegasusio-0.8.0/pegasusio/cyto_utils.py` & `pegasusio-0.8.1/pegasusio/cyto_utils.py`

 * *Files identical despite different names*

### Comparing `pegasusio-0.8.0/pegasusio/data_aggregation.py` & `pegasusio-0.8.1/pegasusio/data_aggregation.py`

 * *Files identical despite different names*

### Comparing `pegasusio-0.8.0/pegasusio/datadict.py` & `pegasusio-0.8.1/pegasusio/datadict.py`

 * *Files identical despite different names*

### Comparing `pegasusio-0.8.0/pegasusio/decorators.py` & `pegasusio-0.8.1/pegasusio/decorators.py`

 * *Files identical despite different names*

### Comparing `pegasusio-0.8.0/pegasusio/hdf5_utils.py` & `pegasusio-0.8.1/pegasusio/hdf5_utils.py`

 * *Files identical despite different names*

### Comparing `pegasusio-0.8.0/pegasusio/multimodal_data.py` & `pegasusio-0.8.1/pegasusio/multimodal_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -345,15 +345,19 @@
 
         return results
 
 
     def drop_data(self, key: str) -> UnimodalData:
         if key not in self.data:
             raise ValueError("Key {} does not exist!".format(key))
-        return self.data.pop(key)
+        dat = self.data.pop(key)
+        if len(self.data) == 0:
+            self._selected = None
+            self._unidata = None
+        return dat
 
 
     def filter_data(self,
         select_singlets: Optional[bool] = False,
         remap_string: Optional[str] = None,
         subset_string: Optional[str] = None,
         min_genes: Optional[int] = None,
```

### Comparing `pegasusio-0.8.0/pegasusio/nanostring_data.py` & `pegasusio-0.8.1/pegasusio/nanostring_data.py`

 * *Files identical despite different names*

### Comparing `pegasusio-0.8.0/pegasusio/nanostring_utils.py` & `pegasusio-0.8.1/pegasusio/nanostring_utils.py`

 * *Files identical despite different names*

### Comparing `pegasusio-0.8.0/pegasusio/qc_utils.py` & `pegasusio-0.8.1/pegasusio/qc_utils.py`

 * *Files identical despite different names*

### Comparing `pegasusio-0.8.0/pegasusio/readwrite.py` & `pegasusio-0.8.1/pegasusio/readwrite.py`

 * *Files identical despite different names*

### Comparing `pegasusio-0.8.0/pegasusio/spatial_data.py` & `pegasusio-0.8.1/pegasusio/spatial_data.py`

 * *Files identical despite different names*

### Comparing `pegasusio-0.8.0/pegasusio/spatial_utils.py` & `pegasusio-0.8.1/pegasusio/spatial_utils.py`

 * *Files identical despite different names*

### Comparing `pegasusio-0.8.0/pegasusio/text_utils.py` & `pegasusio-0.8.1/pegasusio/text_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -304,14 +304,16 @@
 
     for key in data.list_data():
         _write_mtx(data.get_data(key), os.path.join(output_dir, key), precision)
 
     logger.info("Mtx files are written.")
 
 
+def _strip_quotes(rowkey: str, rownames: List[str], colnames: List[str]) -> Tuple[str, List[str], List[str]]:
+    return rowkey.strip("\"'"), list(map(lambda x: x.strip("\"'"), rownames)), list(map(lambda x: x.strip("\"'"), colnames))
 
 def load_csv_file(
     input_csv: str,
     sep: str = ",",
     genome: str = None,
     modality: str = None,
     transpose: bool = False,
```

### Comparing `pegasusio-0.8.0/pegasusio/unimodal_data.py` & `pegasusio-0.8.1/pegasusio/unimodal_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,18 +123,19 @@
                 raise ValueError(
                     f"Wrong number of features : matrix '{key}' has {mat.shape[1]} features, features file has {self._shape[1]} features."
                 )
 
         if len(self.matrices) == 0:
             self._cur_matrix = ""
         else:
-            if cur_matrix == None:
+            if cur_matrix == None or len(list(self.matrices.keys())) == 1:
                 cur_matrix = list(self.matrices.keys())[0]
             elif cur_matrix not in self.matrices.keys():
                 raise ValueError("Cannot find the default count matrix to bind to. Please set 'cur_matrix' argument in UnimodalData constructor!")
+
             self._cur_matrix = cur_matrix # cur_matrix
 
         # For backword compatibility, check metadata and move arrays and graphs to multiarrays/multigraphs
         for key in list(metadata.keys()):
             value = metadata[key]
             if isinstance(value, np.ndarray) and value.ndim == 2:
                 if value.shape[0] == self._shape[0]: # put in barcode_multiarrays
```

### Comparing `pegasusio-0.8.0/pegasusio/vdj_data.py` & `pegasusio-0.8.1/pegasusio/vdj_data.py`

 * *Files identical despite different names*

### Comparing `pegasusio-0.8.0/pegasusio/vdj_utils.py` & `pegasusio-0.8.1/pegasusio/vdj_utils.py`

 * *Files identical despite different names*

### Comparing `pegasusio-0.8.0/pegasusio/views.py` & `pegasusio-0.8.1/pegasusio/views.py`

 * *Files identical despite different names*

### Comparing `pegasusio-0.8.0/pegasusio/zarr_utils.py` & `pegasusio-0.8.1/pegasusio/zarr_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,15 +300,15 @@
             categories = group.require_group('_categories', overwrite = False)
             values = array.categories.values
             if isinstance(values[0], bytes):
                 values = np.array([x.decode() for x in values], dtype = object)
             self.write_array(categories, name, values)
             # write codes
             codes_arr = group.create_dataset(name, data = array.codes, shape = array.codes.shape, chunks = calc_chunk(array.codes.shape), dtype = array.codes.dtype, compressor = COMPRESSOR, overwrite = True, write_empty_chunks = self.write_empty_chunks)
-            codes_arr.attrs['ordered'] = array.ordered
+            codes_arr.attrs['ordered'] = bool(array.ordered)
         else:
             self.write_array(group, name, array)
 
 
     def write_dataframe(self, parent: zarr.Group, name: str, df: pd.DataFrame) -> None:
         group = parent.create_group(name, overwrite = True)
         attrs_dict = {'data_type' : 'data_frame', 'columns' : list(df.columns)}
```

### Comparing `pegasusio-0.8.0/pegasusio.egg-info/PKG-INFO` & `pegasusio-0.8.1/pegasusio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pegasusio
-Version: 0.8.0
+Version: 0.8.1
 Summary: Pegasusio is a Python package for reading / writing single-cell genomics data
 Home-page: https://github.com/lilab-bcb/pegasusio
 Author: Yiming Yang, Rimte Rocher, Joshua Gould and Bo Li
 Author-email: cumulus-support@googlegroups.com
 Keywords: single cell/nucleus genomics data reading and writing
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Jupyter
```

### Comparing `pegasusio-0.8.0/pegasusio.egg-info/SOURCES.txt` & `pegasusio-0.8.1/pegasusio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pegasusio-0.8.0/setup.py` & `pegasusio-0.8.1/setup.py`

 * *Files identical despite different names*

