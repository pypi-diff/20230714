# Comparing `tmp/aa-discordnotify-1.1.1.tar.gz` & `tmp/aa_discordnotify-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-discordnotify-1.1.1.tar", last modified: Fri Jun 17 12:26:19 2022, max compression
+gzip compressed data, was "aa_discordnotify-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aa-discordnotify-1.1.1.tar` & `aa_discordnotify-1.2.0.tar`

### file list

```diff
@@ -1,31 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-17 12:26:19.032234 aa-discordnotify-1.1.1/
--rw-rw-rw-   0 root         (0) root         (0)     1070 2021-03-12 20:32:47.000000 aa-discordnotify-1.1.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      102 2021-03-13 14:13:16.000000 aa-discordnotify-1.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5092 2022-06-17 12:26:19.032234 aa-discordnotify-1.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4179 2021-04-16 23:02:23.000000 aa-discordnotify-1.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-17 12:26:19.028234 aa-discordnotify-1.1.1/aa_discordnotify.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5092 2022-06-17 12:26:18.000000 aa-discordnotify-1.1.1/aa_discordnotify.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      600 2022-06-17 12:26:18.000000 aa-discordnotify-1.1.1/aa_discordnotify.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-17 12:26:18.000000 aa-discordnotify-1.1.1/aa_discordnotify.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2022-06-17 12:26:18.000000 aa-discordnotify-1.1.1/aa_discordnotify.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2022-06-17 12:26:18.000000 aa-discordnotify-1.1.1/aa_discordnotify.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-17 12:26:19.032234 aa-discordnotify-1.1.1/discordnotify/
--rw-rw-rw-   0 root         (0) root         (0)      114 2022-06-17 12:03:03.000000 aa-discordnotify-1.1.1/discordnotify/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      665 2021-04-16 23:02:23.000000 aa-discordnotify-1.1.1/discordnotify/app_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      229 2021-03-12 20:32:47.000000 aa-discordnotify-1.1.1/discordnotify/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      212 2021-03-13 20:20:25.000000 aa-discordnotify-1.1.1/discordnotify/auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     2351 2021-12-29 22:00:17.000000 aa-discordnotify-1.1.1/discordnotify/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-17 12:26:19.032234 aa-discordnotify-1.1.1/discordnotify/migrations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-03-12 20:32:47.000000 aa-discordnotify-1.1.1/discordnotify/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1781 2021-04-16 23:02:23.000000 aa-discordnotify-1.1.1/discordnotify/signals.py
--rw-rw-rw-   0 root         (0) root         (0)     1255 2021-12-29 22:00:17.000000 aa-discordnotify-1.1.1/discordnotify/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)      176 2021-03-13 20:20:25.000000 aa-discordnotify-1.1.1/discordnotify/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      580 2021-03-30 12:03:26.000000 aa-discordnotify-1.1.1/discordnotify/views.py
--rw-rw-rw-   0 root         (0) root         (0)      187 2022-06-17 12:26:19.032234 aa-discordnotify-1.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1586 2021-12-29 22:13:08.000000 aa-discordnotify-1.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-17 12:26:19.032234 aa-discordnotify-1.1.1/testauth/
--rw-rw-rw-   0 root         (0) root         (0)       46 2021-03-12 20:32:47.000000 aa-discordnotify-1.1.1/testauth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      612 2021-03-12 20:32:47.000000 aa-discordnotify-1.1.1/testauth/celery.py
--rw-rw-rw-   0 root         (0) root         (0)    10080 2021-12-28 19:35:45.000000 aa-discordnotify-1.1.1/testauth/settings.py
--rw-rw-rw-   0 root         (0) root         (0)      121 2021-03-12 20:32:47.000000 aa-discordnotify-1.1.1/testauth/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      397 2021-03-12 20:32:47.000000 aa-discordnotify-1.1.1/testauth/wsgi.py
+-rw-r--r--   0        0        0     1070 2021-03-12 20:32:47.332721 aa_discordnotify-1.2.0/LICENSE
+-rw-r--r--   0        0        0     4179 2021-04-16 23:02:23.491958 aa_discordnotify-1.2.0/README.md
+-rw-r--r--   0        0        0      178 2023-07-14 11:31:09.713456 aa_discordnotify-1.2.0/discordnotify/__init__.py
+-rw-r--r--   0        0        0      665 2021-04-16 23:02:23.491958 aa_discordnotify-1.2.0/discordnotify/app_settings.py
+-rw-r--r--   0        0        0      229 2021-03-12 20:32:47.332721 aa_discordnotify-1.2.0/discordnotify/apps.py
+-rw-r--r--   0        0        0      212 2021-03-13 20:20:25.313908 aa_discordnotify-1.2.0/discordnotify/auth_hooks.py
+-rw-r--r--   0        0        0     2351 2021-12-29 22:00:17.139779 aa_discordnotify-1.2.0/discordnotify/core.py
+-rw-r--r--   0        0        0        0 2023-07-14 12:48:05.696896 aa_discordnotify-1.2.0/discordnotify/migrations/__init__.py
+-rw-r--r--   0        0        0     1808 2023-07-14 11:31:09.713456 aa_discordnotify-1.2.0/discordnotify/signals.py
+-rw-r--r--   0        0        0     1027 2021-12-28 19:35:45.108126 aa_discordnotify-1.2.0/discordnotify/static/discordnotify/discordnotify_logo.png
+-rw-r--r--   0        0        0     1255 2021-12-29 22:00:17.139779 aa_discordnotify-1.2.0/discordnotify/tasks.py
+-rw-r--r--   0        0        0        0 2023-07-14 12:48:05.700897 aa_discordnotify-1.2.0/discordnotify/tests/__init__.py
+-rw-r--r--   0        0        0     9267 2023-07-14 11:31:09.713456 aa_discordnotify-1.2.0/discordnotify/tests/test_integration.py
+-rw-r--r--   0        0        0      176 2021-03-13 20:20:25.317908 aa_discordnotify-1.2.0/discordnotify/urls.py
+-rw-r--r--   0        0        0      580 2021-03-30 12:03:26.011127 aa_discordnotify-1.2.0/discordnotify/views.py
+-rw-r--r--   0        0        0     1876 2023-07-14 11:31:09.713456 aa_discordnotify-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5457 1970-01-01 00:00:00.000000 aa_discordnotify-1.2.0/PKG-INFO
```

