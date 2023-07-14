# Comparing `tmp/python-negar-1.2.4.tar.gz` & `tmp/python-negar-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-negar-1.2.4.tar", last modified: Thu Jun 15 08:21:46 2023, max compression
+gzip compressed data, was "python-negar-1.2.5.tar", last modified: Fri Jul 14 10:08:12 2023, max compression
```

## Comparing `python-negar-1.2.4.tar` & `python-negar-1.2.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-06-15 08:21:46.034626 python-negar-1.2.4/
--rw-r--r--   0 javad     (1000) javad     (1000)       41 2022-03-28 12:11:27.000000 python-negar-1.2.4/AUTHORS
--rw-r--r--   0 javad     (1000) javad     (1000)     6740 2023-06-15 08:13:09.000000 python-negar-1.2.4/Changelog.txt
--rw-r--r--   0 javad     (1000) javad     (1000)    35147 2022-03-28 12:06:56.000000 python-negar-1.2.4/LICENSE
--rw-r--r--   0 javad     (1000) javad     (1000)      149 2022-03-28 12:06:56.000000 python-negar-1.2.4/MANIFEST.in
--rw-r--r--   0 javad     (1000) javad     (1000)     8548 2023-06-15 08:21:46.034626 python-negar-1.2.4/PKG-INFO
--rw-r--r--   0 javad     (1000) javad     (1000)     7590 2022-09-09 08:02:13.000000 python-negar-1.2.4/README.md
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-06-15 08:21:46.034626 python-negar-1.2.4/negar/
--rw-r--r--   0 javad     (1000) javad     (1000)       96 2022-03-28 12:34:31.000000 python-negar-1.2.4/negar/__init__.py
--rw-r--r--   0 javad     (1000) javad     (1000)     5047 2023-06-15 07:11:16.000000 python-negar-1.2.4/negar/constants.py
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-06-15 08:21:46.034626 python-negar-1.2.4/negar/data/
--rw-r--r--   0 javad     (1000) javad     (1000)        0 2022-03-28 12:06:56.000000 python-negar-1.2.4/negar/data/__init__.py
--rw-r--r--   0 javad     (1000) javad     (1000)    29312 2022-12-21 09:31:33.000000 python-negar-1.2.4/negar/data/untouchable.dat
--rw-r--r--   0 javad     (1000) javad     (1000)      346 2023-03-28 18:56:35.000000 python-negar-1.2.4/negar/gui.py
--rw-r--r--   0 javad     (1000) javad     (1000)    14681 2023-06-15 08:11:40.000000 python-negar-1.2.4/negar/virastar.py
-drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-06-15 08:21:46.034626 python-negar-1.2.4/python_negar.egg-info/
--rw-r--r--   0 javad     (1000) javad     (1000)     8548 2023-06-15 08:21:46.000000 python-negar-1.2.4/python_negar.egg-info/PKG-INFO
--rw-r--r--   0 javad     (1000) javad     (1000)      396 2023-06-15 08:21:46.000000 python-negar-1.2.4/python_negar.egg-info/SOURCES.txt
--rw-r--r--   0 javad     (1000) javad     (1000)        1 2023-06-15 08:21:46.000000 python-negar-1.2.4/python_negar.egg-info/dependency_links.txt
--rw-r--r--   0 javad     (1000) javad     (1000)       42 2023-06-15 08:21:46.000000 python-negar-1.2.4/python_negar.egg-info/entry_points.txt
--rw-r--r--   0 javad     (1000) javad     (1000)        6 2023-06-15 08:21:46.000000 python-negar-1.2.4/python_negar.egg-info/requires.txt
--rw-r--r--   0 javad     (1000) javad     (1000)        6 2023-06-15 08:21:46.000000 python-negar-1.2.4/python_negar.egg-info/top_level.txt
--rw-r--r--   0 javad     (1000) javad     (1000)       38 2023-06-15 08:21:46.034626 python-negar-1.2.4/setup.cfg
--rw-r--r--   0 javad     (1000) javad     (1000)     1541 2022-05-30 08:43:57.000000 python-negar-1.2.4/setup.py
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-07-14 10:08:12.206168 python-negar-1.2.5/
+-rw-r--r--   0 javad     (1000) javad     (1000)       41 2022-03-28 12:11:27.000000 python-negar-1.2.5/AUTHORS
+-rw-r--r--   0 javad     (1000) javad     (1000)     6863 2023-07-14 08:12:22.000000 python-negar-1.2.5/Changelog.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)    35147 2022-03-28 12:06:56.000000 python-negar-1.2.5/LICENSE
+-rw-r--r--   0 javad     (1000) javad     (1000)      125 2023-06-15 16:17:35.000000 python-negar-1.2.5/MANIFEST.in
+-rw-r--r--   0 javad     (1000) javad     (1000)     8548 2023-07-14 10:08:12.206168 python-negar-1.2.5/PKG-INFO
+-rw-r--r--   0 javad     (1000) javad     (1000)     7590 2022-09-09 08:02:13.000000 python-negar-1.2.5/README.md
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-07-14 10:08:12.206168 python-negar-1.2.5/negar/
+-rw-r--r--   0 javad     (1000) javad     (1000)       96 2022-03-28 12:34:31.000000 python-negar-1.2.5/negar/__init__.py
+-rw-r--r--   0 javad     (1000) javad     (1000)     5047 2023-07-14 08:12:53.000000 python-negar-1.2.5/negar/constants.py
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-07-14 10:08:12.206168 python-negar-1.2.5/negar/data/
+-rw-r--r--   0 javad     (1000) javad     (1000)        0 2022-03-28 12:06:56.000000 python-negar-1.2.5/negar/data/__init__.py
+-rw-r--r--   0 javad     (1000) javad     (1000)    29312 2022-12-21 09:31:33.000000 python-negar-1.2.5/negar/data/untouchable.dat
+-rw-r--r--   0 javad     (1000) javad     (1000)      346 2023-03-28 18:56:35.000000 python-negar-1.2.5/negar/gui.py
+-rw-r--r--   0 javad     (1000) javad     (1000)    15106 2023-07-14 10:03:34.000000 python-negar-1.2.5/negar/virastar.py
+drwxr-xr-x   0 javad     (1000) javad     (1000)        0 2023-07-14 10:08:12.206168 python-negar-1.2.5/python_negar.egg-info/
+-rw-r--r--   0 javad     (1000) javad     (1000)     8548 2023-07-14 10:08:12.000000 python-negar-1.2.5/python_negar.egg-info/PKG-INFO
+-rw-r--r--   0 javad     (1000) javad     (1000)      396 2023-07-14 10:08:12.000000 python-negar-1.2.5/python_negar.egg-info/SOURCES.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)        1 2023-07-14 10:08:12.000000 python-negar-1.2.5/python_negar.egg-info/dependency_links.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)       42 2023-07-14 10:08:12.000000 python-negar-1.2.5/python_negar.egg-info/entry_points.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)        6 2023-07-14 10:08:12.000000 python-negar-1.2.5/python_negar.egg-info/requires.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)        6 2023-07-14 10:08:12.000000 python-negar-1.2.5/python_negar.egg-info/top_level.txt
+-rw-r--r--   0 javad     (1000) javad     (1000)       38 2023-07-14 10:08:12.206168 python-negar-1.2.5/setup.cfg
+-rw-r--r--   0 javad     (1000) javad     (1000)     1541 2022-05-30 08:43:57.000000 python-negar-1.2.5/setup.py
```

### Comparing `python-negar-1.2.4/Changelog.txt` & `python-negar-1.2.5/Changelog.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+1.2.5 - 2023-07-14
+-- Fix issues with texts that include backslashes as part of their context, such as LaTeX source code.
+
 1.2.4 - 2023-06-15
 -- Fix the issue with multiple ! and ? and extra space after parantheses at the end of line
 
 1.2.2 - 2023-06-13
 -- Fix the issue with the triple dots that was caused by the previous update
 
 1.2.1 - 2023-05-23
