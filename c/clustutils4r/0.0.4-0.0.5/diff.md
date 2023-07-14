# Comparing `tmp/clustutils4r-0.0.4.tar.gz` & `tmp/clustutils4r-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clustutils4r-0.0.4.tar", last modified: Fri Jul 14 00:22:25 2023, max compression
+gzip compressed data, was "clustutils4r-0.0.5.tar", last modified: Fri Jul 14 00:29:24 2023, max compression
```

## Comparing `clustutils4r-0.0.4.tar` & `clustutils4r-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-14 00:22:25.811096 clustutils4r-0.0.4/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    35128 2023-07-13 07:56:53.000000 clustutils4r-0.0.4/LICENSE
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     3779 2023-07-14 00:22:25.811096 clustutils4r-0.0.4/PKG-INFO
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     3147 2023-07-14 00:17:31.000000 clustutils4r-0.0.4/README.md
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      659 2023-07-14 00:21:40.000000 clustutils4r-0.0.4/pyproject.toml
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       38 2023-07-14 00:22:25.811096 clustutils4r-0.0.4/setup.cfg
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      978 2023-07-14 00:21:34.000000 clustutils4r-0.0.4/setup.py
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-14 00:22:25.811096 clustutils4r-0.0.4/src/
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-14 00:22:25.811096 clustutils4r-0.0.4/src/clustutils4r/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        0 2023-07-13 05:33:28.000000 clustutils4r-0.0.4/src/clustutils4r/__init__.py
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    25231 2023-07-14 00:18:19.000000 clustutils4r-0.0.4/src/clustutils4r/eval_clustering.py
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-14 00:22:25.811096 clustutils4r-0.0.4/src/clustutils4r.egg-info/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     3779 2023-07-14 00:22:25.000000 clustutils4r-0.0.4/src/clustutils4r.egg-info/PKG-INFO
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      305 2023-07-14 00:22:25.000000 clustutils4r-0.0.4/src/clustutils4r.egg-info/SOURCES.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        1 2023-07-14 00:22:25.000000 clustutils4r-0.0.4/src/clustutils4r.egg-info/dependency_links.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       44 2023-07-14 00:22:25.000000 clustutils4r-0.0.4/src/clustutils4r.egg-info/requires.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       13 2023-07-14 00:22:25.000000 clustutils4r-0.0.4/src/clustutils4r.egg-info/top_level.txt
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-14 00:29:24.681324 clustutils4r-0.0.5/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    35128 2023-07-13 07:56:53.000000 clustutils4r-0.0.5/LICENSE
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     3823 2023-07-14 00:29:24.681324 clustutils4r-0.0.5/PKG-INFO
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     3191 2023-07-14 00:24:10.000000 clustutils4r-0.0.5/README.md
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      659 2023-07-14 00:28:49.000000 clustutils4r-0.0.5/pyproject.toml
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       38 2023-07-14 00:29:24.681324 clustutils4r-0.0.5/setup.cfg
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      978 2023-07-14 00:28:53.000000 clustutils4r-0.0.5/setup.py
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-14 00:29:24.681324 clustutils4r-0.0.5/src/
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-14 00:29:24.681324 clustutils4r-0.0.5/src/clustutils4r/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        0 2023-07-13 05:33:28.000000 clustutils4r-0.0.5/src/clustutils4r/__init__.py
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    25231 2023-07-14 00:18:19.000000 clustutils4r-0.0.5/src/clustutils4r/eval_clustering.py
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-14 00:29:24.681324 clustutils4r-0.0.5/src/clustutils4r.egg-info/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     3823 2023-07-14 00:29:24.000000 clustutils4r-0.0.5/src/clustutils4r.egg-info/PKG-INFO
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      305 2023-07-14 00:29:24.000000 clustutils4r-0.0.5/src/clustutils4r.egg-info/SOURCES.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        1 2023-07-14 00:29:24.000000 clustutils4r-0.0.5/src/clustutils4r.egg-info/dependency_links.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       44 2023-07-14 00:29:24.000000 clustutils4r-0.0.5/src/clustutils4r.egg-info/requires.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       13 2023-07-14 00:29:24.000000 clustutils4r-0.0.5/src/clustutils4r.egg-info/top_level.txt
```

### Comparing `clustutils4r-0.0.4/LICENSE` & `clustutils4r-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `clustutils4r-0.0.4/PKG-INFO` & `clustutils4r-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clustutils4r
-Version: 0.0.4
+Version: 0.0.5
 Summary: Wrapper around some basic sklearn utilities for clustering.
 Home-page: https://github.com/rutujagurav/clustutils4r
 Author: Rutuja Gurav
 Author-email: Rutuja Gurav <rutujagurav100@gmail.com>
 Project-URL: Homepage, https://github.com/rutujagurav/clustutils4r
 Project-URL: Bug Tracker, https://github.com/rutujagurav/clustutils4r/issues
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Clustering Utilities
 
 This packages provides a simple convenience wrapper around some basic sklearn utilities for clustering. The only function available is `eval_clustering()`.
 
+## Installation
+`pip install clustutils4r`
+
 ## Available Parameters
 
 `model`: Clustering model object (untrained)
 
 `X`: Numpy array containing preprocessed, normalized, complete dataset features
 
 `gt_labels`: Numpy array containing encoded ground-truth labels for `X` (often not available)
```

