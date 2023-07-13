# Comparing `tmp/trycortex-1.0.2.tar.gz` & `tmp/trycortex-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trycortex-1.0.2.tar", max compression
+gzip compressed data, was "trycortex-1.0.3.tar", max compression
```

## Comparing `trycortex-1.0.2.tar` & `trycortex-1.0.3.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0       15 2023-07-06 19:03:30.611452 trycortex-1.0.2/README.md
--rw-r--r--   0        0        0      392 2023-07-13 21:46:43.668428 trycortex-1.0.2/pyproject.toml
--rw-r--r--   0        0        0       87 2023-07-10 22:39:25.965913 trycortex-1.0.2/trycortex/__init__.py
--rw-r--r--   0        0        0    12976 2023-07-10 22:57:38.671868 trycortex-1.0.2/trycortex/api.py
--rw-r--r--   0        0        0        0 2023-07-13 21:06:47.906830 trycortex-1.0.2/trycortex/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 21:06:52.532395 trycortex-1.0.2/trycortex/cli/cli.py
--rw-r--r--   0        0        0      325 1970-01-01 00:00:00.000000 trycortex-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0       57 2023-07-13 22:45:28.866895 trycortex-1.0.3/README.md
+-rw-r--r--   0        0        0      406 2023-07-13 22:44:57.064647 trycortex-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0       90 2023-07-13 21:47:58.631841 trycortex-1.0.3/trycortex/__init__.py
+-rw-r--r--   0        0        0    12976 2023-07-13 21:48:07.353240 trycortex-1.0.3/trycortex/api.py
+-rw-r--r--   0        0        0      308 2023-07-13 22:44:29.754288 trycortex-1.0.3/trycortex/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 22:29:16.670150 trycortex-1.0.3/trycortex/cli/callable/__init__.py
+-rw-r--r--   0        0        0      204 2023-07-13 22:41:02.868738 trycortex-1.0.3/trycortex/cli/callable/commands.py
+-rw-r--r--   0        0        0        0 2023-07-13 22:21:46.365142 trycortex-1.0.3/trycortex/cli/cli.py
+-rw-r--r--   0        0        0      405 1970-01-01 00:00:00.000000 trycortex-1.0.3/PKG-INFO
```

### Comparing `trycortex-1.0.2/trycortex/api.py` & `trycortex-1.0.3/trycortex/api.py`

 * *Files identical despite different names*

