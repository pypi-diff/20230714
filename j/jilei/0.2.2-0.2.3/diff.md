# Comparing `tmp/jilei-0.2.2.tar.gz` & `tmp/jilei-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\jilei-0.2.2.tar", last modified: Fri Jul 14 07:26:53 2023, max compression
+gzip compressed data, was "dist\jilei-0.2.3.tar", last modified: Fri Jul 14 07:50:55 2023, max compression
```

## Comparing `jilei-0.2.2.tar` & `jilei-0.2.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 07:26:53.428734 jilei-0.2.2/
--rw-rw-rw-   0        0        0      448 2023-07-14 07:26:53.428734 jilei-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      369 2023-05-07 08:49:40.000000 jilei-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 07:26:53.421728 jilei-0.2.2/jilei/
--rw-rw-rw-   0        0        0        0 2023-04-12 11:09:36.000000 jilei-0.2.2/jilei/__init__.py
--rw-rw-rw-   0        0        0     3229 2023-07-14 04:55:57.000000 jilei-0.2.2/jilei/dicom.py
--rw-rw-rw-   0        0        0     2666 2023-05-07 09:36:18.000000 jilei-0.2.2/jilei/docker_tools.py
--rw-rw-rw-   0        0        0     1521 2023-06-07 09:04:28.000000 jilei-0.2.2/jilei/mapping_3d_to_2d.py
--rw-rw-rw-   0        0        0     7409 2023-05-26 10:47:48.000000 jilei-0.2.2/jilei/medical_image_tools.py
--rw-rw-rw-   0        0        0     4446 2023-07-13 16:35:27.000000 jilei-0.2.2/jilei/mimics.py
--rw-rw-rw-   0        0        0    17057 2023-07-14 07:26:34.000000 jilei-0.2.2/jilei/mimics_qt.py
--rw-rw-rw-   0        0        0     1006 2023-04-20 06:23:16.000000 jilei-0.2.2/jilei/nnunet_tools.py
--rw-rw-rw-   0        0        0      640 2023-07-13 04:01:00.000000 jilei-0.2.2/jilei/qt.py
--rw-rw-rw-   0        0        0     1210 2023-05-07 09:28:34.000000 jilei-0.2.2/jilei/system_tools.py
--rw-rw-rw-   0        0        0     1744 2023-04-12 12:32:48.000000 jilei-0.2.2/jilei/wxwork.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:26:53.427733 jilei-0.2.2/jilei.egg-info/
--rw-rw-rw-   0        0        0      448 2023-07-14 07:26:53.000000 jilei-0.2.2/jilei.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2023-07-14 07:26:53.000000 jilei-0.2.2/jilei.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 07:26:53.000000 jilei-0.2.2/jilei.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-14 07:26:53.000000 jilei-0.2.2/jilei.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 07:26:53.428734 jilei-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      523 2023-07-14 07:26:53.000000 jilei-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:50:55.566428 jilei-0.2.3/
+-rw-rw-rw-   0        0        0      448 2023-07-14 07:50:55.566428 jilei-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2023-05-07 08:49:40.000000 jilei-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 07:50:55.556419 jilei-0.2.3/jilei/
+-rw-rw-rw-   0        0        0        0 2023-04-12 11:09:36.000000 jilei-0.2.3/jilei/__init__.py
+-rw-rw-rw-   0        0        0     3229 2023-07-14 04:55:57.000000 jilei-0.2.3/jilei/dicom.py
+-rw-rw-rw-   0        0        0     2666 2023-05-07 09:36:18.000000 jilei-0.2.3/jilei/docker_tools.py
+-rw-rw-rw-   0        0        0     1521 2023-06-07 09:04:28.000000 jilei-0.2.3/jilei/mapping_3d_to_2d.py
+-rw-rw-rw-   0        0        0     7409 2023-05-26 10:47:48.000000 jilei-0.2.3/jilei/medical_image_tools.py
+-rw-rw-rw-   0        0        0     4446 2023-07-13 16:35:27.000000 jilei-0.2.3/jilei/mimics.py
+-rw-rw-rw-   0        0        0    16996 2023-07-14 07:49:34.000000 jilei-0.2.3/jilei/mimics_qt.py
+-rw-rw-rw-   0        0        0     1006 2023-04-20 06:23:16.000000 jilei-0.2.3/jilei/nnunet_tools.py
+-rw-rw-rw-   0        0        0      640 2023-07-13 04:01:00.000000 jilei-0.2.3/jilei/qt.py
+-rw-rw-rw-   0        0        0     1210 2023-05-07 09:28:34.000000 jilei-0.2.3/jilei/system_tools.py
+-rw-rw-rw-   0        0        0     1744 2023-04-12 12:32:48.000000 jilei-0.2.3/jilei/wxwork.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:50:55.565426 jilei-0.2.3/jilei.egg-info/
+-rw-rw-rw-   0        0        0      448 2023-07-14 07:50:55.000000 jilei-0.2.3/jilei.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2023-07-14 07:50:55.000000 jilei-0.2.3/jilei.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 07:50:55.000000 jilei-0.2.3/jilei.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-14 07:50:55.000000 jilei-0.2.3/jilei.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 07:50:55.566428 jilei-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      523 2023-07-14 07:50:55.000000 jilei-0.2.3/setup.py
```

### Comparing `jilei-0.2.2/jilei/dicom.py` & `jilei-0.2.3/jilei/dicom.py`

 * *Files identical despite different names*

### Comparing `jilei-0.2.2/jilei/docker_tools.py` & `jilei-0.2.3/jilei/docker_tools.py`

 * *Files identical despite different names*

### Comparing `jilei-0.2.2/jilei/mapping_3d_to_2d.py` & `jilei-0.2.3/jilei/mapping_3d_to_2d.py`

 * *Files identical despite different names*

### Comparing `jilei-0.2.2/jilei/medical_image_tools.py` & `jilei-0.2.3/jilei/medical_image_tools.py`

 * *Files identical despite different names*

### Comparing `jilei-0.2.2/jilei/mimics.py` & `jilei-0.2.3/jilei/mimics.py`

 * *Files identical despite different names*

### Comparing `jilei-0.2.2/jilei/mimics_qt.py` & `jilei-0.2.3/jilei/mimics_qt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 import os
 import re
 import sys
 import json
 import numpy as np
 import pydicom
