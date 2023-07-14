# Comparing `tmp/mutual-0.0.4.tar.gz` & `tmp/mutual-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutual-0.0.4.tar", last modified: Thu Jul 13 03:46:59 2023, max compression
+gzip compressed data, was "mutual-0.1.0.tar", last modified: Fri Jul 14 08:34:08 2023, max compression
```

## Comparing `mutual-0.0.4.tar` & `mutual-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-13 03:46:59.504562 mutual-0.0.4/
--rw-r--r--   0 alexbetita   (501) staff       (20)     1068 2023-07-13 03:33:58.000000 mutual-0.0.4/LICENSE.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)     1831 2023-07-13 03:46:59.504316 mutual-0.0.4/PKG-INFO
--rw-r--r--   0 alexbetita   (501) staff       (20)     1404 2023-07-13 03:44:59.000000 mutual-0.0.4/README.md
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-13 03:46:59.502982 mutual-0.0.4/mutual/
--rw-r--r--   0 alexbetita   (501) staff       (20)      615 2023-07-13 03:33:58.000000 mutual-0.0.4/mutual/Auth.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     1888 2023-07-13 03:45:58.000000 mutual-0.0.4/mutual/Bot.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     1490 2023-07-13 03:45:25.000000 mutual-0.0.4/mutual/Chat.py
--rw-r--r--   0 alexbetita   (501) staff       (20)       74 2023-07-13 03:33:58.000000 mutual-0.0.4/mutual/__init__.py
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-13 03:46:59.504000 mutual-0.0.4/mutual.egg-info/
--rw-r--r--   0 alexbetita   (501) staff       (20)     1831 2023-07-13 03:46:59.000000 mutual-0.0.4/mutual.egg-info/PKG-INFO
--rw-r--r--   0 alexbetita   (501) staff       (20)      257 2023-07-13 03:46:59.000000 mutual-0.0.4/mutual.egg-info/SOURCES.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)        1 2023-07-13 03:46:59.000000 mutual-0.0.4/mutual.egg-info/dependency_links.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)        9 2023-07-13 03:46:59.000000 mutual-0.0.4/mutual.egg-info/requires.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)        7 2023-07-13 03:46:59.000000 mutual-0.0.4/mutual.egg-info/top_level.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)       38 2023-07-13 03:46:59.504610 mutual-0.0.4/setup.cfg
--rw-r--r--   0 alexbetita   (501) staff       (20)      727 2023-07-13 03:46:57.000000 mutual-0.0.4/setup.py
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-14 08:34:08.016731 mutual-0.1.0/
+-rw-r--r--   0 alexbetita   (501) staff       (20)     1068 2023-07-14 00:38:03.000000 mutual-0.1.0/LICENSE.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)     3701 2023-07-14 08:34:08.016572 mutual-0.1.0/PKG-INFO
+-rw-r--r--   0 alexbetita   (501) staff       (20)     3274 2023-07-14 08:33:11.000000 mutual-0.1.0/README.md
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-14 08:34:08.015120 mutual-0.1.0/mutual/
+-rw-r--r--   0 alexbetita   (501) staff       (20)     1560 2023-07-14 07:16:33.000000 mutual-0.1.0/mutual/Auth.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     6185 2023-07-14 08:22:10.000000 mutual-0.1.0/mutual/Bot.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     3694 2023-07-14 08:06:23.000000 mutual-0.1.0/mutual/Chat.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)      546 2023-07-14 08:11:54.000000 mutual-0.1.0/mutual/Dev.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     4229 2023-07-14 08:30:49.000000 mutual-0.1.0/mutual/Prompt.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     1403 2023-07-14 08:23:22.000000 mutual-0.1.0/mutual/__init__.py
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-14 08:34:08.016245 mutual-0.1.0/mutual.egg-info/
+-rw-r--r--   0 alexbetita   (501) staff       (20)     3701 2023-07-14 08:34:08.000000 mutual-0.1.0/mutual.egg-info/PKG-INFO
+-rw-r--r--   0 alexbetita   (501) staff       (20)      273 2023-07-14 08:34:08.000000 mutual-0.1.0/mutual.egg-info/SOURCES.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)        1 2023-07-14 08:34:08.000000 mutual-0.1.0/mutual.egg-info/dependency_links.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)        9 2023-07-14 08:34:08.000000 mutual-0.1.0/mutual.egg-info/requires.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)        7 2023-07-14 08:34:08.000000 mutual-0.1.0/mutual.egg-info/top_level.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)       38 2023-07-14 08:34:08.016777 mutual-0.1.0/setup.cfg
+-rw-r--r--   0 alexbetita   (501) staff       (20)      727 2023-07-14 08:13:14.000000 mutual-0.1.0/setup.py
```

### Comparing `mutual-0.0.4/LICENSE.txt` & `mutual-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mutual-0.0.4/mutual/Auth.py` & `mutual-0.1.0/mutual/Dev.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 import requests
 import json
 import mutual
 
