# Comparing `tmp/eswrap-0.4.9.tar.gz` & `tmp/eswrap-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eswrap-0.4.9.tar", last modified: Fri Jul 14 09:36:05 2023, max compression
+gzip compressed data, was "eswrap-0.5.0.tar", last modified: Fri Jul 14 11:32:35 2023, max compression
```

## Comparing `eswrap-0.4.9.tar` & `eswrap-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:36:05.742912 eswrap-0.4.9/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-14 09:36:05.742912 eswrap-0.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 09:35:50.000000 eswrap-0.4.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:36:05.742912 eswrap-0.4.9/eswrap/
--rw-r--r--   0 runner    (1001) docker     (123)    34509 2023-07-14 09:35:50.000000 eswrap-0.4.9/eswrap/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-14 09:36:05.000000 eswrap-0.4.9/eswrap/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-14 09:35:50.000000 eswrap-0.4.9/eswrap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:36:05.742912 eswrap-0.4.9/eswrap/common/
--rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-07-14 09:35:50.000000 eswrap-0.4.9/eswrap/common/EsHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:35:50.000000 eswrap-0.4.9/eswrap/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-07-14 09:35:50.000000 eswrap-0.4.9/eswrap/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:36:05.742912 eswrap-0.4.9/eswrap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-14 09:36:05.000000 eswrap-0.4.9/eswrap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-14 09:36:05.000000 eswrap-0.4.9/eswrap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 09:36:05.000000 eswrap-0.4.9/eswrap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-14 09:36:05.000000 eswrap-0.4.9/eswrap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 09:36:05.000000 eswrap-0.4.9/eswrap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 09:36:05.742912 eswrap-0.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-14 09:35:50.000000 eswrap-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:32:35.351192 eswrap-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-14 11:32:35.351192 eswrap-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 11:32:23.000000 eswrap-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:32:35.351192 eswrap-0.5.0/eswrap/
+-rw-r--r--   0 runner    (1001) docker     (123)    34509 2023-07-14 11:32:23.000000 eswrap-0.5.0/eswrap/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-14 11:32:35.000000 eswrap-0.5.0/eswrap/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-14 11:32:23.000000 eswrap-0.5.0/eswrap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:32:35.351192 eswrap-0.5.0/eswrap/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-07-14 11:32:23.000000 eswrap-0.5.0/eswrap/common/EsHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 11:32:23.000000 eswrap-0.5.0/eswrap/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-07-14 11:32:23.000000 eswrap-0.5.0/eswrap/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:32:35.351192 eswrap-0.5.0/eswrap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-14 11:32:35.000000 eswrap-0.5.0/eswrap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-14 11:32:35.000000 eswrap-0.5.0/eswrap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 11:32:35.000000 eswrap-0.5.0/eswrap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-14 11:32:35.000000 eswrap-0.5.0/eswrap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 11:32:35.000000 eswrap-0.5.0/eswrap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 11:32:35.351192 eswrap-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-14 11:32:23.000000 eswrap-0.5.0/setup.py
```

### Comparing `eswrap-0.4.9/PKG-INFO` & `eswrap-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eswrap
-Version: 0.4.9
+Version: 0.5.0
 Summary: Python wrapper for simple elasticsearch queries
 Home-page: 
 Author: Paul Tikken
 Author-email: paul.tikken@gmail.com
 License: GNU General Public License v3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `eswrap-0.4.9/eswrap/LICENSE` & `eswrap-0.5.0/eswrap/LICENSE`

 * *Files identical despite different names*

### Comparing `eswrap-0.4.9/eswrap/__init__.py` & `eswrap-0.5.0/eswrap/__init__.py`

 * *Files identical despite different names*

### Comparing `eswrap-0.4.9/eswrap/common/EsHandler.py` & `eswrap-0.5.0/eswrap/common/EsHandler.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     def search(self, filter: dict = None, skip: int = 0, limit: int = 10):
         """
         Search the index.
         """
         return EsCursor(self, filter, limit=limit, skip=skip).search()
 
-    def find(self, filter: dict = None,  **kwargs):
+    def find(self, filter: dict = None, **kwargs):
         """
         Query the index.
         """
         return EsCursor(self, filter, **kwargs)
 
     def find_one(self, filter: dict = None):
         """
@@ -52,39 +52,29 @@
             else:
                 data = {"query": {"match": filter}}
 
         return self.es_connection.count(index=self.index, body=data, **kwargs)["count"]
 
     def query_on_field(self, field_name: str, missing: bool = True, **kwargs):
 
+        kwargs = kwargs
+        kwargs["query_on_field"] = True
+
         if missing:
+            kwargs["bool_query"] = True
 
-            data = {
-                "query": {
-                    "bool": {
-                        "must_not": {
-                            "exists": {
-                                "field": f"{field_name}"
-                            }
-                        }
-                    }
-                }
-            }
+            data = {"must_not": {"exists": {"field": f"{field_name}"}}}
 
         else:
 
-            data = {
-                "query": {
-                    "exists": {
-                        "field": f"{field_name}"
-                    }
-                }
-            }
+            kwargs["exists_query"] = True
+
+            data = {"field": f"{field_name}"}
 
-        return self.es_connection.search(index=self.index, body=data, **kwargs)
+        return EsCursor(self, data, **kwargs)
 
     def upsert(self, document: dict, doc_id: Optional[str] = None, **kwargs):
         """ """
         if doc_id is None:
             return self.es_connection.index(
                 index=self.index, document=document, **kwargs
             )
@@ -108,21 +98,21 @@
 
 class EsCursor(object):
     """
     The EsCursor
     """
 
     def __init__(
-            self,
-            es_handler: EsHandler,
-            filter: dict = None,
-            limit: int = 10,
-            skip: int = None,
-            sort: tuple = None,
-            **kwargs
+        self,
+        es_handler: EsHandler,
+        filter: dict = None,
+        limit: int = 10,
+        skip: int = None,
+        sort: tuple = None,
+        **kwargs,
     ):
         """
         Create a new CveSearchApi object.
 
         :param es_handler: EsHandler object
         :type es_handler: EsHandler
         """
@@ -142,14 +132,19 @@
                 if self.regexp:
                     if hasattr(self, "bool_query") and self.bool_query:
                         data = {"query": {"bool": filter}}
                     else:
                         data = {"query": {"regexp": filter}}
                 else:
                     data = {"query": {"match": filter}}
+            elif hasattr(self, "query_on_field"):
+                if hasattr(self, "bool_query") and self.bool_query:
+                    data = {"query": {"bool": filter}}
+                if hasattr(self, "exists_query") and self.exists_query:
+                    data = {"query": {"exists": filter}}
             else:
                 data = {"query": {"match": filter}}
 
         self.__data = data
 
         self.__empty = False
```

### Comparing `eswrap-0.4.9/eswrap/main.py` & `eswrap-0.5.0/eswrap/main.py`

 * *Files identical despite different names*

### Comparing `eswrap-0.4.9/eswrap.egg-info/PKG-INFO` & `eswrap-0.5.0/eswrap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eswrap
-Version: 0.4.9
+Version: 0.5.0
 Summary: Python wrapper for simple elasticsearch queries
 Home-page: 
 Author: Paul Tikken
 Author-email: paul.tikken@gmail.com
 License: GNU General Public License v3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `eswrap-0.4.9/setup.py` & `eswrap-0.5.0/setup.py`

 * *Files identical despite different names*

