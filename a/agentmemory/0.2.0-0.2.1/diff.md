# Comparing `tmp/agentmemory-0.2.0.tar.gz` & `tmp/agentmemory-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentmemory-0.2.0.tar", last modified: Thu Jul 13 02:27:52 2023, max compression
+gzip compressed data, was "agentmemory-0.2.1.tar", last modified: Fri Jul 14 01:08:25 2023, max compression
```

## Comparing `agentmemory-0.2.0.tar` & `agentmemory-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-13 02:27:52.092797 agentmemory-0.2.0/
--rw-r--r--   0 shawwalters   (501) staff       (20)     1126 2023-07-06 21:19:09.000000 agentmemory-0.2.0/LICENSE
--rw-r--r--   0 shawwalters   (501) staff       (20)    11763 2023-07-13 02:27:52.092539 agentmemory-0.2.0/PKG-INFO
--rw-r--r--   0 shawwalters   (501) staff       (20)    11205 2023-07-13 02:18:43.000000 agentmemory-0.2.0/README.md
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-13 02:27:52.091037 agentmemory-0.2.0/agentmemory/
--rw-r--r--   0 shawwalters   (501) staff       (20)     1103 2023-07-13 02:27:48.000000 agentmemory-0.2.0/agentmemory/__init__.py
--rw-r--r--   0 shawwalters   (501) staff       (20)    24183 2023-07-13 02:25:22.000000 agentmemory-0.2.0/agentmemory/main.py
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-13 02:27:52.092299 agentmemory-0.2.0/agentmemory.egg-info/
--rw-r--r--   0 shawwalters   (501) staff       (20)    11763 2023-07-13 02:27:52.000000 agentmemory-0.2.0/agentmemory.egg-info/PKG-INFO
--rw-r--r--   0 shawwalters   (501) staff       (20)      244 2023-07-13 02:27:52.000000 agentmemory-0.2.0/agentmemory.egg-info/SOURCES.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)        1 2023-07-13 02:27:52.000000 agentmemory-0.2.0/agentmemory.egg-info/dependency_links.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)        9 2023-07-13 02:27:52.000000 agentmemory-0.2.0/agentmemory.egg-info/requires.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       12 2023-07-13 02:27:52.000000 agentmemory-0.2.0/agentmemory.egg-info/top_level.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       38 2023-07-13 02:27:52.092871 agentmemory-0.2.0/setup.cfg
--rw-r--r--   0 shawwalters   (501) staff       (20)     1257 2023-07-13 02:27:48.000000 agentmemory-0.2.0/setup.py
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-14 01:08:25.858259 agentmemory-0.2.1/
+-rw-r--r--   0 shawwalters   (501) staff       (20)     1126 2023-07-06 21:19:09.000000 agentmemory-0.2.1/LICENSE
+-rw-r--r--   0 shawwalters   (501) staff       (20)    11763 2023-07-14 01:08:25.857976 agentmemory-0.2.1/PKG-INFO
+-rw-r--r--   0 shawwalters   (501) staff       (20)    11205 2023-07-13 02:18:43.000000 agentmemory-0.2.1/README.md
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-14 01:08:25.856226 agentmemory-0.2.1/agentmemory/
+-rw-r--r--   0 shawwalters   (501) staff       (20)     1104 2023-07-14 01:08:21.000000 agentmemory-0.2.1/agentmemory/__init__.py
+-rw-r--r--   0 shawwalters   (501) staff       (20)    24896 2023-07-14 01:06:04.000000 agentmemory-0.2.1/agentmemory/main.py
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-14 01:08:25.857689 agentmemory-0.2.1/agentmemory.egg-info/
+-rw-r--r--   0 shawwalters   (501) staff       (20)    11763 2023-07-14 01:08:25.000000 agentmemory-0.2.1/agentmemory.egg-info/PKG-INFO
+-rw-r--r--   0 shawwalters   (501) staff       (20)      244 2023-07-14 01:08:25.000000 agentmemory-0.2.1/agentmemory.egg-info/SOURCES.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)        1 2023-07-14 01:08:25.000000 agentmemory-0.2.1/agentmemory.egg-info/dependency_links.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)        9 2023-07-14 01:08:25.000000 agentmemory-0.2.1/agentmemory.egg-info/requires.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)       12 2023-07-14 01:08:25.000000 agentmemory-0.2.1/agentmemory.egg-info/top_level.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)       38 2023-07-14 01:08:25.858346 agentmemory-0.2.1/setup.cfg
+-rw-r--r--   0 shawwalters   (501) staff       (20)     1257 2023-07-14 01:08:21.000000 agentmemory-0.2.1/setup.py
```

### Comparing `agentmemory-0.2.0/LICENSE` & `agentmemory-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `agentmemory-0.2.0/PKG-INFO` & `agentmemory-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentmemory
-Version: 0.2.0
+Version: 0.2.1
 Summary: Easy-to-use agent memory, powered by chromadb
 Home-page: https://github.com/lalalune/agentmemory
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `agentmemory-0.2.0/README.md` & `agentmemory-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `agentmemory-0.2.0/agentmemory/__init__.py` & `agentmemory-0.2.1/agentmemory/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 agentmemory
 
 Simple agent memory, powered by chromadb
 """
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 __author__ = "Moon (https://github.com/lalalune)"
 __credits__ = "https://github.com/lalalune/agentmemory and https://www.trychroma.com/"
 
 from .main import (
     create_memory,
     get_memories,
     search_memory,
@@ -22,16 +22,15 @@
     save_memory,
     get_chroma_client,
     chroma_collection_to_list,
     list_to_chroma_collection,
     export_memory_to_json,
     export_memory_to_file,
     import_json_to_memory,
-    import_file_to_memory
-
+    import_file_to_memory,
 )
 
 __all__ = [
     "create_memory",
     "get_memories",
     "search_memory",
     "get_memory",
@@ -44,9 +43,9 @@
     "save_memory",
     "get_chroma_client",
     "chroma_collection_to_list",
     "list_to_chroma_collection",
     "export_memory_to_json",
     "export_memory_to_file",
     "import_json_to_memory",
-    "import_file_to_memory"
+    "import_file_to_memory",
 ]
```

