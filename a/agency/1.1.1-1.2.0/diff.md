# Comparing `tmp/agency-1.1.1.tar.gz` & `tmp/agency-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agency-1.1.1.tar", max compression
+gzip compressed data, was "agency-1.2.0.tar", max compression
```

## Comparing `agency-1.1.1.tar` & `agency-1.2.0.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0    35148 2023-07-11 02:07:16.551773 agency-1.1.1/LICENSE
--rw-r--r--   0        0        0     9363 2023-07-11 02:07:16.551773 agency-1.1.1/README.md
--rw-r--r--   0        0        0        0 2023-07-11 02:07:16.551773 agency-1.1.1/agency/__init__.py
--rw-r--r--   0        0        0     9470 2023-07-11 02:07:16.551773 agency-1.1.1/agency/agent.py
--rw-r--r--   0        0        0      802 2023-07-11 02:07:16.551773 agency-1.1.1/agency/schema.py
--rwxr-xr-x   0        0        0     8876 2023-07-11 02:07:16.551773 agency-1.1.1/agency/space.py
--rw-r--r--   0        0        0     3824 2023-07-11 02:07:16.551773 agency-1.1.1/agency/util.py
--rw-r--r--   0        0        0      539 2023-07-11 02:07:18.035794 agency-1.1.1/pyproject.toml
--rw-r--r--   0        0        0    10037 1970-01-01 00:00:00.000000 agency-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-07-14 02:22:38.241824 agency-1.2.0/LICENSE
+-rw-r--r--   0        0        0     9366 2023-07-14 02:22:38.241824 agency-1.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-14 02:22:38.241824 agency-1.2.0/agency/__init__.py
+-rw-r--r--   0        0        0     9516 2023-07-14 02:22:38.241824 agency-1.2.0/agency/agent.py
+-rw-r--r--   0        0        0     6808 2023-07-14 02:22:38.241824 agency-1.2.0/agency/amqp_space.py
+-rw-r--r--   0        0        0     2770 2023-07-14 02:22:38.241824 agency-1.2.0/agency/native_space.py
+-rw-r--r--   0        0        0      802 2023-07-14 02:22:38.241824 agency-1.2.0/agency/schema.py
+-rwxr-xr-x   0        0        0      754 2023-07-14 02:22:38.241824 agency-1.2.0/agency/space.py
+-rw-r--r--   0        0        0     3824 2023-07-14 02:22:38.241824 agency-1.2.0/agency/util.py
+-rw-r--r--   0        0        0      540 2023-07-14 02:22:40.333922 agency-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    10041 1970-01-01 00:00:00.000000 agency-1.2.0/PKG-INFO
```

### Comparing `agency-1.1.1/LICENSE` & `agency-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `agency-1.1.1/README.md` & `agency-1.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Summary
 
 `agency` is a python library that provides a communication and action framework
-for creating AI agent integrated applications.
+for creating AI agent-integrated applications.
 
 The library provides a low-level means for connecting agents, systems, and human
 users by defining actions, callbacks, and access policies that you can use to
 connect, monitor, control, and interact with your agents.
 
 `agency` handles the details of the common messaging system and allows
 discovering and invoking actions across parties, automatically handling things
@@ -166,23 +166,19 @@
 
 ## How does `agency` compare to agent libraries like LangChain?
 
 Though you could entirely create a simple agent using only the primitives in
 `agency` (see [`examples/demo/agents/`](./examples/demo/agents/)), it is not
 intended to be a full-fledged agent toolset like other libraries or tools.
 
-`agency` is focused on the problems surrounding agent/tool/human integration,
-such as communication, observability, and access control. The library strives to
-provide a minimal yet practical foundation for defining and integrating agent
-systems, allowing developers the freedom to experiment with different agent
-solutions as they desire.
-
-More likely, you would use LangChain or other libraries for defining agent
-specific behavior and rely on `agency` to provide the connective layer for
-bringing agents and other systems together.
+`agency` is an application framework focused on the problems surrounding
+agent/tool/human integration, such as communication, observability, and access
+control. The library strives to provide a minimal yet practical foundation for
+defining and integrating agent-based systems, allowing developers the freedom
+to experiment with different agent solutions as they desire.
 
 
 ## What are some known limitations or issues?
 
 * It's a new project, so keep that in mind in terms of
   completeness, but see [the issues
   page](https://github.com/operand/agency/issues) for what is currently planned,
@@ -264,14 +260,18 @@
 An additional space type utilizing python multiprocessing, as another
 parallelism option for single-host systems.
 
 - **Multimodal Support**:
 Image/audio transfer for use with multimodal models or other multimedia
 services.
 
+- **Storage Support**
+Durable session support will be included. Other forms of storage will be
+considered as well though it's not clear yet what that will look like.
+
 - **More Examples**:
 More examples of integrations with popular AI libraries and tools such as
 Langchain and oobabooga.
 
 
 ## Planned Work
```

