# Comparing `tmp/abm_shape_collection-0.6.0.tar.gz` & `tmp/abm_shape_collection-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abm_shape_collection-0.6.0.tar", max compression
+gzip compressed data, was "abm_shape_collection-0.7.0.tar", max compression
```

## Comparing `abm_shape_collection-0.6.0.tar` & `abm_shape_collection-0.7.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1540 2023-06-29 20:18:32.131239 abm_shape_collection-0.6.0/LICENSE
--rw-r--r--   0        0        0     2573 2023-06-29 20:18:32.131239 abm_shape_collection-0.6.0/README.md
--rw-r--r--   0        0        0     1933 2023-06-29 20:18:32.135239 abm_shape_collection-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1307 2023-06-29 20:18:32.135239 abm_shape_collection-0.6.0/src/abm_shape_collection/__init__.py
--rw-r--r--   0        0        0       52 2023-06-29 20:18:32.135239 abm_shape_collection-0.6.0/src/abm_shape_collection/__main__.py
--rw-r--r--   0        0        0     2898 2023-06-29 20:18:32.135239 abm_shape_collection-0.6.0/src/abm_shape_collection/calculate_shape_stats.py
--rw-r--r--   0        0        0     2765 2023-06-29 20:18:32.135239 abm_shape_collection-0.6.0/src/abm_shape_collection/calculate_size_stats.py
--rw-r--r--   0        0        0     6161 2023-06-29 20:18:32.135239 abm_shape_collection-0.6.0/src/abm_shape_collection/compile_shape_modes.py
--rw-r--r--   0        0        0      383 2023-06-29 20:18:32.135239 abm_shape_collection-0.6.0/src/abm_shape_collection/construct_mesh_from_array.py
--rw-r--r--   0        0        0     1016 2023-06-29 20:18:32.135239 abm_shape_collection-0.6.0/src/abm_shape_collection/construct_mesh_from_coeffs.py
--rw-r--r--   0        0        0      576 2023-06-29 20:18:32.135239 abm_shape_collection-0.6.0/src/abm_shape_collection/construct_mesh_from_points.py
--rw-r--r--   0        0        0     2506 2023-06-29 20:18:32.135239 abm_shape_collection-0.6.0/src/abm_shape_collection/extract_shape_modes.py
--rw-r--r--   0        0        0      508 2023-06-29 20:18:32.135239 abm_shape_collection-0.6.0/src/abm_shape_collection/fit_pca_model.py
--rw-r--r--   0        0        0      430 2023-06-29 20:18:32.135239 abm_shape_collection-0.6.0/src/abm_shape_collection/get_shape_coefficients.py
--rw-r--r--   0        0        0      352 2023-06-29 20:18:32.135239 abm_shape_collection-0.6.0/src/abm_shape_collection/get_shape_properties.py
--rw-r--r--   0        0        0      942 2023-06-29 20:18:32.135239 abm_shape_collection-0.6.0/src/abm_shape_collection/make_voxels_array.py
--rw-r--r--   0        0        0     3648 2023-06-29 20:18:32.135239 abm_shape_collection-0.6.0/src/abm_shape_collection/merge_shape_modes.py
--rw-r--r--   0        0        0        0 2023-06-29 20:18:32.135239 abm_shape_collection-0.6.0/src/abm_shape_collection/py.typed
--rw-r--r--   0        0        0     3325 1970-01-01 00:00:00.000000 abm_shape_collection-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1540 2023-07-14 21:32:00.106938 abm_shape_collection-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2573 2023-07-14 21:32:00.106938 abm_shape_collection-0.7.0/README.md
+-rw-r--r--   0        0        0     1933 2023-07-14 21:32:00.106938 abm_shape_collection-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1347 2023-07-14 21:32:00.106938 abm_shape_collection-0.7.0/src/abm_shape_collection/__init__.py
+-rw-r--r--   0        0        0       52 2023-07-14 21:32:00.106938 abm_shape_collection-0.7.0/src/abm_shape_collection/__main__.py
+-rw-r--r--   0        0        0     2898 2023-07-14 21:32:00.106938 abm_shape_collection-0.7.0/src/abm_shape_collection/calculate_shape_stats.py
+-rw-r--r--   0        0        0     2765 2023-07-14 21:32:00.106938 abm_shape_collection-0.7.0/src/abm_shape_collection/calculate_size_stats.py
+-rw-r--r--   0        0        0      777 2023-07-14 21:32:00.106938 abm_shape_collection-0.7.0/src/abm_shape_collection/construct_mesh_from_array.py
+-rw-r--r--   0        0        0     1016 2023-07-14 21:32:00.110938 abm_shape_collection-0.7.0/src/abm_shape_collection/construct_mesh_from_coeffs.py
+-rw-r--r--   0        0        0      576 2023-07-14 21:32:00.110938 abm_shape_collection-0.7.0/src/abm_shape_collection/construct_mesh_from_points.py
+-rw-r--r--   0        0        0     2384 2023-07-14 21:32:00.110938 abm_shape_collection-0.7.0/src/abm_shape_collection/extract_mesh_projections.py
+-rw-r--r--   0        0        0      582 2023-07-14 21:32:00.110938 abm_shape_collection-0.7.0/src/abm_shape_collection/extract_mesh_wireframe.py
+-rw-r--r--   0        0        0     3058 2023-07-14 21:32:00.110938 abm_shape_collection-0.7.0/src/abm_shape_collection/extract_shape_modes.py
+-rw-r--r--   0        0        0      508 2023-07-14 21:32:00.110938 abm_shape_collection-0.7.0/src/abm_shape_collection/fit_pca_model.py
+-rw-r--r--   0        0        0      611 2023-07-14 21:32:00.110938 abm_shape_collection-0.7.0/src/abm_shape_collection/get_shape_coefficients.py
+-rw-r--r--   0        0        0      352 2023-07-14 21:32:00.110938 abm_shape_collection-0.7.0/src/abm_shape_collection/get_shape_properties.py
+-rw-r--r--   0        0        0     1228 2023-07-14 21:32:00.110938 abm_shape_collection-0.7.0/src/abm_shape_collection/make_voxels_array.py
+-rw-r--r--   0        0        0        0 2023-07-14 21:32:00.110938 abm_shape_collection-0.7.0/src/abm_shape_collection/py.typed
+-rw-r--r--   0        0        0     3325 1970-01-01 00:00:00.000000 abm_shape_collection-0.7.0/PKG-INFO
```

### Comparing `abm_shape_collection-0.6.0/LICENSE` & `abm_shape_collection-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `abm_shape_collection-0.6.0/README.md` & `abm_shape_collection-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `abm_shape_collection-0.6.0/pyproject.toml` & `abm_shape_collection-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "abm-shape-collection"
-version = "0.6.0"
+version = "0.7.0"
 description = "Collection of tasks for analyzing cell shapes."
 authors = [
     "Jessica S. Yu <jesyu@uw.edu>"
 ]
 license = "BSD-3-Clause"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 prefect = "^2.8.2"
 numpy = "^1.24.2"
 pandas = "^1.5.3"
