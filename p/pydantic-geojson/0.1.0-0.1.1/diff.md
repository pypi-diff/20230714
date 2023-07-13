# Comparing `tmp/pydantic_geojson-0.1.0.tar.gz` & `tmp/pydantic_geojson-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_geojson-0.1.0.tar", max compression
+gzip compressed data, was "pydantic_geojson-0.1.1.tar", max compression
```

## Comparing `pydantic_geojson-0.1.0.tar` & `pydantic_geojson-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     1077 2022-01-16 21:08:27.904000 pydantic_geojson-0.1.0/LICENSE
--rw-r--r--   0        0        0    10462 2022-03-27 21:46:19.593340 pydantic_geojson-0.1.0/README.md
--rw-r--r--   0        0        0      912 2022-01-19 20:16:07.670160 pydantic_geojson-0.1.0/pydantic_geojson/__init__.py
--rw-r--r--   0        0        0     1477 2023-04-10 20:43:17.804226 pydantic_geojson-0.1.0/pydantic_geojson/_base.py
--rw-r--r--   0        0        0      579 2022-01-19 20:15:45.520690 pydantic_geojson-0.1.0/pydantic_geojson/feature.py
--rw-r--r--   0        0        0      724 2022-01-19 20:10:00.168102 pydantic_geojson-0.1.0/pydantic_geojson/feature_collection.py
--rw-r--r--   0        0        0      669 2022-01-19 21:53:21.864629 pydantic_geojson-0.1.0/pydantic_geojson/geometry_collection.py
--rw-r--r--   0        0        0      216 2022-01-19 20:06:35.961738 pydantic_geojson-0.1.0/pydantic_geojson/line_string.py
--rw-r--r--   0        0        0      251 2022-01-19 20:06:18.826313 pydantic_geojson-0.1.0/pydantic_geojson/multi_line_string.py
--rw-r--r--   0        0        0      216 2022-01-19 20:06:04.567018 pydantic_geojson-0.1.0/pydantic_geojson/multi_point.py
--rw-r--r--   0        0        0      270 2022-01-19 20:05:45.468348 pydantic_geojson-0.1.0/pydantic_geojson/multi_polygon.py
--rw-r--r--   0        0        0      836 2022-01-19 17:15:44.273212 pydantic_geojson-0.1.0/pydantic_geojson/object_type.py
--rw-r--r--   0        0        0      170 2022-01-19 20:05:05.802095 pydantic_geojson-0.1.0/pydantic_geojson/point.py
--rw-r--r--   0        0        0      227 2022-01-19 20:04:21.640066 pydantic_geojson-0.1.0/pydantic_geojson/polygon.py
--rw-r--r--   0        0        0     1269 2023-04-10 20:43:49.045564 pydantic_geojson-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    11553 2023-04-10 20:55:48.257503 pydantic_geojson-0.1.0/setup.py
--rw-r--r--   0        0        0    11514 2023-04-10 20:55:48.258262 pydantic_geojson-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2022-01-16 21:08:27.904000 pydantic_geojson-0.1.1/LICENSE
+-rw-r--r--   0        0        0    10462 2022-03-27 21:46:19.593340 pydantic_geojson-0.1.1/README.md
+-rw-r--r--   0        0        0      909 2023-07-13 21:36:18.919640 pydantic_geojson-0.1.1/pydantic_geojson/__init__.py
+-rw-r--r--   0        0        0     1333 2023-07-13 21:36:18.920047 pydantic_geojson-0.1.1/pydantic_geojson/_base.py
+-rw-r--r--   0        0        0      579 2022-01-19 20:15:45.520690 pydantic_geojson-0.1.1/pydantic_geojson/feature.py
+-rw-r--r--   0        0        0      724 2022-01-19 20:10:00.168102 pydantic_geojson-0.1.1/pydantic_geojson/feature_collection.py
+-rw-r--r--   0        0        0      669 2022-01-19 21:53:21.864629 pydantic_geojson-0.1.1/pydantic_geojson/geometry_collection.py
+-rw-r--r--   0        0        0      216 2022-01-19 20:06:35.961738 pydantic_geojson-0.1.1/pydantic_geojson/line_string.py
+-rw-r--r--   0        0        0      237 2023-07-13 21:36:18.920916 pydantic_geojson-0.1.1/pydantic_geojson/multi_line_string.py
+-rw-r--r--   0        0        0      216 2022-01-19 20:06:04.567018 pydantic_geojson-0.1.1/pydantic_geojson/multi_point.py
+-rw-r--r--   0        0        0      234 2023-07-13 21:36:18.921523 pydantic_geojson-0.1.1/pydantic_geojson/multi_polygon.py
+-rw-r--r--   0        0        0      837 2023-07-13 21:36:18.924501 pydantic_geojson-0.1.1/pydantic_geojson/object_type.py
+-rw-r--r--   0        0        0      170 2022-01-19 20:05:05.802095 pydantic_geojson-0.1.1/pydantic_geojson/point.py
+-rw-r--r--   0        0        0      213 2023-07-13 21:36:18.924889 pydantic_geojson-0.1.1/pydantic_geojson/polygon.py
+-rw-r--r--   0        0        0     1345 2023-07-13 21:36:18.927870 pydantic_geojson-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    11598 1970-01-01 00:00:00.000000 pydantic_geojson-0.1.1/PKG-INFO
```

### Comparing `pydantic_geojson-0.1.0/LICENSE` & `pydantic_geojson-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_geojson-0.1.0/README.md` & `pydantic_geojson-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_geojson-0.1.0/pydantic_geojson/__init__.py` & `pydantic_geojson-0.1.1/pydantic_geojson/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,34 +5,31 @@
 from .multi_line_string import MultiLineStringModel
 from .multi_point import MultiPointModel
 from .multi_polygon import MultiPolygonModel
 from .object_type import GeometryType
 from .point import PointModel
 from .polygon import PolygonModel
 
