# Comparing `tmp/umshini-0.0.7.tar.gz` & `tmp/umshini-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umshini-0.0.7.tar", last modified: Sat Jun  3 01:06:54 2023, max compression
+gzip compressed data, was "umshini-0.0.8.tar", last modified: Fri Jul 14 21:42:11 2023, max compression
```

## Comparing `umshini-0.0.7.tar` & `umshini-0.0.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 01:06:54.123701 umshini-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    34629 2023-06-03 01:06:45.000000 umshini-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    40723 2023-06-03 01:06:54.123701 umshini-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-03 01:06:45.000000 umshini-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 01:06:54.119701 umshini-0.0.7/Umshini/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-03 01:06:45.000000 umshini-0.0.7/Umshini/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 01:06:54.119701 umshini-0.0.7/Umshini/envs/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-03 01:06:45.000000 umshini-0.0.7/Umshini/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-03 01:06:45.000000 umshini-0.0.7/Umshini/envs/envs_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-03 01:06:45.000000 umshini-0.0.7/Umshini/example_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-03 01:06:45.000000 umshini-0.0.7/Umshini/learner.py
--rw-r--r--   0 runner    (1001) docker     (123)    14858 2023-06-03 01:06:45.000000 umshini-0.0.7/Umshini/tournament_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 01:06:54.119701 umshini-0.0.7/Umshini/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 01:06:45.000000 umshini-0.0.7/Umshini/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-03 01:06:45.000000 umshini-0.0.7/Umshini/utils/compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-03 01:06:45.000000 umshini-0.0.7/Umshini/utils/socket_wrap.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-03 01:06:45.000000 umshini-0.0.7/Umshini/utils/test_compression.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-03 01:06:45.000000 umshini-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 01:06:54.123701 umshini-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-03 01:06:45.000000 umshini-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 01:06:54.123701 umshini-0.0.7/umshini.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    40723 2023-06-03 01:06:54.000000 umshini-0.0.7/umshini.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-03 01:06:54.000000 umshini-0.0.7/umshini.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 01:06:54.000000 umshini-0.0.7/umshini.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-03 01:06:54.000000 umshini-0.0.7/umshini.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-03 01:06:54.000000 umshini-0.0.7/umshini.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:42:11.271493 umshini-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    34629 2023-07-14 21:42:08.000000 umshini-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    42840 2023-07-14 21:42:11.271493 umshini-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-14 21:42:08.000000 umshini-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-14 21:42:08.000000 umshini-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 21:42:11.271493 umshini-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-14 21:42:08.000000 umshini-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:42:11.267492 umshini-0.0.8/umshini/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-14 21:42:08.000000 umshini-0.0.8/umshini/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:42:11.271493 umshini-0.0.8/umshini/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-14 21:42:08.000000 umshini-0.0.8/umshini/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-14 21:42:08.000000 umshini-0.0.8/umshini/envs/envs_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-07-14 21:42:08.000000 umshini-0.0.8/umshini/example_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-14 21:42:08.000000 umshini-0.0.8/umshini/learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15361 2023-07-14 21:42:08.000000 umshini-0.0.8/umshini/tournament_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:42:11.271493 umshini-0.0.8/umshini/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 21:42:08.000000 umshini-0.0.8/umshini/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-14 21:42:08.000000 umshini-0.0.8/umshini/utils/compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-14 21:42:08.000000 umshini-0.0.8/umshini/utils/socket_wrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-14 21:42:08.000000 umshini-0.0.8/umshini/utils/test_compression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:42:11.271493 umshini-0.0.8/umshini.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42840 2023-07-14 21:42:11.000000 umshini-0.0.8/umshini.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-14 21:42:11.000000 umshini-0.0.8/umshini.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 21:42:11.000000 umshini-0.0.8/umshini.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-14 21:42:11.000000 umshini-0.0.8/umshini.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 21:42:11.000000 umshini-0.0.8/umshini.egg-info/top_level.txt
```

### Comparing `umshini-0.0.7/LICENSE` & `umshini-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `umshini-0.0.7/PKG-INFO` & `umshini-0.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: umshini
-Version: 0.0.7
+Version: 0.0.8
 Summary: Umshini client for playing in MARL tournaments
-Home-page: https://github.com/umshini/umshini
-Author: umshini team
 Author-email: "Jordan K. Terry" <j.k.terry@swarmlabs.com>
 License: This code is copyright Jordan Terry, 2021, and is released under the GNU AGPLv3 license, included below:
         
                             GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -667,22 +665,63 @@
           You should also get your employer (if you work as a programmer) or school,
         if any, to sign a "copyright disclaimer" for the program, if necessary.
         For more information on this, and how to apply and follow the GNU AGPL, see
         <https://www.gnu.org/licenses/>.
         
 Project-URL: Homepage, https://github.com/umshini/umshini
 Keywords: Reinforcement Learning,game,RL,AI,gym
-Classifier: Programming Language :: Python
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6, <3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: <3.10,>=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: classic
+Provides-Extra: llm
+Provides-Extra: all
 License-File: LICENSE
 
-# Colosseum
+# Umshini-Client
 
-To run the Colosseum server for testing, refer to [the server repo](https://github.com/PettingZoo-Team/Colosseum-Server).
+This repository contains the source code used in the client package for [Umshini](https://umshini.ai/). 
 
-To run one or multiple clients you can use the following command:
+For full documentation and usage information, see https://umshini.ai/documentation
 
-```
-python test_tournament_clients user1 user2 ...
-```
+## Installation & Connection
+1. **Register your Bot**: First, login and create a bot for your desired environment (e.g. Connect Four) on the account page. 
+2. **Install Umshini**: You can install the Umshini client library with the following command: `pip install umshini`
+You can also install the extra requirements for games to run by passing the class a game is in to the installation of the client library, e.g. `pip install umshini[classic]` Or `pip install umshini[llm]`
+3. **Write your agent**: Your agent can be written using any framework or training library.
+4. **Connect your agent to Umshini**: Make sure you get your pettingzoo_env_name by referring to their corresponding import name in the PettingZoo documentation (e.g. for Atari Combat: Tank you’ll use combat_tank_v2). Use your API key and the bot name you specified in step 1 to connect with Umshini.
+
+## Example Usage
+
+This is an example of how to use umshini to compete in a Connect Four tournament. 
+
+After bot registration and noting down your API key and bot name, you can follow the following steps:
+### Install Umshini 
+```pip install umshini[classic]```
+### Write your Agent
+
+The code below is an agent that plays Connect Four with random (legal) actions.
+
+```    
+import umshini
+import numpy as np
+
+def my_bot(obs, rew, term, trunc, info):
+    """
+    Return a random legal action.
+    """
+    legal_mask = obs["action_mask"]
+    legal_action = legal_mask.nonzero()[0]
+    action = np.random.choice(legal_actions)
+    return (action, surprise)
+
+# Call 'connect' from the umshini package
+# with your user info and the “connect_four_v3” as the first arg.
+umshini.connect("connect_four_v3", "Bot-Name", "API_Key", my_bot)
+```    
+  
+And that's it! Running this script during a tournament will allow your bot to compete! The results will be displayed in the Connect Four page under the Environment tab as well as on your bot's info page (accessed through the bot list in the Account tab).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `umshini-0.0.7/Umshini/example_client.py` & `umshini-0.0.8/umshini/example_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,65 @@
 #!/usr/bin/env python3
