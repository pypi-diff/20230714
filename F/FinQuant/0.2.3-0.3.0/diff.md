# Comparing `tmp/FinQuant-0.2.3.tar.gz` & `tmp/FinQuant-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FinQuant-0.2.3.tar", last modified: Wed Jul 12 07:32:42 2023, max compression
+gzip compressed data, was "FinQuant-0.3.0.tar", last modified: Fri Jul 14 13:23:40 2023, max compression
```

## Comparing `FinQuant-0.2.3.tar` & `FinQuant-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,37 @@
-drwxrwxrwx   0 frank     (1000) frank     (1000)        0 2023-07-12 07:32:43.098627 FinQuant-0.2.3/
-drwxrwxrwx   0 frank     (1000) frank     (1000)        0 2023-07-12 07:32:42.939143 FinQuant-0.2.3/FinQuant.egg-info/
--rwxrwxrwx   0 frank     (1000) frank     (1000)    14845 2023-07-12 07:32:42.000000 FinQuant-0.2.3/FinQuant.egg-info/PKG-INFO
--rwxrwxrwx   0 frank     (1000) frank     (1000)      582 2023-07-12 07:32:42.000000 FinQuant-0.2.3/FinQuant.egg-info/SOURCES.txt
--rwxrwxrwx   0 frank     (1000) frank     (1000)        1 2023-07-12 07:32:42.000000 FinQuant-0.2.3/FinQuant.egg-info/dependency_links.txt
--rwxrwxrwx   0 frank     (1000) frank     (1000)      193 2023-07-12 07:32:42.000000 FinQuant-0.2.3/FinQuant.egg-info/requires.txt
--rwxrwxrwx   0 frank     (1000) frank     (1000)        9 2023-07-12 07:32:42.000000 FinQuant-0.2.3/FinQuant.egg-info/top_level.txt
--rwxrwxrwx   0 frank     (1000) frank     (1000)     1059 2023-07-08 06:47:36.000000 FinQuant-0.2.3/LICENSE.txt
--rwxrwxrwx   0 frank     (1000) frank     (1000)    14845 2023-07-12 07:32:43.099125 FinQuant-0.2.3/PKG-INFO
--rwxrwxrwx   0 frank     (1000) frank     (1000)    13659 2023-07-11 12:42:27.000000 FinQuant-0.2.3/README.md
-drwxrwxrwx   0 frank     (1000) frank     (1000)        0 2023-07-12 07:32:43.022645 FinQuant-0.2.3/finquant/
--rwxrwxrwx   0 frank     (1000) frank     (1000)        0 2023-07-08 06:47:36.000000 FinQuant-0.2.3/finquant/__init__.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)    16801 2023-07-10 17:36:45.000000 FinQuant-0.2.3/finquant/efficient_frontier.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)     1990 2023-07-10 13:30:17.000000 FinQuant-0.2.3/finquant/minimise_fun.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)    11159 2023-07-08 06:47:36.000000 FinQuant-0.2.3/finquant/monte_carlo.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)     6685 2023-07-08 06:47:36.000000 FinQuant-0.2.3/finquant/moving_average.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)    43673 2023-07-08 08:26:58.000000 FinQuant-0.2.3/finquant/portfolio.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)     3936 2023-07-08 06:47:36.000000 FinQuant-0.2.3/finquant/quants.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)     2142 2023-07-08 06:47:36.000000 FinQuant-0.2.3/finquant/returns.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)     4291 2023-07-08 08:26:58.000000 FinQuant-0.2.3/finquant/stock.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)      106 2023-07-12 07:32:43.102127 FinQuant-0.2.3/setup.cfg
--rwxrwxrwx   0 frank     (1000) frank     (1000)     2173 2023-07-12 07:27:20.000000 FinQuant-0.2.3/setup.py
-drwxrwxrwx   0 frank     (1000) frank     (1000)        0 2023-07-12 07:32:43.088627 FinQuant-0.2.3/tests/
--rwxrwxrwx   0 frank     (1000) frank     (1000)      212 2023-07-08 06:47:36.000000 FinQuant-0.2.3/tests/test_efficient_frontier.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)     6288 2023-07-08 08:26:58.000000 FinQuant-0.2.3/tests/test_moving_average.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)      212 2023-07-08 06:47:36.000000 FinQuant-0.2.3/tests/test_optimisation.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)    15918 2023-07-08 08:26:58.000000 FinQuant-0.2.3/tests/test_portfolio.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)     1283 2023-07-08 06:47:36.000000 FinQuant-0.2.3/tests/test_quants.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)     2250 2023-07-08 06:47:36.000000 FinQuant-0.2.3/tests/test_returns.py
--rwxrwxrwx   0 frank     (1000) frank     (1000)     1926 2023-07-08 08:26:58.000000 FinQuant-0.2.3/tests/test_stock.py
+drwxrwxrwx   0 frank     (1000) frank     (1000)        0 2023-07-14 13:23:41.721071 FinQuant-0.3.0/
+drwxrwxrwx   0 frank     (1000) frank     (1000)        0 2023-07-14 13:23:41.482070 FinQuant-0.3.0/FinQuant.egg-info/
+-rwxrwxrwx   0 frank     (1000) frank     (1000)    14821 2023-07-14 13:23:41.000000 FinQuant-0.3.0/FinQuant.egg-info/PKG-INFO
+-rwxrwxrwx   0 frank     (1000) frank     (1000)      801 2023-07-14 13:23:41.000000 FinQuant-0.3.0/FinQuant.egg-info/SOURCES.txt
+-rwxrwxrwx   0 frank     (1000) frank     (1000)        1 2023-07-14 13:23:41.000000 FinQuant-0.3.0/FinQuant.egg-info/dependency_links.txt
+-rwxrwxrwx   0 frank     (1000) frank     (1000)      176 2023-07-14 13:23:41.000000 FinQuant-0.3.0/FinQuant.egg-info/requires.txt
+-rwxrwxrwx   0 frank     (1000) frank     (1000)        9 2023-07-14 13:23:41.000000 FinQuant-0.3.0/FinQuant.egg-info/top_level.txt
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     1059 2023-07-08 06:47:36.000000 FinQuant-0.3.0/LICENSE.txt
+-rwxrwxrwx   0 frank     (1000) frank     (1000)    14821 2023-07-14 13:23:41.722070 FinQuant-0.3.0/PKG-INFO
+-rwxrwxrwx   0 frank     (1000) frank     (1000)    13659 2023-07-14 13:20:17.000000 FinQuant-0.3.0/README.md
+drwxrwxrwx   0 frank     (1000) frank     (1000)        0 2023-07-14 13:23:41.592070 FinQuant-0.3.0/finquant/
+-rwxrwxrwx   0 frank     (1000) frank     (1000)        0 2023-07-08 06:47:36.000000 FinQuant-0.3.0/finquant/__init__.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     2764 2023-07-14 10:30:56.000000 FinQuant-0.3.0/finquant/asset.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)    16801 2023-07-10 17:36:45.000000 FinQuant-0.3.0/finquant/efficient_frontier.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     3180 2023-07-14 13:11:14.000000 FinQuant-0.3.0/finquant/market.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     1993 2023-07-14 09:57:06.000000 FinQuant-0.3.0/finquant/minimise_fun.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)    11159 2023-07-08 06:47:36.000000 FinQuant-0.3.0/finquant/monte_carlo.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     6685 2023-07-14 13:11:10.000000 FinQuant-0.3.0/finquant/moving_average.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)    47239 2023-07-14 13:11:10.000000 FinQuant-0.3.0/finquant/portfolio.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     3936 2023-07-08 06:47:36.000000 FinQuant-0.3.0/finquant/quants.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     2209 2023-07-14 09:57:06.000000 FinQuant-0.3.0/finquant/returns.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     4940 2023-07-14 13:11:14.000000 FinQuant-0.3.0/finquant/stock.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)      106 2023-07-14 13:23:41.725073 FinQuant-0.3.0/setup.cfg
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     2111 2023-07-12 07:35:01.000000 FinQuant-0.3.0/setup.py
+drwxrwxrwx   0 frank     (1000) frank     (1000)        0 2023-07-14 13:23:41.711074 FinQuant-0.3.0/tests/
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     7949 2023-07-14 12:13:25.000000 FinQuant-0.3.0/tests/test_Example-Analysis.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     3056 2023-07-14 12:13:25.000000 FinQuant-0.3.0/tests/test_Example-Build-Portfolio-from-file.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     5368 2023-07-14 12:13:25.000000 FinQuant-0.3.0/tests/test_Example-Build-Portfolio-from-web.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     6715 2023-07-14 12:13:25.000000 FinQuant-0.3.0/tests/test_Example-Optimisation.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)      212 2023-07-08 06:47:36.000000 FinQuant-0.3.0/tests/test_efficient_frontier.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     1006 2023-07-14 09:57:06.000000 FinQuant-0.3.0/tests/test_market.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     6288 2023-07-08 08:26:58.000000 FinQuant-0.3.0/tests/test_moving_average.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)      212 2023-07-08 06:47:36.000000 FinQuant-0.3.0/tests/test_optimisation.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)    15918 2023-07-08 08:26:58.000000 FinQuant-0.3.0/tests/test_portfolio.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     1283 2023-07-08 06:47:36.000000 FinQuant-0.3.0/tests/test_quants.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     2250 2023-07-08 06:47:36.000000 FinQuant-0.3.0/tests/test_returns.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     1926 2023-07-08 08:26:58.000000 FinQuant-0.3.0/tests/test_stock.py
```

### Comparing `FinQuant-0.2.3/FinQuant.egg-info/PKG-INFO` & `FinQuant-0.3.0/FinQuant.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: FinQuant
-Version: 0.2.3
+Version: 0.3.0
 Summary: A program for financial portfolio management, analysis and optimisation
 Home-page: https://github.com/fmilthaler/FinQuant
