# Comparing `tmp/for-testing-48.0.0.tar.gz` & `tmp/for-testing-48.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/demo/demo/dist/.tmp-zw7bunkw/for-testing-48.0.0.tar", last modified: Fri Jul 14 17:18:30 2023, max compression
+gzip compressed data, was "/home/runner/work/demo/demo/dist/.tmp-93iiv5p9/for-testing-48.0.1.tar", last modified: Fri Jul 14 17:29:48 2023, max compression
```

## Comparing `for-testing-48.0.0.tar` & `for-testing-48.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:18:30.000000 for-testing-48.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-14 17:18:30.000000 for-testing-48.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-14 17:18:22.000000 for-testing-48.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:18:30.000000 for-testing-48.0.0/for_testing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-14 17:18:30.000000 for-testing-48.0.0/for_testing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-14 17:18:30.000000 for-testing-48.0.0/for_testing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:18:30.000000 for-testing-48.0.0/for_testing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 17:18:30.000000 for-testing-48.0.0/for_testing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 17:18:30.000000 for-testing-48.0.0/for_testing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-14 17:18:22.000000 for-testing-48.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 17:18:30.000000 for-testing-48.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:29:48.000000 for-testing-48.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-14 17:29:48.000000 for-testing-48.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-14 17:29:40.000000 for-testing-48.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:29:48.000000 for-testing-48.0.1/for_testing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-14 17:29:48.000000 for-testing-48.0.1/for_testing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-14 17:29:48.000000 for-testing-48.0.1/for_testing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:29:48.000000 for-testing-48.0.1/for_testing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 17:29:48.000000 for-testing-48.0.1/for_testing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 17:29:48.000000 for-testing-48.0.1/for_testing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-14 17:29:40.000000 for-testing-48.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 17:29:48.000000 for-testing-48.0.1/setup.cfg
```

### Comparing `for-testing-48.0.0/pyproject.toml` & `for-testing-48.0.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "for-testing"
-version = "48.0.0"
+version = "48.0.1"
 description = "foo"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
   	{email = "ascacascascdac@acacascaiuvbasceav.ascaeavav"},
 ]
```

