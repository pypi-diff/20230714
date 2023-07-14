# Comparing `tmp/unbiasedness-0.1.0.tar.gz` & `tmp/unbiasedness-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unbiasedness-0.1.0.tar", max compression
+gzip compressed data, was "unbiasedness-0.1.1.tar", max compression
```

## Comparing `unbiasedness-0.1.0.tar` & `unbiasedness-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-01-10 19:43:48.988798 unbiasedness-0.1.0/LICENSE
--rw-r--r--   0        0        0      122 2023-07-14 15:50:24.241842 unbiasedness-0.1.0/README.md
--rw-r--r--   0        0        0      542 2023-07-14 15:49:53.336982 unbiasedness-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      172 2023-04-25 12:59:32.903726 unbiasedness-0.1.0/unbiasedness/__init__.py
--rw-r--r--   0        0        0     9613 2023-06-06 16:50:29.477481 unbiasedness-0.1.0/unbiasedness/bootstrap.py
--rw-r--r--   0        0        0     4048 2023-04-04 18:09:22.076998 unbiasedness-0.1.0/unbiasedness/numba_jit.py
--rw-r--r--   0        0        0    13676 2023-06-13 20:48:59.137868 unbiasedness-0.1.0/unbiasedness/table.py
--rw-r--r--   0        0        0     2553 2023-06-06 16:50:22.783427 unbiasedness-0.1.0/unbiasedness/unbiasedness.py
--rw-r--r--   0        0        0     9262 2023-06-06 13:27:16.279373 unbiasedness-0.1.0/unbiasedness/windows.py
--rw-r--r--   0        0        0      774 1970-01-01 00:00:00.000000 unbiasedness-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-01-10 19:43:48.988798 unbiasedness-0.1.1/LICENSE
+-rw-r--r--   0        0        0      122 2023-07-14 15:50:24.241842 unbiasedness-0.1.1/README.md
+-rw-r--r--   0        0        0      538 2023-07-14 16:25:01.143928 unbiasedness-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      172 2023-04-25 12:59:32.903726 unbiasedness-0.1.1/unbiasedness/__init__.py
+-rw-r--r--   0        0        0     9613 2023-06-06 16:50:29.477481 unbiasedness-0.1.1/unbiasedness/bootstrap.py
+-rw-r--r--   0        0        0     4048 2023-04-04 18:09:22.076998 unbiasedness-0.1.1/unbiasedness/numba_jit.py
+-rw-r--r--   0        0        0    13676 2023-06-13 20:48:59.137868 unbiasedness-0.1.1/unbiasedness/table.py
+-rw-r--r--   0        0        0     2553 2023-06-06 16:50:22.783427 unbiasedness-0.1.1/unbiasedness/unbiasedness.py
+-rw-r--r--   0        0        0     9404 2023-07-14 16:24:27.262559 unbiasedness-0.1.1/unbiasedness/windows.py
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 unbiasedness-0.1.1/PKG-INFO
```

### Comparing `unbiasedness-0.1.0/LICENSE` & `unbiasedness-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unbiasedness-0.1.0/pyproject.toml` & `unbiasedness-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "unbiasedness"
-version = "0.1.0"
+version = "0.1.1"
 description = "Functions for estimating unbiasedness regressions."
 authors = ["Vincent Grégoire <vincent.gregoire@gmail.com>"]
 license = "Apache License, Version 2"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-pandas = "^2.0.3"
-numpy = "^1.25.1"
+pandas = "^2.0"
+numpy = "^1.24"
 statsmodels = "^0.14.0"
 numba = "^0.57.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.7.0"
 pytest = "^7.4.0"
 jupyter = "^1.0.0"
```

### Comparing `unbiasedness-0.1.0/unbiasedness/bootstrap.py` & `unbiasedness-0.1.1/unbiasedness/bootstrap.py`

 * *Files identical despite different names*

### Comparing `unbiasedness-0.1.0/unbiasedness/numba_jit.py` & `unbiasedness-0.1.1/unbiasedness/numba_jit.py`

 * *Files identical despite different names*

### Comparing `unbiasedness-0.1.0/unbiasedness/table.py` & `unbiasedness-0.1.1/unbiasedness/table.py`

 * *Files identical despite different names*

### Comparing `unbiasedness-0.1.0/unbiasedness/unbiasedness.py` & `unbiasedness-0.1.1/unbiasedness/unbiasedness.py`

 * *Files identical despite different names*

### Comparing `unbiasedness-0.1.0/unbiasedness/windows.py` & `unbiasedness-0.1.1/unbiasedness/windows.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from collections import ChainMap
 
 import pandas as pd
 import numpy as np
 
 
 def resample_windows(
-    win_df: Dict[Tuple[int, int], pd.DataFrame]
-) -> Dict[Tuple[int, int], pd.DataFrame]:
+    win_df: Dict[Tuple[int, int] | str, pd.DataFrame]
+) -> Dict[Tuple[int, int] | str, pd.DataFrame]:
     """Resample observations with replacement.
 
     Args:
         win_df (Dict[Tuple[int, int], pd.DataFrame]): Dictionnary of dataframes with observations
         for each window.
 
     Returns:
@@ -26,14 +26,16 @@
     The event dates are assumed to be in the column `index`.
     """
     if not win_df:
         raise ValueError("win_df is empty")
 
     try:
         first_key = next(iter(win_df))
+        if type(win_df[first_key]) is not pd.DataFrame:
+            raise ValueError("win_df must be a dictionary of dataframes")
         dates = win_df[first_key]["index"].unique()
     except AttributeError as e:
         raise ValueError("win_df must be a dictionary of dataframes") from e
 
     # Sample index with replacement
     dates = np.random.choice(dates, size=len(dates), replace=True)
```

### Comparing `unbiasedness-0.1.0/PKG-INFO` & `unbiasedness-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: unbiasedness
-Version: 0.1.0
+Version: 0.1.1
 Summary: Functions for estimating unbiasedness regressions.
 License: Apache License, Version 2
 Author: Vincent Grégoire
 Author-email: vincent.gregoire@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numba (>=0.57.1,<0.58.0)
-Requires-Dist: numpy (>=1.25.1,<2.0.0)
-Requires-Dist: pandas (>=2.0.3,<3.0.0)
+Requires-Dist: numpy (>=1.24,<2.0)
+Requires-Dist: pandas (>=2.0,<3.0)
 Requires-Dist: statsmodels (>=0.14.0,<0.15.0)
 Description-Content-Type: text/markdown
 
 # Unbiasedness regressions in Python
 
 This module provides many functions to estimate unbiasedness regressions in Python.
```

