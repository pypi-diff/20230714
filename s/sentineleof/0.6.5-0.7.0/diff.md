# Comparing `tmp/sentineleof-0.6.5.tar.gz` & `tmp/sentineleof-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentineleof-0.6.5.tar", last modified: Wed Dec  7 21:13:43 2022, max compression
+gzip compressed data, was "sentineleof-0.7.0.tar", last modified: Thu Jul 13 22:08:22 2023, max compression
```

## Comparing `sentineleof-0.6.5.tar` & `sentineleof-0.7.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 21:13:43.669817 sentineleof-0.6.5/
--rw-r--r--   0 runner    (1001) docker     (122)     1079 2022-12-07 21:13:33.000000 sentineleof-0.6.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)     3078 2022-12-07 21:13:43.669817 sentineleof-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2289 2022-12-07 21:13:33.000000 sentineleof-0.6.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 21:13:43.665817 sentineleof-0.6.5/eof/
--rw-r--r--   0 runner    (1001) docker     (122)       45 2022-12-07 21:13:33.000000 sentineleof-0.6.5/eof/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       76 2022-12-07 21:13:33.000000 sentineleof-0.6.5/eof/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1996 2022-12-07 21:13:33.000000 sentineleof-0.6.5/eof/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     8741 2022-12-07 21:13:33.000000 sentineleof-0.6.5/eof/download.py
--rw-r--r--   0 runner    (1001) docker     (122)      426 2022-12-07 21:13:33.000000 sentineleof-0.6.5/eof/log.py
--rw-r--r--   0 runner    (1001) docker     (122)     4307 2022-12-07 21:13:33.000000 sentineleof-0.6.5/eof/parsing.py
--rw-r--r--   0 runner    (1001) docker     (122)    14181 2022-12-07 21:13:33.000000 sentineleof-0.6.5/eof/products.py
--rw-r--r--   0 runner    (1001) docker     (122)    11312 2022-12-07 21:13:33.000000 sentineleof-0.6.5/eof/scihubclient.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 21:13:43.665817 sentineleof-0.6.5/eof/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-07 21:13:33.000000 sentineleof-0.6.5/eof/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6602 2022-12-07 21:13:33.000000 sentineleof-0.6.5/eof/tests/test_eof.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-07 21:13:43.669817 sentineleof-0.6.5/sentineleof.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3078 2022-12-07 21:13:43.000000 sentineleof-0.6.5/sentineleof.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      441 2022-12-07 21:13:43.000000 sentineleof-0.6.5/sentineleof.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-07 21:13:43.000000 sentineleof-0.6.5/sentineleof.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       36 2022-12-07 21:13:43.000000 sentineleof-0.6.5/sentineleof.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-07 21:13:43.000000 sentineleof-0.6.5/sentineleof.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       48 2022-12-07 21:13:43.000000 sentineleof-0.6.5/sentineleof.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        4 2022-12-07 21:13:43.000000 sentineleof-0.6.5/sentineleof.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-07 21:13:43.669817 sentineleof-0.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1260 2022-12-07 21:13:33.000000 sentineleof-0.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:08:22.360398 sentineleof-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-13 22:08:11.000000 sentineleof-0.7.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-13 22:08:22.360398 sentineleof-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-07-13 22:08:11.000000 sentineleof-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:08:22.356398 sentineleof-0.7.0/eof/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-13 22:08:11.000000 sentineleof-0.7.0/eof/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-13 22:08:11.000000 sentineleof-0.7.0/eof/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-13 22:08:11.000000 sentineleof-0.7.0/eof/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8741 2023-07-13 22:08:11.000000 sentineleof-0.7.0/eof/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-13 22:08:11.000000 sentineleof-0.7.0/eof/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-13 22:08:11.000000 sentineleof-0.7.0/eof/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14181 2023-07-13 22:08:11.000000 sentineleof-0.7.0/eof/products.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11536 2023-07-13 22:08:11.000000 sentineleof-0.7.0/eof/scihubclient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:08:22.356398 sentineleof-0.7.0/eof/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 22:08:11.000000 sentineleof-0.7.0/eof/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-07-13 22:08:11.000000 sentineleof-0.7.0/eof/tests/test_eof.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:08:22.360398 sentineleof-0.7.0/sentineleof.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-13 22:08:22.000000 sentineleof-0.7.0/sentineleof.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-13 22:08:22.000000 sentineleof-0.7.0/sentineleof.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 22:08:22.000000 sentineleof-0.7.0/sentineleof.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-13 22:08:22.000000 sentineleof-0.7.0/sentineleof.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 22:08:22.000000 sentineleof-0.7.0/sentineleof.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-13 22:08:22.000000 sentineleof-0.7.0/sentineleof.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-13 22:08:22.000000 sentineleof-0.7.0/sentineleof.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 22:08:22.360398 sentineleof-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-13 22:08:11.000000 sentineleof-0.7.0/setup.py
```

### Comparing `sentineleof-0.6.5/LICENSE.txt` & `sentineleof-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sentineleof-0.6.5/PKG-INFO` & `sentineleof-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentineleof
-Version: 0.6.5
+Version: 0.7.0
 Summary: Download precise orbit files for Sentinel 1 products
 Home-page: https://github.com/scottstanie/sentineleof
 Author: Scott Staniewicz
 Author-email: scott.stanie@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `sentineleof-0.6.5/README.md` & `sentineleof-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `sentineleof-0.6.5/eof/cli.py` & `sentineleof-0.7.0/eof/cli.py`

 * *Files identical despite different names*

### Comparing `sentineleof-0.6.5/eof/download.py` & `sentineleof-0.7.0/eof/download.py`

 * *Files identical despite different names*

### Comparing `sentineleof-0.6.5/eof/parsing.py` & `sentineleof-0.7.0/eof/parsing.py`

 * *Files identical despite different names*

### Comparing `sentineleof-0.6.5/eof/products.py` & `sentineleof-0.7.0/eof/products.py`

 * *Files identical despite different names*

### Comparing `sentineleof-0.6.5/eof/scihubclient.py` & `sentineleof-0.7.0/eof/scihubclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,18 +17,23 @@
 
 
 class ValidityError(ValueError):
     pass
 
 
 def lastval_cover(
-    t0: datetime.datetime, t1: datetime.datetime, data: Sequence[SentinelOrbit]
+    t0: datetime.datetime,
+    t1: datetime.datetime,
+    data: Sequence[SentinelOrbit],
+    margin: datetime.timedelta = datetime.timedelta(minutes=5),
 ) -> str:
     candidates = [
-        item for item in data if item.start_time <= t0 and item.stop_time >= t1
+        item
+        for item in data
+        if item.start_time <= (t0 - margin) and item.stop_time >= (t1 + margin)
     ]
     if not candidates:
         raise ValidityError(
             "none of the input products completely covers the requested "
             "time interval: [t0={}, t1={}]".format(t0, t1)
         )
 
