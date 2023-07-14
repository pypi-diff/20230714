# Comparing `tmp/django-aps-0.0.1.tar.gz` & `tmp/django-aps-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\django-aps-0.0.1.tar", last modified: Fri Jul 14 07:16:17 2023, max compression
+gzip compressed data, was "django-aps-0.0.2.tar", last modified: Fri Jul 14 07:29:15 2023, max compression
```

## Comparing `django-aps-0.0.1.tar` & `django-aps-0.0.2.tar`

### file list

```diff
@@ -1,40 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 07:16:17.000000 django-aps-0.0.1/
--rw-rw-rw-   0        0        0     2063 2023-07-14 07:16:17.000000 django-aps-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      789 2023-07-14 07:05:34.000000 django-aps-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 07:16:17.000000 django-aps-0.0.1/django_aps.egg-info/
--rw-rw-rw-   0        0        0     2063 2023-07-14 07:16:17.000000 django-aps-0.0.1/django_aps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      789 2023-07-14 07:16:17.000000 django-aps-0.0.1/django_aps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 07:16:17.000000 django-aps-0.0.1/django_aps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-14 07:13:29.000000 django-aps-0.0.1/django_aps.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      100 2023-07-14 07:16:17.000000 django-aps-0.0.1/django_aps.egg-info/requires.txt
--rw-rw-rw-   0        0        0       60 2023-07-14 07:16:17.000000 django-aps-0.0.1/django_aps.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-14 07:16:17.000000 django-aps-0.0.1/migrations/
--rw-rw-rw-   0        0        0     2250 2023-07-11 09:01:22.000000 django-aps-0.0.1/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     3103 2023-07-13 03:45:17.000000 django-aps-0.0.1/migrations/0002_auto_20230713_1145.py
--rw-rw-rw-   0        0        0      320 2023-07-13 09:18:07.000000 django-aps-0.0.1/migrations/0003_delete_apschedulerjobinfo.py
--rw-rw-rw-   0        0        0        0 2023-07-06 06:38:23.000000 django-aps-0.0.1/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:16:17.000000 django-aps-0.0.1/model/
--rw-rw-rw-   0        0        0      380 2023-07-12 09:27:43.000000 django-aps-0.0.1/model/__init__.py
--rw-rw-rw-   0        0        0     1951 2023-07-13 09:18:05.000000 django-aps-0.0.1/model/aps_models.py
--rw-rw-rw-   0        0        0     1249 2023-07-13 09:58:54.000000 django-aps-0.0.1/model/trigger_models.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:16:17.000000 django-aps-0.0.1/repository/
--rw-rw-rw-   0        0        0      378 2023-07-07 06:27:53.000000 django-aps-0.0.1/repository/__init__.py
--rw-rw-rw-   0        0        0      969 2023-07-13 10:51:03.000000 django-aps-0.0.1/repository/apscheduler_func_model_mapper.py
--rw-rw-rw-   0        0        0      561 2023-07-13 10:51:03.000000 django-aps-0.0.1/repository/apscheduler_job_model_mapper.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:16:17.000000 django-aps-0.0.1/serializers/
--rw-rw-rw-   0        0        0      378 2023-07-06 10:20:02.000000 django-aps-0.0.1/serializers/__init__.py
--rw-rw-rw-   0        0        0     3499 2023-07-13 10:51:03.000000 django-aps-0.0.1/serializers/apscheduler_serializers.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:16:17.000000 django-aps-0.0.1/service/
--rw-rw-rw-   0        0        0      378 2023-07-06 10:28:33.000000 django-aps-0.0.1/service/__init__.py
--rw-rw-rw-   0        0        0     2147 2023-07-14 02:44:22.000000 django-aps-0.0.1/service/discover_service.py
--rw-rw-rw-   0        0        0     8325 2023-07-13 10:51:03.000000 django-aps-0.0.1/service/scheduler_service.py
--rw-rw-rw-   0        0        0      145 2023-07-14 07:16:17.000000 django-aps-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1583 2023-07-14 07:12:20.000000 django-aps-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:16:17.000000 django-aps-0.0.1/utils/
--rw-rw-rw-   0        0        0        0 2023-07-14 01:53:06.000000 django-aps-0.0.1/utils/__init__.py
--rw-rw-rw-   0        0        0      276 2023-07-07 09:13:35.000000 django-aps-0.0.1/utils/common.py
--rw-rw-rw-   0        0        0     2052 2023-07-11 09:02:41.000000 django-aps-0.0.1/utils/discover.py
--rw-rw-rw-   0        0        0     1714 2023-07-06 07:20:53.000000 django-aps-0.0.1/utils/register.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:16:17.000000 django-aps-0.0.1/views/
--rw-rw-rw-   0        0        0      378 2023-07-06 06:39:31.000000 django-aps-0.0.1/views/__init__.py
--rw-rw-rw-   0        0        0     4276 2023-07-13 10:51:03.000000 django-aps-0.0.1/views/apscheduler_view.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:29:15.915365 django-aps-0.0.2/
+-rw-rw-rw-   0        0        0     1782 2023-07-14 07:29:15.915365 django-aps-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      790 2023-07-14 07:26:50.000000 django-aps-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 07:29:15.865848 django-aps-0.0.2/django_aps/
+-rw-rw-rw-   0        0        0        0 2023-07-06 06:38:23.000000 django-aps-0.0.2/django_aps/__init__.py
+-rw-rw-rw-   0        0        0       66 2023-07-06 06:38:23.000000 django-aps-0.0.2/django_aps/admin.py
+-rw-rw-rw-   0        0        0      514 2023-07-14 07:26:50.000000 django-aps-0.0.2/django_aps/apps.py
+-rw-rw-rw-   0        0        0     1017 2023-07-06 10:17:36.000000 django-aps-0.0.2/django_aps/base.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:29:15.882145 django-aps-0.0.2/django_aps/migrations/
+-rw-rw-rw-   0        0        0     2250 2023-07-11 09:01:22.000000 django-aps-0.0.2/django_aps/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     3110 2023-07-14 07:26:50.000000 django-aps-0.0.2/django_aps/migrations/0002_auto_20230713_1145.py
+-rw-rw-rw-   0        0        0      327 2023-07-14 07:26:50.000000 django-aps-0.0.2/django_aps/migrations/0003_delete_apschedulerjobinfo.py
+-rw-rw-rw-   0        0        0        0 2023-07-06 06:38:23.000000 django-aps-0.0.2/django_aps/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:29:15.882145 django-aps-0.0.2/django_aps/model/
+-rw-rw-rw-   0        0        0      380 2023-07-12 09:27:43.000000 django-aps-0.0.2/django_aps/model/__init__.py
+-rw-rw-rw-   0        0        0     1951 2023-07-13 09:18:05.000000 django-aps-0.0.2/django_aps/model/aps_models.py
+-rw-rw-rw-   0        0        0     1249 2023-07-13 09:58:54.000000 django-aps-0.0.2/django_aps/model/trigger_models.py
+-rw-rw-rw-   0        0        0     2623 2023-07-13 09:18:05.000000 django-aps-0.0.2/django_aps/models.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:29:15.882145 django-aps-0.0.2/django_aps/repository/
+-rw-rw-rw-   0        0        0      378 2023-07-07 06:27:53.000000 django-aps-0.0.2/django_aps/repository/__init__.py
+-rw-rw-rw-   0        0        0      976 2023-07-14 07:26:50.000000 django-aps-0.0.2/django_aps/repository/apscheduler_func_model_mapper.py
+-rw-rw-rw-   0        0        0      568 2023-07-14 07:26:50.000000 django-aps-0.0.2/django_aps/repository/apscheduler_job_model_mapper.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:29:15.882145 django-aps-0.0.2/django_aps/serializers/
+-rw-rw-rw-   0        0        0      378 2023-07-06 10:20:02.000000 django-aps-0.0.2/django_aps/serializers/__init__.py
+-rw-rw-rw-   0        0        0     3499 2023-07-13 10:51:03.000000 django-aps-0.0.2/django_aps/serializers/apscheduler_serializers.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:29:15.882145 django-aps-0.0.2/django_aps/service/
+-rw-rw-rw-   0        0        0      378 2023-07-06 10:28:33.000000 django-aps-0.0.2/django_aps/service/__init__.py
+-rw-rw-rw-   0        0        0     2182 2023-07-14 07:26:50.000000 django-aps-0.0.2/django_aps/service/discover_service.py
+-rw-rw-rw-   0        0        0     8346 2023-07-14 07:26:50.000000 django-aps-0.0.2/django_aps/service/scheduler_service.py
+-rw-rw-rw-   0        0        0     3251 2023-07-12 08:23:04.000000 django-aps-0.0.2/django_aps/settings.py
+-rw-rw-rw-   0        0        0       63 2023-07-06 06:38:23.000000 django-aps-0.0.2/django_aps/tests.py
+-rw-rw-rw-   0        0        0      742 2023-07-14 07:26:50.000000 django-aps-0.0.2/django_aps/urls.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:29:15.899229 django-aps-0.0.2/django_aps/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-14 01:53:06.000000 django-aps-0.0.2/django_aps/utils/__init__.py
+-rw-rw-rw-   0        0        0      276 2023-07-07 09:13:35.000000 django-aps-0.0.2/django_aps/utils/common.py
+-rw-rw-rw-   0        0        0     2066 2023-07-14 07:26:50.000000 django-aps-0.0.2/django_aps/utils/discover.py
+-rw-rw-rw-   0        0        0     1714 2023-07-06 07:20:53.000000 django-aps-0.0.2/django_aps/utils/register.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:29:15.901344 django-aps-0.0.2/django_aps/views/
+-rw-rw-rw-   0        0        0      378 2023-07-06 06:39:31.000000 django-aps-0.0.2/django_aps/views/__init__.py
+-rw-rw-rw-   0        0        0     4304 2023-07-14 07:26:50.000000 django-aps-0.0.2/django_aps/views/apscheduler_view.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:29:15.865848 django-aps-0.0.2/django_aps.egg-info/
+-rw-rw-rw-   0        0        0     1782 2023-07-14 07:29:15.000000 django-aps-0.0.2/django_aps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1364 2023-07-14 07:29:15.000000 django-aps-0.0.2/django_aps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 07:29:15.000000 django-aps-0.0.2/django_aps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-14 07:29:15.000000 django-aps-0.0.2/django_aps.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      100 2023-07-14 07:29:15.000000 django-aps-0.0.2/django_aps.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-07-14 07:29:15.000000 django-aps-0.0.2/django_aps.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 07:29:15.849824 django-aps-0.0.2/django_aps1/
+drwxrwxrwx   0        0        0        0 2023-07-14 07:29:15.882145 django-aps-0.0.2/django_aps1/utils/
+-rw-rw-rw-   0        0        0      380 2023-07-11 03:50:12.000000 django-aps-0.0.2/django_aps1/utils/__init__.py
+-rw-rw-rw-   0        0        0      712 2023-07-11 06:22:51.000000 django-aps-0.0.2/django_aps1/utils/loc_mem_cache.py
+-rw-rw-rw-   0        0        0      145 2023-07-14 07:29:15.915365 django-aps-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1612 2023-07-14 07:29:01.000000 django-aps-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:29:15.849824 django-aps-0.0.2/test/
+drwxrwxrwx   0        0        0        0 2023-07-14 07:29:15.901344 django-aps-0.0.2/test/service/
+-rw-rw-rw-   0        0        0      380 2023-07-11 07:05:44.000000 django-aps-0.0.2/test/service/__init__.py
+-rw-rw-rw-   0        0        0     2983 2023-07-14 07:26:50.000000 django-aps-0.0.2/test/service/test_scheduler_service.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:29:15.915365 django-aps-0.0.2/test/utils/
+-rw-rw-rw-   0        0        0      378 2023-07-07 09:40:04.000000 django-aps-0.0.2/test/utils/__init__.py
+-rw-rw-rw-   0        0        0      894 2023-07-14 07:26:50.000000 django-aps-0.0.2/test/utils/test_discover.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-aps-0.0.1/PKG-INFO` & `django-aps-0.0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,52 +1,16 @@
 Metadata-Version: 2.1
 Name: django-aps
