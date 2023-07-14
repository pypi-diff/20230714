# Comparing `tmp/django-admin-index-3.0.0.tar.gz` & `tmp/django-admin-index-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-admin-index-3.0.0.tar", last modified: Wed May  3 08:59:40 2023, max compression
+gzip compressed data, was "django-admin-index-3.1.0.tar", last modified: Fri Jul 14 11:07:29 2023, max compression
```

## Comparing `django-admin-index-3.0.0.tar` & `django-admin-index-3.1.0.tar`

### file list

```diff
@@ -1,63 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:59:40.967847 django-admin-index-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/CONTRIBUTORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10319 2023-05-03 08:59:40.967847 django-admin-index-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8728 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:59:40.959847 django-admin-index-3.0.0/django_admin_index/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/django_admin_index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/django_admin_index/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/django_admin_index/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/django_admin_index/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:59:40.963847 django-admin-index-3.0.0/django_admin_index/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/django_admin_index/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/django_admin_index/migrations/0002_auto_20170802_1754.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/django_admin_index/migrations/0003_auto_20200724_1516.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/django_admin_index/migrations/0004_auto_20230503_0723.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/django_admin_index/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/django_admin_index/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:59:40.955847 django-admin-index-3.0.0/django_admin_index/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:59:40.955847 django-admin-index-3.0.0/django_admin_index/static/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:59:40.963847 django-admin-index-3.0.0/django_admin_index/static/admin/css/
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/django_admin_index/static/admin/css/admin-index.css
--rw-r--r--   0 runner    (1001) docker     (123)    11217 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/django_admin_index/static/admin/css/admin-index.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:59:40.955847 django-admin-index-3.0.0/django_admin_index/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:59:40.963847 django-admin-index-3.0.0/django_admin_index/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/django_admin_index/templates/admin/change_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/django_admin_index/templates/admin/change_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/django_admin_index/templates/admin/delete_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/django_admin_index/templates/admin/delete_selected_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/django_admin_index/templates/admin/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/django_admin_index/templates/admin/object_history.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:59:40.955847 django-admin-index-3.0.0/django_admin_index/templates/django_admin_index/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:59:40.963847 django-admin-index-3.0.0/django_admin_index/templates/django_admin_index/includes/
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/django_admin_index/templates/django_admin_index/includes/app_list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:59:40.967847 django-admin-index-3.0.0/django_admin_index/templates/registration/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/django_admin_index/templates/registration/password_change_done.html
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/django_admin_index/templates/registration/password_change_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/django_admin_index/templates/registration/password_reset_complete.html
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/django_admin_index/templates/registration/password_reset_confirm.html
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/django_admin_index/templates/registration/password_reset_done.html
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/django_admin_index/templates/registration/password_reset_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:59:40.967847 django-admin-index-3.0.0/django_admin_index/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/django_admin_index/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/django_admin_index/templatetags/django_admin_index.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/django_admin_index/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:59:40.963847 django-admin-index-3.0.0/django_admin_index.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10319 2023-05-03 08:59:40.000000 django-admin-index-3.0.0/django_admin_index.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-03 08:59:40.000000 django-admin-index-3.0.0/django_admin_index.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 08:59:40.000000 django-admin-index-3.0.0/django_admin_index.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 08:59:40.000000 django-admin-index-3.0.0/django_admin_index.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-03 08:59:40.000000 django-admin-index-3.0.0/django_admin_index.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-03 08:59:40.000000 django-admin-index-3.0.0/django_admin_index.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:59:40.967847 django-admin-index-3.0.0/scss/
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/scss/_vars.scss
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/scss/admin-index.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:59:40.967847 django-admin-index-3.0.0/scss/components/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/scss/components/_containers.scss
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/scss/components/_dropdown-menu.scss
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/scss/components/_header.scss
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-03 08:59:40.967847 django-admin-index-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 08:59:33.000000 django-admin-index-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:07:29.795879 django-admin-index-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/CONTRIBUTORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10305 2023-07-14 11:07:29.795879 django-admin-index-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8714 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:07:29.791880 django-admin-index-3.1.0/django_admin_index/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/django_admin_index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/django_admin_index/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/django_admin_index/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/django_admin_index/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:07:29.791880 django-admin-index-3.1.0/django_admin_index/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/django_admin_index/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/django_admin_index/migrations/0002_auto_20170802_1754.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/django_admin_index/migrations/0003_auto_20200724_1516.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/django_admin_index/migrations/0004_auto_20230503_0723.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/django_admin_index/migrations/0005_auto_20230503_1910.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/django_admin_index/migrations/0006_auto_20230503_1910.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/django_admin_index/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/django_admin_index/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:07:29.787880 django-admin-index-3.1.0/django_admin_index/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:07:29.787880 django-admin-index-3.1.0/django_admin_index/static/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:07:29.791880 django-admin-index-3.1.0/django_admin_index/static/admin/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/django_admin_index/static/admin/css/admin-index.css
+-rw-r--r--   0 runner    (1001) docker     (123)    11217 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/django_admin_index/static/admin/css/admin-index.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:07:29.787880 django-admin-index-3.1.0/django_admin_index/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:07:29.795879 django-admin-index-3.1.0/django_admin_index/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/django_admin_index/templates/admin/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/django_admin_index/templates/admin/change_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/django_admin_index/templates/admin/delete_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/django_admin_index/templates/admin/delete_selected_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/django_admin_index/templates/admin/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/django_admin_index/templates/admin/object_history.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:07:29.787880 django-admin-index-3.1.0/django_admin_index/templates/django_admin_index/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:07:29.795879 django-admin-index-3.1.0/django_admin_index/templates/django_admin_index/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/django_admin_index/templates/django_admin_index/includes/app_list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:07:29.795879 django-admin-index-3.1.0/django_admin_index/templates/registration/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/django_admin_index/templates/registration/password_change_done.html
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/django_admin_index/templates/registration/password_change_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/django_admin_index/templates/registration/password_reset_complete.html
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/django_admin_index/templates/registration/password_reset_confirm.html
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/django_admin_index/templates/registration/password_reset_done.html
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/django_admin_index/templates/registration/password_reset_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:07:29.795879 django-admin-index-3.1.0/django_admin_index/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/django_admin_index/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/django_admin_index/templatetags/django_admin_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/django_admin_index/translations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/django_admin_index/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:07:29.791880 django-admin-index-3.1.0/django_admin_index.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10305 2023-07-14 11:07:29.000000 django-admin-index-3.1.0/django_admin_index.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-07-14 11:07:29.000000 django-admin-index-3.1.0/django_admin_index.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 11:07:29.000000 django-admin-index-3.1.0/django_admin_index.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 11:07:29.000000 django-admin-index-3.1.0/django_admin_index.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-14 11:07:29.000000 django-admin-index-3.1.0/django_admin_index.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 11:07:29.000000 django-admin-index-3.1.0/django_admin_index.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:07:29.795879 django-admin-index-3.1.0/scss/
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/scss/_vars.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/scss/admin-index.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:07:29.795879 django-admin-index-3.1.0/scss/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/scss/components/_containers.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/scss/components/_dropdown-menu.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/scss/components/_header.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-07-14 11:07:29.795879 django-admin-index-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 11:07:22.000000 django-admin-index-3.1.0/setup.py
```

### Comparing `django-admin-index-3.0.0/CHANGELOG.rst` & `django-admin-index-3.1.0/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 ==============
 Change history
 ==============
 
