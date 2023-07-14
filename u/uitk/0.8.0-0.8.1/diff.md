# Comparing `tmp/uitk-0.8.0.tar.gz` & `tmp/uitk-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uitk-0.8.0.tar", last modified: Mon Jul 10 17:27:54 2023, max compression
+gzip compressed data, was "uitk-0.8.1.tar", last modified: Fri Jul 14 17:30:55 2023, max compression
```

## Comparing `uitk-0.8.0.tar` & `uitk-0.8.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 17:27:54.482700 uitk-0.8.0/
--rw-rw-rw-   0        0        0     7815 2023-04-16 12:18:04.000000 uitk-0.8.0/COPYING.LESSER
--rw-rw-rw-   0        0        0       24 2023-03-28 23:38:26.000000 uitk-0.8.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3691 2023-07-10 17:27:54.481702 uitk-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-10 17:27:54.482700 uitk-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0     1535 2023-06-28 02:16:42.000000 uitk-0.8.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 17:27:54.426702 uitk-0.8.0/uitk/
--rw-rw-rw-   0        0        0     2937 2023-07-10 17:27:49.000000 uitk-0.8.0/uitk/__init__.py
--rw-rw-rw-   0        0        0    11209 2023-07-02 22:36:44.000000 uitk-0.8.0/uitk/events.py
--rw-rw-rw-   0        0        0    79234 2023-07-08 18:06:12.000000 uitk-0.8.0/uitk/switchboard.py
--rw-rw-rw-   0        0        0    78582 2023-07-07 17:26:57.000000 uitk-0.8.0/uitk/switchboard.py.bak
-drwxrwxrwx   0        0        0        0 2023-07-10 17:27:54.471702 uitk-0.8.0/uitk/widgets/
--rw-rw-rw-   0        0        0    19457 2023-07-02 22:38:42.000000 uitk-0.8.0/uitk/widgets/MainWindow.py
--rw-rw-rw-   0        0        0     3204 2023-05-24 20:56:51.000000 uitk-0.8.0/uitk/widgets/__init__.py
--rw-rw-rw-   0        0        0    15978 2023-06-29 12:22:22.000000 uitk-0.8.0/uitk/widgets/attributeWindow.py
--rw-rw-rw-   0        0        0     5597 2023-07-03 11:38:23.000000 uitk-0.8.0/uitk/widgets/checkBox.py
--rw-rw-rw-   0        0        0     9719 2023-07-10 16:56:56.000000 uitk-0.8.0/uitk/widgets/comboBox.py
--rw-rw-rw-   0        0        0     6954 2023-07-02 00:38:56.000000 uitk-0.8.0/uitk/widgets/draggableHeader.py
--rw-rw-rw-   0        0        0    22493 2023-07-10 00:53:06.000000 uitk-0.8.0/uitk/widgets/expandableList.py
--rw-rw-rw-   0        0        0     2494 2023-07-02 00:29:49.000000 uitk-0.8.0/uitk/widgets/label.py
--rw-rw-rw-   0        0        0     3234 2023-07-02 00:30:20.000000 uitk-0.8.0/uitk/widgets/lineEdit.py
--rw-rw-rw-   0        0        0    22168 2023-07-07 13:37:31.000000 uitk-0.8.0/uitk/widgets/menu.py
--rw-rw-rw-   0        0        0     8559 2023-06-23 14:22:44.000000 uitk-0.8.0/uitk/widgets/messageBox.py
-drwxrwxrwx   0        0        0        0 2023-07-10 17:27:54.480701 uitk-0.8.0/uitk/widgets/mixins/
--rw-rw-rw-   0        0        0     3028 2023-05-12 17:13:16.000000 uitk-0.8.0/uitk/widgets/mixins/__init__.py
--rw-rw-rw-   0        0        0    11901 2023-07-02 22:55:42.000000 uitk-0.8.0/uitk/widgets/mixins/attributes.py
--rw-rw-rw-   0        0        0     4023 2023-05-12 17:25:02.000000 uitk-0.8.0/uitk/widgets/mixins/convert.py
--rw-rw-rw-   0        0        0     9499 2023-05-20 02:33:14.000000 uitk-0.8.0/uitk/widgets/mixins/docking.py
--rw-rw-rw-   0        0        0    49547 2023-06-29 12:04:05.000000 uitk-0.8.0/uitk/widgets/mixins/style_sheet.py
--rw-rw-rw-   0        0        0     3409 2023-05-12 17:27:14.000000 uitk-0.8.0/uitk/widgets/mixins/tasks.py
--rw-rw-rw-   0        0        0    11111 2023-07-02 22:52:42.000000 uitk-0.8.0/uitk/widgets/mixins/text.py
--rw-rw-rw-   0        0        0     6046 2023-07-10 16:14:24.000000 uitk-0.8.0/uitk/widgets/optionBox.py
--rw-rw-rw-   0        0        0     3278 2023-06-05 16:23:13.000000 uitk-0.8.0/uitk/widgets/progressBar.py
--rw-rw-rw-   0        0        0     2113 2023-07-03 11:07:37.000000 uitk-0.8.0/uitk/widgets/pushButton.py
--rw-rw-rw-   0        0        0     7907 2023-05-28 21:08:35.000000 uitk-0.8.0/uitk/widgets/region.py
--rw-rw-rw-   0        0        0     3655 2023-07-02 00:31:26.000000 uitk-0.8.0/uitk/widgets/textEdit.py
-drwxrwxrwx   0        0        0        0 2023-07-10 17:27:54.455701 uitk-0.8.0/uitk.egg-info/
--rw-rw-rw-   0        0        0     3691 2023-07-10 17:27:54.000000 uitk-0.8.0/uitk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4282 2023-05-11 02:02:25.000000 uitk-0.8.0/uitk.egg-info/PKG-INFO.bak
--rw-rw-rw-   0        0        0      948 2023-07-10 17:27:54.000000 uitk-0.8.0/uitk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      767 2023-04-15 12:48:17.000000 uitk-0.8.0/uitk.egg-info/SOURCES.txt.bak
--rw-rw-rw-   0        0        0        1 2023-07-10 17:27:54.000000 uitk-0.8.0/uitk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-10 17:27:54.000000 uitk-0.8.0/uitk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 17:30:55.020821 uitk-0.8.1/
+-rw-rw-rw-   0        0        0     7815 2023-04-16 12:18:04.000000 uitk-0.8.1/COPYING.LESSER
+-rw-rw-rw-   0        0        0       24 2023-03-28 23:38:26.000000 uitk-0.8.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3763 2023-07-14 17:30:55.019822 uitk-0.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-14 17:30:55.020821 uitk-0.8.1/setup.cfg
+-rw-rw-rw-   0        0        0     1535 2023-06-28 02:16:42.000000 uitk-0.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 17:30:54.979821 uitk-0.8.1/uitk/
+-rw-rw-rw-   0        0        0     2628 2023-07-14 17:30:52.000000 uitk-0.8.1/uitk/__init__.py
+-rw-rw-rw-   0        0        0    11209 2023-07-02 22:36:44.000000 uitk-0.8.1/uitk/events.py
+-rw-rw-rw-   0        0        0    79234 2023-07-08 18:06:12.000000 uitk-0.8.1/uitk/switchboard.py
+-rw-rw-rw-   0        0        0    78582 2023-07-07 17:26:57.000000 uitk-0.8.1/uitk/switchboard.py.bak
+drwxrwxrwx   0        0        0        0 2023-07-14 17:30:55.012821 uitk-0.8.1/uitk/widgets/
+-rw-rw-rw-   0        0        0    20154 2023-07-11 19:19:34.000000 uitk-0.8.1/uitk/widgets/MainWindow.py
+-rw-rw-rw-   0        0        0     3204 2023-05-24 20:56:51.000000 uitk-0.8.1/uitk/widgets/__init__.py
+-rw-rw-rw-   0        0        0    15978 2023-06-29 12:22:22.000000 uitk-0.8.1/uitk/widgets/attributeWindow.py
+-rw-rw-rw-   0        0        0     5597 2023-07-03 11:38:23.000000 uitk-0.8.1/uitk/widgets/checkBox.py
+-rw-rw-rw-   0        0        0     9821 2023-07-11 19:40:31.000000 uitk-0.8.1/uitk/widgets/comboBox.py
+-rw-rw-rw-   0        0        0     6954 2023-07-02 00:38:56.000000 uitk-0.8.1/uitk/widgets/draggableHeader.py
+-rw-rw-rw-   0        0        0    22493 2023-07-10 00:53:06.000000 uitk-0.8.1/uitk/widgets/expandableList.py
+-rw-rw-rw-   0        0        0     2494 2023-07-02 00:29:49.000000 uitk-0.8.1/uitk/widgets/label.py
+-rw-rw-rw-   0        0        0     3234 2023-07-02 00:30:20.000000 uitk-0.8.1/uitk/widgets/lineEdit.py
+-rw-rw-rw-   0        0        0    22168 2023-07-07 13:37:31.000000 uitk-0.8.1/uitk/widgets/menu.py
+-rw-rw-rw-   0        0        0     8559 2023-06-23 14:22:44.000000 uitk-0.8.1/uitk/widgets/messageBox.py
+drwxrwxrwx   0        0        0        0 2023-07-14 17:30:55.018821 uitk-0.8.1/uitk/widgets/mixins/
+-rw-rw-rw-   0        0        0     3028 2023-05-12 17:13:16.000000 uitk-0.8.1/uitk/widgets/mixins/__init__.py
+-rw-rw-rw-   0        0        0    11901 2023-07-02 22:55:42.000000 uitk-0.8.1/uitk/widgets/mixins/attributes.py
+-rw-rw-rw-   0        0        0     4023 2023-05-12 17:25:02.000000 uitk-0.8.1/uitk/widgets/mixins/convert.py
+-rw-rw-rw-   0        0        0     9499 2023-05-20 02:33:14.000000 uitk-0.8.1/uitk/widgets/mixins/docking.py
+-rw-rw-rw-   0        0        0    49547 2023-06-29 12:04:05.000000 uitk-0.8.1/uitk/widgets/mixins/style_sheet.py
+-rw-rw-rw-   0        0        0     3409 2023-05-12 17:27:14.000000 uitk-0.8.1/uitk/widgets/mixins/tasks.py
+-rw-rw-rw-   0        0        0    11111 2023-07-02 22:52:42.000000 uitk-0.8.1/uitk/widgets/mixins/text.py
+-rw-rw-rw-   0        0        0     6046 2023-07-10 16:14:24.000000 uitk-0.8.1/uitk/widgets/optionBox.py
+-rw-rw-rw-   0        0        0     3278 2023-06-05 16:23:13.000000 uitk-0.8.1/uitk/widgets/progressBar.py
+-rw-rw-rw-   0        0        0     2113 2023-07-03 11:07:37.000000 uitk-0.8.1/uitk/widgets/pushButton.py
+-rw-rw-rw-   0        0        0     7907 2023-05-28 21:08:35.000000 uitk-0.8.1/uitk/widgets/region.py
+-rw-rw-rw-   0        0        0     3655 2023-07-02 00:31:26.000000 uitk-0.8.1/uitk/widgets/textEdit.py
+drwxrwxrwx   0        0        0        0 2023-07-14 17:30:54.994822 uitk-0.8.1/uitk.egg-info/
+-rw-rw-rw-   0        0        0     3763 2023-07-14 17:30:54.000000 uitk-0.8.1/uitk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4282 2023-05-11 02:02:25.000000 uitk-0.8.1/uitk.egg-info/PKG-INFO.bak
+-rw-rw-rw-   0        0        0      948 2023-07-14 17:30:54.000000 uitk-0.8.1/uitk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      767 2023-04-15 12:48:17.000000 uitk-0.8.1/uitk.egg-info/SOURCES.txt.bak
+-rw-rw-rw-   0        0        0        1 2023-07-14 17:30:54.000000 uitk-0.8.1/uitk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-14 17:30:54.000000 uitk-0.8.1/uitk.egg-info/top_level.txt
```

### Comparing `uitk-0.8.0/COPYING.LESSER` & `uitk-0.8.1/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `uitk-0.8.0/PKG-INFO` & `uitk-0.8.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: uitk
-Version: 0.8.0
+Version: 0.8.1
 Home-page: https://github.com/m3trik/uitk
 Author: Ryan Simpson
 Author-email: m3trik@outlook.com
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: COPYING.LESSER
 
 [![License: LGPL v3](https://img.shields.io/badge/License-LGPL%20v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0.en.html)
+![Version](https://img.shields.io/badge/Version-0.8.1-brightgreen.svg)
 
 # UITK: Dynamic UI Management for Python with PySide2
 
 UITK is a comprehensive Python package designed to streamline the creation, management, and interaction of user interfaces (UIs) using PySide2. With a focus on versatility, UITK leverages a naming convention-based switchboard module to dynamically load UI files, register custom widgets, manage slots and styles, and facilitate interaction with widgets. The primary goal of UITK is to simplify the development process of complex UIs and enhance the efficiency of event handling.
 
 ## Key Features
```

