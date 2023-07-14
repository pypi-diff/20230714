# Comparing `tmp/dLuxToliman-0.1.3.tar.gz` & `tmp/dLuxToliman-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dLuxToliman-0.1.3.tar", last modified: Thu Jul 13 04:50:18 2023, max compression
+gzip compressed data, was "dLuxToliman-0.2.0.tar", last modified: Fri Jul 14 07:12:55 2023, max compression
```

## Comparing `dLuxToliman-0.1.3.tar` & `dLuxToliman-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 mcha5804   (501) staff       (20)        0 2023-07-13 04:50:18.024553 dLuxToliman-0.1.3/
--rw-r--r--   0 mcha5804   (501) staff       (20)       93 2023-05-29 04:35:46.000000 dLuxToliman-0.1.3/.gitignore
--rw-r--r--   0 mcha5804   (501) staff       (20)     1498 2023-05-29 03:55:35.000000 dLuxToliman-0.1.3/LICENSE
--rw-r--r--   0 mcha5804   (501) staff       (20)     3232 2023-07-13 04:50:18.024396 dLuxToliman-0.1.3/PKG-INFO
--rw-r--r--   0 mcha5804   (501) staff       (20)     2742 2023-07-13 04:26:03.000000 dLuxToliman-0.1.3/README.md
-drwxr-xr-x   0 mcha5804   (501) staff       (20)        0 2023-07-13 04:50:18.011849 dLuxToliman-0.1.3/assets/
--rw-r--r--   0 mcha5804   (501) staff       (20)    20565 2023-05-29 23:40:33.000000 dLuxToliman-0.1.3/assets/basic_toliman_psf.jpg
-drwxr-xr-x   0 mcha5804   (501) staff       (20)        0 2023-07-13 04:50:18.023488 dLuxToliman-0.1.3/dLuxToliman/
--rw-r--r--   0 mcha5804   (501) staff       (20)      515 2023-07-13 04:49:41.000000 dLuxToliman-0.1.3/dLuxToliman/__init__.py
--rw-r--r--   0 mcha5804   (501) staff       (20) 16777344 2023-05-29 04:35:46.000000 dLuxToliman-0.1.3/dLuxToliman/diffractive_pupil.npy
--rw-r--r--   0 mcha5804   (501) staff       (20)     2598 2023-07-13 04:26:03.000000 dLuxToliman-0.1.3/dLuxToliman/gradient_energy.py
--rw-r--r--   0 mcha5804   (501) staff       (20)     1044 2023-07-13 04:26:03.000000 dLuxToliman-0.1.3/dLuxToliman/instruments.py
--rw-r--r--   0 mcha5804   (501) staff       (20)     6751 2023-07-13 04:26:03.000000 dLuxToliman-0.1.3/dLuxToliman/optical_layers.py
--rw-r--r--   0 mcha5804   (501) staff       (20)     8198 2023-07-13 04:26:03.000000 dLuxToliman-0.1.3/dLuxToliman/optics.py
--rw-r--r--   0 mcha5804   (501) staff       (20)     9556 2023-07-13 04:42:31.000000 dLuxToliman-0.1.3/dLuxToliman/sources.py
-drwxr-xr-x   0 mcha5804   (501) staff       (20)        0 2023-07-13 04:50:18.024176 dLuxToliman-0.1.3/dLuxToliman.egg-info/
--rw-r--r--   0 mcha5804   (501) staff       (20)     3232 2023-07-13 04:50:17.000000 dLuxToliman-0.1.3/dLuxToliman.egg-info/PKG-INFO
--rw-r--r--   0 mcha5804   (501) staff       (20)      463 2023-07-13 04:50:17.000000 dLuxToliman-0.1.3/dLuxToliman.egg-info/SOURCES.txt
--rw-r--r--   0 mcha5804   (501) staff       (20)        1 2023-07-13 04:50:17.000000 dLuxToliman-0.1.3/dLuxToliman.egg-info/dependency_links.txt
--rw-r--r--   0 mcha5804   (501) staff       (20)       13 2023-07-13 04:50:17.000000 dLuxToliman-0.1.3/dLuxToliman.egg-info/requires.txt
--rw-r--r--   0 mcha5804   (501) staff       (20)       12 2023-07-13 04:50:17.000000 dLuxToliman-0.1.3/dLuxToliman.egg-info/top_level.txt
--rw-r--r--   0 mcha5804   (501) staff       (20)      361 2023-07-13 04:49:41.000000 dLuxToliman-0.1.3/pyproject.toml
--rw-r--r--   0 mcha5804   (501) staff       (20)       13 2023-06-16 01:08:49.000000 dLuxToliman-0.1.3/requirements.txt
--rw-r--r--   0 mcha5804   (501) staff       (20)       38 2023-07-13 04:50:18.024604 dLuxToliman-0.1.3/setup.cfg
--rw-r--r--   0 mcha5804   (501) staff       (20)     2603 2023-06-06 00:49:10.000000 dLuxToliman-0.1.3/setup.py
+drwxr-xr-x   0 mcha5804   (501) staff       (20)        0 2023-07-14 07:12:55.179903 dLuxToliman-0.2.0/
+-rw-r--r--   0 mcha5804   (501) staff       (20)       93 2023-05-29 04:35:46.000000 dLuxToliman-0.2.0/.gitignore
+-rw-r--r--   0 mcha5804   (501) staff       (20)     1498 2023-05-29 03:55:35.000000 dLuxToliman-0.2.0/LICENSE
+-rw-r--r--   0 mcha5804   (501) staff       (20)     3232 2023-07-14 07:12:55.179748 dLuxToliman-0.2.0/PKG-INFO
+-rw-r--r--   0 mcha5804   (501) staff       (20)     2742 2023-07-13 04:26:03.000000 dLuxToliman-0.2.0/README.md
+drwxr-xr-x   0 mcha5804   (501) staff       (20)        0 2023-07-14 07:12:55.161742 dLuxToliman-0.2.0/assets/
+-rw-r--r--   0 mcha5804   (501) staff       (20)    20565 2023-05-29 23:40:33.000000 dLuxToliman-0.2.0/assets/basic_toliman_psf.jpg
+drwxr-xr-x   0 mcha5804   (501) staff       (20)        0 2023-07-14 07:12:55.178782 dLuxToliman-0.2.0/dLuxToliman/
+-rw-r--r--   0 mcha5804   (501) staff       (20)      515 2023-07-14 07:09:55.000000 dLuxToliman-0.2.0/dLuxToliman/__init__.py
+-rw-r--r--   0 mcha5804   (501) staff       (20) 16777344 2023-05-29 04:35:46.000000 dLuxToliman-0.2.0/dLuxToliman/diffractive_pupil.npy
+-rw-r--r--   0 mcha5804   (501) staff       (20)     2598 2023-07-13 04:26:03.000000 dLuxToliman-0.2.0/dLuxToliman/gradient_energy.py
+-rw-r--r--   0 mcha5804   (501) staff       (20)     3830 2023-07-14 07:08:40.000000 dLuxToliman-0.2.0/dLuxToliman/instruments.py
+-rw-r--r--   0 mcha5804   (501) staff       (20)     6987 2023-07-14 07:08:40.000000 dLuxToliman-0.2.0/dLuxToliman/optical_layers.py
+-rw-r--r--   0 mcha5804   (501) staff       (20)    12488 2023-07-14 07:08:40.000000 dLuxToliman-0.2.0/dLuxToliman/optics.py
+-rw-r--r--   0 mcha5804   (501) staff       (20)     9855 2023-07-14 07:08:40.000000 dLuxToliman-0.2.0/dLuxToliman/sources.py
+drwxr-xr-x   0 mcha5804   (501) staff       (20)        0 2023-07-14 07:12:55.179560 dLuxToliman-0.2.0/dLuxToliman.egg-info/
+-rw-r--r--   0 mcha5804   (501) staff       (20)     3232 2023-07-14 07:12:55.000000 dLuxToliman-0.2.0/dLuxToliman.egg-info/PKG-INFO
+-rw-r--r--   0 mcha5804   (501) staff       (20)      463 2023-07-14 07:12:55.000000 dLuxToliman-0.2.0/dLuxToliman.egg-info/SOURCES.txt
+-rw-r--r--   0 mcha5804   (501) staff       (20)        1 2023-07-14 07:12:55.000000 dLuxToliman-0.2.0/dLuxToliman.egg-info/dependency_links.txt
+-rw-r--r--   0 mcha5804   (501) staff       (20)       13 2023-07-14 07:12:55.000000 dLuxToliman-0.2.0/dLuxToliman.egg-info/requires.txt
+-rw-r--r--   0 mcha5804   (501) staff       (20)       12 2023-07-14 07:12:55.000000 dLuxToliman-0.2.0/dLuxToliman.egg-info/top_level.txt
+-rw-r--r--   0 mcha5804   (501) staff       (20)      361 2023-07-14 07:09:55.000000 dLuxToliman-0.2.0/pyproject.toml
+-rw-r--r--   0 mcha5804   (501) staff       (20)       13 2023-06-16 01:08:49.000000 dLuxToliman-0.2.0/requirements.txt
+-rw-r--r--   0 mcha5804   (501) staff       (20)       38 2023-07-14 07:12:55.179946 dLuxToliman-0.2.0/setup.cfg
+-rw-r--r--   0 mcha5804   (501) staff       (20)     2603 2023-06-06 00:49:10.000000 dLuxToliman-0.2.0/setup.py
```

### Comparing `dLuxToliman-0.1.3/LICENSE` & `dLuxToliman-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dLuxToliman-0.1.3/PKG-INFO` & `dLuxToliman-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dLuxToliman
-Version: 0.1.3
+Version: 0.2.0
 Summary: A repo to hold the canonical dLux Toliman models.
 Home-page: https://github.com/maxecharles/dLuxToliman
 Author: Max Charles
 Author-email: max.charles@sydney.edu.au
 Project-URL: Bug Tracker, https://github.com/maxecharles/dLuxToliman/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `dLuxToliman-0.1.3/README.md` & `dLuxToliman-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dLuxToliman-0.1.3/assets/basic_toliman_psf.jpg` & `dLuxToliman-0.2.0/assets/basic_toliman_psf.jpg`

 * *Files identical despite different names*