```

### Comparing `python-negar-1.2.4/LICENSE` & `python-negar-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python-negar-1.2.4/PKG-INFO` & `python-negar-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-negar
-Version: 1.2.4
+Version: 1.2.5
 Summary: Negar is a spell corrector and Persian text editor
 Home-page: http://github.com/shahinism/python-negar
 Author: Shahin Azad
 Author-email: ishahinism@gmail.com
 Maintainer: Javad Razavian, Alireza Savand
 Maintainer-email: javadr@gmail.com, alireza.savand@gmail.com
 License: GPL
```

### Comparing `python-negar-1.2.4/README.md` & `python-negar-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `python-negar-1.2.4/negar/constants.py` & `python-negar-1.2.5/negar/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pathlib import Path
 
-__version__ = "1.2.4"
+__version__ = "1.2.5"
 
 DATAFILE = Path(__file__).parent.absolute() / "data/untouchable.dat"
 USERFILE = Path.home() / ".python-negar"
 
 INFO = f"""قابلیت های ویراستار ' نگار  ' -- نسخه {__version__} :
 * جایگزینی
 	╛═ خط تیره های پیاپی نظیر (--) و (---) با معادل های استاندارد شان
```

### Comparing `python-negar-1.2.4/negar/data/untouchable.dat` & `python-negar-1.2.5/negar/data/untouchable.dat`

 * *Files identical despite different names*

