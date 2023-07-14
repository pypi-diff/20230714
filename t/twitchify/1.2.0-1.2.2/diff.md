# Comparing `tmp/twitchify-1.2.0.tar.gz` & `tmp/twitchify-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitchify-1.2.0.tar", last modified: Mon Jul  3 17:33:31 2023, max compression
+gzip compressed data, was "twitchify-1.2.2.tar", last modified: Fri Jul 14 02:40:39 2023, max compression
```

## Comparing `twitchify-1.2.0.tar` & `twitchify-1.2.2.tar`

### file list

```diff
@@ -1,52 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:33:31.479354 twitchify-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-03 17:33:15.000000 twitchify-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-03 17:33:31.479354 twitchify-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-03 17:33:15.000000 twitchify-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 17:33:31.479354 twitchify-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-03 17:33:15.000000 twitchify-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:33:31.475354 twitchify-1.2.0/twitch/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/broadcaster.py
--rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    11134 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/goals.py
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/guest.py
--rw-r--r--   0 runner    (1001) docker     (123)    16199 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/moderation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)    15988 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/survey.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:33:31.475354 twitchify-1.2.0/twitch/types/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:33:31.479354 twitchify-1.2.0/twitch/types/eventsub/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/eventsub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/eventsub/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/eventsub/charity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/eventsub/goal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/eventsub/guest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/eventsub/hypertrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/eventsub/moderation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/eventsub/poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/eventsub/prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/eventsub/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/eventsub/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/eventsub/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/eventsub/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/types/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    10869 2023-07-03 17:33:15.000000 twitchify-1.2.0/twitch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:33:31.479354 twitchify-1.2.0/twitchify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-03 17:33:31.000000 twitchify-1.2.0/twitchify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-03 17:33:31.000000 twitchify-1.2.0/twitchify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 17:33:31.000000 twitchify-1.2.0/twitchify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 17:33:31.000000 twitchify-1.2.0/twitchify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 17:33:31.000000 twitchify-1.2.0/twitchify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:39.647008 twitchify-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-14 02:40:28.000000 twitchify-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-14 02:40:39.647008 twitchify-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-14 02:40:28.000000 twitchify-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 02:40:39.647008 twitchify-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-14 02:40:28.000000 twitchify-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:39.643008 twitchify-1.2.2/twitch/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/broadcaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9565 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8497 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/goals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/guest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17683 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/moderation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15857 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/survey.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:39.647008 twitchify-1.2.2/twitch/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:39.647008 twitchify-1.2.2/twitch/types/eventsub/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/eventsub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/eventsub/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/eventsub/charity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/eventsub/goal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/eventsub/guest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/eventsub/hypertrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/eventsub/moderation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/eventsub/poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/eventsub/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/eventsub/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/eventsub/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/eventsub/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/eventsub/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/scoopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13267 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:39.647008 twitchify-1.2.2/twitchify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-14 02:40:39.000000 twitchify-1.2.2/twitchify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-14 02:40:39.000000 twitchify-1.2.2/twitchify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 02:40:39.000000 twitchify-1.2.2/twitchify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-14 02:40:39.000000 twitchify-1.2.2/twitchify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 02:40:39.000000 twitchify-1.2.2/twitchify.egg-info/top_level.txt
```

### Comparing `twitchify-1.2.0/LICENSE` & `twitchify-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.0/PKG-INFO` & `twitchify-1.2.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitchify
-Version: 1.2.0
+Version: 1.2.2
 Summary: A Python library for Twitch's WebSocket EventSub integration.
 Home-page: https://github.com/mrsnifo/twitchify
 Author: Snifo
 Author-email: Snifo@mail.com
 License: MIT
 Project-URL: Issue tracker, https://github.com/mrsnifo/twitchify/issues
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,48 +21,74 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Twitchify
 
