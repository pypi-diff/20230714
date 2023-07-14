# Comparing `tmp/for-testing-47.10.300b31.tar.gz` & `tmp/for-testing-47.11.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/demo/demo/dist/.tmp-2cal3ybd/for-testing-47.10.300b31.tar", last modified: Fri Jul 14 17:06:23 2023, max compression
+gzip compressed data, was "/home/runner/work/demo/demo/dist/.tmp-p8fwj5m5/for-testing-47.11.0b0.tar", last modified: Fri Jul 14 13:28:57 2023, max compression
```

## Comparing `for-testing-47.10.300b31.tar` & `for-testing-47.11.0b0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:06:23.000000 for-testing-47.10.300b31/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-14 17:06:23.000000 for-testing-47.10.300b31/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-14 17:06:16.000000 for-testing-47.10.300b31/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:06:23.000000 for-testing-47.10.300b31/for_testing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-14 17:06:23.000000 for-testing-47.10.300b31/for_testing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-14 17:06:23.000000 for-testing-47.10.300b31/for_testing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:06:23.000000 for-testing-47.10.300b31/for_testing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 17:06:23.000000 for-testing-47.10.300b31/for_testing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 17:06:23.000000 for-testing-47.10.300b31/for_testing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-14 17:06:17.000000 for-testing-47.10.300b31/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 17:06:23.000000 for-testing-47.10.300b31/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:28:57.000000 for-testing-47.11.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-14 13:28:57.000000 for-testing-47.11.0b0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:28:57.000000 for-testing-47.11.0b0/for_testing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-14 13:28:57.000000 for-testing-47.11.0b0/for_testing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-14 13:28:57.000000 for-testing-47.11.0b0/for_testing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 13:28:57.000000 for-testing-47.11.0b0/for_testing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 13:28:57.000000 for-testing-47.11.0b0/for_testing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 13:28:57.000000 for-testing-47.11.0b0/for_testing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-14 13:28:49.000000 for-testing-47.11.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 13:28:57.000000 for-testing-47.11.0b0/setup.cfg
```

### Comparing `for-testing-47.10.300b31/pyproject.toml` & `for-testing-47.11.0b0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "for-testing"
-version = "47.10.300b31"
+version = "47.11.0b"
 description = "foo"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
   	{email = "ascacascascdac@acacascaiuvbasceav.ascaeavav"},
 ]
```

