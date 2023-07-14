# Comparing `tmp/macrometa-source-collection-0.0.55.tar.gz` & `tmp/macrometa-source-collection-0.0.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-collection-0.0.55.tar", max compression
+gzip compressed data, was "macrometa-source-collection-0.0.56.tar", max compression
```

## Comparing `macrometa-source-collection-0.0.55.tar` & `macrometa-source-collection-0.0.56.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11137 2023-07-06 13:42:22.627178 macrometa-source-collection-0.0.55/macrometa_source_collection/__init__.py
--rw-r--r--   0        0        0    10291 2023-07-06 13:42:22.627178 macrometa-source-collection-0.0.55/macrometa_source_collection/client.py
--rw-r--r--   0        0        0     1626 2023-07-06 13:42:22.987179 macrometa-source-collection-0.0.55/pyproject.toml
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.55/setup.py
--rw-r--r--   0        0        0     1160 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.55/PKG-INFO
+-rw-r--r--   0        0        0    11137 2023-07-14 08:38:33.443026 macrometa-source-collection-0.0.56/macrometa_source_collection/__init__.py
+-rw-r--r--   0        0        0    10411 2023-07-14 08:38:33.443026 macrometa-source-collection-0.0.56/macrometa_source_collection/client.py
+-rw-r--r--   0        0        0     1626 2023-07-14 08:38:33.711036 macrometa-source-collection-0.0.56/pyproject.toml
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.56/setup.py
+-rw-r--r--   0        0        0     1160 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.56/PKG-INFO
```

### Comparing `macrometa-source-collection-0.0.55/macrometa_source_collection/__init__.py` & `macrometa-source-collection-0.0.56/macrometa_source_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-collection-0.0.55/macrometa_source_collection/client.py` & `macrometa-source-collection-0.0.56/macrometa_source_collection/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 import os
 import time
 import uuid
 
 import pulsar
 import singer
 from c8 import C8Client
-from datetime import datetime, timezone
-from prometheus_client import start_http_server, Counter, Histogram
+from prometheus_client import start_http_server, Counter
 from singer import utils
 from singer.catalog import CatalogEntry
 
 LOGGER = singer.get_logger('macrometa_source_collection')
 
 region_label = os.getenv("GDN_FEDERATION", "NA")
 tenant_label = os.getenv("GDN_TENANT", "NA")
@@ -51,20 +50,20 @@
             self._c8_client.update_collection_properties(self._collection, has_stream=True)
         except:
             pass
 
         self.exported_bytes = Counter("exported_bytes", "Total number of bytes exported from GDN collections", ['region', 'tenant', 'fabric', 'workflow'])
         self.exported_documents = Counter("exported_documents", "Total number of documents exported from GDN collections", ['region', 'tenant', 'fabric', 'workflow'])
         self.export_errors = Counter("export_errors", "Total count of errors while exporting data from GDN collections", ['region', 'tenant', 'fabric', 'workflow'])
-        self.export_lag = Histogram("export_lag", "The average time from when the data changes in GDN collections are reflected in external data sources", ['region', 'tenant', 'fabric', 'workflow'])
-        
+        if is_metrics_enabled.lower() == 'false':
+            self.ingest_errors = Counter('ingest_errors', 'Total number of errors during ingestion',
+                        ['region', 'tenant', 'fabric', 'workflow'])
         # Start the Prometheus HTTP server for exposing metrics
-        if is_metrics_enabled.lower() == 'true':
-            LOGGER.info("Source is starting the metrics server.")
-            start_http_server(8000)
+        LOGGER.info("Macrometa collection source is starting the metrics server.")
+        start_http_server(8000)
 
     def sync(self, stream):
         """Return documents in target GDN collection as records."""
         if self._c8_client.has_collection(self._collection):
             self.send_schema_message(stream)
             columns = list(stream.schema.properties.keys())
             columns.remove("_sdc_deleted_at")
@@ -91,79 +90,84 @@
             self.load_existing_data(stream, columns, schema_properties)
             LOGGER.info("Full table sync completed.")
 
             # Change data capture
             while True:
                 try: 
                     msg = _consumer.receive()
+                    time_extracted = utils.now()
                     data = msg.data()
                     if data == None or not data:
                         continue
                     props = msg.properties()
                     j = json.loads(data.decode("utf8"))
                     j.pop('_id', None)
                     j.pop('_rev', None)
-
+                    record_sent =  False
                     if props["op"] == "INSERT" or props["op"] == "UPDATE":
                         # skip inserts not having valid schema
                         if len(j.keys() ^ columns) == 0 and all(
                             j[key] is None or (isinstance(schema_properties[key].type, list) and get_singer_data_type(j[key]) in schema_properties[key].type)
                                                  or (isinstance(schema_properties[key].type, str) and get_singer_data_type(j[key]) == schema_properties[key].type)
                             for key in j.keys()
                         ):
                             j['_sdc_deleted_at'] = None
