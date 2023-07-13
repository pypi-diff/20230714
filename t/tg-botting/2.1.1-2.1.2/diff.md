# Comparing `tmp/tg-botting-2.1.1.tar.gz` & `tmp/tg-botting-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg-botting-2.1.1.tar", last modified: Thu Jul 13 14:59:43 2023, max compression
+gzip compressed data, was "tg-botting-2.1.2.tar", last modified: Thu Jul 13 23:54:32 2023, max compression
```

## Comparing `tg-botting-2.1.1.tar` & `tg-botting-2.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 14:59:43.907504 tg-botting-2.1.1/
--rw-rw-rw-   0        0        0     3407 2023-07-13 14:59:43.907504 tg-botting-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1709 2023-07-12 19:32:58.000000 tg-botting-2.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-13 14:59:43.907504 tg-botting-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0     2624 2023-07-12 19:37:56.000000 tg-botting-2.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 14:59:43.907504 tg-botting-2.1.1/tg_botting/
--rw-rw-rw-   0        0        0      798 2023-07-13 14:59:25.000000 tg-botting-2.1.1/tg_botting/__init__.py
--rw-rw-rw-   0        0        0       39 2023-05-26 21:28:31.000000 tg-botting-2.1.1/tg_botting/_types.py
--rw-rw-rw-   0        0        0      730 2023-07-13 11:59:36.000000 tg-botting-2.1.1/tg_botting/abstract.py
--rw-rw-rw-   0        0        0    19269 2023-07-12 16:28:14.000000 tg-botting-2.1.1/tg_botting/bot.py
--rw-rw-rw-   0        0        0    27119 2023-07-13 14:59:13.000000 tg-botting-2.1.1/tg_botting/client.py
--rw-rw-rw-   0        0        0    12615 2023-05-26 21:34:31.000000 tg-botting-2.1.1/tg_botting/cog.py
--rw-rw-rw-   0        0        0    35621 2023-05-26 21:39:01.000000 tg-botting-2.1.1/tg_botting/commands.py
--rw-rw-rw-   0        0        0     3635 2023-07-13 11:59:36.000000 tg-botting-2.1.1/tg_botting/context.py
--rw-rw-rw-   0        0        0     1361 2023-05-26 21:43:21.000000 tg-botting-2.1.1/tg_botting/context_managers.py
--rw-rw-rw-   0        0        0     1410 2023-05-26 21:35:15.000000 tg-botting-2.1.1/tg_botting/conversions.py
--rw-rw-rw-   0        0        0     3679 2023-05-26 21:31:45.000000 tg-botting-2.1.1/tg_botting/cooldowns.py
--rw-rw-rw-   0        0        0    10433 2023-05-26 21:27:27.000000 tg-botting-2.1.1/tg_botting/exceptions.py
--rw-rw-rw-   0        0        0      902 2023-05-27 14:01:15.000000 tg-botting-2.1.1/tg_botting/general.py
--rw-rw-rw-   0        0        0     9737 2023-05-27 13:35:03.000000 tg-botting-2.1.1/tg_botting/group.py
--rw-rw-rw-   0        0        0    19098 2023-07-13 14:58:01.000000 tg-botting-2.1.1/tg_botting/message.py
--rw-rw-rw-   0        0        0    29358 2023-07-12 16:28:14.000000 tg-botting-2.1.1/tg_botting/objects.py
--rw-rw-rw-   0        0        0     3037 2023-07-11 21:05:01.000000 tg-botting-2.1.1/tg_botting/permissions.py
--rw-rw-rw-   0        0        0     1919 2023-07-12 15:17:24.000000 tg-botting-2.1.1/tg_botting/user.py
--rw-rw-rw-   0        0        0     1021 2023-07-12 15:20:00.000000 tg-botting-2.1.1/tg_botting/utils.py
--rw-rw-rw-   0        0        0     4368 2023-05-26 21:44:26.000000 tg-botting-2.1.1/tg_botting/view.py
-drwxrwxrwx   0        0        0        0 2023-07-13 14:59:43.907504 tg-botting-2.1.1/tg_botting.egg-info/
--rw-rw-rw-   0        0        0     3407 2023-07-13 14:59:43.000000 tg-botting-2.1.1/tg_botting.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      632 2023-07-13 14:59:43.000000 tg-botting-2.1.1/tg_botting.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 14:59:43.000000 tg-botting-2.1.1/tg_botting.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-07-13 14:59:43.000000 tg-botting-2.1.1/tg_botting.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-13 14:59:43.000000 tg-botting-2.1.1/tg_botting.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 23:54:32.264267 tg-botting-2.1.2/
+-rw-rw-rw-   0        0        0     3407 2023-07-13 23:54:32.264267 tg-botting-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1709 2023-07-12 19:32:58.000000 tg-botting-2.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-13 23:54:32.265264 tg-botting-2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     2624 2023-07-12 19:37:56.000000 tg-botting-2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 23:54:32.260277 tg-botting-2.1.2/tg_botting/
+-rw-rw-rw-   0        0        0      798 2023-07-13 23:54:27.000000 tg-botting-2.1.2/tg_botting/__init__.py
+-rw-rw-rw-   0        0        0       39 2023-05-26 21:28:31.000000 tg-botting-2.1.2/tg_botting/_types.py
+-rw-rw-rw-   0        0        0      730 2023-07-13 11:59:36.000000 tg-botting-2.1.2/tg_botting/abstract.py
+-rw-rw-rw-   0        0        0    19269 2023-07-12 16:28:14.000000 tg-botting-2.1.2/tg_botting/bot.py
+-rw-rw-rw-   0        0        0    29574 2023-07-13 23:53:43.000000 tg-botting-2.1.2/tg_botting/client.py
+-rw-rw-rw-   0        0        0    12615 2023-05-26 21:34:31.000000 tg-botting-2.1.2/tg_botting/cog.py
+-rw-rw-rw-   0        0        0    35621 2023-05-26 21:39:01.000000 tg-botting-2.1.2/tg_botting/commands.py
+-rw-rw-rw-   0        0        0     3635 2023-07-13 11:59:36.000000 tg-botting-2.1.2/tg_botting/context.py
+-rw-rw-rw-   0        0        0     1361 2023-05-26 21:43:21.000000 tg-botting-2.1.2/tg_botting/context_managers.py
+-rw-rw-rw-   0        0        0     1410 2023-05-26 21:35:15.000000 tg-botting-2.1.2/tg_botting/conversions.py
+-rw-rw-rw-   0        0        0     3679 2023-05-26 21:31:45.000000 tg-botting-2.1.2/tg_botting/cooldowns.py
+-rw-rw-rw-   0        0        0    10433 2023-05-26 21:27:27.000000 tg-botting-2.1.2/tg_botting/exceptions.py
+-rw-rw-rw-   0        0        0      902 2023-05-27 14:01:15.000000 tg-botting-2.1.2/tg_botting/general.py
+-rw-rw-rw-   0        0        0     9737 2023-05-27 13:35:03.000000 tg-botting-2.1.2/tg_botting/group.py
+-rw-rw-rw-   0        0        0    19272 2023-07-13 23:53:43.000000 tg-botting-2.1.2/tg_botting/message.py
+-rw-rw-rw-   0        0        0    33416 2023-07-13 23:43:36.000000 tg-botting-2.1.2/tg_botting/objects.py
+-rw-rw-rw-   0        0        0     3037 2023-07-11 21:05:01.000000 tg-botting-2.1.2/tg_botting/permissions.py
+-rw-rw-rw-   0        0        0     1919 2023-07-12 15:17:24.000000 tg-botting-2.1.2/tg_botting/user.py
+-rw-rw-rw-   0        0        0     1023 2023-07-13 22:59:13.000000 tg-botting-2.1.2/tg_botting/utils.py
+-rw-rw-rw-   0        0        0     4368 2023-05-26 21:44:26.000000 tg-botting-2.1.2/tg_botting/view.py
+drwxrwxrwx   0        0        0        0 2023-07-13 23:54:32.263269 tg-botting-2.1.2/tg_botting.egg-info/
+-rw-rw-rw-   0        0        0     3407 2023-07-13 23:54:32.000000 tg-botting-2.1.2/tg_botting.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      632 2023-07-13 23:54:32.000000 tg-botting-2.1.2/tg_botting.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 23:54:32.000000 tg-botting-2.1.2/tg_botting.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-07-13 23:54:32.000000 tg-botting-2.1.2/tg_botting.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-13 23:54:32.000000 tg-botting-2.1.2/tg_botting.egg-info/top_level.txt
```

### Comparing `tg-botting-2.1.1/PKG-INFO` & `tg-botting-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-botting
-Version: 2.1.1
+Version: 2.1.2
 Summary: A basic package for building async TG bots
 Home-page: https://github.com/2sweetheart2/tg_botting
 Author: Sweetie (Roma Fomkin)
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `tg-botting-2.1.1/README.md` & `tg-botting-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.1/setup.py` & `tg-botting-2.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.1/tg_botting/__init__.py` & `tg-botting-2.1.2/tg_botting/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 _title__ = 'tg_botting'
 __author__ = 'Sweetie'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023-present Sweetie'
-__version__ = '2.1.1'
+__version__ = '2.1.2'
 
 from collections import namedtuple
 import logging
 
 from .bot import Bot
 from .conversions import Converter
 from .message import *
```

