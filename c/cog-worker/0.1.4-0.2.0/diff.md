# Comparing `tmp/cog_worker-0.1.4.tar.gz` & `tmp/cog_worker-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cog_worker-0.1.4.tar", last modified: Tue Nov 30 01:04:32 2021, max compression
+gzip compressed data, was "cog_worker-0.2.0.tar", last modified: Fri Jul 14 15:07:05 2023, max compression
```

## Comparing `cog_worker-0.1.4.tar` & `cog_worker-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,24 @@
-drwxr-xr-x   0 fgassert   (501) staff       (20)        0 2021-11-30 01:04:32.009371 cog_worker-0.1.4/
--rw-r--r--   0 fgassert   (501) staff       (20)     1073 2021-08-04 15:05:21.000000 cog_worker-0.1.4/LICENSE.md
--rw-r--r--   0 fgassert   (501) staff       (20)     3598 2021-11-30 01:04:32.009584 cog_worker-0.1.4/PKG-INFO
--rw-r--r--   0 fgassert   (501) staff       (20)     3119 2021-08-18 20:12:15.000000 cog_worker-0.1.4/README.md
-drwxr-xr-x   0 fgassert   (501) staff       (20)        0 2021-11-30 01:04:32.006345 cog_worker-0.1.4/cog_worker/
--rw-r--r--   0 fgassert   (501) staff       (20)      314 2021-11-30 01:04:28.000000 cog_worker-0.1.4/cog_worker/__init__.py
--rw-r--r--   0 fgassert   (501) staff       (20)     6855 2021-11-30 01:04:28.000000 cog_worker-0.1.4/cog_worker/distributed.py
--rw-r--r--   0 fgassert   (501) staff       (20)    17137 2021-11-30 01:04:28.000000 cog_worker-0.1.4/cog_worker/manager.py
--rw-r--r--   0 fgassert   (501) staff       (20)     1780 2021-08-12 23:38:18.000000 cog_worker-0.1.4/cog_worker/types.py
--rw-r--r--   0 fgassert   (501) staff       (20)     1037 2021-08-11 16:19:00.000000 cog_worker-0.1.4/cog_worker/utils.py
--rw-r--r--   0 fgassert   (501) staff       (20)    10788 2021-11-30 01:04:28.000000 cog_worker-0.1.4/cog_worker/worker.py
-drwxr-xr-x   0 fgassert   (501) staff       (20)        0 2021-11-30 01:04:32.008921 cog_worker-0.1.4/cog_worker.egg-info/
--rw-r--r--   0 fgassert   (501) staff       (20)     3598 2021-11-30 01:04:31.000000 cog_worker-0.1.4/cog_worker.egg-info/PKG-INFO
--rw-r--r--   0 fgassert   (501) staff       (20)      340 2021-11-30 01:04:31.000000 cog_worker-0.1.4/cog_worker.egg-info/SOURCES.txt
--rw-r--r--   0 fgassert   (501) staff       (20)        1 2021-11-30 01:04:31.000000 cog_worker-0.1.4/cog_worker.egg-info/dependency_links.txt
--rw-r--r--   0 fgassert   (501) staff       (20)      216 2021-11-30 01:04:31.000000 cog_worker-0.1.4/cog_worker.egg-info/requires.txt
--rw-r--r--   0 fgassert   (501) staff       (20)       11 2021-11-30 01:04:31.000000 cog_worker-0.1.4/cog_worker.egg-info/top_level.txt
--rw-r--r--   0 fgassert   (501) staff       (20)      547 2021-11-30 01:04:32.010501 cog_worker-0.1.4/setup.cfg
--rw-r--r--   0 fgassert   (501) staff       (20)     1008 2021-11-30 01:04:28.000000 cog_worker-0.1.4/setup.py
+drwxr-xr-x   0 fgassert   (501) staff       (20)        0 2023-07-14 15:07:05.777037 cog_worker-0.2.0/
+-rw-r--r--   0 fgassert   (501) staff       (20)     1073 2021-08-04 15:05:21.000000 cog_worker-0.2.0/LICENSE.md
+-rw-r--r--   0 fgassert   (501) staff       (20)     3579 2023-07-14 15:07:05.777092 cog_worker-0.2.0/PKG-INFO
+-rw-r--r--   0 fgassert   (501) staff       (20)     3119 2021-08-18 20:12:15.000000 cog_worker-0.2.0/README.md
+drwxr-xr-x   0 fgassert   (501) staff       (20)        0 2023-07-14 15:07:05.775833 cog_worker-0.2.0/cog_worker/
+-rw-r--r--   0 fgassert   (501) staff       (20)      314 2023-07-14 15:00:39.000000 cog_worker-0.2.0/cog_worker/__init__.py
+-rw-r--r--   0 fgassert   (501) staff       (20)     6845 2023-07-14 15:00:39.000000 cog_worker-0.2.0/cog_worker/distributed.py
+-rw-r--r--   0 fgassert   (501) staff       (20)    17345 2023-07-14 15:00:39.000000 cog_worker-0.2.0/cog_worker/manager.py
+-rw-r--r--   0 fgassert   (501) staff       (20)     1780 2021-08-12 23:38:18.000000 cog_worker-0.2.0/cog_worker/types.py
+-rw-r--r--   0 fgassert   (501) staff       (20)     1037 2021-08-11 16:19:00.000000 cog_worker-0.2.0/cog_worker/utils.py
+-rw-r--r--   0 fgassert   (501) staff       (20)    10425 2023-07-14 15:00:39.000000 cog_worker-0.2.0/cog_worker/worker.py
+drwxr-xr-x   0 fgassert   (501) staff       (20)        0 2023-07-14 15:07:05.776412 cog_worker-0.2.0/cog_worker.egg-info/
+-rw-r--r--   0 fgassert   (501) staff       (20)     3579 2023-07-14 15:07:05.000000 cog_worker-0.2.0/cog_worker.egg-info/PKG-INFO
+-rw-r--r--   0 fgassert   (501) staff       (20)      429 2023-07-14 15:07:05.000000 cog_worker-0.2.0/cog_worker.egg-info/SOURCES.txt
+-rw-r--r--   0 fgassert   (501) staff       (20)        1 2023-07-14 15:07:05.000000 cog_worker-0.2.0/cog_worker.egg-info/dependency_links.txt
+-rw-r--r--   0 fgassert   (501) staff       (20)      216 2023-07-14 15:07:05.000000 cog_worker-0.2.0/cog_worker.egg-info/requires.txt
+-rw-r--r--   0 fgassert   (501) staff       (20)       11 2023-07-14 15:07:05.000000 cog_worker-0.2.0/cog_worker.egg-info/top_level.txt
+-rw-r--r--   0 fgassert   (501) staff       (20)      547 2023-07-14 15:07:05.777306 cog_worker-0.2.0/setup.cfg
+-rw-r--r--   0 fgassert   (501) staff       (20)     1008 2023-07-14 15:00:39.000000 cog_worker-0.2.0/setup.py
+drwxr-xr-x   0 fgassert   (501) staff       (20)        0 2023-07-14 15:07:05.776913 cog_worker-0.2.0/tests/
+-rw-r--r--   0 fgassert   (501) staff       (20)     1457 2023-07-14 15:00:39.000000 cog_worker-0.2.0/tests/test_distributed.py
+-rw-r--r--   0 fgassert   (501) staff       (20)     2968 2021-10-02 17:26:05.000000 cog_worker-0.2.0/tests/test_manager.py
+-rw-r--r--   0 fgassert   (501) staff       (20)      633 2021-08-11 16:00:29.000000 cog_worker-0.2.0/tests/test_utils.py
+-rw-r--r--   0 fgassert   (501) staff       (20)     2617 2023-07-14 15:00:39.000000 cog_worker-0.2.0/tests/test_worker.py
```

### Comparing `cog_worker-0.1.4/LICENSE.md` & `cog_worker-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cog_worker-0.1.4/PKG-INFO` & `cog_worker-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: cog_worker
-Version: 0.1.4
+Version: 0.2.0
 Summary: Scalable geospatial analysis on Cloud Optimized GeoTIFFs.
 Home-page: https://github.com/vizzuality/cog_worker
 Author: Francis Gassert
 Author-email: francis.gassert@vizzuality.com
 License: MIT
 Keywords: cog geotiff raster gdal rasterio dask
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: distributed
 Provides-Extra: docs
 License-File: LICENSE.md
 
