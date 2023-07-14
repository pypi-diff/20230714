# Comparing `tmp/Signal8-4.91.tar.gz` & `tmp/Signal8-4.915.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signal8-4.91.tar", last modified: Fri Jul 14 00:52:05 2023, max compression
+gzip compressed data, was "Signal8-4.915.tar", last modified: Fri Jul 14 01:02:02 2023, max compression
```

## Comparing `Signal8-4.91.tar` & `Signal8-4.915.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 00:52:05.235300 Signal8-4.91/
--rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-4.91/LICENSE
--rw-rw-rw-   0        0        0     4769 2023-07-14 00:52:05.219296 Signal8-4.91/PKG-INFO
--rw-rw-rw-   0        0        0     4270 2023-07-01 17:14:19.000000 Signal8-4.91/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 00:52:05.127297 Signal8-4.91/Signal8/
--rw-rw-rw-   0        0        0    11981 2023-07-14 00:50:58.000000 Signal8-4.91/Signal8/Signal8.py
--rw-rw-rw-   0        0        0       24 2023-06-19 21:16:46.000000 Signal8-4.91/Signal8/__init__.py
--rw-rw-rw-   0        0        0      239 2023-07-13 18:08:55.000000 Signal8-4.91/Signal8/main.py
-drwxrwxrwx   0        0        0        0 2023-07-14 00:52:05.214298 Signal8-4.91/Signal8/utils/
--rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-4.91/Signal8/utils/__init__.py
--rw-rw-rw-   0        0        0     5369 2023-07-13 18:05:08.000000 Signal8-4.91/Signal8/utils/core.py
--rw-rw-rw-   0        0        0     2322 2023-06-30 20:05:49.000000 Signal8-4.91/Signal8/utils/problems.py
--rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-4.91/Signal8/utils/scenario.py
--rw-rw-rw-   0        0        0    11960 2023-07-13 18:01:37.000000 Signal8-4.91/Signal8/utils/simple_env.py
--rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-4.91/Signal8/utils/test_dynamic_obs.py
-drwxrwxrwx   0        0        0        0 2023-07-14 00:52:05.175301 Signal8-4.91/Signal8.egg-info/
--rw-rw-rw-   0        0        0     4769 2023-07-14 00:52:04.000000 Signal8-4.91/Signal8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      510 2023-07-14 00:52:04.000000 Signal8-4.91/Signal8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 00:52:04.000000 Signal8-4.91/Signal8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-14 00:52:04.000000 Signal8-4.91/Signal8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 00:52:05.235300 Signal8-4.91/setup.cfg
--rw-rw-rw-   0        0        0      646 2023-07-14 00:51:13.000000 Signal8-4.91/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 01:02:02.845108 Signal8-4.915/
+-rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-4.915/LICENSE
+-rw-rw-rw-   0        0        0     4770 2023-07-14 01:02:02.841109 Signal8-4.915/PKG-INFO
+-rw-rw-rw-   0        0        0     4270 2023-07-01 17:14:19.000000 Signal8-4.915/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 01:02:02.749107 Signal8-4.915/Signal8/
+-rw-rw-rw-   0        0        0    11550 2023-07-14 01:00:30.000000 Signal8-4.915/Signal8/Signal8.py
+-rw-rw-rw-   0        0        0       24 2023-06-19 21:16:46.000000 Signal8-4.915/Signal8/__init__.py
+-rw-rw-rw-   0        0        0      239 2023-07-13 18:08:55.000000 Signal8-4.915/Signal8/main.py
+drwxrwxrwx   0        0        0        0 2023-07-14 01:02:02.832108 Signal8-4.915/Signal8/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-4.915/Signal8/utils/__init__.py
+-rw-rw-rw-   0        0        0     5285 2023-07-14 01:01:24.000000 Signal8-4.915/Signal8/utils/core.py
+-rw-rw-rw-   0        0        0     2322 2023-06-30 20:05:49.000000 Signal8-4.915/Signal8/utils/problems.py
+-rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-4.915/Signal8/utils/scenario.py
+-rw-rw-rw-   0        0        0    11960 2023-07-13 18:01:37.000000 Signal8-4.915/Signal8/utils/simple_env.py
+-rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-4.915/Signal8/utils/test_dynamic_obs.py
+drwxrwxrwx   0        0        0        0 2023-07-14 01:02:02.795107 Signal8-4.915/Signal8.egg-info/
+-rw-rw-rw-   0        0        0     4770 2023-07-14 01:02:02.000000 Signal8-4.915/Signal8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      510 2023-07-14 01:02:02.000000 Signal8-4.915/Signal8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 01:02:02.000000 Signal8-4.915/Signal8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-14 01:02:02.000000 Signal8-4.915/Signal8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 01:02:02.846107 Signal8-4.915/setup.cfg
+-rw-rw-rw-   0        0        0      647 2023-07-14 01:01:03.000000 Signal8-4.915/setup.py
```

### Comparing `Signal8-4.91/LICENSE` & `Signal8-4.915/LICENSE`

 * *Files identical despite different names*

### Comparing `Signal8-4.91/PKG-INFO` & `Signal8-4.915/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 4.91
+Version: 4.915
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-4.91/README.md` & `Signal8-4.915/README.md`

 * *Files identical despite different names*

### Comparing `Signal8-4.91/Signal8/Signal8.py` & `Signal8-4.915/Signal8/Signal8.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
         num_agents=1, 
         num_large_obstacles=4, 
         num_small_obstacles=10, 
         render_mode=None,
         max_cycles=500,
         ):
         
