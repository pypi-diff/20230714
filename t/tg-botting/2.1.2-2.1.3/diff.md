# Comparing `tmp/tg-botting-2.1.2.tar.gz` & `tmp/tg-botting-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg-botting-2.1.2.tar", last modified: Thu Jul 13 23:54:32 2023, max compression
+gzip compressed data, was "tg-botting-2.1.3.tar", last modified: Fri Jul 14 00:06:21 2023, max compression
```

## Comparing `tg-botting-2.1.2.tar` & `tg-botting-2.1.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 23:54:32.264267 tg-botting-2.1.2/
--rw-rw-rw-   0        0        0     3407 2023-07-13 23:54:32.264267 tg-botting-2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1709 2023-07-12 19:32:58.000000 tg-botting-2.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-13 23:54:32.265264 tg-botting-2.1.2/setup.cfg
--rw-rw-rw-   0        0        0     2624 2023-07-12 19:37:56.000000 tg-botting-2.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 23:54:32.260277 tg-botting-2.1.2/tg_botting/
--rw-rw-rw-   0        0        0      798 2023-07-13 23:54:27.000000 tg-botting-2.1.2/tg_botting/__init__.py
--rw-rw-rw-   0        0        0       39 2023-05-26 21:28:31.000000 tg-botting-2.1.2/tg_botting/_types.py
--rw-rw-rw-   0        0        0      730 2023-07-13 11:59:36.000000 tg-botting-2.1.2/tg_botting/abstract.py
--rw-rw-rw-   0        0        0    19269 2023-07-12 16:28:14.000000 tg-botting-2.1.2/tg_botting/bot.py
--rw-rw-rw-   0        0        0    29574 2023-07-13 23:53:43.000000 tg-botting-2.1.2/tg_botting/client.py
--rw-rw-rw-   0        0        0    12615 2023-05-26 21:34:31.000000 tg-botting-2.1.2/tg_botting/cog.py
--rw-rw-rw-   0        0        0    35621 2023-05-26 21:39:01.000000 tg-botting-2.1.2/tg_botting/commands.py
--rw-rw-rw-   0        0        0     3635 2023-07-13 11:59:36.000000 tg-botting-2.1.2/tg_botting/context.py
--rw-rw-rw-   0        0        0     1361 2023-05-26 21:43:21.000000 tg-botting-2.1.2/tg_botting/context_managers.py
--rw-rw-rw-   0        0        0     1410 2023-05-26 21:35:15.000000 tg-botting-2.1.2/tg_botting/conversions.py
--rw-rw-rw-   0        0        0     3679 2023-05-26 21:31:45.000000 tg-botting-2.1.2/tg_botting/cooldowns.py
--rw-rw-rw-   0        0        0    10433 2023-05-26 21:27:27.000000 tg-botting-2.1.2/tg_botting/exceptions.py
--rw-rw-rw-   0        0        0      902 2023-05-27 14:01:15.000000 tg-botting-2.1.2/tg_botting/general.py
--rw-rw-rw-   0        0        0     9737 2023-05-27 13:35:03.000000 tg-botting-2.1.2/tg_botting/group.py
--rw-rw-rw-   0        0        0    19272 2023-07-13 23:53:43.000000 tg-botting-2.1.2/tg_botting/message.py
--rw-rw-rw-   0        0        0    33416 2023-07-13 23:43:36.000000 tg-botting-2.1.2/tg_botting/objects.py
--rw-rw-rw-   0        0        0     3037 2023-07-11 21:05:01.000000 tg-botting-2.1.2/tg_botting/permissions.py
--rw-rw-rw-   0        0        0     1919 2023-07-12 15:17:24.000000 tg-botting-2.1.2/tg_botting/user.py
--rw-rw-rw-   0        0        0     1023 2023-07-13 22:59:13.000000 tg-botting-2.1.2/tg_botting/utils.py
--rw-rw-rw-   0        0        0     4368 2023-05-26 21:44:26.000000 tg-botting-2.1.2/tg_botting/view.py
-drwxrwxrwx   0        0        0        0 2023-07-13 23:54:32.263269 tg-botting-2.1.2/tg_botting.egg-info/
--rw-rw-rw-   0        0        0     3407 2023-07-13 23:54:32.000000 tg-botting-2.1.2/tg_botting.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      632 2023-07-13 23:54:32.000000 tg-botting-2.1.2/tg_botting.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 23:54:32.000000 tg-botting-2.1.2/tg_botting.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-07-13 23:54:32.000000 tg-botting-2.1.2/tg_botting.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-13 23:54:32.000000 tg-botting-2.1.2/tg_botting.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 00:06:21.574089 tg-botting-2.1.3/
+-rw-rw-rw-   0        0        0     3407 2023-07-14 00:06:21.573066 tg-botting-2.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1709 2023-07-12 19:32:58.000000 tg-botting-2.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-14 00:06:21.574089 tg-botting-2.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     2624 2023-07-12 19:37:56.000000 tg-botting-2.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 00:06:21.569076 tg-botting-2.1.3/tg_botting/
+-rw-rw-rw-   0        0        0      798 2023-07-14 00:06:13.000000 tg-botting-2.1.3/tg_botting/__init__.py
+-rw-rw-rw-   0        0        0       39 2023-05-26 21:28:31.000000 tg-botting-2.1.3/tg_botting/_types.py
+-rw-rw-rw-   0        0        0      730 2023-07-13 11:59:36.000000 tg-botting-2.1.3/tg_botting/abstract.py
+-rw-rw-rw-   0        0        0    19269 2023-07-12 16:28:14.000000 tg-botting-2.1.3/tg_botting/bot.py
+-rw-rw-rw-   0        0        0    29574 2023-07-13 23:53:43.000000 tg-botting-2.1.3/tg_botting/client.py
+-rw-rw-rw-   0        0        0    12615 2023-05-26 21:34:31.000000 tg-botting-2.1.3/tg_botting/cog.py
+-rw-rw-rw-   0        0        0    35621 2023-05-26 21:39:01.000000 tg-botting-2.1.3/tg_botting/commands.py
+-rw-rw-rw-   0        0        0     3635 2023-07-13 11:59:36.000000 tg-botting-2.1.3/tg_botting/context.py
+-rw-rw-rw-   0        0        0     1361 2023-05-26 21:43:21.000000 tg-botting-2.1.3/tg_botting/context_managers.py
+-rw-rw-rw-   0        0        0     1410 2023-05-26 21:35:15.000000 tg-botting-2.1.3/tg_botting/conversions.py
+-rw-rw-rw-   0        0        0     3679 2023-05-26 21:31:45.000000 tg-botting-2.1.3/tg_botting/cooldowns.py
+-rw-rw-rw-   0        0        0    10433 2023-05-26 21:27:27.000000 tg-botting-2.1.3/tg_botting/exceptions.py
+-rw-rw-rw-   0        0        0      902 2023-05-27 14:01:15.000000 tg-botting-2.1.3/tg_botting/general.py
+-rw-rw-rw-   0        0        0     9737 2023-05-27 13:35:03.000000 tg-botting-2.1.3/tg_botting/group.py
+-rw-rw-rw-   0        0        0    19264 2023-07-14 00:05:53.000000 tg-botting-2.1.3/tg_botting/message.py
+-rw-rw-rw-   0        0        0    33416 2023-07-13 23:43:36.000000 tg-botting-2.1.3/tg_botting/objects.py
+-rw-rw-rw-   0        0        0     3037 2023-07-11 21:05:01.000000 tg-botting-2.1.3/tg_botting/permissions.py
+-rw-rw-rw-   0        0        0     1919 2023-07-12 15:17:24.000000 tg-botting-2.1.3/tg_botting/user.py
+-rw-rw-rw-   0        0        0     1023 2023-07-13 22:59:13.000000 tg-botting-2.1.3/tg_botting/utils.py
+-rw-rw-rw-   0        0        0     4368 2023-05-26 21:44:26.000000 tg-botting-2.1.3/tg_botting/view.py
+drwxrwxrwx   0        0        0        0 2023-07-14 00:06:21.572069 tg-botting-2.1.3/tg_botting.egg-info/
+-rw-rw-rw-   0        0        0     3407 2023-07-14 00:06:21.000000 tg-botting-2.1.3/tg_botting.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      632 2023-07-14 00:06:21.000000 tg-botting-2.1.3/tg_botting.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 00:06:21.000000 tg-botting-2.1.3/tg_botting.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-07-14 00:06:21.000000 tg-botting-2.1.3/tg_botting.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-14 00:06:21.000000 tg-botting-2.1.3/tg_botting.egg-info/top_level.txt
```

### Comparing `tg-botting-2.1.2/PKG-INFO` & `tg-botting-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-botting
-Version: 2.1.2
+Version: 2.1.3
 Summary: A basic package for building async TG bots
 Home-page: https://github.com/2sweetheart2/tg_botting
 Author: Sweetie (Roma Fomkin)
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `tg-botting-2.1.2/README.md` & `tg-botting-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.2/setup.py` & `tg-botting-2.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.2/tg_botting/__init__.py` & `tg-botting-2.1.3/tg_botting/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 _title__ = 'tg_botting'
 __author__ = 'Sweetie'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023-present Sweetie'
-__version__ = '2.1.2'
+__version__ = '2.1.3'
 
 from collections import namedtuple
 import logging
 
 from .bot import Bot
 from .conversions import Converter
 from .message import *
```

