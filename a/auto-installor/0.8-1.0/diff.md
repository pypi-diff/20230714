# Comparing `tmp/auto-installor-0.8.tar.gz` & `tmp/auto-installor-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\auto-installor-0.8.tar", last modified: Thu Jul 13 23:19:24 2023, max compression
+gzip compressed data, was "dist\auto-installor-1.0.tar", last modified: Thu Jul 13 23:13:39 2023, max compression
```

## Comparing `auto-installor-0.8.tar` & `auto-installor-1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 23:19:24.000000 auto-installor-0.8/
--rw-rw-rw-   0        0        0      196 2023-07-13 23:19:24.000000 auto-installor-0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-13 23:19:24.000000 auto-installor-0.8/auto_installor.egg-info/
--rw-rw-rw-   0        0        0      196 2023-07-13 23:19:24.000000 auto-installor-0.8/auto_installor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-07-13 23:19:24.000000 auto-installor-0.8/auto_installor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 23:19:24.000000 auto-installor-0.8/auto_installor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-13 23:19:24.000000 auto-installor-0.8/auto_installor.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      251 2023-07-13 23:19:24.000000 auto-installor-0.8/auto_installor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 23:19:24.000000 auto-installor-0.8/auto_installor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 23:19:24.000000 auto-installor-0.8/setup.cfg
--rw-rw-rw-   0        0        0      641 2023-07-13 23:18:30.000000 auto-installor-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 23:13:39.000000 auto-installor-1.0/
+-rw-rw-rw-   0        0        0      196 2023-07-13 23:13:39.000000 auto-installor-1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-13 23:13:39.000000 auto-installor-1.0/auto_installor.egg-info/
+-rw-rw-rw-   0        0        0      196 2023-07-13 23:13:39.000000 auto-installor-1.0/auto_installor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-07-13 23:13:39.000000 auto-installor-1.0/auto_installor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 23:13:39.000000 auto-installor-1.0/auto_installor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-13 23:13:39.000000 auto-installor-1.0/auto_installor.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      251 2023-07-13 23:13:39.000000 auto-installor-1.0/auto_installor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 23:13:39.000000 auto-installor-1.0/auto_installor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 23:13:39.000000 auto-installor-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      641 2023-07-13 23:13:13.000000 auto-installor-1.0/setup.py
```

### Comparing `auto-installor-0.8/setup.py` & `auto-installor-1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="auto-installor",
-    version='0.8',
+    version='1.0',
     packages=find_packages(),
     package_data={'utils': ['*']},
     install_requires=[
     'click==8.1.4',
     'colorama==0.4.6',
     'importlib-metadata==6.7.0',
     'pip==23.1.2',
```

