# Comparing `tmp/pydantic_db_backend-0.5.0.tar.gz` & `tmp/pydantic_db_backend-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_db_backend-0.5.0.tar", max compression
+gzip compressed data, was "pydantic_db_backend-0.6.0.tar", max compression
```

## Comparing `pydantic_db_backend-0.5.0.tar` & `pydantic_db_backend-0.6.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       87 2023-06-14 17:15:43.151729 pydantic_db_backend-0.5.0/README.md
--rw-r--r--   0        0        0        0 2023-05-11 08:45:17.171212 pydantic_db_backend-0.5.0/pydantic_db_backend/__init__.py
--rw-r--r--   0        0        0     6872 2023-07-12 12:03:04.958498 pydantic_db_backend-0.5.0/pydantic_db_backend/backend.py
--rw-r--r--   0        0        0        0 2023-05-13 10:06:57.338481 pydantic_db_backend-0.5.0/pydantic_db_backend/backends/__init__.py
--rw-r--r--   0        0        0     7703 2023-07-12 12:59:36.806580 pydantic_db_backend-0.5.0/pydantic_db_backend/backends/couchdb.py
--rw-r--r--   0        0        0      100 2023-06-14 12:06:00.522425 pydantic_db_backend-0.5.0/pydantic_db_backend/backends/json_files.py
--rw-r--r--   0        0        0      701 2023-06-20 16:53:47.237618 pydantic_db_backend-0.5.0/pydantic_db_backend/exceptions/__init__.py
--rw-r--r--   0        0        0      617 2023-07-12 08:51:34.282543 pydantic_db_backend-0.5.0/pydantic_db_backend/indexes.py
--rw-r--r--   0        0        0     1192 2023-06-28 08:36:47.839745 pydantic_db_backend-0.5.0/pydantic_db_backend/utils.py
--rw-r--r--   0        0        0      996 2023-07-12 13:00:59.529502 pydantic_db_backend-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 pydantic_db_backend-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-06-14 17:15:43.151729 pydantic_db_backend-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-11 08:45:17.171212 pydantic_db_backend-0.6.0/pydantic_db_backend/__init__.py
+-rw-r--r--   0        0        0     7789 2023-07-14 09:24:44.711216 pydantic_db_backend-0.6.0/pydantic_db_backend/backend.py
+-rw-r--r--   0        0        0        0 2023-05-13 10:06:57.338481 pydantic_db_backend-0.6.0/pydantic_db_backend/backends/__init__.py
+-rw-r--r--   0        0        0     8650 2023-07-14 10:07:43.763037 pydantic_db_backend-0.6.0/pydantic_db_backend/backends/couchdb.py
+-rw-r--r--   0        0        0      100 2023-06-14 12:06:00.522425 pydantic_db_backend-0.6.0/pydantic_db_backend/backends/json_files.py
+-rw-r--r--   0        0        0      990 2023-07-14 09:23:03.448444 pydantic_db_backend-0.6.0/pydantic_db_backend/exceptions/__init__.py
+-rw-r--r--   0        0        0      768 2023-07-12 13:44:19.743864 pydantic_db_backend-0.6.0/pydantic_db_backend/indexes.py
+-rw-r--r--   0        0        0     1192 2023-06-28 08:36:47.839745 pydantic_db_backend-0.6.0/pydantic_db_backend/utils.py
+-rw-r--r--   0        0        0      996 2023-07-14 10:12:23.112441 pydantic_db_backend-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 pydantic_db_backend-0.6.0/PKG-INFO
```

### Comparing `pydantic_db_backend-0.5.0/pydantic_db_backend/backend.py` & `pydantic_db_backend-0.6.0/pydantic_db_backend/backend.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import re
 from contextvars import ContextVar
 from typing import Type, Dict, List, Tuple
 
 from dotenv import load_dotenv
 from pydantic import BaseModel, Field
 
+from pydantic_db_backend.exceptions import IndexNotExisting
 from pydantic_db_backend.indexes import Index
 from pydantic_db_backend.utils import uid, utcnow, str_to_datetime_if_parseable
 
 log = logging.getLogger(__name__)
 
 backend_context_var = ContextVar('backend_context_var')
 backend_alias_context_var = ContextVar('backend_alias_context_var', default='default')
@@ -57,29 +58,42 @@
         return cls.backend().get_instance(model, uid)
 
     @classmethod
     def put_instance(cls, instance: BackendModel, ignore_revision_conflict: bool = False) -> BackendModel:
         return cls.backend().put_instance(instance, ignore_revision_conflict)
 
     @classmethod
