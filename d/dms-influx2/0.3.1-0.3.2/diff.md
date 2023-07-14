# Comparing `tmp/dms-influx2-0.3.1.tar.gz` & `tmp/dms-influx2-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dms-influx2-0.3.1.tar", last modified: Tue Jul  4 18:40:02 2023, max compression
+gzip compressed data, was "dist\dms-influx2-0.3.2.tar", last modified: Fri Jul 14 12:10:59 2023, max compression
```

## Comparing `dms-influx2-0.3.1.tar` & `dms-influx2-0.3.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 18:40:02.374486 dms-influx2-0.3.1/
--rw-rw-rw-   0        0        0      556 2023-07-04 18:40:02.373485 dms-influx2-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-01-09 21:18:36.000000 dms-influx2-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 18:40:02.361412 dms-influx2-0.3.1/dms_influx2/
--rw-rw-rw-   0        0        0        0 2023-01-09 21:18:36.000000 dms-influx2-0.3.1/dms_influx2/__init__.py
--rw-rw-rw-   0        0        0     5108 2023-01-09 21:18:36.000000 dms-influx2-0.3.1/dms_influx2/authorizations.py
--rw-rw-rw-   0        0        0     6376 2023-03-22 11:19:56.000000 dms-influx2-0.3.1/dms_influx2/buckets.py
--rw-rw-rw-   0        0        0     5591 2023-01-19 07:18:35.000000 dms-influx2-0.3.1/dms_influx2/checks.py
--rw-rw-rw-   0        0        0      630 2023-01-09 21:18:36.000000 dms-influx2-0.3.1/dms_influx2/decorators.py
--rw-rw-rw-   0        0        0     2729 2023-07-03 09:35:10.000000 dms-influx2-0.3.1/dms_influx2/delete.py
--rw-rw-rw-   0        0        0     1487 2023-01-19 06:30:10.000000 dms-influx2-0.3.1/dms_influx2/dtv_files.py
--rw-rw-rw-   0        0        0      327 2023-01-09 21:18:36.000000 dms-influx2-0.3.1/dms_influx2/exceptions.py
--rw-rw-rw-   0        0        0    21500 2023-04-11 13:17:17.000000 dms-influx2-0.3.1/dms_influx2/lib.py
--rw-rw-rw-   0        0        0     3562 2023-01-09 21:18:36.000000 dms-influx2-0.3.1/dms_influx2/notifications.py
--rw-rw-rw-   0        0        0     1012 2023-01-09 21:18:36.000000 dms-influx2-0.3.1/dms_influx2/organisations.py
--rw-rw-rw-   0        0        0     7217 2023-07-04 18:39:09.000000 dms-influx2-0.3.1/dms_influx2/query.py
--rw-rw-rw-   0        0        0        0 2023-01-18 17:42:37.000000 dms-influx2-0.3.1/dms_influx2/sync.py
--rw-rw-rw-   0        0        0     4025 2023-01-09 21:18:36.000000 dms-influx2-0.3.1/dms_influx2/tasks.py
--rw-rw-rw-   0        0        0     1203 2023-01-26 19:35:58.000000 dms-influx2-0.3.1/dms_influx2/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-04 18:40:02.371486 dms-influx2-0.3.1/dms_influx2.egg-info/
--rw-rw-rw-   0        0        0      556 2023-07-04 18:40:02.000000 dms-influx2-0.3.1/dms_influx2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      636 2023-07-04 18:40:02.000000 dms-influx2-0.3.1/dms_influx2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 18:40:02.000000 dms-influx2-0.3.1/dms_influx2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-07-04 18:40:02.000000 dms-influx2-0.3.1/dms_influx2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-04 18:40:02.000000 dms-influx2-0.3.1/dms_influx2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 18:40:02.374486 dms-influx2-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     3023 2023-07-04 18:39:37.000000 dms-influx2-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-04 18:40:02.373485 dms-influx2-0.3.1/tests/
--rw-rw-rw-   0        0        0     1882 2023-07-03 09:02:50.000000 dms-influx2-0.3.1/tests/test_auth.py
--rw-rw-rw-   0        0        0     4632 2023-07-03 09:02:50.000000 dms-influx2-0.3.1/tests/test_buckets.py
--rw-rw-rw-   0        0        0     2018 2023-07-03 09:11:49.000000 dms-influx2-0.3.1/tests/test_copy-values.py
--rw-rw-rw-   0        0        0    11926 2023-07-03 09:34:27.000000 dms-influx2-0.3.1/tests/test_data.py
+drwxrwxrwx   0        0        0        0 2023-07-14 12:10:59.370574 dms-influx2-0.3.2/
+-rw-rw-rw-   0        0        0      556 2023-07-14 12:10:59.369575 dms-influx2-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-01-09 21:18:36.000000 dms-influx2-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 12:10:59.347227 dms-influx2-0.3.2/dms_influx2/
+-rw-rw-rw-   0        0        0        0 2023-01-09 21:18:36.000000 dms-influx2-0.3.2/dms_influx2/__init__.py
+-rw-rw-rw-   0        0        0     5108 2023-01-09 21:18:36.000000 dms-influx2-0.3.2/dms_influx2/authorizations.py
+-rw-rw-rw-   0        0        0     6376 2023-03-22 11:19:56.000000 dms-influx2-0.3.2/dms_influx2/buckets.py
+-rw-rw-rw-   0        0        0     5591 2023-01-19 07:18:35.000000 dms-influx2-0.3.2/dms_influx2/checks.py
+-rw-rw-rw-   0        0        0      630 2023-01-09 21:18:36.000000 dms-influx2-0.3.2/dms_influx2/decorators.py
+-rw-rw-rw-   0        0        0     2729 2023-07-03 09:35:10.000000 dms-influx2-0.3.2/dms_influx2/delete.py
+-rw-rw-rw-   0        0        0     1487 2023-01-19 06:30:10.000000 dms-influx2-0.3.2/dms_influx2/dtv_files.py
+-rw-rw-rw-   0        0        0      327 2023-01-09 21:18:36.000000 dms-influx2-0.3.2/dms_influx2/exceptions.py
+-rw-rw-rw-   0        0        0    24601 2023-07-14 12:04:20.000000 dms-influx2-0.3.2/dms_influx2/lib.py
+-rw-rw-rw-   0        0        0     3562 2023-01-09 21:18:36.000000 dms-influx2-0.3.2/dms_influx2/notifications.py
+-rw-rw-rw-   0        0        0     1012 2023-01-09 21:18:36.000000 dms-influx2-0.3.2/dms_influx2/organisations.py
+-rw-rw-rw-   0        0        0     7217 2023-07-04 18:39:09.000000 dms-influx2-0.3.2/dms_influx2/query.py
+-rw-rw-rw-   0        0        0        0 2023-01-18 17:42:37.000000 dms-influx2-0.3.2/dms_influx2/sync.py
+-rw-rw-rw-   0        0        0     4025 2023-01-09 21:18:36.000000 dms-influx2-0.3.2/dms_influx2/tasks.py
+-rw-rw-rw-   0        0        0     1203 2023-01-26 19:35:58.000000 dms-influx2-0.3.2/dms_influx2/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-14 12:10:59.356922 dms-influx2-0.3.2/dms_influx2.egg-info/
+-rw-rw-rw-   0        0        0      556 2023-07-14 12:10:59.000000 dms-influx2-0.3.2/dms_influx2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      636 2023-07-14 12:10:59.000000 dms-influx2-0.3.2/dms_influx2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 12:10:59.000000 dms-influx2-0.3.2/dms_influx2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-07-14 12:10:59.000000 dms-influx2-0.3.2/dms_influx2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-14 12:10:59.000000 dms-influx2-0.3.2/dms_influx2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 12:10:59.370574 dms-influx2-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     3023 2023-07-14 12:10:30.000000 dms-influx2-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 12:10:59.369575 dms-influx2-0.3.2/tests/
+-rw-rw-rw-   0        0        0     1882 2023-07-03 09:02:50.000000 dms-influx2-0.3.2/tests/test_auth.py
+-rw-rw-rw-   0        0        0     4632 2023-07-03 09:02:50.000000 dms-influx2-0.3.2/tests/test_buckets.py
+-rw-rw-rw-   0        0        0     2018 2023-07-03 09:11:49.000000 dms-influx2-0.3.2/tests/test_copy-values.py
+-rw-rw-rw-   0        0        0    16796 2023-07-14 12:09:20.000000 dms-influx2-0.3.2/tests/test_data.py
```

### Comparing `dms-influx2-0.3.1/PKG-INFO` & `dms-influx2-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dms-influx2
-Version: 0.3.1
+Version: 0.3.2
 Summary: Library to connect and retrieve data from DMS influxdb
 Home-page: https://github.com/belingarb/dms-influx2
 Author: Bozidar Belingar
 Author-email: bozidar.belingar@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dms-influx2-0.3.1/dms_influx2/authorizations.py` & `dms-influx2-0.3.2/dms_influx2/authorizations.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.1/dms_influx2/buckets.py` & `dms-influx2-0.3.2/dms_influx2/buckets.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.1/dms_influx2/checks.py` & `dms-influx2-0.3.2/dms_influx2/checks.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.1/dms_influx2/decorators.py` & `dms-influx2-0.3.2/dms_influx2/decorators.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.1/dms_influx2/delete.py` & `dms-influx2-0.3.2/dms_influx2/delete.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.1/dms_influx2/dtv_files.py` & `dms-influx2-0.3.2/dms_influx2/dtv_files.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.1/dms_influx2/lib.py` & `dms-influx2-0.3.2/dms_influx2/lib.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import logging
