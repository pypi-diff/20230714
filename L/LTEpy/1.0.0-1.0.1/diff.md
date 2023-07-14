# Comparing `tmp/LTEpy-1.0.0.tar.gz` & `tmp/LTEpy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LTEpy-1.0.0.tar", last modified: Fri Jul 14 15:20:01 2023, max compression
+gzip compressed data, was "LTEpy-1.0.1.tar", last modified: Fri Jul 14 16:28:28 2023, max compression
```

## Comparing `LTEpy-1.0.0.tar` & `LTEpy-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-14 15:20:01.625787 LTEpy-1.0.0/
--rw-r--r--   0 calebharada   (501) staff       (20)     1089 2023-07-14 14:07:27.000000 LTEpy-1.0.0/LICENSE
-drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-14 15:20:01.622343 LTEpy-1.0.0/LTEpy/
--rw-r--r--   0 calebharada   (501) staff       (20)       21 2023-07-14 15:16:18.000000 LTEpy-1.0.0/LTEpy/__init__.py
--rw-r--r--   0 calebharada   (501) staff       (20)     3275 2023-07-14 14:07:27.000000 LTEpy-1.0.0/LTEpy/atom.py
--rw-r--r--   0 calebharada   (501) staff       (20)     2033 2023-07-12 16:10:18.000000 LTEpy-1.0.0/LTEpy/constants.py
--rw-r--r--   0 calebharada   (501) staff       (20)    11933 2023-07-14 14:07:27.000000 LTEpy-1.0.0/LTEpy/lte.py
--rw-r--r--   0 calebharada   (501) staff       (20)     5354 2023-07-14 14:07:27.000000 LTEpy-1.0.0/LTEpy/plot.py
-drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-14 15:20:01.623693 LTEpy-1.0.0/LTEpy.egg-info/
--rw-r--r--   0 calebharada   (501) staff       (20)      335 2023-07-14 15:20:01.000000 LTEpy-1.0.0/LTEpy.egg-info/PKG-INFO
--rw-r--r--   0 calebharada   (501) staff       (20)      309 2023-07-14 15:20:01.000000 LTEpy-1.0.0/LTEpy.egg-info/SOURCES.txt
--rw-r--r--   0 calebharada   (501) staff       (20)        1 2023-07-14 15:20:01.000000 LTEpy-1.0.0/LTEpy.egg-info/dependency_links.txt
--rw-r--r--   0 calebharada   (501) staff       (20)       12 2023-07-14 15:20:01.000000 LTEpy-1.0.0/LTEpy.egg-info/top_level.txt
--rw-r--r--   0 calebharada   (501) staff       (20)      335 2023-07-14 15:20:01.625477 LTEpy-1.0.0/PKG-INFO
--rw-r--r--   0 calebharada   (501) staff       (20)     1199 2023-07-14 15:16:18.000000 LTEpy-1.0.0/README.md
--rw-r--r--   0 calebharada   (501) staff       (20)       38 2023-07-14 15:20:01.625915 LTEpy-1.0.0/setup.cfg
--rw-r--r--   0 calebharada   (501) staff       (20)      875 2023-07-12 17:59:38.000000 LTEpy-1.0.0/setup.py
-drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-14 15:20:01.625019 LTEpy-1.0.0/tests/
--rw-r--r--   0 calebharada   (501) staff       (20)        0 2023-07-14 14:07:27.000000 LTEpy-1.0.0/tests/__init__.py
--rw-r--r--   0 calebharada   (501) staff       (20)     2258 2023-07-14 14:07:27.000000 LTEpy-1.0.0/tests/test_atom.py
--rw-r--r--   0 calebharada   (501) staff       (20)     1159 2023-07-14 14:07:27.000000 LTEpy-1.0.0/tests/test_boltzmann_factor.py
--rw-r--r--   0 calebharada   (501) staff       (20)     1329 2023-07-14 14:07:27.000000 LTEpy-1.0.0/tests/test_planck.py
+drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-14 16:28:28.913709 LTEpy-1.0.1/
+-rw-r--r--   0 calebharada   (501) staff       (20)     1089 2023-07-14 14:07:27.000000 LTEpy-1.0.1/LICENSE
+drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-14 16:28:28.909055 LTEpy-1.0.1/LTEpy/
+-rw-r--r--   0 calebharada   (501) staff       (20)       21 2023-07-14 16:27:32.000000 LTEpy-1.0.1/LTEpy/__init__.py
+-rw-r--r--   0 calebharada   (501) staff       (20)     3275 2023-07-14 14:07:27.000000 LTEpy-1.0.1/LTEpy/atom.py
+-rw-r--r--   0 calebharada   (501) staff       (20)     2033 2023-07-12 16:10:18.000000 LTEpy-1.0.1/LTEpy/constants.py
+-rw-r--r--   0 calebharada   (501) staff       (20)    11933 2023-07-14 14:07:27.000000 LTEpy-1.0.1/LTEpy/lte.py
+-rw-r--r--   0 calebharada   (501) staff       (20)     5354 2023-07-14 14:07:27.000000 LTEpy-1.0.1/LTEpy/plot.py
+drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-14 16:28:28.911325 LTEpy-1.0.1/LTEpy.egg-info/
+-rw-r--r--   0 calebharada   (501) staff       (20)      335 2023-07-14 16:28:28.000000 LTEpy-1.0.1/LTEpy.egg-info/PKG-INFO
+-rw-r--r--   0 calebharada   (501) staff       (20)      337 2023-07-14 16:28:28.000000 LTEpy-1.0.1/LTEpy.egg-info/SOURCES.txt
+-rw-r--r--   0 calebharada   (501) staff       (20)        1 2023-07-14 16:28:28.000000 LTEpy-1.0.1/LTEpy.egg-info/dependency_links.txt
+-rw-r--r--   0 calebharada   (501) staff       (20)       32 2023-07-14 16:28:28.000000 LTEpy-1.0.1/LTEpy.egg-info/requires.txt
+-rw-r--r--   0 calebharada   (501) staff       (20)       12 2023-07-14 16:28:28.000000 LTEpy-1.0.1/LTEpy.egg-info/top_level.txt
+-rw-r--r--   0 calebharada   (501) staff       (20)      335 2023-07-14 16:28:28.913349 LTEpy-1.0.1/PKG-INFO
+-rw-r--r--   0 calebharada   (501) staff       (20)     1252 2023-07-14 16:25:00.000000 LTEpy-1.0.1/README.md
+-rw-r--r--   0 calebharada   (501) staff       (20)       38 2023-07-14 16:28:28.913802 LTEpy-1.0.1/setup.cfg
+-rw-r--r--   0 calebharada   (501) staff       (20)      911 2023-07-14 16:24:05.000000 LTEpy-1.0.1/setup.py
+drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-14 16:28:28.912926 LTEpy-1.0.1/tests/
+-rw-r--r--   0 calebharada   (501) staff       (20)        0 2023-07-14 14:07:27.000000 LTEpy-1.0.1/tests/__init__.py
+-rw-r--r--   0 calebharada   (501) staff       (20)     2258 2023-07-14 14:07:27.000000 LTEpy-1.0.1/tests/test_atom.py
+-rw-r--r--   0 calebharada   (501) staff       (20)     1159 2023-07-14 14:07:27.000000 LTEpy-1.0.1/tests/test_boltzmann_factor.py
+-rw-r--r--   0 calebharada   (501) staff       (20)     1329 2023-07-14 14:07:27.000000 LTEpy-1.0.1/tests/test_planck.py
```

### Comparing `LTEpy-1.0.0/LICENSE` & `LTEpy-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `LTEpy-1.0.0/LTEpy/atom.py` & `LTEpy-1.0.1/LTEpy/atom.py`

 * *Files identical despite different names*