+3.1.0 (2023-07-14)
+==================
+
+🌐 Added content translations support
+
+You can now provide translations for the app group and link names, which are activated
+based on the currently active language. You (optionally) provide translations through a
+JSON datastructure, keyed by language code.
+
+* Fixed supported django version badge.
+* Added support for content translations.
+
 3.0.0 (2023-05-03)
 ==================
 
 Periodic version compatibility release.
 
 The major version is bumped due to dropping support for Django 2.2 - the library itself
 does not have any breaking changes and upgrading from 2.0.x should be smooth.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-admin-index-3.0.0/LICENSE` & `django-admin-index-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-admin-index-3.0.0/PKG-INFO` & `django-admin-index-3.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-index
-Version: 3.0.0
+Version: 3.1.0
 Summary: Admin index for Django
 Home-page: https://github.com/maykinmedia/django-admin-index
 Author: Joeri Bekker
 Author-email: joeri@maykinmedia.nl
 License: BSD
 Project-URL: Changelog, https://github.com/maykinmedia/django-admin-index/blob/master/CHANGELOG.rst
 Project-URL: Bug Tracker, https://github.com/maykinmedia/django-admin-index/issues
@@ -35,15 +35,15 @@
 Provides-Extra: release
 License-File: LICENSE
 
 ======================
 Admin Index for Django
 ======================
 
