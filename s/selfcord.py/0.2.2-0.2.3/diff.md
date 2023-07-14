# Comparing `tmp/selfcord.py-0.2.2.tar.gz` & `tmp/selfcord.py-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selfcord.py-0.2.2.tar", last modified: Fri Jun 30 22:49:39 2023, max compression
+gzip compressed data, was "selfcord.py-0.2.3.tar", last modified: Fri Jul 14 16:54:38 2023, max compression
```

## Comparing `selfcord.py-0.2.2.tar` & `selfcord.py-0.2.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:49:39.103731 selfcord.py-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-06-30 22:49:39.103731 selfcord.py-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:49:39.103731 selfcord.py-0.2.2/selfcord/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:49:39.103731 selfcord.py-0.2.2/selfcord/api/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/api/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    18394 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/api/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    23063 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/api/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    10865 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/api/http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:49:39.103731 selfcord.py-0.2.2/selfcord/api/voice/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/api/voice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/api/voice/voice.py
--rw-r--r--   0 runner    (1001) docker     (123)    28870 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:49:39.103731 selfcord.py-0.2.2/selfcord/models/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29311 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/models/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/models/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/models/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)    12092 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/models/guild.py
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/models/interactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/models/member.py
--rw-r--r--   0 runner    (1001) docker     (123)    10729 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/models/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/models/permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/models/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/models/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/models/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:49:39.103731 selfcord.py-0.2.2/selfcord/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17065 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/utils/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/selfcord/utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:49:39.103731 selfcord.py-0.2.2/selfcord.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-06-30 22:49:39.000000 selfcord.py-0.2.2/selfcord.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-30 22:49:39.000000 selfcord.py-0.2.2/selfcord.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 22:49:39.000000 selfcord.py-0.2.2/selfcord.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-30 22:49:39.000000 selfcord.py-0.2.2/selfcord.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 22:49:39.000000 selfcord.py-0.2.2/selfcord.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 22:49:39.103731 selfcord.py-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:49:39.103731 selfcord.py-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-30 22:49:28.000000 selfcord.py-0.2.2/tests/test_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:54:38.771494 selfcord.py-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-07-14 16:54:38.771494 selfcord.py-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:54:38.767494 selfcord.py-0.2.3/selfcord/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:54:38.767494 selfcord.py-0.2.3/selfcord/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/api/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21098 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/api/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23084 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/api/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10865 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/api/http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:54:38.767494 selfcord.py-0.2.3/selfcord/api/voice/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/api/voice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/api/voice/voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29153 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:54:38.771494 selfcord.py-0.2.3/selfcord/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29691 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/models/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/models/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/models/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12092 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/models/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/models/interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/models/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11281 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/models/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/models/permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/models/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/models/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/models/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:54:38.771494 selfcord.py-0.2.3/selfcord/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17064 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/utils/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/selfcord/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:54:38.767494 selfcord.py-0.2.3/selfcord.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-07-14 16:54:38.000000 selfcord.py-0.2.3/selfcord.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-14 16:54:38.000000 selfcord.py-0.2.3/selfcord.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:54:38.000000 selfcord.py-0.2.3/selfcord.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-14 16:54:38.000000 selfcord.py-0.2.3/selfcord.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 16:54:38.000000 selfcord.py-0.2.3/selfcord.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 16:54:38.771494 selfcord.py-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:54:38.771494 selfcord.py-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-14 16:54:13.000000 selfcord.py-0.2.3/tests/test_commands.py
```

### Comparing `selfcord.py-0.2.2/LICENSE` & `selfcord.py-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.2/PKG-INFO` & `selfcord.py-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selfcord.py
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Discord API wrapper designed for selfbots!
 Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell
 License: MIT
 Keywords: selfbot,discord,discordapi,discordwrapper
 Description-Content-Type: text/markdown
 Provides-Extra: voice
@@ -16,15 +16,15 @@
 <strong><i>A Powerful Library for Discord Selfbots</i></strong>
 <br>
 <br>
 <a href="https://www.python.org/">
 <img src="https://img.shields.io/badge/MADE%20WITH-PYTHON-red?logoColor=red&logo=Python&style=for-the-badge">
 </a>
 <a href="https://pypi.org/project/selfcord/">
