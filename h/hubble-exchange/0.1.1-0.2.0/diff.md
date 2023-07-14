# Comparing `tmp/hubble_exchange-0.1.1.tar.gz` & `tmp/hubble_exchange-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hubble_exchange-0.1.1.tar", last modified: Fri Jun 30 07:14:10 2023, max compression
+gzip compressed data, was "hubble_exchange-0.2.0.tar", last modified: Fri Jul 14 06:48:56 2023, max compression
```

## Comparing `hubble_exchange-0.1.1.tar` & `hubble_exchange-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-06-30 07:14:10.299959 hubble_exchange-0.1.1/
--rw-r--r--   0 shubham    (501) staff       (20)     1072 2023-06-28 09:55:40.000000 hubble_exchange-0.1.1/LICENSE
--rw-r--r--   0 shubham    (501) staff       (20)      101 2023-06-29 11:35:24.000000 hubble_exchange-0.1.1/MANIFEST.in
--rw-r--r--   0 shubham    (501) staff       (20)     1516 2023-06-30 07:14:10.299781 hubble_exchange-0.1.1/PKG-INFO
--rw-r--r--   0 shubham    (501) staff       (20)     2068 2023-06-29 11:42:50.000000 hubble_exchange-0.1.1/README.md
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-06-30 07:14:10.298042 hubble_exchange-0.1.1/hubble_exchange/
--rw-r--r--   0 shubham    (501) staff       (20)      187 2023-06-28 16:09:21.000000 hubble_exchange-0.1.1/hubble_exchange/__init__.py
--rw-r--r--   0 shubham    (501) staff       (20)     5629 2023-06-30 06:44:07.000000 hubble_exchange-0.1.1/hubble_exchange/client.py
--rw-r--r--   0 shubham    (501) staff       (20)      205 2023-06-30 06:22:24.000000 hubble_exchange-0.1.1/hubble_exchange/constants.py
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-06-30 07:14:10.299122 hubble_exchange-0.1.1/hubble_exchange/contract_abis/
--rw-r--r--   0 shubham    (501) staff       (20)    23029 2023-06-28 04:43:57.000000 hubble_exchange-0.1.1/hubble_exchange/contract_abis/OrderBook.json
--rw-r--r--   0 shubham    (501) staff       (20)     1170 2023-06-30 06:41:16.000000 hubble_exchange-0.1.1/hubble_exchange/eip712.py
--rw-r--r--   0 shubham    (501) staff       (20)     2384 2023-06-29 08:43:56.000000 hubble_exchange-0.1.1/hubble_exchange/models.py
--rw-r--r--   0 shubham    (501) staff       (20)     3487 2023-06-30 06:39:11.000000 hubble_exchange-0.1.1/hubble_exchange/order_book.py
--rw-r--r--   0 shubham    (501) staff       (20)     1592 2023-06-29 08:55:15.000000 hubble_exchange-0.1.1/hubble_exchange/utils.py
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-06-30 07:14:10.298879 hubble_exchange-0.1.1/hubble_exchange.egg-info/
--rw-r--r--   0 shubham    (501) staff       (20)     1516 2023-06-30 07:14:10.000000 hubble_exchange-0.1.1/hubble_exchange.egg-info/PKG-INFO
--rw-r--r--   0 shubham    (501) staff       (20)      482 2023-06-30 07:14:10.000000 hubble_exchange-0.1.1/hubble_exchange.egg-info/SOURCES.txt
--rw-r--r--   0 shubham    (501) staff       (20)        1 2023-06-30 07:14:10.000000 hubble_exchange-0.1.1/hubble_exchange.egg-info/dependency_links.txt
--rw-r--r--   0 shubham    (501) staff       (20)      112 2023-06-30 07:14:10.000000 hubble_exchange-0.1.1/hubble_exchange.egg-info/requires.txt
--rw-r--r--   0 shubham    (501) staff       (20)       16 2023-06-30 07:14:10.000000 hubble_exchange-0.1.1/hubble_exchange.egg-info/top_level.txt
--rw-r--r--   0 shubham    (501) staff       (20)      896 2023-06-30 07:13:13.000000 hubble_exchange-0.1.1/pyproject.toml
--rw-r--r--   0 shubham    (501) staff       (20)       38 2023-06-30 07:14:10.300020 hubble_exchange-0.1.1/setup.cfg
--rw-r--r--   0 shubham    (501) staff       (20)       69 2023-06-29 07:08:06.000000 hubble_exchange-0.1.1/setup.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-07-14 06:48:56.445812 hubble_exchange-0.2.0/
+-rw-r--r--   0 shubham    (501) staff       (20)     1072 2023-06-28 09:55:40.000000 hubble_exchange-0.2.0/LICENSE
+-rw-r--r--   0 shubham    (501) staff       (20)      101 2023-06-29 11:35:24.000000 hubble_exchange-0.2.0/MANIFEST.in
+-rw-r--r--   0 shubham    (501) staff       (20)     5428 2023-07-14 06:48:56.445633 hubble_exchange-0.2.0/PKG-INFO
+-rw-r--r--   0 shubham    (501) staff       (20)     3771 2023-07-14 06:35:59.000000 hubble_exchange-0.2.0/README.md
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-07-14 06:48:56.442436 hubble_exchange-0.2.0/hubble_exchange/
+-rw-r--r--   0 shubham    (501) staff       (20)      351 2023-07-14 06:05:29.000000 hubble_exchange-0.2.0/hubble_exchange/__init__.py
+-rw-r--r--   0 shubham    (501) staff       (20)     5271 2023-07-14 06:05:29.000000 hubble_exchange-0.2.0/hubble_exchange/client.py
+-rw-r--r--   0 shubham    (501) staff       (20)      202 2023-07-14 06:05:29.000000 hubble_exchange-0.2.0/hubble_exchange/constants.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-07-14 06:48:56.444964 hubble_exchange-0.2.0/hubble_exchange/contract_abis/
+-rw-r--r--   0 shubham    (501) staff       (20)    23029 2023-06-28 04:43:57.000000 hubble_exchange-0.2.0/hubble_exchange/contract_abis/OrderBook.json
+-rw-r--r--   0 shubham    (501) staff       (20)     1200 2023-07-14 06:05:29.000000 hubble_exchange-0.2.0/hubble_exchange/eip712.py
+-rw-r--r--   0 shubham    (501) staff       (20)       84 2023-07-14 06:05:29.000000 hubble_exchange-0.2.0/hubble_exchange/errors.py
+-rw-r--r--   0 shubham    (501) staff       (20)     5038 2023-07-14 06:05:29.000000 hubble_exchange-0.2.0/hubble_exchange/eth.py
+-rw-r--r--   0 shubham    (501) staff       (20)     2389 2023-07-14 06:14:28.000000 hubble_exchange-0.2.0/hubble_exchange/models.py
+-rw-r--r--   0 shubham    (501) staff       (20)     4407 2023-07-14 06:05:29.000000 hubble_exchange-0.2.0/hubble_exchange/order_book.py
+-rw-r--r--   0 shubham    (501) staff       (20)      466 2023-07-14 06:05:29.000000 hubble_exchange-0.2.0/hubble_exchange/utils.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-07-14 06:48:56.443193 hubble_exchange-0.2.0/hubble_exchange.egg-info/
+-rw-r--r--   0 shubham    (501) staff       (20)     5428 2023-07-14 06:48:56.000000 hubble_exchange-0.2.0/hubble_exchange.egg-info/PKG-INFO
+-rw-r--r--   0 shubham    (501) staff       (20)      531 2023-07-14 06:48:56.000000 hubble_exchange-0.2.0/hubble_exchange.egg-info/SOURCES.txt
+-rw-r--r--   0 shubham    (501) staff       (20)        1 2023-07-14 06:48:56.000000 hubble_exchange-0.2.0/hubble_exchange.egg-info/dependency_links.txt
+-rw-r--r--   0 shubham    (501) staff       (20)      112 2023-07-14 06:48:56.000000 hubble_exchange-0.2.0/hubble_exchange.egg-info/requires.txt
+-rw-r--r--   0 shubham    (501) staff       (20)       16 2023-07-14 06:48:56.000000 hubble_exchange-0.2.0/hubble_exchange.egg-info/top_level.txt
+-rw-r--r--   0 shubham    (501) staff       (20)     1035 2023-07-14 06:46:26.000000 hubble_exchange-0.2.0/pyproject.toml
+-rw-r--r--   0 shubham    (501) staff       (20)       38 2023-07-14 06:48:56.445858 hubble_exchange-0.2.0/setup.cfg
+-rw-r--r--   0 shubham    (501) staff       (20)       69 2023-06-29 07:08:06.000000 hubble_exchange-0.2.0/setup.py
```

### Comparing `hubble_exchange-0.1.1/LICENSE` & `hubble_exchange-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.1.1/hubble_exchange/client.py` & `hubble_exchange-0.2.0/hubble_exchange/client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,81 +1,46 @@
 import json
