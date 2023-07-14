# Comparing `tmp/geckoterminal_py-0.1.1.tar.gz` & `tmp/geckoterminal_py-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geckoterminal_py-0.1.1.tar", max compression
+gzip compressed data, was "geckoterminal_py-0.1.2.tar", max compression
```

## Comparing `geckoterminal_py-0.1.1.tar` & `geckoterminal_py-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-07-07 16:16:21.780816 geckoterminal_py-0.1.1/LICENSE
--rw-r--r--   0        0        0     2964 2023-07-13 21:58:39.762420 geckoterminal_py-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-07-07 16:16:21.784451 geckoterminal_py-0.1.1/geckoterminal_py/__init__.py
--rw-r--r--   0        0        0     9325 2023-07-13 21:58:39.762642 geckoterminal_py-0.1.1/geckoterminal_py/client.py
--rw-r--r--   0        0        0      600 2023-07-13 18:35:42.614243 geckoterminal_py-0.1.1/geckoterminal_py/constants.py
--rw-r--r--   0        0        0      789 2023-07-13 21:58:39.763538 geckoterminal_py-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3561 1970-01-01 00:00:00.000000 geckoterminal_py-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-07 16:16:21.780816 geckoterminal_py-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2992 2023-07-14 04:36:57.323188 geckoterminal_py-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-07 16:16:21.784451 geckoterminal_py-0.1.2/geckoterminal_py/__init__.py
+-rw-r--r--   0        0        0     9254 2023-07-14 04:54:51.682042 geckoterminal_py-0.1.2/geckoterminal_py/client.py
+-rw-r--r--   0        0        0      600 2023-07-13 18:35:42.614243 geckoterminal_py-0.1.2/geckoterminal_py/constants.py
+-rw-r--r--   0        0        0      788 2023-07-14 04:49:14.605507 geckoterminal_py-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3688 1970-01-01 00:00:00.000000 geckoterminal_py-0.1.2/PKG-INFO
```

### Comparing `geckoterminal_py-0.1.1/LICENSE` & `geckoterminal_py-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `geckoterminal_py-0.1.1/README.md` & `geckoterminal_py-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # GeckoTerminal Py
 
-GeckoTerminal Py is a Python client for the [GeckoTerminal API](https://api.geckoterminal.com/api/v2). It provides a user-friendly way to fetch network and pool data asynchronously or synchronously.
+GeckoTerminal Py is a Python client for the [GeckoTerminal](https://www.geckoterminal.com). It provides a user-friendly way to fetch network and pool data asynchronously or synchronously.
 
 ## Installation
 
 To install GeckoTerminal Py, use pip:
 
 ```bash
 pip install geckoterminal-py
@@ -22,28 +22,30 @@
 import asyncio
 
 
 async def main():
     client = GeckoTerminalClient()
     networks_df = await client.get_networks()
     print(networks_df)
+    client.close()
 
 # In an asyncio environment, you'd use:
 asyncio.run(main())
 ```
 
 ### Synchronous usage
 
 ```python
 from geckoterminal_py.client import GeckoTerminalClient
 
 def main():
     client = GeckoTerminalClient()
     networks_df = client.get_networks_sync()
     print(networks_df)
+    client.close()
 
 main()
 ```
 
 ## Methods Available
 
 Here is a brief description of the methods available in the GeckoTerminalClient:
@@ -62,8 +64,8 @@
 - **get_networks_sync():** Fetches network data in a synchronous way.
 - **get_dexes_by_network_sync(network_id: str):** Synchronously fetches dex data by network ID.
 - **get_top_pools_by_network_sync(network_id: str):** Synchronously fetches top pool data by network ID.
 - **get_top_pools_by_network_dex_sync(network_id: str, dex_id: str):** Synchronously fetches top pool data by network and dex IDs.
 - **get_top_pools_by_network_token_sync(network_id: str, token_id: str):** Synchronously fetches top pool data by network and token IDs.
 - **get_new_pools_by_network_sync(network_id: str):** Synchronously fetches data of new pools by network ID.
 - **get_new_pools_all_networks_sync():** Synchronously fetches data of new pools across all networks.
-- **get_ohlcv_sync(network_id: str, pool_address: str, timeframe: str, before_timestamp: int = None, currency: str = "usd", token: str = "base", limit: int = 1000):** Synchronously fetches OHLCV data for a pool.
+- **get_ohlcv_sync(network_id: str, pool_address: str, timeframe: str, before_timestamp: int = None, currency: str = "usd", token: str = "base", limit: int = 1000):** Synchronously fetches OHLCV data for a pool.
```

### Comparing `geckoterminal_py-0.1.1/geckoterminal_py/client.py` & `geckoterminal_py-0.1.2/geckoterminal_py/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,26 +143,29 @@
         return self.process_pools_list(new_pools_all_networks)
 
     def get_new_pools_all_networks_sync(self) -> pd.DataFrame:
         return self.ev_loop.run_until_complete(self.get_new_pools_all_networks())
 
     async def get_ohlcv(self, network_id: str, pool_address: str, timeframe: str, before_timestamp: int = None,
                         currency: str = "usd", token: str = "base", limit: int = 1000) -> pd.DataFrame:
