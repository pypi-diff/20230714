# Comparing `tmp/agentmemory-0.2.1.tar.gz` & `tmp/agentmemory-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentmemory-0.2.1.tar", last modified: Fri Jul 14 01:08:25 2023, max compression
+gzip compressed data, was "agentmemory-0.2.2.tar", last modified: Fri Jul 14 01:27:19 2023, max compression
```

## Comparing `agentmemory-0.2.1.tar` & `agentmemory-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-14 01:08:25.858259 agentmemory-0.2.1/
--rw-r--r--   0 shawwalters   (501) staff       (20)     1126 2023-07-06 21:19:09.000000 agentmemory-0.2.1/LICENSE
--rw-r--r--   0 shawwalters   (501) staff       (20)    11763 2023-07-14 01:08:25.857976 agentmemory-0.2.1/PKG-INFO
--rw-r--r--   0 shawwalters   (501) staff       (20)    11205 2023-07-13 02:18:43.000000 agentmemory-0.2.1/README.md
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-14 01:08:25.856226 agentmemory-0.2.1/agentmemory/
--rw-r--r--   0 shawwalters   (501) staff       (20)     1104 2023-07-14 01:08:21.000000 agentmemory-0.2.1/agentmemory/__init__.py
--rw-r--r--   0 shawwalters   (501) staff       (20)    24896 2023-07-14 01:06:04.000000 agentmemory-0.2.1/agentmemory/main.py
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-14 01:08:25.857689 agentmemory-0.2.1/agentmemory.egg-info/
--rw-r--r--   0 shawwalters   (501) staff       (20)    11763 2023-07-14 01:08:25.000000 agentmemory-0.2.1/agentmemory.egg-info/PKG-INFO
--rw-r--r--   0 shawwalters   (501) staff       (20)      244 2023-07-14 01:08:25.000000 agentmemory-0.2.1/agentmemory.egg-info/SOURCES.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)        1 2023-07-14 01:08:25.000000 agentmemory-0.2.1/agentmemory.egg-info/dependency_links.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)        9 2023-07-14 01:08:25.000000 agentmemory-0.2.1/agentmemory.egg-info/requires.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       12 2023-07-14 01:08:25.000000 agentmemory-0.2.1/agentmemory.egg-info/top_level.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       38 2023-07-14 01:08:25.858346 agentmemory-0.2.1/setup.cfg
--rw-r--r--   0 shawwalters   (501) staff       (20)     1257 2023-07-14 01:08:21.000000 agentmemory-0.2.1/setup.py
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-14 01:27:19.917572 agentmemory-0.2.2/
+-rw-r--r--   0 shawwalters   (501) staff       (20)     1126 2023-07-06 21:19:09.000000 agentmemory-0.2.2/LICENSE
+-rw-r--r--   0 shawwalters   (501) staff       (20)    11763 2023-07-14 01:27:19.916925 agentmemory-0.2.2/PKG-INFO
+-rw-r--r--   0 shawwalters   (501) staff       (20)    11205 2023-07-14 01:24:31.000000 agentmemory-0.2.2/README.md
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-14 01:27:19.915488 agentmemory-0.2.2/agentmemory/
+-rw-r--r--   0 shawwalters   (501) staff       (20)     1104 2023-07-14 01:27:15.000000 agentmemory-0.2.2/agentmemory/__init__.py
+-rw-r--r--   0 shawwalters   (501) staff       (20)    24901 2023-07-14 01:26:35.000000 agentmemory-0.2.2/agentmemory/main.py
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-14 01:27:19.916649 agentmemory-0.2.2/agentmemory.egg-info/
+-rw-r--r--   0 shawwalters   (501) staff       (20)    11763 2023-07-14 01:27:19.000000 agentmemory-0.2.2/agentmemory.egg-info/PKG-INFO
+-rw-r--r--   0 shawwalters   (501) staff       (20)      244 2023-07-14 01:27:19.000000 agentmemory-0.2.2/agentmemory.egg-info/SOURCES.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)        1 2023-07-14 01:27:19.000000 agentmemory-0.2.2/agentmemory.egg-info/dependency_links.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)        9 2023-07-14 01:27:19.000000 agentmemory-0.2.2/agentmemory.egg-info/requires.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)       12 2023-07-14 01:27:19.000000 agentmemory-0.2.2/agentmemory.egg-info/top_level.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)       38 2023-07-14 01:27:19.917641 agentmemory-0.2.2/setup.cfg
+-rw-r--r--   0 shawwalters   (501) staff       (20)     1257 2023-07-14 01:27:15.000000 agentmemory-0.2.2/setup.py
```

### Comparing `agentmemory-0.2.1/LICENSE` & `agentmemory-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `agentmemory-0.2.1/PKG-INFO` & `agentmemory-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentmemory
-Version: 0.2.1
+Version: 0.2.2
 Summary: Easy-to-use agent memory, powered by chromadb
 Home-page: https://github.com/lalalune/agentmemory
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `agentmemory-0.2.1/README.md` & `agentmemory-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `agentmemory-0.2.1/agentmemory/__init__.py` & `agentmemory-0.2.2/agentmemory/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 agentmemory
 
 Simple agent memory, powered by chromadb
 """
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 __author__ = "Moon (https://github.com/lalalune)"
 __credits__ = "https://github.com/lalalune/agentmemory and https://www.trychroma.com/"
 
 from .main import (
     create_memory,
     get_memories,
     search_memory,
```

### Comparing `agentmemory-0.2.1/agentmemory/main.py` & `agentmemory-0.2.2/agentmemory/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     if id is None:
         id = str(memories.count())
         # pad the id with zeros to make it 10 digits long
         id = id.zfill(10)
 
     # insert the document into the collection
     memories.upsert(
-        ids=[id],
+        ids=[str(id)],
         documents=[text],
         metadatas=[metadata],
         embeddings=[embedding] if embedding is not None else None,
     )
 
     if persist:
         persist_memory()
```

### Comparing `agentmemory-0.2.1/agentmemory.egg-info/PKG-INFO` & `agentmemory-0.2.2/agentmemory.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentmemory
-Version: 0.2.1
+Version: 0.2.2
 Summary: Easy-to-use agent memory, powered by chromadb
 Home-page: https://github.com/lalalune/agentmemory
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `agentmemory-0.2.1/setup.py` & `agentmemory-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = [line for line in long_description if not '<img' in line]
     # now join all the lines back together
     long_description = '\n'.join(long_description)
     
 
 setup(
     name='agentmemory',
-    version='0.2.1',
+    version='0.2.2',
     description='Easy-to-use agent memory, powered by chromadb',
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url='https://github.com/lalalune/agentmemory',
     author='Moon',
     author_email='shawmakesmagic@gmail.com',
     license='MIT',
```

