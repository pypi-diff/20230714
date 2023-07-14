# Comparing `tmp/vum-1.0.0.0.tar.gz` & `tmp/vum-1.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vum-1.0.0.0.tar", last modified: Fri Jul 14 08:31:03 2023, max compression
+gzip compressed data, was "vum-1.0.0.1.tar", last modified: Fri Jul 14 09:00:06 2023, max compression
```

## Comparing `vum-1.0.0.0.tar` & `vum-1.0.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2023-07-14 08:31:03.608229 vum-1.0.0.0/
--rw-r--r--   0 jon        (501) staff       (20)      366 2023-07-14 08:31:03.607997 vum-1.0.0.0/PKG-INFO
--rw-r--r--   0 jon        (501) staff       (20)      198 2023-05-08 10:58:22.000000 vum-1.0.0.0/README.md
--rw-r--r--   0 jon        (501) staff       (20)       38 2023-07-14 08:31:03.608326 vum-1.0.0.0/setup.cfg
--rw-r--r--   0 jon        (501) staff       (20)      550 2023-07-14 08:25:48.000000 vum-1.0.0.0/setup.py
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2023-07-14 08:31:03.606200 vum-1.0.0.0/vum/
--rw-r--r--   0 jon        (501) staff       (20)      208 2023-05-08 12:45:27.000000 vum-1.0.0.0/vum/__init__.py
--rw-r--r--   0 jon        (501) staff       (20)    14414 2023-06-28 03:48:50.000000 vum-1.0.0.0/vum/vum.py
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2023-07-14 08:31:03.607615 vum-1.0.0.0/vum.egg-info/
--rw-r--r--   0 jon        (501) staff       (20)      366 2023-07-14 08:31:03.000000 vum-1.0.0.0/vum.egg-info/PKG-INFO
--rw-r--r--   0 jon        (501) staff       (20)      153 2023-07-14 08:31:03.000000 vum-1.0.0.0/vum.egg-info/SOURCES.txt
--rw-r--r--   0 jon        (501) staff       (20)        1 2023-07-14 08:31:03.000000 vum-1.0.0.0/vum.egg-info/dependency_links.txt
--rw-r--r--   0 jon        (501) staff       (20)        4 2023-07-14 08:31:03.000000 vum-1.0.0.0/vum.egg-info/top_level.txt
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2023-07-14 09:00:06.689235 vum-1.0.0.1/
+-rw-r--r--   0 jon        (501) staff       (20)      366 2023-07-14 09:00:06.689008 vum-1.0.0.1/PKG-INFO
+-rw-r--r--   0 jon        (501) staff       (20)      198 2023-05-08 10:58:22.000000 vum-1.0.0.1/README.md
+-rw-r--r--   0 jon        (501) staff       (20)       38 2023-07-14 09:00:06.689326 vum-1.0.0.1/setup.cfg
+-rw-r--r--   0 jon        (501) staff       (20)      550 2023-07-14 08:59:09.000000 vum-1.0.0.1/setup.py
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2023-07-14 09:00:06.687575 vum-1.0.0.1/vum/
+-rw-r--r--   0 jon        (501) staff       (20)      209 2023-07-14 08:59:23.000000 vum-1.0.0.1/vum/__init__.py
+-rw-r--r--   0 jon        (501) staff       (20)    14450 2023-07-14 08:56:27.000000 vum-1.0.0.1/vum/vum.py
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2023-07-14 09:00:06.688660 vum-1.0.0.1/vum.egg-info/
+-rw-r--r--   0 jon        (501) staff       (20)      366 2023-07-14 09:00:06.000000 vum-1.0.0.1/vum.egg-info/PKG-INFO
+-rw-r--r--   0 jon        (501) staff       (20)      153 2023-07-14 09:00:06.000000 vum-1.0.0.1/vum.egg-info/SOURCES.txt
+-rw-r--r--   0 jon        (501) staff       (20)        1 2023-07-14 09:00:06.000000 vum-1.0.0.1/vum.egg-info/dependency_links.txt
+-rw-r--r--   0 jon        (501) staff       (20)        4 2023-07-14 09:00:06.000000 vum-1.0.0.1/vum.egg-info/top_level.txt
```

### Comparing `vum-1.0.0.0/setup.py` & `vum-1.0.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name = 'vum',
-    version = '1.0.0.0',    
+    version = '1.0.0.1',    
     description = 'A simple UI with curses',
     # long_description = long_description,
     url = 'https://github.com/GaffaSnobb/vum',
     author = ['Jon Kristian Dahl',],
     author_email = 'jonkd@uio.no',
     packages = ['vum'],
     install_requires = [],
```

### Comparing `vum-1.0.0.0/vum/vum.py` & `vum-1.0.0.1/vum/vum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 import curses, time
 from typing import Callable
 
 KEY_RETURN: int = 10
 KEY_BACKSPACE: int = 127
 KEY_TAB: int = 9
 
@@ -344,8 +345,8 @@
     def endwin(self):
         curses.endwin()
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
-        curses.endwin()
+        curses.endwin()
```

