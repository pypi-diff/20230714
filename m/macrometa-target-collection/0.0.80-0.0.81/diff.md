# Comparing `tmp/macrometa-target-collection-0.0.80.tar.gz` & `tmp/macrometa-target-collection-0.0.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-collection-0.0.80.tar", last modified: Sat Jun 17 11:01:02 2023, max compression
+gzip compressed data, was "macrometa-target-collection-0.0.81.tar", last modified: Fri Jul 14 08:39:22 2023, max compression
```

## Comparing `macrometa-target-collection-0.0.80.tar` & `macrometa-target-collection-0.0.81.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:01:02.512419 macrometa-target-collection-0.0.80/
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-06-17 11:00:43.000000 macrometa-target-collection-0.0.80/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-17 11:01:02.512419 macrometa-target-collection-0.0.80/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-17 11:00:43.000000 macrometa-target-collection-0.0.80/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:01:02.512419 macrometa-target-collection-0.0.80/macrometa_target_collection/
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-06-17 11:00:43.000000 macrometa-target-collection-0.0.80/macrometa_target_collection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16278 2023-06-17 11:00:43.000000 macrometa-target-collection-0.0.80/macrometa_target_collection/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:01:02.512419 macrometa-target-collection-0.0.80/macrometa_target_collection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-17 11:01:02.000000 macrometa-target-collection-0.0.80/macrometa_target_collection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-17 11:01:02.000000 macrometa-target-collection-0.0.80/macrometa_target_collection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 11:01:02.000000 macrometa-target-collection-0.0.80/macrometa_target_collection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-17 11:01:02.000000 macrometa-target-collection-0.0.80/macrometa_target_collection.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-17 11:01:02.000000 macrometa-target-collection-0.0.80/macrometa_target_collection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-17 11:01:02.000000 macrometa-target-collection-0.0.80/macrometa_target_collection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-17 11:00:43.000000 macrometa-target-collection-0.0.80/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-17 11:01:02.512419 macrometa-target-collection-0.0.80/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:39:22.439684 macrometa-target-collection-0.0.81/
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-07-14 08:38:55.000000 macrometa-target-collection-0.0.81/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-07-14 08:39:22.443684 macrometa-target-collection-0.0.81/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-14 08:38:55.000000 macrometa-target-collection-0.0.81/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:39:22.439684 macrometa-target-collection-0.0.81/macrometa_target_collection/
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-07-14 08:38:55.000000 macrometa-target-collection-0.0.81/macrometa_target_collection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16271 2023-07-14 08:38:55.000000 macrometa-target-collection-0.0.81/macrometa_target_collection/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:39:22.439684 macrometa-target-collection-0.0.81/macrometa_target_collection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-07-14 08:39:22.000000 macrometa-target-collection-0.0.81/macrometa_target_collection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-14 08:39:22.000000 macrometa-target-collection-0.0.81/macrometa_target_collection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 08:39:22.000000 macrometa-target-collection-0.0.81/macrometa_target_collection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-14 08:39:22.000000 macrometa-target-collection-0.0.81/macrometa_target_collection.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-14 08:39:22.000000 macrometa-target-collection-0.0.81/macrometa_target_collection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-14 08:39:22.000000 macrometa-target-collection-0.0.81/macrometa_target_collection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-14 08:38:55.000000 macrometa-target-collection-0.0.81/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-14 08:39:22.443684 macrometa-target-collection-0.0.81/setup.cfg
```

### Comparing `macrometa-target-collection-0.0.80/LICENSE` & `macrometa-target-collection-0.0.81/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.80/PKG-INFO` & `macrometa-target-collection-0.0.81/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.80
+Version: 0.0.81
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.80/macrometa_target_collection/__init__.py` & `macrometa-target-collection-0.0.81/macrometa_target_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.80/macrometa_target_collection/main.py` & `macrometa-target-collection-0.0.81/macrometa_target_collection/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 import time
 from datetime import datetime, timezone
 from threading import Lock
 
 import jsonschema
 import requests
 from adjust_precision_for_schema import adjust_decimal_precision_for_schema
-from c8 import C8Client, DocumentInsertError
+from c8 import C8Client, DocumentInsertError, DocumentUpdateError, DocumentRevisionError
 from c8.collection import StandardCollection
+from c8connector import ensure_datetime
 from jsonschema import Draft4Validator
 from prometheus_client import Counter, Gauge, start_http_server
 from singer import get_logger
 from typing import AsyncIterable
 
 from macrometa_target_collection import extract_gdn_host
 
