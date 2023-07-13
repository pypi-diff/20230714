# Comparing `tmp/unigui-1.8.0.tar.gz` & `tmp/unigui-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unigui-1.8.0.tar", last modified: Tue Jul 11 21:52:33 2023, max compression
+gzip compressed data, was "dist/unigui-1.8.1.tar", last modified: Thu Jul 13 23:20:16 2023, max compression
```

## Comparing `unigui-1.8.0.tar` & `unigui-1.8.1.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-11 21:52:33.000000 unigui-1.8.0/
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-11 21:52:33.000000 unigui-1.8.0/unigui/
--rw-rw-r--   0 george    (1000) george    (1000)     9132 2023-07-11 20:55:41.000000 unigui-1.8.0/unigui/guielements.py
--rw-rw-r--   0 george    (1000) george    (1000)     3280 2023-07-11 18:46:47.000000 unigui-1.8.0/unigui/server.py
--rw-rw-r--   0 george    (1000) george    (1000)       99 2023-07-11 08:13:29.000000 unigui-1.8.0/unigui/__init__.py
--rw-r--r--   0 george    (1000) george    (1000)     2449 2023-07-11 13:55:58.000000 unigui-1.8.0/unigui/utils.py
--rw-rw-r--   0 george    (1000) george    (1000)     9608 2023-07-11 20:49:39.000000 unigui-1.8.0/unigui/user.py
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-11 21:52:33.000000 unigui-1.8.0/unigui/web/
--rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/favicon.ico
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-11 21:52:33.000000 unigui-1.8.0/unigui/web/css/
--rw-rw-r--   0 george    (1000) george    (1000)        0 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/css/app.31d6cfe0.css
--rw-rw-r--   0 george    (1000) george    (1000)     3267 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/css/223.f0f63b8f.css
--rw-rw-r--   0 george    (1000) george    (1000)   219590 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/css/vendor.49a52e8f.css
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-11 21:52:33.000000 unigui-1.8.0/unigui/web/icons/
--rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/icons/favicon-96x96.png
--rw-rw-r--   0 george    (1000) george    (1000)      859 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/icons/favicon-16x16.png
--rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/icons/favicon-32x32.png
--rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/icons/favicon-128x128.png
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-11 21:52:33.000000 unigui-1.8.0/unigui/web/fonts/
--rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-rw-r--   0 george    (1000) george    (1000)   128360 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
--rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-11 21:52:33.000000 unigui-1.8.0/unigui/web/js/
--rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/js/430.591e9a73.js
--rw-rw-r--   0 george    (1000) george    (1000)    44624 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/js/223.7924e6b0.js
--rw-rw-r--   0 george    (1000) george    (1000)     5868 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/js/app.fc1b2f39.js
--rw-rw-r--   0 george    (1000) george    (1000)      763 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/js/193.283445be.js
--rw-rw-r--   0 george    (1000) george    (1000)  1431597 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/js/vendor.3e8714c2.js
--rw-rw-r--   0 george    (1000) george    (1000)      907 2023-07-11 21:46:03.000000 unigui-1.8.0/unigui/web/index.html
--rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.8.0/LICENSE
--rw-rw-r--   0 george    (1000) george    (1000)      600 2023-07-11 21:47:23.000000 unigui-1.8.0/setup.py
--rw-rw-r--   0 george    (1000) george    (1000)    19080 2023-07-11 21:52:33.000000 unigui-1.8.0/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)       38 2023-07-11 21:52:33.000000 unigui-1.8.0/setup.cfg
--rw-rw-r--   0 george    (1000) george    (1000)    18775 2023-07-11 08:15:37.000000 unigui-1.8.0/README.md
--rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.8.0/MANIFEST.in
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-11 21:52:33.000000 unigui-1.8.0/unigui.egg-info/
--rw-rw-r--   0 george    (1000) george    (1000)       30 2023-07-11 21:52:33.000000 unigui-1.8.0/unigui.egg-info/requires.txt
--rw-r--r--   0 george    (1000) george    (1000)        1 2023-07-11 21:52:33.000000 unigui-1.8.0/unigui.egg-info/dependency_links.txt
--rw-r--r--   0 george    (1000) george    (1000)    19080 2023-07-11 21:52:33.000000 unigui-1.8.0/unigui.egg-info/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.8.0/unigui.egg-info/not-zip-safe
--rw-r--r--   0 george    (1000) george    (1000)     1202 2023-07-11 21:52:33.000000 unigui-1.8.0/unigui.egg-info/SOURCES.txt
--rw-r--r--   0 george    (1000) george    (1000)        7 2023-07-11 21:52:33.000000 unigui-1.8.0/unigui.egg-info/top_level.txt
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-13 23:20:16.000000 unigui-1.8.1/
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-13 23:20:16.000000 unigui-1.8.1/unigui/
+-rw-rw-r--   0 george    (1000) george    (1000)     8633 2023-07-12 21:13:45.000000 unigui-1.8.1/unigui/guielements.py
+-rw-rw-r--   0 george    (1000) george    (1000)     3344 2023-07-13 22:22:30.000000 unigui-1.8.1/unigui/server.py
+-rw-rw-r--   0 george    (1000) george    (1000)       99 2023-07-11 08:13:29.000000 unigui-1.8.1/unigui/__init__.py
+-rw-r--r--   0 george    (1000) george    (1000)     2449 2023-07-12 21:10:40.000000 unigui-1.8.1/unigui/utils.py
+-rw-rw-r--   0 george    (1000) george    (1000)     9567 2023-07-13 22:25:57.000000 unigui-1.8.1/unigui/user.py
+-rw-rw-r--   0 george    (1000) george    (1000)     4277 2023-07-13 23:09:22.000000 unigui-1.8.1/unigui/reloader.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-13 23:20:16.000000 unigui-1.8.1/unigui/web/
+-rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/favicon.ico
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-13 23:20:16.000000 unigui-1.8.1/unigui/web/css/
+-rw-rw-r--   0 george    (1000) george    (1000)        0 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/css/app.31d6cfe0.css
+-rw-rw-r--   0 george    (1000) george    (1000)     3267 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/css/295.f0f63b8f.css
+-rw-rw-r--   0 george    (1000) george    (1000)   219590 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/css/vendor.49a52e8f.css
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-13 23:20:16.000000 unigui-1.8.1/unigui/web/icons/
+-rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/icons/favicon-96x96.png
+-rw-rw-r--   0 george    (1000) george    (1000)      859 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/icons/favicon-16x16.png
+-rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/icons/favicon-32x32.png
+-rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/icons/favicon-128x128.png
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-13 23:20:16.000000 unigui-1.8.1/unigui/web/fonts/
+-rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-rw-r--   0 george    (1000) george    (1000)   128360 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
+-rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-13 23:20:16.000000 unigui-1.8.1/unigui/web/js/
+-rw-rw-r--   0 george    (1000) george    (1000)     5868 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/js/app.9384942b.js
+-rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/js/430.591e9a73.js
+-rw-rw-r--   0 george    (1000) george    (1000)    44706 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/js/295.e2b7be53.js
+-rw-rw-r--   0 george    (1000) george    (1000)      763 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/js/193.283445be.js
+-rw-rw-r--   0 george    (1000) george    (1000)  1431597 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/js/vendor.3e8714c2.js
+-rw-rw-r--   0 george    (1000) george    (1000)      907 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/index.html
+-rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.8.1/LICENSE
+-rw-rw-r--   0 george    (1000) george    (1000)      600 2023-07-13 23:18:48.000000 unigui-1.8.1/setup.py
+-rw-rw-r--   0 george    (1000) george    (1000)    18989 2023-07-13 23:20:16.000000 unigui-1.8.1/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)       38 2023-07-13 23:20:16.000000 unigui-1.8.1/setup.cfg
+-rw-rw-r--   0 george    (1000) george    (1000)    18684 2023-07-12 08:54:15.000000 unigui-1.8.1/README.md
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.8.1/MANIFEST.in
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-13 23:20:16.000000 unigui-1.8.1/unigui.egg-info/
+-rw-rw-r--   0 george    (1000) george    (1000)       30 2023-07-13 23:20:15.000000 unigui-1.8.1/unigui.egg-info/requires.txt
+-rw-r--r--   0 george    (1000) george    (1000)        1 2023-07-13 23:20:15.000000 unigui-1.8.1/unigui.egg-info/dependency_links.txt
+-rw-r--r--   0 george    (1000) george    (1000)    18989 2023-07-13 23:20:15.000000 unigui-1.8.1/unigui.egg-info/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.8.1/unigui.egg-info/not-zip-safe
+-rw-r--r--   0 george    (1000) george    (1000)     1221 2023-07-13 23:20:15.000000 unigui-1.8.1/unigui.egg-info/SOURCES.txt
+-rw-r--r--   0 george    (1000) george    (1000)        7 2023-07-13 23:20:15.000000 unigui-1.8.1/unigui.egg-info/top_level.txt
```

### Comparing `unigui-1.8.0/unigui/guielements.py` & `unigui-1.8.1/unigui/guielements.py`

 * *Files 3% similar despite different names*

```diff
@@ -205,36 +205,28 @@
 
     def clean(self):
         self.rows = []
         self.value = [] if isinstance(self.value,(tuple, list)) else None
         return self
         
 class Block(Gui):
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs):        
         self.name = args[0]        
         self.type = 'block'
