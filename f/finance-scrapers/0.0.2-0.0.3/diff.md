# Comparing `tmp/finance-scrapers-0.0.2.tar.gz` & `tmp/finance-scrapers-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finance-scrapers-0.0.2.tar", last modified: Fri Jul 14 17:01:38 2023, max compression
+gzip compressed data, was "finance-scrapers-0.0.3.tar", last modified: Fri Jul 14 18:02:52 2023, max compression
```

## Comparing `finance-scrapers-0.0.2.tar` & `finance-scrapers-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:38.280541 finance-scrapers-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-14 17:01:20.000000 finance-scrapers-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-14 17:01:38.280541 finance-scrapers-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-14 17:01:20.000000 finance-scrapers-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:38.276541 finance-scrapers-0.0.2/finance_scrapers/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-14 17:01:20.000000 finance-scrapers-0.0.2/finance_scrapers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-14 17:01:20.000000 finance-scrapers-0.0.2/finance_scrapers/stock_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-07-14 17:01:20.000000 finance-scrapers-0.0.2/finance_scrapers/yahoo_finance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:38.280541 finance-scrapers-0.0.2/finance_scrapers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-14 17:01:38.000000 finance-scrapers-0.0.2/finance_scrapers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-14 17:01:38.000000 finance-scrapers-0.0.2/finance_scrapers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:01:38.000000 finance-scrapers-0.0.2/finance_scrapers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-14 17:01:38.000000 finance-scrapers-0.0.2/finance_scrapers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 17:01:38.000000 finance-scrapers-0.0.2/finance_scrapers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-14 17:01:20.000000 finance-scrapers-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-14 17:01:38.280541 finance-scrapers-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:02:52.038704 finance-scrapers-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-14 18:02:38.000000 finance-scrapers-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-14 18:02:52.038704 finance-scrapers-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-14 18:02:38.000000 finance-scrapers-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:02:52.034704 finance-scrapers-0.0.3/finance_scrapers/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-14 18:02:38.000000 finance-scrapers-0.0.3/finance_scrapers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-14 18:02:38.000000 finance-scrapers-0.0.3/finance_scrapers/stock_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-07-14 18:02:38.000000 finance-scrapers-0.0.3/finance_scrapers/yahoo_finance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:02:52.038704 finance-scrapers-0.0.3/finance_scrapers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-14 18:02:52.000000 finance-scrapers-0.0.3/finance_scrapers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-14 18:02:52.000000 finance-scrapers-0.0.3/finance_scrapers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 18:02:52.000000 finance-scrapers-0.0.3/finance_scrapers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-14 18:02:52.000000 finance-scrapers-0.0.3/finance_scrapers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 18:02:52.000000 finance-scrapers-0.0.3/finance_scrapers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-14 18:02:38.000000 finance-scrapers-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-14 18:02:52.038704 finance-scrapers-0.0.3/setup.cfg
```

### Comparing `finance-scrapers-0.0.2/LICENSE` & `finance-scrapers-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `finance-scrapers-0.0.2/PKG-INFO` & `finance-scrapers-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finance-scrapers
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool to scrape stock information from Yahoo Finance
 Home-page: https://github.com/Mandy-cyber/Yahoo-Finance
 Author: Mandy-cyber
 Keywords: python,selenium,stocks,stock-data,yahoofinance,finance
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `finance-scrapers-0.0.2/README.md` & `finance-scrapers-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `finance-scrapers-0.0.2/finance_scrapers/yahoo_finance.py` & `finance-scrapers-0.0.3/finance_scrapers/yahoo_finance.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,28 +7,29 @@
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.common.by import By
 from typing import Dict, List
 import progressbar
 import json
 import time
 # internal imports
-from finance_scrapers.stock_options import StockOption
+# from finance_scrapers.stock_info import StockInfo
+from finance_scrapers.stock_info import StockInfo
 
 
 class YahooFinance:
     """
     A tool for scraping publicly available stock information from Yahoo Finance
 
     Attrs:
         home_url (str): the url of the home page for Yahoo Finance
     """
     home_url: str = "https://www.finance.yahoo.com"
 
     def __init__(self, tickers: List[str], validate_tickers: bool = True, 
-                 show_progress: bool = False, info_to_find: set[StockOption] = set(StockOption)) -> None:
+                 show_progress: bool = False, info_to_find: set[StockInfo] = set(StockInfo)) -> None:
         """
         Initializes a YahooFinance to scrape information about the given stocks
         (identified by their tickers).
 
         Args
             tickers: the tickers of the stocks to be scraped
             validate_tickers: if the tickers should be validated before scraping
@@ -206,16 +207,18 @@
         Returns:
             stock_info: information about the stock
         """
         self.__find_stock(ticker)
         stock_info: Dict[str, str] = dict()
         
         for idx, info in enumerate(self.info_to_find):
-            info_text = self.__explicit_wait(By.XPATH, info.value)
-            stock_info[info.name] = info_text
+            info_val = info.value
+            info_name = self.__explicit_wait(By.XPATH, info_val['name_loc'])
+            info_text = self.__explicit_wait(By.XPATH, info_val['info_loc'])
+            stock_info[info_name] = info_text
 
         return stock_info
     
 
     def __find_stocks(self) -> Dict[str, Dict[str, str]]:
         """
         Finds all the stocks, with their information, requested by the user
```

### Comparing `finance-scrapers-0.0.2/finance_scrapers.egg-info/PKG-INFO` & `finance-scrapers-0.0.3/finance_scrapers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finance-scrapers
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool to scrape stock information from Yahoo Finance
 Home-page: https://github.com/Mandy-cyber/Yahoo-Finance
 Author: Mandy-cyber
 Keywords: python,selenium,stocks,stock-data,yahoofinance,finance
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `finance-scrapers-0.0.2/setup.cfg` & `finance-scrapers-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = finance-scrapers
-version = 0.0.2
+version = 0.0.3
 author = Mandy-cyber
 description = A tool to scrape stock information from Yahoo Finance
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = python, selenium, stocks, stock-data, yahoofinance, finance
 url = https://github.com/Mandy-cyber/Yahoo-Finance
 classifiers =
```

