# Comparing `tmp/nb-thumb-0.0.1.tar.gz` & `tmp/nb-thumb-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nb-thumb-0.0.1.tar", last modified: Fri Jul 14 05:41:00 2023, max compression
+gzip compressed data, was "nb-thumb-0.0.2.tar", last modified: Fri Jul 14 06:04:25 2023, max compression
```

## Comparing `nb-thumb-0.0.1.tar` & `nb-thumb-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-07-14 05:41:00.918884 nb-thumb-0.0.1/
--rw-rw-r--   0 hamel      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 nb-thumb-0.0.1/LICENSE
--rw-rw-r--   0 hamel      (501) staff       (20)      111 2023-04-27 10:12:58.000000 nb-thumb-0.0.1/MANIFEST.in
--rw-r--r--   0 hamel      (501) staff       (20)     1171 2023-07-14 05:41:00.918697 nb-thumb-0.0.1/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)      370 2023-07-14 05:39:28.000000 nb-thumb-0.0.1/README.md
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-07-14 05:41:00.917488 nb-thumb-0.0.1/nb_thumb/
--rw-r--r--   0 hamel      (501) staff       (20)       22 2023-07-14 05:40:15.000000 nb-thumb-0.0.1/nb_thumb/__init__.py
--rw-r--r--   0 hamel      (501) staff       (20)      791 2023-07-14 05:40:15.000000 nb-thumb-0.0.1/nb_thumb/_modidx.py
--rw-r--r--   0 hamel      (501) staff       (20)      142 2023-07-14 03:45:28.000000 nb-thumb-0.0.1/nb_thumb/core.py
--rw-r--r--   0 hamel      (501) staff       (20)     1904 2023-07-14 05:40:15.000000 nb-thumb-0.0.1/nb_thumb/thumb.py
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-07-14 05:41:00.918484 nb-thumb-0.0.1/nb_thumb.egg-info/
--rw-r--r--   0 hamel      (501) staff       (20)     1171 2023-07-14 05:41:00.000000 nb-thumb-0.0.1/nb_thumb.egg-info/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)      352 2023-07-14 05:41:00.000000 nb-thumb-0.0.1/nb_thumb.egg-info/SOURCES.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2023-07-14 05:41:00.000000 nb-thumb-0.0.1/nb_thumb.egg-info/dependency_links.txt
--rw-r--r--   0 hamel      (501) staff       (20)       38 2023-07-14 05:41:00.000000 nb-thumb-0.0.1/nb_thumb.egg-info/entry_points.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2023-07-14 05:34:35.000000 nb-thumb-0.0.1/nb_thumb.egg-info/not-zip-safe
--rw-r--r--   0 hamel      (501) staff       (20)        7 2023-07-14 05:41:00.000000 nb-thumb-0.0.1/nb_thumb.egg-info/requires.txt
--rw-r--r--   0 hamel      (501) staff       (20)        9 2023-07-14 05:41:00.000000 nb-thumb-0.0.1/nb_thumb.egg-info/top_level.txt
--rw-r--r--   0 hamel      (501) staff       (20)      964 2023-07-14 03:45:27.000000 nb-thumb-0.0.1/settings.ini
--rw-r--r--   0 hamel      (501) staff       (20)       38 2023-07-14 05:41:00.918934 nb-thumb-0.0.1/setup.cfg
--rw-rw-r--   0 hamel      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 nb-thumb-0.0.1/setup.py
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-07-14 06:04:25.676774 nb-thumb-0.0.2/
+-rw-rw-r--   0 hamel      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 nb-thumb-0.0.2/LICENSE
+-rw-rw-r--   0 hamel      (501) staff       (20)      111 2023-04-27 10:12:58.000000 nb-thumb-0.0.2/MANIFEST.in
+-rw-r--r--   0 hamel      (501) staff       (20)     1402 2023-07-14 06:04:25.676605 nb-thumb-0.0.2/PKG-INFO
+-rw-r--r--   0 hamel      (501) staff       (20)      601 2023-07-14 06:03:56.000000 nb-thumb-0.0.2/README.md
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-07-14 06:04:25.675410 nb-thumb-0.0.2/nb_thumb/
+-rw-r--r--   0 hamel      (501) staff       (20)       22 2023-07-14 06:04:15.000000 nb-thumb-0.0.2/nb_thumb/__init__.py
+-rw-r--r--   0 hamel      (501) staff       (20)      791 2023-07-14 06:04:15.000000 nb-thumb-0.0.2/nb_thumb/_modidx.py
+-rw-r--r--   0 hamel      (501) staff       (20)      142 2023-07-14 03:45:28.000000 nb-thumb-0.0.2/nb_thumb/core.py
+-rw-r--r--   0 hamel      (501) staff       (20)     1932 2023-07-14 06:04:15.000000 nb-thumb-0.0.2/nb_thumb/thumb.py
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-07-14 06:04:25.676412 nb-thumb-0.0.2/nb_thumb.egg-info/
+-rw-r--r--   0 hamel      (501) staff       (20)     1402 2023-07-14 06:04:25.000000 nb-thumb-0.0.2/nb_thumb.egg-info/PKG-INFO
+-rw-r--r--   0 hamel      (501) staff       (20)      352 2023-07-14 06:04:25.000000 nb-thumb-0.0.2/nb_thumb.egg-info/SOURCES.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        1 2023-07-14 06:04:25.000000 nb-thumb-0.0.2/nb_thumb.egg-info/dependency_links.txt
+-rw-r--r--   0 hamel      (501) staff       (20)       38 2023-07-14 06:04:25.000000 nb-thumb-0.0.2/nb_thumb.egg-info/entry_points.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        1 2023-07-14 05:34:35.000000 nb-thumb-0.0.2/nb_thumb.egg-info/not-zip-safe
+-rw-r--r--   0 hamel      (501) staff       (20)       46 2023-07-14 06:04:25.000000 nb-thumb-0.0.2/nb_thumb.egg-info/requires.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        9 2023-07-14 06:04:25.000000 nb-thumb-0.0.2/nb_thumb.egg-info/top_level.txt
+-rw-r--r--   0 hamel      (501) staff       (20)      850 2023-07-14 06:04:15.000000 nb-thumb-0.0.2/settings.ini
+-rw-r--r--   0 hamel      (501) staff       (20)       38 2023-07-14 06:04:25.676823 nb-thumb-0.0.2/setup.cfg
+-rw-rw-r--   0 hamel      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 nb-thumb-0.0.2/setup.py
```

### Comparing `nb-thumb-0.0.1/LICENSE` & `nb-thumb-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nb-thumb-0.0.1/PKG-INFO` & `nb-thumb-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-thumb
-Version: 0.0.1
+Version: 0.0.2
 Summary: Extract thumbnails from Jupyter notebooks
 Home-page: https://github.com/fastai/nb-thumb
 Author: Hamel Husain
 Author-email: hamel.husain@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
