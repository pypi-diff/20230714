# Comparing `tmp/sqlalchemy_crud-0.1.1b0.tar.gz` & `tmp/sqlalchemy_crud-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_crud-0.1.1b0.tar", max compression
+gzip compressed data, was "sqlalchemy_crud-0.1.2.tar", max compression
```

## Comparing `sqlalchemy_crud-0.1.1b0.tar` & `sqlalchemy_crud-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0      617 2023-07-13 22:05:16.918993 sqlalchemy_crud-0.1.1b0/pyproject.toml
--rw-r--r--   0        0        0      221 2023-07-13 22:05:16.918993 sqlalchemy_crud-0.1.1b0/sqlalchemy_crud/__init__.py
--rw-r--r--   0        0        0     2945 2023-07-13 22:05:16.918993 sqlalchemy_crud-0.1.1b0/sqlalchemy_crud/crud.py
--rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 sqlalchemy_crud-0.1.1b0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-14 00:03:20.483645 sqlalchemy_crud-0.1.2/LICENSE
+-rw-r--r--   0        0        0      627 2023-07-14 00:03:20.483645 sqlalchemy_crud-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      221 2023-07-14 00:03:20.483645 sqlalchemy_crud-0.1.2/sqlalchemy_crud/__init__.py
+-rw-r--r--   0        0        0     2945 2023-07-14 00:03:20.483645 sqlalchemy_crud-0.1.2/sqlalchemy_crud/crud.py
+-rw-r--r--   0        0        0      788 1970-01-01 00:00:00.000000 sqlalchemy_crud-0.1.2/PKG-INFO
```

### Comparing `sqlalchemy_crud-0.1.1b0/pyproject.toml` & `sqlalchemy_crud-0.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tool.poetry]
 name = "sqlalchemy-crud"
 repository = "https://github.com/cblack34/sqlalchemy-crud"
-version = "v0.1.1-beta"
+version = "0.1.2"
 description = "Basic C.R.U.D for SQLAlchemy models"
 authors = ["Clayton Black"]
+license = "MIT"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/cblack34/sqlalchemy-crud/issues"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 SQLAlchemy = "^1.3.19"
```

### Comparing `sqlalchemy_crud-0.1.1b0/sqlalchemy_crud/crud.py` & `sqlalchemy_crud-0.1.2/sqlalchemy_crud/crud.py`

 * *Files identical despite different names*