@@ -137,8 +136,7 @@
     bounds = (-180, -90, 180, 90),
     buffer = 128
 )
 
 # Execute in worker pool and save chunks to disk as they complete.
 distributed_manager.chunk_save('output.tif', MyAnalysis, chunksize=2048)
 ```
-
```

### Comparing `cog_worker-0.1.4/README.md` & `cog_worker-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cog_worker-0.1.4/cog_worker/distributed.py` & `cog_worker-0.2.0/cog_worker/distributed.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,11 +168,11 @@
             for params in self.chunk_params(chunksize)
         ]
         if compute:
             futures = self.client.compute(tasks)
             for future, result in dask.distributed.as_completed(
                 futures, with_results=True
             ):
+                future.release()
                 yield result
         else:
-            for t in tasks:
-                yield t  # type: ignore
+            return tasks
```

### Comparing `cog_worker-0.1.4/cog_worker/manager.py` & `cog_worker-0.2.0/cog_worker/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 
 import numpy as np
 import morecantile
 from pyproj import Proj
 import rasterio as rio
 from rasterio.io import DatasetWriter
 import rasterio.windows
+import rasterio.transform
 
 import cog_worker.worker
 from .utils import _bbox_size, _get_profile
 from .types import WorkerFunction, BoundingBox
 
 logger = logging.getLogger(__name__)
 