### Comparing `dLuxToliman-0.1.3/dLuxToliman/__init__.py` & `dLuxToliman-0.2.0/dLuxToliman/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 name = "dLuxToliman"
-__version__ = "0.1.3"
+__version__ = "0.2.0"
 
 # Import as modules
 from . import optics
 from . import optical_layers
 from . import gradient_energy
 from . import instruments
 from . import sources
```

### Comparing `dLuxToliman-0.1.3/dLuxToliman/diffractive_pupil.npy` & `dLuxToliman-0.2.0/dLuxToliman/diffractive_pupil.npy`

 * *Files identical despite different names*

### Comparing `dLuxToliman-0.1.3/dLuxToliman/gradient_energy.py` & `dLuxToliman-0.2.0/dLuxToliman/gradient_energy.py`

 * *Files identical despite different names*

### Comparing `dLuxToliman-0.1.3/dLuxToliman/optical_layers.py` & `dLuxToliman-0.2.0/dLuxToliman/optical_layers.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,29 +4,32 @@
 import dLux
 
 __all__ = ["ApplyBasisCLIMB"]
 
 OpticalLayer = lambda: dLux.optical_layers.OpticalLayer
 BasisLayer = lambda: dLux.optical_layers.BasisLayer
 
-# TODO write this class
+# TODO write this class: make it take arbitrary oversamples (its hardcoded to 3x),
+#  and take arbitrary output size (its hardcoded to 256)
 class ApplyBasisCLIMB(BasisLayer()):
     """
     Adds an array of binary phase values to the input wavefront from a set of
     continuous basis vectors. This uses the CLIMB algorithm in order to
     generate the binary values in a continuous manner as described in the
     paper Wong et al. 2021. The basis vectors are taken as an Optical Path
     Difference (OPD), and applied to the phase of the wavefront. The ideal
     wavelength parameter described the wavelength that will have a perfect
     anti-phase relationship given by the Optical Path Difference.
 
     TODO: Many of the methods in the class still need doccumentation.
     TODO: This currently only outputs 256 pixel arrays and uses a 3x oversample,
     therefore requiring a 768 pixel basis array.
 
+    "This class is the crazy lady we keep in the attic, but turns out her name is actually Ben." - L. Desdoigts, 2023.
+
     Attributes
     ----------
     basis: Array
         Arrays holding the continous pre-calculated basis vectors.
     coefficients: Array
         The Array of coefficients to be applied to each basis vector.
     ideal_wavelength : Array
```

### Comparing `dLuxToliman-0.1.3/dLuxToliman/sources.py` & `dLuxToliman-0.2.0/dLuxToliman/sources.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,79 +1,84 @@
 from __future__ import annotations
 from jax import Array, vmap
 import jax.numpy as np
-import matplotlib.pyplot as plt
 import dLux
 import dLux.utils as dlu
 
-# TODO check if this lambda was necessary
 Source = lambda: dLux.sources.BaseSource
 Optics = lambda: dLux.core.BaseOptics
 
 __all__ = ["AlphaCen"]  # , "MixedAlphaCen"]
 
 
 class AlphaCen(dLux.sources.BaseSource):
     """
     A parametrised model of the Alpha Centauri binary pair.
 
