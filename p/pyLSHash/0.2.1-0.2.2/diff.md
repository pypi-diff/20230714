# Comparing `tmp/pyLSHash-0.2.1.tar.gz` & `tmp/pyLSHash-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyLSHash-0.2.1.tar", last modified: Fri Jul 14 03:50:22 2023, max compression
+gzip compressed data, was "pyLSHash-0.2.2.tar", last modified: Fri Jul 14 03:53:37 2023, max compression
```

## Comparing `pyLSHash-0.2.1.tar` & `pyLSHash-0.2.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-14 03:50:22.730537 pyLSHash-0.2.1/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1063 2023-07-14 03:40:21.000000 pyLSHash-0.2.1/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11654 2023-07-14 03:50:22.730537 pyLSHash-0.2.1/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11285 2023-07-14 03:40:21.000000 pyLSHash-0.2.1/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-14 03:50:22.722537 pyLSHash-0.2.1/pyLSHash/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      176 2023-07-14 03:49:11.000000 pyLSHash-0.2.1/pyLSHash/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      876 2023-07-14 03:40:21.000000 pyLSHash-0.2.1/pyLSHash/dist_func.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      202 2023-07-14 03:40:21.000000 pyLSHash-0.2.1/pyLSHash/distance.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      464 2023-07-14 03:40:21.000000 pyLSHash-0.2.1/pyLSHash/fuzzy_hash.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1073 2023-07-14 03:40:21.000000 pyLSHash-0.2.1/pyLSHash/img_hash.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1539 2023-07-14 03:40:21.000000 pyLSHash-0.2.1/pyLSHash/img_hist.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      924 2023-07-14 03:40:21.000000 pyLSHash-0.2.1/pyLSHash/img_ssim.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5299 2023-07-14 03:40:21.000000 pyLSHash-0.2.1/pyLSHash/lshash.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1782 2023-07-14 03:40:21.000000 pyLSHash-0.2.1/pyLSHash/min_hash.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3022 2023-07-14 03:40:21.000000 pyLSHash-0.2.1/pyLSHash/simhash.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2673 2023-07-14 03:40:21.000000 pyLSHash-0.2.1/pyLSHash/storage.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-14 03:50:22.730537 pyLSHash-0.2.1/pyLSHash.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11654 2023-07-14 03:50:22.000000 pyLSHash-0.2.1/pyLSHash.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      446 2023-07-14 03:50:22.000000 pyLSHash-0.2.1/pyLSHash.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-14 03:50:22.000000 pyLSHash-0.2.1/pyLSHash.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-14 03:50:22.000000 pyLSHash-0.2.1/pyLSHash.egg-info/not-zip-safe
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        6 2023-07-14 03:50:22.000000 pyLSHash-0.2.1/pyLSHash.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-07-14 03:50:22.000000 pyLSHash-0.2.1/pyLSHash.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-07-14 03:50:22.730537 pyLSHash-0.2.1/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      991 2023-07-14 03:40:21.000000 pyLSHash-0.2.1/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-14 03:53:37.934537 pyLSHash-0.2.2/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1063 2023-07-14 03:40:21.000000 pyLSHash-0.2.2/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11654 2023-07-14 03:53:37.934537 pyLSHash-0.2.2/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11285 2023-07-14 03:40:21.000000 pyLSHash-0.2.2/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-14 03:53:37.926537 pyLSHash-0.2.2/pyLSHash/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      176 2023-07-14 03:53:27.000000 pyLSHash-0.2.2/pyLSHash/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      876 2023-07-14 03:40:21.000000 pyLSHash-0.2.2/pyLSHash/dist_func.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      202 2023-07-14 03:40:21.000000 pyLSHash-0.2.2/pyLSHash/distance.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      464 2023-07-14 03:40:21.000000 pyLSHash-0.2.2/pyLSHash/fuzzy_hash.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1073 2023-07-14 03:40:21.000000 pyLSHash-0.2.2/pyLSHash/img_hash.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1539 2023-07-14 03:40:21.000000 pyLSHash-0.2.2/pyLSHash/img_hist.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      924 2023-07-14 03:40:21.000000 pyLSHash-0.2.2/pyLSHash/img_ssim.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5299 2023-07-14 03:40:21.000000 pyLSHash-0.2.2/pyLSHash/lshash.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1782 2023-07-14 03:40:21.000000 pyLSHash-0.2.2/pyLSHash/min_hash.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3022 2023-07-14 03:40:21.000000 pyLSHash-0.2.2/pyLSHash/simhash.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2673 2023-07-14 03:40:21.000000 pyLSHash-0.2.2/pyLSHash/storage.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-14 03:53:37.934537 pyLSHash-0.2.2/pyLSHash.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11654 2023-07-14 03:53:37.000000 pyLSHash-0.2.2/pyLSHash.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      446 2023-07-14 03:53:37.000000 pyLSHash-0.2.2/pyLSHash.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-14 03:53:37.000000 pyLSHash-0.2.2/pyLSHash.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-14 03:50:22.000000 pyLSHash-0.2.2/pyLSHash.egg-info/not-zip-safe
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       24 2023-07-14 03:53:37.000000 pyLSHash-0.2.2/pyLSHash.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-07-14 03:53:37.000000 pyLSHash-0.2.2/pyLSHash.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-07-14 03:53:37.934537 pyLSHash-0.2.2/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1019 2023-07-14 03:53:22.000000 pyLSHash-0.2.2/setup.py
```

### Comparing `pyLSHash-0.2.1/LICENSE` & `pyLSHash-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyLSHash-0.2.1/PKG-INFO` & `pyLSHash-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyLSHash
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python implementation of locality sensitive hashing.
 Home-page: https://github.com/guofei9987/pyLSHash
 Author: Guo Fei
 Author-email: guofei9987@foxmail.com
 License: MIT
 Platform: linux
 Platform: windows