-    def get_uids(cls, model: Type[BackendModel], skip: int = 0, limit: int = 0, query_filter: dict | None = None,
-                 sort: List | None = None) -> List[str]:
+    def get_uids(
+        cls,
+        model: Type[BackendModel],
+        skip: int = 0,
+        limit: int = 0,
+        query_filter: dict | None = None,
+        sort: List | None = None
+    ) -> Tuple[List[str], int] | List[str]:
         return cls.backend().get_uids(model=model, skip=skip, limit=limit, query_filter=query_filter, sort=sort)
 
     @classmethod
     def get_instances(
         cls,
         model: Type[BackendModel],
         skip: int = 0,
         limit: int = 0,
         query_filter: dict | None = None,
         sort: List | None = None,
         max_results: bool | None = False
-    ) -> Tuple[List[BackendModel], int]:
-        return cls.backend().get_instances(model=model, skip=skip, limit=limit, query_filter=query_filter, sort=sort)
+    ) -> Tuple[List[BackendModel], int] | List[BackendModel]:
+        return cls.backend().get_instances(
+            model=model,
+            skip=skip,
+            limit=limit,
+            query_filter=query_filter,
+            sort=sort,
+            max_results=max_results
+        )
 
     @classmethod
     def delete_uid(cls, model: Type[BackendModel], uid: str) -> None:
         return cls.backend().delete_uid(model=model, uid=uid)
 
     @classmethod
     def delete_collection(cls, model: Type[BackendModel]) -> None:
@@ -126,14 +140,24 @@
     ) -> List[Index]:
         if model not in cls._indexes or force_index_creation:
             indexes = cls.create_indexes(model, create_index_kwargs)
             cls._indexes[model] = indexes
         return cls._indexes[model]
 
     @classmethod
+    def get_index_by_name(cls, model: Type[BaseModel], name: str) -> Index:
+        if model not in cls._indexes:
+            raise IndexNotExisting(model=model, name=name)
+        model_indexes = cls._indexes[model]
+        index = next(filter(lambda x: x.name == name, model_indexes), None)
+        if index is None:
+            raise IndexNotExisting(model=model, name=name)
+        return index
+
+    @classmethod
     def create_indexes(cls, model: Type[BaseModel], create_index_kwargs: dict | None) -> List[Index]:
 
         if not hasattr(model, "Config"):
             return True
 
         if not hasattr(model.Config, "backend_indexes"):
             return True
@@ -169,36 +193,46 @@
         cls,
         model: Type[BackendModel],
         skip: int = 0,
         limit: int = 0,
         query_filter: dict | None = None,
         sort: List | None = None,
         max_results: bool | None = False
-    ) -> Tuple[List[str], int]:
+    ) -> Tuple[List[str], int] | List[str]:
         raise NotImplementedError
 
     @classmethod
     def get_instances(
         cls,
         model: Type[BackendModel],
         skip: int = 0,
         limit: int = 0,
         query_filter: dict = None,
         sort: List = None,
         max_results: bool = False,
-    ) -> Tuple[List[BackendModel], int]:
-        ids, max_results = cls.get_uids(
+    ) -> Tuple[List[BackendModel], int] | List[BackendModel]:
+        params = dict(
             model=model,
             skip=skip,
             limit=limit,
             query_filter=query_filter,
             sort=sort,
             max_results=max_results
         )
-        return [cls.get_instance(model, uid=x) for x in ids], max_results
+        if max_results:
+            ids, max_results = cls.get_uids(**params)
+        else:
+            ids = cls.get_uids(**params)
+
+        instances = [cls.get_instance(model, uid=x) for x in ids]
+
+        if max_results:
+            return instances, max_results
+        else:
+            return instances
 
     @classmethod
     def delete_uid(cls, model: Type[BackendModel], uid: str) -> None:
         raise NotImplementedError
 
     @classmethod
     def delete_collection(cls, model: Type[BackendModel]) -> None:
```

### Comparing `pydantic_db_backend-0.5.0/pydantic_db_backend/backends/couchdb.py` & `pydantic_db_backend-0.6.0/pydantic_db_backend/backends/couchdb.py`

 * *Files 16% similar despite different names*

```diff
@@ -75,31 +75,33 @@
 
 
         else:
             pass
 
     @classmethod
     def view_from_aggregation_index(cls, db: couchdb.Database, collection_name: str, index: AggregationIndex):
-        design_document = f"_design/{collection_name}_{index.name}"
+        design_document = index.design_document
+
         if design_document not in db:
             field, func = next(iter(index.spec.items()))
             map_function = f"function (doc) {{ emit(doc.{field}, 1); }}"
