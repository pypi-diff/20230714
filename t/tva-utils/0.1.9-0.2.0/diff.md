# Comparing `tmp/tva_utils-0.1.9.tar.gz` & `tmp/tva_utils-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tva_utils-0.1.9.tar", max compression
+gzip compressed data, was "tva_utils-0.2.0.tar", max compression
```

## Comparing `tva_utils-0.1.9.tar` & `tva_utils-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2023-07-13 23:17:23.166450 tva_utils-0.1.9/README.md
--rw-r--r--   0        0        0      432 2023-07-14 02:45:58.570355 tva_utils-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      154 2023-07-14 02:45:46.127026 tva_utils-0.1.9/tva_utils/__init__.py
--rw-r--r--   0        0        0      132 2023-07-14 01:37:17.931047 tva_utils-0.1.9/tva_utils/logging/__init__.py
--rw-r--r--   0        0        0      326 2023-07-14 01:37:19.727024 tva_utils-0.1.9/tva_utils/logging/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2361 2023-07-14 01:39:03.597655 tva_utils-0.1.9/tva_utils/logging/__pycache__/logging.cpython-311.pyc
--rw-r--r--   0        0        0     1467 2023-07-14 01:39:36.474015 tva_utils-0.1.9/tva_utils/logging/logging.py
--rw-r--r--   0        0        0       64 2023-07-14 02:04:46.808096 tva_utils-0.1.9/tva_utils/parser/__init__.py
--rw-r--r--   0        0        0      543 2023-07-14 02:44:50.430904 tva_utils-0.1.9/tva_utils/parser/parser.py
--rw-r--r--   0        0        0      130 2023-07-14 02:45:38.826522 tva_utils-0.1.9/tva_utils/postgres/__init__.py
--rw-r--r--   0        0        0      459 2023-07-14 01:36:40.919534 tva_utils-0.1.9/tva_utils/postgres/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     9791 2023-07-14 01:36:40.921077 tva_utils-0.1.9/tva_utils/postgres/__pycache__/funcs.cpython-311.pyc
--rw-r--r--   0        0        0     9650 2023-07-14 00:50:45.404384 tva_utils-0.1.9/tva_utils/postgres/__pycache__/postgres.cpython-311.pyc
--rw-r--r--   0        0        0     1887 2023-07-14 00:16:18.073842 tva_utils-0.1.9/tva_utils/postgres/__pycache__/schemas.cpython-311.pyc
--rw-r--r--   0        0        0     5541 2023-07-14 02:35:22.372810 tva_utils-0.1.9/tva_utils/postgres/funcs.py
--rw-r--r--   0        0        0      520 1970-01-01 00:00:00.000000 tva_utils-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-13 23:17:23.166450 tva_utils-0.2.0/README.md
+-rw-r--r--   0        0        0      432 2023-07-14 02:50:11.612042 tva_utils-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      154 2023-07-14 02:45:46.127026 tva_utils-0.2.0/tva_utils/__init__.py
+-rw-r--r--   0        0        0      132 2023-07-14 01:37:17.931047 tva_utils-0.2.0/tva_utils/logging/__init__.py
+-rw-r--r--   0        0        0      326 2023-07-14 01:37:19.727024 tva_utils-0.2.0/tva_utils/logging/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2361 2023-07-14 01:39:03.597655 tva_utils-0.2.0/tva_utils/logging/__pycache__/logging.cpython-311.pyc
+-rw-r--r--   0        0        0     1467 2023-07-14 01:39:36.474015 tva_utils-0.2.0/tva_utils/logging/logging.py
+-rw-r--r--   0        0        0       64 2023-07-14 02:04:46.808096 tva_utils-0.2.0/tva_utils/parser/__init__.py
+-rw-r--r--   0        0        0      543 2023-07-14 02:44:50.430904 tva_utils-0.2.0/tva_utils/parser/parser.py
+-rw-r--r--   0        0        0      130 2023-07-14 02:45:38.826522 tva_utils-0.2.0/tva_utils/postgres/__init__.py
+-rw-r--r--   0        0        0      459 2023-07-14 01:36:40.919534 tva_utils-0.2.0/tva_utils/postgres/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     9791 2023-07-14 01:36:40.921077 tva_utils-0.2.0/tva_utils/postgres/__pycache__/funcs.cpython-311.pyc
+-rw-r--r--   0        0        0     9650 2023-07-14 00:50:45.404384 tva_utils-0.2.0/tva_utils/postgres/__pycache__/postgres.cpython-311.pyc
+-rw-r--r--   0        0        0     1887 2023-07-14 00:16:18.073842 tva_utils-0.2.0/tva_utils/postgres/__pycache__/schemas.cpython-311.pyc
+-rw-r--r--   0        0        0     5491 2023-07-14 02:49:56.905018 tva_utils-0.2.0/tva_utils/postgres/funcs.py
+-rw-r--r--   0        0        0      520 1970-01-01 00:00:00.000000 tva_utils-0.2.0/PKG-INFO
```

### Comparing `tva_utils-0.1.9/tva_utils/logging/__pycache__/logging.cpython-311.pyc` & `tva_utils-0.2.0/tva_utils/logging/__pycache__/logging.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tva_utils-0.1.9/tva_utils/logging/logging.py` & `tva_utils-0.2.0/tva_utils/logging/logging.py`

 * *Files identical despite different names*

### Comparing `tva_utils-0.1.9/tva_utils/parser/parser.py` & `tva_utils-0.2.0/tva_utils/parser/parser.py`

 * *Files identical despite different names*

### Comparing `tva_utils-0.1.9/tva_utils/postgres/__pycache__/funcs.cpython-311.pyc` & `tva_utils-0.2.0/tva_utils/postgres/__pycache__/funcs.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tva_utils-0.1.9/tva_utils/postgres/__pycache__/postgres.cpython-311.pyc` & `tva_utils-0.2.0/tva_utils/postgres/__pycache__/postgres.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tva_utils-0.1.9/tva_utils/postgres/__pycache__/schemas.cpython-311.pyc` & `tva_utils-0.2.0/tva_utils/postgres/__pycache__/schemas.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tva_utils-0.1.9/tva_utils/postgres/funcs.py` & `tva_utils-0.2.0/tva_utils/postgres/funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from tva_utils.postgres.schemas import BaseModel
-
 from sqlalchemy.exc import DBAPIError
 from sqlalchemy.orm.session import Session
 from sqlalchemy import text, inspect
 from sqlalchemy import create_engine
 from sqlalchemy.engine.base import Engine
 from sqlalchemy.orm import sessionmaker, scoped_session
 from sqlalchemy.orm import DeclarativeMeta
```

### Comparing `tva_utils-0.1.9/PKG-INFO` & `tva_utils-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tva-utils
-Version: 0.1.9
+Version: 0.2.0
 Summary: 
 Author: jsaied99
 Author-email: jsaied99@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

