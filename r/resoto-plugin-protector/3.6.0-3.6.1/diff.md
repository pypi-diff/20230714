# Comparing `tmp/resoto-plugin-protector-3.6.0.tar.gz` & `tmp/resoto-plugin-protector-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-protector-3.6.0.tar", last modified: Fri Jun 30 19:23:25 2023, max compression
+gzip compressed data, was "resoto-plugin-protector-3.6.1.tar", last modified: Fri Jul 14 17:05:20 2023, max compression
```

## Comparing `resoto-plugin-protector-3.6.0.tar` & `resoto-plugin-protector-3.6.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:23:25.751123 resoto-plugin-protector-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 19:20:00.000000 resoto-plugin-protector-3.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-30 19:23:25.751123 resoto-plugin-protector-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-30 19:20:00.000000 resoto-plugin-protector-3.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-30 19:20:00.000000 resoto-plugin-protector-3.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:23:25.751123 resoto-plugin-protector-3.6.0/resoto_plugin_protector/
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-30 19:20:00.000000 resoto-plugin-protector-3.6.0/resoto_plugin_protector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-06-30 19:20:00.000000 resoto-plugin-protector-3.6.0/resoto_plugin_protector/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:23:25.751123 resoto-plugin-protector-3.6.0/resoto_plugin_protector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-30 19:23:25.000000 resoto-plugin-protector-3.6.0/resoto_plugin_protector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-30 19:23:25.000000 resoto-plugin-protector-3.6.0/resoto_plugin_protector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:23:25.000000 resoto-plugin-protector-3.6.0/resoto_plugin_protector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-30 19:23:25.000000 resoto-plugin-protector-3.6.0/resoto_plugin_protector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:21:25.000000 resoto-plugin-protector-3.6.0/resoto_plugin_protector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-30 19:23:25.000000 resoto-plugin-protector-3.6.0/resoto_plugin_protector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-30 19:23:25.000000 resoto-plugin-protector-3.6.0/resoto_plugin_protector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-30 19:23:25.751123 resoto-plugin-protector-3.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:23:25.751123 resoto-plugin-protector-3.6.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-30 19:20:00.000000 resoto-plugin-protector-3.6.0/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:20.211890 resoto-plugin-protector-3.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 17:01:07.000000 resoto-plugin-protector-3.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-14 17:05:20.211890 resoto-plugin-protector-3.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-14 17:01:07.000000 resoto-plugin-protector-3.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-14 17:01:07.000000 resoto-plugin-protector-3.6.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:20.207889 resoto-plugin-protector-3.6.1/resoto_plugin_protector/
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-14 17:01:07.000000 resoto-plugin-protector-3.6.1/resoto_plugin_protector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-07-14 17:01:07.000000 resoto-plugin-protector-3.6.1/resoto_plugin_protector/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:20.211890 resoto-plugin-protector-3.6.1/resoto_plugin_protector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-14 17:05:20.000000 resoto-plugin-protector-3.6.1/resoto_plugin_protector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-14 17:05:20.000000 resoto-plugin-protector-3.6.1/resoto_plugin_protector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:05:20.000000 resoto-plugin-protector-3.6.1/resoto_plugin_protector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-14 17:05:20.000000 resoto-plugin-protector-3.6.1/resoto_plugin_protector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:02:50.000000 resoto-plugin-protector-3.6.1/resoto_plugin_protector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 17:05:20.000000 resoto-plugin-protector-3.6.1/resoto_plugin_protector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-14 17:05:20.000000 resoto-plugin-protector-3.6.1/resoto_plugin_protector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-14 17:05:20.211890 resoto-plugin-protector-3.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:20.211890 resoto-plugin-protector-3.6.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-14 17:01:07.000000 resoto-plugin-protector-3.6.1/test/test_config.py
```

### Comparing `resoto-plugin-protector-3.6.0/PKG-INFO` & `resoto-plugin-protector-3.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-protector
-Version: 3.6.0
+Version: 3.6.1
 Summary: Resoto Protector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/protector
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-protector-3.6.0/README.md` & `resoto-plugin-protector-3.6.1/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-protector-3.6.0/pyproject.toml` & `resoto-plugin-protector-3.6.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-protector"
 description = "Resoto Protector Plugin"
-version = "3.6.0"
+version = "3.6.1"
 authors = [{name="Some Engineering Inc."}]
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
     # Audience
@@ -23,15 +23,15 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "resotolib==3.6.0",
+    "resotolib==3.6.1",
 ]
 
 [project.entry-points."resoto.plugins"]
 protector = "resoto_plugin_protector:ProtectorPlugin"
 
 [project.urls]
 Documentation = "https://resoto.com"
```

### Comparing `resoto-plugin-protector-3.6.0/resoto_plugin_protector/__init__.py` & `resoto-plugin-protector-3.6.1/resoto_plugin_protector/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-protector-3.6.0/resoto_plugin_protector/config.py` & `resoto-plugin-protector-3.6.1/resoto_plugin_protector/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-protector-3.6.0/resoto_plugin_protector.egg-info/PKG-INFO` & `resoto-plugin-protector-3.6.1/resoto_plugin_protector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-protector
-Version: 3.6.0
+Version: 3.6.1
 Summary: Resoto Protector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/protector
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

