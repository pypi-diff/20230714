# Comparing `tmp/garpixcms-4.5.0rc2.tar.gz` & `tmp/garpixcms-4.5.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garpixcms-4.5.0rc2.tar", last modified: Mon Jul  3 10:19:24 2023, max compression
+gzip compressed data, was "garpixcms-4.5.0rc3.tar", last modified: Mon Jul  3 10:25:46 2023, max compression
```

## Comparing `garpixcms-4.5.0rc2.tar` & `garpixcms-4.5.0rc3.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:19:24.163143 garpixcms-4.5.0rc2/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       30 2023-07-03 10:19:24.000000 garpixcms-4.5.0rc2/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1769 2023-07-03 10:19:24.162984 garpixcms-4.5.0rc2/PKG-INFO
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:19:24.149457 garpixcms-4.5.0rc2/garpixcms/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)    13969 2023-07-03 10:18:38.000000 garpixcms-4.5.0rc2/garpixcms/CHANGELOG.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1084 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/CONTRIBUTING.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       30 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1207 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/README.rst
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:19:24.150696 garpixcms-4.5.0rc2/garpixcms/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      161 2023-04-18 20:28:30.000000 garpixcms-4.5.0rc2/garpixcms/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      387 2023-04-18 20:28:30.000000 garpixcms-4.5.0rc2/garpixcms/__pycache__/apps.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6796 2023-04-18 20:28:30.000000 garpixcms-4.5.0rc2/garpixcms/__pycache__/settings.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1743 2023-04-18 20:28:31.000000 garpixcms-4.5.0rc2/garpixcms/__pycache__/urls.cpython-38.pyc
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:19:24.150928 garpixcms-4.5.0rc2/garpixcms/admin/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       36 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/admin/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:19:24.151166 garpixcms-4.5.0rc2/garpixcms/admin/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      205 2023-04-18 20:28:31.000000 garpixcms-4.5.0rc2/garpixcms/admin/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      487 2023-04-18 20:28:31.000000 garpixcms-4.5.0rc2/garpixcms/admin/__pycache__/page.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      173 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/admin/page.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       93 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/apps.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:19:24.151381 garpixcms-4.5.0rc2/garpixcms/contexts/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/contexts/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      691 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/contexts/global_context.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:19:24.151490 garpixcms-4.5.0rc2/garpixcms/management/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/management/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:19:24.151581 garpixcms-4.5.0rc2/garpixcms/management/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      172 2023-05-10 14:01:00.000000 garpixcms-4.5.0rc2/garpixcms/management/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:19:24.151784 garpixcms-4.5.0rc2/garpixcms/management/commands/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/management/commands/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      872 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/management/commands/update_user_module.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:19:24.151987 garpixcms-4.5.0rc2/garpixcms/middleware/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/middleware/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:19:24.152241 garpixcms-4.5.0rc2/garpixcms/middleware/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      172 2023-05-10 14:00:43.000000 garpixcms-4.5.0rc2/garpixcms/middleware/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2037 2023-05-10 14:00:43.000000 garpixcms-4.5.0rc2/garpixcms/middleware/__pycache__/locale.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2196 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/middleware/locale.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:19:24.154463 garpixcms-4.5.0rc2/garpixcms/models/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       31 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/models/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:19:24.155027 garpixcms-4.5.0rc2/garpixcms/models/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      201 2023-04-18 20:28:31.000000 garpixcms-4.5.0rc2/garpixcms/models/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      818 2023-04-18 20:28:31.000000 garpixcms-4.5.0rc2/garpixcms/models/__pycache__/page.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      413 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/models/page.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8440 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/settings.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1705 2023-07-03 10:19:09.000000 garpixcms-4.5.0rc2/garpixcms/setup.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:19:24.147589 garpixcms-4.5.0rc2/garpixcms/static/
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:19:24.147772 garpixcms-4.5.0rc2/garpixcms/static/admin/
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:19:24.159679 garpixcms-4.5.0rc2/garpixcms/static/admin/css/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8440 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/static/admin/css/autocomplete.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)    22662 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/static/admin/css/base.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6469 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/static/admin/css/changelists.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      355 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/static/admin/css/dashboard.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      423 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/static/admin/css/fonts.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8370 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/static/admin/css/forms.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1185 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/static/admin/css/login.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2505 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/static/admin/css/nav_sidebar.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)    18344 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/static/admin/css/responsive.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1741 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/static/admin/css/responsive_rtl.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3487 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/static/admin/css/rtl.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      502 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/static/admin/css/tabbed_translation_fields.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)    10010 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/static/admin/css/widgets.css
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:19:24.160843 garpixcms-4.5.0rc2/garpixcms/static/admin/img/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      908 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/static/admin/img/icon-addlink.svg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      825 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/static/admin/img/icon-changelink.svg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      218 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/static/admin/img/icon-custom-checked.svg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      705 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/static/admin/img/icon-deletelink.svg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      930 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/static/admin/img/search.svg
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:19:24.160966 garpixcms-4.5.0rc2/garpixcms/static/admin/js/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      291 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/static/admin/js/admin.js
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:19:24.147954 garpixcms-4.5.0rc2/garpixcms/templates/
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:19:24.161318 garpixcms-4.5.0rc2/garpixcms/templates/admin/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4421 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/templates/admin/app_list.html
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4395 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/templates/admin/base.html
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      809 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/templates/admin/base_site.html
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:19:24.161433 garpixcms-4.5.0rc2/garpixcms/templates/garpixcms/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      450 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/templates/garpixcms/base.html
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:19:24.161780 garpixcms-4.5.0rc2/garpixcms/templates/garpixcms/include/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      730 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/templates/garpixcms/include/footer.html
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      642 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/templates/garpixcms/include/header.html
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      428 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/templates/garpixcms/include/login.html
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:19:24.162003 garpixcms-4.5.0rc2/garpixcms/templates/garpixcms/menus/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      202 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/templates/garpixcms/menus/footer_menu.html
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      369 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/templates/garpixcms/menus/header_menu.html
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:19:24.162341 garpixcms-4.5.0rc2/garpixcms/templates/garpixcms/pages/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      139 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/templates/garpixcms/pages/default.html
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      202 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/templates/garpixcms/pages/home.html
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      346 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/templates/garpixcms/pages/login.html
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:19:24.162567 garpixcms-4.5.0rc2/garpixcms/translation/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       49 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/translation/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:19:24.162793 garpixcms-4.5.0rc2/garpixcms/translation/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      224 2023-04-18 20:28:31.000000 garpixcms-4.5.0rc2/garpixcms/translation/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      502 2023-04-18 20:28:31.000000 garpixcms-4.5.0rc2/garpixcms/translation/__pycache__/page.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      189 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/translation/page.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1842 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc2/garpixcms/urls.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:19:24.150112 garpixcms-4.5.0rc2/garpixcms.egg-info/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1769 2023-07-03 10:19:24.000000 garpixcms-4.5.0rc2/garpixcms.egg-info/PKG-INFO
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2848 2023-07-03 10:19:24.000000 garpixcms-4.5.0rc2/garpixcms.egg-info/SOURCES.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-07-03 10:19:24.000000 garpixcms-4.5.0rc2/garpixcms.egg-info/dependency_links.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-07-03 10:19:24.000000 garpixcms-4.5.0rc2/garpixcms.egg-info/not-zip-safe
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      405 2023-07-03 10:19:24.000000 garpixcms-4.5.0rc2/garpixcms.egg-info/requires.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       10 2023-07-03 10:19:24.000000 garpixcms-4.5.0rc2/garpixcms.egg-info/top_level.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-07-03 10:19:24.163186 garpixcms-4.5.0rc2/setup.cfg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1705 2023-07-03 10:19:24.000000 garpixcms-4.5.0rc2/setup.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:25:46.390146 garpixcms-4.5.0rc3/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       30 2023-07-03 10:25:46.000000 garpixcms-4.5.0rc3/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1769 2023-07-03 10:25:46.389968 garpixcms-4.5.0rc3/PKG-INFO
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:25:46.379286 garpixcms-4.5.0rc3/garpixcms/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)    14044 2023-07-03 10:25:23.000000 garpixcms-4.5.0rc3/garpixcms/CHANGELOG.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1084 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/CONTRIBUTING.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       30 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1207 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/README.rst
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:25:46.381090 garpixcms-4.5.0rc3/garpixcms/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      161 2023-04-18 20:28:30.000000 garpixcms-4.5.0rc3/garpixcms/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      387 2023-04-18 20:28:30.000000 garpixcms-4.5.0rc3/garpixcms/__pycache__/apps.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6796 2023-04-18 20:28:30.000000 garpixcms-4.5.0rc3/garpixcms/__pycache__/settings.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1743 2023-04-18 20:28:31.000000 garpixcms-4.5.0rc3/garpixcms/__pycache__/urls.cpython-38.pyc
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:25:46.381355 garpixcms-4.5.0rc3/garpixcms/admin/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       36 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/admin/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:25:46.381801 garpixcms-4.5.0rc3/garpixcms/admin/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      205 2023-04-18 20:28:31.000000 garpixcms-4.5.0rc3/garpixcms/admin/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      487 2023-04-18 20:28:31.000000 garpixcms-4.5.0rc3/garpixcms/admin/__pycache__/page.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      173 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/admin/page.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       93 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/apps.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:25:46.382079 garpixcms-4.5.0rc3/garpixcms/contexts/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/contexts/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      691 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/contexts/global_context.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:25:46.382206 garpixcms-4.5.0rc3/garpixcms/management/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/management/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:25:46.382303 garpixcms-4.5.0rc3/garpixcms/management/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      172 2023-05-10 14:01:00.000000 garpixcms-4.5.0rc3/garpixcms/management/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:25:46.383080 garpixcms-4.5.0rc3/garpixcms/management/commands/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/management/commands/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      872 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/management/commands/update_user_module.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:25:46.383498 garpixcms-4.5.0rc3/garpixcms/middleware/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/middleware/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:25:46.383823 garpixcms-4.5.0rc3/garpixcms/middleware/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      172 2023-05-10 14:00:43.000000 garpixcms-4.5.0rc3/garpixcms/middleware/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2037 2023-05-10 14:00:43.000000 garpixcms-4.5.0rc3/garpixcms/middleware/__pycache__/locale.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2196 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/middleware/locale.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:25:46.384371 garpixcms-4.5.0rc3/garpixcms/models/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       31 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/models/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:25:46.384683 garpixcms-4.5.0rc3/garpixcms/models/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      201 2023-04-18 20:28:31.000000 garpixcms-4.5.0rc3/garpixcms/models/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      818 2023-04-18 20:28:31.000000 garpixcms-4.5.0rc3/garpixcms/models/__pycache__/page.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      413 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/models/page.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8440 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/settings.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1705 2023-07-03 10:25:06.000000 garpixcms-4.5.0rc3/garpixcms/setup.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:25:46.376939 garpixcms-4.5.0rc3/garpixcms/static/
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:25:46.377137 garpixcms-4.5.0rc3/garpixcms/static/admin/
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:25:46.386855 garpixcms-4.5.0rc3/garpixcms/static/admin/css/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8440 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/static/admin/css/autocomplete.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)    22662 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/static/admin/css/base.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6469 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/static/admin/css/changelists.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      355 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/static/admin/css/dashboard.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      423 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/static/admin/css/fonts.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8370 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/static/admin/css/forms.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1185 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/static/admin/css/login.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2505 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/static/admin/css/nav_sidebar.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)    18344 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/static/admin/css/responsive.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1741 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/static/admin/css/responsive_rtl.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3487 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/static/admin/css/rtl.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      502 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/static/admin/css/tabbed_translation_fields.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)    10010 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/static/admin/css/widgets.css
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:25:46.387451 garpixcms-4.5.0rc3/garpixcms/static/admin/img/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      908 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/static/admin/img/icon-addlink.svg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      825 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/static/admin/img/icon-changelink.svg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      218 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/static/admin/img/icon-custom-checked.svg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      705 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/static/admin/img/icon-deletelink.svg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      930 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/static/admin/img/search.svg
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:25:46.387576 garpixcms-4.5.0rc3/garpixcms/static/admin/js/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      291 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/static/admin/js/admin.js
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:25:46.377343 garpixcms-4.5.0rc3/garpixcms/templates/
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:25:46.387920 garpixcms-4.5.0rc3/garpixcms/templates/admin/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4421 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/templates/admin/app_list.html
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4395 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/templates/admin/base.html
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      809 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/templates/admin/base_site.html
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:25:46.388033 garpixcms-4.5.0rc3/garpixcms/templates/garpixcms/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      450 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/templates/garpixcms/base.html
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:25:46.388538 garpixcms-4.5.0rc3/garpixcms/templates/garpixcms/include/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      730 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/templates/garpixcms/include/footer.html
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      642 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/templates/garpixcms/include/header.html
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      428 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/templates/garpixcms/include/login.html
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:25:46.388814 garpixcms-4.5.0rc3/garpixcms/templates/garpixcms/menus/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      202 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/templates/garpixcms/menus/footer_menu.html
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      369 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/templates/garpixcms/menus/header_menu.html
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:25:46.389189 garpixcms-4.5.0rc3/garpixcms/templates/garpixcms/pages/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      139 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/templates/garpixcms/pages/default.html
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      202 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/templates/garpixcms/pages/home.html
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      346 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/templates/garpixcms/pages/login.html
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:25:46.389488 garpixcms-4.5.0rc3/garpixcms/translation/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       49 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/translation/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:25:46.389774 garpixcms-4.5.0rc3/garpixcms/translation/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      224 2023-04-18 20:28:31.000000 garpixcms-4.5.0rc3/garpixcms/translation/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      502 2023-04-18 20:28:31.000000 garpixcms-4.5.0rc3/garpixcms/translation/__pycache__/page.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      189 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/translation/page.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1842 2023-04-18 19:40:20.000000 garpixcms-4.5.0rc3/garpixcms/urls.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-07-03 10:25:46.380487 garpixcms-4.5.0rc3/garpixcms.egg-info/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1769 2023-07-03 10:25:46.000000 garpixcms-4.5.0rc3/garpixcms.egg-info/PKG-INFO
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2848 2023-07-03 10:25:46.000000 garpixcms-4.5.0rc3/garpixcms.egg-info/SOURCES.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-07-03 10:25:46.000000 garpixcms-4.5.0rc3/garpixcms.egg-info/dependency_links.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-07-03 10:25:46.000000 garpixcms-4.5.0rc3/garpixcms.egg-info/not-zip-safe
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      405 2023-07-03 10:25:46.000000 garpixcms-4.5.0rc3/garpixcms.egg-info/requires.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       10 2023-07-03 10:25:46.000000 garpixcms-4.5.0rc3/garpixcms.egg-info/top_level.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-07-03 10:25:46.390195 garpixcms-4.5.0rc3/setup.cfg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1705 2023-07-03 10:25:46.000000 garpixcms-4.5.0rc3/setup.py
```

### Comparing `garpixcms-4.5.0rc2/PKG-INFO` & `garpixcms-4.5.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpixcms
-Version: 4.5.0rc2
+Version: 4.5.0rc3
 Home-page: https://github.com/garpixcms/garpixcms
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `garpixcms-4.5.0rc2/garpixcms/CHANGELOG.md` & `garpixcms-4.5.0rc3/garpixcms/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+### 4.5.0-rc3 (03.07.2023)
+
+- Upgrade `garpix_utils` to version 1.9.0-rc3
+
 ### 4.5.0-rc2 (03.07.2023)
 
 - Upgrade `garpix_utils` to version 1.9.0-rc2
 
 ### 4.5.0-rc1 (26.06.2023)
 
 - Upgrade `garpix_utils` to version 1.9.0-rc1
```

