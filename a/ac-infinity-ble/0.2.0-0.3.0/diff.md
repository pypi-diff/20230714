# Comparing `tmp/ac_infinity_ble-0.2.0.tar.gz` & `tmp/ac_infinity_ble-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ac_infinity_ble-0.2.0.tar", max compression
+gzip compressed data, was "ac_infinity_ble-0.3.0.tar", max compression
```

## Comparing `ac_infinity_ble-0.2.0.tar` & `ac_infinity_ble-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1070 2023-07-14 20:37:17.454602 ac_infinity_ble-0.2.0/LICENSE
--rw-r--r--   0        0        0     3538 2023-07-14 20:37:17.454602 ac_infinity_ble-0.2.0/README.md
--rw-r--r--   0        0        0     2182 2023-07-14 20:37:18.390612 ac_infinity_ble-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      163 2023-07-14 20:37:18.354611 ac_infinity_ble-0.2.0/src/ac_infinity_ble/__init__.py
--rw-r--r--   0        0        0      283 2023-07-14 20:37:17.458602 ac_infinity_ble-0.2.0/src/ac_infinity_ble/const.py
--rw-r--r--   0        0        0    15367 2023-07-14 20:37:17.458602 ac_infinity_ble-0.2.0/src/ac_infinity_ble/device.py
--rw-r--r--   0        0        0       96 2023-07-14 20:37:17.458602 ac_infinity_ble-0.2.0/src/ac_infinity_ble/exceptions.py
--rw-r--r--   0        0        0      591 2023-07-14 20:37:17.458602 ac_infinity_ble-0.2.0/src/ac_infinity_ble/models.py
--rw-r--r--   0        0        0     3150 2023-07-14 20:37:17.458602 ac_infinity_ble-0.2.0/src/ac_infinity_ble/protocol.py
--rw-r--r--   0        0        0        0 2023-07-14 20:37:17.458602 ac_infinity_ble-0.2.0/src/ac_infinity_ble/py.typed
--rw-r--r--   0        0        0      756 2023-07-14 20:37:17.458602 ac_infinity_ble-0.2.0/src/ac_infinity_ble/util.py
--rw-r--r--   0        0        0     4659 1970-01-01 00:00:00.000000 ac_infinity_ble-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 21:09:32.979167 ac_infinity_ble-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3538 2023-07-14 21:09:32.979167 ac_infinity_ble-0.3.0/README.md
+-rw-r--r--   0        0        0     2182 2023-07-14 21:09:33.771173 ac_infinity_ble-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      322 2023-07-14 21:09:33.743172 ac_infinity_ble-0.3.0/src/ac_infinity_ble/__init__.py
+-rw-r--r--   0        0        0      405 2023-07-14 21:09:32.983168 ac_infinity_ble-0.3.0/src/ac_infinity_ble/const.py
+-rw-r--r--   0        0        0    16046 2023-07-14 21:09:32.983168 ac_infinity_ble-0.3.0/src/ac_infinity_ble/device.py
+-rw-r--r--   0        0        0       96 2023-07-14 21:09:32.983168 ac_infinity_ble-0.3.0/src/ac_infinity_ble/exceptions.py
+-rw-r--r--   0        0        0      591 2023-07-14 21:09:32.983168 ac_infinity_ble-0.3.0/src/ac_infinity_ble/models.py
+-rw-r--r--   0        0        0     3150 2023-07-14 21:09:32.983168 ac_infinity_ble-0.3.0/src/ac_infinity_ble/protocol.py
+-rw-r--r--   0        0        0        0 2023-07-14 21:09:32.983168 ac_infinity_ble-0.3.0/src/ac_infinity_ble/py.typed
+-rw-r--r--   0        0        0      756 2023-07-14 21:09:32.983168 ac_infinity_ble-0.3.0/src/ac_infinity_ble/util.py
+-rw-r--r--   0        0        0     4659 1970-01-01 00:00:00.000000 ac_infinity_ble-0.3.0/PKG-INFO
```

### Comparing `ac_infinity_ble-0.2.0/LICENSE` & `ac_infinity_ble-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ac_infinity_ble-0.2.0/README.md` & `ac_infinity_ble-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ac_infinity_ble-0.2.0/pyproject.toml` & `ac_infinity_ble-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ac-infinity-ble"
-version = "0.2.0"
+version = "0.3.0"
 description = "AC Infinity BLE Controller"
 authors = ["Jason Hunter <hunterjm@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/hunterjm/ac-infinity-ble"
 documentation = "https://ac-infinity-ble.readthedocs.io"
 classifiers = [
```

### Comparing `ac_infinity_ble-0.2.0/src/ac_infinity_ble/device.py` & `ac_infinity_ble-0.3.0/src/ac_infinity_ble/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import asyncio
 import logging
 from collections.abc import Callable
 from dataclasses import asdict, replace
 
+import async_timeout
 from bleak.backends.device import BLEDevice
 from bleak.backends.scanner import AdvertisementData
 from bleak.backends.service import BleakGATTCharacteristic, BleakGATTServiceCollection
 from bleak.exc import BleakDBusError
 from bleak_retry_connector import BLEAK_RETRY_EXCEPTIONS as BLEAK_EXCEPTIONS
 from bleak_retry_connector import (
     BleakClientWithServiceCache,
@@ -18,14 +19,15 @@
     retry_bluetooth_connection_error,
 )
 
 from .const import (
     MANUFACTURER_ID,
     POSSIBLE_READ_CHARACTERISTIC_UUIDS,
     POSSIBLE_WRITE_CHARACTERISTIC_UUIDS,
+    CallbackType,
 )
 from .exceptions import CharacteristicMissingError
 from .models import DeviceInfo
 from .protocol import Protocol, parse_manufacturer_data
 from .util import get_bit, get_bits, get_short
 
 BLEAK_BACKOFF_TIME = 0.25
@@ -56,15 +58,15 @@
         self._read_char: BleakGATTCharacteristic | None = None
         self._write_char: BleakGATTCharacteristic | None = None
         self._disconnect_timer: asyncio.TimerHandle | None = None
         self._client: BleakClientWithServiceCache | None = None
         self._protocol: Protocol = Protocol()
         self._expected_disconnect = False
         self.loop = asyncio.get_running_loop()
-        self._callbacks: list[Callable[[DeviceInfo], None]] = []
+        self._callbacks: list[Callable[[DeviceInfo, CallbackType], None]] = []
         self._sequence = 1
 
     def set_ble_device_and_advertisement_data(
         self, ble_device: BLEDevice, advertisement_data: AdvertisementData
     ) -> None:
         """Set the ble device."""
         self._ble_device = ble_device
@@ -132,19 +134,34 @@
         if self._sequence == 65535:
             self._sequence = 0
         self._sequence += 1
         return self._sequence
 
     async def update(self) -> None:
         """Update the controller."""
+        events = {
+            CallbackType.NOTIFICATION: asyncio.Event(),
+            CallbackType.UPDATE_RESPONSE: asyncio.Event(),
+        }
+
+        def on_event(_: DeviceInfo, type: CallbackType) -> None:
+            events[type].set()
+
+        cancel_callback = self.register_callback(on_event)
+
         await self._ensure_connected()
         _LOGGER.debug("%s: Updating", self.name)
         command = self._protocol.get_model_data(self._state.type, 0, self.sequence)
         await self._send_command([command])
 
+        async with async_timeout.timeout(5):
+            await events[CallbackType.NOTIFICATION].wait()
+            await events[CallbackType.UPDATE_RESPONSE].wait()
+        cancel_callback()
+
     async def turn_on(self) -> None:
         """Turn on the controller."""
         await self._ensure_connected()
         _LOGGER.debug("%s: Turn on", self.name)
         self._state.work_type = 2
         self._state.fan = self._state.level_on or 10
         self._state.level_on = self._state.fan
@@ -177,21 +194,21 @@
         await self._send_command([command])
 
     async def stop(self) -> None:
         """Stop the controller."""
         _LOGGER.debug("%s: Stop", self.name)
         await self._execute_disconnect()
 
-    def _fire_callbacks(self) -> None:
+    def _fire_callbacks(self, type: CallbackType) -> None:
         """Fire the callbacks."""
         for callback in self._callbacks:
-            callback(self._state)
+            callback(self._state, type)
 
     def register_callback(
-        self, callback: Callable[[DeviceInfo], None]
+        self, callback: Callable[[DeviceInfo, CallbackType], None]
     ) -> Callable[[], None]:
         """Register a callback to be called when the state changes."""
 
         def unregister_callback() -> None:
             self._callbacks.remove(callback)
 
         self._callbacks.append(callback)
@@ -249,25 +266,25 @@
             self._state.tmp = get_short(data, 8) / 100
             self._state.hum = get_short(data, 10) / 100
             self._state.vpd = get_short(data, 12) / 100
             self._state.fan_type = get_short(data, 14)
             self._state.fan_state = get_bits(data[16], 0, 2)
             # self._state.fan = get_bits(data[17], 0, 4) # Not accurate
             self._state.work_type = get_bits(data[17], 4, 4)
+            self._fire_callbacks(CallbackType.NOTIFICATION)
 
         if data[0] == 0xA5 and data[1] == 0x17 and len(data) == 63:
             self._state.work_type = data[12]
             self._state.level_off = data[15]
             self._state.level_on = data[18]
             if self._state.work_type == 1:
                 self._state.fan = self._state.level_off
             if self._state.work_type == 2:
                 self._state.fan = self._state.level_on
-
-        self._fire_callbacks()
+            self._fire_callbacks(CallbackType.UPDATE_RESPONSE)
 
     def _reset_disconnect_timer(self) -> None:
         """Reset disconnect timer."""
         if self._disconnect_timer:
             self._disconnect_timer.cancel()
         self._expected_disconnect = False
         self._disconnect_timer = self.loop.call_later(
```

### Comparing `ac_infinity_ble-0.2.0/src/ac_infinity_ble/models.py` & `ac_infinity_ble-0.3.0/src/ac_infinity_ble/models.py`

 * *Files identical despite different names*

### Comparing `ac_infinity_ble-0.2.0/src/ac_infinity_ble/protocol.py` & `ac_infinity_ble-0.3.0/src/ac_infinity_ble/protocol.py`

 * *Files identical despite different names*

### Comparing `ac_infinity_ble-0.2.0/src/ac_infinity_ble/util.py` & `ac_infinity_ble-0.3.0/src/ac_infinity_ble/util.py`

 * *Files identical despite different names*

### Comparing `ac_infinity_ble-0.2.0/PKG-INFO` & `ac_infinity_ble-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ac-infinity-ble
-Version: 0.2.0
+Version: 0.3.0
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
-Metadata-Version: 2.1 Name: ac-infinity-ble Version: 0.2.0 Summary: AC Infinity
+Metadata-Version: 2.1 Name: ac-infinity-ble Version: 0.3.0 Summary: AC Infinity
 BLE Controller Home-page: https://github.com/hunterjm/ac-infinity-ble License:
 MIT Author: Jason Hunter Author-email: hunterjm@gmail.com Requires-Python:
 >=3.10,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