### Comparing `tg-botting-2.1.1/tg_botting/abstract.py` & `tg-botting-2.1.2/tg_botting/abstract.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.1/tg_botting/bot.py` & `tg-botting-2.1.2/tg_botting/bot.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.1/tg_botting/client.py` & `tg-botting-2.1.2/tg_botting/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 import asyncio
 import enum
 import sys
 import textwrap
 import traceback
+import typing
+from typing import TypeVar
 
 import aiohttp
 
 from tg_botting.exceptions import TGException, TGApiError, BadArgument
 from tg_botting.general import convert_params
 from tg_botting.message import Chat, Message, CallbackQuery
-from tg_botting.objects import get_chat_member
+from tg_botting.objects import get_chat_member, MessageEntity, InlineKeyboardMarkup, ReplyKeyboardMarkup, \
+    ReplyKeyboardRemove
 from tg_botting.user import User
 from tg_botting.utils import to_json, maybe_coroutine
 
+String = TypeVar('String', bound=str)
+Integer = TypeVar('Integer', bound=int)
+Float = TypeVar('Float', bound=float)
+Boolean = TypeVar('Boolean', bound=bool)
+T = TypeVar('T')
 
 class UserMessageFlags(enum.IntFlag):
     Unread = 1,
     Outbox = 2,
     Replied = 4,
     Important = 8,
     Chat = 16,
