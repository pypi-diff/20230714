# Comparing `tmp/arcade_collection-0.8.1.tar.gz` & `tmp/arcade_collection-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcade_collection-0.8.1.tar", max compression
+gzip compressed data, was "arcade_collection-0.9.0.tar", max compression
```

## Comparing `arcade_collection-0.8.1.tar` & `arcade_collection-0.9.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0     1519 2023-06-29 21:02:53.041198 arcade_collection-0.8.1/LICENSE
--rw-r--r--   0        0        0     2502 2023-06-29 21:02:53.041198 arcade_collection-0.8.1/README.md
--rw-r--r--   0        0        0     1870 2023-06-29 21:02:53.041198 arcade_collection-0.8.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-29 21:02:53.041198 arcade_collection-0.8.1/src/arcade_collection/__init__.py
--rw-r--r--   0        0        0       52 2023-06-29 21:02:53.041198 arcade_collection-0.8.1/src/arcade_collection/__main__.py
--rw-r--r--   0        0        0      592 2023-06-29 21:02:53.041198 arcade_collection-0.8.1/src/arcade_collection/input/__init__.py
--rw-r--r--   0        0        0     6982 2023-06-29 21:02:53.041198 arcade_collection-0.8.1/src/arcade_collection/input/convert_to_cells_file.py
--rw-r--r--   0        0        0     2313 2023-06-29 21:02:53.045198 arcade_collection-0.8.1/src/arcade_collection/input/convert_to_locations_file.py
--rw-r--r--   0        0        0     2607 2023-06-29 21:02:53.045198 arcade_collection-0.8.1/src/arcade_collection/input/generate_setup_file.py
--rw-r--r--   0        0        0     2375 2023-06-29 21:02:53.045198 arcade_collection-0.8.1/src/arcade_collection/input/group_template_conditions.py
--rw-r--r--   0        0        0     2517 2023-06-29 21:02:53.045198 arcade_collection-0.8.1/src/arcade_collection/input/merge_region_samples.py
--rw-r--r--   0        0        0      916 2023-06-29 21:02:53.045198 arcade_collection-0.8.1/src/arcade_collection/output/__init__.py
--rw-r--r--   0        0        0     1015 2023-06-29 21:02:53.045198 arcade_collection-0.8.1/src/arcade_collection/output/convert_model_units.py
--rw-r--r--   0        0        0     2777 2023-06-29 21:02:53.045198 arcade_collection-0.8.1/src/arcade_collection/output/convert_to_images.py
--rw-r--r--   0        0        0     2682 2023-06-29 21:02:53.045198 arcade_collection-0.8.1/src/arcade_collection/output/convert_to_meshes.py
--rw-r--r--   0        0        0     3709 2023-06-29 21:02:53.045198 arcade_collection-0.8.1/src/arcade_collection/output/convert_to_simularium.py
--rw-r--r--   0        0        0      301 2023-06-29 21:02:53.045198 arcade_collection-0.8.1/src/arcade_collection/output/extract_tick_json.py
--rw-r--r--   0        0        0      308 2023-06-29 21:02:53.045198 arcade_collection-0.8.1/src/arcade_collection/output/get_location_voxels.py
--rw-r--r--   0        0        0      260 2023-06-29 21:02:53.045198 arcade_collection-0.8.1/src/arcade_collection/output/merge_parsed_results.py
--rw-r--r--   0        0        0     1457 2023-06-29 21:02:53.045198 arcade_collection-0.8.1/src/arcade_collection/output/parse_cells_file.py
--rw-r--r--   0        0        0     2103 2023-06-29 21:02:53.045198 arcade_collection-0.8.1/src/arcade_collection/output/parse_locations_file.py
--rw-r--r--   0        0        0        0 2023-06-29 21:02:53.045198 arcade_collection-0.8.1/src/arcade_collection/py.typed
--rw-r--r--   0        0        0     3219 1970-01-01 00:00:00.000000 arcade_collection-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1519 2023-07-14 21:44:37.922209 arcade_collection-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2502 2023-07-14 21:44:37.926209 arcade_collection-0.9.0/README.md
+-rw-r--r--   0        0        0     1870 2023-07-14 21:44:37.926209 arcade_collection-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-14 21:44:37.926209 arcade_collection-0.9.0/src/arcade_collection/__init__.py
+-rw-r--r--   0        0        0       52 2023-07-14 21:44:37.926209 arcade_collection-0.9.0/src/arcade_collection/__main__.py
+-rw-r--r--   0        0        0      592 2023-07-14 21:44:37.926209 arcade_collection-0.9.0/src/arcade_collection/input/__init__.py
+-rw-r--r--   0        0        0     6982 2023-07-14 21:44:37.926209 arcade_collection-0.9.0/src/arcade_collection/input/convert_to_cells_file.py
+-rw-r--r--   0        0        0     2313 2023-07-14 21:44:37.926209 arcade_collection-0.9.0/src/arcade_collection/input/convert_to_locations_file.py
+-rw-r--r--   0        0        0     2607 2023-07-14 21:44:37.926209 arcade_collection-0.9.0/src/arcade_collection/input/generate_setup_file.py
+-rw-r--r--   0        0        0     2375 2023-07-14 21:44:37.926209 arcade_collection-0.9.0/src/arcade_collection/input/group_template_conditions.py
+-rw-r--r--   0        0        0     2517 2023-07-14 21:44:37.926209 arcade_collection-0.9.0/src/arcade_collection/input/merge_region_samples.py
+-rw-r--r--   0        0        0     1126 2023-07-14 21:44:37.926209 arcade_collection-0.9.0/src/arcade_collection/output/__init__.py
+-rw-r--r--   0        0        0     1015 2023-07-14 21:44:37.926209 arcade_collection-0.9.0/src/arcade_collection/output/convert_model_units.py
+-rw-r--r--   0        0        0     2142 2023-07-14 21:44:37.926209 arcade_collection-0.9.0/src/arcade_collection/output/convert_to_colorizer.py
+-rw-r--r--   0        0        0     3511 2023-07-14 21:44:37.926209 arcade_collection-0.9.0/src/arcade_collection/output/convert_to_images.py
+-rw-r--r--   0        0        0     2682 2023-07-14 21:44:37.926209 arcade_collection-0.9.0/src/arcade_collection/output/convert_to_meshes.py
+-rw-r--r--   0        0        0     7024 2023-07-14 21:44:37.926209 arcade_collection-0.9.0/src/arcade_collection/output/convert_to_simularium.py
+-rw-r--r--   0        0        0     2329 2023-07-14 21:44:37.926209 arcade_collection-0.9.0/src/arcade_collection/output/extract_feature_bins.py
+-rw-r--r--   0        0        0      301 2023-07-14 21:44:37.926209 arcade_collection-0.9.0/src/arcade_collection/output/extract_tick_json.py
+-rw-r--r--   0        0        0      308 2023-07-14 21:44:37.926209 arcade_collection-0.9.0/src/arcade_collection/output/get_location_voxels.py
+-rw-r--r--   0        0        0      260 2023-07-14 21:44:37.926209 arcade_collection-0.9.0/src/arcade_collection/output/merge_parsed_results.py
+-rw-r--r--   0        0        0     1457 2023-07-14 21:44:37.926209 arcade_collection-0.9.0/src/arcade_collection/output/parse_cells_file.py
+-rw-r--r--   0        0        0     2103 2023-07-14 21:44:37.926209 arcade_collection-0.9.0/src/arcade_collection/output/parse_locations_file.py
+-rw-r--r--   0        0        0        0 2023-07-14 21:44:37.926209 arcade_collection-0.9.0/src/arcade_collection/py.typed
+-rw-r--r--   0        0        0     3219 1970-01-01 00:00:00.000000 arcade_collection-0.9.0/PKG-INFO
```

### Comparing `arcade_collection-0.8.1/LICENSE` & `arcade_collection-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arcade_collection-0.8.1/README.md` & `arcade_collection-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `arcade_collection-0.8.1/pyproject.toml` & `arcade_collection-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arcade-collection"
-version = "0.8.1"
+version = "0.9.0"
 description = "Collection of tasks for working with ARCADE."
 authors = [
     "Jessica S. Yu <jesyu@uw.edu>"
 ]
 license = "BSD-3-Clause"
 readme = "README.md"
```