@@ -33,36 +34,40 @@
 ingested_bytes = Counter('ingested_bytes', 'Total number of bytes ingested', ['region', 'tenant', 'fabric', 'workflow'])
 ingested_documents = Counter('ingested_documents', 'Total number of documents ingested',
                              ['region', 'tenant', 'fabric', 'workflow'])
 ingest_errors = Counter('ingest_errors', 'Total number of errors during ingestion',
                         ['region', 'tenant', 'fabric', 'workflow'])
 ingest_lag = Gauge('ingest_lag', 'Average time lag between data changes in GDN collections and external data sources',
                    ['region', 'tenant', 'fabric', 'workflow'])
+export_lag = Gauge("export_lag", "The average time from when the data changes in GDN collections are reflected in external data sources",
+                   ['region', 'tenant', 'fabric', 'workflow'])
+export_errors = Counter("export_errors", "Total count of errors while exporting data from GDN collections",
+                        ['region', 'tenant', 'fabric', 'workflow'])
 scrape_complete_flag = Counter("scrape_complete_flag", "Flag to check if the last scrape has been completed",
                                ['workflow'])
 
 region_label = os.getenv("GDN_FEDERATION", "NA")
 tenant_label = os.getenv("GDN_TENANT", "NA")
 fabric_label = os.getenv("GDN_FABRIC", "NA")
 workflow_label = os.getenv("WORKFLOW_UUID", "NA")
 metric_service_url = os.getenv("METRIC_SERVICE_API")
 is_metrics_enabled = os.getenv("MACROMETA_TARGET_COLLECTION_IS_METRICS_ENABLED", 'False')
 
 # Start the Prometheus HTTP server for exposing metrics
-if is_metrics_enabled.lower() == 'true':
-    logger.info("Target is starting the metrics server.")
-    start_http_server(8000)
+logger.info("Macrometa target is starting the metrics server.")
+start_http_server(8001)
 
 
 class RecordBatch:
     """Class wrapping the record batch in order to make it thread safe."""
 
     def __init__(self, config: dict):
         self._list = list()
         self._delete_list = set()
+        self.time_extracted_list = []
         self._lock = Lock()
         self.interval = config.get('batch_flush_interval', DEFAULT_BATCH_FLUSH_INTERVAL)
         self.last_executed_time = datetime.now(timezone.utc)
         self.min_time_gap = config.get('batch_flush_min_time_gap', DEFAULT_MIN_BATCH_FLUSH_TIME_GAP)
         self.max_batch_size = config.get('batch_size_rows', DEFAULT_BATCH_SIZE_ROWS)
         self.is_completed = False
 
@@ -70,20 +75,30 @@
         """Acquire the lock and add a record to the list."""
         with self._lock:
             if not delete:
                 self._list.append(value)
             else:
                 self._delete_list.add(value)
 
+    def append_time_extracted(self, value) -> None:
+        """Acquire the lock and add a record to time extracted list."""
+        with self._lock:
+            self.time_extracted_list.append(value)
+
     def remove_from_delete_list(self, value) -> None:
         """Acquire the lock and delete a record from the delete list."""
         with self._lock:
             if value in self._delete_list:
                 self._delete_list.remove(value)
 
