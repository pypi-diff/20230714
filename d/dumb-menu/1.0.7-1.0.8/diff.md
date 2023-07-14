# Comparing `tmp/dumb_menu-1.0.7.tar.gz` & `tmp/dumb_menu-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dumb_menu-1.0.7.tar", last modified: Sun Mar 12 05:30:49 2023, max compression
+gzip compressed data, was "dumb_menu-1.0.8.tar", last modified: Fri Jul 14 06:59:21 2023, max compression
```

## Comparing `dumb_menu-1.0.7.tar` & `dumb_menu-1.0.8.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 kasusa     (501) staff       (20)        0 2023-03-12 05:30:49.340189 dumb_menu-1.0.7/
--rw-r--r--   0 kasusa     (501) staff       (20)     1986 2023-03-12 05:30:49.339977 dumb_menu-1.0.7/PKG-INFO
--rw-r--r--   0 kasusa     (501) staff       (20)     1471 2023-03-12 05:30:34.000000 dumb_menu-1.0.7/README.md
-drwxr-xr-x   0 kasusa     (501) staff       (20)        0 2023-03-12 05:30:49.338919 dumb_menu-1.0.7/dumb_menu/
--rw-r--r--   0 kasusa     (501) staff       (20)     4295 2023-03-12 05:28:03.000000 dumb_menu-1.0.7/dumb_menu/__init__.py
-drwxr-xr-x   0 kasusa     (501) staff       (20)        0 2023-03-12 05:30:49.339717 dumb_menu-1.0.7/dumb_menu.egg-info/
--rw-r--r--   0 kasusa     (501) staff       (20)     1986 2023-03-12 05:30:49.000000 dumb_menu-1.0.7/dumb_menu.egg-info/PKG-INFO
--rw-r--r--   0 kasusa     (501) staff       (20)      172 2023-03-12 05:30:49.000000 dumb_menu-1.0.7/dumb_menu.egg-info/SOURCES.txt
--rw-r--r--   0 kasusa     (501) staff       (20)        1 2023-03-12 05:30:49.000000 dumb_menu-1.0.7/dumb_menu.egg-info/dependency_links.txt
--rw-r--r--   0 kasusa     (501) staff       (20)       10 2023-03-12 05:30:49.000000 dumb_menu-1.0.7/dumb_menu.egg-info/top_level.txt
--rw-r--r--   0 kasusa     (501) staff       (20)       38 2023-03-12 05:30:49.340246 dumb_menu-1.0.7/setup.cfg
--rw-r--r--   0 kasusa     (501) staff       (20)     1123 2023-03-12 05:22:10.000000 dumb_menu-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 06:59:21.155039 dumb_menu-1.0.8/
+-rw-rw-rw-   0        0        0     3224 2023-07-14 06:59:21.153942 dumb_menu-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2550 2023-07-14 06:55:21.000000 dumb_menu-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 06:59:21.144311 dumb_menu-1.0.8/dumb_menu/
+-rw-rw-rw-   0        0        0     4618 2023-07-14 03:01:35.000000 dumb_menu-1.0.8/dumb_menu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 06:59:21.145839 dumb_menu-1.0.8/dumb_menu.egg-info/
+-rw-rw-rw-   0        0        0     3224 2023-07-14 06:59:21.000000 dumb_menu-1.0.8/dumb_menu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2023-07-14 06:59:21.000000 dumb_menu-1.0.8/dumb_menu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 06:59:21.000000 dumb_menu-1.0.8/dumb_menu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-07-14 06:59:21.000000 dumb_menu-1.0.8/dumb_menu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-14 06:59:21.000000 dumb_menu-1.0.8/dumb_menu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 06:59:21.155039 dumb_menu-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1306 2023-07-14 06:59:18.000000 dumb_menu-1.0.8/setup.py
```

### Comparing `dumb_menu-1.0.7/dumb_menu/__init__.py` & `dumb_menu-1.0.8/dumb_menu/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,133 +1,138 @@
-import os
-import re
-
-#region windows
-def get_menu_choice1(options):
-    shortcuts = scan_short_cuts(options) # scan for shortcuts
-    selected_index = 0
-    while True:
-        os.system("cls" if os.name == "nt" else "clear") #clear screen
-        show_menu(options,selected_index)
-
-        key = b'\a' #default to error
-        try:
-            import msvcrt
-            char = msvcrt.getch() #get keypress
-        except :
-            pass
-
-        if key == b'\x1b':  # Esc key to exit
-            return -1
-        elif key == b'\r':  # Enter key to select
-            return selected_index
-        elif key in (b'\x48', b'\x50'):  # Up or Down arrow
-            selected_index = (selected_index + (1 if key == b'\x50' else -1) + len(options)) % len(options)
-        elif key in shortcuts: # Shortcut key
-            return shortcuts[key]
-        elif key == b'\a':
-            print('error , may not support your system')
-            exit()
-# endregion
-def get_key(): #get keypress using getch , msvcrt = windows or termios = linux
-    flag_have_getch = False
-    flag_have_msvcrt = False
-    try :
-        import getch
-        flag_have_getch = True
-        first_char = getch.getch()
-        if first_char == '\x1b': #arrow keys
-            a=getch.getch()
-            b=getch.getch()
-            return {'[A': 'up', '[B': 'down', '[C': 'right', '[D': 'left' }[a+b]
-        if ord(first_char) == 10:
-            return  'enter'
-        if ord(first_char) == 32:
-            return  'space'
-        else:
-            return first_char #normal keys like abcd 1234
-    except :
-        pass
-    
-    try:
-        import msvcrt
-        flag_have_msvcrt = True
-        key = msvcrt.getch()  # get keypress
-        if key == b'\x1b':  # Esc key to exit
-            return 'esc'
-        elif key == b'\r':  # Enter key to select
-            return 'enter'
-        elif key == b'\x48':  # Up or Down arrow
-            return  'up'
-        elif key == b'\x50':  # Up or Down arrow
-            return 'down'
-        else:
-            return key.decode('utf-8')
-    except:
-        pass
-    
-    if flag_have_getch == False and flag_have_msvcrt == False:
-        print('\nErr:\tcan\'t get input \nFix:\tpip install getch')
-        exit()
-
-
-def get_menu_choice(options,isclean = False):
-    shortcuts = scan_short_cuts(options)  # scan for shortcuts
-    selected_index = 0
-    print(shortcuts)
-    while True:
-        show_menu(options, selected_index , isclean)
-        key = get_key()
-        if key == 'enter':  # Enter key to select
-            return selected_index
-        elif key in ('up','down'):  # Up or Down arrow
-            selected_index = (selected_index + (1 if key == 'down' else -1) + len(options)) % len(options)
-        elif key in shortcuts:  # Shortcut key
-            show_menu(options, shortcuts[key],isclean) #show selected option when using shortcut
-            return shortcuts[key]
-
-def scan_short_cuts(options):
-    shortcuts = {}
-    for i, option in enumerate(options):
-        match = re.match(r"\[(.*)\](.*)", option)
-        if match:
-            shortcut, text = match.group(1, 2)
-            shortcuts[shortcut] = i
-    return shortcuts
-
-def show_menu(options, selected_index,isclean):
-    if isclean:
-        show_clean_menu(options, selected_index)
-    else:
-        show_normal_menu(options, selected_index)
-
-
-def show_normal_menu(options, selected_index):
-    os.system("cls" if os.name == "nt" else "clear")
-    print("Menu","current option:",selected_index)
-    for i, option in enumerate(options):
-        if i == selected_index:
-            print(f"> {option}")
-        else:
-            print(f"  {option}")
-    print("\nUse the arrow keys to move, Enter/Hotkey to select.")
-
-def show_clean_menu(options, selected_index):
-    os.system("cls" if os.name == "nt" else "clear")
-    for i, option in enumerate(options):
-        if i == selected_index:
-            print(f"> {option}")
-        else:
-            print(f"  {option}")
-
-def demo():
-    options = ["[1]Option 1", "[2]Option 2", "[3]Option 3","[q]quit"]
-    index = get_menu_choice(options,isclean=True)
-
-    if index != -1:
-        print(f"You selected option {index + 1}: {options[index]}")
-    else:
-        print("You exited the menu.")
-
-#! test code 
-# if __name__ == "__main__":
+import os
+import re
+
+#region windows
+def get_menu_choice1(options):
+    shortcuts = scan_short_cuts(options) # scan for shortcuts
+    selected_index = 0
+    while True:
+        os.system("cls" if os.name == "nt" else "clear") #clear screen
+        show_menu(options,selected_index)
+
+        key = b'\a' #default to error
+        try:
+            import msvcrt
+            char = msvcrt.getch() #get keypress
+        except :
+            pass
+
+        if key == b'\x1b':  # Esc key to exit
+            return -1
+        elif key == b'\r':  # Enter key to select
+            return selected_index
+        elif key in (b'\x48', b'\x50'):  # Up or Down arrow
+            selected_index = (selected_index + (1 if key == b'\x50' else -1) + len(options)) % len(options)
+        elif key in shortcuts: # Shortcut key
+            return shortcuts[key]
+        elif key == b'\a':
+            print('error , may not support your system')
+            exit()
+# endregion
+def get_key(): #get keypress using getch, msvcrt = windows
+    flag_have_getch = False
+    flag_have_msvcrt = False
+    try :
+        import getch
+        flag_have_getch = True
+        first_char = getch.getch()
+        if first_char == '\x1b': #arrow keys
+            a=getch.getch()
+            b=getch.getch()
+            return {'[A': 'up', '[B': 'down', '[C': 'right', '[D': 'left' }[a+b]
+        if ord(first_char) == 10:
+            return  'enter'
+        if ord(first_char) == 32:
+            return  'space'
+        else:
+            return first_char #normal keys like abcd 1234
+    except :
+        pass
+    
+    try:
+        import msvcrt
+        flag_have_msvcrt = True
+        key = msvcrt.getch()  # get keypress
+        if key == b'\x1b':  # Esc key to exit
+            return 'esc'
+        elif key == b'\r':  # Enter key to select
+            return 'enter'
+        elif key == b'\x48':  # Up or Down arrow
+            return  'up'
+        elif key == b'\x50':  # Up or Down arrow
+            return 'down'
+        else:
+            return key.decode('utf-8')
+    except:
+        pass
+    
+    if flag_have_getch == False and flag_have_msvcrt == False:
+        print('\nErr:\tcan\'t get input \nFix:\tpip install getch')
+        exit()
+
+# isclean gives a clean meun without hint text
+# give_key_str gives the key pressed instead of the index
+def get_menu_choice(options,isclean = False,give_key_str = False):
+    shortcuts = scan_short_cuts(options)  # scan for shortcuts
+    selected_index = 0
+    print(shortcuts)
+    while True:
+        show_menu(options, selected_index , isclean)
+        key = get_key()
+        if key == 'enter':  # Enter key to select
+            return selected_index
+        elif key in ('up','down'):  # Up or Down arrow
+            selected_index = (selected_index + (1 if key == 'down' else -1) + len(options)) % len(options)
+        elif key in shortcuts:  # Shortcut key
+            show_menu(options, shortcuts[key],isclean) #show selected option when using shortcut
+            if(give_key_str):
+                return key
+            else:
+                return shortcuts[key]
+
+
+def scan_short_cuts(options):
+    shortcuts = {}
+    for i, option in enumerate(options):
+        match = re.match(r"\[(.*)\](.*)", option)
+        if match:
+            shortcut, text = match.group(1, 2)
+            shortcuts[shortcut] = i
+    return shortcuts
+
+def show_menu(options, selected_index,isclean):
+    if isclean:
+        show_clean_menu(options, selected_index)
+    else:
+        show_normal_menu(options, selected_index)
+
+
+def show_normal_menu(options, selected_index):
+    os.system("cls" if os.name == "nt" else "clear")
+    print("Menu","current option:",selected_index)
+    for i, option in enumerate(options):
+        if i == selected_index:
+            print(f"> {option}")
+        else:
+            print(f"  {option}")
+    print("\nUse the arrow keys to move, Enter/Hotkey to select.")
+
+def show_clean_menu(options, selected_index):
+    os.system("cls" if os.name == "nt" else "clear")
+    for i, option in enumerate(options):
+        if i == selected_index:
+            print(f"> {option}")
+        else:
+            print(f"  {option}")
+
+def demo():
+    options = ["[1]Option 1", "[2]Option 2", "[3]Option 3","[q]quit"]
+    index = get_menu_choice(options,isclean=True)
+
+    if index != -1:
+        print(f"You selected option {index + 1}: {options[index]}")
+    else:
+        print("You exited the menu.")
+
+# # test code 
+# if __name__ == "__main__":
 #     demo()
