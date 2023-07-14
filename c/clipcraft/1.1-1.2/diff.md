# Comparing `tmp/clipcraft-1.1.tar.gz` & `tmp/clipcraft-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipcraft-1.1.tar", last modified: Fri Jul 14 14:46:43 2023, max compression
+gzip compressed data, was "clipcraft-1.2.tar", last modified: Fri Jul 14 16:43:46 2023, max compression
```

## Comparing `clipcraft-1.1.tar` & `clipcraft-1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 14:46:43.603839 clipcraft-1.1/
--rw-rw-rw-   0        0        0     3581 2023-07-14 14:46:43.603839 clipcraft-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3242 2023-07-14 14:35:14.000000 clipcraft-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 14:46:43.574205 clipcraft-1.1/clipcraft/
--rw-rw-rw-   0        0        0      128 2023-07-14 14:35:14.000000 clipcraft-1.1/clipcraft/__init__.py
--rw-rw-rw-   0        0        0     8166 2023-07-14 14:35:14.000000 clipcraft-1.1/clipcraft/create_embeddings.py
--rw-rw-rw-   0        0        0     3533 2023-07-14 14:35:14.000000 clipcraft-1.1/clipcraft/knn_search.py
-drwxrwxrwx   0        0        0        0 2023-07-14 14:46:43.600023 clipcraft-1.1/clipcraft.egg-info/
--rw-rw-rw-   0        0        0     3581 2023-07-14 14:46:43.000000 clipcraft-1.1/clipcraft.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-07-14 14:46:43.000000 clipcraft-1.1/clipcraft.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 14:46:43.000000 clipcraft-1.1/clipcraft.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-07-14 14:46:43.000000 clipcraft-1.1/clipcraft.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-14 14:46:43.000000 clipcraft-1.1/clipcraft.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 14:46:43.603839 clipcraft-1.1/setup.cfg
--rw-rw-rw-   0        0        0      640 2023-07-14 14:45:44.000000 clipcraft-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 16:43:46.013834 clipcraft-1.2/
+-rw-rw-rw-   0        0        0     3766 2023-07-14 16:43:46.013834 clipcraft-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3427 2023-07-14 16:29:27.000000 clipcraft-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 16:43:46.002434 clipcraft-1.2/clipcraft/
+-rw-rw-rw-   0        0        0      128 2023-07-14 14:35:14.000000 clipcraft-1.2/clipcraft/__init__.py
+-rw-rw-rw-   0        0        0     8256 2023-07-14 16:25:37.000000 clipcraft-1.2/clipcraft/create_embeddings.py
+-rw-rw-rw-   0        0        0     3535 2023-07-14 16:15:59.000000 clipcraft-1.2/clipcraft/knn_search.py
+drwxrwxrwx   0        0        0        0 2023-07-14 16:43:46.013834 clipcraft-1.2/clipcraft.egg-info/
+-rw-rw-rw-   0        0        0     3766 2023-07-14 16:43:45.000000 clipcraft-1.2/clipcraft.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-07-14 16:43:45.000000 clipcraft-1.2/clipcraft.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 16:43:45.000000 clipcraft-1.2/clipcraft.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-07-14 16:43:45.000000 clipcraft-1.2/clipcraft.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-14 16:43:45.000000 clipcraft-1.2/clipcraft.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 16:43:46.013834 clipcraft-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      640 2023-07-14 16:30:26.000000 clipcraft-1.2/setup.py
```

### Comparing `clipcraft-1.1/PKG-INFO` & `clipcraft-1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipcraft
-Version: 1.1
+Version: 1.2
 Summary: A package for CLIP-based image and text processing.
 Home-page: https://github.com/mmckenzieORCEN/CLIPCraft
 Author: Morgan McKenzie
 Author-email: morgancmckenziecs@gmail.com
 Description-Content-Type: text/markdown
 
 # CLIPCraft