-Download-URL: https://github.com/fmilthaler/FinQuant/archive/v0.2.3.tar.gz
+Download-URL: https://github.com/fmilthaler/FinQuant/archive/v0.3.0.tar.gz
 Author: Frank Milthaler
 Author-email: f.milthaler@gmail.com
 License: MIT
 Project-URL: Documentation, https://finquant.readthedocs.io
 Keywords: finance,portfolio,investment,numerical,optimisation,monte carlo,efficient frontier,quantitative,quant
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
@@ -20,27 +20,26 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: docs
-Provides-Extra: publish
 License-File: LICENSE.txt
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/images/finquant-logo.png" width="45%">
 </p>
 
 <p align="center">
   <a href="https://GitHub.com/fmilthaler/FinQuant/stargazers/">
     <img src="https://img.shields.io/github/stars/fmilthaler/FinQuant.svg?style=social&label=Star" alt='pypi'>
   </a>
   <a href="https://pypi.org/project/FinQuant">
-    <img src="https://img.shields.io/badge/pypi-v0.2.2-brightgreen.svg?style=popout" alt='pypi'>
+    <img src="https://img.shields.io/badge/pypi-v0.3.0-brightgreen.svg?style=popout" alt='pypi'>
   </a>
   <a href="https://github.com/fmilthaler/FinQuant">
     <img src="https://github.com/fmilthaler/finquant/actions/workflows/pytest.yml/badge.svg?branch=master" alt='GitHub Actions'>
   </a>
   <a href="http://finquant.readthedocs.io/">
     <img src="https://img.shields.io/readthedocs/finquant.svg?style=popout" alt="docs">
   </a>
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: FinQuant Version: 0.2.3 Summary: A program for
+Metadata-Version: 2.1 Name: FinQuant Version: 0.3.0 Summary: A program for
 financial portfolio management, analysis and optimisation Home-page: https://
 github.com/fmilthaler/FinQuant Download-URL: https://github.com/fmilthaler/