### Comparing `tg-botting-2.1.2/tg_botting/abstract.py` & `tg-botting-2.1.3/tg_botting/abstract.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.2/tg_botting/bot.py` & `tg-botting-2.1.3/tg_botting/bot.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.2/tg_botting/client.py` & `tg-botting-2.1.3/tg_botting/client.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.2/tg_botting/cog.py` & `tg-botting-2.1.3/tg_botting/cog.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.2/tg_botting/commands.py` & `tg-botting-2.1.3/tg_botting/commands.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.2/tg_botting/context.py` & `tg-botting-2.1.3/tg_botting/context.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.2/tg_botting/context_managers.py` & `tg-botting-2.1.3/tg_botting/context_managers.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.2/tg_botting/conversions.py` & `tg-botting-2.1.3/tg_botting/conversions.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.2/tg_botting/cooldowns.py` & `tg-botting-2.1.3/tg_botting/cooldowns.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.2/tg_botting/exceptions.py` & `tg-botting-2.1.3/tg_botting/exceptions.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.2/tg_botting/general.py` & `tg-botting-2.1.3/tg_botting/general.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.2/tg_botting/group.py` & `tg-botting-2.1.3/tg_botting/group.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.2/tg_botting/message.py` & `tg-botting-2.1.3/tg_botting/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -257,18 +257,18 @@
             'message_id': self.message_id
         }
         res = await self.bot.tg_request('deleteMessage', **params)
         if 'error' in res.keys():
             raise TGApiError('[{error_code}] {error_msg}'.format(**res['error']))
 
 
