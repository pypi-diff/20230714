# Comparing `tmp/django-aps-0.1.0.tar.gz` & `tmp/django-aps-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-aps-0.1.0.tar", last modified: Fri Jul 14 08:35:55 2023, max compression
+gzip compressed data, was "django-aps-0.1.1.tar", last modified: Fri Jul 14 08:38:39 2023, max compression
```

## Comparing `django-aps-0.1.0.tar` & `django-aps-0.1.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 08:35:55.168914 django-aps-0.1.0/
--rw-rw-rw-   0        0        0       58 2023-07-14 07:58:26.000000 django-aps-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1781 2023-07-14 08:35:55.168914 django-aps-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      789 2023-07-14 08:13:26.000000 django-aps-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 08:35:55.154914 django-aps-0.1.0/django_aps/
--rw-rw-rw-   0        0        0        0 2023-07-06 06:38:23.000000 django-aps-0.1.0/django_aps/__init__.py
--rw-rw-rw-   0        0        0       66 2023-07-06 06:38:23.000000 django-aps-0.1.0/django_aps/admin.py
--rw-rw-rw-   0        0        0      514 2023-07-14 07:26:50.000000 django-aps-0.1.0/django_aps/apps.py
--rw-rw-rw-   0        0        0     1017 2023-07-06 10:17:36.000000 django-aps-0.1.0/django_aps/base.py
-drwxrwxrwx   0        0        0        0 2023-07-14 08:35:55.160916 django-aps-0.1.0/django_aps/migrations/
--rw-rw-rw-   0        0        0     1111 2023-07-14 08:12:24.000000 django-aps-0.1.0/django_aps/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2023-07-06 06:38:23.000000 django-aps-0.1.0/django_aps/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 08:35:55.161915 django-aps-0.1.0/django_aps/model/
--rw-rw-rw-   0        0        0        0 2023-07-14 08:13:26.000000 django-aps-0.1.0/django_aps/model/__init__.py
--rw-rw-rw-   0        0        0     1951 2023-07-13 09:18:05.000000 django-aps-0.1.0/django_aps/model/aps_models.py
--rw-rw-rw-   0        0        0     1249 2023-07-13 09:58:54.000000 django-aps-0.1.0/django_aps/model/trigger_models.py
--rw-rw-rw-   0        0        0     2623 2023-07-13 09:18:05.000000 django-aps-0.1.0/django_aps/models.py
-drwxrwxrwx   0        0        0        0 2023-07-14 08:35:55.162914 django-aps-0.1.0/django_aps/repository/
--rw-rw-rw-   0        0        0        0 2023-07-14 08:13:27.000000 django-aps-0.1.0/django_aps/repository/__init__.py
--rw-rw-rw-   0        0        0      976 2023-07-14 07:26:50.000000 django-aps-0.1.0/django_aps/repository/apscheduler_func_model_mapper.py
--rw-rw-rw-   0        0        0      568 2023-07-14 07:26:50.000000 django-aps-0.1.0/django_aps/repository/apscheduler_job_model_mapper.py
-drwxrwxrwx   0        0        0        0 2023-07-14 08:35:55.163914 django-aps-0.1.0/django_aps/serializers/
--rw-rw-rw-   0        0        0      378 2023-07-06 10:20:02.000000 django-aps-0.1.0/django_aps/serializers/__init__.py
--rw-rw-rw-   0        0        0     3499 2023-07-13 10:51:03.000000 django-aps-0.1.0/django_aps/serializers/apscheduler_serializers.py
-drwxrwxrwx   0        0        0        0 2023-07-14 08:35:55.165915 django-aps-0.1.0/django_aps/service/
--rw-rw-rw-   0        0        0      378 2023-07-06 10:28:33.000000 django-aps-0.1.0/django_aps/service/__init__.py
--rw-rw-rw-   0        0        0     2182 2023-07-14 07:26:50.000000 django-aps-0.1.0/django_aps/service/discover_service.py
--rw-rw-rw-   0        0        0     8346 2023-07-14 07:26:50.000000 django-aps-0.1.0/django_aps/service/scheduler_service.py
--rw-rw-rw-   0        0        0     3251 2023-07-12 08:23:04.000000 django-aps-0.1.0/django_aps/settings.py
--rw-rw-rw-   0        0        0       63 2023-07-06 06:38:23.000000 django-aps-0.1.0/django_aps/tests.py
--rw-rw-rw-   0        0        0      742 2023-07-14 07:26:50.000000 django-aps-0.1.0/django_aps/urls.py
-drwxrwxrwx   0        0        0        0 2023-07-14 08:35:55.166914 django-aps-0.1.0/django_aps/utils/
--rw-rw-rw-   0        0        0        0 2023-07-14 01:53:06.000000 django-aps-0.1.0/django_aps/utils/__init__.py
--rw-rw-rw-   0        0        0      276 2023-07-07 09:13:35.000000 django-aps-0.1.0/django_aps/utils/common.py
--rw-rw-rw-   0        0        0     2066 2023-07-14 07:26:50.000000 django-aps-0.1.0/django_aps/utils/discover.py
--rw-rw-rw-   0        0        0     1714 2023-07-06 07:20:53.000000 django-aps-0.1.0/django_aps/utils/register.py
-drwxrwxrwx   0        0        0        0 2023-07-14 08:35:55.167915 django-aps-0.1.0/django_aps/views/
--rw-rw-rw-   0        0        0      378 2023-07-06 06:39:31.000000 django-aps-0.1.0/django_aps/views/__init__.py
--rw-rw-rw-   0        0        0     4304 2023-07-14 07:26:50.000000 django-aps-0.1.0/django_aps/views/apscheduler_view.py
-drwxrwxrwx   0        0        0        0 2023-07-14 08:35:55.159921 django-aps-0.1.0/django_aps.egg-info/
--rw-rw-rw-   0        0        0     1781 2023-07-14 08:35:55.000000 django-aps-0.1.0/django_aps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1091 2023-07-14 08:35:55.000000 django-aps-0.1.0/django_aps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 08:35:55.000000 django-aps-0.1.0/django_aps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-14 08:35:55.000000 django-aps-0.1.0/django_aps.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      100 2023-07-14 08:35:55.000000 django-aps-0.1.0/django_aps.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-14 08:35:55.000000 django-aps-0.1.0/django_aps.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      164 2023-07-14 08:35:55.169917 django-aps-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1630 2023-07-14 08:35:40.000000 django-aps-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 08:38:39.779996 django-aps-0.1.1/
+-rw-rw-rw-   0        0        0       58 2023-07-14 07:58:26.000000 django-aps-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1781 2023-07-14 08:38:39.779996 django-aps-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      789 2023-07-14 08:13:26.000000 django-aps-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 08:38:39.764997 django-aps-0.1.1/django_aps/
+-rw-rw-rw-   0        0        0        0 2023-07-06 06:38:23.000000 django-aps-0.1.1/django_aps/__init__.py
+-rw-rw-rw-   0        0        0       66 2023-07-06 06:38:23.000000 django-aps-0.1.1/django_aps/admin.py
+-rw-rw-rw-   0        0        0      514 2023-07-14 07:26:50.000000 django-aps-0.1.1/django_aps/apps.py
+-rw-rw-rw-   0        0        0     1017 2023-07-06 10:17:36.000000 django-aps-0.1.1/django_aps/base.py
+drwxrwxrwx   0        0        0        0 2023-07-14 08:38:39.771006 django-aps-0.1.1/django_aps/migrations/
+-rw-rw-rw-   0        0        0     1111 2023-07-14 08:12:24.000000 django-aps-0.1.1/django_aps/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2023-07-06 06:38:23.000000 django-aps-0.1.1/django_aps/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 08:38:39.771999 django-aps-0.1.1/django_aps/model/
+-rw-rw-rw-   0        0        0        0 2023-07-14 08:13:26.000000 django-aps-0.1.1/django_aps/model/__init__.py
+-rw-rw-rw-   0        0        0     1951 2023-07-13 09:18:05.000000 django-aps-0.1.1/django_aps/model/aps_models.py
+-rw-rw-rw-   0        0        0     1249 2023-07-13 09:58:54.000000 django-aps-0.1.1/django_aps/model/trigger_models.py
+-rw-rw-rw-   0        0        0     2623 2023-07-13 09:18:05.000000 django-aps-0.1.1/django_aps/models.py
+drwxrwxrwx   0        0        0        0 2023-07-14 08:38:39.773998 django-aps-0.1.1/django_aps/repository/
+-rw-rw-rw-   0        0        0        0 2023-07-14 08:13:27.000000 django-aps-0.1.1/django_aps/repository/__init__.py
+-rw-rw-rw-   0        0        0      976 2023-07-14 07:26:50.000000 django-aps-0.1.1/django_aps/repository/apscheduler_func_model_mapper.py
+-rw-rw-rw-   0        0        0      568 2023-07-14 07:26:50.000000 django-aps-0.1.1/django_aps/repository/apscheduler_job_model_mapper.py
+drwxrwxrwx   0        0        0        0 2023-07-14 08:38:39.774995 django-aps-0.1.1/django_aps/serializers/
+-rw-rw-rw-   0        0        0      378 2023-07-06 10:20:02.000000 django-aps-0.1.1/django_aps/serializers/__init__.py
+-rw-rw-rw-   0        0        0     3499 2023-07-13 10:51:03.000000 django-aps-0.1.1/django_aps/serializers/apscheduler_serializers.py
+drwxrwxrwx   0        0        0        0 2023-07-14 08:38:39.775995 django-aps-0.1.1/django_aps/service/
+-rw-rw-rw-   0        0        0      378 2023-07-06 10:28:33.000000 django-aps-0.1.1/django_aps/service/__init__.py
+-rw-rw-rw-   0        0        0     2182 2023-07-14 07:26:50.000000 django-aps-0.1.1/django_aps/service/discover_service.py
+-rw-rw-rw-   0        0        0     8346 2023-07-14 07:26:50.000000 django-aps-0.1.1/django_aps/service/scheduler_service.py
+-rw-rw-rw-   0        0        0     3251 2023-07-12 08:23:04.000000 django-aps-0.1.1/django_aps/settings.py
+-rw-rw-rw-   0        0        0       63 2023-07-06 06:38:23.000000 django-aps-0.1.1/django_aps/tests.py
+-rw-rw-rw-   0        0        0      742 2023-07-14 07:26:50.000000 django-aps-0.1.1/django_aps/urls.py
+drwxrwxrwx   0        0        0        0 2023-07-14 08:38:39.777996 django-aps-0.1.1/django_aps/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-14 01:53:06.000000 django-aps-0.1.1/django_aps/utils/__init__.py
+-rw-rw-rw-   0        0        0      276 2023-07-07 09:13:35.000000 django-aps-0.1.1/django_aps/utils/common.py
+-rw-rw-rw-   0        0        0     2066 2023-07-14 07:26:50.000000 django-aps-0.1.1/django_aps/utils/discover.py
+-rw-rw-rw-   0        0        0     1714 2023-07-06 07:20:53.000000 django-aps-0.1.1/django_aps/utils/register.py
+drwxrwxrwx   0        0        0        0 2023-07-14 08:38:39.778996 django-aps-0.1.1/django_aps/views/
+-rw-rw-rw-   0        0        0      378 2023-07-06 06:39:31.000000 django-aps-0.1.1/django_aps/views/__init__.py
+-rw-rw-rw-   0        0        0     4304 2023-07-14 07:26:50.000000 django-aps-0.1.1/django_aps/views/apscheduler_view.py
+drwxrwxrwx   0        0        0        0 2023-07-14 08:38:39.769002 django-aps-0.1.1/django_aps.egg-info/
+-rw-rw-rw-   0        0        0     1781 2023-07-14 08:38:39.000000 django-aps-0.1.1/django_aps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1091 2023-07-14 08:38:39.000000 django-aps-0.1.1/django_aps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 08:38:39.000000 django-aps-0.1.1/django_aps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-14 08:38:39.000000 django-aps-0.1.1/django_aps.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      100 2023-07-14 08:38:39.000000 django-aps-0.1.1/django_aps.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-14 08:38:39.000000 django-aps-0.1.1/django_aps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      164 2023-07-14 08:38:39.779996 django-aps-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1630 2023-07-14 08:38:34.000000 django-aps-0.1.1/setup.py
```

### Comparing `django-aps-0.1.0/PKG-INFO` & `django-aps-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-aps
-Version: 0.1.0
+Version: 0.1.1
 Summary: APScheduler Register for Django
 Home-page: https://github.com/cuidingyong/django-aps
 Author: Dillon
 Author-email: cuidingyong@yeah.net
 License: MIT
 Keywords: django apscheduler django-django_aps register
 Platform: UNKNOWN