@@ -37,25 +37,25 @@
 
 **KNNSearchText(text_embeddings, image_urls)** This function will find the most similar caption to a given image. It is designed for use by providing the list returned from createTextEmbeddings. text_embeddings should be the return value of createTextEmbeddings, while image_urls should be a single URL or a list of URLs. 
 
 ## Example
 ```python
 import clipcraft as cc
 
-file_urls = ["first_100_rows.json.gz"]
+file_urls = "https://upload.wikimedia.org/wikipedia/commons/thumb/6/68/Orange_tabby_cat_sitting_on_fallen_leaves-Hisashi-01A.jpg/800px-Orange_tabby_cat_sitting_on_fallen_leaves-Hisashi-01A.jpg"
 
 image_embeds = cc.createImageEmbeddings(file_urls)
 
-text_embed_list = ["a man in a green jacket and a basketball player in a white shirt",  "Grandma with makeup", "Football player"]
+text_embed_list = ["a picture of a cat"]
 
 text_embeds = cc.createTextEmbeddings(text_embed_list)
 
 cc.KNNSearchImage(text_embeds, image_embeds)
 
-cc.KNNSearchText(textembeds, ["https://www.outkick.com/wp-content/uploads/Nowell-Thomas.jpg"])
+cc.KNNSearchText(textembeds, ["https://upload.wikimedia.org/wikipedia/commons/thumb/6/68/Orange_tabby_cat_sitting_on_fallen_leaves-Hisashi-01A.jpg/800px-Orange_tabby_cat_sitting_on_fallen_leaves-Hisashi-01A.jpg"])
 ```
 Note the arguments taken by the KNN functions are the return values of the previous external functions. <br>
 
 The output of KNNSearchImage will be 5 images with the closest euclidean distance in ascending order; that is, the closest related image being output first. <br>
 The output of KNNSearchText will be a caption of the image based on the lowest euclidean distance between your list of input captions and the input image.
 
 ## Requirements
```

### Comparing `clipcraft-1.1/README.md` & `clipcraft-1.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -28,25 +28,25 @@
 
 **KNNSearchText(text_embeddings, image_urls)** This function will find the most similar caption to a given image. It is designed for use by providing the list returned from createTextEmbeddings. text_embeddings should be the return value of createTextEmbeddings, while image_urls should be a single URL or a list of URLs. 
 
 ## Example
 ```python
 import clipcraft as cc
 
-file_urls = ["first_100_rows.json.gz"]
+file_urls = "https://upload.wikimedia.org/wikipedia/commons/thumb/6/68/Orange_tabby_cat_sitting_on_fallen_leaves-Hisashi-01A.jpg/800px-Orange_tabby_cat_sitting_on_fallen_leaves-Hisashi-01A.jpg"
 
 image_embeds = cc.createImageEmbeddings(file_urls)
 
-text_embed_list = ["a man in a green jacket and a basketball player in a white shirt",  "Grandma with makeup", "Football player"]
+text_embed_list = ["a picture of a cat"]
 
 text_embeds = cc.createTextEmbeddings(text_embed_list)
 
 cc.KNNSearchImage(text_embeds, image_embeds)
 
-cc.KNNSearchText(textembeds, ["https://www.outkick.com/wp-content/uploads/Nowell-Thomas.jpg"])
+cc.KNNSearchText(textembeds, ["https://upload.wikimedia.org/wikipedia/commons/thumb/6/68/Orange_tabby_cat_sitting_on_fallen_leaves-Hisashi-01A.jpg/800px-Orange_tabby_cat_sitting_on_fallen_leaves-Hisashi-01A.jpg"])
 ```
 Note the arguments taken by the KNN functions are the return values of the previous external functions. <br>
 
 The output of KNNSearchImage will be 5 images with the closest euclidean distance in ascending order; that is, the closest related image being output first. <br>
 The output of KNNSearchText will be a caption of the image based on the lowest euclidean distance between your list of input captions and the input image.
 
 ## Requirements
```

### Comparing `clipcraft-1.1/clipcraft/create_embeddings.py` & `clipcraft-1.2/clipcraft/create_embeddings.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from transformers import CLIPProcessor, CLIPModel, CLIPTokenizer
 from PIL import Image
 import numpy as np
 import requests
 import json
 import gzip
 import os
+from io import BytesIO
 
 # Helper function to extract the URLs from a json file
 def _extractURLFromJSON(data, urls):
     # Determining if the provided data is in list format
     if isinstance(data, list):
         # Looping through the items in the list
         for item in data:
@@ -119,29 +120,32 @@
             break
         else:
             print("Invalid output type. Expected 'list' or 'file'. Please try again")
     
     embeddings = []
     if isinstance(input_urls, str):
     # Read the file and process its contents
-        url_list = _extractURLFromFile(input_urls)
-        embeddings.extend(_imageEmbeddings(url_list))
+        if input_urls.startswith("http"):
+            embeddings.extend(_imageEmbeddings([input_urls]))
+        else:
+            url_list = _extractURLFromFile(input_urls)
+            embeddings.extend(_imageEmbeddings(url_list))
                              
     if isinstance(input_urls, list):
         embeddings = []
         # Multiple files provided
         for url in input_urls:
-            if isinstance(url, str):
-                # Process a file
-                url_list = _extractURLFromFile(url)
-                embeddings = _imageEmbeddings(url_list)
-            elif isinstance(url, str) and url.startswith('http'):
-                # Process a URL
-                for i in url_list:
-                    embeddings=((url, _imageEmbeddings(url)))
+        if isinstance(url, str) and url.startswith('http'):
+            # Process a URL
+            embeddings.extend(_imageEmbeddings([url]))
+        elif isinstance(url, str):
+            # Process a file
+            url_list = _extractURLFromFile(url)
+            embeddings.extend(_imageEmbeddings(url_list))
+
 
     print("All image embeddings finished.")
     if output_type == "list":
         return embeddings
     elif output_type == "file":
         _writeEmbeddingsToFile("image",embeddings)
         return "Embeddings successfully written to file."
```

### Comparing `clipcraft-1.1/clipcraft/knn_search.py` & `clipcraft-1.2/clipcraft/knn_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,16 @@
 
     # Loop through our 2d array to output the original text, as well as the image url and the image itself
     for text_embedding, nearest_images in result:
         print("Original Text:", text_embedding)
         for image, image_url in nearest_images:
             print("Image URL:", image_url)
             display(image)
-        print('5 most similar images displayed for text input. \n')
+        print('Most similar image(s) displayed for text input. \n')
+ 
         
 # User-callable function to display KNN, or most similar text given an image
 def KNNSearchText(text_embeddings, image_urls):
     # Use NumPy stack method to convert the 2d array to 1d with embeddings
     text_embeddings_array = np.stack([embedding for _, embedding in text_embeddings])
     result = []
     # Determine if we have only one image url as input
```

### Comparing `clipcraft-1.1/clipcraft.egg-info/PKG-INFO` & `clipcraft-1.2/clipcraft.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipcraft
-Version: 1.1
+Version: 1.2
 Summary: A package for CLIP-based image and text processing.
 Home-page: https://github.com/mmckenzieORCEN/CLIPCraft
 Author: Morgan McKenzie
 Author-email: morgancmckenziecs@gmail.com
 Description-Content-Type: text/markdown
 
 # CLIPCraft
@@ -37,25 +37,25 @@
 
 **KNNSearchText(text_embeddings, image_urls)** This function will find the most similar caption to a given image. It is designed for use by providing the list returned from createTextEmbeddings. text_embeddings should be the return value of createTextEmbeddings, while image_urls should be a single URL or a list of URLs. 
 
 ## Example
 ```python
 import clipcraft as cc
 
-file_urls = ["first_100_rows.json.gz"]
+file_urls = "https://upload.wikimedia.org/wikipedia/commons/thumb/6/68/Orange_tabby_cat_sitting_on_fallen_leaves-Hisashi-01A.jpg/800px-Orange_tabby_cat_sitting_on_fallen_leaves-Hisashi-01A.jpg"
 
 image_embeds = cc.createImageEmbeddings(file_urls)
 
-text_embed_list = ["a man in a green jacket and a basketball player in a white shirt",  "Grandma with makeup", "Football player"]
+text_embed_list = ["a picture of a cat"]
 
 text_embeds = cc.createTextEmbeddings(text_embed_list)
 
 cc.KNNSearchImage(text_embeds, image_embeds)
 
-cc.KNNSearchText(textembeds, ["https://www.outkick.com/wp-content/uploads/Nowell-Thomas.jpg"])
+cc.KNNSearchText(textembeds, ["https://upload.wikimedia.org/wikipedia/commons/thumb/6/68/Orange_tabby_cat_sitting_on_fallen_leaves-Hisashi-01A.jpg/800px-Orange_tabby_cat_sitting_on_fallen_leaves-Hisashi-01A.jpg"])
 ```
 Note the arguments taken by the KNN functions are the return values of the previous external functions. <br>
 
 The output of KNNSearchImage will be 5 images with the closest euclidean distance in ascending order; that is, the closest related image being output first. <br>
 The output of KNNSearchText will be a caption of the image based on the lowest euclidean distance between your list of input captions and the input image.
 
 ## Requirements
```

### Comparing `clipcraft-1.1/setup.py` & `clipcraft-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', 'r', encoding='utf-8') as readme_file:
     long_description = readme_file.read()
 
 setup(
     name="clipcraft",
-    version="1.1",
+    version="1.2",
     description="A package for CLIP-based image and text processing.",
     author='Morgan McKenzie',
     author_email='morgancmckenziecs@gmail.com',
     packages=["clipcraft"],
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/mmckenzieORCEN/CLIPCraft',
```