### Comparing `aa-discordnotify-1.1.1/LICENSE` & `aa_discordnotify-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-discordnotify-1.1.1/PKG-INFO` & `aa_discordnotify-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: aa-discordnotify
-Version: 1.1.1
-Summary: Forward Alliance Auth notifications to users on Discord
-Home-page: https://gitlab.com/ErikKalkoken/aa-discordnotify
-Author: Erik Kalkoken
-Author-email: kalkoken87@gmail.com
-License: MIT
-Platform: UNKNOWN
+Version: 1.2.0
+Summary: Forward Alliance Auth notifications to users on Discord.
+Author-email: Erik Kalkoken <kalkoken87@gmail.com>
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: ~=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
+Requires-Dist: allianceauth-app-utils>=1.19
+Requires-Dist: allianceauth>=3
+Requires-Dist: discordproxy>=1.3.0
+Project-URL: Changelog, https://gitlab.com/ErikKalkoken/aa-discordnotify/-/blob/master/CHANGELOG.md
+Project-URL: Homepage, https://gitlab.com/ErikKalkoken/aa-discordnotify
+Project-URL: Source, https://gitlab.com/ErikKalkoken/aa-discordnotify
+Project-URL: Tracker, https://gitlab.com/ErikKalkoken/aa-discordnotify/-/issues
 
 # Discord Notify
 
 Forward Alliance Auth notifications to users on Discord
 
 [![release](https://img.shields.io/pypi/v/aa-discordnotify?label=release)](https://pypi.org/project/aa-discordnotify/)
 [![python](https://img.shields.io/pypi/pyversions/aa-discordnotify)](https://pypi.org/project/aa-discordnotify/)
@@ -108,8 +111,7 @@
 Name | Description | Default
 -- | -- | --
 `DISCORDNOTIFY_ENABLED`| Set this to False to disable this app temporarily | `True`
 `DISCORDNOTIFY_DISCORDPROXY_PORT`| Port used to communicate with Discord Proxy. | `50051`
 `DISCORDNOTIFY_MARK_AS_VIEWED`| When enabled will mark all notifications as viewed that have been successfully submitted to Discord | `False`
 `DISCORDNOTIFY_SUPERUSER_ONLY`| When enabled only superusers will be get their notifications forwarded. | `False`
 
-
```

### Comparing `aa-discordnotify-1.1.1/README.md` & `aa_discordnotify-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `aa-discordnotify-1.1.1/discordnotify/app_settings.py` & `aa_discordnotify-1.2.0/discordnotify/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa-discordnotify-1.1.1/discordnotify/core.py` & `aa_discordnotify-1.2.0/discordnotify/core.py`

 * *Files identical despite different names*

### Comparing `aa-discordnotify-1.1.1/discordnotify/signals.py` & `aa_discordnotify-1.2.0/discordnotify/signals.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,21 +19,22 @@
         if created and (not DISCORDNOTIFY_SUPERUSER_ONLY or instance.user.is_superuser):
             logger.info(
                 "Processing notification %d for: %s", instance.id, instance.user
             )
             try:
                 discord_uid = instance.user.discord.uid
             except (AttributeError, ObjectDoesNotExist):
-                logger.info(
-                    "Can not forward notification to user %s, because he has no Discord account",
+                logger.warning(
+                    "Can not forward notification to user %s, "
+                    "because he has no Discord account",
                     instance.user,
                 )
                 return
-            # we are passing through the instance attributes, because it is not garanteed
-            # that the object has already been saved
+            # we are passing through the instance attributes,
+            # because it is not guaranteed that the object has already been saved
             task_forward_notification_to_discord.delay(
                 notification_id=instance.id,
                 discord_uid=discord_uid,
                 title=instance.title,
                 message=instance.message,
                 level=instance.level,
                 timestamp=instance.timestamp.isoformat(),
```

### Comparing `aa-discordnotify-1.1.1/discordnotify/tasks.py` & `aa_discordnotify-1.2.0/discordnotify/tasks.py`

 * *Files identical despite different names*

### Comparing `aa-discordnotify-1.1.1/discordnotify/views.py` & `aa_discordnotify-1.2.0/discordnotify/views.py`

 * *Files identical despite different names*

