# Comparing `tmp/Coquille-1.0.0.tar.gz` & `tmp/Coquille-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Coquille-1.0.0.tar", last modified: Fri Jul 14 10:59:06 2023, max compression
+gzip compressed data, was "Coquille-1.0.1.tar", last modified: Fri Jul 14 11:17:39 2023, max compression
```

## Comparing `Coquille-1.0.0.tar` & `Coquille-1.0.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-14 10:59:06.371747 Coquille-1.0.0/
--rw-r--r--   0 qexat     (1000) qexat     (1001)     1813 2023-07-14 10:50:09.000000 Coquille-1.0.0/.gitignore
--rw-r--r--   0 qexat     (1000) qexat     (1001)      551 2023-07-14 10:50:09.000000 Coquille-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 qexat     (1000) qexat     (1001)     1062 2023-07-14 10:50:09.000000 Coquille-1.0.0/LICENSE
--rw-r--r--   0 qexat     (1000) qexat     (1001)     4690 2023-07-14 10:59:06.371747 Coquille-1.0.0/PKG-INFO
--rw-r--r--   0 qexat     (1000) qexat     (1001)     3086 2023-07-14 10:50:09.000000 Coquille-1.0.0/README.md
-drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-14 10:59:06.365081 Coquille-1.0.0/examples/
-drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-14 10:59:06.368414 Coquille-1.0.0/examples/coquille_context/
--rw-r--r--   0 qexat     (1000) qexat     (1001)      437 2023-07-14 10:50:09.000000 Coquille-1.0.0/examples/coquille_context/__main__.py
--rw-r--r--   0 qexat     (1000) qexat     (1001)    31985 2023-07-14 10:50:09.000000 Coquille-1.0.0/examples/coquille_context/screenshot.png
-drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-14 10:59:06.368414 Coquille-1.0.0/examples/coquille_write/
--rw-r--r--   0 qexat     (1000) qexat     (1001)      436 2023-07-14 10:50:09.000000 Coquille-1.0.0/examples/coquille_write/__main__.py
--rw-r--r--   0 qexat     (1000) qexat     (1001)       45 2023-07-14 10:50:09.000000 Coquille-1.0.0/examples/coquille_write/output.txt
--rw-r--r--   0 qexat     (1000) qexat     (1001)    44980 2023-07-14 10:50:09.000000 Coquille-1.0.0/examples/coquille_write/screenshot.png
--rw-r--r--   0 qexat     (1000) qexat     (1001)      533 2023-07-14 10:54:29.000000 Coquille-1.0.0/pyproject.toml
--rw-r--r--   0 qexat     (1000) qexat     (1001)       38 2023-07-14 10:59:06.371747 Coquille-1.0.0/setup.cfg
-drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-14 10:59:06.365081 Coquille-1.0.0/src/
-drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-14 10:59:06.371747 Coquille-1.0.0/src/Coquille.egg-info/
--rw-r--r--   0 qexat     (1000) qexat     (1001)     4690 2023-07-14 10:59:06.000000 Coquille-1.0.0/src/Coquille.egg-info/PKG-INFO
--rw-r--r--   0 qexat     (1000) qexat     (1001)      601 2023-07-14 10:59:06.000000 Coquille-1.0.0/src/Coquille.egg-info/SOURCES.txt
--rw-r--r--   0 qexat     (1000) qexat     (1001)        1 2023-07-14 10:59:06.000000 Coquille-1.0.0/src/Coquille.egg-info/dependency_links.txt
--rw-r--r--   0 qexat     (1000) qexat     (1001)       29 2023-07-14 10:59:06.000000 Coquille-1.0.0/src/Coquille.egg-info/requires.txt
--rw-r--r--   0 qexat     (1000) qexat     (1001)        9 2023-07-14 10:59:06.000000 Coquille-1.0.0/src/Coquille.egg-info/top_level.txt
-drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-14 10:59:06.371747 Coquille-1.0.0/src/coquille/
--rw-r--r--   0 qexat     (1000) qexat     (1001)       32 2023-07-14 10:50:09.000000 Coquille-1.0.0/src/coquille/__init__.py
--rw-r--r--   0 qexat     (1000) qexat     (1001)     6327 2023-07-14 10:57:15.000000 Coquille-1.0.0/src/coquille/coquille.py
--rw-r--r--   0 qexat     (1000) qexat     (1001)    10596 2023-07-14 10:50:09.000000 Coquille-1.0.0/src/coquille/sequences.py
--rw-r--r--   0 qexat     (1000) qexat     (1001)      340 2023-07-14 10:50:09.000000 Coquille-1.0.0/src/coquille/typeshed.py
-drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-14 10:59:06.371747 Coquille-1.0.0/tests/
--rw-r--r--   0 qexat     (1000) qexat     (1001)        0 2023-07-14 10:50:09.000000 Coquille-1.0.0/tests/__init__.py
--rw-r--r--   0 qexat     (1000) qexat     (1001)     1081 2023-07-14 10:50:09.000000 Coquille-1.0.0/tests/coquille_test.py
--rw-r--r--   0 qexat     (1000) qexat     (1001)     4219 2023-07-14 10:50:09.000000 Coquille-1.0.0/tests/sequences_test.py
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-14 11:17:39.758945 Coquille-1.0.1/
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     1813 2023-07-14 10:50:09.000000 Coquille-1.0.1/.gitignore
+-rw-r--r--   0 qexat     (1000) qexat     (1001)      551 2023-07-14 10:50:09.000000 Coquille-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     1062 2023-07-14 10:50:09.000000 Coquille-1.0.1/LICENSE
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     4842 2023-07-14 11:17:39.758945 Coquille-1.0.1/PKG-INFO
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     3086 2023-07-14 10:50:09.000000 Coquille-1.0.1/README.md
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-14 11:17:39.748945 Coquille-1.0.1/examples/
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-14 11:17:39.752278 Coquille-1.0.1/examples/coquille_context/
+-rw-r--r--   0 qexat     (1000) qexat     (1001)      437 2023-07-14 10:50:09.000000 Coquille-1.0.1/examples/coquille_context/__main__.py
+-rw-r--r--   0 qexat     (1000) qexat     (1001)    31985 2023-07-14 10:50:09.000000 Coquille-1.0.1/examples/coquille_context/screenshot.png
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-14 11:17:39.752278 Coquille-1.0.1/examples/coquille_write/
+-rw-r--r--   0 qexat     (1000) qexat     (1001)      436 2023-07-14 10:50:09.000000 Coquille-1.0.1/examples/coquille_write/__main__.py
+-rw-r--r--   0 qexat     (1000) qexat     (1001)       45 2023-07-14 10:50:09.000000 Coquille-1.0.1/examples/coquille_write/output.txt
+-rw-r--r--   0 qexat     (1000) qexat     (1001)    44980 2023-07-14 10:50:09.000000 Coquille-1.0.1/examples/coquille_write/screenshot.png
+-rw-r--r--   0 qexat     (1000) qexat     (1001)      698 2023-07-14 11:17:20.000000 Coquille-1.0.1/pyproject.toml
+-rw-r--r--   0 qexat     (1000) qexat     (1001)       38 2023-07-14 11:17:39.758945 Coquille-1.0.1/setup.cfg
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-14 11:17:39.748945 Coquille-1.0.1/src/
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-14 11:17:39.755612 Coquille-1.0.1/src/Coquille.egg-info/
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     4842 2023-07-14 11:17:39.000000 Coquille-1.0.1/src/Coquille.egg-info/PKG-INFO
+-rw-r--r--   0 qexat     (1000) qexat     (1001)      601 2023-07-14 11:17:39.000000 Coquille-1.0.1/src/Coquille.egg-info/SOURCES.txt
+-rw-r--r--   0 qexat     (1000) qexat     (1001)        1 2023-07-14 11:17:39.000000 Coquille-1.0.1/src/Coquille.egg-info/dependency_links.txt
+-rw-r--r--   0 qexat     (1000) qexat     (1001)       35 2023-07-14 11:17:39.000000 Coquille-1.0.1/src/Coquille.egg-info/requires.txt
+-rw-r--r--   0 qexat     (1000) qexat     (1001)        9 2023-07-14 11:17:39.000000 Coquille-1.0.1/src/Coquille.egg-info/top_level.txt
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-14 11:17:39.758945 Coquille-1.0.1/src/coquille/
+-rw-r--r--   0 qexat     (1000) qexat     (1001)       32 2023-07-14 10:50:09.000000 Coquille-1.0.1/src/coquille/__init__.py
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     6327 2023-07-14 10:57:15.000000 Coquille-1.0.1/src/coquille/coquille.py
+-rw-r--r--   0 qexat     (1000) qexat     (1001)    10596 2023-07-14 10:50:09.000000 Coquille-1.0.1/src/coquille/sequences.py
+-rw-r--r--   0 qexat     (1000) qexat     (1001)      340 2023-07-14 10:50:09.000000 Coquille-1.0.1/src/coquille/typeshed.py
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-14 11:17:39.758945 Coquille-1.0.1/tests/
+-rw-r--r--   0 qexat     (1000) qexat     (1001)        0 2023-07-14 10:50:09.000000 Coquille-1.0.1/tests/__init__.py
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     1081 2023-07-14 10:50:09.000000 Coquille-1.0.1/tests/coquille_test.py
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     4219 2023-07-14 10:50:09.000000 Coquille-1.0.1/tests/sequences_test.py
```

### Comparing `Coquille-1.0.0/.gitignore` & `Coquille-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `Coquille-1.0.0/.pre-commit-config.yaml` & `Coquille-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `Coquille-1.0.0/LICENSE` & `Coquille-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Coquille-1.0.0/PKG-INFO` & `Coquille-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Coquille
-Version: 1.0.0
+Version: 1.0.1
 Summary: Coquille is a library that wraps terminal escape sequences as convenient functions.
 Author: Qexat
 License: MIT License
         
         Copyright (c) 2023 Qexat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,14 +21,17 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