-# -*- coding: utf-8 -*-
+# pyright: reportOptionalMemberAccess=false
 import time
 import traceback
-from .tournament_client import TournamentConnection
+
 from colorama import Fore, Style
-from halo import Halo
+
+from .tournament_client import TournamentConnection
 
 
 class ColosseumTournamentAgent:
-    def __init__(self, policy, latency=0,  games=["__all__"], port=12345,
-                 direct=False, host="localhost", maximum_rounds=10000, debug=False):
+    def __init__(
+        self,
+        policy,
+        latency=0,
+        games=["__all__"],
+        port=12345,
+        direct=False,
+        host="localhost",
+        maximum_rounds=10000,
+        debug=False,
+    ):
         self.host = host
         self.policy = policy
         self.port = port
-        self.botname = ''
-        self.key = ''
+        self.botname = ""
+        self.key = ""
         self.latency = latency
         self.direct = direct
         self.games = games
         self.tournament = None
         self.maximum_rounds = maximum_rounds
         self.debug = debug
 
     def connect(self, botname, key):
         self.botname = botname
         self.key = key
         try:
             # TODO: Use policy for test
             # Test that policy runs without errors in local environments
             self.tournament = TournamentConnection(
-                self.host, self.port, self.botname, self.key,
-                available_games=self.games, debug=self.debug
+                self.host,
+                self.port,
+                self.botname,
+                self.key,
+                available_games=self.games,
+                debug=self.debug,
+            )
+            print(
+                Fore.GREEN
+                + f"Bot: {self.botname}'s policy has passed environment verifications"
             )