@@ -291,15 +292,23 @@
         arr: np.ndarray,
         bbox: BoundingBox,
     ):
         """Write a chunk to a rasterio.DatasetWriter."""
         if len(arr.shape) == 2:
             arr = arr[np.newaxis]
         height, width = arr.shape[1:]
-        window = rasterio.windows.from_bounds(*bbox, writer.transform, height, width)
+
+        left, bottom, right, top = bbox
+        rows, cols = rasterio.transform.rowcol(
+            writer.transform,
+            [left],
+            [top],
+            op=round,
+        )
+        window = rasterio.windows.Window(min(cols), min(rows), width, height)
 
         writer.write(arr, window=window)
         if isinstance(arr, np.ma.MaskedArray):
             mask = np.ma.getmask(arr)
             if len(mask.shape) == 3:
                 mask = np.any(mask, axis=0)
             writer.write_mask(~mask, window=window)
```

### Comparing `cog_worker-0.1.4/cog_worker/types.py` & `cog_worker-0.2.0/cog_worker/types.py`

 * *Files identical despite different names*

### Comparing `cog_worker-0.1.4/cog_worker/utils.py` & `cog_worker-0.2.0/cog_worker/utils.py`

 * *Files identical despite different names*

### Comparing `cog_worker-0.1.4/cog_worker/worker.py` & `cog_worker-0.2.0/cog_worker/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,18 @@
 """
 import logging
 from typing import Sequence, Union
 
 from pyproj import Proj
 from pyproj.enums import TransformDirection
 import rasterio as rio
-from rasterio._err import CPLE_AppDefinedError
 import numpy as np
 from rio_tiler.errors import EmptyMosaicError
 from rio_tiler.models import ImageData
-from rio_tiler.io.cogeo import COGReader
+from rio_tiler.io import COGReader
 from rio_tiler.mosaic.reader import mosaic_reader
 
 from cog_worker.types import BoundingBox
 from cog_worker.utils import _bbox_size, _get_profile
 
 logger = logging.getLogger(__name__)
 
@@ -120,14 +119,15 @@
             that covers the Worker's projected extent may be larger
             than the bounding box used to instantiate the Worker.
 
         Args:
             buffered (bool): Buffer the Worker's bounding box.
         """
         pts = max(self.width, self.height) + (buffered * self.buffer * 2) - 1
+        pts = min(pts, 10000)
         bounds = self.xy_bounds(buffered)
         return self.proj.transform_bounds(
             *bounds, pts, direction=TransformDirection.INVERSE
         )
 
     def empty(self, mask: bool = False) -> np.ndarray:
         """Return a zeroed array covering the Worker's extent including the buffer.
@@ -135,20 +135,22 @@
         Args:
             mask (bool): Return a Numpy masked array with all pixels masked.
                 Otherwise returns a standard Numpy array filled with zeros.
         """
         arr = np.zeros((1, self.height + self.buffer * 2, self.width + self.buffer * 2))
         if mask:
             _mask = np.ones(
-                (self.height + self.buffer * 2, self.width + self.buffer * 2)
+                (1, self.height + self.buffer * 2, self.width + self.buffer * 2)
             )
             arr = np.ma.array(arr, mask=_mask)
         return arr
 
