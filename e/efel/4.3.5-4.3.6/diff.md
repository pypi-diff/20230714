# Comparing `tmp/efel-4.3.5.tar.gz` & `tmp/efel-4.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efel-4.3.5.tar", last modified: Fri Jul 14 11:51:49 2023, max compression
+gzip compressed data, was "efel-4.3.6.tar", last modified: Fri Jul 14 13:13:23 2023, max compression
```

## Comparing `efel-4.3.5.tar` & `efel-4.3.6.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 11:51:49.624136 efel-4.3.5/
--rw-r--r--   0 runner    (1001) docker     (122)      167 2023-07-14 11:51:48.000000 efel-4.3.5/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (122)    35151 2023-07-14 11:51:48.000000 efel-4.3.5/COPYING
--rw-r--r--   0 runner    (1001) docker     (122)     7651 2023-07-14 11:51:48.000000 efel-4.3.5/COPYING.less
--rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-07-14 11:51:48.000000 efel-4.3.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      126 2023-07-14 11:51:48.000000 efel-4.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-07-14 11:51:49.624136 efel-4.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     8785 2023-07-14 11:51:48.000000 efel-4.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 11:51:49.624136 efel-4.3.5/efel/
--rw-r--r--   0 runner    (1001) docker     (122)    12825 2023-07-14 11:51:48.000000 efel-4.3.5/efel/DependencyV5.txt
--rw-r--r--   0 runner    (1001) docker     (122)      967 2023-07-14 11:51:48.000000 efel-4.3.5/efel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-07-14 11:51:49.624136 efel-4.3.5/efel/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)    18462 2023-07-14 11:51:48.000000 efel-4.3.5/efel/api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 11:51:49.620136 efel-4.3.5/efel/cppcore/
--rw-r--r--   0 runner    (1001) docker     (122)     6902 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/DependencyTree.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/DependencyTree.h
--rw-r--r--   0 runner    (1001) docker     (122)    14462 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/FillFptrTable.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1700 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/FillFptrTable.h
--rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/Global.h
--rw-r--r--   0 runner    (1001) docker     (122)    69609 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/LibV1.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     7239 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/LibV1.h
--rw-r--r--   0 runner    (1001) docker     (122)    57446 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/LibV2.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     8364 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/LibV2.h
--rw-r--r--   0 runner    (1001) docker     (122)    40008 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/LibV3.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     4874 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/LibV3.h
--rw-r--r--   0 runner    (1001) docker     (122)     3611 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/LibV4.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1596 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/LibV4.h
--rw-r--r--   0 runner    (1001) docker     (122)   137180 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/LibV5.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    15913 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/LibV5.h
--rw-r--r--   0 runner    (1001) docker     (122)     6931 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/Utils.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3430 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/Utils.h
--rw-r--r--   0 runner    (1001) docker     (122)    22270 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/cfeature.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3274 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/cfeature.h
--rw-r--r--   0 runner    (1001) docker     (122)    10351 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/cppcore.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1829 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/eFELLogger.h
--rw-r--r--   0 runner    (1001) docker     (122)     3597 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/efel.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2399 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/efel.h
--rw-r--r--   0 runner    (1001) docker     (122)     8378 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/mapoperations.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2832 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/mapoperations.h
--rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-07-14 11:51:48.000000 efel-4.3.5/efel/cppcore/types.h
--rw-r--r--   0 runner    (1001) docker     (122)    10312 2023-07-14 11:51:48.000000 efel-4.3.5/efel/io.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 11:51:49.620136 efel-4.3.5/efel/pyfeatures/
--rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-07-14 11:51:48.000000 efel-4.3.5/efel/pyfeatures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10309 2023-07-14 11:51:48.000000 efel-4.3.5/efel/pyfeatures/pyfeatures.py
--rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-07-14 11:51:48.000000 efel-4.3.5/efel/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 11:51:49.624136 efel-4.3.5/efel/units/
--rw-r--r--   0 runner    (1001) docker     (122)      266 2023-07-14 11:51:48.000000 efel-4.3.5/efel/units/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4677 2023-07-14 11:51:48.000000 efel-4.3.5/efel/units/units.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 11:51:49.616136 efel-4.3.5/efel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-07-14 11:51:49.000000 efel-4.3.5/efel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-07-14 11:51:49.000000 efel-4.3.5/efel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-14 11:51:49.000000 efel-4.3.5/efel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-07-14 11:51:49.000000 efel-4.3.5/efel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-14 11:51:49.000000 efel-4.3.5/efel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      221 2023-07-14 11:51:49.624136 efel-4.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4090 2023-07-14 11:51:48.000000 efel-4.3.5/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)    69513 2023-07-14 11:51:48.000000 efel-4.3.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:23.119804 efel-4.3.6/
+-rw-r--r--   0 runner    (1001) docker     (122)      167 2023-07-14 13:13:21.000000 efel-4.3.6/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    35151 2023-07-14 13:13:21.000000 efel-4.3.6/COPYING
+-rw-r--r--   0 runner    (1001) docker     (122)     7651 2023-07-14 13:13:21.000000 efel-4.3.6/COPYING.less
+-rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-07-14 13:13:21.000000 efel-4.3.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2023-07-14 13:13:21.000000 efel-4.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-07-14 13:13:23.119804 efel-4.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     8785 2023-07-14 13:13:21.000000 efel-4.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:23.119804 efel-4.3.6/efel/
+-rw-r--r--   0 runner    (1001) docker     (122)    12825 2023-07-14 13:13:21.000000 efel-4.3.6/efel/DependencyV5.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      967 2023-07-14 13:13:21.000000 efel-4.3.6/efel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-07-14 13:13:23.119804 efel-4.3.6/efel/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18462 2023-07-14 13:13:21.000000 efel-4.3.6/efel/api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:23.115804 efel-4.3.6/efel/cppcore/
+-rw-r--r--   0 runner    (1001) docker     (122)     6902 2023-07-14 13:13:21.000000 efel-4.3.6/efel/cppcore/DependencyTree.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-07-14 13:13:21.000000 efel-4.3.6/efel/cppcore/DependencyTree.h
+-rw-r--r--   0 runner    (1001) docker     (122)    14462 2023-07-14 13:13:21.000000 efel-4.3.6/efel/cppcore/FillFptrTable.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1700 2023-07-14 13:13:21.000000 efel-4.3.6/efel/cppcore/FillFptrTable.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-07-14 13:13:21.000000 efel-4.3.6/efel/cppcore/Global.h
+-rw-r--r--   0 runner    (1001) docker     (122)    69609 2023-07-14 13:13:21.000000 efel-4.3.6/efel/cppcore/LibV1.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7239 2023-07-14 13:13:21.000000 efel-4.3.6/efel/cppcore/LibV1.h
+-rw-r--r--   0 runner    (1001) docker     (122)    57446 2023-07-14 13:13:21.000000 efel-4.3.6/efel/cppcore/LibV2.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8364 2023-07-14 13:13:21.000000 efel-4.3.6/efel/cppcore/LibV2.h
+-rw-r--r--   0 runner    (1001) docker     (122)    40008 2023-07-14 13:13:21.000000 efel-4.3.6/efel/cppcore/LibV3.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4874 2023-07-14 13:13:21.000000 efel-4.3.6/efel/cppcore/LibV3.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3611 2023-07-14 13:13:21.000000 efel-4.3.6/efel/cppcore/LibV4.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1596 2023-07-14 13:13:21.000000 efel-4.3.6/efel/cppcore/LibV4.h
+-rw-r--r--   0 runner    (1001) docker     (122)   137333 2023-07-14 13:13:21.000000 efel-4.3.6/efel/cppcore/LibV5.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    15913 2023-07-14 13:13:21.000000 efel-4.3.6/efel/cppcore/LibV5.h
+-rw-r--r--   0 runner    (1001) docker     (122)     6931 2023-07-14 13:13:21.000000 efel-4.3.6/efel/cppcore/Utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3430 2023-07-14 13:13:21.000000 efel-4.3.6/efel/cppcore/Utils.h
+-rw-r--r--   0 runner    (1001) docker     (122)    22270 2023-07-14 13:13:21.000000 efel-4.3.6/efel/cppcore/cfeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3274 2023-07-14 13:13:21.000000 efel-4.3.6/efel/cppcore/cfeature.h
+-rw-r--r--   0 runner    (1001) docker     (122)    10351 2023-07-14 13:13:21.000000 efel-4.3.6/efel/cppcore/cppcore.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1829 2023-07-14 13:13:21.000000 efel-4.3.6/efel/cppcore/eFELLogger.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3597 2023-07-14 13:13:21.000000 efel-4.3.6/efel/cppcore/efel.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2399 2023-07-14 13:13:21.000000 efel-4.3.6/efel/cppcore/efel.h
+-rw-r--r--   0 runner    (1001) docker     (122)     8378 2023-07-14 13:13:21.000000 efel-4.3.6/efel/cppcore/mapoperations.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2832 2023-07-14 13:13:21.000000 efel-4.3.6/efel/cppcore/mapoperations.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-07-14 13:13:21.000000 efel-4.3.6/efel/cppcore/types.h
+-rw-r--r--   0 runner    (1001) docker     (122)    10312 2023-07-14 13:13:21.000000 efel-4.3.6/efel/io.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:23.115804 efel-4.3.6/efel/pyfeatures/
+-rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-07-14 13:13:21.000000 efel-4.3.6/efel/pyfeatures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10309 2023-07-14 13:13:21.000000 efel-4.3.6/efel/pyfeatures/pyfeatures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-07-14 13:13:21.000000 efel-4.3.6/efel/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:23.119804 efel-4.3.6/efel/units/
+-rw-r--r--   0 runner    (1001) docker     (122)      266 2023-07-14 13:13:22.000000 efel-4.3.6/efel/units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4677 2023-07-14 13:13:22.000000 efel-4.3.6/efel/units/units.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 13:13:23.115804 efel-4.3.6/efel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-07-14 13:13:23.000000 efel-4.3.6/efel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-07-14 13:13:23.000000 efel-4.3.6/efel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-14 13:13:23.000000 efel-4.3.6/efel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-07-14 13:13:23.000000 efel-4.3.6/efel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-14 13:13:23.000000 efel-4.3.6/efel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-07-14 13:13:23.119804 efel-4.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4090 2023-07-14 13:13:22.000000 efel-4.3.6/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)    69513 2023-07-14 13:13:22.000000 efel-4.3.6/versioneer.py
```

### Comparing `efel-4.3.5/COPYING` & `efel-4.3.6/COPYING`

 * *Files identical despite different names*

### Comparing `efel-4.3.5/COPYING.less` & `efel-4.3.6/COPYING.less`

 * *Files identical despite different names*

### Comparing `efel-4.3.5/LICENSE.txt` & `efel-4.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `efel-4.3.5/PKG-INFO` & `efel-4.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efel
-Version: 4.3.5
+Version: 4.3.6
 Summary: Electrophys Feature Extract Library (eFEL)
 Home-page: https://github.com/BlueBrain/eFEL
 Author: BlueBrain Project, EPFL
 Maintainer: Werner Van Geit
 Maintainer-email: werner.vangeit@epfl.ch
 License: LGPLv3
 Keywords: feature,extraction,electrophysiology,BlueBrainProject
```

