# Comparing `tmp/curatedmetagenomicdata3-0.1.0.tar.gz` & `tmp/curatedmetagenomicdata3-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/curatedmetagenomicdata3-0.1.0.tar", last modified: Thu Jul 13 21:53:00 2023, max compression
+gzip compressed data, was "dist/curatedmetagenomicdata3-0.1.1.tar", last modified: Thu Jul 13 21:59:17 2023, max compression
```

## Comparing `curatedmetagenomicdata3-0.1.0.tar` & `curatedmetagenomicdata3-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-13 21:53:00.000000 curatedmetagenomicdata3-0.1.0/
--rw-r--r--   0 saad      (1000) saad      (1000)     3078 2023-07-11 20:09:26.000000 curatedmetagenomicdata3-0.1.0/.gitignore
--rw-r--r--   0 saad      (1000) saad      (1000)     1066 2023-07-11 20:09:26.000000 curatedmetagenomicdata3-0.1.0/LICENSE
--rw-rw-r--   0 saad      (1000) saad      (1000)     1948 2023-07-13 21:53:00.000000 curatedmetagenomicdata3-0.1.0/PKG-INFO
--rw-r--r--   0 saad      (1000) saad      (1000)     1186 2023-07-13 21:49:28.000000 curatedmetagenomicdata3-0.1.0/README.md
-drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-13 21:53:00.000000 curatedmetagenomicdata3-0.1.0/curatedmetagenomicdata3/
--rw-rw-r--   0 saad      (1000) saad      (1000)     4590 2023-07-13 20:15:10.000000 curatedmetagenomicdata3-0.1.0/curatedmetagenomicdata3/__init__.py
-drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-13 21:53:00.000000 curatedmetagenomicdata3-0.1.0/curatedmetagenomicdata3.egg-info/
--rw-rw-r--   0 saad      (1000) saad      (1000)     1948 2023-07-13 21:53:00.000000 curatedmetagenomicdata3-0.1.0/curatedmetagenomicdata3.egg-info/PKG-INFO
--rw-rw-r--   0 saad      (1000) saad      (1000)      476 2023-07-13 21:53:00.000000 curatedmetagenomicdata3-0.1.0/curatedmetagenomicdata3.egg-info/SOURCES.txt
--rw-rw-r--   0 saad      (1000) saad      (1000)        1 2023-07-13 21:53:00.000000 curatedmetagenomicdata3-0.1.0/curatedmetagenomicdata3.egg-info/dependency_links.txt
--rw-rw-r--   0 saad      (1000) saad      (1000)       42 2023-07-13 21:53:00.000000 curatedmetagenomicdata3-0.1.0/curatedmetagenomicdata3.egg-info/requires.txt
--rw-rw-r--   0 saad      (1000) saad      (1000)       24 2023-07-13 21:53:00.000000 curatedmetagenomicdata3-0.1.0/curatedmetagenomicdata3.egg-info/top_level.txt
-drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-13 21:53:00.000000 curatedmetagenomicdata3-0.1.0/curatedmetagenomicdataextractor3/
--rw-r--r--   0 saad      (1000) saad      (1000)     1116 2022-11-06 20:47:24.000000 curatedmetagenomicdata3-0.1.0/curatedmetagenomicdataextractor3/README.md
-drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-13 21:53:00.000000 curatedmetagenomicdata3-0.1.0/curatedmetagenomicdataextractor3/download/
--rwxr-xr-x   0 saad      (1000) saad      (1000)     1043 2022-11-06 20:45:18.000000 curatedmetagenomicdata3-0.1.0/curatedmetagenomicdataextractor3/download/download_dataset.R
--rw-rw-r--   0 saad      (1000) saad      (1000)      788 2022-11-06 20:45:18.000000 curatedmetagenomicdata3-0.1.0/curatedmetagenomicdataextractor3/download/download_one_dataset.R
--rw-rw-r--   0 saad      (1000) saad      (1000)       38 2023-07-13 21:53:00.000000 curatedmetagenomicdata3-0.1.0/setup.cfg
--rw-rw-r--   0 saad      (1000) saad      (1000)      649 2023-07-13 21:24:58.000000 curatedmetagenomicdata3-0.1.0/setup.py
+drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-13 21:59:17.000000 curatedmetagenomicdata3-0.1.1/
+-rw-r--r--   0 saad      (1000) saad      (1000)     3078 2023-07-11 20:09:26.000000 curatedmetagenomicdata3-0.1.1/.gitignore
+-rw-r--r--   0 saad      (1000) saad      (1000)     1066 2023-07-11 20:09:26.000000 curatedmetagenomicdata3-0.1.1/LICENSE
+-rw-rw-r--   0 saad      (1000) saad      (1000)     1948 2023-07-13 21:59:17.000000 curatedmetagenomicdata3-0.1.1/PKG-INFO
+-rw-r--r--   0 saad      (1000) saad      (1000)     1186 2023-07-13 21:49:28.000000 curatedmetagenomicdata3-0.1.1/README.md
+drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-13 21:59:17.000000 curatedmetagenomicdata3-0.1.1/curatedmetagenomicdata3/
+-rw-rw-r--   0 saad      (1000) saad      (1000)     4590 2023-07-13 20:15:10.000000 curatedmetagenomicdata3-0.1.1/curatedmetagenomicdata3/__init__.py
+drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-13 21:59:17.000000 curatedmetagenomicdata3-0.1.1/curatedmetagenomicdata3.egg-info/
+-rw-rw-r--   0 saad      (1000) saad      (1000)     1948 2023-07-13 21:59:16.000000 curatedmetagenomicdata3-0.1.1/curatedmetagenomicdata3.egg-info/PKG-INFO
+-rw-rw-r--   0 saad      (1000) saad      (1000)      476 2023-07-13 21:59:17.000000 curatedmetagenomicdata3-0.1.1/curatedmetagenomicdata3.egg-info/SOURCES.txt
+-rw-rw-r--   0 saad      (1000) saad      (1000)        1 2023-07-13 21:59:16.000000 curatedmetagenomicdata3-0.1.1/curatedmetagenomicdata3.egg-info/dependency_links.txt
+-rw-rw-r--   0 saad      (1000) saad      (1000)       42 2023-07-13 21:59:16.000000 curatedmetagenomicdata3-0.1.1/curatedmetagenomicdata3.egg-info/requires.txt
+-rw-rw-r--   0 saad      (1000) saad      (1000)       24 2023-07-13 21:59:16.000000 curatedmetagenomicdata3-0.1.1/curatedmetagenomicdata3.egg-info/top_level.txt
+drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-13 21:59:17.000000 curatedmetagenomicdata3-0.1.1/curatedmetagenomicdataextractor3/
+-rw-r--r--   0 saad      (1000) saad      (1000)     1116 2022-11-06 20:47:24.000000 curatedmetagenomicdata3-0.1.1/curatedmetagenomicdataextractor3/README.md
+drwxrwxr-x   0 saad      (1000) saad      (1000)        0 2023-07-13 21:59:17.000000 curatedmetagenomicdata3-0.1.1/curatedmetagenomicdataextractor3/download/
+-rwxr-xr-x   0 saad      (1000) saad      (1000)     1043 2022-11-06 20:45:18.000000 curatedmetagenomicdata3-0.1.1/curatedmetagenomicdataextractor3/download/download_dataset.R
+-rw-rw-r--   0 saad      (1000) saad      (1000)      788 2022-11-06 20:45:18.000000 curatedmetagenomicdata3-0.1.1/curatedmetagenomicdataextractor3/download/download_one_dataset.R
+-rw-rw-r--   0 saad      (1000) saad      (1000)       38 2023-07-13 21:59:17.000000 curatedmetagenomicdata3-0.1.1/setup.cfg
+-rw-rw-r--   0 saad      (1000) saad      (1000)      649 2023-07-13 21:59:10.000000 curatedmetagenomicdata3-0.1.1/setup.py
```

### Comparing `curatedmetagenomicdata3-0.1.0/.gitignore` & `curatedmetagenomicdata3-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `curatedmetagenomicdata3-0.1.0/LICENSE` & `curatedmetagenomicdata3-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `curatedmetagenomicdata3-0.1.0/PKG-INFO` & `curatedmetagenomicdata3-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: curatedmetagenomicdata3
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python wrapper for curatedMetagenomicData3.
 Home-page: https://github.com/kellylab/curatedmetagenomidata3-python
 Author: UNKNOWN
 Author-email: skhan8@mail.einstein.yu.edu
 License: UNKNOWN
 Description: # curatedMetagenomicData3-python
