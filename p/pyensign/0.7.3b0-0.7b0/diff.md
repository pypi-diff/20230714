# Comparing `tmp/pyensign-0.7.3b0.tar.gz` & `tmp/pyensign-0.7b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyensign-0.7.3b0.tar", last modified: Fri Jul 14 17:19:07 2023, max compression
+gzip compressed data, was "pyensign-0.7b0.tar", last modified: Wed May 31 20:40:58 2023, max compression
```

## Comparing `pyensign-0.7.3b0.tar` & `pyensign-0.7b0.tar`

### file list

```diff
@@ -1,60 +1,54 @@
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-14 17:19:07.034302 pyensign-0.7.3b0/
--rw-r--r--   0 patrick    (501) staff       (20)    10536 2023-05-16 21:00:20.000000 pyensign-0.7.3b0/CONTRIBUTING.md
--rw-r--r--   0 patrick    (501) staff       (20)     2265 2023-07-14 14:39:16.000000 pyensign-0.7.3b0/DESCRIPTION.md
--rw-r--r--   0 patrick    (501) staff       (20)      180 2023-05-16 21:00:20.000000 pyensign-0.7.3b0/MANIFEST.in
--rw-r--r--   0 patrick    (501) staff       (20)      394 2023-05-16 21:00:20.000000 pyensign-0.7.3b0/Makefile
--rw-r--r--   0 patrick    (501) staff       (20)     3661 2023-07-14 17:19:07.034438 pyensign-0.7.3b0/PKG-INFO
--rw-r--r--   0 patrick    (501) staff       (20)     5637 2023-07-14 14:39:16.000000 pyensign-0.7.3b0/README.md
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-14 17:19:07.027070 pyensign-0.7.3b0/pyensign/
--rw-r--r--   0 patrick    (501) staff       (20)      507 2023-05-16 21:00:20.000000 pyensign-0.7.3b0/pyensign/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-14 17:19:07.028788 pyensign-0.7.3b0/pyensign/api/
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7.3b0/pyensign/api/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-14 17:19:07.030485 pyensign-0.7.3b0/pyensign/api/v1beta1/
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7.3b0/pyensign/api/v1beta1/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     7865 2023-05-16 21:00:20.000000 pyensign-0.7.3b0/pyensign/api/v1beta1/ensign_pb2.py
--rw-r--r--   0 patrick    (501) staff       (20)    19552 2023-05-16 21:00:20.000000 pyensign-0.7.3b0/pyensign/api/v1beta1/ensign_pb2_grpc.py
--rw-r--r--   0 patrick    (501) staff       (20)      809 2023-06-20 18:33:01.000000 pyensign-0.7.3b0/pyensign/api/v1beta1/event.py
--rw-r--r--   0 patrick    (501) staff       (20)     7539 2023-05-31 15:33:48.000000 pyensign-0.7.3b0/pyensign/api/v1beta1/event_pb2.py
--rw-r--r--   0 patrick    (501) staff       (20)     2367 2023-05-16 21:00:20.000000 pyensign-0.7.3b0/pyensign/api/v1beta1/groups_pb2.py
--rw-r--r--   0 patrick    (501) staff       (20)     4416 2023-05-16 21:00:20.000000 pyensign-0.7.3b0/pyensign/api/v1beta1/topic_pb2.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-14 17:19:07.031164 pyensign-0.7.3b0/pyensign/auth/
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7.3b0/pyensign/auth/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     4664 2023-06-20 18:33:01.000000 pyensign-0.7.3b0/pyensign/auth/client.py
--rw-r--r--   0 patrick    (501) staff       (20)      347 2023-05-16 21:00:20.000000 pyensign-0.7.3b0/pyensign/auth/tokens.py
--rw-r--r--   0 patrick    (501) staff       (20)     8988 2023-07-14 14:39:16.000000 pyensign-0.7.3b0/pyensign/connection.py
--rw-r--r--   0 patrick    (501) staff       (20)    15456 2023-07-14 14:39:16.000000 pyensign-0.7.3b0/pyensign/ensign.py
--rw-r--r--   0 patrick    (501) staff       (20)     6362 2023-06-20 18:33:01.000000 pyensign-0.7.3b0/pyensign/events.py
--rw-r--r--   0 patrick    (501) staff       (20)     6047 2023-06-28 21:07:54.000000 pyensign-0.7.3b0/pyensign/exceptions.py
--rw-r--r--   0 patrick    (501) staff       (20)     4112 2023-07-14 17:13:10.000000 pyensign-0.7.3b0/pyensign/iterator.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-14 17:19:07.031439 pyensign-0.7.3b0/pyensign/mimetype/
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7.3b0/pyensign/mimetype/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-14 17:19:07.031819 pyensign-0.7.3b0/pyensign/mimetype/v1beta1/
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7.3b0/pyensign/mimetype/v1beta1/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     2376 2023-05-16 21:00:20.000000 pyensign-0.7.3b0/pyensign/mimetype/v1beta1/mimetype_pb2.py
--rw-r--r--   0 patrick    (501) staff       (20)     5383 2023-05-31 15:33:48.000000 pyensign-0.7.3b0/pyensign/mimetypes.py
--rw-r--r--   0 patrick    (501) staff       (20)     2472 2023-06-28 21:07:54.000000 pyensign-0.7.3b0/pyensign/publisher.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-14 17:19:07.032034 pyensign-0.7.3b0/pyensign/region/
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7.3b0/pyensign/region/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-14 17:19:07.032470 pyensign-0.7.3b0/pyensign/region/v1beta1/
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7.3b0/pyensign/region/v1beta1/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     7945 2023-05-16 21:00:20.000000 pyensign-0.7.3b0/pyensign/region/v1beta1/region_pb2.py
--rw-r--r--   0 patrick    (501) staff       (20)    10993 2023-07-14 14:39:16.000000 pyensign-0.7.3b0/pyensign/stream.py
--rw-r--r--   0 patrick    (501) staff       (20)     2146 2023-07-14 14:39:16.000000 pyensign-0.7.3b0/pyensign/subscriber.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-14 17:19:07.034099 pyensign-0.7.3b0/pyensign/utils/
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-31 18:56:39.000000 pyensign-0.7.3b0/pyensign/utils/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     1454 2023-06-28 21:07:54.000000 pyensign-0.7.3b0/pyensign/utils/cache.py
--rw-r--r--   0 patrick    (501) staff       (20)     1542 2023-07-14 14:57:31.000000 pyensign-0.7.3b0/pyensign/utils/queue.py
--rw-r--r--   0 patrick    (501) staff       (20)     1089 2023-07-12 19:59:49.000000 pyensign-0.7.3b0/pyensign/utils/tasks.py
--rw-r--r--   0 patrick    (501) staff       (20)     1297 2023-06-28 21:07:54.000000 pyensign-0.7.3b0/pyensign/utils/topics.py
--rw-r--r--   0 patrick    (501) staff       (20)     1108 2023-07-14 17:18:40.000000 pyensign-0.7.3b0/pyensign/version.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-14 17:19:07.028547 pyensign-0.7.3b0/pyensign.egg-info/
--rw-r--r--   0 patrick    (501) staff       (20)     3661 2023-07-14 17:19:06.000000 pyensign-0.7.3b0/pyensign.egg-info/PKG-INFO
--rw-r--r--   0 patrick    (501) staff       (20)     1210 2023-07-14 17:19:07.000000 pyensign-0.7.3b0/pyensign.egg-info/SOURCES.txt
--rw-r--r--   0 patrick    (501) staff       (20)        1 2023-07-14 17:19:06.000000 pyensign-0.7.3b0/pyensign.egg-info/dependency_links.txt
--rw-r--r--   0 patrick    (501) staff       (20)        1 2023-07-14 17:19:06.000000 pyensign-0.7.3b0/pyensign.egg-info/not-zip-safe
--rw-r--r--   0 patrick    (501) staff       (20)       64 2023-07-14 17:19:06.000000 pyensign-0.7.3b0/pyensign.egg-info/requires.txt
--rw-r--r--   0 patrick    (501) staff       (20)        9 2023-07-14 17:19:06.000000 pyensign-0.7.3b0/pyensign.egg-info/top_level.txt
--rw-r--r--   0 patrick    (501) staff       (20)       47 2023-06-20 18:33:01.000000 pyensign-0.7.3b0/pyproject.toml
--rw-r--r--   0 patrick    (501) staff       (20)       63 2023-06-20 18:33:01.000000 pyensign-0.7.3b0/requirements.txt
--rw-r--r--   0 patrick    (501) staff       (20)       38 2023-07-14 17:19:07.034743 pyensign-0.7.3b0/setup.cfg
--rw-r--r--   0 patrick    (501) staff       (20)     4023 2023-05-16 21:00:20.000000 pyensign-0.7.3b0/setup.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.854409 pyensign-0.7b0/
+-rw-r--r--   0 patrick    (501) staff       (20)    10536 2023-05-16 21:00:20.000000 pyensign-0.7b0/CONTRIBUTING.md
+-rw-r--r--   0 patrick    (501) staff       (20)     2360 2023-05-31 19:58:09.000000 pyensign-0.7b0/DESCRIPTION.md
+-rw-r--r--   0 patrick    (501) staff       (20)      180 2023-05-16 21:00:20.000000 pyensign-0.7b0/MANIFEST.in
+-rw-r--r--   0 patrick    (501) staff       (20)      394 2023-05-16 21:00:20.000000 pyensign-0.7b0/Makefile
+-rw-r--r--   0 patrick    (501) staff       (20)     3752 2023-05-31 20:40:58.854558 pyensign-0.7b0/PKG-INFO
+-rw-r--r--   0 patrick    (501) staff       (20)     4329 2023-05-31 19:58:28.000000 pyensign-0.7b0/README.md
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.846230 pyensign-0.7b0/pyensign/
+-rw-r--r--   0 patrick    (501) staff       (20)      507 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.848027 pyensign-0.7b0/pyensign/api/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/api/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.850724 pyensign-0.7b0/pyensign/api/v1beta1/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/api/v1beta1/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7865 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/api/v1beta1/ensign_pb2.py
+-rw-r--r--   0 patrick    (501) staff       (20)    19552 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/api/v1beta1/ensign_pb2_grpc.py
+-rw-r--r--   0 patrick    (501) staff       (20)      786 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/api/v1beta1/event.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7539 2023-05-31 15:33:48.000000 pyensign-0.7b0/pyensign/api/v1beta1/event_pb2.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2367 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/api/v1beta1/groups_pb2.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4416 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/api/v1beta1/topic_pb2.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.851841 pyensign-0.7b0/pyensign/auth/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/auth/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3937 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/auth/client.py
+-rw-r--r--   0 patrick    (501) staff       (20)      347 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/auth/tokens.py
+-rw-r--r--   0 patrick    (501) staff       (20)    11976 2023-05-31 18:56:39.000000 pyensign-0.7b0/pyensign/connection.py
+-rw-r--r--   0 patrick    (501) staff       (20)    10517 2023-05-31 15:33:48.000000 pyensign-0.7b0/pyensign/ensign.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1905 2023-05-31 15:33:48.000000 pyensign-0.7b0/pyensign/events.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3601 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/exceptions.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.852166 pyensign-0.7b0/pyensign/mimetype/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/mimetype/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.852581 pyensign-0.7b0/pyensign/mimetype/v1beta1/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/mimetype/v1beta1/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2376 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/mimetype/v1beta1/mimetype_pb2.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5383 2023-05-31 15:33:48.000000 pyensign-0.7b0/pyensign/mimetypes.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.852880 pyensign-0.7b0/pyensign/region/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/region/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.853269 pyensign-0.7b0/pyensign/region/v1beta1/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/region/v1beta1/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7945 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/region/v1beta1/region_pb2.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.854128 pyensign-0.7b0/pyensign/utils/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-31 18:56:39.000000 pyensign-0.7b0/pyensign/utils/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)      983 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/utils/cache.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1089 2023-05-31 15:33:49.000000 pyensign-0.7b0/pyensign/utils/tasks.py
+-rw-r--r--   0 patrick    (501) staff       (20)      964 2023-05-31 19:17:18.000000 pyensign-0.7b0/pyensign/version.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.847769 pyensign-0.7b0/pyensign.egg-info/
+-rw-r--r--   0 patrick    (501) staff       (20)     3752 2023-05-31 20:40:58.000000 pyensign-0.7b0/pyensign.egg-info/PKG-INFO
+-rw-r--r--   0 patrick    (501) staff       (20)     1076 2023-05-31 20:40:58.000000 pyensign-0.7b0/pyensign.egg-info/SOURCES.txt
+-rw-r--r--   0 patrick    (501) staff       (20)        1 2023-05-31 20:40:58.000000 pyensign-0.7b0/pyensign.egg-info/dependency_links.txt
+-rw-r--r--   0 patrick    (501) staff       (20)        1 2023-05-31 20:40:58.000000 pyensign-0.7b0/pyensign.egg-info/not-zip-safe
+-rw-r--r--   0 patrick    (501) staff       (20)       89 2023-05-31 20:40:58.000000 pyensign-0.7b0/pyensign.egg-info/requires.txt
+-rw-r--r--   0 patrick    (501) staff       (20)        9 2023-05-31 20:40:58.000000 pyensign-0.7b0/pyensign.egg-info/top_level.txt
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyproject.toml
+-rw-r--r--   0 patrick    (501) staff       (20)       88 2023-05-31 18:56:39.000000 pyensign-0.7b0/requirements.txt
+-rw-r--r--   0 patrick    (501) staff       (20)       38 2023-05-31 20:40:58.854916 pyensign-0.7b0/setup.cfg
+-rw-r--r--   0 patrick    (501) staff       (20)     4023 2023-05-16 21:00:20.000000 pyensign-0.7b0/setup.py
```

### Comparing `pyensign-0.7.3b0/CONTRIBUTING.md` & `pyensign-0.7b0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyensign-0.7.3b0/DESCRIPTION.md` & `pyensign-0.7b0/DESCRIPTION.md`

 * *Files 14% similar despite different names*

```diff
@@ -30,29 +30,29 @@
 
 ```python
 await client.publish("weather", event)
 await client.publish("weather", event1, event2)
 await client.publish("weather", [event1, event2])
 ```
 