-FinQuant/archive/v0.2.3.tar.gz Author: Frank Milthaler Author-email:
+FinQuant/archive/v0.3.0.tar.gz Author: Frank Milthaler Author-email:
 f.milthaler@gmail.com License: MIT Project-URL: Documentation, https://
 finquant.readthedocs.io Keywords:
 finance,portfolio,investment,numerical,optimisation,monte carlo,efficient
 frontier,quantitative,quant Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education Classifier: Intended Audience ::
 Financial and Insurance Industry Classifier: Intended Audience :: Other
 Audience Classifier: Intended Audience :: Science/Research Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.10 Description-Content-Type: text/markdown
-Provides-Extra: test Provides-Extra: dev Provides-Extra: docs Provides-Extra:
-publish License-File: LICENSE.txt
+Provides-Extra: test Provides-Extra: dev Provides-Extra: docs License-File:
+LICENSE.txt
 [https://raw.githubusercontent.com/fmilthaler/finquant/master/images/finquant-
                                    logo.png]
 [pypi] [pypi] [GitHub_Actions] [docs] [contributors] [contributions] [license]
 # FinQuant *FinQuant* is a program for financial **portfolio management,
 analysis and optimisation**. This README only gives a brief overview of
 *FinQuant*. The interested reader should refer to its [documentation](https://
 finquant.readthedocs.io "FinQuant Documentation"). ## Table of contents -
```

### Comparing `FinQuant-0.2.3/LICENSE.txt` & `FinQuant-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FinQuant-0.2.3/PKG-INFO` & `FinQuant-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: FinQuant
-Version: 0.2.3
+Version: 0.3.0
 Summary: A program for financial portfolio management, analysis and optimisation
 Home-page: https://github.com/fmilthaler/FinQuant
-Download-URL: https://github.com/fmilthaler/FinQuant/archive/v0.2.3.tar.gz
+Download-URL: https://github.com/fmilthaler/FinQuant/archive/v0.3.0.tar.gz
 Author: Frank Milthaler
 Author-email: f.milthaler@gmail.com
 License: MIT
 Project-URL: Documentation, https://finquant.readthedocs.io
 Keywords: finance,portfolio,investment,numerical,optimisation,monte carlo,efficient frontier,quantitative,quant
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
@@ -20,27 +20,26 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: docs
-Provides-Extra: publish
 License-File: LICENSE.txt
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/images/finquant-logo.png" width="45%">
 </p>
 
 <p align="center">
   <a href="https://GitHub.com/fmilthaler/FinQuant/stargazers/">
     <img src="https://img.shields.io/github/stars/fmilthaler/FinQuant.svg?style=social&label=Star" alt='pypi'>
   </a>
   <a href="https://pypi.org/project/FinQuant">
