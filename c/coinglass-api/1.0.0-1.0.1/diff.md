# Comparing `tmp/coinglass_api-1.0.0.tar.gz` & `tmp/coinglass_api-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coinglass_api-1.0.0.tar", max compression
+gzip compressed data, was "coinglass_api-1.0.1.tar", max compression
```

## Comparing `coinglass_api-1.0.0.tar` & `coinglass_api-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1069 2023-01-15 20:06:02.595582 coinglass_api-1.0.0/LICENSE.md
--rw-r--r--   0        0        0     4426 2023-07-07 16:17:16.974156 coinglass_api-1.0.0/README.md
--rw-r--r--   0        0        0      122 2023-07-07 14:56:03.702274 coinglass_api-1.0.0/coinglass_api/__init__.py
--rw-r--r--   0        0        0    31118 2023-07-07 16:00:32.778643 coinglass_api-1.0.0/coinglass_api/api.py
--rw-r--r--   0        0        0      809 2023-07-07 16:15:36.754227 coinglass_api-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     5170 1970-01-01 00:00:00.000000 coinglass_api-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-01-15 20:06:02.595582 coinglass_api-1.0.1/LICENSE.md
+-rw-r--r--   0        0        0     4427 2023-07-07 22:54:36.965648 coinglass_api-1.0.1/README.md
+-rw-r--r--   0        0        0      261 2023-07-11 10:54:46.783124 coinglass_api-1.0.1/coinglass_api/__init__.py
+-rw-r--r--   0        0        0    31200 2023-07-11 10:54:46.791160 coinglass_api-1.0.1/coinglass_api/api.py
+-rw-r--r--   0        0        0      715 2023-07-11 10:55:20.071147 coinglass_api-1.0.1/coinglass_api/exceptions.py
+-rw-r--r--   0        0        0      809 2023-07-11 11:04:47.849241 coinglass_api-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5171 1970-01-01 00:00:00.000000 coinglass_api-1.0.1/PKG-INFO
```

### Comparing `coinglass_api-1.0.0/LICENSE.md` & `coinglass_api-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `coinglass_api-1.0.0/README.md` & `coinglass_api-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 [![PyPi version](https://img.shields.io/pypi/v/coinglass-api)](https://pypi.python.org/pypi/coinglass-api/)
 [![Downloads](https://pepy.tech/badge/coinglass-api)](https://pepy.tech/project/coinglass-api)
 [![codecov](https://codecov.io/gh/dineshpinto/coinglass-api/branch/main/graph/badge.svg?token=XTJRRU2W1T)](https://codecov.io/gh/dineshpinto/coinglass-api)
 [![API unittest](https://github.com/dineshpinto/coinglass-api/actions/workflows/api_unitests.yml/badge.svg)](https://github.com/dineshpinto/coinglass-api/actions/workflows/api_unitests.yml)
 
 ## Unofficial Python client for Coinglass API
 
-Wrapper around the [Coinglass API](https://coinglass.com/pricing) to fetch data about the crypto markets.
+Wrapper around the [Coinglass API](https://coinglass.com/pricing) to fetch data about crypto derivatives.
 All data is output in pandas DataFrames (single or multi-index) and all time-series data uses a `DateTimeIndex`.
-Supports all CoinGlass API endpoints.
+Supports all Coinglass API endpoints.
 
 ![Example Plot](https://github.com/dineshpinto/coinglass-api/blob/main/examples/example_plot.jpg?raw=true)
 
 ## Installation
 
 ```bash
 pip install coinglass-api
@@ -34,21 +34,21 @@
 
 # Funding rate of ETH on dYdX
 fr_btc_dydx = cg.funding(ex="dYdX", pair="ETH-USD", interval="h8")
 
 # Get average funding for BTC
 fr_avg_btc = cg.funding_average(symbol="BTC", interval="h4")
 
