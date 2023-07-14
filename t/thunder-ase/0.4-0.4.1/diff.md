# Comparing `tmp/thunder-ase-0.4.tar.gz` & `tmp/thunder-ase-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thunder-ase-0.4.tar", last modified: Tue Jun 20 09:43:19 2023, max compression
+gzip compressed data, was "thunder-ase-0.4.1.tar", last modified: Fri Jul 14 05:48:11 2023, max compression
```

## Comparing `thunder-ase-0.4.tar` & `thunder-ase-0.4.1.tar`

### file list

```diff
@@ -1,22 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:43:19.731167 thunder-ase-0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-20 09:43:19.731167 thunder-ase-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-20 09:43:07.000000 thunder-ase-0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-20 09:43:07.000000 thunder-ase-0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 09:43:19.731167 thunder-ase-0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 09:43:07.000000 thunder-ase-0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:43:19.731167 thunder-ase-0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-20 09:43:07.000000 thunder-ase-0.4/tests/test_Si_lightning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:43:19.731167 thunder-ase-0.4/thunder_ase/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:43:07.000000 thunder-ase-0.4/thunder_ase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32039 2023-06-20 09:43:07.000000 thunder-ase-0.4/thunder_ase/fireball.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:43:19.731167 thunder-ase-0.4/thunder_ase/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-20 09:43:07.000000 thunder-ase-0.4/thunder_ase/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11490 2023-06-20 09:43:07.000000 thunder-ase-0.4/thunder_ase/utils/basis_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-20 09:43:07.000000 thunder-ase-0.4/thunder_ase/utils/mwfn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-06-20 09:43:07.000000 thunder-ase-0.4/thunder_ase/utils/shell_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:43:19.731167 thunder-ase-0.4/thunder_ase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-20 09:43:19.000000 thunder-ase-0.4/thunder_ase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-20 09:43:19.000000 thunder-ase-0.4/thunder_ase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 09:43:19.000000 thunder-ase-0.4/thunder_ase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-20 09:43:19.000000 thunder-ase-0.4/thunder_ase.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-20 09:43:19.000000 thunder-ase-0.4/thunder_ase.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:48:11.485443 thunder-ase-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-07-14 05:48:11.485443 thunder-ase-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-07-14 05:48:00.000000 thunder-ase-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-14 05:48:00.000000 thunder-ase-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 05:48:11.485443 thunder-ase-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 05:48:00.000000 thunder-ase-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:48:11.485443 thunder-ase-0.4.1/thunder_ase/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:48:00.000000 thunder-ase-0.4.1/thunder_ase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32532 2023-07-14 05:48:00.000000 thunder-ase-0.4.1/thunder_ase/fireball.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:48:11.485443 thunder-ase-0.4.1/thunder_ase/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-14 05:48:00.000000 thunder-ase-0.4.1/thunder_ase/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11490 2023-07-14 05:48:00.000000 thunder-ase-0.4.1/thunder_ase/utils/basis_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-07-14 05:48:00.000000 thunder-ase-0.4.1/thunder_ase/utils/mwfn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-14 05:48:00.000000 thunder-ase-0.4.1/thunder_ase/utils/shell_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:48:11.485443 thunder-ase-0.4.1/thunder_ase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-07-14 05:48:11.000000 thunder-ase-0.4.1/thunder_ase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-14 05:48:11.000000 thunder-ase-0.4.1/thunder_ase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 05:48:11.000000 thunder-ase-0.4.1/thunder_ase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-14 05:48:11.000000 thunder-ase-0.4.1/thunder_ase.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 05:48:11.000000 thunder-ase-0.4.1/thunder_ase.egg-info/top_level.txt
```

### Comparing `thunder-ase-0.4/pyproject.toml` & `thunder-ase-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "thunder-ase"
-version = "0.4"
+version = "0.4.1"
 authors = [
   { name="PJ Ren", email="openrpj@gmail.com" },
 ]
 description = "ASE calculator interface for FIREBALL code"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `thunder-ase-0.4/thunder_ase/fireball.py` & `thunder-ase-0.4.1/thunder_ase/fireball.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,31 +82,33 @@
     kpoints_weight = [[k[0], k[1], k[2], len(v) / nkpt] for k, v in irreducible_dct.items()]
     return kpoints_weight
 
 
 options_params = {
     'nstepi': {'type': (int,), 'name': 'nstepi', 'default': 1},
     'nstepf': {'type': (int,), 'name': 'nstepf', 'default': 1},
-    'qstate': {'type': (int,), 'name': 'qstate', 'default': 0},  # Extra electron. +1 mean adding 1 electron.
+    'qstate': {'type': (int, float), 'name': 'qstate', 'default': 0},  # Extra electron. +1 mean adding 1 electron.
     'iquench': {'type': (int,), 'name': 'iquench', 'default': 0},
+    # optimization algorithm, 0: MD, -1: hard quench at KE achieve maximum, -3: power (force * velocity) quench,
+    # positive number N: quench every N step
     't_initial': {'type': (int, float), 'name': 'T_initial', 'default': 300.0},
     't_final': {'type': (int, float), 'name': 'T_final', 'default': 0.0},
     't_want': {'type': (int, float), 'name': 'T_want', 'default': 300.0},
     'taurelax': {'type': (int, float), 'name': 'taurelax', 'default': 5.0},
     'efermi_t': {'type': (int, float), 'name': 'efermi_T', 'default': 100.0},
     'dt': {'type': (int, float), 'name': 'dt', 'default': 0.25},  # fs
     'iensemble': {'type': (int,), 'name': 'iensemble', 'default': 0},
     'iconstraint_rcm': {'type': (int,), 'name': 'iconstraint_rcm', 'default': 1},  # shift molecule to COM or not
     'iconstraint_vcm': {'type': (int,), 'name': 'iconstraint_vcm', 'default': 1},  # whether keep COM fixed during md
     'iconstraint_l': {'type': (int,), 'name': 'iconstraint_L', 'default': 0},
     'iconstraint_ke': {'type': (int,), 'name': 'iconstraint_KE', 'default': 1},
     'ifix_neighbors': {'type': (int,), 'name': 'ifix_neighbors', 'default': 0},
     'ifix_charges': {'type': (int,), 'name': 'ifix_CHARGES', 'default': 1},
     'max_scf_iterations_set': {'type': (int,), 'name': 'max_scf_iterations_set', 'default': 50},
-    'scf_tolerance_set': {'type': (int, float), 'name': 'scf_tolerance_set', 'default': 0.00000001},
+    'scf_tolerance_set': {'type': (int, float), 'name': 'scf_tolerance_set', 'default': 0.000001},
     'beta_set': {'type': (int, float), 'name': 'beta_set', 'default': 0.08},  # mix factor
     'ecut_set': {'type': (int, float), 'name': 'Ecut_set', 'default': 200.0},  # control mesh grid number
 }
 
 output_params = {
     'iwriteout_me_sandh': {'type': (int,), 'name': 'iwriteout_ME_SandH', 'default': 0},
     'iwriteout_density': {'type': (int,), 'name': 'iwriteout_density', 'default': 0},
@@ -251,15 +253,16 @@
     def check_kwargs(self, kwargs):
         for key, v in kwargs.items():
             k = key.lower()
             if k not in fireball_params:
                 print("The option {} not supported!".format(k))
                 raise KeyError
             if type(v) not in fireball_params[k]['type']:
-                print("The type of {} should be {}".format(k, ' or '.join(fireball_params[k]['type'])))
+                print("The type of {} should be {}, but type {} is provided!".format(k, ' or '.join(
+                    [i.__name__ for i in fireball_params[k]['type']]), type(v).__name__))
                 raise TypeError
             if k in output_params:
                 self.output_params[k] = v
             elif k in options_params:
                 self.options_params[k] = v
             elif k in xsfoptions_params:
                 self.xsfoptions_params[k] = v
@@ -487,28 +490,34 @@
 
     def read_results(self):
         output = self.sname + ".json"
         result = jsonio.read_json(output)
         if 'charges' in result['fireball'][-1]:
             shell_charges = result['fireball'][-1]['charges']
             result['fireball'][-1]['shell_charges'] = shell_charges
+            del(result['fireball'][-1]['charges'])
+
         self.results = result['fireball'][-1]
 
     def get_charges(self, atoms=None):
         if self.results is None:
             try:
                 self.read_results()
             except AttributeError:
                 return None
-        shell_charges = self.results['fireball'][-1]['shell_charges']
+        else:
+            if 'charges' in self.results:
+                return self.results['charges']
+
+        shell_charges = self.results['shell_charges']
         sum_charges = [sum(isc) for isc in shell_charges]
         if atoms is None:
             atoms = self.atoms
         ref_charges = [sum(self.shell_info[s]['occupation']) for s in atoms.symbols]
-        charges = [ref-sc for sc, ref in zip(sum_charges, ref_charges)]
+        charges = [ref - sc for sc, ref in zip(sum_charges, ref_charges)]
         self.results['charges'] = charges
         return charges
 
     def get_forces(self, atoms=None):
         forces = self.get_property('forces', atoms)
         return np.asarray(forces)
 
@@ -623,15 +632,15 @@
         return self._shell_info
 
     def get_valence_charge(self, i):
         isymbol = self.atoms.symbols[i]
         shell_info = self.shell_info[isymbol]
         return sum(shell_info['occupation'])
 
-    def write_mwfn(self, kpoint=0):
+    def write_mwfn(self, kpoint=0, filename=None):
         mwfn_dict = MWFN_DEFAULT.copy()
         # Initialize default data format
         for k, v in mwfn_dict.items():
             if v is not None:
                 mwfn_dict[k] = MWFN_FORMAT[k].format(v)
 
         # atom information
@@ -653,15 +662,15 @@
                 'cellv3': (MWFN_FORMAT['cellv3'] * 3).format(*self.atoms.cell[2]),
             }
             mwfn_dict['cell_info'] = CELL_TEMPLATE.substitute(cell_info)
         else:
             mwfn_dict['cell_info'] = ''
 
         # electron for alpha and beta
-        tot_elec = sum([self.get_valence_charge(i) for i in range(len(self.atoms))])
+        tot_elec = sum([self.get_valence_charge(i) for i in range(len(self.atoms))]) - sum(self.get_charges())
         naelec = 0.5 * tot_elec
         nbelec = 0.5 * tot_elec
         mwfn_dict['naelec'] = MWFN_FORMAT['naelec'].format(naelec)
         mwfn_dict['nbelec'] = MWFN_FORMAT['nbelec'].format(nbelec)
         # total energy
         mwfn_dict['e_tot'] = MWFN_FORMAT['e_tot'].format(self.get_potential_energy() / Hartree)
         # Basis set info
@@ -709,15 +718,17 @@
         mwfn_dict['orbital_coeffs'] = '\n\n'.join(orbital_coeffs)
 
         self.mwfn_dict = mwfn_dict
         content = MWFN_TEMPLATE.substitute(mwfn_dict)
         # TODO: read orbital info, append to the content
 
         # write out
-        with open(self.sname + '.mwfn', 'w') as f:
+        if filename is None:
+            filename = self.sname + '.mwfn'
+        with open(filename, 'w') as f:
             f.write(content)
 
 
 class MultiFireball:
     name = 'multi_fireball'
 
     def __init__(self, atoms_list=None, calc=None, sname_list=None):
```

### Comparing `thunder-ase-0.4/thunder_ase/utils/basis_set.py` & `thunder-ase-0.4.1/thunder_ase/utils/basis_set.py`

 * *Files identical despite different names*

### Comparing `thunder-ase-0.4/thunder_ase/utils/mwfn.py` & `thunder-ase-0.4.1/thunder_ase/utils/mwfn.py`

 * *Files identical despite different names*

### Comparing `thunder-ase-0.4/thunder_ase/utils/shell_dict.py` & `thunder-ase-0.4.1/thunder_ase/utils/shell_dict.py`

 * *Files identical despite different names*

