# Comparing `tmp/linsolve-1.1.0.tar.gz` & `tmp/linsolve-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linsolve-1.1.0.tar", last modified: Mon Jun  6 15:11:03 2022, max compression
+gzip compressed data, was "linsolve-1.1.2.tar", last modified: Fri Jul 14 13:46:48 2023, max compression
```

## Comparing `linsolve-1.1.0.tar` & `linsolve-1.1.2.tar`

### file list

```diff
@@ -1,32 +1,47 @@
-drwxrwxr-x   0 aparsons  (1000) aparsons  (1000)        0 2022-06-06 15:11:03.137432 linsolve-1.1.0/
--rw-r--r--   0 aparsons  (1000) aparsons  (1000)       94 2020-04-12 05:31:56.000000 linsolve-1.1.0/.coveragerc
--rw-rw-r--   0 aparsons  (1000) aparsons  (1000)      106 2021-02-14 16:50:33.000000 linsolve-1.1.0/.gitignore
--rw-r--r--   0 aparsons  (1000) aparsons  (1000)     1100 2020-04-12 05:31:56.000000 linsolve-1.1.0/LICENSE
--rw-r--r--   0 aparsons  (1000) aparsons  (1000)       63 2020-04-12 05:31:56.000000 linsolve-1.1.0/MANIFEST.in
--rw-rw-r--   0 aparsons  (1000) aparsons  (1000)      541 2022-06-06 15:11:03.137432 linsolve-1.1.0/PKG-INFO
--rw-rw-r--   0 aparsons  (1000) aparsons  (1000)     4706 2021-02-14 16:50:33.000000 linsolve-1.1.0/README.md
-drwxrwxr-x   0 aparsons  (1000) aparsons  (1000)        0 2022-06-06 15:11:03.133432 linsolve-1.1.0/imgs/
--rw-r--r--   0 aparsons  (1000) aparsons  (1000)    72241 2020-04-12 05:31:56.000000 linsolve-1.1.0/imgs/linear_model.png
--rw-r--r--   0 aparsons  (1000) aparsons  (1000)    16889 2020-04-12 05:31:56.000000 linsolve-1.1.0/imgs/points.png
-drwxrwxr-x   0 aparsons  (1000) aparsons  (1000)        0 2022-06-06 15:11:03.133432 linsolve-1.1.0/linsolve/
--rw-r--r--   0 aparsons  (1000) aparsons  (1000)       16 2022-06-06 15:11:02.000000 linsolve-1.1.0/linsolve/GIT_INFO
--rw-rw-r--   0 aparsons  (1000) aparsons  (1000)        6 2021-02-14 16:30:36.000000 linsolve-1.1.0/linsolve/VERSION
--rw-rw-r--   0 aparsons  (1000) aparsons  (1000)       77 2021-02-14 16:30:36.000000 linsolve-1.1.0/linsolve/__init__.py
--rw-rw-r--   0 aparsons  (1000) aparsons  (1000)    44488 2021-08-24 23:53:08.000000 linsolve-1.1.0/linsolve/linsolve.py
-drwxrwxr-x   0 aparsons  (1000) aparsons  (1000)        0 2022-06-06 15:11:03.137432 linsolve-1.1.0/linsolve/tests/
--rw-rw-r--   0 aparsons  (1000) aparsons  (1000)      777 2021-02-14 16:30:36.000000 linsolve-1.1.0/linsolve/tests/benchmark_A_large_shared.py
--rw-rw-r--   0 aparsons  (1000) aparsons  (1000)      845 2021-02-14 16:30:36.000000 linsolve-1.1.0/linsolve/tests/benchmark_A_large_shared_sparse.py
--rw-rw-r--   0 aparsons  (1000) aparsons  (1000)      745 2021-02-14 16:30:36.000000 linsolve-1.1.0/linsolve/tests/benchmark_A_small_shared.py
--rw-rw-r--   0 aparsons  (1000) aparsons  (1000)      824 2021-02-14 16:30:36.000000 linsolve-1.1.0/linsolve/tests/benchmark_A_small_shared_sparse.py
--rw-rw-r--   0 aparsons  (1000) aparsons  (1000)      899 2021-02-14 16:30:36.000000 linsolve-1.1.0/linsolve/tests/benchmark_A_small_unique.py
--rw-rw-r--   0 aparsons  (1000) aparsons  (1000)      985 2021-02-14 16:30:36.000000 linsolve-1.1.0/linsolve/tests/benchmark_A_small_unique_sparse.py
--rw-rw-r--   0 aparsons  (1000) aparsons  (1000)     2903 2021-02-14 16:50:33.000000 linsolve-1.1.0/linsolve/version.py
-drwxrwxr-x   0 aparsons  (1000) aparsons  (1000)        0 2022-06-06 15:11:03.137432 linsolve-1.1.0/linsolve.egg-info/
--rw-r--r--   0 aparsons  (1000) aparsons  (1000)      541 2022-06-06 15:11:02.000000 linsolve-1.1.0/linsolve.egg-info/PKG-INFO
--rw-r--r--   0 aparsons  (1000) aparsons  (1000)      657 2022-06-06 15:11:03.000000 linsolve-1.1.0/linsolve.egg-info/SOURCES.txt
--rw-r--r--   0 aparsons  (1000) aparsons  (1000)        1 2022-06-06 15:11:02.000000 linsolve-1.1.0/linsolve.egg-info/dependency_links.txt
--rw-r--r--   0 aparsons  (1000) aparsons  (1000)       18 2022-06-06 15:11:03.000000 linsolve-1.1.0/linsolve.egg-info/requires.txt
--rw-r--r--   0 aparsons  (1000) aparsons  (1000)        9 2022-06-06 15:11:03.000000 linsolve-1.1.0/linsolve.egg-info/top_level.txt
--rw-rw-r--   0 aparsons  (1000) aparsons  (1000)    17443 2022-03-15 21:45:34.000000 linsolve-1.1.0/linsolve_example.ipynb
--rw-rw-r--   0 aparsons  (1000) aparsons  (1000)       38 2022-06-06 15:11:03.137432 linsolve-1.1.0/setup.cfg
--rw-rw-r--   0 aparsons  (1000) aparsons  (1000)     1150 2021-02-14 16:30:36.000000 linsolve-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:48.747940 linsolve-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-14 13:46:38.000000 linsolve-1.1.2/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-14 13:46:38.000000 linsolve-1.1.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-14 13:46:38.000000 linsolve-1.1.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:48.743940 linsolve-1.1.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-14 13:46:38.000000 linsolve-1.1.2/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-14 13:46:38.000000 linsolve-1.1.2/.github/labels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-14 13:46:38.000000 linsolve-1.1.2/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:48.743940 linsolve-1.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-14 13:46:38.000000 linsolve-1.1.2/.github/workflows/auto-merge-deps.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-14 13:46:38.000000 linsolve-1.1.2/.github/workflows/check-build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-14 13:46:38.000000 linsolve-1.1.2/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-14 13:46:38.000000 linsolve-1.1.2/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-14 13:46:38.000000 linsolve-1.1.2/.github/workflows/run_tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-14 13:46:38.000000 linsolve-1.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-14 13:46:38.000000 linsolve-1.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-14 13:46:38.000000 linsolve-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-07-14 13:46:48.747940 linsolve-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-07-14 13:46:38.000000 linsolve-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:48.743940 linsolve-1.1.2/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-14 13:46:38.000000 linsolve-1.1.2/ci/test_environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:48.743940 linsolve-1.1.2/imgs/
+-rw-r--r--   0 runner    (1001) docker     (123)    72241 2023-07-14 13:46:38.000000 linsolve-1.1.2/imgs/linear_model.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16889 2023-07-14 13:46:38.000000 linsolve-1.1.2/imgs/points.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16058 2023-07-14 13:46:38.000000 linsolve-1.1.2/linsolve_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-14 13:46:38.000000 linsolve-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 13:46:48.747940 linsolve-1.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:48.739940 linsolve-1.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:48.743940 linsolve-1.1.2/src/linsolve/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-14 13:46:38.000000 linsolve-1.1.2/src/linsolve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-14 13:46:48.000000 linsolve-1.1.2/src/linsolve/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45766 2023-07-14 13:46:38.000000 linsolve-1.1.2/src/linsolve/linsolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-14 13:46:38.000000 linsolve-1.1.2/src/linsolve/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:48.743940 linsolve-1.1.2/src/linsolve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-07-14 13:46:48.000000 linsolve-1.1.2/src/linsolve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-14 13:46:48.000000 linsolve-1.1.2/src/linsolve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 13:46:48.000000 linsolve-1.1.2/src/linsolve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-14 13:46:48.000000 linsolve-1.1.2/src/linsolve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 13:46:48.000000 linsolve-1.1.2/src/linsolve.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:48.747940 linsolve-1.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-14 13:46:38.000000 linsolve-1.1.2/tests/benchmark_A_large_shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-14 13:46:38.000000 linsolve-1.1.2/tests/benchmark_A_large_shared_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-14 13:46:38.000000 linsolve-1.1.2/tests/benchmark_A_small_shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-14 13:46:38.000000 linsolve-1.1.2/tests/benchmark_A_small_shared_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-14 13:46:38.000000 linsolve-1.1.2/tests/benchmark_A_small_unique.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-14 13:46:38.000000 linsolve-1.1.2/tests/benchmark_A_small_unique_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29149 2023-07-14 13:46:38.000000 linsolve-1.1.2/tests/test_linsolve.py
```

### Comparing `linsolve-1.1.0/LICENSE` & `linsolve-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `linsolve-1.1.0/README.md` & `linsolve-1.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 See [linsolve_example.ipynb](linsolve_example.ipynb) for a tutorial on how to use these functionalities.
 
 ---
 
 Below we give a brief example on the general usage of `LinearSolver`.
 
 Assume we have a linear system of equations, with a data vector `y` containing measurements
-and a model vector `b` containing parameters we would like to solve for. Let's simplify to 
+and a model vector `b` containing parameters we would like to solve for. Let's simplify to
 the problem of fitting a line to three data points, which amounts to solving for a slope and an offset.
 In this case, our linear system of equations can be written as
 
 <img align='center' src="imgs/linear_model.png" width=300/>
 
 where `b_1` is the slope and `b_2` is the offset, and the `A` matrix contains the mapping
 from model vector `b` to data vector `y`. In our case, the `a_x1` values are the x-values of the data points, and the `a_x2` values are equal to unity. Let's assume the data vector measurements are `y_1 = 2`, `y_2 = 4` and `y_3 = 7`, and their corresponding dependent variable values are `a_11 = 0`, `a_21 = 2` and `a_31 = 4`.
@@ -78,15 +78,15 @@
 the existing tests pass and any new code is well covered by unit tests.
 
 Bug reports or feature requests are also very welcome, please add them to the
 issue log after verifying that the issue does not already exist.
 Comments on existing issues are also welcome.
 
 # Installation
-Preferred method of installation is `pip install .` 
+Preferred method of installation is `pip install .`
 (or `pip install git+https://github.com/HERA-Team/linsolve`). This will install all
 dependencies. See below for manual management of dependencies.
 
 ## Dependencies
 If you use `conda` and would like to ensure that dependencies are installed with `conda`
 rather than `pip`, you should execute::
 
@@ -97,14 +97,13 @@
 If you are developing `linsolve`, it is recommended to create a fresh environment by::
 
     $ git clone https://github.com/HERA-Team/linsolve.git
     $ cd linsolve
     $ conda create -n linsolve python=3
     $ conda activate linsolve
     $ conda env update -n linsolve -f environment.yml
-    $ pip install -e . 
-    
-This will install extra dependencies required for testing/development as well as the 
+    $ pip install -e .
+
+This will install extra dependencies required for testing/development as well as the
 standard ones.
 
 To run tests, just run `nosetests` in the top-level directory.
