# Comparing `tmp/chainbench-0.3.2.tar.gz` & `tmp/chainbench-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainbench-0.3.2.tar", max compression
+gzip compressed data, was "chainbench-0.4.0.tar", max compression
```

## Comparing `chainbench-0.3.2.tar` & `chainbench-0.4.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0    11357 2023-07-11 08:05:25.229816 chainbench-0.3.2/LICENSE
--rw-r--r--   0        0        0     8428 2023-07-11 08:05:25.229816 chainbench-0.3.2/README.md
--rw-r--r--   0        0        0        0 2023-07-11 08:05:25.229816 chainbench-0.3.2/chainbench/__init__.py
--rw-r--r--   0        0        0       39 2023-07-11 08:05:25.229816 chainbench-0.3.2/chainbench/__main__.py
--rw-r--r--   0        0        0     8401 2023-07-11 08:05:25.229816 chainbench-0.3.2/chainbench/main.py
--rw-r--r--   0        0        0        0 2023-07-11 08:05:25.229816 chainbench-0.3.2/chainbench/profile/__init__.py
--rw-r--r--   0        0        0     3597 2023-07-11 08:05:25.229816 chainbench-0.3.2/chainbench/profile/avalanche/general.py
--rw-r--r--   0        0        0     2693 2023-07-11 08:05:25.229816 chainbench-0.3.2/chainbench/profile/bsc/general.py
--rw-r--r--   0        0        0     2912 2023-07-11 08:05:25.229816 chainbench-0.3.2/chainbench/profile/ethereum/general.py
--rw-r--r--   0        0        0      361 2023-07-11 08:05:25.229816 chainbench-0.3.2/chainbench/profile/evm/get_logs.py
--rw-r--r--   0        0        0     4158 2023-07-11 08:05:25.233816 chainbench-0.3.2/chainbench/profile/evm/heavy.py
--rw-r--r--   0        0        0     1645 2023-07-11 08:05:25.233816 chainbench-0.3.2/chainbench/profile/evm/light.py
--rw-r--r--   0        0        0     1838 2023-07-11 08:05:25.233816 chainbench-0.3.2/chainbench/profile/oasis/general.py
--rw-r--r--   0        0        0     2845 2023-07-11 08:05:25.233816 chainbench-0.3.2/chainbench/profile/polygon/general.py
--rw-r--r--   0        0        0      168 2023-07-11 08:05:25.233816 chainbench-0.3.2/chainbench/test_data/__init__.py
--rw-r--r--   0        0        0     4705 2023-07-11 08:05:25.233816 chainbench-0.3.2/chainbench/test_data/base.py
--rw-r--r--   0        0        0      166 2023-07-11 08:05:25.233816 chainbench-0.3.2/chainbench/test_data/dummy.py
--rw-r--r--   0        0        0     2979 2023-07-11 08:05:25.233816 chainbench-0.3.2/chainbench/test_data/evm.py
--rw-r--r--   0        0        0        0 2023-07-11 08:05:25.233816 chainbench-0.3.2/chainbench/user/__init__.py
--rw-r--r--   0        0        0     3511 2023-07-11 08:05:25.233816 chainbench-0.3.2/chainbench/user/base.py
--rw-r--r--   0        0        0     2740 2023-07-11 08:05:25.233816 chainbench-0.3.2/chainbench/user/evm.py
--rw-r--r--   0        0        0        0 2023-07-11 08:05:25.233816 chainbench-0.3.2/chainbench/util/__init__.py
--rw-r--r--   0        0        0     3907 2023-07-11 08:05:25.233816 chainbench-0.3.2/chainbench/util/cli.py
--rw-r--r--   0        0        0     2511 2023-07-11 08:05:25.233816 chainbench-0.3.2/chainbench/util/event.py
--rw-r--r--   0        0        0     3436 2023-07-11 08:05:25.233816 chainbench-0.3.2/chainbench/util/monitor.py
--rw-r--r--   0        0        0     3463 2023-07-11 08:05:25.233816 chainbench-0.3.2/chainbench/util/notify.py
--rw-r--r--   0        0        0      279 2023-07-11 08:05:25.233816 chainbench-0.3.2/chainbench/util/rpc.py
--rw-r--r--   0        0        0      438 2023-07-11 08:05:25.233816 chainbench-0.3.2/chainbench/util/timer.py
--rw-r--r--   0        0        0      895 2023-07-11 08:05:25.233816 chainbench-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     9033 1970-01-01 00:00:00.000000 chainbench-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-14 03:10:04.505115 chainbench-0.4.0/LICENSE
+-rw-r--r--   0        0        0     8428 2023-07-14 03:10:04.505115 chainbench-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/__init__.py
+-rw-r--r--   0        0        0       39 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/__main__.py
+-rw-r--r--   0        0        0     8455 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/main.py
+-rw-r--r--   0        0        0        0 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/profile/__init__.py
+-rw-r--r--   0        0        0     3681 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/profile/avalanche/general.py
+-rw-r--r--   0        0        0     2777 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/profile/bsc/general.py
+-rw-r--r--   0        0        0     2987 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/profile/ethereum/general.py
+-rw-r--r--   0        0        0      410 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/profile/evm/get_logs.py
+-rw-r--r--   0        0        0     4234 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/profile/evm/heavy.py
+-rw-r--r--   0        0        0     1711 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/profile/evm/light.py
+-rw-r--r--   0        0        0     1922 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/profile/oasis/general.py
+-rw-r--r--   0        0        0     2919 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/profile/polygon/general.py
+-rw-r--r--   0        0        0      168 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/test_data/__init__.py
+-rw-r--r--   0        0        0     5356 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/test_data/base.py
+-rw-r--r--   0        0        0      166 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/test_data/dummy.py
+-rw-r--r--   0        0        0     3497 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/test_data/evm.py
+-rw-r--r--   0        0        0        0 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/user/__init__.py
+-rw-r--r--   0        0        0     3837 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/user/base.py
+-rw-r--r--   0        0        0     2873 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/user/evm.py
+-rw-r--r--   0        0        0        0 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/util/__init__.py
+-rw-r--r--   0        0        0     3907 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/util/cli.py
+-rw-r--r--   0        0        0     2511 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/util/event.py
+-rw-r--r--   0        0        0     3436 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/util/monitor.py
+-rw-r--r--   0        0        0     3463 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/util/notify.py
+-rw-r--r--   0        0        0      863 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/util/rng.py
+-rw-r--r--   0        0        0      279 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/util/rpc.py
+-rw-r--r--   0        0        0      438 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/util/timer.py
+-rw-r--r--   0        0        0      895 2023-07-14 03:10:04.505115 chainbench-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     9033 1970-01-01 00:00:00.000000 chainbench-0.4.0/PKG-INFO
```

### Comparing `chainbench-0.3.2/LICENSE` & `chainbench-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chainbench-0.3.2/README.md` & `chainbench-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `chainbench-0.3.2/chainbench/main.py` & `chainbench-0.4.0/chainbench/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 @click.group(
     help="Tool for flexible blockchain infrastructure benchmarking.",
 )
+@click.version_option(message="%(prog)s-%(version)s")
 @click.pass_context
 def cli(ctx: click.Context):
     ctx.obj = ContextData()
 
 
 @cli.command(
     help="Start the test using the configured profile. "
```