-    <img src="https://img.shields.io/badge/pypi-v0.2.2-brightgreen.svg?style=popout" alt='pypi'>
+    <img src="https://img.shields.io/badge/pypi-v0.3.0-brightgreen.svg?style=popout" alt='pypi'>
   </a>
   <a href="https://github.com/fmilthaler/FinQuant">
     <img src="https://github.com/fmilthaler/finquant/actions/workflows/pytest.yml/badge.svg?branch=master" alt='GitHub Actions'>
   </a>
   <a href="http://finquant.readthedocs.io/">
     <img src="https://img.shields.io/readthedocs/finquant.svg?style=popout" alt="docs">
   </a>
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: FinQuant Version: 0.2.3 Summary: A program for
+Metadata-Version: 2.1 Name: FinQuant Version: 0.3.0 Summary: A program for
 financial portfolio management, analysis and optimisation Home-page: https://
 github.com/fmilthaler/FinQuant Download-URL: https://github.com/fmilthaler/
-FinQuant/archive/v0.2.3.tar.gz Author: Frank Milthaler Author-email:
+FinQuant/archive/v0.3.0.tar.gz Author: Frank Milthaler Author-email:
 f.milthaler@gmail.com License: MIT Project-URL: Documentation, https://
 finquant.readthedocs.io Keywords:
 finance,portfolio,investment,numerical,optimisation,monte carlo,efficient
 frontier,quantitative,quant Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education Classifier: Intended Audience ::
 Financial and Insurance Industry Classifier: Intended Audience :: Other
 Audience Classifier: Intended Audience :: Science/Research Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.10 Description-Content-Type: text/markdown
-Provides-Extra: test Provides-Extra: dev Provides-Extra: docs Provides-Extra:
-publish License-File: LICENSE.txt
+Provides-Extra: test Provides-Extra: dev Provides-Extra: docs License-File:
+LICENSE.txt
 [https://raw.githubusercontent.com/fmilthaler/finquant/master/images/finquant-
                                    logo.png]
 [pypi] [pypi] [GitHub_Actions] [docs] [contributors] [contributions] [license]
 # FinQuant *FinQuant* is a program for financial **portfolio management,
 analysis and optimisation**. This README only gives a brief overview of
 *FinQuant*. The interested reader should refer to its [documentation](https://
 finquant.readthedocs.io "FinQuant Documentation"). ## Table of contents -
```

### Comparing `FinQuant-0.2.3/README.md` & `FinQuant-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 </p>
 
 <p align="center">
   <a href="https://GitHub.com/fmilthaler/FinQuant/stargazers/">
     <img src="https://img.shields.io/github/stars/fmilthaler/FinQuant.svg?style=social&label=Star" alt='pypi'>
   </a>
   <a href="https://pypi.org/project/FinQuant">
-    <img src="https://img.shields.io/badge/pypi-v0.2.2-brightgreen.svg?style=popout" alt='pypi'>
+    <img src="https://img.shields.io/badge/pypi-v0.3.0-brightgreen.svg?style=popout" alt='pypi'>
   </a>
   <a href="https://github.com/fmilthaler/FinQuant">
     <img src="https://github.com/fmilthaler/finquant/actions/workflows/pytest.yml/badge.svg?branch=master" alt='GitHub Actions'>
   </a>
   <a href="http://finquant.readthedocs.io/">
     <img src="https://img.shields.io/readthedocs/finquant.svg?style=popout" alt="docs">
   </a>
```

### Comparing `FinQuant-0.2.3/finquant/efficient_frontier.py` & `FinQuant-0.3.0/finquant/efficient_frontier.py`

 * *Files identical despite different names*

### Comparing `FinQuant-0.2.3/finquant/minimise_fun.py` & `FinQuant-0.3.0/finquant/minimise_fun.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 
 from finquant.quants import annualised_portfolio_quantities
 
 
 def portfolio_volatility(weights, mean_returns, cov_matrix):
-    """Calculates the volatility a portfolio
+    """Calculates the volatility of a portfolio
 
     :Input:
      :weights: numpy.ndarray, weights of the stocks in the portfolio
      :mean_returns: pandas.Series, individual expected returns for all stocks
          in the portfolio
      :cov_matrix: pandas.DataFrame, covariance matrix of returns
```

### Comparing `FinQuant-0.2.3/finquant/monte_carlo.py` & `FinQuant-0.3.0/finquant/monte_carlo.py`

 * *Files identical despite different names*

### Comparing `FinQuant-0.2.3/finquant/moving_average.py` & `FinQuant-0.3.0/finquant/moving_average.py`

 * *Files identical despite different names*

### Comparing `FinQuant-0.2.3/finquant/portfolio.py` & `FinQuant-0.3.0/finquant/portfolio.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 - cumulative returns of the portfolio's stocks
 - daily returns of the portfolio's stocks (daily percentage change),
 - daily log returns of the portfolio's stocks,
 - Expected (annualised) Return,
 - Volatility,
 - Sharpe Ratio,
+- Beta parameter (optional),
 - skewness of the portfolio's stocks,
 - Kurtosis of the portfolio's stocks,
 - the portfolio's covariance matrix.
 
 Furthermore, the constructed portfolio can be optimised for
 
 - minimum Volatility,
