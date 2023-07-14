# Comparing `tmp/clipcraft-1.4.1.tar.gz` & `tmp/clipcraft-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipcraft-1.4.1.tar", last modified: Fri Jul 14 17:27:30 2023, max compression
+gzip compressed data, was "clipcraft-1.4.2.tar", last modified: Fri Jul 14 17:34:17 2023, max compression
```

## Comparing `clipcraft-1.4.1.tar` & `clipcraft-1.4.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 17:27:30.098257 clipcraft-1.4.1/
--rw-rw-rw-   0        0        0     3769 2023-07-14 17:27:30.098257 clipcraft-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     3428 2023-07-14 17:15:39.000000 clipcraft-1.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 17:27:30.081120 clipcraft-1.4.1/clipcraft/
--rw-rw-rw-   0        0        0      128 2023-07-14 14:35:14.000000 clipcraft-1.4.1/clipcraft/__init__.py
--rw-rw-rw-   0        0        0     8285 2023-07-14 17:25:01.000000 clipcraft-1.4.1/clipcraft/create_embeddings.py
--rw-rw-rw-   0        0        0     3583 2023-07-14 17:25:03.000000 clipcraft-1.4.1/clipcraft/knn_search.py
-drwxrwxrwx   0        0        0        0 2023-07-14 17:27:30.098257 clipcraft-1.4.1/clipcraft.egg-info/
--rw-rw-rw-   0        0        0     3769 2023-07-14 17:27:29.000000 clipcraft-1.4.1/clipcraft.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-07-14 17:27:29.000000 clipcraft-1.4.1/clipcraft.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 17:27:29.000000 clipcraft-1.4.1/clipcraft.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-07-14 17:27:29.000000 clipcraft-1.4.1/clipcraft.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-14 17:27:29.000000 clipcraft-1.4.1/clipcraft.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 17:27:30.098257 clipcraft-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0      642 2023-07-14 17:27:19.000000 clipcraft-1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 17:34:17.224104 clipcraft-1.4.2/
+-rw-rw-rw-   0        0        0     3769 2023-07-14 17:34:17.224104 clipcraft-1.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3428 2023-07-14 17:15:39.000000 clipcraft-1.4.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 17:34:17.208701 clipcraft-1.4.2/clipcraft/
+-rw-rw-rw-   0        0        0      128 2023-07-14 14:35:14.000000 clipcraft-1.4.2/clipcraft/__init__.py
+-rw-rw-rw-   0        0        0     8285 2023-07-14 17:33:46.000000 clipcraft-1.4.2/clipcraft/create_embeddings.py
+-rw-rw-rw-   0        0        0     5177 2023-07-14 17:33:43.000000 clipcraft-1.4.2/clipcraft/knn_search.py
+drwxrwxrwx   0        0        0        0 2023-07-14 17:34:17.224104 clipcraft-1.4.2/clipcraft.egg-info/
+-rw-rw-rw-   0        0        0     3769 2023-07-14 17:34:17.000000 clipcraft-1.4.2/clipcraft.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-07-14 17:34:17.000000 clipcraft-1.4.2/clipcraft.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 17:34:17.000000 clipcraft-1.4.2/clipcraft.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-07-14 17:34:17.000000 clipcraft-1.4.2/clipcraft.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-14 17:34:17.000000 clipcraft-1.4.2/clipcraft.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 17:34:17.224104 clipcraft-1.4.2/setup.cfg
+-rw-rw-rw-   0        0        0      642 2023-07-14 17:34:13.000000 clipcraft-1.4.2/setup.py
```

### Comparing `clipcraft-1.4.1/PKG-INFO` & `clipcraft-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipcraft
-Version: 1.4.1
+Version: 1.4.2
 Summary: A package for CLIP-based image and text processing.
 Home-page: https://github.com/mmckenzieORCEN/CLIPCraft
 Author: Morgan McKenzie
 Author-email: morgancmckenziecs@gmail.com
 Description-Content-Type: text/markdown
 
 # CLIPCraft
```

### Comparing `clipcraft-1.4.1/README.md` & `clipcraft-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `clipcraft-1.4.1/clipcraft/create_embeddings.py` & `clipcraft-1.4.2/clipcraft/create_embeddings.py`

 * *Files identical despite different names*

### Comparing `clipcraft-1.4.1/clipcraft.egg-info/PKG-INFO` & `clipcraft-1.4.2/clipcraft.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipcraft
-Version: 1.4.1
+Version: 1.4.2
 Summary: A package for CLIP-based image and text processing.
 Home-page: https://github.com/mmckenzieORCEN/CLIPCraft
 Author: Morgan McKenzie
 Author-email: morgancmckenziecs@gmail.com
 Description-Content-Type: text/markdown
 
 # CLIPCraft
```

### Comparing `clipcraft-1.4.1/setup.py` & `clipcraft-1.4.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', 'r', encoding='utf-8') as readme_file:
     long_description = readme_file.read()
 
 setup(
     name="clipcraft",
-    version="1.4.1",
+    version="1.4.2",
     description="A package for CLIP-based image and text processing.",
     author='Morgan McKenzie',
     author_email='morgancmckenziecs@gmail.com',
     packages=["clipcraft"],
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/mmckenzieORCEN/CLIPCraft',
```

