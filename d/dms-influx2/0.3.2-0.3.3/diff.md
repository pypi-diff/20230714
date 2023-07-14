# Comparing `tmp/dms-influx2-0.3.2.tar.gz` & `tmp/dms-influx2-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dms-influx2-0.3.2.tar", last modified: Fri Jul 14 12:10:59 2023, max compression
+gzip compressed data, was "dist\dms-influx2-0.3.3.tar", last modified: Fri Jul 14 12:57:15 2023, max compression
```

## Comparing `dms-influx2-0.3.2.tar` & `dms-influx2-0.3.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 12:10:59.370574 dms-influx2-0.3.2/
--rw-rw-rw-   0        0        0      556 2023-07-14 12:10:59.369575 dms-influx2-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-01-09 21:18:36.000000 dms-influx2-0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 12:10:59.347227 dms-influx2-0.3.2/dms_influx2/
--rw-rw-rw-   0        0        0        0 2023-01-09 21:18:36.000000 dms-influx2-0.3.2/dms_influx2/__init__.py
--rw-rw-rw-   0        0        0     5108 2023-01-09 21:18:36.000000 dms-influx2-0.3.2/dms_influx2/authorizations.py
--rw-rw-rw-   0        0        0     6376 2023-03-22 11:19:56.000000 dms-influx2-0.3.2/dms_influx2/buckets.py
--rw-rw-rw-   0        0        0     5591 2023-01-19 07:18:35.000000 dms-influx2-0.3.2/dms_influx2/checks.py
--rw-rw-rw-   0        0        0      630 2023-01-09 21:18:36.000000 dms-influx2-0.3.2/dms_influx2/decorators.py
--rw-rw-rw-   0        0        0     2729 2023-07-03 09:35:10.000000 dms-influx2-0.3.2/dms_influx2/delete.py
--rw-rw-rw-   0        0        0     1487 2023-01-19 06:30:10.000000 dms-influx2-0.3.2/dms_influx2/dtv_files.py
--rw-rw-rw-   0        0        0      327 2023-01-09 21:18:36.000000 dms-influx2-0.3.2/dms_influx2/exceptions.py
--rw-rw-rw-   0        0        0    24601 2023-07-14 12:04:20.000000 dms-influx2-0.3.2/dms_influx2/lib.py
--rw-rw-rw-   0        0        0     3562 2023-01-09 21:18:36.000000 dms-influx2-0.3.2/dms_influx2/notifications.py
--rw-rw-rw-   0        0        0     1012 2023-01-09 21:18:36.000000 dms-influx2-0.3.2/dms_influx2/organisations.py
--rw-rw-rw-   0        0        0     7217 2023-07-04 18:39:09.000000 dms-influx2-0.3.2/dms_influx2/query.py
--rw-rw-rw-   0        0        0        0 2023-01-18 17:42:37.000000 dms-influx2-0.3.2/dms_influx2/sync.py
--rw-rw-rw-   0        0        0     4025 2023-01-09 21:18:36.000000 dms-influx2-0.3.2/dms_influx2/tasks.py
--rw-rw-rw-   0        0        0     1203 2023-01-26 19:35:58.000000 dms-influx2-0.3.2/dms_influx2/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-14 12:10:59.356922 dms-influx2-0.3.2/dms_influx2.egg-info/
--rw-rw-rw-   0        0        0      556 2023-07-14 12:10:59.000000 dms-influx2-0.3.2/dms_influx2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      636 2023-07-14 12:10:59.000000 dms-influx2-0.3.2/dms_influx2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 12:10:59.000000 dms-influx2-0.3.2/dms_influx2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-07-14 12:10:59.000000 dms-influx2-0.3.2/dms_influx2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-14 12:10:59.000000 dms-influx2-0.3.2/dms_influx2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 12:10:59.370574 dms-influx2-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     3023 2023-07-14 12:10:30.000000 dms-influx2-0.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-14 12:10:59.369575 dms-influx2-0.3.2/tests/
--rw-rw-rw-   0        0        0     1882 2023-07-03 09:02:50.000000 dms-influx2-0.3.2/tests/test_auth.py
--rw-rw-rw-   0        0        0     4632 2023-07-03 09:02:50.000000 dms-influx2-0.3.2/tests/test_buckets.py
--rw-rw-rw-   0        0        0     2018 2023-07-03 09:11:49.000000 dms-influx2-0.3.2/tests/test_copy-values.py
--rw-rw-rw-   0        0        0    16796 2023-07-14 12:09:20.000000 dms-influx2-0.3.2/tests/test_data.py
+drwxrwxrwx   0        0        0        0 2023-07-14 12:57:15.619992 dms-influx2-0.3.3/
+-rw-rw-rw-   0        0        0      556 2023-07-14 12:57:15.618992 dms-influx2-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-01-09 21:18:36.000000 dms-influx2-0.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 12:57:15.613953 dms-influx2-0.3.3/dms_influx2/
+-rw-rw-rw-   0        0        0        0 2023-01-09 21:18:36.000000 dms-influx2-0.3.3/dms_influx2/__init__.py
+-rw-rw-rw-   0        0        0     5108 2023-01-09 21:18:36.000000 dms-influx2-0.3.3/dms_influx2/authorizations.py
+-rw-rw-rw-   0        0        0     6376 2023-03-22 11:19:56.000000 dms-influx2-0.3.3/dms_influx2/buckets.py
+-rw-rw-rw-   0        0        0     5591 2023-01-19 07:18:35.000000 dms-influx2-0.3.3/dms_influx2/checks.py
+-rw-rw-rw-   0        0        0      630 2023-01-09 21:18:36.000000 dms-influx2-0.3.3/dms_influx2/decorators.py
+-rw-rw-rw-   0        0        0     2729 2023-07-03 09:35:10.000000 dms-influx2-0.3.3/dms_influx2/delete.py
+-rw-rw-rw-   0        0        0     1487 2023-01-19 06:30:10.000000 dms-influx2-0.3.3/dms_influx2/dtv_files.py
+-rw-rw-rw-   0        0        0      327 2023-01-09 21:18:36.000000 dms-influx2-0.3.3/dms_influx2/exceptions.py
+-rw-rw-rw-   0        0        0    25256 2023-07-14 12:55:32.000000 dms-influx2-0.3.3/dms_influx2/lib.py
+-rw-rw-rw-   0        0        0     3562 2023-01-09 21:18:36.000000 dms-influx2-0.3.3/dms_influx2/notifications.py
+-rw-rw-rw-   0        0        0     1012 2023-01-09 21:18:36.000000 dms-influx2-0.3.3/dms_influx2/organisations.py
+-rw-rw-rw-   0        0        0     7217 2023-07-04 18:39:09.000000 dms-influx2-0.3.3/dms_influx2/query.py
+-rw-rw-rw-   0        0        0        0 2023-01-18 17:42:37.000000 dms-influx2-0.3.3/dms_influx2/sync.py
+-rw-rw-rw-   0        0        0     4025 2023-01-09 21:18:36.000000 dms-influx2-0.3.3/dms_influx2/tasks.py
+-rw-rw-rw-   0        0        0     1203 2023-01-26 19:35:58.000000 dms-influx2-0.3.3/dms_influx2/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-14 12:57:15.616993 dms-influx2-0.3.3/dms_influx2.egg-info/
+-rw-rw-rw-   0        0        0      556 2023-07-14 12:57:15.000000 dms-influx2-0.3.3/dms_influx2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      636 2023-07-14 12:57:15.000000 dms-influx2-0.3.3/dms_influx2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 12:57:15.000000 dms-influx2-0.3.3/dms_influx2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-07-14 12:57:15.000000 dms-influx2-0.3.3/dms_influx2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-14 12:57:15.000000 dms-influx2-0.3.3/dms_influx2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 12:57:15.619992 dms-influx2-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     3023 2023-07-14 12:56:51.000000 dms-influx2-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 12:57:15.618992 dms-influx2-0.3.3/tests/
+-rw-rw-rw-   0        0        0     1882 2023-07-03 09:02:50.000000 dms-influx2-0.3.3/tests/test_auth.py
+-rw-rw-rw-   0        0        0     4632 2023-07-03 09:02:50.000000 dms-influx2-0.3.3/tests/test_buckets.py
+-rw-rw-rw-   0        0        0     2018 2023-07-03 09:11:49.000000 dms-influx2-0.3.3/tests/test_copy-values.py
+-rw-rw-rw-   0        0        0    16796 2023-07-14 12:09:20.000000 dms-influx2-0.3.3/tests/test_data.py
```

### Comparing `dms-influx2-0.3.2/PKG-INFO` & `dms-influx2-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dms-influx2
-Version: 0.3.2
+Version: 0.3.3
 Summary: Library to connect and retrieve data from DMS influxdb
 Home-page: https://github.com/belingarb/dms-influx2
 Author: Bozidar Belingar
 Author-email: bozidar.belingar@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dms-influx2-0.3.2/dms_influx2/authorizations.py` & `dms-influx2-0.3.3/dms_influx2/authorizations.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.2/dms_influx2/buckets.py` & `dms-influx2-0.3.3/dms_influx2/buckets.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.2/dms_influx2/checks.py` & `dms-influx2-0.3.3/dms_influx2/checks.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.2/dms_influx2/decorators.py` & `dms-influx2-0.3.3/dms_influx2/decorators.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.2/dms_influx2/delete.py` & `dms-influx2-0.3.3/dms_influx2/delete.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.2/dms_influx2/dtv_files.py` & `dms-influx2-0.3.3/dms_influx2/dtv_files.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.2/dms_influx2/lib.py` & `dms-influx2-0.3.3/dms_influx2/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import math
 from typing import List, Union
 
 from ciso8601 import parse_datetime
 from dateutil.parser import parse
 from influxdb_client import InfluxDBClient, Point
 from datetime import datetime, timedelta
 from influxdb_client.client.flux_table import FluxTable