-def signup(user_id, email):
-    url = "https://api-agent.mutuai.io/api/signup"
-    data = {
-        "user_id": user_id,
-        "email": email
-    }
-
+def clear(bot_id):
+    url = f"https://api-agent.mutuai.io/api/clear/{bot_id}"
     headers = {
-        'Content-Type': 'application/json'
+        "Authorization": f"Bearer {mutual.api_key}"
     }
+    response = requests.get(url, headers=headers)
 
-    response = requests.post(url, data=json.dumps(data), headers=headers)
-
-    if response.status_code == 200:
+    if response.status_code < 300:
         response_json = response.json()
-        mutual.api_key = response_json.get('api_key') # save the api_key to config
         return response_json
     else:
-        raise Exception(f"Request failed with status code {response.status_code}")
+        return {
+            "details":f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
+        }
```

### Comparing `mutual-0.0.4/mutual/Bot.py` & `mutual-0.1.0/mutual/Auth.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,54 @@
 import requests
 import json
 import mutual
 
-def getBot(limit=20, offset=0):
-    url = f"https://api-agent.mutuai.io/api/bots?limit={limit}&offset={offset}"
-    headers = {
-        "Authorization": f"Bearer {mutual.api_key}"
+def signup(user_id, email):
+    url = "https://api-agent.mutuai.io/api/signup"
+    data = {
+        "user_id": user_id,
+        "email": email
     }
-    response = requests.get(url, headers=headers)
-    response.raise_for_status()  # Raise an exception if the response contains an HTTP error status code
-    return response.json()
 
-def getBots(bot_id):
-    url = f"https://api-agent.mutuai.io/api/bots/{str(bot_id)}"
     headers = {
-        "Authorization": f"Bearer {mutual.api_key}"
+        'Content-Type': 'application/json'
     }
-    response = requests.get(url, headers=headers)
-    response.raise_for_status()  # Raise an exception if the response contains an HTTP error status code
-    return response.json()
 
-def createBot(bot_id, bot_name, bot_org):
-    url = "https://api-agent.mutuai.io/api/bots"
-    headers = {
-        "Content-Type": "application/json",
-        "Authorization": f"Bearer {mutual.api_key}"
-    }
+    response = requests.post(url, data=json.dumps(data), headers=headers)
+
+    if response.status_code < 300:
+        response_json = response.json()
+        mutual.api_key = response_json.get('api_key') # save the api_key to config
+        return response_json
+    else:
+        return {
+            "user_id": None,
+            "email": None,
+            "api_key": None,
+            "details":f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
+        }
+
+
+def login(user_id, email):
+    url = "https://api-agent.mutuai.io/api/login"
     data = {
-        "bot_id": str(bot_id),
-        "bot_name": bot_name,
-        "bot_org": bot_org
+        "user_id": user_id,
+        "email": email
     }
-    response = requests.post(url, data=json.dumps(data), headers=headers)
-    response.raise_for_status()  # Raise an exception if the response contains an HTTP error status code
-    return response.json()
 
-def updateBot(bot_id, bot_name=None, bot_org=None):
-    url = f"https://api-agent.mutuai.io/api/bots/{str(bot_id)}"
     headers = {
-        "Content-Type": "application/json",
-        "Authorization": f"Bearer {mutual.api_key}"
-    }
-    data = {
-        "bot_name": bot_name,
-        "bot_org": bot_org
+        'Content-Type': 'application/json'
     }
-    # remove keys with None value
-    data = {k: v for k, v in data.items() if v is not None}
-    response = requests.patch(url, data=json.dumps(data), headers=headers)
-    response.raise_for_status()  # Raise an exception if the response contains an HTTP error status code
-    return response.json()
+
+    response = requests.post(url, data=json.dumps(data), headers=headers)
+
+    if response.status_code < 300:
+        response_json = response.json()
+        mutual.api_key = response_json.get('api_key') # save the api_key to config
+        return response_json
+    else:
+        return {
+            "user_id": None,
+            "email": None,
+            "api_key": None,
+            "details":f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
+        }
```

### Comparing `mutual-0.0.4/setup.py` & `mutual-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mutual',
-    version='0.0.4',  # beta
+    version='0.1.0',  # beta
     description='A Python client for the Mutual API.',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     author='Alex Betita', # placeholder for now
     author_email='alexbetita25@gmail.com', # placeholder for now
     url='https://github.com/Mutu-AI',  # if you have a github repo for the package
     packages=find_packages(),
```