-                            singer_record = self.msg_to_singer_message(stream, j, None, utils.now())
+                            singer_record = self.msg_to_singer_message(stream, j, None, time_extracted)
                             singer.write_message(singer_record)
+                            record_sent = True
                         else:
                             LOGGER.warn("The record: %s, does not match the most common schema. Skipping it..", j)
                     elif props["op"] == "DELETE":
                         # Currently, we don't have a way to validate schema here
                         j.pop('_delete', None)
                         j['_sdc_deleted_at'] = singer.utils.strftime(utils.now())
-                        singer_record = self.msg_to_singer_message(stream, j, None, utils.now())
+                        singer_record = self.msg_to_singer_message(stream, j, None, time_extracted)
                         singer.write_message(singer_record)
+                        record_sent = True
                     _consumer.acknowledge(msg.message_id())
-                    self.exported_bytes.labels(region_label, tenant_label, fabric_label, workflow_label).inc(len(data))
-                    self.exported_documents.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
-                    time = datetime.fromtimestamp(msg.publish_timestamp()/1000)
-                    time_str = time.strftime("%Y-%m-%dT%H:%M:%S.%fZ")
-                    event_time = datetime.strptime(time_str, "%Y-%m-%dT%H:%M:%S.%fZ").replace(tzinfo=timezone.utc)
-                    self.export_lag.labels(region_label, tenant_label, fabric_label, workflow_label).observe((utils.now() - event_time).total_seconds())
+                    if is_metrics_enabled.lower() == 'true' and record_sent:
+                        self.exported_bytes.labels(region_label, tenant_label, fabric_label, workflow_label).inc(len(json.dumps(j)))
+                        self.exported_documents.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
                 except Exception as e:
                     LOGGER.warn(f"Exception received: {e}")
-                    self.export_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
+                    if is_metrics_enabled.lower() == 'false':
+                        self.ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
+                    else:
+                        self.export_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
                     raise e
         
         else:
             raise FileNotFoundError("Collection {} not found".format(self._collection))
 
 
     def load_existing_data(self, stream, columns, schema_properties):
         cursor = self._c8_client._fabric.c8ql.execute(f"FOR d IN @@collection RETURN d",
                                                       bind_vars={"@collection": self._collection}, stream=True,
                                                       batch_size=self._cursor_batch_size, ttl=self._cursor_ttl)
         try:
             while (not cursor.empty()) or cursor.has_more():
                 rec = cursor.next()
+                time_extracted = utils.now()
                 rec.pop('_id', None)
                 rec.pop('_rev', None)
                 # skip existing data not having valid schema
                 if len(rec.keys() ^ columns) == 0 and all(
                     rec[key] is None or (isinstance(schema_properties[key].type, list) and get_singer_data_type(rec[key]) in schema_properties[key].type)
                                          or (isinstance(schema_properties[key].type, str) and get_singer_data_type(rec[key]) == schema_properties[key].type)
                     for key in rec.keys()
                 ):
-                    singer_record = self.msg_to_singer_message(stream, rec, None, utils.now())
+                    singer_record = self.msg_to_singer_message(stream, rec, None, time_extracted)
                     start_time = time.time()
                     singer.write_message(singer_record)
                     end_time = time.time()
                     if end_time - start_time > 10:
                         LOGGER.warn(f"Took {end_time - start_time}seconds to write record:{singer_record}")
-                    self.exported_bytes.labels(region_label, tenant_label, fabric_label, workflow_label).inc(len(rec))
-                    self.exported_documents.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
+                    if is_metrics_enabled.lower() == 'true':
+                        self.exported_bytes.labels(region_label, tenant_label, fabric_label, workflow_label).inc(len(json.dumps(rec)))
+                        self.exported_documents.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
                 else:
                     LOGGER.warn("The record: %s, does not match the most common schema. Skipping it..", rec)
         except Exception as e:
             time.sleep(100)
             raise e
 
     def send_schema_message(self, stream: CatalogEntry, bookmark_properties=[]):
```

### Comparing `macrometa-source-collection-0.0.55/pyproject.toml` & `macrometa-source-collection-0.0.56/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-collection"
-version='0.0.55'
+version='0.0.56'
 description = "Pipelinewise tap for reading from GDN Collections"
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-collection-0.0.55/setup.py` & `macrometa-source-collection-0.0.56/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 entry_points = \
 {'console_scripts': ['macrometa-source-collection = '
                      'macrometa_source_collection:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-collection',
-    'version': '0.0.55',
+    'version': '0.0.56',
     'description': 'Pipelinewise tap for reading from GDN Collections',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-collection-0.0.55/PKG-INFO` & `macrometa-source-collection-0.0.56/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-collection
-Version: 0.0.55
+Version: 0.0.56
 Summary: Pipelinewise tap for reading from GDN Collections
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,GDN,Collection,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

