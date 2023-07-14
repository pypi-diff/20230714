# Comparing `tmp/Simple_Q-1.0.0.tar.gz` & `tmp/Simple_Q-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Simple_Q-1.0.0.tar", last modified: Fri Jul 14 12:28:33 2023, max compression
+gzip compressed data, was "Simple_Q-1.0.1.tar", last modified: Fri Jul 14 13:00:43 2023, max compression
```

## Comparing `Simple_Q-1.0.0.tar` & `Simple_Q-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 12:28:33.131217 Simple_Q-1.0.0/
--rw-rw-rw-   0        0        0     1091 2023-07-14 12:20:54.000000 Simple_Q-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     6148 2023-07-14 12:28:33.130221 Simple_Q-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     8273 2023-07-14 11:23:23.000000 Simple_Q-1.0.0/Qlearning.py
--rw-rw-rw-   0        0        0     4429 2023-07-14 12:27:18.000000 Simple_Q-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 12:28:33.127229 Simple_Q-1.0.0/Simple_Q.egg-info/
--rw-rw-rw-   0        0        0     6148 2023-07-14 12:28:33.000000 Simple_Q-1.0.0/Simple_Q.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2023-07-14 12:28:33.000000 Simple_Q-1.0.0/Simple_Q.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 12:28:33.000000 Simple_Q-1.0.0/Simple_Q.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-14 12:28:33.000000 Simple_Q-1.0.0/Simple_Q.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-14 12:28:33.000000 Simple_Q-1.0.0/Simple_Q.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      674 2023-07-14 11:43:56.000000 Simple_Q-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-14 12:28:33.131217 Simple_Q-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-14 13:00:43.340113 Simple_Q-1.0.1/
+-rw-rw-rw-   0        0        0     1091 2023-07-14 12:20:54.000000 Simple_Q-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     6561 2023-07-14 13:00:43.339115 Simple_Q-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8273 2023-07-14 11:23:23.000000 Simple_Q-1.0.1/Qlearning.py
+-rw-rw-rw-   0        0        0     4844 2023-07-14 12:58:55.000000 Simple_Q-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 13:00:43.335127 Simple_Q-1.0.1/Simple_Q.egg-info/
+-rw-rw-rw-   0        0        0     6561 2023-07-14 13:00:43.000000 Simple_Q-1.0.1/Simple_Q.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2023-07-14 13:00:43.000000 Simple_Q-1.0.1/Simple_Q.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 13:00:43.000000 Simple_Q-1.0.1/Simple_Q.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-14 13:00:43.000000 Simple_Q-1.0.1/Simple_Q.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-14 13:00:43.000000 Simple_Q-1.0.1/Simple_Q.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      674 2023-07-14 12:31:07.000000 Simple_Q-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-14 13:00:43.341111 Simple_Q-1.0.1/setup.cfg
```

### Comparing `Simple_Q-1.0.0/LICENSE` & `Simple_Q-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Simple_Q-1.0.0/PKG-INFO` & `Simple_Q-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simple_Q
-Version: 1.0.0
+Version: 1.0.1
 Summary: A low learning curve implementation of a Q-Learning algorithm.
 Author-email: Nesta <nesta110402@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -26,23 +26,22 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-```
 # Q-Learning
 
 A low learning curve implementation of Q-learning.
 
 [![PyPI](https://img.shields.io/pypi/v/qlearning)](https://pypi.org/project/Simple-Q/)
-[![License](https://img.shields.io/pypi/l/qlearning)](https://github.com/Nesta-gitU/Simple-Q/Simple-Q/LICENSE).
+[![License](https://img.shields.io/pypi/l/qlearning)](https://github.com/Nesta-gitU/Simple-Q/blob/main/Simple_Q/LICENSE).
 
-Q-learning is a reinforcement learning algorithm that allows an agent to learn an optimal policy for sequential decision-making problems. This implementation provides an easy-to-use and beginner-friendly approach to Q-learning, making it accessible to users with varying levels of experience. This implementation is build to work with "GYM" environments from the [Gymnasium Project](https://gymnasium.farama.org/) 
+Q-learning is a reinforcement learning algorithm that allows an agent to learn an optimal policy for sequential decision-making problems. This implementation provides an easy-to-use and beginner-friendly approach to Q-learning, making it accessible to users with varying levels of experience. This implementation is build to work with "GYM" environments from the [Gymnasium Project](https://gymnasium.farama.org/).
 
 ## Features
 
 - Provides flexibility to work with either integer or custom objects for states and actions.
 - Offers customizable learning rate and exploration-exploitation trade-off parameters.
 - Implements epsilon-greedy strategy for action selection.
 - Supports polynomial and power decay functions for learning rate and exploration parameter respecitively. 
@@ -71,15 +70,15 @@
     action = agent.get_action(state)
     next_state, reward, done, _ = env.step(action)
     agent.update_q_table(state, action, reward, next_state)
     state = next_state
     agent.update_epsilon()
 ```
 
