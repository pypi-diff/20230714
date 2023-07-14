# Comparing `tmp/aiocomelit-0.0.3.tar.gz` & `tmp/aiocomelit-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiocomelit-0.0.3.tar", max compression
+gzip compressed data, was "aiocomelit-0.0.4.tar", max compression
```

## Comparing `aiocomelit-0.0.3.tar` & `aiocomelit-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11346 2023-07-04 19:31:04.621003 aiocomelit-0.0.3/LICENSE
--rw-r--r--   0        0        0     3306 2023-07-04 19:31:04.721003 aiocomelit-0.0.3/README.md
--rw-r--r--   0        0        0     1940 2023-07-14 12:48:05.775671 aiocomelit-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      420 2023-07-14 12:48:05.775671 aiocomelit-0.0.3/src/aiocomelit/__init__.py
--rw-r--r--   0        0        0     8175 2023-07-14 12:48:05.775671 aiocomelit-0.0.3/src/aiocomelit/api.py
--rw-r--r--   0        0        0      388 2023-07-14 12:48:05.775671 aiocomelit-0.0.3/src/aiocomelit/const.py
--rw-r--r--   0        0        0      441 2023-07-05 21:05:53.271526 aiocomelit-0.0.3/src/aiocomelit/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-04 19:31:04.451003 aiocomelit-0.0.3/src/aiocomelit/py.typed
--rw-r--r--   0        0        0     4322 1970-01-01 00:00:00.000000 aiocomelit-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-07-04 19:31:04.621003 aiocomelit-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3306 2023-07-04 19:31:04.721003 aiocomelit-0.0.4/README.md
+-rw-r--r--   0        0        0     1940 2023-07-14 17:48:38.640530 aiocomelit-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      420 2023-07-14 17:48:38.640530 aiocomelit-0.0.4/src/aiocomelit/__init__.py
+-rw-r--r--   0        0        0     9639 2023-07-14 17:43:51.602105 aiocomelit-0.0.4/src/aiocomelit/api.py
+-rw-r--r--   0        0        0      428 2023-07-14 17:43:51.602105 aiocomelit-0.0.4/src/aiocomelit/const.py
+-rw-r--r--   0        0        0      441 2023-07-05 21:05:53.271526 aiocomelit-0.0.4/src/aiocomelit/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-04 19:31:04.451003 aiocomelit-0.0.4/src/aiocomelit/py.typed
+-rw-r--r--   0        0        0     4322 1970-01-01 00:00:00.000000 aiocomelit-0.0.4/PKG-INFO
```

### Comparing `aiocomelit-0.0.3/LICENSE` & `aiocomelit-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aiocomelit-0.0.3/README.md` & `aiocomelit-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `aiocomelit-0.0.3/pyproject.toml` & `aiocomelit-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiocomelit"
-version = "0.0.3"
+version = "0.0.4"
 description = "Python library to control Comelit Simplehome"
 authors = ["Simone Chemelli <simone.chemelli@gmail.com>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 repository = "https://github.com/chemelli74/aiocomelit"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
```

### Comparing `aiocomelit-0.0.3/src/aiocomelit/api.py` & `aiocomelit-0.0.4/src/aiocomelit/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,25 @@
 from dataclasses import dataclass
 from datetime import datetime
 from http.cookies import SimpleCookie
 from typing import Any
 
 import aiohttp
 
-from .const import _LOGGER, CLIMATE, COVER, COVER_STATUS, LIGHT, MAX_ZONES, OTHER
+from .const import (
+    _LOGGER,
+    CLIMATE,
+    COVER,
+    COVER_STATUS,
+    LIGHT,
+    LIGHT_ON,
+    MAX_ZONES,
+    OTHER,
+    SLEEP,
+)
 from .exceptions import CannotAuthenticate, CannotConnect
 
 
 @dataclass
 class ComelitSerialBridgeObject:
     """Comelit SimpleHome Serial bridge class."""
 
@@ -60,14 +70,15 @@
             "Referer": f"{self.base_url}/",
         }
         jar = aiohttp.CookieJar(unsafe=True)
         self.session = aiohttp.ClientSession(cookie_jar=jar)
         self._unique_id: str | None = None
         self._devices: list[ComelitSerialBridgeObject] = []
         self._alarm: list[ComelitVedoObject] = []
