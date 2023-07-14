# Comparing `tmp/pointstorm-1.1.8.tar.gz` & `tmp/pointstorm-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pointstorm-1.1.8.tar", last modified: Sun Jun 25 19:55:44 2023, max compression
+gzip compressed data, was "pointstorm-1.1.9.tar", last modified: Fri Jul 14 02:24:02 2023, max compression
```

## Comparing `pointstorm-1.1.8.tar` & `pointstorm-1.1.9.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-25 19:55:44.886303 pointstorm-1.1.8/
--rw-r--r--   0 tesfa      (501) staff       (20)    11357 2023-04-16 03:52:15.000000 pointstorm-1.1.8/LICENSE
--rw-r--r--   0 tesfa      (501) staff       (20)    13576 2023-06-25 19:55:44.886087 pointstorm-1.1.8/PKG-INFO
--rw-r--r--   0 tesfa      (501) staff       (20)      737 2023-05-20 01:17:30.000000 pointstorm-1.1.8/README.md
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-25 19:55:44.882766 pointstorm-1.1.8/pointstorm/
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 03:52:45.000000 pointstorm-1.1.8/pointstorm/__init__.py
--rw-r--r--   0 tesfa      (501) staff       (20)      363 2023-04-16 22:54:08.000000 pointstorm-1.1.8/pointstorm/config.py
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-25 19:55:44.883790 pointstorm-1.1.8/pointstorm/destinations/
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:51:39.000000 pointstorm-1.1.8/pointstorm/destinations/__init__.py
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-25 19:55:44.884120 pointstorm-1.1.8/pointstorm/embedding/
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:21:31.000000 pointstorm-1.1.8/pointstorm/embedding/__init__.py
--rw-r--r--   0 tesfa      (501) staff       (20)     1213 2023-06-25 19:54:11.000000 pointstorm-1.1.8/pointstorm/embedding/text.py
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-25 19:55:44.884298 pointstorm-1.1.8/pointstorm/examples/
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-06-20 01:56:08.000000 pointstorm-1.1.8/pointstorm/examples/__init__.py
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-25 19:55:44.884752 pointstorm-1.1.8/pointstorm/examples/kafka/
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-06-20 01:56:17.000000 pointstorm-1.1.8/pointstorm/examples/kafka/__init__.py
--rw-r--r--   0 tesfa      (501) staff       (20)      560 2023-06-20 02:30:06.000000 pointstorm-1.1.8/pointstorm/examples/kafka/kafka_producer.py
--rw-r--r--   0 tesfa      (501) staff       (20)      547 2023-06-20 02:22:00.000000 pointstorm-1.1.8/pointstorm/examples/kafka/run_kafka.py
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-25 19:55:44.884947 pointstorm-1.1.8/pointstorm/ingestion/
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-05-20 00:59:06.000000 pointstorm-1.1.8/pointstorm/ingestion/__init__.py
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-25 19:55:44.885212 pointstorm-1.1.8/pointstorm/ingestion/cdc/
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:50:52.000000 pointstorm-1.1.8/pointstorm/ingestion/cdc/__init__.py
--rw-r--r--   0 tesfa      (501) staff       (20)       78 2023-04-30 00:19:04.000000 pointstorm-1.1.8/pointstorm/ingestion/cdc/debezium.py
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-25 19:55:44.885454 pointstorm-1.1.8/pointstorm/ingestion/event/
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:02:57.000000 pointstorm-1.1.8/pointstorm/ingestion/event/__init__.py
--rw-r--r--   0 tesfa      (501) staff       (20)     3776 2023-06-25 19:41:33.000000 pointstorm-1.1.8/pointstorm/ingestion/event/kafka.py
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-25 19:55:44.885632 pointstorm-1.1.8/pointstorm/inputs/
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-06-16 06:13:48.000000 pointstorm-1.1.8/pointstorm/inputs/__init__.py
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 04:50:18.000000 pointstorm-1.1.8/pointstorm/monitoring.py
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-25 19:55:44.885881 pointstorm-1.1.8/pointstorm/producers/
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-06-20 01:44:46.000000 pointstorm-1.1.8/pointstorm/producers/__init__.py
--rw-r--r--   0 tesfa      (501) staff       (20)     1014 2023-06-20 02:17:13.000000 pointstorm-1.1.8/pointstorm/producers/text_producer.py
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-06-25 19:55:44.883552 pointstorm-1.1.8/pointstorm.egg-info/
--rw-r--r--   0 tesfa      (501) staff       (20)    13576 2023-06-25 19:55:44.000000 pointstorm-1.1.8/pointstorm.egg-info/PKG-INFO
--rw-r--r--   0 tesfa      (501) staff       (20)      813 2023-06-25 19:55:44.000000 pointstorm-1.1.8/pointstorm.egg-info/SOURCES.txt
--rw-r--r--   0 tesfa      (501) staff       (20)        1 2023-06-25 19:55:44.000000 pointstorm-1.1.8/pointstorm.egg-info/dependency_links.txt
--rw-r--r--   0 tesfa      (501) staff       (20)      116 2023-06-25 19:55:44.000000 pointstorm-1.1.8/pointstorm.egg-info/requires.txt
--rw-r--r--   0 tesfa      (501) staff       (20)       11 2023-06-25 19:55:44.000000 pointstorm-1.1.8/pointstorm.egg-info/top_level.txt
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:22:49.000000 pointstorm-1.1.8/pyproject.toml
--rw-r--r--   0 tesfa      (501) staff       (20)       38 2023-06-25 19:55:44.886348 pointstorm-1.1.8/setup.cfg
--rw-r--r--   0 tesfa      (501) staff       (20)     1054 2023-06-25 19:54:29.000000 pointstorm-1.1.8/setup.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-07-14 02:24:02.025940 pointstorm-1.1.9/
+-rw-r--r--   0 tesfa      (501) staff       (20)    11357 2023-04-16 03:52:15.000000 pointstorm-1.1.9/LICENSE
+-rw-r--r--   0 tesfa      (501) staff       (20)    13576 2023-07-14 02:24:02.025768 pointstorm-1.1.9/PKG-INFO
+-rw-r--r--   0 tesfa      (501) staff       (20)      824 2023-07-14 02:23:28.000000 pointstorm-1.1.9/README.md
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-07-14 02:24:02.022266 pointstorm-1.1.9/pointstorm/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 03:52:45.000000 pointstorm-1.1.9/pointstorm/__init__.py
+-rw-r--r--   0 tesfa      (501) staff       (20)      363 2023-04-16 22:54:08.000000 pointstorm-1.1.9/pointstorm/config.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-07-14 02:24:02.023092 pointstorm-1.1.9/pointstorm/destinations/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:51:39.000000 pointstorm-1.1.9/pointstorm/destinations/__init__.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-07-14 02:24:02.023566 pointstorm-1.1.9/pointstorm/embedding/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:21:31.000000 pointstorm-1.1.9/pointstorm/embedding/__init__.py
+-rw-r--r--   0 tesfa      (501) staff       (20)     1907 2023-07-14 02:23:28.000000 pointstorm-1.1.9/pointstorm/embedding/text.py
+-rw-r--r--   0 tesfa      (501) staff       (20)     2145 2023-07-14 02:23:28.000000 pointstorm-1.1.9/pointstorm/embedding/text_tests.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-07-14 02:24:02.023742 pointstorm-1.1.9/pointstorm/examples/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-06-20 01:56:08.000000 pointstorm-1.1.9/pointstorm/examples/__init__.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-07-14 02:24:02.024307 pointstorm-1.1.9/pointstorm/examples/kafka/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-06-20 01:56:17.000000 pointstorm-1.1.9/pointstorm/examples/kafka/__init__.py
+-rw-r--r--   0 tesfa      (501) staff       (20)      560 2023-07-14 02:16:25.000000 pointstorm-1.1.9/pointstorm/examples/kafka/kafka_producer.py
+-rw-r--r--   0 tesfa      (501) staff       (20)      547 2023-07-14 02:16:35.000000 pointstorm-1.1.9/pointstorm/examples/kafka/run_kafka.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-07-14 02:24:02.024556 pointstorm-1.1.9/pointstorm/ingestion/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-05-20 00:59:06.000000 pointstorm-1.1.9/pointstorm/ingestion/__init__.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-07-14 02:24:02.024754 pointstorm-1.1.9/pointstorm/ingestion/cdc/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:50:52.000000 pointstorm-1.1.9/pointstorm/ingestion/cdc/__init__.py
+-rw-r--r--   0 tesfa      (501) staff       (20)       78 2023-04-30 00:19:04.000000 pointstorm-1.1.9/pointstorm/ingestion/cdc/debezium.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-07-14 02:24:02.025081 pointstorm-1.1.9/pointstorm/ingestion/event/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:02:57.000000 pointstorm-1.1.9/pointstorm/ingestion/event/__init__.py
+-rw-r--r--   0 tesfa      (501) staff       (20)     2481 2023-07-14 02:23:28.000000 pointstorm-1.1.9/pointstorm/ingestion/event/kafka.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-07-14 02:24:02.025213 pointstorm-1.1.9/pointstorm/inputs/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-06-16 06:13:48.000000 pointstorm-1.1.9/pointstorm/inputs/__init__.py
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 04:50:18.000000 pointstorm-1.1.9/pointstorm/monitoring.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-07-14 02:24:02.025421 pointstorm-1.1.9/pointstorm/producers/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-06-20 01:44:46.000000 pointstorm-1.1.9/pointstorm/producers/__init__.py
+-rw-r--r--   0 tesfa      (501) staff       (20)     1014 2023-06-20 02:17:13.000000 pointstorm-1.1.9/pointstorm/producers/text_producer.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-07-14 02:24:02.022962 pointstorm-1.1.9/pointstorm.egg-info/
+-rw-r--r--   0 tesfa      (501) staff       (20)    13576 2023-07-14 02:24:01.000000 pointstorm-1.1.9/pointstorm.egg-info/PKG-INFO
+-rw-r--r--   0 tesfa      (501) staff       (20)      848 2023-07-14 02:24:01.000000 pointstorm-1.1.9/pointstorm.egg-info/SOURCES.txt
+-rw-r--r--   0 tesfa      (501) staff       (20)        1 2023-07-14 02:24:01.000000 pointstorm-1.1.9/pointstorm.egg-info/dependency_links.txt
+-rw-r--r--   0 tesfa      (501) staff       (20)      130 2023-07-14 02:24:01.000000 pointstorm-1.1.9/pointstorm.egg-info/requires.txt
+-rw-r--r--   0 tesfa      (501) staff       (20)       11 2023-07-14 02:24:01.000000 pointstorm-1.1.9/pointstorm.egg-info/top_level.txt
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:22:49.000000 pointstorm-1.1.9/pyproject.toml
+-rw-r--r--   0 tesfa      (501) staff       (20)       38 2023-07-14 02:24:02.025997 pointstorm-1.1.9/setup.cfg
+-rw-r--r--   0 tesfa      (501) staff       (20)     1090 2023-07-14 02:23:28.000000 pointstorm-1.1.9/setup.py
```

### Comparing `pointstorm-1.1.8/LICENSE` & `pointstorm-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pointstorm-1.1.8/PKG-INFO` & `pointstorm-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pointstorm
-Version: 1.1.8
+Version: 1.1.9
 Summary: Embedding vectors for data on the move
 Home-page: https://github.com/xsfa/pointstorm
 Author: xsfa
 Author-email: tesfaaog@gmail.com
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `pointstorm-1.1.8/README.md` & `pointstorm-1.1.9/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -5,23 +5,27 @@
 ```shell
 pip install pointstorm
 ```
 
 ```py
 from pointstorm.ingestion.event.kafka import KafkaTextEmbeddings
 
