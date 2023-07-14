# Comparing `tmp/drupal-scout-1.0.1.tar.gz` & `tmp/drupal-scout-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drupal-scout-1.0.1.tar", last modified: Fri Jul 14 11:07:17 2023, max compression
+gzip compressed data, was "drupal-scout-1.0.2.tar", last modified: Fri Jul 14 11:37:05 2023, max compression
```

## Comparing `drupal-scout-1.0.1.tar` & `drupal-scout-1.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 rtech     (1000) rtech     (1000)        0 2023-07-14 11:07:17.417325 drupal-scout-1.0.1/
--rw-rw-r--   0 rtech     (1000) rtech     (1000)     1073 2023-07-13 15:48:33.000000 drupal-scout-1.0.1/LICENSE.txt
--rw-rw-r--   0 rtech     (1000) rtech     (1000)     3985 2023-07-14 11:07:17.417325 drupal-scout-1.0.1/PKG-INFO
--rw-rw-r--   0 rtech     (1000) rtech     (1000)     1775 2023-07-13 15:03:30.000000 drupal-scout-1.0.1/README.md
-drwxrwxr-x   0 rtech     (1000) rtech     (1000)        0 2023-07-14 11:07:17.413325 drupal-scout-1.0.1/bin/
--rwxrwxr-x   0 rtech     (1000) rtech     (1000)       91 2023-07-13 15:03:30.000000 drupal-scout-1.0.1/bin/drupal-scout
-drwxrwxr-x   0 rtech     (1000) rtech     (1000)        0 2023-07-14 11:07:17.413325 drupal-scout-1.0.1/drupal_scout/
--rw-rw-r--   0 rtech     (1000) rtech     (1000)       37 2023-07-13 15:03:30.000000 drupal-scout-1.0.1/drupal_scout/__init__.py
--rw-rw-r--   0 rtech     (1000) rtech     (1000)     9547 2023-07-13 15:03:30.000000 drupal-scout-1.0.1/drupal_scout/application.py
--rw-rw-r--   0 rtech     (1000) rtech     (1000)     1015 2023-07-13 15:03:30.000000 drupal-scout-1.0.1/drupal_scout/exceptions.py
-drwxrwxr-x   0 rtech     (1000) rtech     (1000)        0 2023-07-14 11:07:17.417325 drupal-scout-1.0.1/drupal_scout/formatters/
--rw-rw-r--   0 rtech     (1000) rtech     (1000)      231 2023-07-13 15:03:30.000000 drupal-scout-1.0.1/drupal_scout/formatters/formatter.py
--rw-rw-r--   0 rtech     (1000) rtech     (1000)      845 2023-07-13 15:03:30.000000 drupal-scout-1.0.1/drupal_scout/formatters/formatterfactory.py
--rw-rw-r--   0 rtech     (1000) rtech     (1000)     1038 2023-07-13 15:03:30.000000 drupal-scout-1.0.1/drupal_scout/formatters/jsonformatter.py
--rw-rw-r--   0 rtech     (1000) rtech     (1000)     3030 2023-07-13 15:03:30.000000 drupal-scout-1.0.1/drupal_scout/formatters/suggestformatter.py
--rw-rw-r--   0 rtech     (1000) rtech     (1000)     1495 2023-07-13 15:03:30.000000 drupal-scout-1.0.1/drupal_scout/formatters/tableformatter.py
--rw-rw-r--   0 rtech     (1000) rtech     (1000)      465 2023-07-13 15:03:30.000000 drupal-scout-1.0.1/drupal_scout/module.py
-drwxrwxr-x   0 rtech     (1000) rtech     (1000)        0 2023-07-14 11:07:17.417325 drupal-scout-1.0.1/drupal_scout/tests/
--rw-rw-r--   0 rtech     (1000) rtech     (1000)        0 2023-07-13 15:03:30.000000 drupal-scout-1.0.1/drupal_scout/tests/__init__.py
--rw-rw-r--   0 rtech     (1000) rtech     (1000)     1886 2023-07-13 15:03:30.000000 drupal-scout-1.0.1/drupal_scout/tests/test_application.py
--rw-rw-r--   0 rtech     (1000) rtech     (1000)      553 2023-07-13 15:03:30.000000 drupal-scout-1.0.1/drupal_scout/tests/test_worker.py
--rw-rw-r--   0 rtech     (1000) rtech     (1000)     5439 2023-07-13 15:03:30.000000 drupal-scout-1.0.1/drupal_scout/worker.py
--rw-rw-r--   0 rtech     (1000) rtech     (1000)     1344 2023-07-13 15:03:30.000000 drupal-scout-1.0.1/drupal_scout/workers_manager.py
-drwxrwxr-x   0 rtech     (1000) rtech     (1000)        0 2023-07-14 11:07:17.413325 drupal-scout-1.0.1/drupal_scout.egg-info/
--rw-rw-r--   0 rtech     (1000) rtech     (1000)     3985 2023-07-14 11:07:17.000000 drupal-scout-1.0.1/drupal_scout.egg-info/PKG-INFO
--rw-rw-r--   0 rtech     (1000) rtech     (1000)      702 2023-07-14 11:07:17.000000 drupal-scout-1.0.1/drupal_scout.egg-info/SOURCES.txt
--rw-rw-r--   0 rtech     (1000) rtech     (1000)        1 2023-07-14 11:07:17.000000 drupal-scout-1.0.1/drupal_scout.egg-info/dependency_links.txt
--rw-rw-r--   0 rtech     (1000) rtech     (1000)      100 2023-07-14 11:07:17.000000 drupal-scout-1.0.1/drupal_scout.egg-info/requires.txt
--rw-rw-r--   0 rtech     (1000) rtech     (1000)       40 2023-07-14 11:07:17.000000 drupal-scout-1.0.1/drupal_scout.egg-info/top_level.txt
--rw-rw-r--   0 rtech     (1000) rtech     (1000)     1375 2023-07-14 11:06:48.000000 drupal-scout-1.0.1/pyproject.toml
--rw-rw-r--   0 rtech     (1000) rtech     (1000)       38 2023-07-14 11:07:17.417325 drupal-scout-1.0.1/setup.cfg
+drwxrwxr-x   0 rtech     (1000) rtech     (1000)        0 2023-07-14 11:37:05.193378 drupal-scout-1.0.2/
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)     1073 2023-07-13 15:48:33.000000 drupal-scout-1.0.2/LICENSE.txt
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)     4045 2023-07-14 11:37:05.193378 drupal-scout-1.0.2/PKG-INFO
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)     1835 2023-07-14 11:36:56.000000 drupal-scout-1.0.2/README.md
+drwxrwxr-x   0 rtech     (1000) rtech     (1000)        0 2023-07-14 11:37:05.189378 drupal-scout-1.0.2/bin/
+-rwxrwxr-x   0 rtech     (1000) rtech     (1000)       91 2023-07-13 15:03:30.000000 drupal-scout-1.0.2/bin/drupal-scout
+drwxrwxr-x   0 rtech     (1000) rtech     (1000)        0 2023-07-14 11:37:05.189378 drupal-scout-1.0.2/drupal_scout/
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)       37 2023-07-13 15:03:30.000000 drupal-scout-1.0.2/drupal_scout/__init__.py
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)     9547 2023-07-13 15:03:30.000000 drupal-scout-1.0.2/drupal_scout/application.py
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)     1015 2023-07-13 15:03:30.000000 drupal-scout-1.0.2/drupal_scout/exceptions.py
+drwxrwxr-x   0 rtech     (1000) rtech     (1000)        0 2023-07-14 11:37:05.193378 drupal-scout-1.0.2/drupal_scout/formatters/
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)      231 2023-07-13 15:03:30.000000 drupal-scout-1.0.2/drupal_scout/formatters/formatter.py
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)      845 2023-07-13 15:03:30.000000 drupal-scout-1.0.2/drupal_scout/formatters/formatterfactory.py
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)     1038 2023-07-13 15:03:30.000000 drupal-scout-1.0.2/drupal_scout/formatters/jsonformatter.py
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)     3030 2023-07-13 15:03:30.000000 drupal-scout-1.0.2/drupal_scout/formatters/suggestformatter.py
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)     1495 2023-07-13 15:03:30.000000 drupal-scout-1.0.2/drupal_scout/formatters/tableformatter.py
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)      465 2023-07-13 15:03:30.000000 drupal-scout-1.0.2/drupal_scout/module.py
+drwxrwxr-x   0 rtech     (1000) rtech     (1000)        0 2023-07-14 11:37:05.193378 drupal-scout-1.0.2/drupal_scout/tests/
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)        0 2023-07-13 15:03:30.000000 drupal-scout-1.0.2/drupal_scout/tests/__init__.py
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)     1886 2023-07-13 15:03:30.000000 drupal-scout-1.0.2/drupal_scout/tests/test_application.py
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)      553 2023-07-13 15:03:30.000000 drupal-scout-1.0.2/drupal_scout/tests/test_worker.py
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)     5439 2023-07-13 15:03:30.000000 drupal-scout-1.0.2/drupal_scout/worker.py
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)     1344 2023-07-13 15:03:30.000000 drupal-scout-1.0.2/drupal_scout/workers_manager.py
+drwxrwxr-x   0 rtech     (1000) rtech     (1000)        0 2023-07-14 11:37:05.193378 drupal-scout-1.0.2/drupal_scout.egg-info/
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)     4045 2023-07-14 11:37:05.000000 drupal-scout-1.0.2/drupal_scout.egg-info/PKG-INFO
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)      702 2023-07-14 11:37:05.000000 drupal-scout-1.0.2/drupal_scout.egg-info/SOURCES.txt
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)        1 2023-07-14 11:37:05.000000 drupal-scout-1.0.2/drupal_scout.egg-info/dependency_links.txt
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)      100 2023-07-14 11:37:05.000000 drupal-scout-1.0.2/drupal_scout.egg-info/requires.txt
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)       40 2023-07-14 11:37:05.000000 drupal-scout-1.0.2/drupal_scout.egg-info/top_level.txt
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)     1375 2023-07-14 11:36:56.000000 drupal-scout-1.0.2/pyproject.toml
+-rw-rw-r--   0 rtech     (1000) rtech     (1000)       38 2023-07-14 11:37:05.193378 drupal-scout-1.0.2/setup.cfg
```

### Comparing `drupal-scout-1.0.1/LICENSE.txt` & `drupal-scout-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `drupal-scout-1.0.1/PKG-INFO` & `drupal-scout-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drupal-scout
-Version: 1.0.1
+Version: 1.0.2
 Summary: Scout out for transitive versions of Drupal modules for the upgrade of the core.
 Author-email: "Andrew [R-Tech] Tsyhaniuk" <in0mad91@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Andrew Tsyhaniuk
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -54,15 +54,15 @@
 
 ## Features
 
 - Use multithreading to speed up the process of searching for the Drupal module entries with transitive core version requirements.
 - Choose between three output formats: table, json, and suggest.  
     - `table` format will output the data in the table format.  
     Example:
-    ![Table format example](screenshots/format_table_example.png)
+    ![Table format example](https://raw.githubusercontent.com/rtech91/drupal-scout/main/screenshots/format_table_example.png)
     - `json` format will output the raw data in the json format.  
     - `suggest` format will output the suggested composer.json file with the updated module version requirements.  
     It will also dump the suggested composer.json file to the specified path if the `--save-dump` argument is used.
 
 ## Limitations
 
 - The application will only work with Composer-based (Composer v2) Drupal 8+ projects.
```

