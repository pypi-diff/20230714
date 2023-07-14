# Comparing `tmp/aiocomelit-0.0.2.tar.gz` & `tmp/aiocomelit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiocomelit-0.0.2.tar", max compression
+gzip compressed data, was "aiocomelit-0.0.3.tar", max compression
```

## Comparing `aiocomelit-0.0.2.tar` & `aiocomelit-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11346 2023-07-04 19:31:04.621003 aiocomelit-0.0.2/LICENSE
--rw-r--r--   0        0        0     3306 2023-07-04 19:31:04.721003 aiocomelit-0.0.2/README.md
--rw-r--r--   0        0        0     1940 2023-07-08 10:59:45.676430 aiocomelit-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      420 2023-07-08 10:59:45.676430 aiocomelit-0.0.2/src/aiocomelit/__init__.py
--rw-r--r--   0        0        0     7833 2023-07-08 10:59:45.676430 aiocomelit-0.0.2/src/aiocomelit/api.py
--rw-r--r--   0        0        0      319 2023-07-05 21:05:53.271526 aiocomelit-0.0.2/src/aiocomelit/const.py
--rw-r--r--   0        0        0      441 2023-07-05 21:05:53.271526 aiocomelit-0.0.2/src/aiocomelit/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-04 19:31:04.451003 aiocomelit-0.0.2/src/aiocomelit/py.typed
--rw-r--r--   0        0        0     4322 1970-01-01 00:00:00.000000 aiocomelit-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-07-04 19:31:04.621003 aiocomelit-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3306 2023-07-04 19:31:04.721003 aiocomelit-0.0.3/README.md
+-rw-r--r--   0        0        0     1940 2023-07-14 12:48:05.775671 aiocomelit-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      420 2023-07-14 12:48:05.775671 aiocomelit-0.0.3/src/aiocomelit/__init__.py
+-rw-r--r--   0        0        0     8175 2023-07-14 12:48:05.775671 aiocomelit-0.0.3/src/aiocomelit/api.py
+-rw-r--r--   0        0        0      388 2023-07-14 12:48:05.775671 aiocomelit-0.0.3/src/aiocomelit/const.py
+-rw-r--r--   0        0        0      441 2023-07-05 21:05:53.271526 aiocomelit-0.0.3/src/aiocomelit/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-04 19:31:04.451003 aiocomelit-0.0.3/src/aiocomelit/py.typed
+-rw-r--r--   0        0        0     4322 1970-01-01 00:00:00.000000 aiocomelit-0.0.3/PKG-INFO
```

### Comparing `aiocomelit-0.0.2/LICENSE` & `aiocomelit-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aiocomelit-0.0.2/README.md` & `aiocomelit-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `aiocomelit-0.0.2/pyproject.toml` & `aiocomelit-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiocomelit"
-version = "0.0.2"
+version = "0.0.3"
 description = "Python library to control Comelit Simplehome"
 authors = ["Simone Chemelli <simone.chemelli@gmail.com>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 repository = "https://github.com/chemelli74/aiocomelit"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
```

### Comparing `aiocomelit-0.0.2/src/aiocomelit/api.py` & `aiocomelit-0.0.3/src/aiocomelit/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,14 +141,23 @@
         """Makes status human readable."""
 
         if dev_type == COVER:
             return COVER_STATUS[dev_status]
 
         return "on" if dev_status == 1 else "off"
 
+    async def light_switch(self, index: int, action: int) -> bool:
+        """Set status of the light."""
+        return await self._set_device_status(LIGHT, index, action)
+
+    async def cover_move(self, index: int, action: int) -> bool:
+        """Move cover up/down."""
+
+        return await self._set_device_status(COVER, index, action)
+
     async def get_all_devices(self) -> list[ComelitSerialBridgeObject]:
         """Get all connected devices."""
 
         _LOGGER.debug("Getting all devices for host %s", self.host)
 
         for dev_type in (CLIMATE, COVER, LIGHT, OTHER):
             reply_json = await self._get_devices(dev_type)
```

### Comparing `aiocomelit-0.0.2/PKG-INFO` & `aiocomelit-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocomelit
-Version: 0.0.2
+Version: 0.0.3
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
-Metadata-Version: 2.1 Name: aiocomelit Version: 0.0.2 Summary: Python library
+Metadata-Version: 2.1 Name: aiocomelit Version: 0.0.3 Summary: Python library
 to control Comelit Simplehome Home-page: https://github.com/chemelli74/
 aiocomelit License: Apache Software License 2.0 Author: Simone Chemelli Author-
 email: simone.chemelli@gmail.com Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License Classifier: Natural Language
 :: English Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