-
```

### Comparing `linsolve-1.1.0/imgs/linear_model.png` & `linsolve-1.1.2/imgs/linear_model.png`

 * *Files identical despite different names*

### Comparing `linsolve-1.1.0/imgs/points.png` & `linsolve-1.1.2/imgs/points.png`

 * *Files identical despite different names*

### Comparing `linsolve-1.1.0/linsolve/linsolve.py` & `linsolve-1.1.2/src/linsolve/linsolve.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-'''Module providing high-level tools for linearizing and finding chi^2 minimizing 
-solutions to systems of equations.
+"""High-level tools for linearizing and finding chi^2 minimizing systems of equations.
 
 Solvers: LinearSolver, LogProductSolver, and LinProductSolver.
 
 These generally follow the form:
-> data = {'a1*x+b1*y': np.array([5.,7]), 'a2*x+b2*y': np.array([4.,6])}
-> ls = LinearSolver(data, a1=1., b1=np.array([2.,3]), a2=2., b2=np.array([1.,2]))
-> sol = ls.solve()
+
+    >>> data = {'a1*x+b1*y': np.array([5.,7]), 'a2*x+b2*y': np.array([4.,6])}
+    >>> ls = LinearSolver(data, a1=1., b1=np.array([2.,3]), a2=2., b2=np.array([1.,2]))
+    >>> sol = ls.solve()
 
 where equations are passed in as a dictionary where each key is a string
 describing the equation (which is parsed according to python syntax) and each
 value is the corresponding "measured" value of that equation.  Variable names
 in equations are checked against keyword arguments to the solver to determine
 if they are provided constants or parameters to be solved for.  Parameter anmes
 and solutions are return are returned as key:value pairs in ls.solve().
@@ -21,865 +21,1082 @@
 
 LinearSolver solves linear equations of the form 'a*x + b*y + c*z'.
 LogProductSolver uses logrithms to linearize equations of the form 'x*y*z'.
 LinProductSolver uses symbolic Taylor expansion to linearize equations of the
 form 'x*y + y*z'.
 
 For more detail on usage, see linsolve_example.ipynb
-'''
+"""
 
-import numpy as np
 import ast
-from scipy.sparse import csc_matrix
-import scipy.sparse.linalg
-import scipy.linalg
-import warnings
 from copy import deepcopy
 from functools import reduce
 
+import numpy as np
+import scipy.linalg
+import scipy.sparse.linalg
+from scipy.sparse import csc_matrix
+
 # Monkey patch for backward compatibility:
 # ast.Num deprecated in Python 3.8. Make it an alias for ast.Constant
 # if it gets removed.
-if not hasattr(ast, 'Num'):
+if not hasattr(ast, "Num"):
     ast.Num = ast.Constant
 
+
 def ast_getterms(n):
-    '''Convert an AST parse tree into a list of terms.  E.g. 'a*x1+b*x2' -> [[a,x1],[b,x2]]'''
+    """Convert an AST parse tree into a list of terms.
+
+    E.g. 'a*x1+b*x2' -> [[a,x1],[b,x2]]
+    """
     if type(n) is ast.Name:
         return [[n.id]]
     elif type(n) is ast.Constant or type(n) is ast.Num:
         return [[n.n]]
     elif type(n) is ast.Expression:
         return ast_getterms(n.body)
     elif type(n) is ast.UnaryOp:
-        assert(type(n.op) is ast.USub)
-        return [[-1]+ast_getterms(n.operand)[0]]
+        assert type(n.op) is ast.USub
+        return [[-1] + ast_getterms(n.operand)[0]]
     elif type(n) is ast.BinOp:
         if type(n.op) is ast.Mult:
             return [ast_getterms(n.left)[0] + ast_getterms(n.right)[0]]
         elif type(n.op) is ast.Add:
             return ast_getterms(n.left) + ast_getterms(n.right)
         elif type(n.op) is ast.Sub:
             return ast_getterms(n.left) + [[-1] + ast_getterms(n.right)[0]]
         else:
-            raise ValueError('Unsupported operation: %s' % str(n.op))
+            raise ValueError("Unsupported operation: %s" % str(n.op))
     else:
-        raise ValueError('Unsupported: %s' % str(n))
+        raise ValueError("Unsupported: %s" % str(n))
+
 
 def get_name(s, isconj=False):
-    '''Parse variable names of form 'var_' as 'var' + conjugation.'''
+    """Parse variable names of form ``var_`` as ``var + conjugation``."""
     if not type(s) is str:
-        if isconj: return str(s), False
-        else: return str(s)
-    if isconj: return s.rstrip('_'), s.endswith('_') # tag names ending in '_' for conj
-    else: return s.rstrip('_') # parse 'name_' as 'name' + conj
+        if isconj:
+            return str(s), False
+        else:
+            return str(s)
+    if isconj:
+        return s.rstrip("_"), s.endswith("_")  # tag names ending in '_' for conj
+    else:
+        return s.rstrip("_")  # parse 'name_' as 'name' + conj
 
 
 class Constant:
-    '''Container for constants (which can be arrays) in linear equations.'''
+    """Container for constants (which can be arrays) in linear equations."""
+
     def __init__(self, name, constants):
         self.name = get_name(name)
-        if type(name) is str: 
+        if type(name) is str:
             self.val = constants[self.name]
-        else: 
+        else:
             self.val = name
-        try: 
+        try:
             self.dtype = self.val.dtype
-        except(AttributeError): 
+        except AttributeError:
             self.dtype = type(self.val)
+
     def shape(self):
+        """Return the shape of the constants."""
         try:
             return self.val.shape
-        except(AttributeError):
+        except AttributeError:
             return ()
+
     def get_val(self, name=None):
-        '''Return value of constant. Handles conj if name='varname_' is requested 
-        instead of name='varname'.'''
+        """Return value of constant.
+
+        Handles conj if ``name='varname_'`` is requested instead of ``name='varname'``.
+        """
         if name is not None and type(name) is str:
             name, conj = get_name(name, isconj=True)
-            assert(self.name == name)
-            if conj: 
+            assert self.name == name
+            if conj:
                 return self.val.conjugate()
-            else: 
+            else:
                 return self.val
-        else: 
+        else:
             return self.val
 
 
 class Parameter:
-    
     def __init__(self, name):
-        '''Container for parameters that are to be solved for.'''
+        """Container for parameters that are to be solved for."""
         self.name = get_name(name)
 
     def sparse_form(self, name, eqnum, prm_order, prefactor, re_im_split=True):
-        xs,ys,vals = [], [], []
-        # separated into real and imaginary parts iff one of the variables is conjugated with "_"
-        if re_im_split: 
-            name,conj = get_name(name, True)
-            ordr,ordi = 2*prm_order[self.name], 2*prm_order[self.name]+1 
-            cr,ci = prefactor.real, prefactor.imag
-            i = 2*eqnum
+        xs, ys, vals = [], [], []
+        # separated into real and imaginary parts iff one of the variables
+        # is conjugated with "_"
+        if re_im_split:
+            name, conj = get_name(name, True)
+            ordr, ordi = 2 * prm_order[self.name], 2 * prm_order[self.name] + 1
+            cr, ci = prefactor.real, prefactor.imag
+            i = 2 * eqnum
             # (cr,ci) * (pr,pi) = (cr*pr-ci*pi, ci*pr+cr*pi)
-            xs.append(i); ys.append(ordr); vals.append(cr) # real component
-            xs.append(i+1); ys.append(ordr); vals.append(ci) # imag component
+            xs.append(i)
+            ys.append(ordr)
+            vals.append(cr)  # real component
+            xs.append(i + 1)
+            ys.append(ordr)
+            vals.append(ci)  # imag component
             if not conj:
-                xs.append(i); ys.append(ordi); vals.append(-ci) # imag component
-                xs.append(i+1); ys.append(ordi); vals.append(cr) # imag component
+                xs.append(i)
+                ys.append(ordi)
+                vals.append(-ci)  # imag component
+                xs.append(i + 1)
+                ys.append(ordi)
+                vals.append(cr)  # imag component
             else:
-                xs.append(i); ys.append(ordi); vals.append(ci) # imag component
-                xs.append(i+1); ys.append(ordi); vals.append(-cr) # imag component
+                xs.append(i)
+                ys.append(ordi)
+                vals.append(ci)  # imag component
+                xs.append(i + 1)
+                ys.append(ordi)
+                vals.append(-cr)  # imag component
         else:
-            xs.append(eqnum); ys.append(prm_order[self.name]); vals.append(prefactor)
+            xs.append(eqnum)
+            ys.append(prm_order[self.name])
+            vals.append(prefactor)
         return xs, ys, vals
-    
+
     def get_sol(self, x, prm_order):
-        '''Extract prm value from appropriate row of x solution.'''
-        if x.shape[0] > len(prm_order): # detect that we are splitting up real and imaginary parts
-            ordr,ordi = 2*prm_order[self.name], 2*prm_order[self.name]+1
-            return {self.name: x[ordr] + np.complex64(1.0j)*x[ordi]}
-        else: return {self.name: x[prm_order[self.name]]}
+        """Extract prm value from appropriate row of x solution."""
+        if x.shape[0] > len(
+            prm_order
+        ):  # detect that we are splitting up real and imaginary parts
+            ordr, ordi = 2 * prm_order[self.name], 2 * prm_order[self.name] + 1
+            return {self.name: x[ordr] + np.complex64(1.0j) * x[ordi]}
+        else:
+            return {self.name: x[prm_order[self.name]]}
 
 
 class LinearEquation:
-    '''Container for all prms and constants associated with a linear equation.'''
+    """Container for all prms and constants associated with a linear equation."""
+
     def __init__(self, val, **kwargs):
         self.val = val
         if type(val) is str:
-            n = ast.parse(val, mode='eval')
+            n = ast.parse(val, mode="eval")
             val = ast_getterms(n)
-        self.wgts = kwargs.pop('wgts',np.float32(1.))
+        self.wgts = kwargs.pop("wgts", np.float32(1.0))
         self.has_conj = False
-        constants = kwargs.pop('constants', kwargs)
+        constants = kwargs.pop("constants", kwargs)
         self.process_terms(val, constants)
 
     def process_terms(self, terms, constants):
-        '''Classify terms from parsed str as Constant or Parameter.'''
+        """Classify terms from parsed str as Constant or Parameter."""
         self.consts, self.prms = {}, {}
         for term in terms:
             for t in term:
                 try:
                     self.add_const(t, constants)
-                except(KeyError): # must be a parameter then
+                except KeyError:  # must be a parameter then
                     p = Parameter(t)
-                    self.has_conj |= get_name(t,isconj=True)[-1] # keep track if any prms are conj
+                    self.has_conj |= get_name(t, isconj=True)[
+                        -1
+                    ]  # keep track if any prms are conj
                     self.prms[p.name] = p
         self.terms = self.order_terms(terms)
 
     def add_const(self, name, constants):
-        '''Manually add a constant of given name to internal list of constants. Value is drawn from constants.'''
+        """Manually add a constant of given name to internal list of constants.
+
+        Value is drawn from constants.
+        """
         n = get_name(name)
-        if n in constants and isinstance(constants[n], Constant): c = constants[n]
-        else: c = Constant(name, constants) # raises KeyError if not a constant
+        if n in constants and isinstance(constants[n], Constant):
+            c = constants[n]
+        else:
+            c = Constant(name, constants)  # raises KeyError if not a constant
         self.consts[c.name] = c
-    
+
     def order_terms(self, terms):
-        '''Reorder terms to obey (const1,const2,...,prm) ordering.'''
-        for L in terms: L.sort(key=lambda x: get_name(x) in self.prms)
+        """Reorder terms to obey (const1,const2,...,prm) ordering."""
+        for L in terms:
+            L.sort(key=lambda x: get_name(x) in self.prms)
         # Validate that each term has exactly 1 unsolved parameter.
         for t in terms:
-            assert(get_name(t[-1]) in self.prms)
+            assert get_name(t[-1]) in self.prms
             for ti in t[:-1]:
-                assert(type(ti) is not str or get_name(ti) in self.consts)
+                assert type(ti) is not str or get_name(ti) in self.consts
         return terms
 
-    def eval_consts(self, const_list, wgts=np.float32(1.)):
-        '''Multiply out constants (and wgts) for placing in matrix.'''
+    def eval_consts(self, const_list, wgts=np.float32(1.0)):
+        """Multiply out constants (and wgts) for placing in matrix."""
         const_list = [self.consts[get_name(c)].get_val(c) for c in const_list]
-        return wgts**.5 * reduce(lambda x,y: x*y, const_list, np.float32(1.))
-        # this has the effect of putting the square root of the weights into each A matrix
-        #return 1. * reduce(lambda x,y: x*y, const_list, 1.)
+        return wgts**0.5 * reduce(lambda x, y: x * y, const_list, np.float32(1.0))
 
     def sparse_form(self, eqnum, prm_order, re_im_split=True):
-        '''Returns the row and col information and the values of coefficients to build up 
-        part of the sparse (CSR) reprentation of the A matrix corresponding to this equation.'''
+        """Return the row/col info and the values of coefficients.
+
+        Intended to build up part of the sparse (CSR) reprentation of the A matrix
+        corresponding to this equation.
+        """
         xs, ys, vals = [], [], []
         for term in self.terms:
             p = self.prms[get_name(term[-1])]
             f = self.eval_consts(term[:-1], self.wgts)
-            x,y,val = p.sparse_form(term[-1], eqnum, prm_order, f.flatten(), re_im_split)
-            xs += x; ys += y; vals += val
+            x, y, val = p.sparse_form(
+                term[-1], eqnum, prm_order, f.flatten(), re_im_split
+            )
+            xs += x
+            ys += y
+            vals += val
         return xs, ys, vals
-    
+
     def eval(self, sol):
-        '''Given dict of parameter solutions, evaluate this equation.'''
+        """Given dict of parameter solutions, evaluate this equation."""
         rv = 0
         for term in self.terms:
             total = self.eval_consts(term[:-1])
-            name,isconj = get_name(term[-1],isconj=True)
-            if isconj: total *= np.conj(sol[name])
-            else: total *= sol[name]
+            name, isconj = get_name(term[-1], isconj=True)
+            if isconj:
+                total *= np.conj(sol[name])
+            else:
+                total *= sol[name]
             rv += total
         return rv
-        
+
 
 def verify_weights(wgts, keys):
-    '''Given wgts and keys, ensure wgts have all keys and are all real.
-    If wgts == {} or None, return all 1s.'''
+    """Given wgts and keys, ensure wgts have all keys and are all real.
+
+    If wgts == {} or None, return all 1s.
+    """
     if wgts is None or wgts == {}:
-        return {k: np.float32(1.) for k in keys}
-    else:
-        for k in keys:
-            assert(k in wgts) # must have weights for all keys
-            assert(np.iscomplexobj(wgts[k]) == False) # tricky errors happen if wgts are complex
-        return wgts
+        return {k: np.float32(1.0) for k in keys}
+    for k in keys:
+        assert k in wgts  # must have weights for all keys
+        # tricky errors happen if wgts are complex
+        assert not np.iscomplexobj(wgts[k])
+    return wgts
+
 
 def infer_dtype(values):
-    '''Given a list of values, return the appropriate numpy data 
-    type for matrices, solutions.  
+    """Get the appropriate numpy data type for matrices, solutions.
+
     Returns float32, float64, complex64, or complex128.
     Python scalars will be treated float 32 or complex64 as appropriate.
