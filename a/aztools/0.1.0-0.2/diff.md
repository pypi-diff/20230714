# Comparing `tmp/aztools-0.1.0.tar.gz` & `tmp/aztools-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aztools-0.1.0.tar", last modified: Tue Mar 30 15:34:23 2021, max compression
+gzip compressed data, was "aztools-0.2.tar", last modified: Fri Jul 14 11:51:53 2023, max compression
```

## Comparing `aztools-0.1.0.tar` & `aztools-0.2.tar`

### file list

```diff
@@ -1,10 +1,53 @@
-drwxr-xr-x   0 abzoghbi (99974152) users      (100)        0 2021-03-30 15:34:23.634967 aztools-0.1.0/
--rw-r--r--   0 abzoghbi (99974152) users      (100)      795 2021-03-30 15:34:23.634967 aztools-0.1.0/PKG-INFO
-drwxr-xr-x   0 abzoghbi (99974152) users      (100)        0 2021-03-30 15:34:23.634967 aztools-0.1.0/aztools/
--rw-r--r--   0 abzoghbi (99974152) users      (100)       97 2020-04-22 11:48:30.066726 aztools-0.1.0/aztools/__init__.py
--rw-r--r--   0 abzoghbi (99974152) users      (100)    25072 2021-02-21 03:49:33.269813 aztools-0.1.0/aztools/data_tools.py
--rw-r--r--   0 abzoghbi (99974152) users      (100)    32014 2020-12-21 02:18:41.734736 aztools-0.1.0/aztools/lcurve.py
--rw-r--r--   0 abzoghbi (99974152) users      (100)    12975 2020-05-08 14:52:12.832281 aztools-0.1.0/aztools/misc.py
--rw-r--r--   0 abzoghbi (99974152) users      (100)    13903 2018-10-23 16:16:11.807626 aztools-0.1.0/aztools/simlc.py
--rw-r--r--   0 abzoghbi (99974152) users      (100)       39 2021-03-30 15:28:59.215124 aztools-0.1.0/setup.cfg
--rw-r--r--   0 abzoghbi (99974152) users      (100)      920 2021-03-30 15:29:55.656968 aztools-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:51:53.202162 aztools-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-14 11:51:38.000000 aztools-0.2/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:51:53.194162 aztools-0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:51:53.198162 aztools-0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-14 11:51:38.000000 aztools-0.2/.github/workflows/build-documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-14 11:51:38.000000 aztools-0.2/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-14 11:51:38.000000 aztools-0.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-14 11:51:38.000000 aztools-0.2/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-14 11:51:38.000000 aztools-0.2/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-07-14 11:51:38.000000 aztools-0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-07-14 11:51:38.000000 aztools-0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-14 11:51:38.000000 aztools-0.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-14 11:51:38.000000 aztools-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-14 11:51:53.202162 aztools-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-14 11:51:38.000000 aztools-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:51:53.198162 aztools-0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-14 11:51:38.000000 aztools-0.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-14 11:51:38.000000 aztools-0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-14 11:51:38.000000 aztools-0.2/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:51:53.198162 aztools-0.2/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-14 11:51:38.000000 aztools-0.2/docs/notebooks/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-07-14 11:51:38.000000 aztools-0.2/docs/notebooks/intro_notebook.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-14 11:51:38.000000 aztools-0.2/docs/notebooks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-14 11:51:38.000000 aztools-0.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-14 11:51:38.000000 aztools-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 11:51:53.202162 aztools-0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:51:53.198162 aztools-0.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    20895 2023-07-14 11:51:38.000000 aztools-0.2/src/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:51:53.198162 aztools-0.2/src/aztools/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-14 11:51:38.000000 aztools-0.2/src/aztools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-14 11:51:53.000000 aztools-0.2/src/aztools/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34927 2023-07-14 11:51:38.000000 aztools-0.2/src/aztools/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26716 2023-07-14 11:51:38.000000 aztools-0.2/src/aztools/lcurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19853 2023-07-14 11:51:38.000000 aztools-0.2/src/aztools/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16312 2023-07-14 11:51:38.000000 aztools-0.2/src/aztools/simlc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:51:53.198162 aztools-0.2/src/aztools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-14 11:51:53.000000 aztools-0.2/src/aztools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-14 11:51:53.000000 aztools-0.2/src/aztools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 11:51:53.000000 aztools-0.2/src/aztools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-14 11:51:53.000000 aztools-0.2/src/aztools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-14 11:51:53.000000 aztools-0.2/src/aztools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:51:53.198162 aztools-0.2/src/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-07-14 11:51:38.000000 aztools-0.2/src/scripts/ogrppha.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:51:53.198162 aztools-0.2/src/simulations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11896 2023-07-14 11:51:38.000000 aztools-0.2/src/simulations/sim__bin_psd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5040 2023-07-14 11:51:38.000000 aztools-0.2/src/simulations/sim__calculate_psd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10842 2023-07-14 11:51:38.000000 aztools-0.2/src/simulations/sim__phase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:51:53.198162 aztools-0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    20871 2023-07-14 11:51:38.000000 aztools-0.2/tests/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:51:53.202162 aztools-0.2/tests/aztools/
+-rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-07-14 11:51:38.000000 aztools-0.2/tests/aztools/test_lcurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-07-14 11:51:38.000000 aztools-0.2/tests/aztools/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-07-14 11:51:38.000000 aztools-0.2/tests/aztools/test_simlc.py
```

### Comparing `aztools-0.1.0/aztools/lcurve.py` & `aztools-0.2/src/aztools/lcurve.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,949 +1,809 @@
+"""A module for handling light curves."""
 
-import numpy as np
-import os
-
-from . import misc
+from itertools import groupby
+from typing import Union
 
+import numpy as np
 
-class LCurve(object):
-    """Light curve holder class"""
+from .misc import group_array, read_fits_lcurve
 
+__all__ = ['LCurve']
 
-    def __init__(self, t, r, re, dt=None, fexp=None):
-        """Initialize LCurve from array r and optional t, re, dt
+class LCurve:
+    """Light curve class"""
 
-        Parameters:
-            t:  an array containing the time axis
-            r:  an array containing the count rate
-            re: an array containing the measurement errors.
-            dt: time sampling. If not given, dt = min(diff(t))
-            fexp: fraction exposure array. If not given, fexp=np.ones_like(t)
+    def __init__(self,
+                 tarr: np.ndarray,
+                 rarr: np.ndarray,
+                 rerr: np.ndarray = None,
+                 **kwargs):
+        """Initialize LCurve with tarr, rarr and optional rerr, fexp
+
+        Parameters
+        ----------
+        tarr: np.ndarray
+            An array containing the time axis
+        rarr: np.ndarray
+            An array containing the count rate
+        rerr: np.ndarray
+            An array containing the measurement errors.
+            
+        Keywords
+        --------
+        deltat: float
+            Time sampling. If not given, dt = min(diff(t))
+        fexp: np.ndarray
+            fraction exposure array. If not given, fexp=np.ones_like(t)
+        
         """
 
-        # check input arrays #
-        if not (len(t) == len(r) == len(re)):
-            raise ValueError('arrays t, r, re do not match')
+        # keyword arguments
+        deltat = kwargs.get('deltat', None)
+        fexp = kwargs.get('fexp')
 
+        # check input arrays #
+        if not len(tarr) == len(rarr) == len(rerr):
+            raise ValueError('arrays tarr, rarr, rerr do not match')
 
         # time sampling #
-        if dt is None:
-            dt = np.min(np.diff(t))
-
+        if deltat is None:
+            deltat = np.min(np.diff(tarr))
 
         # fraction exposure #
         if fexp is None:
-            fexp = np.ones_like(t)
-
-
-        # is the light curve evenly sampled? #
-        iseven = np.all(np.isclose(np.diff(t), dt))
-
+            fexp = np.ones_like(tarr)
 
         # global variables #
-        self.time = np.array(t)
-        self.rate = np.array(r)
-        self.rerr = np.array(re)
+        self.time = np.array(tarr)
+        self.rate = np.array(rarr)
+        self.rerr = np.array(rerr)
         self.fexp = fexp
-        self.dt = dt
-        self.iseven = iseven
-        self.nt = len(t)
-
+        self.deltat = deltat
+        self.iseven = np.all(np.isclose(np.diff(tarr), deltat))
+        self.npoints = len(tarr)
 
 
     def __repr__(self):
-        return ('<LCurve :: nt({}) :: dt({})>').format(self.nt, self.dt)
-
+        """LCurve as a str"""
+        return f'<LCurve :: nt({self.npoints}) :: dt({self.deltat})>'
 
 
-    def make_even(self, fill=np.nan):
+    def make_even(self, fill: float = np.nan):
         """Make the light curve even in time, filling gaps with fill
 
-        Parameters:
-            fill: value to use in gaps.
-
-        Returns:
-            a new LCurve object
+        Parameters
+        ----------
+        fill: float
+            The value to use in gaps.
+
+        Return
+        ------
+        a new LCurve object
 
         """
 
         if self.iseven:
             return self
 
         # make sure time axis can be made even #
-        itime = np.round((self.time - self.time[0]) / self.dt)
-        if not np.allclose(itime - np.array(itime, np.int), 0):
+        itime = np.round((self.time - self.time[0]) / self.deltat)
+        if not np.allclose(itime - np.array(itime, np.int64), 0):
             raise ValueError('time axis cannot be made even')
 
 
-        # do work #
-        t_new = np.arange(np.int(itime[-1]) + 1) * self.dt + self.time[0]
+        # do the work #
+        t_new = np.arange(np.int64(itime[-1]) + 1) * self.deltat + self.time[0]
         idx = np.in1d(t_new, self.time)
-        r, re = [np.zeros_like(t_new) + fill for i in range(2)]
-        f = np.zeros_like(t_new)
-        r[idx]  = self.rate
-        re[idx] = self.rerr
-        f[idx]  = self.fexp
+        rarr = np.zeros_like(t_new) + fill
+        rerr = np.zeros_like(t_new) + fill
+        fexp = np.zeros_like(t_new)
+        rarr[idx] = self.rate
+        rerr[idx] = self.rerr
+        fexp[idx] = self.fexp
 
         # return a new LCurve object #
-        return LCurve(t_new, r, re, self.dt, f)
-
+        return LCurve(t_new, rarr, rerr=rerr, deltat=self.deltat, fexp=fexp)
 
 
-    def rebin(self, factor, error='norm', min_exp=0.0):
-        """Rebin the light curve to so new_dt = dt*factor
+    def rebin(self, factor: int, error: str = 'norm', min_exp: float = 0.0):
+        """Rebin the light curve to so new_deltat = deltat*factor
         
-        Parameters:
-            factor: rebinning factor. dt_new = factor * dt
-            error: error type (poiss|norm). 
-                If poiss: rerr = sqrt(rate*dt)/dt, otherwise,
-                errors are summed quadratically
-            min_exp: minimum fractional exposure to leave [0-1]
+        Parameters
+        ----------
+        factor: int
+            Rebinning factor. deltat_new = factor * deltat
+        error: str
+            Error type (poiss|norm). 
+            If poiss: rerr = sqrt(rate*dt)/dt, otherwise,
+            errors are summed quadratically
+        min_exp: float
+            Minimum fractional exposure to leave [0-1]
 
         Return:
             new binned LCurve
 
         """
 
         # check input error type #
