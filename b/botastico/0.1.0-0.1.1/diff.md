# Comparing `tmp/botastico-0.1.0.tar.gz` & `tmp/botastico-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botastico-0.1.0.tar", max compression
+gzip compressed data, was "botastico-0.1.1.tar", max compression
```

## Comparing `botastico-0.1.0.tar` & `botastico-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       18 2023-07-13 14:16:03.034135 botastico-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-13 12:47:16.893653 botastico-0.1.0/botastico/__init__.py
--rw-r--r--   0        0        0     5718 2023-07-14 05:26:26.560273 botastico-0.1.0/botastico/langchain.py
--rw-r--r--   0        0        0      465 2023-07-13 14:17:51.383033 botastico-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      441 1970-01-01 00:00:00.000000 botastico-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2447 2023-07-14 06:27:49.591714 botastico-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 12:47:16.893653 botastico-0.1.1/botastico/__init__.py
+-rw-r--r--   0        0        0     5718 2023-07-14 05:26:26.560273 botastico-0.1.1/botastico/langchain.py
+-rw-r--r--   0        0        0      465 2023-07-14 06:34:18.969053 botastico-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2870 1970-01-01 00:00:00.000000 botastico-0.1.1/PKG-INFO
```

### Comparing `botastico-0.1.0/botastico/langchain.py` & `botastico-0.1.1/botastico/langchain.py`

 * *Files identical despite different names*

