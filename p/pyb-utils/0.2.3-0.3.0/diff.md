# Comparing `tmp/pyb_utils-0.2.3.tar.gz` & `tmp/pyb_utils-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyb_utils-0.2.3.tar", max compression
+gzip compressed data, was "pyb_utils-0.3.0.tar", max compression
```

## Comparing `pyb_utils-0.2.3.tar` & `pyb_utils-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0     1077 2023-03-01 18:44:35.352445 pyb_utils-0.2.3/LICENSE
--rw-r--r--   0        0        0     1956 2023-04-11 22:45:04.986417 pyb_utils-0.2.3/README.md
--rw-r--r--   0        0        0        0 2023-03-01 18:44:35.352445 pyb_utils-0.2.3/pyb_utils/__init__.py
--rw-r--r--   0        0        0     8332 2023-03-01 18:44:35.352445 pyb_utils-0.2.3/pyb_utils/camera.py
--rw-r--r--   0        0        0     4587 2023-03-01 18:44:35.356445 pyb_utils-0.2.3/pyb_utils/collision.py
--rw-r--r--   0        0        0     1425 2023-03-01 18:44:35.356445 pyb_utils-0.2.3/pyb_utils/frame.py
--rw-r--r--   0        0        0     4588 2023-03-01 18:44:35.356445 pyb_utils-0.2.3/pyb_utils/ghost.py
--rw-r--r--   0        0        0      729 2023-03-01 18:44:35.356445 pyb_utils-0.2.3/pyb_utils/math.py
--rw-r--r--   0        0        0      881 2023-03-01 18:44:35.356445 pyb_utils-0.2.3/pyb_utils/robots.py
--rw-r--r--   0        0        0      598 2023-04-11 22:46:45.778095 pyb_utils-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2854 1970-01-01 00:00:00.000000 pyb_utils-0.2.3/setup.py
--rw-r--r--   0        0        0     2815 1970-01-01 00:00:00.000000 pyb_utils-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-03-01 18:44:35.352445 pyb_utils-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4155 2023-07-14 19:56:54.274466 pyb_utils-0.3.0/README.md
+-rw-r--r--   0        0        0      483 2023-07-14 19:47:26.213579 pyb_utils-0.3.0/pyb_utils/__init__.py
+-rw-r--r--   0        0        0     8890 2023-07-14 19:47:26.213579 pyb_utils-0.3.0/pyb_utils/bodies.py
+-rw-r--r--   0        0        0     8332 2023-03-01 18:44:35.352445 pyb_utils-0.3.0/pyb_utils/camera.py
+-rw-r--r--   0        0        0     4587 2023-03-01 18:44:35.356445 pyb_utils-0.3.0/pyb_utils/collision.py
+-rw-r--r--   0        0        0     1417 2023-07-14 19:47:26.213579 pyb_utils-0.3.0/pyb_utils/frame.py
+-rw-r--r--   0        0        0     4742 2023-07-14 19:47:26.213579 pyb_utils-0.3.0/pyb_utils/ghost.py
+-rw-r--r--   0        0        0      729 2023-03-01 18:44:35.356445 pyb_utils-0.3.0/pyb_utils/math.py
+-rw-r--r--   0        0        0     2430 2023-07-14 19:47:26.213579 pyb_utils-0.3.0/pyb_utils/named_tuples.py
+-rw-r--r--   0        0        0      881 2023-03-01 18:44:35.356445 pyb_utils-0.3.0/pyb_utils/robots.py
+-rw-r--r--   0        0        0      598 2023-07-14 19:47:58.273625 pyb_utils-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5130 1970-01-01 00:00:00.000000 pyb_utils-0.3.0/setup.py
+-rw-r--r--   0        0        0     5014 1970-01-01 00:00:00.000000 pyb_utils-0.3.0/PKG-INFO
```

### Comparing `pyb_utils-0.2.3/LICENSE` & `pyb_utils-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyb_utils-0.2.3/pyb_utils/camera.py` & `pyb_utils-0.3.0/pyb_utils/camera.py`

 * *Files identical despite different names*

### Comparing `pyb_utils-0.2.3/pyb_utils/collision.py` & `pyb_utils-0.3.0/pyb_utils/collision.py`

 * *Files identical despite different names*

### Comparing `pyb_utils-0.2.3/pyb_utils/frame.py` & `pyb_utils-0.3.0/pyb_utils/frame.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pybullet as pyb
-from pyb_utils.math import quaternion_rotate
+
+from .math import quaternion_rotate
 
 
 def debug_frame_world(size, origin, orientation=(0, 0, 0, 1), line_width=1):
     """Attach a frame to the world for debugging purposes."""
     dx = quaternion_rotate(orientation, [size, 0, 0])
     dy = quaternion_rotate(orientation, [0, size, 0])
     dz = quaternion_rotate(orientation, [0, 0, size])
