# Comparing `tmp/nsj_multi_database_lib-0.3.5.tar.gz` & `tmp/nsj_multi_database_lib-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsj_multi_database_lib-0.3.5.tar", max compression
+gzip compressed data, was "nsj_multi_database_lib-0.3.6.tar", max compression
```

## Comparing `nsj_multi_database_lib-0.3.5.tar` & `nsj_multi_database_lib-0.3.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       74 2023-07-03 15:14:51.914114 nsj_multi_database_lib-0.3.5/nsj_multi_database_lib/__init__.py
--rw-r--r--   0        0        0      288 2023-07-03 15:14:51.914114 nsj_multi_database_lib-0.3.5/nsj_multi_database_lib/crypt_key_sample.py
--rw-r--r--   0        0        0      268 2023-07-03 15:14:51.914114 nsj_multi_database_lib-0.3.5/nsj_multi_database_lib/crypt_util.py
--rw-r--r--   0        0        0        0 2023-07-03 15:14:51.914114 nsj_multi_database_lib-0.3.5/nsj_multi_database_lib/dao/__init__.py
--rw-r--r--   0        0        0     1989 2023-07-03 15:14:51.914114 nsj_multi_database_lib-0.3.5/nsj_multi_database_lib/dao/database.py
--rw-r--r--   0        0        0      838 2023-07-03 15:14:51.914114 nsj_multi_database_lib-0.3.5/nsj_multi_database_lib/dao/usuario.py
--rw-r--r--   0        0        0     2230 2023-07-14 19:34:54.832503 nsj_multi_database_lib-0.3.5/nsj_multi_database_lib/db_pool_config.py
--rw-r--r--   0        0        0        0 2023-07-03 15:14:51.914114 nsj_multi_database_lib-0.3.5/nsj_multi_database_lib/decorator/__init__.py
--rw-r--r--   0        0        0     3689 2023-07-03 15:14:51.914114 nsj_multi_database_lib-0.3.5/nsj_multi_database_lib/decorator/multi_database.py
--rw-r--r--   0        0        0        0 2023-07-03 15:14:51.918114 nsj_multi_database_lib-0.3.5/nsj_multi_database_lib/dto/__init__.py
--rw-r--r--   0        0        0     1536 2023-07-03 15:14:51.918114 nsj_multi_database_lib-0.3.5/nsj_multi_database_lib/dto/database.py
--rw-r--r--   0        0        0        0 2023-07-03 15:14:51.918114 nsj_multi_database_lib-0.3.5/nsj_multi_database_lib/entity/__init__.py
--rw-r--r--   0        0        0     1036 2023-07-03 15:14:51.918114 nsj_multi_database_lib-0.3.5/nsj_multi_database_lib/entity/database.py
--rw-r--r--   0        0        0      930 2023-07-03 15:14:51.918114 nsj_multi_database_lib-0.3.5/nsj_multi_database_lib/env_config.py
--rw-r--r--   0        0        0       45 2023-07-03 15:14:51.918114 nsj_multi_database_lib-0.3.5/nsj_multi_database_lib/exception.py
--rw-r--r--   0        0        0     1837 2023-07-03 15:14:51.918114 nsj_multi_database_lib-0.3.5/nsj_multi_database_lib/injector_factory.py
--rw-r--r--   0        0        0      913 2023-07-03 15:14:51.918114 nsj_multi_database_lib-0.3.5/nsj_multi_database_lib/settings.py
--rw-r--r--   0        0        0      592 2023-07-14 19:34:59.083978 nsj_multi_database_lib-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      876 1970-01-01 00:00:00.000000 nsj_multi_database_lib-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0       74 2023-07-03 15:14:51.914114 nsj_multi_database_lib-0.3.6/nsj_multi_database_lib/__init__.py
+-rw-r--r--   0        0        0      288 2023-07-03 15:14:51.914114 nsj_multi_database_lib-0.3.6/nsj_multi_database_lib/crypt_key_sample.py
+-rw-r--r--   0        0        0      268 2023-07-03 15:14:51.914114 nsj_multi_database_lib-0.3.6/nsj_multi_database_lib/crypt_util.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:14:51.914114 nsj_multi_database_lib-0.3.6/nsj_multi_database_lib/dao/__init__.py
+-rw-r--r--   0        0        0     1989 2023-07-03 15:14:51.914114 nsj_multi_database_lib-0.3.6/nsj_multi_database_lib/dao/database.py
+-rw-r--r--   0        0        0      838 2023-07-03 15:14:51.914114 nsj_multi_database_lib-0.3.6/nsj_multi_database_lib/dao/usuario.py
+-rw-r--r--   0        0        0     2747 2023-07-14 19:57:45.314134 nsj_multi_database_lib-0.3.6/nsj_multi_database_lib/db_pool_config.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:14:51.914114 nsj_multi_database_lib-0.3.6/nsj_multi_database_lib/decorator/__init__.py
+-rw-r--r--   0        0        0     3689 2023-07-03 15:14:51.914114 nsj_multi_database_lib-0.3.6/nsj_multi_database_lib/decorator/multi_database.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:14:51.918114 nsj_multi_database_lib-0.3.6/nsj_multi_database_lib/dto/__init__.py
+-rw-r--r--   0        0        0     1536 2023-07-03 15:14:51.918114 nsj_multi_database_lib-0.3.6/nsj_multi_database_lib/dto/database.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:14:51.918114 nsj_multi_database_lib-0.3.6/nsj_multi_database_lib/entity/__init__.py
+-rw-r--r--   0        0        0     1036 2023-07-03 15:14:51.918114 nsj_multi_database_lib-0.3.6/nsj_multi_database_lib/entity/database.py
+-rw-r--r--   0        0        0      930 2023-07-03 15:14:51.918114 nsj_multi_database_lib-0.3.6/nsj_multi_database_lib/env_config.py
+-rw-r--r--   0        0        0       45 2023-07-03 15:14:51.918114 nsj_multi_database_lib-0.3.6/nsj_multi_database_lib/exception.py
+-rw-r--r--   0        0        0     1837 2023-07-03 15:14:51.918114 nsj_multi_database_lib-0.3.6/nsj_multi_database_lib/injector_factory.py
+-rw-r--r--   0        0        0      913 2023-07-03 15:14:51.918114 nsj_multi_database_lib-0.3.6/nsj_multi_database_lib/settings.py
+-rw-r--r--   0        0        0      592 2023-07-14 19:57:50.049920 nsj_multi_database_lib-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0      876 1970-01-01 00:00:00.000000 nsj_multi_database_lib-0.3.6/PKG-INFO
```

### Comparing `nsj_multi_database_lib-0.3.5/nsj_multi_database_lib/dao/database.py` & `nsj_multi_database_lib-0.3.6/nsj_multi_database_lib/dao/database.py`

 * *Files identical despite different names*

### Comparing `nsj_multi_database_lib-0.3.5/nsj_multi_database_lib/dao/usuario.py` & `nsj_multi_database_lib-0.3.6/nsj_multi_database_lib/dao/usuario.py`

 * *Files identical despite different names*

### Comparing `nsj_multi_database_lib-0.3.5/nsj_multi_database_lib/db_pool_config.py` & `nsj_multi_database_lib-0.3.6/nsj_multi_database_lib/db_pool_config.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,29 +20,68 @@
         # https://stackoverflow.com/questions/14783505/encoding-error-with-sqlalchemy-and-postgresql
         # o sqlalchemy usa, por padrão, o encoding da configuração do banco de dados
         # , client_encoding='utf8'
     )
     return db_pool
 
 
