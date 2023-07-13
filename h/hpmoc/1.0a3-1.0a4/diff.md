# Comparing `tmp/hpmoc-1.0a3.tar.gz` & `tmp/hpmoc-1.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hpmoc-1.0a3.tar", last modified: Mon Jul  3 21:55:15 2023, max compression
+gzip compressed data, was "hpmoc-1.0a4.tar", last modified: Thu Jul 13 23:02:26 2023, max compression
```

## Comparing `hpmoc-1.0a3.tar` & `hpmoc-1.0a4.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0    18092 2023-07-03 06:59:36.334737 hpmoc-1.0a3/LICENSE
--rw-r--r--   0        0        0     2549 2022-12-23 19:45:53.082596 hpmoc-1.0a3/Makefile
--rw-r--r--   0        0        0     3301 2023-07-03 19:52:28.451592 hpmoc-1.0a3/README.md
--rw-r--r--   0        0        0       25 2022-12-23 19:45:53.082596 hpmoc-1.0a3/docs/.gitignore
--rw-r--r--   0        0        0      638 2022-12-23 19:45:53.082596 hpmoc-1.0a3/docs/Makefile
--rw-r--r--   0        0        0      804 2022-12-23 19:45:53.082596 hpmoc-1.0a3/docs/make.bat
--rw-r--r--   0        0        0     6203 2022-12-23 19:45:53.082596 hpmoc-1.0a3/docs/source/conf.py
--rw-r--r--   0        0        0     3842 2022-12-23 19:45:53.082596 hpmoc-1.0a3/docs/source/index.rst
--rw-r--r--   0        0        0    40825 2022-12-23 19:45:53.082596 hpmoc-1.0a3/docs/source/jup/plotting-examples.ipynb
--rw-r--r--   0        0        0      521 2023-07-03 19:32:25.161624 hpmoc-1.0a3/hpmoc-dev-win.yml
--rw-r--r--   0        0        0      562 2023-07-03 19:32:25.161624 hpmoc-1.0a3/hpmoc-dev.yml
--rw-r--r--   0        0        0     1032 2023-07-03 21:54:52.211627 hpmoc-1.0a3/hpmoc/__init__.py
--rw-r--r--   0        0        0     1143 2023-07-03 19:43:54.661628 hpmoc-1.0a3/hpmoc/abstract.py
--rw-r--r--   0        0        0     5992 2023-07-03 19:39:12.181616 hpmoc-1.0a3/hpmoc/healpy.py
--rw-r--r--   0        0        0     2434 2023-07-03 19:43:58.561626 hpmoc-1.0a3/hpmoc/healpy_utils.py
--rw-r--r--   0        0        0     6949 2023-07-03 21:54:38.341626 hpmoc-1.0a3/hpmoc/io/__init__.py
--rw-r--r--   0        0        0     2279 2023-07-03 20:49:43.901611 hpmoc-1.0a3/hpmoc/io/abstract.py
--rw-r--r--   0        0        0     3297 2023-07-03 20:50:42.731624 hpmoc-1.0a3/hpmoc/io/astroquery.py
--rw-r--r--   0        0        0    12349 2023-07-03 20:42:44.021630 hpmoc-1.0a3/hpmoc/io/fits.py
--rw-r--r--   0        0        0     4849 2023-07-03 20:50:34.541623 hpmoc-1.0a3/hpmoc/io/gracedb.py
--rw-r--r--   0        0        0     3394 2023-07-03 20:16:09.031605 hpmoc-1.0a3/hpmoc/io/ligo.py
--rw-r--r--   0        0        0    53953 2023-07-03 21:35:31.821599 hpmoc-1.0a3/hpmoc/partial.py
--rw-r--r--   0        0        0    56536 2023-07-03 20:42:18.371588 hpmoc-1.0a3/hpmoc/plot.py
--rw-r--r--   0        0        0    36795 2023-07-03 19:44:32.571620 hpmoc-1.0a3/hpmoc/plotters.py
--rw-r--r--   0        0        0    12325 2023-07-03 19:44:44.001626 hpmoc-1.0a3/hpmoc/points.py
--rw-r--r--   0        0        0     3721 2023-07-03 19:44:52.571626 hpmoc-1.0a3/hpmoc/psf.py
--rw-r--r--   0        0        0    92991 2023-07-03 20:43:05.981627 hpmoc-1.0a3/hpmoc/utils.py
--rw-r--r--   0        0        0     1749 2023-07-03 21:06:24.211608 hpmoc-1.0a3/pyproject.toml
--rw-r--r--   0        0        0     5413 1970-01-01 00:00:00.000000 hpmoc-1.0a3/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-07-03 06:59:36.334737 hpmoc-1.0a4/LICENSE
+-rw-r--r--   0        0        0     2549 2022-12-23 19:45:53.082596 hpmoc-1.0a4/Makefile
+-rw-r--r--   0        0        0     3301 2023-07-03 19:52:28.451592 hpmoc-1.0a4/README.md
+-rw-r--r--   0        0        0       25 2022-12-23 19:45:53.082596 hpmoc-1.0a4/docs/.gitignore
+-rw-r--r--   0        0        0      638 2022-12-23 19:45:53.082596 hpmoc-1.0a4/docs/Makefile
+-rw-r--r--   0        0        0      804 2022-12-23 19:45:53.082596 hpmoc-1.0a4/docs/make.bat
+-rw-r--r--   0        0        0     6203 2022-12-23 19:45:53.082596 hpmoc-1.0a4/docs/source/conf.py
+-rw-r--r--   0        0        0     3842 2022-12-23 19:45:53.082596 hpmoc-1.0a4/docs/source/index.rst
+-rw-r--r--   0        0        0    40825 2022-12-23 19:45:53.082596 hpmoc-1.0a4/docs/source/jup/plotting-examples.ipynb
+-rw-r--r--   0        0        0      521 2023-07-03 19:32:25.161624 hpmoc-1.0a4/hpmoc-dev-win.yml
+-rw-r--r--   0        0        0      562 2023-07-03 19:32:25.161624 hpmoc-1.0a4/hpmoc-dev.yml
+-rw-r--r--   0        0        0     1032 2023-07-13 23:00:13.150068 hpmoc-1.0a4/hpmoc/__init__.py
+-rw-r--r--   0        0        0     1143 2023-07-03 19:43:54.661628 hpmoc-1.0a4/hpmoc/abstract.py
+-rw-r--r--   0        0        0     6201 2023-07-07 05:29:37.570077 hpmoc-1.0a4/hpmoc/arraysetops.py
+-rw-r--r--   0        0        0     5992 2023-07-03 19:39:12.181616 hpmoc-1.0a4/hpmoc/healpy.py
+-rw-r--r--   0        0        0     2434 2023-07-03 19:43:58.561626 hpmoc-1.0a4/hpmoc/healpy_utils.py
+-rw-r--r--   0        0        0     6949 2023-07-03 21:54:38.341626 hpmoc-1.0a4/hpmoc/io/__init__.py
+-rw-r--r--   0        0        0     2279 2023-07-03 20:49:43.901611 hpmoc-1.0a4/hpmoc/io/abstract.py
+-rw-r--r--   0        0        0     3297 2023-07-03 20:50:42.731624 hpmoc-1.0a4/hpmoc/io/astroquery.py
+-rw-r--r--   0        0        0    12349 2023-07-03 20:42:44.021630 hpmoc-1.0a4/hpmoc/io/fits.py
+-rw-r--r--   0        0        0     4849 2023-07-03 20:50:34.541623 hpmoc-1.0a4/hpmoc/io/gracedb.py
+-rw-r--r--   0        0        0     3394 2023-07-03 20:16:09.031605 hpmoc-1.0a4/hpmoc/io/ligo.py
+-rw-r--r--   0        0        0    54606 2023-07-13 22:46:35.890064 hpmoc-1.0a4/hpmoc/partial.py
+-rw-r--r--   0        0        0    56536 2023-07-03 20:42:18.371588 hpmoc-1.0a4/hpmoc/plot.py
+-rw-r--r--   0        0        0    36795 2023-07-03 19:44:32.571620 hpmoc-1.0a4/hpmoc/plotters.py
+-rw-r--r--   0        0        0    12325 2023-07-03 19:44:44.001626 hpmoc-1.0a4/hpmoc/points.py
+-rw-r--r--   0        0        0     3721 2023-07-03 19:44:52.571626 hpmoc-1.0a4/hpmoc/psf.py
+-rw-r--r--   0        0        0    93078 2023-07-07 05:26:12.900078 hpmoc-1.0a4/hpmoc/utils.py
+-rw-r--r--   0        0        0     1768 2023-07-13 22:48:45.670065 hpmoc-1.0a4/pyproject.toml
+-rw-r--r--   0        0        0     5458 1970-01-01 00:00:00.000000 hpmoc-1.0a4/PKG-INFO
```

### Comparing `hpmoc-1.0a3/LICENSE` & `hpmoc-1.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a3/Makefile` & `hpmoc-1.0a4/Makefile`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a3/README.md` & `hpmoc-1.0a4/README.md`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a3/docs/Makefile` & `hpmoc-1.0a4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a3/docs/make.bat` & `hpmoc-1.0a4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a3/docs/source/conf.py` & `hpmoc-1.0a4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a3/docs/source/index.rst` & `hpmoc-1.0a4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a3/docs/source/jup/plotting-examples.ipynb` & `hpmoc-1.0a4/docs/source/jup/plotting-examples.ipynb`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a3/hpmoc-dev-win.yml` & `hpmoc-1.0a4/hpmoc-dev-win.yml`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a3/hpmoc-dev.yml` & `hpmoc-1.0a4/hpmoc-dev.yml`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a3/hpmoc/__init__.py` & `hpmoc-1.0a4/hpmoc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,10 +16,10 @@
 
 """
 HPMOC is an ultra high-performance, cross-platform toolset for working with
 multi-order coordinate (MOC) HEALPix images (i.e. images with multiple pixel
 resolutions).
 """
 
-__version__ = '1.0a3'
+__version__ = '1.0a4'
 
 from .partial import PartialUniqSkymap as PartialUniqSkymap
```

