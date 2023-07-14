# Comparing `tmp/rabbitmq-utils-1.2.1.tar.gz` & `tmp/rabbitmq-utils-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rabbitmq-utils-1.2.1.tar", last modified: Fri Jul 14 08:01:55 2023, max compression
+gzip compressed data, was "rabbitmq-utils-1.3.0.tar", last modified: Fri Jul 14 11:59:01 2023, max compression
```

## Comparing `rabbitmq-utils-1.2.1.tar` & `rabbitmq-utils-1.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-14 08:01:55.955950 rabbitmq-utils-1.2.1/
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     6289 2023-07-14 08:01:55.955950 rabbitmq-utils-1.2.1/PKG-INFO
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     5438 2023-07-14 08:01:52.000000 rabbitmq-utils-1.2.1/README.md
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-14 08:01:55.951949 rabbitmq-utils-1.2.1/rabbitmq_utils/
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      128 2023-07-14 08:01:52.000000 rabbitmq-utils-1.2.1/rabbitmq_utils/__init__.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     3423 2023-07-14 08:01:52.000000 rabbitmq-utils-1.2.1/rabbitmq_utils/consumer.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     3552 2023-07-14 08:01:52.000000 rabbitmq-utils-1.2.1/rabbitmq_utils/producer.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)       12 2023-07-14 08:01:52.000000 rabbitmq-utils-1.2.1/rabbitmq_utils/requirements.txt
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-14 08:01:55.955950 rabbitmq-utils-1.2.1/rabbitmq_utils/rpc/
--rw-rw-r--   0 sigma     (1000) sigma     (1000)       59 2023-07-14 08:01:52.000000 rabbitmq-utils-1.2.1/rabbitmq_utils/rpc/__init__.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     3371 2023-07-14 08:01:52.000000 rabbitmq-utils-1.2.1/rabbitmq_utils/rpc/client.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     1876 2023-07-14 08:01:52.000000 rabbitmq-utils-1.2.1/rabbitmq_utils/rpc/server.py
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-14 08:01:55.955950 rabbitmq-utils-1.2.1/rabbitmq_utils.egg-info/
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     6289 2023-07-14 08:01:55.000000 rabbitmq-utils-1.2.1/rabbitmq_utils.egg-info/PKG-INFO
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      409 2023-07-14 08:01:55.000000 rabbitmq-utils-1.2.1/rabbitmq_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 sigma     (1000) sigma     (1000)        1 2023-07-14 08:01:55.000000 rabbitmq-utils-1.2.1/rabbitmq_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 sigma     (1000) sigma     (1000)       12 2023-07-14 08:01:55.000000 rabbitmq-utils-1.2.1/rabbitmq_utils.egg-info/requires.txt
--rw-rw-r--   0 sigma     (1000) sigma     (1000)       25 2023-07-14 08:01:55.000000 rabbitmq-utils-1.2.1/rabbitmq_utils.egg-info/top_level.txt
--rw-rw-r--   0 sigma     (1000) sigma     (1000)       38 2023-07-14 08:01:55.955950 rabbitmq-utils-1.2.1/setup.cfg
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     2068 2023-06-21 09:46:18.000000 rabbitmq-utils-1.2.1/setup.py
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-14 11:59:01.713063 rabbitmq-utils-1.3.0/
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     6561 2023-07-14 11:59:01.713063 rabbitmq-utils-1.3.0/PKG-INFO
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     5710 2023-07-14 11:58:58.000000 rabbitmq-utils-1.3.0/README.md
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-14 11:59:01.709063 rabbitmq-utils-1.3.0/rabbitmq_utils/
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      128 2023-07-14 11:58:58.000000 rabbitmq-utils-1.3.0/rabbitmq_utils/__init__.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     3423 2023-07-14 11:58:58.000000 rabbitmq-utils-1.3.0/rabbitmq_utils/consumer.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     3774 2023-07-14 11:58:58.000000 rabbitmq-utils-1.3.0/rabbitmq_utils/producer.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)       12 2023-07-14 11:58:58.000000 rabbitmq-utils-1.3.0/rabbitmq_utils/requirements.txt
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-14 11:59:01.713063 rabbitmq-utils-1.3.0/rabbitmq_utils/rpc/
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)       59 2023-07-14 11:58:58.000000 rabbitmq-utils-1.3.0/rabbitmq_utils/rpc/__init__.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     3417 2023-07-14 11:58:58.000000 rabbitmq-utils-1.3.0/rabbitmq_utils/rpc/client.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     1876 2023-07-14 11:58:58.000000 rabbitmq-utils-1.3.0/rabbitmq_utils/rpc/server.py
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-14 11:59:01.713063 rabbitmq-utils-1.3.0/rabbitmq_utils.egg-info/
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     6561 2023-07-14 11:59:01.000000 rabbitmq-utils-1.3.0/rabbitmq_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      409 2023-07-14 11:59:01.000000 rabbitmq-utils-1.3.0/rabbitmq_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)        1 2023-07-14 11:59:01.000000 rabbitmq-utils-1.3.0/rabbitmq_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)       12 2023-07-14 11:59:01.000000 rabbitmq-utils-1.3.0/rabbitmq_utils.egg-info/requires.txt
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)       25 2023-07-14 11:59:01.000000 rabbitmq-utils-1.3.0/rabbitmq_utils.egg-info/top_level.txt
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)       38 2023-07-14 11:59:01.713063 rabbitmq-utils-1.3.0/setup.cfg
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     2068 2023-06-21 09:46:18.000000 rabbitmq-utils-1.3.0/setup.py
```

### Comparing `rabbitmq-utils-1.2.1/PKG-INFO` & `rabbitmq-utils-1.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabbitmq-utils
-Version: 1.2.1
+Version: 1.3.0
 Summary: Provide easy connection to rabbitmq server.
 Author: Tahir Rafique
 Author-email: tahirrafiqueasad@gmail.com
 License: MIT
 Keywords: rabbitmq,consumer,producer,publisher,subscriber
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,28 +24,31 @@
 
 ## Producer
 
 Following sample code will allow you to send the message to desire queue. 
 
 In **RabbitMQProducer** class **Publisher Confirms** is implemented, So it will tell you weather the message is send to desire location or not.
 
