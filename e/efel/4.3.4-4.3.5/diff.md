# Comparing `tmp/efel-4.3.4.tar.gz` & `tmp/efel-4.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efel-4.3.4.tar", last modified: Fri Jul 14 10:24:51 2023, max compression
+gzip compressed data, was "efel-4.3.5.tar", last modified: Fri Jul 14 11:51:49 2023, max compression
```

## Comparing `efel-4.3.4.tar` & `efel-4.3.5.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:24:51.007802 efel-4.3.4/
--rw-r--r--   0 runner    (1001) docker     (122)      167 2023-07-14 10:24:49.000000 efel-4.3.4/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (122)    35151 2023-07-14 10:24:49.000000 efel-4.3.4/COPYING
--rw-r--r--   0 runner    (1001) docker     (122)     7651 2023-07-14 10:24:49.000000 efel-4.3.4/COPYING.less
--rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-07-14 10:24:49.000000 efel-4.3.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      126 2023-07-14 10:24:49.000000 efel-4.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-07-14 10:24:51.007802 efel-4.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7400 2023-07-14 10:24:49.000000 efel-4.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:24:51.007802 efel-4.3.4/efel/
--rw-r--r--   0 runner    (1001) docker     (122)    12825 2023-07-14 10:24:49.000000 efel-4.3.4/efel/DependencyV5.txt
--rw-r--r--   0 runner    (1001) docker     (122)      967 2023-07-14 10:24:49.000000 efel-4.3.4/efel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-07-14 10:24:51.007802 efel-4.3.4/efel/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)    18462 2023-07-14 10:24:49.000000 efel-4.3.4/efel/api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:24:51.007802 efel-4.3.4/efel/cppcore/
--rw-r--r--   0 runner    (1001) docker     (122)     6902 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/DependencyTree.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/DependencyTree.h
--rw-r--r--   0 runner    (1001) docker     (122)    14462 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/FillFptrTable.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1700 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/FillFptrTable.h
--rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/Global.h
--rw-r--r--   0 runner    (1001) docker     (122)    69609 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/LibV1.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     7239 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/LibV1.h
--rw-r--r--   0 runner    (1001) docker     (122)    57446 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/LibV2.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     8364 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/LibV2.h
--rw-r--r--   0 runner    (1001) docker     (122)    40008 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/LibV3.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     4874 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/LibV3.h
--rw-r--r--   0 runner    (1001) docker     (122)     3611 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/LibV4.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1596 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/LibV4.h
--rw-r--r--   0 runner    (1001) docker     (122)   137180 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/LibV5.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    15913 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/LibV5.h
--rw-r--r--   0 runner    (1001) docker     (122)     6931 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/Utils.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3430 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/Utils.h
--rw-r--r--   0 runner    (1001) docker     (122)    22270 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/cfeature.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3274 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/cfeature.h
--rw-r--r--   0 runner    (1001) docker     (122)    10351 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/cppcore.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1829 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/eFELLogger.h
--rw-r--r--   0 runner    (1001) docker     (122)     3597 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/efel.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2399 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/efel.h
--rw-r--r--   0 runner    (1001) docker     (122)     8378 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/mapoperations.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2832 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/mapoperations.h
--rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/types.h
--rw-r--r--   0 runner    (1001) docker     (122)    10312 2023-07-14 10:24:49.000000 efel-4.3.4/efel/io.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:24:51.007802 efel-4.3.4/efel/pyfeatures/
--rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-07-14 10:24:49.000000 efel-4.3.4/efel/pyfeatures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10309 2023-07-14 10:24:49.000000 efel-4.3.4/efel/pyfeatures/pyfeatures.py
--rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-07-14 10:24:49.000000 efel-4.3.4/efel/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:24:51.007802 efel-4.3.4/efel/units/
--rw-r--r--   0 runner    (1001) docker     (122)      266 2023-07-14 10:24:49.000000 efel-4.3.4/efel/units/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4677 2023-07-14 10:24:49.000000 efel-4.3.4/efel/units/units.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:24:51.003802 efel-4.3.4/efel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-07-14 10:24:50.000000 efel-4.3.4/efel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-07-14 10:24:50.000000 efel-4.3.4/efel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-14 10:24:50.000000 efel-4.3.4/efel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-07-14 10:24:50.000000 efel-4.3.4/efel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-14 10:24:50.000000 efel-4.3.4/efel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      221 2023-07-14 10:24:51.007802 efel-4.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4090 2023-07-14 10:24:49.000000 efel-4.3.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)    69513 2023-07-14 10:24:49.000000 efel-4.3.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 11:51:49.624136 efel-4.3.5/
+-rw-r--r--   0 runner    (1001) docker     (122)      167 2023-07-14 11:51:48.000000 efel-4.3.5/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    35151 2023-07-14 11:51:48.000000 efel-4.3.5/COPYING
+-rw-r--r--   0 runner    (1001) docker     (122)     7651 2023-07-14 11:51:48.000000 efel-4.3.5/COPYING.less
+-rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-07-14 11:51:48.000000 efel-4.3.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2023-07-14 11:51:48.000000 efel-4.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-07-14 11:51:49.624136 efel-4.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     8785 2023-07-14 11:51:48.000000 efel-4.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 11:51:49.624136 efel-4.3.5/efel/
+-rw-r--r--   0 runner    (1001) docker     (122)    12825 2023-07-14 11:51:48.000000 efel-4.3.5/efel/DependencyV5.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      967 2023-07-14 11:51:48.000000 efel-4.3.5/efel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-07-14 11:51:49.624136 efel-4.3.5/efel/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18462 2023-07-14 11:51:48.000000 efel-4.3.5/efel/api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 11:51:49.620136 efel-4.3.5/efel/cppcore/
+-rw-r--r--   0 runner    (1001) docker     (122)     6902 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/DependencyTree.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/DependencyTree.h
+-rw-r--r--   0 runner    (1001) docker     (122)    14462 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/FillFptrTable.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1700 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/FillFptrTable.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/Global.h
+-rw-r--r--   0 runner    (1001) docker     (122)    69609 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/LibV1.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7239 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/LibV1.h
+-rw-r--r--   0 runner    (1001) docker     (122)    57446 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/LibV2.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8364 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/LibV2.h
+-rw-r--r--   0 runner    (1001) docker     (122)    40008 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/LibV3.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4874 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/LibV3.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3611 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/LibV4.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1596 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/LibV4.h
+-rw-r--r--   0 runner    (1001) docker     (122)   137180 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/LibV5.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    15913 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/LibV5.h
+-rw-r--r--   0 runner    (1001) docker     (122)     6931 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/Utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3430 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/Utils.h
+-rw-r--r--   0 runner    (1001) docker     (122)    22270 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/cfeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3274 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/cfeature.h
+-rw-r--r--   0 runner    (1001) docker     (122)    10351 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/cppcore.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1829 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/eFELLogger.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3597 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/efel.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2399 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/efel.h
+-rw-r--r--   0 runner    (1001) docker     (122)     8378 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/mapoperations.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2832 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/mapoperations.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/types.h
+-rw-r--r--   0 runner    (1001) docker     (122)    10312 2023-07-14 11:51:48.000000 efel-4.3.5/efel/io.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 11:51:49.620136 efel-4.3.5/efel/pyfeatures/
+-rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-07-14 11:51:48.000000 efel-4.3.5/efel/pyfeatures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10309 2023-07-14 11:51:48.000000 efel-4.3.5/efel/pyfeatures/pyfeatures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-07-14 11:51:48.000000 efel-4.3.5/efel/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 11:51:49.624136 efel-4.3.5/efel/units/
+-rw-r--r--   0 runner    (1001) docker     (122)      266 2023-07-14 11:51:48.000000 efel-4.3.5/efel/units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4677 2023-07-14 11:51:48.000000 efel-4.3.5/efel/units/units.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 11:51:49.616136 efel-4.3.5/efel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-07-14 11:51:49.000000 efel-4.3.5/efel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-07-14 11:51:49.000000 efel-4.3.5/efel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-14 11:51:49.000000 efel-4.3.5/efel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-07-14 11:51:49.000000 efel-4.3.5/efel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-14 11:51:49.000000 efel-4.3.5/efel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-07-14 11:51:49.624136 efel-4.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4090 2023-07-14 11:51:48.000000 efel-4.3.5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)    69513 2023-07-14 11:51:48.000000 efel-4.3.5/versioneer.py
```

### Comparing `efel-4.3.4/COPYING` & `efel-4.3.5/COPYING`

 * *Files identical despite different names*

### Comparing `efel-4.3.4/COPYING.less` & `efel-4.3.5/COPYING.less`

 * *Files identical despite different names*

### Comparing `efel-4.3.4/LICENSE.txt` & `efel-4.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `efel-4.3.4/PKG-INFO` & `efel-4.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efel
-Version: 4.3.4
+Version: 4.3.5
 Summary: Electrophys Feature Extract Library (eFEL)
 Home-page: https://github.com/BlueBrain/eFEL
 Author: BlueBrain Project, EPFL
 Maintainer: Werner Van Geit
 Maintainer-email: werner.vangeit@epfl.ch
 License: LGPLv3
 Keywords: feature,extraction,electrophysiology,BlueBrainProject
```