-__author__ = 'Aliaksandr Vaskevich'
+__author__ = "Aliaksandr Vaskevich"
 __maintainer__ = __author__
 
-__email__ = 'vaskevic.an@gmail.com'
-__license__ = 'MIT'
+__email__ = "vaskevic.an@gmail.com"
+__license__ = "MIT"
 
 __all__ = [
-    '__author__',
-    '__email__',
-    '__license__',
-    '__maintainer__',
-
+    "__author__",
+    "__email__",
+    "__license__",
+    "__maintainer__",
     # object type
-    'GeometryType',
-
+    "GeometryType",
     # models
-    'PointModel',
-    'MultiPointModel',
-    'LineStringModel',
-    'MultiLineStringModel',
-    'PolygonModel',
-    'MultiPolygonModel',
-    'GeometryCollectionModel',
-    'FeatureModel',
-    'FeatureCollectionModel',
-
+    "PointModel",
+    "MultiPointModel",
+    "LineStringModel",
+    "MultiLineStringModel",
+    "PolygonModel",
+    "MultiPolygonModel",
+    "GeometryCollectionModel",
+    "FeatureModel",
+    "FeatureCollectionModel",
 ]
```

### Comparing `pydantic_geojson-0.1.0/pydantic_geojson/_base.py` & `pydantic_geojson-0.1.1/pydantic_geojson/_base.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,80 +14,71 @@
     POINT,
     POLYGON,
 )
 
 LonField = Annotated[
     Union[float, int],
     Field(
-        title='Coordinate longitude',
+        title="Coordinate longitude",
         ge=-180,
         le=180,
     ),
 ]
 
 LatField = Annotated[
     Union[float, int],
     Field(
-        title='Coordinate latitude',
+        title="Coordinate latitude",
         ge=-90,
         le=90,
     ),
 ]
 
 PointFieldType = Field(
     POINT,
-    const=True,
-    title='Point',
+    title="Point",
 )
 
 MultiPointFieldType = Field(
     MULTI_POINT,
-    const=True,
-    title='Multi Point',
+    title="Multi Point",
 )
 
 LineStringFieldType = Field(
     LINE_STRING,
-    const=True,
-    title='LineS String',
+    title="LineS String",
 )
 
 MultiLineStringFieldType = Field(
     MULTI_LINE_STRING,
-    const=True,
-    title='Multi Line String',
+    title="Multi Line String",
 )
 
 PolygonFieldType = Field(
     POLYGON,
-    const=True,
-    title='Polygon',
+    title="Polygon",
 )
 
 MultiPolygonFieldType = Field(
     MULTI_POLYGON,
-    const=True,
-    title='Multi Polygon',
+    title="Multi Polygon",
 )
 
 GeometryCollectionFieldType = Field(
     GEOMETRY_COLLECTION,
-    const=True,
-    title='Geometry Collection',
+    title="Geometry Collection",
 )
 
 FeatureFieldType = Field(
     FEATURE,
-    const=True,
-    title='Feature',
+    title="Feature",
 )
 
 FeatureCollectionFieldType = Field(
     FEATURE_COLLECTION,
-    const=True,
-    title='Feature Collection',
+    title="Feature Collection",
 )
 
 
 class Coordinates(NamedTuple):
     lon: LonField
     lat: LatField
```

### Comparing `pydantic_geojson-0.1.0/pydantic_geojson/feature.py` & `pydantic_geojson-0.1.1/pydantic_geojson/feature.py`

 * *Files identical despite different names*

### Comparing `pydantic_geojson-0.1.0/pydantic_geojson/feature_collection.py` & `pydantic_geojson-0.1.1/pydantic_geojson/feature_collection.py`

 * *Files identical despite different names*

### Comparing `pydantic_geojson-0.1.0/pydantic_geojson/geometry_collection.py` & `pydantic_geojson-0.1.1/pydantic_geojson/geometry_collection.py`

 * *Files identical despite different names*

### Comparing `pydantic_geojson-0.1.0/pydantic_geojson/object_type.py` & `pydantic_geojson-0.1.1/pydantic_geojson/object_type.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 from enum import Enum
 
 """
 https://www.rfc-editor.org/rfc/rfc7946.html#section-1.4
 """
 
