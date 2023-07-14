# Comparing `tmp/pythontk-0.6.8.tar.gz` & `tmp/pythontk-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythontk-0.6.8.tar", last modified: Mon Jul  3 15:09:52 2023, max compression
+gzip compressed data, was "pythontk-0.6.9.tar", last modified: Fri Jul 14 18:02:00 2023, max compression
```

## Comparing `pythontk-0.6.8.tar` & `pythontk-0.6.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 15:09:52.617932 pythontk-0.6.8/
--rw-rw-rw-   0        0        0     1093 2023-03-28 23:38:48.000000 pythontk-0.6.8/LICENSE
--rw-rw-rw-   0        0        0     1155 2023-07-03 15:09:52.616927 pythontk-0.6.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-03 15:09:52.592320 pythontk-0.6.8/pythontk/
--rw-rw-rw-   0        0        0     7133 2023-07-03 15:09:47.000000 pythontk-0.6.8/pythontk/__init__.py
--rw-rw-rw-   0        0        0    28018 2023-07-03 14:39:57.000000 pythontk-0.6.8/pythontk/file_utils.py
--rw-rw-rw-   0        0        0    29291 2023-06-27 22:55:30.000000 pythontk-0.6.8/pythontk/img_utils.py
--rw-rw-rw-   0        0        0    29221 2023-06-24 12:29:41.000000 pythontk-0.6.8/pythontk/img_utils.py.bak
--rw-rw-rw-   0        0        0    16318 2023-06-30 22:19:51.000000 pythontk-0.6.8/pythontk/iter_utils.py
--rw-rw-rw-   0        0        0    18070 2023-06-27 22:52:04.000000 pythontk-0.6.8/pythontk/math_utils.py
--rw-rw-rw-   0        0        0    24621 2023-06-27 23:08:47.000000 pythontk-0.6.8/pythontk/str_utils.py
--rw-rw-rw-   0        0        0    11206 2023-06-27 22:12:52.000000 pythontk-0.6.8/pythontk/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-03 15:09:52.616927 pythontk-0.6.8/pythontk.egg-info/
--rw-rw-rw-   0        0        0     1155 2023-07-03 15:09:52.000000 pythontk-0.6.8/pythontk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1287 2023-05-20 13:28:19.000000 pythontk-0.6.8/pythontk.egg-info/PKG-INFO.bak
--rw-rw-rw-   0        0        0      387 2023-07-03 15:09:52.000000 pythontk-0.6.8/pythontk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      265 2023-05-07 12:53:37.000000 pythontk-0.6.8/pythontk.egg-info/SOURCES.txt.bak
--rw-rw-rw-   0        0        0        1 2023-07-03 15:09:52.000000 pythontk-0.6.8/pythontk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-03 15:09:52.000000 pythontk-0.6.8/pythontk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 15:09:52.617932 pythontk-0.6.8/setup.cfg
--rw-rw-rw-   0        0        0     1383 2023-06-28 23:01:31.000000 pythontk-0.6.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 18:02:00.054506 pythontk-0.6.9/
+-rw-rw-rw-   0        0        0     1093 2023-03-28 23:38:48.000000 pythontk-0.6.9/LICENSE
+-rw-rw-rw-   0        0        0     1928 2023-07-14 18:02:00.053499 pythontk-0.6.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-14 18:02:00.019356 pythontk-0.6.9/pythontk/
+-rw-rw-rw-   0        0        0     7133 2023-07-14 18:01:57.000000 pythontk-0.6.9/pythontk/__init__.py
+-rw-rw-rw-   0        0        0    11174 2023-07-03 18:15:52.000000 pythontk-0.6.9/pythontk/core_utils.py
+-rw-rw-rw-   0        0        0    28733 2023-07-14 17:25:19.000000 pythontk-0.6.9/pythontk/file_utils.py
+-rw-rw-rw-   0        0        0    29304 2023-07-05 14:08:01.000000 pythontk-0.6.9/pythontk/img_utils.py
+-rw-rw-rw-   0        0        0    29221 2023-06-24 12:29:41.000000 pythontk-0.6.9/pythontk/img_utils.py.bak
+-rw-rw-rw-   0        0        0    16263 2023-07-03 17:30:24.000000 pythontk-0.6.9/pythontk/iter_utils.py
+-rw-rw-rw-   0        0        0    18087 2023-07-05 14:07:54.000000 pythontk-0.6.9/pythontk/math_utils.py
+-rw-rw-rw-   0        0        0    24642 2023-07-05 14:07:42.000000 pythontk-0.6.9/pythontk/str_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-14 18:02:00.051632 pythontk-0.6.9/pythontk.egg-info/
+-rw-rw-rw-   0        0        0     1928 2023-07-14 18:01:59.000000 pythontk-0.6.9/pythontk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1287 2023-05-20 13:28:19.000000 pythontk-0.6.9/pythontk.egg-info/PKG-INFO.bak
+-rw-rw-rw-   0        0        0      392 2023-07-14 18:01:59.000000 pythontk-0.6.9/pythontk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      265 2023-05-07 12:53:37.000000 pythontk-0.6.9/pythontk.egg-info/SOURCES.txt.bak
+-rw-rw-rw-   0        0        0        1 2023-07-14 18:01:59.000000 pythontk-0.6.9/pythontk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-14 18:01:59.000000 pythontk-0.6.9/pythontk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 18:02:00.054506 pythontk-0.6.9/setup.cfg
+-rw-rw-rw-   0        0        0     1383 2023-06-28 23:01:31.000000 pythontk-0.6.9/setup.py
```

### Comparing `pythontk-0.6.8/LICENSE` & `pythontk-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pythontk-0.6.8/pythontk/__init__.py` & `pythontk-0.6.9/pythontk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 import inspect
 import importlib
 import pkgutil
 
 
 __package__ = "pythontk"
