# Comparing `tmp/ecallisto_ng-0.1.4.tar.gz` & `tmp/ecallisto_ng-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecallisto_ng-0.1.4.tar", last modified: Fri Jul 14 19:02:46 2023, max compression
+gzip compressed data, was "ecallisto_ng-0.1.5.tar", last modified: Fri Jul 14 19:06:02 2023, max compression
```

## Comparing `ecallisto_ng-0.1.4.tar` & `ecallisto_ng-0.1.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-14 19:02:46.870868 ecallisto_ng-0.1.4/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1083 2023-07-06 16:13:05.000000 ecallisto_ng-0.1.4/LICENSE
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3548 2023-07-14 19:02:46.870868 ecallisto_ng-0.1.4/PKG-INFO
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2967 2023-07-11 14:51:23.000000 ecallisto_ng-0.1.4/README.md
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      858 2023-07-14 19:02:25.000000 ecallisto_ng-0.1.4/pyproject.toml
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       38 2023-07-14 19:02:46.870868 ecallisto_ng-0.1.4/setup.cfg
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-14 19:02:46.860868 ecallisto_ng-0.1.4/src/
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-14 19:02:46.860868 ecallisto_ng-0.1.4/src/ecallisto_ng/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 17:35:07.000000 ecallisto_ng-0.1.4/src/ecallisto_ng/__init__.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-14 19:02:46.870868 ecallisto_ng-0.1.4/src/ecallisto_ng/data_fetching/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:51.000000 ecallisto_ng-0.1.4/src/ecallisto_ng/data_fetching/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     6006 2023-07-14 19:01:04.000000 ecallisto_ng-0.1.4/src/ecallisto_ng/data_fetching/get_data.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2006 2023-07-13 17:59:20.000000 ecallisto_ng-0.1.4/src/ecallisto_ng/data_fetching/get_information.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-14 19:02:46.870868 ecallisto_ng-0.1.4/src/ecallisto_ng/data_processing/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:54.000000 ecallisto_ng-0.1.4/src/ecallisto_ng/data_processing/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     5256 2023-07-11 08:45:15.000000 ecallisto_ng-0.1.4/src/ecallisto_ng/data_processing/utils.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-14 19:02:46.870868 ecallisto_ng-0.1.4/src/ecallisto_ng/plotting/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:40:01.000000 ecallisto_ng-0.1.4/src/ecallisto_ng/plotting/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2425 2023-07-10 17:56:33.000000 ecallisto_ng-0.1.4/src/ecallisto_ng/plotting/utils.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-14 19:02:46.870868 ecallisto_ng-0.1.4/src/ecallisto_ng.egg-info/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3548 2023-07-14 19:02:46.000000 ecallisto_ng-0.1.4/src/ecallisto_ng.egg-info/PKG-INFO
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      556 2023-07-14 19:02:46.000000 ecallisto_ng-0.1.4/src/ecallisto_ng.egg-info/SOURCES.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        1 2023-07-14 19:02:46.000000 ecallisto_ng-0.1.4/src/ecallisto_ng.egg-info/dependency_links.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      129 2023-07-14 19:02:46.000000 ecallisto_ng-0.1.4/src/ecallisto_ng.egg-info/requires.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       13 2023-07-14 19:02:46.000000 ecallisto_ng-0.1.4/src/ecallisto_ng.egg-info/top_level.txt
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-14 19:06:01.999316 ecallisto_ng-0.1.5/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1083 2023-07-06 16:13:05.000000 ecallisto_ng-0.1.5/LICENSE
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3548 2023-07-14 19:06:01.999316 ecallisto_ng-0.1.5/PKG-INFO
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2967 2023-07-11 14:51:23.000000 ecallisto_ng-0.1.5/README.md
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      858 2023-07-14 19:05:51.000000 ecallisto_ng-0.1.5/pyproject.toml
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)       38 2023-07-14 19:06:01.999316 ecallisto_ng-0.1.5/setup.cfg
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-14 19:06:01.979315 ecallisto_ng-0.1.5/src/
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-14 19:06:01.999316 ecallisto_ng-0.1.5/src/ecallisto_ng/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 17:35:07.000000 ecallisto_ng-0.1.5/src/ecallisto_ng/__init__.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-14 19:06:01.999316 ecallisto_ng-0.1.5/src/ecallisto_ng/data_fetching/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:51.000000 ecallisto_ng-0.1.5/src/ecallisto_ng/data_fetching/__init__.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     6006 2023-07-14 19:01:04.000000 ecallisto_ng-0.1.5/src/ecallisto_ng/data_fetching/get_data.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2006 2023-07-13 17:59:20.000000 ecallisto_ng-0.1.5/src/ecallisto_ng/data_fetching/get_information.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-14 19:06:01.999316 ecallisto_ng-0.1.5/src/ecallisto_ng/data_processing/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:54.000000 ecallisto_ng-0.1.5/src/ecallisto_ng/data_processing/__init__.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     5256 2023-07-11 08:45:15.000000 ecallisto_ng-0.1.5/src/ecallisto_ng/data_processing/utils.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-14 19:06:01.999316 ecallisto_ng-0.1.5/src/ecallisto_ng/plotting/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:40:01.000000 ecallisto_ng-0.1.5/src/ecallisto_ng/plotting/__init__.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2425 2023-07-10 17:56:33.000000 ecallisto_ng-0.1.5/src/ecallisto_ng/plotting/utils.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-14 19:06:01.999316 ecallisto_ng-0.1.5/src/ecallisto_ng.egg-info/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3548 2023-07-14 19:06:01.000000 ecallisto_ng-0.1.5/src/ecallisto_ng.egg-info/PKG-INFO
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      556 2023-07-14 19:06:01.000000 ecallisto_ng-0.1.5/src/ecallisto_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        1 2023-07-14 19:06:01.000000 ecallisto_ng-0.1.5/src/ecallisto_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      129 2023-07-14 19:06:01.000000 ecallisto_ng-0.1.5/src/ecallisto_ng.egg-info/requires.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)       13 2023-07-14 19:06:01.000000 ecallisto_ng-0.1.5/src/ecallisto_ng.egg-info/top_level.txt
```

### Comparing `ecallisto_ng-0.1.4/LICENSE` & `ecallisto_ng-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.1.4/PKG-INFO` & `ecallisto_ng-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecallisto_ng
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API.
 Author-email: Vincenzo Timmel <vincenzo.timmel@fhnw.ch>
 Project-URL: Homepage, https://github.com/i4Ds/ecallisto_ng
 Project-URL: Bug Tracker, https://github.com/i4Ds/ecallisto_ng/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ecallisto_ng-0.1.4/README.md` & `ecallisto_ng-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.1.4/pyproject.toml` & `ecallisto_ng-0.1.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ecallisto_ng"