```

### Comparing `pyLSHash-0.2.1/README.md` & `pyLSHash-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pyLSHash-0.2.1/pyLSHash/dist_func.py` & `pyLSHash-0.2.2/pyLSHash/dist_func.py`

 * *Files identical despite different names*

### Comparing `pyLSHash-0.2.1/pyLSHash/img_hash.py` & `pyLSHash-0.2.2/pyLSHash/img_hash.py`

 * *Files identical despite different names*

### Comparing `pyLSHash-0.2.1/pyLSHash/img_hist.py` & `pyLSHash-0.2.2/pyLSHash/img_hist.py`

 * *Files identical despite different names*

### Comparing `pyLSHash-0.2.1/pyLSHash/img_ssim.py` & `pyLSHash-0.2.2/pyLSHash/img_ssim.py`

 * *Files identical despite different names*

### Comparing `pyLSHash-0.2.1/pyLSHash/lshash.py` & `pyLSHash-0.2.2/pyLSHash/lshash.py`

 * *Files identical despite different names*

### Comparing `pyLSHash-0.2.1/pyLSHash/min_hash.py` & `pyLSHash-0.2.2/pyLSHash/min_hash.py`

 * *Files identical despite different names*

### Comparing `pyLSHash-0.2.1/pyLSHash/simhash.py` & `pyLSHash-0.2.2/pyLSHash/simhash.py`

 * *Files identical despite different names*

### Comparing `pyLSHash-0.2.1/pyLSHash/storage.py` & `pyLSHash-0.2.2/pyLSHash/storage.py`

 * *Files identical despite different names*

### Comparing `pyLSHash-0.2.1/pyLSHash.egg-info/PKG-INFO` & `pyLSHash-0.2.2/pyLSHash.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyLSHash
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python implementation of locality sensitive hashing.
 Home-page: https://github.com/guofei9987/pyLSHash
 Author: Guo Fei
 Author-email: guofei9987@foxmail.com
 License: MIT
 Platform: linux
 Platform: windows
```

### Comparing `pyLSHash-0.2.1/setup.py` & `pyLSHash-0.2.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,9 +24,9 @@
       long_description_content_type="text/markdown",
       url='https://github.com/guofei9987/pyLSHash',
       author='Guo Fei',
       author_email='guofei9987@foxmail.com',
       license='MIT',
       packages=find_packages(),
       platforms=['linux', 'windows', 'macos'],
-      install_requires=['numpy'],
+      install_requires=read_requirements('requirements.txt'),
       zip_safe=False)
```

