# Comparing `tmp/fredeco-0.1.0.tar.gz` & `tmp/fredeco-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fredeco-0.1.0.tar", max compression
+gzip compressed data, was "fredeco-0.1.1.tar", max compression
```

## Comparing `fredeco-0.1.0.tar` & `fredeco-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-07-05 22:35:41.129213 fredeco-0.1.0/fredeco/__init__.py
--rw-r--r--   0        0        0     6488 2023-07-11 18:48:30.179556 fredeco-0.1.0/fredeco/fredData.py
--rw-r--r--   0        0        0      336 2023-07-10 04:05:12.705933 fredeco-0.1.0/fredeco/fredKey.py
--rw-r--r--   0        0        0     4293 2023-07-12 04:27:04.321650 fredeco-0.1.0/fredeco/fredSearch.py
--rw-r--r--   0        0        0      764 2023-07-12 04:07:05.950757 fredeco-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3638 2023-07-11 18:49:35.303226 fredeco-0.1.0/README.rst
--rw-r--r--   0        0        0     4224 1970-01-01 00:00:00.000000 fredeco-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-05 22:35:41.129213 fredeco-0.1.1/fredeco/__init__.py
+-rw-r--r--   0        0        0     6488 2023-07-11 18:48:30.179556 fredeco-0.1.1/fredeco/fredData.py
+-rw-r--r--   0        0        0      336 2023-07-10 04:05:12.705933 fredeco-0.1.1/fredeco/fredKey.py
+-rw-r--r--   0        0        0     4293 2023-07-12 04:27:04.321650 fredeco-0.1.1/fredeco/fredSearch.py
+-rw-r--r--   0        0        0     1146 2023-07-14 09:07:31.726289 fredeco-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3717 2023-07-14 06:14:04.229654 fredeco-0.1.1/README.rst
+-rw-r--r--   0        0        0     4752 1970-01-01 00:00:00.000000 fredeco-0.1.1/PKG-INFO
```

### Comparing `fredeco-0.1.0/fredeco/fredData.py` & `fredeco-0.1.1/fredeco/fredData.py`

 * *Files identical despite different names*

### Comparing `fredeco-0.1.0/fredeco/fredSearch.py` & `fredeco-0.1.1/fredeco/fredSearch.py`

 * *Files identical despite different names*

### Comparing `fredeco-0.1.0/pyproject.toml` & `fredeco-0.1.1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,32 @@
 [tool.poetry]
 name = "Fredeco"
-version = "0.1.0"
-description =  "This package allows its users to retrieve data provided by FRED® API and information related to them, such as their source."
-authors = ["Raulin Cadet <cadetraulin@gmail.com>"]
+version = "0.1.1"
+description =  "This python package allows its users to retrieve data provided by FRED® API and information related to them, such as their source."
+license="MIT"
+authors = ["Raulin L. Cadet"]
+maintainers = [
+    "Raulin L. Cadet"
+]
 readme = "README.rst"
