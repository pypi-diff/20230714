# Comparing `tmp/KIF-0.2.0.tar.gz` & `tmp/KIF-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KIF-0.2.0.tar", last modified: Wed Apr  5 11:41:45 2023, max compression
+gzip compressed data, was "KIF-0.3.0.tar", last modified: Fri Jul 14 15:27:55 2023, max compression
```

## Comparing `KIF-0.2.0.tar` & `KIF-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 11:41:45.467195 KIF-0.2.0/
-drwxrwxrwx   0        0        0        0 2023-04-05 11:41:45.394191 KIF-0.2.0/KIF.egg-info/
--rw-rw-rw-   0        0        0      478 2023-04-05 11:41:45.000000 KIF-0.2.0/KIF.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      894 2023-04-05 11:41:45.000000 KIF-0.2.0/KIF.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 11:41:45.000000 KIF-0.2.0/KIF.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-04-05 11:41:45.000000 KIF-0.2.0/KIF.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-04-05 11:41:45.000000 KIF-0.2.0/KIF.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    18431 2022-09-22 10:55:30.000000 KIF-0.2.0/LICENSE.md
--rw-rw-rw-   0        0        0      478 2023-04-05 11:41:45.466198 KIF-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    10596 2023-04-05 11:38:25.000000 KIF-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-05 11:41:45.417193 KIF-0.2.0/key_interactions_finder/
--rw-rw-rw-   0        0        0        0 2021-12-19 18:36:56.000000 KIF-0.2.0/key_interactions_finder/__init__.py
--rw-rw-rw-   0        0        0    10228 2023-04-05 11:38:25.000000 KIF-0.2.0/key_interactions_finder/contact_identification.py
--rw-rw-rw-   0        0        0    15396 2023-04-05 11:38:25.000000 KIF-0.2.0/key_interactions_finder/data_preperation.py
--rw-rw-rw-   0        0        0    35948 2023-03-29 13:17:18.000000 KIF-0.2.0/key_interactions_finder/model_building.py
-drwxrwxrwx   0        0        0        0 2023-04-05 11:41:45.464234 KIF-0.2.0/key_interactions_finder/model_params/
--rw-rw-rw-   0        0        0      418 2022-08-15 09:07:57.000000 KIF-0.2.0/key_interactions_finder/model_params/gridsearch_custom.json
--rw-rw-rw-   0        0        0     4457 2022-08-15 08:59:17.000000 KIF-0.2.0/key_interactions_finder/model_params/gridsearch_exhaustive.json
--rw-rw-rw-   0        0        0     3003 2022-08-15 09:00:56.000000 KIF-0.2.0/key_interactions_finder/model_params/gridsearch_moderate.json
--rw-rw-rw-   0        0        0     1159 2022-03-02 11:45:57.000000 KIF-0.2.0/key_interactions_finder/model_params/gridsearch_none.json
--rw-rw-rw-   0        0        0     1471 2022-08-15 09:01:34.000000 KIF-0.2.0/key_interactions_finder/model_params/gridsearch_quick.json
--rw-rw-rw-   0        0        0    14942 2023-03-29 12:27:54.000000 KIF-0.2.0/key_interactions_finder/network_analysis.py
--rw-rw-rw-   0        0        0    36620 2023-03-29 13:17:18.000000 KIF-0.2.0/key_interactions_finder/post_proccessing.py
--rw-rw-rw-   0        0        0    17183 2023-03-29 13:17:18.000000 KIF-0.2.0/key_interactions_finder/pycontact_processing.py
--rw-rw-rw-   0        0        0    11503 2023-03-29 13:17:18.000000 KIF-0.2.0/key_interactions_finder/pymol_projections.py
--rw-rw-rw-   0        0        0    19316 2023-03-29 13:17:18.000000 KIF-0.2.0/key_interactions_finder/stat_modelling.py
--rw-rw-rw-   0        0        0     7786 2023-04-05 11:38:25.000000 KIF-0.2.0/key_interactions_finder/utils.py
--rw-rw-rw-   0        0        0       42 2023-04-05 11:41:45.468200 KIF-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1027 2023-04-05 11:38:25.000000 KIF-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:27:55.660726 KIF-0.3.0/
+drwxrwxrwx   0        0        0        0 2023-07-14 15:27:55.582602 KIF-0.3.0/KIF.egg-info/
+-rw-rw-rw-   0        0        0      439 2023-07-14 15:27:55.000000 KIF-0.3.0/KIF.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      948 2023-07-14 15:27:55.000000 KIF-0.3.0/KIF.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 15:27:55.000000 KIF-0.3.0/KIF.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2023-07-14 15:27:55.000000 KIF-0.3.0/KIF.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-07-14 15:27:55.000000 KIF-0.3.0/KIF.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    18431 2022-09-22 10:55:30.000000 KIF-0.3.0/LICENSE.md
+-rw-rw-rw-   0        0        0      439 2023-07-14 15:27:55.660726 KIF-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10602 2023-06-06 09:10:36.000000 KIF-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 15:27:55.645132 KIF-0.3.0/key_interactions_finder/
+-rw-rw-rw-   0        0        0        0 2021-12-19 18:36:56.000000 KIF-0.3.0/key_interactions_finder/__init__.py
+-rw-rw-rw-   0        0        0    12306 2023-07-14 15:10:53.000000 KIF-0.3.0/key_interactions_finder/contact_identification.py
+-rw-rw-rw-   0        0        0    10177 2023-07-14 09:23:12.000000 KIF-0.3.0/key_interactions_finder/contact_identification_old.py
+-rw-rw-rw-   0        0        0    15396 2023-04-05 11:38:25.000000 KIF-0.3.0/key_interactions_finder/data_preperation.py
+-rw-rw-rw-   0        0        0    35948 2023-03-29 13:17:18.000000 KIF-0.3.0/key_interactions_finder/model_building.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:27:55.660726 KIF-0.3.0/key_interactions_finder/model_params/
+-rw-rw-rw-   0        0        0      418 2022-08-15 09:07:57.000000 KIF-0.3.0/key_interactions_finder/model_params/gridsearch_custom.json
+-rw-rw-rw-   0        0        0     4457 2022-08-15 08:59:17.000000 KIF-0.3.0/key_interactions_finder/model_params/gridsearch_exhaustive.json
+-rw-rw-rw-   0        0        0     3003 2022-08-15 09:00:56.000000 KIF-0.3.0/key_interactions_finder/model_params/gridsearch_moderate.json
+-rw-rw-rw-   0        0        0     1159 2022-03-02 11:45:57.000000 KIF-0.3.0/key_interactions_finder/model_params/gridsearch_none.json
+-rw-rw-rw-   0        0        0     1471 2022-08-15 09:01:34.000000 KIF-0.3.0/key_interactions_finder/model_params/gridsearch_quick.json
+-rw-rw-rw-   0        0        0    14426 2023-07-14 15:10:53.000000 KIF-0.3.0/key_interactions_finder/network_analysis.py
+-rw-rw-rw-   0        0        0    36620 2023-03-29 13:17:18.000000 KIF-0.3.0/key_interactions_finder/post_proccessing.py
+-rw-rw-rw-   0        0        0    17183 2023-03-29 13:17:18.000000 KIF-0.3.0/key_interactions_finder/pycontact_processing.py
+-rw-rw-rw-   0        0        0    11503 2023-03-29 13:17:18.000000 KIF-0.3.0/key_interactions_finder/pymol_projections.py
+-rw-rw-rw-   0        0        0    19316 2023-03-29 13:17:18.000000 KIF-0.3.0/key_interactions_finder/stat_modelling.py
+-rw-rw-rw-   0        0        0     7786 2023-04-05 11:38:25.000000 KIF-0.3.0/key_interactions_finder/utils.py
+-rw-rw-rw-   0        0        0       42 2023-07-14 15:27:55.660726 KIF-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      978 2023-07-14 15:11:43.000000 KIF-0.3.0/setup.py
```

### Comparing `KIF-0.2.0/KIF.egg-info/SOURCES.txt` & `KIF-0.3.0/KIF.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 KIF.egg-info/PKG-INFO
 KIF.egg-info/SOURCES.txt
 KIF.egg-info/dependency_links.txt
 KIF.egg-info/requires.txt
 KIF.egg-info/top_level.txt
 key_interactions_finder/__init__.py
 key_interactions_finder/contact_identification.py