### Comparing `clustutils4r-0.0.4/README.md` & `clustutils4r-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # Clustering Utilities
 
 This packages provides a simple convenience wrapper around some basic sklearn utilities for clustering. The only function available is `eval_clustering()`.
 
+## Installation
+`pip install clustutils4r`
+
 ## Available Parameters
 
 `model`: Clustering model object (untrained)
 
 `X`: Numpy array containing preprocessed, normalized, complete dataset features
 
 `gt_labels`: Numpy array containing encoded ground-truth labels for `X` (often not available)
```

### Comparing `clustutils4r-0.0.4/pyproject.toml` & `clustutils4r-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clustutils4r"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Rutuja Gurav", email="rutujagurav100@gmail.com" },
 ]
 description = "Wrapper around some basic sklearn utilities for clustering."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers=[
```

### Comparing `clustutils4r-0.0.4/setup.py` & `clustutils4r-0.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="clustutils4r", # Replace with your own username
-    version="0.0.4",
+    version="0.0.5",
     author="Rutuja Gurav",
     author_email="rutujagurav100@gmail.com",
     description="Wrapper around some basic sklearn utilities for clustering.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rutujagurav/clustutils4r",
     project_urls={
```

### Comparing `clustutils4r-0.0.4/src/clustutils4r/eval_clustering.py` & `clustutils4r-0.0.5/src/clustutils4r/eval_clustering.py`

 * *Files identical despite different names*

### Comparing `clustutils4r-0.0.4/src/clustutils4r.egg-info/PKG-INFO` & `clustutils4r-0.0.5/src/clustutils4r.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clustutils4r
-Version: 0.0.4
+Version: 0.0.5
 Summary: Wrapper around some basic sklearn utilities for clustering.
 Home-page: https://github.com/rutujagurav/clustutils4r
 Author: Rutuja Gurav
 Author-email: Rutuja Gurav <rutujagurav100@gmail.com>
 Project-URL: Homepage, https://github.com/rutujagurav/clustutils4r
 Project-URL: Bug Tracker, https://github.com/rutujagurav/clustutils4r/issues
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Clustering Utilities
 
 This packages provides a simple convenience wrapper around some basic sklearn utilities for clustering. The only function available is `eval_clustering()`.
 
+## Installation
+`pip install clustutils4r`
+
 ## Available Parameters
 
 `model`: Clustering model object (untrained)
 
 `X`: Numpy array containing preprocessed, normalized, complete dataset features
 
 `gt_labels`: Numpy array containing encoded ground-truth labels for `X` (often not available)
```

