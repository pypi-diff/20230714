# Comparing `tmp/modis_tools-1.1.0.tar.gz` & `tmp/modis_tools-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modis_tools-1.1.0.tar", last modified: Fri Sep 16 21:20:23 2022, max compression
+gzip compressed data, was "modis_tools-1.1.1.tar", last modified: Fri Jul 14 16:54:43 2023, max compression
```

## Comparing `modis_tools-1.1.0.tar` & `modis_tools-1.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 shengpeiwang   (503) staff       (20)        0 2022-09-16 21:20:23.704808 modis_tools-1.1.0/
--rw-r--r--   0 shengpeiwang   (503) staff       (20)    10141 2022-02-28 19:41:52.000000 modis_tools-1.1.0/LICENSE
--rw-r--r--   0 shengpeiwang   (503) staff       (20)       25 2022-02-28 19:41:52.000000 modis_tools-1.1.0/MANIFEST.in
--rw-r--r--   0 shengpeiwang   (503) staff       (20)     9599 2022-09-16 21:20:23.704608 modis_tools-1.1.0/PKG-INFO
--rw-r--r--   0 shengpeiwang   (503) staff       (20)     9098 2022-02-28 19:41:52.000000 modis_tools-1.1.0/README.md
-drwxr-xr-x   0 shengpeiwang   (503) staff       (20)        0 2022-09-16 21:20:23.702040 modis_tools-1.1.0/modis_tools/
--rw-r--r--   0 shengpeiwang   (503) staff       (20)        0 2022-02-28 19:41:52.000000 modis_tools-1.1.0/modis_tools/__init__.py
--rw-r--r--   0 shengpeiwang   (503) staff       (20)     2414 2022-02-28 19:41:52.000000 modis_tools-1.1.0/modis_tools/api.py
--rw-r--r--   0 shengpeiwang   (503) staff       (20)     4022 2022-09-16 21:19:56.000000 modis_tools-1.1.0/modis_tools/auth.py
-drwxr-xr-x   0 shengpeiwang   (503) staff       (20)        0 2022-09-16 21:20:23.703354 modis_tools-1.1.0/modis_tools/constants/
--rw-r--r--   0 shengpeiwang   (503) staff       (20)        0 2022-02-28 19:41:52.000000 modis_tools-1.1.0/modis_tools/constants/__init__.py
--rw-r--r--   0 shengpeiwang   (503) staff       (20)      559 2022-02-28 19:41:52.000000 modis_tools-1.1.0/modis_tools/constants/mimetypes.py
--rw-r--r--   0 shengpeiwang   (503) staff       (20)      299 2022-09-13 15:43:46.000000 modis_tools-1.1.0/modis_tools/constants/urls.py
--rw-r--r--   0 shengpeiwang   (503) staff       (20)     1092 2022-02-28 19:41:52.000000 modis_tools-1.1.0/modis_tools/decorators.py
--rw-r--r--   0 shengpeiwang   (503) staff       (20)     7345 2022-09-16 21:19:56.000000 modis_tools-1.1.0/modis_tools/granule_handler.py
--rw-r--r--   0 shengpeiwang   (503) staff       (20)     2437 2022-09-13 15:43:46.000000 modis_tools-1.1.0/modis_tools/models.py
--rw-r--r--   0 shengpeiwang   (503) staff       (20)     8558 2022-02-28 19:41:52.000000 modis_tools-1.1.0/modis_tools/request_helpers.py
--rw-r--r--   0 shengpeiwang   (503) staff       (20)     4733 2022-09-16 21:19:56.000000 modis_tools-1.1.0/modis_tools/resources.py
-drwxr-xr-x   0 shengpeiwang   (503) staff       (20)        0 2022-09-16 21:20:23.702847 modis_tools-1.1.0/modis_tools.egg-info/
--rw-r--r--   0 shengpeiwang   (503) staff       (20)     9599 2022-09-16 21:20:23.000000 modis_tools-1.1.0/modis_tools.egg-info/PKG-INFO
--rw-r--r--   0 shengpeiwang   (503) staff       (20)      611 2022-09-16 21:20:23.000000 modis_tools-1.1.0/modis_tools.egg-info/SOURCES.txt
--rw-r--r--   0 shengpeiwang   (503) staff       (20)        1 2022-09-16 21:20:23.000000 modis_tools-1.1.0/modis_tools.egg-info/dependency_links.txt
--rw-r--r--   0 shengpeiwang   (503) staff       (20)      103 2022-09-16 21:20:23.000000 modis_tools-1.1.0/modis_tools.egg-info/requires.txt
--rw-r--r--   0 shengpeiwang   (503) staff       (20)       18 2022-09-16 21:20:23.000000 modis_tools-1.1.0/modis_tools.egg-info/top_level.txt
--rw-r--r--   0 shengpeiwang   (503) staff       (20)       74 2022-09-13 21:49:37.000000 modis_tools-1.1.0/requirements.txt
--rw-r--r--   0 shengpeiwang   (503) staff       (20)       38 2022-09-16 21:20:23.704861 modis_tools-1.1.0/setup.cfg
--rw-r--r--   0 shengpeiwang   (503) staff       (20)      916 2022-09-16 21:19:56.000000 modis_tools-1.1.0/setup.py
-drwxr-xr-x   0 shengpeiwang   (503) staff       (20)        0 2022-09-16 21:20:23.704350 modis_tools-1.1.0/tests/
--rw-r--r--   0 shengpeiwang   (503) staff       (20)        0 2022-02-28 19:41:52.000000 modis_tools-1.1.0/tests/__init__.py
--rw-r--r--   0 shengpeiwang   (503) staff       (20)     2422 2022-02-28 19:41:52.000000 modis_tools-1.1.0/tests/test_api.py
--rw-r--r--   0 shengpeiwang   (503) staff       (20)     3966 2022-02-28 19:41:52.000000 modis_tools-1.1.0/tests/test_auth.py
--rw-r--r--   0 shengpeiwang   (503) staff       (20)     6662 2022-02-28 19:41:52.000000 modis_tools-1.1.0/tests/test_request_helpers.py
+drwxr-xr-x   0 leith      (502) staff       (20)        0 2023-07-14 16:54:43.524702 modis_tools-1.1.1/
+-rw-r--r--   0 leith      (502) staff       (20)    10141 2023-07-14 16:52:13.000000 modis_tools-1.1.1/LICENSE
+-rw-r--r--   0 leith      (502) staff       (20)       25 2023-07-14 16:52:13.000000 modis_tools-1.1.1/MANIFEST.in
+-rw-r--r--   0 leith      (502) staff       (20)     9599 2023-07-14 16:54:43.523371 modis_tools-1.1.1/PKG-INFO
+-rw-r--r--   0 leith      (502) staff       (20)     9098 2023-07-14 16:52:13.000000 modis_tools-1.1.1/README.md
+drwxr-xr-x   0 leith      (502) staff       (20)        0 2023-07-14 16:54:43.520031 modis_tools-1.1.1/modis_tools/
+-rw-r--r--   0 leith      (502) staff       (20)        0 2023-07-14 16:52:13.000000 modis_tools-1.1.1/modis_tools/__init__.py
+-rw-r--r--   0 leith      (502) staff       (20)     2414 2023-07-14 16:52:13.000000 modis_tools-1.1.1/modis_tools/api.py
+-rw-r--r--   0 leith      (502) staff       (20)     4022 2023-07-14 16:52:13.000000 modis_tools-1.1.1/modis_tools/auth.py
+drwxr-xr-x   0 leith      (502) staff       (20)        0 2023-07-14 16:54:43.521755 modis_tools-1.1.1/modis_tools/constants/
+-rw-r--r--   0 leith      (502) staff       (20)        0 2023-07-14 16:52:13.000000 modis_tools-1.1.1/modis_tools/constants/__init__.py
+-rw-r--r--   0 leith      (502) staff       (20)      559 2023-07-14 16:52:13.000000 modis_tools-1.1.1/modis_tools/constants/mimetypes.py
+-rw-r--r--   0 leith      (502) staff       (20)      429 2023-07-14 16:52:13.000000 modis_tools-1.1.1/modis_tools/constants/urls.py
+-rw-r--r--   0 leith      (502) staff       (20)     1092 2023-07-14 16:52:13.000000 modis_tools-1.1.1/modis_tools/decorators.py
+-rw-r--r--   0 leith      (502) staff       (20)     7694 2023-07-14 16:52:13.000000 modis_tools-1.1.1/modis_tools/granule_handler.py
+-rw-r--r--   0 leith      (502) staff       (20)     2475 2023-07-14 16:52:13.000000 modis_tools-1.1.1/modis_tools/models.py
+-rw-r--r--   0 leith      (502) staff       (20)     8558 2023-07-14 16:52:13.000000 modis_tools-1.1.1/modis_tools/request_helpers.py
+-rw-r--r--   0 leith      (502) staff       (20)     4732 2023-07-14 16:52:13.000000 modis_tools-1.1.1/modis_tools/resources.py
+drwxr-xr-x   0 leith      (502) staff       (20)        0 2023-07-14 16:54:43.520925 modis_tools-1.1.1/modis_tools.egg-info/
+-rw-r--r--   0 leith      (502) staff       (20)     9599 2023-07-14 16:54:43.000000 modis_tools-1.1.1/modis_tools.egg-info/PKG-INFO
+-rw-r--r--   0 leith      (502) staff       (20)      611 2023-07-14 16:54:43.000000 modis_tools-1.1.1/modis_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 leith      (502) staff       (20)        1 2023-07-14 16:54:43.000000 modis_tools-1.1.1/modis_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 leith      (502) staff       (20)      103 2023-07-14 16:54:43.000000 modis_tools-1.1.1/modis_tools.egg-info/requires.txt
+-rw-r--r--   0 leith      (502) staff       (20)       18 2023-07-14 16:54:43.000000 modis_tools-1.1.1/modis_tools.egg-info/top_level.txt
+-rw-r--r--   0 leith      (502) staff       (20)       74 2023-07-14 16:52:13.000000 modis_tools-1.1.1/requirements.txt
+-rw-r--r--   0 leith      (502) staff       (20)       38 2023-07-14 16:54:43.524764 modis_tools-1.1.1/setup.cfg
+-rw-r--r--   0 leith      (502) staff       (20)      916 2023-07-14 16:54:00.000000 modis_tools-1.1.1/setup.py
+drwxr-xr-x   0 leith      (502) staff       (20)        0 2023-07-14 16:54:43.522580 modis_tools-1.1.1/tests/
+-rw-r--r--   0 leith      (502) staff       (20)        0 2023-07-14 16:52:13.000000 modis_tools-1.1.1/tests/__init__.py
+-rw-r--r--   0 leith      (502) staff       (20)     2422 2023-07-14 16:52:13.000000 modis_tools-1.1.1/tests/test_api.py
+-rw-r--r--   0 leith      (502) staff       (20)     3966 2023-07-14 16:52:13.000000 modis_tools-1.1.1/tests/test_auth.py
+-rw-r--r--   0 leith      (502) staff       (20)     6662 2023-07-14 16:52:13.000000 modis_tools-1.1.1/tests/test_request_helpers.py
```

### Comparing `modis_tools-1.1.0/LICENSE` & `modis_tools-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `modis_tools-1.1.0/PKG-INFO` & `modis_tools-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modis_tools
-Version: 1.1.0
+Version: 1.1.1
 Summary: Tools for working with the MODIS API and MODIS data.
 Home-page: https://github.com/fraymio/modis-tools.git
 Author: fraym
 Author-email: datascience@fraym.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
@@ -33,15 +33,15 @@
 password = ""  # Update this line
 
 # Authenticate a session
 session = ModisSession(username=username, password=password)
 
 # Query the MODIS catalog for collections
 collection_client = CollectionApi(session=session)
-collections = collection_client.query(short_name="MOD13A1", version="006")
+collections = collection_client.query(short_name="MOD13A1", version="061")
 
 # Query the selected collection for granules
 granule_client = GranuleApi.from_collection(collections[0], session=session)
 
 # Filter the selected granules via spatial and temporal parameters
 nigeria_bbox = [2.1448863675, 4.002583177, 15.289420717, 14.275061098]
 nigeria_granules = granule_client.query(start_date="2016-01-01", end_date="2018-12-31", bounding_box=nigeria_bbox)
@@ -106,15 +106,15 @@
 
 *Note: To specify a modifier for a parameter (eg. `parameter[option]`), you'll need to unpack it from a dictionary: `**{"parameter[option]": "value"}` rather than passing it directly as a keyword argument.*
 
 *Note: Response models for both classes' `query()` methods can be found in `modis_tools/models.py`.*
 
 ```python
 # Collections query returns a list of matching collections
