# Comparing `tmp/connect_four_game-0.1.4.tar.gz` & `tmp/connect_four_game-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/connect_four_game-0.1.4.tar", last modified: Fri Jul  7 15:43:07 2023, max compression
+gzip compressed data, was "dist/connect_four_game-0.1.5.tar", last modified: Fri Jul 14 15:27:30 2023, max compression
```

## Comparing `connect_four_game-0.1.4.tar` & `connect_four_game-0.1.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:43:07.000000 connect_four_game-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-07 15:42:51.000000 connect_four_game-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-07 15:42:51.000000 connect_four_game-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16010 2023-07-07 15:43:07.000000 connect_four_game-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14903 2023-07-07 15:42:51.000000 connect_four_game-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-07 15:42:51.000000 connect_four_game-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-07 15:43:07.000000 connect_four_game-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-07 15:42:51.000000 connect_four_game-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:43:07.000000 connect_four_game-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:43:07.000000 connect_four_game-0.1.4/src/connect_four_game/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-07 15:42:51.000000 connect_four_game-0.1.4/src/connect_four_game/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:43:07.000000 connect_four_game-0.1.4/src/connect_four_game/app/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-07 15:42:51.000000 connect_four_game-0.1.4/src/connect_four_game/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:43:07.000000 connect_four_game-0.1.4/src/connect_four_game/app/agent/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-07 15:42:51.000000 connect_four_game-0.1.4/src/connect_four_game/app/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-07 15:42:51.000000 connect_four_game-0.1.4/src/connect_four_game/app/agent/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-07 15:42:51.000000 connect_four_game-0.1.4/src/connect_four_game/app/agent/base_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-07 15:42:51.000000 connect_four_game-0.1.4/src/connect_four_game/app/agent/test_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:43:07.000000 connect_four_game-0.1.4/src/connect_four_game/app/board/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-07 15:42:51.000000 connect_four_game-0.1.4/src/connect_four_game/app/board/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-07 15:42:51.000000 connect_four_game-0.1.4/src/connect_four_game/app/board/board.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-07 15:42:51.000000 connect_four_game-0.1.4/src/connect_four_game/app/board/test_board.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:43:07.000000 connect_four_game-0.1.4/src/connect_four_game/app/board_evaluator/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-07 15:42:51.000000 connect_four_game-0.1.4/src/connect_four_game/app/board_evaluator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-07 15:42:51.000000 connect_four_game-0.1.4/src/connect_four_game/app/board_evaluator/board_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-07 15:42:51.000000 connect_four_game-0.1.4/src/connect_four_game/app/board_evaluator/test_board_evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:43:07.000000 connect_four_game-0.1.4/src/connect_four_game/app/lifecycle_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 15:42:51.000000 connect_four_game-0.1.4/src/connect_four_game/app/lifecycle_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-07 15:42:51.000000 connect_four_game-0.1.4/src/connect_four_game/app/lifecycle_manager/lifecycle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-07 15:42:51.000000 connect_four_game-0.1.4/src/connect_four_game/app/setup_test_env.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-07 15:42:51.000000 connect_four_game-0.1.4/src/connect_four_game/app/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:43:07.000000 connect_four_game-0.1.4/src/connect_four_game.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16010 2023-07-07 15:43:07.000000 connect_four_game-0.1.4/src/connect_four_game.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-07 15:43:07.000000 connect_four_game-0.1.4/src/connect_four_game.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 15:43:07.000000 connect_four_game-0.1.4/src/connect_four_game.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-07 15:43:07.000000 connect_four_game-0.1.4/src/connect_four_game.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-07 15:43:07.000000 connect_four_game-0.1.4/src/connect_four_game.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:27:30.000000 connect_four_game-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-14 15:27:14.000000 connect_four_game-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-14 15:27:14.000000 connect_four_game-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-14 15:27:30.000000 connect_four_game-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-14 15:27:14.000000 connect_four_game-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-14 15:27:14.000000 connect_four_game-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-14 15:27:30.000000 connect_four_game-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-14 15:27:14.000000 connect_four_game-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:27:30.000000 connect_four_game-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:27:30.000000 connect_four_game-0.1.5/src/connect_four_game/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-14 15:27:14.000000 connect_four_game-0.1.5/src/connect_four_game/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:27:30.000000 connect_four_game-0.1.5/src/connect_four_game/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-14 15:27:14.000000 connect_four_game-0.1.5/src/connect_four_game/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:27:30.000000 connect_four_game-0.1.5/src/connect_four_game/app/agent/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-14 15:27:14.000000 connect_four_game-0.1.5/src/connect_four_game/app/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-14 15:27:14.000000 connect_four_game-0.1.5/src/connect_four_game/app/agent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-14 15:27:14.000000 connect_four_game-0.1.5/src/connect_four_game/app/agent/base_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-14 15:27:14.000000 connect_four_game-0.1.5/src/connect_four_game/app/agent/test_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:27:30.000000 connect_four_game-0.1.5/src/connect_four_game/app/board/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-14 15:27:14.000000 connect_four_game-0.1.5/src/connect_four_game/app/board/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-14 15:27:14.000000 connect_four_game-0.1.5/src/connect_four_game/app/board/board.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-14 15:27:14.000000 connect_four_game-0.1.5/src/connect_four_game/app/board/test_board.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:27:30.000000 connect_four_game-0.1.5/src/connect_four_game/app/board_evaluator/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-14 15:27:14.000000 connect_four_game-0.1.5/src/connect_four_game/app/board_evaluator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-14 15:27:14.000000 connect_four_game-0.1.5/src/connect_four_game/app/board_evaluator/board_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-14 15:27:14.000000 connect_four_game-0.1.5/src/connect_four_game/app/board_evaluator/test_board_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:27:30.000000 connect_four_game-0.1.5/src/connect_four_game/app/lifecycle_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 15:27:14.000000 connect_four_game-0.1.5/src/connect_four_game/app/lifecycle_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-14 15:27:14.000000 connect_four_game-0.1.5/src/connect_four_game/app/lifecycle_manager/lifecycle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-14 15:27:14.000000 connect_four_game-0.1.5/src/connect_four_game/app/setup_test_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-14 15:27:14.000000 connect_four_game-0.1.5/src/connect_four_game/app/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:27:30.000000 connect_four_game-0.1.5/src/connect_four_game.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-14 15:27:30.000000 connect_four_game-0.1.5/src/connect_four_game.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-14 15:27:30.000000 connect_four_game-0.1.5/src/connect_four_game.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 15:27:30.000000 connect_four_game-0.1.5/src/connect_four_game.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 15:27:30.000000 connect_four_game-0.1.5/src/connect_four_game.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 15:27:30.000000 connect_four_game-0.1.5/src/connect_four_game.egg-info/top_level.txt
```

### Comparing `connect_four_game-0.1.4/LICENSE` & `connect_four_game-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `connect_four_game-0.1.4/setup.py` & `connect_four_game-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `connect_four_game-0.1.4/src/connect_four_game/app/agent/agent.py` & `connect_four_game-0.1.5/src/connect_four_game/app/agent/agent.py`

 * *Files identical despite different names*

### Comparing `connect_four_game-0.1.4/src/connect_four_game/app/board/board.py` & `connect_four_game-0.1.5/src/connect_four_game/app/board/board.py`

 * *Files identical despite different names*

### Comparing `connect_four_game-0.1.4/src/connect_four_game/app/board/test_board.py` & `connect_four_game-0.1.5/src/connect_four_game/app/board/test_board.py`

 * *Files identical despite different names*

### Comparing `connect_four_game-0.1.4/src/connect_four_game/app/board_evaluator/board_evaluator.py` & `connect_four_game-0.1.5/src/connect_four_game/app/board_evaluator/board_evaluator.py`

 * *Files identical despite different names*

### Comparing `connect_four_game-0.1.4/src/connect_four_game/app/board_evaluator/test_board_evaluator.py` & `connect_four_game-0.1.5/src/connect_four_game/app/board_evaluator/test_board_evaluator.py`

 * *Files identical despite different names*

### Comparing `connect_four_game-0.1.4/src/connect_four_game/app/lifecycle_manager/lifecycle_manager.py` & `connect_four_game-0.1.5/src/connect_four_game/app/lifecycle_manager/lifecycle_manager.py`

 * *Files identical despite different names*

### Comparing `connect_four_game-0.1.4/src/connect_four_game.egg-info/SOURCES.txt` & `connect_four_game-0.1.5/src/connect_four_game.egg-info/SOURCES.txt`

 * *Files identical despite different names*