-:Version: 3.0.0
+:Version: 3.1.0
 :Download: https://pypi.python.org/pypi/django-admin-index
 :Source: https://github.com/maykinmedia/django-admin-index
 :Keywords: django, admin, dashboard
 
 |build-status| |code-quality| |black| |coverage| |license| |python-versions| |django-versions| |pypi-version|
 
 About
@@ -275,15 +275,15 @@
     :alt: BSD License
     :target: https://opensource.org/licenses/BSD-3-Clause
 
 .. |python-versions| image:: https://img.shields.io/pypi/pyversions/django-admin-index.svg
     :alt: Supported Python versions
     :target: http://pypi.python.org/pypi/django-admin-index/
 
-.. |django-versions| image:: https://img.shields.io/badge/django-2.2%2C%203.0%2C%203.2%2C%204.0-blue.svg
+.. |django-versions| image:: https://img.shields.io/pypi/djversions/django-admin-index.svg
     :alt: Supported Django versions
     :target: http://pypi.python.org/pypi/django-admin-index/
 
 .. |pypi-version| image:: https://img.shields.io/pypi/v/django-admin-index.svg
     :target: https://pypi.org/project/django-admin-index/
 
 .. |screenshot-1| image:: https://github.com/maykinmedia/django-admin-index/raw/master/docs/_assets/dashboard_with_menu_thumb.png
```

### Comparing `django-admin-index-3.0.0/README.rst` & `django-admin-index-3.1.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ======================
 Admin Index for Django
 ======================
 
-:Version: 3.0.0
+:Version: 3.1.0
 :Download: https://pypi.python.org/pypi/django-admin-index
 :Source: https://github.com/maykinmedia/django-admin-index
 :Keywords: django, admin, dashboard
 
 |build-status| |code-quality| |black| |coverage| |license| |python-versions| |django-versions| |pypi-version|
 
 About
@@ -238,15 +238,15 @@
     :alt: BSD License
     :target: https://opensource.org/licenses/BSD-3-Clause
 
 .. |python-versions| image:: https://img.shields.io/pypi/pyversions/django-admin-index.svg
     :alt: Supported Python versions
     :target: http://pypi.python.org/pypi/django-admin-index/
 
-.. |django-versions| image:: https://img.shields.io/badge/django-2.2%2C%203.0%2C%203.2%2C%204.0-blue.svg
+.. |django-versions| image:: https://img.shields.io/pypi/djversions/django-admin-index.svg
     :alt: Supported Django versions
     :target: http://pypi.python.org/pypi/django-admin-index/
 
 .. |pypi-version| image:: https://img.shields.io/pypi/v/django-admin-index.svg
     :target: https://pypi.org/project/django-admin-index/
 
 .. |screenshot-1| image:: https://github.com/maykinmedia/django-admin-index/raw/master/docs/_assets/dashboard_with_menu_thumb.png