-            print(Fore.GREEN + f"Bot: {self.botname}'s policy has passed environment verifications")
             print(Style.RESET_ALL)
         except Exception:
-            print(Fore.RED + f"Bot: {self.botname}'s policy has failed verification testing in environment: {self.games}")
+            print(
+                Fore.RED
+                + f"Bot: {self.botname}'s policy has failed verification testing in environment: {self.games}"
+            )
             print(Style.RESET_ALL)
             quit()
 
     def run(self):
         # Connect to tournament server each round, until the end signal is received.
         try:
             env = self.tournament.next_match()
@@ -58,16 +78,20 @@
             timestep = 0
             rew = info = None
             obs = env.reset()
             while not (term or trunc):
                 if timestep % 100 == 0 and self.debug:
                     print(f"{self.botname}: Timestep {timestep}\n")
                 time.sleep(self.latency / 1000)  # Used to simulate network latency
-                action_surprise = self.policy(obs, rew, term, trunc, info)  # receive action and surprise from user
-                obs, rew, term, trunc, info = env.step(action_surprise)  # Send action to game server
+                action_surprise = self.policy(
+                    obs, rew, term, trunc, info
+                )  # receive action and surprise from user
+                obs, rew, term, trunc, info = env.step(
+                    action_surprise
+                )  # Send action to game server
                 timestep += 1
             print(Fore.GREEN + f"Round {current_round} complete")
             print(Style.RESET_ALL)
             current_round += 1
             if current_round > self.maximum_rounds:
                 env = None
             else:
```

### Comparing `umshini-0.0.7/Umshini/learner.py` & `umshini-0.0.8/umshini/learner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,47 @@
+# pyright: reportGeneralTypeIssues=false
+
+from colorama import Fore, Style
+
 from .example_client import ColosseumTournamentAgent
 from .tournament_client import TestEnv
-from colorama import Fore, Style
 
 
 def create_and_run(botname, user_key):
     agent = ColosseumTournamentAgent(maximum_rounds=100)
     agent.connect(botname, user_key)
     agent.run()
 
 
 def connect(environment, botname, user_key, user_policy, debug=False, testing=False):
