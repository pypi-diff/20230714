# Comparing `tmp/ecallisto_ng-0.1.2.tar.gz` & `tmp/ecallisto_ng-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecallisto_ng-0.1.2.tar", last modified: Thu Jul 13 17:59:51 2023, max compression
+gzip compressed data, was "ecallisto_ng-0.1.3.tar", last modified: Thu Jul 13 18:04:42 2023, max compression
```

## Comparing `ecallisto_ng-0.1.2.tar` & `ecallisto_ng-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 17:59:51.205465 ecallisto_ng-0.1.2/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1083 2023-07-06 16:13:05.000000 ecallisto_ng-0.1.2/LICENSE
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3548 2023-07-13 17:59:51.205465 ecallisto_ng-0.1.2/PKG-INFO
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2967 2023-07-11 14:51:23.000000 ecallisto_ng-0.1.2/README.md
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      836 2023-07-13 17:59:27.000000 ecallisto_ng-0.1.2/pyproject.toml
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       38 2023-07-13 17:59:51.205465 ecallisto_ng-0.1.2/setup.cfg
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 17:59:51.183798 ecallisto_ng-0.1.2/src/
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 17:59:51.194631 ecallisto_ng-0.1.2/src/ecallisto_ng/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 17:35:07.000000 ecallisto_ng-0.1.2/src/ecallisto_ng/__init__.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 17:59:51.205465 ecallisto_ng-0.1.2/src/ecallisto_ng/data_fetching/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:51.000000 ecallisto_ng-0.1.2/src/ecallisto_ng/data_fetching/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     6470 2023-07-13 08:29:09.000000 ecallisto_ng-0.1.2/src/ecallisto_ng/data_fetching/get_data.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2006 2023-07-13 17:59:20.000000 ecallisto_ng-0.1.2/src/ecallisto_ng/data_fetching/get_information.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 17:59:51.205465 ecallisto_ng-0.1.2/src/ecallisto_ng/data_processing/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:54.000000 ecallisto_ng-0.1.2/src/ecallisto_ng/data_processing/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     5256 2023-07-11 08:45:15.000000 ecallisto_ng-0.1.2/src/ecallisto_ng/data_processing/utils.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 17:59:51.205465 ecallisto_ng-0.1.2/src/ecallisto_ng/plotting/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:40:01.000000 ecallisto_ng-0.1.2/src/ecallisto_ng/plotting/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2425 2023-07-10 17:56:33.000000 ecallisto_ng-0.1.2/src/ecallisto_ng/plotting/utils.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 17:59:51.194631 ecallisto_ng-0.1.2/src/ecallisto_ng.egg-info/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3548 2023-07-13 17:59:51.000000 ecallisto_ng-0.1.2/src/ecallisto_ng.egg-info/PKG-INFO
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      556 2023-07-13 17:59:51.000000 ecallisto_ng-0.1.2/src/ecallisto_ng.egg-info/SOURCES.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        1 2023-07-13 17:59:51.000000 ecallisto_ng-0.1.2/src/ecallisto_ng.egg-info/dependency_links.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      113 2023-07-13 17:59:51.000000 ecallisto_ng-0.1.2/src/ecallisto_ng.egg-info/requires.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       13 2023-07-13 17:59:51.000000 ecallisto_ng-0.1.2/src/ecallisto_ng.egg-info/top_level.txt
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 18:04:42.362043 ecallisto_ng-0.1.3/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1083 2023-07-06 16:13:05.000000 ecallisto_ng-0.1.3/LICENSE
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3548 2023-07-13 18:04:42.362043 ecallisto_ng-0.1.3/PKG-INFO
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2967 2023-07-11 14:51:23.000000 ecallisto_ng-0.1.3/README.md
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      836 2023-07-13 18:04:24.000000 ecallisto_ng-0.1.3/pyproject.toml
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)       38 2023-07-13 18:04:42.362043 ecallisto_ng-0.1.3/setup.cfg
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 18:04:42.340377 ecallisto_ng-0.1.3/src/
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 18:04:42.351210 ecallisto_ng-0.1.3/src/ecallisto_ng/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 17:35:07.000000 ecallisto_ng-0.1.3/src/ecallisto_ng/__init__.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 18:04:42.351210 ecallisto_ng-0.1.3/src/ecallisto_ng/data_fetching/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:51.000000 ecallisto_ng-0.1.3/src/ecallisto_ng/data_fetching/__init__.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     6471 2023-07-13 18:03:37.000000 ecallisto_ng-0.1.3/src/ecallisto_ng/data_fetching/get_data.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2006 2023-07-13 17:59:20.000000 ecallisto_ng-0.1.3/src/ecallisto_ng/data_fetching/get_information.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 18:04:42.362043 ecallisto_ng-0.1.3/src/ecallisto_ng/data_processing/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:54.000000 ecallisto_ng-0.1.3/src/ecallisto_ng/data_processing/__init__.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     5256 2023-07-11 08:45:15.000000 ecallisto_ng-0.1.3/src/ecallisto_ng/data_processing/utils.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 18:04:42.362043 ecallisto_ng-0.1.3/src/ecallisto_ng/plotting/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:40:01.000000 ecallisto_ng-0.1.3/src/ecallisto_ng/plotting/__init__.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2425 2023-07-10 17:56:33.000000 ecallisto_ng-0.1.3/src/ecallisto_ng/plotting/utils.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 18:04:42.351210 ecallisto_ng-0.1.3/src/ecallisto_ng.egg-info/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3548 2023-07-13 18:04:42.000000 ecallisto_ng-0.1.3/src/ecallisto_ng.egg-info/PKG-INFO
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      556 2023-07-13 18:04:42.000000 ecallisto_ng-0.1.3/src/ecallisto_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        1 2023-07-13 18:04:42.000000 ecallisto_ng-0.1.3/src/ecallisto_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      113 2023-07-13 18:04:42.000000 ecallisto_ng-0.1.3/src/ecallisto_ng.egg-info/requires.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)       13 2023-07-13 18:04:42.000000 ecallisto_ng-0.1.3/src/ecallisto_ng.egg-info/top_level.txt
```

### Comparing `ecallisto_ng-0.1.2/LICENSE` & `ecallisto_ng-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.1.2/PKG-INFO` & `ecallisto_ng-0.1.3/src/ecallisto_ng.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ecallisto_ng
-Version: 0.1.2
+Name: ecallisto-ng
+Version: 0.1.3
 Summary: A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API.
 Author-email: Vincenzo Timmel <vincenzo.timmel@fhnw.ch>
 Project-URL: Homepage, https://github.com/i4Ds/ecallisto_ng
 Project-URL: Bug Tracker, https://github.com/i4Ds/ecallisto_ng/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ecallisto_ng-0.1.2/README.md` & `ecallisto_ng-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.1.2/pyproject.toml` & `ecallisto_ng-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ecallisto_ng"