+        self.value = list(args[1:])
         for key in kwargs.keys():            
-            self.add(key, kwargs[key])
-        la = len(args) 
-        self.top_childs = (args[1] if isinstance(args[1], list) else [args[1]]) if la > 1 else []                    
-        self.childs = list(args[2:]) if la > 2 else []
+            self.add(key, kwargs[key])        
         self.check()
 
     def check(self):
         ch_names = set()        
-        for child in self.childs:
-            if isinstance(child, list) or isinstance(child, tuple):
-                for sub in child:                                        
-                    if sub.name in ch_names:                        
-                        raise Exception(f'Error: the block {self.name} contains a duplicated name {sub.name}!')                        
-                    ch_names.add(sub.name)
-            else:
-                if child.name in ch_names:
-                    raise Exception(f'Error: the block {self.name} contains a duplicated name {child.name}!')                    
-                ch_names.add(child.name)
+        for child in utils.flatten(self.value):            
+            if child.name in ch_names:                        
+                raise Exception(f'Error: the block {self.name} contains a duplicated name {child.name}!')                        
+            ch_names.add(child.name)            
 
 class Dialog:  
     def __init__(self, name, callback, *content, buttons = ['Ok', 'Cancel'], icon = 'not_listed_location'):
         self.name = name
         self.callback = callback  
         self.type = 'dialog'         
         self.buttons = buttons
