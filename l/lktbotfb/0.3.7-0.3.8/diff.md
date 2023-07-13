# Comparing `tmp/lktbotfb-0.3.7.tar.gz` & `tmp/lktbotfb-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lktbotfb-0.3.7.tar", last modified: Thu Jul 13 00:39:13 2023, max compression
+gzip compressed data, was "lktbotfb-0.3.8.tar", last modified: Thu Jul 13 23:38:52 2023, max compression
```

## Comparing `lktbotfb-0.3.7.tar` & `lktbotfb-0.3.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 00:39:13.597291 lktbotfb-0.3.7/
--rw-rw-rw-   0        0        0     1093 2023-07-10 16:21:58.000000 lktbotfb-0.3.7/LICENSE
--rw-rw-rw-   0        0        0      885 2023-07-13 00:39:13.595306 lktbotfb-0.3.7/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-07-10 16:19:54.000000 lktbotfb-0.3.7/README.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 00:39:13.597291 lktbotfb-0.3.7/setup.cfg
--rw-rw-rw-   0        0        0      764 2023-07-13 00:38:21.000000 lktbotfb-0.3.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 00:39:13.512057 lktbotfb-0.3.7/src/
-drwxrwxrwx   0        0        0        0 2023-07-13 00:39:13.552714 lktbotfb-0.3.7/src/botfb/
--rw-rw-rw-   0        0        0       22 2023-07-10 14:52:18.000000 lktbotfb-0.3.7/src/botfb/__init__.py
--rw-rw-rw-   0        0        0     8829 2023-07-12 23:27:28.000000 lktbotfb-0.3.7/src/botfb/mylib.py
-drwxrwxrwx   0        0        0        0 2023-07-13 00:39:13.592295 lktbotfb-0.3.7/src/lktbotfb.egg-info/
--rw-rw-rw-   0        0        0      885 2023-07-13 00:39:13.000000 lktbotfb-0.3.7/src/lktbotfb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2023-07-13 00:39:13.000000 lktbotfb-0.3.7/src/lktbotfb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 00:39:13.000000 lktbotfb-0.3.7/src/lktbotfb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-13 00:39:13.000000 lktbotfb-0.3.7/src/lktbotfb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-13 00:39:13.000000 lktbotfb-0.3.7/src/lktbotfb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 23:38:52.872034 lktbotfb-0.3.8/
+-rw-rw-rw-   0        0        0     1093 2023-07-10 16:21:58.000000 lktbotfb-0.3.8/LICENSE
+-rw-rw-rw-   0        0        0      885 2023-07-13 23:38:52.870030 lktbotfb-0.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-07-10 16:19:54.000000 lktbotfb-0.3.8/README.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 23:38:52.872034 lktbotfb-0.3.8/setup.cfg
+-rw-rw-rw-   0        0        0      764 2023-07-13 23:37:39.000000 lktbotfb-0.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 23:38:52.693043 lktbotfb-0.3.8/src/
+drwxrwxrwx   0        0        0        0 2023-07-13 23:38:52.765039 lktbotfb-0.3.8/src/botfb/
+-rw-rw-rw-   0        0        0       22 2023-07-10 14:52:18.000000 lktbotfb-0.3.8/src/botfb/__init__.py
+-rw-rw-rw-   0        0        0     9401 2023-07-13 23:31:39.000000 lktbotfb-0.3.8/src/botfb/mylib.py
+drwxrwxrwx   0        0        0        0 2023-07-13 23:38:52.867032 lktbotfb-0.3.8/src/lktbotfb.egg-info/
+-rw-rw-rw-   0        0        0      885 2023-07-13 23:38:52.000000 lktbotfb-0.3.8/src/lktbotfb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2023-07-13 23:38:52.000000 lktbotfb-0.3.8/src/lktbotfb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 23:38:52.000000 lktbotfb-0.3.8/src/lktbotfb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-13 23:38:52.000000 lktbotfb-0.3.8/src/lktbotfb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-13 23:38:52.000000 lktbotfb-0.3.8/src/lktbotfb.egg-info/top_level.txt
```

### Comparing `lktbotfb-0.3.7/LICENSE` & `lktbotfb-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lktbotfb-0.3.7/PKG-INFO` & `lktbotfb-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lktbotfb
-Version: 0.3.7
+Version: 0.3.8
 Summary: This makes it easy for you to create a chatbot for your Facebook page
 Home-page: https://github.com/AmirLouktaila/lktbotfb
 Author: Salah Louktaila
 Author-email: amir.Louktila@gmail.com
 License: MIT
 Keywords: chatbot
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `lktbotfb-0.3.7/setup.py` & `lktbotfb-0.3.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
 
 setup(
   name='lktbotfb',
-  version='0.3.7',
+  version='0.3.8',
   description='This makes it easy for you to create a chatbot for your Facebook page',
   long_description=open('README.txt').read(),
   url='https://github.com/AmirLouktaila/lktbotfb',  
   author='Salah Louktaila',
   author_email='amir.Louktila@gmail.com',
   license='MIT', 
   classifiers=classifiers,
```

### Comparing `lktbotfb-0.3.7/src/botfb/mylib.py` & `lktbotfb-0.3.8/src/botfb/mylib.py`

 * *Files 5% similar despite different names*

```diff
@@ -159,17 +159,28 @@
 
 
 def post_facebook_message(fbid, received_message):
 
 
     global talks_text
 
-    if 'attachments' in received_message and received_message['attachments'][0]['type'] == 'image':
-        reply = "شكراً على الإعجاب!"
+    if 'attachments' in received_message and received_message['attachments'][0]['type'] == 'image' and 'payload' in received_message['attachments'][0] and 'sticker_id' in received_message['attachments'][0]['payload']:
+      
+        reply = 'thanks for like'
         talks_text = reply
+    elif 'attachments' in received_message and received_message['attachments'][0]['type'] == 'image':
+        
+        reply ='this image'#received_message['attachments'][0]['payload']['url']
+
+        talks_text = reply   
+    elif 'attachments' in received_message and received_message['attachments'][0]['type'] == 'video':
+        reply ='this video'#received_message['attachments'][0]['payload']['url']
+        talks_text = reply   
+        
+        
     elif 'text' in received_message:
         talks = received_message['text']
         reply = tempmail_bot(talks)
         talks_text = reply
     else:
         talks_text = ""  # Default value if no match in cases
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `lktbotfb-0.3.7/src/lktbotfb.egg-info/PKG-INFO` & `lktbotfb-0.3.8/src/lktbotfb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lktbotfb
-Version: 0.3.7
+Version: 0.3.8
 Summary: This makes it easy for you to create a chatbot for your Facebook page
 Home-page: https://github.com/AmirLouktaila/lktbotfb
 Author: Salah Louktaila
 Author-email: amir.Louktila@gmail.com
 License: MIT
 Keywords: chatbot
 Classifier: Development Status :: 5 - Production/Stable
```