@@ -410,14 +418,58 @@
         else:
             self._schedule_event(coro, method, *args, **kwargs)
 
     async def on_error(self, event_method, *args, **kwargs):
         print('Ignoring exception in {}'.format(event_method), file=sys.stderr)
         traceback.print_exc()
 
+    async def send_photo(self,
+                         chat_id: typing.Union[Integer],
+                         photo: typing.Union[String],
+                         caption: typing.Optional[String] = None,
+                         parse_mode: typing.Optional[String] = None,
+                         caption_entities: typing.Optional[typing.List[MessageEntity]] = None,
+                         message_thread_id: typing.Optional[Integer] = None,
+                         disable_notification: typing.Optional[Boolean] = None,
+                         protect_content: typing.Optional[Boolean] = None,
+                         reply_to_message_id: typing.Optional[Integer] = None,
+                         allow_sending_without_reply: typing.Optional[Boolean] = None,
+                         reply_markup: typing.Union[InlineKeyboardMarkup,
+                         ReplyKeyboardMarkup,
+                         ReplyKeyboardRemove,
+                         None] = None,
+                         has_spoiler: typing.Optional[Boolean] = None,
+                         ) -> Message:
+        reply_markup = reply_markup.dict if reply_markup is not None else None
+        caption_entities = [r.dict for r in caption_entities] if caption_entities else None
+        data = {
+            'chat_id':chat_id,
+            'photo':photo,
+            'caption':caption,
+            'parse_mode':parse_mode,
+            'caption_entities':caption_entities,
+            'message_thread_id':message_thread_id,
+            'disable_notification':disable_notification,
+            'protect_content':protect_content,
+            'reply_to_message_id':reply_to_message_id,
+            'allow_sending_without_reply':allow_sending_without_reply,
+            'reply_markup':reply_markup,
+            'has_spoiler':has_spoiler
+        }
+
+        result = await self.tg_request('dendPhoto', True, **data)
+        return result
+
+    @staticmethod
+    def prepare_file(payload, files, key, file):
+        if isinstance(file, str):
+            payload[key] = file
+        elif file is not None:
+            files[key] = file
+
     async def _run_event(self, coro, event_name, *args, **kwargs):
         try:
             await coro(*args, **kwargs)
         except asyncio.CancelledError:
             pass
         except Exception:
             try:
