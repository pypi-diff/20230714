# Comparing `tmp/mcemtools-0.5.0.tar.gz` & `tmp/mcemtools-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcemtools-0.5.0.tar", last modified: Wed Jul 12 04:56:10 2023, max compression
+gzip compressed data, was "mcemtools-0.6.0.tar", last modified: Fri Jul 14 12:18:42 2023, max compression
```

## Comparing `mcemtools-0.5.0.tar` & `mcemtools-0.6.0.tar`

### file list

```diff
@@ -1,43 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:56:10.539544 mcemtools-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-12 04:55:58.000000 mcemtools-0.5.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-07-12 04:55:58.000000 mcemtools-0.5.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-12 04:55:58.000000 mcemtools-0.5.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-12 04:55:58.000000 mcemtools-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-12 04:55:58.000000 mcemtools-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-12 04:56:10.543545 mcemtools-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-12 04:55:58.000000 mcemtools-0.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:56:10.539544 mcemtools-0.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-12 04:55:58.000000 mcemtools-0.5.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-12 04:55:58.000000 mcemtools-0.5.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-07-12 04:55:58.000000 mcemtools-0.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-12 04:55:58.000000 mcemtools-0.5.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-12 04:55:58.000000 mcemtools-0.5.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-12 04:55:58.000000 mcemtools-0.5.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-12 04:55:58.000000 mcemtools-0.5.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-12 04:55:58.000000 mcemtools-0.5.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-12 04:55:58.000000 mcemtools-0.5.0/docs/mcemtools.denoise.rst
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-12 04:55:58.000000 mcemtools-0.5.0/docs/mcemtools.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-12 04:55:58.000000 mcemtools-0.5.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-12 04:55:58.000000 mcemtools-0.5.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:56:10.539544 mcemtools-0.5.0/mcemtools/
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-12 04:55:58.000000 mcemtools-0.5.0/mcemtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-07-12 04:55:58.000000 mcemtools-0.5.0/mcemtools/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-12 04:55:58.000000 mcemtools-0.5.0/mcemtools/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11535 2023-07-12 04:55:58.000000 mcemtools-0.5.0/mcemtools/masking.py
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-07-12 04:55:58.000000 mcemtools-0.5.0/mcemtools/mcemtools.py
--rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-07-12 04:55:58.000000 mcemtools-0.5.0/mcemtools/tensor_svd.py
--rw-r--r--   0 runner    (1001) docker     (123)     8984 2023-07-12 04:55:58.000000 mcemtools-0.5.0/mcemtools/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:56:10.539544 mcemtools-0.5.0/mcemtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-12 04:56:10.000000 mcemtools-0.5.0/mcemtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-12 04:56:10.000000 mcemtools-0.5.0/mcemtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 04:56:10.000000 mcemtools-0.5.0/mcemtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-12 04:56:10.000000 mcemtools-0.5.0/mcemtools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 04:56:10.000000 mcemtools-0.5.0/mcemtools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 04:56:10.000000 mcemtools-0.5.0/mcemtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 04:56:10.000000 mcemtools-0.5.0/mcemtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-12 04:55:58.000000 mcemtools-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-12 04:56:10.543545 mcemtools-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-12 04:55:58.000000 mcemtools-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:56:10.539544 mcemtools-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-12 04:55:58.000000 mcemtools-0.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-12 04:55:58.000000 mcemtools-0.5.0/tests/test_mcemtools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:18:42.402227 mcemtools-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-14 12:18:32.000000 mcemtools-0.6.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-07-14 12:18:32.000000 mcemtools-0.6.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-14 12:18:32.000000 mcemtools-0.6.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-14 12:18:32.000000 mcemtools-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-14 12:18:32.000000 mcemtools-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-07-14 12:18:42.402227 mcemtools-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-14 12:18:32.000000 mcemtools-0.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:18:42.398227 mcemtools-0.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-14 12:18:32.000000 mcemtools-0.6.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-14 12:18:32.000000 mcemtools-0.6.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-07-14 12:18:32.000000 mcemtools-0.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-14 12:18:32.000000 mcemtools-0.6.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-14 12:18:32.000000 mcemtools-0.6.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-14 12:18:32.000000 mcemtools-0.6.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-14 12:18:32.000000 mcemtools-0.6.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-14 12:18:32.000000 mcemtools-0.6.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-14 12:18:32.000000 mcemtools-0.6.0/docs/mcemtools.denoise.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-14 12:18:32.000000 mcemtools-0.6.0/docs/mcemtools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-14 12:18:32.000000 mcemtools-0.6.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-14 12:18:32.000000 mcemtools-0.6.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:18:42.402227 mcemtools-0.6.0/mcemtools/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-14 12:18:32.000000 mcemtools-0.6.0/mcemtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-07-14 12:18:32.000000 mcemtools-0.6.0/mcemtools/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-14 12:18:32.000000 mcemtools-0.6.0/mcemtools/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-07-14 12:18:32.000000 mcemtools-0.6.0/mcemtools/masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-07-14 12:18:32.000000 mcemtools-0.6.0/mcemtools/mcemtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-07-14 12:18:32.000000 mcemtools-0.6.0/mcemtools/tensor_svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-07-14 12:18:32.000000 mcemtools-0.6.0/mcemtools/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:18:42.402227 mcemtools-0.6.0/mcemtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-07-14 12:18:42.000000 mcemtools-0.6.0/mcemtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-14 12:18:42.000000 mcemtools-0.6.0/mcemtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:18:42.000000 mcemtools-0.6.0/mcemtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-14 12:18:42.000000 mcemtools-0.6.0/mcemtools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:18:42.000000 mcemtools-0.6.0/mcemtools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-14 12:18:42.000000 mcemtools-0.6.0/mcemtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-14 12:18:42.000000 mcemtools-0.6.0/mcemtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-14 12:18:32.000000 mcemtools-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-14 12:18:42.402227 mcemtools-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-14 12:18:32.000000 mcemtools-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:18:42.402227 mcemtools-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-14 12:18:32.000000 mcemtools-0.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-14 12:18:32.000000 mcemtools-0.6.0/tests/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-14 12:18:32.000000 mcemtools-0.6.0/tests/test_masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-14 12:18:32.000000 mcemtools-0.6.0/tests/test_mcemtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-14 12:18:32.000000 mcemtools-0.6.0/tests/test_tensor_svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-14 12:18:32.000000 mcemtools-0.6.0/tests/test_transforms.py
```

### Comparing `mcemtools-0.5.0/CONTRIBUTING.rst` & `mcemtools-0.6.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mcemtools-0.5.0/LICENSE` & `mcemtools-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mcemtools-0.5.0/PKG-INFO` & `mcemtools-0.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcemtools
-Version: 0.5.0
+Version: 0.6.0
 Summary: State of the art analysis tools for electron microscopy
 Home-page: https://github.com/arsadri/mcemtools
 Author: Alireza Sadri
 Author-email: Alireza.Sadri@monash.edu
 License: MIT license
 Keywords: mcemtools
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -89,7 +89,12 @@
 ------------------
 
 * Many small bugs are fixed
 
 0.5.0 (2023-07-12)
 ------------------
 * Added binning to transforms
