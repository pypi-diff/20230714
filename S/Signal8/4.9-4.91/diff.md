# Comparing `tmp/Signal8-4.9.tar.gz` & `tmp/Signal8-4.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signal8-4.9.tar", last modified: Thu Jul 13 21:23:45 2023, max compression
+gzip compressed data, was "Signal8-4.91.tar", last modified: Fri Jul 14 00:52:05 2023, max compression
```

## Comparing `Signal8-4.9.tar` & `Signal8-4.91.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 21:23:45.087731 Signal8-4.9/
--rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-4.9/LICENSE
--rw-rw-rw-   0        0        0     4768 2023-07-13 21:23:45.082731 Signal8-4.9/PKG-INFO
--rw-rw-rw-   0        0        0     4270 2023-07-01 17:14:19.000000 Signal8-4.9/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 21:23:44.858733 Signal8-4.9/Signal8/
--rw-rw-rw-   0        0        0    12074 2023-07-13 21:21:08.000000 Signal8-4.9/Signal8/Signal8.py
--rw-rw-rw-   0        0        0       24 2023-06-19 21:16:46.000000 Signal8-4.9/Signal8/__init__.py
--rw-rw-rw-   0        0        0      239 2023-07-13 18:08:55.000000 Signal8-4.9/Signal8/main.py
-drwxrwxrwx   0        0        0        0 2023-07-13 21:23:45.059730 Signal8-4.9/Signal8/utils/
--rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-4.9/Signal8/utils/__init__.py
--rw-rw-rw-   0        0        0     5369 2023-07-13 18:05:08.000000 Signal8-4.9/Signal8/utils/core.py
--rw-rw-rw-   0        0        0     2322 2023-06-30 20:05:49.000000 Signal8-4.9/Signal8/utils/problems.py
--rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-4.9/Signal8/utils/scenario.py
--rw-rw-rw-   0        0        0    11960 2023-07-13 18:01:37.000000 Signal8-4.9/Signal8/utils/simple_env.py
--rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-4.9/Signal8/utils/test_dynamic_obs.py
-drwxrwxrwx   0        0        0        0 2023-07-13 21:23:44.967729 Signal8-4.9/Signal8.egg-info/
--rw-rw-rw-   0        0        0     4768 2023-07-13 21:23:43.000000 Signal8-4.9/Signal8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      510 2023-07-13 21:23:43.000000 Signal8-4.9/Signal8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 21:23:43.000000 Signal8-4.9/Signal8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-13 21:23:43.000000 Signal8-4.9/Signal8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 21:23:45.088731 Signal8-4.9/setup.cfg
--rw-rw-rw-   0        0        0      645 2023-07-13 21:22:11.000000 Signal8-4.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 00:52:05.235300 Signal8-4.91/
+-rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-4.91/LICENSE
+-rw-rw-rw-   0        0        0     4769 2023-07-14 00:52:05.219296 Signal8-4.91/PKG-INFO
+-rw-rw-rw-   0        0        0     4270 2023-07-01 17:14:19.000000 Signal8-4.91/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 00:52:05.127297 Signal8-4.91/Signal8/
+-rw-rw-rw-   0        0        0    11981 2023-07-14 00:50:58.000000 Signal8-4.91/Signal8/Signal8.py
+-rw-rw-rw-   0        0        0       24 2023-06-19 21:16:46.000000 Signal8-4.91/Signal8/__init__.py
+-rw-rw-rw-   0        0        0      239 2023-07-13 18:08:55.000000 Signal8-4.91/Signal8/main.py
+drwxrwxrwx   0        0        0        0 2023-07-14 00:52:05.214298 Signal8-4.91/Signal8/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-4.91/Signal8/utils/__init__.py
+-rw-rw-rw-   0        0        0     5369 2023-07-13 18:05:08.000000 Signal8-4.91/Signal8/utils/core.py
+-rw-rw-rw-   0        0        0     2322 2023-06-30 20:05:49.000000 Signal8-4.91/Signal8/utils/problems.py
+-rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-4.91/Signal8/utils/scenario.py
+-rw-rw-rw-   0        0        0    11960 2023-07-13 18:01:37.000000 Signal8-4.91/Signal8/utils/simple_env.py
+-rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-4.91/Signal8/utils/test_dynamic_obs.py
+drwxrwxrwx   0        0        0        0 2023-07-14 00:52:05.175301 Signal8-4.91/Signal8.egg-info/
+-rw-rw-rw-   0        0        0     4769 2023-07-14 00:52:04.000000 Signal8-4.91/Signal8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      510 2023-07-14 00:52:04.000000 Signal8-4.91/Signal8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 00:52:04.000000 Signal8-4.91/Signal8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-14 00:52:04.000000 Signal8-4.91/Signal8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 00:52:05.235300 Signal8-4.91/setup.cfg
+-rw-rw-rw-   0        0        0      646 2023-07-14 00:51:13.000000 Signal8-4.91/setup.py
```

### Comparing `Signal8-4.9/LICENSE` & `Signal8-4.91/LICENSE`

 * *Files identical despite different names*

### Comparing `Signal8-4.9/PKG-INFO` & `Signal8-4.91/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 4.9
+Version: 4.91
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-4.9/README.md` & `Signal8-4.91/README.md`

 * *Files identical despite different names*

### Comparing `Signal8-4.9/Signal8/Signal8.py` & `Signal8-4.91/Signal8/Signal8.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,15 +259,13 @@
             dist = np.linalg.norm(relative_pos)
             if dist <= max_observable_dist:
                 observed_obstacles[i] = relative_pos
                 
         goal_pos = agent.goal.state.p_pos
         relative_goal_pos = goal_pos - agent_pos
         goal_dist = np.linalg.norm(relative_goal_pos)
-        if goal_dist <= max_observable_dist:
-            observed_goal = relative_goal_pos
         
         return np.concatenate((agent_pos, np.concatenate(observed_obstacles, axis=0), observed_goal))
         
     # Reward given by agents to agents for reaching their respective goals
     def reward(self, agent, world):
         return 0
```

### Comparing `Signal8-4.9/Signal8/utils/core.py` & `Signal8-4.91/Signal8/utils/core.py`

 * *Files identical despite different names*

### Comparing `Signal8-4.9/Signal8/utils/problems.py` & `Signal8-4.91/Signal8/utils/problems.py`

 * *Files identical despite different names*

### Comparing `Signal8-4.9/Signal8/utils/simple_env.py` & `Signal8-4.91/Signal8/utils/simple_env.py`

 * *Files identical despite different names*

### Comparing `Signal8-4.9/Signal8/utils/test_dynamic_obs.py` & `Signal8-4.91/Signal8/utils/test_dynamic_obs.py`

 * *Files identical despite different names*

### Comparing `Signal8-4.9/Signal8.egg-info/PKG-INFO` & `Signal8-4.91/Signal8.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 4.9
+Version: 4.91
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-4.9/setup.py` & `Signal8-4.91/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Signal8",
-    version="4.9",
+    version="4.91",
     packages=find_packages(),
     author="Ethan Clark",
     author_email="eclark715@gmail.com.com",
     description="A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/ethanmclark1/signal8",
```

