# Comparing `tmp/catgpt-0.0.4.tar.gz` & `tmp/catgpt-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catgpt-0.0.4.tar", max compression
+gzip compressed data, was "catgpt-0.0.5.tar", max compression
```

## Comparing `catgpt-0.0.4.tar` & `catgpt-0.0.5.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       46 2023-04-29 02:55:42.000000 catgpt-0.0.4/catgpt/__init__.py
--rw-r--r--   0        0        0     4396 2023-05-30 06:39:23.426058 catgpt-0.0.4/catgpt/model.py
--rw-r--r--   0        0        0      404 2023-05-31 06:30:54.371070 catgpt-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 catgpt-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       46 2023-04-29 02:55:42.000000 catgpt-0.0.5/catgpt/__init__.py
+-rw-r--r--   0        0        0     7453 2023-07-14 06:51:11.478843 catgpt-0.0.5/catgpt/model.py
+-rw-r--r--   0        0        0      404 2023-07-14 06:51:56.702494 catgpt-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 catgpt-0.0.5/PKG-INFO
```

### Comparing `catgpt-0.0.4/catgpt/model.py` & `catgpt-0.0.5/catgpt/model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+#!/usr/bin/env python3
 import os
 import json
 import requests
 import json
 import codefast as cf
 import requests
 import sseclient
 import ast
 import time
+import aiohttp
 from typing import Dict, List
 
 
 class ChatDB(cf.osdb):
     def __init__(self, path: str = 'chat.db'):
         super().__init__(path)
 
@@ -126,14 +128,107 @@
     def __call__(self, prompt: str, stream: bool = False) -> str:
         if stream:
             return self.get_stream(prompt)
         else:
             return self.get_response(prompt)
 
 
+
+
+class AsyncGPT(object):
+    def __init__(self, api: str,
+                 token: str,
+                 model: str = 'gpt-3.5-turbo',
+                 openai_key:str = '',
+                 history_path: str = None,
+                 history_length: int = 5,
+                 proxy: dict = None) -> None:
+        """
+        Args:
+            api: api url
+            token: api token
+            openai_key: openai key
+            model: model name
+            history_path: path to save chat history
+            history_length: number of history to show
+            proxy: proxy dict
+        
+        1. if no openai_key is specified, then the server side will use the default openai key
+        2. otherwise, input `openai_key` will be used.
+        """
+        self.api = api
+        self.token = token
+        self.model = model
+        self.history_length = history_length
+        self.openai_key=openai_key
+        if history_path is None:
+            today = time.strftime("%Y-%m-%d", time.localtime())
+            history_path = os.path.join('/tmp', 'chat-' + today + '.txt')
+        self.chatdb = ChatDB(history_path)
+        self.proxy = proxy
+
+    def get_headers(self):
+        return {
+            "Content-Type": "application/json",
+            "token": self.token,
+            "openai_key": self.openai_key
+        }
+
+    def get_history(self, n: int = 5) -> list:
+        if n == 0:
+            return []
+        history = self.chatdb.latest(n)
+        return [h for h in history if h]
+
+    def update_history(self, item: Dict[str, str]) -> None:
+        self.chatdb.save(item)
+
+    async def make_post(self, prompt: str, stream: bool) -> requests.Response:
+        """ Generate a post request to the API
+        """
+        prompt_dict = {"role": "user", "content": prompt}
+        history = self.get_history(self.history_length)
+        data = {
+            "model":  self.model,
+            "messages": history + [prompt_dict],
+            "stream": stream
+        }
+        self.update_history(prompt_dict)
+        async with aiohttp.ClientSession() as session:
+            async with session.post(self.api, json=data, headers=self.get_headers()) as resp:
+                if stream:
+                    return resp
+                else:
+                    return await resp.json()
+
+
+    async def get_stream(self, prompt: str) -> str:
+        raise NotImplementedError
+  
+    async def get_response(self, prompt: str) -> str:
+        response = await self.make_post(prompt, stream=False)
+        try:
+            if response:
+                return response['choices'][0]['message']['content']
+        except Exception:
+            cf.warning({
+                'prompt': prompt,
+                'response': request.text
+            })
+        return 'FOUND NO RESPONSE'
+
+    async def __call__(self, prompt: str, stream: bool = False) -> str:
+        if stream:
+            resp = await self.get_stream(prompt)
+        else:
+            resp= await self.get_response(prompt)
+        return resp
+
+
+
 if __name__ == '__main__':
     import dotenv
     dotenv.load_dotenv()
     api = os.getenv('API')
     token = os.getenv('TOKEN')
     gpt = GPT(api, token)
     print(gpt('Hello, I am a robot.'))
```

### Comparing `catgpt-0.0.4/PKG-INFO` & `catgpt-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catgpt
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple cli tool to generate text using GPT-turbo
 Author: tom
 Author-email: tom@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

