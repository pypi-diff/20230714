# Comparing `tmp/simple_ts-0.1.tar.gz` & `tmp/simple_ts-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_ts-0.1.tar", last modified: Fri Jul 14 03:06:43 2023, max compression
+gzip compressed data, was "simple_ts-0.2.tar", last modified: Fri Jul 14 03:17:31 2023, max compression
```

## Comparing `simple_ts-0.1.tar` & `simple_ts-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 03:06:43.906380 simple_ts-0.1/
--rw-rw-rw-   0        0        0      125 2023-07-14 03:06:43.906380 simple_ts-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      655 2023-07-14 03:06:27.000000 simple_ts-0.1/README.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 03:06:43.906380 simple_ts-0.1/setup.cfg
--rw-rw-rw-   0        0        0      264 2023-07-14 03:06:25.000000 simple_ts-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:06:43.893197 simple_ts-0.1/simple_ts.egg-info/
--rw-rw-rw-   0        0        0      125 2023-07-14 03:06:43.000000 simple_ts-0.1/simple_ts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-07-14 03:06:43.000000 simple_ts-0.1/simple_ts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 03:06:43.000000 simple_ts-0.1/simple_ts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-07-14 03:06:43.000000 simple_ts-0.1/simple_ts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-14 03:06:43.000000 simple_ts-0.1/simple_ts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-14 03:06:43.901862 simple_ts-0.1/simplets/
--rw-rw-rw-   0        0        0        0 2023-07-14 02:35:40.000000 simple_ts-0.1/simplets/__init__.py
--rw-rw-rw-   0        0        0     2871 2023-07-14 02:39:24.000000 simple_ts-0.1/simplets/simplets.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:17:31.305736 simple_ts-0.2/
+-rw-rw-rw-   0        0        0      125 2023-07-14 03:17:31.305736 simple_ts-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      655 2023-07-14 03:15:08.000000 simple_ts-0.2/README.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 03:17:31.305736 simple_ts-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      262 2023-07-14 03:15:07.000000 simple_ts-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:17:31.302672 simple_ts-0.2/simple_ts.egg-info/
+-rw-rw-rw-   0        0        0      125 2023-07-14 03:17:31.000000 simple_ts-0.2/simple_ts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-07-14 03:17:31.000000 simple_ts-0.2/simple_ts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 03:17:31.000000 simple_ts-0.2/simple_ts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-14 03:17:31.000000 simple_ts-0.2/simple_ts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-14 03:17:31.000000 simple_ts-0.2/simple_ts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 03:17:31.305736 simple_ts-0.2/simplets/
+-rw-rw-rw-   0        0        0        0 2023-07-14 02:35:40.000000 simple_ts-0.2/simplets/__init__.py
+-rw-rw-rw-   0        0        0     2871 2023-07-14 02:39:24.000000 simple_ts-0.2/simplets/simplets.py
```

### Comparing `simple_ts-0.1/README.txt` & `simple_ts-0.2/README.txt`

 * *Files identical despite different names*

### Comparing `simple_ts-0.1/simplets/simplets.py` & `simple_ts-0.2/simplets/simplets.py`

 * *Files identical despite different names*