```

### Comparing `curatedmetagenomicdata3-0.1.0/README.md` & `curatedmetagenomicdata3-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `curatedmetagenomicdata3-0.1.0/curatedmetagenomicdata3/__init__.py` & `curatedmetagenomicdata3-0.1.1/curatedmetagenomicdata3/__init__.py`

 * *Files identical despite different names*

### Comparing `curatedmetagenomicdata3-0.1.0/curatedmetagenomicdata3.egg-info/PKG-INFO` & `curatedmetagenomicdata3-0.1.1/curatedmetagenomicdata3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: curatedmetagenomicdata3
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python wrapper for curatedMetagenomicData3.
 Home-page: https://github.com/kellylab/curatedmetagenomidata3-python
 Author: UNKNOWN
 Author-email: skhan8@mail.einstein.yu.edu
 License: UNKNOWN
 Description: # curatedMetagenomicData3-python
```

### Comparing `curatedmetagenomicdata3-0.1.0/curatedmetagenomicdataextractor3/README.md` & `curatedmetagenomicdata3-0.1.1/curatedmetagenomicdataextractor3/README.md`

 * *Files identical despite different names*

### Comparing `curatedmetagenomicdata3-0.1.0/curatedmetagenomicdataextractor3/download/download_dataset.R` & `curatedmetagenomicdata3-0.1.1/curatedmetagenomicdataextractor3/download/download_dataset.R`

 * *Files identical despite different names*

### Comparing `curatedmetagenomicdata3-0.1.0/curatedmetagenomicdataextractor3/download/download_one_dataset.R` & `curatedmetagenomicdata3-0.1.1/curatedmetagenomicdataextractor3/download/download_one_dataset.R`

 * *Files identical despite different names*

### Comparing `curatedmetagenomicdata3-0.1.0/setup.py` & `curatedmetagenomicdata3-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='curatedmetagenomicdata3',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
     author_email="skhan8@mail.einstein.yu.edu",
     description="Python wrapper for curatedMetagenomicData3.",
     long_description=open('README.md').read(),
     url="https://github.com/kellylab/curatedmetagenomidata3-python",
     install_requires=requirements,
     classifiers=[
```

