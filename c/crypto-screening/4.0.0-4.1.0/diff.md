# Comparing `tmp/crypto-screening-4.0.0.tar.gz` & `tmp/crypto-screening-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-4.0.0.tar", last modified: Fri Jul 14 07:59:30 2023, max compression
+gzip compressed data, was "crypto-screening-4.1.0.tar", last modified: Fri Jul 14 09:03:15 2023, max compression
```

## Comparing `crypto-screening-4.0.0.tar` & `crypto-screening-4.1.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 07:59:30.294831 crypto-screening-4.0.0/
--rw-rw-rw-   0        0        0       98 2023-07-14 07:59:28.000000 crypto-screening-4.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-14 07:59:30.293831 crypto-screening-4.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-4.0.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-4.0.0/build.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:59:30.205653 crypto-screening-4.0.0/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-14 07:59:30.257826 crypto-screening-4.0.0/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-4.0.0/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-4.0.0/crypto_screening/collect/exchanges.py
--rw-rw-rw-   0        0        0    43483 2023-07-13 19:47:18.000000 crypto-screening-4.0.0/crypto_screening/collect/market.py
--rw-rw-rw-   0        0        0    21191 2023-07-13 17:18:17.000000 crypto-screening-4.0.0/crypto_screening/collect/ohlcv.py
--rw-rw-rw-   0        0        0    19312 2023-07-13 17:18:17.000000 crypto-screening-4.0.0/crypto_screening/collect/orderbook.py
--rw-rw-rw-   0        0        0    18142 2023-07-12 05:47:33.000000 crypto-screening-4.0.0/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    18974 2023-07-06 12:49:00.000000 crypto-screening-4.0.0/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    14087 2023-07-14 07:29:46.000000 crypto-screening-4.0.0/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-4.0.0/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-4.0.0/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:59:30.267857 crypto-screening-4.0.0/crypto_screening/market/
--rw-rw-rw-   0        0        0    10937 2023-07-13 18:50:12.000000 crypto-screening-4.0.0/crypto_screening/market/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:59:30.288866 crypto-screening-4.0.0/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-4.0.0/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-4.0.0/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-4.0.0/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6860 2023-07-12 22:15:07.000000 crypto-screening-4.0.0/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:59:30.292831 crypto-screening-4.0.0/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-4.0.0/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    10966 2023-07-14 07:29:46.000000 crypto-screening-4.0.0/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0     7037 2023-07-14 07:32:35.000000 crypto-screening-4.0.0/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    34746 2023-07-14 07:57:08.000000 crypto-screening-4.0.0/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    19814 2023-07-14 07:57:08.000000 crypto-screening-4.0.0/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0    20526 2023-07-14 07:57:08.000000 crypto-screening-4.0.0/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0     3887 2023-07-12 22:15:36.000000 crypto-screening-4.0.0/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-4.0.0/crypto_screening/process.py
--rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-4.0.0/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     4221 2023-07-14 06:26:34.000000 crypto-screening-4.0.0/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:59:30.218980 crypto-screening-4.0.0/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-14 07:59:30.000000 crypto-screening-4.0.0/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1239 2023-07-14 07:59:30.000000 crypto-screening-4.0.0/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 07:59:30.000000 crypto-screening-4.0.0/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-07-14 07:59:30.000000 crypto-screening-4.0.0/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-14 07:59:30.000000 crypto-screening-4.0.0/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-14 07:59:28.000000 crypto-screening-4.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      100 2023-07-13 15:40:31.000000 crypto-screening-4.0.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       65 2023-07-13 15:40:31.000000 crypto-screening-4.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 07:59:30.294831 crypto-screening-4.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-07-14 07:59:20.000000 crypto-screening-4.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:03:15.837650 crypto-screening-4.1.0/
+-rw-rw-rw-   0        0        0       98 2023-07-14 09:03:14.000000 crypto-screening-4.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-14 09:03:15.837650 crypto-screening-4.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-4.1.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-4.1.0/build.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:03:15.753360 crypto-screening-4.1.0/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-14 09:03:15.792439 crypto-screening-4.1.0/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-4.1.0/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-4.1.0/crypto_screening/collect/exchanges.py
+-rw-rw-rw-   0        0        0    45525 2023-07-14 09:02:59.000000 crypto-screening-4.1.0/crypto_screening/collect/market.py
+-rw-rw-rw-   0        0        0    21191 2023-07-13 17:18:17.000000 crypto-screening-4.1.0/crypto_screening/collect/ohlcv.py
+-rw-rw-rw-   0        0        0    19312 2023-07-13 17:18:17.000000 crypto-screening-4.1.0/crypto_screening/collect/orderbook.py
+-rw-rw-rw-   0        0        0    18142 2023-07-12 05:47:33.000000 crypto-screening-4.1.0/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    18974 2023-07-06 12:49:00.000000 crypto-screening-4.1.0/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    14087 2023-07-14 07:29:46.000000 crypto-screening-4.1.0/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-4.1.0/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-4.1.0/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:03:15.798409 crypto-screening-4.1.0/crypto_screening/market/
+-rw-rw-rw-   0        0        0    10937 2023-07-13 18:50:12.000000 crypto-screening-4.1.0/crypto_screening/market/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:03:15.815444 crypto-screening-4.1.0/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-4.1.0/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-4.1.0/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-4.1.0/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6860 2023-07-12 22:15:07.000000 crypto-screening-4.1.0/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:03:15.836682 crypto-screening-4.1.0/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-4.1.0/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    10966 2023-07-14 07:29:46.000000 crypto-screening-4.1.0/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0     7037 2023-07-14 07:32:35.000000 crypto-screening-4.1.0/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    36128 2023-07-14 08:12:31.000000 crypto-screening-4.1.0/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    17662 2023-07-14 08:12:31.000000 crypto-screening-4.1.0/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0    20526 2023-07-14 07:57:08.000000 crypto-screening-4.1.0/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0     3887 2023-07-12 22:15:36.000000 crypto-screening-4.1.0/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-4.1.0/crypto_screening/process.py
+-rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-4.1.0/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     4221 2023-07-14 06:26:34.000000 crypto-screening-4.1.0/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:03:15.764360 crypto-screening-4.1.0/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-14 09:03:15.000000 crypto-screening-4.1.0/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1239 2023-07-14 09:03:15.000000 crypto-screening-4.1.0/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 09:03:15.000000 crypto-screening-4.1.0/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-07-14 09:03:15.000000 crypto-screening-4.1.0/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-14 09:03:15.000000 crypto-screening-4.1.0/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-14 09:03:14.000000 crypto-screening-4.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      100 2023-07-13 15:40:31.000000 crypto-screening-4.1.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       65 2023-07-13 15:40:31.000000 crypto-screening-4.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 09:03:15.837650 crypto-screening-4.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-07-14 09:03:09.000000 crypto-screening-4.1.0/setup.py
```

### Comparing `crypto-screening-4.0.0/PKG-INFO` & `crypto-screening-4.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 4.0.0
+Version: 4.1.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-4.0.0/README.md` & `crypto-screening-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.0.0/build.py` & `crypto-screening-4.1.0/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.0.0/crypto_screening/collect/assets.py` & `crypto-screening-4.1.0/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.0.0/crypto_screening/collect/exchanges.py` & `crypto-screening-4.1.0/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.0.0/crypto_screening/collect/market.py` & `crypto-screening-4.1.0/crypto_screening/collect/market.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     "symbols_market_price",
     "assets_market_prices",
     "validate_symbols_market_state_prices_symbol",
     "is_exchange_in_market_prices",
     "is_symbol_in_symbols_market_prices",
     "symbol_to_assets_market_prices",
     "assets_to_symbol_market_prices",
