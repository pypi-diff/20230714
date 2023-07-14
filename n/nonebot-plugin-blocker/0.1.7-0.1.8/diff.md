# Comparing `tmp/nonebot-plugin-blocker-0.1.7.tar.gz` & `tmp/nonebot-plugin-blocker-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-blocker-0.1.7.tar", last modified: Mon Jul 10 20:07:14 2023, max compression
+gzip compressed data, was "nonebot-plugin-blocker-0.1.8.tar", last modified: Fri Jul 14 12:04:28 2023, max compression
```

## Comparing `nonebot-plugin-blocker-0.1.7.tar` & `nonebot-plugin-blocker-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:07:14.371394 nonebot-plugin-blocker-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-10 20:07:14.367393 nonebot-plugin-blocker-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-10 20:06:57.000000 nonebot-plugin-blocker-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:07:14.367393 nonebot-plugin-blocker-0.1.7/nonebot_plugin_blocker/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-10 20:06:57.000000 nonebot-plugin-blocker-0.1.7/nonebot_plugin_blocker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-10 20:06:57.000000 nonebot-plugin-blocker-0.1.7/nonebot_plugin_blocker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-10 20:06:57.000000 nonebot-plugin-blocker-0.1.7/nonebot_plugin_blocker/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:07:14.367393 nonebot-plugin-blocker-0.1.7/nonebot_plugin_blocker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-10 20:07:14.000000 nonebot-plugin-blocker-0.1.7/nonebot_plugin_blocker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-10 20:07:14.000000 nonebot-plugin-blocker-0.1.7/nonebot_plugin_blocker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 20:07:14.000000 nonebot-plugin-blocker-0.1.7/nonebot_plugin_blocker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-10 20:07:14.000000 nonebot-plugin-blocker-0.1.7/nonebot_plugin_blocker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 20:07:14.000000 nonebot-plugin-blocker-0.1.7/nonebot_plugin_blocker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-10 20:06:57.000000 nonebot-plugin-blocker-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 20:07:14.371394 nonebot-plugin-blocker-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:04:28.575801 nonebot-plugin-blocker-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-14 12:04:28.575801 nonebot-plugin-blocker-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-14 12:04:07.000000 nonebot-plugin-blocker-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:04:28.575801 nonebot-plugin-blocker-0.1.8/nonebot_plugin_blocker/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-14 12:04:07.000000 nonebot-plugin-blocker-0.1.8/nonebot_plugin_blocker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-14 12:04:07.000000 nonebot-plugin-blocker-0.1.8/nonebot_plugin_blocker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-14 12:04:07.000000 nonebot-plugin-blocker-0.1.8/nonebot_plugin_blocker/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:04:28.575801 nonebot-plugin-blocker-0.1.8/nonebot_plugin_blocker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-14 12:04:28.000000 nonebot-plugin-blocker-0.1.8/nonebot_plugin_blocker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-14 12:04:28.000000 nonebot-plugin-blocker-0.1.8/nonebot_plugin_blocker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:04:28.000000 nonebot-plugin-blocker-0.1.8/nonebot_plugin_blocker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-14 12:04:28.000000 nonebot-plugin-blocker-0.1.8/nonebot_plugin_blocker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-14 12:04:28.000000 nonebot-plugin-blocker-0.1.8/nonebot_plugin_blocker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-14 12:04:07.000000 nonebot-plugin-blocker-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 12:04:28.575801 nonebot-plugin-blocker-0.1.8/setup.cfg
```

### Comparing `nonebot-plugin-blocker-0.1.7/PKG-INFO` & `nonebot-plugin-blocker-0.1.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-blocker
-Version: 0.1.7
+Version: 0.1.8
 Summary: Message Blocker
 Author-email: MerCuJerry <mercujerry@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/MerCuJerry/nonebot-plugin-blocker
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
 
@@ -76,7 +76,9 @@
 ## 💬 指令
 
 指令只有管理员，群主以及Bot的SUPERUSER能够使用
 
 ### .bot on在该群开启bot
 
 ### .bot off在该群关闭bot
+
+### 在上述指令后at特定bot将关闭使用了本插件的特定Bot，不会影响使用本插件的其他Bot
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.1.7 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.1.8 Summary:
 Message Blocker Author-email: MerCuJerry
 gmail.com> License: MIT Project-URL: homepage, https://github.com/MerCuJerry/
 nonebot-plugin-blocker Requires-Python: <4.0,>=3.8 Description-Content-Type:
 text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
   # nonebot-plugin-blocker _â¨ NoneBot Plugin Blocker â¨_ [license] [pypi]
