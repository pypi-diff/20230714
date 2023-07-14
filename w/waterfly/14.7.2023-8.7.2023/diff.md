# Comparing `tmp/waterfly-14.7.2023.tar.gz` & `tmp/waterfly-8.7.2023.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waterfly-14.7.2023.tar", last modified: Fri Jul 14 18:54:58 2023, max compression
+gzip compressed data, was "waterfly-8.7.2023.tar", last modified: Sat Jul  8 18:40:09 2023, max compression
```

## Comparing `waterfly-14.7.2023.tar` & `waterfly-8.7.2023.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 18:54:58.084597 waterfly-14.7.2023/
--rw-rw-rw-   0        0        0     3798 2023-07-14 18:54:58.068979 waterfly-14.7.2023/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-14 18:54:58.084597 waterfly-14.7.2023/setup.cfg
--rw-rw-rw-   0        0        0     4062 2023-07-14 18:52:18.000000 waterfly-14.7.2023/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-14 18:54:58.037738 waterfly-14.7.2023/waterfly/
--rw-rw-rw-   0        0        0    35140 2023-07-14 18:51:24.000000 waterfly-14.7.2023/waterfly/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 18:54:58.068979 waterfly-14.7.2023/waterfly.egg-info/
--rw-rw-rw-   0        0        0     3798 2023-07-14 18:54:57.000000 waterfly-14.7.2023/waterfly.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-07-14 18:54:57.000000 waterfly-14.7.2023/waterfly.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 18:54:57.000000 waterfly-14.7.2023/waterfly.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-07-14 18:54:57.000000 waterfly-14.7.2023/waterfly.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-14 18:54:57.000000 waterfly-14.7.2023/waterfly.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 18:40:09.640290 waterfly-8.7.2023/
+-rw-rw-rw-   0        0        0     1822 2023-07-08 18:40:09.640290 waterfly-8.7.2023/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-08 18:40:09.640290 waterfly-8.7.2023/setup.cfg
+-rw-rw-rw-   0        0        0     2173 2023-07-08 18:34:35.000000 waterfly-8.7.2023/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 18:40:09.593429 waterfly-8.7.2023/waterfly/
+-rw-rw-rw-   0        0        0     7887 2023-07-08 17:40:07.000000 waterfly-8.7.2023/waterfly/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 18:40:09.640290 waterfly-8.7.2023/waterfly.egg-info/
+-rw-rw-rw-   0        0        0     1822 2023-07-08 18:40:09.000000 waterfly-8.7.2023/waterfly.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-07-08 18:40:09.000000 waterfly-8.7.2023/waterfly.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 18:40:09.000000 waterfly-8.7.2023/waterfly.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-08 18:40:09.000000 waterfly-8.7.2023/waterfly.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-08 18:40:09.000000 waterfly-8.7.2023/waterfly.egg-info/top_level.txt
```