-        if not error in ['poiss', 'norm']:
+        if error not in ['poiss', 'norm']:
             raise ValueError('error need to be poiss|norm')
 
 
         # make lc evenly sampled, so we bin arrays easily #
-        iseven = self.iseven
-        lc = self.make_even()
+        newlc = self.make_even()
 
 
         # new sampling time and length #
-        factor = np.int(factor)
-        dt_new = lc.dt * factor
-        nt_new = lc.nt//factor
-        nt_scal = nt_new * factor
+        factor = np.int64(factor)
+        dt_new = newlc.deltat * factor
+        nt_new = newlc.npoints//factor
 
 
         # pre-binning #
-        t  = lc.time[:nt_scal].reshape(nt_new, factor)
-        r  = lc.rate[:nt_scal].reshape(nt_new, factor)
-        re = lc.rerr[:nt_scal].reshape(nt_new, factor)
-        f  = lc.fexp[:nt_scal].reshape(nt_new, factor)
+        tarr = newlc.time[:nt_new*factor].reshape(nt_new, factor)
+        rarr = newlc.rate[:nt_new*factor].reshape(nt_new, factor)
+        rerr = newlc.rerr[:nt_new*factor].reshape(nt_new, factor)
+        fexp = newlc.fexp[:nt_new*factor].reshape(nt_new, factor)
 
         # rescale the rates to pre-fexp counts/bin #
-        c  = r  * (f * lc.dt)
-        ce = re * (f * lc.dt)
+        carr = rarr * (fexp * newlc.deltat)
+        cerr = rerr * (fexp * newlc.deltat)
 
 
         # do binning #
-        t  = np.mean(t, 1)
-        c  = np.nansum(c, 1)
+        tarr = np.mean(tarr, 1)
+        carr = np.nansum(carr, 1)
         if error == 'poiss':
-            ce = np.sqrt(c)
-            ce[ce==0] = np.nanmean(ce[ce!=0])
+            cerr = np.sqrt(carr)
+            cerr[cerr==0] = np.nanmean(cerr[cerr!=0])
         else:
-            ce = np.nansum(ce**2, 1)**0.5
-
-        f  = np.mean(f, 1)
-        fs = np.array(f)
-        it = (fs != 0)
-        fs[~it] = np.nan
-        r  = c /(dt_new * fs)
-        re = ce/(dt_new * fs)
-
+            cerr = np.nansum(cerr**2, 1)**0.5
+        fexp = np.mean(fexp, 1)
 
+        # calculate the rate again
+        fexps = np.array(fexp)
+        itarr = fexps != 0
+        fexps[~itarr] = np.nan
+        rarr = carr /(dt_new * fexps)
+        rerr = cerr/(dt_new * fexps)
 
-        # # leave nan values if original lc had nan (i.e it was even)
-        if iseven: 
-            it = np.ones_like(it) == 1
+        # leave nan values if original lc had nan (i.e it was even)
+        if self.iseven:
+            itarr = np.ones_like(itarr) == 1
 
-        # # filter on fracexp if needed #
+        # filter on fracexp if needed #
         if min_exp > 0:
-            it[f < min_exp] = False
+            itarr[fexp < min_exp] = False
 
         # return a new LCurve object #
-        return LCurve(t[it], r[it], re[it], dt_new, f[it])
-
+        return LCurve(tarr[itarr], rarr[itarr],
+                      rerr=rerr[itarr], deltat=dt_new, fexp=fexp[itarr])
 
 
-    def interp_small_gaps(self, maxgap=None, noise='poiss', seed=None):
+    def interp_small_gaps(self,
+                          maxgap: int = None,
+                          noise: str = 'poiss',
+                          seed: int = None):
         """Interpolate small gaps in the lightcurve if the gap
             is <maxgap; applying noise if requested
 
-        Parameters:
-            maxgap: the maximum length of a gap to be interpolated
-            noise: poiss|norm|None
-            seed: random seen if noise is requested
+        Parameters
+        ----------
+        maxgap: int
+            The maximum length of a gap to be interpolated.
+        noise: str:
+            poiss|norm|None
+        seed: int
+            Random seed if noise is requested
 
         """
-        from itertools import groupby
 
         if not self.iseven:
             raise ValueError('lc is not even; make even first')
 
         # random seed if noise is needed #
         if noise is not None:
             np.random.seed(seed)
 
 
         # find gap lengths in the data #
-        maxn = self.nt if maxgap is None else maxgap
-        iarr = [list(i[1]) for i in groupby(np.arange(self.nt), 
-                    lambda ix:np.isfinite(self.rate[ix]))]
+        maxn = self.npoints if maxgap is None else maxgap
+        iarr = [list(igrp[1]) for igrp in
+                groupby(
+                    np.arange(self.npoints),
+                    lambda ixarr:np.isfinite(self.rate[ixarr])
+                )
+               ]
         # indices of non-finite segments #
         iinf = iarr[(1 if np.isfinite(iarr[0][0]) else 0)::2]
         # length of each non-finite segment #
         iinf = [i for i in iinf if len(i)<=maxn]
         iinf = [j for i in iinf for j in i]
-        
-
 
 
         # interpolate all values then keep only those with length<maxn #
         idx = np.isfinite(self.rate)
-        y  = np.interp(self.time, self.time[idx], self.rate[idx])
-        ye = np.zeros_like(y)
-        me = np.mean(self.rerr[idx])
+        yarr = np.interp(self.time, self.time[idx], self.rate[idx])
+        yerr = np.zeros_like(yarr)
+        mean = np.mean(self.rerr[idx])
         if noise is None:
             # no noise requested; the value is not altered from the interp
             # while the error is the average of all errors
-            ye += me
+            yerr += mean
 
         elif noise == 'poiss':
             # apply noise to counts/bin then convert back to counts/s
-            yp = np.random.poisson(y*self.dt)
-            y  = yp / self.dt
-            ye = np.sqrt(yp) / self.dt
+            ypoiss = np.random.poisson(yarr*self.deltat)
+            yarr = ypoiss / self.deltat
+            yerr = np.sqrt(ypoiss) / self.deltat
             # reset points where y=0 (hence ye=0)
-            ye[yp == 0] = me
-        
-        elif noise == 'norm':
-            y  += np.random.randn(len(y)) * me
-            ye += me
-
-        # now update fill in the gaps with length<maxn #
-        self.rate[iinf] = y[iinf]
-        self.rerr[iinf] = ye[iinf]
-
-    
-    @staticmethod
-    def sync(lc_list, tbase=None):
-        """Synchronize a list of arrays or LCurve's
-        lc_list: a list of arrays or a list of LCurve objects.
-            if arrays, the shape is (nlc, 3 (or 4 for fexp), nt).
-            The 3 is for (time, rate, rerr)
-        tbase: time array to use for reference. 
-            If not given, use the intersection of all t
-        """
-        if not isinstance(lc_list, (list, np.ndarray)):
-            raise ValueError('lc_list must be a list')
-        if isinstance(lc_list[0], LCurve):
-            data = [np.array([l.time, l.rate, l.rerr]) for l in lc_list]
-        else:
-            # consider if fexp is not given
-            data = [np.array(l) for l in lc_list]
-        
-        if tbase is None:
-            tbase = data[0][0]
-            for d in data[1:]:
-                tbase = tbase[np.in1d(tbase, d[0])]
-        
-        data = [d[:, np.in1d(d[0], tbase)] for d in data]
-        return data
-
-
-    @staticmethod
-    def read_fits_file(fits_file, **kwargs):
-        """Read LCurve from fits file
-
-        Parameters:
-            fits_file: name of the fits file
-
-        Keywords:
-            min_exp: minimum fractional exposure to allow. Default 0.0 for all
-            rate_tbl: name or number of hdu that contains lc data. Default: RATE
-            rate_col: name or number of rate column. Default: RATE
-            time_col: name or number of time column. Default: TIME
-            rerr_col: name or number of rerr column. Default: ERROR
-            fexp_col: name or number of the fracexp column. Default: FRACEXP
-            gti_table: name or number of gti extension hdu. Default: GTI 
-            dt_key: name of dt keyword in header. Default: TIMEDEL
-            gti_skip: how many seconds to skip at the gti boundaries. Default: 0
-            verbose. 
-
-
-        Returns:
-            ldata (shape: 4,nt containing, time, rate, rerr, fexp), dt
-        """
-
-        # pyfits #
-        import astropy.io.fits as pyfits
-
-
-        # default parameters #
-        min_exp  = kwargs.get('min_exp', 0.)
-        rate_tbl = kwargs.get('rate_tbl', 'RATE')
-        rate_col = kwargs.get('rate_col', 'RATE')
-        time_col = kwargs.get('time_col', 'TIME')
-        rerr_col = kwargs.get('rerr_col', 'ERROR')
-        fexp_col = kwargs.get('fexp_col', 'FRACEXP')
-        gti_tbl  = kwargs.get('gti_tbl' , 'GTI')
-        dt_key   = kwargs.get('dt_key', 'TIMEDEL')
-        #dt = pyfits.open(fits_file)[1].header['timedel']
-        gti_skip = kwargs.get('gti_skip', 0.0)
-        verbose  = kwargs.get('verbose', False)
-
-
-        # does file exist? #
-        if not os.path.exists(fits_file):
-            raise ValueError('file {} does not exist'.format(fits_file))
-
-        # read file #
-        with pyfits.open(fits_file) as fs:
-            
-            # lc data #
-            data = fs[rate_tbl].data
-            ldata = np.array([  data.field(time_col),
-                                data.field(rate_col),
-                                data.field(rerr_col)], dtype=np.double)
-
-            
-            # start time and time sampling #
-            t0 = (fs[rate_tbl].header['TSTART'] if 'TSTART' in 
-                        fs[rate_tbl].header.keys() else 0.0)
-            dt = (fs[rate_tbl].header[dt_key] if dt_key in 
-                        fs[rate_tbl].header.keys() else None)
-            if not dt is None: t0 += dt/2
-
-            # if the time-axis offset, correct it #
-            if t0/ldata[0, 1] > 1e5:
-                ldata[0] += t0
-
-
-            # gti #
-            try:
-                ghdu = fs[gti_tbl]
-                lgti  = np.array([ghdu.data.field(0), ghdu.data.field(1)],
-                                dtype=np.double)
-            except KeyError:
-                if verbose:
-                    print('No GTI found in {}'.format(fits_file))
-                lgti = np.array([[ldata[0, 0]], [ldata[0, -1]]])
-
-
-            # fractional exposure #
-            try:
-                lfracexp = data.field(fexp_col)
-            except KeyError:
-                if verbose:
-                    print('cannot read fracexp_col in {}'.format(fits_file))
-                lfracexp = np.ones_like(ldata[0])
-
-
-            # apply gti #
-            igti  = ldata[0] < 0
-            for gstart, gstop in lgti.T:
-                igti = igti | ( (ldata[0] >= (gstart+gti_skip)) & 
-                                (ldata[0] <= (gstop -gti_skip)) )
-            igood = igti & (lfracexp >= min_exp) & (np.isfinite(ldata[0]))
-            ldata = np.vstack([ldata, lfracexp])
-            ldata = ldata[:, igood]
-
-        return ldata, dt
-
-
-    @staticmethod
-    def read_pn_lcurve(fits_file, **kwargs):
-        """Read pn lcurve fits_file created with xmmlc_lc.
-            This sets values relevant to PN and calls read_fits_file
-
-        Parameters:
-            fits_file: name of the files file
-
-        Keywords:
-            See @LCurve.read_fits_file
-
-
-        Returns:
-            LCurve object
-        """
-
-        # set values relevant to XMM-PN files #
-        kwargs.setdefault('min_exp' , 0.7)
-        kwargs.setdefault('gti_tbl' , 2)
-    
-        data, dt = LCurve.read_fits_file(fits_file, **kwargs)
-        return LCurve(data[0], data[1], data[2], dt, data[3])        
-
-
-    @staticmethod
-    def read_pca_lcurve(fits_file, **kwargs):
-        """Read pca lcurve fits_file.
-            This sets values relevant to PCA and calls read_fits_file
-
-        Parameters:
-            fits_file: name of the files file
-
-        Keywords:
-            See @LCurve.read_fits_file
-
-
-        Returns:
-            LCurve object
-        """
-
-        # set values relevant to XMM-PN files #
-        kwargs.setdefault('min_exp' , 0.99)
-        kwargs.setdefault('gti_tbl' , 'STDGTI')
-    
-        data, dt = LCurve.read_fits_file(fits_file, **kwargs)
-        return LCurve(data[0], data[1], data[2], dt, data[3])  
-
-
-    @staticmethod
-    def read_nu_lcurve(fits_file, **kwargs):
-        """Read nustar lcurve fits_file.
-            This sets values relevant to NUSTAR and calls read_fits_file
-
-        Parameters:
-            fits_file: name of the files file
-
-        Keywords:
-            See @LCurve.read_fits_file
-
-
-        Returns:
-            LCurve object
-        """
-
-        # set values relevant to XMM-PN files #
-        kwargs.setdefault('min_exp' , 0.1)
-        kwargs.setdefault('gti_tbl' , 'GTI')
-        kwargs.setdefault('gti_skip', 3.0)
-    
-        data, dt = LCurve.read_fits_file(fits_file, **kwargs)
-        return LCurve(data[0], data[1], data[2], dt, data[3])  
-
-    
-    @staticmethod
-    def read_xis_lcurve(fits_file, **kwargs):
-        """Read suzaku xis lcurve fits_file.
-            This sets values relevant to NUSTAR and calls read_fits_file
-
-        Parameters:
-            fits_file: name of the files file
-
-        Keywords:
-            See @LCurve.read_fits_file
-
-
-        Returns:
-            LCurve object
-        """
-
-        # set values relevant to XIS files #
-        kwargs.setdefault('min_exp' , 0.1)
-        kwargs.setdefault('gti_tbl' , 'GTI')
-    
-        data, dt = LCurve.read_fits_file(fits_file, **kwargs)
-        return LCurve(data[0], data[1], data[2], dt, data[3])  
-
-    @staticmethod
-    def read_ni_lcurve(fits_file, **kwargs):
-        """Read nicer lcurve fits_file.
-            This sets values relevant to NICER and calls read_fits_file
-
-        Parameters:
-            fits_file: name of the files file
-
-        Keywords:
-            See @LCurve.read_fits_file
+            yerr[ypoiss == 0] = mean
 
+        elif noise == 'norm':
+            yarr += np.random.randn(len(yarr)) * mean
+            yerr += mean
 
-        Returns:
-            LCurve object
-        """
-
-        # set values relevant to NICER files #
-        kwargs.setdefault('min_exp' , 0.99)
-        kwargs.setdefault('gti_tbl' , 'GTI')
-        #kwargs.setdefault('gti_skip', 3.0)
-    
-        data, dt = LCurve.read_fits_file(fits_file, **kwargs)
-        return LCurve(data[0], data[1], data[2], dt, data[3]) 
+        # now fill in the gaps with length<maxn #
+        self.rate[iinf] = yarr[iinf]
+        self.rerr[iinf] = yerr[iinf]
 
 
     @staticmethod
