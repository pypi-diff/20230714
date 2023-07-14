# Comparing `tmp/tentacletk-0.6.9.tar.gz` & `tmp/tentacletk-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tentacletk-0.6.9.tar", last modified: Mon Jul 10 18:21:57 2023, max compression
+gzip compressed data, was "tentacletk-0.7.0.tar", last modified: Fri Jul 14 17:50:00 2023, max compression
```

## Comparing `tentacletk-0.6.9.tar` & `tentacletk-0.7.0.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 18:21:57.464597 tentacletk-0.6.9/
--rw-rw-rw-   0        0        0     7815 2023-06-22 17:46:01.000000 tentacletk-0.6.9/COPYING.LESSER
--rw-rw-rw-   0        0        0       24 2023-03-28 23:37:53.000000 tentacletk-0.6.9/MANIFEST.in
--rw-rw-rw-   0        0        0     2951 2023-07-10 18:21:57.464597 tentacletk-0.6.9/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-10 18:21:57.465599 tentacletk-0.6.9/setup.cfg
--rw-rw-rw-   0        0        0     1447 2023-07-10 18:21:48.000000 tentacletk-0.6.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 18:21:57.408599 tentacletk-0.6.9/tentacle/
--rw-rw-rw-   0        0        0     1581 2023-07-10 18:21:54.000000 tentacletk-0.6.9/tentacle/__init__.py
--rw-rw-rw-   0        0        0    14113 2023-07-02 22:35:29.000000 tentacletk-0.6.9/tentacle/overlay.py
-drwxrwxrwx   0        0        0        0 2023-07-10 18:21:57.409597 tentacletk-0.6.9/tentacle/slots/
--rw-rw-rw-   0        0        0     1535 2023-07-02 22:34:48.000000 tentacletk-0.6.9/tentacle/slots/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 18:21:57.442597 tentacletk-0.6.9/tentacle/slots/maya/
--rw-rw-rw-   0        0        0      758 2023-06-22 17:46:01.000000 tentacletk-0.6.9/tentacle/slots/maya/__init__.py
--rw-rw-rw-   0        0        0     4877 2023-07-01 23:43:08.000000 tentacletk-0.6.9/tentacle/slots/maya/animation_maya.py
--rw-rw-rw-   0        0        0    13291 2023-07-07 13:31:21.000000 tentacletk-0.6.9/tentacle/slots/maya/cameras_maya.py
--rw-rw-rw-   0        0        0     4554 2023-07-07 14:07:28.000000 tentacletk-0.6.9/tentacle/slots/maya/convert_maya.py
--rw-rw-rw-   0        0        0    10767 2023-07-01 23:43:08.000000 tentacletk-0.6.9/tentacle/slots/maya/crease_maya.py
--rw-rw-rw-   0        0        0    13166 2023-07-07 14:11:56.000000 tentacletk-0.6.9/tentacle/slots/maya/create_maya.py
--rw-rw-rw-   0        0        0      534 2023-06-22 17:46:01.000000 tentacletk-0.6.9/tentacle/slots/maya/deformation_maya.py
--rw-rw-rw-   0        0        0     4939 2023-06-22 17:46:01.000000 tentacletk-0.6.9/tentacle/slots/maya/display_maya.py
--rw-rw-rw-   0        0        0    25512 2023-07-07 13:33:24.000000 tentacletk-0.6.9/tentacle/slots/maya/duplicate_maya.py
--rw-rw-rw-   0        0        0    18624 2023-07-07 17:35:30.000000 tentacletk-0.6.9/tentacle/slots/maya/edit_maya.py
--rw-rw-rw-   0        0        0    12380 2023-06-22 17:46:01.000000 tentacletk-0.6.9/tentacle/slots/maya/editors_maya.py
--rw-rw-rw-   0        0        0    12553 2023-07-07 14:05:51.000000 tentacletk-0.6.9/tentacle/slots/maya/file_maya.py
--rw-rw-rw-   0        0        0     6919 2023-06-22 17:46:01.000000 tentacletk-0.6.9/tentacle/slots/maya/init_maya.py
--rw-rw-rw-   0        0        0      629 2023-06-22 17:46:01.000000 tentacletk-0.6.9/tentacle/slots/maya/lighting_maya.py
--rw-rw-rw-   0        0        0     3265 2023-06-23 21:19:10.000000 tentacletk-0.6.9/tentacle/slots/maya/main_maya.py
--rw-rw-rw-   0        0        0    10735 2023-07-10 16:59:48.000000 tentacletk-0.6.9/tentacle/slots/maya/materials_maya.py
--rw-rw-rw-   0        0        0    12955 2023-07-01 23:43:08.000000 tentacletk-0.6.9/tentacle/slots/maya/mirror_maya.py
--rw-rw-rw-   0        0        0     9340 2023-07-01 23:43:08.000000 tentacletk-0.6.9/tentacle/slots/maya/normals_maya.py
--rw-rw-rw-   0        0        0    30767 2023-07-07 14:11:04.000000 tentacletk-0.6.9/tentacle/slots/maya/nurbs_maya.py
--rw-rw-rw-   0        0        0     3918 2023-07-01 23:43:08.000000 tentacletk-0.6.9/tentacle/slots/maya/pivot_maya.py
--rw-rw-rw-   0        0        0    23332 2023-07-03 03:10:09.000000 tentacletk-0.6.9/tentacle/slots/maya/polygons_maya.py
--rw-rw-rw-   0        0        0     3153 2023-07-07 13:31:33.000000 tentacletk-0.6.9/tentacle/slots/maya/preferences_maya.py
--rw-rw-rw-   0        0        0     3415 2023-06-22 17:46:01.000000 tentacletk-0.6.9/tentacle/slots/maya/rendering_maya.py
--rw-rw-rw-   0        0        0    23526 2023-07-07 17:35:30.000000 tentacletk-0.6.9/tentacle/slots/maya/rigging_maya.py
--rw-rw-rw-   0        0        0     4076 2023-07-01 23:43:08.000000 tentacletk-0.6.9/tentacle/slots/maya/scene_maya.py
--rw-rw-rw-   0        0        0    27172 2023-07-07 19:04:50.000000 tentacletk-0.6.9/tentacle/slots/maya/selection_maya.py
--rw-rw-rw-   0        0        0     5853 2023-06-23 21:19:10.000000 tentacletk-0.6.9/tentacle/slots/maya/subdivision_maya.py
--rw-rw-rw-   0        0        0     2927 2023-06-22 17:46:01.000000 tentacletk-0.6.9/tentacle/slots/maya/symmetry_maya.py
--rw-rw-rw-   0        0        0    25170 2023-07-07 14:13:18.000000 tentacletk-0.6.9/tentacle/slots/maya/transform_maya.py
--rw-rw-rw-   0        0        0      957 2023-06-22 17:46:01.000000 tentacletk-0.6.9/tentacle/slots/maya/utilities_maya.py
--rw-rw-rw-   0        0        0    22998 2023-07-07 14:11:36.000000 tentacletk-0.6.9/tentacle/slots/maya/uv_maya.py
--rw-rw-rw-   0        0        0      624 2023-06-22 17:46:01.000000 tentacletk-0.6.9/tentacle/slots/maya/vfx_maya.py
--rw-rw-rw-   0        0        0    21461 2023-07-03 14:35:57.000000 tentacletk-0.6.9/tentacle/tcl.py
--rw-rw-rw-   0        0        0    25342 2023-06-06 00:33:56.000000 tentacletk-0.6.9/tentacle/tcl.py.bak
--rw-rw-rw-   0        0        0     3561 2023-07-02 22:31:43.000000 tentacletk-0.6.9/tentacle/tcl_blender.py
--rw-rw-rw-   0        0        0     4885 2023-07-02 22:30:32.000000 tentacletk-0.6.9/tentacle/tcl_max.py
--rw-rw-rw-   0        0        0     2930 2023-07-02 22:33:24.000000 tentacletk-0.6.9/tentacle/tcl_maya.py
-drwxrwxrwx   0        0        0        0 2023-07-10 18:21:57.443596 tentacletk-0.6.9/tentacle/ui/
--rw-rw-rw-   0        0        0      511 2023-07-02 22:34:35.000000 tentacletk-0.6.9/tentacle/ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 18:21:57.462597 tentacletk-0.6.9/tentacletk.egg-info/
--rw-rw-rw-   0        0        0     2951 2023-07-10 18:21:57.000000 tentacletk-0.6.9/tentacletk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1511 2023-07-10 18:21:57.000000 tentacletk-0.6.9/tentacletk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 18:21:57.000000 tentacletk-0.6.9/tentacletk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-10 18:21:57.000000 tentacletk-0.6.9/tentacletk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 17:50:00.076485 tentacletk-0.7.0/
+-rw-rw-rw-   0        0        0     7815 2023-06-22 17:46:01.000000 tentacletk-0.7.0/COPYING.LESSER
+-rw-rw-rw-   0        0        0       24 2023-03-28 23:37:53.000000 tentacletk-0.7.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3023 2023-07-14 17:50:00.076485 tentacletk-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-14 17:50:00.077483 tentacletk-0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     1447 2023-07-10 18:21:48.000000 tentacletk-0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 17:49:59.818767 tentacletk-0.7.0/tentacle/
+-rw-rw-rw-   0        0        0     1581 2023-07-14 17:49:56.000000 tentacletk-0.7.0/tentacle/__init__.py
+-rw-rw-rw-   0        0        0    14113 2023-07-02 22:35:29.000000 tentacletk-0.7.0/tentacle/overlay.py
+drwxrwxrwx   0        0        0        0 2023-07-14 17:49:59.825766 tentacletk-0.7.0/tentacle/slots/
+-rw-rw-rw-   0        0        0     1535 2023-07-02 22:34:48.000000 tentacletk-0.7.0/tentacle/slots/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 17:50:00.041744 tentacletk-0.7.0/tentacle/slots/maya/
+-rw-rw-rw-   0        0        0      758 2023-06-22 17:46:01.000000 tentacletk-0.7.0/tentacle/slots/maya/__init__.py
+-rw-rw-rw-   0        0        0     4877 2023-07-01 23:43:08.000000 tentacletk-0.7.0/tentacle/slots/maya/animation_maya.py
+-rw-rw-rw-   0        0        0    13291 2023-07-07 13:31:21.000000 tentacletk-0.7.0/tentacle/slots/maya/cameras_maya.py
+-rw-rw-rw-   0        0        0     4554 2023-07-07 14:07:28.000000 tentacletk-0.7.0/tentacle/slots/maya/convert_maya.py
+-rw-rw-rw-   0        0        0    10767 2023-07-01 23:43:08.000000 tentacletk-0.7.0/tentacle/slots/maya/crease_maya.py
+-rw-rw-rw-   0        0        0    13166 2023-07-07 14:11:56.000000 tentacletk-0.7.0/tentacle/slots/maya/create_maya.py
+-rw-rw-rw-   0        0        0      534 2023-06-22 17:46:01.000000 tentacletk-0.7.0/tentacle/slots/maya/deformation_maya.py
+-rw-rw-rw-   0        0        0     4939 2023-06-22 17:46:01.000000 tentacletk-0.7.0/tentacle/slots/maya/display_maya.py
+-rw-rw-rw-   0        0        0    25512 2023-07-07 13:33:24.000000 tentacletk-0.7.0/tentacle/slots/maya/duplicate_maya.py
+-rw-rw-rw-   0        0        0    18624 2023-07-07 17:35:30.000000 tentacletk-0.7.0/tentacle/slots/maya/edit_maya.py
+-rw-rw-rw-   0        0        0    12380 2023-06-22 17:46:01.000000 tentacletk-0.7.0/tentacle/slots/maya/editors_maya.py
+-rw-rw-rw-   0        0        0    12553 2023-07-07 14:05:51.000000 tentacletk-0.7.0/tentacle/slots/maya/file_maya.py
+-rw-rw-rw-   0        0        0     6919 2023-06-22 17:46:01.000000 tentacletk-0.7.0/tentacle/slots/maya/init_maya.py
+-rw-rw-rw-   0        0        0      629 2023-06-22 17:46:01.000000 tentacletk-0.7.0/tentacle/slots/maya/lighting_maya.py
+-rw-rw-rw-   0        0        0     3265 2023-06-23 21:19:10.000000 tentacletk-0.7.0/tentacle/slots/maya/main_maya.py
+-rw-rw-rw-   0        0        0    10771 2023-07-11 17:16:25.000000 tentacletk-0.7.0/tentacle/slots/maya/materials_maya.py
+-rw-rw-rw-   0        0        0    12955 2023-07-01 23:43:08.000000 tentacletk-0.7.0/tentacle/slots/maya/mirror_maya.py
+-rw-rw-rw-   0        0        0     9340 2023-07-01 23:43:08.000000 tentacletk-0.7.0/tentacle/slots/maya/normals_maya.py
+-rw-rw-rw-   0        0        0    30767 2023-07-07 14:11:04.000000 tentacletk-0.7.0/tentacle/slots/maya/nurbs_maya.py
+-rw-rw-rw-   0        0        0     3918 2023-07-01 23:43:08.000000 tentacletk-0.7.0/tentacle/slots/maya/pivot_maya.py
+-rw-rw-rw-   0        0        0    23332 2023-07-03 03:10:09.000000 tentacletk-0.7.0/tentacle/slots/maya/polygons_maya.py
+-rw-rw-rw-   0        0        0     3153 2023-07-07 13:31:33.000000 tentacletk-0.7.0/tentacle/slots/maya/preferences_maya.py
+-rw-rw-rw-   0        0        0     3415 2023-06-22 17:46:01.000000 tentacletk-0.7.0/tentacle/slots/maya/rendering_maya.py
+-rw-rw-rw-   0        0        0    23526 2023-07-07 17:35:30.000000 tentacletk-0.7.0/tentacle/slots/maya/rigging_maya.py
+-rw-rw-rw-   0        0        0     4076 2023-07-01 23:43:08.000000 tentacletk-0.7.0/tentacle/slots/maya/scene_maya.py
+-rw-rw-rw-   0        0        0    27172 2023-07-07 19:04:50.000000 tentacletk-0.7.0/tentacle/slots/maya/selection_maya.py
+-rw-rw-rw-   0        0        0     5853 2023-06-23 21:19:10.000000 tentacletk-0.7.0/tentacle/slots/maya/subdivision_maya.py
+-rw-rw-rw-   0        0        0     2927 2023-06-22 17:46:01.000000 tentacletk-0.7.0/tentacle/slots/maya/symmetry_maya.py
+-rw-rw-rw-   0        0        0    25170 2023-07-07 14:13:18.000000 tentacletk-0.7.0/tentacle/slots/maya/transform_maya.py
+-rw-rw-rw-   0        0        0      957 2023-06-22 17:46:01.000000 tentacletk-0.7.0/tentacle/slots/maya/utilities_maya.py
+-rw-rw-rw-   0        0        0    22998 2023-07-07 14:11:36.000000 tentacletk-0.7.0/tentacle/slots/maya/uv_maya.py
+-rw-rw-rw-   0        0        0      624 2023-06-22 17:46:01.000000 tentacletk-0.7.0/tentacle/slots/maya/vfx_maya.py
+-rw-rw-rw-   0        0        0    21461 2023-07-11 19:33:29.000000 tentacletk-0.7.0/tentacle/tcl.py
+-rw-rw-rw-   0        0        0     3492 2023-07-11 19:38:49.000000 tentacletk-0.7.0/tentacle/tcl_blender.py
+-rw-rw-rw-   0        0        0     4875 2023-07-11 19:38:16.000000 tentacletk-0.7.0/tentacle/tcl_max.py
+-rw-rw-rw-   0        0        0     2790 2023-07-11 19:38:01.000000 tentacletk-0.7.0/tentacle/tcl_maya.py
+drwxrwxrwx   0        0        0        0 2023-07-14 17:50:00.045732 tentacletk-0.7.0/tentacle/ui/
+-rw-rw-rw-   0        0        0      511 2023-07-02 22:34:35.000000 tentacletk-0.7.0/tentacle/ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 17:50:00.075482 tentacletk-0.7.0/tentacletk.egg-info/
+-rw-rw-rw-   0        0        0     3023 2023-07-14 17:49:59.000000 tentacletk-0.7.0/tentacletk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2951 2023-07-10 18:21:57.000000 tentacletk-0.7.0/tentacletk.egg-info/PKG-INFO.bak
+-rw-rw-rw-   0        0        0     1560 2023-07-14 17:49:59.000000 tentacletk-0.7.0/tentacletk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0     1511 2023-07-10 18:21:57.000000 tentacletk-0.7.0/tentacletk.egg-info/SOURCES.txt.bak
+-rw-rw-rw-   0        0        0        1 2023-07-14 17:49:59.000000 tentacletk-0.7.0/tentacletk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-14 17:49:59.000000 tentacletk-0.7.0/tentacletk.egg-info/top_level.txt
```

### Comparing `tentacletk-0.6.9/COPYING.LESSER` & `tentacletk-0.7.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `tentacletk-0.6.9/PKG-INFO` & `tentacletk-0.7.0/tentacletk.egg-info/PKG-INFO.bak`

 * *Files identical despite different names*

