# Comparing `tmp/curatedmetagenomicdata3-0.1.2.tar.gz` & `tmp/curatedmetagenomicdata3-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/curatedmetagenomicdata3-0.1.2.tar", last modified: Thu Jul 13 22:14:07 2023, max compression
+gzip compressed data, was "dist/curatedmetagenomicdata3-0.1.3.tar", last modified: Thu Jul 13 22:22:16 2023, max compression
```

## Comparing `curatedmetagenomicdata3-0.1.2.tar` & `curatedmetagenomicdata3-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-13 22:14:07.000000 curatedmetagenomicdata3-0.1.2/
--rw-r--r--   0 saad      (1000) saad      (1000)     3078 2023-07-11 20:09:26.000000 curatedmetagenomicdata3-0.1.2/.gitignore
--rw-r--r--   0 saad      (1000) saad      (1000)     1066 2023-07-11 20:09:26.000000 curatedmetagenomicdata3-0.1.2/LICENSE
--rw-rw-r--   0 saad      (1000) saad      (1000)       75 2023-07-13 22:05:34.000000 curatedmetagenomicdata3-0.1.2/MANIFEST.in
--rw-rw-r--   0 saad      (1000) saad      (1000)     1948 2023-07-13 22:14:07.000000 curatedmetagenomicdata3-0.1.2/PKG-INFO
--rw-r--r--   0 saad      (1000) saad      (1000)     1186 2023-07-13 21:49:28.000000 curatedmetagenomicdata3-0.1.2/README.md
-drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-13 22:14:07.000000 curatedmetagenomicdata3-0.1.2/curatedmetagenomicdata3/
--rw-rw-r--   0 saad      (1000) saad      (1000)     4590 2023-07-13 20:15:10.000000 curatedmetagenomicdata3-0.1.2/curatedmetagenomicdata3/__init__.py
-drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-13 22:14:07.000000 curatedmetagenomicdata3-0.1.2/curatedmetagenomicdata3.egg-info/
--rw-rw-r--   0 saad      (1000) saad      (1000)     1948 2023-07-13 22:14:07.000000 curatedmetagenomicdata3-0.1.2/curatedmetagenomicdata3.egg-info/PKG-INFO
--rw-rw-r--   0 saad      (1000) saad      (1000)      505 2023-07-13 22:14:07.000000 curatedmetagenomicdata3-0.1.2/curatedmetagenomicdata3.egg-info/SOURCES.txt
--rw-rw-r--   0 saad      (1000) saad      (1000)        1 2023-07-13 22:14:07.000000 curatedmetagenomicdata3-0.1.2/curatedmetagenomicdata3.egg-info/dependency_links.txt
--rw-rw-r--   0 saad      (1000) saad      (1000)       42 2023-07-13 22:14:07.000000 curatedmetagenomicdata3-0.1.2/curatedmetagenomicdata3.egg-info/requires.txt
--rw-rw-r--   0 saad      (1000) saad      (1000)       24 2023-07-13 22:14:07.000000 curatedmetagenomicdata3-0.1.2/curatedmetagenomicdata3.egg-info/top_level.txt
-drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-13 22:14:07.000000 curatedmetagenomicdata3-0.1.2/curatedmetagenomicdataextractor3/
--rw-r--r--   0 saad      (1000) saad      (1000)     1116 2022-11-06 20:47:24.000000 curatedmetagenomicdata3-0.1.2/curatedmetagenomicdataextractor3/README.md
-drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-13 22:14:07.000000 curatedmetagenomicdata3-0.1.2/curatedmetagenomicdataextractor3/download/
--rwxr-xr-x   0 saad      (1000) saad      (1000)     1043 2022-11-06 20:45:18.000000 curatedmetagenomicdata3-0.1.2/curatedmetagenomicdataextractor3/download/download_dataset.R
--rw-rw-r--   0 saad      (1000) saad      (1000)      788 2022-11-06 20:45:18.000000 curatedmetagenomicdata3-0.1.2/curatedmetagenomicdataextractor3/download/download_one_dataset.R
--rw-rw-r--   0 saad      (1000) saad      (1000)       41 2023-07-13 21:52:41.000000 curatedmetagenomicdata3-0.1.2/requirements.txt
--rw-rw-r--   0 saad      (1000) saad      (1000)       38 2023-07-13 22:14:07.000000 curatedmetagenomicdata3-0.1.2/setup.cfg
--rw-rw-r--   0 saad      (1000) saad      (1000)      717 2023-07-13 22:13:59.000000 curatedmetagenomicdata3-0.1.2/setup.py
+drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-13 22:22:16.000000 curatedmetagenomicdata3-0.1.3/
+-rw-r--r--   0 saad      (1000) saad      (1000)     3078 2023-07-11 20:09:26.000000 curatedmetagenomicdata3-0.1.3/.gitignore
+-rw-r--r--   0 saad      (1000) saad      (1000)     1066 2023-07-11 20:09:26.000000 curatedmetagenomicdata3-0.1.3/LICENSE
+-rw-rw-r--   0 saad      (1000) saad      (1000)      185 2023-07-13 22:21:20.000000 curatedmetagenomicdata3-0.1.3/MANIFEST.in
+-rw-rw-r--   0 saad      (1000) saad      (1000)     1948 2023-07-13 22:22:16.000000 curatedmetagenomicdata3-0.1.3/PKG-INFO
+-rw-r--r--   0 saad      (1000) saad      (1000)     1186 2023-07-13 21:49:28.000000 curatedmetagenomicdata3-0.1.3/README.md
+drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-13 22:22:16.000000 curatedmetagenomicdata3-0.1.3/curatedmetagenomicdata3/
+-rw-rw-r--   0 saad      (1000) saad      (1000)     4590 2023-07-13 20:15:10.000000 curatedmetagenomicdata3-0.1.3/curatedmetagenomicdata3/__init__.py
+drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-13 22:22:16.000000 curatedmetagenomicdata3-0.1.3/curatedmetagenomicdata3/assets/
+-rw-rw-r--   0 saad      (1000) saad      (1000) 17080410 2022-11-20 19:38:13.000000 curatedmetagenomicdata3-0.1.3/curatedmetagenomicdata3/assets/pathways.csv
+-rw-rw-r--   0 saad      (1000) saad      (1000) 23731776 2023-07-13 20:10:30.000000 curatedmetagenomicdata3-0.1.3/curatedmetagenomicdata3/assets/sampleMetadata.pickle
+-rw-rw-r--   0 saad      (1000) saad      (1000)   261689 2022-11-18 04:47:38.000000 curatedmetagenomicdata3-0.1.3/curatedmetagenomicdata3/assets/taxa.txt
+drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-13 22:22:16.000000 curatedmetagenomicdata3-0.1.3/curatedmetagenomicdata3.egg-info/
+-rw-rw-r--   0 saad      (1000) saad      (1000)     1948 2023-07-13 22:22:16.000000 curatedmetagenomicdata3-0.1.3/curatedmetagenomicdata3.egg-info/PKG-INFO
+-rw-rw-r--   0 saad      (1000) saad      (1000)      642 2023-07-13 22:22:16.000000 curatedmetagenomicdata3-0.1.3/curatedmetagenomicdata3.egg-info/SOURCES.txt
+-rw-rw-r--   0 saad      (1000) saad      (1000)        1 2023-07-13 22:22:16.000000 curatedmetagenomicdata3-0.1.3/curatedmetagenomicdata3.egg-info/dependency_links.txt
+-rw-rw-r--   0 saad      (1000) saad      (1000)       42 2023-07-13 22:22:16.000000 curatedmetagenomicdata3-0.1.3/curatedmetagenomicdata3.egg-info/requires.txt
+-rw-rw-r--   0 saad      (1000) saad      (1000)       24 2023-07-13 22:22:16.000000 curatedmetagenomicdata3-0.1.3/curatedmetagenomicdata3.egg-info/top_level.txt
+drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-13 22:22:16.000000 curatedmetagenomicdata3-0.1.3/curatedmetagenomicdataextractor3/
+-rw-r--r--   0 saad      (1000) saad      (1000)     1116 2022-11-06 20:47:24.000000 curatedmetagenomicdata3-0.1.3/curatedmetagenomicdataextractor3/README.md
+drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-13 22:22:16.000000 curatedmetagenomicdata3-0.1.3/curatedmetagenomicdataextractor3/download/
+-rwxr-xr-x   0 saad      (1000) saad      (1000)     1043 2022-11-06 20:45:18.000000 curatedmetagenomicdata3-0.1.3/curatedmetagenomicdataextractor3/download/download_dataset.R
+-rw-rw-r--   0 saad      (1000) saad      (1000)      788 2022-11-06 20:45:18.000000 curatedmetagenomicdata3-0.1.3/curatedmetagenomicdataextractor3/download/download_one_dataset.R
+-rw-rw-r--   0 saad      (1000) saad      (1000)       41 2023-07-13 21:52:41.000000 curatedmetagenomicdata3-0.1.3/requirements.txt
+-rw-rw-r--   0 saad      (1000) saad      (1000)       38 2023-07-13 22:22:16.000000 curatedmetagenomicdata3-0.1.3/setup.cfg
+-rw-rw-r--   0 saad      (1000) saad      (1000)      717 2023-07-13 22:22:11.000000 curatedmetagenomicdata3-0.1.3/setup.py
```

### Comparing `curatedmetagenomicdata3-0.1.2/.gitignore` & `curatedmetagenomicdata3-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `curatedmetagenomicdata3-0.1.2/LICENSE` & `curatedmetagenomicdata3-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `curatedmetagenomicdata3-0.1.2/PKG-INFO` & `curatedmetagenomicdata3-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: curatedmetagenomicdata3
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python wrapper for curatedMetagenomicData3.
 Home-page: https://github.com/kellylab/curatedmetagenomidata3-python
 Author: UNKNOWN
 Author-email: skhan8@mail.einstein.yu.edu
 License: UNKNOWN
 Description: # curatedMetagenomicData3-python
