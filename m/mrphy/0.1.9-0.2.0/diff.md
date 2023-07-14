# Comparing `tmp/mrphy-0.1.9.tar.gz` & `tmp/mrphy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrphy-0.1.9.tar", last modified: Mon Jun 21 15:50:26 2021, max compression
+gzip compressed data, was "mrphy-0.2.0.tar", last modified: Fri Jul 14 01:22:46 2023, max compression
```

## Comparing `mrphy-0.1.9.tar` & `mrphy-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 tluo      (1000) tluo      (1000)        0 2021-06-21 15:50:26.807002 mrphy-0.1.9/
--rw-r--r--   0 tluo      (1000) tluo      (1000)     3246 2021-06-21 15:50:26.807002 mrphy-0.1.9/PKG-INFO
--rw-r--r--   0 tluo      (1000) tluo      (1000)     2273 2021-06-21 15:44:15.000000 mrphy-0.1.9/README.md
-drwxr-xr-x   0 tluo      (1000) tluo      (1000)        0 2021-06-21 15:50:26.807002 mrphy-0.1.9/mrphy/
--rw-r--r--   0 tluo      (1000) tluo      (1000)     2346 2021-06-14 15:35:48.000000 mrphy-0.1.9/mrphy/__init__.py
--rw-r--r--   0 tluo      (1000) tluo      (1000)     5597 2021-06-21 15:44:15.000000 mrphy-0.1.9/mrphy/beffective.py
--rw-r--r--   0 tluo      (1000) tluo      (1000)    38202 2021-06-21 15:44:15.000000 mrphy-0.1.9/mrphy/mobjs.py
--rw-r--r--   0 tluo      (1000) tluo      (1000)    12432 2021-06-21 15:44:15.000000 mrphy-0.1.9/mrphy/sims.py
--rw-r--r--   0 tluo      (1000) tluo      (1000)     4103 2021-06-21 15:44:15.000000 mrphy-0.1.9/mrphy/slowsims.py
--rw-r--r--   0 tluo      (1000) tluo      (1000)     9204 2021-06-21 15:44:15.000000 mrphy-0.1.9/mrphy/utils.py
-drwxr-xr-x   0 tluo      (1000) tluo      (1000)        0 2021-06-21 15:50:26.807002 mrphy-0.1.9/mrphy.egg-info/
--rw-r--r--   0 tluo      (1000) tluo      (1000)     3246 2021-06-21 15:50:26.000000 mrphy-0.1.9/mrphy.egg-info/PKG-INFO
--rw-r--r--   0 tluo      (1000) tluo      (1000)      362 2021-06-21 15:50:26.000000 mrphy-0.1.9/mrphy.egg-info/SOURCES.txt
--rw-r--r--   0 tluo      (1000) tluo      (1000)        1 2021-06-21 15:50:26.000000 mrphy-0.1.9/mrphy.egg-info/dependency_links.txt
--rw-r--r--   0 tluo      (1000) tluo      (1000)       23 2021-06-21 15:50:26.000000 mrphy-0.1.9/mrphy.egg-info/requires.txt
--rw-r--r--   0 tluo      (1000) tluo      (1000)       12 2021-06-21 15:50:26.000000 mrphy-0.1.9/mrphy.egg-info/top_level.txt
--rw-r--r--   0 tluo      (1000) tluo      (1000)       38 2021-06-21 15:50:26.807002 mrphy-0.1.9/setup.cfg
--rw-r--r--   0 tluo      (1000) tluo      (1000)     1158 2021-06-21 15:44:15.000000 mrphy-0.1.9/setup.py
-drwxr-xr-x   0 tluo      (1000) tluo      (1000)        0 2021-06-21 15:50:26.807002 mrphy-0.1.9/tests/
--rw-r--r--   0 tluo      (1000) tluo      (1000)        0 2021-06-14 15:35:48.000000 mrphy-0.1.9/tests/__init__.py
--rw-r--r--   0 tluo      (1000) tluo      (1000)     5280 2021-06-21 15:44:15.000000 mrphy-0.1.9/tests/test_mobjs.py
--rw-r--r--   0 tluo      (1000) tluo      (1000)     4862 2021-06-21 15:44:15.000000 mrphy-0.1.9/tests/test_sims.py
--rw-r--r--   0 tluo      (1000) tluo      (1000)     3442 2021-06-21 15:41:37.000000 mrphy-0.1.9/tests/test_slowsims.py
--rw-r--r--   0 tluo      (1000) tluo      (1000)     2860 2021-06-14 15:35:48.000000 mrphy-0.1.9/tests/test_utils.py
+drwxr-xr-x   0 tianrluo  (1000) tianrluo  (1000)        0 2023-07-14 01:22:46.462279 mrphy-0.2.0/
+-rw-r--r--   0 tianrluo  (1000) tianrluo  (1000)     1068 2020-08-16 03:03:07.000000 mrphy-0.2.0/LICENSE
+-rw-r--r--   0 tianrluo  (1000) tianrluo  (1000)     2725 2023-07-14 01:22:46.462279 mrphy-0.2.0/PKG-INFO
+-rw-r--r--   0 tianrluo  (1000) tianrluo  (1000)     2273 2021-06-21 23:41:51.000000 mrphy-0.2.0/README.md
+drwxr-xr-x   0 tianrluo  (1000) tianrluo  (1000)        0 2023-07-14 01:22:46.462279 mrphy-0.2.0/mrphy/
+-rw-r--r--   0 tianrluo  (1000) tianrluo  (1000)     3065 2023-07-14 00:46:58.000000 mrphy-0.2.0/mrphy/__init__.py
+-rw-r--r--   0 tianrluo  (1000) tianrluo  (1000)     5622 2023-07-14 00:46:58.000000 mrphy-0.2.0/mrphy/beffective.py
+-rw-r--r--   0 tianrluo  (1000) tianrluo  (1000)    39858 2023-07-14 00:46:58.000000 mrphy-0.2.0/mrphy/mobjs.py
+-rw-r--r--   0 tianrluo  (1000) tianrluo  (1000)    17805 2023-07-14 00:46:58.000000 mrphy-0.2.0/mrphy/sims.py
+-rw-r--r--   0 tianrluo  (1000) tianrluo  (1000)     5750 2023-07-14 00:46:58.000000 mrphy-0.2.0/mrphy/slowsims.py
+-rw-r--r--   0 tianrluo  (1000) tianrluo  (1000)    10845 2023-07-14 00:46:58.000000 mrphy-0.2.0/mrphy/utils.py
+-rw-r--r--   0 tianrluo  (1000) tianrluo  (1000)       22 2023-07-14 00:46:58.000000 mrphy-0.2.0/mrphy/version.py
+drwxr-xr-x   0 tianrluo  (1000) tianrluo  (1000)        0 2023-07-14 01:22:46.462279 mrphy-0.2.0/mrphy.egg-info/
+-rw-r--r--   0 tianrluo  (1000) tianrluo  (1000)     2725 2023-07-14 01:22:46.000000 mrphy-0.2.0/mrphy.egg-info/PKG-INFO
+-rw-r--r--   0 tianrluo  (1000) tianrluo  (1000)      387 2023-07-14 01:22:46.000000 mrphy-0.2.0/mrphy.egg-info/SOURCES.txt
+-rw-r--r--   0 tianrluo  (1000) tianrluo  (1000)        1 2023-07-14 01:22:46.000000 mrphy-0.2.0/mrphy.egg-info/dependency_links.txt
+-rw-r--r--   0 tianrluo  (1000) tianrluo  (1000)       24 2023-07-14 01:22:46.000000 mrphy-0.2.0/mrphy.egg-info/requires.txt
+-rw-r--r--   0 tianrluo  (1000) tianrluo  (1000)       12 2023-07-14 01:22:46.000000 mrphy-0.2.0/mrphy.egg-info/top_level.txt
+-rw-r--r--   0 tianrluo  (1000) tianrluo  (1000)       38 2023-07-14 01:22:46.462279 mrphy-0.2.0/setup.cfg
+-rw-r--r--   0 tianrluo  (1000) tianrluo  (1000)      895 2023-07-14 00:46:58.000000 mrphy-0.2.0/setup.py
+drwxr-xr-x   0 tianrluo  (1000) tianrluo  (1000)        0 2023-07-14 01:22:46.462279 mrphy-0.2.0/tests/
+-rw-r--r--   0 tianrluo  (1000) tianrluo  (1000)        0 2020-08-16 02:54:43.000000 mrphy-0.2.0/tests/__init__.py
+-rw-r--r--   0 tianrluo  (1000) tianrluo  (1000)     6532 2022-02-03 02:46:19.000000 mrphy-0.2.0/tests/test_mobjs.py
+-rw-r--r--   0 tianrluo  (1000) tianrluo  (1000)     6606 2023-07-14 00:46:58.000000 mrphy-0.2.0/tests/test_sims.py
+-rw-r--r--   0 tianrluo  (1000) tianrluo  (1000)     4193 2023-07-14 00:46:58.000000 mrphy-0.2.0/tests/test_slowsims.py
+-rw-r--r--   0 tianrluo  (1000) tianrluo  (1000)     3285 2023-07-14 00:46:58.000000 mrphy-0.2.0/tests/test_utils.py
```

### Comparing `mrphy-0.1.9/PKG-INFO` & `mrphy-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,79 +1,79 @@
 Metadata-Version: 2.1
 Name: mrphy
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Pytorch based tool for MR physics simulations
 Home-page: https://github.com/tianrluo/MRphy.py
 Author: Tianrui Luo
 Author-email: tianrluo@umich.edu
 License: MIT