-Version: 0.0.1
+Version: 0.0.2
 Summary: APScheduler Register for Django
 Home-page: https://github.com/cuidingyong/django-aps
 Author: Dillon
 Author-email: cuidingyong@yeah.net
 License: MIT
-Description: # Django APScheduler Register
-        
-        Django-aps adds the task registration discovery function on the basis of A,
-        which is more convenient for users to realize the configuration of scheduled tasks.
-        
-        ## Installation
-        
-        ```commandline
-        pip install django-aps
-        ```
-        
-        ## Quick start
-        
-        - Add ``aps`` to your ``INSTALLED_APPS`` setting like this:
-        
-        ```python
-        INSTALLED_APPS = (
-            # ...
-            "django_aps",
-        )
-        ```
-        
-        - django-aps comes with sensible configuration defaults out of the box. The defaults can be overridden by adding
-          the following settings to your Django `settings.py` file:
-        
-        ```python
-        DEFAULT_DISCOVER_SCHEMA = 'pkg'
-        ```
-        
-        - Run `python manage.py migrate` to create the django_apscheduler models.
-        
-        - Register a APScheduler function in your project
-        
-        ```python
-        
-        ```
-Keywords: django apscheduler django-aps register
+Keywords: django apscheduler django-django_aps register
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -55,7 +19,45 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Description-Content-Type: text/markdown
+
+# Django APScheduler Register
+
+Django-aps adds the task registration discovery function on the basis of A,
+which is more convenient for users to realize the configuration of scheduled tasks.
+
+## Installation
+
+```commandline
+pip install django-aps
+```
+
+## Quick start
+
+- Add ``aps`` to your ``INSTALLED_APPS`` setting like this:
+
+```python
+INSTALLED_APPS = (
+    # ...
+    "django_aps1",
+)
+```
+
+- django-aps comes with sensible configuration defaults out of the box. The defaults can be overridden by adding
+  the following settings to your Django `settings.py` file:
+
+```python
+DEFAULT_DISCOVER_SCHEMA = 'pkg'
+```
+
+- Run `python manage.py migrate` to create the django_apscheduler models.
+
+- Register a APScheduler function in your project
+
+```python
+
+```
+
```

### Comparing `django-aps-0.0.1/README.md` & `django-aps-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ## Quick start
 
 - Add ``aps`` to your ``INSTALLED_APPS`` setting like this:
 
 ```python
 INSTALLED_APPS = (
     # ...
-    "django_aps",
+    "django_aps1",
 )
 ```
 
 - django-aps comes with sensible configuration defaults out of the box. The defaults can be overridden by adding
   the following settings to your Django `settings.py` file:
 
 ```python
```

