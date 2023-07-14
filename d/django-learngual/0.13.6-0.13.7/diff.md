# Comparing `tmp/django-learngual-0.13.6.tar.gz` & `tmp/django-learngual-0.13.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-learngual-0.13.6.tar", last modified: Fri Jul  7 14:31:01 2023, max compression
+gzip compressed data, was "django-learngual-0.13.7.tar", last modified: Fri Jul 14 17:53:15 2023, max compression
```

## Comparing `django-learngual-0.13.6.tar` & `django-learngual-0.13.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:31:01.199071 django-learngual-0.13.6/
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-07 14:30:06.000000 django-learngual-0.13.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-07 14:30:06.000000 django-learngual-0.13.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-07 14:31:01.199071 django-learngual-0.13.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-07 14:30:06.000000 django-learngual-0.13.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:31:01.199071 django-learngual-0.13.6/django_learngual.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-07 14:31:01.000000 django-learngual-0.13.6/django_learngual.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-07 14:31:01.000000 django-learngual-0.13.6/django_learngual.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 14:31:01.000000 django-learngual-0.13.6/django_learngual.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 14:31:01.000000 django-learngual-0.13.6/django_learngual.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:31:01.199071 django-learngual-0.13.6/learngual/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:30:55.000000 django-learngual-0.13.6/learngual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:30:55.000000 django-learngual-0.13.6/learngual/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:31:01.199071 django-learngual-0.13.6/learngual/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:30:55.000000 django-learngual-0.13.6/learngual/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:30:55.000000 django-learngual-0.13.6/learngual/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-07 14:30:55.000000 django-learngual-0.13.6/learngual/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-07-07 14:30:55.000000 django-learngual-0.13.6/learngual/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-07 14:30:55.000000 django-learngual-0.13.6/learngual/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:31:01.199071 django-learngual-0.13.6/learngual/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:30:55.000000 django-learngual-0.13.6/learngual/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:30:55.000000 django-learngual-0.13.6/learngual/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-07 14:30:55.000000 django-learngual-0.13.6/learngual/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:30:55.000000 django-learngual-0.13.6/learngual/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:31:01.199071 django-learngual-0.13.6/learngual/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:30:55.000000 django-learngual-0.13.6/learngual/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:30:55.000000 django-learngual-0.13.6/learngual/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-07 14:30:55.000000 django-learngual-0.13.6/learngual/tests/request_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-07 14:30:55.000000 django-learngual-0.13.6/learngual/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:30:55.000000 django-learngual-0.13.6/learngual/tests/test_drf_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-07-07 14:30:55.000000 django-learngual-0.13.6/learngual/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-07 14:30:55.000000 django-learngual-0.13.6/learngual/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    14738 2023-07-07 14:30:55.000000 django-learngual-0.13.6/learngual/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-07 14:31:01.199071 django-learngual-0.13.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 14:30:06.000000 django-learngual-0.13.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:53:15.932215 django-learngual-0.13.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-14 17:52:24.000000 django-learngual-0.13.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-14 17:52:24.000000 django-learngual-0.13.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-14 17:53:15.932215 django-learngual-0.13.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-14 17:52:24.000000 django-learngual-0.13.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:53:15.932215 django-learngual-0.13.7/django_learngual.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-14 17:53:15.000000 django-learngual-0.13.7/django_learngual.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-14 17:53:15.000000 django-learngual-0.13.7/django_learngual.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:53:15.000000 django-learngual-0.13.7/django_learngual.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-14 17:53:15.000000 django-learngual-0.13.7/django_learngual.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:53:15.932215 django-learngual-0.13.7/learngual/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:53:12.000000 django-learngual-0.13.7/learngual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:53:12.000000 django-learngual-0.13.7/learngual/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:53:15.932215 django-learngual-0.13.7/learngual/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:53:12.000000 django-learngual-0.13.7/learngual/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:53:12.000000 django-learngual-0.13.7/learngual/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-14 17:53:12.000000 django-learngual-0.13.7/learngual/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-07-14 17:53:12.000000 django-learngual-0.13.7/learngual/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-14 17:53:12.000000 django-learngual-0.13.7/learngual/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:53:15.932215 django-learngual-0.13.7/learngual/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:53:12.000000 django-learngual-0.13.7/learngual/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:53:12.000000 django-learngual-0.13.7/learngual/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-14 17:53:12.000000 django-learngual-0.13.7/learngual/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:53:12.000000 django-learngual-0.13.7/learngual/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:53:15.932215 django-learngual-0.13.7/learngual/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:53:12.000000 django-learngual-0.13.7/learngual/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:53:12.000000 django-learngual-0.13.7/learngual/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-14 17:53:12.000000 django-learngual-0.13.7/learngual/tests/request_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-14 17:53:12.000000 django-learngual-0.13.7/learngual/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:53:12.000000 django-learngual-0.13.7/learngual/tests/test_drf_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-07-14 17:53:12.000000 django-learngual-0.13.7/learngual/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-14 17:53:12.000000 django-learngual-0.13.7/learngual/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14739 2023-07-14 17:53:12.000000 django-learngual-0.13.7/learngual/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-14 17:53:15.932215 django-learngual-0.13.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 17:52:24.000000 django-learngual-0.13.7/setup.py
```

### Comparing `django-learngual-0.13.6/LICENSE` & `django-learngual-0.13.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.6/PKG-INFO` & `django-learngual-0.13.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-learngual
-Version: 0.13.6
+Version: 0.13.7
 Summary: Learngual helper package
 Home-page: https://learngual.com
 Author: learngual
 Author-email: developer@leanrgual.com
 Maintainer: Aniekutmfon
 Maintainer-email: aniekutmfonekere@gmail.com
 License: Proprietary Software License Agreement