-__version__ = '0.6.8'
+__version__ = '0.6.9'
 
 
 # Define dictionaries to map class names, method names, and class method names to their respective modules
 CLASS_TO_MODULE = {}
 METHOD_TO_MODULE = {}
 CLASS_METHOD_TO_MODULE = {}
```

### Comparing `pythontk-0.6.8/pythontk/file_utils.py` & `pythontk-0.6.9/pythontk/file_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 import os
 import re
 import json
 import traceback
 
 # from this package:
-from pythontk.utils import Utils
+from pythontk.core_utils import CoreUtils
 from pythontk.iter_utils import IterUtils
 from pythontk.str_utils import StrUtils
 
 
 class FileUtils:
     """ """
 
@@ -285,15 +285,15 @@
             return os.path.abspath(filepath)
         elif filepath:
             return os.path.abspath(os.path.dirname(filepath))
         else:
             return None
 
     @staticmethod
-    @Utils.listify(threading=True)
+    @CoreUtils.listify(threading=True)
     def format_path(p, section="", replace=""):
         """Format a given filepath(s).
         When a section arg is given, the correlating section of the string will be returned.
         If a replace arg is given, the stated section will be replaced by the given value.
 
         Parameters:
             p (str/list): The filepath(s) to be formatted.
@@ -410,15 +410,15 @@
                         for base in cls.bases:
                             # Add the class name and file path to the dictionary
                             widget_classes[cls.name] = os.path.join(dir_path, filename)
 
         return widget_classes
 
     @classmethod
-    @Utils.listify(threading=True)
+    @CoreUtils.listify(threading=True)
     def time_stamp(cls, filepath, stamp="%m-%d-%Y  %H:%M"):
         """Attach or detach a modified timestamp and date to/from a given file path.
 
         Parameters:
             filepath (str): The full path to a file. ie. 'C:/Windows/Temp/__AUTO-SAVE__untitled.0001.mb'
             stamp (str): The time stamp format.
 
@@ -451,38 +451,39 @@
     @classmethod
     def update_version(
         cls,
         filepath: str,
         change: str = "increment",
         version_part: str = "patch",
         max_version_parts: tuple = (9, 9),
+        version_regex: str = r"__version__\s*=\s*['\"](\d+)\.(\d+)\.(\d+)['\"]",
     ) -> None:
         """This function updates the version number in a text file depending on its state.
-        The version number is defined as a line in the following format: __version__ = "0.0.0"
-        The version number is represented as a string in the format 'x.y.z', where x, y, and z are integers.
+        The version number is represented as a string in the format 'x.y.z', where x, y, and z are integers and it matches the provided regex pattern.
 
         Parameters:
             filepath (str): The path to the text file containing the version number.
             change (str, optional): The type of change, either 'increment' or 'decrement'. Defaults to 'increment'.
             version_part (str, optional): The part of the version number to update, either 'major', 'minor', or 'patch'. Defaults to 'patch'.
             max_version_parts (tuple, optional): A tuple containing the maximum values for the minor and patch version parts. Defaults to (9, 9).
-
+            version_regex (str, optional): A regex pattern that defines the format of the version line in the file.
+                    The pattern should have three groups each representing major, minor, and patch versions respectively.
         Returns:
-            (str): The new version number.
+            str: The new version number. If the function could not find a version number that matches the provided pattern in the file, it will print an error message and return an empty string.
         """
         import re
 
         lines = cls.get_file_contents(filepath, as_list=True)
 