+def create_url(
+    username: str,
+    password: str,
+    host: str,
+    port: str,
+    database: str,
+    db_dialect: str = "postgresql+pg8000",
+):
+    return sqlalchemy.engine.URL.create(
+        db_dialect,
+        username=username,
+        password=password,
+        host=host,
+        port=port,
+        database=database,
+    )
+
+
 def create_external_pool_with_default_credentials():
     external_database = g.external_database
-    external_database_conn_url = f'postgresql+pg8000://{EnvConfig.instance().default_external_database_user}:{EnvConfig.instance().default_external_database_password}@{external_database["host"]}:{external_database["port"]}/{external_database["name"]}'
+    external_database_conn_url = create_url(
+        username=EnvConfig.instance().default_external_database_user,
+        password=EnvConfig.instance().default_external_database_password,
+        host=external_database["host"],
+        port=external_database["port"],
+        database=external_database["name"],
+    )
     line = re.sub(r":[^/]+@", ":********@", external_database_conn_url)
     get_logger().debug(f"URL Conexao: {line}")
+
     external_db_pool = create_pool(external_database_conn_url)
     return external_db_pool
 
 
 def create_external_pool():
     external_database = g.external_database
-    external_database_conn_url = f'postgresql+pg8000://{external_database["user"]}:{external_database["password"]}@{external_database["host"]}:{external_database["port"]}/{external_database["name"]}'
+    external_database_conn_url = create_url(
+        username=external_database["user"],
+        password=external_database["password"],
+        host=external_database["host"],
+        port=external_database["port"],
+        database=external_database["name"],
+    )
     line = re.sub(r":[^/]+@", ":********@", external_database_conn_url)
     get_logger().debug(f"URL Conexao: {line}")
