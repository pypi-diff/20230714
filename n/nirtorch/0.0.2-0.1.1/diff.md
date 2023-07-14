# Comparing `tmp/nirtorch-0.0.2.tar.gz` & `tmp/nirtorch-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nirtorch-0.0.2.tar", last modified: Tue Jul 11 22:23:36 2023, max compression
+gzip compressed data, was "nirtorch-0.1.1.tar", last modified: Fri Jul 14 00:55:24 2023, max compression
```

## Comparing `nirtorch-0.0.2.tar` & `nirtorch-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 jens      (1003) jens      (1003)        0 2023-07-11 22:23:36.702988 nirtorch-0.0.2/
--rw-rw-r--   0 jens      (1003) jens      (1003)     3070 2023-07-11 22:23:36.702988 nirtorch-0.0.2/PKG-INFO
--rw-rw-r--   0 jens      (1003) jens      (1003)     2010 2023-07-11 22:20:12.000000 nirtorch-0.0.2/README.md
-drwxrwxr-x   0 jens      (1003) jens      (1003)        0 2023-07-11 22:23:36.698988 nirtorch-0.0.2/nirtorch/
--rw-rw-r--   0 jens      (1003) jens      (1003)       91 2023-07-11 22:20:12.000000 nirtorch-0.0.2/nirtorch/__init__.py
--rw-rw-r--   0 jens      (1003) jens      (1003)     4182 2023-07-11 22:20:12.000000 nirtorch-0.0.2/nirtorch/from_nir.py
--rw-rw-r--   0 jens      (1003) jens      (1003)    12733 2023-07-11 22:20:12.000000 nirtorch-0.0.2/nirtorch/graph.py
--rw-rw-r--   0 jens      (1003) jens      (1003)     2206 2023-07-11 22:20:12.000000 nirtorch-0.0.2/nirtorch/graph_utils.py
--rw-rw-r--   0 jens      (1003) jens      (1003)     2885 2023-07-11 22:20:12.000000 nirtorch-0.0.2/nirtorch/to_nir.py
-drwxrwxr-x   0 jens      (1003) jens      (1003)        0 2023-07-11 22:23:36.702988 nirtorch-0.0.2/nirtorch.egg-info/
--rw-rw-r--   0 jens      (1003) jens      (1003)     3070 2023-07-11 22:23:36.000000 nirtorch-0.0.2/nirtorch.egg-info/PKG-INFO
--rw-rw-r--   0 jens      (1003) jens      (1003)      350 2023-07-11 22:23:36.000000 nirtorch-0.0.2/nirtorch.egg-info/SOURCES.txt
--rw-rw-r--   0 jens      (1003) jens      (1003)        1 2023-07-11 22:23:36.000000 nirtorch-0.0.2/nirtorch.egg-info/dependency_links.txt
--rw-rw-r--   0 jens      (1003) jens      (1003)       10 2023-07-11 22:23:36.000000 nirtorch-0.0.2/nirtorch.egg-info/requires.txt
--rw-rw-r--   0 jens      (1003) jens      (1003)        9 2023-07-11 22:23:36.000000 nirtorch-0.0.2/nirtorch.egg-info/top_level.txt
--rw-rw-r--   0 jens      (1003) jens      (1003)     1265 2023-07-11 22:20:12.000000 nirtorch-0.0.2/pyproject.toml
--rw-rw-r--   0 jens      (1003) jens      (1003)       38 2023-07-11 22:23:36.702988 nirtorch-0.0.2/setup.cfg
-drwxrwxr-x   0 jens      (1003) jens      (1003)        0 2023-07-11 22:23:36.702988 nirtorch-0.0.2/tests/
--rw-rw-r--   0 jens      (1003) jens      (1003)     1427 2023-07-11 22:20:12.000000 nirtorch-0.0.2/tests/test_from_nir.py
--rw-rw-r--   0 jens      (1003) jens      (1003)     7367 2023-07-11 22:20:12.000000 nirtorch-0.0.2/tests/test_graph.py
--rw-rw-r--   0 jens      (1003) jens      (1003)     3170 2023-07-11 22:20:12.000000 nirtorch-0.0.2/tests/test_to_nir.py
+drwxrwxr-x   0 jens      (1003) jens      (1003)        0 2023-07-14 00:55:24.644890 nirtorch-0.1.1/
+-rw-rw-r--   0 jens      (1003) jens      (1003)     3534 2023-07-14 00:55:24.640890 nirtorch-0.1.1/PKG-INFO
+-rw-rw-r--   0 jens      (1003) jens      (1003)     2474 2023-07-13 23:20:41.000000 nirtorch-0.1.1/README.md
+drwxrwxr-x   0 jens      (1003) jens      (1003)        0 2023-07-14 00:55:24.640890 nirtorch-0.1.1/nirtorch/
+-rw-rw-r--   0 jens      (1003) jens      (1003)       91 2023-07-13 23:20:41.000000 nirtorch-0.1.1/nirtorch/__init__.py
+-rw-rw-r--   0 jens      (1003) jens      (1003)     4167 2023-07-13 23:20:41.000000 nirtorch-0.1.1/nirtorch/from_nir.py
+-rw-rw-r--   0 jens      (1003) jens      (1003)    12742 2023-07-13 23:29:20.000000 nirtorch-0.1.1/nirtorch/graph.py
+-rw-rw-r--   0 jens      (1003) jens      (1003)     2164 2023-07-13 23:20:41.000000 nirtorch-0.1.1/nirtorch/graph_utils.py
+-rw-rw-r--   0 jens      (1003) jens      (1003)     2889 2023-07-13 23:28:58.000000 nirtorch-0.1.1/nirtorch/to_nir.py
+drwxrwxr-x   0 jens      (1003) jens      (1003)        0 2023-07-14 00:55:24.640890 nirtorch-0.1.1/nirtorch.egg-info/
+-rw-rw-r--   0 jens      (1003) jens      (1003)     3534 2023-07-14 00:55:24.000000 nirtorch-0.1.1/nirtorch.egg-info/PKG-INFO
+-rw-rw-r--   0 jens      (1003) jens      (1003)      375 2023-07-14 00:55:24.000000 nirtorch-0.1.1/nirtorch.egg-info/SOURCES.txt
+-rw-rw-r--   0 jens      (1003) jens      (1003)        1 2023-07-14 00:55:24.000000 nirtorch-0.1.1/nirtorch.egg-info/dependency_links.txt
+-rw-rw-r--   0 jens      (1003) jens      (1003)       10 2023-07-14 00:55:24.000000 nirtorch-0.1.1/nirtorch.egg-info/requires.txt
+-rw-rw-r--   0 jens      (1003) jens      (1003)        9 2023-07-14 00:55:24.000000 nirtorch-0.1.1/nirtorch.egg-info/top_level.txt
+-rw-rw-r--   0 jens      (1003) jens      (1003)     1265 2023-07-14 00:53:24.000000 nirtorch-0.1.1/pyproject.toml
+-rw-rw-r--   0 jens      (1003) jens      (1003)       38 2023-07-14 00:55:24.644890 nirtorch-0.1.1/setup.cfg
+drwxrwxr-x   0 jens      (1003) jens      (1003)        0 2023-07-14 00:55:24.640890 nirtorch-0.1.1/tests/
+-rw-rw-r--   0 jens      (1003) jens      (1003)     1231 2023-07-14 00:51:45.000000 nirtorch-0.1.1/tests/test_conversion.py
+-rw-rw-r--   0 jens      (1003) jens      (1003)     1426 2023-07-13 23:20:41.000000 nirtorch-0.1.1/tests/test_from_nir.py
+-rw-rw-r--   0 jens      (1003) jens      (1003)     7401 2023-07-14 00:51:45.000000 nirtorch-0.1.1/tests/test_graph.py
+-rw-rw-r--   0 jens      (1003) jens      (1003)     3170 2023-07-13 23:20:41.000000 nirtorch-0.1.1/tests/test_to_nir.py
```

### Comparing `nirtorch-0.0.2/PKG-INFO` & `nirtorch-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nirtorch
-Version: 0.0.2
+Version: 0.1.1
 Summary: Neuromorphic Intermediate Representation
 Author-email: Steven Abreu <s.abreu@rug.nl>, Felix Bauer <felix.bauer@synsen.ai>, Jason Eshraghian <jeshragh@ucsc.edu>, Matthias Jobst <matthias.jobst2@tu-dresden.de>, Gregor Lenz <mail@lenzgregor.com>, Jens Egholm Pedersen <jens@jepedersen.dk>, Sadique Sheik <sadique.sheik@synsense.ai>
 Keywords: neuromorphic,intermediate,representation
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
@@ -74,7 +74,18 @@
   year         = 2023,
   publisher    = {Zenodo},
   version      = {0.0.1},
   doi          = {10.5281/zenodo.8105042},
   url          = {https://doi.org/10.5281/zenodo.8105042}
 }
 ```
+
+## For developers
+If you want to make sure that your code is linted correctly on your local machine, use [pre-commit](https://pre-commit.com/) to automatically perform checks before every git commit. To use it, first install the package in your environment
+```
+pip install pre-commit
+```
+and then install the pre-commit hooks that are listed in the root of this repository
+```
+pre-commit install
+```
+Next time you commit some changes, all the checks will be run!
```

