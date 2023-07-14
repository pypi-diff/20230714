# Comparing `tmp/cenas-1.1.tar.gz` & `tmp/cenas-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cenas-1.1.tar", last modified: Fri Jul 14 11:52:09 2023, max compression
+gzip compressed data, was "cenas-1.1.1.tar", last modified: Fri Jul 14 12:19:15 2023, max compression
```

## Comparing `cenas-1.1.tar` & `cenas-1.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-14 11:52:09.933248 cenas-1.1/
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       47 2023-07-14 11:52:09.933248 cenas-1.1/PKG-INFO
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)        6 2023-07-14 11:35:05.000000 cenas-1.1/README.md
-drwxrwxr-x   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-14 11:52:09.933248 cenas-1.1/cenas/
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-13 08:46:15.000000 cenas-1.1/cenas/__init__.py
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       63 2023-07-13 08:46:15.000000 cenas-1.1/cenas/admin.py
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      142 2023-07-14 11:43:46.000000 cenas-1.1/cenas/apps.py
-drwxrwxr-x   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-14 11:52:09.933248 cenas-1.1/cenas/migrations/
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-13 08:46:15.000000 cenas-1.1/cenas/migrations/__init__.py
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       57 2023-07-13 08:46:15.000000 cenas-1.1/cenas/models.py
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       60 2023-07-13 08:46:15.000000 cenas-1.1/cenas/tests.py
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      198 2023-07-13 10:45:15.000000 cenas-1.1/cenas/urls.py
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      225 2023-07-13 11:25:45.000000 cenas-1.1/cenas/views.py
-drwxrwxr-x   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-14 11:52:09.933248 cenas-1.1/cenas.egg-info/
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       47 2023-07-14 11:52:09.000000 cenas-1.1/cenas.egg-info/PKG-INFO
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      413 2023-07-14 11:52:09.000000 cenas-1.1/cenas.egg-info/SOURCES.txt
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)        1 2023-07-14 11:52:09.000000 cenas-1.1/cenas.egg-info/dependency_links.txt
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       42 2023-07-14 11:52:09.000000 cenas-1.1/cenas.egg-info/entry_points.txt
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)        7 2023-07-14 11:52:09.000000 cenas-1.1/cenas.egg-info/requires.txt
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       13 2023-07-14 11:52:09.000000 cenas-1.1/cenas.egg-info/top_level.txt
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       38 2023-07-14 11:52:09.933248 cenas-1.1/setup.cfg
--rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      346 2023-07-14 11:42:34.000000 cenas-1.1/setup.py
-drwxrwxr-x   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-14 11:52:09.933248 cenas-1.1/webapp/
--rw-r--r--   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-13 08:44:19.000000 cenas-1.1/webapp/__init__.py
--rw-r--r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      389 2023-07-13 08:44:19.000000 cenas-1.1/webapp/asgi.py
--rw-r--r--   0 cerqueiraf  (1000) cerqueiraf  (1000)     3252 2023-07-14 11:44:23.000000 cenas-1.1/webapp/settings.py
--rw-r--r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      871 2023-07-13 10:50:44.000000 cenas-1.1/webapp/urls.py
--rw-r--r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      389 2023-07-13 08:44:19.000000 cenas-1.1/webapp/wsgi.py
+drwxrwxr-x   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-14 12:19:15.793610 cenas-1.1.1/
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       49 2023-07-14 12:19:15.793610 cenas-1.1.1/PKG-INFO
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)        6 2023-07-14 11:35:05.000000 cenas-1.1.1/README.md
+drwxrwxr-x   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-14 12:19:15.789610 cenas-1.1.1/cenas/
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-13 08:46:15.000000 cenas-1.1.1/cenas/__init__.py
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       63 2023-07-13 08:46:15.000000 cenas-1.1.1/cenas/admin.py
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      142 2023-07-14 11:43:46.000000 cenas-1.1.1/cenas/apps.py
+drwxrwxr-x   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-14 12:19:15.793610 cenas-1.1.1/cenas/migrations/
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-13 08:46:15.000000 cenas-1.1.1/cenas/migrations/__init__.py
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       57 2023-07-13 08:46:15.000000 cenas-1.1.1/cenas/models.py
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       60 2023-07-13 08:46:15.000000 cenas-1.1.1/cenas/tests.py
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      198 2023-07-13 10:45:15.000000 cenas-1.1.1/cenas/urls.py
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      362 2023-07-14 12:10:33.000000 cenas-1.1.1/cenas/views.py
+drwxrwxr-x   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-14 12:19:15.793610 cenas-1.1.1/cenas.egg-info/
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       49 2023-07-14 12:19:15.000000 cenas-1.1.1/cenas.egg-info/PKG-INFO
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      413 2023-07-14 12:19:15.000000 cenas-1.1.1/cenas.egg-info/SOURCES.txt
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)        1 2023-07-14 12:19:15.000000 cenas-1.1.1/cenas.egg-info/dependency_links.txt
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       42 2023-07-14 12:19:15.000000 cenas-1.1.1/cenas.egg-info/entry_points.txt
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)        7 2023-07-14 12:19:15.000000 cenas-1.1.1/cenas.egg-info/requires.txt
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       13 2023-07-14 12:19:15.000000 cenas-1.1.1/cenas.egg-info/top_level.txt
+drwxrwxr-x   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-14 12:19:15.793610 cenas-1.1.1/cenas1/
+-rw-r--r--   0 cerqueiraf  (1000) cerqueiraf  (1000)        0 2023-07-13 08:44:19.000000 cenas-1.1.1/cenas1/__init__.py
+-rw-r--r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      389 2023-07-13 08:44:19.000000 cenas-1.1.1/cenas1/asgi.py
+-rw-r--r--   0 cerqueiraf  (1000) cerqueiraf  (1000)     3252 2023-07-14 11:44:23.000000 cenas-1.1.1/cenas1/settings.py
+-rw-r--r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      871 2023-07-13 10:50:44.000000 cenas-1.1.1/cenas1/urls.py
+-rw-r--r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      389 2023-07-13 08:44:19.000000 cenas-1.1.1/cenas1/wsgi.py
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)       38 2023-07-14 12:19:15.793610 cenas-1.1.1/setup.cfg
+-rw-rw-r--   0 cerqueiraf  (1000) cerqueiraf  (1000)      348 2023-07-14 12:11:38.000000 cenas-1.1.1/setup.py
```

### Comparing `cenas-1.1/webapp/settings.py` & `cenas-1.1.1/cenas1/settings.py`

 * *Files identical despite different names*

### Comparing `cenas-1.1/webapp/urls.py` & `cenas-1.1.1/cenas1/urls.py`

 * *Files identical despite different names*

