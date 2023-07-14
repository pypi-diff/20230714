# Comparing `tmp/flake8-eol-0.0.1.tar.gz` & `tmp/flake8-eol-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-eol-0.0.1.tar", last modified: Fri Jul 14 14:27:19 2023, max compression
+gzip compressed data, was "flake8-eol-0.0.2.tar", last modified: Fri Jul 14 14:38:43 2023, max compression
```

## Comparing `flake8-eol-0.0.1.tar` & `flake8-eol-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2023-07-14 14:27:19.392990 flake8-eol-0.0.1/
--rw-rw-r--   0 water     (1000) water     (1000)      566 2023-07-14 14:27:19.392990 flake8-eol-0.0.1/PKG-INFO
--rw-rw-r--   0 water     (1000) water     (1000)       56 2023-07-14 14:22:27.000000 flake8-eol-0.0.1/README.md
--rw-rw-r--   0 water     (1000) water     (1000)      656 2023-07-14 14:27:19.392990 flake8-eol-0.0.1/setup.cfg
--rw-rw-r--   0 water     (1000) water     (1000)      615 2023-07-14 14:27:12.000000 flake8-eol-0.0.1/setup.py
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2023-07-14 14:27:19.392990 flake8-eol-0.0.1/src/
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2023-07-14 14:27:19.392990 flake8-eol-0.0.1/src/flake8-eol/
--rw-rw-r--   0 water     (1000) water     (1000)        0 2023-07-14 14:11:33.000000 flake8-eol-0.0.1/src/flake8-eol/__init__.py
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2023-07-14 14:27:19.392990 flake8-eol-0.0.1/src/flake8_eol.egg-info/
--rw-rw-r--   0 water     (1000) water     (1000)      566 2023-07-14 14:27:19.000000 flake8-eol-0.0.1/src/flake8_eol.egg-info/PKG-INFO
--rw-rw-r--   0 water     (1000) water     (1000)      266 2023-07-14 14:27:19.000000 flake8-eol-0.0.1/src/flake8_eol.egg-info/SOURCES.txt
--rw-rw-r--   0 water     (1000) water     (1000)        1 2023-07-14 14:27:19.000000 flake8-eol-0.0.1/src/flake8_eol.egg-info/dependency_links.txt
--rw-rw-r--   0 water     (1000) water     (1000)        7 2023-07-14 14:27:19.000000 flake8-eol-0.0.1/src/flake8_eol.egg-info/requires.txt
--rw-rw-r--   0 water     (1000) water     (1000)       28 2023-07-14 14:27:19.000000 flake8-eol-0.0.1/src/flake8_eol.egg-info/top_level.txt
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2023-07-14 14:27:19.392990 flake8-eol-0.0.1/src/tests/
--rw-rw-r--   0 water     (1000) water     (1000)        0 2023-07-14 14:11:51.000000 flake8-eol-0.0.1/src/tests/__init__.py
+drwxrwxr-x   0 water     (1000) water     (1000)        0 2023-07-14 14:38:43.909570 flake8-eol-0.0.2/
+-rw-rw-r--   0 water     (1000) water     (1000)      566 2023-07-14 14:38:43.909570 flake8-eol-0.0.2/PKG-INFO
+-rw-rw-r--   0 water     (1000) water     (1000)       56 2023-07-14 14:22:27.000000 flake8-eol-0.0.2/README.md
+-rw-rw-r--   0 water     (1000) water     (1000)      656 2023-07-14 14:38:43.909570 flake8-eol-0.0.2/setup.cfg
+-rw-rw-r--   0 water     (1000) water     (1000)      615 2023-07-14 14:38:32.000000 flake8-eol-0.0.2/setup.py
+drwxrwxr-x   0 water     (1000) water     (1000)        0 2023-07-14 14:38:43.909570 flake8-eol-0.0.2/src/
+drwxrwxr-x   0 water     (1000) water     (1000)        0 2023-07-14 14:38:43.909570 flake8-eol-0.0.2/src/flake8_eol/
+-rw-rw-r--   0 water     (1000) water     (1000)        0 2023-07-14 14:11:33.000000 flake8-eol-0.0.2/src/flake8_eol/__init__.py
+-rw-rw-r--   0 water     (1000) water     (1000)       49 2023-07-14 14:36:34.000000 flake8-eol-0.0.2/src/flake8_eol/add.py
+drwxrwxr-x   0 water     (1000) water     (1000)        0 2023-07-14 14:38:43.909570 flake8-eol-0.0.2/src/flake8_eol.egg-info/
+-rw-rw-r--   0 water     (1000) water     (1000)      566 2023-07-14 14:38:43.000000 flake8-eol-0.0.2/src/flake8_eol.egg-info/PKG-INFO
+-rw-rw-r--   0 water     (1000) water     (1000)      310 2023-07-14 14:38:43.000000 flake8-eol-0.0.2/src/flake8_eol.egg-info/SOURCES.txt
+-rw-rw-r--   0 water     (1000) water     (1000)        1 2023-07-14 14:38:43.000000 flake8-eol-0.0.2/src/flake8_eol.egg-info/dependency_links.txt
+-rw-rw-r--   0 water     (1000) water     (1000)        7 2023-07-14 14:38:43.000000 flake8-eol-0.0.2/src/flake8_eol.egg-info/requires.txt
+-rw-rw-r--   0 water     (1000) water     (1000)       17 2023-07-14 14:38:43.000000 flake8-eol-0.0.2/src/flake8_eol.egg-info/top_level.txt
+drwxrwxr-x   0 water     (1000) water     (1000)        0 2023-07-14 14:38:43.909570 flake8-eol-0.0.2/src/tests/
+-rw-rw-r--   0 water     (1000) water     (1000)        0 2023-07-14 14:11:51.000000 flake8-eol-0.0.2/src/tests/__init__.py
+-rw-rw-r--   0 water     (1000) water     (1000)      195 2023-07-14 14:36:07.000000 flake8-eol-0.0.2/src/tests/test_add.py
```

### Comparing `flake8-eol-0.0.1/PKG-INFO` & `flake8-eol-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-eol
-Version: 0.0.1
+Version: 0.0.2
 Summary: Flake8 plugin to enforce EOL consistency
 Home-page: https://github.com/claudioscheer/flake8-eol
 Author: Claudio Scheer
 Author-email: claudioscheer@protonmail.com
 Keywords: flake8,eol,line endings
 Classifier: Framework :: Flake8
 Classifier: Intended Audience :: Developers
