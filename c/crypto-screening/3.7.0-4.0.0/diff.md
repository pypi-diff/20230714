# Comparing `tmp/crypto-screening-3.7.0.tar.gz` & `tmp/crypto-screening-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-3.7.0.tar", last modified: Thu Jul 13 19:48:04 2023, max compression
+gzip compressed data, was "crypto-screening-4.0.0.tar", last modified: Fri Jul 14 07:59:30 2023, max compression
```

## Comparing `crypto-screening-3.7.0.tar` & `crypto-screening-4.0.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 19:48:04.909408 crypto-screening-3.7.0/
--rw-rw-rw-   0        0        0       98 2023-07-13 19:48:04.000000 crypto-screening-3.7.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-13 19:48:04.909408 crypto-screening-3.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-3.7.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-3.7.0/build.py
-drwxrwxrwx   0        0        0        0 2023-07-13 19:48:04.884410 crypto-screening-3.7.0/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-13 19:48:04.898408 crypto-screening-3.7.0/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-3.7.0/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-3.7.0/crypto_screening/collect/exchanges.py
--rw-rw-rw-   0        0        0    43483 2023-07-13 19:47:18.000000 crypto-screening-3.7.0/crypto_screening/collect/market.py
--rw-rw-rw-   0        0        0    21191 2023-07-13 17:18:17.000000 crypto-screening-3.7.0/crypto_screening/collect/ohlcv.py
--rw-rw-rw-   0        0        0    19312 2023-07-13 17:18:17.000000 crypto-screening-3.7.0/crypto_screening/collect/orderbook.py
--rw-rw-rw-   0        0        0    18142 2023-07-12 05:47:33.000000 crypto-screening-3.7.0/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    18974 2023-07-06 12:49:00.000000 crypto-screening-3.7.0/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    13639 2023-07-13 15:21:10.000000 crypto-screening-3.7.0/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-3.7.0/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5281 2023-07-06 12:49:43.000000 crypto-screening-3.7.0/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-13 19:48:04.900383 crypto-screening-3.7.0/crypto_screening/market/
--rw-rw-rw-   0        0        0    10937 2023-07-13 18:50:12.000000 crypto-screening-3.7.0/crypto_screening/market/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-07-13 19:48:04.903409 crypto-screening-3.7.0/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-3.7.0/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-3.7.0/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-3.7.0/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6860 2023-07-12 22:15:07.000000 crypto-screening-3.7.0/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-13 19:48:04.908383 crypto-screening-3.7.0/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-3.7.0/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    18442 2023-07-13 14:37:22.000000 crypto-screening-3.7.0/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0     7012 2023-07-13 18:45:57.000000 crypto-screening-3.7.0/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    30311 2023-07-13 17:42:52.000000 crypto-screening-3.7.0/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    14109 2023-07-13 13:54:09.000000 crypto-screening-3.7.0/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0    14866 2023-07-13 13:45:46.000000 crypto-screening-3.7.0/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0     3887 2023-07-12 22:15:36.000000 crypto-screening-3.7.0/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-3.7.0/crypto_screening/process.py
--rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-3.7.0/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     3857 2023-07-10 17:12:15.000000 crypto-screening-3.7.0/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-13 19:48:04.893383 crypto-screening-3.7.0/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-13 19:48:04.000000 crypto-screening-3.7.0/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1239 2023-07-13 19:48:04.000000 crypto-screening-3.7.0/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 19:48:04.000000 crypto-screening-3.7.0/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-07-13 19:48:04.000000 crypto-screening-3.7.0/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-13 19:48:04.000000 crypto-screening-3.7.0/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-13 19:48:04.000000 crypto-screening-3.7.0/pyproject.toml
--rw-rw-rw-   0        0        0      100 2023-07-13 15:40:31.000000 crypto-screening-3.7.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       65 2023-07-13 15:40:31.000000 crypto-screening-3.7.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 19:48:04.909408 crypto-screening-3.7.0/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-07-13 19:47:53.000000 crypto-screening-3.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:59:30.294831 crypto-screening-4.0.0/
+-rw-rw-rw-   0        0        0       98 2023-07-14 07:59:28.000000 crypto-screening-4.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-14 07:59:30.293831 crypto-screening-4.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-4.0.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-4.0.0/build.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:59:30.205653 crypto-screening-4.0.0/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-14 07:59:30.257826 crypto-screening-4.0.0/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-4.0.0/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-4.0.0/crypto_screening/collect/exchanges.py
+-rw-rw-rw-   0        0        0    43483 2023-07-13 19:47:18.000000 crypto-screening-4.0.0/crypto_screening/collect/market.py
+-rw-rw-rw-   0        0        0    21191 2023-07-13 17:18:17.000000 crypto-screening-4.0.0/crypto_screening/collect/ohlcv.py
+-rw-rw-rw-   0        0        0    19312 2023-07-13 17:18:17.000000 crypto-screening-4.0.0/crypto_screening/collect/orderbook.py
+-rw-rw-rw-   0        0        0    18142 2023-07-12 05:47:33.000000 crypto-screening-4.0.0/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    18974 2023-07-06 12:49:00.000000 crypto-screening-4.0.0/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    14087 2023-07-14 07:29:46.000000 crypto-screening-4.0.0/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-4.0.0/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-4.0.0/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:59:30.267857 crypto-screening-4.0.0/crypto_screening/market/
+-rw-rw-rw-   0        0        0    10937 2023-07-13 18:50:12.000000 crypto-screening-4.0.0/crypto_screening/market/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:59:30.288866 crypto-screening-4.0.0/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-4.0.0/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-4.0.0/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-4.0.0/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6860 2023-07-12 22:15:07.000000 crypto-screening-4.0.0/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:59:30.292831 crypto-screening-4.0.0/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-4.0.0/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    10966 2023-07-14 07:29:46.000000 crypto-screening-4.0.0/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0     7037 2023-07-14 07:32:35.000000 crypto-screening-4.0.0/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    34746 2023-07-14 07:57:08.000000 crypto-screening-4.0.0/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    19814 2023-07-14 07:57:08.000000 crypto-screening-4.0.0/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0    20526 2023-07-14 07:57:08.000000 crypto-screening-4.0.0/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0     3887 2023-07-12 22:15:36.000000 crypto-screening-4.0.0/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-4.0.0/crypto_screening/process.py
+-rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-4.0.0/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     4221 2023-07-14 06:26:34.000000 crypto-screening-4.0.0/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:59:30.218980 crypto-screening-4.0.0/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-14 07:59:30.000000 crypto-screening-4.0.0/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1239 2023-07-14 07:59:30.000000 crypto-screening-4.0.0/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 07:59:30.000000 crypto-screening-4.0.0/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-07-14 07:59:30.000000 crypto-screening-4.0.0/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-14 07:59:30.000000 crypto-screening-4.0.0/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-14 07:59:28.000000 crypto-screening-4.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0      100 2023-07-13 15:40:31.000000 crypto-screening-4.0.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       65 2023-07-13 15:40:31.000000 crypto-screening-4.0.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 07:59:30.294831 crypto-screening-4.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-07-14 07:59:20.000000 crypto-screening-4.0.0/setup.py
```

### Comparing `crypto-screening-3.7.0/PKG-INFO` & `crypto-screening-4.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 3.7.0
+Version: 4.0.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-3.7.0/README.md` & `crypto-screening-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.7.0/build.py` & `crypto-screening-4.0.0/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.7.0/crypto_screening/collect/assets.py` & `crypto-screening-4.0.0/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.7.0/crypto_screening/collect/exchanges.py` & `crypto-screening-4.0.0/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.7.0/crypto_screening/collect/market.py` & `crypto-screening-4.0.0/crypto_screening/collect/market.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.7.0/crypto_screening/collect/ohlcv.py` & `crypto-screening-4.0.0/crypto_screening/collect/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.7.0/crypto_screening/collect/orderbook.py` & `crypto-screening-4.0.0/crypto_screening/collect/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.7.0/crypto_screening/collect/screeners.py` & `crypto-screening-4.0.0/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.7.0/crypto_screening/collect/symbols.py` & `crypto-screening-4.0.0/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.7.0/crypto_screening/dataset.py` & `crypto-screening-4.0.0/crypto_screening/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,16 @@
     "BIDS_VOLUME",
     "ASKS_VOLUME",
     "CSV_EXTENSION",
     "JSON_EXTENSION",
     "DEFAULT_EXTENSION",
     "BASE_VOLUME",
     "QUOTE_VOLUME",
-    "bid_ask_to_ohlcv"
+    "bid_ask_to_ohlcv",
+    "create_market_dataframe"
 ]
 
 OPEN = "Open"
 CLOSE = "Close"
 HIGH = "High"
 LOW = "Low"
 VOLUME = "Volume"
@@ -509,8 +510,25 @@
     volume: pd.DataFrame = (
         dataset[BIDS_VOLUME].resample(adjuster).ohlc()
     )
     volume.columns = [OPEN, HIGH, LOW, CLOSE]
     ohlcv_dataset[VOLUME] = volume[CLOSE]
 
     return ohlcv_dataset
