# Comparing `tmp/chemfunc-1.0.3.tar.gz` & `tmp/chemfunc-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemfunc-1.0.3.tar", last modified: Fri Jun  2 15:51:40 2023, max compression
+gzip compressed data, was "chemfunc-1.0.4.tar", last modified: Thu Jul 13 23:26:46 2023, max compression
```

## Comparing `chemfunc-1.0.3.tar` & `chemfunc-1.0.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2023-06-02 15:51:40.232228 chemfunc-1.0.3/
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1069 2023-03-07 02:37:32.000000 chemfunc-1.0.3/LICENSE
--rw-r--r--   0 kyleswanson   (501) staff       (20)     6386 2023-06-02 15:51:40.232379 chemfunc-1.0.3/PKG-INFO
--rw-r--r--   0 kyleswanson   (501) staff       (20)     5644 2023-05-25 21:30:47.000000 chemfunc-1.0.3/README.md
-drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2023-06-02 15:51:40.228368 chemfunc-1.0.3/chemfunc/
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2014 2023-05-23 23:24:43.000000 chemfunc-1.0.3/chemfunc/__init__.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)      176 2023-06-02 15:51:11.000000 chemfunc-1.0.3/chemfunc/_version.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2841 2023-05-23 23:24:43.000000 chemfunc-1.0.3/chemfunc/canonicalize_smiles.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2007 2023-05-23 23:24:43.000000 chemfunc-1.0.3/chemfunc/chemical_diversity.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1583 2023-05-23 23:24:43.000000 chemfunc-1.0.3/chemfunc/cluster_molecules.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1520 2023-05-23 23:24:43.000000 chemfunc-1.0.3/chemfunc/compute_properties.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)      137 2023-03-07 00:44:25.000000 chemfunc-1.0.3/chemfunc/constants.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)      877 2023-05-23 23:24:43.000000 chemfunc-1.0.3/chemfunc/deduplicate_smiles.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     4002 2023-05-23 18:54:45.000000 chemfunc-1.0.3/chemfunc/filter_molecules.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1199 2023-05-23 23:24:43.000000 chemfunc-1.0.3/chemfunc/main.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2643 2023-05-23 20:59:02.000000 chemfunc-1.0.3/chemfunc/measure_experimental_reproducibility.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     4600 2023-06-01 23:18:30.000000 chemfunc-1.0.3/chemfunc/molecular_fingerprints.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     4093 2023-06-01 19:01:48.000000 chemfunc-1.0.3/chemfunc/molecular_properties.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     8551 2023-05-23 23:24:43.000000 chemfunc-1.0.3/chemfunc/molecular_similarities.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     3274 2023-06-02 15:22:59.000000 chemfunc-1.0.3/chemfunc/nearest_neighbor.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1659 2023-05-23 21:00:59.000000 chemfunc-1.0.3/chemfunc/plot_property_distribution.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     6620 2023-05-23 23:24:43.000000 chemfunc-1.0.3/chemfunc/plot_tsne.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1672 2023-05-23 18:54:45.000000 chemfunc-1.0.3/chemfunc/regression_to_classification.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1654 2023-05-23 18:54:45.000000 chemfunc-1.0.3/chemfunc/sample_molecules.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1956 2023-05-23 23:24:43.000000 chemfunc-1.0.3/chemfunc/sdf_to_smiles.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1223 2023-05-23 23:24:43.000000 chemfunc-1.0.3/chemfunc/select_from_clusters.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)      878 2023-05-23 21:04:54.000000 chemfunc-1.0.3/chemfunc/smiles_to_svg.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2129 2023-05-23 18:54:45.000000 chemfunc-1.0.3/chemfunc/utils.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2514 2023-05-23 23:24:43.000000 chemfunc-1.0.3/chemfunc/visualize_molecules.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2141 2023-05-23 21:10:47.000000 chemfunc-1.0.3/chemfunc/visualize_reactions.py
-drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2023-06-02 15:51:40.231846 chemfunc-1.0.3/chemfunc.egg-info/
--rw-r--r--   0 kyleswanson   (501) staff       (20)     6386 2023-06-02 15:51:40.000000 chemfunc-1.0.3/chemfunc.egg-info/PKG-INFO
--rw-r--r--   0 kyleswanson   (501) staff       (20)      974 2023-06-02 15:51:40.000000 chemfunc-1.0.3/chemfunc.egg-info/SOURCES.txt
--rw-r--r--   0 kyleswanson   (501) staff       (20)        1 2023-06-02 15:51:40.000000 chemfunc-1.0.3/chemfunc.egg-info/dependency_links.txt
--rw-r--r--   0 kyleswanson   (501) staff       (20)       48 2023-06-02 15:51:40.000000 chemfunc-1.0.3/chemfunc.egg-info/entry_points.txt
--rw-r--r--   0 kyleswanson   (501) staff       (20)       93 2023-06-02 15:51:40.000000 chemfunc-1.0.3/chemfunc.egg-info/requires.txt
--rw-r--r--   0 kyleswanson   (501) staff       (20)        9 2023-06-02 15:51:40.000000 chemfunc-1.0.3/chemfunc.egg-info/top_level.txt
--rw-r--r--   0 kyleswanson   (501) staff       (20)       79 2023-06-02 15:51:40.232933 chemfunc-1.0.3/setup.cfg
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1612 2023-05-23 23:24:43.000000 chemfunc-1.0.3/setup.py
+drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2023-07-13 23:26:46.338860 chemfunc-1.0.4/
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1069 2023-03-07 02:37:32.000000 chemfunc-1.0.4/LICENSE
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     6521 2023-07-13 23:26:46.339246 chemfunc-1.0.4/PKG-INFO
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     5779 2023-07-13 23:02:21.000000 chemfunc-1.0.4/README.md
+drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2023-07-13 23:26:46.333810 chemfunc-1.0.4/chemfunc/
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2037 2023-07-13 23:01:21.000000 chemfunc-1.0.4/chemfunc/__init__.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      176 2023-07-13 23:13:01.000000 chemfunc-1.0.4/chemfunc/_version.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2841 2023-05-23 23:24:43.000000 chemfunc-1.0.4/chemfunc/canonicalize_smiles.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2007 2023-05-23 23:24:43.000000 chemfunc-1.0.4/chemfunc/chemical_diversity.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1583 2023-05-23 23:24:43.000000 chemfunc-1.0.4/chemfunc/cluster_molecules.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1520 2023-05-23 23:24:43.000000 chemfunc-1.0.4/chemfunc/compute_properties.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      137 2023-03-07 00:44:25.000000 chemfunc-1.0.4/chemfunc/constants.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      877 2023-05-23 23:24:43.000000 chemfunc-1.0.4/chemfunc/deduplicate_smiles.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     4002 2023-05-23 18:54:45.000000 chemfunc-1.0.4/chemfunc/filter_molecules.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1222 2023-07-13 23:01:21.000000 chemfunc-1.0.4/chemfunc/main.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2643 2023-05-23 20:59:02.000000 chemfunc-1.0.4/chemfunc/measure_experimental_reproducibility.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     5736 2023-07-13 23:19:10.000000 chemfunc-1.0.4/chemfunc/molecular_fingerprints.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     4093 2023-06-01 19:01:48.000000 chemfunc-1.0.4/chemfunc/molecular_properties.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     8551 2023-05-23 23:24:43.000000 chemfunc-1.0.4/chemfunc/molecular_similarities.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     3274 2023-06-02 15:22:59.000000 chemfunc-1.0.4/chemfunc/nearest_neighbor.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1659 2023-05-23 21:00:59.000000 chemfunc-1.0.4/chemfunc/plot_property_distribution.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     6620 2023-05-23 23:24:43.000000 chemfunc-1.0.4/chemfunc/plot_tsne.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1672 2023-05-23 18:54:45.000000 chemfunc-1.0.4/chemfunc/regression_to_classification.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1654 2023-05-23 18:54:45.000000 chemfunc-1.0.4/chemfunc/sample_molecules.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1956 2023-05-23 23:24:43.000000 chemfunc-1.0.4/chemfunc/sdf_to_smiles.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1223 2023-05-23 23:24:43.000000 chemfunc-1.0.4/chemfunc/select_from_clusters.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      878 2023-05-23 21:04:54.000000 chemfunc-1.0.4/chemfunc/smiles_to_svg.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2129 2023-05-23 18:54:45.000000 chemfunc-1.0.4/chemfunc/utils.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2514 2023-06-24 07:43:27.000000 chemfunc-1.0.4/chemfunc/visualize_molecules.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2141 2023-05-23 21:10:47.000000 chemfunc-1.0.4/chemfunc/visualize_reactions.py
+drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2023-07-13 23:26:46.338233 chemfunc-1.0.4/chemfunc.egg-info/
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     6521 2023-07-13 23:26:46.000000 chemfunc-1.0.4/chemfunc.egg-info/PKG-INFO
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      974 2023-07-13 23:26:46.000000 chemfunc-1.0.4/chemfunc.egg-info/SOURCES.txt
+-rw-r--r--   0 kyleswanson   (501) staff       (20)        1 2023-07-13 23:26:46.000000 chemfunc-1.0.4/chemfunc.egg-info/dependency_links.txt
+-rw-r--r--   0 kyleswanson   (501) staff       (20)       48 2023-07-13 23:26:46.000000 chemfunc-1.0.4/chemfunc.egg-info/entry_points.txt
+-rw-r--r--   0 kyleswanson   (501) staff       (20)       93 2023-07-13 23:26:46.000000 chemfunc-1.0.4/chemfunc.egg-info/requires.txt
+-rw-r--r--   0 kyleswanson   (501) staff       (20)        9 2023-07-13 23:26:46.000000 chemfunc-1.0.4/chemfunc.egg-info/top_level.txt
+-rw-r--r--   0 kyleswanson   (501) staff       (20)       79 2023-07-13 23:26:46.340568 chemfunc-1.0.4/setup.cfg
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1612 2023-05-23 23:24:43.000000 chemfunc-1.0.4/setup.py
```

### Comparing `chemfunc-1.0.3/LICENSE` & `chemfunc-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.3/PKG-INFO` & `chemfunc-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: chemfunc
-Version: 1.0.3
+Version: 1.0.4
 Summary: Chem Func
 Home-page: https://github.com/swansonk14/chemfunc
