# Comparing `tmp/io_collection-0.7.3.tar.gz` & `tmp/io_collection-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "io_collection-0.7.3.tar", max compression
+gzip compressed data, was "io_collection-0.8.0.tar", max compression
```

## Comparing `io_collection-0.7.3.tar` & `io_collection-0.8.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1540 2023-06-29 20:45:22.718034 io_collection-0.7.3/LICENSE
--rw-r--r--   0        0        0     2506 2023-06-29 20:45:22.718034 io_collection-0.7.3/README.md
--rw-r--r--   0        0        0     1915 2023-06-29 20:45:22.722034 io_collection-0.7.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/__init__.py
--rw-r--r--   0        0        0       52 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/__main__.py
--rw-r--r--   0        0        0      389 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/keys/__init__.py
--rw-r--r--   0        0        0      709 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/keys/change_key.py
--rw-r--r--   0        0        0      525 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/keys/check_key.py
--rw-r--r--   0        0        0      726 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/keys/copy_key.py
--rw-r--r--   0        0        0     1365 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/keys/get_keys.py
--rw-r--r--   0        0        0      297 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/keys/make_key.py
--rw-r--r--   0        0        0      461 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/keys/remove_key.py
--rw-r--r--   0        0        0      429 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/load/__init__.py
--rw-r--r--   0        0        0     1028 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/load/load_buffer.py
--rw-r--r--   0        0        0      705 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/load/load_dataframe.py
--rw-r--r--   0        0        0      953 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/load/load_image.py
--rw-r--r--   0        0        0      223 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/load/load_pickle.py
--rw-r--r--   0        0        0      606 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/load/load_tar.py
--rw-r--r--   0        0        0      561 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/load/load_text.py
--rw-r--r--   0        0        0        0 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/py.typed
--rw-r--r--   0        0        0      209 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/quilt/__init__.py
--rw-r--r--   0        0        0      185 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/quilt/load_quilt_package.py
--rw-r--r--   0        0        0      287 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/quilt/save_quilt_item.py
--rw-r--r--   0        0        0      616 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/save/__init__.py
--rw-r--r--   0        0        0      745 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/save/save_buffer.py
--rw-r--r--   0        0        0      920 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/save/save_dataframe.py
--rw-r--r--   0        0        0      889 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/save/save_figure.py
--rw-r--r--   0        0        0      514 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/save/save_gif.py
--rw-r--r--   0        0        0      902 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/save/save_image.py
--rw-r--r--   0        0        0      587 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/save/save_json.py
--rw-r--r--   0        0        0      274 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/save/save_pickle.py
--rw-r--r--   0        0        0     1018 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/save/save_tar.py
--rw-r--r--   0        0        0      712 2023-06-29 20:45:22.726034 io_collection-0.7.3/src/io_collection/save/save_text.py
--rw-r--r--   0        0        0     3320 1970-01-01 00:00:00.000000 io_collection-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1540 2023-07-14 21:37:39.031324 io_collection-0.8.0/LICENSE
+-rw-r--r--   0        0        0     2506 2023-07-14 21:37:39.031324 io_collection-0.8.0/README.md
+-rw-r--r--   0        0        0     1915 2023-07-14 21:37:39.035325 io_collection-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-14 21:37:39.035325 io_collection-0.8.0/src/io_collection/__init__.py
+-rw-r--r--   0        0        0       52 2023-07-14 21:37:39.035325 io_collection-0.8.0/src/io_collection/__main__.py
+-rw-r--r--   0        0        0      389 2023-07-14 21:37:39.035325 io_collection-0.8.0/src/io_collection/keys/__init__.py
+-rw-r--r--   0        0        0      709 2023-07-14 21:37:39.035325 io_collection-0.8.0/src/io_collection/keys/change_key.py
+-rw-r--r--   0        0        0      525 2023-07-14 21:37:39.035325 io_collection-0.8.0/src/io_collection/keys/check_key.py
+-rw-r--r--   0        0        0      726 2023-07-14 21:37:39.035325 io_collection-0.8.0/src/io_collection/keys/copy_key.py
+-rw-r--r--   0        0        0     1365 2023-07-14 21:37:39.035325 io_collection-0.8.0/src/io_collection/keys/get_keys.py
+-rw-r--r--   0        0        0      297 2023-07-14 21:37:39.035325 io_collection-0.8.0/src/io_collection/keys/make_key.py
+-rw-r--r--   0        0        0      461 2023-07-14 21:37:39.035325 io_collection-0.8.0/src/io_collection/keys/remove_key.py
+-rw-r--r--   0        0        0      429 2023-07-14 21:37:39.035325 io_collection-0.8.0/src/io_collection/load/__init__.py
+-rw-r--r--   0        0        0     1028 2023-07-14 21:37:39.035325 io_collection-0.8.0/src/io_collection/load/load_buffer.py
+-rw-r--r--   0        0        0      705 2023-07-14 21:37:39.035325 io_collection-0.8.0/src/io_collection/load/load_dataframe.py
+-rw-r--r--   0        0        0      953 2023-07-14 21:37:39.035325 io_collection-0.8.0/src/io_collection/load/load_image.py
+-rw-r--r--   0        0        0      223 2023-07-14 21:37:39.035325 io_collection-0.8.0/src/io_collection/load/load_pickle.py
+-rw-r--r--   0        0        0      606 2023-07-14 21:37:39.035325 io_collection-0.8.0/src/io_collection/load/load_tar.py
+-rw-r--r--   0        0        0      561 2023-07-14 21:37:39.035325 io_collection-0.8.0/src/io_collection/load/load_text.py
+-rw-r--r--   0        0        0        0 2023-07-14 21:37:39.035325 io_collection-0.8.0/src/io_collection/py.typed
+-rw-r--r--   0        0        0      209 2023-07-14 21:37:39.035325 io_collection-0.8.0/src/io_collection/quilt/__init__.py
+-rw-r--r--   0        0        0      185 2023-07-14 21:37:39.035325 io_collection-0.8.0/src/io_collection/quilt/load_quilt_package.py
+-rw-r--r--   0        0        0      287 2023-07-14 21:37:39.039325 io_collection-0.8.0/src/io_collection/quilt/save_quilt_item.py
+-rw-r--r--   0        0        0      616 2023-07-14 21:37:39.039325 io_collection-0.8.0/src/io_collection/save/__init__.py
+-rw-r--r--   0        0        0      745 2023-07-14 21:37:39.039325 io_collection-0.8.0/src/io_collection/save/save_buffer.py
+-rw-r--r--   0        0        0      920 2023-07-14 21:37:39.039325 io_collection-0.8.0/src/io_collection/save/save_dataframe.py
+-rw-r--r--   0        0        0      889 2023-07-14 21:37:39.039325 io_collection-0.8.0/src/io_collection/save/save_figure.py
+-rw-r--r--   0        0        0      514 2023-07-14 21:37:39.039325 io_collection-0.8.0/src/io_collection/save/save_gif.py
+-rw-r--r--   0        0        0     1404 2023-07-14 21:37:39.039325 io_collection-0.8.0/src/io_collection/save/save_image.py
+-rw-r--r--   0        0        0      590 2023-07-14 21:37:39.039325 io_collection-0.8.0/src/io_collection/save/save_json.py
+-rw-r--r--   0        0        0      274 2023-07-14 21:37:39.039325 io_collection-0.8.0/src/io_collection/save/save_pickle.py
+-rw-r--r--   0        0        0     1018 2023-07-14 21:37:39.039325 io_collection-0.8.0/src/io_collection/save/save_tar.py
+-rw-r--r--   0        0        0      712 2023-07-14 21:37:39.039325 io_collection-0.8.0/src/io_collection/save/save_text.py
+-rw-r--r--   0        0        0     3320 1970-01-01 00:00:00.000000 io_collection-0.8.0/PKG-INFO
```

### Comparing `io_collection-0.7.3/LICENSE` & `io_collection-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `io_collection-0.7.3/README.md` & `io_collection-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `io_collection-0.7.3/pyproject.toml` & `io_collection-0.8.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "io-collection"
-version = "0.7.3"
+version = "0.8.0"
 description = "Collection of tasks for I/O."
 authors = [
     "Jessica S. Yu <jesyu@uw.edu>"
 ]
 license = "BSD-3-Clause"
 readme = "README.md"