### Comparing `tentacletk-0.6.9/setup.py` & `tentacletk-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.6.9/tentacle/__init__.py` & `tentacletk-0.7.0/tentacle/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # !/usr/bin/python
 # coding=utf-8
 import sys
 
 __package__ = "tentacle"
-__version__ = '0.6.9'
+__version__ = "0.7.0"
 
 
 def greeting(string, outputToConsole=True):
     """Format a string using preset variables.
 
     Parameters:
             string (str): The greeting to format as a string with placeholders using the below keywords.
```

### Comparing `tentacletk-0.6.9/tentacle/overlay.py` & `tentacletk-0.7.0/tentacle/overlay.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.6.9/tentacle/slots/__init__.py` & `tentacletk-0.7.0/tentacle/slots/__init__.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.6.9/tentacle/slots/maya/__init__.py` & `tentacletk-0.7.0/tentacle/slots/maya/__init__.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.6.9/tentacle/slots/maya/animation_maya.py` & `tentacletk-0.7.0/tentacle/slots/maya/animation_maya.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.6.9/tentacle/slots/maya/cameras_maya.py` & `tentacletk-0.7.0/tentacle/slots/maya/cameras_maya.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.6.9/tentacle/slots/maya/convert_maya.py` & `tentacletk-0.7.0/tentacle/slots/maya/convert_maya.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.6.9/tentacle/slots/maya/crease_maya.py` & `tentacletk-0.7.0/tentacle/slots/maya/crease_maya.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.6.9/tentacle/slots/maya/create_maya.py` & `tentacletk-0.7.0/tentacle/slots/maya/create_maya.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.6.9/tentacle/slots/maya/deformation_maya.py` & `tentacletk-0.7.0/tentacle/slots/maya/deformation_maya.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.6.9/tentacle/slots/maya/display_maya.py` & `tentacletk-0.7.0/tentacle/slots/maya/display_maya.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.6.9/tentacle/slots/maya/duplicate_maya.py` & `tentacletk-0.7.0/tentacle/slots/maya/duplicate_maya.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.6.9/tentacle/slots/maya/edit_maya.py` & `tentacletk-0.7.0/tentacle/slots/maya/edit_maya.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.6.9/tentacle/slots/maya/editors_maya.py` & `tentacletk-0.7.0/tentacle/slots/maya/editors_maya.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.6.9/tentacle/slots/maya/file_maya.py` & `tentacletk-0.7.0/tentacle/slots/maya/file_maya.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.6.9/tentacle/slots/maya/init_maya.py` & `tentacletk-0.7.0/tentacle/slots/maya/init_maya.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.6.9/tentacle/slots/maya/lighting_maya.py` & `tentacletk-0.7.0/tentacle/slots/maya/lighting_maya.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.6.9/tentacle/slots/maya/main_maya.py` & `tentacletk-0.7.0/tentacle/slots/maya/main_maya.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.6.9/tentacle/slots/maya/materials_maya.py` & `tentacletk-0.7.0/tentacle/slots/maya/materials_maya.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
         self.random_mat = None
 
     def cmb002_init(self, widget):
         """ """
         widget.refresh = True
         if not widget.is_initialized:
+            widget.editable = True
             widget.menu.add(
                 "QComboBox",
                 setObjectName="cmb001",
                 addItems=["Scene Materials", "ID Map Materials", "Favorite Materials"],
                 setToolTip="Filter materials list based on type.",
             )
             widget.menu.add(
```

### Comparing `tentacletk-0.6.9/tentacle/slots/maya/mirror_maya.py` & `tentacletk-0.7.0/tentacle/slots/maya/mirror_maya.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.6.9/tentacle/slots/maya/normals_maya.py` & `tentacletk-0.7.0/tentacle/slots/maya/normals_maya.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.6.9/tentacle/slots/maya/nurbs_maya.py` & `tentacletk-0.7.0/tentacle/slots/maya/nurbs_maya.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.6.9/tentacle/slots/maya/pivot_maya.py` & `tentacletk-0.7.0/tentacle/slots/maya/pivot_maya.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.6.9/tentacle/slots/maya/polygons_maya.py` & `tentacletk-0.7.0/tentacle/slots/maya/polygons_maya.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.6.9/tentacle/slots/maya/preferences_maya.py` & `tentacletk-0.7.0/tentacle/slots/maya/preferences_maya.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.6.9/tentacle/slots/maya/rendering_maya.py` & `tentacletk-0.7.0/tentacle/slots/maya/rendering_maya.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.6.9/tentacle/slots/maya/rigging_maya.py` & `tentacletk-0.7.0/tentacle/slots/maya/rigging_maya.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.6.9/tentacle/slots/maya/scene_maya.py` & `tentacletk-0.7.0/tentacle/slots/maya/scene_maya.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.6.9/tentacle/slots/maya/selection_maya.py` & `tentacletk-0.7.0/tentacle/slots/maya/selection_maya.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.6.9/tentacle/slots/maya/subdivision_maya.py` & `tentacletk-0.7.0/tentacle/slots/maya/subdivision_maya.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.6.9/tentacle/slots/maya/symmetry_maya.py` & `tentacletk-0.7.0/tentacle/slots/maya/symmetry_maya.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.6.9/tentacle/slots/maya/transform_maya.py` & `tentacletk-0.7.0/tentacle/slots/maya/transform_maya.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.6.9/tentacle/slots/maya/utilities_maya.py` & `tentacletk-0.7.0/tentacle/slots/maya/utilities_maya.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.6.9/tentacle/slots/maya/uv_maya.py` & `tentacletk-0.7.0/tentacle/slots/maya/uv_maya.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.6.9/tentacle/slots/maya/vfx_maya.py` & `tentacletk-0.7.0/tentacle/slots/maya/vfx_maya.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.6.9/tentacle/tcl.py` & `tentacletk-0.7.0/tentacle/tcl.py`

 * *Files identical despite different names*

### Comparing `tentacletk-0.6.9/tentacle/tcl_blender.py` & `tentacletk-0.7.0/tentacle/tcl_blender.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # !/usr/bin/python
 # coding=utf-8
 import sys
 from PySide2 import QtWidgets, QtCore
 from tentacle.tcl import Tcl
 
 
-# constants
 INSTANCES = {}
 
 
 class TclBlender(Tcl):
     """Tcl class overridden for use with Blender.
 
     Parameters:
@@ -47,29 +46,29 @@
             modifiers = QtWidgets.QApplication.instance().keyboardModifiers()
 
             if event.key() == self.key_undo and modifiers == QtCore.Qt.ControlModifier:
                 import bpy
 
                 bpy.ops.ed.undo()
 
-        Tcl.keyPressEvent(self, event)
+        super().keyPressEvent(event)
 
     def showEvent(self, event):
         """
         Parameters:
                 event = <QEvent>
         """
-        Tcl.showEvent(self, event)  # super().showEvent(event)
+        super().showEvent(event)  # super().showEvent(event)
 
     def hideEvent(self, event):
         """
         Parameters:
                 event = <QEvent>
         """
-        Tcl.hideEvent(self, event)  # super().hideEvent(event)
+        super().hideEvent(event)  # super().hideEvent(event)
 
 
 # --------------------------------------------------------------------------------------------
 
 
 def getInstance(instanceID=None, *args, **kwargs):
     """Get an instance of this class using a given instanceID.
@@ -78,15 +77,15 @@
     Parameters:
             instanceID () = The instanceID can be any immutable type.
             args/kwargs () = The args to be passed to the class instance when it is created.
 
     Returns:
             (obj) An instance of this class.
 
-    Example: tcl = getInstance(id(0), key_show='Key_F12') #returns the class instance with an instance ID of the value of `id(0)`.
+    Example: tentacle = getInstance(id(0), key_show='Key_F12') #returns the class instance with an instance ID of the value of `id(0)`.
     """
     import inspect
 
     if instanceID is None:
         instanceID = inspect.stack()[1][3]
     try:
         return INSTANCES[instanceID]