```

### Comparing `dumb_menu-1.0.7/setup.py` & `dumb_menu-1.0.8/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,40 @@
-import codecs
-import os
-from setuptools import setup, find_packages
-
-# these things are needed for the README.md show on pypi
-here = os.path.abspath(os.path.dirname(__file__))
-
-with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
-    long_description = "\n" + fh.read()
-
-
-VERSION = '1.0.7'
-DESCRIPTION = 'a ligh weight menu , support both win and mac '
-LONG_DESCRIPTION = 'dumb_menu is a ligh weight menu ,support hot key, support both win and mac'
-
-# Setting up
-setup(
-    name="dumb_menu",
-    version=VERSION,
-    author="clever chen",
-    author_email="",
-    description=DESCRIPTION,
-    long_description_content_type="text/markdown",
-    long_description=long_description,
-    packages=find_packages(),
-    install_requires=[],
-    keywords=['python', 'menu', 'dumb_menu','windows','mac','linux'],
-    classifiers=[
-        "Development Status :: 1 - Planning",
-        "Intended Audience :: Developers",
-        "Programming Language :: Python :: 3",
-        "Operating System :: Unix",
-        "Operating System :: MacOS :: MacOS X",
-        "Operating System :: Microsoft :: Windows",
-    ]
+import codecs
+import os
+
+from setuptools import find_packages, setup
+
+# these things are needed for the README.md show on pypi
+here = os.path.abspath(os.path.dirname(__file__))
+
+with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
+    long_description = "\n" + fh.read()
+
+
+VERSION = '1.0.8'
+DESCRIPTION = 'A light weight command line menu that supports Windows, MacOS, and Linux'
+LONG_DESCRIPTION = 'A light weight command line menu. Supporting Windows, MacOS, and Linux. It has support for hotkeys'
+
+# Setting up
+setup(
+    name="dumb_menu",
+    version=VERSION,
+    author="clever chen",
+    author_email="",
+    description=DESCRIPTION,
+    long_description_content_type="text/markdown",
+    long_description=long_description,
+    packages=find_packages(),
+    install_requires=[
+        'getch; platform_system=="Unix"',
+        'getch; platform_system=="MacOS"',
+    ],
+    keywords=['python', 'menu', 'dumb_menu', 'windows', 'mac', 'linux'],
+    classifiers=[
+        "Development Status :: 1 - Planning",
+        "Intended Audience :: Developers",
+        "Programming Language :: Python :: 3",
+        "Operating System :: Unix",
+        "Operating System :: MacOS :: MacOS X",
+        "Operating System :: Microsoft :: Windows",
+    ]
 )
```