### Comparing `nirtorch-0.0.2/README.md` & `nirtorch-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -56,7 +56,18 @@
   year         = 2023,
   publisher    = {Zenodo},
   version      = {0.0.1},
   doi          = {10.5281/zenodo.8105042},
   url          = {https://doi.org/10.5281/zenodo.8105042}
 }
 ```
+
+## For developers
+If you want to make sure that your code is linted correctly on your local machine, use [pre-commit](https://pre-commit.com/) to automatically perform checks before every git commit. To use it, first install the package in your environment
+```
+pip install pre-commit
+```
+and then install the pre-commit hooks that are listed in the root of this repository
+```
+pre-commit install
+```
+Next time you commit some changes, all the checks will be run!
```

### Comparing `nirtorch-0.0.2/nirtorch/from_nir.py` & `nirtorch-0.1.1/nirtorch/from_nir.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from .graph import Graph, Node
 
 
 def execution_order_up_to_node(
     node: Node, graph: Graph, execution_order: List[Node]
 ) -> List[Node]:
-    """Recursive function to evaluate execution order until a given node
+    """Recursive function to evaluate execution order until a given node.
 
     Args:
         node (Node): Execution order for the node of interest
         graph (Graph): Graph object describing the network
         execution_order (List[Node]): The current known execution order.
 
     Returns:
@@ -36,17 +36,15 @@
         self.graph = graph
         self.instantiate_modules()
         self.execution_order = self.get_execution_order()
         if len(self.execution_order) == 0:
             raise ValueError("Graph is empty")
 
     def get_execution_order(self) -> List[Node]:
-        """
-        Evaluate the execution order and instantiate that as a list
-        """
+        """Evaluate the execution order and instantiate that as a list."""
         execution_order = []
         # Then loop over all nodes and check that they are added to the execution order.
         for node in self.graph.node_list:
             if node not in execution_order:
                 execution_order = execution_order_up_to_node(
                     node, self.graph, execution_order
                 )
@@ -96,15 +94,15 @@
     nodes = [model_map(node) for node in nir_graph.nodes]
     return nir.NIRGraph(nodes, nir_graph.edges)
 
 
 def load(
     nir_graph: nir.NIRNode, model_map: Callable[[nir.NIRNode], nn.Module]
 ) -> nn.Module:
-    """Load a NIR object and convert it to a torch module using the given model map
+    """Load a NIR object and convert it to a torch module using the given model map.
 
     Args:
         nir_graph (nir.NIRNode): NIR object
         model_map (Callable[[nn.NIRNode], nn.Module]): A method that returns the a torch
             module that corresponds to each NIR node.
 
     Returns:
```

### Comparing `nirtorch-0.0.2/nirtorch/graph.py` & `nirtorch-0.1.1/nirtorch/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import torch
 import torch.nn as nn
 
 
 def named_modules_map(
     model: nn.Module, model_name: Optional[str] = "model"
 ) -> Dict[str, nn.Module]:
-    """Inverse of named modules dictionary
+    """Inverse of named modules dictionary.
 
     Args:
         model (nn.Module): The module to be hashed
         model_name (str | None): Name of the top level module. If this doesn't need
             to be include, this option can be set to None
 
     Returns:
@@ -155,15 +155,16 @@
                     child_in_graph = True
                     break
             if child_in_graph:
                 del filtered_module_names[mod]
         return filtered_module_names
 
     def _is_mod_and_not_in_module_names(self, elem: Any) -> bool:
-        """Check if a node is a module and is included in the module_names of this graph
+        """Check if a node is a module and is included in the module_names of this
+        graph.
 
         Args:
             node (Node): Node to verify
 
         Returns:
             bool
         """
@@ -226,15 +227,15 @@
                 new_named_modules[mod] = name
         # Create a new graph with the allowed modules
         new_graph = Graph(new_named_modules)
         new_graph.populate_from(self)
         return new_graph
 
     def find_source_nodes_of(self, node: Node) -> List[Node]:
-        """Find all the sources of a node in the graph
+        """Find all the sources of a node in the graph.
 
         Args:
             node (Node): Node of interest
 
         Returns:
             List[Node]: A list of all nodes that have this node as outgoing_node
         """
@@ -242,15 +243,15 @@
         for source_node in self.node_list:
             for outnode in source_node.outgoing_nodes:
                 if node == outnode:
                     source_node_list.append(source_node)
         return source_node_list
 
     def ignore_tensors(self) -> "Graph":
-        """Simplify the graph by ignoring all the tensors in it
+        """Simplify the graph by ignoring all the tensors in it.
 
         Returns:
             Graph: Returns a simplified graph with only modules in it
         """
         return self.ignore_nodes(torch.Tensor)
 
     def ignore_nodes(self, class_type: Type) -> "Graph":
@@ -283,15 +284,15 @@
                 # already filtered
                 for outnode in node.outgoing_nodes:
                     if not isinstance(outnode.elem, class_type):
                         graph.add_edge(node.elem, outnode.elem)
         return graph
 
     def get_root(self) -> List[Node]:
-        """Returns the root node/s of the graph
+        """Returns the root node/s of the graph.
 
         Returns:
             List[Node]: A list of root nodes for the graph.
         """
         roots = []
         for node in self.node_list:
             sources = self.find_source_nodes_of(node)
@@ -322,16 +323,15 @@
             model_graph.add_edge(mod, output_data)
         return out
 
     return my_forward
 
 
 class GraphTracer:
-    """
-    Context manager to trace a model's execution graph
+    """Context manager to trace a model's execution graph.
 
     Example:
 
     ```python
     with GraphTracer(mymodel) as tracer, torch.no_grad():
         out = mymodel(data)
```

### Comparing `nirtorch-0.0.2/nirtorch/graph_utils.py` & `nirtorch-0.1.1/nirtorch/graph_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,21 @@
 def find_children(node, edges):
-    """
-    Given a node and the edges of a graph, find all direct children of
-    that node.
-    """
+    """Given a node and the edges of a graph, find all direct children of that node."""
     return set(child for (parent, child) in edges if parent == node)
 
 
 def find_parents(node, edges):
-    """
-    Given a node and the edges of a graph, find all direct parents of
-    that node.
-    """
+    """Given a node and the edges of a graph, find all direct parents of that node."""
     return set(parent for (parent, child) in edges if child == node)
 
 
 def find_all_ancestors(
     node, edges, roots=None, parents_found=None, nodes_inspected=None
 ):
-    """
-    Given a node and the edges of a graph, find all ancesters of
-    that node.
-    """
+    """Given a node and the edges of a graph, find all ancesters of that node."""
     roots = roots  # or find_roots(edges)
     if node in roots:
         return set()
 
     parents_found = parents_found or set()
     nodes_inspected = nodes_inspected or set()
     if node in nodes_inspected:
```

### Comparing `nirtorch-0.0.2/nirtorch/to_nir.py` & `nirtorch-0.1.1/nirtorch/to_nir.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from typing import Any, Optional, Callable
+from typing import Any, Callable, Optional
 
-import torch.nn as nn
 import nir
 import numpy as np