```

### Comparing `flake8-eol-0.0.1/setup.cfg` & `flake8-eol-0.0.2/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = "flake8-eol
-version = 0.0.1
+version = 0.0.2
 description = Flake8 plugin to enforce EOL consistency
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = flake8, eol, line endings
 author = Claudio Scheer
 author_email = claudioscheer@protonmail.com
 classifiers =
```

### Comparing `flake8-eol-0.0.1/setup.py` & `flake8-eol-0.0.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="flake8-eol",
-    version="0.0.1",
+    version="0.0.2",
     description="Flake8 plugin to enforce EOL consistency",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/claudioscheer/flake8-eol",
     author="Claudio Scheer",
     author_email="claudioscheer@protonmail.com",
     install_requires=["flake8"],
```

### Comparing `flake8-eol-0.0.1/src/flake8_eol.egg-info/PKG-INFO` & `flake8-eol-0.0.2/src/flake8_eol.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-eol
-Version: 0.0.1
+Version: 0.0.2
 Summary: Flake8 plugin to enforce EOL consistency
 Home-page: https://github.com/claudioscheer/flake8-eol
 Author: Claudio Scheer
 Author-email: claudioscheer@protonmail.com
 Keywords: flake8,eol,line endings
 Classifier: Framework :: Flake8
 Classifier: Intended Audience :: Developers
```