```

### Comparing `tg-botting-2.1.1/tg_botting/cog.py` & `tg-botting-2.1.2/tg_botting/cog.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.1/tg_botting/commands.py` & `tg-botting-2.1.2/tg_botting/commands.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.1/tg_botting/context.py` & `tg-botting-2.1.2/tg_botting/context.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.1/tg_botting/context_managers.py` & `tg-botting-2.1.2/tg_botting/context_managers.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.1/tg_botting/conversions.py` & `tg-botting-2.1.2/tg_botting/conversions.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.1/tg_botting/cooldowns.py` & `tg-botting-2.1.2/tg_botting/cooldowns.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.1/tg_botting/exceptions.py` & `tg-botting-2.1.2/tg_botting/exceptions.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.1/tg_botting/general.py` & `tg-botting-2.1.2/tg_botting/general.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.1/tg_botting/group.py` & `tg-botting-2.1.2/tg_botting/group.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.1/tg_botting/message.py` & `tg-botting-2.1.2/tg_botting/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -256,22 +256,25 @@
             'chat_id': self.chat.id,
             'message_id': self.message_id
         }
         res = await self.bot.tg_request('deleteMessage', **params)
         if 'error' in res.keys():
             raise TGApiError('[{error_code}] {error_msg}'.format(**res['error']))
 
-    async def reply(self, message=None, **kwargs):
-        forward = {
-            'peer_id': self.peer_id,
-            'is_reply': True,
-            'conversation_message_ids': self.conversation_message_id,
-        }
-        kwargs['forward'] = forward
-        return await self.bot.send_message(self.peer_id, message, **kwargs)
+
+    async def send_photo(self,chat_id: int,
+                         photo:str,
+                         caption: str=None,**kwargs):
+        res = await self.bot.send_message(chat_id,photo,caption,*kwargs)
+        if 'error' in res.keys():
+            raise TGApiError('[{error_code}] {error_msg}'.format(**res['error']))
+        return Message(res['result'])
+
+    async def reply(self, text, **kwargs):
+        return await self.bot.send_message(text, reply_to_message_id=self.message_id,**kwargs)
 
     async def get_user(self):
         author = await self.bot.get_pages(self.from_id)
         return author[0]
 
     async def get_author(self):
         return await self.get_user()
```

### Comparing `tg-botting-2.1.1/tg_botting/objects.py` & `tg-botting-2.1.2/tg_botting/objects.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 from copy import deepcopy
 from datetime import datetime
 
 from tg_botting.user import User
 from tg_botting.utils import get_params_from_func, get_params_from_class
 
 
@@ -545,14 +546,18 @@
     def __init__(self, data):
         self.original_data = deepcopy(data)
         self._unpack(data)
 
     def _unpack(self, data):
         self.url = data.get('url')
 
+    @property
+    def dict(self):
+        return {'url':self.url}
+
 
 class LoginUrl:
     def __init__(self, data):
         self.original_data = deepcopy(data)
         self._unpack(data)
 
     def _unpack(self, data):
@@ -642,14 +647,109 @@
     @property
     def dict(self):
         data = {
             'inline_keyboard': [r.dict for r in self.inline_keyboard]
         }
         return data
 
