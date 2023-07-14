# Comparing `tmp/Simple_Q-1.0.2.tar.gz` & `tmp/Simple_Q-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Simple_Q-1.0.2.tar", last modified: Fri Jul 14 13:23:00 2023, max compression
+gzip compressed data, was "Simple_Q-1.0.3.tar", last modified: Fri Jul 14 13:26:07 2023, max compression
```

## Comparing `Simple_Q-1.0.2.tar` & `Simple_Q-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 13:23:00.378503 Simple_Q-1.0.2/
--rw-rw-rw-   0        0        0     1091 2023-07-14 12:20:54.000000 Simple_Q-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     6565 2023-07-14 13:23:00.377506 Simple_Q-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4848 2023-07-14 13:07:47.000000 Simple_Q-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 13:23:00.374514 Simple_Q-1.0.2/Simple_Q.egg-info/
--rw-rw-rw-   0        0        0     6565 2023-07-14 13:23:00.000000 Simple_Q-1.0.2/Simple_Q.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-07-14 13:23:00.000000 Simple_Q-1.0.2/Simple_Q.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 13:23:00.000000 Simple_Q-1.0.2/Simple_Q.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-14 13:23:00.000000 Simple_Q-1.0.2/Simple_Q.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-14 13:23:00.000000 Simple_Q-1.0.2/Simple_Q.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8273 2023-07-14 13:15:54.000000 Simple_Q-1.0.2/Simple_Q.py
--rw-rw-rw-   0        0        0      674 2023-07-14 13:22:25.000000 Simple_Q-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-14 13:23:00.378503 Simple_Q-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-14 13:26:07.329588 Simple_Q-1.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-07-14 12:20:54.000000 Simple_Q-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     6565 2023-07-14 13:26:07.327593 Simple_Q-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4848 2023-07-14 13:25:27.000000 Simple_Q-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 13:26:07.323603 Simple_Q-1.0.3/Simple_Q.egg-info/
+-rw-rw-rw-   0        0        0     6565 2023-07-14 13:26:07.000000 Simple_Q-1.0.3/Simple_Q.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2023-07-14 13:26:07.000000 Simple_Q-1.0.3/Simple_Q.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 13:26:07.000000 Simple_Q-1.0.3/Simple_Q.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-14 13:26:07.000000 Simple_Q-1.0.3/Simple_Q.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-14 13:26:07.000000 Simple_Q-1.0.3/Simple_Q.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8273 2023-07-14 13:15:54.000000 Simple_Q-1.0.3/Simple_Q.py
+-rw-rw-rw-   0        0        0      674 2023-07-14 13:25:42.000000 Simple_Q-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-14 13:26:07.329588 Simple_Q-1.0.3/setup.cfg
```

### Comparing `Simple_Q-1.0.2/LICENSE` & `Simple_Q-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Simple_Q-1.0.2/PKG-INFO` & `Simple_Q-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simple_Q
-Version: 1.0.2
+Version: 1.0.3
 Summary: A low learning curve implementation of a Q-Learning algorithm.
 Author-email: Nesta <nesta110402@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -54,15 +54,15 @@
 ```shell
 pip install Simple-Q
 ```
 
 ## Usage
 
 ```python
-from Simple-Q import Qlearning
+from Simple_Q import Qlearning
 
 # Create the Q-learning agent
 agent = Qlearning(states=10, actions = ['forward', 'left', 'right' 'stop'])
 
 # Use the Q-learning agent in your reinforcement learning loop
 state = env.reset()
 N = 100
```

### Comparing `Simple_Q-1.0.2/README.md` & `Simple_Q-1.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 ```shell
 pip install Simple-Q
 ```
 
 ## Usage
 
 ```python
-from Simple-Q import Qlearning
+from Simple_Q import Qlearning
 
 # Create the Q-learning agent
 agent = Qlearning(states=10, actions = ['forward', 'left', 'right' 'stop'])
 
 # Use the Q-learning agent in your reinforcement learning loop
 state = env.reset()
 N = 100
```

### Comparing `Simple_Q-1.0.2/Simple_Q.egg-info/PKG-INFO` & `Simple_Q-1.0.3/Simple_Q.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simple-Q
-Version: 1.0.2
+Version: 1.0.3
 Summary: A low learning curve implementation of a Q-Learning algorithm.
 Author-email: Nesta <nesta110402@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -54,15 +54,15 @@
 ```shell
 pip install Simple-Q
 ```
 
 ## Usage
 
 ```python
-from Simple-Q import Qlearning
+from Simple_Q import Qlearning
 
 # Create the Q-learning agent
 agent = Qlearning(states=10, actions = ['forward', 'left', 'right' 'stop'])
 
 # Use the Q-learning agent in your reinforcement learning loop
 state = env.reset()
 N = 100
```

### Comparing `Simple_Q-1.0.2/Simple_Q.py` & `Simple_Q-1.0.3/Simple_Q.py`

 * *Files identical despite different names*

### Comparing `Simple_Q-1.0.2/pyproject.toml` & `Simple_Q-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Simple_Q"
-version = "1.0.2"
+version = "1.0.3"
 description = "A low learning curve implementation of a Q-Learning algorithm."
 readme = "README.md"
 authors = [{ name = "Nesta", email = "nesta110402@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

