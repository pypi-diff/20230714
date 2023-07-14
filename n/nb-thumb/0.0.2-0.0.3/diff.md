# Comparing `tmp/nb-thumb-0.0.2.tar.gz` & `tmp/nb-thumb-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nb-thumb-0.0.2.tar", last modified: Fri Jul 14 06:04:25 2023, max compression
+gzip compressed data, was "nb-thumb-0.0.3.tar", last modified: Fri Jul 14 06:09:41 2023, max compression
```

## Comparing `nb-thumb-0.0.2.tar` & `nb-thumb-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-07-14 06:04:25.676774 nb-thumb-0.0.2/
--rw-rw-r--   0 hamel      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 nb-thumb-0.0.2/LICENSE
--rw-rw-r--   0 hamel      (501) staff       (20)      111 2023-04-27 10:12:58.000000 nb-thumb-0.0.2/MANIFEST.in
--rw-r--r--   0 hamel      (501) staff       (20)     1402 2023-07-14 06:04:25.676605 nb-thumb-0.0.2/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)      601 2023-07-14 06:03:56.000000 nb-thumb-0.0.2/README.md
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-07-14 06:04:25.675410 nb-thumb-0.0.2/nb_thumb/
--rw-r--r--   0 hamel      (501) staff       (20)       22 2023-07-14 06:04:15.000000 nb-thumb-0.0.2/nb_thumb/__init__.py
--rw-r--r--   0 hamel      (501) staff       (20)      791 2023-07-14 06:04:15.000000 nb-thumb-0.0.2/nb_thumb/_modidx.py
--rw-r--r--   0 hamel      (501) staff       (20)      142 2023-07-14 03:45:28.000000 nb-thumb-0.0.2/nb_thumb/core.py
--rw-r--r--   0 hamel      (501) staff       (20)     1932 2023-07-14 06:04:15.000000 nb-thumb-0.0.2/nb_thumb/thumb.py
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-07-14 06:04:25.676412 nb-thumb-0.0.2/nb_thumb.egg-info/
--rw-r--r--   0 hamel      (501) staff       (20)     1402 2023-07-14 06:04:25.000000 nb-thumb-0.0.2/nb_thumb.egg-info/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)      352 2023-07-14 06:04:25.000000 nb-thumb-0.0.2/nb_thumb.egg-info/SOURCES.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2023-07-14 06:04:25.000000 nb-thumb-0.0.2/nb_thumb.egg-info/dependency_links.txt
--rw-r--r--   0 hamel      (501) staff       (20)       38 2023-07-14 06:04:25.000000 nb-thumb-0.0.2/nb_thumb.egg-info/entry_points.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2023-07-14 05:34:35.000000 nb-thumb-0.0.2/nb_thumb.egg-info/not-zip-safe
--rw-r--r--   0 hamel      (501) staff       (20)       46 2023-07-14 06:04:25.000000 nb-thumb-0.0.2/nb_thumb.egg-info/requires.txt
--rw-r--r--   0 hamel      (501) staff       (20)        9 2023-07-14 06:04:25.000000 nb-thumb-0.0.2/nb_thumb.egg-info/top_level.txt
--rw-r--r--   0 hamel      (501) staff       (20)      850 2023-07-14 06:04:15.000000 nb-thumb-0.0.2/settings.ini
--rw-r--r--   0 hamel      (501) staff       (20)       38 2023-07-14 06:04:25.676823 nb-thumb-0.0.2/setup.cfg
--rw-rw-r--   0 hamel      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 nb-thumb-0.0.2/setup.py
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-07-14 06:09:41.848395 nb-thumb-0.0.3/
+-rw-rw-r--   0 hamel      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 nb-thumb-0.0.3/LICENSE
+-rw-rw-r--   0 hamel      (501) staff       (20)      111 2023-04-27 10:12:58.000000 nb-thumb-0.0.3/MANIFEST.in
+-rw-r--r--   0 hamel      (501) staff       (20)     1402 2023-07-14 06:09:41.848225 nb-thumb-0.0.3/PKG-INFO
+-rw-r--r--   0 hamel      (501) staff       (20)      601 2023-07-14 06:03:56.000000 nb-thumb-0.0.3/README.md
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-07-14 06:09:41.846852 nb-thumb-0.0.3/nb_thumb/
+-rw-r--r--   0 hamel      (501) staff       (20)       22 2023-07-14 06:09:30.000000 nb-thumb-0.0.3/nb_thumb/__init__.py
+-rw-r--r--   0 hamel      (501) staff       (20)      791 2023-07-14 06:09:30.000000 nb-thumb-0.0.3/nb_thumb/_modidx.py
+-rw-r--r--   0 hamel      (501) staff       (20)      142 2023-07-14 03:45:28.000000 nb-thumb-0.0.3/nb_thumb/core.py
+-rw-r--r--   0 hamel      (501) staff       (20)     1948 2023-07-14 06:09:30.000000 nb-thumb-0.0.3/nb_thumb/thumb.py
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-07-14 06:09:41.847972 nb-thumb-0.0.3/nb_thumb.egg-info/
+-rw-r--r--   0 hamel      (501) staff       (20)     1402 2023-07-14 06:09:41.000000 nb-thumb-0.0.3/nb_thumb.egg-info/PKG-INFO
+-rw-r--r--   0 hamel      (501) staff       (20)      352 2023-07-14 06:09:41.000000 nb-thumb-0.0.3/nb_thumb.egg-info/SOURCES.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        1 2023-07-14 06:09:41.000000 nb-thumb-0.0.3/nb_thumb.egg-info/dependency_links.txt
+-rw-r--r--   0 hamel      (501) staff       (20)       38 2023-07-14 06:09:41.000000 nb-thumb-0.0.3/nb_thumb.egg-info/entry_points.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        1 2023-07-14 05:34:35.000000 nb-thumb-0.0.3/nb_thumb.egg-info/not-zip-safe
+-rw-r--r--   0 hamel      (501) staff       (20)       46 2023-07-14 06:09:41.000000 nb-thumb-0.0.3/nb_thumb.egg-info/requires.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        9 2023-07-14 06:09:41.000000 nb-thumb-0.0.3/nb_thumb.egg-info/top_level.txt
+-rw-r--r--   0 hamel      (501) staff       (20)      850 2023-07-14 06:09:30.000000 nb-thumb-0.0.3/settings.ini
+-rw-r--r--   0 hamel      (501) staff       (20)       38 2023-07-14 06:09:41.848446 nb-thumb-0.0.3/setup.cfg
+-rw-rw-r--   0 hamel      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 nb-thumb-0.0.3/setup.py
```

### Comparing `nb-thumb-0.0.2/LICENSE` & `nb-thumb-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nb-thumb-0.0.2/PKG-INFO` & `nb-thumb-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-thumb
-Version: 0.0.2
+Version: 0.0.3
 Summary: Extract thumbnails from Jupyter notebooks
 Home-page: https://github.com/fastai/nb-thumb
 Author: Hamel Husain
 Author-email: hamel.husain@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `nb-thumb-0.0.2/README.md` & `nb-thumb-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nb-thumb-0.0.2/nb_thumb/_modidx.py` & `nb-thumb-0.0.3/nb_thumb/_modidx.py`

 * *Files identical despite different names*

