# Comparing `tmp/qubolite-0.8.tar.gz` & `tmp/qubolite-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qubolite-0.8.tar", last modified: Thu Jul 13 13:34:23 2023, max compression
+gzip compressed data, was "qubolite-0.8.1.tar", last modified: Fri Jul 14 09:33:44 2023, max compression
```

## Comparing `qubolite-0.8.tar` & `qubolite-0.8.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 smuecke   (1000) smuecke   (1000)        0 2023-07-13 13:34:23.548317 qubolite-0.8/
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)     5231 2023-07-13 13:34:23.548317 qubolite-0.8/PKG-INFO
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)     4722 2023-07-13 08:34:09.000000 qubolite-0.8/README.md
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)      850 2023-07-13 08:34:09.000000 qubolite-0.8/pyproject.toml
-drwxr-xr-x   0 smuecke   (1000) smuecke   (1000)        0 2023-07-13 13:34:23.548317 qubolite-0.8/qubolite/
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)      205 2023-07-13 11:56:09.000000 qubolite-0.8/qubolite/__init__.py
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)     5873 2023-07-13 08:34:09.000000 qubolite-0.8/qubolite/_c_utils.c
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)    10472 2023-07-13 08:34:09.000000 qubolite-0.8/qubolite/_heuristics.py
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)     2487 2023-07-13 08:34:09.000000 qubolite-0.8/qubolite/_misc.py
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)     6153 2023-07-13 08:49:00.000000 qubolite-0.8/qubolite/bitvec.py
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)     4689 2023-07-13 12:40:40.000000 qubolite-0.8/qubolite/bounds.py
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)     9413 2023-07-13 08:34:09.000000 qubolite-0.8/qubolite/compression.py
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)     8161 2023-07-13 12:23:13.000000 qubolite-0.8/qubolite/embedding.py
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)    21656 2023-07-13 12:48:30.000000 qubolite-0.8/qubolite/qubo.py
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)    11257 2023-07-13 08:34:09.000000 qubolite-0.8/qubolite/sampling.py
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)     6740 2023-07-13 12:48:17.000000 qubolite-0.8/qubolite/solving.py
-drwxr-xr-x   0 smuecke   (1000) smuecke   (1000)        0 2023-07-13 13:34:23.548317 qubolite-0.8/qubolite.egg-info/
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)     5231 2023-07-13 13:34:23.000000 qubolite-0.8/qubolite.egg-info/PKG-INFO
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)      417 2023-07-13 13:34:23.000000 qubolite-0.8/qubolite.egg-info/SOURCES.txt
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)        1 2023-07-13 13:34:23.000000 qubolite-0.8/qubolite.egg-info/dependency_links.txt
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)      185 2023-07-13 13:34:23.000000 qubolite-0.8/qubolite.egg-info/requires.txt
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)       18 2023-07-13 13:34:23.000000 qubolite-0.8/qubolite.egg-info/top_level.txt
--rw-r--r--   0 smuecke   (1000) smuecke   (1000)       38 2023-07-13 13:34:23.548317 qubolite-0.8/setup.cfg
--rwxr-xr-x   0 smuecke   (1000) smuecke   (1000)      836 2023-07-13 08:34:09.000000 qubolite-0.8/setup.py
+drwxr-xr-x   0 smuecke   (1000) smuecke   (1000)        0 2023-07-14 09:33:44.595992 qubolite-0.8.1/
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)     5369 2023-07-14 09:33:44.595992 qubolite-0.8.1/PKG-INFO
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)     4795 2023-07-14 09:31:22.000000 qubolite-0.8.1/README.md
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)      907 2023-07-14 09:30:45.000000 qubolite-0.8.1/pyproject.toml
+drwxr-xr-x   0 smuecke   (1000) smuecke   (1000)        0 2023-07-14 09:33:44.595992 qubolite-0.8.1/qubolite/
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)      205 2023-07-12 14:20:19.000000 qubolite-0.8.1/qubolite/__init__.py
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)     5873 2023-07-12 14:20:19.000000 qubolite-0.8.1/qubolite/_c_utils.c
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)    10472 2023-07-12 14:20:19.000000 qubolite-0.8.1/qubolite/_heuristics.py
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)     2487 2023-07-12 14:20:19.000000 qubolite-0.8.1/qubolite/_misc.py
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)     6139 2023-07-14 08:43:25.000000 qubolite-0.8.1/qubolite/bitvec.py
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)     4689 2023-07-14 08:43:25.000000 qubolite-0.8.1/qubolite/bounds.py
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)     9413 2023-07-12 14:20:19.000000 qubolite-0.8.1/qubolite/compression.py
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)     8161 2023-07-14 08:43:25.000000 qubolite-0.8.1/qubolite/embedding.py
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)    22037 2023-07-14 09:14:59.000000 qubolite-0.8.1/qubolite/qubo.py
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)    11257 2023-07-12 14:20:19.000000 qubolite-0.8.1/qubolite/sampling.py
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)     6590 2023-07-14 08:43:25.000000 qubolite-0.8.1/qubolite/solving.py
+drwxr-xr-x   0 smuecke   (1000) smuecke   (1000)        0 2023-07-14 09:33:44.595992 qubolite-0.8.1/qubolite.egg-info/
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)     5369 2023-07-14 09:33:44.000000 qubolite-0.8.1/qubolite.egg-info/PKG-INFO
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)      417 2023-07-14 09:33:44.000000 qubolite-0.8.1/qubolite.egg-info/SOURCES.txt
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)        1 2023-07-14 09:33:44.000000 qubolite-0.8.1/qubolite.egg-info/dependency_links.txt
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)      185 2023-07-14 09:33:44.000000 qubolite-0.8.1/qubolite.egg-info/requires.txt
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)       18 2023-07-14 09:33:44.000000 qubolite-0.8.1/qubolite.egg-info/top_level.txt
+-rw-r--r--   0 smuecke   (1000) smuecke   (1000)       38 2023-07-14 09:33:44.595992 qubolite-0.8.1/setup.cfg
+-rwxr-xr-x   0 smuecke   (1000) smuecke   (1000)      836 2023-07-12 13:34:37.000000 qubolite-0.8.1/setup.py
```

### Comparing `qubolite-0.8/PKG-INFO` & `qubolite-0.8.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: qubolite
-Version: 0.8
+Version: 0.8.1
 Summary: Toolbox for quadratic binary optimization
 Author-email: Sascha Mücke <sascha.muecke@tu-dortmund.de>, Thore Gerlach <thore.gerlach@iais.fraunhofer.de>
 Project-URL: Homepage, https://github.com/smuecke/qubolite
