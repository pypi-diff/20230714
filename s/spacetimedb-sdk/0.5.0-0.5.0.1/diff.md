# Comparing `tmp/spacetimedb_sdk-0.5.0.tar.gz` & `tmp/spacetimedb_sdk-0.5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacetimedb_sdk-0.5.0.tar", last modified: Wed Jul  5 18:36:49 2023, max compression
+gzip compressed data, was "spacetimedb_sdk-0.5.0.1.tar", last modified: Fri Jul 14 16:06:47 2023, max compression
```

## Comparing `spacetimedb_sdk-0.5.0.tar` & `spacetimedb_sdk-0.5.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:36:49.375952 spacetimedb_sdk-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-05 18:36:49.375952 spacetimedb_sdk-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-05 18:36:36.000000 spacetimedb_sdk-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 18:36:49.375952 spacetimedb_sdk-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:36:49.371952 spacetimedb_sdk-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:36:49.375952 spacetimedb_sdk-0.5.0/src/spacetimedb_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 18:36:36.000000 spacetimedb_sdk-0.5.0/src/spacetimedb_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-05 18:36:36.000000 spacetimedb_sdk-0.5.0/src/spacetimedb_sdk/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-07-05 18:36:36.000000 spacetimedb_sdk-0.5.0/src/spacetimedb_sdk/client_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-07-05 18:36:36.000000 spacetimedb_sdk-0.5.0/src/spacetimedb_sdk/local_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-05 18:36:36.000000 spacetimedb_sdk-0.5.0/src/spacetimedb_sdk/spacetime_websocket_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-07-05 18:36:36.000000 spacetimedb_sdk-0.5.0/src/spacetimedb_sdk/spacetimedb_async_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23599 2023-07-05 18:36:36.000000 spacetimedb_sdk-0.5.0/src/spacetimedb_sdk/spacetimedb_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:36:49.375952 spacetimedb_sdk-0.5.0/src/spacetimedb_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-05 18:36:49.000000 spacetimedb_sdk-0.5.0/src/spacetimedb_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-05 18:36:49.000000 spacetimedb_sdk-0.5.0/src/spacetimedb_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 18:36:49.000000 spacetimedb_sdk-0.5.0/src/spacetimedb_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-05 18:36:49.000000 spacetimedb_sdk-0.5.0/src/spacetimedb_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-05 18:36:49.000000 spacetimedb_sdk-0.5.0/src/spacetimedb_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:47.532444 spacetimedb_sdk-0.5.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-14 16:06:47.532444 spacetimedb_sdk-0.5.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-14 16:06:37.000000 spacetimedb_sdk-0.5.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 16:06:47.532444 spacetimedb_sdk-0.5.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:47.528444 spacetimedb_sdk-0.5.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:47.532444 spacetimedb_sdk-0.5.0.1/src/spacetimedb_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:37.000000 spacetimedb_sdk-0.5.0.1/src/spacetimedb_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-14 16:06:37.000000 spacetimedb_sdk-0.5.0.1/src/spacetimedb_sdk/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-07-14 16:06:37.000000 spacetimedb_sdk-0.5.0.1/src/spacetimedb_sdk/client_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-07-14 16:06:37.000000 spacetimedb_sdk-0.5.0.1/src/spacetimedb_sdk/local_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-14 16:06:37.000000 spacetimedb_sdk-0.5.0.1/src/spacetimedb_sdk/spacetime_websocket_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-07-14 16:06:37.000000 spacetimedb_sdk-0.5.0.1/src/spacetimedb_sdk/spacetimedb_async_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23365 2023-07-14 16:06:37.000000 spacetimedb_sdk-0.5.0.1/src/spacetimedb_sdk/spacetimedb_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:06:47.532444 spacetimedb_sdk-0.5.0.1/src/spacetimedb_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-14 16:06:47.000000 spacetimedb_sdk-0.5.0.1/src/spacetimedb_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-14 16:06:47.000000 spacetimedb_sdk-0.5.0.1/src/spacetimedb_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:06:47.000000 spacetimedb_sdk-0.5.0.1/src/spacetimedb_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-14 16:06:47.000000 spacetimedb_sdk-0.5.0.1/src/spacetimedb_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-14 16:06:47.000000 spacetimedb_sdk-0.5.0.1/src/spacetimedb_sdk.egg-info/top_level.txt
```

### Comparing `spacetimedb_sdk-0.5.0/src/spacetimedb_sdk/client_cache.py` & `spacetimedb_sdk-0.5.0.1/src/spacetimedb_sdk/client_cache.py`

 * *Files identical despite different names*

### Comparing `spacetimedb_sdk-0.5.0/src/spacetimedb_sdk/local_config.py` & `spacetimedb_sdk-0.5.0.1/src/spacetimedb_sdk/local_config.py`

 * *Files identical despite different names*

### Comparing `spacetimedb_sdk-0.5.0/src/spacetimedb_sdk/spacetime_websocket_client.py` & `spacetimedb_sdk-0.5.0.1/src/spacetimedb_sdk/spacetime_websocket_client.py`

 * *Files identical despite different names*

### Comparing `spacetimedb_sdk-0.5.0/src/spacetimedb_sdk/spacetimedb_async_client.py` & `spacetimedb_sdk-0.5.0.1/src/spacetimedb_sdk/spacetimedb_async_client.py`

 * *Files identical despite different names*

### Comparing `spacetimedb_sdk-0.5.0/src/spacetimedb_sdk/spacetimedb_client.py` & `spacetimedb_sdk-0.5.0.1/src/spacetimedb_sdk/spacetimedb_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -357,15 +357,15 @@
         }
 
         json_data = json.dumps(message)
         # print("_reducer_call(JSON): " + json_data)
         self.wsc.send(bytes(f'{{"call": {json_data}}}', "ascii"))
 
     def _on_message(self, data):
