# Comparing `tmp/plateauutils-0.0.1.tar.gz` & `tmp/plateauutils-0.0.2.tar.gz`

## Comparing `plateauutils-0.0.1.tar` & `plateauutils-0.0.2.tar`

### file list

```diff
@@ -1,34 +1,41 @@
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 plateauutils-0.0.1/dev-requirements.txt
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 plateauutils-0.0.1/requirements.txt
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 plateauutils-0.0.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 plateauutils-0.0.1/doc/Makefile
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 plateauutils-0.0.1/doc/conf.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 plateauutils-0.0.1/doc/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 plateauutils-0.0.1/doc/make.bat
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 plateauutils-0.0.1/doc/modules.rst
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 plateauutils-0.0.1/doc/plateauutils.mesh_geocorder.rst
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 plateauutils-0.0.1/doc/plateauutils.rst
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 plateauutils-0.0.1/doc/plateauutils.tile_list.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.1/plateauutils/__init__.py
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 plateauutils-0.0.1/plateauutils/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.1/plateauutils/abc/__init__.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 plateauutils-0.0.1/plateauutils/abc/polygon_to_list.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.1/plateauutils/mesh_geocorder/__init__.py
--rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 plateauutils-0.0.1/plateauutils/mesh_geocorder/geo_to_mesh.py
--rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 plateauutils-0.0.1/plateauutils/mesh_geocorder/polygon_to_meshcode_list.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.1/plateauutils/mesh_geocorder/tests/__init__.py
--rw-r--r--   0        0        0     5626 2020-02-02 00:00:00.000000 plateauutils-0.0.1/plateauutils/mesh_geocorder/tests/test_geo_to_mesh.py
--rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 plateauutils-0.0.1/plateauutils/mesh_geocorder/tests/test_polygon_to_meshcode_list.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.1/plateauutils/tests/__init__.py
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 plateauutils-0.0.1/plateauutils/tests/test_cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.1/plateauutils/tile_list/__init__.py
--rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 plateauutils-0.0.1/plateauutils/tile_list/geo_to_tile.py
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 plateauutils-0.0.1/plateauutils/tile_list/polygon_to_tile_list.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.1/plateauutils/tile_list/tests/__init__.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 plateauutils-0.0.1/plateauutils/tile_list/tests/test_geo_to_tile.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 plateauutils-0.0.1/plateauutils/tile_list/tests/test_polygon_to_tile_list.py
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 plateauutils-0.0.1/.gitignore
--rw-r--r--   0        0        0    11342 2020-02-02 00:00:00.000000 plateauutils-0.0.1/LICENSE
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 plateauutils-0.0.1/README.rst
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 plateauutils-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    14017 2020-02-02 00:00:00.000000 plateauutils-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 plateauutils-0.0.2/dev-requirements.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 plateauutils-0.0.2/requirements.txt
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 plateauutils-0.0.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 plateauutils-0.0.2/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 plateauutils-0.0.2/doc/Makefile
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 plateauutils-0.0.2/doc/conf.py
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 plateauutils-0.0.2/doc/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 plateauutils-0.0.2/doc/make.bat
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 plateauutils-0.0.2/doc/modules.rst
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 plateauutils-0.0.2/doc/plateauutils.mesh_geocorder.rst
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 plateauutils-0.0.2/doc/plateauutils.parser.rst
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 plateauutils-0.0.2/doc/plateauutils.rst
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 plateauutils-0.0.2/doc/plateauutils.tile_list.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/__init__.py
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/abc/__init__.py
+-rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/abc/plateau_parser.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/abc/polygon_to_list.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/mesh_geocorder/__init__.py
+-rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/mesh_geocorder/geo_to_mesh.py
+-rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/mesh_geocorder/polygon_to_meshcode_list.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/mesh_geocorder/tests/__init__.py
+-rw-r--r--   0        0        0     5626 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/mesh_geocorder/tests/test_geo_to_mesh.py
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/mesh_geocorder/tests/test_polygon_to_meshcode_list.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/parser/__init__.py
+-rw-r--r--   0        0        0     7573 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/parser/city_gml_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/parser/tests/__init__.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/parser/tests/test_city_gml_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/tests/__init__.py
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/tests/test_cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/tile_list/__init__.py
+-rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/tile_list/geo_to_tile.py
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/tile_list/polygon_to_tile_list.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/tile_list/tests/__init__.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/tile_list/tests/test_geo_to_tile.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 plateauutils-0.0.2/plateauutils/tile_list/tests/test_polygon_to_tile_list.py
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 plateauutils-0.0.2/.gitignore
+-rw-r--r--   0        0        0    11342 2020-02-02 00:00:00.000000 plateauutils-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 plateauutils-0.0.2/README.rst
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 plateauutils-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    15290 2020-02-02 00:00:00.000000 plateauutils-0.0.2/PKG-INFO
```

