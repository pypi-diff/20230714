# Comparing `tmp/flake8-eol-0.0.3.tar.gz` & `tmp/flake8-eol-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-eol-0.0.3.tar", last modified: Fri Jul 14 16:21:27 2023, max compression
+gzip compressed data, was "flake8-eol-0.0.4.tar", last modified: Fri Jul 14 16:45:16 2023, max compression
```

## Comparing `flake8-eol-0.0.3.tar` & `flake8-eol-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2023-07-14 16:21:27.947052 flake8-eol-0.0.3/
--rw-rw-r--   0 water     (1000) water     (1000)      724 2023-07-14 16:21:27.947052 flake8-eol-0.0.3/PKG-INFO
--rw-rw-r--   0 water     (1000) water     (1000)      214 2023-07-14 16:14:24.000000 flake8-eol-0.0.3/README.md
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2023-07-14 16:21:27.947052 flake8-eol-0.0.3/flake8_eol/
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2023-07-14 16:21:27.947052 flake8-eol-0.0.3/flake8_eol/flake8_eol.egg-info/
--rw-rw-r--   0 water     (1000) water     (1000)      724 2023-07-14 16:21:27.000000 flake8-eol-0.0.3/flake8_eol/flake8_eol.egg-info/PKG-INFO
--rw-rw-r--   0 water     (1000) water     (1000)      325 2023-07-14 16:21:27.000000 flake8-eol-0.0.3/flake8_eol/flake8_eol.egg-info/SOURCES.txt
--rw-rw-r--   0 water     (1000) water     (1000)        1 2023-07-14 16:21:27.000000 flake8-eol-0.0.3/flake8_eol/flake8_eol.egg-info/dependency_links.txt
--rw-rw-r--   0 water     (1000) water     (1000)       58 2023-07-14 16:21:27.000000 flake8-eol-0.0.3/flake8_eol/flake8_eol.egg-info/entry_points.txt
--rw-rw-r--   0 water     (1000) water     (1000)        7 2023-07-14 16:21:27.000000 flake8-eol-0.0.3/flake8_eol/flake8_eol.egg-info/requires.txt
--rw-rw-r--   0 water     (1000) water     (1000)       11 2023-07-14 16:21:27.000000 flake8-eol-0.0.3/flake8_eol/flake8_eol.egg-info/top_level.txt
--rw-rw-r--   0 water     (1000) water     (1000)      801 2023-07-14 16:20:27.000000 flake8-eol-0.0.3/flake8_eol/flake8_eol.py
--rw-rw-r--   0 water     (1000) water     (1000)      754 2023-07-14 16:21:27.947052 flake8-eol-0.0.3/setup.cfg
--rw-rw-r--   0 water     (1000) water     (1000)      615 2023-07-14 16:21:19.000000 flake8-eol-0.0.3/setup.py
+drwxrwxr-x   0 water     (1000) water     (1000)        0 2023-07-14 16:45:16.723123 flake8-eol-0.0.4/
+-rw-rw-r--   0 water     (1000) water     (1000)      836 2023-07-14 16:45:16.723123 flake8-eol-0.0.4/PKG-INFO
+-rw-rw-r--   0 water     (1000) water     (1000)      214 2023-07-14 16:14:24.000000 flake8-eol-0.0.4/README.md
+drwxrwxr-x   0 water     (1000) water     (1000)        0 2023-07-14 16:45:16.723123 flake8-eol-0.0.4/flake8_eol/
+drwxrwxr-x   0 water     (1000) water     (1000)        0 2023-07-14 16:45:16.723123 flake8-eol-0.0.4/flake8_eol/flake8_eol.egg-info/
+-rw-rw-r--   0 water     (1000) water     (1000)      836 2023-07-14 16:45:16.000000 flake8-eol-0.0.4/flake8_eol/flake8_eol.egg-info/PKG-INFO
+-rw-rw-r--   0 water     (1000) water     (1000)      325 2023-07-14 16:45:16.000000 flake8-eol-0.0.4/flake8_eol/flake8_eol.egg-info/SOURCES.txt
+-rw-rw-r--   0 water     (1000) water     (1000)        1 2023-07-14 16:45:16.000000 flake8-eol-0.0.4/flake8_eol/flake8_eol.egg-info/dependency_links.txt
+-rw-rw-r--   0 water     (1000) water     (1000)       58 2023-07-14 16:45:16.000000 flake8-eol-0.0.4/flake8_eol/flake8_eol.egg-info/entry_points.txt
+-rw-rw-r--   0 water     (1000) water     (1000)       14 2023-07-14 16:45:16.000000 flake8-eol-0.0.4/flake8_eol/flake8_eol.egg-info/requires.txt
+-rw-rw-r--   0 water     (1000) water     (1000)       11 2023-07-14 16:45:16.000000 flake8-eol-0.0.4/flake8_eol/flake8_eol.egg-info/top_level.txt
+-rw-rw-r--   0 water     (1000) water     (1000)      725 2023-07-14 16:42:38.000000 flake8-eol-0.0.4/flake8_eol/flake8_eol.py
+-rw-rw-r--   0 water     (1000) water     (1000)      308 2023-07-14 16:45:16.723123 flake8-eol-0.0.4/setup.cfg
+-rw-rw-r--   0 water     (1000) water     (1000)      725 2023-07-14 16:39:04.000000 flake8-eol-0.0.4/setup.py
```

### Comparing `flake8-eol-0.0.3/flake8_eol/flake8_eol.py` & `flake8-eol-0.0.4/flake8_eol/flake8_eol.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,10 @@
 import ast
-import sys
 from typing import Any, Generator, Tuple, Type
-
-if sys.version_info < (3, 8):
-    import importlib_metadata
-else:
-    import importlib.metadata as importlib_metadata
+import importlib.metadata as importlib_metadata
 
 
 class EOLChecker:
     name = "flake8-eol"
     version = importlib_metadata.version(name)
 
     def __init__(self, tree: ast.AST, filename: str) -> None:
@@ -19,10 +14,10 @@
     def run(self) -> Generator[Tuple[int, int, str, Type[Any]], None, None]:
         with open(self.filename, "rb") as f:
             first_line = f.readline()
             if first_line.endswith(b"\r\n"):
                 yield (
                     1,
                     1,
-                    "EOL001 '\\r\\n' at the end of the line is incorrect",
+                    "EOL001 replace '\\r\\n' at the end of the line with '\\n'",
                     type(self),
                 )
```

### Comparing `flake8-eol-0.0.3/setup.py` & `flake8-eol-0.0.4/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from setuptools import setup
 
+
 setup(
     name="flake8-eol",
-    version="0.0.3",
+    version="0.0.4",
+    author="Claudio Scheer",
+    author_email="claudioscheer@protonmail.com",
     description="Flake8 plugin to enforce EOL consistency",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
-    url="https://github.com/claudioscheer/flake8-eol",
-    author="Claudio Scheer",
-    author_email="claudioscheer@protonmail.com",
-    install_requires=["flake8"],
     classifiers=[
         "Framework :: Flake8",
+        "Environment :: Console",
         "Intended Audience :: Developers",
-        "Topic :: Software Development :: Quality Assurance",
         "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+        "Topic :: Software Development :: Quality Assurance",
     ],
 )
```