-        print("_on_message data: " + data)
+        # print("_on_message data: " + data)
         message = json.loads(data)
         if "IdentityToken" in message:
             # is this safe to do in the message thread?
             token = message["IdentityToken"]["token"]
             identity = bytes.fromhex(message["IdentityToken"]["identity"])
             self.message_queue.put(_IdentityReceivedMessage(token, identity))
         elif "SubscriptionUpdate" in message or "TransactionUpdate" in message:
@@ -419,22 +419,17 @@
             next_message = self.message_queue.get()
 
             if next_message.transaction_type == "IdentityReceived":
                 self.identity = next_message.identity
                 if self._on_identity:
                     self._on_identity(next_message.auth_token, self.identity)
             else:
-                print(f"next_message: {next_message.transaction_type}")
+                # print(f"next_message: {next_message.transaction_type}")
                 # apply all the event state before calling callbacks
                 for table_name, table_events in next_message.events.items():
-                    for row_pk, element in self.client_cache.get_table_cache(
-                        table_name
-                    ).entries.items():
-                        print("Cache entry: " + str(row_pk) + " " + str(element))
-
                     # first retrieve the old values for all events
                     for db_event in table_events:
                         # get the old value for sending callbacks
                         db_event.old_value = self.client_cache.get_entry(
                             db_event.table_name, db_event.row_pk
                         )
 
@@ -486,15 +481,15 @@
                                 primary_key_row_ops[primary_key_value] = db_event
 
                         table_events = primary_key_row_ops.values()
                         next_message.events[table_name] = table_events
 
                     # now we can apply the events to the cache
                     for db_event in table_events:
-                        print(f"db_event: {db_event.row_op} {table_name}")
+                        # print(f"db_event: {db_event.row_op} {table_name}")
                         if db_event.row_op == "insert" or db_event.row_op == "update":
                             # in the case of updates we need to delete the old entry
                             if db_event.row_op == "update":
                                 self.client_cache.delete_entry(
                                     db_event.table_name, db_event.old_pk
                                 )
                             self.client_cache.set_entry_decoded(
```

