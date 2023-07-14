# Comparing `tmp/gundi_client_v2-2.0.1.tar.gz` & `tmp/gundi_client_v2-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gundi_client_v2-2.0.1.tar", max compression
+gzip compressed data, was "gundi_client_v2-2.1.0.tar", max compression
```

## Comparing `gundi_client_v2-2.0.1.tar` & `gundi_client_v2-2.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1542 2023-07-04 12:49:45.871005 gundi_client_v2-2.0.1/README.md
--rw-r--r--   0        0        0       53 2023-06-16 14:01:41.406285 gundi_client_v2-2.0.1/gundi_client_v2/__init__.py
--rw-r--r--   0        0        0      684 2023-06-16 13:13:56.285203 gundi_client_v2-2.0.1/gundi_client_v2/auth.py
--rw-r--r--   0        0        0     4824 2023-07-03 21:19:55.524453 gundi_client_v2-2.0.1/gundi_client_v2/client.py
--rw-r--r--   0        0        0        0 2023-06-16 12:38:36.081819 gundi_client_v2-2.0.1/gundi_client_v2/errors.py
--rw-r--r--   0        0        0      657 2023-06-16 12:43:16.414342 gundi_client_v2-2.0.1/gundi_client_v2/settings.py
--rw-r--r--   0        0        0      678 2023-07-04 12:36:57.916916 gundi_client_v2-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     2355 1970-01-01 00:00:00.000000 gundi_client_v2-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1542 2023-07-14 12:26:43.861804 gundi_client_v2-2.1.0/README.md
+-rw-r--r--   0        0        0       53 2023-07-14 12:26:43.861804 gundi_client_v2-2.1.0/gundi_client_v2/__init__.py
+-rw-r--r--   0        0        0      684 2023-07-14 12:26:43.861804 gundi_client_v2-2.1.0/gundi_client_v2/auth.py
+-rw-r--r--   0        0        0     5343 2023-07-14 14:07:45.155266 gundi_client_v2-2.1.0/gundi_client_v2/client.py
+-rw-r--r--   0        0        0        0 2023-07-14 12:26:43.889805 gundi_client_v2-2.1.0/gundi_client_v2/errors.py
+-rw-r--r--   0        0        0      657 2023-07-14 12:26:43.889805 gundi_client_v2-2.1.0/gundi_client_v2/settings.py
+-rw-r--r--   0        0        0      678 2023-07-14 12:42:41.019860 gundi_client_v2-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2355 1970-01-01 00:00:00.000000 gundi_client_v2-2.1.0/PKG-INFO
```

### Comparing `gundi_client_v2-2.0.1/README.md` & `gundi_client_v2-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `gundi_client_v2-2.0.1/gundi_client_v2/auth.py` & `gundi_client_v2-2.1.0/gundi_client_v2/auth.py`

 * *Files identical despite different names*

### Comparing `gundi_client_v2-2.0.1/gundi_client_v2/client.py` & `gundi_client_v2-2.1.0/gundi_client_v2/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import logging
 from datetime import datetime, timezone, timedelta
 from httpx import (
     AsyncClient,
     AsyncHTTPTransport,
-    RequestError,
     Timeout,
-    TimeoutException,
-    HTTPStatusError
 )
+from pydantic import parse_obj_as
+from typing import List
 from gundi_core.schemas import (
     OAuthToken,
 )
-from gundi_core.schemas.v2 import Connection, Route, Integration
+from gundi_core.schemas.v2 import Connection, Route, Integration, GundiTrace
 from . import settings, errors
 from . import auth
 
 
 logger = logging.getLogger(__name__)
 logger.setLevel(settings.LOG_LEVEL)
 
@@ -31,14 +30,15 @@
         self.base_url = kwargs.get("base_url", settings.GUNDI_API_BASE_URL)
         self.api_base_path = f"{self.base_url}/api/{self.gundi_version}"
         self.connections_endpoint = f"{self.api_base_path}/connections"
         self.integrations_endpoint = f"{self.api_base_path}/integrations"
         self.source_states_endpoint = f"{self.api_base_path}/sources/states"
         self.sources_endpoint = f"{self.api_base_path}/sources"
         self.routes_endpoint = f"{self.api_base_path}/routes"
+        self.traces_endpoint = f"{self.api_base_path}/traces"
 
         # Authentication settings
         self.ssl_verify = kwargs.get("use_ssl", settings.GUNDI_API_SSL_VERIFY)
         self.client_id = kwargs.get("keycloak_client_id", settings.KEYCLOAK_CLIENT_ID)
         self.client_secret = kwargs.get("keycloak_client_secret", settings.KEYCLOAK_CLIENT_SECRET)
         self.oauth_token_url = kwargs.get("oauth_token_url", settings.OAUTH_TOKEN_URL)
         self.audience = kwargs.get("keycloak_audience", settings.KEYCLOAK_AUDIENCE)
@@ -123,7 +123,20 @@
             url,
             headers=headers,
         )
         # ToDo: Add custom exceptions to handle errors
         response.raise_for_status()
         data = response.json()
         return Integration.parse_obj(data)
+
+    async def get_traces(self, params: dict):
+        headers = await self.get_auth_header()
+        url = f"{self.traces_endpoint}/"
+        response = await self._session.get(
+            url,
+            params=params,
+            headers=headers,
+        )
+        # ToDo: Add custom exceptions to handle errors
+        response.raise_for_status()
+        data = response.json()["results"]
+        return parse_obj_as(List[GundiTrace], data)
```

### Comparing `gundi_client_v2-2.0.1/gundi_client_v2/settings.py` & `gundi_client_v2-2.1.0/gundi_client_v2/settings.py`

 * *Files identical despite different names*

### Comparing `gundi_client_v2-2.0.1/pyproject.toml` & `gundi_client_v2-2.1.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gundi-client-v2"
-version = "2.0.1"
+version = "2.1.0"
 description = "An async client for Gundi's API"
 authors = [
     "Chris Doehring <chrisdo@earthranger.com>",
     "Mariano M <marianom@earthranger.com>",
     "Victor Garcia <victorg@earthranger.com>"
 ]
 license = "Apache-2.0"
@@ -16,15 +16,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.7"
 environs = "^9.5"
 pydantic = "^1.10"
 httpx = "^0.24.0"
 respx = "^0.20.1"
-gundi-core = "^1.0.5"
+gundi-core = "^1.2.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 pytest = "^7.2.1"
 pytest-asyncio = "^0.20.3"
 
 [build-system]
```

### Comparing `gundi_client_v2-2.0.1/PKG-INFO` & `gundi_client_v2-2.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: gundi-client-v2
-Version: 2.0.1
+Version: 2.1.0
 Summary: An async client for Gundi's API
 License: Apache-2.0
 Author: Chris Doehring
 Author-email: chrisdo@earthranger.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: environs (>=9.5,<10.0)
-Requires-Dist: gundi-core (>=1.0.5,<2.0.0)
+Requires-Dist: gundi-core (>=1.2.0,<2.0.0)
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: pydantic (>=1.10,<2.0)
 Requires-Dist: respx (>=0.20.1,<0.21.0)
 Description-Content-Type: text/markdown
 
 # Gundi Client
 ## Introduction
```

