# Comparing `tmp/bbat-5.2.7.tar.gz` & `tmp/bbat-5.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbat-5.2.7.tar", last modified: Fri Jul 14 08:32:41 2023, max compression
+gzip compressed data, was "bbat-5.2.8.tar", last modified: Fri Jul 14 08:35:41 2023, max compression
```

## Comparing `bbat-5.2.7.tar` & `bbat-5.2.8.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 08:32:41.891872 bbat-5.2.7/
--rw-rw-rw-   0        0        0      289 2023-07-14 08:32:41.891872 bbat-5.2.7/PKG-INFO
--rw-rw-rw-   0        0        0      163 2023-07-10 01:19:32.000000 bbat-5.2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 08:32:41.837277 bbat-5.2.7/bbat/
--rw-rw-rw-   0        0        0        0 2023-07-10 08:21:51.000000 bbat-5.2.7/bbat/__init__.py
--rw-rw-rw-   0        0        0     1720 2023-07-12 02:26:35.000000 bbat-5.2.7/bbat/config.py
--rw-rw-rw-   0        0        0     3085 2023-07-12 02:26:35.000000 bbat-5.2.7/bbat/crypto.py
--rw-rw-rw-   0        0        0     1230 2023-07-11 01:11:37.000000 bbat-5.2.7/bbat/date.py
-drwxrwxrwx   0        0        0        0 2023-07-14 08:32:41.860872 bbat-5.2.7/bbat/db/
--rw-rw-rw-   0        0        0        0 2023-07-10 01:19:32.000000 bbat-5.2.7/bbat/db/__init__.py
--rw-rw-rw-   0        0        0     5371 2023-07-10 05:33:54.000000 bbat-5.2.7/bbat/db/aio_mysql.py
--rw-rw-rw-   0        0        0     2632 2023-07-10 01:19:32.000000 bbat-5.2.7/bbat/db/aio_sqlite.py
--rw-rw-rw-   0        0        0     2339 2023-07-10 05:34:01.000000 bbat-5.2.7/bbat/db/mysql.py
--rw-rw-rw-   0        0        0       30 2023-07-10 01:19:32.000000 bbat-5.2.7/bbat/hi.py
--rw-rw-rw-   0        0        0     1978 2023-07-11 01:47:46.000000 bbat-5.2.7/bbat/image.py
-drwxrwxrwx   0        0        0        0 2023-07-14 08:32:41.863875 bbat-5.2.7/bbat/llm/
--rw-rw-rw-   0        0        0        0 2023-07-12 02:26:35.000000 bbat-5.2.7/bbat/llm/__init__.py
--rw-rw-rw-   0        0        0     2387 2023-07-13 04:46:10.000000 bbat-5.2.7/bbat/llm/chatgpt.py
--rw-rw-rw-   0        0        0      920 2023-07-10 08:19:47.000000 bbat-5.2.7/bbat/log.py
--rw-rw-rw-   0        0        0      828 2023-07-12 02:35:59.000000 bbat-5.2.7/bbat/machine.py
--rw-rw-rw-   0        0        0     1868 2023-07-11 02:21:26.000000 bbat-5.2.7/bbat/notice.py
--rw-rw-rw-   0        0        0     2413 2023-07-10 06:14:27.000000 bbat-5.2.7/bbat/np.py
--rw-rw-rw-   0        0        0      981 2023-07-10 08:07:34.000000 bbat-5.2.7/bbat/path.py
--rw-rw-rw-   0        0        0     4198 2023-07-10 06:52:29.000000 bbat-5.2.7/bbat/text.py
-drwxrwxrwx   0        0        0        0 2023-07-14 08:32:41.874874 bbat-5.2.7/bbat/web/
--rw-rw-rw-   0        0        0        0 2023-07-11 01:54:28.000000 bbat-5.2.7/bbat/web/__init__.py
--rw-rw-rw-   0        0        0     1685 2023-07-11 01:55:27.000000 bbat-5.2.7/bbat/web/client.py
--rw-rw-rw-   0        0        0      504 2023-07-10 01:19:32.000000 bbat-5.2.7/bbat/web/cors.py
--rw-rw-rw-   0        0        0     3929 2023-07-12 02:26:35.000000 bbat-5.2.7/bbat/web/db_server.py
--rw-rw-rw-   0        0        0      178 2023-07-13 05:18:31.000000 bbat-5.2.7/bbat/web/flask_app.py
--rw-rw-rw-   0        0        0     1566 2023-07-11 01:11:37.000000 bbat-5.2.7/bbat/web/sanic_app.py
-drwxrwxrwx   0        0        0        0 2023-07-14 08:32:41.885874 bbat-5.2.7/bbat/web/url_to_sql/
--rw-rw-rw-   0        0        0        0 2023-07-10 01:19:32.000000 bbat-5.2.7/bbat/web/url_to_sql/__init__.py
--rw-rw-rw-   0        0        0     1488 2023-07-10 07:04:39.000000 bbat-5.2.7/bbat/web/url_to_sql/field.py
--rw-rw-rw-   0        0        0     7552 2023-07-10 07:04:45.000000 bbat-5.2.7/bbat/web/url_to_sql/query.py
--rw-rw-rw-   0        0        0     2256 2023-07-10 07:04:49.000000 bbat-5.2.7/bbat/web/url_to_sql/relation.py
--rw-rw-rw-   0        0        0      722 2023-07-10 07:04:52.000000 bbat-5.2.7/bbat/web/url_to_sql/test.py
--rw-rw-rw-   0        0        0      964 2023-07-10 01:19:32.000000 bbat-5.2.7/bbat/web/url_to_sql/util.py
--rw-rw-rw-   0        0        0     1473 2023-07-10 07:04:56.000000 bbat-5.2.7/bbat/web/url_to_sql/where.py
--rw-rw-rw-   0        0        0     1614 2023-07-12 09:36:02.000000 bbat-5.2.7/bbat/zcli.py
-drwxrwxrwx   0        0        0        0 2023-07-14 08:32:41.855872 bbat-5.2.7/bbat.egg-info/
--rw-rw-rw-   0        0        0      289 2023-07-14 08:32:41.000000 bbat-5.2.7/bbat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      832 2023-07-14 08:32:41.000000 bbat-5.2.7/bbat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 08:32:41.000000 bbat-5.2.7/bbat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-14 08:32:41.000000 bbat-5.2.7/bbat.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2023-07-14 08:32:41.000000 bbat-5.2.7/bbat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 08:32:41.892874 bbat-5.2.7/setup.cfg
--rw-rw-rw-   0        0        0      553 2023-07-14 08:32:38.000000 bbat-5.2.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-14 08:32:41.889874 bbat-5.2.7/test/
--rw-rw-rw-   0        0        0      209 2023-07-10 06:44:06.000000 bbat-5.2.7/test/test_config.py
--rw-rw-rw-   0        0        0      194 2023-07-10 06:44:18.000000 bbat-5.2.7/test/test_db_mysql.py
+drwxrwxrwx   0        0        0        0 2023-07-14 08:35:41.538939 bbat-5.2.8/
+-rw-rw-rw-   0        0        0      289 2023-07-14 08:35:41.537939 bbat-5.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0      163 2023-07-10 01:19:32.000000 bbat-5.2.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 08:35:41.483937 bbat-5.2.8/bbat/
+-rw-rw-rw-   0        0        0        0 2023-07-10 08:21:51.000000 bbat-5.2.8/bbat/__init__.py
+-rw-rw-rw-   0        0        0     1720 2023-07-12 02:26:35.000000 bbat-5.2.8/bbat/config.py
+-rw-rw-rw-   0        0        0     3085 2023-07-12 02:26:35.000000 bbat-5.2.8/bbat/crypto.py
+-rw-rw-rw-   0        0        0     1230 2023-07-11 01:11:37.000000 bbat-5.2.8/bbat/date.py
+drwxrwxrwx   0        0        0        0 2023-07-14 08:35:41.504939 bbat-5.2.8/bbat/db/
+-rw-rw-rw-   0        0        0        0 2023-07-10 01:19:32.000000 bbat-5.2.8/bbat/db/__init__.py
+-rw-rw-rw-   0        0        0     5498 2023-07-14 08:35:13.000000 bbat-5.2.8/bbat/db/aio_mysql.py
+-rw-rw-rw-   0        0        0     2632 2023-07-10 01:19:32.000000 bbat-5.2.8/bbat/db/aio_sqlite.py
+-rw-rw-rw-   0        0        0     2339 2023-07-10 05:34:01.000000 bbat-5.2.8/bbat/db/mysql.py
+-rw-rw-rw-   0        0        0       30 2023-07-10 01:19:32.000000 bbat-5.2.8/bbat/hi.py
+-rw-rw-rw-   0        0        0     1978 2023-07-11 01:47:46.000000 bbat-5.2.8/bbat/image.py
+drwxrwxrwx   0        0        0        0 2023-07-14 08:35:41.507938 bbat-5.2.8/bbat/llm/
+-rw-rw-rw-   0        0        0        0 2023-07-12 02:26:35.000000 bbat-5.2.8/bbat/llm/__init__.py
+-rw-rw-rw-   0        0        0     2416 2023-07-14 08:35:08.000000 bbat-5.2.8/bbat/llm/chatgpt.py
+-rw-rw-rw-   0        0        0      920 2023-07-10 08:19:47.000000 bbat-5.2.8/bbat/log.py
+-rw-rw-rw-   0        0        0      828 2023-07-12 02:35:59.000000 bbat-5.2.8/bbat/machine.py
+-rw-rw-rw-   0        0        0     1868 2023-07-11 02:21:26.000000 bbat-5.2.8/bbat/notice.py
+-rw-rw-rw-   0        0        0     2413 2023-07-10 06:14:27.000000 bbat-5.2.8/bbat/np.py
+-rw-rw-rw-   0        0        0      981 2023-07-10 08:07:34.000000 bbat-5.2.8/bbat/path.py
+-rw-rw-rw-   0        0        0     4198 2023-07-10 06:52:29.000000 bbat-5.2.8/bbat/text.py
+drwxrwxrwx   0        0        0        0 2023-07-14 08:35:41.514938 bbat-5.2.8/bbat/web/
+-rw-rw-rw-   0        0        0        0 2023-07-11 01:54:28.000000 bbat-5.2.8/bbat/web/__init__.py
+-rw-rw-rw-   0        0        0     1685 2023-07-11 01:55:27.000000 bbat-5.2.8/bbat/web/client.py
+-rw-rw-rw-   0        0        0      504 2023-07-10 01:19:32.000000 bbat-5.2.8/bbat/web/cors.py
+-rw-rw-rw-   0        0        0     4758 2023-07-14 08:35:13.000000 bbat-5.2.8/bbat/web/db_server.py
+-rw-rw-rw-   0        0        0      177 2023-07-14 08:35:05.000000 bbat-5.2.8/bbat/web/flask_app.py
+-rw-rw-rw-   0        0        0     1566 2023-07-11 01:11:37.000000 bbat-5.2.8/bbat/web/sanic_app.py
+drwxrwxrwx   0        0        0        0 2023-07-14 08:35:41.533938 bbat-5.2.8/bbat/web/url_to_sql/
+-rw-rw-rw-   0        0        0        0 2023-07-10 01:19:32.000000 bbat-5.2.8/bbat/web/url_to_sql/__init__.py
+-rw-rw-rw-   0        0        0     1488 2023-07-10 07:04:39.000000 bbat-5.2.8/bbat/web/url_to_sql/field.py
+-rw-rw-rw-   0        0        0     7542 2023-07-14 08:35:13.000000 bbat-5.2.8/bbat/web/url_to_sql/query.py
+-rw-rw-rw-   0        0        0     2256 2023-07-10 07:04:49.000000 bbat-5.2.8/bbat/web/url_to_sql/relation.py
+-rw-rw-rw-   0        0        0      722 2023-07-10 07:04:52.000000 bbat-5.2.8/bbat/web/url_to_sql/test.py
+-rw-rw-rw-   0        0        0      964 2023-07-10 01:19:32.000000 bbat-5.2.8/bbat/web/url_to_sql/util.py
+-rw-rw-rw-   0        0        0     1473 2023-07-10 07:04:56.000000 bbat-5.2.8/bbat/web/url_to_sql/where.py
+-rw-rw-rw-   0        0        0     1614 2023-07-12 09:36:02.000000 bbat-5.2.8/bbat/zcli.py
+drwxrwxrwx   0        0        0        0 2023-07-14 08:35:41.499940 bbat-5.2.8/bbat.egg-info/
+-rw-rw-rw-   0        0        0      289 2023-07-14 08:35:41.000000 bbat-5.2.8/bbat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      832 2023-07-14 08:35:41.000000 bbat-5.2.8/bbat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 08:35:41.000000 bbat-5.2.8/bbat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-14 08:35:41.000000 bbat-5.2.8/bbat.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2023-07-14 08:35:41.000000 bbat-5.2.8/bbat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 08:35:41.538939 bbat-5.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      553 2023-07-14 08:35:36.000000 bbat-5.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 08:35:41.536939 bbat-5.2.8/test/
+-rw-rw-rw-   0        0        0      209 2023-07-10 06:44:06.000000 bbat-5.2.8/test/test_config.py
+-rw-rw-rw-   0        0        0      194 2023-07-10 06:44:18.000000 bbat-5.2.8/test/test_db_mysql.py
```

### Comparing `bbat-5.2.7/bbat/config.py` & `bbat-5.2.8/bbat/config.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.7/bbat/crypto.py` & `bbat-5.2.8/bbat/crypto.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.7/bbat/date.py` & `bbat-5.2.8/bbat/date.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.7/bbat/db/aio_mysql.py` & `bbat-5.2.8/bbat/db/aio_mysql.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,15 +94,20 @@
                     await conn.ping()
                     await cur.execute(query, kwparameters or parameters)
                 return cur.lastrowid
             
     async def insert(self, table, data):
         keys = list(data.keys())
         keys = ','.join(keys)