@@ -21,30 +21,38 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # nb-thumb
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
+<div>
+
+[![](https://github.com/fastai/nb-thumb/actions/workflows/test.yaml/badge.svg)](https://github.com/fastai/nb-thumb/actions/workflows/test.yaml)
+
+</div>
+
 ## Install
 
 ``` sh
 pip install nb_thumb
 ```
 
 ## Quickstart
 
 ``` python
 from nb_thumb.thumb import nb2thumb
 ```
 
 ``` python
-nb2thumb('_test_nbs/geom_col.ipynb', label='two_variable_bar_plot')
+nb2thumb(nb_path='_test_nbs/geom_col.ipynb', 
+         label='two_variable_bar_plot',
+         size=(200,200))
 ```
 
 ![](index_files/figure-commonmark/cell-3-output-1.png)
 
 ## Usage
 
-See [this page](./00_thumb.ipynb).
+See [this page](https://fastai.github.io/nb-thumb/thumb.html).
```

### Comparing `nb-thumb-0.0.1/nb_thumb/_modidx.py` & `nb-thumb-0.0.2/nb_thumb/_modidx.py`

 * *Files identical despite different names*

### Comparing `nb-thumb-0.0.1/nb_thumb.egg-info/PKG-INFO` & `nb-thumb-0.0.2/nb_thumb.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-thumb
-Version: 0.0.1
+Version: 0.0.2
 Summary: Extract thumbnails from Jupyter notebooks
 Home-page: https://github.com/fastai/nb-thumb
 Author: Hamel Husain
 Author-email: hamel.husain@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
@@ -21,30 +21,38 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # nb-thumb
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
+<div>
+
+[![](https://github.com/fastai/nb-thumb/actions/workflows/test.yaml/badge.svg)](https://github.com/fastai/nb-thumb/actions/workflows/test.yaml)
+
+</div>
+
 ## Install
 
 ``` sh
 pip install nb_thumb
 ```
 
 ## Quickstart
 
 ``` python
 from nb_thumb.thumb import nb2thumb
 ```
 
 ``` python
-nb2thumb('_test_nbs/geom_col.ipynb', label='two_variable_bar_plot')
+nb2thumb(nb_path='_test_nbs/geom_col.ipynb', 
+         label='two_variable_bar_plot',
+         size=(200,200))
 ```
 
 ![](index_files/figure-commonmark/cell-3-output-1.png)
 
 ## Usage
 
-See [this page](./00_thumb.ipynb).
+See [this page](https://fastai.github.io/nb-thumb/thumb.html).
```

### Comparing `nb-thumb-0.0.1/setup.py` & `nb-thumb-0.0.2/setup.py`

 * *Files identical despite different names*

