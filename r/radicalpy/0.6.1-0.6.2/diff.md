# Comparing `tmp/radicalpy-0.6.1.tar.gz` & `tmp/radicalpy-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radicalpy-0.6.1.tar", last modified: Thu Jul 13 04:54:22 2023, max compression
+gzip compressed data, was "radicalpy-0.6.2.tar", last modified: Fri Jul 14 03:06:46 2023, max compression
```

## Comparing `radicalpy-0.6.1.tar` & `radicalpy-0.6.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 04:54:22.957596 radicalpy-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-07-13 04:54:12.000000 radicalpy-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-07-13 04:54:22.957596 radicalpy-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      772 2023-07-13 04:54:12.000000 radicalpy-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-07-13 04:54:12.000000 radicalpy-0.6.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 04:54:22.953596 radicalpy-0.6.1/radicalpy/
--rw-r--r--   0 runner    (1001) docker     (122)      311 2023-07-13 04:54:12.000000 radicalpy-0.6.1/radicalpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4924 2023-07-13 04:54:12.000000 radicalpy-0.6.1/radicalpy/classical.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 04:54:22.953596 radicalpy-0.6.1/radicalpy/data/
--rw-r--r--   0 runner    (1001) docker     (122)     2498 2023-07-13 04:54:12.000000 radicalpy-0.6.1/radicalpy/data/constants.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 04:54:22.957596 radicalpy-0.6.1/radicalpy/data/molecules/
--rw-r--r--   0 runner    (1001) docker     (122)      471 2023-07-13 04:54:12.000000 radicalpy-0.6.1/radicalpy/data/molecules/2_6_aqds.json
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-07-13 04:54:12.000000 radicalpy-0.6.1/radicalpy/data/molecules/adenine_cation.json
--rw-r--r--   0 runner    (1001) docker     (122)     6719 2023-07-13 04:54:12.000000 radicalpy-0.6.1/radicalpy/data/molecules/flavin_anion.json
--rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-07-13 04:54:12.000000 radicalpy-0.6.1/radicalpy/data/molecules/flavin_neutral.json
--rw-r--r--   0 runner    (1001) docker     (122)     3297 2023-07-13 04:54:12.000000 radicalpy-0.6.1/radicalpy/data/molecules/tryptophan_cation.json
--rw-r--r--   0 runner    (1001) docker     (122)     3293 2023-07-13 04:54:12.000000 radicalpy-0.6.1/radicalpy/data/molecules/tyrosine_neutral.json
--rw-r--r--   0 runner    (1001) docker     (122)    27847 2023-07-13 04:54:12.000000 radicalpy-0.6.1/radicalpy/data/spin_data.json
--rw-r--r--   0 runner    (1001) docker     (122)    16112 2023-07-13 04:54:12.000000 radicalpy-0.6.1/radicalpy/data.py
--rw-r--r--   0 runner    (1001) docker     (122)    20261 2023-07-13 04:54:12.000000 radicalpy-0.6.1/radicalpy/estimations.py
--rw-r--r--   0 runner    (1001) docker     (122)     5054 2023-07-13 04:54:12.000000 radicalpy-0.6.1/radicalpy/kinetics.py
--rw-r--r--   0 runner    (1001) docker     (122)     6252 2023-07-13 04:54:12.000000 radicalpy-0.6.1/radicalpy/plot.py
--rw-r--r--   0 runner    (1001) docker     (122)     9710 2023-07-13 04:54:12.000000 radicalpy-0.6.1/radicalpy/relaxation.py
--rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-07-13 04:54:12.000000 radicalpy-0.6.1/radicalpy/shared.py
--rw-r--r--   0 runner    (1001) docker     (122)    25084 2023-07-13 04:54:12.000000 radicalpy-0.6.1/radicalpy/simulation.py
--rw-r--r--   0 runner    (1001) docker     (122)    11422 2023-07-13 04:54:12.000000 radicalpy-0.6.1/radicalpy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 04:54:22.953596 radicalpy-0.6.1/radicalpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-07-13 04:54:22.000000 radicalpy-0.6.1/radicalpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      872 2023-07-13 04:54:22.000000 radicalpy-0.6.1/radicalpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-13 04:54:22.000000 radicalpy-0.6.1/radicalpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-07-13 04:54:22.000000 radicalpy-0.6.1/radicalpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-13 04:54:22.000000 radicalpy-0.6.1/radicalpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-07-13 04:54:12.000000 radicalpy-0.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-13 04:54:22.957596 radicalpy-0.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 04:54:22.957596 radicalpy-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     3157 2023-07-13 04:54:12.000000 radicalpy-0.6.1/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     3948 2023-07-13 04:54:12.000000 radicalpy-0.6.1/tests/test_estimations.py
--rw-r--r--   0 runner    (1001) docker     (122)      325 2023-07-13 04:54:12.000000 radicalpy-0.6.1/tests/test_relaxations.py
--rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-07-13 04:54:12.000000 radicalpy-0.6.1/tests/test_shared.py
--rw-r--r--   0 runner    (1001) docker     (122)    19571 2023-07-13 04:54:12.000000 radicalpy-0.6.1/tests/test_simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 03:06:46.491118 radicalpy-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-07-14 03:06:37.000000 radicalpy-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-07-14 03:06:46.491118 radicalpy-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      772 2023-07-14 03:06:37.000000 radicalpy-0.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-07-14 03:06:37.000000 radicalpy-0.6.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 03:06:46.487118 radicalpy-0.6.2/radicalpy/
+-rw-r--r--   0 runner    (1001) docker     (122)      311 2023-07-14 03:06:37.000000 radicalpy-0.6.2/radicalpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4924 2023-07-14 03:06:37.000000 radicalpy-0.6.2/radicalpy/classical.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 03:06:46.491118 radicalpy-0.6.2/radicalpy/data/
+-rw-r--r--   0 runner    (1001) docker     (122)     2498 2023-07-14 03:06:37.000000 radicalpy-0.6.2/radicalpy/data/constants.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 03:06:46.491118 radicalpy-0.6.2/radicalpy/data/molecules/
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-07-14 03:06:37.000000 radicalpy-0.6.2/radicalpy/data/molecules/2_6_aqds.json
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-07-14 03:06:37.000000 radicalpy-0.6.2/radicalpy/data/molecules/adenine_cation.json
+-rw-r--r--   0 runner    (1001) docker     (122)     6719 2023-07-14 03:06:37.000000 radicalpy-0.6.2/radicalpy/data/molecules/flavin_anion.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-07-14 03:06:37.000000 radicalpy-0.6.2/radicalpy/data/molecules/flavin_neutral.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3297 2023-07-14 03:06:37.000000 radicalpy-0.6.2/radicalpy/data/molecules/tryptophan_cation.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3293 2023-07-14 03:06:37.000000 radicalpy-0.6.2/radicalpy/data/molecules/tyrosine_neutral.json
+-rw-r--r--   0 runner    (1001) docker     (122)    27847 2023-07-14 03:06:37.000000 radicalpy-0.6.2/radicalpy/data/spin_data.json
+-rw-r--r--   0 runner    (1001) docker     (122)    16112 2023-07-14 03:06:37.000000 radicalpy-0.6.2/radicalpy/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20209 2023-07-14 03:06:37.000000 radicalpy-0.6.2/radicalpy/estimations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5054 2023-07-14 03:06:37.000000 radicalpy-0.6.2/radicalpy/kinetics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6365 2023-07-14 03:06:37.000000 radicalpy-0.6.2/radicalpy/plot.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9710 2023-07-14 03:06:37.000000 radicalpy-0.6.2/radicalpy/relaxation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-07-14 03:06:37.000000 radicalpy-0.6.2/radicalpy/shared.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25118 2023-07-14 03:06:37.000000 radicalpy-0.6.2/radicalpy/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11422 2023-07-14 03:06:37.000000 radicalpy-0.6.2/radicalpy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 03:06:46.491118 radicalpy-0.6.2/radicalpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-07-14 03:06:46.000000 radicalpy-0.6.2/radicalpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      872 2023-07-14 03:06:46.000000 radicalpy-0.6.2/radicalpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-14 03:06:46.000000 radicalpy-0.6.2/radicalpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-07-14 03:06:46.000000 radicalpy-0.6.2/radicalpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-14 03:06:46.000000 radicalpy-0.6.2/radicalpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-07-14 03:06:37.000000 radicalpy-0.6.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-14 03:06:46.491118 radicalpy-0.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 03:06:46.491118 radicalpy-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     3157 2023-07-14 03:06:37.000000 radicalpy-0.6.2/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3948 2023-07-14 03:06:37.000000 radicalpy-0.6.2/tests/test_estimations.py
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2023-07-14 03:06:37.000000 radicalpy-0.6.2/tests/test_relaxations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-07-14 03:06:37.000000 radicalpy-0.6.2/tests/test_shared.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19571 2023-07-14 03:06:37.000000 radicalpy-0.6.2/tests/test_simulation.py
```

### Comparing `radicalpy-0.6.1/LICENSE` & `radicalpy-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.1/PKG-INFO` & `radicalpy-0.6.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radicalpy
-Version: 0.6.1
+Version: 0.6.2
 Summary: RadicalPy: a toolbox for radical pair spin dynamics
 Author-email: "Lewis M. Antill" <lewismantill@gmail.com>, Emil Vatai <emil.vatai@gmail.com>
 Maintainer-email: Emil Vatai <emil.vatai@gmail.com>, "Lewis M. Antill" <lewismantill@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Spin-Chemistry-Labs/radicalpy
 Project-URL: Documentation, https://radicalpy.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/Spin-Chemistry-Labs/radicalpy
