# Comparing `tmp/acapy-plugin-pickup-0.1.0.post1.tar.gz` & `tmp/acapy_plugin_pickup-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acapy-plugin-pickup-0.1.0.post1.tar", max compression
+gzip compressed data, was "acapy_plugin_pickup-0.2.0.tar", max compression
```

## Comparing `acapy-plugin-pickup-0.1.0.post1.tar` & `acapy_plugin_pickup-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0    11402 2022-08-25 15:59:04.600395 acapy-plugin-pickup-0.1.0.post1/LICENSE
--rw-r--r--   0        0        0      909 2022-08-25 15:13:48.632839 acapy-plugin-pickup-0.1.0.post1/acapy_plugin_pickup/__init__.py
--rw-r--r--   0        0        0      168 2022-04-07 16:06:38.490397 acapy-plugin-pickup-0.1.0.post1/acapy_plugin_pickup/acapy/__init__.py
--rw-r--r--   0        0        0      192 2021-09-28 16:39:50.449139 acapy-plugin-pickup-0.1.0.post1/acapy_plugin_pickup/acapy/error.py
--rw-r--r--   0        0        0     7313 2022-04-07 16:06:38.490397 acapy-plugin-pickup-0.1.0.post1/acapy_plugin_pickup/acapy/message.py
--rw-r--r--   0        0        0        0 2022-04-07 16:06:38.490397 acapy-plugin-pickup-0.1.0.post1/acapy_plugin_pickup/protocol/__init__.py
--rw-r--r--   0        0        0     6999 2022-08-25 15:13:48.633839 acapy-plugin-pickup-0.1.0.post1/acapy_plugin_pickup/protocol/delivery.py
--rw-r--r--   0        0        0      702 2022-04-07 16:06:38.490397 acapy-plugin-pickup-0.1.0.post1/acapy_plugin_pickup/protocol/live_mode.py
--rw-r--r--   0        0        0     1835 2022-08-25 15:13:48.633839 acapy-plugin-pickup-0.1.0.post1/acapy_plugin_pickup/protocol/status.py
--rw-r--r--   0        0        0      510 2021-09-28 16:39:50.449139 acapy-plugin-pickup-0.1.0.post1/acapy_plugin_pickup/valid.py
--rw-r--r--   0        0        0      788 2022-08-25 16:15:45.918950 acapy-plugin-pickup-0.1.0.post1/pyproject.toml
--rw-r--r--   0        0        0      897 2022-08-25 16:15:52.295862 acapy-plugin-pickup-0.1.0.post1/setup.py
--rw-r--r--   0        0        0      780 2022-08-25 16:15:52.296370 acapy-plugin-pickup-0.1.0.post1/PKG-INFO
+-rw-r--r--   0        0        0    11402 2023-07-14 17:46:20.682919 acapy_plugin_pickup-0.2.0/LICENSE
+-rw-r--r--   0        0        0       37 2023-07-14 17:46:20.682919 acapy_plugin_pickup-0.2.0/acapy_plugin_pickup/__init__.py
+-rw-r--r--   0        0        0      168 2023-07-14 17:46:20.682919 acapy_plugin_pickup-0.2.0/acapy_plugin_pickup/acapy/__init__.py
+-rw-r--r--   0        0        0      192 2023-07-14 17:46:20.682919 acapy_plugin_pickup-0.2.0/acapy_plugin_pickup/acapy/error.py
+-rw-r--r--   0        0        0     7446 2023-07-14 17:46:20.682919 acapy_plugin_pickup-0.2.0/acapy_plugin_pickup/acapy/message.py
+-rw-r--r--   0        0        0      197 2023-07-14 17:46:20.682919 acapy_plugin_pickup-0.2.0/acapy_plugin_pickup/definition.py
+-rw-r--r--   0        0        0        0 2023-07-14 17:46:20.682919 acapy_plugin_pickup-0.2.0/acapy_plugin_pickup/v2_0/__init__.py
+-rw-r--r--   0        0        0     6893 2023-07-14 17:46:20.682919 acapy_plugin_pickup-0.2.0/acapy_plugin_pickup/v2_0/delivery.py
+-rw-r--r--   0        0        0      702 2023-07-14 17:46:20.682919 acapy_plugin_pickup-0.2.0/acapy_plugin_pickup/v2_0/live_mode.py
+-rw-r--r--   0        0        0      939 2023-07-14 17:46:20.682919 acapy_plugin_pickup-0.2.0/acapy_plugin_pickup/v2_0/message_types.py
+-rw-r--r--   0        0        0      696 2023-07-14 17:46:20.682919 acapy_plugin_pickup-0.2.0/acapy_plugin_pickup/v2_0/routes.py
+-rw-r--r--   0        0        0     1835 2023-07-14 17:46:20.682919 acapy_plugin_pickup-0.2.0/acapy_plugin_pickup/v2_0/status.py
+-rw-r--r--   0        0        0      510 2023-07-14 17:46:20.682919 acapy_plugin_pickup-0.2.0/acapy_plugin_pickup/valid.py
+-rw-r--r--   0        0        0      689 2023-07-14 17:46:20.686919 acapy_plugin_pickup-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 acapy_plugin_pickup-0.2.0/PKG-INFO
```

### Comparing `acapy-plugin-pickup-0.1.0.post1/LICENSE` & `acapy_plugin_pickup-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `acapy-plugin-pickup-0.1.0.post1/acapy_plugin_pickup/acapy/message.py` & `acapy_plugin_pickup-0.2.0/acapy_plugin_pickup/acapy/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,14 +172,19 @@
         return value
 
     @property
     def _id(self):
         return self.id
 
     @property
+    def _message_type(self):
+        """Return the message type for this message."""
+        return self.message_type
+
+    @property
     def _thread_id(self) -> Optional[str]:
         """Return this message's thread id."""
         return self.thread and self.thread.thid
 
     def serialize(self) -> dict:
         """Serialize an instance of message to dictionary."""
         return self.dict(exclude_none=True, by_alias=True)
```

