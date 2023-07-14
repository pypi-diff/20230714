# Comparing `tmp/tf2-sku-to-name-1.0.1.tar.gz` & `tmp/tf2-sku-to-name-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tf2-sku-to-name-1.0.1.tar", last modified: Fri Jul 14 15:08:01 2023, max compression
+gzip compressed data, was "tf2-sku-to-name-1.0.2.tar", last modified: Fri Jul 14 15:14:08 2023, max compression
```

## Comparing `tf2-sku-to-name-1.0.1.tar` & `tf2-sku-to-name-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ketan1     (502) staff       (20)        0 2023-07-14 15:08:01.075055 tf2-sku-to-name-1.0.1/
--rw-r--r--   0 ketan1     (502) staff       (20)     1070 2023-07-14 08:20:26.000000 tf2-sku-to-name-1.0.1/LICENSE
--rw-r--r--   0 ketan1     (502) staff       (20)      418 2023-07-14 15:08:01.074942 tf2-sku-to-name-1.0.1/PKG-INFO
--rw-r--r--   0 ketan1     (502) staff       (20)     1508 2023-07-14 14:53:36.000000 tf2-sku-to-name-1.0.1/README.md
--rw-r--r--   0 ketan1     (502) staff       (20)       38 2023-07-14 15:08:01.075094 tf2-sku-to-name-1.0.1/setup.cfg
--rw-r--r--   0 ketan1     (502) staff       (20)      560 2023-07-14 15:04:25.000000 tf2-sku-to-name-1.0.1/setup.py
-drwxr-xr-x   0 ketan1     (502) staff       (20)        0 2023-07-14 15:08:01.074129 tf2-sku-to-name-1.0.1/sku/
--rw-r--r--   0 ketan1     (502) staff       (20)      668 2023-07-14 07:35:40.000000 tf2-sku-to-name-1.0.1/sku/models.py
--rw-r--r--   0 ketan1     (502) staff       (20)     5144 2023-07-14 08:36:38.000000 tf2-sku-to-name-1.0.1/sku/parser.py
-drwxr-xr-x   0 ketan1     (502) staff       (20)        0 2023-07-14 15:08:01.074783 tf2-sku-to-name-1.0.1/tf2_sku_to_name.egg-info/
--rw-r--r--   0 ketan1     (502) staff       (20)      418 2023-07-14 15:08:01.000000 tf2-sku-to-name-1.0.1/tf2_sku_to_name.egg-info/PKG-INFO
--rw-r--r--   0 ketan1     (502) staff       (20)      248 2023-07-14 15:08:01.000000 tf2-sku-to-name-1.0.1/tf2_sku_to_name.egg-info/SOURCES.txt
--rw-r--r--   0 ketan1     (502) staff       (20)        1 2023-07-14 15:08:01.000000 tf2-sku-to-name-1.0.1/tf2_sku_to_name.egg-info/dependency_links.txt
--rw-r--r--   0 ketan1     (502) staff       (20)       24 2023-07-14 15:08:01.000000 tf2-sku-to-name-1.0.1/tf2_sku_to_name.egg-info/requires.txt
--rw-r--r--   0 ketan1     (502) staff       (20)        4 2023-07-14 15:08:01.000000 tf2-sku-to-name-1.0.1/tf2_sku_to_name.egg-info/top_level.txt
+drwxr-xr-x   0 ketan1     (502) staff       (20)        0 2023-07-14 15:14:08.506106 tf2-sku-to-name-1.0.2/
+-rw-r--r--   0 ketan1     (502) staff       (20)     1070 2023-07-14 08:20:26.000000 tf2-sku-to-name-1.0.2/LICENSE
+-rw-r--r--   0 ketan1     (502) staff       (20)      418 2023-07-14 15:14:08.505983 tf2-sku-to-name-1.0.2/PKG-INFO
+-rw-r--r--   0 ketan1     (502) staff       (20)     1508 2023-07-14 14:53:36.000000 tf2-sku-to-name-1.0.2/README.md
+-rw-r--r--   0 ketan1     (502) staff       (20)       38 2023-07-14 15:14:08.506144 tf2-sku-to-name-1.0.2/setup.cfg
+-rw-r--r--   0 ketan1     (502) staff       (20)      560 2023-07-14 15:14:05.000000 tf2-sku-to-name-1.0.2/setup.py
+drwxr-xr-x   0 ketan1     (502) staff       (20)        0 2023-07-14 15:14:08.505182 tf2-sku-to-name-1.0.2/sku/
+-rw-r--r--   0 ketan1     (502) staff       (20)      668 2023-07-14 07:35:40.000000 tf2-sku-to-name-1.0.2/sku/models.py
+-rw-r--r--   0 ketan1     (502) staff       (20)     5249 2023-07-14 15:13:23.000000 tf2-sku-to-name-1.0.2/sku/parser.py
+drwxr-xr-x   0 ketan1     (502) staff       (20)        0 2023-07-14 15:14:08.505819 tf2-sku-to-name-1.0.2/tf2_sku_to_name.egg-info/
+-rw-r--r--   0 ketan1     (502) staff       (20)      418 2023-07-14 15:14:08.000000 tf2-sku-to-name-1.0.2/tf2_sku_to_name.egg-info/PKG-INFO
+-rw-r--r--   0 ketan1     (502) staff       (20)      248 2023-07-14 15:14:08.000000 tf2-sku-to-name-1.0.2/tf2_sku_to_name.egg-info/SOURCES.txt
+-rw-r--r--   0 ketan1     (502) staff       (20)        1 2023-07-14 15:14:08.000000 tf2-sku-to-name-1.0.2/tf2_sku_to_name.egg-info/dependency_links.txt
+-rw-r--r--   0 ketan1     (502) staff       (20)       24 2023-07-14 15:14:08.000000 tf2-sku-to-name-1.0.2/tf2_sku_to_name.egg-info/requires.txt
+-rw-r--r--   0 ketan1     (502) staff       (20)        4 2023-07-14 15:14:08.000000 tf2-sku-to-name-1.0.2/tf2_sku_to_name.egg-info/top_level.txt
```

### Comparing `tf2-sku-to-name-1.0.1/LICENSE` & `tf2-sku-to-name-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tf2-sku-to-name-1.0.1/README.md` & `tf2-sku-to-name-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tf2-sku-to-name-1.0.1/setup.py` & `tf2-sku-to-name-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='tf2-sku-to-name',
-    version='1.0.1',
+    version='1.0.2',
     author='Purple Barber',
     description="A python library that parses TF2 item SKU to the item's name and vice versa.",
     url='https://github.com/purplebarber/tf2-sku',
     license='MIT',
     packages=["sku"],
     install_requires=[
         'requests',
```

### Comparing `tf2-sku-to-name-1.0.1/sku/models.py` & `tf2-sku-to-name-1.0.2/sku/models.py`

 * *Files identical despite different names*

### Comparing `tf2-sku-to-name-1.0.1/sku/parser.py` & `tf2-sku-to-name-1.0.2/sku/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from sku.models import itemClass as itemClass
 from typing import List
 from collections import deque
 import requests
 from bs4 import BeautifulSoup as bs
 from json import load, dump
+import os
 
-DATA_FILE = "sku/data/data.json"
+current_directory = os.path.dirname(os.path.abspath(__file__))
+DATA_FILE = os.path.join(current_directory, 'data', 'data.json')
 
 
 class Sku:
     @staticmethod
     def object_to_sku(item: itemClass) -> str:
         sku_parts: List[str] = [str(item.Defindex), str(int(item.Quality))]
```