-from typing import List
+from typing import List, Union
 
 from ciso8601 import parse_datetime
+from dateutil.parser import parse
 from influxdb_client import InfluxDBClient, Point
-from datetime import datetime
+from datetime import datetime, timedelta
 from influxdb_client.client.flux_table import FluxTable
 from influxdb_client.client.write_api import WriteOptions
 
 from dms_influx2.authorizations import Authorizations
 from dms_influx2.buckets import Buckets
 from dms_influx2.checks import ChecksApi
 from dms_influx2.decorators import runtime
 from dms_influx2.delete import Delete
 from dms_influx2.dtv_files import parse_dtv_bytes
 from dms_influx2.notifications import NotificationEndpointApi, NotificationRuleApi
 from dms_influx2.organisations import Organizations
 from dms_influx2.query import get_flux_query
 from dms_influx2.tasks import Tasks
 
-from dms_influx2.utils import localize_dt
+from dms_influx2.utils import localize_dt, timestamp_to_influx_string
 
 logger = logging.getLogger(__name__)
 
 
 class DmsInflux2(InfluxDBClient):
     def __init__(self,
                  url=None,
@@ -35,14 +36,15 @@
         self.query_str = None
         self.predicates = None
 
         self.time_offset = timezone_offset
         self.time_shift = f'{timezone_offset}h' if timezone_offset is not None else None
 
         self.timezone = timezone
+        self.downsample_temp_bucket = 'downsampled_temp_bucket'
 
         super().__init__(url=url, token=token, org=org, enable_gzip=enable_gzip, timeout=timeout)
 
     def buckets_api(self) -> Buckets:
         return Buckets(self)
 
     def organizations_api(self) -> Organizations:
@@ -439,15 +441,15 @@
 
     def copy_bucket_to_bucket(self, bucket_from, bucket_to):
         query = 'from(bucket:"{bucket_from}") |> range(start: -1h)'
 
         records = self.query_api().query_stream(query)
 
         for record in records:
-            print (record)
+            print(record)
             # print(f'Temperature in {record["location"]} is {record["_value"]}')
 
     def _copy_data(self, bucket_from, bucket_to, org_to=None, measurement=None, device_id=None, description=None,
                    time_range=None, time_from=None, time_to=None, aggregate_window=None, aggregate_func=None,
                    sort='desc', limit=None):
         """Copy data from one bucket to another bucket"""
 
@@ -510,8 +512,76 @@
             "measurement": device_id.split('.')[0],
             "device_id": device_id,
             "values": data['values'],
             "unit": data['unit']
         }
         self.save_data(bucket=bucket, data=data_write)
 