@@ -518,23 +519,27 @@
 
     def down_sample(self,
                     bucket: str,
                     aggregate_window: str,
                     measurement: str = None,
                     time_from: Union[str, datetime] = None,
                     time_to: Union[str, datetime] = None,
-                    older_than: str = None):
+                    older_than: str = None,
+                    decimal_places: int = None):
         if time_from is None and time_to is None and older_than is None:
             raise ValueError("Params (`time_from`, `time_to`, `older_than`) must not all be None")
 
         if type(time_from) == str:
             parse(time_from)
         if type(time_to) == str:
             parse(time_to)
 
+        if decimal_places is None:
+            decimal_places = 3
+
         if older_than is not None:
             window_type = older_than[-1]
             window_number = int(older_than[0:-1])
             dt = localize_dt(datetime.utcnow())
             if window_type == 'y':
                 window_type = 'd'
                 window_number = window_number * 365
@@ -559,25 +564,36 @@
 
         # Erase bucket every each time for this operation
         downsampled_bucket = self.downsample_temp_bucket
         if self.buckets_api().bucket_exists(bucket_name=downsampled_bucket):
             self.buckets_api().delete_bucket_by_name(bucket_name=downsampled_bucket)
         self.buckets_api().create_bucket(bucket_name=downsampled_bucket)
 