### Comparing `drupal-scout-1.0.1/README.md` & `drupal-scout-1.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 ## Features
 
 - Use multithreading to speed up the process of searching for the Drupal module entries with transitive core version requirements.
 - Choose between three output formats: table, json, and suggest.  
     - `table` format will output the data in the table format.  
     Example:
-    ![Table format example](screenshots/format_table_example.png)
+    ![Table format example](https://raw.githubusercontent.com/rtech91/drupal-scout/main/screenshots/format_table_example.png)
     - `json` format will output the raw data in the json format.  
     - `suggest` format will output the suggested composer.json file with the updated module version requirements.  
     It will also dump the suggested composer.json file to the specified path if the `--save-dump` argument is used.
 
 ## Limitations
 
 - The application will only work with Composer-based (Composer v2) Drupal 8+ projects.
```

### Comparing `drupal-scout-1.0.1/drupal_scout/application.py` & `drupal-scout-1.0.2/drupal_scout/application.py`

 * *Files identical despite different names*

### Comparing `drupal-scout-1.0.1/drupal_scout/exceptions.py` & `drupal-scout-1.0.2/drupal_scout/exceptions.py`

 * *Files identical despite different names*

### Comparing `drupal-scout-1.0.1/drupal_scout/formatters/formatterfactory.py` & `drupal-scout-1.0.2/drupal_scout/formatters/formatterfactory.py`

 * *Files identical despite different names*

### Comparing `drupal-scout-1.0.1/drupal_scout/formatters/jsonformatter.py` & `drupal-scout-1.0.2/drupal_scout/formatters/jsonformatter.py`

 * *Files identical despite different names*

### Comparing `drupal-scout-1.0.1/drupal_scout/formatters/suggestformatter.py` & `drupal-scout-1.0.2/drupal_scout/formatters/suggestformatter.py`

 * *Files identical despite different names*

### Comparing `drupal-scout-1.0.1/drupal_scout/formatters/tableformatter.py` & `drupal-scout-1.0.2/drupal_scout/formatters/tableformatter.py`

 * *Files identical despite different names*

### Comparing `drupal-scout-1.0.1/drupal_scout/tests/test_application.py` & `drupal-scout-1.0.2/drupal_scout/tests/test_application.py`

 * *Files identical despite different names*

### Comparing `drupal-scout-1.0.1/drupal_scout/tests/test_worker.py` & `drupal-scout-1.0.2/drupal_scout/tests/test_worker.py`

 * *Files identical despite different names*

### Comparing `drupal-scout-1.0.1/drupal_scout/worker.py` & `drupal-scout-1.0.2/drupal_scout/worker.py`

 * *Files identical despite different names*

### Comparing `drupal-scout-1.0.1/drupal_scout/workers_manager.py` & `drupal-scout-1.0.2/drupal_scout/workers_manager.py`

 * *Files identical despite different names*

### Comparing `drupal-scout-1.0.1/drupal_scout.egg-info/PKG-INFO` & `drupal-scout-1.0.2/drupal_scout.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drupal-scout
-Version: 1.0.1
+Version: 1.0.2
 Summary: Scout out for transitive versions of Drupal modules for the upgrade of the core.
 Author-email: "Andrew [R-Tech] Tsyhaniuk" <in0mad91@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Andrew Tsyhaniuk
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -54,15 +54,15 @@
 
 ## Features
 
 - Use multithreading to speed up the process of searching for the Drupal module entries with transitive core version requirements.
 - Choose between three output formats: table, json, and suggest.  
     - `table` format will output the data in the table format.  
     Example:
-    ![Table format example](screenshots/format_table_example.png)
+    ![Table format example](https://raw.githubusercontent.com/rtech91/drupal-scout/main/screenshots/format_table_example.png)
     - `json` format will output the raw data in the json format.  
     - `suggest` format will output the suggested composer.json file with the updated module version requirements.  
     It will also dump the suggested composer.json file to the specified path if the `--save-dump` argument is used.
 
 ## Limitations
 
 - The application will only work with Composer-based (Composer v2) Drupal 8+ projects.
```

### Comparing `drupal-scout-1.0.1/drupal_scout.egg-info/SOURCES.txt` & `drupal-scout-1.0.2/drupal_scout.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drupal-scout-1.0.1/pyproject.toml` & `drupal-scout-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "drupal-scout"
-version = "1.0.1"
+version = "1.0.2"
 description = "Scout out for transitive versions of Drupal modules for the upgrade of the core."
 readme = "README.md"
 license = { file="LICENSE.txt", name="MIT" }
 keywords = ["drupal", "scout", "upgrade", "core", "transitive", "dependencies"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
```