+import torch.nn as nn
 
 from .graph import extract_torch_graph
 
 
 def extract_nir_graph(
     model: nn.Module,
     model_map: Callable[[nn.Module], nir.NIRNode],
@@ -73,13 +73,13 @@
     outputs = []
 
     # Get all the edges
     for node in torch_graph.node_list:
         for destination in node.outgoing_nodes:
             nir_edges.append((indices[node], indices[destination]))
         if len(node.outgoing_nodes) == 0:
-            output_node = nir.Output()
+            output_node = nir.Output(None)
             outputs.append(output_node)
             nir_nodes.append(output_node)
             nir_edges.append((indices[node], len(nir_nodes) - 1))
 
     return nir.NIRGraph(nir_nodes, nir_edges)
```

### Comparing `nirtorch-0.0.2/nirtorch.egg-info/PKG-INFO` & `nirtorch-0.1.1/nirtorch.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nirtorch
-Version: 0.0.2
+Version: 0.1.1
 Summary: Neuromorphic Intermediate Representation
 Author-email: Steven Abreu <s.abreu@rug.nl>, Felix Bauer <felix.bauer@synsen.ai>, Jason Eshraghian <jeshragh@ucsc.edu>, Matthias Jobst <matthias.jobst2@tu-dresden.de>, Gregor Lenz <mail@lenzgregor.com>, Jens Egholm Pedersen <jens@jepedersen.dk>, Sadique Sheik <sadique.sheik@synsense.ai>
 Keywords: neuromorphic,intermediate,representation
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
@@ -74,7 +74,18 @@
   year         = 2023,
   publisher    = {Zenodo},
   version      = {0.0.1},
   doi          = {10.5281/zenodo.8105042},
   url          = {https://doi.org/10.5281/zenodo.8105042}
 }
 ```
+
+## For developers
+If you want to make sure that your code is linted correctly on your local machine, use [pre-commit](https://pre-commit.com/) to automatically perform checks before every git commit. To use it, first install the package in your environment
+```
+pip install pre-commit
+```
+and then install the pre-commit hooks that are listed in the root of this repository
+```
+pre-commit install
+```
+Next time you commit some changes, all the checks will be run!
```

### Comparing `nirtorch-0.0.2/pyproject.toml` & `nirtorch-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools"]
 
 [project]
 name = "nirtorch"
-version = "0.0.2"
+version = "0.1.1"
 description = "Neuromorphic Intermediate Representation"
 authors = [
   { name = "Steven Abreu", email = "s.abreu@rug.nl" },
   { name = "Felix Bauer", email = "felix.bauer@synsen.ai" },
   { name = "Jason Eshraghian", email = "jeshragh@ucsc.edu" },
   { name = "Matthias Jobst", email = "matthias.jobst2@tu-dresden.de" },
   { name = "Gregor Lenz", email = "mail@lenzgregor.com" },
```

### Comparing `nirtorch-0.0.2/tests/test_from_nir.py` & `nirtorch-0.1.1/tests/test_from_nir.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-import torch
+import nir
 import norse
+import pytest
+import torch
 
-import nir
 from nirtorch.from_nir import load
 
-import pytest
-
 
 def _torch_model_map(m: nir.NIRNode, device: str = "cpu") -> torch.nn.Module:
     if isinstance(m, nir.Affine):
         lin = torch.nn.Linear(*m.weight.shape[-2:])
         lin.weight.data = torch.tensor(m.weight, device=device)
         lin.bias.data = torch.tensor(m.bias, device=device)
         return lin
```

### Comparing `nirtorch-0.0.2/tests/test_graph.py` & `nirtorch-0.1.1/tests/test_graph.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-import torch.nn as nn
+import pytest
 import torch
-
-from sinabs.layers import Merge
+import torch.nn as nn
 from norse.torch import LIFCell, SequentialState
-import pytest
+from sinabs.layers import Merge
 
 
 class TupleModule(torch.nn.Module):
     def forward(self, data):
         return (data, data)
 
 
@@ -34,15 +33,15 @@
     ).ignore_tensors()
     print(graph)
 
     assert len(graph.node_list) == 11
 
 
 # Branched model
-class MyBranchedModel(nn.Module):
+class SinabsBranchedModel(nn.Module):
     def __init__(self) -> None:
         super().__init__()
         self.relu1 = nn.ReLU()
         self.relu2_1 = nn.ReLU()
         self.relu2_2 = nn.ReLU()
         self.add_mod = Merge()
         self.relu3 = nn.ReLU()
@@ -52,15 +51,15 @@
         out2_1 = self.relu2_1(out1)
         out2_2 = self.relu2_2(out1)
         out3 = self.add_mod(out2_1, out2_2)
         out4 = self.relu3(out3)
         return out4
 
 
-class MyStatefulModel(nn.Module):
+class NorseStatefulModel(nn.Module):
     def __init__(self) -> None:
         super().__init__()
         self.relu1 = nn.ReLU()
         self.lif = SequentialState(LIFCell())
 
     def forward(self, data):
         out1 = self.relu1(data)
@@ -69,22 +68,22 @@
 
 
 input_shape = (2, 28, 28)
 batch_size = 1
 
 data = torch.ones((batch_size, *input_shape))
 
-my_branched_model = MyBranchedModel()
+my_branched_model = SinabsBranchedModel()
 
 
 class DeepModel(nn.Module):
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
-        self.block1 = MyBranchedModel()
-        self.block2 = MyBranchedModel()
+        self.block1 = SinabsBranchedModel()
+        self.block2 = SinabsBranchedModel()
 
     def forward(self, data):
         out = self.block1(data)
         out2 = self.block2(out)
         return out2
 
 
@@ -98,15 +97,15 @@
     print(mod_map)
     for k, v in mod_map.items():
         assert isinstance(k, nn.Module)
         assert isinstance(v, str)
 
 
 def test_module_forward_wrapper():
-    mymodel = MyBranchedModel()
+    mymodel = SinabsBranchedModel()
 
     orig_call = nn.Module.__call__
 
     from nirtorch.graph import Graph, module_forward_wrapper, named_modules_map
 
     model_graph = Graph(named_modules_map(mymodel))
     new_call = module_forward_wrapper(model_graph)
@@ -157,23 +156,24 @@
 def test_ignore_submodules_of():
     from nirtorch.graph import GraphTracer, named_modules_map
 
     with GraphTracer(named_modules_map(mydeepmodel)) as tracer, torch.no_grad():
         _ = mydeepmodel(data)
 
     top_overview_graph = tracer.graph.ignore_submodules_of(
-        [MyBranchedModel]
+        [SinabsBranchedModel]
     ).leaf_only()
     print(top_overview_graph)
     assert len(top_overview_graph.node_list) == 2 + 2 + 1
 
 
 def test_snn_branched():
-    from sinabs.layers import IAFSqueeze, ChannelShift, SumPool2d
+    from sinabs.layers import ChannelShift, IAFSqueeze, SumPool2d
     from torch.nn import Conv2d
+
     from nirtorch.graph import extract_torch_graph
 
     class MySNN(nn.Module):
         def __init__(self) -> None:
             super().__init__()
             self.conv1 = Conv2d(2, 8, 3, bias=False)
             self.iaf1 = IAFSqueeze(batch_size=1)
@@ -215,15 +215,15 @@
     print(graph)
     assert len(graph.node_list) == 27  # 2*13 + 1
 
 
 def test_snn_stateful():
     from nirtorch.graph import extract_torch_graph
 
-    model = MyStatefulModel()
+    model = NorseStatefulModel()
     graph = extract_torch_graph(model, sample_data=torch.rand((1, 2, 3, 4)))
     assert len(graph.node_list) == 7  # 2 + 1 nested + 4 tensors
 
 
 def test_ignore_tensors():
     from nirtorch.graph import extract_torch_graph
 
@@ -255,12 +255,12 @@
 def test_ignore_nodes_parent_model():
     from nirtorch.graph import extract_torch_graph
 
     graph = extract_torch_graph(
         my_branched_model, sample_data=data, model_name="ShouldDisappear"
     )
 
-    new_graph = graph.ignore_nodes(MyBranchedModel)
+    new_graph = graph.ignore_nodes(SinabsBranchedModel)
     print(new_graph)
 
     with pytest.raises(ValueError):
         new_graph.find_node(my_branched_model)
```

### Comparing `nirtorch-0.0.2/tests/test_to_nir.py` & `nirtorch-0.1.1/tests/test_to_nir.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+import nir
+import numpy as np
 import torch
 import torch.nn as nn
-import numpy as np
 
-import nir
 from nirtorch.to_nir import extract_nir_graph
 
 
 def test_extract_single():
     m = nn.Linear(1, 1)
     g = extract_nir_graph(
         m,
```