@@ -53,14 +54,15 @@
 from finquant.quants import weighted_mean, weighted_std, sharpe_ratio
 from finquant.returns import historical_mean_return
 from finquant.returns import daily_returns, cumulative_returns
 from finquant.returns import daily_log_returns
 from finquant.stock import Stock
 from finquant.efficient_frontier import EfficientFrontier
 from finquant.monte_carlo import MonteCarloOpt
+from finquant.market import Market
 
 
 class Portfolio(object):
     """Object that contains information about an investment portfolio.
     To initialise the object, it does not require any input.
     To fill the portfolio with investment information, the
     function ``add_stock(stock)`` should be used, in which ``stock`` is
@@ -81,14 +83,19 @@
         self.totalinvestment = None
         self.risk_free_rate = 0.005
         self.freq = 252
         # instance variables for Efficient Frontier and
         # Monte Carlo optimisations
         self.ef = None
         self.mc = None
+        # instance variable for Market class
+        self.market_index = None
+        # dataframe containing beta values of stocks
+        self.beta_stocks = pd.DataFrame(index=["beta"])
+        self.beta = None
 
     @property
     def totalinvestment(self):
         return self.__totalinvestment
 
     @totalinvestment.setter
     def totalinvestment(self, val):
@@ -127,14 +134,26 @@
         if not isinstance(val, (float, int)):
             raise ValueError("Risk free rate must be a float or an integer.")
         else:
             self.__risk_free_rate = val
             # now that this changed, update other quantities
             self._update()
 
+    @property
+    def market_index(self) -> Market:
+        return self.__market_index
+
+    @market_index.setter
+    def market_index(self, index: Market) -> None:
+        """Set the market index to the portfolio.
+
+        :param index: An object of the ``Market`` class.
+        """
+        self.__market_index = index
+
     def add_stock(self, stock):
         """Adds a stock of type ``Stock`` to the portfolio. Each time ``add_stock``
         is called, the following instance variables are updated:
 
         - ``portfolio``: ``pandas.DataFrame``, adds a column with information from ``stock``
         - ``stocks``: ``dictionary``, adds an entry for ``stock``
         - ``data``: ``pandas.DataFrame``, adds a column of stock prices from ``stock``
@@ -155,38 +174,46 @@
         # adding information of stock to the portfolio
         self.portfolio = pd.concat(
             [self.portfolio, stock.investmentinfo.to_frame().T], ignore_index=True
         )
         # setting an appropriate name for the portfolio
         self.portfolio.name = "Allocation of stocks"
         # also add stock data of stock to the dataframe
-        self._add_stock_data(stock.data)
+        self._add_stock_data(stock)
 
         # update quantities of portfolio
         self._update()
 
-    def _add_stock_data(self, df):
+    def _add_stock_data(self, stock: Stock) -> None:
         # loop over columns in given dataframe
-        for datacol in df.columns:
+        for datacol in stock.data.columns:
             cols = len(self.data.columns)
-            self.data.insert(loc=cols, column=datacol, value=df[datacol].values)
+            self.data.insert(loc=cols, column=datacol, value=stock.data[datacol].values)
         # set index correctly
-        self.data.set_index(df.index.values, inplace=True)
+        self.data.set_index(stock.data.index.values, inplace=True)
         # set index name:
         self.data.index.rename("Date", inplace=True)
 
+        if self.market_index is not None:
+            # compute beta parameter of stock
+            beta_stock = stock.comp_beta(self.market_index.daily_returns)
+            # add beta of stock to portfolio's betas dataframe
+            self.beta_stocks[stock.name] = [beta_stock]
+
     def _update(self):
         # sanity check (only update values if none of the below is empty):
         if not (self.portfolio.empty or self.stocks == {} or self.data.empty):
             self.totalinvestment = self.portfolio.Allocation.sum()
             self.expected_return = self.comp_expected_return(freq=self.freq)
             self.volatility = self.comp_volatility(freq=self.freq)
             self.sharpe = self.comp_sharpe()
             self.skew = self._comp_skew()
             self.kurtosis = self._comp_kurtosis()
+            if self.market_index is not None:
+                self.beta = self.comp_beta()
 
     def get_stock(self, name):
         """Returns the instance of ``Stock`` with name ``name``.
 
         :Input:
          :name: ``string`` of the name of the stock that is returned. Must match
              one of the labels in the dictionary ``self.stocks``.
@@ -320,14 +347,28 @@
         # compute the Sharpe Ratio of the portfolio
         sharpe = sharpe_ratio(
             self.expected_return, self.volatility, self.risk_free_rate
         )
         self.sharpe = sharpe
         return sharpe
 
+    def comp_beta(self) -> float:
+        """Compute and return the Beta parameter of the portfolio.
+
+        :Output:
+         :sharpe: ``float``, the Beta parameter of the portfolio
+        """
+
+        # compute the Beta parameter of the portfolio
+        weights = self.comp_weights()
+        beta = weighted_mean(self.beta_stocks.transpose()["beta"].values, weights)
+
+        self.beta = beta
+        return beta
+
     def _comp_skew(self):
         """Computes and returns the skewness of the stocks in the portfolio."""
         return self.data.skew()
 
     def _comp_kurtosis(self):
         """Computes and returns the Kurtosis of the stocks in the portfolio."""
         return self.data.kurt()
@@ -582,28 +623,33 @@
 
     def properties(self):
         """Nicely prints out the properties of the portfolio:
 
         - Expected Return,
         - Volatility,
         - Sharpe Ratio,