+        decimal_places_number = math.pow(10, decimal_places)
+
         if measurement is not None:
             query = f'''
+                import "math"
                 from(bucket: "{bucket}") |> range(start: {start}, stop: {stop})
                     |> filter(fn: (r) => r["_measurement"] == "{measurement}")
                     |> aggregateWindow(every: {aggregate_window}, fn: mean, createEmpty: false)
+                    |> map(
+                        fn: (r) =>
+                        ({{r with _value: (math.round(x: r._value * {decimal_places_number}) / {decimal_places_number}),}}),
+                    )
                     |> to(bucket: "{downsampled_bucket}", org: "{self.org}")
             '''
         else:
             query = f'''
                 from(bucket: "{bucket}") |> range(start: {start}, stop: {stop})
                     |> aggregateWindow(every: {aggregate_window}, fn: mean, createEmpty: false)
+                    |> map(
+                        fn: (r) =>
+                        ({{r with _value: (math.round(x: r._value * {decimal_places_number}) / {decimal_places_number}),}}),
+                    )
                     |> to(bucket: "{downsampled_bucket}", org: "{self.org}")
             '''
         self.query_api().query(query=query)
 
         self.delete_api().delete_data(bucket=bucket, time_from=time_from, time_to=time_to)
 
         query = f'''
```

### Comparing `dms-influx2-0.3.2/dms_influx2/notifications.py` & `dms-influx2-0.3.3/dms_influx2/notifications.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.2/dms_influx2/organisations.py` & `dms-influx2-0.3.3/dms_influx2/organisations.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.2/dms_influx2/query.py` & `dms-influx2-0.3.3/dms_influx2/query.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.2/dms_influx2/tasks.py` & `dms-influx2-0.3.3/dms_influx2/tasks.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.2/dms_influx2/utils.py` & `dms-influx2-0.3.3/dms_influx2/utils.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.2/dms_influx2.egg-info/PKG-INFO` & `dms-influx2-0.3.3/dms_influx2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dms-influx2
-Version: 0.3.2
+Version: 0.3.3
 Summary: Library to connect and retrieve data from DMS influxdb
 Home-page: https://github.com/belingarb/dms-influx2
 Author: Bozidar Belingar
 Author-email: bozidar.belingar@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dms-influx2-0.3.2/dms_influx2.egg-info/SOURCES.txt` & `dms-influx2-0.3.3/dms_influx2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.2/setup.py` & `dms-influx2-0.3.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 NAME = 'dms-influx2'
 DESCRIPTION = 'Library to connect and retrieve data from DMS influxdb'
 URL = 'https://github.com/belingarb/dms-influx2'
 EMAIL = 'bozidar.belingar@gmail.com'
 AUTHOR = 'Bozidar Belingar'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '0.3.2'
+VERSION = '0.3.3'
 
 # Get required packages from requirements.txt file
 with open('requirements/base.txt') as f:
     REQUIRED = f.read().splitlines()
 
 dir_path = os.path.abspath(os.path.dirname(__file__))
```

### Comparing `dms-influx2-0.3.2/tests/test_auth.py` & `dms-influx2-0.3.3/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.2/tests/test_buckets.py` & `dms-influx2-0.3.3/tests/test_buckets.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.2/tests/test_copy-values.py` & `dms-influx2-0.3.3/tests/test_copy-values.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.2/tests/test_data.py` & `dms-influx2-0.3.3/tests/test_data.py`

 * *Files identical despite different names*

