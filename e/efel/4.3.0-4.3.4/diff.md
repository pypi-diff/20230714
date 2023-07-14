# Comparing `tmp/efel-4.3.0.tar.gz` & `tmp/efel-4.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efel-4.3.0.tar", last modified: Wed Jul 12 11:10:29 2023, max compression
+gzip compressed data, was "efel-4.3.4.tar", last modified: Fri Jul 14 10:24:51 2023, max compression
```

## Comparing `efel-4.3.0.tar` & `efel-4.3.4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 11:10:29.435202 efel-4.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)      167 2023-07-12 11:10:28.000000 efel-4.3.0/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (122)    35151 2023-07-12 11:10:28.000000 efel-4.3.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (122)     7651 2023-07-12 11:10:28.000000 efel-4.3.0/COPYING.less
--rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-07-12 11:10:28.000000 efel-4.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      126 2023-07-12 11:10:28.000000 efel-4.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-07-12 11:10:29.435202 efel-4.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7400 2023-07-12 11:10:28.000000 efel-4.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 11:10:29.435202 efel-4.3.0/efel/
--rw-r--r--   0 runner    (1001) docker     (122)    12825 2023-07-12 11:10:28.000000 efel-4.3.0/efel/DependencyV5.txt
--rw-r--r--   0 runner    (1001) docker     (122)      967 2023-07-12 11:10:28.000000 efel-4.3.0/efel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-07-12 11:10:29.435202 efel-4.3.0/efel/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)    18462 2023-07-12 11:10:28.000000 efel-4.3.0/efel/api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 11:10:29.435202 efel-4.3.0/efel/cppcore/
--rw-r--r--   0 runner    (1001) docker     (122)     6902 2023-07-12 11:10:28.000000 efel-4.3.0/efel/cppcore/DependencyTree.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-07-12 11:10:28.000000 efel-4.3.0/efel/cppcore/DependencyTree.h
--rw-r--r--   0 runner    (1001) docker     (122)    14462 2023-07-12 11:10:28.000000 efel-4.3.0/efel/cppcore/FillFptrTable.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1700 2023-07-12 11:10:28.000000 efel-4.3.0/efel/cppcore/FillFptrTable.h
--rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-07-12 11:10:28.000000 efel-4.3.0/efel/cppcore/Global.h
--rw-r--r--   0 runner    (1001) docker     (122)    69609 2023-07-12 11:10:28.000000 efel-4.3.0/efel/cppcore/LibV1.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     7239 2023-07-12 11:10:28.000000 efel-4.3.0/efel/cppcore/LibV1.h
--rw-r--r--   0 runner    (1001) docker     (122)    57446 2023-07-12 11:10:28.000000 efel-4.3.0/efel/cppcore/LibV2.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     8364 2023-07-12 11:10:28.000000 efel-4.3.0/efel/cppcore/LibV2.h
--rw-r--r--   0 runner    (1001) docker     (122)    40008 2023-07-12 11:10:28.000000 efel-4.3.0/efel/cppcore/LibV3.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     4874 2023-07-12 11:10:28.000000 efel-4.3.0/efel/cppcore/LibV3.h
--rw-r--r--   0 runner    (1001) docker     (122)     3611 2023-07-12 11:10:28.000000 efel-4.3.0/efel/cppcore/LibV4.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1596 2023-07-12 11:10:28.000000 efel-4.3.0/efel/cppcore/LibV4.h
--rw-r--r--   0 runner    (1001) docker     (122)   137180 2023-07-12 11:10:28.000000 efel-4.3.0/efel/cppcore/LibV5.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    15913 2023-07-12 11:10:28.000000 efel-4.3.0/efel/cppcore/LibV5.h
--rw-r--r--   0 runner    (1001) docker     (122)     6931 2023-07-12 11:10:28.000000 efel-4.3.0/efel/cppcore/Utils.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3430 2023-07-12 11:10:28.000000 efel-4.3.0/efel/cppcore/Utils.h
--rw-r--r--   0 runner    (1001) docker     (122)    22270 2023-07-12 11:10:28.000000 efel-4.3.0/efel/cppcore/cfeature.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3274 2023-07-12 11:10:28.000000 efel-4.3.0/efel/cppcore/cfeature.h
--rw-r--r--   0 runner    (1001) docker     (122)    10351 2023-07-12 11:10:28.000000 efel-4.3.0/efel/cppcore/cppcore.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1829 2023-07-12 11:10:28.000000 efel-4.3.0/efel/cppcore/eFELLogger.h
--rw-r--r--   0 runner    (1001) docker     (122)     3597 2023-07-12 11:10:28.000000 efel-4.3.0/efel/cppcore/efel.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2399 2023-07-12 11:10:28.000000 efel-4.3.0/efel/cppcore/efel.h
--rw-r--r--   0 runner    (1001) docker     (122)     8378 2023-07-12 11:10:28.000000 efel-4.3.0/efel/cppcore/mapoperations.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2832 2023-07-12 11:10:28.000000 efel-4.3.0/efel/cppcore/mapoperations.h
--rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-07-12 11:10:28.000000 efel-4.3.0/efel/cppcore/types.h
--rw-r--r--   0 runner    (1001) docker     (122)    10312 2023-07-12 11:10:28.000000 efel-4.3.0/efel/io.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 11:10:29.435202 efel-4.3.0/efel/pyfeatures/
--rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-07-12 11:10:28.000000 efel-4.3.0/efel/pyfeatures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10309 2023-07-12 11:10:28.000000 efel-4.3.0/efel/pyfeatures/pyfeatures.py
--rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-07-12 11:10:28.000000 efel-4.3.0/efel/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 11:10:29.435202 efel-4.3.0/efel/units/
--rw-r--r--   0 runner    (1001) docker     (122)      266 2023-07-12 11:10:28.000000 efel-4.3.0/efel/units/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4677 2023-07-12 11:10:28.000000 efel-4.3.0/efel/units/units.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 11:10:29.431201 efel-4.3.0/efel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-07-12 11:10:29.000000 efel-4.3.0/efel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-07-12 11:10:29.000000 efel-4.3.0/efel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-12 11:10:29.000000 efel-4.3.0/efel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-07-12 11:10:29.000000 efel-4.3.0/efel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-12 11:10:29.000000 efel-4.3.0/efel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      221 2023-07-12 11:10:29.435202 efel-4.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4090 2023-07-12 11:10:28.000000 efel-4.3.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)    69513 2023-07-12 11:10:28.000000 efel-4.3.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:24:51.007802 efel-4.3.4/
+-rw-r--r--   0 runner    (1001) docker     (122)      167 2023-07-14 10:24:49.000000 efel-4.3.4/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    35151 2023-07-14 10:24:49.000000 efel-4.3.4/COPYING
+-rw-r--r--   0 runner    (1001) docker     (122)     7651 2023-07-14 10:24:49.000000 efel-4.3.4/COPYING.less
+-rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-07-14 10:24:49.000000 efel-4.3.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2023-07-14 10:24:49.000000 efel-4.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-07-14 10:24:51.007802 efel-4.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7400 2023-07-14 10:24:49.000000 efel-4.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:24:51.007802 efel-4.3.4/efel/
+-rw-r--r--   0 runner    (1001) docker     (122)    12825 2023-07-14 10:24:49.000000 efel-4.3.4/efel/DependencyV5.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      967 2023-07-14 10:24:49.000000 efel-4.3.4/efel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-07-14 10:24:51.007802 efel-4.3.4/efel/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18462 2023-07-14 10:24:49.000000 efel-4.3.4/efel/api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:24:51.007802 efel-4.3.4/efel/cppcore/
+-rw-r--r--   0 runner    (1001) docker     (122)     6902 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/DependencyTree.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/DependencyTree.h
+-rw-r--r--   0 runner    (1001) docker     (122)    14462 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/FillFptrTable.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1700 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/FillFptrTable.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/Global.h
+-rw-r--r--   0 runner    (1001) docker     (122)    69609 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/LibV1.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7239 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/LibV1.h
+-rw-r--r--   0 runner    (1001) docker     (122)    57446 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/LibV2.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8364 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/LibV2.h
+-rw-r--r--   0 runner    (1001) docker     (122)    40008 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/LibV3.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4874 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/LibV3.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3611 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/LibV4.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1596 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/LibV4.h
+-rw-r--r--   0 runner    (1001) docker     (122)   137180 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/LibV5.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    15913 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/LibV5.h
+-rw-r--r--   0 runner    (1001) docker     (122)     6931 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/Utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3430 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/Utils.h
+-rw-r--r--   0 runner    (1001) docker     (122)    22270 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/cfeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3274 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/cfeature.h
+-rw-r--r--   0 runner    (1001) docker     (122)    10351 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/cppcore.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1829 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/eFELLogger.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3597 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/efel.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2399 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/efel.h
+-rw-r--r--   0 runner    (1001) docker     (122)     8378 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/mapoperations.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2832 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/mapoperations.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-07-14 10:24:49.000000 efel-4.3.4/efel/cppcore/types.h
+-rw-r--r--   0 runner    (1001) docker     (122)    10312 2023-07-14 10:24:49.000000 efel-4.3.4/efel/io.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:24:51.007802 efel-4.3.4/efel/pyfeatures/
+-rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-07-14 10:24:49.000000 efel-4.3.4/efel/pyfeatures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10309 2023-07-14 10:24:49.000000 efel-4.3.4/efel/pyfeatures/pyfeatures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-07-14 10:24:49.000000 efel-4.3.4/efel/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:24:51.007802 efel-4.3.4/efel/units/
+-rw-r--r--   0 runner    (1001) docker     (122)      266 2023-07-14 10:24:49.000000 efel-4.3.4/efel/units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4677 2023-07-14 10:24:49.000000 efel-4.3.4/efel/units/units.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:24:51.003802 efel-4.3.4/efel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-07-14 10:24:50.000000 efel-4.3.4/efel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-07-14 10:24:50.000000 efel-4.3.4/efel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-14 10:24:50.000000 efel-4.3.4/efel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-07-14 10:24:50.000000 efel-4.3.4/efel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-14 10:24:50.000000 efel-4.3.4/efel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-07-14 10:24:51.007802 efel-4.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4090 2023-07-14 10:24:49.000000 efel-4.3.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)    69513 2023-07-14 10:24:49.000000 efel-4.3.4/versioneer.py
```

### Comparing `efel-4.3.0/COPYING` & `efel-4.3.4/COPYING`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/COPYING.less` & `efel-4.3.4/COPYING.less`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/LICENSE.txt` & `efel-4.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/PKG-INFO` & `efel-4.3.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efel
-Version: 4.3.0
+Version: 4.3.4
 Summary: Electrophys Feature Extract Library (eFEL)
 Home-page: https://github.com/BlueBrain/eFEL
 Author: BlueBrain Project, EPFL
 Maintainer: Werner Van Geit
 Maintainer-email: werner.vangeit@epfl.ch
 License: LGPLv3
 Keywords: feature,extraction,electrophysiology,BlueBrainProject
