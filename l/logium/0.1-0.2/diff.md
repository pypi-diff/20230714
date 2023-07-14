# Comparing `tmp/logium-0.1.tar.gz` & `tmp/logium-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logium-0.1.tar", last modified: Mon Jul 10 23:09:27 2023, max compression
+gzip compressed data, was "logium-0.2.tar", last modified: Fri Jul 14 19:24:49 2023, max compression
```

## Comparing `logium-0.1.tar` & `logium-0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 23:09:27.779027 logium-0.1/
--rw-rw-rw-   0        0        0      157 2023-07-10 23:09:27.779027 logium-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-10 23:09:27.717843 logium-0.1/logium/
--rw-rw-rw-   0        0        0     1796 2023-07-10 22:54:07.000000 logium-0.1/logium/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 23:09:27.779027 logium-0.1/logium.egg-info/
--rw-rw-rw-   0        0        0      157 2023-07-10 23:09:27.000000 logium-0.1/logium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      157 2023-07-10 23:09:27.000000 logium-0.1/logium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 23:09:27.000000 logium-0.1/logium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-10 23:09:27.000000 logium-0.1/logium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 23:09:27.787029 logium-0.1/setup.cfg
--rw-rw-rw-   0        0        0      388 2023-07-10 23:09:02.000000 logium-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 19:24:48.998425 logium-0.2/
+-rw-rw-rw-   0        0        0      157 2023-07-14 19:24:48.998425 logium-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-14 19:24:48.946737 logium-0.2/logium/
+-rw-rw-rw-   0        0        0     2785 2023-07-14 19:23:45.000000 logium-0.2/logium/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 19:24:48.998425 logium-0.2/logium.egg-info/
+-rw-rw-rw-   0        0        0      157 2023-07-14 19:24:48.000000 logium-0.2/logium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      157 2023-07-14 19:24:48.000000 logium-0.2/logium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 19:24:48.000000 logium-0.2/logium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-14 19:24:48.000000 logium-0.2/logium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 19:24:49.006434 logium-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      388 2023-07-14 19:24:11.000000 logium-0.2/setup.py
```

