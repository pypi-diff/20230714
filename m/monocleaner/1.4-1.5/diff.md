# Comparing `tmp/monocleaner-1.4.tar.gz` & `tmp/monocleaner-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monocleaner-1.4.tar", last modified: Fri Apr 28 14:17:39 2023, max compression
+gzip compressed data, was "monocleaner-1.5.tar", last modified: Fri Jul 14 09:43:28 2023, max compression
```

## Comparing `monocleaner-1.4.tar` & `monocleaner-1.5.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 14:17:39.233454 monocleaner-1.4/
--rw-r--r--   0 runner    (1001) docker     (122)    35147 2023-04-28 14:17:26.000000 monocleaner-1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     6114 2023-04-28 14:17:39.233454 monocleaner-1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5020 2023-04-28 14:17:26.000000 monocleaner-1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1537 2023-04-28 14:17:26.000000 monocleaner-1.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 14:17:39.229453 monocleaner-1.4/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (122)      918 2023-04-28 14:17:26.000000 monocleaner-1.4/scripts/monocleaner-download
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-28 14:17:39.233454 monocleaner-1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 14:17:39.229453 monocleaner-1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 14:17:39.233454 monocleaner-1.4/src/monocleaner/
--rw-r--r--   0 runner    (1001) docker     (122)       77 2023-04-28 14:17:26.000000 monocleaner-1.4/src/monocleaner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7703 2023-04-28 14:17:26.000000 monocleaner-1.4/src/monocleaner/hardrules.py
--rw-r--r--   0 runner    (1001) docker     (122)    13407 2023-04-28 14:17:26.000000 monocleaner-1.4/src/monocleaner/lm.py
--rw-r--r--   0 runner    (1001) docker     (122)     6516 2023-04-28 14:17:26.000000 monocleaner-1.4/src/monocleaner/monocleaner.py
--rw-r--r--   0 runner    (1001) docker     (122)     3302 2023-04-28 14:17:26.000000 monocleaner-1.4/src/monocleaner/monocleaner_train.py
--rw-r--r--   0 runner    (1001) docker     (122)     2193 2023-04-28 14:17:26.000000 monocleaner-1.4/src/monocleaner/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3124 2023-04-28 14:17:26.000000 monocleaner-1.4/src/monocleaner/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 14:17:39.233454 monocleaner-1.4/src/monocleaner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6114 2023-04-28 14:17:39.000000 monocleaner-1.4/src/monocleaner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-04-28 14:17:39.000000 monocleaner-1.4/src/monocleaner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-28 14:17:39.000000 monocleaner-1.4/src/monocleaner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      116 2023-04-28 14:17:39.000000 monocleaner-1.4/src/monocleaner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-04-28 14:17:39.000000 monocleaner-1.4/src/monocleaner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-28 14:17:39.000000 monocleaner-1.4/src/monocleaner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 09:43:28.646980 monocleaner-1.5/
+-rw-r--r--   0 runner    (1001) docker     (122)    35147 2023-07-14 09:43:13.000000 monocleaner-1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     6114 2023-07-14 09:43:28.646980 monocleaner-1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5020 2023-07-14 09:43:13.000000 monocleaner-1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1539 2023-07-14 09:43:13.000000 monocleaner-1.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 09:43:28.642980 monocleaner-1.5/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1304 2023-07-14 09:43:13.000000 monocleaner-1.5/scripts/monocleaner-download
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-14 09:43:28.646980 monocleaner-1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 09:43:28.642980 monocleaner-1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 09:43:28.646980 monocleaner-1.5/src/monocleaner/
+-rw-r--r--   0 runner    (1001) docker     (122)       77 2023-07-14 09:43:13.000000 monocleaner-1.5/src/monocleaner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7703 2023-07-14 09:43:13.000000 monocleaner-1.5/src/monocleaner/hardrules.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13458 2023-07-14 09:43:13.000000 monocleaner-1.5/src/monocleaner/lm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6516 2023-07-14 09:43:13.000000 monocleaner-1.5/src/monocleaner/monocleaner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3302 2023-07-14 09:43:13.000000 monocleaner-1.5/src/monocleaner/monocleaner_train.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6878 2023-07-14 09:43:13.000000 monocleaner-1.5/src/monocleaner/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2193 2023-07-14 09:43:13.000000 monocleaner-1.5/src/monocleaner/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3124 2023-07-14 09:43:13.000000 monocleaner-1.5/src/monocleaner/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 09:43:28.646980 monocleaner-1.5/src/monocleaner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6114 2023-07-14 09:43:28.000000 monocleaner-1.5/src/monocleaner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      526 2023-07-14 09:43:28.000000 monocleaner-1.5/src/monocleaner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-14 09:43:28.000000 monocleaner-1.5/src/monocleaner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      116 2023-07-14 09:43:28.000000 monocleaner-1.5/src/monocleaner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-07-14 09:43:28.000000 monocleaner-1.5/src/monocleaner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-07-14 09:43:28.000000 monocleaner-1.5/src/monocleaner.egg-info/top_level.txt
```

### Comparing `monocleaner-1.4/LICENSE` & `monocleaner-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `monocleaner-1.4/PKG-INFO` & `monocleaner-1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monocleaner
-Version: 1.4
+Version: 1.5
 Summary: Monolingual corpus fluency filter
 Author-email: Prompsit Language Engineering <info@prompsit.com>
 Maintainer-email: Jaume Zaragoza <jzaragoza@prompsit.com>
 License: GNU General Public License v3.0
 Project-URL: Homepage, https://github.com/bitextor/monocleaner
 Project-URL: Monocleaner on GitHub, https://github.com/bitextor/monocleaner
 Project-URL: Prompsit Language Engineering, http://www.prompsit.com
```

