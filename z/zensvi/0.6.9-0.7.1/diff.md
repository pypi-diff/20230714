# Comparing `tmp/zensvi-0.6.9.tar.gz` & `tmp/zensvi-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zensvi-0.6.9.tar", max compression
+gzip compressed data, was "zensvi-0.7.1.tar", max compression
```

## Comparing `zensvi-0.6.9.tar` & `zensvi-0.7.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rwxr-xr-x   0        0        0     1072 2023-05-10 07:40:35.070000 zensvi-0.6.9/LICENSE
--rwxr-xr-x   0        0        0      669 2023-05-14 01:59:06.762105 zensvi-0.6.9/README.md
--rwxr-xr-x   0        0        0     1400 2023-07-11 09:05:50.294362 zensvi-0.6.9/pyproject.toml
--rwxr-xr-x   0        0        0      131 2023-05-14 01:59:06.769291 zensvi-0.6.9/src/zensvi/__init__.py
--rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769717 zensvi-0.6.9/src/zensvi/cv/__init__.py
--rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769911 zensvi-0.6.9/src/zensvi/cv/segmentation/__init__.py
--rwxr-xr-x   0        0        0    45608 2023-06-18 04:31:54.293066 zensvi-0.6.9/src/zensvi/cv/segmentation/segmentation.py
--rwxr-xr-x   0        0        0       63 2023-05-30 03:03:24.804064 zensvi-0.6.9/src/zensvi/download/__init__.py
--rw-r--r--   0        0        0      629 2023-07-11 07:03:47.656454 zensvi-0.6.9/src/zensvi/download/mapillary/__init__.py
--rw-r--r--   0        0        0        0 2023-07-11 07:03:47.656489 zensvi-0.6.9/src/zensvi/download/mapillary/config/.gitkeep
--rw-r--r--   0        0        0     1110 2023-07-11 07:03:47.656962 zensvi-0.6.9/src/zensvi/download/mapillary/config/__init__.py
--rw-r--r--   0        0        0      398 2023-07-11 07:03:47.657311 zensvi-0.6.9/src/zensvi/download/mapillary/config/api/__init__.py
--rw-r--r--   0        0        0    25264 2023-07-11 07:03:47.657833 zensvi-0.6.9/src/zensvi/download/mapillary/config/api/entities.py
--rw-r--r--   0        0        0     1917 2023-07-11 07:03:47.658201 zensvi-0.6.9/src/zensvi/download/mapillary/config/api/general.py
--rw-r--r--   0        0        0     8163 2023-07-11 07:03:47.658519 zensvi-0.6.9/src/zensvi/download/mapillary/config/api/vector_tiles.py
--rw-r--r--   0        0        0      481 2023-07-11 07:03:47.658811 zensvi-0.6.9/src/zensvi/download/mapillary/controller/__init__.py
--rw-r--r--   0        0        0     2297 2023-07-11 08:21:16.088478 zensvi-0.6.9/src/zensvi/download/mapillary/controller/detection.py
--rw-r--r--   0        0        0     4775 2023-07-11 08:21:17.279629 zensvi-0.6.9/src/zensvi/download/mapillary/controller/feature.py
--rw-r--r--   0        0        0    31634 2023-07-11 08:20:22.811895 zensvi-0.6.9/src/zensvi/download/mapillary/controller/image.py
--rw-r--r--   0        0        0     4904 2023-07-11 08:20:39.797301 zensvi-0.6.9/src/zensvi/download/mapillary/controller/save.py
--rw-r--r--   0        0        0    34865 2023-07-11 07:03:47.660533 zensvi-0.6.9/src/zensvi/download/mapillary/interface.py
--rw-r--r--   0        0        0        0 2023-07-11 07:03:47.660579 zensvi-0.6.9/src/zensvi/download/mapillary/models/.gitkeep
--rw-r--r--   0        0        0      520 2023-07-11 07:03:47.660843 zensvi-0.6.9/src/zensvi/download/mapillary/models/__init__.py
--rw-r--r--   0        0        0      396 2023-07-11 07:03:47.660998 zensvi-0.6.9/src/zensvi/download/mapillary/models/api/__init__.py
--rw-r--r--   0        0        0     8168 2023-07-11 08:21:35.171162 zensvi-0.6.9/src/zensvi/download/mapillary/models/api/entities.py
--rw-r--r--   0        0        0    14403 2023-07-11 08:23:11.396978 zensvi-0.6.9/src/zensvi/download/mapillary/models/api/general.py
--rw-r--r--   0        0        0    19294 2023-07-11 08:22:13.318683 zensvi-0.6.9/src/zensvi/download/mapillary/models/api/vector_tiles.py
--rw-r--r--   0        0        0     8273 2023-07-11 08:26:45.376434 zensvi-0.6.9/src/zensvi/download/mapillary/models/client.py
--rw-r--r--   0        0        0     1398 2023-07-11 07:03:47.662813 zensvi-0.6.9/src/zensvi/download/mapillary/models/config.py
--rw-r--r--   0        0        0    10328 2023-07-11 07:03:47.663102 zensvi-0.6.9/src/zensvi/download/mapillary/models/exceptions.py
--rw-r--r--   0        0        0    14602 2023-07-11 08:21:05.329571 zensvi-0.6.9/src/zensvi/download/mapillary/models/geojson.py
--rw-r--r--   0        0        0     2496 2023-07-11 07:03:47.663608 zensvi-0.6.9/src/zensvi/download/mapillary/models/logger.py
--rw-r--r--   0        0        0        0 2023-07-11 07:03:47.663642 zensvi-0.6.9/src/zensvi/download/mapillary/utils/.gitkeep
--rw-r--r--   0        0        0      511 2023-07-11 07:03:47.663779 zensvi-0.6.9/src/zensvi/download/mapillary/utils/__init__.py
--rw-r--r--   0        0        0     1774 2023-07-11 08:22:50.091875 zensvi-0.6.9/src/zensvi/download/mapillary/utils/auth.py
--rw-r--r--   0        0        0     1750 2023-07-11 07:03:47.664341 zensvi-0.6.9/src/zensvi/download/mapillary/utils/extract.py
--rw-r--r--   0        0        0    16138 2023-07-11 08:22:32.866063 zensvi-0.6.9/src/zensvi/download/mapillary/utils/filter.py
--rw-r--r--   0        0        0    26693 2023-07-11 08:26:13.918807 zensvi-0.6.9/src/zensvi/download/mapillary/utils/format.py
--rw-r--r--   0        0        0     1723 2023-07-11 07:03:47.665237 zensvi-0.6.9/src/zensvi/download/mapillary/utils/time.py
--rw-r--r--   0        0        0     9976 2023-07-11 08:22:46.586975 zensvi-0.6.9/src/zensvi/download/mapillary/utils/verify.py
--rwxr-xr-x   0        0        0    46157 2023-07-11 08:17:09.841741 zensvi-0.6.9/src/zensvi/download/streetview_downloader.py
--rwxr-xr-x   0        0        0   316244 2023-05-14 01:59:06.772840 zensvi-0.6.9/src/zensvi/download/utils/UserAgent.csv
--rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.772946 zensvi-0.6.9/src/zensvi/download/utils/__init__.py
--rwxr-xr-x   0        0        0     8651 2023-06-05 08:53:58.000000 zensvi-0.6.9/src/zensvi/download/utils/geoprocess.py
--rwxr-xr-x   0        0        0     1810 2023-06-05 08:53:58.000000 zensvi-0.6.9/src/zensvi/download/utils/get_pids.py
--rwxr-xr-x   0        0        0      956 2023-05-14 09:11:59.596085 zensvi-0.6.9/src/zensvi/download/utils/helpers.py
--rwxr-xr-x   0        0        0     6747 2023-06-23 05:30:15.378713 zensvi-0.6.9/src/zensvi/download/utils/imtool.py
--rw-r--r--   0        0        0    82321 2023-05-11 09:02:38.204470 zensvi-0.6.9/src/zensvi/download/utils/proxies.csv
--rwxr-xr-x   0        0        0       30 2023-05-14 01:59:06.778122 zensvi-0.6.9/src/zensvi/transform/__init__.py
--rwxr-xr-x   0        0        0    10503 2023-06-01 06:19:20.344499 zensvi-0.6.9/src/zensvi/transform/transform_image.py
--rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.778944 zensvi-0.6.9/src/zensvi/zensvi.py
--rw-r--r--   0        0        0     3182 1970-01-01 00:00:00.000000 zensvi-0.6.9/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2023-05-10 07:40:35.070000 zensvi-0.7.1/LICENSE
+-rwxr-xr-x   0        0        0      669 2023-05-14 01:59:06.762105 zensvi-0.7.1/README.md
+-rwxr-xr-x   0        0        0     1401 2023-07-14 07:55:46.212406 zensvi-0.7.1/pyproject.toml
+-rwxr-xr-x   0        0        0      131 2023-05-14 01:59:06.769291 zensvi-0.7.1/src/zensvi/__init__.py
+-rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769717 zensvi-0.7.1/src/zensvi/cv/__init__.py
+-rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769911 zensvi-0.7.1/src/zensvi/cv/segmentation/__init__.py
+-rwxr-xr-x   0        0        0    45608 2023-07-13 09:34:43.004230 zensvi-0.7.1/src/zensvi/cv/segmentation/segmentation.py
+-rwxr-xr-x   0        0        0       63 2023-05-30 03:03:24.804064 zensvi-0.7.1/src/zensvi/download/__init__.py
+-rw-r--r--   0        0        0      629 2023-07-11 07:03:47.656454 zensvi-0.7.1/src/zensvi/download/mapillary/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 07:03:47.656489 zensvi-0.7.1/src/zensvi/download/mapillary/config/.gitkeep
+-rw-r--r--   0        0        0     1110 2023-07-11 07:03:47.656962 zensvi-0.7.1/src/zensvi/download/mapillary/config/__init__.py
+-rw-r--r--   0        0        0      398 2023-07-11 07:03:47.657311 zensvi-0.7.1/src/zensvi/download/mapillary/config/api/__init__.py
+-rw-r--r--   0        0        0    25264 2023-07-11 07:03:47.657833 zensvi-0.7.1/src/zensvi/download/mapillary/config/api/entities.py
+-rw-r--r--   0        0        0     1917 2023-07-11 07:03:47.658201 zensvi-0.7.1/src/zensvi/download/mapillary/config/api/general.py
+-rw-r--r--   0        0        0     8163 2023-07-11 07:03:47.658519 zensvi-0.7.1/src/zensvi/download/mapillary/config/api/vector_tiles.py
+-rw-r--r--   0        0        0      481 2023-07-11 07:03:47.658811 zensvi-0.7.1/src/zensvi/download/mapillary/controller/__init__.py
+-rw-r--r--   0        0        0     2297 2023-07-11 08:21:16.088478 zensvi-0.7.1/src/zensvi/download/mapillary/controller/detection.py
+-rw-r--r--   0        0        0     4775 2023-07-11 08:21:17.279629 zensvi-0.7.1/src/zensvi/download/mapillary/controller/feature.py
+-rw-r--r--   0        0        0    31634 2023-07-11 08:20:22.811895 zensvi-0.7.1/src/zensvi/download/mapillary/controller/image.py
+-rw-r--r--   0        0        0     4904 2023-07-11 08:20:39.797301 zensvi-0.7.1/src/zensvi/download/mapillary/controller/save.py
+-rw-r--r--   0        0        0    34865 2023-07-11 07:03:47.660533 zensvi-0.7.1/src/zensvi/download/mapillary/interface.py
+-rw-r--r--   0        0        0        0 2023-07-11 07:03:47.660579 zensvi-0.7.1/src/zensvi/download/mapillary/models/.gitkeep
+-rw-r--r--   0        0        0      520 2023-07-11 07:03:47.660843 zensvi-0.7.1/src/zensvi/download/mapillary/models/__init__.py
+-rw-r--r--   0        0        0      396 2023-07-11 07:03:47.660998 zensvi-0.7.1/src/zensvi/download/mapillary/models/api/__init__.py
+-rw-r--r--   0        0        0     8168 2023-07-11 08:21:35.171162 zensvi-0.7.1/src/zensvi/download/mapillary/models/api/entities.py
+-rw-r--r--   0        0        0    14403 2023-07-11 08:23:11.396978 zensvi-0.7.1/src/zensvi/download/mapillary/models/api/general.py
+-rw-r--r--   0        0        0    19294 2023-07-11 08:22:13.318683 zensvi-0.7.1/src/zensvi/download/mapillary/models/api/vector_tiles.py
+-rw-r--r--   0        0        0     8273 2023-07-11 08:26:45.376434 zensvi-0.7.1/src/zensvi/download/mapillary/models/client.py
+-rw-r--r--   0        0        0     1398 2023-07-11 07:03:47.662813 zensvi-0.7.1/src/zensvi/download/mapillary/models/config.py
+-rw-r--r--   0        0        0    10328 2023-07-11 07:03:47.663102 zensvi-0.7.1/src/zensvi/download/mapillary/models/exceptions.py
+-rw-r--r--   0        0        0    14602 2023-07-11 08:21:05.329571 zensvi-0.7.1/src/zensvi/download/mapillary/models/geojson.py
+-rw-r--r--   0        0        0     2496 2023-07-11 07:03:47.663608 zensvi-0.7.1/src/zensvi/download/mapillary/models/logger.py
+-rw-r--r--   0        0        0        0 2023-07-11 07:03:47.663642 zensvi-0.7.1/src/zensvi/download/mapillary/utils/.gitkeep
+-rw-r--r--   0        0        0      511 2023-07-11 07:03:47.663779 zensvi-0.7.1/src/zensvi/download/mapillary/utils/__init__.py
+-rw-r--r--   0        0        0     1774 2023-07-11 08:22:50.091875 zensvi-0.7.1/src/zensvi/download/mapillary/utils/auth.py
+-rw-r--r--   0        0        0     1750 2023-07-11 07:03:47.664341 zensvi-0.7.1/src/zensvi/download/mapillary/utils/extract.py
+-rw-r--r--   0        0        0    16350 2023-07-14 07:43:43.677493 zensvi-0.7.1/src/zensvi/download/mapillary/utils/filter.py
+-rw-r--r--   0        0        0    26693 2023-07-11 08:26:13.918807 zensvi-0.7.1/src/zensvi/download/mapillary/utils/format.py
+-rw-r--r--   0        0        0     1723 2023-07-11 07:03:47.665237 zensvi-0.7.1/src/zensvi/download/mapillary/utils/time.py
+-rw-r--r--   0        0        0     9976 2023-07-11 08:22:46.586975 zensvi-0.7.1/src/zensvi/download/mapillary/utils/verify.py
+-rwxr-xr-x   0        0        0    46486 2023-07-14 07:46:10.092959 zensvi-0.7.1/src/zensvi/download/streetview_downloader.py
+-rwxr-xr-x   0        0        0   316244 2023-05-14 01:59:06.772840 zensvi-0.7.1/src/zensvi/download/utils/UserAgent.csv
+-rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.772946 zensvi-0.7.1/src/zensvi/download/utils/__init__.py
+-rwxr-xr-x   0        0        0     8651 2023-06-05 08:53:58.000000 zensvi-0.7.1/src/zensvi/download/utils/geoprocess.py
+-rwxr-xr-x   0        0        0     1810 2023-06-05 08:53:58.000000 zensvi-0.7.1/src/zensvi/download/utils/get_pids.py
+-rwxr-xr-x   0        0        0      956 2023-05-14 09:11:59.596085 zensvi-0.7.1/src/zensvi/download/utils/helpers.py
+-rwxr-xr-x   0        0        0     6921 2023-07-13 10:04:29.377009 zensvi-0.7.1/src/zensvi/download/utils/imtool.py
+-rw-r--r--   0        0        0    82321 2023-05-11 09:02:38.204470 zensvi-0.7.1/src/zensvi/download/utils/proxies.csv
+-rwxr-xr-x   0        0        0       30 2023-05-14 01:59:06.778122 zensvi-0.7.1/src/zensvi/transform/__init__.py
+-rwxr-xr-x   0        0        0    10503 2023-06-01 06:19:20.344499 zensvi-0.7.1/src/zensvi/transform/transform_image.py
+-rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.778944 zensvi-0.7.1/src/zensvi/zensvi.py
+-rw-r--r--   0        0        0     3158 1970-01-01 00:00:00.000000 zensvi-0.7.1/PKG-INFO
```

### Comparing `zensvi-0.6.9/LICENSE` & `zensvi-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.9/README.md` & `zensvi-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.9/pyproject.toml` & `zensvi-0.7.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "zensvi"
-version = "0.6.9"
+version = "0.7.1"
 description = "This package handles downloading, cleaning, analyzing street view imagery in a one-stop and zen manner."
 authors = ["koito19960406"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
 Pillow = ">=8.3.2,<9.6"
 geopandas = ">=0.10.0"
 geopy = "^2.2.0"
-numpy = "^1.21.0"
-opencv_python = "^4.5.3"
+numpy = ">=1.21.0"
+opencv_python = ">=4.5.3"
 osmnx = "^1.1.1"
 pandas = "^1.3.3"
 requests = "^2.25.1"
 setuptools = ">=64.0.3"
 Shapely=">=1.8.1"
 torch = "^2.0.0"
 tqdm = "^4.61.1"
@@ -27,15 +27,15 @@
 bleach = "^3.3.0"
 certifi = "^2021.5.30"
 chardet = "^4.0.0"
 click = "^8.0.1"
 click-plugins = "^1.1.1"
 cligj = "^0.7.2"
 coverage = "^5.5"
-docutils = "^0.17.1"
+docutils = ">=0.16"
 future = "^0.18.2"
 hypothesis = "^6.14.0"
 idna = "^2.10"
 iniconfig = "^1.1.1"
 mapbox-vector-tile = "^1.2.1"
 mercantile = "^1.2.1"
 munch = "^2.5.0"
```

### Comparing `zensvi-0.6.9/src/zensvi/cv/segmentation/segmentation.py` & `zensvi-0.7.1/src/zensvi/cv/segmentation/segmentation.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.9/src/zensvi/download/mapillary/__init__.py` & `zensvi-0.7.1/src/zensvi/download/mapillary/__init__.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.9/src/zensvi/download/mapillary/config/__init__.py` & `zensvi-0.7.1/src/zensvi/download/mapillary/config/__init__.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.9/src/zensvi/download/mapillary/config/api/entities.py` & `zensvi-0.7.1/src/zensvi/download/mapillary/config/api/entities.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.9/src/zensvi/download/mapillary/config/api/general.py` & `zensvi-0.7.1/src/zensvi/download/mapillary/config/api/general.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.9/src/zensvi/download/mapillary/config/api/vector_tiles.py` & `zensvi-0.7.1/src/zensvi/download/mapillary/config/api/vector_tiles.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.9/src/zensvi/download/mapillary/controller/detection.py` & `zensvi-0.7.1/src/zensvi/download/mapillary/controller/detection.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.9/src/zensvi/download/mapillary/controller/feature.py` & `zensvi-0.7.1/src/zensvi/download/mapillary/controller/feature.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.9/src/zensvi/download/mapillary/controller/image.py` & `zensvi-0.7.1/src/zensvi/download/mapillary/controller/image.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.9/src/zensvi/download/mapillary/controller/save.py` & `zensvi-0.7.1/src/zensvi/download/mapillary/controller/save.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.9/src/zensvi/download/mapillary/interface.py` & `zensvi-0.7.1/src/zensvi/download/mapillary/interface.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.9/src/zensvi/download/mapillary/models/__init__.py` & `zensvi-0.7.1/src/zensvi/download/mapillary/models/__init__.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.9/src/zensvi/download/mapillary/models/api/entities.py` & `zensvi-0.7.1/src/zensvi/download/mapillary/models/api/entities.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.9/src/zensvi/download/mapillary/models/api/general.py` & `zensvi-0.7.1/src/zensvi/download/mapillary/models/api/general.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.9/src/zensvi/download/mapillary/models/api/vector_tiles.py` & `zensvi-0.7.1/src/zensvi/download/mapillary/models/api/vector_tiles.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.9/src/zensvi/download/mapillary/models/client.py` & `zensvi-0.7.1/src/zensvi/download/mapillary/models/client.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.9/src/zensvi/download/mapillary/models/config.py` & `zensvi-0.7.1/src/zensvi/download/mapillary/models/config.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.9/src/zensvi/download/mapillary/models/exceptions.py` & `zensvi-0.7.1/src/zensvi/download/mapillary/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.9/src/zensvi/download/mapillary/models/geojson.py` & `zensvi-0.7.1/src/zensvi/download/mapillary/models/geojson.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.9/src/zensvi/download/mapillary/models/logger.py` & `zensvi-0.7.1/src/zensvi/download/mapillary/models/logger.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.9/src/zensvi/download/mapillary/utils/auth.py` & `zensvi-0.7.1/src/zensvi/download/mapillary/utils/auth.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.9/src/zensvi/download/mapillary/utils/extract.py` & `zensvi-0.7.1/src/zensvi/download/mapillary/utils/extract.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.9/src/zensvi/download/mapillary/utils/filter.py` & `zensvi-0.7.1/src/zensvi/download/mapillary/utils/filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -336,26 +336,31 @@
 
     # Define an empty list
     output = []
 
     # Go through the features
     for feature in data:
 
-        # If the calculated haversince distance is less than the radius ...
+        # Reverse the order of the coords to (lon, lat) before feeding into the haversine function
+        reversed_coords = coords[::-1]
+        reversed_feature_coords = feature["geometry"]["coordinates"][::-1]
+
+        # If the calculated haversine distance is less than the radius ...
         if (
-            haversine.haversine(coords, feature["geometry"]["coordinates"], unit=unit)
+            haversine.haversine(reversed_coords, reversed_feature_coords, unit=unit)
             < radius
         ):
             # ... append to the output
             output.append(feature)
 
     # Return the output
     return output
 
 
+
 def image_type(data: list, image_type: str) -> list:
     """
     The parameter might be 'all' (both is_pano == true and false), 'pano' (is_pano == true only),
     or 'flat' (is_pano == false only)
 
     :param data: The data to be filtered
     :type data: list
```

### Comparing `zensvi-0.6.9/src/zensvi/download/mapillary/utils/format.py` & `zensvi-0.7.1/src/zensvi/download/mapillary/utils/format.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.9/src/zensvi/download/mapillary/utils/time.py` & `zensvi-0.7.1/src/zensvi/download/mapillary/utils/time.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.9/src/zensvi/download/mapillary/utils/verify.py` & `zensvi-0.7.1/src/zensvi/download/mapillary/utils/verify.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.9/src/zensvi/download/streetview_downloader.py` & `zensvi-0.7.1/src/zensvi/download/streetview_downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from zensvi.download.utils.imtool import ImageTool
 from zensvi.download.utils.get_pids import panoids
 from zensvi.download.utils.geoprocess import GeoProcessor
 from zensvi.download.utils.helpers import standardize_column_names, create_buffer_gdf
 
 # set logging level to warning
 import logging
-logging.getLogger('zensvi.download.mapillary.utils.client').setLevel(logging.WARNING)
+logging.getLogger('mapillary.utils.client').setLevel(logging.WARNING)
 
 class BaseDownloader(ABC):
     @abstractmethod
     def __init__(self, log_path = None, distance = 1, grid = False, grid_size = 1):
         self._log_path = log_path
         self._distance = distance
         self._grid = grid
@@ -108,19 +108,22 @@
             return
         with open(self.log_path, 'a+') as fw:
             for pid in pids:
                 fw.write(pid+'\n')
                 
     def _check_already(self, all_panoids):
         # Get the set of already downloaded images
-        name_r = set(name.split(".")[0] for name in tqdm(os.listdir(self.panorama_output), desc="Checking already downloaded images"))
+        name_r = set()
+        for dirpath, dirnames, filenames in os.walk(self.panorama_output):
+            for name in filenames:
+                name_r.add(name.split(".")[0])
 
         # Filter the list of all panoids to only include those not already downloaded
         all_panoids = list(set(all_panoids) - name_r)
-        return all_panoids 
+        return all_panoids
     
     def _read_pids(self, path_pid):
         pid_df = pd.read_csv(path_pid)
         # get unique pids as a list
         pids = pid_df.iloc[:,0].unique().tolist()
         return pids
 
@@ -478,15 +481,15 @@
         # set other cache directories
         self.cache_lat_lon = self.dir_cache / "lat_lon.csv"
         self.cache_pids_raw = self.dir_cache / "pids_raw.csv"
         self.cache_pids_augmented = self.dir_cache / "pids_augemented.csv"
         
     def download_svi(self, dir_output, path_pid = None, zoom=2, h_tiles=4, v_tiles=2, cropped=False, full=True, 
                     lat=None, lon=None, input_csv_file="", input_shp_file = "", input_place_name = "", id_columns=None, buffer = 0, 
-                    augment_metadata=False, update_pids = False, **kwargs):
+                    augment_metadata=False, batch_size = 1000, update_pids = False, **kwargs):
         # set necessary directories
         self._set_dirs(dir_output)
         
         # call get_pids function first if path_pid is None
         if (path_pid is None) & (self.cache_pids_augmented.exists() == False):
             print("Getting pids...")
             path_pid = self.dir_output / "gsv_pids.csv"
@@ -518,15 +521,15 @@
             print("There is no panorama ID to download")
             return
         else:
             panoids_rest = self._check_already(panoids)
 
         if len(panoids_rest) > 0:
             UAs = random.choices(self.user_agents, k = len(panoids_rest))
-            ImageTool.dwl_multiple(panoids_rest, zoom, v_tiles, h_tiles, self.panorama_output, UAs, self.proxies, cropped, full, log_path=self.log_path)
+            ImageTool.dwl_multiple(panoids_rest, zoom, v_tiles, h_tiles, self.panorama_output, UAs, self.proxies, cropped, full, batch_size = batch_size, log_path=self.log_path)
         else:
             print("All images have been downloaded")
         
         # delete the cache directory
         if self.dir_cache.exists():
             shutil.rmtree(self.dir_cache)
             print("The cache directory has been deleted")
@@ -587,15 +590,15 @@
             # Merge on the ID column, keeping track of where each row originates
             merged = df.merge(completed_ids, on='lat_lon_id', how='outer', indicator=True)
 
             # Filter out rows that come from the 'completed_ids' DataFrame
             df = merged[merged['_merge'] == 'left_only'].drop(columns='_merge')
 
         def get_street_view_info(latitude, longitude, **kwargs):
-            results = mly.get_image_close_to(latitude, longitude, **kwargs).to_dict()["features"]
+            results = mly.get_image_close_to(latitude = latitude, longitude = longitude, **kwargs).to_dict()["features"]
             return results
 
         def worker(row, **kwargs):
             input_latitude = row.latitude
             input_longitude = row.longitude
             lat_lon_id = row.lat_lon_id
             id_dict = {column: getattr(row, column) for column in id_columns} if id_columns else {}
@@ -761,15 +764,15 @@
         mly_kwargs = {k: v for k, v in kwargs.items() if k in mly_allowed_keys}
         if self.cache_pids_raw.exists():
             pid = pd.read_csv(self.cache_pids_raw)
             print("The raw panorama IDs have been read from the cache")
             return pid
 
         if kwargs['lat'] is not None and kwargs['lon'] is not None:
-            pid = mly.get_image_close_to(kwargs['lat'], kwargs['lon'], **mly_kwargs)
+            pid = mly.get_image_close_to(latitude = kwargs['lat'], longitude = kwargs['lon'], **mly_kwargs)
             # Convert to DataFrame
             pid = gpd.GeoDataFrame.from_features(pid.to_dict()['features'])
             pid['lon'] = pid['geometry'].apply(lambda geom: geom.x)
             pid['lat'] = pid['geometry'].apply(lambda geom: geom.y)
             # drop geometry column
             pid = pid.drop(columns='geometry')
             pid = pd.DataFrame(pid)
@@ -900,16 +903,16 @@
         results_df = pd.concat([pd.read_csv(checkpoint) for checkpoint in glob.glob(str(dir_cache_urls / '*.csv'))], ignore_index=True)
         results_df.to_csv(self.pids_url, index=False)
 
         if dir_cache_urls.exists():
             shutil.rmtree(dir_cache_urls)
 
     
-    def _download_images_mly(self, cropped):
-        checkpoints = glob.glob(str(self.panorama_output / '*.png'))
+    def _download_images_mly(self, cropped, batch_size):
+        checkpoints = glob.glob(str(self.panorama_output / '**/*.png'), recursive=True)
 
         # Read already downloaded images and convert to ids
         downloaded_ids = set([Path(file_path).stem for file_path in checkpoints])  # Use set for faster operations
 
         urls_df = pd.read_csv(self.pids_url)
 
         # Filter out the ids that have already been processed
@@ -936,29 +939,32 @@
 
                 else:
                     self._log_write(panoid)
             except Exception as e:
                 self._log_write(panoid)
                 print(f"Error: {e}" )
 
-
-        batch_size = 1000
         num_batches = (len(urls_df) + batch_size - 1) // batch_size
 
         for i in tqdm(range(num_batches), desc=f"Downloading images by batch size {min(batch_size, len(urls_df))}"):
+            # Create a new sub-folder for each batch
+            batch_out_path = self.panorama_output / f"batch_{i+1}"
+            batch_out_path.mkdir(exist_ok=True)
+            
             with ThreadPoolExecutor() as executor:
-                batch_futures = {executor.submit(worker, row, self.panorama_output, cropped): row.id for row in urls_df.iloc[i*batch_size : (i+1)*batch_size].itertuples()}
+                batch_futures = {executor.submit(worker, row, batch_out_path, cropped): row.id for row in urls_df.iloc[i*batch_size : (i+1)*batch_size].itertuples()}
                 for future in tqdm(as_completed(batch_futures), total=len(batch_futures), desc=f"Downloading images for batch #{i+1}"):
                     try:
                         future.result()
                     except Exception as e:
                         print(f"Error: {e}")
+
                 
     def download_svi(self, dir_output, path_pid = None, lat=None, lon=None, input_csv_file="", input_shp_file = "", input_place_name =
-                    "", id_columns=None, buffer = 0, update_pids = False, resolution = 1024, cropped = False, **kwargs):
+                    "", id_columns=None, buffer = 0, update_pids = False, resolution = 1024, cropped = False, batch_size = 1000, **kwargs):
         # set necessary directories
         self._set_dirs(dir_output)
         
         # call get_pids function first if path_pid is None
         if path_pid is None:
             print("Getting pids...")
             path_pid = self.dir_output / "mly_pids.csv"
@@ -981,15 +987,15 @@
         self.panorama_output = self.dir_output / "mly_svi"
         self.panorama_output.mkdir(parents=True, exist_ok=True)
         
         # get urls
         if path_pid.exists():
             self._get_urls_mly(path_pid, resolution=resolution) 
             # download images
-            self._download_images_mly(cropped)
+            self._download_images_mly(cropped, batch_size)
         else: 
             print("There is no panorama ID to download within the given input parameters")
         
         # delete the cache directory
         if self.dir_cache.exists():
             shutil.rmtree(self.dir_cache)
             print("The cache directory has been deleted")
```

### Comparing `zensvi-0.6.9/src/zensvi/download/utils/UserAgent.csv` & `zensvi-0.7.1/src/zensvi/download/utils/UserAgent.csv`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.9/src/zensvi/download/utils/geoprocess.py` & `zensvi-0.7.1/src/zensvi/download/utils/geoprocess.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.9/src/zensvi/download/utils/get_pids.py` & `zensvi-0.7.1/src/zensvi/download/utils/get_pids.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.9/src/zensvi/download/utils/helpers.py` & `zensvi-0.7.1/src/zensvi/download/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.9/src/zensvi/download/utils/imtool.py` & `zensvi-0.7.1/src/zensvi/download/utils/imtool.py`

 * *Files 12% similar despite different names*

```diff
@@ -115,15 +115,15 @@
             else:
                 raise ValueError(f"Invalid image for pano_id {pano_id}")
 
         return identif
 
 
     @staticmethod
-    def dwl_multiple(panoids, zoom, v_tiles, h_tiles, out_path, uas, proxies, cropped, full, log_path=None):
+    def dwl_multiple(panoids, zoom, v_tiles, h_tiles, out_path, uas, proxies, cropped, full, batch_size = 1000, log_path=None):
         """
         Description of dwl_multiple
         
         Calls the get_and_save_image function using multiple threads.
         
         Args:
             panoids (undefined): GSV anorama id
@@ -143,32 +143,35 @@
 
         def log_error(panoid):
             nonlocal log_path
             if log_path is not None:
                 with open(log_path, 'a') as log_file:
                     log_file.write(f"{panoid}\n")
 
-        batch_size = 100  # Modify this to a suitable value
         num_batches = (len(panoids) + batch_size - 1) // batch_size
 
         for i in tqdm(range(num_batches), desc= f"Downloading images by batch size {min(batch_size, len(panoids))}"):
+            # Create a new sub-folder for each batch
+            batch_out_path = os.path.join(out_path, f"batch_{i+1}")
+            os.makedirs(batch_out_path, exist_ok=True)
+
             with ThreadPoolExecutor(max_workers=min(len(uas), batch_size)) as executor:
                 jobs = []
                 batch_panoids = panoids[i*batch_size : (i+1)*batch_size]
                 batch_uas = uas[i*batch_size : (i+1)*batch_size]
                 for pano, ua in zip(batch_panoids, batch_uas):
                     kw = {
                         "pano_id": pano,
                         "identif": pano,
                         "ua": ua,
                         "proxies": proxies,
                         "zoom": zoom,
                         "vertical_tiles": v_tiles,
                         "horizontal_tiles": h_tiles,
-                        "out_path": out_path,
+                        "out_path": batch_out_path,  # Pass the new sub-folder path
                         "cropped": cropped,
                         "full": full
                     }
                     jobs.append(executor.submit(ImageTool.get_and_save_image, **kw))
 
                 for job in tqdm(as_completed(jobs), total=len(jobs), desc=f"Downloading images for batch #{i+1}"):
                     try:
```

### Comparing `zensvi-0.6.9/src/zensvi/download/utils/proxies.csv` & `zensvi-0.7.1/src/zensvi/download/utils/proxies.csv`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.9/src/zensvi/transform/transform_image.py` & `zensvi-0.7.1/src/zensvi/transform/transform_image.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.6.9/PKG-INFO` & `zensvi-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zensvi
-Version: 0.6.9
+Version: 0.7.1
 Summary: This package handles downloading, cleaning, analyzing street view imagery in a one-stop and zen manner.
 License: MIT
 Author: koito19960406
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -17,29 +17,29 @@
 Requires-Dist: bleach (>=3.3.0,<4.0.0)
 Requires-Dist: certifi (>=2021.5.30,<2022.0.0)
 Requires-Dist: chardet (>=4.0.0,<5.0.0)
 Requires-Dist: click (>=8.0.1,<9.0.0)
 Requires-Dist: click-plugins (>=1.1.1,<2.0.0)
 Requires-Dist: cligj (>=0.7.2,<0.8.0)
 Requires-Dist: coverage (>=5.5,<6.0)
-Requires-Dist: docutils (>=0.17.1,<0.18.0)
+Requires-Dist: docutils (>=0.16)
 Requires-Dist: future (>=0.18.2,<0.19.0)
 Requires-Dist: geojson (>=2.5.0,<3.0.0)
 Requires-Dist: geopandas (>=0.10.0)
 Requires-Dist: geopy (>=2.2.0,<3.0.0)
 Requires-Dist: haversine (>=2.3.1,<3.0.0)
 Requires-Dist: hypothesis (>=6.14.0,<7.0.0)
 Requires-Dist: idna (>=2.10,<3.0)
 Requires-Dist: iniconfig (>=1.1.1,<2.0.0)
 Requires-Dist: mapbox-vector-tile (>=1.2.1,<2.0.0)
 Requires-Dist: mercantile (>=1.2.1,<2.0.0)
 Requires-Dist: munch (>=2.5.0,<3.0.0)
 Requires-Dist: networkx (>=3.1,<4.0)
-Requires-Dist: numpy (>=1.21.0,<2.0.0)
-Requires-Dist: opencv_python (>=4.5.3,<5.0.0)
+Requires-Dist: numpy (>=1.21.0)
+Requires-Dist: opencv_python (>=4.5.3)
 Requires-Dist: osmnx (>=1.1.1,<2.0.0)
 Requires-Dist: pandas (>=1.3.3,<2.0.0)
 Requires-Dist: pkginfo (>=1.7.0,<2.0.0)
 Requires-Dist: pluggy (>=0.13.1,<0.14.0)
 Requires-Dist: protobuf (>=3.17.3,<4.0.0)
 Requires-Dist: psutil (>=5.8.0,<6.0.0)
 Requires-Dist: py (>=1.10.0,<2.0.0)
```