-# end bid_ask_to_ohlcv
+# end bid_ask_to_ohlcv
+
+def create_market_dataframe(columns: Optional[Iterable[str]] = None) -> pd.DataFrame:
+    """
+    Creates a dataframe for the order book data.
+
+    :param columns: The dataset columns.
+
+    :return: The dataframe.
+    """
+
+    market = pd.DataFrame(
+        {column: [] for column in columns or []}, index=[]
+    )
+    market.index.name = DATE_TIME
+
+    return market
+# end create_market_dataframe
```

### Comparing `crypto-screening-3.7.0/crypto_screening/interval.py` & `crypto-screening-4.0.0/crypto_screening/interval.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,15 +189,20 @@
     :param interval: The interval to extract.
 
     :return: The type from the interval.
     """
 
     number = interval_to_duration(interval)
 
-    return INTERVALS[interval.replace(str(number), "")]
+    try:
+        return INTERVALS[interval.replace(str(number), "")]
+
+    except KeyError:
+        raise ValueError(f"Invalid interval structure: {interval}.")
+    # end try
 # end interval_to_time
 
 def interval_to_total_time(interval: str) -> dt.timedelta:
     """
     Extracts the type from the interval.
 
     :param interval: The interval to extract.
```

### Comparing `crypto-screening-3.7.0/crypto_screening/market/dynamic.py` & `crypto-screening-4.0.0/crypto_screening/market/dynamic.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.7.0/crypto_screening/market/foundation/data.py` & `crypto-screening-4.0.0/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.7.0/crypto_screening/market/foundation/protocols.py` & `crypto-screening-4.0.0/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.7.0/crypto_screening/market/foundation/state.py` & `crypto-screening-4.0.0/crypto_screening/market/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.7.0/crypto_screening/market/foundation/waiting.py` & `crypto-screening-4.0.0/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.7.0/crypto_screening/market/screeners/base.py` & `crypto-screening-4.0.0/crypto_screening/market/screeners/recorder.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,275 +1,165 @@
-# base.py
+# recorder.py
 
-import datetime as dt
+import warnings
+import threading
 import time
+import datetime as dt
 from typing import (
-    Optional, Union, Dict, Iterable, Any, List, Callable
+    Optional, Dict, Any, List, Iterable, Type, Union
 )
+from functools import partial
+import asyncio
 
 import pandas as pd
 
 from represent import Modifiers, represent
 
-from multithreading import Caller, multi_threaded_call
-
-from cryptofeed.defines import L2_BOOK
+from cryptofeed import FeedHandler
+from cryptofeed.feed import Feed
 
+from crypto_screening.validate import validate_exchange, validate_symbol
 from crypto_screening.process import find_string_value
-from crypto_screening.dataset import save_dataset, load_dataset, DATE_TIME
+from crypto_screening.exchanges import EXCHANGES, EXCHANGE_NAMES
 from crypto_screening.symbols import Separator