```

### Comparing `unigui-1.8.0/unigui/server.py` & `unigui-1.8.1/unigui/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from aiohttp import web, WSMsgType
 from .user import *
 from config import port, pretty_print, socket_ip, socket_port, upload_dir
 from pathlib import Path
+from .reloader import empty_app 
 
 async def post_handler(request):
     reader = await request.multipart()
     field = await reader.next()   
     filename = upload_path(field.filename)  
     # You cannot rely on Content-Length if transfer is chunked.
     size = 0
@@ -38,17 +39,18 @@
     ws = web.WebSocketResponse()
     await ws.prepare(request)
     user = User.UserType()
 
     async def send(res):
         await ws.send_str(jsonString(user.prepare_result(res)))        
     user.send = send 
-    user.load()
     
-    await ws.send_str(jsonString(user.screen)) 
+    ok = user.load()
+    
+    await ws.send_str(jsonString(user.screen if ok else empty_app)) 
 
     async for msg in ws:
         if msg.type == WSMsgType.TEXT:
             if msg.data == 'close':
                 await ws.close()
             else:
                 data = json.loads(msg.data)
```

### Comparing `unigui-1.8.0/unigui/utils.py` & `unigui-1.8.1/unigui/utils.py`

 * *Files identical despite different names*

### Comparing `unigui-1.8.0/unigui/user.py` & `unigui-1.8.1/unigui/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import importlib
 from .utils import *
-import itertools
 from .guielements import *
 import sys
 import asyncio
 import requests
 from threading import Thread
 
 class User:      
@@ -36,26 +35,28 @@
             file.write(response.content)
             file.close() 
         return cname
 
     @staticmethod
     def create_fixed_js():
         dir = f"{utils.webpath}/js"        
+        def replace(b, what, tothat):
+            return b.replace(bytes(what,encoding='utf8'), bytes(str(tothat),encoding='utf8'))  
         for file in os.listdir(dir):
             fn = f'{dir}/{file}'
             if file[0].isdigit() and file.endswith(".js") and os.path.getsize(fn) > 25000:
                 User.fix_file = f'/js/{file}'
                 with open(fn, 'rb') as main:
                     b = main.read()
                     if utils.socket_ip != 'localhost':
-                        b = b.replace(bytes('localhost',encoding='utf8'), bytes(str(utils.socket_ip),encoding='utf8'))                
+                        b = replace(b,'localhost', utils.socket_ip)
                     if utils.resource_port != 8000:
-                        b = b.replace(bytes('8000',encoding='utf8'), bytes(str(utils.resource_port),encoding='utf8'))                
+                        b = replace(b,'8000',utils.resource_port)
                     if utils.socket_port != 1234:
-                        b = b.replace(bytes('1234',encoding='utf8'), bytes(str(utils.socket_port),encoding='utf8'))                
+                        b = replace(b,'1234', utils.socket_port)                
                     User.fixed_main = b.decode("utf-8") 
                     print(f"Fixed {file} created on ip {utils.socket_ip}, http port {utils.resource_port}, socket port {utils.socket_port}.")
                     break
 
     def sync_send(self, obj):
         asyncio.run_coroutine_threadsafe(self.send(obj), self.extra_loop)            
 
@@ -66,16 +67,15 @@
             d['update'] = None            
             d['data'] = updates          
         self.sync_send(d)               
 
     def load_module(self, file):
         screen_vars = {
             'icon' : None,
-            'prepare' : None,
-            'dispatch' : None,
+            'prepare' : None,            
             'blocks' : [],
             'header' : utils.appname,                        
             'toolbar' : [], 
             'order' : 0
         }             
         name = file[0:-3]        
         path = f'{screens_dir}/{file}'                
@@ -86,45 +86,48 @@
         module.user = self                               
         
         spec.loader.exec_module(module)            
         screen = Screen(module.name)
         #set system vars
         for var in screen_vars:                                            
             setattr(screen, var, getattr(module,var,screen_vars[var])) 
