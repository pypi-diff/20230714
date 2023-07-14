# Comparing `tmp/django-learngual-0.13.7.tar.gz` & `tmp/django-learngual-0.13.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-learngual-0.13.7.tar", last modified: Fri Jul 14 17:53:15 2023, max compression
+gzip compressed data, was "django-learngual-0.13.9.tar", last modified: Fri Jul 14 17:59:56 2023, max compression
```

## Comparing `django-learngual-0.13.7.tar` & `django-learngual-0.13.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:53:15.932215 django-learngual-0.13.7/
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-14 17:52:24.000000 django-learngual-0.13.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-14 17:52:24.000000 django-learngual-0.13.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-14 17:53:15.932215 django-learngual-0.13.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-14 17:52:24.000000 django-learngual-0.13.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:53:15.932215 django-learngual-0.13.7/django_learngual.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-14 17:53:15.000000 django-learngual-0.13.7/django_learngual.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-14 17:53:15.000000 django-learngual-0.13.7/django_learngual.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:53:15.000000 django-learngual-0.13.7/django_learngual.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-14 17:53:15.000000 django-learngual-0.13.7/django_learngual.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:53:15.932215 django-learngual-0.13.7/learngual/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:53:12.000000 django-learngual-0.13.7/learngual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:53:12.000000 django-learngual-0.13.7/learngual/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:53:15.932215 django-learngual-0.13.7/learngual/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:53:12.000000 django-learngual-0.13.7/learngual/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:53:12.000000 django-learngual-0.13.7/learngual/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-14 17:53:12.000000 django-learngual-0.13.7/learngual/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-07-14 17:53:12.000000 django-learngual-0.13.7/learngual/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-14 17:53:12.000000 django-learngual-0.13.7/learngual/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:53:15.932215 django-learngual-0.13.7/learngual/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:53:12.000000 django-learngual-0.13.7/learngual/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:53:12.000000 django-learngual-0.13.7/learngual/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-14 17:53:12.000000 django-learngual-0.13.7/learngual/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:53:12.000000 django-learngual-0.13.7/learngual/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:53:15.932215 django-learngual-0.13.7/learngual/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:53:12.000000 django-learngual-0.13.7/learngual/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:53:12.000000 django-learngual-0.13.7/learngual/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-14 17:53:12.000000 django-learngual-0.13.7/learngual/tests/request_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-14 17:53:12.000000 django-learngual-0.13.7/learngual/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:53:12.000000 django-learngual-0.13.7/learngual/tests/test_drf_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-07-14 17:53:12.000000 django-learngual-0.13.7/learngual/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-14 17:53:12.000000 django-learngual-0.13.7/learngual/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    14739 2023-07-14 17:53:12.000000 django-learngual-0.13.7/learngual/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-14 17:53:15.932215 django-learngual-0.13.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 17:52:24.000000 django-learngual-0.13.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:59:56.087071 django-learngual-0.13.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-14 17:59:00.000000 django-learngual-0.13.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-14 17:59:00.000000 django-learngual-0.13.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-14 17:59:56.087071 django-learngual-0.13.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-14 17:59:00.000000 django-learngual-0.13.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:59:56.083071 django-learngual-0.13.9/django_learngual.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-14 17:59:56.000000 django-learngual-0.13.9/django_learngual.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-14 17:59:56.000000 django-learngual-0.13.9/django_learngual.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:59:56.000000 django-learngual-0.13.9/django_learngual.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-14 17:59:56.000000 django-learngual-0.13.9/django_learngual.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:59:56.087071 django-learngual-0.13.9/learngual/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:59:50.000000 django-learngual-0.13.9/learngual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:59:50.000000 django-learngual-0.13.9/learngual/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:59:56.087071 django-learngual-0.13.9/learngual/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:59:50.000000 django-learngual-0.13.9/learngual/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:59:50.000000 django-learngual-0.13.9/learngual/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-14 17:59:50.000000 django-learngual-0.13.9/learngual/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-07-14 17:59:50.000000 django-learngual-0.13.9/learngual/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-14 17:59:50.000000 django-learngual-0.13.9/learngual/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:59:56.087071 django-learngual-0.13.9/learngual/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:59:50.000000 django-learngual-0.13.9/learngual/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:59:50.000000 django-learngual-0.13.9/learngual/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-14 17:59:50.000000 django-learngual-0.13.9/learngual/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:59:50.000000 django-learngual-0.13.9/learngual/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:59:56.087071 django-learngual-0.13.9/learngual/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:59:50.000000 django-learngual-0.13.9/learngual/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:59:50.000000 django-learngual-0.13.9/learngual/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-14 17:59:50.000000 django-learngual-0.13.9/learngual/tests/request_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-14 17:59:50.000000 django-learngual-0.13.9/learngual/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:59:50.000000 django-learngual-0.13.9/learngual/tests/test_drf_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-07-14 17:59:50.000000 django-learngual-0.13.9/learngual/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-14 17:59:50.000000 django-learngual-0.13.9/learngual/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14775 2023-07-14 17:59:50.000000 django-learngual-0.13.9/learngual/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-14 17:59:56.087071 django-learngual-0.13.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 17:59:00.000000 django-learngual-0.13.9/setup.py
```

### Comparing `django-learngual-0.13.7/LICENSE` & `django-learngual-0.13.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.7/PKG-INFO` & `django-learngual-0.13.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-learngual
-Version: 0.13.7
+Version: 0.13.9
 Summary: Learngual helper package
 Home-page: https://learngual.com
 Author: learngual
 Author-email: developer@leanrgual.com
 Maintainer: Aniekutmfon
 Maintainer-email: aniekutmfonekere@gmail.com
 License: Proprietary Software License Agreement