-    def calculate_psd(rate, dt, norm='var', **kwargs):
+    def calculate_psd(rate: Union[list, np.ndarray],
+                      deltat: float,
+                      norm: str = 'var',
+                      **kwargs):
         """Calculate raw psd from a list of light curves.
-        
-        Parameters:
-            rate: array or list of arrays of lcurve rates
-            dt: time bin width of the light curve
-            norm: psd normalization: var|rms|leahy
 
-        Keywords:
-            rerr: array or list of errors on rate. If not give,
-                assume, poisson noise.
-            bgd: array or list of background rates. In this case,
-                rate above is assumed background subtracted.
-            taper: apply Hanning tapering before calculating the psd
-                see p388 Bendat & Piersol; the psd need to be multiplied
-                by 8/3 to componsate for the reduced variance.
-        
-        Return:
-            freq, rpsd, nois. 
+        Parameters
+        ----------
+        rate: np.ndarray or a list of np.ndarray
+            An array or a list of arrays of lcurve rates
+        deltat: float
+            Time bin width of the light curve(s).
+        norm: str
+            Psd normalization: var|rms|leahy
+
+        Keywords
+        --------
+        rerr: np.ndarray or a list of np.ndarray
+            The measurement error arrays that corresponds to rate.
+            If not given, assume, poisson noise.
+        bgd: np.ndarray or a list of np.ndarray.
+            The background rate arrays that corresponds to source rate. 
+            In this case, rate above is assumed background subtracted.
+        taper: bool
+            Apply Hanning tapering before calculating the psd
+            see p388 Bendat & Piersol; the psd needs to be multiplied
+            by 8/3 to componsate for the reduced variance.
+
+        Return
+        ------
+        freq, rpsd, nois. 
+
         """
 
         # check input #
         if not isinstance(rate[0], (np.ndarray, list)):
             rate = [rate]
 
-        if not norm in ['var', 'rms', 'leahy']:
+        if norm not in ['var', 'rms', 'leahy']:
             raise ValueError('norm need to be var|rms|leahy')
 
         # rerr and bgd; for estimating noise level #
         rerr = kwargs.get('rerr', None)
         bgd  = kwargs.get('bgd', 0.0)
         if not isinstance(bgd, (np.ndarray, list)):
-            bgd = [bgd for r in rate]
+            bgd = [bgd for rat in rate]
         if rerr is None:
             # err is sqrt of number of counts/bin
-            rerr = [np.sqrt((r+b)/dt) for r,b in zip(rate, bgd)]
+            rerr = [np.sqrt((rat+bak)/deltat) for rat,bak in zip(rate, bgd)]
 
 
         # tapering ? #
         taper = kwargs.get('taper', False)
         if taper:
-            rate = [(r-r.mean()) * np.hanning(len(r)) + r.mean() for r in rate]
+            rate = [(rat-rat.mean()) * np.hanning(len(rat)) + rat.mean()
+                    for rat in rate]
 
 
         # fft; remove the 0-freq and the nyquist #
-        freq = [np.fft.rfftfreq(len(r), dt)[1:-1] for r in rate]
-        rfft = [np.fft.rfft(r)[1:-1] for r in rate]
-        mean = [np.mean(r) for r in rate]
+        freq = [np.fft.rfftfreq(len(rat), deltat)[1:-1] for rat in rate]
+        rfft = [np.fft.rfft(rat)[1:-1] for rat in rate]
+        mean = [np.mean(rat) for rat in rate]
 
         # normalize psd #
-        expo = {'var':0, 'leahy':1, 'rms':2} 
-        rpsd = [(2.*dt / (len(r) * mu**expo[norm])) * np.abs(rf)**2
-                    for r,rf,mu in zip(rate, rfft, mean)]
+        expo = {'var':0, 'leahy':1, 'rms':2}
+        rpsd = [(2.*deltat / (len(rat) * mu_**expo[norm])) * np.abs(ratf)**2
+                    for rat,ratf,mu_ in zip(rate, rfft, mean)]
 
         # renormalize rpsd if tapering has been applied #
         if taper:
-            rpsd = [r * 8/3 for r in rpsd]
+            rpsd = [rat * 8/3 for rat in rpsd]
 
         ## ------ noise level ------- ##
         # noise level is: 2*(mu+bgd)/(mu^2) for RMS normalization; eqn A2, Vaughan+03
         # This the special case of poisson noise light curves.
         # Generally: noise = <e^2>/(mu^2 fq_nyq)
         # where <e^2> is the averaged squared error in the measurements
         # which for poisson case: e = sqrt((mu+bgd)*dt)/dt = sqrt((mu+bgd)/dt)
         # --> <e^2> = (mu+bgd)/dt
         # fq_nyq: is the Nyquist frequency: fq_nyq = 1/(2*dt)
         # ==> for poisson case: noise = 2*(mu+bgd)/mu^2
         # For other normalization, we need to renormalize accordingly
         ## -------------------------- ##
-        fnyq = 0.5/dt
-        nois = [ff*0+np.mean(re**2)/(fnyq*mu**expo[norm]) 
-                    for ff,re,mu in zip(freq, rerr, mean)]
-
+        fnyq = 0.5/deltat
+        nois = [frq*0+np.mean(ree**2)/(fnyq*mu_**expo[norm])
+                    for frq,ree,mu_ in zip(freq, rerr, mean)]
 
         # flattern lists #
-        _c = np.concatenate
-        freq = _c(freq)
+        concat = np.concatenate
+        freq = concat(freq)
         isort = np.argsort(freq)
         freq = freq[isort]
-        rpsd = _c(rpsd)[isort]
-        nois = _c(nois)[isort]
+        rpsd = concat(rpsd)[isort]
+        nois = concat(nois)[isort]
 
         return freq, rpsd, nois
 
 
     @staticmethod
-    def bin_psd(freq, rpsd, fqbin, noise=None, logavg=True):
+    def bin_psd(freq: np.ndarray,
+                rpsd: np.ndarray,
+                fqbin: dict,
+                noise: bool = None,
+                logavg: bool = True):
         """Bin power spectrum.
 
-        Parameters:
-            freq: array of frequencies
-            rpsd: array of raw powers
-            fqbin: binning dict to be passed to @misc.group_array
-                to bin the frequency axis
-            noise: array of noise.
-            logavg: do averaging in log-space, and correct for
-                bias. Otherwise it is simple averaging
-
-        Returns:
-            fq, psd, psde, desc; with desc having some useful info
+        Parameters
+        ----------
+        freq: np.ndarray
+            Array of raw frequencies.
+        rpsd: np.ndarray
+            Array of raw powers.
+        fqbin: dict
+            Binning dict to be passed to @misc.group_array
+            to bin the frequency axis.
+        noise: bool
+            Array of noise values or None.
+        logavg: bool
+            Do averaging in log-space, and correct for
+            bias. Otherwise it is linear averaging.
+
+        Return
+        ------
+            freq, psd, psde, desc::dict having some useful info
 
         """
 
-
         # ensure the arrays are compatible #
         if len(freq) != len(rpsd):
             raise ValueError('freq and rpsd are not compatible')
 