```

### Comparing `radicalpy-0.6.1/README.md` & `radicalpy-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.1/pyproject.toml` & `radicalpy-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.1/radicalpy/classical.py` & `radicalpy-0.6.2/radicalpy/classical.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.1/radicalpy/data/constants.json` & `radicalpy-0.6.2/radicalpy/data/constants.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.1/radicalpy/data/molecules/flavin_anion.json` & `radicalpy-0.6.2/radicalpy/data/molecules/flavin_anion.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.1/radicalpy/data/molecules/flavin_neutral.json` & `radicalpy-0.6.2/radicalpy/data/molecules/flavin_neutral.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.1/radicalpy/data/molecules/tryptophan_cation.json` & `radicalpy-0.6.2/radicalpy/data/molecules/tryptophan_cation.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.1/radicalpy/data/molecules/tyrosine_neutral.json` & `radicalpy-0.6.2/radicalpy/data/molecules/tyrosine_neutral.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.1/radicalpy/data/spin_data.json` & `radicalpy-0.6.2/radicalpy/data/spin_data.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.1/radicalpy/data.py` & `radicalpy-0.6.2/radicalpy/data.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.1/radicalpy/estimations.py` & `radicalpy-0.6.2/radicalpy/estimations.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,30 +236,28 @@
        https://doi.org/10.1021/jp0456943
     .. _Miura et al. J. Phys. Chem. A, 119, 22, 5534-5544 (2015):
        https://doi.org/10.1021/acs.jpca.5b02183
     """
     return dipolar_interaction_isotropic(r) * (3 * np.cos(theta) ** 2 - 1)
 
 
-def dipolar_interaction_anisotropic(
-    r: float | np.ndarray, gamma: float = Isotope("E").gamma_mT
-) -> np.ndarray:
+def dipolar_interaction_anisotropic(r: float | np.ndarray) -> np.ndarray:
     """Anisotropic dipolar coupling.
 
     Point dipole approximation is used.
 
     Args:
             r (float or np.ndarray): The interradical separation (m).
 
     Returns:
             np.ndarray: The dipolar coupling tensor in millitesla (mT).
     .. todo:: np.ndarray not implemented.  `dipolar * diag` fails.
     """
     dipolar1d = dipolar_interaction_isotropic(r)
-    dipolar = gamma * (2 / 3) * dipolar1d
+    dipolar = (2 / 3) * dipolar1d
     return dipolar * np.diag([-1, -1, 2])
 
 
 def dipolar_interaction_isotropic(r: float | np.ndarray) -> float | np.ndarray:
     """Isotropic dipolar coupling.
 
     Point dipole approximation is used.