```

### Comparing `django-aps-0.1.0/README.md` & `django-aps-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `django-aps-0.1.0/django_aps/apps.py` & `django-aps-0.1.1/django_aps/apps.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.1.0/django_aps/base.py` & `django-aps-0.1.1/django_aps/base.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.1.0/django_aps/migrations/0001_initial.py` & `django-aps-0.1.1/django_aps/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.1.0/django_aps/model/aps_models.py` & `django-aps-0.1.1/django_aps/model/aps_models.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.1.0/django_aps/model/trigger_models.py` & `django-aps-0.1.1/django_aps/model/trigger_models.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.1.0/django_aps/models.py` & `django-aps-0.1.1/django_aps/models.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.1.0/django_aps/repository/apscheduler_func_model_mapper.py` & `django-aps-0.1.1/django_aps/repository/apscheduler_func_model_mapper.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.1.0/django_aps/repository/apscheduler_job_model_mapper.py` & `django-aps-0.1.1/django_aps/repository/apscheduler_job_model_mapper.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.1.0/django_aps/serializers/apscheduler_serializers.py` & `django-aps-0.1.1/django_aps/serializers/apscheduler_serializers.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.1.0/django_aps/service/discover_service.py` & `django-aps-0.1.1/django_aps/service/discover_service.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.1.0/django_aps/service/scheduler_service.py` & `django-aps-0.1.1/django_aps/service/scheduler_service.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.1.0/django_aps/settings.py` & `django-aps-0.1.1/django_aps/settings.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.1.0/django_aps/urls.py` & `django-aps-0.1.1/django_aps/urls.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.1.0/django_aps/utils/discover.py` & `django-aps-0.1.1/django_aps/utils/discover.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.1.0/django_aps/utils/register.py` & `django-aps-0.1.1/django_aps/utils/register.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.1.0/django_aps/views/apscheduler_view.py` & `django-aps-0.1.1/django_aps/views/apscheduler_view.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.1.0/django_aps.egg-info/PKG-INFO` & `django-aps-0.1.1/django_aps.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-aps
-Version: 0.1.0
+Version: 0.1.1
 Summary: APScheduler Register for Django
 Home-page: https://github.com/cuidingyong/django-aps
 Author: Dillon
 Author-email: cuidingyong@yeah.net
 License: MIT
 Keywords: django apscheduler django-django_aps register
 Platform: UNKNOWN
```

### Comparing `django-aps-0.1.0/django_aps.egg-info/SOURCES.txt` & `django-aps-0.1.1/django_aps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-aps-0.1.0/setup.py` & `django-aps-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="django-aps",
-    version="0.1.0",
+    version="0.1.1",
     description="APScheduler Register for Django",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cuidingyong/django-aps",
     author="Dillon",
     author_email="cuidingyong@yeah.net",
     license="MIT",
```

