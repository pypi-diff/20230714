# Comparing `tmp/isometry-1.0.1.tar.gz` & `tmp/isometry-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isometry-1.0.1.tar", last modified: Fri Jul 14 11:58:41 2023, max compression
+gzip compressed data, was "isometry-1.0.2.tar", last modified: Fri Jul 14 12:16:04 2023, max compression
```

## Comparing `isometry-1.0.1.tar` & `isometry-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 11:58:41.633643 isometry-1.0.1/
--rw-rw-rw-   0        0        0     1091 2023-07-14 11:07:30.000000 isometry-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     1675 2023-07-14 11:58:41.633643 isometry-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1312 2023-07-14 11:57:59.000000 isometry-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 11:58:41.580643 isometry-1.0.1/isometry/
--rw-rw-rw-   0        0        0       32 2023-06-29 11:08:57.000000 isometry-1.0.1/isometry/__init__.py
--rw-rw-rw-   0        0        0     7047 2023-07-14 11:54:23.000000 isometry-1.0.1/isometry/isometry.py
-drwxrwxrwx   0        0        0        0 2023-07-14 11:58:41.632651 isometry-1.0.1/isometry.egg-info/
--rw-rw-rw-   0        0        0     1675 2023-07-14 11:58:41.000000 isometry-1.0.1/isometry.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-07-14 11:58:41.000000 isometry-1.0.1/isometry.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 11:58:41.000000 isometry-1.0.1/isometry.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-07-14 11:58:41.000000 isometry-1.0.1/isometry.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-14 11:58:41.000000 isometry-1.0.1/isometry.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 11:58:41.640644 isometry-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      931 2023-07-14 11:58:20.000000 isometry-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 12:16:04.848687 isometry-1.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-07-14 11:07:30.000000 isometry-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1817 2023-07-14 12:16:04.848687 isometry-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1454 2023-07-14 12:11:35.000000 isometry-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 12:16:04.824686 isometry-1.0.2/isometry/
+-rw-rw-rw-   0        0        0       32 2023-06-29 11:08:57.000000 isometry-1.0.2/isometry/__init__.py
+-rw-rw-rw-   0        0        0     7047 2023-07-14 12:03:18.000000 isometry-1.0.2/isometry/isometry.py
+drwxrwxrwx   0        0        0        0 2023-07-14 12:16:04.847685 isometry-1.0.2/isometry.egg-info/
+-rw-rw-rw-   0        0        0     1817 2023-07-14 12:16:04.000000 isometry-1.0.2/isometry.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-07-14 12:16:04.000000 isometry-1.0.2/isometry.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 12:16:04.000000 isometry-1.0.2/isometry.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-07-14 12:16:04.000000 isometry-1.0.2/isometry.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-14 12:16:04.000000 isometry-1.0.2/isometry.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 12:16:04.851685 isometry-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      679 2023-07-14 12:15:58.000000 isometry-1.0.2/setup.py
```

### Comparing `isometry-1.0.1/LICENSE` & `isometry-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `isometry-1.0.1/PKG-INFO` & `isometry-1.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isometry
-Version: 1.0.1
+Version: 1.0.2
 Summary: Package to get isometric image by three images
 Home-page: https://github.com/anton8963kobelev/isometry
 Author: akobelev
 Author-email: ya@akobelev.ru
 Keywords: isometry three images 3Ddimensions isometric
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -42,7 +42,10 @@
 isomentric_image.save('isomentric_image_pil.png')
 ```
 **Be careful: while using Pillow library parameter ```is_pil_format``` must be True (default value is False)**
 
 #### Additional parameters
 * ```angle``` - angle in degrees between three images in final isometric image (*default=30*);
 * ```is_crop_white_background``` - if ```True``` -> white background on each three input images will be deleted (*default=False*)
+
+## Isometric image example
+![isometric_image](https://github.com/anton8963kobelev/isometry/blob/main/images/isometric_image.png?raw=true)
```

### Comparing `isometry-1.0.1/README.md` & `isometry-1.0.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -30,7 +30,10 @@
 isomentric_image.save('isomentric_image_pil.png')
 ```
 **Be careful: while using Pillow library parameter ```is_pil_format``` must be True (default value is False)**
 
 #### Additional parameters
 * ```angle``` - angle in degrees between three images in final isometric image (*default=30*);
 * ```is_crop_white_background``` - if ```True``` -> white background on each three input images will be deleted (*default=False*)
+
+## Isometric image example
+![isometric_image](https://github.com/anton8963kobelev/isometry/blob/main/images/isometric_image.png?raw=true)
```

### Comparing `isometry-1.0.1/isometry/isometry.py` & `isometry-1.0.2/isometry/isometry.py`

 * *Files identical despite different names*

### Comparing `isometry-1.0.1/isometry.egg-info/PKG-INFO` & `isometry-1.0.2/isometry.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isometry
-Version: 1.0.1
+Version: 1.0.2
 Summary: Package to get isometric image by three images
 Home-page: https://github.com/anton8963kobelev/isometry
 Author: akobelev
 Author-email: ya@akobelev.ru
 Keywords: isometry three images 3Ddimensions isometric
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -42,7 +42,10 @@
 isomentric_image.save('isomentric_image_pil.png')
 ```
 **Be careful: while using Pillow library parameter ```is_pil_format``` must be True (default value is False)**
 
 #### Additional parameters
 * ```angle``` - angle in degrees between three images in final isometric image (*default=30*);
 * ```is_crop_white_background``` - if ```True``` -> white background on each three input images will be deleted (*default=False*)
+
+## Isometric image example
+![isometric_image](https://github.com/anton8963kobelev/isometry/blob/main/images/isometric_image.png?raw=true)
```

