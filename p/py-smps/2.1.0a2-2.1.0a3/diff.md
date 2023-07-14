# Comparing `tmp/py-smps-2.1.0a2.tar.gz` & `tmp/py_smps-2.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-smps-2.1.0a2.tar", last modified: Mon Sep  5 01:04:54 2022, max compression
+gzip compressed data, was "py_smps-2.1.0a3.tar", max compression
```

## Comparing `py-smps-2.1.0a2.tar` & `py_smps-2.1.0a3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1070 2022-09-05 01:04:10.194187 py-smps-2.1.0a2/LICENSE
--rw-r--r--   0        0        0     2335 2022-09-05 01:04:10.194187 py-smps-2.1.0a2/README.md
--rw-r--r--   0        0        0      854 2022-09-05 01:04:10.206188 py-smps-2.1.0a2/pyproject.toml
--rw-r--r--   0        0        0      178 2022-09-05 01:04:10.234188 py-smps-2.1.0a2/smps/__init__.py
--rw-r--r--   0        0        0    19179 2022-09-05 01:04:10.234188 py-smps-2.1.0a2/smps/fit.py
--rw-r--r--   0        0        0     7413 2022-09-05 01:04:10.234188 py-smps-2.1.0a2/smps/io.py
--rw-r--r--   0        0        0    23426 2022-09-05 01:04:10.234188 py-smps-2.1.0a2/smps/models.py
--rw-r--r--   0        0        0     6124 2022-09-05 01:04:10.234188 py-smps-2.1.0a2/smps/plots.py
--rw-r--r--   0        0        0      801 2022-09-05 01:04:10.234188 py-smps-2.1.0a2/smps/rcmod.py
--rw-r--r--   0        0        0     8753 2022-09-05 01:04:10.234188 py-smps-2.1.0a2/smps/utils.py
--rw-r--r--   0        0        0     3351 2022-09-05 01:04:54.800964 py-smps-2.1.0a2/setup.py
--rw-r--r--   0        0        0     3242 2022-09-05 01:04:54.801441 py-smps-2.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 12:07:26.930735 py_smps-2.1.0a3/LICENSE
+-rw-r--r--   0        0        0     2361 2023-07-14 12:07:26.930735 py_smps-2.1.0a3/README.md
+-rw-r--r--   0        0        0      933 2023-07-14 12:07:26.966736 py_smps-2.1.0a3/pyproject.toml
+-rw-r--r--   0        0        0      176 2023-07-14 12:07:27.010737 py_smps-2.1.0a3/smps/__init__.py
+-rw-r--r--   0        0        0    19832 2023-07-14 12:07:27.010737 py_smps-2.1.0a3/smps/fit.py
+-rw-r--r--   0        0        0     7881 2023-07-14 12:07:27.010737 py_smps-2.1.0a3/smps/io.py
+-rw-r--r--   0        0        0    30952 2023-07-14 12:07:27.010737 py_smps-2.1.0a3/smps/models.py
+-rw-r--r--   0        0        0     5414 2023-07-14 12:07:27.010737 py_smps-2.1.0a3/smps/plots.py
+-rw-r--r--   0        0        0      801 2023-07-14 12:07:27.010737 py_smps-2.1.0a3/smps/rcmod.py
+-rw-r--r--   0        0        0     9321 2023-07-14 12:07:27.010737 py_smps-2.1.0a3/smps/utils.py
+-rw-r--r--   0        0        0     3359 1970-01-01 00:00:00.000000 py_smps-2.1.0a3/setup.py
+-rw-r--r--   0        0        0     3362 1970-01-01 00:00:00.000000 py_smps-2.1.0a3/PKG-INFO
```

### Comparing `py-smps-2.1.0a2/LICENSE` & `py_smps-2.1.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `py-smps-2.1.0a2/smps/models.py` & `py_smps-2.1.0a3/smps/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,54 +2,91 @@
 # -*- coding: utf-8 -*-
 """
 """
 import numpy as np
 import pandas as pd
 import math
 import copy
+import sys
 import joblib
 import json
+import logging
 from .utils import make_bins
 
+logging.basicConfig(stream=sys.stdout, level=logging.WARN)
 
 __all__ = [
     "GenericParticleSizer", 
     "SMPS", 
     "AlphasenseOPCN2", 
     "AlphasenseOPCN3", 
     "ModulairPM", 
     "Modulair", 
     "POPS", 
     "ParticlesPlus", 
     "Grimm11D"
 ]
 
 
+class ValidationError(Exception):
+    def __init__(self, msg):
+        self.msg = msg
+
+
 class GenericParticleSizer(object):
     """
-        GenericParticleSizer is the base class for all
-        available particle sizing instruments. It contains
-        all of the basic functionality and methods used for
-        making calculations.
-
-        It can receive data in several formats including: 
-        dN, dNdlogDp.
-        
-        :param data: Data values indexed by timestamp with 
-            bins as columns.
-        :type data: DataFrame
-        :param bins: A list, ordered respective to the bins, 
-            where for each bin a min, midpoint, 
-            and max particle size is given.
-        :type bins: list of lists
-        :param dp_units: Units in which the diameter 
-            is measured, defaults to 'um'.
-        :type dp_units: {'um','nm'}
+    The base class for a Generic Size-Resolving Particle Instrument.
+    
+    Parameters
+    ----------
+    data : pd.DataFrame
+            A dataframe containing the binned particle data, timestamp column, 
+            and optional metadata columns.
+    bins :  array-like
+            A 3xn array defining the left, mid, and right boundaries for 
+            each particle size bin.
+    dp_units : str, deafult='um'
+        Define the units of particle bin sizes - one of ('um', 'nm')
+    meta : dict, default=None
+        An optional dictionary containing meta information about the instrument.
+    weight : str, default='number'
+        The moment of the model. One of ('number', 'surface', 'volume').
+    units : str, default='dw/dlogdp'
+        The default data format in AIM-compatible string format.
+    bin_weights : array-like, default=ones
+        An optional array to set bin weights (e.g., counting efficiency). By 
+        default, all bin weights are 1.
+    bin_prefix : str, default='bin'
+        An optional kwarg to name the bins if not already named.
+    fmt : str, default='dn' 
+        Optional kwarg describing the default data format. One of ('dn', 'dndlogdp').
+    
+    See Also
+    --------
+    smps.models.Modulair
+    smps.models.ModulairPM
+    smps.models.SMPS
+    smps.models.Grimm11D
+    smps.models.POPS
+    smps.models.ParticlesPlus
+    smps.models.AlphasenseOPCN2
+    smps.models.AlphasenseOPCN3
+
+    Examples
+    --------
+    
+    Initialize a base object with data and bins:
+    
+    >>> obj = smps.models.GenericParticleSizer(data=df, bins=bins)
+    
     """
     def __init__(self, data, bins, **kwargs):
+        self.logger = logging.getLogger(__name__)
+        self.logger.setLevel(logging.DEBUG)
+
         self.data = data.copy(deep=True)
         self.bins = bins
         self.meta = kwargs.pop('meta', dict())
         self.bin_labels = kwargs.pop('bin_labels', None)
 
         self.meta['weight'] = kwargs.pop("weight", "number")
         self.meta['units'] = kwargs.pop("units", "dw/dlogdp")
@@ -89,119 +126,133 @@
             .data[self.bin_labels]
             .mul(self.bin_weights)
         )
 
     @property
     def s_multiplier(self):
         """
-        A list of the surface areas corresponding
-        to the midpoitns of the respective bins.
+        Per particle surface area representing the mean particle in each bin.
         """
         return 4 * np.pi * (self.bins[:, 1]/2)**2
 
     @property
     def v_multiplier(self):
         """
-        A list of the volumes corresponding to the 
-        midpoitns of the respective bins.
+        Per particle volume representing the mean particle in each bin.
         """
         return (4./3)*np.pi*(self.bins[:, 1]/2)**3
 
     @property
     def midpoints(self):
         """
-        A list of the midpoints of the respective bins.
+        Midpoint particle diameter in each bin.
         """
         return self.bins[:, 1]
 
     @property
     def dlogdp(self):
         """
-        A list of the differences between the upper 
-        and lower bound of each bin on a Log scale.
+        Log difference between the upper and lower bound of each bin.
         """
         return np.log10(self.bins[:, -1]) - np.log10(self.bins[:, 0])
 
     @property
     def dn(self):
         """
-        A DataFrame with the number of particles in 
-        each bin at each time.
+        The number concentration per bin. Can otherwise be represented as :math:`dN/dD_p`. Units 
+        are pp/cm3.
         """
         return self.dndlogdp.mul(self.dlogdp)
 
     @property
     def dndlogdp(self):
         """
-        The histogram in units of dNd/logDp [#/cm3].
+        The log normalized number concentration per bin. Can otherwise be represented as 
+        :math:`dN/dlogD_p`. Units are pp/cm3.
         """
         return self.data[self.bin_labels]
 
     @property
     def dddlogdp(self):
         """
-        The histogram in units of dDpd/logDp [um/cm3].
+        Can otherwise be represented as :math:`dD/dlogD_p`.
         """
         return self.dndlogdp.mul(self.midpoints)
 
     @property
     def ds(self):
         """
-        A DataFrame with the total surface area of 
-        all the particles in each bin at each time.
+        Surface area per bin.
         """
         return self.dn.mul(self.s_multiplier)
 
     @property
     def dsdlogdp(self):
         """
-        The histogram in units of dSd/logDp [um2/cm3].
+        Log normalized surface area per bin. Otherwise represented as :math:`dS/dlogDp`.
+        Units are: µm2/cm3.
         """
         return self.dndlogdp.mul(self.s_multiplier)
 
     @property
     def dv(self):
         """
-        A DataFrame with the total volume of all 
-        the particels in each bin at each time.
+        Volume per bin.
         """
         return self.dvdlogdp.mul(self.dlogdp)
 
     @property
     def dvdlogdp(self):
         """
-        The histogram in units of dSd/logDp [um3/cm3].
+        Log normalized volume per bin. Can otherwise be represented as
+        :math:`dV/dlogDp`. Units are µm3/cm3.
         """
         return self.dndlogdp.mul(self.v_multiplier)
 
+    @property
+    def scan_stats(self):
+        """
+        Return the non-binned data.
+        """
+        return self.data[list(set(self.data.columns)
+                              - set(self.bin_labels))]
+        
     def copy(self):
         """
         Return a copy of the GenericParticleSizer.
+        
+        Examples
+        --------
+        >>> obj = GenericParticleSize(data=df)
+        >>> cpy = obj.copy()
         """
         return copy.deepcopy(self)
 
-    def dump(self, filepath, ):
+    def dump(self, filepath):
         """
-        Save a copy to disk at `filepath`.
-
-        :param filepath: The path at which to save the file.
-        :type filepath: string
-        :return: The list of file names in which the data is stored.
-        :rtype: list of strings
+        Save a copy of the model to disk.
+        
+        Parameters
+        ----------
+        filepath : str
+            The filepath to save the file at.
+        
+        Returns
+        -------
+        filepath : list
+            The list of filepaths where data was saved.
+        
+        Examples
+        --------
+        
+        >>> model.dump(filepath="path-to-file.sav")
+        
         """
         return joblib.dump(self, filepath)
 
-    @property
-    def scan_stats(self):
-        """
-        A DataFrame with all the data except for the bin data.
-        """
-        return self.data[list(set(self.data.columns)
-                              - set(self.bin_labels))]
-
     def _subselect_frame(self, df, dmin=0., dmax=1e3):
         """
         Sub-select the bins that are used to make calculations by
         zeroing out bins which are outside of the range. This
         is similar to a slice, except in the bin-dimension 
         rather than the time-dimension. Edge cases are 
         appropriately weighted.
@@ -234,50 +285,92 @@
         # copy the dataframe
         cpy = df.copy()
 
         # multiply the histogram by the factors we just calculated
         cpy[self.bin_labels] = cpy[self.bin_labels].mul(factors)
 
         return cpy
+    
+    def _subselect_bins(self, **kwargs):
+        """Return an array of multipliers corresponding to the 
+        percentage of a given bin to use in a calculation based 
+        on the size cutoffs defined.
+        
+        Args:
+            bins (array): Array of bins
+            dmin (float): Minimum particle diameter
+            dmax (float): Maximum particle diameter
+        """
+        bins = kwargs.pop("bins")
+        dmin = kwargs.pop("dmin")
+        dmax = kwargs.pop("dmax")
+        
+        # Create a placeholder for the factors
+        factors = np.zeros(bins.shape[0])
+        
+        for i, b in enumerate(bins):
+            if b[0] >= dmin and b[-1] <= dmax:
+                factors[i] = 1.
+            
+            if dmin >= b[0] and dmin < b[-1]:
+                factors[i] = (b[-1] - dmin) / (b[-1] - b[0])
+            
+            if dmax >= b[0] and dmax < b[-1]:
+                factors[i] = (dmax - b[0]) / (b[-1] - b[0])
+        
+        return factors
 
-    def stats(self, weight='number', dmin=0., 
-              dmax=1e3, rho=1.65, **kwargs):
+    def stats(self, weight='number', dmin=0., dmax=1e3, rho=1.65, **kwargs):
         """
-        Calculate and return the total number of particles, 
-        total surface area, total volume, and total mass 
-        between dmin and dmax. In addition, the arithmetic 
-        mean (AM), geometric mean (GM), mode (Mode), and geometric 
-        standard deviation (GSD, CMD) are calculated and are
-        weighted by the input parameter `weight`.
-        
-        :param weight: The dimension to consider in computing 
-            statistics.
-        :type weight: {"number", "surface", "volume", "mass"}
-        :param dmin: The minimum particle diameter in microns, 
-            defaults to `0`.
-        :type dmin: float
-        :param dmax: The maximum particle diameter in microns, 
-            defaults to `1e3`.
-        :type dmax: float
-        :param rho: The particle density in units of g/cc3, 
-            defaults to `1.65`.
-        :type rho: float
-        :return: The statistics for each timestamp.
-        :rtype: DataFrame
+        Compute and return the aerosol size distribution statistics.
+        
+        Calculate the total number of particles, surface area, 
+        volume, mass, arithmetic mean particle diameter, 
+        geometric mean particle diameter, and geometric 
+        standard deviation between any two particle diameters.
+        
+        Parameters
+        ----------
+        weight: str, default='number'
+            The moment to use to compute the statistics. Should be one of 
+            ('number', 'surface', 'volume', 'mass').
+        dmin : float, default=0.0
+            The minimum particle diameter to consider. Units are in µm.
+        dmax : float, default=1000.0
+            The maximum particle diameter to consider. Units are in µm.
+        rho : float, default=1.65
+            The particle density in units of g/cm3.
+        
+        Returns
+        -------
+        data : pd.DataFrame
+            A dataframe containing the computed statistics at each point in time.
+        
+        Examples
+        --------
+        
+        Compute the number-weighted stats
+        
+        >>> obj.stats(weight='number')
+        
+        Compute the volume-weighted stats for PM2.5
+        
+        >>> obj.stats(weight='volume', dmin=0, dmax=2.5)
+        
         """
         # remove the weight from the kwargs
         assert(weight in ["number", "surface", "volume", "mass"])
 
         # initialize an empty dataframe to hold the results
         res = pd.DataFrame(index=self.data.index)
 
         # subselect the dataframe to only include 
         # diameters of interest
         cpy = self.copy()
-        cpy.data = cpy._subselect_frame(cpy.data, **kwargs)
+        cpy.data = cpy._subselect_frame(cpy.data, dmin=dmin, dmax=dmax, **kwargs)
 
         # drop all rows that are completely NaN
         cpy.data = cpy.data.dropna(how='all')
 
         # make a shortcut for the index to inject
         idx = cpy.data.index
 
@@ -374,96 +467,211 @@
         # delete the cpy to free up memory
         del cpy, tmp
 
         return res
 
     def integrate(self, weight='number', dmin=0., dmax=1., **kwargs):
         """
-        For each timestamp give the total number 
-        (or surface, volume, or mass) of all the particles 
-        (with a diameter between `dmin` and `dmax`) at that time.
-        
-        :param weight: The variable to sum over, 
-            defaults to "number".
-        :type weight: {"number", "surface", "volume", "mass"}
-        :param dmin: The minimum particle diameter in microns, 
-            defaults to `0`.
-        :type dmin: float
-        :param dmax: The maximum particle diameter in microns, 
-            defaults to `1e3`.
-        :type dmax: float
-        :param rho: The particle density in units of g/cc3, 
-            defaults to `1.65`.
-        :type rho: float
-        :return: The desired values indexed by timestamp.
-        :rtype: Pandas Series
+        Integrate by weight for each record in time.
+        
+        Compute the total number of particles, surface area, volume, or 
+        mass between any two particle diameters. Correct for hygroscopic 
+        growth by defining a hygroscopic growth factor, kappa.
+        
+        Parameters
+        ----------
+        weight : str, default='number'
+            The moment/variable to integrate. One of ('number', 'surface', 'volume', 'mass').
+        dmin : float, default=0.0
+            The minimum particle diameter in µm.
+        dmax : float, default=1.
+            The maximum particle diameter in µm.
+        rho : float or callable
+            The density as a float or a callable function which takes particle diameter as its 
+            only argument and returns the density at that diameter.
+        kappa : float or callable
+            The kappa growth factor as a float or a callable function which takes particles diameter 
+            as its only argument and returns the kappa value at that diameter.
+        rh : str
+            If kappa is defined, rh is the column of data corresponding to the relative humidity 
+            which is required to correct for hygroscopic growth.
+        
+        Returns
+        -------
+        data : pd.Series
+            A series containing the integrated values.
+        
+        Examples
+        --------
+        
+        Compute the total particle concentration under 1 µm:
+        
+        >>> obj.integrate(weight='number', dmin=0., dmax=1.)
+        
+        Compute PM1
+        
+        >>> obj.integrate(weight='mass', dmin=0., dmax=1.)
+        
+        Compute PM2.5 assuming a kappa=0.3
+        
+        >>> obj.integrate(weight='mass', dmin=0., dmax=2.5, kappa=0.3, rh="sample_rh")
+        
         """
+        # Convert the density to a callable if not already
         rho = kwargs.pop("rho", 1.65)
-
-        weight = weight.lower()
+        if not callable(rho):
+            _rho = lambda x: rho
+        else:
+            _rho = rho
 
         assert(weight in ['number', 'surface', 'volume', 'mass']), \
-        "Invalid `weight`"
-
-        if weight == 'number':
-            df = self.dn
-        elif weight == 'surface':
-            df = self.ds
-        elif weight == 'volume':
-            df = self.dv
+                "Invalid `weight`"
+                
+        # Check for kappa
+        kappa = kwargs.pop("kappa", None)
+        if kappa:
+            if not callable(kappa):
+                _kappa = lambda x: kappa
+            else:
+                _kappa = kappa
+                
+            # Check for a column with rh
+            rh_c = kwargs.pop("rh", None)
+            if not rh_c:
+                raise AttributeError("`rh` is a required column when correcting for hygroscopic growth")
+            
+            # Check to make sure the rh column exists
+            if rh_c not in self.data.columns:
+                raise ValidationError(f"No column for {rh_c} was found in `data`")
+            
+            # Check to see if there are rh values below 1% or above 95%
+            count_low_rh = self.data[self.data[rh_c] <= 1.0].shape[0]
+            if count_low_rh > 0:
+                self.logger.warning(f"There are {count_low_rh} values below 1% RH in your data which may cause problems when correcting for hygroscopic growth.")
+            
+            count_high_rh = self.data[self.data[rh_c] >= 95.0].shape[0]
+            if count_high_rh > 0:
+                self.logger.warning(f"There are {count_high_rh} values above 95% RH in your data which may cause problems when correcting for hygroscopic growth.")
         else:
-            df = self.dv * rho
-
-        # subsample the data
-        df = self._subselect_frame(df, dmin=dmin, dmax=dmax)
-
-        return df[self.bin_labels].sum(axis=1)
+            _kappa = None
+            
+        # If kappa is not set, compute the integrated values and return
+        if not _kappa:
+            if weight == 'number':
+                df = self.dn
+            elif weight == 'surface':
+                df = self.ds
+            elif weight == 'volume':
+                df = self.dv
+            else:
+                df = self.dv * [_rho(dp) for dp in self.midpoints]
+            
+            # Subsample the data and return
+            df = self._subselect_frame(df, dmin=dmin, dmax=dmax)
+            
+            return df[self.bin_labels].sum(axis=1)
+             
+        def compute_integration_by_row(row, weight):
+            # Recompute the bins
+            _bins = self.bins.copy()
+            
+            # Get rh
+            rh = row[rh_c]
+            
+            # Compute kappa for each (wet) diameter
+            k = [_kappa(dp) for dp in _bins[:, 1]]
+            
+            for i in range(_bins.shape[0]):
+                for j in range(3):
+                    _bins[i, j] = _bins[i, j] / (1 + k[i] * (rh / (100. - rh)))**(1./3.)
+                    
+            # Extract the midpoints
+            midpoints = _bins[:, 1]
+            
+            # Keep only the data for the bins that are relevant for this record
+            histogram = row[self.bin_labels] * self._subselect_bins(dmin=dmin, dmax=dmax, bins=_bins)
+            
+            # Return the histogram depending on which weight we're using
+            if weight == 'surface':
+                hgram = histogram.mul((4 * np.pi * (_bins[:, 1]/2)**2))
+            elif weight == 'volume':
+                hgram = histogram.mul((4./3)*np.pi*(_bins[:, 1]/2)**3)
+            elif weight == 'mass':
+                hgram = histogram.mul((4./3)*np.pi*(_bins[:, 1]/2)**3).mul([_rho(dp) for dp in _bins[:, 1]])
+            else:
+                hgram = histogram
+                
+            return hgram.sum()
+        
+        # Create a dataframe that is dn + humidity so that we are always sending the correct 
+        # format to the integration computation 
+        cpy = self.dn
+        cpy.loc[:, rh_c] = self.data[rh_c]
+        
+        s = cpy.apply(compute_integration_by_row, axis=1, weight=weight)
+        
+        return s
 
     def slice(self, start=None, end=None, inplace=False):
         """
-        Slice the data between the start and end dates, inclusive.
+        Slice the data between two datetimes.
+        
+        Parameters
+        ----------
+        start : str
+            The timestamp (as a string) to begin the slice.
+        end : str
+            The timestamp (as a string) to end the slice.
+        inplace : bool, default=False
+            If True, replace the data with the specified slice of the data, 
+            otherwise return a copy of the sliced data.
+        
+        Returns
+        -------
+        data : pd.DataFrame or None
+            If inplace=False, return the dataframe with the sliced data.
+        
+        Examples
+        --------
+        >>> obj.slice(start="2023-01-01", end="2023-02-15")
         
-        :param start: The first timestamp to be contained 
-            in the result.
-        :type start: string, Pandas Timestamp, or numpy DateTime64
-        :param end: The last timestamp to be contained in the 
-            result.
-        :type end: string, Pandas Timestamp, or numpy DateTime64
-        :param inplace: If False a new object is returned, 
-            defaults to False.
-        :type inplace: bool
-        :return: The data restricted to the given time interval.
-        :rtype: an object the same type as self
         """
         if inplace:
             self.data = self.data[start:end]
         else:
             cpy = self.copy()
 
             cpy.data = cpy.data[start:end]
 
             return cpy
         return
 
     def resample(self, rs, inplace=False):
         """
-        Resample on the timeseries.
-
-        :param rs: The resample period using normal 
-            Pandas conventions.
-        :type rs: string
-        :param inplace: If True, update the current instance, 
-            otherwise create a new one and return it.
-        :type inpace: bool
-        :return: A timeseries that has been resampled with 
-            period `rs`.
-        :rtype: an object from the same class as `self`
-
-        Example::
-            m.resample("15min", True)
+        Resample the data to a new time base.
+        
+        Parameters
+        ----------
+        rs : str
+            The resample period using normal pandas convention. Examples include 
+            '1h', '1d', '15min', etc.
+        inplace : bool, default=False
+            If True, modify the data inplace, otherwise return.
+        
+        Returns
+        -------
+        data : pd.DataFrame or None
+            If inplace=False, return the dataframe with the resampled data.
+        
+        Examples
+        --------
+        
+        Resample to 1h and modify in place
+        
+        >>> obj.resample('1h', inplace=True)
 
         """
         obj_cols = (
             self
             .data
             .select_dtypes(include=['object'])
             .resample(rs)
@@ -528,29 +736,35 @@
             )
         )
 
         return gsd
 
     
 class SMPS(GenericParticleSizer):
+    """
+    The TSI Scanning Mobility Particle Sizer.
+    
+    The TSI SMPS is a research instrument 
+    for counting and sizing submicron aerosol.
+    
+    """
     def __init__(self, **kwargs):
-        super(SMPS, self).__init__(fmt='dndlogdp', dp_units='nm', 
-                                   **kwargs)
-    def __repr__(self):
-        return "<SMPS>"
+        super(SMPS, self).__init__(fmt='dndlogdp', dp_units='nm', **kwargs)
 
 
 class AlphasenseOPCN2(GenericParticleSizer):
     """
-    The Alphasense OPC-N2 is a consumer-grade optical 
-    particle counter that uses a 658 nm red laser to count 
-    and size individual particles. It can count particles 
-    between 380-17,500 nm. Read more `here
+    The Alphasense OPC-N2.
+    
+    The Alphasense OPC-N2 is a consumer-grade OPC
+    that uses a 658 nm red laser to count 
+    and size particles between 380 - 17,500 nm. Read more `here
     <https://www.alphasense.com/products/
     optical-particle-counter/>`__.