-    "assets_market_dataset_to_symbols_market_datasets",
+    "assets_to_symbols_market_datasets",
     "symbols_to_assets_market_datasets",
     "symbols_screeners",
     "symbols_market_datasets_to_symbols_screeners",
     "assets_screeners",
     "assets_market_datasets_to_assets_screeners",
     "assets_to_symbols_market_data",
     "add_symbols_data_to_screeners",
@@ -61,15 +61,17 @@
     "assets_market_data",
     "symbols_market_data",
     "assets_market_state",
     "symbols_market_state",
     "merge_assets_market_states",
     "merge_symbols_market_states",
     "ORDERBOOK_COLUMNS",
-    "OHLCV_COLUMNS"
+    "OHLCV_COLUMNS",
+    "assets_to_symbols_screeners",
+    "symbols_to_assets_screeners"
 ]
 
 AssetsPrices = Dict[str, Dict[str, Dict[str, List[Tuple[dt.datetime, float]]]]]
 SymbolsPrices = Dict[str, Dict[str, List[Tuple[dt.datetime, float]]]]
 
 def is_exchange_in_market_prices(
         exchange: str,
@@ -573,15 +575,15 @@
             )
         # end for
     # end for
 
     return assets_datasets
 # end symbols_to_assets_market_datasets
 