-        values = [f'"{i}"' for i in data.values()]
+        values = []
+        for i in data.values():
+            if isinstance(i, str):
+                i = i.replace('"', '\"')
+            values.append(f'"{i}"')
+        
         values = ','.join(values)
         sql = f'INSERT INTO {table} ({keys}) VALUES ({values})'
         print('>>> insert sql:', sql)
         res = await self.execute(sql)
         return res
```

### Comparing `bbat-5.2.7/bbat/db/aio_sqlite.py` & `bbat-5.2.8/bbat/db/aio_sqlite.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.7/bbat/db/mysql.py` & `bbat-5.2.8/bbat/db/mysql.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.7/bbat/image.py` & `bbat-5.2.8/bbat/image.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.7/bbat/llm/chatgpt.py` & `bbat-5.2.8/bbat/llm/chatgpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
                 **params
             )
             messages.append({
                 "role": response['choices'][0]['message']['role'],
                 "content": response['choices'][0]['message']['content']
             })
             msg = response['choices'][0]['message']
+            print(f'{msg}')
             return msg
     except Exception as err:
         traceback.print_exc()
         print(f'OpenAI API 异常: {err}')
         return None
```

### Comparing `bbat-5.2.7/bbat/log.py` & `bbat-5.2.8/bbat/log.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.7/bbat/machine.py` & `bbat-5.2.8/bbat/machine.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.7/bbat/notice.py` & `bbat-5.2.8/bbat/notice.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.7/bbat/np.py` & `bbat-5.2.8/bbat/np.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.7/bbat/path.py` & `bbat-5.2.8/bbat/path.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.7/bbat/text.py` & `bbat-5.2.8/bbat/text.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.7/bbat/web/client.py` & `bbat-5.2.8/bbat/web/client.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.7/bbat/web/sanic_app.py` & `bbat-5.2.8/bbat/web/sanic_app.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.7/bbat/web/url_to_sql/field.py` & `bbat-5.2.8/bbat/web/url_to_sql/field.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.7/bbat/web/url_to_sql/query.py` & `bbat-5.2.8/bbat/web/url_to_sql/query.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,22 +8,23 @@
 from bbat.web.url_to_sql.relation import Relation
 
 class Query:
     def __init__(self, table, query_string):
         if not table:
             raise Exception("params error: table")
         self.table_name  = table