-    Parameters
-    ----------
-    n_wavels : int
-        The number of wavelengths to model.
-    separation : float
-        The binary separation of the two stars in arcseconds.
-    position_angle : float
-        The position angle of the binary pair in degrees.
-    x_position : float
-        The horizontal offset of the image in arcseconds.
-    y_position : float
-        The vertical offset of the image in arcseconds.
-    log_flux : float
-        The log10 of the total number of photons in the image.
-    contrast : float
-        The flux ratio of Alpha Cen A / Alpha Cen B.
-    bandpass : tuple
-        The wavelength range of the image in nanometers, with syntax (min, max).
-    weights : Array
-    TODO im not actually sure
-
-    Attributes
+    Properties
     ----------
+    xy_positions : Array
+        The x and y positions of the two stars in radians.
+    raw_fluxes : Array
+        The raw fluxes of the two stars in photons.
+    norm_weights : Array
+        The normalised spectral weights of each modelled wavelength.
 
     Methods
     -------
-    TODO CONTINUE
+    normalise()
+        Normalises the source flux to 1.
+    model()
+        Models the PSF by propagating the AlphaCen source through the given optics.
     """
+
     separation: float
     position_angle: float
     x_position: float
     y_position: float
     log_flux: float
     contrast: float
     bandpass: tuple
     weights: Array
     wavelengths: Array
 
-    # TODO : update default values
-    # TODO: Add bandpass as a parameter?
     def __init__(self,
                  n_wavels=3,
                  separation=10.,  # arcseconds
                  position_angle=90,  # degrees
                  x_position=0.,  # arcseconds
                  y_position=0.,  # arcseconds
                  log_flux=6.832,  # Photons
                  contrast=3.37,
                  bandpass=(530, 640),  # nm
                  weights=None,
                  ):
         """
