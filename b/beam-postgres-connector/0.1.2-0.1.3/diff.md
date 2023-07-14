# Comparing `tmp/beam_postgres_connector-0.1.2.tar.gz` & `tmp/beam_postgres_connector-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beam_postgres_connector-0.1.2.tar", max compression
+gzip compressed data, was "beam_postgres_connector-0.1.3.tar", max compression
```

## Comparing `beam_postgres_connector-0.1.2.tar` & `beam_postgres_connector-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1061 2023-04-11 02:59:31.754263 beam_postgres_connector-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0     2349 2023-05-19 11:06:08.366962 beam_postgres_connector-0.1.2/README.md
--rw-r--r--   0        0        0     2583 2023-07-01 02:13:07.706103 beam_postgres_connector-0.1.2/pyproject.toml
--rwxr-xr-x   0        0        0       22 2023-05-19 11:56:11.896780 beam_postgres_connector-0.1.2/src/beam_postgres/__init__.py
--rwxr-xr-x   0        0        0     5025 2023-06-30 13:49:21.196890 beam_postgres_connector-0.1.2/src/beam_postgres/client.py
--rwxr-xr-x   0        0        0      417 2023-04-10 09:57:56.818016 beam_postgres_connector-0.1.2/src/beam_postgres/errors.py
--rwxr-xr-x   0        0        0     4616 2023-06-30 13:49:21.196890 beam_postgres_connector-0.1.2/src/beam_postgres/io.py
--rwxr-xr-x   0        0        0     2717 2023-05-19 11:56:34.495107 beam_postgres_connector-0.1.2/src/beam_postgres/source.py
--rwxr-xr-x   0        0        0     4018 2023-04-10 10:15:56.339706 beam_postgres_connector-0.1.2/src/beam_postgres/splitters.py
--rwxr-xr-x   0        0        0      296 2023-04-10 09:58:49.818002 beam_postgres_connector-0.1.2/src/beam_postgres/utils.py
--rw-r--r--   0        0        0     3221 1970-01-01 00:00:00.000000 beam_postgres_connector-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-04-11 02:59:31.754263 beam_postgres_connector-0.1.3/LICENSE.txt
+-rw-r--r--   0        0        0     2349 2023-05-19 11:06:08.366962 beam_postgres_connector-0.1.3/README.md
+-rw-r--r--   0        0        0     2583 2023-07-14 14:14:05.260260 beam_postgres_connector-0.1.3/pyproject.toml
+-rwxr-xr-x   0        0        0       22 2023-05-19 11:56:11.896780 beam_postgres_connector-0.1.3/src/beam_postgres/__init__.py
+-rwxr-xr-x   0        0        0     5501 2023-07-14 13:46:09.470646 beam_postgres_connector-0.1.3/src/beam_postgres/client.py
+-rwxr-xr-x   0        0        0      417 2023-04-10 09:57:56.818016 beam_postgres_connector-0.1.3/src/beam_postgres/errors.py
+-rwxr-xr-x   0        0        0     4616 2023-06-30 13:49:21.196890 beam_postgres_connector-0.1.3/src/beam_postgres/io.py
+-rwxr-xr-x   0        0        0     2717 2023-05-19 11:56:34.495107 beam_postgres_connector-0.1.3/src/beam_postgres/source.py
+-rwxr-xr-x   0        0        0     4018 2023-04-10 10:15:56.339706 beam_postgres_connector-0.1.3/src/beam_postgres/splitters.py
+-rwxr-xr-x   0        0        0      296 2023-04-10 09:58:49.818002 beam_postgres_connector-0.1.3/src/beam_postgres/utils.py
+-rw-r--r--   0        0        0     3221 1970-01-01 00:00:00.000000 beam_postgres_connector-0.1.3/PKG-INFO
```

### Comparing `beam_postgres_connector-0.1.2/LICENSE.txt` & `beam_postgres_connector-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `beam_postgres_connector-0.1.2/README.md` & `beam_postgres_connector-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `beam_postgres_connector-0.1.2/pyproject.toml` & `beam_postgres_connector-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beam-postgres-connector"
-version = "0.1.2"
+version = "0.1.3"
 description = "An io connector for PostgreSQL read/write in Apache Beam pipelines."
 authors = ["satokiyo <satokiyo@loop8.biz>"]
 readme = "README.md"
 packages = [
     {include = "beam_postgres", from = "src"},
 ]
 license = "MIT"
```

### Comparing `beam_postgres_connector-0.1.2/src/beam_postgres/client.py` & `beam_postgres_connector-0.1.3/src/beam_postgres/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from contextlib import contextmanager
 from logging import INFO, getLogger
 import re