-        self.table_query = unquote(query_string)
+        self.table_query = unquote(str(query_string))
+
         self.group = []
         self.order = []
         self.limit = 0
         self.offset = 0
         self.meta = []
         self.page = 1   # 默认页
-        self.size = 1000  # 默认数据数
+        self.size = 100  # 默认数据数
 
         self.relation = []
         self.where = []
         self.fields = []
         self.keywords  = ['meta', 'field', 'group', 'size', 'page', 'sort']
         # 提取query_string信息
         self.parse()
@@ -147,23 +148,23 @@
         return node
 
      # sql
     def to_sql(self):
         n = self.build_sql_node()
         sql = f"SELECT {n['field']} FROM {n['table']} {n['where']} {n['groupby']} {n['orderby']} {n['limit']}"
         sql = re.sub(r"\s+", " ", sql)
-        print("QUERY SQL>>>", sql)
+        print("sql>", sql)
         return sql
     
     # meta 函数 查询总数
     def to_count_sql(self):
         n = self.build_sql_node()
         sql = f"SELECT count(1) cnt FROM {n['table']} {n['where']} {n['groupby']}"
         sql = re.sub(r"\s+", " ", sql)
-        print("COUNT SQL>>>", sql)
+        print("sql>", sql)
         return sql
       
     # 插入sql
     def to_insert_sql(self, data, replace=False):
         length, keys, insert_data = self.data2sqlvalue(data)
         if type(insert_data) is tuple:
             insert_data = [insert_data]