+key_interactions_finder/contact_identification_old.py
 key_interactions_finder/data_preperation.py
 key_interactions_finder/model_building.py
 key_interactions_finder/network_analysis.py
 key_interactions_finder/post_proccessing.py
 key_interactions_finder/pycontact_processing.py
 key_interactions_finder/pymol_projections.py
 key_interactions_finder/stat_modelling.py
```

### Comparing `KIF-0.2.0/LICENSE.md` & `KIF-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `KIF-0.2.0/README.md` & `KIF-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # KIF - Key Interactions Finder
  A python package to identify the key molecular interactions that regulate any conformational change.
 
  ### New in Version 0.2.0  - (05/04/2023)
-Now non-covalent interactions can be identified directly from a trajectory using KIF, just make sure you're trajecory is [imaged](http://ambermd.org/Questions/periodic2.html), as you would normally do so.
+Now non-covalent interactions can be identified directly from a trajectory using KIF, just make sure your trajectory is [imaged](http://ambermd.org/Questions/periodic2.html), as you would normally do so.
 
 **Note** - If you have already used PyContact (the prior method to calculate non-covalent interactions) don't worry, you can still use the PyContact generated dataset in the newer version(s) of KIF.
 
 In order to use this feature you'll need to update your install of KIF to at least 0.2.0 or greater:
 ```
 pip install --upgrade KIF
 ```
 
 ![KIF_ReadMe_Pic](https://user-images.githubusercontent.com/49672044/207597051-7dcde86a-62bd-4f69-96aa-326cad938a65.png)
 
 
 ## In short, this package allows you to:
- - Identify important non-covalent interactions that are associated with any conformational you are interested in (as long as you can describe the descriptor and sample the descriptor in your MD simulations). The non-covalent interactions are scored according to their association/importance to the conformational change and you can easily convert the per interaction/feature scores to per residue scores as well.
+ - Identify important non-covalent interactions that are associated with any conformational change you are interested in (as long as you can describe the descriptor and sample the descriptor in your MD simulations). The non-covalent interactions are scored according to their association/importance to the conformational change and you can easily convert the per interaction/feature scores to per residue scores as well.
  - Generate [PyMOL](https://pymol.org/2/) output scripts that enable you to visualise your results on 3D structures.
  - Generate per residue correlation and distance matrices that can be easily applied to the many graph theory methods available in order to study protein interaction networks and allostery within your system (no descriptor/target variable required for this).
 
 Note that how you define the descriptor is up to you, and you can use either a continuous variable or a categorical variable (some tips on how to decide what to use will be given below).
 
 **More Detail Please!**
 For a more complete description of KIF, [please refer to our article](https://aip.scitation.org/doi/10.1063/5.0140882). Included in the article is a description of some of the generic workflows possible alongside the application of KIF to several different biomolecular systems.
```