-Subscribe to one or more topics by providing the topic name(s) or ID(s).
+Subscribe to one or more topic IDs. Topic IDs are assigned by Ensign so a common pattern is to first retrieve the topic ID from the topic name.
 
 ```python
-async for event in client.subscribe("weather"):
-    print("Received event with data: {}".format(event.data))
-    event.ack()
+topic_id = await client.topic_id("weather")
+async for event in client.subscribe(topic_id):
+    print("Received event: {}".format(event))
 ```
 
 ## Advanced Usage
 
 The `publish` coroutine accepts asynchronous callbacks so the client can distinguish between committed and uncommitted events. Callbacks are invoked when acks and nacks are received from the server and the first argument passed to the callback is the `Ack` or `Nack` itself. An `Ack` contains a committed timestamp. A `Nack` is returned if the event couldn't be committed and contains the ID of the event along with an error describing what went wrong.
 
 ```python
 async def handle_ack(self, ack):
     ts = datetime.fromtimestamp(ack.committed.seconds + ack.committed.nanos / 1e9)
     print(f"Event committed at {ts}")
 
 async def handle_nack(self, nack):
     print(f"Could not commit event {nack.id} with error {nack.code}: {nack.error}")
 
-await client.publish("weather", event, on_ack=handle_ack, on_nack=handle_nack)
+await client.publish("weather", event, ack_callback=handle_ack, nack_callback=handle_nack)
 ```