@@ -172,15 +173,15 @@
             for i in d]) + ")" for d in insert_data
         ]
         sql = "INSERT INTO %s (%s) VALUES %s" % (self.table_name, ', '.join( [f"`{i}`" for i in keys]), ', '.join(data))
         if replace:
             sql += (' ON DUPLICATE KEY UPDATE ' + ', '.join(['%s=VALUES(%s)' % (x, x) for x in keys]))
         # sqlalcheme parse bug
         sql = sql.replace(":", "\:")
-        print("INSERT SQL>>>", sql)
+        print("sql>", sql)
         return sql
     
     # 更新sql
     def to_update_sql(self, data):
         n = self.build_sql_node()
         sql = "UPDATE %s SET %s" % (
             self.table_name,
@@ -189,24 +190,24 @@
                 for k, v in data.items()
             ]),
         )
         # where 
         sql += n['where']
         # sqlalcheme parse bug
         sql = sql.replace(":", "\:")
-        print("UPDATE SQL>>>", sql)
+        print("sql>", sql)
         return sql
 
     # 删除sql
     def to_delete_sql(self):
         n = self.build_sql_node()
         sql = "DELETE FROM %s " % (self.table_name)
         sql += n['where']
         sql = sql.replace(':', '\:')
-        print("DELETE SQL>>>", sql)
+        print("sql>", sql)
         return sql
 
     def data2sqlvalue(self, data):
         if isinstance(data, dict):
             item = data
             keys = item.keys()
             length = len(item)
@@ -218,10 +219,11 @@
             values = [
                 tuple([str(i) if i is not None else None for i in item.values()])
                 for item in data
             ]
         elif data is None:
             return None, None, None
         else:
-            raise Exception("data type error")
+            print(data)
+            raise Exception("data type error: ")
         return length, keys, values
```

### Comparing `bbat-5.2.7/bbat/web/url_to_sql/relation.py` & `bbat-5.2.8/bbat/web/url_to_sql/relation.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.7/bbat/web/url_to_sql/test.py` & `bbat-5.2.8/bbat/web/url_to_sql/test.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.7/bbat/web/url_to_sql/util.py` & `bbat-5.2.8/bbat/web/url_to_sql/util.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.7/bbat/web/url_to_sql/where.py` & `bbat-5.2.8/bbat/web/url_to_sql/where.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.7/bbat/zcli.py` & `bbat-5.2.8/bbat/zcli.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.7/bbat.egg-info/SOURCES.txt` & `bbat-5.2.8/bbat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bbat-5.2.7/setup.py` & `bbat-5.2.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 name = "bbat"
-version = "5.2.7"
+version = "5.2.8"
 
 setuptools.setup(
     name=name,
     version=version,
     author="zlge",
     author_email="test@test.com",
     description="",
```

