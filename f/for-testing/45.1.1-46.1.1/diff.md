# Comparing `tmp/for-testing-45.1.1.tar.gz` & `tmp/for-testing-46.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/demo/demo/dist/.tmp-rv3fcmkv/for-testing-45.1.1.tar", last modified: Thu Jul 13 14:36:07 2023, max compression
+gzip compressed data, was "/home/runner/work/demo/demo/dist/.tmp-eutm88nz/for-testing-46.1.1.tar", last modified: Thu Jul 13 15:58:51 2023, max compression
```

## Comparing `for-testing-45.1.1.tar` & `for-testing-46.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:36:07.000000 for-testing-45.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-13 14:36:07.000000 for-testing-45.1.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:36:07.000000 for-testing-45.1.1/for_testing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-13 14:36:07.000000 for-testing-45.1.1/for_testing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-13 14:36:07.000000 for-testing-45.1.1/for_testing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 14:36:07.000000 for-testing-45.1.1/for_testing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 14:36:07.000000 for-testing-45.1.1/for_testing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 14:36:07.000000 for-testing-45.1.1/for_testing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-13 14:36:00.000000 for-testing-45.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 14:36:07.000000 for-testing-45.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:58:51.000000 for-testing-46.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-13 15:58:51.000000 for-testing-46.1.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:58:51.000000 for-testing-46.1.1/for_testing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-13 15:58:51.000000 for-testing-46.1.1/for_testing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-13 15:58:51.000000 for-testing-46.1.1/for_testing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 15:58:51.000000 for-testing-46.1.1/for_testing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 15:58:51.000000 for-testing-46.1.1/for_testing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 15:58:51.000000 for-testing-46.1.1/for_testing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-13 15:58:44.000000 for-testing-46.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 15:58:51.000000 for-testing-46.1.1/setup.cfg
```

### Comparing `for-testing-45.1.1/pyproject.toml` & `for-testing-46.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "for-testing"
-version = "45.1.1"
+version = "46.1.1"
 description = "foo"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
   	{email = "ascacascascdac@acacascaiuvbasceav.ascaeavav"},
 ]
```

