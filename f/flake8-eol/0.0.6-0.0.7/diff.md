# Comparing `tmp/flake8-eol-0.0.6.tar.gz` & `tmp/flake8-eol-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-eol-0.0.6.tar", last modified: Fri Jul 14 16:51:18 2023, max compression
+gzip compressed data, was "flake8-eol-0.0.7.tar", last modified: Fri Jul 14 16:53:14 2023, max compression
```

## Comparing `flake8-eol-0.0.6.tar` & `flake8-eol-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2023-07-14 16:51:18.136693 flake8-eol-0.0.6/
--rw-rw-r--   0 water     (1000) water     (1000)      836 2023-07-14 16:51:18.136693 flake8-eol-0.0.6/PKG-INFO
--rw-rw-r--   0 water     (1000) water     (1000)      214 2023-07-14 16:14:24.000000 flake8-eol-0.0.6/README.md
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2023-07-14 16:51:18.136693 flake8-eol-0.0.6/flake8_eol.egg-info/
--rw-rw-r--   0 water     (1000) water     (1000)      836 2023-07-14 16:51:18.000000 flake8-eol-0.0.6/flake8_eol.egg-info/PKG-INFO
--rw-rw-r--   0 water     (1000) water     (1000)      234 2023-07-14 16:51:18.000000 flake8-eol-0.0.6/flake8_eol.egg-info/SOURCES.txt
--rw-rw-r--   0 water     (1000) water     (1000)        1 2023-07-14 16:51:18.000000 flake8-eol-0.0.6/flake8_eol.egg-info/dependency_links.txt
--rw-rw-r--   0 water     (1000) water     (1000)       47 2023-07-14 16:51:18.000000 flake8-eol-0.0.6/flake8_eol.egg-info/entry_points.txt
--rw-rw-r--   0 water     (1000) water     (1000)       14 2023-07-14 16:51:18.000000 flake8-eol-0.0.6/flake8_eol.egg-info/requires.txt
--rw-rw-r--   0 water     (1000) water     (1000)       11 2023-07-14 16:51:18.000000 flake8-eol-0.0.6/flake8_eol.egg-info/top_level.txt
--rw-rw-r--   0 water     (1000) water     (1000)      207 2023-07-14 16:51:18.136693 flake8-eol-0.0.6/setup.cfg
--rw-rw-r--   0 water     (1000) water     (1000)      725 2023-07-14 16:51:10.000000 flake8-eol-0.0.6/setup.py
+drwxrwxr-x   0 water     (1000) water     (1000)        0 2023-07-14 16:53:14.532539 flake8-eol-0.0.7/
+-rw-rw-r--   0 water     (1000) water     (1000)      836 2023-07-14 16:53:14.532539 flake8-eol-0.0.7/PKG-INFO
+-rw-rw-r--   0 water     (1000) water     (1000)      214 2023-07-14 16:14:24.000000 flake8-eol-0.0.7/README.md
+drwxrwxr-x   0 water     (1000) water     (1000)        0 2023-07-14 16:53:14.532539 flake8-eol-0.0.7/flake8_eol/
+drwxrwxr-x   0 water     (1000) water     (1000)        0 2023-07-14 16:53:14.532539 flake8-eol-0.0.7/flake8_eol/flake8_eol.egg-info/
+-rw-rw-r--   0 water     (1000) water     (1000)      836 2023-07-14 16:53:14.000000 flake8-eol-0.0.7/flake8_eol/flake8_eol.egg-info/PKG-INFO
+-rw-rw-r--   0 water     (1000) water     (1000)      325 2023-07-14 16:53:14.000000 flake8-eol-0.0.7/flake8_eol/flake8_eol.egg-info/SOURCES.txt
+-rw-rw-r--   0 water     (1000) water     (1000)        1 2023-07-14 16:53:14.000000 flake8-eol-0.0.7/flake8_eol/flake8_eol.egg-info/dependency_links.txt
+-rw-rw-r--   0 water     (1000) water     (1000)       47 2023-07-14 16:53:14.000000 flake8-eol-0.0.7/flake8_eol/flake8_eol.egg-info/entry_points.txt
+-rw-rw-r--   0 water     (1000) water     (1000)       14 2023-07-14 16:53:14.000000 flake8-eol-0.0.7/flake8_eol/flake8_eol.egg-info/requires.txt
+-rw-rw-r--   0 water     (1000) water     (1000)       11 2023-07-14 16:53:14.000000 flake8-eol-0.0.7/flake8_eol/flake8_eol.egg-info/top_level.txt
+-rw-rw-r--   0 water     (1000) water     (1000)      725 2023-07-14 16:42:38.000000 flake8-eol-0.0.7/flake8_eol/flake8_eol.py
+-rw-rw-r--   0 water     (1000) water     (1000)      297 2023-07-14 16:53:14.532539 flake8-eol-0.0.7/setup.cfg
+-rw-rw-r--   0 water     (1000) water     (1000)      725 2023-07-14 16:52:59.000000 flake8-eol-0.0.7/setup.py
```

### Comparing `flake8-eol-0.0.6/PKG-INFO` & `flake8-eol-0.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-eol
-Version: 0.0.6
+Version: 0.0.7
 Summary: Flake8 plugin to enforce EOL consistency
 Author: Claudio Scheer
 Author-email: claudioscheer@protonmail.com
 Classifier: Framework :: Flake8
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flake8-eol-0.0.6/flake8_eol.egg-info/PKG-INFO` & `flake8-eol-0.0.7/flake8_eol/flake8_eol.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-eol
-Version: 0.0.6
+Version: 0.0.7
 Summary: Flake8 plugin to enforce EOL consistency
 Author: Claudio Scheer
 Author-email: claudioscheer@protonmail.com
 Classifier: Framework :: Flake8
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flake8-eol-0.0.6/setup.py` & `flake8-eol-0.0.7/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name="flake8-eol",
-    version="0.0.6",
+    version="0.0.7",
     author="Claudio Scheer",
     author_email="claudioscheer@protonmail.com",
     description="Flake8 plugin to enforce EOL consistency",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     classifiers=[
         "Framework :: Flake8",
```