```

### Comparing `django-learngual-0.13.7/README.rst` & `django-learngual-0.13.9/README.rst`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.7/django_learngual.egg-info/PKG-INFO` & `django-learngual-0.13.9/django_learngual.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-learngual
-Version: 0.13.7
+Version: 0.13.9
 Summary: Learngual helper package
 Home-page: https://learngual.com
 Author: learngual
 Author-email: developer@leanrgual.com
 Maintainer: Aniekutmfon
 Maintainer-email: aniekutmfonekere@gmail.com
 License: Proprietary Software License Agreement
```

### Comparing `django-learngual-0.13.7/django_learngual.egg-info/SOURCES.txt` & `django-learngual-0.13.9/django_learngual.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.7/learngual/apps.py` & `django-learngual-0.13.9/learngual/apps.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.7/learngual/authentication.py` & `django-learngual-0.13.9/learngual/authentication.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.7/learngual/permissions.py` & `django-learngual-0.13.9/learngual/permissions.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.7/learngual/tests/request_mock.py` & `django-learngual-0.13.9/learngual/tests/request_mock.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.7/learngual/tests/test_authentication.py` & `django-learngual-0.13.9/learngual/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.7/learngual/tests/test_utils.py` & `django-learngual-0.13.9/learngual/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.7/learngual/utils.py` & `django-learngual-0.13.9/learngual/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -418,30 +418,30 @@
         url_path = f"/{service}/v1/permissions/{permission_id}/"
         res = requests.patch(
             base_url.rstrip("/") + url_path + get_service_request_params(**params),
             json=permmission_data,
             headers=get_service_request_headers(**headers),
         )
         if not res.ok:
-            raise requests.exceptions.RequestException(res.content)
+            raise requests.exceptions.RequestException("permission service is down")
         return res.json()
 
     def clear_cache(
         self,
         *,
         service: Literal["iam", "payment", "notify", "learn", "media"] = "iam",
         permission_id: str,
     ):
         """clear cache
 
         Args:
             permission_id (str): _description_
             service (Literal["iam", "payment", "notify", "learn", "media"], optional): _description_. Defaults to "iam".
         """
-        url_path = f"/{service}/v1/service/permission/{permission_id}/"
+        url_path = f"/{service}/v1/service/permissions/{permission_id}/"
         cache.delete(url_path)
 
     def retrieve_permission(
         self,
         *,
         base_url: str,
         permission_id: str,
@@ -458,15 +458,15 @@
             service (_type_): "iam" | "pay" | "notify" | "learn" | "media"
             base_url (str):
             dot_path (str):Default:None, e.g metadata.request_count.value
             headers (dict):Default:{}
             params (str):Default:"", e.g name=ann&age=102
             cache_timeout (float):Default:timezone.timedelta(hours=1).total_seconds()
         """
-        url_path = f"/{service}/v1/service/permission/{permission_id}/"
+        url_path = f"/{service}/v1/service/permissions/{permission_id}/"
         if "localhost" in base_url:
             if dot_path:
                 return True
             else:
                 return {
                     "id": "test-local",
                     "metadata": {"request_count": True, "messages": True},
@@ -478,14 +478,14 @@
 
         if not data:
             res = requests.get(
                 base_url.rstrip("/") + url_path + get_service_request_params(**params),
                 headers=get_service_request_headers(**headers),
             )
             if not res.ok:
-                raise requests.exceptions.RequestException(res.content)
+                raise requests.exceptions.RequestException("permission service is down")
             data = res.json()
             cache.set(url_path, data, timeout=cache_timeout)
 
         if dot_path:
             return get_nested_value(data, dot_path)
         return data
```

### Comparing `django-learngual-0.13.7/setup.cfg` & `django-learngual-0.13.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-learngual
-version = 0.13.7
+version = 0.13.9
 author = learngual
 author_email = developer@leanrgual.com
 maintainer = Aniekutmfon
 maintainer_email = aniekutmfonekere@gmail.com
 description = Learngual helper package
 long_description = file:README.rst
 long_description_content_type = text/x-rst
```

