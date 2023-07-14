# Comparing `tmp/rabbitmq-utils-1.2.0.tar.gz` & `tmp/rabbitmq-utils-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rabbitmq-utils-1.2.0.tar", last modified: Wed Jun 21 09:51:26 2023, max compression
+gzip compressed data, was "rabbitmq-utils-1.2.1.tar", last modified: Fri Jul 14 08:01:55 2023, max compression
```

## Comparing `rabbitmq-utils-1.2.0.tar` & `rabbitmq-utils-1.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-06-21 09:51:26.275294 rabbitmq-utils-1.2.0/
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     6216 2023-06-21 09:51:26.271294 rabbitmq-utils-1.2.0/PKG-INFO
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     5365 2023-06-21 09:51:22.000000 rabbitmq-utils-1.2.0/README.md
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-06-21 09:51:26.271294 rabbitmq-utils-1.2.0/rabbitmq_utils/
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      128 2023-06-21 09:51:22.000000 rabbitmq-utils-1.2.0/rabbitmq_utils/__init__.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     3423 2023-06-21 09:51:22.000000 rabbitmq-utils-1.2.0/rabbitmq_utils/consumer.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     3552 2023-06-21 09:51:22.000000 rabbitmq-utils-1.2.0/rabbitmq_utils/producer.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)       12 2023-06-21 09:51:22.000000 rabbitmq-utils-1.2.0/rabbitmq_utils/requirements.txt
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-06-21 09:51:26.271294 rabbitmq-utils-1.2.0/rabbitmq_utils/rpc/
--rw-rw-r--   0 sigma     (1000) sigma     (1000)       59 2023-06-21 09:51:22.000000 rabbitmq-utils-1.2.0/rabbitmq_utils/rpc/__init__.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     3371 2023-06-21 09:51:22.000000 rabbitmq-utils-1.2.0/rabbitmq_utils/rpc/client.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     1876 2023-06-21 09:51:22.000000 rabbitmq-utils-1.2.0/rabbitmq_utils/rpc/server.py
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-06-21 09:51:26.271294 rabbitmq-utils-1.2.0/rabbitmq_utils.egg-info/
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     6216 2023-06-21 09:51:26.000000 rabbitmq-utils-1.2.0/rabbitmq_utils.egg-info/PKG-INFO
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      409 2023-06-21 09:51:26.000000 rabbitmq-utils-1.2.0/rabbitmq_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 sigma     (1000) sigma     (1000)        1 2023-06-21 09:51:26.000000 rabbitmq-utils-1.2.0/rabbitmq_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 sigma     (1000) sigma     (1000)       12 2023-06-21 09:51:26.000000 rabbitmq-utils-1.2.0/rabbitmq_utils.egg-info/requires.txt
--rw-rw-r--   0 sigma     (1000) sigma     (1000)       25 2023-06-21 09:51:26.000000 rabbitmq-utils-1.2.0/rabbitmq_utils.egg-info/top_level.txt
--rw-rw-r--   0 sigma     (1000) sigma     (1000)       38 2023-06-21 09:51:26.275294 rabbitmq-utils-1.2.0/setup.cfg
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     2068 2023-06-21 09:46:18.000000 rabbitmq-utils-1.2.0/setup.py
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-14 08:01:55.955950 rabbitmq-utils-1.2.1/
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     6289 2023-07-14 08:01:55.955950 rabbitmq-utils-1.2.1/PKG-INFO
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     5438 2023-07-14 08:01:52.000000 rabbitmq-utils-1.2.1/README.md
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-14 08:01:55.951949 rabbitmq-utils-1.2.1/rabbitmq_utils/
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      128 2023-07-14 08:01:52.000000 rabbitmq-utils-1.2.1/rabbitmq_utils/__init__.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     3423 2023-07-14 08:01:52.000000 rabbitmq-utils-1.2.1/rabbitmq_utils/consumer.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     3552 2023-07-14 08:01:52.000000 rabbitmq-utils-1.2.1/rabbitmq_utils/producer.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)       12 2023-07-14 08:01:52.000000 rabbitmq-utils-1.2.1/rabbitmq_utils/requirements.txt
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-14 08:01:55.955950 rabbitmq-utils-1.2.1/rabbitmq_utils/rpc/
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)       59 2023-07-14 08:01:52.000000 rabbitmq-utils-1.2.1/rabbitmq_utils/rpc/__init__.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     3371 2023-07-14 08:01:52.000000 rabbitmq-utils-1.2.1/rabbitmq_utils/rpc/client.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     1876 2023-07-14 08:01:52.000000 rabbitmq-utils-1.2.1/rabbitmq_utils/rpc/server.py
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-14 08:01:55.955950 rabbitmq-utils-1.2.1/rabbitmq_utils.egg-info/
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     6289 2023-07-14 08:01:55.000000 rabbitmq-utils-1.2.1/rabbitmq_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      409 2023-07-14 08:01:55.000000 rabbitmq-utils-1.2.1/rabbitmq_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)        1 2023-07-14 08:01:55.000000 rabbitmq-utils-1.2.1/rabbitmq_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)       12 2023-07-14 08:01:55.000000 rabbitmq-utils-1.2.1/rabbitmq_utils.egg-info/requires.txt
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)       25 2023-07-14 08:01:55.000000 rabbitmq-utils-1.2.1/rabbitmq_utils.egg-info/top_level.txt
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)       38 2023-07-14 08:01:55.955950 rabbitmq-utils-1.2.1/setup.cfg
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     2068 2023-06-21 09:46:18.000000 rabbitmq-utils-1.2.1/setup.py
```

### Comparing `rabbitmq-utils-1.2.0/PKG-INFO` & `rabbitmq-utils-1.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabbitmq-utils
-Version: 1.2.0
+Version: 1.2.1
 Summary: Provide easy connection to rabbitmq server.
 Author: Tahir Rafique
 Author-email: tahirrafiqueasad@gmail.com
 License: MIT
 Keywords: rabbitmq,consumer,producer,publisher,subscriber
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Development Status :: 5 - Production/Stable
@@ -37,15 +37,15 @@
 # DEFINING MESSAGE
 message = json.dumps({'hello': 'world'})
 
 # SENDING
 rmqp = RabbitMQProducer(
     host='localhost', port=5672, virtual_host='/', 
     username='guest', password='guest', 
-    exchange='test_exc', exchane_type='topic'
+    exchange='test_exc', exchange_type='topic'
 )
 is_sent = rmqp.sendMessage(
     message,
     routing_key='test_key'
 )
 
 # RESULT