----
-
 [![Discord](https://img.shields.io/discord/938786168592547880)](https://discord.gg/hH4ZkNg6cA)
 [![PyPI Version](https://img.shields.io/pypi/v/twitchify)](https://pypi.org/project/twitchify)
-![Python versions](https://img.shields.io/pypi/pyversions/twitchify)
+[![Python versions](https://img.shields.io/pypi/pyversions/twitchify)](https://pypi.org/project/twitchify)
 
-Python library for Twitch's WebSocket **EventSub** integration
+Python library for Twitch's WebSocket **EventSub** integration.
 
 ## Features
 - Comprehensive support for WebSocket EventSub, providing real-time Twitch event notifications.
 - User-friendly interfaces for seamless integration.
 - Built-in support for type hinting, ensuring code clarity and maintainability.
 
 ## Installation
-
 You can install Twitchify using pip:
 
 ```shell
 # Windows
 py -3 -m pip install -U twitchify
 
 # Linux/macOS
 python3 -m pip install -U twitchify
 ```
 
-## Documentation
-Please refer to the [Events Documentation](https://github.com/MrSniFo/Twitchify/blob/main/docs/EVENTS.md) for detailed information on handling events with Twitchify.
-
 ## Quick Example
 ```python
 from twitch import Client
 from twitch.user import Follower
 
-client = Client(client_id="CLIENT ID HERE")
+client = Client(client_id="YOUR_CLIENT_ID")
+
+@client.event
+async def on_ready():
+    """
+    Event handler triggered when the client is ready to start processing events.
+    """
+    print("Ready as %s" % client.user.display_name)
+
+
+@client.event
+async def on_follow(user: Follower):
+    """
+    Event handler triggered when a user follows the channel.
+    """
+    print("%s just followed you!" % user.display_name)
+
+# Run the client with your user access token.
+client.run(access_token="YOUR_ACCESS_TOKEN")
+```
+
+### With built-in Authorization
+
+```python
+from twitch import Client
+from twitch.user import Follower
+
+# Initialize the Twitch client with your client ID and client secret.
+client = Client(client_id="YOUR_CLIENT_ID", client_secret="YOUR_CLIENT_SECRET")
+
+# Generate the authorization URL for the Twitch client.
+# The user should visit the provided URL to authorize the app.
+auth = client.auth()
 
 @client.event
 async def on_ready():
     """
     Event handler triggered when the client is ready to start processing events.
     """
     print("Ready as %s" % client.user.display_name)
@@ -71,9 +97,12 @@
 @client.event
 async def on_follow(user: Follower):
     """
     Event handler triggered when a user follows the channel.
     """
     print("%s just followed you!" % user.display_name)
 
-client.run(access_token="USER ACCESS TOKEN HERE")
+# You can store the access token and refresh token for future use, so you don't have to authorize again.
+client.run(access_token=auth.access_token, refresh_token=auth.refresh_token)
 ```
+
+Please refer to the [Documentation](https://github.com/MrSniFo/Twitchify/blob/main/docs) or [Examples](https://github.com/MrSniFo/Twitchify/tree/main/examples) for more details.
```

### Comparing `twitchify-1.2.0/README.md` & `twitchify-1.2.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,69 @@
 # Twitchify
 
----
-
 [![Discord](https://img.shields.io/discord/938786168592547880)](https://discord.gg/hH4ZkNg6cA)
 [![PyPI Version](https://img.shields.io/pypi/v/twitchify)](https://pypi.org/project/twitchify)
-![Python versions](https://img.shields.io/pypi/pyversions/twitchify)
+[![Python versions](https://img.shields.io/pypi/pyversions/twitchify)](https://pypi.org/project/twitchify)
 
-Python library for Twitch's WebSocket **EventSub** integration
+Python library for Twitch's WebSocket **EventSub** integration.
 
 ## Features
 - Comprehensive support for WebSocket EventSub, providing real-time Twitch event notifications.
 - User-friendly interfaces for seamless integration.
 - Built-in support for type hinting, ensuring code clarity and maintainability.
 
 ## Installation
-
 You can install Twitchify using pip:
 
 ```shell
 # Windows
 py -3 -m pip install -U twitchify
 
 # Linux/macOS
 python3 -m pip install -U twitchify
 ```
 
-## Documentation
-Please refer to the [Events Documentation](https://github.com/MrSniFo/Twitchify/blob/main/docs/EVENTS.md) for detailed information on handling events with Twitchify.
-
 ## Quick Example
 ```python
 from twitch import Client
 from twitch.user import Follower
 
-client = Client(client_id="CLIENT ID HERE")
+client = Client(client_id="YOUR_CLIENT_ID")
+
+@client.event
+async def on_ready():
+    """
+    Event handler triggered when the client is ready to start processing events.
+    """
+    print("Ready as %s" % client.user.display_name)
+
+
+@client.event
+async def on_follow(user: Follower):
+    """
+    Event handler triggered when a user follows the channel.
+    """
+    print("%s just followed you!" % user.display_name)
+
+# Run the client with your user access token.
+client.run(access_token="YOUR_ACCESS_TOKEN")
+```
+
+### With built-in Authorization
+
+```python
+from twitch import Client
+from twitch.user import Follower
+
+# Initialize the Twitch client with your client ID and client secret.
+client = Client(client_id="YOUR_CLIENT_ID", client_secret="YOUR_CLIENT_SECRET")
+
+# Generate the authorization URL for the Twitch client.
+# The user should visit the provided URL to authorize the app.
+auth = client.auth()
 
 @client.event
 async def on_ready():
     """
     Event handler triggered when the client is ready to start processing events.
     """
     print("Ready as %s" % client.user.display_name)
@@ -46,9 +72,12 @@
 @client.event
 async def on_follow(user: Follower):
     """
     Event handler triggered when a user follows the channel.
     """
     print("%s just followed you!" % user.display_name)
 
-client.run(access_token="USER ACCESS TOKEN HERE")
+# You can store the access token and refresh token for future use, so you don't have to authorize again.
+client.run(access_token=auth.access_token, refresh_token=auth.refresh_token)
 ```
+
+Please refer to the [Documentation](https://github.com/MrSniFo/Twitchify/blob/main/docs) or [Examples](https://github.com/MrSniFo/Twitchify/tree/main/examples) for more details.
```

### Comparing `twitchify-1.2.0/setup.py` & `twitchify-1.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.0/twitch/__init__.py` & `twitchify-1.2.2/twitch/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 A Python library for Twitch's WebSocket EventSub integration.
 
 :copyright: (c) 2023-present Snifo
 :license: MIT, see LICENSE for more details.
 """
 
 __title__ = 'Twitchify'
-__version__ = '1.2.0'
+__version__ = '1.2.2'
 __license__ = 'MIT License'
 __author__ = 'Snifo'
 __email__ = 'Snifo@mail.com'
 __github__ = 'https://github.com/mrsnifo/twitchify'
 
 from .client import *
+from .auth import *
 from .user import *
 from .broadcaster import *
 from .channel import *
 from .stream import *
 from .moderation import *
 from .reward import *
 from .goals import *
```

### Comparing `twitchify-1.2.0/twitch/broadcaster.py` & `twitchify-1.2.2/twitch/broadcaster.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     :param user: The user data representing the broadcaster.
     """
     def __init__(self, *, http: HTTPClient, user: UserType):
         self.__http = http
         self.id: str = user['id']
         self.name: str = user['login']
         self.display_name: str = user['display_name']
-        self.email: Optional[str] = empty_to_none(text=user['email'])
+        self.email: Optional[str] = user.get('email')
         self.images: Images = Images(user=user)
         # Set the broadcaster tier.
         self.tier: Tier = user['broadcaster_type'] if user['broadcaster_type'] else 'regular'
         # Set the user type.
         self.type: Types = user['type'] if user['type'] else 'regular'
         self.joined_at: datetime = parse_rfc3339_timestamp(user['created_at'])
         # Updating the channel description from the user.
```

### Comparing `twitchify-1.2.0/twitch/channel.py` & `twitchify-1.2.2/twitch/channel.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,21 +55,24 @@
 
 class Channel:
     """
     Represents a channel.
 
     :param channel: The channel data.
     """
-    __slots__ = ('title', 'description', 'delay', 'tags', 'category')
+    __slots__ = ('title', 'description', 'delay', 'tags', 'category', 'classification',
+                 'is_branded_content')
 
     def __init__(self, channel: ch.Channel):
         self.description: Optional[str] = None
         self.title: Optional[str] = channel['title']
         self.delay: int = channel['delay']
         self.tags: List[str] = channel['tags']
+        self.classification: List[str] = channel['content_classification_labels']
+        self.is_branded_content: bool = channel['is_branded_content']
         # Category.
         _c = Category(channel=channel) if channel['game_id'] != '' else None
         self.category: Optional[Category] = _c
 
     def __repr__(self) -> str:
         return f'<Channel title={self.title} description={self.description}>'
```

### Comparing `twitchify-1.2.0/twitch/client.py` & `twitchify-1.2.2/twitch/client.py`

 * *Files 25% similar despite different names*

```diff
@@ -26,40 +26,43 @@
 
 from .gateway import EventSubWebSocket
 from .state import ConnectionState
 from .utils import setup_logging
 from .http import HTTPClient
 from .channel import Channel
 from .stream import Stream
+from .auth import Auth
 
 import asyncio
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from typing import Any, List, Optional, Callable
+    from .types.scoopes import ScopesType
     from .broadcaster import Broadcaster
 
 import logging
 _logger = logging.getLogger(__name__)
-
 __all__ = ('Client',)
 
 
 class Client:
     """
     Represents a Twitch client for interacting with the Twitch API and receiving event
     notifications.
 
     :param client_id: Client id
     :param client_secret: Client secret needed to re-generate a new access token.
     """
 
     def __init__(self, client_id: str, client_secret: Optional[str] = None) -> None:
-        self.loop: Optional[asyncio.AbstractEventLoop] = None
-        self._http = HTTPClient(dispatcher=self.dispatch, client=client_id, secret=client_secret)
+        setup_logging()
+        self._loop: Optional[asyncio.AbstractEventLoop] = None
+        self._http = HTTPClient(dispatcher=self.dispatch, client_id=client_id, secret_secret=client_secret)
+        self._auth = Auth(http=self._http, client_id=client_id)
         self._connection: ConnectionState = ConnectionState(dispatcher=self.dispatch,
                                                             http=self._http,
                                                             events=self._sub_events)
 
     @property
     def user(self) -> Broadcaster:
         """
@@ -81,21 +84,46 @@
         """
         Retrieves the stream of the broadcaster if currently live.
 
         :return: An instance of the Stream class representing the stream if live, otherwise None.
         """
         return await self._connection.broadcaster.get_stream()
 
+    def auth(self, scopes: Optional[ScopesType] = None, verify: bool = False, port: int = 3000) -> Auth:
+        """
+        Authenticates with the Twitch API using OAuth 2.0 authorization code grant flow.
+
+        :param scopes: Optional. The list of scopes to request authorization for.
+        :param verify: Optional. Whether to force verification during the authorization process.
+        :param port: Optional. The port to use for the local server during the authorization process.
+        :return: An instance of the Auth class representing the authentication result.
+        """
+        if scopes:
+            self._auth.scopes = scopes
+        _logger.info('1. Create an app on the Twitch Developer Console:\n'
+                     '   - Go to https://dev.twitch.tv/console\n'
+                     '   - Sign in with your Twitch account\n'
+                     '   - Click on \'Applications\' in the top navigation\n'
+                     '   - Click on \'Register Your Application\'\n'
+                     '   - Fill in the required details for your app\n'
+                     '   - Set \'OAuth Redirect URLs\' to your redirect URI:\n'
+                     '     -> Redirect URI: %s\n'
+                     '   - Save your changes\n', self._auth.uri)
+        _logger.info('2. Navigate to the following URL in your web browser:\n'
+                     '   -> Authorization URL: %s\n', self._auth.url)
+        self._auth.get_code(verify=verify, port=port)
+        _logger.info('Successfully authorized with the app!\n')
+        return self._auth
+
     @property
     def _sub_events(self) -> List[str]:
         """Retrieve the names of the subscribed events."""
         return [attr.replace('on_', '', 1) for attr in dir(self) if attr.startswith('on_')]
 
-    async def _run_event(self, coro: Callable[..., Any], event_name: str, *args: Any,
-                         **kwargs: Any) -> None:
+    async def _run_event(self, coro: Callable[..., Any], event_name: str, *args: Any, **kwargs: Any) -> None:
         """
         Execute the specified event coroutine with the given arguments.
         """
         try:
             await coro(*args, **kwargs)
         except asyncio.CancelledError:
             pass
@@ -104,19 +132,22 @@
 
     def dispatch(self, event: str, /, *args: Any, **kwargs: Any) -> None:
         """
         Dispatch the specified event with the given arguments.
         """
         _logger.debug('Dispatching event %s', event)
         method = "on_" + event
-        coro = getattr(self, method)
-        if coro is not None and asyncio.iscoroutinefunction(coro):
-            wrapped = self._run_event(coro, method, *args, **kwargs)
-            # Schedule the task
-            self.loop.create_task(wrapped, name=f'Twitchify:{method}')
+        try:
+            coro = getattr(self, method)
+            if coro is not None and asyncio.iscoroutinefunction(coro):
+                wrapped = self._run_event(coro, method, *args, **kwargs)
+                # Schedule the task
+                self._loop.create_task(wrapped, name=f'Twitchify:{method}')
+        except AttributeError as error:
+            _logger.error('Event: %s Error: %s', event, error)
 
     @staticmethod
     async def on_error(event_name: str, error: str, /, *args: Any, **kwargs: Any) -> None:
         """
         The default error handler for events.
         """
         _logger.exception('Ignoring error: %s from %s, args: %s kwargs: %s', error, event_name,
@@ -124,59 +155,70 @@
 
     def event(self, coro: Callable[..., Any], /) -> None:
         """
         Decorator to register an event coroutine.
         """
         if not asyncio.iscoroutinefunction(coro):
             raise TypeError("The registered event must be a coroutine function")
-
         setattr(self, coro.__name__, coro)
 
-    async def connect(self, access_token: str, refresh_token: Optional[str]) -> None:
+    async def connect(self, *, access_token: str, refresh_token: Optional[str], reconnect: bool) -> None:
+
         """
         Establishes a connection to Twitch services.
         """
-        # Setup logger
-        setup_logging()
-        if self.loop is None:
-            self.loop = asyncio.get_running_loop()
+        # Setup loop
+        if self._loop is None:
+            self._loop = asyncio.get_running_loop()
+
         # Validating the access key and opening a new session.
         validation = await self._http.open_session(token=access_token,
                                                    refresh_token=refresh_token)
         # Retrieving the client.
         await self._connection.get_client()
         # Creating an EventSub websocket.
-        EventSub = EventSubWebSocket(http=self._http, cnx=self._connection,
-                                     loop=self.loop,
+        EventSub = EventSubWebSocket(http=self._http, connection=self._connection,
+                                     loop=self._loop,
                                      events=self._sub_events)
         # Creating tasks.
         tasks = [
-            self.loop.create_task(self._http.Refresher(expires_in=validation['expires_in']),
-                                  name="Twitchify:Refresher"),
-            self.loop.create_task(EventSub.connect(), name="Twitchify:EventSub")
+            self._loop.create_task(self._http.refresher(expires_in=validation['expires_in']),
+                                   name="Twitchify:Refresher"),
+            self._loop.create_task(EventSub.connect(reconnect=reconnect), name="Twitchify:EventSub")
         ]
         self.dispatch('connect')
+
         await asyncio.gather(*tasks)
 
-    async def start(self, access_token: str, refresh_token: Optional[str] = None) -> None:
+    async def start(self, access_token: str, refresh_token: Optional[str] = None,
+                    reconnect: bool = True) -> None:
         """
         Starts the Twitch client by establishing a connection and initiating the event loop.
         """
         try:
-            await self.connect(access_token, refresh_token)
-        # Automatically close the HTTP session when an error occurs.
-        except asyncio.CancelledError:
-            if self._http is not None and self._http.is_open:
-                await self._http.close()
-            raise
+            await self.connect(access_token=access_token, refresh_token=refresh_token, reconnect=reconnect)
         except Exception as error:
+
             if self._http is not None and self._http.is_open:
                 await self._http.close()
             raise error
+        finally:
+            pass
 
-    def run(self, access_token: str, refresh_token: Optional[str] = None) -> None:
+    def run(self, access_token: str, refresh_token: Optional[str] = None, reconnect: bool = True) -> None:
         """
         Runs the Twitch client without establishing a connection and initiating the event loop.
         """
+
         async def runner():
-            await self.start(access_token, refresh_token)
-        asyncio.run(runner())
+            await self.start(access_token=access_token, refresh_token=refresh_token, reconnect=reconnect)
+
+        try:
+            self._loop = asyncio.get_running_loop()
+        except RuntimeError:
+            self._loop = asyncio.get_event_loop()
+        if self._loop.is_running():
+            # Already running in an event loop, so directly run the main function.
+            asyncio.run(runner())
+        else:
+            # No running event loop, so run the event loop and then run the main function.
+            self._loop.run_until_complete(runner())
```

### Comparing `twitchify-1.2.0/twitch/errors.py` & `twitchify-1.2.2/twitch/errors.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     """
 
     def __init__(self):
         super().__init__('Twitch API server error.')
 
 
 # ------------------------------------------
-#               HTTPException
+#              HTTP Exception
 # ------------------------------------------
 
 class HTTPException(TwitchException):
     """
     Exception raised when an HTTP request operation fails.
     """
     pass
@@ -107,25 +107,30 @@
 class WebsocketClosed(WebSocketError):
     """
     Exception raised when the websocket connection is closed.
     """
     pass
 
 
+class WebsocketUnused(WebSocketError):
+    """
+    Exception is raised when no subscription has been created within 10 seconds.
+    """
+
+
 class WsReconnect(WebSocketError):
     """
     Exception raised to indicate that WebSocket should reconnect to a new URL.
     """
-
     def __init__(self, url: str):
         super().__init__(url)
 
 
 # -------------------------------------------
-#               ClientException
+#              Client Exception
 # -------------------------------------------
 
 class ClientException(TwitchException):
     """
     Exception raised when a Client operation fails.
     """
     pass
@@ -136,15 +141,17 @@
     Exception raised when the user does not exist.
     """
 
     def __init__(self, message: str = 'Unable to find the requested user.'):
         super().__init__(message)
 
 
-class SubscriptionError(ClientException):
+# ------------------------------------------
+#               Auth Exception
+# ------------------------------------------
+class AuthorizationError(ClientException):
     """
-    Exception raised when the authorization is revoked.
+    Exception raised when access is denied.
     """
 
-    def __init__(self, subscription: str, version: str):
-        message = f'Subscription type `{subscription}` and version `{version}`.'
+    def __init__(self, message: str):
         super().__init__(message)
```

### Comparing `twitchify-1.2.0/twitch/gateway.py` & `twitchify-1.2.2/twitch/gateway.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,21 +20,22 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 from __future__ import annotations
 
-from .errors import (WebSocketError, WebsocketClosed, NotFound, SessionClosed, Forbidden,
-                     SubscriptionError, WsReconnect)
+from .errors import (WebSocketError, WebsocketClosed, NotFound, SessionClosed, Forbidden, WebsocketUnused,
+                     WsReconnect)
 from .utils import to_json, get_subscriptions
 
 from json import JSONDecodeError
-from aiohttp import WSMsgType
 import asyncio
+import aiohttp
+
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from .types.eventsub.subscriptions import SubscriptionInfo
     from asyncio import AbstractEventLoop
     from typing import Optional, List, Dict, Any
     from aiohttp import ClientWebSocketResponse
@@ -43,118 +44,113 @@
     from .types.gateway import Session, Subscription
 
 import logging
 _logger = logging.getLogger(__name__)
 
 
 class EventSubWebSocket:
-    DEFAULT_URL = 'wss://eventsub.wss.twitch.tv/ws'
+    """
+    Represents EventSub WebSocket.
 
-    __slots__ = ('__http', '__connection', '__loop', 'subscriptions', '_ready', '_keep_alive',
-                 '_ws', '_ws_switch', 'session_id', 'retry_count')
+    :param http: The HTTP client for making API requests.
+    :param connection: The ConnectionState object.
+    :param loop: The event loop.
+    :param events: A list of events.
+    """
 
-    def __init__(self, *, http: HTTPClient, cnx: ConnectionState, loop, events: List[str]) -> None:
-        """
-        Initialize the EventSubWebSocket.
+    __slots__ = ('__http', '__connection', '__loop', 'subscriptions', '_ready', '_keep_alive',
+                 '_ws', '_ws_switch', 'session_id', '__reconnect')
 
-        :param http: The HTTP client for making API requests.
-        :param cnx: The ConnectionState object.
-        :param loop: The event loop.
-        :param events: A list of events.
-        """
+    def __init__(self, *, http: HTTPClient, connection: ConnectionState, loop: AbstractEventLoop,
+                 events: List[str]) -> None:
         self.__http: HTTPClient = http
-        self.__connection: ConnectionState = cnx
+        self.__connection: ConnectionState = connection
         self.__loop: AbstractEventLoop = loop
         self.subscriptions: List[SubscriptionInfo] = get_subscriptions(events=events)
         # Default subscription
         self.subscriptions.append({'name': 'user.update', 'version': '1'})
         # Default Session KeepAlive.
         self._keep_alive: int = 10
         self._ws: Optional[ClientWebSocketResponse] = None
         self._ws_switch: Optional[ClientWebSocketResponse] = None
         self.session_id: Optional[str] = None
-        self.retry_count: int = 0
 
-    async def _connect(self, url) -> None:
-        """
-        Establish a WebSocket connection.
-
-        :param url: The URL to connect to.
-        """
-        if self.__http.is_open:
-            _ws = await self.__http.ws_connect(url=url)
-            if self._ws is not None and not self._ws.closed:
-                self._ws_switch = self._ws
-                self._ws = _ws
-            else:
-                self._ws = _ws
-            self.retry_count = 0
-            await self.handle_messages()
-        else:
-            raise SessionClosed
-
-    async def connect(self, url: str = DEFAULT_URL) -> None:
+    async def connect(self, reconnect: bool, url: str = 'wss://eventsub.wss.twitch.tv/ws') -> None:
         """
         Connect to the WebSocket.
 
+        :param reconnect: reconnect to the websocket if an error occurred
         :param url: The URL to connect to. Default is the DEFAULT_URL.
         """
+        _retry: int = 0
         while True:
+            # Reset retry timer
+            if _retry == 12:
+                _retry = 1
+            else:
+                _retry += 1
             try:
-                await self._connect(url=url)
+                _ws = await self.__http.ws_connect(url=url)
+                if self._ws is not None and not self._ws.closed:
+                    self._ws_switch = self._ws
+                    self._ws = _ws
+                else:
+                    self._ws = _ws
+                await self.handle_messages()
             except WsReconnect as reconnect_url:
                 url = str(reconnect_url)
                 _logger.debug('Reconnecting to URL: %s', url)
                 continue
-            except (OSError, WebSocketError, SessionClosed, TimeoutError) as error:
-                self.retry_count += 1
-                if 3 >= self.retry_count:
-                    if isinstance(error, WebSocketError):
-                        _logger.error('WebSocket connection closed. Retrying in %s seconds...',
-                                      (5 * self.retry_count))
-                    elif isinstance(error, SessionClosed):
-                        _logger.error('Cannot connect because the session is closed.'
-                                      ' Retrying in %s seconds...', (5 * self.retry_count))
-                    elif isinstance(error, asyncio.TimeoutError):
-                        _logger.error('Timeout occurred while waiting for WebSocket message. '
-                                      'Retrying in %s seconds...', (5 * self.retry_count))
-                    else:
-                        _logger.info('Retrying to connect to the WebSocket (%s) in %s seconds...',
-                                     url, (5 * self.retry_count))
+            except (WebsocketClosed, SessionClosed, asyncio.TimeoutError) as error:
+                if isinstance(error, WebsocketUnused):
+                    raise
+                if isinstance(error, SessionClosed):
+                    _logger.error('Failed to establish a WebSocket connection due to a closed session. '
+                                  'Retrying in %s seconds...', _retry * 5)
+                else:
+                    _logger.error('WebSocket connection failed: %s Retrying in %s seconds...',
+                                  str(error), _retry * 5)
+                await asyncio.sleep(5 * _retry)
+            except (WebSocketError, aiohttp.ClientConnectorError, TimeoutError) as error:
+                if reconnect:
+                    _logger.error('WebSocket connection error: %s Retrying in %s seconds...',
+                                  str(error), _retry * 5)
+                    await asyncio.sleep(5 * _retry)
                 else:
-                    raise  # Re-raise the original error
-                await asyncio.sleep(5 * self.retry_count)
+                    raise
 
     async def handle_messages(self) -> None:
         """
         Handle incoming WebSocket messages.
         """
         while True:
             msg = await asyncio.wait_for(self._ws.receive(), timeout=(self._keep_alive + 10))
-            if msg.type == WSMsgType.TEXT:
+            if msg.type == aiohttp.WSMsgType.TEXT:
                 await self.received_response(response=str(msg.data))
-            elif msg.type == WSMsgType.CLOSED:
-                _logger.error('WebSocket connection closed by the server')
+            elif msg.type == aiohttp.WSMsgType.CLOSED:
+                _logger.error('WebSocket connection has been closed by the server.')
                 close_code = self._ws.close_code
-                if close_code == 4004:
-                    raise WebsocketClosed('Failed to reconnect to a new WebSocket within'
-                                          ' the specified time.')
+                if close_code == 4000:
+                    raise WebsocketClosed(message='Internal server error.')
+                elif close_code == 4001:
+                    raise WebsocketClosed(message='Client sent inbound traffic.')
+                elif close_code == 4003:
+                    raise WebsocketUnused(message='Connection unused.')
+                elif close_code == 4004:
+                    raise WebsocketClosed(message='Reconnect grace time expired.')
+                elif close_code == 4005:
+                    raise WebsocketClosed(message='Network timeout.')
+                elif close_code == 4006:
+                    raise WebsocketClosed(message='Network error.')
                 elif close_code == 4007:
-                    raise WebsocketClosed('Failed to reconnect to a new WebSocket.'
-                                          ' The reconnect URL provided is invalid.')
-                elif close_code in [4000, 4001, 4002, 4003, 4005, 4006]:
-                    raise WebSocketError(
-                        f'WebSocket connection closed by the server. Close code:{close_code}')
-                else:
-                    raise WebSocketError(
-                        f'WebSocket connection closed by the server. Close code:{close_code}')
-            elif msg.type == WSMsgType.ERROR:
+                    raise WebsocketClosed(message='Invalid reconnect.')
+            elif msg.type == aiohttp.WSMsgType.ERROR:
                 exception = self._ws.exception()
-                error_message = str(exception) if exception else 'Unknown error occurred'
-                raise WebSocketError(f'WebSocket connection closed with error:{error_message}')
+                error_message = str(exception) if exception else 'Unknown error occurred.'
+                raise WebSocketError(message=error_message)
 
     async def received_response(self, response: str) -> None:
         """
         Process the received response.
 
         :param response: The response received from the WebSocket.
         """
@@ -178,18 +174,20 @@
                     # Welcome message.
                     if self._ws_switch is not None and not self._ws_switch.closed:
                         # Closing the old connection.
                         await self._ws_switch.close()
                         self._ws_switch = None
                     else:
                         # Subscribing to events.
-                        task = self.__http.subscribe(user_id=self.__connection.broadcaster.id,
-                                                     session_id=_session['id'],
-                                                     subscriptions=self.subscriptions)
-                        self.__loop.create_task(task, name='Twitchify:Subscriptions')
+                        subscribe = self.__http.subscribe(
+                            user_id=self.__connection.broadcaster.id,
+                            session_id=_session['id'],
+                            subscriptions=self.subscriptions)
+
+                        self.__loop.create_task(subscribe, name='Twitchify:Subscriptions')
                     if _session['id'] != self.session_id:
                         if self.session_id is not None:
                             _logger.debug('A new WebSocket Session has been detected ID: %s',
                                           _session['id'])
                         self.session_id = _session['id']
                     # KeepAlive timeout.
                     self._keep_alive = _session['keepalive_timeout_seconds']
@@ -216,9 +214,9 @@
                     # The user mentioned in the subscription no longer exists.
                     elif _status == 'user_removed':
                         raise NotFound(
                             'The user mentioned in the subscription no longer exists.'
                         )
                     # Subscription type and version is no longer supported.
                     elif _status == 'version_removed':
-                        raise SubscriptionError(subscription=_subscription['type'],
-                                                version=_subscription['version'])
+                        _logger.warning('Subscription type `%s` version `%s` is no longer supported.',
+                                        _subscription['type'], _subscription['version'])
```

### Comparing `twitchify-1.2.0/twitch/goals.py` & `twitchify-1.2.2/twitch/goals.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,17 +44,17 @@
 
     :param charity: A dictionary containing charity information.
     """
     __slots__ = ('name', 'description', 'logo', 'website')
 
     def __init__(self, charity: ch.SpecificCharity) -> None:
         self.name: str = charity['charity_name']
-        self.description: Optional[str] = charity.get('charity_description')  # Beta
+        self.description: Optional[str] = charity.get('charity_description')
         self.logo: str = charity['charity_logo']
-        self.website: Optional[str] = charity.get('charity_website')  # Beta
+        self.website: Optional[str] = charity.get('charity_website')
 
     def __repr__(self) -> str:
         return f'<CharityInfo name={self.name} description={self.description}>'
 
 
 class CharityAmount:
     """
```

### Comparing `twitchify-1.2.0/twitch/guest.py` & `twitchify-1.2.2/twitch/guest.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.0/twitch/http.py` & `twitchify-1.2.2/twitch/http.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,50 +20,50 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 from __future__ import annotations
 
-from .errors import (
-    UnknownError, TwitchServerError, BadRequest, Unauthorized,
-    Forbidden, HTTPException, SubscriptionError, NotFound)
+from .errors import (TwitchServerError, BadRequest, Unauthorized, Forbidden, HTTPException, NotFound,
+                     SessionClosed)
 from aiohttp import ClientSession, helpers
 from . import __version__, __github__
 from asyncio import Lock, sleep, Task
 from .utils import format_seconds
 from time import time
+from json import JSONDecodeError
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from .types.eventsub.subscriptions import SubscriptionInfo
     from typing import Optional, List, Callable, Any
     from aiohttp import ClientWebSocketResponse
-    from .types.http import Validate, Refresh
+    from .types.http import Validate, Token
     from .types.stream import Stream
     from .types.user import UserType
     from .types.channel import Channel
 
 import logging
 _logger = logging.getLogger(__name__)
 
 
 class Route:
+    """
+    Initialize a Route object.
+
+    :param method: The HTTP method of the route.
+    :param path: The path of the route.
+    :param url: The complete URL of the route (overrides BASE_ROUTE + path). Defaults to None.
+    """
     BASE_ROUTE: str = 'https://api.twitch.tv/helix/'
 
     __slots__ = ('method', 'url')
 
     def __init__(self, method: str, path: Optional[str] = None, url: Optional[str] = None) -> None:
-        """
-        Initialize a Route object.
-
-        :param method: The HTTP method of the route.
-        :param path: The path of the route.
-        :param url: The complete URL of the route (overrides BASE_ROUTE + path). Defaults to None.
-        """
         self.method: str = method
         if path is None and url is None:
             raise TypeError
         else:
             if url is not None:
                 self.url = url
             else:
@@ -74,48 +74,49 @@
 
 
 class HTTPClient:
     """Serves as an HTTP client responsible for sending HTTP requests to the Twitch API."""
     __slots__ = ('_dispatch', '_client_id', '_client_secret', '__session', '_session_lock',
                  '_user_agent', '_refresh_token')
 
-    def __init__(self, dispatcher: Callable[..., Any], client: str, secret: Optional[str]) -> None:
+    def __init__(self, dispatcher: Callable[..., Any], client_id: str, secret_secret: Optional[str]) -> None:
         """
         Initialize the HTTPClient object.
         """
         self._dispatch: Callable[[str, Any, Any], Task] = dispatcher
-        self._client_id = client
-        self._client_secret = secret
+        self._client_id: str = client_id
+        self._client_secret: str = secret_secret
         self.__session: Optional[ClientSession] = None
         self._session_lock: Lock = Lock()
         self._user_agent: str = f'Twitchify/{__version__} (GitHub: {__github__})'
         self._refresh_token: Optional[str] = None
 
     @property
     def is_open(self) -> bool:
         """
         Checks if the HTTP session is open.
 
         :return: True if the session is open, False otherwise.
         """
         return self.__session is not None and not self.__session.closed
 
-    async def _open(self, *, access_token: str) -> None:
+    async def _open(self, *, access_token: Optional[str] = None) -> None:
         """
         Opens an HTTP session.
 
         :param access_token: The access token to use for authentication.
         """
         async with self._session_lock:
             if not self.is_open:
                 headers = {
                     'Client-ID': self._client_id,
-                    'Authorization': f'Bearer {access_token}',
                     'Content-Type': 'application/json'
                 }
+                if access_token:
+                    headers.update({'Authorization': f'Bearer {access_token}'})
                 self.__session = ClientSession(headers=headers)
                 _logger.debug('New HTTP session has been created.')
 
     async def close(self) -> bool:
         """
         Closes the HTTP session.
 
@@ -138,44 +139,47 @@
 
         :param refresh_token:
          (Optional) The refresh token for refreshing the access token.
 
         :return: A validation response.
         """
         # Opening a session.
-        await self._open(access_token=token)
-        self._refresh_token: Optional[str] = refresh_token
+        if self.is_open:
+            self.__session.headers.update({'Authorization': f'Bearer {token}'})
+        else:
+            await self._open(access_token=token)
+        self._refresh_token = refresh_token
         validation: Validate = await self._validate_token(generate=True)
         if validation['expires_in'] == 0:
-            _logger.debug('Old application detected, exempt from expiration rules.'
+            _logger.debug('An old has been application detected, exempt from expiration rules.'
                           ' Investigation needed.')
             if self._refresh_token is not None:
                 _logger.warning(
                     'The refresh token has been removed due to the access token returning an'
                     ' expire time of 0.')
-        else:
-            self._refresh_token = refresh_token
-
+                self._refresh_token = None
         return validation
 
     async def ws_connect(self, *, url: str) -> ClientWebSocketResponse:
         """
         Creates a websocket using the existing session.
 
         :return:
          The created websocket.
         """
 
-        websocket: ClientWebSocketResponse = await self.__session.ws_connect(
-            url=url,
-            headers={'User-Agent': self._user_agent},
-            timeout=30,
-            autoclose=False
-        )
-        return websocket
+        if self.is_open:
+            websocket: ClientWebSocketResponse = await self.__session.ws_connect(
+                url=url,
+                headers={'User-Agent': self._user_agent},
+                timeout=30,
+                autoclose=False
+            )
+            return websocket
+        raise SessionClosed
 
     async def _request(self, *, route: Route, **kwargs) -> dict:
         """
         HTTP request base.
 
         :param route:
          The route to send the request to.
@@ -194,55 +198,82 @@
                     if response.status in [200, 202]:
                         return await response.json()
                     if response.status == 400:
                         raise BadRequest
                     elif response.status == 401:
                         raise Unauthorized
                     elif response.status == 403:
+                        try:
+                            error = await response.json()
+                            if error.get('message'):
+                                raise Forbidden(message=error['message'])
+                        except JSONDecodeError:
+                            pass
                         raise Forbidden
                     elif response.status == 404:
                         raise NotFound
                     elif 500 <= response.status < 600:
                         raise TwitchServerError
-                    raise UnknownError
+                    raise HTTPException
             except OSError as exc:
                 if 3 >= retry_count:
                     _logger.info('Request failed: %s. Retrying in %s seconds...',
                                  Route, (5 * retry_count))
                     await sleep(5 * retry_count)
                 raise HTTPException from exc
 
-    async def _generate_token(self) -> Optional[Refresh]:
+    async def _generate_token(self) -> Optional[Token]:
+        """
+        Generate a new access token using client_secret and refresh_token.
+        """
         if self._refresh_token and self._client_secret:
             # There is a chance that both the task and the normal
             # request can refresh the token at the same time.
             if not self._session_lock.locked():
                 async with self._session_lock:
                     # Encoding the client secret.
                     encoded_secret = helpers.quote(self._refresh_token)
                     params = {'grant_type': 'refresh_token',
                               'refresh_token': encoded_secret,
                               'client_id': self._client_id,
                               'client_secret': self._client_secret}
                     _logger.debug('Generating a new access token to refresh the existing one.')
                     route = Route(method='POST', url='https://id.twitch.tv/oauth2/token')
-                    refresh: Refresh = await self.request(route=route, params=params)
+                    refresh: Token = await self.request(route=route, params=params)
                     # Updating the session headers.
-                    self.__session.headers.update({
-                        'Authorization': f'Bearer {refresh["access_token"]}'
-                    })
+                    self.__session.headers.update({'Authorization': f'Bearer {refresh["access_token"]}'})
                     _logger.debug('Session headers have been successfully updated with'
                                   ' the new access token.')
                     self._dispatch('refresh_token', refresh['access_token'])
                     return refresh
         return None
 
+    async def auth_code(self, code: str, redirect_uri: str) -> Token:
+        """
+        Authorization using the code to get the access token and refresh token.
+
+        :param code: The authorization code.
+        :param redirect_uri: The redirect URI.
+
+        :return:
+         User Token.
+        """
+        await self._open()
+        params = {'client_id': self._client_id,
+                  'client_secret': self._client_secret,
+                  'code': code,
+                  'grant_type': 'authorization_code',
+                  'redirect_uri': redirect_uri}
+        route = Route(method='POST', url='https://id.twitch.tv/oauth2/token')
+        generate: Token = await self.request(route=route, params=params)
+        return generate
+
     async def _validate_token(self, *, generate: bool = False) -> Validate:
         """
-        Validating access token.
+        Validate access token.
 
         :param generate:
          Generate a new token if it's unauthorized. Defaults to False.
 
         :return:
          The validation response.
         """
@@ -255,20 +286,19 @@
             except Unauthorized as exc:
                 if generate and (self._client_secret and self._refresh_token):
                     try:
                         # Generating a new access token.
                         await self._generate_token()
                         continue
                     except (BadRequest, Forbidden):
-                        raise Unauthorized(message='Invalid refresh token or client secret.'
-                                           ) from exc
+                        raise Unauthorized(message='Invalid refresh token or client secret.') from exc
                 else:
                     raise
 
-    async def Refresher(self, *, expires_in: int) -> None:
+    async def refresher(self, *, expires_in: int) -> None:
         """
         Refresher task to refresh the current access token.
 
         :param expires_in:
          The expiration time of the current access token.
         """
         start_time = time()
@@ -326,27 +356,27 @@
                     _logger.error('Unable to make the request to URL: %s Unauthorized access.',
                                   route.url)
                     await self._validate_token(generate=True)
                     continue
                 except (Unauthorized, BadRequest):
                     raise
 
-    async def subscribe(self, *,
-                        user_id: str, session_id: str, subscriptions: List[SubscriptionInfo]) -> None:
+    async def subscribe(self, *, user_id: str, session_id: str,
+                        subscriptions: List[SubscriptionInfo]) -> None:
         """
         Subscribes to multiple events with the specified subscriptions.
 
         :param user_id:
          The user ID.
 
         :param session_id:
          The session ID for the subscriptions.
 
         :param subscriptions:
-         A list of event Subscription.
+         A list of subscription events.
         """
         for subscription in subscriptions:
             try:
                 data = {
                     'type': subscription['name'],
                     'version': subscription['version'],
                     'condition': {
@@ -360,20 +390,21 @@
                         'session_id': session_id
                     }
                 }
                 _logger.debug('Subscribing to `%s` event version %s.',
                               subscription['name'], subscription['version'])
                 route = Route(method='POST', path='eventsub/subscriptions')
                 await self.request(route=route, json=data)
-            except Forbidden as exc:
-                raise Forbidden(f'Subscription `{subscription["name"]}`'
-                                f' is missing proper authorization') from exc
-            except BadRequest as exc:
-                raise SubscriptionError(subscription=subscription['name'],
-                                        version=subscription['version']) from exc
+            except (Forbidden, BadRequest) as error:
+                if isinstance(error, Forbidden):
+                    _logger.error('Subscription type `%s` version `%s` is missing proper authorization.',
+                                  subscription['name'], subscription['version'])
+                if isinstance(error, BadRequest):
+                    _logger.warning('Subscription type `%s` version `%s` unsupported.',
+                                    subscription['name'], subscription['version'])
         self._dispatch('ready')
 
     async def get_client(self) -> UserType:
         """
         Retrieves the broadcaster with the associated access token.
         """
         data = await self.request(route=Route(method='GET', path='users'))
```

### Comparing `twitchify-1.2.0/twitch/message.py` & `twitchify-1.2.2/twitch/message.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.0/twitch/moderation.py` & `twitchify-1.2.2/twitch/moderation.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.0/twitch/reward.py` & `twitchify-1.2.2/twitch/reward.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.0/twitch/state.py` & `twitchify-1.2.2/twitch/state.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,20 +85,14 @@
             if data is None:
                 await parse()
             else:
                 await parse(data)
         except Exception as error:
             _logger.error('Failed to parse event: %s, %s', method, error)
 
-    async def parse_ready(self) -> None:
-        """
-        Parse ready event.
-        """
-        self._dispatch('ready')
-
     async def parse_channel_update(self, data: chl.Update) -> None:
         """
         Parse a channel update event.
         """
         _channel = ChannelUpdate(channel=data)
         self._dispatch('channel_update', _channel)
```

### Comparing `twitchify-1.2.0/twitch/stream.py` & `twitchify-1.2.2/twitch/stream.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.0/twitch/survey.py` & `twitchify-1.2.2/twitch/survey.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.0/twitch/types/channel.py` & `twitchify-1.2.2/twitch/types/stream.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,18 +18,26 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
-from typing import List
-from .user import Broadcaster
+from .user import SpecificUser
+from typing import TypedDict, Literal, List
 
 
-class Channel(Broadcaster):
-    broadcaster_language: str
-    game_name: str
+class Category(TypedDict):
     game_id: str
+    game_name: str
+
+
+class Stream(SpecificUser, Category):
+    id: str
     title: str
-    delay: int
+    language: str
     tags: List[str]
+    type: Literal['live', '']
+    is_mature: bool
+    viewer_count: int
+    thumbnail_url: str
+    started_at: str
```

### Comparing `twitchify-1.2.0/twitch/types/eventsub/channel.py` & `twitchify-1.2.2/twitch/types/eventsub/channel.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.0/twitch/types/eventsub/charity.py` & `twitchify-1.2.2/twitch/types/eventsub/charity.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.0/twitch/types/eventsub/goal.py` & `twitchify-1.2.2/twitch/types/eventsub/goal.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.0/twitch/types/eventsub/guest.py` & `twitchify-1.2.2/twitch/types/eventsub/guest.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.0/twitch/types/eventsub/hypertrain.py` & `twitchify-1.2.2/twitch/types/eventsub/hypertrain.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.0/twitch/types/eventsub/moderation.py` & `twitchify-1.2.2/twitch/types/eventsub/moderation.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.0/twitch/types/eventsub/poll.py` & `twitchify-1.2.2/twitch/types/eventsub/poll.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.0/twitch/types/eventsub/prediction.py` & `twitchify-1.2.2/twitch/types/eventsub/prediction.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.0/twitch/types/eventsub/reward.py` & `twitchify-1.2.2/twitch/types/eventsub/reward.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.0/twitch/types/eventsub/stream.py` & `twitchify-1.2.2/twitch/types/eventsub/stream.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.0/twitch/types/eventsub/subscriptions.py` & `twitchify-1.2.2/twitch/types/eventsub/subscriptions.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.0/twitch/types/eventsub/user.py` & `twitchify-1.2.2/twitch/types/eventsub/user.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.0/twitch/types/gateway.py` & `twitchify-1.2.2/twitch/types/gateway.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.0/twitch/types/http.py` & `twitchify-1.2.2/twitch/types/http.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,12 +29,12 @@
     client_id: str
     login: str
     scopes: List[str]
     user_id: str
     expires_in: int
 
 
-class Refresh(TypedDict):
+class Token(TypedDict):
     access_token: str
     refresh_token: str
     scope: List[str]
     token_type: str
```

### Comparing `twitchify-1.2.0/twitch/types/message.py` & `twitchify-1.2.2/twitch/types/message.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.0/twitch/types/stream.py` & `twitchify-1.2.2/twitch/types/channel.py`

 * *Files 27% similar despite different names*

```diff
@@ -18,26 +18,20 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
-from .user import SpecificUser
-from typing import TypedDict, Literal, List
+from typing import List
+from .user import Broadcaster
 
 
-class Category(TypedDict):
-    game_id: str
+class Channel(Broadcaster):
+    broadcaster_language: str
     game_name: str
-
-
-class Stream(SpecificUser, Category):
-    id: str
+    game_id: str
     title: str
-    language: str
+    delay: int
     tags: List[str]
-    type: Literal['live', '']
-    is_mature: bool
-    viewer_count: int
-    thumbnail_url: str
-    started_at: str
+    content_classification_labels: List[str]
+    is_branded_content: bool
```

### Comparing `twitchify-1.2.0/twitch/types/user.py` & `twitchify-1.2.2/twitch/types/user.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.0/twitch/user.py` & `twitchify-1.2.2/twitch/user.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.0/twitchify.egg-info/PKG-INFO` & `twitchify-1.2.2/twitchify.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitchify
-Version: 1.2.0
+Version: 1.2.2
 Summary: A Python library for Twitch's WebSocket EventSub integration.
 Home-page: https://github.com/mrsnifo/twitchify
 Author: Snifo
 Author-email: Snifo@mail.com
 License: MIT
 Project-URL: Issue tracker, https://github.com/mrsnifo/twitchify/issues
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,48 +21,74 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Twitchify
 
----
-
 [![Discord](https://img.shields.io/discord/938786168592547880)](https://discord.gg/hH4ZkNg6cA)
 [![PyPI Version](https://img.shields.io/pypi/v/twitchify)](https://pypi.org/project/twitchify)
-![Python versions](https://img.shields.io/pypi/pyversions/twitchify)
+[![Python versions](https://img.shields.io/pypi/pyversions/twitchify)](https://pypi.org/project/twitchify)
 
-Python library for Twitch's WebSocket **EventSub** integration
+Python library for Twitch's WebSocket **EventSub** integration.
 
 ## Features
 - Comprehensive support for WebSocket EventSub, providing real-time Twitch event notifications.
 - User-friendly interfaces for seamless integration.
 - Built-in support for type hinting, ensuring code clarity and maintainability.
 
 ## Installation
-
 You can install Twitchify using pip:
 
 ```shell
 # Windows
 py -3 -m pip install -U twitchify
 
 # Linux/macOS
 python3 -m pip install -U twitchify
 ```
 
-## Documentation
-Please refer to the [Events Documentation](https://github.com/MrSniFo/Twitchify/blob/main/docs/EVENTS.md) for detailed information on handling events with Twitchify.
-
 ## Quick Example
 ```python
 from twitch import Client
 from twitch.user import Follower
 
-client = Client(client_id="CLIENT ID HERE")
+client = Client(client_id="YOUR_CLIENT_ID")
+
+@client.event
+async def on_ready():
+    """
+    Event handler triggered when the client is ready to start processing events.
+    """
+    print("Ready as %s" % client.user.display_name)
+
+
+@client.event
+async def on_follow(user: Follower):
+    """
+    Event handler triggered when a user follows the channel.
+    """
+    print("%s just followed you!" % user.display_name)
+
+# Run the client with your user access token.
+client.run(access_token="YOUR_ACCESS_TOKEN")
+```
+
+### With built-in Authorization
+
+```python
+from twitch import Client
+from twitch.user import Follower
+
+# Initialize the Twitch client with your client ID and client secret.
+client = Client(client_id="YOUR_CLIENT_ID", client_secret="YOUR_CLIENT_SECRET")
+
+# Generate the authorization URL for the Twitch client.
+# The user should visit the provided URL to authorize the app.
+auth = client.auth()
 
 @client.event
 async def on_ready():
     """
     Event handler triggered when the client is ready to start processing events.
     """
     print("Ready as %s" % client.user.display_name)
@@ -71,9 +97,12 @@
 @client.event
 async def on_follow(user: Follower):
     """
     Event handler triggered when a user follows the channel.
     """
     print("%s just followed you!" % user.display_name)
 
-client.run(access_token="USER ACCESS TOKEN HERE")
+# You can store the access token and refresh token for future use, so you don't have to authorize again.
+client.run(access_token=auth.access_token, refresh_token=auth.refresh_token)
 ```
+
+Please refer to the [Documentation](https://github.com/MrSniFo/Twitchify/blob/main/docs) or [Examples](https://github.com/MrSniFo/Twitchify/tree/main/examples) for more details.
```

### Comparing `twitchify-1.2.0/twitchify.egg-info/SOURCES.txt` & `twitchify-1.2.2/twitchify.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 twitch/__init__.py
+twitch/auth.py
 twitch/broadcaster.py
 twitch/channel.py
 twitch/client.py
 twitch/errors.py
 twitch/gateway.py
 twitch/goals.py
 twitch/guest.py
@@ -19,14 +20,15 @@
 twitch/user.py
 twitch/utils.py
 twitch/types/__init__.py
 twitch/types/channel.py
 twitch/types/gateway.py
 twitch/types/http.py
 twitch/types/message.py
+twitch/types/scoopes.py
 twitch/types/stream.py
 twitch/types/user.py
 twitch/types/eventsub/__init__.py
 twitch/types/eventsub/channel.py
 twitch/types/eventsub/charity.py
 twitch/types/eventsub/goal.py
 twitch/types/eventsub/guest.py
```