@@ -114,10 +113,7 @@
         sys.exit(exit_code)
 
 # module name
 print(__name__)
 # --------------------------------------------------------------------------------------------
 # Notes
 # --------------------------------------------------------------------------------------------
-
-
-# deprecated: -----------------------------------
```

### Comparing `tentacletk-0.6.9/tentacle/tcl_max.py` & `tentacletk-0.7.0/tentacle/tcl_max.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 try:
     from pymxs import runtime as rt
 except ImportError as error:
     print(error)
 from tentacle.tcl import Tcl
 
-# constants
+
 INSTANCES = {}
 
 
 class TclMax(Tcl):
     """Tcl class overridden for use with Autodesk 3ds max.
 
     Parameters:
@@ -64,28 +64,28 @@
         """
         try:
             rt.enableAccelerators = False
 
         except Exception as error:
             print(error)
 
-        Tcl.showEvent(self, event)  # super().showEvent(event)
+        super().showEvent(event)  # super().showEvent(event)
 
     def hideEvent(self, event):
         """
         Parameters:
                 event = <QEvent>
         """
         try:
             rt.enableAccelerators = True
 
         except Exception as error:
             print(error)
 
-        Tcl.hideEvent(self, event)  # super().hideEvent(event)
+        super().hideEvent(event)  # super().hideEvent(event)
 
 
 # --------------------------------------------------------------------------------------------
 
 
 def getInstance(instanceID=None, *args, **kwargs):
     """Get an instance of this class using a given instanceID.
@@ -94,15 +94,15 @@
     Parameters:
             instanceID () = The instanceID can be any immutable type.
             args/kwargs () = The args to be passed to the class instance when it is created.
 
     Returns:
             (obj) An instance of this class.
 
-    Example: tcl = getInstance(id(0), key_show='Key_F12') #returns the class instance with an instance ID of the value of `id(0)`.
+    Example: tentacle = getInstance(id(0), key_show='Key_F12') #returns the class instance with an instance ID of the value of `id(0)`.
     """
     import inspect
 
     if instanceID is None:
         instanceID = inspect.stack()[1][3]
     try:
         return INSTANCES[instanceID]
