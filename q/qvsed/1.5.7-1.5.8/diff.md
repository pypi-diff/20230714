# Comparing `tmp/qvsed-1.5.7.tar.gz` & `tmp/qvsed-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qvsed-1.5.7.tar", last modified: Fri Jul 14 15:42:29 2023, max compression
+gzip compressed data, was "qvsed-1.5.8.tar", last modified: Fri Jul 14 16:25:51 2023, max compression
```

## Comparing `qvsed-1.5.7.tar` & `qvsed-1.5.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 15:42:29.032380 qvsed-1.5.7/
--rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.5.7/LICENSE.txt
--rw-rw-rw-   0        0        0       88 2023-07-13 16:48:35.000000 qvsed-1.5.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1263 2023-07-14 15:42:29.032380 qvsed-1.5.7/PKG-INFO
--rw-rw-rw-   0        0        0     7389 2023-07-14 15:41:43.000000 qvsed-1.5.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 15:42:28.977516 qvsed-1.5.7/qvsed/
--rw-rw-rw-   0        0        0       50 2023-07-08 20:05:55.000000 qvsed-1.5.7/qvsed/__init__.py
--rw-rw-rw-   0        0        0      767 2023-07-13 15:51:04.000000 qvsed-1.5.7/qvsed/config_default.py
--rw-rw-rw-   0        0        0    27722 2023-07-14 15:38:07.000000 qvsed-1.5.7/qvsed/qvsed.py
--rw-rw-rw-   0        0        0     7950 2023-07-09 10:52:35.000000 qvsed-1.5.7/qvsed/qvsed.ui
--rw-rw-rw-   0        0        0     5043 2023-07-14 15:38:03.000000 qvsed-1.5.7/qvsed/qvsed_dialog.ui
-drwxrwxrwx   0        0        0        0 2023-07-14 15:42:29.029379 qvsed-1.5.7/qvsed.egg-info/
--rw-rw-rw-   0        0        0     1263 2023-07-14 15:42:28.000000 qvsed-1.5.7/qvsed.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-07-14 15:42:28.000000 qvsed-1.5.7/qvsed.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 15:42:28.000000 qvsed-1.5.7/qvsed.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-14 15:42:28.000000 qvsed-1.5.7/qvsed.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-07-14 15:42:28.000000 qvsed-1.5.7/qvsed.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-14 15:42:28.000000 qvsed-1.5.7/qvsed.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 15:42:29.035678 qvsed-1.5.7/setup.cfg
--rw-rw-rw-   0        0        0     1652 2023-07-14 15:38:41.000000 qvsed-1.5.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 16:25:51.081826 qvsed-1.5.8/
+-rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.5.8/LICENSE.txt
+-rw-rw-rw-   0        0        0       88 2023-07-13 16:48:35.000000 qvsed-1.5.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1263 2023-07-14 16:25:51.081826 qvsed-1.5.8/PKG-INFO
+-rw-rw-rw-   0        0        0     7389 2023-07-14 15:41:43.000000 qvsed-1.5.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 16:25:51.060540 qvsed-1.5.8/qvsed/
+-rw-rw-rw-   0        0        0       50 2023-07-08 20:05:55.000000 qvsed-1.5.8/qvsed/__init__.py
+-rw-rw-rw-   0        0        0      787 2023-07-14 16:23:39.000000 qvsed-1.5.8/qvsed/config_default.py
+-rw-rw-rw-   0        0        0    28049 2023-07-14 16:14:05.000000 qvsed-1.5.8/qvsed/qvsed.py
+-rw-rw-rw-   0        0        0     7950 2023-07-09 10:52:35.000000 qvsed-1.5.8/qvsed/qvsed.ui
+-rw-rw-rw-   0        0        0     5043 2023-07-14 15:38:03.000000 qvsed-1.5.8/qvsed/qvsed_dialog.ui
+drwxrwxrwx   0        0        0        0 2023-07-14 16:25:51.079439 qvsed-1.5.8/qvsed.egg-info/
+-rw-rw-rw-   0        0        0     1263 2023-07-14 16:25:50.000000 qvsed-1.5.8/qvsed.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-07-14 16:25:50.000000 qvsed-1.5.8/qvsed.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 16:25:50.000000 qvsed-1.5.8/qvsed.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-14 16:25:50.000000 qvsed-1.5.8/qvsed.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-07-14 16:25:50.000000 qvsed-1.5.8/qvsed.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-14 16:25:50.000000 qvsed-1.5.8/qvsed.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 16:25:51.081826 qvsed-1.5.8/setup.cfg
+-rw-rw-rw-   0        0        0     1652 2023-07-14 16:25:39.000000 qvsed-1.5.8/setup.py
```

### Comparing `qvsed-1.5.7/LICENSE.txt` & `qvsed-1.5.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qvsed-1.5.7/PKG-INFO` & `qvsed-1.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.5.7
+Version: 1.5.8
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.5.7/README.md` & `qvsed-1.5.8/README.md`

 * *Files identical despite different names*

### Comparing `qvsed-1.5.7/qvsed/config_default.py` & `qvsed-1.5.8/qvsed/config_default.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # pylint: disable=all
 
 # Font
 font_family = ["JetBrains Mono", "Cascadia Code", "Consolas", "Menlo", "monospace"]
 font_size = 11
 
 # Options
