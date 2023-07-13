# Comparing `tmp/pzSQL-0.0.7.3.tar.gz` & `tmp/pzSQL-0.0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pzSQL-0.0.7.3.tar", last modified: Wed Jun  2 15:02:24 2021, max compression
+gzip compressed data, was "pzSQL-0.0.7.7.tar", last modified: Thu Jul 13 23:42:07 2023, max compression
```

## Comparing `pzSQL-0.0.7.3.tar` & `pzSQL-0.0.7.7.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2021-06-02 15:02:24.666345 pzSQL-0.0.7.3/
--rw-rw-rw-   0        0        0      286 2021-06-02 15:02:24.665347 pzSQL-0.0.7.3/PKG-INFO
--rw-rw-rw-   0        0        0      243 2021-05-25 15:26:51.000000 pzSQL-0.0.7.3/README.md
-drwxrwxrwx   0        0        0        0 2021-06-02 15:02:24.637420 pzSQL-0.0.7.3/pzSQL/
--rw-rw-rw-   0        0        0        0 2021-05-17 02:20:27.000000 pzSQL-0.0.7.3/pzSQL/__init__.py
--rw-rw-rw-   0        0        0        2 2021-05-25 15:10:56.000000 pzSQL-0.0.7.3/pzSQL/connect.py
--rw-rw-rw-   0        0        0     2248 2021-06-02 14:57:56.000000 pzSQL-0.0.7.3/pzSQL/pzSQL.py
-drwxrwxrwx   0        0        0        0 2021-06-02 15:02:24.663350 pzSQL-0.0.7.3/pzSQL.egg-info/
--rw-rw-rw-   0        0        0      286 2021-06-02 15:02:24.000000 pzSQL-0.0.7.3/pzSQL.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2021-06-02 15:02:24.000000 pzSQL-0.0.7.3/pzSQL.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-06-02 15:02:24.000000 pzSQL-0.0.7.3/pzSQL.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2021-06-02 15:02:24.000000 pzSQL-0.0.7.3/pzSQL.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2021-06-02 15:02:24.000000 pzSQL-0.0.7.3/pzSQL.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-06-02 15:02:24.667340 pzSQL-0.0.7.3/setup.cfg
--rw-rw-rw-   0        0        0      418 2021-06-02 15:02:19.000000 pzSQL-0.0.7.3/setup.py
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-13 23:42:07.563473 pzSQL-0.0.7.7/
+-rw-r--r--   0 jreyno     (501) staff       (20)      219 2023-07-13 23:42:07.563359 pzSQL-0.0.7.7/PKG-INFO
+-rw-r--r--   0 jreyno     (501) staff       (20)      427 2023-07-13 23:26:55.000000 pzSQL-0.0.7.7/README.md
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-13 23:42:07.562604 pzSQL-0.0.7.7/pzSQL/
+-rw-r--r--   0 jreyno     (501) staff       (20)        0 2023-07-13 23:14:03.000000 pzSQL-0.0.7.7/pzSQL/__init__.py
+-rw-r--r--   0 jreyno     (501) staff       (20)     2847 2023-07-13 23:37:31.000000 pzSQL-0.0.7.7/pzSQL/pzSQL.py
+drwxr-xr-x   0 jreyno     (501) staff       (20)        0 2023-07-13 23:42:07.563212 pzSQL-0.0.7.7/pzSQL.egg-info/
+-rw-r--r--   0 jreyno     (501) staff       (20)      219 2023-07-13 23:42:07.000000 pzSQL-0.0.7.7/pzSQL.egg-info/PKG-INFO
+-rw-r--r--   0 jreyno     (501) staff       (20)      195 2023-07-13 23:42:07.000000 pzSQL-0.0.7.7/pzSQL.egg-info/SOURCES.txt
+-rw-r--r--   0 jreyno     (501) staff       (20)        1 2023-07-13 23:42:07.000000 pzSQL-0.0.7.7/pzSQL.egg-info/dependency_links.txt
+-rw-r--r--   0 jreyno     (501) staff       (20)       16 2023-07-13 23:42:07.000000 pzSQL-0.0.7.7/pzSQL.egg-info/requires.txt
+-rw-r--r--   0 jreyno     (501) staff       (20)        6 2023-07-13 23:42:07.000000 pzSQL-0.0.7.7/pzSQL.egg-info/top_level.txt
+-rw-r--r--   0 jreyno     (501) staff       (20)       38 2023-07-13 23:42:07.563503 pzSQL-0.0.7.7/setup.cfg
+-rw-r--r--   0 jreyno     (501) staff       (20)      418 2023-07-13 23:41:17.000000 pzSQL-0.0.7.7/setup.py
```

### Comparing `pzSQL-0.0.7.3/pzSQL/pzSQL.py` & `pzSQL-0.0.7.7/pzSQL/pzSQL.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,74 +1,86 @@
-import psycopg2 as pgsql
-
-
-class Db:
-
-    def __init__(self, name, user, code, host):
-
-        self.name = name
-        self.user = user
-        self.code = code
-        self.host = host
-        self.cursor = self.connection.cursor()
-
-    @property
-    def connection(self):
-
-        return pgsql.connect(dbname=self.name, user=self.user, password=self.code, host=self.host)
-
-    def close_connection(self):
-        """closes connection to database"""
-        self.connection.close()
-
-    def select(self, query_string) -> list:
-        """executes query and returns data"""
-        self.cursor.execute(query_string)
-        return self.cursor.fetchall()
-
-    def select_where(self, query_string, params):
-
-        self.cursor.execute(query_string, params)
-        return self.cursor.fetchall()
-
-    def insert(self, statement, values):
-        """writes query to database"""
-        return self.cursor.execute(statement, values)
-
-    def commit_transactions(self):
-        """commits transaction to database"""
-        self.connection.commit()
-
-    def commit_and_close_connection(self):
-        """commits transaction and closes connection"""
-        self.commit_transactions()
-        self.connection.close()
-
-    def insert_and_commit(self, statement, values):
-        """writes query to database and commits transaction"""
-        insert = self.insert(statement, values)
-        self.commit_transactions()
-        return insert
-    
-    def restart_connection(self):
-        """closes connection and starts new one"""
-        self.connection.close()
-        self.connection
-
-    def rollback(self):
-        """rollsback statements"""
-        self.cursor.execute("ROLLBACK")
-
-    def update(self, statement, values):
-        """updates row(s) in database"""
-        return self.cusrsore.execute(statement, tuple(_ for _ in row[1:]) + (row[0],))
-
-    def update_and_commit(self, statement, values):
-        """updates row(s) in database and commits transactions"""
-        update = self.update(statement, values)
-        self.commit_transactions()
-        return update
-
-    def switch_database(self, database):
-
-        self.name = database
+import psycopg2 as pgsql
+
+
+class Db:
+
+    def __init__(self, name, user, code, host):
+
+        self.name = name
+        self.user = user
+        self.code = code
+        self.host = host
+        self.cursor = self.connection.cursor()
+
+    @property
+    def connection(self):
+
+        return pgsql.connect(dbname=self.name, user=self.user, password=self.code, host=self.host)
+
+    def close_connection(self):
+        """closes connection to database"""
+        self.connection.close()
+
+    def select(self, query_string: str) -> list[tuple]:
+        """executes query and returns data"""
+        self.cursor.execute(query_string)
+        return self.cursor.fetchall()
+
+
+    def select_json(self, query_string: str) -> list[dict]:
+
+        """executes query and returns data as a list of dictionaries"""
+        self.cursor.execute(f"SELECT json_agg(__temp_table__) FROM ({query_string}) __temp_table__;")
+        return self.cursor.fetchall()
+
+    def select_where(self, query_string: str, params: tuple) -> list[tuple]:
+
+        self.cursor.execute(query_string, params)
+        return self.cursor.fetchall()
+
+    def select_where_json(self, query_string: str, params: tuple) -> list[dict]:
+
+        self.cursor.execute(f"SELECT json_agg(__temp_table__) FROM ({query_string}) __temp_table__;", params)
+        return self.cursor.fetchall()
+
+    def insert(self, statement: str, values: list or tuple or dict):
+        """writes query to database"""
+        return self.cursor.execute(statement, tuple(values.values()) if isinstance(values, dict) else tuple(values))
+
+    def commit_transactions(self):
+        """commits transaction to database"""
+        self.connection.commit()
+
+    def commit_and_close_connection(self):
+        """commits transaction and closes connection"""
+        self.commit_transactions()
+        self.connection.close()
+
+    def insert_and_commit(self, statement: str, values: list or tuple or dict):
+        """writes query to database and commits transaction"""
+        insert = self.insert(statement, values)
+        self.commit_transactions()
+        return insert
+    
+    def restart_connection(self):
+        """closes connection and starts new one"""
+        self.connection.close()
+        self.connection
+
+    def rollback(self):
+        """rollsback statements"""
+        self.cursor.execute("ROLLBACK")
+
+    #def update(self, statement, values):
+     #   """updates row(s) in database"""
+     #   return self.cusrsore.execute(statement, tuple(_ for _ in row[1:]) + (row[0],))
+
+    #def update_and_commit(self, statement, values):
+     #   """updates row(s) in database and commits transactions"""
+      #  update = self.update(statement, values)
+       # self.commit_transactions()
+        #return update
+
+    def switch_database(self, database):
+
+        self.name = database
         return self.connection
```