-        
+        Parameters
+        ----------
+        n_wavels : int
+            The number of wavelengths to model.
+        separation : float
+            The binary separation of the two stars in arcseconds.
+        position_angle : float
+            The position angle of the binary pair in degrees.
+        x_position : float
+            The horizontal offset of the image in arcseconds.
+        y_position : float
+            The vertical offset of the image in arcseconds.
+        log_flux : float
+            The log10 of the total number of photons in the image.
+        contrast : float
+            The flux ratio of Alpha Cen A / Alpha Cen B.
+        bandpass : tuple
+            The wavelength range of the image in nanometers, with syntax (min, max).
+        weights : Array
+            Spectral weights for each wavelength modelled. If None, the weights are uniform.
         """
+
         # Positional Parameters
         self.x_position = x_position
         self.y_position = y_position
         self.separation = separation
         self.position_angle = position_angle
 
         # Flux & Contrast
@@ -86,68 +91,65 @@
         if weights is None:
             self.weights = np.ones((2, n_wavels)) / n_wavels
         else:
             self.weights = weights
 
     def normalise(self):
         """
-        
+        Normalises the source flux to 1.
         """
         return self.multiply('weights', 1 / self.weights.sum(1)[:, None])
 
     @property
     def xy_positions(self):
         """
-        
+        Returns the x and y positions of the two stars in units of radians.
         """
         # Calculate
         r = self.separation / 2
         phi = dlu.deg_to_rad(self.position_angle)
         sep_vec = np.array([r * np.sin(phi), r * np.cos(phi)])
 
         # Add to Position vectors
         pos_vec = np.array([self.x_position, self.y_position])
         output_vec = np.array([pos_vec + sep_vec, pos_vec - sep_vec])
         return dlu.arcsec_to_rad(output_vec)
 
     @property
     def raw_fluxes(self):
         """
