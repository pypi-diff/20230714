# Comparing `tmp/tva_utils-0.1.4.tar.gz` & `tmp/tva_utils-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tva_utils-0.1.4.tar", max compression
+gzip compressed data, was "tva_utils-0.1.5.tar", max compression
```

## Comparing `tva_utils-0.1.4.tar` & `tva_utils-0.1.5.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0        0 2023-07-13 23:17:23.166450 tva_utils-0.1.4/README.md
--rw-r--r--   0        0        0      352 2023-07-14 01:12:58.890042 tva_utils-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       71 2023-07-14 01:07:51.494172 tva_utils-0.1.4/tva_utils/__init__.py
--rw-r--r--   0        0        0      165 2023-07-14 01:07:56.427003 tva_utils-0.1.4/tva_utils/postgres/__init__.py
--rw-r--r--   0        0        0      427 2023-07-14 01:08:02.963561 tva_utils-0.1.4/tva_utils/postgres/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     9647 2023-07-14 01:08:02.965155 tva_utils-0.1.4/tva_utils/postgres/__pycache__/funcs.cpython-311.pyc
--rw-r--r--   0        0        0     9650 2023-07-14 00:50:45.404384 tva_utils-0.1.4/tva_utils/postgres/__pycache__/postgres.cpython-311.pyc
--rw-r--r--   0        0        0     1887 2023-07-14 00:16:18.073842 tva_utils-0.1.4/tva_utils/postgres/__pycache__/schemas.cpython-311.pyc
--rw-r--r--   0        0        0     4902 2023-07-14 01:17:56.068070 tva_utils-0.1.4/tva_utils/postgres/funcs.py
--rw-r--r--   0        0        0      655 2023-07-13 23:44:23.809176 tva_utils-0.1.4/tva_utils/postgres/schemas.py
--rw-r--r--   0        0        0      475 1970-01-01 00:00:00.000000 tva_utils-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-13 23:17:23.166450 tva_utils-0.1.5/README.md
+-rw-r--r--   0        0        0      376 2023-07-14 01:27:23.581833 tva_utils-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      129 2023-07-14 01:27:00.735841 tva_utils-0.1.5/tva_utils/__init__.py
+-rw-r--r--   0        0        0      191 2023-07-14 01:27:15.934581 tva_utils-0.1.5/tva_utils/postgres/__init__.py
+-rw-r--r--   0        0        0      427 2023-07-14 01:08:02.963561 tva_utils-0.1.5/tva_utils/postgres/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     9647 2023-07-14 01:08:02.965155 tva_utils-0.1.5/tva_utils/postgres/__pycache__/funcs.cpython-311.pyc
+-rw-r--r--   0        0        0     9650 2023-07-14 00:50:45.404384 tva_utils-0.1.5/tva_utils/postgres/__pycache__/postgres.cpython-311.pyc
+-rw-r--r--   0        0        0     1887 2023-07-14 00:16:18.073842 tva_utils-0.1.5/tva_utils/postgres/__pycache__/schemas.cpython-311.pyc
+-rw-r--r--   0        0        0     5141 2023-07-14 01:22:18.988402 tva_utils-0.1.5/tva_utils/postgres/funcs.py
+-rw-r--r--   0        0        0      655 2023-07-13 23:44:23.809176 tva_utils-0.1.5/tva_utils/postgres/schemas.py
+-rw-r--r--   0        0        0       57 2023-07-14 01:26:54.473423 tva_utils-0.1.5/tva_utils/timers/__init__.py
+-rw-r--r--   0        0        0     1251 2023-07-14 01:26:01.937830 tva_utils-0.1.5/tva_utils/timers/timers.py
+-rw-r--r--   0        0        0      520 1970-01-01 00:00:00.000000 tva_utils-0.1.5/PKG-INFO
```

### Comparing `tva_utils-0.1.4/tva_utils/postgres/__pycache__/funcs.cpython-311.pyc` & `tva_utils-0.1.5/tva_utils/postgres/__pycache__/funcs.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tva_utils-0.1.4/tva_utils/postgres/__pycache__/postgres.cpython-311.pyc` & `tva_utils-0.1.5/tva_utils/postgres/__pycache__/postgres.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tva_utils-0.1.4/tva_utils/postgres/__pycache__/schemas.cpython-311.pyc` & `tva_utils-0.1.5/tva_utils/postgres/__pycache__/schemas.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tva_utils-0.1.4/tva_utils/postgres/funcs.py` & `tva_utils-0.1.5/tva_utils/postgres/funcs.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,23 @@
         cls.engine: Engine = get_engine(url, **kwargs)
         cls.SessionLocal = sessionmaker(
             autocommit=False, autoflush=False, bind=cls.engine
         )
         cls.inspector = inspect(cls.engine)
         cls.utils = DBUtils()
 
-    def create_tables(cls, Bases: List[DeclarativeMeta], schemas: List[str]):
+    def create_tables(cls, Bases: List[DeclarativeMeta], schemas: List[str] = ["public"]):
+        """
+        Creates tables for all the models in the list of Bases
+        """
+        if type(Bases) != list:
+            Bases = [Bases]
+            
+        if type(schemas) != list:
+            schemas = [schemas]
 
         for Base, schema in zip(Bases, schemas):
             try:
                 if schema not in cls.inspector.get_schema_names():
                     cls.engine.execute(sqlalchemy.schema.CreateSchema(schema))
                 Base.metadata.create_all(cls.engine)
             except Exception as e:
```

### Comparing `tva_utils-0.1.4/tva_utils/postgres/schemas.py` & `tva_utils-0.1.5/tva_utils/postgres/schemas.py`

 * *Files identical despite different names*

