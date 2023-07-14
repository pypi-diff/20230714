# Comparing `tmp/dequeai-0.8238.tar.gz` & `tmp/dequeai-0.8240.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.8238.tar", last modified: Thu Jul 13 23:38:22 2023, max compression
+gzip compressed data, was "dequeai-0.8240.tar", last modified: Fri Jul 14 00:17:55 2023, max compression
```

## Comparing `dequeai-0.8238.tar` & `dequeai-0.8240.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 23:38:22.098832 dequeai-0.8238/
--rw-r--r--   0 root         (0) root         (0)      341 2023-07-13 23:38:22.098832 dequeai-0.8238/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 23:38:22.098832 dequeai-0.8238/dequeai/
--rw-r--r--   0 root         (0) root         (0)      441 2023-07-10 20:40:27.000000 dequeai-0.8238/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19225 2023-07-13 23:37:20.000000 dequeai-0.8238/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.8238/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.8238/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)     1523 2023-07-10 18:20:31.000000 dequeai-0.8238/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    15109 2023-07-10 23:35:46.000000 dequeai-0.8238/dequeai/dequeai_model.py
--rw-r--r--   0 root         (0) root         (0)    32599 2023-07-10 17:50:20.000000 dequeai-0.8238/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.8238/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.8238/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.8238/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2535 2023-06-22 19:21:57.000000 dequeai-0.8238/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 23:38:22.098832 dequeai-0.8238/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      341 2023-07-13 23:38:21.000000 dequeai-0.8238/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      416 2023-07-13 23:38:22.000000 dequeai-0.8238/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 23:38:21.000000 dequeai-0.8238/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-07-13 23:38:21.000000 dequeai-0.8238/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-13 23:38:22.000000 dequeai-0.8238/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 23:38:22.098832 dequeai-0.8238/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      515 2023-07-13 23:38:08.000000 dequeai-0.8238/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:17:55.169028 dequeai-0.8240/
+-rw-r--r--   0 root         (0) root         (0)      341 2023-07-14 00:17:55.169028 dequeai-0.8240/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:17:55.169028 dequeai-0.8240/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      441 2023-07-10 20:40:27.000000 dequeai-0.8240/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19892 2023-07-14 00:16:25.000000 dequeai-0.8240/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.8240/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.8240/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)     1523 2023-07-10 18:20:31.000000 dequeai-0.8240/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    15109 2023-07-10 23:35:46.000000 dequeai-0.8240/dequeai/dequeai_model.py
+-rw-r--r--   0 root         (0) root         (0)    32599 2023-07-10 17:50:20.000000 dequeai-0.8240/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.8240/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.8240/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.8240/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2535 2023-06-22 19:21:57.000000 dequeai-0.8240/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:17:55.169028 dequeai-0.8240/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      341 2023-07-14 00:17:54.000000 dequeai-0.8240/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      416 2023-07-14 00:17:55.000000 dequeai-0.8240/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 00:17:54.000000 dequeai-0.8240/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-07-14 00:17:55.000000 dequeai-0.8240/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-14 00:17:55.000000 dequeai-0.8240/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 00:17:55.169028 dequeai-0.8240/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      515 2023-07-14 00:17:39.000000 dequeai-0.8240/setup.py
```

### Comparing `dequeai-0.8238/dequeai/datatypes.py` & `dequeai-0.8240/dequeai/datatypes.py`

 * *Files 7% similar despite different names*

```diff
@@ -58,14 +58,17 @@
                 self.process_numpy_img(img.numpy())
             else:
                 raise ValueError(f'Unsupported image data type {type(img)}')
 
         self._box_data = box_data
 
     def process_numpy_img(self, img):
+
+        img = self.to_uint8(img)
+
         if len(img.shape) == 2:  # Grayscale image, no batch
             self._images.append(img)
         elif len(img.shape) == 3:  # Could be RGB image or batch of grayscale images
             if img.shape[-1] == 3:  # Likely RGB
                 self._images.append(img)
             elif img.shape[0] <= 3:  # Likely RGB but with width/height of 3
                 self._images.append(np.transpose(img, (1, 2, 0)))  # Transpose to common format
@@ -75,14 +78,33 @@
         elif len(img.shape) == 4:  # Likely batch of RGB images
             if img.shape[1] == 3:  # Format is (batch, channel, height, width)
                 img = np.transpose(img, (0, 2, 3, 1))  # Transpose to (batch, height, width, channel)
             self._images.extend([i for i in img])
         else:
             raise ValueError(f'Unsupported image data shape {img.shape}')
 
+    @staticmethod
+    def to_uint8(data: "np.ndarray") -> "np.ndarray":
+        """
+        Converts floating point image on the range [0,1] and integer images
+        on the range [0,255] to uint8, clipping if necessary.
+        """
+        np = util.get_module(
+            "numpy",
+            required="Deque.Image requires numpy if not supplying PIL Images: pip install numpy",
+        )
+
+        dmin = np.min(data)
+        if dmin < 0:
+            data = (data - np.min(data)) / np.ptp(data)
+        if np.max(data) <= 1.0:
+            data = (data * 255).astype(np.int32)
+
+        return data.clip(0, 255).astype(np.uint8)
+
 
 class Image_Old:
     _type = DEQUE_IMAGE
 
     def __init__(self, data, box_data=None, mode=None):
         self._images = []
         self._box_data = []
```

### Comparing `dequeai-0.8238/dequeai/dequeai.py` & `dequeai-0.8240/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.8238/dequeai/dequeai_model.py` & `dequeai-0.8240/dequeai/dequeai_model.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.8238/dequeai/dequeai_run.py` & `dequeai-0.8240/dequeai/dequeai_run.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.8238/dequeai/parsing_service.py` & `dequeai-0.8240/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.8238/dequeai/rest_connect.py` & `dequeai-0.8240/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.8238/dequeai/util.py` & `dequeai-0.8240/dequeai/util.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.8238/setup.py` & `dequeai-0.8240/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, Extension
 
 
 setup(
     name='dequeai',
-    version='0.000008238',
+    version='0.000008240',
     description='Python Package for DEQUE AI Platform',
     author="The DEQUE AI Team",
     author_email='team@deque.app',
     packages=["dequeai"],
     url='https://dequeapp-deque.gitbook.io/deque-docs/getting-started/dequeai-experiment-tracking',
     keywords='dequeai client for deep learning',
     install_requires=[
```