### Comparing `efel-4.3.5/README.md` & `efel-4.3.6/README.md`

 * *Files identical despite different names*

### Comparing `efel-4.3.5/efel/DependencyV5.txt` & `efel-4.3.6/efel/DependencyV5.txt`

 * *Files identical despite different names*

### Comparing `efel-4.3.5/efel/__init__.py` & `efel-4.3.6/efel/__init__.py`

 * *Files identical despite different names*

### Comparing `efel-4.3.5/efel/api.py` & `efel-4.3.6/efel/api.py`

 * *Files identical despite different names*

### Comparing `efel-4.3.5/efel/cppcore/DependencyTree.cpp` & `efel-4.3.6/efel/cppcore/DependencyTree.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.3.5/efel/cppcore/DependencyTree.h` & `efel-4.3.6/efel/cppcore/DependencyTree.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.5/efel/cppcore/FillFptrTable.cpp` & `efel-4.3.6/efel/cppcore/FillFptrTable.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.3.5/efel/cppcore/FillFptrTable.h` & `efel-4.3.6/efel/cppcore/FillFptrTable.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.5/efel/cppcore/Global.h` & `efel-4.3.6/efel/cppcore/Global.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.5/efel/cppcore/LibV1.cpp` & `efel-4.3.6/efel/cppcore/LibV1.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.3.5/efel/cppcore/LibV1.h` & `efel-4.3.6/efel/cppcore/LibV1.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.5/efel/cppcore/LibV2.cpp` & `efel-4.3.6/efel/cppcore/LibV2.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.3.5/efel/cppcore/LibV2.h` & `efel-4.3.6/efel/cppcore/LibV2.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.5/efel/cppcore/LibV3.cpp` & `efel-4.3.6/efel/cppcore/LibV3.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.3.5/efel/cppcore/LibV3.h` & `efel-4.3.6/efel/cppcore/LibV3.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.5/efel/cppcore/LibV4.cpp` & `efel-4.3.6/efel/cppcore/LibV4.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.3.5/efel/cppcore/LibV4.h` & `efel-4.3.6/efel/cppcore/LibV4.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.5/efel/cppcore/LibV5.cpp` & `efel-4.3.6/efel/cppcore/LibV5.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -779,28 +779,32 @@
 static int __AP_end_indices(const vector<double>& t, const vector<double>& v,
                             const vector<int>& pi, vector<int>& apei,
                             double derivativethreshold) {
 
   vector<double> dvdt(v.size());
   vector<double> dv;
   vector<double> dt;
+  int max_slope;
   getCentralDifferenceDerivative(1., v, dv);
   getCentralDifferenceDerivative(1., t, dt);
   transform(dv.begin(), dv.end(), dt.begin(), dvdt.begin(),
             std::divides<double>());
 
   apei.resize(pi.size());
   vector<int> picopy(pi.begin(), pi.end());
   picopy.push_back(v.size() - 1);
 
   for (size_t i = 0; i < apei.size(); i++) {
+    max_slope = std::distance(
+        dvdt.begin(),
+        std::min_element(dvdt.begin() + picopy[i] + 1, dvdt.begin() + picopy[i + 1]));
     // assure that the width of the slope is bigger than 4
     apei[i] = std::distance(
         dvdt.begin(),
-        std::find_if(dvdt.begin() + picopy[i] + 1, dvdt.begin() + picopy[i + 1],
+        std::find_if(dvdt.begin() + max_slope, dvdt.begin() + picopy[i + 1],
                 std::bind2nd(std::greater_equal<double>(), derivativethreshold)));
   }
   return apei.size();
 }
 
 
 int LibV5::AP_end_indices(mapStr2intVec& IntFeatureData,
```

### Comparing `efel-4.3.5/efel/cppcore/LibV5.h` & `efel-4.3.6/efel/cppcore/LibV5.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.5/efel/cppcore/Utils.cpp` & `efel-4.3.6/efel/cppcore/Utils.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.3.5/efel/cppcore/Utils.h` & `efel-4.3.6/efel/cppcore/Utils.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.5/efel/cppcore/cfeature.cpp` & `efel-4.3.6/efel/cppcore/cfeature.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.3.5/efel/cppcore/cfeature.h` & `efel-4.3.6/efel/cppcore/cfeature.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.5/efel/cppcore/cppcore.cpp` & `efel-4.3.6/efel/cppcore/cppcore.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.3.5/efel/cppcore/eFELLogger.h` & `efel-4.3.6/efel/cppcore/eFELLogger.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.5/efel/cppcore/efel.cpp` & `efel-4.3.6/efel/cppcore/efel.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.3.5/efel/cppcore/efel.h` & `efel-4.3.6/efel/cppcore/efel.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.5/efel/cppcore/mapoperations.cpp` & `efel-4.3.6/efel/cppcore/mapoperations.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.3.5/efel/cppcore/mapoperations.h` & `efel-4.3.6/efel/cppcore/mapoperations.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.5/efel/cppcore/types.h` & `efel-4.3.6/efel/cppcore/types.h`

 * *Files identical despite different names*

### Comparing `efel-4.3.5/efel/io.py` & `efel-4.3.6/efel/io.py`

 * *Files identical despite different names*

### Comparing `efel-4.3.5/efel/pyfeatures/__init__.py` & `efel-4.3.6/efel/pyfeatures/__init__.py`

 * *Files identical despite different names*

### Comparing `efel-4.3.5/efel/pyfeatures/pyfeatures.py` & `efel-4.3.6/efel/pyfeatures/pyfeatures.py`

 * *Files identical despite different names*

### Comparing `efel-4.3.5/efel/settings.py` & `efel-4.3.6/efel/settings.py`

 * *Files identical despite different names*

### Comparing `efel-4.3.5/efel/units/units.json` & `efel-4.3.6/efel/units/units.json`

 * *Files identical despite different names*

### Comparing `efel-4.3.5/efel.egg-info/PKG-INFO` & `efel-4.3.6/efel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efel
-Version: 4.3.5
+Version: 4.3.6
 Summary: Electrophys Feature Extract Library (eFEL)
 Home-page: https://github.com/BlueBrain/eFEL
 Author: BlueBrain Project, EPFL
 Maintainer: Werner Van Geit
 Maintainer-email: werner.vangeit@epfl.ch
 License: LGPLv3
 Keywords: feature,extraction,electrophysiology,BlueBrainProject
```

### Comparing `efel-4.3.5/efel.egg-info/SOURCES.txt` & `efel-4.3.6/efel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `efel-4.3.5/setup.py` & `efel-4.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `efel-4.3.5/versioneer.py` & `efel-4.3.6/versioneer.py`

 * *Files identical despite different names*

