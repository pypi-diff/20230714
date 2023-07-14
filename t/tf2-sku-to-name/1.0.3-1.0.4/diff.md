# Comparing `tmp/tf2-sku-to-name-1.0.3.tar.gz` & `tmp/tf2-sku-to-name-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tf2-sku-to-name-1.0.3.tar", last modified: Fri Jul 14 15:22:36 2023, max compression
+gzip compressed data, was "tf2-sku-to-name-1.0.4.tar", last modified: Fri Jul 14 15:25:33 2023, max compression
```

## Comparing `tf2-sku-to-name-1.0.3.tar` & `tf2-sku-to-name-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 ketan1     (502) staff       (20)        0 2023-07-14 15:22:36.998666 tf2-sku-to-name-1.0.3/
--rw-r--r--   0 ketan1     (502) staff       (20)     1070 2023-07-14 08:20:26.000000 tf2-sku-to-name-1.0.3/LICENSE
--rw-r--r--   0 ketan1     (502) staff       (20)      418 2023-07-14 15:22:36.998307 tf2-sku-to-name-1.0.3/PKG-INFO
--rw-r--r--   0 ketan1     (502) staff       (20)     1508 2023-07-14 14:53:36.000000 tf2-sku-to-name-1.0.3/README.md
--rw-r--r--   0 ketan1     (502) staff       (20)       38 2023-07-14 15:22:36.998729 tf2-sku-to-name-1.0.3/setup.cfg
--rw-r--r--   0 ketan1     (502) staff       (20)      633 2023-07-14 15:22:28.000000 tf2-sku-to-name-1.0.3/setup.py
-drwxr-xr-x   0 ketan1     (502) staff       (20)        0 2023-07-14 15:22:36.995999 tf2-sku-to-name-1.0.3/sku/
--rw-r--r--   0 ketan1     (502) staff       (20)      668 2023-07-14 07:35:40.000000 tf2-sku-to-name-1.0.3/sku/models.py
--rw-r--r--   0 ketan1     (502) staff       (20)     5204 2023-07-14 15:20:38.000000 tf2-sku-to-name-1.0.3/sku/parser.py
-drwxr-xr-x   0 ketan1     (502) staff       (20)        0 2023-07-14 15:22:36.997897 tf2-sku-to-name-1.0.3/tf2_sku_to_name.egg-info/
--rw-r--r--   0 ketan1     (502) staff       (20)      418 2023-07-14 15:22:36.000000 tf2-sku-to-name-1.0.3/tf2_sku_to_name.egg-info/PKG-INFO
--rw-r--r--   0 ketan1     (502) staff       (20)      248 2023-07-14 15:22:36.000000 tf2-sku-to-name-1.0.3/tf2_sku_to_name.egg-info/SOURCES.txt
--rw-r--r--   0 ketan1     (502) staff       (20)        1 2023-07-14 15:22:36.000000 tf2-sku-to-name-1.0.3/tf2_sku_to_name.egg-info/dependency_links.txt
--rw-r--r--   0 ketan1     (502) staff       (20)       24 2023-07-14 15:22:36.000000 tf2-sku-to-name-1.0.3/tf2_sku_to_name.egg-info/requires.txt
--rw-r--r--   0 ketan1     (502) staff       (20)        4 2023-07-14 15:22:36.000000 tf2-sku-to-name-1.0.3/tf2_sku_to_name.egg-info/top_level.txt
+drwxr-xr-x   0 ketan1     (502) staff       (20)        0 2023-07-14 15:25:33.001724 tf2-sku-to-name-1.0.4/
+-rw-r--r--   0 ketan1     (502) staff       (20)     1070 2023-07-14 08:20:26.000000 tf2-sku-to-name-1.0.4/LICENSE
+-rw-r--r--   0 ketan1     (502) staff       (20)      418 2023-07-14 15:25:33.001602 tf2-sku-to-name-1.0.4/PKG-INFO
+-rw-r--r--   0 ketan1     (502) staff       (20)     1508 2023-07-14 14:53:36.000000 tf2-sku-to-name-1.0.4/README.md
+-rw-r--r--   0 ketan1     (502) staff       (20)       38 2023-07-14 15:25:33.001764 tf2-sku-to-name-1.0.4/setup.cfg
+-rw-r--r--   0 ketan1     (502) staff       (20)      621 2023-07-14 15:25:28.000000 tf2-sku-to-name-1.0.4/setup.py
+drwxr-xr-x   0 ketan1     (502) staff       (20)        0 2023-07-14 15:25:32.998936 tf2-sku-to-name-1.0.4/sku/
+drwxr-xr-x   0 ketan1     (502) staff       (20)        0 2023-07-14 15:25:32.999045 tf2-sku-to-name-1.0.4/sku/data/
+-rw-r--r--   0 ketan1     (502) staff       (20)  3849421 2023-07-14 15:22:12.000000 tf2-sku-to-name-1.0.4/sku/data/data.json
+-rw-r--r--   0 ketan1     (502) staff       (20)      668 2023-07-14 07:35:40.000000 tf2-sku-to-name-1.0.4/sku/models.py
+-rw-r--r--   0 ketan1     (502) staff       (20)     5204 2023-07-14 15:20:38.000000 tf2-sku-to-name-1.0.4/sku/parser.py
+drwxr-xr-x   0 ketan1     (502) staff       (20)        0 2023-07-14 15:25:33.001410 tf2-sku-to-name-1.0.4/tf2_sku_to_name.egg-info/
+-rw-r--r--   0 ketan1     (502) staff       (20)      418 2023-07-14 15:25:32.000000 tf2-sku-to-name-1.0.4/tf2_sku_to_name.egg-info/PKG-INFO
+-rw-r--r--   0 ketan1     (502) staff       (20)      267 2023-07-14 15:25:32.000000 tf2-sku-to-name-1.0.4/tf2_sku_to_name.egg-info/SOURCES.txt
+-rw-r--r--   0 ketan1     (502) staff       (20)        1 2023-07-14 15:25:32.000000 tf2-sku-to-name-1.0.4/tf2_sku_to_name.egg-info/dependency_links.txt
+-rw-r--r--   0 ketan1     (502) staff       (20)       24 2023-07-14 15:25:32.000000 tf2-sku-to-name-1.0.4/tf2_sku_to_name.egg-info/requires.txt
+-rw-r--r--   0 ketan1     (502) staff       (20)        4 2023-07-14 15:25:32.000000 tf2-sku-to-name-1.0.4/tf2_sku_to_name.egg-info/top_level.txt
```

### Comparing `tf2-sku-to-name-1.0.3/LICENSE` & `tf2-sku-to-name-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tf2-sku-to-name-1.0.3/README.md` & `tf2-sku-to-name-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `tf2-sku-to-name-1.0.3/setup.py` & `tf2-sku-to-name-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='tf2-sku-to-name',
-    version='1.0.3',
+    version='1.0.4',
     author='Purple Barber',
     description="A python library that parses TF2 item SKU to the item's name and vice versa.",
     url='https://github.com/purplebarber/tf2-sku',
     license='MIT',
     packages=["sku"],
     package_data={
-        'tf2-sku-to-name': ['data/data.json'],
+        'sku': ['data/data.json'],
     },
     install_requires=[
         'requests',
         'beautifulsoup4'
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `tf2-sku-to-name-1.0.3/sku/models.py` & `tf2-sku-to-name-1.0.4/sku/models.py`

 * *Files identical despite different names*

### Comparing `tf2-sku-to-name-1.0.3/sku/parser.py` & `tf2-sku-to-name-1.0.4/sku/parser.py`

 * *Files identical despite different names*

