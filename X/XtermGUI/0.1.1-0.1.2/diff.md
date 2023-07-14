# Comparing `tmp/XtermGUI-0.1.1.tar.gz` & `tmp/XtermGUI-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "XtermGUI-0.1.1.tar", last modified: Fri Jul 14 16:26:00 2023, max compression
+gzip compressed data, was "XtermGUI-0.1.2.tar", last modified: Fri Jul 14 18:17:05 2023, max compression
```

## Comparing `XtermGUI-0.1.1.tar` & `XtermGUI-0.1.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:26:00.644476 XtermGUI-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-14 16:25:45.000000 XtermGUI-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    58115 2023-07-14 16:26:00.640476 XtermGUI-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16704 2023-07-14 16:25:45.000000 XtermGUI-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:26:00.632475 XtermGUI-0.1.1/XtermGUI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    58115 2023-07-14 16:26:00.000000 XtermGUI-0.1.1/XtermGUI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-14 16:26:00.000000 XtermGUI-0.1.1/XtermGUI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:26:00.000000 XtermGUI-0.1.1/XtermGUI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 16:26:00.000000 XtermGUI-0.1.1/XtermGUI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-14 16:25:45.000000 XtermGUI-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 16:26:00.644476 XtermGUI-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:26:00.632475 XtermGUI-0.1.1/xtermgui/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-14 16:25:45.000000 XtermGUI-0.1.1/xtermgui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:26:00.636475 XtermGUI-0.1.1/xtermgui/control/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-14 16:25:45.000000 XtermGUI-0.1.1/xtermgui/control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-07-14 16:25:45.000000 XtermGUI-0.1.1/xtermgui/control/colour.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-14 16:25:45.000000 XtermGUI-0.1.1/xtermgui/control/colours.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-07-14 16:25:45.000000 XtermGUI-0.1.1/xtermgui/control/cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-14 16:25:45.000000 XtermGUI-0.1.1/xtermgui/control/rgb.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-14 16:25:45.000000 XtermGUI-0.1.1/xtermgui/control/rgbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-14 16:25:45.000000 XtermGUI-0.1.1/xtermgui/control/style.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-14 16:25:45.000000 XtermGUI-0.1.1/xtermgui/control/styles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-14 16:25:45.000000 XtermGUI-0.1.1/xtermgui/control/text.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-14 16:25:45.000000 XtermGUI-0.1.1/xtermgui/control/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:26:00.636475 XtermGUI-0.1.1/xtermgui/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-14 16:25:45.000000 XtermGUI-0.1.1/xtermgui/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-14 16:25:45.000000 XtermGUI-0.1.1/xtermgui/geometry/coordinate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-14 16:25:45.000000 XtermGUI-0.1.1/xtermgui/geometry/region.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:26:00.640476 XtermGUI-0.1.1/xtermgui/gui/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-14 16:25:45.000000 XtermGUI-0.1.1/xtermgui/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-14 16:25:45.000000 XtermGUI-0.1.1/xtermgui/gui/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-14 16:25:45.000000 XtermGUI-0.1.1/xtermgui/gui/keyboard_interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-14 16:25:45.000000 XtermGUI-0.1.1/xtermgui/gui/mouse_interaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:26:00.640476 XtermGUI-0.1.1/xtermgui/input/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-14 16:25:45.000000 XtermGUI-0.1.1/xtermgui/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-14 16:25:45.000000 XtermGUI-0.1.1/xtermgui/input/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-07-14 16:25:45.000000 XtermGUI-0.1.1/xtermgui/input/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-14 16:25:45.000000 XtermGUI-0.1.1/xtermgui/input/input.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-14 16:25:45.000000 XtermGUI-0.1.1/xtermgui/input/keyboard_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-14 16:25:45.000000 XtermGUI-0.1.1/xtermgui/input/keyboard_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-14 16:25:45.000000 XtermGUI-0.1.1/xtermgui/input/mouse_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-14 16:25:45.000000 XtermGUI-0.1.1/xtermgui/input/mouse_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-14 16:25:45.000000 XtermGUI-0.1.1/xtermgui/input/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:26:00.640476 XtermGUI-0.1.1/xtermgui/layered_gui/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-14 16:25:45.000000 XtermGUI-0.1.1/xtermgui/layered_gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-07-14 16:25:45.000000 XtermGUI-0.1.1/xtermgui/layered_gui/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-14 16:25:45.000000 XtermGUI-0.1.1/xtermgui/layered_gui/layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:17:05.433780 XtermGUI-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-14 18:16:48.000000 XtermGUI-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    58113 2023-07-14 18:17:05.433780 XtermGUI-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16704 2023-07-14 18:16:48.000000 XtermGUI-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:17:05.429780 XtermGUI-0.1.2/XtermGUI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    58113 2023-07-14 18:17:05.000000 XtermGUI-0.1.2/XtermGUI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-14 18:17:05.000000 XtermGUI-0.1.2/XtermGUI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 18:17:05.000000 XtermGUI-0.1.2/XtermGUI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 18:17:05.000000 XtermGUI-0.1.2/XtermGUI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-14 18:16:48.000000 XtermGUI-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 18:17:05.433780 XtermGUI-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:17:05.429780 XtermGUI-0.1.2/xtermgui/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-14 18:16:48.000000 XtermGUI-0.1.2/xtermgui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:17:05.429780 XtermGUI-0.1.2/xtermgui/control/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-14 18:16:48.000000 XtermGUI-0.1.2/xtermgui/control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-07-14 18:16:48.000000 XtermGUI-0.1.2/xtermgui/control/colour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-14 18:16:48.000000 XtermGUI-0.1.2/xtermgui/control/colours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-07-14 18:16:48.000000 XtermGUI-0.1.2/xtermgui/control/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-14 18:16:48.000000 XtermGUI-0.1.2/xtermgui/control/rgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-14 18:16:48.000000 XtermGUI-0.1.2/xtermgui/control/rgbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-14 18:16:48.000000 XtermGUI-0.1.2/xtermgui/control/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-14 18:16:48.000000 XtermGUI-0.1.2/xtermgui/control/styles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-14 18:16:48.000000 XtermGUI-0.1.2/xtermgui/control/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-14 18:16:48.000000 XtermGUI-0.1.2/xtermgui/control/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:17:05.429780 XtermGUI-0.1.2/xtermgui/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-14 18:16:48.000000 XtermGUI-0.1.2/xtermgui/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-14 18:16:48.000000 XtermGUI-0.1.2/xtermgui/geometry/coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-14 18:16:48.000000 XtermGUI-0.1.2/xtermgui/geometry/region.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:17:05.433780 XtermGUI-0.1.2/xtermgui/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-14 18:16:48.000000 XtermGUI-0.1.2/xtermgui/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-14 18:16:48.000000 XtermGUI-0.1.2/xtermgui/gui/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-14 18:16:48.000000 XtermGUI-0.1.2/xtermgui/gui/keyboard_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-14 18:16:48.000000 XtermGUI-0.1.2/xtermgui/gui/mouse_interaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:17:05.433780 XtermGUI-0.1.2/xtermgui/input/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-14 18:16:48.000000 XtermGUI-0.1.2/xtermgui/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-14 18:16:48.000000 XtermGUI-0.1.2/xtermgui/input/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-07-14 18:16:48.000000 XtermGUI-0.1.2/xtermgui/input/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-14 18:16:48.000000 XtermGUI-0.1.2/xtermgui/input/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-14 18:16:48.000000 XtermGUI-0.1.2/xtermgui/input/keyboard_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-14 18:16:48.000000 XtermGUI-0.1.2/xtermgui/input/keyboard_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-14 18:16:48.000000 XtermGUI-0.1.2/xtermgui/input/mouse_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-14 18:16:48.000000 XtermGUI-0.1.2/xtermgui/input/mouse_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-14 18:16:48.000000 XtermGUI-0.1.2/xtermgui/input/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:17:05.433780 XtermGUI-0.1.2/xtermgui/layered_gui/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-14 18:16:48.000000 XtermGUI-0.1.2/xtermgui/layered_gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-07-14 18:16:48.000000 XtermGUI-0.1.2/xtermgui/layered_gui/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-14 18:16:48.000000 XtermGUI-0.1.2/xtermgui/layered_gui/layer.py
```

### Comparing `XtermGUI-0.1.1/LICENSE` & `XtermGUI-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `XtermGUI-0.1.1/PKG-INFO` & `XtermGUI-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XtermGUI
-Version: 0.1.1
+Version: 0.1.2
 Summary: A lightweight, expressive GUI framework for compatible terminals
 Author-email: Kieran Lock <kieran.lock@outlook.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -682,17 +682,17 @@
 Project-URL: Documentation, https://github.com/Kieran-Lock/XtermGUI/blob/main/DOCUMENTATION.md
 Project-URL: License, https://github.com/Kieran-Lock/XtermGUI/blob/main/LICENSE
 Keywords: gui,framework,xterm,zero-dependency,terminal-based
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Intended Audience :: Developers
-Requires-Python: >=3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="readme-top"></a>
```

