# Comparing `tmp/chess-board-0.4.0.tar.gz` & `tmp/chess-board-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess-board-0.4.0.tar", last modified: Mon Jul 10 20:46:59 2023, max compression
+gzip compressed data, was "chess-board-0.4.1.tar", last modified: Fri Jul 14 13:55:01 2023, max compression
```

## Comparing `chess-board-0.4.0.tar` & `chess-board-0.4.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 20:46:59.614145 chess-board-0.4.0/
--rw-rw-rw-   0        0        0    35128 2022-04-10 11:32:03.000000 chess-board-0.4.0/LICENSE
--rw-rw-rw-   0        0        0       28 2022-05-15 10:49:54.000000 chess-board-0.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2325 2023-07-10 20:46:59.614145 chess-board-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     1655 2023-07-09 03:20:46.000000 chess-board-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 20:46:59.517675 chess-board-0.4.0/chess_board.egg-info/
--rw-rw-rw-   0        0        0     2325 2023-07-10 20:46:59.000000 chess-board-0.4.0/chess_board.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      722 2023-07-10 20:46:59.000000 chess-board-0.4.0/chess_board.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 20:46:59.000000 chess-board-0.4.0/chess_board.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-10 20:46:59.000000 chess-board-0.4.0/chess_board.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-10 20:46:59.000000 chess-board-0.4.0/chess_board.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-10 20:46:59.555510 chess-board-0.4.0/chessboard/
--rw-rw-rw-   0        0        0        0 2022-04-10 11:32:03.000000 chess-board-0.4.0/chessboard/__init__.py
--rw-rw-rw-   0        0        0     5106 2023-07-09 04:24:41.000000 chess-board-0.4.0/chessboard/board.py
--rw-rw-rw-   0        0        0      244 2022-04-10 11:32:03.000000 chess-board-0.4.0/chessboard/constants.py
--rw-rw-rw-   0        0        0     1194 2023-07-09 03:32:25.000000 chess-board-0.4.0/chessboard/display.py
--rw-rw-rw-   0        0        0      787 2023-07-09 03:24:53.000000 chess-board-0.4.0/chessboard/fenparser.py
-drwxrwxrwx   0        0        0        0 2023-07-10 20:46:59.614145 chess-board-0.4.0/chessboard/images/
--rw-rw-rw-   0        0        0      905 2022-04-10 11:32:03.000000 chess-board-0.4.0/chessboard/images/bB.png
--rw-rw-rw-   0        0        0     1955 2022-04-10 11:32:03.000000 chess-board-0.4.0/chessboard/images/bK.png
--rw-rw-rw-   0        0        0     1239 2022-04-10 11:32:03.000000 chess-board-0.4.0/chessboard/images/bN.png
--rw-rw-rw-   0        0        0      561 2022-04-10 11:32:03.000000 chess-board-0.4.0/chessboard/images/bP.png
--rw-rw-rw-   0        0        0     1797 2022-04-10 11:32:03.000000 chess-board-0.4.0/chessboard/images/bQ.png
--rw-rw-rw-   0        0        0      652 2022-04-10 11:32:03.000000 chess-board-0.4.0/chessboard/images/bR.png
--rw-rw-rw-   0        0        0      330 2022-04-10 11:32:03.000000 chess-board-0.4.0/chessboard/images/btile.png
--rw-rw-rw-   0        0        0     1475 2022-04-10 11:32:03.000000 chess-board-0.4.0/chessboard/images/wB.png
--rw-rw-rw-   0        0        0     1910 2022-04-10 11:32:03.000000 chess-board-0.4.0/chessboard/images/wK.png
--rw-rw-rw-   0        0        0     1508 2022-04-10 11:32:03.000000 chess-board-0.4.0/chessboard/images/wN.png
--rw-rw-rw-   0        0        0      988 2022-04-10 11:32:03.000000 chess-board-0.4.0/chessboard/images/wP.png
--rw-rw-rw-   0        0        0     2288 2022-04-10 11:32:03.000000 chess-board-0.4.0/chessboard/images/wQ.png
--rw-rw-rw-   0        0        0     1043 2022-04-10 11:32:03.000000 chess-board-0.4.0/chessboard/images/wR.png
--rw-rw-rw-   0        0        0      208 2022-04-10 11:32:03.000000 chess-board-0.4.0/chessboard/images/wtile.png
--rw-rw-rw-   0        0        0     2869 2022-07-12 13:32:23.000000 chess-board-0.4.0/chessboard/pieces.py
--rw-rw-rw-   0        0        0       66 2022-04-10 11:32:58.000000 chess-board-0.4.0/chessboard/utils.py
--rw-rw-rw-   0        0        0       42 2023-07-10 20:46:59.614145 chess-board-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     3823 2023-07-10 20:42:22.000000 chess-board-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 13:55:01.828029 chess-board-0.4.1/
+-rw-rw-rw-   0        0        0    35128 2022-04-10 11:32:03.000000 chess-board-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0       28 2022-05-15 10:49:54.000000 chess-board-0.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2421 2023-07-14 13:55:01.827028 chess-board-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1747 2023-07-10 20:52:02.000000 chess-board-0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 13:55:01.797032 chess-board-0.4.1/chess_board.egg-info/
+-rw-rw-rw-   0        0        0     2421 2023-07-14 13:55:01.000000 chess-board-0.4.1/chess_board.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      722 2023-07-14 13:55:01.000000 chess-board-0.4.1/chess_board.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 13:55:01.000000 chess-board-0.4.1/chess_board.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-14 13:55:01.000000 chess-board-0.4.1/chess_board.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-14 13:55:01.000000 chess-board-0.4.1/chess_board.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 13:55:01.807014 chess-board-0.4.1/chessboard/
+-rw-rw-rw-   0        0        0        0 2022-04-10 11:32:03.000000 chess-board-0.4.1/chessboard/__init__.py
+-rw-rw-rw-   0        0        0     5106 2023-07-09 04:24:41.000000 chess-board-0.4.1/chessboard/board.py
+-rw-rw-rw-   0        0        0      244 2022-04-10 11:32:03.000000 chess-board-0.4.1/chessboard/constants.py
+-rw-rw-rw-   0        0        0     1275 2023-07-14 13:47:43.000000 chess-board-0.4.1/chessboard/display.py
+-rw-rw-rw-   0        0        0      787 2023-07-09 03:24:53.000000 chess-board-0.4.1/chessboard/fenparser.py
+drwxrwxrwx   0        0        0        0 2023-07-14 13:55:01.826032 chess-board-0.4.1/chessboard/images/
+-rw-rw-rw-   0        0        0      905 2022-04-10 11:32:03.000000 chess-board-0.4.1/chessboard/images/bB.png
+-rw-rw-rw-   0        0        0     1955 2022-04-10 11:32:03.000000 chess-board-0.4.1/chessboard/images/bK.png
+-rw-rw-rw-   0        0        0     1239 2022-04-10 11:32:03.000000 chess-board-0.4.1/chessboard/images/bN.png
+-rw-rw-rw-   0        0        0      561 2022-04-10 11:32:03.000000 chess-board-0.4.1/chessboard/images/bP.png
+-rw-rw-rw-   0        0        0     1797 2022-04-10 11:32:03.000000 chess-board-0.4.1/chessboard/images/bQ.png
+-rw-rw-rw-   0        0        0      652 2022-04-10 11:32:03.000000 chess-board-0.4.1/chessboard/images/bR.png
+-rw-rw-rw-   0        0        0      330 2022-04-10 11:32:03.000000 chess-board-0.4.1/chessboard/images/btile.png
+-rw-rw-rw-   0        0        0     1475 2022-04-10 11:32:03.000000 chess-board-0.4.1/chessboard/images/wB.png
+-rw-rw-rw-   0        0        0     1910 2022-04-10 11:32:03.000000 chess-board-0.4.1/chessboard/images/wK.png
+-rw-rw-rw-   0        0        0     1508 2022-04-10 11:32:03.000000 chess-board-0.4.1/chessboard/images/wN.png
+-rw-rw-rw-   0        0        0      988 2022-04-10 11:32:03.000000 chess-board-0.4.1/chessboard/images/wP.png
+-rw-rw-rw-   0        0        0     2288 2022-04-10 11:32:03.000000 chess-board-0.4.1/chessboard/images/wQ.png
+-rw-rw-rw-   0        0        0     1043 2022-04-10 11:32:03.000000 chess-board-0.4.1/chessboard/images/wR.png
+-rw-rw-rw-   0        0        0      208 2022-04-10 11:32:03.000000 chess-board-0.4.1/chessboard/images/wtile.png
+-rw-rw-rw-   0        0        0     2869 2022-07-12 13:32:23.000000 chess-board-0.4.1/chessboard/pieces.py
+-rw-rw-rw-   0        0        0       66 2022-04-10 11:32:58.000000 chess-board-0.4.1/chessboard/utils.py
+-rw-rw-rw-   0        0        0       42 2023-07-14 13:55:01.828029 chess-board-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     3823 2023-07-14 13:50:17.000000 chess-board-0.4.1/setup.py
```

### Comparing `chess-board-0.4.0/LICENSE` & `chess-board-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chess-board-0.4.0/PKG-INFO` & `chess-board-0.4.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chess-board
-Version: 0.4.0
+Version: 0.4.1
 Summary: A python chessboard library for representing game positions.
 Home-page: https://github.com/ahira-justice/chess-board
 Author: Ahira Adefokun
 Author-email: justiceahira@gmail.com
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
@@ -60,14 +60,18 @@
 
 game_board = display.start()
 
 while True:
     display.check_for_quit()
     display.update(valid_fen, game_board)
 