+
+0.6.0 (2023-07-15)
+------------------
+* More tests are added
+* Names are consistant accross the package.
```

### Comparing `mcemtools-0.5.0/README.rst` & `mcemtools-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `mcemtools-0.5.0/docs/Makefile` & `mcemtools-0.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mcemtools-0.5.0/docs/conf.py` & `mcemtools-0.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.5.0/docs/installation.rst` & `mcemtools-0.6.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `mcemtools-0.5.0/docs/make.bat` & `mcemtools-0.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mcemtools-0.5.0/mcemtools/__init__.py` & `mcemtools-0.6.0/mcemtools/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # -*- coding: utf-8 -*-
 
 """Top-level package for mcemtools."""
 
 __author__ = """Alireza Sadri"""
 __email__ = 'Alireza.Sadri@monash.edu'
-__version__ = '0.5.0'
+__version__ = '0.6.0'
+
+from .analysis import pyMSSE, cross_correlation_4D, SymmSTEM
+from .analysis import centre_of_mass_4D, sum_4D
 
-from .analysis import pyMSSE, cross_corr, SymmSTEM, annular_CoM4D, annular4D
 from .masking import annular_mask, image_by_windows, markimage, mask2D_to_4D
+
 from .tensor_svd import svd_fit, svd_eval