### Comparing `chainbench-0.3.2/chainbench/profile/avalanche/general.py` & `chainbench-0.4.0/chainbench/profile/avalanche/general.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     "eth_getBalance" : 11
     "Others" : 28
 ```
 """
 from locust import constant_pacing, tag, task
 
 from chainbench.user.evm import EVMBenchUser
+from chainbench.util.rng import get_rng
 
 
 class AvalancheProfile(EVMBenchUser):
     wait_time = constant_pacing(2)
     weight = 91
 
     @task(100)
@@ -39,23 +40,23 @@
         ),
 
     @task(50)
     def get_block_by_number_task(self):
         self.make_call(
             name="get_block_by_number",
             method="eth_getBlockByNumber",
-            params=self._block_by_number_params_factory(),
+            params=self._block_params_factory(get_rng()),
         ),
 
     @task(17)
     def get_transaction_receipt_task(self):
         self.make_call(
             name="get_transaction_receipt",
             method="eth_getTransactionReceipt",
-            params=self._transaction_by_hash_params_factory(),
+            params=self._transaction_by_hash_params_factory(get_rng()),
         ),
 
     @task(15)
     def chain_id_task(self):
         self.make_call(
             name="chain_id",
             method="eth_chainId",
@@ -69,23 +70,23 @@
         ),
 
     @task(11)
     def get_balance_task(self):
         self.make_call(
             name="get_balance",
             method="eth_getBalance",
-            params=self._get_balance_params_factory_latest(),
+            params=self._get_balance_params_factory_latest(get_rng()),
         ),
 
     @task(10)
     def get_transaction_by_hash_task(self):
         self.make_call(
             name="get_transaction_by_hash",
             method="eth_getTransactionByHash",
-            params=self._transaction_by_hash_params_factory(),
+            params=self._transaction_by_hash_params_factory(get_rng()),
         ),
 
     @task(5)
     def estimate_gas_task(self):
         self.make_call(
             name="estimate_gas",
             method="eth_estimateGas",
@@ -106,15 +107,15 @@
         ),
 
     @task(3)
     def get_block_by_hash_task(self):
         self.make_call(
             name="get_block_by_hash",
             method="eth_getBlockByHash",
-            params=self._block_by_hash_params_factory(),
+            params=self._block_by_hash_params_factory(get_rng()),
         ),
 
     @task(3)
     def gas_price_task(self):
         self.make_call(
             name="gas_price",
             method="eth_gasPrice",
@@ -134,9 +135,9 @@
 
     @tag("get-logs")
     @task
     def get_logs_task(self):
         self.make_call(
             name="get_logs",
             method="eth_getLogs",
-            params=self._get_logs_params_factory(),
+            params=self._get_logs_params_factory(get_rng()),
         ),
```