+    
     """
     def __init__(self, **kwargs):
         bb = np.array([0.38, 0.54, 0.78, 1.05, 1.34, 1.59, 2.07, 3., 
                        4., 5., 6.5, 8., 10., 12., 14., 16., 17.5])
 
         bins = kwargs.pop("bins", make_bins(boundaries=bb))
         fmt = kwargs.pop("fmt", "dn")
@@ -565,14 +779,16 @@
             bin_labels=bin_labels, 
             **kwargs
         )
 
 
 class AlphasenseOPCN3(GenericParticleSizer):
     """
+    The Alphasense OPC-N3.
+    
     The Alphasense OPC-N3 is a consumer-grade optical
     particle counter that uses a 658 nm red laser to count 
     and size individual particles. It can count particles 
     between 380-40,000 nm. Read more `here <https://www.
     alphasense.com/products/optical-particle-counter/>`__.
     """
     def __init__(self, **kwargs):
@@ -590,16 +806,19 @@
         super(AlphasenseOPCN3, self).__init__(
             bins=bins, 
             fmt=fmt, 
             bin_labels=bin_labels, 
             **kwargs
         )
 
+
 class ModulairPM(GenericParticleSizer):
     """
+    The QuantAQ MODULAIR-PM.
+    
     QuantAQ's MODULAIR-PM sensors use the Alphasense OPC-N3,
     a consumer-grade optical particle counter that uses a 658 nm 
     red laser to count and size individual particles. It can 
     count particles between 380-40,000 nm. Read more 
     `here <https://www.alphasense.com/products/optical-particle-counter/>`__.
     """
     def __init__(self, **kwargs):
@@ -617,16 +836,19 @@
         super(ModulairPM, self).__init__(
             bins=bins, 
             fmt=fmt, 
             bin_labels=bin_labels, 
             **kwargs
         )
 
+
 class Modulair(GenericParticleSizer):
     """
