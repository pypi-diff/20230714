# Comparing `tmp/qvsed-1.5.6.tar.gz` & `tmp/qvsed-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qvsed-1.5.6.tar", last modified: Thu Jul 13 16:10:37 2023, max compression
+gzip compressed data, was "qvsed-1.5.7.tar", last modified: Fri Jul 14 15:42:29 2023, max compression
```

## Comparing `qvsed-1.5.6.tar` & `qvsed-1.5.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 16:10:37.523616 qvsed-1.5.6/
--rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.5.6/LICENSE.txt
--rw-rw-rw-   0        0        0       88 2023-07-13 11:04:38.000000 qvsed-1.5.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1263 2023-07-13 16:10:37.523616 qvsed-1.5.6/PKG-INFO
--rw-rw-rw-   0        0        0     6818 2023-07-13 15:58:25.000000 qvsed-1.5.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 16:10:37.499352 qvsed-1.5.6/qvsed/
--rw-rw-rw-   0        0        0       50 2023-07-08 20:05:55.000000 qvsed-1.5.6/qvsed/__init__.py
--rw-rw-rw-   0        0        0      767 2023-07-13 15:51:04.000000 qvsed-1.5.6/qvsed/config_default.py
--rw-rw-rw-   0        0        0    26528 2023-07-13 15:54:00.000000 qvsed-1.5.6/qvsed/qvsed.py
--rw-rw-rw-   0        0        0     7950 2023-07-09 10:52:35.000000 qvsed-1.5.6/qvsed/qvsed.ui
--rw-rw-rw-   0        0        0     4175 2023-07-13 15:16:38.000000 qvsed-1.5.6/qvsed/qvsed_dialog.ui
-drwxrwxrwx   0        0        0        0 2023-07-13 16:10:37.521089 qvsed-1.5.6/qvsed.egg-info/
--rw-rw-rw-   0        0        0     1263 2023-07-13 16:10:37.000000 qvsed-1.5.6/qvsed.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-07-13 16:10:37.000000 qvsed-1.5.6/qvsed.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 16:10:37.000000 qvsed-1.5.6/qvsed.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-13 16:10:37.000000 qvsed-1.5.6/qvsed.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-07-13 16:10:37.000000 qvsed-1.5.6/qvsed.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-13 16:10:37.000000 qvsed-1.5.6/qvsed.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 16:10:37.523616 qvsed-1.5.6/setup.cfg
--rw-rw-rw-   0        0        0     1652 2023-07-13 16:10:15.000000 qvsed-1.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:42:29.032380 qvsed-1.5.7/
+-rw-rw-rw-   0        0        0    35823 2023-07-06 15:36:27.000000 qvsed-1.5.7/LICENSE.txt
+-rw-rw-rw-   0        0        0       88 2023-07-13 16:48:35.000000 qvsed-1.5.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1263 2023-07-14 15:42:29.032380 qvsed-1.5.7/PKG-INFO
+-rw-rw-rw-   0        0        0     7389 2023-07-14 15:41:43.000000 qvsed-1.5.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 15:42:28.977516 qvsed-1.5.7/qvsed/
+-rw-rw-rw-   0        0        0       50 2023-07-08 20:05:55.000000 qvsed-1.5.7/qvsed/__init__.py
+-rw-rw-rw-   0        0        0      767 2023-07-13 15:51:04.000000 qvsed-1.5.7/qvsed/config_default.py
+-rw-rw-rw-   0        0        0    27722 2023-07-14 15:38:07.000000 qvsed-1.5.7/qvsed/qvsed.py
+-rw-rw-rw-   0        0        0     7950 2023-07-09 10:52:35.000000 qvsed-1.5.7/qvsed/qvsed.ui
+-rw-rw-rw-   0        0        0     5043 2023-07-14 15:38:03.000000 qvsed-1.5.7/qvsed/qvsed_dialog.ui
+drwxrwxrwx   0        0        0        0 2023-07-14 15:42:29.029379 qvsed-1.5.7/qvsed.egg-info/
+-rw-rw-rw-   0        0        0     1263 2023-07-14 15:42:28.000000 qvsed-1.5.7/qvsed.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-07-14 15:42:28.000000 qvsed-1.5.7/qvsed.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 15:42:28.000000 qvsed-1.5.7/qvsed.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-14 15:42:28.000000 qvsed-1.5.7/qvsed.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-07-14 15:42:28.000000 qvsed-1.5.7/qvsed.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-14 15:42:28.000000 qvsed-1.5.7/qvsed.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 15:42:29.035678 qvsed-1.5.7/setup.cfg
+-rw-rw-rw-   0        0        0     1652 2023-07-14 15:38:41.000000 qvsed-1.5.7/setup.py
```

### Comparing `qvsed-1.5.6/LICENSE.txt` & `qvsed-1.5.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qvsed-1.5.6/PKG-INFO` & `qvsed-1.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.5.6
+Version: 1.5.7
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.5.6/README.md` & `qvsed-1.5.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # QVSED - Qt-based Volatile Small Editor
 
 QVSED is a volatile text editor.
 