+        - Beta (optional),
         - skewness,
         - Kurtosis
 
         as well as the allocation of the stocks across the portfolio.
         """
         # nicely printing out information and quantities of the portfolio
         string = "-" * 70
         stocknames = self.portfolio.Name.values.tolist()
         string += "\nStocks: {}".format(", ".join(stocknames))
+        if self.market_index is not None:
+            string += "\nMarket Index: {}".format(self.market_index.name)
         string += "\nTime window/frequency: {}".format(self.freq)
         string += "\nRisk free rate: {}".format(self.risk_free_rate)
         string += "\nPortfolio Expected Return: {:0.3f}".format(self.expected_return)
         string += "\nPortfolio Volatility: {:0.3f}".format(self.volatility)
         string += "\nPortfolio Sharpe Ratio: {:0.3f}".format(self.sharpe)
+        if self.beta is not None:
+            string += "\nPortfolio Beta: {:0.3f}".format(self.beta)
         string += "\n\nSkewness:"
         string += "\n" + str(self.skew.to_frame().transpose())
         string += "\n\nKurtosis:"
         string += "\n" + str(self.kurtosis.to_frame().transpose())
         string += "\n\nInformation:"
         string += "\n" + str(self.portfolio)
         string += "\n"
@@ -795,15 +841,20 @@
                 {_get_quandl_data_column_label(names[i], cols[0]): names[i]}
             )
         data.rename(columns=newcolnames, inplace=True)
     return data
 
 
 def _build_portfolio_from_api(
-    names, pf_allocation=None, start_date=None, end_date=None, data_api="quandl"
+    names,
+    pf_allocation=None,
+    start_date=None,
+    end_date=None,
+    data_api="quandl",
+    market_index: str = None,
 ):
     """Returns a portfolio based on input in form of a list of strings/names
     of stocks.
 
     :Input:
      :names: A string or list of strings, containing the names of the
          stocks, e.g. 'GOOG' for Google.
@@ -813,41 +864,64 @@
          be requested through `quandl`/`yfinance` (default: None)
      :end_date (optional): String/datetime end date of stock data to be
          requested through `quandl`/`yfinance` (default: None)
      :data_api: (optional) A ``string`` (default: ``quandl``) which determines how to
          obtain stock prices, if data is not provided by the user. Valid values:
          - ``quandl`` (Python package/API to `Quandl`)
          - ``yfinance`` (Python package formerly known as ``fix-yahoo-finance``)
+     :market_index: (optional) ``string`` (default: ``None``) which determines the
+         market index to be used for the computation of the beta parameter of the stocks.
 
     :Output:
      :pf: Instance of Portfolio which contains all the information
          requested by the user.
     """
     # create an empty portfolio
     pf = Portfolio()
+    # create empty dataframe for market data
+    market_data = pd.DataFrame()
     # request data from service:
     if data_api == "yfinance":
         data = _yfinance_request(names, start_date, end_date)
+        if market_index is not None:
+            market_data = _yfinance_request([market_index], start_date, end_date)
     elif data_api == "quandl":
         data = _quandl_request(names, start_date, end_date)
+        if market_index is not None:
+            # only generated if user explicitly requests market index with quandl
+            raise Warning("Market index is not supported for quandl data.")
     # check pf_allocation:
     if pf_allocation is None:
         pf_allocation = _generate_pf_allocation(names=names)
     # build portfolio:
-    pf = _build_portfolio_from_df(data, pf_allocation)
+    pf = _build_portfolio_from_df(data, pf_allocation, market_data=market_data)
     return pf
 
 
 def _stocknames_in_data_columns(names, df):
     """Returns True if at least one element of names was found as a column
     label in the dataframe df.
     """
     return any((name in label for name in names for label in df.columns))
 
 
+def _get_index_adj_clos_pr(data: pd.DataFrame) -> pd.Series:
+    """This function returns a subset of the given ``pandas.DataFrame`` data, which
+    contains only the data columns corresponding to Adjusted Closing Price.
+
+    :Input:
+     :data: A ``pandas.DataFrame`` which contains financial data.
+
+    :Output:
+     :data: A ``pandas.Series`` which contains only the data column of
+         data corresponding to Adjusted Closing Price.
+    """
+    return data["Adj Close"].squeeze()
+
+
 def _generate_pf_allocation(names=None, data=None):
     """Takes column names of provided ``pandas.DataFrame`` ``data``, and generates a
     ``pandas.DataFrame`` with columns ``Name`` and ``Allocation`` which contain the
     names found in input ``data`` and 1.0/len(data.columns) respectively.
 
     :Input:
      :data: A ``pandas.DataFrame`` which contains prices of the stocks