-from .transforms import get_polar_coords, polar2image, image2polar, bin4D
-from .transforms import normalize4D
-from .mcemtools import fig2data, locate_atoms, numbers_as_images
+
+from .transforms import get_polar_coords, polar2image, image2polar, bin_4D
+from .transforms import normalize_4D
+
+from .mcemtools import pltfig_to_numpy, locate_atoms, numbers_as_images
```

### Comparing `mcemtools-0.5.0/mcemtools/masking.py` & `mcemtools-0.6.0/mcemtools/masking.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,87 +1,87 @@
 import matplotlib.pyplot as plt
 from matplotlib.widgets import RangeSlider, Slider
-from lognflow import select_file
 import numpy as np
 
 def mask2D_to_4D(mask2D, data4D_shape):
     n_x, n_y, n_r, n_c = data4D_shape
     assert len(mask2D.shape) == 2, 'mask should be 2d'
     assert mask2D.shape[0] == n_r, 'mask should have same shape as patterns'
     assert mask2D.shape[1] == n_c, 'mask should have same shape as patterns'
         
     _mask4D = np.array([np.array([mask2D.copy()])])
     _mask4D = np.tile(_mask4D, (n_x, n_y, 1, 1))
     return _mask4D
 
 def annular_mask(image_shape : tuple, 
-                 center:tuple = None, radius:float=None, in_radius:float=None):
+                 centre:tuple = None, radius:float=None, in_radius:float=None):
     """make a circle bianry pattern in a given window
     This simple function makes a circle filled with ones for where the circle is
     in a window and leaves the rest of the elements to remain zero.
     Parameters
     ----------
         :param image_shape:
             a tuple of the shape of the image
-        :param center: 
+        :param centre: 
             tuple of two float scalars
             Intensity difference threshold.
         :param radius :
             float radius of the circle, if in_radius is None, inside this 
             radius is filledup with 1.
         :param in_radius :
             float radius of the circle inside where it is not masked. If given
             the annular ring between in_radius and radius will be 1.
     Returns
     -------
         : np.ndarray of type uint8
             An image of size h x w where all elements that are closer to the origin
-            of a circle with center at center and radius radius are one and the rest
+            of a circle with centre at centre and radius radius are one and the rest
             are zero. We use equal or greater than for both radius and in_radius.
     """
     n_r, n_c = image_shape
-    if center is None: # use the middle of the image
-        center = (int(n_r/2), int(n_c/2))
-    if radius is None: # use the smallest distance between the center and image walls
-        radius = np.minimum(center[0], center[1])
+    if centre is None: # use the middle of the image
+        centre = (int(n_r/2), int(n_c/2))
+    if radius is None: # use the smallest distance between the centre and image walls
+        radius = np.minimum(centre[0], centre[1])
 
     Y, X = np.ogrid[:n_r, :n_c]
-    dist_from_center = np.sqrt((X - center[0])**2 + (Y-center[1])**2)
+    dist_from_centre = np.sqrt((X - centre[0])**2 + (Y-centre[1])**2)
 
-    mask = dist_from_center <= radius
+    mask = dist_from_centre <= radius
     
     if(in_radius is not None):
-        mask *= in_radius <= dist_from_center
+        mask *= in_radius <= dist_from_centre
 
     return mask.astype('uint8') 
 
 class image_by_windows:
     def __init__(self, 
-                 img_shape: tuple, 
+                 img_shape: tuple[int, int], 
                  win_shape: tuple[int, int] = (2, 2),
-                 skip: tuple[int, int] = (1, 1),
-                 compensate_epochs : bool = False):
+                 skip: tuple[int, int] = (1, 1)):
         """image by windows
+        
+            I am using OOP here because the user pretty much always wants to
+            transform results back to the original shape. It is different
+            from typical transforms, where the processing ends at the other
+            space.
+        
             Parameters
             ----------
             :param img_shape:
                 pass your_data.shape. First two dimensions should be for the
                 image to be cropped.
             :param win_shape:
                 the cropping windows shape
             :param skip:
                 The skipping length of windows
-            :param compensate_epochs:
-                Some pixels will be more visited than others. This is a way of
-                making a balance.
         """
         self.img_shape = img_shape
         self.win_shape = win_shape
         self.skip = skip