+    def down_sample(self,
+                    bucket: str,
+                    aggregate_window: str,
+                    measurement: str = None,
+                    time_from: Union[str, datetime] = None,
+                    time_to: Union[str, datetime] = None,
+                    older_than: str = None):
+        if time_from is None and time_to is None and older_than is None:
+            raise ValueError("Params (`time_from`, `time_to`, `older_than`) must not all be None")
+
+        if type(time_from) == str:
+            parse(time_from)
+        if type(time_to) == str:
+            parse(time_to)
+
+        if older_than is not None:
+            window_type = older_than[-1]
+            window_number = int(older_than[0:-1])
+            dt = localize_dt(datetime.utcnow())
+            if window_type == 'y':
+                window_type = 'd'
+                window_number = window_number * 365
+            d = {
+                "s": "seconds",
+                "m": "minutes",
+                "h": "hours",
+                "d": "days"
+            }
+            time_to = dt - timedelta(**{d[window_type]: window_number})
+            time_from = None
 
+        if time_from is not None:
+            start = timestamp_to_influx_string(time_from)
+        else:
+            start = '-100y'
+
+        if time_to is not None:
+            stop = timestamp_to_influx_string(time_to)
+        else:
+            stop = timestamp_to_influx_string(localize_dt(datetime.utcnow()))
+
+        # Erase bucket every each time for this operation
+        downsampled_bucket = self.downsample_temp_bucket
+        if self.buckets_api().bucket_exists(bucket_name=downsampled_bucket):
+            self.buckets_api().delete_bucket_by_name(bucket_name=downsampled_bucket)
+        self.buckets_api().create_bucket(bucket_name=downsampled_bucket)
+
+        if measurement is not None:
+            query = f'''
+                from(bucket: "{bucket}") |> range(start: {start}, stop: {stop})
+                    |> filter(fn: (r) => r["_measurement"] == "{measurement}")
+                    |> aggregateWindow(every: {aggregate_window}, fn: mean, createEmpty: false)
+                    |> to(bucket: "{downsampled_bucket}", org: "{self.org}")
+            '''
+        else:
+            query = f'''
+                from(bucket: "{bucket}") |> range(start: {start}, stop: {stop})
+                    |> aggregateWindow(every: {aggregate_window}, fn: mean, createEmpty: false)
+                    |> to(bucket: "{downsampled_bucket}", org: "{self.org}")
+            '''
+        self.query_api().query(query=query)
+
+        self.delete_api().delete_data(bucket=bucket, time_from=time_from, time_to=time_to)
+
+        query = f'''
+            from(bucket: "{downsampled_bucket}") |> range(start: -100y)
+                |> to(bucket: "{bucket}", org: "{self.org}")
+        '''
+        self.query_api().query(query=query)
```

### Comparing `dms-influx2-0.3.1/dms_influx2/notifications.py` & `dms-influx2-0.3.2/dms_influx2/notifications.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.1/dms_influx2/organisations.py` & `dms-influx2-0.3.2/dms_influx2/organisations.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.1/dms_influx2/query.py` & `dms-influx2-0.3.2/dms_influx2/query.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.1/dms_influx2/tasks.py` & `dms-influx2-0.3.2/dms_influx2/tasks.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.1/dms_influx2/utils.py` & `dms-influx2-0.3.2/dms_influx2/utils.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.1/dms_influx2.egg-info/PKG-INFO` & `dms-influx2-0.3.2/dms_influx2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dms-influx2
-Version: 0.3.1
+Version: 0.3.2
 Summary: Library to connect and retrieve data from DMS influxdb
 Home-page: https://github.com/belingarb/dms-influx2
 Author: Bozidar Belingar
 Author-email: bozidar.belingar@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dms-influx2-0.3.1/dms_influx2.egg-info/SOURCES.txt` & `dms-influx2-0.3.2/dms_influx2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.1/setup.py` & `dms-influx2-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 NAME = 'dms-influx2'
 DESCRIPTION = 'Library to connect and retrieve data from DMS influxdb'
 URL = 'https://github.com/belingarb/dms-influx2'
 EMAIL = 'bozidar.belingar@gmail.com'
 AUTHOR = 'Bozidar Belingar'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '0.3.1'