```

### Comparing `efel-4.3.0/README.md` & `efel-4.3.4/README.md`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/efel/DependencyV5.txt` & `efel-4.3.4/efel/DependencyV5.txt`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/efel/__init__.py` & `efel-4.3.4/efel/__init__.py`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/efel/api.py` & `efel-4.3.4/efel/api.py`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/efel/cppcore/DependencyTree.cpp` & `efel-4.3.4/efel/cppcore/DependencyTree.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/efel/cppcore/DependencyTree.h` & `efel-4.3.4/efel/cppcore/DependencyTree.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/efel/cppcore/FillFptrTable.cpp` & `efel-4.3.4/efel/cppcore/FillFptrTable.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/efel/cppcore/FillFptrTable.h` & `efel-4.3.4/efel/cppcore/FillFptrTable.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/efel/cppcore/Global.h` & `efel-4.3.4/efel/cppcore/Global.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/efel/cppcore/LibV1.cpp` & `efel-4.3.4/efel/cppcore/LibV1.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/efel/cppcore/LibV1.h` & `efel-4.3.4/efel/cppcore/LibV1.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/efel/cppcore/LibV2.cpp` & `efel-4.3.4/efel/cppcore/LibV2.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/efel/cppcore/LibV2.h` & `efel-4.3.4/efel/cppcore/LibV2.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/efel/cppcore/LibV3.cpp` & `efel-4.3.4/efel/cppcore/LibV3.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/efel/cppcore/LibV3.h` & `efel-4.3.4/efel/cppcore/LibV3.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/efel/cppcore/LibV4.cpp` & `efel-4.3.4/efel/cppcore/LibV4.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/efel/cppcore/LibV4.h` & `efel-4.3.4/efel/cppcore/LibV4.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/efel/cppcore/LibV5.cpp` & `efel-4.3.4/efel/cppcore/LibV5.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/efel/cppcore/LibV5.h` & `efel-4.3.4/efel/cppcore/LibV5.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/efel/cppcore/Utils.cpp` & `efel-4.3.4/efel/cppcore/Utils.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/efel/cppcore/Utils.h` & `efel-4.3.4/efel/cppcore/Utils.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/efel/cppcore/cfeature.cpp` & `efel-4.3.4/efel/cppcore/cfeature.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/efel/cppcore/cfeature.h` & `efel-4.3.4/efel/cppcore/cfeature.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/efel/cppcore/cppcore.cpp` & `efel-4.3.4/efel/cppcore/cppcore.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/efel/cppcore/eFELLogger.h` & `efel-4.3.4/efel/cppcore/eFELLogger.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/efel/cppcore/efel.cpp` & `efel-4.3.4/efel/cppcore/efel.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/efel/cppcore/efel.h` & `efel-4.3.4/efel/cppcore/efel.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/efel/cppcore/mapoperations.cpp` & `efel-4.3.4/efel/cppcore/mapoperations.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/efel/cppcore/mapoperations.h` & `efel-4.3.4/efel/cppcore/mapoperations.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/efel/cppcore/types.h` & `efel-4.3.4/efel/cppcore/types.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/efel/io.py` & `efel-4.3.4/efel/io.py`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/efel/pyfeatures/__init__.py` & `efel-4.3.4/efel/pyfeatures/__init__.py`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/efel/pyfeatures/pyfeatures.py` & `efel-4.3.4/efel/pyfeatures/pyfeatures.py`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/efel/settings.py` & `efel-4.3.4/efel/settings.py`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/efel/units/units.json` & `efel-4.3.4/efel/units/units.json`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/efel.egg-info/PKG-INFO` & `efel-4.3.4/efel.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efel
-Version: 4.3.0
+Version: 4.3.4
 Summary: Electrophys Feature Extract Library (eFEL)
 Home-page: https://github.com/BlueBrain/eFEL
 Author: BlueBrain Project, EPFL
 Maintainer: Werner Van Geit
 Maintainer-email: werner.vangeit@epfl.ch
 License: LGPLv3
 Keywords: feature,extraction,electrophysiology,BlueBrainProject
```

### Comparing `efel-4.3.0/efel.egg-info/SOURCES.txt` & `efel-4.3.4/efel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/setup.py` & `efel-4.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `efel-4.3.0/versioneer.py` & `efel-4.3.4/versioneer.py`

 * *Files identical despite different names*

