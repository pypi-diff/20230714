# Comparing `tmp/pipforester-1.0.0a1.tar.gz` & `tmp/pipforester-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipforester-1.0.0a1.tar", last modified: Mon May 15 20:09:11 2023, max compression
+gzip compressed data, was "pipforester-1.0.1.tar", last modified: Fri Jul 14 16:53:31 2023, max compression
```

## Comparing `pipforester-1.0.0a1.tar` & `pipforester-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-05-15 20:09:11.748016 pipforester-1.0.0a1/
--rw-r--r--   0 gil       (1000) gil       (1000)       61 2023-05-15 20:07:15.000000 pipforester-1.0.0a1/CHANGES.md
--rw-r--r--   0 gil       (1000) gil       (1000)     1320 2023-05-15 20:05:44.000000 pipforester-1.0.0a1/LICENSE.md
--rw-r--r--   0 gil       (1000) gil       (1000)     4039 2023-05-15 20:09:11.748016 pipforester-1.0.0a1/PKG-INFO
--rw-r--r--   0 gil       (1000) gil       (1000)     1567 2023-05-15 20:05:44.000000 pipforester-1.0.0a1/README.md
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-05-15 20:09:11.747016 pipforester-1.0.0a1/pipforester/
--rw-r--r--   0 gil       (1000) gil       (1000)      878 2023-05-15 20:05:44.000000 pipforester-1.0.0a1/pipforester/__init__.py
--rw-r--r--   0 gil       (1000) gil       (1000)     2621 2023-05-15 20:05:44.000000 pipforester-1.0.0a1/pipforester/deptree.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-05-15 20:09:11.748016 pipforester-1.0.0a1/pipforester.egg-info/
--rw-r--r--   0 gil       (1000) gil       (1000)     4039 2023-05-15 20:09:11.000000 pipforester-1.0.0a1/pipforester.egg-info/PKG-INFO
--rw-r--r--   0 gil       (1000) gil       (1000)      339 2023-05-15 20:09:11.000000 pipforester-1.0.0a1/pipforester.egg-info/SOURCES.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-05-15 20:09:11.000000 pipforester-1.0.0a1/pipforester.egg-info/dependency_links.txt
--rw-r--r--   0 gil       (1000) gil       (1000)       49 2023-05-15 20:09:11.000000 pipforester-1.0.0a1/pipforester.egg-info/entry_points.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-05-15 20:07:03.000000 pipforester-1.0.0a1/pipforester.egg-info/not-zip-safe
--rw-r--r--   0 gil       (1000) gil       (1000)       52 2023-05-15 20:09:11.000000 pipforester-1.0.0a1/pipforester.egg-info/requires.txt
--rw-r--r--   0 gil       (1000) gil       (1000)       12 2023-05-15 20:09:11.000000 pipforester-1.0.0a1/pipforester.egg-info/top_level.txt
--rw-r--r--   0 gil       (1000) gil       (1000)     2298 2023-05-15 20:07:15.000000 pipforester-1.0.0a1/pyproject.toml
--rw-r--r--   0 gil       (1000) gil       (1000)       38 2023-05-15 20:09:11.748016 pipforester-1.0.0a1/setup.cfg
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-07-14 16:53:31.459227 pipforester-1.0.1/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      360 2023-07-14 16:53:10.000000 pipforester-1.0.1/CHANGES.md
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1320 2023-02-09 10:40:05.000000 pipforester-1.0.1/LICENSE.md
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     4713 2023-07-14 16:53:31.459227 pipforester-1.0.1/PKG-INFO
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1932 2023-06-20 08:40:17.000000 pipforester-1.0.1/README.md
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-07-14 16:53:31.447227 pipforester-1.0.1/pipforester/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      868 2023-07-14 16:48:12.000000 pipforester-1.0.1/pipforester/__init__.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1829 2023-07-14 16:48:12.000000 pipforester-1.0.1/pipforester/deptree.py
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-07-14 16:53:31.459227 pipforester-1.0.1/pipforester.egg-info/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     4713 2023-07-14 16:53:31.000000 pipforester-1.0.1/pipforester.egg-info/PKG-INFO
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      339 2023-07-14 16:53:31.000000 pipforester-1.0.1/pipforester.egg-info/SOURCES.txt
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)        1 2023-07-14 16:53:31.000000 pipforester-1.0.1/pipforester.egg-info/dependency_links.txt
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)       49 2023-07-14 16:53:31.000000 pipforester-1.0.1/pipforester.egg-info/entry_points.txt
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)        1 2023-02-09 10:49:31.000000 pipforester-1.0.1/pipforester.egg-info/not-zip-safe
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)       52 2023-07-14 16:53:31.000000 pipforester-1.0.1/pipforester.egg-info/requires.txt
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)       12 2023-07-14 16:53:31.000000 pipforester-1.0.1/pipforester.egg-info/top_level.txt
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     2308 2023-07-14 16:53:10.000000 pipforester-1.0.1/pyproject.toml
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)       38 2023-07-14 16:53:31.459227 pipforester-1.0.1/setup.cfg
```

### Comparing `pipforester-1.0.0a1/LICENSE.md` & `pipforester-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pipforester-1.0.0a1/PKG-INFO` & `pipforester-1.0.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pipforester
-Version: 1.0.0a1
+Version: 1.0.1
 Summary: A tool to analyze the dependency graph of a pip package.
 Author-email: Jens Klein et al <jk@kleinundpartner.at>
 License: BSD 2-Clause License
 Project-URL: Homepage, https://github.com/collective/pipforester
 Project-URL: Bug Reports, https://github.com/collective/pipforester/issues
 Project-URL: Source, https://github.com/collective/pipforester/
 Keywords: pip,graph,analysis
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,35 +22,51 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
 
 # pipforester
 
