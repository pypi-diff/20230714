# Comparing `tmp/idea_bio-0.1.4.tar.gz` & `tmp/idea_bio-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idea_bio-0.1.4.tar", max compression
+gzip compressed data, was "idea_bio-0.1.5.tar", max compression
```

## Comparing `idea_bio-0.1.4.tar` & `idea_bio-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-07-14 03:15:58.372612 idea_bio-0.1.4/LICENSE
--rw-r--r--   0        0        0     2069 2023-07-14 03:15:58.375945 idea_bio-0.1.4/README.md
--rw-r--r--   0        0        0      201 2023-07-14 03:15:58.392612 idea_bio-0.1.4/idea/__init__.py
--rw-r--r--   0        0        0     1561 2023-07-14 03:15:58.392612 idea_bio-0.1.4/idea/_go.py
--rw-r--r--   0        0        0    10142 2023-07-14 03:15:58.392612 idea_bio-0.1.4/idea/_idea.py
--rw-r--r--   0        0        0      438 2023-07-14 03:15:58.392612 idea_bio-0.1.4/idea/_utils.py
--rw-r--r--   0        0        0      669 2023-07-14 03:26:52.073806 idea_bio-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2958 1970-01-01 00:00:00.000000 idea_bio-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 03:15:58.372612 idea_bio-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2069 2023-07-14 03:15:58.375945 idea_bio-0.1.5/README.md
+-rw-r--r--   0        0        0      201 2023-07-14 03:15:58.392612 idea_bio-0.1.5/idea/__init__.py
+-rw-r--r--   0        0        0     1561 2023-07-14 03:15:58.392612 idea_bio-0.1.5/idea/_go.py
+-rw-r--r--   0        0        0    10142 2023-07-14 03:15:58.392612 idea_bio-0.1.5/idea/_idea.py
+-rw-r--r--   0        0        0      438 2023-07-14 03:15:58.392612 idea_bio-0.1.5/idea/_utils.py
+-rw-r--r--   0        0        0      691 2023-07-14 15:12:08.109779 idea_bio-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3001 1970-01-01 00:00:00.000000 idea_bio-0.1.5/PKG-INFO
```

### Comparing `idea_bio-0.1.4/LICENSE` & `idea_bio-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `idea_bio-0.1.4/README.md` & `idea_bio-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `idea_bio-0.1.4/idea/_go.py` & `idea_bio-0.1.5/idea/_go.py`

 * *Files identical despite different names*

### Comparing `idea_bio-0.1.4/idea/_idea.py` & `idea_bio-0.1.5/idea/_idea.py`

 * *Files identical despite different names*

### Comparing `idea_bio-0.1.4/pyproject.toml` & `idea_bio-0.1.5/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "idea-bio"
-version = "0.1.4"
+version = "0.1.5"
 description = "Integrated Differential Expression and Annotation"
 authors = ["Noam Teyssier"]
 license = "MIT"
 readme = "README.md"
 packages = [
   { include = "idea" }
 ]
@@ -14,14 +14,15 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = "^1.24.0"
 pandas = "^2.0.3"
 networkx = "^3.1"
 pyvis = "^0.3.2"
 ggetrs = "^0.1.73"
+matplotlib = "^3.7.2"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.7.0"
 pytest = "^7.4.0"
 jupyterlab = "^4.0.2"
 
 [build-system]
```

### Comparing `idea_bio-0.1.4/PKG-INFO` & `idea_bio-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: idea-bio
-Version: 0.1.4
+Version: 0.1.5
 Summary: Integrated Differential Expression and Annotation
 Home-page: https://github.com/noamteyssier/idea
 License: MIT
 Keywords: bioinformatics,differential expression,annotation,networks
 Author: Noam Teyssier
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ggetrs (>=0.1.73,<0.2.0)
+Requires-Dist: matplotlib (>=3.7.2,<4.0.0)
 Requires-Dist: networkx (>=3.1,<4.0)
 Requires-Dist: numpy (>=1.24.0,<2.0.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: pyvis (>=0.3.2,<0.4.0)
 Project-URL: Repository, https://github.com/noamteyssier/idea
 Description-Content-Type: text/markdown
```