-aicsshparam = "^0.1.1"
+aicsshparam = "^0.1.6"
 vtk = "^9.2.5"
 trimesh = "^3.18.3"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 isort = "^5.12.0"
 mypy = "^1.3.0"
```

### Comparing `abm_shape_collection-0.6.0/src/abm_shape_collection/calculate_shape_stats.py` & `abm_shape_collection-0.7.0/src/abm_shape_collection/calculate_shape_stats.py`

 * *Files identical despite different names*

### Comparing `abm_shape_collection-0.6.0/src/abm_shape_collection/calculate_size_stats.py` & `abm_shape_collection-0.7.0/src/abm_shape_collection/calculate_size_stats.py`

 * *Files identical despite different names*

### Comparing `abm_shape_collection-0.6.0/src/abm_shape_collection/construct_mesh_from_coeffs.py` & `abm_shape_collection-0.7.0/src/abm_shape_collection/construct_mesh_from_coeffs.py`

 * *Files identical despite different names*

### Comparing `abm_shape_collection-0.6.0/src/abm_shape_collection/construct_mesh_from_points.py` & `abm_shape_collection-0.7.0/src/abm_shape_collection/construct_mesh_from_points.py`

 * *Files identical despite different names*

### Comparing `abm_shape_collection-0.6.0/src/abm_shape_collection/extract_shape_modes.py` & `abm_shape_collection-0.7.0/src/abm_shape_collection/extract_shape_modes.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,77 +1,89 @@
-import tempfile
-
 import numpy as np
 import pandas as pd
-import trimesh
 from sklearn.decomposition import PCA
-from vtk import vtkPLYWriter, vtkPolyData
 
 from abm_shape_collection.construct_mesh_from_points import construct_mesh_from_points
+from abm_shape_collection.extract_mesh_projections import extract_mesh_projections
 
 
 def extract_shape_modes(
     pca: PCA, data: pd.DataFrame, components: int, regions: list[str], order: int, delta: float
 ) -> dict:
-    features = data.filter(like="shcoeffs").columns.values
-    data_transform = pca.transform(data[features].values)
-    means = data_transform.mean(axis=0)
-    stds = data_transform.std(axis=0, ddof=1)
+    # Transform data into shape mode space.
+    features = data.filter(like="shcoeffs").columns
+    transform = pca.transform(data[features].values)
+
+    # Calculate transformed means and standard deviations.
+    means = transform.mean(axis=0)
+    stds = transform.std(axis=0, ddof=1)
+
+    # Create bins.
+    map_points = np.arange(-2, 2.5, delta)
+    bin_edges = [-np.inf] + [point + delta / 2 for point in map_points[:-1]] + [np.inf]
+    transform_binned = np.digitize(transform / stds, bin_edges)
+
+    # Calculate offsets.
+    offsets = {
+        region: calculate_region_offsets(data, region) for region in regions if region != "DEFAULT"
+    }
 
