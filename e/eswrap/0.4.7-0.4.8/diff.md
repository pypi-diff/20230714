# Comparing `tmp/eswrap-0.4.7.tar.gz` & `tmp/eswrap-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eswrap-0.4.7.tar", last modified: Wed May 17 14:04:52 2023, max compression
+gzip compressed data, was "eswrap-0.4.8.tar", last modified: Fri Jul 14 06:30:53 2023, max compression
```

## Comparing `eswrap-0.4.7.tar` & `eswrap-0.4.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:04:52.090729 eswrap-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-17 14:04:52.090729 eswrap-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-17 14:04:36.000000 eswrap-0.4.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:04:52.090729 eswrap-0.4.7/eswrap/
--rw-r--r--   0 runner    (1001) docker     (123)    34509 2023-05-17 14:04:36.000000 eswrap-0.4.7/eswrap/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-17 14:04:51.000000 eswrap-0.4.7/eswrap/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-17 14:04:36.000000 eswrap-0.4.7/eswrap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:04:52.090729 eswrap-0.4.7/eswrap/common/
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-05-17 14:04:36.000000 eswrap-0.4.7/eswrap/common/EsHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 14:04:36.000000 eswrap-0.4.7/eswrap/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-17 14:04:36.000000 eswrap-0.4.7/eswrap/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:04:52.090729 eswrap-0.4.7/eswrap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-17 14:04:52.000000 eswrap-0.4.7/eswrap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-17 14:04:52.000000 eswrap-0.4.7/eswrap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 14:04:52.000000 eswrap-0.4.7/eswrap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-17 14:04:52.000000 eswrap-0.4.7/eswrap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 14:04:52.000000 eswrap-0.4.7/eswrap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 14:04:52.094729 eswrap-0.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-17 14:04:36.000000 eswrap-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:30:53.430874 eswrap-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-14 06:30:53.430874 eswrap-0.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 06:30:36.000000 eswrap-0.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:30:53.430874 eswrap-0.4.8/eswrap/
+-rw-r--r--   0 runner    (1001) docker     (123)    34509 2023-07-14 06:30:36.000000 eswrap-0.4.8/eswrap/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-14 06:30:53.000000 eswrap-0.4.8/eswrap/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-14 06:30:36.000000 eswrap-0.4.8/eswrap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:30:53.430874 eswrap-0.4.8/eswrap/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-07-14 06:30:36.000000 eswrap-0.4.8/eswrap/common/EsHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:30:36.000000 eswrap-0.4.8/eswrap/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-07-14 06:30:36.000000 eswrap-0.4.8/eswrap/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:30:53.430874 eswrap-0.4.8/eswrap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-14 06:30:53.000000 eswrap-0.4.8/eswrap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-14 06:30:53.000000 eswrap-0.4.8/eswrap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 06:30:53.000000 eswrap-0.4.8/eswrap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-14 06:30:53.000000 eswrap-0.4.8/eswrap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 06:30:53.000000 eswrap-0.4.8/eswrap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 06:30:53.430874 eswrap-0.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-14 06:30:36.000000 eswrap-0.4.8/setup.py
```

### Comparing `eswrap-0.4.7/PKG-INFO` & `eswrap-0.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eswrap
-Version: 0.4.7
+Version: 0.4.8
 Summary: Python wrapper for simple elasticsearch queries
 Home-page: 
 Author: Paul Tikken
 Author-email: paul.tikken@gmail.com
 License: GNU General Public License v3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `eswrap-0.4.7/eswrap/LICENSE` & `eswrap-0.4.8/eswrap/LICENSE`

 * *Files identical despite different names*

### Comparing `eswrap-0.4.7/eswrap/__init__.py` & `eswrap-0.4.8/eswrap/__init__.py`

 * *Files identical despite different names*

### Comparing `eswrap-0.4.7/eswrap/common/EsHandler.py` & `eswrap-0.4.8/eswrap/common/EsHandler.py`

 * *Files identical despite different names*

### Comparing `eswrap-0.4.7/eswrap/main.py` & `eswrap-0.4.8/eswrap/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         [
             'http://user:secret@localhost:9200/',
             'https://user:secret@other_host:443/production'
         ]
         """
         self.__version = VERSION
 
-        if connection_details is not None:
+        if connection_details is None:
             self.connection_details = [{"host": host, "port": port, "scheme": scheme}]
         else:
             self.connection_details = connection_details
 
         self.logger = logging.getLogger(__name__)
 
         self.__es_client = Elasticsearch(self.connection_details, **kwargs)
```

### Comparing `eswrap-0.4.7/eswrap.egg-info/PKG-INFO` & `eswrap-0.4.8/eswrap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eswrap
-Version: 0.4.7
+Version: 0.4.8
 Summary: Python wrapper for simple elasticsearch queries
 Home-page: 
 Author: Paul Tikken
 Author-email: paul.tikken@gmail.com
 License: GNU General Public License v3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `eswrap-0.4.7/setup.py` & `eswrap-0.4.8/setup.py`

 * *Files identical despite different names*