-        if noise is None: noise = np.zeros_like(freq) + 1e-10
+        if noise is None:
+            noise = np.zeros_like(freq) + 1e-10
 
         # group the freq array #
-        nfq = len(freq)
-        idx  = misc.group_array(freq, do_unique=True, **fqbin)
-        fqm  = [len(i) for i in idx]
-        fqL = [freq[i].min() for i in idx] + [freq[idx[-1].max()]]
+        idx = group_array(freq, do_unique=True, **fqbin)
+        fqm = [len(jdx) for jdx in idx]
+        fql = [freq[i].min() for i in idx] + [freq[idx[-1].max()]]
 
 
         # do the actual binning #
-        # the noise is logavg if needed, without bias correction
+        # the noise in the logavg case is without bias correction
         if logavg:
-            f  = [10**np.mean(np.log10(freq[i])) for i in idx]
-            p  = [10**np.mean(np.log10(rpsd[i])) for i in idx]
-            n  = [10**np.mean(np.log10(noise[i])) for i in idx]
-            pe = [np.log(10)*p[i]*(0.310/fqm[i])**0.5 for i in range(len(p))]
+            frq = [10**np.mean(np.log10(freq[i])) for i in idx]
+            psd = [10**np.mean(np.log10(rpsd[i])) for i in idx]
+            nse = [10**np.mean(np.log10(noise[i])) for i in idx]
+            per = [np.log(10)*psd[ipp]*(0.310/fqm[ipp])**0.5
+                   for ipp in range(len(psd))]
         else:
-            f  = [np.mean(freq[i]) for i in idx]
-            p  = [np.mean(rpsd[i]) for i in idx]
-            n  = [np.mean(noise[i]) for i in idx]
-            pe = [p[i]*(1./fqm[i])**0.5 for i in range(len(p))]
+            frq = [np.mean(freq[i]) for i in idx]
+            psd = [np.mean(rpsd[i]) for i in idx]
+            nse = [np.mean(noise[i]) for i in idx]
+            per = [psd[ipp]*(1./fqm[ipp])**0.5
+                   for ipp in range(len(psd))]
 
-        fq, psd, psde, n = np.array(f), np.array(p), np.array(pe), np.array(n)
+        frq, psd, psde, nse = np.array(frq), np.array(psd), np.array(per), np.array(nse)
 
         # bias correction #
         #####################################
         # From the simulations in test_lcurve.py:
         # 1- Whenever logavg=True is used, bias correciton needs
         #    to be applied. Logavg=True does better, most of the
         #    times, particularly when averaging neighboring frequencies
         # bias function: bias_f(2) ~ 0.253 in Papadakis93
         # bias_f = lambda k: -sp.digamma(k/2.)/np.log(10)
         #####################################
-        import scipy.special as sp
-        bias_f = lambda k: -sp.digamma(k/2.)/np.log(10)
-        bias = np.zeros_like(psd) + bias_f(2)
-        if logavg: psd *= 10**bias
-
-        # return #    
-        desc = {'fqL': fqL, 'fqm':fqm, 'noise':n, 'bias':bias}
-        return fq, psd, psde, desc
+        bias = np.zeros_like(psd) + 0.253
+        if logavg:
+            psd *= 10**bias
+
+        # return #
+        desc = {'fql': fql, 'fqm':fqm, 'noise':nse, 'bias':bias}
+        return frq, psd, psde, desc
 
 
     @staticmethod
-    def calculate_lag(rate, Rate, dt, fqbin=None, **kwargs):
+    def calculate_lag(xarr: Union[np.ndarray, list],
+                      yarr: Union[np.ndarray, list],
+                      deltat: float,
+                      fqbin: dict = None,
+                      **kwargs):
         """Calculate and bin lags from two lists of light curves.
         
-        Parameters:
-            rate: array or list of arrays of lcurve rates
-            Rate: array or list of arrays of Reference lcurve rates
-            dt: time bin width of the light curve
-            fqbin: binning dict to be passed to @misc.group_array
-                to bin the frequency axis. If None, return raw lag
-
-        Keywords:
-            rerr: array or list of errors on rate. If not give,
-                assume, poisson noise.
-            bgd: array or list of background rates. In this case,
-                rate above is assumed background subtracted.
-            Rerr: array or list of errors on Rate. If not give,
-                assume, poisson noise.
-            Bgd: array or list of background rates for the reference. 
-                In this case, Rate above is assumed background subtracted.
-            phase: return phase lag instead of time lag
-            taper: apply Hanning tapering before calculating the fft
-                see p388 Bendat & Piersol; the fft need to be multiplied
-                by sqrt(8/3) to componsate for the reduced variance. Default: False
-            norm: how to normalize the fft during the calculations. None|rms|leahy|var.
-                Default is None, so the calculations is done with raw numpy fft
-
-                
-        
-        Return:
-            freq, lag, lage, desc;
-            desc = {'fqm', 'fqL', 'limit', 'Limit'}
+        Parameters
+        ----------
+        xarr: np.ndarray or list
+            Array or list of arrays of light curve rates.
+        yarr: np.ndarray or list
+            Array or list of arrays of reference light curve rates.
+        deltat: float
+            Time bin width of the light curve.
+        fqbin: dict
+            Binning dict to be passed to @misc.group_array
+            to bin the frequency axis. If None, return raw lag
+
+        Keywords
+        --------
+        xerr: np.ndarray or a list of np.ndarray
+            The measurement error arrays that corresponds to rate.
+            If not given, assume, poisson noise.
+        xbgd: np.ndarray or a list of np.ndarray.
+            The background rate arrays that corresponds to source rate. 
+            In this case, rate above is assumed background subtracted.
+        yerr: np.ndarray or a list of np.ndarray
+            The measurement error arrays that corresponds to yarr.
+            If not given, assume, poisson noise.
+        ybgd: np.ndarray or a list of np.ndarray.
+            The background rate arrays that corresponds to ref_rate. 
+            In this case, yarr above is assumed background subtracted.
+        phase: bool
+            return phase lag instead of time lag
+        taper: bool
+            Apply Hanning tapering before calculating the fft
+            see p388 Bendat & Piersol; the fft need to be multiplied
+            by sqrt(8/3) to componsate for the reduced variance. Default: False
+        norm: str
+            How to normalize the fft during the calculations. None|rms|leahy|var.
+            Default is None, so the calculations is done with raw numpy fft
+
+
+        Return
+        ------
+        freq, lag, lage, extra
+        extra = {'fqm', 'fql', 'xlimit', 'ylimit' ..}
         """
 
         phase = kwargs.get('phase', False)
 
 
         # check input #
-        if not isinstance(rate[0], (np.ndarray, list)): rate = [rate]
-        if not isinstance(Rate[0], (np.ndarray, list)): Rate = [Rate]
+        if not isinstance(xarr[0], (np.ndarray, list)):
+            xarr = [xarr]
+        if not isinstance(yarr[0], (np.ndarray, list)):
+            yarr = [yarr]
 
         # check that lc and reference are compatible #
-        for r1,r2 in zip(rate, Rate):
-            if len(r1) != len(r2):
-                raise ValueError('rate and Rate are incompatible')
-
-
-        # rerr and bgd; for estimating noise level #
-        bgd  = kwargs.get('bgd', 0.0)
-        Bgd  = kwargs.get('Bgd', 0.0)
-        if not isinstance(bgd, (np.ndarray, list)):
-            bgd = [bgd for r in rate]
-        if not isinstance(Bgd, (np.ndarray, list)):
-            Bgd = [Bgd for r in Rate]
-
-        rerr = kwargs.get('rerr', None)
-        Rerr = kwargs.get('Rerr', None)
-        if rerr is None:
-            # TODO: this is not always correct!
-            rerr = [np.sqrt((r+b)/dt) for r,b in zip(rate, bgd)]
-        if Rerr is None:
-            # TODO: this is not always correct!
-            Rerr = [np.sqrt((r+b)/dt) for r,b in zip(Rate, Bgd)]
-
-        # make sure error arrays are also ready 
-        if not isinstance(rerr[0], (np.ndarray, list)): rerr = [rerr]
-        if not isinstance(Rerr[0], (np.ndarray, list)): Rerr = [Rerr]
+        for xar,yar in zip(xarr, yarr):
+            if len(xar) != len(yar):
+                raise ValueError('xarr and yarr are incompatible')
+
+
+        # error and background values for estimating noise level #
+        xbgd = kwargs.get('xbgd', 0.0)
+        ybgd = kwargs.get('ybgd', 0.0)
+        if not isinstance(xbgd, (np.ndarray, list)):
+            xbgd = [xbgd for _ in xarr]
+        if not isinstance(ybgd, (np.ndarray, list)):
+            ybgd = [ybgd for _ in yarr]
+
+        xerr = kwargs.get('xerr', None)
+        yerr = kwargs.get('yerr', None)
+        if xerr is None:
+            # this is not always correct!
+            xerr = [np.sqrt((xar+xbg)/deltat) for xar,xbg in zip(xarr, xbgd)]
+        if yerr is None:
+            # this is not always correct!
+            yerr = [np.sqrt((yar+ybg)/deltat) for yar,ybg in zip(yarr, ybgd)]
+
+        if not isinstance(xerr[0], (np.ndarray, list)):
+            xerr = [xerr]
+        if not isinstance(yerr[0], (np.ndarray, list)):
+            yerr = [yerr]
 
 
         # tapering ? #
         taper = kwargs.get('taper', True)
         taper_factor = 1.0
         if taper:
-            rate = [(r-r.mean()) * np.hanning(len(r)) + r.mean() for r in rate]
-            Rate = [(r-r.mean()) * np.hanning(len(r)) + r.mean() for r in Rate]
+            xarr = [(arr-arr.mean()) * np.hanning(len(arr)) + arr.mean() for arr in xarr]
+            yarr = [(arr-arr.mean()) * np.hanning(len(arr)) + arr.mean() for arr in yarr]
             taper_factor = np.sqrt(8/3)
 
 
         # normalization ? #
         norm = kwargs.get('norm', None)
         if not norm in [None, 'rms', 'leahy', 'var']:
             raise ValueError('Unknown norm value. It should be None|rms|leahy|var')
         expo = {'var':0, 'leahy':1, 'rms':2}
-        if norm is None:
-            normf = lambda r: 1.0
-        else:
-            normf = lambda r: (2.*dt / (len(r) * np.mean(r)**expo[norm]))**0.5
+        def normf(arr):
+            return 1.0 if norm is None else (
+                2.*deltat / (len(arr) * np.mean(arr)**expo[norm]))**0.5
 
-        
-        # fft; remove the 0-freq and the nyquist #
-        rfft = [np.fft.rfft(r)[1:-1]*taper_factor*normf(r) for r in rate]
-        Rfft = [np.fft.rfft(r)[1:-1]*taper_factor*normf(r) for r in Rate]
-        freq = [np.fft.rfftfreq(len(r), dt)[1:-1] for r in rate]
-        crss = [R*np.conj(r) for r,R in zip(rfft, Rfft)]
-        rpsd = [np.abs(r)**2 for r in rfft]
-        Rpsd = [np.abs(r)**2 for r in Rfft]
-        
 