-import random
-import time
-import requests
+from typing import Any, Callable, List
+
 import websocket
-from typing import List, Callable, Any
 from hexbytes import HexBytes
-from hubble_exchange.models import (
-    Order,
-    OrderStatusResponse,
-    OrderBookDepthResponse,
-    GetPositionsResponse,
-    OrderBookDepthUpdateResponse,
-    WebsocketResponse,
-)
+
+from hubble_exchange.eth import (get_web3_client,
+                                 get_websocket_endpoint)
+from hubble_exchange.models import (GetPositionsResponse, Order,
+                                    OrderBookDepthResponse,
+                                    OrderBookDepthUpdateResponse,
+                                    OrderStatusResponse, WebsocketResponse)
 from hubble_exchange.order_book import OrderBookClient
-from hubble_exchange.utils import (
-    get_rpc_endpoint,
-    get_websocket_endpoint,
-    float_to_scaled_int,
-    get_address_from_private_key,
-    get_new_salt,
-)
+from hubble_exchange.utils import (float_to_scaled_int,
+                                   get_address_from_private_key, get_new_salt)
 
 
 class HubbleClient:
     def __init__(self, private_key: str):
         if not private_key:
             raise ValueError("Private key is not set")
         self.trader_address = get_address_from_private_key(private_key)
         if not self.trader_address:
             raise ValueError("Cannot determine trader address from private key")
 