### Comparing `chainbench-0.3.2/chainbench/profile/bsc/general.py` & `chainbench-0.4.0/chainbench/profile/bsc/general.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     "eth_getBlockByNumber" : 13
     "Others" : 20
 ```
 """
 from locust import constant_pacing, tag, task
 
 from chainbench.user.evm import EVMBenchUser
+from chainbench.util.rng import get_rng
 
 
 class BscProfile(EVMBenchUser):
     wait_time = constant_pacing(2)
     weight = 89
 
     @task(100)
@@ -38,15 +39,15 @@
         ),
 
     @task(93)
     def get_transaction_receipt_task(self):
         self.make_call(
             name="get_transaction_receipt",
             method="eth_getTransactionReceipt",
-            params=self._transaction_by_hash_params_factory(),
+            params=self._transaction_by_hash_params_factory(get_rng()),
         ),
 
     @task(28)
     def block_number_task(self):
         self.make_call(
             name="block_number",
             method="eth_blockNumber",
@@ -62,47 +63,47 @@
         ),
 
     @task(13)
     def get_block_by_number_task(self):
         self.make_call(
             name="get_block_by_number",
             method="eth_getBlockByNumber",
-            params=self._block_by_number_params_factory(),
+            params=self._block_params_factory(get_rng()),
         ),
 
     @task(9)
     def get_transaction_by_hash_task(self):
         self.make_call(
             name="get_transaction_by_hash",
             method="eth_getTransactionByHash",
-            params=self._transaction_by_hash_params_factory(),
+            params=self._transaction_by_hash_params_factory(get_rng()),
         ),
 
     @task(5)
     def get_balance_task(self):
         self.make_call(
             name="get_balance",
             method="eth_getBalance",
-            params=self._get_balance_params_factory_latest(),
+            params=self._get_balance_params_factory_latest(get_rng()),
         ),
 
     @task(3)
     def get_block_by_hash_task(self):
         self.make_call(
             name="get_block_by_hash",
             method="eth_getBlockByHash",
-            params=self._block_by_hash_params_factory(),
+            params=self._block_by_hash_params_factory(get_rng()),
         ),
 
 
 class GetLogsProfile(EVMBenchUser):
     wait_time = constant_pacing(10)
     weight = 12
 
     @tag("get-logs")
     @task
     def get_logs_task(self):
         self.make_call(
             name="get_logs",
             method="eth_getLogs",
-            params=self._get_logs_params_factory(),
+            params=self._get_logs_params_factory(get_rng()),
         ),
```

### Comparing `chainbench-0.3.2/chainbench/profile/ethereum/general.py` & `chainbench-0.4.0/chainbench/profile/ethereum/general.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     "eth_getTransactionByHash" : 8
     "Others" : 12
 ```
 """
 from locust import constant_pacing, tag, task
 
 from chainbench.user.evm import EVMBenchUser
+from chainbench.util.rng import get_rng
 
 
 class EthereumProfile(EVMBenchUser):
     wait_time = constant_pacing(2)
     weight = 487
 
     @task(100)
@@ -39,15 +40,15 @@
         ),
 
     @task(24)
     def get_transaction_receipt_task(self):
         self.make_call(
             name="get_transaction_receipt",
             method="eth_getTransactionReceipt",
-            params=self._transaction_by_hash_params_factory(),
+            params=self._transaction_by_hash_params_factory(get_rng()),
         ),
 
     @task(19)
     def block_number_task(self):
         self.make_call(
             name="block_number",
             method="eth_blockNumber",
@@ -55,15 +56,15 @@
         ),
 
     @task(12)
     def get_balance_task(self):
         self.make_call(
             name="get_balance",
             method="eth_getBalance",
-            params=self._get_balance_params_factory_latest(),
+            params=self._get_balance_params_factory_latest(get_rng()),
         ),
 
     @task(11)
     def chain_id_task(self):
         self.make_call(
             name="chain_id",
             method="eth_chainId",
@@ -71,23 +72,23 @@
         ),
 
     @task(9)
     def get_block_by_number_task(self):
         self.make_call(
             name="get_block_by_number",
             method="eth_getBlockByNumber",
-            params=self._block_by_number_params_factory(),
+            params=self._block_params_factory(get_rng()),
         ),
 
     @task(8)
     def get_transaction_by_hash_task(self):
         self.make_call(
             name="get_transaction_by_hash",
             method="eth_getTransactionByHash",
-            params=self._transaction_by_hash_params_factory(),
+            params=self._transaction_by_hash_params_factory(get_rng()),
         ),
 
     @tag("debug")
     @task(3)
     def trace_transaction_task(self):
         self.make_call(
             name="trace_transaction",
@@ -110,9 +111,9 @@
 
     @tag("get-logs")
     @task
     def get_logs_task(self):
         self.make_call(
             name="get_logs",
             method="eth_getLogs",
-            params=self._get_logs_params_factory(),
+            params=self._get_logs_params_factory(get_rng()),
         ),
```