```

### Comparing `curatedmetagenomicdata3-0.1.2/README.md` & `curatedmetagenomicdata3-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `curatedmetagenomicdata3-0.1.2/curatedmetagenomicdata3/__init__.py` & `curatedmetagenomicdata3-0.1.3/curatedmetagenomicdata3/__init__.py`

 * *Files identical despite different names*

### Comparing `curatedmetagenomicdata3-0.1.2/curatedmetagenomicdata3.egg-info/PKG-INFO` & `curatedmetagenomicdata3-0.1.3/curatedmetagenomicdata3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: curatedmetagenomicdata3
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python wrapper for curatedMetagenomicData3.
 Home-page: https://github.com/kellylab/curatedmetagenomidata3-python
 Author: UNKNOWN
 Author-email: skhan8@mail.einstein.yu.edu
 License: UNKNOWN
 Description: # curatedMetagenomicData3-python
```

### Comparing `curatedmetagenomicdata3-0.1.2/curatedmetagenomicdataextractor3/README.md` & `curatedmetagenomicdata3-0.1.3/curatedmetagenomicdataextractor3/README.md`

 * *Files identical despite different names*

### Comparing `curatedmetagenomicdata3-0.1.2/curatedmetagenomicdataextractor3/download/download_dataset.R` & `curatedmetagenomicdata3-0.1.3/curatedmetagenomicdataextractor3/download/download_dataset.R`

 * *Files identical despite different names*

### Comparing `curatedmetagenomicdata3-0.1.2/curatedmetagenomicdataextractor3/download/download_one_dataset.R` & `curatedmetagenomicdata3-0.1.3/curatedmetagenomicdataextractor3/download/download_one_dataset.R`

 * *Files identical despite different names*

### Comparing `curatedmetagenomicdata3-0.1.2/setup.py` & `curatedmetagenomicdata3-0.1.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='curatedmetagenomicdata3',
-    version='0.1.2',
+    version='0.1.3',
     packages=find_packages(),
     author_email="skhan8@mail.einstein.yu.edu",
     description="Python wrapper for curatedMetagenomicData3.",
     long_description=open('README.md').read(),
     url="https://github.com/kellylab/curatedmetagenomidata3-python",
     install_requires=requirements,
     include_package_data=True,
```