### Comparing `nb-thumb-0.0.2/nb_thumb/thumb.py` & `nb-thumb-0.0.3/nb_thumb/thumb.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 def _decode_img(base64_str):
     img = Image.open(BytesIO(base64.b64decode(base64_str)))
     if img.mode == "RGBA":
         img = img.convert("RGB")
     return img
 
 def get_img(nb_path, label='thumbnail'):
-    "Get image from notebook with a cell comment #|label: {label}"
+    "Get image from notebook with a quarto cell directive with `#|label: {label}`"
     out_plots = None
     lbl = re.compile(f'#\|(\s*)label:(\s*){label}')
     nb = nbformat.read(open(nb_path), as_version=4)
     for cell in nb.cells:
         if lbl.search(cell.source):
             out_plots = [x for x in cell.outputs if x.output_type == "display_data" and 'data' in x]
             if out_plots:
```

### Comparing `nb-thumb-0.0.2/nb_thumb.egg-info/PKG-INFO` & `nb-thumb-0.0.3/nb_thumb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-thumb
-Version: 0.0.2
+Version: 0.0.3
 Summary: Extract thumbnails from Jupyter notebooks
 Home-page: https://github.com/fastai/nb-thumb
 Author: Hamel Husain
 Author-email: hamel.husain@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `nb-thumb-0.0.2/settings.ini` & `nb-thumb-0.0.3/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = nb-thumb
 lib_name = nb-thumb
-version = 0.0.2
+version = 0.0.3
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = nb_thumb
 nbs_path = nbs
 recursive = True
```

### Comparing `nb-thumb-0.0.2/setup.py` & `nb-thumb-0.0.3/setup.py`

 * *Files identical despite different names*

