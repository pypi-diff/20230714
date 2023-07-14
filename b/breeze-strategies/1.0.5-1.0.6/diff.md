# Comparing `tmp/breeze_strategies-1.0.5.tar.gz` & `tmp/breeze_strategies-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "breeze_strategies-1.0.5.tar", last modified: Wed Jul 12 06:39:45 2023, max compression
+gzip compressed data, was "breeze_strategies-1.0.6.tar", last modified: Fri Jul 14 04:17:20 2023, max compression
```

## Comparing `breeze_strategies-1.0.5.tar` & `breeze_strategies-1.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 06:39:45.452181 breeze_strategies-1.0.5/
--rw-rw-rw-   0        0        0     1113 2023-06-23 07:11:33.000000 breeze_strategies-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     1727 2023-07-12 06:39:45.451172 breeze_strategies-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1176 2023-07-12 06:35:15.000000 breeze_strategies-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 06:39:45.397310 breeze_strategies-1.0.5/breeze_strategies/
--rw-rw-rw-   0        0        0       58 2023-06-15 05:52:47.000000 breeze_strategies-1.0.5/breeze_strategies/__init__.py
--rw-rw-rw-   0        0        0    28160 2023-07-12 06:39:28.000000 breeze_strategies-1.0.5/breeze_strategies/breeze_strategies.py
-drwxrwxrwx   0        0        0        0 2023-07-12 06:39:45.448451 breeze_strategies-1.0.5/breeze_strategies.egg-info/
--rw-rw-rw-   0        0        0     1727 2023-07-12 06:39:45.000000 breeze_strategies-1.0.5/breeze_strategies.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-07-12 06:39:45.000000 breeze_strategies-1.0.5/breeze_strategies.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 06:39:45.000000 breeze_strategies-1.0.5/breeze_strategies.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-07-12 06:39:45.000000 breeze_strategies-1.0.5/breeze_strategies.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-07-12 06:39:45.000000 breeze_strategies-1.0.5/breeze_strategies.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 06:39:45.452181 breeze_strategies-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      817 2023-07-12 06:36:35.000000 breeze_strategies-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 04:17:20.219633 breeze_strategies-1.0.6/
+-rw-rw-rw-   0        0        0     1113 2023-06-23 07:11:33.000000 breeze_strategies-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0     1727 2023-07-14 04:17:20.217571 breeze_strategies-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1176 2023-07-14 04:16:25.000000 breeze_strategies-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 04:17:20.171157 breeze_strategies-1.0.6/breeze_strategies/
+-rw-rw-rw-   0        0        0       58 2023-06-15 05:52:47.000000 breeze_strategies-1.0.6/breeze_strategies/__init__.py
+-rw-rw-rw-   0        0        0    28194 2023-07-14 04:16:57.000000 breeze_strategies-1.0.6/breeze_strategies/breeze_strategies.py
+drwxrwxrwx   0        0        0        0 2023-07-14 04:17:20.215571 breeze_strategies-1.0.6/breeze_strategies.egg-info/
+-rw-rw-rw-   0        0        0     1727 2023-07-14 04:17:20.000000 breeze_strategies-1.0.6/breeze_strategies.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-07-14 04:17:20.000000 breeze_strategies-1.0.6/breeze_strategies.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 04:17:20.000000 breeze_strategies-1.0.6/breeze_strategies.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-07-14 04:17:20.000000 breeze_strategies-1.0.6/breeze_strategies.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-14 04:17:20.000000 breeze_strategies-1.0.6/breeze_strategies.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 04:17:20.220575 breeze_strategies-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      817 2023-07-14 04:16:39.000000 breeze_strategies-1.0.6/setup.py
```

### Comparing `breeze_strategies-1.0.5/LICENSE` & `breeze_strategies-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `breeze_strategies-1.0.5/PKG-INFO` & `breeze_strategies-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: breeze_strategies
-Version: 1.0.5
+Version: 1.0.6
 Summary: ICICIDIRECT's breezeconnect strategies in python
 Home-page: https://github.com/Idirect-Tech/python_strategies/tree/master
 Author: ICICI Direct Breeze
 Author-email: breezeapi@icicisecurities.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 # LIVE  python_strategies
 
 ## Steps to install Strategy Library for LIVE
 
 
 ```python
 
-pip install breeze_strategies==1.0.5
+pip install breeze_strategies==1.0.6
 
 ```
 
 ## Updating Library
 
 ```python
```

### Comparing `breeze_strategies-1.0.5/README.md` & `breeze_strategies-1.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # LIVE  python_strategies
 
 ## Steps to install Strategy Library for LIVE
 
 
 ```python
 
-pip install breeze_strategies==1.0.5
+pip install breeze_strategies==1.0.6
 
 ```
 
 ## Updating Library
 
 ```python
```

### Comparing `breeze_strategies-1.0.5/breeze_strategies/breeze_strategies.py` & `breeze_strategies-1.0.6/breeze_strategies/breeze_strategies.py`

 * *Files 0% similar despite different names*

```diff
@@ -463,15 +463,15 @@
             print(f"P&L (PUT) : {plput}/- Rs")
             print(f"P&L (NET) : {plput + plcall}/- Rs")
             print("----------------------------------------")
         else:
             print("One of Square off operation failed..")
 
 
-    def single_leg(self,right, strategy_type,stock_code, strike_price, quantity, expiry_date, price = "0", stoploss = "",product_type = "options", order_type = "market", validity = "day", validity_date = datetime.utcnow().strftime('%Y-%m-%dT%H:%M:%S.%fZ'), exchange_code = "NFO"):
+    def single_leg(self,right, strategy_type,stock_code, strike_price, quantity, expiry_date, price = "0", stoploss = "",product_type = "options", order_type = "market", validity = "day", validity_date = datetime.utcnow().strftime('%Y-%m-%dT%H:%M:%S.%fZ'), exchange_code = "NFO",put_price = "0", call_price = "0"):
         self.quantity = quantity
         self.strategy_type = strategy_type
         self.exchange_code = exchange_code 
         self.stock_code = stock_code
         self.product_type = product_type 
         self.expiry_date = expiry_date  
         self.strike_price = strike_price
```

### Comparing `breeze_strategies-1.0.5/breeze_strategies.egg-info/PKG-INFO` & `breeze_strategies-1.0.6/breeze_strategies.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: breeze-strategies
-Version: 1.0.5
+Version: 1.0.6
 Summary: ICICIDIRECT's breezeconnect strategies in python
 Home-page: https://github.com/Idirect-Tech/python_strategies/tree/master
 Author: ICICI Direct Breeze
 Author-email: breezeapi@icicisecurities.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 # LIVE  python_strategies
 
 ## Steps to install Strategy Library for LIVE
 
 
 ```python
 
-pip install breeze_strategies==1.0.5
+pip install breeze_strategies==1.0.6
 
 ```
 
 ## Updating Library
 
 ```python
```

### Comparing `breeze_strategies-1.0.5/setup.py` & `breeze_strategies-1.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="breeze_strategies",
-    version="1.0.5",
+    version="1.0.6",
     author="ICICI Direct Breeze",
     author_email="breezeapi@icicisecurities.com",
     description="ICICIDIRECT's breezeconnect strategies in python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=['breeze_connect==1.0.37','nest_asyncio'],
     url="https://github.com/Idirect-Tech/python_strategies/tree/master",
```