+        # fft; remove the 0-freq and the nyquist #
         # noise level in psd. See comments in @calculate_psd #
         # noise level is: <e^2>/(mu^2 fq_nyq) for rms norm; then renorm accordingly
-        fnyq = 0.5/dt
-        nois = [ff*0+(np.mean(re**2)*len(re)*normf(r)**2)/(fnyq*2*dt) 
-                    for ff,re,r in zip(freq, rerr, rate)]
-        Nois = [ff*0+(np.mean(re**2)*len(re)*normf(r)**2)/(fnyq*2*dt) 
-                    for ff,re,r in zip(freq, Rerr, Rate)]
+        fnyq = 0.5/deltat
+        freq = [np.fft.rfftfreq(len(_), deltat)[1:-1] for _ in xarr]
+
+        xfft = [np.fft.rfft(_)[1:-1]*taper_factor*normf(_) for _ in xarr]
+        xpsd = [np.abs(_)**2 for _ in xfft]
+        xnse = [_[0]*0+(np.mean(_[1]**2)*len(_[1])*normf(_[2])**2)/(fnyq*2*deltat)
+                    for _ in zip(freq, xerr, xarr)]
+
+        yfft = [np.fft.rfft(_)[1:-1]*taper_factor*normf(_) for _ in yarr]
+        ypsd = [np.abs(_)**2 for _ in yfft]
+        ynse = [_[0]*0+(np.mean(_[1]**2)*len(_[1])*normf(_[2])**2)/(fnyq*2*deltat)
+                    for _ in zip(freq, yerr, yarr)]
+
+        crss  = [_[1]*np.conj(_[0]) for _ in zip(xfft, yfft)]
 
 
         # flattern lists #
-        _c = np.concatenate
-        freq = _c(freq)
+        concat = np.concatenate
+        freq = concat(freq)
         isort = np.argsort(freq)
         freq = freq[isort]
-        crss = _c(crss)[isort]
-        rpsd = _c(rpsd)[isort]
-        Rpsd = _c(Rpsd)[isort]
-        nois = _c(nois)[isort]
-        Nois = _c(Nois)[isort]
+        crss = concat(crss)[isort]
+        xpsd = concat(xpsd)[isort]
+        ypsd = concat(ypsd)[isort]
+        xnse = concat(xnse)[isort]
+        ynse = concat(ynse)[isort]
+
 
+        # save raw values
+        raw = {'freq': freq, 'crss':crss,
+               'xfft': xfft, 'xpsd': xpsd, 'xnse': xnse,
+               'yftt': yfft, 'ypsd': ypsd, 'ynse': ynse}
 
         # do we need just raw lags? #
         if fqbin is None:
             lag = np.angle(crss) / (1. if phase else 2*np.pi*freq)
-            return freq, lag
+            return freq, lag, raw
+
 
-        
         # bin the lag #
-        _a = np.array
-        idx = misc.group_array(freq, do_unique=True, **fqbin)
-        fqm = _a([len(i) for i in idx])
-        fqL = _a([freq[i].min() for i in idx] + [freq[idx[-1].max()]])
+        idx = group_array(freq, do_unique=True, **fqbin)
+        fqm = np.array([len(jdx) for jdx in idx])
+        fql = np.array([freq[i].min() for i in idx] + [freq[idx[-1].max()]])
+
+
+        def mean(arr):
+            return np.array([np.mean(arr[jdx]) for jdx in idx])
+        def lmean(arr):
+            return np.array([10**(np.mean(np.log10(arr[jdx]))) for jdx in idx])
+
+        freq = lmean(freq)
+        xpsd = mean(xpsd)
+        ypsd = mean(ypsd)
+        xnse = mean(xnse)
+        ynse = mean(ynse)
+        crss = mean(crss)
 
 
-        meanf  = lambda a: np.mean(a)
-        lmeanf = lambda a: 10**(np.mean(np.log10(a)))
-
-        f  = _a([lmeanf(freq[i]) for i in idx])
-        p  = _a([meanf(rpsd[i])  for i in idx])
-        P  = _a([meanf(Rpsd[i])  for i in idx])
-        n  = _a([meanf(nois[i])  for i in idx])
-        N  = _a([meanf(Nois[i])  for i in idx])
-        c  = _a([meanf(crss[i])  for i in idx])
-            
-
         # phase lag and its error #
         # g2 is caluclated without noise subtraciton
         # see paragraph after eq. 17 in Nowak+99
-        # see eq. 11, 12 in Uttley+14. Nowak (and Uttley too) clearly 
+        # see eq. 11, 12 in Uttley+14. Nowak (and Uttley too) clearly
         # states that the noise shouldn't be subtracted)
-        lag = np.angle(c)
-        n2  = ((p - n)*N + (P - N)*n + n*N) / fqm
-        g2  = (np.abs(c)**2) / (p * P)
+        lag = np.angle(crss)
+        nn2 = ((xpsd - xnse)*ynse + (ypsd - ynse)*xnse + xnse*ynse) / fqm
+        gg2 = (np.abs(crss)**2) / (xpsd * ypsd)
 
         # mask out points where coherence is undefined #
-        g2  = np.clip(g2, 1e-5, 1.0)
-        lag_e = np.clip(np.sqrt((1 - g2) / (2*g2*fqm)), 0, np.pi)
+        gg2 = np.clip(gg2, 1e-5, 1.0)
+        lag_e = np.clip(np.sqrt((1 - gg2) / (2*gg2*fqm)), 0, np.pi)
 
 
         # coherence gamma_2 #
         # here we subtract the noise; see eq. 8
         # in Vaughan+97 and related definitions
-        coh   = (np.abs(c)**2 - n2) / ((p-n) * (P-N))
+        coh   = (np.abs(crss)**2 - nn2) / ((xpsd-xnse) * (ypsd-ynse))
         coh = np.clip(coh, 1e-5, 1-1e-5)
         dcoh  = (2/fqm)**0.5 * (1 - coh)/np.sqrt(coh)
-        coh_e = coh * (fqm**-0.5) * ((2*n2*n2*fqm)/(np.abs(c)**2 - n2)**2 + 
-                (n**2/(p-n)**2) + (N**2/(P-N)**2) + (fqm*dcoh/coh**2))**0.5
+        coh_e = coh * (fqm**-0.5) * ((2*nn2*nn2*fqm)/(np.abs(crss)**2 - nn2)**2 +
+                (xnse**2/(xpsd-xnse)**2) + (ynse**2/(ypsd-ynse)**2) + (fqm*dcoh/coh**2))**0.5
+        coh_e[(coh - coh_e) < 0] = coh[(coh - coh_e) < 0]
+
 
         # rms spectrum from psd; error from eq. 14 in Uttley+14 #
         # the rms here is in absolute not fractional units
-        dfq  = fqL[1:]-fqL[:-1]
-        mu   = np.mean([np.mean(r) for r in rate])
-        Mu   = np.mean([np.mean(r) for r in Rate])
-        rms  = mu * (dfq * np.abs(p - n))**0.5
-        sigx2  = rms**2
-        sigxn2 = dfq * n * mu**2 
+        dfq = fql[1:]-fql[:-1]
+        xmu = np.mean([np.mean(_) for _ in xarr])
+        ymu = np.mean([np.mean(_) for _ in yarr])
+        rms = xmu * (dfq * np.abs(xpsd - xnse))**0.5
+        sigx2 = rms**2
+        sigxn2 = dfq * xnse * xmu**2
         rmse = ((2*sigx2*sigxn2 + sigxn2**2) / (2*fqm*sigx2) ) **0.5
-        ibad = p<n
+        ibad = xpsd<xnse
         rms[ibad] = 0.0
         rmse[ibad] = np.max(np.concatenate((rms, rmse)))
 
 
         # covariance: eq. 13, 15 in Uttley+14 #
         # again in absolute not fractional units #
-        cov  = ( (np.abs(c)**2 - n2) * mu * mu * dfq / (P-N) )
-        ibad = (cov < 0) | (P<=N)
+        cov  = ( (np.abs(crss)**2 - nn2) * xmu * xmu * dfq / (ypsd-ynse) )
+        ibad = (cov < 0) | (ypsd<=ynse)
         cov  = np.abs(cov)**0.5
-        sigy2 = dfq * np.abs(P-N) * Mu**2
-        sigyn2 = dfq * N * Mu**2
+        sigy2 = dfq * np.abs(ypsd-ynse) * ymu**2
+        sigyn2 = dfq * ynse * ymu**2
         cove = ((sigyn2*cov**2 + sigy2*sigxn2 + sigxn2*sigyn2) / (2*fqm*sigy2))**0.5
         cov[ibad] = 0.0
         cove[ibad] = np.max(np.concatenate((cov, cove)))
-        
+
 
         # limits on lag measurements due to poisson noise #
         # equation 30 in Vaughan+2003 #
-        limit = np.sqrt(np.abs(n/(fqm * g2 * (p-n))))
-        Limit = np.sqrt(np.abs(N/(fqm * g2 * (P-N))))
-        limit = np.clip(limit, -np.pi, np.pi)
-        Limit = np.clip(Limit, -np.pi, np.pi)
+        xlimit = np.sqrt(np.abs(xnse/(fqm * gg2 * (xpsd-xnse))))
+        ylimit = np.sqrt(np.abs(ynse/(fqm * gg2 * (ypsd-ynse))))
+        xlimit = np.clip(xlimit, -np.pi, np.pi)
+        ylimit = np.clip(ylimit, -np.pi, np.pi)
 
 
         # do we need time lag instead of phase lag? #
         if not phase:
-            lag   /= (2*np.pi*f)
-            lag_e /= (2*np.pi*f)
-            limit /= (2*np.pi*f)
-            Limit /= (2*np.pi*f)
+            lag    /= (2*np.pi*freq)
+            lag_e  /= (2*np.pi*freq)
+            xlimit /= (2*np.pi*freq)
+            ylimit /= (2*np.pi*freq)
 
 
         # return #
-        desc = {'fqL': fqL, 'fqm':fqm, 'limit':limit, 'Limit':Limit, 
-                'limit_avg':(limit+Limit)/2, 'coh': _a([coh, coh_e]),
-                'psd': p, 'nois': n, 'Psd': P, 'Nois': N, 'cxd': c, 'n2': n2, 
-                'g2': g2, 'idx': idx, 'crss': crss, 'freq': f,
-                'rfreq':freq, 'rpsd':rpsd, 'Rpsd':Rpsd, 'rnois':nois, 'RNois': Nois,
-                'rms': _a([rms, rmse]), 'cov': _a([cov, cove]),}
+        extra = {'fql': fql, 'fqm':fqm, 'xlimit':xlimit, 'yLimit':ylimit,
+                'limit_avg':(xlimit+ylimit)/2, 'coh': np.array([coh, coh_e]),
+                'xpsd': xpsd, 'xnse': xnse, 'ypsd': ypsd, 'ynse': ynse,
+                'cxd': crss, 'nn2': nn2, 'gg2': gg2, 'idx': idx, 'freq': freq,
+                'raw': raw, 'rms': np.array([rms, rmse]), 'cov': np.array([cov, cove])}
 
-        return f, lag, lag_e, desc
+        return freq, lag, lag_e, extra
 
 
     @staticmethod
