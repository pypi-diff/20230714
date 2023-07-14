# Comparing `tmp/qvsed-1.5.8.tar.gz` & `tmp/qvsed-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qvsed-1.5.8.tar", last modified: Fri Jul 14 16:25:51 2023, max compression
+gzip compressed data, was "qvsed-1.5.9.tar", last modified: Fri Jul 14 21:20:16 2023, max compression
```

## Comparing `qvsed-1.5.8.tar` & `qvsed-1.5.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 16:25:51.081826 qvsed-1.5.8/
--rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.5.8/LICENSE.txt
--rw-rw-rw-   0        0        0       88 2023-07-13 16:48:35.000000 qvsed-1.5.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1263 2023-07-14 16:25:51.081826 qvsed-1.5.8/PKG-INFO
--rw-rw-rw-   0        0        0     7389 2023-07-14 15:41:43.000000 qvsed-1.5.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 16:25:51.060540 qvsed-1.5.8/qvsed/
--rw-rw-rw-   0        0        0       50 2023-07-08 20:05:55.000000 qvsed-1.5.8/qvsed/__init__.py
--rw-rw-rw-   0        0        0      787 2023-07-14 16:23:39.000000 qvsed-1.5.8/qvsed/config_default.py
--rw-rw-rw-   0        0        0    28049 2023-07-14 16:14:05.000000 qvsed-1.5.8/qvsed/qvsed.py
--rw-rw-rw-   0        0        0     7950 2023-07-09 10:52:35.000000 qvsed-1.5.8/qvsed/qvsed.ui
--rw-rw-rw-   0        0        0     5043 2023-07-14 15:38:03.000000 qvsed-1.5.8/qvsed/qvsed_dialog.ui
-drwxrwxrwx   0        0        0        0 2023-07-14 16:25:51.079439 qvsed-1.5.8/qvsed.egg-info/
--rw-rw-rw-   0        0        0     1263 2023-07-14 16:25:50.000000 qvsed-1.5.8/qvsed.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-07-14 16:25:50.000000 qvsed-1.5.8/qvsed.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 16:25:50.000000 qvsed-1.5.8/qvsed.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-14 16:25:50.000000 qvsed-1.5.8/qvsed.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-07-14 16:25:50.000000 qvsed-1.5.8/qvsed.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-14 16:25:50.000000 qvsed-1.5.8/qvsed.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 16:25:51.081826 qvsed-1.5.8/setup.cfg
--rw-rw-rw-   0        0        0     1652 2023-07-14 16:25:39.000000 qvsed-1.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 21:20:16.071239 qvsed-1.5.9/
+-rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.5.9/LICENSE.txt
+-rw-rw-rw-   0        0        0       88 2023-07-13 16:48:35.000000 qvsed-1.5.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1263 2023-07-14 21:20:16.071239 qvsed-1.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0     7389 2023-07-14 15:41:43.000000 qvsed-1.5.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 21:20:16.041498 qvsed-1.5.9/qvsed/
+-rw-rw-rw-   0        0        0       50 2023-07-08 20:05:55.000000 qvsed-1.5.9/qvsed/__init__.py
+-rw-rw-rw-   0        0        0      787 2023-07-14 16:23:39.000000 qvsed-1.5.9/qvsed/config_default.py
+-rw-rw-rw-   0        0        0    28046 2023-07-14 21:19:41.000000 qvsed-1.5.9/qvsed/qvsed.py
+-rw-rw-rw-   0        0        0     7950 2023-07-09 10:52:35.000000 qvsed-1.5.9/qvsed/qvsed.ui
+-rw-rw-rw-   0        0        0     5043 2023-07-14 15:38:03.000000 qvsed-1.5.9/qvsed/qvsed_dialog.ui
+drwxrwxrwx   0        0        0        0 2023-07-14 21:20:16.071239 qvsed-1.5.9/qvsed.egg-info/
+-rw-rw-rw-   0        0        0     1263 2023-07-14 21:20:15.000000 qvsed-1.5.9/qvsed.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-07-14 21:20:15.000000 qvsed-1.5.9/qvsed.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 21:20:15.000000 qvsed-1.5.9/qvsed.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-14 21:20:15.000000 qvsed-1.5.9/qvsed.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-07-14 21:20:15.000000 qvsed-1.5.9/qvsed.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-14 21:20:15.000000 qvsed-1.5.9/qvsed.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 21:20:16.071239 qvsed-1.5.9/setup.cfg
+-rw-rw-rw-   0        0        0     1652 2023-07-14 21:19:57.000000 qvsed-1.5.9/setup.py
```

### Comparing `qvsed-1.5.8/LICENSE.txt` & `qvsed-1.5.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qvsed-1.5.8/PKG-INFO` & `qvsed-1.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.5.8
+Version: 1.5.9
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.5.8/README.md` & `qvsed-1.5.9/README.md`

 * *Files identical despite different names*

### Comparing `qvsed-1.5.8/qvsed/config_default.py` & `qvsed-1.5.9/qvsed/config_default.py`

 * *Files identical despite different names*

### Comparing `qvsed-1.5.8/qvsed/qvsed.py` & `qvsed-1.5.9/qvsed/qvsed.py`

 * *Files 0% similar despite different names*

```diff
@@ -338,15 +338,15 @@
         button_color = getattr(qvsed_config, 'button_color', None)
         button_text_color = getattr(qvsed_config, 'button_text_color', text_color)
         button_hover_color = getattr(qvsed_config, 'button_hover_color', getattr(qvsed_config, 'button_focus_color', None))
         button_pressed_color = getattr(qvsed_config, 'button_pressed_color', background_color)
 
         text_area_color = getattr(qvsed_config, 'text_area_color', button_hover_color)
         text_area_text_color = getattr(qvsed_config, 'text_area_text_color', text_color)
