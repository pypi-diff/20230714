# Comparing `tmp/pathgenmap-0.0.3.tar.gz` & `tmp/pathgenmap-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathgenmap-0.0.3.tar", last modified: Thu Jul 13 21:57:32 2023, max compression
+gzip compressed data, was "pathgenmap-0.0.4.tar", last modified: Thu Jul 13 23:37:18 2023, max compression
```

## Comparing `pathgenmap-0.0.3.tar` & `pathgenmap-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-13 21:57:32.610142 pathgenmap-0.0.3/
--rw-r--r--   0 marcossousa   (501) staff       (20)     1083 2023-07-13 00:05:25.000000 pathgenmap-0.0.3/LICENSE
--rw-r--r--   0 marcossousa   (501) staff       (20)      422 2023-07-13 21:57:32.609322 pathgenmap-0.0.3/PKG-INFO
--rw-r--r--   0 marcossousa   (501) staff       (20)      740 2023-07-13 21:56:31.000000 pathgenmap-0.0.3/README.md
-drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-13 21:57:32.602739 pathgenmap-0.0.3/pathgenmap/
--rw-r--r--   0 marcossousa   (501) staff       (20)     1307 2023-07-13 00:07:52.000000 pathgenmap-0.0.3/pathgenmap/EggAnnot.py
--rw-r--r--   0 marcossousa   (501) staff       (20)     3011 2023-07-13 13:17:10.000000 pathgenmap-0.0.3/pathgenmap/Integration.py
--rw-r--r--   0 marcossousa   (501) staff       (20)     1889 2023-07-13 11:28:07.000000 pathgenmap-0.0.3/pathgenmap/PathAnalys.py
--rw-r--r--   0 marcossousa   (501) staff       (20)     1139 2023-07-13 13:17:10.000000 pathgenmap-0.0.3/pathgenmap/PathGenMap.py
--rw-r--r--   0 marcossousa   (501) staff       (20)     1205 2023-07-13 11:46:42.000000 pathgenmap-0.0.3/pathgenmap/SpeciesAbundance.py
--rw-r--r--   0 marcossousa   (501) staff       (20)        0 2023-07-13 00:03:39.000000 pathgenmap-0.0.3/pathgenmap/__init__.py
-drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-13 21:57:32.608199 pathgenmap-0.0.3/pathgenmap.egg-info/
--rw-r--r--   0 marcossousa   (501) staff       (20)      422 2023-07-13 21:57:32.000000 pathgenmap-0.0.3/pathgenmap.egg-info/PKG-INFO
--rw-r--r--   0 marcossousa   (501) staff       (20)      348 2023-07-13 21:57:32.000000 pathgenmap-0.0.3/pathgenmap.egg-info/SOURCES.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)        1 2023-07-13 21:57:32.000000 pathgenmap-0.0.3/pathgenmap.egg-info/dependency_links.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       27 2023-07-13 21:57:32.000000 pathgenmap-0.0.3/pathgenmap.egg-info/requires.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       11 2023-07-13 21:57:32.000000 pathgenmap-0.0.3/pathgenmap.egg-info/top_level.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       38 2023-07-13 21:57:32.610456 pathgenmap-0.0.3/setup.cfg
--rw-r--r--   0 marcossousa   (501) staff       (20)      570 2023-07-13 21:57:06.000000 pathgenmap-0.0.3/setup.py
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-13 23:37:18.726168 pathgenmap-0.0.4/
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1083 2023-07-13 00:05:25.000000 pathgenmap-0.0.4/LICENSE
+-rw-r--r--   0 marcossousa   (501) staff       (20)      422 2023-07-13 23:37:18.724546 pathgenmap-0.0.4/PKG-INFO
+-rw-r--r--   0 marcossousa   (501) staff       (20)      740 2023-07-13 21:56:31.000000 pathgenmap-0.0.4/README.md
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-13 23:37:18.717040 pathgenmap-0.0.4/pathgenmap/
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1307 2023-07-13 00:07:52.000000 pathgenmap-0.0.4/pathgenmap/EggAnnot.py
+-rw-r--r--   0 marcossousa   (501) staff       (20)     3011 2023-07-13 13:17:10.000000 pathgenmap-0.0.4/pathgenmap/Integration.py
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1889 2023-07-13 11:28:07.000000 pathgenmap-0.0.4/pathgenmap/PathAnalys.py
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1139 2023-07-13 13:17:10.000000 pathgenmap-0.0.4/pathgenmap/PathGenMap.py
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1205 2023-07-13 11:46:42.000000 pathgenmap-0.0.4/pathgenmap/SpeciesAbundance.py
+-rw-r--r--   0 marcossousa   (501) staff       (20)        0 2023-07-13 00:03:39.000000 pathgenmap-0.0.4/pathgenmap/__init__.py
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-13 23:37:18.722914 pathgenmap-0.0.4/pathgenmap.egg-info/
+-rw-r--r--   0 marcossousa   (501) staff       (20)      422 2023-07-13 23:37:18.000000 pathgenmap-0.0.4/pathgenmap.egg-info/PKG-INFO
+-rw-r--r--   0 marcossousa   (501) staff       (20)      348 2023-07-13 23:37:18.000000 pathgenmap-0.0.4/pathgenmap.egg-info/SOURCES.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)        1 2023-07-13 23:37:18.000000 pathgenmap-0.0.4/pathgenmap.egg-info/dependency_links.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       27 2023-07-13 23:37:18.000000 pathgenmap-0.0.4/pathgenmap.egg-info/requires.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       11 2023-07-13 23:37:18.000000 pathgenmap-0.0.4/pathgenmap.egg-info/top_level.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       38 2023-07-13 23:37:18.726480 pathgenmap-0.0.4/setup.cfg
+-rw-r--r--   0 marcossousa   (501) staff       (20)      570 2023-07-13 23:34:56.000000 pathgenmap-0.0.4/setup.py
```

### Comparing `pathgenmap-0.0.3/LICENSE` & `pathgenmap-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pathgenmap-0.0.3/README.md` & `pathgenmap-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pathgenmap-0.0.3/pathgenmap/EggAnnot.py` & `pathgenmap-0.0.4/pathgenmap/EggAnnot.py`

 * *Files identical despite different names*

### Comparing `pathgenmap-0.0.3/pathgenmap/Integration.py` & `pathgenmap-0.0.4/pathgenmap/Integration.py`

 * *Files identical despite different names*

### Comparing `pathgenmap-0.0.3/pathgenmap/PathAnalys.py` & `pathgenmap-0.0.4/pathgenmap/PathAnalys.py`

 * *Files identical despite different names*

### Comparing `pathgenmap-0.0.3/pathgenmap/PathGenMap.py` & `pathgenmap-0.0.4/pathgenmap/PathGenMap.py`

 * *Files identical despite different names*

### Comparing `pathgenmap-0.0.3/pathgenmap/SpeciesAbundance.py` & `pathgenmap-0.0.4/pathgenmap/SpeciesAbundance.py`

 * *Files identical despite different names*

### Comparing `pathgenmap-0.0.3/setup.py` & `pathgenmap-0.0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pathgenmap",
-    version="0.0.3",
+    version="0.0.4",
     packages=find_packages(),
     scripts=["PathGenMap.py"],
 
     install_requires=["pandas>=1.1.0", "tqdm>=4.48.0"],
     author="Marcos Paulo Alves de Sousa",
     author_email="msousa@museu-goeldi.br",
     description="PathGenMap is a comprehensive Python application designed to integrate pathway, annotation, and species abundance data.",
```