### Comparing `chainbench-0.3.2/chainbench/profile/evm/light.py` & `chainbench-0.4.0/chainbench/profile/oasis/general.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,66 +1,70 @@
-"""
-Ethereum profile (light mode).
-"""
 from locust import constant_pacing, task
 
 from chainbench.user.evm import EVMBenchUser
+from chainbench.util.rng import get_rng
 
 
-class EthereumLightProfile(EVMBenchUser):
+class OasisProfile(EVMBenchUser):
     wait_time = constant_pacing(2)
 
     @task
-    def get_transaction_receipt_task(self):
-        self.make_call(
-            name="get_transaction_receipt",
-            method="eth_getTransactionReceipt",
-            params=self._transaction_by_hash_params_factory(),
-        ),
-
-    @task
-    def block_number_task(self):
+    def get_block_by_number_task(self):
         self.make_call(
-            name="block_number",
-            method="eth_blockNumber",
-            params=[],
+            name="get_block_by_number",
+            method="eth_getBlockByNumber",
+            params=self._block_params_factory(get_rng()),
         ),
 
     @task
     def get_balance_task(self):
         self.make_call(
             name="get_balance",
             method="eth_getBalance",
-            params=self._get_balance_params_factory_latest(),
+            params=self._get_balance_params_factory(get_rng()),
         ),
 
     @task
-    def chain_id_task(self):
+    def get_transaction_count_task(self):
         self.make_call(
-            name="chain_id",
-            method="eth_chainId",
-            params=[],
+            name="get_transaction_count",
+            method="eth_getTransactionCount",
+            params=self._get_balance_params_factory(get_rng()),
         ),
 
     @task
-    def get_block_by_number_task(self):
+    def get_code_task(self):
         self.make_call(
-            name="get_block_by_number",
-            method="eth_getBlockByNumber",
-            params=self._block_by_number_params_factory(),
+            name="get_code",
+            method="eth_getCode",
+            params=self._get_balance_params_factory(get_rng()),
         ),
 
     @task
     def get_transaction_by_hash_task(self):
         self.make_call(
             name="get_transaction_by_hash",
             method="eth_getTransactionByHash",
-            params=self._transaction_by_hash_params_factory(),
+            params=self._transaction_by_hash_params_factory(get_rng()),
+        ),
+
+    @task
+    def get_block_number_task(self):
+        self.make_call(
+            name="block_number",
+            method="eth_blockNumber",
+        ),
+
+    @task
+    def get_syncing_task(self):
+        self.make_call(
+            name="get_syncing",
+            method="eth_syncing",
         ),
 
     @task
-    def client_version_task(self):
+    def get_block_transaction_count_by_number_task(self):
         self.make_call(
-            name="client_version",
-            method="web3_clientVersion",
-            params=[],
+            name="get_block_transaction_count_by_number",
+            method="eth_getBlockTransactionCountByNumber",
+            params=self._random_block_number_params_factory(get_rng()),
         ),
```

### Comparing `chainbench-0.3.2/chainbench/profile/oasis/general.py` & `chainbench-0.4.0/chainbench/profile/evm/light.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,67 @@
+"""
+Ethereum profile (light mode).
+"""
 from locust import constant_pacing, task
 
 from chainbench.user.evm import EVMBenchUser
+from chainbench.util.rng import get_rng
 
 
-class OasisProfile(EVMBenchUser):
+class EthereumLightProfile(EVMBenchUser):
     wait_time = constant_pacing(2)
 
     @task
