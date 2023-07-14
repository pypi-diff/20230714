# Comparing `tmp/mayatk-0.6.8.tar.gz` & `tmp/mayatk-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mayatk-0.6.8.tar", last modified: Mon Jul  3 15:10:24 2023, max compression
+gzip compressed data, was "mayatk-0.6.9.tar", last modified: Fri Jul 14 18:00:56 2023, max compression
```

## Comparing `mayatk-0.6.8.tar` & `mayatk-0.6.9.tar`

### file list

```diff
@@ -1,50 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 15:10:24.561608 mayatk-0.6.8/
--rw-rw-rw-   0        0        0     1093 2023-03-28 23:39:14.000000 mayatk-0.6.8/LICENSE
--rw-rw-rw-   0        0        0       27 2023-03-28 23:39:14.000000 mayatk-0.6.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1246 2023-07-03 15:10:24.560606 mayatk-0.6.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-03 15:10:24.520828 mayatk-0.6.8/mayatk/
--rw-rw-rw-   0        0        0     4335 2023-07-03 15:10:21.000000 mayatk-0.6.8/mayatk/__init__.py
--rw-rw-rw-   0        0        0     8065 2023-06-27 21:45:31.000000 mayatk-0.6.8/mayatk/cam_utils.py
--rw-rw-rw-   0        0        0     8083 2023-05-30 18:39:58.000000 mayatk-0.6.8/mayatk/cam_utils.py.bak
--rw-rw-rw-   0        0        0    64489 2023-06-29 16:12:36.000000 mayatk-0.6.8/mayatk/cmpt_utils.py
--rw-rw-rw-   0        0        0    48216 2023-05-30 18:39:58.000000 mayatk-0.6.8/mayatk/cmpt_utils.py.bak
-drwxrwxrwx   0        0        0        0 2023-07-03 15:10:24.546613 mayatk-0.6.8/mayatk/display_utils/
--rw-rw-rw-   0        0        0      397 2023-06-25 00:47:10.000000 mayatk-0.6.8/mayatk/display_utils/__init__.py
--rw-rw-rw-   0        0        0     7746 2023-06-27 21:52:32.000000 mayatk-0.6.8/mayatk/display_utils/exploded_view.py
--rw-rw-rw-   0        0        0    30701 2023-06-28 01:35:20.000000 mayatk-0.6.8/mayatk/edit_utils.py
--rw-rw-rw-   0        0        0    22313 2023-05-28 17:20:26.000000 mayatk-0.6.8/mayatk/macro_utils.py
--rw-rw-rw-   0        0        0    13411 2023-06-05 16:23:13.000000 mayatk-0.6.8/mayatk/mash_utils.py
--rw-rw-rw-   0        0        0    13413 2023-05-29 19:59:22.000000 mayatk-0.6.8/mayatk/mash_utils.py.bak
-drwxrwxrwx   0        0        0        0 2023-07-03 15:10:24.549613 mayatk-0.6.8/mayatk/mat_utils/
--rw-rw-rw-   0        0        0      337 2023-06-25 00:47:26.000000 mayatk-0.6.8/mayatk/mat_utils/__init__.py
--rw-rw-rw-   0        0        0     8911 2023-06-28 02:10:10.000000 mayatk-0.6.8/mayatk/mat_utils/mat_utils.py
--rw-rw-rw-   0        0        0    17681 2023-06-27 21:41:18.000000 mayatk-0.6.8/mayatk/mat_utils/stingray_arnold_shader.py
--rw-rw-rw-   0        0        0    15374 2023-06-17 12:29:07.000000 mayatk-0.6.8/mayatk/misc_utils.py.bak
--rw-rw-rw-   0        0        0    27018 2023-06-27 22:30:12.000000 mayatk-0.6.8/mayatk/node_utils.py
--rw-rw-rw-   0        0        0    13177 2023-06-28 22:54:55.000000 mayatk-0.6.8/mayatk/project_utils.py
--rw-rw-rw-   0        0        0    11613 2023-05-20 16:09:43.000000 mayatk-0.6.8/mayatk/project_utils.py.bak
--rw-rw-rw-   0        0        0    18251 2023-06-27 23:39:34.000000 mayatk-0.6.8/mayatk/rig_utils.py
--rw-rw-rw-   0        0        0    20342 2023-05-30 18:34:56.000000 mayatk-0.6.8/mayatk/rig_utils.py.bak
--rw-rw-rw-   0        0        0     2771 2023-05-20 16:34:41.000000 mayatk-0.6.8/mayatk/script_utils.py
--rw-rw-rw-   0        0        0    15184 2023-06-27 22:23:17.000000 mayatk-0.6.8/mayatk/utils.py
--rw-rw-rw-   0        0        0    31389 2023-06-27 23:49:44.000000 mayatk-0.6.8/mayatk/xform_utils.py
--rw-rw-rw-   0        0        0    32309 2023-06-05 16:23:13.000000 mayatk-0.6.8/mayatk/xform_utils.py.bak
-drwxrwxrwx   0        0        0        0 2023-07-03 15:10:24.545608 mayatk-0.6.8/mayatk.egg-info/
--rw-rw-rw-   0        0        0     1246 2023-07-03 15:10:24.000000 mayatk-0.6.8/mayatk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1157 2023-05-20 15:52:44.000000 mayatk-0.6.8/mayatk.egg-info/PKG-INFO.bak
--rw-rw-rw-   0        0        0     1006 2023-07-03 15:10:24.000000 mayatk-0.6.8/mayatk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      518 2023-03-29 13:02:37.000000 mayatk-0.6.8/mayatk.egg-info/SOURCES.txt.bak
--rw-rw-rw-   0        0        0        1 2023-07-03 15:10:24.000000 mayatk-0.6.8/mayatk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-03 15:10:24.000000 mayatk-0.6.8/mayatk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 15:10:24.561608 mayatk-0.6.8/setup.cfg
--rw-rw-rw-   0        0        0     1442 2023-06-28 02:16:01.000000 mayatk-0.6.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-03 15:10:24.560606 mayatk-0.6.8/test/
--rw-rw-rw-   0        0        0     1289 2023-05-20 14:01:35.000000 mayatk-0.6.8/test/__init__.py
--rw-rw-rw-   0        0        0    26026 2023-06-28 00:01:13.000000 mayatk-0.6.8/test/cmpt_utils_test.py
--rw-rw-rw-   0        0        0     7676 2023-06-28 00:35:52.000000 mayatk-0.6.8/test/edit_utils_test.py
--rw-rw-rw-   0        0        0     4505 2023-06-28 02:10:41.000000 mayatk-0.6.8/test/mat_utils_test.py
--rw-rw-rw-   0        0        0     7396 2023-06-28 00:17:04.000000 mayatk-0.6.8/test/node_utils_test.py
--rw-rw-rw-   0        0        0     5086 2023-06-28 01:40:55.000000 mayatk-0.6.8/test/rig_utils_test.py
--rw-rw-rw-   0        0        0     2068 2023-06-28 01:24:21.000000 mayatk-0.6.8/test/run_tests.py
--rw-rw-rw-   0        0        0     7022 2023-06-28 00:34:32.000000 mayatk-0.6.8/test/utils_test.py
--rw-rw-rw-   0        0        0     7298 2023-06-28 01:39:40.000000 mayatk-0.6.8/test/xform_utils_test.py
+drwxrwxrwx   0        0        0        0 2023-07-14 18:00:56.832372 mayatk-0.6.9/
+-rw-rw-rw-   0        0        0     1093 2023-03-28 23:39:14.000000 mayatk-0.6.9/LICENSE
+-rw-rw-rw-   0        0        0       27 2023-03-28 23:39:14.000000 mayatk-0.6.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2579 2023-07-14 18:00:56.830854 mayatk-0.6.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-14 18:00:56.694511 mayatk-0.6.9/mayatk/
+-rw-rw-rw-   0        0        0     4335 2023-07-14 18:00:53.000000 mayatk-0.6.9/mayatk/__init__.py
+-rw-rw-rw-   0        0        0     8115 2023-07-03 18:08:35.000000 mayatk-0.6.9/mayatk/cam_utils.py
+-rw-rw-rw-   0        0        0    64713 2023-07-03 18:11:33.000000 mayatk-0.6.9/mayatk/cmpt_utils.py
+-rw-rw-rw-   0        0        0    16201 2023-07-03 18:12:10.000000 mayatk-0.6.9/mayatk/core_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-14 18:00:56.747996 mayatk-0.6.9/mayatk/display_utils/
+-rw-rw-rw-   0        0        0      397 2023-06-25 00:47:10.000000 mayatk-0.6.9/mayatk/display_utils/__init__.py
+-rw-rw-rw-   0        0        0     7759 2023-07-03 18:09:10.000000 mayatk-0.6.9/mayatk/display_utils/exploded_view.py
+-rw-rw-rw-   0        0        0    30742 2023-07-03 18:09:50.000000 mayatk-0.6.9/mayatk/edit_utils.py
+-rw-rw-rw-   0        0        0    22313 2023-05-28 17:20:26.000000 mayatk-0.6.9/mayatk/macro_utils.py
+-rw-rw-rw-   0        0        0    13411 2023-06-05 16:23:13.000000 mayatk-0.6.9/mayatk/mash_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-14 18:00:56.762031 mayatk-0.6.9/mayatk/mat_utils/
+-rw-rw-rw-   0        0        0      337 2023-06-25 00:47:26.000000 mayatk-0.6.9/mayatk/mat_utils/__init__.py
+-rw-rw-rw-   0        0        0     8911 2023-06-28 02:10:10.000000 mayatk-0.6.9/mayatk/mat_utils/mat_utils.py
+-rw-rw-rw-   0        0        0    17668 2023-07-11 19:14:32.000000 mayatk-0.6.9/mayatk/mat_utils/stingray_arnold_shader.py
+-rw-rw-rw-   0        0        0    27050 2023-07-03 18:13:42.000000 mayatk-0.6.9/mayatk/node_utils.py
+-rw-rw-rw-   0        0        0    11296 2023-07-03 17:52:23.000000 mayatk-0.6.9/mayatk/proj_utils.py
+-rw-rw-rw-   0        0        0    18251 2023-06-27 23:39:34.000000 mayatk-0.6.9/mayatk/rig_utils.py
+-rw-rw-rw-   0        0        0    24543 2023-07-03 18:14:33.000000 mayatk-0.6.9/mayatk/xform_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-14 18:00:56.728559 mayatk-0.6.9/mayatk.egg-info/
+-rw-rw-rw-   0        0        0     2579 2023-07-14 18:00:56.000000 mayatk-0.6.9/mayatk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1157 2023-05-20 15:52:44.000000 mayatk-0.6.9/mayatk.egg-info/PKG-INFO.bak
+-rw-rw-rw-   0        0        0      813 2023-07-14 18:00:56.000000 mayatk-0.6.9/mayatk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      518 2023-03-29 13:02:37.000000 mayatk-0.6.9/mayatk.egg-info/SOURCES.txt.bak
+-rw-rw-rw-   0        0        0        1 2023-07-14 18:00:56.000000 mayatk-0.6.9/mayatk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-14 18:00:56.000000 mayatk-0.6.9/mayatk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 18:00:56.833407 mayatk-0.6.9/setup.cfg
+-rw-rw-rw-   0        0        0     1442 2023-06-28 02:16:01.000000 mayatk-0.6.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 18:00:56.829832 mayatk-0.6.9/test/
+-rw-rw-rw-   0        0        0     1289 2023-05-20 14:01:35.000000 mayatk-0.6.9/test/__init__.py
+-rw-rw-rw-   0        0        0    26026 2023-06-28 00:01:13.000000 mayatk-0.6.9/test/cmpt_utils_test.py
+-rw-rw-rw-   0        0        0     6935 2023-07-03 18:22:03.000000 mayatk-0.6.9/test/core_utils_test.py
+-rw-rw-rw-   0        0        0     7676 2023-06-28 00:35:52.000000 mayatk-0.6.9/test/edit_utils_test.py
+-rw-rw-rw-   0        0        0     4505 2023-06-28 02:10:41.000000 mayatk-0.6.9/test/mat_utils_test.py
+-rw-rw-rw-   0        0        0     7396 2023-06-28 00:17:04.000000 mayatk-0.6.9/test/node_utils_test.py
+-rw-rw-rw-   0        0        0     5086 2023-06-28 01:40:55.000000 mayatk-0.6.9/test/rig_utils_test.py
+-rw-rw-rw-   0        0        0     2068 2023-06-28 01:24:21.000000 mayatk-0.6.9/test/run_tests.py
+-rw-rw-rw-   0        0        0     7298 2023-06-28 01:39:40.000000 mayatk-0.6.9/test/xform_utils_test.py
```

### Comparing `mayatk-0.6.8/LICENSE` & `mayatk-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.8/mayatk/__init__.py` & `mayatk-0.6.9/mayatk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 import inspect
 import importlib
 import pkgutil
 
 
 __package__ = "mayatk"