+    The QuantAQ MODULAIR.
+    
     QuantAQ's MODULAIR sensors use the Alphasense OPC-N3,
     a consumer-grade optical particle counter that uses a 658 nm 
     red laser to count and size individual particles. It can 
     count particles between 380-40,000 nm. However, because the last
     few bins (bin18-bin24) collect negligible data, they are removed to conserve 
     memory, which means the MODULAIR data differs slightly from the MODULAIR-PM data.
     Read more about the Alphasense OPC-N3
@@ -650,14 +872,16 @@
             bin_labels=bin_labels, 
             **kwargs
         )
 
 
 class POPS(GenericParticleSizer):
     """
+    The Handix Scientific Portable Optical Particle Spectrometer (POPS).
+    
     The Portable Optical Particle Spectrometer is based on 
     the design of R. Gao and is currently manufactured by 
     Handix Scientific. It is a research-grade OPC that can see 
     particles as small as 132 nm. Read more `here 
     <http://www.handixscientific.com/pops>`__.
     """
     def __init__(self, **kwargs):
@@ -678,14 +902,16 @@
             bin_labels=bin_labels, 
             **kwargs
         )
 
 
 class ParticlesPlus(GenericParticleSizer):
     """
+    The Particles Plus OPC.
+    
     The Particles Plus is a consumer-grade optical particle counter
     that uses a red laser to count and size individual particles. It
     can count particles between 300-10,000 nm. Read more `here 
     <https://particlesplus.com/ambient-air-monitoring/>`__.
     """
     def __init__(self, **kwargs):
         bb = np.array([0.3, 0.5, 0.7, 1., 2.5, 10.0, 10.1])