+        if timeframe not in self.ohlcv_timeframes:
+            raise ValueError(f"Timeframe {timeframe} is not supported. Please select one timeframe of the following"
+                             f"list {self.ohlcv_timeframes}")
         timeframe, period = self.get_timeframe_and_period(timeframe)
+        params = {
+            "aggregate": period,
+            "limit": limit,
+            "currency": currency,
+            "token": token,
+        }
+        if before_timestamp:
+            params["before_timestamp"] = before_timestamp
         response = await self.api_request("GET",
-                                          CONSTANTS.GET_OHLCV_DATA_PATH.format(network_id,
-                                                                               pool_address,
-                                                                               timeframe),
-                                          params={
-                                              "before_timestamp": before_timestamp,
-                                              "aggregate": period,
-                                              "limit": limit,
-                                              "currency": currency,
-                                              "token": token,
-                                          })
+                                          CONSTANTS.GET_OHLCV_DATA_PATH.format(network_id, pool_address, timeframe),
+                                          params=params)
 
         df = pd.DataFrame(response["data"]["attributes"]["ohlcv_list"],
                           columns=["timestamp", "open", "high", "low", "close", "volume_usd"])
         df["datetime"] = pd.to_datetime(df["timestamp"], unit="s")
         return df.drop_duplicates(subset="timestamp").sort_values("datetime").reset_index(drop=True)
 
     def get_ohlcv_sync(self, network_id: str, pool_address: str, timeframe: str, before_timestamp: int = None,
```

### Comparing `geckoterminal_py-0.1.1/geckoterminal_py/constants.py` & `geckoterminal_py-0.1.2/geckoterminal_py/constants.py`

 * *Files identical despite different names*

### Comparing `geckoterminal_py-0.1.1/pyproject.toml` & `geckoterminal_py-0.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "geckoterminal-py"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["cardosofede <federico.cardoso.e@gmail.com>"]
 readme = "README.md"
 packages = [{include = "geckoterminal_py"}]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.8"
 aiohttp = "^3.8.4"
 aiodns = "^3.0.0"
 cchardet = "^2.1.7"
 aioresponses = "^0.7.4"
 glom = "^23.3.0"
 pandas = "^2.0.3"
```

### Comparing `geckoterminal_py-0.1.1/PKG-INFO` & `geckoterminal_py-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: geckoterminal-py
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: cardosofede
 Author-email: federico.cardoso.e@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiodns (>=3.0.0,<4.0.0)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: aioresponses (>=0.7.4,<0.8.0)
 Requires-Dist: cchardet (>=2.1.7,<3.0.0)
 Requires-Dist: glom (>=23.3.0,<24.0.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Description-Content-Type: text/markdown
 
 # GeckoTerminal Py
 
-GeckoTerminal Py is a Python client for the [GeckoTerminal API](https://api.geckoterminal.com/api/v2). It provides a user-friendly way to fetch network and pool data asynchronously or synchronously.
+GeckoTerminal Py is a Python client for the [GeckoTerminal](https://www.geckoterminal.com). It provides a user-friendly way to fetch network and pool data asynchronously or synchronously.
 
 ## Installation
 
 To install GeckoTerminal Py, use pip:
 
 ```bash
 pip install geckoterminal-py
@@ -40,28 +42,30 @@
 import asyncio
 
 
 async def main():
     client = GeckoTerminalClient()
     networks_df = await client.get_networks()
     print(networks_df)
+    client.close()
 
 # In an asyncio environment, you'd use:
 asyncio.run(main())
 ```
 
 ### Synchronous usage
 
 ```python
 from geckoterminal_py.client import GeckoTerminalClient
 
 def main():
     client = GeckoTerminalClient()
     networks_df = client.get_networks_sync()
     print(networks_df)
+    client.close()
 
 main()
 ```
 
 ## Methods Available
 
 Here is a brief description of the methods available in the GeckoTerminalClient:
@@ -81,7 +85,8 @@
 - **get_dexes_by_network_sync(network_id: str):** Synchronously fetches dex data by network ID.
 - **get_top_pools_by_network_sync(network_id: str):** Synchronously fetches top pool data by network ID.
 - **get_top_pools_by_network_dex_sync(network_id: str, dex_id: str):** Synchronously fetches top pool data by network and dex IDs.
 - **get_top_pools_by_network_token_sync(network_id: str, token_id: str):** Synchronously fetches top pool data by network and token IDs.
 - **get_new_pools_by_network_sync(network_id: str):** Synchronously fetches data of new pools by network ID.
 - **get_new_pools_all_networks_sync():** Synchronously fetches data of new pools across all networks.
 - **get_ohlcv_sync(network_id: str, pool_address: str, timeframe: str, before_timestamp: int = None, currency: str = "usd", token: str = "base", limit: int = 1000):** Synchronously fetches OHLCV data for a pool.
+
```