-        screen.handlers__ = utils.handlers__
+        module.handlers__ = utils.handlers__
         
         if not screen.toolbar:
             screen.toolbar = self.tool_buttons
                         
         screen.check()                         
         module.screen = screen
         return module
 
-    def clean_sys4next_user(self):
-        #remove user modules from sys for repeating loading for new users
+    def set_clean(self):
+        #remove user modules from sys 
         if os.path.exists(blocks_dir):
             for file in os.listdir(blocks_dir):
                 if file.endswith(".py") and file != '__init__.py':
                     name = f'{blocks_dir}.{file[0:-3]}'
                     if name in sys.modules:
                         sys.modules[name].user = self
                         del sys.modules[name]                          
     def load(self):            
-        for file in os.listdir(screens_dir):
-            if file.endswith(".py") and file != '__init__.py':
-                module = self.load_module(file)                
-                self.screens.append(module)                
-        
-        self.screens.sort(key=lambda s: s.screen.order)
-        main = self.screens[0]
-        if 'prepare' in dir(main):
-            main.prepare()
-        self.screen_module = main
-        self.update_menu()
-        self.clean_sys4next_user()                        
+        if os.path.exists(screens_dir):
+            for file in os.listdir(screens_dir):
+                if file.endswith(".py") and file != '__init__.py':
+                    module = self.load_module(file)                
+                    self.screens.append(module)                
+            
+        if self.screens:
+            self.screens.sort(key=lambda s: s.screen.order)            
+            main = self.screens[0]
+            if 'prepare' in dir(main):
+                main.prepare()
+            self.screen_module = main
+            self.update_menu()
+            self.set_clean()       
+            return True                 
 
     def update_menu(self):
         menu = [[s.name,getattr(s,'icon', None)] for s in self.screens]        
         for s in self.screens:
             s.screen.menu = menu
 
     @property
@@ -162,28 +165,28 @@
     def find_element(self, path):       
         if path[0] == 'toolbar':
             for e in self.screen.toolbar:
                 if e.name == path[1]:                
                     return e
         for bl in flatten(self.blocks):
             if bl.name == path[0]:
-                for c in itertools.chain(bl.top_childs, bl.childs):
-                    if type(c) == list:
+                for c in bl.value:
+                    if isinstance(c, list):
                         for sub in c:
                             if sub.name == path[1]:
                                 return sub
                     elif c.name == path[1]:
                         return c
 
     def find_path(self, elem):        
         for bl in flatten(self.blocks):        
             if bl == elem:
                 return [bl.name]
-            for c in itertools.chain(bl.top_childs, bl.childs):
-                if type(c) == list:
+            for c in bl.value:
+                if isinstance(c, list):
                     for sub in c:
                         if sub == elem:
                             return [bl.name, sub.name]
                 elif c == elem:
                     return [bl.name, c.name]
 
     def prepare_result(self, raw):
@@ -213,36 +216,36 @@
             print(f'Unknown root command {s.name}')
         else:
             elem = self.find_element(arr)                        
             return self.process_element(elem, arr)        
         
     def process_element(self, elem, arr):        
         id = arr.pop() if len(arr) == 5 else 0
-        smeth = arr[-2]        
+        action = arr[-2]        
         val = arr[-1]
         
-        handler = self.screen.handlers__.get((elem, smeth))
+        handler = self.screen_module.handlers__.get((elem, action))
         if handler:
             result = handler(elem, val)                
             return result
         
-        handler = getattr(elem, smeth, False)                                
+        handler = getattr(elem, action, False)                                
         if handler:                
             res = handler(elem, val)  
             if id:                        
                 res = Answer(res, None, id)                
             return res
-        elif smeth == 'changed':
+        elif action == 'changed':
             if hasattr(elem,'value'): #exlude Buttons and others without 'value'
                 elem.value = val                                        
             return                        
 
-        return Error(f'{elem} does not contain method for {smeth} event type!')
+        return Error(f'{elem} does not contain method for {action} event type!')
 
-#loop and thread is for progress window and async interactions
+#loop and thread is for progress window and sync interactions
 loop = asyncio.new_event_loop()
 def f(loop):
     asyncio.set_event_loop(loop)
     loop.run_forever() 
 
 async_thread = Thread(target=f, args=(loop,))
 async_thread.start()
```

### Comparing `unigui-1.8.0/unigui/web/favicon.ico` & `unigui-1.8.1/unigui/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `unigui-1.8.0/unigui/web/css/223.f0f63b8f.css` & `unigui-1.8.1/unigui/web/css/295.f0f63b8f.css`

 * *Files identical despite different names*

### Comparing `unigui-1.8.0/unigui/web/css/vendor.49a52e8f.css` & `unigui-1.8.1/unigui/web/css/vendor.49a52e8f.css`

 * *Files identical despite different names*