### Comparing `agency-1.1.1/agency/agent.py` & `agency-1.2.0/agency/agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-from agency import util
-from agency.schema import ActionSchema, MessageSchema
-from colorama import Fore, Style
-from typing import List
 import inspect
 import re
+import threading
+from typing import List
+
+from colorama import Fore, Style
+
+from agency.schema import ActionSchema, MessageSchema
 
 # access keys
 ACCESS = "access"
 ACCESS_PERMITTED = "permitted"
 ACCESS_DENIED = "denied"
 ACCESS_REQUESTED = "requested"
 
@@ -28,14 +30,18 @@
 
     def __init__(self, id: str) -> None:
         if len(id) < 1 or len(id) > 255:
             raise ValueError("id must be between 1 and 255 characters")
         if re.match(r"^amq\.", id):
             raise ValueError("id cannot start with \"amq.\"")
         self.__id: str = id
+        # threading state
+        self._thread_started = threading.Event()
+        self._thread_stopping = threading.Event()
+        self._thread_stopped = threading.Event()
         # set by Space when added
         self._space = None
         # a basic approach to storing messages
         self._message_log: List[MessageSchema] = []
         self.__cached__help = None
 
     def id(self) -> str:
@@ -46,17 +52,15 @@
         """
         return self.__id
 
     def _send(self, action: dict):
         """
         Sends (out) an action
         """
-        action = ActionSchema(**action).dict(by_alias=True)  # validate
-        message = self._space._route(sender=self, action=action)
-        self._message_log.append(message)
+        self._space._route(sender=self, action=action)
 
     def _receive(self, message: dict):
         """
         Receives and processes an incoming message
         """
         message = MessageSchema(**message).dict(by_alias=True)  # validate
         try:
@@ -124,15 +128,15 @@
                         "return_value": return_value,
                       },
                     })
             else:
                 raise PermissionError(
                   f"\"{self.id()}.{message['action']}\" not permitted")
         except Exception as e:
-            error = e # save the error for _after_action
+            error = e  # save the error for _after_action
             raise Exception(e)
         finally:
             self._after_action(message, return_value, error)
 
     def __permitted(self, message: dict) -> bool:
         """
         Checks whether the action represented by the message is allowed
```

### Comparing `agency-1.1.1/agency/schema.py` & `agency-1.2.0/agency/schema.py`

 * *Files identical despite different names*

### Comparing `agency-1.1.1/agency/space.py` & `agency-1.2.0/agency/amqp_space.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,243 +1,186 @@
-from abc import ABC, ABCMeta, abstractmethod
-from agency.agent import Agent
-from agency.schema import MessageSchema
-from typing import List
 import json
 import os
-import pika
-import queue
+import socket
 import threading
 import time
+from dataclasses import dataclass
 
+from amqp import ChannelError
+from kombu import Connection, Exchange, Queue
 
