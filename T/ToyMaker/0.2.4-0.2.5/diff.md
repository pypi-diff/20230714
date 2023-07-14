# Comparing `tmp/ToyMaker-0.2.4.tar.gz` & `tmp/ToyMaker-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ToyMaker-0.2.4.tar", last modified: Tue Feb 28 02:07:06 2023, max compression
+gzip compressed data, was "ToyMaker-0.2.5.tar", last modified: Fri Jul 14 05:21:05 2023, max compression
```

## Comparing `ToyMaker-0.2.4.tar` & `ToyMaker-0.2.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
-drwxrwxrwx   0 massive_wave  (1000) massive_wave  (1000)        0 2023-02-28 02:07:06.285042 ToyMaker-0.2.4/
--rwxrwxrwx   0 massive_wave  (1000) massive_wave  (1000)      901 2023-02-28 02:07:06.285042 ToyMaker-0.2.4/PKG-INFO
-drwxrwxrwx   0 massive_wave  (1000) massive_wave  (1000)        0 2023-02-28 02:07:06.285042 ToyMaker-0.2.4/ToyMaker/
--rwxrwxrwx   0 massive_wave  (1000) massive_wave  (1000)     7203 2023-02-28 01:48:47.156062 ToyMaker-0.2.4/ToyMaker/Assembler.py
--rwxrwxrwx   0 massive_wave  (1000) massive_wave  (1000)       39 2023-02-24 21:35:07.003590 ToyMaker-0.2.4/ToyMaker/__init__.py
--rwxrwxrwx   0 massive_wave  (1000) massive_wave  (1000)       39 2023-02-24 16:24:34.426661 ToyMaker-0.2.4/setup.cfg
--rwxrwxrwx   0 massive_wave  (1000) massive_wave  (1000)     1102 2023-02-28 02:05:37.574469 ToyMaker-0.2.4/setup.py
+drwxrwxrwx   0 massive_wave  (1000) massive_wave  (1000)        0 2023-07-14 05:21:05.125044 ToyMaker-0.2.5/
+-rwxrwxrwx   0 massive_wave  (1000) massive_wave  (1000)      901 2023-07-14 05:21:05.133042 ToyMaker-0.2.5/PKG-INFO
+drwxrwxrwx   0 massive_wave  (1000) massive_wave  (1000)        0 2023-07-14 05:21:05.125044 ToyMaker-0.2.5/ToyMaker/
+-rwxrwxrwx   0 massive_wave  (1000) massive_wave  (1000)     7216 2023-07-14 04:16:54.101078 ToyMaker-0.2.5/ToyMaker/Assembler.py
+-rwxrwxrwx   0 massive_wave  (1000) massive_wave  (1000)       39 2023-02-24 21:35:07.003590 ToyMaker-0.2.5/ToyMaker/__init__.py
+-rwxrwxrwx   0 massive_wave  (1000) massive_wave  (1000)       39 2023-02-24 16:24:34.426661 ToyMaker-0.2.5/setup.cfg
+-rwxrwxrwx   0 massive_wave  (1000) massive_wave  (1000)     1102 2023-07-14 05:20:34.862335 ToyMaker-0.2.5/setup.py
```

### Comparing `ToyMaker-0.2.4/PKG-INFO` & `ToyMaker-0.2.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: ToyMaker
-Version: 0.2.4
+Version: 0.2.5
 Summary: This library is designed to facilitate research of stochasticity effects in genetic circuits
 Home-page: https://github.com/SergioPachonDotor
 Author: Sergio Andrés Pachón Dotor
 Author-email: sap9827@gmail.com
 License: MIT
-Download-URL: https://github.com/SergioPachonDotor/ToyMaker/archive/refs/tags/v_0.2.4.tar.gz
+Download-URL: https://github.com/SergioPachonDotor/ToyMaker/archive/refs/tags/v_0.2.5.tar.gz
 Description: UNKNOWN
 Keywords: Stochastic process,Genetic circuits,Simulation,Synthetic Biology,Systems Biology
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ToyMaker-0.2.4/ToyMaker/Assembler.py` & `ToyMaker-0.2.5/ToyMaker/Assembler.py`

 * *Files 15% similar despite different names*

```diff
@@ -79,25 +79,25 @@
                          '        propensities = np.zeros({reactions_keys_values}, dtype=np.float64)\n', 
                          '        tarr = np.arange(0, tmax,   sampling_time, dtype=np.float64)\n', 
                          '        # Simulation Space\n', '        sim  = np.zeros((len(tarr), len(species)), dtype=np.float64)\n', 
                          '        sim[0] = species\n', '        for indx_dt in range(1, len(tarr)):\n', 
                          '            species = sim[indx_dt - 1]\n', '            while species[0] < tarr[indx_dt]:\n', 
                          '                # Species\n', '            {species_to_write}\n', '                # Propensities\n', 
                          '            {propensities_to_write}\n', 
-                         '                τarr = np.zeros(len(propensities), dtype=np.float64)\n', 
+                         '                tauarr = np.zeros(len(propensities), dtype=np.float64)\n', 
                          '                # Calculate tau times\n', 
-                         '                for indx_τ in range(len(propensities)):\n', 
-                         '                    if propensities[indx_τ] > 0 :\n', 
-                         '                        τarr[indx_τ] = -(1/propensities[indx_τ]) * np.log(np.random.rand())\n', 
+                         '                for indx_tau in range(len(propensities)):\n', 
+                         '                    if propensities[indx_tau] > 0 :\n', 
+                         '                        tauarr[indx_tau] = -(1/propensities[indx_tau]) * np.log(np.random.rand())\n', 
                          '                    else:\n', 
-                         '                        τarr[indx_τ] = np.inf\n', 
-                         '                τ = np.min(τarr)\n', 
-                         '                q = np.argmin(τarr)\n', 
-                         '                species = species + reaction_type[q] if τ != np.inf else species\n', 
-                         '                species[0] = species[0] + τ\n', 
+                         '                        tauarr[indx_tau] = np.inf\n', 
+                         '                tau = np.min(tauarr)\n', 
+                         '                q = np.argmin(tauarr)\n', 
+                         '                species = species + reaction_type[q] if tau != np.inf else species\n', 
+                         '                species[0] = species[0] + tau\n', 
                          '            sim[indx_dt] = species\n', 
                          '        cells_arr.append(sim)\n', 
                          '    return cells_arr']
         
         gillespie_str = ''.join(gillespie_str).format(**replacements)   
         return gillespie_str
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ToyMaker-0.2.4/setup.py` & `ToyMaker-0.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'ToyMaker',         
   packages = ['ToyMaker'],
-  version = '0.2.4',  
+  version = '0.2.5',  
   license='MIT',    
   description = 'This library is designed to facilitate research of stochasticity effects in genetic circuits',
   author = 'Sergio Andrés Pachón Dotor',
   author_email = 'sap9827@gmail.com',
   url = 'https://github.com/SergioPachonDotor',
-  download_url = 'https://github.com/SergioPachonDotor/ToyMaker/archive/refs/tags/v_0.2.4.tar.gz',
+  download_url = 'https://github.com/SergioPachonDotor/ToyMaker/archive/refs/tags/v_0.2.5.tar.gz',
   keywords = ['Stochastic process', 'Genetic circuits', 'Simulation', 'Synthetic Biology', 'Systems Biology'],
   install_requires=[     
           'numpy',
           'numba',
       ],
   classifiers=[
     'Development Status :: 4 - Beta',      # "3 - Alpha", "4 - Beta" or "5 - Production/Stable"
```

