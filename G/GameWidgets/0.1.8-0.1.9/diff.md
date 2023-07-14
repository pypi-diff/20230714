# Comparing `tmp/GameWidgets-0.1.8.tar.gz` & `tmp/GameWidgets-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GameWidgets-0.1.8.tar", last modified: Sat Jul  8 21:18:25 2023, max compression
+gzip compressed data, was "GameWidgets-0.1.9.tar", last modified: Fri Jul 14 00:38:17 2023, max compression
```

## Comparing `GameWidgets-0.1.8.tar` & `GameWidgets-0.1.9.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-08 21:18:25.028021 GameWidgets-0.1.8/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-08 21:18:25.016021 GameWidgets-0.1.8/GameWidgets/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-08 21:18:25.016021 GameWidgets-0.1.8/GameWidgets/Assets/
--rw-------   0 runner    (1000) runner    (1000)        0 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/Assets/__init__.py
--rw-------   0 runner    (1000) runner    (1000)     5844 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/Constants.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-08 21:18:25.016021 GameWidgets-0.1.8/GameWidgets/Engine/
--rw-------   0 runner    (1000) runner    (1000)     1011 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/Engine/Backdrop.py
--rw-------   0 runner    (1000) runner    (1000)      602 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/Engine/Entity.py
--rw-------   0 runner    (1000) runner    (1000)     1041 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/Engine/Group.py
--rw-------   0 runner    (1000) runner    (1000)      122 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/Engine/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-08 21:18:25.016021 GameWidgets-0.1.8/GameWidgets/Examples/
--rw-------   0 runner    (1000) runner    (1000)     1758 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/Examples/Widget_Screen_GameWidgets_Example.py
--rw-------   0 runner    (1000) runner    (1000)        4 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/Examples/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-08 21:18:25.020021 GameWidgets-0.1.8/GameWidgets/GameWidgets/
--rw-------   0 runner    (1000) runner    (1000)     1422 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/GameWidgets/Animatrix.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-08 21:18:25.020021 GameWidgets-0.1.8/GameWidgets/GameWidgets/Controller/
--rw-------   0 runner    (1000) runner    (1000)     1497 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/GameWidgets/Controller/Button.py
--rw-------   0 runner    (1000) runner    (1000)     1404 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/GameWidgets/Controller/Joystick.py
--rw-------   0 runner    (1000) runner    (1000)       13 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/GameWidgets/Controller/R1_R2.py
--rw-------   0 runner    (1000) runner    (1000)      148 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/GameWidgets/Controller/__init__.py
--rw-------   0 runner    (1000) runner    (1000)      735 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/GameWidgets/Draw.py
--rw-------   0 runner    (1000) runner    (1000)      652 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/GameWidgets/ScreenSlide.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-08 21:18:25.020021 GameWidgets-0.1.8/GameWidgets/GameWidgets/TileMaps/
--rw-------   0 runner    (1000) runner    (1000)      424 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/GameWidgets/TileMaps/Sprite.py
--rw-------   0 runner    (1000) runner    (1000)      703 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/GameWidgets/TileMaps/Tile.py
--rw-------   0 runner    (1000) runner    (1000)      124 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/GameWidgets/TileMaps/__init__.py
--rw-------   0 runner    (1000) runner    (1000)      121 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/GameWidgets/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-08 21:18:25.024021 GameWidgets-0.1.8/GameWidgets/RuntimeTests/
--rw-------   0 runner    (1000) runner    (1000)      649 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/RuntimeTests/AllTest.py
--rw-------   0 runner    (1000) runner    (1000)      397 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/RuntimeTests/GameWidgetTest.py
--rw-------   0 runner    (1000) runner    (1000)      359 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/RuntimeTests/SetUpTest.py
--rw-------   0 runner    (1000) runner    (1000)      369 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/RuntimeTests/WidgetTest.py
--rw-------   0 runner    (1000) runner    (1000)        4 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/RuntimeTests/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-08 21:18:25.024021 GameWidgets-0.1.8/GameWidgets/SetUp/
--rw-------   0 runner    (1000) runner    (1000)     1689 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/SetUp/ScreenCommands.py
--rw-------   0 runner    (1000) runner    (1000)      109 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/SetUp/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-08 21:18:25.028021 GameWidgets-0.1.8/GameWidgets/Widgets/
--rw-------   0 runner    (1000) runner    (1000)     3691 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/Widgets/Btn.py
--rw-------   0 runner    (1000) runner    (1000)      597 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/Widgets/Clock.py
--rw-------   0 runner    (1000) runner    (1000)     1489 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/Widgets/Cursor.py
--rw-------   0 runner    (1000) runner    (1000)     2761 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/Widgets/DialogeBox.py
--rw-------   0 runner    (1000) runner    (1000)     1574 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/Widgets/ImgDecoder.py
--rw-------   0 runner    (1000) runner    (1000)      246 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/Widgets/Sound.py
--rw-------   0 runner    (1000) runner    (1000)     1876 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/Widgets/TextInp.py
--rw-------   0 runner    (1000) runner    (1000)     2807 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/Widgets/ToggleBtn.py
--rw-------   0 runner    (1000) runner    (1000)      191 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/Widgets/__init__.py
--rw-------   0 runner    (1000) runner    (1000)      654 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/__init__.py
--rw-------   0 runner    (1000) runner    (1000)      567 2023-07-08 21:17:33.000000 GameWidgets-0.1.8/GameWidgets/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-08 21:18:25.016021 GameWidgets-0.1.8/GameWidgets.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1325 2023-07-08 21:18:24.000000 GameWidgets-0.1.8/GameWidgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     1493 2023-07-08 21:18:24.000000 GameWidgets-0.1.8/GameWidgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-08 21:18:24.000000 GameWidgets-0.1.8/GameWidgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        7 2023-07-08 21:18:24.000000 GameWidgets-0.1.8/GameWidgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-07-08 21:18:24.000000 GameWidgets-0.1.8/GameWidgets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     1325 2023-07-08 21:18:25.028021 GameWidgets-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      385 2022-09-11 21:19:38.000000 GameWidgets-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-08 21:18:25.028021 GameWidgets-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-14 00:38:17.433046 GameWidgets-0.1.9/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-14 00:38:17.421047 GameWidgets-0.1.9/GameWidgets/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-14 00:38:17.421047 GameWidgets-0.1.9/GameWidgets/Assets/
+-rw-------   0 runner    (1000) runner    (1000)        0 2023-07-14 00:37:56.000000 GameWidgets-0.1.9/GameWidgets/Assets/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)     5845 2023-07-14 00:37:56.000000 GameWidgets-0.1.9/GameWidgets/Constants.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-14 00:38:17.425047 GameWidgets-0.1.9/GameWidgets/Engine/
+-rw-------   0 runner    (1000) runner    (1000)     1011 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/Engine/Backdrop.py
+-rw-------   0 runner    (1000) runner    (1000)     1211 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/Engine/Entity.py
+-rw-------   0 runner    (1000) runner    (1000)     1607 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/Engine/Group.py
+-rw-------   0 runner    (1000) runner    (1000)     1082 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/Engine/Manager.py
+-rw-------   0 runner    (1000) runner    (1000)      164 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/Engine/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-14 00:38:17.425047 GameWidgets-0.1.9/GameWidgets/Examples/
+-rw-------   0 runner    (1000) runner    (1000)     1758 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/Examples/Widget_Screen_GameWidgets_Example.py
+-rw-------   0 runner    (1000) runner    (1000)        4 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/Examples/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-14 00:38:17.425047 GameWidgets-0.1.9/GameWidgets/GameWidgets/
+-rw-------   0 runner    (1000) runner    (1000)     1422 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/GameWidgets/Animatrix.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-14 00:38:17.425047 GameWidgets-0.1.9/GameWidgets/GameWidgets/Controller/
+-rw-------   0 runner    (1000) runner    (1000)     1497 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/GameWidgets/Controller/Button.py
+-rw-------   0 runner    (1000) runner    (1000)     1404 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/GameWidgets/Controller/Joystick.py
+-rw-------   0 runner    (1000) runner    (1000)       13 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/GameWidgets/Controller/R1_R2.py
+-rw-------   0 runner    (1000) runner    (1000)      148 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/GameWidgets/Controller/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)      735 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/GameWidgets/Draw.py
+-rw-------   0 runner    (1000) runner    (1000)      652 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/GameWidgets/ScreenSlide.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-14 00:38:17.425047 GameWidgets-0.1.9/GameWidgets/GameWidgets/TileMaps/
+-rw-------   0 runner    (1000) runner    (1000)      424 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/GameWidgets/TileMaps/Sprite.py
+-rw-------   0 runner    (1000) runner    (1000)      703 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/GameWidgets/TileMaps/Tile.py
+-rw-------   0 runner    (1000) runner    (1000)      124 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/GameWidgets/TileMaps/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)      121 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/GameWidgets/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-14 00:38:17.429046 GameWidgets-0.1.9/GameWidgets/RuntimeTests/
+-rw-------   0 runner    (1000) runner    (1000)      649 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/RuntimeTests/AllTest.py
+-rw-------   0 runner    (1000) runner    (1000)      397 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/RuntimeTests/GameWidgetTest.py
+-rw-------   0 runner    (1000) runner    (1000)      359 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/RuntimeTests/SetUpTest.py
+-rw-------   0 runner    (1000) runner    (1000)      369 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/RuntimeTests/WidgetTest.py
+-rw-------   0 runner    (1000) runner    (1000)        4 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/RuntimeTests/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-14 00:38:17.429046 GameWidgets-0.1.9/GameWidgets/SetUp/
+-rw-------   0 runner    (1000) runner    (1000)     1689 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/SetUp/ScreenCommands.py
+-rw-------   0 runner    (1000) runner    (1000)      109 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/SetUp/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-14 00:38:17.433046 GameWidgets-0.1.9/GameWidgets/Widgets/
+-rw-------   0 runner    (1000) runner    (1000)     3691 2023-07-14 00:37:56.000000 GameWidgets-0.1.9/GameWidgets/Widgets/Btn.py
+-rw-------   0 runner    (1000) runner    (1000)      597 2023-07-14 00:37:56.000000 GameWidgets-0.1.9/GameWidgets/Widgets/Clock.py
+-rw-------   0 runner    (1000) runner    (1000)     1489 2023-07-14 00:37:56.000000 GameWidgets-0.1.9/GameWidgets/Widgets/Cursor.py
+-rw-------   0 runner    (1000) runner    (1000)     2761 2023-07-14 00:37:56.000000 GameWidgets-0.1.9/GameWidgets/Widgets/DialogeBox.py
+-rw-------   0 runner    (1000) runner    (1000)     1574 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/Widgets/ImgDecoder.py
+-rw-------   0 runner    (1000) runner    (1000)      246 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/Widgets/Sound.py
+-rw-------   0 runner    (1000) runner    (1000)     1876 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/Widgets/TextInp.py
+-rw-------   0 runner    (1000) runner    (1000)     2807 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/Widgets/ToggleBtn.py
+-rw-------   0 runner    (1000) runner    (1000)      201 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/Widgets/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)      116 2023-07-14 00:37:56.000000 GameWidgets-0.1.9/GameWidgets/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)      567 2023-07-14 00:37:56.000000 GameWidgets-0.1.9/GameWidgets/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-14 00:38:17.421047 GameWidgets-0.1.9/GameWidgets.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1823 2023-07-14 00:38:17.000000 GameWidgets-0.1.9/GameWidgets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     1523 2023-07-14 00:38:17.000000 GameWidgets-0.1.9/GameWidgets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-14 00:38:17.000000 GameWidgets-0.1.9/GameWidgets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        7 2023-07-14 00:38:17.000000 GameWidgets-0.1.9/GameWidgets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-07-14 00:38:17.000000 GameWidgets-0.1.9/GameWidgets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     1823 2023-07-14 00:38:17.433046 GameWidgets-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      385 2022-09-11 21:19:38.000000 GameWidgets-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-14 00:38:17.433046 GameWidgets-0.1.9/setup.cfg
```

### Comparing `GameWidgets-0.1.8/GameWidgets/Constants.py` & `GameWidgets-0.1.9/GameWidgets/Constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,7 +176,8 @@
         return (s[0] / 4, y)
     elif align[1] == "Center":
         return (s[0] / 2, y)
     elif align[1] == "Right":
         return (s[0] / 4 * 3, y)
     elif align[1] == "RightMost":
         return (s[0], y)