+Project-URL: Documentation, https://smuecke.github.io/qubolite
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: roof_dual
 Provides-Extra: kendall_tau
 Provides-Extra: embedding
 Provides-Extra: compression
@@ -91,15 +92,15 @@
 ```
 
 The method `brute_force` is implemented efficiently in C and parallelized with OpenMP.
 Still, for instances with more than 30 variables take a long time to solve this way.
 
 ## Documentation
 
-The complete API documentation can be found [here](https://smuecke.github.com/qubolite).
+The complete API documentation can be found [here](https://smuecke.github.io/qubolite/api.html).
 
 ## Version Log
 
 * **0.2** Added problem embeddings (binary clustering, subset sum problem)
 * **0.3** Added `QUBOSample` class and sampling methods `full` and `gibbs`
 * **0.4** Renamed `QUBOSample` to `BinarySample`; added methods for saving and loading QUBO and Sample instances
 * **0.5** Moved `gibbs` to `mcmc` and implemented true Gibbs sampling as `gibbs`; added `numba` as dependency
@@ -112,8 +113,9 @@
     * **0.6.5** complete empirical prob. vector can be returned from `BinarySample`
     * **0.6.6** fixed spectral gap implementation
     * **0.6.7** moved `brute_force` to new sub-module `solving`; added some approximate solving methods
     * **0.6.8** added `bitvec` sub-module; `dynamic_range` now uses bits by default, changed `bits=False` to `decibel=False`; removed scipy from requirements
     * **0.6.9** new, more memory-efficient save format
     * **0.6.10** fixed requirements in `setup.py`; fixed size estimation in `qubo.save()`
 * **0.7** Added more efficient brute-force implementation using C extension; added optional dependencies for calculating bounds and ordering distance
-* **0.8** New embeddings, new solving methods; switched to NumPy random generators from `RandomState`; added parameter compression for dynamic range reduction
+* **0.8** New embeddings, new solving methods; switched to NumPy random generators from `RandomState`; added parameter compression for dynamic range reduction; Added documentation
+    * **0.8.1** some fixes to documentation
```