-Download-URL: https://github.com/swansonk14/chemfunc/v_1.0.3.tar.gz
+Download-URL: https://github.com/swansonk14/chemfunc/v_1.0.4.tar.gz
 Author: Kyle Swanson
 Author-email: swansonk.14@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/swansonk14/chemfunc
 Project-URL: PyPi, https://pypi.org/project/chemfunc/
 Keywords: computational chemistry
 Classifier: Programming Language :: Python :: 3
@@ -105,17 +105,17 @@
 
 Filters molecules to those with values in a certain range.
 
 [`measure_experimental_reproducibility.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/measure_experimental_reproducibility.py) (function, script)
 
 Measures the experimental reproducibility of two biological replicates by using one replicate to predict the other.
 
-[`molecular_fingerprints.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/molecular_fingerprints.py) (functions)
+[`molecular_fingerprints.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/molecular_fingerprints.py) (functions, script)
 
-Contains functions to compute fingerprints for molecules. Parallelized for speed.
+Contains functions to compute fingerprints for molecules. Parallelized for speed. The function `save_fingerprints` can be used as a script to compute fingerprints from a CSV file and save them as an NPZ file.
 
 [`molecular_properties.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/molecular_properties.py) (functions)
 
 Contains functions to compute molecular properties. Parallelized for speed.
 
 [`molecular_similarities.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/molecular_similarities.py) (functions)
```

### Comparing `chemfunc-1.0.3/README.md` & `chemfunc-1.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -84,17 +84,17 @@
 
 Filters molecules to those with values in a certain range.
 
 [`measure_experimental_reproducibility.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/measure_experimental_reproducibility.py) (function, script)
 
 Measures the experimental reproducibility of two biological replicates by using one replicate to predict the other.
 
-[`molecular_fingerprints.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/molecular_fingerprints.py) (functions)
+[`molecular_fingerprints.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/molecular_fingerprints.py) (functions, script)
 
-Contains functions to compute fingerprints for molecules. Parallelized for speed.
+Contains functions to compute fingerprints for molecules. Parallelized for speed. The function `save_fingerprints` can be used as a script to compute fingerprints from a CSV file and save them as an NPZ file.
 
 [`molecular_properties.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/molecular_properties.py) (functions)
 
 Contains functions to compute molecular properties. Parallelized for speed.
 
 [`molecular_similarities.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/molecular_similarities.py) (functions)
```

### Comparing `chemfunc-1.0.3/chemfunc/__init__.py` & `chemfunc-1.0.4/chemfunc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 from chemfunc.molecular_fingerprints import (
     register_fingerprint_generator,
     get_fingerprint_generator,
     get_available_fingerprint_generators,
     compute_morgan_fingerprint,
     compute_rdkit_fingerprint,
     compute_fingerprint,
-    compute_fingerprints
+    compute_fingerprints,
+    save_fingerprints
 )
 from chemfunc.molecular_properties import (
     register_property_function,
     get_property_function,
     get_available_property_functions,
     smiles_to_mol_wrapper,
     compute_clogp,
```

### Comparing `chemfunc-1.0.3/chemfunc/canonicalize_smiles.py` & `chemfunc-1.0.4/chemfunc/canonicalize_smiles.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.3/chemfunc/chemical_diversity.py` & `chemfunc-1.0.4/chemfunc/chemical_diversity.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.3/chemfunc/cluster_molecules.py` & `chemfunc-1.0.4/chemfunc/cluster_molecules.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.3/chemfunc/compute_properties.py` & `chemfunc-1.0.4/chemfunc/compute_properties.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.3/chemfunc/deduplicate_smiles.py` & `chemfunc-1.0.4/chemfunc/deduplicate_smiles.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.3/chemfunc/filter_molecules.py` & `chemfunc-1.0.4/chemfunc/filter_molecules.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.3/chemfunc/main.py` & `chemfunc-1.0.4/chemfunc/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     filter_molecules,
     measure_experimental_reproducibility,
     nearest_neighbor,
     plot_property_distribution,
     plot_tsne,
     regression_to_classification,
     sample_molecules,
+    save_fingerprints,
     sdf_to_smiles,
     select_from_clusters,
     smiles_to_svg,
     visualize_molecules,
     visualize_reactions
 ]
 NAME_TO_FUNCTION = {
```

### Comparing `chemfunc-1.0.3/chemfunc/measure_experimental_reproducibility.py` & `chemfunc-1.0.4/chemfunc/measure_experimental_reproducibility.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.3/chemfunc/molecular_fingerprints.py` & `chemfunc-1.0.4/chemfunc/molecular_fingerprints.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 """Functions to compute fingerprints for molecules."""
 from multiprocessing import Pool
-from typing import Callable
+from pathlib import Path
+from typing import Callable, Literal
 
 import numpy as np
-from descriptastorus.descriptors import rdNormalizedDescriptors
+import pandas as pd
+import scipy
 from rdkit import Chem
 from rdkit.DataStructs import ConvertToNumpyArray
 from rdkit.Chem import AllChem
 from tqdm import tqdm
 
-from chemfunc.constants import Molecule
+from chemfunc.constants import Molecule, SMILES_COLUMN
 
-# Fix for NumPy >= 1.24.0
+# Fixes for descriptastorus
+# for NumPy >= 1.24.0
 np.float = float
 
+# for SciPy >= 1.11.0
+if not hasattr(scipy.stats, 'gilbrat'):
+    scipy.stats.gilbrat = scipy.stats.gibrat
+
+from descriptastorus.descriptors import rdNormalizedDescriptors
+
+
 FingerprintGenerator = Callable[[Molecule], np.ndarray]
 FINGERPRINT_GENERATOR_REGISTRY = {}
 MORGAN_RADIUS = 2
 MORGAN_NUM_BITS = 2048
 
 
 def register_fingerprint_generator(fingerprint_type: str) -> Callable[[FingerprintGenerator], FingerprintGenerator]:
@@ -111,7 +121,34 @@
     fingerprint_generator = get_fingerprint_generator(fingerprint_type)
 
     with Pool() as pool:
         fingerprints = np.array(list(tqdm(pool.imap(fingerprint_generator, mols),
                                           total=len(mols), desc=f'{fingerprint_type} fingerprints')))
 
     return fingerprints
+
+
+def save_fingerprints(
+        data_path: Path,
+        save_path: Path,
+        fingerprint_type: Literal['morgan', 'rdkit'] = 'rdkit',
+        smiles_column: str = SMILES_COLUMN
+) -> None:
+    """Saves fingerprints for molecules in a dataset.
+
+    :param data_path: Path to a CSV file containing molecules.
+    :param save_path: Path to a NPZ file where the fingerprints are saved (under the name "features").
+    :param fingerprint_type: The type of fingerprint to compute.
+    :param smiles_column: Name of column containing SMILES strings.
+    """
+    # Load data
+    data = pd.read_csv(data_path)
+
+    # Get SMILES
+    smiles = data[smiles_column].tolist()
+
+    # Compute fingerprints
+    fingerprints = compute_fingerprints(mols=smiles, fingerprint_type=fingerprint_type)
+
+    # Save fingerprints
+    save_path.parent.mkdir(parents=True, exist_ok=True)
+    np.savez_compressed(save_path, features=fingerprints)
```

### Comparing `chemfunc-1.0.3/chemfunc/molecular_properties.py` & `chemfunc-1.0.4/chemfunc/molecular_properties.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.3/chemfunc/molecular_similarities.py` & `chemfunc-1.0.4/chemfunc/molecular_similarities.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.3/chemfunc/nearest_neighbor.py` & `chemfunc-1.0.4/chemfunc/nearest_neighbor.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.3/chemfunc/plot_property_distribution.py` & `chemfunc-1.0.4/chemfunc/plot_property_distribution.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.3/chemfunc/plot_tsne.py` & `chemfunc-1.0.4/chemfunc/plot_tsne.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.3/chemfunc/regression_to_classification.py` & `chemfunc-1.0.4/chemfunc/regression_to_classification.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.3/chemfunc/sample_molecules.py` & `chemfunc-1.0.4/chemfunc/sample_molecules.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.3/chemfunc/sdf_to_smiles.py` & `chemfunc-1.0.4/chemfunc/sdf_to_smiles.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.3/chemfunc/select_from_clusters.py` & `chemfunc-1.0.4/chemfunc/select_from_clusters.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.3/chemfunc/smiles_to_svg.py` & `chemfunc-1.0.4/chemfunc/smiles_to_svg.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.3/chemfunc/utils.py` & `chemfunc-1.0.4/chemfunc/utils.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.3/chemfunc/visualize_molecules.py` & `chemfunc-1.0.4/chemfunc/visualize_molecules.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.3/chemfunc/visualize_reactions.py` & `chemfunc-1.0.4/chemfunc/visualize_reactions.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.3/chemfunc.egg-info/PKG-INFO` & `chemfunc-1.0.4/chemfunc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: chemfunc
-Version: 1.0.3
+Version: 1.0.4
 Summary: Chem Func
 Home-page: https://github.com/swansonk14/chemfunc
-Download-URL: https://github.com/swansonk14/chemfunc/v_1.0.3.tar.gz
+Download-URL: https://github.com/swansonk14/chemfunc/v_1.0.4.tar.gz
 Author: Kyle Swanson
 Author-email: swansonk.14@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/swansonk14/chemfunc
 Project-URL: PyPi, https://pypi.org/project/chemfunc/
 Keywords: computational chemistry
 Classifier: Programming Language :: Python :: 3
@@ -105,17 +105,17 @@
 
 Filters molecules to those with values in a certain range.
 
 [`measure_experimental_reproducibility.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/measure_experimental_reproducibility.py) (function, script)
 
 Measures the experimental reproducibility of two biological replicates by using one replicate to predict the other.
 
-[`molecular_fingerprints.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/molecular_fingerprints.py) (functions)
+[`molecular_fingerprints.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/molecular_fingerprints.py) (functions, script)
 
-Contains functions to compute fingerprints for molecules. Parallelized for speed.
+Contains functions to compute fingerprints for molecules. Parallelized for speed. The function `save_fingerprints` can be used as a script to compute fingerprints from a CSV file and save them as an NPZ file.
 
 [`molecular_properties.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/molecular_properties.py) (functions)
 
 Contains functions to compute molecular properties. Parallelized for speed.
 
 [`molecular_similarities.py`](https://github.com/swansonk14/chemfunc/blob/main/chemfunc/molecular_similarities.py) (functions)
```

### Comparing `chemfunc-1.0.3/chemfunc.egg-info/SOURCES.txt` & `chemfunc-1.0.4/chemfunc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.3/setup.py` & `chemfunc-1.0.4/setup.py`

 * *Files identical despite different names*

