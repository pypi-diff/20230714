# Comparing `tmp/loco_hd-0.1.1.tar.gz` & `tmp/loco_hd-0.1.2.tar.gz`

## Comparing `loco_hd-0.1.1.tar` & `loco_hd-0.1.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      590 1970-01-01 00:00:00.000000 loco_hd-0.1.1/Cargo.toml
--rw-rw-r--   0     1000     1000     1462 2023-02-09 09:29:24.000000 loco_hd-0.1.1/.github/workflows/CI.yml
--rw-rw-r--   0     1000     1000      725 2022-08-15 09:48:38.000000 loco_hd-0.1.1/.gitignore
--rw-r--r--   0     1000     1000     1070 2023-07-14 15:16:26.000000 loco_hd-0.1.1/LICENSE
--rw-rw-r--   0     1000     1000     2750 2023-07-09 09:33:57.000000 loco_hd-0.1.1/README.md
--rw-rw-r--   0     1000     1000      192 2023-07-05 07:38:55.000000 loco_hd-0.1.1/loco_hd/__init__.py
--rw-rw-r--   0     1000     1000     5859 2023-05-27 18:48:17.000000 loco_hd-0.1.1/loco_hd/atom_converter_utils.py
--rw-rw-r--   0     1000     1000    10262 2023-07-05 09:21:30.000000 loco_hd-0.1.1/loco_hd/loco_hd.pyi
--rw-rw-r--   0     1000     1000        0 2023-05-27 18:48:17.000000 loco_hd-0.1.1/loco_hd/py.typed
--rw-rw-r--   0     1000     1000    79633 2023-07-05 13:57:31.000000 loco_hd-0.1.1/locohd_logo.png
--rw-rw-r--   0     1000     1000      591 2023-07-14 15:30:10.000000 loco_hd-0.1.1/pyproject.toml
--rw-rw-r--   0     1000     1000     8445 2023-07-05 08:32:15.000000 loco_hd-0.1.1/python_codes/casp14_compare_structures.py
--rw-rw-r--   0     1000     1000     5089 2023-01-11 08:17:42.000000 loco_hd-0.1.1/python_codes/casp14_predictor_extractor.py
--rw-rw-r--   0     1000     1000    12075 2023-07-05 07:43:41.000000 loco_hd-0.1.1/python_codes/casp14_predictor_test.py
--rw-rw-r--   0     1000     1000    12707 2023-07-05 09:33:56.000000 loco_hd-0.1.1/python_codes/compare_ensembles.py
--rw-rw-r--   0     1000     1000     2709 2023-07-05 09:04:33.000000 loco_hd-0.1.1/python_codes/kras_scan.py
--rw-rw-r--   0     1000     1000     6629 2023-07-05 09:14:09.000000 loco_hd-0.1.1/python_codes/pisces_random_pairs.py
--rw-rw-r--   0     1000     1000    14302 2023-02-08 12:00:46.000000 loco_hd-0.1.1/python_codes/pisces_random_pairs_analyze.py
--rw-rw-r--   0     1000     1000     1665 2023-03-27 08:14:26.000000 loco_hd-0.1.1/python_codes/primitive_typings/all_atom.config.json
--rw-rw-r--   0     1000     1000     1718 2023-05-27 18:48:17.000000 loco_hd-0.1.1/python_codes/primitive_typings/all_atom_with_centroid.config.json
--rw-rw-r--   0     1000     1000     1031 2023-05-27 18:48:17.000000 loco_hd-0.1.1/python_codes/primitive_typings/coarse_grained.config.json
--rw-rw-r--   0     1000     1000     1084 2023-05-27 18:48:17.000000 loco_hd-0.1.1/python_codes/primitive_typings/coarse_grained_with_centroid.config.json
--rw-rw-r--   0     1000     1000     1611 2023-07-13 11:38:45.000000 loco_hd-0.1.1/python_codes/simple_test.py
--rw-rw-r--   0     1000     1000     1152 2023-06-25 17:06:17.000000 loco_hd-0.1.1/python_codes/test_integrators.py
--rw-rw-r--   0     1000     1000    13402 2023-07-05 09:54:31.000000 loco_hd-0.1.1/python_codes/trajectory_analyzer.py
--rw-rw-r--   0     1000     1000      333 2023-07-04 18:40:06.000000 loco_hd-0.1.1/src/lib.rs
--rw-rw-r--   0     1000     1000     1031 2023-07-05 09:28:40.000000 loco_hd-0.1.1/src/locohd/locohd_utests.rs
--rw-rw-r--   0     1000     1000     2610 2023-07-04 14:26:07.000000 loco_hd-0.1.1/src/locohd/pmf.rs
--rw-rw-r--   0     1000     1000     1358 2023-07-04 14:30:01.000000 loco_hd-0.1.1/src/locohd/pmf_utests.rs
--rw-rw-r--   0     1000     1000      633 2023-05-27 18:48:17.000000 loco_hd-0.1.1/src/locohd/primitive_atom.rs
--rw-r--r--   0     1000     1000     1691 2023-07-05 09:26:30.000000 loco_hd-0.1.1/src/locohd/tag_pairing_rule.rs
--rw-r--r--   0     1000     1000        0 2023-07-04 18:38:40.000000 loco_hd-0.1.1/src/locohd/tag_pairing_rule_utests.rs
--rw-rw-r--   0     1000     1000     1227 2023-05-27 18:48:17.000000 loco_hd-0.1.1/src/locohd/utils.rs
--rw-rw-r--   0     1000     1000     2106 2023-05-27 18:48:17.000000 loco_hd-0.1.1/src/locohd/weight_function/cdfs.rs
--rw-rw-r--   0     1000     1000     4253 2023-07-05 07:09:39.000000 loco_hd-0.1.1/src/locohd/weight_function.rs
--rw-rw-r--   0     1000     1000     6902 2023-05-27 18:48:17.000000 loco_hd-0.1.1/src/locohd/weight_function_utests.rs
--rw-rw-r--   0     1000     1000    13001 2023-07-05 09:29:39.000000 loco_hd-0.1.1/src/locohd.rs
--rw-rw-r--   0     1000     1000    10496 2023-05-27 18:48:17.000000 loco_hd-0.1.1/Cargo.lock
--rw-r--r--   0        0        0     3322 1970-01-01 00:00:00.000000 loco_hd-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      590 1970-01-01 00:00:00.000000 loco_hd-0.1.2/Cargo.toml
+-rw-rw-r--   0     1000     1000     1462 2023-02-09 09:29:24.000000 loco_hd-0.1.2/.github/workflows/CI.yml
+-rw-rw-r--   0     1000     1000      725 2022-08-15 09:48:38.000000 loco_hd-0.1.2/.gitignore
+-rw-r--r--   0     1000     1000     1070 2023-07-14 15:16:26.000000 loco_hd-0.1.2/LICENSE
+-rw-rw-r--   0     1000     1000     2803 2023-07-14 15:32:40.000000 loco_hd-0.1.2/README.md
+-rw-rw-r--   0     1000     1000      192 2023-07-05 07:38:55.000000 loco_hd-0.1.2/loco_hd/__init__.py
+-rw-rw-r--   0     1000     1000     5859 2023-05-27 18:48:17.000000 loco_hd-0.1.2/loco_hd/atom_converter_utils.py
+-rw-rw-r--   0     1000     1000    10262 2023-07-05 09:21:30.000000 loco_hd-0.1.2/loco_hd/loco_hd.pyi
+-rw-rw-r--   0     1000     1000        0 2023-05-27 18:48:17.000000 loco_hd-0.1.2/loco_hd/py.typed
+-rw-rw-r--   0     1000     1000    79633 2023-07-05 13:57:31.000000 loco_hd-0.1.2/locohd_logo.png
+-rw-rw-r--   0     1000     1000      591 2023-07-14 15:32:37.000000 loco_hd-0.1.2/pyproject.toml
+-rw-rw-r--   0     1000     1000     8445 2023-07-05 08:32:15.000000 loco_hd-0.1.2/python_codes/casp14_compare_structures.py
+-rw-rw-r--   0     1000     1000     5089 2023-01-11 08:17:42.000000 loco_hd-0.1.2/python_codes/casp14_predictor_extractor.py
+-rw-rw-r--   0     1000     1000    12075 2023-07-05 07:43:41.000000 loco_hd-0.1.2/python_codes/casp14_predictor_test.py
+-rw-rw-r--   0     1000     1000    12707 2023-07-05 09:33:56.000000 loco_hd-0.1.2/python_codes/compare_ensembles.py
+-rw-rw-r--   0     1000     1000     2709 2023-07-05 09:04:33.000000 loco_hd-0.1.2/python_codes/kras_scan.py
+-rw-rw-r--   0     1000     1000     6629 2023-07-05 09:14:09.000000 loco_hd-0.1.2/python_codes/pisces_random_pairs.py
+-rw-rw-r--   0     1000     1000    14302 2023-02-08 12:00:46.000000 loco_hd-0.1.2/python_codes/pisces_random_pairs_analyze.py
+-rw-rw-r--   0     1000     1000     1665 2023-03-27 08:14:26.000000 loco_hd-0.1.2/python_codes/primitive_typings/all_atom.config.json
+-rw-rw-r--   0     1000     1000     1718 2023-05-27 18:48:17.000000 loco_hd-0.1.2/python_codes/primitive_typings/all_atom_with_centroid.config.json
+-rw-rw-r--   0     1000     1000     1031 2023-05-27 18:48:17.000000 loco_hd-0.1.2/python_codes/primitive_typings/coarse_grained.config.json
+-rw-rw-r--   0     1000     1000     1084 2023-05-27 18:48:17.000000 loco_hd-0.1.2/python_codes/primitive_typings/coarse_grained_with_centroid.config.json
+-rw-rw-r--   0     1000     1000     1611 2023-07-13 11:38:45.000000 loco_hd-0.1.2/python_codes/simple_test.py
+-rw-rw-r--   0     1000     1000     1152 2023-06-25 17:06:17.000000 loco_hd-0.1.2/python_codes/test_integrators.py
+-rw-rw-r--   0     1000     1000    13402 2023-07-05 09:54:31.000000 loco_hd-0.1.2/python_codes/trajectory_analyzer.py
+-rw-rw-r--   0     1000     1000      333 2023-07-04 18:40:06.000000 loco_hd-0.1.2/src/lib.rs
+-rw-rw-r--   0     1000     1000     1031 2023-07-05 09:28:40.000000 loco_hd-0.1.2/src/locohd/locohd_utests.rs
+-rw-rw-r--   0     1000     1000     2610 2023-07-04 14:26:07.000000 loco_hd-0.1.2/src/locohd/pmf.rs
+-rw-rw-r--   0     1000     1000     1358 2023-07-04 14:30:01.000000 loco_hd-0.1.2/src/locohd/pmf_utests.rs
+-rw-rw-r--   0     1000     1000      633 2023-05-27 18:48:17.000000 loco_hd-0.1.2/src/locohd/primitive_atom.rs
+-rw-r--r--   0     1000     1000     1691 2023-07-05 09:26:30.000000 loco_hd-0.1.2/src/locohd/tag_pairing_rule.rs
+-rw-r--r--   0     1000     1000        0 2023-07-04 18:38:40.000000 loco_hd-0.1.2/src/locohd/tag_pairing_rule_utests.rs
+-rw-rw-r--   0     1000     1000     1227 2023-05-27 18:48:17.000000 loco_hd-0.1.2/src/locohd/utils.rs
+-rw-rw-r--   0     1000     1000     2106 2023-05-27 18:48:17.000000 loco_hd-0.1.2/src/locohd/weight_function/cdfs.rs
+-rw-rw-r--   0     1000     1000     4253 2023-07-05 07:09:39.000000 loco_hd-0.1.2/src/locohd/weight_function.rs
+-rw-rw-r--   0     1000     1000     6902 2023-05-27 18:48:17.000000 loco_hd-0.1.2/src/locohd/weight_function_utests.rs
+-rw-rw-r--   0     1000     1000    13001 2023-07-05 09:29:39.000000 loco_hd-0.1.2/src/locohd.rs
+-rw-rw-r--   0     1000     1000    10496 2023-05-27 18:48:17.000000 loco_hd-0.1.2/Cargo.lock
+-rw-r--r--   0        0        0     3375 1970-01-01 00:00:00.000000 loco_hd-0.1.2/PKG-INFO
```

### Comparing `loco_hd-0.1.1/Cargo.toml` & `loco_hd-0.1.2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.1/.github/workflows/CI.yml` & `loco_hd-0.1.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.1/.gitignore` & `loco_hd-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.1/LICENSE` & `loco_hd-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.1/README.md` & `loco_hd-0.1.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 the [TM-score](https://en.wikipedia.org/wiki/Template_modeling_score), 
 [lDDT](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3799472/), 
 or [GDT_TS](https://en.wikipedia.org/wiki/Global_distance_test), 
 it is based on the measurement of local composition differences, rather than of the Euclidean deviations. 
 
 ## Where can I read about it?
 
-The theory behind LoCoHD was published [here](journal).
+<p style="color:red">Still unpublished...<p>
 
 ## How can I install it?
 
 ### From PyPI
 
 With pip, it is easy to add LoCoHD to your packages:
 
@@ -56,8 +56,10 @@
 ```
 
 And you are done!
 
 
 ## How can I use it?
 
-LoCoHD was intended to be used within Python scripts, mostly through [BioPython](https://github.com/biopython/biopython) as the main `.pdb` file reader. It is also possible to use it with other protein/molecular structure readers, but the user has to write the appropriate parser that converts the information within the file into the information required for LoCoHD. An example for this can be found [here](./python_codes/trajectory_analyzer.py), where the structures come from a molecular dynamics trajectory and parsing is achieved by [MDAnalysis](https://github.com/MDAnalysis/mdanalysis).
+LoCoHD was intended to be used within Python scripts, mostly through [BioPython](https://github.com/biopython/biopython) as the main `.pdb` file reader. It is also possible to use it with other protein/molecular structure readers, but the user has to write the appropriate parser that converts the information within the file into the information required for LoCoHD. An example for this can be found [here](./python_codes/trajectory_analyzer.py), where the structures come from a molecular dynamics trajectory and parsing is achieved by [MDAnalysis](https://github.com/MDAnalysis/mdanalysis).
+
+<p style="color:red">Detailed description is coming soon...<p>
```

### Comparing `loco_hd-0.1.1/loco_hd/atom_converter_utils.py` & `loco_hd-0.1.2/loco_hd/atom_converter_utils.py`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.1/loco_hd/loco_hd.pyi` & `loco_hd-0.1.2/loco_hd/loco_hd.pyi`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.1/locohd_logo.png` & `loco_hd-0.1.2/locohd_logo.png`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.1/pyproject.toml` & `loco_hd-0.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["maturin>=0.13,<0.14"]
 build-backend = "maturin"
 
 [project]
 name = "loco_hd"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
     { name = "Zsolt Fazekas", email = "zsolt.fazekas.9@gmail.com" }
 ]
 description = "Implementation of the LoCoHD metric for quantitative protein structure and substructure comparison"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-    "biopython>=1.81",
+    "biopython>=1.80",
     "numpy>=1.21.6"
 ]
