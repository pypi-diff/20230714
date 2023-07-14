# Comparing `tmp/tva_utils-0.1.6.tar.gz` & `tmp/tva_utils-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tva_utils-0.1.6.tar", max compression
+gzip compressed data, was "tva_utils-0.1.7.tar", max compression
```

## Comparing `tva_utils-0.1.6.tar` & `tva_utils-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0        0 2023-07-13 23:17:23.166450 tva_utils-0.1.6/README.md
--rw-r--r--   0        0        0      376 2023-07-14 01:39:44.064644 tva_utils-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      129 2023-07-14 01:27:00.735841 tva_utils-0.1.6/tva_utils/__init__.py
--rw-r--r--   0        0        0      132 2023-07-14 01:37:17.931047 tva_utils-0.1.6/tva_utils/logging/__init__.py
--rw-r--r--   0        0        0      326 2023-07-14 01:37:19.727024 tva_utils-0.1.6/tva_utils/logging/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2361 2023-07-14 01:39:03.597655 tva_utils-0.1.6/tva_utils/logging/__pycache__/logging.cpython-311.pyc
--rw-r--r--   0        0        0     1467 2023-07-14 01:39:36.474015 tva_utils-0.1.6/tva_utils/logging/logging.py
--rw-r--r--   0        0        0      191 2023-07-14 01:27:15.934581 tva_utils-0.1.6/tva_utils/postgres/__init__.py
--rw-r--r--   0        0        0      459 2023-07-14 01:36:40.919534 tva_utils-0.1.6/tva_utils/postgres/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     9791 2023-07-14 01:36:40.921077 tva_utils-0.1.6/tva_utils/postgres/__pycache__/funcs.cpython-311.pyc
--rw-r--r--   0        0        0     9650 2023-07-14 00:50:45.404384 tva_utils-0.1.6/tva_utils/postgres/__pycache__/postgres.cpython-311.pyc
--rw-r--r--   0        0        0     1887 2023-07-14 00:16:18.073842 tva_utils-0.1.6/tva_utils/postgres/__pycache__/schemas.cpython-311.pyc
--rw-r--r--   0        0        0     5141 2023-07-14 01:22:18.988402 tva_utils-0.1.6/tva_utils/postgres/funcs.py
--rw-r--r--   0        0        0      655 2023-07-13 23:44:23.809176 tva_utils-0.1.6/tva_utils/postgres/schemas.py
--rw-r--r--   0        0        0      520 1970-01-01 00:00:00.000000 tva_utils-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-13 23:17:23.166450 tva_utils-0.1.7/README.md
+-rw-r--r--   0        0        0      461 2023-07-14 02:23:44.228724 tva_utils-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      171 2023-07-14 02:06:45.158105 tva_utils-0.1.7/tva_utils/__init__.py
+-rw-r--r--   0        0        0      132 2023-07-14 01:37:17.931047 tva_utils-0.1.7/tva_utils/logging/__init__.py
+-rw-r--r--   0        0        0      326 2023-07-14 01:37:19.727024 tva_utils-0.1.7/tva_utils/logging/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2361 2023-07-14 01:39:03.597655 tva_utils-0.1.7/tva_utils/logging/__pycache__/logging.cpython-311.pyc
+-rw-r--r--   0        0        0     1467 2023-07-14 01:39:36.474015 tva_utils-0.1.7/tva_utils/logging/logging.py
+-rw-r--r--   0        0        0       64 2023-07-14 02:04:46.808096 tva_utils-0.1.7/tva_utils/parser/__init__.py
+-rw-r--r--   0        0        0      608 2023-07-14 02:08:15.103802 tva_utils-0.1.7/tva_utils/parser/parser.py
+-rw-r--r--   0        0        0      191 2023-07-14 01:27:15.934581 tva_utils-0.1.7/tva_utils/postgres/__init__.py
+-rw-r--r--   0        0        0      459 2023-07-14 01:36:40.919534 tva_utils-0.1.7/tva_utils/postgres/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     9791 2023-07-14 01:36:40.921077 tva_utils-0.1.7/tva_utils/postgres/__pycache__/funcs.cpython-311.pyc
+-rw-r--r--   0        0        0     9650 2023-07-14 00:50:45.404384 tva_utils-0.1.7/tva_utils/postgres/__pycache__/postgres.cpython-311.pyc
+-rw-r--r--   0        0        0     1887 2023-07-14 00:16:18.073842 tva_utils-0.1.7/tva_utils/postgres/__pycache__/schemas.cpython-311.pyc
+-rw-r--r--   0        0        0     5541 2023-07-14 02:23:04.652363 tva_utils-0.1.7/tva_utils/postgres/funcs.py
+-rw-r--r--   0        0        0      655 2023-07-13 23:44:23.809176 tva_utils-0.1.7/tva_utils/postgres/schemas.py
+-rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 tva_utils-0.1.7/PKG-INFO
```

### Comparing `tva_utils-0.1.6/tva_utils/logging/__pycache__/logging.cpython-311.pyc` & `tva_utils-0.1.7/tva_utils/logging/__pycache__/logging.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tva_utils-0.1.6/tva_utils/logging/logging.py` & `tva_utils-0.1.7/tva_utils/logging/logging.py`

 * *Files identical despite different names*

### Comparing `tva_utils-0.1.6/tva_utils/postgres/__pycache__/funcs.cpython-311.pyc` & `tva_utils-0.1.7/tva_utils/postgres/__pycache__/funcs.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tva_utils-0.1.6/tva_utils/postgres/__pycache__/postgres.cpython-311.pyc` & `tva_utils-0.1.7/tva_utils/postgres/__pycache__/postgres.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tva_utils-0.1.6/tva_utils/postgres/__pycache__/schemas.cpython-311.pyc` & `tva_utils-0.1.7/tva_utils/postgres/__pycache__/schemas.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tva_utils-0.1.6/tva_utils/postgres/funcs.py` & `tva_utils-0.1.7/tva_utils/postgres/funcs.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,45 +4,55 @@
 from sqlalchemy.orm.session import Session
 from sqlalchemy import text, inspect
 from sqlalchemy import create_engine
 from sqlalchemy.engine.base import Engine
 from sqlalchemy.orm import sessionmaker, scoped_session
 from sqlalchemy.orm import DeclarativeMeta
 import sqlalchemy
