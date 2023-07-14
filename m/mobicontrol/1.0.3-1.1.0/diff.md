# Comparing `tmp/mobicontrol-1.0.3.tar.gz` & `tmp/mobicontrol-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobicontrol-1.0.3.tar", last modified: Fri Jul 14 09:13:18 2023, max compression
+gzip compressed data, was "mobicontrol-1.1.0.tar", last modified: Fri Jul 14 11:41:03 2023, max compression
```

## Comparing `mobicontrol-1.0.3.tar` & `mobicontrol-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:13:18.794892 mobicontrol-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-14 09:13:18.794892 mobicontrol-1.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:13:18.790892 mobicontrol-1.0.3/mobicontrol/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:12:49.000000 mobicontrol-1.0.3/mobicontrol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:13:18.794892 mobicontrol-1.0.3/mobicontrol/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-14 09:12:49.000000 mobicontrol-1.0.3/mobicontrol/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-14 09:12:49.000000 mobicontrol-1.0.3/mobicontrol/cli/apply.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-14 09:12:49.000000 mobicontrol-1.0.3/mobicontrol/cli/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-14 09:12:49.000000 mobicontrol-1.0.3/mobicontrol/cli/policies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:13:18.794892 mobicontrol-1.0.3/mobicontrol/client/
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-14 09:12:49.000000 mobicontrol-1.0.3/mobicontrol/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-14 09:12:49.000000 mobicontrol-1.0.3/mobicontrol/client/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-14 09:12:49.000000 mobicontrol-1.0.3/mobicontrol/client/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-07-14 09:12:49.000000 mobicontrol-1.0.3/mobicontrol/client/policies.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-14 09:12:49.000000 mobicontrol-1.0.3/mobicontrol/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:13:18.790892 mobicontrol-1.0.3/mobicontrol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-14 09:13:18.000000 mobicontrol-1.0.3/mobicontrol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-14 09:13:18.000000 mobicontrol-1.0.3/mobicontrol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 09:13:18.000000 mobicontrol-1.0.3/mobicontrol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-14 09:13:18.000000 mobicontrol-1.0.3/mobicontrol.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 09:13:18.000000 mobicontrol-1.0.3/mobicontrol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 09:13:18.000000 mobicontrol-1.0.3/mobicontrol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 09:13:18.794892 mobicontrol-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-14 09:12:49.000000 mobicontrol-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:41:03.455071 mobicontrol-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-14 11:41:03.455071 mobicontrol-1.1.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:41:03.455071 mobicontrol-1.1.0/mobicontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 11:40:39.000000 mobicontrol-1.1.0/mobicontrol/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:41:03.455071 mobicontrol-1.1.0/mobicontrol/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-14 11:40:39.000000 mobicontrol-1.1.0/mobicontrol/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-07-14 11:40:39.000000 mobicontrol-1.1.0/mobicontrol/cli/apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-14 11:40:39.000000 mobicontrol-1.1.0/mobicontrol/cli/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-14 11:40:39.000000 mobicontrol-1.1.0/mobicontrol/cli/policies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:41:03.455071 mobicontrol-1.1.0/mobicontrol/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-14 11:40:39.000000 mobicontrol-1.1.0/mobicontrol/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-14 11:40:39.000000 mobicontrol-1.1.0/mobicontrol/client/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-14 11:40:39.000000 mobicontrol-1.1.0/mobicontrol/client/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-07-14 11:40:39.000000 mobicontrol-1.1.0/mobicontrol/client/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-14 11:40:39.000000 mobicontrol-1.1.0/mobicontrol/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:41:03.455071 mobicontrol-1.1.0/mobicontrol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-14 11:41:03.000000 mobicontrol-1.1.0/mobicontrol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-14 11:41:03.000000 mobicontrol-1.1.0/mobicontrol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 11:41:03.000000 mobicontrol-1.1.0/mobicontrol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-14 11:41:03.000000 mobicontrol-1.1.0/mobicontrol.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 11:41:03.000000 mobicontrol-1.1.0/mobicontrol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 11:41:03.000000 mobicontrol-1.1.0/mobicontrol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 11:41:03.455071 mobicontrol-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-14 11:40:39.000000 mobicontrol-1.1.0/setup.py
```

### Comparing `mobicontrol-1.0.3/mobicontrol/cli/__init__.py` & `mobicontrol-1.1.0/mobicontrol/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `mobicontrol-1.0.3/mobicontrol/cli/apps.py` & `mobicontrol-1.1.0/mobicontrol/cli/apps.py`

 * *Files identical despite different names*

### Comparing `mobicontrol-1.0.3/mobicontrol/cli/policies.py` & `mobicontrol-1.1.0/mobicontrol/cli/policies.py`

 * *Files identical despite different names*

### Comparing `mobicontrol-1.0.3/mobicontrol/client/__init__.py` & `mobicontrol-1.1.0/mobicontrol/client/__init__.py`

 * *Files identical despite different names*

### Comparing `mobicontrol-1.0.3/mobicontrol/client/apps.py` & `mobicontrol-1.1.0/mobicontrol/client/apps.py`

 * *Files identical despite different names*

### Comparing `mobicontrol-1.0.3/mobicontrol/client/auth.py` & `mobicontrol-1.1.0/mobicontrol/client/auth.py`

 * *Files identical despite different names*

### Comparing `mobicontrol-1.0.3/mobicontrol/client/policies.py` & `mobicontrol-1.1.0/mobicontrol/client/policies.py`

 * *Files identical despite different names*

