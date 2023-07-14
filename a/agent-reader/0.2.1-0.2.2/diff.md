# Comparing `tmp/agent_reader-0.2.1.tar.gz` & `tmp/agent_reader-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agent_reader-0.2.1.tar", max compression
+gzip compressed data, was "agent_reader-0.2.2.tar", max compression
```

## Comparing `agent_reader-0.2.1.tar` & `agent_reader-0.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-06-19 09:36:08.930199 agent_reader-0.2.1/LICENSE
--rw-r--r--   0        0        0      462 2023-06-23 12:47:40.304840 agent_reader-0.2.1/README.md
--rw-r--r--   0        0        0       94 2023-07-14 15:58:30.709680 agent_reader-0.2.1/agent_reader/__init__.py
--rw-r--r--   0        0        0      642 2023-06-23 12:29:06.788197 agent_reader-0.2.1/agent_reader/link_type.py
--rw-r--r--   0        0        0     4823 2023-07-14 15:40:32.244340 agent_reader-0.2.1/agent_reader/reader.py
--rw-r--r--   0        0        0      535 2023-07-14 15:59:22.539665 agent_reader-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1186 1970-01-01 00:00:00.000000 agent_reader-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-19 09:36:08.930199 agent_reader-0.2.2/LICENSE
+-rw-r--r--   0        0        0      528 2023-07-14 16:07:50.836312 agent_reader-0.2.2/README.md
+-rw-r--r--   0        0        0       94 2023-07-14 15:58:30.709680 agent_reader-0.2.2/agent_reader/__init__.py
+-rw-r--r--   0        0        0      642 2023-06-23 12:29:06.788197 agent_reader-0.2.2/agent_reader/link_type.py
+-rw-r--r--   0        0        0     4824 2023-07-14 16:05:46.668637 agent_reader-0.2.2/agent_reader/reader.py
+-rw-r--r--   0        0        0      535 2023-07-14 16:06:40.107352 agent_reader-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1252 1970-01-01 00:00:00.000000 agent_reader-0.2.2/PKG-INFO
```

### Comparing `agent_reader-0.2.1/LICENSE` & `agent_reader-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `agent_reader-0.2.1/agent_reader/link_type.py` & `agent_reader-0.2.2/agent_reader/link_type.py`

 * *Files identical despite different names*

### Comparing `agent_reader-0.2.1/agent_reader/reader.py` & `agent_reader-0.2.2/agent_reader/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 from langchain.chains.summarize import load_summarize_chain
 
 from .link_type import LinkType
 
 class ModelType(Enum):
   OPENAI_GPT35 = 1
   OPENAI_GPT4 = 2
-  COHERE_L = 3
+  COHERE_M = 3
   COHERE_XL = 4
 
 def get_model(model_type, api_key, temperature=0):
   if model_type == ModelType.OPENAI_GPT35:
     return ChatOpenAI(openai_api_key=api_key, model="gpt-3.5-turbo", temperature=temperature)
   elif model_type == ModelType.OPENAI_GPT4:
     return ChatOpenAI(openai_api_key=api_key, model="gpt-4", temperature=temperature)
-  elif model_type == ModelType.COHERE_L:
-    return Cohere(cohere_api_key=api_key, model="summarize-large")
+  elif model_type == ModelType.COHERE_M:
+    return Cohere(cohere_api_key=api_key, model="summarize-medium")
   elif model_type == ModelType.COHERE_XL:
     return Cohere(cohere_api_key=api_key, model="summarize-xlarge")
   else:
     raise Exception(f"Unknown model type: {model_type}")
 
 def get_the_page_content(url):
   headers = {
```

### Comparing `agent_reader-0.2.1/pyproject.toml` & `agent_reader-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "agent_reader"
-version = "0.2.1"
+version = "0.2.2"
 description = "Intelligent Reader of various types of media"
 authors = ["Mariya Davydova <mrs.mariya.davydova@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `agent_reader-0.2.1/PKG-INFO` & `agent_reader-0.2.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agent-reader
-Version: 0.2.1
+Version: 0.2.2
 Summary: Intelligent Reader of various types of media
 License: Apache 2.0
 Author: Mariya Davydova
 Author-email: mrs.mariya.davydova@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -14,17 +14,17 @@
 Requires-Dist: cohere (>=4.11.2,<5.0.0)
 Requires-Dist: langchain (>=0.0.216,<0.0.217)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: transformers (>=4.30.2,<5.0.0)
 Description-Content-Type: text/markdown
 
-# Agent Summarizer
+# Agent Reader
 
-Intelligent summarizer for various kinds of media sources: web pages, Twitter threads, etc.
+Intelligent Reader for various kinds of media sources: web pages, Twitter threads, etc.
 
 Early alpha version. Please don't use it for anything serious.
 
 ## Supported media sources
 
 * [x] Web pages
 * [x] GitHub projects
@@ -33,9 +33,13 @@
 * [ ] Twitter threads
 * [ ] Reddit threads
 * [ ] YouTube videos (aspirational; it's beyond text summarization)
 
 ## Installation
 
 ```bash
-pip install summarizer
+pip install agent-reader
 ```
+
+## Usage
+
+Look at the [demo](demo.py) script for the example of usage.
```

