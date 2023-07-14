# Comparing `tmp/fast-webflow-0.5.0.tar.gz` & `tmp/fast-webflow-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast-webflow-0.5.0.tar", last modified: Tue Jul  4 20:34:29 2023, max compression
+gzip compressed data, was "fast-webflow-0.5.1.tar", last modified: Fri Jul 14 14:38:10 2023, max compression
```

## Comparing `fast-webflow-0.5.0.tar` & `fast-webflow-0.5.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:34:29.146427 fast-webflow-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-04 20:34:18.000000 fast-webflow-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-07-04 20:34:29.146427 fast-webflow-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-07-04 20:34:18.000000 fast-webflow-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-04 20:34:18.000000 fast-webflow-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-04 20:34:29.146427 fast-webflow-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:34:29.142427 fast-webflow-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:34:29.146427 fast-webflow-0.5.0/src/fast_webflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-07-04 20:34:29.000000 fast-webflow-0.5.0/src/fast_webflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-04 20:34:29.000000 fast-webflow-0.5.0/src/fast_webflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 20:34:29.000000 fast-webflow-0.5.0/src/fast_webflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-04 20:34:29.000000 fast-webflow-0.5.0/src/fast_webflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:34:29.146427 fast-webflow-0.5.0/src/webflow/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-04 20:34:18.000000 fast-webflow-0.5.0/src/webflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:34:29.146427 fast-webflow-0.5.0/src/webflow/cms/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-04 20:34:18.000000 fast-webflow-0.5.0/src/webflow/cms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-07-04 20:34:18.000000 fast-webflow-0.5.0/src/webflow/cms/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-04 20:34:18.000000 fast-webflow-0.5.0/src/webflow/cms/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-07-04 20:34:18.000000 fast-webflow-0.5.0/src/webflow/cms/site.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-04 20:34:18.000000 fast-webflow-0.5.0/src/webflow/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-07-04 20:34:18.000000 fast-webflow-0.5.0/src/webflow/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-07-04 20:34:18.000000 fast-webflow-0.5.0/src/webflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:34:29.146427 fast-webflow-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-04 20:34:18.000000 fast-webflow-0.5.0/tests/test_authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:38:10.107393 fast-webflow-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-14 14:37:54.000000 fast-webflow-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-07-14 14:38:10.107393 fast-webflow-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-07-14 14:37:54.000000 fast-webflow-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-14 14:37:54.000000 fast-webflow-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-14 14:38:10.107393 fast-webflow-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:38:10.103393 fast-webflow-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:38:10.103393 fast-webflow-0.5.1/src/fast_webflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-07-14 14:38:10.000000 fast-webflow-0.5.1/src/fast_webflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-14 14:38:10.000000 fast-webflow-0.5.1/src/fast_webflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 14:38:10.000000 fast-webflow-0.5.1/src/fast_webflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 14:38:10.000000 fast-webflow-0.5.1/src/fast_webflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:38:10.103393 fast-webflow-0.5.1/src/webflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-14 14:37:54.000000 fast-webflow-0.5.1/src/webflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:38:10.103393 fast-webflow-0.5.1/src/webflow/cms/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-14 14:37:54.000000 fast-webflow-0.5.1/src/webflow/cms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-07-14 14:37:54.000000 fast-webflow-0.5.1/src/webflow/cms/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-14 14:37:54.000000 fast-webflow-0.5.1/src/webflow/cms/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-07-14 14:37:54.000000 fast-webflow-0.5.1/src/webflow/cms/site.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-14 14:37:54.000000 fast-webflow-0.5.1/src/webflow/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-07-14 14:37:54.000000 fast-webflow-0.5.1/src/webflow/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-07-14 14:37:54.000000 fast-webflow-0.5.1/src/webflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:38:10.103393 fast-webflow-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-14 14:37:54.000000 fast-webflow-0.5.1/tests/test_authentication.py
```

### Comparing `fast-webflow-0.5.0/LICENSE` & `fast-webflow-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fast-webflow-0.5.0/PKG-INFO` & `fast-webflow-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-webflow
-Version: 0.5.0
+Version: 0.5.1
 Summary: A client library to communicate with the WebFlow API
 Home-page: https://github.com/tcilloni/fast-webflow
 Author: Thomas Cilloni
 Author-email: tcilloni@outlook.com
 Project-URL: Bug Tracker, https://github.com/tcilloni/fast-webflow/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fast-webflow-0.5.0/README.md` & `fast-webflow-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `fast-webflow-0.5.0/setup.cfg` & `fast-webflow-0.5.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = fast-webflow
-version = 0.5.0
+version = 0.5.1
 author = Thomas Cilloni
 author_email = tcilloni@outlook.com
 description = A client library to communicate with the WebFlow API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tcilloni/fast-webflow
 project_urls =
```

### Comparing `fast-webflow-0.5.0/src/fast_webflow.egg-info/PKG-INFO` & `fast-webflow-0.5.1/src/fast_webflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-webflow
-Version: 0.5.0
+Version: 0.5.1
 Summary: A client library to communicate with the WebFlow API
 Home-page: https://github.com/tcilloni/fast-webflow
 Author: Thomas Cilloni
 Author-email: tcilloni@outlook.com
 Project-URL: Bug Tracker, https://github.com/tcilloni/fast-webflow/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fast-webflow-0.5.0/src/webflow/cms/collection.py` & `fast-webflow-0.5.1/src/webflow/cms/collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,15 +159,15 @@
         Args:
             offset (int, optional): number of items to skip. Defaults to 0.
             limit (int, optional): max number of items to return (capped at 100). Defaults to 100.
 
         Returns:
             dict[str, any]: group of items (index with the key `items` to get the actual data).
         '''
-        url = self._items_url + f"&offset={offset}&limit={limit}"
+        url = self._items_url + f"?offset={offset}&limit={limit}"
 
         return self._get(url)
     
 
     def get_all_items(self) -> list[dict]:
         '''
         Fetch all items in this collection.
```

### Comparing `fast-webflow-0.5.0/src/webflow/cms/item.py` & `fast-webflow-0.5.1/src/webflow/cms/item.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             collection_id (str): ID field (often `_id`) of the collection in the CMS.
             item_id (str): ID field (often `_id`) of the item in the CMS.
             throttle_delay (float, optional): number of seconds to wait after a request hits the 
                 rate limit. Defaults to 10.
             max_retries (int, optional): number of times failed requests are retried (including 
                 after hitting rate limits). Defaults to 50.
         '''
-        super(Site, self).__init__(id, *args, **kwargs)
+        super(Item, self).__init__(id, *args, **kwargs)
         self._url = f'https://api.webflow.com/collections/{collection_id}/items/{id}'
         self.data = self.get_data()
     
 
     def get_data(self) -> dict[str, any]:
         '''
         Fetch the item's information.
```

### Comparing `fast-webflow-0.5.0/src/webflow/cms/site.py` & `fast-webflow-0.5.1/src/webflow/cms/site.py`

 * *Files identical despite different names*

### Comparing `fast-webflow-0.5.0/src/webflow/config.py` & `fast-webflow-0.5.1/src/webflow/config.py`

 * *Files identical despite different names*

### Comparing `fast-webflow-0.5.0/src/webflow/entity.py` & `fast-webflow-0.5.1/src/webflow/entity.py`

 * *Files identical despite different names*

### Comparing `fast-webflow-0.5.0/src/webflow/utils.py` & `fast-webflow-0.5.1/src/webflow/utils.py`

 * *Files identical despite different names*

