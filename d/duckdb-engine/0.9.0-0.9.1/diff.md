# Comparing `tmp/duckdb_engine-0.9.0.tar.gz` & `tmp/duckdb_engine-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckdb_engine-0.9.0.tar", max compression
+gzip compressed data, was "duckdb_engine-0.9.1.tar", max compression
```

## Comparing `duckdb_engine-0.9.0.tar` & `duckdb_engine-0.9.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1076 2023-06-21 03:45:37.107242 duckdb_engine-0.9.0/LICENSE.txt
--rw-r--r--   0        0        0     5953 2023-06-21 03:45:37.107242 duckdb_engine-0.9.0/README.md
--rw-r--r--   0        0        0        4 2023-06-21 03:45:37.107242 duckdb_engine-0.9.0/duckdb_engine/.hypothesis/examples/f024fc7dfe5f1878/7210af19145ec2a8
--rw-r--r--   0        0        0        1 2023-06-21 03:45:37.111242 duckdb_engine-0.9.0/duckdb_engine/.hypothesis/examples/f024fc7dfe5f1878/bec021b4f368e306
--rw-r--r--   0        0        0    20688 2023-06-21 03:45:37.111242 duckdb_engine-0.9.0/duckdb_engine/.hypothesis/unicode_data/12.1.0/charmap.json.gz
--rw-r--r--   0        0        0    12277 2023-06-21 03:45:37.111242 duckdb_engine-0.9.0/duckdb_engine/__init__.py
--rw-r--r--   0        0        0     1096 2023-06-21 03:45:37.111242 duckdb_engine-0.9.0/duckdb_engine/config.py
--rw-r--r--   0        0        0        0 2023-06-21 03:45:37.111242 duckdb_engine-0.9.0/duckdb_engine/conftest.py
--rw-r--r--   0        0        0     5731 2023-06-21 03:45:37.111242 duckdb_engine-0.9.0/duckdb_engine/datatypes.py
--rw-r--r--   0        0        0        0 2023-06-21 03:45:37.111242 duckdb_engine-0.9.0/duckdb_engine/py.typed
--rw-r--r--   0        0        0        0 2023-06-21 03:45:37.111242 duckdb_engine-0.9.0/duckdb_engine/tests/__init__.py
--rw-r--r--   0        0        0     1209 2023-06-21 03:45:37.111242 duckdb_engine-0.9.0/duckdb_engine/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-06-21 03:45:37.111242 duckdb_engine-0.9.0/duckdb_engine/tests/snapshots/__init__.py
--rw-r--r--   0        0        0      338 2023-06-21 03:45:37.111242 duckdb_engine-0.9.0/duckdb_engine/tests/snapshots/snap_test_basic.py
--rw-r--r--   0        0        0    11631 2023-06-21 03:45:37.111242 duckdb_engine-0.9.0/duckdb_engine/tests/test_basic.py
--rw-r--r--   0        0        0     4016 2023-06-21 03:45:37.111242 duckdb_engine-0.9.0/duckdb_engine/tests/test_datatypes.py
--rw-r--r--   0        0        0      948 2023-06-21 03:45:37.111242 duckdb_engine-0.9.0/duckdb_engine/tests/test_ibis.py
--rw-r--r--   0        0        0     1740 2023-06-21 03:45:37.111242 duckdb_engine-0.9.0/duckdb_engine/tests/test_integration.py
--rw-r--r--   0        0        0     3946 2023-06-21 03:45:37.111242 duckdb_engine-0.9.0/duckdb_engine/tests/test_pandas.py
--rw-r--r--   0        0        0      257 2023-06-21 03:45:37.111242 duckdb_engine-0.9.0/duckdb_engine/tests/util.py
--rw-r--r--   0        0        0     1403 2023-06-21 03:45:37.111242 duckdb_engine-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     6867 1970-01-01 00:00:00.000000 duckdb_engine-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-14 06:49:36.523742 duckdb_engine-0.9.1/LICENSE.txt
+-rw-r--r--   0        0        0     5953 2023-07-14 06:49:36.523742 duckdb_engine-0.9.1/README.md
+-rw-r--r--   0        0        0        4 2023-07-14 06:49:36.523742 duckdb_engine-0.9.1/duckdb_engine/.hypothesis/examples/f024fc7dfe5f1878/7210af19145ec2a8
+-rw-r--r--   0        0        0        1 2023-07-14 06:49:36.523742 duckdb_engine-0.9.1/duckdb_engine/.hypothesis/examples/f024fc7dfe5f1878/bec021b4f368e306
+-rw-r--r--   0        0        0    20688 2023-07-14 06:49:36.523742 duckdb_engine-0.9.1/duckdb_engine/.hypothesis/unicode_data/12.1.0/charmap.json.gz
+-rw-r--r--   0        0        0    12277 2023-07-14 06:49:36.523742 duckdb_engine-0.9.1/duckdb_engine/__init__.py
+-rw-r--r--   0        0        0     1096 2023-07-14 06:49:36.523742 duckdb_engine-0.9.1/duckdb_engine/config.py
+-rw-r--r--   0        0        0        0 2023-07-14 06:49:36.523742 duckdb_engine-0.9.1/duckdb_engine/conftest.py
+-rw-r--r--   0        0        0     5731 2023-07-14 06:49:36.523742 duckdb_engine-0.9.1/duckdb_engine/datatypes.py
+-rw-r--r--   0        0        0        0 2023-07-14 06:49:36.523742 duckdb_engine-0.9.1/duckdb_engine/py.typed
+-rw-r--r--   0        0        0        0 2023-07-14 06:49:36.523742 duckdb_engine-0.9.1/duckdb_engine/tests/__init__.py
+-rw-r--r--   0        0        0     1209 2023-07-14 06:49:36.523742 duckdb_engine-0.9.1/duckdb_engine/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-07-14 06:49:36.523742 duckdb_engine-0.9.1/duckdb_engine/tests/snapshots/__init__.py
+-rw-r--r--   0        0        0      338 2023-07-14 06:49:36.523742 duckdb_engine-0.9.1/duckdb_engine/tests/snapshots/snap_test_basic.py
+-rw-r--r--   0        0        0    11631 2023-07-14 06:49:36.523742 duckdb_engine-0.9.1/duckdb_engine/tests/test_basic.py
+-rw-r--r--   0        0        0     4035 2023-07-14 06:49:36.523742 duckdb_engine-0.9.1/duckdb_engine/tests/test_datatypes.py
+-rw-r--r--   0        0        0      948 2023-07-14 06:49:36.523742 duckdb_engine-0.9.1/duckdb_engine/tests/test_ibis.py
+-rw-r--r--   0        0        0     1740 2023-07-14 06:49:36.523742 duckdb_engine-0.9.1/duckdb_engine/tests/test_integration.py
+-rw-r--r--   0        0        0     3946 2023-07-14 06:49:36.523742 duckdb_engine-0.9.1/duckdb_engine/tests/test_pandas.py
+-rw-r--r--   0        0        0      257 2023-07-14 06:49:36.523742 duckdb_engine-0.9.1/duckdb_engine/tests/util.py
+-rw-r--r--   0        0        0     1403 2023-07-14 06:49:36.523742 duckdb_engine-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     6846 1970-01-01 00:00:00.000000 duckdb_engine-0.9.1/PKG-INFO
```

### Comparing `duckdb_engine-0.9.0/LICENSE.txt` & `duckdb_engine-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.9.0/README.md` & `duckdb_engine-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.9.0/duckdb_engine/.hypothesis/unicode_data/12.1.0/charmap.json.gz` & `duckdb_engine-0.9.1/duckdb_engine/.hypothesis/unicode_data/12.1.0/charmap.json.gz`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.9.0/duckdb_engine/__init__.py` & `duckdb_engine-0.9.1/duckdb_engine/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from sqlalchemy.engine.default import DefaultDialect
 from sqlalchemy.engine.url import URL
 from sqlalchemy.ext.compiler import compiles
 
 from .config import apply_config, get_core_config
 from .datatypes import ISCHEMA_NAMES, register_extension_types
 
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 
 if TYPE_CHECKING:
     from sqlalchemy.base import Connection
     from sqlalchemy.engine.interfaces import _IndexDict
 
 
 register_extension_types()
```