### Comparing `unigui-1.8.0/unigui/web/icons/favicon-96x96.png` & `unigui-1.8.1/unigui/web/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `unigui-1.8.0/unigui/web/icons/favicon-16x16.png` & `unigui-1.8.1/unigui/web/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `unigui-1.8.0/unigui/web/icons/favicon-32x32.png` & `unigui-1.8.1/unigui/web/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `unigui-1.8.0/unigui/web/icons/favicon-128x128.png` & `unigui-1.8.1/unigui/web/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `unigui-1.8.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `unigui-1.8.1/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.8.0/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `unigui-1.8.1/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.8.0/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `unigui-1.8.1/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.8.0/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `unigui-1.8.1/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.8.0/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `unigui-1.8.1/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.8.0/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `unigui-1.8.1/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.8.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2` & `unigui-1.8.1/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2`

 * *Files identical despite different names*

### Comparing `unigui-1.8.0/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `unigui-1.8.1/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.8.0/unigui/web/js/430.591e9a73.js` & `unigui-1.8.1/unigui/web/js/430.591e9a73.js`

 * *Files identical despite different names*

### Comparing `unigui-1.8.0/unigui/web/js/223.7924e6b0.js` & `unigui-1.8.1/unigui/web/js/295.e2b7be53.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 "use strict";
 (globalThis["webpackChunkuniqua"] = globalThis["webpackChunkuniqua"] || []).push([
-    [223], {
-        4223: (e, t, a) => {
+    [295], {
+        8295: (e, t, a) => {
             a.r(t), a.d(t, {
                 default: () => Jt
             });
             var l = a(3673),
                 s = a(2323);
             const i = (0, l._)("div", {
                     class: "q-pa-lg"
@@ -216,15 +216,15 @@
                     a = Q(e);
                 for (let [l, s] of Object.entries(t)) {
                     let e = k[l];
                     const [t, i] = a[l];
                     let o, n = e.geom().el,
                         d = e.pdata ? e.pdata.name : e.name,
                         r = b[d];
-                    for (let a of r.data.childs)
+                    for (let a of r.data.value.slice(1))
                         if (Array.isArray(a)) {
                             if (a.find((t => t.name == e.data.name))) {
                                 let e = a[a.length - 1],
                                     t = `${e.name}@${d}`;
                                 o = k[t];
                                 break
                             }
@@ -465,25 +465,25 @@
                         key: 0,
                         data: e.data.logo,
                         pdata: e.data
                     }, null, 8, ["data", "pdata"])) : e.data.icon ? ((0, l.wg)(), (0, l.j4)(r, {
                         key: 1,
                         size: "sm",
                         name: e.data.icon
-                    }, null, 8, ["name"])) : (0, l.kq)("", !0), "_" != e.name[0] ? ((0, l.wg)(), (0, l.iD)("p", te, (0, s.zw)(e.name), 1)) : (0, l.kq)("", !0), ((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.data.top_childs, (t => ((0, l.wg)(), (0, l.j4)(d, {
+                    }, null, 8, ["name"])) : (0, l.kq)("", !0), "_" != e.name[0] ? ((0, l.wg)(), (0, l.iD)("p", te, (0, s.zw)(e.name), 1)) : (0, l.kq)("", !0), ((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.tops, (t => ((0, l.wg)(), (0, l.j4)(d, {
                         class: "q-ma-xs",
                         data: t,
                         pdata: e.data
                     }, null, 8, ["data", "pdata"])))), 256))]), e.data.scroll ? ((0, l.wg)(), (0, l.j4)(c, {
                         key: 0,
                         style: (0, s.j5)(e.styleSize),
                         "thumb-style": e.thumbStyle,
                         "bar-style": e.barStyle
                     }, {
-                        default: (0, l.w5)((() => [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.data.childs, (t => ((0, l.wg)(), (0, l.iD)("div", {
+                        default: (0, l.w5)((() => [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.data.value.slice(1), (t => ((0, l.wg)(), (0, l.iD)("div", {
                             class: "column",
                             data: t,
                             pdata: e.data
                         }, [t instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", le, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(t, (t => ((0, l.wg)(), (0, l.j4)(d, {
                             class: "q-ma-xs",
                             data: t,
                             pdata: e.data
@@ -492,15 +492,15 @@
                             class: "q-ma-xs",
                             data: t,
                             pdata: e.data
                         }, null, 8, ["data", "pdata"]))], 8, ae)))), 256))])),
                         _: 1
                     }, 8, ["style", "thumb-style", "bar-style"])) : ((0, l.wg)(!0), (0, l.iD)(l.HY, {
                         key: 1
-                    }, (0, l.Ko)(e.data.childs, (t => ((0, l.wg)(), (0, l.iD)("div", {
+                    }, (0, l.Ko)(e.data.value.slice(1), (t => ((0, l.wg)(), (0, l.iD)("div", {
                         class: "column",
                         data: t,
                         pdata: e.data
                     }, [t instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", ie, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(t, (t => ((0, l.wg)(), (0, l.j4)(d, {
                         class: "q-ma-xs",
                         data: t,
                         pdata: e.data
@@ -1999,14 +1999,18 @@
                         return this.data.scroll
                     },
                     expanding_width() {
                         return this.expanding
                     },
                     expanding_height() {
                         return !this.data.height && this.expanding
+                    },
+                    tops() {
+                        let e = this.data.value;
+                        return e.length ? Array.isArray(e[0]) ? e[0] : [e[0]] : []
                     }
                 },
                 props: {
                     data: {
                         type: Object,
                         required: !0
                     }
@@ -2181,16 +2185,17 @@
                             {
                                 height: a,
                                 ...l
                             } = e;
                         l.width = 750;
                         let s = {
                             name: `Picture lens of ${e.name}`,
-                            top_childs: [],
-                            childs: [l],
+                            value: [
+                                [], l
+                            ],
                             internal: !0
                         };
                         t.componentProps = {
                             data: s,
                             buttons: ["Close"]
                         }, this.$q.dialog(t)
                     },
```

### Comparing `unigui-1.8.0/unigui/web/js/app.fc1b2f39.js` & `unigui-1.8.1/unigui/web/js/app.9384942b.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -22,15 +22,15 @@
                         ["render", l]
                     ]),
                     d = c;
                 var p = r(3340),
                     f = r(8339);
                 const h = [{
                         path: "/",
-                        component: () => Promise.all([r.e(736), r.e(223)]).then(r.bind(r, 4223)),
+                        component: () => Promise.all([r.e(736), r.e(295)]).then(r.bind(r, 8295)),
                         children: [{
                             path: "",
                             component: () => Promise.all([r.e(736), r.e(430)]).then(r.bind(r, 6430))
                         }]
                     }, {
                         path: "/:catchAll(.*)*",
                         component: () => Promise.all([r.e(736), r.e(193)]).then(r.bind(r, 2193))
@@ -44,30 +44,30 @@
                                     top: 0
                                 }),
                                 routes: v,
                                 history: e("")
                             });
                         return t
                     }));
-                async function g(e, t) {
+                async function b(e, t) {
                     const r = "function" === typeof m ? await m({}) : m,
                         n = e(d);
                     return n.use(o.Z, t), {
                         app: n,
                         router: r
                     }
                 }
-                var b = r(6417),
+                var g = r(6417),
                     y = r(5597);
                 const w = {
                         config: {
                             notify: {}
                         },
                         plugins: {
-                            Notify: b.Z,
+                            Notify: g.Z,
                             Dialog: y.Z
                         }
                     },
                     O = "";
                 async function k({
                     app: e,
                     router: t
@@ -94,15 +94,15 @@
                             urlPath: i,
                             publicPath: O
                         })
                     } catch (l) {
                         return l && l.url ? void a(l.url) : void console.error("[Quasar] boot error:", l)
                     }!0 !== n && (e.use(t), e.mount("#q-app"))
                 }
-                g(n.ri, w).then((e => Promise.all([Promise.resolve().then(r.bind(r, 2390))]).then((t => {
+                b(n.ri, w).then((e => Promise.all([Promise.resolve().then(r.bind(r, 2390))]).then((t => {
                     const r = t.map((e => e.default)).filter((e => "function" === typeof e));
                     k(e, r)
                 }))))
             },
             2390: (e, t, r) => {
                 r.r(t), r.d(t, {
                     default: () => o
@@ -159,24 +159,24 @@
             })
         }
     })(), (() => {
         r.f = {}, r.e = e => Promise.all(Object.keys(r.f).reduce(((t, n) => (r.f[n](e, t), t)), []))
     })(), (() => {
         r.u = e => "js/" + e + "." + {
             193: "283445be",
-            223: "7924e6b0",
+            295: "e2b7be53",
             430: "591e9a73"
         } [e] + ".js"
     })(), (() => {
         r.miniCssF = e => "css/" + ({
             143: "app",
             736: "vendor"
         } [e] || e) + "." + {
             143: "31d6cfe0",
-            223: "f0f63b8f",
+            295: "f0f63b8f",
             736: "49a52e8f"
         } [e] + ".css"
     })(), (() => {
         r.g = function() {
             if ("object" === typeof globalThis) return globalThis;
             try {
                 return this || new Function("return this")()
@@ -260,15 +260,15 @@
                 e(n, l, o, a)
             })),
             o = {
                 143: 0
             };
         r.f.miniCss = (e, t) => {
             var r = {
-                223: 1
+                295: 1
             };
             o[e] ? t.push(o[e]) : 0 !== o[e] && r[e] && t.push(o[e] = n(e).then((() => {
                 o[e] = 0
             }), (t => {
                 throw delete o[e], t
             })))
         }
```

### Comparing `unigui-1.8.0/unigui/web/js/193.283445be.js` & `unigui-1.8.1/unigui/web/js/193.283445be.js`

 * *Files identical despite different names*

### Comparing `unigui-1.8.0/unigui/web/js/vendor.3e8714c2.js` & `unigui-1.8.1/unigui/web/js/vendor.3e8714c2.js`

 * *Files identical despite different names*

### Comparing `unigui-1.8.0/unigui/web/index.html` & `unigui-1.8.1/unigui/web/index.html`

 * *Files 9% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.3e8714c2.js></script><script defer src=js/app.fc1b2f39.js></script><link href=css/vendor.49a52e8f.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
+<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.3e8714c2.js></script><script defer src=js/app.9384942b.js></script><link href=css/vendor.49a52e8f.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
```

### Comparing `unigui-1.8.0/LICENSE` & `unigui-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unigui-1.8.0/setup.py` & `unigui-1.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
  
 setup(name='unigui',
-      version='1.8.0',      
+      version='1.8.1',      
       license='MIT',
       author='Georgii Dernovyi',
       author_email='g.dernovoy@gmail.com',
       description='Unigui - Universal GUI Framework and protocol',
       packages=find_packages(exclude=['tests']),
       long_description=open('README.md').read(),
       long_description_content_type="text/markdown",
```

### Comparing `unigui-1.8.0/PKG-INFO` & `unigui-1.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.8.0
+Version: 1.8.1
 Summary: Unigui - Universal GUI Framework and protocol
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -30,15 +30,14 @@
 ### High level - Screen ###
 The program directory has to contain a screens folder which contains all screens which Unigui has to show.
 
 Screen example tests/screens/main.py
 ```
 name = "Main"
 blocks = [block] 
-icon = 'blur_linear' 
 ```
 The block example with a table and a selector
 ```
 table = Table('Videos', 0, headers = ['Video', 'Duration',  'Links', 'Mine'],rows = [
     ['opt_sync1_3_0.mp4', '30 seconds',  '@Refer to signal1', True],
     ['opt_sync1_3_0.mp4', '37 seconds',  '@Refer to signal8', False]    
 ])
@@ -54,29 +53,28 @@
 | :---: | :---: | :---: | :---: | 
 | name  | Has to be defined | str | Unique screen name |
 | blocks | Has to be defined | list |which blocks to show on the screen |
 | user   | Always defined, read-only | User+ | Access to User(inherited) class which associated with a current user |
 | header | Optional | str | show it instead of app name |
 | toolbar | Optional | list | Gui elements to show in the screen toolbar |
 | order | Optional | int | order in the program menu |
-| icon  | Optional | str | MD icon of screen to show in screen menu |
+| icon  | Optional | str | MD icon of screen to show in the screen menu |
 | prepare | Optional | def prepare() | Syncronizes GUI elements one to another and with the program/system data. If defined then is called before screen appearing. |
 
 
 ### Server start ###
-tests/run_hello.py
+tests/template/run.py
 ```
 import unigui
-#app name, the others server setting in config.py like port, upload_dir, ..
 unigui.start('Test app') 
 ```
 Unigui builds the interactive app for the code above.
 Connect a browser to localhast:8000 which are by default and will see:
 
-![image](https://github.com/Claus1/unigui/assets/1247062/62caca12-86fc-4dcd-99b4-26845963b5cf)
+![image](https://github.com/Claus1/unigui/assets/1247062/aca4db13-df32-4c16-8fff-e6a1a74bf640)
 
 ### Handling events ###
 All handlers are functions which have a signature
 ```
 def handler_x(gui_object, value_x)
 ```
 where gui_object is a Python object the user interacted with and value for the event.
```

### Comparing `unigui-1.8.0/README.md` & `unigui-1.8.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 ### High level - Screen ###
 The program directory has to contain a screens folder which contains all screens which Unigui has to show.
 
 Screen example tests/screens/main.py
 ```
 name = "Main"
 blocks = [block] 
-icon = 'blur_linear' 
 ```
 The block example with a table and a selector
 ```
 table = Table('Videos', 0, headers = ['Video', 'Duration',  'Links', 'Mine'],rows = [
     ['opt_sync1_3_0.mp4', '30 seconds',  '@Refer to signal1', True],
     ['opt_sync1_3_0.mp4', '37 seconds',  '@Refer to signal8', False]    
 ])
@@ -42,29 +41,28 @@
 | :---: | :---: | :---: | :---: | 
 | name  | Has to be defined | str | Unique screen name |
 | blocks | Has to be defined | list |which blocks to show on the screen |
 | user   | Always defined, read-only | User+ | Access to User(inherited) class which associated with a current user |
 | header | Optional | str | show it instead of app name |
 | toolbar | Optional | list | Gui elements to show in the screen toolbar |
 | order | Optional | int | order in the program menu |
-| icon  | Optional | str | MD icon of screen to show in screen menu |
+| icon  | Optional | str | MD icon of screen to show in the screen menu |
 | prepare | Optional | def prepare() | Syncronizes GUI elements one to another and with the program/system data. If defined then is called before screen appearing. |
 
 
 ### Server start ###
-tests/run_hello.py
+tests/template/run.py
 ```
 import unigui
-#app name, the others server setting in config.py like port, upload_dir, ..
 unigui.start('Test app') 
 ```
 Unigui builds the interactive app for the code above.
 Connect a browser to localhast:8000 which are by default and will see:
 
-![image](https://github.com/Claus1/unigui/assets/1247062/62caca12-86fc-4dcd-99b4-26845963b5cf)
+![image](https://github.com/Claus1/unigui/assets/1247062/aca4db13-df32-4c16-8fff-e6a1a74bf640)
 
 ### Handling events ###
 All handlers are functions which have a signature
 ```
 def handler_x(gui_object, value_x)
 ```
 where gui_object is a Python object the user interacted with and value for the event.
```

### Comparing `unigui-1.8.0/unigui.egg-info/PKG-INFO` & `unigui-1.8.1/unigui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.8.0
+Version: 1.8.1
 Summary: Unigui - Universal GUI Framework and protocol
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -30,15 +30,14 @@
 ### High level - Screen ###
 The program directory has to contain a screens folder which contains all screens which Unigui has to show.
 
 Screen example tests/screens/main.py
 ```
 name = "Main"
 blocks = [block] 
-icon = 'blur_linear' 
 ```
 The block example with a table and a selector
 ```
 table = Table('Videos', 0, headers = ['Video', 'Duration',  'Links', 'Mine'],rows = [
     ['opt_sync1_3_0.mp4', '30 seconds',  '@Refer to signal1', True],
     ['opt_sync1_3_0.mp4', '37 seconds',  '@Refer to signal8', False]    
 ])
@@ -54,29 +53,28 @@
 | :---: | :---: | :---: | :---: | 
 | name  | Has to be defined | str | Unique screen name |
 | blocks | Has to be defined | list |which blocks to show on the screen |
 | user   | Always defined, read-only | User+ | Access to User(inherited) class which associated with a current user |
 | header | Optional | str | show it instead of app name |
 | toolbar | Optional | list | Gui elements to show in the screen toolbar |
 | order | Optional | int | order in the program menu |
-| icon  | Optional | str | MD icon of screen to show in screen menu |
+| icon  | Optional | str | MD icon of screen to show in the screen menu |
 | prepare | Optional | def prepare() | Syncronizes GUI elements one to another and with the program/system data. If defined then is called before screen appearing. |
 
 
 ### Server start ###
-tests/run_hello.py
+tests/template/run.py
 ```
 import unigui
-#app name, the others server setting in config.py like port, upload_dir, ..
 unigui.start('Test app') 
 ```
 Unigui builds the interactive app for the code above.
 Connect a browser to localhast:8000 which are by default and will see:
 
-![image](https://github.com/Claus1/unigui/assets/1247062/62caca12-86fc-4dcd-99b4-26845963b5cf)
+![image](https://github.com/Claus1/unigui/assets/1247062/aca4db13-df32-4c16-8fff-e6a1a74bf640)
 
 ### Handling events ###
 All handlers are functions which have a signature
 ```
 def handler_x(gui_object, value_x)
 ```
 where gui_object is a Python object the user interacted with and value for the event.
```

### Comparing `unigui-1.8.0/unigui.egg-info/SOURCES.txt` & `unigui-1.8.1/unigui.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 unigui/__init__.py
 unigui/guielements.py
+unigui/reloader.py
 unigui/server.py
 unigui/user.py
 unigui/utils.py
 unigui.egg-info/PKG-INFO
 unigui.egg-info/SOURCES.txt
 unigui.egg-info/dependency_links.txt
 unigui.egg-info/not-zip-safe
 unigui.egg-info/requires.txt
 unigui.egg-info/top_level.txt
 unigui/web/favicon.ico
 unigui/web/index.html
-unigui/web/css/223.f0f63b8f.css
+unigui/web/css/295.f0f63b8f.css
 unigui/web/css/app.31d6cfe0.css
 unigui/web/css/vendor.49a52e8f.css
 unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
@@ -27,11 +28,11 @@
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
 unigui/web/icons/favicon-128x128.png
 unigui/web/icons/favicon-16x16.png
 unigui/web/icons/favicon-32x32.png
 unigui/web/icons/favicon-96x96.png
 unigui/web/js/193.283445be.js
-unigui/web/js/223.7924e6b0.js
+unigui/web/js/295.e2b7be53.js
 unigui/web/js/430.591e9a73.js
-unigui/web/js/app.fc1b2f39.js
+unigui/web/js/app.9384942b.js
 unigui/web/js/vendor.3e8714c2.js
```