-<img src="https://img.shields.io/badge/version-0.2.2-blue?logo=adguard&style=for-the-badge">
+<img src="https://img.shields.io/badge/version-0.2.3-blue?logo=adguard&style=for-the-badge">
 </a>
 <a href="https://github.com/Shell1010/Selfcord/wiki">
 <img src="https://img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge">
 </a>
 </div>
 
 ## Feautres
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: selfcord.py Version: 0.2.2 Summary: A Discord API
+Metadata-Version: 2.1 Name: selfcord.py Version: 0.2.3 Summary: A Discord API
 wrapper designed for selfbots! Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell License: MIT Keywords: selfbot,discord,discordapi,discordwrapper
 Description-Content-Type: text/markdown Provides-Extra: voice License-File:
 LICENSE
                                  [./logo.png]
                             ****** SELFCORD ******
                    A Powerful Library for Discord Selfbots
 
                [https://img.shields.io/badge/MADE%20WITH-PYTHON-
   red?logoColor=red&logo=Python&style=for-the-badge] [https://img.shields.io/
-     badge/version-0.2.2-blue?logo=adguard&style=for-the-badge] [https://
+     badge/version-0.2.3-blue?logo=adguard&style=for-the-badge] [https://
   img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge]
 ## Feautres - Modern Pythonic API using `async`/`await` syntax - Easy to use
 with an object oriented design - Optimised for both speed and memory - Prevents
 detection of user account automation - Clean Documentation - Community Support
 ## Installation Python 3.10 or higher is required. ``` pip install selfcord.py
 ``` ## Wiki Read our [Wiki](https://github.com/Shell1010/Selfcord/wiki) in
 regards to documentation and getting started. ## Getting Started A selfbot that
```

### Comparing `selfcord.py-0.2.2/README.md` & `selfcord.py-0.2.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 <strong><i>A Powerful Library for Discord Selfbots</i></strong>
 <br>
 <br>
 <a href="https://www.python.org/">
 <img src="https://img.shields.io/badge/MADE%20WITH-PYTHON-red?logoColor=red&logo=Python&style=for-the-badge">
 </a>
 <a href="https://pypi.org/project/selfcord/">
-<img src="https://img.shields.io/badge/version-0.2.2-blue?logo=adguard&style=for-the-badge">
+<img src="https://img.shields.io/badge/version-0.2.3-blue?logo=adguard&style=for-the-badge">
 </a>
 <a href="https://github.com/Shell1010/Selfcord/wiki">
 <img src="https://img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge">
 </a>
 </div>
 
 ## Feautres
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
                                  [./logo.png]
                             ****** SELFCORD ******
                    A Powerful Library for Discord Selfbots
 
                [https://img.shields.io/badge/MADE%20WITH-PYTHON-
   red?logoColor=red&logo=Python&style=for-the-badge] [https://img.shields.io/
-     badge/version-0.2.2-blue?logo=adguard&style=for-the-badge] [https://
+     badge/version-0.2.3-blue?logo=adguard&style=for-the-badge] [https://
   img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge]
 ## Feautres - Modern Pythonic API using `async`/`await` syntax - Easy to use
 with an object oriented design - Optimised for both speed and memory - Prevents
 detection of user account automation - Clean Documentation - Community Support
 ## Installation Python 3.10 or higher is required. ``` pip install selfcord.py
 ``` ## Wiki Read our [Wiki](https://github.com/Shell1010/Selfcord/wiki) in
 regards to documentation and getting started. ## Getting Started A selfbot that
```

### Comparing `selfcord.py-0.2.2/selfcord/api/errors.py` & `selfcord.py-0.2.3/selfcord/api/errors.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.2/selfcord/api/events.py` & `selfcord.py-0.2.3/selfcord/api/events.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,17 @@
     async def handle_ready(self, data: dict, user: Client, http: http):
         """Handles what happens when the ready event is fired, when the bot first connects
 
         Args:
             data (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
+
+        Usage:
+            @bot.on("ready")
         """
         self.user = user
         for relationship in data.get("relationships"):
             if relationship.get("type") == 1:
                 self.user.friends.append(User(relationship["user"], self.bot, http))
 
         for channel in data.get("private_channels"):
@@ -63,28 +66,34 @@
     async def handle_guild_create(self, data: dict, user: Client, http: http):
         """Handles what happens when a guild is created
 
         Args:
             data (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
+
+        Usage:
+            @bot.on("guild_create")
         """
         self.user = user
         guild = Guild(data, self.bot, http)
         self.user.guilds.append(guild)
 
         # Sends data from ready to the event handler in main.py (if it exists)
         await self.bot.emit("guild_create", guild)
 
     async def handle_message_create(self, data: dict, user: Client, http: http):
         """Handles what happens when a message is created, or sent
         Args:
             data (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
+
+        Usage:
+            @bot.on("message")
         """
         self.user = user
         message = Message(data, self.bot, http)
         self.user.messages.append(message)
 
         # Sends data from ready to the event handler in main.py (if it exists)
         await self.bot.emit("message", message)
@@ -103,14 +112,17 @@
     async def handle_message_delete(self, data: dict, user: Client, http: http):
         """Handles what happens when a message is deleted. Very little data will be logged if the message is not in the bots cache.
 
         Args:
             data (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
+
+        Usage:
+            @bot.on("message_delete")
         """
         self.user = user
         id = data.get("id")
         for message in self.user.messages:
             if message.id == id:
                 setattr(message, "deleted_time", time.time())
                 await self.bot.emit("message_delete", message)