### Comparing `garpixcms-4.5.0rc2/garpixcms/CONTRIBUTING.md` & `garpixcms-4.5.0rc3/garpixcms/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `garpixcms-4.5.0rc2/garpixcms/README.rst` & `garpixcms-4.5.0rc3/garpixcms/README.rst`

 * *Files identical despite different names*

### Comparing `garpixcms-4.5.0rc2/garpixcms/__pycache__/settings.cpython-38.pyc` & `garpixcms-4.5.0rc3/garpixcms/__pycache__/settings.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpixcms-4.5.0rc2/garpixcms/__pycache__/urls.cpython-38.pyc` & `garpixcms-4.5.0rc3/garpixcms/__pycache__/urls.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpixcms-4.5.0rc2/garpixcms/contexts/global_context.py` & `garpixcms-4.5.0rc3/garpixcms/contexts/global_context.py`

 * *Files identical despite different names*

### Comparing `garpixcms-4.5.0rc2/garpixcms/management/commands/update_user_module.py` & `garpixcms-4.5.0rc3/garpixcms/management/commands/update_user_module.py`

 * *Files identical despite different names*

### Comparing `garpixcms-4.5.0rc2/garpixcms/middleware/__pycache__/locale.cpython-38.pyc` & `garpixcms-4.5.0rc3/garpixcms/middleware/__pycache__/locale.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpixcms-4.5.0rc2/garpixcms/middleware/locale.py` & `garpixcms-4.5.0rc3/garpixcms/middleware/locale.py`

 * *Files identical despite different names*