+VERSION = '0.3.2'
 
 # Get required packages from requirements.txt file
 with open('requirements/base.txt') as f:
     REQUIRED = f.read().splitlines()
 
 dir_path = os.path.abspath(os.path.dirname(__file__))
```

### Comparing `dms-influx2-0.3.1/tests/test_auth.py` & `dms-influx2-0.3.2/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.1/tests/test_buckets.py` & `dms-influx2-0.3.2/tests/test_buckets.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.1/tests/test_copy-values.py` & `dms-influx2-0.3.2/tests/test_copy-values.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.1/tests/test_data.py` & `dms-influx2-0.3.2/tests/test_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from time import sleep
 
 import pytest
 
 from dms_influx2.lib import DmsInflux2
 from datetime import datetime, timedelta
 from dateutil.parser import parse
 
@@ -71,15 +72,14 @@
 def test_get_values_count(init):
     data = CLIENT.get_values_count(bucket=BUCKET, measurement=MEASUREMENT, device_id=DEVICE_ID)
     assert data[DEVICE_ID] == N_SAMPLES
 
 
 def test_get_metadata(init):
     data = CLIENT.get_metadata(bucket=BUCKET, measurement=MEASUREMENT, device_id=DEVICE_ID)
-    print(data)
     assert data[0]['device_id'] == DEVICE_ID
     assert data[0]['values_count'] == N_SAMPLES
     assert data[0]['timestamp'] == str(TEST_DATA['values'][0][0])
     assert data[0]['value'] == TEST_DATA['values'][0][1]
 
 
 def test_get_first_value(init):