-    def get_block_by_number_task(self):
+    def get_transaction_receipt_task(self):
         self.make_call(
-            name="get_block_by_number",
-            method="eth_getBlockByNumber",
-            params=self._block_by_number_params_factory(),
+            name="get_transaction_receipt",
+            method="eth_getTransactionReceipt",
+            params=self._transaction_by_hash_params_factory(get_rng()),
+        ),
+
+    @task
+    def block_number_task(self):
+        self.make_call(
+            name="block_number",
+            method="eth_blockNumber",
+            params=[],
         ),
 
     @task
     def get_balance_task(self):
         self.make_call(
             name="get_balance",
             method="eth_getBalance",
-            params=self._get_balance_params_factory(),
+            params=self._get_balance_params_factory_latest(get_rng()),
         ),
 
     @task
-    def get_transaction_count_task(self):
+    def chain_id_task(self):
         self.make_call(
-            name="get_transaction_count",
-            method="eth_getTransactionCount",
-            params=self._get_balance_params_factory(),
+            name="chain_id",
+            method="eth_chainId",
+            params=[],
         ),
 
     @task
-    def get_code_task(self):
+    def get_block_by_number_task(self):
         self.make_call(
-            name="get_code",
-            method="eth_getCode",
-            params=self._get_balance_params_factory(),
+            name="get_block_by_number",
+            method="eth_getBlockByNumber",
+            params=self._block_params_factory(get_rng()),
         ),
 
     @task
     def get_transaction_by_hash_task(self):
         self.make_call(
             name="get_transaction_by_hash",
             method="eth_getTransactionByHash",
-            params=self._transaction_by_hash_params_factory(),
-        ),
-
-    @task
-    def get_block_number_task(self):
-        self.make_call(
-            name="block_number",
-            method="eth_blockNumber",
-        ),
-
-    @task
-    def get_syncing_task(self):
-        self.make_call(
-            name="get_syncing",
-            method="eth_syncing",
+            params=self._transaction_by_hash_params_factory(get_rng()),
         ),
 
     @task
-    def get_block_transaction_count_by_number_task(self):
+    def client_version_task(self):
         self.make_call(
-            name="get_block_transaction_count_by_number",
-            method="eth_getBlockTransactionCountByNumber",
-            params=self._random_block_number_params_factory(),
+            name="client_version",
+            method="web3_clientVersion",
+            params=[],
         ),
```

### Comparing `chainbench-0.3.2/chainbench/profile/polygon/general.py` & `chainbench-0.4.0/chainbench/profile/polygon/general.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     "eth_getLogs" : 11
     "Others" : 9
 ```
 """
 from locust import constant_pacing, tag, task
 
 from chainbench.user.evm import EVMBenchUser
+from chainbench.util.rng import get_rng
 
 
 class PolygonGeneral(EVMBenchUser):
     wait_time = constant_pacing(2)
     weight = 19
 
     @task(100)
@@ -42,15 +43,15 @@
         ),
 
     @task(64)
     def get_transaction_receipt_task(self):
         self.make_call(
             name="get_transaction_receipt",
             method="eth_getTransactionReceipt",
-            params=self._transaction_by_hash_params_factory(),
+            params=self._transaction_by_hash_params_factory(get_rng()),
         ),
 
     @task(20)
     def chain_id_task(self):
         self.make_call(
             name="chain_id",
             method="eth_chainId",
@@ -58,15 +59,15 @@
         ),
 
     @task(17)
     def get_block_by_number_task(self):
         self.make_call(
             name="get_block_by_number",
             method="eth_getBlockByNumber",
-            params=self._block_by_number_params_factory(),
+            params=self._block_params_factory(get_rng()),
         ),
 
     @task(16)
     def block_number_task(self):
         self.make_call(
             name="block_number",
             method="eth_blockNumber",
@@ -74,40 +75,40 @@
         ),
 
     @task(11)
     def get_transaction_by_hash_task(self):
         self.make_call(
             name="get_transaction_by_hash",
             method="eth_getTransactionByHash",
-            params=self._transaction_by_hash_params_factory(),
+            params=self._transaction_by_hash_params_factory(get_rng()),
         ),
 
     @task(4)
     def get_balance_task(self):
         self.make_call(
             name="get_balance",
             method="eth_getBalance",
-            params=self._get_balance_params_factory_latest(),
+            params=self._get_balance_params_factory_latest(get_rng()),
         ),
 
     @tag("trace")
     @task(2)
     def block_task(self):
         self.make_call(
             name="block",
             method="trace_block",
-            params=self._block_by_number_params_factory(),
+            params=self._block_params_factory(get_rng()),
         ),
 
 
 class GetLogsProfile(EVMBenchUser):
     wait_time = constant_pacing(10)
     weight = 1
 
     @tag("get-logs")
     @task
     def get_logs_task(self):
         self.make_call(
             name="get_logs",
             method="eth_getLogs",
-            params=self._get_logs_params_factory(),
+            params=self._get_logs_params_factory(get_rng()),
         ),
```

