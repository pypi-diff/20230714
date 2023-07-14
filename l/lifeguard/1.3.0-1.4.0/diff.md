# Comparing `tmp/lifeguard-1.3.0.tar.gz` & `tmp/lifeguard-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeguard-1.3.0.tar", last modified: Fri Jul  7 16:48:55 2023, max compression
+gzip compressed data, was "lifeguard-1.4.0.tar", last modified: Fri Jul 14 19:25:48 2023, max compression
```

## Comparing `lifeguard-1.3.0.tar` & `lifeguard-1.4.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:55.952991 lifeguard-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-07-07 16:48:55.952991 lifeguard-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-07-07 16:48:43.000000 lifeguard-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:55.948991 lifeguard-1.3.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2929 2023-07-07 16:48:43.000000 lifeguard-1.3.0/bin/lifeguard
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:55.948991 lifeguard-1.3.0/lifeguard/
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:55.948991 lifeguard-1.3.0/lifeguard/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/actions/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/actions/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/actions/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:55.948991 lifeguard-1.3.0/lifeguard/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/controllers/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/statuses.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/validations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:55.948991 lifeguard-1.3.0/lifeguard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-07-07 16:48:55.000000 lifeguard-1.3.0/lifeguard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-07 16:48:55.000000 lifeguard-1.3.0/lifeguard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 16:48:55.000000 lifeguard-1.3.0/lifeguard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-07 16:48:55.000000 lifeguard-1.3.0/lifeguard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-07 16:48:55.000000 lifeguard-1.3.0/lifeguard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-07 16:48:55.952991 lifeguard-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-07 16:48:43.000000 lifeguard-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:55.952991 lifeguard-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:55.952991 lifeguard-1.3.0/tests/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/actions/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/actions/test_email.py
--rw-r--r--   0 runner    (1001) docker     (123)    15144 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/actions/test_notification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:55.952991 lifeguard-1.3.0/tests/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/controllers/test_assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:55.952991 lifeguard-1.3.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/fixtures/fixtures_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/fixtures/mock_lifeguard_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/test_controllers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/test_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/test_lifeguard_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/test_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/test_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/test_validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:25:48.496218 lifeguard-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-14 19:25:48.496218 lifeguard-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-07-14 19:25:39.000000 lifeguard-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:25:48.492218 lifeguard-1.4.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2929 2023-07-14 19:25:39.000000 lifeguard-1.4.0/bin/lifeguard
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:25:48.492218 lifeguard-1.4.0/lifeguard/
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-14 19:25:39.000000 lifeguard-1.4.0/lifeguard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:25:48.492218 lifeguard-1.4.0/lifeguard/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:25:39.000000 lifeguard-1.4.0/lifeguard/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-14 19:25:39.000000 lifeguard-1.4.0/lifeguard/actions/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-14 19:25:39.000000 lifeguard-1.4.0/lifeguard/actions/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-07-14 19:25:39.000000 lifeguard-1.4.0/lifeguard/actions/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-14 19:25:39.000000 lifeguard-1.4.0/lifeguard/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-14 19:25:39.000000 lifeguard-1.4.0/lifeguard/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-14 19:25:39.000000 lifeguard-1.4.0/lifeguard/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:25:48.492218 lifeguard-1.4.0/lifeguard/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-14 19:25:39.000000 lifeguard-1.4.0/lifeguard/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-14 19:25:39.000000 lifeguard-1.4.0/lifeguard/controllers/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-14 19:25:39.000000 lifeguard-1.4.0/lifeguard/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-14 19:25:39.000000 lifeguard-1.4.0/lifeguard/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-07-14 19:25:39.000000 lifeguard-1.4.0/lifeguard/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-14 19:25:39.000000 lifeguard-1.4.0/lifeguard/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-07-14 19:25:39.000000 lifeguard-1.4.0/lifeguard/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-14 19:25:39.000000 lifeguard-1.4.0/lifeguard/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-07-14 19:25:39.000000 lifeguard-1.4.0/lifeguard/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-14 19:25:39.000000 lifeguard-1.4.0/lifeguard/statuses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-14 19:25:39.000000 lifeguard-1.4.0/lifeguard/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-07-14 19:25:39.000000 lifeguard-1.4.0/lifeguard/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:25:48.492218 lifeguard-1.4.0/lifeguard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-14 19:25:48.000000 lifeguard-1.4.0/lifeguard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-14 19:25:48.000000 lifeguard-1.4.0/lifeguard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 19:25:48.000000 lifeguard-1.4.0/lifeguard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-14 19:25:48.000000 lifeguard-1.4.0/lifeguard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-14 19:25:48.000000 lifeguard-1.4.0/lifeguard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-14 19:25:48.496218 lifeguard-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-14 19:25:39.000000 lifeguard-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:25:48.492218 lifeguard-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:25:39.000000 lifeguard-1.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:25:48.492218 lifeguard-1.4.0/tests/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:25:39.000000 lifeguard-1.4.0/tests/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-14 19:25:39.000000 lifeguard-1.4.0/tests/actions/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-07-14 19:25:39.000000 lifeguard-1.4.0/tests/actions/test_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15144 2023-07-14 19:25:39.000000 lifeguard-1.4.0/tests/actions/test_notification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:25:48.496218 lifeguard-1.4.0/tests/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:25:39.000000 lifeguard-1.4.0/tests/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-07-14 19:25:39.000000 lifeguard-1.4.0/tests/controllers/test_assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:25:48.496218 lifeguard-1.4.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:25:39.000000 lifeguard-1.4.0/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-14 19:25:39.000000 lifeguard-1.4.0/tests/fixtures/fixtures_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-14 19:25:39.000000 lifeguard-1.4.0/tests/fixtures/mock_lifeguard_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-14 19:25:39.000000 lifeguard-1.4.0/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-14 19:25:39.000000 lifeguard-1.4.0/tests/test_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-07-14 19:25:39.000000 lifeguard-1.4.0/tests/test_controllers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-14 19:25:39.000000 lifeguard-1.4.0/tests/test_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-14 19:25:39.000000 lifeguard-1.4.0/tests/test_lifeguard_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-14 19:25:39.000000 lifeguard-1.4.0/tests/test_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-07-14 19:25:39.000000 lifeguard-1.4.0/tests/test_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-07-14 19:25:39.000000 lifeguard-1.4.0/tests/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-07-14 19:25:39.000000 lifeguard-1.4.0/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-07-14 19:25:39.000000 lifeguard-1.4.0/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-07-14 19:25:39.000000 lifeguard-1.4.0/tests/test_validations.py
```

### Comparing `lifeguard-1.3.0/PKG-INFO` & `lifeguard-1.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifeguard
-Version: 1.3.0
+Version: 1.4.0
 Summary: Application to monitor your systems and give you the security to sleep peacefully at night
 Home-page: https://github.com/LifeguardSystem/lifeguard
 Author: Diego Rubin
 Author-email: contact@diegorubin.dev
 License: GPL2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -75,14 +75,35 @@
 
     return ValidationResponse(
         status,
         {status: result.status_code},
     )
 ```
 
+Starting with version 1.3.0, it is possible to create validations using yaml files. The file should ends with `_validation.yaml`. See the example:
+
+```yaml
+validations:
+  - validation_name: "validation_name"
+    description: "description of validation"
+    actions:
+      - lifeguard.actions.database.save_result_into_database
+    schedule:
+      every:
+        minutes: 1
+    settings:
+      notification:
+        update_thread_interval: 3600
+    execute:
+      command: path.to.module.function
+      args:
+        - "arg1"
+        - "arg2"
+```
+
 ### Validation Actions
 
 Action is a simple python function with only 2 arguments: a validation response and a dict called settings. These settings are the parameter called settings in validation.
 
 ```python
 def custom_action(validation_response, settings):
     pass
