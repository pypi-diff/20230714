# Comparing `tmp/trycortex-1.0.4.tar.gz` & `tmp/trycortex-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trycortex-1.0.4.tar", max compression
+gzip compressed data, was "trycortex-1.0.5.tar", max compression
```

## Comparing `trycortex-1.0.4.tar` & `trycortex-1.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       57 2023-07-13 22:45:36.236046 trycortex-1.0.4/README.md
--rw-r--r--   0        0        0      406 2023-07-13 23:07:12.968586 trycortex-1.0.4/pyproject.toml
--rw-r--r--   0        0        0       90 2023-07-13 21:47:58.631841 trycortex-1.0.4/trycortex/__init__.py
--rw-r--r--   0        0        0    12976 2023-07-13 21:48:07.353240 trycortex-1.0.4/trycortex/api.py
--rw-r--r--   0        0        0        0 2023-07-13 23:06:56.199856 trycortex-1.0.4/trycortex/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 23:06:53.816915 trycortex-1.0.4/trycortex/cli/callable/__init__.py
--rw-r--r--   0        0        0      204 2023-07-13 23:06:52.759994 trycortex-1.0.4/trycortex/cli/callable/commands.py
--rw-r--r--   0        0        0      308 2023-07-13 23:06:51.108222 trycortex-1.0.4/trycortex/cli/cli.py
--rw-r--r--   0        0        0      405 1970-01-01 00:00:00.000000 trycortex-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0       57 2023-07-13 22:45:36.236046 trycortex-1.0.5/README.md
+-rw-r--r--   0        0        0      409 2023-07-13 23:10:02.080965 trycortex-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0       90 2023-07-13 21:47:58.631841 trycortex-1.0.5/trycortex/__init__.py
+-rw-r--r--   0        0        0    12976 2023-07-13 21:48:07.353240 trycortex-1.0.5/trycortex/api.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:06:56.199856 trycortex-1.0.5/trycortex/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:06:53.816915 trycortex-1.0.5/trycortex/cli/callable/__init__.py
+-rw-r--r--   0        0        0      204 2023-07-13 23:06:52.759994 trycortex-1.0.5/trycortex/cli/callable/commands.py
+-rw-r--r--   0        0        0      308 2023-07-13 23:09:13.654204 trycortex-1.0.5/trycortex/cli/cli.py
+-rw-r--r--   0        0        0      405 1970-01-01 00:00:00.000000 trycortex-1.0.5/PKG-INFO
```

### Comparing `trycortex-1.0.4/trycortex/api.py` & `trycortex-1.0.5/trycortex/api.py`

 * *Files identical despite different names*