### Comparing `python-negar-1.2.4/negar/virastar.py` & `python-negar-1.2.5/negar/virastar.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python
 
-import re, regex
+import re
+import regex
 import sys
 import enum
 from pathlib import Path
 sys.path.append(Path(__file__).parent.parent.as_posix()) # https://stackoverflow.com/questions/16981921
 from negar.constants import DATAFILE, USERFILE, URLREGX, INFO
 
 class State(enum.Enum):
@@ -167,25 +168,29 @@
         # regx = re.compile(r"\b(بی|ن?می)‌*([^\[\]\(\)\s]+)") #  \b for words like سهمیه
         regx = regex.compile(r"""
         \b(بی|ن?می)‌*
         ([^\[\]\(\)\s]+)
         (?<!های|هایی|ها|شناس|شناسی|گذار|گذاری)\b
         """, re.VERBOSE) #  \b for words like سهمیه
 
-        wlist = self.text.split(" ")
+        # Replace backslashes with a temporary placeholder
+        text = self.text.replace('\\', 'PN__BACKSLASH__PN')
+        wlist = text.split(" ")
         for word in wlist:
             regx_iter = regx.finditer(word)
             for p in regx_iter:
                 # Checks that the prefix (mi* nemi* bi*) is part a a word or not, like میلاد.
                 if p.group() not in UnTouchable.words:
-                    self.text = re.sub(
+                    text = re.sub(
                         re.escape( p.group() ),
-                        p.group(1) + r"‌" + p.group(2),
-                        self.text
+                        p.group(1) + "\u200c" + p.group(2) ,
+                        text
                     )
+        # Restore the original backslashes
+        self.text = text.replace('PN__BACKSLASH__PN', '\\')
 
     def fix_suffix_spacing(self):
         """Puts ZWNJ between a word and its suffix (*ha[ye] *tar[in])"""
         regx = re.compile(
             r"""\s+
             (تر(ی(ن)?)?
             |[تمش]ان
@@ -219,25 +224,29 @@
             # تر(ی(ن)?)?
             # [تمش]ان|
             # ها(ی(ی|ت|م|ش|تان|شان)?)?|
             شناس(ی)?|
             گذار(ی)?|گزار(ی)?
             )\b""", re.VERBOSE
         )
-        wlist = self.text.split(" ")
+        # Replace backslashes with a temporary placeholder
+        text = self.text.replace('\\', 'PN__BACKSLASH__PN')
+        wlist = text.split(" ")
         for word in wlist:
             regx_iter = regx.finditer(word)
             for p in regx_iter:
                 # Checks that the suffix (tar* haye*) is part of a word or not, like بهتر.
                 if p.group() not in UnTouchable.words:
-                    self.text = re.sub(
+                    text = re.sub(
                         re.escape( p.group() ),
-                        p.group(1) + r"‌" + p.group(2) ,
-                        self.text
+                        p.group(1) + "\u200c" + p.group(2) ,
+                        text
                     )
+        # Restore the original backslashes
+        self.text = text.replace('PN__BACKSLASH__PN', '\\')
 
     def aggressive(self):
         """Reduces Aggressive Punctuation to one sign."""
         if self._cleanup_extra_marks:
             self.text = re.sub(r'(؟){2,}', r'\1', self.text)
             self.text = re.sub(r'(!){2,}', r'\1', self.text)
```

### Comparing `python-negar-1.2.4/python_negar.egg-info/PKG-INFO` & `python-negar-1.2.5/python_negar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-negar
-Version: 1.2.4
+Version: 1.2.5
 Summary: Negar is a spell corrector and Persian text editor
 Home-page: http://github.com/shahinism/python-negar
 Author: Shahin Azad
 Author-email: ishahinism@gmail.com
 Maintainer: Javad Razavian, Alireza Savand
 Maintainer-email: javadr@gmail.com, alireza.savand@gmail.com
 License: GPL
```

### Comparing `python-negar-1.2.4/setup.py` & `python-negar-1.2.5/setup.py`

 * *Files identical despite different names*

