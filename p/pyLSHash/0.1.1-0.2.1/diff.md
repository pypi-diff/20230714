# Comparing `tmp/pyLSHash-0.1.1.tar.gz` & `tmp/pyLSHash-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyLSHash-0.1.1.tar", last modified: Sat Jul 23 19:15:02 2022, max compression
+gzip compressed data, was "pyLSHash-0.2.1.tar", last modified: Fri Jul 14 03:50:22 2023, max compression
```

## Comparing `pyLSHash-0.1.1.tar` & `pyLSHash-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,25 @@
-drwxr-xr-x   0 guofei     (501) staff       (20)        0 2022-07-23 19:15:02.973693 pyLSHash-0.1.1/
--rw-r--r--   0 guofei     (501) staff       (20)     5616 2022-07-23 19:15:02.973536 pyLSHash-0.1.1/PKG-INFO
--rw-r--r--   0 guofei     (501) staff       (20)     4065 2022-07-23 18:46:37.000000 pyLSHash-0.1.1/README.md
-drwxr-xr-x   0 guofei     (501) staff       (20)        0 2022-07-23 19:15:02.972440 pyLSHash-0.1.1/pyLSHash/
--rw-r--r--   0 guofei     (501) staff       (20)       83 2022-07-23 18:46:54.000000 pyLSHash-0.1.1/pyLSHash/__init__.py
--rw-r--r--   0 guofei     (501) staff       (20)      876 2022-07-19 08:40:26.000000 pyLSHash-0.1.1/pyLSHash/dist_func.py
--rw-r--r--   0 guofei     (501) staff       (20)     5299 2022-07-24 17:03:22.000000 pyLSHash-0.1.1/pyLSHash/lshash.py
--rw-r--r--   0 guofei     (501) staff       (20)     2673 2022-07-24 17:13:42.000000 pyLSHash-0.1.1/pyLSHash/storage.py
-drwxr-xr-x   0 guofei     (501) staff       (20)        0 2022-07-23 19:15:02.973332 pyLSHash-0.1.1/pyLSHash.egg-info/
--rw-r--r--   0 guofei     (501) staff       (20)     5616 2022-07-23 19:15:02.000000 pyLSHash-0.1.1/pyLSHash.egg-info/PKG-INFO
--rw-r--r--   0 guofei     (501) staff       (20)      290 2022-07-23 19:15:02.000000 pyLSHash-0.1.1/pyLSHash.egg-info/SOURCES.txt
--rw-r--r--   0 guofei     (501) staff       (20)        1 2022-07-23 19:15:02.000000 pyLSHash-0.1.1/pyLSHash.egg-info/dependency_links.txt
--rw-r--r--   0 guofei     (501) staff       (20)        1 2022-07-23 19:15:02.000000 pyLSHash-0.1.1/pyLSHash.egg-info/not-zip-safe
--rw-r--r--   0 guofei     (501) staff       (20)        6 2022-07-23 19:15:02.000000 pyLSHash-0.1.1/pyLSHash.egg-info/requires.txt
--rw-r--r--   0 guofei     (501) staff       (20)        9 2022-07-23 19:15:02.000000 pyLSHash-0.1.1/pyLSHash.egg-info/top_level.txt
--rw-r--r--   0 guofei     (501) staff       (20)       38 2022-07-23 19:15:02.973741 pyLSHash-0.1.1/setup.cfg
--rw-r--r--   0 guofei     (501) staff       (20)      991 2022-07-19 08:40:26.000000 pyLSHash-0.1.1/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-14 03:50:22.730537 pyLSHash-0.2.1/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1063 2023-07-14 03:40:21.000000 pyLSHash-0.2.1/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11654 2023-07-14 03:50:22.730537 pyLSHash-0.2.1/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11285 2023-07-14 03:40:21.000000 pyLSHash-0.2.1/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-14 03:50:22.722537 pyLSHash-0.2.1/pyLSHash/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      176 2023-07-14 03:49:11.000000 pyLSHash-0.2.1/pyLSHash/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      876 2023-07-14 03:40:21.000000 pyLSHash-0.2.1/pyLSHash/dist_func.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      202 2023-07-14 03:40:21.000000 pyLSHash-0.2.1/pyLSHash/distance.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      464 2023-07-14 03:40:21.000000 pyLSHash-0.2.1/pyLSHash/fuzzy_hash.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1073 2023-07-14 03:40:21.000000 pyLSHash-0.2.1/pyLSHash/img_hash.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1539 2023-07-14 03:40:21.000000 pyLSHash-0.2.1/pyLSHash/img_hist.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      924 2023-07-14 03:40:21.000000 pyLSHash-0.2.1/pyLSHash/img_ssim.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5299 2023-07-14 03:40:21.000000 pyLSHash-0.2.1/pyLSHash/lshash.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1782 2023-07-14 03:40:21.000000 pyLSHash-0.2.1/pyLSHash/min_hash.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3022 2023-07-14 03:40:21.000000 pyLSHash-0.2.1/pyLSHash/simhash.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2673 2023-07-14 03:40:21.000000 pyLSHash-0.2.1/pyLSHash/storage.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-14 03:50:22.730537 pyLSHash-0.2.1/pyLSHash.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11654 2023-07-14 03:50:22.000000 pyLSHash-0.2.1/pyLSHash.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      446 2023-07-14 03:50:22.000000 pyLSHash-0.2.1/pyLSHash.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-14 03:50:22.000000 pyLSHash-0.2.1/pyLSHash.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-14 03:50:22.000000 pyLSHash-0.2.1/pyLSHash.egg-info/not-zip-safe
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        6 2023-07-14 03:50:22.000000 pyLSHash-0.2.1/pyLSHash.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-07-14 03:50:22.000000 pyLSHash-0.2.1/pyLSHash.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-07-14 03:50:22.730537 pyLSHash-0.2.1/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      991 2023-07-14 03:40:21.000000 pyLSHash-0.2.1/setup.py
```

### Comparing `pyLSHash-0.1.1/pyLSHash/dist_func.py` & `pyLSHash-0.2.1/pyLSHash/dist_func.py`

 * *Files identical despite different names*

### Comparing `pyLSHash-0.1.1/pyLSHash/lshash.py` & `pyLSHash-0.2.1/pyLSHash/lshash.py`

 * *Files identical despite different names*

### Comparing `pyLSHash-0.1.1/pyLSHash/storage.py` & `pyLSHash-0.2.1/pyLSHash/storage.py`

 * *Files identical despite different names*

### Comparing `pyLSHash-0.1.1/setup.py` & `pyLSHash-0.2.1/setup.py`

 * *Files identical despite different names*

