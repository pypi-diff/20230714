# Comparing `tmp/django-loose-fk-1.0.2.tar.gz` & `tmp/django-loose-fk-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-loose-fk-1.0.2.tar", last modified: Fri Mar 18 11:18:42 2022, max compression
+gzip compressed data, was "django-loose-fk-1.0.3.tar", last modified: Fri Jul 14 14:33:31 2023, max compression
```

## Comparing `django-loose-fk-1.0.2.tar` & `django-loose-fk-1.0.3.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 11:18:42.062562 django-loose-fk-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1052 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5449 2022-03-18 11:18:42.062562 django-loose-fk-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4333 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 11:18:42.058562 django-loose-fk-1.0.2/django_loose_fk/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/django_loose_fk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1107 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/django_loose_fk/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      646 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/django_loose_fk/checks.py
--rw-r--r--   0 runner    (1001) docker     (121)     2771 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/django_loose_fk/constraints.py
--rw-r--r--   0 runner    (1001) docker     (121)     7099 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/django_loose_fk/drf.py
--rw-r--r--   0 runner    (1001) docker     (121)     7767 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/django_loose_fk/fields.py
--rw-r--r--   0 runner    (1001) docker     (121)     3234 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/django_loose_fk/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 11:18:42.058562 django-loose-fk-1.0.2/django_loose_fk/inspectors/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/django_loose_fk/inspectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1141 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/django_loose_fk/inspectors/fields.py
--rw-r--r--   0 runner    (1001) docker     (121)     1274 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/django_loose_fk/inspectors/query.py
--rw-r--r--   0 runner    (1001) docker     (121)     3366 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/django_loose_fk/loaders.py
--rw-r--r--   0 runner    (1001) docker     (121)     5151 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/django_loose_fk/lookups.py
--rw-r--r--   0 runner    (1001) docker     (121)     1292 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/django_loose_fk/query_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     1773 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/django_loose_fk/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3925 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/django_loose_fk/virtual_models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 11:18:42.058562 django-loose-fk-1.0.2/django_loose_fk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5449 2022-03-18 11:18:41.000000 django-loose-fk-1.0.2/django_loose_fk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1318 2022-03-18 11:18:42.000000 django-loose-fk-1.0.2/django_loose_fk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-18 11:18:41.000000 django-loose-fk-1.0.2/django_loose_fk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-18 11:18:41.000000 django-loose-fk-1.0.2/django_loose_fk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-03-18 11:18:41.000000 django-loose-fk-1.0.2/django_loose_fk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-03-18 11:18:41.000000 django-loose-fk-1.0.2/django_loose_fk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1825 2022-03-18 11:18:42.062562 django-loose-fk-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 11:18:42.062562 django-loose-fk-1.0.2/testapp/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/testapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1900 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/testapp/api.py
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/testapp/loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 11:18:42.062562 django-loose-fk-1.0.2/testapp/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     9689 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/testapp/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)     3993 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/testapp/migrations/0002_auto_20220310_1612.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/testapp/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2603 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/testapp/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1400 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/testapp/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/testapp/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 11:18:42.062562 django-loose-fk-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     6632 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1643 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/tests/test_api_docs.py
--rw-r--r--   0 runner    (1001) docker     (121)      881 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/tests/test_chain_loose_fk.py
--rw-r--r--   0 runner    (1001) docker     (121)      839 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/tests/test_compare.py
--rw-r--r--   0 runner    (1001) docker     (121)     3655 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/tests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)      742 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/tests/test_integrity.py
--rw-r--r--   0 runner    (1001) docker     (121)      961 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/tests/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (121)     3245 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/tests/test_model_field_interface.py
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/tests/test_model_layer.py
--rw-r--r--   0 runner    (1001) docker     (121)     4311 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/tests/test_querying.py
--rw-r--r--   0 runner    (1001) docker     (121)      974 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/tests/test_querylist.py
--rw-r--r--   0 runner    (1001) docker     (121)      632 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/tests/test_serializer_field.py
--rw-r--r--   0 runner    (1001) docker     (121)      701 2022-03-18 11:18:36.000000 django-loose-fk-1.0.2/tests/test_system_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:33:31.294602 django-loose-fk-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-07-14 14:33:31.294602 django-loose-fk-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:33:31.286602 django-loose-fk-1.0.3/django_loose_fk/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/django_loose_fk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/django_loose_fk/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/django_loose_fk/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/django_loose_fk/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/django_loose_fk/drf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/django_loose_fk/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/django_loose_fk/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:33:31.290602 django-loose-fk-1.0.3/django_loose_fk/inspectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/django_loose_fk/inspectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/django_loose_fk/inspectors/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/django_loose_fk/inspectors/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/django_loose_fk/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/django_loose_fk/lookups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/django_loose_fk/query_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/django_loose_fk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/django_loose_fk/virtual_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:33:31.290602 django-loose-fk-1.0.3/django_loose_fk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-07-14 14:33:31.000000 django-loose-fk-1.0.3/django_loose_fk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-14 14:33:31.000000 django-loose-fk-1.0.3/django_loose_fk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 14:33:31.000000 django-loose-fk-1.0.3/django_loose_fk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 14:33:31.000000 django-loose-fk-1.0.3/django_loose_fk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-14 14:33:31.000000 django-loose-fk-1.0.3/django_loose_fk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-14 14:33:31.000000 django-loose-fk-1.0.3/django_loose_fk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-14 14:33:31.294602 django-loose-fk-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:33:31.290602 django-loose-fk-1.0.3/testapp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/testapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/testapp/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/testapp/loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:33:31.290602 django-loose-fk-1.0.3/testapp/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     9688 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/testapp/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/testapp/migrations/0002_auto_20220310_1612.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/testapp/migrations/0003_auto_20230705_0917.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/testapp/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/testapp/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/testapp/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/testapp/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:33:31.294602 django-loose-fk-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/tests/test_api_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/tests/test_chain_loose_fk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/tests/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/tests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/tests/test_integrity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/tests/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/tests/test_model_field_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/tests/test_model_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/tests/test_querying.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/tests/test_querylist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/tests/test_serializer_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-14 14:33:26.000000 django-loose-fk-1.0.3/tests/test_system_checks.py
```

### Comparing `django-loose-fk-1.0.2/CHANGELOG.rst` & `django-loose-fk-1.0.3/CHANGELOG.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 =========
 Changelog
 =========
 