-# Get funding OHLC for ETHUSDT on Binance
+# Get funding OHLC for ETH-USDT on Binance
 fr_ohlc_eth_binance = cg.funding_ohlc(ex="Binance", pair="ETHUSDT", interval="h4")
 
 # Get aggregated OI OHLC data for BTC
 oi_agg_eth = cg.open_interest_aggregated_ohlc(symbol="ETH", interval="h4")
 
-# Get OHLC liquidations data for ETHUSDT on dYdX
+# Get OHLC liquidations data for ETH-USD on dYdX
 liq_ohlc_eth_dydx = cg.liquidation_pair(ex="dYdX", pair="ETH-USD", interval="h4")
 
 # Get liquidation data for BTC
 liq_btc = cg.liquidation_symbol(symbol="BTC", interval="h4")
 
 # Get long/short ratios for BTC
 lsr_btc = cg.long_short_symbol(symbol="BTC", interval="h4")
```

### Comparing `coinglass_api-1.0.0/coinglass_api/api.py` & `coinglass_api-1.0.1/coinglass_api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 import pandas as pd
 import requests
 
-
-class RequiresUpgradedPlanException(Exception):
-    """ Raised when an endpoint requires an upgraded plan """
-    pass
-
-
-class RateLimitExceededException(Exception):
-    """ Raised when rate limit is exceeded """
-    pass
+from .exceptions import CoinglassAPIException, CoinglassRequestException, RateLimitExceededException
 
 
 class CoinglassAPI:
     """ Unofficial Python client for Coinglass API """
 
     def __init__(self, coinglass_secret: str):
         """
         Args:
             coinglass_secret: key from Coinglass, get one at https://www.coinglass.com/pricing
         """
         self.__coinglass_secret = coinglass_secret
         self._base_url = "https://open-api.coinglass.com/public/v2/"
         self._session = requests.Session()
 