-__version__ = '0.6.8'
+__version__ = '0.6.9'
 
 
 # Define dictionaries to map class names, method names, class method names, and sub-modules to their respective modules
 CLASS_TO_MODULE = {}
 METHOD_TO_MODULE = {}
 CLASS_METHOD_TO_MODULE = {}
 SUBMODULE_TO_MODULE = {}
```

### Comparing `mayatk-0.6.8/mayatk/cam_utils.py` & `mayatk-0.6.9/mayatk/cam_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 # coding=utf-8
 try:
     import pymel.core as pm
 except ImportError as error:
     print(__file__, error)
 
 # from this package:
-from mayatk import utils
+from mayatk import core_utils
 
 
 class Cam(object):
     """ """
 
     @staticmethod
-    @utils.Utils.undo
+    @core_utils.CoreUtils.undo
     def group_cameras(
         name="cameras", non_default=True, root_only=False, hide_group=False
     ):
         """Group cameras in the scene based on the provided parameters.
 
         Parameters:
                 name (str): The name of the group that will contain the cameras. Default is 'cameras'.
@@ -100,26 +100,26 @@
         view = M3dView.active3dView()
         cam = MDagPath()
         view.getCamera(cam)
         camPath = cam.fullPathName()
         return camPath
 
     @staticmethod
-    @utils.Utils.undo
+    @core_utils.CoreUtils.undo
     def create_camera_from_view(name="camera#"):
         """Create a new camera based on the current view."""
         # Find the current modelPanel (viewport)
         current_panel = None
-        for panel in utils.Utils.get_panel(all=True):
-            if utils.Utils.get_panel(typeOf=panel) == "modelPanel":
+        for panel in core_utils.CoreUtils.get_panel(all=True):
+            if core_utils.CoreUtils.get_panel(typeOf=panel) == "modelPanel":
                 current_panel = panel
                 break
 
         if current_panel:
-            if utils.Utils.get_panel(typeOf=current_panel) == "modelPanel":
+            if core_utils.CoreUtils.get_panel(typeOf=current_panel) == "modelPanel":
                 camera = pm.modelPanel(current_panel, q=1, cam=1)
                 new_camera = pm.duplicate(camera)[0]
                 pm.showHidden(new_camera)
                 new_camera = pm.rename(new_camera, name)
                 print(f"# Result: {new_camera} #")
                 return new_camera
         else:
```

### Comparing `mayatk-0.6.8/mayatk/cmpt_utils.py` & `mayatk-0.6.9/mayatk/cmpt_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 try:
     import pymel.core as pm
 except ImportError as error:
     print(__file__, error)
 import pythontk as ptk
 
 # from this package:
-from mayatk import utils, node_utils
+from mayatk import core_utils, node_utils
 
 
 class GetComponentsMixin:
     """ """
 
     componentTypes = [  # abv, singular, plural, full, int, hex
         (
@@ -330,15 +330,15 @@
         )  # get the correct component_type variable from possible args.
 
         if typ not in d:
             return components
         components = pm.polyListComponentConversion(
             components, **{d[typ.lower()]: True}
         )
-        return utils.Utils.convert_array_type(
+        return core_utils.CoreUtils.convert_array_type(
             components, returned_type=returned_type, flatten=flatten
         )
 
     @classmethod
     def convert_int_to_component(
         cls, obj, integers, component_type, returned_type="str", flatten=False
     ):
@@ -370,15 +370,15 @@
             result = [
                 "{}.{}[{}]".format(objName, component_type, n(c))
                 for c in ptk.split_list(integers, "range")
             ]
         else:
             result = ["{}.{}[{}]".format(objName, component_type, c) for c in integers]
 
-        return utils.Utils.convert_array_type(
+        return core_utils.CoreUtils.convert_array_type(
             result, returned_type=returned_type, flatten=flatten
         )
 
     @classmethod
     def filter_components(cls, components, inc=[], exc=[], flatten=False):
         """Filter the given components.
 