-        self.compensate_epochs = compensate_epochs
         n_r, n_c = img_shape[:2]
         rows = np.arange(0, n_r - win_shape[0] + 1, skip[0])
         clms = np.arange(0, n_c - win_shape[1] + 1, skip[1])
         
         if rows[-1] < n_r - win_shape[0]:
             rows = np.concatenate(rows, n_r - win_shape[0])
         if clms[-1] > n_c - win_shape[1]:
@@ -153,17 +153,17 @@
         self.mark_shape = mark_shape
         self.fig, axs = plt.subplots(1, 2, figsize=figsize)
         self.fig.subplots_adjust(bottom=0.4)
         # cm = plt.colormaps["Spectral"]
         self.im = axs[0].imshow(in_image, **kwargs_for_imshow)
         cm = self.im.get_cmap()
         _, bins, patches = axs[1].hist(in_image.flatten(), bins='auto')
-        bin_centers = 0.5 * (bins[:-1] + bins[1:])
+        bin_centres = 0.5 * (bins[:-1] + bins[1:])
         # scale values to interval [0,1]
-        col = bin_centers - min(bin_centers)
+        col = bin_centres - min(bin_centres)
         col /= max(col)
         for c, p in zip(col, patches):
             plt.setp(p, 'facecolor', cm(c))
         axs[1].set_title('Histogram of pixel intensities')
         
         # Create the RangeSlider
         slider_ax = self.fig.add_axes([0.25, 0.25, 0.6, 0.03])
@@ -250,15 +250,15 @@
         self.fig.canvas.draw_idle()
 
     def update2(self, val):
         if(self.mark_shape == 'circle'):
             r = self.slider_r.val
             cx = self.slider_cx.val
             cy  = self.slider_cy.val
-            self.markshape.center = (cy, cx)
+            self.markshape.centre = (cy, cx)
             self.markshape.set_radius(r)
             
         if(self.mark_shape == 'rectangle'):
             self.slider_top_left_r.val
             self.slider_top_left_c.val
             self.slider_bot_right_r.val
             self.slider_s_bot_right_c.val
@@ -267,13 +267,8 @@
                 self.slider_top_left_r.val,
                 self.slider_top_left_c.val)
             self.markshape.set_width(
                 self.slider_bot_right_r.val - self.slider_top_left_r.val)
             self.markshape.set_height(
                 self.slider_s_bot_right_c.val - self.slider_top_left_c.val)
 
-        self.fig.canvas.draw_idle()
-
-if __name__ == '__main__':
-    in_image = np.load(select_file())
-    markimage(in_image, 'circle', cmap = 'jet')
-    # markimage(in_image, 'rectangle', cmap = 'gray')
+        self.fig.canvas.draw_idle()
```

### Comparing `mcemtools-0.5.0/mcemtools/mcemtools.py` & `mcemtools-0.6.0/mcemtools/mcemtools.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from .masking import annular_mask, mask2D_to_4D
+import matplotlib.pyplot as plt
 from lognflow import printprogress
 
 def locate_atoms(data4D, min_distance = 3, filter_size = 3,
                  reject_too_close = False):
     from skimage.feature import peak_local_max
     import scipy.ndimage
     _, _, n_r, n_c = data4D.shape
@@ -22,33 +22,33 @@
                          & (coordinates[:, 0] < n_r - dist2_threshold)
                          & (dist2_threshold < coordinates[:, 1])
                          & (coordinates[:, 1] < n_c - dist2_threshold)  )[0]
         
         coordinates = coordinates[inds]
     return coordinates
 
