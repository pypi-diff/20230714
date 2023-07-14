# Comparing `tmp/seatable-api-2.6.5.tar.gz` & `tmp/seatable-api-2.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seatable-api-2.6.5.tar", last modified: Tue Jun 13 02:51:00 2023, max compression
+gzip compressed data, was "seatable-api-2.6.6.tar", last modified: Fri Jul 14 06:57:02 2023, max compression
```

## Comparing `seatable-api-2.6.5.tar` & `seatable-api-2.6.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 chengxiongchao   (501) staff       (20)        0 2023-06-13 02:51:00.398452 seatable-api-2.6.5/
--rw-r--r--   0 chengxiongchao   (501) staff       (20)    11357 2023-01-04 02:34:58.000000 seatable-api-2.6.5/LICENSE
--rw-r--r--   0 chengxiongchao   (501) staff       (20)      656 2023-06-13 02:51:00.397685 seatable-api-2.6.5/PKG-INFO
--rw-r--r--   0 chengxiongchao   (501) staff       (20)      300 2023-01-04 02:34:58.000000 seatable-api-2.6.5/README.md
-drwxr-xr-x   0 chengxiongchao   (501) staff       (20)        0 2023-06-13 02:51:00.377592 seatable-api-2.6.5/seatable_api/
--rw-r--r--   0 chengxiongchao   (501) staff       (20)      171 2023-01-04 02:34:58.000000 seatable-api-2.6.5/seatable_api/__init__.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)    11418 2023-01-04 02:34:58.000000 seatable-api-2.6.5/seatable_api/column.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)     1135 2023-01-04 02:34:58.000000 seatable-api-2.6.5/seatable_api/constants.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)     1108 2023-01-04 02:34:58.000000 seatable-api-2.6.5/seatable_api/context.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)    29097 2023-01-04 02:34:58.000000 seatable-api-2.6.5/seatable_api/convert_airtable.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)    13988 2023-01-04 02:34:58.000000 seatable-api-2.6.5/seatable_api/date_utils.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)      119 2023-04-03 02:56:24.000000 seatable-api-2.6.5/seatable_api/exception.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)    42359 2023-05-24 08:00:54.000000 seatable-api-2.6.5/seatable_api/main.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)     2876 2023-01-04 02:34:58.000000 seatable-api-2.6.5/seatable_api/message.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)     9400 2023-01-04 02:34:58.000000 seatable-api-2.6.5/seatable_api/query.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)     2744 2023-01-04 02:34:58.000000 seatable-api-2.6.5/seatable_api/socket_io.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)     6424 2023-01-04 02:34:58.000000 seatable-api-2.6.5/seatable_api/utils.py
-drwxr-xr-x   0 chengxiongchao   (501) staff       (20)        0 2023-06-13 02:51:00.391618 seatable-api-2.6.5/seatable_api.egg-info/
--rw-r--r--   0 chengxiongchao   (501) staff       (20)      656 2023-06-13 02:51:00.000000 seatable-api-2.6.5/seatable_api.egg-info/PKG-INFO
--rw-r--r--   0 chengxiongchao   (501) staff       (20)      546 2023-06-13 02:51:00.000000 seatable-api-2.6.5/seatable_api.egg-info/SOURCES.txt
--rw-r--r--   0 chengxiongchao   (501) staff       (20)        1 2023-06-13 02:51:00.000000 seatable-api-2.6.5/seatable_api.egg-info/dependency_links.txt
--rw-r--r--   0 chengxiongchao   (501) staff       (20)       47 2023-06-13 02:51:00.000000 seatable-api-2.6.5/seatable_api.egg-info/requires.txt
--rw-r--r--   0 chengxiongchao   (501) staff       (20)       19 2023-06-13 02:51:00.000000 seatable-api-2.6.5/seatable_api.egg-info/top_level.txt
--rw-r--r--   0 chengxiongchao   (501) staff       (20)       38 2023-06-13 02:51:00.402124 seatable-api-2.6.5/setup.cfg
--rw-r--r--   0 chengxiongchao   (501) staff       (20)      723 2023-06-13 02:50:41.000000 seatable-api-2.6.5/setup.py
-drwxr-xr-x   0 chengxiongchao   (501) staff       (20)        0 2023-06-13 02:51:00.394290 seatable-api-2.6.5/tests/
--rw-r--r--   0 chengxiongchao   (501) staff       (20)        0 2023-06-13 02:45:17.000000 seatable-api-2.6.5/tests/__init__.py
--rw-r--r--   0 chengxiongchao   (501) staff       (20)     5261 2023-06-13 02:45:20.000000 seatable-api-2.6.5/tests/dateutils_test.py
+drwxr-xr-x   0 chengxiongchao   (501) staff       (20)        0 2023-07-14 06:57:02.442038 seatable-api-2.6.6/
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)    11357 2023-01-04 02:34:58.000000 seatable-api-2.6.6/LICENSE
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)      656 2023-07-14 06:57:02.437045 seatable-api-2.6.6/PKG-INFO
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)      300 2023-01-04 02:34:58.000000 seatable-api-2.6.6/README.md
+drwxr-xr-x   0 chengxiongchao   (501) staff       (20)        0 2023-07-14 06:57:02.428316 seatable-api-2.6.6/seatable_api/
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)      171 2023-01-04 02:34:58.000000 seatable-api-2.6.6/seatable_api/__init__.py
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)    11418 2023-01-04 02:34:58.000000 seatable-api-2.6.6/seatable_api/column.py
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)     1135 2023-01-04 02:34:58.000000 seatable-api-2.6.6/seatable_api/constants.py
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)     1322 2023-07-14 06:55:21.000000 seatable-api-2.6.6/seatable_api/context.py
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)    29097 2023-01-04 02:34:58.000000 seatable-api-2.6.6/seatable_api/convert_airtable.py
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)    13988 2023-01-04 02:34:58.000000 seatable-api-2.6.6/seatable_api/date_utils.py
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)      119 2023-04-03 02:56:24.000000 seatable-api-2.6.6/seatable_api/exception.py
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)    42361 2023-07-14 06:55:21.000000 seatable-api-2.6.6/seatable_api/main.py
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)     2876 2023-01-04 02:34:58.000000 seatable-api-2.6.6/seatable_api/message.py
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)     9400 2023-01-04 02:34:58.000000 seatable-api-2.6.6/seatable_api/query.py
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)     2744 2023-01-04 02:34:58.000000 seatable-api-2.6.6/seatable_api/socket_io.py
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)     6424 2023-01-04 02:34:58.000000 seatable-api-2.6.6/seatable_api/utils.py
+drwxr-xr-x   0 chengxiongchao   (501) staff       (20)        0 2023-07-14 06:57:02.432160 seatable-api-2.6.6/seatable_api.egg-info/
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)      656 2023-07-14 06:57:02.000000 seatable-api-2.6.6/seatable_api.egg-info/PKG-INFO
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)      546 2023-07-14 06:57:02.000000 seatable-api-2.6.6/seatable_api.egg-info/SOURCES.txt
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)        1 2023-07-14 06:57:02.000000 seatable-api-2.6.6/seatable_api.egg-info/dependency_links.txt
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)       47 2023-07-14 06:57:02.000000 seatable-api-2.6.6/seatable_api.egg-info/requires.txt
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)       19 2023-07-14 06:57:02.000000 seatable-api-2.6.6/seatable_api.egg-info/top_level.txt
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)       38 2023-07-14 06:57:02.442480 seatable-api-2.6.6/setup.cfg
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)      723 2023-07-14 06:56:35.000000 seatable-api-2.6.6/setup.py
+drwxr-xr-x   0 chengxiongchao   (501) staff       (20)        0 2023-07-14 06:57:02.434862 seatable-api-2.6.6/tests/
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)        0 2023-06-13 02:45:17.000000 seatable-api-2.6.6/tests/__init__.py
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)     5261 2023-06-13 02:45:20.000000 seatable-api-2.6.6/tests/dateutils_test.py
```

### Comparing `seatable-api-2.6.5/LICENSE` & `seatable-api-2.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.5/PKG-INFO` & `seatable-api-2.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seatable-api
-Version: 2.6.5
+Version: 2.6.6
 Summary: Python client for SeaTable web api
 Home-page: https://github.com/seatable/seatable-api-python
 Author: seatable
 Author-email: support@seafile.com
 License: Apache Licence
 Platform: any
 Classifier: Programming Language :: Python