-        This casts log flux to be the total (not mean) flux.
+        Returns the raw integrated fluxes of Alpha Centauri A and B respectively, in units of photons.
         """
         flux = (10 ** self.log_flux) / 2
         flux_A = 2 * self.contrast * flux / (1 + self.contrast)
         flux_B = 2 * flux / (1 + self.contrast)
         return np.array([flux_A, flux_B])
 
     @property
     def norm_weights(self):
         """
-        
+        Returns the normalised spectral weights of each modelled wavelength.
         """
         return self.weights / self.weights.sum(1)[:, None]
 
     def model(self: Source(), optics: Optics()) -> Array:
         """
-        Method to model the psf of the point source through the optics.
+        Models the PSF by propagating the AlphaCen source through the given optics.
 
         Parameters
         ----------
         optics : Optics
-            The optics through which to model the source objects.
-        detector : Detector = None
-            The detector object that is observing the psf.
-        filter_in : Filter = None
-            The filter through which the source is being observed.
+            The optics to propagate the source through.
 
         Returns
         -------
         psf : Array
-            The psf of the source modelled through the optics.
+            The PSF of the source modelled through the optics.
         """
+
         # Get Values
         weights = self.norm_weights
         fluxes = self.raw_fluxes
         positions = self.xy_positions
 
         # vmap propagator
         source_propagator = vmap(optics.propagate_mono, in_axes=(0, None))
@@ -156,23 +158,29 @@
         # Model PSF
         input_weights = weights * fluxes[:, None]
         psfs = propagator(self.wavelengths, positions)
         psfs *= input_weights[..., None, None]
         return psfs.sum((0, 1))
 
 
-def get_mixed_alpha_cen_spectra(
-        nwavels: int,
-        min_wavel: float = 545e-9,
-        max_wavels: float = 645e-9
-):
+def get_mixed_alpha_cen_spectra(nwavels: int, bandpass: tuple = (530, 640)):
     """
-    
+    Under Construction. PySynPhot not currently listed in package requirements. TODO complete.
+    Gets the spectra of Alpha Centauri A and B using PySynPhot phoenix models.
+
+    Parameters
+    ----------
+    nwavels : int
+        The number of wavelengths to sample.
+    bandpass : tuple
+        The wavelength range of the image in nanometers, with syntax (min, max).
+
     """
-    # Import Here to prevent issues with google colab install, for example
+
+    # Importing PySynPhot here to prevent issues with Google colab install, for example
     import pysynphot as S
 
     alpha_cen_a_spectrum: float = S.Icat("phoenix",
                                          5790,  # Surface temp (K)
                                          0.2,  # Metalicity (Unit?)
                                          4.0, )  # Surface gravity (unit?)
     alpha_cen_a_spectrum.convert('flam')
@@ -189,109 +197,94 @@
                                   4000,  # Surface temp (K)
                                   0.23,  # Metalicity (Unit?)
                                   4.37)  # Surface gravity (unit?)
     spot_spectrum.convert('flam')
     spot_spectrum.convert('m')
 
     # Full spectrum
-    wavelengths = np.linspace(545e-9, 645e-9, nwavels)
+    wavelengths = 1e-9 * np.linspace(bandpass[0], bandpass[1], nwavels)
     Aspec = alpha_cen_a_spectrum.sample(wavelengths)
     Bspec = alpha_cen_b_spectrum.sample(wavelengths)
     Sspec = spot_spectrum.sample(wavelengths)
 
     Aspec /= Aspec.max()
     Bspec /= Bspec.max()
     Sspec /= Sspec.max()
 
     return np.array([Aspec, Bspec, Sspec]), wavelengths
 
 
 class MixedAlphaCen(AlphaCen):
+    """
+    A class representing an Alpha Centauri class with a mixed spectrum. Each spectrum is generated from the PySynPhot
+    Phoenix model for a star of its properties plus one of the same properties but with a much lower temperature.
+    This lower temperature spectrum represents the contribution of the star spots to the overall spectrum. The ratio
+    of these two different spectra is determined by the 'mixing' parameter.
+
+    Attributes
+    ----------
+    mixing : float
+        The ratio of the spot spectrum to the star spectrum. A value of 0.0 means no spots, 1.0 means only spots.
+
+    Methods
+    -------
+    model()
+        Models the mixed Alpha Cen source through the given optics.
+    """
     mixing: float
 
     def __init__(self,
-                 n_wavels=101,
+                 n_wavels=3,
+                 separation=10.,  # arcseconds
+                 position_angle=90,  # degrees
                  x_position=0.,  # arcseconds
                  y_position=0.,  # arcseconds
-                 separation=10.,  # arcseconds
-                 position_angle=90,  # Degrees
-                 weights=None,
+                 log_flux=6.832,  # Photons
+                 contrast=3.37,
                  mixing=0.05,
-                 log_flux=5,  # Photons TODO: Find true flux
-                 A_mag=1.33,
-                 B_mag=0.01,
+                 bandpass=(530, 640),  # nm
+                 weights=None,
                  ):
         """
         
         """
         self.mixing = mixing
         weights, wavelengths = get_mixed_alpha_cen_spectra(n_wavels)
-        super().__init__(n_wavels, x_position, y_position, separation,
-                         position_angle, weights, log_flux, A_mag, B_mag)
-
-        def plot(self):
-            """
-            
-            """
-            plt.figure(figsize=(12, 4))
-            plt.subplot(1, 2, 1)
-            plt.title(f"Alpha Cen A, f: {f}")
-            plt.xlabel("Wavelength (nm)")
-            plt.ylabel("Weight")
-            plt.plot(spec_wavelengths * 1e9, MixedA, label='Mixed')
-            plt.plot(spec_wavelengths * 1e9, SpecA, label='Main')
-            plt.plot(spec_wavelengths * 1e9, SpottedA, label='Spotted')
-            plt.legend()
-
-            SpecB = (1 - f) * Bspec
-            SpottedB = f * Sspec
-            MixedB = SpecB + SpottedB
-            plt.subplot(1, 2, 2)
-            plt.title("Alpha Cen B, f: {f}")
-            plt.xlabel("Wavelength (nm)")
-            plt.ylabel("Weight")
-            plt.plot(spec_wavelengths * 1e9, MixedB, label='Mixed')
-            plt.plot(spec_wavelengths * 1e9, SpecB, label='Main')
-            plt.plot(spec_wavelengths * 1e9, SpottedB, label='Spotted')
-            plt.legend()
-            plt.show()
+        super().__init__(n_wavels, separation, position_angle, x_position, y_position,
+                         log_flux, contrast, bandpass, weights)
 
     @property
     def norm_weights(self):
         """