@@ -15,8 +15,9 @@
 `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
 ["nonebot-plugin-blocker"]  ## âï¸ éç½® æä»¶çéç½®æä»¶ä½äº `data/
 blocker/blocker_reply.json` é ```jsonc { "reply_on":{ "type":"text" "data":
 { "text":"å¨æ¬ç¾¤å¼å¯" } }, "reply_off":{ "type":"text" "data":{ "text":
 "å¨æ¬ç¾¤å³é­" } } } ``` `data/blocker/blocklist.json`
 éæ¯å·²ç»è®¾ç½®å³é­Botçç¾¤å·ï¼å¯ä»¥å¨å³é­nonebotä¹åæå¨ç¼è¾
 ## ð¬ æä»¤ æä»¤åªæç®¡çåï¼ç¾¤ä¸»ä»¥åBotçSUPERUSERè½å¤ä½¿ç¨
-### .bot onå¨è¯¥ç¾¤å¼å¯bot ### .bot offå¨è¯¥ç¾¤å³é­bot
+### .bot onå¨è¯¥ç¾¤å¼å¯bot ### .bot offå¨è¯¥ç¾¤å³é­bot ###
+å¨ä¸è¿°æä»¤åatç¹å®botå°å³é­ä½¿ç¨äºæ¬æä»¶çç¹å®Botï¼ä¸ä¼å½±åä½¿ç¨æ¬æä»¶çå¶ä»Bot
```

### Comparing `nonebot-plugin-blocker-0.1.7/README.md` & `nonebot-plugin-blocker-0.1.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -65,8 +65,10 @@
 
 ## 💬 指令
 
 指令只有管理员，群主以及Bot的SUPERUSER能够使用
 
 ### .bot on在该群开启bot
 
-### .bot off在该群关闭bot
+### .bot off在该群关闭bot
+
+### 在上述指令后at特定bot将关闭使用了本插件的特定Bot，不会影响使用本插件的其他Bot
```

#### html2text {}

```diff
@@ -10,8 +10,9 @@
 `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
 ["nonebot-plugin-blocker"]  ## âï¸ éç½® æä»¶çéç½®æä»¶ä½äº `data/
 blocker/blocker_reply.json` é ```jsonc { "reply_on":{ "type":"text" "data":
 { "text":"å¨æ¬ç¾¤å¼å¯" } }, "reply_off":{ "type":"text" "data":{ "text":
 "å¨æ¬ç¾¤å³é­" } } } ``` `data/blocker/blocklist.json`
 éæ¯å·²ç»è®¾ç½®å³é­Botçç¾¤å·ï¼å¯ä»¥å¨å³é­nonebotä¹åæå¨ç¼è¾
 ## ð¬ æä»¤ æä»¤åªæç®¡çåï¼ç¾¤ä¸»ä»¥åBotçSUPERUSERè½å¤ä½¿ç¨
-### .bot onå¨è¯¥ç¾¤å¼å¯bot ### .bot offå¨è¯¥ç¾¤å³é­bot
+### .bot onå¨è¯¥ç¾¤å¼å¯bot ### .bot offå¨è¯¥ç¾¤å³é­bot ###
+å¨ä¸è¿°æä»¤åatç¹å®botå°å³é­ä½¿ç¨äºæ¬æä»¶çç¹å®Botï¼ä¸ä¼å½±åä½¿ç¨æ¬æä»¶çå¶ä»Bot
```

### Comparing `nonebot-plugin-blocker-0.1.7/nonebot_plugin_blocker/__main__.py` & `nonebot-plugin-blocker-0.1.8/nonebot_plugin_blocker/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,40 +10,42 @@
 from nonebot.matcher import Matcher
 import re
 from nonebot.message import run_preprocessor
 from .config import BlockerList
 
 blockerlist: BlockerList
 
-blocker = on_regex(r"^[.。]bot (on|off)$",permission= GROUP_ADMIN | GROUP_OWNER | SUPERUSER, priority=2,block=True)
+blocker = on_regex(r"^[.。]bot (on|off)\s?(|\[at:qq=\d+\])$", permission=GROUP_ADMIN | GROUP_OWNER | SUPERUSER, priority=2, block=True)
 
 @driver.on_startup
 async def load_blocker_on_start():
     global blockerlist
     blockerlist = BlockerList()
 
 @driver.on_shutdown
 async def save_blocker_on_shut():
     global blockerlist
     del blockerlist
 
 @run_preprocessor
 async def blocker_hook(matcher: Matcher,event: GroupMessageEvent):
