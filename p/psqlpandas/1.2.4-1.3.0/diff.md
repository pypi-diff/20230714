# Comparing `tmp/psqlpandas-1.2.4.tar.gz` & `tmp/psqlpandas-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psqlpandas-1.2.4.tar", max compression
+gzip compressed data, was "psqlpandas-1.3.0.tar", max compression
```

## Comparing `psqlpandas-1.2.4.tar` & `psqlpandas-1.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      900 2023-07-11 10:16:31.854836 psqlpandas-1.2.4/LICENSE
--rw-r--r--   0        0        0      199 2023-07-11 10:16:31.854836 psqlpandas-1.2.4/README.md
--rw-r--r--   0        0        0        0 2023-07-11 10:16:31.877836 psqlpandas-1.2.4/psqlpandas/__init__.py
--rw-r--r--   0        0        0       22 2023-07-11 10:16:31.855836 psqlpandas-1.2.4/psqlpandas/__version__.py
--rw-r--r--   0        0        0     7939 2023-07-11 10:16:31.855836 psqlpandas-1.2.4/psqlpandas/postgresql.py
--rw-r--r--   0        0        0       88 2023-07-11 10:16:31.855836 psqlpandas-1.2.4/psqlpandas/scripts/script.py
--rw-r--r--   0        0        0     3091 2023-07-11 10:16:31.855836 psqlpandas-1.2.4/psqlpandas/tables.py
--rw-r--r--   0        0        0     1908 2023-07-11 10:16:31.855836 psqlpandas-1.2.4/pyproject.toml
--rw-r--r--   0        0        0      994 1970-01-01 00:00:00.000000 psqlpandas-1.2.4/setup.py
--rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 psqlpandas-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0      900 2023-07-14 14:48:26.587735 psqlpandas-1.3.0/LICENSE
+-rw-r--r--   0        0        0      199 2023-07-14 14:48:26.587735 psqlpandas-1.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-14 14:48:26.611734 psqlpandas-1.3.0/psqlpandas/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-14 14:48:26.588735 psqlpandas-1.3.0/psqlpandas/__version__.py
+-rw-r--r--   0        0        0     8220 2023-07-14 14:48:26.588735 psqlpandas-1.3.0/psqlpandas/postgresql.py
+-rw-r--r--   0        0        0       88 2023-07-14 14:48:26.588735 psqlpandas-1.3.0/psqlpandas/scripts/script.py
+-rw-r--r--   0        0        0     3091 2023-07-14 14:48:26.588735 psqlpandas-1.3.0/psqlpandas/tables.py
+-rw-r--r--   0        0        0     1886 2023-07-14 14:48:26.588735 psqlpandas-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 psqlpandas-1.3.0/setup.py
+-rw-r--r--   0        0        0      920 1970-01-01 00:00:00.000000 psqlpandas-1.3.0/PKG-INFO
```

### Comparing `psqlpandas-1.2.4/LICENSE` & `psqlpandas-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `psqlpandas-1.2.4/psqlpandas/postgresql.py` & `psqlpandas-1.3.0/psqlpandas/postgresql.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,56 +1,54 @@
 from typing import List, Dict, Tuple, Any
 import logging
 
 import pandas as pd
 import numpy as np
 import psycopg2
 import psycopg2.extras as pgex
-from sqlalchemy import create_engine, text
 
 
 class PostgresqlDatabaseConnector:
     def __init__(
         self, dbname: str, user: str, host: str, port: str, password: str
     ) -> None:
         self._conn = psycopg2.connect(
             user=user,
             password=password,
             host=host,
             port=port,
             database=dbname,
         )
-        self._sqlalchemy_conn = create_engine(
-            f"postgresql+psycopg2://{user}:{password}@{host}:{port}/{dbname}"
-        )
+        self._db_uri = f"postgresql+psycopg2://{user}:{password}@{host}:{port}/{dbname}"
 
     def __del__(self) -> None:
         self._conn.close()
-        self._sqlalchemy_conn.dispose()
 
     @staticmethod
     def execute_values(cursor, query, tuples):
         return pgex.execute_values(cursor, query, tuples)
 
-    def read(self, query: str) -> List[Tuple[str]]:
+    def read(self, query: str, params: Tuple[Any] | None = None) -> List[Tuple[str]]:
         """
         Reads values from database.
 
         NOTE: around 3x faster than self.read_df
 
         Args:
             query (str): select query to be executed
+            params (Tuple[Any], optional): bind parameters to pass to the query. Defaults to None.
 
         Returns:
             List[Tuple[str]]: list of rows retrieved
         """
         cur = self._conn.cursor()
+        params = params if params is not None else tuple()
 
         try:
-            cur.execute(query)
+            cur.execute(query, params)
             data = cur.fetchall()
         except Exception as e:
             logging.error(f"Error while reading query: {query}")
             logging.error(e)
             cur.close()
             raise
         else:
@@ -58,31 +56,34 @@
             return data
 
     def read_df(
         self,
         query: str,
         parse_dates: List[str] | str | None = None,
         uppercase_colnames: bool = False,
+        params: Tuple[Any] | None = None,
     ) -> pd.DataFrame:
         """
         Reads values from database directly into pandas dataframe
 
         NOTE: generally slower than self.read. But can be usefult for automatic casting of types (including dates).
 
         Args:
             query (str): select query to be executed
             parse_dates (List[str] | str | None, optional): columns to be parsed at dates. Defaults to None.
-            uppercase_colnames (bool): whether to return uppercase colnames. Defaults to False.
+            uppercase_colnames (bool, optional): whether to return uppercase colnames. Defaults to False.
+            params (Tuple[Any], optional): bind parameters to pass to the query. Defaults to None.
 
         Returns:
             pd.DataFrame: dataframe of data retrieved
         """
+        params = params if params is not None else tuple()
         try:
             data = pd.read_sql_query(
-                text(query), con=self._sqlalchemy_conn, parse_dates=parse_dates
+                query, con=self._db_uri, parse_dates=parse_dates, params=params
             )
             if uppercase_colnames:
                 data.columns = data.columns.str.upper()
             return data
         except Exception as e:
             logging.error(f"Error while reading query: {query}")
             logging.error(e)
```