-def fig2data(fig):
+def pltfig_to_numpy(fig):
     """ from https://www.icare.univ-lille.fr/how-to-
                     convert-a-matplotlib-figure-to-a-numpy-array-or-a-pil-image/
     """
     fig.canvas.draw()
     w,h = fig.canvas.get_width_height()
     buf = np.frombuffer(fig.canvas.tostring_argb(), dtype=np.ubyte)
     buf.shape = (w, h, 4)
     buf = np.roll (buf, 3, axis = 2)
     return buf
 
 def numbers_as_images(dataset_shape, fontsize, verbose = False):
     """ Numbers4D
-    This scripts generates a 4D dataset of images with shape
+    This function generates a 4D dataset of images with shape
     (n_x, n_y, n_r, n_c) where in each image the value "x, y" is written as a text
-    that fills the image. As such later when working with such a dataset you can
-    look at the image and know which index it had before you using it.
+    that fills the image. As such, later when working with such a dataset you can
+    look at the image and know which index it had before you use it.
     
-    Follow this receip to make good images:
+    Follow this recipe to make good images:
     
     1- set n_x, n_y to 10, Set the desired n_r and width. 
     2- try fontsize that is the largest
     3- Increase n_x and n_y to desired siez.
     
     You can provide a logs_root, log_dir or simply select a directory to save the
     output 4D array.
@@ -69,15 +69,15 @@
                                                   width = txt_width)
             fig = plt.figure(figsize = (1, 1))
             ax = fig.add_subplot(111)
             ax.imshow(mat, cmap = 'gray', vmin = 0, vmax = 1)
             ax.text(mat.shape[0]//2 - fontsize, mat.shape[1]//2 ,
                     number_text, fontsize = fontsize)
             ax.axis('off')
-            buf = fig2data (fig)
+            buf = pltfig_to_numpy(fig)
             plt.close()
             buf2 = buf[::buf.shape[0]//n_r, ::buf.shape[1]//n_c, :3].mean(2)
             buf2 = buf2[:n_r, :n_c]
             dataset[ind_x, ind_y] = buf2.copy()
             if(verbose):
                 pBar()
     return dataset
```

### Comparing `mcemtools-0.5.0/mcemtools/tensor_svd.py` & `mcemtools-0.6.0/mcemtools/tensor_svd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+This code is modified from Tensor SVD repo for mcemtools
+ 
+"""
+
 import numpy as np
 from sklearn.utils.extmath import randomized_svd
 
 def tensor_svd_denoise(data, rank):
     """ Wrapper to pre-process STEM data for tensor SVD denoise
 
     Parameters
@@ -81,29 +86,31 @@
     ordered_indexes = np.argsort(data_shape) # getting the indicies from min len to max, initialization starts from smallest size
 
     ## Initialize U and Y with SVD
     U = [None] * dimensions # Generate an empty array to save all the U matrices with fixed length
     X = data
     for k in ordered_indexes: # calculating initial SVD
         unfolded = unfold_axis(X, k) # unfolding from the axis with minimum size
-        [U[k], _ , _] = randomized_svd(unfolded,rank[k],n_iter=svd_iter)
+        [U[k], _ , _] = randomized_svd(unfolded,rank[k],n_iter=svd_iter,
+                                       random_state = None)
         X = ttm(X, np.transpose(U[k]), k) # This needs to be fixed!
 
     ## Update U with HOOI
     iter_count = 0
     while iter_count < max_iter:
         iter_count += 1
         for k in range(0, dimensions):
             Y = data
             minus_k = list(range(0,dimensions))
             minus_k.remove(k)  # every value except for k, seems do it in one step will remove all the elements in the list.
             for j in minus_k:
                 Y = ttm(Y, np.transpose(U[j]), j)
             MY = unfold_axis(Y, k)
-            [U[k], _, _] = randomized_svd(MY, rank[k],n_iter=svd_iter)
+            [U[k], _, _] = randomized_svd(MY, rank[k],n_iter=svd_iter,
+                                          random_state = None)
 
     ## Use the determined U matrices to calculate core tensor and denoised tensor
     X = data
     for k in ordered_indexes:
         X = ttm(X,np.transpose(U[k]), k)  # Check this part.
     S = X   # core tensor
     for k in range(0,dimensions):
@@ -157,29 +164,31 @@
     # initialization starts from smallest size
 
     ## Initialize U and Y with SVD
     U = [None] * dimensions # Generate an empty array to save all the U matrices with fixed length
     X = data
     for k in ordered_indexes: # calculating initial SVD
         unfolded = unfold_axis(X, k) # unfolding from the axis with minimum size
-        [U[k], _ , _] = randomized_svd(unfolded,rank[k],n_iter=svd_iter)
+        [U[k], _ , _] = randomized_svd(unfolded,rank[k],n_iter=svd_iter,
+                                       random_state = None)
         X = ttm(X, np.transpose(U[k]), k) # This needs to be fixed!
 
     ## Update U with HOOI
     iter_count = 0
     while iter_count < max_iter:
         iter_count += 1
         for k in range(0, dimensions):
             Y = data
             minus_k = list(range(0,dimensions))
             minus_k.remove(k)  # every value except for k, seems do it in one step will remove all the elements in the list.
             for j in minus_k:
                 Y = ttm(Y, np.transpose(U[j]), j)
             MY = unfold_axis(Y, k)
-            [U[k], _, _] = randomized_svd(MY, rank[k],n_iter=svd_iter)
+            [U[k], _, _] = randomized_svd(MY, rank[k],n_iter=svd_iter,
+                                          random_state = None)
 
     return U, ordered_indexes
 
 def svd_eval(data, U, ordered_indexes):
     dimensions = len(data.shape)
     # ordered_indexes = np.argsort(data.shape)
     X = data.copy()
@@ -286,13 +295,15 @@
         for i in range(total_dim):
             if ndim[i] > t.shape[i]:
                 ndim[i] = t.shape[i]
     
     scree = []
     for i in range(total_dim):
         t_unfold = unfold_axis(t, i)
-        [ _, e, _ ] = randomized_svd(np.matmul(t_unfold,np.transpose(t_unfold)),ndim[i],n_iter=15)
+        [ _, e, _ ] = randomized_svd(
+            np.matmul(t_unfold,np.transpose(t_unfold)),ndim[i],n_iter=15,
+            random_state = None)
         e = np.sqrt(e)
         e = np.real(e)
         scree.append(e)
 
     return scree
```

### Comparing `mcemtools-0.5.0/mcemtools.egg-info/PKG-INFO` & `mcemtools-0.6.0/mcemtools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcemtools
-Version: 0.5.0
+Version: 0.6.0
 Summary: State of the art analysis tools for electron microscopy
 Home-page: https://github.com/arsadri/mcemtools
 Author: Alireza Sadri
 Author-email: Alireza.Sadri@monash.edu
 License: MIT license
 Keywords: mcemtools
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -89,7 +89,12 @@
 ------------------
 
 * Many small bugs are fixed
 
 0.5.0 (2023-07-12)
 ------------------
 * Added binning to transforms
+
+0.6.0 (2023-07-15)
+------------------
+* More tests are added
+* Names are consistant accross the package.
```

### Comparing `mcemtools-0.5.0/setup.py` & `mcemtools-0.6.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 #!/usr/bin/env python
 
-__version__ = '0.5.0'
+__version__ = '0.6.0'
 
 """The setup script."""
 
 from setuptools import setup, find_packages
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
-requirements = ['numpy']
+requirements = ['numpy', 'matplotlib', 'scipy', 
+                'scikit-learn', 'scikit-image',
+                'lognflow', 'RobustGaussianFittingLibrary']
 
 test_requirements = ['pytest>=3', ]
 
 setup(
     author="Alireza Sadri",
     author_email='Alireza.Sadri@monash.edu',
     python_requires='>=3.7',
@@ -44,10 +46,10 @@
     include_package_data=True,
     keywords='mcemtools',
     name='mcemtools',
     packages=find_packages(include=['mcemtools', 'mcemtools.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/arsadri/mcemtools',
-    version=__version__,
+    version = __version__,
     zip_safe=False,
-)
+)
```