+Project-URL: homepage, https://github.com/qexat/Coquille
+Project-URL: repository, https://github.com/qexat/Coquille
+Keywords: terminal,escape sequences
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `Coquille-1.0.0/README.md` & `Coquille-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `Coquille-1.0.0/examples/coquille_context/screenshot.png` & `Coquille-1.0.1/examples/coquille_context/screenshot.png`

 * *Files identical despite different names*

### Comparing `Coquille-1.0.0/examples/coquille_write/screenshot.png` & `Coquille-1.0.1/examples/coquille_write/screenshot.png`

 * *Files identical despite different names*

### Comparing `Coquille-1.0.0/pyproject.toml` & `Coquille-1.0.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 [project]
 name = "Coquille"
-version = "1.0.0"
+version = "1.0.1"
 authors = [{ name = "Qexat" }]
 description = "Coquille is a library that wraps terminal escape sequences as convenient functions."
 readme = "README.md"
 requires-python = ">=3.9"
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
 ]
+keywords = ["terminal", "escape sequences"]
+
+[project.urls]
+homepage = "https://github.com/qexat/Coquille"
+repository = "https://github.com/qexat/Coquille"
 
 [project.optional-dependencies]
-dev = ["pytest", "coverage", "build"]
+dev = ["pytest", "coverage", "build", "twine"]
 
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
```

### Comparing `Coquille-1.0.0/src/Coquille.egg-info/PKG-INFO` & `Coquille-1.0.1/src/Coquille.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Coquille
-Version: 1.0.0
+Version: 1.0.1
 Summary: Coquille is a library that wraps terminal escape sequences as convenient functions.
 Author: Qexat
 License: MIT License
         
         Copyright (c) 2023 Qexat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,14 +21,17 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
+Project-URL: homepage, https://github.com/qexat/Coquille
+Project-URL: repository, https://github.com/qexat/Coquille
+Keywords: terminal,escape sequences
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `Coquille-1.0.0/src/Coquille.egg-info/SOURCES.txt` & `Coquille-1.0.1/src/Coquille.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Coquille-1.0.0/src/coquille/coquille.py` & `Coquille-1.0.1/src/coquille/coquille.py`

 * *Files identical despite different names*

### Comparing `Coquille-1.0.0/src/coquille/sequences.py` & `Coquille-1.0.1/src/coquille/sequences.py`

 * *Files identical despite different names*

### Comparing `Coquille-1.0.0/tests/coquille_test.py` & `Coquille-1.0.1/tests/coquille_test.py`

 * *Files identical despite different names*

### Comparing `Coquille-1.0.0/tests/sequences_test.py` & `Coquille-1.0.1/tests/sequences_test.py`

 * *Files identical despite different names*

