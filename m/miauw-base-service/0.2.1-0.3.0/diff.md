# Comparing `tmp/miauw-base-service-0.2.1.tar.gz` & `tmp/miauw-base-service-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miauw-base-service-0.2.1.tar", last modified: Thu Jul 13 14:25:36 2023, max compression
+gzip compressed data, was "miauw-base-service-0.3.0.tar", last modified: Fri Jul 14 10:12:08 2023, max compression
```

## Comparing `miauw-base-service-0.2.1.tar` & `miauw-base-service-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-13 14:25:36.480947 miauw-base-service-0.2.1/
--rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-13 14:25:36.480947 miauw-base-service-0.2.1/PKG-INFO
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-13 14:25:36.480947 miauw-base-service-0.2.1/base_service/
--rw-r--r--   0 leo       (1000) leo       (1000)       63 2023-07-13 05:13:50.000000 miauw-base-service-0.2.1/base_service/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)     1850 2023-07-13 09:02:41.000000 miauw-base-service-0.2.1/base_service/service.py
--rw-r--r--   0 leo       (1000) leo       (1000)     1677 2023-07-13 09:00:52.000000 miauw-base-service-0.2.1/base_service/worker.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-13 14:25:36.480947 miauw-base-service-0.2.1/miauw_base_service.egg-info/
--rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-13 14:25:36.000000 miauw-base-service-0.2.1/miauw_base_service.egg-info/PKG-INFO
--rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-13 14:25:36.000000 miauw-base-service-0.2.1/miauw_base_service.egg-info/SOURCES.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        1 2023-07-13 14:25:36.000000 miauw-base-service-0.2.1/miauw_base_service.egg-info/dependency_links.txt
--rw-r--r--   0 leo       (1000) leo       (1000)       23 2023-07-13 14:25:36.000000 miauw-base-service-0.2.1/miauw_base_service.egg-info/requires.txt
--rw-r--r--   0 leo       (1000) leo       (1000)       31 2023-07-13 14:25:36.000000 miauw-base-service-0.2.1/miauw_base_service.egg-info/top_level.txt
--rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-13 14:23:06.000000 miauw-base-service-0.2.1/pyproject.toml
--rw-r--r--   0 leo       (1000) leo       (1000)       38 2023-07-13 14:25:36.480947 miauw-base-service-0.2.1/setup.cfg
--rw-r--r--   0 leo       (1000) leo       (1000)      437 2023-07-13 14:22:39.000000 miauw-base-service-0.2.1/setup.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-14 10:12:08.369837 miauw-base-service-0.3.0/
+-rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-14 10:12:08.366504 miauw-base-service-0.3.0/PKG-INFO
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-14 10:12:08.366504 miauw-base-service-0.3.0/base_service/
+-rw-r--r--   0 leo       (1000) leo       (1000)       63 2023-07-13 05:13:50.000000 miauw-base-service-0.3.0/base_service/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     1850 2023-07-13 09:02:41.000000 miauw-base-service-0.3.0/base_service/service.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     1879 2023-07-14 10:06:11.000000 miauw-base-service-0.3.0/base_service/worker.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-14 10:12:08.366504 miauw-base-service-0.3.0/miauw_base_service.egg-info/
+-rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-14 10:12:08.000000 miauw-base-service-0.3.0/miauw_base_service.egg-info/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-14 10:12:08.000000 miauw-base-service-0.3.0/miauw_base_service.egg-info/SOURCES.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        1 2023-07-14 10:12:08.000000 miauw-base-service-0.3.0/miauw_base_service.egg-info/dependency_links.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)       23 2023-07-14 10:12:08.000000 miauw-base-service-0.3.0/miauw_base_service.egg-info/requires.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)       31 2023-07-14 10:12:08.000000 miauw-base-service-0.3.0/miauw_base_service.egg-info/top_level.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-14 10:04:54.000000 miauw-base-service-0.3.0/pyproject.toml
+-rw-r--r--   0 leo       (1000) leo       (1000)       38 2023-07-14 10:12:08.369837 miauw-base-service-0.3.0/setup.cfg
+-rw-r--r--   0 leo       (1000) leo       (1000)      437 2023-07-14 10:11:27.000000 miauw-base-service-0.3.0/setup.py
```

### Comparing `miauw-base-service-0.2.1/base_service/service.py` & `miauw-base-service-0.3.0/base_service/service.py`

 * *Files identical despite different names*

### Comparing `miauw-base-service-0.2.1/base_service/worker.py` & `miauw-base-service-0.3.0/base_service/worker.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,48 @@
 from typing import Callable, Awaitable, Any
 import aio_pika
 import json
 import asyncio
 
+
 class RabbitMQWorker:
     """RabbitMQ Base Worker Class"""
+
     def __init__(self, url: str):
         self.connection = None
         self.url: str = url
         self.channel: aio_pika.abc.AbstractChannel = None
         self.ex: aio_pika.abc.AbstractExchange = None
 
     async def setup(self, chan_id: int | None = None) -> "RabbitMQWorker":
         """setup worker"""
         self.connection = await aio_pika.connect(self.url)
         self.channel = await self.connection.channel(channel_number=chan_id)
         self.ex = self.channel.default_exchange
         return self
 
-    async def listen(self, queue_name: str, worker_function: Callable[[dict], Awaitable[dict]]):
+    async def send_basic(self, queue_name: str, data: bytes) -> None:
+        """sends something to queue"""
+        await self.ex.publish(aio_pika.Message(data), routing_key=queue_name)
+
+    async def listen(
+        self, queue_name: str, worker_function: Callable[[dict], Awaitable[dict]]
+    ):
         await self.setup()
         queue = await self.channel.declare_queue(queue_name)
         async with queue.iterator() as qi:
             message: aio_pika.abc.AbstractMessage
             async for message in qi:
                 try:
                     async with message.process(requeue=False):
                         assert message.reply_to is not None
                         data: dict = json.loads(message.body)
                         res = await worker_function(data)
                         await self.ex.publish(
                             aio_pika.Message(
-                                body = json.dumps(res).encode("utf-8"),
-                                correlation_id=message.correlation_id
+                                body=json.dumps(res).encode("utf-8"),
+                                correlation_id=message.correlation_id,
                             ),
-                            routing_key=message.reply_to
+                            routing_key=message.reply_to,
                         )
                 except Exception as e:
                     print("[!] Exception: ", e)
-
-
```

