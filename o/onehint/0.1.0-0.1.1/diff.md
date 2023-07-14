# Comparing `tmp/onehint-0.1.0.tar.gz` & `tmp/onehint-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onehint-0.1.0.tar", max compression
+gzip compressed data, was "onehint-0.1.1.tar", max compression
```

## Comparing `onehint-0.1.0.tar` & `onehint-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2022-07-13 14:13:28.362670 onehint-0.1.0/README.md
--rw-r--r--   0        0        0        0 2022-07-13 14:13:28.362557 onehint-0.1.0/onehint/__init__.py
--rw-r--r--   0        0        0      259 2022-07-13 14:13:28.367178 onehint-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      491 1970-01-01 00:00:00.000000 onehint-0.1.0/setup.py
--rw-r--r--   0        0        0      428 1970-01-01 00:00:00.000000 onehint-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-07-13 14:13:28.362670 onehint-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2022-07-13 14:13:28.362557 onehint-0.1.1/onehint/__init__.py
+-rw-r--r--   0        0        0      259 2023-07-14 19:59:20.088838 onehint-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      491 1970-01-01 00:00:00.000000 onehint-0.1.1/setup.py
+-rw-r--r--   0        0        0      479 1970-01-01 00:00:00.000000 onehint-0.1.1/PKG-INFO
```

