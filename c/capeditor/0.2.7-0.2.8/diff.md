# Comparing `tmp/capeditor-0.2.7.tar.gz` & `tmp/capeditor-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capeditor-0.2.7.tar", last modified: Wed Jul 12 22:05:43 2023, max compression
+gzip compressed data, was "capeditor-0.2.8.tar", last modified: Fri Jul 14 14:00:01 2023, max compression
```

## Comparing `capeditor-0.2.7.tar` & `capeditor-0.2.8.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:05:43.751358 capeditor-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-12 22:05:26.000000 capeditor-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-07-12 22:05:43.751358 capeditor-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-07-12 22:05:26.000000 capeditor-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:05:43.747357 capeditor-0.2.7/capeditor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    23891 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/blocks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:05:43.747357 capeditor-0.2.7/capeditor/forms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/forms/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/forms/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:05:43.743357 capeditor-0.2.7/capeditor/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:05:43.739357 capeditor-0.2.7/capeditor/locale/am/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:05:43.747357 capeditor-0.2.7/capeditor/locale/am/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20372 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/locale/am/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    30677 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/locale/am/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:05:43.739357 capeditor-0.2.7/capeditor/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:05:43.747357 capeditor-0.2.7/capeditor/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19629 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    30023 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:05:43.739357 capeditor-0.2.7/capeditor/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:05:43.747357 capeditor-0.2.7/capeditor/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    16403 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    26134 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:05:43.743357 capeditor-0.2.7/capeditor/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:05:43.747357 capeditor-0.2.7/capeditor/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17296 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    27356 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:05:43.743357 capeditor-0.2.7/capeditor/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:05:43.747357 capeditor-0.2.7/capeditor/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    17262 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    27296 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:05:43.743357 capeditor-0.2.7/capeditor/locale/sw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:05:43.747357 capeditor-0.2.7/capeditor/locale/sw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    16625 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/locale/sw/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    26453 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/locale/sw/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:05:43.747357 capeditor-0.2.7/capeditor/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14556 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/renderers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:05:43.743357 capeditor-0.2.7/capeditor/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:05:43.743357 capeditor-0.2.7/capeditor/static/capeditor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:05:43.747357 capeditor-0.2.7/capeditor/static/capeditor/css/
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/static/capeditor/css/cap_detail_page.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:05:43.747357 capeditor-0.2.7/capeditor/static/capeditor/css/widget/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/static/capeditor/css/widget/boundary-widget.css
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/static/capeditor/css/widget/circle-widget.css
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/static/capeditor/css/widget/polygon-widget.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:05:43.747357 capeditor-0.2.7/capeditor/static/capeditor/js/
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/static/capeditor/js/cap_accordion.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:05:43.751358 capeditor-0.2.7/capeditor/static/capeditor/js/widget/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/static/capeditor/js/widget/boundary-polygon-widget-telepath.js
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/static/capeditor/js/widget/boundary-polygon-widget.js
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/static/capeditor/js/widget/circle-widget-telepath.js
--rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/static/capeditor/js/widget/circle-widget.js
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/static/capeditor/js/widget/conditional_fields.js
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/static/capeditor/js/widget/polygon-widget-telepath.js
--rw-r--r--   0 runner    (1001) docker     (123)    10704 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/static/capeditor/js/widget/polygon-widget.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:05:43.743357 capeditor-0.2.7/capeditor/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:05:43.751358 capeditor-0.2.7/capeditor/templates/capeditor/
--rw-r--r--   0 runner    (1001) docker     (123)    15623 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/templates/capeditor/cap_alert_page.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:05:43.751358 capeditor-0.2.7/capeditor/templates/capeditor/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/templates/capeditor/icons/cap-alert-full.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/templates/capeditor/icons/cap-alert.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:05:43.751358 capeditor-0.2.7/capeditor/templates/capeditor/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/templates/capeditor/widgets/boundary_polygon_widget.html
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/templates/capeditor/widgets/circle_widget.html
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/templates/capeditor/widgets/polygon_widget.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-12 22:05:26.000000 capeditor-0.2.7/capeditor/wagtail_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:05:43.747357 capeditor-0.2.7/capeditor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-07-12 22:05:43.000000 capeditor-0.2.7/capeditor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-12 22:05:43.000000 capeditor-0.2.7/capeditor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 22:05:43.000000 capeditor-0.2.7/capeditor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-12 22:05:43.000000 capeditor-0.2.7/capeditor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 22:05:43.000000 capeditor-0.2.7/capeditor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-12 22:05:26.000000 capeditor-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-12 22:05:43.751358 capeditor-0.2.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:01.242204 capeditor-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-14 13:59:42.000000 capeditor-0.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-07-14 14:00:01.242204 capeditor-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-07-14 13:59:42.000000 capeditor-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:01.234204 capeditor-0.2.8/capeditor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24001 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/blocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:01.234204 capeditor-0.2.8/capeditor/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/forms/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/forms/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:01.234204 capeditor-0.2.8/capeditor/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:01.230204 capeditor-0.2.8/capeditor/locale/am/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:01.238204 capeditor-0.2.8/capeditor/locale/am/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18830 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/locale/am/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30674 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/locale/am/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:01.230204 capeditor-0.2.8/capeditor/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:01.238204 capeditor-0.2.8/capeditor/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18042 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30025 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:01.230204 capeditor-0.2.8/capeditor/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:01.238204 capeditor-0.2.8/capeditor/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    15036 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    26134 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:01.230204 capeditor-0.2.8/capeditor/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:01.238204 capeditor-0.2.8/capeditor/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    15856 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    27357 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:01.234204 capeditor-0.2.8/capeditor/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:01.238204 capeditor-0.2.8/capeditor/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    15859 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    27296 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:01.234204 capeditor-0.2.8/capeditor/locale/sw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:01.238204 capeditor-0.2.8/capeditor/locale/sw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    15240 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/locale/sw/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    26457 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/locale/sw/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:01.238204 capeditor-0.2.8/capeditor/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14563 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:01.234204 capeditor-0.2.8/capeditor/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:01.234204 capeditor-0.2.8/capeditor/static/capeditor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:01.238204 capeditor-0.2.8/capeditor/static/capeditor/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/static/capeditor/css/cap_detail_page.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:01.238204 capeditor-0.2.8/capeditor/static/capeditor/css/widget/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/static/capeditor/css/widget/boundary-widget.css
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/static/capeditor/css/widget/circle-widget.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/static/capeditor/css/widget/polygon-widget.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:01.238204 capeditor-0.2.8/capeditor/static/capeditor/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/static/capeditor/js/cap_accordion.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/static/capeditor/js/conditional_fields.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:01.238204 capeditor-0.2.8/capeditor/static/capeditor/js/widget/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/static/capeditor/js/widget/boundary-polygon-widget-telepath.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/static/capeditor/js/widget/boundary-polygon-widget.js
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/static/capeditor/js/widget/circle-widget-telepath.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/static/capeditor/js/widget/circle-widget.js
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/static/capeditor/js/widget/polygon-widget-telepath.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10704 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/static/capeditor/js/widget/polygon-widget.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:01.234204 capeditor-0.2.8/capeditor/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:01.238204 capeditor-0.2.8/capeditor/templates/capeditor/
+-rw-r--r--   0 runner    (1001) docker     (123)    15623 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/templates/capeditor/cap_alert_page.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:01.238204 capeditor-0.2.8/capeditor/templates/capeditor/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/templates/capeditor/icons/cap-alert-full.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/templates/capeditor/icons/cap-alert.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:01.242204 capeditor-0.2.8/capeditor/templates/capeditor/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/templates/capeditor/widgets/boundary_polygon_widget.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/templates/capeditor/widgets/circle_widget.html
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/templates/capeditor/widgets/polygon_widget.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-14 13:59:42.000000 capeditor-0.2.8/capeditor/wagtail_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:00:01.234204 capeditor-0.2.8/capeditor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-07-14 14:00:01.000000 capeditor-0.2.8/capeditor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-14 14:00:01.000000 capeditor-0.2.8/capeditor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 14:00:01.000000 capeditor-0.2.8/capeditor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-14 14:00:01.000000 capeditor-0.2.8/capeditor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-14 14:00:01.000000 capeditor-0.2.8/capeditor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-14 13:59:42.000000 capeditor-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-14 14:00:01.242204 capeditor-0.2.8/setup.cfg
```

### Comparing `capeditor-0.2.7/PKG-INFO` & `capeditor-0.2.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capeditor
-Version: 0.2.7
+Version: 0.2.8
 Summary: Wagtail based CAP Editor
 Home-page: https://github.com/wmo-raf/cap-editor
 Author: Grace Amondi, Erick Otenyo
 Author-email: miswa.grace@gmail.com, otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -51,27 +51,21 @@
             -   [B. Alert Info](#b.-alert-info)
             -   [C. Alert Area](#c.-alert-area)
             -   [D. Alert Resource](#d.-alert-resource)
     -   [Integrations](#integrations)
     
 ## Quick start
 
-#### 1. Clone repository
+#### 1. Install in virualenvironment using pip
 
 ``` sh
-git clone https://github.com/wmo-raf/cap-editor.git
+pip install capeditor
 ```
 
-#### 2. Install in virualenvironment using pip
-
-``` sh
-pip install path_to/capeditor/dist/capeditor-{version}.tar.gz
-```
-
-#### 3. Configure settings
+#### 2. Configure settings
 
 In your `settings.py` or `settings/base.py`, within the installed apps,
 include the `rest_framework, rest_framework_xml` and `capeditor` as
 below:
 
 ``` py
 INSTALLED_APPS = [
@@ -92,31 +86,15 @@
     ),
     'DEFAULT_PARSER_CLASSES': (
         'rest_framework_xml.parsers.XMLParser',
     ),
 }
 ```
 
-#### 4. Include the cap urls
-
-In `urls.py`, include the cap urls as below. This is where the cap api
-for listed (`/cap/caps.xml`) and detailed(`/cap/{cap_id}.xml`) cap view
-will be hosted.
-
-``` py
-from capeditor import urls as cap_urls
-
-urlpatterns = [
-    # ...
-    path('cap', include(cap_urls))
-
-]
-```
-
-#### 5. Run model migrations
+#### 3. Run model migrations
 
 ``` sh
 python manage.py migrate
 ```
 
 ## Usage
 
@@ -242,54 +220,10 @@
 Multiple instances of this section are allowed. It contains the
 **Description (resourceDesc), MIME Type (mimeType), File Size (size),
 URI (uri), Dereferenced URI (derefUri) and Digest (digest)**
 
 ## Integrations
 
 To integrate the alerts to another wagtail page and include in
-templates, for example in the home page follow the instructions below:
+templates, for example in the home page refer to sandbox folder for sample standalone.
 
-Call the alerts in your models.py under the 'get_context' method:
 
-``` py
-from capeditor.models import Alert
-
-class HomePage(Page):
-
-    # ...
-
-
-    def get_context(self, request, *args, **kwargs):
-        context =super().get_context(request, *args, **kwargs)
-       
-        context['alerts'] = Alert.objects.live().public()
-        context['latest_alerts'] = context['alerts'][:3]
-        return context  
-```
-
-Parse the alerts in the home template:
-
-``` django
-
-{% for alert in latest_alerts.all %}
-    
-    <p>{{alert.sent}}</p>
-
-    <!-- info list  -->
-    {% for info in alert.alert_info.all %}
-        {% if alerts %}
-
-            <p>{{info.event}}</p>
-            <p>{{info.get_severity_display}}</p>
-
-            <!-- area list  -->
-            {% for alert_area in info.alert_areas.values%}
-                <p>{{alert_area.areaDesc}}</p>
-                <p>{{ alert_area.area }}</p>
-            {% endfor %}
-
-            <!-- other fields  -->
-
-        {% endif %}
-    {% endfor %}
-{% endfor %}
-```
```

### Comparing `capeditor-0.2.7/README.md` & `capeditor-0.2.8/capeditor.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: capeditor
+Version: 0.2.8
+Summary: Wagtail based CAP Editor
+Home-page: https://github.com/wmo-raf/cap-editor
+Author: Grace Amondi, Erick Otenyo
+Author-email: miswa.grace@gmail.com, otenyo.erick@gmail.com
+License: MIT
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+
 # CAP Editor  <img style="float: right;" height="40" src="images/caplogo.jpeg" markdown="1"> 
 [![Upload Python Package](https://github.com/wmo-raf/cap-editor/actions/workflows/publish.yml/badge.svg)](https://github.com/wmo-raf/cap-editor/actions/workflows/publish.yml)
 
 A Wagtail Commmon Alerting Protocol (CAP) Editor python package
 installable as an app on any wagtail project (version\>=4.1).
 
 The **Common Alerting Protocol (CAP)** provides an open, non-proprietary
@@ -30,27 +51,21 @@
             -   [B. Alert Info](#b.-alert-info)
             -   [C. Alert Area](#c.-alert-area)
             -   [D. Alert Resource](#d.-alert-resource)
     -   [Integrations](#integrations)
     
 ## Quick start
 
-#### 1. Clone repository
+#### 1. Install in virualenvironment using pip
 
 ``` sh
-git clone https://github.com/wmo-raf/cap-editor.git
+pip install capeditor
 ```
 
-#### 2. Install in virualenvironment using pip
-
-``` sh
-pip install path_to/capeditor/dist/capeditor-{version}.tar.gz
-```
-
-#### 3. Configure settings
+#### 2. Configure settings
 
 In your `settings.py` or `settings/base.py`, within the installed apps,
 include the `rest_framework, rest_framework_xml` and `capeditor` as
 below:
 
 ``` py
 INSTALLED_APPS = [
@@ -71,31 +86,15 @@
     ),
     'DEFAULT_PARSER_CLASSES': (
         'rest_framework_xml.parsers.XMLParser',
     ),
 }
 ```
 
-#### 4. Include the cap urls
-
-In `urls.py`, include the cap urls as below. This is where the cap api
-for listed (`/cap/caps.xml`) and detailed(`/cap/{cap_id}.xml`) cap view
-will be hosted.
-
-``` py
-from capeditor import urls as cap_urls
-
-urlpatterns = [
-    # ...
-    path('cap', include(cap_urls))
-
-]
-```
-
-#### 5. Run model migrations
+#### 3. Run model migrations
 
 ``` sh
 python manage.py migrate
 ```
 
 ## Usage
 
@@ -221,54 +220,10 @@
 Multiple instances of this section are allowed. It contains the
 **Description (resourceDesc), MIME Type (mimeType), File Size (size),
 URI (uri), Dereferenced URI (derefUri) and Digest (digest)**
 
 ## Integrations
 
 To integrate the alerts to another wagtail page and include in
-templates, for example in the home page follow the instructions below:
+templates, for example in the home page refer to sandbox folder for sample standalone.
 
-Call the alerts in your models.py under the 'get_context' method:
 
-``` py
-from capeditor.models import Alert
-
-class HomePage(Page):
-
-    # ...
-
-
-    def get_context(self, request, *args, **kwargs):
-        context =super().get_context(request, *args, **kwargs)
-       
-        context['alerts'] = Alert.objects.live().public()
-        context['latest_alerts'] = context['alerts'][:3]
-        return context  
-```
-
-Parse the alerts in the home template:
-
-``` django
-
-{% for alert in latest_alerts.all %}
-    
-    <p>{{alert.sent}}</p>
-
-    <!-- info list  -->
-    {% for info in alert.alert_info.all %}
-        {% if alerts %}
-
-            <p>{{info.event}}</p>
-            <p>{{info.get_severity_display}}</p>
-
-            <!-- area list  -->
-            {% for alert_area in info.alert_areas.values%}
-                <p>{{alert_area.areaDesc}}</p>
-                <p>{{ alert_area.area }}</p>
-            {% endfor %}
-
-            <!-- other fields  -->
-
-        {% endif %}
-    {% endfor %}
-{% endfor %}
-```
```

### Comparing `capeditor-0.2.7/capeditor/blocks.py` & `capeditor-0.2.8/capeditor/blocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -501,21 +501,22 @@
     CERTAINTY_CHOICES = (
         ('Observed', _("Observed - Determined to have occurred or to be ongoing")),
         ('Likely', _("Likely - Likely (percentage > ~50%)")),
         ('Possible', _("Possible - Possible but not likely (percentage <= ~50%)")),
         ('Unlikely', _("Unlikely - Not expected to occur (percentage ~ 0)")),
         ('Unknown', _("Unknown - Certainty unknown")),
     )
+    event = blocks.CharBlock(max_length=255, label=_("Event"), help_text=EVENT_HELP_TEXT)
 
-    language = blocks.ChoiceBlock(choices=LANGUAGE_CHOICES, default="en", required=False, label=_("Language"),
-                                  help_text=_("The code denoting the language of the alert message"), )
     category = blocks.ChoiceBlock(choices=CATEGORY_CHOICES, default="Met", label=_("Category"),
                                   help_text=_("The code denoting the category of the subject"
                                               " event of the alert message"))
-    event = blocks.CharBlock(max_length=255, label=_("Event"), help_text=EVENT_HELP_TEXT)
+    language = blocks.ChoiceBlock(choices=LANGUAGE_CHOICES, default="en", required=False, label=_("Language"),
+                                  help_text=_("The code denoting the language of the alert message"), )
+    
     urgency = blocks.ChoiceBlock(choices=URGENCY_CHOICES, label=_("Urgency"),
                                  help_text=_("The code denoting the urgency of the subject "
                                              "event of the alert message"))
     severity = blocks.ChoiceBlock(choices=SEVERITY_CHOICES, label=_("Severity"),
                                   help_text=_("The code denoting the severity of the subject "
                                               "event of the alert message"))
     certainty = blocks.ChoiceBlock(choices=CERTAINTY_CHOICES, label=_("Certainty"),
@@ -562,14 +563,17 @@
                                                          "related to this alert information"))
 
     parameter = blocks.ListBlock(AlertInfoParameter(label=_("Parameter")), label=_("Parameters"), default=[])
     eventCode = blocks.ListBlock(AlertEventCode(label=_("Event Code")), label=_("Event codes"), default=[])
 
     # NOTE: web attribute is obtained from the url of the page
 
+    class Meta:
+        value_class = AlertInfoStructValue
+        label_format = "({language}) {event}"
 
 class HazardTypeBlock(blocks.StructBlock):
     hazard = blocks.CharBlock(max_length=255, label=_("Hazard"), help_text="Name of Hazard")
     icon = IconChooserBlock(required=False)
 
 
 class AudienceTypeBlock(blocks.StructBlock):
```

### Comparing `capeditor-0.2.7/capeditor/forms/widgets.py` & `capeditor-0.2.8/capeditor/forms/widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,23 +36,22 @@
 
 class BasePolygonWidget(BaseGeometryWidget, BaseMapWidget):
     def serialize(self, value):
         return value.json if value else ""
 
     def deserialize(self, value):
         geom = super().deserialize(value)
-        tolerance = 0.0002
+        tolerance = 0.05
 
         if geom.geom_type != "Polygon":
             # try to get the smallest Polygon that contains all the geometries in the MultiPolygon.
             geom = geom.unary_union
 
-        if geom.geom_type != "Polygon":
-            # still not a Polygon. Try initial simplification
-            geom = geom.simplify(tolerance)
+        # first simplification
+        geom = geom.simplify(tolerance)
 
         # still not a Polygon. Simplify with incrementing tolerance until we have a polygon
         while geom.geom_type != "Polygon":
             tolerance *= 2
             geom = geom.simplify(tolerance)
 
         # check for holes and close if any
```

### Comparing `capeditor-0.2.7/capeditor/locale/am/LC_MESSAGES/django.mo` & `capeditor-0.2.8/capeditor/locale/am/LC_MESSAGES/django.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,90 +7,80 @@
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 msgid ""
-" Identifies the originator of an alert. This can be an email of the "
-"institution for example"
-msgstr "የማንቂያ ጀማሪን ይለያል። ይህ ለምሳሌ የተቋሙ ኢሜይል ሊሆን ይችላል።"
-
-msgid ""
 "Acknowledge - Acknowledges receipt and acceptance of the message(s) "
 "identified in references field"
 msgstr "እውቅና - በማጣቀሻ መስክ ውስጥ ተለይተው የታወቁትን መልእክት (ቶች) መቀበል እና መቀበልን እውቅና ይሰጣል"
 
 msgid "Actual - Actionable by all targeted recipients"
 msgstr "ትክክለኛ - በሁሉም የታለሙ ተቀባዮች ሊተገበር የሚችል"
 
+msgid ""
+"Additional file with supplemental information related to this alert "
+"information"
+msgstr "ከዚህ የማንቂያ መረጃ ጋር የተያያዘ ተጨማሪ መረጃ ያለው ተጨማሪ ፋይል"
+
+msgid "Addresses"
+msgstr "አድራሻዎች"
+
+msgid "Admin Boundary"
+msgstr "የአስተዳዳሪ ወሰን"
+
+msgid "Admin Boundary, Polygon, Circle or Geocode"
+msgstr "የአስተዳዳሪ ድንበር ፣ ፖሊጎን ፣ ክበብ ወይም ጂኦኮድ"
+
+msgid "Administrative Level"
+msgstr "የአስተዳደር ደረጃ"
+
 msgid "Affected areas / Regions"
 msgstr "የተጎዱ አካባቢዎች / ክልሎች"
 
-msgid "Alert"
-msgstr "ማንቂያ"
-
 msgid "Alert - Initial information requiring attention by targeted recipients"
 msgstr "ማንቂያ - በታለመላቸው ተቀባዮች ትኩረት የሚፈልግ የመጀመሪያ መረጃ"
 
 msgid "Alert Area"
 msgstr "ማንቂያ አካባቢ"
 
-msgid "Alert Areas "
-msgstr "የማንቂያ ቦታዎች"
-
-msgid ""
-"Alert Categorization (Category, Urgency, Severity, Certainity, Response & "
-"Dates)"
-msgstr "የማንቂያ ምድብ (ምድብ፣ አጣዳፊነት፣ ክብደት፣ እርግጠኝነት፣ ምላሽ እና ቀኖች)"
-
-msgid ""
-"Alert Delivery Message (Headline, Description, Intsructions, Contact & "
-"Website)"
-msgstr "የማንቂያ ማቅረቢያ መልእክት (አርዕስት፣ መግለጫ፣ መመሪያ፣ አድራሻ እና ድር ጣቢያ)"
-
-msgid "Alert Identification (Sender, Message Type, Scope)"
-msgstr "የማንቂያ መለያ (ላኪ፣ የመልእክት አይነት፣ ወሰን)"
-
-msgid "Alert Info"
-msgstr "የማንቂያ መረጃ"
-
 msgid "Alert Information"
 msgstr "የማንቂያ መረጃ"
 
-msgid "Alert Resources "
-msgstr "የማንቂያ መርጃዎች"
-
-msgid "Alerts Per Page"
-msgstr "ማንቂያዎች በገጽ"
-
 msgid ""
 "All Clear - The subject event no longer poses a threat or concern and any "
 "follow on action is described in instruction"
 msgstr ""
 "ሁሉም ግልጽ - የርዕሰ-ጉዳዩ ክስተት ከአሁን በኋላ ስጋት ወይም ስጋት አያመጣም እና ማንኛውም የተግባር ክትትል "
 "በመመሪያው ውስጥ ተገልጿል"
 
 msgid "Altitude"
 msgstr "ከፍታ"
 
-msgid "Area"
-msgstr "አካባቢ"
-
 msgid ""
 "Assess - Evaluate the information in this message - DONT USE FOR PUBLIC "
 "ALERTS"
 msgstr "ይገምግሙ - በዚህ መልእክት ውስጥ ያለውን መረጃ ይገምግሙ - ለሕዝብ ማንቂያዎች አይጠቀሙ"
 
 msgid "Audience"
 msgstr "ታዳሚዎች"
 
 msgid "Avoid - Avoid the subject event as per the instruction"
 msgstr "አስወግዱ - እንደ መመሪያው የርዕሰ-ጉዳዩን ክስተት ያስወግዱ"
 
+msgid "Boundary"
+msgstr "ድንበር"
+
+msgid "CAP Sender Name"
+msgstr "የ CAP ላኪ ስም"
+
+msgid "Can be the website link or email of the sending institution"
+msgstr "የላኪው ተቋም የድር ጣቢያ አገናኝ ወይም ኢሜይል ሊሆን ይችላል።"
+
 msgid "Cancel - Cancels the earlier message(s) identified in references"
 msgstr "ሰርዝ - በማጣቀሻዎች ውስጥ የተገለጸውን የቀደመ መልእክት(ዎች) ይሰርዛል"
 
 msgid "Category"
 msgstr "ምድብ"
 
 msgid "Ceiling"
@@ -100,45 +90,42 @@
 msgstr "እርግጠኝነት"
 
 msgid ""
 "Chemical, Biological, Radiological, Nuclear or High-Yield Explosive threat "
 "or attack"
 msgstr "ኬሚካል፣ ባዮሎጂካል፣ ራዲዮሎጂካል፣ ኑክሌር ወይም ከፍተኛ ምርት የሚፈነዳ ዛቻ ወይም ጥቃት"
 
+msgid "Circle"
+msgstr "ክብ"
+
 msgid "Code"
 msgstr "ኮድ"
 
 msgid "Contact"
 msgstr "ተገናኝ"
 
 msgid "Description"
 msgstr "መግለጫ"
 
-msgid "Description of the incident"
-msgstr "የክስተቱ መግለጫ"
-
 msgid ""
 "Draft - A preliminary template or draft, not actionable in its current form"
 msgstr "ረቂቅ - ቀዳሚ አብነት ወይም ረቂቅ፣ አሁን ባለው መልኩ ሊተገበር የሚችል አይደለም።"
 
-msgid "Earlier Reference Alerts -  If applicable"
-msgstr "ቀደምት የማጣቀሻ ማንቂያዎች - አስፈላጊ ከሆነ"
+msgid "Drag the marker to change position"
+msgstr "ቦታውን ለመቀየር ምልክት ማድረጊያውን ይጎትቱት።"
+
+msgid "Draw Polygon"
+msgstr "ፖሊጎን ይሳሉ"
 
 msgid "Earlier alert referenced by this alert"
 msgstr "የቀደመው ማንቂያ በዚህ ማንቂያ ተጠቅሷል"
 
 msgid "Effective"
 msgstr "ውጤታማ"
 
-msgid "Email"
-msgstr "ኢሜይል"
-
-msgid "Email address"
-msgstr "የ ኢሜል አድራሻ"
-
 msgid "English"
 msgstr "እንግሊዝኛ"
 
 msgid ""
 "Error -  Indicates rejection of the message(s) identified in references; "
 "explanation SHOULD appear in note field"
 msgstr ""
@@ -157,81 +144,75 @@
 msgid ""
 "Exercise - Actionable only by designated exercise participants; exercise "
 "identifier SHOULD appear in note"
 msgstr ""
 "የአካል ብቃት እንቅስቃሴ - በተሰየሙ የአካል ብቃት እንቅስቃሴ ተሳታፊዎች ብቻ ሊተገበር የሚችል; የአካል ብቃት "
 "እንቅስቃሴ መለያ በማስታወሻ ውስጥ መታየት አለበት።"
 
-msgid "Expected"
-msgstr "የሚጠበቀው"
-
 msgid "Expected - Responsive action SHOULD be taken soon (within next hour)"
 msgstr "የሚጠበቀው - ምላሽ ሰጪ እርምጃ በቅርቡ መወሰድ አለበት (በሚቀጥለው ሰዓት ውስጥ)"
 
 msgid "Expires"
 msgstr "ጊዜው ያበቃል"
 
 msgid "Extreme - Extraordinary threat to life or property"
 msgstr "እጅግ በጣም ከባድ - ለሕይወት ወይም ለንብረት ያልተለመደ ስጋት"
 
-msgid "File"
-msgstr "ፋይል"
-
-msgid "File, Document etc"
-msgstr "ሰነድ ፣ ፋይል ፣ ወዘተ"
-
 msgid "Fire suppression and rescue"
 msgstr "እሳትን ማዳን እና ማዳን"
 
-msgid "Future"
-msgstr "ወደፊት"
-
 msgid "Future - Responsive action SHOULD be taken in the near future"
 msgstr "ወደፊት - ምላሽ ሰጪ እርምጃ በቅርብ ጊዜ ውስጥ መወሰድ አለበት"
 
 msgid "General emergency and public safety"
 msgstr "አጠቃላይ ድንገተኛ እና የህዝብ ደህንነት"
 
+msgid "Geocode"
+msgstr "ጂኦኮድ"
+
 msgid "Geophysical"
 msgstr "ጂኦፊዚካል"
 
+msgid "Hazard"
+msgstr "ሃዛርድ"
+
+msgid "Hazards monitored by the institution"
+msgstr "በተቋሙ ቁጥጥር የሚደረግባቸው አደጋዎች"
+
 msgid "Headline"
 msgstr "ርዕስ"
 
-msgid ""
-"How many of this products should be visible on the landing page filter "
-"section ?"
-msgstr "ከእነዚህ ምርቶች ውስጥ ስንት ናቸው በማረፊያ ገጽ ማጣሪያ ክፍል ላይ መታየት ያለባቸው?"
-
 msgid "Identifier"
 msgstr "መለያ"
 
-msgid "Immediate"
-msgstr "ወዲያውኑ"
-
 msgid "Immediate - Responsive action SHOULD be taken immediately"
 msgstr "ወዲያውኑ - ምላሽ ሰጪ እርምጃ ወዲያውኑ መወሰድ አለበት"
 
+msgid "Incident"
+msgstr "ክስተት"
+
+msgid "Incidents"
+msgstr "ክስተቶች"
+
 msgid "Instruction"
 msgstr "መመሪያ"
 
-msgid "Intended Recipients (If scope is Private) "
-msgstr "የታቀዱ ተቀባዮች (ክልሉ የግል ከሆነ)"
-
 msgid "Language"
 msgstr "ቋንቋ"
 
 msgid "Law enforcement, military, homeland and local/private security"
 msgstr "የሕግ አስከባሪ፣ ወታደራዊ፣ የአገር ቤት እና የአካባቢ/የግል ደህንነት"
 
 msgid "Likely - Likely (percentage > ~50%)"
 msgstr "ምናልባት - ምናልባት (መቶኛ > ~ 50%)"
 
-msgid "Link"
-msgstr "አገናኝ"
+msgid ""
+"Link to external resource. This can be for example a link to related "
+"websites. "
+msgstr "ወደ ውጫዊ ምንጭ አገናኝ. ይህ ለምሳሌ ወደ ተዛማጅ ድር ጣቢያዎች አገናኝ ሊሆን ይችላል."
 
 msgid "Medical and public health"
 msgstr "የሕክምና እና የህዝብ ጤና"
 
 msgid "Message Type"
 msgstr "የመልእክት አይነት"
 
@@ -249,17 +230,14 @@
 
 msgid "Name"
 msgstr "ስም"
 
 msgid "Name for the event code"
 msgstr "የክስተት ኮድ ስም"
 
-msgid "Name for the geocode"
-msgstr "የጂኦኮድ ስም"
-
 msgid "Name of the recipient"
 msgstr "የተቀባዩ ስም"
 
 msgid "No action recommended"
 msgstr "ምንም እርምጃ አይመከርም"
 
 msgid "Note"
@@ -270,23 +248,29 @@
 
 msgid "Onset"
 msgstr "ጅምር"
 
 msgid "Other events"
 msgstr "ሌሎች ክስተቶች"
 
-msgid "Past"
-msgstr "ያለፈው"
+msgid "Parameter"
+msgstr "መለኪያ"
+
+msgid "Parameters"
+msgstr "መለኪያዎች"
 
 msgid "Past - Responsive action is no longer required"
 msgstr "ያለፈው - ምላሽ ሰጪ እርምጃ ከአሁን በኋላ አያስፈልግም"
 
 msgid "Pollution and other environmental"
 msgstr "ብክለት እና ሌሎች አካባቢያዊ"
 
+msgid "Polygon"
+msgstr "ፖሊጎን"
+
 msgid "Possible - Possible but not likely (percentage <= ~50%)"
 msgstr "ይቻላል - ይቻላል ነገር ግን የማይሆን ​​(መቶኛ <= ~ 50%)"
 
 msgid "Prepare - Relocate as instructed in the instruction"
 msgstr "አዘጋጅ - በመመሪያው ውስጥ እንደታዘዘው ወደ ሌላ ቦታ ይቀይሩ"
 
 msgid ""
@@ -305,20 +289,14 @@
 
 msgid "Reference Alert"
 msgstr "የማጣቀሻ ማንቂያ"
 
 msgid "Rescue and recovery"
 msgstr "ማዳን እና ማገገም"
 
-msgid "Resource"
-msgstr "ምንጭ"
-
-msgid "Resource type whether is image, file etc"
-msgstr "የመርጃ አይነት ምስል፣ ፋይል ወዘተ"
-
 msgid "Response type"
 msgstr "የምላሽ አይነት"
 
 msgid ""
 "Restricted - For dissemination only to users with a known operational "
 "requirement as in the restriction field"
 msgstr "የተገደበ - እንደ ገዳቢው መስክ የታወቀ የአሠራር መስፈርት ላላቸው ተጠቃሚዎች ብቻ ለማሰራጨት"
@@ -349,20 +327,20 @@
 
 msgid "Status"
 msgstr "ሁኔታ"
 
 msgid "System - For messages that support alert network internal functions"
 msgstr "ስርዓት - የማንቂያ አውታር ውስጣዊ ተግባራትን ለሚደግፉ መልዕክቶች"
 
+msgid "Target audiences for published alerts"
+msgstr "ለታተሙ ማንቂያዎች ዒላማ ታዳሚዎች"
+
 msgid "Test - Technical testing only, all recipients disregard"
 msgstr "ሙከራ - የቴክኒክ ሙከራ ብቻ፣ ሁሉም ተቀባዮች ችላ ይላሉ"
 
-msgid "The base-64 encoded data content of the resource file"
-msgstr "የመሠረት-64 ኮድ የተደረገበት የመረጃ ፋይሉ ይዘት"
-
 msgid "The code denoting the appropriate handling of the alert"
 msgstr "የማስጠንቀቂያውን ተገቢ አያያዝ የሚያመለክት ኮድ"
 
 msgid ""
 "The code denoting the category of the subject event of the alert message"
 msgstr "የማንቂያ መልእክቱ ርዕሰ ጉዳይ ክስተት ምድብን የሚያመለክት ኮድ"
 
@@ -390,35 +368,27 @@
 "The code denoting the type of action recommended for the target audience"
 msgstr "ለዒላማ ታዳሚዎች የሚመከር የእርምጃ አይነትን የሚያመለክት ኮድ"
 
 msgid "The code denoting the urgency of the subject event of the alert message"
 msgstr "የማንቂያ መልእክቱ የርእሰ ጉዳይ ክስተት አጣዳፊነት የሚያመለክት ኮድ"
 
 msgid ""
-"The code representing the digital digest ('hash') computed from the resource "
-"file"
-msgstr "ከንብረት ፋይሉ የተሰላውን ዲጂታል ዲጀስት ('hash') የሚወክል ኮድ"
-
-msgid "The effective time of the information of the alert message"
-msgstr "የማንቂያ መልእክት መረጃ ውጤታማ ጊዜ"
-
-msgid ""
 "The expected time of the beginning of the subject event of the alert message"
 msgstr "የማንቂያ መልእክቱ ርዕሰ ጉዳይ ክስተት የሚጠበቀው ጊዜ"
 
-msgid "The expiry time of the information of the alert message"
-msgstr "የማንቂያ መልእክቱ መረጃ የሚያበቃበት ጊዜ"
-
 msgid ""
-"The identifier of the hyperlink associating additional information with the "
-"alert message"
-msgstr "ተጨማሪ መረጃን ከማንቂያ መልዕክቱ ጋር የሚያገናኘው የሃይፐርሊንክ መለያ"
+"The expiry time of the information of the alert message. If not set, each "
+"recipient is free to set its own policy as to when the message is no longer "
+"in effect."
+msgstr ""
+"የማንቂያ መልእክቱ መረጃ የሚያበቃበት ጊዜ። ካልተዋቀረ እያንዳንዱ ተቀባይ መልእክቱ መቼ እንደማይሰራ የራሱን ፖሊሲ "
+"ለማዘጋጀት ነፃ ነው።"
 
-msgid "The identifier of the hyperlink for the resource file"
-msgstr "ለሀብት ፋይሉ የገጽ አገናኝ መለያ"
+msgid "The human-readable name of the agency or authority issuing this alert."
+msgstr "ይህን ማንቂያ የሚያወጣው ኤጀንሲ ወይም ባለስልጣን በሰው ሊነበብ የሚችል ስም።"
 
 msgid ""
 "The maximum altitude of the affected area of the alert message.MUST NOT be "
 "used except in combination with the altitude element. "
 msgstr ""
 "የማስጠንቀቂያ መልእክት የተጎዳው አካባቢ ከፍተኛው ከፍታ ከፍ ካለው ኤለመንት ጋር ካልተጣመረ በስተቀር ጥቅም ላይ መዋል "
 "የለበትም።"
@@ -461,68 +431,47 @@
 
 msgid ""
 "The text describing the rule for limiting distribution of the restricted "
 "alert message. Used when scope value is Restricted"
 msgstr ""
 "የተገደበ የማንቂያ መልእክት ስርጭትን ለመገደብ ደንቡን የሚገልጽ ጽሑፍ። የወሰን እሴት ሲገደብ ጥቅም ላይ ይውላል"
 
-msgid "The text describing the subject event of the alert message"
-msgstr "የማንቂያ መልእክቱን ርዕሰ ጉዳይ ክስተት የሚገልጽ ጽሑፍ"
-
 msgid "The text describing the type and content of the resource file"
 msgstr "የመርጃ ፋይሉን ዓይነት እና ይዘት የሚገልጽ ጽሑፍ"
 
-msgid "The text headline of the alert message"
-msgstr "የማንቂያ መልእክቱ የጽሑፍ ርዕስ"
+msgid ""
+"The text headline of the alert message. Make it direct and actionable as "
+"possible while remaining short"
+msgstr "የማንቂያ መልእክቱ የጽሑፍ ርዕስ። አጭር ሲቀሩ በተቻለ መጠን ቀጥተኛ እና ተግባራዊ ያድርጉት"
 
 msgid "The text identifying the source of the alert message"
 msgstr "የማንቂያ መልእክቱን ምንጭ የሚለይ ጽሑፍ"
 
 msgid "Time and date of origination of the alert"
 msgstr "የማንቂያው መነሻ ጊዜ እና ቀን"
 
-msgid "Title"
-msgstr "ርዕስ"
-
-msgid "Title of the incident referent of the alert"
-msgstr "የማስጠንቀቂያው የክስተት አመልካች ርዕስ"
-
 msgid "Unique ID. Auto generated on creation."
 msgstr "ልዩ መታወቂያ በፍጥረት ላይ በራስ-ሰር የተፈጠረ።"
 
-msgid "Unknown"
-msgstr "ያልታወቀ"
-
 msgid "Unknown - Certainty unknown"
 msgstr "ያልታወቀ - በእርግጠኝነት የማይታወቅ"
 
 msgid "Unknown - Severity unknown"
 msgstr "ያልታወቀ - ክብደት የማይታወቅ"
 
 msgid "Unknown - Urgency not known"
 msgstr "ያልታወቀ - አጣዳፊነት አይታወቅም"
 
 msgid "Unlikely - Not expected to occur (percentage ~ 0)"
 msgstr "የማይመስል - ይከሰታል ተብሎ አይጠበቅም (መቶኛ ~ 0)"
 
-msgid ""
-"Update - Updates and supercedes the earlier message(s) identified in "
-"referenced alerts"
-msgstr "አዘምን - በተጠቀሱት ማንቂያዎች ውስጥ የተገለጸውን የቀደመ መልእክት(ዎች) ያዘምናል እና ይበልጣል"
-
 msgid "Urgency"
 msgstr "አስቸኳይ"
 
 msgid "Utility, telecommunication, other non-transport infrastructure"
 msgstr "መገልገያ፣ ቴሌኮሙኒኬሽን፣ ሌሎች የትራንስፖርት ያልሆኑ መሠረተ ልማቶች"
 
 msgid "Value"
 msgstr "ዋጋ"
 
 msgid "Value of the event code"
 msgstr "የክስተቱ ኮድ ዋጋ"
-
-msgid "Value of the geocode"
-msgstr "የጂኦኮድ እሴት"
-
-msgid "Web"
-msgstr "ድር"
```

### Comparing `capeditor-0.2.7/capeditor/locale/am/LC_MESSAGES/django.po` & `capeditor-0.2.8/capeditor/locale/am/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-12 14:00+0300\n"
+"POT-Creation-Date: 2023-07-14 12:05+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
-#: capeditor/blocks.py:70 capeditor/blocks.py:98 capeditor/blocks.py:370
+#: capeditor/blocks.py:70 capeditor/blocks.py:98 capeditor/blocks.py:375
 msgid "Name"
 msgstr "ስም"
 
 #: capeditor/blocks.py:70
 msgid "Name of the recipient"
 msgstr "የተቀባዩ ስም"
 
@@ -51,15 +51,15 @@
 
 #: capeditor/blocks.py:94
 #, fuzzy
 #| msgid "The text headline of the alert message"
 msgid "Referent incident to this alert message"
 msgstr "ለዚህ የማንቂያ መልእክት የማጣቀሻ ክስተት"
 
-#: capeditor/blocks.py:99 capeditor/blocks.py:295 capeditor/blocks.py:371
+#: capeditor/blocks.py:99 capeditor/blocks.py:300 capeditor/blocks.py:376
 msgid "Value"
 msgstr "ዋጋ"
 
 #: capeditor/blocks.py:104
 msgid "Shelter - Take shelter in place or per instruction"
 msgstr "መጠለያ - በቦታ ወይም በመመሪያው መጠለል"
 
@@ -106,430 +106,430 @@
 msgstr "የምላሽ አይነት"
 
 #: capeditor/blocks.py:117
 msgid ""
 "The code denoting the type of action recommended for the target audience"
 msgstr "ለዒላማ ታዳሚዎች የሚመከር የእርምጃ አይነትን የሚያመለክት ኮድ"
 
-#: capeditor/blocks.py:158 capeditor/blocks.py:204 capeditor/blocks.py:256
-#: capeditor/blocks.py:292
+#: capeditor/blocks.py:163 capeditor/blocks.py:209 capeditor/blocks.py:261
+#: capeditor/blocks.py:297
 msgid "Affected areas / Regions"
 msgstr "የተጎዱ አካባቢዎች / ክልሎች"
 
-#: capeditor/blocks.py:159 capeditor/blocks.py:205 capeditor/blocks.py:257
-#: capeditor/blocks.py:293
+#: capeditor/blocks.py:164 capeditor/blocks.py:210 capeditor/blocks.py:262
+#: capeditor/blocks.py:298
 msgid "The text describing the affected area of the alert message"
 msgstr "የማስጠንቀቂያ መልእክት የተጎዳውን አካባቢ የሚገልጽ ጽሑፍ"
 
-#: capeditor/blocks.py:160
+#: capeditor/blocks.py:165
 msgid "Administrative Level"
 msgstr "የአስተዳደር ደረጃ"
 
-#: capeditor/blocks.py:161
+#: capeditor/blocks.py:166
 msgid "Boundary"
 msgstr "ድንበር"
 
-#: capeditor/blocks.py:162 capeditor/blocks.py:207
+#: capeditor/blocks.py:167 capeditor/blocks.py:212
 msgid ""
 "The paired values of points defining a polygon that delineates the affected "
 "area of the alert message"
 msgstr "የማንቂያ መልእክቱ የተጎዳውን አካባቢ የሚገልጽ ፖሊጎን የሚወስኑ ጥንድ ጥንድ እሴቶች"
 
-#: capeditor/blocks.py:165 capeditor/blocks.py:209 capeditor/blocks.py:260
-#: capeditor/blocks.py:297
+#: capeditor/blocks.py:170 capeditor/blocks.py:214 capeditor/blocks.py:265
+#: capeditor/blocks.py:302
 msgid "Altitude"
 msgstr "ከፍታ"
 
-#: capeditor/blocks.py:166 capeditor/blocks.py:210 capeditor/blocks.py:261
-#: capeditor/blocks.py:298
+#: capeditor/blocks.py:171 capeditor/blocks.py:215 capeditor/blocks.py:266
+#: capeditor/blocks.py:303
 msgid ""
 "The specific or minimum altitude of the affected area of the alert message"
 msgstr "የማስጠንቀቂያው መልእክት የተጎዳው አካባቢ ልዩ ወይም ዝቅተኛ ከፍታ"
 
-#: capeditor/blocks.py:168 capeditor/blocks.py:212 capeditor/blocks.py:263
-#: capeditor/blocks.py:300
+#: capeditor/blocks.py:173 capeditor/blocks.py:217 capeditor/blocks.py:268
+#: capeditor/blocks.py:305
 msgid "Ceiling"
 msgstr "ጣሪያ"
 
-#: capeditor/blocks.py:169 capeditor/blocks.py:213 capeditor/blocks.py:264
-#: capeditor/blocks.py:301
+#: capeditor/blocks.py:174 capeditor/blocks.py:218 capeditor/blocks.py:269
+#: capeditor/blocks.py:306
 msgid ""
 "The maximum altitude of the affected area of the alert message.MUST NOT be "
 "used except in combination with the altitude element. "
 msgstr ""
 "የማስጠንቀቂያ መልእክት የተጎዳው አካባቢ ከፍተኛው ከፍታ ከፍ ካለው ኤለመንት ጋር ካልተጣመረ በስተቀር ጥቅም ላይ መዋል "
 "የለበትም።"
 
-#: capeditor/blocks.py:206
+#: capeditor/blocks.py:211
 msgid "Polygon"
 msgstr "ፖሊጎን"
 
-#: capeditor/blocks.py:258 capeditor/blocks.py:528
+#: capeditor/blocks.py:263 capeditor/blocks.py:555
 msgid "Circle"
 msgstr "ክብ"
 
-#: capeditor/blocks.py:258
+#: capeditor/blocks.py:263
 msgid "Drag the marker to change position"
 msgstr "ቦታውን ለመቀየር ምልክት ማድረጊያውን ይጎትቱት።"
 
-#: capeditor/blocks.py:305
+#: capeditor/blocks.py:310
 msgid "The human-readable name of the agency or authority issuing this alert."
 msgstr "ይህን ማንቂያ የሚያወጣው ኤጀንሲ ወይም ባለስልጣን በሰው ሊነበብ የሚችል ስም።"
 
-#: capeditor/blocks.py:306
+#: capeditor/blocks.py:311
 msgid ""
 "The text describing the contact for follow-up and confirmation of the alert "
 "message"
 msgstr "ለመከታተል እና ለማንቂያ መልእክቱ ማረጋገጫ እውቂያውን የሚገልጽ ጽሑፍ"
 
-#: capeditor/blocks.py:307
+#: capeditor/blocks.py:312
 msgid "The text denoting the type of the subject event of the alert message"
 msgstr "የማንቂያ መልእክቱ የርዕሰ ጉዳይ ክስተት አይነትን የሚያመለክት ጽሑፍ"
 
-#: capeditor/blocks.py:308
+#: capeditor/blocks.py:313
 msgid "The text describing the intended audience of the alert message"
 msgstr "የማንቂያ መልእክቱ የታሰቡትን ታዳሚዎች የሚገልጽ ጽሑፍ"
 
-#: capeditor/blocks.py:350 capeditor/blocks.py:359
+#: capeditor/blocks.py:355 capeditor/blocks.py:364
 #, fuzzy
 #| msgid "Description"
 msgid "Resource Description"
 msgstr "የንብረት መግለጫ"
 
-#: capeditor/blocks.py:351 capeditor/blocks.py:360
+#: capeditor/blocks.py:356 capeditor/blocks.py:365
 msgid "The text describing the type and content of the resource file"
 msgstr "የመርጃ ፋይሉን ዓይነት እና ይዘት የሚገልጽ ጽሑፍ"
 
-#: capeditor/blocks.py:361
+#: capeditor/blocks.py:366
 #, fuzzy
 #| msgid "Alert Resources "
 msgid "External Resource Link"
 msgstr "የውጭ መገልገያ አገናኝ"
 
-#: capeditor/blocks.py:362
+#: capeditor/blocks.py:367
 msgid ""
 "Link to external resource. This can be for example a link to related "
 "websites. "
 msgstr "ወደ ውጫዊ ምንጭ አገናኝ. ይህ ለምሳሌ ወደ ተዛማጅ ድር ጣቢያዎች አገናኝ ሊሆን ይችላል."
 
-#: capeditor/blocks.py:370
+#: capeditor/blocks.py:375
 msgid "Name for the event code"
 msgstr "የክስተት ኮድ ስም"
 
-#: capeditor/blocks.py:371
+#: capeditor/blocks.py:376
 msgid "Value of the event code"
 msgstr "የክስተቱ ኮድ ዋጋ"
 
-#: capeditor/blocks.py:441
+#: capeditor/blocks.py:467
 msgid "English"
 msgstr "እንግሊዝኛ"
 
-#: capeditor/blocks.py:445
+#: capeditor/blocks.py:471
 msgid "Geophysical"
 msgstr "ጂኦፊዚካል"
 
-#: capeditor/blocks.py:446
+#: capeditor/blocks.py:472
 msgid "Meteorological"
 msgstr "ሜትሮሎጂ"
 
-#: capeditor/blocks.py:447
+#: capeditor/blocks.py:473
 msgid "General emergency and public safety"
 msgstr "አጠቃላይ ድንገተኛ እና የህዝብ ደህንነት"
 
-#: capeditor/blocks.py:448
+#: capeditor/blocks.py:474
 msgid "Law enforcement, military, homeland and local/private security"
 msgstr "የሕግ አስከባሪ፣ ወታደራዊ፣ የአገር ቤት እና የአካባቢ/የግል ደህንነት"
 
-#: capeditor/blocks.py:449
+#: capeditor/blocks.py:475
 msgid "Rescue and recovery"
 msgstr "ማዳን እና ማገገም"
 
-#: capeditor/blocks.py:450
+#: capeditor/blocks.py:476
 msgid "Fire suppression and rescue"
 msgstr "እሳትን ማዳን እና ማዳን"
 
-#: capeditor/blocks.py:451
+#: capeditor/blocks.py:477
 msgid "Medical and public health"
 msgstr "የሕክምና እና የህዝብ ጤና"
 
-#: capeditor/blocks.py:452
+#: capeditor/blocks.py:478
 msgid "Pollution and other environmental"
 msgstr "ብክለት እና ሌሎች አካባቢያዊ"
 
-#: capeditor/blocks.py:453
+#: capeditor/blocks.py:479
 msgid "Public and private transportation"
 msgstr "የህዝብ እና የግል መጓጓዣ"
 
-#: capeditor/blocks.py:454
+#: capeditor/blocks.py:480
 msgid "Utility, telecommunication, other non-transport infrastructure"
 msgstr "መገልገያ፣ ቴሌኮሙኒኬሽን፣ ሌሎች የትራንስፖርት ያልሆኑ መሠረተ ልማቶች"
 
-#: capeditor/blocks.py:455
+#: capeditor/blocks.py:481
 msgid ""
 "Chemical, Biological, Radiological, Nuclear or High-Yield Explosive threat "
 "or attack"
 msgstr "ኬሚካል፣ ባዮሎጂካል፣ ራዲዮሎጂካል፣ ኑክሌር ወይም ከፍተኛ ምርት የሚፈነዳ ዛቻ ወይም ጥቃት"
 
-#: capeditor/blocks.py:456
+#: capeditor/blocks.py:482
 msgid "Other events"
 msgstr "ሌሎች ክስተቶች"
 
-#: capeditor/blocks.py:460
+#: capeditor/blocks.py:486
 msgid "Immediate - Responsive action SHOULD be taken immediately"
 msgstr "ወዲያውኑ - ምላሽ ሰጪ እርምጃ ወዲያውኑ መወሰድ አለበት"
 
-#: capeditor/blocks.py:461
+#: capeditor/blocks.py:487
 msgid "Expected - Responsive action SHOULD be taken soon (within next hour)"
 msgstr "የሚጠበቀው - ምላሽ ሰጪ እርምጃ በቅርቡ መወሰድ አለበት (በሚቀጥለው ሰዓት ውስጥ)"
 
-#: capeditor/blocks.py:462
+#: capeditor/blocks.py:488
 msgid "Future - Responsive action SHOULD be taken in the near future"
 msgstr "ወደፊት - ምላሽ ሰጪ እርምጃ በቅርብ ጊዜ ውስጥ መወሰድ አለበት"
 
-#: capeditor/blocks.py:463
+#: capeditor/blocks.py:489
 msgid "Past - Responsive action is no longer required"
 msgstr "ያለፈው - ምላሽ ሰጪ እርምጃ ከአሁን በኋላ አያስፈልግም"
 
-#: capeditor/blocks.py:464
+#: capeditor/blocks.py:490
 msgid "Unknown - Urgency not known"
 msgstr "ያልታወቀ - አጣዳፊነት አይታወቅም"
 
-#: capeditor/blocks.py:468
+#: capeditor/blocks.py:494
 msgid "Extreme - Extraordinary threat to life or property"
 msgstr "እጅግ በጣም ከባድ - ለሕይወት ወይም ለንብረት ያልተለመደ ስጋት"
 
-#: capeditor/blocks.py:469
+#: capeditor/blocks.py:495
 msgid "Severe - Significant threat to life or property"
 msgstr "ከባድ - ለሕይወት ወይም ለንብረት ትልቅ ስጋት"
 
-#: capeditor/blocks.py:470
+#: capeditor/blocks.py:496
 msgid "Moderate - Possible threat to life or property"
 msgstr "መጠነኛ - በህይወት ወይም በንብረት ላይ ሊከሰት የሚችል ስጋት"
 
-#: capeditor/blocks.py:471
+#: capeditor/blocks.py:497
 msgid "Minor - Minimal to no known threat to life or property"
 msgstr "አናሳ - በህይወት ወይም በንብረት ላይ የማይታወቅ አነስተኛ ስጋት"
 
-#: capeditor/blocks.py:472
+#: capeditor/blocks.py:498
 msgid "Unknown - Severity unknown"
 msgstr "ያልታወቀ - ክብደት የማይታወቅ"
 
-#: capeditor/blocks.py:476
+#: capeditor/blocks.py:502
 msgid "Observed - Determined to have occurred or to be ongoing"
 msgstr "ታይቷል - ተከስቷል ወይም ቀጣይነት እንዲኖረው ተወስኗል"
 
-#: capeditor/blocks.py:477
+#: capeditor/blocks.py:503
 msgid "Likely - Likely (percentage > ~50%)"
 msgstr "ምናልባት - ምናልባት (መቶኛ > ~ 50%)"
 
-#: capeditor/blocks.py:478
+#: capeditor/blocks.py:504
 msgid "Possible - Possible but not likely (percentage <= ~50%)"
 msgstr "ይቻላል - ይቻላል ነገር ግን የማይሆን ​​(መቶኛ <= ~ 50%)"
 
-#: capeditor/blocks.py:479
+#: capeditor/blocks.py:505
 msgid "Unlikely - Not expected to occur (percentage ~ 0)"
 msgstr "የማይመስል - ይከሰታል ተብሎ አይጠበቅም (መቶኛ ~ 0)"
 
-#: capeditor/blocks.py:480
+#: capeditor/blocks.py:506
 msgid "Unknown - Certainty unknown"
 msgstr "ያልታወቀ - በእርግጠኝነት የማይታወቅ"
 
-#: capeditor/blocks.py:483
-msgid "Language"
-msgstr "ቋንቋ"
-
-#: capeditor/blocks.py:484
-msgid "The code denoting the language of the alert message"
-msgstr "የማስጠንቀቂያ መልእክት ቋንቋን የሚያመለክት ኮድ"
+#: capeditor/blocks.py:508
+msgid "Event"
+msgstr "ክስተት"
 
-#: capeditor/blocks.py:485
+#: capeditor/blocks.py:510
 msgid "Category"
 msgstr "ምድብ"
 
-#: capeditor/blocks.py:486
+#: capeditor/blocks.py:511
 msgid ""
 "The code denoting the category of the subject event of the alert message"
 msgstr "የማንቂያ መልእክቱ ርዕሰ ጉዳይ ክስተት ምድብን የሚያመለክት ኮድ"
 
-#: capeditor/blocks.py:488
-msgid "Event"
-msgstr "ክስተት"
+#: capeditor/blocks.py:513
+msgid "Language"
+msgstr "ቋንቋ"
 
-#: capeditor/blocks.py:489
+#: capeditor/blocks.py:514
+msgid "The code denoting the language of the alert message"
+msgstr "የማስጠንቀቂያ መልእክት ቋንቋን የሚያመለክት ኮድ"
+
+#: capeditor/blocks.py:516
 msgid "Urgency"
 msgstr "አስቸኳይ"
 
-#: capeditor/blocks.py:490
+#: capeditor/blocks.py:517
 msgid ""
 "The code denoting the urgency of the subject event of the alert message"
 msgstr "የማንቂያ መልእክቱ የርእሰ ጉዳይ ክስተት አጣዳፊነት የሚያመለክት ኮድ"
 
-#: capeditor/blocks.py:492
+#: capeditor/blocks.py:519
 msgid "Severity"
 msgstr "ከባድነት"
 
-#: capeditor/blocks.py:493
+#: capeditor/blocks.py:520
 msgid ""
 "The code denoting the severity of the subject event of the alert message"
 msgstr "የማንቂያ መልእክቱ የርዕሰ ጉዳይ ክስተት ክብደትን የሚያመለክት ኮድ"
 
-#: capeditor/blocks.py:495
+#: capeditor/blocks.py:522
 msgid "Certainty"
 msgstr "እርግጠኝነት"
 
-#: capeditor/blocks.py:496
+#: capeditor/blocks.py:523
 msgid ""
 "The code denoting the certainty of the subject event of the alert message"
 msgstr "የማንቂያ መልእክቱ ርዕሰ ጉዳይ ክስተት እርግጠኝነትን የሚያመለክት ኮድ"
 
-#: capeditor/blocks.py:498
+#: capeditor/blocks.py:525
 msgid "Headline"
 msgstr "ርዕስ"
 
-#: capeditor/blocks.py:499
+#: capeditor/blocks.py:526
 msgid ""
 "The text headline of the alert message. Make it direct and actionable as "
 "possible while remaining short"
 msgstr "የማንቂያ መልእክቱ የጽሑፍ ርዕስ። አጭር ሲቀሩ በተቻለ መጠን ቀጥተኛ እና ተግባራዊ ያድርጉት"
 
-#: capeditor/blocks.py:501
+#: capeditor/blocks.py:528
 msgid "Description"
 msgstr "መግለጫ"
 
-#: capeditor/blocks.py:503
+#: capeditor/blocks.py:530
 #, fuzzy
 #| msgid "The text describing the subject event of the alert message"
 msgid ""
 "The text describing the subject event of the alert message. An extended "
 "description of the hazard or event that occasioned this message"
 msgstr ""
-"የማንቂያ መልእክቱን ርዕሰ ጉዳይ ክስተት የሚገልጽ ጽሑፍ። ይህንን መልእክት ያስከተለው አደጋ ወይም ክስተት የተራዘመ "
+"የማንቂያ መልእክቱን ርዕሰ ጉዳይ ክስተት የሚገልጽ ጽሑፍ። ይህን መልእክት ያስከተለው አደጋ ወይም ክስተት የተራዘመ "
 "መግለጫ"
 
-#: capeditor/blocks.py:505
+#: capeditor/blocks.py:532
 msgid "Instruction"
 msgstr "መመሪያ"
 
-#: capeditor/blocks.py:506
+#: capeditor/blocks.py:533
 msgid ""
 "The text describing the recommended action to be taken by recipients of the "
 "alert message"
 msgstr "የማንቂያ መልእክቱ ተቀባዮች የሚመከር እርምጃን የሚገልጽ ጽሑፍ"
 
-#: capeditor/blocks.py:508
+#: capeditor/blocks.py:535
 msgid "Effective"
 msgstr "ውጤታማ"
 
-#: capeditor/blocks.py:509
+#: capeditor/blocks.py:536
 #, fuzzy
 #| msgid "The effective time of the information of the alert message"
 msgid ""
 "The effective time of the information of the alert message. If not set, the "
 "sent date will be used"
 msgstr "የማንቂያ መልእክት መረጃ ውጤታማ ጊዜ። ካልተዋቀረ የተላከው ቀን ስራ ላይ ይውላል"
 
-#: capeditor/blocks.py:511
+#: capeditor/blocks.py:538
 msgid "Onset"
 msgstr "ጅምር"
 
-#: capeditor/blocks.py:512
+#: capeditor/blocks.py:539
 msgid ""
 "The expected time of the beginning of the subject event of the alert message"
 msgstr "የማንቂያ መልእክቱ ርዕሰ ጉዳይ ክስተት የሚጠበቀው ጊዜ"
 
-#: capeditor/blocks.py:514
+#: capeditor/blocks.py:541
 msgid "Expires"
 msgstr "ጊዜው ያበቃል"
 
-#: capeditor/blocks.py:515
+#: capeditor/blocks.py:542
 msgid ""
 "The expiry time of the information of the alert message. If not set, each "
 "recipient is free to set its own policy as to when the message is no longer "
 "in effect."
 msgstr ""
 "የማንቂያ መልእክቱ መረጃ የሚያበቃበት ጊዜ። ካልተዋቀረ እያንዳንዱ ተቀባይ መልእክቱ መቼ እንደማይሰራ የራሱን ፖሊሲ "
 "ለማዘጋጀት ነፃ ነው።"
 
-#: capeditor/blocks.py:518
+#: capeditor/blocks.py:545
 #, fuzzy
 #| msgid "Response type"
 msgid "Response Types"
 msgstr "የምላሽ ዓይነቶች"
 
-#: capeditor/blocks.py:520
+#: capeditor/blocks.py:547
 #, fuzzy
 #| msgid "Sender"
 msgid "Sender name"
 msgstr "የላኪ ስም"
 
-#: capeditor/blocks.py:522
+#: capeditor/blocks.py:549
 msgid "Contact"
 msgstr "ተገናኝ"
 
-#: capeditor/blocks.py:523 capeditor/blocks.py:550
+#: capeditor/blocks.py:550 capeditor/blocks.py:580
 msgid "Audience"
 msgstr "ታዳሚዎች"
 
-#: capeditor/blocks.py:526
+#: capeditor/blocks.py:553
 msgid "Admin Boundary"
 msgstr "የአስተዳዳሪ ወሰን"
 
-#: capeditor/blocks.py:527
+#: capeditor/blocks.py:554
 msgid "Draw Polygon"
 msgstr "ፖሊጎን ይሳሉ"
 
-#: capeditor/blocks.py:529
+#: capeditor/blocks.py:556
 msgid "Geocode"
 msgstr "ጂኦኮድ"
 
-#: capeditor/blocks.py:530
+#: capeditor/blocks.py:557
 msgid "Alert Area"
 msgstr "ማንቂያ አካባቢ"
 
-#: capeditor/blocks.py:530
+#: capeditor/blocks.py:557
 msgid "Admin Boundary, Polygon, Circle or Geocode"
 msgstr "የአስተዳዳሪ ድንበር ፣ ፖሊጎን ፣ ክበብ ወይም ጂኦኮድ"
 
-#: capeditor/blocks.py:535
+#: capeditor/blocks.py:562
 #, fuzzy
 #| msgid "Resource"
 msgid "Resources"
 msgstr "መርጃዎች"
 
-#: capeditor/blocks.py:535
+#: capeditor/blocks.py:562
 msgid ""
 "Additional file with supplemental information related to this alert "
 "information"
 msgstr "ከዚህ የማንቂያ መረጃ ጋር የተያያዘ ተጨማሪ መረጃ ያለው ተጨማሪ ፋይል"
 
-#: capeditor/blocks.py:538
+#: capeditor/blocks.py:565
 msgid "Parameter"
 msgstr "መለኪያ"
 
-#: capeditor/blocks.py:538
+#: capeditor/blocks.py:565
 msgid "Parameters"
 msgstr "መለኪያዎች"
 
-#: capeditor/blocks.py:539
+#: capeditor/blocks.py:566
 #, fuzzy
 #| msgid "Event"
 msgid "Event Code"
 msgstr "የክስተት ኮድ"
 
-#: capeditor/blocks.py:539
+#: capeditor/blocks.py:566
 #, fuzzy
 #| msgid "Event"
 msgid "Event codes"
 msgstr "የክስተት ኮዶች"
 
-#: capeditor/blocks.py:545
+#: capeditor/blocks.py:575
 msgid "Hazard"
 msgstr "ሃዛርድ"
 
-#: capeditor/blocks.py:554
+#: capeditor/blocks.py:584
 #, fuzzy
 #| msgid "Contact"
 msgid "Contact Detail"
 msgstr "የእውቂያ ዝርዝር"
 
 #: capeditor/models.py:35
 #, fuzzy
@@ -600,15 +600,15 @@
 #, fuzzy
 #| msgid ""
 #| "Update - Updates and supercedes the earlier message(s) identified in "
 #| "referenced alerts"
 msgid ""
 "Update - Updates and supersedes the earlier message(s) identified in "
 "referenced alerts"
-msgstr "አዘምን - በተጠቀሱት ማንቂያዎች ውስጥ የተገለጸውን የቀደመ መልእክት(ዎች) ያዘምናል እና ይተካል።"
+msgstr "አዘምን - በተጠቀሱት ማንቂያዎች ውስጥ የተገለጸውን የቀደመ መልእክት(ዎች) ያሻሽላል እና ይተካል።"
 
 #: capeditor/models.py:184
 msgid "Cancel - Cancels the earlier message(s) identified in references"
 msgstr "ሰርዝ - በማጣቀሻዎች ውስጥ የተገለጸውን የቀደመ መልእክት(ዎች) ይሰርዛል"
 
 #: capeditor/models.py:185
 msgid ""
```

### Comparing `capeditor-0.2.7/capeditor/locale/ar/LC_MESSAGES/django.mo` & `capeditor-0.2.8/capeditor/locale/ar/LC_MESSAGES/django.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -9,95 +9,81 @@
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
 "&& n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 
 msgid ""
-" Identifies the originator of an alert. This can be an email of the "
-"institution for example"
-msgstr ""
-"يحدد منشئ التنبيه. يمكن أن يكون هذا بريدًا إلكترونيًا للمؤسسة على سبيل المثال"
-
-msgid ""
 "Acknowledge - Acknowledges receipt and acceptance of the message(s) "
 "identified in references field"
 msgstr "إقرار - يقر باستلام وقبول الرسالة (الرسائل) المحددة في حقل المراجع"
 
 msgid "Actual - Actionable by all targeted recipients"
 msgstr "فعلي - قابل للتنفيذ من قبل جميع المستفيدين المستهدفين"
 
+msgid ""
+"Additional file with supplemental information related to this alert "
+"information"
+msgstr "ملف إضافي بمعلومات تكميلية متعلقة بمعلومات التنبيه هذه"
+
+msgid "Addresses"
+msgstr "عناوين"
+
+msgid "Admin Boundary"
+msgstr "حدود الإدارة"
+
+msgid "Admin Boundary, Polygon, Circle or Geocode"
+msgstr "حدود الإدارة أو المضلع أو الدائرة أو الرمز الجغرافي"
+
+msgid "Administrative Level"
+msgstr "المستوى الإداري"
+
 msgid "Affected areas / Regions"
 msgstr "المناطق / المناطق المتضررة"
 
-msgid "Alert"
-msgstr "يُحذًِر"
-
 msgid "Alert - Initial information requiring attention by targeted recipients"
 msgstr "تنبيه - معلومات أولية تتطلب اهتمام المستلمين المستهدفين"
 
 msgid "Alert Area"
 msgstr "منطقة التنبيه"
 
-msgid "Alert Areas "
-msgstr "مناطق التنبيه"
-
-msgid ""
-"Alert Categorization (Category, Urgency, Severity, Certainity, Response & "
-"Dates)"
-msgstr ""
-"تصنيف التنبيه (الفئة ، الاستعجال ، الخطورة ، اليقين ، الاستجابة والتواريخ)"
-
-msgid ""
-"Alert Delivery Message (Headline, Description, Intsructions, Contact & "
-"Website)"
-msgstr ""
-"رسالة تسليم التنبيه (العنوان ، الوصف ، التعليمات ، جهة الاتصال والموقع "
-"الإلكتروني)"
-
-msgid "Alert Identification (Sender, Message Type, Scope)"
-msgstr "تعريف التنبيه (المرسل ، نوع الرسالة ، النطاق)"
-
-msgid "Alert Info"
-msgstr "معلومات التنبيه"
-
 msgid "Alert Information"
 msgstr "معلومات التنبيه"
 
-msgid "Alert Resources "
-msgstr "موارد التنبيه"
-
-msgid "Alerts Per Page"
-msgstr "تنبيهات لكل صفحة"
-
 msgid ""
 "All Clear - The subject event no longer poses a threat or concern and any "
 "follow on action is described in instruction"
 msgstr ""
 "الكل واضح - لم يعد حدث الموضوع يمثل تهديدًا أو قلقًا وأي متابعة للإجراء موصوف "
 "في التعليمات"
 
 msgid "Altitude"
 msgstr "ارتفاع"
 
-msgid "Area"
-msgstr "منطقة"
-
 msgid ""
 "Assess - Evaluate the information in this message - DONT USE FOR PUBLIC "
 "ALERTS"
 msgstr ""
 "قيم - قيم المعلومات الواردة في هذه الرسالة - لا تستخدم في التنبيهات العامة"
 
 msgid "Audience"
 msgstr "جمهور"
 
 msgid "Avoid - Avoid the subject event as per the instruction"
 msgstr "تجنب - تجنب موضوع الحدث حسب التعليمات"
 
+msgid "Boundary"
+msgstr "الحدود"
+
+msgid "CAP Sender Name"
+msgstr "اسم مرسل CAP"
+
+msgid "Can be the website link or email of the sending institution"
+msgstr "يمكن أن يكون رابط موقع الويب أو البريد الإلكتروني للمؤسسة المرسلة"
+
 msgid "Cancel - Cancels the earlier message(s) identified in references"
 msgstr "إلغاء - يلغي الرسالة (الرسائل) السابقة المحددة في المراجع"
 
 msgid "Category"
 msgstr "فئة"
 
 msgid "Ceiling"
@@ -109,45 +95,42 @@
 msgid ""
 "Chemical, Biological, Radiological, Nuclear or High-Yield Explosive threat "
 "or attack"
 msgstr ""
 "التهديد أو الهجوم الكيميائي أو البيولوجي أو الإشعاعي أو النووي أو بالمتفجرات "
 "عالية الإنتاجية"
 
+msgid "Circle"
+msgstr "دائرة"
+
 msgid "Code"
 msgstr "شفرة"
 
 msgid "Contact"
 msgstr "اتصال"
 
 msgid "Description"
 msgstr "وصف"
 
-msgid "Description of the incident"
-msgstr "وصف الحادث"
-
 msgid ""
 "Draft - A preliminary template or draft, not actionable in its current form"
 msgstr "مسودة - نموذج أو مسودة أولية ، غير قابلة للتنفيذ في شكلها الحالي"
 
-msgid "Earlier Reference Alerts -  If applicable"
-msgstr "تنبيهات مرجعية سابقة - إن وجدت"
+msgid "Drag the marker to change position"
+msgstr "اسحب العلامة لتغيير الموضع"
+
+msgid "Draw Polygon"
+msgstr "ارسم مضلع"
 
 msgid "Earlier alert referenced by this alert"
 msgstr "التنبيه السابق المشار إليه في هذا التنبيه"
 
 msgid "Effective"
 msgstr "فعال"
 
-msgid "Email"
-msgstr "بريد إلكتروني"
-
-msgid "Email address"
-msgstr "عنوان البريد الإلكتروني"
-
 msgid "English"
 msgstr "إنجليزي"
 
 msgid ""
 "Error -  Indicates rejection of the message(s) identified in references; "
 "explanation SHOULD appear in note field"
 msgstr ""
@@ -166,82 +149,77 @@
 msgid ""
 "Exercise - Actionable only by designated exercise participants; exercise "
 "identifier SHOULD appear in note"
 msgstr ""
 "التمرين - قابل للتنفيذ فقط بواسطة مشاركين معينين في التمرين ؛ يجب أن يظهر "
 "معرف التمرين في الملاحظة"
 
-msgid "Expected"
-msgstr "مُتوقع"
-
 msgid "Expected - Responsive action SHOULD be taken soon (within next hour)"
 msgstr "متوقع - يجب اتخاذ إجراء مستجيب قريبًا (خلال الساعة القادمة)"
 
 msgid "Expires"
 msgstr "تنتهي"
 
 msgid "Extreme - Extraordinary threat to life or property"
 msgstr "شديد - تهديد غير عادي للحياة أو الممتلكات"
 
-msgid "File"
-msgstr "ملف"
-
-msgid "File, Document etc"
-msgstr "ملف ، وثيقة إلخ"
-
 msgid "Fire suppression and rescue"
 msgstr "إخماد الحرائق والإنقاذ"
 
-msgid "Future"
-msgstr "مستقبل"
-
 msgid "Future - Responsive action SHOULD be taken in the near future"
 msgstr "المستقبل - يجب اتخاذ إجراءات استجابة في المستقبل القريب"
 
 msgid "General emergency and public safety"
 msgstr "الطوارئ العامة والسلامة العامة"
 
+msgid "Geocode"
+msgstr "تكويد جغرافيًا"
+
 msgid "Geophysical"
 msgstr "الجيوفيزيائية"
 
+msgid "Hazard"
+msgstr "خطر"
+
+msgid "Hazards monitored by the institution"
+msgstr "الأخطار التي ترصدها المؤسسة"
+
 msgid "Headline"
 msgstr "العنوان"
 
-msgid ""
-"How many of this products should be visible on the landing page filter "
-"section ?"
-msgstr ""
-"كم عدد هذه المنتجات التي يجب أن تكون مرئية في قسم مرشح الصفحة المقصودة؟"
-
 msgid "Identifier"
 msgstr "المعرف"
 
-msgid "Immediate"
-msgstr "مباشر"
-
 msgid "Immediate - Responsive action SHOULD be taken immediately"
 msgstr "فوري - يجب اتخاذ إجراء مستجيب على الفور"
 
+msgid "Incident"
+msgstr "حادثة"
+
+msgid "Incidents"
+msgstr "الحوادث"
+
 msgid "Instruction"
 msgstr "تعليمات"
 
-msgid "Intended Recipients (If scope is Private) "
-msgstr "المستلمون المقصودون (إذا كان النطاق خاصًا)"
-
 msgid "Language"
 msgstr "لغة"
 
 msgid "Law enforcement, military, homeland and local/private security"
 msgstr "إنفاذ القانون والجيش والوطن والأمن المحلي / الخاص"
 
 msgid "Likely - Likely (percentage > ~50%)"
 msgstr "مرجح - مرجح (نسبة مئوية> ~ 50٪)"
 
-msgid "Link"
-msgstr "وصلة"
+msgid ""
+"Link to external resource. This can be for example a link to related "
+"websites. "
+msgstr ""
+"ارتباط بمورد خارجي. يمكن أن يكون هذا على سبيل المثال رابطًا إلى مواقع الويب "
+"ذات الصلة."
 
 msgid "Medical and public health"
 msgstr "الطب والصحة العامة"
 
 msgid "Message Type"
 msgstr "نوع الرسالة"
 
@@ -259,17 +237,14 @@
 
 msgid "Name"
 msgstr "اسم"
 
 msgid "Name for the event code"
 msgstr "اسم رمز الحدث"
 
-msgid "Name for the geocode"
-msgstr "اسم الكود الجغرافي"
-
 msgid "Name of the recipient"
 msgstr "اسم المستلم"
 
 msgid "No action recommended"
 msgstr "لا يوجد إجراء موصى به"
 
 msgid "Note"
@@ -280,23 +255,29 @@
 
 msgid "Onset"
 msgstr "بداية"
 
 msgid "Other events"
 msgstr "أحداث أخرى"
 
-msgid "Past"
-msgstr "ماضي"
+msgid "Parameter"
+msgstr "معامل"
+
+msgid "Parameters"
+msgstr "حدود"
 
 msgid "Past - Responsive action is no longer required"
 msgstr "الماضي - لم يعد الإجراء المستجيب مطلوبًا"
 
 msgid "Pollution and other environmental"
 msgstr "التلوث والبيئية الأخرى"
 
+msgid "Polygon"
+msgstr "مضلع"
+
 msgid "Possible - Possible but not likely (percentage <= ~50%)"
 msgstr "ممكن - ممكن لكن غير محتمل (النسبة المئوية <= ~ 50٪)"
 
 msgid "Prepare - Relocate as instructed in the instruction"
 msgstr "الاستعداد - الانتقال كما هو موضح في التعليمات"
 
 msgid ""
@@ -316,20 +297,14 @@
 
 msgid "Reference Alert"
 msgstr "تنبيه مرجعي"
 
 msgid "Rescue and recovery"
 msgstr "الإنقاذ والإنعاش"
 
-msgid "Resource"
-msgstr "الموارد"
-
-msgid "Resource type whether is image, file etc"
-msgstr "نوع المورد سواء كان صورة أو ملف وما إلى ذلك"
-
 msgid "Response type"
 msgstr "نوع الاستجابة"
 
 msgid ""
 "Restricted - For dissemination only to users with a known operational "
 "requirement as in the restriction field"
 msgstr ""
@@ -362,20 +337,20 @@
 
 msgid "Status"
 msgstr "حالة"
 
 msgid "System - For messages that support alert network internal functions"
 msgstr "النظام - للرسائل التي تدعم وظائف شبكة التنبيه الداخلية"
 
+msgid "Target audiences for published alerts"
+msgstr "استهداف الجماهير للتنبيهات المنشورة"
+
 msgid "Test - Technical testing only, all recipients disregard"
 msgstr "الاختبار - الاختبار الفني فقط ، يتجاهل جميع المتلقين"
 
-msgid "The base-64 encoded data content of the resource file"
-msgstr "محتوى البيانات المشفرة base-64 لملف المورد"
-
 msgid "The code denoting the appropriate handling of the alert"
 msgstr "الرمز الذي يشير إلى المعالجة المناسبة للتنبيه"
 
 msgid ""
 "The code denoting the category of the subject event of the alert message"
 msgstr "الرمز الذي يشير إلى فئة موضوع الحدث لرسالة التنبيه"
 
@@ -403,35 +378,27 @@
 "The code denoting the type of action recommended for the target audience"
 msgstr "الرمز الذي يشير إلى نوع الإجراء الموصى به للجمهور المستهدف"
 
 msgid "The code denoting the urgency of the subject event of the alert message"
 msgstr "رمز يشير إلى إلحاح موضوع الحدث لرسالة التنبيه"
 
 msgid ""
-"The code representing the digital digest ('hash') computed from the resource "
-"file"
-msgstr "الكود الذي يمثل الملخص الرقمي (\"التجزئة\") المحسوب من ملف المصدر"
-
-msgid "The effective time of the information of the alert message"
-msgstr "الوقت الفعلي لمعلومات رسالة التنبيه"
-
-msgid ""
 "The expected time of the beginning of the subject event of the alert message"
 msgstr "الوقت المتوقع لبداية موضوع الحدث لرسالة التنبيه"
 
-msgid "The expiry time of the information of the alert message"
-msgstr "وقت انتهاء صلاحية معلومات رسالة التنبيه"
-
 msgid ""
-"The identifier of the hyperlink associating additional information with the "
-"alert message"
-msgstr "معرّف الارتباط التشعبي الذي يربط معلومات إضافية برسالة التنبيه"
+"The expiry time of the information of the alert message. If not set, each "
+"recipient is free to set its own policy as to when the message is no longer "
+"in effect."
+msgstr ""
+"وقت انتهاء صلاحية معلومات رسالة التنبيه. في حالة عدم التعيين ، يكون لكل "
+"مستلم الحرية في تعيين سياسته الخاصة عندما لا تكون الرسالة سارية المفعول."
 
-msgid "The identifier of the hyperlink for the resource file"
-msgstr "معرّف الارتباط التشعبي لملف المورد"
+msgid "The human-readable name of the agency or authority issuing this alert."
+msgstr "الاسم الذي يمكن للبشر قراءته للوكالة أو السلطة التي أصدرت هذا التنبيه."
 
 msgid ""
 "The maximum altitude of the affected area of the alert message.MUST NOT be "
 "used except in combination with the altitude element. "
 msgstr ""
 "أقصى ارتفاع للمنطقة المتأثرة برسالة التنبيه. يجب عدم استخدامه إلا بالاقتران "
 "مع عنصر الارتفاع."
@@ -477,72 +444,51 @@
 msgid ""
 "The text describing the rule for limiting distribution of the restricted "
 "alert message. Used when scope value is Restricted"
 msgstr ""
 "النص الذي يصف القاعدة للحد من توزيع رسالة التنبيه المقيدة. يُستخدم عندما تكون "
 "قيمة النطاق مقيدة"
 
-msgid "The text describing the subject event of the alert message"
-msgstr "النص الذي يصف الحدث الموضوع لرسالة التنبيه"
-
 msgid "The text describing the type and content of the resource file"
 msgstr "النص الذي يصف نوع ومحتوى ملف المصدر"
 
-msgid "The text headline of the alert message"
-msgstr "العنوان النصي لرسالة التنبيه"
+msgid ""
+"The text headline of the alert message. Make it direct and actionable as "
+"possible while remaining short"
+msgstr ""
+"العنوان النصي لرسالة التنبيه. اجعلها مباشرة وقابلة للتنفيذ قدر الإمكان مع "
+"البقاء قصيرًا"
 
 msgid "The text identifying the source of the alert message"
 msgstr "النص الذي يحدد مصدر رسالة التنبيه"
 
 msgid "Time and date of origination of the alert"
 msgstr "وقت وتاريخ إصدار التنبيه"
 
-msgid "Title"
-msgstr "عنوان"
-
-msgid "Title of the incident referent of the alert"
-msgstr "عنوان الحادث المشار إليه في التنبيه"
-
 msgid "Unique ID. Auto generated on creation."
 msgstr "معرف فريد. تم إنشاؤه تلقائيًا عند الإنشاء."
 
-msgid "Unknown"
-msgstr "مجهول"
-
 msgid "Unknown - Certainty unknown"
 msgstr "غير معروف - اليقين غير معروف"
 
 msgid "Unknown - Severity unknown"
 msgstr "غير معروف - الخطورة غير معروفة"
 
 msgid "Unknown - Urgency not known"
 msgstr "غير معروف - الاستعجال غير معروف"
 
 msgid "Unlikely - Not expected to occur (percentage ~ 0)"
 msgstr "غير محتمل - غير متوقع حدوثه (النسبة المئوية ~ 0)"
 
-msgid ""
-"Update - Updates and supercedes the earlier message(s) identified in "
-"referenced alerts"
-msgstr ""
-"تحديث - يحدّث ويحل محل الرسالة (الرسائل) السابقة المحددة في التنبيهات المشار "
-"إليها"
-
 msgid "Urgency"
 msgstr "الاستعجال"
 
 msgid "Utility, telecommunication, other non-transport infrastructure"
 msgstr ""
 "المرافق والاتصالات السلكية واللاسلكية والبنية التحتية الأخرى غير المتعلقة "
 "بالنقل"
 
 msgid "Value"
 msgstr "قيمة"
 
 msgid "Value of the event code"
 msgstr "قيمة رمز الحدث"
-
-msgid "Value of the geocode"
-msgstr "قيمة الكود الجغرافي"
-
-msgid "Web"
-msgstr "الويب"
```

### Comparing `capeditor-0.2.7/capeditor/locale/ar/LC_MESSAGES/django.po` & `capeditor-0.2.8/capeditor/locale/ar/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-12 14:01+0300\n"
+"POT-Creation-Date: 2023-07-14 12:05+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 && n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 
-#: capeditor/blocks.py:70 capeditor/blocks.py:98 capeditor/blocks.py:370
+#: capeditor/blocks.py:70 capeditor/blocks.py:98 capeditor/blocks.py:375
 msgid "Name"
 msgstr "اسم"
 
 #: capeditor/blocks.py:70
 msgid "Name of the recipient"
 msgstr "اسم المستلم"
 
@@ -52,15 +52,15 @@
 
 #: capeditor/blocks.py:94
 #, fuzzy
 #| msgid "The text headline of the alert message"
 msgid "Referent incident to this alert message"
 msgstr "إحالة الحادث إلى رسالة التنبيه هذه"
 
-#: capeditor/blocks.py:99 capeditor/blocks.py:295 capeditor/blocks.py:371
+#: capeditor/blocks.py:99 capeditor/blocks.py:300 capeditor/blocks.py:376
 msgid "Value"
 msgstr "قيمة"
 
 #: capeditor/blocks.py:104
 msgid "Shelter - Take shelter in place or per instruction"
 msgstr "المأوى - احتمي في المكان أو حسب التعليمات"
 
@@ -108,444 +108,444 @@
 msgstr "نوع الاستجابة"
 
 #: capeditor/blocks.py:117
 msgid ""
 "The code denoting the type of action recommended for the target audience"
 msgstr "الرمز الذي يشير إلى نوع الإجراء الموصى به للجمهور المستهدف"
 
-#: capeditor/blocks.py:158 capeditor/blocks.py:204 capeditor/blocks.py:256
-#: capeditor/blocks.py:292
+#: capeditor/blocks.py:163 capeditor/blocks.py:209 capeditor/blocks.py:261
+#: capeditor/blocks.py:297
 msgid "Affected areas / Regions"
 msgstr "المناطق / المناطق المتضررة"
 
-#: capeditor/blocks.py:159 capeditor/blocks.py:205 capeditor/blocks.py:257
-#: capeditor/blocks.py:293
+#: capeditor/blocks.py:164 capeditor/blocks.py:210 capeditor/blocks.py:262
+#: capeditor/blocks.py:298
 msgid "The text describing the affected area of the alert message"
 msgstr "النص الذي يصف المنطقة المتأثرة برسالة التنبيه"
 
-#: capeditor/blocks.py:160
+#: capeditor/blocks.py:165
 msgid "Administrative Level"
 msgstr "المستوى الإداري"
 
-#: capeditor/blocks.py:161
+#: capeditor/blocks.py:166
 msgid "Boundary"
 msgstr "الحدود"
 
-#: capeditor/blocks.py:162 capeditor/blocks.py:207
+#: capeditor/blocks.py:167 capeditor/blocks.py:212
 msgid ""
 "The paired values of points defining a polygon that delineates the affected "
 "area of the alert message"
 msgstr ""
 "القيم المزدوجة للنقاط التي تحدد مضلعًا يحدد المنطقة المتأثرة من رسالة "
 "التنبيه"
 
-#: capeditor/blocks.py:165 capeditor/blocks.py:209 capeditor/blocks.py:260
-#: capeditor/blocks.py:297
+#: capeditor/blocks.py:170 capeditor/blocks.py:214 capeditor/blocks.py:265
+#: capeditor/blocks.py:302
 msgid "Altitude"
 msgstr "ارتفاع"
 
-#: capeditor/blocks.py:166 capeditor/blocks.py:210 capeditor/blocks.py:261
-#: capeditor/blocks.py:298
+#: capeditor/blocks.py:171 capeditor/blocks.py:215 capeditor/blocks.py:266
+#: capeditor/blocks.py:303
 msgid ""
 "The specific or minimum altitude of the affected area of the alert message"
 msgstr "الارتفاع المحدد أو الأدنى للمنطقة المتأثرة برسالة التنبيه"
 
-#: capeditor/blocks.py:168 capeditor/blocks.py:212 capeditor/blocks.py:263
-#: capeditor/blocks.py:300
+#: capeditor/blocks.py:173 capeditor/blocks.py:217 capeditor/blocks.py:268
+#: capeditor/blocks.py:305
 msgid "Ceiling"
 msgstr "سقف"
 
-#: capeditor/blocks.py:169 capeditor/blocks.py:213 capeditor/blocks.py:264
-#: capeditor/blocks.py:301
+#: capeditor/blocks.py:174 capeditor/blocks.py:218 capeditor/blocks.py:269
+#: capeditor/blocks.py:306
 msgid ""
 "The maximum altitude of the affected area of the alert message.MUST NOT be "
 "used except in combination with the altitude element. "
 msgstr ""
 "أقصى ارتفاع للمنطقة المتأثرة برسالة التنبيه. يجب عدم استخدامه إلا بالاقتران "
 "مع عنصر الارتفاع."
 
-#: capeditor/blocks.py:206
+#: capeditor/blocks.py:211
 msgid "Polygon"
 msgstr "مضلع"
 
-#: capeditor/blocks.py:258 capeditor/blocks.py:528
+#: capeditor/blocks.py:263 capeditor/blocks.py:555
 msgid "Circle"
 msgstr "دائرة"
 
-#: capeditor/blocks.py:258
+#: capeditor/blocks.py:263
 msgid "Drag the marker to change position"
 msgstr "اسحب العلامة لتغيير الموضع"
 
-#: capeditor/blocks.py:305
+#: capeditor/blocks.py:310
 msgid "The human-readable name of the agency or authority issuing this alert."
 msgstr ""
 "الاسم الذي يمكن للبشر قراءته للوكالة أو السلطة التي أصدرت هذا التنبيه."
 
-#: capeditor/blocks.py:306
+#: capeditor/blocks.py:311
 msgid ""
 "The text describing the contact for follow-up and confirmation of the alert "
 "message"
 msgstr "النص الذي يصف جهة الاتصال للمتابعة وتأكيد رسالة التنبيه"
 
-#: capeditor/blocks.py:307
+#: capeditor/blocks.py:312
 msgid "The text denoting the type of the subject event of the alert message"
 msgstr "النص الذي يشير إلى نوع الحدث الموضوع لرسالة التنبيه"
 
-#: capeditor/blocks.py:308
+#: capeditor/blocks.py:313
 msgid "The text describing the intended audience of the alert message"
 msgstr "النص الذي يصف الجمهور المستهدف لرسالة التنبيه"
 
-#: capeditor/blocks.py:350 capeditor/blocks.py:359
+#: capeditor/blocks.py:355 capeditor/blocks.py:364
 #, fuzzy
 #| msgid "Description"
 msgid "Resource Description"
 msgstr "وصف المورد"
 
-#: capeditor/blocks.py:351 capeditor/blocks.py:360
+#: capeditor/blocks.py:356 capeditor/blocks.py:365
 msgid "The text describing the type and content of the resource file"
 msgstr "النص الذي يصف نوع ومحتوى ملف المصدر"
 
-#: capeditor/blocks.py:361
+#: capeditor/blocks.py:366
 #, fuzzy
 #| msgid "Alert Resources "
 msgid "External Resource Link"
 msgstr "رابط الموارد الخارجية"
 
-#: capeditor/blocks.py:362
+#: capeditor/blocks.py:367
 msgid ""
 "Link to external resource. This can be for example a link to related "
 "websites. "
 msgstr ""
 "ارتباط بمورد خارجي. يمكن أن يكون هذا على سبيل المثال رابطًا إلى مواقع الويب "
 "ذات الصلة."
 
-#: capeditor/blocks.py:370
+#: capeditor/blocks.py:375
 msgid "Name for the event code"
 msgstr "اسم رمز الحدث"
 
-#: capeditor/blocks.py:371
+#: capeditor/blocks.py:376
 msgid "Value of the event code"
 msgstr "قيمة رمز الحدث"
 
-#: capeditor/blocks.py:441
+#: capeditor/blocks.py:467
 msgid "English"
 msgstr "إنجليزي"
 
-#: capeditor/blocks.py:445
+#: capeditor/blocks.py:471
 msgid "Geophysical"
 msgstr "الجيوفيزيائية"
 
-#: capeditor/blocks.py:446
+#: capeditor/blocks.py:472
 msgid "Meteorological"
 msgstr "الأرصاد الجوية"
 
-#: capeditor/blocks.py:447
+#: capeditor/blocks.py:473
 msgid "General emergency and public safety"
 msgstr "الطوارئ العامة والسلامة العامة"
 
-#: capeditor/blocks.py:448
+#: capeditor/blocks.py:474
 msgid "Law enforcement, military, homeland and local/private security"
 msgstr "إنفاذ القانون والجيش والوطن والأمن المحلي / الخاص"
 
-#: capeditor/blocks.py:449
+#: capeditor/blocks.py:475
 msgid "Rescue and recovery"
 msgstr "الإنقاذ والإنعاش"
 
-#: capeditor/blocks.py:450
+#: capeditor/blocks.py:476
 msgid "Fire suppression and rescue"
 msgstr "إخماد الحرائق والإنقاذ"
 
-#: capeditor/blocks.py:451
+#: capeditor/blocks.py:477
 msgid "Medical and public health"
 msgstr "الطب والصحة العامة"
 
-#: capeditor/blocks.py:452
+#: capeditor/blocks.py:478
 msgid "Pollution and other environmental"
 msgstr "التلوث والبيئية الأخرى"
 
-#: capeditor/blocks.py:453
+#: capeditor/blocks.py:479
 msgid "Public and private transportation"
 msgstr "المواصلات العامة والخاصة"
 
-#: capeditor/blocks.py:454
+#: capeditor/blocks.py:480
 msgid "Utility, telecommunication, other non-transport infrastructure"
 msgstr ""
 "المرافق والاتصالات السلكية واللاسلكية والبنية التحتية الأخرى غير المتعلقة "
 "بالنقل"
 
-#: capeditor/blocks.py:455
+#: capeditor/blocks.py:481
 msgid ""
 "Chemical, Biological, Radiological, Nuclear or High-Yield Explosive threat "
 "or attack"
 msgstr ""
 "التهديد أو الهجوم الكيميائي أو البيولوجي أو الإشعاعي أو النووي أو بالمتفجرات"
 " عالية الإنتاجية"
 
-#: capeditor/blocks.py:456
+#: capeditor/blocks.py:482
 msgid "Other events"
 msgstr "أحداث أخرى"
 
-#: capeditor/blocks.py:460
+#: capeditor/blocks.py:486
 msgid "Immediate - Responsive action SHOULD be taken immediately"
 msgstr "فوري - يجب اتخاذ إجراء مستجيب على الفور"
 
-#: capeditor/blocks.py:461
+#: capeditor/blocks.py:487
 msgid "Expected - Responsive action SHOULD be taken soon (within next hour)"
 msgstr "متوقع - يجب اتخاذ إجراء مستجيب قريبًا (خلال الساعة القادمة)"
 
-#: capeditor/blocks.py:462
+#: capeditor/blocks.py:488
 msgid "Future - Responsive action SHOULD be taken in the near future"
 msgstr "المستقبل - يجب اتخاذ إجراءات استجابة في المستقبل القريب"
 
-#: capeditor/blocks.py:463
+#: capeditor/blocks.py:489
 msgid "Past - Responsive action is no longer required"
 msgstr "الماضي - لم يعد الإجراء المستجيب مطلوبًا"
 
-#: capeditor/blocks.py:464
+#: capeditor/blocks.py:490
 msgid "Unknown - Urgency not known"
 msgstr "غير معروف - الاستعجال غير معروف"
 
-#: capeditor/blocks.py:468
+#: capeditor/blocks.py:494
 msgid "Extreme - Extraordinary threat to life or property"
 msgstr "شديد - تهديد غير عادي للحياة أو الممتلكات"
 
-#: capeditor/blocks.py:469
+#: capeditor/blocks.py:495
 msgid "Severe - Significant threat to life or property"
 msgstr "خطير - تهديد خطير للحياة أو الممتلكات"
 
-#: capeditor/blocks.py:470
+#: capeditor/blocks.py:496
 msgid "Moderate - Possible threat to life or property"
 msgstr "معتدل - تهديد محتمل للحياة أو الممتلكات"
 
-#: capeditor/blocks.py:471
+#: capeditor/blocks.py:497
 msgid "Minor - Minimal to no known threat to life or property"
 msgstr "طفيف - من الحد الأدنى إلى عدم وجود تهديد معروف للحياة أو الممتلكات"
 
-#: capeditor/blocks.py:472
+#: capeditor/blocks.py:498
 msgid "Unknown - Severity unknown"
 msgstr "غير معروف - الخطورة غير معروفة"
 
-#: capeditor/blocks.py:476
+#: capeditor/blocks.py:502
 msgid "Observed - Determined to have occurred or to be ongoing"
 msgstr "تمت ملاحظته - تم العزم على حدوثه أو استمراره"
 
-#: capeditor/blocks.py:477
+#: capeditor/blocks.py:503
 msgid "Likely - Likely (percentage > ~50%)"
 msgstr "مرجح - مرجح (نسبة مئوية> ~ 50٪)"
 
-#: capeditor/blocks.py:478
+#: capeditor/blocks.py:504
 msgid "Possible - Possible but not likely (percentage <= ~50%)"
 msgstr "ممكن - ممكن لكن غير محتمل (النسبة المئوية <= ~ 50٪)"
 
-#: capeditor/blocks.py:479
+#: capeditor/blocks.py:505
 msgid "Unlikely - Not expected to occur (percentage ~ 0)"
 msgstr "غير محتمل - غير متوقع حدوثه (النسبة المئوية ~ 0)"
 
-#: capeditor/blocks.py:480
+#: capeditor/blocks.py:506
 msgid "Unknown - Certainty unknown"
 msgstr "غير معروف - اليقين غير معروف"
 
-#: capeditor/blocks.py:483
-msgid "Language"
-msgstr "لغة"
-
-#: capeditor/blocks.py:484
-msgid "The code denoting the language of the alert message"
-msgstr "الرمز الذي يشير إلى لغة رسالة التنبيه"
+#: capeditor/blocks.py:508
+msgid "Event"
+msgstr "حدث"
 
-#: capeditor/blocks.py:485
+#: capeditor/blocks.py:510
 msgid "Category"
 msgstr "فئة"
 
-#: capeditor/blocks.py:486
+#: capeditor/blocks.py:511
 msgid ""
 "The code denoting the category of the subject event of the alert message"
 msgstr "الرمز الذي يشير إلى فئة موضوع الحدث لرسالة التنبيه"
 
-#: capeditor/blocks.py:488
-msgid "Event"
-msgstr "حدث"
+#: capeditor/blocks.py:513
+msgid "Language"
+msgstr "لغة"
 
-#: capeditor/blocks.py:489
+#: capeditor/blocks.py:514
+msgid "The code denoting the language of the alert message"
+msgstr "الرمز الذي يشير إلى لغة رسالة التنبيه"
+
+#: capeditor/blocks.py:516
 msgid "Urgency"
 msgstr "الاستعجال"
 
-#: capeditor/blocks.py:490
+#: capeditor/blocks.py:517
 msgid ""
 "The code denoting the urgency of the subject event of the alert message"
 msgstr "رمز يشير إلى إلحاح موضوع الحدث لرسالة التنبيه"
 
-#: capeditor/blocks.py:492
+#: capeditor/blocks.py:519
 msgid "Severity"
 msgstr "خطورة"
 
-#: capeditor/blocks.py:493
+#: capeditor/blocks.py:520
 msgid ""
 "The code denoting the severity of the subject event of the alert message"
 msgstr "رمز يدل على خطورة الحدث موضوع رسالة التنبيه"
 
-#: capeditor/blocks.py:495
+#: capeditor/blocks.py:522
 msgid "Certainty"
 msgstr "بالتاكيد"
 
-#: capeditor/blocks.py:496
+#: capeditor/blocks.py:523
 msgid ""
 "The code denoting the certainty of the subject event of the alert message"
 msgstr "الرمز الذي يشير إلى يقين موضوع الحدث لرسالة التنبيه"
 
-#: capeditor/blocks.py:498
+#: capeditor/blocks.py:525
 msgid "Headline"
 msgstr "العنوان"
 
-#: capeditor/blocks.py:499
+#: capeditor/blocks.py:526
 msgid ""
 "The text headline of the alert message. Make it direct and actionable as "
 "possible while remaining short"
 msgstr ""
 "العنوان النصي لرسالة التنبيه. اجعلها مباشرة وقابلة للتنفيذ قدر الإمكان مع "
 "البقاء قصيرًا"
 
-#: capeditor/blocks.py:501
+#: capeditor/blocks.py:528
 msgid "Description"
 msgstr "وصف"
 
-#: capeditor/blocks.py:503
+#: capeditor/blocks.py:530
 #, fuzzy
 #| msgid "The text describing the subject event of the alert message"
 msgid ""
 "The text describing the subject event of the alert message. An extended "
 "description of the hazard or event that occasioned this message"
 msgstr ""
 "النص الذي يصف الحدث الموضوع لرسالة التنبيه. وصف موسع للمخاطر أو الحدث الذي "
 "تسبب في هذه الرسالة"
 
-#: capeditor/blocks.py:505
+#: capeditor/blocks.py:532
 msgid "Instruction"
 msgstr "تعليمات"
 
-#: capeditor/blocks.py:506
+#: capeditor/blocks.py:533
 msgid ""
 "The text describing the recommended action to be taken by recipients of the "
 "alert message"
 msgstr ""
 "النص الذي يصف الإجراء الموصى به الذي يتعين على مستلمي رسالة التنبيه اتخاذه"
 
-#: capeditor/blocks.py:508
+#: capeditor/blocks.py:535
 msgid "Effective"
 msgstr "فعال"
 
-#: capeditor/blocks.py:509
+#: capeditor/blocks.py:536
 #, fuzzy
 #| msgid "The effective time of the information of the alert message"
 msgid ""
 "The effective time of the information of the alert message. If not set, the "
 "sent date will be used"
 msgstr ""
 "الوقت الفعلي لمعلومات رسالة التنبيه. إذا لم يتم التعيين ، فسيتم استخدام "
 "تاريخ الإرسال"
 
-#: capeditor/blocks.py:511
+#: capeditor/blocks.py:538
 msgid "Onset"
 msgstr "بداية"
 
-#: capeditor/blocks.py:512
+#: capeditor/blocks.py:539
 msgid ""
 "The expected time of the beginning of the subject event of the alert message"
 msgstr "الوقت المتوقع لبداية موضوع الحدث لرسالة التنبيه"
 
-#: capeditor/blocks.py:514
+#: capeditor/blocks.py:541
 msgid "Expires"
 msgstr "تنتهي"
 
-#: capeditor/blocks.py:515
+#: capeditor/blocks.py:542
 msgid ""
 "The expiry time of the information of the alert message. If not set, each "
 "recipient is free to set its own policy as to when the message is no longer "
 "in effect."
 msgstr ""
 "وقت انتهاء صلاحية معلومات رسالة التنبيه. في حالة عدم التعيين ، يكون لكل "
 "مستلم الحرية في تعيين سياسته الخاصة عندما لا تكون الرسالة سارية المفعول."
 
-#: capeditor/blocks.py:518
+#: capeditor/blocks.py:545
 #, fuzzy
 #| msgid "Response type"
 msgid "Response Types"
 msgstr "أنواع الاستجابة"
 
-#: capeditor/blocks.py:520
+#: capeditor/blocks.py:547
 #, fuzzy
 #| msgid "Sender"
 msgid "Sender name"
 msgstr "اسم المرسل"
 
-#: capeditor/blocks.py:522
+#: capeditor/blocks.py:549
 msgid "Contact"
 msgstr "اتصال"
 
-#: capeditor/blocks.py:523 capeditor/blocks.py:550
+#: capeditor/blocks.py:550 capeditor/blocks.py:580
 msgid "Audience"
 msgstr "جمهور"
 
-#: capeditor/blocks.py:526
+#: capeditor/blocks.py:553
 msgid "Admin Boundary"
 msgstr "حدود الإدارة"
 
-#: capeditor/blocks.py:527
+#: capeditor/blocks.py:554
 msgid "Draw Polygon"
 msgstr "ارسم مضلع"
 
-#: capeditor/blocks.py:529
+#: capeditor/blocks.py:556
 msgid "Geocode"
 msgstr "تكويد جغرافيًا"
 
-#: capeditor/blocks.py:530
+#: capeditor/blocks.py:557
 msgid "Alert Area"
 msgstr "منطقة التنبيه"
 
-#: capeditor/blocks.py:530
+#: capeditor/blocks.py:557
 msgid "Admin Boundary, Polygon, Circle or Geocode"
 msgstr "حدود الإدارة أو المضلع أو الدائرة أو الرمز الجغرافي"
 
-#: capeditor/blocks.py:535
+#: capeditor/blocks.py:562
 #, fuzzy
 #| msgid "Resource"
 msgid "Resources"
 msgstr "موارد"
 
-#: capeditor/blocks.py:535
+#: capeditor/blocks.py:562
 msgid ""
 "Additional file with supplemental information related to this alert "
 "information"
 msgstr "ملف إضافي بمعلومات تكميلية متعلقة بمعلومات التنبيه هذه"
 
-#: capeditor/blocks.py:538
+#: capeditor/blocks.py:565
 msgid "Parameter"
 msgstr "معامل"
 
-#: capeditor/blocks.py:538
+#: capeditor/blocks.py:565
 msgid "Parameters"
 msgstr "حدود"
 
-#: capeditor/blocks.py:539
+#: capeditor/blocks.py:566
 #, fuzzy
 #| msgid "Event"
 msgid "Event Code"
 msgstr "كود الحدث"
 
-#: capeditor/blocks.py:539
+#: capeditor/blocks.py:566
 #, fuzzy
 #| msgid "Event"
 msgid "Event codes"
 msgstr "رموز الحدث"
 
-#: capeditor/blocks.py:545
+#: capeditor/blocks.py:575
 msgid "Hazard"
 msgstr "خطر"
 
-#: capeditor/blocks.py:554
+#: capeditor/blocks.py:584
 #, fuzzy
 #| msgid "Contact"
 msgid "Contact Detail"
 msgstr "تفاصيل الإتصال"
 
 #: capeditor/models.py:35
 #, fuzzy
@@ -821,15 +821,15 @@
 #~ msgid "Earlier Reference Alerts -  If applicable"
 #~ msgstr "تنبيهات مرجعية سابقة - إن وجدت"
 
 #~ msgid "Alert"
 #~ msgstr "يُحذًِر"
 
 #~ msgid "Intended Recipients (If scope is Private) "
-#~ msgstr "المستلمون المقصودون (إذا كان النطاق خاصًا)"
+#~ msgstr "المستلمون المستهدفون (إذا كان النطاق خاصًا)"
 
 #~ msgid "Alert Identification (Sender, Message Type, Scope)"
 #~ msgstr "تعريف التنبيه (المرسل ، نوع الرسالة ، النطاق)"
 
 #~ msgid "Alert Info"
 #~ msgstr "معلومات التنبيه"
```

### Comparing `capeditor-0.2.7/capeditor/locale/en/LC_MESSAGES/django.mo` & `capeditor-0.2.8/capeditor/locale/en/LC_MESSAGES/django.mo`

 * *Files 11% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,100 +8,86 @@
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid ""
-" Identifies the originator of an alert. This can be an email of the "
-"institution for example"
-msgstr ""
-"Identifies the originator of an alert. This can be an email of the "
-"institution for example"
-
-msgid ""
 "Acknowledge - Acknowledges receipt and acceptance of the message(s) "
 "identified in references field"
 msgstr ""
 "Acknowledge - Acknowledges receipt and acceptance of the message(s) "
 "identified in references field"
 
 msgid "Actual - Actionable by all targeted recipients"
 msgstr "Actual - Actionable by all targeted recipients"
 
+msgid ""
+"Additional file with supplemental information related to this alert "
+"information"
+msgstr ""
+"Additional file with supplemental information related to this alert "
+"information"
+
+msgid "Addresses"
+msgstr "Addresses"
+
+msgid "Admin Boundary"
+msgstr "Admin Boundary"
+
+msgid "Admin Boundary, Polygon, Circle or Geocode"
+msgstr "Admin Boundary, Polygon, Circle or Geocode"
+
+msgid "Administrative Level"
+msgstr "Administrative Level"
+
 msgid "Affected areas / Regions"
 msgstr "Affected areas / Regions"
 
-msgid "Alert"
-msgstr "Alert"
-
 msgid "Alert - Initial information requiring attention by targeted recipients"
 msgstr "Alert - Initial information requiring attention by targeted recipients"
 
 msgid "Alert Area"
 msgstr "Alert Area"
 
-msgid "Alert Areas "
-msgstr "Alert Areas"
-
-msgid ""
-"Alert Categorization (Category, Urgency, Severity, Certainity, Response & "
-"Dates)"
-msgstr ""
-"Alert Categorization (Category, Urgency, Severity, Certainity, Response & "
-"Dates)"
-
-msgid ""
-"Alert Delivery Message (Headline, Description, Intsructions, Contact & "
-"Website)"
-msgstr ""
-"Alert Delivery Message (Headline, Description, Intsructions, Contact & "
-"Website)"
-
-msgid "Alert Identification (Sender, Message Type, Scope)"
-msgstr "Alert Identification (Sender, Message Type, Scope)"
-
-msgid "Alert Info"
-msgstr "Alert Info"
-
 msgid "Alert Information"
 msgstr "Alert Information"
 
-msgid "Alert Resources "
-msgstr "Alert Resources"
-
-msgid "Alerts Per Page"
-msgstr "Alerts Per Page"
-
 msgid ""
 "All Clear - The subject event no longer poses a threat or concern and any "
 "follow on action is described in instruction"
 msgstr ""
 "All Clear - The subject event no longer poses a threat or concern and any "
 "follow on action is described in instruction"
 
 msgid "Altitude"
 msgstr "Altitude"
 
-msgid "Area"
-msgstr "Area"
-
 msgid ""
 "Assess - Evaluate the information in this message - DONT USE FOR PUBLIC "
 "ALERTS"
 msgstr ""
 "Assess - Evaluate the information in this message - DONT USE FOR PUBLIC "
 "ALERTS"
 
 msgid "Audience"
 msgstr "Audience"
 
 msgid "Avoid - Avoid the subject event as per the instruction"
 msgstr "Avoid - Avoid the subject event as per the instruction"
 
+msgid "Boundary"
+msgstr "Boundary"
+
+msgid "CAP Sender Name"
+msgstr "CAP Sender Name"
+
+msgid "Can be the website link or email of the sending institution"
+msgstr "Can be the website link or email of the sending institution"
+
 msgid "Cancel - Cancels the earlier message(s) identified in references"
 msgstr "Cancel - Cancels the earlier message(s) identified in references"
 
 msgid "Category"
 msgstr "Category"
 
 msgid "Ceiling"
@@ -113,46 +99,43 @@
 msgid ""
 "Chemical, Biological, Radiological, Nuclear or High-Yield Explosive threat "
 "or attack"
 msgstr ""
 "Chemical, Biological, Radiological, Nuclear or High-Yield Explosive threat "
 "or attack"
 
+msgid "Circle"
+msgstr "Circle"
+
 msgid "Code"
 msgstr "Code"
 
 msgid "Contact"
 msgstr "Contact"
 
 msgid "Description"
 msgstr "Description"
 
-msgid "Description of the incident"
-msgstr "Description of the incident"
-
 msgid ""
 "Draft - A preliminary template or draft, not actionable in its current form"
 msgstr ""
 "Draft - A preliminary template or draft, not actionable in its current form"
 
-msgid "Earlier Reference Alerts -  If applicable"
-msgstr "Earlier Reference Alerts -  If applicable"
+msgid "Drag the marker to change position"
+msgstr "Drag the marker to change position"
+
+msgid "Draw Polygon"
+msgstr "Draw Polygon"
 
 msgid "Earlier alert referenced by this alert"
 msgstr "Earlier alert referenced by this alert"
 
 msgid "Effective"
 msgstr "Effective"
 
-msgid "Email"
-msgstr "Email"
-
-msgid "Email address"
-msgstr "Email address"
-
 msgid "English"
 msgstr "English"
 
 msgid ""
 "Error -  Indicates rejection of the message(s) identified in references; "
 "explanation SHOULD appear in note field"
 msgstr ""
@@ -171,83 +154,77 @@
 msgid ""
 "Exercise - Actionable only by designated exercise participants; exercise "
 "identifier SHOULD appear in note"
 msgstr ""
 "Exercise - Actionable only by designated exercise participants; exercise "
 "identifier SHOULD appear in note"
 
-msgid "Expected"
-msgstr "Expected"
-
 msgid "Expected - Responsive action SHOULD be taken soon (within next hour)"
 msgstr "Expected - Responsive action SHOULD be taken soon (within next hour)"
 
 msgid "Expires"
 msgstr "Expires"
 
 msgid "Extreme - Extraordinary threat to life or property"
 msgstr "Extreme - Extraordinary threat to life or property"
 
-msgid "File"
-msgstr "File"
-
-msgid "File, Document etc"
-msgstr "File, Document etc"
-
 msgid "Fire suppression and rescue"
 msgstr "Fire suppression and rescue"
 
-msgid "Future"
-msgstr "Future"
-
 msgid "Future - Responsive action SHOULD be taken in the near future"
 msgstr "Future - Responsive action SHOULD be taken in the near future"
 
 msgid "General emergency and public safety"
 msgstr "General emergency and public safety"
 
+msgid "Geocode"
+msgstr "Geocode"
+
 msgid "Geophysical"
 msgstr "Geophysical"
 
+msgid "Hazard"
+msgstr "Hazard"
+
+msgid "Hazards monitored by the institution"
+msgstr "Hazards monitored by the institution"
+
 msgid "Headline"
 msgstr "Headline"
 
-msgid ""
-"How many of this products should be visible on the landing page filter "
-"section ?"
-msgstr ""
-"How many of this products should be visible on the landing page filter "
-"section ?"
-
 msgid "Identifier"
 msgstr "Identifier"
 
-msgid "Immediate"
-msgstr "Immediate"
-
 msgid "Immediate - Responsive action SHOULD be taken immediately"
 msgstr "Immediate - Responsive action SHOULD be taken immediately"
 
+msgid "Incident"
+msgstr "Incident"
+
+msgid "Incidents"
+msgstr "Incidents"
+
 msgid "Instruction"
 msgstr "Instruction"
 
-msgid "Intended Recipients (If scope is Private) "
-msgstr "Intended Recipients (If scope is Private)"
-
 msgid "Language"
 msgstr "Language"
 
 msgid "Law enforcement, military, homeland and local/private security"
 msgstr "Law enforcement, military, homeland and local/private security"
 
 msgid "Likely - Likely (percentage > ~50%)"
 msgstr "Likely - Likely (percentage > ~50%)"
 
-msgid "Link"
-msgstr "Link"
+msgid ""
+"Link to external resource. This can be for example a link to related "
+"websites. "
+msgstr ""
+"Link to external resource. This can be for example a link to related "
+"websites."
 
 msgid "Medical and public health"
 msgstr "Medical and public health"
 
 msgid "Message Type"
 msgstr "Message Type"
 
@@ -265,17 +242,14 @@
 
 msgid "Name"
 msgstr "Name"
 
 msgid "Name for the event code"
 msgstr "Name for the event code"
 
-msgid "Name for the geocode"
-msgstr "Name for the geocode"
-
 msgid "Name of the recipient"
 msgstr "Name of the recipient"
 
 msgid "No action recommended"
 msgstr "No action recommended"
 
 msgid "Note"
@@ -286,23 +260,29 @@
 
 msgid "Onset"
 msgstr "Onset"
 
 msgid "Other events"
 msgstr "Other events"
 
-msgid "Past"
-msgstr "Past"
+msgid "Parameter"
+msgstr "Parameter"
+
+msgid "Parameters"
+msgstr "Parameters"
 
 msgid "Past - Responsive action is no longer required"
 msgstr "Past - Responsive action is no longer required"
 
 msgid "Pollution and other environmental"
 msgstr "Pollution and other environmental"
 
+msgid "Polygon"
+msgstr "Polygon"
+
 msgid "Possible - Possible but not likely (percentage <= ~50%)"
 msgstr "Possible - Possible but not likely (percentage <= ~50%)"
 
 msgid "Prepare - Relocate as instructed in the instruction"
 msgstr "Prepare - Relocate as instructed in the instruction"
 
 msgid ""
@@ -323,20 +303,14 @@
 
 msgid "Reference Alert"
 msgstr "Reference Alert"
 
 msgid "Rescue and recovery"
 msgstr "Rescue and recovery"
 
-msgid "Resource"
-msgstr "Resource"
-
-msgid "Resource type whether is image, file etc"
-msgstr "Resource type whether is image, file etc"
-
 msgid "Response type"
 msgstr "Response type"
 
 msgid ""
 "Restricted - For dissemination only to users with a known operational "
 "requirement as in the restriction field"
 msgstr ""
@@ -369,20 +343,20 @@
 
 msgid "Status"
 msgstr "Status"
 
 msgid "System - For messages that support alert network internal functions"
 msgstr "System - For messages that support alert network internal functions"
 
+msgid "Target audiences for published alerts"
+msgstr "Target audiences for published alerts"
+
 msgid "Test - Technical testing only, all recipients disregard"
 msgstr "Test - Technical testing only, all recipients disregard"
 
-msgid "The base-64 encoded data content of the resource file"
-msgstr "The base-64 encoded data content of the resource file"
-
 msgid "The code denoting the appropriate handling of the alert"
 msgstr "The code denoting the appropriate handling of the alert"
 
 msgid ""
 "The code denoting the category of the subject event of the alert message"
 msgstr ""
 "The code denoting the category of the subject event of the alert message"
@@ -415,40 +389,29 @@
 "The code denoting the type of action recommended for the target audience"
 
 msgid "The code denoting the urgency of the subject event of the alert message"
 msgstr ""
 "The code denoting the urgency of the subject event of the alert message"
 
 msgid ""
-"The code representing the digital digest ('hash') computed from the resource "
-"file"
-msgstr ""
-"The code representing the digital digest ('hash') computed from the resource "
-"file"
-
-msgid "The effective time of the information of the alert message"
-msgstr "The effective time of the information of the alert message"
-
-msgid ""
 "The expected time of the beginning of the subject event of the alert message"
 msgstr ""
 "The expected time of the beginning of the subject event of the alert message"
 
-msgid "The expiry time of the information of the alert message"
-msgstr "The expiry time of the information of the alert message"
-
 msgid ""
-"The identifier of the hyperlink associating additional information with the "
-"alert message"
-msgstr ""
-"The identifier of the hyperlink associating additional information with the "
-"alert message"
+"The expiry time of the information of the alert message. If not set, each "
+"recipient is free to set its own policy as to when the message is no longer "
+"in effect."
+msgstr ""
+"The expiry time of the information of the alert message. If not set, each "
+"recipient is free to set its own policy as to when the message is no longer "
+"in effect."
 
-msgid "The identifier of the hyperlink for the resource file"
-msgstr "The identifier of the hyperlink for the resource file"
+msgid "The human-readable name of the agency or authority issuing this alert."
+msgstr "The human-readable name of the agency or authority issuing this alert."
 
 msgid ""
 "The maximum altitude of the affected area of the alert message.MUST NOT be "
 "used except in combination with the altitude element. "
 msgstr ""
 "The maximum altitude of the affected area of the alert message.MUST NOT be "
 "used except in combination with the altitude element."
@@ -500,70 +463,49 @@
 msgid ""
 "The text describing the rule for limiting distribution of the restricted "
 "alert message. Used when scope value is Restricted"
 msgstr ""
 "The text describing the rule for limiting distribution of the restricted "
 "alert message. Used when scope value is Restricted"
 
-msgid "The text describing the subject event of the alert message"
-msgstr "The text describing the subject event of the alert message"
-
 msgid "The text describing the type and content of the resource file"
 msgstr "The text describing the type and content of the resource file"
 
-msgid "The text headline of the alert message"
-msgstr "The text headline of the alert message"
+msgid ""
+"The text headline of the alert message. Make it direct and actionable as "
+"possible while remaining short"
+msgstr ""
+"The text headline of the alert message. Make it direct and actionable as "
+"possible while remaining short"
 
 msgid "The text identifying the source of the alert message"
 msgstr "The text identifying the source of the alert message"
 
 msgid "Time and date of origination of the alert"
 msgstr "Time and date of origination of the alert"
 
-msgid "Title"
-msgstr "Title"
-
-msgid "Title of the incident referent of the alert"
-msgstr "Title of the incident referent of the alert"
-
 msgid "Unique ID. Auto generated on creation."
 msgstr "Unique ID. Auto generated on creation."
 
-msgid "Unknown"
-msgstr "Unknown"
-
 msgid "Unknown - Certainty unknown"
 msgstr "Unknown - Certainty unknown"
 
 msgid "Unknown - Severity unknown"
 msgstr "Unknown - Severity unknown"
 
 msgid "Unknown - Urgency not known"
 msgstr "Unknown - Urgency not known"
 
 msgid "Unlikely - Not expected to occur (percentage ~ 0)"
 msgstr "Unlikely - Not expected to occur (percentage ~ 0)"
 
-msgid ""
-"Update - Updates and supercedes the earlier message(s) identified in "
-"referenced alerts"
-msgstr ""
-"Update - Updates and supercedes the earlier message(s) identified in "
-"referenced alerts"
-
 msgid "Urgency"
 msgstr "Urgency"
 
 msgid "Utility, telecommunication, other non-transport infrastructure"
 msgstr "Utility, telecommunication, other non-transport infrastructure"
 
 msgid "Value"
 msgstr "Value"
 
 msgid "Value of the event code"
 msgstr "Value of the event code"
-
-msgid "Value of the geocode"
-msgstr "Value of the geocode"
-
-msgid "Web"
-msgstr "Web"
```

### Comparing `capeditor-0.2.7/capeditor/locale/en/LC_MESSAGES/django.po` & `capeditor-0.2.8/capeditor/locale/en/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-12 14:01+0300\n"
+"POT-Creation-Date: 2023-07-14 12:05+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: capeditor/blocks.py:70 capeditor/blocks.py:98 capeditor/blocks.py:370
+#: capeditor/blocks.py:70 capeditor/blocks.py:98 capeditor/blocks.py:375
 msgid "Name"
 msgstr "Name"
 
 #: capeditor/blocks.py:70
 msgid "Name of the recipient"
 msgstr "Name of the recipient"
 
@@ -52,15 +52,15 @@
 
 #: capeditor/blocks.py:94
 #, fuzzy
 #| msgid "The text headline of the alert message"
 msgid "Referent incident to this alert message"
 msgstr "Referent incident to this alert message"
 
-#: capeditor/blocks.py:99 capeditor/blocks.py:295 capeditor/blocks.py:371
+#: capeditor/blocks.py:99 capeditor/blocks.py:300 capeditor/blocks.py:376
 msgid "Value"
 msgstr "Value"
 
 #: capeditor/blocks.py:104
 msgid "Shelter - Take shelter in place or per instruction"
 msgstr "Shelter - Take shelter in place or per instruction"
 
@@ -110,454 +110,454 @@
 
 #: capeditor/blocks.py:117
 msgid ""
 "The code denoting the type of action recommended for the target audience"
 msgstr ""
 "The code denoting the type of action recommended for the target audience"
 
-#: capeditor/blocks.py:158 capeditor/blocks.py:204 capeditor/blocks.py:256
-#: capeditor/blocks.py:292
+#: capeditor/blocks.py:163 capeditor/blocks.py:209 capeditor/blocks.py:261
+#: capeditor/blocks.py:297
 msgid "Affected areas / Regions"
 msgstr "Affected areas / Regions"
 
-#: capeditor/blocks.py:159 capeditor/blocks.py:205 capeditor/blocks.py:257
-#: capeditor/blocks.py:293
+#: capeditor/blocks.py:164 capeditor/blocks.py:210 capeditor/blocks.py:262
+#: capeditor/blocks.py:298
 msgid "The text describing the affected area of the alert message"
 msgstr "The text describing the affected area of the alert message"
 
-#: capeditor/blocks.py:160
+#: capeditor/blocks.py:165
 msgid "Administrative Level"
 msgstr "Administrative Level"
 
-#: capeditor/blocks.py:161
+#: capeditor/blocks.py:166
 msgid "Boundary"
 msgstr "Boundary"
 
-#: capeditor/blocks.py:162 capeditor/blocks.py:207
+#: capeditor/blocks.py:167 capeditor/blocks.py:212
 msgid ""
 "The paired values of points defining a polygon that delineates the affected "
 "area of the alert message"
 msgstr ""
 "The paired values of points defining a polygon that delineates the affected "
 "area of the alert message"
 
-#: capeditor/blocks.py:165 capeditor/blocks.py:209 capeditor/blocks.py:260
-#: capeditor/blocks.py:297
+#: capeditor/blocks.py:170 capeditor/blocks.py:214 capeditor/blocks.py:265
+#: capeditor/blocks.py:302
 msgid "Altitude"
 msgstr "Altitude"
 
-#: capeditor/blocks.py:166 capeditor/blocks.py:210 capeditor/blocks.py:261
-#: capeditor/blocks.py:298
+#: capeditor/blocks.py:171 capeditor/blocks.py:215 capeditor/blocks.py:266
+#: capeditor/blocks.py:303
 msgid ""
 "The specific or minimum altitude of the affected area of the alert message"
 msgstr ""
 "The specific or minimum altitude of the affected area of the alert message"
 
-#: capeditor/blocks.py:168 capeditor/blocks.py:212 capeditor/blocks.py:263
-#: capeditor/blocks.py:300
+#: capeditor/blocks.py:173 capeditor/blocks.py:217 capeditor/blocks.py:268
+#: capeditor/blocks.py:305
 msgid "Ceiling"
 msgstr "Ceiling"
 
-#: capeditor/blocks.py:169 capeditor/blocks.py:213 capeditor/blocks.py:264
-#: capeditor/blocks.py:301
+#: capeditor/blocks.py:174 capeditor/blocks.py:218 capeditor/blocks.py:269
+#: capeditor/blocks.py:306
 msgid ""
 "The maximum altitude of the affected area of the alert message.MUST NOT be "
 "used except in combination with the altitude element. "
 msgstr ""
 "The maximum altitude of the affected area of the alert message.MUST NOT be "
 "used except in combination with the altitude element."
 
-#: capeditor/blocks.py:206
+#: capeditor/blocks.py:211
 msgid "Polygon"
 msgstr "Polygon"
 
-#: capeditor/blocks.py:258 capeditor/blocks.py:528
+#: capeditor/blocks.py:263 capeditor/blocks.py:555
 msgid "Circle"
 msgstr "Circle"
 
-#: capeditor/blocks.py:258
+#: capeditor/blocks.py:263
 msgid "Drag the marker to change position"
 msgstr "Drag the marker to change position"
 
-#: capeditor/blocks.py:305
+#: capeditor/blocks.py:310
 msgid "The human-readable name of the agency or authority issuing this alert."
 msgstr ""
 "The human-readable name of the agency or authority issuing this alert."
 
-#: capeditor/blocks.py:306
+#: capeditor/blocks.py:311
 msgid ""
 "The text describing the contact for follow-up and confirmation of the alert "
 "message"
 msgstr ""
 "The text describing the contact for follow-up and confirmation of the alert "
 "message"
 
-#: capeditor/blocks.py:307
+#: capeditor/blocks.py:312
 msgid "The text denoting the type of the subject event of the alert message"
 msgstr "The text denoting the type of the subject event of the alert message"
 
-#: capeditor/blocks.py:308
+#: capeditor/blocks.py:313
 msgid "The text describing the intended audience of the alert message"
 msgstr "The text describing the intended audience of the alert message"
 
-#: capeditor/blocks.py:350 capeditor/blocks.py:359
+#: capeditor/blocks.py:355 capeditor/blocks.py:364
 #, fuzzy
 #| msgid "Description"
 msgid "Resource Description"
 msgstr "Resource Description"
 
-#: capeditor/blocks.py:351 capeditor/blocks.py:360
+#: capeditor/blocks.py:356 capeditor/blocks.py:365
 msgid "The text describing the type and content of the resource file"
 msgstr "The text describing the type and content of the resource file"
 
-#: capeditor/blocks.py:361
+#: capeditor/blocks.py:366
 #, fuzzy
 #| msgid "Alert Resources "
 msgid "External Resource Link"
 msgstr "External Resource Link"
 
-#: capeditor/blocks.py:362
+#: capeditor/blocks.py:367
 msgid ""
 "Link to external resource. This can be for example a link to related "
 "websites. "
 msgstr ""
 "Link to external resource. This can be for example a link to related "
 "websites."
 
-#: capeditor/blocks.py:370
+#: capeditor/blocks.py:375
 msgid "Name for the event code"
 msgstr "Name for the event code"
 
-#: capeditor/blocks.py:371
+#: capeditor/blocks.py:376
 msgid "Value of the event code"
 msgstr "Value of the event code"
 
-#: capeditor/blocks.py:441
+#: capeditor/blocks.py:467
 msgid "English"
 msgstr "English"
 
-#: capeditor/blocks.py:445
+#: capeditor/blocks.py:471
 msgid "Geophysical"
 msgstr "Geophysical"
 
-#: capeditor/blocks.py:446
+#: capeditor/blocks.py:472
 msgid "Meteorological"
 msgstr "Meteorological"
 
-#: capeditor/blocks.py:447
+#: capeditor/blocks.py:473
 msgid "General emergency and public safety"
 msgstr "General emergency and public safety"
 
-#: capeditor/blocks.py:448
+#: capeditor/blocks.py:474
 msgid "Law enforcement, military, homeland and local/private security"
 msgstr "Law enforcement, military, homeland and local/private security"
 
-#: capeditor/blocks.py:449
+#: capeditor/blocks.py:475
 msgid "Rescue and recovery"
 msgstr "Rescue and recovery"
 
-#: capeditor/blocks.py:450
+#: capeditor/blocks.py:476
 msgid "Fire suppression and rescue"
 msgstr "Fire suppression and rescue"
 
-#: capeditor/blocks.py:451
+#: capeditor/blocks.py:477
 msgid "Medical and public health"
 msgstr "Medical and public health"
 
-#: capeditor/blocks.py:452
+#: capeditor/blocks.py:478
 msgid "Pollution and other environmental"
 msgstr "Pollution and other environmental"
 
-#: capeditor/blocks.py:453
+#: capeditor/blocks.py:479
 msgid "Public and private transportation"
 msgstr "Public and private transportation"
 
-#: capeditor/blocks.py:454
+#: capeditor/blocks.py:480
 msgid "Utility, telecommunication, other non-transport infrastructure"
 msgstr "Utility, telecommunication, other non-transport infrastructure"
 
-#: capeditor/blocks.py:455
+#: capeditor/blocks.py:481
 msgid ""
 "Chemical, Biological, Radiological, Nuclear or High-Yield Explosive threat "
 "or attack"
 msgstr ""
 "Chemical, Biological, Radiological, Nuclear or High-Yield Explosive threat "
 "or attack"
 
-#: capeditor/blocks.py:456
+#: capeditor/blocks.py:482
 msgid "Other events"
 msgstr "Other events"
 
-#: capeditor/blocks.py:460
+#: capeditor/blocks.py:486
 msgid "Immediate - Responsive action SHOULD be taken immediately"
 msgstr "Immediate - Responsive action SHOULD be taken immediately"
 
-#: capeditor/blocks.py:461
+#: capeditor/blocks.py:487
 msgid "Expected - Responsive action SHOULD be taken soon (within next hour)"
 msgstr "Expected - Responsive action SHOULD be taken soon (within next hour)"
 
-#: capeditor/blocks.py:462
+#: capeditor/blocks.py:488
 msgid "Future - Responsive action SHOULD be taken in the near future"
 msgstr "Future - Responsive action SHOULD be taken in the near future"
 
-#: capeditor/blocks.py:463
+#: capeditor/blocks.py:489
 msgid "Past - Responsive action is no longer required"
 msgstr "Past - Responsive action is no longer required"
 
-#: capeditor/blocks.py:464
+#: capeditor/blocks.py:490
 msgid "Unknown - Urgency not known"
 msgstr "Unknown - Urgency not known"
 
-#: capeditor/blocks.py:468
+#: capeditor/blocks.py:494
 msgid "Extreme - Extraordinary threat to life or property"
 msgstr "Extreme - Extraordinary threat to life or property"
 
-#: capeditor/blocks.py:469
+#: capeditor/blocks.py:495
 msgid "Severe - Significant threat to life or property"
 msgstr "Severe - Significant threat to life or property"
 
-#: capeditor/blocks.py:470
+#: capeditor/blocks.py:496
 msgid "Moderate - Possible threat to life or property"
 msgstr "Moderate - Possible threat to life or property"
 
-#: capeditor/blocks.py:471
+#: capeditor/blocks.py:497
 msgid "Minor - Minimal to no known threat to life or property"
 msgstr "Minor - Minimal to no known threat to life or property"
 
-#: capeditor/blocks.py:472
+#: capeditor/blocks.py:498
 msgid "Unknown - Severity unknown"
 msgstr "Unknown - Severity unknown"
 
-#: capeditor/blocks.py:476
+#: capeditor/blocks.py:502
 msgid "Observed - Determined to have occurred or to be ongoing"
 msgstr "Observed - Determined to have occurred or to be ongoing"
 
-#: capeditor/blocks.py:477
+#: capeditor/blocks.py:503
 msgid "Likely - Likely (percentage > ~50%)"
 msgstr "Likely - Likely (percentage > ~50%)"
 
-#: capeditor/blocks.py:478
+#: capeditor/blocks.py:504
 msgid "Possible - Possible but not likely (percentage <= ~50%)"
 msgstr "Possible - Possible but not likely (percentage <= ~50%)"
 
-#: capeditor/blocks.py:479
+#: capeditor/blocks.py:505
 msgid "Unlikely - Not expected to occur (percentage ~ 0)"
 msgstr "Unlikely - Not expected to occur (percentage ~ 0)"
 
-#: capeditor/blocks.py:480
+#: capeditor/blocks.py:506
 msgid "Unknown - Certainty unknown"
 msgstr "Unknown - Certainty unknown"
 
-#: capeditor/blocks.py:483
-msgid "Language"
-msgstr "Language"
-
-#: capeditor/blocks.py:484
-msgid "The code denoting the language of the alert message"
-msgstr "The code denoting the language of the alert message"
+#: capeditor/blocks.py:508
+msgid "Event"
+msgstr "Event"
 
-#: capeditor/blocks.py:485
+#: capeditor/blocks.py:510
 msgid "Category"
 msgstr "Category"
 
-#: capeditor/blocks.py:486
+#: capeditor/blocks.py:511
 msgid ""
 "The code denoting the category of the subject event of the alert message"
 msgstr ""
 "The code denoting the category of the subject event of the alert message"
 
-#: capeditor/blocks.py:488
-msgid "Event"
-msgstr "Event"
+#: capeditor/blocks.py:513
+msgid "Language"
+msgstr "Language"
 
-#: capeditor/blocks.py:489
+#: capeditor/blocks.py:514
+msgid "The code denoting the language of the alert message"
+msgstr "The code denoting the language of the alert message"
+
+#: capeditor/blocks.py:516
 msgid "Urgency"
 msgstr "Urgency"
 
-#: capeditor/blocks.py:490
+#: capeditor/blocks.py:517
 msgid ""
 "The code denoting the urgency of the subject event of the alert message"
 msgstr ""
 "The code denoting the urgency of the subject event of the alert message"
 
-#: capeditor/blocks.py:492
+#: capeditor/blocks.py:519
 msgid "Severity"
 msgstr "Severity"
 
-#: capeditor/blocks.py:493
+#: capeditor/blocks.py:520
 msgid ""
 "The code denoting the severity of the subject event of the alert message"
 msgstr ""
 "The code denoting the severity of the subject event of the alert message"
 
-#: capeditor/blocks.py:495
+#: capeditor/blocks.py:522
 msgid "Certainty"
 msgstr "Certainty"
 
-#: capeditor/blocks.py:496
+#: capeditor/blocks.py:523
 msgid ""
 "The code denoting the certainty of the subject event of the alert message"
 msgstr ""
 "The code denoting the certainty of the subject event of the alert message"
 
-#: capeditor/blocks.py:498
+#: capeditor/blocks.py:525
 msgid "Headline"
 msgstr "Headline"
 
-#: capeditor/blocks.py:499
+#: capeditor/blocks.py:526
 msgid ""
 "The text headline of the alert message. Make it direct and actionable as "
 "possible while remaining short"
 msgstr ""
 "The text headline of the alert message. Make it direct and actionable as "
 "possible while remaining short"
 
-#: capeditor/blocks.py:501
+#: capeditor/blocks.py:528
 msgid "Description"
 msgstr "Description"
 
-#: capeditor/blocks.py:503
+#: capeditor/blocks.py:530
 #, fuzzy
 #| msgid "The text describing the subject event of the alert message"
 msgid ""
 "The text describing the subject event of the alert message. An extended "
 "description of the hazard or event that occasioned this message"
 msgstr ""
 "The text describing the subject event of the alert message. An extended "
 "description of the hazard or event that occasioned this message"
 
-#: capeditor/blocks.py:505
+#: capeditor/blocks.py:532
 msgid "Instruction"
 msgstr "Instruction"
 
-#: capeditor/blocks.py:506
+#: capeditor/blocks.py:533
 msgid ""
 "The text describing the recommended action to be taken by recipients of the "
 "alert message"
 msgstr ""
 "The text describing the recommended action to be taken by recipients of the "
 "alert message"
 
-#: capeditor/blocks.py:508
+#: capeditor/blocks.py:535
 msgid "Effective"
 msgstr "Effective"
 
-#: capeditor/blocks.py:509
+#: capeditor/blocks.py:536
 #, fuzzy
 #| msgid "The effective time of the information of the alert message"
 msgid ""
 "The effective time of the information of the alert message. If not set, the "
 "sent date will be used"
 msgstr ""
 "The effective time of the information of the alert message. If not set, the "
 "sent date will be used"
 
-#: capeditor/blocks.py:511
+#: capeditor/blocks.py:538
 msgid "Onset"
 msgstr "Onset"
 
-#: capeditor/blocks.py:512
+#: capeditor/blocks.py:539
 msgid ""
 "The expected time of the beginning of the subject event of the alert message"
 msgstr ""
 "The expected time of the beginning of the subject event of the alert message"
 
-#: capeditor/blocks.py:514
+#: capeditor/blocks.py:541
 msgid "Expires"
 msgstr "Expires"
 
-#: capeditor/blocks.py:515
+#: capeditor/blocks.py:542
 msgid ""
 "The expiry time of the information of the alert message. If not set, each "
 "recipient is free to set its own policy as to when the message is no longer "
 "in effect."
 msgstr ""
 "The expiry time of the information of the alert message. If not set, each "
 "recipient is free to set its own policy as to when the message is no longer "
 "in effect."
 
-#: capeditor/blocks.py:518
+#: capeditor/blocks.py:545
 #, fuzzy
 #| msgid "Response type"
 msgid "Response Types"
 msgstr "Response Types"
 
-#: capeditor/blocks.py:520
+#: capeditor/blocks.py:547
 #, fuzzy
 #| msgid "Sender"
 msgid "Sender name"
 msgstr "Sender name"
 
-#: capeditor/blocks.py:522
+#: capeditor/blocks.py:549
 msgid "Contact"
 msgstr "Contact"
 
-#: capeditor/blocks.py:523 capeditor/blocks.py:550
+#: capeditor/blocks.py:550 capeditor/blocks.py:580
 msgid "Audience"
 msgstr "Audience"
 
-#: capeditor/blocks.py:526
+#: capeditor/blocks.py:553
 msgid "Admin Boundary"
 msgstr "Admin Boundary"
 
-#: capeditor/blocks.py:527
+#: capeditor/blocks.py:554
 msgid "Draw Polygon"
 msgstr "Draw Polygon"
 
-#: capeditor/blocks.py:529
+#: capeditor/blocks.py:556
 msgid "Geocode"
 msgstr "Geocode"
 
-#: capeditor/blocks.py:530
+#: capeditor/blocks.py:557
 msgid "Alert Area"
 msgstr "Alert Area"
 
-#: capeditor/blocks.py:530
+#: capeditor/blocks.py:557
 msgid "Admin Boundary, Polygon, Circle or Geocode"
 msgstr "Admin Boundary, Polygon, Circle or Geocode"
 
-#: capeditor/blocks.py:535
+#: capeditor/blocks.py:562
 #, fuzzy
 #| msgid "Resource"
 msgid "Resources"
 msgstr "Resources"
 
-#: capeditor/blocks.py:535
+#: capeditor/blocks.py:562
 msgid ""
 "Additional file with supplemental information related to this alert "
 "information"
 msgstr ""
 "Additional file with supplemental information related to this alert "
 "information"
 
-#: capeditor/blocks.py:538
+#: capeditor/blocks.py:565
 msgid "Parameter"
 msgstr "Parameter"
 
-#: capeditor/blocks.py:538
+#: capeditor/blocks.py:565
 msgid "Parameters"
 msgstr "Parameters"
 
-#: capeditor/blocks.py:539
+#: capeditor/blocks.py:566
 #, fuzzy
 #| msgid "Event"
 msgid "Event Code"
 msgstr "Event Code"
 
-#: capeditor/blocks.py:539
+#: capeditor/blocks.py:566
 #, fuzzy
 #| msgid "Event"
 msgid "Event codes"
 msgstr "Event codes"
 
-#: capeditor/blocks.py:545
+#: capeditor/blocks.py:575
 msgid "Hazard"
 msgstr "Hazard"
 
-#: capeditor/blocks.py:554
+#: capeditor/blocks.py:584
 #, fuzzy
 #| msgid "Contact"
 msgid "Contact Detail"
 msgstr "Contact Detail"
 
 #: capeditor/models.py:35
 #, fuzzy
```

### Comparing `capeditor-0.2.7/capeditor/locale/es/LC_MESSAGES/django.mo` & `capeditor-0.2.8/capeditor/locale/es/LC_MESSAGES/django.mo`

 * *Files 17% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,103 +8,91 @@
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid ""
-" Identifies the originator of an alert. This can be an email of the "
-"institution for example"
-msgstr ""
-"Identifica el autor de una alerta. Este puede ser un correo electrónico de "
-"la institución por ejemplo"
-
-msgid ""
 "Acknowledge - Acknowledges receipt and acceptance of the message(s) "
 "identified in references field"
 msgstr ""
 "Acuse de recibo: acusa recibo y aceptación de los mensajes identificados en "
 "el campo de referencias."
 
 msgid "Actual - Actionable by all targeted recipients"
 msgstr "Real: procesable por todos los destinatarios objetivo"
 
+msgid ""
+"Additional file with supplemental information related to this alert "
+"information"
+msgstr ""
+"Archivo adicional con información complementaria relacionada con esta "
+"información de alerta"
+
+msgid "Addresses"
+msgstr "direcciones"
+
+msgid "Admin Boundary"
+msgstr "Límite de administración"
+
+msgid "Admin Boundary, Polygon, Circle or Geocode"
+msgstr "Límite de administrador, polígono, círculo o código geográfico"
+
+msgid "Administrative Level"
+msgstr "Nivel Administrativo"
+
 msgid "Affected areas / Regions"
 msgstr "Áreas / Regiones afectadas"
 
-msgid "Alert"
-msgstr "Alerta"
-
 msgid "Alert - Initial information requiring attention by targeted recipients"
 msgstr ""
 "Alerta: información inicial que requiere atención por parte de los "
 "destinatarios específicos"
 
 msgid "Alert Area"
 msgstr "Área de alerta"
 
-msgid "Alert Areas "
-msgstr "Áreas de alerta"
-
-msgid ""
-"Alert Categorization (Category, Urgency, Severity, Certainity, Response & "
-"Dates)"
-msgstr ""
-"Categorización de alertas (categoría, urgencia, gravedad, certeza, respuesta "
-"y fechas)"
-
-msgid ""
-"Alert Delivery Message (Headline, Description, Intsructions, Contact & "
-"Website)"
-msgstr ""
-"Mensaje de entrega de alerta (título, descripción, instrucciones, contacto y "
-"sitio web)"
-
-msgid "Alert Identification (Sender, Message Type, Scope)"
-msgstr "Identificación de alertas (remitente, tipo de mensaje, alcance)"
-
-msgid "Alert Info"
-msgstr "Información de alerta"
-
 msgid "Alert Information"
 msgstr "Información de alerta"
 
-msgid "Alert Resources "
-msgstr "Recursos de alerta"
-
-msgid "Alerts Per Page"
-msgstr "Alertas por página"
-
 msgid ""
 "All Clear - The subject event no longer poses a threat or concern and any "
 "follow on action is described in instruction"
 msgstr ""
 "Todo despejado: el evento en cuestión ya no representa una amenaza o "
 "preocupación y cualquier acción de seguimiento se describe en las "
 "instrucciones."
 
 msgid "Altitude"
 msgstr "Altitud"
 
-msgid "Area"
-msgstr "Área"
-
 msgid ""
 "Assess - Evaluate the information in this message - DONT USE FOR PUBLIC "
 "ALERTS"
 msgstr ""
 "Evaluar - Evaluar la información de este mensaje - NO UTILIZAR PARA ALERTAS "
 "PÚBLICAS"
 
 msgid "Audience"
 msgstr "Audiencia"
 
 msgid "Avoid - Avoid the subject event as per the instruction"
 msgstr "Evitar: evita el evento en cuestión según las instrucciones."
 
+msgid "Boundary"
+msgstr "Perímetro"
+
+msgid "CAP Sender Name"
+msgstr "Nombre del remitente CAP"
+
+msgid "Can be the website link or email of the sending institution"
+msgstr ""
+"Puede ser el enlace del sitio web o el correo electrónico de la institución "
+"de envío"
+
 msgid "Cancel - Cancels the earlier message(s) identified in references"
 msgstr ""
 "Cancelar: cancela los mensajes anteriores identificados en las referencias"
 
 msgid "Category"
 msgstr "Categoría"
 
@@ -117,47 +105,44 @@
 msgid ""
 "Chemical, Biological, Radiological, Nuclear or High-Yield Explosive threat "
 "or attack"
 msgstr ""
 "Amenaza o ataque químico, biológico, radiológico, nuclear o explosivo de "
 "alto rendimiento"
 
+msgid "Circle"
+msgstr "Círculo"
+
 msgid "Code"
 msgstr "Código"
 
 msgid "Contact"
 msgstr "Contacto"
 
 msgid "Description"
 msgstr "Descripción"
 
-msgid "Description of the incident"
-msgstr "Descripción del incidente"
-
 msgid ""
 "Draft - A preliminary template or draft, not actionable in its current form"
 msgstr ""
 "Borrador: una plantilla o borrador preliminar, no procesable en su forma "
 "actual"
 
-msgid "Earlier Reference Alerts -  If applicable"
-msgstr "Alertas de referencia anteriores: si corresponde"
+msgid "Drag the marker to change position"
+msgstr "Arrastra el marcador para cambiar de posición"
+
+msgid "Draw Polygon"
+msgstr "dibujar polígono"
 
 msgid "Earlier alert referenced by this alert"
 msgstr "Alerta anterior a la que hace referencia esta alerta"
 
 msgid "Effective"
 msgstr "Eficaz"
 
-msgid "Email"
-msgstr "Correo electrónico"
-
-msgid "Email address"
-msgstr "Dirección de correo electrónico"
-
 msgid "English"
 msgstr "Inglés"
 
 msgid ""
 "Error -  Indicates rejection of the message(s) identified in references; "
 "explanation SHOULD appear in note field"
 msgstr ""
@@ -178,85 +163,79 @@
 msgid ""
 "Exercise - Actionable only by designated exercise participants; exercise "
 "identifier SHOULD appear in note"
 msgstr ""
 "Ejercicio: procesable solo por los participantes designados del ejercicio; "
 "el identificador del ejercicio DEBE aparecer en la nota"
 
-msgid "Expected"
-msgstr "Esperado"
-
 msgid "Expected - Responsive action SHOULD be taken soon (within next hour)"
 msgstr ""
 "Esperado: la acción de respuesta DEBE tomarse pronto (dentro de la próxima "
 "hora)"
 
 msgid "Expires"
 msgstr "Caduca"
 
 msgid "Extreme - Extraordinary threat to life or property"
 msgstr "Extremo: amenaza extraordinaria para la vida o la propiedad"
 
-msgid "File"
-msgstr "Archivo"
-
-msgid "File, Document etc"
-msgstr "archivo, documento, etc."
-
 msgid "Fire suppression and rescue"
 msgstr "Extinción de incendios y salvamento"
 
-msgid "Future"
-msgstr "Futuro"
-
 msgid "Future - Responsive action SHOULD be taken in the near future"
 msgstr "Futuro: se DEBERÍA tomar medidas de respuesta en un futuro próximo"
 
 msgid "General emergency and public safety"
 msgstr "Emergencia general y seguridad ciudadana"
 
+msgid "Geocode"
+msgstr "Geocodificar"
+
 msgid "Geophysical"
 msgstr "Geofísico"
 
+msgid "Hazard"
+msgstr "Peligro"
+
+msgid "Hazards monitored by the institution"
+msgstr "Peligros monitoreados por la institución"
+
 msgid "Headline"
 msgstr "Titular"
 
-msgid ""
-"How many of this products should be visible on the landing page filter "
-"section ?"
-msgstr ""
-"¿Cuántos de estos productos deberían estar visibles en la sección de filtro "
-"de la página de destino?"
-
 msgid "Identifier"
 msgstr "identificador"
 
-msgid "Immediate"
-msgstr "Inmediato"
-
 msgid "Immediate - Responsive action SHOULD be taken immediately"
 msgstr "Inmediato: la acción de respuesta DEBE tomarse de inmediato"
 
+msgid "Incident"
+msgstr "Incidente"
+
+msgid "Incidents"
+msgstr "incidentes"
+
 msgid "Instruction"
 msgstr "Instrucción"
 
-msgid "Intended Recipients (If scope is Private) "
-msgstr "Destinatarios previstos (si el ámbito es privado)"
-
 msgid "Language"
 msgstr "Idioma"
 
 msgid "Law enforcement, military, homeland and local/private security"
 msgstr "Aplicación de la ley, militar, nacional y seguridad local/privada"
 
 msgid "Likely - Likely (percentage > ~50%)"
 msgstr "Probable - Probable (porcentaje > ~50%)"
 
-msgid "Link"
-msgstr "Enlace"
+msgid ""
+"Link to external resource. This can be for example a link to related "
+"websites. "
+msgstr ""
+"Enlace a recurso externo. Esto puede ser, por ejemplo, un enlace a sitios "
+"web relacionados."
 
 msgid "Medical and public health"
 msgstr "Médico y salud pública"
 
 msgid "Message Type"
 msgstr "Tipo de mensaje"
 
@@ -276,17 +255,14 @@
 
 msgid "Name"
 msgstr "Nombre"
 
 msgid "Name for the event code"
 msgstr "Nombre para el código de evento"
 
-msgid "Name for the geocode"
-msgstr "Nombre para el código geográfico"
-
 msgid "Name of the recipient"
 msgstr "Nombre del destinatario"
 
 msgid "No action recommended"
 msgstr "No se recomienda ninguna acción"
 
 msgid "Note"
@@ -297,23 +273,29 @@
 
 msgid "Onset"
 msgstr "Comienzo"
 
 msgid "Other events"
 msgstr "Otros eventos"
 
-msgid "Past"
-msgstr "Pasado"
+msgid "Parameter"
+msgstr "Parámetro"
+
+msgid "Parameters"
+msgstr "Parámetros"
 
 msgid "Past - Responsive action is no longer required"
 msgstr "Pasado: la acción de respuesta ya no es necesaria"
 
 msgid "Pollution and other environmental"
 msgstr "Contaminación y otros ambientales."
 
+msgid "Polygon"
+msgstr "Polígono"
+
 msgid "Possible - Possible but not likely (percentage <= ~50%)"
 msgstr "Posible - Posible pero no probable (porcentaje <= ~50%)"
 
 msgid "Prepare - Relocate as instructed in the instruction"
 msgstr "Preparar - Reubicar como se indica en las instrucciones"
 
 msgid ""
@@ -334,20 +316,14 @@
 
 msgid "Reference Alert"
 msgstr "Alerta de referencia"
 
 msgid "Rescue and recovery"
 msgstr "Rescate y recuperación"
 
-msgid "Resource"
-msgstr "Recurso"
-
-msgid "Resource type whether is image, file etc"
-msgstr "Tipo de recurso, ya sea imagen, archivo, etc."
-
 msgid "Response type"
 msgstr "Tipo de respuesta"
 
 msgid ""
 "Restricted - For dissemination only to users with a known operational "
 "requirement as in the restriction field"
 msgstr ""
@@ -380,20 +356,20 @@
 
 msgid "Status"
 msgstr "Estado"
 
 msgid "System - For messages that support alert network internal functions"
 msgstr "Sistema: para mensajes que admiten funciones internas de red de alerta"
 
+msgid "Target audiences for published alerts"
+msgstr "Audiencias objetivo para las alertas publicadas"
+
 msgid "Test - Technical testing only, all recipients disregard"
 msgstr "Prueba: solo prueba técnica, todos los destinatarios ignoran"
 
-msgid "The base-64 encoded data content of the resource file"
-msgstr "El contenido de datos codificados en base 64 del archivo de recursos"
-
 msgid "The code denoting the appropriate handling of the alert"
 msgstr "El código que indica el manejo adecuado de la alerta."
 
 msgid ""
 "The code denoting the category of the subject event of the alert message"
 msgstr ""
 "El código que indica la categoría del evento sujeto del mensaje de alerta."
@@ -427,40 +403,31 @@
 "El código que indica el tipo de acción recomendada para el público objetivo"
 
 msgid "The code denoting the urgency of the subject event of the alert message"
 msgstr ""
 "El código que indica la urgencia del evento sujeto del mensaje de alerta."
 
 msgid ""
-"The code representing the digital digest ('hash') computed from the resource "
-"file"
-msgstr ""
-"El código que representa el resumen digital ('hash') calculado a partir del "
-"archivo de recursos"
-
-msgid "The effective time of the information of the alert message"
-msgstr "El tiempo efectivo de la información del mensaje de alerta."
-
-msgid ""
 "The expected time of the beginning of the subject event of the alert message"
 msgstr ""
 "La hora prevista del comienzo del evento de asunto del mensaje de alerta."
 
-msgid "The expiry time of the information of the alert message"
-msgstr "El tiempo de caducidad de la información del mensaje de alerta."
-
 msgid ""
-"The identifier of the hyperlink associating additional information with the "
-"alert message"
+"The expiry time of the information of the alert message. If not set, each "
+"recipient is free to set its own policy as to when the message is no longer "
+"in effect."
 msgstr ""
-"El identificador del hipervínculo que asocia información adicional con el "
-"mensaje de alerta."
+"El tiempo de caducidad de la información del mensaje de alerta. Si no se "
+"establece, cada destinatario es libre de establecer su propia política en "
+"cuanto a cuándo el mensaje ya no está en vigor."
 
-msgid "The identifier of the hyperlink for the resource file"
-msgstr "El identificador del hipervínculo para el archivo de recursos."
+msgid "The human-readable name of the agency or authority issuing this alert."
+msgstr ""
+"El nombre legible por humanos de la agencia o autoridad que emite esta "
+"alerta."
 
 msgid ""
 "The maximum altitude of the affected area of the alert message.MUST NOT be "
 "used except in combination with the altitude element. "
 msgstr ""
 "La altitud máxima del área afectada del mensaje de alerta. NO DEBE usarse "
 "excepto en combinación con el elemento de altitud."
@@ -512,72 +479,51 @@
 msgid ""
 "The text describing the rule for limiting distribution of the restricted "
 "alert message. Used when scope value is Restricted"
 msgstr ""
 "El texto que describe la regla para limitar la distribución del mensaje de "
 "alerta restringida. Se usa cuando el valor del alcance está restringido"
 
-msgid "The text describing the subject event of the alert message"
-msgstr "El texto que describe el evento de asunto del mensaje de alerta."
-
 msgid "The text describing the type and content of the resource file"
 msgstr "El texto que describe el tipo y el contenido del archivo de recursos."
 
-msgid "The text headline of the alert message"
-msgstr "El título de texto del mensaje de alerta."
+msgid ""
+"The text headline of the alert message. Make it direct and actionable as "
+"possible while remaining short"
+msgstr ""
+"El título de texto del mensaje de alerta. Hágalo lo más directo y procesable "
+"posible sin dejar de ser corto."
 
 msgid "The text identifying the source of the alert message"
 msgstr "El texto que identifica la fuente del mensaje de alerta."
 
 msgid "Time and date of origination of the alert"
 msgstr "Hora y fecha de origen de la alerta"
 
-msgid "Title"
-msgstr "Título"
-
-msgid "Title of the incident referent of the alert"
-msgstr "Título del incidente referente de la alerta"
-
 msgid "Unique ID. Auto generated on creation."
 msgstr "Identificación única. Generado automáticamente en la creación."
 
-msgid "Unknown"
-msgstr "Desconocido"
-
 msgid "Unknown - Certainty unknown"
 msgstr "Desconocido - Certeza desconocida"
 
 msgid "Unknown - Severity unknown"
 msgstr "Desconocido: gravedad desconocida"
 
 msgid "Unknown - Urgency not known"
 msgstr "Desconocido - Urgencia no conocida"
 
 msgid "Unlikely - Not expected to occur (percentage ~ 0)"
 msgstr "Improbable: no se espera que ocurra (porcentaje ~ 0)"
 
-msgid ""
-"Update - Updates and supercedes the earlier message(s) identified in "
-"referenced alerts"
-msgstr ""
-"Actualizar: actualiza y reemplaza los mensajes anteriores identificados en "
-"las alertas a las que se hace referencia"
-
 msgid "Urgency"
 msgstr "Urgencia"
 
 msgid "Utility, telecommunication, other non-transport infrastructure"
 msgstr ""
 "Servicios públicos, telecomunicaciones, otra infraestructura no relacionada "
 "con el transporte"
 
 msgid "Value"
 msgstr "Valor"
 
 msgid "Value of the event code"
 msgstr "Valor del código de evento"
-
-msgid "Value of the geocode"
-msgstr "Valor del geocódigo"
-
-msgid "Web"
-msgstr "Web"
```

### Comparing `capeditor-0.2.7/capeditor/locale/es/LC_MESSAGES/django.po` & `capeditor-0.2.8/capeditor/locale/es/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-12 14:01+0300\n"
+"POT-Creation-Date: 2023-07-14 12:05+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: capeditor/blocks.py:70 capeditor/blocks.py:98 capeditor/blocks.py:370
+#: capeditor/blocks.py:70 capeditor/blocks.py:98 capeditor/blocks.py:375
 msgid "Name"
 msgstr "Nombre"
 
 #: capeditor/blocks.py:70
 msgid "Name of the recipient"
 msgstr "Nombre del destinatario"
 
@@ -52,15 +52,15 @@
 
 #: capeditor/blocks.py:94
 #, fuzzy
 #| msgid "The text headline of the alert message"
 msgid "Referent incident to this alert message"
 msgstr "Incidente referente a este mensaje de alerta"
 
-#: capeditor/blocks.py:99 capeditor/blocks.py:295 capeditor/blocks.py:371
+#: capeditor/blocks.py:99 capeditor/blocks.py:300 capeditor/blocks.py:376
 msgid "Value"
 msgstr "Valor"
 
 #: capeditor/blocks.py:104
 msgid "Shelter - Take shelter in place or per instruction"
 msgstr "Refugio: refúgiese en el lugar o según las instrucciones"
 
@@ -115,461 +115,461 @@
 
 #: capeditor/blocks.py:117
 msgid ""
 "The code denoting the type of action recommended for the target audience"
 msgstr ""
 "El código que indica el tipo de acción recomendada para el público objetivo"
 
-#: capeditor/blocks.py:158 capeditor/blocks.py:204 capeditor/blocks.py:256
-#: capeditor/blocks.py:292
+#: capeditor/blocks.py:163 capeditor/blocks.py:209 capeditor/blocks.py:261
+#: capeditor/blocks.py:297
 msgid "Affected areas / Regions"
 msgstr "Áreas / Regiones afectadas"
 
-#: capeditor/blocks.py:159 capeditor/blocks.py:205 capeditor/blocks.py:257
-#: capeditor/blocks.py:293
+#: capeditor/blocks.py:164 capeditor/blocks.py:210 capeditor/blocks.py:262
+#: capeditor/blocks.py:298
 msgid "The text describing the affected area of the alert message"
 msgstr "El texto que describe el área afectada del mensaje de alerta."
 
-#: capeditor/blocks.py:160
+#: capeditor/blocks.py:165
 msgid "Administrative Level"
 msgstr "Nivel Administrativo"
 
-#: capeditor/blocks.py:161
+#: capeditor/blocks.py:166
 msgid "Boundary"
 msgstr "Perímetro"
 
-#: capeditor/blocks.py:162 capeditor/blocks.py:207
+#: capeditor/blocks.py:167 capeditor/blocks.py:212
 msgid ""
 "The paired values of points defining a polygon that delineates the affected "
 "area of the alert message"
 msgstr ""
 "Los valores emparejados de puntos que definen un polígono que delimita el "
 "área afectada del mensaje de alerta"
 
-#: capeditor/blocks.py:165 capeditor/blocks.py:209 capeditor/blocks.py:260
-#: capeditor/blocks.py:297
+#: capeditor/blocks.py:170 capeditor/blocks.py:214 capeditor/blocks.py:265
+#: capeditor/blocks.py:302
 msgid "Altitude"
 msgstr "Altitud"
 
-#: capeditor/blocks.py:166 capeditor/blocks.py:210 capeditor/blocks.py:261
-#: capeditor/blocks.py:298
+#: capeditor/blocks.py:171 capeditor/blocks.py:215 capeditor/blocks.py:266
+#: capeditor/blocks.py:303
 msgid ""
 "The specific or minimum altitude of the affected area of the alert message"
 msgstr ""
 "La altitud específica o mínima del área afectada del mensaje de alerta."
 
-#: capeditor/blocks.py:168 capeditor/blocks.py:212 capeditor/blocks.py:263
-#: capeditor/blocks.py:300
+#: capeditor/blocks.py:173 capeditor/blocks.py:217 capeditor/blocks.py:268
+#: capeditor/blocks.py:305
 msgid "Ceiling"
 msgstr "Techo"
 
-#: capeditor/blocks.py:169 capeditor/blocks.py:213 capeditor/blocks.py:264
-#: capeditor/blocks.py:301
+#: capeditor/blocks.py:174 capeditor/blocks.py:218 capeditor/blocks.py:269
+#: capeditor/blocks.py:306
 msgid ""
 "The maximum altitude of the affected area of the alert message.MUST NOT be "
 "used except in combination with the altitude element. "
 msgstr ""
 "La altitud máxima del área afectada del mensaje de alerta. NO DEBE usarse "
 "excepto en combinación con el elemento de altitud."
 
-#: capeditor/blocks.py:206
+#: capeditor/blocks.py:211
 msgid "Polygon"
 msgstr "Polígono"
 
-#: capeditor/blocks.py:258 capeditor/blocks.py:528
+#: capeditor/blocks.py:263 capeditor/blocks.py:555
 msgid "Circle"
 msgstr "Círculo"
 
-#: capeditor/blocks.py:258
+#: capeditor/blocks.py:263
 msgid "Drag the marker to change position"
 msgstr "Arrastra el marcador para cambiar de posición"
 
-#: capeditor/blocks.py:305
+#: capeditor/blocks.py:310
 msgid "The human-readable name of the agency or authority issuing this alert."
 msgstr ""
 "El nombre legible por humanos de la agencia o autoridad que emite esta "
 "alerta."
 
-#: capeditor/blocks.py:306
+#: capeditor/blocks.py:311
 msgid ""
 "The text describing the contact for follow-up and confirmation of the alert "
 "message"
 msgstr ""
 "El texto que describe el contacto para el seguimiento y confirmación del "
 "mensaje de alerta."
 
-#: capeditor/blocks.py:307
+#: capeditor/blocks.py:312
 msgid "The text denoting the type of the subject event of the alert message"
 msgstr ""
 "El texto que indica el tipo de evento de asunto del mensaje de alerta."
 
-#: capeditor/blocks.py:308
+#: capeditor/blocks.py:313
 msgid "The text describing the intended audience of the alert message"
 msgstr "El texto que describe la audiencia prevista del mensaje de alerta."
 
-#: capeditor/blocks.py:350 capeditor/blocks.py:359
+#: capeditor/blocks.py:355 capeditor/blocks.py:364
 #, fuzzy
 #| msgid "Description"
 msgid "Resource Description"
 msgstr "Descripción del recurso"
 
-#: capeditor/blocks.py:351 capeditor/blocks.py:360
+#: capeditor/blocks.py:356 capeditor/blocks.py:365
 msgid "The text describing the type and content of the resource file"
 msgstr "El texto que describe el tipo y el contenido del archivo de recursos."
 
-#: capeditor/blocks.py:361
+#: capeditor/blocks.py:366
 #, fuzzy
 #| msgid "Alert Resources "
 msgid "External Resource Link"
 msgstr "Enlace de recurso externo"
 
-#: capeditor/blocks.py:362
+#: capeditor/blocks.py:367
 msgid ""
 "Link to external resource. This can be for example a link to related "
 "websites. "
 msgstr ""
 "Enlace a recurso externo. Esto puede ser, por ejemplo, un enlace a sitios "
 "web relacionados."
 
-#: capeditor/blocks.py:370
+#: capeditor/blocks.py:375
 msgid "Name for the event code"
 msgstr "Nombre para el código de evento"
 
-#: capeditor/blocks.py:371
+#: capeditor/blocks.py:376
 msgid "Value of the event code"
 msgstr "Valor del código de evento"
 
-#: capeditor/blocks.py:441
+#: capeditor/blocks.py:467
 msgid "English"
 msgstr "Inglés"
 
-#: capeditor/blocks.py:445
+#: capeditor/blocks.py:471
 msgid "Geophysical"
 msgstr "Geofísico"
 
-#: capeditor/blocks.py:446
+#: capeditor/blocks.py:472
 msgid "Meteorological"
 msgstr "Meteorológico"
 
-#: capeditor/blocks.py:447
+#: capeditor/blocks.py:473
 msgid "General emergency and public safety"
 msgstr "Emergencia general y seguridad ciudadana"
 
-#: capeditor/blocks.py:448
+#: capeditor/blocks.py:474
 msgid "Law enforcement, military, homeland and local/private security"
 msgstr "Aplicación de la ley, militar, nacional y seguridad local/privada"
 
-#: capeditor/blocks.py:449
+#: capeditor/blocks.py:475
 msgid "Rescue and recovery"
 msgstr "Rescate y recuperación"
 
-#: capeditor/blocks.py:450
+#: capeditor/blocks.py:476
 msgid "Fire suppression and rescue"
 msgstr "Extinción de incendios y salvamento"
 
-#: capeditor/blocks.py:451
+#: capeditor/blocks.py:477
 msgid "Medical and public health"
 msgstr "Médico y salud pública"
 
-#: capeditor/blocks.py:452
+#: capeditor/blocks.py:478
 msgid "Pollution and other environmental"
 msgstr "Contaminación y otros ambientales."
 
-#: capeditor/blocks.py:453
+#: capeditor/blocks.py:479
 msgid "Public and private transportation"
 msgstr "Transporte publico y privado"
 
-#: capeditor/blocks.py:454
+#: capeditor/blocks.py:480
 msgid "Utility, telecommunication, other non-transport infrastructure"
 msgstr ""
 "Servicios públicos, telecomunicaciones, otra infraestructura no relacionada "
 "con el transporte"
 
-#: capeditor/blocks.py:455
+#: capeditor/blocks.py:481
 msgid ""
 "Chemical, Biological, Radiological, Nuclear or High-Yield Explosive threat "
 "or attack"
 msgstr ""
 "Amenaza o ataque químico, biológico, radiológico, nuclear o explosivo de "
 "alto rendimiento"
 
-#: capeditor/blocks.py:456
+#: capeditor/blocks.py:482
 msgid "Other events"
 msgstr "Otros eventos"
 
-#: capeditor/blocks.py:460
+#: capeditor/blocks.py:486
 msgid "Immediate - Responsive action SHOULD be taken immediately"
 msgstr "Inmediato: la acción de respuesta DEBE tomarse de inmediato"
 
-#: capeditor/blocks.py:461
+#: capeditor/blocks.py:487
 msgid "Expected - Responsive action SHOULD be taken soon (within next hour)"
 msgstr ""
 "Esperado: la acción de respuesta DEBE tomarse pronto (dentro de la próxima "
 "hora)"
 
-#: capeditor/blocks.py:462
+#: capeditor/blocks.py:488
 msgid "Future - Responsive action SHOULD be taken in the near future"
 msgstr "Futuro: se DEBERÍA tomar medidas de respuesta en un futuro próximo"
 
-#: capeditor/blocks.py:463
+#: capeditor/blocks.py:489
 msgid "Past - Responsive action is no longer required"
 msgstr "Pasado: la acción de respuesta ya no es necesaria"
 
-#: capeditor/blocks.py:464
+#: capeditor/blocks.py:490
 msgid "Unknown - Urgency not known"
 msgstr "Desconocido - Urgencia no conocida"
 
-#: capeditor/blocks.py:468
+#: capeditor/blocks.py:494
 msgid "Extreme - Extraordinary threat to life or property"
 msgstr "Extremo: amenaza extraordinaria para la vida o la propiedad"
 
-#: capeditor/blocks.py:469
+#: capeditor/blocks.py:495
 msgid "Severe - Significant threat to life or property"
 msgstr "Grave: amenaza importante para la vida o la propiedad"
 
-#: capeditor/blocks.py:470
+#: capeditor/blocks.py:496
 msgid "Moderate - Possible threat to life or property"
 msgstr "Moderado: posible amenaza para la vida o la propiedad"
 
-#: capeditor/blocks.py:471
+#: capeditor/blocks.py:497
 msgid "Minor - Minimal to no known threat to life or property"
 msgstr "Menor: mínima o ninguna amenaza conocida para la vida o la propiedad"
 
-#: capeditor/blocks.py:472
+#: capeditor/blocks.py:498
 msgid "Unknown - Severity unknown"
 msgstr "Desconocido: gravedad desconocida"
 
-#: capeditor/blocks.py:476
+#: capeditor/blocks.py:502
 msgid "Observed - Determined to have occurred or to be ongoing"
 msgstr "Observado - Determinado que ha ocurrido o que está en curso"
 
-#: capeditor/blocks.py:477
+#: capeditor/blocks.py:503
 msgid "Likely - Likely (percentage > ~50%)"
 msgstr "Probable - Probable (porcentaje > ~50%)"
 
-#: capeditor/blocks.py:478
+#: capeditor/blocks.py:504
 msgid "Possible - Possible but not likely (percentage <= ~50%)"
 msgstr "Posible - Posible pero no probable (porcentaje <= ~50%)"
 
-#: capeditor/blocks.py:479
+#: capeditor/blocks.py:505
 msgid "Unlikely - Not expected to occur (percentage ~ 0)"
 msgstr "Improbable: no se espera que ocurra (porcentaje ~ 0)"
 
-#: capeditor/blocks.py:480
+#: capeditor/blocks.py:506
 msgid "Unknown - Certainty unknown"
 msgstr "Desconocido - Certeza desconocida"
 
-#: capeditor/blocks.py:483
-msgid "Language"
-msgstr "Idioma"
-
-#: capeditor/blocks.py:484
-msgid "The code denoting the language of the alert message"
-msgstr "El código que indica el idioma del mensaje de alerta."
+#: capeditor/blocks.py:508
+msgid "Event"
+msgstr "Evento"
 
-#: capeditor/blocks.py:485
+#: capeditor/blocks.py:510
 msgid "Category"
 msgstr "Categoría"
 
-#: capeditor/blocks.py:486
+#: capeditor/blocks.py:511
 msgid ""
 "The code denoting the category of the subject event of the alert message"
 msgstr ""
 "El código que indica la categoría del evento sujeto del mensaje de alerta."
 
-#: capeditor/blocks.py:488
-msgid "Event"
-msgstr "Evento"
+#: capeditor/blocks.py:513
+msgid "Language"
+msgstr "Idioma"
 
-#: capeditor/blocks.py:489
+#: capeditor/blocks.py:514
+msgid "The code denoting the language of the alert message"
+msgstr "El código que indica el idioma del mensaje de alerta."
+
+#: capeditor/blocks.py:516
 msgid "Urgency"
 msgstr "Urgencia"
 
-#: capeditor/blocks.py:490
+#: capeditor/blocks.py:517
 msgid ""
 "The code denoting the urgency of the subject event of the alert message"
 msgstr ""
 "El código que indica la urgencia del evento sujeto del mensaje de alerta."
 
-#: capeditor/blocks.py:492
+#: capeditor/blocks.py:519
 msgid "Severity"
 msgstr "Gravedad"
 
-#: capeditor/blocks.py:493
+#: capeditor/blocks.py:520
 msgid ""
 "The code denoting the severity of the subject event of the alert message"
 msgstr ""
 "El código que indica la gravedad del evento en cuestión del mensaje de "
 "alerta."
 
-#: capeditor/blocks.py:495
+#: capeditor/blocks.py:522
 msgid "Certainty"
 msgstr "Certeza"
 
-#: capeditor/blocks.py:496
+#: capeditor/blocks.py:523
 msgid ""
 "The code denoting the certainty of the subject event of the alert message"
 msgstr ""
 "El código que indica la certeza del evento sujeto del mensaje de alerta."
 
-#: capeditor/blocks.py:498
+#: capeditor/blocks.py:525
 msgid "Headline"
 msgstr "Titular"
 
-#: capeditor/blocks.py:499
+#: capeditor/blocks.py:526
 msgid ""
 "The text headline of the alert message. Make it direct and actionable as "
 "possible while remaining short"
 msgstr ""
 "El título de texto del mensaje de alerta. Hágalo lo más directo y procesable"
 " posible sin dejar de ser corto."
 
-#: capeditor/blocks.py:501
+#: capeditor/blocks.py:528
 msgid "Description"
 msgstr "Descripción"
 
-#: capeditor/blocks.py:503
+#: capeditor/blocks.py:530
 #, fuzzy
 #| msgid "The text describing the subject event of the alert message"
 msgid ""
 "The text describing the subject event of the alert message. An extended "
 "description of the hazard or event that occasioned this message"
 msgstr ""
 "El texto que describe el evento de asunto del mensaje de alerta. Una "
 "descripción detallada del peligro o evento que ocasionó este mensaje"
 
-#: capeditor/blocks.py:505
+#: capeditor/blocks.py:532
 msgid "Instruction"
 msgstr "Instrucción"
 
-#: capeditor/blocks.py:506
+#: capeditor/blocks.py:533
 msgid ""
 "The text describing the recommended action to be taken by recipients of the "
 "alert message"
 msgstr ""
 "El texto que describe la acción recomendada que deben tomar los "
 "destinatarios del mensaje de alerta."
 
-#: capeditor/blocks.py:508
+#: capeditor/blocks.py:535
 msgid "Effective"
 msgstr "Eficaz"
 
-#: capeditor/blocks.py:509
+#: capeditor/blocks.py:536
 #, fuzzy
 #| msgid "The effective time of the information of the alert message"
 msgid ""
 "The effective time of the information of the alert message. If not set, the "
 "sent date will be used"
 msgstr ""
 "El tiempo efectivo de la información del mensaje de alerta. Si no se "
 "establece, se utilizará la fecha de envío"
 
-#: capeditor/blocks.py:511
+#: capeditor/blocks.py:538
 msgid "Onset"
 msgstr "Comienzo"
 
-#: capeditor/blocks.py:512
+#: capeditor/blocks.py:539
 msgid ""
 "The expected time of the beginning of the subject event of the alert message"
 msgstr ""
 "La hora prevista del comienzo del evento de asunto del mensaje de alerta."
 
-#: capeditor/blocks.py:514
+#: capeditor/blocks.py:541
 msgid "Expires"
 msgstr "Caduca"
 
-#: capeditor/blocks.py:515
+#: capeditor/blocks.py:542
 msgid ""
 "The expiry time of the information of the alert message. If not set, each "
 "recipient is free to set its own policy as to when the message is no longer "
 "in effect."
 msgstr ""
 "El tiempo de caducidad de la información del mensaje de alerta. Si no se "
 "establece, cada destinatario es libre de establecer su propia política en "
 "cuanto a cuándo el mensaje ya no está en vigor."
 
-#: capeditor/blocks.py:518
+#: capeditor/blocks.py:545
 #, fuzzy
 #| msgid "Response type"
 msgid "Response Types"
 msgstr "Tipos de respuesta"
 
-#: capeditor/blocks.py:520
+#: capeditor/blocks.py:547
 #, fuzzy
 #| msgid "Sender"
 msgid "Sender name"
 msgstr "Nombre del remitente"
 
-#: capeditor/blocks.py:522
+#: capeditor/blocks.py:549
 msgid "Contact"
 msgstr "Contacto"
 
-#: capeditor/blocks.py:523 capeditor/blocks.py:550
+#: capeditor/blocks.py:550 capeditor/blocks.py:580
 msgid "Audience"
 msgstr "Audiencia"
 
-#: capeditor/blocks.py:526
+#: capeditor/blocks.py:553
 msgid "Admin Boundary"
 msgstr "Límite de administración"
 
-#: capeditor/blocks.py:527
+#: capeditor/blocks.py:554
 msgid "Draw Polygon"
 msgstr "dibujar polígono"
 
-#: capeditor/blocks.py:529
+#: capeditor/blocks.py:556
 msgid "Geocode"
 msgstr "Geocodificar"
 
-#: capeditor/blocks.py:530
+#: capeditor/blocks.py:557
 msgid "Alert Area"
 msgstr "Área de alerta"
 
-#: capeditor/blocks.py:530
+#: capeditor/blocks.py:557
 msgid "Admin Boundary, Polygon, Circle or Geocode"
 msgstr "Límite de administrador, polígono, círculo o código geográfico"
 
-#: capeditor/blocks.py:535
+#: capeditor/blocks.py:562
 #, fuzzy
 #| msgid "Resource"
 msgid "Resources"
 msgstr "Recursos"
 
-#: capeditor/blocks.py:535
+#: capeditor/blocks.py:562
 msgid ""
 "Additional file with supplemental information related to this alert "
 "information"
 msgstr ""
 "Archivo adicional con información complementaria relacionada con esta "
 "información de alerta"
 
-#: capeditor/blocks.py:538
+#: capeditor/blocks.py:565
 msgid "Parameter"
 msgstr "Parámetro"
 
-#: capeditor/blocks.py:538
+#: capeditor/blocks.py:565
 msgid "Parameters"
 msgstr "Parámetros"
 
-#: capeditor/blocks.py:539
+#: capeditor/blocks.py:566
 #, fuzzy
 #| msgid "Event"
 msgid "Event Code"
 msgstr "Código de evento"
 
-#: capeditor/blocks.py:539
+#: capeditor/blocks.py:566
 #, fuzzy
 #| msgid "Event"
 msgid "Event codes"
-msgstr "Códigos de evento"
+msgstr "Códigos de eventos"
 
-#: capeditor/blocks.py:545
+#: capeditor/blocks.py:575
 msgid "Hazard"
 msgstr "Peligro"
 
-#: capeditor/blocks.py:554
+#: capeditor/blocks.py:584
 #, fuzzy
 #| msgid "Contact"
 msgid "Contact Detail"
 msgstr "Detalles del contacto"
 
 #: capeditor/models.py:35
 #, fuzzy
```

### Comparing `capeditor-0.2.7/capeditor/locale/fr/LC_MESSAGES/django.mo` & `capeditor-0.2.8/capeditor/locale/fr/LC_MESSAGES/django.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,102 +8,88 @@
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 msgid ""
-" Identifies the originator of an alert. This can be an email of the "
-"institution for example"
-msgstr ""
-"Identifie l'origine d'une alerte. Cela peut être un email de l'institution "
-"par exemple"
-
-msgid ""
 "Acknowledge - Acknowledges receipt and acceptance of the message(s) "
 "identified in references field"
 msgstr ""
 "Accusé de réception - Accusé de réception et d'acceptation du ou des "
 "messages identifiés dans le champ des références"
 
 msgid "Actual - Actionable by all targeted recipients"
 msgstr "Réel - Actionnable par tous les destinataires ciblés"
 
+msgid ""
+"Additional file with supplemental information related to this alert "
+"information"
+msgstr ""
+"Fichier supplémentaire avec des informations supplémentaires liées à cette "
+"information d'alerte"
+
+msgid "Addresses"
+msgstr "Adresses"
+
+msgid "Admin Boundary"
+msgstr "Limite administrative"
+
+msgid "Admin Boundary, Polygon, Circle or Geocode"
+msgstr "Limite administrative, Polygone, Cercle ou Géocode"
+
+msgid "Administrative Level"
+msgstr "Niveau administratif"
+
 msgid "Affected areas / Regions"
 msgstr "Zones / Régions touchées"
 
-msgid "Alert"
-msgstr "Alerte"
-
 msgid "Alert - Initial information requiring attention by targeted recipients"
 msgstr ""
 "Alerte - Information initiale nécessitant l'attention des destinataires "
 "ciblés"
 
 msgid "Alert Area"
 msgstr "Zone d'alerte"
 
-msgid "Alert Areas "
-msgstr "Zones d'alerte"
-
-msgid ""
-"Alert Categorization (Category, Urgency, Severity, Certainity, Response & "
-"Dates)"
-msgstr ""
-"Catégorisation des alertes (catégorie, urgence, gravité, certitude, réponse "
-"et dates)"
-
-msgid ""
-"Alert Delivery Message (Headline, Description, Intsructions, Contact & "
-"Website)"
-msgstr ""
-"Message de livraison d'alerte (titre, description, instructions, contact et "
-"site Web)"
-
-msgid "Alert Identification (Sender, Message Type, Scope)"
-msgstr "Identification de l'alerte (expéditeur, type de message, portée)"
-
-msgid "Alert Info"
-msgstr "Informations d'alerte"
-
 msgid "Alert Information"
 msgstr "Informations d'alerte"
 
-msgid "Alert Resources "
-msgstr "Ressources d'alerte"
-
-msgid "Alerts Per Page"
-msgstr "Alertes par page"
-
 msgid ""
 "All Clear - The subject event no longer poses a threat or concern and any "
 "follow on action is described in instruction"
 msgstr ""
 "Tout est clair - L'événement en question ne constitue plus une menace ou une "
 "préoccupation et toute action de suivi est décrite dans les instructions"
 
 msgid "Altitude"
 msgstr "Altitude"
 
-msgid "Area"
-msgstr "Zone"
-
 msgid ""
 "Assess - Evaluate the information in this message - DONT USE FOR PUBLIC "
 "ALERTS"
 msgstr ""
 "Évaluer - Évaluez les informations contenues dans ce message - NE PAS "
 "UTILISER POUR LES ALERTES PUBLIQUES"
 
 msgid "Audience"
 msgstr "Public"
 
 msgid "Avoid - Avoid the subject event as per the instruction"
 msgstr "Éviter - Éviter l'événement sujet selon les instructions"
 
+msgid "Boundary"
+msgstr "Frontière"
+
+msgid "CAP Sender Name"
+msgstr "Nom de l'expéditeur CAP"
+
+msgid "Can be the website link or email of the sending institution"
+msgstr "Peut être le lien du site Web ou l'e-mail de l'institution d'envoi"
+
 msgid "Cancel - Cancels the earlier message(s) identified in references"
 msgstr ""
 "Annuler - Annule le(s) message(s) antérieur(s) identifié(s) dans les "
 "références"
 
 msgid "Category"
 msgstr "Catégorie"
@@ -117,47 +103,44 @@
 msgid ""
 "Chemical, Biological, Radiological, Nuclear or High-Yield Explosive threat "
 "or attack"
 msgstr ""
 "Menace ou attaque chimique, biologique, radiologique, nucléaire ou explosive "
 "à haut rendement"
 
+msgid "Circle"
+msgstr "Cercle"
+
 msgid "Code"
 msgstr "Code"
 
 msgid "Contact"
 msgstr "Contact"
 
 msgid "Description"
 msgstr "Description"
 
-msgid "Description of the incident"
-msgstr "Description de l'incident"
-
 msgid ""
 "Draft - A preliminary template or draft, not actionable in its current form"
 msgstr ""
 "Brouillon - Un modèle ou un brouillon préliminaire, non exploitable dans sa "
 "forme actuelle"
 
-msgid "Earlier Reference Alerts -  If applicable"
-msgstr "Alertes de référence antérieures - Le cas échéant"
+msgid "Drag the marker to change position"
+msgstr "Faites glisser le marqueur pour changer de position"
+
+msgid "Draw Polygon"
+msgstr "Dessiner un polygone"
 
 msgid "Earlier alert referenced by this alert"
 msgstr "Alerte antérieure référencée par cette alerte"
 
 msgid "Effective"
 msgstr "Efficace"
 
-msgid "Email"
-msgstr "E-mail"
-
-msgid "Email address"
-msgstr "Adresse e-mail"
-
 msgid "English"
 msgstr "Anglais"
 
 msgid ""
 "Error -  Indicates rejection of the message(s) identified in references; "
 "explanation SHOULD appear in note field"
 msgstr ""
@@ -177,86 +160,80 @@
 msgid ""
 "Exercise - Actionable only by designated exercise participants; exercise "
 "identifier SHOULD appear in note"
 msgstr ""
 "Exercice - Actionnable uniquement par les participants désignés à "
 "l'exercice ; l'identifiant de l'exercice DOIT apparaître dans la note"
 
-msgid "Expected"
-msgstr "Attendu"
-
 msgid "Expected - Responsive action SHOULD be taken soon (within next hour)"
 msgstr ""
 "Attendu - Une action réactive DEVRAIT être entreprise rapidement (dans "
 "l'heure qui suit)"
 
 msgid "Expires"
 msgstr "Expire"
 
 msgid "Extreme - Extraordinary threat to life or property"
 msgstr "Extrême - Menace extraordinaire pour la vie ou la propriété"
 
-msgid "File"
-msgstr "Déposer"
-
-msgid "File, Document etc"
-msgstr "Fichier, document, etc."
-
 msgid "Fire suppression and rescue"
 msgstr "Lutte contre les incendies et sauvetage"
 
-msgid "Future"
-msgstr "Avenir"
-
 msgid "Future - Responsive action SHOULD be taken in the near future"
 msgstr ""
 "Futur - Des mesures réactives DOIVENT être prises dans un proche avenir"
 
 msgid "General emergency and public safety"
 msgstr "Urgence générale et sécurité publique"
 
+msgid "Geocode"
+msgstr "Géocoder"
+
 msgid "Geophysical"
 msgstr "Géophysique"
 
+msgid "Hazard"
+msgstr "Danger"
+
+msgid "Hazards monitored by the institution"
+msgstr "Dangers surveillés par l'établissement"
+
 msgid "Headline"
 msgstr "Gros titre"
 
-msgid ""
-"How many of this products should be visible on the landing page filter "
-"section ?"
-msgstr ""
-"Combien de ces produits doivent être visibles dans la section de filtrage de "
-"la page de destination ?"
-
 msgid "Identifier"
 msgstr "Identifiant"
 
-msgid "Immediate"
-msgstr "Immédiat"
-
 msgid "Immediate - Responsive action SHOULD be taken immediately"
 msgstr "Immédiat - Une action réactive DOIT être prise immédiatement"
 
+msgid "Incident"
+msgstr "Incident"
+
+msgid "Incidents"
+msgstr "Incidents"
+
 msgid "Instruction"
 msgstr "Instruction"
 
-msgid "Intended Recipients (If scope is Private) "
-msgstr "Destinataires prévus (si la portée est privée)"
-
 msgid "Language"
 msgstr "Langue"
 
 msgid "Law enforcement, military, homeland and local/private security"
 msgstr "Application de la loi, militaire, sécurité intérieure et locale/privée"
 
 msgid "Likely - Likely (percentage > ~50%)"
 msgstr "Probable - Probable (pourcentage > ~50%)"
 
-msgid "Link"
-msgstr "Lien"
+msgid ""
+"Link to external resource. This can be for example a link to related "
+"websites. "
+msgstr ""
+"Lien vers une ressource externe. Il peut s'agir, par exemple, d'un lien vers "
+"des sites Web connexes."
 
 msgid "Medical and public health"
 msgstr "Médecine et santé publique"
 
 msgid "Message Type"
 msgstr "Type de message"
 
@@ -276,17 +253,14 @@
 
 msgid "Name"
 msgstr "Nom"
 
 msgid "Name for the event code"
 msgstr "Nom du code d'événement"
 
-msgid "Name for the geocode"
-msgstr "Nom du géocode"
-
 msgid "Name of the recipient"
 msgstr "Nom du destinataire"
 
 msgid "No action recommended"
 msgstr "Aucune action recommandée"
 
 msgid "Note"
@@ -297,23 +271,29 @@
 
 msgid "Onset"
 msgstr "Début"
 
 msgid "Other events"
 msgstr "Autres événements"
 
-msgid "Past"
-msgstr "Passé"
+msgid "Parameter"
+msgstr "Paramètre"
+
+msgid "Parameters"
+msgstr "Paramètres"
 
 msgid "Past - Responsive action is no longer required"
 msgstr "Passé - Une action réactive n'est plus requise"
 
 msgid "Pollution and other environmental"
 msgstr "Pollution et autres problèmes environnementaux"
 
+msgid "Polygon"
+msgstr "Polygone"
+
 msgid "Possible - Possible but not likely (percentage <= ~50%)"
 msgstr "Possible - Possible mais peu probable (pourcentage <= ~50%)"
 
 msgid "Prepare - Relocate as instructed in the instruction"
 msgstr "Préparer - Déplacer comme indiqué dans l'instruction"
 
 msgid ""
@@ -334,20 +314,14 @@
 
 msgid "Reference Alert"
 msgstr "Alerte de référence"
 
 msgid "Rescue and recovery"
 msgstr "Sauvetage et récupération"
 
-msgid "Resource"
-msgstr "Ressource"
-
-msgid "Resource type whether is image, file etc"
-msgstr "Type de ressource, qu'il s'agisse d'une image, d'un fichier, etc."
-
 msgid "Response type"
 msgstr "Type de réponse"
 
 msgid ""
 "Restricted - For dissemination only to users with a known operational "
 "requirement as in the restriction field"
 msgstr ""
@@ -382,22 +356,22 @@
 msgstr "Statut"
 
 msgid "System - For messages that support alert network internal functions"
 msgstr ""
 "Système - Pour les messages prenant en charge les fonctions internes du "
 "réseau d'alerte"
 
+msgid "Target audiences for published alerts"
+msgstr "Publics cibles pour les alertes publiées"
+
 msgid "Test - Technical testing only, all recipients disregard"
 msgstr ""
 "Test - Test technique uniquement, tous les destinataires ne tiennent pas "
 "compte"
 
-msgid "The base-64 encoded data content of the resource file"
-msgstr "Le contenu des données encodées en base 64 du fichier de ressources"
-
 msgid "The code denoting the appropriate handling of the alert"
 msgstr "Le code indiquant le traitement approprié de l'alerte"
 
 msgid ""
 "The code denoting the category of the subject event of the alert message"
 msgstr ""
 "Le code désignant la catégorie de l'événement objet du message d'alerte"
@@ -427,39 +401,30 @@
 "The code denoting the type of action recommended for the target audience"
 msgstr "Le code désignant le type d'action recommandé pour le public cible"
 
 msgid "The code denoting the urgency of the subject event of the alert message"
 msgstr "Le code indiquant l'urgence de l'événement objet du message d'alerte"
 
 msgid ""
-"The code representing the digital digest ('hash') computed from the resource "
-"file"
-msgstr ""
-"Le code représentant le résumé numérique (\"hash\") calculé à partir du "
-"fichier de ressources"
-
-msgid "The effective time of the information of the alert message"
-msgstr "L'heure effective de l'information du message d'alerte"
-
-msgid ""
 "The expected time of the beginning of the subject event of the alert message"
 msgstr "L'heure prévue du début de l'événement objet du message d'alerte"
 
-msgid "The expiry time of the information of the alert message"
-msgstr "L'heure d'expiration des informations du message d'alerte"
-
 msgid ""
-"The identifier of the hyperlink associating additional information with the "
-"alert message"
-msgstr ""
-"L'identifiant du lien hypertexte associant des informations complémentaires "
-"au message d'alerte"
+"The expiry time of the information of the alert message. If not set, each "
+"recipient is free to set its own policy as to when the message is no longer "
+"in effect."
+msgstr ""
+"L'heure d'expiration des informations du message d'alerte. S'il n'est pas "
+"défini, chaque destinataire est libre de définir sa propre politique quant "
+"au moment où le message n'est plus en vigueur."
 
-msgid "The identifier of the hyperlink for the resource file"
-msgstr "L'identifiant du lien hypertexte pour le fichier de ressources"
+msgid "The human-readable name of the agency or authority issuing this alert."
+msgstr ""
+"Le nom lisible par l'homme de l'agence ou de l'autorité émettant cette "
+"alerte."
 
 msgid ""
 "The maximum altitude of the affected area of the alert message.MUST NOT be "
 "used except in combination with the altitude element. "
 msgstr ""
 "L'altitude maximale de la zone affectée du message d'alerte. NE DOIT PAS "
 "être utilisée sauf en combinaison avec l'élément d'altitude."
@@ -511,72 +476,51 @@
 msgid ""
 "The text describing the rule for limiting distribution of the restricted "
 "alert message. Used when scope value is Restricted"
 msgstr ""
 "Texte décrivant la règle de limitation de la distribution du message "
 "d'alerte restreint. Utilisé lorsque la valeur d'étendue est restreinte"
 
-msgid "The text describing the subject event of the alert message"
-msgstr "Le texte décrivant l'événement objet du message d'alerte"
-
 msgid "The text describing the type and content of the resource file"
 msgstr "Le texte décrivant le type et le contenu du fichier de ressources"
 
-msgid "The text headline of the alert message"
-msgstr "Le titre du texte du message d'alerte"
+msgid ""
+"The text headline of the alert message. Make it direct and actionable as "
+"possible while remaining short"
+msgstr ""
+"Le titre du texte du message d'alerte. Rendez-le aussi direct et exploitable "
+"que possible tout en restant court"
 
 msgid "The text identifying the source of the alert message"
 msgstr "Le texte identifiant la source du message d'alerte"
 
 msgid "Time and date of origination of the alert"
 msgstr "Heure et date d'origine de l'alerte"
 
-msgid "Title"
-msgstr "Titre"
-
-msgid "Title of the incident referent of the alert"
-msgstr "Intitulé de l'incident référent de l'alerte"
-
 msgid "Unique ID. Auto generated on creation."
 msgstr "Identifiant unique. Généré automatiquement à la création."
 
-msgid "Unknown"
-msgstr "Inconnu"
-
 msgid "Unknown - Certainty unknown"
 msgstr "Inconnu - certitude inconnue"
 
 msgid "Unknown - Severity unknown"
 msgstr "Inconnu - Gravité inconnue"
 
 msgid "Unknown - Urgency not known"
 msgstr "Inconnu - Urgence non connue"
 
 msgid "Unlikely - Not expected to occur (percentage ~ 0)"
 msgstr "Improbable – Ne devrait pas se produire (pourcentage ~ 0)"
 
-msgid ""
-"Update - Updates and supercedes the earlier message(s) identified in "
-"referenced alerts"
-msgstr ""
-"Mettre à jour - Met à jour et remplace le(s) message(s) antérieur(s) "
-"identifié(s) dans les alertes référencées"
-
 msgid "Urgency"
 msgstr "Urgence"
 
 msgid "Utility, telecommunication, other non-transport infrastructure"
 msgstr ""
 "Services publics, télécommunications, autres infrastructures non liées au "
 "transport"
 
 msgid "Value"
 msgstr "Valeur"
 
 msgid "Value of the event code"
 msgstr "Valeur du code événement"
-
-msgid "Value of the geocode"
-msgstr "Valeur du géocode"
-
-msgid "Web"
-msgstr "la toile"
```

### Comparing `capeditor-0.2.7/capeditor/locale/fr/LC_MESSAGES/django.po` & `capeditor-0.2.8/capeditor/locale/fr/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-12 14:01+0300\n"
+"POT-Creation-Date: 2023-07-14 12:05+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
-#: capeditor/blocks.py:70 capeditor/blocks.py:98 capeditor/blocks.py:370
+#: capeditor/blocks.py:70 capeditor/blocks.py:98 capeditor/blocks.py:375
 msgid "Name"
 msgstr "Nom"
 
 #: capeditor/blocks.py:70
 msgid "Name of the recipient"
 msgstr "Nom du destinataire"
 
@@ -52,15 +52,15 @@
 
 #: capeditor/blocks.py:94
 #, fuzzy
 #| msgid "The text headline of the alert message"
 msgid "Referent incident to this alert message"
 msgstr "Incident référent à ce message d'alerte"
 
-#: capeditor/blocks.py:99 capeditor/blocks.py:295 capeditor/blocks.py:371
+#: capeditor/blocks.py:99 capeditor/blocks.py:300 capeditor/blocks.py:376
 msgid "Value"
 msgstr "Valeur"
 
 #: capeditor/blocks.py:104
 msgid "Shelter - Take shelter in place or per instruction"
 msgstr "Abri - Abritez-vous sur place ou selon les instructions"
 
@@ -112,458 +112,458 @@
 msgstr "Type de réponse"
 
 #: capeditor/blocks.py:117
 msgid ""
 "The code denoting the type of action recommended for the target audience"
 msgstr "Le code désignant le type d'action recommandé pour le public cible"
 
-#: capeditor/blocks.py:158 capeditor/blocks.py:204 capeditor/blocks.py:256
-#: capeditor/blocks.py:292
+#: capeditor/blocks.py:163 capeditor/blocks.py:209 capeditor/blocks.py:261
+#: capeditor/blocks.py:297
 msgid "Affected areas / Regions"
 msgstr "Zones / Régions touchées"
 
-#: capeditor/blocks.py:159 capeditor/blocks.py:205 capeditor/blocks.py:257
-#: capeditor/blocks.py:293
+#: capeditor/blocks.py:164 capeditor/blocks.py:210 capeditor/blocks.py:262
+#: capeditor/blocks.py:298
 msgid "The text describing the affected area of the alert message"
 msgstr "Le texte décrivant la zone affectée du message d'alerte"
 
-#: capeditor/blocks.py:160
+#: capeditor/blocks.py:165
 msgid "Administrative Level"
 msgstr "Niveau administratif"
 
-#: capeditor/blocks.py:161
+#: capeditor/blocks.py:166
 msgid "Boundary"
 msgstr "Frontière"
 
-#: capeditor/blocks.py:162 capeditor/blocks.py:207
+#: capeditor/blocks.py:167 capeditor/blocks.py:212
 msgid ""
 "The paired values of points defining a polygon that delineates the affected "
 "area of the alert message"
 msgstr ""
 "Les valeurs appariées des points définissant un polygone qui délimite la "
 "zone affectée du message d'alerte"
 
-#: capeditor/blocks.py:165 capeditor/blocks.py:209 capeditor/blocks.py:260
-#: capeditor/blocks.py:297
+#: capeditor/blocks.py:170 capeditor/blocks.py:214 capeditor/blocks.py:265
+#: capeditor/blocks.py:302
 msgid "Altitude"
 msgstr "Altitude"
 
-#: capeditor/blocks.py:166 capeditor/blocks.py:210 capeditor/blocks.py:261
-#: capeditor/blocks.py:298
+#: capeditor/blocks.py:171 capeditor/blocks.py:215 capeditor/blocks.py:266
+#: capeditor/blocks.py:303
 msgid ""
 "The specific or minimum altitude of the affected area of the alert message"
 msgstr ""
 "L'altitude spécifique ou minimale de la zone affectée du message d'alerte"
 
-#: capeditor/blocks.py:168 capeditor/blocks.py:212 capeditor/blocks.py:263
-#: capeditor/blocks.py:300
+#: capeditor/blocks.py:173 capeditor/blocks.py:217 capeditor/blocks.py:268
+#: capeditor/blocks.py:305
 msgid "Ceiling"
 msgstr "Plafond"
 
-#: capeditor/blocks.py:169 capeditor/blocks.py:213 capeditor/blocks.py:264
-#: capeditor/blocks.py:301
+#: capeditor/blocks.py:174 capeditor/blocks.py:218 capeditor/blocks.py:269
+#: capeditor/blocks.py:306
 msgid ""
 "The maximum altitude of the affected area of the alert message.MUST NOT be "
 "used except in combination with the altitude element. "
 msgstr ""
 "L'altitude maximale de la zone affectée du message d'alerte. NE DOIT PAS "
 "être utilisée sauf en combinaison avec l'élément d'altitude."
 
-#: capeditor/blocks.py:206
+#: capeditor/blocks.py:211
 msgid "Polygon"
 msgstr "Polygone"
 
-#: capeditor/blocks.py:258 capeditor/blocks.py:528
+#: capeditor/blocks.py:263 capeditor/blocks.py:555
 msgid "Circle"
 msgstr "Cercle"
 
-#: capeditor/blocks.py:258
+#: capeditor/blocks.py:263
 msgid "Drag the marker to change position"
 msgstr "Faites glisser le marqueur pour changer de position"
 
-#: capeditor/blocks.py:305
+#: capeditor/blocks.py:310
 msgid "The human-readable name of the agency or authority issuing this alert."
 msgstr ""
 "Le nom lisible par l'homme de l'agence ou de l'autorité émettant cette "
 "alerte."
 
-#: capeditor/blocks.py:306
+#: capeditor/blocks.py:311
 msgid ""
 "The text describing the contact for follow-up and confirmation of the alert "
 "message"
 msgstr ""
 "Le texte décrivant le contact pour le suivi et la confirmation du message "
 "d'alerte"
 
-#: capeditor/blocks.py:307
+#: capeditor/blocks.py:312
 msgid "The text denoting the type of the subject event of the alert message"
 msgstr "Le texte indiquant le type de l'événement objet du message d'alerte"
 
-#: capeditor/blocks.py:308
+#: capeditor/blocks.py:313
 msgid "The text describing the intended audience of the alert message"
 msgstr "Le texte décrivant le public visé par le message d'alerte"
 
-#: capeditor/blocks.py:350 capeditor/blocks.py:359
+#: capeditor/blocks.py:355 capeditor/blocks.py:364
 #, fuzzy
 #| msgid "Description"
 msgid "Resource Description"
 msgstr "Description de la ressource"
 
-#: capeditor/blocks.py:351 capeditor/blocks.py:360
+#: capeditor/blocks.py:356 capeditor/blocks.py:365
 msgid "The text describing the type and content of the resource file"
 msgstr "Le texte décrivant le type et le contenu du fichier de ressources"
 
-#: capeditor/blocks.py:361
+#: capeditor/blocks.py:366
 #, fuzzy
 #| msgid "Alert Resources "
 msgid "External Resource Link"
 msgstr "Lien de ressource externe"
 
-#: capeditor/blocks.py:362
+#: capeditor/blocks.py:367
 msgid ""
 "Link to external resource. This can be for example a link to related "
 "websites. "
 msgstr ""
 "Lien vers une ressource externe. Il peut s'agir, par exemple, d'un lien vers"
 " des sites Web connexes."
 
-#: capeditor/blocks.py:370
+#: capeditor/blocks.py:375
 msgid "Name for the event code"
 msgstr "Nom du code d'événement"
 
-#: capeditor/blocks.py:371
+#: capeditor/blocks.py:376
 msgid "Value of the event code"
 msgstr "Valeur du code événement"
 
-#: capeditor/blocks.py:441
+#: capeditor/blocks.py:467
 msgid "English"
 msgstr "Anglais"
 
-#: capeditor/blocks.py:445
+#: capeditor/blocks.py:471
 msgid "Geophysical"
 msgstr "Géophysique"
 
-#: capeditor/blocks.py:446
+#: capeditor/blocks.py:472
 msgid "Meteorological"
 msgstr "Météorologique"
 
-#: capeditor/blocks.py:447
+#: capeditor/blocks.py:473
 msgid "General emergency and public safety"
 msgstr "Urgence générale et sécurité publique"
 
-#: capeditor/blocks.py:448
+#: capeditor/blocks.py:474
 msgid "Law enforcement, military, homeland and local/private security"
 msgstr ""
 "Application de la loi, militaire, sécurité intérieure et locale/privée"
 
-#: capeditor/blocks.py:449
+#: capeditor/blocks.py:475
 msgid "Rescue and recovery"
 msgstr "Sauvetage et récupération"
 
-#: capeditor/blocks.py:450
+#: capeditor/blocks.py:476
 msgid "Fire suppression and rescue"
 msgstr "Lutte contre les incendies et sauvetage"
 
-#: capeditor/blocks.py:451
+#: capeditor/blocks.py:477
 msgid "Medical and public health"
 msgstr "Médecine et santé publique"
 
-#: capeditor/blocks.py:452
+#: capeditor/blocks.py:478
 msgid "Pollution and other environmental"
 msgstr "Pollution et autres problèmes environnementaux"
 
-#: capeditor/blocks.py:453
+#: capeditor/blocks.py:479
 msgid "Public and private transportation"
 msgstr "Transport public et privé"
 
-#: capeditor/blocks.py:454
+#: capeditor/blocks.py:480
 msgid "Utility, telecommunication, other non-transport infrastructure"
 msgstr ""
 "Services publics, télécommunications, autres infrastructures non liées au "
 "transport"
 
-#: capeditor/blocks.py:455
+#: capeditor/blocks.py:481
 msgid ""
 "Chemical, Biological, Radiological, Nuclear or High-Yield Explosive threat "
 "or attack"
 msgstr ""
 "Menace ou attaque chimique, biologique, radiologique, nucléaire ou explosive"
 " à haut rendement"
 
-#: capeditor/blocks.py:456
+#: capeditor/blocks.py:482
 msgid "Other events"
 msgstr "Autres événements"
 
-#: capeditor/blocks.py:460
+#: capeditor/blocks.py:486
 msgid "Immediate - Responsive action SHOULD be taken immediately"
 msgstr "Immédiat - Une action réactive DOIT être prise immédiatement"
 
-#: capeditor/blocks.py:461
+#: capeditor/blocks.py:487
 msgid "Expected - Responsive action SHOULD be taken soon (within next hour)"
 msgstr ""
 "Attendu - Une action réactive DEVRAIT être entreprise rapidement (dans "
 "l'heure qui suit)"
 
-#: capeditor/blocks.py:462
+#: capeditor/blocks.py:488
 msgid "Future - Responsive action SHOULD be taken in the near future"
 msgstr ""
 "Futur - Des mesures réactives DOIVENT être prises dans un proche avenir"
 
-#: capeditor/blocks.py:463
+#: capeditor/blocks.py:489
 msgid "Past - Responsive action is no longer required"
 msgstr "Passé - Une action réactive n'est plus requise"
 
-#: capeditor/blocks.py:464
+#: capeditor/blocks.py:490
 msgid "Unknown - Urgency not known"
 msgstr "Inconnu - Urgence non connue"
 
-#: capeditor/blocks.py:468
+#: capeditor/blocks.py:494
 msgid "Extreme - Extraordinary threat to life or property"
 msgstr "Extrême - Menace extraordinaire pour la vie ou la propriété"
 
-#: capeditor/blocks.py:469
+#: capeditor/blocks.py:495
 msgid "Severe - Significant threat to life or property"
 msgstr "Grave - Menace importante pour la vie ou la propriété"
 
-#: capeditor/blocks.py:470
+#: capeditor/blocks.py:496
 msgid "Moderate - Possible threat to life or property"
 msgstr "Modéré - Menace possible pour la vie ou la propriété"
 
-#: capeditor/blocks.py:471
+#: capeditor/blocks.py:497
 msgid "Minor - Minimal to no known threat to life or property"
 msgstr "Mineur - Menace minimale ou nulle connue pour la vie ou la propriété"
 
-#: capeditor/blocks.py:472
+#: capeditor/blocks.py:498
 msgid "Unknown - Severity unknown"
 msgstr "Inconnu - Gravité inconnue"
 
-#: capeditor/blocks.py:476
+#: capeditor/blocks.py:502
 msgid "Observed - Determined to have occurred or to be ongoing"
 msgstr "Observé - Déterminé s'être produit ou être en cours"
 
-#: capeditor/blocks.py:477
+#: capeditor/blocks.py:503
 msgid "Likely - Likely (percentage > ~50%)"
 msgstr "Probable - Probable (pourcentage > ~50%)"
 
-#: capeditor/blocks.py:478
+#: capeditor/blocks.py:504
 msgid "Possible - Possible but not likely (percentage <= ~50%)"
 msgstr "Possible - Possible mais peu probable (pourcentage <= ~50%)"
 
-#: capeditor/blocks.py:479
+#: capeditor/blocks.py:505
 msgid "Unlikely - Not expected to occur (percentage ~ 0)"
 msgstr "Improbable – Ne devrait pas se produire (pourcentage ~ 0)"
 
-#: capeditor/blocks.py:480
+#: capeditor/blocks.py:506
 msgid "Unknown - Certainty unknown"
 msgstr "Inconnu - certitude inconnue"
 
-#: capeditor/blocks.py:483
-msgid "Language"
-msgstr "Langue"
-
-#: capeditor/blocks.py:484
-msgid "The code denoting the language of the alert message"
-msgstr "Le code désignant la langue du message d'alerte"
+#: capeditor/blocks.py:508
+msgid "Event"
+msgstr "Événement"
 
-#: capeditor/blocks.py:485
+#: capeditor/blocks.py:510
 msgid "Category"
 msgstr "Catégorie"
 
-#: capeditor/blocks.py:486
+#: capeditor/blocks.py:511
 msgid ""
 "The code denoting the category of the subject event of the alert message"
 msgstr ""
 "Le code désignant la catégorie de l'événement objet du message d'alerte"
 
-#: capeditor/blocks.py:488
-msgid "Event"
-msgstr "Événement"
+#: capeditor/blocks.py:513
+msgid "Language"
+msgstr "Langue"
 
-#: capeditor/blocks.py:489
+#: capeditor/blocks.py:514
+msgid "The code denoting the language of the alert message"
+msgstr "Le code désignant la langue du message d'alerte"
+
+#: capeditor/blocks.py:516
 msgid "Urgency"
 msgstr "Urgence"
 
-#: capeditor/blocks.py:490
+#: capeditor/blocks.py:517
 msgid ""
 "The code denoting the urgency of the subject event of the alert message"
 msgstr "Le code indiquant l'urgence de l'événement objet du message d'alerte"
 
-#: capeditor/blocks.py:492
+#: capeditor/blocks.py:519
 msgid "Severity"
 msgstr "Gravité"
 
-#: capeditor/blocks.py:493
+#: capeditor/blocks.py:520
 msgid ""
 "The code denoting the severity of the subject event of the alert message"
 msgstr "Le code indiquant la gravité de l'événement objet du message d'alerte"
 
-#: capeditor/blocks.py:495
+#: capeditor/blocks.py:522
 msgid "Certainty"
 msgstr "Certitude"
 
-#: capeditor/blocks.py:496
+#: capeditor/blocks.py:523
 msgid ""
 "The code denoting the certainty of the subject event of the alert message"
 msgstr ""
 "Le code indiquant la certitude de l'événement objet du message d'alerte"
 
-#: capeditor/blocks.py:498
+#: capeditor/blocks.py:525
 msgid "Headline"
 msgstr "Gros titre"
 
-#: capeditor/blocks.py:499
+#: capeditor/blocks.py:526
 msgid ""
 "The text headline of the alert message. Make it direct and actionable as "
 "possible while remaining short"
 msgstr ""
 "Le titre du texte du message d'alerte. Rendez-le aussi direct et exploitable"
 " que possible tout en restant court"
 
-#: capeditor/blocks.py:501
+#: capeditor/blocks.py:528
 msgid "Description"
 msgstr "Description"
 
-#: capeditor/blocks.py:503
+#: capeditor/blocks.py:530
 #, fuzzy
 #| msgid "The text describing the subject event of the alert message"
 msgid ""
 "The text describing the subject event of the alert message. An extended "
 "description of the hazard or event that occasioned this message"
 msgstr ""
 "Le texte décrivant l'événement objet du message d'alerte. Une description "
 "détaillée du danger ou de l'événement à l'origine de ce message"
 
-#: capeditor/blocks.py:505
+#: capeditor/blocks.py:532
 msgid "Instruction"
 msgstr "Instruction"
 
-#: capeditor/blocks.py:506
+#: capeditor/blocks.py:533
 msgid ""
 "The text describing the recommended action to be taken by recipients of the "
 "alert message"
 msgstr ""
 "Le texte décrivant l'action recommandée à entreprendre par les destinataires"
 " du message d'alerte"
 
-#: capeditor/blocks.py:508
+#: capeditor/blocks.py:535
 msgid "Effective"
 msgstr "Efficace"
 
-#: capeditor/blocks.py:509
+#: capeditor/blocks.py:536
 #, fuzzy
 #| msgid "The effective time of the information of the alert message"
 msgid ""
 "The effective time of the information of the alert message. If not set, the "
 "sent date will be used"
 msgstr ""
 "L'heure effective de l'information du message d'alerte. Si elle n'est pas "
 "définie, la date d'envoi sera utilisée"
 
-#: capeditor/blocks.py:511
+#: capeditor/blocks.py:538
 msgid "Onset"
 msgstr "Début"
 
-#: capeditor/blocks.py:512
+#: capeditor/blocks.py:539
 msgid ""
 "The expected time of the beginning of the subject event of the alert message"
 msgstr "L'heure prévue du début de l'événement objet du message d'alerte"
 
-#: capeditor/blocks.py:514
+#: capeditor/blocks.py:541
 msgid "Expires"
 msgstr "Expire"
 
-#: capeditor/blocks.py:515
+#: capeditor/blocks.py:542
 msgid ""
 "The expiry time of the information of the alert message. If not set, each "
 "recipient is free to set its own policy as to when the message is no longer "
 "in effect."
 msgstr ""
 "L'heure d'expiration des informations du message d'alerte. S'il n'est pas "
 "défini, chaque destinataire est libre de définir sa propre politique quant "
 "au moment où le message n'est plus en vigueur."
 
-#: capeditor/blocks.py:518
+#: capeditor/blocks.py:545
 #, fuzzy
 #| msgid "Response type"
 msgid "Response Types"
 msgstr "Types de réponse"
 
-#: capeditor/blocks.py:520
+#: capeditor/blocks.py:547
 #, fuzzy
 #| msgid "Sender"
 msgid "Sender name"
 msgstr "Nom de l'expéditeur"
 
-#: capeditor/blocks.py:522
+#: capeditor/blocks.py:549
 msgid "Contact"
 msgstr "Contact"
 
-#: capeditor/blocks.py:523 capeditor/blocks.py:550
+#: capeditor/blocks.py:550 capeditor/blocks.py:580
 msgid "Audience"
 msgstr "Public"
 
-#: capeditor/blocks.py:526
+#: capeditor/blocks.py:553
 msgid "Admin Boundary"
 msgstr "Limite administrative"
 
-#: capeditor/blocks.py:527
+#: capeditor/blocks.py:554
 msgid "Draw Polygon"
 msgstr "Dessiner un polygone"
 
-#: capeditor/blocks.py:529
+#: capeditor/blocks.py:556
 msgid "Geocode"
 msgstr "Géocoder"
 
-#: capeditor/blocks.py:530
+#: capeditor/blocks.py:557
 msgid "Alert Area"
 msgstr "Zone d'alerte"
 
-#: capeditor/blocks.py:530
+#: capeditor/blocks.py:557
 msgid "Admin Boundary, Polygon, Circle or Geocode"
 msgstr "Limite administrative, Polygone, Cercle ou Géocode"
 
-#: capeditor/blocks.py:535
+#: capeditor/blocks.py:562
 #, fuzzy
 #| msgid "Resource"
 msgid "Resources"
 msgstr "Ressources"
 
-#: capeditor/blocks.py:535
+#: capeditor/blocks.py:562
 msgid ""
 "Additional file with supplemental information related to this alert "
 "information"
 msgstr ""
 "Fichier supplémentaire avec des informations supplémentaires liées à cette "
 "information d'alerte"
 
-#: capeditor/blocks.py:538
+#: capeditor/blocks.py:565
 msgid "Parameter"
 msgstr "Paramètre"
 
-#: capeditor/blocks.py:538
+#: capeditor/blocks.py:565
 msgid "Parameters"
 msgstr "Paramètres"
 
-#: capeditor/blocks.py:539
+#: capeditor/blocks.py:566
 #, fuzzy
 #| msgid "Event"
 msgid "Event Code"
 msgstr "Code d'événement"
 
-#: capeditor/blocks.py:539
+#: capeditor/blocks.py:566
 #, fuzzy
 #| msgid "Event"
 msgid "Event codes"
 msgstr "Codes d'événement"
 
-#: capeditor/blocks.py:545
+#: capeditor/blocks.py:575
 msgid "Hazard"
 msgstr "Danger"
 
-#: capeditor/blocks.py:554
+#: capeditor/blocks.py:584
 #, fuzzy
 #| msgid "Contact"
 msgid "Contact Detail"
 msgstr "Coordonnées"
 
 #: capeditor/models.py:35
 #, fuzzy
```

### Comparing `capeditor-0.2.7/capeditor/locale/sw/LC_MESSAGES/django.mo` & `capeditor-0.2.8/capeditor/locale/sw/LC_MESSAGES/django.mo`

 * *Files 11% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,99 +8,86 @@
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid ""
-" Identifies the originator of an alert. This can be an email of the "
-"institution for example"
-msgstr ""
-"Hubainisha mwanzilishi wa arifa. Hii inaweza kuwa barua pepe ya taasisi kwa "
-"mfano"
-
-msgid ""
 "Acknowledge - Acknowledges receipt and acceptance of the message(s) "
 "identified in references field"
 msgstr ""
 "Thibitisha - Inakubali kupokea na kukubali ujumbe uliotambuliwa katika uga "
 "wa marejeleo"
 
 msgid "Actual - Actionable by all targeted recipients"
 msgstr "Halisi - Inaweza kutekelezwa na wapokeaji wote wanaolengwa"
 
+msgid ""
+"Additional file with supplemental information related to this alert "
+"information"
+msgstr ""
+"Faili ya ziada iliyo na maelezo ya ziada yanayohusiana na taarifa hii ya "
+"arifa"
+
+msgid "Addresses"
+msgstr "Anwani"
+
+msgid "Admin Boundary"
+msgstr "Mpaka wa Utawala"
+
+msgid "Admin Boundary, Polygon, Circle or Geocode"
+msgstr "Mpaka wa Msimamizi, Poligoni, Mduara au Msimbo wa Jiografia"
+
+msgid "Administrative Level"
+msgstr "Kiwango cha Utawala"
+
 msgid "Affected areas / Regions"
 msgstr "Maeneo / Mikoa iliyoathirika"
 
-msgid "Alert"
-msgstr "Tahadhari"
-
 msgid "Alert - Initial information requiring attention by targeted recipients"
 msgstr ""
 "Tahadhari - Taarifa ya awali inayohitaji kushughulikiwa na wapokeaji lengwa"
 
 msgid "Alert Area"
 msgstr "Eneo la Tahadhari"
 
-msgid "Alert Areas "
-msgstr "Maeneo ya Tahadhari"
-
-msgid ""
-"Alert Categorization (Category, Urgency, Severity, Certainity, Response & "
-"Dates)"
-msgstr ""
-"Uainishaji wa Arifa (Kitengo, Udharura, Ukali, Uhakika, Majibu na Tarehe)"
-
-msgid ""
-"Alert Delivery Message (Headline, Description, Intsructions, Contact & "
-"Website)"
-msgstr ""
-"Ujumbe wa Tahadhari (Kichwa cha Habari, Maelezo, Maagizo, Mawasiliano na "
-"Tovuti)"
-
-msgid "Alert Identification (Sender, Message Type, Scope)"
-msgstr "Kitambulisho cha Arifa (Mtumaji, Aina ya Ujumbe, Mawanda)"
-
-msgid "Alert Info"
-msgstr "Taarifa za Tahadhari"
-
 msgid "Alert Information"
 msgstr "Taarifa za Tahadhari"
 
-msgid "Alert Resources "
-msgstr "Nyenzo za Tahadhari"
-
-msgid "Alerts Per Page"
-msgstr "Tahadhari kwa Kila Ukurasa"
-
 msgid ""
 "All Clear - The subject event no longer poses a threat or concern and any "
 "follow on action is described in instruction"
 msgstr ""
 "Yote Wazi - Tukio la somo halileti tishio au wasiwasi tena na ufuatiliaji "
 "wowote wa hatua unaelezwa katika maagizo"
 
 msgid "Altitude"
 msgstr "Urefu"
 
-msgid "Area"
-msgstr "Eneo"
-
 msgid ""
 "Assess - Evaluate the information in this message - DONT USE FOR PUBLIC "
 "ALERTS"
 msgstr ""
 "Tathmini - Tathmini taarifa katika ujumbe huu - USITUMIE KWA TAARIFA KWA UMMA"
 
 msgid "Audience"
 msgstr "Hadhira"
 
 msgid "Avoid - Avoid the subject event as per the instruction"
 msgstr "Epuka - Epuka tukio la somo kulingana na maagizo"
 
+msgid "Boundary"
+msgstr "Mpaka"
+
+msgid "CAP Sender Name"
+msgstr "Jina la Mtumaji CAP"
+
+msgid "Can be the website link or email of the sending institution"
+msgstr "Inaweza kuwa kiungo cha tovuti au barua pepe ya taasisi inayotuma"
+
 msgid "Cancel - Cancels the earlier message(s) identified in references"
 msgstr "Ghairi - Hughairi ujumbe wa awali uliotambuliwa katika marejeleo"
 
 msgid "Category"
 msgstr "Kategoria"
 
 msgid "Ceiling"
@@ -112,47 +99,44 @@
 msgid ""
 "Chemical, Biological, Radiological, Nuclear or High-Yield Explosive threat "
 "or attack"
 msgstr ""
 "Tishio au mashambulizi ya Kemikali, Baiolojia, Radiolojia, Nyuklia au Mavuno "
 "ya Juu"
 
+msgid "Circle"
+msgstr "Mduara"
+
 msgid "Code"
 msgstr "Kanuni"
 
 msgid "Contact"
 msgstr "Wasiliana"
 
 msgid "Description"
 msgstr "Maelezo"
 
-msgid "Description of the incident"
-msgstr "Maelezo ya tukio"
-
 msgid ""
 "Draft - A preliminary template or draft, not actionable in its current form"
 msgstr ""
 "Rasimu - Kiolezo au rasimu ya awali, isiyoweza kutekelezeka katika umbo lake "
 "la sasa"
 
-msgid "Earlier Reference Alerts -  If applicable"
-msgstr "Arifa za Marejeleo za Awali - Ikitumika"
+msgid "Drag the marker to change position"
+msgstr "Buruta alama ili kubadilisha nafasi"
+
+msgid "Draw Polygon"
+msgstr "Chora Polygon"
 
 msgid "Earlier alert referenced by this alert"
 msgstr "Tahadhari ya awali iliyorejelewa na tahadhari hii"
 
 msgid "Effective"
 msgstr "Ufanisi"
 
-msgid "Email"
-msgstr "Barua pepe"
-
-msgid "Email address"
-msgstr "Barua pepe"
-
 msgid "English"
 msgstr "Kiingereza"
 
 msgid ""
 "Error -  Indicates rejection of the message(s) identified in references; "
 "explanation SHOULD appear in note field"
 msgstr ""
@@ -172,85 +156,79 @@
 msgid ""
 "Exercise - Actionable only by designated exercise participants; exercise "
 "identifier SHOULD appear in note"
 msgstr ""
 "Zoezi - Inaweza kutekelezwa tu na washiriki walioteuliwa wa mazoezi; "
 "kitambulisho cha zoezi LAZIMA kionekane kwenye dokezo"
 
-msgid "Expected"
-msgstr "Inatarajiwa"
-
 msgid "Expected - Responsive action SHOULD be taken soon (within next hour)"
 msgstr ""
 "Inatarajiwa - Hatua ya kujibu LAZIMA ichukuliwe hivi karibuni (ndani ya saa "
 "ijayo)"
 
 msgid "Expires"
 msgstr "Muda wake unaisha"
 
 msgid "Extreme - Extraordinary threat to life or property"
 msgstr "Uliokithiri - Tishio lisilo la kawaida kwa maisha au mali"
 
-msgid "File"
-msgstr "Faili"
-
-msgid "File, Document etc"
-msgstr "Faili, Hati n.k"
-
 msgid "Fire suppression and rescue"
 msgstr "Kuzuia moto na uokoaji"
 
-msgid "Future"
-msgstr "Baadaye"
-
 msgid "Future - Responsive action SHOULD be taken in the near future"
 msgstr "Wakati Ujao - Hatua ya kuitikia LAZIMA ichukuliwe katika siku za usoni"
 
 msgid "General emergency and public safety"
 msgstr "Dharura ya jumla na usalama wa umma"
 
+msgid "Geocode"
+msgstr "Msimbo wa kijiografia"
+
 msgid "Geophysical"
 msgstr "Kijiofizikia"
 
+msgid "Hazard"
+msgstr "Hatari"
+
+msgid "Hazards monitored by the institution"
+msgstr "Hatari zinazofuatiliwa na taasisi"
+
 msgid "Headline"
 msgstr "Kichwa cha habari"
 
-msgid ""
-"How many of this products should be visible on the landing page filter "
-"section ?"
-msgstr ""
-"Je, ni bidhaa ngapi kati ya hizi zinazopaswa kuonekana kwenye sehemu ya "
-"kichujio cha ukurasa wa kutua?"
-
 msgid "Identifier"
 msgstr "Kitambulisho"
 
-msgid "Immediate"
-msgstr "Mara moja"
-
 msgid "Immediate - Responsive action SHOULD be taken immediately"
 msgstr "Hapo Hapo - Hatua ya kuitikia INATAKIWA ichukuliwe mara moja"
 
+msgid "Incident"
+msgstr "Tukio"
+
+msgid "Incidents"
+msgstr "Matukio"
+
 msgid "Instruction"
 msgstr "Maagizo"
 
-msgid "Intended Recipients (If scope is Private) "
-msgstr "Wapokeaji Wanaotarajiwa (Ikiwa upeo ni wa Faragha)"
-
 msgid "Language"
 msgstr "Lugha"
 
 msgid "Law enforcement, military, homeland and local/private security"
 msgstr "Utekelezaji wa sheria, kijeshi, nchi na usalama wa ndani/binafsi"
 
 msgid "Likely - Likely (percentage > ~50%)"
 msgstr "Huenda - Huenda (asilimia> ~50%)"
 
-msgid "Link"
-msgstr "Kiungo"
+msgid ""
+"Link to external resource. This can be for example a link to related "
+"websites. "
+msgstr ""
+"Unganisha kwa rasilimali ya nje. Hii inaweza kuwa kwa mfano kiungo cha "
+"tovuti zinazohusiana."
 
 msgid "Medical and public health"
 msgstr "Afya ya matibabu na ya umma"
 
 msgid "Message Type"
 msgstr "Aina ya Ujumbe"
 
@@ -269,17 +247,14 @@
 
 msgid "Name"
 msgstr "Jina"
 
 msgid "Name for the event code"
 msgstr "Jina la msimbo wa tukio"
 
-msgid "Name for the geocode"
-msgstr "Jina la msimbo wa kijiografia"
-
 msgid "Name of the recipient"
 msgstr "Jina la mpokeaji"
 
 msgid "No action recommended"
 msgstr "Hakuna hatua inayopendekezwa"
 
 msgid "Note"
@@ -290,23 +265,29 @@
 
 msgid "Onset"
 msgstr "Kuanza"
 
 msgid "Other events"
 msgstr "Matukio mengine"
 
-msgid "Past"
-msgstr "Zamani"
+msgid "Parameter"
+msgstr "Kigezo"
+
+msgid "Parameters"
+msgstr "Vigezo"
 
 msgid "Past - Responsive action is no longer required"
 msgstr "Zamani - Hatua ya kujibu haihitajiki tena"
 
 msgid "Pollution and other environmental"
 msgstr "Uchafuzi na mazingira mengine"
 
+msgid "Polygon"
+msgstr "Poligoni"
+
 msgid "Possible - Possible but not likely (percentage <= ~50%)"
 msgstr "Inawezekana - Inawezekana lakini haiwezekani (asilimia <= ~50%)"
 
 msgid "Prepare - Relocate as instructed in the instruction"
 msgstr "Jitayarishe - Hamisha kama ilivyoelekezwa katika maagizo"
 
 msgid ""
@@ -327,20 +308,14 @@
 
 msgid "Reference Alert"
 msgstr "Tahadhari ya Marejeleo"
 
 msgid "Rescue and recovery"
 msgstr "Kuokoa na kupona"
 
-msgid "Resource"
-msgstr "Rasilimali"
-
-msgid "Resource type whether is image, file etc"
-msgstr "Aina ya rasilimali iwe ni picha, faili n.k"
-
 msgid "Response type"
 msgstr "Aina ya majibu"
 
 msgid ""
 "Restricted - For dissemination only to users with a known operational "
 "requirement as in the restriction field"
 msgstr ""
@@ -373,20 +348,20 @@
 
 msgid "Status"
 msgstr "Hali"
 
 msgid "System - For messages that support alert network internal functions"
 msgstr "Mfumo - Kwa ujumbe unaoauni vitendaji vya ndani vya arifa"
 
+msgid "Target audiences for published alerts"
+msgstr "Hadhira inayolengwa kwa arifa zilizochapishwa"
+
 msgid "Test - Technical testing only, all recipients disregard"
 msgstr "Jaribio - Jaribio la kiufundi pekee, wapokeaji wote hupuuza"
 
-msgid "The base-64 encoded data content of the resource file"
-msgstr "Maudhui ya data iliyosimbwa ya base-64 ya faili ya rasilimali"
-
 msgid "The code denoting the appropriate handling of the alert"
 msgstr "Msimbo unaoashiria utunzaji unaofaa wa tahadhari"
 
 msgid ""
 "The code denoting the category of the subject event of the alert message"
 msgstr "Msimbo unaoashiria aina ya tukio la somo la ujumbe wa tahadhari"
 
@@ -415,39 +390,29 @@
 msgstr ""
 "Msimbo unaoashiria aina ya kitendo kinachopendekezwa kwa hadhira lengwa"
 
 msgid "The code denoting the urgency of the subject event of the alert message"
 msgstr "Msimbo unaoashiria uharaka wa tukio la somo la ujumbe wa tahadhari"
 
 msgid ""
-"The code representing the digital digest ('hash') computed from the resource "
-"file"
-msgstr ""
-"Msimbo unaowakilisha muhtasari wa dijiti ('hash') uliokokotwa kutoka kwa "
-"faili ya rasilimali"
-
-msgid "The effective time of the information of the alert message"
-msgstr "Wakati unaofaa wa taarifa ya ujumbe wa tahadhari"
-
-msgid ""
 "The expected time of the beginning of the subject event of the alert message"
 msgstr "Muda unaotarajiwa wa mwanzo wa tukio la somo la ujumbe wa tahadhari"
 
-msgid "The expiry time of the information of the alert message"
-msgstr "Muda wa mwisho wa taarifa ya ujumbe wa arifa"
-
 msgid ""
-"The identifier of the hyperlink associating additional information with the "
-"alert message"
+"The expiry time of the information of the alert message. If not set, each "
+"recipient is free to set its own policy as to when the message is no longer "
+"in effect."
 msgstr ""
-"Kitambulisho cha kiungo kinachohusisha maelezo ya ziada na ujumbe wa "
-"tahadhari"
+"Muda wa mwisho wa taarifa ya ujumbe wa arifa. Ikiwa haijawekwa, kila "
+"mpokeaji yuko huru kuweka sera yake mwenyewe kuhusu ni lini ujumbe haufanyi "
+"kazi tena."
 
-msgid "The identifier of the hyperlink for the resource file"
-msgstr "Kitambulisho cha kiungo cha faili ya rasilimali"
+msgid "The human-readable name of the agency or authority issuing this alert."
+msgstr ""
+"Jina linaloweza kusomeka na binadamu la wakala au mamlaka inayotoa arifa hii."
 
 msgid ""
 "The maximum altitude of the affected area of the alert message.MUST NOT be "
 "used except in combination with the altitude element. "
 msgstr ""
 "Upeo wa mwinuko wa eneo lililoathiriwa la ujumbe wa tahadhari.LAZIMA "
 "USITUMIKE isipokuwa pamoja na kipengele cha mwinuko."
@@ -499,70 +464,49 @@
 msgid ""
 "The text describing the rule for limiting distribution of the restricted "
 "alert message. Used when scope value is Restricted"
 msgstr ""
 "Maandishi yanayoelezea sheria ya kuzuia usambazaji wa ujumbe wa tahadhari "
 "uliowekewa vikwazo. Inatumika wakati thamani ya upeo imezuiwa"
 
-msgid "The text describing the subject event of the alert message"
-msgstr "Maandishi yanayoelezea tukio la somo la ujumbe wa tahadhari"
-
 msgid "The text describing the type and content of the resource file"
 msgstr "Maandishi yanayoelezea aina na maudhui ya faili ya rasilimali"
 
-msgid "The text headline of the alert message"
-msgstr "Kichwa cha maandishi cha ujumbe wa tahadhari"
+msgid ""
+"The text headline of the alert message. Make it direct and actionable as "
+"possible while remaining short"
+msgstr ""
+"Kichwa cha maandishi cha ujumbe wa tahadhari. Ifanye moja kwa moja na iweze "
+"kutekelezeka iwezekanavyo huku ikisalia kuwa fupi"
 
 msgid "The text identifying the source of the alert message"
 msgstr "Maandishi yanayotambulisha chanzo cha ujumbe wa arifa"
 
 msgid "Time and date of origination of the alert"
 msgstr "Wakati na tarehe ya asili ya arifa"
 
-msgid "Title"
-msgstr "Kichwa"
-
-msgid "Title of the incident referent of the alert"
-msgstr "Kichwa cha mrejeleaji wa tukio la arifa"
-
 msgid "Unique ID. Auto generated on creation."
 msgstr "Kitambulisho cha kipekee. Imetengenezwa kiotomatiki kwenye uundaji."
 
-msgid "Unknown"
-msgstr "Haijulikani"
-
 msgid "Unknown - Certainty unknown"
 msgstr "Haijulikani - Hakika haijulikani"
 
 msgid "Unknown - Severity unknown"
 msgstr "Haijulikani - Ukali haujulikani"
 
 msgid "Unknown - Urgency not known"
 msgstr "Haijulikani - Udharura haujulikani"
 
 msgid "Unlikely - Not expected to occur (percentage ~ 0)"
 msgstr "Haiwezekani - Haitarajiwi kutokea (asilimia ~ 0)"
 
-msgid ""
-"Update - Updates and supercedes the earlier message(s) identified in "
-"referenced alerts"
-msgstr ""
-"Sasisha - Inasasisha na kuchukua nafasi ya ujumbe wa awali uliotambuliwa "
-"katika arifa zilizorejelewa"
-
 msgid "Urgency"
 msgstr "Uharaka"
 
 msgid "Utility, telecommunication, other non-transport infrastructure"
 msgstr "Huduma, mawasiliano ya simu, miundombinu mingine isiyo ya usafiri"
 
 msgid "Value"
 msgstr "Thamani"
 
 msgid "Value of the event code"
 msgstr "Thamani ya msimbo wa tukio"
-
-msgid "Value of the geocode"
-msgstr "Thamani ya msimbo wa kijiografia"
-
-msgid "Web"
-msgstr "Mtandao"
```

### Comparing `capeditor-0.2.7/capeditor/locale/sw/LC_MESSAGES/django.po` & `capeditor-0.2.8/capeditor/locale/sw/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-12 14:01+0300\n"
+"POT-Creation-Date: 2023-07-14 12:05+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: capeditor/blocks.py:70 capeditor/blocks.py:98 capeditor/blocks.py:370
+#: capeditor/blocks.py:70 capeditor/blocks.py:98 capeditor/blocks.py:375
 msgid "Name"
 msgstr "Jina"
 
 #: capeditor/blocks.py:70
 msgid "Name of the recipient"
 msgstr "Jina la mpokeaji"
 
@@ -52,15 +52,15 @@
 
 #: capeditor/blocks.py:94
 #, fuzzy
 #| msgid "The text headline of the alert message"
 msgid "Referent incident to this alert message"
 msgstr "Tukio linalorejelewa kwa ujumbe huu wa tahadhari"
 
-#: capeditor/blocks.py:99 capeditor/blocks.py:295 capeditor/blocks.py:371
+#: capeditor/blocks.py:99 capeditor/blocks.py:300 capeditor/blocks.py:376
 msgid "Value"
 msgstr "Thamani"
 
 #: capeditor/blocks.py:104
 msgid "Shelter - Take shelter in place or per instruction"
 msgstr "Makazi - Pata makazi mahali au kwa maagizo"
 
@@ -113,455 +113,455 @@
 
 #: capeditor/blocks.py:117
 msgid ""
 "The code denoting the type of action recommended for the target audience"
 msgstr ""
 "Msimbo unaoashiria aina ya kitendo kinachopendekezwa kwa hadhira lengwa"
 
-#: capeditor/blocks.py:158 capeditor/blocks.py:204 capeditor/blocks.py:256
-#: capeditor/blocks.py:292
+#: capeditor/blocks.py:163 capeditor/blocks.py:209 capeditor/blocks.py:261
+#: capeditor/blocks.py:297
 msgid "Affected areas / Regions"
 msgstr "Maeneo / Mikoa iliyoathirika"
 
-#: capeditor/blocks.py:159 capeditor/blocks.py:205 capeditor/blocks.py:257
-#: capeditor/blocks.py:293
+#: capeditor/blocks.py:164 capeditor/blocks.py:210 capeditor/blocks.py:262
+#: capeditor/blocks.py:298
 msgid "The text describing the affected area of the alert message"
 msgstr "Maandishi yanayoelezea eneo lililoathiriwa la ujumbe wa tahadhari"
 
-#: capeditor/blocks.py:160
+#: capeditor/blocks.py:165
 msgid "Administrative Level"
 msgstr "Kiwango cha Utawala"
 
-#: capeditor/blocks.py:161
+#: capeditor/blocks.py:166
 msgid "Boundary"
 msgstr "Mpaka"
 
-#: capeditor/blocks.py:162 capeditor/blocks.py:207
+#: capeditor/blocks.py:167 capeditor/blocks.py:212
 msgid ""
 "The paired values of points defining a polygon that delineates the affected "
 "area of the alert message"
 msgstr ""
 "Thamani zilizooanishwa za vidokezo vinavyofafanua poligoni ambayo hufafanua "
 "eneo lililoathiriwa la ujumbe wa tahadhari."
 
-#: capeditor/blocks.py:165 capeditor/blocks.py:209 capeditor/blocks.py:260
-#: capeditor/blocks.py:297
+#: capeditor/blocks.py:170 capeditor/blocks.py:214 capeditor/blocks.py:265
+#: capeditor/blocks.py:302
 msgid "Altitude"
 msgstr "Urefu"
 
-#: capeditor/blocks.py:166 capeditor/blocks.py:210 capeditor/blocks.py:261
-#: capeditor/blocks.py:298
+#: capeditor/blocks.py:171 capeditor/blocks.py:215 capeditor/blocks.py:266
+#: capeditor/blocks.py:303
 msgid ""
 "The specific or minimum altitude of the affected area of the alert message"
 msgstr ""
 "Urefu mahususi au wa chini kabisa wa eneo lililoathiriwa la ujumbe wa "
 "tahadhari"
 
-#: capeditor/blocks.py:168 capeditor/blocks.py:212 capeditor/blocks.py:263
-#: capeditor/blocks.py:300
+#: capeditor/blocks.py:173 capeditor/blocks.py:217 capeditor/blocks.py:268
+#: capeditor/blocks.py:305
 msgid "Ceiling"
 msgstr "Dari"
 
-#: capeditor/blocks.py:169 capeditor/blocks.py:213 capeditor/blocks.py:264
-#: capeditor/blocks.py:301
+#: capeditor/blocks.py:174 capeditor/blocks.py:218 capeditor/blocks.py:269
+#: capeditor/blocks.py:306
 msgid ""
 "The maximum altitude of the affected area of the alert message.MUST NOT be "
 "used except in combination with the altitude element. "
 msgstr ""
 "Upeo wa mwinuko wa eneo lililoathiriwa la ujumbe wa tahadhari.LAZIMA "
 "USITUMIKE isipokuwa pamoja na kipengele cha mwinuko."
 
-#: capeditor/blocks.py:206
+#: capeditor/blocks.py:211
 msgid "Polygon"
 msgstr "Poligoni"
 
-#: capeditor/blocks.py:258 capeditor/blocks.py:528
+#: capeditor/blocks.py:263 capeditor/blocks.py:555
 msgid "Circle"
 msgstr "Mduara"
 
-#: capeditor/blocks.py:258
+#: capeditor/blocks.py:263
 msgid "Drag the marker to change position"
 msgstr "Buruta alama ili kubadilisha nafasi"
 
-#: capeditor/blocks.py:305
+#: capeditor/blocks.py:310
 msgid "The human-readable name of the agency or authority issuing this alert."
 msgstr ""
 "Jina linaloweza kusomeka na binadamu la wakala au mamlaka inayotoa arifa "
 "hii."
 
-#: capeditor/blocks.py:306
+#: capeditor/blocks.py:311
 msgid ""
 "The text describing the contact for follow-up and confirmation of the alert "
 "message"
 msgstr ""
 "Maandishi yanayoelezea mwasiliani kwa ufuatiliaji na uthibitisho wa ujumbe "
 "wa tahadhari"
 
-#: capeditor/blocks.py:307
+#: capeditor/blocks.py:312
 msgid "The text denoting the type of the subject event of the alert message"
 msgstr "Maandishi yanayoashiria aina ya tukio la somo la ujumbe wa tahadhari"
 
-#: capeditor/blocks.py:308
+#: capeditor/blocks.py:313
 msgid "The text describing the intended audience of the alert message"
 msgstr "Maandishi yanayoelezea hadhira iliyokusudiwa ya ujumbe wa tahadhari"
 
-#: capeditor/blocks.py:350 capeditor/blocks.py:359
+#: capeditor/blocks.py:355 capeditor/blocks.py:364
 #, fuzzy
 #| msgid "Description"
 msgid "Resource Description"
 msgstr "Maelezo ya Rasilimali"
 
-#: capeditor/blocks.py:351 capeditor/blocks.py:360
+#: capeditor/blocks.py:356 capeditor/blocks.py:365
 msgid "The text describing the type and content of the resource file"
 msgstr "Maandishi yanayoelezea aina na maudhui ya faili ya rasilimali"
 
-#: capeditor/blocks.py:361
+#: capeditor/blocks.py:366
 #, fuzzy
 #| msgid "Alert Resources "
 msgid "External Resource Link"
 msgstr "Kiungo cha Rasilimali za Nje"
 
-#: capeditor/blocks.py:362
+#: capeditor/blocks.py:367
 msgid ""
 "Link to external resource. This can be for example a link to related "
 "websites. "
 msgstr ""
 "Unganisha kwa rasilimali ya nje. Hii inaweza kuwa kwa mfano kiungo cha "
 "tovuti zinazohusiana."
 
-#: capeditor/blocks.py:370
+#: capeditor/blocks.py:375
 msgid "Name for the event code"
 msgstr "Jina la msimbo wa tukio"
 
-#: capeditor/blocks.py:371
+#: capeditor/blocks.py:376
 msgid "Value of the event code"
 msgstr "Thamani ya msimbo wa tukio"
 
-#: capeditor/blocks.py:441
+#: capeditor/blocks.py:467
 msgid "English"
 msgstr "Kiingereza"
 
-#: capeditor/blocks.py:445
+#: capeditor/blocks.py:471
 msgid "Geophysical"
 msgstr "Kijiofizikia"
 
-#: capeditor/blocks.py:446
+#: capeditor/blocks.py:472
 msgid "Meteorological"
 msgstr "Hali ya hewa"
 
-#: capeditor/blocks.py:447
+#: capeditor/blocks.py:473
 msgid "General emergency and public safety"
 msgstr "Dharura ya jumla na usalama wa umma"
 
-#: capeditor/blocks.py:448
+#: capeditor/blocks.py:474
 msgid "Law enforcement, military, homeland and local/private security"
 msgstr "Utekelezaji wa sheria, kijeshi, nchi na usalama wa ndani/binafsi"
 
-#: capeditor/blocks.py:449
+#: capeditor/blocks.py:475
 msgid "Rescue and recovery"
 msgstr "Kuokoa na kupona"
 
-#: capeditor/blocks.py:450
+#: capeditor/blocks.py:476
 msgid "Fire suppression and rescue"
 msgstr "Kuzuia moto na uokoaji"
 
-#: capeditor/blocks.py:451
+#: capeditor/blocks.py:477
 msgid "Medical and public health"
 msgstr "Afya ya matibabu na ya umma"
 
-#: capeditor/blocks.py:452
+#: capeditor/blocks.py:478
 msgid "Pollution and other environmental"
 msgstr "Uchafuzi na mazingira mengine"
 
-#: capeditor/blocks.py:453
+#: capeditor/blocks.py:479
 msgid "Public and private transportation"
 msgstr "Usafiri wa umma na wa kibinafsi"
 
-#: capeditor/blocks.py:454
+#: capeditor/blocks.py:480
 msgid "Utility, telecommunication, other non-transport infrastructure"
 msgstr "Huduma, mawasiliano ya simu, miundombinu mingine isiyo ya usafiri"
 
-#: capeditor/blocks.py:455
+#: capeditor/blocks.py:481
 msgid ""
 "Chemical, Biological, Radiological, Nuclear or High-Yield Explosive threat "
 "or attack"
 msgstr ""
 "Tishio au mashambulizi ya Kemikali, Baiolojia, Radiolojia, Nyuklia au Mavuno"
 " ya Juu"
 
-#: capeditor/blocks.py:456
+#: capeditor/blocks.py:482
 msgid "Other events"
 msgstr "Matukio mengine"
 
-#: capeditor/blocks.py:460
+#: capeditor/blocks.py:486
 msgid "Immediate - Responsive action SHOULD be taken immediately"
 msgstr "Hapo Hapo - Hatua ya kuitikia INATAKIWA ichukuliwe mara moja"
 
-#: capeditor/blocks.py:461
+#: capeditor/blocks.py:487
 msgid "Expected - Responsive action SHOULD be taken soon (within next hour)"
 msgstr ""
 "Inatarajiwa - Hatua ya kujibu LAZIMA ichukuliwe hivi karibuni (ndani ya saa "
 "ijayo)"
 
-#: capeditor/blocks.py:462
+#: capeditor/blocks.py:488
 msgid "Future - Responsive action SHOULD be taken in the near future"
 msgstr ""
 "Wakati Ujao - Hatua ya kuitikia LAZIMA ichukuliwe katika siku za usoni"
 
-#: capeditor/blocks.py:463
+#: capeditor/blocks.py:489
 msgid "Past - Responsive action is no longer required"
 msgstr "Zamani - Hatua ya kujibu haihitajiki tena"
 
-#: capeditor/blocks.py:464
+#: capeditor/blocks.py:490
 msgid "Unknown - Urgency not known"
 msgstr "Haijulikani - Udharura haujulikani"
 
-#: capeditor/blocks.py:468
+#: capeditor/blocks.py:494
 msgid "Extreme - Extraordinary threat to life or property"
 msgstr "Uliokithiri - Tishio lisilo la kawaida kwa maisha au mali"
 
-#: capeditor/blocks.py:469
+#: capeditor/blocks.py:495
 msgid "Severe - Significant threat to life or property"
 msgstr "Kali - Tishio kubwa kwa maisha au mali"
 
-#: capeditor/blocks.py:470
+#: capeditor/blocks.py:496
 msgid "Moderate - Possible threat to life or property"
 msgstr "Wastani - Tishio linalowezekana kwa maisha au mali"
 
-#: capeditor/blocks.py:471
+#: capeditor/blocks.py:497
 msgid "Minor - Minimal to no known threat to life or property"
 msgstr ""
 "Ndogo - Kiwango cha chini kwa tishio lisilojulikana kwa maisha au mali"
 
-#: capeditor/blocks.py:472
+#: capeditor/blocks.py:498
 msgid "Unknown - Severity unknown"
 msgstr "Haijulikani - Ukali haujulikani"
 
-#: capeditor/blocks.py:476
+#: capeditor/blocks.py:502
 msgid "Observed - Determined to have occurred or to be ongoing"
 msgstr "Imezingatiwa - Imedhamiriwa kuwa imetokea au kuwa inaendelea"
 
-#: capeditor/blocks.py:477
+#: capeditor/blocks.py:503
 msgid "Likely - Likely (percentage > ~50%)"
 msgstr "Huenda - Huenda (asilimia> ~50%)"
 
-#: capeditor/blocks.py:478
+#: capeditor/blocks.py:504
 msgid "Possible - Possible but not likely (percentage <= ~50%)"
 msgstr "Inawezekana - Inawezekana lakini haiwezekani (asilimia <= ~50%)"
 
-#: capeditor/blocks.py:479
+#: capeditor/blocks.py:505
 msgid "Unlikely - Not expected to occur (percentage ~ 0)"
 msgstr "Haiwezekani - Haitarajiwi kutokea (asilimia ~ 0)"
 
-#: capeditor/blocks.py:480
+#: capeditor/blocks.py:506
 msgid "Unknown - Certainty unknown"
 msgstr "Haijulikani - Hakika haijulikani"
 
-#: capeditor/blocks.py:483
-msgid "Language"
-msgstr "Lugha"
-
-#: capeditor/blocks.py:484
-msgid "The code denoting the language of the alert message"
-msgstr "Msimbo unaoashiria lugha ya ujumbe wa tahadhari"
+#: capeditor/blocks.py:508
+msgid "Event"
+msgstr "Tukio"
 
-#: capeditor/blocks.py:485
+#: capeditor/blocks.py:510
 msgid "Category"
 msgstr "Kategoria"
 
-#: capeditor/blocks.py:486
+#: capeditor/blocks.py:511
 msgid ""
 "The code denoting the category of the subject event of the alert message"
 msgstr "Msimbo unaoashiria aina ya tukio la somo la ujumbe wa tahadhari"
 
-#: capeditor/blocks.py:488
-msgid "Event"
-msgstr "Tukio"
+#: capeditor/blocks.py:513
+msgid "Language"
+msgstr "Lugha"
 
-#: capeditor/blocks.py:489
+#: capeditor/blocks.py:514
+msgid "The code denoting the language of the alert message"
+msgstr "Msimbo unaoashiria lugha ya ujumbe wa tahadhari"
+
+#: capeditor/blocks.py:516
 msgid "Urgency"
 msgstr "Uharaka"
 
-#: capeditor/blocks.py:490
+#: capeditor/blocks.py:517
 msgid ""
 "The code denoting the urgency of the subject event of the alert message"
 msgstr "Msimbo unaoashiria uharaka wa tukio la somo la ujumbe wa tahadhari"
 
-#: capeditor/blocks.py:492
+#: capeditor/blocks.py:519
 msgid "Severity"
 msgstr "Ukali"
 
-#: capeditor/blocks.py:493
+#: capeditor/blocks.py:520
 msgid ""
 "The code denoting the severity of the subject event of the alert message"
 msgstr "Msimbo unaoashiria ukali wa tukio la somo la ujumbe wa tahadhari"
 
-#: capeditor/blocks.py:495
+#: capeditor/blocks.py:522
 msgid "Certainty"
 msgstr "Uhakika"
 
-#: capeditor/blocks.py:496
+#: capeditor/blocks.py:523
 msgid ""
 "The code denoting the certainty of the subject event of the alert message"
 msgstr "Msimbo unaoashiria uhakika wa tukio la somo la ujumbe wa tahadhari"
 
-#: capeditor/blocks.py:498
+#: capeditor/blocks.py:525
 msgid "Headline"
 msgstr "Kichwa cha habari"
 
-#: capeditor/blocks.py:499
+#: capeditor/blocks.py:526
 msgid ""
 "The text headline of the alert message. Make it direct and actionable as "
 "possible while remaining short"
 msgstr ""
 "Kichwa cha maandishi cha ujumbe wa tahadhari. Ifanye moja kwa moja na iweze "
 "kutekelezeka iwezekanavyo huku ikisalia kuwa fupi"
 
-#: capeditor/blocks.py:501
+#: capeditor/blocks.py:528
 msgid "Description"
 msgstr "Maelezo"
 
-#: capeditor/blocks.py:503
+#: capeditor/blocks.py:530
 #, fuzzy
 #| msgid "The text describing the subject event of the alert message"
 msgid ""
 "The text describing the subject event of the alert message. An extended "
 "description of the hazard or event that occasioned this message"
 msgstr ""
 "Maandishi yanayoelezea tukio la somo la ujumbe wa tahadhari. Maelezo "
 "yaliyopanuliwa ya hatari au tukio lililosababisha ujumbe huu"
 
-#: capeditor/blocks.py:505
+#: capeditor/blocks.py:532
 msgid "Instruction"
 msgstr "Maagizo"
 
-#: capeditor/blocks.py:506
+#: capeditor/blocks.py:533
 msgid ""
 "The text describing the recommended action to be taken by recipients of the "
 "alert message"
 msgstr ""
 "Maandishi yanayoelezea hatua iliyopendekezwa kuchukuliwa na wapokeaji wa "
 "ujumbe wa arifa"
 
-#: capeditor/blocks.py:508
+#: capeditor/blocks.py:535
 msgid "Effective"
 msgstr "Ufanisi"
 
-#: capeditor/blocks.py:509
+#: capeditor/blocks.py:536
 #, fuzzy
 #| msgid "The effective time of the information of the alert message"
 msgid ""
 "The effective time of the information of the alert message. If not set, the "
 "sent date will be used"
 msgstr ""
 "Wakati unaofaa wa taarifa ya ujumbe wa tahadhari. Ikiwa haijawekwa, tarehe "
 "iliyotumwa itatumika"
 
-#: capeditor/blocks.py:511
+#: capeditor/blocks.py:538
 msgid "Onset"
 msgstr "Kuanza"
 
-#: capeditor/blocks.py:512
+#: capeditor/blocks.py:539
 msgid ""
 "The expected time of the beginning of the subject event of the alert message"
 msgstr "Muda unaotarajiwa wa mwanzo wa tukio la somo la ujumbe wa tahadhari"
 
-#: capeditor/blocks.py:514
+#: capeditor/blocks.py:541
 msgid "Expires"
 msgstr "Muda wake unaisha"
 
-#: capeditor/blocks.py:515
+#: capeditor/blocks.py:542
 msgid ""
 "The expiry time of the information of the alert message. If not set, each "
 "recipient is free to set its own policy as to when the message is no longer "
 "in effect."
 msgstr ""
 "Muda wa mwisho wa taarifa ya ujumbe wa arifa. Ikiwa haijawekwa, kila "
 "mpokeaji yuko huru kuweka sera yake mwenyewe kuhusu ni lini ujumbe haufanyi "
 "kazi tena."
 
-#: capeditor/blocks.py:518
+#: capeditor/blocks.py:545
 #, fuzzy
 #| msgid "Response type"
 msgid "Response Types"
 msgstr "Aina za Majibu"
 
-#: capeditor/blocks.py:520
+#: capeditor/blocks.py:547
 #, fuzzy
 #| msgid "Sender"
 msgid "Sender name"
 msgstr "Jina la mtumaji"
 
-#: capeditor/blocks.py:522
+#: capeditor/blocks.py:549
 msgid "Contact"
 msgstr "Wasiliana"
 
-#: capeditor/blocks.py:523 capeditor/blocks.py:550
+#: capeditor/blocks.py:550 capeditor/blocks.py:580
 msgid "Audience"
 msgstr "Hadhira"
 
-#: capeditor/blocks.py:526
+#: capeditor/blocks.py:553
 msgid "Admin Boundary"
 msgstr "Mpaka wa Utawala"
 
-#: capeditor/blocks.py:527
+#: capeditor/blocks.py:554
 msgid "Draw Polygon"
 msgstr "Chora Polygon"
 
-#: capeditor/blocks.py:529
+#: capeditor/blocks.py:556
 msgid "Geocode"
 msgstr "Msimbo wa kijiografia"
 
-#: capeditor/blocks.py:530
+#: capeditor/blocks.py:557
 msgid "Alert Area"
 msgstr "Eneo la Tahadhari"
 
-#: capeditor/blocks.py:530
+#: capeditor/blocks.py:557
 msgid "Admin Boundary, Polygon, Circle or Geocode"
 msgstr "Mpaka wa Msimamizi, Poligoni, Mduara au Msimbo wa Jiografia"
 
-#: capeditor/blocks.py:535
+#: capeditor/blocks.py:562
 #, fuzzy
 #| msgid "Resource"
 msgid "Resources"
 msgstr "Rasilimali"
 
-#: capeditor/blocks.py:535
+#: capeditor/blocks.py:562
 msgid ""
 "Additional file with supplemental information related to this alert "
 "information"
 msgstr ""
 "Faili ya ziada iliyo na maelezo ya ziada yanayohusiana na taarifa hii ya "
 "arifa"
 
-#: capeditor/blocks.py:538
+#: capeditor/blocks.py:565
 msgid "Parameter"
 msgstr "Kigezo"
 
-#: capeditor/blocks.py:538
+#: capeditor/blocks.py:565
 msgid "Parameters"
 msgstr "Vigezo"
 
-#: capeditor/blocks.py:539
+#: capeditor/blocks.py:566
 #, fuzzy
 #| msgid "Event"
 msgid "Event Code"
 msgstr "Msimbo wa Tukio"
 
-#: capeditor/blocks.py:539
+#: capeditor/blocks.py:566
 #, fuzzy
 #| msgid "Event"
 msgid "Event codes"
 msgstr "Misimbo ya tukio"
 
-#: capeditor/blocks.py:545
+#: capeditor/blocks.py:575
 msgid "Hazard"
 msgstr "Hatari"
 
-#: capeditor/blocks.py:554
+#: capeditor/blocks.py:584
 #, fuzzy
 #| msgid "Contact"
 msgid "Contact Detail"
 msgstr "Maelezo ya Mawasiliano"
 
 #: capeditor/models.py:35
 #, fuzzy
@@ -830,15 +830,15 @@
 #~ msgid "Immediate"
 #~ msgstr "Mara moja"
 
 #~ msgid "Expected"
 #~ msgstr "Inatarajiwa"
 
 #~ msgid "Future"
-#~ msgstr "Baadaye"
+#~ msgstr "Wakati ujao"
 
 #~ msgid "Past"
 #~ msgstr "Zamani"
 
 #~ msgid "Unknown"
 #~ msgstr "Haijulikani"
```

### Comparing `capeditor-0.2.7/capeditor/migrations/0001_initial.py` & `capeditor-0.2.8/capeditor/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.7/capeditor/models.py` & `capeditor-0.2.8/capeditor/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -315,7 +315,9 @@
                 areas.append(area.get("areaDesc"))
 
         return ", ".join(areas)
 
     @property
     def xml_link(self):
         return None
+    
+
```

### Comparing `capeditor-0.2.7/capeditor/renderers.py` & `capeditor-0.2.8/capeditor/renderers.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.7/capeditor/serializers.py` & `capeditor-0.2.8/capeditor/serializers.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.7/capeditor/static/capeditor/css/cap_detail_page.css` & `capeditor-0.2.8/capeditor/static/capeditor/css/cap_detail_page.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.7/capeditor/static/capeditor/css/widget/circle-widget.css` & `capeditor-0.2.8/capeditor/static/capeditor/css/widget/circle-widget.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.7/capeditor/static/capeditor/css/widget/polygon-widget.css` & `capeditor-0.2.8/capeditor/static/capeditor/css/widget/polygon-widget.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.7/capeditor/static/capeditor/js/cap_accordion.js` & `capeditor-0.2.8/capeditor/static/capeditor/js/cap_accordion.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.7/capeditor/static/capeditor/js/widget/boundary-polygon-widget-telepath.js` & `capeditor-0.2.8/capeditor/static/capeditor/js/widget/boundary-polygon-widget-telepath.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.7/capeditor/static/capeditor/js/widget/boundary-polygon-widget.js` & `capeditor-0.2.8/capeditor/static/capeditor/js/widget/boundary-polygon-widget.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.7/capeditor/static/capeditor/js/widget/circle-widget-telepath.js` & `capeditor-0.2.8/capeditor/static/capeditor/js/widget/circle-widget-telepath.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.7/capeditor/static/capeditor/js/widget/circle-widget.js` & `capeditor-0.2.8/capeditor/static/capeditor/js/widget/circle-widget.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.7/capeditor/static/capeditor/js/widget/conditional_fields.js` & `capeditor-0.2.8/capeditor/static/capeditor/js/conditional_fields.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.7/capeditor/static/capeditor/js/widget/polygon-widget-telepath.js` & `capeditor-0.2.8/capeditor/static/capeditor/js/widget/polygon-widget-telepath.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.7/capeditor/static/capeditor/js/widget/polygon-widget.js` & `capeditor-0.2.8/capeditor/static/capeditor/js/widget/polygon-widget.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.7/capeditor/templates/capeditor/cap_alert_page.html` & `capeditor-0.2.8/capeditor/templates/capeditor/cap_alert_page.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.7/capeditor/templates/capeditor/icons/cap-alert-full.svg` & `capeditor-0.2.8/capeditor/templates/capeditor/icons/cap-alert-full.svg`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.7/capeditor/templates/capeditor/icons/cap-alert.svg` & `capeditor-0.2.8/capeditor/templates/capeditor/icons/cap-alert.svg`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.7/capeditor/templates/capeditor/widgets/circle_widget.html` & `capeditor-0.2.8/capeditor/templates/capeditor/widgets/circle_widget.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.7/capeditor.egg-info/PKG-INFO` & `capeditor-0.2.8/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: capeditor
-Version: 0.2.7
-Summary: Wagtail based CAP Editor
-Home-page: https://github.com/wmo-raf/cap-editor
-Author: Grace Amondi, Erick Otenyo
-Author-email: miswa.grace@gmail.com, otenyo.erick@gmail.com
-License: MIT
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-
 # CAP Editor  <img style="float: right;" height="40" src="images/caplogo.jpeg" markdown="1"> 
 [![Upload Python Package](https://github.com/wmo-raf/cap-editor/actions/workflows/publish.yml/badge.svg)](https://github.com/wmo-raf/cap-editor/actions/workflows/publish.yml)
 
 A Wagtail Commmon Alerting Protocol (CAP) Editor python package
 installable as an app on any wagtail project (version\>=4.1).
 
 The **Common Alerting Protocol (CAP)** provides an open, non-proprietary
@@ -51,27 +30,21 @@
             -   [B. Alert Info](#b.-alert-info)
             -   [C. Alert Area](#c.-alert-area)
             -   [D. Alert Resource](#d.-alert-resource)
     -   [Integrations](#integrations)
     
 ## Quick start
 
-#### 1. Clone repository
+#### 1. Install in virualenvironment using pip
 
 ``` sh
-git clone https://github.com/wmo-raf/cap-editor.git
+pip install capeditor
 ```
 
-#### 2. Install in virualenvironment using pip
-
-``` sh
-pip install path_to/capeditor/dist/capeditor-{version}.tar.gz
-```
-
-#### 3. Configure settings
+#### 2. Configure settings
 
 In your `settings.py` or `settings/base.py`, within the installed apps,
 include the `rest_framework, rest_framework_xml` and `capeditor` as
 below:
 
 ``` py
 INSTALLED_APPS = [
@@ -92,31 +65,15 @@
     ),
     'DEFAULT_PARSER_CLASSES': (
         'rest_framework_xml.parsers.XMLParser',
     ),
 }
 ```
 
-#### 4. Include the cap urls
-
-In `urls.py`, include the cap urls as below. This is where the cap api
-for listed (`/cap/caps.xml`) and detailed(`/cap/{cap_id}.xml`) cap view
-will be hosted.
-
-``` py
-from capeditor import urls as cap_urls
-
-urlpatterns = [
-    # ...
-    path('cap', include(cap_urls))
-
-]
-```
-
-#### 5. Run model migrations
+#### 3. Run model migrations
 
 ``` sh
 python manage.py migrate
 ```
 
 ## Usage
 
@@ -242,54 +199,10 @@
 Multiple instances of this section are allowed. It contains the
 **Description (resourceDesc), MIME Type (mimeType), File Size (size),
 URI (uri), Dereferenced URI (derefUri) and Digest (digest)**
 
 ## Integrations
 
 To integrate the alerts to another wagtail page and include in
-templates, for example in the home page follow the instructions below:
+templates, for example in the home page refer to sandbox folder for sample standalone.
 
-Call the alerts in your models.py under the 'get_context' method:
 
-``` py
-from capeditor.models import Alert
-
-class HomePage(Page):
-
-    # ...
-
-
-    def get_context(self, request, *args, **kwargs):
-        context =super().get_context(request, *args, **kwargs)
-       
-        context['alerts'] = Alert.objects.live().public()
-        context['latest_alerts'] = context['alerts'][:3]
-        return context  
-```
-
-Parse the alerts in the home template:
-
-``` django
-
-{% for alert in latest_alerts.all %}
-    
-    <p>{{alert.sent}}</p>
-
-    <!-- info list  -->
-    {% for info in alert.alert_info.all %}
-        {% if alerts %}
-
-            <p>{{info.event}}</p>
-            <p>{{info.get_severity_display}}</p>
-
-            <!-- area list  -->
-            {% for alert_area in info.alert_areas.values%}
-                <p>{{alert_area.areaDesc}}</p>
-                <p>{{ alert_area.area }}</p>
-            {% endfor %}
-
-            <!-- other fields  -->
-
-        {% endif %}
-    {% endfor %}
-{% endfor %}
-```
```

### Comparing `capeditor-0.2.7/capeditor.egg-info/SOURCES.txt` & `capeditor-0.2.8/capeditor.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -35,19 +35,19 @@
 capeditor/migrations/0001_initial.py
 capeditor/migrations/__init__.py
 capeditor/static/capeditor/css/cap_detail_page.css
 capeditor/static/capeditor/css/widget/boundary-widget.css
 capeditor/static/capeditor/css/widget/circle-widget.css
 capeditor/static/capeditor/css/widget/polygon-widget.css
 capeditor/static/capeditor/js/cap_accordion.js
+capeditor/static/capeditor/js/conditional_fields.js
 capeditor/static/capeditor/js/widget/boundary-polygon-widget-telepath.js
 capeditor/static/capeditor/js/widget/boundary-polygon-widget.js
 capeditor/static/capeditor/js/widget/circle-widget-telepath.js
 capeditor/static/capeditor/js/widget/circle-widget.js
-capeditor/static/capeditor/js/widget/conditional_fields.js
 capeditor/static/capeditor/js/widget/polygon-widget-telepath.js
 capeditor/static/capeditor/js/widget/polygon-widget.js
 capeditor/templates/capeditor/cap_alert_page.html
 capeditor/templates/capeditor/icons/cap-alert-full.svg
 capeditor/templates/capeditor/icons/cap-alert.svg
 capeditor/templates/capeditor/widgets/boundary_polygon_widget.html
 capeditor/templates/capeditor/widgets/circle_widget.html
```

### Comparing `capeditor-0.2.7/setup.cfg` & `capeditor-0.2.8/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = capeditor
-version = 0.2.7
+version = 0.2.8
 description = Wagtail based CAP Editor
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/cap-editor
 author = Grace Amondi, Erick Otenyo
 author_email = miswa.grace@gmail.com, otenyo.erick@gmail.com
 license = MIT
```

