# Comparing `tmp/eztils-0.3.6.tar.gz` & `tmp/eztils-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eztils-0.3.6.tar", max compression
+gzip compressed data, was "eztils-0.4.0.tar", max compression
```

## Comparing `eztils-0.3.6.tar` & `eztils-0.4.0.tar`

### file list

```diff
@@ -1,10 +1,13 @@
--rw-r--r--   0        0        0     1075 2023-07-14 01:17:51.780650 eztils-0.3.6/LICENSE
--rw-r--r--   0        0        0    12714 2023-07-14 01:18:58.083876 eztils-0.3.6/README.md
--rw-r--r--   0        0        0      625 2023-07-14 01:17:51.780650 eztils-0.3.6/eztils/__init__.py
--rw-r--r--   0        0        0     1446 2023-07-14 01:17:51.780650 eztils-0.3.6/eztils/utils/__init__.py
--rw-r--r--   0        0        0     5798 2023-07-14 01:17:51.780650 eztils-0.3.6/eztils/utils/arrays.py
--rw-r--r--   0        0        0     2288 2023-07-14 01:17:51.780650 eztils-0.3.6/eztils/utils/logging.py
--rw-r--r--   0        0        0      962 2023-07-14 01:17:51.780650 eztils-0.3.6/eztils/utils/model_wrappers.py
--rw-r--r--   0        0        0     1028 2023-07-14 01:17:51.780650 eztils-0.3.6/eztils/utils/structures.py
--rw-r--r--   0        0        0     3457 2023-07-14 01:18:57.575882 eztils-0.3.6/pyproject.toml
--rw-r--r--   0        0        0    13749 1970-01-01 00:00:00.000000 eztils-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-14 01:17:51.780650 eztils-0.4.0/LICENSE
+-rw-r--r--   0        0        0    12710 2023-07-14 01:52:52.320035 eztils-0.4.0/README.md
+-rw-r--r--   0        0        0      542 2023-07-14 02:09:17.596159 eztils-0.4.0/eztils/__init__.py
+-rw-r--r--   0        0        0      808 2023-07-14 02:09:17.600159 eztils-0.4.0/eztils/default/__init__.py
+-rw-r--r--   0        0        0     2341 2023-07-14 01:58:12.724178 eztils-0.4.0/eztils/default/logging.py
+-rw-r--r--   0        0        0      112 2023-07-14 02:09:16.540172 eztils-0.4.0/eztils/default/math.py
+-rw-r--r--   0        0        0     1091 2023-07-14 01:58:12.704178 eztils-0.4.0/eztils/default/structures.py
+-rw-r--r--   0        0        0      265 2023-07-14 02:09:16.960167 eztils-0.4.0/eztils/torch/__init__.py
+-rw-r--r--   0        0        0      688 2023-07-14 02:09:17.632159 eztils-0.4.0/eztils/torch/utils/__init__.py
+-rw-r--r--   0        0        0     5667 2023-07-14 02:09:17.640159 eztils-0.4.0/eztils/torch/utils/arrays.py
+-rw-r--r--   0        0        0      962 2023-07-14 01:17:51.780650 eztils-0.4.0/eztils/torch/utils/model_wrappers.py
+-rw-r--r--   0        0        0     3457 2023-07-14 02:09:10.176249 eztils-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    13743 1970-01-01 00:00:00.000000 eztils-0.4.0/PKG-INFO
```

### Comparing `eztils-0.3.6/LICENSE` & `eztils-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eztils-0.3.6/README.md` & `eztils-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/ezhang7423/eztils/blob/master/.pre-commit-config.yaml)
 [![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/ezhang7423/eztils/releases)
 [![License](https://img.shields.io/github/license/ezhang7423/eztils)](https://github.com/ezhang7423/eztils/blob/master/LICENSE)
 
-eds torch stuff.
+eds utilities.
 
 torch, torchvision, and numpy are required but not specified, so as to be flexible with any environment this package is installed in.
 
 </div>
 
 ## Installation
 
@@ -393,15 +393,15 @@
 This project is licensed under the terms of the `MIT` license. See [LICENSE](https://github.com/ezhang7423/eztils/blob/master/LICENSE) for more details.
 
 ## 📃 Citation
 
 ```bibtex
 @misc{eztils,
   author = {ezhang7423},
-  title = {eds torch stuff},
+  title = {eds utilities},
   year = {2023},
   publisher = {GitHub},
   journal = {GitHub repository},
   howpublished = {\url{https://github.com/ezhang7423/eztils}}
 }
 ```
```

### Comparing `eztils-0.3.6/eztils/utils/arrays.py` & `eztils-0.4.0/eztils/torch/utils/arrays.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from typing import Any, Union
 
 import pdb
 
 import numpy as np
 import torch
 
+from eztils.default import apply_dict
+from eztils.default.math import normalize
+
 DTYPE = torch.float
 DEVICE = "cuda:0"
 
 # -----------------------------------------------------------------------------#
 # ------------------------------ numpy <--> torch -----------------------------#
 # -----------------------------------------------------------------------------#
 
@@ -53,27 +56,14 @@
     for field in batch._fields:
         val = getattr(batch, field)
         val = apply_dict(fn, val) if type(val) is dict else fn(val)
         batched_vals.append(val)
     return type(batch)(*batched_vals)
 
 
-def apply_dict(fn, d, *args, **kwargs):
-    return {k: fn(v, *args, **kwargs) for k, v in d.items()}
-
-
-def normalize(x):
-    """
-    scales `x` to [0, 1]
-    """
-    x = x - x.min()
-    x = x / x.max()
-    return x
-
-
 def to_img(x):
     normalized = normalize(x)
     array = to_np(normalized)
     array = np.transpose(array, (1, 2, 0))
     return (array * 255).astype(np.uint8)
 
 
@@ -84,25 +74,20 @@
 
 
 def batch_to_device(batch, device="cuda:0"):
     vals = [to_device(getattr(batch, field), device) for field in batch._fields]
     return type(batch)(*vals)
 
 
-def _to_str(num):
-    if num >= 1e6:
-        return f"{(num/1e6):.2f} M"
-    else:
-        return f"{(num/1e3):.2f} k"
-
-
 # -----------------------------------------------------------------------------#
 # ----------------------------- parameter counting ----------------------------#
 # -----------------------------------------------------------------------------#
 # https://github.com/allenai/allenact/blob/f00445e4ae8724ccc001b3300af5c56a7f882614/allenact/utils/tensor_utils.py#L1
+
+
 def to_device_recursively(
     input: Any, device: Union[str, torch.device, int], inplace: bool = True
 ) -> Any:
     """Recursively places tensors on the appropriate device."""
     if input is None:
         return input
     elif isinstance(input, torch.Tensor):
@@ -160,20 +145,26 @@
 
 def param_to_module(param):
     module_name = param[::-1].split(".", maxsplit=1)[-1][::-1]
     return module_name
 
 
 def report_parameters(model, topk=10):
+    def _to_str(num):
+        if num >= 1e6:
+            return f"{(num/1e6):.2f} M"
+        else:
+            return f"{(num/1e3):.2f} k"
+
     counts = {k: p.numel() for k, p in model.named_parameters()}
     n_parameters = sum(counts.values())
     print(f"[ utils/arrays ] Total parameters: {_to_str(n_parameters)}")
 
     modules = dict(model.named_modules())
-    sorted_keys = sorted(counts, key=lambda x: -counts[x])  # type: ignore
+    sorted_keys = sorted(counts, key=lambda x: -counts[x])
     max_length = max([len(k) for k in sorted_keys])
     for i in range(topk):
         key = sorted_keys[i]
         count = counts[key]
         module = param_to_module(key)
         print(" " * 8, f"{key:10}: {_to_str(count)} | {modules[module]}")
```

### Comparing `eztils-0.3.6/eztils/utils/logging.py` & `eztils-0.4.0/eztils/default/logging.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,17 @@
                 return self.tree.add(label)  # type: ignore
 
     def type_fmt(obj):
         # get string within single quotes regex
         import re
 
         m = re.search(r"'(.*?)'", str(type(obj)))
-        return m.group(1)
+        if m is not None:
+            return m.group(1)
+        return None  #
 
     def add_children(obj: object, root: Tree) -> None:
         if isinstance(obj, dict):
             dict_node = root.add(f"dict")
             for key in obj.keys():
                 add_children(obj[key], dict_node.add(f"[bold]{key}[/bold]"))
         elif isinstance(obj, list) or isinstance(obj, np.ndarray):
```

### Comparing `eztils-0.3.6/eztils/utils/model_wrappers.py` & `eztils-0.4.0/eztils/torch/utils/model_wrappers.py`

 * *Files identical despite different names*

### Comparing `eztils-0.3.6/eztils/utils/structures.py` & `eztils-0.4.0/eztils/default/structures.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-class AttriDict(dict):
+from typing import Any, Dict, MutableMapping
+
+
+class AttriDict(dict):  # type: ignore
     """
     A dict which is accessible via attribute dot notation
     https://stackoverflow.com/a/41514848
     https://stackoverflow.com/a/14620633
     """
 
     DICT_RESERVED_KEYS = list(vars(dict).keys())
```

### Comparing `eztils-0.3.6/pyproject.toml` & `eztils-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry_core>=1.0.0"]
 
 [tool.poetry]
 authors = ["ezhang7423 <ezhang7423@student.palomar.edu>"]
-description = "eds torch stuff"
+description = "eds utilities"
 homepage = "https://github.com/ezhang7423/eztils"
 license = "MIT"
 name = "eztils"
 readme = "README.md"
 repository = "https://github.com/ezhang7423/eztils"
-version = "0.3.6"
+version = "0.4.0"
 
 # Keywords description https://python-poetry.org/docs/pyproject/#keywords
 keywords = [] #! Update me
 
 # Pypi classifiers: https://pypi.org/classifiers/
 classifiers = [
   #! Update me
@@ -26,28 +26,28 @@
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
 ]
 
 [tool.poetry.dependencies]
-einops = "^0.6.0"
-loguru = "^0.6.0"
 python = "^3.8"
 rich = "^13.3.3"
-tqdm = "^4.65.0"
 numpy = "^1.24.3"
+loguru = "^0.7.0"
+einops = "^0.6.1"
+tqdm = "^4.65.0"
 
 [tool.poetry.group.dev.dependencies]
 bandit = "^1.7.5"
 black = "^23.3.0"
 coverage = "^7.2.2"
 coverage-badge = "^1.1.0"
 darglint = "^1.8.1"
-isort = {extras = ["colors"], version = "^5.12.0"}
+isort = { extras = ["colors"], version = "^5.12.0" }
 mypy = "^1.1.1"
 mypy-extensions = "^1.0.0"
 pre-commit = "^3.2.1"
 pydocstyle = "^6.3.0"
 pylint = "^2.17.1"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
```

### Comparing `eztils-0.3.6/PKG-INFO` & `eztils-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: eztils
-Version: 0.3.6
-Summary: eds torch stuff
+Version: 0.4.0
+Summary: eds utilities
 Home-page: https://github.com/ezhang7423/eztils
 License: MIT
 Author: ezhang7423
 Author-email: ezhang7423@student.palomar.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -13,16 +13,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: einops (>=0.6.0,<0.7.0)
-Requires-Dist: loguru (>=0.6.0,<0.7.0)
+Requires-Dist: einops (>=0.6.1,<0.7.0)
+Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: rich (>=13.3.3,<14.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Repository, https://github.com/ezhang7423/eztils
 Description-Content-Type: text/markdown
 
 # eztils
@@ -35,15 +35,15 @@
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/ezhang7423/eztils/blob/master/.pre-commit-config.yaml)
 [![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/ezhang7423/eztils/releases)
 [![License](https://img.shields.io/github/license/ezhang7423/eztils)](https://github.com/ezhang7423/eztils/blob/master/LICENSE)
 
-eds torch stuff.
+eds utilities.
 
 torch, torchvision, and numpy are required but not specified, so as to be flexible with any environment this package is installed in.
 
 </div>
 
 ## Installation
 
@@ -420,15 +420,15 @@
 This project is licensed under the terms of the `MIT` license. See [LICENSE](https://github.com/ezhang7423/eztils/blob/master/LICENSE) for more details.
 
 ## 📃 Citation
 
 ```bibtex
 @misc{eztils,
   author = {ezhang7423},
-  title = {eds torch stuff},
+  title = {eds utilities},
   year = {2023},
   publisher = {GitHub},
   journal = {GitHub repository},
   howpublished = {\url{https://github.com/ezhang7423/eztils}}
 }
 ```
```