-POINT = 'Point'
-MULTI_POINT = 'MultiPoint'
-LINE_STRING = 'LineString'
-MULTI_LINE_STRING = 'MultiLineString'
-POLYGON = 'Polygon'
-MULTI_POLYGON = 'MultiPolygon'
-GEOMETRY_COLLECTION = 'GeometryCollection'
+POINT = "Point"
+MULTI_POINT = "MultiPoint"
+LINE_STRING = "LineString"
+MULTI_LINE_STRING = "MultiLineString"
+POLYGON = "Polygon"
+MULTI_POLYGON = "MultiPolygon"
+GEOMETRY_COLLECTION = "GeometryCollection"
 
 
 class GeometryType(str, Enum):
     """
     Inside this document, the term "geometry type" refers to seven
     case-sensitive strings: "Point", "MultiPoint", "LineString",
     "MultiLineString", "Polygon", "MultiPolygon", and
     "GeometryCollection".
     """
+
     point = POINT
     multi_point = MULTI_POINT
     line_string = LINE_STRING
     multi_line_string = MULTI_LINE_STRING
     polygon = POLYGON
     multi_polygon = MULTI_POLYGON
     geometry_collection = GEOMETRY_COLLECTION
 
 
-FEATURE = 'Feature'
-FEATURE_COLLECTION = 'FeatureCollection'
+FEATURE = "Feature"
+FEATURE_COLLECTION = "FeatureCollection"
```

### Comparing `pydantic_geojson-0.1.0/pyproject.toml` & `pydantic_geojson-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic_geojson"
-version = "0.1.0"
+version = "0.1.1"
 description = "Pydantic validation for GeoJson"
 authors = [
   "Aliaksandr Vaskevich <vaskevic.an@gmail.com>",
 ]
 license = "MIT"
 readme = "README.md"
 
@@ -37,21 +37,25 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: Implementation :: CPython",
   "License :: OSI Approved :: MIT License",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-pydantic = "^1.9.0"
+pydantic = ">=1.9,<3.0"
+mypy = "^1.4.1"
 
 [tool.poetry.dev-dependencies]
 isort = "^5.10.1"
 pytest = "^7.1.1"
 pytest-cov = "^4.0.0"
 
+[tool.poetry.group.dev.dependencies]
+bandit = "^1.7.5"
+
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.isort]
 profile = "hug"
 src_paths = ["isort", "tests"]
```

### Comparing `pydantic_geojson-0.1.0/setup.py` & `pydantic_geojson-0.1.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,395 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pydantic-geojson
+Version: 0.1.1
+Summary: Pydantic validation for GeoJson
+Home-page: https://github.com/gb-libs/pydantic-geojson
+License: MIT
+Keywords: pydantic,validation,geojson,schema,gis,geo,json,json-schema,rest,fastapi,swagger,openapi
+Author: Aliaksandr Vaskevich
+Author-email: vaskevic.an@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Scientific/Engineering :: GIS
+Requires-Dist: mypy (>=1.4.1,<2.0.0)
+Requires-Dist: pydantic (>=1.9,<3.0)
+Project-URL: Documentation, https://github.com/gb-libs/pydantic-geojson
+Project-URL: Repository, https://github.com/gb-libs/pydantic-geojson
+Description-Content-Type: text/markdown
 