### Comparing `acapy-plugin-pickup-0.1.0.post1/acapy_plugin_pickup/protocol/delivery.py` & `acapy_plugin_pickup-0.2.0/acapy_plugin_pickup/v2_0/delivery.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,17 +58,15 @@
             session = self.determine_session(manager, key)
             if session is None:
                 LOGGER.warning("No session available to deliver messages as requested")
                 return
 
             returned_count = 0
             async with context.session() as profile_session:
-
                 for msg in get_messages_for_key(queue, key):
-
                     recipient_key = (
                         msg.target_list[0].recipient_keys
                         or context.message_receipt.recipient_verkey
                     )
                     routing_keys = msg.target_list[0].routing_keys or []
                     sender_key = msg.target_list[0].sender_key or key
 
@@ -93,21 +91,19 @@
                     message_attachments.append(attached_msg)
                     returned_count += 1
 
                     if returned_count >= self.limit:
                         break
 
             response = Delivery(message_attachments=message_attachments)
-            response.assign_thread_from(self)
-            await responder.send_reply(response)
-
         else:
             response = Status(recipient_key=self.recipient_key, message_count=0)
-            response.assign_thread_from(self)
-            await responder.send_reply(response)
+
+        response.assign_thread_from(self)
+        await responder.send_reply(response)
 
 
 class Delivery(AgentMessage):
     """Message wrapper for delivering messages to a recipient."""
 
     class Config:
         allow_population_by_field_name = True
@@ -155,15 +151,14 @@
     """
     return remove_message_by_tag_list(queue, recipient_key, {tag})
 
 
 def remove_message_by_tag_list(
     queue: DeliveryQueue, recipient_key: str, tag_list: Set[str]
 ):
-
     # For debugging, logs the contents of each message as it's retrieved from the queue
     for i in queue.queue_by_key[recipient_key]:
         LOGGER.debug("%s", i.msg)
 
     if recipient_key not in queue.queue_by_key:
         return
     LOGGER.debug(
```

### Comparing `acapy-plugin-pickup-0.1.0.post1/acapy_plugin_pickup/protocol/live_mode.py` & `acapy_plugin_pickup-0.2.0/acapy_plugin_pickup/v2_0/live_mode.py`

 * *Files identical despite different names*

### Comparing `acapy-plugin-pickup-0.1.0.post1/acapy_plugin_pickup/protocol/status.py` & `acapy_plugin_pickup-0.2.0/acapy_plugin_pickup/v2_0/status.py`

 * *Files identical despite different names*

### Comparing `acapy-plugin-pickup-0.1.0.post1/pyproject.toml` & `acapy_plugin_pickup-0.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 [tool.poetry]
 name = "acapy-plugin-pickup"
-version = "0.1.0-post1"
+version = "0.2.0"
 description = "Pickup Protocol for ACA-Py"
 authors = ["Daniel Bluhm <dbluhm@pm.me>", "Micah Peltier <micah6_8@yahoo.com>", "Peter Strobel <peter@indicio.tech>"]
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
-python = ">=3.6.9,<4.0"
-aries-cloudagent = { version = "^0.7.3" }
+python = ">=3.8,<4.0"
+aries-cloudagent = { version = "0.8.2", extras = ["askar", "bbs", "indy"] }
 pydantic = "^1.8.1"
 typing-extensions = "^3.7.4"
 python-dateutil = "^2.8.1"
 
-# ACA-Py Optionals
-python3-indy = { version = ">=1.11.1<2", optional = true }
-
 [tool.poetry.dev-dependencies]
 pre-commit = "^2.12.0"
 black = "^22.6.0"
 flake8 = "^5.0.4"
 pytest = "^6.2.3"
 pytest-asyncio = "^0.14.0"
 
-[tool.poetry.extras]
-indy = ["python3-indy"]
-
 [build-system]
-requires = ["setuptools", "poetry-core>=1.0.0"]
+requires = ["setuptools", "poetry-core>=1.1.5"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `acapy-plugin-pickup-0.1.0.post1/PKG-INFO` & `acapy_plugin_pickup-0.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: acapy-plugin-pickup
-Version: 0.1.0.post1
+Version: 0.2.0
 Summary: Pickup Protocol for ACA-Py
 License: Apache-2.0
 Author: Daniel Bluhm
 Author-email: dbluhm@pm.me
-Requires-Python: >=3.6.9,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Provides-Extra: indy
-Requires-Dist: aries-cloudagent (>=0.7.3,<0.8.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aries-cloudagent[askar,bbs,indy] (==0.8.2)
 Requires-Dist: pydantic (>=1.8.1,<2.0.0)
 Requires-Dist: python-dateutil (>=2.8.1,<3.0.0)
-Requires-Dist: python3-indy (>=1.11.1); extra == "indy"
 Requires-Dist: typing-extensions (>=3.7.4,<4.0.0)
```

