# Comparing `tmp/django-aps-0.0.5.tar.gz` & `tmp/django-aps-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-aps-0.0.5.tar", last modified: Fri Jul 14 07:41:16 2023, max compression
+gzip compressed data, was "django-aps-0.0.6.tar", last modified: Fri Jul 14 07:47:51 2023, max compression
```

## Comparing `django-aps-0.0.5.tar` & `django-aps-0.0.6.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 07:41:16.782314 django-aps-0.0.5/
--rw-rw-rw-   0        0        0     1782 2023-07-14 07:41:16.782314 django-aps-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      790 2023-07-14 07:26:50.000000 django-aps-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 07:41:16.746936 django-aps-0.0.5/django_aps/
--rw-rw-rw-   0        0        0        0 2023-07-06 06:38:23.000000 django-aps-0.0.5/django_aps/__init__.py
--rw-rw-rw-   0        0        0       66 2023-07-06 06:38:23.000000 django-aps-0.0.5/django_aps/admin.py
--rw-rw-rw-   0        0        0      514 2023-07-14 07:26:50.000000 django-aps-0.0.5/django_aps/apps.py
--rw-rw-rw-   0        0        0     1017 2023-07-06 10:17:36.000000 django-aps-0.0.5/django_aps/base.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:41:16.763572 django-aps-0.0.5/django_aps/migrations/
--rw-rw-rw-   0        0        0     2250 2023-07-11 09:01:22.000000 django-aps-0.0.5/django_aps/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     3110 2023-07-14 07:26:50.000000 django-aps-0.0.5/django_aps/migrations/0002_auto_20230713_1145.py
--rw-rw-rw-   0        0        0      327 2023-07-14 07:26:50.000000 django-aps-0.0.5/django_aps/migrations/0003_delete_apschedulerjobinfo.py
--rw-rw-rw-   0        0        0        0 2023-07-06 06:38:23.000000 django-aps-0.0.5/django_aps/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:41:16.763572 django-aps-0.0.5/django_aps/model/
--rw-rw-rw-   0        0        0      380 2023-07-12 09:27:43.000000 django-aps-0.0.5/django_aps/model/__init__.py
--rw-rw-rw-   0        0        0     1951 2023-07-13 09:18:05.000000 django-aps-0.0.5/django_aps/model/aps_models.py
--rw-rw-rw-   0        0        0     1249 2023-07-13 09:58:54.000000 django-aps-0.0.5/django_aps/model/trigger_models.py
--rw-rw-rw-   0        0        0     2623 2023-07-13 09:18:05.000000 django-aps-0.0.5/django_aps/models.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:41:16.763572 django-aps-0.0.5/django_aps/repository/
--rw-rw-rw-   0        0        0      378 2023-07-07 06:27:53.000000 django-aps-0.0.5/django_aps/repository/__init__.py
--rw-rw-rw-   0        0        0      976 2023-07-14 07:26:50.000000 django-aps-0.0.5/django_aps/repository/apscheduler_func_model_mapper.py
--rw-rw-rw-   0        0        0      568 2023-07-14 07:26:50.000000 django-aps-0.0.5/django_aps/repository/apscheduler_job_model_mapper.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:41:16.763572 django-aps-0.0.5/django_aps/serializers/
--rw-rw-rw-   0        0        0      378 2023-07-06 10:20:02.000000 django-aps-0.0.5/django_aps/serializers/__init__.py
--rw-rw-rw-   0        0        0     3499 2023-07-13 10:51:03.000000 django-aps-0.0.5/django_aps/serializers/apscheduler_serializers.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:41:16.773090 django-aps-0.0.5/django_aps/service/
--rw-rw-rw-   0        0        0      378 2023-07-06 10:28:33.000000 django-aps-0.0.5/django_aps/service/__init__.py
--rw-rw-rw-   0        0        0     2182 2023-07-14 07:26:50.000000 django-aps-0.0.5/django_aps/service/discover_service.py
--rw-rw-rw-   0        0        0     8346 2023-07-14 07:26:50.000000 django-aps-0.0.5/django_aps/service/scheduler_service.py
--rw-rw-rw-   0        0        0     3251 2023-07-12 08:23:04.000000 django-aps-0.0.5/django_aps/settings.py
--rw-rw-rw-   0        0        0       63 2023-07-06 06:38:23.000000 django-aps-0.0.5/django_aps/tests.py
--rw-rw-rw-   0        0        0      742 2023-07-14 07:26:50.000000 django-aps-0.0.5/django_aps/urls.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:41:16.773090 django-aps-0.0.5/django_aps/utils/
--rw-rw-rw-   0        0        0        0 2023-07-14 01:53:06.000000 django-aps-0.0.5/django_aps/utils/__init__.py
--rw-rw-rw-   0        0        0      276 2023-07-07 09:13:35.000000 django-aps-0.0.5/django_aps/utils/common.py
--rw-rw-rw-   0        0        0     2066 2023-07-14 07:26:50.000000 django-aps-0.0.5/django_aps/utils/discover.py
--rw-rw-rw-   0        0        0     1714 2023-07-06 07:20:53.000000 django-aps-0.0.5/django_aps/utils/register.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:41:16.773090 django-aps-0.0.5/django_aps/views/
--rw-rw-rw-   0        0        0      378 2023-07-06 06:39:31.000000 django-aps-0.0.5/django_aps/views/__init__.py
--rw-rw-rw-   0        0        0     4304 2023-07-14 07:26:50.000000 django-aps-0.0.5/django_aps/views/apscheduler_view.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:41:16.746936 django-aps-0.0.5/django_aps.egg-info/
--rw-rw-rw-   0        0        0     1782 2023-07-14 07:41:16.000000 django-aps-0.0.5/django_aps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1364 2023-07-14 07:41:16.000000 django-aps-0.0.5/django_aps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 07:41:16.000000 django-aps-0.0.5/django_aps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-14 07:29:15.000000 django-aps-0.0.5/django_aps.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      100 2023-07-14 07:41:16.000000 django-aps-0.0.5/django_aps.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-14 07:41:16.000000 django-aps-0.0.5/django_aps.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-14 07:41:16.714092 django-aps-0.0.5/django_aps1/
-drwxrwxrwx   0        0        0        0 2023-07-14 07:41:16.746936 django-aps-0.0.5/django_aps1/utils/
--rw-rw-rw-   0        0        0      380 2023-07-11 03:50:12.000000 django-aps-0.0.5/django_aps1/utils/__init__.py
--rw-rw-rw-   0        0        0      712 2023-07-11 06:22:51.000000 django-aps-0.0.5/django_aps1/utils/loc_mem_cache.py
--rw-rw-rw-   0        0        0      164 2023-07-14 07:41:16.782314 django-aps-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1571 2023-07-14 07:41:01.000000 django-aps-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:41:16.733625 django-aps-0.0.5/test/
-drwxrwxrwx   0        0        0        0 2023-07-14 07:41:16.778745 django-aps-0.0.5/test/service/
--rw-rw-rw-   0        0        0      380 2023-07-11 07:05:44.000000 django-aps-0.0.5/test/service/__init__.py
--rw-rw-rw-   0        0        0     2983 2023-07-14 07:26:50.000000 django-aps-0.0.5/test/service/test_scheduler_service.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:41:16.778745 django-aps-0.0.5/test/utils/
--rw-rw-rw-   0        0        0      378 2023-07-07 09:40:04.000000 django-aps-0.0.5/test/utils/__init__.py
--rw-rw-rw-   0        0        0      894 2023-07-14 07:26:50.000000 django-aps-0.0.5/test/utils/test_discover.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:47:51.303259 django-aps-0.0.6/
+-rw-rw-rw-   0        0        0     1782 2023-07-14 07:47:51.303259 django-aps-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      790 2023-07-14 07:26:50.000000 django-aps-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 07:47:51.276406 django-aps-0.0.6/django_aps/
+-rw-rw-rw-   0        0        0        0 2023-07-06 06:38:23.000000 django-aps-0.0.6/django_aps/__init__.py
+-rw-rw-rw-   0        0        0       66 2023-07-06 06:38:23.000000 django-aps-0.0.6/django_aps/admin.py
+-rw-rw-rw-   0        0        0      514 2023-07-14 07:26:50.000000 django-aps-0.0.6/django_aps/apps.py
+-rw-rw-rw-   0        0        0     1017 2023-07-06 10:17:36.000000 django-aps-0.0.6/django_aps/base.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:47:51.286543 django-aps-0.0.6/django_aps/migrations/
+-rw-rw-rw-   0        0        0     2250 2023-07-11 09:01:22.000000 django-aps-0.0.6/django_aps/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     3110 2023-07-14 07:26:50.000000 django-aps-0.0.6/django_aps/migrations/0002_auto_20230713_1145.py
+-rw-rw-rw-   0        0        0      327 2023-07-14 07:26:50.000000 django-aps-0.0.6/django_aps/migrations/0003_delete_apschedulerjobinfo.py
+-rw-rw-rw-   0        0        0        0 2023-07-06 06:38:23.000000 django-aps-0.0.6/django_aps/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:47:51.286543 django-aps-0.0.6/django_aps/model/
+-rw-rw-rw-   0        0        0      380 2023-07-12 09:27:43.000000 django-aps-0.0.6/django_aps/model/__init__.py
+-rw-rw-rw-   0        0        0     1951 2023-07-13 09:18:05.000000 django-aps-0.0.6/django_aps/model/aps_models.py
+-rw-rw-rw-   0        0        0     1249 2023-07-13 09:58:54.000000 django-aps-0.0.6/django_aps/model/trigger_models.py
+-rw-rw-rw-   0        0        0     2623 2023-07-13 09:18:05.000000 django-aps-0.0.6/django_aps/models.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:47:51.286543 django-aps-0.0.6/django_aps/repository/
+-rw-rw-rw-   0        0        0      378 2023-07-07 06:27:53.000000 django-aps-0.0.6/django_aps/repository/__init__.py
+-rw-rw-rw-   0        0        0      976 2023-07-14 07:26:50.000000 django-aps-0.0.6/django_aps/repository/apscheduler_func_model_mapper.py
+-rw-rw-rw-   0        0        0      568 2023-07-14 07:26:50.000000 django-aps-0.0.6/django_aps/repository/apscheduler_job_model_mapper.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:47:51.286543 django-aps-0.0.6/django_aps/serializers/
+-rw-rw-rw-   0        0        0      378 2023-07-06 10:20:02.000000 django-aps-0.0.6/django_aps/serializers/__init__.py
+-rw-rw-rw-   0        0        0     3499 2023-07-13 10:51:03.000000 django-aps-0.0.6/django_aps/serializers/apscheduler_serializers.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:47:51.286543 django-aps-0.0.6/django_aps/service/
+-rw-rw-rw-   0        0        0      378 2023-07-06 10:28:33.000000 django-aps-0.0.6/django_aps/service/__init__.py
+-rw-rw-rw-   0        0        0     2182 2023-07-14 07:26:50.000000 django-aps-0.0.6/django_aps/service/discover_service.py
+-rw-rw-rw-   0        0        0     8346 2023-07-14 07:26:50.000000 django-aps-0.0.6/django_aps/service/scheduler_service.py
+-rw-rw-rw-   0        0        0     3251 2023-07-12 08:23:04.000000 django-aps-0.0.6/django_aps/settings.py
+-rw-rw-rw-   0        0        0       63 2023-07-06 06:38:23.000000 django-aps-0.0.6/django_aps/tests.py
+-rw-rw-rw-   0        0        0      742 2023-07-14 07:26:50.000000 django-aps-0.0.6/django_aps/urls.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:47:51.286543 django-aps-0.0.6/django_aps/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-14 01:53:06.000000 django-aps-0.0.6/django_aps/utils/__init__.py
+-rw-rw-rw-   0        0        0      276 2023-07-07 09:13:35.000000 django-aps-0.0.6/django_aps/utils/common.py
+-rw-rw-rw-   0        0        0     2066 2023-07-14 07:26:50.000000 django-aps-0.0.6/django_aps/utils/discover.py
+-rw-rw-rw-   0        0        0     1714 2023-07-06 07:20:53.000000 django-aps-0.0.6/django_aps/utils/register.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:47:51.286543 django-aps-0.0.6/django_aps/views/
+-rw-rw-rw-   0        0        0      378 2023-07-06 06:39:31.000000 django-aps-0.0.6/django_aps/views/__init__.py
+-rw-rw-rw-   0        0        0     4304 2023-07-14 07:26:50.000000 django-aps-0.0.6/django_aps/views/apscheduler_view.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:47:51.277416 django-aps-0.0.6/django_aps.egg-info/
+-rw-rw-rw-   0        0        0     1782 2023-07-14 07:47:51.000000 django-aps-0.0.6/django_aps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1364 2023-07-14 07:47:51.000000 django-aps-0.0.6/django_aps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 07:47:51.000000 django-aps-0.0.6/django_aps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-14 07:29:15.000000 django-aps-0.0.6/django_aps.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      100 2023-07-14 07:47:51.000000 django-aps-0.0.6/django_aps.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-14 07:47:51.000000 django-aps-0.0.6/django_aps.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 07:47:51.250784 django-aps-0.0.6/django_aps1/
+drwxrwxrwx   0        0        0        0 2023-07-14 07:47:51.277416 django-aps-0.0.6/django_aps1/utils/
+-rw-rw-rw-   0        0        0      380 2023-07-11 03:50:12.000000 django-aps-0.0.6/django_aps1/utils/__init__.py
+-rw-rw-rw-   0        0        0      712 2023-07-11 06:22:51.000000 django-aps-0.0.6/django_aps1/utils/loc_mem_cache.py
+-rw-rw-rw-   0        0        0      164 2023-07-14 07:47:51.303259 django-aps-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1630 2023-07-14 07:47:48.000000 django-aps-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:47:51.259416 django-aps-0.0.6/test/
+drwxrwxrwx   0        0        0        0 2023-07-14 07:47:51.302756 django-aps-0.0.6/test/service/
+-rw-rw-rw-   0        0        0      380 2023-07-11 07:05:44.000000 django-aps-0.0.6/test/service/__init__.py
+-rw-rw-rw-   0        0        0     2983 2023-07-14 07:26:50.000000 django-aps-0.0.6/test/service/test_scheduler_service.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:47:51.303259 django-aps-0.0.6/test/utils/
+-rw-rw-rw-   0        0        0      378 2023-07-07 09:40:04.000000 django-aps-0.0.6/test/utils/__init__.py
+-rw-rw-rw-   0        0        0      894 2023-07-14 07:26:50.000000 django-aps-0.0.6/test/utils/test_discover.py
```

### Comparing `django-aps-0.0.5/PKG-INFO` & `django-aps-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-aps
-Version: 0.0.5
+Version: 0.0.6
 Summary: APScheduler Register for Django
 Home-page: https://github.com/cuidingyong/django-aps
 Author: Dillon
 Author-email: cuidingyong@yeah.net
 License: MIT
 Keywords: django apscheduler django-django_aps register
 Platform: UNKNOWN