```

### Comparing `django-admin-index-3.0.0/django_admin_index/apps.py` & `django-admin-index-3.1.0/django_admin_index/apps.py`

 * *Files identical despite different names*

### Comparing `django-admin-index-3.0.0/django_admin_index/conf.py` & `django-admin-index-3.1.0/django_admin_index/conf.py`

 * *Files identical despite different names*

### Comparing `django-admin-index-3.0.0/django_admin_index/migrations/0001_initial.py` & `django-admin-index-3.1.0/django_admin_index/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-admin-index-3.0.0/django_admin_index/migrations/0003_auto_20200724_1516.py` & `django-admin-index-3.1.0/django_admin_index/migrations/0003_auto_20200724_1516.py`

 * *Files identical despite different names*

### Comparing `django-admin-index-3.0.0/django_admin_index/migrations/0004_auto_20230503_0723.py` & `django-admin-index-3.1.0/django_admin_index/migrations/0004_auto_20230503_0723.py`

 * *Files identical despite different names*

### Comparing `django-admin-index-3.0.0/django_admin_index/models.py` & `django-admin-index-3.1.0/django_admin_index/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from django.contrib.admin import site
 from django.contrib.contenttypes.models import ContentType
 from django.db import models
+from django.db.models import F
 from django.urls import reverse
 from django.utils.text import capfirst
-from django.utils.translation import gettext_lazy as _
+from django.utils.translation import get_language, gettext_lazy as _
 
 from ordered_model.models import OrderedModel, OrderedModelManager, OrderedModelQuerySet
 
 from .conf import settings
+from .translations import TranslationsMixin
 
 
 class AppGroupQuerySet(OrderedModelQuerySet):
     def get_by_natural_key(self, slug):
         return self.get(slug=slug)
 
     def as_list(self, request, include_remaining=True):
@@ -45,45 +47,51 @@
                         "active": active,
                     }
                 )
                 model_dicts[key] = model_dict
 
         added = []
 
+        language_code = get_language()
+
         # Create new list based on our groups, using the model_dicts constructed above.  # noqa
         result = []
-        app_list = self.prefetch_related("models", "applink_set")
+        app_list = self.annotate(
+            localized_name=F(f"translations__{language_code}")
+        ).prefetch_related("models", "applink_set")
         active_app = request.path == reverse("admin:index")
         for app in app_list:
             models = []
             active = False
             for model in app.models.all():
                 key = "{}.{}".format(model.app_label, model.model)
                 o = model_dicts.get(key)
                 if o:
                     models.append(o)
                     added.append(key)
                     if o["active"]:
                         active = True
 
-            for app_link in app.applink_set.all():
+            for app_link in app.applink_set.annotate(
+                localized_name=F(f"translations__{language_code}")
+            ):
                 models.append(
                     {
-                        "name": app_link.name,
+                        "name": app_link.localized_name or app_link.name,
                         "app_label": app.slug,
                         "admin_url": app_link.link,
                         "active": request.path.startswith(app_link.link),
                     }
                 )
                 active = request.path.startswith(app_link.link)
 
             if models:
                 result.append(
                     {
-                        "name": app.name,
+                        "name": app.localized_name or app.name,
                         "app_label": app.slug,
                         "models": sorted(models, key=lambda m: m["name"]),
                         "active": active,
                     }
                 )
                 if active:
                     active_app = True
@@ -138,15 +146,15 @@
         proxy = True
         ordering = ("app_label", "model")
 
     def __str__(self):
         return "{}.{}".format(self.app_label, capfirst(self.model))
 
 
-class AppGroup(OrderedModel):
+class AppGroup(TranslationsMixin, OrderedModel):
     name = models.CharField(_("name"), max_length=200)
     slug = models.SlugField(_("slug"), unique=True)
     models = models.ManyToManyField(ContentTypeProxy, blank=True)
 
     objects = AppGroupManager.from_queryset(AppGroupQuerySet)()
 
     class Meta(OrderedModel.Meta):
