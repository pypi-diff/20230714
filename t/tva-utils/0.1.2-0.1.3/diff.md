# Comparing `tmp/tva_utils-0.1.2.tar.gz` & `tmp/tva_utils-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tva_utils-0.1.2.tar", max compression
+gzip compressed data, was "tva_utils-0.1.3.tar", max compression
```

## Comparing `tva_utils-0.1.2.tar` & `tva_utils-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0        0 2023-07-13 23:17:23.166450 tva_utils-0.1.2/README.md
--rw-r--r--   0        0        0      352 2023-07-14 00:51:10.088678 tva_utils-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       71 2023-07-14 00:50:32.767732 tva_utils-0.1.2/tva_utils/__init__.py
--rw-r--r--   0        0        0      168 2023-07-14 00:50:27.683031 tva_utils-0.1.2/tva_utils/postgres/__init__.py
--rw-r--r--   0        0        0      430 2023-07-14 00:50:45.402621 tva_utils-0.1.2/tva_utils/postgres/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     9650 2023-07-14 00:50:45.404384 tva_utils-0.1.2/tva_utils/postgres/__pycache__/postgres.cpython-311.pyc
--rw-r--r--   0        0        0     1887 2023-07-14 00:16:18.073842 tva_utils-0.1.2/tva_utils/postgres/__pycache__/schemas.cpython-311.pyc
--rw-r--r--   0        0        0     4809 2023-07-14 00:50:10.421521 tva_utils-0.1.2/tva_utils/postgres/postgres.py
--rw-r--r--   0        0        0      655 2023-07-13 23:44:23.809176 tva_utils-0.1.2/tva_utils/postgres/schemas.py
--rw-r--r--   0        0        0      475 1970-01-01 00:00:00.000000 tva_utils-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-13 23:17:23.166450 tva_utils-0.1.3/README.md
+-rw-r--r--   0        0        0      352 2023-07-14 01:08:14.893163 tva_utils-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       71 2023-07-14 01:07:51.494172 tva_utils-0.1.3/tva_utils/__init__.py
+-rw-r--r--   0        0        0      165 2023-07-14 01:07:56.427003 tva_utils-0.1.3/tva_utils/postgres/__init__.py
+-rw-r--r--   0        0        0      427 2023-07-14 01:08:02.963561 tva_utils-0.1.3/tva_utils/postgres/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     9647 2023-07-14 01:08:02.965155 tva_utils-0.1.3/tva_utils/postgres/__pycache__/funcs.cpython-311.pyc
+-rw-r--r--   0        0        0     9650 2023-07-14 00:50:45.404384 tva_utils-0.1.3/tva_utils/postgres/__pycache__/postgres.cpython-311.pyc
+-rw-r--r--   0        0        0     1887 2023-07-14 00:16:18.073842 tva_utils-0.1.3/tva_utils/postgres/__pycache__/schemas.cpython-311.pyc
+-rw-r--r--   0        0        0     4809 2023-07-14 01:07:33.382706 tva_utils-0.1.3/tva_utils/postgres/funcs.py
+-rw-r--r--   0        0        0      655 2023-07-13 23:44:23.809176 tva_utils-0.1.3/tva_utils/postgres/schemas.py
+-rw-r--r--   0        0        0      475 1970-01-01 00:00:00.000000 tva_utils-0.1.3/PKG-INFO
```

### Comparing `tva_utils-0.1.2/tva_utils/postgres/__pycache__/postgres.cpython-311.pyc` & `tva_utils-0.1.3/tva_utils/postgres/__pycache__/postgres.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tva_utils-0.1.2/tva_utils/postgres/__pycache__/schemas.cpython-311.pyc` & `tva_utils-0.1.3/tva_utils/postgres/__pycache__/schemas.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tva_utils-0.1.2/tva_utils/postgres/postgres.py` & `tva_utils-0.1.3/tva_utils/postgres/funcs.py`

 * *Files identical despite different names*

### Comparing `tva_utils-0.1.2/tva_utils/postgres/schemas.py` & `tva_utils-0.1.3/tva_utils/postgres/schemas.py`

 * *Files identical despite different names*