@@ -703,14 +929,16 @@
             bin_labels=bin_labels, 
             **kwargs
         )
 
 
 class Grimm11D(GenericParticleSizer):
     """
+    The GRIMM 11D.
+    
     The Grimm11D is an optical particle counter that uses a blue 
     laser to count and size individual particles. It can count 
     particles between 250-35,000 nm. Read more `here 
     <https://www.grimm-aerosol.com/products-en/dust-monitors/the-
     dust-decoder/11-d/>`__.
     """
     def __init__(self, **kwargs):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `py-smps-2.1.0a2/smps/rcmod.py` & `py_smps-2.1.0a3/smps/rcmod.py`

 * *Files identical despite different names*

### Comparing `py-smps-2.1.0a2/smps/utils.py` & `py_smps-2.1.0a3/smps/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,43 +5,63 @@
 import numpy as np
 import requests
 import math
 from scipy.stats.mstats import gmean
 
 def make_bins(**kwargs):
     """
-    'make_bins` computes the upper and lower bounds and
-    midpoints of all the bins given either
-    * `boundaries`
-    * `boundaries_left` and `boundaries_right`
-    * or `lb`, `ub`, and `midpoints` (`channels_per_decade` optional).
-    
-    :param boundaries: A list containing, for each bin, a list of 
-        the lower and upper bound for the bin.
-    :type boundaries: list of lists, or numpy array
-    :param boundaries_left: A list of lower boundaries for each bin.
-    :type boundaries_left: list
-    :param boundaries_right: A list of upper boundaries for each 
-        bin.
-    :type boundaries_right: list
-    :param lb: The lower bound of the lowermost bin.
-    :type lb: float
-    :param ub: The upper bound of the uppermost bin.
-    :type ub: float
-    :param midpoints: A list of midpoints for each bin.
-    :type midpoints: list
-    :param channels_per_decade: A measure of bin width on the log 
-        scale.
-    :type channels_per_decade: float
-    :param mean_calc: Determins wether the geometric or arethmetic 
-        mean should be used to compute the midpoints.
-    :type mean_calc: {"gm", "am"}
-    :return: For each bin a row is given with the lower boundary, 
-        the midpoint, and the upper bounary for that bin.
-    :rtype: numpy array
+    Create a 3xn array of particle size bins.
+    
+    Compute the lower boundary, upper boundary, and midpoint 
+    diameter for each particle size bin.
+    
+    Parameters
+    ----------
+    boundaries : array-like
+        A list or array containing all unique lower and upper bounds.
+    boundaries_left : array-like
+        A list of lower boundaries for each bin. If used, you must also define the boundaries_right.
+    boundaries_right : array-like
+        A list of upper boundaries for each bin. If used, you must also define the boundaries_left.
+    lb : float
+        The lower bound of the lowest size bin. If used, you must also provide a value for ub.
+    ub : float
+        The upper bound of the largest size bin. If used, you must also provide a value for lb.
+    midpoints : array-like
+        A list of midpoints to use. If used, you must also provide values for lb and ub.
+    channels_per_decade : int
+        A measure of the bin width on a log scale.
+    mean_calc : str
+        The method of calculation for midpoints. Should be one of ('am', 'gm') corresponding 
+        to the arithmetic or geometric mean.
+    
+    Returns
+    -------
+    bins : array-like
+        A 3xn array of particle size bins with a (lower boundary, midpoint, upper boundary)
+        for each particle size bin.
+    
+    Examples
+    --------
+    
+    Create a set of bins from a list of boundaries:
+    
+    >>> bins = make_bins(boundaries=np.array([0.35, 1.0, 2.5, 10.0]))
+    
+    Create a set of bins from lists of lower and upper boundaries:
+    
+    >>> bins = make_bins(
+    >>>    boundaries_left=np.array([0.35, 1.0, 2.5]),
+    >>>    boundaries_right=np.array([1.0, 2.5, 10.0])
+    >>> )
+    
+    Create a set of bins from the lowest boundary, highest boundary, and midpoints:
+    
+    >>> bins = make_bins(lb=0.35, ub=10.0, midpoints=np.array([.5, 2.0, 5.0]))
+    
     """
     boundaries = kwargs.pop("boundaries", None)
     boundaries_left = kwargs.pop("boundaries_left", None)
     boundaries_right = kwargs.pop("boundaries_right", None)
     lb = kwargs.pop("lb", None)
     ub = kwargs.pop("ub", None)
     midpoints = kwargs.pop("midpoints", None)