+repository = "https://github.com/raulincadet/fredeco"
+documentation = "https://fredeco.readthedocs.io/en/latest/"
+keywords = ["economics","data","indicators", "fred"]
+classifiers = [
+    "Development Status :: 4 - Beta",
+    "Intended Audience :: Financial and Insurance Industry",
+    "Intended Audience :: Science/Research",
+]
 packages = [{include = "fredeco"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 requests = "^2.31.0"
 datetime = "^5.1"
-pandas = "^2.0.3"
+pandas = "^2.0.3" 
 numpy = "^1.25.0"
 nbsphinx = "^0.9.2"
 pandoc = "^2.3"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
```

### Comparing `fredeco-0.1.0/README.rst` & `fredeco-0.1.1/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 =============
 Description
 =============
 
-This package allows its users to retrieve data provided by FRED® API. This package uses FRED® API but is not endorsed or certified by the Federal Reserve Bank of St. Louis.
+This python package allows its users to retrieve economic data provided by FRED® API. Although ``fredeco`` uses FRED® API, it is not endorsed or certified by the Federal Reserve Bank of St. Louis. 
 
 ===========
 Features
 ===========
 
-* Retrieve a time series, when indicating its code;
-* Retrieve several time series, indicating their codes;
-* Search for all time series related to the keywords indicated by the user;
-* Find all time series of a category of series, by indicating the ID of the category;
-* Find the dates of all release of a time series;
-* Find the information related to a time series, such as the notes where the source of data can be found.
+* Retrieve a time series, when indicating the ID of the related indicator;
+* Retrieve several time series, indicating their IDs;
+* Search for all indicators related to the keywords indicated by the user;
+* Find all indicators of a category of series, by indicating the ID of the category;
+* Find the dates of all release of an indicator;
+* Find the information related to an indicator, such as the notes where the source of data can be found.
 
 ================
 Installation
 ================
 
 
     $ pip install fredeco
@@ -31,15 +31,15 @@
 * `requests <https://requests.readthedocs.io/en/latest/>`_
 * `datetime <https://docs.python.org/3/library/datetime.html>`_
 
 
 =========
 Usage
 =========
-The usage of the package is explained in this section, whereas some examples are provided in the *Examples* section of the documentation of the package. It is strongly recommanded to read also the section *Examples* of the documentation.
+The usage of the package is explained in this section, whereas some examples are provided in the *Examples* section of the `full documentation web page <https://fredeco.readthedocs.io/en/latest/index.html>`_ of the package. It is strongly recommanded to read that section.
 
 * Each user of ``fredeco`` should have his own FRED® API key. To accomodate a new user of ``fredeco``. One of the functions of the package, ``request_api_key()`` allows the user to open the webpage to request a FRED® API key.
 
 * To retrieve data, the user of ``fredeco`` should indicate the ID of an indicator, such as GDP for the US Gross Domestic Product, and GDPCA for the US Real Gross Domestic Product. Data related to an economic indicator, with the function ``fred_series()``, or several indicators, with the function ``fred_multi_series()``, can be retreived. Remember that each user should have her/his own API key as explained previously.
 
 * ``fredeco`` allows its users to retrieve information about an indicator, as illustrated in the section *Examples*. To retrieve information about an indicator, the function ``fred_info_series()`` should be used. 
 
@@ -51,8 +51,8 @@
 
 
 =========================
 License and terms of use
 =========================
 
 * ``fredeco`` is created by Raulin L. Cadet. It is licensed under the terms of the MIT license.
-* By using the package ``fredeco``, you are also agreeing to be bound by the FRED® API Terms of Use. The link to these Terms of Use is: `Here <https://fred.stlouisfed.org/docs/api/terms_of_use.html>`_. 
+* By using the package ``fredeco``, you are also agreeing to be bound by the FRED® API Terms of Use. The link to these Terms of Use is: `Here <https://fred.stlouisfed.org/docs/api/terms_of_use.html>`_.
```

### Comparing `fredeco-0.1.0/PKG-INFO` & `fredeco-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,49 @@
 Metadata-Version: 2.1
 Name: fredeco
-Version: 0.1.0
-Summary: This package allows its users to retrieve data provided by FRED® API and information related to them, such as their source.
-Author: Raulin Cadet
-Author-email: cadetraulin@gmail.com
+Version: 0.1.1
+Summary: This python package allows its users to retrieve data provided by FRED® API and information related to them, such as their source.
+Home-page: https://github.com/raulincadet/fredeco
+License: MIT
+Keywords: economics,data,indicators,fred
+Author: Raulin L. Cadet
+Maintainer: Raulin L. Cadet
 Requires-Python: >=3.11,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Financial and Insurance Industry
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: datetime (>=5.1,<6.0)
 Requires-Dist: nbsphinx (>=0.9.2,<0.10.0)
 Requires-Dist: numpy (>=1.25.0,<2.0.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: pandoc (>=2.3,<3.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Project-URL: Documentation, https://fredeco.readthedocs.io/en/latest/
+Project-URL: Repository, https://github.com/raulincadet/fredeco
 Description-Content-Type: text/x-rst
 
 =============
 Description
 =============
 
-This package allows its users to retrieve data provided by FRED® API. This package uses FRED® API but is not endorsed or certified by the Federal Reserve Bank of St. Louis.
+This python package allows its users to retrieve economic data provided by FRED® API. Although ``fredeco`` uses FRED® API, it is not endorsed or certified by the Federal Reserve Bank of St. Louis. 
 
 ===========
 Features
 ===========
 
-* Retrieve a time series, when indicating its code;
-* Retrieve several time series, indicating their codes;
-* Search for all time series related to the keywords indicated by the user;
-* Find all time series of a category of series, by indicating the ID of the category;
-* Find the dates of all release of a time series;
-* Find the information related to a time series, such as the notes where the source of data can be found.
+* Retrieve a time series, when indicating the ID of the related indicator;
+* Retrieve several time series, indicating their IDs;
+* Search for all indicators related to the keywords indicated by the user;
+* Find all indicators of a category of series, by indicating the ID of the category;
+* Find the dates of all release of an indicator;
+* Find the information related to an indicator, such as the notes where the source of data can be found.
 
 ================
 Installation
 ================
 
 
     $ pip install fredeco
@@ -48,15 +57,15 @@
 * `requests <https://requests.readthedocs.io/en/latest/>`_
 * `datetime <https://docs.python.org/3/library/datetime.html>`_
 
 
 =========
 Usage
 =========
-The usage of the package is explained in this section, whereas some examples are provided in the *Examples* section of the documentation of the package. It is strongly recommanded to read also the section *Examples* of the documentation.
+The usage of the package is explained in this section, whereas some examples are provided in the *Examples* section of the `full documentation web page <https://fredeco.readthedocs.io/en/latest/index.html>`_ of the package. It is strongly recommanded to read that section.
 
 * Each user of ``fredeco`` should have his own FRED® API key. To accomodate a new user of ``fredeco``. One of the functions of the package, ``request_api_key()`` allows the user to open the webpage to request a FRED® API key.
 
 * To retrieve data, the user of ``fredeco`` should indicate the ID of an indicator, such as GDP for the US Gross Domestic Product, and GDPCA for the US Real Gross Domestic Product. Data related to an economic indicator, with the function ``fred_series()``, or several indicators, with the function ``fred_multi_series()``, can be retreived. Remember that each user should have her/his own API key as explained previously.
 
 * ``fredeco`` allows its users to retrieve information about an indicator, as illustrated in the section *Examples*. To retrieve information about an indicator, the function ``fred_info_series()`` should be used. 
 
@@ -69,7 +78,8 @@
 
 =========================
 License and terms of use
 =========================
 
 * ``fredeco`` is created by Raulin L. Cadet. It is licensed under the terms of the MIT license.
 * By using the package ``fredeco``, you are also agreeing to be bound by the FRED® API Terms of Use. The link to these Terms of Use is: `Here <https://fred.stlouisfed.org/docs/api/terms_of_use.html>`_. 
+
```

