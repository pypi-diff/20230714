# Comparing `tmp/ontoenv-0.3.6.tar.gz` & `tmp/ontoenv-0.3.7a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ontoenv-0.3.6.tar", max compression
+gzip compressed data, was "ontoenv-0.3.7a1.tar", max compression
```

## Comparing `ontoenv-0.3.6.tar` & `ontoenv-0.3.7a1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1519 2023-04-20 23:37:22.604572 ontoenv-0.3.6/LICENSE
--rw-r--r--   0        0        0    11493 2023-05-23 00:33:34.327522 ontoenv-0.3.6/ontoenv/__init__.py
--rw-r--r--   0        0        0     2065 2023-04-20 23:37:22.605017 ontoenv-0.3.6/ontoenv/cli.py
--rw-r--r--   0        0        0      527 2023-05-23 00:38:28.702655 ontoenv-0.3.6/pyproject.toml
--rw-r--r--   0        0        0      811 1970-01-01 00:00:00.000000 ontoenv-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1519 2023-04-20 23:37:22.604572 ontoenv-0.3.7a1/LICENSE
+-rw-r--r--   0        0        0    12565 2023-07-13 23:36:29.662858 ontoenv-0.3.7a1/ontoenv/__init__.py
+-rw-r--r--   0        0        0     2065 2023-04-20 23:37:22.605017 ontoenv-0.3.7a1/ontoenv/cli.py
+-rw-r--r--   0        0        0      529 2023-07-13 23:36:40.716858 ontoenv-0.3.7a1/pyproject.toml
+-rw-r--r--   0        0        0      813 1970-01-01 00:00:00.000000 ontoenv-0.3.7a1/PKG-INFO
```

### Comparing `ontoenv-0.3.6/LICENSE` & `ontoenv-0.3.7a1/LICENSE`

 * *Files identical despite different names*

### Comparing `ontoenv-0.3.6/ontoenv/__init__.py` & `ontoenv-0.3.7a1/ontoenv/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 """
 import sys
+from typing import Callable
 import json
 from pathlib import Path
 import os
 import glob
 import shutil
 import logging
 import rdflib
@@ -226,27 +227,42 @@
         print(f"{'|  '*indent}{char} {uri}")
         seen.add(uri)
         num_deps = len(self._dependencies.edges([uri]))
         for (i, (_, dep)) in enumerate(self._dependencies.edges([uri])):
             self._print_dep_graph(dep, indent + 1, seen, last=i == num_deps - 1)
 
     def import_dependencies(
-        self, graph, cache=None, recursive=True, recursive_limit=-1
+        self, graph: rdflib.Graph, cache=None, recursive=True, recursive_limit=-1, keep_matching: Optional[Callable[[rdflib.term.Node], bool]]=None
     ):
+        """
+        Imports graph dependencies required by the provided graph into that graph object
+
+        :param graph: The graph from which to read the import statements, and the graph in which the graphs are deposited
+        :type graph: rdflib.Graph
+        :param recursive: if True, include all graphs in the transitive closure of `owl:imports`, defaults to True
+        :type recursive: bool, optional
+        :param recursive_limit: A limit to the size of the transitive closure resolved when `recursive` is True; for example, if recursive_limit = 1, then only the immediate dependencies of the graph are included
+        :type recursive_limit: bool, optional
+        :param keep_matching: an optional function which returns True for ontologies which should be imported
+        """
         if recursive_limit > 0:
             recursive = False
         elif recursive_limit == 0:
             return
         if cache is None:
             cache = set()
         new_imports = False
         for importURI in graph.objects(predicate=rdflib.OWL.imports):
             uri = str(importURI)
             if uri in cache:
                 continue
+            # skip if it doesn't match a provided filter
+            if keep_matching and not keep_matching(uri):
+                cache.add(uri)
+                continue
             new_imports = True
             filename = self.mapping.get(uri)
             if filename is None:
                 if self._strict:
                     raise Exception(f"Could not load {uri} (no definition found)")
                 logging.error(f"Could not load {uri} (no definition found)")
                 cache.add(uri)
```

### Comparing `ontoenv-0.3.6/ontoenv/cli.py` & `ontoenv-0.3.7a1/ontoenv/cli.py`

 * *Files identical despite different names*

### Comparing `ontoenv-0.3.6/pyproject.toml` & `ontoenv-0.3.7a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ontoenv"
-version = "0.3.6"
+version = "0.3.7a1"
 description = "Manages owl:imports statements for multi-file development"
 authors = ["Gabe Fierro <gtfierro@mines.edu>"]
 license = "BSD 3-Clause"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 rdflib = "^6.0.0"
```

### Comparing `ontoenv-0.3.6/PKG-INFO` & `ontoenv-0.3.7a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ontoenv
-Version: 0.3.6
+Version: 0.3.7a1
 Summary: Manages owl:imports statements for multi-file development
 License: BSD 3-Clause
 Author: Gabe Fierro
 Author-email: gtfierro@mines.edu
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

