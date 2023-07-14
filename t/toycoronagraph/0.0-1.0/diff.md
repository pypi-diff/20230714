# Comparing `tmp/toycoronagraph-0.0.tar.gz` & `tmp/toycoronagraph-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toycoronagraph-0.0.tar", last modified: Thu Jul 13 21:56:19 2023, max compression
+gzip compressed data, was "toycoronagraph-1.0.tar", last modified: Fri Jul 14 14:37:32 2023, max compression
```

## Comparing `toycoronagraph-0.0.tar` & `toycoronagraph-1.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 yuchia    (1000) yuchia    (1000)        0 2023-07-13 21:56:19.021775 toycoronagraph-0.0/
--rw-rw-r--   0 yuchia    (1000) yuchia    (1000)     1066 2023-07-11 23:55:42.000000 toycoronagraph-0.0/LICENSE
--rw-rw-r--   0 yuchia    (1000) yuchia    (1000)      473 2023-07-13 21:56:19.021775 toycoronagraph-0.0/PKG-INFO
--rw-rw-r--   0 yuchia    (1000) yuchia    (1000)       47 2023-07-11 23:55:42.000000 toycoronagraph-0.0/README.md
--rw-rw-r--   0 yuchia    (1000) yuchia    (1000)       38 2023-07-13 21:56:19.021775 toycoronagraph-0.0/setup.cfg
--rw-rw-r--   0 yuchia    (1000) yuchia    (1000)     1298 2023-07-13 21:52:16.000000 toycoronagraph-0.0/setup.py
-drwxrwxr-x   0 yuchia    (1000) yuchia    (1000)        0 2023-07-13 21:56:19.021775 toycoronagraph-0.0/toycoronagraph/
--rw-rw-r--   0 yuchia    (1000) yuchia    (1000)      198 2023-07-13 21:24:09.000000 toycoronagraph-0.0/toycoronagraph/__init__.py
--rw-rw-r--   0 yuchia    (1000) yuchia    (1000)     2634 2023-07-13 21:18:26.000000 toycoronagraph-0.0/toycoronagraph/main.py
-drwxrwxr-x   0 yuchia    (1000) yuchia    (1000)        0 2023-07-13 21:56:19.021775 toycoronagraph-0.0/toycoronagraph.egg-info/
--rw-rw-r--   0 yuchia    (1000) yuchia    (1000)      473 2023-07-13 21:56:18.000000 toycoronagraph-0.0/toycoronagraph.egg-info/PKG-INFO
--rw-rw-r--   0 yuchia    (1000) yuchia    (1000)      302 2023-07-13 21:56:19.000000 toycoronagraph-0.0/toycoronagraph.egg-info/SOURCES.txt
--rw-rw-r--   0 yuchia    (1000) yuchia    (1000)        1 2023-07-13 21:56:18.000000 toycoronagraph-0.0/toycoronagraph.egg-info/dependency_links.txt
--rw-rw-r--   0 yuchia    (1000) yuchia    (1000)        1 2023-07-13 21:24:15.000000 toycoronagraph-0.0/toycoronagraph.egg-info/not-zip-safe
--rw-rw-r--   0 yuchia    (1000) yuchia    (1000)       28 2023-07-13 21:56:18.000000 toycoronagraph-0.0/toycoronagraph.egg-info/requires.txt
--rw-rw-r--   0 yuchia    (1000) yuchia    (1000)       15 2023-07-13 21:56:18.000000 toycoronagraph-0.0/toycoronagraph.egg-info/top_level.txt
+drwxrwxr-x   0 yuchia    (1000) yuchia    (1000)        0 2023-07-14 14:37:32.399708 toycoronagraph-1.0/
+-rw-rw-r--   0 yuchia    (1000) yuchia    (1000)     1066 2023-07-11 23:55:42.000000 toycoronagraph-1.0/LICENSE
+-rw-rw-r--   0 yuchia    (1000) yuchia    (1000)      473 2023-07-14 14:37:32.399708 toycoronagraph-1.0/PKG-INFO
+-rw-rw-r--   0 yuchia    (1000) yuchia    (1000)       88 2023-07-14 00:20:27.000000 toycoronagraph-1.0/README.md
+-rw-rw-r--   0 yuchia    (1000) yuchia    (1000)       38 2023-07-14 14:37:32.399708 toycoronagraph-1.0/setup.cfg
+-rw-rw-r--   0 yuchia    (1000) yuchia    (1000)     1298 2023-07-13 21:52:16.000000 toycoronagraph-1.0/setup.py
+drwxrwxr-x   0 yuchia    (1000) yuchia    (1000)        0 2023-07-14 14:37:32.399708 toycoronagraph-1.0/toycoronagraph/
+-rw-rw-r--   0 yuchia    (1000) yuchia    (1000)      199 2023-07-14 13:49:07.000000 toycoronagraph-1.0/toycoronagraph/__init__.py
+-rw-rw-r--   0 yuchia    (1000) yuchia    (1000)     3612 2023-07-14 14:34:22.000000 toycoronagraph-1.0/toycoronagraph/main.py
+-rw-rw-r--   0 yuchia    (1000) yuchia    (1000)     3320 2023-07-14 13:56:27.000000 toycoronagraph-1.0/toycoronagraph/psf.py
+drwxrwxr-x   0 yuchia    (1000) yuchia    (1000)        0 2023-07-14 14:37:32.399708 toycoronagraph-1.0/toycoronagraph.egg-info/
+-rw-rw-r--   0 yuchia    (1000) yuchia    (1000)      473 2023-07-14 14:37:32.000000 toycoronagraph-1.0/toycoronagraph.egg-info/PKG-INFO
+-rw-rw-r--   0 yuchia    (1000) yuchia    (1000)      324 2023-07-14 14:37:32.000000 toycoronagraph-1.0/toycoronagraph.egg-info/SOURCES.txt
+-rw-rw-r--   0 yuchia    (1000) yuchia    (1000)        1 2023-07-14 14:37:32.000000 toycoronagraph-1.0/toycoronagraph.egg-info/dependency_links.txt
+-rw-rw-r--   0 yuchia    (1000) yuchia    (1000)        1 2023-07-13 21:24:15.000000 toycoronagraph-1.0/toycoronagraph.egg-info/not-zip-safe
+-rw-rw-r--   0 yuchia    (1000) yuchia    (1000)       73 2023-07-14 14:37:32.000000 toycoronagraph-1.0/toycoronagraph.egg-info/requires.txt
+-rw-rw-r--   0 yuchia    (1000) yuchia    (1000)       15 2023-07-14 14:37:32.000000 toycoronagraph-1.0/toycoronagraph.egg-info/top_level.txt
```

### Comparing `toycoronagraph-0.0/LICENSE` & `toycoronagraph-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `toycoronagraph-0.0/setup.py` & `toycoronagraph-1.0/setup.py`

 * *Files identical despite different names*