### Comparing `chainbench-0.3.2/chainbench/test_data/base.py` & `chainbench-0.4.0/chainbench/test_data/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import logging
-import random
 import typing as t
 from dataclasses import dataclass, field
 from secrets import token_hex
 
 import httpx
 from gevent.lock import Semaphore as GeventSemaphore
 
+from chainbench.util.rng import RNG, get_rng
+
 Account = str
 Accounts = list[Account]
 TxHash = str
 TxHashes = list[TxHash]
 Tx = dict[str, t.Any]
 Txs = list[Tx]
 Block = dict[str, t.Any]
 BlockNumber = int
 BlockHash = str
 Blocks = list[tuple[BlockNumber, BlockHash]]
 
 
 @dataclass
 class BlockchainData:
-    first_block_number: BlockNumber = 0
-    latest_block: Block = field(default_factory=dict)
-    latest_block_number: BlockNumber = 0
+    start_block_number: BlockNumber = 0
+    end_block_number: BlockNumber = 0
     blocks: Blocks = field(default_factory=list)
     txs: Txs = field(default_factory=list)
     tx_hashes: TxHashes = field(default_factory=list)
     accounts: Accounts = field(default_factory=list)
 
 
 class BaseTestData:
@@ -126,38 +126,58 @@
 
     def close(self):
         self._client.close()
 
     def wait(self):
         self._lock.wait()
 
-    def get_random_block_number(self) -> BlockNumber:
-        return random.randint(self.first_block_number, self.latest_block_number)
-
-    def get_random_block_hash(self) -> BlockHash:
-        _, block_hash = random.choice(self.blocks)
+    @staticmethod
+    def get_random_bool(rng: RNG | None = None) -> bool:
+        if rng is None:
+            rng = get_rng()
+        return rng.random.choice([True, False])
+
+    def get_random_block_number(self, rng: RNG | None = None) -> BlockNumber:
+        if rng is None:
+            rng = get_rng()
+        return rng.random.randint(self.start_block_number, self.end_block_number)
+
+    def get_random_block_hash(self, rng: RNG | None = None) -> BlockHash:
+        if rng is None:
+            rng = get_rng()
+        _, block_hash = rng.random.choice(self.blocks)
         return block_hash
 
-    def get_random_tx_hash(self) -> TxHash:
-        return random.choice(self.tx_hashes)
-
-    def get_random_account(self) -> Account:
-        return random.choice(self.accounts)
+    def get_random_tx_hash(self, rng: RNG | None = None) -> TxHash:
+        if rng is None:
+            rng = get_rng()
+        return rng.random.choice(self.tx_hashes)
+
+    def get_random_recent_block_number(
+        self, n: int, rng: RNG | None = None
+    ) -> BlockNumber:
+        if rng is None:
+            rng = get_rng()
+        return rng.random.randint(
+            self.end_block_number - n,
+            self.end_block_number,
+        )
 
-    @property
-    def latest_block(self) -> Block:
-        return self.data.latest_block
+    def get_random_account(self, rng: RNG | None = None) -> Account:
+        if rng is None:
+            rng = get_rng()
+        return rng.random.choice(self.accounts)
 
     @property
-    def first_block_number(self) -> BlockNumber:
-        return self.data.first_block_number
+    def start_block_number(self) -> BlockNumber:
+        return self.data.start_block_number
 
     @property
-    def latest_block_number(self) -> BlockNumber:
-        return self.data.latest_block_number
+    def end_block_number(self) -> BlockNumber:
+        return self.data.end_block_number
 
     @property
     def txs(self) -> Txs:
         return self.data.txs
 
     @property
     def tx_hashes(self) -> TxHashes:
```

### Comparing `chainbench-0.3.2/chainbench/user/base.py` & `chainbench-0.4.0/chainbench/user/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from locust import FastHttpUser
 from locust.contrib.fasthttp import RestResponseContextManager
 from locust.exception import RescheduleTask
 
 from chainbench.test_data import BaseTestData, DummyTestData
 from chainbench.util.event import setup_event_listeners
+from chainbench.util.rng import RNGManager
 from chainbench.util.rpc import generate_request
 
 # importing plugins here as all profiles depend on it
 import locust_plugins  # isort: skip  # noqa
 
 
 setup_event_listeners()