### Comparing `qubolite-0.8/README.md` & `qubolite-0.8.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 ```
 
 The method `brute_force` is implemented efficiently in C and parallelized with OpenMP.
 Still, for instances with more than 30 variables take a long time to solve this way.
 
 ## Documentation
 
-The complete API documentation can be found [here](https://smuecke.github.com/qubolite).
+The complete API documentation can be found [here](https://smuecke.github.io/qubolite/api.html).
 
 ## Version Log
 
 * **0.2** Added problem embeddings (binary clustering, subset sum problem)
 * **0.3** Added `QUBOSample` class and sampling methods `full` and `gibbs`
 * **0.4** Renamed `QUBOSample` to `BinarySample`; added methods for saving and loading QUBO and Sample instances
 * **0.5** Moved `gibbs` to `mcmc` and implemented true Gibbs sampling as `gibbs`; added `numba` as dependency
@@ -97,8 +97,9 @@
     * **0.6.5** complete empirical prob. vector can be returned from `BinarySample`
     * **0.6.6** fixed spectral gap implementation
     * **0.6.7** moved `brute_force` to new sub-module `solving`; added some approximate solving methods
     * **0.6.8** added `bitvec` sub-module; `dynamic_range` now uses bits by default, changed `bits=False` to `decibel=False`; removed scipy from requirements
     * **0.6.9** new, more memory-efficient save format
     * **0.6.10** fixed requirements in `setup.py`; fixed size estimation in `qubo.save()`
 * **0.7** Added more efficient brute-force implementation using C extension; added optional dependencies for calculating bounds and ordering distance
-* **0.8** New embeddings, new solving methods; switched to NumPy random generators from `RandomState`; added parameter compression for dynamic range reduction
+* **0.8** New embeddings, new solving methods; switched to NumPy random generators from `RandomState`; added parameter compression for dynamic range reduction; Added documentation
+    * **0.8.1** some fixes to documentation
```

### Comparing `qubolite-0.8/pyproject.toml` & `qubolite-0.8.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61.0",
     "numpy>=1.23.5"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qubolite"
-version = "0.8"
+version = "0.8.1"
 authors = [
     { name = "Sascha Mücke", email="sascha.muecke@tu-dortmund.de" },
     { name = "Thore Gerlach", email="thore.gerlach@iais.fraunhofer.de" }
 ]
 description = "Toolbox for quadratic binary optimization"
 readme = "README.md"
 requires-python = ">=3.8"
@@ -20,14 +20,15 @@
 ]
 dependencies = [
     "numpy>=1.23.5"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/smuecke/qubolite"
+"Documentation" = "https://smuecke.github.io/qubolite"
 
 [project.optional-dependencies]
 roof_dual = [
     "igraph>=0.10.4"
 ]
 kendall_tau = [
     "scipy>=1.10.1"
```

### Comparing `qubolite-0.8/qubolite/_c_utils.c` & `qubolite-0.8.1/qubolite/_c_utils.c`

 * *Files identical despite different names*

### Comparing `qubolite-0.8/qubolite/_heuristics.py` & `qubolite-0.8.1/qubolite/_heuristics.py`

 * *Files identical despite different names*

### Comparing `qubolite-0.8/qubolite/_misc.py` & `qubolite-0.8.1/qubolite/_misc.py`

 * *Files identical despite different names*

### Comparing `qubolite-0.8/qubolite/bitvec.py` & `qubolite-0.8.1/qubolite/bitvec.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,21 +150,18 @@
             # check if constant needs to be inverted
         i += 1
     return tokens
 
 def from_expression(expr: str):
     """Generate an array of bit vectors from a string
     containing a bit vector expression. Such an expression
-    consists of a sequence of these symbols::
-
-        0     a constant 0
-        1     a constant 1
-        *     all combinations of 0 and 1
-        [i]   the same as the bit at index i
-        [!i]  the inverse of the bit at index i
+    consists of a sequence of these symbols: ``0`` - a constant 0,
+    ``1`` - a constant 1, ``*`` - all combinations of 0 and 1,
+    ``[i]`` - the same as the bit at index i, ``[!i]`` -  the
+    inverse of the bit at index i.
 
     The last two symbols are called references, and ``i`` their
     pointing index (counting from 0). A reference can only ever
     point to a constant or ``*``, i.e., higher-order references are
     not allowed (and not necessary).
 
     Args:
@@ -180,15 +177,14 @@
         the same" can be expressed as
 
         >>> from_expression('1**[2]')
         array([[1., 0., 0., 0.],
         ...    [1., 1., 0., 0.],
         ...    [1., 0., 1., 1.],
         ...    [1., 1., 1., 1.]])
-    
     """
     tokens = _expr_normal_form(list(_BITVEC_EXPR.findall(expr)))
     n = len(tokens)
     n_free = expr.count('*')
     x = np.empty((1<<n_free, n))
     power = 0
     for i, token in enumerate(tokens):
```

### Comparing `qubolite-0.8/qubolite/bounds.py` & `qubolite-0.8.1/qubolite/bounds.py`

 * *Files identical despite different names*

### Comparing `qubolite-0.8/qubolite/compression.py` & `qubolite-0.8.1/qubolite/compression.py`

 * *Files identical despite different names*

### Comparing `qubolite-0.8/qubolite/embedding.py` & `qubolite-0.8.1/qubolite/embedding.py`

 * *Files identical despite different names*

### Comparing `qubolite-0.8/qubolite/qubo.py` & `qubolite-0.8.1/qubolite/qubo.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 import struct
 from functools import reduce
 
 import numpy as np
 
 from .bitvec  import all_bitvectors, all_bitvectors_array
 from ._misc    import get_random_state, is_triu, warn_size
-
-try:
-    # catch import error, so that sphinx's autodoc works
-    # without compiling C sources.
-    from _c_utils import brute_force as _brute_force_c
-except ImportError as e:
-    _brute_force_c = e
+from _c_utils import brute_force as _brute_force_c
 
 def is_qubo_like(arr):
     """Check if given array defines a QUBO instance, i.e.,
     if the array is 2-dimensional and square.
 
     Args:
         arr (numpy.ndarray): Input array.
@@ -306,14 +300,26 @@
                     i, = k
                     m[names[i], names[i]] += v
                 except ValueError:
                     pass
         m = np.triu(m + np.tril(m, -1).T)
         return cls(m), { i: k for k, i in names.items() }
 
+    @classmethod
+    def from_ising(cls, linear, quadratic, offset=0.0):
+        lin = np.asarray(linear)
+        qua = np.asarray(quadratic)
+        n, = lin.shape
+        assert qua.shape == (n, n), '`linear` and `quadratic` must have shapes (n,) and (n, n)'
+        qua_symm = np.tril(qua, -1).T + np.triu(qua, 1) + qua
+        m  = 2*np.diag(qua.sum(0)+lin)
+        m -= 4*np.triu(qua_symm, 1)
+        return cls(m)
+
+
     def spectral_gap(self, return_optimum=False):
         """Calculate the spectral gap of this QUBO instance.
         Here, this is defined as the difference between the lowest and second-to lowest QUBO energy value across all bit vectors.
         Note that the QUBO instance must be solved for calculating this value, therefore only QUBOs of sizes up to about 30 are feasible in practice.
         
         Args:
             return_optimum (bool, optional): If ``True``, returns the minimizing bit vector of this QUBO instance (which is calculated anyway). Defaults to False.
@@ -333,18 +339,22 @@
         sgap = v1-v0
         if return_optimum:
             return sgap, x
         else:
             return sgap
 
     def clamp(self, partial_assignment=None):
-        """Create QUBO instance equivalent to this but with a subset of parameters fixed (_clamped_) to constant values.
+        """Create QUBO instance equivalent to this but with a subset
+        of variables fixed (_clamped_) to constant values.
 
         Args:
-            partial_assignment (dict, optional): Dictionary mapping variable indices (counting from 0) to constant values 0 or 1. Defaults to None, which does nothing and returns a copy of this QUBO instance.
+            partial_assignment (dict, optional): Dictionary mapping
+                variable indices (counting from 0) to constant values
+                0 or 1. Defaults to None, which does nothing and
+                returns a copy of this QUBO instance.
 
         Returns:
             qubo: Clamped QUBO instance.
             const (float): Constant offset value, which must be added to the QUBO energy to obtain the original energy.
             free (list): List of indices which the variable indices of the new QUBO instance correspond to (i.e., those indices that were not clamped).
         """
         if partial_assignment is None:
@@ -528,7 +538,10 @@
         posiform[0][diag_ix] = lin + qua_neg.sum(1)
         lin_ = posiform[0][diag_ix].copy()  # =: c'
         lin_neg = np.minimum(lin_, 0)
         posiform[1][diag_ix] = -lin_neg
         posiform[0][diag_ix] = np.maximum(lin_, 0)
         const = lin_neg.sum()
         return posiform, const
+
+    def to_ising(self):
+        return NotImplemented
```

### Comparing `qubolite-0.8/qubolite/sampling.py` & `qubolite-0.8.1/qubolite/sampling.py`

 * *Files identical despite different names*

### Comparing `qubolite-0.8/qubolite/solving.py` & `qubolite-0.8.1/qubolite/solving.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,12 @@
 import numpy as np
 
 from ._misc import get_random_state, warn_size
 from .qubo import qubo
-
-try:
-    # catch import error, so that sphinx's autodoc works
-    # without compiling C sources.
-    from _c_utils import brute_force as _brute_force_c
-except ImportError as e:
-    _brute_force_c = e
+from _c_utils import brute_force as _brute_force_c
 
 
 def brute_force(Q: qubo):
     """Solve QUBO instance exactly by brute force.
     Note that this method is infeasible for instances
     with a size beyond around 30.
```

### Comparing `qubolite-0.8/qubolite.egg-info/PKG-INFO` & `qubolite-0.8.1/qubolite.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: qubolite
-Version: 0.8
+Version: 0.8.1
 Summary: Toolbox for quadratic binary optimization
 Author-email: Sascha Mücke <sascha.muecke@tu-dortmund.de>, Thore Gerlach <thore.gerlach@iais.fraunhofer.de>
 Project-URL: Homepage, https://github.com/smuecke/qubolite
+Project-URL: Documentation, https://smuecke.github.io/qubolite
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: roof_dual
 Provides-Extra: kendall_tau
 Provides-Extra: embedding
 Provides-Extra: compression
@@ -91,15 +92,15 @@
 ```
 
 The method `brute_force` is implemented efficiently in C and parallelized with OpenMP.
 Still, for instances with more than 30 variables take a long time to solve this way.
 
 ## Documentation
 
-The complete API documentation can be found [here](https://smuecke.github.com/qubolite).
+The complete API documentation can be found [here](https://smuecke.github.io/qubolite/api.html).
 
 ## Version Log
 
 * **0.2** Added problem embeddings (binary clustering, subset sum problem)
 * **0.3** Added `QUBOSample` class and sampling methods `full` and `gibbs`
 * **0.4** Renamed `QUBOSample` to `BinarySample`; added methods for saving and loading QUBO and Sample instances
 * **0.5** Moved `gibbs` to `mcmc` and implemented true Gibbs sampling as `gibbs`; added `numba` as dependency
@@ -112,8 +113,9 @@
     * **0.6.5** complete empirical prob. vector can be returned from `BinarySample`
     * **0.6.6** fixed spectral gap implementation
     * **0.6.7** moved `brute_force` to new sub-module `solving`; added some approximate solving methods
     * **0.6.8** added `bitvec` sub-module; `dynamic_range` now uses bits by default, changed `bits=False` to `decibel=False`; removed scipy from requirements
     * **0.6.9** new, more memory-efficient save format
     * **0.6.10** fixed requirements in `setup.py`; fixed size estimation in `qubo.save()`
 * **0.7** Added more efficient brute-force implementation using C extension; added optional dependencies for calculating bounds and ordering distance
-* **0.8** New embeddings, new solving methods; switched to NumPy random generators from `RandomState`; added parameter compression for dynamic range reduction
+* **0.8** New embeddings, new solving methods; switched to NumPy random generators from `RandomState`; added parameter compression for dynamic range reduction; Added documentation
+    * **0.8.1** some fixes to documentation
```

### Comparing `qubolite-0.8/setup.py` & `qubolite-0.8.1/setup.py`

 * *Files identical despite different names*

