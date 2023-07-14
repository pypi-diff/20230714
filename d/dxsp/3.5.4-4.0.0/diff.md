# Comparing `tmp/dxsp-3.5.4.tar.gz` & `tmp/dxsp-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-3.5.4.tar", max compression
+gzip compressed data, was "dxsp-4.0.0.tar", max compression
```

## Comparing `dxsp-3.5.4.tar` & `dxsp-4.0.0.tar`

### file list

```diff
@@ -1,12 +1,17 @@
--rw-r--r--   0        0        0     1064 2023-07-12 17:44:08.491625 dxsp-3.5.4/LICENSE
--rw-r--r--   0        0        0     2697 2023-07-12 17:44:08.491625 dxsp-3.5.4/README.md
--rw-r--r--   0        0        0      115 2023-07-12 17:44:09.419632 dxsp-3.5.4/dxsp/__init__.py
--rw-r--r--   0        0        0      417 2023-07-12 17:44:08.491625 dxsp-3.5.4/dxsp/config.py
--rw-r--r--   0        0        0    10713 2023-07-12 17:44:08.491625 dxsp-3.5.4/dxsp/default_settings.toml
--rw-r--r--   0        0        0    17573 2023-07-12 17:44:08.491625 dxsp-3.5.4/dxsp/main.py
--rw-r--r--   0        0        0      103 2023-07-12 17:44:08.491625 dxsp-3.5.4/dxsp/protocols/__init__.py
--rw-r--r--   0        0        0     3536 2023-07-12 17:44:08.491625 dxsp-3.5.4/dxsp/protocols/oneinch.py
--rw-r--r--   0        0        0     1773 2023-07-12 17:44:08.491625 dxsp-3.5.4/dxsp/protocols/uniswap.py
--rw-r--r--   0        0        0      990 2023-07-12 17:44:08.491625 dxsp-3.5.4/dxsp/protocols/zerox.py
--rw-r--r--   0        0        0     2328 2023-07-12 17:44:09.419632 dxsp-3.5.4/pyproject.toml
--rw-r--r--   0        0        0     3546 1970-01-01 00:00:00.000000 dxsp-3.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-14 20:53:25.789043 dxsp-4.0.0/LICENSE
+-rw-r--r--   0        0        0     2697 2023-07-14 20:53:25.789043 dxsp-4.0.0/README.md
+-rw-r--r--   0        0        0      115 2023-07-14 20:53:26.693052 dxsp-4.0.0/dxsp/__init__.py
+-rw-r--r--   0        0        0      417 2023-07-14 20:53:25.789043 dxsp-4.0.0/dxsp/config.py
+-rw-r--r--   0        0        0    10529 2023-07-14 20:53:25.789043 dxsp-4.0.0/dxsp/default_settings.toml
+-rw-r--r--   0        0        0     5622 2023-07-14 20:53:25.789043 dxsp-4.0.0/dxsp/main.py
+-rw-r--r--   0        0        0      103 2023-07-14 20:53:25.789043 dxsp-4.0.0/dxsp/protocols/__init__.py
+-rw-r--r--   0        0        0     3536 2023-07-14 20:53:25.789043 dxsp-4.0.0/dxsp/protocols/oneinch.py
+-rw-r--r--   0        0        0     1835 2023-07-14 20:53:25.789043 dxsp-4.0.0/dxsp/protocols/uniswap.py
+-rw-r--r--   0        0        0     1036 2023-07-14 20:53:25.789043 dxsp-4.0.0/dxsp/protocols/zerox.py
+-rw-r--r--   0        0        0      102 2023-07-14 20:53:25.789043 dxsp-4.0.0/dxsp/utils/__init__.py
+-rw-r--r--   0        0        0     4636 2023-07-14 20:53:25.789043 dxsp-4.0.0/dxsp/utils/account_utils.py
+-rw-r--r--   0        0        0     6590 2023-07-14 20:53:25.789043 dxsp-4.0.0/dxsp/utils/contract_utils.py
+-rw-r--r--   0        0        0     1989 2023-07-14 20:53:25.789043 dxsp-4.0.0/dxsp/utils/explorer_utils.py
+-rw-r--r--   0        0        0      363 2023-07-14 20:53:25.789043 dxsp-4.0.0/dxsp/utils/utils.py
+-rw-r--r--   0        0        0     2328 2023-07-14 20:53:26.693052 dxsp-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3546 1970-01-01 00:00:00.000000 dxsp-4.0.0/PKG-INFO
```

### Comparing `dxsp-3.5.4/LICENSE` & `dxsp-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-3.5.4/README.md` & `dxsp-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-3.5.4/dxsp/default_settings.toml` & `dxsp-4.0.0/dxsp/default_settings.toml`

 * *Files 15% similar despite different names*

```diff
@@ -15,25 +15,25 @@
 dex_erc20_abi_url = "https://raw.githubusercontent.com/Uniswap/interface/44c355c7f0f8ab5bdb3e0790560e84e59f5666f7/src/abis/erc20.json"
 dex_block_explorer_url = "https://api.etherscan.io/api?"
 dex_block_explorer_api =  "798437294880920392"
 headers = {User-Agent= 'Mozilla/5.0'}
 token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
 token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
 token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
