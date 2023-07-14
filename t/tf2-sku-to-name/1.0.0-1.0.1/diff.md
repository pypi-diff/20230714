# Comparing `tmp/tf2-sku-to-name-1.0.0.tar.gz` & `tmp/tf2-sku-to-name-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tf2-sku-to-name-1.0.0.tar", last modified: Fri Jul 14 14:51:08 2023, max compression
+gzip compressed data, was "tf2-sku-to-name-1.0.1.tar", last modified: Fri Jul 14 15:08:01 2023, max compression
```

## Comparing `tf2-sku-to-name-1.0.0.tar` & `tf2-sku-to-name-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxr-xr-x   0 ketan1     (502) staff       (20)        0 2023-07-14 14:51:08.590152 tf2-sku-to-name-1.0.0/
--rw-r--r--   0 ketan1     (502) staff       (20)     1070 2023-07-14 08:20:26.000000 tf2-sku-to-name-1.0.0/LICENSE
--rw-r--r--   0 ketan1     (502) staff       (20)      418 2023-07-14 14:51:08.590025 tf2-sku-to-name-1.0.0/PKG-INFO
--rw-r--r--   0 ketan1     (502) staff       (20)     1451 2023-07-14 14:46:41.000000 tf2-sku-to-name-1.0.0/README.md
--rw-r--r--   0 ketan1     (502) staff       (20)       38 2023-07-14 14:51:08.590197 tf2-sku-to-name-1.0.0/setup.cfg
--rw-r--r--   0 ketan1     (502) staff       (20)      568 2023-07-14 14:51:06.000000 tf2-sku-to-name-1.0.0/setup.py
-drwxr-xr-x   0 ketan1     (502) staff       (20)        0 2023-07-14 14:51:08.589837 tf2-sku-to-name-1.0.0/tf2_sku_to_name.egg-info/
--rw-r--r--   0 ketan1     (502) staff       (20)      418 2023-07-14 14:51:08.000000 tf2-sku-to-name-1.0.0/tf2_sku_to_name.egg-info/PKG-INFO
--rw-r--r--   0 ketan1     (502) staff       (20)      220 2023-07-14 14:51:08.000000 tf2-sku-to-name-1.0.0/tf2_sku_to_name.egg-info/SOURCES.txt
--rw-r--r--   0 ketan1     (502) staff       (20)        1 2023-07-14 14:51:08.000000 tf2-sku-to-name-1.0.0/tf2_sku_to_name.egg-info/dependency_links.txt
--rw-r--r--   0 ketan1     (502) staff       (20)       24 2023-07-14 14:51:08.000000 tf2-sku-to-name-1.0.0/tf2_sku_to_name.egg-info/requires.txt
--rw-r--r--   0 ketan1     (502) staff       (20)        1 2023-07-14 14:51:08.000000 tf2-sku-to-name-1.0.0/tf2_sku_to_name.egg-info/top_level.txt
+drwxr-xr-x   0 ketan1     (502) staff       (20)        0 2023-07-14 15:08:01.075055 tf2-sku-to-name-1.0.1/
+-rw-r--r--   0 ketan1     (502) staff       (20)     1070 2023-07-14 08:20:26.000000 tf2-sku-to-name-1.0.1/LICENSE
+-rw-r--r--   0 ketan1     (502) staff       (20)      418 2023-07-14 15:08:01.074942 tf2-sku-to-name-1.0.1/PKG-INFO
+-rw-r--r--   0 ketan1     (502) staff       (20)     1508 2023-07-14 14:53:36.000000 tf2-sku-to-name-1.0.1/README.md
+-rw-r--r--   0 ketan1     (502) staff       (20)       38 2023-07-14 15:08:01.075094 tf2-sku-to-name-1.0.1/setup.cfg
+-rw-r--r--   0 ketan1     (502) staff       (20)      560 2023-07-14 15:04:25.000000 tf2-sku-to-name-1.0.1/setup.py
+drwxr-xr-x   0 ketan1     (502) staff       (20)        0 2023-07-14 15:08:01.074129 tf2-sku-to-name-1.0.1/sku/
+-rw-r--r--   0 ketan1     (502) staff       (20)      668 2023-07-14 07:35:40.000000 tf2-sku-to-name-1.0.1/sku/models.py
+-rw-r--r--   0 ketan1     (502) staff       (20)     5144 2023-07-14 08:36:38.000000 tf2-sku-to-name-1.0.1/sku/parser.py
+drwxr-xr-x   0 ketan1     (502) staff       (20)        0 2023-07-14 15:08:01.074783 tf2-sku-to-name-1.0.1/tf2_sku_to_name.egg-info/
+-rw-r--r--   0 ketan1     (502) staff       (20)      418 2023-07-14 15:08:01.000000 tf2-sku-to-name-1.0.1/tf2_sku_to_name.egg-info/PKG-INFO
+-rw-r--r--   0 ketan1     (502) staff       (20)      248 2023-07-14 15:08:01.000000 tf2-sku-to-name-1.0.1/tf2_sku_to_name.egg-info/SOURCES.txt
+-rw-r--r--   0 ketan1     (502) staff       (20)        1 2023-07-14 15:08:01.000000 tf2-sku-to-name-1.0.1/tf2_sku_to_name.egg-info/dependency_links.txt
+-rw-r--r--   0 ketan1     (502) staff       (20)       24 2023-07-14 15:08:01.000000 tf2-sku-to-name-1.0.1/tf2_sku_to_name.egg-info/requires.txt
+-rw-r--r--   0 ketan1     (502) staff       (20)        4 2023-07-14 15:08:01.000000 tf2-sku-to-name-1.0.1/tf2_sku_to_name.egg-info/top_level.txt
```

### Comparing `tf2-sku-to-name-1.0.0/LICENSE` & `tf2-sku-to-name-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tf2-sku-to-name-1.0.0/README.md` & `tf2-sku-to-name-1.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -41,10 +41,15 @@
   "CraftNum": null,
   "CrateSn": null,
   "Output": null,
   "OutputQuality": null
 }
 ```
 
+## Installation
+```bash
+pip install tf2-sku-to-name
+```
+
 ## Acknowledgements
 [idinium96's tf2autobot](https://github.com/TF2Autobot/tf2autobot) for the item name schema\
 Inspired by [Nicklason's node-tf2-sku](https://github.com/Nicklason/node-tf2-sku) and [TryHardDo's TF2Sku](https://github.com/TryHardDo/TF2Sku/tree/master)
```

### Comparing `tf2-sku-to-name-1.0.0/setup.py` & `tf2-sku-to-name-1.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name='tf2-sku-to-name',
-    version='1.0.0',
+    version='1.0.1',
     author='Purple Barber',
     description="A python library that parses TF2 item SKU to the item's name and vice versa.",
     url='https://github.com/purplebarber/tf2-sku',
     license='MIT',
-    packages=find_packages(),
+    packages=["sku"],
     install_requires=[
         'requests',
         'beautifulsoup4'
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License'
```