-    def read(self, src: Union[str, Sequence[str]], **kwargs) -> np.ma.MaskedArray:
+    def read(
+        self, src: Union[str, Sequence[str]], masked=True, **kwargs
+    ) -> Union[np.ndarray, np.ma.MaskedArray]:
         """Read a COG, reprojecting and clipping as necessary.
 
         The read method uses ``rio_tiler.COGReader`` to takes advantage of the
         file structure and internal overviews in COGs, minimizing the amount of
         data that needs to be read and transferred when working at reduced resolutions.
 
         In general, any valid GDAL path can be read. This may be a url pointing to a COG, a local
@@ -160,14 +162,15 @@
 
         Note:
             The resampling method used to generate the COG's internal overviews will affect
             how it appears at reduced resolutions.
 
         Args:
             src (str, list): The data source to read or list of sources to mosiac.
+            masked (bool): Return a Numpy masked array, otherwise ignore dataset mask.
             **kwargs: Additional keyword arguments to pass to ``rio_tiler.COGReader.part``
                 or ``rio_tiler.mosaic_reader``. See: https://cogeotiff.github.io/rio-tiler/.
 
         Returns:
             A Numpy masked array containing the data for the Worker's bounding box and its
             buffer.
 
@@ -184,18 +187,19 @@
             try:
                 img, asset = mosaic_reader(
                     src, _read_COG, proj_bounds, self.proj.crs, width, height, **kwargs
                 )
             except EmptyMosaicError:
                 return self.empty(mask=True)
 
-        arr = img.data
-        mask = (img.mask == 0) | np.isnan(arr)
+        arr = img.array
 
-        return np.ma.array(arr, mask=mask)
+        if not masked:
+            return arr.data
+        return arr
 
     def write(self, arr: np.ndarray, dst: str, **kwargs):
         """Write a Numpy array to a GeoTIFF.
 
         The write method will create a GeoTIFF with a profile matching the Worker's properties.
         Uses ``rasterio.open`` under the hood.
 
@@ -260,27 +264,16 @@
     proj_bounds: BoundingBox,
     crs: Union[str, int, Proj],
     width: int,
     height: int,
     **kwargs,
 ) -> ImageData:
     """Read part of a COG, warping and resampling to a target shape."""
-    tries = 6
-    while tries > 0:
-        try:
-            with COGReader(asset, **kwargs) as cog:  # type: ignore
-                return cog.part(
-                    proj_bounds,
-                    bounds_crs=crs,
-                    dst_crs=crs,
-                    max_size=None,
-                    width=width,
-                    height=height,
-                )
-        except CPLE_AppDefinedError as e:
-            # Ignore some strange GDAL errors when reading in some projections
-            # see: https://rasterio.groups.io/g/main/message/780
-            logger.debug(e)
-            if tries <= 1:
-                raise e
-        tries -= 1
-    raise Exception(f"Failed reading asset {asset}")
+    with COGReader(asset, **kwargs) as cog:  # type: ignore
+        return cog.part(
+            proj_bounds,
+            bounds_crs=crs,
+            dst_crs=crs,
+            max_size=None,
+            width=width,
+            height=height,
+        )
```

### Comparing `cog_worker-0.1.4/cog_worker.egg-info/PKG-INFO` & `cog_worker-0.2.0/cog_worker.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: cog-worker
-Version: 0.1.4
+Version: 0.2.0
 Summary: Scalable geospatial analysis on Cloud Optimized GeoTIFFs.
 Home-page: https://github.com/vizzuality/cog_worker
 Author: Francis Gassert
 Author-email: francis.gassert@vizzuality.com
 License: MIT
 Keywords: cog geotiff raster gdal rasterio dask
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: distributed
 Provides-Extra: docs
 License-File: LICENSE.md
 
@@ -137,8 +136,7 @@
     bounds = (-180, -90, 180, 90),
     buffer = 128
 )
 
 # Execute in worker pool and save chunks to disk as they complete.
 distributed_manager.chunk_save('output.tif', MyAnalysis, chunksize=2048)
 ```
-
```

### Comparing `cog_worker-0.1.4/setup.cfg` & `cog_worker-0.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [bumpversion]
 commit = True
 tag = True
-current_version = 0.1.4
+current_version = 0.2.0
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
 
 [bumpversion:file:cog_worker/__init__.py]
 search = __version__ = "{current_version}"
```

### Comparing `cog_worker-0.1.4/setup.py` & `cog_worker-0.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 from setuptools import setup
 
 with open("README.md") as f:
     desc = f.read()
 
 setup(
     name="cog_worker",
-    version="0.1.4",
+    version="0.2.0",
     description="Scalable geospatial analysis on Cloud Optimized GeoTIFFs.",
     long_description=desc,
     long_description_content_type="text/markdown",
     license="MIT",
     author="Francis Gassert",
     author_email="francis.gassert@vizzuality.com",
     url="https://github.com/vizzuality/cog_worker",
     packages=["cog_worker"],
     keywords="cog geotiff raster gdal rasterio dask",
     install_requires=[
         "numpy>=1,<2",
         "pyproj>=3.0.0,<4",
-        "rasterio>=1.2,<2",
-        "morecantile>=3.0.0,<4",
-        "rio_tiler>=3.0.0,<4",
+        "rasterio>=1.3,<2",
+        "morecantile>=4.3.0,<5",
+        "rio_tiler>=5.0.0,<6",
     ],
     extras_require={
         "test": ["pytest"],
         "dev": ["pre-commit"],
         "distributed": ["dask[distributed]"],
         "docs": [
             "Sphinx",
```