-    Likewise, all int types will be treated as single precision floats.'''
-    
+    Likewise, all int types will be treated as single precision floats.
+    """
     # ensure we are at least a float32 if we were passed integers
-    types = [np.dtype('float32')]
+    types = [np.dtype("float32")]
     # determine the data type of all values
-    all_types = list(set([v.dtype if hasattr(v,'dtype') else type(v)
-                        for v in values]))
+    all_types = list({v.dtype if hasattr(v, "dtype") else type(v) for v in values})
     # split types into numpy vs. python dtypes
     py_types = [t for t in all_types if not isinstance(t, np.dtype)]
     np_types = [t for t in all_types if isinstance(t, np.dtype)]
     # only use numpy dtypes that are floating/complex
-    types += [t for t in np_types if np.issubdtype(t, np.floating) 
-                                  or np.issubdtype(t, np.complexfloating)]
+    types += [
+        t
+        for t in np_types
+        if np.issubdtype(t, np.floating) or np.issubdtype(t, np.complexfloating)
+    ]
     # if any python constants are complex, promote to complex, but otherwise
     # don't promote to double if we have floats/doubles/ints in python
     if complex in py_types:
-        types.append(np.dtype('complex64'))
+        types.append(np.dtype("complex64"))
     # Use promote_types to determine the final floating/complex dtype
     dtype = reduce(np.promote_types, types)
     return dtype
 
-class LinearSolver:
 
+class LinearSolver:
     def __init__(self, data, wgts={}, sparse=False, **kwargs):
         """Set up a linear system of equations of the form 1*a + 2*b + 3*c = 4.
 
-        Args:
-            data: Dictionary that maps linear equations, written as valid python-interpetable strings 
-                that include the variables in question, to (complex) numbers or numpy arrarys. 
-                Variables with trailing underscores '_' are interpreted as complex conjugates.
-            wgts: Dictionary that maps equation strings from data to real weights to apply to each 
-                equation. Weights are treated as 1/sigma^2. All equations in the data must have a weight 
-                if wgts is not the default, {}, which means all 1.0s.
-            sparse: Boolean (default False). If True, represents A matrix sparsely (though AtA, Aty end up dense)
-                May be faster for certain systems of equations. 
-            **kwargs: keyword arguments of constants (python variables in keys of data that 
-                are not to be solved for)
-
-        Returns:
-            None
+        Parameters
+        ----------
+        data : dict
+            maps linear equations, written as valid python-interpetable strings
+            that include the variables in question, to (complex) numbers or numpy
+            arrays. Variables with trailing underscores '_' are interpreted as complex
+            conjugates.
+        wgts : dict
+            maps equation strings from data to real weights to apply to each
+            equation. Weights are treated as 1/sigma^2. All equations in the data must
+            have a weight if wgts is not the default, {}, which means all 1.0s.
+        sparse : bool
+            If True, represents A matrix sparsely (though AtA, Aty end up dense)
+            May be faster for certain systems of equations.
+        **kwargs: keyword arguments of constants (python variables in keys of data that
+            are not to be solved for)
         """
         # XXX add ability to override datatype inference
         # see https://github.com/HERA-Team/linsolve/issues/30
         self.data = data
         self.keys = list(data.keys())
         self.sparse = sparse
         self.wgts = verify_weights(wgts, self.keys)
-        constants = kwargs.pop('constants', kwargs)
-        self.eqs = [LinearEquation(k,wgts=self.wgts[k], constants=constants) for k in self.keys]
+        constants = kwargs.pop("constants", kwargs)
+        self.eqs = [
+            LinearEquation(k, wgts=self.wgts[k], constants=constants) for k in self.keys
+        ]
         # XXX add ability to have more than one measurment for a key=equation
         # see https://github.com/HERA-Team/linsolve/issues/14
         self.prms = {}
-        for eq in self.eqs: 
+        for eq in self.eqs:
             self.prms.update(eq.prms)
         self.consts = {}
-        for eq in self.eqs: 
-            self.consts.update(eq.consts) 
+        for eq in self.eqs:
+            self.consts.update(eq.consts)
         self.prm_order = {}
-        for i,p in enumerate(self.prms): 
+        for i, p in enumerate(self.prms):
             self.prm_order[p] = i
 
         # infer dtype for later arrays
-        self.re_im_split = kwargs.pop('re_im_split',False)
-        #go through and figure out if any variables are conjugated
-        for eq in self.eqs: 
+        self.re_im_split = kwargs.pop("re_im_split", False)
+        # go through and figure out if any variables are conjugated
+        for eq in self.eqs:
             self.re_im_split |= eq.has_conj
-        self.dtype = infer_dtype(list(self.data.values()) + list(self.consts.values()) + list(self.wgts.values()))
-        if self.re_im_split: self.dtype = np.real(np.ones(1, dtype=self.dtype)).dtype
+        self.dtype = infer_dtype(
+            list(self.data.values())
+            + list(self.consts.values())
+            + list(self.wgts.values())
+        )
+        if self.re_im_split:
+            self.dtype = np.real(np.ones(1, dtype=self.dtype)).dtype
         self.shape = self._shape()
 
     def _shape(self):
-        '''Get broadcast shape of constants, weights for last dim of A'''
+        """Get broadcast shape of constants, weights for last dim of A."""
         sh = []
         for k in self.consts:
             shk = self.consts[k].shape()
-            if len(shk) > len(sh): sh += [0] * (len(shk)-len(sh))
-            for i in range(min(len(sh),len(shk))): sh[i] = max(sh[i],shk[i])
+            if len(shk) > len(sh):
+                sh += [0] * (len(shk) - len(sh))
+            for i in range(min(len(sh), len(shk))):
+                sh[i] = max(sh[i], shk[i])
         for k in self.wgts:
-            try: shk = self.wgts[k].shape
-            except(AttributeError): continue
-            if len(shk) > len(sh): sh += [0] * (len(shk)-len(sh))
-            for i in range(min(len(sh),len(shk))): sh[i] = max(sh[i],shk[i])
+            try:
+                shk = self.wgts[k].shape
+            except AttributeError:
+                continue
+            if len(shk) > len(sh):
+                sh += [0] * (len(shk) - len(sh))
+            for i in range(min(len(sh), len(shk))):
+                sh[i] = max(sh[i], shk[i])
         return tuple(sh)
 
     def _A_shape(self):
-        '''Get shape of A matrix (# eqs, # prms, data.size). Now always 3D.'''
-        try: 
-            sh = (reduce(lambda x,y: x*y, self.shape),) # flatten data dimensions so A is always 3D
-        except(TypeError): 
+        """Get shape of A matrix (# eqs, # prms, data.size). Now always 3D."""
+        try:
+            sh = (
+                reduce(lambda x, y: x * y, self.shape),
+            )  # flatten data dimensions so A is always 3D
+        except TypeError:
             sh = (1,)
-        if self.re_im_split: 
-            return (2*len(self.eqs),2*len(self.prm_order))+sh
-        else: return (len(self.eqs),len(self.prm_order))+sh
+        if self.re_im_split:
+            return (2 * len(self.eqs), 2 * len(self.prm_order)) + sh
+        else:
+            return (len(self.eqs), len(self.prm_order)) + sh
 
     def get_A(self):
-        '''Return A matrix for A*x=y.'''
+        """Return A matrix for A*x=y."""
         A = np.zeros(self._A_shape(), dtype=self.dtype)
-        xs,ys,vals = self.sparse_form()
-        ones = np.ones_like(A[0,0])
-        #A[xs,ys] += [v * ones for v in vals] # This is broken when a single equation has the same param more than once
-        for x,y,v in zip(xs,ys,[v * ones for v in vals]):
-            A[x,y] += v # XXX ugly
+        xs, ys, vals = self.sparse_form()
+        ones = np.ones_like(A[0, 0])
+
+        # This is broken when a single equation has the same param more than once:
+        # --> A[xs,ys] += [v * ones for v in vals]
+
+        for x, y, v in zip(xs, ys, [v * ones for v in vals]):
+            A[x, y] += v  # XXX ugly
         return A
 
     def sparse_form(self):
-        '''Returns a lists of lists of row and col numbers and coefficients in order to
-        express the linear system as a CSR sparse matrix.'''
+        """Get a list of lists of row/col numbers and coefficients.
+
+        Intended to express the linear system as a CSR sparse matrix.
+        """
         xs, ys, vals = [], [], []
-        for i,eq in enumerate(self.eqs):
-            x,y,val = eq.sparse_form(i, self.prm_order, self.re_im_split)
-            xs += x; ys += y; vals += val
+        for i, eq in enumerate(self.eqs):
+            x, y, val = eq.sparse_form(i, self.prm_order, self.re_im_split)
+            xs += x
+            ys += y
+            vals += val
         return xs, ys, vals
 
     def get_A_sparse(self):
-        '''Fixes dimension needed for CSR sparse matrix representation.'''
-        xs,ys,vals = self.sparse_form()
-        ones = np.ones(self._A_shape()[2:],dtype=self.dtype)
-        for n,val in enumerate(vals): 
+        """Fixes dimension needed for CSR sparse matrix representation."""
+        xs, ys, vals = self.sparse_form()
+        ones = np.ones(self._A_shape()[2:], dtype=self.dtype)
+        for n, val in enumerate(vals):
             if not isinstance(val, np.ndarray) or val.size == 1:
-                vals[n] = ones*val
+                vals[n] = ones * val
         return np.array(xs), np.array(ys), np.array(vals, dtype=self.dtype).T
-    
+
     def get_weighted_data(self):
-        '''Return y = data * wgt**.5 as a 2D vector, regardless of original data/wgt shape.'''
-        dtype = self.dtype # default
+        """Return y = data * wgt**.5 as a 2D vector, regardless of original shape."""
+        dtype = self.dtype  # default
         if self.re_im_split:
             if dtype == np.float32:
                 dtype = np.complex64
             else:
                 dtype = np.complex128
         d = np.array([self.data[k] for k in self.keys], dtype=dtype)
         if len(self.wgts) > 0:
             w = np.array([self.wgts[k] for k in self.keys])
-            w.shape += (1,) * (d.ndim-w.ndim)
-            d.shape += (1,) * (w.ndim-d.ndim)
-            d = d*(w**.5) 
-            # this is w**.5 because A already has a factor of w**.5 in it, so 
-            # (At N^-1 A)^1 At N^1 y ==> (At A)^1 At d (where d is the result of this 
+            w.shape += (1,) * (d.ndim - w.ndim)
+            d.shape += (1,) * (w.ndim - d.ndim)
+            d = d * (w**0.5)
+            # this is w**.5 because A already has a factor of w**.5 in it, so
+            # (At N^-1 A)^1 At N^1 y ==> (At A)^1 At d (where d is the result of this
             # function and A is redefined to include half of the weights)
-        self._data_shape = d.shape[1:] # store for reshaping sols to original
-        d.shape = (d.shape[0],-1) # Flatten 
+        self._data_shape = d.shape[1:]  # store for reshaping sols to original
+
+        # It's possible to have a zero-size d (if there are no keys)
+        d.shape = (d.shape[0], -1) if d.size > 0 else (0, 0)
+
         if self.re_im_split:
-            rv = np.empty((2*d.shape[0],)+d.shape[1:], dtype=self.dtype)
-            rv[::2],rv[1::2] = d.real, d.imag
+            rv = np.empty((2 * d.shape[0],) + d.shape[1:], dtype=self.dtype)
+            rv[::2], rv[1::2] = d.real, d.imag
             return rv
-        else: return d
-    
+        else:
+            return d
+
     def _invert_lsqr(self, A, y, rcond):
-        '''Use np.linalg.lstsq to solve a system of equations.  Usually the best 
-        performer, but for a fully-constrained system, 'solve' can be faster.  Also,
-        there are a couple corner cases where lstsq is unstable but pinv works 
-        for the same rcond. It seems particularly the case for single precision matrices.'''
+        """Solve a system of equations.
+
+        Uses :func`np.linalg.lstsq`. Usually the best performer, but for a
+        fully-constrained system, 'solve' can be faster.  Also, there are a couple
+        corner cases where lstsq is unstable but pinv works for the same rcond. It
+        seems particularly the case for single precision matrices.
+        """
         # add ability for lstsq to work on stacks of matrices
         # see https://github.com/HERA-Team/linsolve/issues/31
 
-        #x = [np.linalg.lstsq(A[...,k], y[...,k], rcond=rcond)[0] for k in range(y.shape[-1])]
         # np.linalg.lstsq uses lapack gelsd and is slower:
-        # see https://stackoverflow.com/questions/55367024/fastest-way-of-solving-linear-least-squares
-        x = [scipy.linalg.lstsq(A[...,k], y[...,k],
-                                cond=rcond, lapack_driver='gelsy')[0]
-                      for k in range(y.shape[-1])]
+        # see https://stackoverflow.com/questions/55367024/
+        #        fastest-way-of-solving-linear-least-squares
+        x = [
+            scipy.linalg.lstsq(A[..., k], y[..., k], cond=rcond, lapack_driver="gelsy")[
+                0
+            ]
+            for k in range(y.shape[-1])
+        ]
         return np.array(x).T
 
     def _invert_lsqr_sparse(self, xs_ys_vals, y, rcond):
-        '''Use the scipy.sparse lsqr solver.'''
-        # x = [scipy.sparse.linalg.lsqr(A[k], y[...,k], atol=rcond, btol=rcond)[0] for k in range(y.shape[-1])] # this is crazy slow for unknown reasons
+        """Use the scipy.sparse lsqr solver."""
+        # Note that using scipy.sparse.linalg.lsqr is crazy slow for unknown reasons.
         AtA, Aty = self._get_AtA_Aty_sparse(xs_ys_vals, y)
-        x = [scipy.linalg.lstsq(AtA[k], Aty[k],
-                                cond=rcond, lapack_driver='gelsy')[0]
-                      for k in range(y.shape[-1])]
+        x = [
+            scipy.linalg.lstsq(AtA[k], Aty[k], cond=rcond, lapack_driver="gelsy")[0]
+            for k in range(y.shape[-1])
+        ]
         return np.array(x).T
 
     def _invert_pinv_shared(self, A, y, rcond):
-        '''Helper function for forming (At A)^-1 At.  Uses pinv to invert.'''
+        """Helper function for forming (At A)^-1 At.  Uses pinv to invert."""
         At = A.T.conj()
         AtA = np.dot(At, A)
         AtAi = np.linalg.pinv(AtA, rcond=rcond, hermitian=True)
-        # x = np.einsum('ij,jk,kn->in', AtAi, At, y, optimize=True) # slow for small matrices
-        x = np.dot(AtAi, np.dot(At, y))
-        return x
+        # Following is slow for small matrices:
+        # --> x = np.einsum('ij,jk,kn->in', AtAi, At, y, optimize=True)
+        return np.dot(AtAi, np.dot(At, y))
 
     def _invert_pinv_shared_sparse(self, xs_ys_vals, y, rcond):
-        '''Use pinv to invert AtA matrix.  Tends to be ~10x slower than lsqr for sparse matrices'''
+        """Use pinv to invert AtA matrix.
+
+        Tends to be ~10x slower than lsqr for sparse matrices.
+        """
         xs, ys, vals = xs_ys_vals
         A = csc_matrix((vals[0], (xs, ys)))
         At = A.T.conj()
-        AtA = At.dot(A).toarray() # make dense after sparse dot product
+        AtA = At.dot(A).toarray()  # make dense after sparse dot product
         AtAi = np.linalg.pinv(AtA, rcond=rcond, hermitian=True)
-        x = np.dot(AtAi, At.dot(y))
-        return x
+        return np.dot(AtAi, At.dot(y))
 
     def _invert_pinv(self, A, y, rcond):
-        '''Use np.linalg.pinv to invert AtA matrix.  Tends to be about ~3x slower than solve.'''
+        """Use np.linalg.pinv to invert AtA matrix.
+
+        Tends to be about ~3x slower than solve.
+        """
         # As of numpy 1.14, pinv works on stacks of matrices
-        At = A.transpose([2,1,0]).conj()
-        AtA = [np.dot(At[k], A[...,k]) for k in range(y.shape[-1])]
-        # AtA = np.einsum('jin,jkn->nik', A.conj(), A, optimize=True) # slower
+        At = A.transpose([2, 1, 0]).conj()
+        AtA = [np.dot(At[k], A[..., k]) for k in range(y.shape[-1])]
+
+        # This is slower:
+        # --> AtA = np.einsum('jin,jkn->nik', A.conj(), A, optimize=True)
+
         AtAi = np.linalg.pinv(AtA, rcond=rcond, hermitian=True)
-        x = np.einsum('nij,njk,kn->in', AtAi, At, y, optimize=True)
-        return x
+        return np.einsum("nij,njk,kn->in", AtAi, At, y, optimize=True)
 
     def _get_AtA_Aty_sparse(self, xs_ys_vals, y):
         xs, ys, vals = xs_ys_vals
         # rolling our own sparse representation b/c scipy.sparse
         # can't share sparsity over a 3rd axis and remaking
         # sparse matrices for each value is too slow
         A = {}
         # can below be coded as a comprehension? need to be sure
         # to sum over repeat xs...
-        for _y,_x,_v in zip(ys, xs, vals.T):
+        for _y, _x, _v in zip(ys, xs, vals.T):
             try:
                 A[_y][_x] = A[_y].get(_x, 0) + _v
-            except(KeyError):
+            except KeyError:
                 A[_y] = {_x: _v}
         nprms = self._A_shape()[1]
         AtA = np.empty((y.shape[-1], nprms, nprms), dtype=self.dtype)
         Aty = np.empty((y.shape[-1], nprms), dtype=self.dtype)
         # Compute AtA and Aty using sparse format used above.
         # Speedup over scipy.sparse b/c y[x] and A[i][x] are arrays
         for i in range(AtA.shape[1]):
             # 'i' is the column index, 'x' is the row index of A
-            Aty[:,i] = sum([A[i][x].conj() * y[x] for x in A[i]])
+            Aty[:, i] = sum(A[i][x].conj() * y[x] for x in A[i])
             for j in range(i, AtA.shape[1]):
-                AtA[:,i,j] = sum([A[i][x].conj() * A[j][x]
-                                  for x in A[i] if x in A[j]])
-                AtA[:,j,i] = AtA[:,i,j].conj() # explicitly hermitian
+                AtA[:, i, j] = sum(A[i][x].conj() * A[j][x] for x in A[i] if x in A[j])
+                AtA[:, j, i] = AtA[:, i, j].conj()  # explicitly hermitian
         return AtA, Aty
 
     def _invert_pinv_sparse(self, xs_ys_vals, y, rcond):
-        '''Use pinv to invert AtA matrix.  Tends to be ~10x slower than lsqr for sparse matrices'''
+        """Use pinv to invert AtA matrix.
+
+        Tends to be ~10x slower than lsqr for sparse matrices.
+        """
         AtA, Aty = self._get_AtA_Aty_sparse(xs_ys_vals, y)
         AtAi = np.linalg.pinv(AtA, rcond=rcond, hermitian=True)
         x = [np.dot(AtAi[k], Aty[k]) for k in range(y.shape[-1])]
         return np.array(x).T
 
     def _invert_solve(self, A, y, rcond):
-        '''Use np.linalg.solve to solve a system of equations.  Requires a fully constrained
-        system of equations (i.e. doesn't deal with singular matrices).  Can by ~1.5x faster that lstsq
-        for this case. 'rcond' is unused, but passed as an argument to match the interface of other
-        _invert methods.'''
+        """Use np.linalg.solve to solve a system of equations.
+
+        Requires a fully constrained system of equations (i.e. doesn't deal with
+        singular matrices).  Can by ~1.5x faster that lstsq for this case. 'rcond'
+        is unused, but passed as an argument to match the interface of other _invert
+        methods.
+        """
         # As of numpy 1.8, solve works on stacks of matrices
-        At = A.transpose([2,1,0]).conj()
-        AtA = [np.dot(At[k], A[...,k]) for k in range(y.shape[-1])]
-        Aty = [np.dot(At[k], y[...,k]) for k in range(y.shape[-1])]
-        return np.linalg.solve(AtA, Aty).T # sometimes errors if singular
-        #return scipy.linalg.solve(AtA, Aty, 'her') # slower by about 50%
+        At = A.transpose([2, 1, 0]).conj()
+        AtA = [np.dot(At[k], A[..., k]) for k in range(y.shape[-1])]
+        Aty = [np.dot(At[k], y[..., k]) for k in range(y.shape[-1])]
+
+        # This is slower by about 50%: scipy.linalg.solve(AtA, Aty, 'her')
+
+        # But this sometimes errors if singular:
+        return np.linalg.solve(AtA, Aty).T
 
     def _invert_solve_sparse(self, xs_ys_vals, y, rcond):
-        '''Use linalg.solve to solve a fully constrained (non-degenerate) system of equations.
-        Tends to be ~3x slower than lsqr for sparse matrices.  'rcond' is unused, but passed
-        as an argument to match the interface of other _invert methods.'''
+        """Use linalg.solve to solve a fully constrained (non-degenerate) system of eqs.
+
+        Tends to be ~3x slower than lsqr for sparse matrices. 'rcond' is unused,
+        but passed as an argument to match the interface of other _invert methods.
+        """
         AtA, Aty = self._get_AtA_Aty_sparse(xs_ys_vals, y)
-        #x = scipy.sparse.linalg.spsolve(AtA, Aty) # AtA and Aty don't end up being that sparse, usually
+        # AtA and Aty don't end up being that sparse, usually, so don't use this:
+        # --> x = scipy.sparse.linalg.spsolve(AtA, Aty)
         return np.linalg.solve(AtA, Aty).T
 
     def _invert_default(self, A, y, rcond):
-        '''The default inverter, currently 'pinv'.'''
+        """The default inverter, currently 'pinv'."""
         # XXX doesn't deal w/ fact that individual matrices might
         # fail for one inversion method.
         # see https://github.com/HERA-Team/linsolve/issues/32
 
         # XXX for now, lsqr is slower than pinv, but that may
         # change once numpy supports stacks of matrices
         # see https://github.com/HERA-Team/linsolve/issues/31
         return self._invert_pinv(A, y, rcond)
 
     def _invert_default_sparse(self, xs_ys_vals, y, rcond):
-        '''The default sparse inverter, currently 'pinv'.'''
+        """The default sparse inverter, currently 'pinv'."""
         return self._invert_pinv_sparse(xs_ys_vals, y, rcond)
 
-    def solve(self, rcond=None, mode='default'):
+    def solve(self, rcond=None, mode="default"):
         """Compute x' = (At A)^-1 At * y, returning x' as dict of prms:values.
 
-        Args:
-            rcond: cutoff ratio for singular values useed in numpy.linalg.lstsq, numpy.linalg.pinv,
-                or (if sparse) as atol and btol in scipy.sparse.linalg.lsqr
-                Default: None (resolves to machine precision for inferred dtype)
-            mode: 'default', 'lsqr', 'pinv', or 'solve', selects which inverter to use, unless all equations share the same A matrix, in which case pinv is always used`. 
-                'default': alias for 'pinv'.
-                'lsqr': uses numpy.linalg.lstsq to do an inversion-less solve.  Usually 
-                    the fastest solver.
-                'solve': uses numpy.linalg.solve to do an inversion-less solve.  Fastest, 
-                    but only works for fully constrained systems of equations.
-                'pinv': uses numpy.linalg.pinv to perform a pseudo-inverse and then solves.  Can
-                    sometimes be more numerically stable (but slower) than 'lsqr'.
-                All of these modes are superceded if the same system of equations applies
-                to all datapoints in an array.  In this case, a inverse-based method is used so
-                that the inverted matrix can be re-used to solve all array indices.
-
-        Returns:
-            sol: a dictionary of solutions with variables as keys
+        Parameters
+        ----------
+        rcond
+            cutoff ratio for singular values useed in :func:`numpy.linalg.lstsq`,
+            :func:`numpy.linalg.pinv`, or (if sparse) as atol and btol in
+            :func:`scipy.sparse.linalg.lsqr`
+        mode : {'default', 'lsqr', 'pinv', or 'solve'},
+            selects which inverter to use, unless all equations share the same A matrix,
+            in which case pinv is always used:
+
+            * 'default': alias for 'pinv'.
+            * 'lsqr': uses numpy.linalg.lstsq to do an inversion-less solve.  Usually
+              the fastest solver.
+            * 'solve': uses numpy.linalg.solve to do an inversion-less solve.  Fastest,
+              but only works for fully constrained systems of equations.
+            * 'pinv': uses numpy.linalg.pinv to perform a pseudo-inverse and then
+              solves. Can sometimes be more numerically stable (but slower) than 'lsqr'.
+
+            All of these modes are superceded if the same system of equations applies
+            to all datapoints in an array.  In this case, a inverse-based method is
+            used so that the inverted matrix can be re-used to solve all array indices.
+
+        Returns
+        -------
+        sol
+            a dictionary of solutions with variables as keys
         """
-        assert(mode in ['default','lsqr','pinv','solve'])
+        assert mode in ["default", "lsqr", "pinv", "solve"]
         if rcond is None:
             rcond = np.finfo(self.dtype).resolution
         y = self.get_weighted_data()
         if self.sparse:
             xs, ys, vals = self.get_A_sparse()
-            if vals.shape[0] == 1 and y.shape[-1] > 1: # reuse inverse
-                x = self._invert_pinv_shared_sparse((xs,ys,vals), y, rcond)
-            else: # we can't reuse inverses
-                if mode == 'default': _invert = self._invert_default_sparse
-                elif mode == 'lsqr': _invert = self._invert_lsqr_sparse
-                elif mode == 'pinv': _invert = self._invert_pinv_sparse
-                elif mode == 'solve': _invert = self._invert_solve_sparse
-                x = _invert((xs,ys,vals), y, rcond)
-        else: 
+            if vals.shape[0] == 1 and y.shape[-1] > 1:  # reuse inverse
+                x = self._invert_pinv_shared_sparse((xs, ys, vals), y, rcond)
+            else:  # we can't reuse inverses
+                if mode == "default":
+                    _invert = self._invert_default_sparse
+                elif mode == "lsqr":
+                    _invert = self._invert_lsqr_sparse
+                elif mode == "pinv":
+                    _invert = self._invert_pinv_sparse
+                elif mode == "solve":
+                    _invert = self._invert_solve_sparse
+                x = _invert((xs, ys, vals), y, rcond)
+        else:
             A = self.get_A()
             Ashape = self._A_shape()
-            assert(A.ndim == 3)
-            if Ashape[-1] == 1 and y.shape[-1] > 1: # can reuse inverse
-                x = self._invert_pinv_shared(A[...,0], y, rcond)
-            else: # we can't reuse inverses
-                if mode == 'default': _invert = self._invert_default
-                elif mode == 'lsqr': _invert = self._invert_lsqr
-                elif mode == 'pinv': _invert = self._invert_pinv
-                elif mode == 'solve': _invert = self._invert_solve
+            assert A.ndim == 3
+            if Ashape[-1] == 1 and y.shape[-1] > 1:  # can reuse inverse
+                x = self._invert_pinv_shared(A[..., 0], y, rcond)
+            else:  # we can't reuse inverses
+                if mode == "default":
+                    _invert = self._invert_default
+                elif mode == "lsqr":
+                    _invert = self._invert_lsqr
+                elif mode == "pinv":
+                    _invert = self._invert_pinv
+                elif mode == "solve":
+                    _invert = self._invert_solve
                 x = _invert(A, y, rcond)
 
-        x.shape = x.shape[:1] + self._data_shape # restore to shape of original data
+        x.shape = x.shape[:1] + self._data_shape  # restore to shape of original data
         sol = {}
-        for p in list(self.prms.values()): sol.update(p.get_sol(x,self.prm_order))
+        for p in list(self.prms.values()):
+            sol.update(p.get_sol(x, self.prm_order))
         return sol
 
     def eval(self, sol, keys=None):
-        """Returns a dictionary evaluating data keys to the current values given sol and consts.
-        Uses the stored data object unless otherwise specified."""
-        if keys is None: keys = self.keys
-        elif type(keys) is str: keys = [keys]
-        elif type(keys) is dict: keys = list(keys.keys())
+        """Get a dict mapping data keys to the current values given sol and consts.
+
+        Uses the stored data object unless otherwise specified.
+        """
+        if keys is None:
+            keys = self.keys
+        elif type(keys) is str:
+            keys = [keys]
+        elif type(keys) is dict:
+            keys = list(keys.keys())
         result = {}
         for k in keys:
             eq = LinearEquation(k, **self.consts)
             result[k] = eq.eval(sol)
         return result
-    
+
     def _chisq(self, sol, data, wgts, evaluator):
         """Internal adaptable chisq calculator."""
-        if len(wgts) == 0: sigma2 = {k: 1.0 for k in list(data.keys())} #equal weights
-        else: sigma2 = {k: wgts[k]**-1 for k in list(wgts.keys())} 
+        if len(wgts) == 0:
+            sigma2 = {k: 1.0 for k in list(data.keys())}  # equal weights
+        else:
+            sigma2 = {k: wgts[k] ** -1 for k in list(wgts.keys())}
         evaluated = evaluator(sol, keys=data)
         chisq = 0
-        for k in list(data.keys()): chisq += np.abs(evaluated[k]-data[k])**2 / sigma2[k]
+        for k in list(data.keys()):
+            chisq += np.abs(evaluated[k] - data[k]) ** 2 / sigma2[k]
         return chisq
-    
+
     def chisq(self, sol, data=None, wgts=None):
-        """Compute Chi^2 = |obs - mod|^2 / sigma^2 for the specified solution. Weights are treated as 1/sigma^2. 
-        wgts = {} means sigma = 1. Default uses the stored data and weights unless otherwise overwritten."""
-        if data is None: 
+        """Compute ``Chi^2 = |obs - mod|^2 / sigma^2`` for the specified solution.
+
+        Weights are treated as 1/sigma^2. wgts = {} means sigma = 1. Default uses the
+        stored data and weights unless otherwise overwritten.
+        """
+        if data is None:
             data = self.data
-        if wgts is None: 
+        if wgts is None:
             wgts = self.wgts
         wgts = verify_weights(wgts, list(data.keys()))
         return self._chisq(sol, data, wgts, self.eval)
-        
 
-# XXX need to add support for conjugated constants...maybe this already works because we have conjugated constants inherited from taylor expansion
+
+# XXX need to add support for conjugated constants...maybe this already works because
+# we have conjugated constants inherited from taylor expansion
 # see https://github.com/HERA-Team/linsolve/issues/12
-def conjterm(term, mode='amp'):
-    '''Modify prefactor for conjugated terms, according to mode='amp|phs|real|imag'.'''
-    f = {'amp':1,'phs':-1,'real':1,'imag':1j}[mode] # if KeyError, mode was invalid
-    terms = [[f,t[:-1]] if t.endswith('_') else [t] for t in term]
-    return reduce(lambda x,y: x+y, terms)
-
-def jointerms(terms): 
-    '''String that joins lists of lists of terms as the sum of products.'''
-    return '+'.join(['*'.join(map(str,t)) for t in terms])
+def conjterm(term, mode="amp"):
+    """Modify prefactor for conjugated terms, for ``mode='amp|phs|real|imag'``."""
+    f = {"amp": 1, "phs": -1, "real": 1, "imag": 1j}[
+        mode
+    ]  # if KeyError, mode was invalid
+    terms = [[f, t[:-1]] if t.endswith("_") else [t] for t in term]
+    return reduce(lambda x, y: x + y, terms)
 
 
-class LogProductSolver: 
+def jointerms(terms):
+    """String that joins lists of lists of terms as the sum of products."""
+    return "+".join(["*".join(map(str, t)) for t in terms])
 
-    def __init__(self, data, wgts={}, sparse=False, **kwargs):
-        """Set up a nonlinear system of equations of the form a*b = 1.0 to linearze via logarithm.
 
-        Args:
-            data: Dictionary that maps nonlinear product equations, written as valid python-interpetable 
-                strings that include the variables in question, to (complex) numbers or numpy arrarys. 
-                Variables with trailing underscores '_' are interpreted as complex conjugates (e.g. x*y_ 
-                parses as x * y.conj()).
-            wgts: Dictionary that maps equation strings from data to real weights to apply to each 
-                equation. Weights are treated as 1/sigma^2. All equations in the data must have a weight 
-                if wgts is not the default, {}, which means all 1.0s.
-            sparse: Boolean (default False). If True, represents A matrix sparsely (though AtA, Aty end up dense)
-                May be faster for certain systems of equations. 
-            **kwargs: keyword arguments of constants (python variables in keys of data that 
-                are not to be solved for)
+class LogProductSolver:
+    def __init__(self, data, wgts={}, sparse=False, **kwargs):
+        """A log-solver for systems of equations of the form a*b = 1.0.
 
-        Returns:
-            None
+        Parameters
+        ----------
+        data
+            dict mapping nonlinear product equations, written as valid
+            python-interpetable strings that include the variables in question, to
+            (complex) numbers or numpy arrarys. Variables with trailing underscores '_'
+            are interpreted as complex conjugates (e.g. x*y_ parses as x * y.conj()).
+        wgts
+            dict that maps equation strings from data to real weights to apply to each
+            equation. Weights are treated as 1/sigma^2. All equations in the data must
+            have a weight if wgts is not the default, {}, which means all 1.0s.
+        sparse : bool.
+            If True, represents A matrix sparsely (though  AtA, Aty end up dense).
+            May be faster for certain systems of equations.
+        **kwargs: keyword arguments of constants (python variables in keys of data that
+            are not to be solved for)
         """
         keys = list(data.keys())
         wgts = verify_weights(wgts, keys)
-        eqs = [ast_getterms(ast.parse(k, mode='eval')) for k in keys]
+        eqs = [ast_getterms(ast.parse(k, mode="eval")) for k in keys]
         logamp, logphs = {}, {}
         logampw, logphsw = {}, {}
-        for k,eq in zip(keys,eqs):
-            assert(len(eq) == 1) # equations have to be purely products---no adds
-            eqamp = jointerms([conjterm([t],mode='amp') for t in eq[0]])
-            eqphs = jointerms([conjterm([t],mode='phs') for t in eq[0]])
+        for k, eq in zip(keys, eqs):
+            assert len(eq) == 1  # equations have to be purely products---no adds
+            eqamp = jointerms([conjterm([t], mode="amp") for t in eq[0]])
+            eqphs = jointerms([conjterm([t], mode="phs") for t in eq[0]])
             dk = np.log(data[k])
-            logamp[eqamp],logphs[eqphs] = dk.real, dk.imag
-            try: logampw[eqamp],logphsw[eqphs] = wgts[k], wgts[k]
-            except(KeyError): pass
-        constants = kwargs.pop('constants', kwargs)
-        self.dtype = infer_dtype(list(data.values()) + list(constants.values()) + list(wgts.values()))
+            logamp[eqamp], logphs[eqphs] = dk.real, dk.imag
+            try:
+                logampw[eqamp], logphsw[eqphs] = wgts[k], wgts[k]
+            except KeyError:
+                pass
+        constants = kwargs.pop("constants", kwargs)
+        self.dtype = infer_dtype(
+            list(data.values()) + list(constants.values()) + list(wgts.values())
+        )
         logamp_consts, logphs_consts = {}, {}
         for k in constants:
-            c = np.log(constants[k]) # log unwraps complex circle at -pi
+            c = np.log(constants[k])  # log unwraps complex circle at -pi
             logamp_consts[k], logphs_consts[k] = c.real, c.imag
-        self.ls_amp = LinearSolver(logamp, logampw, sparse=sparse, constants=logamp_consts)
+        self.ls_amp = LinearSolver(
+            logamp, logampw, sparse=sparse, constants=logamp_consts
+        )
         if self.dtype in (np.complex64, np.complex128):
             # XXX worry about enumrating these here without
             # explicitly ensuring that these are the support complex
             # dtypes.
             # see https://github.com/HERA-Team/linsolve/issues/33
-            self.ls_phs = LinearSolver(logphs, logphsw, sparse=sparse, constants=logphs_consts)
+            self.ls_phs = LinearSolver(
+                logphs, logphsw, sparse=sparse, constants=logphs_consts
+            )
         else:
-            self.ls_phs = None # no phase term to solve for
+            self.ls_phs = None  # no phase term to solve for
 
-    def solve(self, rcond=None, mode='default'):
+    def solve(self, rcond=None, mode="default"):
         """Solve both amplitude and phase by taking the log of both sides to linearize.
 
-        Args:
-            rcond: cutoff ratio for singular values useed in numpy.linalg.lstsq, numpy.linalg.pinv,
-                or (if sparse) as atol and btol in scipy.sparse.linalg.lsqr
-                Default: None (resolves to machine precision for inferred dtype)
-            mode: 'default', 'lsqr', 'pinv', or 'solve', selects which inverter to use, unless all equations share the same A matrix, in which case pinv is always used`. 
-                'default': alias for 'pinv'.
-                'lsqr': uses numpy.linalg.lstsq to do an inversion-less solve.  Usually 
-                    the fastest solver.
-                'solve': uses numpy.linalg.solve to do an inversion-less solve.  Fastest, 
-                    but only works for fully constrained systems of equations.
-                'pinv': uses numpy.linalg.pinv to perform a pseudo-inverse and then solves.  Can
-                    sometimes be more numerically stable (but slower) than 'lsqr'.
-                All of these modes are superceded if the same system of equations applies
-                to all datapoints in an array.  In this case, a inverse-based method is used so
-                that the inverted matrix can be re-used to solve all array indices.
-
-        Returns:
-            sol: a dictionary of complex solutions with variables as keys
+        Parameters
+        ----------
+        rcond
+            cutoff ratio for singular values used in :func:`numpy.linalg.lstsq`,
+            :func:`numpy.linalg.pinv`, or (if sparse) as atol and btol in
+            :func:`scipy.sparse.linalg.lsqr`. Default is to resolve to machine precision
+            for inferred dtype.
+        mode : {'default', 'lsqr', 'pinv', or 'solve'}
+            Selects which inverter to use, unless all equations share the same A matrix,
+            in which case pinv is always used.
+
+            * 'default': alias for 'pinv'.
+            * 'lsqr': uses numpy.linalg.lstsq to do an inversion-less solve.  Usually
+              the fastest solver.
+            * 'solve': uses numpy.linalg.solve to do an inversion-less solve.  Fastest,
+              but only works for fully constrained systems of equations.
+            * 'pinv': uses numpy.linalg.pinv to perform a pseudo-inverse and then
+              solves. Can sometimes be more numerically stable (but slower) than 'lsqr'.
+
+            All of these modes are superceded if the same system of equations applies
+            to all datapoints in an array.  In this case, a inverse-based method is
+            used so that the inverted matrix can be re-used to solve all array indices.
+
+        Returns
+        -------
+        sol
+            a dictionary of complex solutions with variables as keys
         """
         sol_amp = self.ls_amp.solve(rcond=rcond, mode=mode)
         if self.ls_phs is not None:
             sol_phs = self.ls_phs.solve(rcond=rcond, mode=mode)
-            sol = {k: np.exp(sol_amp[k] + 
-                      np.complex64(1j) * sol_phs[k]).astype(self.dtype)
-                      for k in sol_amp.keys()}
+            return {
+                k: np.exp(sol_amp[k] + np.complex64(1j) * sol_phs[k]).astype(self.dtype)
+                for k in sol_amp.keys()
+            }
         else:
-            sol = {k: np.exp(sol_amp[k]).astype(self.dtype)
-                      for k in sol_amp.keys()}
-        return sol
+            return {k: np.exp(sol_amp[k]).astype(self.dtype) for k in sol_amp.keys()}
 
-def taylor_expand(terms, consts={}, prepend='d'):
-    '''First-order Taylor expand terms (product of variables or the sum of a 
-    product of variables) wrt all parameters except those listed in consts.'''
-    taylors = []
-    for term in terms: taylors.append(term)
+
+def taylor_expand(terms, consts=None, prepend="d"):
+    """First-order Taylor expand terms.
+
+    The product of variables or the sum of a product of variables wrt all parameters
+    except those listed in consts.
+    """
+    if consts is None:
+        consts = {}
+    taylors = list(terms)
     for term in terms:
-        for i,t in enumerate(term):
-            if type(t) is not str or get_name(t) in consts: continue
-            taylors.append(term[:i]+[prepend+t]+term[i+1:])
+        for i, t in enumerate(term):
+            if type(t) is not str or get_name(t) in consts:
+                continue
+            taylors.append(term[:i] + [prepend + t] + term[i + 1 :])
     return taylors
 
 
 # XXX make a version of linproductsolver that taylor expands in e^{a+bi} form
 # see https://github.com/HERA-Team/linsolve/issues/15
 class LinProductSolver:
-
     def __init__(self, data, sol0, wgts={}, sparse=False, **kwargs):
-        """Set up a nonlinear system of equations of the form a*b + c*d = 1.0 
-        to linearize via Taylor expansion and solve iteratively using the Gauss-Newton algorithm.
+        """Set up a nonlinear system of equations of the form a*b + c*d = 1.0.
 
-        Args:
-            data: Dictionary that maps nonlinear product equations, written as valid python-interpetable 
-                strings that include the variables in question, to (complex) numbers or numpy arrarys. 
-                Variables with trailing underscores '_' are interpreted as complex conjugates (e.g. x*y_ 
-                parses as x * y.conj()).
-            sol0: Dictionary mapping all variables (as keyword strings) to their starting guess values.
-                This is the point that is Taylor expanded around, so it must be relatively close to the
-                true chi^2 minimizing solution. In the same format as that produced by 
-                linsolve.LogProductSolver.solve() or linsolve.LinProductSolver.solve().
-            wgts: Dictionary that maps equation strings from data to real weights to apply to each 
-                equation. Weights are treated as 1/sigma^2. All equations in the data must have a weight 
-                if wgts is not the default, {}, which means all 1.0s.
-            sparse: Boolean (default False). If True, represents A matrix sparsely (though AtA, Aty end up dense)
-                May be faster for certain systems of equations. 
-            **kwargs: keyword arguments of constants (python variables in keys of data that 
-                are not to be solved for)
+        Linearize via Taylor expansion and solve iteratively using the Gauss-Newton
+        algorithm.
 
-        Returns:
-            None
+        Parameters
+        ----------
+        data
+            dict that maps nonlinear product equations, written as valid
+            python-interpetable strings that include the variables in question, to
+            (complex) numbers or numpy arrarys. Variables with trailing underscores '_'
+            are interpreted as complex conjugates (e.g. x*y_ parses as x * y.conj()).
+        sol0
+            dict mapping all variables (as keyword strings) to their starting guess
+            values. This is the point that is Taylor expanded around, so it must be
+            relatively close to the true chi^2 minimizing solution. In the same format
+            as that produced by :func:`~LogProductSolver.solve()` or
+            :func:`~LinProductSolver.solve()`.
+        wgts
+            dict that maps equation strings from data to real weights to apply to each
+            equation. Weights are treated as 1/sigma^2. All equations in the data must
+            have a weight if wgts is not the default, {}, which means all 1.0s.
+        sparse : bool
+            If True, represents A matrix sparsely (though AtA, Aty end up dense)
+            May be faster for certain systems of equations.
+        **kwargs: keyword arguments of constants (python variables in keys of data that
+            are not to be solved for)
         """
         # XXX make this something hard to collide with
         # see https://github.com/HERA-Team/linsolve/issues/17
-        self.prepend = 'd'
+        self.prepend = "d"
         self.data, self.sparse, self.keys = data, sparse, list(data.keys())
         self.wgts = verify_weights(wgts, self.keys)
-        constants = kwargs.pop('constants', kwargs)
+        constants = kwargs.pop("constants", kwargs)
         self.init_kwargs, self.sols_kwargs = constants, deepcopy(constants)
         self.sols_kwargs.update(sol0)
         self.all_terms, self.taylors, self.taylor_keys = self.gen_taylors()
-        self.build_solver(sol0) 
+        self.build_solver(sol0)
         self.dtype = self.ls.dtype
-    
+
     def gen_taylors(self, keys=None):
-        '''Parses all terms, performs a taylor expansion, and maps equation keys to taylor expansion keys.'''
-        if keys is None: keys = self.keys
-        all_terms = [ast_getterms(ast.parse(k, mode='eval')) for k in keys]
+        """Perform Taylor expansion, and map eq. keys to taylor expansion keys."""
+        if keys is None:
+            keys = self.keys
+        all_terms = [ast_getterms(ast.parse(k, mode="eval")) for k in keys]
         taylors, taylor_keys = [], {}
         for terms, k in zip(all_terms, keys):
             taylor = taylor_expand(terms, self.init_kwargs, prepend=self.prepend)
             taylors.append(taylor)
-            taylor_keys[k] = jointerms(taylor[len(terms):])
+            taylor_keys[k] = jointerms(taylor[len(terms) :])
         return all_terms, taylors, taylor_keys
 
     def build_solver(self, sol0):
-        '''Builds a LinearSolver using the taylor expansions and all relevant constants.
-        Update it with the latest solutions.'''
+        """Builds a LinearSolver using the taylor expansions and all relevant constants.
+
+        Update it with the latest solutions.
+        """
         dlin, wlin = {}, {}
         for k in self.keys:
             tk = self.taylor_keys[k]
-            dlin[tk] = self.data[k] #in theory, this will always be replaced with data - ans0 before use
-            try: 
+            # in theory, this will always be replaced with data - ans0 before use
+            dlin[tk] = self.data[k]
+            try:
                 wlin[tk] = self.wgts[k]
-            except(KeyError):
+            except KeyError:
                 pass
-        self.ls = LinearSolver(dlin, wgts=wlin, sparse=self.sparse, constants=self.sols_kwargs)
-        self.eq_dict = {eq.val: eq for eq in self.ls.eqs} #maps taylor string expressions to linear equations 
-        #Now make sure every taylor equation has every relevant constant, even if they don't appear in the derivative terms.
-        for k,terms in zip(self.keys, self.all_terms):
+        self.ls = LinearSolver(
+            dlin, wgts=wlin, sparse=self.sparse, constants=self.sols_kwargs
+        )
+        self.eq_dict = {
+            eq.val: eq for eq in self.ls.eqs
+        }  # maps taylor string expressions to linear equations
+        # Now make sure every taylor equation has every relevant constant, even if
+        # they don't appear in the derivative terms.
+        for k, terms in zip(self.keys, self.all_terms):
             for term in terms:
                 for t in term:
                     t_name = get_name(t)
                     if t_name in self.sols_kwargs:
-                        self.eq_dict[self.taylor_keys[k]].add_const(t_name, self.sols_kwargs)
+                        self.eq_dict[self.taylor_keys[k]].add_const(
+                            t_name, self.sols_kwargs
+                        )
         self._update_solver(sol0)
 
     def _update_solver(self, sol):
-        '''Update all constants in the internal LinearSolver and its LinearEquations based on new solutions.
-        Also update the residuals (data - ans0) for next iteration.'''
+        """Update the solver.
+
+        Updates all constants in the internal LinearSolver and its LinearEquations
+        based on new solutions. Also update the residuals (data - ans0) for next
+        iteration.
+        """
         self.sol0 = sol
         self.sols_kwargs.update(sol)
         for eq in self.ls.eqs:
-            for c in list(eq.consts.values()): 
-                if c.name in sol: eq.consts[c.name].val = self.sols_kwargs[c.name]
+            for c in list(eq.consts.values()):
+                if c.name in sol:
+                    eq.consts[c.name].val = self.sols_kwargs[c.name]
             self.ls.consts.update(eq.consts)
         ans0 = self._get_ans0(sol)
-        for k in ans0: self.ls.data[self.taylor_keys[k]] = self.data[k]-ans0[k]
+        for k in ans0:
+            self.ls.data[self.taylor_keys[k]] = self.data[k] - ans0[k]
 
     def _get_ans0(self, sol, keys=None):
-        '''Evaluate the system of equations given input sol. 
-        Specify keys to evaluate only a subset of the equations.'''
-        if keys is None: 
+        """Evaluate the system of equations given input sol.
+
+        Specify keys to evaluate only a subset of the equations.
+        """
+        if keys is None:
             keys = self.keys
             all_terms = self.all_terms
             taylors = self.taylors
         else:
             all_terms, taylors, _ = self.gen_taylors(keys)
         ans0 = {}
-        for k,taylor,terms in zip(keys,taylors,all_terms):
+        for k, taylor, terms in zip(keys, taylors, all_terms):
             eq = self.eq_dict[self.taylor_keys[k]]
-            ans0[k] = np.sum([eq.eval_consts(t) for t in taylor[:len(terms)]], axis=0)
+            ans0[k] = np.sum([eq.eval_consts(t) for t in taylor[: len(terms)]], axis=0)
         return ans0
 
-    def solve(self, rcond=None, mode='default'):
-        '''Executes one iteration of a LinearSolver on the taylor-expanded system of 
-        equations, improving sol0 to get sol.
-
-        Args:
-            rcond: cutoff ratio for singular values useed in numpy.linalg.lstsq, numpy.linalg.pinv,
-                or (if sparse) as atol and btol in scipy.sparse.linalg.lsqr
-                Default: None (resolves to machine precision for inferred dtype)
-            mode: 'default', 'lsqr', 'pinv', or 'solve', selects which inverter to use, unless all equations share the same A matrix, in which case pinv is always used`. 
-                'default': alias for 'pinv'.
-                'lsqr': uses numpy.linalg.lstsq to do an inversion-less solve.  Usually 
-                    the fastest solver.
-                'solve': uses numpy.linalg.solve to do an inversion-less solve.  Fastest, 
-                    but only works for fully constrained systems of equations.
-                'pinv': uses numpy.linalg.pinv to perform a pseudo-inverse and then solves.  Can
-                    sometimes be more numerically stable (but slower) than 'lsqr'.
-                All of these modes are superceded if the same system of equations applies
-                to all datapoints in an array.  In this case, a inverse-based method is used so
-                that the inverted matrix can be re-used to solve all array indices.
-
-        Returns:
-            sol: a dictionary of complex solutions with variables as keys
-        '''
+    def solve(self, rcond=None, mode="default"):
+        """Execute one iteration of a LinearSolver.
+
+        Executes on the taylor-expanded system of equations, improving sol0 to get sol.
+
+        Parameters
+        ----------
+        rcond
+            cutoff ratio for singular values useed in :func:`numpy.linalg.lstsq`,
+            :func:`numpy.linalg.pinv`, or (if sparse) as atol and btol in
+            :func:`scipy.sparse.linalg.lsqr`. Default is to resolve to machine precision
+            for inferred dtype.
+        mode : {}'default', 'lsqr', 'pinv', or 'solve'}
+            Selects which inverter to use, unless all equations share the same A matrix,
+            in which case pinv is always used`.
+
+            * 'default': alias for 'pinv'.
+            * 'lsqr': uses numpy.linalg.lstsq to do an inversion-less solve.  Usually
+              the fastest solver.
+            * 'solve': uses numpy.linalg.solve to do an inversion-less solve.  Fastest,
+              but only works for fully constrained systems of equations.
+            * 'pinv': uses numpy.linalg.pinv to perform a pseudo-inverse and then
+              solves. Can sometimes be more numerically stable (but slower) than 'lsqr'.
+
+            All of these modes are superceded if the same system of equations applies
+            to all datapoints in an array.  In this case, a inverse-based method is
+            used so that the inverted matrix can be re-used to solve all array indices.
+
+        Returns
+        -------
+        sol
+            a dictionary of complex solutions with variables as keys
+        """
         dsol = self.ls.solve(rcond=rcond, mode=mode)
         sol = {}
         for dk in dsol:
-            k = dk[len(self.prepend):]
+            k = dk[len(self.prepend) :]
             sol[k] = self.sol0[k] + dsol[dk]
         return sol
-    
+
     def eval(self, sol, keys=None):
-        '''Returns a dictionary evaluating data keys to the current values given sol and consts.
-        Uses the stored data object unless otherwise specified.'''
-        if type(keys) is str: keys = [keys]
-        elif type(keys) is dict: keys = list(keys.keys())
+        """Get a dict mapping data keys to the current values given sol and consts.
+
+        Uses the stored data object unless otherwise specified.
+        """
+        if type(keys) is str:
+            keys = [keys]
+        elif type(keys) is dict:
+            keys = list(keys.keys())
         return self._get_ans0(sol, keys=keys)
-    
+
     def chisq(self, sol, data=None, wgts=None):
-        '''Compute Chi^2 = |obs - mod|^2 / sigma^2 for the specified solution. Weights are treated as 1/sigma^2. 
-        wgts = {} means sigma = 1. Uses the stored data and weights unless otherwise overwritten.'''
-        if data is None: 
+        """Compute ``Chi^2 = |obs - mod|^2 / sigma^2`` for the specified solution.
+
+        Weights are treated as 1/sigma^2. wgts = {} means sigma = 1. Uses the stored
+        data and weights unless otherwise overwritten.
+        """
+        if data is None:
             data = self.data
-        if wgts is None: 
+        if wgts is None:
             wgts = self.wgts
         wgts = verify_weights(wgts, list(data.keys()))
         return self.ls._chisq(sol, data, wgts, self.eval)
 
-    def solve_iteratively(self, conv_crit=None, maxiter=50, mode='default', verbose=False):
-        """Repeatedly solves and updates linsolve until convergence or maxiter is reached. 
-        Returns a meta object containing the number of iterations, chisq, and convergence criterion.
-
-        Args:
-            conv_crit: A convergence criterion below which to stop iterating. 
-                Converegence is measured L2-norm of the change in the solution of all the variables
-                divided by the L2-norm of the solution itself.
-                Default: None (resolves to machine precision for inferred dtype)
-            maxiter: An integer maximum number of iterations to perform before quitting. Default 50.
-            mode: 'default', 'lsqr', 'pinv', or 'solve', selects which inverter to use, unless all equations share the same A matrix, in which case pinv is always used`. 
-                'default': alias for 'pinv'.
-                'lsqr': uses numpy.linalg.lstsq to do an inversion-less solve.  Usually 
-                    the fastest solver.
-                'solve': uses numpy.linalg.solve to do an inversion-less solve.  Fastest, 
-                    but only works for fully constrained systems of equations.
-                'pinv': uses numpy.linalg.pinv to perform a pseudo-inverse and then solves.  Can
-                    sometimes be more numerically stable (but slower) than 'lsqr'.
-                All of these modes are superceded if the same system of equations applies
-                to all datapoints in an array.  In this case, a inverse-based method is used so
-                that the inverted matrix can be re-used to solve all array indices.
-            verbose: print information about iterations
-
-        Returns: meta, sol
-            meta: a dictionary with metadata about the solution, including
-                iter: the number of iterations taken to reach convergence (or maxiter)
-                chisq: the chi^2 of the solution produced by the final iteration
-                conv_crit: the convergence criterion evaluated at the final iteration
-            sol: a dictionary of complex solutions with variables as keys
+    def solve_iteratively(
+        self, conv_crit=None, maxiter=50, mode="default", verbose=False
+    ):
+        """Repeatedly solve and update linsolve until convergence or maxiter is reached.
+
+        Parameters
+        ----------
+        conv_crit
+            A convergence criterion below which to stop iterating.
+            Converegence is measured L2-norm of the change in the solution of all the
+            variables divided by the L2-norm of the solution itself.
+            Default: None (resolves to machine precision for inferred dtype)
+        maxiter : int, optional (default 50)
+            An integer maximum number of iterations to perform before quitting.
+        mode : {}'default', 'lsqr', 'pinv', or 'solve'}
+            Selects which inverter to use, unless all equations share the same A matrix,
+            in which case pinv is always used`.
+
+            * 'default': alias for 'pinv'.
+            * 'lsqr': uses numpy.linalg.lstsq to do an inversion-less solve.  Usually
+              the fastest solver.
+            * 'solve': uses numpy.linalg.solve to do an inversion-less solve.  Fastest,
+              but only works for fully constrained systems of equations.
+            * 'pinv': uses numpy.linalg.pinv to perform a pseudo-inverse and then
+              solves. Can sometimes be more numerically stable (but slower) than 'lsqr'.
+
+            All of these modes are superceded if the same system of equations applies
+            to all datapoints in an array.  In this case, a inverse-based method is
+            used so that the inverted matrix can be re-used to solve all array indices.
+
+        verbose : bool
+            print information about iterations
+
+        Returns
+        -------
+        meta : dict
+            A dictionary with metadata about the solution, including
+            * iter: the number of iterations taken to reach convergence (or maxiter)
+            * chisq: the chi^2 of the solution produced by the final iteration
+            * conv_crit: the convergence criterion evaluated at the final iteration
+        sol : dict
+            A dictionary of complex solutions with variables as keys
         """
         if conv_crit is None:
             conv_crit = np.finfo(self.dtype).resolution
-        for i in range(1,maxiter+1):
+        for i in range(1, maxiter + 1):
             if verbose:
-                print('Beginning iteration %d/%d' % (i,maxiter))
-            # rcond=conv_crit works because you can't get better precision than the accuracy of your inversion
-            # and vice versa, there's no real point in inverting with greater precision than you are shooting for
+                print("Beginning iteration %d/%d" % (i, maxiter))
+            # rcond=conv_crit works because you can't get better precision than the
+            # accuracy of your inversion and vice versa, there's no real point in
+            # inverting with greater precision than you are shooting for
             new_sol = self.solve(rcond=conv_crit, mode=mode)
-            deltas = [new_sol[k]-self.sol0[k] for k in new_sol.keys()]
-            conv = np.linalg.norm(deltas, axis=0) / np.linalg.norm(list(new_sol.values()),axis=0)
+            deltas = [new_sol[k] - self.sol0[k] for k in new_sol.keys()]
+            conv = np.linalg.norm(deltas, axis=0) / np.linalg.norm(
+                list(new_sol.values()), axis=0
+            )
             if np.all(conv < conv_crit) or i == maxiter:
-                meta = {'iter': i, 'chisq': self.chisq(new_sol), 'conv_crit': conv}
+                meta = {"iter": i, "chisq": self.chisq(new_sol), "conv_crit": conv}
                 return meta, new_sol
             self._update_solver(new_sol)
```

### Comparing `linsolve-1.1.0/linsolve/tests/benchmark_A_large_shared.py` & `linsolve-1.1.2/tests/benchmark_A_small_shared.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,35 @@
-'''Benchmark a system of equations with a large number of independent
-parameters and a modest number of parallel instances that allow the
-inverted A matrix to be reused.'''
-import linsolve
+"""Benchmark a system of equations with a small number of independent parameters.
+
+Use a large number of parallel instances that allow the inverted A matrix to be reused.
+"""
+
+import random
+import time
+
 import numpy as np
-import time, random
+
+import linsolve
 
 np.random.seed(0)
 
-NPRMS = 2000
-NEQS = 5000
-SIZE = 100
-sparse = False # sparse: 1.30 s, dense: 1.50 s
+NPRMS = 10
+NEQS = 100
+SIZE = 1000000
+# dense: 0.48 s
 
-prms = {'g%d' % i: np.arange(SIZE) for i in range(NPRMS)}
+prms = {"g%d" % i: np.arange(SIZE) for i in range(NPRMS)}
 prm_list = list(prms.keys())
 
-eqs = [('+'.join(['%s'] * 5))  % tuple(random.sample(prm_list, 5)) 
-            for i in range(NEQS)]
+eqs = [("+".join(["%s"] * 5)) % tuple(random.sample(prm_list, 5)) for _ in range(NEQS)]
 
 data = {eq: eval(eq, prms) for eq in eqs}
 
-ls = linsolve.LinearSolver(data, sparse=sparse)
+ls = linsolve.LinearSolver(data, sparse=False)
 t0 = time.time()
 sol = ls.solve()
 t1 = time.time()
 
-print('Solved in {}'.format(t1-t0))
+print(f"Solved in {t1 - t0}")
 
 for k in prm_list:
-    assert np.mean(np.abs(sol[k] - prms[k])**2) < 1e-3
+    assert np.mean(np.abs(sol[k] - prms[k]) ** 2) < 1e-3
```

### Comparing `linsolve-1.1.0/linsolve/tests/benchmark_A_large_shared_sparse.py` & `linsolve-1.1.2/tests/benchmark_A_small_shared_sparse.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,36 @@
-'''Benchmark a system of equations with a large number of independent
-parameters and a modest number of parallel instances that allow the
-inverted A matrix to be reused. In this case, we test the speedup
-for using a sparse representation.'''
-import linsolve
+"""Benchmark a system of equations with a small number of independent parameters.
+
+Use a large number of parallel instances that allow the inverted A matrix to be reused.
+In this case, we benchmark the case when a sparse representation of A is used.
+"""
+
+import random
+import time
+
 import numpy as np
-import time, random
+
+import linsolve
 
 np.random.seed(0)
 
-NPRMS = 2000
-NEQS = 5000
-SIZE = 100
-sparse = True # sparse: 1.30 s, dense: 1.50 s
+NPRMS = 10
+NEQS = 100
+SIZE = 1000000
+# sparse: 0.82 s
 
-prms = {'g%d' % i: np.arange(SIZE) for i in range(NPRMS)}
+prms = {"g%d" % i: np.arange(SIZE) for i in range(NPRMS)}
 prm_list = list(prms.keys())
 
-eqs = [('+'.join(['%s'] * 5))  % tuple(random.sample(prm_list, 5)) 
-            for i in range(NEQS)]
+eqs = [("+".join(["%s"] * 3)) % tuple(random.sample(prm_list, 3)) for _ in range(NEQS)]
 
 data = {eq: eval(eq, prms) for eq in eqs}
 
-ls = linsolve.LinearSolver(data, sparse=sparse)
+ls = linsolve.LinearSolver(data, sparse=True)
 t0 = time.time()
 sol = ls.solve()
 t1 = time.time()
 
-print('Solved in {}'.format(t1-t0))
+print(f"Solved in {t1 - t0}")
 
 for k in prm_list:
-    assert np.mean(np.abs(sol[k] - prms[k])**2) < 1e-3
+    assert np.mean(np.abs(sol[k] - prms[k]) ** 2) < 1e-3
```

### Comparing `linsolve-1.1.0/linsolve/tests/benchmark_A_small_shared.py` & `linsolve-1.1.2/tests/benchmark_A_small_unique.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,40 @@
-'''Benchmark a system of equations with a small number of independent
-parameters and a large number of parallel instances that allow the
-inverted A matrix to be reused.'''
-import linsolve
+"""Benchmark a system of equations with a small number of independent parameters.
+
+Use a large number of instances with different coefficients so that inversions of the
+A matrix cannot be reused.
+"""
+import random
+import time
+
 import numpy as np
-import time, random
+
+import linsolve
 
 np.random.seed(0)
 
 NPRMS = 10
 NEQS = 100
-SIZE = 1000000
-# dense: 0.48 s
+SIZE = 100000
+# --> MODE = 'solve' # dense:1.56 s
+MODE = "lsqr"  # dense:5.4 s
+# --> MODE = 'pinv'  # dense:3.4 s
 
-prms = {'g%d' % i: np.arange(SIZE) for i in range(NPRMS)}
+prms = {"g%d" % i: np.arange(SIZE) for i in range(NPRMS)}
 prm_list = list(prms.keys())
+prms["c0"] = np.arange(SIZE)
 
-eqs = [('+'.join(['%s'] * 5))  % tuple(random.sample(prm_list, 5)) 
-            for i in range(NEQS)]
+eqs = [
+    ("+c0*".join(["%s"] * 5)) % tuple(random.sample(prm_list, 5)) for i in range(NEQS)
+]
 
 data = {eq: eval(eq, prms) for eq in eqs}
 
-ls = linsolve.LinearSolver(data, sparse=False)
+ls = linsolve.LinearSolver(data, c0=prms["c0"], sparse=False)
 t0 = time.time()
-sol = ls.solve()
+sol = ls.solve(mode=MODE)
 t1 = time.time()
 
-print('Solved in {}'.format(t1-t0))
+print(f"Solved in {t1 - t0}")
 
 for k in prm_list:
-    assert np.mean(np.abs(sol[k] - prms[k])**2) < 1e-3
+    assert np.mean(np.abs(sol[k] - prms[k]) ** 2) < 1e-3
```

### Comparing `linsolve-1.1.0/linsolve/tests/benchmark_A_small_shared_sparse.py` & `linsolve-1.1.2/tests/benchmark_A_large_shared_sparse.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,36 @@
-'''Benchmark a system of equations with a small number of independent
-parameters and a large number of parallel instances that allow the
-inverted A matrix to be reused. In this case, we benchmark the
-case when a sparse representation of A is used.'''
-import linsolve
+"""Benchmark a system of equations with a large number of independent parameters.
+
+Use a modest number of parallel instances that allow the inverted A matrix to be reused.
+In this case, we test the speedup for using a sparse representation.
+"""
+
+import random
+import time
+
 import numpy as np
-import time, random
+
+import linsolve
 
 np.random.seed(0)
 
-NPRMS = 10
-NEQS = 100
-SIZE = 1000000
-# sparse: 0.82 s
+NPRMS = 2000
+NEQS = 5000
+SIZE = 100
+sparse = True  # sparse: 1.30 s, dense: 1.50 s
 
-prms = {'g%d' % i: np.arange(SIZE) for i in range(NPRMS)}
+prms = {"g%d" % i: np.arange(SIZE) for i in range(NPRMS)}
 prm_list = list(prms.keys())
 
-eqs = [('+'.join(['%s'] * 3))  % tuple(random.sample(prm_list, 3)) 
-            for i in range(NEQS)]
+eqs = [("+".join(["%s"] * 5)) % tuple(random.sample(prm_list, 5)) for _ in range(NEQS)]
 
 data = {eq: eval(eq, prms) for eq in eqs}
 
-ls = linsolve.LinearSolver(data, sparse=True)
+ls = linsolve.LinearSolver(data, sparse=sparse)
 t0 = time.time()
 sol = ls.solve()
 t1 = time.time()
 
-print('Solved in {}'.format(t1-t0))
+print(f"Solved in {t1 - t0}")
 
 for k in prm_list:
-    assert np.mean(np.abs(sol[k] - prms[k])**2) < 1e-3
+    assert np.mean(np.abs(sol[k] - prms[k]) ** 2) < 1e-3
```

### Comparing `linsolve-1.1.0/linsolve/tests/benchmark_A_small_unique.py` & `linsolve-1.1.2/tests/benchmark_A_small_unique_sparse.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,42 @@
-'''Benchmark a system of equations with a small number of independent
-parameters and a large number of instances with different coefficients
-so that inversions of the A matrix cannot be reused.'''
-import linsolve
+"""Benchmark a system of equations with a small number of independent parameters.
+
+Use a large number of instances with different coefficients so that inversions of the
+A matrix cannot be reused. In this case, we benchmark the case when a sparse
+representation of A is used.
+"""
+import random
+import time
+
 import numpy as np
-import time, random
+
+import linsolve
 
 np.random.seed(0)
 
 NPRMS = 10
 NEQS = 100
 SIZE = 100000
-#MODE = 'solve' # dense:1.56 s
-MODE = 'lsqr'  # dense:5.4 s
-#MODE = 'pinv'  # dense:3.4 s
+MODE = "solve"  # sparse: 0.43 s
+
+# --> MODE = 'lsqr'  # sparse: 3.8
+# --> MODE = 'pinv'  # sparse: 2.72 s
 
-prms = {'g%d' % i: np.arange(SIZE) for i in range(NPRMS)}
+prms = {"g%d" % i: np.arange(SIZE) for i in range(NPRMS)}
 prm_list = list(prms.keys())
-prms['c0'] = np.arange(SIZE)
+prms["c0"] = np.arange(SIZE)
 
-eqs = [('+c0*'.join(['%s'] * 5))  % tuple(random.sample(prm_list, 5)) 
-            for i in range(NEQS)]
+eqs = [
+    ("+c0*".join(["%s"] * 2)) % tuple(random.sample(prm_list, 2)) for i in range(NEQS)
+]
 
 data = {eq: eval(eq, prms) for eq in eqs}
 
-ls = linsolve.LinearSolver(data, c0=prms['c0'], sparse=False)
+ls = linsolve.LinearSolver(data, c0=prms["c0"], sparse=True)
 t0 = time.time()
 sol = ls.solve(mode=MODE)
 t1 = time.time()
 
-print('Solved in {}'.format(t1-t0))
+print(f"Solved in {t1 - t0}")
 
 for k in prm_list:
-    assert np.mean(np.abs(sol[k] - prms[k])**2) < 1e-3
+    assert np.mean(np.abs(sol[k] - prms[k]) ** 2) < 1e-3
```

### Comparing `linsolve-1.1.0/linsolve_example.ipynb` & `linsolve-1.1.2/linsolve_example.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9898193760262726%*

 * *Differences: {"'cells'": '{4: {\'outputs\': {0: {\'text\': ["{\'x\': 1.0, \'y\': 2.0}\\n"]}}}, 6: '*

 * *            "{'execution_count': None, 'outputs': []}, 8: {'execution_count': None, 'outputs': "*

 * *            "[]}, 10: {'execution_count': None, 'outputs': []}, 12: {'execution_count': None, "*

 * *            "'outputs': []}, 14: {'execution_count': None, 'outputs': []}, 16: {'execution_count': "*

 * *            "None, 'outputs': []}, 18: {'execution_count': None, 'outputs': []}, 22: "*

 * *            "{'execution_count': None, 'outp […]*

```diff
@@ -82,15 +82,15 @@
                 "scrolled": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "{'x': 1.0, 'y': 2.000002}\n"
+                        "{'x': 1.0, 'y': 2.0}\n"
                     ]
                 }
             ],
             "source": [
                 "import numpy as np\n",
                 "import linsolve\n",
                 "\n",
@@ -117,34 +117,26 @@
                 "### Array Systems\n",
                 "\n",
                 "Often, it its useful to solve the same system of equations for many different \"measurements\" on the LHS of the system of equations. In this case, the dictionary of equations can map strings to $N$-dimensional numpy arrays."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": null,
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2020-06-13T00:06:10.891288Z",
                     "start_time": "2020-06-13T00:06:10.548Z"
                 },
                 "run_control": {
                     "frozen": false,
                     "read_only": false
                 }
             },
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "{'x': array([1., 2.]), 'y': array([2., 4.])}\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "data = {'3*x+4*y': np.array([11.0,22.0]), '-1*x-3*y': np.array([-7.0,-14.0])}\n",
                 "ls = linsolve.LinearSolver(data)\n",
                 "sol = ls.solve()\n",
                 "print(sol)"
             ]
         },
@@ -160,34 +152,26 @@
                 "### Constants\n",
                 "\n",
                 "While all terms that evaluate to valid python variables in the dictionary keys are assumed to be variables, it is possible to designate some of them as constants. They are passed `LinearSolver` via its `kwargs`. Constants can be expressed either as single numbers or as arrays that can broadcast according to `numpy` rules to the shape of the data, allowing the equations to change between solves."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": null,
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2020-06-13T00:06:10.891963Z",
                     "start_time": "2020-06-13T00:06:10.551Z"
                 },
                 "run_control": {
                     "frozen": false,
                     "read_only": false
                 }
             },
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "{'x': array([ 1., 10.]), 'y': array([ 2., -2.])}\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "data = {'3*x+a*y': np.array([11.0,22.0]), 'b*x-3*y': np.array([-7.0,-14.0])}\n",
                 "ls = linsolve.LinearSolver(data, a=4, b=np.array([-1,-2]))\n",
                 "sol = ls.solve()\n",
                 "print(sol)"
             ]
         },
@@ -201,34 +185,26 @@
             },
             "source": [
                 "Any variable names that are not assigned values are assumed to be parameters in need of solutions.  However, `linsolve` being a linear solver, if more than one variable per term is unknown (i.e. if the expression is non-linear), `linsolve` will raise an `AssertionError`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": null,
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2020-06-13T00:06:10.892560Z",
                     "start_time": "2020-06-13T00:06:10.552Z"
                 },
                 "run_control": {
                     "frozen": false,
                     "read_only": false
                 }
             },
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "AssertionError encountered.\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "try:\n",
                 "    ls = linsolve.LinearSolver({'a*x':6., 'b*x':8.}) # raises an AssertionError because 'a' and 'b' are not defined.\n",
                 "except(AssertionError):\n",
                 "    print('AssertionError encountered.')"
             ]
         },
@@ -244,34 +220,26 @@
                 "### Complex Conjugation \n",
                 "\n",
                 "Complex conjugation of variables is accomplished via trailing underscore in the variable name."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": null,
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2020-06-13T00:06:10.893232Z",
                     "start_time": "2020-06-13T00:06:10.554Z"
                 },
                 "run_control": {
                     "frozen": false,
                     "read_only": false
                 }
             },
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "{'x': (1+1j), 'y': (1-1j)}\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "data = {'x': 1.0+1.0j, 'y_': 1.0+1.0j}\n",
                 "ls = linsolve.LinearSolver(data)\n",
                 "sol = ls.solve()\n",
                 "print(sol)"
             ]
         },
@@ -287,34 +255,26 @@
                 "### Weights\n",
                 "\n",
                 "When a system of equations is overdetermined (as is usually the case in data analysis), `linsolve` lets you apply different weights to each equation. The default behavior is to weight all equations equally."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": null,
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2020-06-13T00:06:10.893948Z",
                     "start_time": "2020-06-13T00:06:10.557Z"
                 },
                 "run_control": {
                     "frozen": false,
                     "read_only": false
                 }
             },
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "{'x': 1.5}\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "data = {'1*x': 2.0, 'x': 1.0}\n",
                 "ls = linsolve.LinearSolver(data)\n",
                 "sol = ls.solve()\n",
                 "print(sol)"
             ]
         },
@@ -328,34 +288,26 @@
             },
             "source": [
                 "However, you can provide weights through the `wgts` keyword argument. Weights are multiplied by the data, so in standard inverse covariance weighting they can be thought of as $1/\\sigma^2$ where $\\sigma$ is the noise on that equation."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": null,
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2020-06-13T00:06:10.894732Z",
                     "start_time": "2020-06-13T00:06:10.559Z"
                 },
                 "run_control": {
                     "frozen": false,
                     "read_only": false
                 }
             },
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "{'x': 1.6666667106324469}\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "data = {'1*x': 2.0, 'x': 1.0}\n",
                 "wgts = {'1*x': 1.0, 'x': .5}\n",
                 "ls = linsolve.LinearSolver(data, wgts=wgts)\n",
                 "sol = ls.solve()\n",
                 "print(sol)"
             ]
@@ -374,34 +326,26 @@
                 "$\\chi^2 = \\sum_i \\frac{(d_i - m_i)^2}{\\sigma_i^2} = \\sum_i W_i^2 (d_i - m_i)^2$\n",
                 "\n",
                 "where $i$ indexes over equations, $d_i$ is the data (RHS), $m_i$ is the model (LHS evaluated at `sol`), and $W_i$ are the weights. We can calculate $\\chi^2$ with this handy function:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": null,
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2020-06-13T00:06:10.895376Z",
                     "start_time": "2020-06-13T00:06:10.561Z"
                 },
                 "run_control": {
                     "frozen": false,
                     "read_only": false
                 }
             },
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "0.33333333333333626\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "print(ls.chisq(sol))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
@@ -444,34 +388,26 @@
                 "`LogProductSolver` can tackle a special class of non-linear equations where all expressions are products. For example, we can solve\n",
                 "\n",
                 "$ab = 2 \\\\ bc = 1 \\\\ ac = 2$"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": null,
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2020-06-13T00:06:10.896074Z",
                     "start_time": "2020-06-13T00:06:10.562Z"
                 },
                 "run_control": {
                     "frozen": false,
                     "read_only": false
                 }
             },
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "{'a': 2.0, 'b': 1.0, 'c': 1.0}\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "data = {'a*b': 2.0, 'b*c': 1.0, 'a*c': 2.0}\n",
                 "lps = linsolve.LogProductSolver(data)\n",
                 "sol = lps.solve()\n",
                 "print(sol)"
             ]
         },
@@ -510,34 +446,26 @@
                 "$10(a_0+\\Delta a)(b_0+\\Delta b) + 3(b_0 + \\Delta b)(c_0 + \\Delta c) - 2(a_0 + \\Delta a)(c_0 + \\Delta c) = 32 \\\\ 10a\\Delta b + 10b\\Delta a + 3b\\Delta c + 3c \\Delta b - 2a\\Delta c - 2c\\Delta a + \\mathcal{O}(\\Delta^2) = 32 - 10a_0b_0 + 3b_0c_0 - 2a_0c_0$ \n",
                 "\n",
                 "`LinProductSolver` then solves for all the $\\Delta$ terms and updates `sol0` to `sol` accordingly. Just as with `LinearSolver`, `LinProductSolver` can take array systems, constants passed as keyword arguments, complex conjugated variables, and equation weighting."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": null,
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2020-06-13T00:06:10.896715Z",
                     "start_time": "2020-06-13T00:06:10.567Z"
                 },
                 "run_control": {
                     "frozen": false,
                     "read_only": false
                 }
             },
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "{'a': 0.9999999999972942, 'b': 2.0000000000014553, 'c': 2.9999999999999547}\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "data = {'10*a*b + 3*b*c - 2*a*c': 32, \n",
                 "        '2*a*a +3*b*b -2*c*c': -4,\n",
                 "        '-a*a + 2*b*c + a*c': 14}\n",
                 "sol0 = {'a': .9, 'b': 2.1, 'c': 3.2}\n",
                 "lps = linsolve.LinProductSolver(data, sol0)\n",
                 "meta, sol = lps.solve_iteratively()\n",
@@ -558,34 +486,26 @@
                 "* `conv_crit`: A convergence criterion (default `1e-10`) below which to stop iterating. Converegence is measured $\\ell^2$-norm of the change in the solution of all the variables since the previous iteration divided by the $\\ell^2$-norm of the solution itself.\n",
                 "* `chisq`: $\\chi^2$ as calculated above for the final iteration\n",
                 "* `iter`: the number of iterations ran. The iterative solver runs until until either convergence or `maxiter` is hit (default 50)."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": null,
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2020-06-13T00:06:10.897422Z",
                     "start_time": "2020-06-13T00:06:10.568Z"
                 },
                 "run_control": {
                     "frozen": false,
                     "read_only": false
                 }
             },
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "{'iter': 3, 'chisq': 8.199105284444733e-11, 'conv_crit': 3.7914394211356605e-07}\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "print(meta)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
@@ -613,15 +533,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.10"
+            "version": "3.7.6"
         },
         "toc": {
             "base_numbering": 1,
             "nav_menu": {},
             "number_sections": true,
             "sideBar": true,
             "skip_h1_title": false,
```