### Comparing `django-aps-0.0.1/django_aps.egg-info/PKG-INFO` & `django-aps-0.0.2/django_aps.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,52 +1,16 @@
 Metadata-Version: 2.1
 Name: django-aps
-Version: 0.0.1
+Version: 0.0.2
 Summary: APScheduler Register for Django
 Home-page: https://github.com/cuidingyong/django-aps
 Author: Dillon
 Author-email: cuidingyong@yeah.net
 License: MIT
-Description: # Django APScheduler Register
-        
-        Django-aps adds the task registration discovery function on the basis of A,
-        which is more convenient for users to realize the configuration of scheduled tasks.
-        
-        ## Installation
-        
-        ```commandline
-        pip install django-aps
-        ```
-        
-        ## Quick start
-        
-        - Add ``aps`` to your ``INSTALLED_APPS`` setting like this:
-        
-        ```python
-        INSTALLED_APPS = (
-            # ...
-            "django_aps",
-        )
-        ```
-        
-        - django-aps comes with sensible configuration defaults out of the box. The defaults can be overridden by adding
-          the following settings to your Django `settings.py` file:
-        
-        ```python
-        DEFAULT_DISCOVER_SCHEMA = 'pkg'
-        ```
-        
-        - Run `python manage.py migrate` to create the django_apscheduler models.
-        
-        - Register a APScheduler function in your project
-        
-        ```python
-        
-        ```
-Keywords: django apscheduler django-aps register
+Keywords: django apscheduler django-django_aps register
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -55,7 +19,45 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Description-Content-Type: text/markdown
+
+# Django APScheduler Register
+
+Django-aps adds the task registration discovery function on the basis of A,
+which is more convenient for users to realize the configuration of scheduled tasks.
+
+## Installation
+
+```commandline
+pip install django-aps
+```
+
+## Quick start
+
+- Add ``aps`` to your ``INSTALLED_APPS`` setting like this:
+
+```python
+INSTALLED_APPS = (
+    # ...
+    "django_aps1",
+)
+```
+
+- django-aps comes with sensible configuration defaults out of the box. The defaults can be overridden by adding
+  the following settings to your Django `settings.py` file:
+
+```python
+DEFAULT_DISCOVER_SCHEMA = 'pkg'
+```
+
+- Run `python manage.py migrate` to create the django_apscheduler models.
+
+- Register a APScheduler function in your project
+
+```python
+
+```
+
```

### Comparing `django-aps-0.0.1/migrations/0001_initial.py` & `django-aps-0.0.2/django_aps/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.0.1/migrations/0002_auto_20230713_1145.py` & `django-aps-0.0.2/django_aps/migrations/0002_auto_20230713_1145.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from django.db import migrations, models
 import django.utils.timezone
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
-        ('aps', '0001_initial'),
+        ('django_aps', '0001_initial'),
     ]
 
     operations = [
         migrations.RenameField(
             model_name='apschedulerjobinfo',
             old_name='func_module',
             new_name='func_ref',
```

### Comparing `django-aps-0.0.1/model/aps_models.py` & `django-aps-0.0.2/django_aps/model/aps_models.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.0.1/model/trigger_models.py` & `django-aps-0.0.2/django_aps/model/trigger_models.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.0.1/repository/apscheduler_func_model_mapper.py` & `django-aps-0.0.2/django_aps/repository/apscheduler_func_model_mapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 APScheduler func model mapper
 """
 from typing import Union, List, Dict
 
-from aps.models import ApschedulerFunc
+from django_aps.models import ApschedulerFunc
 
 
 def get_aps_funcs(name: str = None, **kwargs) -> Union[List, None]:
     if name:
         kwargs.setdefault('func_name__contains', name)
     aps_funcs_queryset = ApschedulerFunc.objects.filter(
         **kwargs
```

### Comparing `django-aps-0.0.1/repository/apscheduler_job_model_mapper.py` & `django-aps-0.0.2/django_aps/repository/apscheduler_job_model_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # """
 # apscheduler job model mapper
 # """
 # from django.db import DatabaseError
 #
-# from aps.models import ApschedulerJobInfo
+# from django_aps.models import ApschedulerJobInfo
 #
 #
 # def add_apscheduler_job_info(job_info: dict):
 #     try:
 #         obj = ApschedulerJobInfo.objects.create(
 #             **job_info
 #         )
```

### Comparing `django-aps-0.0.1/serializers/apscheduler_serializers.py` & `django-aps-0.0.2/django_aps/serializers/apscheduler_serializers.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.0.1/service/discover_service.py` & `django-aps-0.0.2/django_aps/service/discover_service.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 Discover service
 """
 import logging
 from typing import List, Dict
 
 from django.db import transaction
 
-from aps.repository import apscheduler_func_model_mapper
-from aps.settings import aps_settings
-from aps.utils.common import check_table_exist
-from aps.utils.discover import autodiscover_aps
+from django_aps.repository import apscheduler_func_model_mapper
+from django_aps.settings import aps_settings
+from django_aps.utils.common import check_table_exist
+from django_aps.utils.discover import autodiscover_aps
 
 logger = logging.getLogger(__name__)
 
 
 class DiscoverService:
 
     def __init__(self, schema: str = None):
@@ -46,15 +46,15 @@
             if name in aps_func.get('func_name'):
                 aps_name_funcs.append(aps_func)
 
         return aps_name_funcs
 
     def sync_aps_to_db(self):
         """
-        Synchronize auto discover aps function to the database
+        Synchronize auto discover django_aps function to the database
 
         """
         if self.schema != 'database':
             logger.warning(f'Skip sync because current schema is {self.schema} not equal database.')
             return
         if not check_table_exist('django_apscheduler_func'):
             logger.warning('Skip sync because table "django_apscheduler_func" does not exist.')
```

### Comparing `django-aps-0.0.1/service/scheduler_service.py` & `django-aps-0.0.2/django_aps/service/scheduler_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import logging
 from typing import Union
 
 from apscheduler.job import Job
 from apscheduler.schedulers.background import BackgroundScheduler
 from django.utils.module_loading import import_string
 
-from aps.model.aps_models import APSchedulerJob
-from aps.model.trigger_models import CronTriggerModel, IntervalTriggerModel, DateTriggerModel
-from aps.settings import aps_settings
+from django_aps.model.aps_models import APSchedulerJob
+from django_aps.model.trigger_models import CronTriggerModel, IntervalTriggerModel, DateTriggerModel
+from django_aps.settings import aps_settings
 
 logger = logging.getLogger(__name__)
 
 
 class APSchedulerService:
 
     def __init__(self):
```

### Comparing `django-aps-0.0.1/setup.py` & `django-aps-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="django-aps",
-    version="0.0.1",
+    version="0.0.2",
     description="APScheduler Register for Django",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cuidingyong/django-aps",
     author="Dillon",
     author_email="cuidingyong@yeah.net",
     license="MIT",
@@ -29,16 +29,16 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Framework :: Django",
         "Framework :: Django :: 3.2",
         "Framework :: Django :: 4.0",
     ],
-    keywords="django apscheduler django-aps register",
-    packages=find_packages(exclude=("tests",)),
+    keywords="django apscheduler django-django_aps register",
+    packages=find_packages(exclude=("tests", "django_aps1", "test")),
     install_requires=[
         "django>=3.2",
         "apscheduler>=3.2,<4.0",
         "djangorestframework>=3.14",
         "django-apscheduler>=0.6.2",
         "pydantic>=2.0"
     ],
```

### Comparing `django-aps-0.0.1/utils/discover.py` & `django-aps-0.0.2/django_aps/utils/discover.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import logging
 import os.path
 import pkgutil
 from typing import List
 
 from django.apps import apps
 
-from aps.settings import aps_settings
-from aps.utils.register import Register
+from django_aps.settings import aps_settings
+from django_aps.utils.register import Register
 
 logger = logging.getLogger(__name__)
 
 
 def autodiscover_aps(custom_pkgs: List[str] = None) -> List:
     aps_funcs = []
     discover_pkgs = aps_settings.DEFAULT_DISCOVER_PKG
```

### Comparing `django-aps-0.0.1/utils/register.py` & `django-aps-0.0.2/django_aps/utils/register.py`

 * *Files identical despite different names*

### Comparing `django-aps-0.0.1/views/apscheduler_view.py` & `django-aps-0.0.2/django_aps/views/apscheduler_view.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 Apscheduler functions view
 """
 from django.http import JsonResponse
 
-from aps.base import BaseGenericAPIView
-from aps.serializers.apscheduler_serializers import RegisteredFuncQuerySerializers, SchedulerJobAddSerializers, \
+from django_aps.base import BaseGenericAPIView
+from django_aps.serializers.apscheduler_serializers import RegisteredFuncQuerySerializers, SchedulerJobAddSerializers, \
     SchedulerJobQuerySerializers, SchedulerJobUpdateSerializers, SchedulerJobPauseSerializers
-from aps.service.discover_service import DiscoverService
-from aps.service.scheduler_service import APSchedulerService
+from django_aps.service.discover_service import DiscoverService
+from django_aps.service.scheduler_service import APSchedulerService
 
 
 class RegisteredFuncQueryView(BaseGenericAPIView):
     serializer_class = RegisteredFuncQuerySerializers
 
     def get(self, request):
         serializer = self.serializer_class(data=request.query_params)
```