-    shape_svgs = {}
+    # Initialize output dictionary.
+    shape_modes: dict[str, list] = {}
 
-    for component in range(components):
-        point_vector = np.zeros((components))
-        component_shape_modes = {}
+    for region in regions:
+        region_shape_modes = []
 
-        for point in np.arange(-2, 2.5, delta):
-            point_vector[component] = point
-            vector = means + np.multiply(stds, point_vector)
-            point_shape_modes = {}
+        suffix = f".{region}" if region != "DEFAULT" else ""
+        offsets = calculate_region_offsets(data, region)
 
-            for region in regions:
-                shape_mode_slices = extract_shape_mode_slices(pca, vector, features, order, region)
-                point_shape_modes[region] = shape_mode_slices
+        for component in range(components):
+            point_vector = np.zeros((components))
 
-            component_shape_modes[point] = point_shape_modes
+            for point in map_points:
+                point_bin = np.digitize(point, bin_edges)
+                point_vector[component] = point
 
-        shape_svgs[component + 1] = component_shape_modes
+                vector = means + np.multiply(stds, point_vector)
+                indices = transform_binned[:, component] == point_bin
 
-    return shape_svgs
+                mesh = construct_mesh_from_points(pca, vector, features, order, suffix=suffix)
 
+                if region == "DEFAULT":
+                    offset = None
+                else:
+                    offset = (
+                        offsets["x"][indices].mean(),
+                        offsets["y"][indices].mean(),
+                        offsets["z"][indices].mean(),
+                    )
 
-def extract_shape_mode_slices(
-    pca: PCA, vector: np.ndarray, feature_names: list[str], order: int, region: str
-) -> dict:
-    prefix = ""
-    suffix = f".{region}" if region != "DEFAULT" else ""
-    mesh = construct_mesh_from_points(pca, vector, feature_names, order, prefix, suffix)
-    mesh = convert_vtk_to_trimesh(mesh)
-    slices = get_mesh_slices(mesh)
-    return slices
-
-
-def convert_vtk_to_trimesh(mesh: vtkPolyData) -> trimesh.Trimesh:
-    with tempfile.NamedTemporaryFile() as temp:
-        writer = vtkPLYWriter()
-        writer.SetInputData(mesh)
-        writer.SetFileTypeToASCII()
-        writer.SetFileName(f"{temp.name}.ply")
-        _ = writer.Write()
-        mesh = trimesh.load(f"{temp.name}.ply")
+                region_shape_modes.append(
+                    {
+                        "mode": component + 1,
+                        "point": point,
+                        "projections": extract_mesh_projections(mesh, extents=False, offset=offset),
+                    }
+                )
 
-    return mesh
+        shape_modes[region] = region_shape_modes
 
+    return shape_modes
 
-def get_mesh_slices(mesh: trimesh.Trimesh) -> dict:
-    return {
-        "side_1": get_mesh_slice(mesh, (0, 1, 0)),
-        "side_2": get_mesh_slice(mesh, (1, 0, 0)),
-        "top": get_mesh_slice(mesh, (0, 0, 1)),
-    }
 
+def calculate_region_offsets(data: pd.DataFrame, region: str) -> dict:
+    if region == "DEFAULT":
+        return {}
 
-def get_mesh_slice(mesh: trimesh.Trimesh, normal: tuple[int, int, int]) -> str:
-    """Get svg slice of mesh along plane for given normal."""
-    mesh_slice = mesh.section_multiplane(mesh.centroid, normal, [0])
-    svg = trimesh.path.exchange.svg_io.export_svg(mesh_slice[0])
-    return svg
+    x_deltas = data[f"CENTER_X.{region}"].values - data["CENTER_X"].values
+    y_deltas = data[f"CENTER_Y.{region}"].values - data["CENTER_Y"].values
+    z_deltas = data[f"CENTER_Z.{region}"].values - data["CENTER_Z"].values
+    angles = data["angle"].values * np.pi / 180.0
+
+    sin_angles = np.sin(angles)
+    cos_angles = np.cos(angles)
+
+    return {
+        "x": x_deltas * cos_angles - y_deltas * sin_angles,
+        "y": x_deltas * sin_angles + y_deltas * cos_angles,
+        "z": z_deltas,
+    }
```

### Comparing `abm_shape_collection-0.6.0/PKG-INFO` & `abm_shape_collection-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: abm-shape-collection
-Version: 0.6.0
+Version: 0.7.0
 Summary: Collection of tasks for analyzing cell shapes.
 License: BSD-3-Clause
 Author: Jessica S. Yu
 Author-email: jesyu@uw.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aicsshparam (>=0.1.1,<0.2.0)
+Requires-Dist: aicsshparam (>=0.1.6,<0.2.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: prefect (>=2.8.2,<3.0.0)
 Requires-Dist: trimesh (>=3.18.3,<4.0.0)
 Requires-Dist: vtk (>=9.2.5,<10.0.0)
 Description-Content-Type: text/markdown
```

