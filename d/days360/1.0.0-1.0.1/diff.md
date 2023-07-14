# Comparing `tmp/days360-1.0.0.tar.gz` & `tmp/days360-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "days360-1.0.0.tar", max compression
+gzip compressed data, was "days360-1.0.1.tar", max compression
```

## Comparing `days360-1.0.0.tar` & `days360-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1073 2023-07-12 16:46:32.936705 days360-1.0.0/Readme.md
--rw-r--r--   0        0        0      159 2023-07-12 15:25:38.141249 days360-1.0.0/days360/__init__.py
--rw-r--r--   0        0        0     3275 2023-07-12 16:10:03.393954 days360-1.0.0/days360/days360.py
--rw-r--r--   0        0        0        0 2023-07-12 16:46:31.405282 days360-1.0.0/days360/py.typed
--rw-r--r--   0        0        0      435 2023-07-12 16:47:37.195393 days360-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1636 1970-01-01 00:00:00.000000 days360-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-13 10:39:25.029115 days360-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     1296 2023-07-13 10:46:21.167801 days360-1.0.1/README.md
+-rw-r--r--   0        0        0      159 2023-07-12 15:25:38.141249 days360-1.0.1/days360/__init__.py
+-rw-r--r--   0        0        0     3275 2023-07-14 13:17:15.989300 days360-1.0.1/days360/days360.py
+-rw-r--r--   0        0        0        0 2023-07-12 16:46:31.405282 days360-1.0.1/days360/py.typed
+-rw-r--r--   0        0        0      773 2023-07-14 13:34:51.720591 days360-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2117 1970-01-01 00:00:00.000000 days360-1.0.1/PKG-INFO
```

### Comparing `days360-1.0.0/Readme.md` & `days360-1.0.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -28,13 +28,16 @@
 # supported methods: "US" (default), "US_NASD", "EU"
 days = days360(date_a, date_b, method="US")
 print(days)  # prints 418
 ```
 
 ## Planned
 
-- ISDA and PSA methods.
+- ISDA, PSA and SIA methods
+  - https://www.isda.org/2008/12/22/30-360-day-count-conventions/)
+  - https://web.archive.org/web/20160425044113/http://www.nyift.com/lesson/day-count-convention-bonds/
+  - https://github.com/miradulo/isda_daycounters
 
 ## Notes and credits
 
 - Implementations are based on https://en.wikipedia.org/wiki/360-day_calendar.
 - This library started as a port of this ruby gem: https://github.com/tamaloa/days360/tree/master
```

#### html2text {}

```diff
@@ -4,10 +4,13 @@
 two dates based on the 360-day year. - Implementation of Excel's (or Number's)
 `DAYS360` / `TAGE360` formula in python. - Both EU and US methods of
 calculation are supported, with optional Excel bug compatibility. ##
 Installation ``` pip install days360 ``` ## Usage ```python from datetime
 import date from days360 import days360 date_a = date(2022, 10, 2) date_b =
 date(2023, 11, 30) # supported methods: "US" (default), "US_NASD", "EU" days =
 days360(date_a, date_b, method="US") print(days) # prints 418 ``` ## Planned -
-ISDA and PSA methods. ## Notes and credits - Implementations are based on
-https://en.wikipedia.org/wiki/360-day_calendar. - This library started as a
-port of this ruby gem: https://github.com/tamaloa/days360/tree/master
+ISDA, PSA and SIA methods - https://www.isda.org/2008/12/22/30-360-day-count-
+conventions/) - https://web.archive.org/web/20160425044113/http://
+www.nyift.com/lesson/day-count-convention-bonds/ - https://github.com/miradulo/
+isda_daycounters ## Notes and credits - Implementations are based on https://
+en.wikipedia.org/wiki/360-day_calendar. - This library started as a port of
+this ruby gem: https://github.com/tamaloa/days360/tree/master
```

### Comparing `days360-1.0.0/days360/days360.py` & `days360-1.0.1/days360/days360.py`

 * *Files identical despite different names*

### Comparing `days360-1.0.0/PKG-INFO` & `days360-1.0.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 Metadata-Version: 2.1
 Name: days360
-Version: 1.0.0
-Summary: Calculates the days between two dates based on a 360 day year.
+Version: 1.0.1
+Summary: Excel's DAYS360() formula for python.
+Home-page: https://github.com/tfeldmann/organize
 License: MIT
+Keywords: excel,formula,finance,days360
 Author: Thomas Feldmann
 Author-email: mail@tfeldmann.de
 Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Typing :: Typed
