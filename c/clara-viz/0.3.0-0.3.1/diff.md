# Comparing `tmp/clara_viz-0.3.0-py2.py3-none-any.whl.zip` & `tmp/clara_viz-0.3.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 9416 bytes, number of entries: 8
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-22 07:56 clara/viz/VERSION
+Zip file size: 9471 bytes, number of entries: 8
+-rw-r--r--  2.0 unx        6 b- defN 23-Jul-12 11:16 clara/viz/VERSION
 -rw-r--r--  2.0 unx      710 b- defN 21-Nov-16 13:11 clara/viz/__init__.py
 -rw-r--r--  2.0 unx     1626 b- defN 21-Dec-06 12:45 clara/viz/_version.py
--rw-rw-r--  2.0 unx    11419 b- defN 23-Jun-22 07:56 clara_viz-0.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     6660 b- defN 23-Jun-22 07:56 clara_viz-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-22 07:56 clara_viz-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-22 07:56 clara_viz-0.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      623 b- defN 23-Jun-22 07:56 clara_viz-0.3.0.dist-info/RECORD
-8 files, 21160 bytes uncompressed, 8330 bytes compressed:  60.6%
+-rw-rw-r--  2.0 unx    11419 b- defN 23-Jul-12 11:16 clara_viz-0.3.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6799 b- defN 23-Jul-12 11:16 clara_viz-0.3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-12 11:16 clara_viz-0.3.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jul-12 11:16 clara_viz-0.3.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      623 b- defN 23-Jul-12 11:16 clara_viz-0.3.1.dist-info/RECORD
+8 files, 21299 bytes uncompressed, 8385 bytes compressed:  60.6%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: clara/viz/__init__.py
 Comment: 
 
 Filename: clara/viz/_version.py
 Comment: 
 
-Filename: clara_viz-0.3.0.dist-info/LICENSE
+Filename: clara_viz-0.3.1.dist-info/LICENSE
 Comment: 
 
-Filename: clara_viz-0.3.0.dist-info/METADATA
+Filename: clara_viz-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: clara_viz-0.3.0.dist-info/WHEEL
+Filename: clara_viz-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: clara_viz-0.3.0.dist-info/top_level.txt
+Filename: clara_viz-0.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: clara_viz-0.3.0.dist-info/RECORD
+Filename: clara_viz-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## clara/viz/VERSION

```diff
@@ -1 +1 @@
-0.3.0
+0.3.1
```

## Comparing `clara_viz-0.3.0.dist-info/LICENSE` & `clara_viz-0.3.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `clara_viz-0.3.0.dist-info/METADATA` & `clara_viz-0.3.1.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clara-viz
-Version: 0.3.0
+Version: 0.3.1
 Summary: A toolkit to provide GPU accelerated visualization of medical data.
 Home-page: https://github.com/NVIDIA/clara-viz
 Author: NVIDIA Corporation
 License: Apache-2.0
 Platform: manylinux_2_28_x86_64
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -14,16 +14,16 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >= 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: packaging
-Requires-Dist: clara-viz-core (==0.3.0)
-Requires-Dist: clara-viz-widgets (==0.3.0)
+Requires-Dist: clara-viz-core (==0.3.1)
+Requires-Dist: clara-viz-widgets (==0.3.1)
 
 # Quick Start
 
 ## Installation
 
 This will install all Clara Viz packages use pip:
 
@@ -80,14 +80,21 @@
 rgb_data = np.asarray(output)[:, :, :3]
 
 # show with PIL
 image = Image.fromarray(rgb_data)
 image.show()
 ```
 
+# clara-viz 0.3.1 (July 12 2023)
+
+## Bug Fixes
+
+* Gracefully disable OptiX denoiser if it can't be created
+* make nvjpeg support optional
+
 # clara-viz 0.3.0 (June 22 2023)
 
 ## Features
 
 * C++ interface is now public
 * Add support for aarch64 (not for Python wheels)
 * Add support for VR/AR rendering
```

