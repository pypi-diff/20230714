# Comparing `tmp/gispandas-0.1.8.tar.gz` & `tmp/gispandas-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gispandas-0.1.8.tar", last modified: Fri Jul 14 07:29:21 2023, max compression
+gzip compressed data, was "gispandas-0.1.9.tar", last modified: Fri Jul 14 08:02:25 2023, max compression
```

## Comparing `gispandas-0.1.8.tar` & `gispandas-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 07:29:21.540085 gispandas-0.1.8/
--rw-rw-rw-   0        0        0     1313 2023-07-14 07:29:21.540085 gispandas-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1009 2023-07-14 07:28:15.000000 gispandas-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 07:29:21.530111 gispandas-0.1.8/gispandas/
--rw-rw-rw-   0        0        0      308 2023-07-14 06:50:55.000000 gispandas-0.1.8/gispandas/__init__.py
--rw-rw-rw-   0        0        0     5913 2023-07-14 07:28:45.000000 gispandas-0.1.8/gispandas/mxclf.py
--rw-rw-rw-   0        0        0    18038 2023-07-14 06:06:06.000000 gispandas-0.1.8/gispandas/mxgdal.py
--rw-rw-rw-   0        0        0     1457 2023-07-14 05:32:01.000000 gispandas-0.1.8/gispandas/mxgee.py
--rw-rw-rw-   0        0        0     2787 2023-07-14 06:09:39.000000 gispandas-0.1.8/gispandas/mxgpd.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:29:21.538088 gispandas-0.1.8/gispandas.egg-info/
--rw-rw-rw-   0        0        0     1313 2023-07-14 07:29:21.000000 gispandas-0.1.8/gispandas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-07-14 07:29:21.000000 gispandas-0.1.8/gispandas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 07:29:21.000000 gispandas-0.1.8/gispandas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-14 07:25:00.000000 gispandas-0.1.8/gispandas.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-07-14 07:29:21.000000 gispandas-0.1.8/gispandas.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 07:29:21.541082 gispandas-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      876 2023-07-14 07:28:10.000000 gispandas-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 08:02:25.165472 gispandas-0.1.9/
+-rw-rw-rw-   0        0        0     1315 2023-07-14 08:02:25.164475 gispandas-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1011 2023-07-14 07:30:45.000000 gispandas-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 08:02:25.152507 gispandas-0.1.9/gispandas/
+-rw-rw-rw-   0        0        0      308 2023-07-14 08:02:03.000000 gispandas-0.1.9/gispandas/__init__.py
+-rw-rw-rw-   0        0        0     5923 2023-07-14 07:53:39.000000 gispandas-0.1.9/gispandas/mxclf.py
+-rw-rw-rw-   0        0        0    18038 2023-07-14 06:06:06.000000 gispandas-0.1.9/gispandas/mxgdal.py
+-rw-rw-rw-   0        0        0     1467 2023-07-14 07:58:23.000000 gispandas-0.1.9/gispandas/mxgee.py
+-rw-rw-rw-   0        0        0     2787 2023-07-14 06:09:39.000000 gispandas-0.1.9/gispandas/mxgpd.py
+drwxrwxrwx   0        0        0        0 2023-07-14 08:02:25.162481 gispandas-0.1.9/gispandas.egg-info/
+-rw-rw-rw-   0        0        0     1315 2023-07-14 08:02:24.000000 gispandas-0.1.9/gispandas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-07-14 08:02:24.000000 gispandas-0.1.9/gispandas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 08:02:24.000000 gispandas-0.1.9/gispandas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-14 08:02:24.000000 gispandas-0.1.9/gispandas.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2023-07-14 08:02:24.000000 gispandas-0.1.9/gispandas.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 08:02:25.165472 gispandas-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      876 2023-07-14 08:01:55.000000 gispandas-0.1.9/setup.py
```

### Comparing `gispandas-0.1.8/PKG-INFO` & `gispandas-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gispandas
-Version: 0.1.8
+Version: 0.1.9
 Summary: gispandas
 Home-page: https://github.com/mxhou/gispandas/
 Author: HMX
 Author-email: kzdhb8023@163.com
 License: MIT
 Keywords: gis,geo,tif,json,shp
 Requires-Python: >=3.6
@@ -13,15 +13,15 @@
 # GisPandas针对栅格数据进行统计的python包
 GisPandas是一个为栅格、矢量数据处理、分析以及可视化而开发的Python包。GisPandas为常见栅格矢量数据提供了快速而简洁的gis操作方法，代码简洁、高效、灵活、易用，可以用简洁的代码实现复杂的数据任务。
 # 主要功能
 目前，GisPandas主要提供以下方法：
 
 1.栅格数据进行阿尔伯斯等面积投影，根据矢量区划计算面积并导出json。
 