-import matplotlib.pyplot as plt
 from collections import OrderedDict
 
-from PIL import Image
 from PyQt5 import QtGui, QtCore
 from PyQt5.QtWidgets import QApplication, QMainWindow, QWidget, QVBoxLayout, QHBoxLayout, QLabel, QLineEdit, \
     QPushButton, QFileDialog, QMessageBox
-import dicom2nifti
 
 from jilei.mimics import draw_pixel_value_distribution
 from jilei.dicom import change_pixel_value, change_pixel_value_from_dcmfile, get_dicoms, dicoms_to_nii
 from jilei.qt import pixel_array_2_qimage
 
 
 def start():
@@ -89,19 +86,19 @@
     # 保存标签名称
     with open(os.path.join(dcm_path, 'dist', "dataset.json"), 'w') as fp:
         labelnames["0"] = "background"
         labelnames = OrderedDict(sorted(labelnames.items()))
         datasetjson = {"labels": labelnames}
         modality = dcms[0].Modality
         if modality == "CT":
-            datasetjson["modality"] = {"CT"}
+            datasetjson["modality"] = {"0": "CT"}
         elif modality == "MR":
-            datasetjson["modality"] = {"MRI"}
+            datasetjson["modality"] = {"0": "MRI"}
         else:
-            datasetjson["modality"] = {modality}
+            datasetjson["modality"] = {"0": modality}
         json_str = json.dumps(datasetjson, indent=4)
         fp.write(json_str)
 
     message("提示", "转换完成")
 
 
 def convert_original(dcm_path):
```

### Comparing `jilei-0.2.2/jilei/nnunet_tools.py` & `jilei-0.2.3/jilei/nnunet_tools.py`

 * *Files identical despite different names*

### Comparing `jilei-0.2.2/jilei/qt.py` & `jilei-0.2.3/jilei/qt.py`

 * *Files identical despite different names*

### Comparing `jilei-0.2.2/jilei/system_tools.py` & `jilei-0.2.3/jilei/system_tools.py`

 * *Files identical despite different names*

### Comparing `jilei-0.2.2/jilei/wxwork.py` & `jilei-0.2.3/jilei/wxwork.py`

 * *Files identical despite different names*

### Comparing `jilei-0.2.2/setup.py` & `jilei-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="jilei",
-    version="0.2.2",
+    version="0.2.3",
     author="jilei",
     author_email="developer@jlzn.cc",
     description="For internal use.",
     long_description="python setup.py bdist_wheel\ntwine upload ./dist/*",
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