-from crypto_screening.validate import validate_exchange, validate_symbol
-from crypto_screening.market.foundation.state import WaitingState
-from crypto_screening.market.foundation.waiting import (
-    base_wait_for_initialization, base_wait_for_dynamic_initialization,
-    base_wait_for_dynamic_update, base_wait_for_update
+from crypto_screening.market.screeners.base import (
+    BaseMultiScreener, BaseScreener
 )
-from crypto_screening.market.foundation.data import DataCollector
 
 __all__ = [
-    "BaseScreener",
-    "BaseMultiScreener",
+    "MarketHandler",
+    "ExchangeFeed",
+    "FEED_GROUP_SIZE",
+    "add_feeds",
+    "MarketScreener",
     "structure_screeners_datasets",
     "structure_screener_datasets",
-    "create_market_dataframe",
     "MarketRecorder",
     "validate_market"
 ]
 
-class BaseScreener(DataCollector):
-    """
-    A class to represent an asset price screener.
-
-    Using this class, you can create a screener object to
-    screen the market ask and bid data for a specific asset in
-    a specific exchange at real time.
-
-    Parameters:
-
-    - symbol:
-        The symbol of an asset to screen.
-
-    - exchange:
-        The name of the exchange platform to screen data from.
-
-    - location:
-        The saving location for the saved data of the screener.
-
-    - cancel:
-        The time to cancel screening process after no new data is fetched.
-
-    - delay:
-        The delay to wait between each data fetching.
-
-    - market:
-        The dataset of the market data.
-    """
-
-    __modifiers__ = Modifiers(**DataCollector.__modifiers__)
-    __modifiers__.hidden.append("market")
-
-    __slots__ = "symbol", "exchange", "market"
-
-    def __init__(
-            self,
-            symbol: str,
-            exchange: str,
-            location: Optional[str] = None,
-            cancel: Optional[Union[float, dt.timedelta]] = None,
-            delay: Optional[Union[float, dt.timedelta]] = None,
-            market: Optional[pd.DataFrame] = None,
-    ) -> None:
-        """
-        Defines the class attributes.
-
-        :param symbol: The symbol of the asset.
-        :param exchange: The exchange to get source data from.
-        :param location: The saving location for the data.
-        :param delay: The delay for the process.
-        :param cancel: The cancel time for the loops.
-        :param market: The data for the market.
-        """
+class MarketHandler(FeedHandler):
+    """A class to handle the market data feed."""
 
-        super().__init__(location=location, cancel=cancel, delay=delay)
+    def __init__(self) -> None:
+        """Defines the class attributes."""
 
-        self.exchange = self.validate_exchange(exchange=exchange)
-        self.symbol = self.validate_symbol(
-            exchange=self.exchange, symbol=symbol
+        super().__init__(
+            config={'uvloop': False, 'log': {'disabled': True}}
         )
-
-        if market is None:
-            market = create_market_dataframe()
-        # end if
-
-        self.market = market
     # end __init__
+# end MarketHandler
 
-    def wait_for_initialization(
-            self,
-            stop: Optional[Union[bool, int]] = False,
-            delay: Optional[Union[float, dt.timedelta]] = None,
-            cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None
-    ) -> WaitingState:
-        """
-        Waits for all the create_screeners to update.
-
-        :param delay: The delay for the waiting.
-        :param stop: The value to stop the screener objects.
-        :param cancel: The time to cancel the waiting.
+class ExchangeFeed(Feed):
+    """A class to represent an exchange feed object."""
 
-        :returns: The total delay.
-        """
+    handler: Optional[FeedHandler] = None
 
-        return base_wait_for_initialization(
-            self, stop=stop, delay=delay, cancel=cancel
-        )
-    # end base_wait_for_initialization
-
-    def wait_for_update(
-            self,
-            stop: Optional[Union[bool, int]] = False,
-            delay: Optional[Union[float, dt.timedelta]] = None,
-            cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None
-    ) -> WaitingState:
-        """
-        Waits for all the create_screeners to update.
+    running: bool = False
 
-        :param delay: The delay for the waiting.
-        :param stop: The value to stop the screener objects.
-        :param cancel: The time to cancel the waiting.
+    def stop(self) -> None:
+        """Stops the process."""
 
-        :returns: The total delay.
-        """
+        self.running = False
 
-        return base_wait_for_update(
-            self, stop=stop, delay=delay, cancel=cancel
-        )
-    # end base_wait_for_update
+        Feed.stop(self)
+    # end stop
 
-    @staticmethod
-    def validate_exchange(exchange: str) -> str:
+    def start(self, loop: asyncio.AbstractEventLoop) -> None:
         """
-        Validates the symbol value.
+        Create tasks for exchange interfaces and backends.
 
-        :param exchange: The exchange name.
-
-        :return: The validates symbol.
+        :param loop: The event loop for the process.
         """
 
-        return validate_exchange(exchange=exchange)
-    # end validate_exchange
-
-    @staticmethod
-    def validate_symbol(exchange: str, symbol: Any) -> str:
-        """
-        Validates the symbol value.
+        self.running = True
 
-        :param exchange: The exchange name.
-        :param symbol: The name of the symbol.
+        Feed.start(self, loop=loop)
+    # end start
+# end ExchangeFeed
 
-        :return: The validates symbol.
-        """
 
-        return validate_symbol(exchange=exchange, symbol=symbol)
-    # end validate_symbol
+FEED_GROUP_SIZE = 20
 
-    def dataset_path(self, location: Optional[str] = None) -> str:
-        """
-        Creates the path to the saving file for the screener object.
+def add_feeds(
+        handler: FeedHandler,
+        data: Dict[str, Iterable[str]],
+        fixed: Optional[bool] = False,
+        amount: Optional[int] = FEED_GROUP_SIZE,
+        separator: Optional[str] = None,
+        parameters: Optional[Union[Dict[str, Dict[str, Any]], Dict[str, Any]]] = None
+) -> None:
+    """
+    Adds the symbols to the handler for each exchange.
 
-        :param location: The saving location of the dataset.
+    :param handler: The handler object.
+    :param data: The data of the exchanges and symbols to add.
+    :param parameters: The parameters for the exchanges.
+    :param fixed: The value for fixed parameters to all exchanges.
+    :param separator: The separator of the assets.
+    :param amount: The maximum amount of symbols for each feed.
+    """
 
-        :return: The saving path for the dataset.
-        """
+    base_parameters = None
 
-        location = location or self.location
+    if not fixed:
+        parameters = parameters or {}
 
-        if location is None:
-            location = "."
-        # end if
+    else:
+        base_parameters = parameters or {}
+        parameters = {}
+    # end if
 
-        return (
-            f"{location}/"
-            f"{self.exchange.lower()}/"
-            f"{self.symbol.replace(Separator.value, '-')}.csv"
-        )
-    # end dataset_path
+    if separator is None:
+        separator = Separator.value
+    # end if
 
-    def save_dataset(self, location: Optional[str] = None) -> None:
-        """
-        Saves the data of the screener.
+    for exchange, symbols in data.items():
+        exchange = find_string_value(value=exchange, values=EXCHANGE_NAMES)
 
-        :param location: The saving location of the dataset.
-        """
+        symbols = [
+            symbol.replace(separator, '-')
+            for symbol in symbols
+        ]
 
-        if len(self.market) == 0:
-            return
+        if fixed:
+            parameters.setdefault(exchange, base_parameters)
         # end if
 
-        save_dataset(
-            dataset=self.market,
-            path=self.dataset_path(location=location)
-        )
-    # end save_dataset
-
-    def load_dataset(self, location: Optional[str] = None) -> None:
-        """
-        Saves the data of the screener.
-
-        :param location: The saving location of the dataset.
-        """
+        EXCHANGES[exchange]: Type[ExchangeFeed]
 
-        data = load_dataset(path=self.dataset_path(location=location))
+        packets = []
 
-        for index, data in zip(data.index[:], data.loc[:]):
-            self.market.loc[index] = data
+        for i in range(0, int(len(symbols) / amount) + len(symbols) % amount, amount):
+            packets.append(symbols[i:])
         # end for
-    # end load_dataset
-
-    def saving_loop(self) -> None:
-        """Runs the process of the price screening."""
-
-        self._saving = True
-
-        delay = self.delay
 
-        if isinstance(self.delay, dt.timedelta):
-            delay = delay.total_seconds()
-        # end if
-
-        while self.saving:
-            start = time.time()
-
-            self.save_dataset()
-
-            end = time.time()
-
-            time.sleep(max([delay - (end - start), 1]))
-        # end while
-    # end saving_loop
-# end BaseScreener
+        for symbols_packet in packets:
+            feed = EXCHANGES[exchange](
+                symbols=symbols_packet,
+                **(
+                    parameters[exchange]
+                    if (
+                        (exchange in parameters) and
+                        isinstance(parameters[exchange], dict) and
+                        all(isinstance(key, str) for key in parameters)
 
-def create_market_dataframe(columns: Optional[Iterable[str]] = None) -> pd.DataFrame:
-    """
-    Creates a dataframe for the order book data.
-
-    :param columns: The dataset columns.
-
-    :return: The dataframe.
-    """
-
-    market = pd.DataFrame(
-        {column: [] for column in columns or []}, index=[]
-    )
-    market.index.name = DATE_TIME
+                    ) else {}
+                )
+            )
 
-    return market
-# end create_market_dataframe
+            feed.start = partial(ExchangeFeed.start, feed)
+            feed.stop = partial(ExchangeFeed.stop, feed)
+            feed.handler = handler
+            feed.running = False
 
-RecorderParameters = Dict[str, Union[Iterable[str], Dict[str, Callable]]]
+            handler.add_feed(feed)
+        # end for
+    # end for
+# end add_feeds
 
 Market = Dict[str, Dict[str, Any]]
 
 def validate_market(data: Any) -> Market:
     """
     Validates the data.
 
@@ -281,22 +171,22 @@
     try:
         if not isinstance(data, dict):
             raise ValueError
         # end if
 
         for exchange, values in data.items():
             if not (
-                isinstance(exchange, str) and
-                (
-                    isinstance(values, dict) and
-                    all(
-                        isinstance(symbol, str)
-                        for symbol, _ in values.items()
+                    isinstance(exchange, str) and
+                    (
+                            isinstance(values, dict) and
+                            all(
+                                isinstance(symbol, str)
+                                for symbol, _ in values.items()
+                            )
                     )
-                )
             ):
                 raise ValueError
             # end if
         # end for
 
     except (TypeError, ValueError):
         raise ValueError(
@@ -318,15 +208,15 @@
 
     - market:
         The market structure of the data to store the fetched data in.
         This structure is a dictionary with exchange names as keys
         and dictionaries as values, where their keys are symbols,
         and their values are the dataframes to record the data.
 
-    >>> from crypto_screening.market.screeners.base import MarketRecorder
+    >>> from crypto_screening.market.screeners.recorder import MarketRecorder
     >>>
     >>> market = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
     >>>
     >>> recorder = MarketRecorder(data=market)
 
     """
 
@@ -341,41 +231,37 @@
 
         :param market: The object to fill with the crypto feed record.
         """
 
         self.market = self.validate_market(data=market)
     # end __init__
 
-    def parameters(self) -> RecorderParameters:
-        """
-        Returns the order book parameters.
-
-        :return: The order book parameters.
-        """
-
-        return dict(
-            channels=[L2_BOOK],
-            callbacks={L2_BOOK: self.record},
-            max_depth=1
-        )
-    # end parameters
-
     @staticmethod
     def validate_market(data: Any) -> Market:
         """
         Validates the data.
 
         :param data: The data to validate.
 
         :return: The valid data.
         """
 
         return validate_market(data=data)
     # end validate_market
 
+    def parameters(self) -> Dict[str, Any]:
+        """
+        Returns the order book parameters.
+
+        :return: The order book parameters.
+        """
+
+        raise NotImplemented
+    # end parameters
+
     def structure(self) -> Dict[str, List[str]]:
         """
         Returns the structure of the market data.
 
         :return: The structure of the market.
         """
 
@@ -433,15 +319,15 @@
 
         except ValueError:
             return False
         # end try
     # end in_market
 # end MarketRecorder
 
-class BaseMultiScreener(DataCollector):
+class MarketScreener(BaseMultiScreener):
     """
     A class to represent an asset price screener.
 
     Using this class, you can create a screener object to
     screen the market ask and bid data for a specific asset in
     a specific exchange at real time.
 
@@ -451,168 +337,361 @@
         The saving location for the saved data of the screener.
 
     - cancel:
         The time to cancel screening process after no new data is fetched.
 
     - delay:
         The delay to wait between each data fetching.
+
+    - handler:
+        The handler object to handle the data feed.
+
+    - recorder:
+        The recorder object to record the data of the market from the feed.
     """
 
-    __modifiers__ = Modifiers(**DataCollector.__modifiers__)
-    __modifiers__.hidden.extend(["screeners", 'recorder'])
+    __modifiers__ = Modifiers(**BaseMultiScreener.__modifiers__)
+    __modifiers__.excluded.extend(
+        ['_run_parameters', '_feeds_parameters', 'handler']
+    )
+
+    __slots__ = (
+        "handler", 'amount', "loop", "limited", "_feeds_parameters",
+        "_run_parameters", 'refresh'
+    )
 
     screeners: List[BaseScreener]
+    recorder: MarketRecorder
 
-    __slots__ = 'recorder', 'screeners'
+    DELAY = 5
+    AMOUNT = FEED_GROUP_SIZE
+
+    REFRESH = dt.timedelta(minutes=5)
 
     def __init__(
             self,
-            recorder: MarketRecorder,
             screeners: Optional[Iterable[BaseScreener]] = None,
             location: Optional[str] = None,
             cancel: Optional[Union[float, dt.timedelta]] = None,
-            delay: Optional[Union[float, dt.timedelta]] = None
+            delay: Optional[Union[float, dt.timedelta]] = None,
+            refresh: Optional[Union[float, dt.timedelta, bool]] = None,
+            limited: Optional[bool] = None,
+            handler: Optional[FeedHandler] = None,
+            amount: Optional[int] = None,
+            recorder: Optional[MarketRecorder] = None
     ) -> None:
         """
-        Defines the class attributes.
+        Creates the class attributes.
 
         :param location: The saving location for the data.
         :param delay: The delay for the process.
         :param cancel: The cancel time for the loops.
+        :param limited: The value to limit the screeners to active only.
+        :param refresh: The refresh time for rerunning.
+        :param handler: The handler object for the market data.
+        :param amount: The maximum amount of symbols for each feed.
+        :param recorder: The recorder object for recording the data.
         """
 
-        super().__init__(location=location, cancel=cancel, delay=delay)
+        super().__init__(
+            location=location, cancel=cancel,
+            delay=delay, screeners=screeners
+        )
 
-        self.screeners = list(screeners or [])
+        if refresh is True:
+            refresh = self.REFRESH
+        # end if
 
         self.recorder = recorder
+        self.handler = handler or MarketHandler()
+        self.limited = limited or False
+        self.amount = amount or self.AMOUNT
+        self.refresh = refresh
+
+        self.loop: Optional[asyncio.AbstractEventLoop] = None
+
+        self._feeds_parameters: Optional[Dict[str, Any]] = None
+        self._run_parameters: Optional[Dict[str, Any]] = None
     # end __init__
 
-    @property
-    def market(self) -> Dict[str, Dict[str, pd.DataFrame]]:
+    def structure(self) -> Dict[str, List[str]]:
         """
-        Returns the market to hold the recorder data.
+        Returns the structure of the market data.
 
-        :return: The market object.
+        :return: The structure of the market.
         """
 
-        return self.recorder.market
-    # end market
+        return self.recorder.structure()
+    # end structure
 
-    def wait_for_initialization(
+    def add_feeds(
             self,
-            stop: Optional[Union[bool, int]] = False,
-            delay: Optional[Union[float, dt.timedelta]] = None,
-            cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None
-    ) -> WaitingState:
+            data: Dict[str, Iterable[str]],
+            fixed: Optional[bool] = True,
+            separator: Optional[str] = None,
+            amount: Optional[int] = None,
+            parameters: Optional[Union[Dict[str, Dict[str, Any]], Dict[str, Any]]] = None
+    ) -> None:
         """
-        Waits for all the create_screeners to update.
-
-        :param delay: The delay for the waiting.
-        :param stop: The value to stop the screener objects.
-        :param cancel: The time to cancel the waiting.
+        Adds the symbols to the handler for each exchange.
 
-        :returns: The total delay.
+        :param data: The data of the exchanges and symbols to add.
+        :param parameters: The parameters for the exchanges.
+        :param fixed: The value for fixed parameters to all exchanges.
+        :param amount: The maximum amount of symbols for each feed.
+        :param separator: The separator of the assets.
         """
 
-        return base_wait_for_dynamic_initialization(
-            self.screeners, stop=stop, delay=delay, cancel=cancel
+        self._feeds_parameters = dict(
+            data=data, fixed=fixed, separator=separator,
+            parameters=parameters
         )
-    # end base_wait_for_initialization
 
-    def wait_for_update(
-            self,
-            stop: Optional[Union[bool, int]] = False,
-            delay: Optional[Union[float, dt.timedelta]] = None,
-            cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None
-    ) -> WaitingState:
-        """
-        Waits for all the create_screeners to update.
+        feed_params = self.recorder.parameters()
+        feed_params.update(parameters or {})
 
-        :param delay: The delay for the waiting.
-        :param stop: The value to stop the screener objects.
-        :param cancel: The time to cancel the waiting.
+        add_feeds(
+            self.handler, data=data, fixed=fixed, separator=separator,
+            parameters=feed_params, amount=amount or self.amount
+        )
+    # end add_feeds
 
-        :returns: The total delay.
-        """
+    def refresh_feeds(self) -> None:
+        """Refreshes the feed objects."""
 
-        return base_wait_for_dynamic_update(
-            self.screeners, stop=stop, delay=delay, cancel=cancel
-        )
-    # end base_wait_for_update
+        if self._feeds_parameters is None:
+            warnings.warn(
+                "Cannot refresh feeds as there was "
+                "no feeds initialization to repeat."
+            )
 
-    def connect_screeners(self) -> None:
-        """Connects the screeners to the recording object."""
+            return
+        # end if
 
-        for screener in self.screeners:
-            screener.market = self.recorder.data(
-                exchange=screener.exchange, symbol=screener.symbol
+        self.handler.feeds.clear()
+
+        self.add_feeds(**self._feeds_parameters)
+    # end refresh
+
+    def rerun(self) -> None:
+        """Refreshes the process."""
+
+        if self._run_parameters is None:
+            warnings.warn(
+                "Cannot rerun as there was "
+                "no initial process to repeat."
             )
-        # end for
-    # end connect_screeners
 
-    def in_market(self, exchange: str, symbol: str) -> bool:
+            return
+        # end if
+
+        self.terminate()
+        self.refresh_feeds()
+        self.run(**self._run_parameters)
+    # end rerun
+
+    def orderbook(self, exchange: str, symbol: str) -> pd.DataFrame:
         """
         Returns the market data of the symbol from the exchange.
 
         :param exchange: The source name of the exchange.
         :param symbol: The symbol of the pair.
 
         :return: The dataset of the spread data.
         """
 
-        return self.recorder.in_market(exchange=exchange, symbol=symbol)
-    # end in_market
+        return self.recorder.orderbook(exchange=exchange, symbol=symbol)
+    # end orderbook
 
-    def save_datasets(self, location: Optional[str] = None) -> None:
+    def screening_loop(
+            self,
+            start: Optional[bool] = True,
+            loop: Optional[asyncio.AbstractEventLoop] = None
+    ) -> None:
         """
-        Runs the data handling loop.
+        Runs the process of the price screening.
 
-        :param location: The saving location.
+        :param start: The value to start the loop.
+        :param loop: The event loop.
         """
 
-        callers = []
+        if loop is None:
+            loop = asyncio.new_event_loop()
+        # end if
+
+        self.loop = loop
+
+        asyncio.set_event_loop(loop)
+
+        self._screening = True
 
         for screener in self.screeners:
-            location = location or screener.location or self.location
+            screener._screening = True
+        # end for
 
-            callers.append(
-                Caller(
-                    target=screener.save_dataset,
-                    kwargs=dict(location=location)
-                )
+        self.handler.run(
+            start_loop=start and (not loop.is_running()),
+            install_signal_handlers=False
+        )
+    # end screening_loop
+
+    def saving_loop(self) -> None:
+        """Runs the process of the price screening."""
+
+        for screener in self.screeners:
+            screener._saving_process = threading.Thread(
+                target=screener.saving_loop
             )
+            screener._saving_process.start()
         # end for
+    # end saving_loop
 
-        multi_threaded_call(callers=callers)
-    # end save_datasets
+    def update_loop(self) -> None:
+        """Updates the state of the screeners."""
 
-    def load_datasets(self, location: Optional[str] = None) -> None:
-        """
-        Runs the data handling loop.
+        self._updating = True
 
-        :param location: The saving location.
-        """
+        refresh = self.refresh
+
+        if isinstance(refresh, dt.timedelta):
+            refresh = refresh.total_seconds()
+        # end if
+
+        start = time.time()
+
+        while self.updating:
+            s = time.time()
+
+            if self.screening:
+                self.update()
+
+                current = time.time()
+
+                if refresh and ((current - start) >= refresh):
+                    self.rerun()
+
+                    start = current
+                # end if
+            # end if
+
+            time.sleep(max([self.delay - (time.time() - s), 0]))
+        # end while
+    # end update_loop
 
-        callers = []
+    def update(self) -> None:
+        """Updates the state of the screeners."""
 
         for screener in self.screeners:
-            location = location or screener.location or self.location
+            for feed in self.handler.feeds:
+                feed: ExchangeFeed
 
-            callers.append(
-                Caller(
-                    target=screener.load_dataset,
-                    kwargs=dict(location=location)
-                )
-            )
+                if (
+                    self.limited and
+                    (screener.exchange.lower() == feed.id.lower()) and
+                    (not feed.running)
+                ):
+                    screener.stop()
+                # end if
+            # end for
+        # end for
+    # end update
+
+    def stop(self) -> None:
+        """Stops the data handling loop."""
+
+        super().stop()
+
+        self.loop: asyncio.AbstractEventLoop
+
+        async def stop() -> None:
+            """Stops the handler."""
+
+            self.handler.stop(self.loop)
+            self.handler.close(self.loop)
+        # end stop
+
+        self.loop.create_task(stop())
+
+        for task in asyncio.all_tasks(self.loop):
+            task.cancel()
         # end for
 
-        multi_threaded_call(callers=callers)
-    # end load_datasets
-# end BaseScreener
+        self.loop = None
+
+        self.handler.running = False
+    # end stop
+
+    def start_screening(
+            self,
+            start: Optional[bool] = True,
+            loop: Optional[asyncio.AbstractEventLoop] = None
+    ) -> None:
+        """
+        Starts the screening process.
+
+        :param start: The value to start the loop.
+        :param loop: The event loop.
+        """
+
+        if self.screening:
+            warnings.warn(f"Timeout process of {self} is already running.")
+
+            return
+        # end if
+
+        self._screening_process = threading.Thread(
+            target=lambda: self.screening_loop(loop=loop, start=start)
+        )
+
+        self._screening_process.start()
+    # end start_screening
+
+    def run(
+            self,
+            save: Optional[bool] = True,
+            block: Optional[bool] = False,
+            update: Optional[bool] = True,
+            screen: Optional[bool] = True,
+            loop: Optional[asyncio.AbstractEventLoop] = None,
+            wait: Optional[Union[bool, float, dt.timedelta, dt.datetime]] = False,
+            timeout: Optional[Union[float, dt.timedelta, dt.datetime]] = None,
+    ) -> None:
+        """
+        Runs the program.
+
+        :param save: The value to save the data.
+        :param wait: The value to wait after starting to run the process.
+        :param block: The value to block the execution.
+        :param timeout: The valur to add a start_timeout to the process.
+        :param update: The value to update the screeners.
+        :param screen: The value to start the loop.
+        :param loop: The event loop.
+
+        :return: The start_timeout process.
+        """
+
+        self._run_parameters = dict(
+            save=save, block=block, update=update, screen=screen,
+            loop=loop, wait=wait, timeout=timeout
+        )
+
+        if not block:
+            self.start_screening(loop=loop, start=screen)
+        # end if
+
+        super().run(
+            screen=False, block=False, wait=wait,
+            timeout=timeout, update=update, save=save
+        )
+
+        if block:
+            self.screening_loop(loop=loop, start=screen)
+        # end if
+    # end run
+# end MarketScreener
 
 def structure_screeners_datasets(
         screeners: Iterable[BaseScreener]
 ) -> Dict[str, Dict[str, List[pd.DataFrame]]]:
     """
     Structures the screener objects by exchanges and symbols
```

### Comparing `crypto-screening-3.7.0/crypto_screening/market/screeners/container.py` & `crypto-screening-4.0.0/crypto_screening/market/screeners/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 # container.py
 
 from typing import Iterable, List
 
 from represent import Modifiers
 
-from crypto_screening.market.screeners.base import (
-    BaseScreener, structure_screener_datasets
-)
-from crypto_screening.market.screeners import (
-    MarketRecorder, OrderbookScreener, OHLCVScreener
+from crypto_screening.market.screeners.recorder import (
+    structure_screener_datasets, MarketRecorder
 )
+from crypto_screening.market.screeners.base import BaseScreener
+from crypto_screening.market.screeners.ohlcv import OHLCVScreener
+from crypto_screening.market.screeners.orderbook import OrderbookScreener
 
 class ScreenersContainer(MarketRecorder):
     """
     A class to represent a multi-exchange multi-pairs crypto data screener.
     Using this class enables extracting screener objects and screeners
     data by the exchange name and the symbol of the pair.
 
     parameters:
 
     - screeners:
         The screener objects.
 
-    - data:
-        The structure of the screeners, by exchanges and symbols.
-
     >>> from crypto_screening.market.screeners.container import ScreenersContainer
     >>> from crypto_screening.market.screeners.base import BaseScreener
     >>>
     >>> dynamic_screener = ScreenersContainer(
     >>>     screeners=[BaseScreener(exchange="binance", symbol="BTC/USDT")]
     >>> )
     >>>
```

### Comparing `crypto-screening-3.7.0/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-4.0.0/crypto_screening/market/screeners/ohlcv.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,32 +8,29 @@
 import pandas as pd
 
 from represent import Modifiers
 
 from cryptofeed import FeedHandler
 from cryptofeed.types import OrderBook
 
+from crypto_screening.process import find_string_value
 from crypto_screening.interval import interval_to_total_time
 from crypto_screening.dataset import (
-    OHLCV_COLUMNS, OPEN, HIGH, LOW, CLOSE, VOLUME,
-    BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME
+    OHLCV_COLUMNS, VOLUME, BIDS, BIDS_VOLUME,
+    load_dataset, save_dataset, OHLC_COLUMNS, create_market_dataframe
 )
+from crypto_screening.validate import validate_interval
 from crypto_screening.symbols import adjust_symbol
-from crypto_screening.market.screeners.base import (
-    BaseScreener, structure_screener_datasets
-)
-from crypto_screening.market.screeners.recorder import MarketScreener
-from crypto_screening.market.screeners.base import (
-    create_market_dataframe, MarketRecorder, validate_market
+from crypto_screening.market.screeners.recorder import (
+    structure_screener_datasets, MarketRecorder, validate_market
 )
 from crypto_screening.market.screeners.orderbook import (
-    create_orderbook_dataframe, OrderbookScreener,
-    OrderbookMarketScreener, create_orderbook_market
+    create_orderbook_dataframe, OrderbookScreener, record_orderbook,
+    OrderbookMarketScreener, create_orderbook_market, OrderbookMarketRecorder
 )
-from crypto_screening.process import find_string_value
 
 __all__ = [
     "OHLCVMarketScreener",
     "OHLCVMarketRecorder",
     "OHLCVScreener",
     "create_ohlcv_market",
     "ohlcv_market_screener",
@@ -83,15 +80,15 @@
         exchange.lower(): {
             symbol.upper(): [interval]
             for symbol in symbols
         } for exchange, symbols in data.items()
     }
 # end datasets_to_intervals_datasets
 
-class OHLCVScreener(BaseScreener):
+class OHLCVScreener(OrderbookScreener):
     """
     A class to represent an asset price screener.
 
     Using this class, you can create a screener object to
     screen the market ask and bid data for a specific asset in
     a specific exchange at real time.
 
@@ -135,46 +132,153 @@
             market: Optional[pd.DataFrame] = None,
             base_market: Optional[pd.DataFrame] = None
     ) -> None:
         """
         Defines the class attributes.
 
         :param symbol: The symbol of the asset.
+        :param interval: The interval for the data.
         :param exchange: The exchange to get source data from.
         :param location: The saving location for the data.
         :param delay: The delay for the process.
         :param cancel: The cancel time for the loops.
         :param market: The data for the market.
         :param base_market: The base market dataset.
         """
 
         super().__init__(
             symbol=symbol, exchange=exchange, location=location,
             cancel=cancel, delay=delay, market=market
         )
 
-        self.interval = interval or self.INTERVAL
+        self.interval = self.validate_interval(interval or self.INTERVAL)
 
         self.base_market = base_market
     # end __init__
 
-    def dataset_path(self, location: Optional[str] = None) -> str:
+    @staticmethod
+    def validate_interval(interval: str) -> str:
+        """
+        Validates the symbol value.
+
+        :param interval: The interval for the data.
+
+        :return: The validates symbol.
+        """
+
+        return validate_interval(interval=interval)
+    # end validate_symbol
+
+    @property
+    def orderbook_market(self) -> pd.DataFrame:
+        """
+        Returns the market to hold the recorder data.
+
+        :return: The market object.
+        """
+
+        return self.base_market
+    # end orderbook_market
+
+    @property
+    def ohlcv_market(self) -> pd.DataFrame:
+        """
+        Returns the market to hold the recorder data.
+
+        :return: The market object.
+        """
+
+        return self.market
+    # end ohlcv_market
+
+    def ohlcv_dataset_path(self, location: Optional[str] = None) -> str:
         """
         Creates the path to the saving file for the screener object.
 
         :param location: The saving location of the dataset.
 
         :return: The saving path for the dataset.
         """
 
         return (
-            super().dataset_path(location=location).
+            self.dataset_path(location=location).
             replace(".csv", f"-{self.interval}.csv")
         )
-    # end dataset_path
+    # end ohlcv_dataset_path
+
+    def save_ohlcv_dataset(self, location: Optional[str] = None) -> None:
+        """
+        Saves the data of the screener.
+
+        :param location: The saving location of the dataset.
+        """
+
+        if len(self.ohlcv_market) > 0:
+            save_dataset(
+                dataset=self.ohlcv_market,
+                path=self.ohlcv_dataset_path(location=location)
+            )
+        # end if
+    # end save_ohlcv_dataset
+
+    def save_datasets(self, location: Optional[str] = None) -> None:
+        """
+        Saves the data of the screener.
+
+        :param location: The saving location of the dataset.
+        """
+
+        self.save_ohlcv_dataset(location=location)
+        self.save_orderbook_dataset(location=location)
+    # end save_datasets
+
+    def save_dataset(self, location: Optional[str] = None) -> None:
+        """
+        Saves the data of the screener.
+
+        :param location: The saving location of the dataset.
+        """
+
+        self.save_datasets(location=location)
+    # end save_dataset
+
+    def load_ohlcv_dataset(self, location: Optional[str] = None) -> None:
+        """
+        Saves the data of the screener.
+
+        :param location: The saving location of the dataset.
+        """
+
+        data = load_dataset(path=self.ohlcv_dataset_path(location=location))
+
+        for index, data in zip(data.index[:], data.loc[:]):
+            self.market.loc[index] = data
+        # end for
+    # end load_ohlcv_dataset
+
+    def load_datasets(self, location: Optional[str] = None) -> None:
+        """
+        Saves the data of the screener.
+
+        :param location: The saving location of the dataset.
+        """
+
+        self.load_ohlcv_dataset(location=location)
+        self.load_orderbook_dataset(location=location)
+    # end load_datasets
+
+    def load_dataset(self, location: Optional[str] = None) -> None:
+        """
+        Saves the data of the screener.
+
+        :param location: The saving location of the dataset.
+        """
+
+        self.load_datasets(location=location)
+    # end load_dataset
 
     def orderbook_screener(self) -> OrderbookScreener:
         """
         Creates the orderbook screener object.
 
         :return: The orderbook screener.
         """
@@ -368,15 +472,78 @@
     return dict(
         market=market,
         ohlcv_market=ohlcv_market,
         intervals=intervals
     )
 # end create_ohlcv_market_recorder_initializers
 
-class OHLCVMarketRecorder(MarketRecorder):
+def record_ohlcv(
+        market: Market,
+        ohlcv_market: OHLCVMarket,
+        indexes: Indexes,
+        data: OrderBook,
+        timestamp: float
+) -> bool:
+    """
+    Records the data from the crypto feed into the dataset.
+
+    :param market: The market structure.
+    :param ohlcv_market: The OHLCV market structure.
+    :param indexes: The indexes of the OHLCV market.
+    :param data: The data from the exchange.
+    :param timestamp: The time of the request.
+    """
+
+    if not record_orderbook(market=market, data=data, timestamp=timestamp):
+        return False
+    # end if
+
+    exchange = find_string_value(
+        value=data.exchange, values=market.keys()
+    )
+    symbol = find_string_value(
+        value=adjust_symbol(symbol=data.symbol),
+        values=exchange
+    )
+
+    spread = market[exchange][symbol]
+
+    for interval, ohlcv_dataset in ohlcv_market[exchange][symbol].items():
+        dataset_index = (
+            indexes.
+            setdefault(exchange, {}).
+            setdefault(symbol, {}).
+            setdefault(interval, 0)
+        )
+
+        span: dt.timedelta = spread.index[-1] - spread.index[dataset_index]
+
+        interval_total_time = interval_to_total_time(interval)
+
+        if (span >= interval_total_time) or (dataset_index == 0):
+            interval_total_minutes = interval_total_time.total_seconds() // 60
+            adjuster = f'{interval_total_minutes}Min'
+
+            ohlcv: pd.DataFrame = spread[BIDS].resample(adjuster).ohlc()
+            ohlcv.columns = list(OHLC_COLUMNS)
+            volume: pd.DataFrame = spread[BIDS_VOLUME].resample(adjuster).ohlc()
+            ohlcv[VOLUME] = volume[list(volume.columns)[-1]]
+
+            for index, row in ohlcv.iterrows():
+                ohlcv_dataset.loc[index] = row
+            # end for
+
+            indexes[exchange][symbol][interval] += 1
+        # end for
+    # end for
+
+    return True
+# end record_ohlcv
+
+class OHLCVMarketRecorder(OrderbookMarketRecorder):
     """
     A class to represent a crypto data feed recorder.
     This object passes the record method to the handler object to record
     the data fetched by the handler.
 
     Parameters:
 
@@ -396,15 +563,15 @@
     >>>
     >>> recorder = ohlcv_market_recorder(data=market)
     """
 
     __modifiers__ = Modifiers(**MarketRecorder.__modifiers__)
     __modifiers__.hidden.extend(["intervals", "ohlcv_market"])
 
-    __slots__ = "_index", "ohlcv_market", "intervals"
+    __slots__ = "_indexes", "ohlcv_market", "intervals"
 
     COLUMNS = OHLCV_COLUMNS
     INTERVAL = OHLCVScreener.INTERVAL
 
     def __init__(
             self,
             intervals: Optional[Intervals] = None,
@@ -426,17 +593,17 @@
         market = data["market"]
         intervals = data["intervals"]
         ohlcv_market = data["ohlcv_market"]
 
         super().__init__(market=market)
 
         self.intervals = self.validate_intervals(intervals)
-        self.ohlcv_market = self.validate_market(ohlcv_market)
+        self.ohlcv_market = self.validate_ohlcv_market(ohlcv_market)
 
-        self._index: Indexes = {}
+        self._indexes: Indexes = {}
     # end __init__
 
     @staticmethod
     def validate_ohlcv_market(data: Any) -> OHLCVMarket:
         """
         Validates the data.
 
@@ -485,106 +652,47 @@
                 f"Valid symbols: {', '.join(intervals.keys() or [])} for {self}."
             )
         # end if
 
         return intervals[interval]
     # end ohlcv
 
-    def orderbook(self, exchange: str, symbol: str) -> pd.DataFrame:
+    def ohlcv_in_market(self, exchange: str, symbol: str, interval: str) -> bool:
         """
         Returns the market data of the symbol from the exchange.
 
         :param exchange: The source name of the exchange.
         :param symbol: The symbol of the pair.
+        :param interval: The interval for the dataset.
 
         :return: The dataset of the spread data.
         """
 
-        return self.data(exchange=exchange, symbol=symbol)
-    # end orderbook
+        try:
+            self.ohlcv(exchange=exchange, symbol=symbol, interval=interval)
 
-    async def record(self, data: OrderBook, timestamp: float) -> None:
+            return True
+
+        except ValueError:
+            return False
+        # end try
+    # end ohlcv_in_market
+
+    async def record(self, data: OrderBook, timestamp: float) -> bool:
         """
         Records the data from the crypto feed into the dataset.
 
         :param data: The data from the exchange.
         :param timestamp: The time of the request.
         """
 
-        exchange = find_string_value(
-            value=data.exchange, values=self.market.keys()
-        )
-        symbol = find_string_value(
-            value=adjust_symbol(symbol=data.symbol),
-            values=exchange
-        )
-
-        spread_dataset = (
-            self.market.
-            setdefault(exchange, {}).
-            setdefault(symbol, create_orderbook_dataframe())
+        return record_ohlcv(
+            market=self.market, ohlcv_market=self.ohlcv_market,
+            indexes=self._indexes, data=data, timestamp=timestamp
         )
-
-        bids = data.book.bids.to_list()
-        asks = data.book.asks.to_list()
-
-        try:
-            current_index = dt.datetime.fromtimestamp(timestamp)
-
-            spread_dataset.loc[current_index] = {
-                BIDS: float(bids[0][0]),
-                ASKS: float(asks[0][0]),
-                BIDS_VOLUME: float(bids[0][1]),
-                ASKS_VOLUME: float(asks[0][1])
-            }
-
-        except IndexError:
-            return
-        # end try
-
-        for interval, ohlcv_dataset in (
-            self.ohlcv_market[exchange][symbol].items()
-        ):
-            dataset_index = (
-                self._index.
-                setdefault(exchange, {}).
-                setdefault(symbol, {}).
-                setdefault(interval, 0)
-            )
-
-            span: dt.timedelta = (
-                spread_dataset.index[-1] -
-                spread_dataset.index[dataset_index]
-            )
-
-            interval_total_time = interval_to_total_time(interval)
-
-            if (span >= interval_total_time) or (dataset_index == 0):
-                interval_total_minutes = (
-                    interval_total_time.total_seconds() // 60
-                )
-                adjuster = f'{interval_total_minutes}Min'
-
-                dataset: pd.DataFrame = (
-                    spread_dataset[BIDS].resample(adjuster).ohlc()
-                )
-                dataset.columns = [OPEN, HIGH, LOW, CLOSE]
-                volume: pd.DataFrame = (
-                    spread_dataset[BIDS_VOLUME].resample(adjuster).ohlc()
-                )
-                volume.columns = [OPEN, HIGH, LOW, CLOSE]
-                dataset[VOLUME] = volume[CLOSE]
-
-                for index, row in dataset.iterrows():
-                    ohlcv_dataset.loc[index] = row
-                # end for
-
-                self._index[exchange][symbol][interval] += 1
-            # end for
-        # end if
     # end record
 # end MarketOHLCVRecorder
 
 def structure_screener_intervals(
         screeners: Iterable[OHLCVScreener]
 ) -> Dict[str, Dict[str, List[str]]]:
     """
@@ -630,15 +738,15 @@
             setdefault(screener.interval, screeners)
         )
     # end for
 
     return structure
 # end structure_screeners_intervals
 
-class OHLCVMarketScreener(MarketScreener):
+class OHLCVMarketScreener(OrderbookMarketScreener):
     """
     A class to represent an asset price screener.
 
     Using this class, you can create a screener object to
     screen the market ask and bid data for a specific asset in
     a specific exchange at real time.
 
@@ -710,15 +818,15 @@
         """
 
         screeners = screeners or []
 
         data = create_ohlcv_market_recorder_initializers(
             market=market or structure_screener_datasets(screeners=screeners),
             intervals=intervals or structure_screener_intervals(screeners=screeners),
-            ohlcv_market=ohlcv_market,
+            ohlcv_market=ohlcv_market
         )
 
         market = data["market"]
         intervals = data["intervals"]
         ohlcv_market = data["ohlcv_market"]
 
         super().__init__(
@@ -726,30 +834,27 @@
             delay=delay, recorder=recorder or OHLCVMarketRecorder(
                 market=market, intervals=intervals, ohlcv_market=ohlcv_market
             ),
             screeners=screeners, handler=handler, limited=limited,
             amount=amount, refresh=refresh
         )
 
-        self.screeners[:] = self.screeners or self.create_ohlcv_screeners()
+        self.screeners[:] = screeners or self.create_ohlcv_screeners()
     # end __init__
 
     @property
-    def orderbook_screeners(self) -> List[OrderbookScreener]:
+    def ohlcv_market(self) -> OHLCVMarket:
         """
-        Returns a list of all the order-book screeners.
+        Returns the market to hold the recorder data.
 
-        :return: The order-book screeners.
+        :return: The market object.
         """
 
-        return [
-            screener for screener in self.screeners
-            if isinstance(screener, OrderbookScreener)
-        ]
-    # end orderbook_screeners
+        return self.recorder.ohlcv_market
+    # end ohlcv_market
 
     @property
     def ohlcv_screeners(self) -> List[OHLCVScreener]:
         """
         Returns a list of all the ohlcv screeners.
 
         :return: The ohlcv screeners.
@@ -757,14 +862,63 @@
 
         return [
             screener for screener in self.screeners
             if isinstance(screener, OHLCVScreener)
         ]
     # end ohlcv_screeners
 
+    def connect_screeners(self) -> None:
+        """Connects the screeners to the recording object."""
+
+        super().connect_screeners()
+
+        for screener in self.screeners:
+            if isinstance(screener, OHLCVScreener):
+                screener.base_market = self.recorder.orderbook(
+                    exchange=screener.exchange, symbol=screener.symbol
+                )
+                screener.market = self.recorder.ohlcv(
+                    exchange=screener.exchange, symbol=screener.symbol,
+                    interval=screener.interval
+                )
+        # end for
+    # end connect_screeners
+
+    def ohlcv(self, exchange: str, symbol: str, interval: str) -> pd.DataFrame:
+        """
+        Returns the market data of the symbol from the exchange.
+
+        :param exchange: The source name of the exchange.
+        :param symbol: The symbol of the pair.
+        :param interval: The interval for the dataset.
+
+        :return: The dataset of the spread data.
+        """
+
+        return self.recorder.ohlcv(
+            exchange=exchange, symbol=symbol, interval=interval
+        )
+    # end orderbook
+
+    def ohlcv_in_market(self, exchange: str, symbol: str, interval: str) -> bool:
+        """
+        Returns the market data of the symbol from the exchange.
+
+        :param exchange: The source name of the exchange.
+        :param symbol: The symbol of the pair.
+        :param interval: The interval for the dataset.
+
+        :return: The dataset of the spread data.
+        """
+
+        return self.recorder.ohlcv_in_market(
+            exchange=exchange, symbol=symbol, interval=interval
+        )
+    # end ohlcv_in_market
+
     def create_ohlcv_screener(
             self,
             symbol: str,
             exchange: str,
             interval: Optional[str] = None,
             location: Optional[str] = None,
             cancel: Optional[Union[float, dt.timedelta]] = None,
@@ -798,23 +952,23 @@
         if delay is None:
             delay = self.delay
         # end if
 
         screener = OHLCVScreener(
             symbol=symbol, exchange=exchange, delay=delay,
             location=location, cancel=cancel, market=(
-                self.recorder.ohlcv(
+                self.ohlcv(
                     exchange=exchange, symbol=symbol, interval=interval
-                )
-                if self.in_market(symbol=symbol, exchange=exchange)
-                else None
+                ) if self.ohlcv_in_market(
+                    symbol=symbol, exchange=exchange, interval=interval
+                ) else None
             ),
             base_market=(
-                self.recorder.orderbook(exchange=exchange, symbol=symbol)
-                if self.in_market(symbol=symbol, exchange=exchange)
+                self.orderbook(exchange=exchange, symbol=symbol)
+                if self.orderbook_in_market(symbol=symbol, exchange=exchange)
                 else None
             )
         )
 
         container.setdefault(exchange, {})[symbol] = screener
 
         return screener
@@ -847,16 +1001,16 @@
 
             valid = True
 
         except ValueError:
             valid = False
         # end try
 
-        for exchange in self.market:
-            for symbol in self.market[exchange]:
+        for exchange, symbols in self.structure().items():
+            for symbol in symbols:
                 if valid:
                     interval = intervals[exchange][symbol]
                 # end if
 
                 screeners.append(
                     self.create_ohlcv_screener(
                         symbol=symbol, exchange=exchange, delay=delay,
@@ -865,17 +1019,14 @@
                     )
                 )
             # end for
         # end for
 
         return screeners
     # end create_ohlcv_screeners
-
-    create_orderbook_screener = OrderbookMarketScreener.create_orderbook_screener
-    create_orderbook_screeners = OrderbookMarketScreener.create_orderbook_screeners
 # end MarketOHLCVRecorder
 
 def ohlcv_market_recorder(
         data: Union[Intervals, Dict[str, Iterable[str]]],
         interval: Optional[str] = None
 ) -> OHLCVMarketRecorder:
     """
```

### Comparing `crypto-screening-3.7.0/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-4.0.0/crypto_screening/market/screeners/orderbook.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 # orderbook.py
 
 import datetime as dt
 from typing import (
-    Dict, Optional, Iterable, Any, Union, List
+    Dict, Optional, Iterable, Any, Union, List, Callable
 )
 
 import pandas as pd
 
 from cryptofeed import FeedHandler
 from cryptofeed.types import OrderBook
+from cryptofeed.defines import L2_BOOK
 
-from crypto_screening.dataset import (
-    BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME
-)
 from crypto_screening.symbols import adjust_symbol
-from crypto_screening.market.screeners.base import (
-    BaseScreener, structure_screener_datasets
+from crypto_screening.process import find_string_value
+from crypto_screening.dataset import (
+    BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME, load_dataset,
+    create_market_dataframe, save_dataset
 )
-from crypto_screening.market.screeners.recorder import MarketScreener
-from crypto_screening.market.screeners.base import (
-    create_market_dataframe, MarketRecorder
+from crypto_screening.market.screeners.recorder import MarketRecorder
+from crypto_screening.market.screeners.base import BaseScreener
+from crypto_screening.market.screeners.recorder import (
+    MarketScreener, structure_screener_datasets
 )
-from crypto_screening.process import find_string_value
 
 __all__ = [
     "OrderbookMarketScreener",
     "OrderbookMarketRecorder",
     "OrderbookScreener",
     "create_orderbook_market",
     "orderbook_market_screener",
     "orderbook_market_recorder",
-    "create_orderbook_dataframe"
+    "create_orderbook_dataframe",
+    "record_orderbook"
 ]
 
 Market = Dict[str, Dict[str, pd.DataFrame]]
 
 def create_orderbook_dataframe() -> pd.DataFrame:
     """
     Creates a dataframe for the order book data.
@@ -88,14 +89,86 @@
 
     - delay:
         The delay to wait between each data fetching.
 
     - market:
         The dataset of the market data as BID/ASK spread.
     """
+
+    @property
+    def orderbook_market(self) -> pd.DataFrame:
+        """
+        Returns the market to hold the recorder data.
+
+        :return: The market object.
+        """
+
+        return self.market
+    # end orderbook_market
+
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
+    # end save_ohlcv_dataset
+
+    def save_dataset(self, location: Optional[str] = None) -> None:
+        """
+        Saves the data of the screener.
+
+        :param location: The saving location of the dataset.
+        """
+
+        self.save_orderbook_dataset(location=location)
+    # end save_dataset
+
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
+    def load_dataset(self, location: Optional[str] = None) -> None:
+        """
+        Saves the data of the screener.
+
+        :param location: The saving location of the dataset.
+        """
+
+        self.load_orderbook_dataset(location=location)
+    # end load_dataset
 # end OrderBookScreener
 
 def validate_orderbook_market(data: Any) -> Market:
     """
     Validates the data.
 
     :param data: The data to validate.
@@ -129,14 +202,57 @@
             f"Data must be of type {Market}, not: {data}."
         )
     # end try
 
     return data
 # end validate_orderbook_market
 
+def record_orderbook(market: Market, data: OrderBook, timestamp: float) -> bool:
+    """
+    Records the data from the crypto feed into the dataset.
+
+    :param market: The market structure.
+    :param data: The data from the exchange.
+    :param timestamp: The time of the request.
+    """
+
+    exchange = find_string_value(
+        value=data.exchange, values=market.keys()
+    )
+    symbol = find_string_value(
+        value=adjust_symbol(symbol=data.symbol),
+        values=exchange
+    )
+
+    dataset = (
+        market.
+        setdefault(exchange, {}).
+        setdefault(symbol, create_orderbook_dataframe())
+    )
+
+    bids = data.book.bids.to_list()
+    asks = data.book.asks.to_list()
+
+    try:
+        dataset.loc[dt.datetime.fromtimestamp(timestamp)] = {
+            BIDS: float(bids[0][0]),
+            ASKS: float(asks[0][0]),
+            BIDS_VOLUME: float(bids[0][1]),
+            ASKS_VOLUME: float(asks[0][1])
+        }
+
+        return True
+
+    except IndexError:
+        return False
+    # end try
+# end record_orderbook
+
+RecorderParameters = Dict[str, Union[Iterable[str], Dict[str, Callable]]]
+
 class OrderbookMarketRecorder(MarketRecorder):
     """
     A class to represent a crypto data feed recorder.
     This object passes the record method to the handler object to record
     the data fetched by the handler.
 
     Parameters:
@@ -165,63 +281,83 @@
 
         :return: The valid data.
         """
 
         return validate_orderbook_market(data=data)
     # end validate_market
 
+    @property
+    def orderbook_market(self) -> Market:
+        """
+        Returns the market to hold the recorder data.
+
+        :return: The market object.
+        """
+
+        return self.market
+    # end orderbook_market
+
+    def parameters(self) -> RecorderParameters:
+        """
+        Returns the order book parameters.
+
+        :return: The order book parameters.
+        """
+
+        return dict(
+            channels=[L2_BOOK],
+            callbacks={L2_BOOK: self.record},
+            max_depth=1
+        )
+    # end parameters
+
     def orderbook(self, exchange: str, symbol: str) -> pd.DataFrame:
         """
         Returns the market data of the symbol from the exchange.
 
         :param exchange: The source name of the exchange.
         :param symbol: The symbol of the pair.
 
         :return: The dataset of the spread data.
         """
 
         return self.data(exchange=exchange, symbol=symbol)
     # end orderbook
 
-    async def record(self, data: OrderBook, timestamp: float) -> None:
+    def orderbook_in_market(self, exchange: str, symbol: str) -> bool:
         """
-        Records the data from the crypto feed into the dataset.
+        Returns the market data of the symbol from the exchange.
 
-        :param data: The data from the exchange.
-        :param timestamp: The time of the request.
+        :param exchange: The source name of the exchange.
+        :param symbol: The symbol of the pair.
+
+        :return: The dataset of the spread data.
         """
 
-        exchange = find_string_value(
-            value=data.exchange, values=self.market.keys()
-        )
-        symbol = find_string_value(
-            value=adjust_symbol(symbol=data.symbol),
-            values=exchange
-        )
+        try:
+            self.orderbook(exchange=exchange, symbol=symbol)
 
-        dataset = (
-            self.market.
-            setdefault(exchange, {}).
-            setdefault(symbol, create_orderbook_dataframe())
-        )
+            return True
 
-        bids = data.book.bids.to_list()
-        asks = data.book.asks.to_list()
+        except ValueError:
+            return False
+        # end try
+    # end orderbook_in_market
 
-        try:
-            dataset.loc[dt.datetime.fromtimestamp(timestamp)] = {
-                BIDS: float(bids[0][0]),
-                ASKS: float(asks[0][0]),
-                BIDS_VOLUME: float(bids[0][1]),
-                ASKS_VOLUME: float(asks[0][1])
-            }
+    async def record(self, data: OrderBook, timestamp: float) -> bool:
+        """
+        Records the data from the crypto feed into the dataset.
 
-        except IndexError:
-            pass
-        # end try
+        :param data: The data from the exchange.
+        :param timestamp: The time of the request.
+        """
+
+        return record_orderbook(
+            market=self.market, data=data, timestamp=timestamp
+        )
     # end record
 # end MarketOrderbookRecorder
 
 class OrderbookMarketScreener(MarketScreener):
     """
     A class to represent an asset price screener.
 
@@ -289,17 +425,80 @@
             delay=delay, recorder=recorder or OrderbookMarketRecorder(
                 market=structure_screener_datasets(screeners=screeners)
             ),
             screeners=screeners, handler=handler, limited=limited,
             amount=amount, refresh=refresh
         )
 
-        self.screeners[:] = self.screeners or self.create_orderbook_screeners()
+        self.screeners[:] = screeners or self.create_orderbook_screeners()
     # end __init__
 
+    @property
+    def orderbook_market(self) -> Market:
+        """
+        Returns the market to hold the recorder data.
+
+        :return: The market object.
+        """
+
+        return self.recorder.orderbook_market
+    # end orderbook_market
+
+    @property
+    def orderbook_screeners(self) -> List[OrderbookScreener]:
+        """
+        Returns a list of all the order-book screeners.
+
+        :return: The order-book screeners.
+        """
+
+        return [
+            screener for screener in self.screeners
+            if isinstance(screener, OrderbookScreener)
+        ]
+    # end orderbook_screeners
+
+    def connect_screeners(self) -> None:
+        """Connects the screeners to the recording object."""
+
+        for screener in self.screeners:
+            if isinstance(screener, OrderbookScreener):
+                screener.market = self.orderbook(
+                    exchange=screener.exchange, symbol=screener.symbol
+                )
+            # end if
+        # end for
+    # end connect_screeners
+
+    def orderbook(self, exchange: str, symbol: str) -> pd.DataFrame:
+        """
+        Returns the market data of the symbol from the exchange.
+
+        :param exchange: The source name of the exchange.
+        :param symbol: The symbol of the pair.
+
+        :return: The dataset of the spread data.
+        """
+
+        return self.recorder.orderbook(exchange=exchange, symbol=symbol)
+    # end orderbook
+
+    def orderbook_in_market(self, exchange: str, symbol: str) -> bool:
+        """
+        Returns the market data of the symbol from the exchange.
+
+        :param exchange: The source name of the exchange.
+        :param symbol: The symbol of the pair.
+
+        :return: The dataset of the spread data.
+        """
+
+        return self.recorder.orderbook_in_market(exchange=exchange, symbol=symbol)
+    # end orderbook_in_market
+
     def create_orderbook_screener(
             self,
             symbol: str,
             exchange: str,
             location: Optional[str] = None,
             cancel: Optional[Union[float, dt.timedelta]] = None,
             delay: Optional[Union[float, dt.timedelta]] = None,
@@ -328,15 +527,15 @@
             delay = self.delay
         # end if
 
         screener = OrderbookScreener(
             symbol=symbol, exchange=exchange, delay=delay,
             location=location, cancel=cancel, market=(
                 self.orderbook(exchange=exchange, symbol=symbol)
-                if self.in_market(symbol=symbol, exchange=exchange)
+                if self.orderbook_in_market(symbol=symbol, exchange=exchange)
                 else None
             )
         )
 
         container.setdefault(exchange, {})[symbol] = screener
 
         return screener
@@ -356,16 +555,16 @@
         :param cancel: The time to cancel the waiting.
         :param delay: The delay for the process.
         :param container: The container to contain the new screeners.
         """
 
         screeners = []
 
-        for exchange in self.market:
-            for symbol in self.market[exchange]:
+        for exchange, symbols in self.structure().items():
+            for symbol in symbols:
                 screeners.append(
                     self.create_orderbook_screener(
                         symbol=symbol, exchange=exchange, delay=delay,
                         location=location, cancel=cancel, container=container
                     )
                 )
             # end for
```

### Comparing `crypto-screening-3.7.0/crypto_screening/market/waiting.py` & `crypto-screening-4.0.0/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.7.0/crypto_screening/process.py` & `crypto-screening-4.0.0/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.7.0/crypto_screening/symbols.py` & `crypto-screening-4.0.0/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.7.0/crypto_screening/validate.py` & `crypto-screening-4.0.0/crypto_screening/validate.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # validate.py
 
 from typing import Optional, Iterable, Any
 
 from crypto_screening.process import find_string_value
 from crypto_screening.symbols import adjust_symbol
+from crypto_screening.interval import interval_to_total_time
 from crypto_screening.exchanges import EXCHANGE_NAMES, EXCHANGES
 
 __all__ = [
     "is_valid_symbol",
     "validate_exchange",
     "validate_symbol",
-    "is_valid_exchange"
+    "is_valid_exchange",
+    "validate_interval"
 ]
 
 def is_valid_symbol(
         exchange: str,
         symbol: str,
         exchanges: Optional[Iterable[str]] = None,
         symbols: Optional[Iterable[str]] = None
@@ -87,14 +89,28 @@
             f"{f' for {provider}.' if provider else ''}"
         )
     # end if
 
     return symbol
 # end validate_symbol
 
+def validate_interval(interval: str) -> str:
+    """
+    Validates the symbol value.
+
+    :param interval: The interval for the data.
+
+    :return: The validates symbol.
+    """
+
+    interval_to_total_time(interval)
+
+    return interval
+# end validate_interval
+
 def is_valid_exchange(
         exchange: str, exchanges: Optional[Iterable[str]] = None
 ) -> bool:
     """
     checks of the source os a valid exchange name.
 
     :param exchange: The source name to validate.
```

### Comparing `crypto-screening-3.7.0/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-4.0.0/crypto_screening.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 3.7.0
+Version: 4.0.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-3.7.0/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-4.0.0/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-3.7.0/pyproject.toml` & `crypto-screening-4.0.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '3.7.0'
+version = '4.0.0'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-3.7.0/setup.py` & `crypto-screening-4.0.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='3.7.0',
+        version='4.0.0',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