-    def create_segments(Lc, seglen, strict=False, **kwargs):
-        """Split an LCurve or a list of them to segments. 
-        Useful to be used with calculate_psd|lag etc.
+    def read_pn_lcurve(fits_file, **kwargs):
+        """Read pn lcurve fits file.
+            This sets values relevant to PN and calls @misc.read_fits_lcurve
+
+        Parameters
+        ----------
+        fits_file: str
+            The name of the files file
+
+        Keywords
+        --------
+        See @misc.read_fits_lcurve
+
+
+        Return
+        ------
+        LCurve object
+        """
 
+        # set values relevant to XMM-PN files #
+        kwargs.setdefault('min_exp' , 0.7)
+        kwargs.setdefault('gti_tbl' , 2)
 
-        Parameters:
-            Lc: an LCurve or a list of them
-            seglen: segment length in seconds.
-            strict: force all segments to have length length. Some data 
-                may be discarded
+        data, deltat = read_fits_lcurve(fits_file, **kwargs)
+        return LCurve(data[0], data[1], rerr=data[2], deltat=deltat, fexp=data[3])
 
-        Keywords:
-            uneven: The light curves are uneven, so the splitting produces 
-                segments that have the same number of points. Default: False
-            **other arguments to be passed to az.misc.split_array
 
-        Returns:
-            rate, rerr, time, seg_idx
-            seg_idx is the indices used to create the segments.
+    @staticmethod
+    def read_pca_lcurve(fits_file, **kwargs):
+        """Read pca lcurve fits file.
+            This sets values relevant to PCA and calls @misc.read_fits_lcurve
 
-        """
-        # Keyworkds
-        uneven = kwargs.get('uneven', False)
+        Parameters
+        ----------
+        fits_file: str
+            The name of the files file
 
+        Keywords
+        --------
+        See @misc.read_fits_lcurve
 
-        if not type(Lc) == list:
-            Lc = [Lc]
 
-        # assert the same sampling #
-        dt = Lc[0].dt
-        for l in Lc:
-            if dt != l.dt: 
-                raise ValueError('There is a difference in the time sampling between light curves')
+        Return
+        ------
+        LCurve object
+        """
 
-        # segments details #
-        iseglen = np.int(seglen/dt)
+        # set values relevant to PCA files #
+        kwargs.setdefault('min_exp' , 0.99)
+        kwargs.setdefault('gti_tbl' , 'STDGTI')
 
-        # make sure the LCurve objects are evenly sampled #
-        if not uneven:
-            Lc = [l.make_even() for l in Lc]
+        data, deltat = read_fits_lcurve(fits_file, **kwargs)
+        return LCurve(data[0], data[1], rerr=data[2], deltat=deltat, fexp=data[3])
 
 
-        # split the rate arrays #
-        splt = [misc.split_array(l.rate, iseglen, strict, l.rerr, l.time, **kwargs) 
-                        for l in Lc]
+    @staticmethod
+    def read_nu_lcurve(fits_file, **kwargs):
+        """Read nustar lcurve fits file.
+            This sets values relevant to NUSTAR and calls @misc.read_fits_lcurve
 
-        # flatten the segments into on large list #
-        rate = [i for s in splt for i in s[0]]
-        rerr = [i for s in splt for i in s[2]]
-        time = [i for s in splt for i in s[3]]
-        seg_idx = [s[1] for s in splt]
-        return rate, rerr, time, seg_idx
+        Parameters
+        ----------
+        fits_file: str
+            The name of the files file.
 
+        Keywords
+        --------
+        See @misc.read_fits_lcurve
 
-    @staticmethod
-    def prepare_en_segments(rate, rerr, ibin, iref=None, **kwargs):
-        """Create a light curve array at some energy bin(s), and
-            a corresponding reference band if needed.
 
+        Return
+        ------
+        LCurve object
+        """
 
-        Parameters:
-            rate: a list or array of rate values with shape: nen, nseg, ...
-            rerr: the errors array corresponding to rate
-            ibin: the bin number of a interest. int or a list of int giving
-                the indices of interest
-            iref: the bin number or a list of bin numbers to create a secondary
-                reference band. The ibin value(s) will be removed from the 
-                reference light curve if ibin_exclude is true (default). 
-                -1 means use all available bins (excluding ibin)
+        # set values relevant to NUSTAR files #
+        kwargs.setdefault('min_exp' , 0.1)
+        kwargs.setdefault('gti_tbl' , 'GTI')
+        kwargs.setdefault('gti_skip', 3.0)
 
+        data, deltat = read_fits_lcurve(fits_file, **kwargs)
+        return LCurve(data[0], data[1], rerr=data[2], deltat=deltat, fexp=data[3])
 
-        Keywords:
-            ibin_exclude: exclude ibin from iref. Default True
 
-        Returns:
-            rate, rerr, Rate, Rerr 
-            each has dims: (nseg, ...). The first 2 corresponds to summing over ibin
-            and and the last two are for summing over iref (or None if iref=None). Errors
-            are propagated quadratically from the input rerr
+    @staticmethod
+    def read_xis_lcurve(fits_file, **kwargs):
+        """Read suzaku xis lcurve fits file.
+            This sets values relevant to Suzaku XIS and calls @misc.read_fits_lcurve
 
+        Parameters
+        ----------
+        fits_file: str
+            The name of the files file.
+
+        Keywords
+        --------
+        See @misc.read_fits_lcurve
+
+
+        Return
+        ------
+        LCurve object
         """
 
-        # keywords
-        ibin_exclude = kwargs.get('ibin_exclude', True)
+        # set values relevant to XIS files #
+        kwargs.setdefault('min_exp' , 0.1)
+        kwargs.setdefault('gti_tbl' , 'GTI')
+
+        data, deltat = read_fits_lcurve(fits_file, **kwargs)
+        return LCurve(data[0], data[1], rerr=data[2], deltat=deltat, fexp=data[3])
 
-        nen = len(rate)
 
-        # make sure we are dealing with lists #
-        if not isinstance(ibin, list): ibin = [ibin]
+    @staticmethod
+    def read_ni_lcurve(fits_file, **kwargs):
+        """Read nicer lcurve fits file.
+            This sets values relevant to NICER and calls @misc.read_fits_lcurve
 
-        # the rate and error at the bins of interest #
-        r  = np.sum(np.array(rate, dtype=object)[ibin], 0)
-        re = np.sum(np.square(np.array(rerr, dtype=object))[ibin], 0)**0.5
+        Parameters
+        ----------
+        fits_file: str
+            The name of the files file.
 
-        # reference #
-        R, Re = [], []
-        if not iref is None:
-            if not isinstance(iref, list):
-                iref = list(range(nen)) if iref == -1 else [iref]
-            if ibin_exclude:
-                iref = [i for i in iref if not i in ibin]
-            R  = np.sum(np.array(rate, dtype=object)[iref], 0)
-            Re = np.sum(np.square(np.array(rerr, dtype=object))[iref], 0)**0.5
+        Keywords:
+        See @misc.read_fits_lcurve
+
+
+        Returns:
+            LCurve object
+        """
+
+        # set values relevant to NICER files #
+        kwargs.setdefault('min_exp' , 0.99)
+        kwargs.setdefault('gti_tbl' , 'GTI')
 
-        return r, re, R, Re
+        data, deltat = read_fits_lcurve(fits_file, **kwargs)
+        return LCurve(data[0], data[1], rerr=data[2], deltat=deltat, fexp=data[3])
```

### Comparing `aztools-0.1.0/aztools/simlc.py` & `aztools-0.2/src/aztools/simlc.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,470 +1,562 @@
+"""A module for simulating light curves."""
+
+
+from typing import Callable, Union
 
 import numpy as np
+import scipy.stats as st
+from numpy.random import RandomState
 
+__all__ = ['SimLC']
 
-class SimLC(object):
+class SimLC:
     """Class for simulating light curves"""
 
 
     def __init__(self, seed=None):
-        """Create a simlc object, setting some defaults
+        """Initialize a SimLc instance with some random seed
 
         Parameters:
-            seed: a seed for the random number generator
+        -----------
+        seed: int or None
+            a seed for the random number generator
 
         """
 
-        # built-in models #
-        self.builtin_models = ['powerlaw', 'broken_powerlaw', 'bending_powerlaw',
-                                'step', 'constant', 'lorentz', 'user_array']
+        # built-in models and the number of parameter for each one #
+        self.builtin_models = {
+            'powerlaw': 2,
+            'broken_powerlaw': 4,
+            'bending_powerlaw': 3,
+            'lorentz': 3,
+            'constant': 1,
+            'user_array': None,
+        }
 
 
         # model containers #
         self.psd_models = []
         self.lag_models = []
 
+        # other variables
+        self.normalized_psd = None
+        self.normalized_lag = None
+        self.lcurve = None
 
-        # seed random generator #
-        self.rng = np.random.RandomState(seed)
 
+        # seed random generator #
+        self.rng = RandomState(seed)
 
 
-    def add_model(self, model, params, clear=True, lag=False):
-        """Add a model to the generating psd/lag models. Adds the model
-            to self.psd_models or self.lag_models depending on lag
+    def add_model(self,
+                  model: Union[str, Callable],
+                  params: Union[list, np.ndarray],
+                  clear: bool = True,
+                  lag: bool = False ):
+        """Add a model to be used for generating the psd or lag. 
+            
+        This adds the model to self.psd_models or self.lag_models (if lag=True)
 
         Parameters:
-            model: a callable model(freq, params), or a string
-                from the builtin models
-            params: model parameters
-            clear: If true, clear all previously defined models
-            lag: if true, this is a lag model, else it is a psd
+        -----------
+        model: str or Callable 
+            a callable method with model(freq, params), or a string
+            from the builtin models
+        params: list or np.ndarray
+            model parameters
+        clear: bool
+            If True, clear all previously defined models
+        lag: bool
+            if True, this is a lag model, else it is a psd
         """
 
-        
+
         # check the model is callable or in self.builtin_models #
         if isinstance(model, str):
-            if not model in self.builtin_models:
-                mtxt = ', '.join([x for x in self.builtin_models])
-                raise ValueError('model is not in builtin_models\n' + mtxt)
+
+            if model in self.builtin_models:
+                if model != 'user_array' and len(params) != self.builtin_models[model]:
+                    raise ValueError(f'{model} expects {self.builtin_models[model]} parameter')
+
+                model = getattr(SimLC, model)
             else:
-                model = eval('SimLC.' + model)
+                builtin = ', '.join(self.builtin_models)
+                raise ValueError(f'{model} not found in builtin-models: {builtin}')
+
         else:
-            if not hasattr(model, '__call__'):
-                raise ValueError('model is not callable')
+
+            if not isinstance(model, Callable):
+                raise ValueError(f'{model} is not callable')
 
 
         # add given model to the generating list #
         m_container = self.lag_models if lag else self.psd_models
 
         if clear:
-            for k in m_container: m_container.remove(k)
-        m_container.append([model, params])
+            m_container.clear()
 
+        m_container.append([model, params])
 
 
-    def calculate_model(self, freq, lag=False):
+    def calculate_model(self,
+                        freq: Union[list, np.ndarray],
+                        lag: bool = False ) -> np.ndarray:
         """Calculate the psd/lag model using the models
             added with @add_model.
 
