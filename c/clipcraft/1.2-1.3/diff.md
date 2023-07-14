# Comparing `tmp/clipcraft-1.2.tar.gz` & `tmp/clipcraft-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipcraft-1.2.tar", last modified: Fri Jul 14 16:43:46 2023, max compression
+gzip compressed data, was "clipcraft-1.3.tar", last modified: Fri Jul 14 17:01:26 2023, max compression
```

## Comparing `clipcraft-1.2.tar` & `clipcraft-1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 16:43:46.013834 clipcraft-1.2/
--rw-rw-rw-   0        0        0     3766 2023-07-14 16:43:46.013834 clipcraft-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3427 2023-07-14 16:29:27.000000 clipcraft-1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 16:43:46.002434 clipcraft-1.2/clipcraft/
--rw-rw-rw-   0        0        0      128 2023-07-14 14:35:14.000000 clipcraft-1.2/clipcraft/__init__.py
--rw-rw-rw-   0        0        0     8256 2023-07-14 16:25:37.000000 clipcraft-1.2/clipcraft/create_embeddings.py
--rw-rw-rw-   0        0        0     3535 2023-07-14 16:15:59.000000 clipcraft-1.2/clipcraft/knn_search.py
-drwxrwxrwx   0        0        0        0 2023-07-14 16:43:46.013834 clipcraft-1.2/clipcraft.egg-info/
--rw-rw-rw-   0        0        0     3766 2023-07-14 16:43:45.000000 clipcraft-1.2/clipcraft.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-07-14 16:43:45.000000 clipcraft-1.2/clipcraft.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 16:43:45.000000 clipcraft-1.2/clipcraft.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-07-14 16:43:45.000000 clipcraft-1.2/clipcraft.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-14 16:43:45.000000 clipcraft-1.2/clipcraft.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 16:43:46.013834 clipcraft-1.2/setup.cfg
--rw-rw-rw-   0        0        0      640 2023-07-14 16:30:26.000000 clipcraft-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 17:01:26.328065 clipcraft-1.3/
+-rw-rw-rw-   0        0        0     3766 2023-07-14 17:01:26.328065 clipcraft-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3427 2023-07-14 16:29:27.000000 clipcraft-1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 17:01:26.306041 clipcraft-1.3/clipcraft/
+-rw-rw-rw-   0        0        0      128 2023-07-14 14:35:14.000000 clipcraft-1.3/clipcraft/__init__.py
+-rw-rw-rw-   0        0        0     8285 2023-07-14 16:57:17.000000 clipcraft-1.3/clipcraft/create_embeddings.py
+-rw-rw-rw-   0        0        0     3535 2023-07-14 16:57:50.000000 clipcraft-1.3/clipcraft/knn_search.py
+drwxrwxrwx   0        0        0        0 2023-07-14 17:01:26.323558 clipcraft-1.3/clipcraft.egg-info/
+-rw-rw-rw-   0        0        0     3766 2023-07-14 17:01:26.000000 clipcraft-1.3/clipcraft.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-07-14 17:01:26.000000 clipcraft-1.3/clipcraft.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 17:01:26.000000 clipcraft-1.3/clipcraft.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-07-14 17:01:26.000000 clipcraft-1.3/clipcraft.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-14 17:01:26.000000 clipcraft-1.3/clipcraft.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 17:01:26.328065 clipcraft-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      640 2023-07-14 17:01:10.000000 clipcraft-1.3/setup.py
```

### Comparing `clipcraft-1.2/PKG-INFO` & `clipcraft-1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipcraft
-Version: 1.2
+Version: 1.3
 Summary: A package for CLIP-based image and text processing.
 Home-page: https://github.com/mmckenzieORCEN/CLIPCraft
 Author: Morgan McKenzie
 Author-email: morgancmckenziecs@gmail.com
 Description-Content-Type: text/markdown
 
 # CLIPCraft
```

### Comparing `clipcraft-1.2/README.md` & `clipcraft-1.3/README.md`

 * *Files identical despite different names*

### Comparing `clipcraft-1.2/clipcraft/create_embeddings.py` & `clipcraft-1.3/clipcraft/create_embeddings.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         with gzip.open("CLIP_text_embeddings.json.gz", "wt") as datafile:
             for i in range(len(input_text_embeddings)):
                 new_row = {
                     'original_text': input_text_embeddings[i][0], 
                     'text_embedding': input_text_embeddings[i][1],
                 }
                 datafile.write(json.dumps(new_row) + '\n')
-                j + 1
+                j += 1
         print("Successfully dumped #" + str(i) + " embeddings to file." + '\n')
 
 # Internal function that extracts URL from user-input file
 def _extractURLFromFile(input_urls):
     if isinstance(input_urls, str):  # Check if user input is a string
         input_urls = [input_urls]  # Convert it to a list for processing
 
@@ -130,21 +130,21 @@
             url_list = _extractURLFromFile(input_urls)
             embeddings.extend(_imageEmbeddings(url_list))
                              
     if isinstance(input_urls, list):
         embeddings = []
         # Multiple files provided
         for url in input_urls:
-        if isinstance(url, str) and url.startswith('http'):
-            # Process a URL
-            embeddings.extend(_imageEmbeddings([url]))
-        elif isinstance(url, str):
-            # Process a file
-            url_list = _extractURLFromFile(url)
-            embeddings.extend(_imageEmbeddings(url_list))
+            if isinstance(url, str) and url.startswith('http'):
+                # Process a URL
+                embeddings.extend(_imageEmbeddings([url]))
+            elif isinstance(url, str):
+                # Process a file
+                url_list = _extractURLFromFile(url)
+                embeddings.extend(_imageEmbeddings(url_list))
 
 
     print("All image embeddings finished.")
     if output_type == "list":
         return embeddings
     elif output_type == "file":
         _writeEmbeddingsToFile("image",embeddings)
```

### Comparing `clipcraft-1.2/clipcraft/knn_search.py` & `clipcraft-1.3/clipcraft/knn_search.py`

 * *Files identical despite different names*

### Comparing `clipcraft-1.2/clipcraft.egg-info/PKG-INFO` & `clipcraft-1.3/clipcraft.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipcraft
-Version: 1.2
+Version: 1.3
 Summary: A package for CLIP-based image and text processing.
 Home-page: https://github.com/mmckenzieORCEN/CLIPCraft
 Author: Morgan McKenzie
 Author-email: morgancmckenziecs@gmail.com
 Description-Content-Type: text/markdown
 
 # CLIPCraft
```

### Comparing `clipcraft-1.2/setup.py` & `clipcraft-1.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', 'r', encoding='utf-8') as readme_file:
     long_description = readme_file.read()
 
 setup(
     name="clipcraft",
-    version="1.2",
+    version="1.3",
     description="A package for CLIP-based image and text processing.",
     author='Morgan McKenzie',
     author_email='morgancmckenziecs@gmail.com',
     packages=["clipcraft"],
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/mmckenzieORCEN/CLIPCraft',
```

