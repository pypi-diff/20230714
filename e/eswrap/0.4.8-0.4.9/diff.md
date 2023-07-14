# Comparing `tmp/eswrap-0.4.8.tar.gz` & `tmp/eswrap-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eswrap-0.4.8.tar", last modified: Fri Jul 14 06:30:53 2023, max compression
+gzip compressed data, was "eswrap-0.4.9.tar", last modified: Fri Jul 14 09:36:05 2023, max compression
```

## Comparing `eswrap-0.4.8.tar` & `eswrap-0.4.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:30:53.430874 eswrap-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-14 06:30:53.430874 eswrap-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 06:30:36.000000 eswrap-0.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:30:53.430874 eswrap-0.4.8/eswrap/
--rw-r--r--   0 runner    (1001) docker     (123)    34509 2023-07-14 06:30:36.000000 eswrap-0.4.8/eswrap/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-14 06:30:53.000000 eswrap-0.4.8/eswrap/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-14 06:30:36.000000 eswrap-0.4.8/eswrap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:30:53.430874 eswrap-0.4.8/eswrap/common/
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-07-14 06:30:36.000000 eswrap-0.4.8/eswrap/common/EsHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:30:36.000000 eswrap-0.4.8/eswrap/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-07-14 06:30:36.000000 eswrap-0.4.8/eswrap/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:30:53.430874 eswrap-0.4.8/eswrap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-14 06:30:53.000000 eswrap-0.4.8/eswrap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-14 06:30:53.000000 eswrap-0.4.8/eswrap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 06:30:53.000000 eswrap-0.4.8/eswrap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-14 06:30:53.000000 eswrap-0.4.8/eswrap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 06:30:53.000000 eswrap-0.4.8/eswrap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 06:30:53.430874 eswrap-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-14 06:30:36.000000 eswrap-0.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:36:05.742912 eswrap-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-14 09:36:05.742912 eswrap-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 09:35:50.000000 eswrap-0.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:36:05.742912 eswrap-0.4.9/eswrap/
+-rw-r--r--   0 runner    (1001) docker     (123)    34509 2023-07-14 09:35:50.000000 eswrap-0.4.9/eswrap/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-14 09:36:05.000000 eswrap-0.4.9/eswrap/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-14 09:35:50.000000 eswrap-0.4.9/eswrap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:36:05.742912 eswrap-0.4.9/eswrap/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-07-14 09:35:50.000000 eswrap-0.4.9/eswrap/common/EsHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:35:50.000000 eswrap-0.4.9/eswrap/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-07-14 09:35:50.000000 eswrap-0.4.9/eswrap/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:36:05.742912 eswrap-0.4.9/eswrap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-14 09:36:05.000000 eswrap-0.4.9/eswrap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-14 09:36:05.000000 eswrap-0.4.9/eswrap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 09:36:05.000000 eswrap-0.4.9/eswrap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-14 09:36:05.000000 eswrap-0.4.9/eswrap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 09:36:05.000000 eswrap-0.4.9/eswrap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 09:36:05.742912 eswrap-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-14 09:35:50.000000 eswrap-0.4.9/setup.py
```

### Comparing `eswrap-0.4.8/PKG-INFO` & `eswrap-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eswrap
-Version: 0.4.8
+Version: 0.4.9
 Summary: Python wrapper for simple elasticsearch queries
 Home-page: 
 Author: Paul Tikken
 Author-email: paul.tikken@gmail.com
 License: GNU General Public License v3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `eswrap-0.4.8/eswrap/LICENSE` & `eswrap-0.4.9/eswrap/LICENSE`

 * *Files identical despite different names*

### Comparing `eswrap-0.4.8/eswrap/__init__.py` & `eswrap-0.4.9/eswrap/__init__.py`

 * *Files identical despite different names*

### Comparing `eswrap-0.4.8/eswrap/common/EsHandler.py` & `eswrap-0.4.9/eswrap/common/EsHandler.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,14 +50,42 @@
                 else:
                     data = {"query": {"match": filter}}
             else:
                 data = {"query": {"match": filter}}
 
         return self.es_connection.count(index=self.index, body=data, **kwargs)["count"]
 
+    def query_on_field(self, field_name: str, missing: bool = True, **kwargs):
+
+        if missing:
+
+            data = {
+                "query": {
+                    "bool": {
+                        "must_not": {
+                            "exists": {
+                                "field": f"{field_name}"
+                            }
+                        }
+                    }
+                }
+            }
+
+        else:
+
+            data = {
+                "query": {
+                    "exists": {
+                        "field": f"{field_name}"
+                    }
+                }
+            }
+
+        return self.es_connection.search(index=self.index, body=data, **kwargs)
+
     def upsert(self, document: dict, doc_id: Optional[str] = None, **kwargs):
         """ """
         if doc_id is None:
             return self.es_connection.index(
                 index=self.index, document=document, **kwargs
             )
         else:
@@ -80,21 +108,21 @@
 
 class EsCursor(object):
     """
     The EsCursor
     """
 
     def __init__(
-        self,
-        es_handler: EsHandler,
-        filter: dict = None,
-        limit: int = 10,
-        skip: int = None,
-        sort: tuple = None,
-        **kwargs
+            self,
+            es_handler: EsHandler,
+            filter: dict = None,
+            limit: int = 10,
+            skip: int = None,
+            sort: tuple = None,
+            **kwargs
     ):
         """
         Create a new CveSearchApi object.
 
         :param es_handler: EsHandler object
         :type es_handler: EsHandler
         """
```

### Comparing `eswrap-0.4.8/eswrap/main.py` & `eswrap-0.4.9/eswrap/main.py`

 * *Files identical despite different names*

### Comparing `eswrap-0.4.8/eswrap.egg-info/PKG-INFO` & `eswrap-0.4.9/eswrap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eswrap
-Version: 0.4.8
+Version: 0.4.9
 Summary: Python wrapper for simple elasticsearch queries
 Home-page: 
 Author: Paul Tikken
 Author-email: paul.tikken@gmail.com
 License: GNU General Public License v3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `eswrap-0.4.8/setup.py` & `eswrap-0.4.9/setup.py`

 * *Files identical despite different names*