-![QVSED screenshot, showing the help message](qvsed-screenshot.png)
+![QVSED screenshot, showing the help message](screenshots/qvsed-screenshot.png)
 
 "Volatile" means that QVSED is entirely stateless - once you open a file, QVSED doesn't store any file paths or any other data other than the text contents of the file you loaded.
 Additionally, QVSED won't prompt you if you're about to potentially lose an unsaved file, since it doesn't know of any file metadata.
 
 QVSED follows the philosophy of ultra-minimalism, with its heavy emphasis on just editing text and nothing more.
 QVSED's editing style is text-based, not file-based like basically every other editor out there.
 Text goes in, from a file, and then text later comes out, into another or perhaps the same file.
@@ -28,14 +28,20 @@
 
 To run QVSED, use the `qvsed` command. Feel free to make a shortcut/alias/symlink to it if you find that convenient.
 
 ## License
 
 QVSED is free software, licensed under the GNU General Public License version 3 or later.
 
+## Configuration
+
+For configuration documentation, see [CONFIG.md](CONFIG.md).
+
+For colour scheme configuration, see [COLOURS.md](COLOURS.md) for a list of sample colour schemes.
+
 ## Usage
 
 QVSED is broken up into three parts - the Action Deck, the Text Area and the Echo Area.
 
 The Action Deck contains editing commands, the Text Area is where the text content goes, and the Echo Area is where messages will be printed.
 
 There's also the File Picker, for whenever QVSED prompts you to open or save a file. It provides a simple text entry and a button to open your system's file picker.
@@ -47,17 +53,19 @@
 ### Key Prefixes
 
 + `C-` - `Ctrl` (Windows, Linux), `⌘` (macOS)
 + `A-` - `Alt` (Windows, Linux), `⌥` (macOS)
 
 When you see `<C-n>`, for instance, that means pressing `Ctrl+N` on Windows/Linux, or `⌘N` on macOS.
 
-`Ctrl` being `⌘` and `Alt` being `⌥` is a Qt thing, not a QVSED thing, and there isn't much of a reason to change it.
+This kind of notation was inspired by Emacs (though, QVSED uses `A-` instead of `M-` to explicitly mean "Alt").
+
+`Ctrl` being `⌘` is a Qt thing, not a QVSED thing, and there isn't much of a reason to change it.
 
-This kind of notation was inspired by Emacs (though, QVSED uses `A-` instead of `M-` to be clearer).
+`Alt` being `⌥` is a Mac thing anyway, and there's not much difference in that case, even Emacs uses `⌥`.
 
 ### Action Deck bindings
 
 These bindings are evolutions of the original ASMED key bindings.
 
 + **Clear Text** - `<C-n>` - Clear the Text Area. Think of it like New File.
 + **Open File** - `<C-f>` - Launch a file picker and load the chosen file's contents into the Text Area.
@@ -67,14 +75,15 @@
 + **Quit QVSED**  - `<A-q>` - Quit QVSED on the spot with no confirmation dialog.
 
 ### File Picker bindings
 
 + **Open/Save** - `<RET>` - Load from/save to the specified file path.
 + **Cancel** - `<ESC>` or `<A-q>` - Cancel and go back to QVSED.
 + **System File Picker**  - `<C-d>` - Launch your OS file picker.
