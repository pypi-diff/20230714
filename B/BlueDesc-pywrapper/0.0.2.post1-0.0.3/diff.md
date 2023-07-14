# Comparing `tmp/BlueDesc_pywrapper-0.0.2.post1.tar.gz` & `tmp/BlueDesc_pywrapper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BlueDesc_pywrapper-0.0.2.post1.tar", last modified: Tue Jun 27 13:59:06 2023, max compression
+gzip compressed data, was "BlueDesc_pywrapper-0.0.3.tar", last modified: Fri Jul 14 13:19:25 2023, max compression
```

## Comparing `BlueDesc_pywrapper-0.0.2.post1.tar` & `BlueDesc_pywrapper-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 13:59:06.454673 BlueDesc_pywrapper-0.0.2.post1/
--rw-rw-rw-   0        0        0     1100 2023-06-27 11:18:36.000000 BlueDesc_pywrapper-0.0.2.post1/LICENSE
--rw-rw-rw-   0        0        0     3021 2023-06-27 13:59:06.454673 BlueDesc_pywrapper-0.0.2.post1/PKG-INFO
--rw-rw-rw-   0        0        0     2082 2023-06-27 13:48:39.000000 BlueDesc_pywrapper-0.0.2.post1/README.md
--rw-rw-rw-   0        0        0     1361 2023-06-27 13:59:06.456675 BlueDesc_pywrapper-0.0.2.post1/setup.cfg
--rw-rw-rw-   0        0        0      123 2023-06-27 11:18:36.000000 BlueDesc_pywrapper-0.0.2.post1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 13:59:06.415681 BlueDesc_pywrapper-0.0.2.post1/src/
-drwxrwxrwx   0        0        0        0 2023-06-27 13:59:06.429620 BlueDesc_pywrapper-0.0.2.post1/src/BlueDesc_pywrapper/
--rw-rw-rw-   0        0        0      148 2023-06-27 13:58:36.000000 BlueDesc_pywrapper-0.0.2.post1/src/BlueDesc_pywrapper/__init__.py
--rw-rw-rw-   0        0        0     8450 2023-06-27 13:46:44.000000 BlueDesc_pywrapper-0.0.2.post1/src/BlueDesc_pywrapper/bluedesc_pywrapper.py
--rw-rw-rw-   0        0        0     1990 2023-06-27 13:14:52.000000 BlueDesc_pywrapper-0.0.2.post1/src/BlueDesc_pywrapper/desc_names.json
--rw-rw-rw-   0        0        0     3450 2023-06-27 13:36:16.000000 BlueDesc_pywrapper-0.0.2.post1/src/BlueDesc_pywrapper/dtypes.json
--rw-rw-rw-   0        0        0     3040 2023-06-27 11:18:36.000000 BlueDesc_pywrapper-0.0.2.post1/src/BlueDesc_pywrapper/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-27 13:59:06.452681 BlueDesc_pywrapper-0.0.2.post1/src/BlueDesc_pywrapper.egg-info/
--rw-rw-rw-   0        0        0     3021 2023-06-27 13:59:06.000000 BlueDesc_pywrapper-0.0.2.post1/src/BlueDesc_pywrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      451 2023-06-27 13:59:06.000000 BlueDesc_pywrapper-0.0.2.post1/src/BlueDesc_pywrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 13:59:06.000000 BlueDesc_pywrapper-0.0.2.post1/src/BlueDesc_pywrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      172 2023-06-27 13:59:06.000000 BlueDesc_pywrapper-0.0.2.post1/src/BlueDesc_pywrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-27 13:59:06.000000 BlueDesc_pywrapper-0.0.2.post1/src/BlueDesc_pywrapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 13:19:25.104288 BlueDesc_pywrapper-0.0.3/
+-rw-rw-rw-   0        0        0     1100 2023-06-27 11:18:36.000000 BlueDesc_pywrapper-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     3151 2023-07-14 13:19:25.104288 BlueDesc_pywrapper-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2218 2023-07-14 13:15:51.000000 BlueDesc_pywrapper-0.0.3/README.md
+-rw-rw-rw-   0        0        0     1361 2023-07-14 13:19:25.115288 BlueDesc_pywrapper-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      123 2023-06-27 11:18:36.000000 BlueDesc_pywrapper-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 13:19:25.015769 BlueDesc_pywrapper-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-14 13:19:25.037281 BlueDesc_pywrapper-0.0.3/src/BlueDesc_pywrapper/
+-rw-rw-rw-   0        0        0      142 2023-07-14 13:16:06.000000 BlueDesc_pywrapper-0.0.3/src/BlueDesc_pywrapper/__init__.py
+-rw-rw-rw-   0        0        0     9577 2023-07-14 12:32:58.000000 BlueDesc_pywrapper-0.0.3/src/BlueDesc_pywrapper/bluedesc_pywrapper.py
+-rw-rw-rw-   0        0        0    36313 2023-07-14 12:26:42.000000 BlueDesc_pywrapper-0.0.3/src/BlueDesc_pywrapper/descs.json
+-rw-rw-rw-   0        0        0     3450 2023-06-27 13:36:16.000000 BlueDesc_pywrapper-0.0.3/src/BlueDesc_pywrapper/dtypes.json
+-rw-rw-rw-   0        0        0     3040 2023-06-27 11:18:36.000000 BlueDesc_pywrapper-0.0.3/src/BlueDesc_pywrapper/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-14 13:19:25.100281 BlueDesc_pywrapper-0.0.3/src/BlueDesc_pywrapper.egg-info/
+-rw-rw-rw-   0        0        0     3151 2023-07-14 13:19:24.000000 BlueDesc_pywrapper-0.0.3/src/BlueDesc_pywrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      472 2023-07-14 13:19:25.000000 BlueDesc_pywrapper-0.0.3/src/BlueDesc_pywrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 13:19:24.000000 BlueDesc_pywrapper-0.0.3/src/BlueDesc_pywrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      172 2023-07-14 13:19:24.000000 BlueDesc_pywrapper-0.0.3/src/BlueDesc_pywrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-14 13:19:24.000000 BlueDesc_pywrapper-0.0.3/src/BlueDesc_pywrapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 13:19:25.103288 BlueDesc_pywrapper-0.0.3/tests/
+-rw-rw-rw-   0        0        0     2021 2023-07-14 13:08:16.000000 BlueDesc_pywrapper-0.0.3/tests/test_descriptors.py
```

### Comparing `BlueDesc_pywrapper-0.0.2.post1/LICENSE` & `BlueDesc_pywrapper-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `BlueDesc_pywrapper-0.0.2.post1/PKG-INFO` & `BlueDesc_pywrapper-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BlueDesc_pywrapper
-Version: 0.0.2.post1
+Version: 0.0.3
 Summary: Python wrapper for BlueDesc molecular descriptors
 Home-page: https://github.com/OlivierBeq/bluedesc_pywrapper
 Author: Olivier J. M. Béquignon
 Author-email: "olivier.bequignon.maintainer@gmail.com"
 Maintainer: Olivier J. M. Béquignon
 Maintainer-email: "olivier.bequignon.maintainer@gmail.com"
 Keywords: BlueDesc,molecular descriptors,cheminformatics,toxicoinformatics,QSAR
@@ -47,34 +47,40 @@
 smiles_list = [
   # erlotinib
   "n1cnc(c2cc(c(cc12)OCCOC)OCCOC)Nc1cc(ccc1)C#C",
   # midecamycin
   "CCC(=O)O[C@@H]1CC(=O)O[C@@H](C/C=C/C=C/[C@@H]([C@@H](C[C@@H]([C@@H]([C@H]1OC)O[C@H]2[C@@H]([C@H]([C@@H]([C@H](O2)C)O[C@H]3C[C@@]([C@H]([C@@H](O3)C)OC(=O)CC)(C)O)N(C)C)O)CC=O)C)O)C",
   # selenofolate
   "C1=CC(=CC=C1C(=O)NC(CCC(=O)OCC[Se]C#N)C(=O)O)NCC2=CN=C3C(=N2)C(=O)NC(=N3)N",
-  # cisplatin
-  "N.N.Cl[Pt]Cl"
 ]
 mols = [Chem.AddHs(Chem.MolFromSmiles(smiles)) for smiles in smiles_list]
 for mol in mols:
     _ = AllChem.EmbedMolecule(mol)
 
 bluedesc = BlueDesc()
 print(bluedesc.calculate(mols))
 ```
 