### Comparing `monocleaner-1.4/README.md` & `monocleaner-1.5/README.md`

 * *Files identical despite different names*

### Comparing `monocleaner-1.4/pyproject.toml` & `monocleaner-1.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "monocleaner"
-version = "1.4"
+version = "1.5"
 requires-python = ">=3.8"
 authors = [
     { name = "Prompsit Language Engineering", email = "info@prompsit.com" },
 ]
 maintainers = [
     { name = "Jaume Zaragoza", email = "jzaragoza@prompsit.com" },
 ]
@@ -22,15 +22,15 @@
 ]
 dependencies = [
     "regex",
     "toolwrapper",
     "sacremoses",
     "numpy",
     "pyyaml",
-    "fastspell==0.9",
+    "fastspell==0.9.1",
 ]
 
 [project.license]
 text = "GNU General Public License v3.0"
 
 [project.readme]
 file = "README.md"
```

### Comparing `monocleaner-1.4/src/monocleaner/hardrules.py` & `monocleaner-1.5/src/monocleaner/hardrules.py`

 * *Files identical despite different names*

### Comparing `monocleaner-1.4/src/monocleaner/lm.py` & `monocleaner-1.5/src/monocleaner/lm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from tempfile import TemporaryFile, NamedTemporaryFile
-from sacremoses import MosesPunctNormalizer
 from subprocess import PIPE
 from enum import Enum
 import typing
 import kenlm
 import subprocess
 import shutil
 import argparse
@@ -13,17 +12,19 @@
 import random
 import sys
 import os
 
 try:
     from .util import shuffle_file
     from .tokenizer import Tokenizer
+    from .normalize import MosesPunctNormalizer
 except (SystemError, ImportError):
     from util import shuffle_file
     from tokenizer import Tokenizer
+    from normalize import MosesPunctNormalizer
 
 
 class LMType(Enum):
     #Needed for argparse
     PLACEHOLDER='PLACEHOLDER'
     CHARACTER='CHARACTER'
```

### Comparing `monocleaner-1.4/src/monocleaner/monocleaner.py` & `monocleaner-1.5/src/monocleaner/monocleaner.py`

 * *Files identical despite different names*

### Comparing `monocleaner-1.4/src/monocleaner/monocleaner_train.py` & `monocleaner-1.5/src/monocleaner/monocleaner_train.py`

 * *Files identical despite different names*

### Comparing `monocleaner-1.4/src/monocleaner/tokenizer.py` & `monocleaner-1.5/src/monocleaner/tokenizer.py`

 * *Files identical despite different names*

### Comparing `monocleaner-1.4/src/monocleaner/util.py` & `monocleaner-1.5/src/monocleaner/util.py`

 * *Files identical despite different names*

### Comparing `monocleaner-1.4/src/monocleaner.egg-info/PKG-INFO` & `monocleaner-1.5/src/monocleaner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monocleaner
-Version: 1.4
+Version: 1.5
 Summary: Monolingual corpus fluency filter
 Author-email: Prompsit Language Engineering <info@prompsit.com>
 Maintainer-email: Jaume Zaragoza <jzaragoza@prompsit.com>
 License: GNU General Public License v3.0
 Project-URL: Homepage, https://github.com/bitextor/monocleaner
 Project-URL: Monocleaner on GitHub, https://github.com/bitextor/monocleaner
 Project-URL: Prompsit Language Engineering, http://www.prompsit.com
```