### Comparing `duckdb_engine-0.9.0/duckdb_engine/config.py` & `duckdb_engine-0.9.1/duckdb_engine/config.py`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.9.0/duckdb_engine/datatypes.py` & `duckdb_engine-0.9.1/duckdb_engine/datatypes.py`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.9.0/duckdb_engine/tests/conftest.py` & `duckdb_engine-0.9.1/duckdb_engine/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.9.0/duckdb_engine/tests/test_basic.py` & `duckdb_engine-0.9.1/duckdb_engine/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.9.0/duckdb_engine/tests/test_datatypes.py` & `duckdb_engine-0.9.1/duckdb_engine/tests/test_datatypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     with warnings.catch_warnings() as capture, engine.connect() as conn:
         conn.execute(text("create table t2 as select * from test_all_types()"))
         table = Table("t2", MetaData(), autoload_with=conn)
         for col in table.columns:
             name = col.name
             if name.endswith("_enum") and duckdb.__version__ < "0.7.1":  # type: ignore[attr-defined]
                 continue
-            if "array" in name or "struct" in name or "map" in name:
+            if "array" in name or "struct" in name or "map" in name or "union" in name:
                 assert col.type == sqltypes.NULLTYPE, name
             else:
                 assert col.type != sqltypes.NULLTYPE, name
         assert not capture
 
 
 def test_nested_types(engine: Engine, session: Session) -> None:
```

### Comparing `duckdb_engine-0.9.0/duckdb_engine/tests/test_ibis.py` & `duckdb_engine-0.9.1/duckdb_engine/tests/test_ibis.py`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.9.0/duckdb_engine/tests/test_integration.py` & `duckdb_engine-0.9.1/duckdb_engine/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.9.0/duckdb_engine/tests/test_pandas.py` & `duckdb_engine-0.9.1/duckdb_engine/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.9.0/pyproject.toml` & `duckdb_engine-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "duckdb_engine"
-version = "0.9.0"
+version = "0.9.1"
 description = "SQLAlchemy driver for duckdb"
 authors = ["Elliana <me@mause.me>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Mause/duckdb_engine"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/Mause/duckdb_engine/issues"
 "Changelog" = "https://github.com/Mause/duckdb_engine/releases"
 
 [tool.poetry.dependencies]
 python = ">=3.7"
 duckdb = ">=0.4.0"
 sqlalchemy = ">=1.3.22"
-numpy = "*"
 
 [tool.poetry.dev-dependencies]
+numpy = "*"
 pytest = "^7.3.1"
 pre-commit = "^2.21.0"
 pdbpp = "^0.10.3"
 mypy = "^1.4"
 hypothesis = "^6.75.2"
 pandas = "^1"
 jupysql = "^0.7.8"
```

### Comparing `duckdb_engine-0.9.0/PKG-INFO` & `duckdb_engine-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: duckdb-engine
-Version: 0.9.0
+Version: 0.9.1
 Summary: SQLAlchemy driver for duckdb
 Home-page: https://github.com/Mause/duckdb_engine
 License: MIT
 Author: Elliana
 Author-email: me@mause.me
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: duckdb (>=0.4.0)
-Requires-Dist: numpy
 Requires-Dist: sqlalchemy (>=1.3.22)
 Project-URL: Bug Tracker, https://github.com/Mause/duckdb_engine/issues
 Project-URL: Changelog, https://github.com/Mause/duckdb_engine/releases
 Project-URL: Repository, https://github.com/Mause/duckdb_engine
 Description-Content-Type: text/markdown
 
 # duckdb_engine
```