+1.0.3 (2023-07-14)
+==================
+
+* Fixed a bug which can appear when there is a chain of loose-fk objects, especially
+when external object is related to the local one. In this case the local object was treated
+like an external one, now it's fixed.
+* Dropped support for Django 2.2
+
 1.0.2 (2022-03-18)
 ==================
 
 Bugfix release
 
 * Fixed a bug in the django-filter implementation causing crashes on
   ``.filter(*args, **kwargs)`` calls because of tuples instead of ``models.Q`` objects
```

### Comparing `django-loose-fk-1.0.2/LICENSE` & `django-loose-fk-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.2/PKG-INFO` & `django-loose-fk-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: django-loose-fk
-Version: 1.0.2
+Version: 1.0.3
 Summary: Django Loose FK handles local or remote "ForeignKey" references.
 Home-page: https://github.com/maykinmedia/django-loose-fk
 Author: Maykin Media
 Author-email: support@maykinmedia.nl
 License: MIT
 Keywords: ForeignKey,URL reference,decentralization,integrity
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -29,15 +27,15 @@
 Provides-Extra: release
 License-File: LICENSE
 
 ===============
 Django Loose FK
 ===============
 
-:Version: 1.0.2
+:Version: 1.0.3
 :Source: https://github.com/maykinmedia/django-loose-fk
 :Keywords: ``ForeignKey``, ``URL reference``, ``decentralization``, ``integrity``
 
 |build-status| |code-quality| |black| |coverage|
 
 |python-versions| |django-versions| |pypi-version|
 