-Forester tools for [pipdeptree](https://pypi.org/project/pipdeptree/) outputs to analyze the dependency graph of a pip package.
+Forester tools for [pipdeptree](https://pypi.org/project/pipdeptree/) outputs to analyze and cleanup the dependency graph of installed pip packages.
 
 ## Features
 
-- clean up a graph to remove direct dependencies if a transitive dependency exists
-- detect transitive cyclic dependencies (and color them in output)
+- clean up a graph to remove direct dependencies if a transitive dependency exists and output it as dot-file.
+- detect transitive cyclic dependencies
+  - color them in the graph
+  - show them as separate graphs in one dot-file
+  - exit *pipforester* with exit code 1 if there are cycles detected
+
+### Installation:
+
+- Create an empty virtual environment, separate from the environment to work on.
+- `pip install pipdeptree pipforester`
+
+Dependent on your operation system you
+- want to install a program to view dot-files, like [xdot](https://pypi.org/project/xdot/) i.e. with `apt install xdot` on Debian/Ubuntu-based systems.
+- or use [graphviz](https://www.graphviz.org/) to convert dot-files to PNG/SVG.
 
-## Usage
 
-Important: *pipdeptree* **MUST** be installed in an environment together with the dependencies you want to check.  If you install *pipdeptree* in virtual environment 1 and then call it in the directory of virtual environment 2, it will only report on its own dependencies, which is not very useful.
+## Usage
 
-First, call *pipdeptree* to create a JSON file of the installed dependencies,
+First, call *pipdeptree* on a virtual environment to create a JSON file of the installed dependencies,
 and second call *pipforester* to create a cleaned-up dot file.
 
 ```shell
-pipdeptree -j >forest.json
+pipdeptree --python  path/to/venv/bin/python -j >forest.json
 pipforester -i forest.json -o forest.dot
 ```
 
 Finally use a Graphviz DOT-file visualizer, i.e. *xdot* on Linux, to view the graph.
-Or use the *dot* command line program to generate an svg or png:
+
+```
+xdot forest.dot
+```
+
+Or use the *dot* command line program to generate an SVG or PNG:
 
 ```
 dot -Tsvg -o forest.svg forest.dot
 dot -Tpng -o forest.png forest.dot
 ```
 
 To generate a graph containing only cyclic transitive dependencies, use the `--cycles` option:
@@ -69,17 +85,27 @@
 ```
 
 See `pipforester --help` for details.
 
 
 ## Changes
 
-## 1.0.0a1 (2023-05-15)
+## 1.0.1 (2023-07-14)
+
+- use transitive_reduction from the NetworkX module to speed up edge removal. [@gogobd]
+
+### 1.0.0 (2023-05-16)
+
+- fix the cyclic dependency display to show all edges of a cycle in dark violet. [@jensens]
+- fix graph of cycles not to show graph multiple times. [@jensens]
+
+### 1.0.0a1 (2023-05-15)
+
+- initial code [@jensens]
 
-- initial code [jensens]
 # License
 
 Copyright (c) 2022-2023, mxstack Contributors
 
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
```

### Comparing `pipforester-1.0.0a1/README.md` & `pipforester-1.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,46 @@
 # pipforester
 
-Forester tools for [pipdeptree](https://pypi.org/project/pipdeptree/) outputs to analyze the dependency graph of a pip package.
+Forester tools for [pipdeptree](https://pypi.org/project/pipdeptree/) outputs to analyze and cleanup the dependency graph of installed pip packages.
 
 ## Features
 
-- clean up a graph to remove direct dependencies if a transitive dependency exists
-- detect transitive cyclic dependencies (and color them in output)
+- clean up a graph to remove direct dependencies if a transitive dependency exists and output it as dot-file.
+- detect transitive cyclic dependencies
+  - color them in the graph
+  - show them as separate graphs in one dot-file
+  - exit *pipforester* with exit code 1 if there are cycles detected
+
+### Installation:
+
+- Create an empty virtual environment, separate from the environment to work on.
+- `pip install pipdeptree pipforester`
+
+Dependent on your operation system you
+- want to install a program to view dot-files, like [xdot](https://pypi.org/project/xdot/) i.e. with `apt install xdot` on Debian/Ubuntu-based systems.
+- or use [graphviz](https://www.graphviz.org/) to convert dot-files to PNG/SVG.
 
-## Usage
 
-Important: *pipdeptree* **MUST** be installed in an environment together with the dependencies you want to check.  If you install *pipdeptree* in virtual environment 1 and then call it in the directory of virtual environment 2, it will only report on its own dependencies, which is not very useful.
+## Usage
 
-First, call *pipdeptree* to create a JSON file of the installed dependencies,
+First, call *pipdeptree* on a virtual environment to create a JSON file of the installed dependencies,
 and second call *pipforester* to create a cleaned-up dot file.
 
 ```shell
-pipdeptree -j >forest.json
+pipdeptree --python  path/to/venv/bin/python -j >forest.json
 pipforester -i forest.json -o forest.dot
 ```
 
 Finally use a Graphviz DOT-file visualizer, i.e. *xdot* on Linux, to view the graph.
-Or use the *dot* command line program to generate an svg or png:
+
+```
+xdot forest.dot
+```
+
+Or use the *dot* command line program to generate an SVG or PNG:
 
 ```
 dot -Tsvg -o forest.svg forest.dot
 dot -Tpng -o forest.png forest.dot
 ```
 
 To generate a graph containing only cyclic transitive dependencies, use the `--cycles` option:
```

### Comparing `pipforester-1.0.0a1/pipforester/__init__.py` & `pipforester-1.0.1/pipforester/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,10 +18,10 @@
             print("Cyclic dependencies detected")
             exit(1)
     elif cycles:
         graph = deptree.extract_cyclic_graph(graph)
     else:
         bad_edges = deptree.detect_cyclic_edges(graph)
         deptree.remove_cyclic_edges(graph, bad_edges)
-        deptree.remove_direct_edges(graph, ignore=bad_edges)
+        graph = deptree.remove_direct_edges(graph)
         deptree.add_cyclic_edges(graph, bad_edges)
     deptree.write_dotfile(graph, output)
```

### Comparing `pipforester-1.0.0a1/pipforester/deptree.py` & `pipforester-1.0.1/pipforester/deptree.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,76 +12,58 @@
     nx.nx_agraph.write_dot(G, filepath)
 
 
 def graph_from_json(data):
     G = nx.DiGraph()
     for pkgdef in data:
         pkg = pkgdef["package"]
-        deps = pkgdef["dependencies"]
         G.add_node(
             pkg["key"],
             installed_version=pkg["installed_version"],
             name=pkg["package_name"],
         )
         for dep in pkgdef["dependencies"]:
             G.add_edge(pkg["key"], dep["key"])
     return G
 
 
-def detect_cyclic_edges(G, mark=False):
+def detect_cyclic_edges(G):
     print("Detecting cyclic edges")
     bad_edges = set()
-    for cycle in nx.simple_cycles(G):
-        if mark:
-            for idx in range(len(cycle) - 1):
-                G.edges[cycle[idx], cycle[idx + 1]]["color"] = "darkviolet"
+    cycles = nx.simple_cycles(G)
+    for cycle in cycles:
+        for idx in range(len(cycle) - 1):
+            print(f"found edge {cycle[idx]} -> {cycle[idx + 1]}")
+            bad_edges.add((cycle[idx], cycle[idx + 1]))
         bad_edges.add((cycle[-1], cycle[0]))
     return bad_edges
 
 
 def extract_cyclic_graph(G):
     print("Extracting cyclic edges")
     CG = nx.DiGraph()
     bad_edges = set()
     for num, cycle in enumerate(nx.simple_cycles(G)):
         if (cycle[-1], cycle[0]) in bad_edges:
             continue
         for idx in range(len(cycle) - 1):
-            CG.add_edge(cycle[idx], cycle[idx + 1])
             CG.add_edge(f"{cycle[idx]} ({num})", f"{cycle[idx + 1]} ({num})")
         CG.add_edge(f"{cycle[-1]} ({num})", f"{cycle[0]} ({num})")
         bad_edges.add((cycle[-1], cycle[0]))
     return CG
 
+
 def remove_cyclic_edges(G, bad_edges):
     print("Removing cyclic edges")
     for edge in bad_edges:
         G.remove_edge(edge[0], edge[1])
 
 
 def add_cyclic_edges(G, bad_edges):
     print("Adding cyclic edges")
     for edge in bad_edges:
-        G.add_edge(edge[0], edge[1], color="darkviolet")
+        G.add_edge(edge[0], edge[1])
+        G.edges[edge[0], edge[1]]["color"] = "darkviolet"
 
 
-def remove_direct_edges(G, ignore=None):
-    print("Removing direct edges")
-    to_remove = []
-    if ignore is None:
-        ignore = []
-    for node in G.nodes():
-        # get all edges origin in node
-        print(f"  Node: {node}")
-        out_edges = list(G.out_edges(node))
-        for out_edge in out_edges:
-            if tuple(out_edge) in ignore:
-                print(f"  Ignore cyclic: {node}")
-                continue
-            print(f"    Out edge to {out_edge[1]}")
-            for path in nx.all_simple_paths(G, node, out_edge[1]):
-                # if there is a path from node to out_edge[1] that is longer than 1, then
-                # remove the edge
-                if len(path) > 2:
-                    print(f"    -> remove")
-                    G.remove_edge(out_edge[0], out_edge[1])
-                    break
+def remove_direct_edges(G):
+    return nx.transitive_reduction(G)
```

### Comparing `pipforester-1.0.0a1/pipforester.egg-info/PKG-INFO` & `pipforester-1.0.1/pipforester.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pipforester
-Version: 1.0.0a1
+Version: 1.0.1
 Summary: A tool to analyze the dependency graph of a pip package.
 Author-email: Jens Klein et al <jk@kleinundpartner.at>
 License: BSD 2-Clause License
 Project-URL: Homepage, https://github.com/collective/pipforester
 Project-URL: Bug Reports, https://github.com/collective/pipforester/issues
 Project-URL: Source, https://github.com/collective/pipforester/
 Keywords: pip,graph,analysis
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,35 +22,51 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
 
 # pipforester
 
-Forester tools for [pipdeptree](https://pypi.org/project/pipdeptree/) outputs to analyze the dependency graph of a pip package.
+Forester tools for [pipdeptree](https://pypi.org/project/pipdeptree/) outputs to analyze and cleanup the dependency graph of installed pip packages.
 
 ## Features
 
-- clean up a graph to remove direct dependencies if a transitive dependency exists
-- detect transitive cyclic dependencies (and color them in output)
+- clean up a graph to remove direct dependencies if a transitive dependency exists and output it as dot-file.
+- detect transitive cyclic dependencies
+  - color them in the graph
+  - show them as separate graphs in one dot-file
+  - exit *pipforester* with exit code 1 if there are cycles detected
+
+### Installation:
+
+- Create an empty virtual environment, separate from the environment to work on.
+- `pip install pipdeptree pipforester`
+
+Dependent on your operation system you
+- want to install a program to view dot-files, like [xdot](https://pypi.org/project/xdot/) i.e. with `apt install xdot` on Debian/Ubuntu-based systems.
+- or use [graphviz](https://www.graphviz.org/) to convert dot-files to PNG/SVG.
 
-## Usage
 
-Important: *pipdeptree* **MUST** be installed in an environment together with the dependencies you want to check.  If you install *pipdeptree* in virtual environment 1 and then call it in the directory of virtual environment 2, it will only report on its own dependencies, which is not very useful.
+## Usage
 
-First, call *pipdeptree* to create a JSON file of the installed dependencies,
+First, call *pipdeptree* on a virtual environment to create a JSON file of the installed dependencies,
 and second call *pipforester* to create a cleaned-up dot file.
 
 ```shell
-pipdeptree -j >forest.json
+pipdeptree --python  path/to/venv/bin/python -j >forest.json
 pipforester -i forest.json -o forest.dot
 ```
 
 Finally use a Graphviz DOT-file visualizer, i.e. *xdot* on Linux, to view the graph.
-Or use the *dot* command line program to generate an svg or png:
+
+```
+xdot forest.dot
+```
+
+Or use the *dot* command line program to generate an SVG or PNG:
 
 ```
 dot -Tsvg -o forest.svg forest.dot
 dot -Tpng -o forest.png forest.dot
 ```
 
 To generate a graph containing only cyclic transitive dependencies, use the `--cycles` option:
@@ -69,17 +85,27 @@
 ```
 
 See `pipforester --help` for details.
 
 
 ## Changes
 
-## 1.0.0a1 (2023-05-15)
+## 1.0.1 (2023-07-14)
+
+- use transitive_reduction from the NetworkX module to speed up edge removal. [@gogobd]
+
+### 1.0.0 (2023-05-16)
+
+- fix the cyclic dependency display to show all edges of a cycle in dark violet. [@jensens]
+- fix graph of cycles not to show graph multiple times. [@jensens]
+
+### 1.0.0a1 (2023-05-15)
+
+- initial code [@jensens]
 
-- initial code [jensens]
 # License
 
 Copyright (c) 2022-2023, mxstack Contributors
 
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
```

### Comparing `pipforester-1.0.0a1/pyproject.toml` & `pipforester-1.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 name = "pipforester"
 description = "A tool to analyze the dependency graph of a pip package."
-version = "1.0.0a1"
+version = "1.0.1"
 keywords = ["pip", "graph", "analysis"]
 authors = [
   {name = "Jens Klein et al", email = "jk@kleinundpartner.at" }
 ]
 requires-python = ">=3.7"
 license = { text = "BSD 2-Clause License" }
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Build Tools",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
```