-**Note: In order to use default exchange, use '' as exchange name. When using the default exchange then routing key will be the name of queue.**
+**Note: In order to use default exchange, use "" as exchange name. When using the default exchange then routing key will be the name of queue.**
+
+In order to make message persistent use **persistent_message=True**. This will increase the disk size as well as latency. The message will be recovered even after the rabbitmq server is restarted. 
 
 ```python
 from rabbitmq_utils import RabbitMQProducer
 import json
 
 # DEFINING MESSAGE
 message = json.dumps({'hello': 'world'})
 
 # SENDING
 rmqp = RabbitMQProducer(
     host='localhost', port=5672, virtual_host='/', 
     username='guest', password='guest', 
-    exchange='test_exc', exchange_type='topic'
+    exchange='test_exc', exchange_type='topic',
+    persistent_message=False
 )
 is_sent = rmqp.sendMessage(
     message,
     routing_key='test_key'
 )
 
 # RESULT
@@ -83,15 +86,15 @@
 
 # STARTING RABBITMQ CONSUMER
 rmqc = RabbitMQConsumer(
         host='localhost', port=5672, virtual_host='/', 
         username='guest', password='guest', 
         queue_name='test_que', routing_key='test_key',
     	exchange='test_exc', exchange_type='topic',
-    	my_callback_function
+    	callback_fun=my_callback_function
 )
 rmqc.receiveMessage()
 ```
 
 ## Remote Procedure Call (RPC)
 
 RPC allow to run a function on a remote computer and wait for the result. It is a synchronous call. This package provide simplest implementation of RPC.
@@ -150,15 +153,16 @@
 message = json.dumps({'hello': 'world'})
 
 # SENDING
 client = RPCClient(
     host='localhost', port=5672, virtual_host='/', 
     username='guest', password='guest', 
     exchange='test_exc', exchange_type='topic',
-    timeout=3 # wait 3 seconds for response. default is None (infinite wait).
+    timeout=3, # wait 3 seconds for response. default is None (infinite wait).
+    persistent_message=False
 )
 is_sent, response = client.sendMessage(
     message,
     routing_key='test_key',
     return_response=True
 )