+    def clear_time_extracted(self) -> None:
+        """Acquire the lock and clear time extracted list."""
+        with self._lock:
+            self.time_extracted_list.clear()
+
     def length(self) -> int:
         """Acquire the lock and return the number of items in the list."""
         with self._lock:
             return len(self._list) + len(self._delete_list)
 
     def flush(self) -> tuple:
         """Acquire the lock, create a copy of the existing batch,
@@ -116,55 +131,72 @@
 
 def try_upsert(collection: StandardCollection, record_batch: RecordBatch, force=False):
     if record_batch.length() > 0 and (record_batch.length() >= record_batch.max_batch_size or force):
         to_insert, to_delete = record_batch.flush()
         to_update = []
 
         if len(to_insert) > 0:
-            records_array = remove_time_extracted(to_insert)
-            for i, r in enumerate(collection.insert_many(records_array)):
+            for i, r in enumerate(collection.insert_many(to_insert)):
                 if type(r) is DocumentInsertError:
                     to_update.append(to_insert[i])
                 else:
-                    # Update ingested_documents and ingested_bytes metrics
-                    ingested_documents.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
-                    ingested_bytes.labels(region_label, tenant_label, fabric_label, workflow_label).inc(len(json.dumps(r)))
-                    # Update ingest_lag metric
-                    diff = datetime.now(timezone.utc) - ensure_datetime(to_insert[i]["time_extracted"])
-                    ingest_lag.labels(region_label, tenant_label, fabric_label, workflow_label).set(diff.total_seconds())
-
-        if len(to_update) > 0:
-            records_array = remove_time_extracted(to_update)
-            for i, r in enumerate(collection.update_many(records_array)):
-                if type(r) is DocumentInsertError:
-                    # Increment ingest_errors metric
-                    ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
+                    update_metrics(r)
+
+        if to_update:
+            for i, r in enumerate(collection.update_many(to_update)):
+                if type(r) in (DocumentInsertError, DocumentUpdateError, DocumentRevisionError):
                     logger.warn(f'Failed to insert/update record: {to_update[i]}. {r}')
+                    update_error_metrics()
                 else:
-                    # Update ingest_lag metric
-                    diff = datetime.now(timezone.utc) - ensure_datetime(to_update[i]["time_extracted"])
-                    ingest_lag.labels(region_label, tenant_label, fabric_label, workflow_label).set(
-                        diff.total_seconds())
+                    update_metrics(r)
 
         if len(to_delete) > 0:
             try_delete(collection, to_delete)
+            for key in to_delete:
+                update_metrics(key)
+
+        event_time = datetime.now(timezone.utc)
+        for time_extracted in record_batch.time_extracted_list:
+            diff = event_time - time_extracted
+            update_lag_metrics(diff)
+        record_batch.clear_time_extracted()
     record_batch.update_last_executed_time(datetime.now(timezone.utc))
 
 
-def remove_time_extracted(records):
-    return [{k: v for k, v in record.items() if k != 'time_extracted'} for record in records]
+def update_metrics(r):
+    if is_metrics_enabled.lower() == 'true':
+        # Update ingested_documents and ingested_bytes metrics
+        ingested_documents.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
+        ingested_bytes.labels(region_label, tenant_label, fabric_label, workflow_label).inc(len(json.dumps(r)))
+
+
+def update_lag_metrics(diff):
+    if is_metrics_enabled.lower() == 'true':
+        # Update ingest_lag metric
+        ingest_lag.labels(region_label, tenant_label, fabric_label, workflow_label).set(diff.total_seconds())
+    else:
+        # Update export_lag metric
+        export_lag.labels(region_label, tenant_label, fabric_label, workflow_label).set(diff.total_seconds())
+
+
+def update_error_metrics():
+    if is_metrics_enabled.lower() == 'true':
+        # Increment ingest_errors metric
+        ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
+    else:
+        # Increment export_errors metric
+        export_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
 
 
 def try_delete(collection: StandardCollection, delete_list):
     try:
         collection.delete_many(delete_list)
     except Exception as e:
-        # Increment ingest_errors metric
-        ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
         logger.warn(f'Failed to delete records with keys: {delete_list}. {e}')
+        update_error_metrics()
 
 
 async def read_stdin() -> AsyncIterable[str]:
     loop = asyncio.get_event_loop()
     reader = asyncio.StreamReader()
     reader_protocol = asyncio.StreamReaderProtocol(reader)
     await loop.connect_read_pipe(lambda: reader_protocol, sys.stdin)
@@ -182,41 +214,38 @@
     validators = {}
 
     messages = read_stdin()
     async for message in messages:
         try:
             o = json.loads(message)
         except json.decoder.JSONDecodeError as e:
-            # Increment ingest_errors metric
-            ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
             logger.error(f"Unable to parse:\n{message}")
+            update_error_metrics()
             raise e
 
         message_type = o['type']
         if message_type == 'RECORD':
             stream = o['stream']
             if stream not in schemas:
-                # Increment ingest_errors metric
-                ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
+                update_error_metrics()
                 raise Exception(f"A record for stream {stream} was encountered before a corresponding schema")
 
             try:
                 validators[stream].validate((o['record']))
             except jsonschema.ValidationError as e:
-                # Increment ingest_errors metric
-                ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
                 logger.error(f"Failed parsing the json schema for stream: {stream}.")
+                update_error_metrics()
                 continue
 
             try:
                 rec = o['record']
                 if 'time_extracted' in o:
-                    rec["time_extracted"] = ensure_datetime(o["time_extracted"])
+                    record_batch.append_time_extracted(ensure_datetime(o["time_extracted"]))
                 else:
-                    rec["time_extracted"] = ensure_datetime(record_batch.last_executed_time)
+                    record_batch.append_time_extracted(datetime.now(timezone.utc))
                 try:
                     kps = key_properties.get(stream)
                     _key = None
                     # Appending _ to keys inorder for preserving values of reserved keys in source data
                     reserved_keys = ['_key', '_id', '_rev']
 
                     if kps:
@@ -254,16 +283,15 @@
                     else:
                         rec.pop('_sdc_deleted_at', None)
                         if rec.get('_key'):
                             record_batch.remove_from_delete_list(rec['_key'])
 
                 record_batch.append(rec)
             except TypeError as e:
-                # Increment ingest_errors metric
-                ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
+                update_error_metrics()
                 # TODO: This is temporary until json serializing issue for Decimals are fixed in pyC8
                 logger.debug("pyC8 error occurred")
 
             state = None
             try_upsert(collection, record_batch)
         elif message_type == 'STATE':
             logger.debug('Setting state to {}'.format(o['value']))
@@ -271,34 +299,24 @@
             emit_state(state)
         elif message_type == 'SCHEMA':
             stream = o['stream']
             schemas[stream] = o['schema']
             adjust_decimal_precision_for_schema(schemas[stream])
             validators[stream] = Draft4Validator((o['schema']))
             key_properties[stream] = o['key_properties']
+        elif message_type == 'ACTIVATE_VERSION':
+            logger.debug('ACTIVATE_VERSION message')
         else:
-            # Increment ingest_errors metric
-            ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
+            update_error_metrics()
             logger.warning("Unknown message type {} in message {}".format(o['type'], o))
 
     scrape_complete_flag.labels(workflow_label).inc()
     record_batch.set_is_completed(True)
 
 
-def ensure_datetime(time_extracted):
-    if isinstance(time_extracted, str):
-        time_extracted = datetime.strptime(time_extracted, "%Y-%m-%dT%H:%M:%S.%fZ")
-        # Make the datetime object timezone-aware by setting it to UTC timezone
-        time_extracted = time_extracted.replace(tzinfo=timezone.utc)
-    elif time_extracted.tzinfo is None:
-        # If the datetime object is timezone-naive, set it to UTC timezone
-        time_extracted = time_extracted.replace(tzinfo=timezone.utc)
-    return time_extracted
-
-
 async def setup_batch_task(collection: StandardCollection,
                            record_batch: RecordBatch, state) -> None:
     event_loop = asyncio.get_event_loop()
     persist_messages_coro = persist_messages(collection, record_batch, state)
     asyncio.run_coroutine_threadsafe(persist_messages_coro, event_loop)
     process_batch_coro = process_batch(collection, record_batch)
     asyncio.run_coroutine_threadsafe(process_batch_coro, event_loop)
@@ -310,15 +328,15 @@
     )
 
 
 async def process_batch(collection: StandardCollection, record_batch: RecordBatch) -> None:
     # As soon as persist_messages is completed process_batch should also exit
     while not record_batch.is_completed:
         await asyncio.sleep(record_batch.interval)
-        timedelta = datetime.now(timezone.utc) - ensure_datetime(record_batch.last_executed_time)
+        timedelta = datetime.now(timezone.utc) - record_batch.last_executed_time
         if timedelta.total_seconds() >= record_batch.min_time_gap:
             # if batch has records that need to be processed but haven't reached batch size then process them.
             try_upsert(collection, record_batch, force=True)
 
 
 async def main_impl():
     parser = argparse.ArgumentParser()
```

### Comparing `macrometa-target-collection-0.0.80/macrometa_target_collection.egg-info/PKG-INFO` & `macrometa-target-collection-0.0.81/macrometa_target_collection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.80
+Version: 0.0.81
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.80/pyproject.toml` & `macrometa-target-collection-0.0.81/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "macrometa-target-collection"
-version = "0.0.80"
+version = "0.0.81"
 authors = [
     { name = "Macrometa", email = "info@macrometa.co" },
 ]
 description = "Singer.io target for writing to Macrometa GDN collections"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 dependencies = [
     'pipelinewise-singer-python==1.2.0',
     'adjust-precision-for-schema==0.3.4',
     'pyc8==0.17.1',
-    'c8connector>=0.0.20',
+    'c8connector>=0.0.29',
     'prometheus-client==0.16.0'
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Operating System :: OS Independent",
 ]
```