@@ -82,15 +82,15 @@
 from rabbitmq_utils import RabbitMQConsumer
 
 # STARTING RABBITMQ CONSUMER
 rmqc = RabbitMQConsumer(
         host='localhost', port=5672, virtual_host='/', 
         username='guest', password='guest', 
         queue_name='test_que', routing_key='test_key',
-    	exchange='test_exc', exchane_type='topic',
+    	exchange='test_exc', exchange_type='topic',
     	my_callback_function
 )
 rmqc.receiveMessage()
 ```
 
 ## Remote Procedure Call (RPC)
 
@@ -100,20 +100,20 @@
 
 ### Server
 
 ```python
 from rabbitmq_utils.rpc import RPCServer
 
 # STARTING RPC SERVER
-server = RabbitMQConsumer(
+server = RPCServer(
         host='localhost', port=5672, virtual_host='/', 
         username='guest', password='guest', 
         queue_name='test_que', routing_key='test_key',
-    	exchange='test_exc', exchane_type='topic',
-    	rpc_callback_function
+    	exchange='test_exc', exchange_type='topic',
+    	callback_fun=rpc_callback_function
 )
 server.receiveMessage()
 ```
 
 Callback function of RPC is different from consumer callback function. In this callback we will return the result back to client.
 
 Note: **result** must be string. If it is not then use **json.dumps(**result**)** to convert it to string.
@@ -149,15 +149,15 @@
 # DEFINING MESSAGE
 message = json.dumps({'hello': 'world'})
 
 # SENDING
 client = RPCClient(
     host='localhost', port=5672, virtual_host='/', 
     username='guest', password='guest', 
-    exchange='test_exc', exchane_type='topic',
+    exchange='test_exc', exchange_type='topic',
     timeout=3 # wait 3 seconds for response. default is None (infinite wait).
 )
 is_sent, response = client.sendMessage(
     message,
     routing_key='test_key',
     return_response=True
 )
@@ -199,11 +199,12 @@
 
 **Tahir Rafique**
 
 ## Releases
 
 | Date      | Version | Summary                              |
 | --------- | ------- | ------------------------------------ |
+| 14-Jul-23 | v1.2.1  | Correcting documentation.            |
 | 21-Jun-23 | v1.2.0  | Adding RPC to module.                |
 | 27-Apr-23 | v1.0.1  | Improving default callback function. |
 | 27-Apr-23 | v1.0.0  | Initial build                        |
```

### Comparing `rabbitmq-utils-1.2.0/README.md` & `rabbitmq-utils-1.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # DEFINING MESSAGE
 message = json.dumps({'hello': 'world'})
 
 # SENDING
 rmqp = RabbitMQProducer(
     host='localhost', port=5672, virtual_host='/', 
     username='guest', password='guest', 
-    exchange='test_exc', exchane_type='topic'
+    exchange='test_exc', exchange_type='topic'
 )
 is_sent = rmqp.sendMessage(
     message,
     routing_key='test_key'
 )
 
 # RESULT
@@ -61,15 +61,15 @@
 from rabbitmq_utils import RabbitMQConsumer
 
 # STARTING RABBITMQ CONSUMER
 rmqc = RabbitMQConsumer(
         host='localhost', port=5672, virtual_host='/', 
         username='guest', password='guest', 
         queue_name='test_que', routing_key='test_key',
-    	exchange='test_exc', exchane_type='topic',
+    	exchange='test_exc', exchange_type='topic',
     	my_callback_function
 )
 rmqc.receiveMessage()
 ```
 
 ## Remote Procedure Call (RPC)
 
@@ -79,20 +79,20 @@
 
 ### Server
 
 ```python
 from rabbitmq_utils.rpc import RPCServer
 
 # STARTING RPC SERVER
-server = RabbitMQConsumer(
+server = RPCServer(
         host='localhost', port=5672, virtual_host='/', 
         username='guest', password='guest', 
         queue_name='test_que', routing_key='test_key',
-    	exchange='test_exc', exchane_type='topic',
-    	rpc_callback_function
+    	exchange='test_exc', exchange_type='topic',
+    	callback_fun=rpc_callback_function
 )
 server.receiveMessage()
 ```
 
 Callback function of RPC is different from consumer callback function. In this callback we will return the result back to client.
 
 Note: **result** must be string. If it is not then use **json.dumps(**result**)** to convert it to string.
@@ -128,15 +128,15 @@
 # DEFINING MESSAGE
 message = json.dumps({'hello': 'world'})
 
 # SENDING
 client = RPCClient(
     host='localhost', port=5672, virtual_host='/', 
     username='guest', password='guest', 
-    exchange='test_exc', exchane_type='topic',
+    exchange='test_exc', exchange_type='topic',
     timeout=3 # wait 3 seconds for response. default is None (infinite wait).
 )
 is_sent, response = client.sendMessage(
     message,
     routing_key='test_key',
     return_response=True
 )
@@ -178,11 +178,12 @@
 
 **Tahir Rafique**
 
 ## Releases
 
 | Date      | Version | Summary                              |
 | --------- | ------- | ------------------------------------ |
+| 14-Jul-23 | v1.2.1  | Correcting documentation.            |
 | 21-Jun-23 | v1.2.0  | Adding RPC to module.                |
 | 27-Apr-23 | v1.0.1  | Improving default callback function. |
 | 27-Apr-23 | v1.0.0  | Initial build                        |
```

### Comparing `rabbitmq-utils-1.2.0/rabbitmq_utils/consumer.py` & `rabbitmq-utils-1.2.1/rabbitmq_utils/consumer.py`

 * *Files identical despite different names*

### Comparing `rabbitmq-utils-1.2.0/rabbitmq_utils/producer.py` & `rabbitmq-utils-1.2.1/rabbitmq_utils/producer.py`

 * *Files identical despite different names*

### Comparing `rabbitmq-utils-1.2.0/rabbitmq_utils/rpc/client.py` & `rabbitmq-utils-1.2.1/rabbitmq_utils/rpc/client.py`

 * *Files identical despite different names*

### Comparing `rabbitmq-utils-1.2.0/rabbitmq_utils/rpc/server.py` & `rabbitmq-utils-1.2.1/rabbitmq_utils/rpc/server.py`

 * *Files identical despite different names*

### Comparing `rabbitmq-utils-1.2.0/rabbitmq_utils.egg-info/PKG-INFO` & `rabbitmq-utils-1.2.1/rabbitmq_utils.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabbitmq-utils
-Version: 1.2.0
+Version: 1.2.1
 Summary: Provide easy connection to rabbitmq server.
 Author: Tahir Rafique
 Author-email: tahirrafiqueasad@gmail.com
 License: MIT
 Keywords: rabbitmq,consumer,producer,publisher,subscriber
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Development Status :: 5 - Production/Stable
@@ -37,15 +37,15 @@
 # DEFINING MESSAGE
 message = json.dumps({'hello': 'world'})
 
 # SENDING
 rmqp = RabbitMQProducer(
     host='localhost', port=5672, virtual_host='/', 
     username='guest', password='guest', 
-    exchange='test_exc', exchane_type='topic'
+    exchange='test_exc', exchange_type='topic'
 )
 is_sent = rmqp.sendMessage(
     message,
     routing_key='test_key'
 )
 
 # RESULT
@@ -82,15 +82,15 @@
 from rabbitmq_utils import RabbitMQConsumer
 
 # STARTING RABBITMQ CONSUMER
 rmqc = RabbitMQConsumer(
         host='localhost', port=5672, virtual_host='/', 
         username='guest', password='guest', 
         queue_name='test_que', routing_key='test_key',
-    	exchange='test_exc', exchane_type='topic',
+    	exchange='test_exc', exchange_type='topic',
     	my_callback_function
 )
 rmqc.receiveMessage()
 ```
 
 ## Remote Procedure Call (RPC)
 
@@ -100,20 +100,20 @@
 
 ### Server
 
 ```python
 from rabbitmq_utils.rpc import RPCServer
 
 # STARTING RPC SERVER
-server = RabbitMQConsumer(
+server = RPCServer(
         host='localhost', port=5672, virtual_host='/', 
         username='guest', password='guest', 
         queue_name='test_que', routing_key='test_key',
-    	exchange='test_exc', exchane_type='topic',
-    	rpc_callback_function
+    	exchange='test_exc', exchange_type='topic',
+    	callback_fun=rpc_callback_function
 )
 server.receiveMessage()
 ```
 
 Callback function of RPC is different from consumer callback function. In this callback we will return the result back to client.
 
 Note: **result** must be string. If it is not then use **json.dumps(**result**)** to convert it to string.
@@ -149,15 +149,15 @@
 # DEFINING MESSAGE
 message = json.dumps({'hello': 'world'})
 
 # SENDING
 client = RPCClient(
     host='localhost', port=5672, virtual_host='/', 
     username='guest', password='guest', 
-    exchange='test_exc', exchane_type='topic',
+    exchange='test_exc', exchange_type='topic',
     timeout=3 # wait 3 seconds for response. default is None (infinite wait).
 )
 is_sent, response = client.sendMessage(
     message,
     routing_key='test_key',
     return_response=True
 )
@@ -199,11 +199,12 @@
 
 **Tahir Rafique**
 
 ## Releases
 
 | Date      | Version | Summary                              |
 | --------- | ------- | ------------------------------------ |
+| 14-Jul-23 | v1.2.1  | Correcting documentation.            |
 | 21-Jun-23 | v1.2.0  | Adding RPC to module.                |
 | 27-Apr-23 | v1.0.1  | Improving default callback function. |
 | 27-Apr-23 | v1.0.0  | Initial build                        |
```

### Comparing `rabbitmq-utils-1.2.0/setup.py` & `rabbitmq-utils-1.2.1/setup.py`

 * *Files identical despite different names*