@@ -100,18 +120,15 @@
 
     # calculate the midpoints
     assert(mean_calc in ("gm", "am")), "Invalid mean calculation method."
 
     if mean_calc == 'am':
         bins[:, 1] = (bins[:, 0] + bins[:, 2]) / 2
     else:
-        bins[:, 1] = [gmean([x, y]) for x, y in zip(
-            bins[:, 0], 
-            bins[:, 2]
-        )]
+        bins[:, 1] = [gmean([x, y]) for x, y in zip(bins[:, 0], bins[:, 2])]
 
     return bins
 
 def _get_bin_count(fpath, delimiter=',', encoding='ISO-8859-1'):
     """
     Gets the number of bins in the file.
```

### Comparing `py-smps-2.1.0a2/setup.py` & `py_smps-2.1.0a3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,32 +7,32 @@
 packages = \
 ['smps']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['joblib>=1.0,<2.0',
- 'numpy>=1.23.2,<2.0.0',
+['joblib>=1.2,<2.0',
+ 'numpy>=1.23,<2.0',
  'pandas>=1.4,<2.0',
  'requests>=2.24,<3.0',
  'scipy>=1.9,<2.0',
- 'seaborn>=0.11.0,<0.12.0',
+ 'seaborn>=0.12,<0.13',
  'setuptools>=65.0,<66.0',
  'statsmodels>=0.13,<0.14']
 
 setup_kwargs = {
     'name': 'py-smps',
-    'version': '2.1.0a2',
+    'version': '2.1.0a3',
     'description': 'A simple python library to import and visualize data from particle sizing instruments.',
-    'long_description': '[![PyPI version](https://badge.fury.io/py/py-smps.svg)](https://badge.fury.io/py/py-smps)\n[![Build Status](https://travis-ci.org/dhhagan/py-smps.svg?branch=master)](https://travis-ci.org/dhhagan/py-smps)\n[![Coverage Status](https://coveralls.io/repos/github/dhhagan/py-smps/badge.svg?branch=master)](https://coveralls.io/github/dhhagan/py-smps?branch=master)\n\n\n# py-smps\nPython library for the analysis and visualization of data from a Scanning Mobility Particle Sizer (SMPS) and other particle sizing instruments (SEMS, OPC\'s).\n\n## Dependencies\n\nThe full list of dependencies can be found in the `pyproject.toml` file and are summarized below:\n\n```py\npython = ">=3.8, <3.12"\nstatsmodels = "^0.13"\nseaborn = "^0.10"\njoblib = "^1.0"\nrequests = "^2.24"\nscipy = "^1.9"\nnumpy = "^1.23.2"\npandas = "^1.4"\n```\n\nAs of `v1.2.0a0`, the library should be compatible with Apple silicone (tested on both M1 and M2).\n\n## Python Versions\n\nPython3.8 through Python3.11 are currently supported.\n\n## Installation\n\nTo install from PyPi:\n\n    $ pip install py-smps [--upgrade]\n\nIf you\'d like the latest pre-release:\n\n    $ pip install py-smps --pre [--upgrade]\n\nTo install the edge release directly from GitHub:\n\n    pip install git+https://github.com/quant-aq/py-smps.git\n\n## Unittests\n\nUnittests can be run by issuing the following command from within the main repo:\n\n```sh\n$ poetry run pytest -s tests/ --ignore=tests/datafiles\n```\n\n\n## Documentation\n\nDocumentation is available [here](https://quant-aq.github.io/py-smps/). Docs are built using Sphinx and can be built locally by doing the following:\n\n```sh\n$ cd docs/\n$ make clean\n$ make guides\n$ make html\n$ cd ..\n```\n\nThen, you can navigate to your local directory at `docs/_build/html/` and open up the `index.html` file in your preferred browser window.\n\n\n## Contributing to Development\n\nWe welcome all contributions from the community in the form of issues reporting, feature requests, bug fixes, etc.\n\nIf there is a feature you would like to see or a bug you would like to report, please open an issue. We will try to get to things as promptly as possible. Otherwise, feel free to send PR\'s!\n\n\n## Colorbar Information\n\n  * [matplotlib colorbars](http://matplotlib.org/examples/color/colormaps_reference.html)\n  * [seaborn color palette](http://seaborn.pydata.org/tutorial/color_palettes.html)\n\n',
+    'long_description': "[![PyPI version](https://badge.fury.io/py/py-smps.svg)](https://badge.fury.io/py/py-smps)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n[![Coverage Status](https://coveralls.io/repos/github/dhhagan/py-smps/badge.svg?branch=master)](https://coveralls.io/github/dhhagan/py-smps?branch=master)\n[![ci.tests](https://github.com/quant-aq/py-smps/actions/workflows/test-and-report.yml/badge.svg)](https://github.com/quant-aq/py-smps/actions/workflows/test-and-report.yml)\n\n\n# py-smps\n\npy-smps is a Python data analysis library built for analyzing size-resolved aerosol data from a variety of aerosol sizing instruments (e.g., Scanning Mobility Particle Sizer, Optical Particle Counters).\n\n\n**NOTE: As of `v1.2.0`, the library is compatible with Apple silicone (M1, M2 chips).**\n\n# Installation\n\nOfficial releases of `py-smps` can be installed from [PyPI](https://pypi.org/project/py-smps/):\n\n    $ pip install py-smps [--upgrade]\n\nIf you'd like the latest pre-release:\n\n    $ pip install py-smps --pre [--upgrade]\n\nTo install the edge release directly from GitHub:\n\n    pip install git+https://github.com/quant-aq/py-smps.git\n\n# Dependencies\n\n## Supported Python versions\n- Python 3.8+\n\n## Mandatory Dependencies\n\nThe full list of dependencies can be found in the [`pyproject.toml`](pyproject.toml) file.\n\n# Development\n\n## Testing\n\nTests can be run by issuing the following command from within the main repo:\n\n```sh\n$ poetry run pytest -s tests/ --ignore=tests/datafiles\n```\n\n## Contributing to Development\n\nWe welcome all contributions from the community in the form of issues reporting, feature requests, bug fixes, etc.\n\nIf there is a feature you would like to see or a bug you would like to report, please open an issue. We will try to get to things as promptly as possible. Otherwise, feel free to send PR's!\n\n\n# Documentation\n\nDocumentation is available [here](https://quant-aq.github.io/py-smps/). To build locally, you must first install [pandoc](https://pandoc.org/). Docs are built using Sphinx and can be built locally by doing the following:\n\n```sh\n# Activate the virtualenv\n$ poetry shell\n\n# Build the docs\n$ cd docs/\n$ make clean\n$ make html\n$ cd ..\n```\n\nThen, you can navigate to your local directory at `docs/build/html/` and open up the `index.html` file in your preferred browser window.",
     'author': 'David H Hagan',
     'author_email': 'david.hagan@quant-aq.com',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/quant-aq/py-smps',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.8,<3.12',
 }
```