```

### Comparing `tentacletk-0.6.9/tentacle/tcl_maya.py` & `tentacletk-0.7.0/tentacle/tcl_maya.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # !/usr/bin/python
 # coding=utf-8
 import sys
 import mayatk as mtk
 from tentacle.tcl import Tcl
 
 
-# constants
 INSTANCES = {}
 
 
 class TclMaya(Tcl):
     """Tcl class overridden for use with Autodesk Maya.
 
     Parameters:
@@ -24,31 +23,25 @@
 
             except Exception as error:
                 print(__file__, error)
 
         super().__init__(parent, slots_location=slots_location, *args, **kwargs)
 
     def showEvent(self, event):
-        """
-        Parameters:
-                event = <QEvent>
-        """
+        """ """
 
-        Tcl.showEvent(self, event)  # super().showEvent(event)
+        super().showEvent(event)  # super().showEvent(event)
 
     def hideEvent(self, event):
-        """
-        Parameters:
-                event = <QEvent>
-        """
+        """ """
         if __name__ == "__main__":
             self.app.quit()
             sys.exit()  # assure that the sys processes are terminated.
 
-        Tcl.hideEvent(self, event)  # super().hideEvent(event)
+        super().hideEvent(event)  # super().hideEvent(event)
 
 
 # --------------------------------------------------------------------------------------------
 
 
 def getInstance(instanceID=None, *args, **kwargs):
     """Get an instance of this class using a given instanceID.