-collections = collection_client.query(short_name="MOD13A1", version="006")
+collections = collection_client.query(short_name="MOD13A1", version="061")
 
 # Create a GranuleApi from a Collection, the `concept_id` search parameter is set
 # to the collection
 granule_client = GranuleApi.from_collection(collections[0])
 # Granules collection returns a generator with matching granules
 granules = granule_client.query(start_date="2019-02-02", limit=50)
 ```
```

### Comparing `modis_tools-1.1.0/README.md` & `modis_tools-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 password = ""  # Update this line
 
 # Authenticate a session
 session = ModisSession(username=username, password=password)
 
 # Query the MODIS catalog for collections
 collection_client = CollectionApi(session=session)
-collections = collection_client.query(short_name="MOD13A1", version="006")
+collections = collection_client.query(short_name="MOD13A1", version="061")
 
 # Query the selected collection for granules
 granule_client = GranuleApi.from_collection(collections[0], session=session)
 
 # Filter the selected granules via spatial and temporal parameters
 nigeria_bbox = [2.1448863675, 4.002583177, 15.289420717, 14.275061098]
 nigeria_granules = granule_client.query(start_date="2016-01-01", end_date="2018-12-31", bounding_box=nigeria_bbox)
@@ -90,15 +90,15 @@
 
 *Note: To specify a modifier for a parameter (eg. `parameter[option]`), you'll need to unpack it from a dictionary: `**{"parameter[option]": "value"}` rather than passing it directly as a keyword argument.*
 
 *Note: Response models for both classes' `query()` methods can be found in `modis_tools/models.py`.*
 
 ```python
 # Collections query returns a list of matching collections
-collections = collection_client.query(short_name="MOD13A1", version="006")
+collections = collection_client.query(short_name="MOD13A1", version="061")
 
 # Create a GranuleApi from a Collection, the `concept_id` search parameter is set
 # to the collection
 granule_client = GranuleApi.from_collection(collections[0])
 # Granules collection returns a generator with matching granules
 granules = granule_client.query(start_date="2019-02-02", limit=50)
 ```