### Comparing `KIF-0.2.0/key_interactions_finder/contact_identification.py` & `KIF-0.3.0/key_interactions_finder/contact_identification_old.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,23 +32,26 @@
 NEGATIVE_SB_RESIDUES = ("GLU", "ASP")
 HYDROPHOBIC_RESIDUES = ("ALA", "VAL", "LEU", "ILE", "PRO", "PHE", "Cys")
 
 
 # From clarification on GitHub, this message can be safely ignored.
 # https://github.com/MDAnalysis/mdanalysis/issues/3889
 warnings.filterwarnings(
-    "ignore", message="DCDReader currently makes independent timesteps")
+    "ignore", message="DCDReader currently makes independent timesteps"
+)
 
 
-def calculate_contacts(parm_file: str,
-                       traj_file: str,
-                       out_file: str,
-                       first_res: Optional[int] = None,
-                       last_res: Optional[int] = None,
-                       report_timings: bool = True) -> None:
+def calculate_contacts(
+    parm_file: str,
+    traj_file: str,
+    out_file: str,
+    first_res: Optional[int] = None,
+    last_res: Optional[int] = None,
+    report_timings: bool = True,
+) -> None:
     """
     Identify all non-covalent interactions present in the simulation and save the output.
     Output has each non-covalent interaction as a column
     each column has the following information: [residue1] [residue2] [interaction type]
 
     Parameters
     ----------
@@ -80,14 +83,15 @@
     -------
     None
         Output written to file. Optional timings printed to the console.
     """
     if report_timings:
         import time
         from datetime import timedelta
+
         start_time = time.monotonic()
 
     universe = Universe(parm_file, traj_file)
 
     if first_res is None:
         first_res = 1
     if last_res is None:
@@ -98,63 +102,69 @@
     all_contact_scores = {}
     for res1 in range(first_res, last_res + 1):
         res1_sele = "not name H* and resid " + str(res1)
         res1_atoms = universe.select_atoms(res1_sele)
 
         # symmetrical matrix along diagonal, hence loop style.
         for res2 in range(res1, len(universe.residues) + 1):
-
             res_delta = abs(res1 - res2)
             if res_delta <= 2:  # neighbour residues should have 0 score
                 continue
 
             res2_sele = "not name H* and resid " + str(res2)
             res2_atoms = universe.select_atoms(res2_sele)
 
             contact_scores = []
             for timestep in universe.trajectory:
                 res_res_dists = contacts.distance_array(
-                    res1_atoms.positions,
-                    res2_atoms.positions
+                    res1_atoms.positions, res2_atoms.positions
                 )
-                contact_score = _score_residue_contact(
-                    res_res_dists=res_res_dists)
+                contact_score = _score_residue_contact(res_res_dists=res_res_dists)
                 contact_scores.append(contact_score)
 
             # save contact only if non-negligible interaction present
-            avg_contact_score = sum(
-                contact_scores) / len(universe.trajectory)
+            avg_contact_score = sum(contact_scores) / len(universe.trajectory)
             if avg_contact_score > 0.1:
-
                 # -1 as 0 indexed...
-                res1_name = universe.residues[res1-1].resname.capitalize()
-                res2_name = universe.residues[res2-1].resname.capitalize()
+                res1_name = universe.residues[res1 - 1].resname.capitalize()
+                res2_name = universe.residues[res2 - 1].resname.capitalize()
 
                 interaction_type = _determine_interaction_type(
-                    res1_id=res1, res2_id=res2,
-                    hbond_pairs=hbond_pairs, universe=universe
+                    res1_id=res1,
+                    res2_id=res2,
+                    hbond_pairs=hbond_pairs,
+                    universe=universe,
                 )
 
-                contact_label = str(res1) + res1_name + " " + \
-                    str(res2) + res2_name + " " + interaction_type
+                contact_label = (
+                    str(res1)
+                    + res1_name
+                    + " "
+                    + str(res2)
+                    + res2_name
+                    + " "
+                    + interaction_type
+                )
                 all_contact_scores.update({contact_label: contact_scores})
 
     df_contact_scores = pd.DataFrame(all_contact_scores)
     df_contact_scores.to_csv(out_file, index=False)
 
     if report_timings:
         end_time = time.monotonic()
         delta_time = timedelta(seconds=end_time - start_time)
         print(f"Time taken: {delta_time}")
 
 
 # helper functions below.
 
-def _atom_num_to_res_info(atom_num: int,
-                          universe: MDAnalysis.core.universe.Universe) -> Tuple[str, int]:
+
+def _atom_num_to_res_info(
+    atom_num: int, universe: MDAnalysis.core.universe.Universe
+) -> Tuple[str, int]:
     """
     From an MDAnalysis atom number and universe, obtain the residue number
     and residue name.
 
     Parameters
     ----------
     atom_num: int
@@ -202,29 +212,31 @@
     hbond_results = hbonds.results.hbonds
 
     # Make list of all hbond residue pairs.
     hbond_pairs = []
     for observation in hbond_results:
         donor_atom, acceptor_atom = observation[1], observation[3]
 
-        donor_resid = _atom_num_to_res_info(
-            atom_num=donor_atom, universe=universe)[1]
+        donor_resid = _atom_num_to_res_info(atom_num=donor_atom, universe=universe)[1]
         acceptor_resid = _atom_num_to_res_info(
-            atom_num=acceptor_atom, universe=universe)[1]
+            atom_num=acceptor_atom, universe=universe
+        )[1]
 
         if (donor_resid, acceptor_resid) not in hbond_pairs:
             hbond_pairs.append((donor_resid, acceptor_resid))
 
     return hbond_pairs
 
 
-def _determine_interaction_type(res1_id: int,
-                                res2_id: int,
-                                hbond_pairs: List[tuple],
-                                universe: MDAnalysis.core.universe.Universe) -> str:
+def _determine_interaction_type(
+    res1_id: int,
+    res2_id: int,
+    hbond_pairs: List[tuple],
+    universe: MDAnalysis.core.universe.Universe,
+) -> str:
     """
     Determine the interaction type for a residue pair. Options are:
     hydrogen bond, salt bridge, hydrophobic and VdW's interaction.
 
     Parameters
     ----------
     res1_id:int