### Comparing `plateauutils-0.0.1/dev-requirements.txt` & `plateauutils-0.0.2/dev-requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -43,12 +43,13 @@
 sphinxcontrib-applehelp==1.0.4
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
 tomli==2.0.1
+tqdm==4.65.0
 twine==4.0.2
 typing_extensions==4.6.3
 urllib3==2.0.2
 webencodings==0.5.1
 zipp==3.15.0
```

### Comparing `plateauutils-0.0.1/.github/workflows/ci.yml` & `plateauutils-0.0.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.1/doc/Makefile` & `plateauutils-0.0.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.1/doc/conf.py` & `plateauutils-0.0.2/doc/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 sys.path.insert(0, os.path.abspath(".."))
 import plateauutils
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = "plateauutils"
-copyright = "2023, Taro Matsuzawa"
-author = "Taro Matsuzawa"
+copyright = "2023, Eukarya Inc."
+author = "Eukarya Inc."
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     "sphinx.ext.autodoc",
 ]
```

### Comparing `plateauutils-0.0.1/doc/make.bat` & `plateauutils-0.0.2/doc/make.bat`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.1/doc/plateauutils.mesh_geocorder.rst` & `plateauutils-0.0.2/doc/plateauutils.mesh_geocorder.rst`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.1/doc/plateauutils.tile_list.rst` & `plateauutils-0.0.2/doc/plateauutils.tile_list.rst`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.1/plateauutils/cli.py` & `plateauutils-0.0.2/plateauutils/cli.py`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.1/plateauutils/abc/polygon_to_list.py` & `plateauutils-0.0.2/plateauutils/abc/polygon_to_list.py`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.1/plateauutils/mesh_geocorder/geo_to_mesh.py` & `plateauutils-0.0.2/plateauutils/mesh_geocorder/geo_to_mesh.py`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.1/plateauutils/mesh_geocorder/polygon_to_meshcode_list.py` & `plateauutils-0.0.2/plateauutils/mesh_geocorder/polygon_to_meshcode_list.py`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.1/plateauutils/mesh_geocorder/tests/test_geo_to_mesh.py` & `plateauutils-0.0.2/plateauutils/mesh_geocorder/tests/test_geo_to_mesh.py`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.1/plateauutils/mesh_geocorder/tests/test_polygon_to_meshcode_list.py` & `plateauutils-0.0.2/plateauutils/mesh_geocorder/tests/test_polygon_to_meshcode_list.py`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.1/plateauutils/tests/test_cli.py` & `plateauutils-0.0.2/plateauutils/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.1/plateauutils/tile_list/geo_to_tile.py` & `plateauutils-0.0.2/plateauutils/tile_list/geo_to_tile.py`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.1/plateauutils/tile_list/polygon_to_tile_list.py` & `plateauutils-0.0.2/plateauutils/tile_list/polygon_to_tile_list.py`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.1/plateauutils/tile_list/tests/test_geo_to_tile.py` & `plateauutils-0.0.2/plateauutils/tile_list/tests/test_geo_to_tile.py`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.1/plateauutils/tile_list/tests/test_polygon_to_tile_list.py` & `plateauutils-0.0.2/plateauutils/tile_list/tests/test_polygon_to_tile_list.py`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.1/.gitignore` & `plateauutils-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.1/LICENSE` & `plateauutils-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `plateauutils-0.0.1/pyproject.toml` & `plateauutils-0.0.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -7,21 +7,29 @@
 description = "A collection of utilities for the Plateau project"
 readme = "README.rst"
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: 3",
 ]
