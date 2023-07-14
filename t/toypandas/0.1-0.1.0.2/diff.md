# Comparing `tmp/toypandas-0.1.tar.gz` & `tmp/toypandas-0.1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/toypandas-0.1.tar", last modified: Fri Jul 14 12:59:43 2023, max compression
+gzip compressed data, was "dist/toypandas-0.1.0.2.tar", last modified: Fri Jul 14 13:08:21 2023, max compression
```

## Comparing `toypandas-0.1.tar` & `toypandas-0.1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 danieletraversaro   (501) staff       (20)        0 2023-07-14 12:59:43.000000 toypandas-0.1/
--rw-r--r--   0 danieletraversaro   (501) staff       (20)      281 2023-07-14 12:59:43.000000 toypandas-0.1/PKG-INFO
-drwxr-xr-x   0 danieletraversaro   (501) staff       (20)        0 2023-07-14 12:59:43.000000 toypandas-0.1/ToyPandas/
--rw-r--r--   0 danieletraversaro   (501) staff       (20)     9725 2023-07-14 12:05:35.000000 toypandas-0.1/ToyPandas/toypandas.py
-drwxr-xr-x   0 danieletraversaro   (501) staff       (20)        0 2023-07-14 12:59:43.000000 toypandas-0.1/ToyPandas.egg-info/
--rw-r--r--   0 danieletraversaro   (501) staff       (20)      281 2023-07-14 12:59:43.000000 toypandas-0.1/ToyPandas.egg-info/PKG-INFO
--rw-r--r--   0 danieletraversaro   (501) staff       (20)      382 2023-07-14 12:59:43.000000 toypandas-0.1/ToyPandas.egg-info/SOURCES.txt
--rw-r--r--   0 danieletraversaro   (501) staff       (20)       37 2023-07-14 12:59:43.000000 toypandas-0.1/ToyPandas.egg-info/requires.txt
--rw-r--r--   0 danieletraversaro   (501) staff       (20)       10 2023-07-14 12:59:43.000000 toypandas-0.1/ToyPandas.egg-info/top_level.txt
--rw-r--r--   0 danieletraversaro   (501) staff       (20)        1 2023-07-14 12:59:43.000000 toypandas-0.1/ToyPandas.egg-info/dependency_links.txt
--rw-r--r--   0 danieletraversaro   (501) staff       (20)      360 2023-07-14 12:59:27.000000 toypandas-0.1/setup.py
--rw-r--r--   0 danieletraversaro   (501) staff       (20)       59 2023-07-14 12:59:43.000000 toypandas-0.1/setup.cfg
+drwxr-xr-x   0 danieletraversaro   (501) staff       (20)        0 2023-07-14 13:08:21.000000 toypandas-0.1.0.2/
+-rw-r--r--   0 danieletraversaro   (501) staff       (20)      285 2023-07-14 13:08:21.000000 toypandas-0.1.0.2/PKG-INFO
+drwxr-xr-x   0 danieletraversaro   (501) staff       (20)        0 2023-07-14 13:08:21.000000 toypandas-0.1.0.2/ToyPandas/
+-rw-r--r--   0 danieletraversaro   (501) staff       (20)     9725 2023-07-14 12:05:35.000000 toypandas-0.1.0.2/ToyPandas/toypandas.py
+drwxr-xr-x   0 danieletraversaro   (501) staff       (20)        0 2023-07-14 13:08:21.000000 toypandas-0.1.0.2/ToyPandas.egg-info/
+-rw-r--r--   0 danieletraversaro   (501) staff       (20)      285 2023-07-14 13:08:21.000000 toypandas-0.1.0.2/ToyPandas.egg-info/PKG-INFO
+-rw-r--r--   0 danieletraversaro   (501) staff       (20)      382 2023-07-14 13:08:21.000000 toypandas-0.1.0.2/ToyPandas.egg-info/SOURCES.txt
+-rw-r--r--   0 danieletraversaro   (501) staff       (20)       37 2023-07-14 13:08:21.000000 toypandas-0.1.0.2/ToyPandas.egg-info/requires.txt
+-rw-r--r--   0 danieletraversaro   (501) staff       (20)       10 2023-07-14 13:08:21.000000 toypandas-0.1.0.2/ToyPandas.egg-info/top_level.txt
+-rw-r--r--   0 danieletraversaro   (501) staff       (20)        1 2023-07-14 13:08:21.000000 toypandas-0.1.0.2/ToyPandas.egg-info/dependency_links.txt
+-rw-r--r--   0 danieletraversaro   (501) staff       (20)      364 2023-07-14 13:08:04.000000 toypandas-0.1.0.2/setup.py
+-rw-r--r--   0 danieletraversaro   (501) staff       (20)       59 2023-07-14 13:08:21.000000 toypandas-0.1.0.2/setup.cfg
```

### Comparing `toypandas-0.1/ToyPandas/toypandas.py` & `toypandas-0.1.0.2/ToyPandas/toypandas.py`

 * *Files identical despite different names*