-        self.rpc_endpoint = get_rpc_endpoint()
+        self.web3_client = get_web3_client()
         self.websocket_endpoint = get_websocket_endpoint()
-        self.orderBookClient = OrderBookClient(private_key)
+        self.order_book_client = OrderBookClient(private_key)
 
     def get_order_book(self, market: int) -> OrderBookDepthResponse:
-        request_body = {
-            "jsonrpc": "2.0",
-            "id": 1,
-            "method": "trading_getTradingOrderBookDepth",
-            "params": [market],
-        }
-        response = requests.post(self.rpc_endpoint, json=request_body)
-        response_json = response.json()
-        order_book = OrderBookDepthResponse(**response_json["result"])
-        return order_book
+        return self.web3_client.eth.get_order_book_depth(market)
 
     def get_margin_and_positions(self) -> GetPositionsResponse:
-        request_body = {
-            "jsonrpc": "2.0",
-            "id": 1,
-            "method": "trading_getMarginAndPositions",
-            "params": [self.trader_address],
-        }
-        response = requests.post(self.rpc_endpoint, json=request_body)
-        response_json = response.json()
-        positions = GetPositionsResponse(**response_json["result"])
-        return positions
+        return self.web3_client.eth.get_margin_and_positions(self.trader_address)
 
     def get_order_status(self, order_id: HexBytes) -> OrderStatusResponse:
-        request_body = {
-            "jsonrpc": "2.0",
-            "id": 1,
-            "method": "trading_getOrderStatus",
-            "params": [order_id.hex()],
-        }
-        response = requests.post(self.rpc_endpoint, json=request_body)
-        response_json = response.json()
-        order_status = OrderStatusResponse(**response_json["result"])
-        return order_status
+        return self.web3_client.eth.get_order_status(order_id.hex())
 
-    def place_orders(self, orders: List[Order]) -> List[Order]:
+    def place_orders(self, orders: List[Order], tx_options = None, mode=None) -> List[Order]:
         if len(orders) > 75:
             raise ValueError("Cannot place more than 75 orders at once")
 
         for order in orders:
             if order.amm_index is None:
                 raise ValueError("Order AMM index is not set")
             if order.base_asset_quantity is None:
@@ -87,46 +52,51 @@
 
             # trader and salt can be set automatically
             if order.trader in [None, "0x", ""]:
                 order.trader = self.trader_address
             if order.salt in [None, 0]:
                 order.salt = get_new_salt()
 
-        return self.orderBookClient.place_orders(orders)
+        return self.order_book_client.place_orders(orders, tx_options, mode)
 
     def place_single_order(
-        self, market: int, base_asset_quantity: float, price: float, reduce_only: bool
+        self, market: int, base_asset_quantity: float, price: float, reduce_only: bool, tx_options = None, mode=None
     ) -> Order:
         order = Order(
             id=None,
             amm_index=market,
             trader=self.trader_address,
             base_asset_quantity=float_to_scaled_int(base_asset_quantity, 18),
             price=float_to_scaled_int(price, 6),
             salt=get_new_salt(),
             reduce_only=reduce_only,
         )
-        order_hash = self.orderBookClient.place_order(order)
+        order_hash = self.order_book_client.place_order(order, tx_options, mode)
         order.id = order_hash
         return order
 
-    def cancel_orders(self, orders: List[Order]) -> None:
-        self.orderBookClient.cancel_orders(orders)
+    def cancel_orders(self, orders: List[Order], tx_options = None, mode=None) -> None:
+        if len(orders) > 100:
+            raise ValueError("Cannot cancel more than 100 orders at once")
+
+        self.order_book_client.cancel_orders(orders, tx_options, mode)
 
-    def cancel_order_by_id(self, order_id: HexBytes) -> None:
+    def cancel_order_by_id(self, order_id: HexBytes, tx_options = None, mode=None) -> None:
         order_status = self.get_order_status(order_id)