```

### Comparing `lifeguard-1.3.0/README.md` & `lifeguard-1.4.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -59,14 +59,35 @@
 
     return ValidationResponse(
         status,
         {status: result.status_code},
     )
 ```
 
+Starting with version 1.3.0, it is possible to create validations using yaml files. The file should ends with `_validation.yaml`. See the example:
+
+```yaml
+validations:
+  - validation_name: "validation_name"
+    description: "description of validation"
+    actions:
+      - lifeguard.actions.database.save_result_into_database
+    schedule:
+      every:
+        minutes: 1
+    settings:
+      notification:
+        update_thread_interval: 3600
+    execute:
+      command: path.to.module.function
+      args:
+        - "arg1"
+        - "arg2"
+```
+
 ### Validation Actions
 
 Action is a simple python function with only 2 arguments: a validation response and a dict called settings. These settings are the parameter called settings in validation.
 
 ```python
 def custom_action(validation_response, settings):
     pass
```

### Comparing `lifeguard-1.3.0/bin/lifeguard` & `lifeguard-1.4.0/bin/lifeguard`

 * *Files identical despite different names*

### Comparing `lifeguard-1.3.0/lifeguard/__init__.py` & `lifeguard-1.4.0/lifeguard/__init__.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.3.0/lifeguard/actions/email.py` & `lifeguard-1.4.0/lifeguard/actions/email.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.3.0/lifeguard/actions/notifications.py` & `lifeguard-1.4.0/lifeguard/actions/notifications.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.3.0/lifeguard/auth.py` & `lifeguard-1.4.0/lifeguard/auth.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.3.0/lifeguard/context.py` & `lifeguard-1.4.0/lifeguard/context.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.3.0/lifeguard/controllers/__init__.py` & `lifeguard-1.4.0/lifeguard/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.3.0/lifeguard/controllers/assets.py` & `lifeguard-1.4.0/lifeguard/controllers/assets.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.3.0/lifeguard/http_client.py` & `lifeguard-1.4.0/lifeguard/http_client.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.3.0/lifeguard/logger.py` & `lifeguard-1.4.0/lifeguard/logger.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.3.0/lifeguard/notifications.py` & `lifeguard-1.4.0/lifeguard/notifications.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.3.0/lifeguard/repositories.py` & `lifeguard-1.4.0/lifeguard/repositories.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.3.0/lifeguard/server.py` & `lifeguard-1.4.0/lifeguard/server.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.3.0/lifeguard/settings.py` & `lifeguard-1.4.0/lifeguard/settings.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.3.0/lifeguard/validations.py` & `lifeguard-1.4.0/lifeguard/validations.py`

 * *Files 5% similar despite different names*

```diff
@@ -171,14 +171,21 @@
         """
         Default implementation for validation response encoder
         """
 
         return validation_response.get_attributes()
 
 