-from typing import Dict, Generator, List
+from typing import Dict, Generator
 
 from psycopg2 import Error as PostgresConnectorError
 import psycopg2.extras
 
 from beam_postgres.errors import BeamPostgresClientError
 
 _SELECT_STATEMENT = "SELECT"
@@ -31,15 +31,15 @@
 
         Returns:
             dict record
 
         Raises:
             ~beam_postgres.errors.BeamPostgresClientError
         """
-        self._validate_query(query, [_SELECT_STATEMENT])
+        self._validate_query(query, _SELECT_STATEMENT)
 
         with get_connection(self._config) as conn:
             # buffered is false because it can be assumed that the data size is too large
             cur = conn.cursor(cursor_factory=psycopg2.extras.DictCursor)
 
             try:
                 cur.execute(query)
@@ -64,15 +64,15 @@
 
         Returns:
             the total number of records
 
         Raises:
             ~beam_postgres.errors.BeamPostgresClientError
         """
-        self._validate_query(query, [_SELECT_STATEMENT])
+        self._validate_query(query, _SELECT_STATEMENT)
         count_query = f"EXPLAIN SELECT * FROM ({query}) as subq"
 
         with get_connection(self._config) as conn:
             cur = conn.cursor()
 
             try:
                 cur.execute(count_query)
@@ -106,15 +106,15 @@
 
         Args:
             query: query with insert or update statement
 
         Raises:
             ~beam_postgres.errors.BeamPostgresClientError
         """
-        self._validate_query(query, [_INSERT_STATEMENT])
+        self._validate_query(query, _INSERT_STATEMENT)
 
         with get_connection(self._config) as conn:
             cur = conn.cursor()
 
             try:
                 cur.execute(query)
                 conn.commit()
@@ -133,24 +133,38 @@
         for required in required_keys:
             if required not in config.keys():
                 raise BeamPostgresClientError(
                     "Config is not satisfied. required: %s", required
                 )
 
     @staticmethod
-    def _validate_query(query: str, statements: List[str]) -> None:
-        query = query.lstrip()
-
-        for statement in statements:
-            if statement and not query.lower().startswith(statement.lower()):
-                raise BeamPostgresClientError(
-                    "Query expected to start with %s statement. Query: %s",
-                    statement,
-                    query,
-                )
+    def _validate_query(query: str, statement: str) -> None:
+        def _remove_comments_and_cte(query):
+            # delete comments
+            query = re.sub(r"--.*\n", " ", query)
+            query = re.sub(r"/\*[.\s].*\*/", " ", query, flags=re.DOTALL)
+            # delete new line
+            query = query.replace("\n", " ")
+            # delete cte clause
+            query = re.sub(
+                r"WITH\s+(?:\w+\s+AS\s+\(.+?\)\s*,?\s*)+",
+                "",
+                query,
+                flags=re.IGNORECASE,
+            )
+            return query.strip()
+
+        cleansed_query = _remove_comments_and_cte(query)
+
+        if statement and not cleansed_query.lower().startswith(statement.lower()):
+            raise BeamPostgresClientError(
+                "Query expected to start with %s statement. Query: %s",
+                statement,
+                query,
+            )
 
 
 @contextmanager
 def get_connection(config: Dict):
     """A wrapper object to connect postgres."""
     try:
         conn = psycopg2.connect(**config)
```

### Comparing `beam_postgres_connector-0.1.2/src/beam_postgres/io.py` & `beam_postgres_connector-0.1.3/src/beam_postgres/io.py`

 * *Files identical despite different names*

### Comparing `beam_postgres_connector-0.1.2/src/beam_postgres/source.py` & `beam_postgres_connector-0.1.3/src/beam_postgres/source.py`

 * *Files identical despite different names*

### Comparing `beam_postgres_connector-0.1.2/src/beam_postgres/splitters.py` & `beam_postgres_connector-0.1.3/src/beam_postgres/splitters.py`

 * *Files identical despite different names*

### Comparing `beam_postgres_connector-0.1.2/PKG-INFO` & `beam_postgres_connector-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beam-postgres-connector
-Version: 0.1.2
+Version: 0.1.3
 Summary: An io connector for PostgreSQL read/write in Apache Beam pipelines.
 Home-page: https://github.com/satokiyo/beam-postgres-connector
 License: MIT
 Keywords: apache beam,beam,postgres,postgresql
 Author: satokiyo
 Author-email: satokiyo@loop8.biz
 Requires-Python: >=3.8.1,<4.0.0
```