@@ -142,14 +154,17 @@
     async def handle_channel_create(self, channel: dict, user: Client, http: http):
         """Handles what happens when a channel is created
 
         Args:
             channel (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
+
+        Usage:
+            @bot.on("channel_create")
         """
         self.user = user
         if channel.get("type") == 0 or channel.get("type") not in [1, 2, 3]:
             id = channel.get("guild_id")
             for guild in self.user.guilds:
                 if guild.id == id:
                     channel = TextChannel(channel, self.bot, self.http)
@@ -180,14 +195,17 @@
     ):
         """Handles what happens when a member chunk payload is received
 
         Args:
             data (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
+
+        Usage:
+            @bot.on("member_chunk")
         """
         self.user = user
         ops = []
         data = data["ops"]
         for main in data:
             op = main["op"]
             ops.append(op)
@@ -243,14 +261,17 @@
     async def handle_channel_delete(self, data, user: Client, http: http):
         """Handles what happens when a channel is deleted
 
         Args:
             data (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
+
+        Usage:
+            @bot.on("channel_delete")
         """
         self.user = user
         id = data.get("id")
         for channel in self.user.private_channels:
             if channel.id == id:
                 await self.bot.emit("channel_delete", channel)
                 self.user.private_channels.remove(channel)
@@ -276,14 +297,17 @@
     async def handle_guild_role_create(self, data: dict, user: Client, http: http):
         """Handles what happens when a role is created
 
         Args:
             data (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
+
+        Usage:
+            @bot.on("role_create")
         """
         self.user = user
 
         for guild in self.user.guilds:
             if data.get("guild_id") == guild.id:
                 role = Role(data, self.bot, self.http, guild_id=guild.id)
                 guild.roles.append(role)
@@ -293,67 +317,107 @@
     async def handle_guild_role_delete(self, role: dict, user: Client, http: http):
         """Handles what happens when a role is deleted
 
         Args:
             data (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
+
+        Usage:
+            @bot.on("role_delete")
         """
         self.user = user
 
         for guild in self.user.guilds:
             if role.get("guild_id") == guild.id:
                 for role in guild.roles:
                     if role.get("id") == role.id:
                         await self.bot.emit("role_delete", role)
                         guild.roles.remove(role)
                         return
 
     async def handle_call_update(self, data: dict, user: Client, http: http):
+        """Handles what happens when a voice call is updated
+
+        Args:
+            data (dict): JSON data from gateway
+            user (Client): The client instance
+            http (http): HTTP instance
+
+        Usage:
+            @bot.on("call_update")
+        """
         channel = self.bot.get_channel(data["channel_id"])
         region = data.get("region")
         if isinstance(channel, DMChannel):
             users = channel.recipient
         elif isinstance(channel, GroupChannel):
             users = channel.recipients
 
         await self.bot.emit("call_update", channel, users, region)
 
     async def handle_call_create(self, data: dict, user: Client, http: http):
+        """Handles what happens when a voice call is created
+
+        Args:
+            data (dict): JSON data from gateway
+            user (Client): The client instance
+            http (http): HTTP instance
+
+        Usage:
+            @bot.on("call_create")
+        """
         channel = self.bot.get_channel(data["channel_id"])
         region = data.get("region")
         if isinstance(channel, DMChannel):
             users = channel.recipient
         elif isinstance(channel, GroupChannel):
             users = channel.recipients
 
         await self.bot.emit("call_create", channel, users, region)
 
     async def handle_call_delete(self, data: dict, user: Client, http: http):
+        """Handles what happens when a voice call is ended
+
+        Args:
+            data (dict): JSON data from gateway
+            user (Client): The client instance
+            http (http): HTTP instance
+
+        Usage:
+            @bot.on("call_delete")
+        """
         channel = self.bot.get_channel(data["channel_id"])
         await self.bot.emit("call_delete", channel)
 
     async def handle_voice_state_update(self, data: dict, user: Client, http: http):
         """Handles the voice state updating
 
         Args:
             data (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
+
+        Usage:
+            @bot.on("voice_state_update")
         """
         if data["channel_id"] != None:
             self.session_id = data["session_id"]
+            await self.bot.emit("voice_state_update")
 
     async def handle_presence_update(self, data: dict, user: Client, http: http):
         """Handles the presence updating
 
         Args:
             data (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
+
+        Usage:
+            @bot.on("presence_update")
         """
         LISTENING = 2
         CUSTOM = 4
 
         last_modified = data.get("last_modified")
         status = data.get("status")
         check = data.get("user").get("username")
@@ -388,14 +452,15 @@
     async def handle_voice_server_update(self, data: dict, user: Client, http: http):
         """Handles the voice server updating
 
         Args:
             data (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
+
         """
         self.token = data["token"]
         self.endpoint = data["endpoint"]
         if data["guild_id"] is None:
             self.server_id = data["channel_id"]
         else:
             self.server_id = data["guild_id"]