```

### Comparing `io_collection-0.7.3/src/io_collection/keys/change_key.py` & `io_collection-0.8.0/src/io_collection/keys/change_key.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.7.3/src/io_collection/keys/check_key.py` & `io_collection-0.8.0/src/io_collection/keys/check_key.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.7.3/src/io_collection/keys/copy_key.py` & `io_collection-0.8.0/src/io_collection/keys/copy_key.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.7.3/src/io_collection/keys/get_keys.py` & `io_collection-0.8.0/src/io_collection/keys/get_keys.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.7.3/src/io_collection/load/load_buffer.py` & `io_collection-0.8.0/src/io_collection/load/load_buffer.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.7.3/src/io_collection/load/load_dataframe.py` & `io_collection-0.8.0/src/io_collection/load/load_dataframe.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.7.3/src/io_collection/load/load_image.py` & `io_collection-0.8.0/src/io_collection/load/load_image.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.7.3/src/io_collection/load/load_tar.py` & `io_collection-0.8.0/src/io_collection/load/load_tar.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.7.3/src/io_collection/load/load_text.py` & `io_collection-0.8.0/src/io_collection/load/load_text.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.7.3/src/io_collection/save/__init__.py` & `io_collection-0.8.0/src/io_collection/save/__init__.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.7.3/src/io_collection/save/save_buffer.py` & `io_collection-0.8.0/src/io_collection/save/save_buffer.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.7.3/src/io_collection/save/save_dataframe.py` & `io_collection-0.8.0/src/io_collection/save/save_dataframe.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.7.3/src/io_collection/save/save_figure.py` & `io_collection-0.8.0/src/io_collection/save/save_figure.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.7.3/src/io_collection/save/save_gif.py` & `io_collection-0.8.0/src/io_collection/save/save_gif.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.7.3/src/io_collection/save/save_json.py` & `io_collection-0.8.0/src/io_collection/save/save_json.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,13 +5,13 @@
 from io_collection.save.save_text import save_text
 
 
 def save_json(location: str, key: str, obj: Union[dict, list], levels: int = 5) -> None:
     contents = json.dumps(obj, indent=2)
 
     for level in range(1, levels + 1):
-        match_pattern = r"\[" + ",".join([r"\n\s*([\d\.]+)" for i in range(level)]) + r"\n\s*\]"
+        match_pattern = r"\[" + ",".join([r"\n\s*([e\-\d\.]+)" for i in range(level)]) + r"\n\s*\]"
         sub_pattern = "[" + ",".join([f"\\{i + 1}" for i in range(level)]) + "]"
         pattern = re.compile(match_pattern)
         contents = pattern.sub(sub_pattern, contents)
 
     save_text(location, key, contents)
```

### Comparing `io_collection-0.7.3/src/io_collection/save/save_tar.py` & `io_collection-0.8.0/src/io_collection/save/save_tar.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.7.3/src/io_collection/save/save_text.py` & `io_collection-0.8.0/src/io_collection/save/save_text.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.7.3/PKG-INFO` & `io_collection-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: io-collection
-Version: 0.7.3
+Version: 0.8.0
 Summary: Collection of tasks for I/O.
 License: BSD-3-Clause
 Author: Jessica S. Yu
 Author-email: jesyu@uw.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