@@ -63,15 +61,15 @@
 ============
 
 Requirements
 ------------
 
 * Python 3.7 or above
 * setuptools 30.3.0 or above
-* Django 2.2 or newer
+* Django 3.2 or newer
 
 
 Install
 -------
 
 .. code-block:: bash
 
@@ -174,9 +172,7 @@
 
 .. |python-versions| image:: https://img.shields.io/pypi/pyversions/django-loose-fk.svg
 
 .. |django-versions| image:: https://img.shields.io/pypi/djversions/django-loose-fk.svg
 
 .. |pypi-version| image:: https://img.shields.io/pypi/v/django-loose-fk.svg
     :target: https://pypi.org/project/django-loose-fk/
-
-
```

### Comparing `django-loose-fk-1.0.2/README.rst` & `django-loose-fk-1.0.3/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ===============
 Django Loose FK
 ===============
 
-:Version: 1.0.2
+:Version: 1.0.3
 :Source: https://github.com/maykinmedia/django-loose-fk
 :Keywords: ``ForeignKey``, ``URL reference``, ``decentralization``, ``integrity``
 
 |build-status| |code-quality| |black| |coverage|
 
 |python-versions| |django-versions| |pypi-version|
 
@@ -32,15 +32,15 @@
 ============
 
 Requirements
 ------------
 
 * Python 3.7 or above
 * setuptools 30.3.0 or above
-* Django 2.2 or newer
+* Django 3.2 or newer
 
 
 Install
 -------
 
 .. code-block:: bash
```

### Comparing `django-loose-fk-1.0.2/django_loose_fk/apps.py` & `django-loose-fk-1.0.3/django_loose_fk/apps.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.2/django_loose_fk/checks.py` & `django-loose-fk-1.0.3/django_loose_fk/checks.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.2/django_loose_fk/constraints.py` & `django-loose-fk-1.0.3/django_loose_fk/constraints.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
         return (path, args, kwargs)
 
     def _get_check_constraint(self, model, schema_editor):
         """
         Return the underlying check constraint generated.
         """
         if not hasattr(self, "_check_constraint"):
-
             # URL field is empty if empty string or None
             empty_url_field = models.Q(**{self.url_field: ""})
             empty_fk_field = models.Q(**{f"{self.fk_field}__isnull": True})
 
             fk_filled = ~empty_fk_field & empty_url_field
             url_filled = empty_fk_field & ~empty_url_field
```

### Comparing `django-loose-fk-1.0.2/django_loose_fk/drf.py` & `django-loose-fk-1.0.3/django_loose_fk/drf.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.2/django_loose_fk/fields.py` & `django-loose-fk-1.0.3/django_loose_fk/fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -197,14 +197,20 @@
     def __get__(self, instance, cls=None):
         """
         Get the related instance through the forward relation.
         """
         if instance is None:
             return self
 
+        # for chained loose-fk fields:
+        if isinstance(instance, ProxyMixin):
+            fk_value = instance._loose_fk_data.get(self.fk_field_name, None)
+            if fk_value:
+                return fk_value
+
         # if the value is select_related, this will hit that cache
         pk_value = getattr(instance, self.field._fk_field.attname)
         if pk_value is not None:
             fk_value = getattr(instance, self.fk_field_name)
             if fk_value is not None:
                 return fk_value
 
