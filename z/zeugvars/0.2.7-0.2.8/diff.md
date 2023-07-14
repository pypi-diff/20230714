# Comparing `tmp/zeugvars-0.2.7.tar.gz` & `tmp/zeugvars-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeugvars-0.2.7.tar", max compression
+gzip compressed data, was "zeugvars-0.2.8.tar", max compression
```

## Comparing `zeugvars-0.2.7.tar` & `zeugvars-0.2.8.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1083 2023-06-29 20:37:00.152930 zeugvars-0.2.7/LICENSE
--rw-r--r--   0        0        0     3450 2023-07-13 23:31:25.624178 zeugvars-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     4160 2023-07-04 18:43:08.544957 zeugvars-0.2.7/README.md
--rw-r--r--   0        0        0     9514 2023-07-13 23:31:16.860583 zeugvars-0.2.7/zeugvars/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 10:15:47.964651 zeugvars-0.2.7/zeugvars/py.typed
--rw-r--r--   0        0        0     4503 1970-01-01 00:00:00.000000 zeugvars-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-06-29 20:37:00.152930 zeugvars-0.2.8/LICENSE
+-rw-r--r--   0        0        0     3326 2023-07-14 00:06:08.183904 zeugvars-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0      118 2023-07-14 00:05:49.722185 zeugvars-0.2.8/README.md
+-rw-r--r--   0        0        0      100 2023-07-14 00:04:38.812308 zeugvars-0.2.8/zeugvars/__init__.py
+-rw-r--r--   0        0        0      576 1970-01-01 00:00:00.000000 zeugvars-0.2.8/PKG-INFO
```

### Comparing `zeugvars-0.2.7/LICENSE` & `zeugvars-0.2.8/LICENSE`

 * *Files identical despite different names*