### Comparing `garpixcms-4.5.0rc2/garpixcms/models/__pycache__/page.cpython-38.pyc` & `garpixcms-4.5.0rc3/garpixcms/models/__pycache__/page.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpixcms-4.5.0rc2/garpixcms/settings.py` & `garpixcms-4.5.0rc3/garpixcms/settings.py`

 * *Files identical despite different names*

### Comparing `garpixcms-4.5.0rc2/garpixcms/setup.py` & `garpixcms-4.5.0rc3/garpixcms/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpixcms')
 
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpixcms',
-    version='4.5.0-rc2',
+    version='4.5.0-rc3',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpixcms',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
@@ -27,15 +27,15 @@
         'Framework :: Django',
         'Programming Language :: Python :: 3.8',
     ],
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         'Django >= 3.1, < 4',
-        'garpix_utils == 1.9.0-rc2',
+        'garpix_utils == 1.9.0-rc3',
         'garpix_page == 2.48.0',
         'garpix_menu == 1.16.0',
         'eqator == 2.7.0',
         'garpix_auth == 2.3.0',
         'garpix_notify == 5.16.0',
         'garpix_user == 3.8.1',
         'garpix_package == 2.0.1',
```

### Comparing `garpixcms-4.5.0rc2/garpixcms/static/admin/css/autocomplete.css` & `garpixcms-4.5.0rc3/garpixcms/static/admin/css/autocomplete.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.5.0rc2/garpixcms/static/admin/css/base.css` & `garpixcms-4.5.0rc3/garpixcms/static/admin/css/base.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.5.0rc2/garpixcms/static/admin/css/changelists.css` & `garpixcms-4.5.0rc3/garpixcms/static/admin/css/changelists.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.5.0rc2/garpixcms/static/admin/css/forms.css` & `garpixcms-4.5.0rc3/garpixcms/static/admin/css/forms.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.5.0rc2/garpixcms/static/admin/css/login.css` & `garpixcms-4.5.0rc3/garpixcms/static/admin/css/login.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.5.0rc2/garpixcms/static/admin/css/nav_sidebar.css` & `garpixcms-4.5.0rc3/garpixcms/static/admin/css/nav_sidebar.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.5.0rc2/garpixcms/static/admin/css/responsive.css` & `garpixcms-4.5.0rc3/garpixcms/static/admin/css/responsive.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.5.0rc2/garpixcms/static/admin/css/responsive_rtl.css` & `garpixcms-4.5.0rc3/garpixcms/static/admin/css/responsive_rtl.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.5.0rc2/garpixcms/static/admin/css/rtl.css` & `garpixcms-4.5.0rc3/garpixcms/static/admin/css/rtl.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.5.0rc2/garpixcms/static/admin/css/widgets.css` & `garpixcms-4.5.0rc3/garpixcms/static/admin/css/widgets.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.5.0rc2/garpixcms/static/admin/img/icon-addlink.svg` & `garpixcms-4.5.0rc3/garpixcms/static/admin/img/icon-addlink.svg`

 * *Files identical despite different names*

### Comparing `garpixcms-4.5.0rc2/garpixcms/static/admin/img/icon-changelink.svg` & `garpixcms-4.5.0rc3/garpixcms/static/admin/img/icon-changelink.svg`

 * *Files identical despite different names*

### Comparing `garpixcms-4.5.0rc2/garpixcms/static/admin/img/icon-deletelink.svg` & `garpixcms-4.5.0rc3/garpixcms/static/admin/img/icon-deletelink.svg`

 * *Files identical despite different names*

### Comparing `garpixcms-4.5.0rc2/garpixcms/static/admin/img/search.svg` & `garpixcms-4.5.0rc3/garpixcms/static/admin/img/search.svg`

 * *Files identical despite different names*

### Comparing `garpixcms-4.5.0rc2/garpixcms/templates/admin/app_list.html` & `garpixcms-4.5.0rc3/garpixcms/templates/admin/app_list.html`

 * *Files identical despite different names*

### Comparing `garpixcms-4.5.0rc2/garpixcms/templates/admin/base.html` & `garpixcms-4.5.0rc3/garpixcms/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `garpixcms-4.5.0rc2/garpixcms/templates/admin/base_site.html` & `garpixcms-4.5.0rc3/garpixcms/templates/admin/base_site.html`

 * *Files identical despite different names*

