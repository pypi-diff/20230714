# Comparing `tmp/vnstock-0.1.6.tar.gz` & `tmp/vnstock-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnstock-0.1.6.tar", last modified: Thu Jun 22 13:08:14 2023, max compression
+gzip compressed data, was "vnstock-0.1.7.tar", last modified: Fri Jul 14 16:12:56 2023, max compression
```

## Comparing `vnstock-0.1.6.tar` & `vnstock-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 13:08:14.582264 vnstock-0.1.6/
--rw-rw-rw-   0        0        0     1071 2022-02-26 11:38:24.000000 vnstock-0.1.6/LICENSE
--rw-rw-rw-   0        0        0    42776 2023-06-22 13:08:14.584257 vnstock-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0    42349 2023-06-22 12:15:44.000000 vnstock-0.1.6/README.md
--rw-rw-rw-   0        0        0      146 2023-06-22 12:09:26.000000 vnstock-0.1.6/pyproject.toml
--rw-rw-rw-   0        0        0      512 2023-06-22 13:08:14.595227 vnstock-0.1.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-22 13:08:14.552344 vnstock-0.1.6/vnstock/
--rw-rw-rw-   0        0        0      180 2023-06-22 12:46:57.000000 vnstock-0.1.6/vnstock/__init__.py
--rw-rw-rw-   0        0        0    22767 2023-06-22 12:25:09.000000 vnstock-0.1.6/vnstock/stock.py
--rw-rw-rw-   0        0        0     2398 2023-06-08 05:54:52.000000 vnstock-0.1.6/vnstock/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-22 13:08:14.580266 vnstock-0.1.6/vnstock.egg-info/
--rw-rw-rw-   0        0        0    42776 2023-06-22 13:08:14.000000 vnstock-0.1.6/vnstock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-06-22 13:08:14.000000 vnstock-0.1.6/vnstock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 13:08:14.000000 vnstock-0.1.6/vnstock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-22 13:08:14.000000 vnstock-0.1.6/vnstock.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 16:12:56.561059 vnstock-0.1.7/
+-rw-rw-rw-   0        0        0     1071 2022-02-26 11:38:24.000000 vnstock-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0    98703 2023-07-14 16:12:56.563054 vnstock-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0    98276 2023-07-14 16:10:07.000000 vnstock-0.1.7/README.md
+-rw-rw-rw-   0        0        0      146 2023-06-22 12:09:26.000000 vnstock-0.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0      512 2023-07-14 16:12:56.566047 vnstock-0.1.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-14 16:12:56.531140 vnstock-0.1.7/vnstock/
+-rw-rw-rw-   0        0        0      178 2023-07-13 14:02:40.000000 vnstock-0.1.7/vnstock/__init__.py
+-rw-rw-rw-   0        0        0    59076 2023-07-14 16:02:18.000000 vnstock-0.1.7/vnstock/stock.py
+-rw-rw-rw-   0        0        0     2929 2023-07-13 14:01:17.000000 vnstock-0.1.7/vnstock/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-14 16:12:56.559064 vnstock-0.1.7/vnstock.egg-info/
+-rw-rw-rw-   0        0        0    98703 2023-07-14 16:12:56.000000 vnstock-0.1.7/vnstock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2023-07-14 16:12:56.000000 vnstock-0.1.7/vnstock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 16:12:56.000000 vnstock-0.1.7/vnstock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-14 16:12:56.000000 vnstock-0.1.7/vnstock.egg-info/top_level.txt
```

### Comparing `vnstock-0.1.6/LICENSE` & `vnstock-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vnstock-0.1.6/setup.cfg` & `vnstock-0.1.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6e73 746f 636b 0d0a 7665 7273   = vnstock..vers
-00000020: 696f 6e20 3d20 302e 312e 360d 0a61 7574  ion = 0.1.6..aut
+00000020: 696f 6e20 3d20 302e 312e 370d 0a61 7574  ion = 0.1.7..aut
 00000030: 686f 7220 3d20 5468 696e 6820 5675 0d0a  hor = Thinh Vu..
 00000040: 6175 7468 6f72 5f65 6d61 696c 203d 206d  author_email = m
 00000050: 7274 6869 6e68 406c 6976 652e 636f 6d0d  rthinh@live.com.
 00000060: 0a64 6573 6372 6970 7469 6f6e 203d 2056  .description = V
 00000070: 6965 746e 616d 2053 746f 636b 204d 6172  ietnam Stock Mar
 00000080: 6b65 7420 4461 7461 0d0a 6c6f 6e67 5f64  ket Data..long_d
 00000090: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
```

### Comparing `vnstock-0.1.6/vnstock/utils.py` & `vnstock-0.1.7/vnstock/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,22 @@
-# from datetime import datetime, timedelta
+from datetime import datetime, timedelta
+
+def get_date(n, unit):
+    """
+    Return YYYY-mm-dd value from today to n days, months or years in the past
+    Parameters:
+        n: number of days, months or years
+        unit: 'day', 'month' or 'year'
+    """
+    if unit == 'day':
+        return (datetime.now() - timedelta(days=n)).strftime('%Y-%m-%d')
+    elif unit == 'month':
+        return (datetime.now() - relativedelta(months=n)).strftime('%Y-%m-%d')
+    elif unit == 'year':
+        return (datetime.now() - relativedelta(years=n)).strftime('%Y-%m-%d')
 
 # def previous_weekday (date):
 #   date_value = datetime.strptime(date, '%Y-%m-%d')
 #   weekday_name = date_value.strftime('%a')
 #   if weekday_name == 'Sun':
 #     prev_weekday_date = date_value - timedelta(days=2)
 #   elif weekday_name == 'Mon':
```

