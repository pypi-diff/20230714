# Comparing `tmp/neonelly.core-0.0.4.tar.gz` & `tmp/neonelly.core-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neonelly.core-0.0.4.tar", last modified: Fri Jul 14 05:32:33 2023, max compression
+gzip compressed data, was "neonelly.core-0.0.5.tar", last modified: Fri Jul 14 05:34:50 2023, max compression
```

## Comparing `neonelly.core-0.0.4.tar` & `neonelly.core-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:32:33.079691 neonelly.core-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-14 05:32:33.079691 neonelly.core-0.0.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:32:33.079691 neonelly.core-0.0.4/neonelly.core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-14 05:32:33.000000 neonelly.core-0.0.4/neonelly.core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-14 05:32:33.000000 neonelly.core-0.0.4/neonelly.core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 05:32:33.000000 neonelly.core-0.0.4/neonelly.core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 05:32:33.000000 neonelly.core-0.0.4/neonelly.core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 05:32:33.079691 neonelly.core-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-14 05:32:29.000000 neonelly.core-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:34:50.781387 neonelly.core-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-14 05:34:50.781387 neonelly.core-0.0.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:34:50.781387 neonelly.core-0.0.5/neonelly.core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-14 05:34:50.000000 neonelly.core-0.0.5/neonelly.core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-14 05:34:50.000000 neonelly.core-0.0.5/neonelly.core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 05:34:50.000000 neonelly.core-0.0.5/neonelly.core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 05:34:50.000000 neonelly.core-0.0.5/neonelly.core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 05:34:50.781387 neonelly.core-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-14 05:34:47.000000 neonelly.core-0.0.5/setup.py
```