+import logging
 
 from typing import List, Union, Iterator
 import uuid
 
 
 class DB:
-    def initialize(cls, url: str, **kwargs):
+    def initialize(cls, url: str, logger: logging.Logger = None, **kwargs):
         cls.engine: Engine = get_engine(url, **kwargs)
         cls.SessionLocal = sessionmaker(
             autocommit=False, autoflush=False, bind=cls.engine
         )
         cls.inspector = inspect(cls.engine)
-        cls.utils = DBUtils()
+        cls.logger = logger
 
-    def create_tables(cls, Bases: List[DeclarativeMeta], schemas: List[str] = ["public"]):
+        if cls.logger is None:
+            cls.logger = logging.getLogger("uvicorn.error")
+
+        cls.utils = DBUtils(cls.logger)
+
+        cls.logger.info("Initialized DB")
+
+    def create_tables(
+        cls, Bases: List[DeclarativeMeta], schemas: List[str] = ["public"]
+    ):
         """
         Creates tables for all the models in the list of Bases
         """
         if type(Bases) != list:
             Bases = [Bases]
-            
+
         if type(schemas) != list:
             schemas = [schemas]
 
         for Base, schema in zip(Bases, schemas):
             try:
                 if schema not in cls.inspector.get_schema_names():
                     cls.engine.execute(sqlalchemy.schema.CreateSchema(schema))
                 Base.metadata.create_all(cls.engine)
             except Exception as e:
-                print(e)
+                cls.logger.info(f"Error in create_tables: {e}")
 
     def get_session(cls) -> Iterator[Session]:
         with cls.SessionLocal() as session:
             try:
                 yield session
             finally:
                 session.close()
@@ -51,124 +61,128 @@
         return scoped_session(cls.SessionLocal)
 
     def close(cls):
         cls.engine.dispose()
 
 
 class DBUtils:
-    
-    def __init__(cls):
+    def __init__(cls, logger: logging.Logger):
         cls.session = None
-        
+        cls.logger = logger
+
     def initialize(cls, session: Session):
         cls.session = session
 
     @staticmethod
     def wrap_to_json(stmt: str) -> text:
         stmt = stmt.replace(";", "")
         return text(f"SELECT json_agg(t) FROM ({stmt}) t")
 