### Comparing `psqlpandas-1.2.4/psqlpandas/tables.py` & `psqlpandas-1.3.0/psqlpandas/tables.py`

 * *Files identical despite different names*

### Comparing `psqlpandas-1.2.4/pyproject.toml` & `psqlpandas-1.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [tool.poetry]
 name = "psqlpandas"
-version = "1.2.4"
+version = "1.3.0"
 description = "Utilities to communicate with postgresql database through pandas dataframes."
 authors = ["Mattia Tantardini <mattia.tantardini@gmail.com>"]
 readme = "README.md"
 keywords = ["postgresql", "pandas"]
 classifiers = [
     "Programming Language :: Python :: 3.10",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-sqlalchemy = "^2.0.3"
 numpy = "^1.0.0"
 psycopg2 = "^2.9.5"
 pandas = "^2.0.1"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^2.20.0"
 commitizen = "^2.35.0"
```

### Comparing `psqlpandas-1.2.4/setup.py` & `psqlpandas-1.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,22 +4,19 @@
 packages = \
 ['psqlpandas', 'psqlpandas.scripts']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['numpy>=1.0.0,<2.0.0',
- 'pandas>=2.0.1,<3.0.0',
- 'psycopg2>=2.9.5,<3.0.0',
- 'sqlalchemy>=2.0.3,<3.0.0']
+['numpy>=1.0.0,<2.0.0', 'pandas>=2.0.1,<3.0.0', 'psycopg2>=2.9.5,<3.0.0']
 
 setup_kwargs = {
     'name': 'psqlpandas',
-    'version': '1.2.4',
+    'version': '1.3.0',
     'description': 'Utilities to communicate with postgresql database through pandas dataframes.',
     'long_description': '# psqlpandas\nUtilities to communicate with postgresql database through pandas dataframes.\n\n## Installation\n```\npip install psqlpandas\n```\n\n## Usage\nDescribe how to launch and use psqlpandas project.\n',
     'author': 'Mattia Tantardini',
     'author_email': 'mattia.tantardini@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `psqlpandas-1.2.4/PKG-INFO` & `psqlpandas-1.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: psqlpandas
-Version: 1.2.4
+Version: 1.3.0
 Summary: Utilities to communicate with postgresql database through pandas dataframes.
 Keywords: postgresql,pandas
 Author: Mattia Tantardini
 Author-email: mattia.tantardini@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: numpy (>=1.0.0,<2.0.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: psycopg2 (>=2.9.5,<3.0.0)
-Requires-Dist: sqlalchemy (>=2.0.3,<3.0.0)
 Description-Content-Type: text/markdown
 
 # psqlpandas
 Utilities to communicate with postgresql database through pandas dataframes.
 
 ## Installation
 ```
```

