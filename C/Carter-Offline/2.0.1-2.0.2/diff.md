# Comparing `tmp/Carter-Offline-2.0.1.tar.gz` & `tmp/Carter-Offline-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Carter-Offline-2.0.1.tar", last modified: Fri Jul 14 15:30:13 2023, max compression
+gzip compressed data, was "Carter-Offline-2.0.2.tar", last modified: Fri Jul 14 15:35:56 2023, max compression
```

## Comparing `Carter-Offline-2.0.1.tar` & `Carter-Offline-2.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-14 15:30:13.015148 Carter-Offline-2.0.1/
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-14 15:30:13.011751 Carter-Offline-2.0.1/CarterOffline/
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-14 15:30:13.012129 Carter-Offline-2.0.1/CarterOffline/Carter-Offline-SubFolder/
--rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:07:05.000000 Carter-Offline-2.0.1/CarterOffline/Carter-Offline-SubFolder/JanexSub.py
--rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:20:34.000000 Carter-Offline-2.0.1/CarterOffline/Carter-Offline-SubFolder/__init__.py
--rw-r--r--   0 cipher     (501) staff       (20)     5868 2023-07-14 14:47:21.000000 Carter-Offline-2.0.1/CarterOffline/__init__.py
--rw-r--r--   0 cipher     (501) staff       (20)      260 2023-07-07 20:07:57.000000 Carter-Offline-2.0.1/CarterOffline/chat.py
--rw-r--r--   0 cipher     (501) staff       (20)        1 2023-07-09 19:53:02.000000 Carter-Offline-2.0.1/CarterOffline/main.py
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-14 15:30:13.014815 Carter-Offline-2.0.1/Carter_Offline.egg-info/
--rw-r--r--   0 cipher     (501) staff       (20)     1890 2023-07-14 15:30:12.000000 Carter-Offline-2.0.1/Carter_Offline.egg-info/PKG-INFO
--rw-r--r--   0 cipher     (501) staff       (20)      387 2023-07-14 15:30:12.000000 Carter-Offline-2.0.1/Carter_Offline.egg-info/SOURCES.txt
--rw-r--r--   0 cipher     (501) staff       (20)        1 2023-07-14 15:30:12.000000 Carter-Offline-2.0.1/Carter_Offline.egg-info/dependency_links.txt
--rw-r--r--   0 cipher     (501) staff       (20)       22 2023-07-14 15:30:12.000000 Carter-Offline-2.0.1/Carter_Offline.egg-info/requires.txt
--rw-r--r--   0 cipher     (501) staff       (20)       14 2023-07-14 15:30:12.000000 Carter-Offline-2.0.1/Carter_Offline.egg-info/top_level.txt
--rw-r--r--   0 cipher     (501) staff       (20)     2950 2023-07-07 12:33:15.000000 Carter-Offline-2.0.1/LICENSE
--rw-r--r--   0 cipher     (501) staff       (20)     1890 2023-07-14 15:30:13.015017 Carter-Offline-2.0.1/PKG-INFO
--rw-r--r--   0 cipher     (501) staff       (20)     1503 2023-07-14 15:28:28.000000 Carter-Offline-2.0.1/README.md
--rw-r--r--   0 cipher     (501) staff       (20)       38 2023-07-14 15:30:13.015183 Carter-Offline-2.0.1/setup.cfg
--rw-r--r--   0 cipher     (501) staff       (20)     1322 2023-07-14 15:29:45.000000 Carter-Offline-2.0.1/setup.py
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-14 15:35:56.280927 Carter-Offline-2.0.2/
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-14 15:35:56.275361 Carter-Offline-2.0.2/CarterOffline/
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-14 15:35:56.275747 Carter-Offline-2.0.2/CarterOffline/Carter-Offline-SubFolder/
+-rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:07:05.000000 Carter-Offline-2.0.2/CarterOffline/Carter-Offline-SubFolder/JanexSub.py
+-rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:20:34.000000 Carter-Offline-2.0.2/CarterOffline/Carter-Offline-SubFolder/__init__.py
+-rw-r--r--   0 cipher     (501) staff       (20)     5868 2023-07-14 14:47:21.000000 Carter-Offline-2.0.2/CarterOffline/__init__.py
+-rw-r--r--   0 cipher     (501) staff       (20)      260 2023-07-07 20:07:57.000000 Carter-Offline-2.0.2/CarterOffline/chat.py
+-rw-r--r--   0 cipher     (501) staff       (20)        1 2023-07-09 19:53:02.000000 Carter-Offline-2.0.2/CarterOffline/main.py
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-14 15:35:56.280629 Carter-Offline-2.0.2/Carter_Offline.egg-info/
+-rw-r--r--   0 cipher     (501) staff       (20)     1891 2023-07-14 15:35:56.000000 Carter-Offline-2.0.2/Carter_Offline.egg-info/PKG-INFO
+-rw-r--r--   0 cipher     (501) staff       (20)      387 2023-07-14 15:35:56.000000 Carter-Offline-2.0.2/Carter_Offline.egg-info/SOURCES.txt
+-rw-r--r--   0 cipher     (501) staff       (20)        1 2023-07-14 15:35:56.000000 Carter-Offline-2.0.2/Carter_Offline.egg-info/dependency_links.txt
+-rw-r--r--   0 cipher     (501) staff       (20)       22 2023-07-14 15:35:56.000000 Carter-Offline-2.0.2/Carter_Offline.egg-info/requires.txt
+-rw-r--r--   0 cipher     (501) staff       (20)       14 2023-07-14 15:35:56.000000 Carter-Offline-2.0.2/Carter_Offline.egg-info/top_level.txt
+-rw-r--r--   0 cipher     (501) staff       (20)     2950 2023-07-07 12:33:15.000000 Carter-Offline-2.0.2/LICENSE
+-rw-r--r--   0 cipher     (501) staff       (20)     1891 2023-07-14 15:35:56.280809 Carter-Offline-2.0.2/PKG-INFO
+-rw-r--r--   0 cipher     (501) staff       (20)     1504 2023-07-14 15:34:56.000000 Carter-Offline-2.0.2/README.md
+-rw-r--r--   0 cipher     (501) staff       (20)       38 2023-07-14 15:35:56.280958 Carter-Offline-2.0.2/setup.cfg
+-rw-r--r--   0 cipher     (501) staff       (20)     1322 2023-07-14 15:35:33.000000 Carter-Offline-2.0.2/setup.py
```

### Comparing `Carter-Offline-2.0.1/CarterOffline/__init__.py` & `Carter-Offline-2.0.2/CarterOffline/__init__.py`

 * *Files identical despite different names*

### Comparing `Carter-Offline-2.0.1/Carter_Offline.egg-info/PKG-INFO` & `Carter-Offline-2.0.2/Carter_Offline.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Carter-Offline
-Version: 2.0.1
+Version: 2.0.2
 Home-page: https://github.com/Cipher58
 Download-URL: https://github.com/Cipher58/Carter-Offline/
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -27,15 +27,15 @@
 <h3> How to use </h3>
 
 <h5> Adding to your project </h5>
 
 Firstly, you'll need to install the library using the Python pip package manager.
 
 ```
-python3 -m pip install CarterOffline
+python3 -m pip install Carter-Offline
 ```
 Secondly, you need to import the library into your Python script.
 
 ```
 from CarterOffline import *
 ```