@@ -422,14 +487,17 @@
     async def handle_relationship_add(self, data: dict, user: Client, http: http):
         """Handles relationships being added
 
         Args:
             data (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
+
+        Usage:
+            @bot.on("relationship_add")
         """
         types = {
             "NONE": 0,
             "FRIEND": 1,
             "BLOCKED": 2,
             "PENDING_INCOMING": 3,
             "PENDING_OUTGOING": 4,
@@ -444,28 +512,34 @@
     async def handle_sessions_replace(self, data: list[dict], user: Client, http: http):
         """Handles sessions being created/removed. Used to log initial data.
 
         Args:
             data (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
+
+        Usage:
+            @bot.on("session")
         """
     
         sessions = [Event_Session(session, self.bot, self.http) for session in data]
         await self.bot.emit("session", sessions)
         
 
 
     async def handle_relationship_remove(self, data: dict, user: Client, http: http):
         """Handles relationships being removed
 
         Args:
             data (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
+
+        Usage:
+            @bot.on("relationship_remove")
         """
         types = {
             "NONE": 0,
             "FRIEND": 1,
             "BLOCKED": 2,
             "PENDING_INCOMING": 3,
             "PENDING_OUTGOING": 4,
@@ -474,25 +548,59 @@
         id = data['id']
         since = data['since']
         for type, value in types.items():
             if data.get("type") == value:
                 rs_type = type
         await self.bot.emit("relationship_remove", id, rs_type, since)
 
+    async def handle_channel_recipient_add(self, data: dict, user: Client, http: http):
+        """Handles relationships being removed
+
+        Args:
+            data (dict): JSON data from gateway
+            user (Client): The client instance
+            http (http): HTTP instance
+
+        Usage:
+            @bot.on("group_add")
+        """
+        person = User(data.get('user'), self.bot, self.http)
+        channel = self.bot.get_channel(data.get("channel_id"))
+        await self.bot.emit("group_add", channel, person)
+
+    async def handle_channel_recipient_remove(self, data: dict, user: Client, http: http):
+        """Handles relationships being removed
+
+        Args:
+            data (dict): JSON data from gateway
+            user (Client): The client instance
+            http (http): HTTP instance
+
+        Usage:
+            @bot.on("group_remove")
+        """
+        person = User(data.get('user'), self.bot, self.http)
+        channel = self.bot.get_channel(data.get("channel_id"))
+        await self.bot.emit("group_remove", channel, person)
+
+    
+
     async def handle_interaction_modal_create(self, data: dict, user: Client, http: http):
         """Handles when a text input modal is Created
 
          Args:
             data (dict): JSON data from gateway
             user (Client): The client instance
             http (http): HTTP instance
+
+        Usage:
+            @bot.on("modal_create")
         """
         components = data['components'] if data.get("components") is not None else []
         new_comps = []
-        print(data['id'])
         for component in components:
             if component['type'] == 1:
                 for comp in component['components']:
                     if comp['type'] == 4:
                         text = Text_Input(comp, self.bot, self.http)
                         setattr(text, "id", data['id'])
                         new_comps.append(text)
```

### Comparing `selfcord.py-0.2.2/selfcord/api/gateway.py` & `selfcord.py-0.2.3/selfcord/api/gateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -333,25 +333,25 @@
         if item:
             if self.fired:
                 log.info(f"{item}")
             try:
                 item = self.zlib.decompress(item)
             except Exception as e:
                 log.error(f"Could not decompress\n{e}")
-                await self.close()
-                await self.connect()
+                return
             item = ujson.loads(item)  # Get json message from gateway
 
             op = item.get("op")  # Op code
             data = item.get("d")  # Data
             event = item.get("t")  # The event
-            s = item.get("s")
             if op == self.RECONNECT:
                 await self.close()
-                await self.reconnect(s)
+                log.info(f"DATA: {data}\nOP: {op}\nEVENT: {event}")
+                await asyncio.sleep(10)
+                await self.connect()
                 self.fired = True
                 log.error("Reconnect websocket")
 
             elif op == self.INVALIDATE_SESSION:
                 if data:
                     await self.close()
                     log.error("Session Invalidated")
@@ -469,14 +469,15 @@
 
     async def reconnect(self, seq: int):
         """Reconnect to discord gateway"""
         self.ws = await websockets.connect(
             f"{self.bot.resume_url}?encoding=json&v=9&compress=zlib-stream"
         )
         self.alive = True
+        await asyncio.sleep(1.5)
         payload = {
             "op": 6,
             "d": {"token": self.token, "session_id": self.bot.session_id, "seq": seq},
         }
         await self.send_json(payload)
 
 
@@ -500,15 +501,14 @@
 
     async def identify(self):
         """Identify to gateway, uses amazing mobile client spoof"""
         
         payload = {
             "op": 2,
             "d": {
-                "capabilities": 4079,
                 "token": self.token,
                 "client_state": {
                     "api_code_version": 0,
                     "highest_last_message_id": "0",
                     "initial_guild_id": None,
                     "private_channels_version": "0",
                     "read_state_version": 0,
```

### Comparing `selfcord.py-0.2.2/selfcord/api/http.py` & `selfcord.py-0.2.3/selfcord/api/http.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.2/selfcord/api/voice/voice.py` & `selfcord.py-0.2.3/selfcord/api/voice/voice.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.2/selfcord/bot.py` & `selfcord.py-0.2.3/selfcord/bot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from __future__ import annotations
 
+import ast
 import asyncio
 import contextlib
 import importlib
 import inspect
 import io
 import os
 import random
+import sys
 import time
 import urllib
 from collections import defaultdict
 from traceback import format_exception
 from typing import TYPE_CHECKING
 from urllib.parse import urlparse
 
@@ -189,21 +191,31 @@
 
             def clean_code(content):
                 if content.startswith("```") and content.endswith("```"):
                     return "\n".join(content.split("\n")[1:])[:-3]
                 else:
                     return content
 
+
+
             @self.cmd(description="Executes and runs code", aliases=["exec"])
             async def eval(ctx, *, code):
                 """Runs python code via exec, intended for experienced usage. This can be DANGEROUS if you do not know what you are doing, use with caution."""
-                code = clean_code(code)
+                if code.startswith("```"):
+                    code = clean_code(code)
+                envs = {
+                    "bot": self,
+                    "ctx": ctx,
+                    "selfcord": sys.modules[__name__],
+                    "__import__": __import__
+                }
+                
                 try:
                     with contextlib.redirect_stdout(io.StringIO()) as f:
-                        await aexec(source=code, local=globals() )
+                        await aexec(code, local=envs)
                         result = f"```{f.getvalue()}\n```"
                 except Exception as e:
                     error = "".join(format_exception(e, e, e.__traceback__))
                     result = f"```\n{error}```"
 
                 await ctx.reply(result)
 
@@ -473,15 +485,15 @@
             message_id (str): The message id to search for
 
         Returns:
             Message: The Message object
         """
         for message in self.user.messages:
             if message.id == message_id:
-                return Message
+                return message
 
     def get_channel(self, channel_id: str):
         """
         Function to help retrieve channel from bot cache
 
         Args:
             channel_id (str): The channel id to search for
```

### Comparing `selfcord.py-0.2.2/selfcord/models/channel.py` & `selfcord.py-0.2.3/selfcord/models/channel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import asyncio
 import os
 import random
 import time
+from io import BytesIO
 from traceback import format_exception
 from typing import TYPE_CHECKING
 
 import aiofiles
 import aiohttp
 from aioconsole import aprint
 
@@ -46,27 +47,14 @@
         after: float | None = None,
         offset: int | None = None,
         pinned: bool | None = None
         ):
         """
         Search through channel with specific parameters
 
-        Args:
-            content (str) : Content to search for.
-            author (str) : Author to search for.
-            mentions (str) : Mention to search for.
-            has (str) : Message that contains (file, image, video, etc).
-            before (time) : Before a timestamp.
-            after (time) : After a timestamp.
-            offset (int) : How many messages after to search.
-
-        Returns:
-            total (int) : Total amount of messages possible of receiving.
-            messages (list[Message]) : List of message objects gathered
-
         """
         url = f"/channels/{self.id}/messages/search"
         params = {
             "content": content,
             "author_id": author,
             "mentions": mentions,
             "has": has,
@@ -148,41 +136,64 @@
                     if msg.author == self.bot.user:
                         messages.append(msg)
             if len(messages) >= amount:
                 break
 
         return messages
 
-    async def upload_image(self, paths: list[str]) -> list[dict[str, int | str]]:
+    async def upload_image(self, paths: list) -> list[dict[str, int | str]]:
         files = []
         id = 0
         for path in paths:
-            async with aiofiles.open(path, "rb") as f:
-                file = await f.read()
-                size = len(file)
-                name = os.path.basename(path)
-            files.append({"file_size" : size, "filename": f"{name}", "id": id})
+            if isinstance(path, (bytearray, bytes)):
+                files.append({
+                    "file_size": len(path),
+                    "filename": f"{random.randint(1, 25555)}.png", 
+                    "id": id
+                })
+            elif isinstance(path, BytesIO):
+                files.append({
+                    "file_size": path.getbuffer().nbytes,
+                    "filename": f"{random.randint(1, 25555)}.png", 
+                    "id": id
+                })
+            else:
+                async with aiofiles.open(path, "rb") as f:
+                    file = await f.read()
+                    size = len(file)
+                    name = os.path.basename(path)
+                files.append({"file_size" : size, "filename": f"{name}", "id": id})
             id += 1
 
         json = await self.http.request("post", f"/channels/{self.id}/attachments", json={"files": files})
 
         items = []
         for key, atch in enumerate(json['attachments']):
             upload_url = atch['upload_url']
             id = atch['id']
             upload_filename = atch['upload_filename']
             async with aiohttp.ClientSession() as session:
-                async with aiofiles.open(paths[key], "rb") as f:
-                    file = await f.read()
+                if isinstance(paths[key], BytesIO):
+                    file = paths[key].getvalue()
+                elif isinstance(paths[key], (bytes, bytearray)):
+                    file = paths[key]
+                else:
+                    async with aiofiles.open(paths[key], "rb") as f:
+                        file = await f.read()
                 async with session.put(upload_url, data=file): 
                     pass
             items.append({"uploaded_filename": upload_filename, "filename": os.path.basename(upload_filename) , "id": id})
         return items
     
     async def delayed_delete(self, message: Message, time: int):
+        """Method to delay a delete of a message
+        
+        Args:
+            message (message) : Message object
+            time (int) : Interval to delete after"""
         await asyncio.sleep(time)
         await message.delete()
     
     
 
     async def purge(self, amount: int = 0) -> None:
         """
@@ -230,15 +241,15 @@
                         for message in msgs[i : i + 3]
                     ),
                 )
                 await asyncio.sleep(0.4)
 
 
 
-    async def spam(self, amount: int, content, file_paths: list[str] = [], tts=False) -> None:
+    async def spam(self, amount: int, content, file_paths: list = [], tts=False) -> None:
         """
         Send multiple of the same message.
 
         Args:
             - amount(int) : Number of spam messages to send.
             - content(str) : The message to send.
             - tts(bool) = False : Specify whether it is a TTS message.
@@ -252,15 +263,15 @@
                 *(
                     asyncio.create_task(self.send(tts=tts, content=content, file_paths=file_paths))
                     for _ in amount[i : i + 3]
                 )
             )
             await asyncio.sleep(0.3)
 
-    async def send(self, content=None, file_paths: list[str] = [], delete_after: int | None = None, tts=False) -> Message:
+    async def send(self, content=None, file_paths: list = [], delete_after: int | None = None, tts=False) -> Message:
         """
         Send a message to the text channel.
 
         Args:
             - content(str) : Message content. Should be string type or similar. Discord `embed` type is not allowed.
             - tts(bool) : Specify whether message is text-to-speech or not
 
@@ -295,15 +306,15 @@
                 json=json
             )
         if delete_after is not None:
             asyncio.create_task(self.delayed_delete(Message(resp, self.bot, self.http), delete_after))
 
         return Message(resp, self.bot, self.http)
 
-    async def reply(self, message: Message, content, file_paths: list[str] = [], delete_after: int | None = None, tts=False) -> Message:
+    async def reply(self, message: Message, content, file_paths: list = [], delete_after: int | None = None, tts=False) -> Message:
         """Reply to a specific message
 
         Args:
             message (str): Message to reply to
             content (_type_, optional): Message content to reply with. Defaults to None.
             tts (bool, optional): Specify whether message is text-to-speech or not. Defaults to False.
```

### Comparing `selfcord.py-0.2.2/selfcord/models/client.py` & `selfcord.py-0.2.3/selfcord/models/client.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.2/selfcord/models/emoji.py` & `selfcord.py-0.2.3/selfcord/models/emoji.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.2/selfcord/models/guild.py` & `selfcord.py-0.2.3/selfcord/models/guild.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.2/selfcord/models/interactions.py` & `selfcord.py-0.2.3/selfcord/models/interactions.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.2/selfcord/models/member.py` & `selfcord.py-0.2.3/selfcord/models/member.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.2/selfcord/models/message.py` & `selfcord.py-0.2.3/selfcord/models/message.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 import logging
 import random
 import time
 import urllib
 from itertools import zip_longest
 from typing import TYPE_CHECKING
 
+import aiofiles
+import ujson
+
 if TYPE_CHECKING:
     from ..api.http import http
     from ..bot import Bot
 
 from .user import User
 
 log = logging.getLogger(__name__)
@@ -239,15 +242,18 @@
 
     async def delete(self):
         """Delete the Message Object"""
         await self.http.request(
             method="delete", endpoint=f"/channels/{self.channel_id}/messages/{self.id}"
         )
 
-    async def edit(self, content: str, file_paths: list[str] = [], delete_after: int | None = None) -> Message:
+    
+         
+                
+    async def edit(self, content: str, file_paths: list = [], delete_after: int | None = None) -> Message:
         """Edits the specified message
 
         Args:
             content (str): Content to edit message to.
         """
         json = { "content":  content }
         if file_paths != []:
@@ -287,7 +293,23 @@
         """
         raw_reaction = urllib.parse.urlencode({"emoji": emoji}).split("emoji=")[1]
         await self.http.request(
             method="put",
             endpoint=f"/channels/{self.channel_id}/messages/{self.id}/reactions/{raw_reaction}/%40me?location=Message&burst=false",
             headers={"referer": f"https://discord.com/channels/@me/{self.channel_id}"},
         )
+
+    async def report(self, breadcrumbs: list = []):
+        await self.http.request(
+            method="post",
+            endpoint="/reporting/message",
+            json={
+                "version": "1.0",
+                "variant": "3",
+                "language": "en",
+                "breadcrumbs": breadcrumbs,
+                "elements": {},
+                "name": "message",
+                "channel_id": self.channel_id,
+                "message_id": self.id
+            }
+        )
```

### Comparing `selfcord.py-0.2.2/selfcord/models/permission.py` & `selfcord.py-0.2.3/selfcord/models/permission.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.2/selfcord/models/role.py` & `selfcord.py-0.2.3/selfcord/models/role.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.2/selfcord/models/sessions.py` & `selfcord.py-0.2.3/selfcord/models/sessions.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.2/selfcord/models/user.py` & `selfcord.py-0.2.3/selfcord/models/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,14 +72,15 @@
             Connected_Account(account) for account in data.get("connected_accounts")
         ]
 
         self.mutual_guilds = [
             self.bot.get_guild(guild["id"]) for guild in data.get("mutual_guilds")
         ]
 
+        
         self.id = data["user"]["id"]
         self.premium_type = data.get("premium_type")
         user_profile = data.get("user_profile")
         try:
             self.emoji = user_profile.get("emoji")
         except:
             self.emoji = None
```

### Comparing `selfcord.py-0.2.2/selfcord/models/webhook.py` & `selfcord.py-0.2.3/selfcord/models/webhook.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.2/selfcord/utils/command.py` & `selfcord.py-0.2.3/selfcord/utils/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import inspect
 import re
 import shlex
 from collections import defaultdict
 from traceback import format_exception
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, get_origin
 
 from .logging import logging
 
 if TYPE_CHECKING:
     from ..api import *
     from ..bot import Bot
     from ..models import *
@@ -382,25 +382,32 @@
         if param.annotation is param.empty:
             return str
         if callable(param.annotation):
             return param.annotation
         else:
             log.error("Parameter annotation must be callable")
 
-    def convert(self, param, value) -> str | Any:
+    async def convert(self, param, value) -> str | Any:
         """Attempts to turn x value in y value, using get_converter func for the values
 
         Args:
             param (_type_): function parameter
             value (_type_): value in message
 
         Returns:
             Type[str]: The type of parameter
         """
+        from ..models import User
         converter = self.get_converter(param)
+        if converter is User:
+            id = re.findall(r"[0-9]{18,19}", value)
+            if len(id) > 0:
+                user = await self.bot.get_user(id[0])
+                return user
+            log.error("You failed to pass valid mention or ID")
         return converter(value)
 
     async def get_arguments(self) -> tuple[list, dict]:
         """Get arguments by checking function arguments and comparing to arguments in message.
 
         Returns:
             _type_: _description_
@@ -415,43 +422,36 @@
         if self.command_content == None:
             return args, kwargs
         sh = shlex.shlex(self.command_content[1:], posix=False)
         sh.whitespace = " "
         sh.whitespace_split = True
         splitted = list(sh)
 
-        for index, item in enumerate(splitted):
-            user_regex = re.findall(r"<@[0-9]{18,19}>", item)
-            if len(user_regex) > 0:
-                x = re.findall(r"[0-9]{18,19}", item)
-                if len(x) > 0:
-                    val = x[0]
-                    splitted[index] = val
-            break
+        
         for index, (name, param) in enumerate(signature):
             if name in ["ctx", "self"]:
                 continue
 
             if param.kind is param.POSITIONAL_OR_KEYWORD:
                 try:
-                    arg: str | Any = self.convert(param, splitted.pop(0))
+                    arg: str | Any = await self.convert(param, splitted.pop(0))
                     args.append(arg)
                 except Exception as e:
                     log.error(e)
             if param.kind is param.VAR_KEYWORD:
                 for arg in splitted:
-                    arg = self.convert(param, arg)
+                    arg = await self.convert(param, arg)
                     args.append(arg)
             if param.kind is param.VAR_POSITIONAL:
                 for arg in splitted:
-                    arg = self.convert(param, arg)
+                    arg = await self.convert(param, arg)
                     args.append(arg)
 
             if param.kind is param.KEYWORD_ONLY:
-                arg = self.convert(param, " ".join(splitted))
+                arg = await self.convert(param, " ".join(splitted))
                 kwargs[name] = arg
 
         for key in kwargs.copy():
             if not kwargs[key]:
                 kwargs.pop(key)
 
         return args, kwargs
@@ -473,35 +473,35 @@
                 args.insert(0, self)
         try:
             await func(*args, **kwargs)
         except Exception as e:
             error = "".join(format_exception(e, e, e.__traceback__))
             log.error(f"Could not run command \n{error}")
 
-    async def reply(self, content, file_paths: list[str] = [], delete_after: int | None = None, tts=False) -> Message:
+    async def reply(self, content, file_paths: list = [], delete_after: int | None = None, tts=False) -> Message:
         """Helper function to reply to your own message containing the command
 
         Args:
             content (str): The message you would like to send
             tts (bool, optional): Whether message should be tts or not. Defaults to False.
         """
         message: Message = await self.channel.reply(self.message, content, file_paths, delete_after, tts)
         return message
 
-    async def send(self, content, file_paths: list[str] = [], delete_after: int | None = None, tts=False) -> Message:
+    async def send(self, content, file_paths: list = [], delete_after: int | None = None, tts=False) -> Message:
         """Helper function to send message to the current channel
 
         Args:
             content (str): The message you would like to send
             tts (bool, optional): Whether message should be tts or not. Defaults to False.
         """
         message: Message = await self.channel.send(content=content, file_paths=file_paths, delete_after=delete_after, tts=tts)
         return message
 
-    async def spam(self, amount: int, content, file_paths: list[str] = [], tts: bool = False):
+    async def spam(self, amount: int, content, file_paths: list = [], tts: bool = False):
         """Helper function to spam messages in the current channel (uses asyncio.gather !!!!)
 
         Args:
             amount (int): Amount of messages to spam
             content (str): The message you would like to send
         """
         await self.channel.spam(amount, content, file_paths, tts)
@@ -510,15 +510,15 @@
         """Helper function to purge messages in the current channel, uses asyncio gather.
 
         Args:
             amount (int): The amount of messages to purge, defaults to All.
         """
         await self.channel.purge(amount)
 
-    async def edit(self, content, file_paths: list[str] = [], delete_after: int | None = None) -> Message:
+    async def edit(self, content, file_paths: list = [], delete_after: int | None = None) -> Message:
         """Helper function to edit the message you sent
 
         Args:
             content (str): Content to edit to
         """
         message = await self.message.edit(content, file_paths, delete_after)
         return message
```

### Comparing `selfcord.py-0.2.2/selfcord/utils/logging.py` & `selfcord.py-0.2.3/selfcord/utils/logging.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.2/selfcord.py.egg-info/PKG-INFO` & `selfcord.py-0.2.3/selfcord.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selfcord.py
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Discord API wrapper designed for selfbots!
 Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell
 License: MIT
 Keywords: selfbot,discord,discordapi,discordwrapper
 Description-Content-Type: text/markdown
 Provides-Extra: voice
@@ -16,15 +16,15 @@
 <strong><i>A Powerful Library for Discord Selfbots</i></strong>
 <br>
 <br>
 <a href="https://www.python.org/">
 <img src="https://img.shields.io/badge/MADE%20WITH-PYTHON-red?logoColor=red&logo=Python&style=for-the-badge">
 </a>
 <a href="https://pypi.org/project/selfcord/">
-<img src="https://img.shields.io/badge/version-0.2.2-blue?logo=adguard&style=for-the-badge">
+<img src="https://img.shields.io/badge/version-0.2.3-blue?logo=adguard&style=for-the-badge">
 </a>
 <a href="https://github.com/Shell1010/Selfcord/wiki">
 <img src="https://img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge">
 </a>
 </div>
 
 ## Feautres
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: selfcord.py Version: 0.2.2 Summary: A Discord API
+Metadata-Version: 2.1 Name: selfcord.py Version: 0.2.3 Summary: A Discord API
 wrapper designed for selfbots! Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell License: MIT Keywords: selfbot,discord,discordapi,discordwrapper
 Description-Content-Type: text/markdown Provides-Extra: voice License-File:
 LICENSE
                                  [./logo.png]
                             ****** SELFCORD ******
                    A Powerful Library for Discord Selfbots
 
                [https://img.shields.io/badge/MADE%20WITH-PYTHON-
   red?logoColor=red&logo=Python&style=for-the-badge] [https://img.shields.io/
-     badge/version-0.2.2-blue?logo=adguard&style=for-the-badge] [https://
+     badge/version-0.2.3-blue?logo=adguard&style=for-the-badge] [https://
   img.shields.io/badge/documentation-green?logo=gitbook&style=for-the-badge]
 ## Feautres - Modern Pythonic API using `async`/`await` syntax - Easy to use
 with an object oriented design - Optimised for both speed and memory - Prevents
 detection of user account automation - Clean Documentation - Community Support
 ## Installation Python 3.10 or higher is required. ``` pip install selfcord.py
 ``` ## Wiki Read our [Wiki](https://github.com/Shell1010/Selfcord/wiki) in
 regards to documentation and getting started. ## Getting Started A selfbot that
```

### Comparing `selfcord.py-0.2.2/selfcord.py.egg-info/SOURCES.txt` & `selfcord.py-0.2.3/selfcord.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.2.2/setup.py` & `selfcord.py-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
                 "selfcord",
                 "selfcord.api",
                 "selfcord.utils",
                 "selfcord.models",
                 "selfcord.api.voice",
             ]
         ),
-        version="0.2.2",
+        version="0.2.3",
         description="A Discord API wrapper designed for selfbots!",
         readme="README.md",
         author="Shell",
         extras_require={"voice": ["pynacl==1.5.0", "opuslib==3.0.1"]},
         license="MIT",
         install_requires=[
             "aiohttp==3.7.4.post0",
```