-        
+        Returns the normalised spectral weights of each modelled wavelength.
         """
         # Get Spectra
         Spotted = self.mixing * self.weights[2]
         MixedA = (1 - self.mixing) * self.weights[0] + Spotted
         MixedB = (1 - self.mixing) * self.weights[1] + Spotted
         weights = np.array([MixedA, MixedB])
 
         # Normalise
         return weights / weights.sum(1)[:, None]
 
-    def model(self: Source,
-              optics: Optics) -> Array:
+    def model(self: Source, optics: Optics) -> Array:
         """
-        Method to model the psf of the point source through the optics.
+        Models the PSF by propagating the AlphaCen source through the given optics.
 
         Parameters
         ----------
         optics : Optics
-            The optics through which to model the source objects.
-        detector : Detector = None
-            The detector object that is observing the psf.
-        filter_in : Filter = None
-            The filter through which the source is being observed.
+            The optics to propagate the source through.
 
         Returns
         -------
         psf : Array
-            The psf of the source modelled through the optics.
+            The PSF of the source modelled through the optics.
         """
+
         # Get Values
         weights = self.norm_weights
         fluxes = self.raw_fluxes
         positions = self.xy_positions
 
         # vmap propagator
         source_propagator = vmap(optics.propagate_mono, in_axes=(0, None))
```

### Comparing `dLuxToliman-0.1.3/dLuxToliman.egg-info/PKG-INFO` & `dLuxToliman-0.2.0/dLuxToliman.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dLuxToliman
-Version: 0.1.3
+Version: 0.2.0
 Summary: A repo to hold the canonical dLux Toliman models.
 Home-page: https://github.com/maxecharles/dLuxToliman
 Author: Max Charles
 Author-email: max.charles@sydney.edu.au
 Project-URL: Bug Tracker, https://github.com/maxecharles/dLuxToliman/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `dLuxToliman-0.1.3/setup.py` & `dLuxToliman-0.2.0/setup.py`

 * *Files identical despite different names*

