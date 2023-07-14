# Comparing `tmp/drupal-scout-1.0.0.tar.gz` & `tmp/drupal-scout-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drupal-scout-1.0.0.tar", last modified: Thu Jul 13 15:50:45 2023, max compression
+gzip compressed data, was "drupal-scout-1.0.1.tar", last modified: Fri Jul 14 11:07:17 2023, max compression
```

## Comparing `drupal-scout-1.0.0.tar` & `drupal-scout-1.0.1.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxrwxr-x   0 rtech     (1000) rtech     (1000)        0 2023-07-13 15:50:45.954119 drupal-scout-1.0.0/
--rw-rw-r--   0 rtech     (1000) rtech     (1000)     1073 2023-07-13 15:48:33.000000 drupal-scout-1.0.0/LICENSE.txt
--rw-rw-r--   0 rtech     (1000) rtech     (1000)      361 2023-07-13 15:50:45.954119 drupal-scout-1.0.0/PKG-INFO
--rw-rw-r--   0 rtech     (1000) rtech     (1000)     1775 2023-07-13 15:03:30.000000 drupal-scout-1.0.0/README.md
-drwxrwxr-x   0 rtech     (1000) rtech     (1000)        0 2023-07-13 15:50:45.954119 drupal-scout-1.0.0/bin/
--rwxrwxr-x   0 rtech     (1000) rtech     (1000)       91 2023-07-13 15:03:30.000000 drupal-scout-1.0.0/bin/drupal-scout
-drwxrwxr-x   0 rtech     (1000) rtech     (1000)        0 2023-07-13 15:50:45.954119 drupal-scout-1.0.0/drupal_scout/
--rw-rw-r--   0 rtech     (1000) rtech     (1000)       37 2023-07-13 15:03:30.000000 drupal-scout-1.0.0/drupal_scout/__init__.py
--rw-rw-r--   0 rtech     (1000) rtech     (1000)     9547 2023-07-13 15:03:30.000000 drupal-scout-1.0.0/drupal_scout/application.py
--rw-rw-r--   0 rtech     (1000) rtech     (1000)     1015 2023-07-13 15:03:30.000000 drupal-scout-1.0.0/drupal_scout/exceptions.py
-drwxrwxr-x   0 rtech     (1000) rtech     (1000)        0 2023-07-13 15:50:45.954119 drupal-scout-1.0.0/drupal_scout/formatters/
--rw-rw-r--   0 rtech     (1000) rtech     (1000)      231 2023-07-13 15:03:30.000000 drupal-scout-1.0.0/drupal_scout/formatters/formatter.py
--rw-rw-r--   0 rtech     (1000) rtech     (1000)      845 2023-07-13 15:03:30.000000 drupal-scout-1.0.0/drupal_scout/formatters/formatterfactory.py
--rw-rw-r--   0 rtech     (1000) rtech     (1000)     1038 2023-07-13 15:03:30.000000 drupal-scout-1.0.0/drupal_scout/formatters/jsonformatter.py
--rw-rw-r--   0 rtech     (1000) rtech     (1000)     3030 2023-07-13 15:03:30.000000 drupal-scout-1.0.0/drupal_scout/formatters/suggestformatter.py
--rw-rw-r--   0 rtech     (1000) rtech     (1000)     1495 2023-07-13 15:03:30.000000 drupal-scout-1.0.0/drupal_scout/formatters/tableformatter.py
--rw-rw-r--   0 rtech     (1000) rtech     (1000)      465 2023-07-13 15:03:30.000000 drupal-scout-1.0.0/drupal_scout/module.py
--rw-rw-r--   0 rtech     (1000) rtech     (1000)     5439 2023-07-13 15:03:30.000000 drupal-scout-1.0.0/drupal_scout/worker.py
--rw-rw-r--   0 rtech     (1000) rtech     (1000)     1344 2023-07-13 15:03:30.000000 drupal-scout-1.0.0/drupal_scout/workers_manager.py
-drwxrwxr-x   0 rtech     (1000) rtech     (1000)        0 2023-07-13 15:50:45.954119 drupal-scout-1.0.0/drupal_scout.egg-info/
--rw-rw-r--   0 rtech     (1000) rtech     (1000)      361 2023-07-13 15:50:45.000000 drupal-scout-1.0.0/drupal_scout.egg-info/PKG-INFO
--rw-rw-r--   0 rtech     (1000) rtech     (1000)      637 2023-07-13 15:50:45.000000 drupal-scout-1.0.0/drupal_scout.egg-info/SOURCES.txt
--rw-rw-r--   0 rtech     (1000) rtech     (1000)        1 2023-07-13 15:50:45.000000 drupal-scout-1.0.0/drupal_scout.egg-info/dependency_links.txt
--rw-rw-r--   0 rtech     (1000) rtech     (1000)        1 2023-06-10 20:04:39.000000 drupal-scout-1.0.0/drupal_scout.egg-info/not-zip-safe
--rw-rw-r--   0 rtech     (1000) rtech     (1000)       90 2023-07-13 15:50:45.000000 drupal-scout-1.0.0/drupal_scout.egg-info/requires.txt
--rw-rw-r--   0 rtech     (1000) rtech     (1000)       13 2023-07-13 15:50:45.000000 drupal-scout-1.0.0/drupal_scout.egg-info/top_level.txt
--rw-rw-r--   0 rtech     (1000) rtech     (1000)       79 2023-07-13 15:50:45.954119 drupal-scout-1.0.0/setup.cfg
--rw-rw-r--   0 rtech     (1000) rtech     (1000)      929 2023-07-13 15:48:33.000000 drupal-scout-1.0.0/setup.py
+drwxrwxr-x   0 rtech     (1000) rtech     (1000)        0 2023-07-14 11:07:17.417325 drupal-scout-1.0.1/
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)     1073 2023-07-13 15:48:33.000000 drupal-scout-1.0.1/LICENSE.txt
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)     3985 2023-07-14 11:07:17.417325 drupal-scout-1.0.1/PKG-INFO
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)     1775 2023-07-13 15:03:30.000000 drupal-scout-1.0.1/README.md
+drwxrwxr-x   0 rtech     (1000) rtech     (1000)        0 2023-07-14 11:07:17.413325 drupal-scout-1.0.1/bin/
+-rwxrwxr-x   0 rtech     (1000) rtech     (1000)       91 2023-07-13 15:03:30.000000 drupal-scout-1.0.1/bin/drupal-scout
+drwxrwxr-x   0 rtech     (1000) rtech     (1000)        0 2023-07-14 11:07:17.413325 drupal-scout-1.0.1/drupal_scout/
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)       37 2023-07-13 15:03:30.000000 drupal-scout-1.0.1/drupal_scout/__init__.py
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)     9547 2023-07-13 15:03:30.000000 drupal-scout-1.0.1/drupal_scout/application.py
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)     1015 2023-07-13 15:03:30.000000 drupal-scout-1.0.1/drupal_scout/exceptions.py
+drwxrwxr-x   0 rtech     (1000) rtech     (1000)        0 2023-07-14 11:07:17.417325 drupal-scout-1.0.1/drupal_scout/formatters/
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)      231 2023-07-13 15:03:30.000000 drupal-scout-1.0.1/drupal_scout/formatters/formatter.py
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)      845 2023-07-13 15:03:30.000000 drupal-scout-1.0.1/drupal_scout/formatters/formatterfactory.py
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)     1038 2023-07-13 15:03:30.000000 drupal-scout-1.0.1/drupal_scout/formatters/jsonformatter.py
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)     3030 2023-07-13 15:03:30.000000 drupal-scout-1.0.1/drupal_scout/formatters/suggestformatter.py
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)     1495 2023-07-13 15:03:30.000000 drupal-scout-1.0.1/drupal_scout/formatters/tableformatter.py
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)      465 2023-07-13 15:03:30.000000 drupal-scout-1.0.1/drupal_scout/module.py
+drwxrwxr-x   0 rtech     (1000) rtech     (1000)        0 2023-07-14 11:07:17.417325 drupal-scout-1.0.1/drupal_scout/tests/
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)        0 2023-07-13 15:03:30.000000 drupal-scout-1.0.1/drupal_scout/tests/__init__.py
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)     1886 2023-07-13 15:03:30.000000 drupal-scout-1.0.1/drupal_scout/tests/test_application.py
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)      553 2023-07-13 15:03:30.000000 drupal-scout-1.0.1/drupal_scout/tests/test_worker.py
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)     5439 2023-07-13 15:03:30.000000 drupal-scout-1.0.1/drupal_scout/worker.py
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)     1344 2023-07-13 15:03:30.000000 drupal-scout-1.0.1/drupal_scout/workers_manager.py
+drwxrwxr-x   0 rtech     (1000) rtech     (1000)        0 2023-07-14 11:07:17.413325 drupal-scout-1.0.1/drupal_scout.egg-info/
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)     3985 2023-07-14 11:07:17.000000 drupal-scout-1.0.1/drupal_scout.egg-info/PKG-INFO
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)      702 2023-07-14 11:07:17.000000 drupal-scout-1.0.1/drupal_scout.egg-info/SOURCES.txt
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)        1 2023-07-14 11:07:17.000000 drupal-scout-1.0.1/drupal_scout.egg-info/dependency_links.txt
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)      100 2023-07-14 11:07:17.000000 drupal-scout-1.0.1/drupal_scout.egg-info/requires.txt
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)       40 2023-07-14 11:07:17.000000 drupal-scout-1.0.1/drupal_scout.egg-info/top_level.txt
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)     1375 2023-07-14 11:06:48.000000 drupal-scout-1.0.1/pyproject.toml
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)       38 2023-07-14 11:07:17.417325 drupal-scout-1.0.1/setup.cfg
```

### Comparing `drupal-scout-1.0.0/LICENSE.txt` & `drupal-scout-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `drupal-scout-1.0.0/README.md` & `drupal-scout-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `drupal-scout-1.0.0/drupal_scout/application.py` & `drupal-scout-1.0.1/drupal_scout/application.py`

 * *Files identical despite different names*

### Comparing `drupal-scout-1.0.0/drupal_scout/exceptions.py` & `drupal-scout-1.0.1/drupal_scout/exceptions.py`

 * *Files identical despite different names*

### Comparing `drupal-scout-1.0.0/drupal_scout/formatters/formatterfactory.py` & `drupal-scout-1.0.1/drupal_scout/formatters/formatterfactory.py`

 * *Files identical despite different names*

### Comparing `drupal-scout-1.0.0/drupal_scout/formatters/jsonformatter.py` & `drupal-scout-1.0.1/drupal_scout/formatters/jsonformatter.py`

 * *Files identical despite different names*

### Comparing `drupal-scout-1.0.0/drupal_scout/formatters/suggestformatter.py` & `drupal-scout-1.0.1/drupal_scout/formatters/suggestformatter.py`

 * *Files identical despite different names*

### Comparing `drupal-scout-1.0.0/drupal_scout/formatters/tableformatter.py` & `drupal-scout-1.0.1/drupal_scout/formatters/tableformatter.py`

 * *Files identical despite different names*

### Comparing `drupal-scout-1.0.0/drupal_scout/worker.py` & `drupal-scout-1.0.1/drupal_scout/worker.py`

 * *Files identical despite different names*

### Comparing `drupal-scout-1.0.0/drupal_scout/workers_manager.py` & `drupal-scout-1.0.1/drupal_scout/workers_manager.py`

 * *Files identical despite different names*