```

### Comparing `Carter-Offline-2.0.1/LICENSE` & `Carter-Offline-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Carter-Offline-2.0.1/PKG-INFO` & `Carter-Offline-2.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Carter-Offline
-Version: 2.0.1
+Version: 2.0.2
 Home-page: https://github.com/Cipher58
 Download-URL: https://github.com/Cipher58/Carter-Offline/
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -27,15 +27,15 @@
 <h3> How to use </h3>
 
 <h5> Adding to your project </h5>
 
 Firstly, you'll need to install the library using the Python pip package manager.
 
 ```
-python3 -m pip install CarterOffline
+python3 -m pip install Carter-Offline
 ```
 Secondly, you need to import the library into your Python script.
 
 ```
 from CarterOffline import *
 ```
```

### Comparing `Carter-Offline-2.0.1/README.md` & `Carter-Offline-2.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 <h3> How to use </h3>
 
 <h5> Adding to your project </h5>
 
 Firstly, you'll need to install the library using the Python pip package manager.
 
 ```
-python3 -m pip install CarterOffline
+python3 -m pip install Carter-Offline
 ```
 Secondly, you need to import the library into your Python script.
 
 ```
 from CarterOffline import *
 ```
```

### Comparing `Carter-Offline-2.0.1/setup.py` & `Carter-Offline-2.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setuptools.setup(
     # Here is the module name.
     name="Carter-Offline",
 
     # version of the module
-    version="2.0.1",
+    version="2.0.2",
 
     # Name of Author
     author="Cipher58",
 
     download_url = 'https://github.com/Cipher58/Carter-Offline/',
 
     # your Email address
```