@@ -57,15 +50,15 @@
     Parameters:
             instanceID () = The instanceID can be any immutable type.
             args/kwargs () = The args to be passed to the class instance when it is created.
 
     Returns:
             (obj) An instance of this class.
 
-    Example: tcl = getInstance(id(0), key_show='Key_F12') #returns the class instance with an instance ID of the value of `id(0)`.
+    Example: tentacle = getInstance(id(0), key_show='Key_F12') #returns the class instance with an instance ID of the value of `id(0)`.
     """
     import inspect
 
     if instanceID is None:
         instanceID = inspect.stack()[1][3]
     try:
         return INSTANCES[instanceID]
```

### Comparing `tentacletk-0.6.9/tentacletk.egg-info/PKG-INFO` & `tentacletk-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: tentacletk
-Version: 0.6.9
+Version: 0.7.0
 Summary: A Python3/PySide2 marking menu style toolkit for Maya, 3ds Max, and Blender.
 Home-page: https://github.com/m3trik/tentacle
 Author: Ryan Simpson
 Author-email: m3trik@outlook.com
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: COPYING.LESSER
 
 [![License: LGPL v3](https://img.shields.io/badge/License-LGPL%20v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0.en.html)
+![Version](https://img.shields.io/badge/Version-0.7.0-brightgreen.svg)
 
 # Tentacle: A Python3/PySide2 Marking Menu and UI Toolkit
 
 Tentacle is a Python3/PySide2 marking menu and UI toolkit designed for Maya, 3ds Max, Blender, and any other DCC app that supports the PySide2 framework. It is a personal project and is currently a work in progress.
 
 ## Design
```

### Comparing `tentacletk-0.6.9/tentacletk.egg-info/SOURCES.txt` & `tentacletk-0.7.0/tentacletk.egg-info/SOURCES.txt.bak`

 * *Files identical despite different names*

