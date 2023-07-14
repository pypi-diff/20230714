# Comparing `tmp/uta-gms-engine-0.0.2.tar.gz` & `tmp/uta-gms-engine-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uta-gms-engine-0.0.2.tar", last modified: Thu Jul 13 21:09:14 2023, max compression
+gzip compressed data, was "uta-gms-engine-0.0.5.tar", last modified: Fri Jul 14 21:52:48 2023, max compression
```

## Comparing `uta-gms-engine-0.0.2.tar` & `uta-gms-engine-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:09:14.139255 uta-gms-engine-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-13 21:09:14.139255 uta-gms-engine-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-13 21:09:05.000000 uta-gms-engine-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-13 21:09:05.000000 uta-gms-engine-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-13 21:09:14.143255 uta-gms-engine-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:09:14.139255 uta-gms-engine-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:09:14.139255 uta-gms-engine-0.0.2/src/uta_gms_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-13 21:09:14.000000 uta-gms-engine-0.0.2/src/uta_gms_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-13 21:09:14.000000 uta-gms-engine-0.0.2/src/uta_gms_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 21:09:14.000000 uta-gms-engine-0.0.2/src/uta_gms_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-13 21:09:14.000000 uta-gms-engine-0.0.2/src/uta_gms_engine.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 21:09:14.139255 uta-gms-engine-0.0.2/src/utagms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 21:09:05.000000 uta-gms-engine-0.0.2/src/utagms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-13 21:09:05.000000 uta-gms-engine-0.0.2/src/utagms/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:52:48.702474 uta-gms-engine-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-14 21:52:48.702474 uta-gms-engine-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-14 21:52:35.000000 uta-gms-engine-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-14 21:52:35.000000 uta-gms-engine-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-14 21:52:48.702474 uta-gms-engine-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:52:48.698474 uta-gms-engine-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:52:48.702474 uta-gms-engine-0.0.5/src/uta_gms_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-14 21:52:48.000000 uta-gms-engine-0.0.5/src/uta_gms_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-14 21:52:48.000000 uta-gms-engine-0.0.5/src/uta_gms_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 21:52:48.000000 uta-gms-engine-0.0.5/src/uta_gms_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-14 21:52:48.000000 uta-gms-engine-0.0.5/src/uta_gms_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 21:52:48.000000 uta-gms-engine-0.0.5/src/uta_gms_engine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:52:48.702474 uta-gms-engine-0.0.5/src/utagms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 21:52:35.000000 uta-gms-engine-0.0.5/src/utagms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-14 21:52:35.000000 uta-gms-engine-0.0.5/src/utagms/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-14 21:52:35.000000 uta-gms-engine-0.0.5/src/utagms/solver.py
```

