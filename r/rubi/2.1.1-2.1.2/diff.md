# Comparing `tmp/rubi-2.1.1.tar.gz` & `tmp/rubi-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubi-2.1.1.tar", max compression
+gzip compressed data, was "rubi-2.1.2.tar", max compression
```

## Comparing `rubi-2.1.1.tar` & `rubi-2.1.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    11357 2023-07-10 23:49:14.175642 rubi-2.1.1/LICENSE
--rw-r--r--   0        0        0     2757 2023-07-10 23:49:14.175642 rubi-2.1.1/README.md
--rw-r--r--   0        0        0     6735 2023-07-10 23:49:14.175642 rubi-2.1.1/network_config/ERC20.json
--rw-r--r--   0        0        0     1920 2023-07-10 23:49:14.175642 rubi-2.1.1/network_config/README.md
--rw-r--r--   0        0        0    32732 2023-07-10 23:49:14.179642 rubi-2.1.1/network_config/abitrum_goerli/abis/market.json
--rw-r--r--   0        0        0    15157 2023-07-10 23:49:14.179642 rubi-2.1.1/network_config/abitrum_goerli/abis/router.json
--rw-r--r--   0        0        0      721 2023-07-10 23:49:14.179642 rubi-2.1.1/network_config/abitrum_goerli/network.yaml
--rw-r--r--   0        0        0    32732 2023-07-10 23:49:14.179642 rubi-2.1.1/network_config/optimism/abis/market.json
--rw-r--r--   0        0        0    15157 2023-07-10 23:49:14.179642 rubi-2.1.1/network_config/optimism/abis/router.json
--rw-r--r--   0        0        0      745 2023-07-10 23:49:14.179642 rubi-2.1.1/network_config/optimism/network.yaml
--rw-r--r--   0        0        0    32732 2023-07-10 23:49:14.179642 rubi-2.1.1/network_config/optimism_goerli/abis/market.json
--rw-r--r--   0        0        0    15157 2023-07-10 23:49:14.179642 rubi-2.1.1/network_config/optimism_goerli/abis/router.json
--rw-r--r--   0        0        0      648 2023-07-10 23:49:14.179642 rubi-2.1.1/network_config/optimism_goerli/network.yaml
--rw-r--r--   0        0        0    32732 2023-07-10 23:49:14.179642 rubi-2.1.1/network_config/polygon_mumbai/abis/market.json
--rw-r--r--   0        0        0    15157 2023-07-10 23:49:14.179642 rubi-2.1.1/network_config/polygon_mumbai/abis/router.json
--rw-r--r--   0        0        0      721 2023-07-10 23:49:14.179642 rubi-2.1.1/network_config/polygon_mumbai/network.yaml
--rw-r--r--   0        0        0     1729 2023-07-10 23:49:41.515647 rubi-2.1.1/pyproject.toml
--rw-r--r--   0        0        0      124 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/__init__.py
--rw-r--r--   0        0        0    28087 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/client.py
--rw-r--r--   0        0        0      163 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/contracts/__init__.py
--rw-r--r--   0        0        0    61077 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/contracts/aid.py
--rw-r--r--   0        0        0    12008 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/contracts/base_contract.py
--rw-r--r--   0        0        0       74 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/contracts/contract_types/__init__.py
--rw-r--r--   0        0        0    15968 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/contracts/contract_types/events.py
--rw-r--r--   0        0        0     2708 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/contracts/contract_types/transaction_reciept.py
--rw-r--r--   0        0        0    18524 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/contracts/erc20.py
--rw-r--r--   0        0        0    24736 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/contracts/market.py
--rw-r--r--   0        0        0    14865 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/contracts/router.py
--rw-r--r--   0        0        0       77 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/data/README.md
--rw-r--r--   0        0        0       31 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/data/__init__.py
--rw-r--r--   0        0        0     9355 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/data/market.py
--rw-r--r--   0        0        0       72 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/network/__init__.py
--rw-r--r--   0        0        0     8181 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/network/network.py
--rw-r--r--   0        0        0       93 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/rubicon_types/__init__.py
--rw-r--r--   0        0        0    15639 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/rubicon_types/order.py
--rw-r--r--   0        0        0    10670 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/rubicon_types/order_query.py
--rw-r--r--   0        0        0     6411 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/rubicon_types/orderbook.py
--rw-r--r--   0        0        0     2776 2023-07-10 23:49:14.179642 rubi-2.1.1/rubi/rubicon_types/pair.py
--rw-r--r--   0        0        0     3595 1970-01-01 00:00:00.000000 rubi-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-14 15:31:41.432305 rubi-2.1.2/LICENSE
+-rw-r--r--   0        0        0     2757 2023-07-14 15:31:41.432305 rubi-2.1.2/README.md
+-rw-r--r--   0        0        0     6735 2023-07-14 15:31:41.432305 rubi-2.1.2/network_config/ERC20.json
+-rw-r--r--   0        0        0     1920 2023-07-14 15:31:41.432305 rubi-2.1.2/network_config/README.md
+-rw-r--r--   0        0        0    32732 2023-07-14 15:31:41.432305 rubi-2.1.2/network_config/abitrum_goerli/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-07-14 15:31:41.432305 rubi-2.1.2/network_config/abitrum_goerli/abis/router.json
+-rw-r--r--   0        0        0      721 2023-07-14 15:31:41.432305 rubi-2.1.2/network_config/abitrum_goerli/network.yaml
+-rw-r--r--   0        0        0    32732 2023-07-14 15:31:41.436305 rubi-2.1.2/network_config/optimism/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-07-14 15:31:41.436305 rubi-2.1.2/network_config/optimism/abis/router.json
+-rw-r--r--   0        0        0      745 2023-07-14 15:31:41.436305 rubi-2.1.2/network_config/optimism/network.yaml
+-rw-r--r--   0        0        0    32732 2023-07-14 15:31:41.436305 rubi-2.1.2/network_config/optimism_goerli/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-07-14 15:31:41.436305 rubi-2.1.2/network_config/optimism_goerli/abis/router.json
+-rw-r--r--   0        0        0      648 2023-07-14 15:31:41.436305 rubi-2.1.2/network_config/optimism_goerli/network.yaml
+-rw-r--r--   0        0        0    32732 2023-07-14 15:31:41.436305 rubi-2.1.2/network_config/polygon_mumbai/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-07-14 15:31:41.436305 rubi-2.1.2/network_config/polygon_mumbai/abis/router.json
+-rw-r--r--   0        0        0      721 2023-07-14 15:31:41.436305 rubi-2.1.2/network_config/polygon_mumbai/network.yaml
+-rw-r--r--   0        0        0     1746 2023-07-14 15:32:09.048390 rubi-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0      124 2023-07-14 15:31:41.440305 rubi-2.1.2/rubi/__init__.py
+-rw-r--r--   0        0        0    29040 2023-07-14 15:31:41.440305 rubi-2.1.2/rubi/client.py
+-rw-r--r--   0        0        0      163 2023-07-14 15:31:41.440305 rubi-2.1.2/rubi/contracts/__init__.py
+-rw-r--r--   0        0        0    65755 2023-07-14 15:31:41.440305 rubi-2.1.2/rubi/contracts/aid.py
+-rw-r--r--   0        0        0    12261 2023-07-14 15:31:41.440305 rubi-2.1.2/rubi/contracts/base_contract.py
+-rw-r--r--   0        0        0       74 2023-07-14 15:31:41.440305 rubi-2.1.2/rubi/contracts/contract_types/__init__.py
+-rw-r--r--   0        0        0    16337 2023-07-14 15:31:41.440305 rubi-2.1.2/rubi/contracts/contract_types/events.py
+-rw-r--r--   0        0        0     2805 2023-07-14 15:31:41.440305 rubi-2.1.2/rubi/contracts/contract_types/transaction_reciept.py
+-rw-r--r--   0        0        0    18565 2023-07-14 15:31:41.440305 rubi-2.1.2/rubi/contracts/erc20.py
+-rw-r--r--   0        0        0    24878 2023-07-14 15:31:41.440305 rubi-2.1.2/rubi/contracts/market.py
+-rw-r--r--   0        0        0    14915 2023-07-14 15:31:41.440305 rubi-2.1.2/rubi/contracts/router.py
+-rw-r--r--   0        0        0       77 2023-07-14 15:31:41.440305 rubi-2.1.2/rubi/data/README.md
+-rw-r--r--   0        0        0       31 2023-07-14 15:31:41.440305 rubi-2.1.2/rubi/data/__init__.py
+-rw-r--r--   0        0        0    10146 2023-07-14 15:31:41.440305 rubi-2.1.2/rubi/data/market.py
+-rw-r--r--   0        0        0       72 2023-07-14 15:31:41.440305 rubi-2.1.2/rubi/network/__init__.py
+-rw-r--r--   0        0        0     8346 2023-07-14 15:31:41.440305 rubi-2.1.2/rubi/network/network.py
+-rw-r--r--   0        0        0       94 2023-07-14 15:31:41.440305 rubi-2.1.2/rubi/rubicon_types/__init__.py
+-rw-r--r--   0        0        0    15796 2023-07-14 15:31:41.440305 rubi-2.1.2/rubi/rubicon_types/order.py
+-rw-r--r--   0        0        0    11554 2023-07-14 15:31:41.440305 rubi-2.1.2/rubi/rubicon_types/order_query.py
+-rw-r--r--   0        0        0     6323 2023-07-14 15:31:41.440305 rubi-2.1.2/rubi/rubicon_types/orderbook.py
+-rw-r--r--   0        0        0     2779 2023-07-14 15:31:41.440305 rubi-2.1.2/rubi/rubicon_types/pair.py
+-rw-r--r--   0        0        0     3635 1970-01-01 00:00:00.000000 rubi-2.1.2/PKG-INFO
```

### Comparing `rubi-2.1.1/LICENSE` & `rubi-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rubi-2.1.1/README.md` & `rubi-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.1.1/network_config/ERC20.json` & `rubi-2.1.2/network_config/ERC20.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.1/network_config/README.md` & `rubi-2.1.2/network_config/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.1.1/network_config/abitrum_goerli/abis/market.json` & `rubi-2.1.2/network_config/abitrum_goerli/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.1/network_config/abitrum_goerli/abis/router.json` & `rubi-2.1.2/network_config/abitrum_goerli/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.1/network_config/abitrum_goerli/network.yaml` & `rubi-2.1.2/network_config/abitrum_goerli/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.1.1/network_config/optimism/abis/market.json` & `rubi-2.1.2/network_config/optimism/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.1/network_config/optimism/abis/router.json` & `rubi-2.1.2/network_config/optimism/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.1/network_config/optimism/network.yaml` & `rubi-2.1.2/network_config/optimism/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.1.1/network_config/optimism_goerli/abis/market.json` & `rubi-2.1.2/network_config/optimism_goerli/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.1/network_config/optimism_goerli/abis/router.json` & `rubi-2.1.2/network_config/optimism_goerli/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.1/network_config/optimism_goerli/network.yaml` & `rubi-2.1.2/network_config/optimism_goerli/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.1.1/network_config/polygon_mumbai/abis/market.json` & `rubi-2.1.2/network_config/polygon_mumbai/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.1/network_config/polygon_mumbai/abis/router.json` & `rubi-2.1.2/network_config/polygon_mumbai/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.1/network_config/polygon_mumbai/network.yaml` & `rubi-2.1.2/network_config/polygon_mumbai/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.1.1/pyproject.toml` & `rubi-2.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rubi"
-version = "2.1.1"
+version = "2.1.2"
 description = "A python SDK for the Rubicon Protocol"
 authors = ["denver <denver@rubicon.finance>", "adam <adam@rubicon.finance>"]
 readme = "README.md"
 include = ["network_config/**/*"]
 
 
 [tool.poetry.dependencies]
@@ -17,14 +17,15 @@
 pytest = "7.3.1"
 eth-tester = "0.9.0b1"
 py-evm = "0.7.0a2"
 eth-utils = "2.1.0"
 subgrounds = { version = "1.6.0", extras = ["dash"] }
 pyyaml = "6.0.0"
 python-semantic-release = "7.34.3"
+black = "^23.3.0"
 
 [tool.poetry.group.dev.dependencies]
 python-dotenv = "0.21.1"
 ipykernel = "6.23.1"
 jupyter = "1.0.0"
 
 [tool.poetry.extras]
@@ -38,15 +39,15 @@
 test = "scripts:test"
 test_with_coverage = "scripts:test_with_coverage"
 generate_coverage_report = "scripts:test_coverage_html"
 
 [tool.semantic_release]
 version_toml = "pyproject.toml:tool.poetry.version"     # version location
 branch = "master"                                       # branch to make releases of
-changelog_file = "../CHANGELOG.md"                      # changelog file
+changelog_file = "./CHANGELOG.md"                      # changelog file
 build_command = "poetry build"                          # build dists
 dist_path = "../dist/"                                  # where to put dists
 upload_to_release = true                                # auto-create GitHub release
 upload_to_pypi = false                                  # don't auto-upload to PyPI
 remove_dist = false                                     # don't remove dists
 patch_without_tag = false                               # patch release by default -> TODO    
 version_source = "tag"
```

### Comparing `rubi-2.1.1/rubi/client.py` & `rubi-2.1.2/rubi/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from web3.types import EventData, Nonce
 
 from rubi.contracts import (
     RubiconMarket,
     RubiconRouter,
     ERC20,
     TransactionReceipt,
-    EmitFeeEvent
+    EmitFeeEvent,
 )
 from rubi.network import (
     Network,
 )
 from rubi.rubicon_types import (
     OrderSide,
     NewMarketOrder,
@@ -28,20 +28,18 @@
     PairDoesNotExistException,
     BaseEvent,
     FeeEvent,
     OrderEvent,
     Transaction,
     BaseNewOrder,
     NewCancelOrder,
-    UpdateLimitOrder
+    UpdateLimitOrder,
 )
 
-from rubi.data import (
-    MarketData
-)
+from rubi.data import MarketData
 
 
 class Client:
     """This class is a client for Rubicon. It aims to provide a simple and understandable interface when interacting
     with the Rubicon protocol. If not instantiated with a wallet and key then all the methods that require signing
     will throw an error.
 
@@ -61,26 +59,34 @@
         message_queue: Optional[Queue] = None,
         wallet: Optional[Union[ChecksumAddress, str]] = None,
         key: Optional[str] = None,
     ):
         """constructor method."""
         self.network = network
 
-        self.wallet = self.network.w3.to_checksum_address(wallet) if wallet else wallet  # type: ChecksumAddress |  None
+        self.wallet = (
+            self.network.w3.to_checksum_address(wallet) if wallet else wallet
+        )  # type: ChecksumAddress |  None
         self.key = key  # type: str |  None
 
-        self.market = RubiconMarket.from_network(network=self.network, wallet=self.wallet, key=self.key)
-        self.router = RubiconRouter.from_network(network=self.network, wallet=self.wallet, key=self.key)
+        self.market = RubiconMarket.from_network(
+            network=self.network, wallet=self.wallet, key=self.key
+        )
+        self.router = RubiconRouter.from_network(
+            network=self.network, wallet=self.wallet, key=self.key
+        )
 
         self.tokens = self.get_network_tokens()
         self._pairs: Dict[str, Pair] = {}
 
         self.message_queue = message_queue  # type: Queue | None
 
-        self.market_data = MarketData.from_network_with_tokens(network=self.network, network_tokens=self.tokens)
+        self.market_data = MarketData.from_network_with_tokens(
+            network=self.network, network_tokens=self.tokens
+        )
 
     @classmethod
     def from_http_node_url(
         cls,
         http_node_url: str,
         custom_token_addresses_file: Optional[str] = None,
         message_queue: Optional[Queue] = None,
@@ -100,32 +106,28 @@
         :param wallet: Wallet address (optional, default is None).
         :type wallet: Optional[Union[ChecksumAddress, str]]
         :param key: Key for the wallet (optional, default is None).
         :type key: str
         """
         network = Network.from_config(
             http_node_url=http_node_url,
-            custom_token_addresses_file=custom_token_addresses_file
+            custom_token_addresses_file=custom_token_addresses_file,
         )
 
-        return cls(
-            network=network,
-            message_queue=message_queue,
-            wallet=wallet,
-            key=key
-        )
+        return cls(network=network, message_queue=message_queue, wallet=wallet, key=key)
 
     ######################################################################
     # pair methods
     ######################################################################
 
     def add_pair(
-        self, pair_name: str,
+        self,
+        pair_name: str,
         base_asset_allowance: Optional[Decimal] = None,
-        quote_asset_allowance: Optional[Decimal] = None
+        quote_asset_allowance: Optional[Decimal] = None,
     ) -> None:
         """Add a Pair to the Client. This method creates a Pair instance and adds it to the Client's internal
         _pairs dictionary. Additionally, this method updates the spender allowance of the Rubicon Market for both
         base asset and the quote asset.
 
         :param pair_name: Name of the Pair in the format "<base_asset>/<quote_asset>".
         :type pair_name: str
@@ -133,60 +135,72 @@
         :type base_asset_allowance: Optional[Decimal]
         :param quote_asset_allowance: Allowance for the quote asset (optional, default is None).
         :type quote_asset_allowance: Optional[Decimal]
         """
 
         base, quote = pair_name.split("/")
 
-        base_asset = ERC20.from_network(name=base, network=self.network, wallet=self.wallet, key=self.key)
-        quote_asset = ERC20.from_network(name=quote, network=self.network, wallet=self.wallet, key=self.key)
+        base_asset = ERC20.from_network(
+            name=base, network=self.network, wallet=self.wallet, key=self.key
+        )
+        quote_asset = ERC20.from_network(
+            name=quote, network=self.network, wallet=self.wallet, key=self.key
+        )
 
         current_base_asset_allowance = None
         current_quote_asset_allowance = None
 
         if self.wallet is not None and self.key is not None:
             current_base_asset_allowance = base_asset.to_decimal(
-                number=base_asset.allowance(owner=self.wallet, spender=self.market.address)
+                number=base_asset.allowance(
+                    owner=self.wallet, spender=self.market.address
+                )
             )
             current_quote_asset_allowance = quote_asset.to_decimal(
-                number=quote_asset.allowance(owner=self.wallet, spender=self.market.address)
+                number=quote_asset.allowance(
+                    owner=self.wallet, spender=self.market.address
+                )
             )
 
-            if current_base_asset_allowance == Decimal("0") or current_quote_asset_allowance == Decimal("0"):
-                log.warning("allowance for base or quote asset is zero. this may cause issues when placing orders")
+            if current_base_asset_allowance == Decimal(
+                "0"
+            ) or current_quote_asset_allowance == Decimal("0"):
+                log.warning(
+                    "allowance for base or quote asset is zero. this may cause issues when placing orders"
+                )
 
         self._pairs[f"{base}/{quote}"] = Pair(
             name=pair_name,
             base_asset=base_asset,
             quote_asset=quote_asset,
             current_base_asset_allowance=current_base_asset_allowance,
-            current_quote_asset_allowance=current_quote_asset_allowance
+            current_quote_asset_allowance=current_quote_asset_allowance,
         )
 
         # only edit allowance if client has signing rights
         if self.wallet is not None and self.key is not None:
             self.update_pair_allowance(
                 pair_name=pair_name,
                 new_base_asset_allowance=base_asset_allowance,
-                new_quote_asset_allowance=quote_asset_allowance
+                new_quote_asset_allowance=quote_asset_allowance,
             )
 
     def get_pairs_list(self) -> List[str]:
         """Get a list of all pair names in the clients internal _pairs dictionary.
 
         :return: List of pair names.
         :rtype: List[str]
         """
         return list(self._pairs.keys())
 
     def update_pair_allowance(
         self,
         pair_name: str,
         new_base_asset_allowance: Optional[Decimal] = None,
-        new_quote_asset_allowance: Optional[Decimal] = None
+        new_quote_asset_allowance: Optional[Decimal] = None,
     ) -> None:
         """Update the allowance for the base and quote assets of a pair if the current allowance is different from the
         new allowance. This method also updates the Pair data structure so that the allowance can be read without having
         to do a call to the chain.
 
         :param pair_name: Name of the pair.
         :type pair_name: str
@@ -194,29 +208,39 @@
         :type new_base_asset_allowance: Optional[Decimal]
         :param new_quote_asset_allowance: New allowance for the quote asset. (optional, default is None).
         :type new_quote_asset_allowance: Optional[Decimal]
         :raises PairDoesNotExistException: If the pair does not exist in the clients internal _pairs dict.
         """
         pair = self.get_pair(pair_name=pair_name)
 
-        if new_base_asset_allowance is not None and pair.current_base_asset_allowance != new_base_asset_allowance:
+        if (
+            new_base_asset_allowance is not None
+            and pair.current_base_asset_allowance != new_base_asset_allowance
+        ):
             self._update_asset_allowance(
                 asset=pair.base_asset,
                 spender=self.market.address,
-                new_allowance=new_base_asset_allowance
+                new_allowance=new_base_asset_allowance,
+            )
+            pair.update_base_asset_allowance(
+                new_base_asset_allowance=new_base_asset_allowance
             )
-            pair.update_base_asset_allowance(new_base_asset_allowance=new_base_asset_allowance)
 
-        if new_quote_asset_allowance is not None and pair.current_quote_asset_allowance != new_quote_asset_allowance:
+        if (
+            new_quote_asset_allowance is not None
+            and pair.current_quote_asset_allowance != new_quote_asset_allowance
+        ):
             self._update_asset_allowance(
                 asset=pair.quote_asset,
                 spender=self.market.address,
-                new_allowance=new_quote_asset_allowance
+                new_allowance=new_quote_asset_allowance,
+            )
+            pair.update_quote_asset_allowance(
+                new_quote_asset_allowance=new_quote_asset_allowance
             )
-            pair.update_quote_asset_allowance(new_quote_asset_allowance=new_quote_asset_allowance)
 
     def get_pair(self, pair_name: str) -> Pair:
         """Retrieves the Pair object associated with the specified pair name. If the pair does not exist
         in the client, it raises a PairDoesNotExistException.
 
         :param pair_name: Name of the pair.
         :type pair_name: str
@@ -240,15 +264,15 @@
         :param pair_name: Name of the pair to remove.
         :type pair_name: str
         :raises PairDoesNotExistException: If the pair does not exist in the client before removal.
         """
         self.update_pair_allowance(
             pair_name=pair_name,
             new_base_asset_allowance=Decimal("0"),
-            new_quote_asset_allowance=Decimal("0")
+            new_quote_asset_allowance=Decimal("0"),
         )
 
         del self._pairs[pair_name]
 
     ######################################################################
     # nonce methods
     ######################################################################
@@ -273,22 +297,21 @@
         :return: The order book for the specified pair.
         :rtype: OrderBook
         :raises PairDoesNotExistException: If the pair does not exist in the client.
         """
         pair = self.get_pair(pair_name=pair_name)
 
         rubicon_offer_book = self.router.get_book_from_pair(
-            asset=pair.base_asset.address,
-            quote=pair.quote_asset.address
+            asset=pair.base_asset.address, quote=pair.quote_asset.address
         )
 
         return OrderBook.from_rubicon_offer_book(
             offer_book=rubicon_offer_book,
             base_asset=pair.base_asset,
-            quote_asset=pair.quote_asset
+            quote_asset=pair.quote_asset,
         )
 
     def start_orderbook_poller(self, pair_name: str, poll_time: int = 2) -> None:
         """Starts a background thread that continuously polls the order book for the specified pair
         at a specified polling interval. The retrieved order book is added to the message queue of the client.
         The poller will run until the pair is removed from the client.
 
@@ -297,24 +320,24 @@
         :param poll_time: Polling interval in seconds, defaults to 2 seconds.
         :type poll_time: int, optional
         :raises Exception: If the message queue is not configured.
         :raises PairDoesNotExistException: If the pair does not exist in the client.
         """
 
         if self.message_queue is None:
-            raise Exception("orderbook poller is configured to place messages on the message queue. message queue"
-                            "cannot be none")
+            raise Exception(
+                "orderbook poller is configured to place messages on the message queue. message queue"
+                "cannot be none"
+            )
 
         # Check that pair is defined before starting
         pair = self.get_pair(pair_name=pair_name)
 
         thread = Thread(
-            target=self._start_orderbook_poller,
-            args=(pair, poll_time),
-            daemon=True
+            target=self._start_orderbook_poller, args=(pair, poll_time), daemon=True
         )
         thread.start()
 
     # TODO: ideally this should use the RubiconMarket events to update itself instead of repeatedly polling the
     #  get_orderbook method. But it's fine for now.
     def _start_orderbook_poller(self, pair: Pair, poll_time: int = 2) -> None:
         """The internal implementation of the order book poller. It continuously retrieves the order book
@@ -329,15 +352,17 @@
         polling: bool = True
         while polling:
             try:
                 order_book = self.get_orderbook(pair_name=pair.name)
 
                 self.message_queue.put(order_book)
             except PairDoesNotExistException:
-                log.warning("pair does not exist in client. shutting down orderbook poller")
+                log.warning(
+                    "pair does not exist in client. shutting down orderbook poller"
+                )
                 polling = False
             except Exception as e:
                 log.error(e)
             sleep(poll_time)
 
     ######################################################################
     # event methods
@@ -345,15 +370,15 @@
 
     def start_event_poller(
         self,
         pair_name: str,
         event_type: Type[BaseEvent],
         filters: Optional[Dict[str, Any]] = None,
         event_handler: Optional[Callable] = None,
-        poll_time: int = 2
+        poll_time: int = 2,
     ) -> None:
         """Starts a background event poller that continuously listens for events of the specified event type
         related to the specified pair. The retrieved events are processed by the event handler and added to the message
         queue of the client. The poller will run until the pair is removed from the client.
 
         :param pair_name: Name of the pair to start the event poller for.
         :type pair_name: str
@@ -367,53 +392,69 @@
         :type event_handler: Optional[Callable], optional
         :param poll_time: Polling interval in seconds, defaults to 2 seconds.
         :type poll_time: int, optional
         :raises Exception: If the message queue is not configured.
         :raises PairDoesNotExistException: If the pair does not exist in the client.
         """
         if self.message_queue is None:
-            raise Exception("event poller is configured to place messages on the message queue. message queue"
-                            "cannot be none")
+            raise Exception(
+                "event poller is configured to place messages on the message queue. message queue"
+                "cannot be none"
+            )
 
         pair = self.get_pair(pair_name)
 
