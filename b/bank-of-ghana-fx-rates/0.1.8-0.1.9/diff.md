# Comparing `tmp/bank-of-ghana-fx-rates-0.1.8.tar.gz` & `tmp/bank-of-ghana-fx-rates-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bank-of-ghana-fx-rates-0.1.8.tar", last modified: Thu Jul 13 21:36:38 2023, max compression
+gzip compressed data, was "dist/bank-of-ghana-fx-rates-0.1.9.tar", last modified: Thu Jul 13 21:47:46 2023, max compression
```

## Comparing `bank-of-ghana-fx-rates-0.1.8.tar` & `bank-of-ghana-fx-rates-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-07-13 21:36:38.000000 bank-of-ghana-fx-rates-0.1.8/
--rw-r--r--   0 tsiameh    (501) staff       (20)     1074 2021-01-13 02:45:22.000000 bank-of-ghana-fx-rates-0.1.8/LICENSE
--rw-r--r--   0 tsiameh    (501) staff       (20)     3515 2023-07-13 21:36:38.000000 bank-of-ghana-fx-rates-0.1.8/PKG-INFO
--rw-r--r--   0 tsiameh    (501) staff       (20)     1783 2023-07-13 20:24:44.000000 bank-of-ghana-fx-rates-0.1.8/README.md
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-07-13 21:36:38.000000 bank-of-ghana-fx-rates-0.1.8/bank_of_ghana_fx_rates.egg-info/
--rw-r--r--   0 tsiameh    (501) staff       (20)     3515 2023-07-13 21:36:38.000000 bank-of-ghana-fx-rates-0.1.8/bank_of_ghana_fx_rates.egg-info/PKG-INFO
--rw-r--r--   0 tsiameh    (501) staff       (20)      362 2023-07-13 21:36:38.000000 bank-of-ghana-fx-rates-0.1.8/bank_of_ghana_fx_rates.egg-info/SOURCES.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)        1 2023-07-13 21:36:38.000000 bank-of-ghana-fx-rates-0.1.8/bank_of_ghana_fx_rates.egg-info/dependency_links.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)       44 2023-07-13 21:36:38.000000 bank-of-ghana-fx-rates-0.1.8/bank_of_ghana_fx_rates.egg-info/entry_points.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)       48 2023-07-13 21:36:38.000000 bank-of-ghana-fx-rates-0.1.8/bank_of_ghana_fx_rates.egg-info/requires.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)        4 2023-07-13 21:36:38.000000 bank-of-ghana-fx-rates-0.1.8/bank_of_ghana_fx_rates.egg-info/top_level.txt
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-07-13 21:36:38.000000 bank-of-ghana-fx-rates-0.1.8/bog/
--rw-r--r--   0 tsiameh    (501) staff       (20)        0 2021-01-13 02:45:22.000000 bank-of-ghana-fx-rates-0.1.8/bog/__init__.py
--rw-r--r--   0 tsiameh    (501) staff       (20)      986 2023-07-13 20:05:34.000000 bank-of-ghana-fx-rates-0.1.8/bog/scraper.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     5587 2023-07-13 21:17:20.000000 bank-of-ghana-fx-rates-0.1.8/bog/utils.py
--rw-r--r--   0 tsiameh    (501) staff       (20)       38 2023-07-13 21:36:38.000000 bank-of-ghana-fx-rates-0.1.8/setup.cfg
--rw-r--r--   0 tsiameh    (501) staff       (20)     1902 2023-07-13 20:18:46.000000 bank-of-ghana-fx-rates-0.1.8/setup.py
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-07-13 21:36:38.000000 bank-of-ghana-fx-rates-0.1.8/tests/
--rw-r--r--   0 tsiameh    (501) staff       (20)     4878 2023-07-12 20:28:00.000000 bank-of-ghana-fx-rates-0.1.8/tests/test.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-07-13 21:47:46.000000 bank-of-ghana-fx-rates-0.1.9/
+-rw-r--r--   0 tsiameh    (501) staff       (20)     1074 2021-01-13 02:45:22.000000 bank-of-ghana-fx-rates-0.1.9/LICENSE
+-rw-r--r--   0 tsiameh    (501) staff       (20)     3515 2023-07-13 21:47:46.000000 bank-of-ghana-fx-rates-0.1.9/PKG-INFO
+-rw-r--r--   0 tsiameh    (501) staff       (20)     1783 2023-07-13 20:24:44.000000 bank-of-ghana-fx-rates-0.1.9/README.md
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-07-13 21:47:46.000000 bank-of-ghana-fx-rates-0.1.9/bank_of_ghana_fx_rates.egg-info/
+-rw-r--r--   0 tsiameh    (501) staff       (20)     3515 2023-07-13 21:47:46.000000 bank-of-ghana-fx-rates-0.1.9/bank_of_ghana_fx_rates.egg-info/PKG-INFO
+-rw-r--r--   0 tsiameh    (501) staff       (20)      362 2023-07-13 21:47:46.000000 bank-of-ghana-fx-rates-0.1.9/bank_of_ghana_fx_rates.egg-info/SOURCES.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)        1 2023-07-13 21:47:46.000000 bank-of-ghana-fx-rates-0.1.9/bank_of_ghana_fx_rates.egg-info/dependency_links.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)       44 2023-07-13 21:47:46.000000 bank-of-ghana-fx-rates-0.1.9/bank_of_ghana_fx_rates.egg-info/entry_points.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)       55 2023-07-13 21:47:46.000000 bank-of-ghana-fx-rates-0.1.9/bank_of_ghana_fx_rates.egg-info/requires.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)        4 2023-07-13 21:47:46.000000 bank-of-ghana-fx-rates-0.1.9/bank_of_ghana_fx_rates.egg-info/top_level.txt
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-07-13 21:47:46.000000 bank-of-ghana-fx-rates-0.1.9/bog/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2021-01-13 02:45:22.000000 bank-of-ghana-fx-rates-0.1.9/bog/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      986 2023-07-13 20:05:34.000000 bank-of-ghana-fx-rates-0.1.9/bog/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     5587 2023-07-13 21:17:20.000000 bank-of-ghana-fx-rates-0.1.9/bog/utils.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)       38 2023-07-13 21:47:46.000000 bank-of-ghana-fx-rates-0.1.9/setup.cfg
+-rw-r--r--   0 tsiameh    (501) staff       (20)     1902 2023-07-13 21:47:42.000000 bank-of-ghana-fx-rates-0.1.9/setup.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-07-13 21:47:46.000000 bank-of-ghana-fx-rates-0.1.9/tests/
+-rw-r--r--   0 tsiameh    (501) staff       (20)     4878 2023-07-12 20:28:00.000000 bank-of-ghana-fx-rates-0.1.9/tests/test.py
```

### Comparing `bank-of-ghana-fx-rates-0.1.8/LICENSE` & `bank-of-ghana-fx-rates-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bank-of-ghana-fx-rates-0.1.8/PKG-INFO` & `bank-of-ghana-fx-rates-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bank-of-ghana-fx-rates
-Version: 0.1.8
+Version: 0.1.9
 Summary: A python client library used to extract the exchange rates of Bank of Ghana into CSV
 Home-page: https://github.com/donwany/bank-of-ghana-fx-rates.git
 Author: Theophilus Siameh
 Author-email: theodondre@gmail.com
 License: MIT License
 Description: ![Python 3.7, 3.8, 3.9](https://img.shields.io/badge/Python-3.7%2C%203.8%2C%203.9-3776ab.svg?maxAge=2592000)
         [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bank-of-ghana-fx-rates Version: 0.1.8 Summary: A
+Metadata-Version: 2.1 Name: bank-of-ghana-fx-rates Version: 0.1.9 Summary: A
 python client library used to extract the exchange rates of Bank of Ghana into
 CSV Home-page: https://github.com/donwany/bank-of-ghana-fx-rates.git Author:
 Theophilus Siameh Author-email: theodondre@gmail.com License: MIT License
 Description: ![Python 3.7, 3.8, 3.9](https://img.shields.io/badge/Python-
 3.7%2C%203.8%2C%203.9-3776ab.svg?maxAge=2592000) [![Imports: isort](https://
 img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)]
 (https://pycqa.github.io/isort/) ### Bank of Ghana Exchange Rate Python Library
```

### Comparing `bank-of-ghana-fx-rates-0.1.8/README.md` & `bank-of-ghana-fx-rates-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `bank-of-ghana-fx-rates-0.1.8/bank_of_ghana_fx_rates.egg-info/PKG-INFO` & `bank-of-ghana-fx-rates-0.1.9/bank_of_ghana_fx_rates.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bank-of-ghana-fx-rates
-Version: 0.1.8
+Version: 0.1.9
 Summary: A python client library used to extract the exchange rates of Bank of Ghana into CSV
 Home-page: https://github.com/donwany/bank-of-ghana-fx-rates.git
 Author: Theophilus Siameh
 Author-email: theodondre@gmail.com
 License: MIT License
 Description: ![Python 3.7, 3.8, 3.9](https://img.shields.io/badge/Python-3.7%2C%203.8%2C%203.9-3776ab.svg?maxAge=2592000)
         [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bank-of-ghana-fx-rates Version: 0.1.8 Summary: A
+Metadata-Version: 2.1 Name: bank-of-ghana-fx-rates Version: 0.1.9 Summary: A
 python client library used to extract the exchange rates of Bank of Ghana into
 CSV Home-page: https://github.com/donwany/bank-of-ghana-fx-rates.git Author:
 Theophilus Siameh Author-email: theodondre@gmail.com License: MIT License
 Description: ![Python 3.7, 3.8, 3.9](https://img.shields.io/badge/Python-
 3.7%2C%203.8%2C%203.9-3776ab.svg?maxAge=2592000) [![Imports: isort](https://
 img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)]
 (https://pycqa.github.io/isort/) ### Bank of Ghana Exchange Rate Python Library
```

### Comparing `bank-of-ghana-fx-rates-0.1.8/bog/scraper.py` & `bank-of-ghana-fx-rates-0.1.9/bog/scraper.py`

 * *Files identical despite different names*

### Comparing `bank-of-ghana-fx-rates-0.1.8/bog/utils.py` & `bank-of-ghana-fx-rates-0.1.9/bog/utils.py`

 * *Files identical despite different names*

### Comparing `bank-of-ghana-fx-rates-0.1.8/setup.py` & `bank-of-ghana-fx-rates-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open("requirements.txt", "r") as f:
     install_requires = f.read().splitlines()
 
 setup(
     name='bank-of-ghana-fx-rates',
     py_modules=["bog"],
-    version='0.1.8',
+    version='0.1.9',
     packages=find_packages(exclude=["docs", "tests", "tests.*"]),
     long_description=README,
     long_description_content_type="text/markdown",
     url='https://github.com/donwany/bank-of-ghana-fx-rates.git',
     license="MIT License",
     author="Theophilus Siameh",
     author_email="theodondre@gmail.com",
```

### Comparing `bank-of-ghana-fx-rates-0.1.8/tests/test.py` & `bank-of-ghana-fx-rates-0.1.9/tests/test.py`

 * *Files identical despite different names*