### Comparing `XtermGUI-0.1.1/README.md` & `XtermGUI-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `XtermGUI-0.1.1/XtermGUI.egg-info/PKG-INFO` & `XtermGUI-0.1.2/XtermGUI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XtermGUI
-Version: 0.1.1
+Version: 0.1.2
 Summary: A lightweight, expressive GUI framework for compatible terminals
 Author-email: Kieran Lock <kieran.lock@outlook.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -682,17 +682,17 @@
 Project-URL: Documentation, https://github.com/Kieran-Lock/XtermGUI/blob/main/DOCUMENTATION.md
 Project-URL: License, https://github.com/Kieran-Lock/XtermGUI/blob/main/LICENSE
 Keywords: gui,framework,xterm,zero-dependency,terminal-based
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Intended Audience :: Developers
-Requires-Python: >=3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="readme-top"></a>
```

### Comparing `XtermGUI-0.1.1/XtermGUI.egg-info/SOURCES.txt` & `XtermGUI-0.1.2/XtermGUI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `XtermGUI-0.1.1/pyproject.toml` & `XtermGUI-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [project]
 name = "XtermGUI"
 description = "A lightweight, expressive GUI framework for compatible terminals"
 readme = "README.md"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
     { name = "Kieran Lock", email = "kieran.lock@outlook.com" }
 ]
 keywords = ["gui", "framework", "xterm", "zero-dependency", "terminal-based"]
 classifiers = [
     "Development Status :: 3 - Alpha", 
     "Environment :: Console", 
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)", 
     "Operating System :: POSIX :: Linux", 
-    "Programming Language :: Python :: 3.11", 
+    "Programming Language :: Python :: 3.8", 
     "Intended Audience :: Developers"
 ]
-requires-python = ">=3.11"
+requires-python = ">=3.8"
 license = {file = "LICENSE"}
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project.urls]
```

