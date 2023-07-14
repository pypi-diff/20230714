# Comparing `tmp/decontext-0.1.0.tar.gz` & `tmp/decontext-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decontext-0.1.0.tar", last modified: Wed Jul  5 20:50:31 2023, max compression
+gzip compressed data, was "decontext-0.1.1.tar", last modified: Fri Jul 14 02:49:07 2023, max compression
```

## Comparing `decontext-0.1.0.tar` & `decontext-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,31 @@
-drwxr-xr-x   0 benjaminn   (502) staff       (20)        0 2023-07-05 20:50:31.231564 decontext-0.1.0/
--rw-r--r--   0 benjaminn   (502) staff       (20)     7767 2023-07-05 20:50:31.231397 decontext-0.1.0/PKG-INFO
--rw-r--r--   0 benjaminn   (502) staff       (20)     6647 2023-07-05 20:40:20.000000 decontext-0.1.0/README.md
--rw-r--r--   0 benjaminn   (502) staff       (20)     2642 2023-07-05 20:50:09.000000 decontext-0.1.0/pyproject.toml
--rw-r--r--   0 benjaminn   (502) staff       (20)       38 2023-07-05 20:50:31.231620 decontext-0.1.0/setup.cfg
-drwxr-xr-x   0 benjaminn   (502) staff       (20)        0 2023-07-05 20:50:31.229834 decontext-0.1.0/src/
-drwxr-xr-x   0 benjaminn   (502) staff       (20)        0 2023-07-05 20:50:31.230417 decontext-0.1.0/src/decontext/
--rw-r--r--   0 benjaminn   (502) staff       (20)        0 2023-07-05 20:42:37.000000 decontext-0.1.0/src/decontext/__init__.py
--rw-r--r--   0 benjaminn   (502) staff       (20)        0 2023-07-05 20:48:09.000000 decontext-0.1.0/src/decontext/py.typed
-drwxr-xr-x   0 benjaminn   (502) staff       (20)        0 2023-07-05 20:50:31.231166 decontext-0.1.0/src/decontext.egg-info/
--rw-r--r--   0 benjaminn   (502) staff       (20)     7767 2023-07-05 20:50:31.000000 decontext-0.1.0/src/decontext.egg-info/PKG-INFO
--rw-r--r--   0 benjaminn   (502) staff       (20)      257 2023-07-05 20:50:31.000000 decontext-0.1.0/src/decontext.egg-info/SOURCES.txt
--rw-r--r--   0 benjaminn   (502) staff       (20)        1 2023-07-05 20:50:31.000000 decontext-0.1.0/src/decontext.egg-info/dependency_links.txt
--rw-r--r--   0 benjaminn   (502) staff       (20)      167 2023-07-05 20:50:31.000000 decontext-0.1.0/src/decontext.egg-info/requires.txt
--rw-r--r--   0 benjaminn   (502) staff       (20)       10 2023-07-05 20:50:31.000000 decontext-0.1.0/src/decontext.egg-info/top_level.txt
+drwxr-xr-x   0 benjaminn  (5207) users      (100)        0 2023-07-14 02:49:07.214471 decontext-0.1.1/
+-rw-r--r--   0 benjaminn  (5207) users      (100)    13576 2023-07-14 02:49:07.213471 decontext-0.1.1/PKG-INFO
+-rw-r--r--   0 benjaminn  (5207) users      (100)    12456 2023-07-14 01:41:35.000000 decontext-0.1.1/README.md
+-rw-r--r--   0 benjaminn  (5207) users      (100)     3078 2023-07-14 02:38:41.000000 decontext-0.1.1/pyproject.toml
+-rw-r--r--   0 benjaminn  (5207) users      (100)       38 2023-07-14 02:49:07.215471 decontext-0.1.1/setup.cfg
+drwxr-xr-x   0 benjaminn  (5207) users      (100)        0 2023-07-14 02:49:07.112475 decontext-0.1.1/src/
+drwxr-xr-x   0 benjaminn  (5207) users      (100)        0 2023-07-14 02:49:07.156473 decontext-0.1.1/src/decontext/
+-rw-r--r--   0 benjaminn  (5207) users      (100)      120 2023-07-14 01:43:45.000000 decontext-0.1.1/src/decontext/__init__.py
+-rw-r--r--   0 benjaminn  (5207) users      (100)     6512 2023-07-12 22:06:39.000000 decontext-0.1.1/src/decontext/cache.py
+-rw-r--r--   0 benjaminn  (5207) users      (100)     6503 2023-07-14 01:23:06.000000 decontext-0.1.1/src/decontext/data_types.py
+-rw-r--r--   0 benjaminn  (5207) users      (100)      115 2023-07-13 17:38:14.000000 decontext-0.1.1/src/decontext/logging.py
+-rw-r--r--   0 benjaminn  (5207) users      (100)    13289 2023-07-14 01:05:17.000000 decontext-0.1.1/src/decontext/model.py
+-rw-r--r--   0 benjaminn  (5207) users      (100)     2650 2023-07-14 02:03:38.000000 decontext-0.1.1/src/decontext/pipeline.py
+-rw-r--r--   0 benjaminn  (5207) users      (100)        0 2023-07-07 20:57:14.000000 decontext-0.1.1/src/decontext/py.typed
+drwxr-xr-x   0 benjaminn  (5207) users      (100)        0 2023-07-14 02:49:07.198472 decontext-0.1.1/src/decontext/step/
+-rw-r--r--   0 benjaminn  (5207) users      (100)     5892 2023-07-14 00:52:27.000000 decontext-0.1.1/src/decontext/step/qa.py
+-rw-r--r--   0 benjaminn  (5207) users      (100)      664 2023-07-13 17:38:14.000000 decontext-0.1.1/src/decontext/step/qgen.py
+-rw-r--r--   0 benjaminn  (5207) users      (100)      969 2023-07-13 17:38:14.000000 decontext-0.1.1/src/decontext/step/step.py
+-rw-r--r--   0 benjaminn  (5207) users      (100)      685 2023-07-13 17:38:14.000000 decontext-0.1.1/src/decontext/step/synth.py
+-rw-r--r--   0 benjaminn  (5207) users      (100)     3840 2023-07-14 01:03:23.000000 decontext-0.1.1/src/decontext/template.py
+-rw-r--r--   0 benjaminn  (5207) users      (100)      920 2023-07-14 00:52:27.000000 decontext-0.1.1/src/decontext/utils.py
+drwxr-xr-x   0 benjaminn  (5207) users      (100)        0 2023-07-14 02:49:07.183472 decontext-0.1.1/src/decontext.egg-info/
+-rw-r--r--   0 benjaminn  (5207) users      (100)    13576 2023-07-14 02:49:07.000000 decontext-0.1.1/src/decontext.egg-info/PKG-INFO
+-rw-r--r--   0 benjaminn  (5207) users      (100)      606 2023-07-14 02:49:07.000000 decontext-0.1.1/src/decontext.egg-info/SOURCES.txt
+-rw-r--r--   0 benjaminn  (5207) users      (100)        1 2023-07-14 02:49:07.000000 decontext-0.1.1/src/decontext.egg-info/dependency_links.txt
+-rw-r--r--   0 benjaminn  (5207) users      (100)      477 2023-07-14 02:49:07.000000 decontext-0.1.1/src/decontext.egg-info/requires.txt
+-rw-r--r--   0 benjaminn  (5207) users      (100)       10 2023-07-14 02:49:07.000000 decontext-0.1.1/src/decontext.egg-info/top_level.txt
+drwxr-xr-x   0 benjaminn  (5207) users      (100)        0 2023-07-14 02:49:07.209471 decontext-0.1.1/tests/
+-rw-r--r--   0 benjaminn  (5207) users      (100)     1052 2023-07-14 02:43:59.000000 decontext-0.1.1/tests/test_data_types.py
+-rw-r--r--   0 benjaminn  (5207) users      (100)     8590 2023-07-14 00:56:27.000000 decontext-0.1.1/tests/test_pipeline.py
+-rw-r--r--   0 benjaminn  (5207) users      (100)      348 2023-07-14 00:52:27.000000 decontext-0.1.1/tests/test_utils.py
```

### Comparing `decontext-0.1.0/pyproject.toml` & `decontext-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,34 @@
 [project]
 name = "decontext"
-version = "0.1.0"
+version = "0.1.1"
 description = """\
 Pipeline for decontextualization of scientific snippets.
 """
 license = {text = "Apache-2.0"}
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
+    "anthropic==0.2.10",
+    "diskcache==5.6.1",
+    "filelock==3.12.2",
+    "Jinja2==3.1.2",
+    "shadow-scholar==0.6.1",
+    "omegaconf==2.2.3",
+    "openai==0.27.7",
+    "pydantic==1.9.1",
+    "tiktoken==0.4.0",
+    "numpy==1.23.2",
+    "spacy==3.4.1",
+    "torch<2.0.0",
+    "scikit-learn==1.1.2",
+    "transformers==4.28.0",
+    "unidecode",
+    "sentence-transformers==2.2.2",
+    "typing_extensions==4.5.0",
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
@@ -71,14 +88,15 @@
     "pytest>=5.2",
     "ipython>=8.4.0",
     "autopep8>=1.7.0",
     "flake8>=5.0",
     "ipdb>=0.13.0",
     "flake8-pyi>=22.8.1",
     "Flake8-pyproject>=1.1.0",
+    "pytest==7.1.3",
 ]
 
 [tool.black]
 line-length = 79
 include = '\.pyi?$'
 exclude = '''
 (
```