```

### Comparing `KIF-0.2.0/key_interactions_finder/data_preperation.py` & `KIF-0.3.0/key_interactions_finder/data_preperation.py`

 * *Files identical despite different names*

### Comparing `KIF-0.2.0/key_interactions_finder/model_building.py` & `KIF-0.3.0/key_interactions_finder/model_building.py`

 * *Files identical despite different names*

### Comparing `KIF-0.2.0/key_interactions_finder/model_params/gridsearch_exhaustive.json` & `KIF-0.3.0/key_interactions_finder/model_params/gridsearch_exhaustive.json`

 * *Files identical despite different names*

### Comparing `KIF-0.2.0/key_interactions_finder/model_params/gridsearch_moderate.json` & `KIF-0.3.0/key_interactions_finder/model_params/gridsearch_moderate.json`

 * *Files identical despite different names*

### Comparing `KIF-0.2.0/key_interactions_finder/model_params/gridsearch_none.json` & `KIF-0.3.0/key_interactions_finder/model_params/gridsearch_none.json`

 * *Files identical despite different names*

### Comparing `KIF-0.2.0/key_interactions_finder/model_params/gridsearch_quick.json` & `KIF-0.3.0/key_interactions_finder/model_params/gridsearch_quick.json`

 * *Files identical despite different names*

### Comparing `KIF-0.2.0/key_interactions_finder/network_analysis.py` & `KIF-0.3.0/key_interactions_finder/network_analysis.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         are in contact with each other.
 
     gen_res_correl_matrix(out_file)
         For every residue to every other residue determine the interaction (if exists)
         with the strongest correlation between them and use it to build a per residue
         correlation matrix.
     """
+
     dataset: pd.DataFrame
 
     # Generated during init.
     feature_corr_matrix: pd.DataFrame = field(init=False)
 
     def __post_init__(self):
         """Filter features and generate the full correlation matrix."""
@@ -69,55 +70,48 @@
         Returns
         ----------
         np.ndarray
             A symmetrical matrix (along diagonal) of correlations between each residue.
         """
         # Generate an empty correlation matrix for all residues.
         last_residue = self._get_last_residue()
-        per_res_corr_matrix = np.zeros(
-            (last_residue, last_residue), dtype=float)
+        per_res_corr_matrix = np.zeros((last_residue, last_residue), dtype=float)
 
         # Filter correlation matrix to only include columns with specific res number.
-        for res1 in range(1, last_residue+1):
+        for res1 in range(1, last_residue + 1):
             res1_regex_key = self._build_regex_strs(res_number=res1)
-            res1_matrix = self.feature_corr_matrix.filter(
-                regex=res1_regex_key, axis=1)
+            res1_matrix = self.feature_corr_matrix.filter(regex=res1_regex_key, axis=1)
 
             # Filter matrix on other axis so matrix contains only the pairs of residues.
             if len(res1_matrix.columns) != 0:
-                for res2 in range(1, last_residue+1):
+                for res2 in range(res1 + 1, last_residue + 1):
                     res2_regex_key = self._build_regex_strs(res_number=res2)
-                    res1_res2_matrix = res1_matrix.filter(
-                        regex=res2_regex_key, axis=0)
+                    res1_res2_matrix = res1_matrix.filter(regex=res2_regex_key, axis=0)
 
                     if len(res1_res2_matrix) != 0:
                         correls = res1_res2_matrix.to_numpy()
 
                         try:
                             # prevent identical interactions (== 1) being used.
                             correls = correls[correls != 1]
-                            max_correl = max(
-                                correls.min(), correls.max(), key=abs)
+                            max_correl = max(correls.min(), correls.max(), key=abs)
 
-                            per_res_corr_matrix[(
-                                res1-1), (res2-1)] = max_correl
-                            per_res_corr_matrix[(
-                                res2-1), (res1-1)] = max_correl
+                            per_res_corr_matrix[(res1 - 1), (res2 - 1)] = max_correl
+                            per_res_corr_matrix[(res2 - 1), (res1 - 1)] = max_correl
 
                         # ValueError will happen if array becomes empty
                         # when only identical interactions were present in matrix.
                         except ValueError:
                             pass  # value stays at 0.
 
         # correlation of residue to itself is 1.
         np.fill_diagonal(per_res_corr_matrix, 1)
 
         if out_file is not None:
-            np.savetxt(out_file, per_res_corr_matrix,
-                       delimiter=" ", fmt="%.2f")
+            np.savetxt(out_file, per_res_corr_matrix, delimiter=" ", fmt="%.2f")
             print(f"{out_file} saved to disk.")
 
         return per_res_corr_matrix
 
     def gen_res_contact_matrix(self, out_file: Optional[str] = None) -> np.ndarray:
         """
         Generate a per residue contact map (matrix) that identifies whether two residues
@@ -132,48 +126,43 @@
         Returns
         ----------
         np.ndarray
             A symmetrical matrix (along diagonal) of 1s (in contact) and 0s (not in contact).
         """
         # Generate empty matrix for each residue
         last_residue = self._get_last_residue()
-        per_res_contact_matrix = np.zeros(
-            (last_residue, last_residue), dtype=int)
+        per_res_contact_matrix = np.zeros((last_residue, last_residue), dtype=int)
 
         contact_pairs = self._get_contact_pairs()
         for res1, res2 in contact_pairs.items():
-            per_res_contact_matrix[(res1-1), (res2-1)] = 1
-            per_res_contact_matrix[(res2-1), (res1-1)] = 1
+            per_res_contact_matrix[(res1 - 1), (res2 - 1)] = 1
+            per_res_contact_matrix[(res2 - 1), (res1 - 1)] = 1
 
         # correlation of residue to itself is 1.
         np.fill_diagonal(per_res_contact_matrix, 1)
 
         if out_file is not None:
-            np.savetxt(out_file, per_res_contact_matrix,
-                       delimiter=" ", fmt="%.2f")
+            np.savetxt(out_file, per_res_contact_matrix, delimiter=" ", fmt="%.2f")
             print(f"{out_file} saved to disk.")
 
         return per_res_contact_matrix
 
     def _get_residue_lists(self) -> pd.DataFrame:
         """
         Given a dataframe (self.dataset) containing only PyContact features,
         extract the residue numbers for each contact. (Helper Function.)
 
         Returns
         ----------
         pd.DataFrame
             1st and 2nd residue number of each contact/feature in the dataframe.
         """
-        df_cols = pd.DataFrame(list(self.dataset.columns),
-                               columns=["Feature_Names"])
-        df_cols["Res1"] = df_cols["Feature_Names"].str.split(
-            "[a-zA-Z]+").str.get(0)
-        df_cols["Res2"] = df_cols["Feature_Names"].str.split(
-            "[a-zA-Z]+").str.get(1)
+        df_cols = pd.DataFrame(list(self.dataset.columns), columns=["Feature_Names"])
+        df_cols["Res1"] = df_cols["Feature_Names"].str.split("[a-zA-Z]+").str.get(0)
+        df_cols["Res2"] = df_cols["Feature_Names"].str.split("[a-zA-Z]+").str.get(1)
         df_cols["Res1"] = pd.to_numeric(df_cols["Res1"])
         df_cols["Res2"] = pd.to_numeric(df_cols["Res2"])
         return df_cols[["Res1", "Res2"]]
 
     def _get_last_residue(self) -> int:
         """
         Given a dataframe (self.dataset) containing only PyContact features,
@@ -233,20 +222,21 @@
 
         # matches if target res number is 2nd residue in name
         regex_key_p2 = " " + str(res_number) + "([A-Za-z]{3})" + " "
 
         return regex_key_p1 + "|" + regex_key_p2
 
 
-def heavy_atom_contact_map_from_pdb(pdb_file: str,
-                                    first_res: int,
-                                    last_res: int,
-                                    d_cut: Optional[float] = 4.5,
-                                    out_file: Optional[str] = None,
-                                    ) -> np.ndarray:
+def heavy_atom_contact_map_from_pdb(
+    pdb_file: str,
+    first_res: int,
+    last_res: int,
+    d_cut: Optional[float] = 4.5,
+    out_file: Optional[str] = None,
+) -> np.ndarray:
     """
     Use MDAnalysis to generate a heavy atom contact map/matrix given a single PDB file.
     If 'out_file' specified the result will be saved to disk.
 
     Parameters
     ----------
     pdb_file: str