-        Parameters:
-            freq: frequency array.
-            lag: if true, calculate the lag model, else do the psd
-
-        Returns:
-            model: array of the same length as freq, containing the model
+        Parameters
+        ----------
+        freq: np.ndarray
+            frequency array.
+        lag: bool
+            if True, calculate the lag model, else do the psd
+
+        Returns
+        -------
+        model: np.ndarray
+            array of the same length as freq, containing the model
 
         Note:
             the normalization of the returned psd/lag is taken from
             the input model parameters without any renormalization
 
         """
 
         # check we have models added #
         models = self.lag_models if lag else self.psd_models
         if len(models) == 0:
-            raise ValueError('No models added. Use add_model to do so.')
+            raise ValueError('No models added. Add models with add_model')
 
 
         # calculate the model #
-        freq = np.array(freq, np.float)
-        mod = np.zeros_like(freq)
-        for m,p in models:
-            mod += m(freq, p)
+        freq = np.array(freq, np.double)
+        total_mod = np.zeros_like(freq)
+        for mod,par in models:
+            total_mod += mod(freq, par)
+
+        return total_mod
 
-        return mod
 
-
-
-    def simulate(self, n, dt, mu, norm='var'):
+    def simulate(self,
+                 npoints: int,
+                 deltat: float,
+                 lcmean: float,
+                 **kwargs):
         """Simulate a light curve using the psd model stored in 
-            self.psd_models, added with add_model
-
-        Parameters:
-            n: number of points in the light curve
-            dt: time sampling
-            mu: the light curve mean
-            norm: string var|rms|leahy
-
-        Returns:
-            Nothing. The simulated light curve and time are stored
-            in self.t and self.x
+            self.psd_models
+            
+        The normalized psd is stored in self.normalized_psd
 
-        Note:
-            The normalized psd is stored in self.normalized_psd
+        Parameters
+        ----------
+        npoints: int
+            number of points in the light curve
+        deltat: float
+            time sampling
+        lcmean: float
+            the light curve mean
+            
+        Keywords
+        --------
+        norm: str
+            on of var|rms|leahy
 
         """
+        # get keywords
+        norm = kwargs.get('norm', 'var')
 
         # make sure the norm is known #
-        if not (norm in ['var', 'leahy', 'rms']):
+        if norm not in ['var', 'leahy', 'rms']:
             raise ValueError('norm need to be one of var|rms|leahy')
 
         # calculate psd #
-        freq = np.fft.rfftfreq(n, dt)
+        freq = np.fft.rfftfreq(npoints, deltat)
         psd = self.calculate_model(freq)
         self.normalized_psd = np.array([freq, psd])
 
-        
+
         # get correct renoramlization #
         expon = {'var':0, 'leahy':1, 'rms':2}
-        renorm = mu**expon[norm] * n/(2.*dt)
-        psd *= renorm
-
+        psd *= lcmean**expon[norm] * npoints/(2.*deltat)
 
 
         # inverse fft #
-        ix = ( self.rng.randn(len(psd)) * np.sqrt(0.5*psd)
-             + self.rng.randn(len(psd)) * np.sqrt(0.5*psd)*1j )
-        ix[0] = n * mu
-        ix[-1] = np.abs(ix[-1])
-        self.x = np.fft.irfft(ix)
-        self.t = np.arange(n) * dt * 1.0
-
-
-
-    def simulate_pdf(self, n, dt, mu, norm='var', pdf='lognorm(s=0.5)'):
-        """Simulate a light curve using the psd model stored in 
-            self.psd_models, added with add_model, and enforcing
-            log-normal distribution.
-            This uses the algorithm of Emmanoulopoulos+ (2013) MNRAS 433, 907–927
-
-        Parameters:
-            n: number of points in the light curve
-            dt: time sampling
-            mu: the light curve mean
-            norm: string var|rms|leahy
-            pdf: a string representing a probability distribution
-                from scipy.stats. e.g. lognorm(s=0.5)
-
-        Returns:
-            Nothing. The simulated light curve and time are stored
-            in self.t and self.x
+        ixarr = ( self.rng.randn(len(psd)) * np.sqrt(0.5*psd) +
+                  self.rng.randn(len(psd)) * np.sqrt(0.5*psd)*1j )
+        ixarr[0] = npoints * lcmean
+        ixarr[-1] = np.abs(ixarr[-1])
+        self.lcurve = [
+            np.arange(npoints) * deltat * 1.0,
+            np.fft.irfft(ixarr)
+        ]
+
+
+    def simulate_pdf(self,
+                     npoints: int,
+                     deltat: float,
+                     lcmean: float,
+                     **kwargs):
+        """Simulate a light curve using the psd model enforcing 
+        some probability distribution
+        
+        This uses the algorithm of Emmanoulopoulos+ (2013) MNRAS 433, 907–927
+            
+        The normalized psd is stored in self.normalized_psd
 
-        Note:
-            The normalized psd is stored in self.normalized_psd
+        Parameters
+        ----------
+        npoints: int
+            number of points in the light curve
+        deltat: float
+            time sampling
+        lcmean: float
+            the light curve mean
+            
+        Keywords
+        --------
+        norm: str
+            on of var|rms|leahy
+        pdf: scipy.stats._distn_infrastructure.rv_frozen
+            The probability distribution object from scipy.stats that defines
+            the desired pdf. e.g. scipy.stats.lognorm(s=0.5)
 
         """
+        # get keywords
+        norm = kwargs.get('norm')
+        pdf  = kwargs.get('pdf', st.lognorm(s=0.5))
 
         # make sure the norm is known #
-        if not (norm in ['var', 'leahy', 'rms']):
+        if norm not in ['var', 'leahy', 'rms']:
             raise ValueError('norm need to be one of var|rms|leahy')
 
-        import scipy.stats as st
-        lognorm = eval('st.{}'.format(pdf))
-
+        if not hasattr(pdf, 'rvs'):
+            raise ValueError((
+                'pdf needs to be an instance of '
+                'scipy.stats._distn_infrastructure.rv_frozen'
+            ))
 
         # calculate psd #
-        freq = np.fft.rfftfreq(n, dt)
+        freq = np.fft.rfftfreq(npoints, deltat)
         psd = self.calculate_model(freq)
         self.normalized_psd = np.array([freq, psd])
 
-        
+
         # get correct renoramlization #
         expon = {'var':0, 'leahy':1, 'rms':2}
-        renorm = mu**expon[norm] * n/(2.*dt)
-        psd *= renorm
-
+        psd *= lcmean**expon[norm] * npoints/(2.*deltat)
 
 
         # do the algorithm #
-        ix = ( self.rng.randn(len(psd)) * np.sqrt(0.5*psd)
-             + self.rng.randn(len(psd)) * np.sqrt(0.5*psd)*1j )
-        ix[0] = n * mu
-        ix[-1] = np.abs(ix[-1])
+        ixarr = ( self.rng.randn(len(psd)) * np.sqrt(0.5*psd) +
+                  self.rng.randn(len(psd)) * np.sqrt(0.5*psd)*1j )
+        ixarr[0] = npoints * lcmean
+        ixarr[-1] = np.abs(ixarr[-1])
+
         # step-1 #
-        anorm  = np.abs(ix)
+        anorm  = np.abs(ixarr)
 
         # step-2; before loop starts #
-        xsim   = lognorm.rvs(n)
-        diff   = 1.0
+        xsim = pdf.rvs(npoints)
+        diff = 1.0
         while diff > 1e-4:
 
-            # step-2; main loop #
-            psim   = np.angle(np.fft.rfft(xsim))
-
-            # step-3
-            xsim_j = np.fft.irfft(anorm * np.exp(1j*psim))
+            # step-2 and step-3
+            xsim_j = np.fft.irfft(anorm * np.exp(1j*np.angle(np.fft.rfft(xsim))))
 
             # step-4
             xsim_j[np.argsort(xsim_j)] = xsim[np.argsort(xsim)]
-            
+
             # check for convergenece & prepare for next loop #
-            diff   = np.sum((xsim - xsim_j)**2)/n
+            diff   = np.sum((xsim - xsim_j)**2)/npoints
             xsim[:]= xsim_j[:]
 
-
-        # get the final light curve
-        psim   = np.angle(np.fft.rfft(xsim))
-        self.x = np.fft.irfft(anorm * np.exp(1j*psim))
-        self.t = np.arange(n) * dt * 1.0
-
-
-
-    def apply_lag(self, phase=False):
-        """Apply lag in self.lag_models to the simulate self.c
-
-        Parameters:
-            phase: the lags in self.lag_models are in radians
-            if true, else in seconds.
-
-        Returns:
-            Nothing. creates self.y for the shifted light curve
-            and self.normalized_lag for the actual [freq, lag ] used
-
-        Note:
-            The lag vs freq is found by calling the functions in
-            self.lag_models, filled by calling add_model(..., lag=True)
-            The light curve in self.x is assumed to exist (i.e. self.simulate
-            should've been called already)
+        # final inverse fft #
+        self.lcurve = [
+            np.arange(npoints) * deltat * 1.0,
+            np.fft.irfft(anorm * np.exp(1j*np.angle(np.fft.rfft(xsim))))
+        ]
+
+
+    def apply_lag(self, phase: bool = False):
+        """Apply lag in self.lag_models to the simulated light curve
+
+        - This assumes self.simulate has been run.
+        - Lag models are added by add_model(..., lag=True)
+        - The resulting lag model is stored in self.normalized_lag
+        - The generated lagged light curve is added self.lcurve
+
+
+        Parameters
+        ----------
+        phase: bool
+            If Trye, the lags in self.lag_models are in radians,
+            otherwise they are in seconds.
 
         """
 
         # has simulate beed run? #
-        try:
-            self.x
-        except:
-            raise ValueError('self.x does not exists. Run simulate first')
+        if self.lcurve is None:
+            raise ValueError('self.lcurve does not exists. Call simulate(...) first')
 
         freq = self.normalized_psd[0]
         lag  = self.calculate_model(freq, lag=True)
         self.normalized_lag = np.array([freq, lag])
-        self.y = SimLC.lag_array(self.x, lag, phase, freq)
-
 
+        xarr = self.lcurve[1]
+        yarr = SimLC.lag_array(xarr, lag, phase, freq)
+        if len(self.lcurve) == 3:
+            del self.lcurve[-1]
+        self.lcurve.append(yarr)
 
 
-    @staticmethod 
-    def lag_array(x, lag, phase=False, freq=None):
-        """Shift the x by amount lag
-        
-        Args:
-            x: light curve to be shifted
-            lag: float or array of length len(n)/2+1
-            phase: if True, lag is in radians. Otherwise in seconds
-            freq: the frequency axis (used when phase is False)
+    @staticmethod
+    def lag_array(xarr: np.ndarray,
+                  lag: Union[np.ndarray, float],
+                  phase: bool = False,
+                  freq: Union[np.ndarray, None] = None ) -> np.ndarray:
+        """Shift the array xarr by a lag
+        
+        Parameters
+        ----------
+        xarr: np.ndarray
+            light curve array to be shifted
+        lag: np.ndarray or float
+            If array, it has length len(xarr)/2+1. If float,
+            the lag is assumed constant with frequency
+        phase: bool
+            if True, lag is in radians. Otherwise in seconds
+        freq: np.ndarray or None
+            The frequency axis (used to convert lag to radians when phase is False)
             
 
-        Returns:
-            An array containing the shifted light curve.
+        Returns
+        -------
+        An array containing the shifted light curve.
 
         """