### Comparing `arcade_collection-0.8.1/src/arcade_collection/input/__init__.py` & `arcade_collection-0.9.0/src/arcade_collection/input/__init__.py`

 * *Files identical despite different names*

### Comparing `arcade_collection-0.8.1/src/arcade_collection/input/convert_to_cells_file.py` & `arcade_collection-0.9.0/src/arcade_collection/input/convert_to_cells_file.py`

 * *Files identical despite different names*

### Comparing `arcade_collection-0.8.1/src/arcade_collection/input/convert_to_locations_file.py` & `arcade_collection-0.9.0/src/arcade_collection/input/convert_to_locations_file.py`

 * *Files identical despite different names*

### Comparing `arcade_collection-0.8.1/src/arcade_collection/input/generate_setup_file.py` & `arcade_collection-0.9.0/src/arcade_collection/input/generate_setup_file.py`

 * *Files identical despite different names*

### Comparing `arcade_collection-0.8.1/src/arcade_collection/input/group_template_conditions.py` & `arcade_collection-0.9.0/src/arcade_collection/input/group_template_conditions.py`

 * *Files identical despite different names*

### Comparing `arcade_collection-0.8.1/src/arcade_collection/input/merge_region_samples.py` & `arcade_collection-0.9.0/src/arcade_collection/input/merge_region_samples.py`

 * *Files identical despite different names*

### Comparing `arcade_collection-0.8.1/src/arcade_collection/output/__init__.py` & `arcade_collection-0.9.0/src/arcade_collection/output/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from prefect import task
 
 from .convert_model_units import convert_model_units
