# Comparing `tmp/circuitree-0.3.0.tar.gz` & `tmp/circuitree-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitree-0.3.0.tar", max compression
+gzip compressed data, was "circuitree-0.3.1.tar", max compression
```

## Comparing `circuitree-0.3.0.tar` & `circuitree-0.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35149 2023-04-06 18:32:42.965443 circuitree-0.3.0/LICENSE
--rw-r--r--   0        0        0     1011 2023-06-09 16:36:39.964761 circuitree-0.3.0/README.md
--rwxr-xr-x   0        0        0      117 2023-06-23 05:39:39.142840 circuitree-0.3.0/circuitree/__init__.py
--rwxr-xr-x   0        0        0    15843 2023-06-23 06:25:24.652892 circuitree-0.3.0/circuitree/circuitree.py
--rwxr-xr-x   0        0        0    17012 2023-07-13 01:44:13.327169 circuitree-0.3.0/circuitree/models.py
--rw-r--r--   0        0        0     3991 2023-05-26 18:27:42.279204 circuitree-0.3.0/circuitree/modularity.py
--rw-r--r--   0        0        0     9417 2023-06-28 00:46:06.604507 circuitree-0.3.0/circuitree/parallel.py
--rw-r--r--   0        0        0      267 2023-05-26 18:24:06.289207 circuitree-0.3.0/circuitree/regret.py
--rw-r--r--   0        0        0      750 2023-05-13 02:24:31.319175 circuitree-0.3.0/circuitree/rewards.py
--rw-r--r--   0        0        0     1442 2023-06-23 05:30:14.382829 circuitree-0.3.0/circuitree/utils.py
--rw-r--r--   0        0        0    10391 2023-06-28 20:54:12.669759 circuitree-0.3.0/circuitree/viz.py
--rw-r--r--   0        0        0     1813 2023-07-13 01:45:02.237170 circuitree-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2525 1970-01-01 00:00:00.000000 circuitree-0.3.0/setup.py
--rw-r--r--   0        0        0     2530 1970-01-01 00:00:00.000000 circuitree-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-06 18:32:42.965443 circuitree-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1011 2023-06-09 16:36:39.964761 circuitree-0.3.1/README.md
+-rwxr-xr-x   0        0        0      117 2023-06-23 05:39:39.142840 circuitree-0.3.1/circuitree/__init__.py
+-rwxr-xr-x   0        0        0    15966 2023-07-13 21:38:18.014416 circuitree-0.3.1/circuitree/circuitree.py
+-rwxr-xr-x   0        0        0    17012 2023-07-13 01:44:13.327169 circuitree-0.3.1/circuitree/models.py
+-rw-r--r--   0        0        0     3991 2023-05-26 18:27:42.279204 circuitree-0.3.1/circuitree/modularity.py
+-rw-r--r--   0        0        0     9766 2023-07-14 02:05:56.385892 circuitree-0.3.1/circuitree/parallel.py
+-rw-r--r--   0        0        0      267 2023-05-26 18:24:06.289207 circuitree-0.3.1/circuitree/regret.py
+-rw-r--r--   0        0        0      750 2023-05-13 02:24:31.319175 circuitree-0.3.1/circuitree/rewards.py
+-rw-r--r--   0        0        0     1442 2023-06-23 05:30:14.382829 circuitree-0.3.1/circuitree/utils.py
+-rw-r--r--   0        0        0    10391 2023-06-28 20:54:12.669759 circuitree-0.3.1/circuitree/viz.py
+-rw-r--r--   0        0        0     1813 2023-07-14 19:52:18.408930 circuitree-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2525 1970-01-01 00:00:00.000000 circuitree-0.3.1/setup.py
+-rw-r--r--   0        0        0     2530 1970-01-01 00:00:00.000000 circuitree-0.3.1/PKG-INFO
```

### Comparing `circuitree-0.3.0/LICENSE` & `circuitree-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitree-0.3.0/README.md` & `circuitree-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `circuitree-0.3.0/circuitree/circuitree.py` & `circuitree-0.3.1/circuitree/circuitree.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,14 +184,18 @@
 
     def accumulate_visits_and_rewards(self, graph: Optional[nx.DiGraph] = None):
         _accumulated = self.graph if graph is None else graph
         accumulate_visits_and_rewards(_accumulated)
         if graph is None:
             return _accumulated
 
+    @property
+    def terminal_states(self):
+        return (node for node in self.graph.nodes if self.is_terminal(node))
+
     def search_mcts(
         self,
         n_steps: int,
         root: Optional[Any] = None,
         metric_func: Optional[Callable] = None,
         save_every: int = 1,
         exploration_constant: Optional[float] = None,
```

### Comparing `circuitree-0.3.0/circuitree/models.py` & `circuitree-0.3.1/circuitree/models.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.3.0/circuitree/modularity.py` & `circuitree-0.3.1/circuitree/modularity.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.3.0/circuitree/parallel.py` & `circuitree-0.3.1/circuitree/parallel.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,19 +2,15 @@
 from pathlib import Path
 from typing import Any, Callable, Iterable, Mapping, Optional
 import numpy as np
 import pandas as pd
 
 from .utils import DefaultFactoryDict, DefaultMapping
 
