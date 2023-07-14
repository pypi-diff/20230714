# Comparing `tmp/clipcraft-1.4.2.tar.gz` & `tmp/clipcraft-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipcraft-1.4.2.tar", last modified: Fri Jul 14 17:34:17 2023, max compression
+gzip compressed data, was "clipcraft-1.4.3.tar", last modified: Fri Jul 14 17:40:12 2023, max compression
```

## Comparing `clipcraft-1.4.2.tar` & `clipcraft-1.4.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 17:34:17.224104 clipcraft-1.4.2/
--rw-rw-rw-   0        0        0     3769 2023-07-14 17:34:17.224104 clipcraft-1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     3428 2023-07-14 17:15:39.000000 clipcraft-1.4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 17:34:17.208701 clipcraft-1.4.2/clipcraft/
--rw-rw-rw-   0        0        0      128 2023-07-14 14:35:14.000000 clipcraft-1.4.2/clipcraft/__init__.py
--rw-rw-rw-   0        0        0     8285 2023-07-14 17:33:46.000000 clipcraft-1.4.2/clipcraft/create_embeddings.py
--rw-rw-rw-   0        0        0     5177 2023-07-14 17:33:43.000000 clipcraft-1.4.2/clipcraft/knn_search.py
-drwxrwxrwx   0        0        0        0 2023-07-14 17:34:17.224104 clipcraft-1.4.2/clipcraft.egg-info/
--rw-rw-rw-   0        0        0     3769 2023-07-14 17:34:17.000000 clipcraft-1.4.2/clipcraft.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-07-14 17:34:17.000000 clipcraft-1.4.2/clipcraft.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 17:34:17.000000 clipcraft-1.4.2/clipcraft.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-07-14 17:34:17.000000 clipcraft-1.4.2/clipcraft.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-14 17:34:17.000000 clipcraft-1.4.2/clipcraft.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 17:34:17.224104 clipcraft-1.4.2/setup.cfg
--rw-rw-rw-   0        0        0      642 2023-07-14 17:34:13.000000 clipcraft-1.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 17:40:12.278205 clipcraft-1.4.3/
+-rw-rw-rw-   0        0        0     3769 2023-07-14 17:40:12.274057 clipcraft-1.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3428 2023-07-14 17:15:39.000000 clipcraft-1.4.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 17:40:12.260294 clipcraft-1.4.3/clipcraft/
+-rw-rw-rw-   0        0        0      128 2023-07-14 14:35:14.000000 clipcraft-1.4.3/clipcraft/__init__.py
+-rw-rw-rw-   0        0        0     8334 2023-07-14 17:39:39.000000 clipcraft-1.4.3/clipcraft/create_embeddings.py
+-rw-rw-rw-   0        0        0     5177 2023-07-14 17:39:42.000000 clipcraft-1.4.3/clipcraft/knn_search.py
+drwxrwxrwx   0        0        0        0 2023-07-14 17:40:12.274057 clipcraft-1.4.3/clipcraft.egg-info/
+-rw-rw-rw-   0        0        0     3769 2023-07-14 17:40:12.000000 clipcraft-1.4.3/clipcraft.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-07-14 17:40:12.000000 clipcraft-1.4.3/clipcraft.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 17:40:12.000000 clipcraft-1.4.3/clipcraft.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-07-14 17:40:12.000000 clipcraft-1.4.3/clipcraft.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-14 17:40:12.000000 clipcraft-1.4.3/clipcraft.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 17:40:12.278205 clipcraft-1.4.3/setup.cfg
+-rw-rw-rw-   0        0        0      642 2023-07-14 17:40:00.000000 clipcraft-1.4.3/setup.py
```

### Comparing `clipcraft-1.4.2/PKG-INFO` & `clipcraft-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipcraft
-Version: 1.4.2
+Version: 1.4.3
 Summary: A package for CLIP-based image and text processing.
 Home-page: https://github.com/mmckenzieORCEN/CLIPCraft
 Author: Morgan McKenzie
 Author-email: morgancmckenziecs@gmail.com
 Description-Content-Type: text/markdown
 
 # CLIPCraft
```

### Comparing `clipcraft-1.4.2/README.md` & `clipcraft-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `clipcraft-1.4.2/clipcraft/create_embeddings.py` & `clipcraft-1.4.3/clipcraft/create_embeddings.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     _extractURLFromJSON(data, urls)
     return urls
 
 
 # User-callable for users to call to create Image embeddings
 def createImageEmbeddings(input_urls): 
     while True:
-        output_type = input("Enter the desired output type (list or file): ")
+        output_type = input("Enter the desired output type for the image embeddings (list or file): ")
 
         if output_type in ["list", "file"]:
             break
         else:
             print("Invalid output type. Expected 'list' or 'file'. Please try again")
     
     embeddings = []
@@ -152,15 +152,15 @@
     return embeddings
 
 
                 
 # User-callable function to generate text embeddings from CLIP
 def createTextEmbeddings(input_text):
     while True:
-        output_type = input("Enter the desired output type (list or file): ")
+        output_type = input("Enter the desired output type for the text embeddings (list or file): ")
 
         if output_type in ["list", "file"]:
             break
         else:
             print("Invalid output type. Expected 'list' or 'file'. Please try again")
             
     text_embedding_list = []
```

### Comparing `clipcraft-1.4.2/clipcraft/knn_search.py` & `clipcraft-1.4.3/clipcraft/knn_search.py`

 * *Files identical despite different names*

### Comparing `clipcraft-1.4.2/clipcraft.egg-info/PKG-INFO` & `clipcraft-1.4.3/clipcraft.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipcraft
-Version: 1.4.2
+Version: 1.4.3
 Summary: A package for CLIP-based image and text processing.
 Home-page: https://github.com/mmckenzieORCEN/CLIPCraft
 Author: Morgan McKenzie
 Author-email: morgancmckenziecs@gmail.com
 Description-Content-Type: text/markdown
 
 # CLIPCraft
```

### Comparing `clipcraft-1.4.2/setup.py` & `clipcraft-1.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', 'r', encoding='utf-8') as readme_file:
     long_description = readme_file.read()
 
 setup(
     name="clipcraft",
-    version="1.4.2",
+    version="1.4.3",
     description="A package for CLIP-based image and text processing.",
     author='Morgan McKenzie',
     author_email='morgancmckenziecs@gmail.com',
     packages=["clipcraft"],
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/mmckenzieORCEN/CLIPCraft',
```

