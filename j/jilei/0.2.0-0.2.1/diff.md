# Comparing `tmp/jilei-0.2.0.tar.gz` & `tmp/jilei-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\jilei-0.2.0.tar", last modified: Fri Jul 14 07:01:53 2023, max compression
+gzip compressed data, was "dist\jilei-0.2.1.tar", last modified: Fri Jul 14 07:10:33 2023, max compression
```

## Comparing `jilei-0.2.0.tar` & `jilei-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 07:01:53.097209 jilei-0.2.0/
--rw-rw-rw-   0        0        0      448 2023-07-14 07:01:53.096208 jilei-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      369 2023-05-07 08:49:40.000000 jilei-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 07:01:53.083196 jilei-0.2.0/jilei/
--rw-rw-rw-   0        0        0        0 2023-04-12 11:09:36.000000 jilei-0.2.0/jilei/__init__.py
--rw-rw-rw-   0        0        0     3229 2023-07-14 04:55:57.000000 jilei-0.2.0/jilei/dicom.py
--rw-rw-rw-   0        0        0     2666 2023-05-07 09:36:18.000000 jilei-0.2.0/jilei/docker_tools.py
--rw-rw-rw-   0        0        0     1521 2023-06-07 09:04:28.000000 jilei-0.2.0/jilei/mapping_3d_to_2d.py
--rw-rw-rw-   0        0        0     7409 2023-05-26 10:47:48.000000 jilei-0.2.0/jilei/medical_image_tools.py
--rw-rw-rw-   0        0        0     4446 2023-07-13 16:35:27.000000 jilei-0.2.0/jilei/mimics.py
--rw-rw-rw-   0        0        0    17006 2023-07-14 07:00:44.000000 jilei-0.2.0/jilei/mimics_qt.py
--rw-rw-rw-   0        0        0     1006 2023-04-20 06:23:16.000000 jilei-0.2.0/jilei/nnunet_tools.py
--rw-rw-rw-   0        0        0      640 2023-07-13 04:01:00.000000 jilei-0.2.0/jilei/qt.py
--rw-rw-rw-   0        0        0     1210 2023-05-07 09:28:34.000000 jilei-0.2.0/jilei/system_tools.py
--rw-rw-rw-   0        0        0     1744 2023-04-12 12:32:48.000000 jilei-0.2.0/jilei/wxwork.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:01:53.096208 jilei-0.2.0/jilei.egg-info/
--rw-rw-rw-   0        0        0      448 2023-07-14 07:01:53.000000 jilei-0.2.0/jilei.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2023-07-14 07:01:53.000000 jilei-0.2.0/jilei.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 07:01:53.000000 jilei-0.2.0/jilei.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-14 07:01:53.000000 jilei-0.2.0/jilei.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 07:01:53.097209 jilei-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      523 2023-07-14 07:01:52.000000 jilei-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:10:33.277138 jilei-0.2.1/
+-rw-rw-rw-   0        0        0      448 2023-07-14 07:10:33.276138 jilei-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2023-05-07 08:49:40.000000 jilei-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 07:10:33.267129 jilei-0.2.1/jilei/
+-rw-rw-rw-   0        0        0        0 2023-04-12 11:09:36.000000 jilei-0.2.1/jilei/__init__.py
+-rw-rw-rw-   0        0        0     3229 2023-07-14 04:55:57.000000 jilei-0.2.1/jilei/dicom.py
+-rw-rw-rw-   0        0        0     2666 2023-05-07 09:36:18.000000 jilei-0.2.1/jilei/docker_tools.py
+-rw-rw-rw-   0        0        0     1521 2023-06-07 09:04:28.000000 jilei-0.2.1/jilei/mapping_3d_to_2d.py
+-rw-rw-rw-   0        0        0     7409 2023-05-26 10:47:48.000000 jilei-0.2.1/jilei/medical_image_tools.py
+-rw-rw-rw-   0        0        0     4446 2023-07-13 16:35:27.000000 jilei-0.2.1/jilei/mimics.py
+-rw-rw-rw-   0        0        0    17009 2023-07-14 07:10:17.000000 jilei-0.2.1/jilei/mimics_qt.py
+-rw-rw-rw-   0        0        0     1006 2023-04-20 06:23:16.000000 jilei-0.2.1/jilei/nnunet_tools.py
+-rw-rw-rw-   0        0        0      640 2023-07-13 04:01:00.000000 jilei-0.2.1/jilei/qt.py
+-rw-rw-rw-   0        0        0     1210 2023-05-07 09:28:34.000000 jilei-0.2.1/jilei/system_tools.py
+-rw-rw-rw-   0        0        0     1744 2023-04-12 12:32:48.000000 jilei-0.2.1/jilei/wxwork.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:10:33.276138 jilei-0.2.1/jilei.egg-info/
+-rw-rw-rw-   0        0        0      448 2023-07-14 07:10:33.000000 jilei-0.2.1/jilei.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2023-07-14 07:10:33.000000 jilei-0.2.1/jilei.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 07:10:33.000000 jilei-0.2.1/jilei.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-14 07:10:33.000000 jilei-0.2.1/jilei.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 07:10:33.277138 jilei-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      523 2023-07-14 07:10:32.000000 jilei-0.2.1/setup.py
```

### Comparing `jilei-0.2.0/jilei/dicom.py` & `jilei-0.2.1/jilei/dicom.py`

 * *Files identical despite different names*

### Comparing `jilei-0.2.0/jilei/docker_tools.py` & `jilei-0.2.1/jilei/docker_tools.py`

 * *Files identical despite different names*

### Comparing `jilei-0.2.0/jilei/mapping_3d_to_2d.py` & `jilei-0.2.1/jilei/mapping_3d_to_2d.py`

 * *Files identical despite different names*

### Comparing `jilei-0.2.0/jilei/medical_image_tools.py` & `jilei-0.2.1/jilei/medical_image_tools.py`

 * *Files identical despite different names*

### Comparing `jilei-0.2.0/jilei/mimics.py` & `jilei-0.2.1/jilei/mimics.py`

 * *Files identical despite different names*

### Comparing `jilei-0.2.0/jilei/mimics_qt.py` & `jilei-0.2.1/jilei/mimics_qt.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 
 from PIL import Image
 from PyQt5 import QtGui, QtCore
 from PyQt5.QtWidgets import QApplication, QMainWindow, QWidget, QVBoxLayout, QHBoxLayout, QLabel, QLineEdit, \
     QPushButton, QFileDialog, QMessageBox
 import dicom2nifti
 