@@ -27,14 +28,15 @@
     network_timeout = 360
 
     test_data: BaseTestData = DummyTestData()
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.logger = logging.getLogger(__name__)
+        self.rng = RNGManager()
 
     def on_start(self):
         self.test_data.wait()
 
     def on_stop(self):
         self.test_data.close()
 
@@ -46,51 +48,58 @@
         elif 500 <= response.status_code <= 599:
             self.logger.critical(
                 f"Got internal server error when requesting {response.url}"
             )
         elif 300 <= response.status_code <= 399:
             self.logger.critical(f"Redirect error: {response.url}")
 
-    def check_response(self, response: RestResponseContextManager):
+    def check_response(self, response: RestResponseContextManager, name: str):
         """Check the response for errors."""
         if response.status_code != 200:
             self.logger.info(f"Request failed with {response.status_code} code")
             self.logger.debug(
                 f"Request to {response.url} failed with {response.status_code} code: {response.text}"  # noqa: E501
             )
             self.check_fatal(response)
             response.failure(f"Request failed with {response.status_code} code")
             response.raise_for_status()
 
         if response.request:
             self.logger.debug(f"Request: {response.request.body}")
 
         if response.js is None:
-            self.logger.error(f"Response is not a JSON: {response.text}")
-            response.failure("Response is not a JSON")
+            self.logger.error(f"Response for {name}  is not a JSON: {response.text}")
+            response.failure(f"Response for {name}  is not a JSON")
             raise RescheduleTask()
 
         if "jsonrpc" not in response.js:
-            self.logger.error(f"Response is not a JSON-RPC: {response.text}")
-            response.failure("Response is not a JSON-RPC")
+            self.logger.error(f"Response for {name} is not a JSON-RPC: {response.text}")
+            response.failure(f"Response for {name} is not a JSON-RPC")
             raise RescheduleTask()
 
         if "error" in response.js:
-            self.logger.error(f"Response has a JSON-RPC error: {response.text}")
+            self.logger.error(
+                f"Response for {name} has a JSON-RPC error: {response.text}"
+            )
             if "code" in response.js["error"]:
                 response.failure(
-                    f"Response has a JSON-RPC error {response.js['error']['code']}"
+                    f"Response for {name} has a JSON-RPC error {response.js['error']['code']}"  # noqa: E501
                 )
                 raise RescheduleTask()
             response.failure("Unspecified JSON-RPC error")
             raise RescheduleTask()
 
         if not response.js.get("result"):
-            self.logger.error(f"No result in response: {response.text}")
+            self.logger.error(
+                f"Response for {name} call has no result: {response.text}"
+            )
 
-    def make_call(self, name: str, method: str, params: list[t.Any] | None = None):
+    def make_call(
+        self, method: str, params: list[t.Any] | None = None, name: str | None = None
+    ):
+        name = name if name else method
         return self._post(name, data=generate_request(method, params))
 
     def _post(self, name: str, data: t.Optional[dict] = None):
         """Make a JSON-RPC call."""
         with self.rest("POST", self.rpc_path, json=data, name=name) as response:
-            self.check_response(response)
+            self.check_response(response, name=name)
```

### Comparing `chainbench-0.3.2/chainbench/user/evm.py` & `chainbench-0.4.0/chainbench/user/evm.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,86 +1,86 @@
 import random
 
 from chainbench.test_data import EVMTestData
 from chainbench.user.base import BaseBenchUser
-
-
-def random_bool():
-    return random.choice([True, False])
+from chainbench.util.rng import RNG
 
 
 class EVMBenchUser(BaseBenchUser):
     abstract = True
     test_data = EVMTestData()
 
-    def _get_logs_params_factory(self):
+    def _get_logs_params_factory(self, rng: RNG):
         return [
             {
                 "fromBlock": hex(
-                    self.test_data.latest_block_number - random.randint(0, 20)
+                    self.test_data.get_random_recent_block_number(20, rng)
                 ),
-                "toBlock": hex(self.test_data.latest_block_number),
+                "toBlock": hex(self.test_data.end_block_number),
             }
         ]
 
-    def _transaction_by_hash_params_factory(self):
-        return [self.test_data.get_random_tx_hash()]
+    def _transaction_by_hash_params_factory(self, rng: RNG):
+        return [self.test_data.get_random_tx_hash(rng)]
 
-    def _random_block_number_params_factory(self):
-        return [self.test_data.get_random_block_number_hex()]
+    def _random_block_number_params_factory(self, rng: RNG):
+        return [hex(self.test_data.get_random_block_number(rng))]
 
-    def _block_by_number_params_factory(self):
-        return [self.test_data.get_random_block_number_hex(), random_bool()]
+    def _block_params_factory(self, rng: RNG):
+        return [hex(self.test_data.get_random_block_number(rng)), True]
 