```

### Comparing `seatable-api-2.6.5/seatable_api/column.py` & `seatable-api-2.6.6/seatable_api/column.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.5/seatable_api/constants.py` & `seatable-api-2.6.6/seatable_api/constants.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.5/seatable_api/context.py` & `seatable-api-2.6.6/seatable_api/context.py`

 * *Files 14% similar despite different names*

```diff
@@ -44,13 +44,23 @@
         return context_data.get('table')
 
     @property
     @need_data
     def current_user_id(self):
         return context_data.get('current_user_id')
 
+    @property
+    @need_data
+    def current_username(self):
+        return context_data.get('current_username')
+
+    @property
+    @need_data
+    def id_in_org(self):
+        return context_data.get('id_in_org')
+
     @need_data
     def get_setting_by_key(self, key):
         return context_data.get(key)
 
 
 context = Context()
```

### Comparing `seatable-api-2.6.5/seatable_api/convert_airtable.py` & `seatable-api-2.6.6/seatable_api/convert_airtable.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.5/seatable_api/date_utils.py` & `seatable-api-2.6.6/seatable_api/date_utils.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.5/seatable_api/main.py` & `seatable-api-2.6.6/seatable_api/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -925,18 +925,18 @@
         else:
             return results
 
     def get_related_users(self):
         response = requests.get(self._get_related_users_url(), headers=self.headers)
         return parse_response(response)['user_list']
 
