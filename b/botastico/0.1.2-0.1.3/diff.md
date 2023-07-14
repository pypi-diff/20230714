# Comparing `tmp/botastico-0.1.2.tar.gz` & `tmp/botastico-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botastico-0.1.2.tar", max compression
+gzip compressed data, was "botastico-0.1.3.tar", max compression
```

## Comparing `botastico-0.1.2.tar` & `botastico-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1077 2023-07-14 06:40:48.122486 botastico-0.1.2/LICENSE
--rw-r--r--   0        0        0     2203 2023-07-14 06:36:20.539247 botastico-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-07-13 12:47:16.893653 botastico-0.1.2/botastico/__init__.py
--rw-r--r--   0        0        0     5718 2023-07-14 05:26:26.560273 botastico-0.1.2/botastico/langchain.py
--rw-r--r--   0        0        0      465 2023-07-14 06:41:42.608621 botastico-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2626 1970-01-01 00:00:00.000000 botastico-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-14 06:40:48.122486 botastico-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2203 2023-07-14 06:36:20.539247 botastico-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 12:47:16.893653 botastico-0.1.3/botastico/__init__.py
+-rw-r--r--   0        0        0     5718 2023-07-14 05:26:26.560273 botastico-0.1.3/botastico/langchain.py
+-rw-r--r--   0        0        0      524 2023-07-14 06:47:28.619441 botastico-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2683 1970-01-01 00:00:00.000000 botastico-0.1.3/PKG-INFO
```

### Comparing `botastico-0.1.2/LICENSE` & `botastico-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `botastico-0.1.2/README.md` & `botastico-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `botastico-0.1.2/botastico/langchain.py` & `botastico-0.1.3/botastico/langchain.py`

 * *Files identical despite different names*

### Comparing `botastico-0.1.2/PKG-INFO` & `botastico-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: botastico
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python SDK for using the botasti.co chat API
+Home-page: https://github.com/botastico/botastico-python
 Author: Andres Kull
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: langchain (>=0.0.231,<0.0.232)
```