### Comparing `agentmemory-0.2.0/agentmemory/main.py` & `agentmemory-0.2.1/agentmemory/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,16 @@
     # add timestamps to metadata
     metadata["created_at"] = datetime.datetime.now().timestamp()
     metadata["updated_at"] = datetime.datetime.now().timestamp()
 
     # if no id is provided, generate one based on count of documents in collection
     if id is None:
         id = str(memories.count())
+        # pad the id with zeros to make it 10 digits long
+        id = id.zfill(10)
 
     # insert the document into the collection
     memories.upsert(
         ids=[id],
         documents=[text],
         metadatas=[metadata],
         embeddings=[embedding] if embedding is not None else None,
@@ -93,14 +95,17 @@
     # check if contains_text is provided and format it for the query
     if contains_text is not None:
         contains_text = {"$contains": contains_text}
 
     # get or create the collection
     memories = client.get_or_create_collection(category)
 
+    # min n_results to prevent searching for more elements than are available
+    n_results = min(n_results, memories.count())
+
     # get the types to include
     include_types = get_include_types(include_embeddings, include_distances)
 
     # perform the query and get the response
     query = memories.query(
         query_texts=[search_text],
         where=filter_metadata,
@@ -153,14 +158,20 @@
     memory = memories.get(ids=[str(id)], limit=1, include=include_types)
 
     # Convert the collection to list format
     memory = chroma_collection_to_list(memory)
 
     debug_log(f"Got memory {id} from category {category}", memory)
 
+    if len(memory) == 0:
+        debug_log(
+            f"WARNING: Tried to get memory {id} from category {category} but it does not exist"
+        )
+        return None
+
     # Return the first (and only) memory in the list
     return memory[0]
 
 
 def get_memories(
     category,
     sort_order="desc",
@@ -186,14 +197,17 @@
         >>> get_memories("books", sort_order="asc", n_results=10)
     """
     check_client_initialized()  # client is lazy loaded, so make sure it is is initialized
 
     # Get or create the collection for the given category
     memories = client.get_or_create_collection(category)
 
+    # min n_results to prevent searching for more elements than are available
+    n_results = min(n_results, memories.count())
+
     # Get the types to include based on the function parameters
     include_types = get_include_types(include_embeddings, False)
 
     where_document = None
 
     if contains_text is not None:
         where_document = {"$contains": contains_text}
@@ -281,14 +295,17 @@
     """
 
     check_client_initialized()  # client is lazy loaded, so make sure it is is initialized
 
     # Get or create the collection for the given category
     memories = client.get_or_create_collection(category)
 
+    if memory_exists(category, id) is False:
+        debug_log(f"WARNING: Tried could not delete memory {id} in category {category}")
+        return
     # Delete the memory
     memories.delete(ids=[str(id)])
 
     if persist:
         persist_memory()
 
     debug_log(f"Deleted memory {id} in category {category}")
@@ -336,23 +353,27 @@
         category (str): The category to delete.
         persist (bool, optional): Whether to persist the changes to disk. Defaults to True.
 
     Example:
         >>> wipe_category("books")
     """
 
-    check_client_initialized()  # client is lazy loaded, so make sure it is is initialized
-
-    # Delete the entire category
-    client.delete_collection(category)
+    collection = None
 
-    if persist:
-        persist_memory()
+    try:
+        collection = client.get_collection(category)  # Check if the category exists
+    except:
+        pass
+
+    if collection is not None:
+        # Delete the entire category
+        client.delete_collection(category)
 
-    debug_log(f"Wiped category {category}")
+        if persist:
+            client.persist()
 
 
 def count_memories(category):
     """
     Count the number of memories in a given category.
 
     Arguments:
@@ -497,15 +518,15 @@
 
     collections_dict = {}
 
     # Iterate over all collections
     for collection in collections:
         print(collection)
         collection_name = collection.name
-        print('collection_name')
+        print("collection_name")
         print(collection_name)
 
         collections_dict[collection_name] = []
 
         # Get all memories from the current collection
         memories = get_memories(collection_name, include_embeddings=include_embeddings)
         for memory in memories:
```

### Comparing `agentmemory-0.2.0/agentmemory.egg-info/PKG-INFO` & `agentmemory-0.2.1/agentmemory.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentmemory
-Version: 0.2.0
+Version: 0.2.1
 Summary: Easy-to-use agent memory, powered by chromadb
 Home-page: https://github.com/lalalune/agentmemory
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `agentmemory-0.2.0/setup.py` & `agentmemory-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = [line for line in long_description if not '<img' in line]
     # now join all the lines back together
     long_description = '\n'.join(long_description)
     
 
 setup(
     name='agentmemory',
-    version='0.2.0',
+    version='0.2.1',
     description='Easy-to-use agent memory, powered by chromadb',
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url='https://github.com/lalalune/agentmemory',
     author='Moon',
     author_email='shawmakesmagic@gmail.com',
     license='MIT',
```