+    # board flip interface
+    if not game_board.flipped:
+        display.flip(game_board)
+
 ```
 
 ## Installation
 Download and install the latest release:
 ```sh
 
 # install into virtualenv
```

### Comparing `chess-board-0.4.0/README.md` & `chess-board-0.4.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -43,14 +43,18 @@
 
 game_board = display.start()
 
 while True:
     display.check_for_quit()
     display.update(valid_fen, game_board)
 
+    # board flip interface
+    if not game_board.flipped:
+        display.flip(game_board)
+
 ```
 
 ## Installation
 Download and install the latest release:
 ```sh
 
 # install into virtualenv
```

### Comparing `chess-board-0.4.0/chess_board.egg-info/PKG-INFO` & `chess-board-0.4.1/chess_board.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chess-board
-Version: 0.4.0
+Version: 0.4.1
 Summary: A python chessboard library for representing game positions.
 Home-page: https://github.com/ahira-justice/chess-board
 Author: Ahira Adefokun
 Author-email: justiceahira@gmail.com
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
@@ -60,14 +60,18 @@
 
 game_board = display.start()
 
 while True:
     display.check_for_quit()
     display.update(valid_fen, game_board)
 
+    # board flip interface
+    if not game_board.flipped:
+        display.flip(game_board)
+
 ```
 
 ## Installation
 Download and install the latest release:
 ```sh
 
 # install into virtualenv
