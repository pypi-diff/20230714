# Comparing `tmp/tva_utils-0.1.3.tar.gz` & `tmp/tva_utils-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tva_utils-0.1.3.tar", max compression
+gzip compressed data, was "tva_utils-0.1.4.tar", max compression
```

## Comparing `tva_utils-0.1.3.tar` & `tva_utils-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2023-07-13 23:17:23.166450 tva_utils-0.1.3/README.md
--rw-r--r--   0        0        0      352 2023-07-14 01:08:14.893163 tva_utils-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       71 2023-07-14 01:07:51.494172 tva_utils-0.1.3/tva_utils/__init__.py
--rw-r--r--   0        0        0      165 2023-07-14 01:07:56.427003 tva_utils-0.1.3/tva_utils/postgres/__init__.py
--rw-r--r--   0        0        0      427 2023-07-14 01:08:02.963561 tva_utils-0.1.3/tva_utils/postgres/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     9647 2023-07-14 01:08:02.965155 tva_utils-0.1.3/tva_utils/postgres/__pycache__/funcs.cpython-311.pyc
--rw-r--r--   0        0        0     9650 2023-07-14 00:50:45.404384 tva_utils-0.1.3/tva_utils/postgres/__pycache__/postgres.cpython-311.pyc
--rw-r--r--   0        0        0     1887 2023-07-14 00:16:18.073842 tva_utils-0.1.3/tva_utils/postgres/__pycache__/schemas.cpython-311.pyc
--rw-r--r--   0        0        0     4809 2023-07-14 01:07:33.382706 tva_utils-0.1.3/tva_utils/postgres/funcs.py
--rw-r--r--   0        0        0      655 2023-07-13 23:44:23.809176 tva_utils-0.1.3/tva_utils/postgres/schemas.py
--rw-r--r--   0        0        0      475 1970-01-01 00:00:00.000000 tva_utils-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-13 23:17:23.166450 tva_utils-0.1.4/README.md
+-rw-r--r--   0        0        0      352 2023-07-14 01:12:58.890042 tva_utils-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       71 2023-07-14 01:07:51.494172 tva_utils-0.1.4/tva_utils/__init__.py
+-rw-r--r--   0        0        0      165 2023-07-14 01:07:56.427003 tva_utils-0.1.4/tva_utils/postgres/__init__.py
+-rw-r--r--   0        0        0      427 2023-07-14 01:08:02.963561 tva_utils-0.1.4/tva_utils/postgres/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     9647 2023-07-14 01:08:02.965155 tva_utils-0.1.4/tva_utils/postgres/__pycache__/funcs.cpython-311.pyc
+-rw-r--r--   0        0        0     9650 2023-07-14 00:50:45.404384 tva_utils-0.1.4/tva_utils/postgres/__pycache__/postgres.cpython-311.pyc
+-rw-r--r--   0        0        0     1887 2023-07-14 00:16:18.073842 tva_utils-0.1.4/tva_utils/postgres/__pycache__/schemas.cpython-311.pyc
+-rw-r--r--   0        0        0     4902 2023-07-14 01:17:56.068070 tva_utils-0.1.4/tva_utils/postgres/funcs.py
+-rw-r--r--   0        0        0      655 2023-07-13 23:44:23.809176 tva_utils-0.1.4/tva_utils/postgres/schemas.py
+-rw-r--r--   0        0        0      475 1970-01-01 00:00:00.000000 tva_utils-0.1.4/PKG-INFO
```

### Comparing `tva_utils-0.1.3/tva_utils/postgres/__pycache__/funcs.cpython-311.pyc` & `tva_utils-0.1.4/tva_utils/postgres/__pycache__/funcs.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tva_utils-0.1.3/tva_utils/postgres/__pycache__/postgres.cpython-311.pyc` & `tva_utils-0.1.4/tva_utils/postgres/__pycache__/postgres.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tva_utils-0.1.3/tva_utils/postgres/__pycache__/schemas.cpython-311.pyc` & `tva_utils-0.1.4/tva_utils/postgres/__pycache__/schemas.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tva_utils-0.1.3/tva_utils/postgres/funcs.py` & `tva_utils-0.1.4/tva_utils/postgres/funcs.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,25 +10,23 @@
 import sqlalchemy
 
 from typing import List, Union, Iterator
 import uuid
 
 
 class DB:
-    def initialize(cls, url: str):
-        cls.engine: Engine = get_engine(url)
+    def initialize(cls, url: str, **kwargs):
+        cls.engine: Engine = get_engine(url, **kwargs)
         cls.SessionLocal = sessionmaker(
             autocommit=False, autoflush=False, bind=cls.engine
         )
         cls.inspector = inspect(cls.engine)
         cls.utils = DBUtils()
 