++ **Change Directory**  - `<A-d>` - Change the current working directory.
 
 ### Motion bindings
 
 These bindings are for the most part inspired by Vim, if not Emacs.
 
 + `<A-h>` - Move left a character. Inspired by Vim's `h`.
 + `<A-j>` - Move down a character. Inspired by Vim's `j`.
@@ -88,50 +97,53 @@
 + `<A-b>` - Move back a word. Inspired by Vim's `b`.
 
 + `<A-a>` - Move to the start of the line. Inspired by Emacs' `<C-a>`.
 + `<A-e>` - Move to the end of the line. Inspired by Emacs' `<C-e>`.
 
 ## Action Deck
 
+![Action Deck](screenshots/action-deck-screenshot.png)
+
 The Action Deck, positioned on the left side of the QVSED window, containing commands to clear the Text Area, open or save a file, display this help text, toggle in and out of full screen mode or quit QVSED.
 
 The Action Deck is on the left rather than on the top like a traditional menu bar, so that the buttons can be bigger while still providing enough screen real estate for the Text Area.
 
 ## Text Area
 
+![Text Area](screenshots/text-area-screenshot.png)
+
 The Text Area is where the actual text editing takes place.
 
 You can enter and delete text, scroll down and up, cut, copy, paste, all that standard Notepad stuff.
 
 QVSED is intentionally simplistic, and so there's not much to the Text Area.
 
 ## Echo Area
 
+![Echo Area](screenshots/echo-area-screenshot.png)
+
 The Echo Area is the small bar at the bottom of the QVSED window that prints information.
 
 For example, when a file is opened, it prints its file name. If a config file was not found, it'll generate one and give you the path.
 
 QVSED inherited the name from Emacs. Well, less "inherited" and more "stolen from."
 
 ## File Picker
 
+![File Picker](screenshots/file-picker-screenshot.png)
+
 The File Picker is displayed when you use the **Open File** or **Save File** Action Deck commands.
 
 It consists of the following elements:
 
 + A label instructing you to enter the file path, relative or absolute.
 + Another label that shows the current working directory.
 + A text box where you can enter the file path.
 + Three buttons:
   + **System File Picker** opens your operating system's file picker, so you can select the file you want without having to type in its path, just like in pre-1.5.0 QVSED versions. This can also be accessed with the `<C-d>` key binding.
+  + **Change Directory** changes the current working directory to the one specified in the path box. This can also be accessed with the `<A-d>` key binding.
   + **Open** or **Save** (depending on the Action Deck command you used) opens or saves the file at the specified path.
   + **Cancel** closes the dialog without saving any changes.
 
 The File Picker makes it simple to load the file you want, simply by typing in its path.
 
 If this is too oversimplified for you, or you just need to use your system file picker for whatever reason, you can always use the System File Picker option.
-
-## Configuration
-
-For configuration documentation, see [CONFIG.md](CONFIG.md).
-
-For colour scheme configuration, see [COLOURS.md](COLOURS.md) for a list of sample colour schemes.
```

### Comparing `qvsed-1.5.6/qvsed/config_default.py` & `qvsed-1.5.7/qvsed/config_default.py`

 * *Files identical despite different names*

### Comparing `qvsed-1.5.6/qvsed/qvsed.py` & `qvsed-1.5.7/qvsed/qvsed.py`

 * *Files 3% similar despite different names*

```diff
@@ -649,18 +649,14 @@
     """
     Class for QVSED file dialogs.
     """
     def __init__(self, operation, parent=None):
         super(FileDialogBox, self).__init__(parent)
         self.load_ui_file()
 
-        home_dir = os.path.expanduser("~")
-        cwd = os.getcwd().replace(home_dir, "~").replace("\\", "/")
-        self.cwdLabel.setText(f"Current working directory is {cwd}")
-
         self.operation = operation
         self.selected_file_path = ""
 
         self.setWindowTitle(f"{self.operation.capitalize()} File")
 
         self.set_shortcuts()
         self.update_labels()