+class KeyboardButtonRequestUser:
+    def __init__(self, request_id, user_is_bot=None,user_is_premium=None):
+        self.request_id = request_id
+        self.user_is_bot = user_is_bot
+        self.user_is_premium = user_is_premium
+
+    @property
+    def dict(self):
+        return self.__dict__
+
+class ChatAdministratorRights:
+    def __init__(self,is_anonymous=False,can_manage_chat=False,can_delete_messages=False,
+                 can_manage_video_chats=False,can_restrict_members=False,can_promote_members=False,
+                 can_change_info=False,can_invite_users=False,can_post_messages=False,
+                 can_edit_messages=False,can_pin_messages=False,can_manage_topics=False):
+        self.is_anonymous = is_anonymous
+        self.can_manage_chat = can_manage_chat
+        self.can_delete_messages = can_delete_messages
+        self.can_manage_video_chats = can_manage_video_chats
+        self.can_restrict_members =can_restrict_members
+        self.can_promote_members = can_promote_members
+        self.can_change_info = can_change_info
+        self.can_invite_users = can_invite_users
+        self.can_post_messages = can_post_messages
+        self.can_edit_messages = can_edit_messages
+        self.can_pin_messages = can_pin_messages
+        self.can_manage_topics = can_manage_topics
+
+    @property
+    def dict(self):
+        return self.__dict__
+
+class KeyboardButtonRequestChat:
+    def __init__(self, request_id, chat_is_channel,chat_is_forum=None,chat_has_username=None,chat_is_created=None,
+                 user_administrator_rights:ChatAdministratorRights=None,bot_administrator_rights:ChatAdministratorRights=None,
+                 bot_is_member=None):
+        self.request_id = request_id
+        self.user_is_bot = chat_is_channel
+        self.chat_is_forum = chat_is_forum
+        self.chat_has_username = chat_has_username
+        self.chat_is_created = chat_is_created
+        self.user_administrator_rights = user_administrator_rights.dict if user_administrator_rights else None
+        self.bot_administrator_rights = bot_administrator_rights.dict if bot_administrator_rights else None
+        self.bot_is_member = bot_is_member
+
+    @property
+    def dict(self):
+        return self.__dict__
+
+class KeyboardButtonPollType:
+    def __init__(self,type=None):
+        self.type = type
+
+    @property
+    def dict(self):
+        return self.__dict__
+
+class KeyboardButton:
+    def __init__(self,text,request_user:KeyboardButtonRequestUser=None,request_chat:KeyboardButtonRequestChat=None,
+                 request_contact=None,request_location=None,request_poll:KeyboardButtonPollType=None,web_app:WebAppInfo=None):
+        self.text = text
+        self.request_user = request_user.dict if request_user else None
+        self.request_chat =request_chat.dict if request_chat else None
+        self.request_contact = request_contact
+        self.request_location =request_location
+        self.request_poll = request_poll.dict if request_poll else None
+        self.web_app = web_app.dict if web_app else None
+
+    @property
+    def dict(self):
+        return self.__dict__
+
+
+class ReplyKeyboardMarkup:
+    def __init__(self, keyboard, is_persistent=None,resize_keyboard=None,one_time_keyboard=None,
+                 input_field_placeholder=None,selective=None):
+        self.keyboard = [r.dict for r in keyboard]
+        self.is_persistent = is_persistent
+        self.resize_keyboard = resize_keyboard
+        self.one_time_keyboard = one_time_keyboard
+        self.input_field_placeholder = input_field_placeholder
+        self.selective =selective
+
+    @property
+    def dict(self):
+        return self.__dict__
+
+class ReplyKeyboardRemove:
+    def __init__(self,remove_keyboard,selective=None):
+        self.selective = selective
+        self.remove_keyboard = remove_keyboard
+
+    @property
+    def dict(self):
+        return self.__dict__
 
 class ChatMember:
     def __init__(self, data):
         self.original_data = deepcopy(data)
         self.__unpack(data)
 
     def __unpack(self, data):
```

### Comparing `tg-botting-2.1.1/tg_botting/permissions.py` & `tg-botting-2.1.2/tg_botting/permissions.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.1/tg_botting/user.py` & `tg-botting-2.1.2/tg_botting/user.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.1/tg_botting/utils.py` & `tg-botting-2.1.2/tg_botting/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from inspect import isawaitable
 import json
 
 
 
+
 async def async_all(gen, *, check=isawaitable):
     for elem in gen:
         if check(elem):
             elem = await elem
         if not elem:
             return False
     return True
```

### Comparing `tg-botting-2.1.1/tg_botting/view.py` & `tg-botting-2.1.2/tg_botting/view.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.1/tg_botting.egg-info/PKG-INFO` & `tg-botting-2.1.2/tg_botting.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-botting
-Version: 2.1.1
+Version: 2.1.2
 Summary: A basic package for building async TG bots
 Home-page: https://github.com/2sweetheart2/tg_botting
 Author: Sweetie (Roma Fomkin)
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `tg-botting-2.1.1/tg_botting.egg-info/SOURCES.txt` & `tg-botting-2.1.2/tg_botting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

