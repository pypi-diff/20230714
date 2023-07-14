# Comparing `tmp/cohort-generator-0.2.1.tar.gz` & `tmp/cohort-generator-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cohort-generator-0.2.1.tar", last modified: Tue Jul 11 14:30:33 2023, max compression
+gzip compressed data, was "cohort-generator-0.2.2.tar", last modified: Fri Jul 14 10:13:53 2023, max compression
```

## Comparing `cohort-generator-0.2.1.tar` & `cohort-generator-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:33.876866 cohort-generator-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-11 14:30:33.876866 cohort-generator-0.2.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:33.876866 cohort-generator-0.2.1/cohort_generator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-11 14:30:33.000000 cohort-generator-0.2.1/cohort_generator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-11 14:30:33.000000 cohort-generator-0.2.1/cohort_generator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:30:33.000000 cohort-generator-0.2.1/cohort_generator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-11 14:30:33.000000 cohort-generator-0.2.1/cohort_generator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 14:30:33.000000 cohort-generator-0.2.1/cohort_generator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:33.876866 cohort-generator-0.2.1/ohdsi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:30:33.876866 cohort-generator-0.2.1/ohdsi/cohort_generator/
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-07-11 14:30:22.000000 cohort-generator-0.2.1/ohdsi/cohort_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-11 14:30:22.000000 cohort-generator-0.2.1/ohdsi/cohort_generator/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 14:30:33.876866 cohort-generator-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-11 14:30:22.000000 cohort-generator-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:53.442675 cohort-generator-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-14 10:13:53.442675 cohort-generator-0.2.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:53.442675 cohort-generator-0.2.2/cohort_generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-14 10:13:53.000000 cohort-generator-0.2.2/cohort_generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-14 10:13:53.000000 cohort-generator-0.2.2/cohort_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:13:53.000000 cohort-generator-0.2.2/cohort_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-14 10:13:53.000000 cohort-generator-0.2.2/cohort_generator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 10:13:53.000000 cohort-generator-0.2.2/cohort_generator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:53.442675 cohort-generator-0.2.2/ohdsi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:53.442675 cohort-generator-0.2.2/ohdsi/cohort_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)     9835 2023-07-14 10:13:44.000000 cohort-generator-0.2.2/ohdsi/cohort_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-14 10:13:44.000000 cohort-generator-0.2.2/ohdsi/cohort_generator/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 10:13:53.442675 cohort-generator-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-14 10:13:44.000000 cohort-generator-0.2.2/setup.py
```

### Comparing `cohort-generator-0.2.1/ohdsi/cohort_generator/main.py` & `cohort-generator-0.2.2/ohdsi/cohort_generator/main.py`

 * *Files identical despite different names*

### Comparing `cohort-generator-0.2.1/setup.py` & `cohort-generator-0.2.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,16 +28,16 @@
     install_requires=[
         'rpy2==3.5.12',
     ],
     extras_require={
         'dev': []
     },
     package_data={
-        'ohdsi.cohort_generator.data': [
-            'data/*'
+        'ohdsi.cohort_generator.cohorts': [
+            'data/cohort/*'
         ],
     },
     # entry_points={
     #     'console_scripts': [
     #         'vserver-local=vantage6.server.cli.server:cli_server'
     #     ]
     # }
```