### Comparing `hpmoc-1.0a3/hpmoc/abstract.py` & `hpmoc-1.0a4/hpmoc/abstract.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a3/hpmoc/healpy.py` & `hpmoc-1.0a4/hpmoc/healpy.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a3/hpmoc/healpy_utils.py` & `hpmoc-1.0a4/hpmoc/healpy_utils.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a3/hpmoc/io/__init__.py` & `hpmoc-1.0a4/hpmoc/io/__init__.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a3/hpmoc/io/abstract.py` & `hpmoc-1.0a4/hpmoc/io/abstract.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a3/hpmoc/io/astroquery.py` & `hpmoc-1.0a4/hpmoc/io/astroquery.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a3/hpmoc/io/fits.py` & `hpmoc-1.0a4/hpmoc/io/fits.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a3/hpmoc/io/gracedb.py` & `hpmoc-1.0a4/hpmoc/io/gracedb.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a3/hpmoc/io/ligo.py` & `hpmoc-1.0a4/hpmoc/io/ligo.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a3/hpmoc/partial.py` & `hpmoc-1.0a4/hpmoc/partial.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import base64
 from io import BytesIO
 from textwrap import wrap, dedent
 from collections import OrderedDict
 from typing import (
     List,
     Iterator,
-    MutableMapping,
+    Mapping,
     Callable,
     Literal,
     Sequence,
     Optional,
     Union,
     IO,
     Tuple,
@@ -282,14 +282,15 @@
     A HEALPix skymap object residing in memory with NUNIQ ordering. Only
     a subset of the full sky. You can index into a ``PartialUniqSkymap`` with
     NUNIQ indices to get a skymap with the same shape (optionally padding
     missing values with a second index argument). You can also use index
     notation to set pixel values at the specified NUNIQ index locations.
     """
     point_sources: List[PointsTuple]
+    meta: Mapping[str, Any]
 
     def __init__(
         self,
         s: 'NDArray[_DType]',
         u: Union['NDArray[np.integer[Any]]', 'WCS'],
         copy: bool = False, name=None, point_sources=None,
         meta=None, empty=None, compress=False, interp="nearest"):
@@ -372,28 +373,33 @@
         if not np.issubdtype(self.s.dtype, np.number):
             raise ValueError(f"`s` must be numeric. got: {s}")
 
         # provide point sources and deduplicate
         self.point_sources = PointsTuple.dedup(*(point_sources or []))
 
         meta = meta or {}
-        newmeta = OrderedDict()
+        newmeta = {}
         for k, v in meta.items():
             if not (PT_META_REGEX.match(k) or
                     PT_META_KW_REGEX.match(k) or
                     PT_META_COLOR_REGEX.match(k)):
                 newmeta[k] = v
         newmeta['PIXTYPE'] = 'HEALPIX'
         newmeta['ORDERING'] = 'NUNIQ'
         newmeta['PARTIAL'] = True
         self.meta = newmeta
 
         if isinstance(s, (Qty, Col)):              # preserve astropy unit
             self.s = Qty(self.s, cast(Union[Qty, Col], s).unit, copy=False)
 
+    def _meta_copy(self):
+        """Returns a shallow copy of self.meta. Needed since .copy() isn't in
+        the ABC for Mapping"""
+        return {k: v for k, v in self.meta.items()}
+
     @overload
     def nside(self, as_skymap: Literal[True], copy: bool = False, **kwargs) -> 'PartialUniqSkymap[np.integer[Any]]': ...
 
     @overload
     def nside(self, as_skymap: Literal[False] = False, copy: bool = False, **kwargs) -> 'NDArray[np.integer[Any]]': ...
 
     def nside(self, as_skymap=False, copy=False, **kwargs): # type: ignore
@@ -402,15 +408,15 @@
         ``PartialUniqSkymap`` instance (with ``**kwargs`` passed to init).
         """
         import numpy as np
 
         n = uniq2nside(self.u)
         if as_skymap:
             u = np.array(self.u, copy=True) if copy else self.u
-            m = self.meta.copy()
+            m = self._meta_copy()
             m['HISTORY'] = m.get('HISTORY', []) + ['Take HEALPix NSIDE.']
             return type(self)(n, u, copy=False, name='NSIDE', meta=m,
                               point_sources=self.point_sources,
                               **kwargs)
         return n
 
     @overload
@@ -425,15 +431,15 @@
         ``PartialUniqSkymap`` instance (with ``**kwargs`` passed to init).
         """
         import numpy as np
 
         o = uniq2order(self.u)
         if as_skymap:
             u = np.array(self.u, copy=True) if copy else self.u
-            m = self.meta.copy()
+            m = self._meta_copy()
             m['HISTORY'] = m.get('HISTORY', []) + ['Take HEALPix order.']
             return type(self)(o, u, copy=False, name='ORDER', meta=m,
                               point_sources=self.point_sources,
                               **kwargs)
         return o
 
     def copy(self: 'PartialUniqSkymap[_DType]') -> 'PartialUniqSkymap[_DType]':
@@ -477,15 +483,15 @@
         from astropy.units import Quantity
 
         if not isinstance(self.s, Quantity):
             raise TypeError("Can only convert dimensions of a ``Quantity``")
         _s = cast(Quantity, self.s) # make pyright happy
         return type(self)(_s.to(*args, **kwargs), self.u,
                           copy=False, name=self.name,
-                          meta=self.meta.copy(),
+                          meta=self._meta_copy(),
                           point_sources=self.point_sources)
 
     def compress(self, stype: Optional['np.dtype'] = None, utype: Optional['np.dtype'] = None, **kwargs) -> 'PartialUniqSkymap':
         """
         Eliminate redundant pixels with ``utils.uniq_minimize`` and store
         indices ``u`` in the smallest integer size that represents all values.
 
@@ -509,15 +515,15 @@
         hpmoc.utils.uniq_minimize
         """
         u, s = uniq_minimize(self.u, self.s)
         if utype is None:
             utype = max_uint_type(self.u.max())
         s = s if stype is None else s.astype(stype)
         return type(self)(s, u.astype(utype), copy=False,
-                          name=self.name, meta=self.meta.copy(),
+                          name=self.name, meta=self._meta_copy(),
                           point_sources=self.point_sources)
 
     def sort(self: 'PartialUniqSkymap[_DType]', copy=True) -> 'PartialUniqSkymap[_DType]':
         """
         Sort this skymap by UNIQ indices ``u`` (sorting ``s`` as well, of
         course). If ``copy=True``, copy ``u`` and ``s`` and return a new
         ``PartialUniqSkymap``; otherwise, sort them in-place and return this
@@ -562,15 +568,15 @@
         the NUNIQ indices ``self.u``; otherwise, share them with the new
         skymap. To operate directly on the skymap value (even if it is stored
         as an ``astropy.units.Quantity``), use ``quantity = True``. Note that
         this will strip units from the result.
         """
         from astropy.units import Quantity
 
-        m = self.meta.copy()
+        m = self._meta_copy()
         mod = getattr(func, '__module__',
                       getattr(type(func), '__module__',
                               sys._getframe(-1).f_locals.get('__name__')))
         mod = '' if mod is None else mod + '.'
         m['HISTORY'] = (m.get('HISTORY', []) +
                         [f'Applied {mod}{func.__name__}'])
         n = f"{func.__name__}({self.name})"
@@ -578,28 +584,42 @@
             s = cast(Quantity, self.s).value
         else:
             s = self.s
         return type(self)(func(s), self.u.copy() if copy else self.u,
                           copy=False, name=n, meta=m,
                           point_sources=self.point_sources)
 
-    def to_table(self, name=None, uname='UNIQ'):
+    def to_table(self, name=None, uname='UNIQ', meta_compat=False):
         """
         Return a new ``astropy.table.Table`` whose ``UNIQ`` column is the NUNIQ
         indices ``self.u`` and ``PIXELS`` (or ``self.name``, if set) column is
         the skymap pixel values ``s``. Optionally override the pixel value
         column name and/or the NUNIQ column name with the ``name`` and
-        ``uname`` arguments respectively.
+        ``uname`` arguments respectively. If ``meta_compat`` is ``True``, drop
+        metadata keys that are added by ``ligo.skymap.io.fits.write_sky_map``
+        so they don't get duplicated.
         """
         from astropy.table import Table
 
         name = name or self.name or 'PIXELS'
-        t = Table([self.u, self.s], names=[uname, name], meta=self.meta)
+        filtered_keys = {
+            "PIXTYPE",
+            "ORDERING",
+            "COORDSYS",
+            "MOCORDER",
+            "INDXSCHM"
+        } if self.meta else set()
+        
+        meta = {k: v for k, v in self.meta.items()
+                if k not in filtered_keys}
+
         for pt in self.point_sources:
-            cast(MutableMapping, t.meta).update(PointsTuple(*pt).meta_dict())
+            meta.update(PointsTuple(*pt).meta_dict())
+
+        t = Table([self.u, self.s], names=[uname, name], meta=meta)
         return t
 
     def write(
             self,
             file: Union[IO, str],
             *args,
             strategy: str = 'basic',
@@ -717,15 +737,15 @@
         """
         import numpy as np
 
         nside = nside or uniq2nside(self.u.max())
         sᵒ = fill(self.u, self.s, nside, pad=pad)
         if not as_skymap:
             return sᵒ
-        m = self.meta.copy()
+        m = self._meta_copy()
         m['HISTORY'] = (m.get('HISTORY', []) +
                         [f'Filled to NEST, NSIDE={nside}.'])
         return PartialUniqSkymap(sᵒ, np.arange(4*nside**2, 16*nside**2),
                                  copy=False, meta=m,
                                  point_sources=self.point_sources)
 
     def quantiles(
@@ -788,15 +808,15 @@
 
         quantiles_arr = np.asarray(quantiles, dtype=np.float_)
         indices, levels, norm = nside_quantile_indices(self.nside(), self.s,
                                                        quantiles_arr)
 
         def skymaps():
             for i, l, u in zip(indices, quantiles_arr[:-1], quantiles_arr[1:]):
-                m = self.meta.copy()
+                m = self._meta_copy()
                 m['HISTORY'] = m.get('HISTORY', []) + wrap(
                     f'Downselected to [{l:.2g}, {u:.2g}] quantile '
                     f'({(u-l)*100:.2g}%) of {norm:.2g} ({norm*(u-l):.2g} ',
                     70
                 )
                 yield PartialUniqSkymap(self.s[i], self.u[i], copy=False,
                                         meta=m,
@@ -835,15 +855,15 @@
         UNIQ indices; order matters!**
 
         If you want to guarantee a copy on a view that you know is not copied,
         make a copy with the returned array.
         """
         import numpy as np
 
-        m = self.meta.copy()
+        m = self._meta_copy()
         repidx = repr(idx)
         msg = repidx if len(repidx) < 60 else repidx[:58]+'...'
         m['HISTORY'] = m.get('HISTORY', []) + [f'Got view: {msg}']
         s = np.atleast_1d(self.s[idx])
         u = np.atleast_1d(self.u[idx])
         return type(self)(s, u, copy=False, meta=m,
                           point_sources=self.point_sources)
@@ -920,29 +940,29 @@
             Pixel values at locations specified in ``u⃗ᵒ``. If ``u⃗ᵒ`` is a
             ``WCS`` instance, then values outside of the projection will be
             set to ``np.nan``.
         """
         return render(self.u, self.s, u⃗ᵒ, pad=pad, valid=valid,
                       mask_missing=mask_missing)
 
-    def reraster(self, u_out, pad=None, mask_missing=False, copy=True):
+    def reraster(self, u_out, pad=None, mask_missing=False, copy=True, **kwargs):
         """
         Return a new ``PartialUniqSkymap`` instance with the same pixel values
         rerasterized to match the output NUNIQ indices ``u_out``. Fill in missing
         values in the output skymap with ``pad``. If ``pad`` is not provided
         and this skymap does not cover the full region defined in ``u_out``,
         raises a ``ValueError``. Preserves ``astropy.units.Unit`` of this
         skymap's pixel values (if ``s`` is an ``astropy.units.Quantity``). If
         ``copy`` is ``False``, use ``u_out`` as the indices of the new skymap;
         otherwise, use a copy.
         """
         import numpy as np
 
-        s_out = reraster(self.u, self.s, u_out, pad=pad, mask_missing=mask_missing)
-        m = self.meta.copy()
+        s_out = reraster(self.u, self.s, u_out, pad=pad, mask_missing=mask_missing, **kwargs)
+        m = self._meta_copy()
         m['HISTORY'] = m.get('HISTORY', []) + ['Rerasterized.']
         return PartialUniqSkymap(s_out, np.array(u_out, copy=copy), copy=False,
                                  meta=m, point_sources=self.point_sources)
 
     def coords(self):
         """
         Get the sky coordinates (right-ascension and declination, ICRS)
```

### Comparing `hpmoc-1.0a3/hpmoc/plot.py` & `hpmoc-1.0a4/hpmoc/plot.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a3/hpmoc/plotters.py` & `hpmoc-1.0a4/hpmoc/plotters.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a3/hpmoc/points.py` & `hpmoc-1.0a4/hpmoc/points.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a3/hpmoc/psf.py` & `hpmoc-1.0a4/hpmoc/psf.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a3/hpmoc/utils.py` & `hpmoc-1.0a4/hpmoc/utils.py`

 * *Files identical despite different names*

```diff
@@ -40,14 +40,15 @@
 from textwrap import wrap, dedent
 import logging
 import gzip
 from tempfile import NamedTemporaryFile
 import binascii
 from .healpy_utils import alt_compress, alt_expand
 from .healpy import healpy as hp
+from .arraysetops import intersect1d
 
 import numpy as np
 from numpy.typing import NDArray, ArrayLike, DTypeLike
 
 Int = Union[int, 'np.integer[Any]']
 IntArray = NDArray['np.integer[Any]']
 
@@ -818,15 +819,14 @@
     r /= norm
     j = r.searchsorted(q)
     l = j.copy()
     l[l >= len(i)] = len(i) - 1
     return ((i[ll:u] for ll, u in zip(j[:-1], j[1:])), skymap[i[l]],
             norm*np.pi/3)
 
-
 def uniq_intersection(u1: IntArray, u2: IntArray) -> Tuple[IntArray, IntArray, IntArray]:
     """Downselect the pixel indices given in ``u1`` to the set that
     overlaps with pixels in ``u2`` and return pairs of indices into
     both of the input index lists showing which pixel in ``u2`` each
     downselected pixel from ``u1`` overlaps with. Use this to get rid of
     pixels outside of a given region, or alternatively use it as part of a
     calculation involving two multi-resolution skymaps whose pixel sizes are
@@ -892,22 +892,22 @@
         raise ValueError("`u2` must be unique and non-overlapping.")
 
     ζ = 0
     i⃗ᶠ = [np.ndarray((len(uˢ[0])+len(uˢ[1]),), dtype=int) for _ in [0, 1]]
     δo = np.zeros_like(i⃗ᶠ[0], dtype=int)
 
     for s in reversed(range(len(s⃗[0]))):  # pylint: disable=invalid-name
-        _, *e = np.intersect1d(v⃗[0][s], v⃗[1][s], return_indices=True)
+        _, *e = intersect1d(v⃗[0][s], v⃗[1][s], return_indices=True, assume_unique=(True, True))
         for i in (0, 1):                 
             i⃗ᶠ[i][ζ:ζ+len(e[i])] = e[i] + s⃗[i][s].start # offset by slice start and put in result array
             if s < len(s⃗[0])-1:                          # coarsen high res
                 uˢ[i][s⃗[i][s].stop:] >>= 2*(o⃗[s+1]-o⃗[s])
         ζ += len(e[0])  # offset for array insertions
         for i, j in [(0, 1), (1, 0)]:
-            ρ⃗ = np.intersect1d(v⃗[i][s], uˢ[i][s⃗[i][s].stop:])
+            ρ⃗ = intersect1d(v⃗[i][s], uˢ[i][s⃗[i][s].stop:], assume_unique=(True, False))
             if len(ρ⃗):  # pylint: disable=len-as-condition
                 raise ValueError(f"`i⃗{i}` has pixels overlapping with "
                                  f"themselves at NUNIQ pixel indices {ρ⃗}")
             if len(v⃗[i][s]) == 0:  # pylint: disable=len-as-condition
                 continue                                # skip empty same res
             for sⱼ in reversed(range(s+1, len(s⃗[0]))):
                 ϵ⃗ʲ = np.searchsorted(v⃗[i][s], v⃗[j][sⱼ])
```

### Comparing `hpmoc-1.0a3/pyproject.toml` & `hpmoc-1.0a4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,16 @@
 [project.optional-dependencies]
 jup = ["jupyter", "ipython"]
 test = [
     "pytest",
     "pytest-cov",
     "h5py",
     "PyYAML",
-    "mhealpy"
+    "mhealpy",
+    "ligo.skymap"
 ]
 dev = [
     "flit",
     "sphinx",
     "sphinx_rtd_theme",
     "nbsphinx",
     "astroquery",
```

### Comparing `hpmoc-1.0a3/PKG-INFO` & `hpmoc-1.0a4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpmoc
-Version: 1.0a3
+Version: 1.0a4
 Summary: HPMOC is an ultra high-performance, cross-platform toolset for working with
 Author-email: Stefan Trklja Countryman <stefan.countryman@gmail.com>
 Maintainer-email: Albert Zhang <alchzh@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: IPython
@@ -36,14 +36,15 @@
 Requires-Dist: jupyter ; extra == "jup"
 Requires-Dist: ipython ; extra == "jup"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: h5py ; extra == "test"
 Requires-Dist: PyYAML ; extra == "test"
 Requires-Dist: mhealpy ; extra == "test"
+Requires-Dist: ligo.skymap ; extra == "test"
 Project-URL: Documentation, https://hpmoc.stc.sh/
 Project-URL: Homepage, https://github.com/markalab/hpmoc
 Project-URL: Repository, https://github.com/markalab/hpmoc.git
 Provides-Extra: astroquery
 Provides-Extra: dev
 Provides-Extra: gracedb
 Provides-Extra: healpy
```