-packages = \
-['pydantic_geojson']
+[![GitHub Actions status for master branch](https://github.com/gb-libs/pydantic-geojson/actions/workflows/main.yml/badge.svg)](https://github.com/gb-libs/pydantic-geojson/actions?query=workflow%3A%22Python+package%22)
+[![Latest PyPI package version](https://badge.fury.io/py/pydantic-geojson.svg)](https://pypi.org/project/pydantic-geojson/)
+[![codecov](https://codecov.io/gh/gb-libs/pydantic-geojson/branch/master/graph/badge.svg?token=8LMKSDQTIR)](https://codecov.io/gh/gb-libs/pydantic-geojson)
+[![Downloads](https://static.pepy.tech/personalized-badge/pydantic-geojson?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads)](https://pepy.tech/project/pydantic-geojson)
 
-package_data = \
-{'': ['*']}
+pydantic-geojson 🌍
+===================
 
-install_requires = \
-['pydantic>=1.9.0,<2.0.0']
-
-setup_kwargs = {
-    'name': 'pydantic-geojson',
-    'version': '0.1.0',
-    'description': 'Pydantic validation for GeoJson',
-    'long_description': '[![GitHub Actions status for master branch](https://github.com/gb-libs/pydantic-geojson/actions/workflows/main.yml/badge.svg)](https://github.com/gb-libs/pydantic-geojson/actions?query=workflow%3A%22Python+package%22)\n[![Latest PyPI package version](https://badge.fury.io/py/pydantic-geojson.svg)](https://pypi.org/project/pydantic-geojson/)\n[![codecov](https://codecov.io/gh/gb-libs/pydantic-geojson/branch/master/graph/badge.svg?token=8LMKSDQTIR)](https://codecov.io/gh/gb-libs/pydantic-geojson)\n[![Downloads](https://static.pepy.tech/personalized-badge/pydantic-geojson?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads)](https://pepy.tech/project/pydantic-geojson)\n\npydantic-geojson 🌍\n===================\n\n\n| GeoJSON Objects    | Status |\n|--------------------|--------|\n| Point              | ✅      |\n| MultiPoint         | ✅      |\n| LineString         | ✅      |\n| MultiLineString    | ✅      |\n| Polygon            | ✅      |\n| MultiPolygon       | ✅      |\n| GeometryCollection | ✅      |\n| Feature            | ✅      |\n| FeatureCollection  | ✅      |\n\nInstallation\n------------\n\npydantic-geojson is compatible with Python 3.7 and up.\nThe recommended way to install is via [poetry](https://python-poetry.org/):\n\n```\npoetry add pydantic_geojson\n```\n\nUsing pip to install is also possible.\n\n```\npip install pydantic_geojson\n```\n\nGEOJSON\n-------\n\n[GeoJSON](https://geojson.org/) is a format for encoding a variety of geographic data structures.\n\n```\n{\n    "type": "Feature",\n    "geometry": {\n        "type": "Point",\n        "coordinates": [125.6, 10.1]\n    },\n    "properties": {\n        "name": "Dinagat Islands"\n    }\n}\n```\n\nGeoJSON supports the following geometry types: Point, LineString, Polygon,\nMultiPoint, MultiLineString, and MultiPolygon. Geometric objects with\nadditional properties are Feature objects. Sets of features are contained by\nFeatureCollection objects.\n\nExamples of using\n-----------------\n\nCustom properties:\n\n```\nfrom pydantic import BaseModel\nfrom pydantic_geojson import FeatureModel\n\n\nclass MyPropertiesModel(BaseModel):\n    name: str\n\n\nclass MyFeatureModel(FeatureModel):\n    properties: MyPropertiesModel\n\n\ndata = {\n    "type": "Feature",\n    "properties": {\n        "name": "foo name",\n    },\n    "geometry": {\n        "type": "Polygon",\n        "coordinates": [\n            [\n                [-80.724878, 35.265454],\n                [-80.722646, 35.260338]\n            ]\n        ]\n    }\n}\n\n>>> MyFeatureModel(**data)\n>>> type=\'Feature\' geometry=PolygonModel(type=\'Polygon\', coordinates=[[Coordinates(lon=-80.724878, lat=35.265454), Coordinates(lon=-80.722646, lat=35.260338)]]) properties=MyPropertiesModel(name=\'foo name\')\n```\n\nPoint\n-----\n\nSimple example data:\n\n```\nfrom pydantic_geojson import PointModel\n\ndata = {\n    "type": "Point",\n    "coordinates": [-105.01621, 39.57422]\n}\n\n>>> PointModel(**data)\n>>> type=\'Point\' coordinates=Coordinates(lon=-105.01621, lat=39.57422)\n```\n\nMultiPoint\n----------\n\nSimple example data:\n\n```\nfrom pydantic_geojson import MultiPointModel\n\ndata = {\n    "type": "MultiPoint",\n    "coordinates": [\n        [-105.01621, 39.57422],\n        [-80.666513, 35.053994]\n    ]\n}\n\n>>> PointModel(**data)\n>>> type=\'MultiPoint\' coordinates=[Coordinates(lon=-105.01621, lat=39.57422), Coordinates(lon=-80.666513, lat=35.053994)]\n```\n\nLineString\n----------\n\nSimple example data:\n\n```\nfrom pydantic_geojson import LineStringModel\n\ndata = {\n    "type": "LineString",\n    "coordinates": [\n        [-99.113159, 38.869651],\n        [-99.0802, 38.85682],\n        [-98.822021, 38.85682],\n        [-98.448486, 38.848264]\n    ]\n}\n\n>>> LineStringModel(**data)\n>>> type=\'LineString\' coordinates=[Coordinates(lon=-99.113159, lat=38.869651), Coordinates(lon=-99.0802, lat=38.85682), Coordinates(lon=-98.822021, lat=38.85682), Coordinates(lon=-98.448486, lat=38.848264)]\n```\n\nMultiLineString\n---------------\n\nSimple example data:\n\n```\nfrom pydantic_geojson import MultiLineStringModel\n\ndata = {\n    "type": "MultiLineString",\n    "coordinates": [\n        [\n            [-105.019898, 39.574997],\n            [-105.019598, 39.574898],\n            [-105.019061, 39.574782]\n        ],\n        [\n            [-105.017173, 39.574402],\n            [-105.01698, 39.574385],\n            [-105.016636, 39.574385],\n            [-105.016508, 39.574402],\n            [-105.01595, 39.57427]\n        ],\n        [\n            [-105.014276, 39.573972],\n            [-105.014126, 39.574038],\n            [-105.013825, 39.57417],\n            [-105.01331, 39.574452]\n        ]\n    ]\n}\n\n>>> MultiLineStringModel(**data)\n>>> type=\'MultiLineString\' coordinates=[[Coordinates(lon=-105.019898, lat=39.574997), Coordinates(lon=-105.019598, lat=39.574898), Coordinates(lon=-105.019061, lat=39.574782)], [Coordinates(lon=-105.017173, lat=39.574402), Coordinates(lon=-105.01698, lat=39.574385), Coordinates(lon=-105.016636, lat=39.574385), Coordinates(lon=-105.016508, lat=39.574402), Coordinates(lon=-105.01595, lat=39.57427)], [Coordinates(lon=-105.014276, lat=39.573972), Coordinates(lon=-105.014126, lat=39.574038), Coordinates(lon=-105.013825, lat=39.57417), Coordinates(lon=-105.01331, lat=39.574452)]]\n```\n\nPolygon\n-------\n\nSimple example data:\n\n```\nfrom pydantic_geojson import PolygonModel\n\ndata = {\n    "type": "Polygon",\n    "coordinates": [\n        [\n            [100, 0],\n            [101, 0],\n            [101, 1],\n            [100, 1],\n            [100, 0]\n        ]\n    ]\n}\n\n>>> PolygonModel(**data)\n>>> type=\'Polygon\' coordinates=[[Coordinates(lon=100.0, lat=0.0), Coordinates(lon=101.0, lat=0.0), Coordinates(lon=101.0, lat=1.0), Coordinates(lon=100.0, lat=1.0), Coordinates(lon=100.0, lat=0.0)]]\n```\n\nMultiPolygon\n------------\n\nSimple example data:\n\n```\nfrom pydantic_geojson import MultiPolygonModel\n\ndata = {\n    "type": "MultiPolygon",\n    "coordinates": [\n        [\n            [\n                [107, 7],\n                [108, 7],\n                [108, 8],\n                [107, 8],\n                [107, 7]\n            ]\n        ],\n        [\n            [\n                [100, 0],\n                [101, 0],\n                [101, 1],\n                [100, 1],\n                [100, 0]\n            ]\n        ]\n    ]\n}\n\n>>> MultiPolygonModel(**data)\n>>> type=\'MultiPolygon\' coordinates=[[[Coordinates(lon=107.0, lat=7.0), Coordinates(lon=108.0, lat=7.0), Coordinates(lon=108.0, lat=8.0), Coordinates(lon=107.0, lat=8.0), Coordinates(lon=107.0, lat=7.0)]], [[Coordinates(lon=100.0, lat=0.0), Coordinates(lon=101.0, lat=0.0), Coordinates(lon=101.0, lat=1.0), Coordinates(lon=100.0, lat=1.0), Coordinates(lon=100.0, lat=0.0)]]]\n```\n\nGeometryCollection\n------------------\n\nSimple example data:\n\n```\nfrom pydantic_geojson import GeometryCollectionModel\n\ndata = {\n    "type": "GeometryCollection",\n    "geometries": [\n        {\n            "type": "Point",\n            "coordinates": [-80.660805, 35.049392]\n        },\n        {\n            "type": "Polygon",\n            "coordinates": [\n                [\n                    [-80.664582, 35.044965],\n                    [-80.663874, 35.04428],\n                    [-80.662586, 35.04558],\n                    [-80.663444, 35.046036],\n                    [-80.664582, 35.044965]\n                ]\n            ]\n        },\n        {\n            "type": "LineString",\n            "coordinates": [\n                [-80.662372, 35.059509],\n                [-80.662693, 35.059263],\n                [-80.662844, 35.05893]\n            ]\n        }\n    ]\n}\n\n>>> GeometryCollectionModel(**data)\n>>> type=\'GeometryCollection\' geometries=[PointModel(type=\'Point\', coordinates=Coordinates(lon=-80.660805, lat=35.049392)), PolygonModel(type=\'Polygon\', coordinates=[[Coordinates(lon=-80.664582, lat=35.044965), Coordinates(lon=-80.663874, lat=35.04428), Coordinates(lon=-80.662586, lat=35.04558), Coordinates(lon=-80.663444, lat=35.046036), Coordinates(lon=-80.664582, lat=35.044965)]]), LineStringModel(type=\'LineString\', coordinates=[Coordinates(lon=-80.662372, lat=35.059509), Coordinates(lon=-80.662693, lat=35.059263), Coordinates(lon=-80.662844, lat=35.05893)])]\n```\n\nFeature\n-------\n\nSimple example data:\n\n```\nfrom pydantic_geojson import FeatureModel\n\ndata = {\n    "type": "Feature",\n    "geometry": {\n        "type": "Polygon",\n        "coordinates": [\n            [\n                [-80.724878, 35.265454],\n                [-80.722646, 35.260338],\n                [-80.720329, 35.260618],\n                [-80.71681, 35.255361],\n                [-80.704793, 35.268397],\n                [-82.715179, 35.267696],\n                [-80.721359, 35.267276],\n                [-80.724878, 35.265454]\n            ]\n        ]\n    }\n}\n\n>>> FeatureModel(**data)\n>>> type=\'Feature\' geometry=PolygonModel(type=\'Polygon\', coordinates=[[Coordinates(lon=-80.724878, lat=35.265454), Coordinates(lon=-80.722646, lat=35.260338), Coordinates(lon=-80.720329, lat=35.260618), Coordinates(lon=-80.71681, lat=35.255361), Coordinates(lon=-80.704793, lat=35.268397), Coordinates(lon=-82.715179, lat=35.267696), Coordinates(lon=-80.721359, lat=35.267276), Coordinates(lon=-80.724878, lat=35.265454)]])\n\n```\n\nFeatureCollection\n-----------------\n\nSimple example data:\n\n```\nfrom pydantic_geojson import FeatureCollectionModel\n\ndata = {\n    "type": "FeatureCollection",\n    "features": [\n        {\n            "type": "Feature",\n            "geometry": {\n                "type": "Point",\n                "coordinates": [-80.870885, 35.215151]\n            }\n        },\n        {\n            "type": "Feature",\n            "geometry": {\n                "type": "Polygon",\n                "coordinates": [\n                    [\n                        [-80.724878, 35.265454],\n                        [-80.722646, 35.260338],\n                        [-80.720329, 35.260618],\n                        [-80.704793, 35.268397],\n                        [-80.724878, 35.265454]\n                    ]\n                ]\n            }\n        }\n    ]\n}\n\n>>> FeatureCollectionModel(**data)\n>>> type=\'FeatureCollection\' features=[FeatureModel(type=\'Feature\', geometry=PointModel(type=\'Point\', coordinates=Coordinates(lon=-80.870885, lat=35.215151))), FeatureModel(type=\'Feature\', geometry=PolygonModel(type=\'Polygon\', coordinates=[[Coordinates(lon=-80.724878, lat=35.265454), Coordinates(lon=-80.722646, lat=35.260338), Coordinates(lon=-80.720329, lat=35.260618), Coordinates(lon=-80.704793, lat=35.268397), Coordinates(lon=-80.724878, lat=35.265454)]]))]\n\n```\n',
-    'author': 'Aliaksandr Vaskevich',
-    'author_email': 'vaskevic.an@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/gb-libs/pydantic-geojson',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
+
+| GeoJSON Objects    | Status |
+|--------------------|--------|
+| Point              | ✅      |
+| MultiPoint         | ✅      |
+| LineString         | ✅      |
+| MultiLineString    | ✅      |
+| Polygon            | ✅      |
+| MultiPolygon       | ✅      |
+| GeometryCollection | ✅      |
+| Feature            | ✅      |
+| FeatureCollection  | ✅      |
+
+Installation
+------------
+
+pydantic-geojson is compatible with Python 3.7 and up.
+The recommended way to install is via [poetry](https://python-poetry.org/):
+
+```
+poetry add pydantic_geojson
+```
+
+Using pip to install is also possible.
+
+```
+pip install pydantic_geojson
+```
+
+GEOJSON
+-------
+
+[GeoJSON](https://geojson.org/) is a format for encoding a variety of geographic data structures.
+
+```
+{
+    "type": "Feature",
+    "geometry": {
+        "type": "Point",
+        "coordinates": [125.6, 10.1]
+    },
+    "properties": {
+        "name": "Dinagat Islands"
+    }
+}
+```
+
+GeoJSON supports the following geometry types: Point, LineString, Polygon,
+MultiPoint, MultiLineString, and MultiPolygon. Geometric objects with
+additional properties are Feature objects. Sets of features are contained by
+FeatureCollection objects.
+
+Examples of using
+-----------------
+
+Custom properties:
+
+```
+from pydantic import BaseModel
+from pydantic_geojson import FeatureModel
+
+
+class MyPropertiesModel(BaseModel):
+    name: str
+
+
+class MyFeatureModel(FeatureModel):
+    properties: MyPropertiesModel
+
+
+data = {
+    "type": "Feature",
+    "properties": {
+        "name": "foo name",
+    },
+    "geometry": {
+        "type": "Polygon",
+        "coordinates": [
+            [
+                [-80.724878, 35.265454],
+                [-80.722646, 35.260338]
+            ]
+        ]
+    }
+}
+
+>>> MyFeatureModel(**data)
+>>> type='Feature' geometry=PolygonModel(type='Polygon', coordinates=[[Coordinates(lon=-80.724878, lat=35.265454), Coordinates(lon=-80.722646, lat=35.260338)]]) properties=MyPropertiesModel(name='foo name')
+```
+
+Point
+-----
+
+Simple example data:
+
+```
+from pydantic_geojson import PointModel
+
+data = {
+    "type": "Point",
+    "coordinates": [-105.01621, 39.57422]
+}
+
+>>> PointModel(**data)
+>>> type='Point' coordinates=Coordinates(lon=-105.01621, lat=39.57422)
+```
+
+MultiPoint
+----------
+
+Simple example data:
+
+```
+from pydantic_geojson import MultiPointModel
+
+data = {
+    "type": "MultiPoint",
+    "coordinates": [
+        [-105.01621, 39.57422],
+        [-80.666513, 35.053994]
+    ]
+}
+
+>>> PointModel(**data)
+>>> type='MultiPoint' coordinates=[Coordinates(lon=-105.01621, lat=39.57422), Coordinates(lon=-80.666513, lat=35.053994)]
+```
+
+LineString
+----------
+
+Simple example data:
+
+```
+from pydantic_geojson import LineStringModel
+
+data = {
+    "type": "LineString",
+    "coordinates": [
+        [-99.113159, 38.869651],
+        [-99.0802, 38.85682],
+        [-98.822021, 38.85682],
+        [-98.448486, 38.848264]
+    ]
 }
 
+>>> LineStringModel(**data)
+>>> type='LineString' coordinates=[Coordinates(lon=-99.113159, lat=38.869651), Coordinates(lon=-99.0802, lat=38.85682), Coordinates(lon=-98.822021, lat=38.85682), Coordinates(lon=-98.448486, lat=38.848264)]
+```
+
+MultiLineString
+---------------
+
+Simple example data:
+
+```
+from pydantic_geojson import MultiLineStringModel
+
+data = {
+    "type": "MultiLineString",
+    "coordinates": [
+        [
+            [-105.019898, 39.574997],
+            [-105.019598, 39.574898],
+            [-105.019061, 39.574782]
+        ],
+        [
+            [-105.017173, 39.574402],
+            [-105.01698, 39.574385],
+            [-105.016636, 39.574385],
+            [-105.016508, 39.574402],
+            [-105.01595, 39.57427]
+        ],
+        [
+            [-105.014276, 39.573972],
+            [-105.014126, 39.574038],
+            [-105.013825, 39.57417],
+            [-105.01331, 39.574452]
+        ]
+    ]
+}
+
+>>> MultiLineStringModel(**data)
+>>> type='MultiLineString' coordinates=[[Coordinates(lon=-105.019898, lat=39.574997), Coordinates(lon=-105.019598, lat=39.574898), Coordinates(lon=-105.019061, lat=39.574782)], [Coordinates(lon=-105.017173, lat=39.574402), Coordinates(lon=-105.01698, lat=39.574385), Coordinates(lon=-105.016636, lat=39.574385), Coordinates(lon=-105.016508, lat=39.574402), Coordinates(lon=-105.01595, lat=39.57427)], [Coordinates(lon=-105.014276, lat=39.573972), Coordinates(lon=-105.014126, lat=39.574038), Coordinates(lon=-105.013825, lat=39.57417), Coordinates(lon=-105.01331, lat=39.574452)]]
+```
+
+Polygon
+-------
+
+Simple example data:
+
+```
+from pydantic_geojson import PolygonModel
+
+data = {
+    "type": "Polygon",
+    "coordinates": [
+        [
+            [100, 0],
+            [101, 0],
+            [101, 1],
+            [100, 1],
+            [100, 0]
+        ]
+    ]
+}
+
+>>> PolygonModel(**data)
+>>> type='Polygon' coordinates=[[Coordinates(lon=100.0, lat=0.0), Coordinates(lon=101.0, lat=0.0), Coordinates(lon=101.0, lat=1.0), Coordinates(lon=100.0, lat=1.0), Coordinates(lon=100.0, lat=0.0)]]
+```
+
+MultiPolygon
+------------
+
+Simple example data:
+
+```
+from pydantic_geojson import MultiPolygonModel
+
+data = {
+    "type": "MultiPolygon",
+    "coordinates": [
+        [
+            [
+                [107, 7],
+                [108, 7],
+                [108, 8],
+                [107, 8],
+                [107, 7]
+            ]
+        ],
+        [
+            [
+                [100, 0],
+                [101, 0],
+                [101, 1],
+                [100, 1],
+                [100, 0]
+            ]
+        ]
+    ]
+}
+
+>>> MultiPolygonModel(**data)
+>>> type='MultiPolygon' coordinates=[[[Coordinates(lon=107.0, lat=7.0), Coordinates(lon=108.0, lat=7.0), Coordinates(lon=108.0, lat=8.0), Coordinates(lon=107.0, lat=8.0), Coordinates(lon=107.0, lat=7.0)]], [[Coordinates(lon=100.0, lat=0.0), Coordinates(lon=101.0, lat=0.0), Coordinates(lon=101.0, lat=1.0), Coordinates(lon=100.0, lat=1.0), Coordinates(lon=100.0, lat=0.0)]]]
+```
+
+GeometryCollection
+------------------
+
+Simple example data:
+
+```
+from pydantic_geojson import GeometryCollectionModel
+
+data = {
+    "type": "GeometryCollection",
+    "geometries": [
+        {
+            "type": "Point",
+            "coordinates": [-80.660805, 35.049392]
+        },
+        {
+            "type": "Polygon",
+            "coordinates": [
+                [
+                    [-80.664582, 35.044965],
+                    [-80.663874, 35.04428],
+                    [-80.662586, 35.04558],
+                    [-80.663444, 35.046036],
+                    [-80.664582, 35.044965]
+                ]
+            ]
+        },
+        {
+            "type": "LineString",
+            "coordinates": [
+                [-80.662372, 35.059509],
+                [-80.662693, 35.059263],
+                [-80.662844, 35.05893]
+            ]
+        }
+    ]
+}
+
+>>> GeometryCollectionModel(**data)
+>>> type='GeometryCollection' geometries=[PointModel(type='Point', coordinates=Coordinates(lon=-80.660805, lat=35.049392)), PolygonModel(type='Polygon', coordinates=[[Coordinates(lon=-80.664582, lat=35.044965), Coordinates(lon=-80.663874, lat=35.04428), Coordinates(lon=-80.662586, lat=35.04558), Coordinates(lon=-80.663444, lat=35.046036), Coordinates(lon=-80.664582, lat=35.044965)]]), LineStringModel(type='LineString', coordinates=[Coordinates(lon=-80.662372, lat=35.059509), Coordinates(lon=-80.662693, lat=35.059263), Coordinates(lon=-80.662844, lat=35.05893)])]
+```
+
+Feature
+-------
+
+Simple example data:
+
+```
+from pydantic_geojson import FeatureModel
+
+data = {
+    "type": "Feature",
+    "geometry": {
+        "type": "Polygon",
+        "coordinates": [
+            [
+                [-80.724878, 35.265454],
+                [-80.722646, 35.260338],
+                [-80.720329, 35.260618],
+                [-80.71681, 35.255361],
+                [-80.704793, 35.268397],
+                [-82.715179, 35.267696],
+                [-80.721359, 35.267276],
+                [-80.724878, 35.265454]
+            ]
+        ]
+    }
+}
+
+>>> FeatureModel(**data)
+>>> type='Feature' geometry=PolygonModel(type='Polygon', coordinates=[[Coordinates(lon=-80.724878, lat=35.265454), Coordinates(lon=-80.722646, lat=35.260338), Coordinates(lon=-80.720329, lat=35.260618), Coordinates(lon=-80.71681, lat=35.255361), Coordinates(lon=-80.704793, lat=35.268397), Coordinates(lon=-82.715179, lat=35.267696), Coordinates(lon=-80.721359, lat=35.267276), Coordinates(lon=-80.724878, lat=35.265454)]])
+
+```
+
+FeatureCollection
+-----------------
+
+Simple example data:
+
+```
+from pydantic_geojson import FeatureCollectionModel
+
+data = {
+    "type": "FeatureCollection",
+    "features": [
+        {
+            "type": "Feature",
+            "geometry": {
+                "type": "Point",
+                "coordinates": [-80.870885, 35.215151]
+            }
+        },
+        {
+            "type": "Feature",
+            "geometry": {
+                "type": "Polygon",
+                "coordinates": [
+                    [
+                        [-80.724878, 35.265454],
+                        [-80.722646, 35.260338],
+                        [-80.720329, 35.260618],
+                        [-80.704793, 35.268397],
+                        [-80.724878, 35.265454]
+                    ]
+                ]
+            }
+        }
+    ]
+}
+
+>>> FeatureCollectionModel(**data)
+>>> type='FeatureCollection' features=[FeatureModel(type='Feature', geometry=PointModel(type='Point', coordinates=Coordinates(lon=-80.870885, lat=35.215151))), FeatureModel(type='Feature', geometry=PolygonModel(type='Polygon', coordinates=[[Coordinates(lon=-80.724878, lat=35.265454), Coordinates(lon=-80.722646, lat=35.260338), Coordinates(lon=-80.720329, lat=35.260618), Coordinates(lon=-80.704793, lat=35.268397), Coordinates(lon=-80.724878, lat=35.265454)]]))]
+
+```
 
-setup(**setup_kwargs)
```

