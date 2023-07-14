# Comparing `tmp/reflected_light_sim-0.1.tar.gz` & `tmp/reflected_light_sim-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflected_light_sim-0.1.tar", last modified: Thu Jul 13 23:54:05 2023, max compression
+gzip compressed data, was "reflected_light_sim-0.1.1.tar", last modified: Fri Jul 14 17:27:57 2023, max compression
```

## Comparing `reflected_light_sim-0.1.tar` & `reflected_light_sim-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 huihaoz    (501) staff       (20)        0 2023-07-13 23:54:05.863751 reflected_light_sim-0.1/
--rw-r--r--   0 huihaoz    (501) staff       (20)     1072 2023-07-10 23:10:27.000000 reflected_light_sim-0.1/LICENSE
--rw-r--r--   0 huihaoz    (501) staff       (20)      547 2023-07-13 23:54:05.863589 reflected_light_sim-0.1/PKG-INFO
--rw-r--r--   0 huihaoz    (501) staff       (20)      244 2023-07-13 23:49:09.000000 reflected_light_sim-0.1/README.md
-drwxr-xr-x   0 huihaoz    (501) staff       (20)        0 2023-07-13 23:54:05.862607 reflected_light_sim-0.1/reflected_light_sim/
--rw-r--r--   0 huihaoz    (501) staff       (20)       19 2023-07-13 23:49:09.000000 reflected_light_sim-0.1/reflected_light_sim/__init__.py
--rw-r--r--   0 huihaoz    (501) staff       (20)     2719 2023-07-13 23:49:09.000000 reflected_light_sim-0.1/reflected_light_sim/reflectance.py
-drwxr-xr-x   0 huihaoz    (501) staff       (20)        0 2023-07-13 23:54:05.863402 reflected_light_sim-0.1/reflected_light_sim.egg-info/
--rw-r--r--   0 huihaoz    (501) staff       (20)      547 2023-07-13 23:54:05.000000 reflected_light_sim-0.1/reflected_light_sim.egg-info/PKG-INFO
--rw-r--r--   0 huihaoz    (501) staff       (20)      307 2023-07-13 23:54:05.000000 reflected_light_sim-0.1/reflected_light_sim.egg-info/SOURCES.txt
--rw-r--r--   0 huihaoz    (501) staff       (20)        1 2023-07-13 23:54:05.000000 reflected_light_sim-0.1/reflected_light_sim.egg-info/dependency_links.txt
--rw-r--r--   0 huihaoz    (501) staff       (20)       14 2023-07-13 23:54:05.000000 reflected_light_sim-0.1/reflected_light_sim.egg-info/requires.txt
--rw-r--r--   0 huihaoz    (501) staff       (20)       20 2023-07-13 23:54:05.000000 reflected_light_sim-0.1/reflected_light_sim.egg-info/top_level.txt
--rw-r--r--   0 huihaoz    (501) staff       (20)       38 2023-07-13 23:54:05.863809 reflected_light_sim-0.1/setup.cfg
--rw-r--r--   0 huihaoz    (501) staff       (20)     1432 2023-07-13 23:49:09.000000 reflected_light_sim-0.1/setup.py
+drwxrwxrwx   0 jliberman  (1000) jliberman  (1000)        0 2023-07-14 17:27:57.193206 reflected_light_sim-0.1.1/
+-rwxrwxrwx   0 jliberman  (1000) jliberman  (1000)     1093 2023-07-10 21:35:36.000000 reflected_light_sim-0.1.1/LICENSE
+-rwxrwxrwx   0 jliberman  (1000) jliberman  (1000)      549 2023-07-14 17:27:57.187201 reflected_light_sim-0.1.1/PKG-INFO
+-rwxrwxrwx   0 jliberman  (1000) jliberman  (1000)      378 2023-07-14 17:20:16.000000 reflected_light_sim-0.1.1/README.md
+drwxrwxrwx   0 jliberman  (1000) jliberman  (1000)        0 2023-07-14 17:27:56.912145 reflected_light_sim-0.1.1/reflected_light_sim/
+-rwxrwxrwx   0 jliberman  (1000) jliberman  (1000)       21 2023-07-14 17:25:46.000000 reflected_light_sim-0.1.1/reflected_light_sim/__init__.py
+-rwxrwxrwx   0 jliberman  (1000) jliberman  (1000)     3868 2023-07-14 17:20:17.000000 reflected_light_sim-0.1.1/reflected_light_sim/reflectance.py
+drwxrwxrwx   0 jliberman  (1000) jliberman  (1000)        0 2023-07-14 17:27:57.144199 reflected_light_sim-0.1.1/reflected_light_sim.egg-info/
+-rwxrwxrwx   0 jliberman  (1000) jliberman  (1000)      549 2023-07-14 17:27:56.000000 reflected_light_sim-0.1.1/reflected_light_sim.egg-info/PKG-INFO
+-rwxrwxrwx   0 jliberman  (1000) jliberman  (1000)      307 2023-07-14 17:27:56.000000 reflected_light_sim-0.1.1/reflected_light_sim.egg-info/SOURCES.txt
+-rwxrwxrwx   0 jliberman  (1000) jliberman  (1000)        1 2023-07-14 17:27:56.000000 reflected_light_sim-0.1.1/reflected_light_sim.egg-info/dependency_links.txt
+-rwxrwxrwx   0 jliberman  (1000) jliberman  (1000)       14 2023-07-14 17:27:56.000000 reflected_light_sim-0.1.1/reflected_light_sim.egg-info/requires.txt
+-rwxrwxrwx   0 jliberman  (1000) jliberman  (1000)       20 2023-07-14 17:27:56.000000 reflected_light_sim-0.1.1/reflected_light_sim.egg-info/top_level.txt
+-rwxrwxrwx   0 jliberman  (1000) jliberman  (1000)       38 2023-07-14 17:27:57.196200 reflected_light_sim-0.1.1/setup.cfg
+-rwxrwxrwx   0 jliberman  (1000) jliberman  (1000)     1471 2023-07-14 17:19:47.000000 reflected_light_sim-0.1.1/setup.py
```

### Comparing `reflected_light_sim-0.1/LICENSE` & `reflected_light_sim-0.1.1/LICENSE`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Joshua Liberman
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Joshua Liberman
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `reflected_light_sim-0.1/PKG-INFO` & `reflected_light_sim-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflected_light_sim
-Version: 0.1
+Version: 0.1.1
 Summary: reflected-light-sim: a simulator for reflected light of planet
 Home-page: https://github.com/jlibermann/reflected-light-sim/tree/main
 Author: Josh+Huihao
 License: MIT
 Keywords: Reflectance Astronomy
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
```

### Comparing `reflected_light_sim-0.1/reflected_light_sim/reflectance.py` & `reflected_light_sim-0.1.1/reflected_light_sim/reflectance.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,85 +1,109 @@
-import astropy.io.fits as fits
-import glob
-import os
-import numpy as np
-import astropy.units as u
-import astropy.constants as cons
-
-class Spectrum():
-    '''
-    A class for spectra manipulation (based on PSI Sim's spectrum.py class).
-
-    The main properties will be: 
-    wvs    - sampled wavelengths (np.array of floats, in microns)
-    spectrum    - current flux values of the spectrum (np.array of floats, [photons/s/cm^2/A])
-    R   - spectral resolution (float)
-
-    The main functions will be: 
-    load_phoenix_model      - load a PHOENIX model 
-    calculate_reflected_light  -calculate the reflected light from a planet
-
-
-    '''
-
-    def __init__(self, wvs, spectrum, R):
-
-        self.wvs = wvs
-        self.spectrum = spectrum
-        self.R = R
-
-        return
-    
-    # def load_phoenix_model(self, )
-        
-
-    def load_phoenix_model(lambda_start, lambda_end,steff,path=None):
-        '''
-        Read in a phoenix spectrum
-        '''
-       
-        # Prompt the user to specify a path if none is given
-        if path is None:
-            path = input('Specify a path to your PHOENIX model (directory containing wavels + fluxes): \n')
-        teff =str(int(steff)).zfill(5)
-        path_use = path + 'lte%s-4.50-0.0.PHOENIX-ACES-AGSS-COND-2011-HiRes.fits'%(teff)
-        f = fits.open(path_use)
-        spec = f[0].data / (1e8) # ergs/s/cm2/cm to ergs/s/cm2/Angstrom for conversion
-        f.close()
-        
-        f = fits.open(path + 'WAVE_PHOENIX-ACES-AGSS-COND-2011.fits')
-        lam = f[0].data # angstroms
-        f.close()
-        
-        # Convert
-        conversion_factor = 5.03*10**7 * lam #lam in angstrom here
-        spec *= conversion_factor # phot/cm2/s/angstrom
-        
-        # Take subarray requested
-        isub = np.where( (lam > lambda_start*10.0) & (lam < lambda_end*10.0))[0]
-
-        # Convert 
-        return lam[isub]/10.0,spec[isub] * 10 * 100**2 #nm, phot/m2/s/nm
-
-    def cal_refflux_pl(d_star_earth,host_spec,r_star,r_planet,a_planet, albedo,wvl):
-        '''
-        Calculation about reflected flux from planet
-        '''
-        wvl *= u.nm
-        ph_energy = ((cons.h * cons.c / (wvl) ) /u.ph).to(u.J / u.ph)
-
-        host_spec_J = (host_spec* u.ph / (u.m**2 * u.s * u.nm) * ph_energy).to(u.J / (u.m**2 * u.s * u.nm))
-
-        lum_star = host_spec_J * 4 * np.pi * r_star**2
-
-        # flux of star on planet
-        flux_sp = lum_star / (4 * np.pi * a_planet**2)
-
-        lum_planet = flux_sp * r_planet**2 * np.pi * albedo
-
-        flux_planet = lum_planet / (4 * np.pi * d_star_earth**2)
-
-        flux_planet_ph = (flux_planet / ph_energy).to(u.ph / (u.m**2 * u.s * u.nm))
-
-        # Convert 
-        return flux_planet_ph #nm, phot/m2/s/nm
+import astropy.io.fits as fits
+import glob
+import os
+import numpy as np
+import astropy.units as u
+import astropy.constants as cons
+
+class Spectrum():
+    '''
+    A class for spectra manipulation (based on PSI Sim's spectrum.py class).
+
+    The main properties will be: 
+    wvs    - sampled wavelengths (np.array of floats, in microns)
+    spectrum    - current flux values of the spectrum (np.array of floats, [photons/s/cm^2/A])
+    R   - spectral resolution (float)
+
+    The main functions will be: 
+    load_phoenix_model      - load a PHOENIX model 
+    calculate_reflected_light  -calculate the reflected light from a planet
+
+
+    '''
+
+    def __init__(self, wvs, spectrum, R):
+
+        self.wvs = wvs
+        self.spectrum = spectrum
+        self.R = R
+
+        return
+    
+    # def load_phoenix_model(self, )
+        
+
+    def load_phoenix_model(lambda_start, lambda_end,steff,path=None):
+        """Load a PHOENIX Stellar Model
+
+        Loads a stellar PHOENIX model given a starting + ending wavelength, an effective temperature, and a path to the model.
+
+        Args:
+            lambda_start (int): Starting wavelength value
+            lambda_end (int): Ending wavelength value
+            steff (int): Stellar effective temperature
+            path (str, optional): Path to the PHOENIX model directory. Defaults to None.
+
+        Returns:
+            lam (array) : The wavelength array from the PHOENIX model.
+            spec (array): The flux array from the PHOENIX model.
+
+        """
+       
+        # Prompt the user to specify a path if none is given
+        if path is None:
+            path = input('Specify a path to your PHOENIX model (directory containing wavels + fluxes): \n')
+        teff =str(int(steff)).zfill(5)
+        path_use = path + 'lte%s-4.50-0.0.PHOENIX-ACES-AGSS-COND-2011-HiRes.fits'%(teff)
+        f = fits.open(path_use)
+        spec = f[0].data / (1e8) # ergs/s/cm2/cm to ergs/s/cm2/Angstrom for conversion
+        f.close()
+        
+        f = fits.open(path + 'WAVE_PHOENIX-ACES-AGSS-COND-2011.fits')
+        lam = f[0].data # angstroms
+        f.close()
+        
+        # Convert
+        conversion_factor = 5.03*10**7 * lam #lam in angstrom here
+        spec *= conversion_factor # phot/cm2/s/angstrom
+        
+        # Take subarray requested
+        isub = np.where( (lam > lambda_start*10.0) & (lam < lambda_end*10.0))[0]
+
+        # Convert 
+        return lam[isub]/10.0,spec[isub] * 10 * 100**2 #nm, phot/m2/s/nm
+
+    def cal_refflux_pl(d_star_earth,host_spec,r_star,r_planet,a_planet, albedo,wvl):
+        """Calculate the reflected flux from a planet.
+
+        Args:
+            d_star_earth (int): Star-Earth distance (parsecs)
+            host_spec (array): Flux array from host star model.
+            r_star (int): Stellar radius ($R_{\odot}$)
+            r_planet (int): Planet radius ($R_{Jup})
+            a_planet (int): Planet semi-major axis (AU)
+            albedo (float): Planet albedo.
+            wvl (array): Wavelength array from host star model.
+
+        Returns:
+            flux_planet_ph (array): An array of reflected planet fluxes.
+
+        """
+        wvl *= u.nm
+        ph_energy = ((cons.h * cons.c / (wvl) ) /u.ph).to(u.J / u.ph)
+
+        host_spec_J = (host_spec* u.ph / (u.m**2 * u.s * u.nm) * ph_energy).to(u.J / (u.m**2 * u.s * u.nm))
+
+        lum_star = host_spec_J * 4 * np.pi * r_star**2
+
+        # flux of star on planet
+        flux_sp = lum_star / (4 * np.pi * a_planet**2)
+
+        lum_planet = flux_sp * r_planet**2 * np.pi * albedo
+
+        flux_planet = lum_planet / (4 * np.pi * d_star_earth**2)
+
+        flux_planet_ph = (flux_planet / ph_energy).to(u.ph / (u.m**2 * u.s * u.nm))
+
+        # Convert 
+        return flux_planet_ph #nm, phot/m2/s/nm
```

### Comparing `reflected_light_sim-0.1/reflected_light_sim.egg-info/PKG-INFO` & `reflected_light_sim-0.1.1/reflected_light_sim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflected-light-sim
-Version: 0.1
+Version: 0.1.1
 Summary: reflected-light-sim: a simulator for reflected light of planet
 Home-page: https://github.com/jlibermann/reflected-light-sim/tree/main
 Author: Josh+Huihao
 License: MIT
 Keywords: Reflectance Astronomy
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
```

### Comparing `reflected_light_sim-0.1/setup.py` & `reflected_light_sim-0.1.1/setup.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-from setuptools import setup, find_packages
-import re
-
-
-# auto-updating version code stolen from Orbitize which was stolen from RadVel
-def get_property(prop, project):
-    result = re.search(r'{}\s*=\s*[\'"]([^\'"]*)[\'"]'.format(prop),
-                       open(project + '/__init__.py').read())
-    return result.group(1)
-
-def get_requires():
-    reqs = []
-    for line in open('requirements.txt', 'r').readlines():
-        reqs.append(line)
-    return reqs
-
-setup(
-    name='reflected_light_sim',
-    version=get_property('__version__', 'reflected_light_sim'),
-    description='reflected-light-sim: a simulator for reflected light of planet',
-    url='https://github.com/jlibermann/reflected-light-sim/tree/main',
-    author='Josh+Huihao',
-    license='MIT',
-    packages=find_packages(),
-    classifiers=[
-        # Indicate who your project is intended for
-        'Intended Audience :: Science/Research',
-        'Topic :: Scientific/Engineering :: Astronomy',
-
-        # Pick your license as you wish (should match "license" above)
-        'License :: OSI Approved :: MIT License',
-
-        # Specify the Python versions you support here. In particular, ensure
-        # that you indicate whether you support Python 2, Python 3 or both.
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3',
-        ],
-    keywords='Reflectance Astronomy',
-    install_requires=get_requires()
+from setuptools import setup, find_packages
+import re
+
+
+# auto-updating version code stolen from Orbitize which was stolen from RadVel
+def get_property(prop, project):
+    result = re.search(r'{}\s*=\s*[\'"]([^\'"]*)[\'"]'.format(prop),
+                       open(project + '/__init__.py').read())
+    return result.group(1)
+
+def get_requires():
+    reqs = []
+    for line in open('requirements.txt', 'r').readlines():
+        reqs.append(line)
+    return reqs
+
+setup(
+    name='reflected_light_sim',
+    version=get_property('__version__', 'reflected_light_sim'),
+    description='reflected-light-sim: a simulator for reflected light of planet',
+    url='https://github.com/jlibermann/reflected-light-sim/tree/main',
+    author='Josh+Huihao',
+    license='MIT',
+    packages=find_packages(),
+    classifiers=[
+        # Indicate who your project is intended for
+        'Intended Audience :: Science/Research',
+        'Topic :: Scientific/Engineering :: Astronomy',
+
+        # Pick your license as you wish (should match "license" above)
+        'License :: OSI Approved :: MIT License',
+
+        # Specify the Python versions you support here. In particular, ensure
+        # that you indicate whether you support Python 2, Python 3 or both.
+        'Programming Language :: Python :: 2.7',
+        'Programming Language :: Python :: 3',
+        ],
+    keywords='Reflectance Astronomy',
+    install_requires=get_requires()
     )
```