-trading_asset = "USDT"
 trading_asset_address = "0xdAC17F958D2ee523a2206206994597C13D831ec7"
 trading_risk_amount = 10 # 10% of the position
 dex_trading_slippage = 2 # 2% slippage
 dex_notify_invalid_token = true
 
 
 
 
 
 
+
 ##############
 ## SETTINGS ##
 ## FOR TEST ##
 ##############
 [uniswap]
 VALUE = "On Testing"
 dxsp_enabled = true
@@ -43,15 +43,14 @@
 dex_protocol_type = "uniswap"
 dex_protocol_version = 2
 dex_rpc = "https://rpc.ankr.com/eth"
 dex_router_contract_addr = "0x7a250d5630B4cF539739dF2C5dAcb4c659F2488D"
 dex_factory_contract_addr = "0x5C69bEe701ef814a2B6a3EDD4B1652CB9cc5aA6f"
 dex_router_abi_url = "https://raw.githubusercontent.com/uniswap-python/uniswap-python/master/uniswap/assets/uniswap-v2/router02.abi"
 dex_erc20_abi_url = "https://raw.githubusercontent.com/Uniswap/interface/44c355c7f0f8ab5bdb3e0790560e84e59f5666f7/src/abis/erc20.json"
-trading_asset = "USDT"
 trading_asset_address = "0xdAC17F958D2ee523a2206206994597C13D831ec7"
 trading_risk_amount = 10 
 dex_trading_slippage = 2
 dex_notify_invalid_token = true
 headers = {User-Agent= 'Mozilla/5.0'}
 token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
 token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
@@ -67,15 +66,14 @@
 dex_protocol_version = 2
 dex_rpc = "https://rpc.ankr.com/eth"
 dex_0x_url = "https://api.0x.org/"
 dex_router_contract_addr = "0xdef1c0ded9bec7f1a1670819833240f027b25eff"
 dex_factory_contract_addr = ""
 dex_router_abi_url = "https://raw.githubusercontent.com/0xProject/protocol/development/packages/contract-artifacts/artifacts/Exchange.json"
 dex_erc20_abi_url = "https://raw.githubusercontent.com/Uniswap/interface/44c355c7f0f8ab5bdb3e0790560e84e59f5666f7/src/abis/erc20.json"
-trading_asset = "USDT"
 trading_asset_address = "0xdAC17F958D2ee523a2206206994597C13D831ec7"
 trading_risk_amount = 10
 dex_trading_slippage = 2
 dex_notify_invalid_token = true
 headers = {User-Agent= 'Mozilla/5.0'}
 token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
 token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
@@ -90,15 +88,14 @@
 dex_protocol_type = "uniswap"
 dex_protocol_version = 2
 dex_rpc = "https://rpc.ankr.com/eth_goerli"
 dex_router_contract_addr = "0x7a250d5630B4cF539739dF2C5dAcb4c659F2488D"
 dex_factory_contract_addr = "0x5C69bEe701ef814a2B6a3EDD4B1652CB9cc5aA6f"
 dex_router_abi_url = "https://raw.githubusercontent.com/uniswap-python/uniswap-python/master/uniswap/assets/uniswap-v2/router02.abi"
 dex_erc20_abi_url = "https://raw.githubusercontent.com/Uniswap/interface/44c355c7f0f8ab5bdb3e0790560e84e59f5666f7/src/abis/erc20.json"
-trading_asset = "USDC"
 trading_asset_address = "0xa3726f2e6423caF1824cD7721B543B29b621fB4f"
 trading_risk_amount = 10
 dex_trading_slippage = 2
 dex_notify_invalid_token = true
 headers = {User-Agent= 'Mozilla/5.0'}
 token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
 token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
