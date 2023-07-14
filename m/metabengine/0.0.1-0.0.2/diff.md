# Comparing `tmp/metabengine-0.0.1.tar.gz` & `tmp/metabengine-0.0.2.tar.gz`

## Comparing `metabengine-0.0.1.tar` & `metabengine-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metabengine-0.0.1/src/metabengine/__init__.py
--rw-r--r--   0        0        0     5741 2020-02-02 00:00:00.000000 metabengine-0.0.1/src/metabengine/alignment.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 metabengine-0.0.1/src/metabengine/ann_feat_quality.py
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 metabengine-0.0.1/src/metabengine/calculate_mass.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 metabengine-0.0.1/src/metabengine/feat_extract.py
--rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 metabengine-0.0.1/src/metabengine/feature_grouping.py
--rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 metabengine-0.0.1/src/metabengine/msms.py
--rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 metabengine-0.0.1/src/metabengine/params.py
--rw-r--r--   0        0        0    13615 2020-02-02 00:00:00.000000 metabengine-0.0.1/src/metabengine/peak_detect.py
--rw-r--r--   0        0        0    17876 2020-02-02 00:00:00.000000 metabengine-0.0.1/src/metabengine/raw_data_utils.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 metabengine-0.0.1/src/metabengine/targeted_search.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 metabengine-0.0.1/src/metabengine/visual.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 metabengine-0.0.1/LICENSE
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 metabengine-0.0.1/README.md
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 metabengine-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 metabengine-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metabengine-0.0.2/src/metabengine/__init__.py
+-rw-r--r--   0        0        0     5741 2020-02-02 00:00:00.000000 metabengine-0.0.2/src/metabengine/alignment.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 metabengine-0.0.2/src/metabengine/ann_feat_quality.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 metabengine-0.0.2/src/metabengine/calculate_mass.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 metabengine-0.0.2/src/metabengine/feat_extract.py
+-rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 metabengine-0.0.2/src/metabengine/feature_grouping.py
+-rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 metabengine-0.0.2/src/metabengine/msms.py
+-rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 metabengine-0.0.2/src/metabengine/params.py
+-rw-r--r--   0        0        0    13616 2020-02-02 00:00:00.000000 metabengine-0.0.2/src/metabengine/peak_detect.py
+-rw-r--r--   0        0        0    17883 2020-02-02 00:00:00.000000 metabengine-0.0.2/src/metabengine/raw_data_utils.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 metabengine-0.0.2/src/metabengine/targeted_search.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 metabengine-0.0.2/src/metabengine/visual.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 metabengine-0.0.2/LICENSE
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 metabengine-0.0.2/README.md
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 metabengine-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 metabengine-0.0.2/PKG-INFO
```

### Comparing `metabengine-0.0.1/src/metabengine/alignment.py` & `metabengine-0.0.2/src/metabengine/alignment.py`

 * *Files identical despite different names*

### Comparing `metabengine-0.0.1/src/metabengine/ann_feat_quality.py` & `metabengine-0.0.2/src/metabengine/ann_feat_quality.py`

 * *Files identical despite different names*

### Comparing `metabengine-0.0.1/src/metabengine/calculate_mass.py` & `metabengine-0.0.2/src/metabengine/calculate_mass.py`

 * *Files identical despite different names*

### Comparing `metabengine-0.0.1/src/metabengine/feat_extract.py` & `metabengine-0.0.2/src/metabengine/feat_extract.py`

 * *Files identical despite different names*

### Comparing `metabengine-0.0.1/src/metabengine/feature_grouping.py` & `metabengine-0.0.2/src/metabengine/feature_grouping.py`

 * *Files identical despite different names*

### Comparing `metabengine-0.0.1/src/metabengine/msms.py` & `metabengine-0.0.2/src/metabengine/msms.py`

 * *Files identical despite different names*

### Comparing `metabengine-0.0.1/src/metabengine/params.py` & `metabengine-0.0.2/src/metabengine/params.py`

 * *Files identical despite different names*

### Comparing `metabengine-0.0.1/src/metabengine/peak_detect.py` & `metabengine-0.0.2/src/metabengine/peak_detect.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # A module for feature/peak detection
 
 # Import modules
 import numpy as np
 from tqdm import tqdm
 from scipy.signal import argrelextrema
-from msms import spec_similarity
+from .msms import spec_similarity
 import copy
 
 
 def roi_finder(d, params, **kwargs):
     """
     A function to find the region of interest (ROI) in the MS data.
```

### Comparing `metabengine-0.0.1/src/metabengine/raw_data_utils.py` & `metabengine-0.0.2/src/metabengine/raw_data_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # A module to read and process the raw MS data
 # Classes are defined in order to handle the data
 
 # Import modules
 from pyteomics import mzml, mzxml
 import numpy as np
 import os
-import peak_detect
+from . import peak_detect
 import matplotlib.pyplot as plt
 import pandas as pd
 
 
 class MSData:
     """
     A class that models a single file (mzML or mzXML) and
```

### Comparing `metabengine-0.0.1/src/metabengine/targeted_search.py` & `metabengine-0.0.2/src/metabengine/targeted_search.py`

 * *Files identical despite different names*

### Comparing `metabengine-0.0.1/LICENSE` & `metabengine-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `metabengine-0.0.1/pyproject.toml` & `metabengine-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "metabengine"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Huaxu Yu", email="yhxchem@outlook.com" },
 ]
 maintainers = [
   { name="Huaxu Yu", email="yhxchem@outlook.com" },
 ]
 description = "Data preprocessing for mass spectrometry-based metabolomics data"
@@ -23,11 +23,12 @@
     "numpy>=1.24",
     "pandas>=2.0",
     "pyteomics>=4.6",
     "scikit-learn>=1.2",
     "scipy>=1.10.1",
     "tensorflow>=2.12.0",
     "tqdm>=4.65.0",
+    "lxml>=4.9.2",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/Waddlessss/metabengine"
```

### Comparing `metabengine-0.0.1/PKG-INFO` & `metabengine-0.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: metabengine
-Version: 0.0.1
+Version: 0.0.2
 Summary: Data preprocessing for mass spectrometry-based metabolomics data
 Project-URL: Homepage, https://github.com/Waddlessss/metabengine
 Author-email: Huaxu Yu <yhxchem@outlook.com>
 Maintainer-email: Huaxu Yu <yhxchem@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
+Requires-Dist: lxml>=4.9.2
 Requires-Dist: numpy>=1.24
 Requires-Dist: pandas>=2.0
 Requires-Dist: pyteomics>=4.6
 Requires-Dist: scikit-learn>=1.2
 Requires-Dist: scipy>=1.10.1
 Requires-Dist: tensorflow>=2.12.0
 Requires-Dist: tqdm>=4.65.0
```