-def assets_market_dataset_to_symbols_market_datasets(
+def assets_to_symbols_market_datasets(
         datasets: AssetsMarketDatasets, separator: Optional[str] = None
 ) -> SymbolsMarketDatasets:
     """
     Converts the datasets structure from assets to symbols.
 
     :param datasets: The datasets to convert.
     :param separator: The separator for the symbols.
@@ -600,15 +602,15 @@
                     setdefault(exchange, {}).
                     setdefault(symbol, dataset)
                 )
         # end for
     # end for
 
     return symbols_datasets
-# end assets_market_dataset_to_symbols_market_datasets
+# end assets_to_symbols_market_datasets
 
 def assets_to_symbol_market_prices(
         prices: AssetsPrices, separator: Optional[str] = None
 ) -> SymbolsPrices:
     """
     Converts an assets market prices into a symbols market prices.
 
@@ -730,118 +732,141 @@
             # end for
         # end for
     # end for
 
     return assets_data
 # end assets_to_symbols_market_data
 
-_ST = TypeVar("_ST", Type[BaseScreener], Type[OrderbookScreener])
+_S = TypeVar("_S", BaseScreener, OrderbookScreener)
 
-AssetsScreeners = Dict[str, Dict[str, Dict[str, Union[BaseScreener, _ST]]]]
+AssetsScreeners = Dict[str, Dict[str, Dict[str, Union[BaseScreener, _S]]]]
 
 ORDERBOOK_COLUMNS = {
     "bids": BIDS, "asks": ASKS,
     "bids_volume": BIDS_VOLUME, "asks_volume": ASKS_VOLUME
 }
 
 OHLCV_COLUMNS = {
     "opens": OPEN, "highs": HIGH, "lows": LOW,
     "closes": CLOSE, "volumes": VOLUME
 }
 
+def set_screener_dataset(
+        screener: _S,
+        dataset: pd.DataFrame,
+        clean: Optional[bool] = False,
+        replace: Optional[bool] = False
+) -> None:
+    """
+    Sets the dataset for the screener, and return the screener.
+
+    :param dataset: The dataset to insert to the screener.
+    :param screener: The screener object.
+    :param clean: The value to clean the dataset.
+    :param replace: The value to replace the dataset.
+
+    :return: The screener object.
+    """
+
+    if (
+        isinstance(screener, OHLCVScreener) and
+        (set(dataset.columns) == set(ORDERBOOK_COLUMNS.values()))
+    ):
+        spread_dataset = dataset
+
+        if (screener.base_market is not None) and clean:
+            screener.base_market.drop(screener.base_market.index, inplace=True)
+        # end if
+
+        if (screener.base_market is None) or replace:
+            screener.base_market = spread_dataset
+
+        else:
+            for index, row in spread_dataset.iterrows():
+                screener.base_market[index] = row
+            # end for
+        # end if
+
+        if (screener.market is not None) and clean:
+            screener.market.drop(screener.market.index, inplace=True)
+        # end if
+
+        ohlcv_dataset = bid_ask_to_ohlcv(spread_dataset, interval=screener.interval)
+
+        if (screener.market is None) or replace:
+            screener.market = ohlcv_dataset
+
+        else:
+            for index, row in ohlcv_dataset:
+                screener.market[index] = row
+            # end for
+        # end if
+
+    elif (
+        isinstance(screener, OrderbookScreener) and
+        (set(dataset.columns) == set(OHLCV_COLUMNS.values()))
+    ):
+        raise ValueError(
+            f"Unable to set dataset with columns: "
+            f"{dataset.columns} to {type(screener)} object of "
+            f"'{screener.exchange}' and symbol '{screener.symbol}' to update its data. "
+            f"Consider setting the 'adjust' parameter to True, ignore."
+        )
+
+    else:
+        if (screener.market is not None) and clean:
+            screener.market.drop(screener.market.index, inplace=True)
+        # end if
+
+        if (screener.market is None) or replace:
+            screener.market = dataset
+
+        else:
+            for index, row in dataset:
+                screener.market[index] = row
+            # end for
+        # end if
+    # end if
+# end set_screener_dataset
+
 def assets_market_datasets_to_assets_screeners(
         datasets: AssetsMarketDatasets,
         adjust: Optional[bool] = True,
-        base: Optional[_ST] = None,
-        screeners: Optional[BaseScreener] = None,
+        base: Optional[Type[_S]] = None,
+        screeners: Optional[Iterable[_S]] = None,
         separator: Optional[str] = None
 ) -> AssetsScreeners:
     """
     Builds the screeners from the assets market datasets structure.
 
     :param datasets: The datasets for the screeners.
     :param adjust: The value to adjust the data.
     :param base: The base type for a screener.
     :param screeners: screeners to insert datasets into.
     :param separator: The separator for the symbols.
 
     :return: The screeners.
     """
 
-    if screeners is None:
-        screeners = []
-    # end if
-
-    screener_base = base
-
-    new_screeners: AssetsScreeners = {}
-
-    for exchange, bases in datasets.items():
-        for base, quotes in bases.items():
-            for quote, dataset in quotes.items():
-                symbol = parts_to_symbol(base, quote, separator=separator)
-                for screener in screeners:
-                    if not (
-                        (screener.exchange.lower() == exchange.lower()) and
-                        (screener.symbol.lower() == symbol.lower())
-                    ):
-                        screener = screener_base(
-                            symbol=symbol, exchange=exchange
-                        )
-                    # end if
-
-                    if (
-                        isinstance(screener, OHLCVScreener) and
-                        (set(dataset.columns) == set(ORDERBOOK_COLUMNS.values()))
-                    ):
-                        screener.base_market = dataset
-                        screener.market = bid_ask_to_ohlcv(
-                            dataset, interval=screener.interval
-                        )
-
-                    elif (
-                        isinstance(screener, OrderbookScreener) and
-                        (set(dataset.columns) == set(OHLCV_COLUMNS.values()))
-                    ):
-                        if adjust:
-                            continue
-
-                        else:
-                            raise ValueError(
-                                f"Unable to set dataset with columns: "
-                                f"{dataset.columns} to {type(screener)} object of "
-                                f"'{exchange}' and symbol '{symbol}' to update its data. "
-                                f"Consider setting the 'adjust' parameter to True, ignore."
-                            )
-                        # end if
-
-                    else:
-                        screener.market = dataset
-                    # end if
-
-                    (
-                        new_screeners.setdefault(exchange, {}).
-                        setdefault(base, {}).
-                        setdefault(quote, screener)
-                    )
-                # end for
-            # end for
-        # end for
-    # end for
-
-    return new_screeners
+    return symbols_to_assets_screeners(
+        screeners=symbols_market_datasets_to_symbols_screeners(
+            datasets=assets_to_symbols_market_datasets(
+                datasets=datasets, separator=separator
+            ), adjust=adjust, base=base, screeners=screeners
+        ), separator=separator
+    )
 # end assets_market_datasets_to_assets_screeners
 
-SymbolsScreeners = Dict[str, Dict[str, Union[BaseScreener, _ST]]]
+SymbolsScreeners = Dict[str, Dict[str, Union[BaseScreener, _S]]]
 
 def symbols_market_datasets_to_symbols_screeners(
         datasets: SymbolsMarketDatasets,
         adjust: Optional[bool] = True,
-        base: Optional[_ST] = None,
-        screeners: Optional[BaseScreener] = None
+        base: Optional[Type[_S]] = None,
+        screeners: Optional[Iterable[_S]] = None
 ) -> SymbolsScreeners:
     """
     Builds the screeners from the assets market datasets structure.
 
     :param datasets: The datasets for the screeners.
     :param adjust: The value to adjust the data.
     :param base: The base type for a screener.
@@ -850,70 +875,56 @@
     :return: The screeners.
     """
 
     if screeners is None:
         screeners = []
     # end if
 
-    screener_base = base or OrderbookScreener
+    screener_base = base or OHLCVScreener
 
     new_screeners: SymbolsScreeners = {}
 
     for exchange, symbols in datasets.items():
         for symbol, dataset in symbols.items():
-            for screener in screeners:
-                if not (
-                    (screener.exchange.lower() == exchange.lower()) and
-                    (screener.symbol.lower() == symbol.lower())
-                ):
-                    screener = screener_base(
-                        symbol=symbol, exchange=exchange
-                    )
-                # end if
+            try:
+                found_screeners = find_screeners(
+                    screeners, exchange=exchange, symbol=symbol
+                )
 
-                if (
-                    isinstance(screener, OHLCVScreener) and
-                    (set(dataset.columns) == set(ORDERBOOK_COLUMNS.values()))
-                ):
-                    screener.base_market = dataset
-                    screener.market = bid_ask_to_ohlcv(
-                        dataset, interval=screener.interval
-                    )
+            except IndexError:
+                found_screeners = [
+                    screener_base(symbol=symbol, exchange=exchange)
+                ]
+            # end try
+
+            for screener in found_screeners:
+                try:
+                    set_screener_dataset(screener=screener, dataset=dataset)
 
-                elif (
-                    isinstance(screener, OrderbookScreener) and
-                    (set(dataset.columns) == set(OHLCV_COLUMNS.values()))
-                ):
+                except ValueError as e:
                     if adjust:
                         continue
 
                     else:
-                        raise ValueError(
-                            f"Unable to set dataset with columns: "
-                            f"{dataset.columns} to {type(screener)} object of "
-                            f"'{exchange}' and symbol '{symbol}' to update its data. "
-                            f"Consider setting the 'adjust' parameter to True, ignore."
-                        )
+                        raise e
                     # end if
+                # end try
 
-                else:
-                    screener.market = dataset
-                # end if
                 (
                     new_screeners.setdefault(exchange, {}).
                     setdefault(symbol, screener)
                 )
             # end for
         # end for
     # end for
 
     return new_screeners
 # end symbols_market_datasets_to_symbols_screeners
 
-def assets_screeners(screeners: AssetsScreeners) -> List[Union[BaseScreener, _ST]]:
+def assets_screeners(screeners: AssetsScreeners) -> List[Union[BaseScreener, _S]]:
     """
     Collects the screeners from the assets screeners structure.
 
     :param screeners: The screeners structure.
 
     :return: The screeners' collection.
     """
@@ -927,15 +938,79 @@
             # end for
         # end for
     # end for
 
     return screeners_collection
 # end assets_screeners
 
-def symbols_screeners(screeners: SymbolsScreeners) -> List[Union[BaseScreener, _ST]]:
+def symbols_to_assets_screeners(
+        screeners: SymbolsScreeners,
+        separator: Optional[str] = None
+) -> AssetsScreeners:
+    """
+    Collects the screeners from the assets screeners structure.
+
+    :param screeners: The screeners structure.
+    :param separator: The separator for the symbols.
+
+    :return: The screeners' collection.
+    """
+
+    data: AssetsScreeners = {}
+
+    for exchange, symbols in screeners.items():
+        for symbol, screener in symbols.items():
+            base, quote = symbol_to_parts(symbol, separator=separator)
+            (
+                data.
+                setdefault(exchange, {}).
+                setdefault(base, {}).
+                setdefault(quote, screener)
+            )
+            # end for
+        # end for
+    # end for
+
+    return data
+# end assets_screeners
+
+def assets_to_symbols_screeners(
+        screeners: AssetsScreeners,
+        separator: Optional[str] = None
+) -> SymbolsScreeners:
+    """
+    Collects the screeners from the assets screeners structure.
+
+    :param screeners: The screeners structure.
+    :param separator: The separator for the symbols.
+
+    :return: The screeners' collection.
+    """
+
+    data: SymbolsScreeners = {}
+
+    for exchange, bases in screeners.items():
+        for base, quotes in bases.items():
+            for quote, screener in quotes.items():
+                (
+                    data.
+                    setdefault(exchange, {}).
+                    setdefault(
+                        parts_to_symbol(base, quote, separator=separator),
+                        screener
+                    )
+                )
+            # end for
+        # end for
+    # end for
+
+    return data
+# end assets_screeners
+
+def symbols_screeners(screeners: SymbolsScreeners) -> List[Union[BaseScreener, _S]]:
     """
     Collects the screeners from the symbols screeners structure.
 
     :param screeners: The screeners structure.
 
     :return: The screeners' collection.
     """
@@ -966,32 +1041,32 @@
 
     for exchange, symbols in data.items():
         for symbol, rows in symbols.items():
             found_screeners = find_screeners(
                 screeners, exchange=exchange, symbol=symbol
             )
 
-            if not found_screeners and not adjust:
+            if (not found_screeners) and (not adjust):
                 raise ValueError(
                     f"Unable to find a screener with exchange "
                     f"'{exchange}' and symbol '{symbol}' to update its data. "
                     f"Consider setting the 'adjust' parameter to True, ignore."
                 )
             # end if
 
             for screener in found_screeners:
-                for time, row in rows:
+                for index, row in rows:
                     if (
                         isinstance(screener, OHLCVScreener) and
                         (set(row.keys()) == set(ORDERBOOK_COLUMNS.values()))
                     ):
-                        screener.base_market.loc[time] = row
+                        screener.base_market.loc[index] = row
 
                     else:
-                        screener.market.loc[time] = row
+                        screener.market.loc[index] = row
                     # end if
                 # end for
             # end for
         # end for
     # end for
 # end add_symbols_data_to_screeners
 
@@ -1011,14 +1086,38 @@
     return add_symbols_data_to_screeners(
         screeners=screeners,
         data=assets_to_symbols_market_data(data=data),
         adjust=adjust
     )
 # end add_assets_data_to_screeners
 
+def index_to_datetime(index: Any) -> dt.datetime:
+    """
+    Converts the index into a datetime object.
+
+    :param index: The value to convert.
+
+    :return: The datetime object.
+    """
+
+    try:
+        if isinstance(index, str):
+            index = dt.datetime.fromisoformat(index)
+
+        elif isinstance(index, int):
+            index = dt.datetime.fromtimestamp(index)
+        # end if
+
+    except (Type, ValueError):
+        pass
+    # end try
+
+    return index
+# end index_to_datetime
+
 def assets_market_data(
         columns: Dict[str, str],
         prices: Optional[Dict[str, AssetsPrices]] = None
 ) -> AssetsMarketData:
     """
     Returns the structured data of the state.
 
@@ -1032,33 +1131,23 @@
 
     datasets: Dict[str, Dict[str, Dict[str, Dict[dt.datetime, Dict[str, float]]]]] = {}
 
     for name in columns:
         for exchange, bases in prices[name].items():
             for base, quotes in bases.items():
                 for quote, symbols_prices in quotes.items():
-                    for i, (time, price) in enumerate(symbols_prices):
-                        try:
-                            if isinstance(time, str):
-                                time = dt.datetime.fromisoformat(time)
-
-                            elif isinstance(time, int):
-                                time = dt.datetime.fromtimestamp(time)
-                            # end if
-
-                        except (Type, ValueError):
-                            pass
-                        # end try
+                    for i, (index, price) in enumerate(symbols_prices):
+                        index = index_to_datetime(index)
 
                         (
                             datasets.
                             setdefault(exchange, {}).
                             setdefault(base, {}).
                             setdefault(quote, {}).
-                            setdefault(time, {})
+                            setdefault(index, {})
                         )[columns[name]] = price
                     # end for
             # end for
         # end for
     # end for
 
     new_datasets: AssetsMarketData = {}
@@ -1094,31 +1183,22 @@
     """
 
     datasets: Dict[str, Dict[str, Dict[dt.datetime, Dict[str, float]]]] = {}
 
     for name in columns:
         for exchange, symbols in prices[name].items():
             for symbol, symbols_prices in symbols.items():
-                for i, (time, price) in enumerate(symbols_prices):
-                    try:
-                        if isinstance(time, str):
-                            time = dt.datetime.fromisoformat(time)
-
-                        elif isinstance(time, int):
-                            time = dt.datetime.fromtimestamp(time)
-
-                    except (Type, ValueError):
-                        pass
-                    # end try
+                for i, (index, price) in enumerate(symbols_prices):
+                    index = index_to_datetime(index)
 
                     (
                         datasets.
                         setdefault(exchange, {}).
                         setdefault(symbol, {}).
-                        setdefault(time, {})
+                        setdefault(index, {})
                     )[columns[name]] = price
                 # end for
             # end for
         # end for
     # end for
 
     new_datasets: SymbolsMarketData = {}
@@ -1130,18 +1210,99 @@
             )
         # end for
     # end for
 
     return new_datasets
 # end symbols_market_data
 
