# Comparing `tmp/gispandas-0.1.7.tar.gz` & `tmp/gispandas-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gispandas-0.1.7.tar", last modified: Tue Jul 11 13:42:10 2023, max compression
+gzip compressed data, was "gispandas-0.1.8.tar", last modified: Fri Jul 14 07:29:21 2023, max compression
```

## Comparing `gispandas-0.1.7.tar` & `gispandas-0.1.8.tar`

### file list

```diff
@@ -1,19 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 13:42:10.708968 gispandas-0.1.7/
--rw-rw-rw-   0        0        0     1204 2023-07-11 13:42:10.707971 gispandas-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      909 2023-07-11 13:32:05.000000 gispandas-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 13:42:10.696003 gispandas-0.1.7/gispandas/
--rw-rw-rw-   0        0        0      366 2023-07-11 13:17:54.000000 gispandas-0.1.7/gispandas/__init__.py
--rw-rw-rw-   0        0        0    11760 2023-07-11 13:09:28.000000 gispandas-0.1.7/gispandas/gago_gdal.py
--rw-rw-rw-   0        0        0     2056 2023-07-11 13:36:06.000000 gispandas-0.1.7/gispandas/geemerge.py
--rw-rw-rw-   0        0        0     3326 2023-07-11 13:35:49.000000 gispandas-0.1.7/gispandas/mxgdal.py
--rw-rw-rw-   0        0        0     2561 2023-07-11 12:53:22.000000 gispandas-0.1.7/gispandas/shpinfo.py
--rw-rw-rw-   0        0        0     3280 2023-07-11 13:02:48.000000 gispandas-0.1.7/gispandas/tifarea.py
--rw-rw-rw-   0        0        0     1642 2023-07-11 13:35:08.000000 gispandas-0.1.7/gispandas/tifchange.py
-drwxrwxrwx   0        0        0        0 2023-07-11 13:42:10.705977 gispandas-0.1.7/gispandas.egg-info/
--rw-rw-rw-   0        0        0     1204 2023-07-11 13:42:10.000000 gispandas-0.1.7/gispandas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      365 2023-07-11 13:42:10.000000 gispandas-0.1.7/gispandas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 13:42:10.000000 gispandas-0.1.7/gispandas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-11 13:42:10.000000 gispandas-0.1.7/gispandas.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-07-11 13:42:10.000000 gispandas-0.1.7/gispandas.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 13:42:10.708968 gispandas-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      870 2023-07-11 13:41:16.000000 gispandas-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:29:21.540085 gispandas-0.1.8/
+-rw-rw-rw-   0        0        0     1313 2023-07-14 07:29:21.540085 gispandas-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1009 2023-07-14 07:28:15.000000 gispandas-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 07:29:21.530111 gispandas-0.1.8/gispandas/
+-rw-rw-rw-   0        0        0      308 2023-07-14 06:50:55.000000 gispandas-0.1.8/gispandas/__init__.py
+-rw-rw-rw-   0        0        0     5913 2023-07-14 07:28:45.000000 gispandas-0.1.8/gispandas/mxclf.py
+-rw-rw-rw-   0        0        0    18038 2023-07-14 06:06:06.000000 gispandas-0.1.8/gispandas/mxgdal.py
+-rw-rw-rw-   0        0        0     1457 2023-07-14 05:32:01.000000 gispandas-0.1.8/gispandas/mxgee.py
+-rw-rw-rw-   0        0        0     2787 2023-07-14 06:09:39.000000 gispandas-0.1.8/gispandas/mxgpd.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:29:21.538088 gispandas-0.1.8/gispandas.egg-info/
+-rw-rw-rw-   0        0        0     1313 2023-07-14 07:29:21.000000 gispandas-0.1.8/gispandas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-07-14 07:29:21.000000 gispandas-0.1.8/gispandas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 07:29:21.000000 gispandas-0.1.8/gispandas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-14 07:25:00.000000 gispandas-0.1.8/gispandas.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2023-07-14 07:29:21.000000 gispandas-0.1.8/gispandas.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 07:29:21.541082 gispandas-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      876 2023-07-14 07:28:10.000000 gispandas-0.1.8/setup.py
```

### Comparing `gispandas-0.1.7/README.md` & `gispandas-0.1.8/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 # GisPandas针对栅格数据进行统计的python包
 GisPandas是一个为栅格、矢量数据处理、分析以及可视化而开发的Python包。GisPandas为常见栅格矢量数据提供了快速而简洁的gis操作方法，代码简洁、高效、灵活、易用，可以用简洁的代码实现复杂的数据任务。
 # 主要功能
 目前，GisPandas主要提供以下方法：
