# Comparing `tmp/hpmoc-1.0a4.tar.gz` & `tmp/hpmoc-1.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hpmoc-1.0a4.tar", last modified: Thu Jul 13 23:02:26 2023, max compression
+gzip compressed data, was "hpmoc-1.0a5.tar", last modified: Thu Jul 13 23:20:06 2023, max compression
```

## Comparing `hpmoc-1.0a4.tar` & `hpmoc-1.0a5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    18092 2023-07-03 06:59:36.334737 hpmoc-1.0a4/LICENSE
--rw-r--r--   0        0        0     2549 2022-12-23 19:45:53.082596 hpmoc-1.0a4/Makefile
--rw-r--r--   0        0        0     3301 2023-07-03 19:52:28.451592 hpmoc-1.0a4/README.md
--rw-r--r--   0        0        0       25 2022-12-23 19:45:53.082596 hpmoc-1.0a4/docs/.gitignore
--rw-r--r--   0        0        0      638 2022-12-23 19:45:53.082596 hpmoc-1.0a4/docs/Makefile
--rw-r--r--   0        0        0      804 2022-12-23 19:45:53.082596 hpmoc-1.0a4/docs/make.bat
--rw-r--r--   0        0        0     6203 2022-12-23 19:45:53.082596 hpmoc-1.0a4/docs/source/conf.py
--rw-r--r--   0        0        0     3842 2022-12-23 19:45:53.082596 hpmoc-1.0a4/docs/source/index.rst
--rw-r--r--   0        0        0    40825 2022-12-23 19:45:53.082596 hpmoc-1.0a4/docs/source/jup/plotting-examples.ipynb
--rw-r--r--   0        0        0      521 2023-07-03 19:32:25.161624 hpmoc-1.0a4/hpmoc-dev-win.yml
--rw-r--r--   0        0        0      562 2023-07-03 19:32:25.161624 hpmoc-1.0a4/hpmoc-dev.yml
--rw-r--r--   0        0        0     1032 2023-07-13 23:00:13.150068 hpmoc-1.0a4/hpmoc/__init__.py
--rw-r--r--   0        0        0     1143 2023-07-03 19:43:54.661628 hpmoc-1.0a4/hpmoc/abstract.py
--rw-r--r--   0        0        0     6201 2023-07-07 05:29:37.570077 hpmoc-1.0a4/hpmoc/arraysetops.py
--rw-r--r--   0        0        0     5992 2023-07-03 19:39:12.181616 hpmoc-1.0a4/hpmoc/healpy.py
--rw-r--r--   0        0        0     2434 2023-07-03 19:43:58.561626 hpmoc-1.0a4/hpmoc/healpy_utils.py
--rw-r--r--   0        0        0     6949 2023-07-03 21:54:38.341626 hpmoc-1.0a4/hpmoc/io/__init__.py
--rw-r--r--   0        0        0     2279 2023-07-03 20:49:43.901611 hpmoc-1.0a4/hpmoc/io/abstract.py
--rw-r--r--   0        0        0     3297 2023-07-03 20:50:42.731624 hpmoc-1.0a4/hpmoc/io/astroquery.py
--rw-r--r--   0        0        0    12349 2023-07-03 20:42:44.021630 hpmoc-1.0a4/hpmoc/io/fits.py
--rw-r--r--   0        0        0     4849 2023-07-03 20:50:34.541623 hpmoc-1.0a4/hpmoc/io/gracedb.py
--rw-r--r--   0        0        0     3394 2023-07-03 20:16:09.031605 hpmoc-1.0a4/hpmoc/io/ligo.py
--rw-r--r--   0        0        0    54606 2023-07-13 22:46:35.890064 hpmoc-1.0a4/hpmoc/partial.py
--rw-r--r--   0        0        0    56536 2023-07-03 20:42:18.371588 hpmoc-1.0a4/hpmoc/plot.py
--rw-r--r--   0        0        0    36795 2023-07-03 19:44:32.571620 hpmoc-1.0a4/hpmoc/plotters.py
--rw-r--r--   0        0        0    12325 2023-07-03 19:44:44.001626 hpmoc-1.0a4/hpmoc/points.py
--rw-r--r--   0        0        0     3721 2023-07-03 19:44:52.571626 hpmoc-1.0a4/hpmoc/psf.py
--rw-r--r--   0        0        0    93078 2023-07-07 05:26:12.900078 hpmoc-1.0a4/hpmoc/utils.py
--rw-r--r--   0        0        0     1768 2023-07-13 22:48:45.670065 hpmoc-1.0a4/pyproject.toml
--rw-r--r--   0        0        0     5458 1970-01-01 00:00:00.000000 hpmoc-1.0a4/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-07-03 06:59:36.334737 hpmoc-1.0a5/LICENSE
+-rw-r--r--   0        0        0     2549 2022-12-23 19:45:53.082596 hpmoc-1.0a5/Makefile
+-rw-r--r--   0        0        0     3301 2023-07-03 19:52:28.451592 hpmoc-1.0a5/README.md
+-rw-r--r--   0        0        0       25 2022-12-23 19:45:53.082596 hpmoc-1.0a5/docs/.gitignore
+-rw-r--r--   0        0        0      638 2022-12-23 19:45:53.082596 hpmoc-1.0a5/docs/Makefile
+-rw-r--r--   0        0        0      804 2022-12-23 19:45:53.082596 hpmoc-1.0a5/docs/make.bat
+-rw-r--r--   0        0        0     6203 2022-12-23 19:45:53.082596 hpmoc-1.0a5/docs/source/conf.py
+-rw-r--r--   0        0        0     3842 2022-12-23 19:45:53.082596 hpmoc-1.0a5/docs/source/index.rst
+-rw-r--r--   0        0        0    40825 2022-12-23 19:45:53.082596 hpmoc-1.0a5/docs/source/jup/plotting-examples.ipynb
+-rw-r--r--   0        0        0      521 2023-07-03 19:32:25.161624 hpmoc-1.0a5/hpmoc-dev-win.yml
+-rw-r--r--   0        0        0      562 2023-07-03 19:32:25.161624 hpmoc-1.0a5/hpmoc-dev.yml
+-rw-r--r--   0        0        0     1032 2023-07-13 23:19:20.730072 hpmoc-1.0a5/hpmoc/__init__.py
+-rw-r--r--   0        0        0     1143 2023-07-03 19:43:54.661628 hpmoc-1.0a5/hpmoc/abstract.py
+-rw-r--r--   0        0        0     6201 2023-07-07 05:29:37.570077 hpmoc-1.0a5/hpmoc/arraysetops.py
+-rw-r--r--   0        0        0     5992 2023-07-03 19:39:12.181616 hpmoc-1.0a5/hpmoc/healpy.py
+-rw-r--r--   0        0        0     2434 2023-07-03 19:43:58.561626 hpmoc-1.0a5/hpmoc/healpy_utils.py
+-rw-r--r--   0        0        0     6949 2023-07-03 21:54:38.341626 hpmoc-1.0a5/hpmoc/io/__init__.py
+-rw-r--r--   0        0        0     2279 2023-07-03 20:49:43.901611 hpmoc-1.0a5/hpmoc/io/abstract.py
+-rw-r--r--   0        0        0     3297 2023-07-03 20:50:42.731624 hpmoc-1.0a5/hpmoc/io/astroquery.py
+-rw-r--r--   0        0        0    12349 2023-07-03 20:42:44.021630 hpmoc-1.0a5/hpmoc/io/fits.py
+-rw-r--r--   0        0        0     4849 2023-07-03 20:50:34.541623 hpmoc-1.0a5/hpmoc/io/gracedb.py
+-rw-r--r--   0        0        0     3394 2023-07-03 20:16:09.031605 hpmoc-1.0a5/hpmoc/io/ligo.py
+-rw-r--r--   0        0        0    54608 2023-07-13 23:18:30.270072 hpmoc-1.0a5/hpmoc/partial.py
+-rw-r--r--   0        0        0    56536 2023-07-03 20:42:18.371588 hpmoc-1.0a5/hpmoc/plot.py
+-rw-r--r--   0        0        0    36795 2023-07-03 19:44:32.571620 hpmoc-1.0a5/hpmoc/plotters.py
+-rw-r--r--   0        0        0    12325 2023-07-03 19:44:44.001626 hpmoc-1.0a5/hpmoc/points.py
+-rw-r--r--   0        0        0     3721 2023-07-03 19:44:52.571626 hpmoc-1.0a5/hpmoc/psf.py
+-rw-r--r--   0        0        0    93078 2023-07-07 05:26:12.900078 hpmoc-1.0a5/hpmoc/utils.py
+-rw-r--r--   0        0        0     1768 2023-07-13 22:48:45.670065 hpmoc-1.0a5/pyproject.toml
+-rw-r--r--   0        0        0     5458 1970-01-01 00:00:00.000000 hpmoc-1.0a5/PKG-INFO
```

### Comparing `hpmoc-1.0a4/LICENSE` & `hpmoc-1.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a4/Makefile` & `hpmoc-1.0a5/Makefile`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a4/README.md` & `hpmoc-1.0a5/README.md`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a4/docs/Makefile` & `hpmoc-1.0a5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a4/docs/make.bat` & `hpmoc-1.0a5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a4/docs/source/conf.py` & `hpmoc-1.0a5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a4/docs/source/index.rst` & `hpmoc-1.0a5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a4/docs/source/jup/plotting-examples.ipynb` & `hpmoc-1.0a5/docs/source/jup/plotting-examples.ipynb`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a4/hpmoc-dev-win.yml` & `hpmoc-1.0a5/hpmoc-dev-win.yml`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a4/hpmoc-dev.yml` & `hpmoc-1.0a5/hpmoc-dev.yml`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a4/hpmoc/__init__.py` & `hpmoc-1.0a5/hpmoc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,10 +16,10 @@
 
 """
 HPMOC is an ultra high-performance, cross-platform toolset for working with
 multi-order coordinate (MOC) HEALPix images (i.e. images with multiple pixel
 resolutions).
 """
 
-__version__ = '1.0a4'
+__version__ = '1.0a5'
 
 from .partial import PartialUniqSkymap as PartialUniqSkymap
```

