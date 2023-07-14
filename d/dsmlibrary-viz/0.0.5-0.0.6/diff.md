# Comparing `tmp/dsmlibrary_viz-0.0.5.tar.gz` & `tmp/dsmlibrary_viz-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsmlibrary_viz-0.0.5.tar", last modified: Thu Jul 13 09:26:19 2023, max compression
+gzip compressed data, was "dsmlibrary_viz-0.0.6.tar", last modified: Fri Jul 14 06:15:37 2023, max compression
```

## Comparing `dsmlibrary_viz-0.0.5.tar` & `dsmlibrary_viz-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-13 09:26:19.562590 dsmlibrary_viz-0.0.5/
--rw-r--r--   0 naii       (501) staff       (20)     1066 2023-07-12 12:08:08.000000 dsmlibrary_viz-0.0.5/LICENSE
--rw-r--r--   0 naii       (501) staff       (20)     1054 2023-07-13 09:26:19.562071 dsmlibrary_viz-0.0.5/PKG-INFO
--rw-r--r--   0 naii       (501) staff       (20)      355 2023-07-12 14:26:15.000000 dsmlibrary_viz-0.0.5/README.md
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-13 09:26:19.558595 dsmlibrary_viz-0.0.5/dsmlibrary_viz/
--rw-r--r--   0 naii       (501) staff       (20)      160 2023-07-13 09:26:15.000000 dsmlibrary_viz-0.0.5/dsmlibrary_viz/__init__.py
--rw-r--r--   0 naii       (501) staff       (20)     2255 2023-07-12 14:14:40.000000 dsmlibrary_viz-0.0.5/dsmlibrary_viz/base.py
--rw-r--r--   0 naii       (501) staff       (20)     2221 2023-07-13 09:19:09.000000 dsmlibrary_viz-0.0.5/dsmlibrary_viz/data_viz.py
--rw-r--r--   0 naii       (501) staff       (20)      619 2023-07-12 15:26:02.000000 dsmlibrary_viz-0.0.5/dsmlibrary_viz/utils.py
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-13 09:26:19.561313 dsmlibrary_viz-0.0.5/dsmlibrary_viz.egg-info/
--rw-r--r--   0 naii       (501) staff       (20)     1054 2023-07-13 09:26:19.000000 dsmlibrary_viz-0.0.5/dsmlibrary_viz.egg-info/PKG-INFO
--rw-r--r--   0 naii       (501) staff       (20)      316 2023-07-13 09:26:19.000000 dsmlibrary_viz-0.0.5/dsmlibrary_viz.egg-info/SOURCES.txt
--rw-r--r--   0 naii       (501) staff       (20)        1 2023-07-13 09:26:19.000000 dsmlibrary_viz-0.0.5/dsmlibrary_viz.egg-info/dependency_links.txt
--rw-r--r--   0 naii       (501) staff       (20)       39 2023-07-13 09:26:19.000000 dsmlibrary_viz-0.0.5/dsmlibrary_viz.egg-info/requires.txt
--rw-r--r--   0 naii       (501) staff       (20)       15 2023-07-13 09:26:19.000000 dsmlibrary_viz-0.0.5/dsmlibrary_viz.egg-info/top_level.txt
--rw-r--r--   0 naii       (501) staff       (20)       38 2023-07-13 09:26:19.562789 dsmlibrary_viz-0.0.5/setup.cfg
--rw-r--r--   0 naii       (501) staff       (20)     1432 2023-07-13 09:26:06.000000 dsmlibrary_viz-0.0.5/setup.py
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-14 06:15:37.371340 dsmlibrary_viz-0.0.6/
+-rw-r--r--   0 naii       (501) staff       (20)     1066 2023-07-12 12:08:08.000000 dsmlibrary_viz-0.0.6/LICENSE
+-rw-r--r--   0 naii       (501) staff       (20)     1067 2023-07-14 06:15:37.370991 dsmlibrary_viz-0.0.6/PKG-INFO
+-rw-r--r--   0 naii       (501) staff       (20)      368 2023-07-14 05:57:14.000000 dsmlibrary_viz-0.0.6/README.md
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-14 06:15:37.364927 dsmlibrary_viz-0.0.6/dsmlibrary_viz/
+-rw-r--r--   0 naii       (501) staff       (20)      160 2023-07-14 06:15:29.000000 dsmlibrary_viz-0.0.6/dsmlibrary_viz/__init__.py
+-rw-r--r--   0 naii       (501) staff       (20)     2255 2023-07-12 14:14:40.000000 dsmlibrary_viz-0.0.6/dsmlibrary_viz/base.py
+-rw-r--r--   0 naii       (501) staff       (20)     2221 2023-07-13 09:19:09.000000 dsmlibrary_viz-0.0.6/dsmlibrary_viz/data_viz.py
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-14 06:15:37.369968 dsmlibrary_viz-0.0.6/dsmlibrary_viz/scripts/
+-rw-r--r--   0 naii       (501) staff       (20)       25 2023-07-14 06:11:01.000000 dsmlibrary_viz-0.0.6/dsmlibrary_viz/scripts/__init__.py
+-rw-r--r--   0 naii       (501) staff       (20)      133 2023-07-14 06:13:28.000000 dsmlibrary_viz-0.0.6/dsmlibrary_viz/scripts/install_ext.py
+-rw-r--r--   0 naii       (501) staff       (20)      619 2023-07-12 15:26:02.000000 dsmlibrary_viz-0.0.6/dsmlibrary_viz/utils.py
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-14 06:15:37.367986 dsmlibrary_viz-0.0.6/dsmlibrary_viz.egg-info/
+-rw-r--r--   0 naii       (501) staff       (20)     1067 2023-07-14 06:15:37.000000 dsmlibrary_viz-0.0.6/dsmlibrary_viz.egg-info/PKG-INFO
+-rw-r--r--   0 naii       (501) staff       (20)      389 2023-07-14 06:15:37.000000 dsmlibrary_viz-0.0.6/dsmlibrary_viz.egg-info/SOURCES.txt
+-rw-r--r--   0 naii       (501) staff       (20)        1 2023-07-14 06:15:37.000000 dsmlibrary_viz-0.0.6/dsmlibrary_viz.egg-info/dependency_links.txt
+-rw-r--r--   0 naii       (501) staff       (20)       39 2023-07-14 06:15:37.000000 dsmlibrary_viz-0.0.6/dsmlibrary_viz.egg-info/requires.txt
+-rw-r--r--   0 naii       (501) staff       (20)       15 2023-07-14 06:15:37.000000 dsmlibrary_viz-0.0.6/dsmlibrary_viz.egg-info/top_level.txt
+-rw-r--r--   0 naii       (501) staff       (20)       38 2023-07-14 06:15:37.371480 dsmlibrary_viz-0.0.6/setup.cfg
+-rw-r--r--   0 naii       (501) staff       (20)     1497 2023-07-14 06:14:33.000000 dsmlibrary_viz-0.0.6/setup.py
```

### Comparing `dsmlibrary_viz-0.0.5/LICENSE` & `dsmlibrary_viz-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dsmlibrary_viz-0.0.5/PKG-INFO` & `dsmlibrary_viz-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsmlibrary_viz
-Version: 0.0.5
+Version: 0.0.6
 Summary: A simple way to use Dataset. for dsm
 Home-page: https://github.com/storemesh/dsmlibrary-viz
 Author: DigitalStoreMesh Co.,Ltd
 Author-email: contact@storemesh.com
 License: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -33,11 +33,12 @@
     dataplatform_api_uri="<dataplatform_api_uri>", 
     object_storage_uri="<object_storage_uri>"
 )
 
 data = dataviz.query(
 """
     SELECT * FROM 'DISCOVERY:<FILE_ID>'
+    LIMIT 10
 """ 
 )
 print(data)
 ```
```

