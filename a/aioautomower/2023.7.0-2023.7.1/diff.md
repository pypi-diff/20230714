# Comparing `tmp/aioautomower-2023.7.0.tar.gz` & `tmp/aioautomower-2023.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioautomower-2023.7.0.tar", last modified: Mon Jul  3 19:00:45 2023, max compression
+gzip compressed data, was "aioautomower-2023.7.1.tar", last modified: Fri Jul 14 17:03:37 2023, max compression
```

## Comparing `aioautomower-2023.7.0.tar` & `aioautomower-2023.7.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:00:45.652025 aioautomower-2023.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-03 19:00:34.000000 aioautomower-2023.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-03 19:00:45.652025 aioautomower-2023.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-07-03 19:00:34.000000 aioautomower-2023.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:00:45.652025 aioautomower-2023.7.0/aioautomower/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-03 19:00:34.000000 aioautomower-2023.7.0/aioautomower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-03 19:00:34.000000 aioautomower-2023.7.0/aioautomower/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-03 19:00:34.000000 aioautomower-2023.7.0/aioautomower/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-07-03 19:00:34.000000 aioautomower-2023.7.0/aioautomower/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)    16650 2023-07-03 19:00:34.000000 aioautomower-2023.7.0/aioautomower/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:00:45.652025 aioautomower-2023.7.0/aioautomower.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-03 19:00:45.000000 aioautomower-2023.7.0/aioautomower.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-03 19:00:45.000000 aioautomower-2023.7.0/aioautomower.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:00:45.000000 aioautomower-2023.7.0/aioautomower.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:00:45.000000 aioautomower-2023.7.0/aioautomower.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 19:00:45.000000 aioautomower-2023.7.0/aioautomower.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-03 19:00:45.000000 aioautomower-2023.7.0/aioautomower.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:00:45.652025 aioautomower-2023.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-03 19:00:34.000000 aioautomower-2023.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:03:37.734685 aioautomower-2023.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-14 17:03:19.000000 aioautomower-2023.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-14 17:03:37.734685 aioautomower-2023.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-07-14 17:03:19.000000 aioautomower-2023.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:03:37.734685 aioautomower-2023.7.1/aioautomower/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-14 17:03:19.000000 aioautomower-2023.7.1/aioautomower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-14 17:03:19.000000 aioautomower-2023.7.1/aioautomower/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-14 17:03:19.000000 aioautomower-2023.7.1/aioautomower/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-07-14 17:03:19.000000 aioautomower-2023.7.1/aioautomower/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16983 2023-07-14 17:03:19.000000 aioautomower-2023.7.1/aioautomower/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:03:37.734685 aioautomower-2023.7.1/aioautomower.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-14 17:03:37.000000 aioautomower-2023.7.1/aioautomower.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-14 17:03:37.000000 aioautomower-2023.7.1/aioautomower.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:03:37.000000 aioautomower-2023.7.1/aioautomower.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-14 17:03:37.000000 aioautomower-2023.7.1/aioautomower.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 17:03:37.000000 aioautomower-2023.7.1/aioautomower.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-14 17:03:37.000000 aioautomower-2023.7.1/aioautomower.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 17:03:37.734685 aioautomower-2023.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-14 17:03:19.000000 aioautomower-2023.7.1/setup.py
```

### Comparing `aioautomower-2023.7.0/LICENSE` & `aioautomower-2023.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aioautomower-2023.7.0/PKG-INFO` & `aioautomower-2023.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioautomower
-Version: 2023.7.0
+Version: 2023.7.1
 Summary: module to communicate to Husqvarna Automower API
 Home-page: https://github.com/Thomas55555/aioautomower
 Author: Thomas Protzner
 Author-email: thomas.protzner@gmail.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aioautomower-2023.7.0/README.md` & `aioautomower-2023.7.1/README.md`

 * *Files identical despite different names*

### Comparing `aioautomower-2023.7.0/aioautomower/cli.py` & `aioautomower-2023.7.1/aioautomower/cli.py`

 * *Files identical despite different names*

### Comparing `aioautomower-2023.7.0/aioautomower/const.py` & `aioautomower-2023.7.1/aioautomower/const.py`

 * *Files identical despite different names*

### Comparing `aioautomower-2023.7.0/aioautomower/rest.py` & `aioautomower-2023.7.1/aioautomower/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,23 +34,14 @@
 
     def __init__(self, status: str) -> None:
         """Initialize."""
         super().__init__(status)
         self.status = status
 
 
-class TokenValidationError(Exception):
-    """Raised when Husqvarna Authentication API token request ended in error 404. The reason might be an invalid token or that a refresh is needed"""
-
-    def __init__(self, status: str) -> None:
-        """Initialize."""
-        super().__init__(status)
-        self.status = status
-
-
 class MowerApiConnectionsError(Exception):
     """Raised when Husqvarna Connect API request ended in error 403."""
 
     def __init__(self, status: str) -> None:
         """Initialize."""
         super().__init__(status)
         self.status = status