@@ -266,52 +256,53 @@
 
     Returns
     ----------
     np.ndarray
         Symmetrical (along diagonal) matrix of 1s (in contact) and 0s (not in contact).
     """
     universe = mda.Universe(pdb_file)
-    res_selection = "not name H* and resid " + \
-        str(first_res) + "-" + str(last_res)
+    res_selection = "not name H* and resid " + str(first_res) + "-" + str(last_res)
     group1 = universe.select_atoms(res_selection)
     group2 = universe.select_atoms(res_selection)
     matrix_size = (last_res - first_res) + 1
 
     per_res_contact_map = np.zeros((matrix_size, matrix_size), dtype=int)
 
-    for group1_idx in range(first_res, last_res+1):
+    for group1_idx in range(first_res, last_res + 1):
         group1_selection = "resid " + str(group1_idx)
         res1 = group1.select_atoms(group1_selection)
 
-        for group2_idx in range(first_res, last_res+1):
+        for group2_idx in range(group1_idx, last_res + 1):
             group2_selection = "resid " + str(group2_idx)
             res2 = group2.select_atoms(group2_selection)
 
             # Determine all heavy atom distance between residue pairs.
             dist_arr = distances.distance_array(
-                res1.positions, res2.positions, box=universe.dimensions)
+                res1.positions, res2.positions, box=universe.dimensions
+            )
 
             # Replace matrix pos with 1 if min_dist less than cutoff.
             min_dist = dist_arr.min()
             if min_dist <= d_cut:
-                per_res_contact_map[(group1_idx-1), (group2_idx-1)] = 1
-                per_res_contact_map[(group2_idx-1), (group1_idx-1)] = 1
+                per_res_contact_map[(group1_idx - 1), (group2_idx - 1)] = 1
+                per_res_contact_map[(group2_idx - 1), (group1_idx - 1)] = 1
 
     if out_file is not None:
         np.savetxt(out_file, per_res_contact_map, delimiter=" ", fmt="%.1f")
         print(f"{out_file} saved to disk.")
     return per_res_contact_map
 
 
-def heavy_atom_contact_map_from_multiple_pdbs(pdb_files: list,
-                                              first_res: int,
-                                              last_res: int,
-                                              d_cut: Optional[float] = 4.5,
-                                              out_file: Optional[str] = None,
-                                              ) -> np.ndarray:
+def heavy_atom_contact_map_from_multiple_pdbs(
+    pdb_files: list,
+    first_res: int,
+    last_res: int,
+    d_cut: Optional[float] = 4.5,
+    out_file: Optional[str] = None,
+) -> np.ndarray:
     """
     Use MDAnalysis to generate a heavy atom contact map/matrix given a list of PDB files.
     If 'out_file' specified the result will be saved to disk.
 
     Parameters
     ----------
     pdb_file: list
