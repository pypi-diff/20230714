# Comparing `tmp/clipcraft-1.0.tar.gz` & `tmp/clipcraft-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipcraft-1.0.tar", last modified: Wed Jul 12 13:47:01 2023, max compression
+gzip compressed data, was "clipcraft-1.1.tar", last modified: Fri Jul 14 14:46:43 2023, max compression
```

## Comparing `clipcraft-1.0.tar` & `clipcraft-1.1.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 13:47:01.207599 clipcraft-1.0/
--rw-rw-rw-   0        0        0      116 2023-07-12 13:47:01.206596 clipcraft-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-12 13:47:01.188589 clipcraft-1.0/clipcraft/
--rw-rw-rw-   0        0        0        0 2023-07-07 19:15:00.000000 clipcraft-1.0/clipcraft/__init__.py
--rw-rw-rw-   0        0        0    11714 2023-07-07 20:34:27.000000 clipcraft-1.0/clipcraft/clipcraft.py
-drwxrwxrwx   0        0        0        0 2023-07-12 13:47:01.204594 clipcraft-1.0/clipcraft.egg-info/
--rw-rw-rw-   0        0        0      116 2023-07-12 13:47:01.000000 clipcraft-1.0/clipcraft.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-07-12 13:47:01.000000 clipcraft-1.0/clipcraft.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 13:47:01.000000 clipcraft-1.0/clipcraft.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-07-12 13:47:01.000000 clipcraft-1.0/clipcraft.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-12 13:47:01.000000 clipcraft-1.0/clipcraft.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 13:47:01.207599 clipcraft-1.0/setup.cfg
--rw-rw-rw-   0        0        0      302 2023-07-07 19:15:00.000000 clipcraft-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 14:46:43.603839 clipcraft-1.1/
+-rw-rw-rw-   0        0        0     3581 2023-07-14 14:46:43.603839 clipcraft-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3242 2023-07-14 14:35:14.000000 clipcraft-1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 14:46:43.574205 clipcraft-1.1/clipcraft/
+-rw-rw-rw-   0        0        0      128 2023-07-14 14:35:14.000000 clipcraft-1.1/clipcraft/__init__.py
+-rw-rw-rw-   0        0        0     8166 2023-07-14 14:35:14.000000 clipcraft-1.1/clipcraft/create_embeddings.py
+-rw-rw-rw-   0        0        0     3533 2023-07-14 14:35:14.000000 clipcraft-1.1/clipcraft/knn_search.py
+drwxrwxrwx   0        0        0        0 2023-07-14 14:46:43.600023 clipcraft-1.1/clipcraft.egg-info/
+-rw-rw-rw-   0        0        0     3581 2023-07-14 14:46:43.000000 clipcraft-1.1/clipcraft.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-07-14 14:46:43.000000 clipcraft-1.1/clipcraft.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 14:46:43.000000 clipcraft-1.1/clipcraft.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-07-14 14:46:43.000000 clipcraft-1.1/clipcraft.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-14 14:46:43.000000 clipcraft-1.1/clipcraft.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 14:46:43.603839 clipcraft-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      640 2023-07-14 14:45:44.000000 clipcraft-1.1/setup.py
```

