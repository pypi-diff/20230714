# Comparing `tmp/rayasdk-1.1.2.dev0.tar.gz` & `tmp/rayasdk-1.1.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rayasdk-1.1.2.dev0.tar", last modified: Tue Jul  4 20:59:55 2023, max compression
+gzip compressed data, was "rayasdk-1.1.3.dev0.tar", last modified: Fri Jul 14 19:06:42 2023, max compression
```

## Comparing `rayasdk-1.1.2.dev0.tar` & `rayasdk-1.1.3.dev0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:59:55.604219 rayasdk-1.1.2.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-07-04 20:59:55.604219 rayasdk-1.1.2.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:59:55.600219 rayasdk-1.1.2.dev0/rayasdk/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5706 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/connect.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:59:55.600219 rayasdk-1.1.2.dev0/rayasdk/container_handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/container_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/container_handlers/docker_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/executioner_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/initializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/killer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/sshKeyGen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:59:55.604219 rayasdk-1.1.2.dev0/rayasdk/template/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/template/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/template/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/template/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/template/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13479 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/rayasdk/vcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:59:55.600219 rayasdk-1.1.2.dev0/rayasdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-07-04 20:59:55.000000 rayasdk-1.1.2.dev0/rayasdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-04 20:59:55.000000 rayasdk-1.1.2.dev0/rayasdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 20:59:55.000000 rayasdk-1.1.2.dev0/rayasdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-04 20:59:55.000000 rayasdk-1.1.2.dev0/rayasdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-04 20:59:55.000000 rayasdk-1.1.2.dev0/rayasdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-04 20:59:55.000000 rayasdk-1.1.2.dev0/rayasdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-04 20:59:55.604219 rayasdk-1.1.2.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-04 20:59:44.000000 rayasdk-1.1.2.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:06:42.617452 rayasdk-1.1.3.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-07-14 19:06:42.617452 rayasdk-1.1.3.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-07-14 19:06:28.000000 rayasdk-1.1.3.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:06:42.613452 rayasdk-1.1.3.dev0/rayasdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-14 19:06:28.000000 rayasdk-1.1.3.dev0/rayasdk/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5706 2023-07-14 19:06:28.000000 rayasdk-1.1.3.dev0/rayasdk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-07-14 19:06:28.000000 rayasdk-1.1.3.dev0/rayasdk/connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-07-14 19:06:28.000000 rayasdk-1.1.3.dev0/rayasdk/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:06:42.617452 rayasdk-1.1.3.dev0/rayasdk/container_handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:06:28.000000 rayasdk-1.1.3.dev0/rayasdk/container_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-07-14 19:06:28.000000 rayasdk-1.1.3.dev0/rayasdk/container_handlers/docker_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-14 19:06:28.000000 rayasdk-1.1.3.dev0/rayasdk/executioner_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-14 19:06:28.000000 rayasdk-1.1.3.dev0/rayasdk/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-14 19:06:28.000000 rayasdk-1.1.3.dev0/rayasdk/killer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-07-14 19:06:28.000000 rayasdk-1.1.3.dev0/rayasdk/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-14 19:06:28.000000 rayasdk-1.1.3.dev0/rayasdk/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-07-14 19:06:28.000000 rayasdk-1.1.3.dev0/rayasdk/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-07-14 19:06:28.000000 rayasdk-1.1.3.dev0/rayasdk/scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-07-14 19:06:28.000000 rayasdk-1.1.3.dev0/rayasdk/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-07-14 19:06:28.000000 rayasdk-1.1.3.dev0/rayasdk/sshKeyGen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:06:42.617452 rayasdk-1.1.3.dev0/rayasdk/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-14 19:06:28.000000 rayasdk-1.1.3.dev0/rayasdk/template/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-14 19:06:28.000000 rayasdk-1.1.3.dev0/rayasdk/template/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-14 19:06:28.000000 rayasdk-1.1.3.dev0/rayasdk/template/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-14 19:06:28.000000 rayasdk-1.1.3.dev0/rayasdk/template/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-14 19:06:28.000000 rayasdk-1.1.3.dev0/rayasdk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13479 2023-07-14 19:06:28.000000 rayasdk-1.1.3.dev0/rayasdk/vcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:06:42.613452 rayasdk-1.1.3.dev0/rayasdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-07-14 19:06:42.000000 rayasdk-1.1.3.dev0/rayasdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-14 19:06:42.000000 rayasdk-1.1.3.dev0/rayasdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 19:06:42.000000 rayasdk-1.1.3.dev0/rayasdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-14 19:06:42.000000 rayasdk-1.1.3.dev0/rayasdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-14 19:06:42.000000 rayasdk-1.1.3.dev0/rayasdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 19:06:42.000000 rayasdk-1.1.3.dev0/rayasdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-14 19:06:42.617452 rayasdk-1.1.3.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-14 19:06:28.000000 rayasdk-1.1.3.dev0/setup.py
```

### Comparing `rayasdk-1.1.2.dev0/PKG-INFO` & `rayasdk-1.1.3.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rayasdk
-Version: 1.1.2.dev0
+Version: 1.1.3.dev0
 Summary: Raya SDK - Unlimited Robotics Software Development Kit
 Home-page: 
 Download-URL: 
 Author: Unlimited Robotics
 Author-email: camilo@unlimited-robotics.com
 License: MIT
 Keywords: robotics,unlimited-robotics,gary