-from mimics import draw_pixel_value_distribution
-from dicom import change_pixel_value, change_pixel_value_from_dcmfile, get_dicoms, dicoms_to_nii
-from qt import pixel_array_2_qimage
+from .mimics import draw_pixel_value_distribution
+from .dicom import change_pixel_value, change_pixel_value_from_dcmfile, get_dicoms, dicoms_to_nii
+from .qt import pixel_array_2_qimage
 
 
 def start():
     app = QApplication(sys.argv)
     window = MimicsToolWindow()
     window.show()
     sys.exit(app.exec_())
```

### Comparing `jilei-0.2.0/jilei/nnunet_tools.py` & `jilei-0.2.1/jilei/nnunet_tools.py`

 * *Files identical despite different names*

### Comparing `jilei-0.2.0/jilei/qt.py` & `jilei-0.2.1/jilei/qt.py`

 * *Files identical despite different names*

### Comparing `jilei-0.2.0/jilei/system_tools.py` & `jilei-0.2.1/jilei/system_tools.py`

 * *Files identical despite different names*

### Comparing `jilei-0.2.0/jilei/wxwork.py` & `jilei-0.2.1/jilei/wxwork.py`

 * *Files identical despite different names*

### Comparing `jilei-0.2.0/setup.py` & `jilei-0.2.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="jilei",
-    version="0.2.0",
+    version="0.2.1",
     author="jilei",
     author_email="developer@jlzn.cc",
     description="For internal use.",
     long_description="python setup.py bdist_wheel\ntwine upload ./dist/*",
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