-class Space(ABC, metaclass=ABCMeta):
-    """
-    A Space is responsible for:
-    - managing the connection lifecycle of its agents
-    - routing messages between agents
-    """
-
-    @abstractmethod
-    def add(self, agent: Agent):
-        """
-        Adds an agent to the space allowing it to receive messages
-        """
-
-    @abstractmethod
-    def remove(self, agent: Agent):
-        """
-        Removes an agent from the space preventing it from receiving messages
-        """
-
-    @abstractmethod
-    def _route(self, sender: Agent, action: dict) -> dict:
-        """
-        Routes an action to the appropriate agents on the sender's behalf.
-        Returns the message that was sent.
-        """
+from agency.agent import Agent
+from agency.schema import MessageSchema
+from agency.space import Space
 
 
-class NativeSpace(Space):
+@dataclass
+class AMQPOptions:
     """
-    A Space implementation that uses Python's built-in queue module.
-    Suitable for single-process applications and testing.
+    A class that defines AMQP connection options
     """
-
-    def __init__(self):
-        self.agents: List[Agent] = []
-
-    def add(self, agent: Agent):
-        self.agents.append(agent)
-        # add a thread to process messages
-
-        def _consume_messages():
-            # create queue for agent
-            agent._queue = queue.Queue()
-            agent._space = self
-            agent._connected = threading.Event()
-            agent._connected.set()
-            agent._after_add()
-            while agent._connected.is_set():
-                try:
-                    message_dict = agent._queue.get(block=False)
-                    message = MessageSchema(
-                        **message_dict).dict(by_alias=True)  # validate
-                    if 'to' not in message or message['to'] in [None, ""] or message['to'] == agent.id():
-                        agent._receive(message)
-                except queue.Empty:
-                    pass
-                time.sleep(0.01)  # cooperate
-
-        threading.Thread(target=_consume_messages).start()
-        time.sleep(0.01)  # cooperate
-
-    def remove(self, agent: Agent):
-        agent._before_remove()
-        agent._connected.clear()
-        self.agents.remove(agent)
-        agent._space = None
-
-    def _route(self, sender: Agent, action: dict) -> None:
-        # Define and validate message
-        message = MessageSchema(**{
-          **action,
-          "from": sender.id(),
-        }).dict(by_alias=True)
-
-        broadcast = False
-        if 'to' not in message or message['to'] in [None, ""]:
-            broadcast = True
-
-        recipients = []
-        for agent in self.agents:
-            if broadcast and message['from'] != agent.id() or not broadcast and message['to'] == agent.id():
-                recipients.append(agent)
-
-        if not broadcast and len(recipients) == 0:
-            # route an error back to the sender
-            self._route(sender, {
-                'to': sender.id(),
-                'thoughts': 'An error occurred',
-                'action': 'error',
-                'args': {
-                    'original_message': message,
-                    'error': f"\"{message['to']}\" not found"
-                }
-            })
-        else:
-            # enqueue message for recipients
-            for recipient in recipients:
-                recipient._queue.put(message)
-
-        return message
+    hostname: str = 'localhost'
+    port: int = '5672'
+    username: str = 'guest'
+    password: str = 'guest'
+    virtual_host: str = '/'
+    use_ssl: bool = False
+    heartbeat: float = 60
 
 
 class AMQPSpace(Space):
     """
     A Space that uses AMQP (RabbitMQ) for message delivery
     """
 
     BROADCAST_KEY = "__broadcast__"
 
-    def __init__(self, pika_connection_params: pika.ConnectionParameters = None, exchange: str = "agency"):
-        if pika_connection_params is None:
-            pika_connection_params = self.default_pika_connection_params()
-        self.__connection_params = pika_connection_params
-        self.__exchange = exchange
-        # set up exchange and broadcast queue
-        connection = pika.BlockingConnection(self.__connection_params)
-        init_channel = connection.channel()
-        init_channel.exchange_declare(
-            exchange=self.__exchange, exchange_type='topic')
-        init_channel.queue_declare(queue=self.BROADCAST_KEY, auto_delete=True)
+    def __init__(self, amqp_options: AMQPOptions = None, exchange: str = "agency"):
+        if amqp_options is None:
+            amqp_options = self.default_amqp_options()
+        # map AMQPOptions for kombu
+        self.__kombu_connection_options = {
+            'hostname': amqp_options.hostname,
+            'port': amqp_options.port,
+            'userid': amqp_options.username,
+            'password': amqp_options.password,
+            'virtual_host': amqp_options.virtual_host,
+            'ssl': amqp_options.use_ssl,
+            'heartbeat': amqp_options.heartbeat,
+        }
+        # setup topic exchange
+        self.__topic_exchange = Exchange(exchange, type="topic")
 
     @classmethod
