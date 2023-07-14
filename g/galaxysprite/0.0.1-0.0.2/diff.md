# Comparing `tmp/galaxysprite-0.0.1.tar.gz` & `tmp/galaxysprite-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/marxena/Desktop/galaxysprite/dist/.tmp-e_z02q14/galaxysprite-0.0.1.tar", last modified: Thu Jul 13 21:29:10 2023, max compression
+gzip compressed data, was "galaxysprite-0.0.2.tar", last modified: Fri Jul 14 16:50:40 2023, max compression
```

## Comparing `galaxysprite-0.0.1.tar` & `galaxysprite-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,20 @@
-drwxr-xr-x   0 marxena    (502) staff       (20)        0 2023-07-13 21:29:10.223960 galaxysprite-0.0.1/
--rw-r--r--   0 marxena    (502) staff       (20)      107 2023-07-13 21:29:10.223629 galaxysprite-0.0.1/PKG-INFO
--rw-r--r--   0 marxena    (502) staff       (20)      758 2023-07-13 21:24:37.000000 galaxysprite-0.0.1/README.md
-drwxr-xr-x   0 marxena    (502) staff       (20)        0 2023-07-13 21:29:10.223182 galaxysprite-0.0.1/galaxysprite.egg-info/
--rw-r--r--   0 marxena    (502) staff       (20)      107 2023-07-13 21:29:10.000000 galaxysprite-0.0.1/galaxysprite.egg-info/PKG-INFO
--rw-r--r--   0 marxena    (502) staff       (20)      162 2023-07-13 21:29:10.000000 galaxysprite-0.0.1/galaxysprite.egg-info/SOURCES.txt
--rw-r--r--   0 marxena    (502) staff       (20)        1 2023-07-13 21:29:10.000000 galaxysprite-0.0.1/galaxysprite.egg-info/dependency_links.txt
--rw-r--r--   0 marxena    (502) staff       (20)        1 2023-07-13 21:29:10.000000 galaxysprite-0.0.1/galaxysprite.egg-info/top_level.txt
--rw-r--r--   0 marxena    (502) staff       (20)       38 2023-07-13 21:29:10.224088 galaxysprite-0.0.1/setup.cfg
--rw-r--r--   0 marxena    (502) staff       (20)      184 2023-07-13 21:24:37.000000 galaxysprite-0.0.1/setup.py
+drwxr-xr-x   0 marxena    (502) staff       (20)        0 2023-07-14 16:50:40.335757 galaxysprite-0.0.2/
+-rw-r--r--   0 marxena    (502) staff       (20)     1338 2023-07-14 16:47:22.000000 galaxysprite-0.0.2/LICENSE
+-rw-r--r--   0 marxena    (502) staff       (20)      222 2023-07-14 16:50:40.335373 galaxysprite-0.0.2/PKG-INFO
+-rw-r--r--   0 marxena    (502) staff       (20)      864 2023-07-13 22:02:09.000000 galaxysprite-0.0.2/README.md
+drwxr-xr-x   0 marxena    (502) staff       (20)        0 2023-07-14 16:50:40.329280 galaxysprite-0.0.2/galaxysprite/
+-rw-r--r--   0 marxena    (502) staff       (20)       59 2023-07-14 16:36:31.000000 galaxysprite-0.0.2/galaxysprite/__init__.py
+drwxr-xr-x   0 marxena    (502) staff       (20)        0 2023-07-14 16:50:40.334441 galaxysprite-0.0.2/galaxysprite/src/
+-rw-r--r--   0 marxena    (502) staff       (20)        0 2023-07-14 16:36:02.000000 galaxysprite-0.0.2/galaxysprite/src/__init__.py
+-rw-r--r--   0 marxena    (502) staff       (20)     1144 2023-07-13 21:07:06.000000 galaxysprite-0.0.2/galaxysprite/src/compressor.py
+-rw-r--r--   0 marxena    (502) staff       (20)     3968 2023-07-13 21:07:06.000000 galaxysprite-0.0.2/galaxysprite/src/density.py
+-rw-r--r--   0 marxena    (502) staff       (20)      551 2023-07-13 21:07:06.000000 galaxysprite-0.0.2/galaxysprite/src/galactic.py
+-rw-r--r--   0 marxena    (502) staff       (20)     2011 2023-07-10 21:36:16.000000 galaxysprite-0.0.2/galaxysprite/src/main.py
+drwxr-xr-x   0 marxena    (502) staff       (20)        0 2023-07-14 16:50:40.331571 galaxysprite-0.0.2/galaxysprite.egg-info/
+-rw-r--r--   0 marxena    (502) staff       (20)      222 2023-07-14 16:50:40.000000 galaxysprite-0.0.2/galaxysprite.egg-info/PKG-INFO
+-rw-r--r--   0 marxena    (502) staff       (20)      372 2023-07-14 16:50:40.000000 galaxysprite-0.0.2/galaxysprite.egg-info/SOURCES.txt
+-rw-r--r--   0 marxena    (502) staff       (20)        1 2023-07-14 16:50:40.000000 galaxysprite-0.0.2/galaxysprite.egg-info/dependency_links.txt
+-rw-r--r--   0 marxena    (502) staff       (20)       38 2023-07-14 16:50:40.000000 galaxysprite-0.0.2/galaxysprite.egg-info/requires.txt
+-rw-r--r--   0 marxena    (502) staff       (20)       13 2023-07-14 16:50:40.000000 galaxysprite-0.0.2/galaxysprite.egg-info/top_level.txt
+-rw-r--r--   0 marxena    (502) staff       (20)       38 2023-07-14 16:50:40.335886 galaxysprite-0.0.2/setup.cfg
+-rw-r--r--   0 marxena    (502) staff       (20)      825 2023-07-14 16:50:27.000000 galaxysprite-0.0.2/setup.py
```