+def clear_validations():
+    """
+    Clear validations
+    """
+    VALIDATIONS.clear()
+
+
 def load_validations():
     """
     Load validations from application path
     """
     for root, _dirs, files in os.walk(os.path.join(LIFEGUARD_DIRECTORY, "validations")):
         relative_path = os.path.relpath(root, os.path.join(LIFEGUARD_DIRECTORY))
         for validation_file in files:
```

### Comparing `lifeguard-1.3.0/lifeguard.egg-info/PKG-INFO` & `lifeguard-1.4.0/lifeguard.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifeguard
-Version: 1.3.0
+Version: 1.4.0
 Summary: Application to monitor your systems and give you the security to sleep peacefully at night
 Home-page: https://github.com/LifeguardSystem/lifeguard
 Author: Diego Rubin
 Author-email: contact@diegorubin.dev
 License: GPL2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -75,14 +75,35 @@
 
     return ValidationResponse(
         status,
         {status: result.status_code},
     )
 ```
 
+Starting with version 1.3.0, it is possible to create validations using yaml files. The file should ends with `_validation.yaml`. See the example:
+
+```yaml
+validations:
+  - validation_name: "validation_name"
+    description: "description of validation"
+    actions:
+      - lifeguard.actions.database.save_result_into_database
+    schedule:
+      every:
+        minutes: 1
+    settings:
+      notification:
+        update_thread_interval: 3600
+    execute:
+      command: path.to.module.function
+      args:
+        - "arg1"
+        - "arg2"
+```
+
 ### Validation Actions
 
 Action is a simple python function with only 2 arguments: a validation response and a dict called settings. These settings are the parameter called settings in validation.
 
 ```python
 def custom_action(validation_response, settings):
     pass
```

### Comparing `lifeguard-1.3.0/lifeguard.egg-info/SOURCES.txt` & `lifeguard-1.4.0/lifeguard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lifeguard-1.3.0/setup.py` & `lifeguard-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="lifeguard",
-    version="1.3.0",
+    version="1.4.0",
     url="https://github.com/LifeguardSystem/lifeguard",
     author="Diego Rubin",
     author_email="contact@diegorubin.dev",
     license="GPL2",
     scripts=["bin/lifeguard"],
     include_package_data=True,
     description="Application to monitor your systems and give you the security to sleep peacefully at night",
```

### Comparing `lifeguard-1.3.0/tests/actions/test_database.py` & `lifeguard-1.4.0/tests/actions/test_database.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.3.0/tests/actions/test_email.py` & `lifeguard-1.4.0/tests/actions/test_email.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.3.0/tests/actions/test_notification.py` & `lifeguard-1.4.0/tests/actions/test_notification.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.3.0/tests/controllers/test_assets.py` & `lifeguard-1.4.0/tests/controllers/test_assets.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.3.0/tests/test_auth.py` & `lifeguard-1.4.0/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.3.0/tests/test_bootstrap.py` & `lifeguard-1.4.0/tests/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.3.0/tests/test_controllers.py` & `lifeguard-1.4.0/tests/test_controllers.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.3.0/tests/test_http_client.py` & `lifeguard-1.4.0/tests/test_http_client.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.3.0/tests/test_lifeguard_core.py` & `lifeguard-1.4.0/tests/test_lifeguard_core.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.3.0/tests/test_notifications.py` & `lifeguard-1.4.0/tests/test_notifications.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.3.0/tests/test_repositories.py` & `lifeguard-1.4.0/tests/test_repositories.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.3.0/tests/test_server.py` & `lifeguard-1.4.0/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.3.0/tests/test_settings.py` & `lifeguard-1.4.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.3.0/tests/test_validations.py` & `lifeguard-1.4.0/tests/test_validations.py`

 * *Files identical despite different names*