### Comparing `efel-4.3.4/README.md` & `efel-4.3.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -41,15 +41,23 @@
     </a>
   </td>
 </tr>
 <tr>
     <td>Gitter</td>
     <td>
         <a href="https://gitter.im/bluebrain/efel">
-        <img src="https://badges.gitter.im/Join%20Chat.svg"
+        <img src="https://badges.gitter.im/Join%20Chat.svg" />
+    </a>
+    </td>
+</tr>
+<tr>
+    <td>Citation</td>
+    <td>
+        <a href="https://doi.org/10.5281/zenodo.593869">
+        <img src="https://zenodo.org/badge/DOI/10.5281/zenodo.8146607.svg" alt="DOI"/>
     </a>
     </td>
 </tr>
 </table>
 
 Introduction
 ============
@@ -64,14 +72,40 @@
 the values to the user.
 
 The core of the library is written in C++, and a Python wrapper is included.
 At the moment we provide a way to automatically compile and install the library
 as a Python module. Instructions on how to compile the eFEL as a standalone C++ 
 library can be found [here](http://efel.readthedocs.io/en/latest/installation.html#installing-the-c-standalone-library).
 
+
+Citation
+========
+
+When you use this eFEL software for your research, we ask you to cite the following publications (this includes poster presentations):
+
+```
+    @article{efel, 
+        title={eFEL}, 
+        DOI={10.5281/zenodo.593869},
+        url={https://doi.org/10.5281/zenodo.593869} 
+        abstractNote={The Electrophys Feature Extraction Library (eFEL) allows neuroscientists to automatically extract features from time series data recorded from neurons (both in vitro and in silico). Examples are the action potential width and amplitude in voltage traces recorded during whole-cell patch clamp experiments. The user of the library provides a set of traces and selects the features to be calculated. The library will then extract the requested features and return the values to the user.}, 
+        publisher={Zenodo}, 
+        author={Ranjan, Rajnish and
+                Van Geit, Werner and
+                Moor, Ruben and
+                Rössert, Christian and
+                Riquelme, Juan Luis and
+                Damart, Tanguy and
+                Jaquier, Aurélien and
+                Tuncel, Anil},
+        year={2023}, 
+        month={Jul} 
+    }
+```
+
 News
 ====
 
 * 2023/01/04: We dropped support for Python 3.6. The eFEL code isn't automatically tested on 3.6 anymore.
 
 * 2021/08/25: We dropped support for Python 2.7. The eFEL code isn't automatically tested on 2.7 anymore.
```

### Comparing `efel-4.3.4/efel/DependencyV5.txt` & `efel-4.3.5/efel/DependencyV5.txt`

 * *Files identical despite different names*

### Comparing `efel-4.3.4/efel/__init__.py` & `efel-4.3.5/efel/__init__.py`

 * *Files identical despite different names*

### Comparing `efel-4.3.4/efel/api.py` & `efel-4.3.5/efel/api.py`

 * *Files identical despite different names*

### Comparing `efel-4.3.4/efel/cppcore/DependencyTree.cpp` & `efel-4.3.5/efel/cppcore/DependencyTree.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.3.4/efel/cppcore/DependencyTree.h` & `efel-4.3.5/efel/cppcore/DependencyTree.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.4/efel/cppcore/FillFptrTable.cpp` & `efel-4.3.5/efel/cppcore/FillFptrTable.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.3.4/efel/cppcore/FillFptrTable.h` & `efel-4.3.5/efel/cppcore/FillFptrTable.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.4/efel/cppcore/Global.h` & `efel-4.3.5/efel/cppcore/Global.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.4/efel/cppcore/LibV1.cpp` & `efel-4.3.5/efel/cppcore/LibV1.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.3.4/efel/cppcore/LibV1.h` & `efel-4.3.5/efel/cppcore/LibV1.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.4/efel/cppcore/LibV2.cpp` & `efel-4.3.5/efel/cppcore/LibV2.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.3.4/efel/cppcore/LibV2.h` & `efel-4.3.5/efel/cppcore/LibV2.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.4/efel/cppcore/LibV3.cpp` & `efel-4.3.5/efel/cppcore/LibV3.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.3.4/efel/cppcore/LibV3.h` & `efel-4.3.5/efel/cppcore/LibV3.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.4/efel/cppcore/LibV4.cpp` & `efel-4.3.5/efel/cppcore/LibV4.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.3.4/efel/cppcore/LibV4.h` & `efel-4.3.5/efel/cppcore/LibV4.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.4/efel/cppcore/LibV5.cpp` & `efel-4.3.5/efel/cppcore/LibV5.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.3.4/efel/cppcore/LibV5.h` & `efel-4.3.5/efel/cppcore/LibV5.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.4/efel/cppcore/Utils.cpp` & `efel-4.3.5/efel/cppcore/Utils.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.3.4/efel/cppcore/Utils.h` & `efel-4.3.5/efel/cppcore/Utils.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.4/efel/cppcore/cfeature.cpp` & `efel-4.3.5/efel/cppcore/cfeature.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.3.4/efel/cppcore/cfeature.h` & `efel-4.3.5/efel/cppcore/cfeature.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.4/efel/cppcore/cppcore.cpp` & `efel-4.3.5/efel/cppcore/cppcore.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.3.4/efel/cppcore/eFELLogger.h` & `efel-4.3.5/efel/cppcore/eFELLogger.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.4/efel/cppcore/efel.cpp` & `efel-4.3.5/efel/cppcore/efel.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.3.4/efel/cppcore/efel.h` & `efel-4.3.5/efel/cppcore/efel.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.4/efel/cppcore/mapoperations.cpp` & `efel-4.3.5/efel/cppcore/mapoperations.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.3.4/efel/cppcore/mapoperations.h` & `efel-4.3.5/efel/cppcore/mapoperations.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.4/efel/cppcore/types.h` & `efel-4.3.5/efel/cppcore/types.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.4/efel/io.py` & `efel-4.3.5/efel/io.py`

 * *Files identical despite different names*

### Comparing `efel-4.3.4/efel/pyfeatures/__init__.py` & `efel-4.3.5/efel/pyfeatures/__init__.py`

 * *Files identical despite different names*

### Comparing `efel-4.3.4/efel/pyfeatures/pyfeatures.py` & `efel-4.3.5/efel/pyfeatures/pyfeatures.py`

 * *Files identical despite different names*

### Comparing `efel-4.3.4/efel/settings.py` & `efel-4.3.5/efel/settings.py`

 * *Files identical despite different names*

### Comparing `efel-4.3.4/efel/units/units.json` & `efel-4.3.5/efel/units/units.json`

 * *Files identical despite different names*

### Comparing `efel-4.3.4/efel.egg-info/PKG-INFO` & `efel-4.3.5/efel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efel
-Version: 4.3.4
+Version: 4.3.5
 Summary: Electrophys Feature Extract Library (eFEL)
 Home-page: https://github.com/BlueBrain/eFEL
 Author: BlueBrain Project, EPFL
 Maintainer: Werner Van Geit
 Maintainer-email: werner.vangeit@epfl.ch
 License: LGPLv3
 Keywords: feature,extraction,electrophysiology,BlueBrainProject
```

### Comparing `efel-4.3.4/efel.egg-info/SOURCES.txt` & `efel-4.3.5/efel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `efel-4.3.4/setup.py` & `efel-4.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `efel-4.3.4/versioneer.py` & `efel-4.3.5/versioneer.py`

 * *Files identical despite different names*

