# Comparing `tmp/empiric_network-1.6.0.tar.gz` & `tmp/empiric_network-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "empiric_network-1.6.0.tar", max compression
+gzip compressed data, was "empiric_network-1.6.1.tar", max compression
```

## Comparing `empiric_network-1.6.0.tar` & `empiric_network-1.6.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      284 2023-06-07 10:39:12.630562 empiric_network-1.6.0/README.md
--rw-r--r--   0        0        0        0 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/__init__.py
--rw-r--r--   0        0        0      193 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/__init__.py
--rw-r--r--   0        0        0      284 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/abis/__init__.py
--rw-r--r--   0        0        0    14135 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/abis/oracle.py
--rw-r--r--   0        0        0     1436 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/abis/proxy.py
--rw-r--r--   0        0        0     3896 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/abis/publisher_registry.py
--rw-r--r--   0        0        0     5912 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/abis/randomness.py
--rw-r--r--   0        0        0      868 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/abis/summary_stats.py
--rw-r--r--   0        0        0     4232 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/client.py
--rw-r--r--   0        0        0     1461 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/config.py
--rw-r--r--   0        0        0     3801 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/contract.py
--rw-r--r--   0        0        0     9972 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/entry.py
--rw-r--r--   0        0        0      387 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/logger.py
--rw-r--r--   0        0        0      295 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/mixins/__init__.py
--rw-r--r--   0        0        0    25441 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/mixins/evm.py
--rw-r--r--   0        0        0     3074 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/mixins/nonce.py
--rw-r--r--   0        0        0     8808 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/mixins/oracle.py
--rw-r--r--   0        0        0     2287 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/mixins/publisher_registry.py
--rw-r--r--   0        0        0     3065 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/mixins/randomness.py
--rw-r--r--   0        0        0      669 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/mixins/transactions.py
--rw-r--r--   0        0        0     3886 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/types.py
--rw-r--r--   0        0        0      880 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/core/utils.py
--rw-r--r--   0        0        0       82 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/publisher/__init__.py
--rw-r--r--   0        0        0     2716 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/publisher/assets.py
--rw-r--r--   0        0        0     2261 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/publisher/client.py
--rw-r--r--   0        0        0      354 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/publisher/fetchers/__init__.py
--rw-r--r--   0        0        0     3755 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/publisher/fetchers/ascendex.py
--rw-r--r--   0        0        0     3017 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/publisher/fetchers/bitstamp.py
--rw-r--r--   0        0        0     3380 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/publisher/fetchers/cex.py
--rw-r--r--   0        0        0     2953 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/publisher/fetchers/coinbase.py
--rw-r--r--   0        0        0     3980 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/publisher/fetchers/coingecko.py
--rw-r--r--   0        0        0     3826 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/publisher/fetchers/defillama.py
--rw-r--r--   0        0        0     3814 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/publisher/fetchers/gemini.py
--rw-r--r--   0        0        0     3754 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/publisher/fetchers/kaiko.py
--rw-r--r--   0        0        0     3631 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/publisher/fetchers/okx.py
--rw-r--r--   0        0        0     3762 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/publisher/fetchers/thegraph.py
--rw-r--r--   0        0        0      668 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/publisher/types.py
--rw-r--r--   0        0        0        0 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/test/__init__.py
--rw-r--r--   0        0        0     5965 2023-06-07 10:39:12.630562 empiric_network-1.6.0/empiric/test/interface_consistency.py
--rw-r--r--   0        0        0     1016 2023-06-07 10:39:12.630562 empiric_network-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     1038 1970-01-01 00:00:00.000000 empiric_network-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0      284 2023-07-14 14:50:09.205585 empiric_network-1.6.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-14 14:50:09.205585 empiric_network-1.6.1/empiric/__init__.py
+-rw-r--r--   0        0        0      193 2023-07-14 14:50:09.205585 empiric_network-1.6.1/empiric/core/__init__.py
+-rw-r--r--   0        0        0      284 2023-07-14 14:50:09.205585 empiric_network-1.6.1/empiric/core/abis/__init__.py
+-rw-r--r--   0        0        0    14135 2023-07-14 14:50:09.205585 empiric_network-1.6.1/empiric/core/abis/oracle.py
+-rw-r--r--   0        0        0     1436 2023-07-14 14:50:09.205585 empiric_network-1.6.1/empiric/core/abis/proxy.py
+-rw-r--r--   0        0        0     3896 2023-07-14 14:50:09.205585 empiric_network-1.6.1/empiric/core/abis/publisher_registry.py
+-rw-r--r--   0        0        0     5912 2023-07-14 14:50:09.205585 empiric_network-1.6.1/empiric/core/abis/randomness.py
+-rw-r--r--   0        0        0      868 2023-07-14 14:50:09.205585 empiric_network-1.6.1/empiric/core/abis/summary_stats.py
+-rw-r--r--   0        0        0     4232 2023-07-14 14:50:09.205585 empiric_network-1.6.1/empiric/core/client.py
+-rw-r--r--   0        0        0     1461 2023-07-14 14:50:09.205585 empiric_network-1.6.1/empiric/core/config.py
+-rw-r--r--   0        0        0     3801 2023-07-14 14:50:09.205585 empiric_network-1.6.1/empiric/core/contract.py
+-rw-r--r--   0        0        0     9972 2023-07-14 14:50:09.205585 empiric_network-1.6.1/empiric/core/entry.py
+-rw-r--r--   0        0        0      387 2023-07-14 14:50:09.205585 empiric_network-1.6.1/empiric/core/logger.py
+-rw-r--r--   0        0        0      295 2023-07-14 14:50:09.205585 empiric_network-1.6.1/empiric/core/mixins/__init__.py
+-rw-r--r--   0        0        0    25441 2023-07-14 14:50:09.205585 empiric_network-1.6.1/empiric/core/mixins/evm.py
+-rw-r--r--   0        0        0     3074 2023-07-14 14:50:09.205585 empiric_network-1.6.1/empiric/core/mixins/nonce.py
+-rw-r--r--   0        0        0     8808 2023-07-14 14:50:09.205585 empiric_network-1.6.1/empiric/core/mixins/oracle.py
+-rw-r--r--   0        0        0     2287 2023-07-14 14:50:09.205585 empiric_network-1.6.1/empiric/core/mixins/publisher_registry.py
+-rw-r--r--   0        0        0     3065 2023-07-14 14:50:09.205585 empiric_network-1.6.1/empiric/core/mixins/randomness.py
+-rw-r--r--   0        0        0      669 2023-07-14 14:50:09.205585 empiric_network-1.6.1/empiric/core/mixins/transactions.py
+-rw-r--r--   0        0        0     3896 2023-07-14 14:50:09.205585 empiric_network-1.6.1/empiric/core/types.py
+-rw-r--r--   0        0        0      880 2023-07-14 14:50:09.205585 empiric_network-1.6.1/empiric/core/utils.py
+-rw-r--r--   0        0        0       82 2023-07-14 14:50:09.205585 empiric_network-1.6.1/empiric/publisher/__init__.py
+-rw-r--r--   0        0        0     2716 2023-07-14 14:50:09.205585 empiric_network-1.6.1/empiric/publisher/assets.py
+-rw-r--r--   0        0        0     2261 2023-07-14 14:50:09.205585 empiric_network-1.6.1/empiric/publisher/client.py
+-rw-r--r--   0        0        0      354 2023-07-14 14:50:09.205585 empiric_network-1.6.1/empiric/publisher/fetchers/__init__.py
+-rw-r--r--   0        0        0     3755 2023-07-14 14:50:09.205585 empiric_network-1.6.1/empiric/publisher/fetchers/ascendex.py
+-rw-r--r--   0        0        0     3017 2023-07-14 14:50:09.205585 empiric_network-1.6.1/empiric/publisher/fetchers/bitstamp.py
+-rw-r--r--   0        0        0     3380 2023-07-14 14:50:09.205585 empiric_network-1.6.1/empiric/publisher/fetchers/cex.py
+-rw-r--r--   0        0        0     2953 2023-07-14 14:50:09.205585 empiric_network-1.6.1/empiric/publisher/fetchers/coinbase.py
+-rw-r--r--   0        0        0     3980 2023-07-14 14:50:09.205585 empiric_network-1.6.1/empiric/publisher/fetchers/coingecko.py
+-rw-r--r--   0        0        0     3826 2023-07-14 14:50:09.205585 empiric_network-1.6.1/empiric/publisher/fetchers/defillama.py
+-rw-r--r--   0        0        0     3814 2023-07-14 14:50:09.205585 empiric_network-1.6.1/empiric/publisher/fetchers/gemini.py
+-rw-r--r--   0        0        0     3754 2023-07-14 14:50:09.205585 empiric_network-1.6.1/empiric/publisher/fetchers/kaiko.py
+-rw-r--r--   0        0        0     3631 2023-07-14 14:50:09.205585 empiric_network-1.6.1/empiric/publisher/fetchers/okx.py
+-rw-r--r--   0        0        0     3762 2023-07-14 14:50:09.205585 empiric_network-1.6.1/empiric/publisher/fetchers/thegraph.py
+-rw-r--r--   0        0        0      668 2023-07-14 14:50:09.205585 empiric_network-1.6.1/empiric/publisher/types.py
+-rw-r--r--   0        0        0        0 2023-07-14 14:50:09.205585 empiric_network-1.6.1/empiric/test/__init__.py
+-rw-r--r--   0        0        0     5965 2023-07-14 14:50:09.205585 empiric_network-1.6.1/empiric/test/interface_consistency.py
+-rw-r--r--   0        0        0     1016 2023-07-14 14:50:09.205585 empiric_network-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1038 1970-01-01 00:00:00.000000 empiric_network-1.6.1/PKG-INFO
```

### Comparing `empiric_network-1.6.0/empiric/core/abis/oracle.py` & `empiric_network-1.6.1/empiric/core/abis/oracle.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.0/empiric/core/abis/proxy.py` & `empiric_network-1.6.1/empiric/core/abis/proxy.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.0/empiric/core/abis/publisher_registry.py` & `empiric_network-1.6.1/empiric/core/abis/publisher_registry.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.0/empiric/core/abis/randomness.py` & `empiric_network-1.6.1/empiric/core/abis/randomness.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.0/empiric/core/abis/summary_stats.py` & `empiric_network-1.6.1/empiric/core/abis/summary_stats.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.0/empiric/core/client.py` & `empiric_network-1.6.1/empiric/core/client.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.0/empiric/core/config.py` & `empiric_network-1.6.1/empiric/core/config.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.0/empiric/core/contract.py` & `empiric_network-1.6.1/empiric/core/contract.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.0/empiric/core/entry.py` & `empiric_network-1.6.1/empiric/core/entry.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.0/empiric/core/mixins/evm.py` & `empiric_network-1.6.1/empiric/core/mixins/evm.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.0/empiric/core/mixins/nonce.py` & `empiric_network-1.6.1/empiric/core/mixins/nonce.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.0/empiric/core/mixins/oracle.py` & `empiric_network-1.6.1/empiric/core/mixins/oracle.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.0/empiric/core/mixins/publisher_registry.py` & `empiric_network-1.6.1/empiric/core/mixins/publisher_registry.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.0/empiric/core/mixins/randomness.py` & `empiric_network-1.6.1/empiric/core/mixins/randomness.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.0/empiric/core/mixins/transactions.py` & `empiric_network-1.6.1/empiric/core/mixins/transactions.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.0/empiric/core/types.py` & `empiric_network-1.6.1/empiric/core/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from enum import IntEnum, unique
 from typing import List, Literal
 
 from empiric.core.utils import str_to_felt
 from starknet_py.net.full_node_client import FullNodeClient
 
 ADDRESS = int
