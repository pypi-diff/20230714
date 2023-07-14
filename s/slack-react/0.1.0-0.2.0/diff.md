# Comparing `tmp/slack-react-0.1.0.tar.gz` & `tmp/slack-react-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slack-react-0.1.0.tar", last modified: Fri Jul 14 09:21:56 2023, max compression
+gzip compressed data, was "slack-react-0.2.0.tar", last modified: Fri Jul 14 13:41:06 2023, max compression
```

## Comparing `slack-react-0.1.0.tar` & `slack-react-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:21:56.343261 slack-react-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:21:56.339261 slack-react-0.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-14 09:21:46.000000 slack-react-0.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:21:56.339261 slack-react-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-14 09:21:46.000000 slack-react-0.1.0/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-14 09:21:46.000000 slack-react-0.1.0/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-14 09:21:46.000000 slack-react-0.1.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-14 09:21:46.000000 slack-react-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-14 09:21:46.000000 slack-react-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    40881 2023-07-14 09:21:56.343261 slack-react-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-14 09:21:46.000000 slack-react-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 09:21:56.343261 slack-react-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:21:56.343261 slack-react-0.1.0/slack_react.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    40881 2023-07-14 09:21:56.000000 slack-react-0.1.0/slack_react.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-14 09:21:56.000000 slack-react-0.1.0/slack_react.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 09:21:56.000000 slack-react-0.1.0/slack_react.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-14 09:21:56.000000 slack-react-0.1.0/slack_react.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-14 09:21:56.000000 slack-react-0.1.0/slack_react.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 09:21:56.000000 slack-react-0.1.0/slack_react.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     6145 2023-07-14 09:21:46.000000 slack-react-0.1.0/slack_react.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:41:06.599960 slack-react-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:41:06.595960 slack-react-0.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-14 13:40:53.000000 slack-react-0.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:41:06.595960 slack-react-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-14 13:40:53.000000 slack-react-0.2.0/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-14 13:40:53.000000 slack-react-0.2.0/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-14 13:40:53.000000 slack-react-0.2.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-14 13:40:53.000000 slack-react-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-14 13:40:53.000000 slack-react-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    42415 2023-07-14 13:41:06.599960 slack-react-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-14 13:40:53.000000 slack-react-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-14 13:40:53.000000 slack-react-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 13:41:06.599960 slack-react-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:41:06.599960 slack-react-0.2.0/slack_react.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42415 2023-07-14 13:41:06.000000 slack-react-0.2.0/slack_react.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-14 13:41:06.000000 slack-react-0.2.0/slack_react.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 13:41:06.000000 slack-react-0.2.0/slack_react.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-14 13:41:06.000000 slack-react-0.2.0/slack_react.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-14 13:41:06.000000 slack-react-0.2.0/slack_react.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 13:41:06.000000 slack-react-0.2.0/slack_react.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6729 2023-07-14 13:40:53.000000 slack-react-0.2.0/slack_react.py
```

### Comparing `slack-react-0.1.0/.github/workflows/pypi.yaml` & `slack-react-0.2.0/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `slack-react-0.1.0/.github/workflows/release.yaml` & `slack-react-0.2.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `slack-react-0.1.0/LICENSE` & `slack-react-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `slack-react-0.1.0/PKG-INFO` & `slack-react-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slack-react
-Version: 0.1.0
+Version: 0.2.0
 Summary: Add reactions that spell out messages to Slack messages
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -679,7 +679,66 @@
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Keywords: slack,reactions
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+
+# 💬 slack-react 🚀
+
+Automate your Slack reactions! This Python project allows you to automatically
+add emoji reactions to Slack messages. The emojis are generated based on a 
+user-provided message, with each character in the message converted to a 
+corresponding emoji.
+
+## 📚 Table of Contents
+
+- [Installation](#installation)
+- [Usage](#usage)
+- [Examples](#examples)
+- [License](#license)
+
+## ⚙️ Installation
+
+```bash
+pipx install slack-react
+```
+
+## 🛠 Usage
+
+Before using this project, you need to get your Slack OAUTH token. 
+
+Refer to [this guide](https://api.slack.com/authentication/token-types) to 
+create and install a Slack app to get your token.
+
+Once you have your token, set it as an environment variable.
+
+```bash
+export SLACK_OAUTH_USER_TOKEN=your-slack-token
+```
+
+Now you're ready to use the project! You can run the script using the following
+command:
+
+```bash
+python slack_react.py "your message" -c "your-channel"
+```
+
+Replace `"your message"` with the message you want to spell out with reactions.
+Replace `"your-channel"` with the name of the channel where you want to add the
+reactions. 
+The script will convert each character in the message to a corresponding emoji 
+and add these emojis as reactions to the most recent message in the 
+specified channel.
+
+## 📖 Examples
+
+```bash
+python slack_react.py -c "general" "hello" 
+```
+
+This command will spell out "hello" in emoji reactions in the "general" channel.
+
+## 📜 License
+
+This project is licensed under the [GPL-3.0 License](./LICENSE).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `slack-react-0.1.0/pyproject.toml` & `slack-react-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,14 @@
 classifiers = [
   "Programming Language :: Python :: 3",
 ]
 dependencies = [
   "rich",
   "slack_sdk"
 ]
-version = "0.1.0"
+version = "0.2.0"
 
 [tool.black]
 line-length = 79
 
 [project.scripts]
 slack-react = "slack_react:main"