```

### Comparing `pyensign-0.7.3b0/PKG-INFO` & `pyensign-0.7b0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pyensign
-Version: 0.7.3b0
+Version: 0.7b0
 Summary: Ensign driver, SDK, and helpers for Python
 Home-page: https://github.com/rotationalio/pyensign
 Author: Patrick Deziel
 Author-email: deziel.patrick@gmail.com
 Maintainer: Patrick Deziel
 Maintainer-email: deziel.patrick@gmail.com
 License: BSD
-Download-URL: https://github.com/rotationalio/pyensign/tarball/v0.7.3b0
+Download-URL: https://github.com/rotationalio/pyensign/tarball/v0.7b0
 Description: # PyEnsign
         
         PyEnsign is the official Python SDK for [Ensign](https://rotational.io/ensign), a distributed event store and stream-processing platform. This library allows you to interact with the Ensign API directly from Python in order to create [publishers](https://ensign.rotational.dev/eventing/glossary/#publisher) and [subscribers](https://ensign.rotational.dev/eventing/glossary/#subscriber).
         
         ## Installation
         
         ```
@@ -41,35 +41,35 @@
         
         ```python
         await client.publish("weather", event)
         await client.publish("weather", event1, event2)
         await client.publish("weather", [event1, event2])
         ```
         
-        Subscribe to one or more topics by providing the topic name(s) or ID(s).
+        Subscribe to one or more topic IDs. Topic IDs are assigned by Ensign so a common pattern is to first retrieve the topic ID from the topic name.
         
         ```python
-        async for event in client.subscribe("weather"):
-            print("Received event with data: {}".format(event.data))
-            event.ack()
+        topic_id = await client.topic_id("weather")
+        async for event in client.subscribe(topic_id):
+            print("Received event: {}".format(event))
         ```
         
         ## Advanced Usage
         
         The `publish` coroutine accepts asynchronous callbacks so the client can distinguish between committed and uncommitted events. Callbacks are invoked when acks and nacks are received from the server and the first argument passed to the callback is the `Ack` or `Nack` itself. An `Ack` contains a committed timestamp. A `Nack` is returned if the event couldn't be committed and contains the ID of the event along with an error describing what went wrong.
         
         ```python
         async def handle_ack(self, ack):
             ts = datetime.fromtimestamp(ack.committed.seconds + ack.committed.nanos / 1e9)
             print(f"Event committed at {ts}")
         
         async def handle_nack(self, nack):
             print(f"Could not commit event {nack.id} with error {nack.code}: {nack.error}")
         
-        await client.publish("weather", event, on_ack=handle_ack, on_nack=handle_nack)
+        await client.publish("weather", event, ack_callback=handle_ack, nack_callback=handle_nack)
         ```
 Keywords: python,setup,pypi
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
```

### Comparing `pyensign-0.7.3b0/pyensign/api/v1beta1/ensign_pb2.py` & `pyensign-0.7b0/pyensign/api/v1beta1/ensign_pb2.py`

 * *Files identical despite different names*

### Comparing `pyensign-0.7.3b0/pyensign/api/v1beta1/ensign_pb2_grpc.py` & `pyensign-0.7b0/pyensign/api/v1beta1/ensign_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pyensign-0.7.3b0/pyensign/api/v1beta1/event.py` & `pyensign-0.7b0/pyensign/api/v1beta1/event.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     if not isinstance(event, event_pb2.Event):
         raise TypeError("event must be a protobuf event")
 
     if not isinstance(topic_id, ULID):
         raise TypeError("topic_id must be a ULID")
 
     return event_pb2.EventWrapper(
-        local_id=ULID().bytes, event=event.SerializeToString(), topic_id=topic_id.bytes
+        event=event.SerializeToString(), topic_id=topic_id.bytes
     )
 
 
 def unwrap(event_wrapper):
     """
     Unwrap an event from an EventWrapper.
     """
```

### Comparing `pyensign-0.7.3b0/pyensign/api/v1beta1/event_pb2.py` & `pyensign-0.7b0/pyensign/api/v1beta1/event_pb2.py`

 * *Files identical despite different names*

### Comparing `pyensign-0.7.3b0/pyensign/api/v1beta1/groups_pb2.py` & `pyensign-0.7b0/pyensign/api/v1beta1/groups_pb2.py`

 * *Files identical despite different names*

### Comparing `pyensign-0.7.3b0/pyensign/api/v1beta1/topic_pb2.py` & `pyensign-0.7b0/pyensign/api/v1beta1/topic_pb2.py`

 * *Files identical despite different names*

### Comparing `pyensign-0.7.3b0/pyensign/mimetype/v1beta1/mimetype_pb2.py` & `pyensign-0.7b0/pyensign/mimetype/v1beta1/mimetype_pb2.py`

 * *Files identical despite different names*

### Comparing `pyensign-0.7.3b0/pyensign/mimetypes.py` & `pyensign-0.7b0/pyensign/mimetypes.py`

 * *Files identical despite different names*

### Comparing `pyensign-0.7.3b0/pyensign/region/v1beta1/region_pb2.py` & `pyensign-0.7b0/pyensign/region/v1beta1/region_pb2.py`

 * *Files identical despite different names*

### Comparing `pyensign-0.7.3b0/pyensign/utils/cache.py` & `pyensign-0.7b0/pyensign/utils/cache.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,27 +4,16 @@
 class Cache:
     """
     Cache is a simple cache that maps keys to values to avoid repeated RPC calls to
     Ensign. This is not thread-safe.
     TODO: Implement max size and evictions.
     """
 
-    def __init__(self, read_only=False):
-        """
-        Create a new cache.
-
-        Parameters
-        ----------
-        read_only : bool (default: False)
-            If True, the cache will not be writeable. This creates a disabled cache
-            where get() will always raise a CacheMissError, exists() will always return
-            False, and add() is a no-op.
-        """
+    def __init__(self):
         self._index = {}
-        self._read_only = read_only
 
     def get(self, key):
         """
         Get a value by name, an exception is raised if the key does not exist in the
         cache.
         """
         try:
@@ -32,22 +21,20 @@
         except KeyError as e:
             raise CacheMissError(key) from e
 
     def add(self, key, value):
         """
         Add a value by key to the cache, overwriting the existing key.
         """
-        if not self._read_only:
-            self._index[key] = value
+        self._index[key] = value
 
     def exists(self, key):
         """
         Returns True if the key exists in the cache.
         """
         return key in self._index
 
     def clear(self):
         """
         Reset the cache, deleting all keys.
         """
-        if not self._read_only:
-            self._index.clear()
+        self._index.clear()
```

### Comparing `pyensign-0.7.3b0/pyensign/utils/tasks.py` & `pyensign-0.7b0/pyensign/utils/tasks.py`

 * *Files identical despite different names*

### Comparing `pyensign-0.7.3b0/pyensign/version.py` & `pyensign-0.7b0/pyensign/version.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,32 @@
 ##########################################################################
 ## Module Info
 ##########################################################################
 
 __version_info__ = {
     "major": 0,
     "minor": 7,
-    "micro": 3,
+    "micro": 0,
     "releaselevel": "beta",
     "serial": 0,
 }
 
 ##########################################################################
 ## Helper Functions
 ##########################################################################
 
 
 def get_version(short=False):
     """
-    Returns the version string for pyensign.
+    Prints the version.
     """
     assert __version_info__["releaselevel"] in ("alpha", "beta", "final")
     vers = [
         "%(major)i.%(minor)i" % __version_info__,
     ]
     if __version_info__["micro"]:
         vers.append(".%(micro)i" % __version_info__)
     if __version_info__["releaselevel"] != "final" and not short:
         vers.append(
             "%s%i" % (__version_info__["releaselevel"][0], __version_info__["serial"])
         )
     return "".join(vers)
-
-
-def user_agent():
-    """
-    Returns the user agent string for pyensign.
-    """
-    return "pyensign/" + get_version()
```

### Comparing `pyensign-0.7.3b0/pyensign.egg-info/PKG-INFO` & `pyensign-0.7b0/pyensign.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pyensign
-Version: 0.7.3b0
+Version: 0.7b0
 Summary: Ensign driver, SDK, and helpers for Python
 Home-page: https://github.com/rotationalio/pyensign
 Author: Patrick Deziel
 Author-email: deziel.patrick@gmail.com
 Maintainer: Patrick Deziel
 Maintainer-email: deziel.patrick@gmail.com
 License: BSD
-Download-URL: https://github.com/rotationalio/pyensign/tarball/v0.7.3b0
+Download-URL: https://github.com/rotationalio/pyensign/tarball/v0.7b0
 Description: # PyEnsign
         
         PyEnsign is the official Python SDK for [Ensign](https://rotational.io/ensign), a distributed event store and stream-processing platform. This library allows you to interact with the Ensign API directly from Python in order to create [publishers](https://ensign.rotational.dev/eventing/glossary/#publisher) and [subscribers](https://ensign.rotational.dev/eventing/glossary/#subscriber).
         
         ## Installation
         
         ```
@@ -41,35 +41,35 @@
         
         ```python
         await client.publish("weather", event)
         await client.publish("weather", event1, event2)
         await client.publish("weather", [event1, event2])
         ```
         
-        Subscribe to one or more topics by providing the topic name(s) or ID(s).
+        Subscribe to one or more topic IDs. Topic IDs are assigned by Ensign so a common pattern is to first retrieve the topic ID from the topic name.
         
         ```python
-        async for event in client.subscribe("weather"):
-            print("Received event with data: {}".format(event.data))
-            event.ack()
+        topic_id = await client.topic_id("weather")
+        async for event in client.subscribe(topic_id):
+            print("Received event: {}".format(event))
         ```
         
         ## Advanced Usage
         
         The `publish` coroutine accepts asynchronous callbacks so the client can distinguish between committed and uncommitted events. Callbacks are invoked when acks and nacks are received from the server and the first argument passed to the callback is the `Ack` or `Nack` itself. An `Ack` contains a committed timestamp. A `Nack` is returned if the event couldn't be committed and contains the ID of the event along with an error describing what went wrong.
         
         ```python
         async def handle_ack(self, ack):
             ts = datetime.fromtimestamp(ack.committed.seconds + ack.committed.nanos / 1e9)
             print(f"Event committed at {ts}")
         
         async def handle_nack(self, nack):
             print(f"Could not commit event {nack.id} with error {nack.code}: {nack.error}")
         
-        await client.publish("weather", event, on_ack=handle_ack, on_nack=handle_nack)
+        await client.publish("weather", event, ack_callback=handle_ack, nack_callback=handle_nack)
         ```
 Keywords: python,setup,pypi
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
```

### Comparing `pyensign-0.7.3b0/pyensign.egg-info/SOURCES.txt` & `pyensign-0.7b0/pyensign.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,15 @@
 setup.cfg
 setup.py
 pyensign/__init__.py
 pyensign/connection.py
 pyensign/ensign.py
 pyensign/events.py
 pyensign/exceptions.py
-pyensign/iterator.py
 pyensign/mimetypes.py
-pyensign/publisher.py
-pyensign/stream.py
-pyensign/subscriber.py
 pyensign/version.py
 pyensign.egg-info/PKG-INFO
 pyensign.egg-info/SOURCES.txt
 pyensign.egg-info/dependency_links.txt
 pyensign.egg-info/not-zip-safe
 pyensign.egg-info/requires.txt
 pyensign.egg-info/top_level.txt
@@ -39,10 +35,8 @@
 pyensign/mimetype/v1beta1/__init__.py
 pyensign/mimetype/v1beta1/mimetype_pb2.py
 pyensign/region/__init__.py
 pyensign/region/v1beta1/__init__.py
 pyensign/region/v1beta1/region_pb2.py
 pyensign/utils/__init__.py
 pyensign/utils/cache.py
-pyensign/utils/queue.py
-pyensign/utils/tasks.py
-pyensign/utils/topics.py
+pyensign/utils/tasks.py
```

### Comparing `pyensign-0.7.3b0/setup.py` & `pyensign-0.7b0/setup.py`

 * *Files identical despite different names*