+def minimum_common_dataset_length(
+        columns: Dict[str, str], screeners: Iterable[BaseScreener]
+) -> int:
+    """
+    Finds the minimum common length of all datasets.
+
+    :param columns: The columns for the data.
+    :param screeners: The price screeners.
+
+    :return: The minimum common length.
+    """
+
+    return min(
+        [
+            len(
+                screener.base_market
+                if (
+                    (columns == ORDERBOOK_COLUMNS) and
+                    isinstance(screener, OHLCVScreener)
+                ) else
+                screener.market
+            )
+            for screener in screeners
+        ]
+    )
+# end minimum_common_dataset_length
+
+def screener_dataset(
+        columns: Dict[str, str], screener: BaseScreener
+) -> pd.DataFrame:
+    """
+    Finds the minimum common length of all datasets.
+
+    :param columns: The columns for the data.
+    :param screener: The price screener.
+
+    :return: The minimum common length.
+    """
+
+    market = screener.market
+
+    if (columns == ORDERBOOK_COLUMNS) and isinstance(screener, OHLCVScreener):
+        market = screener.base_market
+    # end if
+
+    return market
+# end dataset_length
+
+def adjusted_dataset_length(
+        dataset: pd.DataFrame,
+        length: Optional[int] = None,
+        adjust: Optional[bool] = True
+) -> int:
+    """
+    Finds the minimum common length of all datasets.
+
+    :param dataset: The price dataset.
+    :param length: The base length.
+    :param adjust: The value to adjust the length.
+
+    :return: The minimum common length.
+    """
+
+    if adjust and (length is None):
+        length = len(dataset)
+
+    elif adjust:
+        length = min([len(dataset), length])
+        # end if
+
+    if length > len(dataset):
+        raise ValueError(
+            f"Data is not long enough for the requested length: {length}. "
+            f"Consider using the 'adjust' parameter as {True}, "
+            f"to adjust to the actual length of the data."
+        )
+    # end if
+
+    return length
+# end adjusted_dataset_length
+
 def assets_market_state(
         columns: Dict[str, str],
+        screeners: Iterable[BaseScreener],
         prices: Optional[Dict[str, AssetsPrices]] = None,
-        screeners: Optional[Iterable[BaseScreener]] = None,
         separator: Optional[str] = None,
         length: Optional[int] = None,
         adjust: Optional[bool] = True
 ) -> Dict[str, AssetsPrices]:
     """
     Fetches the prices and relations between the assets.
 
@@ -1154,52 +1315,33 @@
 
     :return: The prices of the assets.
     """
 
     prices = prices or {name: {} for name in columns}
 
     if (length is None) and (not adjust):
