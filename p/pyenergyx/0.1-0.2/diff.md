# Comparing `tmp/pyenergyx-0.1.tar.gz` & `tmp/pyenergyx-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyenergyx-0.1.tar", last modified: Fri Jul 14 19:30:23 2023, max compression
+gzip compressed data, was "dist/pyenergyx-0.2.tar", last modified: Fri Jul 14 19:37:20 2023, max compression
```

## Comparing `pyenergyx-0.1.tar` & `pyenergyx-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 Mario      (501) staff       (20)        0 2023-07-14 19:30:23.064272 pyenergyx-0.1/
--rw-r--r--   0 Mario      (501) staff       (20)     1058 2023-07-13 10:03:30.000000 pyenergyx-0.1/LICENSE
--rw-r--r--   0 Mario      (501) staff       (20)      856 2023-07-14 19:30:23.063650 pyenergyx-0.1/PKG-INFO
--rw-r--r--   0 Mario      (501) staff       (20)      234 2023-07-13 10:03:30.000000 pyenergyx-0.1/README.md
-drwxr-xr-x   0 Mario      (501) staff       (20)        0 2023-07-14 19:30:23.058375 pyenergyx-0.1/pyenergyx/
--rw-r--r--   0 Mario      (501) staff       (20)        0 2023-07-13 10:03:30.000000 pyenergyx-0.1/pyenergyx/__init__.py
--rw-r--r--   0 Mario      (501) staff       (20)     3825 2023-07-14 06:57:09.000000 pyenergyx-0.1/pyenergyx/pyenergyx.py
-drwxr-xr-x   0 Mario      (501) staff       (20)        0 2023-07-14 19:30:23.062677 pyenergyx-0.1/pyenergyx.egg-info/
--rw-r--r--   0 Mario      (501) staff       (20)      856 2023-07-14 19:30:22.000000 pyenergyx-0.1/pyenergyx.egg-info/PKG-INFO
--rw-r--r--   0 Mario      (501) staff       (20)      203 2023-07-14 19:30:23.000000 pyenergyx-0.1/pyenergyx.egg-info/SOURCES.txt
--rw-r--r--   0 Mario      (501) staff       (20)        1 2023-07-14 19:30:22.000000 pyenergyx-0.1/pyenergyx.egg-info/dependency_links.txt
--rw-r--r--   0 Mario      (501) staff       (20)       10 2023-07-14 19:30:22.000000 pyenergyx-0.1/pyenergyx.egg-info/top_level.txt
--rw-r--r--   0 Mario      (501) staff       (20)       38 2023-07-14 19:30:23.064435 pyenergyx-0.1/setup.cfg
--rw-r--r--   0 Mario      (501) staff       (20)      776 2023-07-13 10:03:30.000000 pyenergyx-0.1/setup.py
+drwxr-xr-x   0 Mario      (501) staff       (20)        0 2023-07-14 19:37:20.517082 pyenergyx-0.2/
+-rw-r--r--   0 Mario      (501) staff       (20)     1058 2023-07-13 10:03:30.000000 pyenergyx-0.2/LICENSE
+-rw-r--r--   0 Mario      (501) staff       (20)     2367 2023-07-14 19:37:20.516577 pyenergyx-0.2/PKG-INFO
+-rw-r--r--   0 Mario      (501) staff       (20)     1745 2023-07-14 19:33:11.000000 pyenergyx-0.2/README.md
+drwxr-xr-x   0 Mario      (501) staff       (20)        0 2023-07-14 19:37:20.511410 pyenergyx-0.2/pyenergyx/
+-rw-r--r--   0 Mario      (501) staff       (20)        0 2023-07-13 10:03:30.000000 pyenergyx-0.2/pyenergyx/__init__.py
+-rw-r--r--   0 Mario      (501) staff       (20)     3825 2023-07-14 06:57:09.000000 pyenergyx-0.2/pyenergyx/pyenergyx.py
+drwxr-xr-x   0 Mario      (501) staff       (20)        0 2023-07-14 19:37:20.515914 pyenergyx-0.2/pyenergyx.egg-info/
+-rw-r--r--   0 Mario      (501) staff       (20)     2367 2023-07-14 19:37:20.000000 pyenergyx-0.2/pyenergyx.egg-info/PKG-INFO
+-rw-r--r--   0 Mario      (501) staff       (20)      203 2023-07-14 19:37:20.000000 pyenergyx-0.2/pyenergyx.egg-info/SOURCES.txt
+-rw-r--r--   0 Mario      (501) staff       (20)        1 2023-07-14 19:37:20.000000 pyenergyx-0.2/pyenergyx.egg-info/dependency_links.txt
+-rw-r--r--   0 Mario      (501) staff       (20)       10 2023-07-14 19:37:20.000000 pyenergyx-0.2/pyenergyx.egg-info/top_level.txt
+-rw-r--r--   0 Mario      (501) staff       (20)       38 2023-07-14 19:37:20.517259 pyenergyx-0.2/setup.cfg
+-rw-r--r--   0 Mario      (501) staff       (20)      776 2023-07-14 19:37:11.000000 pyenergyx-0.2/setup.py
```

### Comparing `pyenergyx-0.1/LICENSE` & `pyenergyx-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyenergyx-0.1/pyenergyx/pyenergyx.py` & `pyenergyx-0.2/pyenergyx/pyenergyx.py`

 * *Files identical despite different names*

### Comparing `pyenergyx-0.1/setup.py` & `pyenergyx-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pyenergyx', 
-    version='0.1', 
+    version='0.2', 
     packages=find_packages(),
     description='A simple energy conversion library',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Mario David Gonzalez Ronda', 
     author_email='mariodgr@protonmail.com', 
     url='https://github.com/mariodgr/pyenergyx',
```

