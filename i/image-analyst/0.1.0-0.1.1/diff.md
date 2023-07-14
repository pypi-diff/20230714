# Comparing `tmp/image_analyst-0.1.0.tar.gz` & `tmp/image_analyst-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_analyst-0.1.0.tar", max compression
+gzip compressed data, was "image_analyst-0.1.1.tar", max compression
```

## Comparing `image_analyst-0.1.0.tar` & `image_analyst-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1088 2023-07-14 16:39:57.000153 image_analyst-0.1.0/LICENSE
--rw-r--r--   0        0        0      895 2023-07-14 17:00:03.455687 image_analyst-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      885 2023-07-14 16:43:27.012629 image_analyst-0.1.0/README.md
--rw-r--r--   0        0        0     3262 2023-07-14 16:30:33.796322 image_analyst-0.1.0/src/image_analyst/analyzers.py
--rw-r--r--   0        0        0      860 2023-07-14 16:31:22.972890 image_analyst-0.1.0/src/image_analyst/exceptions.py
--rw-r--r--   0        0        0    10765 2023-07-14 16:34:50.369226 image_analyst-0.1.0/src/image_analyst/image.py
--rw-r--r--   0        0        0     1928 2023-07-14 15:36:16.430223 image_analyst-0.1.0/src/image_analyst/models.py
--rw-r--r--   0        0        0     6421 2023-07-14 16:35:39.510440 image_analyst-0.1.0/src/image_analyst/trackers.py
--rw-r--r--   0        0        0     5505 2023-07-14 16:34:33.341203 image_analyst-0.1.0/src/image_analyst/utils.py
--rw-r--r--   0        0        0     1461 1970-01-01 00:00:00.000000 image_analyst-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-07-14 16:39:57.000153 image_analyst-0.1.1/LICENSE
+-rw-r--r--   0        0        0      989 2023-07-14 21:02:14.347031 image_analyst-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      885 2023-07-14 16:43:27.012629 image_analyst-0.1.1/README.md
+-rw-r--r--   0        0        0     3262 2023-07-14 16:30:33.796322 image_analyst-0.1.1/src/image_analyst/analyzers.py
+-rw-r--r--   0        0        0      860 2023-07-14 16:31:22.972890 image_analyst-0.1.1/src/image_analyst/exceptions.py
+-rw-r--r--   0        0        0    10784 2023-07-14 20:52:32.058152 image_analyst-0.1.1/src/image_analyst/image.py
+-rw-r--r--   0        0        0     1928 2023-07-14 15:36:16.430223 image_analyst-0.1.1/src/image_analyst/models.py
+-rw-r--r--   0        0        0     6421 2023-07-14 16:35:39.510440 image_analyst-0.1.1/src/image_analyst/trackers.py
+-rw-r--r--   0        0        0     5505 2023-07-14 16:34:33.341203 image_analyst-0.1.1/src/image_analyst/utils.py
+-rw-r--r--   0        0        0     1606 1970-01-01 00:00:00.000000 image_analyst-0.1.1/PKG-INFO
```

### Comparing `image_analyst-0.1.0/LICENSE` & `image_analyst-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `image_analyst-0.1.0/pyproject.toml` & `image_analyst-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 [tool.poetry]
 name = "image-analyst"
-version = "0.1.0"
+version = "0.1.1"
 description = "ImageAnalyst is a library that simplifies image analysis."
 authors = ["Lucas Berg <55436804+BergLucas@users.noreply.github.com>"]
+repository = "https://github.com/BergLucas/ImageAnalyst"
+keywords = ["image", "analysis"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License"
 ]
 packages = [{ include = "image_analyst", from = "src" }]
@@ -31,8 +33,8 @@
 branch = true
 source = [
     "src/image_analyst",
     "tests"
 ]
 
 [tool.mypy]
-ignore_missing_imports = true
+ignore_missing_imports = true
```

### Comparing `image_analyst-0.1.0/README.md` & `image_analyst-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `image_analyst-0.1.0/src/image_analyst/analyzers.py` & `image_analyst-0.1.1/src/image_analyst/analyzers.py`

 * *Files identical despite different names*

### Comparing `image_analyst-0.1.0/src/image_analyst/exceptions.py` & `image_analyst-0.1.1/src/image_analyst/exceptions.py`

 * *Files identical despite different names*

### Comparing `image_analyst-0.1.0/src/image_analyst/image.py` & `image_analyst-0.1.1/src/image_analyst/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,33 +28,33 @@
     @property
     def center(self) -> tuple[int, int]:
         """Gets the center of the bounding box.
 
         Returns:
             tuple[int, int]: the center (x, y).
         """
-        return ((self.xmax + self.xmin) // 2, (self.ymax + self.ymin) // 2)
+        return (self.xmin + self.width // 2, self.ymin + self.height // 2)
 
     @property
     def width(self) -> int:
         """Gets the width of the bounding box.
 
         Returns:
             int: the width.
         """
-        return self.xmax - self.xmin
+        return self.xmax - self.xmin + 1
 
     @property
     def height(self) -> int:
         """Gets the height of the bounding box.
 
         Returns:
             int: the height.
         """
-        return self.ymax - self.ymin
+        return self.ymax - self.ymin + 1
 
     def as_tuple(self) -> tuple[int, int, int, int]:
         """Gets the bounding box as a tuple.
 
         Returns:
             tuple[int, int, int, int]: the bounding box
                 as a tuple (xmin, ymin, xmax, ymax).
@@ -318,10 +318,10 @@
         )
 
         result = np.zeros((new_height, new_width, channels), dtype=image.dtype)
 
         xmax = xmin + embedded_width - 1
         ymax = ymin + embedded_height - 1
 
-        result[ymin:ymax, xmin:xmax, :] = embedded_image
+        result[ymin : ymax + 1, xmin : xmax + 1, :] = embedded_image
 
         return result, BoundingBox(xmin=xmin, ymin=ymin, xmax=xmax, ymax=ymax)
```

### Comparing `image_analyst-0.1.0/src/image_analyst/models.py` & `image_analyst-0.1.1/src/image_analyst/models.py`

 * *Files identical despite different names*

### Comparing `image_analyst-0.1.0/src/image_analyst/trackers.py` & `image_analyst-0.1.1/src/image_analyst/trackers.py`

 * *Files identical despite different names*

### Comparing `image_analyst-0.1.0/src/image_analyst/utils.py` & `image_analyst-0.1.1/src/image_analyst/utils.py`

 * *Files identical despite different names*

### Comparing `image_analyst-0.1.0/PKG-INFO` & `image_analyst-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: image-analyst
-Version: 0.1.0
+Version: 0.1.1
 Summary: ImageAnalyst is a library that simplifies image analysis.
+Home-page: https://github.com/BergLucas/ImageAnalyst
+Keywords: image,analysis
 Author: Lucas Berg
 Author-email: 55436804+BergLucas@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
+Project-URL: Repository, https://github.com/BergLucas/ImageAnalyst
 Description-Content-Type: text/markdown
 
 # ImageAnalyst
 
 ImageAnalyst is a library that simplifies image analysis. The library achieves this goal by standardizing the input and output
 vectors of a few machine learning models and by providing some high-level analysis algorithms.
```

