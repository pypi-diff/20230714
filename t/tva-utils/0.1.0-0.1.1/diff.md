# Comparing `tmp/tva_utils-0.1.0.tar.gz` & `tmp/tva_utils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tva_utils-0.1.0.tar", max compression
+gzip compressed data, was "tva_utils-0.1.1.tar", max compression
```

## Comparing `tva_utils-0.1.0.tar` & `tva_utils-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-07-13 23:17:23.166450 tva_utils-0.1.0/README.md
--rw-r--r--   0        0        0      326 2023-07-14 00:30:14.418959 tva_utils-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       52 2023-07-14 00:02:24.445394 tva_utils-0.1.0/tva_utils/__init__.py
--rw-r--r--   0        0        0      133 2023-07-14 00:16:30.253118 tva_utils-0.1.0/tva_utils/db/__init__.py
--rw-r--r--   0        0        0      375 2023-07-14 00:16:33.202871 tva_utils-0.1.0/tva_utils/db/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     9672 2023-07-14 00:30:09.267273 tva_utils-0.1.0/tva_utils/db/__pycache__/postgres.cpython-311.pyc
--rw-r--r--   0        0        0     1887 2023-07-14 00:16:18.073842 tva_utils-0.1.0/tva_utils/db/__pycache__/schemas.cpython-311.pyc
--rw-r--r--   0        0        0     4786 2023-07-14 00:32:32.607265 tva_utils-0.1.0/tva_utils/db/postgres.py
--rw-r--r--   0        0        0      655 2023-07-13 23:44:23.809176 tva_utils-0.1.0/tva_utils/db/schemas.py
--rw-r--r--   0        0        0      327 1970-01-01 00:00:00.000000 tva_utils-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-13 23:17:23.166450 tva_utils-0.1.1/README.md
+-rw-r--r--   0        0        0      325 2023-07-14 00:40:22.606743 tva_utils-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       52 2023-07-14 00:02:24.445394 tva_utils-0.1.1/tva_utils/__init__.py
+-rw-r--r--   0        0        0      133 2023-07-14 00:16:30.253118 tva_utils-0.1.1/tva_utils/db/__init__.py
+-rw-r--r--   0        0        0      375 2023-07-14 00:16:33.202871 tva_utils-0.1.1/tva_utils/db/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     9672 2023-07-14 00:30:09.267273 tva_utils-0.1.1/tva_utils/db/__pycache__/postgres.cpython-311.pyc
+-rw-r--r--   0        0        0     1887 2023-07-14 00:16:18.073842 tva_utils-0.1.1/tva_utils/db/__pycache__/schemas.cpython-311.pyc
+-rw-r--r--   0        0        0     4786 2023-07-14 00:32:32.607265 tva_utils-0.1.1/tva_utils/db/postgres.py
+-rw-r--r--   0        0        0      655 2023-07-13 23:44:23.809176 tva_utils-0.1.1/tva_utils/db/schemas.py
+-rw-r--r--   0        0        0      427 1970-01-01 00:00:00.000000 tva_utils-0.1.1/PKG-INFO
```

### Comparing `tva_utils-0.1.0/tva_utils/db/__pycache__/postgres.cpython-311.pyc` & `tva_utils-0.1.1/tva_utils/db/__pycache__/postgres.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tva_utils-0.1.0/tva_utils/db/__pycache__/schemas.cpython-311.pyc` & `tva_utils-0.1.1/tva_utils/db/__pycache__/schemas.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tva_utils-0.1.0/tva_utils/db/postgres.py` & `tva_utils-0.1.1/tva_utils/db/postgres.py`

 * *Files identical despite different names*

### Comparing `tva_utils-0.1.0/tva_utils/db/schemas.py` & `tva_utils-0.1.1/tva_utils/db/schemas.py`

 * *Files identical despite different names*