+            view_name = f"{index.view_name}"
             # reduce_function = f"function(keys, values, rereduce) {{ return sum(values); }}"
             data = {
-                "_id": design_document,
+                "_id": f"_design/{design_document}",
                 "views": {
-                    (index.name): {
+                    view_name: {
                         "map": map_function,
                         "reduce": func
                     }
                 },
                 "language": "javascript",
                 "options": {"partitioned": False}
             }
-            logging.info(f"creating view {collection_name}_{index.name}/{index.name}")
+            logging.info(f"creating view {design_document}/{view_name}")
             db.save(data)
 
     @classmethod
     def get_db(cls, model: Type[BackendModel]) -> couchdb.Database:
         db_name = cls.collection_name(model)
 
         with cls.alias() as alias:
@@ -170,15 +172,15 @@
         cls,
         model: Type[BackendModel],
         skip: int = 0,
         limit: int = 25,
         query_filter: dict = None,
         sort: List = None,
         max_results: bool | None = False
-    ) -> Tuple[List[str], int]:
+    ) -> Tuple[List[str], int] | List[str]:
 
         # fix 0 limit, since couchdb does not know this
         limit = 9999999 if limit == 0 else limit
 
         if query_filter is None:
             query_filter = {}
 
@@ -192,16 +194,14 @@
             "skip": skip,
             "limit": limit,
             "fields": ['_id']
         }
         if sort is not None:
             find_dict["sort"] = sort
 
-        max_results = 0
-
         try:
             find_result = db.find(find_dict)
         except ServerError as e:
 
             error_code = pydash.get(e, ["args", 0, 0])
 
             if error_code == 400:
@@ -209,26 +209,53 @@
                 # index cache and initiate a new get_db... and a loop
                 cls.indexes(model, dict(db=db), force_index_creation=True)
                 find_result = db.find(find_dict)
             else:
                 raise e
 
         result = [x["_id"] for x in find_result]
-        return result, max_results
+        if max_results:
+            max_results = cls.get_max_results(model, query_filter)
+            return result, max_results
+        else:
+            return result
 
     @classmethod
     def delete_collection(cls, model: Type[BackendModel]) -> None:
         with cls.alias() as alias:
             server = cls._connections[alias].server
             name = cls.collection_name(model)
             if name in server:
                 server.delete(name)
 
         super().delete_collection(model)
 
+    @classmethod
+    def get_max_results(cls, model: Type[BackendModel], query_filter: dict) -> int:
+        # atm it only works with one field,
+        db = cls.get_db(model)
+
+        field = "_".join(list(query_filter.keys()))
+        view_name = f"{field}_sum"
+        index = cls.get_index_by_name(model, view_name)
+
+        design_document = f"aggregation_{view_name}/{view_name}"
+        for row in db.view(design_document, group=True):
+            for k, v in query_filter.items():
+                if isinstance(v, dict):
+                    k = next(iter(v.keys()))
+                    if k == "$eq":
+                        v = v[k]
+                    else:
+                        return 0
+                if v == row.key:
+                    ret = row.value
+                    return ret
+
+
 
 class CouchDbConnectionModel(BaseModel):
     alias: str
     uri: str
     server: couchdb.Server
     dbs: Dict[str, couchdb.Database] = Field(default_factory=dict)
```

### Comparing `pydantic_db_backend-0.5.0/pydantic_db_backend/exceptions/__init__.py` & `pydantic_db_backend-0.6.0/pydantic_db_backend/exceptions/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from typing import Type
+
+from pydantic import BaseModel
 from webexception.webexception import WebException
 
 
 class BackendException(WebException):
     pass
 
 
@@ -20,7 +23,14 @@
 
 
 class AlreadyExists(BackendException):
     status_code: int = 409  # Conflict
 
     def __init__(self, uid: str) -> None:
         super().__init__(f"Entry with uid '{uid}' already exists.", uid=uid)
+
+
+class IndexNotExisting(BackendException):
+    status_code: int = 422
+
+    def __init__(self, model: Type[BaseModel], name: str) -> None:
+        super().__init__(f"No index named '{name}' existing for model '{model}'.", name=name)
```

### Comparing `pydantic_db_backend-0.5.0/pydantic_db_backend/indexes.py` & `pydantic_db_backend-0.6.0/pydantic_db_backend/indexes.py`

 * *Files 26% similar despite different names*

```diff
@@ -25,8 +25,14 @@
     type = "aggregation"
     spec: dict
 
     def __init__(self, name: str, spec: dict) -> None:
         super().__init__(name)
         self.spec = spec
 
+    @property
+    def design_document(self):
+        return f"aggregation_{self.name}"
 
+    @property
+    def view_name(self):
+        return self.name
```

### Comparing `pydantic_db_backend-0.5.0/pydantic_db_backend/utils.py` & `pydantic_db_backend-0.6.0/pydantic_db_backend/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_db_backend-0.5.0/pyproject.toml` & `pydantic_db_backend-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-db-backend"
-version = "0.5.0"
+version = "0.6.0"
 description = ""
 authors = ["Marco Bartel <bsimpson888@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 python-dotenv = "^0.15.0"
```

### Comparing `pydantic_db_backend-0.5.0/PKG-INFO` & `pydantic_db_backend-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-db-backend
-Version: 0.5.0
+Version: 0.6.0
 Summary: 
 Author: Marco Bartel
 Author-email: bsimpson888@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: couchdb
```