-    def _block_by_hash_params_factory(self):
-        return [self.test_data.get_random_block_hash(), random_bool()]
+    def _block_by_hash_params_factory(self, rng: RNG):
+        return [self.test_data.get_random_block_hash(rng), True]
 
-    def _get_balance_params_factory_latest(self):
-        return [self.test_data.get_random_account(), "latest"]
+    def _get_balance_params_factory_latest(self, rng: RNG):
+        return [self.test_data.get_random_account(rng), "latest"]
 
-    def _get_balance_params_factory(self):
+    def _get_balance_params_factory(self, rng: RNG):
         return [
-            self.test_data.get_random_account(),
-            self.test_data.get_random_block_number_hex(),
+            self.test_data.get_random_account(rng),
+            hex(self.test_data.get_random_block_number(rng)),
         ]
 
-    def _trace_block_by_number_params_factory(self):
+    def _trace_block_by_number_params_factory(self, rng: RNG):
         return [
-            self.test_data.get_random_block_number_hex(),
+            hex(self.test_data.get_random_block_number(rng)),
             {"tracer": "callTracer"},
         ]
 
-    def _trace_block_by_hash_params_factory(self):
+    def _trace_block_by_hash_params_factory(self, rng: RNG):
         return [
-            self.test_data.get_random_block_hash(),
+            self.test_data.get_random_block_hash(rng),
             {"tracer": "callTracer"},
         ]
 
-    def _trace_replay_block_transaction_by_block_number_params_factory(self):
+    def _trace_replay_block_transaction_params_factory(self, rng: RNG):
         return [
-            self.test_data.get_random_block_number_hex(),
+            hex(self.test_data.get_random_block_number(rng)),
             ["vmTrace", "trace", "stateDiff"],
         ]
 
-    def _trace_replay_transaction_by_hash_params_factory(self):
-        return [self.test_data.get_random_tx_hash(), ["vmTrace", "trace", "stateDiff"]]
+    def _trace_replay_transaction_params_factory(self, rng: RNG):
+        return [
+            self.test_data.get_random_tx_hash(rng),
+            ["vmTrace", "trace", "stateDiff"],
+        ]
 
-    def _trace_transaction_by_hash_params_factory(self):
-        return [self.test_data.get_random_tx_hash(), {"tracer": "prestateTracer"}]
+    def _trace_transaction_params_factory(self, rng: RNG):
+        return [self.test_data.get_random_tx_hash(rng), {"tracer": "prestateTracer"}]
 
-    def _trace_filter_params_factory(self):
-        block_number = self.test_data.get_random_block_number()
+    def _trace_filter_params_factory(self, rng: RNG):
+        block_number = self.test_data.get_random_block_number(rng)
         return [
             {
-                "fromAddress": [self.test_data.get_random_account()],
+                "fromAddress": [self.test_data.get_random_account(rng)],
                 "fromBlock": hex(block_number),
                 "toBlock": hex(block_number + random.randint(0, 20)),
             }
         ]
 
-    def _eth_estimate_gas_params_factory(self):
+    def _eth_estimate_gas_params_factory(self, rng: RNG):
         return [
             {
-                "from": self.test_data.get_random_account(),
+                "from": self.test_data.get_random_account(rng),
                 "to": "0x18318221d811Da0fe45412394eAf2C42A10BC678",
             }
         ]
```

### Comparing `chainbench-0.3.2/chainbench/util/cli.py` & `chainbench-0.4.0/chainbench/util/cli.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.3.2/chainbench/util/event.py` & `chainbench-0.4.0/chainbench/util/event.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.3.2/chainbench/util/monitor.py` & `chainbench-0.4.0/chainbench/util/monitor.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.3.2/chainbench/util/notify.py` & `chainbench-0.4.0/chainbench/util/notify.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.3.2/pyproject.toml` & `chainbench-0.4.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chainbench"
-version = "0.3.2"
+version = "0.4.0"
 description = ""
 authors = [
     "Egor Molodik <egor.molodik@chainstack.com>",
     "Erwin Wee <erwin.wee@chainstack.com>"
 ]
 maintainers = ["Erwin Wee <erwin.wee@chainstack.com>"]
 readme = "README.md"
```

### Comparing `chainbench-0.3.2/PKG-INFO` & `chainbench-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainbench
-Version: 0.3.2
+Version: 0.4.0
 Summary: 
 Author: Egor Molodik
 Author-email: egor.molodik@chainstack.com
 Maintainer: Erwin Wee
 Maintainer-email: erwin.wee@chainstack.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
```

