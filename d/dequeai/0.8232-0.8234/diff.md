# Comparing `tmp/dequeai-0.8232.tar.gz` & `tmp/dequeai-0.8234.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.8232.tar", last modified: Thu Jul 13 19:30:37 2023, max compression
+gzip compressed data, was "dequeai-0.8234.tar", last modified: Thu Jul 13 23:24:49 2023, max compression
```

## Comparing `dequeai-0.8232.tar` & `dequeai-0.8234.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 19:30:37.743265 dequeai-0.8232/
--rw-r--r--   0 root         (0) root         (0)      341 2023-07-13 19:30:37.743265 dequeai-0.8232/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 19:30:37.743265 dequeai-0.8232/dequeai/
--rw-r--r--   0 root         (0) root         (0)      441 2023-07-10 20:40:27.000000 dequeai-0.8232/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17283 2023-07-13 19:30:08.000000 dequeai-0.8232/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.8232/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.8232/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)     1523 2023-07-10 18:20:31.000000 dequeai-0.8232/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    15109 2023-07-10 23:35:46.000000 dequeai-0.8232/dequeai/dequeai_model.py
--rw-r--r--   0 root         (0) root         (0)    32599 2023-07-10 17:50:20.000000 dequeai-0.8232/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.8232/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.8232/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.8232/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2535 2023-06-22 19:21:57.000000 dequeai-0.8232/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 19:30:37.743265 dequeai-0.8232/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      341 2023-07-13 19:30:37.000000 dequeai-0.8232/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      416 2023-07-13 19:30:37.000000 dequeai-0.8232/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 19:30:37.000000 dequeai-0.8232/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-07-13 19:30:37.000000 dequeai-0.8232/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-13 19:30:37.000000 dequeai-0.8232/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 19:30:37.743265 dequeai-0.8232/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      515 2023-07-13 19:30:25.000000 dequeai-0.8232/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 23:24:49.937574 dequeai-0.8234/
+-rw-r--r--   0 root         (0) root         (0)      341 2023-07-13 23:24:49.937574 dequeai-0.8234/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 23:24:49.937574 dequeai-0.8234/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      441 2023-07-10 20:40:27.000000 dequeai-0.8234/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19427 2023-07-13 23:24:25.000000 dequeai-0.8234/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.8234/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.8234/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)     1523 2023-07-10 18:20:31.000000 dequeai-0.8234/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    15109 2023-07-10 23:35:46.000000 dequeai-0.8234/dequeai/dequeai_model.py
+-rw-r--r--   0 root         (0) root         (0)    32599 2023-07-10 17:50:20.000000 dequeai-0.8234/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.8234/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.8234/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.8234/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2535 2023-06-22 19:21:57.000000 dequeai-0.8234/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 23:24:49.937574 dequeai-0.8234/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      341 2023-07-13 23:24:49.000000 dequeai-0.8234/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      416 2023-07-13 23:24:49.000000 dequeai-0.8234/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 23:24:49.000000 dequeai-0.8234/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-07-13 23:24:49.000000 dequeai-0.8234/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-13 23:24:49.000000 dequeai-0.8234/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 23:24:49.937574 dequeai-0.8234/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      515 2023-07-13 23:24:36.000000 dequeai-0.8234/setup.py
```

### Comparing `dequeai-0.8232/dequeai/datatypes.py` & `dequeai-0.8234/dequeai/datatypes.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import json
 import time
 import dequeai.util as util
 import numpy as np
 from dequeai.util import DEQUE_IMAGE, DEQUE_HISTOGRAM, DEQUE_AUDIO, DEQUE_TEXT, DEQUE_TABLE, DEQUE_VIDEO, \
     DEQUE_BOUNDING_BOX, DEQUE_PLOT
 from dequeai.util import *
-
+import warnings
 
 # import altair
 
 
 class BoundingBox2D():
     _type = DEQUE_BOUNDING_BOX
 
@@ -28,16 +28,61 @@
     def _validate(self):
         pass
 
     def to_json(self):
         return {"coordinates": self.coordinates, "domain": self.domain, "scores": self
             .scores, "caption": self.caption}
 
-
 class Image:
+
+    _type = DEQUE_IMAGE
+
+    def __init__(self, data, box_data=None):
+        # If the input is a dictionary, extract the image data
+        if isinstance(data, dict):
+            data = list(data.values())
+
+        # If the input is not already a list, make it into a list
+        if not isinstance(data, list):
+            data = [data]
+
+        self.data = []
+
+        for img in data:
+            if isinstance(img, np.ndarray):
+                if len(img.shape) == 2:  # Grayscale image, no batch
+                    self.data.append(img)
+                elif len(img.shape) == 3:  # Could be RGB image or batch of grayscale images
+                    if img.shape[-1] == 3:  # Likely RGB
+                        self.data.append(img)
+                    elif img.shape[0] <= 3:  # Likely RGB but with width/height of 3
+                        self.data.append(np.transpose(img, (1, 2, 0)))  # Transpose to common format
+                        warnings.warn('Input is 3D and has a size of 3 in the first dimension. Assuming it is an RGB image with height and width of 3.')
+                    else:  # Likely batch of grayscale
+                        self.data.extend([i for i in img])
+                elif len(img.shape) == 4:  # Likely batch of RGB images
+                    if img.shape[1] == 3:  # Format is (batch, channel, height, width)
+                        img = np.transpose(img, (0, 2, 3, 1))  # Transpose to (batch, height, width, channel)
+                    self.data.extend([i for i in img])
+                else:
+                    raise ValueError(f'Unsupported image data shape {img.shape}')
+
+            else:
+                torch_module = util.get_module(
+                    "torch", "torch is required to render images"
+                )
+                if isinstance(img, torch_module.Tensor):
+                    # Convert the tensor to a numpy array and recursively call the function
+                    self.__init__(img.numpy(), box_data=box_data)
+                return
+            #TODO: Add default exception for other types of images
+
+        self.box_data = box_data
+
+class Image_Old:
     _type = DEQUE_IMAGE
 
     def __init__(self, data, box_data=None, mode=None):
         self._images = []
         self._box_data = []
 
         if isinstance(data, list):
```

### Comparing `dequeai-0.8232/dequeai/dequeai.py` & `dequeai-0.8234/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.8232/dequeai/dequeai_model.py` & `dequeai-0.8234/dequeai/dequeai_model.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.8232/dequeai/dequeai_run.py` & `dequeai-0.8234/dequeai/dequeai_run.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.8232/dequeai/parsing_service.py` & `dequeai-0.8234/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.8232/dequeai/rest_connect.py` & `dequeai-0.8234/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.8232/dequeai/util.py` & `dequeai-0.8234/dequeai/util.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.8232/setup.py` & `dequeai-0.8234/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, Extension
 
 
 setup(
     name='dequeai',
-    version='0.000008232',
+    version='0.000008234',
     description='Python Package for DEQUE AI Platform',
     author="The DEQUE AI Team",
     author_email='team@deque.app',
     packages=["dequeai"],
     url='https://dequeapp-deque.gitbook.io/deque-docs/getting-started/dequeai-experiment-tracking',
     keywords='dequeai client for deep learning',
     install_requires=[
```