```

### Comparing `slack-react-0.1.0/slack_react.egg-info/PKG-INFO` & `slack-react-0.2.0/slack_react.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slack-react
-Version: 0.1.0
+Version: 0.2.0
 Summary: Add reactions that spell out messages to Slack messages
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -679,7 +679,66 @@
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Keywords: slack,reactions
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+
+# 💬 slack-react 🚀
+
+Automate your Slack reactions! This Python project allows you to automatically
+add emoji reactions to Slack messages. The emojis are generated based on a 
+user-provided message, with each character in the message converted to a 
+corresponding emoji.
+
+## 📚 Table of Contents
+
+- [Installation](#installation)
+- [Usage](#usage)
+- [Examples](#examples)
+- [License](#license)
+
+## ⚙️ Installation
+
+```bash
+pipx install slack-react
+```
+
+## 🛠 Usage
+
+Before using this project, you need to get your Slack OAUTH token. 
+
+Refer to [this guide](https://api.slack.com/authentication/token-types) to 
+create and install a Slack app to get your token.
+
+Once you have your token, set it as an environment variable.
+
+```bash
+export SLACK_OAUTH_USER_TOKEN=your-slack-token
+```
+
+Now you're ready to use the project! You can run the script using the following
+command:
+
+```bash
+python slack_react.py "your message" -c "your-channel"
+```
+
+Replace `"your message"` with the message you want to spell out with reactions.
+Replace `"your-channel"` with the name of the channel where you want to add the
+reactions. 
+The script will convert each character in the message to a corresponding emoji 
+and add these emojis as reactions to the most recent message in the 
+specified channel.
+
+## 📖 Examples
+
+```bash
+python slack_react.py -c "general" "hello" 
+```
+
+This command will spell out "hello" in emoji reactions in the "general" channel.
+
+## 📜 License
+
+This project is licensed under the [GPL-3.0 License](./LICENSE).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `slack-react-0.1.0/slack_react.py` & `slack-react-0.2.0/slack_react.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 import argparse
 import os
 import re
+import sys
 
 import slack_sdk
 from rich import print
 
 
 def parse_args():
     # create the top-level parser
@@ -35,19 +36,19 @@
 
     return parser.parse_args()
 
 
 def message_to_emoji_list(message):
     # mapping of alphabets to their corresponding emoji names
     emoji_mapping = {
-        "a": ["alphabet-white-a", "alphabet-yellow-a"],
-        "b": ["alphabet-white-b", "alphabet-yellow-b"],
+        "a": ["a", "alphabet-white-a", "alphabet-yellow-a"],
+        "b": ["b", "alphabet-white-b", "alphabet-yellow-b"],
         "c": ["alphabet-white-c", "alphabet-yellow-c"],
         "d": ["alphabet-white-d", "alphabet-yellow-d"],
-        "e": ["alphabet-white-e", "alphabet-yellow-e"],
+        "e": ["alphabet-white-e", "alphabet-yellow-e", "e-mail"],
         "f": ["alphabet-white-f", "alphabet-yellow-f"],
         "g": ["alphabet-white-g", "alphabet-yellow-g"],
         "h": ["alphabet-white-h", "alphabet-yellow-h"],
         "i": ["alphabet-white-i", "alphabet-yellow-i"],
         "j": ["alphabet-white-j", "alphabet-yellow-j"],
         "k": ["alphabet-white-k", "alphabet-yellow-k"],
         "l": ["alphabet-white-l", "alphabet-yellow-l"],
@@ -75,28 +76,40 @@
         "7": ["seven", "seven"],
         "8": ["eight", "eight"],
         "9": ["nine", "nine"],
     }
 
     # create a list to hold the emojis
     emojis = []
+    # create a dictionary to hold the index of the next emoji to use for
+    # each character
+    next_emoji_index = {}
 
     # iterate over each character in the message
     for char in message:
         # convert the character to lowercase
         char = char.lower()
 
-        # if the character is in the mapping, add the corresponding emoji to the list
+        # if the character is in the mapping
         if char in emoji_mapping:
-            # use the first emoji if it's not already in the list
-            if emoji_mapping[char][0] not in emojis:
-                emojis.append(emoji_mapping[char][0])
-            # otherwise use the second emoji
-            else:
-                emojis.append(emoji_mapping[char][1])
+            # if the character is not in next_emoji_index, this is the first
+            # time we've seen it
+            if char not in next_emoji_index:
+                next_emoji_index[char] = 0
+
+            # get the next emoji for this character
+            emoji = emoji_mapping[char][next_emoji_index[char]]
+
+            # add the emoji to the list
+            emojis.append(emoji)
+
+            # update the index of the next emoji to use for this character
+            next_emoji_index[char] = (next_emoji_index[char] + 1) % len(
+                emoji_mapping[char]
+            )
 
     return emojis
 
 
 def get_user_id(client):
     response = client.auth_test()
 
@@ -170,26 +183,32 @@
 
     # create a client instance
     client = slack_sdk.WebClient(token=args.token)
 
     channel_id = get_channel_id(client, args.channel)
 
     if not channel_id:
-        print(f"Channel '{args.channel}' not found")
+        print(f"Channel '{args.channel}' not found", file=sys.stderr)
         return 1
 
     response = client.conversations_history(channel=channel_id)
 
     if args.message:
         message = find_matching_message(client, channel_id, args.message)
+        if not message:
+            print("Message not found", file=sys.stderr)
+            return 1
         ts = message["ts"]
     else:
+        # Default to last message
         ts = response["messages"][0]["ts"]
 
     remove_reactions(client, channel_id, ts)
 
     if args.reaction and not args.remove:
         add_reactions(client, channel_id, ts, args.reaction)
 
+    return 0
+
 
 if __name__ == "__main__":
-    main()
+    sys.exit(main())
```

