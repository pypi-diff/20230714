# Comparing `tmp/LTEpy-1.0.1.tar.gz` & `tmp/LTEpy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LTEpy-1.0.1.tar", last modified: Fri Jul 14 16:28:28 2023, max compression
+gzip compressed data, was "LTEpy-1.0.2.tar", last modified: Fri Jul 14 17:54:36 2023, max compression
```

## Comparing `LTEpy-1.0.1.tar` & `LTEpy-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,51 @@
-drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-14 16:28:28.913709 LTEpy-1.0.1/
--rw-r--r--   0 calebharada   (501) staff       (20)     1089 2023-07-14 14:07:27.000000 LTEpy-1.0.1/LICENSE
-drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-14 16:28:28.909055 LTEpy-1.0.1/LTEpy/
--rw-r--r--   0 calebharada   (501) staff       (20)       21 2023-07-14 16:27:32.000000 LTEpy-1.0.1/LTEpy/__init__.py
--rw-r--r--   0 calebharada   (501) staff       (20)     3275 2023-07-14 14:07:27.000000 LTEpy-1.0.1/LTEpy/atom.py
--rw-r--r--   0 calebharada   (501) staff       (20)     2033 2023-07-12 16:10:18.000000 LTEpy-1.0.1/LTEpy/constants.py
--rw-r--r--   0 calebharada   (501) staff       (20)    11933 2023-07-14 14:07:27.000000 LTEpy-1.0.1/LTEpy/lte.py
--rw-r--r--   0 calebharada   (501) staff       (20)     5354 2023-07-14 14:07:27.000000 LTEpy-1.0.1/LTEpy/plot.py
-drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-14 16:28:28.911325 LTEpy-1.0.1/LTEpy.egg-info/
--rw-r--r--   0 calebharada   (501) staff       (20)      335 2023-07-14 16:28:28.000000 LTEpy-1.0.1/LTEpy.egg-info/PKG-INFO
--rw-r--r--   0 calebharada   (501) staff       (20)      337 2023-07-14 16:28:28.000000 LTEpy-1.0.1/LTEpy.egg-info/SOURCES.txt
--rw-r--r--   0 calebharada   (501) staff       (20)        1 2023-07-14 16:28:28.000000 LTEpy-1.0.1/LTEpy.egg-info/dependency_links.txt
--rw-r--r--   0 calebharada   (501) staff       (20)       32 2023-07-14 16:28:28.000000 LTEpy-1.0.1/LTEpy.egg-info/requires.txt
--rw-r--r--   0 calebharada   (501) staff       (20)       12 2023-07-14 16:28:28.000000 LTEpy-1.0.1/LTEpy.egg-info/top_level.txt
--rw-r--r--   0 calebharada   (501) staff       (20)      335 2023-07-14 16:28:28.913349 LTEpy-1.0.1/PKG-INFO
--rw-r--r--   0 calebharada   (501) staff       (20)     1252 2023-07-14 16:25:00.000000 LTEpy-1.0.1/README.md
--rw-r--r--   0 calebharada   (501) staff       (20)       38 2023-07-14 16:28:28.913802 LTEpy-1.0.1/setup.cfg
--rw-r--r--   0 calebharada   (501) staff       (20)      911 2023-07-14 16:24:05.000000 LTEpy-1.0.1/setup.py
-drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-14 16:28:28.912926 LTEpy-1.0.1/tests/
--rw-r--r--   0 calebharada   (501) staff       (20)        0 2023-07-14 14:07:27.000000 LTEpy-1.0.1/tests/__init__.py
--rw-r--r--   0 calebharada   (501) staff       (20)     2258 2023-07-14 14:07:27.000000 LTEpy-1.0.1/tests/test_atom.py
--rw-r--r--   0 calebharada   (501) staff       (20)     1159 2023-07-14 14:07:27.000000 LTEpy-1.0.1/tests/test_boltzmann_factor.py
--rw-r--r--   0 calebharada   (501) staff       (20)     1329 2023-07-14 14:07:27.000000 LTEpy-1.0.1/tests/test_planck.py
+drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-14 17:54:36.629127 LTEpy-1.0.2/
+-rw-r--r--   0 calebharada   (501) staff       (20)       75 2023-07-12 16:10:18.000000 LTEpy-1.0.2/.gitignore
+-rw-r--r--   0 calebharada   (501) staff       (20)      934 2023-07-14 14:07:27.000000 LTEpy-1.0.2/.readthedocs.yaml
+-rw-r--r--   0 calebharada   (501) staff       (20)     1089 2023-07-14 14:07:27.000000 LTEpy-1.0.2/LICENSE
+drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-14 17:54:36.615136 LTEpy-1.0.2/LTEpy/
+-rw-r--r--   0 calebharada   (501) staff       (20)       21 2023-07-14 17:53:11.000000 LTEpy-1.0.2/LTEpy/__init__.py
+drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-14 17:54:36.618007 LTEpy-1.0.2/LTEpy/__pycache__/
+-rw-r--r--   0 calebharada   (501) staff       (20)     1133 2023-07-14 14:07:27.000000 LTEpy-1.0.2/LTEpy/__pycache__/constants.cpython-310.pyc
+-rw-r--r--   0 calebharada   (501) staff       (20)     5306 2023-07-12 16:10:18.000000 LTEpy-1.0.2/LTEpy/__pycache__/equations.cpython-310.pyc
+-rw-r--r--   0 calebharada   (501) staff       (20)     4743 2023-07-11 19:24:11.000000 LTEpy-1.0.2/LTEpy/__pycache__/equations.cpython-311.pyc
+-rw-r--r--   0 calebharada   (501) staff       (20)     3275 2023-07-14 14:07:27.000000 LTEpy-1.0.2/LTEpy/atom.py
+-rw-r--r--   0 calebharada   (501) staff       (20)     2033 2023-07-12 16:10:18.000000 LTEpy-1.0.2/LTEpy/constants.py
+-rw-r--r--   0 calebharada   (501) staff       (20)     1402 2023-07-11 15:15:30.000000 LTEpy-1.0.2/LTEpy/constants.pyc
+-rw-r--r--   0 calebharada   (501) staff       (20)    24294 2023-07-14 14:07:27.000000 LTEpy-1.0.2/LTEpy/custom.mplstyle
+-rw-r--r--   0 calebharada   (501) staff       (20)    11933 2023-07-14 14:07:27.000000 LTEpy-1.0.2/LTEpy/lte.py
+-rw-r--r--   0 calebharada   (501) staff       (20)     5284 2023-07-14 17:49:17.000000 LTEpy-1.0.2/LTEpy/plot.py
+drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-14 17:54:36.616799 LTEpy-1.0.2/LTEpy.egg-info/
+-rw-r--r--   0 calebharada   (501) staff       (20)      363 2023-07-14 17:54:36.000000 LTEpy-1.0.2/LTEpy.egg-info/PKG-INFO
+-rw-r--r--   0 calebharada   (501) staff       (20)      937 2023-07-14 17:54:36.000000 LTEpy-1.0.2/LTEpy.egg-info/SOURCES.txt
+-rw-r--r--   0 calebharada   (501) staff       (20)        1 2023-07-14 17:54:36.000000 LTEpy-1.0.2/LTEpy.egg-info/dependency_links.txt
+-rw-r--r--   0 calebharada   (501) staff       (20)       32 2023-07-14 17:54:36.000000 LTEpy-1.0.2/LTEpy.egg-info/requires.txt
+-rw-r--r--   0 calebharada   (501) staff       (20)       12 2023-07-14 17:54:36.000000 LTEpy-1.0.2/LTEpy.egg-info/top_level.txt
+-rw-r--r--   0 calebharada   (501) staff       (20)      363 2023-07-14 17:54:36.628878 LTEpy-1.0.2/PKG-INFO
+-rw-r--r--   0 calebharada   (501) staff       (20)     1252 2023-07-14 17:01:35.000000 LTEpy-1.0.2/README.md
+drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-14 17:54:36.619957 LTEpy-1.0.2/dist/
+-rw-r--r--   0 calebharada   (501) staff       (20)    11356 2023-07-14 17:01:35.000000 LTEpy-1.0.2/dist/LTEpy-1.0.0-py3-none-any.whl
+-rw-r--r--   0 calebharada   (501) staff       (20)     9991 2023-07-14 17:01:35.000000 LTEpy-1.0.2/dist/LTEpy-1.0.0.tar.gz
+-rw-r--r--   0 calebharada   (501) staff       (20)    11389 2023-07-14 17:01:35.000000 LTEpy-1.0.2/dist/LTEpy-1.0.1-py3-none-any.whl
+-rw-r--r--   0 calebharada   (501) staff       (20)    10113 2023-07-14 17:01:35.000000 LTEpy-1.0.2/dist/LTEpy-1.0.1.tar.gz
+drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-14 17:54:36.623703 LTEpy-1.0.2/docs/
+-rw-r--r--   0 calebharada   (501) staff       (20)      634 2023-07-12 19:05:25.000000 LTEpy-1.0.2/docs/Makefile
+-rw-r--r--   0 calebharada   (501) staff       (20)      104 2023-07-14 14:07:27.000000 LTEpy-1.0.2/docs/api.rst
+-rw-r--r--   0 calebharada   (501) staff       (20)     2179 2023-07-14 14:07:27.000000 LTEpy-1.0.2/docs/conf.py
+-rw-r--r--   0 calebharada   (501) staff       (20)      270 2023-07-14 14:07:27.000000 LTEpy-1.0.2/docs/examples.rst
+-rw-r--r--   0 calebharada   (501) staff       (20)      985 2023-07-14 17:53:39.000000 LTEpy-1.0.2/docs/index.rst
+-rw-r--r--   0 calebharada   (501) staff       (20)      251 2023-07-14 14:07:27.000000 LTEpy-1.0.2/docs/installation.rst
+-rw-r--r--   0 calebharada   (501) staff       (20)      137 2023-07-14 14:07:27.000000 LTEpy-1.0.2/docs/lte.rst
+-rw-r--r--   0 calebharada   (501) staff       (20)      795 2023-07-12 22:14:55.000000 LTEpy-1.0.2/docs/make.bat
+drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-14 17:54:36.626461 LTEpy-1.0.2/docs/notebooks/
+-rw-r--r--   0 calebharada   (501) staff       (20)   114760 2023-07-14 14:53:48.000000 LTEpy-1.0.2/docs/notebooks/boltzmann_factor_demo.ipynb
+-rw-r--r--   0 calebharada   (501) staff       (20)   143024 2023-07-14 14:53:48.000000 LTEpy-1.0.2/docs/notebooks/maxwell_boltzmann_demo.ipynb
+-rw-r--r--   0 calebharada   (501) staff       (20)   141568 2023-07-14 14:53:48.000000 LTEpy-1.0.2/docs/notebooks/planck_demo.ipynb
+-rw-r--r--   0 calebharada   (501) staff       (20)       25 2023-07-14 14:07:27.000000 LTEpy-1.0.2/docs/requirements.txt
+-rw-r--r--   0 calebharada   (501) staff       (20)       31 2023-07-14 14:07:27.000000 LTEpy-1.0.2/requirements.txt
+-rw-r--r--   0 calebharada   (501) staff       (20)       38 2023-07-14 17:54:36.629209 LTEpy-1.0.2/setup.cfg
+-rw-r--r--   0 calebharada   (501) staff       (20)      911 2023-07-14 17:01:35.000000 LTEpy-1.0.2/setup.py
+drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-14 17:54:36.628396 LTEpy-1.0.2/tests/
+-rw-r--r--   0 calebharada   (501) staff       (20)        0 2023-07-14 14:07:27.000000 LTEpy-1.0.2/tests/__init__.py
+-rw-r--r--   0 calebharada   (501) staff       (20)     2258 2023-07-14 14:07:27.000000 LTEpy-1.0.2/tests/test_atom.py
+-rw-r--r--   0 calebharada   (501) staff       (20)     1159 2023-07-14 14:07:27.000000 LTEpy-1.0.2/tests/test_boltzmann_factor.py
+-rw-r--r--   0 calebharada   (501) staff       (20)     1329 2023-07-14 14:07:27.000000 LTEpy-1.0.2/tests/test_planck.py
```

### Comparing `LTEpy-1.0.1/LICENSE` & `LTEpy-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `LTEpy-1.0.1/LTEpy/atom.py` & `LTEpy-1.0.2/LTEpy/atom.py`

 * *Files identical despite different names*