@@ -226,14 +232,21 @@
         """
         if value is None and not self.field.null:
             raise ValueError(
                 "A 'None'-value is not allowed. Make the field "
                 "nullable if empty values should be supported."
             )
 
+        # for chained loose-fk models check if it's a local url
+        if isinstance(instance, ProxyMixin) and isinstance(value, str):
+            if self.field.loader.is_local_url(value):
+                remote_model = self.field._fk_field.related_model
+                value = self.field.loader.load_local_object(value, remote_model)
+
+        # if we try to set loose-fk virtual model instance - it's external url
         if isinstance(value, ProxyMixin):
             value = value._loose_fk_data["url"]
 
         if isinstance(value, models.Model):
             field_name = self.fk_field_name
         elif isinstance(value, str):
             field_name = self.url_field_name
```

### Comparing `django-loose-fk-1.0.2/django_loose_fk/filters.py` & `django-loose-fk-1.0.3/django_loose_fk/filters.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.2/django_loose_fk/inspectors/fields.py` & `django-loose-fk-1.0.3/django_loose_fk/inspectors/fields.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.2/django_loose_fk/inspectors/query.py` & `django-loose-fk-1.0.3/django_loose_fk/inspectors/query.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.2/django_loose_fk/loaders.py` & `django-loose-fk-1.0.3/django_loose_fk/loaders.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.2/django_loose_fk/lookups.py` & `django-loose-fk-1.0.3/django_loose_fk/lookups.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.2/django_loose_fk/query_list.py` & `django-loose-fk-1.0.3/django_loose_fk/query_list.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.2/django_loose_fk/utils.py` & `django-loose-fk-1.0.3/django_loose_fk/utils.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.2/django_loose_fk/virtual_models.py` & `django-loose-fk-1.0.3/django_loose_fk/virtual_models.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.2/django_loose_fk.egg-info/PKG-INFO` & `django-loose-fk-1.0.3/django_loose_fk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: django-loose-fk
-Version: 1.0.2
+Version: 1.0.3
 Summary: Django Loose FK handles local or remote "ForeignKey" references.
 Home-page: https://github.com/maykinmedia/django-loose-fk
 Author: Maykin Media
 Author-email: support@maykinmedia.nl
 License: MIT
 Keywords: ForeignKey,URL reference,decentralization,integrity
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -29,15 +27,15 @@
 Provides-Extra: release
 License-File: LICENSE
 
 ===============
 Django Loose FK
 ===============
 
-:Version: 1.0.2
+:Version: 1.0.3
 :Source: https://github.com/maykinmedia/django-loose-fk
 :Keywords: ``ForeignKey``, ``URL reference``, ``decentralization``, ``integrity``
 
 |build-status| |code-quality| |black| |coverage|
 
 |python-versions| |django-versions| |pypi-version|
 
@@ -63,15 +61,15 @@
 ============
 
 Requirements
 ------------
 
 * Python 3.7 or above
 * setuptools 30.3.0 or above
-* Django 2.2 or newer
+* Django 3.2 or newer
 
 
 Install
 -------
 
 .. code-block:: bash
 
@@ -174,9 +172,7 @@
 
 .. |python-versions| image:: https://img.shields.io/pypi/pyversions/django-loose-fk.svg
 
 .. |django-versions| image:: https://img.shields.io/pypi/djversions/django-loose-fk.svg
 
 .. |pypi-version| image:: https://img.shields.io/pypi/v/django-loose-fk.svg
     :target: https://pypi.org/project/django-loose-fk/
-
-
```

### Comparing `django-loose-fk-1.0.2/django_loose_fk.egg-info/SOURCES.txt` & `django-loose-fk-1.0.3/django_loose_fk.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 testapp/api.py
 testapp/loaders.py
 testapp/models.py
 testapp/settings.py
 testapp/urls.py
 testapp/migrations/0001_initial.py
 testapp/migrations/0002_auto_20220310_1612.py
+testapp/migrations/0003_auto_20230705_0917.py
 testapp/migrations/__init__.py
 tests/__init__.py
 tests/conftest.py
 tests/test_api.py
 tests/test_api_docs.py
 tests/test_chain_loose_fk.py
 tests/test_compare.py
```

### Comparing `django-loose-fk-1.0.2/setup.cfg` & `django-loose-fk-1.0.3/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [metadata]
 name = django-loose-fk
-version = 1.0.2
+version = 1.0.3
 description = Django Loose FK handles local or remote "ForeignKey" references.
 long_description = file: README.rst
 url = https://github.com/maykinmedia/django-loose-fk
 license = MIT
 author = Maykin Media
 author_email = support@maykinmedia.nl
 keywords = ForeignKey, URL reference, decentralization, integrity
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Framework :: Django
-	Framework :: Django :: 2.2
 	Framework :: Django :: 3.2
 	Intended Audience :: Developers
 	Operating System :: Unix
 	Operating System :: MacOS
 	Operating System :: Microsoft :: Windows
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
@@ -24,17 +23,18 @@
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = 
-	django>=2.2
+	django>=3.2
 	djangorestframework>=3.11.0
 	django-filter
+	coreapi
 tests_require = 
 	psycopg2
 	pytest
 	pytest-django
 	tox
 	black
 	isort
```

### Comparing `django-loose-fk-1.0.2/testapp/api.py` & `django-loose-fk-1.0.3/testapp/api.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.2/testapp/migrations/0001_initial.py` & `django-loose-fk-1.0.3/testapp/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from django.db import migrations, models
 
 import django_loose_fk.constraints
 import django_loose_fk.fields
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = []
 
     operations = [
         migrations.CreateModel(
             name="B",
```

### Comparing `django-loose-fk-1.0.2/testapp/migrations/0002_auto_20220310_1612.py` & `django-loose-fk-1.0.3/testapp/migrations/0002_auto_20220310_1612.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from django.db import migrations, models
 
 import django_loose_fk.constraints
 import django_loose_fk.fields
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("testapp", "0001_initial"),
     ]
 
     operations = [
         migrations.CreateModel(
             name="ZaakObject2",
```

### Comparing `django-loose-fk-1.0.2/testapp/models.py` & `django-loose-fk-1.0.3/testapp/models.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.2/testapp/settings.py` & `django-loose-fk-1.0.3/testapp/settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,16 +20,15 @@
     DB = os.getenv("DB", "sqlite")
     MAP = {"sqlite": SQLITE_DB, "postgres": PG_DB}
     return MAP[DB]
 
 
 DATABASES = {"default": get_db()}
 
-# TODO: update to BigAutoField and makemigrations once we drop 2.2 support
-DEFAULT_AUTO_FIELD = "django.db.models.AutoField"
+DEFAULT_AUTO_FIELD = "django.db.models.BigAutoField"
 
 INSTALLED_APPS = ["django_loose_fk", "testapp"]
 
 MIDDLEWARE = [
     "django.middleware.security.SecurityMiddleware",
     "django.middleware.common.CommonMiddleware",
     "django.middleware.csrf.CsrfViewMiddleware",
```

### Comparing `django-loose-fk-1.0.2/tests/test_api.py` & `django-loose-fk-1.0.3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.2/tests/test_api_docs.py` & `django-loose-fk-1.0.3/tests/test_api_docs.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.2/tests/test_chain_loose_fk.py` & `django-loose-fk-1.0.3/tests/test_chain_loose_fk.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.2/tests/test_compare.py` & `django-loose-fk-1.0.3/tests/test_compare.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.2/tests/test_filter.py` & `django-loose-fk-1.0.3/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.2/tests/test_integrity.py` & `django-loose-fk-1.0.3/tests/test_integrity.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.2/tests/test_loaders.py` & `django-loose-fk-1.0.3/tests/test_loaders.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.2/tests/test_model_field_interface.py` & `django-loose-fk-1.0.3/tests/test_model_field_interface.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.2/tests/test_querying.py` & `django-loose-fk-1.0.3/tests/test_querying.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.2/tests/test_querylist.py` & `django-loose-fk-1.0.3/tests/test_querylist.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.2/tests/test_serializer_field.py` & `django-loose-fk-1.0.3/tests/test_serializer_field.py`

 * *Files identical despite different names*

### Comparing `django-loose-fk-1.0.2/tests/test_system_checks.py` & `django-loose-fk-1.0.3/tests/test_system_checks.py`

 * *Files identical despite different names*