@@ -901,26 +975,33 @@
                 raise ValueError(errormsg)
     # if names is given, we go directly to the below:
     # compute equal weights
     weights = [1.0 / len(names) for i in range(len(names))]
     return pd.DataFrame({"Allocation": weights, "Name": names})
 
 
-def _build_portfolio_from_df(data, pf_allocation=None, datacolumns=["Adj. Close"]):
+def _build_portfolio_from_df(
+    data: pd.DataFrame,
+    pf_allocation: pd.DataFrame = None,
+    datacolumns: list = ["Adj. Close"],
+    market_data: pd.DataFrame = None,
+) -> Portfolio:
     """Returns a portfolio based on input in form of ``pandas.DataFrame``.
 
     :Input:
      :data: A ``pandas.DataFrame`` which contains prices of the stocks listed in
          pf_allocation
      :pf_allocation: (optional) ``pandas.DataFrame`` with the required data column
          labels ``Name`` and ``Allocation`` of the stocks. If not given, it is
          automatically generated with an equal weights for all stocks
          in the resulting portfolio.
      :datacolumns: (optional) A list of strings of data column labels
          to be extracted and returned (default: ["Adj. Close"]).
+     :market_data: (optional) A ``pandas.DataFrame`` which contains data of the
+         market index (default: ``None``).
 
     :Output:
      :pf: Instance of Portfolio which contains all the information
          requested by the user.
     """
     # if pf_allocation is None, automatically generate it
     if pf_allocation is None:
@@ -932,14 +1013,19 @@
             + "found in the provided dataframe."
         )
     # extract only "Adjusted Close" price ("Adj. Close" in quandl, "Adj Close" in yfinance)
     # column from DataFrame:
     data = _get_stocks_data_columns(data, pf_allocation.Name.values, datacolumns)
     # building portfolio:
     pf = Portfolio()
+    if market_data is not None and not market_data.empty:
+        # extract only "Adjusted Close" price column from market data
+        market_data = _get_index_adj_clos_pr(market_data)
+        # set market index of portfolio
+        pf.market_index = Market(data=market_data)
     for i in range(len(pf_allocation)):
         # get name of stock
         name = pf_allocation.loc[i].Name
         # extract data column(s) of said stock
         stock_data = data.loc[:, [name]].copy(deep=True)
         # if only one data column per stock exists, give dataframe a name
         if len(datacolumns) == 1:
@@ -983,21 +1069,24 @@
          the stocks listed in ``pf_allocation``.
      :data_api: (optional) A ``string`` (default: ``quandl``) which determines how to
          obtain stock prices, if data is not provided by the user. Valid values:
 
          - ``quandl`` (Python package/API to `Quandl`)
          - ``yfinance`` (Python package formerly known as ``fix-yahoo-finance``)
 
+     :market_index: (optional) ``string`` (default: ``None``) which determines the
+         market index to be used for the computation of the beta parameter of the stocks.
+
     :Output:
      :pf: Instance of ``Portfolio`` which contains all the information
          requested by the user.
 
     .. note:: Only the following combinations of inputs are allowed:
 
-     - ``names``, ``pf_allocation`` (optional), ``start_date`` (optional), ``end_date`` (optional), data_api (optional)
+     - ``names``, ``pf_allocation`` (optional), ``start_date`` (optional), ``end_date`` (optional), data_api (optional), ``market_index`` (optional)
      - ``data``, ``pf_allocation`` (optional)
 
      The two different ways this function can be used are useful for:
 
      1. building a portfolio by pulling data from `quandl`/`yfinance`,
      2. building a portfolio by providing stock data which was obtained otherwise,
         e.g. from data files.
@@ -1026,14 +1115,15 @@
     all_input_args = [
         "pf_allocation",
         "names",
         "start_date",
         "end_date",
         "data",
         "data_api",
+        "market_index",
     ]
 
     # check if no input argument was passed
     if kwargs == {}:
         raise ValueError(
             "Error:\nbuild_portfolio() requires input " + "arguments.\n" + docstring_msg
         )
@@ -1043,22 +1133,23 @@
         raise ValueError(
             "Error:\n" + input_error.format(unsupported_input, all_input_args)
         )
 
     # create an empty portfolio
     pf = Portfolio()
 