### Comparing `hpmoc-1.0a4/hpmoc/abstract.py` & `hpmoc-1.0a5/hpmoc/abstract.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a4/hpmoc/arraysetops.py` & `hpmoc-1.0a5/hpmoc/arraysetops.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a4/hpmoc/healpy.py` & `hpmoc-1.0a5/hpmoc/healpy.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a4/hpmoc/healpy_utils.py` & `hpmoc-1.0a5/hpmoc/healpy_utils.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a4/hpmoc/io/__init__.py` & `hpmoc-1.0a5/hpmoc/io/__init__.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a4/hpmoc/io/abstract.py` & `hpmoc-1.0a5/hpmoc/io/abstract.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a4/hpmoc/io/astroquery.py` & `hpmoc-1.0a5/hpmoc/io/astroquery.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a4/hpmoc/io/fits.py` & `hpmoc-1.0a5/hpmoc/io/fits.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a4/hpmoc/io/gracedb.py` & `hpmoc-1.0a5/hpmoc/io/gracedb.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a4/hpmoc/io/ligo.py` & `hpmoc-1.0a5/hpmoc/io/ligo.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a4/hpmoc/partial.py` & `hpmoc-1.0a5/hpmoc/partial.py`

 * *Files 0% similar despite different names*

```diff
@@ -603,15 +603,15 @@
         name = name or self.name or 'PIXELS'
         filtered_keys = {
             "PIXTYPE",
             "ORDERING",
             "COORDSYS",
             "MOCORDER",
             "INDXSCHM"
-        } if self.meta else set()
+        } if meta_compat else set()
         
         meta = {k: v for k, v in self.meta.items()
                 if k not in filtered_keys}
 
         for pt in self.point_sources:
             meta.update(PointsTuple(*pt).meta_dict())
```

### Comparing `hpmoc-1.0a4/hpmoc/plot.py` & `hpmoc-1.0a5/hpmoc/plot.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a4/hpmoc/plotters.py` & `hpmoc-1.0a5/hpmoc/plotters.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a4/hpmoc/points.py` & `hpmoc-1.0a5/hpmoc/points.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a4/hpmoc/psf.py` & `hpmoc-1.0a5/hpmoc/psf.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a4/hpmoc/utils.py` & `hpmoc-1.0a5/hpmoc/utils.py`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a4/pyproject.toml` & `hpmoc-1.0a5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hpmoc-1.0a4/PKG-INFO` & `hpmoc-1.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpmoc
-Version: 1.0a4
+Version: 1.0a5
 Summary: HPMOC is an ultra high-performance, cross-platform toolset for working with
 Author-email: Stefan Trklja Countryman <stefan.countryman@gmail.com>
 Maintainer-email: Albert Zhang <alchzh@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: IPython
```