### Comparing `LTEpy-1.0.0/LTEpy/constants.py` & `LTEpy-1.0.1/LTEpy/constants.py`

 * *Files identical despite different names*

### Comparing `LTEpy-1.0.0/LTEpy/lte.py` & `LTEpy-1.0.1/LTEpy/lte.py`

 * *Files identical despite different names*

### Comparing `LTEpy-1.0.0/LTEpy/plot.py` & `LTEpy-1.0.1/LTEpy/plot.py`

 * *Files identical despite different names*

### Comparing `LTEpy-1.0.0/README.md` & `LTEpy-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,24 +3,27 @@
 LTEpy is a python package for calculating and visualizing functions in local thermodynamic equilibrium, including:
 * The Planck Function for black body radiation
 * The Maxwell Boltzmann Distribution
 * The Boltzmann Factors for an atom's energy levels
 
 # Installation
 
-Install LTEpy with pip using
-`pip install LTEpy`
+Install LTEpy and its requirements with pip using
+
+`pip install -e LTEpy -r LTEpy/requirements.txt`
+
 
 # Documentation
 
 See documentation and tutorials on [readthedocs](https://ltepy.readthedocs.io/en/latest/).
 
 # Attribution
 
 For attribution, cite the [LTEpy zenodo](https://zenodo.org/record/8139888).
+
 LTEpy uses an [MIT license](LICENSE).
 
 # Acknowledgements
 This package was developed at the [code/astro](https://semaphorep.github.io/codeastro/) workshop. Special thanks to the code/astro instructors, Sarah Blunt, Matthew Hosek, and Jason Wang, and the teaching assistant overseeing this project, Simon Ko.
 
 
 [![Code/Astro](https://img.shields.io/badge/Made%20at-Code/Astro-blueviolet.svg)](https://semaphorep.github.io/codeastro/)
```

### Comparing `LTEpy-1.0.0/setup.py` & `LTEpy-1.0.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,10 +20,10 @@
     name="LTEpy",
     version=get_property("__version__", "LTEpy"),
     description="LTEpy is a package for calculating and vizualing properties of a gas in local thermodynamic equilibrium.",
     packages=find_packages(),
     author="Gardiner, E. C., Harada, C.",
     author_email="ecg@berkeley.edu, charada@berkeley.edu",
     license="MIT",
-    url="https://github.com/CalebHarada/LTEpy"
-
+    url="https://github.com/CalebHarada/LTEpy",
+    install_requires=get_requires()
 )
```

### Comparing `LTEpy-1.0.0/tests/test_atom.py` & `LTEpy-1.0.1/tests/test_atom.py`

 * *Files identical despite different names*

### Comparing `LTEpy-1.0.0/tests/test_boltzmann_factor.py` & `LTEpy-1.0.1/tests/test_boltzmann_factor.py`

 * *Files identical despite different names*

### Comparing `LTEpy-1.0.0/tests/test_planck.py` & `LTEpy-1.0.1/tests/test_planck.py`

 * *Files identical despite different names*