### Comparing `uitk-0.8.0/setup.py` & `uitk-0.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `uitk-0.8.0/uitk/__init__.py` & `uitk-0.8.1/uitk/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import importlib
 import pkgutil
 import inspect
 from .switchboard import signals  # Make signals accessible at package root
 
 
 __package__ = "uitk"
-__version__ = '0.8.0'
+__version__ = "0.8.1"
 __path__ = [os.path.abspath(os.path.dirname(__file__))]
 
 
 # Define a dictionary to map class names to their respective modules
 CLASS_TO_MODULE = {}
 
 # Build the CLASS_TO_MODULE dictionary by iterating over all submodules of the package
@@ -43,25 +43,18 @@
     raise AttributeError(f"module {__package__} has no attribute '{name}'")
 
 
 # --------------------------------------------------------------------------------------------
 
 
 # --------------------------------------------------------------------------------------------
-
-
-# --------------------------------------------------------------------------------------------
 # Notes
 # --------------------------------------------------------------------------------------------
 
 # The CLASS_TO_MODULE dictionary is built by iterating over all submodules of the package and checking if each submodule defines any classes.
 # The resulting dictionary maps class names to their respective module names.
 
 # When __getattr__ is called with a class name, it checks if the class name is in the CLASS_TO_MODULE dictionary.
 # If it is, __getattr__ imports the corresponding module if it hasn't already been imported, and returns the requested class object from the module using getattr.
 
 # Therefore, the classes are imported on-demand as they are requested, rather than all at once when the package is first imported.
 # This can help reduce startup time and memory usage, especially for large packages with many modules and classes.