-        version_pattern = re.compile(r"__version__\s*=\s*['\"](\d+)\.(\d+)\.(\d+)['\"]")
+        version_pattern = re.compile(version_regex)
         max_minor, max_patch = max_version_parts
 
         version = ""
         for i, line in enumerate(lines):
-            match = version_pattern.match(line)
+            match = version_pattern.search(line)
             if match:
                 major, minor, patch = map(int, match.groups())
 
                 if version_part == "patch":
                     if change == "increment":
                         patch = (patch + 1) % (max_patch + 1)
                         if patch == 0:
@@ -524,15 +525,24 @@
                         )
                 else:
                     raise ValueError(
                         "Invalid version_part parameter. Use either 'major', 'minor', or 'patch'."
                     )
 
                 version = f"{major}.{minor}.{patch}"
-                lines[i] = f"__version__ = '{version}'\n"
+
+                # Preserve the original format of the line
+                new_line = re.sub(
+                    version_regex,
+                    lambda m: m.group(0).replace(
+                        m.group(1) + "." + m.group(2) + "." + m.group(3), version
+                    ),
+                    line,
+                )
+                lines[i] = new_line
                 break
 
         cls.write_to_file(filepath, lines)
         if not version:
             print(
                 f'# Error: No version in the format: __version__ = "0.0.0" found in {filepath}'
             )
```

### Comparing `pythontk-0.6.8/pythontk/img_utils.py` & `pythontk-0.6.9/pythontk/img_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     print("{}\n # Error: {} #".format(__file__, error))
 try:
     from PySide2 import QtWidgets
 except ImportError as error:
     print("{}\n # Error: {} #".format(__file__, error))
 
 # from this package:
-from pythontk.utils import Utils
+from pythontk.core_utils import CoreUtils
 from pythontk.file_utils import FileUtils
 from pythontk.iter_utils import IterUtils
 
 
 class ImgUtils:
     """Helper methods for working with image file formats."""
 
@@ -459,15 +459,15 @@
         name = name.removesuffix(typ)
         filepath = "{}/{}{}.{}".format(output_dir, name, new_type, ext)
         inverted_image.save(filepath)
 
         return filepath
 
     @classmethod
-    @Utils.listify(threading=True)
+    @CoreUtils.listify(threading=True)
     def create_mask(
         cls, image, mask, background=(0, 0, 0, 255), foreground=(255, 255, 255, 255)
     ):
         """Create mask(s) from the given image(s).
 
         Parameters:
                 images (str/obj/list): Image(s) or path(s) to an image.
```

### Comparing `pythontk-0.6.8/pythontk/img_utils.py.bak` & `pythontk-0.6.9/pythontk/img_utils.py.bak`

 * *Files identical despite different names*

### Comparing `pythontk-0.6.8/pythontk/iter_utils.py` & `pythontk-0.6.9/pythontk/iter_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -386,10 +386,7 @@
 
 if __name__ == "__main__":
     pass
 
 # --------------------------------------------------------------------------------------------
 # Notes
 # --------------------------------------------------------------------------------------------
-
-
-# Deprecated ------------------------------------
```

### Comparing `pythontk-0.6.8/pythontk/math_utils.py` & `pythontk-0.6.9/pythontk/math_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # !/usr/bin/python
 # coding=utf-8
 from typing import List, Tuple
 
 # from this package:
-from pythontk.utils import Utils
+from pythontk.core_utils import CoreUtils
 
 
 class MathUtils:
     """ """
 
     @staticmethod
-    @Utils.listify(threading=True)
+    @CoreUtils.listify(threading=True)
     def move_decimal_point(num, places):
         """Move the decimal place in a given number.
 
         Parameters:
             num (int/float): The number in which you are modifying.
             places (int): The number of decimal places to move.
 