-    async def send_photo(self,chat_id: int,
+    async def send_photo(self,
                          photo:str,
                          caption: str=None,**kwargs):
-        res = await self.bot.send_message(chat_id,photo,caption,*kwargs)
+        res = await self.bot.send_message(self.chat.id,photo,caption,*kwargs)
         if 'error' in res.keys():
             raise TGApiError('[{error_code}] {error_msg}'.format(**res['error']))
         return Message(res['result'])
 
     async def reply(self, text, **kwargs):
         return await self.bot.send_message(text, reply_to_message_id=self.message_id,**kwargs)
```

### Comparing `tg-botting-2.1.2/tg_botting/objects.py` & `tg-botting-2.1.3/tg_botting/objects.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.2/tg_botting/permissions.py` & `tg-botting-2.1.3/tg_botting/permissions.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.2/tg_botting/user.py` & `tg-botting-2.1.3/tg_botting/user.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.2/tg_botting/utils.py` & `tg-botting-2.1.3/tg_botting/utils.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.2/tg_botting/view.py` & `tg-botting-2.1.3/tg_botting/view.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.2/tg_botting.egg-info/PKG-INFO` & `tg-botting-2.1.3/tg_botting.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-botting
-Version: 2.1.2
+Version: 2.1.3
 Summary: A basic package for building async TG bots
 Home-page: https://github.com/2sweetheart2/tg_botting
 Author: Sweetie (Roma Fomkin)
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `tg-botting-2.1.2/tg_botting.egg-info/SOURCES.txt` & `tg-botting-2.1.3/tg_botting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