-        # cls._create_tables()
-
-    def _create_tables(cls, Bases: List[DeclarativeMeta], schemas: List[str]):
+    def create_tables(cls, Bases: List[DeclarativeMeta], schemas: List[str]):
 
         for Base, schema in zip(Bases, schemas):
             try:
                 if schema not in cls.inspector.get_schema_names():
                     cls.engine.execute(sqlalchemy.schema.CreateSchema(schema))
                 Base.metadata.create_all(cls.engine)
             except Exception as e:
@@ -58,109 +56,111 @@
 
     @staticmethod
     def wrap_to_json(stmt: str) -> text:
         stmt = stmt.replace(";", "")
         return text(f"SELECT json_agg(t) FROM ({stmt}) t")
 
 
-    def select_stmt_raw_sql(cls, sql: str) -> Union[List[dict], None]:
+    def select_stmt_raw_sql(cls, session: Session, sql: str) -> Union[List[dict], None]:
         try:
             stmt: text = cls.wrap_to_json(sql)
-            results = cls.session.execute(stmt).fetchone()[0]
+            results = session.execute(stmt).fetchone()[0]
             if results is None:
                 return []
 
             return results
         except DBAPIError as e:
             raise e
         
-    def execute_stmt_raw_sql(cls, sql: str) -> Union[bool, None]:
+    def execute_stmt_raw_sql(cls, session: Session, sql: str) -> Union[bool, None]:
         try:
             stmt: text = text(sql)
-            cls.session.execute(stmt)
+            session.execute(stmt)
 
             return True
         except DBAPIError as e:
             raise e
 
 
     def select_stmt_raw_sql_params(
         cls,
+        session: Session,
         sql: str,
         params: dict,
     ) -> Union[List[dict], None]:
         try:
             stmt: text = cls.wrap_to_json(sql)
-            results = cls.session.execute(stmt, params=params).fetchone()[0]
+            results = session.execute(stmt, params=params).fetchone()[0]
 
             if results is None:
                 return []
 
             return results
         except DBAPIError as e:
             # logger.info(f"Error in select_stmt_raw_sql_params: {e}")
             raise e
 
 
-    def add_record_sync(cls, model, kwargs) -> Union[object, None]:
+    def add_record_sync(cls, session: Session, model, kwargs) -> Union[object, None]:
         try:
             obj = model(**kwargs)
-            cls.session.add(obj)
-            cls.session.commit()
+            session.add(obj)
+            session.commit()
             return obj
         except DBAPIError as e:
             # logger.info(f"Error in add_record_sync: {e}")
-            cls.session.rollback()
+            session.rollback()
             return None
 
 
     def add_records_sync(
-        cls, model: BaseModel, records: List[dict]
+        cls, session: Session, model: BaseModel, records: List[dict]
     ) -> Union[List[uuid.UUID], List[BaseModel]]:
         try:
             inserted_ids = []
 
             records_to_insert: List[BaseModel] = [model(**record) for record in records]
 
-            cls.session.add_all(records_to_insert)
-            cls.session.flush()  # Flush the records to obtain their IDs
+            session.add_all(records_to_insert)
+            session.flush()  # Flush the records to obtain their IDs
             
             records: dict = [record.to_dict() for record in records_to_insert]
             for record in records_to_insert:
                 inserted_ids.append(record.uuid)
-            cls.session.commit()
+            session.commit()
             return inserted_ids, records
         except DBAPIError as e:
             cls.session.rollback()
             # logger.info(f"Error in add_records_sync: {e}")
             return [], []
 
 
     def remove_records_sync(
-        cls, model: BaseModel, records: List[uuid.UUID]
+        cls, session: Session, model: BaseModel, records: List[uuid.UUID]
     ) -> bool:
         try:
-            cls.session.query(model).filter(model.uuid.in_(records)).delete(
+            session.query(model).filter(model.uuid.in_(records)).delete(
                 synchronize_session=False
             )
-            cls.session.commit()
+            session.commit()
             # logger.info(f"Deleted {len(records)} records")
             return True
         except DBAPIError as e:
-            cls.session.rollback()
+            session.rollback()
             # logger.info(f"Error in remove_records_sync: {e}")
             return False
 
 
-def get_engine(url: str) -> Engine:
+def get_engine(url: str, **kwargs) -> Engine:
     try:
         return create_engine(
             url,
-            pool_size=5,
-            max_overflow=0,
-            pool_pre_ping=True,
+            **kwargs,
+            # pool_size=5,
+            # max_overflow=0,
+            # pool_pre_ping=True,
         )
     except DBAPIError as e:
         # logger.info(f"Error in get_engine: {e}")
         raise e
     
 db = DB()
```

### Comparing `tva_utils-0.1.3/tva_utils/postgres/schemas.py` & `tva_utils-0.1.4/tva_utils/postgres/schemas.py`

 * *Files identical despite different names*