@@ -675,14 +671,17 @@
         self.cancelButton.clicked.connect(self.reject)
         self.cancelButton.setShortcut(QKeySequence(Qt.Key_Escape))
         self.cancelButton.setShortcut(QKeySequence("Alt+Q"))
 
         self.openSystemDialogButton.clicked.connect(self.open_system_dialog)
         self.openSystemDialogButton.setShortcut(QKeySequence("Ctrl+D"))
 
+        self.chdirButton.clicked.connect(self.set_current_working_directory)
+        self.chdirButton.setShortcut(QKeySequence("Alt+D"))
+
     def load_ui_file(self):
         """
         Load the UI file for the QVSED dialog box.
         """
         current_dir = os.path.dirname(os.path.abspath(__file__))
         ui_file = os.path.join(current_dir, "qvsed_dialog.ui")
         loadUi(ui_file, self)
@@ -690,44 +689,80 @@
     def open_system_dialog(self):
         """
         Used to open the system's file dialog.
         """
         file_dialog = QFileDialog()
 
         if self.operation == "save":
-            file_path, _ = file_dialog.getOpenFileName(self, "Save File")
+            file_path, _ = file_dialog.getSaveFileName(self, "Save File", self.get_selected_directory())
         elif self.operation == "open":
-            file_path, _ = file_dialog.getOpenFileName(self, "Open File")
+            file_path, _ = file_dialog.getOpenFileName(self, "Open File", self.get_selected_directory())
 
         if file_path:
             self.filePathBox.setText(file_path)
             self.selected_file_path = file_path
             self.accept()
 
+    def check_path(self, initial_value, isdir=False):
+        """
+        Return a file or directory path with additional checks.
+        """
+        path = initial_value
+
+        if isdir:
+            if path and not path.endswith(("/", "\\")):
+                path += os.sep
+            path = os.path.dirname(path)
+
+        if path.startswith('~'):
+            path = os.path.expanduser(path.replace('~', os.path.expanduser('~')))
+        return path
+
     def get_selected_file_path(self):
         """
         Return the file path specified in the file path box.
         """
-        file_path = self.filePathBox.text()
-        if os.name == 'nt' and file_path.startswith('~'):
-            file_path = os.path.expanduser(file_path.replace('~', os.path.expanduser('~')))
+        file_path = self.check_path(self.filePathBox.text())
+
         if file_path:
             return file_path
         return None
 
+    def get_selected_directory(self):
+        """
+        Return the directory path specified in the file path box.
+        """
+        directory_path = self.check_path(self.filePathBox.text(), True)
+
+        if directory_path and os.path.isdir(directory_path):
+            return directory_path
+        return None
+
+    def set_current_working_directory(self):
+        """
+        Set the current working directory.
+        """
+        chosen_directory = self.get_selected_directory()
+        if chosen_directory is not None:
+            os.chdir(chosen_directory)
+            self.update_labels()
+            self.filePathBox.clear()
+
     def update_labels(self):
         """
-        Update the labels depending on the operation
+        Update the labels depending on the operation.
         """
         self.mainLabel.setText(f"Enter the file path to {self.operation} (relative or absolute)")
         self.confirmButton.setText(self.operation.capitalize())
+        home_dir = os.path.expanduser("~")
+        cwd = os.getcwd().replace(home_dir, "~").replace("\\", "/")
+        self.cwdLabel.setText(f"Current working directory is {cwd}")
 
 def main():
     """
     The entry point for the QVSED application.
     """
     app = QVSEDApp()
     app.run()
 
-
 if __name__ == "__main__":
     main()
```

### Comparing `qvsed-1.5.6/qvsed/qvsed.ui` & `qvsed-1.5.7/qvsed/qvsed.ui`

 * *Files identical despite different names*

### Comparing `qvsed-1.5.6/qvsed/qvsed_dialog.ui` & `qvsed-1.5.7/qvsed/qvsed_dialog.ui`

 * *Files 26% similar despite different names*

#### Comparing `qvsed-1.5.6/qvsed/qvsed_dialog.ui` & `qvsed-1.5.7/qvsed/qvsed_dialog.ui`

```diff
@@ -2,38 +2,44 @@
 <ui version="4.0">
   <class>FileDialog</class>
   <widget class="QDialog" name="FileDialog">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>556</width>
