# Comparing `tmp/apibara-0.7.0.tar.gz` & `tmp/apibara-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apibara-0.7.0.tar", max compression
+gzip compressed data, was "apibara-0.7.1.tar", max compression
```

## Comparing `apibara-0.7.0.tar` & `apibara-0.7.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    11358 2023-01-15 18:52:09.124336 apibara-0.7.0/LICENSE.txt
--rw-r--r--   0        0        0     1342 2023-01-18 12:16:07.977321 apibara-0.7.0/README.rst
--rw-r--r--   0        0        0     1073 2023-07-08 12:11:24.025439 apibara-0.7.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-15 18:52:09.124336 apibara-0.7.0/src/apibara/__init__.py
--rw-r--r--   0        0        0      514 2023-01-15 18:52:09.124336 apibara-0.7.0/src/apibara/cursor.py
--rw-r--r--   0        0        0      160 2023-01-15 18:52:09.124336 apibara-0.7.0/src/apibara/indexer/__init__.py
--rw-r--r--   0        0        0      375 2023-01-15 18:52:09.124336 apibara-0.7.0/src/apibara/indexer/configuration.py
--rw-r--r--   0        0        0     2393 2023-03-16 21:14:54.127582 apibara-0.7.0/src/apibara/indexer/indexer.py
--rw-r--r--   0        0        0     1026 2023-01-16 18:48:50.663792 apibara-0.7.0/src/apibara/indexer/info.py
--rw-r--r--   0        0        0    10488 2023-07-08 12:11:24.025439 apibara-0.7.0/src/apibara/indexer/runner.py
--rw-r--r--   0        0        0    10502 2023-06-08 12:55:13.026953 apibara-0.7.0/src/apibara/indexer/storage.py
--rw-r--r--   0        0        0      697 2023-07-08 12:11:24.025439 apibara-0.7.0/src/apibara/protocol/__init__.py
--rw-r--r--   0        0        0     3596 2023-07-08 12:11:24.025439 apibara-0.7.0/src/apibara/protocol/client.py
--rw-r--r--   0        0        0        0 2023-01-15 18:52:09.125336 apibara-0.7.0/src/apibara/protocol/proto/__init__.py
--rw-r--r--   0        0        0     3107 2023-01-15 18:52:09.125336 apibara-0.7.0/src/apibara/protocol/proto/stream_pb2.py
--rw-r--r--   0        0        0     9814 2023-01-15 18:52:09.125336 apibara-0.7.0/src/apibara/protocol/proto/stream_pb2.pyi
--rw-r--r--   0        0        0     2517 2023-01-15 18:52:09.125336 apibara-0.7.0/src/apibara/protocol/proto/stream_pb2_grpc.py
--rw-r--r--   0        0        0      878 2023-01-15 18:52:09.125336 apibara-0.7.0/src/apibara/protocol/proto/stream_pb2_grpc.pyi
--rw-r--r--   0        0        0      264 2023-01-15 18:52:09.125336 apibara-0.7.0/src/apibara/starknet/__init__.py
--rw-r--r--   0        0        0     1038 2023-01-15 18:52:09.125336 apibara-0.7.0/src/apibara/starknet/cursor.py
--rw-r--r--   0        0        0     1375 2023-01-15 18:52:09.125336 apibara-0.7.0/src/apibara/starknet/felt.py
--rw-r--r--   0        0        0    14725 2023-03-16 21:14:54.127582 apibara-0.7.0/src/apibara/starknet/filter.py
--rw-r--r--   0        0        0      404 2023-01-15 18:52:09.125336 apibara-0.7.0/src/apibara/starknet/indexer.py
--rw-r--r--   0        0        0        0 2023-01-15 18:52:09.125336 apibara-0.7.0/src/apibara/starknet/proto/__init__.py
--rw-r--r--   0        0        0     7836 2023-07-08 12:11:24.025439 apibara-0.7.0/src/apibara/starknet/proto/filter_pb2.py
--rw-r--r--   0        0        0    12814 2023-07-08 12:11:24.025439 apibara-0.7.0/src/apibara/starknet/proto/filter_pb2.pyi
--rw-r--r--   0        0        0      158 2023-01-15 18:52:09.125336 apibara-0.7.0/src/apibara/starknet/proto/filter_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-01-15 18:52:09.125336 apibara-0.7.0/src/apibara/starknet/proto/filter_pb2_grpc.pyi
--rw-r--r--   0        0        0    11734 2023-07-08 12:11:24.025439 apibara-0.7.0/src/apibara/starknet/proto/starknet_pb2.py
--rw-r--r--   0        0        0    20085 2023-07-08 12:11:24.025439 apibara-0.7.0/src/apibara/starknet/proto/starknet_pb2.pyi
--rw-r--r--   0        0        0      158 2023-01-15 18:52:09.125336 apibara-0.7.0/src/apibara/starknet/proto/starknet_pb2_grpc.py
--rw-r--r--   0        0        0      100 2023-01-15 18:52:09.125336 apibara-0.7.0/src/apibara/starknet/proto/starknet_pb2_grpc.pyi
--rw-r--r--   0        0        0     1096 2023-06-30 17:37:45.778732 apibara-0.7.0/src/apibara/starknet/proto/types_pb2.py
--rw-r--r--   0        0        0      732 2023-06-30 17:37:45.775732 apibara-0.7.0/src/apibara/starknet/proto/types_pb2.pyi
--rw-r--r--   0        0        0      158 2023-01-15 18:52:09.125336 apibara-0.7.0/src/apibara/starknet/proto/types_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-01-15 18:52:09.125336 apibara-0.7.0/src/apibara/starknet/proto/types_pb2_grpc.pyi
--rw-r--r--   0        0        0     2408 1970-01-01 00:00:00.000000 apibara-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-01-15 18:52:09.124336 apibara-0.7.1/LICENSE.txt
+-rw-r--r--   0        0        0     1342 2023-01-18 12:16:07.977321 apibara-0.7.1/README.rst
+-rw-r--r--   0        0        0     1073 2023-07-14 20:14:53.243486 apibara-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-15 18:52:09.124336 apibara-0.7.1/src/apibara/__init__.py
+-rw-r--r--   0        0        0      514 2023-01-15 18:52:09.124336 apibara-0.7.1/src/apibara/cursor.py
+-rw-r--r--   0        0        0      160 2023-01-15 18:52:09.124336 apibara-0.7.1/src/apibara/indexer/__init__.py
+-rw-r--r--   0        0        0      375 2023-01-15 18:52:09.124336 apibara-0.7.1/src/apibara/indexer/configuration.py
+-rw-r--r--   0        0        0     2393 2023-03-16 21:14:54.127582 apibara-0.7.1/src/apibara/indexer/indexer.py
+-rw-r--r--   0        0        0     1026 2023-01-16 18:48:50.663792 apibara-0.7.1/src/apibara/indexer/info.py
+-rw-r--r--   0        0        0    10890 2023-07-14 20:14:20.212037 apibara-0.7.1/src/apibara/indexer/runner.py
+-rw-r--r--   0        0        0    10502 2023-06-08 12:55:13.026953 apibara-0.7.1/src/apibara/indexer/storage.py
+-rw-r--r--   0        0        0      697 2023-07-14 19:57:51.972597 apibara-0.7.1/src/apibara/protocol/__init__.py
+-rw-r--r--   0        0        0     3596 2023-07-14 19:57:51.971597 apibara-0.7.1/src/apibara/protocol/client.py
+-rw-r--r--   0        0        0        0 2023-01-15 18:52:09.125336 apibara-0.7.1/src/apibara/protocol/proto/__init__.py
+-rw-r--r--   0        0        0     3107 2023-01-15 18:52:09.125336 apibara-0.7.1/src/apibara/protocol/proto/stream_pb2.py
+-rw-r--r--   0        0        0     9814 2023-01-15 18:52:09.125336 apibara-0.7.1/src/apibara/protocol/proto/stream_pb2.pyi
+-rw-r--r--   0        0        0     2517 2023-01-15 18:52:09.125336 apibara-0.7.1/src/apibara/protocol/proto/stream_pb2_grpc.py
+-rw-r--r--   0        0        0      878 2023-01-15 18:52:09.125336 apibara-0.7.1/src/apibara/protocol/proto/stream_pb2_grpc.pyi
+-rw-r--r--   0        0        0      264 2023-01-15 18:52:09.125336 apibara-0.7.1/src/apibara/starknet/__init__.py
+-rw-r--r--   0        0        0     1038 2023-01-15 18:52:09.125336 apibara-0.7.1/src/apibara/starknet/cursor.py
+-rw-r--r--   0        0        0     1375 2023-01-15 18:52:09.125336 apibara-0.7.1/src/apibara/starknet/felt.py
+-rw-r--r--   0        0        0    14725 2023-03-16 21:14:54.127582 apibara-0.7.1/src/apibara/starknet/filter.py
+-rw-r--r--   0        0        0      404 2023-01-15 18:52:09.125336 apibara-0.7.1/src/apibara/starknet/indexer.py
+-rw-r--r--   0        0        0        0 2023-01-15 18:52:09.125336 apibara-0.7.1/src/apibara/starknet/proto/__init__.py
+-rw-r--r--   0        0        0     7836 2023-07-08 12:11:24.025439 apibara-0.7.1/src/apibara/starknet/proto/filter_pb2.py
+-rw-r--r--   0        0        0    12814 2023-07-08 12:11:24.025439 apibara-0.7.1/src/apibara/starknet/proto/filter_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-01-15 18:52:09.125336 apibara-0.7.1/src/apibara/starknet/proto/filter_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-01-15 18:52:09.125336 apibara-0.7.1/src/apibara/starknet/proto/filter_pb2_grpc.pyi
+-rw-r--r--   0        0        0    11734 2023-07-14 19:57:51.968597 apibara-0.7.1/src/apibara/starknet/proto/starknet_pb2.py
+-rw-r--r--   0        0        0    20085 2023-07-08 12:11:24.025439 apibara-0.7.1/src/apibara/starknet/proto/starknet_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-01-15 18:52:09.125336 apibara-0.7.1/src/apibara/starknet/proto/starknet_pb2_grpc.py
+-rw-r--r--   0        0        0      100 2023-01-15 18:52:09.125336 apibara-0.7.1/src/apibara/starknet/proto/starknet_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1096 2023-06-30 17:37:45.778732 apibara-0.7.1/src/apibara/starknet/proto/types_pb2.py
+-rw-r--r--   0        0        0      732 2023-06-30 17:37:45.775732 apibara-0.7.1/src/apibara/starknet/proto/types_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-01-15 18:52:09.125336 apibara-0.7.1/src/apibara/starknet/proto/types_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-01-15 18:52:09.125336 apibara-0.7.1/src/apibara/starknet/proto/types_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2408 1970-01-01 00:00:00.000000 apibara-0.7.1/PKG-INFO
```

### Comparing `apibara-0.7.0/LICENSE.txt` & `apibara-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apibara-0.7.0/README.rst` & `apibara-0.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `apibara-0.7.0/pyproject.toml` & `apibara-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apibara"
-version = "0.7.0"
+version = "0.7.1"
 description = "Apibara cliend SDK. Stream and transform on-chain data with Python."
 authors = ["Francesco Ceccon <francesco@apibara.com>"]
 license = "Apache-2.0"
 readme = "README.rst"
 homepage = "https://www.apibara.com"
 repository= "https://github.com/apibara/python-sdk"
 keywords = [
```