+
```

### Comparing `GameWidgets-0.1.8/GameWidgets/Engine/Backdrop.py` & `GameWidgets-0.1.9/GameWidgets/Engine/Backdrop.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.8/GameWidgets/Examples/Widget_Screen_GameWidgets_Example.py` & `GameWidgets-0.1.9/GameWidgets/Examples/Widget_Screen_GameWidgets_Example.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.8/GameWidgets/GameWidgets/Animatrix.py` & `GameWidgets-0.1.9/GameWidgets/GameWidgets/Animatrix.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.8/GameWidgets/GameWidgets/Controller/Button.py` & `GameWidgets-0.1.9/GameWidgets/GameWidgets/Controller/Button.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.8/GameWidgets/GameWidgets/Controller/Joystick.py` & `GameWidgets-0.1.9/GameWidgets/GameWidgets/Controller/Joystick.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.8/GameWidgets/GameWidgets/Draw.py` & `GameWidgets-0.1.9/GameWidgets/GameWidgets/Draw.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.8/GameWidgets/GameWidgets/ScreenSlide.py` & `GameWidgets-0.1.9/GameWidgets/GameWidgets/ScreenSlide.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.8/GameWidgets/GameWidgets/TileMaps/Tile.py` & `GameWidgets-0.1.9/GameWidgets/GameWidgets/TileMaps/Tile.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.8/GameWidgets/RuntimeTests/AllTest.py` & `GameWidgets-0.1.9/GameWidgets/RuntimeTests/AllTest.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.8/GameWidgets/SetUp/ScreenCommands.py` & `GameWidgets-0.1.9/GameWidgets/SetUp/ScreenCommands.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.8/GameWidgets/Widgets/Btn.py` & `GameWidgets-0.1.9/GameWidgets/Widgets/Btn.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.8/GameWidgets/Widgets/Clock.py` & `GameWidgets-0.1.9/GameWidgets/Widgets/Clock.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.8/GameWidgets/Widgets/Cursor.py` & `GameWidgets-0.1.9/GameWidgets/Widgets/Cursor.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.8/GameWidgets/Widgets/DialogeBox.py` & `GameWidgets-0.1.9/GameWidgets/Widgets/DialogeBox.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.8/GameWidgets/Widgets/ImgDecoder.py` & `GameWidgets-0.1.9/GameWidgets/Widgets/ImgDecoder.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.8/GameWidgets/Widgets/TextInp.py` & `GameWidgets-0.1.9/GameWidgets/Widgets/TextInp.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.8/GameWidgets/Widgets/ToggleBtn.py` & `GameWidgets-0.1.9/GameWidgets/Widgets/ToggleBtn.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.8/GameWidgets/setup.py` & `GameWidgets-0.1.9/GameWidgets/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
   
 with open("GameWidgets/README.md", "r") as fh:
     description = fh.read()
   
 setup(
     name="GameWidgets",
-    version="0.1.8",
+    version="0.1.9",
     author="Manomay tyagi",
     author_email="tyagimanomay57@gmail.com",
     description="Make Game Easier with pygame and GameWidgets",
     long_description=description,
     long_description_content_type="text/markdown",
     url="https://github.com/SuperGuy123456/GameWidgets",
     license='MIT',
```

### Comparing `GameWidgets-0.1.8/GameWidgets.egg-info/SOURCES.txt` & `GameWidgets-0.1.9/GameWidgets.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 GameWidgets.egg-info/dependency_links.txt
 GameWidgets.egg-info/requires.txt
 GameWidgets.egg-info/top_level.txt
 GameWidgets/Assets/__init__.py
 GameWidgets/Engine/Backdrop.py
 GameWidgets/Engine/Entity.py
 GameWidgets/Engine/Group.py
+GameWidgets/Engine/Manager.py
 GameWidgets/Engine/__init__.py
 GameWidgets/Examples/Widget_Screen_GameWidgets_Example.py
 GameWidgets/Examples/__init__.py
 GameWidgets/GameWidgets/Animatrix.py
 GameWidgets/GameWidgets/Draw.py
 GameWidgets/GameWidgets/ScreenSlide.py
 GameWidgets/GameWidgets/__init__.py
```

