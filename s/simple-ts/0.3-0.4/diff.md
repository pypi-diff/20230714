# Comparing `tmp/simple_ts-0.3.tar.gz` & `tmp/simple_ts-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_ts-0.3.tar", last modified: Fri Jul 14 03:42:46 2023, max compression
+gzip compressed data, was "simple_ts-0.4.tar", last modified: Fri Jul 14 03:52:56 2023, max compression
```

## Comparing `simple_ts-0.3.tar` & `simple_ts-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 03:42:46.553400 simple_ts-0.3/
--rw-rw-rw-   0        0        0      125 2023-07-14 03:42:46.553400 simple_ts-0.3/PKG-INFO
--rw-rw-rw-   0        0        0      655 2023-07-14 03:15:08.000000 simple_ts-0.3/README.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 03:42:46.553400 simple_ts-0.3/setup.cfg
--rw-rw-rw-   0        0        0      262 2023-07-14 03:42:38.000000 simple_ts-0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:42:46.553400 simple_ts-0.3/simple_ts.egg-info/
--rw-rw-rw-   0        0        0      125 2023-07-14 03:42:46.000000 simple_ts-0.3/simple_ts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-07-14 03:42:46.000000 simple_ts-0.3/simple_ts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 03:42:46.000000 simple_ts-0.3/simple_ts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-07-14 03:42:46.000000 simple_ts-0.3/simple_ts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-14 03:42:46.000000 simple_ts-0.3/simple_ts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-14 03:42:46.553400 simple_ts-0.3/simplets/
--rw-rw-rw-   0        0        0        0 2023-07-14 02:35:40.000000 simple_ts-0.3/simplets/__init__.py
--rw-rw-rw-   0        0        0     2860 2023-07-14 03:42:27.000000 simple_ts-0.3/simplets/simplets.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:52:56.111887 simple_ts-0.4/
+-rw-rw-rw-   0        0        0      125 2023-07-14 03:52:56.111887 simple_ts-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      655 2023-07-14 03:15:08.000000 simple_ts-0.4/README.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 03:52:56.111887 simple_ts-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      262 2023-07-14 03:52:38.000000 simple_ts-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:52:56.104868 simple_ts-0.4/simple_ts.egg-info/
+-rw-rw-rw-   0        0        0      125 2023-07-14 03:52:55.000000 simple_ts-0.4/simple_ts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-07-14 03:52:56.000000 simple_ts-0.4/simple_ts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 03:52:55.000000 simple_ts-0.4/simple_ts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-14 03:52:55.000000 simple_ts-0.4/simple_ts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-14 03:52:55.000000 simple_ts-0.4/simple_ts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 03:52:56.111887 simple_ts-0.4/simplets/
+-rw-rw-rw-   0        0        0       32 2023-07-14 03:52:31.000000 simple_ts-0.4/simplets/__init__.py
+-rw-rw-rw-   0        0        0     2860 2023-07-14 03:42:27.000000 simple_ts-0.4/simplets/simplets.py
```

### Comparing `simple_ts-0.3/README.txt` & `simple_ts-0.4/README.txt`

 * *Files identical despite different names*

### Comparing `simple_ts-0.3/simplets/simplets.py` & `simple_ts-0.4/simplets/simplets.py`

 * *Files identical despite different names*

