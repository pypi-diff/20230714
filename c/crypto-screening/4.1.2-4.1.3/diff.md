# Comparing `tmp/crypto-screening-4.1.2.tar.gz` & `tmp/crypto-screening-4.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-4.1.2.tar", last modified: Fri Jul 14 12:28:44 2023, max compression
+gzip compressed data, was "crypto-screening-4.1.3.tar", last modified: Fri Jul 14 15:41:41 2023, max compression
```

## Comparing `crypto-screening-4.1.2.tar` & `crypto-screening-4.1.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 12:28:44.882823 crypto-screening-4.1.2/
--rw-rw-rw-   0        0        0       98 2023-07-14 12:28:44.000000 crypto-screening-4.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-14 12:28:44.882823 crypto-screening-4.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-4.1.2/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-4.1.2/build.py
-drwxrwxrwx   0        0        0        0 2023-07-14 12:28:44.860957 crypto-screening-4.1.2/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-14 12:28:44.874108 crypto-screening-4.1.2/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-4.1.2/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-4.1.2/crypto_screening/collect/exchanges.py
--rw-rw-rw-   0        0        0    45525 2023-07-14 09:02:59.000000 crypto-screening-4.1.2/crypto_screening/collect/market.py
--rw-rw-rw-   0        0        0    21191 2023-07-13 17:18:17.000000 crypto-screening-4.1.2/crypto_screening/collect/ohlcv.py
--rw-rw-rw-   0        0        0    19312 2023-07-13 17:18:17.000000 crypto-screening-4.1.2/crypto_screening/collect/orderbook.py
--rw-rw-rw-   0        0        0    18206 2023-07-14 12:25:47.000000 crypto-screening-4.1.2/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    18977 2023-07-14 12:28:29.000000 crypto-screening-4.1.2/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    14087 2023-07-14 07:29:46.000000 crypto-screening-4.1.2/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-4.1.2/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-4.1.2/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-14 12:28:44.876145 crypto-screening-4.1.2/crypto_screening/market/
--rw-rw-rw-   0        0        0    10937 2023-07-13 18:50:12.000000 crypto-screening-4.1.2/crypto_screening/market/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-07-14 12:28:44.877804 crypto-screening-4.1.2/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-4.1.2/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-4.1.2/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-4.1.2/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6860 2023-07-12 22:15:07.000000 crypto-screening-4.1.2/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-14 12:28:44.881313 crypto-screening-4.1.2/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-4.1.2/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    10966 2023-07-14 07:29:46.000000 crypto-screening-4.1.2/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0     7037 2023-07-14 07:32:35.000000 crypto-screening-4.1.2/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    36128 2023-07-14 08:12:31.000000 crypto-screening-4.1.2/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    17662 2023-07-14 08:12:31.000000 crypto-screening-4.1.2/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0    20526 2023-07-14 07:57:08.000000 crypto-screening-4.1.2/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0     3887 2023-07-12 22:15:36.000000 crypto-screening-4.1.2/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-4.1.2/crypto_screening/process.py
--rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-4.1.2/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     4221 2023-07-14 06:26:34.000000 crypto-screening-4.1.2/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-14 12:28:44.868482 crypto-screening-4.1.2/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-14 12:28:44.000000 crypto-screening-4.1.2/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1239 2023-07-14 12:28:44.000000 crypto-screening-4.1.2/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 12:28:44.000000 crypto-screening-4.1.2/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-07-14 12:28:44.000000 crypto-screening-4.1.2/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-14 12:28:44.000000 crypto-screening-4.1.2/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-14 12:28:44.000000 crypto-screening-4.1.2/pyproject.toml
--rw-rw-rw-   0        0        0      100 2023-07-13 15:40:31.000000 crypto-screening-4.1.2/requirements-dev.txt
--rw-rw-rw-   0        0        0       65 2023-07-13 15:40:31.000000 crypto-screening-4.1.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 12:28:44.882823 crypto-screening-4.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-07-14 12:28:38.000000 crypto-screening-4.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:41:41.122403 crypto-screening-4.1.3/
+-rw-rw-rw-   0        0        0       98 2023-07-14 15:41:40.000000 crypto-screening-4.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-14 15:41:41.122403 crypto-screening-4.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-4.1.3/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-4.1.3/build.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:41:41.094403 crypto-screening-4.1.3/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-14 15:41:41.113403 crypto-screening-4.1.3/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-4.1.3/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-4.1.3/crypto_screening/collect/exchanges.py
+-rw-rw-rw-   0        0        0    45385 2023-07-14 15:39:05.000000 crypto-screening-4.1.3/crypto_screening/collect/market.py
+-rw-rw-rw-   0        0        0    21227 2023-07-14 15:39:05.000000 crypto-screening-4.1.3/crypto_screening/collect/ohlcv.py
+-rw-rw-rw-   0        0        0    19348 2023-07-14 15:39:05.000000 crypto-screening-4.1.3/crypto_screening/collect/orderbook.py
+-rw-rw-rw-   0        0        0    18206 2023-07-14 12:25:47.000000 crypto-screening-4.1.3/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    18977 2023-07-14 12:28:29.000000 crypto-screening-4.1.3/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    14173 2023-07-14 15:33:15.000000 crypto-screening-4.1.3/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-4.1.3/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-4.1.3/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:41:41.114403 crypto-screening-4.1.3/crypto_screening/market/
+-rw-rw-rw-   0        0        0    10937 2023-07-13 18:50:12.000000 crypto-screening-4.1.3/crypto_screening/market/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:41:41.117403 crypto-screening-4.1.3/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-4.1.3/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-4.1.3/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-4.1.3/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6860 2023-07-12 22:15:07.000000 crypto-screening-4.1.3/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:41:41.121403 crypto-screening-4.1.3/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-4.1.3/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    10966 2023-07-14 07:29:46.000000 crypto-screening-4.1.3/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0     7037 2023-07-14 07:32:35.000000 crypto-screening-4.1.3/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    36128 2023-07-14 08:12:31.000000 crypto-screening-4.1.3/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    17662 2023-07-14 08:12:31.000000 crypto-screening-4.1.3/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0    20526 2023-07-14 07:57:08.000000 crypto-screening-4.1.3/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0     3887 2023-07-12 22:15:36.000000 crypto-screening-4.1.3/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-4.1.3/crypto_screening/process.py
+-rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-4.1.3/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     4221 2023-07-14 06:26:34.000000 crypto-screening-4.1.3/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:41:41.108403 crypto-screening-4.1.3/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-14 15:41:41.000000 crypto-screening-4.1.3/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1239 2023-07-14 15:41:41.000000 crypto-screening-4.1.3/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 15:41:41.000000 crypto-screening-4.1.3/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-07-14 15:41:41.000000 crypto-screening-4.1.3/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-14 15:41:41.000000 crypto-screening-4.1.3/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-14 15:41:40.000000 crypto-screening-4.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0      100 2023-07-13 15:40:31.000000 crypto-screening-4.1.3/requirements-dev.txt
+-rw-rw-rw-   0        0        0       65 2023-07-13 15:40:31.000000 crypto-screening-4.1.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 15:41:41.122403 crypto-screening-4.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-07-14 15:39:05.000000 crypto-screening-4.1.3/setup.py
```

### Comparing `crypto-screening-4.1.2/PKG-INFO` & `crypto-screening-4.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 4.1.2
+Version: 4.1.3
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-4.1.2/README.md` & `crypto-screening-4.1.3/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.1.2/build.py` & `crypto-screening-4.1.3/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.1.2/crypto_screening/collect/assets.py` & `crypto-screening-4.1.3/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.1.2/crypto_screening/collect/exchanges.py` & `crypto-screening-4.1.3/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.1.2/crypto_screening/collect/market.py` & `crypto-screening-4.1.3/crypto_screening/collect/market.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,16 +60,16 @@
     "MarketBase",
     "assets_market_data",
     "symbols_market_data",
     "assets_market_state",
     "symbols_market_state",
     "merge_assets_market_states",
     "merge_symbols_market_states",
