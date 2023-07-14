# Comparing `tmp/waterfly-14.7.2023.22.16.tar.gz` & `tmp/waterfly-8.7.2023.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waterfly-14.7.2023.22.16.tar", last modified: Fri Jul 14 19:14:55 2023, max compression
+gzip compressed data, was "waterfly-8.7.2023.tar", last modified: Sat Jul  8 18:40:09 2023, max compression
```

## Comparing `waterfly-14.7.2023.22.16.tar` & `waterfly-8.7.2023.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 19:14:55.579633 waterfly-14.7.2023.22.16/
--rw-rw-rw-   0        0        0     3814 2023-07-14 19:14:55.579633 waterfly-14.7.2023.22.16/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-14 19:14:55.579633 waterfly-14.7.2023.22.16/setup.cfg
--rw-rw-rw-   0        0        0     4078 2023-07-14 19:14:30.000000 waterfly-14.7.2023.22.16/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-14 19:14:55.548391 waterfly-14.7.2023.22.16/waterfly/
--rw-rw-rw-   0        0        0    35140 2023-07-14 18:59:58.000000 waterfly-14.7.2023.22.16/waterfly/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 19:14:55.579633 waterfly-14.7.2023.22.16/waterfly.egg-info/
--rw-rw-rw-   0        0        0     3814 2023-07-14 19:14:55.000000 waterfly-14.7.2023.22.16/waterfly.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-07-14 19:14:55.000000 waterfly-14.7.2023.22.16/waterfly.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 19:14:55.000000 waterfly-14.7.2023.22.16/waterfly.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-07-14 19:14:55.000000 waterfly-14.7.2023.22.16/waterfly.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-14 19:14:55.000000 waterfly-14.7.2023.22.16/waterfly.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 18:40:09.640290 waterfly-8.7.2023/
+-rw-rw-rw-   0        0        0     1822 2023-07-08 18:40:09.640290 waterfly-8.7.2023/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-08 18:40:09.640290 waterfly-8.7.2023/setup.cfg
+-rw-rw-rw-   0        0        0     2173 2023-07-08 18:34:35.000000 waterfly-8.7.2023/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 18:40:09.593429 waterfly-8.7.2023/waterfly/
+-rw-rw-rw-   0        0        0     7887 2023-07-08 17:40:07.000000 waterfly-8.7.2023/waterfly/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 18:40:09.640290 waterfly-8.7.2023/waterfly.egg-info/
+-rw-rw-rw-   0        0        0     1822 2023-07-08 18:40:09.000000 waterfly-8.7.2023/waterfly.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-07-08 18:40:09.000000 waterfly-8.7.2023/waterfly.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 18:40:09.000000 waterfly-8.7.2023/waterfly.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-08 18:40:09.000000 waterfly-8.7.2023/waterfly.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-08 18:40:09.000000 waterfly-8.7.2023/waterfly.egg-info/top_level.txt
```

### Comparing `waterfly-14.7.2023.22.16/setup.py` & `waterfly-8.7.2023/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,83 +1,47 @@
 from setuptools import setup
 
 setup(
     name='waterfly',
-    version='14.7.2023.22.16',
+    version='8.7.2023',
     install_requires=[
         'googletrans>=3.1.0a0',
         'opencv-python',
-        'rembg',
-        'requests',
-        'pyautogui'
+        'rembg'
     ],
-    description='Waterfly is a powerful new AI tool to create Firefly URLs, process images, and draw on images.',
+    description='''Waterfly is a powerful new AI tool
+that reserves as partly an unofficial client for Adobe Firefly,
+to create Firefly URLs, process images, and draw on images.''',
     long_description='''
 
 Hi here!
 
-–––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––
-
-    ABOUT NEW
-
-— New functions such as create.textimage(), create.palette(), edit.oldtv(), random.image_url(), 
-  info.image.created(), info.image.motificated(), info.image.exist() and more
-
-— Added a filter for premium images, now when you generate premium images,
-  images with watermarks are ignored!
-
-— The code is now better commented
-
-–––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––
-
-    CREATE URLS FOR IMAGES AND TEXT STYLES
-
+Create URLs for images and text styles, for example:
 create.image('Chocolate tree', ['hyper_realistic', 'cool_colors', 'studio_light'], 'portrait')
 Create a great photo of a chocolate tree for your Instagram stories with very realistic graphics,
 beautiful colors, and studio lighting.
 Not interested in stories? Create something else! Example:
 create.image('Sakura tree', ['cartoon', 'beautiful', 'pastel_colors', dramatic_light'], 'widescreen')
 Creates a beautifully drawn picture of a sakura tree, in cartoon style, beautiful,
 in pastel colors and with dramatic lighting,
 with an aspect ratio that is ideal for desktop backgrounds
 
 –––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––
 
-    ALREADY HAVE THE IMAGE YOU NEED? EDIT IT!
+Already have the image you need? Edit it!
 
 The code that will remove the background:
-edit.backdrop('image.img', 'backdrop.img')
+edit.backdrop('image.img')
 You can add a vignette like this:
 edit.vignette('image.img', level)
 Turn the image into a cartoon:
 edit.cartoon('image.img')
 
 –––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––
 
-    LIFEHACKS
-
-1. A vulnerability has been discovered in Adobe Firefly, you can upload images without a watermark!
-   Check the element code and find the img tag with alt="Variation n of 4",
-   follow the link in the src and upload the image with the PNG or JPG extension
-
-2. If you don't know how much time it takes to create random image, itc.
-
-        from waterfly import*
-        from time import time
-
-        start = time()
-        random.image()
-        print(f'The code execution took {time()-start} seconds')
-
-   The result should be as follows
-
-        The code execution took 0.9839651584625244 seconds
-
-–––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––
-
 Want to point out something in an image?
 Build any shape with lines and ellipses!
 
 And much more...
 
 ''',
     author = 'Igor_Shapovalov_Andrejovich',
```