-version = "0.0.1"
+version = "0.0.2"
 dependencies = [
     "click",
-    "shapely"
+    "numpy",
+    "requests",
+    "shapely",
+    "tqdm",
 ]
 authors = [
-    {name = "Taro Matsuzawa", email = "btm@tech.email.ne.jp"},
+    {name = "Eukarya Inc."},
 ]
 requires-python = ">=3.9"
 repository = "https://github.com/eukarya-inc/plateauutils"
 keywords = ['plateau']
 
 [tool.hatch.build]
-exclude = ["tests/*"]
+exclude = ["tests/*"]
+
+[project.urls]
+"Homepage" = "https://eukarya-inc.github.io/plateauutils/"
+"Bug Reports" = "https://github.com/eukarya-inc/plateauutils/issues"
+"Source" = "https://github.com/eukarya-inc/plateauutils"
```

### Comparing `plateauutils-0.0.1/PKG-INFO` & `plateauutils-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 Metadata-Version: 2.1
 Name: plateauutils
-Version: 0.0.1
+Version: 0.0.2
 Summary: A collection of utilities for the Plateau project
-Author-email: Taro Matsuzawa <btm@tech.email.ne.jp>
+Project-URL: Homepage, https://eukarya-inc.github.io/plateauutils/
+Project-URL: Bug Reports, https://github.com/eukarya-inc/plateauutils/issues
+Project-URL: Source, https://github.com/eukarya-inc/plateauutils
+Author: Eukarya Inc.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
            1. Definitions.
@@ -206,29 +209,40 @@
            limitations under the License.
 License-File: LICENSE
 Keywords: plateau
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Requires-Dist: click
+Requires-Dist: numpy
+Requires-Dist: requests
 Requires-Dist: shapely
+Requires-Dist: tqdm
 Description-Content-Type: text/x-rst
 
 Plateau Utils
 =============
 
 This is a collection of utilities for the `Plateau <https://www.mlit.go.jp/plateau/>`_ project.
 
 .. code:: python
 
+    >>> from shapely.geometry import Point
     >>> from plateauutils.mesh_geocorder.geo_to_mesh import point_to_meshcode
     >>> point = Point(139.71475, 35.70078)
     >>> mesh_code = point_to_meshcode(point, "2/1")
     >>> mesh_code
     '533945471'
+    >>> from shapely import from_wkt
+    >>> from plateauutils.parser.city_gml_parser import CityGMLParser
+    >>> target_polygon = from_wkt("POLYGON ((130.41249721501615 33.224722548534864, 130.41249721501615 33.22506264293093, 130.41621606802997 33.22506264293093, 130.41621606802997 33.224722548534864, 130.41249721501615 33.224722548534864))")
+    >>> parser = CityGMLParser(target_polygon)
+    >>> result = parser.download_and_parse("https://assets.cms.plateau.reearth.io/assets/d6/70821e-7f58-4f69-bc34-341875704e78/40203_kurume-shi_2020_citygml_3_op.zip", "/tmp")
+    >>> result
+    [{'gid': 'bldg_383f1804-aa34-4634-949f-f769e09fa92d', 'center': [130.41263587199947, 33.22489181671553], 'min_height': 3.805999994277954, 'measured_height': 9.3, 'building_structure_type': '610'}, {'gid': 'bldg_877dea60-35d0-4fd9-8b02-852e39c75d81', 'center': [130.41619367090038, 33.22492719812357], 'min_height': 4.454999923706055, 'measured_height': 3.0, 'building_structure_type': '610'},...]
 
 How to develop
 --------------
 
 .. code:: bash
 
     python3.9 -m venv venv
```