-        argument_filters = event_type.default_filters(
-            bid_identifier=pair.bid_identifier,
-            ask_identifier=pair.ask_identifier,
-            wallet=self.wallet
-        ) if filters is None else filters
+        argument_filters = (
+            event_type.default_filters(
+                bid_identifier=pair.bid_identifier,
+                ask_identifier=pair.ask_identifier,
+                wallet=self.wallet,
+            )
+            if filters is None
+            else filters
+        )
 
-        event_type.get_event_contract(market=self.market, router=self.router).start_event_poller(
+        event_type.get_event_contract(
+            market=self.market, router=self.router
+        ).start_event_poller(
             pair_name=pair_name,
             event_type=event_type,
             argument_filters=argument_filters,
-            event_handler=self._default_event_handler if event_handler is None else event_handler,
-            poll_time=poll_time
+            event_handler=self._default_event_handler
+            if event_handler is None
+            else event_handler,
+            poll_time=poll_time,
         )
 
-    def _default_event_handler(self, pair_name: str, event_type: Type[BaseEvent], event_data: EventData) -> None:
+    def _default_event_handler(
+        self, pair_name: str, event_type: Type[BaseEvent], event_data: EventData
+    ) -> None:
         """The default event handler function used by the event poller. It processes the retrieved events
         and adds the corresponding order events to the message queue of the client.
 
         :param pair_name: Name of the pair associated with the event.
         :type pair_name: str
         :param event_type: Type of the event.
         :type event_type: Type[BaseEvent]
         :param event_data: Data of the retrieved event.
         :type event_data: EventData
         """
-        raw_event = event_type(block_number=event_data["blockNumber"], **event_data["args"])
+        raw_event = event_type(
+            block_number=event_data["blockNumber"], **event_data["args"]
+        )
 
         if raw_event.client_filter(wallet=self.wallet):
             pair = self._pairs.get(pair_name)
 
             if isinstance(raw_event, EmitFeeEvent):
                 event = FeeEvent.from_event(pair=pair, event=raw_event)
             else:
-                event = OrderEvent.from_event(pair=pair, event=raw_event, wallet=self.wallet)
+                event = OrderEvent.from_event(
+                    pair=pair, event=raw_event, wallet=self.wallet
+                )
 
             self.message_queue.put(event)
 
     ######################################################################
     # order methods
     ######################################################################
 
@@ -437,24 +478,28 @@
 
         match order.order_side:
             case OrderSide.BUY:
                 return self.market.buy_all_amount(
                     buy_gem=pair.base_asset.address,
                     buy_amt=pair.base_asset.to_integer(order.size),
                     pay_gem=pair.quote_asset.address,
-                    max_fill_amount=pair.quote_asset.to_integer(order.worst_execution_price * order.size),
-                    **transaction.args()
+                    max_fill_amount=pair.quote_asset.to_integer(
+                        order.worst_execution_price * order.size
+                    ),
+                    **transaction.args(),
                 )
             case OrderSide.SELL:
                 return self.market.sell_all_amount(
                     pay_gem=pair.base_asset.address,
                     pay_amt=pair.base_asset.to_integer(order.size),
                     buy_gem=pair.quote_asset.address,
-                    min_fill_amount=pair.quote_asset.to_integer(order.worst_execution_price * order.size),
-                    **transaction.args()
+                    min_fill_amount=pair.quote_asset.to_integer(
+                        order.worst_execution_price * order.size
+                    ),
+                    **transaction.args(),
                 )
 
     def place_limit_order(self, transaction: Transaction) -> TransactionReceipt:
         """Place a limit order transaction by executing the specified transaction object. The transaction object should
         contain a single order of type NewLimitOrder.
 
         :param transaction: Transaction object containing the limit order.
@@ -473,23 +518,23 @@
         match order.order_side:
             case OrderSide.BUY:
                 return self.market.offer(
                     pay_amt=pair.quote_asset.to_integer(order.price * order.size),
                     pay_gem=pair.quote_asset.address,
                     buy_amt=pair.base_asset.to_integer(order.size),
                     buy_gem=pair.base_asset.address,
-                    **transaction.args()
+                    **transaction.args(),
                 )
             case OrderSide.SELL:
                 return self.market.offer(
                     pay_amt=pair.base_asset.to_integer(order.size),
                     pay_gem=pair.base_asset.address,
                     buy_amt=pair.quote_asset.to_integer(order.price * order.size),
                     buy_gem=pair.quote_asset.address,
-                    **transaction.args()
+                    **transaction.args(),
                 )
 
     def cancel_limit_order(self, transaction: Transaction) -> TransactionReceipt:
         """Place a limit order cancel transaction by executing the specified transaction object. The transaction object
         should contain a single order of type NewCancelOrder.
 
         :param transaction: Transaction object containing the cancel order.
@@ -499,18 +544,15 @@
         :raises Exception: If the transaction contains more than one order.
         """
         if len(transaction.orders) > 1:
             raise Exception("call place_order with one order only")
 
         order: NewCancelOrder = transaction.orders[0]  # noqa
 
-        return self.market.cancel(
-            id=order.order_id,
-            **transaction.args()
-        )
+        return self.market.cancel(id=order.order_id, **transaction.args())
 
     def batch_place_limit_orders(self, transaction: Transaction) -> TransactionReceipt:
         """Place multiple limit orders in a batch transaction.
 
         :param transaction: Transaction object containing multiple limit orders.
         :type transaction: Transaction
         :return: The transaction hash of the executed batch limit orders.
@@ -523,30 +565,34 @@
 
         for order in transaction.orders:
             order: NewLimitOrder
             pair = self.get_pair(order.pair)
 
             match order.order_side:
                 case OrderSide.BUY:
-                    pay_amts.append(pair.quote_asset.to_integer(order.price * order.size))
+                    pay_amts.append(
+                        pair.quote_asset.to_integer(order.price * order.size)
+                    )
                     pay_gems.append(pair.quote_asset.address)
                     buy_amts.append(pair.base_asset.to_integer(order.size))
                     buy_gems.append(pair.base_asset.address)
                 case OrderSide.SELL:
                     pay_amts.append(pair.base_asset.to_integer(order.size))
                     pay_gems.append(pair.base_asset.address)
-                    buy_amts.append(pair.quote_asset.to_integer(order.price * order.size))
+                    buy_amts.append(
+                        pair.quote_asset.to_integer(order.price * order.size)
+                    )
                     buy_gems.append(pair.quote_asset.address)
 
         return self.market.batch_offer(
             pay_amts=pay_amts,
             pay_gems=pay_gems,
             buy_amts=buy_amts,
             buy_gems=buy_gems,
-            **transaction.args()
+            **transaction.args(),
         )
 
     def batch_update_limit_orders(self, transaction: Transaction) -> TransactionReceipt:
         """Update multiple limit orders in a batch transaction.
 
         :param transaction: Transaction object containing multiple limit order updates.
         :type transaction: Transaction
@@ -563,31 +609,35 @@
             order: UpdateLimitOrder
             pair = self.get_pair(order.pair)
 
             order_ids.append(order.order_id)
 
             match order.order_side:
                 case OrderSide.BUY:
-                    pay_amts.append(pair.quote_asset.to_integer(order.price * order.size))
+                    pay_amts.append(
+                        pair.quote_asset.to_integer(order.price * order.size)
+                    )
                     pay_gems.append(pair.quote_asset.address)
                     buy_amts.append(pair.base_asset.to_integer(order.size))
                     buy_gems.append(pair.base_asset.address)
                 case OrderSide.SELL:
                     pay_amts.append(pair.base_asset.to_integer(order.size))
                     pay_gems.append(pair.base_asset.address)
-                    buy_amts.append(pair.quote_asset.to_integer(order.price * order.size))
+                    buy_amts.append(
+                        pair.quote_asset.to_integer(order.price * order.size)
+                    )
                     buy_gems.append(pair.quote_asset.address)
 
         return self.market.batch_requote(
             ids=order_ids,
             pay_amts=pay_amts,
             pay_gems=pay_gems,
             buy_amts=buy_amts,
             buy_gems=buy_gems,
-            **transaction.args()
+            **transaction.args(),
         )
 
     def batch_cancel_limit_orders(self, transaction: Transaction) -> TransactionReceipt:
         """Cancel multiple limit orders in a batch transaction.
 
         :param transaction: Transaction object containing multiple limit order cancellations.
         :type transaction: Transaction
@@ -597,77 +647,85 @@
         order_ids = []
 
         for order in transaction.orders:
             order: NewCancelOrder
 
             order_ids.append(order.order_id)
 
-        return self.market.batch_cancel(
-            ids=order_ids,
-            **transaction.args()
-        )
-    
+        return self.market.batch_cancel(ids=order_ids, **transaction.args())
+
     ######################################################################
     # data methods (raw data) TODO: once we have cleanly formatted data functions, we can switch to only exposing those
     ######################################################################
 
     def get_offers(
-        self, 
+        self,
         maker: Optional[str] = None,
         from_address: Optional[str] = None,
         pair_name: Optional[str] = None,
         book_side: Optional[OrderSide] = None,
         pay_gem: Optional[str] = None,
         buy_gem: Optional[str] = None,
         open: Optional[bool] = None,
         start_time: Optional[int] = None,
         end_time: Optional[int] = None,
         first: Optional[int] = 1000,
-        order_by: Optional[str] = 'timestamp',
-        order_direction: Optional[str] = 'desc',
-        formatted: Optional[bool] = True
+        order_by: Optional[str] = "timestamp",
+        order_direction: Optional[str] = "desc",
+        formatted: Optional[bool] = True,
     ) -> pd.DataFrame:
-        
-        df = self.market_data.get_offers(maker, from_address, pair_name, book_side, pay_gem, buy_gem, open, start_time, end_time, first, order_by, order_direction, formatted)
+        df = self.market_data.get_offers(
+            maker,
+            from_address,
+            pair_name,
+            book_side,
+            pay_gem,
+            buy_gem,
+            open,
+            start_time,
+            end_time,
+            first,
+            order_by,
+            order_direction,
+            formatted,
+        )
         return df
 
     ######################################################################
     # helper methods
     ######################################################################
 
     def get_network_tokens(
-            self, 
-    ) -> Dict[ChecksumAddress, ERC20]: 
+        self,
+    ) -> Dict[ChecksumAddress, ERC20]:
         """Returns a Dict of addresses to ERC20 objects for all tokens on the network."""
 
         network_tokens = {}
 
-        for address in self.network.token_addresses: 
-
-            try: 
-                network_tokens[address] = ERC20.from_network(name=address, network=self.network)
+        for address in self.network.token_addresses:
+            try:
+                network_tokens[address] = ERC20.from_network(
+                    name=address, network=self.network
+                )
 
             except Exception as e:
                 raise Exception(f"Token address: {address} invalid from network: {e}")
 
         return network_tokens
 
     # TODO: revisit as the safer thing is to set approval to 0 and then set approval to new_allowance
     #  or use increaseAllowance and decreaseAllowance but the current abi does not support these methods
     #  See: https://github.com/ethereum/EIPs/issues/20#issuecomment-263524729
     @staticmethod
     def _update_asset_allowance(
-        asset: ERC20,
-        spender: ChecksumAddress,
-        new_allowance: Decimal
+        asset: ERC20, spender: ChecksumAddress, new_allowance: Decimal
     ) -> None:
         log.info(
             asset.approve(
-                spender=spender,
-                amount=asset.to_integer(number=new_allowance)
+                spender=spender, amount=asset.to_integer(number=new_allowance)
             )
         )
 
     # TODO: implement this and use check transactions before they go through to prevent failure
     @staticmethod
     def _check_allowance(pair: Pair, order: BaseNewOrder):
         pass
```

### Comparing `rubi-2.1.1/rubi/contracts/aid.py` & `rubi-2.1.2/rubi/contracts/aid.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 # DEPRECATED
 # TODO: this is the old implementation for the RubiconMarketAidFactory and RubiconMarketAid. It needs to be updated in
 #  line with all the other contracts in this repo. Usage is not recommended in it's current state and it is not included
 #  in any of the __init__.py files.
 class FactoryAid:
     """this class represents the MarketAidFactory.sol contract and has read functionality for the contract
-    
+
     :param w3: Web3 instance
     :type w3: Web3
     :param contract: an optional contract instance, if not provided, the contract will be instantiated using the address and abi from the networks.py file given the chain id of the w3 instance
     :type contract: Web3 object, optional
     """
 
     def __init__(self, w3, contract=None):
@@ -30,15 +30,17 @@
 
         if contract:
             self.contract = contract
             self.address = self.contract.address
         else:
             # TODO: add error handling for unsupported chains
             network = networks[chain]()
-            self.contract = w3.eth.contract(address=network.factory, abi=network.factory_abi)
+            self.contract = w3.eth.contract(
+                address=network.factory, abi=network.factory_abi
+            )
             self.address = network.factory
 
         # set the class variables
         self.chain = chain
         self.w3 = w3
 
     ######################################################################
@@ -68,15 +70,17 @@
         :return: an array of market aid addresses
         :rtype: list
         """
 
         try:
             aids = self.contract.functions.getUserMarketAids(user).call()
         except ValueError:
-            aids = self.contract.functions.getUserMarketAids(self.w3.to_checksum_address(user)).call()
+            aids = self.contract.functions.getUserMarketAids(
+                self.w3.to_checksum_address(user)
+            ).call()
         except Exception as e:
             log.error(e, exc_info=True)
             return None
 
         return aids
 
     # rubiconMarket()
@@ -91,25 +95,26 @@
             rubicon_market = self.contract.functions.rubiconMarket().call()
         except Exception as e:
             log.error(e, exc_info=True)
             return None
 
         return rubicon_market
 
+
 class FactoryAidSigner(FactoryAid):
     """this class represents the MarketAidFactory.sol contract and has read and write functionality for the contract. this class inherits from the FactoryAid class
-    
+
     :param w3: a web3 instance
     :type w3: Web3
     :param wallet: the signers wallet address
     :type wallet: str
     :param key: the signers private key
     :type key: str
     :param contract: an optional parameter that allows you to pass in a contract instance, if none the contract will be instantiated from the rolodex.py file
-    :type contract_address: str, optional  
+    :type contract_address: str, optional
     """
 
     def __init__(self, w3, wallet, key, contract=None):
         super().__init__(w3, contract)
         self.wallet = wallet
         self.key = key
 
@@ -135,65 +140,84 @@
             txn_nonce = self.w3.eth.get_transaction_count(self.wallet)
         else:
             txn_nonce = nonce
 
         if gas_price is None:
             gas_price = self.w3.eth.gas_price
 
-        txn = {'chainId': self.chain, 'gas' : gas, 'gasPrice': gas_price, 'nonce': txn_nonce}
+        txn = {
+            "chainId": self.chain,
+            "gas": gas,
+            "gasPrice": gas_price,
+            "nonce": txn_nonce,
+        }
 
         try:
-            create = self.contract.functions.createMarketAidInstance().build_transaction(txn)
+            create = (
+                self.contract.functions.createMarketAidInstance().build_transaction(txn)
+            )
             create = self.w3.eth.account.sign_transaction(create, self.key)
             self.w3.eth.send_raw_transaction(create.rawTransaction)
 
             # if a user is not providing a nonce, wait for the transaction to either be confirmed or rejected before continuing
             if nonce is None:
-                if self.w3.eth.wait_for_transaction_receipt(create.hash)['status'] == 0:
-                    log.error(f"create_market_aid_instance transaction failed: {create.hash.hex()}")
+                if self.w3.eth.wait_for_transaction_receipt(create.hash)["status"] == 0:
+                    log.error(
+                        f"create_market_aid_instance transaction failed: {create.hash.hex()}"
+                    )
                     raise SystemExit()
 
         except Exception as e:
             log.error(e, exc_info=True)
             return None
 
         return create
 
-class MarketAid:
 
+class MarketAid:
     # init function
     # TODO: possibly allow a chain variable to be passed in
     def __init__(self, w3, address, contract=None):
         raise DeprecationWarning()
 
-        # load in the aid abi 
-        path = f"{os.path.dirname(os.path.realpath(__file__))}/helper/abis/MarketAid.json"
+        # load in the aid abi
+        path = (
+            f"{os.path.dirname(os.path.realpath(__file__))}/helper/abis/MarketAid.json"
+        )
         with open(path) as f:
             aid_abi = json.load(f)
         f.close()
 
         # create contract instance or set based upon initiliazation
         if contract:
             self.contract = contract
             self.address = self.contract.address
             chain = w3.eth.chain_id
         else:
             chain = w3.eth.chain_id
-            #network = networks[chain]()
+            # network = networks[chain]()
             self.contract = w3.eth.contract(address=address, abi=aid_abi)
             self.address = address
 
         # set the class variables
         self.chain = chain
         self.w3 = w3
-        self.log_strategist_trade_abi = self.contract.events.LogStrategistTrade()._get_event_abi()
-        self.log_scrubbed_strat_trade_abi = self.contract.events.LogScrubbedStratTrade()._get_event_abi()
-        self.log_batch_market_making_trades_abi = self.contract.events.LogBatchMarketMakingTrades()._get_event_abi()
+        self.log_strategist_trade_abi = (
+            self.contract.events.LogStrategistTrade()._get_event_abi()
+        )
+        self.log_scrubbed_strat_trade_abi = (
+            self.contract.events.LogScrubbedStratTrade()._get_event_abi()
+        )
+        self.log_batch_market_making_trades_abi = (
+            self.contract.events.LogBatchMarketMakingTrades()._get_event_abi()
+        )
         self.log_requote_abi = self.contract.events.LogRequote()._get_event_abi()
-        self.log_batch_requote_offers_abi = self.contract.events.LogBatchRequoteOffers()._get_event_abi()
+        self.log_batch_requote_offers_abi = (
+            self.contract.events.LogBatchRequoteOffers()._get_event_abi()
+        )
         self.codec: ABICodec = w3.codec
 
     ######################################################################
     # read calls
     ######################################################################
 
     # RubiconMarketAddress()
@@ -201,15 +225,17 @@
         """this function returns the address of the RubiconMarket contract
 
         :return: the address of the RubiconMarket contract
         :rtype: str
         """
 
         try:
-            rubicon_market_address = self.contract.functions.RubiconMarketAddress().call()
+            rubicon_market_address = (
+                self.contract.functions.RubiconMarketAddress().call()
+            )
         except Exception as e:
             log.error(e, exc_info=True)
             return None
 
         return rubicon_market_address
 
     # admin()
@@ -233,15 +259,17 @@
         """this function returns the list of approved strategists
 
         :return: the list of approved strategists
         :rtype: list
         """
 
         try:
-            approved_strategists = self.contract.functions.approvedStrategists(address).call()
+            approved_strategists = self.contract.functions.approvedStrategists(
+                address
+            ).call()
         except Exception as e:
             log.error(e, exc_info=True)
             return None
 
         return approved_strategists
 
     # getOutstandingStrategistTrades(asset (address), quote (address), strategist (address))
@@ -255,41 +283,61 @@
         :param strategist: the address of the strategist
         :type strategist: str
         :return: the list of outstanding trades for a strategist
         :rtype: list
         """
 
         try:
-            outstanding_strategist_trades = self.contract.functions.getOutstandingStrategistTrades(asset, quote, strategist).call()
+            outstanding_strategist_trades = (
+                self.contract.functions.getOutstandingStrategistTrades(
+                    asset, quote, strategist
+                ).call()
+            )
         except ValueError:
-            outstanding_strategist_trades = self.contract.functions.getOutstandingStrategistTrades(self.w3.to_checksum_address(asset), self.w3.to_checksum_address(quote), self.w3.to_checksum_address(strategist)).call()
+            outstanding_strategist_trades = (
+                self.contract.functions.getOutstandingStrategistTrades(
+                    self.w3.to_checksum_address(asset),
+                    self.w3.to_checksum_address(quote),
+                    self.w3.to_checksum_address(strategist),
+                ).call()
+            )
         except Exception as e:
             log.error(e, exc_info=True)
             return None
 
         return outstanding_strategist_trades
 
     # getStrategistTotalLiquidity(asset (address), quote (address), strategist (address))
     def get_strategist_total_liquidity(self, asset, quote, strategist):
-        """this function returns the total liquidity for a strategist 
+        """this function returns the total liquidity for a strategist
 
         :param asset: the address of the asset
         :type asset: str
         :param quote: the address of the quote
         :type quote: str
         :param strategist: the address of the strategist
         :type strategist: str
         :return: the total liquidity for a strategist
         :rtype: int
         """
 
         try:
-            strategist_total_liquidity = self.contract.functions.getStrategistTotalLiquidity(asset, quote, strategist).call()
+            strategist_total_liquidity = (
+                self.contract.functions.getStrategistTotalLiquidity(
+                    asset, quote, strategist
+                ).call()
+            )
         except ValueError:
-            strategist_total_liquidity = self.contract.functions.getStrategistTotalLiquidity(self.w3.to_checksum_address(asset), self.w3.to_checksum_address(quote), self.w3.to_checksum_address(strategist)).call()
+            strategist_total_liquidity = (
+                self.contract.functions.getStrategistTotalLiquidity(
+                    self.w3.to_checksum_address(asset),
+                    self.w3.to_checksum_address(quote),
+                    self.w3.to_checksum_address(strategist),
+                ).call()
+            )
         except Exception as e:
             log.error(e, exc_info=True)
             return None
 
         return strategist_total_liquidity
 
     # isApprovedStrategist(strategist (address))
@@ -299,17 +347,21 @@
         :param strategist: the address of the strategist
         :type strategist: str
         :return: whether or not a strategist is approved
         :rtype: bool
         """
 
         try:
-            is_approved_strategist = self.contract.functions.isApprovedStrategist(strategist).call()
+            is_approved_strategist = self.contract.functions.isApprovedStrategist(
+                strategist
+            ).call()
         except ValueError:
-            is_approved_strategist = self.contract.functions.isApprovedStrategist(self.w3.to_checksum_address(strategist)).call()
+            is_approved_strategist = self.contract.functions.isApprovedStrategist(
+                self.w3.to_checksum_address(strategist)
+            ).call()
         except Exception as e:
             log.error(e, exc_info=True)
             return None
 
         return is_approved_strategist
 
     def get_strategist_trade(self, trade_id):
@@ -335,367 +387,420 @@
         return strategist_trade
 
     ######################################################################
     # events & helpers
     ######################################################################
 
     # TODO: today the event signature is hardcoded, but we should be able to get it from the contract
-    # the graph does something similar to this when you run codegen, it should be a simple string manipulation problem from the abis 
+    # the graph does something similar to this when you run codegen, it should be a simple string manipulation problem from the abis
     def get_log_strategist_trade_hash(self):
-        return self.w3.keccak(text="LogStrategistTrade(uint256,bytes32,bytes32,address,address,uint256,address)").hex()
+        return self.w3.keccak(
+            text="LogStrategistTrade(uint256,bytes32,bytes32,address,address,uint256,address)"
+        ).hex()
 
-    # TODO: determine if this is the right assumtption to make about how the data is being received 
+    # TODO: determine if this is the right assumtption to make about how the data is being received
     # this assumes that the function is being used directly in the context of being passed raw data from a websocket stream that has been loaded and converted to an AttributeDict
     # TODO: i feel like this could be done much faster... tracing will tell us
     def stream_log_strategist_trade(self, data):
-
         # load the data into an attribute dictionary that web3 can use
         # data = AttributeDict(json.loads(data))
 
         # convert the topics, transaction hash, and block hash to hex strings
-        data['params']['result']['topics'] = [hexbytes.HexBytes(topic) for topic in data['params']['result']['topics']]
-        data['params']['result']['transactionHash'] = hexbytes.HexBytes(data['params']['result']['transactionHash'])
-        data['params']['result']['blockHash'] = hexbytes.HexBytes(data['params']['result']['blockHash'])
+        data["params"]["result"]["topics"] = [
+            hexbytes.HexBytes(topic) for topic in data["params"]["result"]["topics"]
+        ]
+        data["params"]["result"]["transactionHash"] = hexbytes.HexBytes(
+            data["params"]["result"]["transactionHash"]
+        )
+        data["params"]["result"]["blockHash"] = hexbytes.HexBytes(
+            data["params"]["result"]["blockHash"]
+        )
 
         # get the event data from the log
         try:
-            event = get_event_data(self.codec, self.log_strategist_trade_abi, data['params']['result'])
+            event = get_event_data(
+                self.codec, self.log_strategist_trade_abi, data["params"]["result"]
+            )
 
             # decode the offer id
             # TODO: there is probably a way to do this that does not hardcode the type of the id
-            trade_id = decode(['uint256'], event['args']['strategistTradeID'])[0]
+            trade_id = decode(["uint256"], event["args"]["strategistTradeID"])[0]
 
             # now pass an offer back in the form of a dictionary
             # TODO: this is probably not the most performant, we will optimize later
             trade = {
-                    'id': trade_id,
-                    'txn': event['transactionHash'].hex(),
-                    'event': event['event'],
-                    'ask_id': event['args']['askId'],
-                    'bid_id': event['args']['bidId'],
-                    'ask_asset': event['args']['askAsset'],
-                    'bid_asset': event['args']['bidAsset'],
-                    'timestamp': event['args']['timestamp'],
-                    'owner': event['args']['strategist']
+                "id": trade_id,
+                "txn": event["transactionHash"].hex(),
+                "event": event["event"],
+                "ask_id": event["args"]["askId"],
+                "bid_id": event["args"]["bidId"],
+                "ask_asset": event["args"]["askAsset"],
+                "bid_asset": event["args"]["bidAsset"],
+                "timestamp": event["args"]["timestamp"],
+                "owner": event["args"]["strategist"],
             }
             return trade
 
         except Exception as e:
             log.error(e, exc_info=True)
             return None
 
     def parse_log_strategist_trade(self, log):
-
         # get the event data from the log
         try:
-            event = get_event_data(self.codec, self.log_strategist_trade_abi, log['params']['result'])
+            event = get_event_data(
+                self.codec, self.log_strategist_trade_abi, log["params"]["result"]
+            )
 
             # decode the offer id
             # TODO: there is probably a way to do this that does not hardcode the type of the id
