# Comparing `tmp/simple_ts-0.4.tar.gz` & `tmp/simple_ts-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_ts-0.4.tar", last modified: Fri Jul 14 03:52:56 2023, max compression
+gzip compressed data, was "simple_ts-0.5.tar", last modified: Fri Jul 14 04:05:06 2023, max compression
```

## Comparing `simple_ts-0.4.tar` & `simple_ts-0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 03:52:56.111887 simple_ts-0.4/
--rw-rw-rw-   0        0        0      125 2023-07-14 03:52:56.111887 simple_ts-0.4/PKG-INFO
--rw-rw-rw-   0        0        0      655 2023-07-14 03:15:08.000000 simple_ts-0.4/README.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 03:52:56.111887 simple_ts-0.4/setup.cfg
--rw-rw-rw-   0        0        0      262 2023-07-14 03:52:38.000000 simple_ts-0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:52:56.104868 simple_ts-0.4/simple_ts.egg-info/
--rw-rw-rw-   0        0        0      125 2023-07-14 03:52:55.000000 simple_ts-0.4/simple_ts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-07-14 03:52:56.000000 simple_ts-0.4/simple_ts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 03:52:55.000000 simple_ts-0.4/simple_ts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-07-14 03:52:55.000000 simple_ts-0.4/simple_ts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-14 03:52:55.000000 simple_ts-0.4/simple_ts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-14 03:52:56.111887 simple_ts-0.4/simplets/
--rw-rw-rw-   0        0        0       32 2023-07-14 03:52:31.000000 simple_ts-0.4/simplets/__init__.py
--rw-rw-rw-   0        0        0     2860 2023-07-14 03:42:27.000000 simple_ts-0.4/simplets/simplets.py
+drwxrwxrwx   0        0        0        0 2023-07-14 04:05:06.769194 simple_ts-0.5/
+-rw-rw-rw-   0        0        0      125 2023-07-14 04:05:06.769194 simple_ts-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      655 2023-07-14 03:15:08.000000 simple_ts-0.5/README.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 04:05:06.769194 simple_ts-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      262 2023-07-14 04:04:56.000000 simple_ts-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 04:05:06.753557 simple_ts-0.5/simple_ts.egg-info/
+-rw-rw-rw-   0        0        0      125 2023-07-14 04:05:06.000000 simple_ts-0.5/simple_ts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-07-14 04:05:06.000000 simple_ts-0.5/simple_ts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 04:05:06.000000 simple_ts-0.5/simple_ts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-14 04:05:06.000000 simple_ts-0.5/simple_ts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-14 04:05:06.000000 simple_ts-0.5/simple_ts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 04:05:06.769194 simple_ts-0.5/simplets/
+-rw-rw-rw-   0        0        0       35 2023-07-14 04:04:35.000000 simple_ts-0.5/simplets/__init__.py
+-rw-rw-rw-   0        0        0     2860 2023-07-14 03:42:27.000000 simple_ts-0.5/simplets/simplets.py
```

### Comparing `simple_ts-0.4/README.txt` & `simple_ts-0.5/README.txt`

 * *Files identical despite different names*

### Comparing `simple_ts-0.4/simplets/simplets.py` & `simple_ts-0.5/simplets/simplets.py`

 * *Files identical despite different names*