-
-# --------------------------------------------------------------------------------------------
-# deprecated:
-# --------------------------------------------------------------------------------------------
```

### Comparing `uitk-0.8.0/uitk/events.py` & `uitk-0.8.1/uitk/events.py`

 * *Files identical despite different names*

### Comparing `uitk-0.8.0/uitk/switchboard.py` & `uitk-0.8.1/uitk/switchboard.py`

 * *Files identical despite different names*

### Comparing `uitk-0.8.0/uitk/switchboard.py.bak` & `uitk-0.8.1/uitk/switchboard.py.bak`

 * *Files identical despite different names*

### Comparing `uitk-0.8.0/uitk/widgets/MainWindow.py` & `uitk-0.8.1/uitk/widgets/MainWindow.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             <UI>.is_current (bool): True if the UI is set as current.
             <UI>.is_initialized (bool): True after the UI is first shown.
             <UI>.is_connected (bool): True if the UI is connected to its slots.
             <UI>.connect_on_show: Establish connections immediately before the UI becomes visible.
             <UI>.prevent_hide (bool): While True, the hide method is disabled.
             <UI>.widgets (list): All the widgets of the UI.
             <UI>.slots (obj): The slots class instance.
+            <UI>.stays_on_top (bool): Keep the window on top of other windows.
             <UI>._deferred: A dictionary of deferred methods.
         """
         super().__init__()
 
         self._init_logger(log_level)
 
         self.sb = switchboard_instance
@@ -217,14 +218,31 @@
                 signal.connect(
                     lambda v=None, w=widget: self.on_child_changed.emit(v, w)
                     if v is not None
                     else None
                 )
 
     @property
+    def stays_on_top(self):
+        """Returns if the window stays on top of all others."""
+        return self.windowFlags() & QtCore.Qt.WindowStaysOnTopHint
+
+    @stays_on_top.setter
+    def stays_on_top(self, value):
+        """Sets the window to stay on top of all others.
+
+        Args:
+            value (bool): If True, the window will stay on top of all others.
+        """
+        if value:
+            self.setWindowFlags(self.windowFlags() | QtCore.Qt.WindowStaysOnTopHint)
+        else:
+            self.setWindowFlags(self.windowFlags() & ~QtCore.Qt.WindowStaysOnTopHint)
+
+    @property
     def slots(self):
         """Returns a list of the slots connected to the widget's signals.
 
         Returns:
             list: A list of the slots connected to the widget's signals.
         """
         return self.sb.get_slots(self)
```

### Comparing `uitk-0.8.0/uitk/widgets/__init__.py` & `uitk-0.8.1/uitk/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `uitk-0.8.0/uitk/widgets/attributeWindow.py` & `uitk-0.8.1/uitk/widgets/attributeWindow.py`

 * *Files identical despite different names*

### Comparing `uitk-0.8.0/uitk/widgets/checkBox.py` & `uitk-0.8.1/uitk/widgets/checkBox.py`

 * *Files identical despite different names*

### Comparing `uitk-0.8.0/uitk/widgets/comboBox.py` & `uitk-0.8.1/uitk/widgets/comboBox.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,24 +9,27 @@
 class ComboBox(QtWidgets.QComboBox, AttributesMixin, RichText, TextOverlay):
     """Custom ComboBox widget with additional features and custom signal handling."""
 
     before_popup_shown = QtCore.Signal()
     before_popup_hidden = QtCore.Signal()
     on_editing_finished = QtCore.Signal(str)
 
-    def __init__(self, parent=None, double_click_interval=100, **kwargs):
+    def __init__(
+        self, parent=None, editable=False, double_click_interval=500, **kwargs
+    ):
         super().__init__(parent)
         self.menu = Menu(self, mode="option")  # Initialize context menu
 
         # Initialize other properties for handling double click and editing
-        self.lastClickTime = QtCore.QTime.currentTime()
-        self.double_click_interval = 500
-        self.doubleClicked = False
+        self.editable = editable
         self.editingInProgress = False
         self.latestEditedText = ""
+        self.double_click_interval = double_click_interval
+        self.lastClickTime = QtCore.QTime.currentTime()
+        self.doubleClicked = False
 
         self.set_attributes(**kwargs)
 
     @property
     def items(self):
         return [
             self.itemData(i) if self.itemData(i) else self.itemText(i)
@@ -152,15 +155,15 @@
     def hidePopup(self):
         self.before_popup_hidden.emit()
         super().hidePopup()
 
     def mousePressEvent(self, event):
         clickTime = QtCore.QTime.currentTime()
         elapsed = clickTime.msecsTo(self.lastClickTime) * -1
-        if elapsed < self.double_click_interval:
+        if self.editable and elapsed < self.double_click_interval:
             self.double_click_behavior()
             self.doubleClicked = True
         else:
             self.doubleClicked = False
         self.lastClickTime = clickTime
         event.accept()
```

### Comparing `uitk-0.8.0/uitk/widgets/draggableHeader.py` & `uitk-0.8.1/uitk/widgets/draggableHeader.py`

 * *Files identical despite different names*

### Comparing `uitk-0.8.0/uitk/widgets/expandableList.py` & `uitk-0.8.1/uitk/widgets/expandableList.py`

 * *Files identical despite different names*

### Comparing `uitk-0.8.0/uitk/widgets/label.py` & `uitk-0.8.1/uitk/widgets/label.py`

 * *Files identical despite different names*

### Comparing `uitk-0.8.0/uitk/widgets/lineEdit.py` & `uitk-0.8.1/uitk/widgets/lineEdit.py`

 * *Files identical despite different names*

### Comparing `uitk-0.8.0/uitk/widgets/menu.py` & `uitk-0.8.1/uitk/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `uitk-0.8.0/uitk/widgets/messageBox.py` & `uitk-0.8.1/uitk/widgets/messageBox.py`

 * *Files identical despite different names*

### Comparing `uitk-0.8.0/uitk/widgets/mixins/__init__.py` & `uitk-0.8.1/uitk/widgets/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `uitk-0.8.0/uitk/widgets/mixins/attributes.py` & `uitk-0.8.1/uitk/widgets/mixins/attributes.py`

 * *Files identical despite different names*

### Comparing `uitk-0.8.0/uitk/widgets/mixins/convert.py` & `uitk-0.8.1/uitk/widgets/mixins/convert.py`

 * *Files identical despite different names*

### Comparing `uitk-0.8.0/uitk/widgets/mixins/docking.py` & `uitk-0.8.1/uitk/widgets/mixins/docking.py`

 * *Files identical despite different names*

### Comparing `uitk-0.8.0/uitk/widgets/mixins/style_sheet.py` & `uitk-0.8.1/uitk/widgets/mixins/style_sheet.py`

 * *Files identical despite different names*

### Comparing `uitk-0.8.0/uitk/widgets/mixins/tasks.py` & `uitk-0.8.1/uitk/widgets/mixins/tasks.py`

 * *Files identical despite different names*

### Comparing `uitk-0.8.0/uitk/widgets/mixins/text.py` & `uitk-0.8.1/uitk/widgets/mixins/text.py`

 * *Files identical despite different names*

### Comparing `uitk-0.8.0/uitk/widgets/optionBox.py` & `uitk-0.8.1/uitk/widgets/optionBox.py`

 * *Files identical despite different names*

### Comparing `uitk-0.8.0/uitk/widgets/progressBar.py` & `uitk-0.8.1/uitk/widgets/progressBar.py`

 * *Files identical despite different names*

### Comparing `uitk-0.8.0/uitk/widgets/pushButton.py` & `uitk-0.8.1/uitk/widgets/pushButton.py`

 * *Files identical despite different names*

### Comparing `uitk-0.8.0/uitk/widgets/region.py` & `uitk-0.8.1/uitk/widgets/region.py`

 * *Files identical despite different names*

### Comparing `uitk-0.8.0/uitk/widgets/textEdit.py` & `uitk-0.8.1/uitk/widgets/textEdit.py`

 * *Files identical despite different names*

### Comparing `uitk-0.8.0/uitk.egg-info/PKG-INFO` & `uitk-0.8.1/uitk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: uitk
-Version: 0.8.0
+Version: 0.8.1
 Home-page: https://github.com/m3trik/uitk
 Author: Ryan Simpson
 Author-email: m3trik@outlook.com
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: COPYING.LESSER
 
 [![License: LGPL v3](https://img.shields.io/badge/License-LGPL%20v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0.en.html)
+![Version](https://img.shields.io/badge/Version-0.8.1-brightgreen.svg)
 
 # UITK: Dynamic UI Management for Python with PySide2
 
 UITK is a comprehensive Python package designed to streamline the creation, management, and interaction of user interfaces (UIs) using PySide2. With a focus on versatility, UITK leverages a naming convention-based switchboard module to dynamically load UI files, register custom widgets, manage slots and styles, and facilitate interaction with widgets. The primary goal of UITK is to simplify the development process of complex UIs and enhance the efficiency of event handling.
 
 ## Key Features
```

### Comparing `uitk-0.8.0/uitk.egg-info/PKG-INFO.bak` & `uitk-0.8.1/uitk.egg-info/PKG-INFO.bak`

 * *Files identical despite different names*

### Comparing `uitk-0.8.0/uitk.egg-info/SOURCES.txt` & `uitk-0.8.1/uitk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `uitk-0.8.0/uitk.egg-info/SOURCES.txt.bak` & `uitk-0.8.1/uitk.egg-info/SOURCES.txt.bak`

 * *Files identical despite different names*