@@ -110,38 +107,36 @@
 dex_wallet_address = "0xf977814e90da44bfa03b6295a0616a897441acec"
 dex_private_key = "0xdeadbeet45ab87712ad64ccb3b10217737f7faacbf2872e88fdd9a537d8fe266" 
 dex_protocol_type = "uniswap"
 dex_protocol_version = 2
 dex_rpc = "https://rpc.ankr.com/bsc"
 dex_router_contract_addr = "0x10ED43C718714eb63d5aA57B78B54704E256024E"
 dex_factory_contract_addr = "0xcA143Ce32Fe78f1f7019d7d551a6402fC5350c73"
-trading_asset = "BUSD"
 trading_asset_address = "0xe9e7cea3dedca5984780bafc599bd69add087d56"
 trading_risk_amount = 10 
 dex_trading_slippage = 2
 dex_notify_invalid_token = false
 headers = {User-Agent= 'Mozilla/5.0'}
 token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
 token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
 token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
 
-[uniswap3]
+[uniswapv3]
 VALUE = "On uniswap3"
 dxsp_enabled = true
 loglevel = "DEBUG"
 dex_wallet_address = "0x1a9C8182C09F50C8318d769245beA52c32BE35BC" 
 dex_private_key = "0xdeadbeet45ab87712ad64ccb3b10217737f7faacbf2872e88fdd9a537d8fe266" 
 dex_protocol_type = "uniswap"
 dex_protocol_version = 3
 dex_rpc = "https://rpc.ankr.com/eth"
 dex_router_contract_addr = "0x1F98431c8aD98523631AE4a59f267346ea31F984"
 dex_factory_contract_addr = "0x68b3465833fb72A70ecDF485E0e4C7bD8665Fc45"
 dex_router_abi_url = "https://raw.githubusercontent.com/uniswap-python/uniswap-python/master/uniswap/assets/uniswap-v2/router02.abi"
 dex_erc20_abi_url = "https://raw.githubusercontent.com/Uniswap/interface/44c355c7f0f8ab5bdb3e0790560e84e59f5666f7/src/abis/erc20.json"
-trading_asset = "USDT"
 trading_asset_address = "0xdAC17F958D2ee523a2206206994597C13D831ec7"
 trading_risk_amount = 10 
 dex_trading_slippage = 2
 dex_notify_invalid_token = true
 headers = {User-Agent= 'Mozilla/5.0'}
 token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
 token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
@@ -156,15 +151,14 @@
 dex_protocol_type = "uniswap"
 dex_protocol_version = 3
 dex_rpc = "https://rpc.ankr.com/bsc"
 dex_router_contract_addr = "0x1F98431c8aD98523631AE4a59f267346ea31F984"
 dex_factory_contract_addr = "0x13f4EA83D0bd40E75C8222255bc855a974568Dd4"
 dex_router_abi_url = "https://raw.githubusercontent.com/uniswap-python/uniswap-python/master/uniswap/assets/uniswap-v2/router02.abi"
 dex_erc20_abi_url = "https://raw.githubusercontent.com/Uniswap/interface/44c355c7f0f8ab5bdb3e0790560e84e59f5666f7/src/abis/erc20.json"
-trading_asset = "BUSD"
 trading_asset_address = "0xe9e7cea3dedca5984780bafc599bd69add087d56"
 trading_risk_amount = 10 
 dex_trading_slippage = 2
 dex_notify_invalid_token = true
 headers = {User-Agent= 'Mozilla/5.0'}
 token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
 token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
@@ -176,15 +170,14 @@
 # VALUE = "1inchtesting"
 # loglevel = "DEBUG"
 # dxsp_enabled = true
 # headers = {User-Agent= 'Mozilla/5.0'}
 # token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
 # token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
 # token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
-# trading_asset = "USDT"
 # trading_asset_address = "0xdAC17F958D2ee523a2206206994597C13D831ec7"
 # trading_risk_amount = 10 # 10% of the position
 # dex_trading_slippage = 2 # 2 % slippage
 # dex_wallet_address = "0x1a9C8182C09F50C8318d769245beA52c32BE35BC" 
 # dex_private_key = "0xdeadbeet45ab87712ad64ccb3b10217737f7faacbf2872e88fdd9a537d8fe266" 
 # dex_chain_id = 1
 # dex_rpc = "https://rpc.ankr.com/eth"