```

### Comparing `modis_tools-1.1.0/modis_tools/api.py` & `modis_tools-1.1.1/modis_tools/api.py`

 * *Files identical despite different names*

### Comparing `modis_tools-1.1.0/modis_tools/auth.py` & `modis_tools-1.1.1/modis_tools/auth.py`

 * *Files identical despite different names*

### Comparing `modis_tools-1.1.0/modis_tools/constants/mimetypes.py` & `modis_tools-1.1.1/modis_tools/constants/mimetypes.py`

 * *Files identical despite different names*

### Comparing `modis_tools-1.1.0/modis_tools/decorators.py` & `modis_tools-1.1.1/modis_tools/decorators.py`

 * *Files identical despite different names*

### Comparing `modis_tools-1.1.0/modis_tools/granule_handler.py` & `modis_tools-1.1.1/modis_tools/granule_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -97,14 +97,16 @@
     @staticmethod
     def get_url_from_granule(granule: Granule, ext: ParamType = "hdf") -> HttpUrl:
         """Return link for file extension from Earthdata resource."""
         for link in granule.links:
             if link.href.host in [
                 URLs.RESOURCE.value,
                 URLs.NSIDC_RESOURCE.value,
+                URLs.MOD11A2_V061_RESOURCE.value,
+                URLs.LAADS_RESOURCE.value,
             ] and link.href.path.endswith(ext):
                 return link.href
         raise Exception("No matching link found")
 
     @classmethod
     def download_from_urls(
         cls,
@@ -171,19 +173,23 @@
 
     @staticmethod
     def _get_location(url: HttpUrl, modis_session: ModisSession) -> str:
         """Make initial request to fetch file location from header."""
         session = modis_session.session
         split_result = urlsplit(url)
         https_url = split_result._replace(scheme="https").geturl()
-        location_resp = session.get(https_url, allow_redirects=False)
-        if location_resp.status_code == 401:
-            # try using ProxyAuth if BasicAuth returns 401 (unauthorized)
-            location_resp = session.get(
-                https_url,
-                allow_redirects=False,
-                auth=HTTPProxyAuth(modis_session.username, modis_session.password),
-            )
-        location = location_resp.headers.get("Location")
+        if url.host == URLs.LAADS_RESOURCE.value:
+            location_resp = session.get(https_url, allow_redirects=True)
+            location = location_resp.url # ends up being the same as https_url
+        else:    
+            location_resp = session.get(https_url, allow_redirects=False)
+            if location_resp.status_code == 401:
+                # try using ProxyAuth if BasicAuth returns 401 (unauthorized)
+                location_resp = session.get(
+                    https_url,
+                    allow_redirects=False,
+                    auth=HTTPProxyAuth(modis_session.username, modis_session.password),
+                )
+            location = location_resp.headers.get("Location")
         if not location:
             raise FileNotFoundError("No file location found")
         return location
```

### Comparing `modis_tools-1.1.0/modis_tools/models.py` & `modis_tools-1.1.1/modis_tools/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """ Return classes from API requests. """
 
 from datetime import datetime
 from typing import List, Optional
 
-from pydantic import BaseModel, HttpUrl
+from pydantic import BaseModel, HttpUrl, AnyUrl
 
 
 # Shared structure
 class ApiLink(BaseModel):
     rel: HttpUrl
     hreflang: str
-    href: HttpUrl
+    href: AnyUrl
+    type: Optional[str] = None
 
     @property
     def rel(self, val: str) -> str:
         """Remove trailing hashes before validating."""
         return val.rstrip("#")
```

### Comparing `modis_tools-1.1.0/modis_tools/request_helpers.py` & `modis_tools-1.1.1/modis_tools/request_helpers.py`

 * *Files identical despite different names*

### Comparing `modis_tools-1.1.0/modis_tools/resources.py` & `modis_tools-1.1.1/modis_tools/resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from typing import Any, Iterator, List, Optional
 
 from .api import ModisApi, Sessions
 from .decorators import params_args
 from .models import Collection, CollectionFeed, Granule, GranuleFeed
 from .request_helpers import DateParams, SpatialQuery
 
-
 class CollectionApi(ModisApi):
     """API for MODIS's 'collections' resource"""
 
     resource: str = "collections"
 
     def __init__(
         self,
```

### Comparing `modis_tools-1.1.0/modis_tools.egg-info/PKG-INFO` & `modis_tools-1.1.1/modis_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modis-tools
-Version: 1.1.0
+Version: 1.1.1
 Summary: Tools for working with the MODIS API and MODIS data.
 Home-page: https://github.com/fraymio/modis-tools.git
 Author: fraym
 Author-email: datascience@fraym.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
@@ -33,15 +33,15 @@
 password = ""  # Update this line
 
 # Authenticate a session
 session = ModisSession(username=username, password=password)
 
 # Query the MODIS catalog for collections
 collection_client = CollectionApi(session=session)
-collections = collection_client.query(short_name="MOD13A1", version="006")
+collections = collection_client.query(short_name="MOD13A1", version="061")
 
 # Query the selected collection for granules
 granule_client = GranuleApi.from_collection(collections[0], session=session)
 
 # Filter the selected granules via spatial and temporal parameters
 nigeria_bbox = [2.1448863675, 4.002583177, 15.289420717, 14.275061098]
 nigeria_granules = granule_client.query(start_date="2016-01-01", end_date="2018-12-31", bounding_box=nigeria_bbox)
@@ -106,15 +106,15 @@
 
 *Note: To specify a modifier for a parameter (eg. `parameter[option]`), you'll need to unpack it from a dictionary: `**{"parameter[option]": "value"}` rather than passing it directly as a keyword argument.*
 
 *Note: Response models for both classes' `query()` methods can be found in `modis_tools/models.py`.*
 
 ```python
 # Collections query returns a list of matching collections
-collections = collection_client.query(short_name="MOD13A1", version="006")
+collections = collection_client.query(short_name="MOD13A1", version="061")
 
 # Create a GranuleApi from a Collection, the `concept_id` search parameter is set
 # to the collection
 granule_client = GranuleApi.from_collection(collections[0])
 # Granules collection returns a generator with matching granules
 granules = granule_client.query(start_date="2019-02-02", limit=50)
 ```
```

### Comparing `modis_tools-1.1.0/modis_tools.egg-info/SOURCES.txt` & `modis_tools-1.1.1/modis_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modis_tools-1.1.0/setup.py` & `modis_tools-1.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     install_requires = fh.read().split()
 
 setuptools.setup(
     name="modis_tools",
-    version="1.1.0",
+    version="1.1.1",
     author="fraym",
     author_email="datascience@fraym.io",
     description="Tools for working with the MODIS API and MODIS data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/fraymio/modis-tools.git",
     packages=setuptools.find_packages(),
```

### Comparing `modis_tools-1.1.0/tests/test_api.py` & `modis_tools-1.1.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `modis_tools-1.1.0/tests/test_auth.py` & `modis_tools-1.1.1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `modis_tools-1.1.0/tests/test_request_helpers.py` & `modis_tools-1.1.1/tests/test_request_helpers.py`

 * *Files identical despite different names*

