# Comparing `tmp/pathgenmap-0.0.4.tar.gz` & `tmp/pathgenmap-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathgenmap-0.0.4.tar", last modified: Thu Jul 13 23:37:18 2023, max compression
+gzip compressed data, was "pathgenmap-0.0.6.tar", last modified: Thu Jul 13 23:48:32 2023, max compression
```

## Comparing `pathgenmap-0.0.4.tar` & `pathgenmap-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-13 23:37:18.726168 pathgenmap-0.0.4/
--rw-r--r--   0 marcossousa   (501) staff       (20)     1083 2023-07-13 00:05:25.000000 pathgenmap-0.0.4/LICENSE
--rw-r--r--   0 marcossousa   (501) staff       (20)      422 2023-07-13 23:37:18.724546 pathgenmap-0.0.4/PKG-INFO
--rw-r--r--   0 marcossousa   (501) staff       (20)      740 2023-07-13 21:56:31.000000 pathgenmap-0.0.4/README.md
-drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-13 23:37:18.717040 pathgenmap-0.0.4/pathgenmap/
--rw-r--r--   0 marcossousa   (501) staff       (20)     1307 2023-07-13 00:07:52.000000 pathgenmap-0.0.4/pathgenmap/EggAnnot.py
--rw-r--r--   0 marcossousa   (501) staff       (20)     3011 2023-07-13 13:17:10.000000 pathgenmap-0.0.4/pathgenmap/Integration.py
--rw-r--r--   0 marcossousa   (501) staff       (20)     1889 2023-07-13 11:28:07.000000 pathgenmap-0.0.4/pathgenmap/PathAnalys.py
--rw-r--r--   0 marcossousa   (501) staff       (20)     1139 2023-07-13 13:17:10.000000 pathgenmap-0.0.4/pathgenmap/PathGenMap.py
--rw-r--r--   0 marcossousa   (501) staff       (20)     1205 2023-07-13 11:46:42.000000 pathgenmap-0.0.4/pathgenmap/SpeciesAbundance.py
--rw-r--r--   0 marcossousa   (501) staff       (20)        0 2023-07-13 00:03:39.000000 pathgenmap-0.0.4/pathgenmap/__init__.py
-drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-13 23:37:18.722914 pathgenmap-0.0.4/pathgenmap.egg-info/
--rw-r--r--   0 marcossousa   (501) staff       (20)      422 2023-07-13 23:37:18.000000 pathgenmap-0.0.4/pathgenmap.egg-info/PKG-INFO
--rw-r--r--   0 marcossousa   (501) staff       (20)      348 2023-07-13 23:37:18.000000 pathgenmap-0.0.4/pathgenmap.egg-info/SOURCES.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)        1 2023-07-13 23:37:18.000000 pathgenmap-0.0.4/pathgenmap.egg-info/dependency_links.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       27 2023-07-13 23:37:18.000000 pathgenmap-0.0.4/pathgenmap.egg-info/requires.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       11 2023-07-13 23:37:18.000000 pathgenmap-0.0.4/pathgenmap.egg-info/top_level.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       38 2023-07-13 23:37:18.726480 pathgenmap-0.0.4/setup.cfg
--rw-r--r--   0 marcossousa   (501) staff       (20)      570 2023-07-13 23:34:56.000000 pathgenmap-0.0.4/setup.py
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-13 23:48:32.316652 pathgenmap-0.0.6/
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1083 2023-07-13 00:05:25.000000 pathgenmap-0.0.6/LICENSE
+-rw-r--r--   0 marcossousa   (501) staff       (20)      422 2023-07-13 23:48:32.315625 pathgenmap-0.0.6/PKG-INFO
+-rw-r--r--   0 marcossousa   (501) staff       (20)      740 2023-07-13 21:56:31.000000 pathgenmap-0.0.6/README.md
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-13 23:48:32.308422 pathgenmap-0.0.6/pathgenmap/
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1307 2023-07-13 00:07:52.000000 pathgenmap-0.0.6/pathgenmap/EggAnnot.py
+-rw-r--r--   0 marcossousa   (501) staff       (20)     3011 2023-07-13 13:17:10.000000 pathgenmap-0.0.6/pathgenmap/Integration.py
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1889 2023-07-13 11:28:07.000000 pathgenmap-0.0.6/pathgenmap/PathAnalys.py
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1139 2023-07-13 13:17:10.000000 pathgenmap-0.0.6/pathgenmap/PathGenMap.py
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1205 2023-07-13 11:46:42.000000 pathgenmap-0.0.6/pathgenmap/SpeciesAbundance.py
+-rw-r--r--   0 marcossousa   (501) staff       (20)        0 2023-07-13 00:03:39.000000 pathgenmap-0.0.6/pathgenmap/__init__.py
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-07-13 23:48:32.314702 pathgenmap-0.0.6/pathgenmap.egg-info/
+-rw-r--r--   0 marcossousa   (501) staff       (20)      422 2023-07-13 23:48:32.000000 pathgenmap-0.0.6/pathgenmap.egg-info/PKG-INFO
+-rw-r--r--   0 marcossousa   (501) staff       (20)      348 2023-07-13 23:48:32.000000 pathgenmap-0.0.6/pathgenmap.egg-info/SOURCES.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)        1 2023-07-13 23:48:32.000000 pathgenmap-0.0.6/pathgenmap.egg-info/dependency_links.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       27 2023-07-13 23:48:32.000000 pathgenmap-0.0.6/pathgenmap.egg-info/requires.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       11 2023-07-13 23:48:32.000000 pathgenmap-0.0.6/pathgenmap.egg-info/top_level.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       38 2023-07-13 23:48:32.316913 pathgenmap-0.0.6/setup.cfg
+-rw-r--r--   0 marcossousa   (501) staff       (20)      625 2023-07-13 23:48:01.000000 pathgenmap-0.0.6/setup.py
```

### Comparing `pathgenmap-0.0.4/LICENSE` & `pathgenmap-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pathgenmap-0.0.4/README.md` & `pathgenmap-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pathgenmap-0.0.4/pathgenmap/EggAnnot.py` & `pathgenmap-0.0.6/pathgenmap/EggAnnot.py`

 * *Files identical despite different names*

### Comparing `pathgenmap-0.0.4/pathgenmap/Integration.py` & `pathgenmap-0.0.6/pathgenmap/Integration.py`

 * *Files identical despite different names*

### Comparing `pathgenmap-0.0.4/pathgenmap/PathAnalys.py` & `pathgenmap-0.0.6/pathgenmap/PathAnalys.py`

 * *Files identical despite different names*

### Comparing `pathgenmap-0.0.4/pathgenmap/PathGenMap.py` & `pathgenmap-0.0.6/pathgenmap/PathGenMap.py`

 * *Files identical despite different names*

### Comparing `pathgenmap-0.0.4/pathgenmap/SpeciesAbundance.py` & `pathgenmap-0.0.6/pathgenmap/SpeciesAbundance.py`

 * *Files identical despite different names*