-    "ORDERBOOK_COLUMNS",
-    "OHLCV_COLUMNS",
+    "ORDERBOOK_ATTRIBUTES",
+    "OHLCV_ATTRIBUTES",
     "assets_to_symbols_screeners",
     "symbols_to_assets_screeners"
 ]
 
 AssetsPrices = Dict[str, Dict[str, Dict[str, List[Tuple[dt.datetime, float]]]]]
 SymbolsPrices = Dict[str, Dict[str, List[Tuple[dt.datetime, float]]]]
 
@@ -736,20 +736,21 @@
     return assets_data
 # end assets_to_symbols_market_data
 
 _S = TypeVar("_S", BaseScreener, OrderbookScreener)
 
 AssetsScreeners = Dict[str, Dict[str, Dict[str, Union[BaseScreener, _S]]]]
 
-ORDERBOOK_COLUMNS = {
+ORDERBOOK_ATTRIBUTES = {
     "bids": BIDS, "asks": ASKS,
-    "bids_volume": BIDS_VOLUME, "asks_volume": ASKS_VOLUME
+    "bids_volume": BIDS_VOLUME,
+    "asks_volume": ASKS_VOLUME
 }
 
-OHLCV_COLUMNS = {
+OHLCV_ATTRIBUTES = {
     "opens": OPEN, "highs": HIGH, "lows": LOW,
     "closes": CLOSE, "volumes": VOLUME
 }
 
 def set_screener_dataset(
         screener: _S,
         dataset: pd.DataFrame,
@@ -765,15 +766,15 @@
     :param replace: The value to replace the dataset.
 
     :return: The screener object.
     """
 
     if (
         isinstance(screener, OHLCVScreener) and
-        (set(dataset.columns) == set(ORDERBOOK_COLUMNS.values()))
+        (set(dataset.columns) == set(ORDERBOOK_ATTRIBUTES.values()))
     ):
         spread_dataset = dataset
 
         if (screener.base_market is not None) and clean:
             screener.base_market.drop(screener.base_market.index, inplace=True)
         # end if
 
@@ -799,15 +800,15 @@
             for index, row in ohlcv_dataset:
                 screener.market[index] = row
             # end for
         # end if
 
     elif (
         isinstance(screener, OrderbookScreener) and
-        (set(dataset.columns) == set(OHLCV_COLUMNS.values()))
+        (set(dataset.columns) != set(ORDERBOOK_ATTRIBUTES.values()))
     ):
         raise ValueError(
             f"Unable to set dataset with columns: "
             f"{dataset.columns} to {type(screener)} object of "
             f"'{screener.exchange}' and symbol '{screener.symbol}' to update its data. "
             f"Consider setting the 'adjust' parameter to True, ignore."
         )
@@ -1053,15 +1054,15 @@
                 )
             # end if
 
             for screener in found_screeners:
                 for index, row in rows:
                     if (
                         isinstance(screener, OHLCVScreener) and
-                        (set(row.keys()) == set(ORDERBOOK_COLUMNS.values()))
+                        (set(row.keys()) == set(ORDERBOOK_ATTRIBUTES.values()))
                     ):
                         screener.base_market.loc[index] = row
 
                     else:
                         screener.market.loc[index] = row
                     # end if
                 # end for
@@ -1210,61 +1211,55 @@
             )
         # end for
     # end for
 
     return new_datasets
 # end symbols_market_data
 
-def minimum_common_dataset_length(
-        columns: Dict[str, str], screeners: Iterable[BaseScreener]
-) -> int:
+def screener_dataset(
+        columns: Dict[str, str], screener: BaseScreener
+) -> pd.DataFrame:
     """
     Finds the minimum common length of all datasets.
 
     :param columns: The columns for the data.
-    :param screeners: The price screeners.
+    :param screener: The price screener.
 
     :return: The minimum common length.
     """
 
-    return min(
-        [
-            len(
-                screener.base_market
-                if (
-                    (columns == ORDERBOOK_COLUMNS) and
-                    isinstance(screener, OHLCVScreener)
-                ) else
-                screener.market
-            )
-            for screener in screeners
-        ]
+    return (
+        screener.base_market
+        if (
+            (columns == ORDERBOOK_ATTRIBUTES) and
+            isinstance(screener, OHLCVScreener)
+        ) else
+        screener.market
     )
-# end minimum_common_dataset_length
+# end screener_dataset
 
-def screener_dataset(
-        columns: Dict[str, str], screener: BaseScreener
-) -> pd.DataFrame:
+def minimum_common_dataset_length(
+        columns: Dict[str, str], screeners: Iterable[BaseScreener]
+) -> int:
     """
     Finds the minimum common length of all datasets.
 
     :param columns: The columns for the data.
-    :param screener: The price screener.
+    :param screeners: The price screeners.
 
     :return: The minimum common length.
     """
 
-    market = screener.market
-
-    if (columns == ORDERBOOK_COLUMNS) and isinstance(screener, OHLCVScreener):
-        market = screener.base_market
-    # end if
-
-    return market
-# end dataset_length
+    return min(
+        [
+            len(screener_dataset(columns=columns, screener=screener))
+            for screener in screeners
+        ]
+    )
+# end minimum_common_dataset_length
 
 def adjusted_dataset_length(
         dataset: pd.DataFrame,
         length: Optional[int] = None,
         adjust: Optional[bool] = True
 ) -> int:
     """
```

### Comparing `crypto-screening-4.1.2/crypto_screening/collect/ohlcv.py` & `crypto-screening-4.1.3/crypto_screening/collect/ohlcv.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,27 +19,27 @@
 from crypto_screening.collect.market import (
     MarketBase, assets_market_prices, symbols_market_data,
     is_symbol_in_assets_market_prices, symbols_market_prices,
     is_symbol_in_symbols_market_prices, assets_market_data,
     assets_to_symbol_market_prices, assets_market_state,
     symbol_to_assets_market_prices, symbols_market_state,
     merge_assets_market_states, merge_symbols_market_states,
-    OHLCV_COLUMNS
+    OHLCV_ATTRIBUTES
 )
 
 __all__ = [
     "symbols_ohlcv_market_state",
     "merge_assets_ohlcv_market_states",
     "merge_symbols_ohlcv_market_states",
     "assets_ohlcv_market_state",
     "AssetsOHLCVMarketState",
     "SymbolsOHLCVMarketState",
     "symbols_to_assets_ohlcv_market_state",
     "assets_to_symbols_ohlcv_market_state",
-    "OHLCV_COLUMNS"
+    "OHLCV_ATTRIBUTES"
 ]
 
 AssetsPrices = Dict[str, Dict[str, Dict[str, List[Tuple[dt.datetime, float]]]]]
 SymbolsPrices = Dict[str, Dict[str, List[Tuple[dt.datetime, float]]]]
 
 @define(repr=False)
 @represent
@@ -311,16 +311,16 @@
         """
         Returns the structured data of the state.
 
         :return: The data of the state.
         """
 
         return assets_market_data(
-            columns=OHLCV_COLUMNS,
-            prices={name: getattr(self, name) for name in OHLCV_COLUMNS}
+            columns=OHLCV_ATTRIBUTES,
+            prices={name: getattr(self, name) for name in OHLCV_ATTRIBUTES}
         )
     # end data
 
     def datasets(self) -> AssetsMarketDatasets:
         """
         Rebuilds the dataset from the market state.
 
@@ -361,15 +361,15 @@
 
     :return: The prices of the assets.
     """
 
     return AssetsOHLCVMarketState(
         screeners=screeners,
         **assets_market_state(
-            columns=OHLCV_COLUMNS,
+            columns=OHLCV_ATTRIBUTES,
             screeners=screeners, separator=separator,
             length=length, adjust=adjust
         )
     )
 # end assets_ohlcv_market_state
 
 SymbolsMarketData = Dict[str, Dict[str, List[Tuple[dt.datetime, Dict[str, float]]]]]
@@ -571,16 +571,16 @@
         """
         Returns the structured data of the state.
 
         :return: The data of the state.
         """
 
         return symbols_market_data(
-            columns=OHLCV_COLUMNS,
-            prices={name: getattr(self, name) for name in OHLCV_COLUMNS}
+            columns=OHLCV_ATTRIBUTES,
+            prices={name: getattr(self, name) for name in OHLCV_ATTRIBUTES}
         )
     # end data
 
     def datasets(self) -> SymbolsMarketDatasets:
         """
         Rebuilds the dataset from the market state.
 
@@ -617,15 +617,15 @@
 
     :return: The prices of the assets.
     """
 
     return SymbolsOHLCVMarketState(
         screeners=screeners,
         **symbols_market_state(
-            columns=OHLCV_COLUMNS, screeners=screeners,
+            columns=OHLCV_ATTRIBUTES, screeners=screeners,
             length=length, adjust=adjust
         )
     )
 # end symbols_ohlcv_market_state
 
 def merge_symbols_ohlcv_market_states(
         *states: SymbolsOHLCVMarketState, sort: Optional[bool] = True
@@ -644,15 +644,15 @@
     for state in states:
         screeners.extend(state.screeners)
     # end for
 
     return SymbolsOHLCVMarketState(
         screeners=set(screeners),
         **merge_symbols_market_states(
-            *states, prices={name: {} for name in OHLCV_COLUMNS}, sort=sort
+            *states, prices={name: {} for name in OHLCV_ATTRIBUTES}, sort=sort
         )
     )
 # end merge_symbols_ohlcv_market_states
 
 def merge_assets_ohlcv_market_states(
         *states: AssetsOHLCVMarketState, sort: Optional[bool] = True
 ) -> AssetsOHLCVMarketState:
@@ -670,15 +670,15 @@
     for state in states:
         screeners.extend(state.screeners)
     # end for
 
     return AssetsOHLCVMarketState(
         screeners=set(screeners),
         **merge_assets_market_states(
-            *states, prices={name: {} for name in OHLCV_COLUMNS}, sort=sort
+            *states, prices={name: {} for name in OHLCV_ATTRIBUTES}, sort=sort
         )
     )
 # end merge_assets_ohlcv_market_states
 
 def assets_to_symbols_ohlcv_market_state(
         state: AssetsOHLCVMarketState,
         separator: Optional[str] = None
@@ -692,15 +692,15 @@
     :return: The results state.
     """
 
     return SymbolsOHLCVMarketState(
         **{
             name: assets_to_symbol_market_prices(
                 prices=getattr(state, name), separator=separator
-            ) for name in OHLCV_COLUMNS
+            ) for name in OHLCV_ATTRIBUTES
         }
     )
 # end assets_to_symbols_ohlcv_market_state
 
 def symbols_to_assets_ohlcv_market_state(
         state: SymbolsOHLCVMarketState,
         separator: Optional[str] = None
@@ -714,11 +714,11 @@
     :return: The results state.
     """
 
     return AssetsOHLCVMarketState(
         **{
             name: symbol_to_assets_market_prices(
                 prices=getattr(state, name), separator=separator
-            ) for name in OHLCV_COLUMNS
+            ) for name in OHLCV_ATTRIBUTES
         }
     )
 # end symbols_to_assets_ohlcv_market_state
```

### Comparing `crypto-screening-4.1.2/crypto_screening/collect/orderbook.py` & `crypto-screening-4.1.3/crypto_screening/collect/orderbook.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,27 +19,27 @@
 from crypto_screening.collect.market import (
     MarketBase, assets_market_prices, assets_market_data,
     is_symbol_in_assets_market_prices, symbols_market_prices,
     is_symbol_in_symbols_market_prices, symbols_market_data,
     assets_to_symbol_market_prices, assets_market_state,
     symbol_to_assets_market_prices, symbols_market_state,
     merge_assets_market_states, merge_symbols_market_states,
-    ORDERBOOK_COLUMNS
+    ORDERBOOK_ATTRIBUTES
 )
 
 __all__ = [
     "symbols_orderbook_market_state",
     "merge_assets_orderbook_market_states",
     "merge_symbols_orderbook_market_states",
     "assets_orderbook_market_state",
     "AssetsOrderbookMarketState",
     "SymbolsOrderbookMarketState",
     "symbols_to_assets_orderbook_market_state",
     "assets_to_symbols_orderbook_market_state",
-    "ORDERBOOK_COLUMNS"
+    "ORDERBOOK_ATTRIBUTES"
 ]
 
 AssetsPrices = Dict[str, Dict[str, Dict[str, List[Tuple[dt.datetime, float]]]]]
 SymbolsPrices = Dict[str, Dict[str, List[Tuple[dt.datetime, float]]]]
 
 @define(repr=False)
 @represent
@@ -269,16 +269,16 @@
         """
         Returns the structured data of the state.
 
         :return: The data of the state.
         """
 
         return assets_market_data(
-            columns=ORDERBOOK_COLUMNS,
-            prices={name: getattr(self, name) for name in ORDERBOOK_COLUMNS}
+            columns=ORDERBOOK_ATTRIBUTES,
+            prices={name: getattr(self, name) for name in ORDERBOOK_ATTRIBUTES}
         )
     # end data
 
     def datasets(self) -> AssetsMarketDatasets:
         """
         Rebuilds the dataset from the market state.
 
@@ -319,15 +319,15 @@
 
     :return: The prices of the assets.
     """
 
     return AssetsOrderbookMarketState(
         screeners=screeners,
         **assets_market_state(
-            columns=ORDERBOOK_COLUMNS,
+            columns=ORDERBOOK_ATTRIBUTES,
             screeners=screeners, separator=separator,
             length=length, adjust=adjust
         )
     )
 # end assets_orderbook_market_state
 
 SymbolsMarketData = Dict[str, Dict[str, List[Tuple[dt.datetime, Dict[str, float]]]]]
@@ -497,16 +497,16 @@
         """
         Returns the structured data of the state.
 
         :return: The data of the state.
         """
 
         return symbols_market_data(
-            columns=ORDERBOOK_COLUMNS,
-            prices={name: getattr(self, name) for name in ORDERBOOK_COLUMNS}
+            columns=ORDERBOOK_ATTRIBUTES,
+            prices={name: getattr(self, name) for name in ORDERBOOK_ATTRIBUTES}
         )
     # end data
 
     def datasets(self) -> SymbolsMarketDatasets:
         """
         Rebuilds the dataset from the market state.
 
@@ -543,15 +543,15 @@
 
     :return: The prices of the assets.
     """
 
     return SymbolsOrderbookMarketState(
         screeners=screeners,
         **symbols_market_state(
-            columns=ORDERBOOK_COLUMNS, screeners=screeners,
+            columns=ORDERBOOK_ATTRIBUTES, screeners=screeners,
             length=length, adjust=adjust
         )
     )
 # end symbols_orderbook_market_state
 
 def merge_symbols_orderbook_market_states(
         *states: SymbolsOrderbookMarketState, sort: Optional[bool] = True
@@ -570,15 +570,15 @@
     for state in states:
         screeners.extend(state.screeners)
     # end for
 
     return SymbolsOrderbookMarketState(
         screeners=set(screeners),
         **merge_symbols_market_states(
-            *states, prices={name: {} for name in ORDERBOOK_COLUMNS}, sort=sort
+            *states, prices={name: {} for name in ORDERBOOK_ATTRIBUTES}, sort=sort
         )
     )
 # end merge_symbols_ohlcv_market_states
 
 def merge_assets_orderbook_market_states(
         *states: AssetsOrderbookMarketState, sort: Optional[bool] = True
 ) -> AssetsOrderbookMarketState:
@@ -596,15 +596,15 @@
     for state in states:
         screeners.extend(state.screeners)
     # end for
 
     return AssetsOrderbookMarketState(
         screeners=set(screeners),
         **merge_assets_market_states(
-            *states, prices={name: {} for name in ORDERBOOK_COLUMNS}, sort=sort
+            *states, prices={name: {} for name in ORDERBOOK_ATTRIBUTES}, sort=sort
         )
     )
 # end merge_assets_ohlcv_market_states
 
 def assets_to_symbols_orderbook_market_state(
         state: AssetsOrderbookMarketState,
         separator: Optional[str] = None
@@ -618,15 +618,15 @@
     :return: The results state.
     """
 
     return SymbolsOrderbookMarketState(
         **{
             name: assets_to_symbol_market_prices(
                 prices=getattr(state, name), separator=separator
-            ) for name in ORDERBOOK_COLUMNS
+            ) for name in ORDERBOOK_ATTRIBUTES
         }
     )
 # end assets_to_symbols_ohlcv_market_state
 
 def symbols_to_assets_orderbook_market_state(
         state: SymbolsOrderbookMarketState,
         separator: Optional[str] = None
@@ -640,11 +640,11 @@
     :return: The results state.
     """
 
     return AssetsOrderbookMarketState(
         **{
             name: symbol_to_assets_market_prices(
                 prices=getattr(state, name), separator=separator
-            ) for name in ORDERBOOK_COLUMNS
+            ) for name in ORDERBOOK_ATTRIBUTES
         }
     )
 # end symbols_to_assets_ohlcv_market_state
```

### Comparing `crypto-screening-4.1.2/crypto_screening/collect/screeners.py` & `crypto-screening-4.1.3/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.1.2/crypto_screening/collect/symbols.py` & `crypto-screening-4.1.3/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.1.2/crypto_screening/dataset.py` & `crypto-screening-4.1.3/crypto_screening/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,16 @@
     "ASKS_VOLUME",
     "CSV_EXTENSION",
     "JSON_EXTENSION",
     "DEFAULT_EXTENSION",
     "BASE_VOLUME",
     "QUOTE_VOLUME",
     "bid_ask_to_ohlcv",
-    "create_market_dataframe"
+    "create_market_dataframe",
+    "ORDERBOOK_COLUMNS"
 ]
 
 OPEN = "Open"
 CLOSE = "Close"
 HIGH = "High"
 LOW = "Low"
 VOLUME = "Volume"
@@ -61,14 +62,15 @@
 BIDS_VOLUME = "Bids Volume"
 ASKS_VOLUME = "Asks Volume"
 BASE_VOLUME = "Base Volume"
 QUOTE_VOLUME = "Quote Volume"
 
 OHLC_COLUMNS = (OPEN, HIGH, LOW, CLOSE)
 OHLCV_COLUMNS = (*OHLC_COLUMNS, VOLUME)
+ORDERBOOK_COLUMNS = (BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME)
 
 def row_to_dataset(
         dataset: Union[pd.DataFrame, pd.Series],
         index: Optional[int] = None
 ) -> pd.DataFrame:
     """
     Creates a dataframe from the row.
```

### Comparing `crypto-screening-4.1.2/crypto_screening/interval.py` & `crypto-screening-4.1.3/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.1.2/crypto_screening/market/dynamic.py` & `crypto-screening-4.1.3/crypto_screening/market/dynamic.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.1.2/crypto_screening/market/foundation/data.py` & `crypto-screening-4.1.3/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.1.2/crypto_screening/market/foundation/protocols.py` & `crypto-screening-4.1.3/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.1.2/crypto_screening/market/foundation/state.py` & `crypto-screening-4.1.3/crypto_screening/market/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.1.2/crypto_screening/market/foundation/waiting.py` & `crypto-screening-4.1.3/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.1.2/crypto_screening/market/screeners/base.py` & `crypto-screening-4.1.3/crypto_screening/market/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.1.2/crypto_screening/market/screeners/container.py` & `crypto-screening-4.1.3/crypto_screening/market/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.1.2/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-4.1.3/crypto_screening/market/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.1.2/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-4.1.3/crypto_screening/market/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.1.2/crypto_screening/market/screeners/recorder.py` & `crypto-screening-4.1.3/crypto_screening/market/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.1.2/crypto_screening/market/waiting.py` & `crypto-screening-4.1.3/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.1.2/crypto_screening/process.py` & `crypto-screening-4.1.3/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.1.2/crypto_screening/symbols.py` & `crypto-screening-4.1.3/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.1.2/crypto_screening/validate.py` & `crypto-screening-4.1.3/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.1.2/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-4.1.3/crypto_screening.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 4.1.2
+Version: 4.1.3
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-4.1.2/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-4.1.3/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.1.2/pyproject.toml` & `crypto-screening-4.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '4.1.2'
+version = '4.1.3'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-4.1.2/setup.py` & `crypto-screening-4.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='4.1.2',
+        version='4.1.3',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