```

### Comparing `aioautomower-2023.7.0/aioautomower/session.py` & `aioautomower-2023.7.1/aioautomower/session.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,23 +19,14 @@
     WS_TOLERANCE_TIME,
     WS_URL,
 )
 
 _LOGGER = logging.getLogger(__name__)
 
 
-class RefresehdTokenNotWorkingError(Exception):
-    """Raised when token is refresehd 5 times, but Connect API still raises an exception."""
-
-    def __init__(self, status: str) -> None:
-        """Initialize."""
-        super().__init__(status)
-        self.status = status
-
-
 class AutomowerSession:
     """Session"""
 
     def __init__(
         self,
         api_key: str,
         token: dict = None,
@@ -64,15 +55,14 @@
 
         self.data = None
 
         self.ws_task = None
         self.token_task = None
         self.websocket_monitor_task = None
         self.rest_task = None
-        self.mower_connection_error_count = 0
 
     def register_data_callback(self, callback, schedule_immediately=False):
         """Register a data update callback.
 
         :param func callback: Callback fired on data updates. Takes one dict argument which is the up-to-date mower data list.
         :param bool schedule_immediately: Schedule callback immediately (if data is available).
         """
@@ -121,16 +111,18 @@
         self._schedule_token_callbacks()
         return self.token
 
     async def connect(self):
         """Connect to the API.
 
         This method handles the login and starts a task that keep the access
-        token constantly fresh. This method works only, if the token is created with the
-        Authorization Code Grant. Call this method before any other methods.
+        token constantly fresh. Also a REST taks will be started, which
+        periodically polls the REST endpoint. This method works only, if the
+        token is created with the Authorization Code Grant. Call this method
+        before any other methods.
         """
         if self.token is None:
             raise AttributeError("No token to connect with.")
         if time.time() > (self.token["expires_at"] - MARGIN_TIME):
             await self.refresh_token()
 
         self.data = await self.get_status()
@@ -142,14 +134,35 @@
                 HUSQVARNA_URL,
             )
         else:
             self.ws_task = self.loop.create_task(self._ws_task())
         self.rest_task = self.loop.create_task(self._rest_task())
         self.token_task = self.loop.create_task(self._token_monitor_task())
 
+    async def ws_and_token_session(self):
+        """Connect to the API.
+
+        This method handles the login and starts a task that keep the access
+        token constantly fresh. This method works only, if the token is created with the
+        Authorization Code Grant. Call this method before any other methods.
+        """
+        if self.token is None:
+            raise AttributeError("No token to connect with.")
+        if time.time() > (self.token["expires_at"] - MARGIN_TIME):
+            await self.refresh_token()
+
+        self.data = await self.get_status()
+        self._schedule_data_callbacks()
+
+        if "amc:api" not in self.token["scope"]:
+            raise NotImplementedError()
+        else:
+            self.ws_task = self.loop.create_task(self._ws_task())
+        self.token_task = self.loop.create_task(self._token_monitor_task())
+
     async def close(self):
         """Close the session."""
         for task in [
             self.ws_task,
             self.token_task,
             self.websocket_monitor_task,
             self.rest_task,
@@ -331,28 +344,24 @@
                             _LOGGER.debug("Received CLOSED")
                         else:
                             _LOGGER.debug("Received msg.type=%d", msg.type)
 
     async def _rest_task(self):
         """Poll data periodically via Rest."""
         while True:
+            _LOGGER.debug(
+                "LE: %s",
+                self.low_energy,
+            )
             if self.low_energy is True:
                 await asyncio.sleep(REST_POLL_CYCLE_LE)
             if self.low_energy is False:
                 await asyncio.sleep(REST_POLL_CYCLE)
-            try:
-                self.data = await self.get_status()
-                self._schedule_data_callbacks()
-                self.mower_connection_error_count = 0
-            except rest.MowerApiConnectionsError:
-                self.mower_connection_error_count += 1
-                if self.mower_connection_error_count < 5:
-                    self.refresh_token()
-                if self.mower_connection_error_count == 5:
-                    raise RefresehdTokenNotWorkingError
+            self.data = await self.get_status()
+            self._schedule_data_callbacks()
 
     async def _websocket_monitor_task(self):
         """Monitor, if the websocket still sends updates. If not, check, via REST,
         if the mower is connected. If there are no recent updates, Start REST task
         to get information"""
         message_sent = []
         mower_connected = []
```

### Comparing `aioautomower-2023.7.0/aioautomower.egg-info/PKG-INFO` & `aioautomower-2023.7.1/aioautomower.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioautomower
-Version: 2023.7.0
+Version: 2023.7.1
 Summary: module to communicate to Husqvarna Automower API
 Home-page: https://github.com/Thomas55555/aioautomower
 Author: Thomas Protzner
 Author-email: thomas.protzner@gmail.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aioautomower-2023.7.0/setup.py` & `aioautomower-2023.7.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,12 +15,12 @@
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     install_requires=list(val.strip() for val in open("requirements.txt")),
-    version="2023.7.0",
+    version="2023.7.1",
     entry_points={
         "console_scripts": ["automower=aioautomower.cli:main"],
     },
 )
```