@@ -41,16 +46,21 @@
     pass
 
 
 class ScihubGnssClient:
     T0 = datetime.timedelta(days=1)
     T1 = datetime.timedelta(days=1)
 
-    def __init__(self, user: str = "gnssguest", password: str = "gnssguest",
-                 api_url: str = "https://scihub.copernicus.eu/gnss/", **kwargs):
+    def __init__(
+        self,
+        user: str = "gnssguest",
+        password: str = "gnssguest",
+        api_url: str = "https://scihub.copernicus.eu/gnss/",
+        **kwargs
+    ):
         self._api = SentinelAPI(user=user, password=password, api_url=api_url, **kwargs)
 
     def query_orbit(self, t0, t1, satellite_id: str, product_type: str = "AUX_POEORB"):
         assert satellite_id in {"S1A", "S1B"}
         assert product_type in {"AUX_POEORB", "AUX_RESORB"}
 
         query_params = dict(
@@ -125,15 +135,17 @@
                 products = self.query_orbit(
                     dt - t0_margin,
                     dt + t1_margin,
                     mission,
                     product_type="AUX_POEORB",
                 )
                 try:
-                    result = self._select_orbit(products, dt, dt + datetime.timedelta(minutes=1))
+                    result = self._select_orbit(
+                        products, dt, dt + datetime.timedelta(minutes=1)
+                    )
                 except ValidityError:
                     result = None
             else:
                 result = None
 
             if result:
                 found_result = True
@@ -206,15 +218,17 @@
         # Try to see if we have the list of EOFs in the cache
         elif os.path.exists(self._get_filename_cache_path(orbit_type)):
             eof_list = self._get_cached_filenames(orbit_type)
             # Need to clear it if it's older than what we're looking for
             max_saved = max([e.start_time for e in eof_list])
             if max_saved < max_dt:
                 logger.warning("Clearing cached {} EOF list:".format(orbit_type))
-                logger.warning("{} is older than requested {}".format(max_saved, max_dt))
+                logger.warning(
+                    "{} is older than requested {}".format(max_saved, max_dt)
+                )
                 self._clear_cache(orbit_type)
             else:
                 logger.info("Using cached EOF list")
                 self.eof_lists[orbit_type] = eof_list
                 return eof_list
 
         logger.info("Downloading all filenames from ASF (may take awhile)")
```

### Comparing `sentineleof-0.6.5/eof/tests/test_eof.py` & `sentineleof-0.7.0/eof/tests/test_eof.py`

 * *Files identical despite different names*

### Comparing `sentineleof-0.6.5/sentineleof.egg-info/PKG-INFO` & `sentineleof-0.7.0/sentineleof.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentineleof
-Version: 0.6.5
+Version: 0.7.0
 Summary: Download precise orbit files for Sentinel 1 products
 Home-page: https://github.com/scottstanie/sentineleof
 Author: Scott Staniewicz
 Author-email: scott.stanie@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `sentineleof-0.6.5/setup.py` & `sentineleof-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sentineleof",
-    version="0.6.5",
+    version="0.7.0",
     author="Scott Staniewicz",
     author_email="scott.stanie@gmail.com",
     description="Download precise orbit files for Sentinel 1 products",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/scottstanie/sentineleof",
     packages=setuptools.find_packages(),
```