+        position_side_multiplier = 1 if order_status.positionSide == "LONG" else -1
         order = Order(
-            amm_index=order_status.Symbol,
+            id=order_id.hex(),
+            amm_index=order_status.symbol,
             trader=self.trader_address,
-            base_asset_quantity=float_to_scaled_int(order_status.OrigQty, 18),
-            price=float_to_scaled_int(order_status.Price, 6),
-            salt=order_status.Salt,
-            reduce_only=order_status.ReduceOnly,
+            base_asset_quantity=float_to_scaled_int(float(order_status.origQty) * position_side_multiplier, 18),
+            price=float_to_scaled_int(float(order_status.price), 6),
+            salt=int(order_status.salt),
+            reduce_only=order_status.reduceOnly,
         )
-        self.cancel_orders([order])
+        self.cancel_orders([order], tx_options, mode)
 
     def subscribe_to_order_book_depth(
         self, market: int, callback: Callable[[websocket.WebSocketApp, OrderBookDepthUpdateResponse], Any]
     ) -> None:
 
         def on_open(ws):
             msg = {
```

### Comparing `hubble_exchange-0.1.1/hubble_exchange/contract_abis/OrderBook.json` & `hubble_exchange-0.2.0/hubble_exchange/contract_abis/OrderBook.json`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.1.1/hubble_exchange/eip712.py` & `hubble_exchange-0.2.0/hubble_exchange/eip712.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from eip712_structs import make_domain, EIP712Struct, Uint, Address, Int, Boolean
+from eip712_structs import (Address, Boolean, EIP712Struct, Int, Uint,
+                            make_domain)
 from eth_utils import keccak
 from hexbytes import HexBytes
 
-from hubble_exchange.constants import OrderBookContractAddress, CHAIN_ID
+from hubble_exchange.constants import CHAIN_ID, OrderBookContractAddress
 from hubble_exchange.models import Order as OrderModel
 
 domain = make_domain(name='Hubble', version="2.0", chainId=CHAIN_ID, verifyingContract=OrderBookContractAddress)
 domain_hash = HexBytes(domain.hash_struct())
 
 
 # Class name must match the struct name in the solidity contract
```

### Comparing `hubble_exchange-0.1.1/hubble_exchange/models.py` & `hubble_exchange-0.2.0/hubble_exchange/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from dataclasses import dataclass
 from typing import List
+
 from eth_typing import Address
 from hexbytes import HexBytes
 
 from hubble_exchange.utils import float_to_scaled_int, get_new_salt
 
 
 @dataclass
@@ -23,15 +24,15 @@
             "baseAssetQuantity": self.base_asset_quantity,
             "price": self.price,
             "salt": self.salt,
             "reduceOnly": self.reduce_only,
         }
 
     @classmethod
-    def new(cls, amm_index: int, base_asset_quantity: int, price: int, reduce_only: bool):
+    def new(cls, amm_index: int, base_asset_quantity: float, price: float, reduce_only: bool):
         """
         Create a new order with a random salt and no ID or trader. This can be used for placing
         multiple orders at once.
         """
         return cls(
             id=None,
             amm_index=amm_index,
@@ -57,17 +58,17 @@
     updateTime: int
     salt: int
 
 
 @dataclass
 class OrderBookDepthResponse:
     lastUpdateId: int
-    symbol: int
     E: int
     T: int
+    symbol: int
     bids: List[List[str]]
     asks: List[List[str]]
 
 
 class Market(int):
     pass
```

### Comparing `hubble_exchange-0.1.1/pyproject.toml` & `hubble_exchange-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -6,25 +6,29 @@
 author_email = "lumos@hubble.exchange"
 long_description = {file = "README.md"}
 long_description_content_type = "text/markdown"
 url = "https://github.com/hubble-exchange/python-sdk"
 
 [project]
 name = "hubble_exchange"
-version = "0.1.1"
+version = "0.2.0"
 description = "Official python SDK for Hubble Exchange"
 authors = [{name = "Lumos", email = "lumos@hubble.exchange"}]
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 dependencies = [
     "web3 >= 6.5.0",
     "eth_typing >= 3.4.0",
     "eth_account >= 0.8.0",
     "requests >= 2.31.0",
     "websocket-client >= 1.6.0",
     "eip712-structs >= 1.1.0",
 ]
-keywords = ["hubble", "exchange", "perpetual", "futures", "sdk", "python", "ethereum", "web3"]
+readme = "README.md"
+keywords = ["hubble", "exchange", "orderbook", "perpetual", "futures", "dex", "sdk", "python", "avalanche", "ethereum", "web3", "crypto"]
 
 [tool.setuptools]
 packages = ["hubble_exchange", "hubble_exchange.contract_abis"]
 include-package-data = true
+
+[project.urls]
+homepage = "https://github.com/hubble-exchange/python-sdk"
```