-    if blockerlist.check_blocker(event.group_id, event.self_id) and re.match('[.。]bot (on|off)',event.get_plaintext()) is None:
-        logger.info("[Blocker]Your Message is Blocked By Blocker.")
+    if blockerlist.check_blocker(event.group_id, event.self_id) and re.match('^[.。]bot (on|off)', event.get_plaintext()) is None:
+        logger.info('[Blocker]Your Message is Blocked By Blocker.')
         await matcher.finish()
         
 @blocker.handle()
 async def blocker_msg_handle(matcher: Matcher,event: GroupMessageEvent):
+    if event.get_plaintext().find('qq') != -1 and event.is_tome() is True:
+        await matcher.finish()
     if event.get_plaintext().find('on') != -1:
-        msg_type , msg_data = blockerlist.get_on_reply()
+        msg_type, msg_data = blockerlist.get_on_reply()
         blockerlist.del_blocker(event.group_id, event.self_id)
-        logger.info("[Blocker]Delete Blocker Successful.")
+        logger.info('[Blocker]Delete Blocker Successful.')
         if msg_type is None:
             await matcher.finish('在本群开启')
     elif event.get_plaintext().find('off') != -1:
-        msg_type , msg_data = blockerlist.get_off_reply()
+        msg_type, msg_data = blockerlist.get_off_reply()
         blockerlist.add_blocker(event.group_id, event.self_id)
-        logger.info("[Blocker]Add Blocker Successful.")
+        logger.info('[Blocker]Add Blocker Successful.')
         if msg_type is None:
             await matcher.finish('在本群关闭')
-    await matcher.finish(MessageSegment(type=msg_type,data=msg_data))
+    await matcher.finish(MessageSegment(type=msg_type, data=msg_data))
```

### Comparing `nonebot-plugin-blocker-0.1.7/nonebot_plugin_blocker/config.py` & `nonebot-plugin-blocker-0.1.8/nonebot_plugin_blocker/config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-blocker-0.1.7/nonebot_plugin_blocker.egg-info/PKG-INFO` & `nonebot-plugin-blocker-0.1.8/nonebot_plugin_blocker.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-blocker
-Version: 0.1.7
+Version: 0.1.8
 Summary: Message Blocker
 Author-email: MerCuJerry <mercujerry@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/MerCuJerry/nonebot-plugin-blocker
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
 
@@ -76,7 +76,9 @@
 ## 💬 指令
 
 指令只有管理员，群主以及Bot的SUPERUSER能够使用
 
 ### .bot on在该群开启bot
 
 ### .bot off在该群关闭bot
+
+### 在上述指令后at特定bot将关闭使用了本插件的特定Bot，不会影响使用本插件的其他Bot
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.1.7 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.1.8 Summary:
 Message Blocker Author-email: MerCuJerry
 gmail.com> License: MIT Project-URL: homepage, https://github.com/MerCuJerry/
 nonebot-plugin-blocker Requires-Python: <4.0,>=3.8 Description-Content-Type:
 text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
   # nonebot-plugin-blocker _â¨ NoneBot Plugin Blocker â¨_ [license] [pypi]
@@ -15,8 +15,9 @@
 `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
 ["nonebot-plugin-blocker"]  ## âï¸ éç½® æä»¶çéç½®æä»¶ä½äº `data/
 blocker/blocker_reply.json` é ```jsonc { "reply_on":{ "type":"text" "data":
 { "text":"å¨æ¬ç¾¤å¼å¯" } }, "reply_off":{ "type":"text" "data":{ "text":
 "å¨æ¬ç¾¤å³é­" } } } ``` `data/blocker/blocklist.json`
 éæ¯å·²ç»è®¾ç½®å³é­Botçç¾¤å·ï¼å¯ä»¥å¨å³é­nonebotä¹åæå¨ç¼è¾
 ## ð¬ æä»¤ æä»¤åªæç®¡çåï¼ç¾¤ä¸»ä»¥åBotçSUPERUSERè½å¤ä½¿ç¨
-### .bot onå¨è¯¥ç¾¤å¼å¯bot ### .bot offå¨è¯¥ç¾¤å³é­bot
+### .bot onå¨è¯¥ç¾¤å¼å¯bot ### .bot offå¨è¯¥ç¾¤å³é­bot ###
+å¨ä¸è¿°æä»¤åatç¹å®botå°å³é­ä½¿ç¨äºæ¬æä»¶çç¹å®Botï¼ä¸ä¼å½±åä½¿ç¨æ¬æä»¶çå¶ä»Bot
```

