# Comparing `tmp/ac_infinity_ble-0.1.0.tar.gz` & `tmp/ac_infinity_ble-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ac_infinity_ble-0.1.0.tar", max compression
+gzip compressed data, was "ac_infinity_ble-0.2.0.tar", max compression
```

## Comparing `ac_infinity_ble-0.1.0.tar` & `ac_infinity_ble-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1070 2023-07-14 07:10:47.299447 ac_infinity_ble-0.1.0/LICENSE
--rw-r--r--   0        0        0     3538 2023-07-14 07:10:47.299447 ac_infinity_ble-0.1.0/README.md
--rw-r--r--   0        0        0     2182 2023-07-14 07:10:48.355525 ac_infinity_ble-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      163 2023-07-14 07:10:48.323523 ac_infinity_ble-0.1.0/src/ac_infinity_ble/__init__.py
--rw-r--r--   0        0        0      283 2023-07-14 07:10:47.303448 ac_infinity_ble-0.1.0/src/ac_infinity_ble/const.py
--rw-r--r--   0        0        0    14662 2023-07-14 07:10:47.303448 ac_infinity_ble-0.1.0/src/ac_infinity_ble/device.py
--rw-r--r--   0        0        0       96 2023-07-14 07:10:47.303448 ac_infinity_ble-0.1.0/src/ac_infinity_ble/exceptions.py
--rw-r--r--   0        0        0      591 2023-07-14 07:10:47.303448 ac_infinity_ble-0.1.0/src/ac_infinity_ble/models.py
--rw-r--r--   0        0        0     3150 2023-07-14 07:10:47.303448 ac_infinity_ble-0.1.0/src/ac_infinity_ble/protocol.py
--rw-r--r--   0        0        0        0 2023-07-14 07:10:47.303448 ac_infinity_ble-0.1.0/src/ac_infinity_ble/py.typed
--rw-r--r--   0        0        0      756 2023-07-14 07:10:47.303448 ac_infinity_ble-0.1.0/src/ac_infinity_ble/util.py
--rw-r--r--   0        0        0     4659 1970-01-01 00:00:00.000000 ac_infinity_ble-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 20:37:17.454602 ac_infinity_ble-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3538 2023-07-14 20:37:17.454602 ac_infinity_ble-0.2.0/README.md
+-rw-r--r--   0        0        0     2182 2023-07-14 20:37:18.390612 ac_infinity_ble-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      163 2023-07-14 20:37:18.354611 ac_infinity_ble-0.2.0/src/ac_infinity_ble/__init__.py
+-rw-r--r--   0        0        0      283 2023-07-14 20:37:17.458602 ac_infinity_ble-0.2.0/src/ac_infinity_ble/const.py
+-rw-r--r--   0        0        0    15367 2023-07-14 20:37:17.458602 ac_infinity_ble-0.2.0/src/ac_infinity_ble/device.py
+-rw-r--r--   0        0        0       96 2023-07-14 20:37:17.458602 ac_infinity_ble-0.2.0/src/ac_infinity_ble/exceptions.py
+-rw-r--r--   0        0        0      591 2023-07-14 20:37:17.458602 ac_infinity_ble-0.2.0/src/ac_infinity_ble/models.py
+-rw-r--r--   0        0        0     3150 2023-07-14 20:37:17.458602 ac_infinity_ble-0.2.0/src/ac_infinity_ble/protocol.py
+-rw-r--r--   0        0        0        0 2023-07-14 20:37:17.458602 ac_infinity_ble-0.2.0/src/ac_infinity_ble/py.typed
+-rw-r--r--   0        0        0      756 2023-07-14 20:37:17.458602 ac_infinity_ble-0.2.0/src/ac_infinity_ble/util.py
+-rw-r--r--   0        0        0     4659 1970-01-01 00:00:00.000000 ac_infinity_ble-0.2.0/PKG-INFO
```

### Comparing `ac_infinity_ble-0.1.0/LICENSE` & `ac_infinity_ble-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ac_infinity_ble-0.1.0/README.md` & `ac_infinity_ble-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ac_infinity_ble-0.1.0/pyproject.toml` & `ac_infinity_ble-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ac-infinity-ble"
-version = "0.1.0"
+version = "0.2.0"
 description = "AC Infinity BLE Controller"
 authors = ["Jason Hunter <hunterjm@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/hunterjm/ac-infinity-ble"
 documentation = "https://ac-infinity-ble.readthedocs.io"
 classifiers = [
```

### Comparing `ac_infinity_ble-0.1.0/src/ac_infinity_ble/device.py` & `ac_infinity_ble-0.2.0/src/ac_infinity_ble/device.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import asyncio
 import logging
 from collections.abc import Callable
+from dataclasses import asdict, replace
 
 from bleak.backends.device import BLEDevice
 from bleak.backends.scanner import AdvertisementData
 from bleak.backends.service import BleakGATTCharacteristic, BleakGATTServiceCollection
 from bleak.exc import BleakDBusError
 from bleak_retry_connector import BLEAK_RETRY_EXCEPTIONS as BLEAK_EXCEPTIONS
 from bleak_retry_connector import (
@@ -57,15 +58,30 @@
         self._disconnect_timer: asyncio.TimerHandle | None = None
         self._client: BleakClientWithServiceCache | None = None
         self._protocol: Protocol = Protocol()
         self._expected_disconnect = False
         self.loop = asyncio.get_running_loop()
         self._callbacks: list[Callable[[DeviceInfo], None]] = []
         self._sequence = 1
-        _LOGGER.debug(self._state)
+
+    def set_ble_device_and_advertisement_data(
+        self, ble_device: BLEDevice, advertisement_data: AdvertisementData
+    ) -> None:
+        """Set the ble device."""
+        self._ble_device = ble_device
+        self._advertisement_data = advertisement_data
+        info = parse_manufacturer_data(
+            advertisement_data.manufacturer_data[MANUFACTURER_ID]
+        )
+        self._state = replace(self._state, **asdict(info))
+        if self._state.fan:
+            if self._state.level_off or 0 > self._state.fan:
+                self._state.level_off = self._state.fan
+            if self._state.level_on or 10 < self._state.fan:
+                self._state.level_on = self._state.fan
 
     @property
     def address(self) -> str:
         """Return the address."""
         return self._ble_device.address
 
     @property
```

### Comparing `ac_infinity_ble-0.1.0/src/ac_infinity_ble/models.py` & `ac_infinity_ble-0.2.0/src/ac_infinity_ble/models.py`

 * *Files identical despite different names*

### Comparing `ac_infinity_ble-0.1.0/src/ac_infinity_ble/protocol.py` & `ac_infinity_ble-0.2.0/src/ac_infinity_ble/protocol.py`

 * *Files identical despite different names*

### Comparing `ac_infinity_ble-0.1.0/src/ac_infinity_ble/util.py` & `ac_infinity_ble-0.2.0/src/ac_infinity_ble/util.py`

 * *Files identical despite different names*

### Comparing `ac_infinity_ble-0.1.0/PKG-INFO` & `ac_infinity_ble-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ac-infinity-ble
-Version: 0.1.0
+Version: 0.2.0
 Summary: AC Infinity BLE Controller
 Home-page: https://github.com/hunterjm/ac-infinity-ble
 License: MIT
 Author: Jason Hunter
 Author-email: hunterjm@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ac-infinity-ble Version: 0.1.0 Summary: AC Infinity
+Metadata-Version: 2.1 Name: ac-infinity-ble Version: 0.2.0 Summary: AC Infinity
 BLE Controller Home-page: https://github.com/hunterjm/ac-infinity-ble License:
 MIT Author: Jason Hunter Author-email: hunterjm@gmail.com Requires-Python:
 >=3.10,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

