# Comparing `tmp/raster_basics-1.3.8.tar.gz` & `tmp/raster_basics-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raster_basics-1.3.8.tar", last modified: Wed Jun 28 19:15:11 2023, max compression
+gzip compressed data, was "raster_basics-1.3.9.tar", last modified: Wed Jun 28 19:18:54 2023, max compression
```

## Comparing `raster_basics-1.3.8.tar` & `raster_basics-1.3.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-28 19:15:11.923421 raster_basics-1.3.8/
--rw-r--r--   0 albinwells   (501) staff       (20)      184 2023-06-28 19:15:11.923498 raster_basics-1.3.8/PKG-INFO
-drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-28 19:15:11.922156 raster_basics-1.3.8/raster_basics/
--rw-rw-r--   0 albinwells   (501) staff       (20)     8673 2023-06-24 16:30:10.000000 raster_basics-1.3.8/raster_basics/BaseFunctions.py
--rw-rw-r--   0 albinwells   (501) staff       (20)    42418 2023-06-24 15:35:22.000000 raster_basics-1.3.8/raster_basics/DataPlots.py
--rw-rw-r--   0 albinwells   (501) staff       (20)    24574 2023-06-16 19:26:40.000000 raster_basics-1.3.8/raster_basics/GlacierFunctions.py
--rw-rw-r--   0 albinwells   (501) staff       (20)    13354 2023-06-28 19:13:48.000000 raster_basics-1.3.8/raster_basics/RasterBasics.py
--rwxrwxrwx   0 albinwells   (501) staff       (20)    12126 2023-06-13 18:14:16.000000 raster_basics-1.3.8/raster_basics/SmoothingFunctions.py
--rw-rw-r--   0 albinwells   (501) staff       (20)      574 2023-02-03 15:09:59.000000 raster_basics-1.3.8/raster_basics/__init__.py
-drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-28 19:15:11.923230 raster_basics-1.3.8/raster_basics.egg-info/
--rw-r--r--   0 albinwells   (501) staff       (20)      184 2023-06-28 19:15:11.000000 raster_basics-1.3.8/raster_basics.egg-info/PKG-INFO
--rw-r--r--   0 albinwells   (501) staff       (20)      386 2023-06-28 19:15:11.000000 raster_basics-1.3.8/raster_basics.egg-info/SOURCES.txt
--rw-r--r--   0 albinwells   (501) staff       (20)        1 2023-06-28 19:15:11.000000 raster_basics-1.3.8/raster_basics.egg-info/dependency_links.txt
--rw-r--r--   0 albinwells   (501) staff       (20)        1 2023-06-28 19:15:11.000000 raster_basics-1.3.8/raster_basics.egg-info/not-zip-safe
--rw-r--r--   0 albinwells   (501) staff       (20)       14 2023-06-28 19:15:11.000000 raster_basics-1.3.8/raster_basics.egg-info/top_level.txt
--rw-rw-r--   0 albinwells   (501) staff       (20)       38 2023-06-28 19:15:11.923799 raster_basics-1.3.8/setup.cfg
--rw-rw-r--   0 albinwells   (501) staff       (20)      421 2023-06-28 19:14:54.000000 raster_basics-1.3.8/setup.py
+drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-28 19:18:54.932656 raster_basics-1.3.9/
+-rw-r--r--   0 albinwells   (501) staff       (20)      184 2023-06-28 19:18:54.932728 raster_basics-1.3.9/PKG-INFO
+drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-28 19:18:54.931842 raster_basics-1.3.9/raster_basics/
+-rw-rw-r--   0 albinwells   (501) staff       (20)     8673 2023-06-24 16:30:10.000000 raster_basics-1.3.9/raster_basics/BaseFunctions.py
+-rw-rw-r--   0 albinwells   (501) staff       (20)    42418 2023-06-24 15:35:22.000000 raster_basics-1.3.9/raster_basics/DataPlots.py
+-rw-rw-r--   0 albinwells   (501) staff       (20)    24574 2023-06-16 19:26:40.000000 raster_basics-1.3.9/raster_basics/GlacierFunctions.py
+-rw-rw-r--   0 albinwells   (501) staff       (20)    13355 2023-06-28 19:18:23.000000 raster_basics-1.3.9/raster_basics/RasterBasics.py
+-rwxrwxrwx   0 albinwells   (501) staff       (20)    12126 2023-06-13 18:14:16.000000 raster_basics-1.3.9/raster_basics/SmoothingFunctions.py
+-rw-rw-r--   0 albinwells   (501) staff       (20)      574 2023-02-03 15:09:59.000000 raster_basics-1.3.9/raster_basics/__init__.py
+drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-28 19:18:54.932547 raster_basics-1.3.9/raster_basics.egg-info/
+-rw-r--r--   0 albinwells   (501) staff       (20)      184 2023-06-28 19:18:54.000000 raster_basics-1.3.9/raster_basics.egg-info/PKG-INFO
+-rw-r--r--   0 albinwells   (501) staff       (20)      386 2023-06-28 19:18:54.000000 raster_basics-1.3.9/raster_basics.egg-info/SOURCES.txt
+-rw-r--r--   0 albinwells   (501) staff       (20)        1 2023-06-28 19:18:54.000000 raster_basics-1.3.9/raster_basics.egg-info/dependency_links.txt
+-rw-r--r--   0 albinwells   (501) staff       (20)        1 2023-06-28 19:18:54.000000 raster_basics-1.3.9/raster_basics.egg-info/not-zip-safe
+-rw-r--r--   0 albinwells   (501) staff       (20)       14 2023-06-28 19:18:54.000000 raster_basics-1.3.9/raster_basics.egg-info/top_level.txt
+-rw-rw-r--   0 albinwells   (501) staff       (20)       38 2023-06-28 19:18:54.932999 raster_basics-1.3.9/setup.cfg
+-rw-rw-r--   0 albinwells   (501) staff       (20)      421 2023-06-28 19:18:31.000000 raster_basics-1.3.9/setup.py
```

### Comparing `raster_basics-1.3.8/raster_basics/BaseFunctions.py` & `raster_basics-1.3.9/raster_basics/BaseFunctions.py`

 * *Files identical despite different names*

### Comparing `raster_basics-1.3.8/raster_basics/DataPlots.py` & `raster_basics-1.3.9/raster_basics/DataPlots.py`

 * *Files identical despite different names*

### Comparing `raster_basics-1.3.8/raster_basics/GlacierFunctions.py` & `raster_basics-1.3.9/raster_basics/GlacierFunctions.py`

 * *Files identical despite different names*

### Comparing `raster_basics-1.3.8/raster_basics/RasterBasics.py` & `raster_basics-1.3.9/raster_basics/RasterBasics.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import geopandas as gpd
 import pandas as pd
 
 
 
 """ Simple way to plot raster file """
 
-def open(geotiff, band=1):
+def rOpen(geotiff, band=1):
      """
 	Open a raster file as an array
 		geotiff: input raster filename (e.g. 'raster.tif')
 		band: the band to read. Defaults to 1 (int)
     """
     array = rasterio.open(geotiff).read(band)
     return array
```

### Comparing `raster_basics-1.3.8/raster_basics/SmoothingFunctions.py` & `raster_basics-1.3.9/raster_basics/SmoothingFunctions.py`

 * *Files identical despite different names*

### Comparing `raster_basics-1.3.8/raster_basics/__init__.py` & `raster_basics-1.3.9/raster_basics/__init__.py`

 * *Files identical despite different names*

