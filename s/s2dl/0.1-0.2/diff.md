# Comparing `tmp/s2dl-0.1.tar.gz` & `tmp/s2dl-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2dl-0.1.tar", last modified: Fri Jul 14 07:32:00 2023, max compression
+gzip compressed data, was "s2dl-0.2.tar", last modified: Fri Jul 14 07:40:41 2023, max compression
```

## Comparing `s2dl-0.1.tar` & `s2dl-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 NickW      (503) staff       (20)        0 2023-07-14 07:32:00.496819 s2dl-0.1/
--rw-r--r--   0 NickW      (503) staff       (20)     1066 2023-07-14 06:27:57.000000 s2dl-0.1/LICENSE
--rw-r--r--   0 NickW      (503) staff       (20)      214 2023-07-14 07:32:00.496403 s2dl-0.1/PKG-INFO
--rw-r--r--   0 NickW      (503) staff       (20)     1261 2023-07-14 07:31:14.000000 s2dl-0.1/README.md
-drwxr-xr-x   0 NickW      (503) staff       (20)        0 2023-07-14 07:32:00.494098 s2dl-0.1/s2dl/
--rw-r--r--   0 NickW      (503) staff       (20)      130 2023-07-14 06:53:41.000000 s2dl-0.1/s2dl/__init__.py
--rw-r--r--   0 NickW      (503) staff       (20)     7886 2023-07-14 06:56:01.000000 s2dl-0.1/s2dl/s2dl.py
-drwxr-xr-x   0 NickW      (503) staff       (20)        0 2023-07-14 07:32:00.495878 s2dl-0.1/s2dl.egg-info/
--rw-r--r--   0 NickW      (503) staff       (20)      214 2023-07-14 07:32:00.000000 s2dl-0.1/s2dl.egg-info/PKG-INFO
--rw-r--r--   0 NickW      (503) staff       (20)      168 2023-07-14 07:32:00.000000 s2dl-0.1/s2dl.egg-info/SOURCES.txt
--rw-r--r--   0 NickW      (503) staff       (20)        1 2023-07-14 07:32:00.000000 s2dl-0.1/s2dl.egg-info/dependency_links.txt
--rw-r--r--   0 NickW      (503) staff       (20)        5 2023-07-14 07:32:00.000000 s2dl-0.1/s2dl.egg-info/top_level.txt
--rw-r--r--   0 NickW      (503) staff       (20)       38 2023-07-14 07:32:00.496963 s2dl-0.1/setup.cfg
--rw-r--r--   0 NickW      (503) staff       (20)      313 2023-07-14 06:51:42.000000 s2dl-0.1/setup.py
+drwxr-xr-x   0 NickW      (503) staff       (20)        0 2023-07-14 07:40:41.247444 s2dl-0.2/
+-rw-r--r--   0 NickW      (503) staff       (20)     1066 2023-07-14 06:27:57.000000 s2dl-0.2/LICENSE
+-rw-r--r--   0 NickW      (503) staff       (20)     1570 2023-07-14 07:40:41.246920 s2dl-0.2/PKG-INFO
+-rw-r--r--   0 NickW      (503) staff       (20)     1261 2023-07-14 07:31:14.000000 s2dl-0.2/README.md
+drwxr-xr-x   0 NickW      (503) staff       (20)        0 2023-07-14 07:40:41.243873 s2dl-0.2/s2dl/
+-rw-r--r--   0 NickW      (503) staff       (20)      130 2023-07-14 06:53:41.000000 s2dl-0.2/s2dl/__init__.py
+-rw-r--r--   0 NickW      (503) staff       (20)     7886 2023-07-14 06:56:01.000000 s2dl-0.2/s2dl/s2dl.py
+drwxr-xr-x   0 NickW      (503) staff       (20)        0 2023-07-14 07:40:41.246050 s2dl-0.2/s2dl.egg-info/
+-rw-r--r--   0 NickW      (503) staff       (20)     1570 2023-07-14 07:40:41.000000 s2dl-0.2/s2dl.egg-info/PKG-INFO
+-rw-r--r--   0 NickW      (503) staff       (20)      168 2023-07-14 07:40:41.000000 s2dl-0.2/s2dl.egg-info/SOURCES.txt
+-rw-r--r--   0 NickW      (503) staff       (20)        1 2023-07-14 07:40:41.000000 s2dl-0.2/s2dl.egg-info/dependency_links.txt
+-rw-r--r--   0 NickW      (503) staff       (20)        5 2023-07-14 07:40:41.000000 s2dl-0.2/s2dl.egg-info/top_level.txt
+-rw-r--r--   0 NickW      (503) staff       (20)       38 2023-07-14 07:40:41.247616 s2dl-0.2/setup.cfg
+-rw-r--r--   0 NickW      (503) staff       (20)      543 2023-07-14 07:36:30.000000 s2dl-0.2/setup.py
```

### Comparing `s2dl-0.1/LICENSE` & `s2dl-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `s2dl-0.1/README.md` & `s2dl-0.2/README.md`

 * *Files identical despite different names*

### Comparing `s2dl-0.1/s2dl/s2dl.py` & `s2dl-0.2/s2dl/s2dl.py`

 * *Files identical despite different names*

