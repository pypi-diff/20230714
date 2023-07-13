# Comparing `tmp/sqlalchemy-crud-0.1.0b0.tar.gz` & `tmp/sqlalchemy_crud-0.1.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-crud-0.1.0b0.tar", last modified: Mon Oct 12 20:03:31 2020, max compression
+gzip compressed data, was "sqlalchemy_crud-0.1.1b0.tar", max compression
```

## Comparing `sqlalchemy-crud-0.1.0b0.tar` & `sqlalchemy_crud-0.1.1b0.tar`

### file list

```diff
@@ -1,7 +1,4 @@
--rw-r--r--   0        0        0      498 2020-10-12 20:03:20.847226 sqlalchemy-crud-0.1.0b0/pyproject.toml
--rw-r--r--   0        0        0       22 2020-10-12 20:03:20.847226 sqlalchemy-crud-0.1.0b0/sqlalchemy_crud/__init__.py
--rw-r--r--   0        0        0     2945 2020-10-12 20:03:20.847226 sqlalchemy-crud-0.1.0b0/sqlalchemy_crud/crud.py
--rw-r--r--   0        0        0        0 2020-10-12 20:03:20.847226 sqlalchemy-crud-0.1.0b0/sqlalchemy_crud/tests/__init__.py
--rw-r--r--   0        0        0       96 2020-10-12 20:03:20.847226 sqlalchemy-crud-0.1.0b0/sqlalchemy_crud/tests/test_sqlalchemy_crud.py
--rw-r--r--   0        0        0      691 2020-10-12 20:03:31.624933 sqlalchemy-crud-0.1.0b0/setup.py
--rw-r--r--   0        0        0      549 2020-10-12 20:03:31.625267 sqlalchemy-crud-0.1.0b0/PKG-INFO
+-rw-r--r--   0        0        0      617 2023-07-13 22:05:16.918993 sqlalchemy_crud-0.1.1b0/pyproject.toml
+-rw-r--r--   0        0        0      221 2023-07-13 22:05:16.918993 sqlalchemy_crud-0.1.1b0/sqlalchemy_crud/__init__.py
+-rw-r--r--   0        0        0     2945 2023-07-13 22:05:16.918993 sqlalchemy_crud-0.1.1b0/sqlalchemy_crud/crud.py
+-rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 sqlalchemy_crud-0.1.1b0/PKG-INFO
```

### Comparing `sqlalchemy-crud-0.1.0b0/sqlalchemy_crud/crud.py` & `sqlalchemy_crud-0.1.1b0/sqlalchemy_crud/crud.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List
 
-from sqlalchemy.orm import Session
 from sqlalchemy.ext.declarative import declarative_base
+from sqlalchemy.orm import Session
 
 Base = declarative_base()
 
 
 def get_models(
     db: Session, model: Base, offset: int = 0, limit: int = 100
 ) -> List[Base]:
```