-    # 1. pf_allocation, names, start_date, end_date, data_api
+    # 1. pf_allocation, names, start_date, end_date, data_api, market_index
     allowed_mandatory_args = ["names"]
     allowed_input_args = [
         "names",
         "pf_allocation",
         "start_date",
         "end_date",
         "data_api",
+        "market_index",
     ]
     complement_input_args = _list_complement(allowed_input_args, all_input_args)
     if _all_list_ele_in_other(allowed_mandatory_args, kwargs.keys()):
         # check that no input argument conflict arises:
         if _any_list_ele_in_other(complement_input_args, kwargs.keys()):
             raise ValueError(
                 input_comb_error.format(complement_input_args, allowed_mandatory_args)
```

### Comparing `FinQuant-0.2.3/finquant/quants.py` & `FinQuant-0.3.0/finquant/quants.py`

 * *Files identical despite different names*

### Comparing `FinQuant-0.2.3/finquant/returns.py` & `FinQuant-0.3.0/finquant/returns.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,17 +51,17 @@
     return np.log(1 + daily_returns(data)).dropna(how="all")
 
 
 def historical_mean_return(data, freq=252):
     """Returns the mean return based on historical stock price data.
 
     :Input:
-     :data: ``pandas.DataFrame`` with daily stock prices
+     :data: ``pandas.DataFrame`` or ``pandas.Series`` with daily stock prices
      :freq: ``int`` (default= ``252``), number of trading days, default
              value corresponds to trading days in a year
 
     :Output:
-     :ret: a ``pandas.DataFrame`` of historical mean Returns.
+     :ret: a ``pandas.Series`` or ``numpy.float`` of historical mean Returns.
     """
-    if not isinstance(data, pd.DataFrame):
-        raise ValueError("data must be a pandas.DataFrame")
+    if not isinstance(data, (pd.DataFrame, pd.Series)):
+        raise ValueError("data must be a pandas.DataFrame or pandas.Series")
     return daily_returns(data).mean() * freq
```

### Comparing `FinQuant-0.2.3/finquant/stock.py` & `FinQuant-0.3.0/finquant/stock.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """ This module provides a public class ``Stock`` that holds and calculates quantities of a single stock.
 Instances of this class are used in the ``Portfolio`` class (provided in ``finquant.portfolio``).   
 Every time a new instance of ``Stock`` is added to ``Portfolio``, the quantities of the portfolio are updated.  
 """
 
 import numpy as np
+import pandas as pd
 from finquant.returns import historical_mean_return
 from finquant.returns import daily_returns
 
 
 class Stock(object):
     """Object that contains information about a stock/fund.
     To initialise the object, it requires a name, information about
@@ -44,14 +45,16 @@
         self.investmentinfo = investmentinfo
         self.data = data
         # compute expected return and volatility of stock
         self.expected_return = self.comp_expected_return()
         self.volatility = self.comp_volatility()
         self.skew = self._comp_skew()
         self.kurtosis = self._comp_kurtosis()
+        # beta parameter of stock (CAPM)
+        self.beta = None
 
     # functions to compute quantities
     def comp_daily_returns(self):
         """Computes the daily returns (percentage change).
         See ``finquant.returns.daily_returns``.
         """
         return daily_returns(self.data)
@@ -84,14 +87,32 @@
         """Computes and returns the skewness of the stock."""
         return self.data.skew().values[0]
 
     def _comp_kurtosis(self):
         """Computes and returns the Kurtosis of the stock."""
         return self.data.kurt().values[0]
 
+    def comp_beta(self, market_daily_returns: pd.Series) -> float:
+        """Compute and return the Beta parameter of the stock.
+
+        :Input:
+         :market_daily_returns: ``pd.Series``, daily returns of the market
+
+        :Output:
+         :sharpe: ``float``, the Beta parameter of the stock
+        """
+        cov_mat = np.cov(
+            self.comp_daily_returns()[self.name],
+            market_daily_returns.to_frame()[market_daily_returns.name],
+        )
+
+        beta = cov_mat[0, 1] / cov_mat[1, 1]
+        self.beta = beta
+        return beta
+
     def properties(self):
         """Nicely prints out the properties of the stock: Expected Return,
         Volatility, Skewness, Kurtosis as well as the ``Allocation`` (and other
         information provided in investmentinfo.)
         """
         # nicely printing out information and quantities of the stock
         string = "-" * 50
```

### Comparing `FinQuant-0.2.3/setup.py` & `FinQuant-0.3.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
 install_requires = read_requirements("requirements.txt")
 
 extras_require = {
     "test": read_requirements("requirements_test.txt"),
     "dev": read_requirements("requirements_dev.txt"),
     "docs": read_requirements("requirements_docs.txt"),
-    "publish": read_requirements("requirements_publish.txt"),
 }
 
 setuptools.setup(
     name="FinQuant",
     version=version["version"],
     author="Frank Milthaler",
     author_email="f.milthaler@gmail.com",
```

### Comparing `FinQuant-0.2.3/tests/test_moving_average.py` & `FinQuant-0.3.0/tests/test_moving_average.py`

 * *Files identical despite different names*

### Comparing `FinQuant-0.2.3/tests/test_portfolio.py` & `FinQuant-0.3.0/tests/test_portfolio.py`

 * *Files identical despite different names*

### Comparing `FinQuant-0.2.3/tests/test_quants.py` & `FinQuant-0.3.0/tests/test_quants.py`

 * *Files identical despite different names*

### Comparing `FinQuant-0.2.3/tests/test_returns.py` & `FinQuant-0.3.0/tests/test_returns.py`

 * *Files identical despite different names*

### Comparing `FinQuant-0.2.3/tests/test_stock.py` & `FinQuant-0.3.0/tests/test_stock.py`

 * *Files identical despite different names*