+tab_stop_width = 4
 echo_area_timeout = 3000
 
 # Colours
 text_color = "#FFFFFF"
 background_color = "#282C34"
 
 button_text_color = "#FFFFFF"
```

### Comparing `qvsed-1.5.7/qvsed/qvsed.py` & `qvsed-1.5.8/qvsed/qvsed.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pkg_resources
 from PyQt5.QtWidgets import (
     QApplication, QMainWindow, QWidget, QFileDialog,
     QAction, QShortcut, QDialog
 )
 from PyQt5.QtGui import (
     QKeySequence, QFont, QDragEnterEvent, QDropEvent,
-    QTextCursor
+    QTextCursor, QFontMetricsF
 )
 from PyQt5.QtCore import (
     Qt, QTextCodec, QEvent, QObject, QTimer
 )
 from PyQt5.uic import loadUi
 
 
@@ -322,14 +322,15 @@
 
         spec = importlib.util.spec_from_file_location("qvsed_config", user_config_file)
         qvsed_config = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(qvsed_config)
 
         self.font_family = qvsed_config.font_family
         self.font_size = qvsed_config.font_size
+        self.tab_stop_width = getattr(qvsed_config, 'tab_stop_width', 4)
 
         self.echo_area_timeout = getattr(qvsed_config, 'echo_area_timeout', 3000)
 
         # Load the colour scheme settings from the config file
         # We use the shorter American spellings because it's standard, I guess
         text_color = getattr(qvsed_config, 'text_color', None)
         background_color = getattr(qvsed_config, 'background_color', None)
@@ -511,25 +512,33 @@
         text_area.dragMoveEvent = self.drag_enter_event
         text_area.dropEvent = self.drop_event
 
     def set_up_fonts(self):
         """
         Set up the fonts for the QVSED window.
         """
-        text_area = self.textArea
         font = QFont()
         font.setFamilies(self.font_family)
         if sys.platform == "darwin":
             # macOS fonts should be bigger
             self.font_size += 4
         font.setPointSize(self.font_size)
-        text_area.setTabStopWidth(4 * text_area.fontMetrics().width(' '))
         QApplication.instance().setFont(font)
+        self.set_tab_stop_width()
         self.update_widget_fonts(self)
 
+    def set_tab_stop_width(self):
+        """
+        Set the tab stop width for the Text Area.
+        """
+        font = self.textArea.font()
+        font_metrics = QFontMetricsF(font)
+        space_width = font_metrics.horizontalAdvance(' ')
+        self.textArea.setTabStopDistance(space_width * 4)
+
     def set_up_shortcuts(self):
         """
         Set up the key bindings for QVSED.
         """
         # Action Deck
         self.clear_shortcut = QShortcut(QKeySequence("Ctrl+N"), self)
         self.save_shortcut = QShortcut(QKeySequence("Ctrl+S"), self)
```

### Comparing `qvsed-1.5.7/qvsed/qvsed.ui` & `qvsed-1.5.8/qvsed/qvsed.ui`

 * *Files identical despite different names*

### Comparing `qvsed-1.5.7/qvsed/qvsed_dialog.ui` & `qvsed-1.5.8/qvsed/qvsed_dialog.ui`

 * *Files identical despite different names*

### Comparing `qvsed-1.5.7/qvsed.egg-info/PKG-INFO` & `qvsed-1.5.8/qvsed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.5.7
+Version: 1.5.8
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.5.7/setup.py` & `qvsed-1.5.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 The setup.py file for QVSED.
 """
 from setuptools import setup, find_packages
 
 setup(
     name='qvsed',
-    version='1.5.7',
+    version='1.5.8',
     author='Arsalan Kazmi',
     description='Qt-Based Volatile Small Editor',
     long_description="""QVSED is a volatile and small text editor.
 
 "Volatile" means that QVSED is entirely stateless - once you open a file, QVSED doesn't store any file paths or any other data other than the text contents of the file you loaded.
 Additionally, QVSED won't prompt you if you're about to potentially lose an unsaved file, since it doesn't know of any file metadata.
 You may be prompted if you're about to overwrite a file, but that's up to your OS, not QVSED.
```

