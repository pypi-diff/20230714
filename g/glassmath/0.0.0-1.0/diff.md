# Comparing `tmp/glassmath-0.0.0.tar.gz` & `tmp/glassmath-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glassmath-0.0.0.tar", last modified: Fri Jul 14 06:27:16 2023, max compression
+gzip compressed data, was "glassmath-1.0.tar", last modified: Fri Jul 14 06:20:19 2023, max compression
```

## Comparing `glassmath-0.0.0.tar` & `glassmath-1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 06:27:16.519506 glassmath-0.0.0/
--rw-rw-rw-   0        0        0      801 2023-07-14 06:19:58.000000 glassmath-0.0.0/LICENSE
--rw-rw-rw-   0        0        0      202 2023-07-14 06:27:16.515511 glassmath-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-07-14 06:19:20.000000 glassmath-0.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 06:27:16.488527 glassmath-0.0.0/glassmath/
--rw-rw-rw-   0        0        0        0 2023-07-14 00:50:41.000000 glassmath-0.0.0/glassmath/__init__.py
--rw-rw-rw-   0        0        0     6960 2023-07-14 01:05:11.000000 glassmath-0.0.0/glassmath/calcplus.py
-drwxrwxrwx   0        0        0        0 2023-07-14 06:27:16.511506 glassmath-0.0.0/glassmath.egg-info/
--rw-rw-rw-   0        0        0      202 2023-07-14 06:27:16.000000 glassmath-0.0.0/glassmath.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-07-14 06:27:16.000000 glassmath-0.0.0/glassmath.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 06:27:16.000000 glassmath-0.0.0/glassmath.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-14 06:27:16.000000 glassmath-0.0.0/glassmath.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 06:27:16.520506 glassmath-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      340 2023-07-14 06:27:01.000000 glassmath-0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 06:20:19.202818 glassmath-1.0/
+-rw-rw-rw-   0        0        0      801 2023-07-14 06:19:58.000000 glassmath-1.0/LICENSE
+-rw-rw-rw-   0        0        0      200 2023-07-14 06:20:19.199815 glassmath-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-07-14 06:19:20.000000 glassmath-1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 06:20:19.177815 glassmath-1.0/calcplus/
+-rw-rw-rw-   0        0        0        0 2023-07-14 00:50:41.000000 glassmath-1.0/calcplus/__init__.py
+-rw-rw-rw-   0        0        0     6960 2023-07-14 01:05:11.000000 glassmath-1.0/calcplus/calcplus.py
+drwxrwxrwx   0        0        0        0 2023-07-14 06:20:19.196822 glassmath-1.0/glassmath.egg-info/
+-rw-rw-rw-   0        0        0      200 2023-07-14 06:20:18.000000 glassmath-1.0/glassmath.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2023-07-14 06:20:19.000000 glassmath-1.0/glassmath.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 06:20:18.000000 glassmath-1.0/glassmath.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-14 06:20:18.000000 glassmath-1.0/glassmath.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 06:20:19.202818 glassmath-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      360 2023-07-14 06:18:47.000000 glassmath-1.0/setup.py
```

### Comparing `glassmath-0.0.0/LICENSE` & `glassmath-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glassmath-0.0.0/glassmath/calcplus.py` & `glassmath-1.0/calcplus/calcplus.py`

 * *Files identical despite different names*

