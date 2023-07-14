# Comparing `tmp/robingrad-0.0.1.tar.gz` & `tmp/robingrad-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robingrad-0.0.1.tar", last modified: Tue Jul 11 18:54:55 2023, max compression
+gzip compressed data, was "robingrad-0.0.2.tar", last modified: Fri Jul 14 10:03:58 2023, max compression
```

## Comparing `robingrad-0.0.1.tar` & `robingrad-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-11 18:54:55.751449 robingrad-0.0.1/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1060 2023-07-11 17:52:34.000000 robingrad-0.0.1/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2252 2023-07-11 18:54:55.751097 robingrad-0.0.1/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      591 2023-07-11 14:21:21.000000 robingrad-0.0.1/README.md
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      694 2023-07-11 18:53:48.000000 robingrad-0.0.1/pyproject.toml
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-11 18:54:55.748234 robingrad-0.0.1/robingrad/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       78 2023-07-09 12:38:46.000000 robingrad-0.0.1/robingrad/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1433 2023-07-11 13:08:02.000000 robingrad-0.0.1/robingrad/graph.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2122 2023-07-11 13:31:47.000000 robingrad-0.0.1/robingrad/lab.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     6040 2023-07-11 13:04:56.000000 robingrad-0.0.1/robingrad/tensor.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-11 18:54:55.750686 robingrad-0.0.1/robingrad.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2252 2023-07-11 18:54:55.000000 robingrad-0.0.1/robingrad.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      274 2023-07-11 18:54:55.000000 robingrad-0.0.1/robingrad.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-07-11 18:54:55.000000 robingrad-0.0.1/robingrad.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       15 2023-07-11 18:54:55.000000 robingrad-0.0.1/robingrad.egg-info/requires.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       10 2023-07-11 18:54:55.000000 robingrad-0.0.1/robingrad.egg-info/top_level.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-07-11 18:54:55.751546 robingrad-0.0.1/setup.cfg
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-14 10:03:58.284901 robingrad-0.0.2/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1060 2023-07-11 17:52:34.000000 robingrad-0.0.2/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2173 2023-07-14 10:03:58.284440 robingrad-0.0.2/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      512 2023-07-13 15:18:38.000000 robingrad-0.0.2/README.md
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      694 2023-07-12 14:06:21.000000 robingrad-0.0.2/pyproject.toml
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-14 10:03:58.280449 robingrad-0.0.2/robingrad/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       78 2023-07-14 10:03:44.000000 robingrad-0.0.2/robingrad/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1459 2023-07-12 20:52:44.000000 robingrad-0.0.2/robingrad/graph.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2267 2023-07-13 14:47:01.000000 robingrad-0.0.2/robingrad/lab.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-14 10:03:58.283136 robingrad-0.0.2/robingrad/nn/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      423 2023-07-13 16:36:34.000000 robingrad-0.0.2/robingrad/nn/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    10607 2023-07-14 10:01:34.000000 robingrad-0.0.2/robingrad/tensor.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-14 10:03:58.282620 robingrad-0.0.2/robingrad.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2173 2023-07-14 10:03:58.000000 robingrad-0.0.2/robingrad.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      320 2023-07-14 10:03:58.000000 robingrad-0.0.2/robingrad.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-07-14 10:03:58.000000 robingrad-0.0.2/robingrad.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       15 2023-07-14 10:03:58.000000 robingrad-0.0.2/robingrad.egg-info/requires.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       10 2023-07-14 10:03:58.000000 robingrad-0.0.2/robingrad.egg-info/top_level.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-07-14 10:03:58.285042 robingrad-0.0.2/setup.cfg
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-07-14 10:03:58.283616 robingrad-0.0.2/tests/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4840 2023-07-13 15:05:49.000000 robingrad-0.0.2/tests/test_tensor.py
```

### Comparing `robingrad-0.0.1/LICENSE` & `robingrad-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `robingrad-0.0.1/PKG-INFO` & `robingrad-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robingrad
-Version: 0.0.1
+Version: 0.0.2
 Summary: Something between Tinygrad and Micrograd
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2023 Marco Salvalaggio
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -18,15 +18,14 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Robingrad
 
 <h1 align="center">
-<img src="logo.png" width="200">
+<img src="logo.png" width="150">
 </h1><br>
 
 
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity) [![stability-wip](https://img.shields.io/badge/stability-wip-lightgrey.svg)](https://github.com/mkenney/software-guides/blob/master/STABILITY-BADGES.md#work-in-progress)
 
-*Despite lacking the ability to fly through the skies like **PyTorch** and **TensorFlow**, the Robin is still a formidable bird that is teeming with untapped potential waiting to be uncovered.* :wink:
-
+Something between [Tinygrad](https://github.com/tinygrad/tinygrad) and [Micrograd](https://github.com/karpathy/micrograd).
```

### Comparing `robingrad-0.0.1/pyproject.toml` & `robingrad-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "robingrad"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Marco Salvalaggio", email="mar.salvalaggio@gmail.com" },
 ]
 description = "Something between Tinygrad and Micrograd"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `robingrad-0.0.1/robingrad/graph.py` & `robingrad-0.0.2/robingrad/graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     nodes, edges = trace(root)
     dot = Digraph(format=format, graph_attr={'rankdir': rankdir})
 
     for n in nodes:
         if inspect:
             dot.node(name=str(id(n)), label=f"data: {np.round(n.data,4)} | grad: {np.round(n.grad,4)} | shape: {n.shape} | type: {n.data.dtype}", shape='record')
         else:
-            dot.node(name=str(id(n)), label=f"name: {n._origin} | shape: {n.shape} | type: {n.data.dtype}", shape='record')
+            dot.node(name=str(id(n)), label=f"name: {n._origin} | shape: {n.shape} | type: {n.data.dtype} | grad: {n.requires_grad}", shape='record')
         if n._op:
             dot.node(name=str(id(n)) + n._op, label=n._op)
             dot.edge(str(id(n)) + n._op, str(id(n)))
 
     for n1, n2 in edges:
         dot.edge(str(id(n1)), str(id(n2)) + n2._op)
```

### Comparing `robingrad-0.0.1/robingrad.egg-info/PKG-INFO` & `robingrad-0.0.2/robingrad.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robingrad
-Version: 0.0.1
+Version: 0.0.2
 Summary: Something between Tinygrad and Micrograd
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2023 Marco Salvalaggio
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -18,15 +18,14 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Robingrad
 
 <h1 align="center">
-<img src="logo.png" width="200">
+<img src="logo.png" width="150">
 </h1><br>
 
 
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity) [![stability-wip](https://img.shields.io/badge/stability-wip-lightgrey.svg)](https://github.com/mkenney/software-guides/blob/master/STABILITY-BADGES.md#work-in-progress)
 
-*Despite lacking the ability to fly through the skies like **PyTorch** and **TensorFlow**, the Robin is still a formidable bird that is teeming with untapped potential waiting to be uncovered.* :wink:
-
+Something between [Tinygrad](https://github.com/tinygrad/tinygrad) and [Micrograd](https://github.com/karpathy/micrograd).
```