-    def send_toast_notification(self, user_id, msg, toast_type='success'):
+    def send_toast_notification(self, username, msg, toast_type='success'):
         url = self._send_toast_notification_url()
         requests.post(url, json={
-            'to_user': user_id,
+            'to_user': username,
             'toast_type': toast_type,
             'detail': {
                 'msg': str(msg)
             }
         }, headers=self.headers)
 
     def add_workflow_task(self, workflow_token, row_data, initiator=None, link_rows=None, new_linked_rows=None):
```

### Comparing `seatable-api-2.6.5/seatable_api/message.py` & `seatable-api-2.6.6/seatable_api/message.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.5/seatable_api/query.py` & `seatable-api-2.6.6/seatable_api/query.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.5/seatable_api/socket_io.py` & `seatable-api-2.6.6/seatable_api/socket_io.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.5/seatable_api/utils.py` & `seatable-api-2.6.6/seatable_api/utils.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.5/seatable_api.egg-info/PKG-INFO` & `seatable-api-2.6.6/seatable_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seatable-api
-Version: 2.6.5
+Version: 2.6.6
 Summary: Python client for SeaTable web api
 Home-page: https://github.com/seatable/seatable-api-python
 Author: seatable
 Author-email: support@seafile.com
 License: Apache Licence
 Platform: any
 Classifier: Programming Language :: Python
```

### Comparing `seatable-api-2.6.5/seatable_api.egg-info/SOURCES.txt` & `seatable-api-2.6.6/seatable_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.5/setup.py` & `seatable-api-2.6.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-__version__ = '2.6.5'
+__version__ = '2.6.6'
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='seatable-api',
     version=__version__,
```

### Comparing `seatable-api-2.6.5/tests/dateutils_test.py` & `seatable-api-2.6.6/tests/dateutils_test.py`

 * *Files identical despite different names*