-            trade_id = decode(['uint256'], event['args']['strategistTradeID'])[0]
+            trade_id = decode(["uint256"], event["args"]["strategistTradeID"])[0]
 
             # now pass an offer back in the form of a dictionary
             # TODO: this is probably not the most performant, we will optimize later
             trade = {
-                    'id': trade_id,
-                    'txn': event['transactionHash'].hex(),
-                    'event': event['event'],
-                    'ask_id': event['args']['askId'],
-                    'bid_id': event['args']['bidId'],
-                    'ask_asset': event['args']['askAsset'],
-                    'bid_asset': event['args']['bidAsset'],
-                    'timestamp': event['args']['timestamp'],
-                    'owner': event['args']['strategist']
+                "id": trade_id,
+                "txn": event["transactionHash"].hex(),
+                "event": event["event"],
+                "ask_id": event["args"]["askId"],
+                "bid_id": event["args"]["bidId"],
+                "ask_asset": event["args"]["askAsset"],
+                "bid_asset": event["args"]["bidAsset"],
+                "timestamp": event["args"]["timestamp"],
+                "owner": event["args"]["strategist"],
             }
             return trade
 
         except Exception as e:
             log.error(e, exc_info=True)
             return None
 
-    '''
+    """
     event LogScrubbedStratTrade(
         uint256 strategistIDScrubbed,
         uint256 assetFill,
         address bathAssetAddress,
         uint256 quoteFill,
         address quoteAddress
     );
-    '''
+    """
 
     # TODO: today the event signature is hardcoded, but we should be able to get it from the contract
-    # the graph does something similar to this when you run codegen, it should be a simple string manipulation problem from the abis 
+    # the graph does something similar to this when you run codegen, it should be a simple string manipulation problem from the abis
     def get_log_scrubbed_strat_trade_hash(self):
-        return self.w3.keccak(text="LogStrategistTrade(uint256,uint256,address,uint256,address)").hex()
+        return self.w3.keccak(
+            text="LogStrategistTrade(uint256,uint256,address,uint256,address)"
+        ).hex()
 
-    # TODO: determine if this is the right assumtption to make about how the data is being received 
+    # TODO: determine if this is the right assumtption to make about how the data is being received
     # this assumes that the function is being used directly in the context of being passed raw data from a websocket stream that has been loaded and converted to an AttributeDict
     # TODO: i feel like this could be done much faster... tracing will tell us
     def stream_log_scrubbed_strat_trade(self, data):
-
         # load the data into an attribute dictionary that web3 can use
         # data = AttributeDict(json.loads(data))
 
         # convert the topics, transaction hash, and block hash to hex strings
-        data['params']['result']['topics'] = [hexbytes.HexBytes(topic) for topic in data['params']['result']['topics']]
-        data['params']['result']['transactionHash'] = hexbytes.HexBytes(data['params']['result']['transactionHash'])
-        data['params']['result']['blockHash'] = hexbytes.HexBytes(data['params']['result']['blockHash'])
+        data["params"]["result"]["topics"] = [
+            hexbytes.HexBytes(topic) for topic in data["params"]["result"]["topics"]
+        ]
+        data["params"]["result"]["transactionHash"] = hexbytes.HexBytes(
+            data["params"]["result"]["transactionHash"]
+        )
+        data["params"]["result"]["blockHash"] = hexbytes.HexBytes(
+            data["params"]["result"]["blockHash"]
+        )
 
         # get the event data from the log
         try:
-            event = get_event_data(self.codec, self.log_scrubbed_strat_trade_abi, data['params']['result'])
+            event = get_event_data(
+                self.codec, self.log_scrubbed_strat_trade_abi, data["params"]["result"]
+            )
 
             # decode the offer id
             # TODO: there is probably a way to do this that does not hardcode the type of the id
-            trade_id = decode(['uint256'], event['args']['strategistIDScrubbed'])[0]
+            trade_id = decode(["uint256"], event["args"]["strategistIDScrubbed"])[0]
 
             # now pass an offer back in the form of a dictionary
             # TODO: this is probably not the most performant, we will optimize later
             trade = {
-                    'id': trade_id,
-                    'txn': event['transactionHash'].hex(),
-                    'event': event['event'],
-                    'asset_fill': event['args']['assetFill'],
-                    'bath_asset_address': event['args']['bathAssetAddress'],
-                    'quote_fill': event['args']['quoteFill'],
-                    'quote_address': event['args']['quoteAddress']
+                "id": trade_id,
+                "txn": event["transactionHash"].hex(),
+                "event": event["event"],
+                "asset_fill": event["args"]["assetFill"],
+                "bath_asset_address": event["args"]["bathAssetAddress"],
+                "quote_fill": event["args"]["quoteFill"],
+                "quote_address": event["args"]["quoteAddress"],
             }
             return trade
 
         except Exception as e:
             log.error(e, exc_info=True)
             return None
 
     def parse_log_scrubbed_strat_trade(self, log):
-
         # get the event data from the log
         try:
-            event = get_event_data(self.codec, self.log_scrubbed_strat_trade_abi, log['params']['result'])
+            event = get_event_data(
+                self.codec, self.log_scrubbed_strat_trade_abi, log["params"]["result"]
+            )
 
             # decode the offer id
             # TODO: there is probably a way to do this that does not hardcode the type of the id
-            trade_id = decode(['uint256'], event['args']['strategistIDScrubbed'])[0]
+            trade_id = decode(["uint256"], event["args"]["strategistIDScrubbed"])[0]
 
             # now pass an offer back in the form of a dictionary
             # TODO: this is probably not the most performant, we will optimize later
             trade = {
-                    'id': trade_id,
-                    'txn': event['transactionHash'].hex(),
-                    'event': event['event'],
-                    'asset_fill': event['args']['assetFill'],
-                    'bath_asset_address': event['args']['bathAssetAddress'],
-                    'quote_fill': event['args']['quoteFill'],
-                    'quote_address': event['args']['quoteAddress']
+                "id": trade_id,
+                "txn": event["transactionHash"].hex(),
+                "event": event["event"],
+                "asset_fill": event["args"]["assetFill"],
+                "bath_asset_address": event["args"]["bathAssetAddress"],
+                "quote_fill": event["args"]["quoteFill"],
+                "quote_address": event["args"]["quoteAddress"],
             }
             return trade
 
         except Exception as e:
             log.error(e, exc_info=True)
             return None
 
-    '''
+    """
     event LogStrategistRewardClaim(
         address strategist,
         address asset,
         uint256 amountOfReward,
         uint256 timestamp
     );
-    '''
+    """
 
-    '''
+    """
     event LogBatchMarketMakingTrades(
         address strategist, 
         uint256[] trades
     );
-    '''
+    """
+
     # TODO: today the event signature is hardcoded, but we should be able to get it from the contract
-    # the graph does something similar to this when you run codegen, it should be a simple string manipulation problem from the abis 
+    # the graph does something similar to this when you run codegen, it should be a simple string manipulation problem from the abis
     def get_log_batch_market_making_trades_hash(self):
-        return self.w3.keccak(text="LogBatchMarketMakingTrades(address,uint256[])").hex()
+        return self.w3.keccak(
+            text="LogBatchMarketMakingTrades(address,uint256[])"
+        ).hex()
 
-    # TODO: determine if this is the right assumtption to make about how the data is being received 
+    # TODO: determine if this is the right assumtption to make about how the data is being received
     # this assumes that the function is being used directly in the context of being passed raw data from a websocket stream that has been loaded and converted to an AttributeDict
     # TODO: i feel like this could be done much faster... tracing will tell us
     def stream_log_batch_market_making_trades(self, data):
-
         # load the data into an attribute dictionary that web3 can use
         # data = AttributeDict(json.loads(data))
 
         # convert the topics, transaction hash, and block hash to hex strings
-        data['params']['result']['topics'] = [hexbytes.HexBytes(topic) for topic in data['params']['result']['topics']]
-        data['params']['result']['transactionHash'] = hexbytes.HexBytes(data['params']['result']['transactionHash'])
-        data['params']['result']['blockHash'] = hexbytes.HexBytes(data['params']['result']['blockHash'])
+        data["params"]["result"]["topics"] = [
+            hexbytes.HexBytes(topic) for topic in data["params"]["result"]["topics"]
+        ]
+        data["params"]["result"]["transactionHash"] = hexbytes.HexBytes(
+            data["params"]["result"]["transactionHash"]
+        )
+        data["params"]["result"]["blockHash"] = hexbytes.HexBytes(
+            data["params"]["result"]["blockHash"]
+        )
 
         # get the event data from the log
         try:
-            event = get_event_data(self.codec, self.log_batch_market_making_trades_abi, data['params']['result'])
+            event = get_event_data(
+                self.codec,
+                self.log_batch_market_making_trades_abi,
+                data["params"]["result"],
+            )
 
             # now pass an offer back in the form of a dictionary
             # TODO: this is probably not the most performant, we will optimize later
             trade = {
-                    'txn': event['transactionHash'].hex(),
-                    'event': event['event'],
-                    'strategist': event['args']['strategist'],
-                    'trades': event['args']['trades']
+                "txn": event["transactionHash"].hex(),
+                "event": event["event"],
+                "strategist": event["args"]["strategist"],
+                "trades": event["args"]["trades"],
             }
             return trade
 
         except Exception as e:
             log.error(e, exc_info=True)
             return None
 
     def parse_log_batch_market_making_trades(self, log):
-
         # get the event data from the log
         try:
-            event = get_event_data(self.codec, self.log_batch_market_making_trades_abi, log['params']['result'])
+            event = get_event_data(
+                self.codec,
+                self.log_batch_market_making_trades_abi,
+                log["params"]["result"],
+            )
 
             # now pass an offer back in the form of a dictionary
             # TODO: this is probably not the most performant, we will optimize later
             trade = {
-                    'txn': event['transactionHash'].hex(),
-                    'event': event['event'],
-                    'strategist': event['args']['strategist'],
-                    'trades': event['args']['trades']
+                "txn": event["transactionHash"].hex(),
+                "event": event["event"],
+                "strategist": event["args"]["strategist"],
+                "trades": event["args"]["trades"],
             }
             return trade
 
         except Exception as e:
             log.error(e, exc_info=True)
             return None
 
-    '''
+    """
         event LogRequote(
         address strategist,
         uint256 scrubbedOfferID,
         uint256 newOfferID
     );
-    '''
+    """
+
     # TODO: today the event signature is hardcoded, but we should be able to get it from the contract
-    # the graph does something similar to this when you run codegen, it should be a simple string manipulation problem from the abis 
+    # the graph does something similar to this when you run codegen, it should be a simple string manipulation problem from the abis
     def get_log_requote_hash(self):
         return self.w3.keccak(text="LogRequote(address,uint256,uint256)").hex()
 
-    # TODO: determine if this is the right assumtption to make about how the data is being received 
+    # TODO: determine if this is the right assumtption to make about how the data is being received
     # this assumes that the function is being used directly in the context of being passed raw data from a websocket stream that has been loaded and converted to an AttributeDict
     # TODO: i feel like this could be done much faster... tracing will tell us
     def stream_log_requote(self, data):
-
         # load the data into an attribute dictionary that web3 can use
         # data = AttributeDict(json.loads(data))
 
         # convert the topics, transaction hash, and block hash to hex strings
-        data['params']['result']['topics'] = [hexbytes.HexBytes(topic) for topic in data['params']['result']['topics']]
-        data['params']['result']['transactionHash'] = hexbytes.HexBytes(data['params']['result']['transactionHash'])
-        data['params']['result']['blockHash'] = hexbytes.HexBytes(data['params']['result']['blockHash'])
+        data["params"]["result"]["topics"] = [
+            hexbytes.HexBytes(topic) for topic in data["params"]["result"]["topics"]
+        ]
+        data["params"]["result"]["transactionHash"] = hexbytes.HexBytes(
+            data["params"]["result"]["transactionHash"]
+        )
+        data["params"]["result"]["blockHash"] = hexbytes.HexBytes(
+            data["params"]["result"]["blockHash"]
+        )
 
         # get the event data from the log
         try:
-            event = get_event_data(self.codec, self.log_requote_abi, data['params']['result'])
+            event = get_event_data(
+                self.codec, self.log_requote_abi, data["params"]["result"]
+            )
 
             # decode the offer id
             # TODO: there is probably a way to do this that does not hardcode the type of the id
-            scrub_trade_id = decode(['uint256'], event['args']['scrubbedOfferID'])[0]
-            trade_id = decode(['uint256'], event['args']['newOfferID'])[0]
+            scrub_trade_id = decode(["uint256"], event["args"]["scrubbedOfferID"])[0]
+            trade_id = decode(["uint256"], event["args"]["newOfferID"])[0]
 
             # now pass an offer back in the form of a dictionary
             # TODO: this is probably not the most performant, we will optimize later
             trade = {
-                    'id': trade_id,
-                    'txn': event['transactionHash'].hex(),
-                    'event': event['event'],
-                    'strategist': event['args']['strategist'],
-                    'scrub_trade_id': scrub_trade_id,
-                    'trade_id': trade_id
+                "id": trade_id,
+                "txn": event["transactionHash"].hex(),
+                "event": event["event"],
+                "strategist": event["args"]["strategist"],
+                "scrub_trade_id": scrub_trade_id,
+                "trade_id": trade_id,
             }
             return trade
 
         except Exception as e:
             log.error(e, exc_info=True)
             return None
 
     def parse_log_requote(self, log):
-
         # get the event data from the log
         try:
-            event = get_event_data(self.codec, self.log_requote_abi, log['params']['result'])
+            event = get_event_data(
+                self.codec, self.log_requote_abi, log["params"]["result"]
+            )
 
             # decode the offer id
             # TODO: there is probably a way to do this that does not hardcode the type of the id
-            scrub_trade_id = decode(['uint256'], event['args']['scrubbedOfferID'])[0]
-            trade_id = decode(['uint256'], event['args']['newOfferID'])[0]
+            scrub_trade_id = decode(["uint256"], event["args"]["scrubbedOfferID"])[0]
+            trade_id = decode(["uint256"], event["args"]["newOfferID"])[0]
 
             # now pass an offer back in the form of a dictionary
             # TODO: this is probably not the most performant, we will optimize later
             trade = {
-                    'id': trade_id,
-                    'txn': event['transactionHash'].hex(),
-                    'event': event['event'],
-                    'strategist': event['args']['strategist'],
-                    'scrub_trade_id': scrub_trade_id,
-                    'trade_id': trade_id
+                "id": trade_id,
+                "txn": event["transactionHash"].hex(),
+                "event": event["event"],
+                "strategist": event["args"]["strategist"],
+                "scrub_trade_id": scrub_trade_id,
+                "trade_id": trade_id,
             }
             return trade
 
         except Exception as e:
             log.error(e, exc_info=True)
             return None
 
-    '''
+    """
     event LogBatchRequoteOffers(address strategist, uint256[] scrubbedOfferIDs);
