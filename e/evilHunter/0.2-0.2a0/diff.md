# Comparing `tmp/evilHunter-0.2.tar.gz` & `tmp/evilHunter-0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evilHunter-0.2.tar", last modified: Fri Jul 14 14:31:41 2023, max compression
+gzip compressed data, was "evilHunter-0.2a0.tar", last modified: Fri Jul 14 14:30:56 2023, max compression
```

## Comparing `evilHunter-0.2.tar` & `evilHunter-0.2a0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-07-14 14:31:41.731982 evilHunter-0.2/
-drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-07-14 14:31:41.731982 evilHunter-0.2/C/
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)     7467 2023-07-14 14:25:30.000000 evilHunter-0.2/C/evilCracker.c
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)     3583 2023-07-14 14:31:41.731982 evilHunter-0.2/PKG-INFO
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)     3355 2023-07-14 14:26:38.000000 evilHunter-0.2/README.md
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)     4127 2023-07-12 16:38:26.000000 evilHunter-0.2/evilCracker.py
-drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-07-14 14:31:41.731982 evilHunter-0.2/evilHunter.egg-info/
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)     3583 2023-07-14 14:31:41.000000 evilHunter-0.2/evilHunter.egg-info/PKG-INFO
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)      232 2023-07-14 14:31:41.000000 evilHunter-0.2/evilHunter.egg-info/SOURCES.txt
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)        1 2023-07-14 14:31:41.000000 evilHunter-0.2/evilHunter.egg-info/dependency_links.txt
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)       14 2023-07-14 14:31:41.000000 evilHunter-0.2/evilHunter.egg-info/requires.txt
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)        8 2023-07-14 14:31:41.000000 evilHunter-0.2/evilHunter.egg-info/top_level.txt
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)    34010 2023-07-14 14:24:21.000000 evilHunter-0.2/evilHunter.py
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)       38 2023-07-14 14:31:41.731982 evilHunter-0.2/setup.cfg
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)      589 2023-07-14 14:31:31.000000 evilHunter-0.2/setup.py
+drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-07-14 14:30:56.328653 evilHunter-0.2a0/
+drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-07-14 14:30:56.324653 evilHunter-0.2a0/C/
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)     7467 2023-07-14 14:25:30.000000 evilHunter-0.2a0/C/evilCracker.c
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)     3585 2023-07-14 14:30:56.328653 evilHunter-0.2a0/PKG-INFO
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)     3355 2023-07-14 14:26:38.000000 evilHunter-0.2a0/README.md
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)     4127 2023-07-12 16:38:26.000000 evilHunter-0.2a0/evilCracker.py
+drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-07-14 14:30:56.328653 evilHunter-0.2a0/evilHunter.egg-info/
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)     3585 2023-07-14 14:30:56.000000 evilHunter-0.2a0/evilHunter.egg-info/PKG-INFO
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)      232 2023-07-14 14:30:56.000000 evilHunter-0.2a0/evilHunter.egg-info/SOURCES.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)        1 2023-07-14 14:30:56.000000 evilHunter-0.2a0/evilHunter.egg-info/dependency_links.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)       14 2023-07-14 14:30:56.000000 evilHunter-0.2a0/evilHunter.egg-info/requires.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)        8 2023-07-14 14:30:56.000000 evilHunter-0.2a0/evilHunter.egg-info/top_level.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)    34010 2023-07-14 14:24:21.000000 evilHunter-0.2a0/evilHunter.py
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)       38 2023-07-14 14:30:56.328653 evilHunter-0.2a0/setup.cfg
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)      590 2023-07-14 14:09:14.000000 evilHunter-0.2a0/setup.py
```

### Comparing `evilHunter-0.2/C/evilCracker.c` & `evilHunter-0.2a0/C/evilCracker.c`

 * *Files identical despite different names*

### Comparing `evilHunter-0.2/PKG-INFO` & `evilHunter-0.2a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evilHunter
-Version: 0.2
+Version: 0.2a0
 Summary: Cracking WiFi(KCRACK)
 Home-page: https://github.com/an0mal1a/evilHunter
 Author: an0mal1a
 Author-email: pablodiez024@proton.me
 Description-Content-Type: text/markdown
 
 # evilHunter
```

### Comparing `evilHunter-0.2/README.md` & `evilHunter-0.2a0/README.md`

 * *Files identical despite different names*

### Comparing `evilHunter-0.2/evilCracker.py` & `evilHunter-0.2a0/evilCracker.py`

 * *Files identical despite different names*

### Comparing `evilHunter-0.2/evilHunter.egg-info/PKG-INFO` & `evilHunter-0.2a0/evilHunter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evilHunter
-Version: 0.2
+Version: 0.2a0
 Summary: Cracking WiFi(KCRACK)
 Home-page: https://github.com/an0mal1a/evilHunter
 Author: an0mal1a
 Author-email: pablodiez024@proton.me
 Description-Content-Type: text/markdown
 
 # evilHunter
```

### Comparing `evilHunter-0.2/evilHunter.py` & `evilHunter-0.2a0/evilHunter.py`

 * *Files identical despite different names*

### Comparing `evilHunter-0.2/setup.py` & `evilHunter-0.2a0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, Extension
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="evilHunter",
-    version="0.2",
+    version="0.2a",
     description="Cracking WiFi(KCRACK)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="an0mal1a",
     url="https://github.com/an0mal1a/evilHunter",
     author_email="pablodiez024@proton.me",
     packages=["words", "C"],
```