```

### Comparing `rayasdk-1.1.2.dev0/README.md` & `rayasdk-1.1.3.dev0/README.md`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.2.dev0/rayasdk/__init__.py` & `rayasdk-1.1.3.dev0/rayasdk/__init__.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.2.dev0/rayasdk/__main__.py` & `rayasdk-1.1.3.dev0/rayasdk/__main__.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.2.dev0/rayasdk/connect.py` & `rayasdk-1.1.3.dev0/rayasdk/connect.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.2.dev0/rayasdk/constants.py` & `rayasdk-1.1.3.dev0/rayasdk/constants.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.2.dev0/rayasdk/container_handlers/docker_handler.py` & `rayasdk-1.1.3.dev0/rayasdk/container_handlers/docker_handler.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.2.dev0/rayasdk/executioner_command.py` & `rayasdk-1.1.3.dev0/rayasdk/executioner_command.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.2.dev0/rayasdk/initializer.py` & `rayasdk-1.1.3.dev0/rayasdk/initializer.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.2.dev0/rayasdk/killer.py` & `rayasdk-1.1.3.dev0/rayasdk/killer.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.2.dev0/rayasdk/logger.py` & `rayasdk-1.1.3.dev0/rayasdk/logger.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.2.dev0/rayasdk/messages.py` & `rayasdk-1.1.3.dev0/rayasdk/messages.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.2.dev0/rayasdk/runner.py` & `rayasdk-1.1.3.dev0/rayasdk/runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,16 +47,15 @@
 
         # Open exec_settings file
         try:
             with open(constants.EXECSETTINGS_PATH, 'r', encoding='utf-8') as f:
                 exec_settings = json.load(f)
             app_id = exec_settings[constants.JSON_EXECINFO_APPID]
         except OSError:
-            log_error((f'Could not open "{constants.EXECSETTINGS_FILE}" file, '
-                       'project not initialized or file not valid.'))
+            log_error('The folder is not a Ra-Ya app')
             return False
         except KeyError as key:
             log_error(f'{key} key not found on {constants.EXECSETTINGS_FILE}.')
             return False
         
         # Check if the parent has the same name that the app id
         if not validate_app_id_and_folder_name(app_id):
```

### Comparing `rayasdk-1.1.2.dev0/rayasdk/scanner.py` & `rayasdk-1.1.3.dev0/rayasdk/scanner.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.2.dev0/rayasdk/simulator.py` & `rayasdk-1.1.3.dev0/rayasdk/simulator.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.2.dev0/rayasdk/sshKeyGen.py` & `rayasdk-1.1.3.dev0/rayasdk/sshKeyGen.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.2.dev0/rayasdk/template/app.py` & `rayasdk-1.1.3.dev0/rayasdk/template/app.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.2.dev0/rayasdk/utils.py` & `rayasdk-1.1.3.dev0/rayasdk/utils.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.2.dev0/rayasdk/vcs.py` & `rayasdk-1.1.3.dev0/rayasdk/vcs.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.2.dev0/rayasdk.egg-info/PKG-INFO` & `rayasdk-1.1.3.dev0/rayasdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rayasdk
-Version: 1.1.2.dev0
+Version: 1.1.3.dev0
 Summary: Raya SDK - Unlimited Robotics Software Development Kit
 Home-page: 
 Download-URL: 
 Author: Unlimited Robotics
 Author-email: camilo@unlimited-robotics.com
 License: MIT
 Keywords: robotics,unlimited-robotics,gary
```

### Comparing `rayasdk-1.1.2.dev0/rayasdk.egg-info/SOURCES.txt` & `rayasdk-1.1.3.dev0/rayasdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.2.dev0/setup.py` & `rayasdk-1.1.3.dev0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.1.2.dev'
+VERSION = '1.1.3.dev'
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='rayasdk',
     packages=find_packages(),
```