+        self._alarm_logged: bool = False
 
     async def _get_devices(self, device_type: str) -> dict[str, Any]:
         """Get devices description."""
         timestamp = datetime.now().strftime("%s")
         url = f"{self.base_url}/user/icon_desc.json?type={device_type}&_={timestamp}"
         response = await self.session.get(
             url,
@@ -89,22 +100,39 @@
         response = await self.session.get(
             url,
             headers=self.headers,
             timeout=10,
         )
         return response.status == 200
 
+    async def _get_device_status(self, device_type: str, index: int) -> int:
+        """Get device status, -1 means API call failed."""
+        url = f"{self.base_url}/user/icon_status.json?type={device_type}"
+        response = await self.session.get(
+            url,
+            headers=self.headers,
+            timeout=10,
+        )
+        if response.status == 200:
+            json = await response.json()
+            _LOGGER.debug("Device %s status: %s", device_type, json["status"])
+            return json["status"][index]
+        return -1
+
     async def _set_cookie(self, value: str) -> None:
         """Enable required session cookie."""
         self.session.cookie_jar.update_cookies(
             SimpleCookie(f"domain={self.host}; name=sid; value=1;")
         )
 
     async def _do_alarm_login(self) -> bool:
         """Login into VEDO system via Comelit Serial Bridge."""
+        if self._alarm_logged:
+            return True
+
         payload = {"alm": self.alarm_pin}
         url = f"{self.base_url}/login.cgi"
         response = await self.session.post(
             url,
             data=payload,
             headers=self.headers,
             timeout=10,
@@ -139,25 +167,46 @@
 
     async def _translate_device_status(self, dev_type: str, dev_status: int) -> str:
         """Makes status human readable."""
 
         if dev_type == COVER:
             return COVER_STATUS[dev_status]
 
-        return "on" if dev_status == 1 else "off"
+        return "on" if dev_status == LIGHT_ON else "off"
+
+    async def login(self) -> bool:
+        """Login to Serial Bridge device."""
+        _LOGGER.info("Logging into Serial Bridge %s", self.host)
+        url = f"{self.base_url}/login.json"
+        response = await self.session.get(
+            url,
+            headers=self.headers,
+            timeout=10,
+        )
+
+        return response.status == 200
 
     async def light_switch(self, index: int, action: int) -> bool:
         """Set status of the light."""
         return await self._set_device_status(LIGHT, index, action)
 
+    async def light_status(self, index: int) -> int:
+        """Get status of the light."""
+        await asyncio.sleep(SLEEP)
+        return await self._get_device_status(LIGHT, index)
+
     async def cover_move(self, index: int, action: int) -> bool:
         """Move cover up/down."""
-
         return await self._set_device_status(COVER, index, action)
 
+    async def cover_status(self, index: int) -> int:
+        """Get cover status."""
+        await asyncio.sleep(SLEEP)
+        return await self._get_device_status(COVER, index)
+
     async def get_all_devices(self) -> list[ComelitSerialBridgeObject]:
         """Get all connected devices."""
 
         _LOGGER.debug("Getting all devices for host %s", self.host)
 
         for dev_type in (CLIMATE, COVER, LIGHT, OTHER):
             reply_json = await self._get_devices(dev_type)
@@ -182,29 +231,29 @@
 
         return self._devices
 
     async def alarm_login(self) -> bool:
         """Login to vedo alarm system."""
         _LOGGER.debug("Logging into %s (VEDO)", self.host)
         try:
-            logged = await self._do_alarm_login()
+            self._alarm_logged = await self._do_alarm_login()
         except (asyncio.exceptions.TimeoutError, aiohttp.ClientConnectorError) as exc:
             _LOGGER.warning("Connection error for %s", self.host)
             raise CannotConnect from exc
 
-        if not logged:
+        if not self._alarm_logged:
             raise CannotAuthenticate
 
+        await asyncio.sleep(SLEEP)
         return True
 
     async def get_alarm_config(self) -> list[ComelitVedoObject]:
         """Get Comelit SimpleHome alarm configuration."""
 
         await self.alarm_login()
-        await asyncio.sleep(0.5)
 
         reply_json_desc = await self._get_alarm_desc()
         _LOGGER.debug("Alarm description: %s", reply_json_desc)
         reply_json_stat = await self._get_alarm_stat()
         _LOGGER.debug("Alarm statistics: %s", reply_json_stat)
 
         if (reply_json_desc or reply_json_stat) is {}:
```

### Comparing `aiocomelit-0.0.3/PKG-INFO` & `aiocomelit-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocomelit
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python library to control Comelit Simplehome
 Home-page: https://github.com/chemelli74/aiocomelit
 License: Apache Software License 2.0
 Author: Simone Chemelli
 Author-email: simone.chemelli@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aiocomelit Version: 0.0.3 Summary: Python library
+Metadata-Version: 2.1 Name: aiocomelit Version: 0.0.4 Summary: Python library
 to control Comelit Simplehome Home-page: https://github.com/chemelli74/
 aiocomelit License: Apache Software License 2.0 Author: Simone Chemelli Author-
 email: simone.chemelli@gmail.com Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License Classifier: Natural Language
 :: English Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