### Comparing `garpixcms-4.5.0rc2/garpixcms/templates/garpixcms/include/footer.html` & `garpixcms-4.5.0rc3/garpixcms/templates/garpixcms/include/footer.html`

 * *Files identical despite different names*

### Comparing `garpixcms-4.5.0rc2/garpixcms/templates/garpixcms/include/header.html` & `garpixcms-4.5.0rc3/garpixcms/templates/garpixcms/include/header.html`

 * *Files identical despite different names*

### Comparing `garpixcms-4.5.0rc2/garpixcms/urls.py` & `garpixcms-4.5.0rc3/garpixcms/urls.py`

 * *Files identical despite different names*

### Comparing `garpixcms-4.5.0rc2/garpixcms.egg-info/PKG-INFO` & `garpixcms-4.5.0rc3/garpixcms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpixcms
-Version: 4.5.0rc2
+Version: 4.5.0rc3
 Home-page: https://github.com/garpixcms/garpixcms
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `garpixcms-4.5.0rc2/garpixcms.egg-info/SOURCES.txt` & `garpixcms-4.5.0rc3/garpixcms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `garpixcms-4.5.0rc2/setup.py` & `garpixcms-4.5.0rc3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpixcms')
 
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpixcms',
-    version='4.5.0-rc2',
+    version='4.5.0-rc3',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpixcms',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
@@ -27,15 +27,15 @@
         'Framework :: Django',
         'Programming Language :: Python :: 3.8',
     ],
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         'Django >= 3.1, < 4',
-        'garpix_utils == 1.9.0-rc2',
+        'garpix_utils == 1.9.0-rc3',
         'garpix_page == 2.48.0',
         'garpix_menu == 1.16.0',
         'eqator == 2.7.0',
         'garpix_auth == 2.3.0',
         'garpix_notify == 5.16.0',
         'garpix_user == 3.8.1',
         'garpix_package == 2.0.1',
```