+from .convert_to_colorizer import convert_to_colorizer
 from .convert_to_images import convert_to_images
 from .convert_to_meshes import convert_to_meshes
 from .convert_to_simularium import convert_to_simularium
+from .extract_feature_bins import extract_feature_bins
 from .extract_tick_json import extract_tick_json
 from .get_location_voxels import get_location_voxels
 from .merge_parsed_results import merge_parsed_results
 from .parse_cells_file import parse_cells_file
 from .parse_locations_file import parse_locations_file
 
 convert_model_units = task(convert_model_units)
+convert_to_colorizer = task(convert_to_colorizer)
 convert_to_images = task(convert_to_images)
 convert_to_meshes = task(convert_to_meshes)
 convert_to_simularium = task(convert_to_simularium)
+extract_feature_bins = task(extract_feature_bins)
 extract_tick_json = task(extract_tick_json)
 get_location_voxels = task(get_location_voxels)
 merge_parsed_results = task(merge_parsed_results)
 parse_cells_file = task(parse_cells_file)
 parse_locations_file = task(parse_locations_file)
```

### Comparing `arcade_collection-0.8.1/src/arcade_collection/output/convert_model_units.py` & `arcade_collection-0.9.0/src/arcade_collection/output/convert_model_units.py`

 * *Files identical despite different names*

### Comparing `arcade_collection-0.8.1/src/arcade_collection/output/convert_to_images.py` & `arcade_collection-0.9.0/src/arcade_collection/output/convert_to_images.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 def convert_to_images(
     series_key: str,
     data_tar: tarfile.TarFile,
     frame_spec: tuple[int, int, int],
     regions: list[str],
     box: tuple[int, int, int],
     chunk_size: int,
-    binary: bool,
-    separate: bool,
+    binary: bool = False,
+    separate: bool = False,
+    flatten: bool = False,
 ) -> list[tuple[int, int, np.ndarray, Optional[int]]]:
     length, width, height = box
     frames = list(np.arange(*frame_spec))
     array = np.zeros((len(frames), len(regions), height, width, length), "uint16")
 
     for index, frame in enumerate(frames):
         locations = extract_tick_json(data_tar, series_key, frame, "LOCATIONS")
@@ -36,15 +37,21 @@
                 ]
 
                 if len(voxels) == 0:
                     continue
 
                 array[index, channel][tuple(np.transpose(voxels))] = 1 if binary else location_id
 
-    if separate:
+    if separate and flatten:
+        chunks = [
+            (i, j, flatten_array_chunk(chunk), frame)
+            for index, frame in enumerate(frames)
+            for i, j, chunk in split_array_chunks(array[[index], :, :, :, :], chunk_size)
+        ]
+    elif separate:
         chunks = [
             (i, j, chunk, frame)
             for index, frame in enumerate(frames)
             for i, j, chunk in split_array_chunks(array[[index], :, :, :, :], chunk_size)
         ]
     else:
         chunks = [(i, j, chunk, None) for i, j, chunk in split_array_chunks(array, chunk_size)]
@@ -79,7 +86,19 @@
             # Extract chunk from full contents.
             chunk = np.copy(array[:, :, :, length_start:length_end, width_start:width_end])
 
             if np.sum(chunk) != 0:
                 chunks.append((i, j, chunk))
 
     return chunks
+
+
+def flatten_array_chunk(array: np.ndarray) -> np.ndarray:
+    array_flat = array[0, 0, :, :, :].max(axis=0)
+
+    array_rgba = np.zeros((*array_flat.shape, 4), dtype=np.uint8)
+    array_rgba[:, :, 0] = (array_flat & 0x000000FF) >> 0
+    array_rgba[:, :, 1] = (array_flat & 0x0000FF00) >> 8
+    array_rgba[:, :, 2] = (array_flat & 0x00FF0000) >> 16
+    array_rgba[:, :, 3] = 255  # (array_flat & 0x00FF0000) >> 24
+
+    return array_rgba
```

### Comparing `arcade_collection-0.8.1/src/arcade_collection/output/convert_to_meshes.py` & `arcade_collection-0.9.0/src/arcade_collection/output/convert_to_meshes.py`

 * *Files identical despite different names*

### Comparing `arcade_collection-0.8.1/src/arcade_collection/output/parse_cells_file.py` & `arcade_collection-0.9.0/src/arcade_collection/output/parse_cells_file.py`

 * *Files identical despite different names*

### Comparing `arcade_collection-0.8.1/src/arcade_collection/output/parse_locations_file.py` & `arcade_collection-0.9.0/src/arcade_collection/output/parse_locations_file.py`

 * *Files identical despite different names*

### Comparing `arcade_collection-0.8.1/PKG-INFO` & `arcade_collection-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcade-collection
-Version: 0.8.1
+Version: 0.9.0
 Summary: Collection of tasks for working with ARCADE.
 License: BSD-3-Clause
 Author: Jessica S. Yu
 Author-email: jesyu@uw.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

