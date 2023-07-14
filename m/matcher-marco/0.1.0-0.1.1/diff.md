# Comparing `tmp/matcher_marco-0.1.0.tar.gz` & `tmp/matcher_marco-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matcher_marco-0.1.0.tar", max compression
+gzip compressed data, was "matcher_marco-0.1.1.tar", max compression
```

## Comparing `matcher_marco-0.1.0.tar` & `matcher_marco-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-07-14 11:06:41.156973 matcher_marco-0.1.0/matcher_marco/__init__.py
--rw-r--r--   0        0        0      481 2023-07-14 11:10:47.802547 matcher_marco-0.1.0/matcher_marco/matcher.py
--rw-r--r--   0        0        0      348 2023-07-14 11:12:46.412337 matcher_marco-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-14 11:06:41.156973 matcher_marco-0.1.0/README.md
--rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 matcher_marco-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       36 2023-07-14 11:22:19.505424 matcher_marco-0.1.1/matcher_marco/__init__.py
+-rw-r--r--   0        0        0      481 2023-07-14 11:10:47.802547 matcher_marco-0.1.1/matcher_marco/matcher.py
+-rw-r--r--   0        0        0      348 2023-07-14 11:23:30.167014 matcher_marco-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-14 11:06:41.156973 matcher_marco-0.1.1/README.md
+-rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 matcher_marco-0.1.1/PKG-INFO
```