+Project-URL: Repository, https://github.com/tfeldmann/organize
 Description-Content-Type: text/markdown
 
 # days360
 
 [![Tests](https://github.com/tfeldmann/days360/actions/workflows/tests.yml/badge.svg)](https://github.com/tfeldmann/days360/actions/workflows/tests.yml)
 <a href="https://pypi.org/project/days360/">
   <img src="https://img.shields.io/pypi/v/days360" title="PyPI Version">
@@ -44,14 +50,17 @@
 # supported methods: "US" (default), "US_NASD", "EU"
 days = days360(date_a, date_b, method="US")
 print(days)  # prints 418
 ```
 
 ## Planned
 
-- ISDA and PSA methods.
+- ISDA, PSA and SIA methods
+  - https://www.isda.org/2008/12/22/30-360-day-count-conventions/)
+  - https://web.archive.org/web/20160425044113/http://www.nyift.com/lesson/day-count-convention-bonds/
+  - https://github.com/miradulo/isda_daycounters
 
 ## Notes and credits
 
 - Implementations are based on https://en.wikipedia.org/wiki/360-day_calendar.
 - This library started as a port of this ruby gem: https://github.com/tamaloa/days360/tree/master
```

#### html2text {}

```diff
@@ -1,20 +1,27 @@
-Metadata-Version: 2.1 Name: days360 Version: 1.0.0 Summary: Calculates the days
-between two dates based on a 360 day year. License: MIT Author: Thomas Feldmann
-Author-email: mail@tfeldmann.de Requires-Python: >=3.8,<4.0 Classifier: License
-:: OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Description-Content-Type:
-text/markdown # days360 [![Tests](https://github.com/tfeldmann/days360/actions/
-workflows/tests.yml/badge.svg)](https://github.com/tfeldmann/days360/actions/
-workflows/tests.yml) [https://img.shields.io/pypi/v/days360] Calculates the
-days between two dates based on the 360-day year. - Implementation of Excel's
-(or Number's) `DAYS360` / `TAGE360` formula in python. - Both EU and US methods
-of calculation are supported, with optional Excel bug compatibility. ##
-Installation ``` pip install days360 ``` ## Usage ```python from datetime
-import date from days360 import days360 date_a = date(2022, 10, 2) date_b =
-date(2023, 11, 30) # supported methods: "US" (default), "US_NASD", "EU" days =
-days360(date_a, date_b, method="US") print(days) # prints 418 ``` ## Planned -
-ISDA and PSA methods. ## Notes and credits - Implementations are based on
-https://en.wikipedia.org/wiki/360-day_calendar. - This library started as a
-port of this ruby gem: https://github.com/tamaloa/days360/tree/master
+Metadata-Version: 2.1 Name: days360 Version: 1.0.1 Summary: Excel's DAYS360()
+formula for python. Home-page: https://github.com/tfeldmann/organize License:
+MIT Keywords: excel,formula,finance,days360 Author: Thomas Feldmann Author-
+email: mail@tfeldmann.de Requires-Python: >=3.8,<4.0 Classifier: Development
+Status :: 5 - Production/Stable Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Typing :: Typed Project-URL: Repository, https://github.com/
+tfeldmann/organize Description-Content-Type: text/markdown # days360 [![Tests]
+(https://github.com/tfeldmann/days360/actions/workflows/tests.yml/badge.svg)]
+(https://github.com/tfeldmann/days360/actions/workflows/tests.yml) [https://
+img.shields.io/pypi/v/days360] Calculates the days between two dates based on
+the 360-day year. - Implementation of Excel's (or Number's) `DAYS360` /
+`TAGE360` formula in python. - Both EU and US methods of calculation are
+supported, with optional Excel bug compatibility. ## Installation ``` pip
+install days360 ``` ## Usage ```python from datetime import date from days360
+import days360 date_a = date(2022, 10, 2) date_b = date(2023, 11, 30) #
+supported methods: "US" (default), "US_NASD", "EU" days = days360(date_a,
+date_b, method="US") print(days) # prints 418 ``` ## Planned - ISDA, PSA and
+SIA methods - https://www.isda.org/2008/12/22/30-360-day-count-conventions/) -
+https://web.archive.org/web/20160425044113/http://www.nyift.com/lesson/day-
+count-convention-bonds/ - https://github.com/miradulo/isda_daycounters ## Notes
+and credits - Implementations are based on https://en.wikipedia.org/wiki/360-
+day_calendar. - This library started as a port of this ruby gem: https://
+github.com/tamaloa/days360/tree/master
```