```

### Comparing `pyb_utils-0.2.3/pyb_utils/ghost.py` & `pyb_utils-0.3.0/pyb_utils/ghost.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import pybullet as pyb
 
-from pyb_utils.math import quaternion_rotate, quaternion_multiply
+from .math import quaternion_rotate, quaternion_multiply
 
 
 class GhostObject:
     """A purely visual PyBullet object.
 
     The GhostObject can be "attached" to another body and positioned relative
     to that body, or it can be positioned at an absolute location in the world
@@ -52,14 +52,36 @@
         self.uid = pyb.createMultiBody(
             baseMass=0,  # non-dynamic body has mass = 0
             baseVisualShapeIndex=visual_uid,
             basePosition=list(world_position),
             baseOrientation=list(world_orientation),
         )
 
+    @classmethod
+    def sphere(
+        cls,
+        radius,
+        position=None,
+        parent_body_uid=None,
+        parent_link_index=-1,
+        color=(1, 0, 0, 0),
+    ):
+        """Spherical ghost object."""
+        visual_uid = pyb.createVisualShape(
+            shapeType=pyb.GEOM_SPHERE,
+            radius=radius,
+            rgbaColor=color,
+        )
+        return cls(
+            visual_uid,
+            position=position,
+            parent_body_uid=parent_body_uid,
+            parent_link_index=parent_link_index,
+        )
+
     def _compute_world_position(self):
         # If the object is attached to a parent, then its position and
         # orientation are relative to the parent
         if self.parent_body_uid is not None:
             state = pyb.getLinkState(
                 self.parent_body_uid,
                 self.parent_link_index,
@@ -100,29 +122,12 @@
         world_position, world_orientation = self._compute_world_position()
 
         pyb.resetBasePositionAndOrientation(
             self.uid, list(world_position), list(world_orientation)
         )
 
 
-class GhostSphere(GhostObject):
-    """Spherical ghost object."""
+def GhostSphere(*args, **kwargs):
+    import logging
 
-    def __init__(
-        self,
-        radius,
-        position=None,
-        parent_body_uid=None,
-        parent_link_index=-1,
-        color=(1, 0, 0, 0),
-    ):
-        visual_uid = pyb.createVisualShape(
-            shapeType=pyb.GEOM_SPHERE,
-            radius=radius,
-            rgbaColor=color,
-        )
-        super().__init__(
-            visual_uid,
-            position=position,
-            parent_body_uid=parent_body_uid,
-            parent_link_index=parent_link_index,
-        )
+    logging.warning("GhostSphere is deprecated. Use GhostObject.sphere instead.")
+    return GhostObject.sphere(*args, **kwargs)
```

### Comparing `pyb_utils-0.2.3/pyb_utils/math.py` & `pyb_utils-0.3.0/pyb_utils/math.py`

 * *Files identical despite different names*

### Comparing `pyb_utils-0.2.3/pyb_utils/robots.py` & `pyb_utils-0.3.0/pyb_utils/robots.py`

 * *Files identical despite different names*

### Comparing `pyb_utils-0.2.3/pyproject.toml` & `pyb_utils-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.black]
 line-length = 80
 
 [tool.poetry]
 name = "pyb_utils"
-version = "0.2.3"
+version = "0.3.0"
 description = "Basic utilities for PyBullet, including collision detection, ghost (i.e. visual-only) objects, and cameras."
 authors = ["Adam Heins <mail@adamheins.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.11"
```