```

### Comparing `rabbitmq-utils-1.2.1/README.md` & `rabbitmq-utils-1.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -3,28 +3,31 @@
 
 ## Producer
 
 Following sample code will allow you to send the message to desire queue. 
 
 In **RabbitMQProducer** class **Publisher Confirms** is implemented, So it will tell you weather the message is send to desire location or not.
 
-**Note: In order to use default exchange, use '' as exchange name. When using the default exchange then routing key will be the name of queue.**
+**Note: In order to use default exchange, use "" as exchange name. When using the default exchange then routing key will be the name of queue.**
+
+In order to make message persistent use **persistent_message=True**. This will increase the disk size as well as latency. The message will be recovered even after the rabbitmq server is restarted. 
 
 ```python
 from rabbitmq_utils import RabbitMQProducer
 import json
 
 # DEFINING MESSAGE
 message = json.dumps({'hello': 'world'})
 
 # SENDING
 rmqp = RabbitMQProducer(
     host='localhost', port=5672, virtual_host='/', 
     username='guest', password='guest', 
-    exchange='test_exc', exchange_type='topic'
+    exchange='test_exc', exchange_type='topic',
+    persistent_message=False
 )
 is_sent = rmqp.sendMessage(
     message,
     routing_key='test_key'
 )
 
 # RESULT
@@ -62,15 +65,15 @@
 
 # STARTING RABBITMQ CONSUMER
 rmqc = RabbitMQConsumer(
         host='localhost', port=5672, virtual_host='/', 
         username='guest', password='guest', 
         queue_name='test_que', routing_key='test_key',
     	exchange='test_exc', exchange_type='topic',
-    	my_callback_function
+    	callback_fun=my_callback_function
 )
 rmqc.receiveMessage()
 ```
 
 ## Remote Procedure Call (RPC)
 
 RPC allow to run a function on a remote computer and wait for the result. It is a synchronous call. This package provide simplest implementation of RPC.
@@ -129,15 +132,16 @@
 message = json.dumps({'hello': 'world'})
 
 # SENDING
 client = RPCClient(
     host='localhost', port=5672, virtual_host='/', 
     username='guest', password='guest', 
     exchange='test_exc', exchange_type='topic',
-    timeout=3 # wait 3 seconds for response. default is None (infinite wait).
+    timeout=3, # wait 3 seconds for response. default is None (infinite wait).
+    persistent_message=False
 )
 is_sent, response = client.sendMessage(
     message,
     routing_key='test_key',
     return_response=True
 )