-        if num_agents > 2:
-            raise ValueError("Signal8 currently can only support up to 2 agents.")
+        if num_agents > 1:
+            raise ValueError("Signal8 currently can only support up to 1 agent.")
         
         if num_large_obstacles > 16:
             raise ValueError("Signal8 has a maximum of 10 large obstacles.")
         
         scenario = Scenario()
         world = scenario.make_world(num_agents, num_large_obstacles, num_small_obstacles)
         
@@ -231,41 +231,34 @@
     
     # Ground agents can only observe the positions of other agents, goals, and small obstacles
     def observation(self, agent, world):
         agent_pos = agent.state.p_pos
         
         num_agents = len(world.agents)
         num_small_obstacles = len(world.small_obstacles)
-        max_observable_dist = agent.max_observable_dist
         
-        observed_agents = [np.full_like(agent_pos, max_observable_dist) for _ in range(num_agents - 1)]
-        observed_goal = np.full_like(agent_pos, max_observable_dist)
-        observed_obstacles = [np.full_like(agent_pos, max_observable_dist) for _ in range(num_small_obstacles)]
+        observed_agents = [np.zeros_like(agent_pos) for _ in range(num_agents - 1)]
+        observed_obstacles = [np.zeros_like(agent_pos) for _ in range(num_small_obstacles)]
         
         idx = 0
         for other_agent in world.agents:
             if agent.name == other_agent.name:
                 continue
             else:
                 other_agent_pos = other_agent.state.p_pos
                 relative_pos = other_agent_pos - agent_pos
-                dist = np.linalg.norm(relative_pos)
-                if dist <= max_observable_dist:
-                    observed_agents[idx] = relative_pos
+                observed_agents[idx] = relative_pos
                 idx += 1
         
         for i, small_obstacle in enumerate(world.small_obstacles):
             obs_pos = small_obstacle.state.p_pos
             relative_pos = obs_pos - agent_pos
-            dist = np.linalg.norm(relative_pos)
-            if dist <= max_observable_dist:
-                observed_obstacles[i] = relative_pos
+            observed_obstacles[i] = relative_pos
                 
         goal_pos = agent.goal.state.p_pos
-        relative_goal_pos = goal_pos - agent_pos
-        goal_dist = np.linalg.norm(relative_goal_pos)
+        observed_goal = goal_pos - agent_pos
         
-        return np.concatenate((agent_pos, np.concatenate(observed_obstacles, axis=0), observed_goal))
+        return np.concatenate((agent_pos, observed_goal, np.concatenate(observed_obstacles, axis=0)))
         
     # Reward given by agents to agents for reaching their respective goals
     def reward(self, agent, world):
         return 0
```

### Comparing `Signal8-4.91/Signal8/utils/core.py` & `Signal8-4.915/Signal8/utils/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,16 +57,15 @@
         self.movable = True
         # goal entity
         self.goal = None
         # state
         self.state = AgentState()
         # action
         self.action = None
-        # how far the agent can sense around itself
-        self.max_observable_dist = 0.30
+        
 
 class World:  # multi-agent world
     def __init__(self):
         # list of agents and entities (can change at execution-time!)
         self.agents = []
         self.goals = []
         self.small_obstacles = []
```

### Comparing `Signal8-4.91/Signal8/utils/problems.py` & `Signal8-4.915/Signal8/utils/problems.py`

 * *Files identical despite different names*

### Comparing `Signal8-4.91/Signal8/utils/simple_env.py` & `Signal8-4.915/Signal8/utils/simple_env.py`

 * *Files identical despite different names*

### Comparing `Signal8-4.91/Signal8/utils/test_dynamic_obs.py` & `Signal8-4.915/Signal8/utils/test_dynamic_obs.py`

 * *Files identical despite different names*

### Comparing `Signal8-4.91/Signal8.egg-info/PKG-INFO` & `Signal8-4.915/Signal8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 4.91
+Version: 4.915
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-4.91/setup.py` & `Signal8-4.915/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Signal8",
-    version="4.91",
+    version="4.915",
     packages=find_packages(),
     author="Ethan Clark",
     author_email="eclark715@gmail.com.com",
     description="A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/ethanmclark1/signal8",
```