```

### Comparing `radicalpy-0.6.1/radicalpy/kinetics.py` & `radicalpy-0.6.2/radicalpy/kinetics.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.1/radicalpy/plot.py` & `radicalpy-0.6.2/radicalpy/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,17 @@
     ax.set_ylabel("Spin state energy (J)", size=14)
     plt.tick_params(labelsize=14)
 
 
 def energy_levels(sim: HilbertSimulation, B: np.ndarray, J=0, D=0):
     # TODO(VATAI): DO THIS PROPERLY
     # TODO(VATAI): use tick labels
+    assert (
+        type(sim) == HilbertSimulation
+    ), "plot.energy_levels assumes Hilbert space simulation"
     H_base = sim.total_hamiltonian(0, J, D)
     H_zee = sim.zeeman_hamiltonian(1)
 
     E = np.zeros([len(B), len(H_base)], dtype=np.complex_)
 
     for i, B0 in enumerate(B):
         H = H_base + B0 * H_zee
```

### Comparing `radicalpy-0.6.1/radicalpy/relaxation.py` & `radicalpy-0.6.2/radicalpy/relaxation.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.1/radicalpy/shared.py` & `radicalpy-0.6.2/radicalpy/shared.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.1/radicalpy/simulation.py` & `radicalpy-0.6.2/radicalpy/simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 
 import enum