@@ -156,15 +164,15 @@
     def natural_key(self):
         return (self.slug,)
 
     def __str__(self):
         return self.name
 
 
-class AppLink(OrderedModel):
+class AppLink(TranslationsMixin, OrderedModel):
     app_group = models.ForeignKey(AppGroup, on_delete=models.CASCADE)
     name = models.CharField(max_length=200)
     link = models.CharField(max_length=200)
 
     objects = AppLinkManager.from_queryset(AppLinkQuerySet)()
 
     class Meta(OrderedModel.Meta):
```

### Comparing `django-admin-index-3.0.0/django_admin_index/static/admin/css/admin-index.css` & `django-admin-index-3.1.0/django_admin_index/static/admin/css/admin-index.css`

 * *Files identical despite different names*

### Comparing `django-admin-index-3.0.0/django_admin_index/static/admin/css/admin-index.css.map` & `django-admin-index-3.1.0/django_admin_index/static/admin/css/admin-index.css.map`

 * *Files identical despite different names*

### Comparing `django-admin-index-3.0.0/django_admin_index/templates/admin/change_form.html` & `django-admin-index-3.1.0/django_admin_index/templates/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `django-admin-index-3.0.0/django_admin_index/templates/admin/change_list.html` & `django-admin-index-3.1.0/django_admin_index/templates/admin/change_list.html`

 * *Files identical despite different names*

### Comparing `django-admin-index-3.0.0/django_admin_index/templates/admin/delete_confirmation.html` & `django-admin-index-3.1.0/django_admin_index/templates/admin/delete_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-admin-index-3.0.0/django_admin_index/templates/admin/delete_selected_confirmation.html` & `django-admin-index-3.1.0/django_admin_index/templates/admin/delete_selected_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-admin-index-3.0.0/django_admin_index/templates/admin/index.html` & `django-admin-index-3.1.0/django_admin_index/templates/admin/index.html`

 * *Files identical despite different names*

### Comparing `django-admin-index-3.0.0/django_admin_index/templates/admin/object_history.html` & `django-admin-index-3.1.0/django_admin_index/templates/admin/object_history.html`

 * *Files identical despite different names*

### Comparing `django-admin-index-3.0.0/django_admin_index/templates/django_admin_index/includes/app_list.html` & `django-admin-index-3.1.0/django_admin_index/templates/django_admin_index/includes/app_list.html`

 * *Files identical despite different names*

### Comparing `django-admin-index-3.0.0/django_admin_index/templatetags/django_admin_index.py` & `django-admin-index-3.1.0/django_admin_index/templatetags/django_admin_index.py`

 * *Files identical despite different names*

### Comparing `django-admin-index-3.0.0/django_admin_index.egg-info/PKG-INFO` & `django-admin-index-3.1.0/django_admin_index.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-index
-Version: 3.0.0
+Version: 3.1.0
 Summary: Admin index for Django
 Home-page: https://github.com/maykinmedia/django-admin-index
 Author: Joeri Bekker
 Author-email: joeri@maykinmedia.nl
 License: BSD
 Project-URL: Changelog, https://github.com/maykinmedia/django-admin-index/blob/master/CHANGELOG.rst
 Project-URL: Bug Tracker, https://github.com/maykinmedia/django-admin-index/issues
@@ -35,15 +35,15 @@
 Provides-Extra: release
 License-File: LICENSE
 
 ======================
 Admin Index for Django
 ======================
 
-:Version: 3.0.0
+:Version: 3.1.0
 :Download: https://pypi.python.org/pypi/django-admin-index
 :Source: https://github.com/maykinmedia/django-admin-index
 :Keywords: django, admin, dashboard
 
 |build-status| |code-quality| |black| |coverage| |license| |python-versions| |django-versions| |pypi-version|
 
 About