```

### Comparing `empiric_network-1.6.0/empiric/core/utils.py` & `empiric_network-1.6.1/empiric/core/utils.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.0/empiric/publisher/assets.py` & `empiric_network-1.6.1/empiric/publisher/assets.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.0/empiric/publisher/client.py` & `empiric_network-1.6.1/empiric/publisher/client.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.0/empiric/publisher/fetchers/ascendex.py` & `empiric_network-1.6.1/empiric/publisher/fetchers/ascendex.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.0/empiric/publisher/fetchers/bitstamp.py` & `empiric_network-1.6.1/empiric/publisher/fetchers/bitstamp.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.0/empiric/publisher/fetchers/cex.py` & `empiric_network-1.6.1/empiric/publisher/fetchers/cex.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.0/empiric/publisher/fetchers/coinbase.py` & `empiric_network-1.6.1/empiric/publisher/fetchers/coinbase.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.0/empiric/publisher/fetchers/coingecko.py` & `empiric_network-1.6.1/empiric/publisher/fetchers/coingecko.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.0/empiric/publisher/fetchers/defillama.py` & `empiric_network-1.6.1/empiric/publisher/fetchers/defillama.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.0/empiric/publisher/fetchers/gemini.py` & `empiric_network-1.6.1/empiric/publisher/fetchers/gemini.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.0/empiric/publisher/fetchers/kaiko.py` & `empiric_network-1.6.1/empiric/publisher/fetchers/kaiko.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.0/empiric/publisher/fetchers/okx.py` & `empiric_network-1.6.1/empiric/publisher/fetchers/okx.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.0/empiric/publisher/fetchers/thegraph.py` & `empiric_network-1.6.1/empiric/publisher/fetchers/thegraph.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.0/empiric/publisher/types.py` & `empiric_network-1.6.1/empiric/publisher/types.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.0/empiric/test/interface_consistency.py` & `empiric_network-1.6.1/empiric/test/interface_consistency.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.0/pyproject.toml` & `empiric_network-1.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
 
 [tool.poetry]
 name = "empiric-network"
-version = "1.6.0"
+version = "1.6.1"
 authors = ["Pragma <contact@pragmaoracle.com>"]
 description = "Core package for rollup-native Pragma Oracle"
 readme = "README.md"
 homepage = "https://pragmaoracle.com"
 repository = "https://github.com/Astraly-Labs/Pragma"
 documentation = "https://docs.pragmaoracle.com"
 classifiers = [
```

### Comparing `empiric_network-1.6.0/PKG-INFO` & `empiric_network-1.6.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: empiric-network
-Version: 1.6.0
+Version: 1.6.1
 Summary: Core package for rollup-native Pragma Oracle
 Home-page: https://pragmaoracle.com
 Author: Pragma
 Author-email: contact@pragmaoracle.com
 Requires-Python: >=3.9,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