-The above calculates 174 molecular descriptors (33 1D, 85 2D and 56 3D).<br/>
-:warning: Molecules are required to have conformers for descriptors to be calculated.<br/>
+The above calculates 118 molecular descriptors (33 1D and 85 2D).<br/>
 :warning: BlueDesc skips molecules it cannot parse internally, a warning is given when that is the case.
 The following command is recommended, should this occur, to prevent the unalignment of input and output indices.
 
 ```python
 bluedesc.calculate(mols, chunksize=1, njobs=-1)
 ```
 
+The additional 56 three-dimensional (3D) descriptors may be computed like so: 
+:warning: Molecules are required to have conformers for 3D descriptors to be calculated.<br/>
+
+```python
+bluedesc = BlueDesc(ignore_3D=False)
+print(bluedesc.calculate(mols))
+
+```
+
 ## Documentation
 
 ```python
 def calculate(mols, show_banner=True, njobs=1, chunksize=1000):
 ```
 
 Default method to calculate BlueDesc fingerprints.
```

### Comparing `BlueDesc_pywrapper-0.0.2.post1/README.md` & `BlueDesc_pywrapper-0.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -25,34 +25,40 @@
 smiles_list = [
   # erlotinib
   "n1cnc(c2cc(c(cc12)OCCOC)OCCOC)Nc1cc(ccc1)C#C",
   # midecamycin
   "CCC(=O)O[C@@H]1CC(=O)O[C@@H](C/C=C/C=C/[C@@H]([C@@H](C[C@@H]([C@@H]([C@H]1OC)O[C@H]2[C@@H]([C@H]([C@@H]([C@H](O2)C)O[C@H]3C[C@@]([C@H]([C@@H](O3)C)OC(=O)CC)(C)O)N(C)C)O)CC=O)C)O)C",
   # selenofolate
   "C1=CC(=CC=C1C(=O)NC(CCC(=O)OCC[Se]C#N)C(=O)O)NCC2=CN=C3C(=N2)C(=O)NC(=N3)N",
-  # cisplatin
-  "N.N.Cl[Pt]Cl"
 ]
 mols = [Chem.AddHs(Chem.MolFromSmiles(smiles)) for smiles in smiles_list]
 for mol in mols:
     _ = AllChem.EmbedMolecule(mol)
 
 bluedesc = BlueDesc()
 print(bluedesc.calculate(mols))
 ```
 
-The above calculates 174 molecular descriptors (33 1D, 85 2D and 56 3D).<br/>
-:warning: Molecules are required to have conformers for descriptors to be calculated.<br/>
+The above calculates 118 molecular descriptors (33 1D and 85 2D).<br/>
 :warning: BlueDesc skips molecules it cannot parse internally, a warning is given when that is the case.
 The following command is recommended, should this occur, to prevent the unalignment of input and output indices.
 
 ```python
 bluedesc.calculate(mols, chunksize=1, njobs=-1)
 ```
 
+The additional 56 three-dimensional (3D) descriptors may be computed like so: 
+:warning: Molecules are required to have conformers for 3D descriptors to be calculated.<br/>
+
+```python
+bluedesc = BlueDesc(ignore_3D=False)
+print(bluedesc.calculate(mols))
+
+```
+
 ## Documentation
 
 ```python
 def calculate(mols, show_banner=True, njobs=1, chunksize=1000):
 ```
 
 Default method to calculate BlueDesc fingerprints.
```