+import itertools
 from math import prod
-from typing import Iterable, Optional
+from typing import Optional
 
 import numpy as np
 import scipy as sp
 from tqdm import tqdm
 
 from . import utils
 from .data import Molecule
@@ -571,19 +572,19 @@
         H_base: np.ndarray,
         theta: list[float],
         phi: list[float],
     ):
         shape = self._get_rho_shape(H_base.shape[0])
         rhos = np.zeros((len(theta), len(phi), len(time), *shape), dtype=complex)
 
-        for i, th in enumerate(theta):
-            for j, ph in enumerate(phi):
-                H_zee = self.zeeman_hamiltonian(B, th, ph)
-                H = H_base + self.convert(H_zee)
-                rhos[i, j] = self.time_evolution(init_state, time, H)
+        iters = itertools.product(enumerate(theta), enumerate(phi))
+        for (i, th), (j, ph) in tqdm(list(iters)):
+            H_zee = self.zeeman_hamiltonian(B, th, ph)
+            H = H_base + self.convert(H_zee)
+            rhos[i, j] = self.time_evolution(init_state, time, H)
         return rhos
 
     def anisotropy(
         self,
         init_state: State,
         obs_state: State,
         time: np.ndarray,
```

### Comparing `radicalpy-0.6.1/radicalpy/utils.py` & `radicalpy-0.6.2/radicalpy/utils.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.1/radicalpy.egg-info/PKG-INFO` & `radicalpy-0.6.2/radicalpy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radicalpy
-Version: 0.6.1
+Version: 0.6.2
 Summary: RadicalPy: a toolbox for radical pair spin dynamics
 Author-email: "Lewis M. Antill" <lewismantill@gmail.com>, Emil Vatai <emil.vatai@gmail.com>
 Maintainer-email: Emil Vatai <emil.vatai@gmail.com>, "Lewis M. Antill" <lewismantill@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Spin-Chemistry-Labs/radicalpy
 Project-URL: Documentation, https://radicalpy.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/Spin-Chemistry-Labs/radicalpy
```

### Comparing `radicalpy-0.6.1/radicalpy.egg-info/SOURCES.txt` & `radicalpy-0.6.2/radicalpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.1/tests/test_data.py` & `radicalpy-0.6.2/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.1/tests/test_estimations.py` & `radicalpy-0.6.2/tests/test_estimations.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.1/tests/test_shared.py` & `radicalpy-0.6.2/tests/test_shared.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.1/tests/test_simulation.py` & `radicalpy-0.6.2/tests/test_simulation.py`

 * *Files identical despite different names*