```

### Comparing `django-learngual-0.13.6/README.rst` & `django-learngual-0.13.7/README.rst`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.6/django_learngual.egg-info/PKG-INFO` & `django-learngual-0.13.7/django_learngual.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-learngual
-Version: 0.13.6
+Version: 0.13.7
 Summary: Learngual helper package
 Home-page: https://learngual.com
 Author: learngual
 Author-email: developer@leanrgual.com
 Maintainer: Aniekutmfon
 Maintainer-email: aniekutmfonekere@gmail.com
 License: Proprietary Software License Agreement
```

### Comparing `django-learngual-0.13.6/django_learngual.egg-info/SOURCES.txt` & `django-learngual-0.13.7/django_learngual.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.6/learngual/apps.py` & `django-learngual-0.13.7/learngual/apps.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.6/learngual/authentication.py` & `django-learngual-0.13.7/learngual/authentication.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.6/learngual/permissions.py` & `django-learngual-0.13.7/learngual/permissions.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.6/learngual/tests/request_mock.py` & `django-learngual-0.13.7/learngual/tests/request_mock.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.6/learngual/tests/test_authentication.py` & `django-learngual-0.13.7/learngual/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.13.6/learngual/tests/test_utils.py` & `django-learngual-0.13.7/learngual/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,17 +174,17 @@
         "metadata.analytics.value": False,
     }
     permission_dict = unflatten_dict(permission_flat_dict)
     assert not permission_dict.get("metadata.request_count.value")
     mock_requests.return_value.json.return_value = permission_dict
     random_key = choice(list(permission_flat_dict.keys()))
     res = permission_manager.retrieve_permission(
-        base_url="https://localhost", permission_id=uuid4().hex[:10], service="iam"
+        base_url="https://example.com", permission_id=uuid4().hex[:10], service="iam"
     )
     assert res == permission_dict, res
     res = permission_manager.retrieve_permission(
-        base_url="https://localhost",
+        base_url="https://example.com",
         permission_id=uuid4().hex[:10],
         service="iam",
         dot_path=random_key,
     )
     assert res == permission_flat_dict.get(random_key), res
```

### Comparing `django-learngual-0.13.6/learngual/utils.py` & `django-learngual-0.13.7/learngual/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -411,15 +411,15 @@
                 "id": "test-local",
                 "metadata": {"request_count": True, "messages": True},
             }
 
         params = params.strip("?")
         params = dict([x.split("=") for x in params.split("&")])
 
-        url_path = f"/{service}/v1/permission/{permission_id}/"
+        url_path = f"/{service}/v1/permissions/{permission_id}/"
         res = requests.patch(
             base_url.rstrip("/") + url_path + get_service_request_params(**params),
             json=permmission_data,
             headers=get_service_request_headers(**headers),
         )
         if not res.ok:
             raise requests.exceptions.RequestException(res.content)
```

### Comparing `django-learngual-0.13.6/setup.cfg` & `django-learngual-0.13.7/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-learngual
-version = 0.13.6
+version = 0.13.7
 author = learngual
 author_email = developer@leanrgual.com
 maintainer = Aniekutmfon
 maintainer_email = aniekutmfonekere@gmail.com
 description = Learngual helper package
 long_description = file:README.rst
 long_description_content_type = text/x-rst
```