-        echo_area_color = getattr(qvsed_config, 'echo_area_color', button_hover_color)
+        echo_area_color = getattr(qvsed_config, 'echo_area_color', text_area_color)
         echo_area_text_color = getattr(qvsed_config, 'echo_area_text_color', text_color)
 
         scroll_bar_color = getattr(qvsed_config, 'scroll_bar_color', button_color)
         scroll_bar_background_color = getattr(qvsed_config, 'scroll_bar_background_color', button_hover_color)
         scroll_bar_hover_color = getattr(qvsed_config, 'scroll_bar_hover_color', button_pressed_color)
         scroll_bar_pressed_color = getattr(qvsed_config, 'scroll_bar_pressed_color', button_pressed_color)
```

### Comparing `qvsed-1.5.8/qvsed/qvsed.ui` & `qvsed-1.5.9/qvsed/qvsed.ui`

 * *Files identical despite different names*

### Comparing `qvsed-1.5.8/qvsed/qvsed_dialog.ui` & `qvsed-1.5.9/qvsed/qvsed_dialog.ui`

 * *Files identical despite different names*

### Comparing `qvsed-1.5.8/qvsed.egg-info/PKG-INFO` & `qvsed-1.5.9/qvsed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.5.8
+Version: 1.5.9
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.5.8/setup.py` & `qvsed-1.5.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 The setup.py file for QVSED.
 """
 from setuptools import setup, find_packages
 
 setup(
     name='qvsed',
-    version='1.5.8',
+    version='1.5.9',
     author='Arsalan Kazmi',
     description='Qt-Based Volatile Small Editor',
     long_description="""QVSED is a volatile and small text editor.
 
 "Volatile" means that QVSED is entirely stateless - once you open a file, QVSED doesn't store any file paths or any other data other than the text contents of the file you loaded.
 Additionally, QVSED won't prompt you if you're about to potentially lose an unsaved file, since it doesn't know of any file metadata.
 You may be prompted if you're about to overwrite a file, but that's up to your OS, not QVSED.
```

