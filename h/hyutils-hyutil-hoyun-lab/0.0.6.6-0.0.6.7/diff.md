# Comparing `tmp/hyutils-hyutil-hoyun-lab-0.0.6.6.tar.gz` & `tmp/hyutils-hyutil-hoyun-lab-0.0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyutils-hyutil-hoyun-lab-0.0.6.6.tar", last modified: Fri Jul 14 02:32:59 2023, max compression
+gzip compressed data, was "hyutils-hyutil-hoyun-lab-0.0.6.7.tar", last modified: Fri Jul 14 02:48:21 2023, max compression
```

## Comparing `hyutils-hyutil-hoyun-lab-0.0.6.6.tar` & `hyutils-hyutil-hoyun-lab-0.0.6.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 02:32:59.138076 hyutils-hyutil-hoyun-lab-0.0.6.6/
--rw-rw-rw-   0        0        0       37 2023-06-08 03:25:08.000000 hyutils-hyutil-hoyun-lab-0.0.6.6/LICENSE.txt
--rw-rw-rw-   0        0        0      600 2023-07-14 02:32:59.137655 hyutils-hyutil-hoyun-lab-0.0.6.6/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-06-07 07:35:00.000000 hyutils-hyutil-hoyun-lab-0.0.6.6/README.md
--rw-rw-rw-   0        0        0      104 2023-06-07 07:28:49.000000 hyutils-hyutil-hoyun-lab-0.0.6.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-14 02:32:59.138587 hyutils-hyutil-hoyun-lab-0.0.6.6/setup.cfg
--rw-rw-rw-   0        0        0      852 2023-07-14 02:32:14.000000 hyutils-hyutil-hoyun-lab-0.0.6.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-14 02:32:59.109576 hyutils-hyutil-hoyun-lab-0.0.6.6/src/
-drwxrwxrwx   0        0        0        0 2023-07-14 02:32:59.130076 hyutils-hyutil-hoyun-lab-0.0.6.6/src/hyutil_hoyun_lab/
--rw-rw-rw-   0        0        0      347 2023-07-14 02:32:14.000000 hyutils-hyutil-hoyun-lab-0.0.6.6/src/hyutil_hoyun_lab/__init__.py
--rw-rw-rw-   0        0        0      435 2023-01-19 02:15:34.000000 hyutils-hyutil-hoyun-lab-0.0.6.6/src/hyutil_hoyun_lab/appcontrol.py
--rw-rw-rw-   0        0        0     4333 2023-06-28 05:31:55.000000 hyutils-hyutil-hoyun-lab-0.0.6.6/src/hyutil_hoyun_lab/augmentjob.py
--rw-rw-rw-   0        0        0      614 2023-05-30 04:04:27.000000 hyutils-hyutil-hoyun-lab-0.0.6.6/src/hyutil_hoyun_lab/date_time.py
--rw-rw-rw-   0        0        0     1471 2023-06-21 03:54:21.000000 hyutils-hyutil-hoyun-lab-0.0.6.6/src/hyutil_hoyun_lab/dirjob.py
--rw-rw-rw-   0        0        0      477 2023-06-16 04:42:56.000000 hyutils-hyutil-hoyun-lab-0.0.6.6/src/hyutil_hoyun_lab/filejob.py
--rw-rw-rw-   0        0        0     1086 2023-02-02 02:25:56.000000 hyutils-hyutil-hoyun-lab-0.0.6.6/src/hyutil_hoyun_lab/hashing.py
--rw-rw-rw-   0        0        0    15362 2023-06-28 07:08:39.000000 hyutils-hyutil-hoyun-lab-0.0.6.6/src/hyutil_hoyun_lab/tfrecrod_utils.py
--rw-rw-rw-   0        0        0     7808 2023-07-14 02:31:08.000000 hyutils-hyutil-hoyun-lab-0.0.6.6/src/hyutil_hoyun_lab/xml_util.py
-drwxrwxrwx   0        0        0        0 2023-07-14 02:32:59.136077 hyutils-hyutil-hoyun-lab-0.0.6.6/src/hyutils_hyutil_hoyun_lab.egg-info/
--rw-rw-rw-   0        0        0      600 2023-07-14 02:32:59.000000 hyutils-hyutil-hoyun-lab-0.0.6.6/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      557 2023-07-14 02:32:59.000000 hyutils-hyutil-hoyun-lab-0.0.6.6/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 02:32:59.000000 hyutils-hyutil-hoyun-lab-0.0.6.6/src/hyutils_hyutil_hoyun_lab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-14 02:32:59.000000 hyutils-hyutil-hoyun-lab-0.0.6.6/src/hyutils_hyutil_hoyun_lab.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 02:48:21.558226 hyutils-hyutil-hoyun-lab-0.0.6.7/
+-rw-rw-rw-   0        0        0       37 2023-06-08 03:25:08.000000 hyutils-hyutil-hoyun-lab-0.0.6.7/LICENSE.txt
+-rw-rw-rw-   0        0        0      600 2023-07-14 02:48:21.557769 hyutils-hyutil-hoyun-lab-0.0.6.7/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2023-06-07 07:35:00.000000 hyutils-hyutil-hoyun-lab-0.0.6.7/README.md
+-rw-rw-rw-   0        0        0      104 2023-06-07 07:28:49.000000 hyutils-hyutil-hoyun-lab-0.0.6.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-14 02:48:21.558725 hyutils-hyutil-hoyun-lab-0.0.6.7/setup.cfg
+-rw-rw-rw-   0        0        0      852 2023-07-14 02:47:12.000000 hyutils-hyutil-hoyun-lab-0.0.6.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 02:48:21.524726 hyutils-hyutil-hoyun-lab-0.0.6.7/src/
+drwxrwxrwx   0        0        0        0 2023-07-14 02:48:21.549224 hyutils-hyutil-hoyun-lab-0.0.6.7/src/hyutil_hoyun_lab/
+-rw-rw-rw-   0        0        0      347 2023-07-14 02:47:12.000000 hyutils-hyutil-hoyun-lab-0.0.6.7/src/hyutil_hoyun_lab/__init__.py
+-rw-rw-rw-   0        0        0      435 2023-01-19 02:15:34.000000 hyutils-hyutil-hoyun-lab-0.0.6.7/src/hyutil_hoyun_lab/appcontrol.py
+-rw-rw-rw-   0        0        0     4333 2023-06-28 05:31:55.000000 hyutils-hyutil-hoyun-lab-0.0.6.7/src/hyutil_hoyun_lab/augmentjob.py
+-rw-rw-rw-   0        0        0      614 2023-05-30 04:04:27.000000 hyutils-hyutil-hoyun-lab-0.0.6.7/src/hyutil_hoyun_lab/date_time.py
+-rw-rw-rw-   0        0        0     1471 2023-06-21 03:54:21.000000 hyutils-hyutil-hoyun-lab-0.0.6.7/src/hyutil_hoyun_lab/dirjob.py
+-rw-rw-rw-   0        0        0      477 2023-06-16 04:42:56.000000 hyutils-hyutil-hoyun-lab-0.0.6.7/src/hyutil_hoyun_lab/filejob.py
+-rw-rw-rw-   0        0        0     1086 2023-02-02 02:25:56.000000 hyutils-hyutil-hoyun-lab-0.0.6.7/src/hyutil_hoyun_lab/hashing.py
+-rw-rw-rw-   0        0        0    15362 2023-06-28 07:08:39.000000 hyutils-hyutil-hoyun-lab-0.0.6.7/src/hyutil_hoyun_lab/tfrecrod_utils.py
+-rw-rw-rw-   0        0        0     7835 2023-07-14 02:47:46.000000 hyutils-hyutil-hoyun-lab-0.0.6.7/src/hyutil_hoyun_lab/xml_util.py
+drwxrwxrwx   0        0        0        0 2023-07-14 02:48:21.555725 hyutils-hyutil-hoyun-lab-0.0.6.7/src/hyutils_hyutil_hoyun_lab.egg-info/
+-rw-rw-rw-   0        0        0      600 2023-07-14 02:48:21.000000 hyutils-hyutil-hoyun-lab-0.0.6.7/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      557 2023-07-14 02:48:21.000000 hyutils-hyutil-hoyun-lab-0.0.6.7/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 02:48:21.000000 hyutils-hyutil-hoyun-lab-0.0.6.7/src/hyutils_hyutil_hoyun_lab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-14 02:48:21.000000 hyutils-hyutil-hoyun-lab-0.0.6.7/src/hyutils_hyutil_hoyun_lab.egg-info/top_level.txt
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.6/PKG-INFO` & `hyutils-hyutil-hoyun-lab-0.0.6.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyutils-hyutil-hoyun-lab
-Version: 0.0.6.6
+Version: 0.0.6.7
 Summary: Hoyun Lab Python Utils
 Home-page: https://www.hoyun.co.kr
 Author: nohgan im
 Author-email: fory2k@hoyun.co.kr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/schooldevops/python-tutorials/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.6/setup.py` & `hyutils-hyutil-hoyun-lab-0.0.6.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
     
 
 setuptools.setup(
     name="hyutils-hyutil-hoyun-lab",
-    version="0.0.6.6",
+    version="0.0.6.7",
     url="https://www.hoyun.co.kr",
     license="MIT",
     author="nohgan im",
     author_email="fory2k@hoyun.co.kr",
     description="Hoyun Lab Python Utils",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.6/src/hyutil_hoyun_lab/augmentjob.py` & `hyutils-hyutil-hoyun-lab-0.0.6.7/src/hyutil_hoyun_lab/augmentjob.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.6/src/hyutil_hoyun_lab/date_time.py` & `hyutils-hyutil-hoyun-lab-0.0.6.7/src/hyutil_hoyun_lab/date_time.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.6/src/hyutil_hoyun_lab/dirjob.py` & `hyutils-hyutil-hoyun-lab-0.0.6.7/src/hyutil_hoyun_lab/dirjob.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.6/src/hyutil_hoyun_lab/hashing.py` & `hyutils-hyutil-hoyun-lab-0.0.6.7/src/hyutil_hoyun_lab/hashing.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.6/src/hyutil_hoyun_lab/tfrecrod_utils.py` & `hyutils-hyutil-hoyun-lab-0.0.6.7/src/hyutil_hoyun_lab/tfrecrod_utils.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.6/src/hyutil_hoyun_lab/xml_util.py` & `hyutils-hyutil-hoyun-lab-0.0.6.7/src/hyutil_hoyun_lab/xml_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import xml.etree.ElementTree as ET
 import os
 import shutil
 import cv2
-import dirjob as dirjob
+from dirjob import get_entry_count
+from dirjob import files_ext
 
 """
 def indent
 
 def read_xml
 
 def make_xml
@@ -123,17 +124,17 @@
     # 주석(xml)기록
     with open(path, 'wb') as f:
         f.write(b_xml)
 
 def check_xml_n_fix(xml_path, image_path):
     if os.path.exists(xml_path) and os.path.exists(image_path):
         index = 0
-        count = dirjob.get_entry_count(xml_path, '.xml')
+        count = get_entry_count(xml_path, '.xml')
 
-        for file in dirjob.files_ext(xml_path, '.xml'):
+        for file in files_ext(xml_path, '.xml'):
             index += 1
             if index % 1000 == 0:
                 print(f'> {index} <')
 
             xml_file = os.path.join(xml_path, file)
             xml_name = os.path.splitext(file)[0]
             image_name = xml_name + '.jpg'
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.6/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO` & `hyutils-hyutil-hoyun-lab-0.0.6.7/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyutils-hyutil-hoyun-lab
-Version: 0.0.6.6
+Version: 0.0.6.7
 Summary: Hoyun Lab Python Utils
 Home-page: https://www.hoyun.co.kr
 Author: nohgan im
 Author-email: fory2k@hoyun.co.kr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/schooldevops/python-tutorials/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.6/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt` & `hyutils-hyutil-hoyun-lab-0.0.6.7/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