-    def default_pika_connection_params(cls) -> pika.ConnectionParameters:
+    def default_amqp_options(cls) -> AMQPOptions:
         """
-        Returns a default pika connection params object configurable from
-        environment variables
+        Returns a default AMQPOptions object configurable from environment
+        variables.
         """
-        credentials = pika.PlainCredentials(
-            os.environ.get('AMQP_USERNAME', 'guest'),
-            os.environ.get('AMQP_PASSWORD', 'guest'),
-        )
-        return pika.ConnectionParameters(
-            host=os.environ.get('AMQP_HOST', 'localhost'),
-            port=os.environ.get('AMQP_PORT', 5672),
+        return AMQPOptions(
+            hostname=os.environ.get('AMQP_HOST', 'localhost'),
+            port=int(os.environ.get('AMQP_PORT', 5672)),
+            username=os.environ.get('AMQP_USERNAME', 'guest'),
+            password=os.environ.get('AMQP_PASSWORD', 'guest'),
             virtual_host=os.environ.get('AMQP_VHOST', '/'),
-            credentials=credentials,
+            use_ssl=False,
+            heartbeat=60,
         )
 
     def add(self, agent: Agent) -> None:
+        # define callback for incoming messages
+        def _on_message(body, message):
+            message_data = json.loads(body)
+            broadcast = 'to' not in message_data or message_data['to'] in [
+                None, ""]
+            if broadcast and message_data['from'] != agent.id() \
+               or not broadcast and message_data['to'] == agent.id():
+                agent._receive(message_data)
+            message.ack()
+
         def _consume_messages():
-            # create in/out channels for agent
-            out_connection = pika.BlockingConnection(self.__connection_params)
-            agent._out_channel = out_connection.channel()
-            in_connection = pika.BlockingConnection(self.__connection_params)
-            agent._in_channel = in_connection.channel()
-            agent._in_channel.queue_declare(queue=agent.id(), auto_delete=True)
-
-            # bind queue to its routing key and broadcast key
-            agent._in_channel.queue_bind(exchange=self.__exchange,
-                                         queue=agent.id(), routing_key=agent.id())
-            agent._in_channel.queue_bind(exchange=self.__exchange,
-                                         queue=agent.id(), routing_key=self.BROADCAST_KEY)
-
-            # define callback for incoming messages
-            def _on_message(channel, method, properties, body):
-                message = MessageSchema(
-                    **json.loads(body)).dict(by_alias=True)  # validate
-                broadcast = 'to' not in message or message['to'] in [None, ""]
-                if broadcast and message['from'] != agent.id() or not broadcast and message['to'] == agent.id():
-                    agent._receive(message)
-
-            # bind callback to queues
-            agent._in_channel.basic_consume(
-                queue=agent.id(), on_message_callback=_on_message, auto_ack=True)
-            agent._in_channel.basic_consume(
-                queue=self.BROADCAST_KEY, on_message_callback=_on_message, auto_ack=True)
+            with Connection(**self.__kombu_connection_options) as connection:
+                # Create a queue for direct messages
+                direct_queue = Queue(
+                    agent.id(),
+                    exchange=self.__topic_exchange,
+                    routing_key=agent.id(),
+                )
+                direct_queue(connection.channel()).declare()
+
+                # Create a separate broadcast queue for each agent and bind it to the broadcast key
+                broadcast_queue = Queue(
+                    f"{agent.id()}_broadcast",
+                    exchange=self.__topic_exchange,
+                    routing_key=self.BROADCAST_KEY,
+                )
+                broadcast_queue(connection.channel()).declare()
+
+                # Consume messages from both direct and broadcast queues
+                with connection.Consumer(
+                    [direct_queue, broadcast_queue],
+                    callbacks=[_on_message],
+                ):
+                    agent._space = self
+                    agent._thread_started.set()
+                    while not agent._thread_stopping.is_set():
+                        time.sleep(0.01)
+                        connection.heartbeat_check()  # sends heartbeat if necessary
+                        try:
+                            connection.drain_events(timeout=0.01)
+                        except socket.timeout:
+                            pass
 
-            # start consuming messages
-            agent._space = self
-            agent._after_add()
-            agent._in_channel.start_consuming()
+            agent._thread_stopped.set()
 
+        # start thread
         threading.Thread(target=_consume_messages).start()
-        time.sleep(0.01)  # cooperate
+        if not agent._thread_started.wait(timeout=5):
+            raise Exception(
+                f"Agent {agent.id()} could not be added. Thread timeout.")
+        else:
+            agent._after_add()
 
     def remove(self, agent: Agent) -> None:
         agent._before_remove()
-
-        agent._in_channel.connection.add_callback_threadsafe(
-            agent._in_channel.connection.close)
-        agent._out_channel.connection.add_callback_threadsafe(
-            agent._out_channel.connection.close)
-
-        agent._in_channel = None
-        agent._out_channel = None
+        agent._thread_stopping.set()
+        agent._thread_stopped.wait()
         agent._space = None
 
     def _route(self, sender: Agent, action: dict) -> dict:
         # Define and validate message
         message = MessageSchema(**{
           **action,
           "from": sender.id(),
         }).dict(by_alias=True)
 
-        routing_key = self.BROADCAST_KEY  # broadcast
         if 'to' in message and message['to'] not in [None, ""]:
-            routing_key = message['to']  # point to point
-            # route an error back to sender if point to point and the queue is not found
-            if not self.__check_queue_exists(sender, routing_key):
-                self._route(sender, {
+            # point to point
+            routing_key = message['to']
+        else:
+            # broadcast
+            routing_key = self.BROADCAST_KEY
+
+        sender._message_log.append(message)
+        if routing_key == self.BROADCAST_KEY or self.__check_queue_exists(routing_key):
+            self.__publish(routing_key, message)
+        else:
+            if routing_key == sender.id():
+                # if the routing key equals the sender id, we have a problem.
+                # the sender's own queue doesn't exist so we can't route an
+                # error back. raise an exception to prevent an infinite loop.
+                raise Exception("Cannot route error. Missing sender queue.")
+            else:
+                # send an error back
+                error_message = {
+                    'from': sender.id(),
                     'to': sender.id(),
                     'thoughts': 'An error occurred',
                     'action': 'error',
                     'args': {
                         'original_message': message,
-                        'error': f"\"{message['to']}\" not found"
+                        'error': f"\"{message['to']}\" not found",
                     }
-                })
-                return message
-        body = json.dumps(message)
-        sender._out_channel.basic_publish(
-            exchange=self.__exchange, routing_key=routing_key, body=body)
-        return message
+                }
+                self.__publish(sender.id(), error_message)
 
-    def __check_queue_exists(self, agent: Agent, queue_name: str) -> bool:
-        """
-        Returns true if the queue exists, false otherwise
-        """
-        connection = pika.BlockingConnection(self.__connection_params)
-        channel = connection.channel()
-        try:
-            channel.queue_declare(queue=queue_name, passive=True)
-            return True
-        except pika.exceptions.ChannelClosedByBroker as e:
-            if e.reply_code == 404:
+    def __publish(self, routing_key: str, message: dict):
+        with Connection(**self.__kombu_connection_options) as connection:
+            with connection.Producer(serializer="json") as producer:
+                producer.publish(
+                    json.dumps(message),
+                    exchange=self.__topic_exchange,
+                    routing_key=routing_key,
+                )
+
+    def __check_queue_exists(self, queue_name):
+        with Connection(**self.__kombu_connection_options) as connection:
+            try:
+                with connection.channel() as channel:
+                    channel.queue_bind(
+                        queue=queue_name,
+                        exchange=self.__topic_exchange.name,
+                        routing_key=queue_name,
+                    )
+                return True
+            except ChannelError:
                 return False
-            else:
-                raise e
-        finally:
-            connection.close()
-        raise Exception("Should not reach here")
```

### Comparing `agency-1.1.1/agency/util.py` & `agency-1.2.0/agency/util.py`

 * *Files identical despite different names*

### Comparing `agency-1.1.1/pyproject.toml` & `agency-1.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "agency"
-version = "1.1.1"
+version = "1.2.0"
 description = "A fast and minimal actor model framework for building agent-integrated systems"
 authors = ["Daniel Rodriguez"]
 license = "GPL-3.0"
 readme = "README.md"
 include = ["agency/**/*"]
 exclude = ["*"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 asyncio = "^3.4"
 colorama = "^0.4"
 pydantic = "^1.8"
-pika = "^1.3.2"
+kombu = "^5.3.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.2"
 pytest-asyncio = "^0.21.0"
 
 
 [build-system]
```

### Comparing `agency-1.1.1/PKG-INFO` & `agency-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: agency
-Version: 1.1.1
+Version: 1.2.0
 Summary: A fast and minimal actor model framework for building agent-integrated systems
 License: GPL-3.0
 Author: Daniel Rodriguez
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: asyncio (>=3.4,<4.0)
 Requires-Dist: colorama (>=0.4,<0.5)
-Requires-Dist: pika (>=1.3.2,<2.0.0)
+Requires-Dist: kombu (>=5.3.1,<6.0.0)
 Requires-Dist: pydantic (>=1.8,<2.0)
 Description-Content-Type: text/markdown
 
 # Summary
 
 `agency` is a python library that provides a communication and action framework
-for creating AI agent integrated applications.
+for creating AI agent-integrated applications.
 
 The library provides a low-level means for connecting agents, systems, and human
 users by defining actions, callbacks, and access policies that you can use to
 connect, monitor, control, and interact with your agents.
 
 `agency` handles the details of the common messaging system and allows
 discovering and invoking actions across parties, automatically handling things
@@ -184,23 +184,19 @@
 
 ## How does `agency` compare to agent libraries like LangChain?
 
 Though you could entirely create a simple agent using only the primitives in
 `agency` (see [`examples/demo/agents/`](./examples/demo/agents/)), it is not
 intended to be a full-fledged agent toolset like other libraries or tools.
 
-`agency` is focused on the problems surrounding agent/tool/human integration,
-such as communication, observability, and access control. The library strives to
-provide a minimal yet practical foundation for defining and integrating agent
-systems, allowing developers the freedom to experiment with different agent
-solutions as they desire.
-
-More likely, you would use LangChain or other libraries for defining agent
-specific behavior and rely on `agency` to provide the connective layer for
-bringing agents and other systems together.
+`agency` is an application framework focused on the problems surrounding
+agent/tool/human integration, such as communication, observability, and access
+control. The library strives to provide a minimal yet practical foundation for
+defining and integrating agent-based systems, allowing developers the freedom
+to experiment with different agent solutions as they desire.
 
 
 ## What are some known limitations or issues?
 
 * It's a new project, so keep that in mind in terms of
   completeness, but see [the issues
   page](https://github.com/operand/agency/issues) for what is currently planned,
@@ -282,14 +278,18 @@
 An additional space type utilizing python multiprocessing, as another
 parallelism option for single-host systems.
 
 - **Multimodal Support**:
 Image/audio transfer for use with multimodal models or other multimedia
 services.
 
+- **Storage Support**
+Durable session support will be included. Other forms of storage will be
+considered as well though it's not clear yet what that will look like.
+
 - **More Examples**:
 More examples of integrations with popular AI libraries and tools such as
 Langchain and oobabooga.
 
 
 ## Planned Work
```