-    """
-    User end function to add their RL policy
+    """User end function to add their RL policy.
 
     Passed function accepts parameters:
         policy(observation, reward, done, info)
 
     Passed function returns action
     """
     if testing:
-        agent = ColosseumTournamentAgent(policy=user_policy, games=[environment], maximum_rounds=100, host="127.0.0.1",
-                                         port="8803", debug=debug)
+        agent = ColosseumTournamentAgent(
+            policy=user_policy,
+            games=[environment],
+            maximum_rounds=100,
+            host="127.0.0.1",
+            port="8803",
+            debug=debug,
+        )
     else:
-        agent = ColosseumTournamentAgent(policy=user_policy, games=[environment], maximum_rounds=100, host="34.70.234.149",
-                                        port="8803", debug=debug)
+        agent = ColosseumTournamentAgent(
+            policy=user_policy,
+            games=[environment],
+            maximum_rounds=100,
+            host="34.70.234.149",
+            port="8803",
+            debug=debug,
+        )
 
     agent.connect(botname, user_key)
     agent.run()
 
 
 def test(environment, user_policy):
     test_env = TestEnv(environment)
@@ -35,14 +49,17 @@
     obs = rew = info = None
     for _ in range(100):
         try:
             (action, surprise) = user_policy(obs, rew, term, trunc, info)
             obs, rew, term, trunc, info = test_env.step(action)
 
             if term or trunc:
-                print(Fore.GREEN + "Policy has passed verification testing in {}".format(environment))
+                print(
+                    Fore.GREEN
+                    + f"Policy has passed verification testing in {environment}"
+                )
                 print(Style.RESET_ALL)
                 break
-        except:
+        except:  # noqa: E722
             print(Fore.RED + "Policy has failed verification testing")
             print(Style.RESET_ALL)
             quit()
```

### Comparing `umshini-0.0.7/Umshini/tournament_client.py` & `umshini-0.0.8/umshini/tournament_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,53 +1,56 @@
-import errno
-import gymnasium as gym
+# pyright: reportGeneralTypeIssues=false, reportUnboundVariable=false, reportOptionalMemberAccess=false
 import json
-import numpy as np
 import socket
-from socket import error as socket_error
-from Umshini.utils.socket_wrap import SocketWrapper
-from Umshini.utils.compress import decompress
-from Umshini.envs import make_test_env, ALL_ENVIRONMENTS
+
+import gymnasium as gym
+import numpy as np
 from colorama import Fore, Style
 from halo import Halo
 
+from umshini.envs import ALL_ENVIRONMENTS, make_test_env
+from umshini.utils.compress import decompress
+from umshini.utils.socket_wrap import SocketWrapper
+
 
 # Send JSON through socket
 def send_json(sock, data):
     return sock.sendall(json.dumps(data).encode("utf-8"))
 
 
 # Receive JSON from socket
 def recv_json(sock, timeout=30):
     sock.settimeout(timeout)
-    data = sock.recv(2 ** 30)  # Arbitrarily large buffer
+    data = sock.recv(2**30)  # Arbitrarily large buffer
     sock.settimeout(30)
     return data
 
 
 class NetworkEnv(gym.Env):
     def __init__(self, env_id, seed, game_ip, game_port, username, token, verbose=0):
         self.verbose = verbose
         if self.verbose > 0:
-            print("Host: {}:{}".format(game_ip, game_port))
+            print(f"Host: {game_ip}:{game_port}")
         self.game_connection = SocketWrapper(
             socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         )
         # Create game server connection
         self.game_connection.connect((game_ip, game_port))
         send_json(self.game_connection, {"username": username, "token": token})
         self.game_data = recv_json(self.game_connection)
         self.terminated = self.game_data["type"] == "terminate"
 
         # Create env for initial action and observation spaces
         self.env, self.turn_based = make_test_env(env_id, seed=seed)
         if self.verbose > 1:
             print("Game server data:", self.game_data)
         self.agent = (
-            self.game_data["agent"] if not self.terminated else self.env.possible_agents[0]
+            self.game_data["agent"]
+            if not self.terminated
+            else self.env.possible_agents[0]
         )
         self.observation_space = self.env.observation_space(self.agent)
         self.action_space = self.env.action_space(self.agent)
         self.action_space.seed(seed)
         self.obs = None
 
     def step(self, action_surprise):
@@ -55,28 +58,31 @@
             print("terminated before single step occurred!")
             return self.obs, 0, True, True, {}
         if type(action_surprise) is tuple:
             action = action_surprise[0]
             surprise = action_surprise[1]
         else:
             action = action_surprise
-            action_surprise = 0.0
+            surprise = 0.0
         # Convert Numpy types to Python types
         if hasattr(action, "dtype"):
             action = action.item()
 
         # Send action to game server
-        assert (isinstance(action, int) or
-                isinstance(action, float) or
-                isinstance(action, str) or
-                isinstance(action, dict) or
-                isinstance(action, list)), "Action is not a valid type."
+        assert (
+            isinstance(action, int)
+            or isinstance(action, float)
+            or isinstance(action, str)
+            or isinstance(action, dict)
+            or isinstance(action, list)
+        ), "Action is not a valid type."
         assert self.action_space.contains(action), "Action not in action space."
-        assert (isinstance(surprise, int) or
-                isinstance(surprise, float)), "Surprise is not a valid type."
+        assert isinstance(surprise, int) or isinstance(
+            surprise, float
+        ), "Surprise is not a valid type."
 
         act_data = {"type": "action", "action": action, "surprise": surprise}
         if self.verbose > 1:
             print("sending action")
         send_json(self.game_connection, act_data)
         if self.verbose > 1:
             print("sent action")
@@ -107,21 +113,26 @@
         info = {}
         term = False
         trunc = False
         self.steps += 1
         self.spinner.text = f"Playing game (step: {self.steps})"
         return obs, rew, term, trunc, info
 
-    def render(self, mode='human'):
+    def render(self, mode="human"):
         # TODO: Figure out appropriate behavior here. Probably rendering live on the website.
         return self.env.render(mode=mode)
 
     def reset(self):
         self.steps = 0
-        self.spinner = Halo(text=f"Playing game (step: {self.steps})", text_color='cyan', color='green', spinner='dots')
+        self.spinner = Halo(
+            text=f"Playing game (step: {self.steps})",
+            text_color="cyan",
+            color="green",
+            spinner="dots",
+        )
         self.spinner.start()
         # Get initial observation
         if self.verbose > 1:
             print("receiving initial obs")
         observation_data = recv_json(self.game_connection)
         if self.verbose > 1:
             print("received initial obs")
@@ -160,19 +171,21 @@
         self.num_steps = 0
         self.was_term = False
         self.was_trunc = False
         obss, info = self.env.reset()
         return obss, info
 
     def step(self, action):
-        assert not self.was_term and not self.was_trunc, "stepped after term or trunc, should terminate loop"
-
+        assert (
+            not self.was_term and not self.was_trunc
+        ), "stepped after term or trunc, should terminate loop"
         # Set random actions for all other agents in parallel game or None in turn-based game
         actions = {
-            agent: (None if self.turn_based else self.env.action_space(agent).sample()) for agent in self.env.agents
+            agent: (None if self.turn_based else self.env.action_space(agent).sample())
+            for agent in self.env.agents
         }
         actions[self.env.aec_env.agent_selection] = action
         self.obss, rews, terms, truncs, infos = self.env.step(actions)
 
         if self.num_steps > 50:
             trunc = True
             term = True
@@ -193,33 +206,35 @@
             active_agents = [self.env.unwrapped.agent_selection]
         else:
             active_agents = self.env.agents
 
         # Step again if testing agent is not next
         if not self.was_term and not self.was_trunc and self.agent not in active_agents:
             obs = self.obss[self.env.unwrapped.agent_selection]
-            if (isinstance(obs, dict) and "action_mask" in obs):
+            if isinstance(obs, dict) and "action_mask" in obs:
                 legal_mask = obs["action_mask"]
                 legal_actions = legal_mask.nonzero()[0]
                 action = np.random.choice(legal_actions)
             else:
-                action = self.env.action_space(self.env.unwrapped.agent_selection).sample()
+                action = self.env.action_space(
+                    self.env.unwrapped.agent_selection
+                ).sample()
             return self.step(action)
         else:
             return obs, rew, term, trunc, info
 
-    def render(self, mode='human'):
+    def render(self, mode="human"):
         return
 
 
 # Local environment used to test if agent works before connecting to network env
 class TestAECEnv(gym.Env):
     def __init__(self, env_id):
         seed = 1
-        self.env = make_test_env(env_id, seed=seed, turn_based=True)
+        self.env = make_test_env(env_id, seed=seed)
         self.env.reset()
         self.agent = agent = self.env.agents[0]
         self.observation_space = self.env.observation_spaces[agent]
         self.action_space = self.env.action_spaces[agent]
         self.num_steps = 0
         self.was_term = False
         self.was_trunc = False
@@ -227,15 +242,17 @@
     def reset(self):
         self.num_steps = 0
         self.was_term = False
         self.was_trunc = False
         self.env.reset()
 
     def step(self, action):
-        assert not self.was_term and not self.was_trunc, "stepped after term or trunc, should terminate loop"
+        assert (
+            not self.was_term and not self.was_trunc
+        ), "stepped after term or trunc, should terminate loop"
         # Set random actions for all other agents
         self.env.step(action)
         if self.num_steps > 50:
             trunc = True
             term = True
         else:
             obs, rew, term, trunc, info = self.env.last()
@@ -243,15 +260,15 @@
         self.was_term = term
         self.was_trunc = trunc
         self.num_steps += 1
 
     def last(self):
         return self.env.last()
 
-    def render(self, mode='human'):
+    def render(self, mode="human"):
         return
 
 
 class TournamentConnection:
     def __init__(self, ip, port, botname, key, available_games, debug=False):
         # Initialize class variables
         self.botname = botname
@@ -275,47 +292,55 @@
         self._test_environments()
 
     # Test agent in every game
     def _test_environments(self):
         for game in self.available_games:
             test_env = TestEnv(game)
             obs, info = test_env.reset()
-            for _ in range(100):
-                if (obs is not None
+            for i in range(100):
+                if (
+                    obs is not None
                     and isinstance(obs, dict)
-                    and obs and "action_mask" in obs):
+                    and obs
+                    and "action_mask" in obs
+                ):
                     action = np.random.choice(obs["action_mask"].nonzero()[0])
                 else:
                     action = test_env.action_space.sample()
                 obs, _, term, trunc, _ = test_env.step(action)
                 if term or trunc:
-                    if self.debug: print("{} passed test in {}".format(self.botname, game))
+                    if self.debug:
+                        print(f"{self.botname} passed test in {game}")
                     break
 
     def _connect_game_server(self):
         # If tournament is over, return no environment
         if self.tournament_completed:
             return None
 
         # Receive game server info from matchmaker
-        spinner = Halo(text='Waiting for players', text_color='cyan', color='green', spinner='dots')
+        spinner = Halo(
+            text="Waiting for players", text_color="cyan", color="green", spinner="dots"
+        )
         spinner.start()
         try:
             ready_data = recv_json(self.main_connection, timeout=60)
         except TimeoutError as err:
             print("Not enough players to start tournament.", flush=True)
             raise err
         spinner.succeed()
 
         if self.debug:
             print(ready_data)
         send_json(self.main_connection, {"type": "ready"})
 
         # Receive game server info from matchmaker
-        spinner = Halo(text='Creating your game', text_color='cyan', color='green', spinner='dots')
+        spinner = Halo(
+            text="Creating your game", text_color="cyan", color="green", spinner="dots"
+        )
         spinner.start()
         try:
             sdata = recv_json(self.main_connection)
         except TimeoutError as err:
             print("Failed to receive game info from server", flush=True)
             raise err
         spinner.succeed()
@@ -360,46 +385,59 @@
 
         # Handle connection errors
         if init_data["type"] == "malformed_creds":
             raise RuntimeError("Credentials were formatted incorrectly")
         if init_data["type"] == "bad_creds":
             raise RuntimeError("server did not accept credentials")
         if init_data["type"] == "bad_client_version":
-            raise RuntimeError("Old client version. Please udpate your client to the latest version available.")
+            raise RuntimeError(
+                "Old client version. Please update your client to the latest version available."
+            )
         if init_data["type"] == "connected_too_many_servers":
-            raise RuntimeError("This user is already connected to the server too many times.")
+            raise RuntimeError(
+                "This user is already connected to the server too many times."
+            )
         if init_data["type"] == "invalid_botname":
-            raise RuntimeError(f"This user does not have a bot with the provided name ({self.botname})")
+            raise RuntimeError(
+                f"This user does not have a bot with the provided name ({self.botname})"
+            )
         if init_data["type"] != "connect_success":
-            raise RuntimeError(f"Something went wrong during login: {init_data['type']}")
+            raise RuntimeError(
+                f"Something went wrong during login: {init_data['type']}"
+            )
 
         # Check if tournament is complete
         if init_data["complete"]:
             self.tournament_completed = True
 
     def next_match(self):
         if self.current_match > 0:
-            spinner = Halo(text='Waiting for next round', text_color='cyan', color='green', spinner='dots')
+            spinner = Halo(
+                text="Waiting for next round",
+                text_color="cyan",
+                color="green",
+                spinner="dots",
+            )
             spinner.start()
 
         # Create tournament server connection if it does not already exist
         if self.main_connection is None:
             try:
                 self._setup_main_connection()
             except Exception as e:
                 raise e
 
         if self.current_match > 0:
             spinner.succeed()
 
         if self.tournament_completed:
-            print(Fore.GREEN + "Bot: {} successfully completed tournament".format(self.botname))
+            print(Fore.GREEN + f"Bot: {self.botname} successfully completed tournament")
         elif self.current_match == 0:
             # Connect to game server
-            print(Fore.GREEN + "Bot: {} successfully connected to Umshini".format(self.botname))
+            print(Fore.GREEN + f"Bot: {self.botname} successfully connected to umshini")
             pass
         print(Style.RESET_ALL)
 
         # Connect to game server
         game_env = self._connect_game_server()
         self.main_connection.close()
         self.main_connection = None
```

### Comparing `umshini-0.0.7/Umshini/utils/compress.py` & `umshini-0.0.8/umshini/utils/compress.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-import json
-import pickle
 import gzip
-from base64 import b64encode, b64decode
+import pickle
+from base64 import b64decode, b64encode
 
 
 def compress(original_data):
     pickled_data = pickle.dumps(original_data)
-    gzipped_data = gzip.compress(pickled_data,compresslevel=1)
+    gzipped_data = gzip.compress(pickled_data, compresslevel=1)
     b64_data = b64encode(gzipped_data)
     return b64_data.decode()
 
 
 def decompress(compressed_data):
     b64_data = bytes(compressed_data, "utf-8")
     gzipped_data = b64decode(b64_data)
```

### Comparing `umshini-0.0.7/Umshini/utils/socket_wrap.py` & `umshini-0.0.8/umshini/utils/socket_wrap.py`

 * *Files identical despite different names*

### Comparing `umshini-0.0.7/umshini.egg-info/PKG-INFO` & `umshini-0.0.8/umshini.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: umshini
-Version: 0.0.7
+Version: 0.0.8
 Summary: Umshini client for playing in MARL tournaments
-Home-page: https://github.com/umshini/umshini
-Author: umshini team
 Author-email: "Jordan K. Terry" <j.k.terry@swarmlabs.com>
 License: This code is copyright Jordan Terry, 2021, and is released under the GNU AGPLv3 license, included below:
         
                             GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -667,22 +665,63 @@
           You should also get your employer (if you work as a programmer) or school,
         if any, to sign a "copyright disclaimer" for the program, if necessary.
         For more information on this, and how to apply and follow the GNU AGPL, see
         <https://www.gnu.org/licenses/>.
         
 Project-URL: Homepage, https://github.com/umshini/umshini
 Keywords: Reinforcement Learning,game,RL,AI,gym
-Classifier: Programming Language :: Python
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6, <3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: <3.10,>=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: classic
+Provides-Extra: llm
+Provides-Extra: all
 License-File: LICENSE
 
-# Colosseum
+# Umshini-Client
 
-To run the Colosseum server for testing, refer to [the server repo](https://github.com/PettingZoo-Team/Colosseum-Server).
+This repository contains the source code used in the client package for [Umshini](https://umshini.ai/). 
 
-To run one or multiple clients you can use the following command:
+For full documentation and usage information, see https://umshini.ai/documentation
 
-```
-python test_tournament_clients user1 user2 ...
-```
+## Installation & Connection
+1. **Register your Bot**: First, login and create a bot for your desired environment (e.g. Connect Four) on the account page. 
+2. **Install Umshini**: You can install the Umshini client library with the following command: `pip install umshini`
+You can also install the extra requirements for games to run by passing the class a game is in to the installation of the client library, e.g. `pip install umshini[classic]` Or `pip install umshini[llm]`
+3. **Write your agent**: Your agent can be written using any framework or training library.
+4. **Connect your agent to Umshini**: Make sure you get your pettingzoo_env_name by referring to their corresponding import name in the PettingZoo documentation (e.g. for Atari Combat: Tank you’ll use combat_tank_v2). Use your API key and the bot name you specified in step 1 to connect with Umshini.
+
+## Example Usage
+
+This is an example of how to use umshini to compete in a Connect Four tournament. 
+
+After bot registration and noting down your API key and bot name, you can follow the following steps:
+### Install Umshini 
+```pip install umshini[classic]```
+### Write your Agent
+
+The code below is an agent that plays Connect Four with random (legal) actions.
+
+```    
+import umshini
+import numpy as np
+
+def my_bot(obs, rew, term, trunc, info):
+    """
+    Return a random legal action.
+    """
+    legal_mask = obs["action_mask"]
+    legal_action = legal_mask.nonzero()[0]
+    action = np.random.choice(legal_actions)
+    return (action, surprise)
+
+# Call 'connect' from the umshini package
+# with your user info and the “connect_four_v3” as the first arg.
+umshini.connect("connect_four_v3", "Bot-Name", "API_Key", my_bot)
+```    
+  
+And that's it! Running this script during a tournament will allow your bot to compete! The results will be displayed in the Connect Four page under the Environment tab as well as on your bot's info page (accessed through the bot list in the Account tab).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