+
 1.栅格数据进行阿尔伯斯等面积投影，根据矢量区划计算面积并导出json。
-2.种植结构变化。
-3.gee栅格数据镶嵌并压缩。
-4.矢量数据写入四至、置信等属性，矢量简化，文本矢量化等。
+
+2.种植结构变化,自动对齐，导出栅格数据和统计json。
+
+3.gee下载数据的后处理主要包括：栅格数据镶嵌并压缩。
+
+4.矢量数据写入四至、中心经纬度等属性，矢量简化，文本矢量化等。
+
 5.栅格数据像素对齐、裁剪、重采样、投影、插值、切片、格式转换等。
 # 安装
 pip install gispandas
 # 相关链接
 本项目的github页面：https://github.com/mxhou/gispandas
 
 有bug请在这个页面提交：https://github.com/mxhou/gispandas/issues
```

### Comparing `gispandas-0.1.7/gispandas/shpinfo.py` & `gispandas-0.1.8/gispandas/mxgpd.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import geopandas as gpd
 import os
 import warnings
 import pandas as pd
 from shapely import geometry
 warnings.filterwarnings('ignore')
 
-def write_info(shp,outshp=None):
+def shpinfo(shp,outshp=None):
     '''写入矢量数据的四至和中心经纬度
 
     :param shp: 待计算的矢量文件路径
     :param outshp:计算后的输出文件路径, defaults to None
     '''
     gdf = gpd.read_file(shp,engine = 'pyogrio')
     gdf['lon'] = gdf.centroid.x
@@ -78,7 +78,16 @@
     :param outshp: 简化后的矢量
     :param EPSG: 投影的坐标系代码, defaults to 4326
     '''
     gdf = gpd.read_file(fn).to_crs(f'EPSG:{EPSG}')
     gdf['geometry'] = gdf['geometry'].simplify(tolerance=0.1, preserve_topology=False)
     gdf.to_file(outshp,encoding='utf-8')
 
+
+def projshp(shp,outshp,EPSG = 4490):
+    '''投影矢量
+
+    :param shp: 待投影矢量路径
+    :param outshp: 投影后矢量路径
+    '''
+    gdf = gpd.read_file(shp).to_crs(f'EPSG:{EPSG}')
+    gdf.to_file(outshp)
```

### Comparing `gispandas-0.1.7/setup.py` & `gispandas-0.1.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 filepath = path.join(this_directory, 'README.md')
-VERSION = '0.1.7'
+VERSION = '0.1.8'
 setup(
     name='gispandas',  # package name
     version=VERSION,  # package version
     author="HMX",
     author_email="kzdhb8023@163.com",
     description='gispandas',  # package description
     packages=find_packages(),
     url="https://github.com/mxhou/gispandas/",
     zip_safe=False,
     # What packages are required for this module to be executed?
     REQUIRED = ['geopandas', 'numpy','json','rasterio','rasterstats','gdal'],
     license='MIT',
     python_requires=">=3.6",
-    keywords=['gis','geo','tif','json'],
+    keywords=['gis','geo','tif','json','shp'],
     data_files=[filepath],
     long_description=open(filepath, encoding='utf-8').read(),
     long_description_content_type='text/markdown'
 )
```