```

### Comparing `django-aps-0.0.5/README.md` & `django-aps-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `django-aps-0.0.5/django_aps/apps.py` & `django-aps-0.0.6/django_aps/apps.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.0.5/django_aps/base.py` & `django-aps-0.0.6/django_aps/base.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.0.5/django_aps/migrations/0001_initial.py` & `django-aps-0.0.6/django_aps/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.0.5/django_aps/migrations/0002_auto_20230713_1145.py` & `django-aps-0.0.6/django_aps/migrations/0002_auto_20230713_1145.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.0.5/django_aps/model/aps_models.py` & `django-aps-0.0.6/django_aps/model/aps_models.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.0.5/django_aps/model/trigger_models.py` & `django-aps-0.0.6/django_aps/model/trigger_models.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.0.5/django_aps/models.py` & `django-aps-0.0.6/django_aps/models.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.0.5/django_aps/repository/apscheduler_func_model_mapper.py` & `django-aps-0.0.6/django_aps/repository/apscheduler_func_model_mapper.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.0.5/django_aps/repository/apscheduler_job_model_mapper.py` & `django-aps-0.0.6/django_aps/repository/apscheduler_job_model_mapper.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.0.5/django_aps/serializers/apscheduler_serializers.py` & `django-aps-0.0.6/django_aps/serializers/apscheduler_serializers.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.0.5/django_aps/service/discover_service.py` & `django-aps-0.0.6/django_aps/service/discover_service.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.0.5/django_aps/service/scheduler_service.py` & `django-aps-0.0.6/django_aps/service/scheduler_service.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.0.5/django_aps/settings.py` & `django-aps-0.0.6/django_aps/settings.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.0.5/django_aps/urls.py` & `django-aps-0.0.6/django_aps/urls.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.0.5/django_aps/utils/discover.py` & `django-aps-0.0.6/django_aps/utils/discover.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.0.5/django_aps/utils/register.py` & `django-aps-0.0.6/django_aps/utils/register.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.0.5/django_aps/views/apscheduler_view.py` & `django-aps-0.0.6/django_aps/views/apscheduler_view.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.0.5/django_aps.egg-info/PKG-INFO` & `django-aps-0.0.6/django_aps.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-aps
-Version: 0.0.5
+Version: 0.0.6
 Summary: APScheduler Register for Django
 Home-page: https://github.com/cuidingyong/django-aps
 Author: Dillon
 Author-email: cuidingyong@yeah.net
 License: MIT
 Keywords: django apscheduler django-django_aps register
 Platform: UNKNOWN
```