-version = "0.1.4"
+version = "0.1.5"
 authors = [{name = "Vincenzo Timmel", email = "vincenzo.timmel@fhnw.ch"}]
 description = "A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API."
 readme = "README.md"
 
 requires-python = ">=3.9"
 
 classifiers = [
```

### Comparing `ecallisto_ng-0.1.4/src/ecallisto_ng/data_fetching/get_data.py` & `ecallisto_ng-0.1.5/src/ecallisto_ng/data_fetching/get_data.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.1.4/src/ecallisto_ng/data_fetching/get_information.py` & `ecallisto_ng-0.1.5/src/ecallisto_ng/data_fetching/get_information.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.1.4/src/ecallisto_ng/data_processing/utils.py` & `ecallisto_ng-0.1.5/src/ecallisto_ng/data_processing/utils.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.1.4/src/ecallisto_ng/plotting/utils.py` & `ecallisto_ng-0.1.5/src/ecallisto_ng/plotting/utils.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.1.4/src/ecallisto_ng.egg-info/PKG-INFO` & `ecallisto_ng-0.1.5/src/ecallisto_ng.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecallisto-ng
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API.
 Author-email: Vincenzo Timmel <vincenzo.timmel@fhnw.ch>
 Project-URL: Homepage, https://github.com/i4Ds/ecallisto_ng
 Project-URL: Bug Tracker, https://github.com/i4Ds/ecallisto_ng/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ecallisto_ng-0.1.4/src/ecallisto_ng.egg-info/SOURCES.txt` & `ecallisto_ng-0.1.5/src/ecallisto_ng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