@@ -393,17 +393,17 @@
             (list)
 
         Example:
             filter_components('cyl.vtx[:]', 'cyl.vtx[:2]', 'cyl.vtx[1:23]') #returns: ['cyl.vtx[0]']
             filter_components('cyl.f[:]', range(2), range(1, 23)) #returns: ['cyl.f[0]']
         """
         typ = cls.get_component_type(components)
-        etyp = utils.Utils.get_array_type(components)
-        etyp_inc = utils.Utils.get_array_type(inc)
-        etyp_exc = utils.Utils.get_array_type(exc)
+        etyp = core_utils.CoreUtils.get_array_type(components)
+        etyp_inc = core_utils.CoreUtils.get_array_type(inc)
+        etyp_exc = core_utils.CoreUtils.get_array_type(exc)
 
         if etyp_inc == "int" or etyp_exc == "int":
             try:
                 obj = pm.ls(components, objectsOnly=True)[0]
             except IndexError as e:
                 print(
                     f'File "{__file__}" in filter_components\n# Error: Operation requires at least one component. #\n{e}',
@@ -417,15 +417,15 @@
         if etyp_exc == "int":
             exc = cls.convert_int_to_component(obj, exc, typ)
         exc = pm.ls(exc, flatten=True)
 
         components = pm.ls(components, flatten=True)
 
         filtered = ptk.filter_list(components, inc=inc, exc=exc)
-        result = utils.Utils.convert_array_type(
+        result = core_utils.CoreUtils.convert_array_type(
             filtered, returned_type=etyp, flatten=flatten
         )
         return result
 
     @classmethod
     def get_components(
         cls,
@@ -465,15 +465,15 @@
 
         if inc or exc:
             components = cls.filter_components(components, inc=inc, exc=exc)
 
         if randomize:
             components = randomize(pm.ls(components, flatten=1), randomize)
 
-        result = utils.Utils.convert_array_type(
+        result = core_utils.CoreUtils.convert_array_type(
             components, returned_type=returned_type, flatten=flatten
         )
         return result
 
 
 class CmptUtils(GetComponentsMixin):
     """ """
@@ -687,15 +687,15 @@
                 attachedFaces = cls.convert_component_type(edge, "face", flatten=1)
                 if len(attachedFaces) == 1:
                     result.append(edge)
 
         result = cls.convert_component_type(
             result, component_type
         )  # convert back to the original component type and flatten /un-flatten list.
-        result = utils.Utils.convert_array_type(
+        result = core_utils.CoreUtils.convert_array_type(
             result, returned_type=returned_type, flatten=flatten
         )
         return result
 
     @classmethod
     def get_closest_verts(cls, a, b, tolerance=1000):
         """Find the two closest vertices between the two sets of vertices.
@@ -709,16 +709,20 @@
             (list): closest vertex pairs by order of distance (excluding those not meeting the tolerance). (<vertex from a>, <vertex from b>).
 
         Example:
             get_closest_verts('pln.vtx[:10]', 'pln.vtx[11:]', 6.667) #returns: [('plnShape.vtx[7]', 'plnShape.vtx[11]'), ('plnShape.vtx[8]', 'plnShape.vtx[12]'), ('plnShape.vtx[9]', 'plnShape.vtx[13]'), ('plnShape.vtx[10]', 'plnShape.vtx[11]'), ('plnShape.vtx[10]', 'plnShape.vtx[14]')]
         """
         from operator import itemgetter
 
-        a = utils.Utils.convert_array_type(a, returned_type="str", flatten=True)
-        b = utils.Utils.convert_array_type(b, returned_type="str", flatten=True)
+        a = core_utils.CoreUtils.convert_array_type(
+            a, returned_type="str", flatten=True
+        )
+        b = core_utils.CoreUtils.convert_array_type(
+            b, returned_type="str", flatten=True
+        )
         vertPairsAndDistance = {}
         for v1 in a:
             v1Pos = pm.pointPosition(v1, world=1)
             for v2 in b:
                 v2Pos = pm.pointPosition(v2, world=1)
                 distance = ptk.get_distance(v1Pos, v2Pos)
                 if distance < tolerance:
@@ -747,15 +751,15 @@
             (dict) closest vertex pairs {<vertex from a>:<vertex from b>}.
 
         Example:
             get_closest_vertex('plnShape.vtx[0]', 'cyl', returned_type='int') #returns: {'plnShape.vtx[0]': 3},
             get_closest_vertex('plnShape.vtx[0]', 'cyl') #returns: {'plnShape.vtx[0]': 'cylShape.vtx[3]'},
             get_closest_vertex('plnShape.vtx[2:3]', 'cyl') #returns: {'plnShape.vtx[2]': 'cylShape.vtx[2]', 'plnShape.vtx[3]': 'cylShape.vtx[1]'}
         """
-        vertices = utils.Utils.convert_array_type(
+        vertices = core_utils.CoreUtils.convert_array_type(
             vertices, returned_type="str", flatten=True
         )
         pm.undoInfo(openChunk=True)
 
         if freeze_transforms:
             pm.makeIdentity(obj, apply=True)
 
@@ -781,15 +785,15 @@
                 cpmNode.closestVertexIndex
             )  # vertex Index. | ie. result: [34]
             v2 = obj2Shape.vtx[index]
 
             v2Pos = pm.pointPosition(v2, world=True)
             distance = ptk.get_distance(v1Pos, v2Pos)
 