@@ -287,7 +287,86 @@
                                     measurements=[test_data['measurement']])
     data = CLIENT.get_data_from_device_id(bucket=bucket,
                                           measurement=test_data['measurement'],
                                           device_id=test_data['device_id'],
                                           time_range='all')
     assert data == {}
 
+
+def test_downsample_data():
+    bucket = 'downsample_test'
+    values = [(datetime.now() - timedelta(hours=i), i) for i in range(5, 100)]
+    test_data = {
+        "measurement": 'downsample',
+        "device_id": 'downsample.12',
+        "values": values
+
+    }
+    CLIENT.save_data(bucket=bucket, data=test_data)
+    '''Test time_from and time_to'''
+    time_from = test_data['values'][-1][0] - timedelta(seconds=1)
+    time_to = test_data['values'][0][0] + timedelta(seconds=1)
+    aggregate_window = '30m'
+    aggregated_data = CLIENT.get_data_from_device_id(bucket=bucket,
+                                                     measurement=test_data['measurement'],
+                                                     device_id=test_data['device_id'],
+                                                     time_from=time_from,
+                                                     time_to=time_to,
+                                                     aggregate_window=aggregate_window)
+    # Perform a downsample and check if all data are downsampled within bucket
+    CLIENT.down_sample(bucket=bucket,
+                       measurement=test_data['measurement'],
+                       aggregate_window=aggregate_window,
+                       time_from=time_from,
+                       time_to=time_to)
+    data_in_downsampled_bucket = CLIENT.get_data_from_device_id(bucket=CLIENT.downsample_temp_bucket,
+                                                                measurement=test_data['measurement'],
+                                                                device_id=test_data['device_id'],
+                                                                time_range='all')
+    assert aggregated_data['values'] == data_in_downsampled_bucket['values']
+    # New data in this bucket must be equal to aggregated data
+    new_data = CLIENT.get_data_from_device_id(bucket=bucket,
+                                              measurement=test_data['measurement'],
+                                              device_id=test_data['device_id'],
+                                              time_from=time_from - timedelta(seconds=1),
+                                              time_to=time_to + timedelta(seconds=1))
+    assert aggregated_data['values'] == new_data['values']
+
+    '''Test2: test older_than param'''
+    bucket = 'downsample_test1'
+    older_than = '1d'
+    aggregate_window = '4h'
+    CLIENT.save_data(bucket=bucket, data=test_data)
+    time_from = datetime(1970, 1, 1, 12, 0, 0)
+    time_to = datetime.now() - timedelta(days=1) + timedelta(seconds=1)
+    aggregated_data = CLIENT.get_data_from_device_id(bucket=bucket,
+                                                     measurement=test_data['measurement'],
+                                                     device_id=test_data['device_id'],
+                                                     time_from=time_from,
+                                                     time_to=time_to,
+                                                     aggregate_window=aggregate_window)
+    # Perform a downsample and check if all data are downsampled within bucket
+    CLIENT.down_sample(bucket=bucket,
+                       measurement=test_data['measurement'],
+                       aggregate_window=aggregate_window,
+                       older_than=older_than)
+    data_in_downsampled_bucket = CLIENT.get_data_from_device_id(bucket=CLIENT.downsample_temp_bucket,
+                                                                measurement=test_data['measurement'],
+                                                                device_id=test_data['device_id'],
+                                                                time_range='all')
+    assert len(aggregated_data['values']) == len(data_in_downsampled_bucket['values'])
+    # Old data must remain the same
+    old_data = CLIENT.get_data_from_device_id(bucket=bucket,
+                                              measurement=test_data['measurement'],
+                                              device_id=test_data['device_id'],
+                                              time_from=time_to)
+    old_data_values = []
+    for value in values:
+        if value[0] > (time_to - timedelta(seconds=1)):
+            old_data_values.append((str(value[0]), value[1]))
+    assert old_data_values == old_data['values']
+    new_data = CLIENT.get_data_from_device_id(bucket=bucket,
+                                              measurement=test_data['measurement'],
+                                              device_id=test_data['device_id'],
+                                              time_from=time_from,
+                                              time_to=time_to)
+    assert len(aggregated_data['values']) == len(new_data['values'])
```

