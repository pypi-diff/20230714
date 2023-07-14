# Comparing `tmp/chatgpt-klient-0.1.0.tar.gz` & `tmp/chatgpt-klient-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt-klient-0.1.0.tar", last modified: Fri Jul 14 09:27:17 2023, max compression
+gzip compressed data, was "chatgpt-klient-0.1.1.tar", last modified: Fri Jul 14 10:35:12 2023, max compression
```

## Comparing `chatgpt-klient-0.1.0.tar` & `chatgpt-klient-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-07-14 09:27:17.189310 chatgpt-klient-0.1.0/
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       58 2023-07-14 09:27:17.189310 chatgpt-klient-0.1.0/PKG-INFO
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      331 2023-06-01 11:59:51.000000 chatgpt-klient-0.1.0/README.md
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      235 2023-07-14 09:21:31.000000 chatgpt-klient-0.1.0/pyproject.toml
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       38 2023-07-14 09:27:17.189310 chatgpt-klient-0.1.0/setup.cfg
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-07-14 09:27:17.177310 chatgpt-klient-0.1.0/src/
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-07-14 09:27:17.185310 chatgpt-klient-0.1.0/src/chatgpt_klient/
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       71 2023-07-14 09:21:25.000000 chatgpt-klient-0.1.0/src/chatgpt_klient/__init__.py
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     8322 2023-07-14 09:21:43.000000 chatgpt-klient-0.1.0/src/chatgpt_klient/client.py
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     1054 2023-07-14 08:06:02.000000 chatgpt-klient-0.1.0/src/chatgpt_klient/consts.py
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      140 2023-07-14 07:46:22.000000 chatgpt-klient-0.1.0/src/chatgpt_klient/exceptions.py
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      149 2023-07-14 08:09:12.000000 chatgpt-klient-0.1.0/src/chatgpt_klient/utils.py
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-07-14 09:27:17.189310 chatgpt-klient-0.1.0/src/chatgpt_klient.egg-info/
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       58 2023-07-14 09:27:17.000000 chatgpt-klient-0.1.0/src/chatgpt_klient.egg-info/PKG-INFO
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      383 2023-07-14 09:27:17.000000 chatgpt-klient-0.1.0/src/chatgpt_klient.egg-info/SOURCES.txt
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)        1 2023-07-14 09:27:17.000000 chatgpt-klient-0.1.0/src/chatgpt_klient.egg-info/dependency_links.txt
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       48 2023-07-14 09:27:17.000000 chatgpt-klient-0.1.0/src/chatgpt_klient.egg-info/requires.txt
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       15 2023-07-14 09:27:17.000000 chatgpt-klient-0.1.0/src/chatgpt_klient.egg-info/top_level.txt
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-07-14 10:35:12.727649 chatgpt-klient-0.1.1/
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       58 2023-07-14 10:35:12.727649 chatgpt-klient-0.1.1/PKG-INFO
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      331 2023-06-01 11:59:51.000000 chatgpt-klient-0.1.1/README.md
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      235 2023-07-14 10:33:56.000000 chatgpt-klient-0.1.1/pyproject.toml
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       38 2023-07-14 10:35:12.727649 chatgpt-klient-0.1.1/setup.cfg
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-07-14 10:35:12.707649 chatgpt-klient-0.1.1/src/
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-07-14 10:35:12.719649 chatgpt-klient-0.1.1/src/chatgpt_klient/
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       71 2023-07-14 10:33:56.000000 chatgpt-klient-0.1.1/src/chatgpt_klient/__init__.py
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     8330 2023-07-14 10:33:44.000000 chatgpt-klient-0.1.1/src/chatgpt_klient/client.py
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     1054 2023-07-14 08:06:02.000000 chatgpt-klient-0.1.1/src/chatgpt_klient/consts.py
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      140 2023-07-14 07:46:22.000000 chatgpt-klient-0.1.1/src/chatgpt_klient/exceptions.py
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-07-14 10:35:12.727649 chatgpt-klient-0.1.1/src/chatgpt_klient.egg-info/
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       58 2023-07-14 10:35:12.000000 chatgpt-klient-0.1.1/src/chatgpt_klient.egg-info/PKG-INFO
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      355 2023-07-14 10:35:12.000000 chatgpt-klient-0.1.1/src/chatgpt_klient.egg-info/SOURCES.txt
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)        1 2023-07-14 10:35:12.000000 chatgpt-klient-0.1.1/src/chatgpt_klient.egg-info/dependency_links.txt
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       48 2023-07-14 10:35:12.000000 chatgpt-klient-0.1.1/src/chatgpt_klient.egg-info/requires.txt
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       15 2023-07-14 10:35:12.000000 chatgpt-klient-0.1.1/src/chatgpt_klient.egg-info/top_level.txt
```

### Comparing `chatgpt-klient-0.1.0/src/chatgpt_klient/client.py` & `chatgpt-klient-0.1.1/src/chatgpt_klient/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import tiktoken
 import time
 from logutils import get_logger
 from chatgpt_klient.consts import MAX_TOKENS, LEGACY_ENGINES, CHAT_ENGINES
 from chatgpt_klient.exceptions import InvalidAPIKeyError, InvalidModelError, InvalidResponseError
 from rich.console import Console
 
-logger = get_logger("logger")
+logger = get_logger("chatgpt_client")
 console = Console()
 
 
 class ChatGPTPrompt:
     def __init__(self, api_key, engine="gpt-3.5-turbo-16k"):
         self.api_key = api_key
         self.openai = openai
```

### Comparing `chatgpt-klient-0.1.0/src/chatgpt_klient/consts.py` & `chatgpt-klient-0.1.1/src/chatgpt_klient/consts.py`

 * *Files identical despite different names*