-            v2_convertedType = utils.Utils.convert_array_type(
+            v2_convertedType = core_utils.CoreUtils.convert_array_type(
                 v2, returned_type=returned_type
             )[0]
             if not tolerance:
                 closestVerts[v1] = v2_convertedType
             elif distance < tolerance:
                 closestVerts[v1] = v2_convertedType
 
@@ -861,15 +865,15 @@
         else:  # EdgeLoop
             edgesLong = pm.polySelect(obj, q=True, edgeLoop=cnums)  # (e..)
 
         objName = obj.name()
         result = ptk.remove_duplicates(
             ["{}.e[{}]".format(objName, e) for e in edgesLong]
         )
-        return utils.Utils.convert_array_type(
+        return core_utils.CoreUtils.convert_array_type(
             result, returned_type=returned_type, flatten=flatten
         )
 
     @classmethod
     def get_shortest_path(cls, components, returned_type="str", flatten=False):
         """Get the shortest path between two components.
 
@@ -1345,15 +1349,17 @@
         result = []
         for c in pm.ls(components, flatten=True):
             attached = cls.convert_component_type(c, ctype, flatten=True)
             n = len(attached)
             if n >= lowRange and n <= highRange:
                 result.append(c)
 
-        result = utils.Utils.convert_array_type(result, returned_type=returned_type)
+        result = core_utils.CoreUtils.convert_array_type(
+            result, returned_type=returned_type
+        )
         return result
 
     @classmethod
     def get_vertex_normal(cls, vertex, angle_weighted=False):
         """Return the normal at the given vertex. The returned normal is a single
         per-vertex normal, so unshared normals at a vertex will be averaged.
 
@@ -1370,15 +1376,15 @@
         mesh = pm.ls(vertex, objectsOnly=True)[0].name()
         selectionList = om.MSelectionList()  # empty selection list.
         selectionList.add(mesh)
 
         dagPath = selectionList.getDagPath(0)  # create empty dag path object.
         mesh = om.MFnMesh(dagPath)  # get mesh.
 
-        vtxID = utils.Utils.convert_array_type(vertex, "int")[0]
+        vtxID = core_utils.CoreUtils.convert_array_type(vertex, "int")[0]
         # get vertex normal and use om.MSpace.kObject for object space.
         return mesh.getVertexNormal(vtxID, angle_weighted, space=om.MSpace.kWorld)
 
     @staticmethod
     def get_vector_from_components(components):
         """Get a vector representing the averaged and normalized vertex-face normals.
 
@@ -1616,10 +1622,10 @@
 #           obj = pm.ls(frm, objectsOnly=1)
 #           if len(obj)>1:
 #               return frm
 #           component_type = cls.get_component_type(frm[0])
 #           typ = cls.convert_alias(component_type) #get the correct component_type variable from possible args.
 #           inc = ["{}.{}[{}]".format(obj[0], typ, n) for n in inc]
 
-#       inc = utils.Utils.convert_array_type(inc, returned_type=rtn, flatten=True) #assure both lists are of the same type for comparison.
-#       exc = utils.Utils.convert_array_type(exc, returned_type=rtn, flatten=True)
+#       inc = core_utils.CoreUtils.convert_array_type(inc, returned_type=rtn, flatten=True) #assure both lists are of the same type for comparison.
+#       exc = core_utils.CoreUtils.convert_array_type(exc, returned_type=rtn, flatten=True)
 #       return [i for i in components if i not in exc and (inc and i in inc)]
```

### Comparing `mayatk-0.6.8/mayatk/display_utils/exploded_view.py` & `mayatk-0.6.9/mayatk/display_utils/exploded_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     print(__file__, error)
 try:
     import maya.OpenMaya as om
 except ModuleNotFoundError as error:
     print(__file__, error)
 
 # from this package:
-from mayatk.utils import Utils
+from mayatk.core_utils import CoreUtils
 from mayatk.xform_utils import XformUtils
 from mayatk.node_utils import NodeUtils
 
 
 class ExplodedView:
     exploded_objects = []
 
@@ -183,15 +183,15 @@
 
 
 def launch_gui(move_to_cursor=False, frameless_window=False):
     """Launch the UI"""
     from PySide2 import QtCore, QtGui
     from uitk import Switchboard
 
-    parent = Utils.get_main_window()
+    parent = CoreUtils.get_main_window()
     sb = Switchboard(
         parent, ui_location="exploded_view.ui", slots_location=ExplodedViewSlots
     )
     if frameless_window:
         sb.ui.setWindowFlags(QtCore.Qt.Tool | QtCore.Qt.FramelessWindowHint)
         sb.ui.setAttribute(QtCore.Qt.WA_TranslucentBackground)
     else:
```

### Comparing `mayatk-0.6.8/mayatk/edit_utils.py` & `mayatk-0.6.9/mayatk/edit_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 try:
     import pymel.core as pm
 except ImportError as error:
     print(__file__, error)
 import pythontk as ptk
 
 # from this package:
-from mayatk import utils, node_utils, cmpt_utils, xform_utils
+from mayatk import core_utils, node_utils, cmpt_utils, xform_utils
 
 
 class EditUtils:
     """ """
 
     @staticmethod
-    @utils.Utils.undo
+    @core_utils.CoreUtils.undo
     def rename(objects, to, fltr="", regex=False, ignore_case=False):
         """Rename scene objects.
 
         Parameters:
             objects (str/obj/list): The object(s to rename. If nothing is given, all scene objects will be renamed.
             to (str): Desired name: An optional asterisk modifier can be used for formatting
                     chars - replace all.
@@ -88,15 +88,15 @@
                         '# Error: Attempt to rename "{}" to "{}" failed. {} #'.format(
                             oldName, newName, str(e).rstrip()
                         )
                     )
         # pm.undoInfo (closeChunk=1)
 
     @staticmethod
-    @utils.Utils.undo
+    @core_utils.CoreUtils.undo
     def set_case(objects=[], case="caplitalize"):
         """Rename objects following the given case.
 
         Parameters:
             objects (str/list): The objects to rename. default:all scene objects
             case (str): Desired case using python case operators.
                     valid: 'upper', 'lower', 'caplitalize', 'swapcase' 'title'. default:'caplitalize'
@@ -113,15 +113,15 @@
                 pm.rename(name, newName)
             except Exception as error:
                 if not pm.ls(obj, readOnly=True) == []:  # ignore read-only errors.
                     print(name + ": ", error)
         # pm.undoInfo(closeChunk=1)
 
     @staticmethod
-    @utils.Utils.undo
+    @core_utils.CoreUtils.undo
     def append_location_based_suffix(
         objects,
         alphanumeric=False,
         strip_trailing_ints=True,
         strip_trailing_alpha=True,
         reverse=False,
     ):
@@ -628,15 +628,15 @@
 
         Returns:
             (list)
         """
         import maya.OpenMaya as om
 
         result = []
-        for mfnMesh in utils.Utils.mfn_mesh_generator(objects):
+        for mfnMesh in core_utils.CoreUtils.mfn_mesh_generator(objects):
             points = om.MPointArray()
             mfnMesh.getPoints(points, om.MSpace.kWorld)
 
             for i in range(points.length()):
                 for ii in range(points.length()):
                     if i == ii:
                         continue
```

### Comparing `mayatk-0.6.8/mayatk/macro_utils.py` & `mayatk-0.6.9/mayatk/macro_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.8/mayatk/mash_utils.py` & `mayatk-0.6.9/mayatk/mash_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.8/mayatk/mat_utils/mat_utils.py` & `mayatk-0.6.9/mayatk/mat_utils/mat_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.8/mayatk/mat_utils/stingray_arnold_shader.py` & `mayatk-0.6.9/mayatk/mat_utils/stingray_arnold_shader.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     import pymel.core as pm
 except ImportError as error:
     print(__file__, error)
 from uitk import Switchboard
 import pythontk as ptk
 
 # from this package:
-from mayatk.utils import Utils
+from mayatk.core_utils import CoreUtils
 from mayatk.node_utils import NodeUtils
 
 
 __version__ = "0.5.3"
 
 
 class StingrayArnoldShader:
@@ -55,15 +55,15 @@
         file_node = NodeUtils.get_incoming_node_by_type(node, "file")
         if not file_node:
             file_node = NodeUtils.create_render_node(
                 "file", "as2DTexture", texture_node=True
             )
             pm.connectAttr(file_node.outColor, node.color, force=True)
 
-        file_node.fileTextureName.set(tex)
+        file_node.fileTextureName.set(str(tex))
 
     @property
     def hdr_env_transform(self) -> object:
         """ """
         node = NodeUtils.get_transform_node(self.hdr_env)
         if not node:
             return None
@@ -71,15 +71,15 @@
 
     def set_hdr_map_visibility(self, state):
         """ """
         node = self.hdr_env
         if node:
             node.camera.set(state)
 
-    @Utils.undo
+    @CoreUtils.undo
     def create_network(
         self,
         textures,
         name="",
         hdrMap="",
         hdrMapVisibility=False,
         normalMapType="OpenGL",
@@ -296,15 +296,15 @@
         self.sb = self.switchboard()
         self.image_files = None
 
         # Add filenames|filepaths to the comboBox.
         hdr_path = f"{self.proj_root_dir}/resources/hdr"
         hdr_filenames = ptk.get_dir_contents(hdr_path, "filenames", inc_files="*.exr")
         hdr_fullpaths = ptk.get_dir_contents(hdr_path, "filepaths", inc_files="*.exr")
-        self.sb.ui.cmb000.add(dict(zip(hdr_filenames, hdr_fullpaths)), ascending=False)
+        self.sb.ui.cmb000.add(zip(hdr_filenames, hdr_fullpaths), ascending=False)
 
         self.sb.ui.txt001.setText(self.msg_intro)
 
         node = self.hdr_env_transform
         if node:
             rotation = node.rotateY.get()
             self.sb.ui.slider000.setSliderPosition(rotation)
@@ -455,27 +455,24 @@
 
     def __init__(self, parent=None, **kwargs):
         super().__init__(parent)
 
         self.ui_location = "stingray_arnold_shader.ui"
         self.slots_location = StingrayArnoldShaderSlots
 
-        self.ui.draggableHeader.hide()
         self.ui.txt001.hide()
-
         self.ui.resize(self.ui.sizeHint())
 
 
 # -----------------------------------------------------------------------------
 
 if __name__ == "__main__":
-    parent = Utils.get_main_window()
+    parent = CoreUtils.get_main_window()
     sb = StingrayArnoldShaderUI(parent)
     sb.ui.set_style(theme="dark")
+    sb.ui.stays_on_top = True
+    sb.ui.draggableHeader.hide()
     sb.ui.show(app_exec=True)
 
 # -----------------------------------------------------------------------------
 # Notes
 # -----------------------------------------------------------------------------
-
-
-# Deprecated ------------------------------------
```

### Comparing `mayatk-0.6.8/mayatk/misc_utils.py.bak` & `mayatk-0.6.9/mayatk/core_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # !/usr/bin/python
 # coding=utf-8
-import os, sys
+import os
+import sys
 
 try:
     import pymel.core as pm
 except ImportError as error:
     print(__file__, error)
-from pythontk import Iter
+import pythontk as ptk
 
 # from this package:
 from mayatk import node_utils
 
 
-class Misc:
+class CoreUtils:
     """ """
 
     def undo(fn):
         """A decorator to place a function into Maya's undo chunk.
         Prevents the undo queue from breaking entirely if an exception is raised within the given function.
 
         Parameters:
@@ -120,15 +121,15 @@
         """
         from PySide2 import QtWidgets
         from shiboken2 import wrapInstance
         from maya.OpenMayaUI import MQtUtil
 
         layout = QtWidgets.QVBoxLayout(container)
         layout.setContentsMargins(0, 0, 0, 0)
-        layoutName = Str.set_case(
+        layoutName = ptk.set_case(
             container.objectName() + "Layout", "camel"
         )  # results in '<objectName>Layout' or 'layout' if container objectName is ''
         layout.setObjectName(layoutName)
         pm.setParent(layoutName)
 
         from uitk.switchboard import Switchboard
 
@@ -151,46 +152,48 @@
 
         Returns:
             (generator)
         """
         import maya.OpenMaya as om
 
         selectionList = om.MSelectionList()
-        for mesh in node_utils.Node.get_shape_node(pm.ls(objects)):
+        for mesh in node_utils.NodeUtils.get_shape_node(pm.ls(objects)):
             selectionList.add(mesh)
 
         for i in range(selectionList.length()):
             dagPath = om.MDagPath()
             selectionList.getDagPath(i, dagPath)
             # print (dagPath.fullPathName()) #debug
             mfnMesh = om.MFnMesh(dagPath)
             yield mfnMesh
 
     @staticmethod
-    def get_array_type(lst):
-        """Determine if the given element(s) type.
+    def get_array_type(array):
+        """Determine the given element(s) type.
         Samples only the first element.
 
         Parameters:
-            obj (str/obj/list): The components(s) to query.
+            array (str/obj/list): The components(s) to query.
 
         Returns:
-            (list) 'str', 'obj'(shape node), 'transform'(as string), 'int'(valid only at sub-object level)
-
-        Example:
-        get_array_type('cyl.vtx[0]') #returns: 'transform'
-        get_array_type('cylShape.vtx[:]') #returns: 'str'
+            (list) 'str', 'int'(valid only at sub-object level), or maya object type as string.
         """
         try:
-            o = Iter.make_iterable(lst)[0]
-        except IndexError as error:
+            o = ptk.make_iterable(array)[0]
+        except IndexError:
             # print (f'# Error: {__file__} in get_array_type:\n#\tOperation requires at least one object.\n#\t{error}')
             return ""
 
-        return "str" if isinstance(o, str) else "int" if isinstance(o, int) else "obj"
+        return (
+            "str"
+            if isinstance(o, str)
+            else "int"
+            if isinstance(o, int)
+            else node_utils.NodeUtils.get_type(o)
+        )
 
     @staticmethod
     def convert_array_type(lst, returned_type="str", flatten=False):
         """Convert the given element(s) to <obj>, 'str', or int values.
 
         Parameters:
             lst (str/obj/list): The components(s) to convert.
@@ -236,16 +239,16 @@
                     )
                     break
 
             objects = set(pm.ls(lst, objectsOnly=True))
             if (
                 len(objects) == 1
             ):  # flatten the dict values from 'result' and remove any duplicates.
-                flattened = Iter.flatten(result.values())
-                result = Iter.remove_duplicates(flattened)
+                flattened = ptk.flatten(result.values())
+                result = ptk.remove_duplicates(flattened)
 
         elif returned_type == "str":
             result = list(map(str, lst))
 
         else:
             result = lst
 
@@ -268,25 +271,18 @@
         Example:
             >>> get_parameter_mapping(obj, 'transformLimits', ['enableTranslationX','translationX'])
             {'enableTranslationX': [False, False], 'translationX': [-1.0, 1.0]}
         """
         cmd = getattr(pm, cmd)
         node = pm.ls(node)[0]
 
-        result = {}
-        for p in parameters:
-            # Query the parameter to get it's value.
-            values = cmd(node, **{"q": True, p: True})
-
-            result[p] = values
-
-        return result
+        return {p: cmd(node, **{"q": True, p: True}) for p in parameters}
 
     @staticmethod
-    def set_parameter_values(node, cmd, parameters):
+    def set_parameter_mapping(node, cmd, parameters):
         """Applies a set of parameter values to a specified Maya node using a given Maya command.
 
         Parameters:
             node (str/obj/list): The object to query attributes of.
             parameters (dict): The command's parameters and their desired values. ie. {'enableTranslationX': [False, False], 'translationX': [-1.0, 1.0]}
 
         Example:
@@ -313,15 +309,15 @@
         if attrs is None:
             attrs = []
         return attrs
 
     @staticmethod
     def get_panel(*args, **kwargs):
         """Returns panel and panel configuration information.
-        A fix for the broken pymel command of the same name.
+        A fix for the broken pymel command `getPanel`.
 
         Parameters:
             [allConfigs=boolean], [allPanels=boolean], [allScriptedTypes=boolean], [allTypes=boolean], [configWithLabel=string], [containing=string], [invisiblePanels=boolean], [scriptType=string], [type=string], [typeOf=string], [underPointer=boolean], [visiblePanels=boolean], [withFocus=boolean], [withLabel=string])
 
         Returns:
             (str) An array of panel names.
         """
@@ -395,14 +391,45 @@
             fade=fade,
             fadeInTime=fadeInTime,
             fadeStayTime=fadeStayTime,
             fadeOutTime=fadeOutTime,
             alpha=alpha,
         )  # 1000ms = 1 sec
 
+    @staticmethod
+    def get_mel_globals(keyword=None, ignore_case=True):
+        """Get global MEL variables."""
+        variables = [
+            v
+            for v in sorted(pm.mel.eval("env"))
+            if not keyword
+            or (
+                v.count(keyword)
+                if not ignore_case
+                else v.lower().count(keyword.lower())
+            )
+        ]
+        return variables
+
+    @staticmethod
+    def list_ui_objects():
+        """List all UI objects."""
+        ui_objects = {
+            "windows": pm.lsUI(windows=True),
+            "panels": pm.lsUI(panels=True),
+            "editors": pm.lsUI(editors=True),
+            "menus": pm.lsUI(menus=True),
+            "menuItems": pm.lsUI(menuItems=True),
+            "controls": pm.lsUI(controls=True),
+            "controlLayouts": pm.lsUI(controlLayouts=True),
+            "contexts": pm.lsUI(contexts=True),
+        }
+        for category, objects in ui_objects.items():
+            print(f"{category}:\n{objects}\n")
+
 
 # --------------------------------------------------------------------------------------------
 
 if __name__ == "__main__":
     pass
 
 # --------------------------------------------------------------------------------------------
```

### Comparing `mayatk-0.6.8/mayatk/node_utils.py` & `mayatk-0.6.9/mayatk/node_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 try:
     import pymel.core as pm
 except ImportError as error:
     print(__file__, error)
 import pythontk as ptk
 
 # from this package:
-from mayatk import utils, cmpt_utils
+from mayatk import core_utils, cmpt_utils
 
 
 class NodeUtils:
     """ """
 
     @staticmethod
     def node_exists(n, search="name"):
@@ -206,15 +206,15 @@
             for n in transforms:
                 result.append(n)
 
         if attributes:
             result = pm.listAttr(result, read=1, hasData=1)
 
         # convert element type.
-        result = utils.Utils.convert_array_type(
+        result = core_utils.CoreUtils.convert_array_type(
             result, returned_type=returned_type, flatten=True
         )
         # filter
         result = ptk.filter_list(result, inc, exc)
         # return as list if `nodes` was given as a list.
         return ptk.format_return(list(set(result)), nodes)
 
@@ -251,15 +251,15 @@
             for n in shapes:
                 result.append(n)
 
         if attributes:
             result = pm.listAttr(result, read=1, hasData=1)
 
         # convert element type.
-        result = utils.Utils.convert_array_type(
+        result = core_utils.CoreUtils.convert_array_type(
             result, returned_type=returned_type, flatten=True
         )
         # filter
         result = ptk.filter_list(result, inc, exc)
         # return as list if `nodes` was given as a list.
         return ptk.format_return(list(set(result)), nodes)
 
@@ -297,15 +297,15 @@
                     continue
             result.append(history)
 
         if attributes:
             result = pm.listAttr(result, read=1, hasData=1)
 
         # convert element type.
-        result = utils.Utils.convert_array_type(
+        result = core_utils.CoreUtils.convert_array_type(
             result, returned_type=returned_type, flatten=True
         )
         # filter
         result = ptk.filter_list(result, inc, exc)
         # return as list if `nodes` was given as a list.
         return ptk.format_return(list(set(result)), nodes)
```

### Comparing `mayatk-0.6.8/mayatk/project_utils.py` & `mayatk-0.6.9/mayatk/proj_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 try:
     import pymel.core as pm
 except ImportError as error:
     print(__file__, error)
 import pythontk as ptk
 
 
-class ProjectUtils:
+class ProjUtils:
     """ """
 
     @staticmethod
     def get_recent_files(index=None, format="standard"):
         """
         Get a list of recent files.
 
@@ -271,60 +271,7 @@
 
 if __name__ == "__main__":
     pass
 
 # -----------------------------------------------------------------------------
 # Notes
 # -----------------------------------------------------------------------------
-
-
-# deprecated ---------------------
-# @staticmethod
-# def reference_scene(scene, remove=False, lockReference=False):
-#     """Create a reference to a Maya scene.
-
-#     Parameters:
-#         remove (bool): Remove a previously referenced scene.
-#     """
-#     if remove:  # unload reference.
-#         # refNode = pm.referenceQuery(scene, referenceNode=True)
-#         pm.mel.file(scene, removeReference=True)
-
-#     else:  # load reference.
-#         # ex. 'sceneName' from 'sceneName.mb'
-#         namespace = scene.split("\\")[-1].rstrip(".mb").rstrip(".ma")
-#         pm.mel.file(
-#             scene,
-#             reference=True,
-#             namespace=namespace,
-#             groupReference=True,
-#             lockReference=lockReference,
-#             loadReferenceDepth="topOnly",
-#             force=True,
-#         )
-
-# @staticmethod
-# def get_recent_autosave(timestamp=False):
-#     """Get a list of autosave files.
-
-#     Parameters:
-#         timestamp (bool): Attach a modified timestamp and date to given file path(s).
-
-#     Returns:
-#         (list)
-#     """
-# dir1 = str(pm.workspace(q=True, rd=1)) + "autosave"  # current project path.
-# # get autosave dir path from env variable.
-# dir2 = os.environ.get("MAYA_AUTOSAVE_FOLDER")
-# if dir2 is not None:  # Check if the environment variable exists
-#     dir2 = dir2.split(";")[0]
-
-#     result = ptk.get_dir_contents(dir1, "filepaths", inc_files=("*.mb", "*.ma"))
-#     if dir2 is not None:  # Add the files from the second directory if it exists
-#         result += ptk.get_dir_contents(dir2, "filepaths", inc_files=("*.mb", "*.ma"))
-#     # # Replace any backslashes with forward slashes and reverse the list.
-#     # result = [ptk.format_path(f) for f in list(reversed(files))]
-
-#     if timestamp:  # attach modified timestamp
-#         result = ptk.time_stamp(result, sort=True)
-
-#     return result
```

### Comparing `mayatk-0.6.8/mayatk/rig_utils.py` & `mayatk-0.6.9/mayatk/rig_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.8/mayatk/xform_utils.py` & `mayatk-0.6.9/mayatk/xform_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 try:
     import pymel.core as pm
 except ImportError as error:
     print(__file__, error)
 import pythontk as ptk
 
 # from this package:
-from mayatk import utils, cmpt_utils
+from mayatk import core_utils, cmpt_utils
 
 
 class XformUtils:
     """ """
 
     @staticmethod
     def move_to(source, target, center=True):
@@ -37,15 +37,15 @@
             target_pos = pm.xform(
                 target, q=1, worldSpace=1, rp=1
             )  # get the pivot position.
 
         pm.xform(source, translation=target_pos, worldSpace=1, relative=1)
 
     @staticmethod
-    @utils.Utils.undo
+    @core_utils.CoreUtils.undo
     def drop_to_grid(
         objects, align="Mid", origin=False, center_pivot=False, freeze_transforms=False
     ):
         """Align objects to Y origin on the grid using a helper plane.
 
         Parameters:
             objects (str/obj/list): The objects to translate.
@@ -83,15 +83,15 @@
                 )  # return pivot to orig position.
 
             if freeze_transforms:
                 pm.makeIdentity(obj, apply=True)
         # pm.undoInfo (closeChunk=1)
 
     @classmethod
-    @utils.Utils.undo
+    @core_utils.CoreUtils.undo
     def reset_translation(cls, objects):
         """Reset the translation transformations on the given object(s).
 
         Parameters:
             objects (str/obj/list): The object(s) to reset the translation values for.
         """
         # pm.undoInfo(openChunk=1)
@@ -115,15 +115,15 @@
         """
         x, y, z = pm.xform(node, query=True, worldSpace=True, rotatePivot=True)
         pm.xform(node, relative=True, translation=[-x, -y, -z])
         pm.makeIdentity(node, apply=True, translate=True)
         pm.xform(node, translation=[x, y, z])
 
     @staticmethod
-    @utils.Utils.undo
+    @core_utils.CoreUtils.undo
     def align_pivot_to_selection(align_from=[], align_to=[], translate=True):
         """Align one objects pivot point to another using 3 point align.
 
         Parameters:
             align_from (list): At minimum; 1 object, 1 Face, 2 Edges, or 3 Vertices.
             align_to (list): The object to align with.
             translate (bool): Move the object with it's pivot.
@@ -168,15 +168,15 @@
             if translate:
                 pm.xform(obj, translation=center_pos, worldSpace=True)
 
             pm.delete(plane)
         # pm.undoInfo(closeChunk=1)
 
     @staticmethod
-    @utils.Utils.undo
+    @core_utils.CoreUtils.undo
     def aim_object_at_point(objects, target_pos, aim_vect=(1, 0, 0), up_vect=(0, 1, 0)):
         """Aim the given object(s) at the given world space position.
 
         Paramters:
             objects (str/obj/list): Transform node(s) of the objects to orient.
             target_pos (obj)(tuple): A point as xyz, or one or more transform nodes at which to aim the other given 'objects'.
             aim_vect (tuple): The vector in local coordinates that points at the target.
@@ -194,15 +194,15 @@
             const = pm.aimConstraint(
                 target, obj, aim=aim_vect, worldUpVector=up_vect, worldUpType="vector"
             )
 
         pm.delete(const, target)
 
     @classmethod
-    @utils.Utils.undo
+    @core_utils.CoreUtils.undo
     def rotate_axis(cls, objects, target_pos):
         """Aim the given object at the given world space position.
         All rotations in rotated channel, geometry is transformed so
         it does not appear to move during this transformation
 
         Parameters:
             objects (str/obj/list): Transform node(s) of the objects to orient.
@@ -501,15 +501,15 @@
             (list) Nested lists if multiple objects given.
         """
         import maya.OpenMaya as om
 
         space = om.MSpace.kWorld if worldSpace else om.MSpace.kObject
 
         result = []
-        for mesh in utils.Utils.mfn_mesh_generator(objects):
+        for mesh in core_utils.CoreUtils.mfn_mesh_generator(objects):
             points = om.MPointArray()
             mesh.getPoints(points, space)
 
             result.append(
                 [
                     (points[i][0], points[i][1], points[i][2])
                     for i in range(points.length())
@@ -582,15 +582,15 @@
 
             distance[bb_dist] = obj
 
         result = [distance[i] for i in sorted(distance)]
         return list(reversed(result)) if reverse else result
 
     @staticmethod
-    @utils.Utils.undo
+    @core_utils.CoreUtils.undo
     def align_vertices(mode, average=False, edgeloop=False):
         """Align vertices.
 
         Parameters:
             mode (int): possible values are align: 0-YZ, 1-XZ, 2-XY, 3-X, 4-Y, 5-Z, 6-XYZ
             average (bool): align to average of all selected vertices. else, align to last selected
             edgeloop (bool): align vertices in edgeloop from a selected edge
@@ -620,16 +620,18 @@
             z = xyz[2::3]
             alignX = float(sum(x)) / (len(xyz) / 3)
             alignY = float(sum(y)) / (len(xyz) / 3)
             alignZ = float(sum(z)) / (len(xyz) / 3)
 
         if len(selection) < 2:
             if len(selection) == 0:
-                utils.Utils.viewport_message("No vertices selected")
-            utils.Utils.viewport_message("Selection must contain at least two vertices")
+                core_utils.CoreUtils.viewport_message("No vertices selected")
+            core_utils.CoreUtils.viewport_message(
+                "Selection must contain at least two vertices"
+            )
 
         for vertex in selection:
             vertexXYZ = pm.xform(vertex, q=True, translation=1, worldSpace=1)
             vertX = vertexXYZ[0]
             vertY = vertexXYZ[1]
             vertZ = vertexXYZ[2]
 
@@ -654,177 +656,7 @@
 
 if __name__ == "__main__":
     pass
 
 # -----------------------------------------------------------------------------
 # Notes
 # -----------------------------------------------------------------------------
-
-
-# deprecated ---------------------
-
-# @staticmethod
-# def snap3PointsTo3Points(vertices):
-#     """Move and align the object defined by the first 3 points to the last 3 points.
-
-#     Parameters:
-#             vertices (list): The first 3 points must be on the same object (i.e. it is the
-#                                     object to be transformed). The second set of points define
-#                                     the position and plane to transform to.
-#     """
-#     import math
-
-#     vertices = pm.ls(vertices, flatten=True)
-#     objectToMove = pm.ls(vertices[:3], objectsOnly=True)
-
-#     # get the world space position of each selected point object
-#     p0, p1, p2 = [pm.pointPosition(v) for v in vertices[0:3]]
-#     p3, p4, p5 = [pm.pointPosition(v) for v in vertices[3:6]]
-
-#     (
-#         dx,
-#         dy,
-#         dz,
-#     ) = (
-#         distance
-#     ) = [  # calculate the translation amount - the first point on each pair is the point to use for translation.
-#         p3[0] - p0[0],
-#         p3[1] - p0[1],
-#         p3[2] - p0[2],
-#     ]
-
-#     pm.move(
-#         dx, dy, dz, objectToMove, relative=1
-#     )  # move the first object by that amount.
-
-#     a1x, a1y, a1z = axis1 = [  # define the two vectors for each pair of points.
-#         p1[0] - p0[0],
-#         p1[1] - p0[1],
-#         p1[2] - p0[2],
-#     ]
-#     a2x, a2y, a2z = axis2 = [p4[0] - p3[0], p4[1] - p3[1], p4[2] - p3[2]]
-
-#     # get the angle (in radians) between the two vectors and the axis of rotation. This is used to move axis1 to match axis2
-#     dp = ptk.dot_product(axis1, axis2, 1)
-#     dp = ptk.clamp(-1.0, 1.0, dp)
-#     angle = math.acos(dp)
-#     cross_product = ptk.cross_product(axis1, axis2, 1, 1)
-
-#     # rotate the first object about the pivot point (the pivot is defined by the first point from the second pair of points. i.e. point 3 from the inputs above)
-#     rotation = ptk.xyz_rotation(angle, cross_product)
-#     pm.rotate(
-#         objectToMove,
-#         str(rotation[0]) + "rad",
-#         str(rotation[1]) + "rad",
-#         str(rotation[2]) + "rad",
-#         pivot=p3,
-#         relative=1,
-#     )
-
-#     # Get these points again since they may have moved
-#     p2 = pm.pointPosition(vertices[2])
-#     p5 = pm.pointPosition(vertices[5])
-
-#     axis3 = [p2[0] - p4[0], p2[1] - p4[1], p2[2] - p4[2]]
-#     axis4 = [p5[0] - p4[0], p5[1] - p4[1], p5[2] - p4[2]]
-
-#     axis2 = ptk.normalize(axis2)
-
-#     # Get the dot product of axis3 on axis2
-#     dp = ptk.dot_product(axis3, axis2, 0)
-#     axis3[0] = p2[0] - p4[0] + dp * axis2[0]
-#     axis3[1] = p2[1] - p4[1] + dp * axis2[1]
-#     axis3[2] = p2[2] - p4[2] + dp * axis2[2]
-
-#     # Get the dot product of axis4 on axis2
-#     dp = ptk.dot_product(axis4, axis2, 0)
-#     axis4[0] = p5[0] - p4[0] + dp * axis2[0]
-#     axis4[1] = p5[1] - p4[1] + dp * axis2[1]
-#     axis4[2] = p5[2] - p4[2] + dp * axis2[2]
-
-#     # rotate the first object again, this time about the 2nd axis so that the 3rd point is in the same plane. ie. match up axis3 with axis4.
-#     dp = ptk.dot_product(axis3, axis4, 1)
-#     dp = ptk.clamp(-1.0, 1.0, dp)
-#     angle = math.acos(dp)
-
-#     # reverse the angle if the cross product is in the -ve axis direction
-#     cross_product = ptk.cross_product(axis3, axis4, 1, 1)
-#     dp = ptk.dot_product(cross_product, axis2, 0)
-#     if dp < 0:
-#         angle = -angle
-
-#     rotation = ptk.xyz_rotation(angle, axis2)
-#     pm.rotate(
-#         objectToMove,
-#         str(rotation[0]) + "rad",
-#         str(rotation[1]) + "rad",
-#         str(rotation[2]) + "rad",
-#         pivot=p4,
-#         relative=1,
-#     )
-
-# @classmethod
-#   def matchTransformByVertexOrder(cls, source, target):
-#       '''Match transform and rotation on like objects by using 3 vertices from each object.
-#       The vertex order is transferred to the target object(s).
-
-#       Parameters:
-#           source (str/obj): The object to move from.
-#           target (str/obj): The object to move to.
-#       '''
-#       pm.polyTransfer(source, alternateObject=target, vertices=2) #vertices positions are copied from the target object.
-
-#       source_verts = [pm.ls(source, objectsOnly=1)[0].verts[i] for i in range(3)]
-#       target_verts = [pm.ls(target, objectsOnly=1)[0].verts[i] for i in range(3)]
-
-#       cls.snap3PointsTo3Points(source_verts+target_verts)
-
-# @staticmethod
-#   def getComponentPoint(component, alignToNormal=False):
-#       '''Get the center point from the given component.
-
-#       Parameters:
-#           component (str/obj): Object component.
-#           alignToNormal (bool): Constain to normal vector.
-
-#       Returns:
-#           (tuple) coordinate as xyz float values.
-#       '''
-#       if ".vtx" in str(component):
-#           x = pm.polyNormalPerVertex(component, q=True, x=1)
-#           y = pm.polyNormalPerVertex(component, q=True, y=1)
-#           z = pm.polyNormalPerVertex(component, q=True, z=1)
-#           xyz = [sum(x) / float(len(x)), sum(y) / float(len(y)), sum(z) / float(len(z))] #get average
-
-#       elif ".e" in str(component):
-#           componentName = str(component).split(".")[0]
-#           vertices = pm.polyInfo (component, edgeToVertex=1)[0]
-#           vertices = vertices.split()
-#           vertices = [componentName+".vtx["+vertices[2]+"]",componentName+".vtx["+vertices[3]+"]"]
-#           x=[];y=[];z=[]
-#           for vertex in vertices:
-#               x_ = pm.polyNormalPerVertex (vertex, q=True, x=1)
-#               x.append(sum(x_) / float(len(x_)))
-#               y_ = pm.polyNormalPerVertex (vertex, q=True, y=1)
-#               x.append(sum(y_) / float(len(y_)))
-#               z_ = pm.polyNormalPerVertex (vertex, q=True, z=1)
-#               x.append(sum(z_) / float(len(z_)))
-#           xyz = [sum(x) / float(len(x)), sum(y) / float(len(y)), sum(z) / float(len(z))] #get average
-
-#       else:# elif ".f" in str(component):
-#           xyz = pm.polyInfo (component, faceNormals=1)
-#           xyz = xyz[0].split()
-#           xyz = [float(xyz[2]), float(xyz[3]), float(xyz[4])]
-
-#       if alignToNormal: #normal constraint
-#           normal = pm.mel.eval("unit <<"+str(xyz[0])+", "+str(xyz[1])+", "+str(xyz[2])+">>;") #normalize value using MEL
-#           # normal = [round(i-min(xyz)/(max(xyz)-min(xyz)),6) for i in xyz] #normalize and round value using python
-
-#           constraint = pm.normalConstraint(component, object_,aimVector=normal,upVector=[0,1,0],worldUpVector=[0,1,0],worldUpType="vector") # "scene","object","objectrotation","vector","none"
-#           pm.delete(constraint) #orient object_ then remove constraint.
-
-#       vertexPoint = pm.xform (component, q=True, translation=1) #average vertex points on destination to get component center.
-#       x = vertexPoint[0::3]
-#       y = vertexPoint[1::3]
-#       z = vertexPoint[2::3]
-
-#       return tuple(round(sum(x) / float(len(x)),4), round(sum(y) / float(len(y)),4), round(sum(z) / float(len(z)),4))
```

### Comparing `mayatk-0.6.8/mayatk.egg-info/PKG-INFO.bak` & `mayatk-0.6.9/mayatk.egg-info/PKG-INFO.bak`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.8/mayatk.egg-info/SOURCES.txt` & `mayatk-0.6.9/mayatk.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,34 @@
 LICENSE
 MANIFEST.in
 setup.py
 mayatk/__init__.py
 mayatk/cam_utils.py
-mayatk/cam_utils.py.bak
 mayatk/cmpt_utils.py
-mayatk/cmpt_utils.py.bak
+mayatk/core_utils.py
 mayatk/edit_utils.py
 mayatk/macro_utils.py
 mayatk/mash_utils.py
-mayatk/mash_utils.py.bak
-mayatk/misc_utils.py.bak
 mayatk/node_utils.py
-mayatk/project_utils.py
-mayatk/project_utils.py.bak
+mayatk/proj_utils.py
 mayatk/rig_utils.py
-mayatk/rig_utils.py.bak
-mayatk/script_utils.py
-mayatk/utils.py
 mayatk/xform_utils.py
-mayatk/xform_utils.py.bak
 mayatk.egg-info/PKG-INFO
 mayatk.egg-info/PKG-INFO.bak
 mayatk.egg-info/SOURCES.txt
 mayatk.egg-info/SOURCES.txt.bak
 mayatk.egg-info/dependency_links.txt
 mayatk.egg-info/top_level.txt
 mayatk/display_utils/__init__.py
 mayatk/display_utils/exploded_view.py
 mayatk/mat_utils/__init__.py
 mayatk/mat_utils/mat_utils.py
 mayatk/mat_utils/stingray_arnold_shader.py
 test/__init__.py
 test/cmpt_utils_test.py
+test/core_utils_test.py
 test/edit_utils_test.py
 test/mat_utils_test.py
 test/node_utils_test.py
 test/rig_utils_test.py
 test/run_tests.py
-test/utils_test.py
 test/xform_utils_test.py
```

### Comparing `mayatk-0.6.8/mayatk.egg-info/SOURCES.txt.bak` & `mayatk-0.6.9/mayatk.egg-info/SOURCES.txt.bak`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.8/setup.py` & `mayatk-0.6.9/setup.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.8/test/__init__.py` & `mayatk-0.6.9/test/__init__.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.8/test/cmpt_utils_test.py` & `mayatk-0.6.9/test/cmpt_utils_test.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.8/test/edit_utils_test.py` & `mayatk-0.6.9/test/edit_utils_test.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.8/test/mat_utils_test.py` & `mayatk-0.6.9/test/mat_utils_test.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.8/test/node_utils_test.py` & `mayatk-0.6.9/test/node_utils_test.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.8/test/rig_utils_test.py` & `mayatk-0.6.9/test/rig_utils_test.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.8/test/run_tests.py` & `mayatk-0.6.9/test/run_tests.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.6.8/test/utils_test.py` & `mayatk-0.6.9/test/core_utils_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 # !/usr/bin/python
 # coding=utf-8
 import os
 import unittest
 import inspect
 import pymel.core as pm
-from mayatk import Utils
-
-
-# sfr = pm.melGlobals['cmdScrollFieldReporter']
-# pm.cmdScrollFieldReporter(sfr, edit=1, clear=1)
+from mayatk import CoreUtils
 
 
 class Main(unittest.TestCase):
     """Main test class."""
 
     def perform_test(self, cases):
         """Execute the test cases."""
@@ -55,15 +51,15 @@
                 "<class 'str'> <PySide2.QtWidgets.QWidget(0x00000000000, name='MayaWindow') at 0x00000000000>"
         """
         import re
 
         return re.sub(r"0x[a-fA-F\d]+", "0x00000000000", str(obj))
 
 
-class Core_test(Main, Utils):
+class CoreUtils_test(Main, CoreUtils):
     """
     set object mode:
             pm.selectMode(object=1)
 
     set component mode:
             pm.selectMode(component=1)
 
@@ -96,15 +92,15 @@
             name="cyl",
         )
 
     def test_undo(self):
         """ """
         self.assertEqual(
             self.replace_mem_address(self.undo()),
-            "<function Utils.undo.<locals>.wrapper at 0x00000000000>",
+            "<function CoreUtils.undo.<locals>.wrapper at 0x00000000000>",
         )
 
     def test_getMainWindow(self):
         """ """
         self.perform_test(
             {
                 "self.replace_mem_address(self.get_main_window())": '<PySide2.QtWidgets.QWidget(0x00000000000, name="MayaWindow") at 0x00000000000>'
```

### Comparing `mayatk-0.6.8/test/xform_utils_test.py` & `mayatk-0.6.9/test/xform_utils_test.py`

 * *Files identical despite different names*

