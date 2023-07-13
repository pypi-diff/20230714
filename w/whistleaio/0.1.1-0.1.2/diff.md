# Comparing `tmp/whistleaio-0.1.1.tar.gz` & `tmp/whistleaio-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whistleaio-0.1.1.tar", last modified: Tue Jun 27 23:37:50 2023, max compression
+gzip compressed data, was "whistleaio-0.1.2.tar", last modified: Thu Jul 13 22:01:59 2023, max compression
```

## Comparing `whistleaio-0.1.1.tar` & `whistleaio-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-06-27 23:37:50.621311 whistleaio-0.1.1/
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1067 2023-06-27 23:35:50.000000 whistleaio-0.1.1/LICENSE
--rw-r--r--   0 robertdrinovac   (501) staff       (20)     1282 2023-06-27 23:37:50.620865 whistleaio-0.1.1/PKG-INFO
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)      460 2023-06-27 23:35:50.000000 whistleaio-0.1.1/README.md
--rw-r--r--   0 robertdrinovac   (501) staff       (20)       38 2023-06-27 23:37:50.621521 whistleaio-0.1.1/setup.cfg
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1007 2023-06-27 23:35:50.000000 whistleaio-0.1.1/setup.py
-drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-06-27 23:37:50.618145 whistleaio-0.1.1/whistleaio/
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)      312 2023-06-27 23:35:50.000000 whistleaio-0.1.1/whistleaio/__init__.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     7255 2023-06-27 23:35:50.000000 whistleaio-0.1.1/whistleaio/client.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)      696 2023-06-27 23:35:50.000000 whistleaio-0.1.1/whistleaio/const.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)      448 2023-06-27 23:35:50.000000 whistleaio-0.1.1/whistleaio/exceptions.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)      497 2023-06-27 23:35:50.000000 whistleaio-0.1.1/whistleaio/model.py
-drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-06-27 23:37:50.620143 whistleaio-0.1.1/whistleaio.egg-info/
--rw-r--r--   0 robertdrinovac   (501) staff       (20)     1282 2023-06-27 23:37:50.000000 whistleaio-0.1.1/whistleaio.egg-info/PKG-INFO
--rw-r--r--   0 robertdrinovac   (501) staff       (20)      304 2023-06-27 23:37:50.000000 whistleaio-0.1.1/whistleaio.egg-info/SOURCES.txt
--rw-r--r--   0 robertdrinovac   (501) staff       (20)        1 2023-06-27 23:37:50.000000 whistleaio-0.1.1/whistleaio.egg-info/dependency_links.txt
--rw-r--r--   0 robertdrinovac   (501) staff       (20)       30 2023-06-27 23:37:50.000000 whistleaio-0.1.1/whistleaio.egg-info/requires.txt
--rw-r--r--   0 robertdrinovac   (501) staff       (20)       11 2023-06-27 23:37:50.000000 whistleaio-0.1.1/whistleaio.egg-info/top_level.txt
+drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-07-13 22:01:59.804583 whistleaio-0.1.2/
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1067 2023-07-13 21:57:43.000000 whistleaio-0.1.2/LICENSE
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)     1282 2023-07-13 22:01:59.804169 whistleaio-0.1.2/PKG-INFO
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)      460 2023-07-13 21:57:43.000000 whistleaio-0.1.2/README.md
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)       38 2023-07-13 22:01:59.804753 whistleaio-0.1.2/setup.cfg
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1007 2023-07-13 21:57:43.000000 whistleaio-0.1.2/setup.py
+drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-07-13 22:01:59.800323 whistleaio-0.1.2/whistleaio/
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)      312 2023-07-13 21:57:43.000000 whistleaio-0.1.2/whistleaio/__init__.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     7380 2023-07-13 21:57:43.000000 whistleaio-0.1.2/whistleaio/client.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)      696 2023-07-13 21:57:43.000000 whistleaio-0.1.2/whistleaio/const.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)      448 2023-07-13 21:57:43.000000 whistleaio-0.1.2/whistleaio/exceptions.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)      497 2023-07-13 21:57:43.000000 whistleaio-0.1.2/whistleaio/model.py
+drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-07-13 22:01:59.803417 whistleaio-0.1.2/whistleaio.egg-info/
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)     1282 2023-07-13 22:01:59.000000 whistleaio-0.1.2/whistleaio.egg-info/PKG-INFO
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)      304 2023-07-13 22:01:59.000000 whistleaio-0.1.2/whistleaio.egg-info/SOURCES.txt
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)        1 2023-07-13 22:01:59.000000 whistleaio-0.1.2/whistleaio.egg-info/dependency_links.txt
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)       30 2023-07-13 22:01:59.000000 whistleaio-0.1.2/whistleaio.egg-info/requires.txt
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)       11 2023-07-13 22:01:59.000000 whistleaio-0.1.2/whistleaio.egg-info/top_level.txt
```

### Comparing `whistleaio-0.1.1/LICENSE` & `whistleaio-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `whistleaio-0.1.1/PKG-INFO` & `whistleaio-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whistleaio
-Version: 0.1.1
+Version: 0.1.2
 Summary: Asynchronous Python library for Whistle's API
 Home-page: https://github.com/RobertD502/whistleaio
 Author: Robert Drinovac
 Author-email: unlisted@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/RobertD502/whistleaio/issues
 Project-URL: Source, https://github.com/RobertD502/whistleaio/
```

### Comparing `whistleaio-0.1.1/setup.py` & `whistleaio-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="whistleaio",
-    version="0.1.1",
+    version="0.1.2",
     author="Robert Drinovac",
     author_email="unlisted@gmail.com",
     description="Asynchronous Python library for Whistle's API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/RobertD502/whistleaio',
     keywords='whistle, whistle fit, whistle api, whistle client, whistle gps, whistle pet',
```

### Comparing `whistleaio-0.1.1/whistleaio/client.py` & `whistleaio-0.1.2/whistleaio/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """ Python client for Whistle API """
 from __future__ import annotations
 
 from typing import Any
 
 import asyncio
 from aiohttp import ClientResponse, ClientSession
+from aiohttp.client_exceptions import ContentTypeError
 
 from whistleaio.const import Endpoint, Header, TIMEOUT
 
 from whistleaio.exceptions import WhistleAuthError, WhistleError
 
 from whistleaio.model import WhistleData, Pet
 
@@ -188,14 +189,14 @@
 
     @staticmethod
     async def _response(resp: ClientResponse) -> dict[str, Any] | None:
         """ Check response for any errors & return original response if none """
 
         try:
             response: dict[str, Any] = await resp.json()
-        except Exception as ex:
-            raise WhistleError(ex)
+        except ContentTypeError as cte:
+            raise WhistleError(f'Whistle servers failed to return data for endpoint {resp.url}')
         if resp.status == 422:
             if response['errors'][0]['message'] == 'Invalid email address or password':
                 raise WhistleAuthError('Invalid email address or password')
         else:
             return response
```

### Comparing `whistleaio-0.1.1/whistleaio/const.py` & `whistleaio-0.1.2/whistleaio/const.py`

 * *Files identical despite different names*

### Comparing `whistleaio-0.1.1/whistleaio.egg-info/PKG-INFO` & `whistleaio-0.1.2/whistleaio.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whistleaio
-Version: 0.1.1
+Version: 0.1.2
 Summary: Asynchronous Python library for Whistle's API
 Home-page: https://github.com/RobertD502/whistleaio
 Author: Robert Drinovac
 Author-email: unlisted@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/RobertD502/whistleaio/issues
 Project-URL: Source, https://github.com/RobertD502/whistleaio/
```

