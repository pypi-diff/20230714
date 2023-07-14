# Comparing `tmp/dependencyhealth-0.0.1.tar.gz` & `tmp/dependencyhealth-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dependencyhealth-0.0.1.tar", last modified: Fri Jul 14 14:49:02 2023, max compression
+gzip compressed data, was "dependencyhealth-0.0.2.tar", last modified: Fri Jul 14 16:19:44 2023, max compression
```

## Comparing `dependencyhealth-0.0.1.tar` & `dependencyhealth-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 algo       (501) staff       (20)        0 2023-07-14 14:49:02.757646 dependencyhealth-0.0.1/
--rw-r--r--   0 algo       (501) staff       (20)     1073 2023-07-14 10:18:42.000000 dependencyhealth-0.0.1/LICENSE
--rw-r--r--   0 algo       (501) staff       (20)     1140 2023-07-14 14:49:02.757522 dependencyhealth-0.0.1/PKG-INFO
--rw-r--r--   0 algo       (501) staff       (20)      767 2023-07-14 13:41:30.000000 dependencyhealth-0.0.1/README.md
--rw-r--r--   0 algo       (501) staff       (20)      478 2023-07-14 14:48:42.000000 dependencyhealth-0.0.1/pyproject.toml
--rw-r--r--   0 algo       (501) staff       (20)       38 2023-07-14 14:49:02.757687 dependencyhealth-0.0.1/setup.cfg
-drwxr-xr-x   0 algo       (501) staff       (20)        0 2023-07-14 14:49:02.755738 dependencyhealth-0.0.1/src/
-drwxr-xr-x   0 algo       (501) staff       (20)        0 2023-07-14 14:49:02.756358 dependencyhealth-0.0.1/src/dependencyhealth/
--rw-r--r--   0 algo       (501) staff       (20)       44 2023-07-14 12:18:32.000000 dependencyhealth-0.0.1/src/dependencyhealth/__init__.py
--rw-r--r--   0 algo       (501) staff       (20)     1516 2023-07-14 12:40:12.000000 dependencyhealth-0.0.1/src/dependencyhealth/abstract_client.py
-drwxr-xr-x   0 algo       (501) staff       (20)        0 2023-07-14 14:49:02.757327 dependencyhealth-0.0.1/src/dependencyhealth/npm/
--rw-r--r--   0 algo       (501) staff       (20)       27 2023-07-14 12:18:51.000000 dependencyhealth-0.0.1/src/dependencyhealth/npm/__init__.py
--rw-r--r--   0 algo       (501) staff       (20)      249 2023-07-14 14:33:44.000000 dependencyhealth-0.0.1/src/dependencyhealth/npm/client.py
-drwxr-xr-x   0 algo       (501) staff       (20)        0 2023-07-14 14:49:02.757013 dependencyhealth-0.0.1/src/dependencyhealth.egg-info/
--rw-r--r--   0 algo       (501) staff       (20)     1140 2023-07-14 14:49:02.000000 dependencyhealth-0.0.1/src/dependencyhealth.egg-info/PKG-INFO
--rw-r--r--   0 algo       (501) staff       (20)      396 2023-07-14 14:49:02.000000 dependencyhealth-0.0.1/src/dependencyhealth.egg-info/SOURCES.txt
--rw-r--r--   0 algo       (501) staff       (20)        1 2023-07-14 14:49:02.000000 dependencyhealth-0.0.1/src/dependencyhealth.egg-info/dependency_links.txt
--rw-r--r--   0 algo       (501) staff       (20)        9 2023-07-14 14:49:02.000000 dependencyhealth-0.0.1/src/dependencyhealth.egg-info/requires.txt
--rw-r--r--   0 algo       (501) staff       (20)       17 2023-07-14 14:49:02.000000 dependencyhealth-0.0.1/src/dependencyhealth.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:19:44.294652 dependencyhealth-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-14 16:19:34.000000 dependencyhealth-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-14 16:19:44.294652 dependencyhealth-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-14 16:19:34.000000 dependencyhealth-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-14 16:19:34.000000 dependencyhealth-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 16:19:44.294652 dependencyhealth-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:19:44.294652 dependencyhealth-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:19:44.294652 dependencyhealth-0.0.2/src/dependencyhealth/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-14 16:19:34.000000 dependencyhealth-0.0.2/src/dependencyhealth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-14 16:19:34.000000 dependencyhealth-0.0.2/src/dependencyhealth/abstract_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:19:44.294652 dependencyhealth-0.0.2/src/dependencyhealth/npm/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-14 16:19:34.000000 dependencyhealth-0.0.2/src/dependencyhealth/npm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-14 16:19:34.000000 dependencyhealth-0.0.2/src/dependencyhealth/npm/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:19:44.294652 dependencyhealth-0.0.2/src/dependencyhealth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-14 16:19:44.000000 dependencyhealth-0.0.2/src/dependencyhealth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-14 16:19:44.000000 dependencyhealth-0.0.2/src/dependencyhealth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:19:44.000000 dependencyhealth-0.0.2/src/dependencyhealth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 16:19:44.000000 dependencyhealth-0.0.2/src/dependencyhealth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 16:19:44.000000 dependencyhealth-0.0.2/src/dependencyhealth.egg-info/top_level.txt
```

### Comparing `dependencyhealth-0.0.1/LICENSE` & `dependencyhealth-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dependencyhealth-0.0.1/PKG-INFO` & `dependencyhealth-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dependencyhealth
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python Client Library for Dependency Health API
 Author: Alex Goncharov
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `dependencyhealth-0.0.1/README.md` & `dependencyhealth-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dependencyhealth-0.0.1/src/dependencyhealth/abstract_client.py` & `dependencyhealth-0.0.2/src/dependencyhealth/abstract_client.py`

 * *Files identical despite different names*

### Comparing `dependencyhealth-0.0.1/src/dependencyhealth.egg-info/PKG-INFO` & `dependencyhealth-0.0.2/src/dependencyhealth.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dependencyhealth
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python Client Library for Dependency Health API
 Author: Alex Goncharov
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