-version = "0.1.2"
+version = "0.1.3"
 authors = [{name = "Vincenzo Timmel", email = "vincenzo.timmel@fhnw.ch"}]
 description = "A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API."
 readme = "README.md"
 
 requires-python = ">=3.9"
 
 classifiers = [
```

### Comparing `ecallisto_ng-0.1.2/src/ecallisto_ng/data_fetching/get_data.py` & `ecallisto_ng-0.1.3/src/ecallisto_ng/data_fetching/get_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         "start_datetime": start_datetime,
         "end_datetime": end_datetime,
         "timebucket": timebucket,
         "agg_function": agg_function,
         "return_type": return_type,
     }
 
-    assert pd.to_datetime(start_datetime) < pd.to_datetime(end_datetime), (
+    assert pd.to_datetime(start_datetime) <= pd.to_datetime(end_datetime), (
         f"start_datetime ({start_datetime}) must be before end_datetime ({end_datetime})"
     )
 
     response = requests.post(BASE_URL + "/api/data", json=data, timeout=180)
 
     if response.status_code == 200:
         url = (
```

### Comparing `ecallisto_ng-0.1.2/src/ecallisto_ng/data_fetching/get_information.py` & `ecallisto_ng-0.1.3/src/ecallisto_ng/data_fetching/get_information.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.1.2/src/ecallisto_ng/data_processing/utils.py` & `ecallisto_ng-0.1.3/src/ecallisto_ng/data_processing/utils.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.1.2/src/ecallisto_ng/plotting/utils.py` & `ecallisto_ng-0.1.3/src/ecallisto_ng/plotting/utils.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.1.2/src/ecallisto_ng.egg-info/PKG-INFO` & `ecallisto_ng-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ecallisto-ng
-Version: 0.1.2
+Name: ecallisto_ng
+Version: 0.1.3
 Summary: A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API.
 Author-email: Vincenzo Timmel <vincenzo.timmel@fhnw.ch>
 Project-URL: Homepage, https://github.com/i4Ds/ecallisto_ng
 Project-URL: Bug Tracker, https://github.com/i4Ds/ecallisto_ng/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ecallisto_ng-0.1.2/src/ecallisto_ng.egg-info/SOURCES.txt` & `ecallisto_ng-0.1.3/src/ecallisto_ng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