-        length = min(
-            [
-                len(
-                    screener.base_market
-                    if (
-                        (columns == ORDERBOOK_COLUMNS) and
-                        isinstance(screener, OHLCVScreener)
-                    ) else
-                    screener.market
-                )
-                for screener in screeners
-            ]
+        length = minimum_common_dataset_length(
+            columns=columns, screeners=screeners
         )
     # end if
 
     for screener in screeners:
-        market = screener.market
-
-        if (columns == ORDERBOOK_COLUMNS) and isinstance(screener, OHLCVScreener):
-            market = screener.base_market
-        # end if
-
-        if adjust and (length is None):
-            length = len(market)
+        market = screener_dataset(columns=columns, screener=screener)
 
-        elif adjust:
-            length = min([len(market), length])
-        # end if
+        try:
+            length = adjusted_dataset_length(
+                dataset=market, adjust=adjust, length=length
+            )
 
-        if length > len(market):
+        except ValueError as e:
             raise ValueError(
                 f"Data of '{screener.exchange}' "
-                f"symbol in '{screener.symbol}' exchange "
-                f"is not long enough for the requested length: {length}. "
-                f"Consider using the 'adjust' parameter as {True}, "
-                f"to adjust to the actual length of the data."
+                f"symbol in '{screener.symbol}' exchange: {e}"
             )
-        # end if
+        # end try
 
         base, quote = symbol_to_parts(
             symbol=screener.symbol, separator=separator
         )
 
         for name in columns:
             (
@@ -1239,51 +1381,33 @@
 
     :return: The prices of the assets.
     """
 
     prices = prices or {name: {} for name in columns}
 
     if (length is None) and (not adjust):
-        length = min(
-            [
-                len(
-                    screener.base_market
-                    if (
-                        (columns == ORDERBOOK_COLUMNS) and
-                        isinstance(screener, OHLCVScreener)
-                    ) else
-                    screener.market
-                )
-                for screener in screeners
-            ]
+        length = minimum_common_dataset_length(
+            columns=columns, screeners=screeners
         )
     # end if
 
     for screener in screeners:
-        market = screener.market
-
-        if (columns == ORDERBOOK_COLUMNS) and isinstance(screener, OHLCVScreener):
-            market = screener.base_market
-        # end if
+        market = screener_dataset(columns=columns, screener=screener)
 
-        if adjust and (length is None):
-            length = len(market)
-
-        elif adjust:
-            length = min([len(market), length])
-        # end if
+        try:
+            length = adjusted_dataset_length(
+                dataset=market, adjust=adjust, length=length
+            )
 
-        if length > len(market):
+        except ValueError as e:
             raise ValueError(
-                f"Data of '{screener.exchange}' symbol in '{screener.symbol}' exchange "
-                f"is not long enough for the requested length: {length}. "
-                f"Consider using the 'adjust' parameter as {True}, "
-                f"to adjust to the actual length of the data."
+                f"Data of '{screener.exchange}' "
+                f"symbol in '{screener.symbol}' exchange: {e}"
             )
-        # end if
+        # end try
 
         for name in columns:
             (
                 prices[name].
                 setdefault(screener.exchange, {}).
                 setdefault(
                     screener.symbol,
```

### Comparing `crypto-screening-4.0.0/crypto_screening/collect/ohlcv.py` & `crypto-screening-4.1.0/crypto_screening/collect/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.0.0/crypto_screening/collect/orderbook.py` & `crypto-screening-4.1.0/crypto_screening/collect/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.0.0/crypto_screening/collect/screeners.py` & `crypto-screening-4.1.0/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.0.0/crypto_screening/collect/symbols.py` & `crypto-screening-4.1.0/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.0.0/crypto_screening/dataset.py` & `crypto-screening-4.1.0/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.0.0/crypto_screening/interval.py` & `crypto-screening-4.1.0/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.0.0/crypto_screening/market/dynamic.py` & `crypto-screening-4.1.0/crypto_screening/market/dynamic.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.0.0/crypto_screening/market/foundation/data.py` & `crypto-screening-4.1.0/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.0.0/crypto_screening/market/foundation/protocols.py` & `crypto-screening-4.1.0/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.0.0/crypto_screening/market/foundation/state.py` & `crypto-screening-4.1.0/crypto_screening/market/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.0.0/crypto_screening/market/foundation/waiting.py` & `crypto-screening-4.1.0/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.0.0/crypto_screening/market/screeners/base.py` & `crypto-screening-4.1.0/crypto_screening/market/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.0.0/crypto_screening/market/screeners/container.py` & `crypto-screening-4.1.0/crypto_screening/market/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.0.0/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-4.1.0/crypto_screening/market/screeners/ohlcv.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from crypto_screening.interval import interval_to_total_time
 from crypto_screening.dataset import (
     OHLCV_COLUMNS, VOLUME, BIDS, BIDS_VOLUME,
     load_dataset, save_dataset, OHLC_COLUMNS, create_market_dataframe
 )
 from crypto_screening.validate import validate_interval
 from crypto_screening.symbols import adjust_symbol
+from crypto_screening.market.screeners.base import BaseScreener
 from crypto_screening.market.screeners.recorder import (
     structure_screener_datasets, MarketRecorder, validate_market
 )
 from crypto_screening.market.screeners.orderbook import (
     create_orderbook_dataframe, OrderbookScreener, record_orderbook,
     OrderbookMarketScreener, create_orderbook_market, OrderbookMarketRecorder
 )
@@ -80,15 +81,15 @@
         exchange.lower(): {
             symbol.upper(): [interval]
             for symbol in symbols
         } for exchange, symbols in data.items()
     }
 # end datasets_to_intervals_datasets
 
-class OHLCVScreener(OrderbookScreener):
+class OHLCVScreener(BaseScreener):
     """
     A class to represent an asset price screener.
 
     Using this class, you can create a screener object to
     screen the market ask and bid data for a specific asset in
     a specific exchange at real time.
 
@@ -186,14 +187,41 @@
 
         :return: The market object.
         """
 
         return self.market
     # end ohlcv_market
 
+    def orderbook_dataset_path(self, location: Optional[str] = None) -> str:
+        """
+        Creates the path to the saving file for the screener object.
+
+        :param location: The saving location of the dataset.
+
+        :return: The saving path for the dataset.
+        """
+
+        return self.dataset_path(location=location)
+    # end orderbook_dataset_path
+
+    def save_orderbook_dataset(self, location: Optional[str] = None) -> None:
+        """
+        Saves the data of the screener.
+
+        :param location: The saving location of the dataset.
+        """
+
+        if len(self.orderbook_market) > 0:
+            save_dataset(
+                dataset=self.orderbook_market,
+                path=self.orderbook_dataset_path(location=location)
+            )
+        # end if
+    # end save_orderbook_dataset
+
     def ohlcv_dataset_path(self, location: Optional[str] = None) -> str:
         """
         Creates the path to the saving file for the screener object.
 
         :param location: The saving location of the dataset.
 
         :return: The saving path for the dataset.
@@ -247,18 +275,32 @@
 
         :param location: The saving location of the dataset.
         """
 
         data = load_dataset(path=self.ohlcv_dataset_path(location=location))
 
         for index, data in zip(data.index[:], data.loc[:]):
-            self.market.loc[index] = data
+            self.ohlcv_market.loc[index] = data
         # end for
     # end load_ohlcv_dataset
 
+    def load_orderbook_dataset(self, location: Optional[str] = None) -> None:
+        """
+        Saves the data of the screener.
+
+        :param location: The saving location of the dataset.
+        """
+
+        data = load_dataset(path=self.orderbook_dataset_path(location=location))
+
+        for index, data in zip(data.index[:], data.loc[:]):
+            self.orderbook_market.loc[index] = data
+        # end for
+    # end load_orderbook_dataset
+
     def load_datasets(self, location: Optional[str] = None) -> None:
         """
         Saves the data of the screener.
 
         :param location: The saving location of the dataset.
         """
```

### Comparing `crypto-screening-4.0.0/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-4.1.0/crypto_screening/market/screeners/orderbook.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from cryptofeed import FeedHandler
 from cryptofeed.types import OrderBook
 from cryptofeed.defines import L2_BOOK
 
 from crypto_screening.symbols import adjust_symbol
 from crypto_screening.process import find_string_value
 from crypto_screening.dataset import (
-    BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME, load_dataset,
-    create_market_dataframe, save_dataset
+    BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME,
+    create_market_dataframe
 )
 from crypto_screening.market.screeners.recorder import MarketRecorder
 from crypto_screening.market.screeners.base import BaseScreener
 from crypto_screening.market.screeners.recorder import (
     MarketScreener, structure_screener_datasets
 )
 
@@ -89,86 +89,14 @@
 
     - delay:
         The delay to wait between each data fetching.
 
     - market:
         The dataset of the market data as BID/ASK spread.
     """
-
-    @property
-    def orderbook_market(self) -> pd.DataFrame:
-        """
-        Returns the market to hold the recorder data.
-
-        :return: The market object.
-        """
-
-        return self.market
-    # end orderbook_market
-
-    def orderbook_dataset_path(self, location: Optional[str] = None) -> str:
-        """
-        Creates the path to the saving file for the screener object.
-
-        :param location: The saving location of the dataset.
-
-        :return: The saving path for the dataset.
-        """
-
-        return self.dataset_path(location=location)
-    # end orderbook_dataset_path
-
-    def save_orderbook_dataset(self, location: Optional[str] = None) -> None:
-        """
-        Saves the data of the screener.
-
-        :param location: The saving location of the dataset.
-        """
-
-        if len(self.orderbook_market) > 0:
-            save_dataset(
-                dataset=self.orderbook_market,
-                path=self.orderbook_dataset_path(location=location)
-            )
-        # end if
-    # end save_ohlcv_dataset
-
-    def save_dataset(self, location: Optional[str] = None) -> None:
-        """
-        Saves the data of the screener.
-
-        :param location: The saving location of the dataset.
-        """
-
-        self.save_orderbook_dataset(location=location)
-    # end save_dataset
-
-    def load_orderbook_dataset(self, location: Optional[str] = None) -> None:
-        """
-        Saves the data of the screener.
-
-        :param location: The saving location of the dataset.
-        """
-
-        data = load_dataset(path=self.orderbook_dataset_path(location=location))
-
-        for index, data in zip(data.index[:], data.loc[:]):
-            self.orderbook_market.loc[index] = data
-        # end for
-    # end load_orderbook_dataset
-
-    def load_dataset(self, location: Optional[str] = None) -> None:
-        """
-        Saves the data of the screener.
-
-        :param location: The saving location of the dataset.
-        """
-
-        self.load_orderbook_dataset(location=location)
-    # end load_dataset
 # end OrderBookScreener
 
 def validate_orderbook_market(data: Any) -> Market:
     """
     Validates the data.
 
     :param data: The data to validate.
```

### Comparing `crypto-screening-4.0.0/crypto_screening/market/screeners/recorder.py` & `crypto-screening-4.1.0/crypto_screening/market/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.0.0/crypto_screening/market/waiting.py` & `crypto-screening-4.1.0/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.0.0/crypto_screening/process.py` & `crypto-screening-4.1.0/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.0.0/crypto_screening/symbols.py` & `crypto-screening-4.1.0/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.0.0/crypto_screening/validate.py` & `crypto-screening-4.1.0/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.0.0/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-4.1.0/crypto_screening.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 4.0.0
+Version: 4.1.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-4.0.0/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-4.1.0/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.0.0/pyproject.toml` & `crypto-screening-4.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '4.0.0'
+version = '4.1.0'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-4.0.0/setup.py` & `crypto-screening-4.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='4.0.0',
+        version='4.1.0',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