-        nfq = len(x)/2 + 1
-        if not isinstance(lag, np.ndarray): lag = np.repeat(lag, nfq)
-        if nfq != len(lag):
-            raise ValueError('Lag array does not match given array')
-        
-        if freq is not None and nfq != len(freq):
-            raise ValueError('freq array does not match given array')
-        
+
+        # xarr has to be even length
+        if len(xarr) % 2 == 1:
+            raise ValueError('xarr has to be even in length')
+
+        nfreq = len(xarr)/2 + 1
+
+        if not isinstance(lag, np.ndarray):
+            lag = np.repeat(lag, nfreq)
+
+        if nfreq != len(lag):
+            raise ValueError(f'lag array does not match given xarr. Expecting {nfreq}')
+
+        if freq is not None and nfreq != len(freq):
+            raise ValueError(f'freq array does not match given xarr. Expecting {nfreq}')
+
         phi = lag if phase else lag*2.*np.pi*freq
-        xfft = np.fft.rfft(x)
+        xfft = np.fft.rfft(xarr)
         xfft[1:-1] *= np.exp(-1j*phi[1:-1])
         return np.fft.irfft(xfft)
 
 
     @staticmethod
-    def add_noise(x, norm=None, seed=None, dt=1.0):
-        """Add noise to lcurve x
-    
-        Parameters:
-            norm: if None, add Poisson noise, else
-                gaussian noise, with std=norm
-            seed: random seed
-            dt: used with norm is None. It gives the time samling
-                of the light curve. Poisson noise is applied to
-                the counts per bin. x in this case is the count rate.
-                Counts/bin = Rate/sec * dt
+    def add_noise(xarr: np.ndarray,
+                  norm: Union[float, None] = None,
+                  seed: Union[int, None] = None,
+                  deltat: float = 1.0):
+        """Add noise to a lcurve xarr
+
+        Parameters
+        ----------
+        xarray: np.ndarray
+            Input light curve array
+        norm: float or None
+            if None, add Poisson noise, else gaussian noise
+            with std=norm.
+        seed: int or None
+            Random seed
+        deltat: float
+            used when norm is None. It gives the time samling
+            of the light curve. Poisson noise is applied to
+            the counts per bin. xarr in this case is the count rate.
+            Counts/bin = Rate/sec * dt
             
 
-        Returns:
-            array similar to x with noise added
+        Return
+        ------
+        An array similar to xarr with noise added
 
         """
 
         if seed is not None:
             np.random.seed(seed)
 
         if norm is None:
-            xn = np.random.poisson(x*dt)/dt
+            xnoise = np.random.poisson(xarr*deltat)/deltat
         else:
-            xn = np.random.randn(len(x)) * norm + x
-        return xn
+            xnoise = np.random.randn(len(xarr)) * norm + xarr
+        return xnoise
 
-    
-    @staticmethod
-    def user_array(freq, params):
-        """The model is given by the user directly as an array params
 
-        Parameters:
-            freq (np.ndarray): the frequency array
-            params (np.ndarray): the model values
-
-        Returns:
-            array mod of same length as freq, containing the psd/lag model
+    @staticmethod
+    def user_array(freq: np.ndarray,
+                   params: np.ndarray) -> np.ndarray:
+        """Generate a model to be used as psd or lag.
+        
+        The model is given by the user directly as an array params
+
+        Parameters
+        ----------
+        freq: np.ndarray
+            The frequency array
+        params: np.ndarray
+            The model values
+
+        Return
+        ------
+            An array of the model values at freq, containing the psd/lag model
         """
 
         if len(params) != len(freq):
-            raise ValueError('params does not match freq: %d vs %d'%(len(params), len(freq)))
+            raise ValueError(f'params does not match freq: {len(params)} vs {len(freq)}')
         return np.array(params)
 
 
     @staticmethod
-    def powerlaw(freq, params):
-        """A powerlaw model for the psd/lag
+    def powerlaw(freq: np.ndarray,
+                 params: Union[np.ndarray, list]) -> np.ndarray:
+        """Generate a powerlaw model to be used as psd or lag.
 
-        Parameters:
-            freq (np.ndarray): the frequency array
-            params (list or array: [norm, indx]): parameters of the model
-        
-        Returns:
-            array mod of same length as freq, containing the psd/lag model
+
+        Parameters
+        ----------
+        freq: np.ndarray
+            The frequency array
+        params: np.ndarray or list
+            Parameters of the model as: [norm, indx]
+
+        Return
+        ------
+            An array of the model values at freq, containing the psd/lag model
 
         """
 
         if len(params) != 2:
             raise ValueError('powerlaw needs 2 params: norm, index')
         norm, indx = params
         freq = np.clip(freq, 1e-30, np.inf)
         mod = norm * freq**indx
         return mod
 
 
     @staticmethod
-    def broken_powerlaw(freq, params):
-        """A borken powerlaw model for the psd/lag.
+    def broken_powerlaw(freq: np.ndarray,
+                        params: Union[np.ndarray, list]) -> np.ndarray:
+        """Generate a broken powerlaw model to be used as psd or lag.
 
-        Parameters:
-            freq (np.ndarray): the frequency array
-            params (list or array: [norm, indx1, indx2, break]):
-                parameters of the model
-        
-        Returns:
-            array mod of same length as freq, containing the psd/lag model
+
+        Parameters
+        ----------
+        freq: np.ndarray
+            The frequency array
+        params: np.ndarray or list
+            Parameters of the model as: [norm, indx1, indx2, break]
+
+        Return
+        ------
+            An array of the model values at freq, containing the psd/lag model
 
         """
 
         if len(params) != 4:
-            raise ValueError(('broek_powerlaw needs 4 params: norm, '
-                      'index1, index2, break'))
-        norm, a1, a2, brk = params
+            raise ValueError((
+                'broek_powerlaw needs 4 params: norm, '
+                'index1, index2, break'
+            ))
+        norm, idx1, idx2, brk = params
         freq = np.clip(freq, 1e-30, np.inf)
         fq_indx = freq < brk
         mod = np.zeros_like(freq)
-        mod[fq_indx] = (freq[fq_indx]/brk) ** a1
-        mod[~fq_indx] = (freq[~fq_indx]/brk) ** a2
-        mod *= norm * brk**a2
+        mod[fq_indx] = (freq[fq_indx]/brk) ** idx1
+        mod[~fq_indx] = (freq[~fq_indx]/brk) ** idx2
+        mod *= norm * brk**idx2
         return mod
 
 
     @staticmethod
-    def bending_powerlaw(freq, params):
-        """A bending powerlaw model for the psd/lag.
-
-        Parameters:
-            freq (np.ndarray): the frequency array
-            params (list or array: [norm, index, break]):
-                parameters of the model. The index below the
-                break is always 0
-        
-        Returns:
-            array mod of same length as freq, containing the psd/lag model
+    def bending_powerlaw(freq: np.ndarray,
+                         params: Union[np.ndarray, list]) -> np.ndarray:
+        """Generate a bending powerlaw model to be used as psd or lag.
+
+
+        Parameters
+        ----------
+        freq: np.ndarray
+            The frequency array
+        params: np.ndarray or list
+            Parameters of the model as: [norm, index, break]). 
+            The index below the break is always 0.
+
+        Return
+        ------
+            An array of the model values at freq, containing the psd/lag model
 
         """
 
         if len(params) != 3:
-            raise ValueError(('bending_powerlaw needs 3 params: norm, '
-                      'index, break'))
-        norm, a, brk = params
+            raise ValueError((
+                'bending_powerlaw needs 3 params: norm, '
+                'index, break'
+            ))
+        norm, idx, brk = params
         freq = np.clip(freq, 1e-30, np.inf)
-        mod = (norm/freq) * (1+(freq/brk)**(-a-1))**(-1)
+        mod = (norm/freq) * (1+(freq/brk)**(-idx-1))**(-1)
         return mod
 
 
     @staticmethod
-    def step(freq, params):
-        """A step function model for the psd/lag.
+    def lorentz(freq: np.ndarray,
+                params: Union[np.ndarray, list]) -> np.ndarray:
+        """Generate a lorentz model to be used as psd or lag.
 
-        Parameters:
-            freq (np.ndarray): the frequency array
-            params: a list (or array) of 2 lists (arrays).
-                The first holds the frequency bin boundaries.
-                The second holds the values of psd|lag
-                len(list_1) = len(list_2) + 1
-        
-        Returns:
-            array mod of same length as freq, containing the psd/lag model
 
-        """
-
-        if len(params) != 2:
-            raise ValueError('step needs a list of 2 arrays/lists')
-        fqL, pars = params
-        fqL, pars = np.array(fqL), np.array(pars)
-        if len(fqL) != len(pars)+1:
-            raise ValueError('fqL and pars do not match')
-
-        ibins = np.digitize(freq, fqL, right=True) - 1
-        ibins[ibins==-1] = 0
-        ibins[ibins==len(fqL)-1] = len(fqL)-2
-        mod = pars[ibins]
-        return mod
-
-
-    @staticmethod
-    def constant(freq, params):
-        """A constant model for the psd/lag
-
-        Parameters:
-            freq (np.ndarray): the frequency array
-            params (float): the value of the constant
-        
-        Returns:
-            array mod of same length as freq, containing the psd model
+        Parameters
+        ----------
+        freq: np.ndarray
+            The frequency array
+        params: np.ndarray or list
+            Parameters of the model as: [norm, fq_center, fq_sigma]
+
+        Return
+        ------
+            An array of the model values at freq, containing the psd/lag model
 
         """
-        mod = freq*0 + params
-        return mod
-
-
-    @staticmethod
-    def lorentz(freq, params):
-        """A lorentzian model for the psd/lag
-
-        Parameters:
-            freq (np.ndarray): the frequency array
-            params (list or array: [norm, fq_center, fq_sigma]):
-                parameters of the model
-        
-        Returns:
-            array mod of same length as freq, containing the psd/lag model
 
-        """
         if len(params) != 3:
             raise ValueError('lorentz needs 3 pars: norm, fq_cent, fq_sig')
         norm, fq_center, fq_sigma = params
         mod = norm * (fq_sigma/(2*np.pi)) / (
-                    (freq-fq_center)**2 + (fq_sigma/2)**2 )
+                     (freq-fq_center)**2 + (fq_sigma/2)**2 )
         return mod
 
 
-
+    @staticmethod
+    def constant(freq: np.ndarray,
+                 params: Union[np.ndarray, list]) -> np.ndarray:
+        """Generate a constant model to be used as psd or lag.
+
+
+        Parameters
+        ----------
+        freq: np.ndarray
+            The frequency array
+        params: np.ndarray or list
+            Parameters of the model as [value]
+
+        Return
+        ------
+            An array of the model values at freq, containing the psd/lag model
+
+        """
+        if len(params) != 1:
+            raise ValueError('constant needs 1 parameter')
+        mod = freq*0 + params[0]
+        return mod
```