### Comparing `XtermGUI-0.1.1/xtermgui/control/colour.py` & `XtermGUI-0.1.2/xtermgui/control/colour.py`

 * *Files identical despite different names*

### Comparing `XtermGUI-0.1.1/xtermgui/control/colours.py` & `XtermGUI-0.1.2/xtermgui/control/colours.py`

 * *Files identical despite different names*

### Comparing `XtermGUI-0.1.1/xtermgui/control/cursor.py` & `XtermGUI-0.1.2/xtermgui/control/cursor.py`

 * *Files identical despite different names*

### Comparing `XtermGUI-0.1.1/xtermgui/control/rgb.py` & `XtermGUI-0.1.2/xtermgui/control/rgb.py`

 * *Files identical despite different names*

### Comparing `XtermGUI-0.1.1/xtermgui/control/rgbs.py` & `XtermGUI-0.1.2/xtermgui/control/rgbs.py`

 * *Files identical despite different names*

### Comparing `XtermGUI-0.1.1/xtermgui/control/style.py` & `XtermGUI-0.1.2/xtermgui/control/style.py`

 * *Files identical despite different names*

### Comparing `XtermGUI-0.1.1/xtermgui/control/text.py` & `XtermGUI-0.1.2/xtermgui/control/text.py`

 * *Files identical despite different names*

### Comparing `XtermGUI-0.1.1/xtermgui/geometry/coordinate.py` & `XtermGUI-0.1.2/xtermgui/geometry/coordinate.py`

 * *Files identical despite different names*

### Comparing `XtermGUI-0.1.1/xtermgui/geometry/region.py` & `XtermGUI-0.1.2/xtermgui/geometry/region.py`

 * *Files identical despite different names*

### Comparing `XtermGUI-0.1.1/xtermgui/gui/gui.py` & `XtermGUI-0.1.2/xtermgui/gui/gui.py`

 * *Files identical despite different names*

### Comparing `XtermGUI-0.1.1/xtermgui/gui/keyboard_interaction.py` & `XtermGUI-0.1.2/xtermgui/gui/keyboard_interaction.py`

 * *Files identical despite different names*

### Comparing `XtermGUI-0.1.1/xtermgui/gui/mouse_interaction.py` & `XtermGUI-0.1.2/xtermgui/gui/mouse_interaction.py`

 * *Files identical despite different names*

### Comparing `XtermGUI-0.1.1/xtermgui/input/event.py` & `XtermGUI-0.1.2/xtermgui/input/event.py`

 * *Files identical despite different names*

### Comparing `XtermGUI-0.1.1/xtermgui/input/events.py` & `XtermGUI-0.1.2/xtermgui/input/events.py`

 * *Files identical despite different names*

### Comparing `XtermGUI-0.1.1/xtermgui/input/input.py` & `XtermGUI-0.1.2/xtermgui/input/input.py`

 * *Files identical despite different names*

### Comparing `XtermGUI-0.1.1/xtermgui/input/keyboard_codes.py` & `XtermGUI-0.1.2/xtermgui/input/keyboard_codes.py`

 * *Files identical despite different names*

### Comparing `XtermGUI-0.1.1/xtermgui/input/setup.py` & `XtermGUI-0.1.2/xtermgui/input/setup.py`

 * *Files identical despite different names*

### Comparing `XtermGUI-0.1.1/xtermgui/layered_gui/gui.py` & `XtermGUI-0.1.2/xtermgui/layered_gui/gui.py`

 * *Files identical despite different names*

### Comparing `XtermGUI-0.1.1/xtermgui/layered_gui/layer.py` & `XtermGUI-0.1.2/xtermgui/layered_gui/layer.py`

 * *Files identical despite different names*