### Comparing `apibara-0.7.0/src/apibara/cursor.py` & `apibara-0.7.1/src/apibara/cursor.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.0/src/apibara/indexer/indexer.py` & `apibara-0.7.1/src/apibara/indexer/indexer.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.0/src/apibara/indexer/info.py` & `apibara-0.7.1/src/apibara/indexer/info.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.0/src/apibara/indexer/runner.py` & `apibara-0.7.1/src/apibara/indexer/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         self._retry_count = 0
 
         logger.debug("starting indexer")
         while True:
             try:
                 await self._connect_and_stream(indexer, ctx)
             except Exception as exc:
-                logger.debug(f"indexer exception {exc}")
+                logger.exception(f"indexer exception")
                 self._retry_count += 1
                 reconnect = await indexer.handle_reconnect(exc, self._retry_count)
 
                 if not reconnect.reconnect:
                     raise
 
     async def _connect_and_stream(self, indexer: Indexer, ctx: Optional[UserContext]):
@@ -201,17 +201,28 @@
                 pending_received = is_pending
 
                 end_cursor = message.data.end_cursor
                 cursor = message.data.cursor
 
                 logger.debug(f"handle batch {cursor} - {end_cursor}")
 
-                with self._indexer_storage.create_storage_for_data(
-                    message.data.end_cursor
-                ) as storage:
+                if is_pending:
+                    create_storage = (
+                        lambda cursor: self._indexer_storage.create_storage_for_pending(
+                            cursor
+                        )
+                    )
+                else:
+                    create_storage = (
+                        lambda cursor: self._indexer_storage.create_storage_for_data(
+                            cursor
+                        )
+                    )
+
+                with create_storage(message.data.end_cursor) as storage:
                     additional_filter = None
                     for batch in message.data.data:
                         decoded_data = indexer.decode_data(batch)
                         info = Info(
                             context=ctx,
                             storage=storage,
                             cursor=cursor,
```

### Comparing `apibara-0.7.0/src/apibara/indexer/storage.py` & `apibara-0.7.1/src/apibara/indexer/storage.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.0/src/apibara/protocol/__init__.py` & `apibara-0.7.1/src/apibara/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.0/src/apibara/protocol/client.py` & `apibara-0.7.1/src/apibara/protocol/client.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.0/src/apibara/protocol/proto/stream_pb2.py` & `apibara-0.7.1/src/apibara/protocol/proto/stream_pb2.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.0/src/apibara/protocol/proto/stream_pb2.pyi` & `apibara-0.7.1/src/apibara/protocol/proto/stream_pb2.pyi`

 * *Files identical despite different names*

### Comparing `apibara-0.7.0/src/apibara/protocol/proto/stream_pb2_grpc.py` & `apibara-0.7.1/src/apibara/protocol/proto/stream_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.0/src/apibara/protocol/proto/stream_pb2_grpc.pyi` & `apibara-0.7.1/src/apibara/protocol/proto/stream_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `apibara-0.7.0/src/apibara/starknet/cursor.py` & `apibara-0.7.1/src/apibara/starknet/cursor.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.0/src/apibara/starknet/felt.py` & `apibara-0.7.1/src/apibara/starknet/felt.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.0/src/apibara/starknet/filter.py` & `apibara-0.7.1/src/apibara/starknet/filter.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.0/src/apibara/starknet/proto/filter_pb2.py` & `apibara-0.7.1/src/apibara/starknet/proto/filter_pb2.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.0/src/apibara/starknet/proto/filter_pb2.pyi` & `apibara-0.7.1/src/apibara/starknet/proto/filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `apibara-0.7.0/src/apibara/starknet/proto/starknet_pb2.py` & `apibara-0.7.1/src/apibara/starknet/proto/starknet_pb2.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.0/src/apibara/starknet/proto/starknet_pb2.pyi` & `apibara-0.7.1/src/apibara/starknet/proto/starknet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `apibara-0.7.0/src/apibara/starknet/proto/types_pb2.py` & `apibara-0.7.1/src/apibara/starknet/proto/types_pb2.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.0/src/apibara/starknet/proto/types_pb2.pyi` & `apibara-0.7.1/src/apibara/starknet/proto/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `apibara-0.7.0/PKG-INFO` & `apibara-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apibara
-Version: 0.7.0
+Version: 0.7.1
 Summary: Apibara cliend SDK. Stream and transform on-chain data with Python.
 Home-page: https://www.apibara.com
 License: Apache-2.0
 Keywords: ethereum,web3,starknet
 Author: Francesco Ceccon
 Author-email: francesco@apibara.com
 Requires-Python: >=3.8,<3.11
```