```

### Comparing `dxsp-3.5.4/dxsp/protocols/oneinch.py` & `dxsp-4.0.0/dxsp/protocols/oneinch.py`

 * *Files identical despite different names*

### Comparing `dxsp-3.5.4/dxsp/protocols/uniswap.py` & `dxsp-4.0.0/dxsp/protocols/uniswap.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,37 +15,37 @@
         self,
         buy_address,
         sell_address,
         amount=1
     ):
         try:
             uniswap = Uniswap(
-                address=self.wallet_address,
-                private_key=self.private_key,
+                address=self.account.wallet_address,
+                private_key=self.account.private_key,
                 version=self.protocol_version, web3=self.w3,
                 factory_contract_addr=settings.dex_factory_contract_addr,
                 router_contract_addr=settings.dex_router_contract_addr
                 )
             amount_wei = amount * (10 ** (
-                await self.get_token_decimals(sell_address)))
+                await self.contract_utils.get_token_decimals(sell_address)))
             quote = uniswap.get_price_input(
                 sell_address, buy_address, amount_wei)
             return round(
                 float((quote /
                        (10 **
-                        (await self.get_token_decimals(buy_address))))), 5)
+                        (await self.contract_utils.get_token_decimals(buy_address))))), 5)
 
         except Exception as error:
             raise ValueError(f"Quote failed {error}") 
 
     async def get_swap(self, sell_address, buy_address, amount):
         try:
             uniswap = Uniswap(
-                        address=self.wallet_address,
-                        private_key=self.private_key,
+                        address=self.account.wallet_address,
+                        private_key=self.account.private_key,
                         version=2, web3=self.w3,
                         factory_contract_addr=settings.dex_factory_contract_addr,
                         router_contract_addr=settings.dex_router_contract_addr
                         )
             return uniswap.make_trade(
                 sell_address, buy_address, amount)
```

### Comparing `dxsp-3.5.4/dxsp/protocols/zerox.py` & `dxsp-4.0.0/dxsp/protocols/zerox.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """
 0️⃣x
 """
 from dxsp.config import settings
 from dxsp.main import DexSwap
+from dxsp.utils.utils import get
 
 class DexSwapZeroX(DexSwap):
+
     async def get_quote(self, buy_address, sell_address, amount=1):
         try:
-            out_amount = amount * (10 ** await self.get_token_decimals(sell_address)) ##1000000000
-            url = f"{settings.dex_0x_url}/swap/v1/quote?buyToken={str(buy_address)}&sellToken={str(sell_address)}&sellAmount={str(out_amount)}"
+            token_decimals = await self.contract_utils.get_token_decimals(sell_address)
+            out_amount = amount * (10 ** token_decimals)
+            url = (f"{settings.dex_0x_url}/swap/v1/quote"
+                f"?buyToken={str(buy_address)}&sellToken={str(sell_address)}&sellAmount={str(out_amount)}")
             headers = {"0x-api-key": settings.dex_0x_api_key}
-            response = await self.get(url, params=None, headers=headers)
+            response = await get(url, params=None, headers=headers)
             if response:
-                quote = float(response['guaranteedPrice'])
-                print(quote)
-                return quote
+                return float(response['guaranteedPrice'])
         except Exception as error:
             raise ValueError(f"Quote failed {error}") 
 
     async def get_swap(self, buy_address, sell_address, amount):
         swap_order = await self.get_quote(buy_address, sell_address, amount)
-        return await self.get_sign(swap_order)
+        return await self.account.get_sign(swap_order)
```

### Comparing `dxsp-3.5.4/pyproject.toml` & `dxsp-4.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dxsp"
-version = "3.5.4"
+version = "4.0.0"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [
     {include = "dxsp"}
 ]
```

### Comparing `dxsp-3.5.4/PKG-INFO` & `dxsp-4.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 3.5.4
+Version: 4.0.0
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dxsp Version: 3.5.4 Summary: DXSP (DeX SwaP), A
+Metadata-Version: 2.1 Name: dxsp Version: 4.0.0 Summary: DXSP (DeX SwaP), A
 defi swap helper package. Swap made easy. License: MIT Author: mraniki Author-
 email: 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
 (>=3.1.12,<4.0.0) Requires-Dist: pycoingecko (>=3.1.0,<4.0.0) Requires-Dist:
 uniswap-python (>=0.7.0,<0.8.0) Requires-Dist: web3 (>=6.4.0,<7.0.0) Project-
```