### Comparing `BlueDesc_pywrapper-0.0.2.post1/setup.cfg` & `BlueDesc_pywrapper-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `BlueDesc_pywrapper-0.0.2.post1/src/BlueDesc_pywrapper/bluedesc_pywrapper.py` & `BlueDesc_pywrapper-0.0.3/src/BlueDesc_pywrapper/bluedesc_pywrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,16 +27,20 @@
 class BlueDesc:
     """Wrapper to obtain molecular descriptor from BlueDesc."""
 
     lock = multiprocessing.RLock()  # Ensure installation of JRE is thread safe
     # Path to the JAR file
     _jarfile = BLUEDESC_EXEC_PATH
 
-    def __init__(self):
-        """Instantiate a wrapper to calculate BlueDesc molecular descriptors."""
+    def __init__(self, ignore_3D: bool = True):
+        """Instantiate a wrapper to calculate BlueDesc molecular descriptors.
+
+        :param ignore_3D: whether to include 3D molecular descriptors
+        """
+        self.include_3D = not ignore_3D
         # Ensure the jar file exists
         if not os.path.isfile(self._jarfile):
             raise IOError('The required BlueDesc JAR file is not present. Reinstall BlueDesc.')
 
     def calculate(self, mols: Iterable[Chem.Mol], show_banner: bool = True, njobs: int = 1,
                   chunksize: Optional[int] = 1000) -> pd.DataFrame:
         """Calculate molecular fingerprints.
@@ -102,17 +106,18 @@
                 if mol is not None and isinstance(mol, Chem.Mol):
                     if mol.GetNumAtoms() > 999:
                         raise ValueError('Cannot calculate descriptors for molecules with more than 999 atoms.')
                     # Does molecule lack hydrogen atoms?
                     if needsHs(mol):
                         warnings.warn('Molecule lacks hydrogen atoms: this might affect the value of calculated descriptors')
                     # Are molecules 3D
-                    confs = list(mol.GetConformers())
-                    if not (len(confs) > 0 and confs[-1].Is3D()):
-                        raise ValueError('Cannot calculate the 3D descriptors of a conformer-less molecule')
+                    if self.include_3D:
+                        confs = list(mol.GetConformers())
+                        if not (len(confs) > 0 and confs[-1].Is3D()):
+                            raise ValueError('Cannot calculate the 3D descriptors of a conformer-less molecule')
                     writer.write(mol)
                 else:
                     self._skipped.append(i)
                 self.n += 1
             writer.close()
             del block
         except ValueError as e:
@@ -147,20 +152,25 @@
                           .drop("'?'", axis=1)
                           .rename(columns=lambda x: x.replace('joelib2.feature.types.count.', ''))
                           .rename(columns=lambda x: x.replace('joelib2.feature.types.', ''))
                           )
                 if values.shape[0] != self.n:
                     warnings.warn('Some molecules were skipped by BlueDesc')
             except:
-                values = np.zeros((self.n, 174))
-                with open(os.path.abspath(os.path.join(__file__, os.pardir, 'desc_names.json'))) as fh:
-                    names = json.load(fh)
+                details = self.get_details()
+                values = np.zeros((self.n, details.shape[0]))
                 with open(os.path.abspath(os.path.join(__file__, os.pardir, 'dtypes.json'))) as fh:
                     dtypes = json.load(fh)
-                values = pd.DataFrame(values, columns=names).astype(dtypes)
+                values = pd.DataFrame(values, columns=details.Name.tolist()).astype(dtypes)
+            # If only 2D, remove 3D descriptors
+            if not self.include_3D:
+                # Get 3D descriptor names to remove
+                descs_3D = self.get_details()
+                descs_3D = descs_3D[descs_3D.Dimensions == '3D']
+                values = values.drop(columns=descs_3D.Name.tolist())
         else:
             self._cleanup()
             raise RuntimeError('BlueDesc did not succeed to run properly.')
         return values
 
     def _calculate(self, mols: List[Chem.Mol]) -> pd.DataFrame:
         """Calculate BlueDesc molecular descriptors on one process.