@@ -51,15 +51,15 @@
 
         Example:
             get_vector_from_two_points([1, 2, 3], [1, 1, -1]) #returns: (0, -1, -4)
         """
         return (b[0] - a[0], b[1] - a[1], b[2] - a[2])
 
     @staticmethod
-    @Utils.listify(threading=True)
+    @CoreUtils.listify(threading=True)
     def clamp(n=0.0, minimum=0.0, maximum=1.0):
         """Clamps the value x between min and max.
 
         Parameters:
             n (float)(tuple): The numeric value to clamp.
             minimum (float): Clamp min value.
             maximum (float): Clamp max value.
```

### Comparing `pythontk-0.6.8/pythontk/str_utils.py` & `pythontk-0.6.9/pythontk/str_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # !/usr/bin/python
 # coding=utf-8
 # from this package:
-from pythontk.utils import Utils
+from pythontk.core_utils import CoreUtils
 from pythontk.iter_utils import IterUtils
 
 
 class StrUtils:
     """ """
 
     @staticmethod
-    @Utils.listify(threading=True)
+    @CoreUtils.listify(threading=True)
     def set_case(string, case="title"):
         """Format the given string(s) in the given case.
 
         Parameters:
             string (str/list): The string(s) to format.
             case (str): The desired return case. Accepts all python case operators.
                     valid: 'upper', 'lower', 'capitalize' (default), 'swapcase', 'title', 'pascal', 'camel', None.
@@ -183,15 +183,15 @@
                 return True
             return False
 
         matches = [item for item in hierarchy_items if filter_items(item)]
         return sorted(matches, key=lambda x: len(x), reverse=reverse)
 
     @staticmethod
-    @Utils.listify(threading=True)
+    @CoreUtils.listify(threading=True)
     def split_at_chars(string, chars="|", occurrence=-1):
         """Split a string containing the given chars at the given occurrence and return
         a two element tuple containing both halves.
 
         Parameters:
             strings (str/list): The string(s) to operate on.
             chars (str): The chars to split at.
@@ -269,15 +269,15 @@
 
         if count is not None:
             return str(new).join(string.rsplit(old, count))
         else:
             return str(new).join(string.rsplit(old))
 
     @staticmethod
-    @Utils.listify(threading=True)
+    @CoreUtils.listify(threading=True)
     def truncate(string, length=75, beginning=True, insert=".."):
         """Shorten the given string to the given length.
         An ellipsis will be added to the section trimmed.
 
         Parameters:
             length (int): The maximum allowed length before trunicating.
             beginning (bool): Trim starting chars, else; ending.
```

### Comparing `pythontk-0.6.8/pythontk/utils.py` & `pythontk-0.6.9/pythontk/core_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import collections.abc
 from typing import Any, Callable
 
 # from this package:
 from pythontk.iter_utils import IterUtils
 
 
-class Utils:
+class CoreUtils:
     """ """
 
     @staticmethod
     def cached_property(func: Callable) -> Any:
         """Decorator that converts a method with a single self argument into a property
         that runs the method only once and stores the result, returning the stored
         result on subsequent accesses.
@@ -37,15 +37,15 @@
             return getattr(self, attr_name)
 
         return _cached_property
 
     @staticmethod
     def listify(func=None, arg_name=None, threading=False):
         if func is None:
-            return lambda func: Utils.listify(func, arg_name=arg_name)
+            return lambda func: CoreUtils.listify(func, arg_name=arg_name)
 
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
             func_args = inspect.getfullargspec(func).args
             if "self" in func_args or "cls" in func_args:
                 func_args = func_args[1:]  # skip 'self' or 'cls' argument for methods
 
@@ -287,10 +287,7 @@
 
 if __name__ == "__main__":
     pass
 
 # -----------------------------------------------------------------------------
 # Notes
 # -----------------------------------------------------------------------------
-
-
-# deprecated ---------------------
```

### Comparing `pythontk-0.6.8/pythontk.egg-info/PKG-INFO.bak` & `pythontk-0.6.9/pythontk.egg-info/PKG-INFO.bak`

 * *Files identical despite different names*

### Comparing `pythontk-0.6.8/setup.py` & `pythontk-0.6.9/setup.py`

 * *Files identical despite different names*

