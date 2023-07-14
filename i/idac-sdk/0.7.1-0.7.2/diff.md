# Comparing `tmp/idac_sdk-0.7.1.tar.gz` & `tmp/idac_sdk-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idac_sdk-0.7.1.tar", last modified: Tue Apr 25 16:27:54 2023, max compression
+gzip compressed data, was "idac_sdk-0.7.2.tar", last modified: Fri Jul 14 10:01:57 2023, max compression
```

## Comparing `idac_sdk-0.7.1.tar` & `idac_sdk-0.7.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 vkumov     (501) staff       (20)        0 2023-04-25 16:27:54.739950 idac_sdk-0.7.1/
--rw-r--r--   0 vkumov     (501) staff       (20)      828 2023-04-25 16:27:54.739635 idac_sdk-0.7.1/PKG-INFO
--rw-r--r--   0 vkumov     (501) staff       (20)      126 2022-03-04 15:54:41.000000 idac_sdk-0.7.1/README.md
-drwxr-xr-x   0 vkumov     (501) staff       (20)        0 2023-04-25 16:27:54.716168 idac_sdk-0.7.1/idac_sdk/
--rw-r--r--   0 vkumov     (501) staff       (20)      513 2022-04-20 11:23:12.000000 idac_sdk-0.7.1/idac_sdk/__init__.py
--rw-r--r--   0 vkumov     (501) staff       (20)       22 2023-04-25 16:27:24.000000 idac_sdk-0.7.1/idac_sdk/_version.py
-drwxr-xr-x   0 vkumov     (501) staff       (20)        0 2023-04-25 16:27:54.721219 idac_sdk-0.7.1/idac_sdk/asynced/
--rw-r--r--   0 vkumov     (501) staff       (20)       39 2022-04-21 13:26:08.000000 idac_sdk-0.7.1/idac_sdk/asynced/__init__.py
--rw-r--r--   0 vkumov     (501) staff       (20)     3191 2022-04-21 13:18:14.000000 idac_sdk-0.7.1/idac_sdk/asynced/controller.py
--rw-r--r--   0 vkumov     (501) staff       (20)    13215 2023-04-25 16:25:48.000000 idac_sdk-0.7.1/idac_sdk/asynced/request.py
-drwxr-xr-x   0 vkumov     (501) staff       (20)        0 2023-04-25 16:27:54.723011 idac_sdk-0.7.1/idac_sdk/base/
--rw-r--r--   0 vkumov     (501) staff       (20)      775 2022-04-21 15:57:46.000000 idac_sdk-0.7.1/idac_sdk/base/__init__.py
--rw-r--r--   0 vkumov     (501) staff       (20)    10216 2023-04-25 16:25:56.000000 idac_sdk-0.7.1/idac_sdk/base/controller.py
--rw-r--r--   0 vkumov     (501) staff       (20)     6462 2022-09-30 14:15:09.000000 idac_sdk-0.7.1/idac_sdk/base/request.py
-drwxr-xr-x   0 vkumov     (501) staff       (20)        0 2023-04-25 16:27:54.724010 idac_sdk-0.7.1/idac_sdk/cli/
--rw-r--r--   0 vkumov     (501) staff       (20)        0 2022-03-02 10:42:29.000000 idac_sdk-0.7.1/idac_sdk/cli/__init__.py
-drwxr-xr-x   0 vkumov     (501) staff       (20)        0 2023-04-25 16:27:54.728611 idac_sdk-0.7.1/idac_sdk/cli/commands/
--rw-r--r--   0 vkumov     (501) staff       (20)        0 2022-03-02 14:57:36.000000 idac_sdk-0.7.1/idac_sdk/cli/commands/__init__.py
--rw-r--r--   0 vkumov     (501) staff       (20)      971 2022-03-08 12:09:25.000000 idac_sdk-0.7.1/idac_sdk/cli/commands/cleanup.py
--rw-r--r--   0 vkumov     (501) staff       (20)     4674 2022-03-18 16:42:32.000000 idac_sdk-0.7.1/idac_sdk/cli/commands/config.py
--rw-r--r--   0 vkumov     (501) staff       (20)     5164 2023-04-25 16:26:02.000000 idac_sdk-0.7.1/idac_sdk/cli/commands/create.py
--rw-r--r--   0 vkumov     (501) staff       (20)      854 2022-03-08 12:10:08.000000 idac_sdk-0.7.1/idac_sdk/cli/commands/extend.py
--rw-r--r--   0 vkumov     (501) staff       (20)      754 2022-03-08 12:10:43.000000 idac_sdk-0.7.1/idac_sdk/cli/commands/restart.py
--rw-r--r--   0 vkumov     (501) staff       (20)     1685 2022-03-22 16:48:08.000000 idac_sdk-0.7.1/idac_sdk/cli/commands/status.py
--rw-r--r--   0 vkumov     (501) staff       (20)      941 2022-03-08 12:49:55.000000 idac_sdk-0.7.1/idac_sdk/cli/idac.py
-drwxr-xr-x   0 vkumov     (501) staff       (20)        0 2023-04-25 16:27:54.731019 idac_sdk-0.7.1/idac_sdk/cli/lib/
--rw-r--r--   0 vkumov     (501) staff       (20)        0 2022-03-01 14:23:45.000000 idac_sdk-0.7.1/idac_sdk/cli/lib/__init__.py
--rw-r--r--   0 vkumov     (501) staff       (20)     2100 2022-03-18 16:42:32.000000 idac_sdk-0.7.1/idac_sdk/cli/lib/_controller_options.py
--rw-r--r--   0 vkumov     (501) staff       (20)     2512 2023-04-25 16:26:09.000000 idac_sdk-0.7.1/idac_sdk/cli/lib/_helpers.py
--rw-r--r--   0 vkumov     (501) staff       (20)     2563 2022-04-22 08:11:32.000000 idac_sdk-0.7.1/idac_sdk/cli/lib/_vpn_options.py
-drwxr-xr-x   0 vkumov     (501) staff       (20)        0 2023-04-25 16:27:54.731744 idac_sdk-0.7.1/idac_sdk/config/
--rw-r--r--   0 vkumov     (501) staff       (20)     2219 2022-03-18 11:31:57.000000 idac_sdk-0.7.1/idac_sdk/config/__init__.py
--rw-r--r--   0 vkumov     (501) staff       (20)      832 2022-03-22 16:53:21.000000 idac_sdk-0.7.1/idac_sdk/errors.py
-drwxr-xr-x   0 vkumov     (501) staff       (20)        0 2023-04-25 16:27:54.733115 idac_sdk-0.7.1/idac_sdk/lib/
--rw-r--r--   0 vkumov     (501) staff       (20)        0 2022-03-18 11:31:57.000000 idac_sdk-0.7.1/idac_sdk/lib/__init__.py
--rw-r--r--   0 vkumov     (501) staff       (20)      646 2023-04-25 16:26:14.000000 idac_sdk-0.7.1/idac_sdk/lib/_helpers.py
--rw-r--r--   0 vkumov     (501) staff       (20)      703 2022-04-21 12:26:37.000000 idac_sdk-0.7.1/idac_sdk/log.py
-drwxr-xr-x   0 vkumov     (501) staff       (20)        0 2023-04-25 16:27:54.737072 idac_sdk-0.7.1/idac_sdk/models/
--rw-r--r--   0 vkumov     (501) staff       (20)        0 2022-02-15 16:51:03.000000 idac_sdk-0.7.1/idac_sdk/models/__init__.py
--rw-r--r--   0 vkumov     (501) staff       (20)      123 2022-03-18 16:42:32.000000 idac_sdk-0.7.1/idac_sdk/models/auth.py
--rw-r--r--   0 vkumov     (501) staff       (20)      435 2022-03-18 16:42:32.000000 idac_sdk-0.7.1/idac_sdk/models/config.py
--rw-r--r--   0 vkumov     (501) staff       (20)      460 2022-02-16 10:03:45.000000 idac_sdk-0.7.1/idac_sdk/models/new_request.py
--rw-r--r--   0 vkumov     (501) staff       (20)     3344 2022-04-22 08:28:14.000000 idac_sdk-0.7.1/idac_sdk/models/request_state.py
--rw-r--r--   0 vkumov     (501) staff       (20)      758 2022-04-20 11:23:00.000000 idac_sdk-0.7.1/idac_sdk/models/vpn_config.py
--rw-r--r--   0 vkumov     (501) staff       (20)     6204 2023-04-25 16:25:39.000000 idac_sdk-0.7.1/idac_sdk/session_data.py
-drwxr-xr-x   0 vkumov     (501) staff       (20)        0 2023-04-25 16:27:54.739022 idac_sdk-0.7.1/idac_sdk/synced/
--rw-r--r--   0 vkumov     (501) staff       (20)       38 2022-02-28 15:43:21.000000 idac_sdk-0.7.1/idac_sdk/synced/__init__.py
--rw-r--r--   0 vkumov     (501) staff       (20)     3302 2022-04-21 13:17:55.000000 idac_sdk-0.7.1/idac_sdk/synced/controller.py
--rw-r--r--   0 vkumov     (501) staff       (20)    13039 2023-04-25 16:26:20.000000 idac_sdk-0.7.1/idac_sdk/synced/request.py
--rw-r--r--   0 vkumov     (501) staff       (20)      734 2022-03-18 11:31:57.000000 idac_sdk-0.7.1/idac_sdk/types.py
-drwxr-xr-x   0 vkumov     (501) staff       (20)        0 2023-04-25 16:27:54.719439 idac_sdk-0.7.1/idac_sdk.egg-info/
--rw-r--r--   0 vkumov     (501) staff       (20)      828 2023-04-25 16:27:54.000000 idac_sdk-0.7.1/idac_sdk.egg-info/PKG-INFO
--rw-r--r--   0 vkumov     (501) staff       (20)     1239 2023-04-25 16:27:54.000000 idac_sdk-0.7.1/idac_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 vkumov     (501) staff       (20)        1 2023-04-25 16:27:54.000000 idac_sdk-0.7.1/idac_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 vkumov     (501) staff       (20)       48 2023-04-25 16:27:54.000000 idac_sdk-0.7.1/idac_sdk.egg-info/entry_points.txt
--rw-r--r--   0 vkumov     (501) staff       (20)      118 2023-04-25 16:27:54.000000 idac_sdk-0.7.1/idac_sdk.egg-info/requires.txt
--rw-r--r--   0 vkumov     (501) staff       (20)        9 2023-04-25 16:27:54.000000 idac_sdk-0.7.1/idac_sdk.egg-info/top_level.txt
--rw-r--r--   0 vkumov     (501) staff       (20)       38 2023-04-25 16:27:54.740059 idac_sdk-0.7.1/setup.cfg
--rw-r--r--   0 vkumov     (501) staff       (20)     1688 2023-04-25 16:25:29.000000 idac_sdk-0.7.1/setup.py
+drwxr-xr-x   0 duferrei   (501) staff       (20)        0 2023-07-14 10:01:57.364268 idac_sdk-0.7.2/
+-rw-r--r--   0 duferrei   (501) staff       (20)      847 2023-07-14 10:01:57.363959 idac_sdk-0.7.2/PKG-INFO
+-rw-r--r--   0 duferrei   (501) staff       (20)      126 2022-03-16 10:33:13.000000 idac_sdk-0.7.2/README.md
+drwxr-xr-x   0 duferrei   (501) staff       (20)        0 2023-07-14 10:01:57.343703 idac_sdk-0.7.2/idac_sdk/
+-rw-r--r--   0 duferrei   (501) staff       (20)      513 2023-01-16 09:47:06.000000 idac_sdk-0.7.2/idac_sdk/__init__.py
+-rw-r--r--   0 duferrei   (501) staff       (20)       22 2023-07-14 10:01:52.000000 idac_sdk-0.7.2/idac_sdk/_version.py
+drwxr-xr-x   0 duferrei   (501) staff       (20)        0 2023-07-14 10:01:57.349039 idac_sdk-0.7.2/idac_sdk/asynced/
+-rw-r--r--   0 duferrei   (501) staff       (20)       39 2023-01-16 09:47:06.000000 idac_sdk-0.7.2/idac_sdk/asynced/__init__.py
+-rw-r--r--   0 duferrei   (501) staff       (20)     3191 2023-01-16 09:47:06.000000 idac_sdk-0.7.2/idac_sdk/asynced/controller.py
+-rw-r--r--   0 duferrei   (501) staff       (20)    13215 2023-07-13 17:03:00.000000 idac_sdk-0.7.2/idac_sdk/asynced/request.py
+drwxr-xr-x   0 duferrei   (501) staff       (20)        0 2023-07-14 10:01:57.350138 idac_sdk-0.7.2/idac_sdk/base/
+-rw-r--r--   0 duferrei   (501) staff       (20)      775 2023-01-16 09:47:06.000000 idac_sdk-0.7.2/idac_sdk/base/__init__.py
+-rw-r--r--   0 duferrei   (501) staff       (20)    10216 2023-07-13 17:01:39.000000 idac_sdk-0.7.2/idac_sdk/base/controller.py
+-rw-r--r--   0 duferrei   (501) staff       (20)     6462 2023-01-16 09:47:06.000000 idac_sdk-0.7.2/idac_sdk/base/request.py
+drwxr-xr-x   0 duferrei   (501) staff       (20)        0 2023-07-14 10:01:57.351024 idac_sdk-0.7.2/idac_sdk/cli/
+-rw-r--r--   0 duferrei   (501) staff       (20)        0 2022-03-16 10:33:13.000000 idac_sdk-0.7.2/idac_sdk/cli/__init__.py
+drwxr-xr-x   0 duferrei   (501) staff       (20)        0 2023-07-14 10:01:57.354174 idac_sdk-0.7.2/idac_sdk/cli/commands/
+-rw-r--r--   0 duferrei   (501) staff       (20)        0 2022-03-16 10:33:13.000000 idac_sdk-0.7.2/idac_sdk/cli/commands/__init__.py
+-rw-r--r--   0 duferrei   (501) staff       (20)      971 2022-03-16 10:33:13.000000 idac_sdk-0.7.2/idac_sdk/cli/commands/cleanup.py
+-rw-r--r--   0 duferrei   (501) staff       (20)     4674 2023-01-16 09:47:06.000000 idac_sdk-0.7.2/idac_sdk/cli/commands/config.py
+-rw-r--r--   0 duferrei   (501) staff       (20)     5164 2023-07-13 12:57:28.000000 idac_sdk-0.7.2/idac_sdk/cli/commands/create.py
+-rw-r--r--   0 duferrei   (501) staff       (20)      854 2022-03-16 10:33:13.000000 idac_sdk-0.7.2/idac_sdk/cli/commands/extend.py
+-rw-r--r--   0 duferrei   (501) staff       (20)      754 2022-03-16 10:33:13.000000 idac_sdk-0.7.2/idac_sdk/cli/commands/restart.py
+-rw-r--r--   0 duferrei   (501) staff       (20)     1685 2023-01-16 09:47:06.000000 idac_sdk-0.7.2/idac_sdk/cli/commands/status.py
+-rw-r--r--   0 duferrei   (501) staff       (20)      941 2022-03-16 10:33:13.000000 idac_sdk-0.7.2/idac_sdk/cli/idac.py
+drwxr-xr-x   0 duferrei   (501) staff       (20)        0 2023-07-14 10:01:57.355968 idac_sdk-0.7.2/idac_sdk/cli/lib/
+-rw-r--r--   0 duferrei   (501) staff       (20)        0 2022-03-16 10:33:13.000000 idac_sdk-0.7.2/idac_sdk/cli/lib/__init__.py
+-rw-r--r--   0 duferrei   (501) staff       (20)     2100 2023-01-16 09:47:06.000000 idac_sdk-0.7.2/idac_sdk/cli/lib/_controller_options.py
+-rw-r--r--   0 duferrei   (501) staff       (20)     2512 2023-07-13 12:57:28.000000 idac_sdk-0.7.2/idac_sdk/cli/lib/_helpers.py
+-rw-r--r--   0 duferrei   (501) staff       (20)     2563 2023-01-16 09:47:06.000000 idac_sdk-0.7.2/idac_sdk/cli/lib/_vpn_options.py
+drwxr-xr-x   0 duferrei   (501) staff       (20)        0 2023-07-14 10:01:57.356491 idac_sdk-0.7.2/idac_sdk/config/
+-rw-r--r--   0 duferrei   (501) staff       (20)     2219 2023-01-16 09:47:06.000000 idac_sdk-0.7.2/idac_sdk/config/__init__.py
+-rw-r--r--   0 duferrei   (501) staff       (20)      832 2023-01-16 09:47:06.000000 idac_sdk-0.7.2/idac_sdk/errors.py
+drwxr-xr-x   0 duferrei   (501) staff       (20)        0 2023-07-14 10:01:57.357455 idac_sdk-0.7.2/idac_sdk/lib/
+-rw-r--r--   0 duferrei   (501) staff       (20)        0 2023-01-16 09:47:06.000000 idac_sdk-0.7.2/idac_sdk/lib/__init__.py
+-rw-r--r--   0 duferrei   (501) staff       (20)      646 2023-07-13 12:57:28.000000 idac_sdk-0.7.2/idac_sdk/lib/_helpers.py
+-rw-r--r--   0 duferrei   (501) staff       (20)      703 2023-01-16 09:47:06.000000 idac_sdk-0.7.2/idac_sdk/log.py
+drwxr-xr-x   0 duferrei   (501) staff       (20)        0 2023-07-14 10:01:57.361503 idac_sdk-0.7.2/idac_sdk/models/
+-rw-r--r--   0 duferrei   (501) staff       (20)        0 2022-03-16 10:33:13.000000 idac_sdk-0.7.2/idac_sdk/models/__init__.py
+-rw-r--r--   0 duferrei   (501) staff       (20)      123 2023-01-16 09:47:06.000000 idac_sdk-0.7.2/idac_sdk/models/auth.py
+-rw-r--r--   0 duferrei   (501) staff       (20)      435 2023-01-16 09:47:06.000000 idac_sdk-0.7.2/idac_sdk/models/config.py
+-rw-r--r--   0 duferrei   (501) staff       (20)      460 2022-03-16 10:33:13.000000 idac_sdk-0.7.2/idac_sdk/models/new_request.py
+-rw-r--r--   0 duferrei   (501) staff       (20)     3344 2023-01-16 09:47:06.000000 idac_sdk-0.7.2/idac_sdk/models/request_state.py
+-rw-r--r--   0 duferrei   (501) staff       (20)      758 2023-01-16 09:47:06.000000 idac_sdk-0.7.2/idac_sdk/models/vpn_config.py
+-rw-r--r--   0 duferrei   (501) staff       (20)     6204 2023-07-13 12:57:28.000000 idac_sdk-0.7.2/idac_sdk/session_data.py
+drwxr-xr-x   0 duferrei   (501) staff       (20)        0 2023-07-14 10:01:57.363368 idac_sdk-0.7.2/idac_sdk/synced/
+-rw-r--r--   0 duferrei   (501) staff       (20)       38 2022-03-16 10:33:13.000000 idac_sdk-0.7.2/idac_sdk/synced/__init__.py
+-rw-r--r--   0 duferrei   (501) staff       (20)     3302 2023-01-16 09:47:06.000000 idac_sdk-0.7.2/idac_sdk/synced/controller.py
+-rw-r--r--   0 duferrei   (501) staff       (20)    13039 2023-07-13 12:57:28.000000 idac_sdk-0.7.2/idac_sdk/synced/request.py
+-rw-r--r--   0 duferrei   (501) staff       (20)      734 2023-01-16 09:47:06.000000 idac_sdk-0.7.2/idac_sdk/types.py
+drwxr-xr-x   0 duferrei   (501) staff       (20)        0 2023-07-14 10:01:57.347521 idac_sdk-0.7.2/idac_sdk.egg-info/
+-rw-r--r--   0 duferrei   (501) staff       (20)      847 2023-07-14 10:01:57.000000 idac_sdk-0.7.2/idac_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 duferrei   (501) staff       (20)     1239 2023-07-14 10:01:57.000000 idac_sdk-0.7.2/idac_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 duferrei   (501) staff       (20)        1 2023-07-14 10:01:57.000000 idac_sdk-0.7.2/idac_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 duferrei   (501) staff       (20)       49 2023-07-14 10:01:57.000000 idac_sdk-0.7.2/idac_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 duferrei   (501) staff       (20)      125 2023-07-14 10:01:57.000000 idac_sdk-0.7.2/idac_sdk.egg-info/requires.txt
+-rw-r--r--   0 duferrei   (501) staff       (20)        9 2023-07-14 10:01:57.000000 idac_sdk-0.7.2/idac_sdk.egg-info/top_level.txt
+-rw-r--r--   0 duferrei   (501) staff       (20)       38 2023-07-14 10:01:57.364395 idac_sdk-0.7.2/setup.cfg
+-rw-r--r--   0 duferrei   (501) staff       (20)     1695 2023-07-14 10:00:40.000000 idac_sdk-0.7.2/setup.py
```

### Comparing `idac_sdk-0.7.1/PKG-INFO` & `idac_sdk-0.7.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: idac_sdk
-Version: 0.7.1
+Version: 0.7.2
 Summary: Python 3 SDK for iDAC
 Home-page: https://www-github.cisco.com/GDE-Content-Engineering/idac-sdk-python
 Author: Cisco GDE CAT
 Author-email: cat-dev-support@cisco.com
 License: MIT
 Keywords: idac sdk
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 
 # Python3 SDK for iDAC
 
 Docs are available [here](https://www-github.cisco.com/pages/GDE-Content-Engineering/idac-sdk-python/)
+
```

### Comparing `idac_sdk-0.7.1/idac_sdk/__init__.py` & `idac_sdk-0.7.2/idac_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.1/idac_sdk/asynced/controller.py` & `idac_sdk-0.7.2/idac_sdk/asynced/controller.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.1/idac_sdk/asynced/request.py` & `idac_sdk-0.7.2/idac_sdk/asynced/request.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.1/idac_sdk/base/__init__.py` & `idac_sdk-0.7.2/idac_sdk/base/__init__.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.1/idac_sdk/base/controller.py` & `idac_sdk-0.7.2/idac_sdk/base/controller.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.1/idac_sdk/base/request.py` & `idac_sdk-0.7.2/idac_sdk/base/request.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.1/idac_sdk/cli/commands/cleanup.py` & `idac_sdk-0.7.2/idac_sdk/cli/commands/cleanup.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.1/idac_sdk/cli/commands/config.py` & `idac_sdk-0.7.2/idac_sdk/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.1/idac_sdk/cli/commands/create.py` & `idac_sdk-0.7.2/idac_sdk/cli/commands/create.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.1/idac_sdk/cli/commands/extend.py` & `idac_sdk-0.7.2/idac_sdk/cli/commands/extend.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.1/idac_sdk/cli/commands/restart.py` & `idac_sdk-0.7.2/idac_sdk/cli/commands/restart.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.1/idac_sdk/cli/commands/status.py` & `idac_sdk-0.7.2/idac_sdk/cli/commands/status.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.1/idac_sdk/cli/idac.py` & `idac_sdk-0.7.2/idac_sdk/cli/idac.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.1/idac_sdk/cli/lib/_controller_options.py` & `idac_sdk-0.7.2/idac_sdk/cli/lib/_controller_options.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.1/idac_sdk/cli/lib/_helpers.py` & `idac_sdk-0.7.2/idac_sdk/cli/lib/_helpers.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.1/idac_sdk/cli/lib/_vpn_options.py` & `idac_sdk-0.7.2/idac_sdk/cli/lib/_vpn_options.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.1/idac_sdk/config/__init__.py` & `idac_sdk-0.7.2/idac_sdk/config/__init__.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.1/idac_sdk/errors.py` & `idac_sdk-0.7.2/idac_sdk/errors.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.1/idac_sdk/lib/_helpers.py` & `idac_sdk-0.7.2/idac_sdk/lib/_helpers.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.1/idac_sdk/log.py` & `idac_sdk-0.7.2/idac_sdk/log.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.1/idac_sdk/models/request_state.py` & `idac_sdk-0.7.2/idac_sdk/models/request_state.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.1/idac_sdk/models/vpn_config.py` & `idac_sdk-0.7.2/idac_sdk/models/vpn_config.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.1/idac_sdk/session_data.py` & `idac_sdk-0.7.2/idac_sdk/session_data.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.1/idac_sdk/synced/controller.py` & `idac_sdk-0.7.2/idac_sdk/synced/controller.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.1/idac_sdk/synced/request.py` & `idac_sdk-0.7.2/idac_sdk/synced/request.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.1/idac_sdk/types.py` & `idac_sdk-0.7.2/idac_sdk/types.py`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.1/idac_sdk.egg-info/PKG-INFO` & `idac_sdk-0.7.2/idac_sdk.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: idac-sdk
-Version: 0.7.1
+Version: 0.7.2
 Summary: Python 3 SDK for iDAC
 Home-page: https://www-github.cisco.com/GDE-Content-Engineering/idac-sdk-python
 Author: Cisco GDE CAT
 Author-email: cat-dev-support@cisco.com
 License: MIT
 Keywords: idac sdk
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 
 # Python3 SDK for iDAC
 
 Docs are available [here](https://www-github.cisco.com/pages/GDE-Content-Engineering/idac-sdk-python/)
+
```

### Comparing `idac_sdk-0.7.1/idac_sdk.egg-info/SOURCES.txt` & `idac_sdk-0.7.2/idac_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idac_sdk-0.7.1/setup.py` & `idac_sdk-0.7.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     url="https://www-github.cisco.com/GDE-Content-Engineering/idac-sdk-python",
     packages=find_packages(include=["idac_sdk", "idac_sdk.*", "tests"]),
     long_description=read("README.md"),
     install_requires=[
         "asyncclick>=8.0.3.2",
         "httpx>=0.22.0",
         "xmltodict>=0.12.0",
-        "pydantic>=1.9.0",
+        "pydantic>=1.9.0,<2.0.0",
         "deepmerge>=1.0.1",
         "PyYAML>=5.4.1",
         "jsonpath-ng>=1.5.3",
     ],
     python_requires=">=3.7",
     classifiers=[
         "Development Status :: 4 - Beta",
```