### Comparing `dsmlibrary_viz-0.0.5/dsmlibrary_viz/base.py` & `dsmlibrary_viz-0.0.6/dsmlibrary_viz/base.py`

 * *Files identical despite different names*

### Comparing `dsmlibrary_viz-0.0.5/dsmlibrary_viz/data_viz.py` & `dsmlibrary_viz-0.0.6/dsmlibrary_viz/data_viz.py`

 * *Files identical despite different names*

### Comparing `dsmlibrary_viz-0.0.5/dsmlibrary_viz/utils.py` & `dsmlibrary_viz-0.0.6/dsmlibrary_viz/utils.py`

 * *Files identical despite different names*

### Comparing `dsmlibrary_viz-0.0.5/dsmlibrary_viz.egg-info/PKG-INFO` & `dsmlibrary_viz-0.0.6/dsmlibrary_viz.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsmlibrary-viz
-Version: 0.0.5
+Version: 0.0.6
 Summary: A simple way to use Dataset. for dsm
 Home-page: https://github.com/storemesh/dsmlibrary-viz
 Author: DigitalStoreMesh Co.,Ltd
 Author-email: contact@storemesh.com
 License: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -33,11 +33,12 @@
     dataplatform_api_uri="<dataplatform_api_uri>", 
     object_storage_uri="<object_storage_uri>"
 )
 
 data = dataviz.query(
 """
     SELECT * FROM 'DISCOVERY:<FILE_ID>'
+    LIMIT 10
 """ 
 )
 print(data)
 ```
```

### Comparing `dsmlibrary_viz-0.0.5/setup.py` & `dsmlibrary_viz-0.0.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import re
 from setuptools import find_packages, setup
+from dsmlibrary_viz import scripts
 
 package="dsmlibrary_viz"
 
 def get_version():
     init_py = open(os.path.join(package, '__init__.py')).read()
     return re.search("__version__ = ['\"]([^'\"]+)['\"]", init_py).group(1)
     
@@ -39,9 +40,11 @@
     ],
     install_requires=[
         'requests',
         's3fs',
         'duckdb',
         'pandas',
         'matplotlib'
-    ],    
-)
+    ]
+)
+
+scripts.install_ext.install_ext()
```