@@ -331,53 +322,60 @@
 
     Returns
     ----------
     np.ndarray
         Symmetrical (along diagonal) matrix of 1s (in contact) and 0s (not in contact).
 
     """
-    res_selection = "not name H* and resid " + \
-        str(first_res) + "-" + str(last_res)
+    res_selection = "not name H* and resid " + str(first_res) + "-" + str(last_res)
 
     all_universes = [mda.Universe(pdb) for pdb in pdb_files]
 
-    all_group1s = [all_universes[idx].select_atoms(
-        res_selection) for idx, _ in enumerate(all_universes)]
-    all_group2s = [all_universes[idx].select_atoms(
-        res_selection) for idx, _ in enumerate(all_universes)]
+    all_group1s = [
+        all_universes[idx].select_atoms(res_selection)
+        for idx, _ in enumerate(all_universes)
+    ]
+    all_group2s = [
+        all_universes[idx].select_atoms(res_selection)
+        for idx, _ in enumerate(all_universes)
+    ]
 
     matrix_size = (last_res - first_res) + 1
     per_res_contact_map = np.zeros((matrix_size, matrix_size), dtype=int)
 
-    for group1_idx in range(first_res, last_res+1):
+    for group1_idx in range(first_res, last_res + 1):
         group1_selection = "resid " + str(group1_idx)
-        residue_1s = [all_group1s[idx].select_atoms(
-            group1_selection) for idx, _ in enumerate(all_group1s)]
+        residue_1s = [
+            all_group1s[idx].select_atoms(group1_selection)
+            for idx, _ in enumerate(all_group1s)
+        ]
 
-        for group2_idx in range(first_res, last_res+1):
+        for group2_idx in range(group1_idx, last_res + 1):
             group2_selection = "resid " + str(group2_idx)
-            residue_2s = [all_group1s[idx].select_atoms(
-                group2_selection) for idx, _ in enumerate(all_group2s)]
+            residue_2s = [
+                all_group1s[idx].select_atoms(group2_selection)
+                for idx, _ in enumerate(all_group2s)
+            ]
 
             # Find the smallest distance between the residue pairs across all pdbs
             min_dist_all_pdbs = 999  # always going to be above cut-off.
             for idx, _ in enumerate(all_group1s):
                 dist_arr = distances.distance_array(
                     residue_1s[idx].positions,
                     residue_2s[idx].positions,
-                    box=all_universes[idx].dimensions
+                    box=all_universes[idx].dimensions,
                 )
                 min_dist = dist_arr.min()
 
                 if min_dist < min_dist_all_pdbs:
                     min_dist_all_pdbs = min_dist
 
             # Replace matrix pos with 1 if min_dist_all_pdbs less than cutoff.
             if min_dist_all_pdbs <= d_cut:
-                per_res_contact_map[(group1_idx-1), (group2_idx-1)] = 1
-                per_res_contact_map[(group2_idx-1), (group1_idx-1)] = 1
+                per_res_contact_map[(group1_idx - 1), (group2_idx - 1)] = 1
+                per_res_contact_map[(group2_idx - 1), (group1_idx - 1)] = 1
 
     if out_file is not None:
         np.savetxt(out_file, per_res_contact_map, delimiter=" ", fmt="%.1f")
         print(f"{out_file} saved to disk.")
 
     return per_res_contact_map
```

### Comparing `KIF-0.2.0/key_interactions_finder/post_proccessing.py` & `KIF-0.3.0/key_interactions_finder/post_proccessing.py`

 * *Files identical despite different names*

### Comparing `KIF-0.2.0/key_interactions_finder/pycontact_processing.py` & `KIF-0.3.0/key_interactions_finder/pycontact_processing.py`

 * *Files identical despite different names*

### Comparing `KIF-0.2.0/key_interactions_finder/pymol_projections.py` & `KIF-0.3.0/key_interactions_finder/pymol_projections.py`

 * *Files identical despite different names*

### Comparing `KIF-0.2.0/key_interactions_finder/stat_modelling.py` & `KIF-0.3.0/key_interactions_finder/stat_modelling.py`

 * *Files identical despite different names*

### Comparing `KIF-0.2.0/key_interactions_finder/utils.py` & `KIF-0.3.0/key_interactions_finder/utils.py`

 * *Files identical despite different names*

### Comparing `KIF-0.2.0/setup.py` & `KIF-0.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.2.0"
+VERSION = "0.3.0"
 DESCRIPTION = "Python package for MD simulation analysis"
 LONG_DESCRIPTION = """
     A python package to identify the key molecular interactions that regulate any conformational change."""
 
-setup(name="KIF",
-      version=VERSION,
-      description=DESCRIPTION,
-      long_description=LONG_DESCRIPTION,
-      author="Rory Crean",
-      author_email="rory.crean@kemi.uu.se",
-      url="https://github.com/kamerlinlab/KIF",
-      packages=find_packages(
-          include=["key_interactions_finder"]),
-      install_requires=[
-          "pandas",
-          "numpy",
-          "scikit-learn",
-          "scipy",
-          "xgboost",
-          "catboost",
-          "MDAnalysis",
-          "MDAnalysisTests",
-          "gdown",
-      ],
-      package_data={"key_interactions_finder": ["model_params/*.json"]},
-      classifiers=[
-          "Programming Language :: Python :: 3",
-          "Operating System :: OS Independent",
-      ])
+setup(
+    name="KIF",
+    version=VERSION,
+    description=DESCRIPTION,
+    long_description=LONG_DESCRIPTION,
+    author="Rory Crean",
+    author_email="rory.crean@kemi.uu.se",
+    url="https://github.com/kamerlinlab/KIF",
+    packages=find_packages(include=["key_interactions_finder"]),
+    install_requires=[
+        "pandas",
+        "numpy",
+        "scikit-learn",
+        "scipy",
+        "xgboost",
+        "catboost",
+        "MDAnalysis",
+        "MDAnalysisTests",
+        "gdown",
+    ],
+    package_data={"key_interactions_finder": ["model_params/*.json"]},
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "Operating System :: OS Independent",
+    ],
+)
```

