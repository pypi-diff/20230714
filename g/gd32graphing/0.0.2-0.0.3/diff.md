# Comparing `tmp/gd32graphing-0.0.2.tar.gz` & `tmp/gd32graphing-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gd32graphing-0.0.2.tar", last modified: Fri Jul 14 13:04:31 2023, max compression
+gzip compressed data, was "gd32graphing-0.0.3.tar", last modified: Fri Jul 14 13:13:03 2023, max compression
```

## Comparing `gd32graphing-0.0.2.tar` & `gd32graphing-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 13:04:31.666185 gd32graphing-0.0.2/
--rw-rw-rw-   0        0        0      270 2023-07-14 13:04:31.664145 gd32graphing-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-14 13:04:31.662134 gd32graphing-0.0.2/gd32graphing.egg-info/
--rw-rw-rw-   0        0        0      270 2023-07-14 13:04:31.000000 gd32graphing-0.0.2/gd32graphing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      152 2023-07-14 13:04:31.000000 gd32graphing-0.0.2/gd32graphing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 13:04:31.000000 gd32graphing-0.0.2/gd32graphing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 13:04:31.000000 gd32graphing-0.0.2/gd32graphing.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 13:04:31.666185 gd32graphing-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      432 2023-07-14 12:38:19.000000 gd32graphing-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 13:13:03.353081 gd32graphing-0.0.3/
+-rw-rw-rw-   0        0        0      270 2023-07-14 13:13:03.352010 gd32graphing-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-14 13:13:03.339790 gd32graphing-0.0.3/gd32graphing/
+-rw-rw-rw-   0        0        0        0 2023-07-13 11:25:47.000000 gd32graphing-0.0.3/gd32graphing/__init__.py
+-rw-rw-rw-   0        0        0    21523 2023-07-13 11:39:30.000000 gd32graphing-0.0.3/gd32graphing/graphing.py
+drwxrwxrwx   0        0        0        0 2023-07-14 13:13:03.349791 gd32graphing-0.0.3/gd32graphing.egg-info/
+-rw-rw-rw-   0        0        0      270 2023-07-14 13:13:03.000000 gd32graphing-0.0.3/gd32graphing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-07-14 13:13:03.000000 gd32graphing-0.0.3/gd32graphing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 13:13:03.000000 gd32graphing-0.0.3/gd32graphing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-14 13:13:03.000000 gd32graphing-0.0.3/gd32graphing.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 13:13:03.353081 gd32graphing-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      432 2023-07-14 13:12:54.000000 gd32graphing-0.0.3/setup.py
```