-__all__ = [
-    "MCTSResult",
-    "ResultsRegistry",
-    "TranspositionTable"
-]
+__all__ = ["MCTSResult", "ResultsRegistry", "TranspositionTable"]
 
 
 @dataclass
 class MCTSResult:
     reward: float
     initial_conditions: Iterable[float | int]
     params: Iterable[float | int]
@@ -134,14 +130,18 @@
                 return state in self.table and visit < len(self.table[state])
             case state:
                 return state in self.table
 
     def __len__(self):
         return len(self.table)
 
+    @property
+    def shape(self):
+        return len(self.table), self.ncols
+
     def n_visits(self, state):
         """Return number of visits with triggering a default factory call."""
         if state in self.table:
             return len(self.table[state])
         else:
             return 0
 
@@ -203,14 +203,21 @@
                     [read_func(f, **load_kw) for f in tqdm(src, desc="Loading data")]
                 )
             else:
                 df = pd.concat([read_func(f, **load_kw) for f in src])
         else:
             df = read_func(src, **load_kw)
 
+        if "state" not in df.columns:
+            if df.index.name == "state":
+                df = df.reset_index()
+            else:
+                raise ValueError(
+                    "Dataframe must have a 'state' column or have 'state' as the index."
+                )
         df["state"] = pd.Categorical(df["state"])
         if visit_col not in df.columns:
             df[visit_col] = df.groupby("state").cumcount()
 
         return cls.from_dataframe(df, visit_column=visit_col, **kwargs)
 
     @classmethod
@@ -242,24 +249,24 @@
         cls,
         df: pd.DataFrame,
         init_columns: Optional[Iterable[str]] = None,
         param_columns: Optional[Iterable[str]] = None,
         visit_column: str = "visit",
         reward_column: str = "reward",
         state_column: str = "state",
+        **kwargs,
     ):
         table = DefaultFactoryDict(default_factory=ResultsRegistry)
         init_columns = init_columns or []
         param_columns = param_columns or []
         for state, state_table in df.sort_values(visit_column).groupby(state_column):
-            rewards = state_table[reward_column]
+            rewards = state_table[reward_column].abs()
             init_conds = state_table[init_columns].values
             params = state_table[param_columns].values
             table[state].extend(zip(rewards, init_conds, params))
-            ...
 
         colnames = [reward_column] + list(init_columns) + list(param_columns)
         return cls(results_colnames=colnames, table=table)
 
     def to_dataframe(self):
         data = {
             state: pd.DataFrame([v.unpack() for v in res], columns=self.columns)
```

### Comparing `circuitree-0.3.0/circuitree/rewards.py` & `circuitree-0.3.1/circuitree/rewards.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.3.0/circuitree/utils.py` & `circuitree-0.3.1/circuitree/utils.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.3.0/circuitree/viz.py` & `circuitree-0.3.1/circuitree/viz.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.3.0/pyproject.toml` & `circuitree-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "circuitree"
-version = "0.3.0"
+version = "0.3.1"
 description = "Genetic circuit design using Monte Carlo tree search"
 authors = ["pranav-bhamidipati <pbhamidi@usc.edu>"]
 license = "GPLv3"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `circuitree-0.3.0/setup.py` & `circuitree-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
               'pandas>=2.0.0,<3.0.0',
               'tables>=3.8.0,<4.0.0',
               'pyarrow>=12.0.0,<13.0.0',
               'h5py>=3.8.0,<4.0.0']}
 
 setup_kwargs = {
     'name': 'circuitree',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'Genetic circuit design using Monte Carlo tree search',
     'long_description': '# CircuiTree\nGenetic circuit design using Monte Carlo tree search\n\n## Installation\n\n### From a package repository\nTo install using `pip`:\n\n```pip install circuitree```\n\n### From the GitHub repository\n\nTo install and use `circuitree` from the GitHub source code, first clone the repo into a directory.\n\n```git clone https://github.com/pranav-bhamidipati/circuitree.git[ dir_name]```\n\nThen, you can build the environment using the command-line tool `poetry`. Instructions for installation can be [found here](https://python-poetry.org/). \n\nFrom the main project directory, run `poetry install` to install a virtual environment with `circuitree` installed. The easiest way to use this environment is to run it interactively with `poetry shell`. Alternatively, you can run a command in the virtual environment with `poetry run <command>`. For instance, to launch a Jupyter notebook with `circuitree` pre-loaded, run `poetry run jupyter notebook`. \n\n## Usage\n\nSee the [quick-start demo](examples/quick_start.ipynb).\n',
     'author': 'pranav-bhamidipati',
     'author_email': 'pbhamidi@usc.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `circuitree-0.3.0/PKG-INFO` & `circuitree-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitree
-Version: 0.3.0
+Version: 0.3.1
 Summary: Genetic circuit design using Monte Carlo tree search
 License: GPLv3
 Author: pranav-bhamidipati
 Author-email: pbhamidi@usc.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

