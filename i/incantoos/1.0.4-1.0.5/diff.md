# Comparing `tmp/incantoos-1.0.4.tar.gz` & `tmp/incantoos-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "incantoos-1.0.4.tar", last modified: Tue Jun 27 03:34:33 2023, max compression
+gzip compressed data, was "incantoos-1.0.5.tar", last modified: Thu Jul 13 23:00:54 2023, max compression
```

## Comparing `incantoos-1.0.4.tar` & `incantoos-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:34:33.953731 incantoos-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-27 03:34:22.000000 incantoos-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-27 03:34:33.953731 incantoos-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-27 03:34:22.000000 incantoos-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:34:33.953731 incantoos-1.0.4/incantoos/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-27 03:34:22.000000 incantoos-1.0.4/incantoos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:34:33.953731 incantoos-1.0.4/incantoos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-27 03:34:33.000000 incantoos-1.0.4/incantoos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-27 03:34:33.000000 incantoos-1.0.4/incantoos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 03:34:33.000000 incantoos-1.0.4/incantoos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-27 03:34:33.000000 incantoos-1.0.4/incantoos.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 03:34:33.953731 incantoos-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-27 03:34:22.000000 incantoos-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:00:54.169796 incantoos-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-13 23:00:43.000000 incantoos-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-13 23:00:54.165796 incantoos-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-13 23:00:43.000000 incantoos-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:00:54.165796 incantoos-1.0.5/incantoos/
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-13 23:00:43.000000 incantoos-1.0.5/incantoos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 23:00:54.165796 incantoos-1.0.5/incantoos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-13 23:00:54.000000 incantoos-1.0.5/incantoos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-13 23:00:54.000000 incantoos-1.0.5/incantoos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 23:00:54.000000 incantoos-1.0.5/incantoos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-13 23:00:54.000000 incantoos-1.0.5/incantoos.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 23:00:54.169796 incantoos-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-13 23:00:43.000000 incantoos-1.0.5/setup.py
```

### Comparing `incantoos-1.0.4/LICENSE` & `incantoos-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `incantoos-1.0.4/PKG-INFO` & `incantoos-1.0.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: incantoos
-Version: 1.0.4
+Version: 1.0.5
 Summary: IncantoOS Is a wrapper related to OS functions that can be put into a smaller faster function
 Home-page: https://github.com/NinoTheMeano/incantoos
 Author: NinoTheMeano
 Author-email: ninosdeveloping@gmail.com
 Project-URL: Discord, https://discord.com/users/255125932447236096
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -48,7 +48,15 @@
         Gives you a 8 character ID Ex. ("944b-fq8d")
 
     ids.ranid(amount : int)
         Gives you a randomized id of the specified amount
         
 ```
 
+```py
+    class times
+
+    times.nowtime()
+        Prints the current system time
+    times.utcnowtime()
+        Prints the current system time in UTC
+```
```

### Comparing `incantoos-1.0.4/README.md` & `incantoos-1.0.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -30,7 +30,15 @@
         Gives you a 8 character ID Ex. ("944b-fq8d")
 
     ids.ranid(amount : int)
         Gives you a randomized id of the specified amount
         
 ```
 
+```py
+    class times
+
+    times.nowtime()
+        Prints the current system time
+    times.utcnowtime()
+        Prints the current system time in UTC
+```
```

### Comparing `incantoos-1.0.4/incantoos/__init__.py` & `incantoos-1.0.5/incantoos/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 import datetime, random
 
-version = "1.0.4"
+version = "1.0.5"
 
 class color:
     blue = 0x0076FF
+    lightblue = 0x5790A8
     green = 0x00FF00
     yellow = 0xFFFF00
     red = 0xFF0000
     black = 0x000001
     teal = 0x00ffff
     purple = 0xA020F0
 
-def nowtime():
-    time = datetime.datetime.now()
-    return time
 
 
+class times:
+    def utcnowtime():
+        time = datetime.datetime.utcnow()
+        return time
+    def nowtime():
+        time = datetime.datetime.now()
+        return time
+    
+
+print()
+
 class ids:
     def fourdashfour():
         ranid = ""
         def gettheid(string):
             for ta in range(4):
                 string += random.choice(["a","b","c","d","e","f","g","h","i","k","l","m","n","o","q","r","s","t","v","x","y","z","1","2","3","4","5","6","7","8","9"])
             return string
@@ -30,8 +39,9 @@
     def ranid(amount : int):
         ranid = ""
         def gettheid(string):
             for ta in range(amount):
                 string += random.choice(["a","b","c","d","e","f","g","h","i","k","l","m","n","o","q","r","s","t","v","x","y","z","1","2","3","4","5","6","7","8","9"])
             return string
         ranid = gettheid(ranid)
-        return ranid   
+        return ranid   
+
```

### Comparing `incantoos-1.0.4/incantoos.egg-info/PKG-INFO` & `incantoos-1.0.5/incantoos.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: incantoos
-Version: 1.0.4
+Version: 1.0.5
 Summary: IncantoOS Is a wrapper related to OS functions that can be put into a smaller faster function
 Home-page: https://github.com/NinoTheMeano/incantoos
 Author: NinoTheMeano
 Author-email: ninosdeveloping@gmail.com
 Project-URL: Discord, https://discord.com/users/255125932447236096
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -48,7 +48,15 @@
         Gives you a 8 character ID Ex. ("944b-fq8d")
 
     ids.ranid(amount : int)
         Gives you a randomized id of the specified amount
         
 ```
 
+```py
+    class times
+
+    times.nowtime()
+        Prints the current system time
+    times.utcnowtime()
+        Prints the current system time in UTC
+```
```

### Comparing `incantoos-1.0.4/setup.py` & `incantoos-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup_info = {
     "name": "incantoos",
-    "version": "1.0.4",
+    "version": "1.0.5",
     "author": "NinoTheMeano",
     "author_email": "ninosdeveloping@gmail.com",
     "description": "IncantoOS Is a wrapper related to OS functions that can be put into a smaller faster function",
     "long_description": long_description,
     "long_description_content_type": "text/markdown",
     "url": "https://github.com/NinoTheMeano/incantoos",
     "packages": setuptools.find_packages(),
```

