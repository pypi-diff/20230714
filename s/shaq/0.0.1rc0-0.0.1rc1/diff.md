# Comparing `tmp/shaq-0.0.1rc0.tar.gz` & `tmp/shaq-0.0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shaq-0.0.1rc0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "shaq-0.0.1rc1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `shaq-0.0.1rc0.tar` & `shaq-0.0.1rc1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1109 2023-07-14 00:57:50.775200 shaq-0.0.1rc0/LICENSE
--rw-r--r--   0        0        0     1099 2023-07-14 00:57:50.775200 shaq-0.0.1rc0/README.md
--rw-r--r--   0        0        0     1664 2023-07-14 00:57:50.775200 shaq-0.0.1rc0/pyproject.toml
--rw-r--r--   0        0        0       25 2023-07-14 00:57:50.775200 shaq-0.0.1rc0/shaq/__init__.py
--rw-r--r--   0        0        0       70 2023-07-14 00:57:50.775200 shaq-0.0.1rc0/shaq/__main__.py
--rw-r--r--   0        0        0     5759 2023-07-14 00:57:50.775200 shaq-0.0.1rc0/shaq/_cli.py
--rw-r--r--   0        0        0     2360 1970-01-01 00:00:00.000000 shaq-0.0.1rc0/PKG-INFO
+-rw-r--r--   0        0        0     1109 2023-07-14 01:07:46.706841 shaq-0.0.1rc1/LICENSE
+-rw-r--r--   0        0        0     1322 2023-07-14 01:07:46.706841 shaq-0.0.1rc1/README.md
+-rw-r--r--   0        0        0     1664 2023-07-14 01:07:46.706841 shaq-0.0.1rc1/pyproject.toml
+-rw-r--r--   0        0        0       25 2023-07-14 01:07:46.706841 shaq-0.0.1rc1/shaq/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-14 01:07:46.706841 shaq-0.0.1rc1/shaq/__main__.py
+-rw-r--r--   0        0        0     5759 2023-07-14 01:07:46.706841 shaq-0.0.1rc1/shaq/_cli.py
+-rw-r--r--   0        0        0     2583 1970-01-01 00:00:00.000000 shaq-0.0.1rc1/PKG-INFO
```

### Comparing `shaq-0.0.1rc0/LICENSE` & `shaq-0.0.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `shaq-0.0.1rc0/README.md` & `shaq-0.0.1rc1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # shaq
 
+[![CI](https://github.com/woodruffw/shaq/actions/workflows/ci.yml/badge.svg)](https://github.com/woodruffw/shaq/actions/workflows/ci.yml)
+[![PyPI version](https://badge.fury.io/py/shaq.svg)](https://badge.fury.io/py/shaq)
+
 A bare-bones CLI client for [Shazam](https://www.shazam.com/home).
 
-![shaq in action](https://github.com/woodruffw/shaq/assets/3059210/9bf22a57-2c7b-48d8-9707-f3d7f9d9a2f4)
+![shaq in action](https://github.com/woodruffw/shaq/assets/3059210/3ee02414-b1c0-4379-8c9d-cb646dba9902)
 
 ## Installation
 
 `shaq` is available via `pip` or `pipx`:
 
 ```bash
 pip install shaq
```

### Comparing `shaq-0.0.1rc0/pyproject.toml` & `shaq-0.0.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `shaq-0.0.1rc0/shaq/_cli.py` & `shaq-0.0.1rc1/shaq/_cli.py`

 * *Files identical despite different names*

### Comparing `shaq-0.0.1rc0/PKG-INFO` & `shaq-0.0.1rc1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaq
-Version: 0.0.1rc0
+Version: 0.0.1rc1
 Summary: A bare-bones Shazam CLI client
 Author-email: William Woodruff <william@yossarian.net>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
@@ -29,17 +29,20 @@
 Project-URL: Source, https://github.com/woodruffw/shaq
 Provides-Extra: dev
 Provides-Extra: lint
 Provides-Extra: test
 
 # shaq
 
+[![CI](https://github.com/woodruffw/shaq/actions/workflows/ci.yml/badge.svg)](https://github.com/woodruffw/shaq/actions/workflows/ci.yml)
+[![PyPI version](https://badge.fury.io/py/shaq.svg)](https://badge.fury.io/py/shaq)
+
 A bare-bones CLI client for [Shazam](https://www.shazam.com/home).
 
-![shaq in action](https://github.com/woodruffw/shaq/assets/3059210/9bf22a57-2c7b-48d8-9707-f3d7f9d9a2f4)
+![shaq in action](https://github.com/woodruffw/shaq/assets/3059210/3ee02414-b1c0-4379-8c9d-cb646dba9902)
 
 ## Installation
 
 `shaq` is available via `pip` or `pipx`:
 
 ```bash
 pip install shaq
```

