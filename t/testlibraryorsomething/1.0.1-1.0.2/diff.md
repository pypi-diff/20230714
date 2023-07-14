# Comparing `tmp/testlibraryorsomething-1.0.1.tar.gz` & `tmp/testlibraryorsomething-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testlibraryorsomething-1.0.1.tar", last modified: Fri Jul 14 14:44:50 2023, max compression
+gzip compressed data, was "testlibraryorsomething-1.0.2.tar", last modified: Fri Jul 14 15:09:08 2023, max compression
```

## Comparing `testlibraryorsomething-1.0.1.tar` & `testlibraryorsomething-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 14:44:50.972551 testlibraryorsomething-1.0.1/
--rw-rw-rw-   0        0        0      159 2023-07-14 14:44:50.972551 testlibraryorsomething-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-14 14:44:50.973551 testlibraryorsomething-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      711 2023-07-14 14:44:21.000000 testlibraryorsomething-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-14 14:44:50.960399 testlibraryorsomething-1.0.1/testlibraryorsomething/
--rw-rw-rw-   0        0        0      104 2023-07-14 14:44:40.000000 testlibraryorsomething-1.0.1/testlibraryorsomething/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 14:44:50.970584 testlibraryorsomething-1.0.1/testlibraryorsomething.egg-info/
--rw-rw-rw-   0        0        0      159 2023-07-14 14:44:50.000000 testlibraryorsomething-1.0.1/testlibraryorsomething.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-07-14 14:44:50.000000 testlibraryorsomething-1.0.1/testlibraryorsomething.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 14:44:50.000000 testlibraryorsomething-1.0.1/testlibraryorsomething.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2023-07-14 14:44:50.000000 testlibraryorsomething-1.0.1/testlibraryorsomething.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       23 2023-07-14 14:44:50.000000 testlibraryorsomething-1.0.1/testlibraryorsomething.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 15:09:08.448779 testlibraryorsomething-1.0.2/
+-rw-rw-rw-   0        0        0      159 2023-07-14 15:09:08.448779 testlibraryorsomething-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-14 15:09:08.448779 testlibraryorsomething-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      254 2023-07-14 15:02:31.000000 testlibraryorsomething-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:09:08.439786 testlibraryorsomething-1.0.2/testlibraryorsomething/
+-rw-rw-rw-   0        0        0      211 2023-07-14 15:08:47.000000 testlibraryorsomething-1.0.2/testlibraryorsomething/__init__.py
+-rw-rw-rw-   0        0        0       45 2023-07-14 15:06:18.000000 testlibraryorsomething-1.0.2/testlibraryorsomething/test_functionality.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:09:08.446779 testlibraryorsomething-1.0.2/testlibraryorsomething.egg-info/
+-rw-rw-rw-   0        0        0      159 2023-07-14 15:09:08.000000 testlibraryorsomething-1.0.2/testlibraryorsomething.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-07-14 15:09:08.000000 testlibraryorsomething-1.0.2/testlibraryorsomething.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 15:09:08.000000 testlibraryorsomething-1.0.2/testlibraryorsomething.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-07-14 15:09:08.000000 testlibraryorsomething-1.0.2/testlibraryorsomething.egg-info/top_level.txt
```

