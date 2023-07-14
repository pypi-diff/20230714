# Comparing `tmp/viyapy-0.2.1.tar.gz` & `tmp/viyapy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viyapy-0.2.1.tar", last modified: Wed Jun 22 20:47:12 2022, max compression
+gzip compressed data, was "viyapy-1.0.0.tar", last modified: Thu Jul 13 13:14:57 2023, max compression
```

## Comparing `viyapy-0.2.1.tar` & `viyapy-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-06-22 20:47:12.099335 viyapy-0.2.1/
--rw-rw-rw-   0        0        0     1084 2022-06-20 16:49:29.000000 viyapy-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     1166 2022-06-22 20:47:12.099474 viyapy-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      662 2022-06-20 19:47:08.000000 viyapy-0.2.1/README.md
--rw-rw-rw-   0        0        0       86 2022-06-20 17:05:59.000000 viyapy-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0      643 2022-06-22 20:47:12.101494 viyapy-0.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-06-22 20:47:12.062675 viyapy-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2022-06-22 20:47:12.068375 viyapy-0.2.1/src/viyapy/
--rw-rw-rw-   0        0        0        0 2022-06-20 16:53:25.000000 viyapy-0.2.1/src/viyapy/__init__.py
--rw-rw-rw-   0        0        0     4496 2022-06-22 20:45:54.000000 viyapy-0.2.1/src/viyapy/viya_utils.py
-drwxrwxrwx   0        0        0        0 2022-06-22 20:47:12.097920 viyapy-0.2.1/src/viyapy.egg-info/
--rw-rw-rw-   0        0        0     1166 2022-06-22 20:47:11.000000 viyapy-0.2.1/src/viyapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2022-06-22 20:47:12.000000 viyapy-0.2.1/src/viyapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-22 20:47:11.000000 viyapy-0.2.1/src/viyapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2022-06-22 20:47:11.000000 viyapy-0.2.1/src/viyapy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 13:14:57.271246 viyapy-1.0.0/
+-rw-rw-rw-   0        0        0     1084 2022-06-20 16:49:29.000000 viyapy-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0      926 2023-07-13 13:14:57.272245 viyapy-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      422 2023-07-07 19:27:14.000000 viyapy-1.0.0/README.md
+-rw-rw-rw-   0        0        0       86 2022-06-20 17:05:59.000000 viyapy-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0      643 2023-07-13 13:14:57.281198 viyapy-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-13 13:14:57.181790 viyapy-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-13 13:14:57.209800 viyapy-1.0.0/src/viyapy/
+-rw-rw-rw-   0        0        0        0 2022-06-20 16:53:25.000000 viyapy-1.0.0/src/viyapy/__init__.py
+-rw-rw-rw-   0        0        0     5265 2023-07-12 18:46:29.000000 viyapy-1.0.0/src/viyapy/viya_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-13 13:14:57.242509 viyapy-1.0.0/src/viyapy.egg-info/
+-rw-rw-rw-   0        0        0      926 2023-07-13 13:14:57.000000 viyapy-1.0.0/src/viyapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-13 13:14:57.000000 viyapy-1.0.0/src/viyapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 13:14:57.000000 viyapy-1.0.0/src/viyapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-13 13:14:57.000000 viyapy-1.0.0/src/viyapy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 13:14:57.265347 viyapy-1.0.0/tests/
+-rw-rw-rw-   0        0        0     2132 2022-06-20 19:36:00.000000 viyapy-1.0.0/tests/test_package.py
+-rw-rw-rw-   0        0        0     3356 2023-07-12 18:48:35.000000 viyapy-1.0.0/tests/test_package_v4.py
```

### Comparing `viyapy-0.2.1/LICENSE` & `viyapy-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `viyapy-0.2.1/setup.cfg` & `viyapy-1.0.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6979 6170 790d 0a76 6572 7369   = viyapy..versi
-00000020: 6f6e 203d 2030 2e32 2e31 0d0a 6175 7468  on = 0.2.1..auth
+00000020: 6f6e 203d 2031 2e30 2e30 0d0a 6175 7468  on = 1.0.0..auth
 00000030: 6f72 203d 2053 6561 6e20 5420 466f 7264  or = Sean T Ford
 00000040: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000050: 2070 7375 6165 726f 6669 6768 7465 7240   psuaerofighter@
 00000060: 676d 6169 6c2e 636f 6d0d 0a64 6573 6372  gmail.com..descr
 00000070: 6970 7469 6f6e 203d 2055 7469 6c69 7469  iption = Utiliti
 00000080: 6573 2066 6f72 2053 4153 2056 6979 610d  es for SAS Viya.
 00000090: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
```

### Comparing `viyapy-0.2.1/src/viyapy/viya_utils.py` & `viyapy-1.0.0/src/viyapy/viya_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -81,27 +81,40 @@
     
     #return the result as a dictionary
     return r.json()
 
 #get all the models in a decision
 def get_models(baseUrl,decisionId,accessToken):
     
+    models = []
+    
     #get the decision content
     response = get_decision_content(baseUrl,decisionId,accessToken)
     
-    #grab the flow setps
-    flow_steps = response['flow']['steps']
-    
-    models = []
+    try:
+        if response['httpStatusCode'] == 400:
+            #grab the flow setps
+            flow_steps = response['flow']['steps']
+
+            #loop through steps and capture any that are models
+            for s in flow_steps:
+                if s['type'] == 'application/vnd.sas.decision.step.model':
+                    models.append({'Model Name': s['model']['name'],'Modified By':s['modifiedBy'],'Modified Timestamp':s['modifiedTimeStamp']})
+        else:
+               print ('Error')
+               print ('errorCode: ', response['errorCode']) 
+               print ('httpStatusCode: ', response['httpStatusCode']) 
+               print ('details: ', response['details']) 
+               print ('version: ', response['version']) 
+    
+    except:
+        print ('unknown error in attempt to get decision content')
+        print ('URL: ', baseUrl)
+        print ('decisionId: ', decisionId)
     
-    #loop through steps and capture any that are models
-    for s in flow_steps:
-        if s['type'] == 'application/vnd.sas.decision.step.model':
-            models.append({'Model Name': s['model']['name'],'Modified By':s['modifiedBy'],'Modified Timestamp':s['modifiedTimeStamp']})
-            
     return models
 
 #generate inputs in the format ID is expecting from a dictionary
 def gen_viya_inputs(feature_dict):
     feature_list = []
     for k,v in feature_dict.items():
         if type(v) == str:
@@ -129,14 +142,20 @@
     # Execute the decision.
     masExecutionResponse = post(requestUrl, contentType,
      acceptType, accessToken, requestBody)
     
     return json.loads(masExecutionResponse.content)
 
 #unpack the ID outputs section as a python dictionary
-def unpack_viya_outputs(outputs):
+def unpack_viya_outputs(response):
     d = {}
-    for elem in outputs:
-        d[elem['name']] = '' if 'value' not in elem.keys() else elem['value']
-        
+    
+    #check if 'outputs' in response
+    if 'outputs' in response.keys():
+        for elem in response['outputs']:
+            d[elem['name']] = '' if 'value' not in elem.keys() else elem['value']
+    else:
+        print('error: response does not have "outputs"')
+        print('response:')
+        print(response)
     return d
```