@@ -194,7 +204,21 @@
         :return: a pandas DataFrame containing all BlueDesc desciptor values
         """
         # Copy self instance to make thread safe
         bluedesc = deepcopy(self)
         # Run copy
         result = bluedesc.calculate(mols, show_banner=False, njobs=1)
         return result
+
+    @staticmethod
+    def get_details(desc_name: Optional[str] = None):
+        """Obtain details about either one or all descriptors.
+
+        :param desc_name: the name of the descriptor to obtain details about (default: None).
+        If None, returns details about all descriptors.
+        """
+        details = pd.read_json(os.path.abspath(os.path.join(__file__, os.pardir, 'descs.json')), orient='index')
+        if desc_name is not None:
+            if desc_name not in details.Name.tolist():
+                raise ValueError(f'descriptor name {desc_name} is not available')
+            details = details[details.Name == desc_name]
+        return details
```

### Comparing `BlueDesc_pywrapper-0.0.2.post1/src/BlueDesc_pywrapper/dtypes.json` & `BlueDesc_pywrapper-0.0.3/src/BlueDesc_pywrapper/dtypes.json`

 * *Files identical despite different names*

### Comparing `BlueDesc_pywrapper-0.0.2.post1/src/BlueDesc_pywrapper/utils.py` & `BlueDesc_pywrapper-0.0.3/src/BlueDesc_pywrapper/utils.py`

 * *Files identical despite different names*

### Comparing `BlueDesc_pywrapper-0.0.2.post1/src/BlueDesc_pywrapper.egg-info/PKG-INFO` & `BlueDesc_pywrapper-0.0.3/src/BlueDesc_pywrapper.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BlueDesc-pywrapper
-Version: 0.0.2.post1
+Version: 0.0.3
 Summary: Python wrapper for BlueDesc molecular descriptors
 Home-page: https://github.com/OlivierBeq/bluedesc_pywrapper
 Author: Olivier J. M. Béquignon
 Author-email: "olivier.bequignon.maintainer@gmail.com"
 Maintainer: Olivier J. M. Béquignon
 Maintainer-email: "olivier.bequignon.maintainer@gmail.com"
 Keywords: BlueDesc,molecular descriptors,cheminformatics,toxicoinformatics,QSAR
@@ -47,34 +47,40 @@
 smiles_list = [
   # erlotinib
   "n1cnc(c2cc(c(cc12)OCCOC)OCCOC)Nc1cc(ccc1)C#C",
   # midecamycin
   "CCC(=O)O[C@@H]1CC(=O)O[C@@H](C/C=C/C=C/[C@@H]([C@@H](C[C@@H]([C@@H]([C@H]1OC)O[C@H]2[C@@H]([C@H]([C@@H]([C@H](O2)C)O[C@H]3C[C@@]([C@H]([C@@H](O3)C)OC(=O)CC)(C)O)N(C)C)O)CC=O)C)O)C",
   # selenofolate
   "C1=CC(=CC=C1C(=O)NC(CCC(=O)OCC[Se]C#N)C(=O)O)NCC2=CN=C3C(=N2)C(=O)NC(=N3)N",
-  # cisplatin
-  "N.N.Cl[Pt]Cl"
 ]
 mols = [Chem.AddHs(Chem.MolFromSmiles(smiles)) for smiles in smiles_list]
 for mol in mols:
     _ = AllChem.EmbedMolecule(mol)
 
 bluedesc = BlueDesc()
 print(bluedesc.calculate(mols))
 ```
 
-The above calculates 174 molecular descriptors (33 1D, 85 2D and 56 3D).<br/>
-:warning: Molecules are required to have conformers for descriptors to be calculated.<br/>
+The above calculates 118 molecular descriptors (33 1D and 85 2D).<br/>
 :warning: BlueDesc skips molecules it cannot parse internally, a warning is given when that is the case.
 The following command is recommended, should this occur, to prevent the unalignment of input and output indices.
 
 ```python
 bluedesc.calculate(mols, chunksize=1, njobs=-1)
 ```
 
+The additional 56 three-dimensional (3D) descriptors may be computed like so: 
+:warning: Molecules are required to have conformers for 3D descriptors to be calculated.<br/>
+
+```python
+bluedesc = BlueDesc(ignore_3D=False)
+print(bluedesc.calculate(mols))
+
+```
+
 ## Documentation
 
 ```python
 def calculate(mols, show_banner=True, njobs=1, chunksize=1000):
 ```
 
 Default method to calculate BlueDesc fingerprints.
```