@@ -275,15 +275,15 @@
     :alt: BSD License
     :target: https://opensource.org/licenses/BSD-3-Clause
 
 .. |python-versions| image:: https://img.shields.io/pypi/pyversions/django-admin-index.svg
     :alt: Supported Python versions
     :target: http://pypi.python.org/pypi/django-admin-index/
 
-.. |django-versions| image:: https://img.shields.io/badge/django-2.2%2C%203.0%2C%203.2%2C%204.0-blue.svg
+.. |django-versions| image:: https://img.shields.io/pypi/djversions/django-admin-index.svg
     :alt: Supported Django versions
     :target: http://pypi.python.org/pypi/django-admin-index/
 
 .. |pypi-version| image:: https://img.shields.io/pypi/v/django-admin-index.svg
     :target: https://pypi.org/project/django-admin-index/
 
 .. |screenshot-1| image:: https://github.com/maykinmedia/django-admin-index/raw/master/docs/_assets/dashboard_with_menu_thumb.png
```

### Comparing `django-admin-index-3.0.0/django_admin_index.egg-info/SOURCES.txt` & `django-admin-index-3.1.0/django_admin_index.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,25 +7,28 @@
 setup.cfg
 setup.py
 django_admin_index/__init__.py
 django_admin_index/admin.py
 django_admin_index/apps.py
 django_admin_index/conf.py
 django_admin_index/models.py
+django_admin_index/translations.py
 django_admin_index/utils.py
 django_admin_index.egg-info/PKG-INFO
 django_admin_index.egg-info/SOURCES.txt
 django_admin_index.egg-info/dependency_links.txt
 django_admin_index.egg-info/not-zip-safe
 django_admin_index.egg-info/requires.txt
 django_admin_index.egg-info/top_level.txt
 django_admin_index/migrations/0001_initial.py
 django_admin_index/migrations/0002_auto_20170802_1754.py
 django_admin_index/migrations/0003_auto_20200724_1516.py
 django_admin_index/migrations/0004_auto_20230503_0723.py
+django_admin_index/migrations/0005_auto_20230503_1910.py
+django_admin_index/migrations/0006_auto_20230503_1910.py
 django_admin_index/migrations/__init__.py
 django_admin_index/static/admin/css/admin-index.css
 django_admin_index/static/admin/css/admin-index.css.map
 django_admin_index/templates/admin/change_form.html
 django_admin_index/templates/admin/change_list.html
 django_admin_index/templates/admin/delete_confirmation.html
 django_admin_index/templates/admin/delete_selected_confirmation.html
```

### Comparing `django-admin-index-3.0.0/scss/_vars.scss` & `django-admin-index-3.1.0/scss/_vars.scss`

 * *Files identical despite different names*

### Comparing `django-admin-index-3.0.0/scss/components/_containers.scss` & `django-admin-index-3.1.0/scss/components/_containers.scss`

 * *Files identical despite different names*

### Comparing `django-admin-index-3.0.0/scss/components/_dropdown-menu.scss` & `django-admin-index-3.1.0/scss/components/_dropdown-menu.scss`

 * *Files identical despite different names*

### Comparing `django-admin-index-3.0.0/scss/components/_header.scss` & `django-admin-index-3.1.0/scss/components/_header.scss`

 * *Files identical despite different names*

### Comparing `django-admin-index-3.0.0/setup.cfg` & `django-admin-index-3.1.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-admin-index
-version = 3.0.0
+version = 3.1.0
 description = Admin index for Django
 long_description = file: README.rst
 url = https://github.com/maykinmedia/django-admin-index
 project_urls = 
 	Changelog = https://github.com/maykinmedia/django-admin-index/blob/master/CHANGELOG.rst
 	Bug Tracker = https://github.com/maykinmedia/django-admin-index/issues
 	Source Code = https://github.com/maykinmedia/django-admin-index
```

