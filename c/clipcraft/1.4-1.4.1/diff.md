# Comparing `tmp/clipcraft-1.4.tar.gz` & `tmp/clipcraft-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipcraft-1.4.tar", last modified: Fri Jul 14 17:19:00 2023, max compression
+gzip compressed data, was "clipcraft-1.4.1.tar", last modified: Fri Jul 14 17:27:30 2023, max compression
```

## Comparing `clipcraft-1.4.tar` & `clipcraft-1.4.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 17:19:00.215490 clipcraft-1.4/
--rw-rw-rw-   0        0        0     3767 2023-07-14 17:19:00.215490 clipcraft-1.4/PKG-INFO
--rw-rw-rw-   0        0        0     3428 2023-07-14 17:15:39.000000 clipcraft-1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 17:19:00.198427 clipcraft-1.4/clipcraft/
--rw-rw-rw-   0        0        0      128 2023-07-14 14:35:14.000000 clipcraft-1.4/clipcraft/__init__.py
--rw-rw-rw-   0        0        0     8285 2023-07-14 17:17:11.000000 clipcraft-1.4/clipcraft/create_embeddings.py
--rw-rw-rw-   0        0        0     3585 2023-07-14 17:17:14.000000 clipcraft-1.4/clipcraft/knn_search.py
-drwxrwxrwx   0        0        0        0 2023-07-14 17:19:00.214419 clipcraft-1.4/clipcraft.egg-info/
--rw-rw-rw-   0        0        0     3767 2023-07-14 17:19:00.000000 clipcraft-1.4/clipcraft.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-07-14 17:19:00.000000 clipcraft-1.4/clipcraft.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 17:19:00.000000 clipcraft-1.4/clipcraft.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-07-14 17:19:00.000000 clipcraft-1.4/clipcraft.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-14 17:19:00.000000 clipcraft-1.4/clipcraft.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 17:19:00.216746 clipcraft-1.4/setup.cfg
--rw-rw-rw-   0        0        0      640 2023-07-14 17:18:41.000000 clipcraft-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 17:27:30.098257 clipcraft-1.4.1/
+-rw-rw-rw-   0        0        0     3769 2023-07-14 17:27:30.098257 clipcraft-1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3428 2023-07-14 17:15:39.000000 clipcraft-1.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 17:27:30.081120 clipcraft-1.4.1/clipcraft/
+-rw-rw-rw-   0        0        0      128 2023-07-14 14:35:14.000000 clipcraft-1.4.1/clipcraft/__init__.py
+-rw-rw-rw-   0        0        0     8285 2023-07-14 17:25:01.000000 clipcraft-1.4.1/clipcraft/create_embeddings.py
+-rw-rw-rw-   0        0        0     3583 2023-07-14 17:25:03.000000 clipcraft-1.4.1/clipcraft/knn_search.py
+drwxrwxrwx   0        0        0        0 2023-07-14 17:27:30.098257 clipcraft-1.4.1/clipcraft.egg-info/
+-rw-rw-rw-   0        0        0     3769 2023-07-14 17:27:29.000000 clipcraft-1.4.1/clipcraft.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-07-14 17:27:29.000000 clipcraft-1.4.1/clipcraft.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 17:27:29.000000 clipcraft-1.4.1/clipcraft.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-07-14 17:27:29.000000 clipcraft-1.4.1/clipcraft.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-14 17:27:29.000000 clipcraft-1.4.1/clipcraft.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 17:27:30.098257 clipcraft-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      642 2023-07-14 17:27:19.000000 clipcraft-1.4.1/setup.py
```

### Comparing `clipcraft-1.4/PKG-INFO` & `clipcraft-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipcraft
-Version: 1.4
+Version: 1.4.1
 Summary: A package for CLIP-based image and text processing.
 Home-page: https://github.com/mmckenzieORCEN/CLIPCraft
 Author: Morgan McKenzie
 Author-email: morgancmckenziecs@gmail.com
 Description-Content-Type: text/markdown
 
 # CLIPCraft
```

### Comparing `clipcraft-1.4/README.md` & `clipcraft-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `clipcraft-1.4/clipcraft/create_embeddings.py` & `clipcraft-1.4.1/clipcraft/create_embeddings.py`

 * *Files identical despite different names*

### Comparing `clipcraft-1.4/clipcraft/knn_search.py` & `clipcraft-1.4.1/clipcraft/knn_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from PIL import Image
 import numpy as np
 import requests
 from io import BytesIO
-from . import create_embeddings
+from .create_embeddings import _imageEmbeddings
 
 # User-callable function to display KNN, or most similar images to given text
 def KNNSearchImage(text_embeddings, image_embeddings):
      #Since we returned the image embeddings as a list of tuples, we grab the embedding tuples
     image_embeddings_array = np.stack([embedding for _, embedding in image_embeddings])
     text_embeddings_array = np.stack([embedding for _, embedding in text_embeddings])
     
@@ -50,15 +50,15 @@
     text_embeddings_array = np.stack([embedding for _, embedding in text_embeddings])
     result = []
     # Determine if we have only one image url as input
     if isinstance(image_urls, str):
         image_urls = [image_urls]  # Convert single URL to a list
 
     # Here we create a list of image embeddings by calling internal function
-    image_embeddings = create_embeddings._imageEmbeddings(image_urls)
+    image_embeddings = _imageEmbeddings(image_urls)
     #Once again using NumPy stack method to get a 1d array of embeddings
     image_embeddings_array = np.stack([embedding for _, embedding in image_embeddings])
 
     # Iterating over each URL in list
     for i in range(len(image_urls)):
 
         # Calculate the Euclidean distances between the text and image embeddings
```

### Comparing `clipcraft-1.4/clipcraft.egg-info/PKG-INFO` & `clipcraft-1.4.1/clipcraft.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipcraft
-Version: 1.4
+Version: 1.4.1
 Summary: A package for CLIP-based image and text processing.
 Home-page: https://github.com/mmckenzieORCEN/CLIPCraft
 Author: Morgan McKenzie
 Author-email: morgancmckenziecs@gmail.com
 Description-Content-Type: text/markdown
 
 # CLIPCraft
```

### Comparing `clipcraft-1.4/setup.py` & `clipcraft-1.4.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', 'r', encoding='utf-8') as readme_file:
     long_description = readme_file.read()
 
 setup(
     name="clipcraft",
-    version="1.4",
+    version="1.4.1",
     description="A package for CLIP-based image and text processing.",
     author='Morgan McKenzie',
     author_email='morgancmckenziecs@gmail.com',
     packages=["clipcraft"],
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/mmckenzieORCEN/CLIPCraft',
```