```

### Comparing `rabbitmq-utils-1.2.1/rabbitmq_utils/consumer.py` & `rabbitmq-utils-1.3.0/rabbitmq_utils/consumer.py`

 * *Files identical despite different names*

### Comparing `rabbitmq-utils-1.2.1/rabbitmq_utils/producer.py` & `rabbitmq-utils-1.3.0/rabbitmq_utils/producer.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 Project:	 rabbitmq-utils
 Description: Provide function to send the message to rabbitmq exchange.
 """
 
 import pika
 
 class RabbitMQProducer():
-    def __init__(self, host, port, virtual_host, username, password, exchange='', exchange_type='topic') -> None:
+    def __init__(self, host, port, virtual_host, username, password, exchange='', exchange_type='topic', persistent_message=False) -> None:
         """Constructor."""
         self.host = host
         self.port = port
         self.virtual_host = virtual_host
         self.username = username
         self.password = password
         self.exchange = exchange
         self.exchange_type = exchange_type
         
         # STATE VARIABLES
         self.channel = None
         self.connection = None
         self._isSent = None
+        
+        # DELIVERTY MODE
+        if persistent_message:
+            self._delivery_mode = pika.DeliveryMode.Persistent
+        else:
+            self._delivery_mode = pika.DeliveryMode.Transient
         return None
     
     def isSent(self):
         """Getting send status."""
         return self._isSent
     
     def setSentStatus(self, status):
@@ -70,15 +76,15 @@
             channel.basic_publish(
                 exchange=self.exchange,
                 routing_key=routing_key,
                 body=message,
                 mandatory=True,
                 properties=pika.BasicProperties(
                     content_type='text/plain',
-                    delivery_mode=pika.DeliveryMode.Transient,
+                    delivery_mode=self._delivery_mode,
                     **kwargs
                 )
             )
             is_sent = True
         except pika.exceptions.UnroutableError:
             is_sent = False
```

### Comparing `rabbitmq-utils-1.2.1/rabbitmq_utils/rpc/client.py` & `rabbitmq-utils-1.3.0/rabbitmq_utils/rpc/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 import uuid
 
 from rabbitmq_utils import RabbitMQProducer
 
 
 class RPCClient(RabbitMQProducer):
     """RPC Client Class."""
-    def __init__(self, host, port, virtual_host, username, password, exchange, exchange_type='topic', timeout=None) -> None:
-        super().__init__(host, port, virtual_host, username, password, exchange, exchange_type)
+    def __init__(self, host, port, virtual_host, username, password, exchange, exchange_type='topic', timeout=None, persistent_message=False) -> None:
+        super().__init__(host, port, virtual_host, username, password, exchange, exchange_type, persistent_message)
         
         self.timeout = timeout
         
         self.channel = self.getChannel()
         result = self.channel.queue_declare(queue='', exclusive=True)
         self.callback_queue = result.method.queue
```

### Comparing `rabbitmq-utils-1.2.1/rabbitmq_utils/rpc/server.py` & `rabbitmq-utils-1.3.0/rabbitmq_utils/rpc/server.py`

 * *Files identical despite different names*

### Comparing `rabbitmq-utils-1.2.1/rabbitmq_utils.egg-info/PKG-INFO` & `rabbitmq-utils-1.3.0/rabbitmq_utils.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabbitmq-utils
-Version: 1.2.1
+Version: 1.3.0
 Summary: Provide easy connection to rabbitmq server.
 Author: Tahir Rafique
 Author-email: tahirrafiqueasad@gmail.com
 License: MIT
 Keywords: rabbitmq,consumer,producer,publisher,subscriber
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,28 +24,31 @@
 
 ## Producer
 
 Following sample code will allow you to send the message to desire queue. 
 
 In **RabbitMQProducer** class **Publisher Confirms** is implemented, So it will tell you weather the message is send to desire location or not.
 
-**Note: In order to use default exchange, use '' as exchange name. When using the default exchange then routing key will be the name of queue.**
+**Note: In order to use default exchange, use "" as exchange name. When using the default exchange then routing key will be the name of queue.**
+
+In order to make message persistent use **persistent_message=True**. This will increase the disk size as well as latency. The message will be recovered even after the rabbitmq server is restarted. 
 
 ```python
 from rabbitmq_utils import RabbitMQProducer
 import json
 
 # DEFINING MESSAGE
 message = json.dumps({'hello': 'world'})
 
 # SENDING
 rmqp = RabbitMQProducer(
     host='localhost', port=5672, virtual_host='/', 
     username='guest', password='guest', 
-    exchange='test_exc', exchange_type='topic'
+    exchange='test_exc', exchange_type='topic',
+    persistent_message=False
 )
 is_sent = rmqp.sendMessage(
     message,
     routing_key='test_key'
 )
 
 # RESULT
@@ -83,15 +86,15 @@
 
 # STARTING RABBITMQ CONSUMER
 rmqc = RabbitMQConsumer(
         host='localhost', port=5672, virtual_host='/', 
         username='guest', password='guest', 
         queue_name='test_que', routing_key='test_key',
     	exchange='test_exc', exchange_type='topic',
-    	my_callback_function
+    	callback_fun=my_callback_function
 )
 rmqc.receiveMessage()
 ```
 
 ## Remote Procedure Call (RPC)
 
 RPC allow to run a function on a remote computer and wait for the result. It is a synchronous call. This package provide simplest implementation of RPC.
@@ -150,15 +153,16 @@
 message = json.dumps({'hello': 'world'})
 
 # SENDING
 client = RPCClient(
     host='localhost', port=5672, virtual_host='/', 
     username='guest', password='guest', 
     exchange='test_exc', exchange_type='topic',
-    timeout=3 # wait 3 seconds for response. default is None (infinite wait).
+    timeout=3, # wait 3 seconds for response. default is None (infinite wait).
+    persistent_message=False
 )
 is_sent, response = client.sendMessage(
     message,
     routing_key='test_key',
     return_response=True
 )
```

### Comparing `rabbitmq-utils-1.2.1/setup.py` & `rabbitmq-utils-1.3.0/setup.py`

 * *Files identical despite different names*