-    '''
+    """
+
     # TODO: today the event signature is hardcoded, but we should be able to get it from the contract
-    # the graph does something similar to this when you run codegen, it should be a simple string manipulation problem from the abis 
+    # the graph does something similar to this when you run codegen, it should be a simple string manipulation problem from the abis
     def get_log_batch_requote_offers_hash(self):
         return self.w3.keccak(text="LogBatchRequoteOffers(address,uint256[])").hex()
 
-    # TODO: determine if this is the right assumtption to make about how the data is being received 
+    # TODO: determine if this is the right assumtption to make about how the data is being received
     # this assumes that the function is being used directly in the context of being passed raw data from a websocket stream that has been loaded and converted to an AttributeDict
     # TODO: i feel like this could be done much faster... tracing will tell us
     def stream_log_batch_requote_offers(self, data):
-
         # load the data into an attribute dictionary that web3 can use
         # data = AttributeDict(json.loads(data))
 
         # convert the topics, transaction hash, and block hash to hex strings
-        data['params']['result']['topics'] = [hexbytes.HexBytes(topic) for topic in data['params']['result']['topics']]
-        data['params']['result']['transactionHash'] = hexbytes.HexBytes(data['params']['result']['transactionHash'])
-        data['params']['result']['blockHash'] = hexbytes.HexBytes(data['params']['result']['blockHash'])
+        data["params"]["result"]["topics"] = [
+            hexbytes.HexBytes(topic) for topic in data["params"]["result"]["topics"]
+        ]
+        data["params"]["result"]["transactionHash"] = hexbytes.HexBytes(
+            data["params"]["result"]["transactionHash"]
+        )
+        data["params"]["result"]["blockHash"] = hexbytes.HexBytes(
+            data["params"]["result"]["blockHash"]
+        )
 
         # get the event data from the log
         try:
-            event = get_event_data(self.codec, self.log_batch_requote_offers_abi, data['params']['result'])
+            event = get_event_data(
+                self.codec, self.log_batch_requote_offers_abi, data["params"]["result"]
+            )
 
             # now pass an offer back in the form of a dictionary
             # TODO: this is probably not the most performant, we will optimize later
             trade = {
-                    'txn': event['transactionHash'].hex(),
-                    'event': event['event'],
-                    'strategist': event['args']['strategist'],
-                    'scrub_trade_id': event['args']['scrubbedOfferIDs']
+                "txn": event["transactionHash"].hex(),
+                "event": event["event"],
+                "strategist": event["args"]["strategist"],
+                "scrub_trade_id": event["args"]["scrubbedOfferIDs"],
             }
             return trade
 
         except Exception as e:
             log.error(e, exc_info=True)
             return None
 
     def parse_log_batch_requote_offers(self, log):
-
         # get the event data from the log
         try:
-            event = get_event_data(self.codec, self.log_batch_requote_offers_abi, log['params']['result'])
+            event = get_event_data(
+                self.codec, self.log_batch_requote_offers_abi, log["params"]["result"]
+            )
 
             # now pass an offer back in the form of a dictionary
             # TODO: this is probably not the most performant, we will optimize later
             trade = {
-                    'txn': event['transactionHash'].hex(),
-                    'event': event['event'],
-                    'strategist': event['args']['strategist'],
-                    'scrub_trade_id': event['args']['scrubbedOfferIDs']
+                "txn": event["transactionHash"].hex(),
+                "event": event["event"],
+                "strategist": event["args"]["strategist"],
+                "scrub_trade_id": event["args"]["scrubbedOfferIDs"],
             }
             return trade
 
         except Exception as e:
             log.error(e, exc_info=True)
             return None
 
@@ -721,17 +826,19 @@
         self.key = key
 
     ######################################################################
     # write calls
     ######################################################################
 
     # adminMaxApproveTarget(target (address), token (address))
-    def admin_max_approve_target(self, target, token, nonce=None, gas=3000000, gas_price=None):
+    def admin_max_approve_target(
+        self, target, token, nonce=None, gas=3000000, gas_price=None
+    ):
         """this function sets the max approval for a target address to spend a token on behalf of the contract
-        
+
         :param target: the address of the target
         :type target: str
         :param token: the address of the token
         :type token: str
         :param nonce: nonce of the transaction, defaults to calling the chain state to get the nonce
         :type nonce: int, optional
         :param gas: gas limit of the transaction, defaults to a value of 3000000
@@ -746,49 +853,70 @@
             txn_nonce = self.w3.eth.get_transaction_count(self.wallet)
         else:
             txn_nonce = nonce
 
         if gas_price is None:
             gas_price = self.w3.eth.gas_price
 
-        txn = {'chainId': self.chain, 'gas' : gas, 'gasPrice': gas_price, 'nonce': txn_nonce}
+        txn = {
+            "chainId": self.chain,
+            "gas": gas,
+            "gasPrice": gas_price,
+            "nonce": txn_nonce,
+        }
 
         try:
-            max_approve = self.contract.functions.adminMaxApproveTarget(target, token).build_transaction(txn)
+            max_approve = self.contract.functions.adminMaxApproveTarget(
+                target, token
+            ).build_transaction(txn)
             max_approve = self.w3.eth.account.sign_transaction(max_approve, self.key)
             self.w3.eth.send_raw_transaction(max_approve.rawTransaction)
 
             # if a user is not providing a nonce, wait for the transaction to either be confirmed or rejected before continuing
             if nonce is None:
-                if self.w3.eth.wait_for_transaction_receipt(max_approve.hash)['status'] == 0:
-                    log.error(f'admin_max_approve_target transaction {max_approve.hash.hex()} failed')
+                if (
+                    self.w3.eth.wait_for_transaction_receipt(max_approve.hash)["status"]
+                    == 0
+                ):
+                    log.error(
+                        f"admin_max_approve_target transaction {max_approve.hash.hex()} failed"
+                    )
                     raise SystemExit()
 
         except ValueError:
-            log.warning('most likely a checksum error... retrying with checksummed addresses')
-            max_approve = self.contract.functions.adminMaxApproveTarget(self.w3.to_checksum_address(target), self.w3.to_checksum_address(token)).build_transaction(txn)
+            log.warning(
+                "most likely a checksum error... retrying with checksummed addresses"
+            )
+            max_approve = self.contract.functions.adminMaxApproveTarget(
+                self.w3.to_checksum_address(target), self.w3.to_checksum_address(token)
+            ).build_transaction(txn)
             max_approve = self.w3.eth.account.sign_transaction(max_approve, self.key)
             self.w3.eth.send_raw_transaction(max_approve.rawTransaction)
 
             # if a user is not providing a nonce, wait for the transaction to either be confirmed or rejected before continuing
             if nonce is None:
-                if self.w3.eth.wait_for_transaction_receipt(max_approve.hash)['status'] == 0:
-                    log.error(f'admin_max_approve_target transaction {max_approve.hash.hex()} failed')
+                if (
+                    self.w3.eth.wait_for_transaction_receipt(max_approve.hash)["status"]
+                    == 0
+                ):
+                    log.error(
+                        f"admin_max_approve_target transaction {max_approve.hash.hex()} failed"
+                    )
                     raise SystemExit()
 
         except Exception as e:
             log.error(e, exc_info=True)
             return None
 
         return max_approve
 
     # adminPullAllFunds(erc20s address[])
     def admin_pull_all_funds(self, erc20s, nonce=None, gas=3000000, gas_price=None):
         """this function pulls all funds from the contract
-        
+
         :param erc20s: a list of erc20 addresses
         :type erc20s: list
         :param nonce: nonce of the transaction, defaults to calling the chain state to get the nonce
         :type nonce: int, optional
         :param gas: gas limit of the transaction, defaults to a value of 3000000
         :type gas: int, optional
         :param gas_price: gas price of the transaction, defaults to the gas price of the chain
@@ -801,33 +929,57 @@
             txn_nonce = self.w3.eth.get_transaction_count(self.wallet)
         else:
             txn_nonce = nonce
 
         if gas_price is None:
             gas_price = self.w3.eth.gas_price
 
-        txn = {'chainId': self.chain, 'gas' : gas, 'gasPrice': gas_price, 'nonce': txn_nonce}
+        txn = {
+            "chainId": self.chain,
+            "gas": gas,
+            "gasPrice": gas_price,
+            "nonce": txn_nonce,
+        }
 
         try:
-            pull_all_funds = self.contract.functions.adminPullAllFunds(erc20s).build_transaction(txn)
-            pull_all_funds = self.w3.eth.account.sign_transaction(pull_all_funds, self.key)
+            pull_all_funds = self.contract.functions.adminPullAllFunds(
+                erc20s
+            ).build_transaction(txn)
+            pull_all_funds = self.w3.eth.account.sign_transaction(
+                pull_all_funds, self.key
+            )
             self.w3.eth.send_raw_transaction(pull_all_funds.rawTransaction)
 
             # if a user is not providing a nonce, wait for the transaction to either be confirmed or rejected before continuing
             if nonce is None:
-                if self.w3.eth.wait_for_transaction_receipt(pull_all_funds.hash)['status'] == 0:
-                    log.error(f'admin_pull_all_funds transaction {pull_all_funds.hash.hex()} failed')
+                if (
+                    self.w3.eth.wait_for_transaction_receipt(pull_all_funds.hash)[
+                        "status"
+                    ]
+                    == 0
+                ):
+                    log.error(
+                        f"admin_pull_all_funds transaction {pull_all_funds.hash.hex()} failed"
+                    )
                     raise SystemExit()
 
         except Exception as e:
             log.error(e, exc_info=True)
             return None
 
     # adminRebalanceFunds(assetToSell (address), amountToSell (uint256), assetToTarget (address))
-    def admin_rebalance_funds(self, asset_to_sell, amount_to_sell, asset_to_target, nonce=None, gas=3000000, gas_price=None):
+    def admin_rebalance_funds(
+        self,
+        asset_to_sell,
+        amount_to_sell,
+        asset_to_target,
+        nonce=None,
+        gas=3000000,
+        gas_price=None,
+    ):
         """this function rebalances funds from one asset to another on the RubiconMarket
 
         :param asset_to_sell: the address of the asset to sell
         :type asset_to_sell: str
         :param amount_to_sell: the amount of the asset to sell
         :type amount_to_sell: int
         :param asset_to_target: the address of the asset to target
@@ -846,37 +998,60 @@
             txn_nonce = self.w3.eth.get_transaction_count(self.wallet)
         else:
             txn_nonce = nonce
 
         if gas_price is None:
             gas_price = self.w3.eth.gas_price
 
-        txn = {'chainId': self.chain, 'gas' : gas, 'gasPrice': gas_price, 'nonce': txn_nonce}
+        txn = {
+            "chainId": self.chain,
+            "gas": gas,
+            "gasPrice": gas_price,
+            "nonce": txn_nonce,
+        }
 
         try:
-            rebalance = self.contract.functions.adminRebalanceFunds(asset_to_sell, amount_to_sell, asset_to_target).build_transaction(txn)
+            rebalance = self.contract.functions.adminRebalanceFunds(
+                asset_to_sell, amount_to_sell, asset_to_target
+            ).build_transaction(txn)
             rebalance = self.w3.eth.account.sign_transaction(rebalance, self.key)
             self.w3.eth.send_raw_transaction(rebalance.rawTransaction)
 
             # if a user is not providing a nonce, wait for the transaction to either be confirmed or rejected before continuing
             if nonce is None:
-                if self.w3.eth.wait_for_transaction_receipt(rebalance.hash)['status'] == 0:
-                    log.error(f'admin_rebalance_funds transaction {rebalance.hash.hex()} failed')
+                if (
+                    self.w3.eth.wait_for_transaction_receipt(rebalance.hash)["status"]
+                    == 0
+                ):
+                    log.error(
+                        f"admin_rebalance_funds transaction {rebalance.hash.hex()} failed"
+                    )
                     raise SystemExit()
 
         except ValueError:
-            log.warning('most likely a checksum error... retrying with checksummed addresses')
-            rebalance = self.contract.functions.adminRebalanceFunds(self.w3.to_checksum_address(asset_to_sell), amount_to_sell, self.w3.to_checksum_address(asset_to_target)).build_transaction(txn)
+            log.warning(
+                "most likely a checksum error... retrying with checksummed addresses"
+            )
+            rebalance = self.contract.functions.adminRebalanceFunds(
+                self.w3.to_checksum_address(asset_to_sell),
+                amount_to_sell,
+                self.w3.to_checksum_address(asset_to_target),
+            ).build_transaction(txn)
             rebalance = self.w3.eth.account.sign_transaction(rebalance, self.key)
             self.w3.eth.send_raw_transaction(rebalance.rawTransaction)
 
             # if a user is not providing a nonce, wait for the transaction to either be confirmed or rejected before continuing
             if nonce is None:
-                if self.w3.eth.wait_for_transaction_receipt(rebalance.hash)['status'] == 0:
-                    log.error(f'admin_rebalance_funds transaction {rebalance.hash.hex()} failed')
+                if (
+                    self.w3.eth.wait_for_transaction_receipt(rebalance.hash)["status"]
+                    == 0
+                ):
+                    log.error(
+                        f"admin_rebalance_funds transaction {rebalance.hash.hex()} failed"
+                    )
                     raise SystemExit()
 
         except Exception as e:
             log.error(e, exc_info=True)
             return None
 
         return rebalance
@@ -901,47 +1076,78 @@
             txn_nonce = self.w3.eth.get_transaction_count(self.wallet)
         else:
             txn_nonce = nonce
 
         if gas_price is None:
             gas_price = self.w3.eth.gas_price
 
-        txn = {'chainId': self.chain, 'gas' : gas, 'gasPrice': gas_price, 'nonce': txn_nonce}
+        txn = {
+            "chainId": self.chain,
+            "gas": gas,
+            "gasPrice": gas_price,
+            "nonce": txn_nonce,
+        }
 
         try:
-            approve = self.contract.functions.approveStrategist(strategist).build_transaction(txn)
+            approve = self.contract.functions.approveStrategist(
+                strategist
+            ).build_transaction(txn)
             approve = self.w3.eth.account.sign_transaction(approve, self.key)
             self.w3.eth.send_raw_transaction(approve.rawTransaction)
 
             # if a user is not providing a nonce, wait for the transaction to either be confirmed or rejected before continuing
             if nonce is None:
-                if self.w3.eth.wait_for_transaction_receipt(approve.hash)['status'] == 0:
-                    log.error(f'approve_strategist transaction {approve.hash.hex()} failed')
+                if (
+                    self.w3.eth.wait_for_transaction_receipt(approve.hash)["status"]
+                    == 0
+                ):
+                    log.error(
+                        f"approve_strategist transaction {approve.hash.hex()} failed"
+                    )
                     raise SystemExit()
 
         except ValueError:
-            log.warning('most likely a checksum error... retrying with checksummed addresses')
-            approve = self.contract.functions.approveStrategist(self.w3.to_checksum_address(strategist)).build_transaction(txn)
+            log.warning(
+                "most likely a checksum error... retrying with checksummed addresses"
+            )
+            approve = self.contract.functions.approveStrategist(
+                self.w3.to_checksum_address(strategist)
+            ).build_transaction(txn)
             approve = self.w3.eth.account.sign_transaction(approve, self.key)
             self.w3.eth.send_raw_transaction(approve.rawTransaction)
 
             # if a user is not providing a nonce, wait for the transaction to either be confirmed or rejected before continuing
             if nonce is None:
-                if self.w3.eth.wait_for_transaction_receipt(approve.hash)['status'] == 0:
-                    log.error(f'approve_strategist transaction {approve.hash.hex()} failed')
+                if (
+                    self.w3.eth.wait_for_transaction_receipt(approve.hash)["status"]
+                    == 0
+                ):
+                    log.error(
+                        f"approve_strategist transaction {approve.hash.hex()} failed"
+                    )
                     raise SystemExit()
 
         except Exception as e:
             log.error(e, exc_info=True)
             return None
 
         return approve
 
     # batchMarketMakingTrades(tokenPairs (address[2]), askNumerators (uint256[]), askDenominators (uint256[]), bidNumerators (uint256[]), bidDenominators (uint256[]))
-    def batch_market_making_trades(self, token_pairs, ask_numerators, ask_denominators, bid_numerators, bid_denominators, nonce=None, gas=3000000, gas_price=None):
+    def batch_market_making_trades(
+        self,
+        token_pairs,
+        ask_numerators,
+        ask_denominators,
+        bid_numerators,
+        bid_denominators,
+        nonce=None,
+        gas=3000000,
+        gas_price=None,
+    ):
         """this function executes a batch of market making trades on the RubiconMarket
 
         :param token_pairs: the token pairs to trade [token0, token1]
         :type token_pairs: list
         :param ask_numerators: the numerators of the ask prices
         :type ask_numerators: list
         :param ask_denominators: the denominators of the ask prices
@@ -964,35 +1170,58 @@
             txn_nonce = self.w3.eth.get_transaction_count(self.wallet)
         else:
             txn_nonce = nonce
 
         if gas_price is None:
             gas_price = self.w3.eth.gas_price
 
-        txn = {'chainId': self.chain, 'gas' : gas, 'gasPrice': gas_price, 'nonce': txn_nonce}
+        txn = {
+            "chainId": self.chain,
+            "gas": gas,
+            "gasPrice": gas_price,
+            "nonce": txn_nonce,
+        }
 
         try:
-            batch = self.contract.functions.batchMarketMakingTrades(token_pairs, ask_numerators, ask_denominators, bid_numerators, bid_denominators).build_transaction(txn)
+            batch = self.contract.functions.batchMarketMakingTrades(
+                token_pairs,
+                ask_numerators,
+                ask_denominators,
+                bid_numerators,
+                bid_denominators,
+            ).build_transaction(txn)
             batch = self.w3.eth.account.sign_transaction(batch, self.key)
             self.w3.eth.send_raw_transaction(batch.rawTransaction)
 
             # if a user is not providing a nonce, wait for the transaction to either be confirmed or rejected before continuing
             if nonce is None:
-                if self.w3.eth.wait_for_transaction_receipt(batch.hash)['status'] == 0:
-                    log.error(f'batch_market_making_trades transaction {batch.hash.hex()} failed')
+                if self.w3.eth.wait_for_transaction_receipt(batch.hash)["status"] == 0:
+                    log.error(
+                        f"batch_market_making_trades transaction {batch.hash.hex()} failed"
+                    )
                     raise SystemExit()
 
         except Exception as e:
             log.error(e, exc_info=True)
             return None
 
         return batch
 
     # batchRequoteAllOffers(tokenPair (address[2]), askNumerators (uint256[]), askDenominators (uint256[]), bidNumerators (uint256[]), bidDenominators (uint256[]))
-    def batch_requote_all_offers(self, token_pair, ask_numerators, ask_denominators, bid_numerators, bid_denominators, nonce=None, gas=3000000, gas_price=None):
+    def batch_requote_all_offers(
+        self,
+        token_pair,
+        ask_numerators,
+        ask_denominators,
+        bid_numerators,
+        bid_denominators,
+        nonce=None,
+        gas=3000000,
+        gas_price=None,
+    ):
         """this function executes a batch requote while clearing all offers the strategist has on the RubiconMarket
 
         :param token_pair: the token pair to trade [token0, token1]
         :type token_pair: list
         :param ask_numerators: the numerators of the ask prices
         :type ask_numerators: list
         :param ask_denominators: the denominators of the ask prices
@@ -1015,37 +1244,61 @@
             txn_nonce = self.w3.eth.get_transaction_count(self.wallet)
         else:
             txn_nonce = nonce
 
         if gas_price is None:
             gas_price = self.w3.eth.gas_price
 
-        txn = {'chainId': self.chain, 'gas' : gas, 'gasPrice': gas_price, 'nonce': txn_nonce}
+        txn = {
+            "chainId": self.chain,
+            "gas": gas,
+            "gasPrice": gas_price,
+            "nonce": txn_nonce,
+        }
 
         try:
-            batch = self.contract.functions.batchRequoteAllOffers(token_pair, ask_numerators, ask_denominators, bid_numerators, bid_denominators).build_transaction(txn)
+            batch = self.contract.functions.batchRequoteAllOffers(
+                token_pair,
+                ask_numerators,
+                ask_denominators,
+                bid_numerators,
+                bid_denominators,
+            ).build_transaction(txn)
             batch = self.w3.eth.account.sign_transaction(batch, self.key)
             self.w3.eth.send_raw_transaction(batch.rawTransaction)
 
             # if a user is not providing a nonce, wait for the transaction to either be confirmed or rejected before continuing
             if nonce is None:
-                if self.w3.eth.wait_for_transaction_receipt(batch.hash)['status'] == 0:
-                    log.error(f'batch_requote_all_offers transaction {batch.hash.hex()} failed')
+                if self.w3.eth.wait_for_transaction_receipt(batch.hash)["status"] == 0:
+                    log.error(
+                        f"batch_requote_all_offers transaction {batch.hash.hex()} failed"
+                    )
                     raise SystemExit()
 
         except Exception as e:
             log.error(e, exc_info=True)
             return None
 
         return batch
 
     # batchRequoteOffers(ids (uint256[]), tokenPair (address[2]), askNumerators (uint256[]), askDenominators (uint256[]), bidNumerators (uint256[]), bidDenominators (uint256[]))
-    def batch_requote_offers(self, ids, token_pair, ask_numerators, ask_denominators, bid_numerators, bid_denominators, nonce=None, gas=3000000, gas_price=None):
+    def batch_requote_offers(
+        self,
+        ids,
+        token_pair,
+        ask_numerators,
+        ask_denominators,
+        bid_numerators,
+        bid_denominators,
+        nonce=None,
+        gas=3000000,
+        gas_price=None,
+    ):
         """this function executes a batch requote of all offers that are provided in the ids array
-        
+
         :param ids: the ids of the offers to requote
         :type ids: list
         :param token_pair: the token pair to trade [token0, token1]
         :type token_pair: list
         :param ask_numerators: the numerators of the ask prices
         :type ask_numerators: list
         :param ask_denominators: the denominators of the ask prices
@@ -1068,38 +1321,62 @@
             txn_nonce = self.w3.eth.get_transaction_count(self.wallet)
         else:
             txn_nonce = nonce
 
         if gas_price is None:
             gas_price = self.w3.eth.gas_price
 
-        txn = {'chainId': self.chain, 'gas' : gas, 'gasPrice': gas_price, 'nonce': txn_nonce}
-
-        try:
-            batch = self.contract.functions.batchRequoteOffers(ids, token_pair, ask_numerators, ask_denominators, bid_numerators, bid_denominators).build_transaction(txn)
+        txn = {
+            "chainId": self.chain,
+            "gas": gas,
+            "gasPrice": gas_price,
+            "nonce": txn_nonce,
+        }
+
+        try:
+            batch = self.contract.functions.batchRequoteOffers(
+                ids,
+                token_pair,
+                ask_numerators,
+                ask_denominators,
+                bid_numerators,
+                bid_denominators,
+            ).build_transaction(txn)
             batch = self.w3.eth.account.sign_transaction(batch, self.key)
             self.w3.eth.send_raw_transaction(batch.rawTransaction)
 
             # if a user is not providing a nonce, wait for the transaction to either be confirmed or rejected before continuing
             if nonce is None:
-                if self.w3.eth.wait_for_transaction_receipt(batch.hash)['status'] == 0:
-                    log.error(f'batch_requote_offers transaction {batch.hash.hex()} failed')
+                if self.w3.eth.wait_for_transaction_receipt(batch.hash)["status"] == 0:
+                    log.error(
+                        f"batch_requote_offers transaction {batch.hash.hex()} failed"
+                    )
                     raise SystemExit()
 
         except Exception as e:
             log.error(e, exc_info=True)
             return None
 
         return batch
 
     # placeMarketMakingTrades(tokenPair (address[2]), askNumerator (uint256), askDenominator (uint256), bidNumerator (uint256), bidDenominator (uint256))
     # aid.batch_market_making_trades([weth.address, usdc.address], [the amount of the asset you will sell], [the amount of the quote you will receive], [the amount of quote you will pay], [the amount of asset you would receive])
-    def place_market_making_trades(self, token_pair, ask_numerator, ask_denominator, bid_numerator, bid_denominator, nonce=None, gas=3000000, gas_price=None):
+    def place_market_making_trades(
+        self,
+        token_pair,
+        ask_numerator,
+        ask_denominator,
+        bid_numerator,
+        bid_denominator,
+        nonce=None,
+        gas=3000000,
+        gas_price=None,
+    ):
         """this function executes a market making trade on the RubiconMarket
-        
+
         :param token_pair: the token pair to trade [token0, token1]
         :type token_pair: list
         :param ask_numerator: the numerator of the ask price. this is the amount of the asset you will sell
         :type ask_numerator: int
         :param ask_denominator: the denominator of the ask price. this is the amount of the quote you will receive
         :type ask_denominator: int
         :param bid_numerator: the numerator of the bid price. this is the amount of quote you will pay
@@ -1120,37 +1397,50 @@
             txn_nonce = self.w3.eth.get_transaction_count(self.wallet)
         else:
             txn_nonce = nonce
 
         if gas_price is None:
             gas_price = self.w3.eth.gas_price
 
-        txn = {'chainId': self.chain, 'gas' : gas, 'gasPrice': gas_price, 'nonce': txn_nonce}
+        txn = {
+            "chainId": self.chain,
+            "gas": gas,
+            "gasPrice": gas_price,
+            "nonce": txn_nonce,
+        }
 
         try:
-            trade = self.contract.functions.placeMarketMakingTrades(token_pair, ask_numerator, ask_denominator, bid_numerator, bid_denominator).build_transaction(txn)
+            trade = self.contract.functions.placeMarketMakingTrades(
+                token_pair,
+                ask_numerator,
+                ask_denominator,
+                bid_numerator,
+                bid_denominator,
+            ).build_transaction(txn)
             trade = self.w3.eth.account.sign_transaction(trade, self.key)
             self.w3.eth.send_raw_transaction(trade.rawTransaction)
 
             # if a user is not providing a nonce, wait for the transaction to either be confirmed or rejected before continuing
             if nonce is None:
-                if self.w3.eth.wait_for_transaction_receipt(trade.hash)['status'] == 0:
-                    log.error(f'place_market_making_trades transaction {trade.hash.hex()} failed')
+                if self.w3.eth.wait_for_transaction_receipt(trade.hash)["status"] == 0:
+                    log.error(
+                        f"place_market_making_trades transaction {trade.hash.hex()} failed"
+                    )
                     raise SystemExit()
 
         except Exception as e:
             log.error(e, exc_info=True)
             return None
 
         return trade
 
     # removeStrategist(strategist (address))
     def remove_strategist(self, strategist, nonce=None, gas=3000000, gas_price=None):
         """this function removes a strategist from the approved strategist list on the market aid contract
-        
+
         :param strategist: the address of the strategist to remove
         :type strategist: str
         :param nonce: nonce of the transaction, defaults to calling the chain state to get the nonce
         :type nonce: int, optional
         :param gas: gas limit of the transaction, defaults to a value of 3000000
         :type gas: int, optional
         :param gas_price: gas price of the transaction, defaults to the gas price of the chain
@@ -1163,49 +1453,75 @@
             txn_nonce = self.w3.eth.get_transaction_count(self.wallet)
         else:
             txn_nonce = nonce
 
         if gas_price is None:
             gas_price = self.w3.eth.gas_price
 
-        txn = {'chainId': self.chain, 'gas' : gas, 'gasPrice': gas_price, 'nonce': txn_nonce}
+        txn = {
+            "chainId": self.chain,
+            "gas": gas,
+            "gasPrice": gas_price,
+            "nonce": txn_nonce,
+        }
 
         try:
-            remove = self.contract.functions.removeStrategist(strategist).build_transaction(txn)
+            remove = self.contract.functions.removeStrategist(
+                strategist
+            ).build_transaction(txn)
             remove = self.w3.eth.account.sign_transaction(remove, self.key)
             self.w3.eth.send_raw_transaction(remove.rawTransaction)
 
             # if a user is not providing a nonce, wait for the transaction to either be confirmed or rejected before continuing
             if nonce is None:
-                if self.w3.eth.wait_for_transaction_receipt(remove.hash)['status'] == 0:
-                    log.error(f'remove_strategist transaction {remove.hash.hex()} failed')
+                if self.w3.eth.wait_for_transaction_receipt(remove.hash)["status"] == 0:
+                    log.error(
+                        f"remove_strategist transaction {remove.hash.hex()} failed"
+                    )
                     raise SystemExit()
 
         except ValueError:
-            log.warning('most likely a checksum error... retrying with checksummed addresses')
-            remove = self.contract.functions.removeStrategist(self.w3.to_checksum_address(strategist)).build_transaction(txn)
+            log.warning(
+                "most likely a checksum error... retrying with checksummed addresses"
+            )
+            remove = self.contract.functions.removeStrategist(
+                self.w3.to_checksum_address(strategist)
+            ).build_transaction(txn)
             remove = self.w3.eth.account.sign_transaction(remove, self.key)
             self.w3.eth.send_raw_transaction(remove.rawTransaction)
 
             # if a user is not providing a nonce, wait for the transaction to either be confirmed or rejected before continuing
             if nonce is None:
-                if self.w3.eth.wait_for_transaction_receipt(remove.hash)['status'] == 0:
-                    log.error(f'remove_strategist transaction {remove.hash.hex()} failed')
+                if self.w3.eth.wait_for_transaction_receipt(remove.hash)["status"] == 0:
+                    log.error(
+                        f"remove_strategist transaction {remove.hash.hex()} failed"
+                    )
                     raise SystemExit()
 
         except Exception as e:
             log.error(e, exc_info=True)
             return None
 
         return remove
 
     # requote(id (uint256), tokenPair (address[2]), askNumerator (uint256), askDenominator (uint256), bidNumerator (uint256), bidDenominator (uint256))
-    def requote(self, id, token_pair, ask_numerator, ask_denominator, bid_numerator, bid_denominator, nonce=None, gas=3000000, gas_price=None):
+    def requote(
+        self,
+        id,
+        token_pair,
+        ask_numerator,
+        ask_denominator,
+        bid_numerator,
+        bid_denominator,
+        nonce=None,
+        gas=3000000,
+        gas_price=None,
+    ):
         """this function requotes an offer on the RubiconMarket
-        
+
         :param id: the id of the offer to requote
         :type id: int
         :param token_pair: the token pair to trade [token0, token1]
         :type token_pair: list
         :param ask_numerator: the numerator of the ask price
         :type ask_numerator: int
         :param ask_denominator: the denominator of the ask price
@@ -1228,25 +1544,40 @@
             txn_nonce = self.w3.eth.get_transaction_count(self.wallet)
         else:
             txn_nonce = nonce
 
         if gas_price is None:
             gas_price = self.w3.eth.gas_price
 
-        txn = {'chainId': self.chain, 'gas' : gas, 'gasPrice': gas_price, 'nonce': txn_nonce}
-
-        try:
-            requote = self.contract.functions.requote(id, token_pair, ask_numerator, ask_denominator, bid_numerator, bid_denominator).build_transaction(txn)
+        txn = {
+            "chainId": self.chain,
+            "gas": gas,
+            "gasPrice": gas_price,
+            "nonce": txn_nonce,
+        }
+
+        try:
+            requote = self.contract.functions.requote(
+                id,
+                token_pair,
+                ask_numerator,
+                ask_denominator,
+                bid_numerator,
+                bid_denominator,
+            ).build_transaction(txn)
             requote = self.w3.eth.account.sign_transaction(requote, self.key)
             self.w3.eth.send_raw_transaction(requote.rawTransaction)
 
             # if a user is not providing a nonce, wait for the transaction to either be confirmed or rejected before continuing
             if nonce is None:
-                if self.w3.eth.wait_for_transaction_receipt(requote.hash)['status'] == 0:
-                    log.error(f'requote transaction {requote.hash.hex()} failed')
+                if (
+                    self.w3.eth.wait_for_transaction_receipt(requote.hash)["status"]
+                    == 0
+                ):
+                    log.error(f"requote transaction {requote.hash.hex()} failed")
                     raise SystemExit()
 
         except Exception as e:
             log.error(e, exc_info=True)
             return None
 
         return requote
@@ -1269,25 +1600,34 @@
             txn_nonce = self.w3.eth.get_transaction_count(self.wallet)
         else:
             txn_nonce = nonce
 
         if gas_price is None:
             gas_price = self.w3.eth.gas_price
 
-        txn = {'chainId': self.chain, 'gas' : gas, 'gasPrice': gas_price, 'nonce': txn_nonce}
+        txn = {
+            "chainId": self.chain,
+            "gas": gas,
+            "gasPrice": gas_price,
+            "nonce": txn_nonce,
+        }
 
         try:
-            scrub = self.contract.functions.scrubStrategistTrade(id).build_transaction(txn)
+            scrub = self.contract.functions.scrubStrategistTrade(id).build_transaction(
+                txn
+            )
             scrub = self.w3.eth.account.sign_transaction(scrub, self.key)
             self.w3.eth.send_raw_transaction(scrub.rawTransaction)
 
             # if a user is not providing a nonce, wait for the transaction to either be confirmed or rejected before continuing
             if nonce is None:
-                if self.w3.eth.wait_for_transaction_receipt(scrub.hash)['status'] == 0:
-                    log.error(f'scrub_strategist_trade transaction {scrub.hash.hex()} failed')
+                if self.w3.eth.wait_for_transaction_receipt(scrub.hash)["status"] == 0:
+                    log.error(
+                        f"scrub_strategist_trade transaction {scrub.hash.hex()} failed"
+                    )
                     raise SystemExit()
 
         except Exception as e:
             log.error(e, exc_info=True)
             return None
 
         return scrub
@@ -1312,25 +1652,34 @@
             txn_nonce = self.w3.eth.get_transaction_count(self.wallet)
         else:
             txn_nonce = nonce
 
         if gas_price is None:
             gas_price = self.w3.eth.gas_price
 
-        txn = {'chainId': self.chain, 'gas' : gas, 'gasPrice': gas_price, 'nonce': txn_nonce}
+        txn = {
+            "chainId": self.chain,
+            "gas": gas,
+            "gasPrice": gas_price,
+            "nonce": txn_nonce,
+        }
 
         try:
-            scrub = self.contract.functions.scrubStrategistTrades(ids).build_transaction(txn)
+            scrub = self.contract.functions.scrubStrategistTrades(
+                ids
+            ).build_transaction(txn)
             scrub = self.w3.eth.account.sign_transaction(scrub, self.key)
             self.w3.eth.send_raw_transaction(scrub.rawTransaction)
 
             # if a user is not providing a nonce, wait for the transaction to either be confirmed or rejected before continuing
             if nonce is None:
-                if self.w3.eth.wait_for_transaction_receipt(scrub.hash)['status'] == 0:
-                    log.error(f'scrub_strategist_trades transaction {scrub.hash.hex()} failed')
+                if self.w3.eth.wait_for_transaction_receipt(scrub.hash)["status"] == 0:
+                    log.error(
+                        f"scrub_strategist_trades transaction {scrub.hash.hex()} failed"
+                    )
                     raise SystemExit()
 
         except Exception as e:
             log.error(e, exc_info=True)
             return None
 
-        return scrub
+        return scrub
```

### Comparing `rubi-2.1.1/rubi/contracts/base_contract.py` & `rubi-2.1.2/rubi/contracts/base_contract.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,27 +30,29 @@
     """
 
     def __init__(
         self,
         w3: Web3,
         contract: Contract,
         wallet: Optional[ChecksumAddress] = None,
-        key: Optional[str] = None
+        key: Optional[str] = None,
     ):
         """constructor method"""
         if (wallet is None) != (key is None):
-            raise Exception("both a wallet and a key are required to sign transactions. provide both or omit both")
+            raise Exception(
+                "both a wallet and a key are required to sign transactions. provide both or omit both"
+            )
 
         self.contract = contract
         self.address = contract.address
         self.w3 = w3
         self.chain_id = self.w3.eth.chain_id
 
         # Signing permissions
-        self.signing_permissions = (wallet is not None and key is not None)
+        self.signing_permissions = wallet is not None and key is not None
 
         if self.signing_permissions:
             log.info(f"instantiated {self.__class__} with signing rights")
 
             # Force typing as my editors inspection is throwing a tantrum
             self.wallet = wallet  # type: ChecksumAddress
             self.key = key  # type: str
@@ -58,15 +60,15 @@
     @classmethod
     def from_address_and_abi(
         cls,
         w3: Web3,
         address: ChecksumAddress,
         contract_abi: ABI,
         wallet: Optional[ChecksumAddress] = None,
-        key: Optional[str] = None
+        key: Optional[str] = None,
     ) -> "BaseContract":
         """Create a BaseContract instance from the contract address and ABI.
 
         :param w3: The Web3 instance.
         :type w3: Web3
         :param address: The address of the contract.
         :type address: ChecksumAddress
@@ -97,15 +99,15 @@
     #  spam the node that is being connected to
     def start_event_poller(
         self,
         pair_name: str,
         event_type: Type[BaseEvent],
         argument_filters: Optional[Dict[str, Any]] = None,
         event_handler: Optional[Callable] = None,
-        poll_time: int = 2
+        poll_time: int = 2,
     ) -> None:
         """Start a thread which runs an event poller for a specific event type.
 
         :param pair_name: The name of the pair we are monitoring events of.
         :type pair_name: str
         :param event_type: The type of event to poll for.
         :type event_type: Type[BaseEvent]
@@ -113,33 +115,45 @@
         :type argument_filters: Optional[Dict[str, Any]]
         :param event_handler: Optional event handler function. Defaults to using the events default handler.
         :type event_handler: Optional[Callable]
         :param poll_time: The time interval between each poll in seconds. Defaults to 2 seconds.
         :type poll_time: int
         """
 
-        event_filter = event_type.create_event_filter(contract=self.contract, argument_filters=argument_filters)
-        handler = event_handler if event_handler is not None else event_type.default_handler
+        event_filter = event_type.create_event_filter(
+            contract=self.contract, argument_filters=argument_filters
+        )
+        handler = (
+            event_handler if event_handler is not None else event_type.default_handler
+        )
 
         thread = Thread(
             target=self._start_default_event_poller,
-            args=(pair_name, event_type, self.contract, argument_filters, event_filter, handler, poll_time),
-            daemon=True
+            args=(
+                pair_name,
+                event_type,
+                self.contract,
+                argument_filters,
+                event_filter,
+                handler,
+                poll_time,
+            ),
+            daemon=True,
         )
         thread.start()
 
     @staticmethod
     def _start_default_event_poller(
         pair_name: str,
         event_type: Type[BaseEvent],
         contract: Contract,
         argument_filters: Optional[Dict[str, Any]],
         event_filter: LogFilter,
         event_handler: Callable,
-        poll_time: int
+        poll_time: int,
     ) -> None:
         """Start the default event poller loop. This thread will stop if the pair is removed from the client.
 
         :param pair_name: The name of the event pair.
         :type pair_name: str
         :param event_type: The type of the event.
         :type event_type: Type[BaseEvent]
@@ -157,15 +171,17 @@
                 for event_data in event_filter.get_new_entries():
                     event_handler(pair_name, event_type, event_data)
             except Exception as e:
                 log.error(e)
 
                 # The filter has been deleted by the node and needs to be recreated
                 if "filter not found" in str(e):
-                    event_filter = event_type.create_event_filter(contract=contract, argument_filters=argument_filters)
+                    event_filter = event_type.create_event_filter(
+                        contract=contract, argument_filters=argument_filters
+                    )
                     log.info(f"event filter for: {event_type} has been recreated")
 
                 # TODO: this is a hack to detect if a PairDoesNotExistException is raised and polling should stop.
                 #  Currently an additional except PairDoesNotExistException as e: cannot be added as this causes a
                 #  circular import. Think about restructuring the directories to avoid this (e.g one root level types
                 #  directory).
                 if "add pair to the client" in str(e):
@@ -202,44 +218,43 @@
         :param max_priority_fee_per_gas: Optional maximum priority fee per gas for the transaction.
             (optional, default is None).
         :type max_priority_fee_per_gas: Optional[int]
         :return: An object representing the transaction receipt
         :rtype: TransactionReceipt
         """
         if not self.signing_permissions:
-            raise Exception(f"cannot write transaction without signing rights. "
-                            f"re-instantiate {self.__class__} with a wallet and private key")
+            raise Exception(
+                f"cannot write transaction without signing rights. "
+                f"re-instantiate {self.__class__} with a wallet and private key"
+            )
 
         base_txn = self._transaction_params(
             gas=gas,
             nonce=nonce,
             max_fee_per_gas=max_fee_per_gas,
-            max_priority_fee_per_gas=max_priority_fee_per_gas
+            max_priority_fee_per_gas=max_priority_fee_per_gas,
         )
 
-        txn = instantiated_contract_function.build_transaction(
-            transaction=base_txn
-        )
+        txn = instantiated_contract_function.build_transaction(transaction=base_txn)
 
         signed_txn = self.w3.eth.account.sign_transaction(
-            transaction_dict=txn,
-            private_key=self.key
+            transaction_dict=txn, private_key=self.key
         )
 
         log.debug(f"SENDING TRANSACTION, nonce: {nonce}, timestamp: {time.time_ns()}")
         self.w3.eth.send_raw_transaction(signed_txn.rawTransaction)
 
         return self._wait_for_transaction_receipt(transaction=signed_txn)
 
     def _transaction_params(
         self,
         nonce: Optional[Nonce],
         gas: Optional[int],
         max_fee_per_gas: Optional[int],
-        max_priority_fee_per_gas: Optional[int]
+        max_priority_fee_per_gas: Optional[int],
     ) -> Dict:
         """Build transaction parameters Dict for a transaction. If a key is associated with a None value after building
         the Dict then this key will be removed before returning the dict.
 
         :param nonce: Optional nonce value for the transaction (optional, default is None).
         :type nonce: Optional[Nonce]
         :param gas: gas limit for the transaction. If None is passed then w3.eth.estimate_gas is used.
@@ -253,25 +268,27 @@
         :rtype: Dict
         """
 
         if nonce is None:
             nonce = self.w3.eth.get_transaction_count(self.wallet)
 
         transaction = {
-            'chainId': self.chain_id,
-            'gas': gas,
-            'maxFeePerGas': max_fee_per_gas,
-            'maxPriorityFeePerGas': max_priority_fee_per_gas,
-            'nonce': nonce,
-            'from': self.wallet
+            "chainId": self.chain_id,
+            "gas": gas,
+            "maxFeePerGas": max_fee_per_gas,
+            "maxPriorityFeePerGas": max_priority_fee_per_gas,
+            "nonce": nonce,
+            "from": self.wallet,
         }
 
         return {key: value for key, value in transaction.items() if value is not None}
 
-    def _wait_for_transaction_receipt(self, transaction: SignedTransaction) -> TransactionReceipt:
+    def _wait_for_transaction_receipt(
+        self, transaction: SignedTransaction
+    ) -> TransactionReceipt:
         """Wait for the transaction receipt and check if the transaction was successful.
 
         :param transaction: The signed transaction object.
         :type transaction: SignedTransaction
         """
 
         result = TransactionReceipt.from_tx_receipt(
```

### Comparing `rubi-2.1.1/rubi/contracts/contract_types/events.py` & `rubi-2.1.2/rubi/contracts/contract_types/events.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,73 +10,80 @@
 
 # To solve for circular dependencies
 _RubiconMarket = TypeVar("_RubiconMarket")
 _RubiconRouter = TypeVar("_RubiconRouter")
 
 
 class BaseEvent(ABC):
-    """Base class for events to define the structure of an Event from a Rubicon contract.
-    """
+    """Base class for events to define the structure of an Event from a Rubicon contract."""
 
     def __init__(self, block_number: int, **args):
         """Initialize a BaseEvent instance.
 
         :param block_number: The block number of the event.
         :type block_number: int
         :param args: Additional arguments for the event.
         :type args: dict
         """
         self.block_number = block_number
 
     @staticmethod
     @abstractmethod
-    def get_event_contract(market: _RubiconMarket, router: _RubiconRouter) -> Union[_RubiconMarket, _RubiconRouter]:
+    def get_event_contract(
+        market: _RubiconMarket, router: _RubiconRouter
+    ) -> Union[_RubiconMarket, _RubiconRouter]:
         """Abstract method to determine the contract an event corresponds to. Must be overridden in subclasses.
 
         :param market: The RubiconMarket instance.
         :type market: _RubiconMarket
         :param router: The RubiconRouter instance.
         :type router: _RubiconRouter
         :return: The contract corresponding to the event.
         :rtype: Union[_RubiconMarket, _RubiconRouter]
         """
         raise NotImplementedError()
 
     @staticmethod
     @abstractmethod
-    def create_event_filter(contract: Contract, argument_filters: Optional[Dict[str, Any]] = None) -> LogFilter:
+    def create_event_filter(
+        contract: Contract, argument_filters: Optional[Dict[str, Any]] = None
+    ) -> LogFilter:
         """Abstract method to create an event filter for the given contract with optional argument filters. Must be
         overridden in each event subclass.
 
         :param contract: The contract instance.
         :type contract: Contract
         :param argument_filters: Optional filters. Only events that match these filters will be returned when the filter
             is queried.
         :type argument_filters: Optional[Dict[str, Any]]
         :return: The created event filter.
         :rtype: LogFilter
         """
         raise NotImplementedError()
 
     @classmethod
-    def default_handler(cls, pair_name: str, event_type: Type["BaseEvent"], event_data: EventData) -> None:
+    def default_handler(
+        cls, pair_name: str, event_type: Type["BaseEvent"], event_data: EventData
+    ) -> None:
         """A default event handler. If no handler is provided then this one is used.
 
         :param pair_name: The name of the pair.
         :type pair_name: str
         :param event_type: The type of the event.
         :type event_type: Type["BaseEvent"]
         :param event_data: The data of the event.
         :type event_data: EventData
         """
         log.info(event_data)
 
     @staticmethod
     @abstractmethod
-    def default_filters(bid_identifier: str, ask_identifier: str, wallet: ChecksumAddress) -> dict:
+    def default_filters(
+        bid_identifier: str, ask_identifier: str, wallet: ChecksumAddress
+    ) -> dict:
         """Get the default filters for an event. These are used if no argument filters are provided. By default, these
         filters make sure we only receive events that relate to us. E.g on markets we care about.
 
         :param bid_identifier: The identifier for bid events.
         :type bid_identifier: str
         :param ask_identifier: The identifier for ask events.
         :type ask_identifier: str
@@ -104,14 +111,15 @@
         return "{}({})".format(type(self).__name__, ", ".join(items))
 
 
 ######################################################################
 # market events
 ######################################################################
 
+
 class BaseMarketEvent(BaseEvent, ABC):
     """This class is a base class for all MarketEvents"""
 
     def __init__(self, id: bytes, pair: bytes, **args):
         """Initialize a BaseMarketEvent instance.
 
         :param id: The event ID.
@@ -122,70 +130,76 @@
         :type args: dict
         """
         super().__init__(**args)
         self.id = int(id.hex(), 16)
         self.pair = add_0x_prefix(HexStr(pair.hex()))
 
     @staticmethod
-    def get_event_contract(market: _RubiconMarket, router: _RubiconRouter) -> Union[_RubiconMarket, _RubiconRouter]:
+    def get_event_contract(
+        market: _RubiconMarket, router: _RubiconRouter
+    ) -> Union[_RubiconMarket, _RubiconRouter]:
         """implementation of BaseEvent get_event_contract"""
         return market
 
 
 class EmitOfferEvent(BaseMarketEvent):
-    """Event emitted whenever a new offer is made on the RubiconMarket
-    """
+    """Event emitted whenever a new offer is made on the RubiconMarket"""
 
     def __init__(
         self,
         maker: ChecksumAddress,
         pay_gem: ChecksumAddress,
         buy_gem: ChecksumAddress,
         pay_amt: int,
         buy_amt: int,
         **args
     ):
         """Initialize an EmitOfferEvent instance.
 
-       :param maker: The maker address.
-       :type maker: ChecksumAddress
-       :param pay_gem: The address of the token to be paid.
-       :type pay_gem: ChecksumAddress
-       :param buy_gem: The address of the token to be bought.
-       :type buy_gem: ChecksumAddress
-       :param pay_amt: The amount to be paid.
-       :type pay_amt: int
-       :param buy_amt: The amount to be bought.
-       :type buy_amt: int
-       :param args: Additional arguments for the event.
-       :type args: dict
-       """
+        :param maker: The maker address.
+        :type maker: ChecksumAddress
+        :param pay_gem: The address of the token to be paid.
+        :type pay_gem: ChecksumAddress
+        :param buy_gem: The address of the token to be bought.
+        :type buy_gem: ChecksumAddress
+        :param pay_amt: The amount to be paid.
+        :type pay_amt: int
+        :param buy_amt: The amount to be bought.
+        :type buy_amt: int
+        :param args: Additional arguments for the event.
+        :type args: dict
+        """
         super().__init__(**args)
         self.maker = maker
         self.pay_gem = pay_gem
         self.buy_gem = buy_gem
         self.pay_amt = pay_amt
         self.buy_amt = buy_amt
 
     @staticmethod
-    def create_event_filter(contract: Contract, argument_filters: Optional[Dict[str, Any]] = None) -> LogFilter:
+    def create_event_filter(
+        contract: Contract, argument_filters: Optional[Dict[str, Any]] = None
+    ) -> LogFilter:
         """implementation of BaseEvent create_event_filter"""
-        return contract.events.emitOffer.create_filter(argument_filters=argument_filters, fromBlock="latest")
+        return contract.events.emitOffer.create_filter(
+            argument_filters=argument_filters, fromBlock="latest"
+        )
 
     @staticmethod
-    def default_filters(bid_identifier: str, ask_identifier: str, wallet: ChecksumAddress) -> dict:
+    def default_filters(
+        bid_identifier: str, ask_identifier: str, wallet: ChecksumAddress
+    ) -> dict:
         """implementation of BaseEvent default_filters"""
         filters = {"pair": [bid_identifier, ask_identifier], "maker": wallet}
 
         return {key: value for key, value in filters.items() if value is not None}
 
 
 class EmitTakeEvent(BaseMarketEvent):
-    """Event emitted whenever an offer is taken by a market order on the RubiconMarket
-    """
+    """Event emitted whenever an offer is taken by a market order on the RubiconMarket"""
 
     def __init__(
         self,
         maker: ChecksumAddress,
         taker: ChecksumAddress,
         pay_gem: ChecksumAddress,
         buy_gem: ChecksumAddress,
@@ -216,33 +230,38 @@
         self.taker = taker
         self.pay_gem = pay_gem
         self.buy_gem = buy_gem
         self.take_amt = take_amt
         self.give_amt = give_amt
 
     @staticmethod
-    def create_event_filter(contract: Contract, argument_filters: Optional[Dict[str, Any]] = None) -> LogFilter:
+    def create_event_filter(
+        contract: Contract, argument_filters: Optional[Dict[str, Any]] = None
+    ) -> LogFilter:
         """implementation of BaseEvent create_event_filter"""
-        return contract.events.emitTake.create_filter(argument_filters=argument_filters, fromBlock="latest")
+        return contract.events.emitTake.create_filter(
+            argument_filters=argument_filters, fromBlock="latest"
+        )
 
     @staticmethod
-    def default_filters(bid_identifier: HexStr, ask_identifier: HexStr, wallet: ChecksumAddress) -> dict:
+    def default_filters(
+        bid_identifier: HexStr, ask_identifier: HexStr, wallet: ChecksumAddress
+    ) -> dict:
         """implementation of BaseEvent default_filters"""
         filters = {"pair": [bid_identifier, ask_identifier]}
 
         return {key: value for key, value in filters.items() if value is not None}
 
     def client_filter(self, wallet: ChecksumAddress) -> bool:
         """overwriting of BaseEvent client_filter to only filter when our wallet is either the maker or taker"""
         return wallet is None or (self.maker == wallet or self.taker == wallet)
 
 
 class EmitCancelEvent(BaseMarketEvent):
-    """Event emitted whenever an offer is cancelled on the RubiconMarket
-    """
+    """Event emitted whenever an offer is cancelled on the RubiconMarket"""
 
     def __init__(
         self,
         maker: ChecksumAddress,
         pay_gem: ChecksumAddress,
         buy_gem: ChecksumAddress,
         pay_amt: int,
@@ -269,29 +288,34 @@
         self.maker = maker
         self.pay_gem = pay_gem
         self.buy_gem = buy_gem
         self.pay_amt = pay_amt
         self.buy_amt = buy_amt
 
     @staticmethod
-    def create_event_filter(contract: Contract, argument_filters: Optional[Dict[str, Any]] = None) -> LogFilter:
+    def create_event_filter(
+        contract: Contract, argument_filters: Optional[Dict[str, Any]] = None
+    ) -> LogFilter:
         """implementation of BaseEvent create_event_filter"""
-        return contract.events.emitCancel.create_filter(argument_filters=argument_filters, fromBlock="latest")
+        return contract.events.emitCancel.create_filter(
+            argument_filters=argument_filters, fromBlock="latest"
+        )
 
     @staticmethod
-    def default_filters(bid_identifier: str, ask_identifier: str, wallet: ChecksumAddress) -> dict:
+    def default_filters(
+        bid_identifier: str, ask_identifier: str, wallet: ChecksumAddress
+    ) -> dict:
         """implementation of BaseEvent default_filters"""
         filters = {"pair": [bid_identifier, ask_identifier], "maker": wallet}
 
         return {key: value for key, value in filters.items() if value is not None}
 
 
 class EmitFeeEvent(BaseMarketEvent):
-    """Event emitted whenever an offer is taken on the RubiconMarket that results in a fee being paid to the maker.
-    """
+    """Event emitted whenever an offer is taken on the RubiconMarket that results in a fee being paid to the maker."""
 
     def __init__(
         self,
         taker: ChecksumAddress,
         feeTo: ChecksumAddress,
         asset: ChecksumAddress,
         feeAmt: int,
@@ -314,20 +338,26 @@
 
         self.taker = taker
         self.fee_to = feeTo
         self.asset = asset
         self.fee_amt = feeAmt
 
     @staticmethod
-    def create_event_filter(contract: Contract, argument_filters: Optional[Dict[str, Any]] = None) -> LogFilter:
+    def create_event_filter(
+        contract: Contract, argument_filters: Optional[Dict[str, Any]] = None
+    ) -> LogFilter:
         """implementation of BaseEvent create_event_filter"""
-        return contract.events.emitFee.create_filter(argument_filters=argument_filters, fromBlock="latest")
+        return contract.events.emitFee.create_filter(
+            argument_filters=argument_filters, fromBlock="latest"
+        )
 
     @staticmethod
-    def default_filters(bid_identifier: str, ask_identifier: str, wallet: ChecksumAddress) -> dict:
+    def default_filters(
+        bid_identifier: str, ask_identifier: str, wallet: ChecksumAddress
+    ) -> dict:
         """implementation of BaseEvent default_filters"""
         filters = {"feeTo": wallet}
 
         return {key: value for key, value in filters.items() if value is not None}
 
 
 class EmitDeleteEvent(BaseMarketEvent):
@@ -344,33 +374,39 @@
         :type args: dict
         """
         super().__init__(**args)
 
         self.maker = maker
 
     @staticmethod
-    def create_event_filter(contract: Contract, argument_filters: Optional[Dict[str, Any]] = None) -> LogFilter:
+    def create_event_filter(
+        contract: Contract, argument_filters: Optional[Dict[str, Any]] = None
+    ) -> LogFilter:
         """implementation of BaseEvent create_event_filter"""
-        return contract.events.emitDelete.create_filter(argument_filters=argument_filters, fromBlock="latest")
+        return contract.events.emitDelete.create_filter(
+            argument_filters=argument_filters, fromBlock="latest"
+        )
 
     @staticmethod
-    def default_filters(bid_identifier: str, ask_identifier: str, wallet: ChecksumAddress) -> dict:
+    def default_filters(
+        bid_identifier: str, ask_identifier: str, wallet: ChecksumAddress
+    ) -> dict:
         """implementation of BaseEvent default_filters"""
         filters = {"pair": [bid_identifier, ask_identifier], "maker": wallet}
 
         return {key: value for key, value in filters.items() if value is not None}
 
 
 ######################################################################
 # router events
 ######################################################################
 
+
 class EmitSwap(BaseEvent):
-    """Event emitted whenever swap is executed on the RubiconRouter
-    """
+    """Event emitted whenever swap is executed on the RubiconRouter"""
 
     def __init__(
         self,
         recipient: ChecksumAddress,
         inputERC20: ChecksumAddress,
         targetERC20: ChecksumAddress,
         pair: bytes,
@@ -405,22 +441,30 @@
         self.targetERC20 = targetERC20
         self.pair = pair
         self.inputAmount = inputAmount
         self.realizedFill = realizedFill
         self.hurdleBuyAmtMin = hurdleBuyAmtMin
 
     @staticmethod
-    def get_event_contract(market: _RubiconMarket, router: _RubiconRouter) -> Union[_RubiconMarket, _RubiconRouter]:
+    def get_event_contract(
+        market: _RubiconMarket, router: _RubiconRouter
+    ) -> Union[_RubiconMarket, _RubiconRouter]:
         """implementation of BaseEvent get_event_contract"""
         return router
 
     @staticmethod
-    def create_event_filter(contract: Contract, argument_filters: Optional[Dict[str, Any]] = None) -> LogFilter:
+    def create_event_filter(
+        contract: Contract, argument_filters: Optional[Dict[str, Any]] = None
+    ) -> LogFilter:
         """implementation of BaseEvent create_event_filter"""
-        return contract.events.emitSwap.create_filter(argument_filters=argument_filters, fromBlock="latest")
+        return contract.events.emitSwap.create_filter(
+            argument_filters=argument_filters, fromBlock="latest"
+        )
 
     @staticmethod
-    def default_filters(bid_identifier: str, ask_identifier: str, wallet: ChecksumAddress) -> dict:
+    def default_filters(
+        bid_identifier: str, ask_identifier: str, wallet: ChecksumAddress
+    ) -> dict:
         """implementation of BaseEvent default_filters"""
         filters = {"recipient": wallet}
 
         return {key: value for key, value in filters.items() if value is not None}
```

### Comparing `rubi-2.1.1/rubi/contracts/contract_types/transaction_reciept.py` & `rubi-2.1.2/rubi/contracts/contract_types/transaction_reciept.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         to_address: ChecksumAddress,
         status: int,
         transaction_hash: HexBytes,
         transaction_index: int,
         l1_fee: Optional[int] = None,
         l1_gas_price: Optional[int] = None,
         l1_gas_used: Optional[int] = None,
-        l1_fee_scalar: Optional[Decimal] = None
+        l1_fee_scalar: Optional[Decimal] = None,
     ):
         self.block_number = block_number
         self.contract_address = contract_address
         self.effective_gas_price = effective_gas_price
         self.gas_used = gas_used
         self.from_address = from_address
         self.to_address = to_address
@@ -37,27 +37,34 @@
         self.l1_fee = l1_fee
         self.l1_gas_price = l1_gas_price
         self.l1_gas_used = l1_gas_used
         self.l1_fee_scalar = l1_fee_scalar
 
     @classmethod
     def from_tx_receipt(cls, tx_receipt: TxReceipt) -> "TransactionReceipt":
-
         return cls(
             block_number=tx_receipt["blockNumber"],
             contract_address=tx_receipt["contractAddress"],
             effective_gas_price=tx_receipt["effectiveGasPrice"],
             gas_used=tx_receipt["gasUsed"],
             from_address=tx_receipt["from"],
             to_address=tx_receipt["to"],
             status=tx_receipt["status"],
             transaction_hash=tx_receipt["transactionHash"],
             transaction_index=tx_receipt["transactionIndex"],
-            l1_fee=None if tx_receipt.get("l1Fee") is None else int(tx_receipt.get("l1Fee"), 16),
-            l1_gas_price=None if tx_receipt.get("l1GasPrice") is None else int(tx_receipt.get("l1GasPrice"), 16),
-            l1_gas_used=None if tx_receipt.get("l1GasUsed") is None else int(tx_receipt.get("l1GasUsed"), 16),
-            l1_fee_scalar=None if tx_receipt.get("l1FeeScalar") is None else Decimal(tx_receipt.get("l1FeeScalar"))
+            l1_fee=None
+            if tx_receipt.get("l1Fee") is None
+            else int(tx_receipt.get("l1Fee"), 16),
+            l1_gas_price=None
+            if tx_receipt.get("l1GasPrice") is None
+            else int(tx_receipt.get("l1GasPrice"), 16),
+            l1_gas_used=None
+            if tx_receipt.get("l1GasUsed") is None
+            else int(tx_receipt.get("l1GasUsed"), 16),
+            l1_fee_scalar=None
+            if tx_receipt.get("l1FeeScalar") is None
+            else Decimal(tx_receipt.get("l1FeeScalar")),
         )
 
     def __repr__(self):
         items = ("{}={!r}".format(k, self.__dict__[k]) for k in self.__dict__)
         return "{}({})".format(type(self).__name__, ", ".join(items))
```

### Comparing `rubi-2.1.1/rubi/contracts/erc20.py` & `rubi-2.1.2/rubi/contracts/erc20.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,35 +28,30 @@
     """
 
     def __init__(
         self,
         w3: Web3,
         contract: Contract,
         wallet: Optional[ChecksumAddress] = None,
-        key: Optional[str] = None
+        key: Optional[str] = None,
     ):
         """constructor method"""
-        super().__init__(
-            w3=w3,
-            contract=contract,
-            wallet=wallet,
-            key=key
-        )
+        super().__init__(w3=w3, contract=contract, wallet=wallet, key=key)
 
         self.name: str = self.name()
         self.symbol: str = self.symbol()
         self.decimal: int = self.decimals()
 
     @classmethod
     def from_network(
         cls,
         name: str,
         network: Network,
         wallet: Optional[ChecksumAddress] = None,
-        key: Optional[str] = None
+        key: Optional[str] = None,
     ) -> "ERC20":
         """Create an ERC20 instance based on a Network instance and token name.
 
         :param name: The name of the token.
         :type name: str
         :param network: A Network instance.
         :type network: Network
@@ -67,45 +62,49 @@
         :return: An ERC20 instance based on the Network instance and token name.
         :rtype: ERC20
         :raises Exception: If the token name does not exist in the network configuration.
         :raises Exception: If the ERC20.json ABI file is not found in the network_config folder.
         """
 
         if network.token_addresses[name] is None:
-            raise Exception(f"{name} in not a valid token according to the network config.")
+            raise Exception(
+                f"{name} in not a valid token according to the network config."
+            )
 
         abi: ABI
 
         try:
             path = f"{os.path.dirname(os.path.abspath(__file__))}/../../network_config/ERC20.json"
 
             with open(path) as f:
                 abi = json.load(f)
 
         except FileNotFoundError:
-            raise Exception("ERC20.json abi not found. this file should in the network_config folder")
+            raise Exception(
+                "ERC20.json abi not found. this file should in the network_config folder"
+            )
 
         return cls.from_address_and_abi(
             w3=network.w3,
             address=network.token_addresses[name],
             contract_abi=abi,
             wallet=wallet,
-            key=key
+            key=key,
         )
-    
+
     @classmethod
     def from_address(
         cls,
         w3: Web3,
         address: ChecksumAddress,
         wallet: Optional[ChecksumAddress] = None,
-        key: Optional[str] = None
+        key: Optional[str] = None,
     ) -> "ERC20":
         """Create an ERC20 instance based on an address and a network connection.
-        
+
         :param w3: Web3 instance.
         :type w3: Web3
         :param address: The address of the contract.
         :type address: ChecksumAddress
         :param wallet: Optional wallet address to use for interacting with the contract (optional, default is None).
         :type wallet: Optional[ChecksumAddress]
         :param key: Optional private key for the wallet (optional, default is None).
@@ -119,25 +118,22 @@
         try:
             path = f"{os.path.dirname(os.path.abspath(__file__))}/../../network_config/ERC20.json"
 
             with open(path) as f:
                 abi = json.load(f)
 
         except FileNotFoundError:
-            raise Exception("ERC20.json abi not found. this file should in the network_config folder")
-        
+            raise Exception(
+                "ERC20.json abi not found. this file should in the network_config folder"
+            )
+
         return cls.from_address_and_abi(
-            w3=w3,
-            address=address,
-            contract_abi=abi,
-            wallet=wallet,
-            key=key
+            w3=w3, address=address, contract_abi=abi, wallet=wallet, key=key
         )
 
-
     ######################################################################
     # read calls
     ######################################################################
 
     # allowance(owner (address), spender (address)) -> uint256
     def allowance(self, owner: ChecksumAddress, spender: ChecksumAddress) -> int:
         """Reads the allowance of the spender from the owner for the erc20 contract
@@ -214,15 +210,15 @@
     def approve(
         self,
         spender: ChecksumAddress,
         amount: int,
         nonce: Optional[int] = None,
         gas: Optional[int] = None,
         max_fee_per_gas: Optional[int] = None,
-        max_priority_fee_per_gas: Optional[int] = None
+        max_priority_fee_per_gas: Optional[int] = None,
     ) -> TransactionReceipt:
         """Approves the spender to spend the amount of the erc20 token from the signer's wallet
 
         :param spender: address of the spender
         :type spender: ChecksumAddress
         :param amount: amount of the erc20 token to approve the spender to spend
         :type amount: int
@@ -243,26 +239,26 @@
         approve = self.contract.functions.approve(spender, amount)
 
         return self._default_transaction_handler(
             instantiated_contract_function=approve,
             gas=gas,
             nonce=nonce,
             max_fee_per_gas=max_fee_per_gas,
-            max_priority_fee_per_gas=max_priority_fee_per_gas
+            max_priority_fee_per_gas=max_priority_fee_per_gas,
         )
 
     # transfer(recipient (address), amount (uint256)) -> bool
     def transfer(
         self,
         recipient: ChecksumAddress,
         amount: int,
         nonce: Optional[int] = None,
         gas: Optional[int] = None,
         max_fee_per_gas: Optional[int] = None,
-        max_priority_fee_per_gas: Optional[int] = None
+        max_priority_fee_per_gas: Optional[int] = None,
     ) -> TransactionReceipt:
         """Transfers the amount of the erc20 token to the recipient
 
         :param recipient: address of the recipient
         :type recipient: ChecksumAddress
         :param amount: amount of the erc20 token to transfer
         :type amount: int
@@ -282,27 +278,27 @@
         transfer = self.contract.functions.transfer(recipient, amount)
 
         return self._default_transaction_handler(
             instantiated_contract_function=transfer,
             gas=gas,
             nonce=nonce,
             max_fee_per_gas=max_fee_per_gas,
-            max_priority_fee_per_gas=max_priority_fee_per_gas
+            max_priority_fee_per_gas=max_priority_fee_per_gas,
         )
 
     # transferFrom(sender (address), recipient (address), amount (uint256)) -> bool
     def transfer_from(
         self,
         sender: ChecksumAddress,
         recipient: ChecksumAddress,
         amount: int,
         nonce: Optional[int] = None,
         gas: Optional[int] = None,
         max_fee_per_gas: Optional[int] = None,
-        max_priority_fee_per_gas: Optional[int] = None
+        max_priority_fee_per_gas: Optional[int] = None,
     ) -> TransactionReceipt:
         """Transfers the amount of the erc20 token from the sender to the recipient
 
         :param sender: address of the sender
         :type sender: ChecksumAddress
         :param recipient: address of the recipient
         :type recipient: ChecksumAddress
@@ -326,26 +322,26 @@
         transfer_from = self.contract.functions.transferFrom(sender, recipient, amount)
 
         return self._default_transaction_handler(
             instantiated_contract_function=transfer_from,
             gas=gas,
             nonce=nonce,
             max_fee_per_gas=max_fee_per_gas,
-            max_priority_fee_per_gas=max_priority_fee_per_gas
+            max_priority_fee_per_gas=max_priority_fee_per_gas,
         )
 
     # increaseAllowance(spender (address), addedValue (uint256)) -> bool
     def increase_allowance(
         self,
         spender: ChecksumAddress,
         added_value: int,
         nonce: Optional[int] = None,
         gas: Optional[int] = None,
         max_fee_per_gas: Optional[int] = None,
-        max_priority_fee_per_gas: Optional[int] = None
+        max_priority_fee_per_gas: Optional[int] = None,
     ) -> TransactionReceipt:
         """Increases the allowance of the spender by the added_value
 
         :param spender: address of the spender
         :type spender: ChecksumAddress
         :param added_value: amount to increase the allowance by, in the integer representation of the erc20 token
         :type added_value: int
@@ -359,33 +355,35 @@
         :type max_fee_per_gas: Optional[int]
         :param max_priority_fee_per_gas: max priority fee that can be paid for gas, defaults to calling the chain to
             estimate the max_priority_fee_per_gas (optional, default is None)
         :type max_priority_fee_per_gas: Optional[int]
         :return: An object representing the transaction receipt
         :rtype: TransactionReceipt
         """
-        increase_allowance = self.contract.functions.increaseAllowance(spender, added_value)
+        increase_allowance = self.contract.functions.increaseAllowance(
+            spender, added_value
+        )
 
         return self._default_transaction_handler(
             instantiated_contract_function=increase_allowance,
             gas=gas,
             nonce=nonce,
             max_fee_per_gas=max_fee_per_gas,
-            max_priority_fee_per_gas=max_priority_fee_per_gas
+            max_priority_fee_per_gas=max_priority_fee_per_gas,
         )
 
     # decreaseAllowance(spender (address), subtractedValue (uint256)) -> bool
     def decrease_allowance(
         self,
         spender: ChecksumAddress,
         subtracted_value: int,
         nonce: Optional[int] = None,
         gas: Optional[int] = None,
         max_fee_per_gas: Optional[int] = None,
-        max_priority_fee_per_gas: Optional[int] = None
+        max_priority_fee_per_gas: Optional[int] = None,
     ) -> TransactionReceipt:
         """Decreases the allowance of the spender by the subtracted_value
 
         :param spender: address of the spender
         :type spender: ChecksumAddress
         :param subtracted_value: amount to decrease the allowance by, in the integer representation of the erc20 token
         :type subtracted_value: int
@@ -399,22 +397,24 @@
         :type max_fee_per_gas: Optional[int]
         :param max_priority_fee_per_gas: max priority fee that can be paid for gas, defaults to calling the chain to
             estimate the max_priority_fee_per_gas (optional, default is None)
         :type max_priority_fee_per_gas: Optional[int]
         :return: An object representing the transaction receipt
         :rtype: TransactionReceipt
         """
-        decrease_allowance = self.contract.functions.decreaseAllowance(spender, subtracted_value)
+        decrease_allowance = self.contract.functions.decreaseAllowance(
+            spender, subtracted_value
+        )
 
         return self._default_transaction_handler(
             instantiated_contract_function=decrease_allowance,
             gas=gas,
             nonce=nonce,
             max_fee_per_gas=max_fee_per_gas,
-            max_priority_fee_per_gas=max_priority_fee_per_gas
+            max_priority_fee_per_gas=max_priority_fee_per_gas,
         )
 
     ######################################################################
     # helper methods
     ######################################################################
 
     def to_decimal(self, number: int) -> Decimal:
@@ -426,34 +426,36 @@
         :return: the Decimal representation of the token
         :rtype: Decimal
         """
 
         if number == 0:
             return Decimal("0")
         else:
-            return Decimal(number) / Decimal(10 ** self.decimal)
+            return Decimal(number) / Decimal(10**self.decimal)
 
     def to_integer(self, number: Decimal) -> int:
         """Converts a Decimal representation of the token to an integer representation of the token by multiplying the
         float by 10 to the power of the number of decimals of the token
 
         :param number: the Decimal representation of the token
         :type number: Decimal
         :return: the integer representation of the token
         :rtype: int
         """
 
         if number == Decimal("0"):
             return 0
         else:
-            return int(number * (10 ** self.decimal))
+            return int(number * (10**self.decimal))
 
     def max_approval_amount(self) -> Decimal:
         """return the max uint256 token approval amount. Note: this is not very secure and if you give this approval you
         should revoke it when you are done!
 
         :return: the max approval amount of a uint256 token in Decimal representation
         :rtype: Decimal
         """
-        max_uint256 = "0xffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff"
+        max_uint256 = (
+            "0xffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff"
+        )
 
         return self.to_decimal(number=int(max_uint256, base=16))
```

### Comparing `rubi-2.1.1/rubi/contracts/market.py` & `rubi-2.1.2/rubi/contracts/market.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,30 +24,25 @@
     """
 
     def __init__(
         self,
         w3: Web3,
         contract: Contract,
         wallet: Optional[ChecksumAddress] = None,
-        key: Optional[str] = None
+        key: Optional[str] = None,
     ) -> None:
         """constructor method"""
-        super().__init__(
-            w3=w3,
-            contract=contract,
-            wallet=wallet,
-            key=key
-        )
+        super().__init__(w3=w3, contract=contract, wallet=wallet, key=key)
 
     @classmethod
     def from_network(
         cls,
         network: Network,
         wallet: Optional[ChecksumAddress] = None,
-        key: Optional[str] = None
+        key: Optional[str] = None,
     ) -> "RubiconMarket":
         """Create a RubiconMarket instance based on a Network instance.
 
         :param network: A Network instance.
         :type network: Network
         :param wallet: Optional wallet address to use for interacting with the contract (optional, default is None).
         :type wallet: Optional[ChecksumAddress]
@@ -57,15 +52,15 @@
         :rtype: RubiconMarket
         """
         return cls.from_address_and_abi(
             w3=network.w3,
             address=network.rubicon.market.address,
             contract_abi=network.rubicon.market.abi,
             wallet=wallet,
-            key=key
+            key=key,
         )
 
     ######################################################################
     # read calls
     ######################################################################
 
     # makerFee() -> (uint265)
@@ -98,15 +93,17 @@
         :return: the minimum amount of pay_gem that can be sold in an offer
         :rtype: int
         """
 
         return self.contract.functions.getMinSell(pay_gem).call()
 
     # getBestOffer(sell_gem (address), buy_gem (address)) -> uint256
-    def get_best_offer(self, sell_gem: ChecksumAddress, buy_gem: ChecksumAddress) -> int:
+    def get_best_offer(
+        self, sell_gem: ChecksumAddress, buy_gem: ChecksumAddress
+    ) -> int:
         """Returns the best offer for the given pair of tokens
 
         :param sell_gem: the address of the token being sold by the maker
         :type sell_gem: str
         :param buy_gem: the address of the token being bought by the maker
         :type buy_gem: str
         :return: the id of the best offer on the book, None if there is no offer on the book
@@ -136,15 +133,17 @@
         :return: the id of the offer that is better than the given offer, none if there is no better offer
         :rtype: int
         """
 
         return self.contract.functions.getBetterOffer(id).call()
 
     # getOfferCount(sell_gem (address), buy_gem (address)) -> uint256
-    def get_offer_count(self, sell_gem: ChecksumAddress, buy_gem: ChecksumAddress) -> int:
+    def get_offer_count(
+        self, sell_gem: ChecksumAddress, buy_gem: ChecksumAddress
+    ) -> int:
         """Returns the number of offers for a token pair
 
         :param sell_gem: the address of the token being sold by the maker
         :type sell_gem: ChecksumAddress
         :param buy_gem: the address of the token being bought by the maker
         :type buy_gem: ChecksumAddress
         :return: the number of offers for a token pair, None if there are no offers for the token pair
@@ -163,56 +162,54 @@
         :rtype: int
         """
         return self.contract.functions.calculateFees(amount, True).call()
 
     # getBuyAmountWithFee(buy_gem (address), pay_gem (address), pay_amt (unit256)) ->
     # (buy_amt (uint256), approvalAmount (uint256))
     def get_buy_amount_with_fee(
-        self,
-        buy_gem: ChecksumAddress,
-        pay_gem: ChecksumAddress,
-        pay_amt: int
+        self, buy_gem: ChecksumAddress, pay_gem: ChecksumAddress, pay_amt: int
     ) -> Tuple[int, int]:
         """Returns the amount of the buy_gem you will receive if you send the pay_amt to the contract along with the
         amount to approve for the transaction
 
         :param buy_gem: the address of the token being bought
         :type buy_gem: ChecksumAddress
         :param pay_gem: the address of the token being sold
         :type pay_gem: ChecksumAddress
         :param pay_amt: the amount of the token being sold to receive the token being bought
         :type pay_amt: int
         :return: (buy_amt, approvalAmount) the amount of tokens that will be received and the amount to approve for the
             transaction
         :rtype: Tuple[int, int]
         """
-        return self.contract.functions.getBuyAmountWithFee(buy_gem, pay_gem, pay_amt).call()
+        return self.contract.functions.getBuyAmountWithFee(
+            buy_gem, pay_gem, pay_amt
+        ).call()
 
     # getPayAmountWithFee(pay_gem (address), buy_gem (address), buy_amt (unit256)) ->
     # (buy_amt (uint256), approvalAmount (uint256))
     def get_pay_amount_with_fee(
-        self,
-        pay_gem: ChecksumAddress,
-        buy_gem: ChecksumAddress,
-        buy_amt: int
+        self, pay_gem: ChecksumAddress, buy_gem: ChecksumAddress, buy_amt: int
     ) -> Tuple[int, int]:
         """Returns the amount of the pay_gem you will need to pay to the contract to receive the buy_amt along with the
         amount to approve for the transaction
 
         :param buy_gem: the address of the token being bought
         :type buy_gem: ChecksumAddress
         :param pay_gem: the address of the token being sold
         :type pay_gem: ChecksumAddress
         :param buy_amt: the amount of the token being bought
         :type buy_amt: int
         :return: (pay_amt, approvalAmount) the amount of tokens that will be paid and the amount to approve for the
             transaction
         :rtype: Tuple[int, int]
         """
-        return self.contract.functions.getPayAmountWithFee(buy_gem, pay_gem, buy_amt).call()
+        return self.contract.functions.getPayAmountWithFee(
+            buy_gem, pay_gem, buy_amt
+        ).call()
 
     ######################################################################
     # write calls
     ######################################################################
 
     # offer offer(pay_amt (uint256), pay_gem (address), buy_amt (uint256), buy_gem (address), pos (uint256),
     # owner (address), recipient (address)) -> uint256
@@ -225,15 +222,15 @@
         pos: int = 0,
         rounding: bool = True,
         owner: Optional[ChecksumAddress] = None,
         recipient: Optional[ChecksumAddress] = None,
         nonce: Optional[int] = None,
         gas: Optional[int] = None,
         max_fee_per_gas: Optional[int] = None,
-        max_priority_fee_per_gas: Optional[int] = None
+        max_priority_fee_per_gas: Optional[int] = None,
     ) -> TransactionReceipt:
         """Make a new offer to buy the buy_amt of the buy_gem token in exchange for the pay_amt of the pay_gem token
 
         :param pay_amt: the amount of the token being sold
         :type pay_amt: int
         :param pay_gem: the address of the token being sold
         :type pay_gem: ChecksumAddress
@@ -264,38 +261,42 @@
             estimate the max_priority_fee_per_gas (optional, default is None)
         :type max_priority_fee_per_gas: Optional[int]
         :return: An object representing the transaction receipt
         :rtype: TransactionReceipt
         """
 
         if not self.signing_permissions:
-            raise Exception(f"cannot write transaction without signing rights. "
-                            f"re-instantiate {self.__class__} with a wallet and private key")
+            raise Exception(
+                f"cannot write transaction without signing rights. "
+                f"re-instantiate {self.__class__} with a wallet and private key"
+            )
 
         owner = owner if owner is not None else self.wallet
         recipient = recipient if recipient is not None else self.wallet
 
-        offer = self.contract.functions.offer(pay_amt, pay_gem, buy_amt, buy_gem, pos, rounding, owner, recipient)
+        offer = self.contract.functions.offer(
+            pay_amt, pay_gem, buy_amt, buy_gem, pos, rounding, owner, recipient
+        )
 
         return self._default_transaction_handler(
             instantiated_contract_function=offer,
             gas=gas,
             nonce=nonce,
             max_fee_per_gas=max_fee_per_gas,
-            max_priority_fee_per_gas=max_priority_fee_per_gas
+            max_priority_fee_per_gas=max_priority_fee_per_gas,
         )
 
     # cancel(id (uint256)) -> bool
     def cancel(
         self,
         id: int,
         nonce: Optional[int] = None,
         gas: Optional[int] = None,
         max_fee_per_gas: Optional[int] = None,
-        max_priority_fee_per_gas: Optional[int] = None
+        max_priority_fee_per_gas: Optional[int] = None,
     ) -> TransactionReceipt:
         """Cancel an offer by offer id
 
         :param id: the id of the offer to cancel
         :type id: int
         :param nonce: nonce of the transaction, defaults to calling the chain state to get the nonce.
             (optional, default is None)
@@ -315,28 +316,28 @@
         cancel = self.contract.functions.cancel(id)
 
         return self._default_transaction_handler(
             instantiated_contract_function=cancel,
             gas=gas,
             nonce=nonce,
             max_fee_per_gas=max_fee_per_gas,
-            max_priority_fee_per_gas=max_priority_fee_per_gas
+            max_priority_fee_per_gas=max_priority_fee_per_gas,
         )
 
     # batchOffer(payAmts (uint[]), payGems (address[]), buyAmts (uint[]), buyGems (address[])) -> uint256[]
     def batch_offer(
         self,
         pay_amts: List[int],
         pay_gems: List[ChecksumAddress],
         buy_amts: List[int],
         buy_gems: List[ChecksumAddress],
         nonce: Optional[int] = None,
         gas: Optional[int] = None,
         max_fee_per_gas: Optional[int] = None,
-        max_priority_fee_per_gas: Optional[int] = None
+        max_priority_fee_per_gas: Optional[int] = None,
     ) -> TransactionReceipt:
         """Batch the placement of a set of offers in one transaction
 
         :param pay_amts: the amounts of the token being sold
         :type pay_amts: List[int]
         :param pay_gems: the addresses of the tokens being sold
         :type pay_gems: List[ChecksumAddress]
@@ -355,34 +356,38 @@
         :param max_priority_fee_per_gas: max priority fee that can be paid for gas, defaults to calling the chain to
             estimate the max_priority_fee_per_gas (optional, default is None)
         :type max_priority_fee_per_gas: Optional[int]
         :return: An object representing the transaction receipt
         :rtype: TransactionReceipt
         """
         if not (len(pay_amts) == len(pay_gems) == len(buy_amts) == len(buy_gems)):
-            raise Exception("mismatches lengths in pay_amts, pay_gems, buy_amts and buy_gems")
+            raise Exception(
+                "mismatches lengths in pay_amts, pay_gems, buy_amts and buy_gems"
+            )
 
-        batch_offer = self.contract.functions.batchOffer(pay_amts, pay_gems, buy_amts, buy_gems)
+        batch_offer = self.contract.functions.batchOffer(
+            pay_amts, pay_gems, buy_amts, buy_gems
+        )
 
         return self._default_transaction_handler(
             instantiated_contract_function=batch_offer,
             gas=gas,
             nonce=nonce,
             max_fee_per_gas=max_fee_per_gas,
-            max_priority_fee_per_gas=max_priority_fee_per_gas
+            max_priority_fee_per_gas=max_priority_fee_per_gas,
         )
 
     # batchCancel (ids (uint256[])) -> bool[]
     def batch_cancel(
         self,
         ids: List[int],
         nonce: Optional[int] = None,
         gas: Optional[int] = None,
         max_fee_per_gas: Optional[int] = None,
-        max_priority_fee_per_gas: Optional[int] = None
+        max_priority_fee_per_gas: Optional[int] = None,
     ) -> TransactionReceipt:
         """Cancel a set offer by offer id in a single transaction
 
         :param ids: the ids of the offers to cancel
         :type ids: List[int]
         :param nonce: nonce of the transaction, defaults to calling the chain state to get the nonce.
             (optional, default is None)
@@ -401,30 +406,30 @@
         cancels = self.contract.functions.batchCancel(ids)
 
         return self._default_transaction_handler(
             instantiated_contract_function=cancels,
             gas=gas,
             nonce=nonce,
             max_fee_per_gas=max_fee_per_gas,
-            max_priority_fee_per_gas=max_priority_fee_per_gas
+            max_priority_fee_per_gas=max_priority_fee_per_gas,
         )
 
     # batchRequote (ids (uint256[]), payAmts (uint[]), payGems (address[]), buyAmts (uint[]), buyGems (address[]))
     # -> uint256[]
     def batch_requote(
         self,
         ids: List[int],
         pay_amts: List[int],
         pay_gems: List[ChecksumAddress],
         buy_amts: List[int],
         buy_gems: List[ChecksumAddress],
         nonce: Optional[int] = None,
         gas: Optional[int] = None,
         max_fee_per_gas: Optional[int] = None,
-        max_priority_fee_per_gas: Optional[int] = None
+        max_priority_fee_per_gas: Optional[int] = None,
     ) -> TransactionReceipt:
         """Batch update a set of offers in a single transaction and return a list of new offer ids
 
         :param ids: the ids of the offers to cancel
         :type ids: List[int]
         :param pay_amts: the amounts of the token being sold
         :type pay_amts: List[int]
@@ -445,35 +450,37 @@
         :param max_priority_fee_per_gas: max priority fee that can be paid for gas, defaults to calling the chain to
             estimate the max_priority_fee_per_gas (optional, default is None)
         :type max_priority_fee_per_gas: Optional[int]
         :return: An object representing the transaction receipt
         :rtype: TransactionReceipt
         """
 
-        batch_requote = self.contract.functions.batchRequote(ids, pay_amts, pay_gems, buy_amts, buy_gems)
+        batch_requote = self.contract.functions.batchRequote(
+            ids, pay_amts, pay_gems, buy_amts, buy_gems
+        )
 
         return self._default_transaction_handler(
             instantiated_contract_function=batch_requote,
             gas=gas,
             nonce=nonce,
             max_fee_per_gas=max_fee_per_gas,
-            max_priority_fee_per_gas=max_priority_fee_per_gas
+            max_priority_fee_per_gas=max_priority_fee_per_gas,
         )
 
     # sellAllAmount(pay_gem (address), pay_amt (uint256), buy_gem (address), min_fill_amount (uint256)) -> uint256
     def sell_all_amount(
         self,
         pay_gem: ChecksumAddress,
         pay_amt: int,
         buy_gem: ChecksumAddress,
         min_fill_amount: int,
         nonce: Optional[int] = None,
         gas: Optional[int] = None,
         max_fee_per_gas: Optional[int] = None,
-        max_priority_fee_per_gas: Optional[int] = None
+        max_priority_fee_per_gas: Optional[int] = None,
     ) -> TransactionReceipt:
         """Sell the pay_amt of the pay_gem token in exchange for buy_gem, on the condition that you receive at least the
         min_fill_amount of the buy_gem token
 
         :param pay_gem: the address of the tokens being sold
         :type pay_gem: ChecksumAddress
         :param pay_amt: the amount of the token being sold
@@ -492,35 +499,37 @@
         :type max_fee_per_gas: Optional[int]
         :param max_priority_fee_per_gas: max priority fee that can be paid for gas, defaults to calling the chain to
             estimate the max_priority_fee_per_gas (optional, default is None)
         :type max_priority_fee_per_gas: Optional[int]
         :return: An object representing the transaction receipt
         :rtype: TransactionReceipt
         """
-        sell_all_amount = self.contract.functions.sellAllAmount(pay_gem, pay_amt, buy_gem, min_fill_amount)
+        sell_all_amount = self.contract.functions.sellAllAmount(
+            pay_gem, pay_amt, buy_gem, min_fill_amount
+        )
 
         return self._default_transaction_handler(
             instantiated_contract_function=sell_all_amount,
             gas=gas,
             nonce=nonce,
             max_fee_per_gas=max_fee_per_gas,
-            max_priority_fee_per_gas=max_priority_fee_per_gas
+            max_priority_fee_per_gas=max_priority_fee_per_gas,
         )
 
     # buyAllAmount(buy_gem (address), buy_amt (uint256), pay_gem (address), max_fill_amount (uint256)) -> uint256
     def buy_all_amount(
         self,
         buy_gem: ChecksumAddress,
         buy_amt: int,
         pay_gem: ChecksumAddress,
         max_fill_amount: int,
         nonce: Optional[int] = None,
         gas: Optional[int] = None,
         max_fee_per_gas: Optional[int] = None,
-        max_priority_fee_per_gas: Optional[int] = None
+        max_priority_fee_per_gas: Optional[int] = None,
     ) -> TransactionReceipt:
         """Buy the buy_amt of the buy_gem token in exchange for pay_gem, on the condition that it does not exceed the
         max_fill_amount of the pay_gem token
 
         :param buy_gem: the address of the tokens being bought
         :type buy_gem: ChecksumAddress
         :param buy_amt: the amount of the token being bought
@@ -539,16 +548,18 @@
         :type max_fee_per_gas: Optional[int]
         :param max_priority_fee_per_gas: max priority fee that can be paid for gas, defaults to calling the chain to
             estimate the max_priority_fee_per_gas (optional, default is None)
         :type max_priority_fee_per_gas: Optional[int]
         :return: An object representing the transaction receipt
         :rtype: TransactionReceipt
         """
-        buy_all_amount = self.contract.functions.buyAllAmount(buy_gem, buy_amt, pay_gem, max_fill_amount)
+        buy_all_amount = self.contract.functions.buyAllAmount(
+            buy_gem, buy_amt, pay_gem, max_fill_amount
+        )
 
         return self._default_transaction_handler(
             instantiated_contract_function=buy_all_amount,
             gas=gas,
             nonce=nonce,
             max_fee_per_gas=max_fee_per_gas,
-            max_priority_fee_per_gas=max_priority_fee_per_gas
-        )
+            max_priority_fee_per_gas=max_priority_fee_per_gas,
+        )
```

### Comparing `rubi-2.1.1/rubi/contracts/router.py` & `rubi-2.1.2/rubi/contracts/router.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,48 +24,43 @@
     """
 
     def __init__(
         self,
         w3: Web3,
         contract: Contract,
         wallet: Optional[ChecksumAddress] = None,
-        key: Optional[str] = None
+        key: Optional[str] = None,
     ) -> None:
         """constructor method"""
-        super().__init__(
-            w3=w3,
-            contract=contract,
-            wallet=wallet,
-            key=key
-        )
+        super().__init__(w3=w3, contract=contract, wallet=wallet, key=key)
 
     @classmethod
     def from_network(
         cls,
         network: Network,
         wallet: Optional[ChecksumAddress] = None,
-        key: Optional[str] = None
+        key: Optional[str] = None,
     ) -> "RubiconRouter":
         """Create a RubiconRouter instance based on a Network instance.
 
         :param network: A Network instance.
         :type network: Network
-        :param wallet: Optional wallet address to use for interacting with the contract (optional, default is None). 
+        :param wallet: Optional wallet address to use for interacting with the contract (optional, default is None).
         :type wallet: Optional[ChecksumAddress]
         :param key: Optional private key for the wallet (optional, default is None).
         :type key: Optional[str]
         :return: A RubiconRouter instance based on the Network instance.
         :rtype: RubiconRouter
         """
         return cls.from_address_and_abi(
             w3=network.w3,
             address=network.rubicon.router.address,
             contract_abi=network.rubicon.router.abi,
             wallet=wallet,
-            key=key
+            key=key,
         )
 
     ######################################################################
     # read calls
     ######################################################################
 
     # getMakerBalance(baseToken (address), tokens (List[address]), maker (address))
@@ -129,15 +124,17 @@
             selling the asset, while the bids list represents the orders buying the asset.
         :rtype: Tuple[List[List[int]], List[List[int]]]
         """
 
         return self.contract.functions.getBookFromPair(asset, quote).call()
 
     # getBookDepth(tokenIn (address), tokenOut (address)) -> (uint256 depth, uint256 bestOfferID)
-    def get_book_depth(self, token_in: ChecksumAddress, token_out: ChecksumAddress) -> Tuple[int, int]:
+    def get_book_depth(
+        self, token_in: ChecksumAddress, token_out: ChecksumAddress
+    ) -> Tuple[int, int]:
         """Retrieves the depth of one side of the order book for a specific token pair along with the id of the best
         offer.
 
         :param token_in: The address of the quote.
         :type token_in: ChecksumAddress
         :param token_out: The address of the asset.
         :type token_out: ChecksumAddress
@@ -145,17 +142,15 @@
         :rtype: Tuple[int, int]
         """
 
         return self.contract.functions.getBookDepth(token_in, token_out).call()
 
     # getBestOfferAndInfo(asset (address), quote (address)) -> (uint256 id, uint256, address, uint256, address)
     def get_best_offer_and_info(
-        self,
-        asset: ChecksumAddress,
-        quote: ChecksumAddress
+        self, asset: ChecksumAddress, quote: ChecksumAddress
     ) -> Tuple[int, int, ChecksumAddress, int, ChecksumAddress]:
         """Retrieves the information and id of the best offer for a specific asset/quote pair.
 
         :param asset: The address of the asset token.
         :type asset: ChecksumAddress
         :param quote: The address of the quote token.
         :type quote: ChecksumAddress
@@ -163,74 +158,82 @@
             the buy_amt, and the address of the buy_gem.
         :rtype: Tuple[int, int, ChecksumAddress, int, ChecksumAddress]
         """
 
         return self.contract.functions.getBestOfferAndInfo(asset, quote).call()
 
     # getExpectedSwapFill(pay_amt (uint256), buy_amt_min (uint256), route (address[])) -> (uint256 amount)
-    def get_expected_swap_fill(self, pay_amt: int, buy_amt_min: int, route: List[ChecksumAddress]) -> int:
+    def get_expected_swap_fill(
+        self, pay_amt: int, buy_amt_min: int, route: List[ChecksumAddress]
+    ) -> int:
         """Estimates the expected amount including fees when swapping the specified payment amount using the specified
         route. reverts with an exception if the swap cannot achieve the buy_amt_min
 
         :param pay_amt: The payment amount.
         :type pay_amt: int
         :param buy_amt_min: The minimum buy amount.
         :type buy_amt_min: int
         :param route: The route of addresses representing the swap path.
         :type route: List[ChecksumAddress]
         :return: The estimated swap amount including fees.
         :rtype: int
         """
 
-        return self.contract.functions.getExpectedSwapFill(pay_amt, buy_amt_min, route).call()
+        return self.contract.functions.getExpectedSwapFill(
+            pay_amt, buy_amt_min, route
+        ).call()
 
     # getExpectedMultiswapFill(pay_amts (uint256[]), buy_amt_mins (uint256[]), routes (address[][]))
     # -> (uint256 amount)
     def get_expected_multiswap_fill(
         self,
         pay_amts: List[int],
         buy_amt_mins: List[int],
-        routes: List[List[ChecksumAddress]]
+        routes: List[List[ChecksumAddress]],
     ) -> int:
         """Estimates the expected amount including fees when swapping multiple specified payment amount using multiple
         specified routes. reverts with an exception if the multiswap cannot achieve the buy_amt_mins along each route
 
         :param pay_amts: The list of payment amounts for each swap.
         :type pay_amts: List[int]
         :param buy_amt_mins: The list of minimum buy amounts for each swap.
         :type buy_amt_mins: List[int]
         :param routes: The list of routes, where each route is a list of addresses representing the swap path.
         :type routes: List[List[ChecksumAddress]]
         :return: The estimated multi-swap amount.
         :rtype: int
         """
 
-        return self.contract.functions.getExpectedMultiswapFill(pay_amts, buy_amt_mins, routes).call()
+        return self.contract.functions.getExpectedMultiswapFill(
+            pay_amts, buy_amt_mins, routes
+        ).call()
 
     # checkClaimAllUserBonusTokens(address user, address[] targetBathTokens, address token)
     # -> (uint256 earnedAcrossPools)
     def check_claim_all_user_bonus_tokens(
         self,
         user: ChecksumAddress,
         target_bath_tokens: List[ChecksumAddress],
-        token: ChecksumAddress
+        token: ChecksumAddress,
     ) -> int:
         """Checks the all bonus tokens that can be claimed by a user earned across all specified rubicon pools.
 
         :param user: The address of the user.
         :type user: ChecksumAddress
         :param target_bath_tokens: The list of target bath tokens to claim bonus from.
         :type target_bath_tokens: List[ChecksumAddress]
         :param token: The address of the token for which the bonus is claimed.
         :type token: ChecksumAddress
         :return: The total amount earned across all pools.
         :rtype: int
         """
 
-        return self.contract.functions.checkClaimAllUserBonusTokens(user, target_bath_tokens, token).call()
+        return self.contract.functions.checkClaimAllUserBonusTokens(
+            user, target_bath_tokens, token
+        ).call()
 
     ######################################################################
     # write calls
     ######################################################################
 
     # multiswap(address[][] routes, uint256[] pay_amts, uint256[] buy_amts_min, address to) -> bool
     def multiswap(
@@ -238,15 +241,15 @@
         routes: List[List[ChecksumAddress]],
         pay_amts: List[int],
         buy_amts_min: List[int],
         to: ChecksumAddress,
         nonce: Optional[int] = None,
         gas: Optional[int] = None,
         max_fee_per_gas: Optional[int] = None,
-        max_priority_fee_per_gas: Optional[int] = None
+        max_priority_fee_per_gas: Optional[int] = None,
     ) -> TransactionReceipt:
         """Perform a multiple swaps for the specified payment amounts using the specified routes. Reverts with an
         exception if any of the swaps cannot achieve the buy_amt_min along the specified route.
 
         :param routes: The list of routes, where each route is a list of addresses representing the swap path.
         :type routes: List[List[ChecksumAddress]]
         :param pay_amts: The list of payment amounts for each swap.
@@ -266,35 +269,37 @@
         :param max_priority_fee_per_gas: Max priority fee that can be paid for gas. Defaults to calling the chain to
             estimate the max_priority_fee_per_gas (optional, default is None).
         :type max_priority_fee_per_gas: Optional[int]
         :return: An object representing the transaction receipt
         :rtype: TransactionReceipt
         """
 
-        multiswap = self.contract.functions.multiswap(routes, pay_amts, buy_amts_min, to)
+        multiswap = self.contract.functions.multiswap(
+            routes, pay_amts, buy_amts_min, to
+        )
 
         return self._default_transaction_handler(
             instantiated_contract_function=multiswap,
             gas=gas,
             nonce=nonce,
             max_fee_per_gas=max_fee_per_gas,
-            max_priority_fee_per_gas=max_priority_fee_per_gas
+            max_priority_fee_per_gas=max_priority_fee_per_gas,
         )
 
     # swap(uint256 pay_amt, uint256 buy_amt_min, address[] memory route, address to) -> uint256
     def swap(
         self,
         pay_amt: int,
         buy_amt_min: int,
         route: List[ChecksumAddress],
         to: ChecksumAddress,
         nonce: Optional[int] = None,
         gas: Optional[int] = None,
         max_fee_per_gas: Optional[int] = None,
-        max_priority_fee_per_gas: Optional[int] = None
+        max_priority_fee_per_gas: Optional[int] = None,
     ) -> TransactionReceipt:
         """Perform a swap operation with the specified payment amount using the specified route and paying out to the
         recipient. Reverts if the swap does not result in the buy_min_amount.
 
         :param pay_amt: The payment amount.
         :type pay_amt: int
         :param buy_amt_min: The minimum buy amount.
@@ -321,15 +326,15 @@
         swap = self.contract.functions.swap(pay_amt, buy_amt_min, route, to)
 
         return self._default_transaction_handler(
             instantiated_contract_function=swap,
             gas=gas,
             nonce=nonce,
             max_fee_per_gas=max_fee_per_gas,
-            max_priority_fee_per_gas=max_priority_fee_per_gas
+            max_priority_fee_per_gas=max_priority_fee_per_gas,
         )
 
     # TODO
     #  sellAllAmountForETH
     #  sellAllAmountWithETH
     #  buyAllAmountWithETH
     #  buyAllAmountForETH
```

### Comparing `rubi-2.1.1/rubi/data/market.py` & `rubi-2.1.2/rubi/data/market.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,82 +16,85 @@
 )
 
 
 class MarketData:
     """This class represents the RubiconV2 Subgraph, which contains data primarily related to the RubiconMarket.sol
     contract. If a Network object is not passed in instantiation then this class will only be used to query data related
      to the subgraph.
-    
-    :param subgrounds: a Subgrounds instance 
+
+    :param subgrounds: a Subgrounds instance
     :type subgrounds: Subgrounds
         param subgraph_url: a RubiconV2 Subgraph url endpoint that should be utilized for this class
     :type subgraph_url: str
     :param network: a Network object, native to the package
     :type network: Network
     """
 
     def __init__(
         self,
         subgrounds: Subgrounds,
         subgraph_url: str,
         network: Optional[Network] = None,
-        network_tokens: Optional[Dict[ChecksumAddress, ERC20]] = None
+        network_tokens: Optional[Dict[ChecksumAddress, ERC20]] = None,
     ):
         """constructor method"""
         self.sg = subgrounds
         self.subgraph_url = subgraph_url
         self.network = network  # type: Network | None
         self.tokens = network_tokens  # type: Dict[ChecksumAddress, ERC20] | None
 
-        # initialize the subgraph 
+        # initialize the subgraph
         try:
             self.data = self.sg.load_subgraph(self.subgraph_url)
             # TODO: we should add a check here to guarantee the schema matches what we expect to be receiving
         except:
-            # TODO: not sure exactly what error we should be throwing here, this is if the url does not work 
-            raise ValueError(f"subgraph_url: {subgraph_url} failed when attempting to load.")
+            # TODO: not sure exactly what error we should be throwing here, this is if the url does not work
+            raise ValueError(
+                f"subgraph_url: {subgraph_url} failed when attempting to load."
+            )
 
         # Initialize the query classes
         self.offer_query = OrderQuery(self.sg, self.data, self.network, self.tokens)
 
     @classmethod
     def from_network_with_tokens(
-        cls,
-        network: Network,
-        network_tokens: Dict[ChecksumAddress, ERC20]
+        cls, network: Network, network_tokens: Dict[ChecksumAddress, ERC20]
     ) -> "MarketData":
-
         """Initialize a MarketData object using a Network object."""
         return cls(
             subgrounds=network.subgrounds,
             subgraph_url=network.market_data_url,
             network=network,
-            network_tokens=network_tokens
+            network_tokens=network_tokens,
         )
 
     #####################################
     # Subgraph Query Methods            #
     #####################################
 
     # TODO: refactor using a decorator to handle the parameter validation
     def get_offers(
         self,
         maker: Optional[str] = None,
         from_address: Optional[str] = None,
         pair_name: Optional[str] = None,
         book_side: Optional[OrderSide] = None,
-        pay_gem: Optional[str] = None,  # TODO: maybe we should allow the user to pass in an address here?
-        buy_gem: Optional[str] = None,  # TODO: maybe we should allow the user to pass in an address here?
+        pay_gem: Optional[
+            str
+        ] = None,  # TODO: maybe we should allow the user to pass in an address here?
+        buy_gem: Optional[
+            str
+        ] = None,  # TODO: maybe we should allow the user to pass in an address here?
         open: Optional[bool] = None,
         start_time: Optional[int] = None,
         end_time: Optional[int] = None,
         first: Optional[int] = 1000,
-        order_by: Optional[str] = 'timestamp',
-        order_direction: Optional[str] = 'desc',
-        formatted: Optional[bool] = False
+        order_by: Optional[str] = "timestamp",
+        order_direction: Optional[str] = "desc",
+        formatted: Optional[bool] = False,
     ) -> pd.DataFrame:
         """Returns a dataframe of offers placed on the market contract, with the option to pass in filters.
 
         :param maker: the address of the maker of the offer
         :type maker: str
         :param from_address: the address that originated the transaction that created the offer
         :type from_address: str
@@ -109,79 +112,128 @@
         :type first: int
         :param order_by: the field to order the offers by (default: timestamp, options: timestamp, price) TODO: expand this list
         :type order_by: str
         :param order_direction: the direction to order the offers by (default: desc, options: asc, desc)
         :type order_direction: str
         :param formatted: whether or not to return the formatted fields (default: False, requires a network object to be passed)
         :return: a dataframe of offers placed on the market contract
-        :rtype: pd.DataFrame 
+        :rtype: pd.DataFrame
         """
 
         # if we want formatted fields, make sure we have a network object
         # TODO: we could pass this to the offers_query method and handle it there - if we start to utilize something like **kargs lets do that
         if formatted and not self.network:
-            raise ValueError("Cannot return formatted fields without a network object initialized on the class.")
+            raise ValueError(
+                "Cannot return formatted fields without a network object initialized on the class."
+            )
 
         # handle the pair_name parameter
         if pair_name:
             base, quote = pair_name.split("/")
             base_asset = ERC20.from_network(name=base, network=self.network)
             quote_asset = ERC20.from_network(name=quote, network=self.network)
 
         # handle the book_side parameter
         if book_side and pair_name:
-
             match book_side:
                 case OrderSide.BUY:
-                    buy_query = self.offer_query.offers_query(order_by, order_direction, first, maker, from_address,
-                                                              pay_gem=quote_asset.address, buy_gem=base_asset.address,
-                                                              open=open, start_time=start_time, end_time=end_time)
+                    buy_query = self.offer_query.offers_query(
+                        order_by,
+                        order_direction,
+                        first,
+                        maker,
+                        from_address,
+                        pay_gem=quote_asset.address,
+                        buy_gem=base_asset.address,
+                        open=open,
+                        start_time=start_time,
+                        end_time=end_time,
+                    )
                     buy_fields = self.offer_query.offers_fields(buy_query, formatted)
                     buy_df = self.offer_query.query_offers(buy_fields, formatted)
                     buy_df[
-                        'side'] = 'buy'  # TODO: we could also pass this data to the offers_query method and handle it there, could help with price
+                        "side"
+                    ] = "buy"  # TODO: we could also pass this data to the offers_query method and handle it there, could help with price
 
                     return buy_df
 
                 case OrderSide.SELL:
-                    sell_query = self.offer_query.offers_query(order_by, order_direction, first, maker, from_address,
-                                                               pay_gem=base_asset.address, buy_gem=quote_asset.address,
-                                                               open=open, start_time=start_time, end_time=end_time)
+                    sell_query = self.offer_query.offers_query(
+                        order_by,
+                        order_direction,
+                        first,
+                        maker,
+                        from_address,
+                        pay_gem=base_asset.address,
+                        buy_gem=quote_asset.address,
+                        open=open,
+                        start_time=start_time,
+                        end_time=end_time,
+                    )
                     sell_fields = self.offer_query.offers_fields(sell_query, formatted)
                     sell_df = self.offer_query.query_offers(sell_fields, formatted)
                     sell_df[
-                        'side'] = 'sell'  # TODO: we could also pass this data to the offers_query method and handle it there, could help with price
+                        "side"
+                    ] = "sell"  # TODO: we could also pass this data to the offers_query method and handle it there, could help with price
 
                     return sell_df
 
                 case OrderSide.NEUTRAL:
-                    buy_query = self.offer_query.offers_query(order_by, order_direction, first, maker, from_address,
-                                                              pay_gem=quote_asset.address, buy_gem=base_asset.address,
-                                                              open=open, start_time=start_time, end_time=end_time)
+                    buy_query = self.offer_query.offers_query(
+                        order_by,
+                        order_direction,
+                        first,
+                        maker,
+                        from_address,
+                        pay_gem=quote_asset.address,
+                        buy_gem=base_asset.address,
+                        open=open,
+                        start_time=start_time,
+                        end_time=end_time,
+                    )
                     buy_fields = self.offer_query.offers_fields(buy_query, formatted)
                     buy_df = self.offer_query.query_offers(buy_fields, formatted)
                     buy_df[
-                        'side'] = 'buy'  # TODO: we could also pass this data to the offers_query method and handle it there, could help with price
+                        "side"
+                    ] = "buy"  # TODO: we could also pass this data to the offers_query method and handle it there, could help with price
 
-                    sell_query = self.offer_query.offers_query(order_by, order_direction, first, maker, from_address,
-                                                               pay_gem=base_asset.address, buy_gem=quote_asset.address,
-                                                               open=open, start_time=start_time, end_time=end_time)
+                    sell_query = self.offer_query.offers_query(
+                        order_by,
+                        order_direction,
+                        first,
+                        maker,
+                        from_address,
+                        pay_gem=base_asset.address,
+                        buy_gem=quote_asset.address,
+                        open=open,
+                        start_time=start_time,
+                        end_time=end_time,
+                    )
                     sell_fields = self.offer_query.offers_fields(sell_query, formatted)
                     sell_df = self.offer_query.query_offers(sell_fields, formatted)
                     sell_df[
-                        'side'] = 'sell'  # TODO: we could also pass this data to the offers_query method and handle it there, could help with price
+                        "side"
+                    ] = "sell"  # TODO: we could also pass this data to the offers_query method and handle it there, could help with price
 
                     # TODO: decide what we want to do here, maybe we just return both dataframes?
 
                     # reset the index  # need to pass a somewhat more complicated ordering here to comply with what happened in the same block time
                     return pd.concat([buy_df, sell_df]).reset_index(drop=True)
 
         # handle the pay_gem and buy_gem parameters
         elif pay_gem and buy_gem:
-
-            query = self.offer_query.offers_query(order_by, order_direction, first, maker, from_address,
-                                                  pay_gem=pay_gem, buy_gem=buy_gem, open=open, start_time=start_time,
-                                                  end_time=end_time)
+            query = self.offer_query.offers_query(
+                order_by,
+                order_direction,
+                first,
+                maker,
+                from_address,
+                pay_gem=pay_gem,
+                buy_gem=buy_gem,
+                open=open,
+                start_time=start_time,
+                end_time=end_time,
+            )
             fields = self.offer_query.offers_fields(query)
             df = self.offer_query.query_offers(fields)
 
             return df
```

### Comparing `rubi-2.1.1/rubi/network/network.py` & `rubi-2.1.2/rubi/network/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         currency: str,
         rpc_url: str,
         explorer_url: str,
         market_data_url: str,
         rubicon: dict,
         token_addresses: dict,
         # optional custom token config file from the user
-        custom_token_addresses_file: Optional[str] = None
+        custom_token_addresses_file: Optional[str] = None,
     ):
         """Initializes a Network instance.
 
         :param path: The path to the network configuration folder.
         :type path: str
         :param w3: The Web3 instance connected to the network.
         :type w3: Web3
@@ -83,33 +83,44 @@
         checksummed_token_addresses: dict[str, ChecksumAddress] = {}
         for k, v in token_addresses.items():
             checksummed_token_addresses[k] = self.w3.to_checksum_address(v)
 
         if custom_token_addresses_file:
             working_directory = os.getcwd()
 
-            if not (custom_token_addresses_file.endswith(".yaml") or custom_token_addresses_file.endswith(".yml")):
-                raise Exception(f"token_config_file: {custom_token_addresses_file} must be a yaml file.")
+            if not (
+                custom_token_addresses_file.endswith(".yaml")
+                or custom_token_addresses_file.endswith(".yml")
+            ):
+                raise Exception(
+                    f"token_config_file: {custom_token_addresses_file} must be a yaml file."
+                )
 
             try:
                 with open(f"{working_directory}/{custom_token_addresses_file}") as f:
                     custom_token_addresses = yaml.safe_load(f)
                     for k, v in custom_token_addresses.items():
                         checksummed_token_addresses[k] = self.w3.to_checksum_address(v)
             except FileNotFoundError:
-                raise Exception(f"could not find token_config_file, expected it to be a yaml file here: "
-                                f"{working_directory}/{custom_token_addresses_file}.")
+                raise Exception(
+                    f"could not find token_config_file, expected it to be a yaml file here: "
+                    f"{working_directory}/{custom_token_addresses_file}."
+                )
             except AttributeError:
-                raise Exception(f"{custom_token_addresses_file} cannot be empty, should be in the format: "
-                                f"token_symbol: address, e.g. WETH: chain_specific_weth_address")
+                raise Exception(
+                    f"{custom_token_addresses_file} cannot be empty, should be in the format: "
+                    f"token_symbol: address, e.g. WETH: chain_specific_weth_address"
+                )
 
         self.token_addresses = checksummed_token_addresses
 
     @classmethod
-    def from_config(cls, http_node_url: str, custom_token_addresses_file: Optional[str] = None) -> "Network":
+    def from_config(
+        cls, http_node_url: str, custom_token_addresses_file: Optional[str] = None
+    ) -> "Network":
         """Create a Network instance based on the node url provided. A call is then made to this node to get the
         chain_id which links to network_config/{network_name}/ using the NetworkId Enum.
 
         :param http_node_url: The URL of the HTTP node for the network.
         :type http_node_url: str
         :param custom_token_addresses_file: The name of a yaml file (relative to the current working directory) with
             custom token addresses. Overwrites the token config found in network_config/{chain}/network.yaml.
@@ -130,19 +141,21 @@
             with open(f"{path}/network.yaml") as f:
                 network_data = yaml.safe_load(f)
                 return cls(
                     path=path,
                     w3=w3,
                     subgrounds=subgrounds,
                     custom_token_addresses_file=custom_token_addresses_file,
-                    **network_data
+                    **network_data,
                 )
         except FileNotFoundError:
-            raise Exception(f"no network config found for {network_name}, there should be a corresponding folder in "
-                            f"the network_config directory")
+            raise Exception(
+                f"no network config found for {network_name}, there should be a corresponding folder in "
+                f"the network_config directory"
+            )
 
     def __repr__(self):
         items = ("{}={!r}".format(k, self.__dict__[k]) for k in self.__dict__)
         return "{}({})".format(type(self).__name__, ", ".join(items))
 
 
 class RubiconContracts:
@@ -167,16 +180,15 @@
 
     def __repr__(self):
         items = ("{}={!r}".format(k, self.__dict__[k]) for k in self.__dict__)
         return "{}({})".format(type(self).__name__, ", ".join(items))
 
 
 class ContractRepr:
-    """This class represents a contract on a specific network.
-    """
+    """This class represents a contract on a specific network."""
 
     def __init__(self, path: str, w3: Web3, name: str, address: str) -> None:
         """Initialize a ContractRepr instance which is a representation of a contract containing the contract address
         and abi.
 
         :param path: The path to the network configuration.
         :type path: str
```

### Comparing `rubi-2.1.1/rubi/rubicon_types/order.py` & `rubi-2.1.2/rubi/rubicon_types/order.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 from _decimal import Decimal
 from enum import Enum
 from typing import Optional, Union, List, Dict
 
 from eth_typing import ChecksumAddress
 
-from rubi.contracts.contract_types.events import BaseEvent, EmitOfferEvent, EmitCancelEvent, EmitTakeEvent, \
-    EmitDeleteEvent, EmitFeeEvent
+from rubi.contracts.contract_types.events import (
+    BaseEvent,
+    EmitOfferEvent,
+    EmitCancelEvent,
+    EmitTakeEvent,
+    EmitDeleteEvent,
+    EmitFeeEvent,
+)
 from rubi.rubicon_types.pair import Pair
 
 
 class OrderSide(Enum):
     """Enumeration representing the order side."""
+
     BUY = "BUY"
     SELL = "SELL"
     NEUTRAL = "NEUTRAL"
 
     def sign(self) -> int:
         """
         :return: Numerical value of the side.
@@ -29,14 +36,15 @@
 
             case OrderSide.SELL:
                 return -1
 
 
 class OrderType(Enum):
     """Enumeration representing the order type."""
+
     MARKET = "MARKET"
     LIMIT = "LIMIT"
 
     # Only used for events coming from the RubiconMarket
     LIMIT_TAKEN = "LIMIT_TAKEN"
     LIMIT_DELETED = "LIMIT_DELETED"
     CANCEL = "CANCEL"
@@ -88,20 +96,21 @@
     ):
         """constructor method."""
 
         super().__init__(
             pair_name=pair_name,
             order_type=OrderType.MARKET,
             order_side=order_side,
-
         )
         self.size = size
 
         if worst_execution_price is None:
-            self.worst_execution_price = Decimal("0") if order_side.SELL else Decimal("10") ** Decimal("7")
+            self.worst_execution_price = (
+                Decimal("0") if order_side.SELL else Decimal("10") ** Decimal("7")
+            )
         else:
             self.worst_execution_price = worst_execution_price
 
 
 class NewLimitOrder(BaseNewOrder):
     """Class representing a new limit order
 
@@ -112,19 +121,15 @@
     :param size: The size of the order.
     :type size: Decimal
     :param price: The price of the order.
     :type price: Decimal
     """
 
     def __init__(
-        self,
-        pair_name: str,
-        order_side: OrderSide,
-        size: Decimal,
-        price: Decimal
+        self, pair_name: str, order_side: OrderSide, size: Decimal, price: Decimal
     ):
         """constructor method."""
         super().__init__(
             pair_name=pair_name,
             order_type=OrderType.LIMIT,
             order_side=order_side,
         )
@@ -150,15 +155,15 @@
 
     def __init__(
         self,
         pair_name: str,
         order_side: OrderSide,
         order_id: int,
         size: Decimal,
-        price: Decimal
+        price: Decimal,
     ):
         """constructor method"""
         super().__init__(
             pair_name=pair_name,
             order_type=OrderType.LIMIT,
             order_side=order_side,
         )
@@ -173,31 +178,28 @@
 
     :param pair_name: The name of the trading pair.
     :type pair_name: str
     :param order_id: The ID of the order to cancel.
     :type order_id: int
     """
 
-    def __init__(
-        self,
-        pair_name: str,
-        order_id: int
-    ):
+    def __init__(self, pair_name: str, order_id: int):
         """constructor method"""
         super().__init__(
             pair_name=pair_name,
             order_type=OrderType.LIMIT,
             order_side=OrderSide.NEUTRAL,
         )
 
         self.order_id = order_id
 
 
 # TODO: add a new class for a limit order object that is returned from the subgraph
 
+
 class Transaction:
     """
     Class representing a transaction to be executed on chain
 
     :param orders: The list of orders to include in the transaction.
     :type orders: List[BaseNewOrder]
     :param nonce: The nonce for the transaction (optional).
@@ -212,19 +214,21 @@
 
     def __init__(
         self,
         orders: List[BaseNewOrder],
         nonce: Optional[int] = None,
         gas: Optional[int] = None,
         max_fee_per_gas: Optional[int] = None,
-        max_priority_fee_per_gas: Optional[int] = None
+        max_priority_fee_per_gas: Optional[int] = None,
     ):
         """constructor method"""
         if len(orders) < 1:
-            raise Exception("Transaction cannot be instantiated with an empty order list")
+            raise Exception(
+                "Transaction cannot be instantiated with an empty order list"
+            )
 
         self.orders = orders
         self.nonce = nonce
         self.gas = gas
         self.max_fee_per_gas = max_fee_per_gas
         self.max_priority_fee_per_gas = max_priority_fee_per_gas
 
@@ -234,15 +238,15 @@
         :return: dictionary of arguments used to send transactions.
         :rtype: Dict
         """
         args = {
             "nonce": self.nonce,
             "gas": self.gas,
             "max_fee_per_gas": self.max_fee_per_gas,
-            "max_priority_fee_per_gas": self.max_priority_fee_per_gas
+            "max_priority_fee_per_gas": self.max_priority_fee_per_gas,
         }
 
         return {key: value for key, value in args.items() if value is not None}
 
 
 class OrderEvent:
     """Class to represent Rubicon Market events as an order
@@ -282,15 +286,17 @@
         self.pair_name = pair_name
         self.order_side = order_side
         self.order_type = order_type
         self.price = price
         self.size = size
 
     @classmethod
-    def from_event(cls, pair: Pair, event: BaseEvent, wallet: ChecksumAddress) -> "OrderEvent":
+    def from_event(
+        cls, pair: Pair, event: BaseEvent, wallet: ChecksumAddress
+    ) -> "OrderEvent":
         """Create an OrderEvent from a BaseEvent emitted by the Rubicon Market.
 
         :param pair: The asset pair associated with the event.
         :type pair: Pair
         :param event: The event to convert.
         :type event: BaseEvent
         :param wallet: The wallet address associated with the event.
@@ -304,98 +310,102 @@
             if pair.bid_identifier == event.pair:
                 return cls._build_order(
                     event=event,
                     pair=pair,
                     side=OrderSide.BUY,
                     order_type=OrderType.LIMIT,
                     base_amt=event.buy_amt,
-                    quote_amt=event.pay_amt
+                    quote_amt=event.pay_amt,
                 )
             else:
                 return cls._build_order(
                     event=event,
                     pair=pair,
                     side=OrderSide.SELL,
                     order_type=OrderType.LIMIT,
                     base_amt=event.pay_amt,
-                    quote_amt=event.buy_amt
+                    quote_amt=event.buy_amt,
                 )
         elif isinstance(event, EmitCancelEvent):
             if pair.bid_identifier == event.pair:
                 return cls._build_order(
                     event=event,
                     pair=pair,
                     side=OrderSide.BUY,
                     order_type=OrderType.CANCEL,
                     base_amt=event.buy_amt,
-                    quote_amt=event.pay_amt
+                    quote_amt=event.pay_amt,
                 )
             else:
                 return cls._build_order(
                     event=event,
                     pair=pair,
                     side=OrderSide.SELL,
                     order_type=OrderType.CANCEL,
                     base_amt=event.pay_amt,
-                    quote_amt=event.buy_amt
+                    quote_amt=event.buy_amt,
                 )
         elif isinstance(event, EmitTakeEvent):
             # This is nuanced as we can either receive a take event for a market order or limit order we placed. When
             # we take the bid_identifier indicates selling into the bids while the ask identifier indicates buying
             # into the asks. While the reverse is true for when we make.
             if pair.bid_identifier == event.pair:
                 return cls._build_order(
                     event=event,
                     pair=pair,
                     side=OrderSide.BUY if wallet == event.maker else OrderSide.SELL,
-                    order_type=OrderType.LIMIT_TAKEN if wallet == event.maker else OrderType.MARKET,
+                    order_type=OrderType.LIMIT_TAKEN
+                    if wallet == event.maker
+                    else OrderType.MARKET,
                     base_amt=event.give_amt,
-                    quote_amt=event.take_amt
+                    quote_amt=event.take_amt,
                 )
             else:
                 return cls._build_order(
                     event=event,
                     pair=pair,
                     side=OrderSide.SELL if wallet == event.maker else OrderSide.BUY,
-                    order_type=OrderType.LIMIT_TAKEN if wallet == event.maker else OrderType.MARKET,
+                    order_type=OrderType.LIMIT_TAKEN
+                    if wallet == event.maker
+                    else OrderType.MARKET,
                     base_amt=event.take_amt,
-                    quote_amt=event.give_amt
+                    quote_amt=event.give_amt,
                 )
         elif isinstance(event, EmitDeleteEvent):
             if pair.bid_identifier == event.pair:
                 return cls._build_order(
                     event=event,
                     pair=pair,
                     side=None,
                     order_type=OrderType.LIMIT_DELETED,
                     base_amt=None,
-                    quote_amt=None
+                    quote_amt=None,
                 )
             else:
                 return cls._build_order(
                     event=event,
                     pair=pair,
                     side=None,
                     order_type=OrderType.LIMIT_DELETED,
                     base_amt=None,
-                    quote_amt=None
+                    quote_amt=None,
                 )
 
         else:
             Exception(f"{event.__class__} cannot be converted into an OrderEvent")
 
     @classmethod
     def _build_order(
         cls,
         event: Union[EmitOfferEvent, EmitCancelEvent, EmitTakeEvent, EmitDeleteEvent],
         pair: Pair,
         side: Optional[OrderSide],
         order_type: OrderType,
         base_amt: Optional[int],
-        quote_amt: Optional[int]
+        quote_amt: Optional[int],
     ) -> "OrderEvent":
         """Build an OrderEvent from event data.
 
         :param event: The event data.
         :type event: Union[EmitOfferEvent, EmitCancelEvent, EmitTakeEvent]
         :param pair: The asset pair associated with the event.
         :type pair: Pair
@@ -412,20 +422,22 @@
         """
         size = pair.base_asset.to_decimal(base_amt) if base_amt else None
         price = pair.quote_asset.to_decimal(quote_amt) / size if quote_amt else None
 
         return cls(
             limit_order_id=event.id,
             limit_order_owner=event.maker,
-            market_order_owner=event.taker if isinstance(event, EmitTakeEvent) else None,
+            market_order_owner=event.taker
+            if isinstance(event, EmitTakeEvent)
+            else None,
             pair_name=pair.name,
             order_side=side,
             order_type=order_type,
             size=size,
-            price=price
+            price=price,
         )
 
     def __repr__(self):
         items = ("{}={!r}".format(k, self.__dict__[k]) for k in self.__dict__)
         return "{}({})".format(type(self).__name__, ", ".join(items))
 
 
@@ -463,13 +475,13 @@
 
         return cls(
             id=event.id,
             pair_name=pair.name,
             fee_to=event.fee_to,
             market_order_owner=event.taker,
             fee=fee,
-            fee_asset=asset_symbol
+            fee_asset=asset_symbol,
         )
 
     def __repr__(self):
         items = ("{}={!r}".format(k, self.__dict__[k]) for k in self.__dict__)
         return "{}({})".format(type(self).__name__, ", ".join(items))
```

### Comparing `rubi-2.1.1/rubi/rubicon_types/order_query.py` & `rubi-2.1.2/rubi/rubicon_types/order_query.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,69 +12,61 @@
 )
 from rubi.network import (
     Network,
 )
 
 
 class OrderQuery:
-
     def __init__(
         self,
         subgrounds: Subgrounds,
         subgraph,  # TODO: determine the type that should be used here
         network: Optional[Network] = None,
-        network_tokens: Optional[Dict[ChecksumAddress, ERC20]] = None
+        network_tokens: Optional[Dict[ChecksumAddress, ERC20]] = None,
     ):
-
         self.sg = subgrounds
         self.data = subgraph
         self.network = network
         self.tokens = network_tokens
         self.offer = self.offer_entity()
 
     # TODO: we will want to move this somewhere else most likely - we can't access the client from here though so we
     #  will need to figure out how to do that
     #####################################
     # General Helper Methods
     #####################################
 
-    def get_token(
-        self,
-        token_address: str
-    ) -> ERC20:
+    def get_token(self, token_address: str) -> ERC20:
         """Returns an ERC20 object for the token address passed from the token_map if it exists or add it to the
         self.tokens if it does not exist.
         """
 
         if not self.tokens:
             raise ValueError("No network object initialized on the class.")
         else:
-
             try:
                 token_address = self.network.w3.to_checksum_address(token_address)
 
                 if token_address not in self.tokens:
                     self.tokens[token_address] = ERC20.from_address(
-                        w3=self.network.w3,
-                        address=token_address
+                        w3=self.network.w3, address=token_address
                     )
 
                 return self.tokens[token_address]
 
             except:
                 raise ValueError(f"Token address: {token_address} is invalid.")
 
     #####################################
     # Query Methods                     #
     #####################################
 
     def offer_entity(
         self,
     ):  # TODO: return a typed object (see subgrounds documentation for more info)
-
         Offer = self.data.Offer
 
         # if we have a network object we can get all the token information we need
         if self.network:
             Offer.pay_amt_formatted = SyntheticField(
                 f=lambda pay_amt, pay_gem: self.get_token(pay_gem).to_decimal(pay_amt),
                 type_=SyntheticField.FLOAT,
@@ -84,21 +76,25 @@
             Offer.buy_amt_formatted = SyntheticField(
                 f=lambda buy_amt, buy_gem: self.get_token(buy_gem).to_decimal(buy_amt),
                 type_=SyntheticField.FLOAT,
                 deps=[Offer.buy_amt, Offer.buy_gem],
             )
 
             Offer.paid_amt_formatted = SyntheticField(
-                f=lambda paid_amt, pay_gem: self.get_token(pay_gem).to_decimal(paid_amt),
+                f=lambda paid_amt, pay_gem: self.get_token(pay_gem).to_decimal(
+                    paid_amt
+                ),
                 type_=SyntheticField.FLOAT,
                 deps=[Offer.paid_amt, Offer.pay_gem],
             )
 
             Offer.bought_amt_formatted = SyntheticField(
-                f=lambda bought_amt, buy_gem: self.get_token(buy_gem).to_decimal(bought_amt),
+                f=lambda bought_amt, buy_gem: self.get_token(buy_gem).to_decimal(
+                    bought_amt
+                ),
                 type_=SyntheticField.FLOAT,
                 deps=[Offer.bought_amt, Offer.buy_gem],
             )
 
             Offer.pay_gem_symbol = SyntheticField(
                 f=lambda pay_gem: self.get_token(pay_gem).symbol,
                 type_=SyntheticField.STRING,
@@ -127,72 +123,76 @@
         maker: Optional[str] = None,
         from_address: Optional[str] = None,
         pay_gem: Optional[str] = None,
         buy_gem: Optional[str] = None,
         open: Optional[bool] = None,
         start_time: Optional[int] = None,
         end_time: Optional[int] = None,
-        # TODO: there is definitely a clear way to pass these parameters in a more concise way, prolly **kargs   
+        # TODO: there is definitely a clear way to pass these parameters in a more concise way, prolly **kargs
     ):  # TODO: return a typed object (see subgrounds documentation for more info)
-
         # determine that the parameters are valid
         error_messages = []
 
         # check the order_by parameter
-        if order_by.lower() not in ('timestamp', 'price'):
-            error_messages.append("Invalid order_by, must be 'timestamp' or 'price' (default: timestamp)")
-        elif order_by.lower() == 'timestamp':
+        if order_by.lower() not in ("timestamp", "price"):
+            error_messages.append(
+                "Invalid order_by, must be 'timestamp' or 'price' (default: timestamp)"
+            )
+        elif order_by.lower() == "timestamp":
             order_by = self.offer.timestamp
-        elif order_by.lower() == 'price':
+        elif order_by.lower() == "price":
             order_by = self.offer.price
 
         # check the order_direction parameter
-        if order_direction.lower() not in ('asc', 'desc'):
-            error_messages.append("Invalid order_direction, must be 'asc' or 'desc' (default: desc)")
+        if order_direction.lower() not in ("asc", "desc"):
+            error_messages.append(
+                "Invalid order_direction, must be 'asc' or 'desc' (default: desc)"
+            )
         else:
             order_direction = order_direction.lower()
 
         # check the first parameter
         if first < 1:
-            error_messages.append("Invalid first, must be greater than 0 (default: 1000)")
+            error_messages.append(
+                "Invalid first, must be greater than 0 (default: 1000)"
+            )
         if not isinstance(first, int):
             error_messages.append("Invalid first, must be an integer (default: 1000)")
 
         # raise an error if there are any
         if error_messages:
-            raise ValueError('\n'.join(error_messages))
+            raise ValueError("\n".join(error_messages))
 
         # build the list of where conditions
         where = [
             self.offer.maker == maker.lower() if maker else None,
             self.offer.from_address == from_address.lower() if from_address else None,
             self.offer.pay_gem == pay_gem.lower() if pay_gem else None,
             self.offer.buy_gem == buy_gem.lower() if buy_gem else None,
             self.offer.open == open if open is not None else None,
             self.offer.timestamp >= start_time if start_time else None,
-            self.offer.timestamp <= end_time if end_time else None
+            self.offer.timestamp <= end_time if end_time else None,
         ]
         where = [condition for condition in where if condition is not None]
 
         """Helper method to build a query for the offers subgraph entity."""
         offers = self.data.Query.offers(
             orderBy=order_by,
             orderDirection=order_direction,
             first=first,
-            where=where if where else {}
+            where=where if where else {},
         )
 
         return offers
 
     def offers_fields(
         self,
         offers: Any,  # TODO: check that this is the correct type (subgrounds may have types that we can utilize here)
-        formatted: bool = False
+        formatted: bool = False,
     ):  # TODO: return a typed object (see subgrounds documentation for more info)
-
         """Helper method to build a list of fields for the offers subgraph entity."""
         fields = [
             offers.id,
             offers.timestamp,
             offers.index,
             offers.maker.id,
             offers.from_address.id,
@@ -204,15 +204,15 @@
             offers.bought_amt,
             offers.price,
             offers.open,
             offers.removed_timestamp,
             offers.removed_block,
             offers.transaction.id,
             offers.transaction.block_number,
-            offers.transaction.block_index
+            offers.transaction.block_index,
         ]
 
         if formatted:
             fields.append(offers.pay_amt_formatted)
             fields.append(offers.buy_amt_formatted)
             fields.append(offers.paid_amt_formatted)
             fields.append(offers.bought_amt_formatted)
@@ -225,48 +225,91 @@
     def query_offers(
         self,
         fields: List,
         formatted: bool = False,
         # TOOD: maybe we give the user the option to define a custom pagination strategy?
     ):  # TODO: return a typed object (see subgrounds documentation for more info)
         """Helper method to query the offers subgraph entity."""
-        df = self.sg.query_df(
-            fields,
-            pagination_strategy=ShallowStrategy
-        )
+        df = self.sg.query_df(fields, pagination_strategy=ShallowStrategy)
 
         # if the dataframe is empty, return an empty dataframe with the correct columns
         if df.empty and not formatted:
-            cols = ['id', 'timestamp', 'index', 'maker', 'from_address', 'pay_gem',
-                    'buy_gem', 'pay_amt', 'buy_amt', 'paid_amt', 'bought_amt', 'price',
-                    'open', 'removed_timestamp', 'removed_block', 'transaction',
-                    'transaction_block_number', 'transaction_block_index']
+            cols = [
+                "id",
+                "timestamp",
+                "index",
+                "maker",
+                "from_address",
+                "pay_gem",
+                "buy_gem",
+                "pay_amt",
+                "buy_amt",
+                "paid_amt",
+                "bought_amt",
+                "price",
+                "open",
+                "removed_timestamp",
+                "removed_block",
+                "transaction",
+                "transaction_block_number",
+                "transaction_block_index",
+            ]
             df = pd.DataFrame(columns=cols)
 
         elif df.empty and formatted:
-            cols = ['id', 'maker', 'from_address', 'pay_gem', 'buy_gem', 'pay_amt', 'buy_amt', 'paid_amt', 'bought_amt']
+            cols = [
+                "id",
+                "maker",
+                "from_address",
+                "pay_gem",
+                "buy_gem",
+                "pay_amt",
+                "buy_amt",
+                "paid_amt",
+                "bought_amt",
+            ]
             df = pd.DataFrame(columns=cols)
 
         else:
-            df.columns = [col.replace('offers_', '') for col in df.columns]
-            df.columns = [col.replace('_id', '') for col in df.columns]
+            df.columns = [col.replace("offers_", "") for col in df.columns]
+            df.columns = [col.replace("_id", "") for col in df.columns]
 
             # convert the id to an integer
             # TODO: i don't love the lambda (cc pickling, but it appears we are forced to use them in sythetic fields
             #  regardless)
-            df['id'] = df['id'].apply(lambda x: int(x, 16))
+            df["id"] = df["id"].apply(lambda x: int(x, 16))
 
             # TODO: decide whether we should return the unformatted fields or not
             if formatted:
                 df = df.drop(
-                    columns=['pay_amt', 'buy_amt', 'paid_amt', 'bought_amt', 'pay_gem', 'buy_gem', 'timestamp', 'index',
-                             'price', 'removed_timestamp', 'removed_block', 'transaction_block_number',
-                             'transaction_block_index'])
-                df = df.rename(columns={'pay_amt_formatted': 'pay_amt', 'buy_amt_formatted': 'buy_amt',
-                                        'paid_amt_formatted': 'paid_amt', 'bought_amt_formatted': 'bought_amt',
-                                        'pay_gem_symbol': 'pay_gem', 'buy_gem_symbol': 'buy_gem',
-                                        'datetime': 'timestamp'})
+                    columns=[
+                        "pay_amt",
+                        "buy_amt",
+                        "paid_amt",
+                        "bought_amt",
+                        "pay_gem",
+                        "buy_gem",
+                        "timestamp",
+                        "index",
+                        "price",
+                        "removed_timestamp",
+                        "removed_block",
+                        "transaction_block_number",
+                        "transaction_block_index",
+                    ]
+                )
+                df = df.rename(
+                    columns={
+                        "pay_amt_formatted": "pay_amt",
+                        "buy_amt_formatted": "buy_amt",
+                        "paid_amt_formatted": "paid_amt",
+                        "bought_amt_formatted": "bought_amt",
+                        "pay_gem_symbol": "pay_gem",
+                        "buy_gem_symbol": "buy_gem",
+                        "datetime": "timestamp",
+                    }
+                )
                 # TODO: we could also get smart with displaying price dependent upon the pair_name and direction of the
                 #  order
 
-        # TODO: apply any data type conversions to the dataframe - possibly converting unformatted values to integers   
+        # TODO: apply any data type conversions to the dataframe - possibly converting unformatted values to integers
         return df
```

### Comparing `rubi-2.1.1/rubi/rubicon_types/orderbook.py` & `rubi-2.1.2/rubi/rubicon_types/orderbook.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,15 @@
 
     :param price: The price of the level.
     :type price: Decimal
     :param size: The size of the level.
     :type size: Decimal
     """
 
-    def __init__(
-        self,
-        price: Decimal,
-        size: Decimal
-    ):
+    def __init__(self, price: Decimal, size: Decimal):
         """constructor method."""
         self.price = price
         self.size = size
 
     def __repr__(self):
         items = ("{}={!r}".format(k, self.__dict__[k]) for k in self.__dict__)
         return "{}({})".format(type(self).__name__, ", ".join(items))
@@ -33,19 +29,15 @@
 
     :param book_side: The side of the order book (BUY or SELL).
     :type book_side: OrderSide
     :param levels: The list of levels on the side.
     :type levels: List[BookLevel]
     """
 
-    def __init__(
-        self,
-        book_side: OrderSide,
-        levels: List[BookLevel]
-    ):
+    def __init__(self, book_side: OrderSide, levels: List[BookLevel]):
         """constructor method."""
         self.book_side = book_side
         self.levels = levels
 
     def best_price(self) -> Decimal:
         """Returns the price of the best level on the book side.
 
@@ -65,15 +57,15 @@
 
     @classmethod
     def from_rubicon_offers(
         cls,
         book_side: OrderSide,
         offers: List[List[int]],
         base_asset: ERC20,
-        quote_asset: ERC20
+        quote_asset: ERC20,
     ) -> "BookSide":
         """Creates a BookSide instance from a list of Rubicon offers.
 
         :param book_side: The side of the order book (BUY or SELL).
         :type book_side: OrderSide
         :param offers: The list of offers retrieved from the Rubicon for an asset pair pay_gem/buy_gem.
         :type offers: List[List[int]]
@@ -102,18 +94,15 @@
                     price = quote_asset.to_decimal(order[0]) / size
 
                     if levels and levels[-1].price == price:
                         levels[-1].size += size
                     else:
                         levels.append(BookLevel(price=price, size=size))
 
-        return cls(
-            book_side=book_side,
-            levels=levels
-        )
+        return cls(book_side=book_side, levels=levels)
 
     def __repr__(self):
         items = ("{}={!r}".format(k, self.__dict__[k]) for k in self.__dict__)
         return "{}({})".format(type(self).__name__, ", ".join(items))
 
 
 class OrderBook:
@@ -131,15 +120,15 @@
         self.asks = asks
 
     @classmethod
     def from_rubicon_offer_book(
         cls,
         offer_book: Tuple[List[List[int]], List[List[int]]],
         base_asset: ERC20,
-        quote_asset: ERC20
+        quote_asset: ERC20,
     ) -> "OrderBook":
         """Create an OrderBook from Rubicon offer book.
 
         :param offer_book: Rubicon offer book containing bid and ask offers.
         :type offer_book: Tuple[List[List[int]], List[List[int]]]
         :param base_asset: An ERC20 instance representing the base asset.
         :type base_asset: ERC20
@@ -149,22 +138,22 @@
         :rtype: OrderBook
         """
         return cls(
             bids=BookSide.from_rubicon_offers(
                 book_side=OrderSide.BUY,  # Corresponds to BIDS
                 offers=offer_book[1],
                 base_asset=base_asset,
-                quote_asset=quote_asset
+                quote_asset=quote_asset,
             ),
             asks=BookSide.from_rubicon_offers(
                 book_side=OrderSide.SELL,  # Corresponds to ASKS
                 offers=offer_book[0],
                 base_asset=base_asset,
-                quote_asset=quote_asset
-            )
+                quote_asset=quote_asset,
+            ),
         )
 
     def best_bid(self) -> Decimal:
         """Get the best bid price from the order book.
 
         :return: Best bid price.
         :rtype: Decimal
@@ -196,8 +185,9 @@
 
         return self.best_ask() - self.best_bid()
 
     def __repr__(self):
         items = ("{}={!r}".format(k, self.__dict__[k]) for k in self.__dict__)
         return "{}({})".format(type(self).__name__, ", ".join(items))
 
+
 # TODO: add a DetailedOrderBook class that contains the full order book composed of LimitOrder instances
```

### Comparing `rubi-2.1.1/rubi/rubicon_types/pair.py` & `rubi-2.1.2/rubi/rubicon_types/pair.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,28 +22,28 @@
 
     def __init__(
         self,
         name: str,
         base_asset: ERC20,
         quote_asset: ERC20,
         current_base_asset_allowance: Optional[Decimal],
-        current_quote_asset_allowance: Optional[Decimal]
+        current_quote_asset_allowance: Optional[Decimal],
     ):
         self.name = name
 
         self.base_asset: ERC20 = base_asset
         self.quote_asset: ERC20 = quote_asset
 
         self.bid_identifier: str = base_asset.w3.solidity_keccak(
             abi_types=["address", "address"],
-            values=[self.quote_asset.address, self.base_asset.address]
+            values=[self.quote_asset.address, self.base_asset.address],
         ).hex()
         self.ask_identifier: str = base_asset.w3.solidity_keccak(
             abi_types=["address", "address"],
-            values=[self.base_asset.address, self.quote_asset.address]
+            values=[self.base_asset.address, self.quote_asset.address],
         ).hex()
 
         # TODO: think about structure of allowances on this class. Currently, this only caters for the RubiconMarket
         #  contract.
         self.current_base_asset_allowance = current_base_asset_allowance
         self.current_quote_asset_allowance = current_quote_asset_allowance
```

### Comparing `rubi-2.1.1/PKG-INFO` & `rubi-2.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: rubi
-Version: 2.1.1
+Version: 2.1.2
 Summary: A python SDK for the Rubicon Protocol
 Author: denver
 Author-email: denver@rubicon.finance
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
 Requires-Dist: attributedict (==0.3.0)
+Requires-Dist: black (>=23.3.0,<24.0.0)
 Requires-Dist: eth-abi (==4.0.0)
 Requires-Dist: eth-tester (==0.9.0b1)
 Requires-Dist: eth-utils (==2.1.0)
 Requires-Dist: hexbytes (==0.3.0)
 Requires-Dist: py-evm (==0.7.0a2)
 Requires-Dist: pytest (==7.3.1)
 Requires-Dist: python-semantic-release (==7.34.3)
```

