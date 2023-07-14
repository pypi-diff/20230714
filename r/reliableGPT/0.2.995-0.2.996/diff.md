# Comparing `tmp/reliableGPT-0.2.995.tar.gz` & `tmp/reliableGPT-0.2.996.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.995.tar", last modified: Fri Jul 14 01:23:07 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.996.tar", last modified: Fri Jul 14 01:58:12 2023, max compression
```

## Comparing `reliableGPT-0.2.995.tar` & `reliableGPT-0.2.996.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-14 01:23:07.610204 reliableGPT-0.2.995/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.995/LICENSE
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-07-14 01:23:07.610049 reliableGPT-0.2.995/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     8826 2023-07-14 01:03:18.000000 reliableGPT-0.2.995/README.md
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      497 2023-06-28 20:45:06.000000 reliableGPT-0.2.995/pyproject.toml
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-14 01:23:07.608768 reliableGPT-0.2.995/reliableGPT.egg-info/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-07-14 01:23:07.000000 reliableGPT-0.2.995/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      361 2023-07-14 01:23:07.000000 reliableGPT-0.2.995/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-07-14 01:23:07.000000 reliableGPT-0.2.995/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       63 2023-07-14 01:23:07.000000 reliableGPT-0.2.995/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-07-14 01:23:07.000000 reliableGPT-0.2.995/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-14 01:23:07.609769 reliableGPT-0.2.995/reliablegpt/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3148 2023-07-14 01:03:18.000000 reliableGPT-0.2.995/reliablegpt/Alerting.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)    22309 2023-07-14 01:22:49.000000 reliableGPT-0.2.995/reliablegpt/IndividualRequest.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1286 2023-07-02 02:49:46.000000 reliableGPT-0.2.995/reliablegpt/Model.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       58 2023-07-10 15:34:25.000000 reliableGPT-0.2.995/reliablegpt/__init__.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     5281 2023-07-14 01:20:06.000000 reliableGPT-0.2.995/reliablegpt/main.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-07-14 01:23:07.610243 reliableGPT-0.2.995/setup.cfg
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      418 2023-07-14 01:22:57.000000 reliableGPT-0.2.995/setup.py
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-14 01:58:12.711750 reliableGPT-0.2.996/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.996/LICENSE
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-07-14 01:58:12.711650 reliableGPT-0.2.996/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     8826 2023-07-14 01:03:18.000000 reliableGPT-0.2.996/README.md
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      497 2023-06-28 20:45:06.000000 reliableGPT-0.2.996/pyproject.toml
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-14 01:58:12.710162 reliableGPT-0.2.996/reliableGPT.egg-info/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-07-14 01:58:12.000000 reliableGPT-0.2.996/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      361 2023-07-14 01:58:12.000000 reliableGPT-0.2.996/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-07-14 01:58:12.000000 reliableGPT-0.2.996/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       74 2023-07-14 01:58:12.000000 reliableGPT-0.2.996/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-07-14 01:58:12.000000 reliableGPT-0.2.996/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-14 01:58:12.711363 reliableGPT-0.2.996/reliablegpt/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3148 2023-07-14 01:03:18.000000 reliableGPT-0.2.996/reliablegpt/Alerting.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)    23016 2023-07-14 01:57:48.000000 reliableGPT-0.2.996/reliablegpt/IndividualRequest.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1286 2023-07-02 02:49:46.000000 reliableGPT-0.2.996/reliablegpt/Model.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       58 2023-07-10 15:34:25.000000 reliableGPT-0.2.996/reliablegpt/__init__.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     5281 2023-07-14 01:20:06.000000 reliableGPT-0.2.996/reliablegpt/main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-07-14 01:58:12.711784 reliableGPT-0.2.996/setup.cfg
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      440 2023-07-14 01:58:00.000000 reliableGPT-0.2.996/setup.py
```

### Comparing `reliableGPT-0.2.995/LICENSE` & `reliableGPT-0.2.996/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.995/README.md` & `reliableGPT-0.2.996/README.md`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.995/reliablegpt/Alerting.py` & `reliableGPT-0.2.996/reliablegpt/Alerting.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.995/reliablegpt/IndividualRequest.py` & `reliableGPT-0.2.996/reliablegpt/IndividualRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,32 @@
 import traceback
 from threading import active_count
 import random 
 import time 
 import asyncio 
 import signal
 
+from slack_bolt import App
+
+# Initialize the Slack app
+slack_app = App(
+  token="xoxb-4623456842593-4868689818500-KxOEnsoQj4daoL4fJx162f29",
+  signing_secret="1bbd221ad49a0e3f75a3d6b0c525ca3a")
+
+alerts_channel = "C04R9G9CXJA"
+
+
+def send_alert(msg):
+  try:
+    slack_app.client.chat_postMessage(channel=alerts_channel, text=msg)
+  except Exception as e:
+    print(f"got slack error rate limited {e}")
+
+
+
 from posthog import Posthog
 
 posthog = Posthog(
   project_api_key='phc_yZ30KsPzRXd3nYaET3VFDmquFKtMZwMTuFKVOei6viB',
   host='https://app.posthog.com')
 
 ## for testing
@@ -114,14 +132,18 @@
             input_prompt, extracted_result
           )  # [TODO] turn this into a threaded call, reduce latency.
         self.print_verbose(f"This is the result: {str(result)[:500]}")
       return result
     except Exception as e:
       self.print_verbose(f"Error: {traceback.format_exc()}")
       self.print_verbose("catches the error")
+      msg = (f'kwargs: {str(kwargs)}\n'
+          f'Exception Email: {e}\n'
+          f'Traceback: {traceback.format_exc()}\n')
+      send_alert("[reliableGPT] Failed original request \n" + msg)
       self.start_cooldown()
       return self.handle_exception(args, kwargs, e)
     
   async def async_call_model(self, args, kwargs):
     try: 
       if self._test: # private function for testing package
         error = {"type": "RandomError in async function"}
@@ -299,14 +321,17 @@
       self.print_verbose(traceback.format_exc())
       return None
 
   def make_LLM_request(self, new_kwargs):
     embedding_model = self.model.get_original_embeddings()
     chat_model = self.model.get_original_chat()
     completion_model = self.model.get_original_completion()
+
+    msg = (f'kwargs: {str(new_kwargs)}\n')
+    send_alert("[reliableGPT] Failed retrying request \n" + msg)
     try:
       self.print_verbose(f"{new_kwargs.keys()}")
       if "azure_fallback" in new_kwargs:
         new_kwargs_except_azure_fallback_flag = {
           k: v
           for k, v in new_kwargs.items() if k != "azure_fallback"
         }
```

### Comparing `reliableGPT-0.2.995/reliablegpt/Model.py` & `reliableGPT-0.2.996/reliablegpt/Model.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.995/reliablegpt/main.py` & `reliableGPT-0.2.996/reliablegpt/main.py`

 * *Files identical despite different names*