+
     external_db_pool = create_pool(external_database_conn_url)
     return external_db_pool
 
 
-internal_database_conn_url = f"postgresql+pg8000://{EnvConfig.instance().multi_database_user}:{EnvConfig.instance().multi_database_password}@{EnvConfig.instance().multi_database_host}:{EnvConfig.instance().multi_database_port}/{EnvConfig.instance().multi_database_name}"
+internal_database_conn_url = create_url(
+    username=EnvConfig.instance().multi_database_user,
+    password=EnvConfig.instance().multi_database_password,
+    host=EnvConfig.instance().multi_database_host,
+    port=EnvConfig.instance().multi_database_port,
+    database=EnvConfig.instance().multi_database_name,
+)
 line = re.sub(r":[^/]+@", ":********@", internal_database_conn_url)
 get_logger().debug(f"URL Conexao: {line}")
+
 internal_db_pool = create_pool(internal_database_conn_url)
```

### Comparing `nsj_multi_database_lib-0.3.5/nsj_multi_database_lib/decorator/multi_database.py` & `nsj_multi_database_lib-0.3.6/nsj_multi_database_lib/decorator/multi_database.py`

 * *Files identical despite different names*

### Comparing `nsj_multi_database_lib-0.3.5/nsj_multi_database_lib/dto/database.py` & `nsj_multi_database_lib-0.3.6/nsj_multi_database_lib/dto/database.py`

 * *Files identical despite different names*

### Comparing `nsj_multi_database_lib-0.3.5/nsj_multi_database_lib/entity/database.py` & `nsj_multi_database_lib-0.3.6/nsj_multi_database_lib/entity/database.py`

 * *Files identical despite different names*

### Comparing `nsj_multi_database_lib-0.3.5/nsj_multi_database_lib/env_config.py` & `nsj_multi_database_lib-0.3.6/nsj_multi_database_lib/env_config.py`

 * *Files identical despite different names*

### Comparing `nsj_multi_database_lib-0.3.5/nsj_multi_database_lib/injector_factory.py` & `nsj_multi_database_lib-0.3.6/nsj_multi_database_lib/injector_factory.py`

 * *Files identical despite different names*

### Comparing `nsj_multi_database_lib-0.3.5/nsj_multi_database_lib/settings.py` & `nsj_multi_database_lib-0.3.6/nsj_multi_database_lib/settings.py`

 * *Files identical despite different names*

### Comparing `nsj_multi_database_lib-0.3.5/pyproject.toml` & `nsj_multi_database_lib-0.3.6/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nsj-multi-database-lib"
-version = "0.3.5"
+version = "0.3.6"
 description = "Modulo que permite o uso de múltiplos bancos de dados na mesma aplicação."
 authors = ["Wallace Pinho <wallacepinho@nasajon.com.br>"]
 
 [tool.poetry.dependencies]
 python = "^3.6"
 Flask = "*"
 nsj_rest_lib = ">=0.1.6, <2.0.0"
```

### Comparing `nsj_multi_database_lib-0.3.5/PKG-INFO` & `nsj_multi_database_lib-0.3.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj-multi-database-lib
-Version: 0.3.5
+Version: 0.3.6
 Summary: Modulo que permite o uso de múltiplos bancos de dados na mesma aplicação.
 Author: Wallace Pinho
 Author-email: wallacepinho@nasajon.com.br
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