-real_time_kafka_embeddings = KafkaTextEmbeddings(
-    kafka_topic="user-tracker",
+kafka_consumer_config = {
+    'group.id': f"kafka_text_vectorizer",
+    'auto.offset.reset': 'largest',
+    'enable.auto.commit': True
+}
+
+kafka_embeddings = KafkaTextEmbeddings(
+    kafka_topic="user-tracker2",
     kafka_bootstrap_server="localhost:9092",
-    kafka_group_id=f"kafka_text_vectorizer_id",
-    text_field="text",
+    kafka_config=kafka_consumer_config,
     huggingface_model_name= "sentence-transformers/paraphrase-MiniLM-L6-v2"
 )
-
-real_time_kafka_embeddings.run()
+kafka_embeddings.run()
 ```
 
 ## Kafka Example Quickstart
 
 ### Prerequisites
 
 - Setup Kafka
```

### Comparing `pointstorm-1.1.8/pointstorm/embedding/text.py` & `pointstorm-1.1.9/pointstorm/embedding/text.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,59 @@
 import hashlib
+from typing import List, Optional
 from pydantic import BaseModel
 from typing import Any, Optional
+from numpy import ndarray
 from transformers import AutoTokenizer, AutoModel
 
 import json
 
 from unstructured.partition.html import partition_html
 from unstructured.cleaners.core import clean, replace_unicode_quotes, clean_non_ascii_chars
 from unstructured.staging.huggingface import chunk_by_attention_window
 from unstructured.staging.huggingface import stage_for_transformers
 
 import hashlib
 from pydantic import BaseModel
 from typing import Any, Optional
 
-tokenizer = AutoTokenizer.from_pretrained("sentence-transformers/all-MiniLM-L6-v2")
-model = AutoModel.from_pretrained("sentence-transformers/all-MiniLM-L6-v2")
-
 class Document(BaseModel):
+    """
+    Document object to be used for generating embeddings.
+    @params:
+        id: Unique identifier for the document.
+        group_key: Group key for the document.
+        metadata: Metadata for the document.
+        text: The text.
+        embeddings: Generated embeddings.
+    """
     id: str
     group_key: Optional[str] = None
     metadata: Optional[dict] = {}
     text: Optional[list]
     embeddings: Optional[list] = []
 
-# create embedding and store in vector db
-def embedding(document):
-    inputs = tokenizer(document.text, padding=True, truncation=True, return_tensors="pt", max_length=384)
-    result = model(**inputs)
-    embeddings = result.last_hidden_state[:, 0, :].cpu().detach().numpy()
-    lst = embeddings.flatten().tolist()
-    document.embeddings.append(lst)
-    return document
+def generate_embedding(document: Document, tokenizer: AutoTokenizer, model: AutoModel) -> Document:
+    """
+    Generate embedding for a given document using a pretrained model.
+    @params: 
+        document: Document for which to generate the embeddings.
+    returns: 
+        Document: Document object with updated embeddings.
+    """
+    try:
+        inputs = tokenizer(
+            document.text,
+            padding=True,
+            truncation=True,
+            return_tensors="pt",
+            max_length=384
+        )
+        result = model(**inputs)
+        embeddings = result.last_hidden_state[:, 0, :].cpu().detach().numpy()
+        flattened_embeddings = embeddings.flatten().tolist()
+        document.embeddings.append(flattened_embeddings)
+
+        return document
+    except Exception as e:
+        print(f"An error occurred: {str(e)}")
+        return None
```

### Comparing `pointstorm-1.1.8/pointstorm/examples/kafka/kafka_producer.py` & `pointstorm-1.1.9/pointstorm/examples/kafka/kafka_producer.py`

 * *Files identical despite different names*

### Comparing `pointstorm-1.1.8/pointstorm/examples/kafka/run_kafka.py` & `pointstorm-1.1.9/pointstorm/examples/kafka/run_kafka.py`

 * *Files identical despite different names*

### Comparing `pointstorm-1.1.8/pointstorm/ingestion/event/kafka.py` & `pointstorm-1.1.9/pointstorm/ingestion/event/kafka.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Generic imports
 import json
 import logging
 import warnings
 import os
+import uuid
 warnings.filterwarnings(action = 'ignore')
 
 # Ingestion Imports
 from bytewax.testing import run_main
 from bytewax.dataflow import Dataflow
 from bytewax.connectors.kafka import KafkaInput
 from bytewax.connectors.stdio import StdOutput
@@ -14,87 +15,58 @@
 
 # ML imports
 from transformers import AutoTokenizer, AutoModel
 import torch
 
 # Local imports
 from pointstorm.config import abstract_logger as kafka_logger
-from pointstorm.embedding.text import Document, embedding
+from pointstorm.embedding.text import Document, generate_embedding
 
 class KafkaIngestionException(Exception):
     pass
 
 class KafkaTextEmbeddings():
     def __init__(self, kafka_topic, kafka_bootstrap_server, kafka_config, huggingface_model_name):
         self.kafka_topic = kafka_topic
         self.kafka_bootstrap_server = kafka_bootstrap_server
         self.kafka_config = kafka_config
         self.model_name = huggingface_model_name
         self.tokenizer = AutoTokenizer.from_pretrained(self.model_name)
         self.model = AutoModel.from_pretrained(self.model_name)
-        # self.previous_messages = self.get_previous_messages()
-
-    #     def set_topic(self, kafka_topic):
-    #         self.kafka_topic = kafka_topic
-
-    # def get_previous_messages(self):
-    #     previous_messages = []
-
-    #     consumer = KafkaConsumer(
-    #         self.kafka_topic,
-    #         bootstrap_servers=self.kafka_bootstrap_server,
-    #         group_id=self.kafka_group_id,
-    #         auto_offset_reset='earliest',
-    #         enable_auto_commit=True,
-    #         value_deserializer=lambda x: x.decode('utf-8')
-    #     )
-
-    #     partitions = consumer.partitions_for_topic(self.kafka_topic)
-    #     topic_partitions = [TopicPartition(self.kafka_topic, p) for p in partitions]
-    #     end_offsets = consumer.end_offsets(topic_partitions)
-
-    #     for message in consumer:
-
-    #         previous_messages.append(json.loads(message.value)[self.text_field]) if self.text_field in json.loads(message.value) else previous_messages.append(json.loads(message.value))
-
-    #         topic_partition = TopicPartition(message.topic, message.partition)
-    #         if message.offset == end_offsets[topic_partition] - 1:
-    #             topic_partitions.remove(topic_partition)
-
-    #             if not topic_partitions:
-    #                 consumer.close()
-    #                 break
-        
-    #     return previous_messages
 
     def set_output(self, output):
         # TODO: Add output
         self.output = output
 
-    def embedding(self, message):
+    def embedding(self, message) -> Document:
         """
         Generating embedding using text embedding class
         """
 
         if "raw_text" in json.loads(message[1]):
             message = str(json.loads(message[1])["raw_text"])
         else:
             raise KafkaIngestionException("Message does not contain the specified text field: " + self.text_field)
         
-        # doc = Document(
-        #     id=
-        #     text=message,
-        #     )
-        inputs = self.tokenizer(message, return_tensors="pt", padding=True, truncation=True)
-
-        with torch.no_grad():
-            outputs = self.model(**inputs)
+        doc = Document(
+            id=str(uuid.uuid4()),
+            group_key="group1",
+            metadata={},
+            text=[message],
+            embeddings=[[]]
+        )
+        
+        doc = generate_embedding(
+            document=doc, 
+            tokenizer=self.tokenizer, 
+            model=self.model
+        )
 
-        embeddings = outputs.last_hidden_state.mean(dim=1).numpy()
-        kafka_logger.info(f"Generated embeddings for message: {message}, {embeddings}")
+        kafka_logger.info(f"Generated embeddings for message: {message} ({doc.id}): {doc.embeddings}")
+        return doc
     
     def run(self):
         input_config = KafkaInput(
             brokers=[self.kafka_bootstrap_server],
             topics=[self.kafka_topic],
             add_config=self.kafka_config
         )
```

### Comparing `pointstorm-1.1.8/pointstorm/producers/text_producer.py` & `pointstorm-1.1.9/pointstorm/producers/text_producer.py`

 * *Files identical despite different names*

### Comparing `pointstorm-1.1.8/pointstorm.egg-info/PKG-INFO` & `pointstorm-1.1.9/pointstorm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pointstorm
-Version: 1.1.8
+Version: 1.1.9
 Summary: Embedding vectors for data on the move
 Home-page: https://github.com/xsfa/pointstorm
 Author: xsfa
 Author-email: tesfaaog@gmail.com
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `pointstorm-1.1.8/pointstorm.egg-info/SOURCES.txt` & `pointstorm-1.1.9/pointstorm.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 pointstorm.egg-info/SOURCES.txt
 pointstorm.egg-info/dependency_links.txt
 pointstorm.egg-info/requires.txt
 pointstorm.egg-info/top_level.txt
 pointstorm/destinations/__init__.py
 pointstorm/embedding/__init__.py
 pointstorm/embedding/text.py
+pointstorm/embedding/text_tests.py
 pointstorm/examples/__init__.py
 pointstorm/examples/kafka/__init__.py
 pointstorm/examples/kafka/kafka_producer.py
 pointstorm/examples/kafka/run_kafka.py
 pointstorm/ingestion/__init__.py
 pointstorm/ingestion/cdc/__init__.py
 pointstorm/ingestion/cdc/debezium.py
```

### Comparing `pointstorm-1.1.8/setup.py` & `pointstorm-1.1.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,14 +18,16 @@
         'kafka-python==2.0.2',
         'confluent-kafka',
         'faker',
         'transformers',
         'torch',
         'pydantic',
         'unstructured'
+        'numpy',
+        'unittest'
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
```

