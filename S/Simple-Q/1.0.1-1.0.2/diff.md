# Comparing `tmp/Simple_Q-1.0.1.tar.gz` & `tmp/Simple_Q-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Simple_Q-1.0.1.tar", last modified: Fri Jul 14 13:00:43 2023, max compression
+gzip compressed data, was "Simple_Q-1.0.2.tar", last modified: Fri Jul 14 13:23:00 2023, max compression
```

## Comparing `Simple_Q-1.0.1.tar` & `Simple_Q-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 13:00:43.340113 Simple_Q-1.0.1/
--rw-rw-rw-   0        0        0     1091 2023-07-14 12:20:54.000000 Simple_Q-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     6561 2023-07-14 13:00:43.339115 Simple_Q-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     8273 2023-07-14 11:23:23.000000 Simple_Q-1.0.1/Qlearning.py
--rw-rw-rw-   0        0        0     4844 2023-07-14 12:58:55.000000 Simple_Q-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 13:00:43.335127 Simple_Q-1.0.1/Simple_Q.egg-info/
--rw-rw-rw-   0        0        0     6561 2023-07-14 13:00:43.000000 Simple_Q-1.0.1/Simple_Q.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2023-07-14 13:00:43.000000 Simple_Q-1.0.1/Simple_Q.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 13:00:43.000000 Simple_Q-1.0.1/Simple_Q.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-14 13:00:43.000000 Simple_Q-1.0.1/Simple_Q.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-14 13:00:43.000000 Simple_Q-1.0.1/Simple_Q.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      674 2023-07-14 12:31:07.000000 Simple_Q-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-14 13:00:43.341111 Simple_Q-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-14 13:23:00.378503 Simple_Q-1.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-07-14 12:20:54.000000 Simple_Q-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     6565 2023-07-14 13:23:00.377506 Simple_Q-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4848 2023-07-14 13:07:47.000000 Simple_Q-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 13:23:00.374514 Simple_Q-1.0.2/Simple_Q.egg-info/
+-rw-rw-rw-   0        0        0     6565 2023-07-14 13:23:00.000000 Simple_Q-1.0.2/Simple_Q.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2023-07-14 13:23:00.000000 Simple_Q-1.0.2/Simple_Q.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 13:23:00.000000 Simple_Q-1.0.2/Simple_Q.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-14 13:23:00.000000 Simple_Q-1.0.2/Simple_Q.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-14 13:23:00.000000 Simple_Q-1.0.2/Simple_Q.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8273 2023-07-14 13:15:54.000000 Simple_Q-1.0.2/Simple_Q.py
+-rw-rw-rw-   0        0        0      674 2023-07-14 13:22:25.000000 Simple_Q-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-14 13:23:00.378503 Simple_Q-1.0.2/setup.cfg
```

### Comparing `Simple_Q-1.0.1/LICENSE` & `Simple_Q-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Simple_Q-1.0.1/PKG-INFO` & `Simple_Q-1.0.2/Simple_Q.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Simple_Q
-Version: 1.0.1
+Name: Simple-Q
+Version: 1.0.2
 Summary: A low learning curve implementation of a Q-Learning algorithm.
 Author-email: Nesta <nesta110402@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -104,15 +104,15 @@
 
 ## License
 
 This project is licensed under the [MIT License](https://github.com/Nesta-gitU/Simple-Q/blob/main/Simple_Q/LICENSE).
 
 ## Acknowledgements
 
-This code is originally based upon the [Q-Learning implementation](https://github.com/PacktPublishing/Advanced-Deep-Learning-with-Keras/blob/master/chapter9-drl/q-learning-9.3.1.py) from the book: Advanced Deep Learning with TensorFlow 2 and Keras by Rowel Atienza. However many changes have been made to the original code, including the addition of the polynomial learning rate decay as well as the ability to work with custom objects for states and actions. 
+This code is originally based upon the [Q-Learning implementation](https://github.com/PacktPublishing/Advanced-Deep-Learning-with-Keras/blob/master/chapter9-drl/q-learning-9.3.1.py) from the book: "*Advanced Deep Learning with TensorFlow 2 and Keras*" by Rowel Atienza. However many changes have been made to the original code, including the addition of the polynomial learning rate decay as well as the ability to work with custom objects for states and actions. 
 
 ## References
 Even-Dar, E., Y. Mansour, and P. Bartlett (2003). Learning rates for q-learning. Journal of machine
 learning Research 5(1).
 
 Watkins, C. J. and P. Dayan (1992, May). Technical note: Q-learning. Machine Learning 8(3),
 279–292
```

### Comparing `Simple_Q-1.0.1/Qlearning.py` & `Simple_Q-1.0.2/Simple_Q.py`

 * *Files identical despite different names*

### Comparing `Simple_Q-1.0.1/README.md` & `Simple_Q-1.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
 ## License
 
 This project is licensed under the [MIT License](https://github.com/Nesta-gitU/Simple-Q/blob/main/Simple_Q/LICENSE).
 
 ## Acknowledgements
 
-This code is originally based upon the [Q-Learning implementation](https://github.com/PacktPublishing/Advanced-Deep-Learning-with-Keras/blob/master/chapter9-drl/q-learning-9.3.1.py) from the book: Advanced Deep Learning with TensorFlow 2 and Keras by Rowel Atienza. However many changes have been made to the original code, including the addition of the polynomial learning rate decay as well as the ability to work with custom objects for states and actions. 
+This code is originally based upon the [Q-Learning implementation](https://github.com/PacktPublishing/Advanced-Deep-Learning-with-Keras/blob/master/chapter9-drl/q-learning-9.3.1.py) from the book: "*Advanced Deep Learning with TensorFlow 2 and Keras*" by Rowel Atienza. However many changes have been made to the original code, including the addition of the polynomial learning rate decay as well as the ability to work with custom objects for states and actions. 
 
 ## References
 Even-Dar, E., Y. Mansour, and P. Bartlett (2003). Learning rates for q-learning. Journal of machine
 learning Research 5(1).
 
 Watkins, C. J. and P. Dayan (1992, May). Technical note: Q-learning. Machine Learning 8(3),
 279–292
```

### Comparing `Simple_Q-1.0.1/Simple_Q.egg-info/PKG-INFO` & `Simple_Q-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Simple-Q
-Version: 1.0.1
+Name: Simple_Q
+Version: 1.0.2
 Summary: A low learning curve implementation of a Q-Learning algorithm.
 Author-email: Nesta <nesta110402@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -104,15 +104,15 @@
 
 ## License
 
 This project is licensed under the [MIT License](https://github.com/Nesta-gitU/Simple-Q/blob/main/Simple_Q/LICENSE).
 
 ## Acknowledgements
 
-This code is originally based upon the [Q-Learning implementation](https://github.com/PacktPublishing/Advanced-Deep-Learning-with-Keras/blob/master/chapter9-drl/q-learning-9.3.1.py) from the book: Advanced Deep Learning with TensorFlow 2 and Keras by Rowel Atienza. However many changes have been made to the original code, including the addition of the polynomial learning rate decay as well as the ability to work with custom objects for states and actions. 
+This code is originally based upon the [Q-Learning implementation](https://github.com/PacktPublishing/Advanced-Deep-Learning-with-Keras/blob/master/chapter9-drl/q-learning-9.3.1.py) from the book: "*Advanced Deep Learning with TensorFlow 2 and Keras*" by Rowel Atienza. However many changes have been made to the original code, including the addition of the polynomial learning rate decay as well as the ability to work with custom objects for states and actions. 
 
 ## References
 Even-Dar, E., Y. Mansour, and P. Bartlett (2003). Learning rates for q-learning. Journal of machine
 learning Research 5(1).
 
 Watkins, C. J. and P. Dayan (1992, May). Technical note: Q-learning. Machine Learning 8(3),
 279–292
```

### Comparing `Simple_Q-1.0.1/pyproject.toml` & `Simple_Q-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Simple_Q"
-version = "1.0.1"
+version = "1.0.2"
 description = "A low learning curve implementation of a Q-Learning algorithm."
 readme = "README.md"
 authors = [{ name = "Nesta", email = "nesta110402@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

