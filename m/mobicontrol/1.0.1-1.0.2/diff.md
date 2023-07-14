# Comparing `tmp/mobicontrol-1.0.1.tar.gz` & `tmp/mobicontrol-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobicontrol-1.0.1.tar", last modified: Fri Jul 14 09:05:49 2023, max compression
+gzip compressed data, was "mobicontrol-1.0.2.tar", last modified: Fri Jul 14 09:07:55 2023, max compression
```

## Comparing `mobicontrol-1.0.1.tar` & `mobicontrol-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:05:49.300339 mobicontrol-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-14 09:05:49.300339 mobicontrol-1.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:05:49.296339 mobicontrol-1.0.1/mobicontrol/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:05:23.000000 mobicontrol-1.0.1/mobicontrol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:05:49.300339 mobicontrol-1.0.1/mobicontrol/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-14 09:05:23.000000 mobicontrol-1.0.1/mobicontrol/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-14 09:05:23.000000 mobicontrol-1.0.1/mobicontrol/cli/apply.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-14 09:05:23.000000 mobicontrol-1.0.1/mobicontrol/cli/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-14 09:05:23.000000 mobicontrol-1.0.1/mobicontrol/cli/policies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:05:49.300339 mobicontrol-1.0.1/mobicontrol/client/
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-14 09:05:23.000000 mobicontrol-1.0.1/mobicontrol/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-14 09:05:23.000000 mobicontrol-1.0.1/mobicontrol/client/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-14 09:05:23.000000 mobicontrol-1.0.1/mobicontrol/client/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-07-14 09:05:23.000000 mobicontrol-1.0.1/mobicontrol/client/policies.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-14 09:05:23.000000 mobicontrol-1.0.1/mobicontrol/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:05:49.296339 mobicontrol-1.0.1/mobicontrol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-14 09:05:49.000000 mobicontrol-1.0.1/mobicontrol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-14 09:05:49.000000 mobicontrol-1.0.1/mobicontrol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 09:05:49.000000 mobicontrol-1.0.1/mobicontrol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-14 09:05:49.000000 mobicontrol-1.0.1/mobicontrol.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-14 09:05:49.000000 mobicontrol-1.0.1/mobicontrol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 09:05:49.000000 mobicontrol-1.0.1/mobicontrol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 09:05:49.300339 mobicontrol-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-14 09:05:23.000000 mobicontrol-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:07:55.917663 mobicontrol-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-14 09:07:55.917663 mobicontrol-1.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:07:55.913663 mobicontrol-1.0.2/mobicontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:07:31.000000 mobicontrol-1.0.2/mobicontrol/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:07:55.913663 mobicontrol-1.0.2/mobicontrol/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-14 09:07:31.000000 mobicontrol-1.0.2/mobicontrol/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-14 09:07:31.000000 mobicontrol-1.0.2/mobicontrol/cli/apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-14 09:07:31.000000 mobicontrol-1.0.2/mobicontrol/cli/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-14 09:07:31.000000 mobicontrol-1.0.2/mobicontrol/cli/policies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:07:55.913663 mobicontrol-1.0.2/mobicontrol/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-14 09:07:31.000000 mobicontrol-1.0.2/mobicontrol/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-14 09:07:31.000000 mobicontrol-1.0.2/mobicontrol/client/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-14 09:07:31.000000 mobicontrol-1.0.2/mobicontrol/client/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-07-14 09:07:31.000000 mobicontrol-1.0.2/mobicontrol/client/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-14 09:07:31.000000 mobicontrol-1.0.2/mobicontrol/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:07:55.913663 mobicontrol-1.0.2/mobicontrol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-14 09:07:55.000000 mobicontrol-1.0.2/mobicontrol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-14 09:07:55.000000 mobicontrol-1.0.2/mobicontrol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 09:07:55.000000 mobicontrol-1.0.2/mobicontrol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-14 09:07:55.000000 mobicontrol-1.0.2/mobicontrol.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 09:07:55.000000 mobicontrol-1.0.2/mobicontrol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 09:07:55.000000 mobicontrol-1.0.2/mobicontrol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 09:07:55.917663 mobicontrol-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-14 09:07:31.000000 mobicontrol-1.0.2/setup.py
```

### Comparing `mobicontrol-1.0.1/mobicontrol/cli/__init__.py` & `mobicontrol-1.0.2/mobicontrol/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `mobicontrol-1.0.1/mobicontrol/cli/apply.py` & `mobicontrol-1.0.2/mobicontrol/cli/apply.py`

 * *Files identical despite different names*

### Comparing `mobicontrol-1.0.1/mobicontrol/cli/apps.py` & `mobicontrol-1.0.2/mobicontrol/cli/apps.py`

 * *Files identical despite different names*

### Comparing `mobicontrol-1.0.1/mobicontrol/cli/policies.py` & `mobicontrol-1.0.2/mobicontrol/cli/policies.py`

 * *Files identical despite different names*

### Comparing `mobicontrol-1.0.1/mobicontrol/client/__init__.py` & `mobicontrol-1.0.2/mobicontrol/client/__init__.py`

 * *Files identical despite different names*

### Comparing `mobicontrol-1.0.1/mobicontrol/client/apps.py` & `mobicontrol-1.0.2/mobicontrol/client/apps.py`

 * *Files identical despite different names*

### Comparing `mobicontrol-1.0.1/mobicontrol/client/auth.py` & `mobicontrol-1.0.2/mobicontrol/client/auth.py`

 * *Files identical despite different names*

### Comparing `mobicontrol-1.0.1/mobicontrol/client/policies.py` & `mobicontrol-1.0.2/mobicontrol/client/policies.py`

 * *Files identical despite different names*