### Comparing `LTEpy-1.0.1/LTEpy/constants.py` & `LTEpy-1.0.2/LTEpy/constants.py`

 * *Files identical despite different names*

### Comparing `LTEpy-1.0.1/LTEpy/lte.py` & `LTEpy-1.0.2/LTEpy/lte.py`

 * *Files identical despite different names*

### Comparing `LTEpy-1.0.1/LTEpy/plot.py` & `LTEpy-1.0.2/LTEpy/plot.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import os
 import matplotlib.pyplot as plt
 import numpy as np
 
-ROOT_DIR = os.path.dirname(os.path.abspath(__file__))
-plt.style.use(ROOT_DIR + '/sty/custom.mplstyle')   # avoid dark backgrounds from dark theme vscode
+plt.style.use('custom.mplstyle')   # avoid dark backgrounds from dark theme vscode
 # plt.rcParams['axes.grid'] = True
 # plt.rcParams['grid.alpha'] = 0.15
 # plt.rcParams["mathtext.fontset"] = "cm"
 # plt.rcParams["font.family"] = "serif"
 # plt.rcParams["legend.handlelength"] = 1.5
 # plt.rcParams["lines.solid_capstyle"] = 'round'
```

### Comparing `LTEpy-1.0.1/README.md` & `LTEpy-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `LTEpy-1.0.1/setup.py` & `LTEpy-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `LTEpy-1.0.1/tests/test_atom.py` & `LTEpy-1.0.2/tests/test_atom.py`

 * *Files identical despite different names*

### Comparing `LTEpy-1.0.1/tests/test_boltzmann_factor.py` & `LTEpy-1.0.2/tests/test_boltzmann_factor.py`

 * *Files identical despite different names*

### Comparing `LTEpy-1.0.1/tests/test_planck.py` & `LTEpy-1.0.2/tests/test_planck.py`

 * *Files identical despite different names*