### Comparing `django-aps-0.0.5/django_aps.egg-info/SOURCES.txt` & `django-aps-0.0.6/django_aps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-aps-0.0.5/django_aps1/utils/loc_mem_cache.py` & `django-aps-0.0.6/django_aps1/utils/loc_mem_cache.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.0.5/setup.py` & `django-aps-0.0.6/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="django-aps",
-    version="0.0.5",
+    version="0.0.6",
     description="APScheduler Register for Django",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cuidingyong/django-aps",
     author="Dillon",
     author_email="cuidingyong@yeah.net",
     license="MIT",
@@ -30,15 +30,15 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Framework :: Django",
         "Framework :: Django :: 3.2",
         "Framework :: Django :: 4.0",
     ],
     keywords="django apscheduler django-django_aps register",
-    packages=["django_aps"],
+    packages=find_packages(exclude=["django_aps1", "django_aps1.*", "test", "test.*"]),
     install_requires=[
         "django>=3.2",
         "apscheduler>=3.2,<4.0",
         "djangorestframework>=3.14",
         "django-apscheduler>=0.6.2",
         "pydantic>=2.0"
     ],
```

### Comparing `django-aps-0.0.5/test/service/test_scheduler_service.py` & `django-aps-0.0.6/test/service/test_scheduler_service.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.0.5/test/utils/test_discover.py` & `django-aps-0.0.6/test/utils/test_discover.py`

 * *Files identical despite different names*