-See also the [Savings Problem](https://github.com/Nesta-gitU/Simple-Q/SavingsProblem) example in the GitHub repository.
+See also the [Savings Problem](https://github.com/Nesta-gitU/Simple-Q/tree/main/SavingsProblem) example in the GitHub repository.
 
 ## Documentation
 
 The Q-Learning class provides the following parameters:
 
 | Parameter             | Description                                                  |
 |-----------------------|--------------------------------------------------------------|
@@ -101,20 +100,19 @@
 
 ## Contributing
 
 Contributions are welcome! If you find any issues or have suggestions for improvement, please feel free to open an issue or submit a pull request.
 
 ## License
 
-This project is licensed under the [MIT License](https://github.com/Nesta-gitU/Simple-Q/Simple-Q/LICENSE).
+This project is licensed under the [MIT License](https://github.com/Nesta-gitU/Simple-Q/blob/main/Simple_Q/LICENSE).
 
 ## Acknowledgements
 
-This code is originally based upon the [Q-Learning implementation](
+This code is originally based upon the [Q-Learning implementation](https://github.com/PacktPublishing/Advanced-Deep-Learning-with-Keras/blob/master/chapter9-drl/q-learning-9.3.1.py) from the book: Advanced Deep Learning with TensorFlow 2 and Keras by Rowel Atienza. However many changes have been made to the original code, including the addition of the polynomial learning rate decay as well as the ability to work with custom objects for states and actions. 
 
 ## References
 Even-Dar, E., Y. Mansour, and P. Bartlett (2003). Learning rates for q-learning. Journal of machine
 learning Research 5(1).
 
 Watkins, C. J. and P. Dayan (1992, May). Technical note: Q-learning. Machine Learning 8(3),
 279–292
-```
```

### Comparing `Simple_Q-1.0.0/Qlearning.py` & `Simple_Q-1.0.1/Qlearning.py`

 * *Files identical despite different names*

### Comparing `Simple_Q-1.0.0/README.md` & `Simple_Q-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,277 +1,303 @@
-00000000: 6060 600d 0a23 2051 2d4c 6561 726e 696e  ```..# Q-Learnin
-00000010: 670d 0a0d 0a41 206c 6f77 206c 6561 726e  g....A low learn
-00000020: 696e 6720 6375 7276 6520 696d 706c 656d  ing curve implem
-00000030: 656e 7461 7469 6f6e 206f 6620 512d 6c65  entation of Q-le
-00000040: 6172 6e69 6e67 2e0d 0a0d 0a5b 215b 5079  arning.....[![Py
-00000050: 5049 5d28 6874 7470 733a 2f2f 696d 672e  PI](https://img.
-00000060: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
-00000070: 762f 716c 6561 726e 696e 6729 5d28 6874  v/qlearning)](ht
-00000080: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
-00000090: 726f 6a65 6374 2f53 696d 706c 652d 512f  roject/Simple-Q/
-000000a0: 290d 0a5b 215b 4c69 6365 6e73 655d 2868  )..[![License](h
-000000b0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-000000c0: 6473 2e69 6f2f 7079 7069 2f6c 2f71 6c65  ds.io/pypi/l/qle
-000000d0: 6172 6e69 6e67 295d 2868 7474 7073 3a2f  arning)](https:/
-000000e0: 2f67 6974 6875 622e 636f 6d2f 4e65 7374  /github.com/Nest
-000000f0: 612d 6769 7455 2f53 696d 706c 652d 512f  a-gitU/Simple-Q/
-00000100: 5369 6d70 6c65 2d51 2f4c 4943 454e 5345  Simple-Q/LICENSE
-00000110: 292e 0d0a 0d0a 512d 6c65 6172 6e69 6e67  ).....Q-learning
-00000120: 2069 7320 6120 7265 696e 666f 7263 656d   is a reinforcem
-00000130: 656e 7420 6c65 6172 6e69 6e67 2061 6c67  ent learning alg
-00000140: 6f72 6974 686d 2074 6861 7420 616c 6c6f  orithm that allo
-00000150: 7773 2061 6e20 6167 656e 7420 746f 206c  ws an agent to l
-00000160: 6561 726e 2061 6e20 6f70 7469 6d61 6c20  earn an optimal 
-00000170: 706f 6c69 6379 2066 6f72 2073 6571 7565  policy for seque
-00000180: 6e74 6961 6c20 6465 6369 7369 6f6e 2d6d  ntial decision-m
-00000190: 616b 696e 6720 7072 6f62 6c65 6d73 2e20  aking problems. 
-000001a0: 5468 6973 2069 6d70 6c65 6d65 6e74 6174  This implementat
-000001b0: 696f 6e20 7072 6f76 6964 6573 2061 6e20  ion provides an 
-000001c0: 6561 7379 2d74 6f2d 7573 6520 616e 6420  easy-to-use and 
-000001d0: 6265 6769 6e6e 6572 2d66 7269 656e 646c  beginner-friendl
-000001e0: 7920 6170 7072 6f61 6368 2074 6f20 512d  y approach to Q-
-000001f0: 6c65 6172 6e69 6e67 2c20 6d61 6b69 6e67  learning, making
-00000200: 2069 7420 6163 6365 7373 6962 6c65 2074   it accessible t
-00000210: 6f20 7573 6572 7320 7769 7468 2076 6172  o users with var
-00000220: 7969 6e67 206c 6576 656c 7320 6f66 2065  ying levels of e
-00000230: 7870 6572 6965 6e63 652e 2054 6869 7320  xperience. This 
-00000240: 696d 706c 656d 656e 7461 7469 6f6e 2069  implementation i
-00000250: 7320 6275 696c 6420 746f 2077 6f72 6b20  s build to work 
-00000260: 7769 7468 2022 4759 4d22 2065 6e76 6972  with "GYM" envir
-00000270: 6f6e 6d65 6e74 7320 6672 6f6d 2074 6865  onments from the
-00000280: 205b 4779 6d6e 6173 6975 6d20 5072 6f6a   [Gymnasium Proj
-00000290: 6563 745d 2868 7474 7073 3a2f 2f67 796d  ect](https://gym
-000002a0: 6e61 7369 756d 2e66 6172 616d 612e 6f72  nasium.farama.or
-000002b0: 672f 2920 0d0a 0d0a 2323 2046 6561 7475  g/) ....## Featu
-000002c0: 7265 730d 0a0d 0a2d 2050 726f 7669 6465  res....- Provide
-000002d0: 7320 666c 6578 6962 696c 6974 7920 746f  s flexibility to
-000002e0: 2077 6f72 6b20 7769 7468 2065 6974 6865   work with eithe
-000002f0: 7220 696e 7465 6765 7220 6f72 2063 7573  r integer or cus
-00000300: 746f 6d20 6f62 6a65 6374 7320 666f 7220  tom objects for 
-00000310: 7374 6174 6573 2061 6e64 2061 6374 696f  states and actio
-00000320: 6e73 2e0d 0a2d 204f 6666 6572 7320 6375  ns...- Offers cu
-00000330: 7374 6f6d 697a 6162 6c65 206c 6561 726e  stomizable learn
-00000340: 696e 6720 7261 7465 2061 6e64 2065 7870  ing rate and exp
-00000350: 6c6f 7261 7469 6f6e 2d65 7870 6c6f 6974  loration-exploit
-00000360: 6174 696f 6e20 7472 6164 652d 6f66 6620  ation trade-off 
-00000370: 7061 7261 6d65 7465 7273 2e0d 0a2d 2049  parameters...- I
-00000380: 6d70 6c65 6d65 6e74 7320 6570 7369 6c6f  mplements epsilo
-00000390: 6e2d 6772 6565 6479 2073 7472 6174 6567  n-greedy strateg
-000003a0: 7920 666f 7220 6163 7469 6f6e 2073 656c  y for action sel
-000003b0: 6563 7469 6f6e 2e0d 0a2d 2053 7570 706f  ection...- Suppo
-000003c0: 7274 7320 706f 6c79 6e6f 6d69 616c 2061  rts polynomial a
-000003d0: 6e64 2070 6f77 6572 2064 6563 6179 2066  nd power decay f
-000003e0: 756e 6374 696f 6e73 2066 6f72 206c 6561  unctions for lea
-000003f0: 726e 696e 6720 7261 7465 2061 6e64 2065  rning rate and e
-00000400: 7870 6c6f 7261 7469 6f6e 2070 6172 616d  xploration param
-00000410: 6574 6572 2072 6573 7065 6369 7469 7665  eter respecitive
-00000420: 6c79 2e20 0d0a 2020 5468 6520 6c65 6172  ly. ..  The lear
-00000430: 6e69 6e67 2072 6174 6520 6465 6361 7920  ning rate decay 
-00000440: 6973 2062 6173 6564 206f 6e20 7468 6520  is based on the 
-00000450: 7265 7365 6172 6368 2069 6e20 4576 656e  research in Even
-00000460: 2d44 6172 2065 7420 616c 2e20 2832 3030  -Dar et al. (200
-00000470: 3329 2e20 5768 656e 206c 616d 6264 6120  3). When lambda 
-00000480: 6973 2069 6e20 2830 2c31 2920 7468 6973  is in (0,1) this
-00000490: 2069 6d70 6c65 6d65 6e74 6174 696f 6e20   implementation 
-000004a0: 6f66 2051 2d6c 6561 726e 696e 6720 7361  of Q-learning sa
-000004b0: 7469 7366 6965 7320 7468 6520 636f 6e64  tisfies the cond
-000004c0: 6974 696f 6e73 2066 6f72 2070 726f 6261  itions for proba
-000004d0: 6269 6c69 7479 206f 6e65 2063 6f6e 7665  bility one conve
-000004e0: 7267 656e 6365 2069 6e20 5761 746b 696e  rgence in Watkin
-000004f0: 7320 616e 6420 4461 7961 6e20 2831 3939  s and Dayan (199
-00000500: 3229 2e0d 0a0d 0a23 2320 496e 7374 616c  2).....## Instal
-00000510: 6c61 7469 6f6e 0d0a 0d0a 496e 7374 616c  lation....Instal
-00000520: 6c20 7468 6520 6053 696d 706c 652d 5160  l the `Simple-Q`
-00000530: 2070 6163 6b61 6765 2066 726f 6d20 5079   package from Py
-00000540: 5049 3a0d 0a0d 0a60 6060 7368 656c 6c0d  PI:....```shell.
-00000550: 0a70 6970 2069 6e73 7461 6c6c 2053 696d  .pip install Sim
-00000560: 706c 652d 510d 0a60 6060 0d0a 0d0a 2323  ple-Q..```....##
-00000570: 2055 7361 6765 0d0a 0d0a 6060 6070 7974   Usage....```pyt
-00000580: 686f 6e0d 0a66 726f 6d20 5369 6d70 6c65  hon..from Simple
-00000590: 2d51 2069 6d70 6f72 7420 516c 6561 726e  -Q import Qlearn
-000005a0: 696e 670d 0a0d 0a23 2043 7265 6174 6520  ing....# Create 
-000005b0: 7468 6520 512d 6c65 6172 6e69 6e67 2061  the Q-learning a
-000005c0: 6765 6e74 0d0a 6167 656e 7420 3d20 516c  gent..agent = Ql
-000005d0: 6561 726e 696e 6728 7374 6174 6573 3d31  earning(states=1
-000005e0: 302c 2061 6374 696f 6e73 203d 205b 2766  0, actions = ['f
-000005f0: 6f72 7761 7264 272c 2027 6c65 6674 272c  orward', 'left',
-00000600: 2027 7269 6768 7427 2027 7374 6f70 275d   'right' 'stop']
-00000610: 290d 0a0d 0a23 2055 7365 2074 6865 2051  )....# Use the Q
-00000620: 2d6c 6561 726e 696e 6720 6167 656e 7420  -learning agent 
-00000630: 696e 2079 6f75 7220 7265 696e 666f 7263  in your reinforc
-00000640: 656d 656e 7420 6c65 6172 6e69 6e67 206c  ement learning l
-00000650: 6f6f 700d 0a73 7461 7465 203d 2065 6e76  oop..state = env
-00000660: 2e72 6573 6574 2829 0d0a 4e20 3d20 3130  .reset()..N = 10
-00000670: 300d 0a66 6f72 206e 2069 6e20 7261 6e67  0..for n in rang
-00000680: 6528 4e29 3a0d 0a20 2020 2061 6374 696f  e(N):..    actio
-00000690: 6e20 3d20 6167 656e 742e 6765 745f 6163  n = agent.get_ac
-000006a0: 7469 6f6e 2873 7461 7465 290d 0a20 2020  tion(state)..   
-000006b0: 206e 6578 745f 7374 6174 652c 2072 6577   next_state, rew
-000006c0: 6172 642c 2064 6f6e 652c 205f 203d 2065  ard, done, _ = e
-000006d0: 6e76 2e73 7465 7028 6163 7469 6f6e 290d  nv.step(action).
-000006e0: 0a20 2020 2061 6765 6e74 2e75 7064 6174  .    agent.updat
-000006f0: 655f 715f 7461 626c 6528 7374 6174 652c  e_q_table(state,
-00000700: 2061 6374 696f 6e2c 2072 6577 6172 642c   action, reward,
-00000710: 206e 6578 745f 7374 6174 6529 0d0a 2020   next_state)..  
-00000720: 2020 7374 6174 6520 3d20 6e65 7874 5f73    state = next_s
-00000730: 7461 7465 0d0a 2020 2020 6167 656e 742e  tate..    agent.
-00000740: 7570 6461 7465 5f65 7073 696c 6f6e 2829  update_epsilon()
-00000750: 0d0a 6060 600d 0a0d 0a53 6565 2061 6c73  ..```....See als
-00000760: 6f20 7468 6520 5b53 6176 696e 6773 2050  o the [Savings P
-00000770: 726f 626c 656d 5d28 6874 7470 733a 2f2f  roblem](https://
-00000780: 6769 7468 7562 2e63 6f6d 2f4e 6573 7461  github.com/Nesta
-00000790: 2d67 6974 552f 5369 6d70 6c65 2d51 2f53  -gitU/Simple-Q/S
-000007a0: 6176 696e 6773 5072 6f62 6c65 6d29 2065  avingsProblem) e
-000007b0: 7861 6d70 6c65 2069 6e20 7468 6520 4769  xample in the Gi
-000007c0: 7448 7562 2072 6570 6f73 6974 6f72 792e  tHub repository.
-000007d0: 0d0a 0d0a 2323 2044 6f63 756d 656e 7461  ....## Documenta
-000007e0: 7469 6f6e 0d0a 0d0a 5468 6520 512d 4c65  tion....The Q-Le
-000007f0: 6172 6e69 6e67 2063 6c61 7373 2070 726f  arning class pro
-00000800: 7669 6465 7320 7468 6520 666f 6c6c 6f77  vides the follow
-00000810: 696e 6720 7061 7261 6d65 7465 7273 3a0d  ing parameters:.
-00000820: 0a0d 0a7c 2050 6172 616d 6574 6572 2020  ...| Parameter  
-00000830: 2020 2020 2020 2020 2020 207c 2044 6573             | Des
-00000840: 6372 6970 7469 6f6e 2020 2020 2020 2020  cription        
-00000850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000000: 2320 512d 4c65 6172 6e69 6e67 0d0a 0d0a  # Q-Learning....
+00000010: 4120 6c6f 7720 6c65 6172 6e69 6e67 2063  A low learning c
+00000020: 7572 7665 2069 6d70 6c65 6d65 6e74 6174  urve implementat
+00000030: 696f 6e20 6f66 2051 2d6c 6561 726e 696e  ion of Q-learnin
+00000040: 672e 0d0a 0d0a 5b21 5b50 7950 495d 2868  g.....[![PyPI](h
+00000050: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000060: 6473 2e69 6f2f 7079 7069 2f76 2f71 6c65  ds.io/pypi/v/qle
+00000070: 6172 6e69 6e67 295d 2868 7474 7073 3a2f  arning)](https:/
+00000080: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
+00000090: 742f 5369 6d70 6c65 2d51 2f29 0d0a 5b21  t/Simple-Q/)..[!
+000000a0: 5b4c 6963 656e 7365 5d28 6874 7470 733a  [License](https:
+000000b0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000000c0: 2f70 7970 692f 6c2f 716c 6561 726e 696e  /pypi/l/qlearnin
+000000d0: 6729 5d28 6874 7470 733a 2f2f 6769 7468  g)](https://gith
+000000e0: 7562 2e63 6f6d 2f4e 6573 7461 2d67 6974  ub.com/Nesta-git
+000000f0: 552f 5369 6d70 6c65 2d51 2f62 6c6f 622f  U/Simple-Q/blob/
+00000100: 6d61 696e 2f53 696d 706c 655f 512f 4c49  main/Simple_Q/LI
+00000110: 4345 4e53 4529 2e0d 0a0d 0a51 2d6c 6561  CENSE).....Q-lea
+00000120: 726e 696e 6720 6973 2061 2072 6569 6e66  rning is a reinf
+00000130: 6f72 6365 6d65 6e74 206c 6561 726e 696e  orcement learnin
+00000140: 6720 616c 676f 7269 7468 6d20 7468 6174  g algorithm that
+00000150: 2061 6c6c 6f77 7320 616e 2061 6765 6e74   allows an agent
+00000160: 2074 6f20 6c65 6172 6e20 616e 206f 7074   to learn an opt
+00000170: 696d 616c 2070 6f6c 6963 7920 666f 7220  imal policy for 
+00000180: 7365 7175 656e 7469 616c 2064 6563 6973  sequential decis
+00000190: 696f 6e2d 6d61 6b69 6e67 2070 726f 626c  ion-making probl
+000001a0: 656d 732e 2054 6869 7320 696d 706c 656d  ems. This implem
+000001b0: 656e 7461 7469 6f6e 2070 726f 7669 6465  entation provide
+000001c0: 7320 616e 2065 6173 792d 746f 2d75 7365  s an easy-to-use
+000001d0: 2061 6e64 2062 6567 696e 6e65 722d 6672   and beginner-fr
+000001e0: 6965 6e64 6c79 2061 7070 726f 6163 6820  iendly approach 
+000001f0: 746f 2051 2d6c 6561 726e 696e 672c 206d  to Q-learning, m
+00000200: 616b 696e 6720 6974 2061 6363 6573 7369  aking it accessi
+00000210: 626c 6520 746f 2075 7365 7273 2077 6974  ble to users wit
+00000220: 6820 7661 7279 696e 6720 6c65 7665 6c73  h varying levels
+00000230: 206f 6620 6578 7065 7269 656e 6365 2e20   of experience. 
+00000240: 5468 6973 2069 6d70 6c65 6d65 6e74 6174  This implementat
+00000250: 696f 6e20 6973 2062 7569 6c64 2074 6f20  ion is build to 
+00000260: 776f 726b 2077 6974 6820 2247 594d 2220  work with "GYM" 
+00000270: 656e 7669 726f 6e6d 656e 7473 2066 726f  environments fro
+00000280: 6d20 7468 6520 5b47 796d 6e61 7369 756d  m the [Gymnasium
+00000290: 2050 726f 6a65 6374 5d28 6874 7470 733a   Project](https:
+000002a0: 2f2f 6779 6d6e 6173 6975 6d2e 6661 7261  //gymnasium.fara
+000002b0: 6d61 2e6f 7267 2f29 2e0d 0a0d 0a23 2320  ma.org/).....## 
+000002c0: 4665 6174 7572 6573 0d0a 0d0a 2d20 5072  Features....- Pr
+000002d0: 6f76 6964 6573 2066 6c65 7869 6269 6c69  ovides flexibili
+000002e0: 7479 2074 6f20 776f 726b 2077 6974 6820  ty to work with 
+000002f0: 6569 7468 6572 2069 6e74 6567 6572 206f  either integer o
+00000300: 7220 6375 7374 6f6d 206f 626a 6563 7473  r custom objects
+00000310: 2066 6f72 2073 7461 7465 7320 616e 6420   for states and 
+00000320: 6163 7469 6f6e 732e 0d0a 2d20 4f66 6665  actions...- Offe
+00000330: 7273 2063 7573 746f 6d69 7a61 626c 6520  rs customizable 
+00000340: 6c65 6172 6e69 6e67 2072 6174 6520 616e  learning rate an
+00000350: 6420 6578 706c 6f72 6174 696f 6e2d 6578  d exploration-ex
+00000360: 706c 6f69 7461 7469 6f6e 2074 7261 6465  ploitation trade
+00000370: 2d6f 6666 2070 6172 616d 6574 6572 732e  -off parameters.
+00000380: 0d0a 2d20 496d 706c 656d 656e 7473 2065  ..- Implements e
+00000390: 7073 696c 6f6e 2d67 7265 6564 7920 7374  psilon-greedy st
+000003a0: 7261 7465 6779 2066 6f72 2061 6374 696f  rategy for actio
+000003b0: 6e20 7365 6c65 6374 696f 6e2e 0d0a 2d20  n selection...- 
+000003c0: 5375 7070 6f72 7473 2070 6f6c 796e 6f6d  Supports polynom
+000003d0: 6961 6c20 616e 6420 706f 7765 7220 6465  ial and power de
+000003e0: 6361 7920 6675 6e63 7469 6f6e 7320 666f  cay functions fo
+000003f0: 7220 6c65 6172 6e69 6e67 2072 6174 6520  r learning rate 
+00000400: 616e 6420 6578 706c 6f72 6174 696f 6e20  and exploration 
+00000410: 7061 7261 6d65 7465 7220 7265 7370 6563  parameter respec
+00000420: 6974 6976 656c 792e 200d 0a20 2054 6865  itively. ..  The
+00000430: 206c 6561 726e 696e 6720 7261 7465 2064   learning rate d
+00000440: 6563 6179 2069 7320 6261 7365 6420 6f6e  ecay is based on
+00000450: 2074 6865 2072 6573 6561 7263 6820 696e   the research in
+00000460: 2045 7665 6e2d 4461 7220 6574 2061 6c2e   Even-Dar et al.
+00000470: 2028 3230 3033 292e 2057 6865 6e20 6c61   (2003). When la
+00000480: 6d62 6461 2069 7320 696e 2028 302c 3129  mbda is in (0,1)
+00000490: 2074 6869 7320 696d 706c 656d 656e 7461   this implementa
+000004a0: 7469 6f6e 206f 6620 512d 6c65 6172 6e69  tion of Q-learni
+000004b0: 6e67 2073 6174 6973 6669 6573 2074 6865  ng satisfies the
+000004c0: 2063 6f6e 6469 7469 6f6e 7320 666f 7220   conditions for 
+000004d0: 7072 6f62 6162 696c 6974 7920 6f6e 6520  probability one 
+000004e0: 636f 6e76 6572 6765 6e63 6520 696e 2057  convergence in W
+000004f0: 6174 6b69 6e73 2061 6e64 2044 6179 616e  atkins and Dayan
+00000500: 2028 3139 3932 292e 0d0a 0d0a 2323 2049   (1992).....## I
+00000510: 6e73 7461 6c6c 6174 696f 6e0d 0a0d 0a49  nstallation....I
+00000520: 6e73 7461 6c6c 2074 6865 2060 5369 6d70  nstall the `Simp
+00000530: 6c65 2d51 6020 7061 636b 6167 6520 6672  le-Q` package fr
+00000540: 6f6d 2050 7950 493a 0d0a 0d0a 6060 6073  om PyPI:....```s
+00000550: 6865 6c6c 0d0a 7069 7020 696e 7374 616c  hell..pip instal
+00000560: 6c20 5369 6d70 6c65 2d51 0d0a 6060 600d  l Simple-Q..```.
+00000570: 0a0d 0a23 2320 5573 6167 650d 0a0d 0a60  ...## Usage....`
+00000580: 6060 7079 7468 6f6e 0d0a 6672 6f6d 2053  ``python..from S
+00000590: 696d 706c 652d 5120 696d 706f 7274 2051  imple-Q import Q
+000005a0: 6c65 6172 6e69 6e67 0d0a 0d0a 2320 4372  learning....# Cr
+000005b0: 6561 7465 2074 6865 2051 2d6c 6561 726e  eate the Q-learn
+000005c0: 696e 6720 6167 656e 740d 0a61 6765 6e74  ing agent..agent
+000005d0: 203d 2051 6c65 6172 6e69 6e67 2873 7461   = Qlearning(sta
+000005e0: 7465 733d 3130 2c20 6163 7469 6f6e 7320  tes=10, actions 
+000005f0: 3d20 5b27 666f 7277 6172 6427 2c20 276c  = ['forward', 'l
+00000600: 6566 7427 2c20 2772 6967 6874 2720 2773  eft', 'right' 's
+00000610: 746f 7027 5d29 0d0a 0d0a 2320 5573 6520  top'])....# Use 
+00000620: 7468 6520 512d 6c65 6172 6e69 6e67 2061  the Q-learning a
+00000630: 6765 6e74 2069 6e20 796f 7572 2072 6569  gent in your rei
+00000640: 6e66 6f72 6365 6d65 6e74 206c 6561 726e  nforcement learn
+00000650: 696e 6720 6c6f 6f70 0d0a 7374 6174 6520  ing loop..state 
+00000660: 3d20 656e 762e 7265 7365 7428 290d 0a4e  = env.reset()..N
+00000670: 203d 2031 3030 0d0a 666f 7220 6e20 696e   = 100..for n in
+00000680: 2072 616e 6765 284e 293a 0d0a 2020 2020   range(N):..    
+00000690: 6163 7469 6f6e 203d 2061 6765 6e74 2e67  action = agent.g
+000006a0: 6574 5f61 6374 696f 6e28 7374 6174 6529  et_action(state)
+000006b0: 0d0a 2020 2020 6e65 7874 5f73 7461 7465  ..    next_state
+000006c0: 2c20 7265 7761 7264 2c20 646f 6e65 2c20  , reward, done, 
+000006d0: 5f20 3d20 656e 762e 7374 6570 2861 6374  _ = env.step(act
+000006e0: 696f 6e29 0d0a 2020 2020 6167 656e 742e  ion)..    agent.
+000006f0: 7570 6461 7465 5f71 5f74 6162 6c65 2873  update_q_table(s
+00000700: 7461 7465 2c20 6163 7469 6f6e 2c20 7265  tate, action, re
+00000710: 7761 7264 2c20 6e65 7874 5f73 7461 7465  ward, next_state
+00000720: 290d 0a20 2020 2073 7461 7465 203d 206e  )..    state = n
+00000730: 6578 745f 7374 6174 650d 0a20 2020 2061  ext_state..    a
+00000740: 6765 6e74 2e75 7064 6174 655f 6570 7369  gent.update_epsi
+00000750: 6c6f 6e28 290d 0a60 6060 0d0a 0d0a 5365  lon()..```....Se
+00000760: 6520 616c 736f 2074 6865 205b 5361 7669  e also the [Savi
+00000770: 6e67 7320 5072 6f62 6c65 6d5d 2868 7474  ngs Problem](htt
+00000780: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000790: 4e65 7374 612d 6769 7455 2f53 696d 706c  Nesta-gitU/Simpl
+000007a0: 652d 512f 7472 6565 2f6d 6169 6e2f 5361  e-Q/tree/main/Sa
+000007b0: 7669 6e67 7350 726f 626c 656d 2920 6578  vingsProblem) ex
+000007c0: 616d 706c 6520 696e 2074 6865 2047 6974  ample in the Git
+000007d0: 4875 6220 7265 706f 7369 746f 7279 2e0d  Hub repository..
+000007e0: 0a0d 0a23 2320 446f 6375 6d65 6e74 6174  ...## Documentat
+000007f0: 696f 6e0d 0a0d 0a54 6865 2051 2d4c 6561  ion....The Q-Lea
+00000800: 726e 696e 6720 636c 6173 7320 7072 6f76  rning class prov
+00000810: 6964 6573 2074 6865 2066 6f6c 6c6f 7769  ides the followi
+00000820: 6e67 2070 6172 616d 6574 6572 733a 0d0a  ng parameters:..
+00000830: 0d0a 7c20 5061 7261 6d65 7465 7220 2020  ..| Parameter   
+00000840: 2020 2020 2020 2020 2020 7c20 4465 7363            | Desc
+00000850: 7269 7074 696f 6e20 2020 2020 2020 2020  ription         
 00000860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000870: 2020 2020 2020 2020 2020 7c0d 0a7c 2d2d            |..|--
-00000880: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000890: 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d  -----|----------
-000008a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000880: 2020 2020 2020 2020 207c 0d0a 7c2d 2d2d           |..|---
+00000890: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000008a0: 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----|-----------
 000008b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000008c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000008d0: 2d2d 2d2d 7c0d 0a7c 2060 7374 6174 6573  ----|..| `states
-000008e0: 6020 2020 2020 2020 2020 2020 2020 207c  `              |
-000008f0: 204e 756d 6265 7220 6f66 2073 7461 7465   Number of state
-00000900: 7320 6f72 2061 206c 6973 7420 6f66 2069  s or a list of i
-00000910: 6d6d 7574 6162 6c65 206f 626a 6563 7473  mmutable objects
-00000920: 2072 6570 7265 7365 6e74 696e 6720 7374   representing st
-00000930: 6174 6573 2e20 4966 2061 206c 6973 7420  ates. If a list 
-00000940: 6973 2070 6173 7365 642c 2074 6865 2073  is passed, the s
-00000950: 7461 7465 7320 6172 6520 6d61 7070 6564  tates are mapped
-00000960: 2074 6f20 696e 7465 6765 7273 2073 7461   to integers sta
-00000970: 7274 696e 6720 6672 6f6d 2030 2c20 616e  rting from 0, an
-00000980: 6420 7468 6520 696d 6d75 7461 626c 6520  d the immutable 
-00000990: 6f62 6a65 6374 7320 286e 6f74 2069 6e64  objects (not ind
-000009a0: 6963 6573 2920 6172 6520 6578 7065 6374  ices) are expect
-000009b0: 6564 2061 7320 696e 7075 7420 666f 7220  ed as input for 
-000009c0: 7468 6520 6f74 6865 7220 6d65 7468 6f64  the other method
-000009d0: 732e 207c 0d0a 7c20 6061 6374 696f 6e73  s. |..| `actions
-000009e0: 6020 2020 2020 2020 2020 2020 2020 7c20  `             | 
-000009f0: 4e75 6d62 6572 206f 6620 6163 7469 6f6e  Number of action
-00000a00: 7320 6f72 2061 206c 6973 7420 6f66 2069  s or a list of i
-00000a10: 6d6d 7574 6162 6c65 206f 626a 6563 7473  mmutable objects
-00000a20: 2072 6570 7265 7365 6e74 696e 6720 6163   representing ac
-00000a30: 7469 6f6e 732e 2049 6620 6120 6c69 7374  tions. If a list
-00000a40: 2069 7320 7061 7373 6564 2c20 7468 6520   is passed, the 
-00000a50: 6163 7469 6f6e 7320 6172 6520 6d61 7070  actions are mapp
-00000a60: 6564 2074 6f20 696e 7465 6765 7273 2073  ed to integers s
-00000a70: 7461 7274 696e 6720 6672 6f6d 2030 2c20  tarting from 0, 
-00000a80: 616e 6420 7468 6520 696d 6d75 7461 626c  and the immutabl
-00000a90: 6520 6f62 6a65 6374 7320 286e 6f74 2069  e objects (not i
-00000aa0: 6e64 6963 6573 2920 6172 6520 6578 7065  ndices) are expe
-00000ab0: 6374 6564 2061 7320 696e 7075 7420 666f  cted as input fo
-00000ac0: 7220 7468 6520 6f74 6865 7220 6d65 7468  r the other meth
-00000ad0: 6f64 732e 207c 0d0a 7c20 6061 6c70 6861  ods. |..| `alpha
-00000ae0: 6020 2020 2020 2020 2020 2020 2020 2020  `               
-00000af0: 7c20 4c65 6172 6e69 6e67 2072 6174 6520  | Learning rate 
-00000b00: 7061 7261 6d65 7465 722e 2049 6620 6027  parameter. If `'
-00000b10: 706f 6c79 6e6f 6d69 616c 2760 2c20 6120  polynomial'`, a 
-00000b20: 706f 6c79 6e6f 6d69 616c 2064 6563 6179  polynomial decay
-00000b30: 2069 7320 7573 6564 2e20 4966 2060 696e   is used. If `in
-00000b40: 7460 206f 7220 6066 6c6f 6174 602c 2061  t` or `float`, a
-00000b50: 2066 6978 6564 2076 616c 7565 2069 7320   fixed value is 
-00000b60: 7573 6564 2e20 7c0d 0a7c 2060 7760 2020  used. |..| `w`  
-00000b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b80: 207c 2044 6563 6179 2065 7870 6f6e 656e   | Decay exponen
-00000b90: 7420 666f 7220 7468 6520 706f 6c79 6e6f  t for the polyno
-00000ba0: 6d69 616c 2064 6563 6179 2e20 4f6e 6c79  mial decay. Only
-00000bb0: 2061 7070 6c69 6361 626c 6520 7768 656e   applicable when
-00000bc0: 2060 616c 7068 613d 2770 6f6c 796e 6f6d   `alpha='polynom
-00000bd0: 6961 6c27 602e 207c 0d0a 7c20 6067 616d  ial'`. |..| `gam
-00000be0: 6d61 6020 2020 2020 2020 2020 2020 2020  ma`             
-00000bf0: 2020 7c20 4469 7363 6f75 6e74 2066 6163    | Discount fac
-00000c00: 746f 7220 666f 7220 6675 7475 7265 2072  tor for future r
-00000c10: 6577 6172 6473 2e20 2020 2020 2020 2020  ewards.         
-00000c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c30: 207c 0d0a 7c20 6065 7073 696c 6f6e 5f64   |..| `epsilon_d
-00000c40: 6563 6179 6020 2020 2020 2020 7c20 4570  ecay`       | Ep
-00000c50: 7369 6c6f 6e20 6465 6361 7920 6675 6e63  silon decay func
-00000c60: 7469 6f6e 2e20 4966 2060 2770 6f77 6572  tion. If `'power
-00000c70: 2760 2c20 6120 706f 7765 7220 6465 6361  '`, a power deca
-00000c80: 7920 6973 2075 7365 642e 207c 0d0a 7c20  y is used. |..| 
-00000c90: 6065 7073 696c 6f6e 6020 2020 2020 2020  `epsilon`       
-00000ca0: 2020 2020 2020 7c20 496e 6974 6961 6c20        | Initial 
-00000cb0: 7661 6c75 6520 666f 7220 7468 6520 6578  value for the ex
-00000cc0: 706c 6f72 6174 696f 6e2d 6578 706c 6f69  ploration-exploi
-00000cd0: 7461 7469 6f6e 2074 7261 6465 2d6f 6666  tation trade-off
-00000ce0: 2070 6172 616d 6574 6572 2e20 7c0d 0a7c   parameter. |..|
-00000cf0: 2060 6570 7369 6c6f 6e5f 6465 6361 795f   `epsilon_decay_
-00000d00: 6661 6374 6f72 607c 2044 6563 6179 2066  factor`| Decay f
-00000d10: 6163 746f 7220 666f 7220 6570 7369 6c6f  actor for epsilo
-00000d20: 6e2e 2044 6574 6572 6d69 6e65 7320 686f  n. Determines ho
-00000d30: 7720 6974 2064 6563 6179 7320 6f76 6572  w it decays over
-00000d40: 2074 696d 652e 207c 0d0a 7c20 6065 7073   time. |..| `eps
-00000d50: 696c 6f6e 5f6d 696e 6020 2020 2020 2020  ilon_min`       
-00000d60: 2020 7c20 4d69 6e69 6d75 6d20 7661 6c75    | Minimum valu
-00000d70: 6520 666f 7220 6570 7369 6c6f 6e2e 2020  e for epsilon.  
-00000d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000008e0: 2d2d 2d7c 0d0a 7c20 6073 7461 7465 7360  ---|..| `states`
+000008f0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00000900: 4e75 6d62 6572 206f 6620 7374 6174 6573  Number of states
+00000910: 206f 7220 6120 6c69 7374 206f 6620 696d   or a list of im
+00000920: 6d75 7461 626c 6520 6f62 6a65 6374 7320  mutable objects 
+00000930: 7265 7072 6573 656e 7469 6e67 2073 7461  representing sta
+00000940: 7465 732e 2049 6620 6120 6c69 7374 2069  tes. If a list i
+00000950: 7320 7061 7373 6564 2c20 7468 6520 7374  s passed, the st
+00000960: 6174 6573 2061 7265 206d 6170 7065 6420  ates are mapped 
+00000970: 746f 2069 6e74 6567 6572 7320 7374 6172  to integers star
+00000980: 7469 6e67 2066 726f 6d20 302c 2061 6e64  ting from 0, and
+00000990: 2074 6865 2069 6d6d 7574 6162 6c65 206f   the immutable o
+000009a0: 626a 6563 7473 2028 6e6f 7420 696e 6469  bjects (not indi
+000009b0: 6365 7329 2061 7265 2065 7870 6563 7465  ces) are expecte
+000009c0: 6420 6173 2069 6e70 7574 2066 6f72 2074  d as input for t
+000009d0: 6865 206f 7468 6572 206d 6574 686f 6473  he other methods
+000009e0: 2e20 7c0d 0a7c 2060 6163 7469 6f6e 7360  . |..| `actions`
+000009f0: 2020 2020 2020 2020 2020 2020 207c 204e               | N
+00000a00: 756d 6265 7220 6f66 2061 6374 696f 6e73  umber of actions
+00000a10: 206f 7220 6120 6c69 7374 206f 6620 696d   or a list of im
+00000a20: 6d75 7461 626c 6520 6f62 6a65 6374 7320  mutable objects 
+00000a30: 7265 7072 6573 656e 7469 6e67 2061 6374  representing act
+00000a40: 696f 6e73 2e20 4966 2061 206c 6973 7420  ions. If a list 
+00000a50: 6973 2070 6173 7365 642c 2074 6865 2061  is passed, the a
+00000a60: 6374 696f 6e73 2061 7265 206d 6170 7065  ctions are mappe
+00000a70: 6420 746f 2069 6e74 6567 6572 7320 7374  d to integers st
+00000a80: 6172 7469 6e67 2066 726f 6d20 302c 2061  arting from 0, a
+00000a90: 6e64 2074 6865 2069 6d6d 7574 6162 6c65  nd the immutable
+00000aa0: 206f 626a 6563 7473 2028 6e6f 7420 696e   objects (not in
+00000ab0: 6469 6365 7329 2061 7265 2065 7870 6563  dices) are expec
+00000ac0: 7465 6420 6173 2069 6e70 7574 2066 6f72  ted as input for
+00000ad0: 2074 6865 206f 7468 6572 206d 6574 686f   the other metho
+00000ae0: 6473 2e20 7c0d 0a7c 2060 616c 7068 6160  ds. |..| `alpha`
+00000af0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00000b00: 204c 6561 726e 696e 6720 7261 7465 2070   Learning rate p
+00000b10: 6172 616d 6574 6572 2e20 4966 2060 2770  arameter. If `'p
+00000b20: 6f6c 796e 6f6d 6961 6c27 602c 2061 2070  olynomial'`, a p
+00000b30: 6f6c 796e 6f6d 6961 6c20 6465 6361 7920  olynomial decay 
+00000b40: 6973 2075 7365 642e 2049 6620 6069 6e74  is used. If `int
+00000b50: 6020 6f72 2060 666c 6f61 7460 2c20 6120  ` or `float`, a 
+00000b60: 6669 7865 6420 7661 6c75 6520 6973 2075  fixed value is u
+00000b70: 7365 642e 207c 0d0a 7c20 6077 6020 2020  sed. |..| `w`   
+00000b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b90: 7c20 4465 6361 7920 6578 706f 6e65 6e74  | Decay exponent
+00000ba0: 2066 6f72 2074 6865 2070 6f6c 796e 6f6d   for the polynom
+00000bb0: 6961 6c20 6465 6361 792e 204f 6e6c 7920  ial decay. Only 
+00000bc0: 6170 706c 6963 6162 6c65 2077 6865 6e20  applicable when 
+00000bd0: 6061 6c70 6861 3d27 706f 6c79 6e6f 6d69  `alpha='polynomi
+00000be0: 616c 2760 2e20 7c0d 0a7c 2060 6761 6d6d  al'`. |..| `gamm
+00000bf0: 6160 2020 2020 2020 2020 2020 2020 2020  a`              
+00000c00: 207c 2044 6973 636f 756e 7420 6661 6374   | Discount fact
+00000c10: 6f72 2066 6f72 2066 7574 7572 6520 7265  or for future re
+00000c20: 7761 7264 732e 2020 2020 2020 2020 2020  wards.          
+00000c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c40: 7c0d 0a7c 2060 6570 7369 6c6f 6e5f 6465  |..| `epsilon_de
+00000c50: 6361 7960 2020 2020 2020 207c 2045 7073  cay`       | Eps
+00000c60: 696c 6f6e 2064 6563 6179 2066 756e 6374  ilon decay funct
+00000c70: 696f 6e2e 2049 6620 6027 706f 7765 7227  ion. If `'power'
+00000c80: 602c 2061 2070 6f77 6572 2064 6563 6179  `, a power decay
+00000c90: 2069 7320 7573 6564 2e20 7c0d 0a7c 2060   is used. |..| `
+00000ca0: 6570 7369 6c6f 6e60 2020 2020 2020 2020  epsilon`        
+00000cb0: 2020 2020 207c 2049 6e69 7469 616c 2076       | Initial v
+00000cc0: 616c 7565 2066 6f72 2074 6865 2065 7870  alue for the exp
+00000cd0: 6c6f 7261 7469 6f6e 2d65 7870 6c6f 6974  loration-exploit
+00000ce0: 6174 696f 6e20 7472 6164 652d 6f66 6620  ation trade-off 
+00000cf0: 7061 7261 6d65 7465 722e 207c 0d0a 7c20  parameter. |..| 
+00000d00: 6065 7073 696c 6f6e 5f64 6563 6179 5f66  `epsilon_decay_f
+00000d10: 6163 746f 7260 7c20 4465 6361 7920 6661  actor`| Decay fa
+00000d20: 6374 6f72 2066 6f72 2065 7073 696c 6f6e  ctor for epsilon
+00000d30: 2e20 4465 7465 726d 696e 6573 2068 6f77  . Determines how
+00000d40: 2069 7420 6465 6361 7973 206f 7665 7220   it decays over 
+00000d50: 7469 6d65 2e20 7c0d 0a7c 2060 6570 7369  time. |..| `epsi
+00000d60: 6c6f 6e5f 6d69 6e60 2020 2020 2020 2020  lon_min`        
+00000d70: 207c 204d 696e 696d 756d 2076 616c 7565   | Minimum value
+00000d80: 2066 6f72 2065 7073 696c 6f6e 2e20 2020   for epsilon.   
 00000d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000da0: 207c 0d0a 0d0a 5468 6520 512d 4c65 6172   |....The Q-Lear
-00000db0: 6e69 6e67 2063 6c61 7373 2070 726f 7669  ning class provi
-00000dc0: 6465 7320 7468 6520 666f 6c6c 6f77 696e  des the followin
-00000dd0: 6720 6174 7472 6962 7574 6573 3a0d 0a0d  g attributes:...
-00000de0: 0a7c 2041 7474 7269 6275 7465 2020 7c20  .| Attribute  | 
-00000df0: 4465 7363 7269 7074 696f 6e20 2020 2020  Description     
-00000e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000db0: 7c0d 0a0d 0a54 6865 2051 2d4c 6561 726e  |....The Q-Learn
+00000dc0: 696e 6720 636c 6173 7320 7072 6f76 6964  ing class provid
+00000dd0: 6573 2074 6865 2066 6f6c 6c6f 7769 6e67  es the following
+00000de0: 2061 7474 7269 6275 7465 733a 0d0a 0d0a   attributes:....
+00000df0: 7c20 4174 7472 6962 7574 6520 207c 2044  | Attribute  | D
+00000e00: 6573 6372 6970 7469 6f6e 2020 2020 2020  escription      
 00000e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e20: 2020 2020 2020 2020 2020 2020 207c 0d0a               |..
-00000e30: 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d  |------------|--
-00000e40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e30: 2020 2020 2020 2020 2020 2020 7c0d 0a7c              |..|
+00000e40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d  ------------|---
 00000e50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00000e60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000e70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c0d 0a7c  ------------|..|
-00000e80: 2060 715f 7461 626c 6560 2020 7c20 512d   `q_table`  | Q-
-00000e90: 7461 626c 6520 7374 6f72 696e 6720 7468  table storing th
-00000ea0: 6520 6c65 6172 6e65 6420 512d 7661 6c75  e learned Q-valu
-00000eb0: 6573 2066 6f72 2073 7461 7465 2d61 6374  es for state-act
-00000ec0: 696f 6e20 7061 6972 732e 207c 0d0a 0d0a  ion pairs. |....
-00000ed0: 2323 2043 6f6e 7472 6962 7574 696e 670d  ## Contributing.
-00000ee0: 0a0d 0a43 6f6e 7472 6962 7574 696f 6e73  ...Contributions
-00000ef0: 2061 7265 2077 656c 636f 6d65 2120 4966   are welcome! If
-00000f00: 2079 6f75 2066 696e 6420 616e 7920 6973   you find any is
-00000f10: 7375 6573 206f 7220 6861 7665 2073 7567  sues or have sug
-00000f20: 6765 7374 696f 6e73 2066 6f72 2069 6d70  gestions for imp
-00000f30: 726f 7665 6d65 6e74 2c20 706c 6561 7365  rovement, please
-00000f40: 2066 6565 6c20 6672 6565 2074 6f20 6f70   feel free to op
-00000f50: 656e 2061 6e20 6973 7375 6520 6f72 2073  en an issue or s
-00000f60: 7562 6d69 7420 6120 7075 6c6c 2072 6571  ubmit a pull req
-00000f70: 7565 7374 2e0d 0a0d 0a23 2320 4c69 6365  uest.....## Lice
-00000f80: 6e73 650d 0a0d 0a54 6869 7320 7072 6f6a  nse....This proj
-00000f90: 6563 7420 6973 206c 6963 656e 7365 6420  ect is licensed 
-00000fa0: 756e 6465 7220 7468 6520 5b4d 4954 204c  under the [MIT L
-00000fb0: 6963 656e 7365 5d28 6874 7470 733a 2f2f  icense](https://
-00000fc0: 6769 7468 7562 2e63 6f6d 2f4e 6573 7461  github.com/Nesta
-00000fd0: 2d67 6974 552f 5369 6d70 6c65 2d51 2f53  -gitU/Simple-Q/S
-00000fe0: 696d 706c 652d 512f 4c49 4345 4e53 4529  imple-Q/LICENSE)
-00000ff0: 2e0d 0a0d 0a23 2320 4163 6b6e 6f77 6c65  .....## Acknowle
-00001000: 6467 656d 656e 7473 0d0a 0d0a 5468 6973  dgements....This
-00001010: 2063 6f64 6520 6973 206f 7269 6769 6e61   code is origina
-00001020: 6c6c 7920 6261 7365 6420 7570 6f6e 2074  lly based upon t
-00001030: 6865 205b 512d 4c65 6172 6e69 6e67 2069  he [Q-Learning i
-00001040: 6d70 6c65 6d65 6e74 6174 696f 6e5d 280d  mplementation](.
-00001050: 0a0d 0a23 2320 5265 6665 7265 6e63 6573  ...## References
-00001060: 0d0a 4576 656e 2d44 6172 2c20 452e 2c20  ..Even-Dar, E., 
-00001070: 592e 204d 616e 736f 7572 2c20 616e 6420  Y. Mansour, and 
-00001080: 502e 2042 6172 746c 6574 7420 2832 3030  P. Bartlett (200
-00001090: 3329 2e20 4c65 6172 6e69 6e67 2072 6174  3). Learning rat
-000010a0: 6573 2066 6f72 2071 2d6c 6561 726e 696e  es for q-learnin
-000010b0: 672e 204a 6f75 726e 616c 206f 6620 6d61  g. Journal of ma
-000010c0: 6368 696e 650d 0a6c 6561 726e 696e 6720  chine..learning 
-000010d0: 5265 7365 6172 6368 2035 2831 292e 0d0a  Research 5(1)...
-000010e0: 0d0a 5761 746b 696e 732c 2043 2e20 4a2e  ..Watkins, C. J.
-000010f0: 2061 6e64 2050 2e20 4461 7961 6e20 2831   and P. Dayan (1
-00001100: 3939 322c 204d 6179 292e 2054 6563 686e  992, May). Techn
-00001110: 6963 616c 206e 6f74 653a 2051 2d6c 6561  ical note: Q-lea
-00001120: 726e 696e 672e 204d 6163 6869 6e65 204c  rning. Machine L
-00001130: 6561 726e 696e 6720 3828 3329 2c0d 0a32  earning 8(3),..2
-00001140: 3739 e280 9332 3932 0d0a 6060 60         79...292..```
+00000e70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000e80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 0d0a 7c20  -----------|..| 
+00000e90: 6071 5f74 6162 6c65 6020 207c 2051 2d74  `q_table`  | Q-t
+00000ea0: 6162 6c65 2073 746f 7269 6e67 2074 6865  able storing the
+00000eb0: 206c 6561 726e 6564 2051 2d76 616c 7565   learned Q-value
+00000ec0: 7320 666f 7220 7374 6174 652d 6163 7469  s for state-acti
+00000ed0: 6f6e 2070 6169 7273 2e20 7c0d 0a0d 0a23  on pairs. |....#
+00000ee0: 2320 436f 6e74 7269 6275 7469 6e67 0d0a  # Contributing..
+00000ef0: 0d0a 436f 6e74 7269 6275 7469 6f6e 7320  ..Contributions 
+00000f00: 6172 6520 7765 6c63 6f6d 6521 2049 6620  are welcome! If 
+00000f10: 796f 7520 6669 6e64 2061 6e79 2069 7373  you find any iss
+00000f20: 7565 7320 6f72 2068 6176 6520 7375 6767  ues or have sugg
+00000f30: 6573 7469 6f6e 7320 666f 7220 696d 7072  estions for impr
+00000f40: 6f76 656d 656e 742c 2070 6c65 6173 6520  ovement, please 
+00000f50: 6665 656c 2066 7265 6520 746f 206f 7065  feel free to ope
+00000f60: 6e20 616e 2069 7373 7565 206f 7220 7375  n an issue or su
+00000f70: 626d 6974 2061 2070 756c 6c20 7265 7175  bmit a pull requ
+00000f80: 6573 742e 0d0a 0d0a 2323 204c 6963 656e  est.....## Licen
+00000f90: 7365 0d0a 0d0a 5468 6973 2070 726f 6a65  se....This proje
+00000fa0: 6374 2069 7320 6c69 6365 6e73 6564 2075  ct is licensed u
+00000fb0: 6e64 6572 2074 6865 205b 4d49 5420 4c69  nder the [MIT Li
+00000fc0: 6365 6e73 655d 2868 7474 7073 3a2f 2f67  cense](https://g
+00000fd0: 6974 6875 622e 636f 6d2f 4e65 7374 612d  ithub.com/Nesta-
+00000fe0: 6769 7455 2f53 696d 706c 652d 512f 626c  gitU/Simple-Q/bl
+00000ff0: 6f62 2f6d 6169 6e2f 5369 6d70 6c65 5f51  ob/main/Simple_Q
+00001000: 2f4c 4943 454e 5345 292e 0d0a 0d0a 2323  /LICENSE).....##
+00001010: 2041 636b 6e6f 776c 6564 6765 6d65 6e74   Acknowledgement
+00001020: 730d 0a0d 0a54 6869 7320 636f 6465 2069  s....This code i
+00001030: 7320 6f72 6967 696e 616c 6c79 2062 6173  s originally bas
+00001040: 6564 2075 706f 6e20 7468 6520 5b51 2d4c  ed upon the [Q-L
+00001050: 6561 726e 696e 6720 696d 706c 656d 656e  earning implemen
+00001060: 7461 7469 6f6e 5d28 6874 7470 733a 2f2f  tation](https://
+00001070: 6769 7468 7562 2e63 6f6d 2f50 6163 6b74  github.com/Packt
+00001080: 5075 626c 6973 6869 6e67 2f41 6476 616e  Publishing/Advan
+00001090: 6365 642d 4465 6570 2d4c 6561 726e 696e  ced-Deep-Learnin
+000010a0: 672d 7769 7468 2d4b 6572 6173 2f62 6c6f  g-with-Keras/blo
+000010b0: 622f 6d61 7374 6572 2f63 6861 7074 6572  b/master/chapter
+000010c0: 392d 6472 6c2f 712d 6c65 6172 6e69 6e67  9-drl/q-learning
+000010d0: 2d39 2e33 2e31 2e70 7929 2066 726f 6d20  -9.3.1.py) from 
+000010e0: 7468 6520 626f 6f6b 3a20 4164 7661 6e63  the book: Advanc
+000010f0: 6564 2044 6565 7020 4c65 6172 6e69 6e67  ed Deep Learning
+00001100: 2077 6974 6820 5465 6e73 6f72 466c 6f77   with TensorFlow
+00001110: 2032 2061 6e64 204b 6572 6173 2062 7920   2 and Keras by 
+00001120: 526f 7765 6c20 4174 6965 6e7a 612e 2048  Rowel Atienza. H
+00001130: 6f77 6576 6572 206d 616e 7920 6368 616e  owever many chan
+00001140: 6765 7320 6861 7665 2062 6565 6e20 6d61  ges have been ma
+00001150: 6465 2074 6f20 7468 6520 6f72 6967 696e  de to the origin
+00001160: 616c 2063 6f64 652c 2069 6e63 6c75 6469  al code, includi
+00001170: 6e67 2074 6865 2061 6464 6974 696f 6e20  ng the addition 
+00001180: 6f66 2074 6865 2070 6f6c 796e 6f6d 6961  of the polynomia
+00001190: 6c20 6c65 6172 6e69 6e67 2072 6174 6520  l learning rate 
+000011a0: 6465 6361 7920 6173 2077 656c 6c20 6173  decay as well as
+000011b0: 2074 6865 2061 6269 6c69 7479 2074 6f20   the ability to 
+000011c0: 776f 726b 2077 6974 6820 6375 7374 6f6d  work with custom
+000011d0: 206f 626a 6563 7473 2066 6f72 2073 7461   objects for sta
+000011e0: 7465 7320 616e 6420 6163 7469 6f6e 732e  tes and actions.
+000011f0: 200d 0a0d 0a23 2320 5265 6665 7265 6e63   ....## Referenc
+00001200: 6573 0d0a 4576 656e 2d44 6172 2c20 452e  es..Even-Dar, E.
+00001210: 2c20 592e 204d 616e 736f 7572 2c20 616e  , Y. Mansour, an
+00001220: 6420 502e 2042 6172 746c 6574 7420 2832  d P. Bartlett (2
+00001230: 3030 3329 2e20 4c65 6172 6e69 6e67 2072  003). Learning r
+00001240: 6174 6573 2066 6f72 2071 2d6c 6561 726e  ates for q-learn
+00001250: 696e 672e 204a 6f75 726e 616c 206f 6620  ing. Journal of 
+00001260: 6d61 6368 696e 650d 0a6c 6561 726e 696e  machine..learnin
+00001270: 6720 5265 7365 6172 6368 2035 2831 292e  g Research 5(1).
+00001280: 0d0a 0d0a 5761 746b 696e 732c 2043 2e20  ....Watkins, C. 
+00001290: 4a2e 2061 6e64 2050 2e20 4461 7961 6e20  J. and P. Dayan 
+000012a0: 2831 3939 322c 204d 6179 292e 2054 6563  (1992, May). Tec
+000012b0: 686e 6963 616c 206e 6f74 653a 2051 2d6c  hnical note: Q-l
+000012c0: 6561 726e 696e 672e 204d 6163 6869 6e65  earning. Machine
+000012d0: 204c 6561 726e 696e 6720 3828 3329 2c0d   Learning 8(3),.
+000012e0: 0a32 3739 e280 9332 3932 0d0a            .279...292..
```

### Comparing `Simple_Q-1.0.0/Simple_Q.egg-info/PKG-INFO` & `Simple_Q-1.0.1/Simple_Q.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simple-Q
-Version: 1.0.0
+Version: 1.0.1
 Summary: A low learning curve implementation of a Q-Learning algorithm.
 Author-email: Nesta <nesta110402@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -26,23 +26,22 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-```
 # Q-Learning
 
 A low learning curve implementation of Q-learning.
 
 [![PyPI](https://img.shields.io/pypi/v/qlearning)](https://pypi.org/project/Simple-Q/)
-[![License](https://img.shields.io/pypi/l/qlearning)](https://github.com/Nesta-gitU/Simple-Q/Simple-Q/LICENSE).
+[![License](https://img.shields.io/pypi/l/qlearning)](https://github.com/Nesta-gitU/Simple-Q/blob/main/Simple_Q/LICENSE).
 
-Q-learning is a reinforcement learning algorithm that allows an agent to learn an optimal policy for sequential decision-making problems. This implementation provides an easy-to-use and beginner-friendly approach to Q-learning, making it accessible to users with varying levels of experience. This implementation is build to work with "GYM" environments from the [Gymnasium Project](https://gymnasium.farama.org/) 
+Q-learning is a reinforcement learning algorithm that allows an agent to learn an optimal policy for sequential decision-making problems. This implementation provides an easy-to-use and beginner-friendly approach to Q-learning, making it accessible to users with varying levels of experience. This implementation is build to work with "GYM" environments from the [Gymnasium Project](https://gymnasium.farama.org/).
 
 ## Features
 
 - Provides flexibility to work with either integer or custom objects for states and actions.
 - Offers customizable learning rate and exploration-exploitation trade-off parameters.
 - Implements epsilon-greedy strategy for action selection.
 - Supports polynomial and power decay functions for learning rate and exploration parameter respecitively. 
@@ -71,15 +70,15 @@
     action = agent.get_action(state)
     next_state, reward, done, _ = env.step(action)
     agent.update_q_table(state, action, reward, next_state)
     state = next_state
     agent.update_epsilon()
 ```
 
-See also the [Savings Problem](https://github.com/Nesta-gitU/Simple-Q/SavingsProblem) example in the GitHub repository.
+See also the [Savings Problem](https://github.com/Nesta-gitU/Simple-Q/tree/main/SavingsProblem) example in the GitHub repository.
 
 ## Documentation
 
 The Q-Learning class provides the following parameters:
 
 | Parameter             | Description                                                  |
 |-----------------------|--------------------------------------------------------------|
@@ -101,20 +100,19 @@
 
 ## Contributing
 
 Contributions are welcome! If you find any issues or have suggestions for improvement, please feel free to open an issue or submit a pull request.
 
 ## License
 
-This project is licensed under the [MIT License](https://github.com/Nesta-gitU/Simple-Q/Simple-Q/LICENSE).
+This project is licensed under the [MIT License](https://github.com/Nesta-gitU/Simple-Q/blob/main/Simple_Q/LICENSE).
 
 ## Acknowledgements
 
-This code is originally based upon the [Q-Learning implementation](
+This code is originally based upon the [Q-Learning implementation](https://github.com/PacktPublishing/Advanced-Deep-Learning-with-Keras/blob/master/chapter9-drl/q-learning-9.3.1.py) from the book: Advanced Deep Learning with TensorFlow 2 and Keras by Rowel Atienza. However many changes have been made to the original code, including the addition of the polynomial learning rate decay as well as the ability to work with custom objects for states and actions. 
 
 ## References
 Even-Dar, E., Y. Mansour, and P. Bartlett (2003). Learning rates for q-learning. Journal of machine
 learning Research 5(1).
 
 Watkins, C. J. and P. Dayan (1992, May). Technical note: Q-learning. Machine Learning 8(3),
 279–292
-```
```

### Comparing `Simple_Q-1.0.0/pyproject.toml` & `Simple_Q-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Simple_Q"
-version = "1.0.0"
+version = "1.0.1"
 description = "A low learning curve implementation of a Q-Learning algorithm."
 readme = "README.md"
 authors = [{ name = "Nesta", email = "nesta110402@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