-
-    def select_stmt_raw_sql(cls, session: Session, sql: str) -> Union[List[dict], None]:
+    def select(cls, session: Session, sql: str) -> Union[List[dict], None]:
         try:
             stmt: text = cls.wrap_to_json(sql)
             results = session.execute(stmt).fetchone()[0]
             if results is None:
                 return []
 
             return results
         except DBAPIError as e:
             raise e
-        
-    def execute_stmt_raw_sql(cls, session: Session, sql: str) -> Union[bool, None]:
+
+    def execute(cls, session: Session, sql: str) -> Union[bool, None]:
         try:
             stmt: text = text(sql)
             session.execute(stmt)
 
             return True
         except DBAPIError as e:
             raise e
 
-
-    def select_stmt_raw_sql_params(
+    def select_with_params(
         cls,
         session: Session,
         sql: str,
         params: dict,
     ) -> Union[List[dict], None]:
         try:
             stmt: text = cls.wrap_to_json(sql)
             results = session.execute(stmt, params=params).fetchone()[0]
 
             if results is None:
                 return []
 
             return results
         except DBAPIError as e:
-            # logger.info(f"Error in select_stmt_raw_sql_params: {e}")
+            cls.logger.info(f"Error in select_stmt_raw_sql_params: {e}")
             raise e
 
-
-    def add_record_sync(cls, session: Session, model, kwargs) -> Union[object, None]:
+    def add_record(cls, session: Session, model, kwargs) -> Union[object, None]:
         try:
             obj = model(**kwargs)
             session.add(obj)
             session.commit()
             return obj
         except DBAPIError as e:
-            # logger.info(f"Error in add_record_sync: {e}")
+            cls.logger.info(f"Error in add_record_sync: {e}")
             session.rollback()
             return None
 
-
-    def add_records_sync(
+    def add_records(
         cls, session: Session, model: BaseModel, records: List[dict]
     ) -> Union[List[uuid.UUID], List[BaseModel]]:
         try:
             inserted_ids = []
 
             records_to_insert: List[BaseModel] = [model(**record) for record in records]
 
             session.add_all(records_to_insert)
             session.flush()  # Flush the records to obtain their IDs
-            
+
             records: dict = [record.to_dict() for record in records_to_insert]
             for record in records_to_insert:
                 inserted_ids.append(record.uuid)
             session.commit()
             return inserted_ids, records
         except DBAPIError as e:
             cls.session.rollback()
-            # logger.info(f"Error in add_records_sync: {e}")
+            cls.logger.info(f"Error in add_records_sync: {e}")
             return [], []
 
+    def add_records_on_conflict(
+        cls,
+        session: Session,
+        model: BaseModel,
+        records: List[dict],
+    ):
+        for record in records:
+            cls.add_record(session, model, record)
 
-    def remove_records_sync(
+    def remove_records(
         cls, session: Session, model: BaseModel, records: List[uuid.UUID]
     ) -> bool:
         try:
             session.query(model).filter(model.uuid.in_(records)).delete(
                 synchronize_session=False
             )
             session.commit()
-            # logger.info(f"Deleted {len(records)} records")
+            cls.logger.info(f"Deleted {len(records)} records")
             return True
         except DBAPIError as e:
             session.rollback()
-            # logger.info(f"Error in remove_records_sync: {e}")
+            cls.logger.info(f"Error in remove_records_sync: {e}")
             return False
 
 
 def get_engine(url: str, **kwargs) -> Engine:
     try:
         return create_engine(
             url,
             **kwargs,
             # pool_size=5,
             # max_overflow=0,
             # pool_pre_ping=True,
         )
     except DBAPIError as e:
-        # logger.info(f"Error in get_engine: {e}")
         raise e
-    
-db = DB()
+
+
+db = DB()
```

### Comparing `tva_utils-0.1.6/tva_utils/postgres/schemas.py` & `tva_utils-0.1.7/tva_utils/postgres/schemas.py`

 * *Files identical despite different names*

### Comparing `tva_utils-0.1.6/PKG-INFO` & `tva_utils-0.1.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: tva-utils
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: jsaied99
 Author-email: jsaied99@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: psycopg2-binary (>=2.9.6,<3.0.0)
+Requires-Dist: pydantic-settings (>=2.0.1,<3.0.0)
 Requires-Dist: sqlalchemy (>=2.0.18,<3.0.0)
 Requires-Dist: string-color (>=1.2.3,<2.0.0)
 Description-Content-Type: text/markdown
```