-2.种植结构变化,自动对齐，导出栅格数据和统计json。
+2.种植结构变化，自动对齐，导出栅格数据和统计json。
 
 3.gee下载数据的后处理主要包括：栅格数据镶嵌并压缩。
 
 4.矢量数据写入四至、中心经纬度等属性，矢量简化，文本矢量化等。
 
 5.栅格数据像素对齐、裁剪、重采样、投影、插值、切片、格式转换等。
 # 安装
```

### Comparing `gispandas-0.1.8/README.md` & `gispandas-0.1.9/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # GisPandas针对栅格数据进行统计的python包
 GisPandas是一个为栅格、矢量数据处理、分析以及可视化而开发的Python包。GisPandas为常见栅格矢量数据提供了快速而简洁的gis操作方法，代码简洁、高效、灵活、易用，可以用简洁的代码实现复杂的数据任务。
 # 主要功能
 目前，GisPandas主要提供以下方法：
 
 1.栅格数据进行阿尔伯斯等面积投影，根据矢量区划计算面积并导出json。
 
-2.种植结构变化,自动对齐，导出栅格数据和统计json。
+2.种植结构变化，自动对齐，导出栅格数据和统计json。
 
 3.gee下载数据的后处理主要包括：栅格数据镶嵌并压缩。
 
 4.矢量数据写入四至、中心经纬度等属性，矢量简化，文本矢量化等。
 
 5.栅格数据像素对齐、裁剪、重采样、投影、插值、切片、格式转换等。
 # 安装
```

### Comparing `gispandas-0.1.8/gispandas/mxclf.py` & `gispandas-0.1.9/gispandas/mxclf.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import time
 from osgeo import gdal
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 import rasterio
 import rasterio.mask
-from mxgdal import *
+from gispandas.mxgdal import *
 from rasterio.warp import Resampling, calculate_default_transform, reproject
 from rasterstats import zonal_stats
 
 
 
 def tif2area(intif,inshp,class_dic,outjson,resolution=10,year=time.strftime('%Y'),code = 'code',name = 'name'):
     '''根据矢量区划统计tif数据的面积
```

### Comparing `gispandas-0.1.8/gispandas/mxgdal.py` & `gispandas-0.1.9/gispandas/mxgdal.py`

 * *Files identical despite different names*

### Comparing `gispandas-0.1.8/gispandas/mxgee.py` & `gispandas-0.1.9/gispandas/mxgee.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 '''
 
 # here put the import lib
 import numpy as np
 from osgeo import gdal
 import os
 import time
-from mxgdal import *
+from gispandas.mxgdal import *
 
 
 
 def merge_geetif(infp,outfp,lzw = True):
     '''镶嵌gee下载的栅格数据
 
     :param infp: 待镶嵌的栅格数据的文件夹路径
```

### Comparing `gispandas-0.1.8/gispandas/mxgpd.py` & `gispandas-0.1.9/gispandas/mxgpd.py`

 * *Files identical despite different names*

### Comparing `gispandas-0.1.8/gispandas.egg-info/PKG-INFO` & `gispandas-0.1.9/gispandas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gispandas
-Version: 0.1.8
+Version: 0.1.9
 Summary: gispandas
 Home-page: https://github.com/mxhou/gispandas/
 Author: HMX
 Author-email: kzdhb8023@163.com
 License: MIT
 Keywords: gis,geo,tif,json,shp
 Requires-Python: >=3.6
@@ -13,15 +13,15 @@
 # GisPandas针对栅格数据进行统计的python包
 GisPandas是一个为栅格、矢量数据处理、分析以及可视化而开发的Python包。GisPandas为常见栅格矢量数据提供了快速而简洁的gis操作方法，代码简洁、高效、灵活、易用，可以用简洁的代码实现复杂的数据任务。
 # 主要功能
 目前，GisPandas主要提供以下方法：
 
 1.栅格数据进行阿尔伯斯等面积投影，根据矢量区划计算面积并导出json。
 
-2.种植结构变化,自动对齐，导出栅格数据和统计json。
+2.种植结构变化，自动对齐，导出栅格数据和统计json。
 
 3.gee下载数据的后处理主要包括：栅格数据镶嵌并压缩。
 
 4.矢量数据写入四至、中心经纬度等属性，矢量简化，文本矢量化等。
 
 5.栅格数据像素对齐、裁剪、重采样、投影、插值、切片、格式转换等。
 # 安装
```

### Comparing `gispandas-0.1.8/setup.py` & `gispandas-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 filepath = path.join(this_directory, 'README.md')
-VERSION = '0.1.8'
+VERSION = '0.1.9'
 setup(
     name='gispandas',  # package name
     version=VERSION,  # package version
     author="HMX",
     author_email="kzdhb8023@163.com",
     description='gispandas',  # package description
     packages=find_packages(),
```