-Description: # MRphy.py
-        
-        A pytorch based MR simulator package.
-        [![](https://img.shields.io/badge/docs-stable-blue.svg)](https://tianrluo.github.io/MRphy.py/stable/index.html)
-        [![](https://img.shields.io/badge/docs-dev-blue.svg)](https://tianrluo.github.io/MRphy.py/dev/index.html)
-        [![codecov](https://codecov.io/gh/tianrluo/MRphy.py/branch/master/graph/badge.svg?token=83sKL5NADl)](https://codecov.io/gh/tianrluo/MRphy.py)
-        [![Actions Status](https://github.com/tianrluo/MRphy.py/workflows/Python%20package/badge.svg)](https://github.com/tianrluo/MRphy.py/actions)
-        
-        Infrastructure of:\
-        [Joint Design of RF and Gradient Waveforms via Auto-Differentiation for 3D Tailored Exitation in MRI](https://ieeexplore.ieee.org/document/9439482)\
-        (arXiv: [https://arxiv.org/abs/2008.10594](https://arxiv.org/abs/2008.10594))
-        
-        cite as:
-        
-        ```bib
-        @article{luo2021joint,
-          author={Luo, Tianrui and Noll, Douglas C. and Fessler, Jeffrey A. and Nielsen, Jon-Fredrik},
-          journal={IEEE Transactions on Medical Imaging}, 
-          title={Joint Design of RF and gradient waveforms via auto-differentiation for 3D tailored excitation in MRI}, 
-          year={2021},
-          volume={},
-          number={},
-          pages={1-1},
-          doi={10.1109/TMI.2021.3083104}}
-        ```
-        
-        For the `interpT` feature, consider citing:
-        ```bib
-        @inproceedings{luo2021MultiScale,
-          title={Multi-scale Accelerated Auto-differentiable Bloch-simulation based joint design of excitation RF and gradient waveforms},
-          booktitle={ISMRM},
-          pages={3958},
-          author={Tianrui Luo and Douglas C. Noll and Jeffrey A. Fessler and Jon-Fredrik Nielsen},
-          year={2021}
-        }
-        ```
-        
-        ## Branches
-        
-        - `master`: Stable;
-        - `dev`: Ocassionally `git squash`'d, `git push --force`'d;
-        - `dev_cache`: Constantly `git push --force`'d.
-        
-        Developments are mostly done on `dev_cache`; when they have passed local checks, `dev` will be `git rebase`'d to `dev_cache`, and sent for CI tests.
-        When enough updates have been accumulated, `dev` will be git squashed into one large commit, followed by having `master`-branch `git rebase`'d onto it.
-        
-        ## Installation
-        
-        ```sh
-        pip install mrphy
-        ```
-        
-        (The package is not yet sent to `conda`.)
-        
-        ## Demos
-        
-        Check out files under `./test`.
-        After installation, one can quickly play with the tests through:
-        
-        ```sh
-        pytest -s
-        ```
-        
-        Only basic demo is available in this early version.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# MRphy.py
+
+A pytorch based MR simulator package.
+[![](https://img.shields.io/badge/docs-stable-blue.svg)](https://tianrluo.github.io/MRphy.py/stable/index.html)
+[![](https://img.shields.io/badge/docs-dev-blue.svg)](https://tianrluo.github.io/MRphy.py/dev/index.html)
+[![codecov](https://codecov.io/gh/tianrluo/MRphy.py/branch/master/graph/badge.svg?token=83sKL5NADl)](https://codecov.io/gh/tianrluo/MRphy.py)
+[![Actions Status](https://github.com/tianrluo/MRphy.py/workflows/Python%20package/badge.svg)](https://github.com/tianrluo/MRphy.py/actions)
+
+Infrastructure of:\
+[Joint Design of RF and Gradient Waveforms via Auto-Differentiation for 3D Tailored Exitation in MRI](https://ieeexplore.ieee.org/document/9439482)\
+(arXiv: [https://arxiv.org/abs/2008.10594](https://arxiv.org/abs/2008.10594))
+
+cite as:
+
+```bib
+@article{luo2021joint,
+  author={Luo, Tianrui and Noll, Douglas C. and Fessler, Jeffrey A. and Nielsen, Jon-Fredrik},
+  journal={IEEE Transactions on Medical Imaging}, 
+  title={Joint Design of RF and gradient waveforms via auto-differentiation for 3D tailored excitation in MRI}, 
+  year={2021},
+  volume={},
+  number={},
+  pages={1-1},
+  doi={10.1109/TMI.2021.3083104}}
+```
+
+For the `interpT` feature, consider citing:
+```bib
+@inproceedings{luo2021MultiScale,
+  title={Multi-scale Accelerated Auto-differentiable Bloch-simulation based joint design of excitation RF and gradient waveforms},
+  booktitle={ISMRM},
+  pages={3958},
+  author={Tianrui Luo and Douglas C. Noll and Jeffrey A. Fessler and Jon-Fredrik Nielsen},
+  year={2021}
+}
+```
+
+## Branches
+
+- `master`: Stable;
+- `dev`: Ocassionally `git squash`'d, `git push --force`'d;
+- `dev_cache`: Constantly `git push --force`'d.
+
+Developments are mostly done on `dev_cache`; when they have passed local checks, `dev` will be `git rebase`'d to `dev_cache`, and sent for CI tests.
+When enough updates have been accumulated, `dev` will be git squashed into one large commit, followed by having `master`-branch `git rebase`'d onto it.
+
+## Installation
+
+```sh
+pip install mrphy
+```
+
+(The package is not yet sent to `conda`.)
+
+## Demos
+
+Check out files under `./test`.
+After installation, one can quickly play with the tests through:
+
+```sh
+pytest -s
+```
+
+Only basic demo is available in this early version.
```

### Comparing `mrphy-0.1.9/README.md` & `mrphy-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mrphy-0.1.9/mrphy/beffective.py` & `mrphy-0.2.0/mrphy/beffective.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-r""" B-effective related functions
-"""
+r"""B-effective related functions"""
 
 import torch
 import torch.nn.functional as F
 from torch import tensor, Tensor
 from typing import Optional, Tuple
 
 from mrphy import γH, dt0, π
@@ -12,19 +11,19 @@
 # TODO:
 # - Faster init of AB in `beff2ab`
 
 
 __all__ = ['beff2ab', 'beff2uφ', 'rfgr2beff']
 
 
-def beff2uϕ(beff: Tensor, γ2πdt: Tensor, dim=-1) -> Tuple[Tensor, Tensor]:
+def beff2uϕ(beff: Tensor, γ2πdt: Tensor, *, dim=-1) -> Tuple[Tensor, Tensor]:
     r"""Compute rotation axes and angles from B-effectives
 
     Usage:
-        ``U, Φ = beff2uϕ(beff, γ2πdt)``
+        ``U, Φ = beff2uϕ(beff, γ2πdt, *, dim)``
     Inputs:
         - ``beff``: `(N, *Nd, xyz)`, "Gauss", B-effective, magnetic field \
           applied on `M`.
         - ``γ2πdt``: `()` ⊻ `(N ⊻ 1, *Nd ⊻ 1,)`, "rad/Gauss", gyro ratio \
           in radiance mutiplied by `dt`.
     Optionals:
         - ``dim``: int. Indicate the `xyz`-dim, allow \
@@ -35,27 +34,29 @@
     """
     U = F.normalize(beff, dim=dim)
     Φ = -torch.norm(beff, dim=dim) * γ2πdt  # negate: BxM -> MxB
     return U, Φ
 
 
 def beff2ab(
-    beff: Tensor,
-    E1: Tensor = tensor(0.), E2: Tensor = tensor(0.), γ: Tensor = γH,
-    dt: Tensor = dt0
+    beff: Tensor, *,
+    E1: Tensor = tensor(0.),
+    E2: Tensor = tensor(0.),
+    γ: Tensor = γH,
+    dt: Tensor = dt0,
 ) -> Tuple[Tensor, Tensor]:
     r"""Compute Hargreave's 𝐴/𝐵, mat/vec, from B-effectives
 
     See: `doi:10.1002/mrm.1170 <https://doi.org/10.1002/mrm.1170>`_.
 
     Usage:
-        ``A, B = beff2ab(beff; E1, E2, γ, dt)``
+        ``A, B = beff2ab(beff, *, E1, E2, γ, dt)``
 
     Inputs:
-        - ``beff``: `(N,*Nd,xyz,nT)`, B-effective.
+        - ``beff``: `(N,*Nd,nT,xyz)`, B-effective.
     Optionals:
         - ``T1``: `()` ⊻ `(N ⊻ 1, *Nd ⊻ 1,)`, "Sec", T1 relaxation.
         - ``T2``: `()` ⊻ `(N ⊻ 1, *Nd ⊻ 1,)`, "Sec", T2 relaxation.
         - ``γ``:  `()` ⊻ `(N ⊻ 1, *Nd ⊻ 1,)`, "Hz/Gauss", gyro ratio.
         - ``dt``: `()` ⊻ `(N ⊻ 1,)`, "Sec", dwell time.
     Outputs:
         - ``A``: `(N, *Nd, xyz, 3)`, `A[:,iM,:,:]`, is the `iM`-th 𝐴.
@@ -71,25 +72,25 @@
     E1, E2, γ, dt = (x.reshape(x.shape+(ndim-x.ndim)*(1,))
                      for x in (E1, E2, γ, dt))  # (N, *Nd) compatible
 
     E1, E2, γ2πdt = E1[..., None], E2[..., None, None], 2*π*γ*dt
     E1_1 = E1.squeeze(dim=-1) - 1
 
     # C/Python `reshape/view` is different from Fortran/MatLab/Julia `reshape`
-    NNd, nT = shape[0:-2], shape[-1]
+    NNd, nT = shape[0:-2], shape[-2]
     s1, s0 = NNd+(1, 1), NNd+(1, 4)
 
     AB = torch.cat([torch.ones(s1, **dkw), torch.zeros(s0, **dkw),
                     torch.ones(s1, **dkw), torch.zeros(s0, **dkw),
                     torch.ones(s1, **dkw), torch.zeros(s1, **dkw)],
                    dim=-1).view(NNd+(3, 4))  # -> (N, *Nd, xyz, 3+1)
 
     # simulation
     for t in range(nT):
-        u, ϕ = beff2uϕ(beff[..., t], γ2πdt)
+        u, ϕ = beff2uϕ(beff[..., t, :], γ2πdt)
 
         if torch.any(ϕ != 0):
             AB1 = utils.uϕrot(u, ϕ, AB)
         else:
             AB1 = AB
 
         # Relaxation
@@ -100,64 +101,68 @@
 
     A, B = AB[..., 0:3], AB[..., 3]
 
     return A, B
 
 
 def rfgr2beff(
-    rf: Tensor, gr: Tensor, loc: Tensor,
-    Δf: Optional[Tensor] = None, b1Map: Optional[Tensor] = None, γ: Tensor = γH
+    rf: Tensor,
+    gr: Tensor,
+    loc: Tensor, *,
+    Δf: Optional[Tensor] = None,
+    b1Map: Optional[Tensor] = None,
+    γ: Tensor = γH
 ) -> Tensor:
     r"""Compute B-effectives from rf and gradients
 
     Usage:
-        ``beff = rfgr2beff(rf, gr, loc, Δf, b1Map, γ)``
+        ``beff = rfgr2beff(rf, gr, loc, *, Δf, b1Map, γ)``
     Inputs:
         - ``rf``: `(N,xy,nT,(nCoils))`, "Gauss", `xy` for separating real and \
           imag part.
         - ``gr``: `(N,xyz,nT)`, "Gauss/cm".
-    Optionals:
         - ``loc``: `(N,*Nd,xyz)`, "cm", locations.
+    Optionals:
         - ``Δf``: `(N,*Nd,)`, "Hz", off-resonance.
         - ``b1Map``: `(N, *Nd, xy (, nCoils)`, a.u., transmit sensitivity.
         - ``γ``:  `()` ⊻ `(N ⊻ 1, *Nd ⊻ 1,)`, "Hz/Gauss", gyro ratio.
     Outputs:
-        - ``beff``: `(N,*Nd,xyz,nT)`, "Gauss"
+        - ``beff``: `(N,*Nd,nT,xyz)`, "Gauss"
     """
     assert(rf.device == gr.device == loc.device)
     device = rf.device
 
     shape = loc.shape
     N, Nd, ndim = shape[0], shape[1:-1], loc.ndim-2
 
-    Bz = (loc.reshape(N, -1, 3) @ gr).reshape((N, *Nd, 1, -1))
+    Bz = (loc.reshape(N, -1, 3) @ gr).reshape((N, *Nd, -1))
 
-    if Δf is not None:  # Δf: -> (N, *Nd, 1, 1); 3 from 1(dim-N) + 2(dim-xtra)
+    if Δf is not None:  # Δf: -> (N, *Nd, 1); 3 from 1(dim-N) + 2(dim-xtra)
         γ = γ.to(device=device)
-        Δf, γ = (x.reshape(x.shape+(ndim+3-x.ndim)*(1,)) for x in (Δf, γ))
+        Δf, γ = (_.reshape(_.shape+(ndim+2-_.ndim)*(1,)) for _ in (Δf, γ))
         Bz += Δf/γ
 
     # rf -> (N, *len(Nd)*(1,), xy, nT, (nCoils))
     rf = rf.reshape((-1,) + ndim*(1,) + rf.shape[1:])
     # Real as `Bx`, Imag as `By`.
     if b1Map is None:
-        if rf.ndim == Bz.ndim+1:  # (N, *len(Nd)*(1,), xy, nT, nCoils)
+        if rf.ndim == Bz.ndim+2:  # (N, *len(Nd)*(1,), xy, nT, nCoils)
             rf = torch.sum(rf, dim=-1)  # -> (N, *len(Nd)*(1,), xy, nT)
 
-        Bx, By = rf[..., 0:1, :].expand_as(Bz), rf[..., 1:2, :].expand_as(Bz)
+        Bx, By = rf[..., 0, :].expand_as(Bz), rf[..., 1, :].expand_as(Bz)
     else:
         if b1Map.ndim == 1+len(Nd)+1:
             b1Map = b1Map[..., None]  # (N, *Nd, xy) -> (N, *Nd, xy, 1)
         if rf.ndim == b1Map.ndim:  # rf missing the nCoil dim
             rf = rf[..., None]
 
         b1Map = b1Map.to(device)
         b1Map = b1Map[..., None, :]  # -> (N, *Nd, xy, 1, nCoils)
-        Bx = torch.sum((b1Map[..., 0:1, :, :]*rf[..., 0:1, :, :]
-                        - b1Map[..., 1:2, :, :]*rf[..., 1:2, :, :]),
+        Bx = torch.sum((b1Map[..., 0, :, :]*rf[..., 0, :, :]
+                        - b1Map[..., 1, :, :]*rf[..., 1, :, :]),
                        dim=-1).expand_as(Bz)  # -> (N, *Nd, x, nT)
-        By = torch.sum((b1Map[..., 0:1, :, :]*rf[:, :, 1:2, ...]
-                        + b1Map[..., 1:2, :, :]*rf[:, :, 0:1, ...]),
+        By = torch.sum((b1Map[..., 0, :, :]*rf[:, :, 1, ...]
+                        + b1Map[..., 1, :, :]*rf[:, :, 0, ...]),
                        dim=-1).expand_as(Bz)  # -> (N, *Nd, y, nT)
 
-    beff = torch.cat([Bx, By, Bz], dim=-2)  # -> (N, *Nd, xyz, nT)
+    beff = torch.stack([Bx, By, Bz], dim=-1)  # -> (N, *Nd, nT, xyz)
     return beff
```

### Comparing `mrphy-0.1.9/mrphy/mobjs.py` & `mrphy-0.2.0/mrphy/mobjs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,30 @@
 r"""Classes for MRI excitation simulations
 """
 import copy
-from typing import TypeVar, Optional
+from typing import Optional
+import inspect
 
 import numpy as np
 from scipy import interpolate
 import torch
 from torch import tensor, Tensor
 
 from mrphy import γH, dt0, gmax0, smax0, rfmax0, T1G, T2G, π
 from mrphy import utils, beffective, sims
 
-# TODO:
-# - Abstract Class
-# - Non-compact SpinCube initialization
-
-
-Pulse = TypeVar('Pulse', bound='Pulse')
-SpinArray = TypeVar('SpinArray', bound='SpinArray')
-SpinCube = TypeVar('SpinCube', bound='SpinCube')
-
-
 __all__ = ['Pulse', 'SpinArray', 'SpinCube', 'Examples']
 
 
 class Pulse(object):
     r"""Pulse object of RF and GR
 
     Usage:
-        ``pulse = Pulse(;rf, gr, dt, gmax, smax, rfmax, desc, device, dtype)``
+        ``pulse = Pulse(rf, gr, *, dt, gmax, smax, rfmax, desc, device,``\
+        `` dtype)``
 
     Inputs:
         - ``rf``: `(N,xy, nT,(nCoils))` "Gauss", ``xy`` for separating real \
           and imag part.
         - ``gr``: `(N,xyz,nT)`, "Gauss/cm"
         - ``dt``: `()` ⊻ `(N ⊻ 1,)`, "Sec", dwell time.
         - ``gmax``: `()` ⊻ `(N ⊻ 1, xyz ⊻ 1)`, "Gauss/cm", max \|gradient\|.
@@ -60,52 +52,57 @@
 
     _readonly = ('device', 'dtype', 'is_cuda', 'shape')
     _limits = ('gmax', 'smax', 'rfmax')
     __slots__ = set(_readonly + _limits + ('rf', 'gr', 'dt', 'desc'))
 
     def __init__(
         self,
-        rf: Optional[Tensor] = None, gr: Optional[Tensor] = None,
+        rf: Optional[Tensor] = None, gr: Optional[Tensor] = None, *,
         dt: Tensor = dt0,
         gmax: Tensor = gmax0, smax: Tensor = smax0, rfmax: Tensor = rfmax0,
         desc: str = "generic pulse",
         device: torch.device = torch.device('cpu'),
         dtype: torch.dtype = torch.float32
     ):
-
         assert(isinstance(device, torch.device) and
                isinstance(dtype, torch.dtype))
 
         # Defaults
         rf_miss, gr_miss = rf is None, gr is None
         assert (not(rf_miss and gr_miss)), "Missing both `rf` and `gr` inputs"
 
-        super().__setattr__('device', device)
-        super().__setattr__('dtype', dtype)
-        super().__setattr__('is_cuda', self.device.type == 'cuda')
+        object.__setattr__(self, 'device', device)
+        object.__setattr__(self, 'dtype', dtype)
+        object.__setattr__(self, 'is_cuda', self.device.type == 'cuda')
 
         kw = {'device': self.device, 'dtype': self.dtype}
 
         if rf_miss:
             N, nT = gr.shape[0], gr.shape[2]
             rf = torch.zeros((N, 2, nT), **kw)
         else:
             N, nT = rf.shape[0], rf.shape[2]
             if gr_miss:
                 gr = torch.zeros((N, 3, nT), **kw)
             else:
                 assert (N == gr.shape[0] and nT == gr.shape[2])
-        super().__setattr__('shape', torch.Size((N, 1, nT)))
+        object.__setattr__(self, 'shape', torch.Size((N, 1, nT)))
 
         self.rf, self.gr = rf.to(**kw), gr.to(**kw)
         self.dt, self.gmax, self.smax, self.rfmax = dt, gmax, smax, rfmax
         self.desc = desc
         return
 
     def __setattr__(self, k, v):
+        if 'deepcopy' in (_.function for _ in inspect.stack()):
+            # Hack, this enables `deepcopy()` w/o overriding `__deepcopy__()`.
+            # Generator is faster than list comprehension.
+            object.__setattr__(self, k, v)
+            return
+
         if k in self._readonly:
             raise AttributeError(f"'Pulse' object attribute '{k}'"
                                  " is read-only")
 
         if k != 'desc':
             kw = {'device': self.device, 'dtype': self.dtype}
             v = (v.to(**kw) if isinstance(v, Tensor) else tensor(v, **kw))
@@ -120,22 +117,22 @@
             elif v.ndim == 2 and v.shape[1] == 1:
                 v = v[:, 0]
         elif k == 'dt':
             if v.ndim == 0:
                 v = v[None]
             assert(v.ndim == 1)
 
-        super().__setattr__(k, v)
+        object.__setattr__(self, k, v)
         return
 
-    def asdict(self, toNumpy: bool = True) -> dict:
+    def asdict(self, *, toNumpy: bool = True) -> dict:
         r"""Convert mrphy.mobjs.Pulse object to dict
 
         Usage:
-            ``d = pulse.asdict(; toNumpy)``
+            ``d = pulse.asdict(*, toNumpy)``
 
         Inputs:
             - ``toNumpy``: [T/f], convert Tensor to Numpy arrays.
         Outputs:
             - ``d``: dict, dictionary with detached data identical to the \
               object.
         """
@@ -145,43 +142,47 @@
 
         d = {k: fn_np(getattr(self, k)) for k in _}
         d.update({k: getattr(self, k) for k in ('desc', 'device', 'dtype')})
 
         return d
 
     def beff(
-            self, loc: Tensor,
-            Δf: Optional[Tensor] = None, b1Map: Optional[Tensor] = None,
-            γ: Tensor = γH) -> Tensor:
+        self, loc: Tensor, *,
+        Δf: Optional[Tensor] = None,
+        b1Map: Optional[Tensor] = None,
+        γ: Tensor = γH
+    ) -> Tensor:
         r"""Compute B-effective of provided location from the pulse
 
         Usage:
-            ``beff = pulse.beff(loc; Δf, b1Map, γ)``
+            ``beff = pulse.beff(loc, *, Δf, b1Map, γ)``
         Inputs:
             - ``loc``: `(N,*Nd,xyz)`, "cm", locations.
         Optionals:
             - ``Δf``: `(N,*Nd,)`, "Hz", off-resonance.
             - ``b1Map``: `(N,*Nd,xy,(nCoils))`, a.u., transmit sensitivity.
             - ``γ``: `(N,*Nd)`, "Hz/Gauss", gyro-ratio
         Outputs:
             - ``beff``: `(N,*Nd,xyz,nT)`
         """
         device = self.device
         loc = loc.to(device=device)
-        fn = lambda x: None if x is None else x.to(device=device)  # noqa: E731
+        fn = lambda x: None if x is None else x.to(device=device)
         Δf, b1Map, γ = (fn(x) for x in (Δf, b1Map, γ))
 
-        return beffective.rfgr2beff(self.rf, self.gr, loc,
-                                    Δf=Δf, b1Map=b1Map, γ=γ)
+        rf, gr = self.rf, self.gr
+        beff = beffective.rfgr2beff(rf, gr, loc, Δf=Δf, b1Map=b1Map, γ=γ)
 
-    def interpT(self, dt: Tensor, kind: str = 'linear') -> Pulse:
+        return beff
+
+    def interpT(self, dt: Tensor, *, kind: str = 'linear') -> 'Pulse':
         r""" Interpolate pulse of `dt` by `kind`.
 
         Usage:
-            ``new_pulse = pulse.interpT(dt; kind)``
+            ``new_pulse = pulse.interpT(dt, *, kind)``
         Inputs:
             - ``dt``: `(1,)`, "Sec", new simulation dwell time.
             - ``kind``: str, passed to scipy.interpolate.interp1d.
         Outputs:
             - ``new_pulse``: mrphy.mobjs.Pulse object.
 
         .. note::
@@ -195,17 +196,16 @@
         if dt_o_np == dt_n_np:
             return copy.deepcopy(self)
 
         axis = 2  # Along temporal dimension
         dkw = {'device': self.device, 'dtype': self.dtype}
         kw = {'axis': axis, 'kind': kind, 'copy': False, 'assume_sorted': True}
 
-        f_np = lambda x: x.detach().cpu().numpy()  # noqa: E731
-        f_0 = lambda x: np.dstack((np.zeros_like(x[:, :, [0]]),  # noqa: E731
-                                   x))
+        f_np = lambda x: x.detach().cpu().numpy()
+        f_0 = lambda x: np.dstack((np.zeros_like(x[:, :, [0]]), x))
 
         # convert to np array, then prepend 0's.
         rf_np, gr_np = f_0(f_np(self.rf)), f_0(f_np(self.gr))
 
         nT = rf_np.shape[axis]
 
         t_o = np.arange(0, nT)*dt_o_np  # (nT,)
@@ -215,20 +215,23 @@
         f_gr = interpolate.interp1d(t_o, gr_np, **kw)
 
         rf_n, gr_n = tensor(f_rf(t_n), **dkw), tensor(f_gr(t_n), **dkw)
 
         desc = f"{self.desc} + interpT\'ed: dt = {dt_n_np}"
         return Pulse(rf_n, gr_n, dt=dt, desc=desc, **dkw)
 
-    def to(self, device: torch.device = torch.device('cpu'),
-           dtype: torch.dtype = torch.float32) -> Pulse:
+    def to(
+        self, *,
+        device: torch.device = torch.device('cpu'),
+        dtype: torch.dtype = torch.float32
+    ) -> 'Pulse':
         r"""Duplicate the object to the prescribed device with dtype
 
         Usage:
-            ``new_pulse = pulse.to(;device, dtype)``
+            ``new_pulse = pulse.to(*, device, dtype)``
         Inputs:
             - ``device``: torch.device
             - ``dtype``: torch.dtype
         Outputs:
             - ``new_pulse``: mrphy.mobjs.Pulse object.
         """
         if self.device == device and self.dtype == dtype:
@@ -237,16 +240,17 @@
                      device=device, dtype=dtype)
 
 
 class SpinArray(object):
     r"""mrphy.mobjs.SpinArray object
 
     Usage:
-        ``spinarray = SpinArray(shape; mask, T1_, T2_, γ_, M_, device, dtype)``
-        ``spinarray = SpinArray(shape; mask, T1, T2, γ, M, device, dtype)``
+        ``spinarray = SpinArray(shape, mask, *, T1_, T2_, γ_, M_, device,``\
+        `` dtype)``
+        ``spinarray = SpinArray(shape, mask, *, T1, T2, γ, M, device, dtype)``
     Inputs:
         - ``shape``: tuple, e.g., ``(N, nx, ny, nz)``.
     Optionals:
         - ``mask``: `(1, *Nd)`, where does compact attributes locate in `Nd`.
         - ``T1`` ⊻ ``T1_``: `(N, *Nd ⊻ nM)`, "Sec", T1 relaxation coeff.
         - ``T2`` ⊻ ``T2_``: `(N, *Nd ⊻ nM)`, "Sec", T2 relaxation coeff.
         - ``γ`` ⊻ ``γ_``: `(N, *Nd ⊻ nM)`,  "Hz/Gauss", gyro ratio.
@@ -256,15 +260,15 @@
 
     Properties:
         - ``shape``: `(N, *Nd)`.
         - ``mask``: `(1, *Nd)`.
         - ``device``.
         - ``dtype``.
         - ``ndim``: ``len(shape)``
-        - ``nM``: ``nM = mask.sum().item()``;
+        - ``nM``: ``nM = torch.count_nonzero(mask).item()``.
         - ``T1_``: `(N, nM)`, "Sec", T1 relaxation coeff.
         - ``T2_``: `(N, nM)`, "Sec", T2 relaxation coeff.
         - ``γ_``: `(N, nM)`, "Hz/Gauss", gyro ratio.
         - ``M_``: `(N, nM, xyz)`, spins, equilibrium [0 0 1]
 
     .. warning::
         - Do NOT modify the ``mask`` of an object, e.g., \
@@ -294,15 +298,15 @@
     """
 
     _readonly = ('shape', 'mask', 'device', 'dtype', 'is_cuda', 'ndim', 'nM')
     _compact = ('T1_', 'T2_', 'γ_', 'M_')
     __slots__ = set(_readonly + _compact)
 
     def __init__(
-        self, shape: tuple, mask: Optional[Tensor] = None,
+        self, shape: tuple, mask: Optional[Tensor] = None, *,
         T1: Optional[Tensor] = None, T1_: Optional[Tensor] = None,
         T2: Optional[Tensor] = None, T2_: Optional[Tensor] = None,
         γ: Optional[Tensor] = None,  γ_: Optional[Tensor] = None,
         M: Optional[Tensor] = None,  M_: Optional[Tensor] = None,
         device: torch.device = torch.device('cpu'),
         dtype: torch.dtype = torch.float32
     ):
@@ -311,21 +315,21 @@
                 if mask is None else mask.to(device=device))
 
         assert(isinstance(device, torch.device) and
                isinstance(dtype, torch.dtype) and
                mask.dtype == torch.bool and
                mask.shape == (1,)+shape[1:])
 
-        super().__setattr__('shape', shape)
-        super().__setattr__('mask', mask)
-        super().__setattr__('ndim', len(shape))
-        super().__setattr__('nM', torch.sum(mask).item())
-        super().__setattr__('device', device)
-        super().__setattr__('dtype', dtype)
-        super().__setattr__('is_cuda', self.device.type == 'cuda')
+        object.__setattr__(self, 'shape', shape)
+        object.__setattr__(self, 'mask', mask)
+        object.__setattr__(self, 'ndim', len(shape))
+        object.__setattr__(self, 'nM', torch.count_nonzero(mask).item())
+        object.__setattr__(self, 'device', device)
+        object.__setattr__(self, 'dtype', dtype)
+        object.__setattr__(self, 'is_cuda', self.device.type == 'cuda')
 
         assert((T1 is None) or (T1_ is None))
         if T1 is None:
             self.T1_ = (T1G if T1_ is None else T1_)
         else:
             self.T1 = T1
 
@@ -345,24 +349,30 @@
         if M is None:
             self.M_ = (tensor([0., 0., 1.]) if M_ is None else M_)
         else:
             self.M = M
 
         return
 
-    def __getattr__(self, k):
+    def __getattr__(self, k):  # provoked only when `__getattribute__` failed
         if k+'_' not in self._compact:
             raise AttributeError(f"'SpinArray' has no attribute '{k}'")
 
         v_ = getattr(self, k+'_')
         return (self.embed(v_) if self.nM != np.prod(self.shape[1:]) else
                 v_.reshape(self.shape+v_.shape[2:]))  # ``mask`` is all True
 
     def __setattr__(self, k_, v_):
-        if (k_ in self._readonly) or (k_+'_' in self._readonly):
+        if 'deepcopy' in (_.function for _ in inspect.stack()):
+            # Hack, this enables `deepcopy()` w/o overriding `__deepcopy__()`.
+            # Generator is faster than list comprehension.
+            object.__setattr__(self, k_, v_)
+            return
+
+        if k_ in self._readonly:
             raise AttributeError(f"'SpinArray' object attribute '{k_}'"
                                  " is read-only")
 
         # Transfer ``v_`` to ``kw`` before ``extract`
         kw = {'device': self.device, 'dtype': self.dtype}
         v_ = (v_.to(**kw) if isinstance(v_, Tensor) else tensor(v_, **kw))
 
@@ -374,30 +384,30 @@
         # `tensor.expand(size)` needs `tensor.shape` broadcastable with `size`
         if k_ == 'M_':
             if v_.shape != shape[:1]+(self.nM, 3):  # (N, nM, xyz)
                 v_ = v_.expand(shape[:1]+(self.nM, 3)).clone()
         elif k_ in self._compact:  # (T1_, T2_, γ_)
             v_ = v_.expand((self.shape[0], self.nM))  # (N, nM)
 
-        super().__setattr__(k_, v_)
+        object.__setattr__(self, k_, v_)
         return
 
     def applypulse(
-        self, pulse: Pulse,
+        self, pulse: Pulse, *,
         doEmbed: bool = False, doRelax: bool = True, doUpdate: bool = False,
         loc: Optional[Tensor] = None, loc_: Optional[Tensor] = None,
         Δf: Optional[Tensor] = None, Δf_: Optional[Tensor] = None,
         b1Map: Optional[Tensor] = None, b1Map_: Optional[Tensor] = None
     ) -> Tensor:
         r"""Apply a pulse to the spinarray object
 
         Typical usage:
-            ``M = spinarray.applypulse(pulse; loc, doEmbed=True, doRelax, ``\
-            ``doUpdate, Δf, b1Map)``
-            ``M_ = spinarray.applypulse(pulse; loc_, doEmbed=False, `` \
+            ``M = spinarray.applypulse(pulse, *, loc, doEmbed=True, doRelax,``\
+            `` doUpdate, Δf, b1Map)``
+            ``M_ = spinarray.applypulse(pulse, *, loc_, doEmbed=False, `` \
             ``doRelax, doUpdate, Δf_, b1Map_)``
         Inputs:
             - ``pulse``: mrphy.mobjs.Pulse.
             - ``loc`` ⊻ ``loc_``: `(N,*Nd ⊻ nM,xyz)`, "cm", locations.
         Optionals:
             - ``doEmbed``: [t/F], return ``M`` or ``M_``
             - ``doRelax``: [T/f], do relaxation during Bloch simulation.
@@ -435,19 +445,19 @@
 
         M_ = sims.blochsim(self.M_, beff_, **kw_bsim)
         if doUpdate:
             self.M_ = M_
         M_ = (self.embed(M_) if doEmbed else M_)
         return M_
 
-    def asdict(self, toNumpy: bool = True, doEmbed: bool = True) -> dict:
+    def asdict(self, *, toNumpy: bool = True, doEmbed: bool = True) -> dict:
         r"""Convert mrphy.mobjs.SpinArray object to dict
 
         Usage:
-            ``d = spinarray.asdict(;toNumpy, doEmbed)``
+            ``d = spinarray.asdict(*, toNumpy, doEmbed)``
 
         Inputs:
             - ``toNumpy``: [T/f], convert ``Tensor`` to Numpy arrays.
             - ``doEmbed``: [T/f], embed compactly stored (nM) data to the \
               mask (\*Nd).
         Outputs:
             - ``d``: dict, dictionary with detached data identical to the \
@@ -495,19 +505,19 @@
         r"""Nd of the spinarray object, syntax sugar for len(spinarray.shape)
 
         Usage:
             ``Nd = spinarray.dim()``
         """
         return len(self.shape)
 
-    def embed(self, v_: Tensor, out: Optional[Tensor] = None) -> Tensor:
+    def embed(self, v_: Tensor, *, out: Optional[Tensor] = None) -> Tensor:
         """Embed compact data into the spinarray.mask
 
         Usage:
-            ``out = spinarray.embed(v_; out)``
+            ``out = spinarray.embed(v_, *, out)``
         Inputs:
             - ``v_``: `(N, nM, ...)`, must be contiguous.
         Optionals:
             - ``out``: `(N, *Nd, ...)`, in-place holder.
         Outputs:
             - ``out``: `(N, *Nd, ...)`.
         """
@@ -515,19 +525,19 @@
         out = (v_.new_full(oshape, float('NaN')) if out is None else out)
         mask = self.mask.expand(self.shape)
         out[mask] = v_.view((-1,)+v_.shape[2:])
         # `v.reshape()` has intermediate alloc, leaving `out` pointless.
         # out[mask] = v_.reshape((-1,)+v_.shape[2:])
         return out
 
-    def extract(self, v: Tensor, out_: Optional[Tensor] = None) -> Tensor:
+    def extract(self, v: Tensor, *, out_: Optional[Tensor] = None) -> Tensor:
         r"""Extract data with the spinarray.mask, making it compact
 
         Usage:
-            ``out_ = spinarray.extract(v; out_)``
+            ``out_ = spinarray.extract(v, *, out_)``
         Inputs:
             - ``v``: `(N, *Nd, ...)`.
         Optionals:
             - ``out_``: `(N, nM, ...)`, in-place holder, must be contiguous.
         Outputs:
             - ``out_``: `(N, nM, ...)`.
         """
@@ -538,15 +548,54 @@
         # fail instead.
         out_.view((-1,)+v.shape[self.ndim:]).copy_(v[mask])
         # ``v[mask].reshape()`` has intermediate alloc, leaving ``out_``
         # pointless.
         # out_.copy_(v[mask].reshape((-1,)+v.shape[self.ndim:]))
         return out_
 
-    def mask_(self, mask: Tensor) -> Tensor:
+    def freeprec(
+        self, dur: Tensor, *,
+        doEmbed: bool = False, doRelax: bool = True, doUpdate: bool = False,
+        Δf: Optional[Tensor] = None, Δf_: Optional[Tensor] = None
+    ) -> Tensor:
+        r"""Free precession of duration ``dur``
+
+        Typical usage:
+            ``M = obj.freeprec(dur, doEmbed=True, doRelax, doUpdate, Δf)``
+            ``M_ = obj.applypulse(dur, doEmbed=False, doRelax, doUpdate, Δf_)``
+        Inputs:
+            - ``dur``: `()` ⊻ `(N ⊻ 1,)`, "Sec", duration of free-precession.
+        Optionals:
+            - ``doEmbed``: [t/F], return ``M`` or ``M_``
+            - ``doRelax``: [T/f], do relaxation during free precession.
+            - ``doUpdate``: [t/F], update ``self.M_``
+            - ``Δf``⊻ ``Δf_``: `(N ⊻ 1,*Nd ⊻ nM)`, "Hz", off-resonance.
+        Outputs:
+            - ``M`` ⊻ ``M_``: `(N,*Nd ⊻ nM,xyz)`
+
+        .. note::
+            When ``doUpdate == True and doEmbed == False``, the output compact
+            magnetization Tensor is a reference to ``self.M_``, and needs
+            caution when being accessed.
+        """
+        assert ((Δf_ is None) or (Δf is None))
+        Δf_ = (Δf_ if Δf is None else self.extract(Δf))
+
+        if doRelax:
+            kw_bsim = {'T1': self.T1_, 'T2': self.T2_}
+        else:
+            kw_bsim = {'T1': None, 'T2': None}
+
+        M_ = sims.freeprec(self.M_, dur, **kw_bsim, Δf=Δf_)
+        if doUpdate:
+            self.M_ = M_
+        M_ = (self.embed(M_) if doEmbed else M_)
+        return M_
+
+    def mask_(self, *, mask: Tensor) -> Tensor:
         r"""Extract the compact region of an input external ``mask``.
 
         Usage:
             ``mask_ = spinarray.mask_(mask)``
         Inputs:
             - ``mask``: `(1, *Nd)`.
         Outputs:
@@ -564,25 +613,25 @@
 
         Usage:
             ``res = spinarray.numel()``
         """
         return self.mask.numel()
 
     def pulse2beff(
-        self, pulse: Pulse, doEmbed: bool = False,
+        self, pulse: Pulse, *, doEmbed: bool = False,
         loc: Optional[Tensor] = None, loc_: Optional[Tensor] = None,
         Δf: Optional[Tensor] = None, Δf_: Optional[Tensor] = None,
         b1Map: Optional[Tensor] = None, b1Map_: Optional[Tensor] = None
     ) -> Tensor:
         r"""Compute B-effective of ``pulse`` with the spinarray's parameters
 
         Typical usage:
-            ``beff = spinarray.pulse2beff(pulse; loc, doEmbed=True, Δf, ``\
+            ``beff = spinarray.pulse2beff(pulse, *, loc, doEmbed=True, Δf, ``\
             ``b1Map)``
-            ``beff_ = spinarray.pulse2beff(pulse; loc_, doEmbed=False, ``\
+            ``beff_ = spinarray.pulse2beff(pulse, *, loc_, doEmbed=False, ``\
             ``Δf_, b1Map_)``
         Inputs:
             - ``pulse``: mrphy.mobjs.Pulse.
             - ``loc`` ⊻ ``loc_``: `(N,*Nd ⊻ nM,xyz)`, "cm", locations.
         Optionals:
             - ``doEmbed``: [t/F], return ``beff`` or ``beff_``
             - ``Δf`` ⊻ ``Δf_``: `(N,*Nd ⊻ nM)`, "Hz", off-resonance.
@@ -612,41 +661,42 @@
 
         Usage:
             ``sz = spinarray.size()``
         """
         return self.shape
 
     def to(
-        self,
+        self, *,
         device: torch.device = torch.device('cpu'),
         dtype: torch.dtype = torch.float32
-    ) -> SpinArray:
+    ) -> 'SpinArray':
         r"""Duplicate the object to the prescribed device with dtype
 
         Usage:
-            ``new_spinarray = spinarray.to(;device, dtype)``
+            ``new_spinarray = spinarray.to(*, device, dtype)``
         Inputs:
             - ``device``: torch.device
             - ``dtype``: torch.dtype
         Outputs:
             - ``new_spinarray``: mrphy.mobjs.SpinArray object
         """
         if self.device == device and self.dtype == dtype:
             return self
         return SpinArray(self.shape, self.mask, T1_=self.T1_, T2_=self.T2_,
                          γ_=self.γ_, M_=self.M_, device=device, dtype=dtype)
 
 
-class SpinCube(object):
+class SpinCube(SpinArray):
     r"""mrphy.mobjs.SpinCube object
 
     Usage:
-        ``SpinCube(shape, fov; mask, ofst, Δf_, T1_, T2_, γ_, M_, device, ``\
-        ``dtype)``
-        ``SpinCube(shape, fov; mask, ofst, Δf, T1, T2, γ, M, device, dtype)``
+        ``SpinCube(shape, fov, mask, *, ofst, Δf_, T1_, T2_, γ_, M_, device,``\
+        `` dtype)``
+        ``SpinCube(shape, fov, mask, *, ofst, Δf, T1, T2, γ, M, device,``\
+        '' dtype)``
     Inputs:
         - ``shape``: tuple, e.g., ``(N, nx, ny, nz)``.
         - ``fov``: `(N, xyz)`, "cm", field of view.
     Optionals:
         - ``mask``: `(1, *Nd)`, where does compact attributes locate in `Nd`.
         - ``ofst``: `(N, xyz)`, Tensor "cm", fov offset from iso-center.
         - ``Δf`` ⊻ ``Δf_``: `(N, *Nd ⊻ nM)`, "Hz", off-resonance map.
@@ -666,56 +716,77 @@
     """
 
     _readonly = ('spinarray', 'loc_')
     _compact = ('Δf_', 'loc_')  # `loc_` depends on `shape`, `fov` and `ofst`
     __slots__ = set(_readonly+_compact+('fov', 'ofst'))
 
     def __init__(
-        self, shape: tuple, fov: Tensor, mask: Optional[Tensor] = None,
+        self, shape: tuple, fov: Tensor, *, mask: Optional[Tensor] = None,
         ofst: Tensor = tensor([[0., 0., 0.]]),
         Δf: Optional[Tensor] = None, Δf_: Optional[Tensor] = None,
         T1: Optional[Tensor] = None, T1_: Optional[Tensor] = None,
         T2: Optional[Tensor] = None, T2_: Optional[Tensor] = None,
         γ: Optional[Tensor] = None,  γ_: Optional[Tensor] = None,
         M: Optional[Tensor] = None,  M_: Optional[Tensor] = None,
         device: torch.device = torch.device('cpu'),
         dtype: torch.dtype = torch.float32
     ):
+        # 1) `SpinCube` is subclassed to `SpinArray`.
+        # 2) Attribute `spinarray` is included to enable extracting the
+        # `SpinArray` part of a `SpinCube()` instance.
+        # 3) `SpinCube.__getattr__` is tweaked for immitating super class
+        # access to `SpinCube().spinarray`'s attributes.
+        # To have these three features, we cannot have `super().__init__()` in
+        # `SpinCube`, which will disable the `__getattr__` tweak.
         sp = SpinArray(shape, mask, T1=T1, T1_=T1_, T2=T2, T2_=T2_, γ=γ, γ_=γ_,
                        M=M, M_=M_, device=device, dtype=dtype)
-        super().__setattr__('spinarray', sp)
+        object.__setattr__(self, 'spinarray', sp)
 
         kw = {'device': sp.device, 'dtype': sp.dtype}
         # setattr(self, k, v), avoid computing `loc_` w/ `fov` & `ofst` not set
-        super().__setattr__('fov', fov.to(**kw))
-        super().__setattr__('ofst', ofst.to(**kw))
+        object.__setattr__(self, 'fov', fov.to(**kw))
+        object.__setattr__(self, 'ofst', ofst.to(**kw))
         # Initialize ``loc_`` in memory, reuse it.
-        super().__setattr__('loc_', torch.zeros((sp.shape[0], sp.nM, 3), **kw))
+        object.__setattr__(self, 'loc_',
+                           torch.zeros((sp.shape[0], sp.nM, 3), **kw))
         self._update_loc_()  # compute ``loc_`` from set ``fov`` & ``ofst`
 
         assert((Δf is None) or (Δf_ is None))
         if Δf is None:
             self.Δf_ = (tensor(0.) if Δf_ is None else Δf_)
         else:
             self.Δf = Δf
 
         return
 
     def __getattr__(self, k):  # provoked only when `__getattribute__` failed
         if k+'_' not in self._compact:  # k not in ('Δf_', 'loc')
+            # Cannot do `self.spinarray` or `getattr(self, 'spinarray')` here.
+            # They cause infinite recursion when `SpinCube().__getattr__()` is
+            # queried with `spinarray`, which may happen during `deepcopy` or
+            # `pickle`.
+            # Therefore, call `object.__getattribute__()` here, and let it fail
+            # when it should.
+            spinarray = object.__getattribute__(self, 'spinarray')
             try:
-                return getattr(self.spinarray, k)
+                return getattr(spinarray, k)
             except AttributeError:
                 raise AttributeError(f"'SpinCube' has no attribute '{k}'")
 
         v_, sp = getattr(self, k+'_'), self.spinarray
         return (sp.embed(v_) if sp.nM != np.prod(sp.shape[1:]) else
                 v_.reshape(sp.shape+v_.shape[2:]))  # `mask` is all True
 
     def __setattr__(self, k_, v_):
+        if 'deepcopy' in (_.function for _ in inspect.stack()):
+            # Hack, this enables `deepcopy()` w/o overriding `__deepcopy__()`.
+            # Generator is faster than list comprehension.
+            object.__setattr__(self, k_, v_)
+            return
+
         if (k_ in self._readonly) or (k_+'_' in self._readonly):
             raise AttributeError(f"'SpinCube' object attribute '{k_}'"
                                  " is read-only")
 
         sp = self.spinarray
         if k_ in SpinArray.__slots__ or k_+'_' in SpinArray.__slots__:
             setattr(sp, k_, v_)
@@ -730,15 +801,15 @@
             v_ = self.extract(v_.expand(shape+(3,) if k_ == 'loc_' else shape))
 
         if k_ == 'Δf_':
             v_ = v_.expand((shape[0], sp.nM))  # (N, nM)
         elif k_ in ('fov', 'ofst'):
             assert(v_.ndim == 2)
 
-        super().__setattr__(k_, v_)
+        object.__setattr__(self, k_, v_)
 
         # update `loc_` when needed
         if k_ in ('fov', 'ofst'):
             self._update_loc_()
         return
 
     def _update_loc_(self):
@@ -764,23 +835,24 @@
             # `torch.addr`'s `vec2`, _locn[i][mask[0, ...]], provokes alloc.
             loc_[..., i] = (fov[:, None, i]*_locn[i][mask[0, ...]][None, ...]
                             + ofst[:, None, i])
 
         return
 
     def applypulse(
-        self, pulse: Pulse,
+        self, pulse: Pulse, *,
         doEmbed: bool = False, doRelax: bool = True, doUpdate: bool = False,
         b1Map: Optional[Tensor] = None, b1Map_: Optional[Tensor] = None
     ) -> Tensor:
         r"""Apply a pulse to the spincube object
 
         Usage:
-            ``M = spincube.applypulse(pulse; doEmbed=True, doRelax, b1Map)``
-            ``M_ = spincube.applypulse(pulse; doEmbed=False, doRelax, b1Map_)``
+            ``M = spincube.applypulse(pulse, *, doEmbed=True, doRelax, b1Map)``
+            ``M_ = spincube.applypulse(pulse, *, doEmbed=False, doRelax,``\
+            `` b1Map_)``
 
         Inputs:
             - ``pulse``: mobjs.Pulse object.
         Optionals:
             - ``doEmbed``: [t/F], return ``M`` or ``M_``.
             - ``doRelax``: [T/f], do relaxation during Bloch simulation.
             - ``b1Map`` ⊻ ``b1Map_``: `(N,*Nd ⊻ nM,xy,(nCoils))`, transmit \
@@ -792,19 +864,46 @@
         b1Map_ = (b1Map_ if b1Map is None else self.extract(b1Map))
 
         return self.spinarray.applypulse(pulse, doEmbed=doEmbed,
                                          doRelax=doRelax, doUpdate=doUpdate,
                                          Δf_=self.Δf_, loc_=self.loc_,
                                          b1Map_=b1Map_)
 
-    def asdict(self, toNumpy: bool = True, doEmbed: bool = True) -> dict:
+    def freeprec(
+        self, dur: Tensor, *,
+        doEmbed: bool = False, doRelax: bool = True, doUpdate: bool = False
+    ) -> Tensor:
+        r"""Free precession of duration ``dur``
+
+        Typical usage:
+            ``M = obj.freeprec(dur, doEmbed=True, doRelax, doUpdate)``
+            ``M_ = obj.applypulse(dur, doEmbed=False, doRelax, doUpdate)``
+        Inputs:
+            - ``dur``: `()` ⊻ `(N ⊻ 1,)`, "Sec", duration of free-precession.
+        Optionals:
+            - ``doEmbed``: [t/F], return ``M`` or ``M_``
+            - ``doRelax``: [T/f], do relaxation during free precession.
+            - ``doUpdate``: [t/F], update ``self.M_``
+        Outputs:
+            - ``M`` ⊻ ``M_``: `(N,*Nd ⊻ nM,xyz)`
+
+        .. note::
+            When ``doUpdate == True and doEmbed == False``, the output compact
+            magnetization Tensor is a reference to ``self.M_``, and needs
+            caution when being accessed.
+        """
+
+        return self.spinarray.freeprec(dur, Δf_=self.Δf_, doEmbed=doEmbed,
+                                       doRelax=doRelax, doUpdate=doUpdate)
+
+    def asdict(self, *, toNumpy: bool = True, doEmbed: bool = True) -> dict:
         r"""Convert mrphy.mobjs.SpinCube object to dict
 
         Usage:
-            ``d = spincube.asdict(;toNumpy, doEmbed)``
+            ``d = spincube.asdict(*, toNumpy, doEmbed)``
 
         Inputs:
             - ``toNumpy``: [T/f], convert ``Tensor`` to Numpy arrays.
             - ``doEmbed``: [T/f], embed compactly stored (nM) data to the \
               mask `(*Nd)`.
         Outputs:
             - ``d``: dict, dictionary with detached data identical to the \
@@ -817,134 +916,46 @@
         d = {k: fn_np(getattr(self, k)) for k in _}
 
         d.update({k: getattr(self, k) for k in ('fov', 'ofst')})
 
         d.update(self.spinarray.asdict(toNumpy=toNumpy, doEmbed=doEmbed))
         return d
 
-    def crds_(self, crds: list) -> list:
-        r"""Compute crds for compact attributes
-
-        Data in a SpinCube object is stored compactly, such that only those
-        correspond to ``1`` on the ``spincube.mask`` is kept.
-        This function is provided to facilitate indexing the compact data from
-        regular indices, by computing (ix, iy, iz) -> iM
-
-        Usage:
-            ``crds_ = spincube.crds_(crds)``
-        Inputs:
-            - ``crds``: indices for indexing non-compact attributes.
-        Outputs:
-            - ``crds_``: list, ``len(crds_) == 2+len(crds)-self.ndim``.
-
-        ``v_[crds_] == v[crds]``, when ``v_[crds_]=new_value`` is effective.
-        """
-        return self.spinarray.crds_(crds)
-
-    def dim(self) -> int:
-        r"""Nd of the spincube object, syntax sugar for len(spincube.shape)
-
-        Usage:
-            ``Nd = spincube.dim()``
-        """
-        return self.spinarray.dim()
-
-    def embed(self, v_: Tensor, out: Optional[Tensor] = None) -> Tensor:
-        r"""Embed compact data into the ``spincube.mask``.
-
-        Usage:
-            ``out = spincube.embed(v_; out)``
-        Inputs:
-            - ``v_``: `(N, nM, ...)`, must be contiguous.
-        Optionals:
-            - ``out``: `(N, *Nd, ...)`, in-place holder.
-        Outputs:
-            - ``out``: `(N, *Nd, ...)`.
-        """
-        return self.spinarray.embed(v_, out=out)
-
-    def extract(self, v: Tensor, out_: Optional[Tensor] = None) -> Tensor:
-        r"""Extract data with the ``spincube.mask``, making it compact
-
-        Usage:
-            ``out_ = spincube.extract(v; out_)``
-        Inputs:
-            - ``v``: `(N, *Nd, ...)`.
-        Optionals:
-            - ``out_``: `(N, nM, ...)`, in-place holder, must be contiguous.
-        Outputs:
-            - ``out_``: `(N, nM, ...)`.
-        """
-        return self.spinarray.extract(v, out_=out_)
-
-    def mask_(self, mask: Tensor) -> Tensor:
-        r"""Extract the compact region of an input external ``mask``.
-
-        Usage:
-            ``mask_ = spincube.mask_(mask)``
-        Inputs:
-            - ``mask``: `(1, *Nd)`.
-        Outputs:
-            - ``mask_``: `(1, nM)`, can be used on compact attributes.
-        """
-        return self.spinarray.mask_(mask)
-
-    def numel(self) -> int:
-        r"""Number of spins for the spincube object, incompact.
-
-        Syntax sugar of ``spincube.mask.numel()``, effectively
-        ``prod(spincube.size())``.
-
-        Usage:
-            ``res = spincube.numel()``
-        """
-        return self.spinarray.numel()
-
     def pulse2beff(
-        self, pulse: Pulse,
+        self, pulse: Pulse, *,
         doEmbed: bool = False,
         b1Map: Optional[Tensor] = None, b1Map_: Optional[Tensor] = None
     ) -> Tensor:
         r"""Compute B-effective of ``pulse`` with the spincube's parameters
 
         Typical usage:
-            ``beff = spincube.pulse2beff(pulse; doEmbed=True, b1Map)``
-            ``beff_ = spincube.pulse2beff(pulse; doEmbed=False, b1Map_)``
+            ``beff = spincube.pulse2beff(pulse, *, doEmbed=True, b1Map)``
+            ``beff_ = spincube.pulse2beff(pulse, *, doEmbed=False, b1Map_)``
         Inputs:
             - ``pulse``: mrphy.mobjs.Pulse.
         Optionals:
             - ``doEmbed``: [t/F], return ``beff`` or ``beff_``.
             - ``b1Map`` ⊻ ``b1Map_``: `(N,*Nd ⊻ nM,xy,(nCoils))`, transmit \
               sensitivity.
         Outputs:
             - ``beff`` ⊻ ``beff_``: `(N,*Nd ⊻ nM,xyz,nT)`.
         """
         return self.spinarray.pulse2beff(pulse, self.loc_, doEmbed=doEmbed,
                                          Δf_=self.Δf_,
                                          b1Map=b1Map, b1Map_=b1Map_)
 
-    def size(self) -> tuple:
-        r"""Size of the spincube object.
-
-        Syntax sugar of ``spincube.shape``.
-
-        Usage:
-            ``sz = spincube.size()``
-        """
-        return self.spinarray.size()
-
     def to(
-        self,
+        self, *,
         device: torch.device = torch.device('cpu'),
         dtype: torch.dtype = torch.float32
-    ) -> SpinCube:
+    ) -> 'SpinCube':
         r"""Duplicate the object to the prescribed device with dtype
 
         Usage:
-            ``new_spincube = spincube.to(;device, dtype)``
+            ``new_spincube = spincube.to(*, device, dtype)``
         Inputs:
             - ``device``: torch.device.
             - ``dtype``: torch.dtype.
         Outputs:
             - ``new_spincube``: mrphy.mobjs.SpinCube object.
         """
         if self.device == device and self.dtype == dtype:
@@ -952,15 +963,16 @@
         return SpinCube(self.shape, self.fov, ofst=self.ofst, Δf_=self.Δf_,
                         T1_=self.T1_, T2_=self.T2_, γ_=self.γ_, M_=self.M_,
                         device=device, dtype=dtype)
 
 
 class SpinBolus(SpinArray):
     def __init__(
-            self):
+        self
+    ):
         pass
     pass
 
 
 class Examples(object):
     r"""Class for quickly creating exemplary instances to play around with.
     """
```

### Comparing `mrphy-0.1.9/mrphy/sims.py` & `mrphy-0.2.0/mrphy/sims.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,203 +14,215 @@
 # TODO:
 # - Avoid caching when needs_input_grad is False
 # - Create `BlochSim_rfgr` that directly computes grads w.r.t. `rf` and `gr`.
 
 
 __all__ = ['blochsim']
 
+_contiguous_format = torch.contiguous_format
+
 
 class BlochSim(Function):
     r"""BlochSim with explict Jacobian operation (backward)
 
     This operator is only differentiable w.r.t. ``Mi`` and ``Beff``.
 
     """
 
     @staticmethod
     def forward(
-        ctx: CTX, Mi: Tensor, Beff: Tensor,
-        T1: Optional[Tensor], T2: Optional[Tensor], γ: Tensor, dt: Tensor
+        ctx: CTX,
+        Mi: Tensor,
+        Beff: Tensor,
+        T1: Optional[Tensor],
+        T2: Optional[Tensor],
+        γ: Tensor,
+        dt: Tensor
     ) -> Tensor:
         r"""Forward evolution of Bloch simulation
 
         Inputs:
             - ``ctx``: `(1,)`, pytorch CTX cacheing object
             - ``Mi``: `(N, *Nd, xyz)`, Magnetic spins, assumed equilibrium \
               [0 0 1]
-            - ``Beff``: `(N, *Nd, xyz, nT)`, "Gauss", B-effective, magnetic \
+            - ``Beff``: `(N, *Nd, nT, xyz)`, "Gauss", B-effective, magnetic \
               field.
             - ``T1``: `(N ⊻ 1, *Nd ⊻ len(Nd)*(1,), 1, 1)`, "Sec", T₁
             - ``T2``: `(N ⊻ 1, *Nd ⊻ len(Nd)*(1,), 1, 1)`, "Sec", T₂
             - ``γ``:  `(N ⊻ 1, *Nd ⊻ len(Nd)*(1,), 1, 1)`, "Hz/Gauss", gyro.
             - ``dt``: `(N ⊻ 1, len(Nd)*(1,), 1, 1)`, "Sec", dwell time.
         Outputs:
             - ``Mo``: `(N, *Nd, xyz)`, Magetic spins after simulation.
         """
-        NNd, nT = Beff.shape[:-2], Beff.shape[-1]
+        NNd, nT = Beff.shape[:-2], Beff.shape[-2]
         # (t)ensor (k)ey(w)ord, contiguous to avoid alloc/copy when reshape
-        tkw = {'memory_format': torch.contiguous_format,
+        tkw = {'memory_format': _contiguous_format,
                'dtype': Mi.dtype, 'device': Mi.device}
 
         # %% Preprocessing
         γ2πdt = 2*π*γ*dt
-        Mi = Mi.clone(memory_format=torch.contiguous_format)[..., None]
         γBeff = torch.empty(Beff.shape, **tkw)
         torch.mul(γ2πdt, Beff, out=γBeff)
+        Mi = Mi.clone(memory_format=_contiguous_format)[..., None, :]
         # γBeff = γ2πdt*Beff.contiguous()
 
         assert((T1 is None) == (T2 is None))  # both or neither
 
         if T1 is None:  # relaxations ignored
             E = e1_1 = None
-            fn_relax_ = lambda m1: None  # noqa: E731
+            fn_relax_ = lambda m1: None
         else:
             E1, E2 = -dt/T1, -dt/T2
             E1.exp_(), E2.exp_()  # should have fewer alloc than exp(-dt/T1)
-            E, e1_1 = torch.cat((E2, E2, E1), dim=-2), E1-1
-            fn_relax_ = lambda m1: (m1.mul_(E)  # noqa: E731
-                                    )[..., 2:3, :].sub_(e1_1)
+            E, e1_1 = torch.cat((E2, E2, E1), dim=-1), E1-1
+            fn_relax_ = lambda m1: (m1.mul_(E))[..., 2:3].sub_(e1_1)
 
         # Pre-allocate intermediate variables, in case of overhead alloc's
-        u = torch.empty(Mi.shape, **tkw)  # (N, *Nd, xyz, 1)
-        ϕ, cϕ_1, sϕ = (torch.empty(NNd+(1, 1), **tkw) for _ in range(3))
+        v = torch.empty(Mi.shape, **tkw)  # (N, *Nd, xyz, 1)
 
         # %% Other variables to be cached
-        m0, Mhst = Mi, torch.empty(NNd+(3, nT), **tkw)
+        m0 = Mi
+        Mhst = torch.empty(NNd+(nT, 3), **tkw)
+        Φ = torch.empty(NNd+(nT, 1), **tkw)
+        cΦ_1 = torch.empty(NNd+(nT, 1), **tkw)
+        sΦ = torch.empty(NNd+(nT, 1), **tkw)
+        UtM0 = torch.empty(NNd+(nT, 1), **tkw)
 
         # %% Simulation. could we learn to live right.
-        for m1, γbeff in zip(Mhst.split(1, dim=-1), γBeff.split(1, dim=-1)):
+        for m1, γbeff, ϕ, cϕ_1, sϕ, utm0 in zip(
+            Mhst.split(1, dim=-2),
+            γBeff.split(1, dim=-2),
+            Φ.split(1, dim=-2),
+            cΦ_1.split(1, dim=-2),
+            sΦ.split(1, dim=-2),
+            UtM0.split(1, dim=-2),
+        ):
             # Rotation
-            torch.norm(γbeff, dim=-2, keepdim=True, out=ϕ)
+            torch.norm(γbeff, dim=-1, keepdim=True, out=ϕ)
             ϕ.clamp_(min=1e-12)
-            torch.div(γbeff, ϕ, out=u)
+            torch.div(γbeff, ϕ, out=γbeff)
+            u = γbeff
 
             torch.sin(ϕ, out=sϕ)
             torch.cos(ϕ, out=cϕ_1)
             cϕ_1.sub_(1)  # (cϕ-1)
 
-            ϕ.clamp_(min=1e-12)
-            torch.div(γbeff, ϕ, out=u)
-
             # wiki/Rotation_matrix#Rotation_matrix_from_axis_and_angle
             # Angle is `-ϕ` as Bloch-eq is 𝑀×𝐵
             # m₁ = R(u, -ϕ)m₀ = cϕ*m₀ + (1-cϕ)*uᵀm₀*u - sϕ*u×m₀
             # m₁ = m₀ - sϕ*u×m₀ + (cϕ-1)*(m₀ - uᵀm₀*u), in-place friendly
             torch.mul(u, m0, out=m1)  # using m₁ as an temporary storage
-            torch.sum(m1, dim=-2, keepdim=True, out=ϕ)  # ϕ reused as uᵀm₀
+            torch.sum(m1, dim=-1, keepdim=True, out=utm0)
 
-            torch.cross(u, m0, dim=-2, out=m1)  # u×m₀
+            torch.cross(u, m0, dim=-1, out=m1)  # u×m₀
             torch.addcmul(m0, sϕ, m1, value=-1, out=m1)  # m₀ - sϕ*(u×m₀)
 
-            torch.addcmul(m0, ϕ, u, value=-1, out=u)  # m₀ - uᵀm₀*u
+            torch.addcmul(m0, utm0, u, value=-1, out=v)  # m₀ - uᵀm₀*u
 
-            torch.addcmul(m1, cϕ_1, u, out=m1)  # m₀-sϕ*u×m₀+(cϕ-1)*(m₀-uᵀm₀*u)
+            torch.addcmul(m1, cϕ_1, v, out=m1)  # m₀-sϕ*u×m₀+(cϕ-1)*(m₀-uᵀm₀*u)
 
             # Relaxation
             fn_relax_(m1)
 
             m0 = m1
 
-        ctx.save_for_backward(Mi, Mhst, γBeff, E, e1_1, γ2πdt)
-        Mo = Mhst[..., -1].clone()  # -> (N, *Nd, xyz)
+        ctx.save_for_backward(
+            Mi, Mhst, γBeff, Φ, cΦ_1, sΦ, UtM0, E, e1_1, γ2πdt
+        )
+        Mo = Mhst[..., -1, :].clone()  # -> (N, *Nd, xyz)
         return Mo
 
     @staticmethod
     def backward(
-        ctx: CTX, grad_Mo: Tensor
+        ctx: CTX,
+        grad_Mo: Tensor
     ) -> Tuple[Tensor, Tensor, None, None, None, None]:
         r"""Backward evolution of Bloch simulation Jacobians
 
         Inputs:
             - ``ctx``: `(1,)`, pytorch CTX cacheing object
             - ``grad_Mo``: `(N, *Nd, xyz)`, derivative w.r.t. output Magetic \
               spins.
         Outputs:
             - ``grad_Mi``: `(N, *Nd, xyz)`, derivative w.r.t. input Magetic \
               spins.
-            - ``grad_Beff``: `(N,*Nd,xyz,nT)`, derivative w.r.t. B-effective.
+            - ``grad_Beff``: `(N,*Nd,nT,xyz)`, derivative w.r.t. B-effective.
             - None*4, this implemendation do not provide derivatives w.r.t.: \
               `T1`, `T2`, `γ`, and `dt`.
         """
         # grads of configuration variables are not supported yet
         needs_grad = ctx.needs_input_grad
         grad_Beff = grad_Mi = grad_T1 = grad_T2 = grad_γ = grad_dt = None
 
         if not any(needs_grad[0:2]):  # (Mi,Beff;T1,T2,γ,dt):
             return grad_Mi, grad_Beff, grad_T1, grad_T2, grad_γ, grad_dt
 
         # %% Jacobians. If we turn back time,
         # ctx.save_for_backward(Mi, Mhst, γBeff, E, e1_1, γ2πdt)
-        Mi, Mhst, γBeff, E, e1_1, γ2πdt = ctx.saved_tensors
+        Mi, Mhst, γBeff, Φ, cΦ_1, sΦ, UtM0, E, e1_1, γ2πdt = ctx.saved_tensors
         NNd = γBeff.shape[:-2]
         # (t)ensor (k)ey(w)ord, contiguous to avoid alloc/copy when reshape
-        tkw = {'memory_format': torch.contiguous_format,
+        tkw = {'memory_format': _contiguous_format,
                'dtype': Mi.dtype, 'device': Mi.device}
 
         # assert((E is None) == (e1_1 is None))  # both or neither
         if E is None:  # relaxations ignored
-            fn_relax_h1_ = lambda h1: None  # noqa: E731
-            fn_relax_m1_ = lambda m1: None  # noqa: E731
+            fn_relax_h1_ = lambda h1: None
+            fn_relax_m1_ = lambda m1: None
         else:
-            fn_relax_h1_ = lambda h1: h1.mul_(E)  # noqa: E731
+            fn_relax_h1_ = lambda h1: h1.mul_(E)
 
             def fn_relax_m1_(m1):
-                m1[..., 2:3, :].add_(e1_1)
+                m1[..., :, 2:3].add_(e1_1)
                 m1.div_(E)
                 return
 
         # Pre-allocate intermediate variables, in case of overhead alloc's
-        h0 = torch.empty(NNd+(3, 1), **tkw)
-        h1 = grad_Mo.clone(memory_format=torch.contiguous_format)[..., None]
+        h0 = torch.empty(NNd+(1, 3), **tkw)
 
-        u, uxh1 = (torch.empty(NNd+(3, 1), **tkw) for _ in range(2))
-        ϕ, cϕ_1, sϕ, utm0, uth1 = (torch.empty(NNd+(1, 1), **tkw)
-                                   for _ in range(5))
+        u, uxh1 = (torch.empty(NNd+(1, 3), **tkw) for _ in range(2))
+        ϕ, cϕ_1, sϕ, uth1 = (torch.empty(NNd+(1, 1), **tkw) for _ in range(4))
         # ϕis0 = torch.empty(NNd+(1, 1),
         #                    memory_format=tkw['memory_format'],
         #                    device=tkw['device'], dtype=torch.bool)
+        h1 = grad_Mo.clone(memory_format=_contiguous_format)[..., None, :]
         # u_dflt = torch.tensor([[0.], [0.], [1.]],  # (xyz, 1)
         #                       device=tkw['device'], dtype=tkw['dtype'])
 
-        m1 = Mhst.narrow(-1, -1, 1)
+        m1 = Mhst.narrow(-2, -1, 1)
 
         # scale by -γ2πdt, so output ∂L/∂B no longer needs multiply by -γ2πdt
         h1.mul_(-γ2πdt)
-        for m0, γbeff in zip(reversed((Mi,)+Mhst.split(1, dim=-1)[:-1]),
-                             reversed(γBeff.split(1, dim=-1))):
+        for m0, γbeff, ϕ, cϕ_1, sϕ, utm0 in zip(
+            reversed((Mi,)+Mhst.split(1, dim=-2)[:-1]),
+            reversed(γBeff.split(1, dim=-2)),
+            reversed(Φ.split(1, dim=-2)),
+            reversed(cΦ_1.split(1, dim=-2)),
+            reversed(sΦ.split(1, dim=-2)),
+            reversed(UtM0.split(1, dim=-2)),
+        ):
             # %% Ajoint Relaxation:
             fn_relax_h1_(h1)  # h₁ → h̃₁ ≔ ∂L/∂m̃₁ = E∂L/∂m₁
             fn_relax_m1_(m1)  # m₁ → m̃₁ ≔ Rm₀ = E⁻¹m₁
 
             # %% Adjoint Rotations:
-            # Prepare all the elements
-            torch.norm(γbeff, dim=-2, keepdim=True, out=ϕ)
-            # compute `sin`, `cos` before `ϕ.clamp_()`
-            torch.sin(ϕ, out=sϕ)
-            torch.cos(ϕ, out=cϕ_1)
-            cϕ_1.sub_(1)
-
-            ϕ.clamp_(min=1e-12)
-            torch.div(γbeff, ϕ, out=u)
+            u.copy_(γbeff)
 
             # TODO: Resolve singularities of ϕ=0, control pov?
             # torch.logical_not(ϕ, out=ϕis0)
             # if torch.any(ϕis0):
             #     u[ϕis0[..., 0, 0]] = u_dflt
 
-            torch.mul(u, m0, out=h0)
-            torch.sum(h0, dim=-2, keepdim=True, out=utm0)  # uᵀm₀
-
             # %% Assemble h₀: (R(u, -ϕ)ᵀ ≡ R(u, ϕ))
             # h₀ ≔ R(u, ϕ)h̃₁ = cϕ*h₁ + (1-cϕ)*uᵀh₁*u + sϕ*u×h₁
             # h₀ = h̃₁ + (cϕ-1)*(h̃₁ - uᵀh̃₁*u) + sϕ*u×h̃₁, in-place friendly
             torch.mul(u, h1, out=h0)  # using h0 as an temporary storage
-            torch.sum(h0, dim=-2, keepdim=True, out=uth1)  # uᵀh̃₁
+            torch.sum(h0, dim=-1, keepdim=True, out=uth1)  # uᵀh̃₁
 
-            torch.cross(u, h1, dim=-2, out=uxh1)  # u×h̃₁
+            torch.cross(u, h1, dim=-1, out=uxh1)  # u×h̃₁
             torch.addcmul(h1, uth1, u, value=-1, out=h0)  # h̃₁-uᵀh̃₁*u
 
             torch.addcmul(h1, cϕ_1, h0, out=h0)  # h̃₁ + (cϕ-1)*(h̃₁-uᵀh̃₁*u)
 
             # Finish: h₀ = h̃₁ + (cϕ-1)*(h̃₁ - uᵀh̃₁*u) + sϕ*u×h̃₁
             torch.addcmul(h0, sϕ, uxh1, value=1, out=h0)
 
@@ -220,65 +232,65 @@
             #       +((sϕ/ϕ⋅m₀-m̃₁)ᵀ(u×h̃₁)-2(cϕ-1)/ϕ⋅uᵀm₀⋅uᵀh̃1)*u )
 
             cϕ_1.div_(ϕ), sϕ.div_(ϕ)  # cϕ-1, sϕ → (cϕ-1)/ϕ, sϕ/ϕ
             # if torch.any(ϕis0):  # handle division-by-0
             #     cϕ_1[ϕis0], sϕ[ϕis0] = 0, 1
 
             # %%% sϕ/ϕ⋅(m₀×h̃₁)
-            torch.cross(m0, h1, dim=-2, out=γbeff)  # m₀×h̃₁
+            torch.cross(m0, h1, dim=-1, out=γbeff)  # m₀×h̃₁
             γbeff.mul_(sϕ)  # sϕ/ϕ⋅(m₀×h̃₁)
 
             # %%% sϕ/ϕ⋅(m₀×h̃₁) + (cϕ-1)/ϕ⋅(uᵀm₀⋅h̃₁+uᵀh̃₁⋅m₀)
             h1.mul_(utm0)  # uᵀm₀⋅h̃₁
             torch.addcmul(h1, uth1, m0, out=h1)  # (uᵀm₀⋅h̃₁+uᵀh̃₁⋅m₀)
             torch.addcmul(γbeff, cϕ_1, h1, value=1, out=γbeff)
 
             # %%% sϕ/ϕ⋅(m₀×h̃₁) + (cϕ-1)/ϕ⋅(uᵀm₀⋅h̃₁+uᵀh̃₁⋅m₀)
             #     -((m̃₁-sϕ/ϕ⋅m₀)ᵀ(u×h̃₁) + 2(cϕ-1)/ϕ⋅uᵀh̃1⋅uᵀm₀)⋅u
 
             # (m̃₁-sϕ/ϕ⋅m₀)ᵀ(u×h̃₁)
             torch.addcmul(m1, sϕ, m0, value=-1, out=m1)  # (m̃₁-sϕ/ϕ⋅m₀)
             m1.mul_(uxh1)
-            torch.sum(m1, dim=-2, keepdim=True, out=sϕ)
+            torch.sum(m1, dim=-1, keepdim=True, out=sϕ)
 
             # ((m̃₁-sϕ/ϕ⋅m₀)ᵀ(u×h̃₁) + 2(cϕ-1)/ϕ⋅uᵀh̃₁⋅uᵀm₀)
             uth1.mul_(utm0)  # uᵀh̃1⋅uᵀm₀
             torch.addcmul(sϕ, cϕ_1, uth1, value=2, out=cϕ_1)
 
             torch.addcmul(γbeff, cϕ_1, u, value=-1, out=γbeff)
 
             m1, h1, h0 = m0, h0, h1
 
         # %% Clean up
         grad_Beff = γBeff
 
         # undo the multiply by -γ2πdt on h1
-        grad_Mi = h1[..., 0].div_(-γ2πdt[0, ...]) if needs_grad[0] else None
+        grad_Mi = h1[..., 0, :].div_(-γ2πdt[0, ...]) if needs_grad[0] else None
         # forward(ctx, Mi, Beff; T1, T2, γ, dt):
         return grad_Mi, grad_Beff, grad_T1, grad_T2, grad_γ, grad_dt
 
 
 def blochsim(
-    Mi: Tensor, Beff: Tensor,
+    Mi: Tensor, Beff: Tensor, *,
     T1: Optional[Tensor] = None, T2: Optional[Tensor] = None,
     γ: Tensor = γH, dt: Tensor = dt0
 ) -> Tensor:
     r"""Bloch simulator with explicit Jacobian operation.
 
     This function is only differentiable w.r.t. ``Mi`` and ``Beff``.
 
     Setting `T1=T2=None` to opt for simulation ignoring relaxation.
 
     Usage:
-        ``Mo = blochsim(Mi, Beff; T1, T2, γ, dt)``
-        ``Mo = blochsim(Mi, Beff; T1=None, T2=None, γ, dt)``
+        ``Mo = blochsim(Mi, Beff, *, T1, T2, γ, dt)``
+        ``Mo = blochsim(Mi, Beff, *, T1=None, T2=None, γ, dt)``
     Inputs:
         - ``Mi``: `(N, *Nd, xyz)`, Magnetic spins, assumed equilibrium \
           [[[0 0 1]]].
-        - ``Beff``: `(N, *Nd, xyz, nT)`, "Gauss", B-effective, magnetic field.
+        - ``Beff``: `(N, *Nd, nT, xyz)`, "Gauss", B-effective, magnetic field.
     Optionals:
         - ``T1``: `()` ⊻ `(N ⊻ 1, *Nd ⊻ 1,)`, "Sec", T1 relaxation.
         - ``T2``: `()` ⊻ `(N ⊻ 1, *Nd ⊻ 1,)`, "Sec", T2 relaxation.
         - ``γ``:  `()` ⊻ `(N ⊻ 1, *Nd ⊻ 1,)`, "Hz/Gauss", gyro ratio.
         - ``dt``: `()` ⊻ `(N ⊻ 1,)`, "Sec", dwell time.
     Outputs:
         - ``Mo``: `(N, *Nd, xyz)`, Magetic spins after simulation.
@@ -297,7 +309,150 @@
     γ, dt = (x.reshape(x.shape+(ndim-x.ndim)*(1,)) for x in (γ, dt))
 
     assert((T1 is None) == (T2 is None))  # both or neither
     if T1 is not None:
         T1, T2 = (x.reshape(x.shape+(ndim-x.ndim)*(1,)) for x in (T1, T2))
 
     return BlochSim.apply(Mi, Beff, T1, T2, γ, dt)
+
+
+class FreePrec(Function):
+    r"""Free precession with explicit Jacobian operation (backward)
+
+    This operator is only differentiable w.r.t. ``Mi``.
+
+    """
+
+    @staticmethod
+    def forward(
+        ctx: CTX, Mi: Tensor, dur: Tensor,
+        T1: Optional[Tensor], T2: Optional[Tensor], Δf: Optional[Tensor]
+    ) -> Tensor:
+        r"""Forward operation of free precession
+
+        Inputs:
+            - ``ctx``: `(1,)`, pytorch CTX cacheing object
+            - ``Mi``: `(N, *Nd, xyz)`, Magnetic spins, assumed equilibrium \
+              [0 0 1]
+            - ``dur``: `(N ⊻ 1, len(Nd)*(1,), 1)`, "Sec", dwell time.
+            - ``T1``: `(N ⊻ 1, *Nd ⊻ len(Nd)*(1,), 1)`, "Sec", T₁
+            - ``T2``: `(N ⊻ 1, *Nd ⊻ len(Nd)*(1,), 1)`, "Sec", T₂
+            - ``Δf``: `(N ⊻ 1, *Nd ⊻ len(Nd)*(1,))`, "Sec", T₂
+        Outputs:
+            - ``Mo``: `(N, *Nd, xyz)`, Magetic spins after simulation.
+        """  # could we learn to live right.
+
+        Mo = Mi.clone(memory_format=_contiguous_format)
+
+        # Precession
+        cϕ = sϕ = tmp = None
+        if Δf is not None:  # positive Δf dephases clock-wise/negatively
+            sϕ = -(2*π)*Δf*dur[..., 0]
+            cϕ = torch.cos(sϕ)
+            sϕ.sin_()  # ϕ is now sϕ
+
+            tmp = Mo[..., 0].clone(memory_format=_contiguous_format)  # Mix
+            Mo[..., 0].mul_(cϕ)  # cϕ*Mix
+            torch.addcmul(Mo[..., 0], sϕ, Mo[..., 1], value=-1,
+                          out=Mo[..., 0])  # Mox = cϕ*Mix - sϕ*Miy
+
+            Mo[..., 1].mul_(cϕ)
+            torch.addcmul(Mo[..., 1], sϕ, tmp,
+                          out=Mo[..., 1])  # Moy = sϕ*Mix + cϕ*Miy
+
+        # Relaxation
+        E1 = E2 = E1_1 = None
+        assert((T1 is None) == (T2 is None))  # both or neither
+
+        if T1 is not None:
+            E1, E2 = -dur/T1, -dur/T2
+            E1_1 = torch.expm1(E1)  # E1 - 1
+            E1.exp_(), E2.exp_()  # should have fewer alloc than exp(-dt/T1)
+            Mo[..., 0:2].mul_(E2)
+            Mo[..., 2:3].mul_(E1).sub_(E1_1)
+
+        ctx.save_for_backward(cϕ, sϕ, E1, E2, tmp)
+
+        return Mo
+
+    @staticmethod
+    def backward(
+        ctx: CTX, grad_Mo: Tensor
+    ) -> Tuple[Tensor, None, None, None, None]:
+        r"""Backward operation of free precession
+
+        Inputs:
+            - ``ctx``: `(1,)`, pytorch CTX cacheing object
+            - ``grad_Mo``: `(N, *Nd, xyz)`, derivative w.r.t. output Magetic \
+              spins.
+        Outputs:
+            - ``grad_Mi``: `(N, *Nd, xyz)`, derivative w.r.t. input Magetic \
+              spins.
+            - None*4, this implemendation do not provide derivatives w.r.t.: \
+              `dur`, `T1`, `T2`, and `Δf`.
+        """  # If we turn back time,
+        # grads of configuration variables are not supported yet
+        needs_grad = ctx.needs_input_grad
+        grad_Mi = grad_dur = grad_T1 = grad_T2 = grad_Δf = None
+
+        if not any(needs_grad[0:1]):
+            return grad_Mi, grad_dur, grad_T1, grad_T2, grad_Δf
+
+        grad_Mi = grad_Mo.clone(memory_format=_contiguous_format)
+
+        # ctx.save_for_backward(cϕ, sϕ, E1, E2, E1_1)
+        cϕ, sϕ, E1, E2, tmp = ctx.saved_tensors
+
+        # Relaxation
+        if E1 is not None:
+            grad_Mi[..., 0:2].mul_(E2)
+            grad_Mi[..., 2:3].mul_(E1)
+
+        # Precession
+        if tmp is not None:
+            tmp.copy_(grad_Mi[..., 1])  # copy of ∂Moy
+            grad_Mi[..., 1].mul_(cϕ)  # cϕ*∂Moy
+            torch.addcmul(grad_Mi[..., 1], sϕ, grad_Mi[..., 0], value=-1,
+                          out=grad_Mi[..., 1])  # ∂Miy = -sϕ∂Mox + cϕ*∂Moy
+
+            grad_Mi[..., 0].mul_(cϕ)  # cϕ*∂Mox
+            torch.addcmul(grad_Mi[..., 0], sϕ, tmp,
+                          out=grad_Mi[..., 0])  # ∂Mix = cϕ*∂Mox + sϕ∂Moy
+
+        return grad_Mi, grad_dur, grad_T1, grad_T2, grad_Δf
+
+
+def freeprec(
+    Mi: Tensor, dur: Tensor, *,
+    T1: Optional[Tensor] = None, T2: Optional[Tensor] = None,
+    Δf: Optional[Tensor] = None
+) -> Tensor:
+    r"""Isochromats free precession with given relaxation and off-resonance
+
+    This function is only differentiable w.r.t. ``Mi``.
+
+    Setting `T1=T2=None` to opt for simulation ignoring relaxation.
+
+    Usage:
+        ``Mo = freeprec(Mi, dur, *, T1, T2, Δf)``
+    Inputs:
+        - ``Mi``: `(N, *Nd, xyz)`, Magnetic spins, assumed equilibrium \
+          magnitude [0 0 1]
+        - ``dur``: `()` ⊻ `(N ⊻ 1,)`, "Sec", duration of free-precession.
+    OPTIONALS:
+        - ``T1``: `()` ⊻ `(N ⊻ 1, *Nd ⊻ 1,)`, "Sec", T1 relaxation.
+        - ``T2``: `()` ⊻ `(N ⊻ 1, *Nd ⊻ 1,)`, "Sec", T2 relaxation.
+        - ``Δf``: `(N ⊻ 1, *Nd ⊻ 1,)`, "Hz", off-resonance.
+    Outputs:
+        - ``Mo``: `(N, *Nd, xyz)`, Result magnetic spins
+    """
+    ndim = Mi.ndim  # dur, T1, T2, Δf are reshaped to be compatible w/ M
+    dur = dur.reshape(dur.shape+(ndim-dur.ndim)*(1,))
+
+    assert((T1 is None) == (T2 is None))  # both or neither
+    if T1 is not None:  # → (N ⊻ 1, *Nd ⊻ len(Nd)*(1,), 1)
+        T1, T2 = (x.reshape(x.shape+(ndim-x.ndim)*(1,)) for x in (T1, T2))
+
+    if Δf is not None:  # → (N ⊻ 1, *Nd ⊻ len(Nd)*(1,))
+        Δf = Δf.reshape(Δf.shape+(ndim-1-Δf.ndim)*(1,))
+
+    return FreePrec.apply(Mi, dur, T1, T2, Δf)
```

### Comparing `mrphy-0.1.9/mrphy/slowsims.py` & `mrphy-0.2.0/mrphy/slowsims.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,20 +5,25 @@
 from torch import tensor, Tensor
 from typing import Optional, Tuple
 
 from mrphy import γH, dt0, π
 from mrphy import utils, beffective
 
 
-__all__ = ['blochsim_1step', 'blochsim', 'blochsim_ab']
+__all__ = ['blochsim_1step', 'blochsim', 'blochsim_ab', 'freeprec']
 
 
 def blochsim_1step(
-    M: Tensor, M1: Tensor, b: Tensor,
-    E1: Tensor, E1_1: Tensor, E2: Tensor, γ2πdt: Tensor
+    M: Tensor,
+    M1: Tensor,
+    b: Tensor,
+    E1: Tensor,
+    E1_1: Tensor,
+    E2: Tensor,
+    γ2πdt: Tensor,
 ) -> Tuple[Tensor, Tensor]:
     r"""Single step bloch simulation
 
     Usage:
         ``M = blochsim_1step(M, M1, b, E1, E1_1, E2, γ2πdt)``
     Inputs:
         - ``M``: `(N, *Nd, xyz)`, Magnetic spins, assumed equilibrium \
@@ -46,27 +51,30 @@
     M1[..., 2] -= E1_1
 
     M, M1 = M1, M
     return M, M1
 
 
 def blochsim(
-    M: Tensor, Beff: Tensor,
-    T1: Optional[Tensor] = None, T2: Optional[Tensor] = None,
-    γ: Tensor = γH, dt: Tensor = dt0
+    M: Tensor,
+    Beff: Tensor, *,
+    T1: Optional[Tensor] = None,
+    T2: Optional[Tensor] = None,
+    γ: Tensor = γH,
+    dt: Tensor = dt0
 ) -> Tensor:
     r"""Bloch simulator with implicit Jacobian operations.
 
     Usage:
-        ``Mo = blochsim(Mi, Beff; T1, T2, γ, dt)``
-        ``Mo = blochsim(Mi, Beff; T1=None, T2=None, γ, dt)``
+        ``Mo = blochsim(Mi, Beff, *, T1, T2, γ, dt)``
+        ``Mo = blochsim(Mi, Beff, *, T1=None, T2=None, γ, dt)``
     Inputs:
         - ``M``: `(N, *Nd, xyz)`, Magnetic spins, assumed equilibrium \
           [[[0 0 1]]].
-        - ``Beff``: `(N, *Nd, xyz, nT)`, "Gauss", B-effective, magnetic field.
+        - ``Beff``: `(N, *Nd, nT, xyz)`, "Gauss", B-effective, magnetic field.
     OPTIONALS:
         - ``T1``: `()` ⊻ `(N ⊻ 1, *Nd ⊻ 1,)`, "Sec", T1 relaxation.
         - ``T2``: `()` ⊻ `(N ⊻ 1, *Nd ⊻ 1,)`, "Sec", T2 relaxation.
         - ``γ``:  `()` ⊻ `(N ⊻ 1, *Nd ⊻ 1,)`, "Hz/Gauss", gyro ratio.
         - ``dt``: `()` ⊻ `(N ⊻ 1,)`, "Sec", dwell time.
     Outputs:
         - ``M``: `(N, *Nd, xyz)`, Magetic spins after simulation.
@@ -86,16 +94,16 @@
     # preprocessing
     E1, E2, γ, dt = map(lambda x: x.reshape(x.shape+(ndim-x.ndim)*(1,)),
                         (E1, E2, γ, dt))  # (N, *Nd) compatible
 
     E1_1, E2, γ2πdt = E1 - 1, E2[..., None], 2*π*γ*dt  # Hz/Gs -> Rad/Gs
 
     # simulation
-    for t in range(Beff.shape[-1]):
-        u, ϕ = beffective.beff2uϕ(Beff[..., t], γ2πdt)
+    for t in range(Beff.shape[-2]):
+        u, ϕ = beffective.beff2uϕ(Beff[..., t, :], γ2πdt)
         if torch.any(ϕ != 0):
             M1 = utils.uϕrot(u, ϕ, M)
         else:
             M1 = M
         # Relaxation
         M1[..., 0:2] *= E2
         M1[..., 2] *= E1
@@ -117,7 +125,50 @@
         - ``A``: `(N, *Nd, xyz, 3)`, ``A[:,iM,:,:]`` is the `iM`-th 𝐴.
         - ``B``: `(N, *Nd, xyz)`, ``B[:,iM,:]`` is the `iM`-th 𝐵.
     Outputs:
         - ``M``: `(N, *Nd, xyz)`, Result magnetic spins
     """
     M = (A @ M[..., None]).squeeze_(dim=-1) + B
     return M
+
+
+def freeprec(
+    M: Tensor, dur: Tensor, *,
+    T1: Optional[Tensor] = None, T2: Optional[Tensor] = None,
+    Δf: Optional[Tensor] = None
+) -> Tensor:
+    r"""Isochromats free precession with given relaxation and off-resonance
+
+    Usage:
+        ``M = freeprec(M, dur, *, T1, T2, Δf)``
+    Inputs:
+        - ``M``: `(N, *Nd, xyz)`, Magnetic spins, assumed equilibrium \
+          magnitude [0 0 1]
+        - ``dur``: `()` ⊻ `(N ⊻ 1,)`, "Sec", duration of free-precession.
+    OPTIONALS:
+        - ``T1``: `()` ⊻ `(N ⊻ 1, *Nd ⊻ 1,)`, "Sec", T1 relaxation.
+        - ``T2``: `()` ⊻ `(N ⊻ 1, *Nd ⊻ 1,)`, "Sec", T2 relaxation.
+        - ``Δf``: `(N ⊻ 1, *Nd ⊻ 1,)`, "Hz", off-resonance.
+    Outputs:
+        - ``M``: `(N, *Nd, xyz)`, Result magnetic spins
+    """
+    ndim = M.ndim  # dur, T1, T2, Δf are reshaped to be compatible w/ M
+    dur = dur.reshape(dur.shape+(ndim-dur.ndim)*(1,))
+
+    Mx, My, Mz = M.split(1, dim=-1)  # (N, *Nd, 1)
+
+    # Precession
+    if Δf is not None:
+        Δf = Δf.reshape(Δf.shape+(ndim-Δf.ndim)*(1,))
+        ϕ = -(2*π)*Δf*dur  # positive Δf dephases spin clock-wise/negatively
+        cϕ, sϕ = torch.cos(ϕ), torch.sin(ϕ)
+        Mx, My = cϕ*Mx-sϕ*My, sϕ*Mx+cϕ*My
+
+    # Relaxation
+    assert((T1 is None) == (T2 is None))  # both or neither
+    if T1 is not None:
+        T1, T2 = (x.reshape(x.shape+(ndim-x.ndim)*(1,)) for x in (T1, T2))
+        E1, E2 = torch.exp(-dur/T1), torch.exp(-dur/T2)
+        Mx, My, Mz = E2*Mx, E2*My, E1*Mz+1-E1
+
+    M = torch.cat((Mx, My, Mz), dim=-1)  # (N, *Nd, xyz)
+    return M
```

### Comparing `mrphy-0.1.9/mrphy/utils.py` & `mrphy-0.2.0/mrphy/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from numbers import Number
 
 import torch
 import numpy as np
 from numpy import ndarray as ndarray_c
 from torch import Tensor
 
-from mrphy import γH, dt0, π
-if torch.cuda.is_available():
+from mrphy import γH, dt0, π, __CUPY_IS_AVAILABLE__
+if __CUPY_IS_AVAILABLE__:
     import cupy as cp
     from cupy import ndarray as ndarray_g
     ndarrayA = Union[ndarray_c, ndarray_g]
 else:
     ndarrayA = ndarray_c
 
 
@@ -29,19 +29,19 @@
 
     Usage:
         ``cSub = ctrsub(shape)``
     """
     return shape//2
 
 
-def g2k(g: Tensor, isTx: bool, γ: Tensor = γH, dt: Tensor = dt0) -> Tensor:
+def g2k(g: Tensor, isTx: bool, dt: Tensor = dt0, *, γ: Tensor = γH) -> Tensor:
     r"""Compute k-space from gradients.
 
     Usage:
-        ``k = g2k(g, isTx; γ, dt)``
+        ``k = g2k(g, isTx, dt, *, γ)``
 
     Inputs:
         - ``g``: `(N, xyz, nT)`, "Gauss/cm", gradient
         - ``isTx``, if ``true``, compute transmit k-space, `k`, ends at the \
           origin.
     Optionals:
         - ``γ``:  `()` ⊻ `(N ⊻ 1, *Nd ⊻ 1,)`, "Hz/Gauss", gyro ratio
@@ -62,15 +62,15 @@
     return k
 
 
 def g2s(g: Tensor, dt: Tensor = dt0) -> Tensor:
     r"""Compute slew rates from gradients.
 
     Usage:
-        ``s = g2s(g; dt)``
+        ``s = g2s(g, dt)``
     Inputs:
         - ``g``: `(N, xyz, nT)`, "Gauss/cm", gradient
     Optionals:
         - ``dt``: `()` ⊻ `(N ⊻ 1,)`, "Sec", dwell time.
     Outputs:
         - ``s``: `(N, xyz, nT)`, "cycle/cm/sec", slew rate
 
@@ -79,19 +79,19 @@
     """
     dt = dt.reshape(dt.shape+(g.ndim-dt.ndim)*(1,))
 
     s = torch.cat((g[:, :, [0]], g[:, :, 1:] - g[:, :, :-1]), dim=2)/dt
     return s
 
 
-def k2g(k: Tensor, isTx: bool, γ: Tensor = γH, dt: Tensor = dt0) -> Tensor:
+def k2g(k: Tensor, isTx: bool, dt: Tensor = dt0, *, γ: Tensor = γH) -> Tensor:
     r"""Compute k-space from gradients
 
     Usage:
-        ``k = k2g(k, isTx; γ, dt)``
+        ``k = k2g(k, isTx, dt, *, γ)``
 
     Inputs:
         - ``k``: `(N, xyz, nT)`, "cycle/cm", Tx or Rx k-space.
         - ``isTx``, if ``true``, compute transmit k-space, ``k``, must end at \
           the origin.
     Optionals:
         - ``γ``:  `()` ⊻ `(N ⊻ 1, *Nd ⊻ 1,)`, "Hz/Gauss", gyro ratio
@@ -107,14 +107,34 @@
     ndim = k.ndim
     γ, dt = (x.reshape(x.shape+(ndim-x.ndim)*(1,)) for x in (γ, dt))
 
     g = torch.cat((k[:, :, [0]], k[:, :, 1:] - k[:, :, :-1]), dim=2)/γ/dt
     return g
 
 
+def lρθ2rf(lρ: Tensor, θ: Tensor, rfmax: Tensor) -> Tensor:
+    r"""Convert tρ ≔ tan(ρ/ρ_max⋅π/2), and θ to real RF
+
+    Usage:
+        ``rf = lρθ2rf(lρ, θ, rfmax)``
+    Inputs:
+        - ``lρ``: `(N, 1, nT, (nCoils))`, logit(ρ/rfmax), [-∞, +∞).
+        - ``θ``: `(N, 1, nT, (nCoils))`, RF phase, [-π, π).
+        - ``rfmax``: `(N, (nCoils))`, RF pulse, Gauss, x for real, y for imag.
+    Outputs:
+        - ``rf``: `(N, xy, nT, (nCoils))`, RF pulse, Gauss, x: real, y: imag.
+
+    See Also:
+        :func:`~mrphy.utils.rf2lρθ`
+    """
+    rfmax = rfmax[None] if rfmax.ndim == 0 else rfmax
+    rfmax = rfmax[:, None, None, ...]  # -> (N, 1, 1, (nCoils))
+    return lρ.sigmoid()*rfmax*torch.cat((θ.cos(), θ.sin()), dim=1)
+
+
 def rf_c2r(rf: ndarrayA) -> ndarrayA:
     r"""Convert complex RF to real RF
 
     Usage:
         ``rf = rf_c2r(rf)``
     Inputs:
         - ``rf``: `(N, 1, nT, (nCoils))`, RF pulse, complex
@@ -122,16 +142,18 @@
         - ``rf``: `(N, xy, nT, (nCoils))`, RF pulse, x for real, y for imag.
 
     See Also:
         :func:`~mrphy.utils.rf_r2c`
     """
     if isinstance(rf, ndarray_c):
         return np.concatenate((np.real(rf), np.imag(rf)), axis=1)
-    else:  # ndarray_g, i.e., cupy.ndarray
+    elif __CUPY_IS_AVAILABLE__:  # ndarray_g, i.e., cupy.ndarray
         return cp.concatenate((cp.real(rf), cp.imag(rf)), axis=1)
+    else:
+        raise TypeError(f'Unknown type: {type(rf)}')
 
 
 def rf_r2c(rf: ndarrayA) -> ndarrayA:
     r"""Convert real RF to complex RF
 
     Usage:
         ``rf = rf_r2c(rf)``
@@ -142,41 +164,65 @@
 
     See Also:
         :func:`~mrphy.utils.rf_c2r`
     """
     return rf[:, [0], ...] + 1j*rf[:, [1], ...]
 
 
+def rf2lρθ(
+    rf: Tensor,
+    rfmax: Tensor, *,
+    eps: Number = 1e-7
+) -> Tuple[Tensor, Tensor]:
+    """Convert real RF to tρ ≔ tan(ρ/ρ_max⋅π/2), and θ
+
+    Usage:
+        ``lρ, θ = rf2lρθ(rf, rfmax)``
+    Inputs:
+        - ``rf``: `(N, xy, nT, (nCoils))`, RF pulse, Gauss, x: real, y: imag.
+        - ``rfmax``: `(N, (nCoils))`, RF pulse, Gauss.
+    Outputs:
+        - ``lρ``: `(N, 1, nT, (nCoils))`, logit(ρ/rfmax), [0, +∞).
+        - ``θ``: `(N, 1, nT, (nCoils))`, RF phase, [-π, π].
+
+    See Also:
+        :func:`~mrphy.utils.lρθ2rf`
+    """
+    rfmax = rfmax[None] if rfmax.ndim == 0 else rfmax  # scalar to 1d-tensor
+    lρ = (rf.norm(dim=1, keepdim=True)/rfmax[:, None, None, ...]).logit(eps)
+    θ = torch.atan2(rf[:, [1], :], rf[:, [0], :])
+    return lρ, θ
+
+
 def rf2tρθ(rf: Tensor, rfmax: Tensor) -> Tuple[Tensor, Tensor]:
     """Convert real RF to tρ ≔ tan(ρ/ρ_max⋅π/2), and θ
 
     Usage:
         ``tρ, θ = rf2tρθ(rf, rfmax)``
     Inputs:
-        - ``rf``: `(N, xy, nT, (nCoils))`, RF pulse, Gauss, x for real, y for \
-          imag.
+        - ``rf``: `(N, xy, nT, (nCoils))`, RF pulse, Gauss, x: real, y: imag.
         - ``rfmax``: `(N, (nCoils))`, RF pulse, Gauss, x for real, y for imag.
     Outputs:
         - ``tρ``: `(N, 1, nT, (nCoils))`, tan(ρ/rfmax*π/2), [0, +∞).
-        - ``θ``: `(N, 1, nT, (nCoils))`, RF phase, [-π/2, π/2].
+        - ``θ``: `(N, 1, nT, (nCoils))`, RF phase, [-π, π).
 
     See Also:
         :func:`~mrphy.utils.tρθ2rf`
     """
     rfmax = rfmax[None] if rfmax.ndim == 0 else rfmax  # scalar to 1d-tensor
     tρ = (rf.norm(dim=1, keepdim=True)/rfmax[:, None, None, ...]*π/2).tan()
     θ = torch.atan2(rf[:, [1], :], rf[:, [0], :])
     return tρ, θ
 
 
-def rfclamp(rf: Tensor, rfmax: Tensor, eps: Number = 1e-7) -> Tensor:
+def rfclamp(rf: Tensor, rfmax: Tensor, *, eps: Number = 1e-7) -> Tensor:
     r"""Clamp RF to rfmax
 
     Usage:
-        ``rf = rfclamp(rf, rfmax)``
+        ``rf = rfclamp(rf, rfmax, *, eps)``
     Inputs:
         - ``rf``: `(N, xy, nT, (nCoils))`, RF pulse, Gauss, x for real, y for \
           imag.
         - ``rfmax``: `(N, (nCoils))`, RF pulse, Gauss, x for real, y for imag.
     Optionals:
         - ``eps``: effective `rfmax`, is `rfmax-eps`, numerical precession.
     Outputs:
@@ -190,15 +236,15 @@
     return rf.mul(((rfmax[:, None, None, ...]-eps)/rf_abs).clamp_(max=1))
 
 
 def s2g(s: Tensor, dt: Tensor = dt0) -> Tensor:
     r"""Compute gradients from slew rates.
 
     Usage:
-        ``g = s2g(s; dt)``
+        ``g = s2g(s, dt)``
 
     Inputs:
         - ``s``: `(N, xyz, nT)`, "Gauss/cm/Sec", Slew rate.
     Optionals:
         - ``dt``: `()` ⊻ `(N ⊻ 1,)`, "Sec", dwell time.
     Outputs:
         - ``g``: `(N, xyz, nT)`, "Gauss/cm", Gradient.
@@ -270,16 +316,15 @@
     Usage:
         ``rf = tρθ2rf(tρ, θ, rfmax)``
     Inputs:
         - ``tρ``: `(N, 1, nT, (nCoils))`, tan(ρ/rfmax*π/2), [0, +∞).
         - ``θ``: `(N, 1, nT, (nCoils))`, RF phase, [-π/2, π/2].
         - ``rfmax``: `(N, (nCoils))`, RF pulse, Gauss, x for real, y for imag.
     Outputs:
-        - ``rf``: `(N, xy, nT, (nCoils))`, RF pulse, Gauss, x for real, y for \
-          imag.
+        - ``rf``: `(N, xy, nT, (nCoils))`, RF pulse, Gauss, x: real, y: imag.
 
     See Also:
         :func:`~mrphy.utils.rf2tρθ`
     """
     rfmax = rfmax[None] if rfmax.ndim == 0 else rfmax
     rfmax = rfmax[:, None, None, ...]  # -> (N, 1, 1, (nCoils))
     return tρ.atan()/π*2*rfmax*torch.cat((θ.cos(), θ.sin()), dim=1)
```

### Comparing `mrphy-0.1.9/mrphy.egg-info/PKG-INFO` & `mrphy-0.2.0/mrphy.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,79 +1,79 @@
 Metadata-Version: 2.1
 Name: mrphy
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Pytorch based tool for MR physics simulations
 Home-page: https://github.com/tianrluo/MRphy.py
 Author: Tianrui Luo
 Author-email: tianrluo@umich.edu
 License: MIT
-Description: # MRphy.py
-        
-        A pytorch based MR simulator package.
-        [![](https://img.shields.io/badge/docs-stable-blue.svg)](https://tianrluo.github.io/MRphy.py/stable/index.html)
-        [![](https://img.shields.io/badge/docs-dev-blue.svg)](https://tianrluo.github.io/MRphy.py/dev/index.html)
-        [![codecov](https://codecov.io/gh/tianrluo/MRphy.py/branch/master/graph/badge.svg?token=83sKL5NADl)](https://codecov.io/gh/tianrluo/MRphy.py)
-        [![Actions Status](https://github.com/tianrluo/MRphy.py/workflows/Python%20package/badge.svg)](https://github.com/tianrluo/MRphy.py/actions)
-        
-        Infrastructure of:\
-        [Joint Design of RF and Gradient Waveforms via Auto-Differentiation for 3D Tailored Exitation in MRI](https://ieeexplore.ieee.org/document/9439482)\
-        (arXiv: [https://arxiv.org/abs/2008.10594](https://arxiv.org/abs/2008.10594))
-        
-        cite as:
-        
-        ```bib
-        @article{luo2021joint,
-          author={Luo, Tianrui and Noll, Douglas C. and Fessler, Jeffrey A. and Nielsen, Jon-Fredrik},
-          journal={IEEE Transactions on Medical Imaging}, 
-          title={Joint Design of RF and gradient waveforms via auto-differentiation for 3D tailored excitation in MRI}, 
-          year={2021},
-          volume={},
-          number={},
-          pages={1-1},
-          doi={10.1109/TMI.2021.3083104}}
-        ```
-        
-        For the `interpT` feature, consider citing:
-        ```bib
-        @inproceedings{luo2021MultiScale,
-          title={Multi-scale Accelerated Auto-differentiable Bloch-simulation based joint design of excitation RF and gradient waveforms},
-          booktitle={ISMRM},
-          pages={3958},
-          author={Tianrui Luo and Douglas C. Noll and Jeffrey A. Fessler and Jon-Fredrik Nielsen},
-          year={2021}
-        }
-        ```
-        
-        ## Branches
-        
-        - `master`: Stable;
-        - `dev`: Ocassionally `git squash`'d, `git push --force`'d;
-        - `dev_cache`: Constantly `git push --force`'d.
-        
-        Developments are mostly done on `dev_cache`; when they have passed local checks, `dev` will be `git rebase`'d to `dev_cache`, and sent for CI tests.
-        When enough updates have been accumulated, `dev` will be git squashed into one large commit, followed by having `master`-branch `git rebase`'d onto it.
-        
-        ## Installation
-        
-        ```sh
-        pip install mrphy
-        ```
-        
-        (The package is not yet sent to `conda`.)
-        
-        ## Demos
-        
-        Check out files under `./test`.
-        After installation, one can quickly play with the tests through:
-        
-        ```sh
-        pytest -s
-        ```
-        
-        Only basic demo is available in this early version.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# MRphy.py
+
+A pytorch based MR simulator package.
+[![](https://img.shields.io/badge/docs-stable-blue.svg)](https://tianrluo.github.io/MRphy.py/stable/index.html)
+[![](https://img.shields.io/badge/docs-dev-blue.svg)](https://tianrluo.github.io/MRphy.py/dev/index.html)
+[![codecov](https://codecov.io/gh/tianrluo/MRphy.py/branch/master/graph/badge.svg?token=83sKL5NADl)](https://codecov.io/gh/tianrluo/MRphy.py)
+[![Actions Status](https://github.com/tianrluo/MRphy.py/workflows/Python%20package/badge.svg)](https://github.com/tianrluo/MRphy.py/actions)
+
+Infrastructure of:\
+[Joint Design of RF and Gradient Waveforms via Auto-Differentiation for 3D Tailored Exitation in MRI](https://ieeexplore.ieee.org/document/9439482)\
+(arXiv: [https://arxiv.org/abs/2008.10594](https://arxiv.org/abs/2008.10594))
+
+cite as:
+
+```bib
+@article{luo2021joint,
+  author={Luo, Tianrui and Noll, Douglas C. and Fessler, Jeffrey A. and Nielsen, Jon-Fredrik},
+  journal={IEEE Transactions on Medical Imaging}, 
+  title={Joint Design of RF and gradient waveforms via auto-differentiation for 3D tailored excitation in MRI}, 
+  year={2021},
+  volume={},
+  number={},
+  pages={1-1},
+  doi={10.1109/TMI.2021.3083104}}
+```
+
+For the `interpT` feature, consider citing:
+```bib
+@inproceedings{luo2021MultiScale,
+  title={Multi-scale Accelerated Auto-differentiable Bloch-simulation based joint design of excitation RF and gradient waveforms},
+  booktitle={ISMRM},
+  pages={3958},
+  author={Tianrui Luo and Douglas C. Noll and Jeffrey A. Fessler and Jon-Fredrik Nielsen},
+  year={2021}
+}
+```
+
+## Branches
+
+- `master`: Stable;
+- `dev`: Ocassionally `git squash`'d, `git push --force`'d;
+- `dev_cache`: Constantly `git push --force`'d.
+
+Developments are mostly done on `dev_cache`; when they have passed local checks, `dev` will be `git rebase`'d to `dev_cache`, and sent for CI tests.
+When enough updates have been accumulated, `dev` will be git squashed into one large commit, followed by having `master`-branch `git rebase`'d onto it.
+
+## Installation
+
+```sh
+pip install mrphy
+```
+
+(The package is not yet sent to `conda`.)
+
+## Demos
+
+Check out files under `./test`.
+After installation, one can quickly play with the tests through:
+
+```sh
+pytest -s
+```
+
+Only basic demo is available in this early version.
```

### Comparing `mrphy-0.1.9/tests/test_mobjs.py` & `mrphy-0.2.0/tests/test_mobjs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,78 @@
+from copy import deepcopy
 import numpy as np
 import torch
 import pytest
 from torch import tensor, cuda
 
 from mrphy import γH, dt0, π, _slice
 from mrphy import mobjs
 
 # TODO:
 # unit_tests for objects `.to()` methods
 
 
+def _setup(T1_, T2, γ, device, dtype):
+    kw = {'dtype': dtype, 'device': device}
+    dt = dt0  # For test coverage, not using self.dt here.
+
+    N, Nd, nT = 1, (3, 3, 3), 512
+    nT = 512
+
+    # pulse: Sec; Gauss; Gauss/cm.
+    pulse_size = (N, 1, nT)
+    t = torch.arange(0, nT, **kw).reshape(pulse_size)
+    rf = 10*torch.cat([torch.cos(t/nT*2*π),                # (1,xy, nT)
+                       torch.sin(t/nT*2*π)], 1)
+    gr = torch.cat([torch.ones(pulse_size, **kw),
+                    torch.ones(pulse_size, **kw),
+                    10*torch.atan(t - round(nT/2))/π], 1)  # (1,xyz,nT)
+
+    # Pulse
+    p = mobjs.Pulse(rf=rf, gr=gr, dt=dt, **kw)
+    p = deepcopy(p)  # for pytest coverage
+    p = mobjs.Pulse(**(p.asdict(toNumpy=False)))
+
+    # SpinCube (SpinArray is implicitly tested via it)
+    shape = (N, *Nd)
+    mask = torch.zeros((1,)+Nd, device=device, dtype=torch.bool)
+    mask[0, :, 1, :], mask[0, 1, :, :] = True, True
+    fov, ofst = tensor([[3., 3., 3.]], **kw), tensor([[0., 0., 1.]], **kw)
+
+    T1_, T2 = T1_.to(**kw), T2.to(**kw)
+    cube = mobjs.SpinCube(shape, fov, mask=mask, T1_=T1_, γ=γ, **kw)
+    cube = deepcopy(cube)  # for pytest coverage
+    cube_dict = cube.asdict(toNumpy=False)
+    cube = mobjs.SpinCube(**{k: cube_dict[k] for
+                             k in ('shape', 'fov', 'mask', 'T1', 'γ'
+                                   )+tuple(kw.keys())})
+    cube.ofst = ofst  # separated for test coverage
+
+    cube.M_ = tensor([0., 1., 0.])
+    cube.T2 = T2.expand(cube.shape)  # for test coverage
+
+    M001, M100 = tensor([0., 0., 1.], **kw), tensor([1., 0., 0.], **kw)
+    crds_100 = cube.crds_([_slice, [0, 1], [1, 0], _slice, _slice])
+    cube.M_[crds_100] = M100
+    crds_001 = cube.crds_([_slice, [2, 1], [1, 2], _slice, _slice])
+    cube.M_[crds_001] = M001
+
+    return cube, p
+
+
+def to_np(x):
+    return x.detach().cpu().numpy()
+
+
 class Test_mobjs:
 
     device = torch.device('cuda' if cuda.is_available() else 'cpu')
     # device = torch.device('cpu')
-    dtype, atol = torch.float32, 1e-4
-    # dtype, atol = torch.float64, 1e-9
+    # dtype, atol = torch.float32, 1e-4
+    dtype, atol = torch.float64, 1e-9
     print(device)
 
     dkw = {'dtype': dtype, 'device': device}
 
     γ = γH.to(**dkw)  # Hz/Gauss
     dt = dt0.to(**dkw)  # Sec
 
@@ -27,66 +80,33 @@
     def np(x):
         return x.detach().cpu().numpy()
 
     def test_Examples(self):
         ''' for coverage :/ '''
         assert(isinstance(mobjs.Examples.pulse(), mobjs.Pulse))
         assert(isinstance(mobjs.Examples.spincube(), mobjs.SpinCube))
+        assert(isinstance(mobjs.Examples.spincube(), mobjs.SpinArray))
         return
 
     def test_mobjs(self):
-        kw, atol = self.dkw, self.atol
-        γ, dt = self.γ, dt0  # For test coverage, not using self.dt here.
-
-        N, Nd, nT = 1, (3, 3, 3), 512
-        nT = 512
-
-        # pulse: Sec; Gauss; Gauss/cm.
-        pulse_size = (N, 1, nT)
-        t = torch.arange(0, nT, **kw).reshape(pulse_size)
-        rf = 10*torch.cat([torch.cos(t/nT*2*π),                # (1,xy, nT)
-                           torch.sin(t/nT*2*π)], 1)
-        gr = torch.cat([torch.ones(pulse_size, **kw),
-                        torch.ones(pulse_size, **kw),
-                        10*torch.atan(t - round(nT/2))/π], 1)  # (1,xyz,nT)
-
-        # Pulse
-        p = mobjs.Pulse(rf=rf, gr=gr, dt=dt, **kw)
+        T1_, T2 = tensor([[1.]]), tensor([[4e-2]])
+        cube, p = _setup(T1_, T2, self.γ, device=self.device, dtype=self.dtype)
         assert(p.is_cuda == (p.device.type == 'cuda'))
-        p = mobjs.Pulse(**(p.asdict(toNumpy=False)))
+        assert(cube.is_cuda == (cube.device.type == 'cuda'))
+        assert(cube.dim() == len(cube.shape))
+        return
 
-        # SpinCube (SpinArray is implicitly tested via it)
-        shape = (N, *Nd)
-        mask = torch.zeros((1,)+Nd, device=self.device, dtype=torch.bool)
-        mask[0, :, 1, :], mask[0, 1, :, :] = True, True
-        fov, ofst = tensor([[3., 3., 3.]], **kw), tensor([[0., 0., 1.]], **kw)
-        T1_, T2 = tensor([[1.]], **kw), tensor([[4e-2]], **kw)
+    def test_applypulse(self):
+        atol = self.atol
 
-        cube = mobjs.SpinCube(shape, fov, mask=mask, T1_=T1_, γ=γ, **kw)
-        assert(cube.is_cuda == (cube.device.type == 'cuda'))
-        cube_dict = cube.asdict(toNumpy=False)
-        cube = mobjs.SpinCube(**{k: cube_dict[k] for
-                                 k in ('shape', 'fov', 'mask', 'T1', 'γ'
-                                       )+tuple(kw.keys())})
-        cube.ofst = ofst  # separated for test coverage
-
-        cube.M_ = tensor([0., 1., 0.])
-        assert(cube.dim() == len(shape))
-        cube.T2 = T2.expand(cube.shape)  # for test coverage
-
-        M001, M100 = tensor([0., 0., 1.], **kw), tensor([1., 0., 0.], **kw)
-        crds_100 = cube.crds_([_slice, [0, 1], [1, 0], _slice, _slice])
-        cube.M_[crds_100] = M100
-        crds_001 = cube.crds_([_slice, [2, 1], [1, 2], _slice, _slice])
-        cube.M_[crds_001] = M001
+        T1_, T2 = tensor([[1.]]), tensor([[4e-2]])
+        cube, p = _setup(T1_, T2, self.γ, device=self.device, dtype=self.dtype)
 
         # gr_x/gr_y == 1 Gauss/cm cancels Δf[1, :, 0]/[1, 0, :] respectively
-        loc = cube.loc
-
-        cube.Δf = torch.sum(-loc[0:1, :, :, :, 0:2], dim=-1) * γ
+        cube.Δf = torch.sum(-cube.loc[0:1, :, :, :, 0:2], dim=-1) * cube.γ
 
         Mres1a = cube.applypulse(p, doEmbed=True)
         cube.applypulse(p, doEmbed=True, doRelax=False, doUpdate=True)
         Mres1b = cube.M
 
         # assertion
         Mo0a = np.array(
@@ -98,19 +118,46 @@
             [[[0.584337330324116,  0.686096989146395, 0.433382978292808],
               [0.404188676945936,  0.217027890590635, -0.888555236400348],
               [-0.703691265981316, 0.694384487290747, -0.150495136106067]]])
 
         Mrefa = pytest.approx(Mo0a, abs=atol)
         Mrefb = pytest.approx(Mo0b, abs=atol)
 
-        assert(self.np(Mres1a[0:1, 1, :, 1, :]) == Mrefa)
-        assert(self.np(Mres1a[0:1, :, 1, 1, :]) == Mrefa)
+        assert(to_np(Mres1a[0:1, 1, :, 1, :]) == Mrefa)
+        assert(to_np(Mres1a[0:1, :, 1, 1, :]) == Mrefa)
+
+        assert(to_np(Mres1b[0:1, 1, :, 1, :]) == Mrefb)
+        assert(to_np(Mres1b[0:1, :, 1, 1, :]) == Mrefb)
+
+        return
+
+    def test_freeprec(self):
+        dkw, atol = self.dkw, self.atol
+
+        E1, E2 = tensor([[0.5]], **dkw), tensor([[0.5]], **dkw)
+
+        # scalar dur, T1, T2
+        dur = torch.tensor(0.5, **dkw)
+        T1, T2 = -dur/torch.log(E1), -dur/torch.log(E2)  # ()
+
+        cube, _ = _setup(T1, T2, self.γ, device=self.device, dtype=self.dtype)
+        shape = cube.shape
+        _, nx, _, nz = shape
+        _Δf = tensor([[[1/4/dur], [-1/4/dur], [1]]], **dkw)
+        Δf = _Δf.repeat(1, 3, 1, 3)
+        cube.Δf = Δf
+
+        Mres1a = cube.freeprec(dur, doEmbed=True)
+
+        # assertion
+        Mo0a = np.array([[[0., -0.5, 0.5], [-0.5, 0, 0.5], [0., 0., 1.]]])
+
+        Mrefa = pytest.approx(Mo0a, abs=atol)
 
-        assert(self.np(Mres1b[0:1, 1, :, 1, :]) == Mrefb)
-        assert(self.np(Mres1b[0:1, :, 1, 1, :]) == Mrefb)
+        assert(to_np(Mres1a[0:1, 1, :, 1, :]) == Mrefa)
 
         return
 
     def test_PulseInterpT(self):
         dkw, atol = self.dkw, self.atol
         dt = dt0
         dt_n = dt*5
@@ -138,16 +185,16 @@
         rf_ref = pytest.approx(np.array([[[0.04, 0.09],
                                           [0.06, 0.01]]]), abs=atol)
 
         gr_ref = pytest.approx(np.array([[[0.04, 0.09],
                                           [0.06, 0.01],
                                           [0.1,   0.1]]]), abs=atol)
 
-        assert(self.np(p_new.rf) == rf_ref)
-        assert(self.np(p_new.gr) == gr_ref)
+        assert(to_np(p_new.rf) == rf_ref)
+        assert(to_np(p_new.gr) == gr_ref)
 
         return
 
 
 if __name__ == '__main__':
     tmp = Test_mobjs()
-    tmp.test_mobjs()
+    tmp.test_applypulse()
```

### Comparing `mrphy-0.1.9/tests/test_sims.py` & `mrphy-0.2.0/tests/test_sims.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from mrphy import beffective, sims, slowsims
 
 import time
 
 
 class Test_sims:
 
-    device = torch.device('cuda:1' if cuda.is_available() else 'cpu')
+    device = torch.device('cuda' if cuda.is_available() else 'cpu')
     # device = torch.device('cpu')
     # dtype, atol = torch.float32, 1e-4
     dtype, atol = torch.float64, 1e-9
 
     dkw = {'dtype': dtype, 'device': device}
 
     print(device)
@@ -22,15 +22,15 @@
     dt = dt0.to(**dkw)   # Sec
 
     def test_blochsims(self):
         """
         *Note*:
         This test relies on the correctness of `test_slowsims.py`.
         """
-        f_t2np = lambda x: x.detach().clone().cpu().numpy()  # noqa: E731
+        f_t2np = lambda x: x.detach().clone().cpu().numpy()
 
         print('\n')
         dkw, atol = self.dkw, self.atol
         γ, dt = self.γ, self.dt
 
         # spins  # (1,nM,xyz)
         M0 = torch.rand((1, 16*16*2, 3), **dkw)
@@ -57,32 +57,33 @@
         rf = 10*torch.cat([torch.cos(t/nT*2*π),  # (1,xy,nT,nCoils)
                            torch.sin(t/nT*2*π)], 1)[..., None]
         gr = torch.cat([torch.ones(pulse_size, **dkw),
                         torch.zeros(pulse_size, **dkw),
                         10*torch.atan(t - round(nT/2))/π], 1)  # (1,xyz,nT)
 
         # rf.requires_grad, gr.requires_grad = True, True
-        beff = beffective.rfgr2beff(rf, gr, loc, Δf, b1Map, γ)
+        beff = beffective.rfgr2beff(rf, gr, loc, Δf=Δf, b1Map=b1Map, γ=γ)
         beff.requires_grad = True
 
         # Check handling of 1-coil `rf`, `b1Map` that omitted the `nCoils` dim
-        beff_missing_dim = beffective.rfgr2beff(rf[..., 0], gr, loc, Δf,
-                                                b1Map[..., 0], γ)
+        beff_missing_dim = beffective.rfgr2beff(rf[..., 0], gr, loc, Δf=Δf,
+                                                b1Map=b1Map[..., 0], γ=γ)
 
         # %% sim
         print('\nblochsim tests:')
         t = time.time()
         Mo_1a = slowsims.blochsim(M0, beff, T1=T1, T2=T2, γ=γ, dt=dt)
         print('forward: slowsims.blochsim', time.time() - t)
 
         res1a = torch.sum(Mo_1a)
         t = time.time()
         res1a.backward()  # keep graph to check `bar.backward()`
         print('backward: slowsims.blochsim', time.time() - t)
         grad_M0_1a = f_t2np(M0.grad)
+        # (..., nT, xyz) → (..., xyz, nT)
         grad_beff_1a = f_t2np(beff.grad)
 
         M0.grad, beff.grad = None, None
 
         t = time.time()
         Mo_2a = sims.blochsim(M0, beff, T1=T1, T2=T2, γ=γ, dt=dt)
         print('forward: sims.blochsim', time.time() - t)
@@ -106,14 +107,15 @@
         # %% sim w/o relaxations
         print('\nblochsim tests (no relaxations):')
         Mo_1b = slowsims.blochsim(M0, beff, T1=None, T2=None, γ=γ, dt=dt)
 
         res1b = torch.sum(Mo_1b)
         res1b.backward()  # keep graph to check `bar.backward()`
         grad_M0_1b = f_t2np(M0.grad)
+        # (..., nT, xyz) → (..., xyz, nT)
         grad_beff_1b = f_t2np(beff.grad)
 
         # dur_f, dur_b, n_repeat = 0., 0., 1000
         dur_f, dur_b, n_repeat = 0., 0., 1
         for _ in range(n_repeat):
             M0.grad, beff.grad = None, None
 
@@ -136,11 +138,67 @@
 
         M0.grad, beff.grad = None, None
 
         # %% assertion
         assert(pytest.approx(grad_M0_1b, abs=atol) == grad_M0_2b)
         assert(pytest.approx(grad_beff_1b, abs=atol) == grad_beff_2b)
 
+    def test_freeprec(self):
+        """
+        *Note*:
+        This test relies on the correctness of `test_slowsims.py`.
+        """
+        f_t2np = lambda x: x.detach().clone().cpu().numpy()
+
+        print('\n')
+        dkw, atol = self.dkw, self.atol
+        γ = self.γ
+
+        # spins  # (1,nM,xyz)
+        M0 = torch.rand((1, 16*16*2, 3), **dkw)
+        N, nM = M0.shape[0], M0.shape[1]
+        Nd = (nM,)
+
+        M0.requires_grad = True
+
+        # parameters: Sec; cm.
+        dur = torch.tensor(0.5, **dkw)
+        T1, T2 = tensor([[1.]], **dkw), tensor([[4e-2]], **dkw)
+
+        loc_x = torch.linspace(-1., 1., steps=nM, **dkw).reshape((N,)+Nd)
+
+        Δf = -loc_x * γ  # gr_x==1 Gauss/cm cancels Δf
+
+        # %% sim
+        print('\nfreeprec tests:')
+        t = time.time()
+        Mo1 = slowsims.freeprec(M0, dur, T1=T1, T2=T2, Δf=Δf)
+        print('forward: slowsims.freeprec', time.time() - t)
+
+        res1 = torch.sum(Mo1)
+        t = time.time()
+        res1.backward()  # keep graph to check `bar.backward()`
+        print('backward: slowsims.freeprec', time.time() - t)
+        grad_M0_1 = f_t2np(M0.grad)
+
+        M0.grad = None
+
+        t = time.time()
+        Mo2 = sims.freeprec(M0, dur, T1=T1, T2=T2, Δf=Δf)
+        print('forward: sims.freeprec', time.time() - t)
+
+        res2 = torch.sum(Mo2)
+        t = time.time()
+        res2.backward()  # keep graph to check `bar.backward()`
+        print('backward: sims.blochsim', time.time() - t)
+        grad_M0_2 = f_t2np(M0.grad)
+
+        M0.grad = None
+
+        assert(pytest.approx(grad_M0_1, abs=atol) == grad_M0_2)
+        return
+
 
 if __name__ == '__main__':
     tmp = Test_sims()
     tmp.test_blochsims()
+    tmp.test_freeprec()
```

### Comparing `mrphy-0.1.9/tests/test_slowsims.py` & `mrphy-0.2.0/tests/test_slowsims.py`

 * *Files 16% similar despite different names*

```diff
@@ -55,24 +55,24 @@
                            torch.sin(t/nT*2*π)], 1)[..., None]
         gr = torch.cat([torch.ones(pulse_size, **dkw),
                         torch.zeros(pulse_size, **dkw),
                         10*torch.atan(t - round(nT/2))/π], 1)  # (1,xyz,nT)
 
         rf.requires_grad, gr.requires_grad = True, True
 
-        beff = beffective.rfgr2beff(rf, gr, loc, Δf, b1Map, γ)
+        beff = beffective.rfgr2beff(rf, gr, loc, Δf=Δf, b1Map=b1Map, γ=γ)
 
         A, B = beffective.beff2ab(beff, E1=E1, E2=E2, γ=γ, dt=dt)
 
         # sim
         Mo1 = slowsims.blochsim(M0, beff, T1=T1, T2=T2, γ=γ, dt=dt)
 
         Mo2, Mo_tmp = M0.clone(), M0.clone()
         for t in range(nT):
-            Mo2, _ = slowsims.blochsim_1step(Mo2, Mo_tmp, beff[..., t],
+            Mo2, _ = slowsims.blochsim_1step(Mo2, Mo_tmp, beff[..., t, :],
                                              E1, E1_1, E2, γ2πdt)
 
         Mo3 = slowsims.blochsim_ab(M0, A, B)
 
         # assertion
         Mo0 = np.array(
             [[[0.559535641648385,  0.663342640621335, 0.416341441715101],
@@ -91,11 +91,37 @@
 
         bar = torch.sum(Mo3)
         bar.backward()
         rf_grad2, gr_grad2 = self.np(rf.grad), self.np(gr.grad)
         assert(rf_grad1 == pytest.approx(rf_grad2, abs=atol))
         assert(gr_grad1 == pytest.approx(gr_grad2, abs=atol))
 
+        return
+
+    def test_freeprec(self):
+
+        dkw, atol = self.dkw, self.atol
+
+        # spins  # (1,nM,xyz)
+        Mi = tensor([[[1., 0., 0.], [0., 1., 0.], [0., 0., 1.]]], **dkw)
+
+        E1, E2 = tensor([[0.5]], **dkw), tensor([[0.5]], **dkw)  # (1,1)
+
+        # scalar dur, T1, T2
+        dur = torch.tensor(0.5, **dkw)
+        T1, T2 = -dur/torch.log(E1), -dur/torch.log(E2)  # ()
+
+        Δf = tensor([[1/4/dur, -1/4/dur, 1]], **dkw)  # (1, nM) quater-circle
+
+        Mo = slowsims.freeprec(Mi, dur, T1=T1, T2=T2, Δf=Δf)
+
+        Mo0 = np.array([[[0., -0.5, 0.5], [-0.5, 0, 0.5], [0., 0., 1.]]])
+        Mref = pytest.approx(Mo0, abs=atol)
+
+        assert(self.np(Mo) == Mref)
+        return
+
 
 if __name__ == '__main__':
     tmp = Test_slowsims()
     tmp.test_blochsims()
+    tmp.test_freeprec()
```

### Comparing `mrphy-0.1.9/tests/test_utils.py` & `mrphy-0.2.0/tests/test_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import torch
 import pytest
 from torch import tensor, cuda
 
-from mrphy import γH, dt0, rfmax0, smax0
+from mrphy import γH, dt0, rfmax0, smax0, __CUPY_IS_AVAILABLE__
 from mrphy import utils
-if torch.cuda.is_available():
+if __CUPY_IS_AVAILABLE__:
     import cupy as cp
 
 
 # TODO:
 # unit_tests for other utils functions
 def to_np(x):
     return x.detach().cpu().numpy()
@@ -51,34 +51,44 @@
                pytest.approx(to_np(k), abs=atol))
 
         assert(to_np(gTx) == pytest.approx(to_np(gTx1), abs=atol))
         return
 
     def test_rc_rf(self):
         shape, atol = (1, 2, 5), self.atol
-        rf_r_0_np = np.random.rand(*shape).astype(np.double)
+        tmp = np.random.rand(*shape)
+        rf_r_0_np = tmp.astype(np.double, copy=False)
         rf_r_1_np = utils.rf_c2r(utils.rf_r2c(rf_r_0_np))
         assert(rf_r_0_np == pytest.approx(rf_r_1_np, abs=atol))
 
-        if torch.cuda.is_available():
-            rf_r_0_cp = cp.random.rand(*shape).astype(cp.double)
+        if __CUPY_IS_AVAILABLE__:
+            rf_r_0_cp = tmp.astype(cp.double, copy=False)
             rf_r_1_cp = utils.rf_c2r(utils.rf_r2c(rf_r_0_cp))
             assert(cp.asnumpy(rf_r_0_cp) ==
                    pytest.approx(cp.asnumpy(rf_r_1_cp), abs=atol))
         return
 
     def test_rfclamptan(self):
         shape, rfmax, atol = (1, 2, 10), rfmax0, self.atol
         rf0 = utils.rfclamp(rfmax0*((torch.rand(shape)-0.5)*4), rfmax)
         assert(torch.all(rf0.norm(dim=1) <= rfmax))
         tρ, θ = utils.rf2tρθ(rf0, rfmax)
         rf1 = utils.tρθ2rf(tρ, θ, rfmax)
         assert(to_np(rf0) == pytest.approx(to_np(rf1), abs=atol))
         return
 
+    def test_rfclamplogit(self):
+        shape, rfmax, atol = (1, 2, 10), rfmax0, self.atol
+        rf0 = utils.rfclamp(rfmax0*((torch.rand(shape)-0.5)*4), rfmax)
+        assert(torch.all(rf0.norm(dim=1) <= rfmax))
+        lρ, θ = utils.rf2lρθ(rf0, rfmax)
+        rf1 = utils.lρθ2rf(lρ, θ, rfmax)
+        assert(to_np(rf0) == pytest.approx(to_np(rf1), abs=atol))
+        return
+
     def test_sclamptan(self):
         shape, smax, atol = (1, 3, 10), smax0, self.atol
         s0 = utils.sclamp(smax0*((torch.rand(shape)-0.5)*4), smax)
         assert(torch.all(s0.abs() <= smax))
         s1 = utils.ts2s(utils.s2ts(s0, smax), smax)
         assert(to_np(s0) == pytest.approx(to_np(s1), abs=atol))
         return
```