-    def _get(self, endpoint: str, params: dict = None) -> dict:
+    def _get(self, endpoint: str, params: dict | None = None) -> dict:
         headers = {
             "accept": "application/json",
             "coinglassSecret": self.__coinglass_secret
         }
         url = self._base_url + endpoint
         return self._session.request(
             method='GET',
@@ -124,37 +116,42 @@
 
         return pd.concat(flattened_data, axis=1)
 
     @staticmethod
     def _flatten_dictionary(data: dict) -> dict:
         flattened_dict = {}
 
-        for k, v in data.items():
-            if isinstance(v, dict):
-                for outer_key, outer_value in v.items():
-                    if isinstance(outer_value, list):
-                        flattened_dict[(k, outer_key)] = outer_value
+        for outer_key, outer_value in data.items():
+            if isinstance(outer_value, dict):
+                for inner_key, inner_value in outer_value.items():
+                    if isinstance(inner_value, list):
+                        flattened_dict[(outer_key, inner_key)] = inner_value
                     else:
-                        flattened_dict[outer_key] = outer_value
+                        flattened_dict[inner_key] = inner_value
             else:
-                flattened_dict[(k, 0)] = v
+                flattened_dict[(outer_key, 0)] = outer_value
 
         return flattened_dict
 
     @staticmethod
     def _check_for_errors(response: dict) -> None:
         """ Check for errors in response """
+
+        if "success" not in response.keys():
+            # Handle error case
+            raise CoinglassAPIException(status=response["status"], error=response["error"])
+
         if not response["success"]:
-            match int(response["code"]):
-                case 40001:
-                    raise RequiresUpgradedPlanException(response['msg'])
+            # Handle unsuccessful response
+            code, msg = int(response["code"]), response["msg"]
+            match code:
                 case 50001:
-                    raise RateLimitExceededException(response['msg'])
+                    raise RateLimitExceededException()
                 case _:
-                    raise Exception(f"Code {response['code']}: {response['msg']}")
+                    raise CoinglassRequestException(code=code, msg=msg)
 
     def perpetual_market(self, symbol: str) -> pd.DataFrame:
         response = self._get(
             endpoint="perpetual_market",
             params={"symbol": symbol}
         )
         self._check_for_errors(response)
```

### Comparing `coinglass_api-1.0.0/pyproject.toml` & `coinglass_api-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "coinglass-api"
-version = "1.0.0"
+version = "1.0.1"
 repository = "https://github.com/dineshpinto/coinglass-api"
 homepage = "https://github.com/dineshpinto/coinglass-api"
 license = "MIT"
 keywords = ["coinglass", "api", "crypto", "cryptocurrency", "bitcoin", "ethereum", "binance", "dydx", "okex"]
 description = "Unofficial Python client for Coinglass API"
 authors = ["dineshpinto <annual.fallout_0z@gmail.com>"]
 readme = "README.md"
```

### Comparing `coinglass_api-1.0.0/PKG-INFO` & `coinglass_api-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coinglass-api
-Version: 1.0.0
+Version: 1.0.1
 Summary: Unofficial Python client for Coinglass API
 Home-page: https://github.com/dineshpinto/coinglass-api
 License: MIT
 Keywords: coinglass,api,crypto,cryptocurrency,bitcoin,ethereum,binance,dydx,okex
 Author: dineshpinto
 Author-email: annual.fallout_0z@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -22,17 +22,17 @@
 [![PyPi version](https://img.shields.io/pypi/v/coinglass-api)](https://pypi.python.org/pypi/coinglass-api/)
 [![Downloads](https://pepy.tech/badge/coinglass-api)](https://pepy.tech/project/coinglass-api)
 [![codecov](https://codecov.io/gh/dineshpinto/coinglass-api/branch/main/graph/badge.svg?token=XTJRRU2W1T)](https://codecov.io/gh/dineshpinto/coinglass-api)
 [![API unittest](https://github.com/dineshpinto/coinglass-api/actions/workflows/api_unitests.yml/badge.svg)](https://github.com/dineshpinto/coinglass-api/actions/workflows/api_unitests.yml)
 
 ## Unofficial Python client for Coinglass API
 
-Wrapper around the [Coinglass API](https://coinglass.com/pricing) to fetch data about the crypto markets.
+Wrapper around the [Coinglass API](https://coinglass.com/pricing) to fetch data about crypto derivatives.
 All data is output in pandas DataFrames (single or multi-index) and all time-series data uses a `DateTimeIndex`.
-Supports all CoinGlass API endpoints.
+Supports all Coinglass API endpoints.
 
 ![Example Plot](https://github.com/dineshpinto/coinglass-api/blob/main/examples/example_plot.jpg?raw=true)
 
 ## Installation
 
 ```bash
 pip install coinglass-api
@@ -53,21 +53,21 @@
 
 # Funding rate of ETH on dYdX
 fr_btc_dydx = cg.funding(ex="dYdX", pair="ETH-USD", interval="h8")
 
 # Get average funding for BTC
 fr_avg_btc = cg.funding_average(symbol="BTC", interval="h4")
 
-# Get funding OHLC for ETHUSDT on Binance
+# Get funding OHLC for ETH-USDT on Binance
 fr_ohlc_eth_binance = cg.funding_ohlc(ex="Binance", pair="ETHUSDT", interval="h4")
 
 # Get aggregated OI OHLC data for BTC
 oi_agg_eth = cg.open_interest_aggregated_ohlc(symbol="ETH", interval="h4")
 
-# Get OHLC liquidations data for ETHUSDT on dYdX
+# Get OHLC liquidations data for ETH-USD on dYdX
 liq_ohlc_eth_dydx = cg.liquidation_pair(ex="dYdX", pair="ETH-USD", interval="h4")
 
 # Get liquidation data for BTC
 liq_btc = cg.liquidation_symbol(symbol="BTC", interval="h4")
 
 # Get long/short ratios for BTC
 lsr_btc = cg.long_short_symbol(symbol="BTC", interval="h4")
```