-        <height>216</height>
+        <width>795</width>
+        <height>214</height>
       </rect>
     </property>
     <property name="windowTitle">
       <string>Dialog</string>
     </property>
+    <property name="sizeGripEnabled">
+      <bool>false</bool>
+    </property>
+    <property name="modal">
+      <bool>false</bool>
+    </property>
     <layout class="QVBoxLayout" name="verticalLayout_2">
       <item>
         <layout class="QVBoxLayout" name="verticalLayout">
           <property name="spacing">
-            <number>16</number>
+            <number>12</number>
           </property>
           <property name="leftMargin">
-            <number>16</number>
+            <number>12</number>
           </property>
           <property name="topMargin">
-            <number>16</number>
+            <number>12</number>
           </property>
           <property name="rightMargin">
-            <number>16</number>
+            <number>12</number>
           </property>
           <property name="bottomMargin">
-            <number>16</number>
+            <number>12</number>
           </property>
           <item>
             <widget class="QLabel" name="mainLabel">
               <property name="font">
                 <font>
                   <pointsize>12</pointsize>
                 </font>
@@ -71,14 +77,17 @@
               <property name="styleSheet">
                 <string notr="true">padding: 8px</string>
               </property>
             </widget>
           </item>
           <item>
             <layout class="QHBoxLayout" name="horizontalLayout">
+              <property name="spacing">
+                <number>8</number>
+              </property>
               <item>
                 <widget class="QPushButton" name="openSystemDialogButton">
                   <property name="font">
                     <font>
                       <pointsize>11</pointsize>
                     </font>
                   </property>
@@ -90,21 +99,42 @@
                   </property>
                   <property name="autoDefault">
                     <bool>false</bool>
                   </property>
                 </widget>
               </item>
               <item>
+                <widget class="QPushButton" name="chdirButton">
+                  <property name="font">
+                    <font>
+                      <pointsize>11</pointsize>
+                    </font>
+                  </property>
+                  <property name="styleSheet">
+                    <string notr="true">padding: 10px 17px</string>
+                  </property>
+                  <property name="text">
+                    <string>Change Directory &lt;A-d&gt;</string>
+                  </property>
+                  <property name="autoDefault">
+                    <bool>false</bool>
+                  </property>
+                  <property name="flat">
+                    <bool>false</bool>
+                  </property>
+                </widget>
+              </item>
+              <item>
                 <spacer name="horizontalSpacer">
                   <property name="orientation">
                     <enum>Qt::Horizontal</enum>
                   </property>
                   <property name="sizeHint" stdset="0">
                     <size>
-                      <width>40</width>
+                      <width>80</width>
                       <height>20</height>
                     </size>
                   </property>
                 </spacer>
               </item>
               <item>
                 <widget class="QPushButton" name="confirmButton">
```

### Comparing `qvsed-1.5.6/qvsed.egg-info/PKG-INFO` & `qvsed-1.5.7/qvsed.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qvsed
-Version: 1.5.6
+Version: 1.5.7
 Summary: Qt-Based Volatile Small Editor
 Home-page: https://github.com/That1M8Head/QVSED/
 Author: Arsalan Kazmi
 License: GPL-3.0-or-later
 License-File: LICENSE.txt
 
 QVSED is a volatile and small text editor.
```

### Comparing `qvsed-1.5.6/setup.py` & `qvsed-1.5.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 The setup.py file for QVSED.
 """
 from setuptools import setup, find_packages
 
 setup(
     name='qvsed',
-    version='1.5.6',
+    version='1.5.7',
     author='Arsalan Kazmi',
     description='Qt-Based Volatile Small Editor',
     long_description="""QVSED is a volatile and small text editor.
 
 "Volatile" means that QVSED is entirely stateless - once you open a file, QVSED doesn't store any file paths or any other data other than the text contents of the file you loaded.
 Additionally, QVSED won't prompt you if you're about to potentially lose an unsaved file, since it doesn't know of any file metadata.
 You may be prompted if you're about to overwrite a file, but that's up to your OS, not QVSED.
```