```

### Comparing `loco_hd-0.1.1/python_codes/casp14_compare_structures.py` & `loco_hd-0.1.2/python_codes/casp14_compare_structures.py`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.1/python_codes/casp14_predictor_extractor.py` & `loco_hd-0.1.2/python_codes/casp14_predictor_extractor.py`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.1/python_codes/casp14_predictor_test.py` & `loco_hd-0.1.2/python_codes/casp14_predictor_test.py`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.1/python_codes/compare_ensembles.py` & `loco_hd-0.1.2/python_codes/compare_ensembles.py`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.1/python_codes/kras_scan.py` & `loco_hd-0.1.2/python_codes/kras_scan.py`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.1/python_codes/pisces_random_pairs.py` & `loco_hd-0.1.2/python_codes/pisces_random_pairs.py`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.1/python_codes/pisces_random_pairs_analyze.py` & `loco_hd-0.1.2/python_codes/pisces_random_pairs_analyze.py`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.1/python_codes/primitive_typings/all_atom.config.json` & `loco_hd-0.1.2/python_codes/primitive_typings/all_atom.config.json`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.1/python_codes/primitive_typings/all_atom_with_centroid.config.json` & `loco_hd-0.1.2/python_codes/primitive_typings/all_atom_with_centroid.config.json`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.1/python_codes/primitive_typings/coarse_grained.config.json` & `loco_hd-0.1.2/python_codes/primitive_typings/coarse_grained.config.json`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.1/python_codes/primitive_typings/coarse_grained_with_centroid.config.json` & `loco_hd-0.1.2/python_codes/primitive_typings/coarse_grained_with_centroid.config.json`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.1/python_codes/simple_test.py` & `loco_hd-0.1.2/python_codes/simple_test.py`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.1/python_codes/test_integrators.py` & `loco_hd-0.1.2/python_codes/test_integrators.py`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.1/python_codes/trajectory_analyzer.py` & `loco_hd-0.1.2/python_codes/trajectory_analyzer.py`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.1/src/locohd/locohd_utests.rs` & `loco_hd-0.1.2/src/locohd/locohd_utests.rs`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.1/src/locohd/pmf.rs` & `loco_hd-0.1.2/src/locohd/pmf.rs`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.1/src/locohd/pmf_utests.rs` & `loco_hd-0.1.2/src/locohd/pmf_utests.rs`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.1/src/locohd/primitive_atom.rs` & `loco_hd-0.1.2/src/locohd/primitive_atom.rs`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.1/src/locohd/tag_pairing_rule.rs` & `loco_hd-0.1.2/src/locohd/tag_pairing_rule.rs`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.1/src/locohd/utils.rs` & `loco_hd-0.1.2/src/locohd/utils.rs`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.1/src/locohd/weight_function/cdfs.rs` & `loco_hd-0.1.2/src/locohd/weight_function/cdfs.rs`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.1/src/locohd/weight_function.rs` & `loco_hd-0.1.2/src/locohd/weight_function.rs`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.1/src/locohd/weight_function_utests.rs` & `loco_hd-0.1.2/src/locohd/weight_function_utests.rs`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.1/src/locohd.rs` & `loco_hd-0.1.2/src/locohd.rs`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.1/Cargo.lock` & `loco_hd-0.1.2/Cargo.lock`

 * *Files identical despite different names*

### Comparing `loco_hd-0.1.1/PKG-INFO` & `loco_hd-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: loco_hd
-Version: 0.1.1
+Version: 0.1.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Dist: biopython>=1.81
+Requires-Dist: biopython>=1.80
 Requires-Dist: numpy>=1.21.6
 License-File: LICENSE
 Summary: Implementation of the LoCoHD metric for quantitative protein structure and substructure comparison
 Author-email: Zsolt Fazekas <zsolt.fazekas.9@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
@@ -29,15 +29,15 @@
 the [TM-score](https://en.wikipedia.org/wiki/Template_modeling_score), 
 [lDDT](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3799472/), 
 or [GDT_TS](https://en.wikipedia.org/wiki/Global_distance_test), 
 it is based on the measurement of local composition differences, rather than of the Euclidean deviations. 
 
 ## Where can I read about it?
 
-The theory behind LoCoHD was published [here](journal).
+<p style="color:red">Still unpublished...<p>
 
 ## How can I install it?
 
 ### From PyPI
 
 With pip, it is easy to add LoCoHD to your packages:
 
@@ -71,7 +71,9 @@
 
 And you are done!
 
 
 ## How can I use it?
 
 LoCoHD was intended to be used within Python scripts, mostly through [BioPython](https://github.com/biopython/biopython) as the main `.pdb` file reader. It is also possible to use it with other protein/molecular structure readers, but the user has to write the appropriate parser that converts the information within the file into the information required for LoCoHD. An example for this can be found [here](./python_codes/trajectory_analyzer.py), where the structures come from a molecular dynamics trajectory and parsing is achieved by [MDAnalysis](https://github.com/MDAnalysis/mdanalysis).
+
+<p style="color:red">Detailed description is coming soon...<p>
```