```

### Comparing `chess-board-0.4.0/chess_board.egg-info/SOURCES.txt` & `chess-board-0.4.1/chess_board.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chess-board-0.4.0/chessboard/board.py` & `chess-board-0.4.1/chessboard/board.py`

 * *Files identical despite different names*

### Comparing `chess-board-0.4.0/chessboard/display.py` & `chess-board-0.4.1/chessboard/display.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 import os
+
+os.environ['PYGAME_HIDE_SUPPORT_PROMPT'] = '1'  # Hide pygame support message
+
 import sys
 import pygame
 
 from pygame.locals import QUIT, KEYUP, K_ESCAPE
 
 from chessboard.board import Board, Color
 from chessboard.constants import FPS, STARTING_FEN, WINDOW_CAPTION, WINDOW_WIDTH, WINDOW_HEIGHT
 
+
 os.environ['SDL_VIDEO_CENTERED'] = '1'  # Centre display window.
 
 fps_clock = pygame.time.Clock()
 
 
 def terminate():
     pygame.quit()
```

### Comparing `chess-board-0.4.0/chessboard/fenparser.py` & `chess-board-0.4.1/chessboard/fenparser.py`

 * *Files identical despite different names*

### Comparing `chess-board-0.4.0/chessboard/images/bB.png` & `chess-board-0.4.1/chessboard/images/bB.png`

 * *Files identical despite different names*

### Comparing `chess-board-0.4.0/chessboard/images/bK.png` & `chess-board-0.4.1/chessboard/images/bK.png`

 * *Files identical despite different names*

### Comparing `chess-board-0.4.0/chessboard/images/bN.png` & `chess-board-0.4.1/chessboard/images/bN.png`

 * *Files identical despite different names*

### Comparing `chess-board-0.4.0/chessboard/images/bP.png` & `chess-board-0.4.1/chessboard/images/bP.png`

 * *Files identical despite different names*

### Comparing `chess-board-0.4.0/chessboard/images/bQ.png` & `chess-board-0.4.1/chessboard/images/bQ.png`

 * *Files identical despite different names*

### Comparing `chess-board-0.4.0/chessboard/images/bR.png` & `chess-board-0.4.1/chessboard/images/bR.png`

 * *Files identical despite different names*

### Comparing `chess-board-0.4.0/chessboard/images/wB.png` & `chess-board-0.4.1/chessboard/images/wB.png`

 * *Files identical despite different names*

### Comparing `chess-board-0.4.0/chessboard/images/wK.png` & `chess-board-0.4.1/chessboard/images/wK.png`

 * *Files identical despite different names*

### Comparing `chess-board-0.4.0/chessboard/images/wN.png` & `chess-board-0.4.1/chessboard/images/wN.png`

 * *Files identical despite different names*

### Comparing `chess-board-0.4.0/chessboard/images/wP.png` & `chess-board-0.4.1/chessboard/images/wP.png`

 * *Files identical despite different names*

### Comparing `chess-board-0.4.0/chessboard/images/wQ.png` & `chess-board-0.4.1/chessboard/images/wQ.png`

 * *Files identical despite different names*

### Comparing `chess-board-0.4.0/chessboard/images/wR.png` & `chess-board-0.4.1/chessboard/images/wR.png`

 * *Files identical despite different names*

### Comparing `chess-board-0.4.0/chessboard/pieces.py` & `chess-board-0.4.1/chessboard/pieces.py`

 * *Files identical despite different names*

### Comparing `chess-board-0.4.0/setup.py` & `chess-board-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'chess-board'
 DESCRIPTION = 'A python chessboard library for representing game positions.'
 URL = 'https://github.com/ahira-justice/chess-board'
 EMAIL = 'justiceahira@gmail.com'
 AUTHOR = 'Ahira Adefokun'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.4.0'
+VERSION = '0.4.1'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'pygame'
 ]
 
 # What packages are optional?
```

