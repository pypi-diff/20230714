# Comparing `tmp/fastmysql-0.0.9.tar.gz` & `tmp/fastmysql-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fastmysql-0.0.9.tar", last modified: Sat Apr  9 07:29:00 2022, max compression
+gzip compressed data, was "fastmysql-0.1.0.tar", last modified: Fri Jul 14 08:50:17 2023, max compression
```

## Comparing `fastmysql-0.0.9.tar` & `fastmysql-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2022-04-09 07:29:00.212222 fastmysql-0.0.9/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1067 2022-04-09 04:45:06.000000 fastmysql-0.0.9/LICENSE
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1710 2022-04-09 07:29:00.211937 fastmysql-0.0.9/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1268 2022-04-09 04:45:06.000000 fastmysql-0.0.9/README.md
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2022-04-09 07:29:00.209092 fastmysql-0.0.9/fastmysql/
--rw-r--r--   0 zeroseeker   (501) staff       (20)      208 2022-04-09 04:46:34.000000 fastmysql-0.0.9/fastmysql/__init__.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    38558 2022-04-09 07:27:43.000000 fastmysql-0.0.9/fastmysql/fastmysql.py
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2022-04-09 07:29:00.211365 fastmysql-0.0.9/fastmysql.egg-info/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1710 2022-04-09 07:29:00.000000 fastmysql-0.0.9/fastmysql.egg-info/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      235 2022-04-09 07:29:00.000000 fastmysql-0.0.9/fastmysql.egg-info/SOURCES.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2022-04-09 07:29:00.000000 fastmysql-0.0.9/fastmysql.egg-info/dependency_links.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)      131 2022-04-09 07:29:00.000000 fastmysql-0.0.9/fastmysql.egg-info/requires.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       10 2022-04-09 07:29:00.000000 fastmysql-0.0.9/fastmysql.egg-info/top_level.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2022-04-09 07:29:00.212330 fastmysql-0.0.9/setup.cfg
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1074 2022-04-09 07:28:39.000000 fastmysql-0.0.9/setup.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-14 08:50:17.427523 fastmysql-0.1.0/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1775 2023-07-14 08:50:17.427429 fastmysql-0.1.0/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1442 2023-02-22 07:55:41.000000 fastmysql-0.1.0/README.md
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-14 08:50:17.426395 fastmysql-0.1.0/fastmysql/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      208 2023-02-22 07:55:41.000000 fastmysql-0.1.0/fastmysql/__init__.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    47513 2023-07-14 08:48:57.000000 fastmysql-0.1.0/fastmysql/fastmysql.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-14 08:50:17.427277 fastmysql-0.1.0/fastmysql.egg-info/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1775 2023-07-14 08:50:17.000000 fastmysql-0.1.0/fastmysql.egg-info/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      227 2023-07-14 08:50:17.000000 fastmysql-0.1.0/fastmysql.egg-info/SOURCES.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-07-14 08:50:17.000000 fastmysql-0.1.0/fastmysql.egg-info/dependency_links.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      131 2023-07-14 08:50:17.000000 fastmysql-0.1.0/fastmysql.egg-info/requires.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       10 2023-07-14 08:50:17.000000 fastmysql-0.1.0/fastmysql.egg-info/top_level.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-07-14 08:50:17.427557 fastmysql-0.1.0/setup.cfg
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1076 2023-07-14 08:49:36.000000 fastmysql-0.1.0/setup.py
```

### Comparing `fastmysql-0.0.9/PKG-INFO` & `fastmysql-0.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 Metadata-Version: 2.1
 Name: fastmysql
-Version: 0.0.9
+Version: 0.1.0
 Summary: make it easy to use pymysql
 Home-page: https://gitee.com/ZeroSeeker/fastmysql
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # fastmysql
 ![](https://img.shields.io/badge/Python-3.8.6-green.svg)
 
 #### 介绍
 简单快速的使用mysql
 
@@ -23,27 +19,36 @@
 软件架构说明
 
 
 #### 安装教程
 
 1.  pip安装
 ```shell script
-pip install fastmysql
+pip3 install fastmysql
 ```
 2.  pip安装（使用淘宝镜像加速）
 ```shell script
-pip install fastmysql -i https://mirrors.aliyun.com/pypi/simple
+pip3 install fastmysql -i https://mirrors.aliyun.com/pypi/simple
 ```
 
 #### 使用说明
 
 1.  demo
 ```python
 import fastmysql
-query_res = fastmysql.query_table_all_data(db_name='test', tb_name='test')
+query_res = fastmysql.query_table_all_data(
+    db_name='test', 
+    tb_name='test'
+)
+
+# 获取建表语句
+res = fastmysql.show_create_table(
+    db_name='test',
+    tb_name='test'
+)
 ```
 
 2.  防止sql注入：
 写法
 
 cursor.execute('insert into user (name,password) value (?,?)',(name,password))
 　　或者
@@ -53,7 +58,9 @@
 
 cursor.execute('insert into user (name,password) value (?,?)'%(name,password))
 　　这种写法是直接将参数拼接到sql语句中，这样数据库就容易被sql注入攻击，比如
 
 cursor.execute('select * from user where user=%s and password=%s'%(name,password))
 　　要是name和password都等于'a or 1=1'，那么这个语句会把整个user表都查询出来
 
+3.  默认环境
+- 默认使用的环境文件为：mysql.env
```

### Comparing `fastmysql-0.0.9/README.md` & `fastmysql-0.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -8,27 +8,36 @@
 软件架构说明
 
 
 #### 安装教程
 
 1.  pip安装
 ```shell script
-pip install fastmysql
+pip3 install fastmysql
 ```
 2.  pip安装（使用淘宝镜像加速）
 ```shell script
-pip install fastmysql -i https://mirrors.aliyun.com/pypi/simple
+pip3 install fastmysql -i https://mirrors.aliyun.com/pypi/simple
 ```
 
 #### 使用说明
 
 1.  demo
 ```python
 import fastmysql
-query_res = fastmysql.query_table_all_data(db_name='test', tb_name='test')
+query_res = fastmysql.query_table_all_data(
+    db_name='test', 
+    tb_name='test'
+)
+
+# 获取建表语句
+res = fastmysql.show_create_table(
+    db_name='test',
+    tb_name='test'
+)
 ```
 
 2.  防止sql注入：
 写法
 
 cursor.execute('insert into user (name,password) value (?,?)',(name,password))
 　　或者
@@ -36,8 +45,11 @@
 cursor.execute('insert into user (name,password) value (%s,%s)',(name,password))
 　　%s与?都可以作为sql语句的占位符，它们作为占位符的功能是没有区别的，mysql.connector用 %s 作为占位符；pymysql用 ? 作为占位符。但是注意不要写成
 
 cursor.execute('insert into user (name,password) value (?,?)'%(name,password))
 　　这种写法是直接将参数拼接到sql语句中，这样数据库就容易被sql注入攻击，比如
 
 cursor.execute('select * from user where user=%s and password=%s'%(name,password))
-　　要是name和password都等于'a or 1=1'，那么这个语句会把整个user表都查询出来
+　　要是name和password都等于'a or 1=1'，那么这个语句会把整个user表都查询出来
+
+3.  默认环境
+- 默认使用的环境文件为：mysql.env
```

### Comparing `fastmysql-0.0.9/fastmysql/fastmysql.py` & `fastmysql-0.1.0/fastmysql/fastmysql.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,642 +11,790 @@
 import pandas as pd
 import numpy as np
 import showlog
 import pymysql
 import time
 import copy
 import envx
-silence_default = True
+silence_default = True  # 默认静默参数为True
+env_file_name_default = 'mysql.env'  # 默认数据库连接环境文件名
+reconnect_errors = (ConnectionError, ConnectionAbortedError, TimeoutError)
+default_charset = 'utf8'
+default_show_sql = False
 
 
 def make_con_info(
-        env_file_name: str = 'mysql.env'
+        env_file_name: str = env_file_name_default,
+        silence: bool = silence_default
 ):
+    """
+    读取当前环境的环境文件信息并生成连接信息
+    """
     inner_env = envx.read(file_name=env_file_name)
-    if inner_env is None or len(inner_env) == 0:
-        showlog.warning('[%s]文件不存在或文件填写错误！' % env_file_name)
+    if not inner_env:
+        if not silence:
+            showlog.warning(f'环境文件[ {env_file_name} ]不存在！')
         exit()
     else:
         con_info = dict()
 
         host = inner_env.get('host')
-        if host is not None and len(host) > 0:
+        if host:
             con_info['host'] = host
         else:
-            showlog.warning('host 未填写，将设置为默认值：localhost')
+            if not silence:
+                showlog.warning('host 未填写，将设置为默认值：localhost')
             con_info['host'] = 'localhost'
 
         port = inner_env.get('port')
-        if port is not None and len(port) > 0:
+        if port:
             try:
                 con_info['port'] = int(port)
             except:
-                showlog.warning('port 填写错误，必须为int')
+                if not silence:
+                    showlog.warning('port 填写错误，必须为int')
                 exit()
         else:
-            showlog.warning('port 未填写，将设置为默认值：3306')
+            if not silence:
+                showlog.warning('port 未填写，将设置为默认值：3306')
             con_info['port'] = 3306
 
         username = inner_env.get('username')
-        if username is not None and len(username) > 0:
+        if username:
             con_info['username'] = username
         else:
-            showlog.warning('username 未填写，将设置为默认值：root')
+            if not silence:
+                showlog.warning('username 未填写，将设置为默认值：root')
             con_info['username'] = 'root'
 
         password = inner_env.get('password')
-        if password is not None and len(password) > 0:
+        if password:
             con_info['password'] = password
         else:
-            showlog.warning('password 未填写，将设置为默认值：空')
+            if not silence:
+                showlog.warning('password 未填写，将设置为默认值：空')
             con_info['password'] = ''
 
         charset = inner_env.get('charset')
-        if charset is not None and len(charset) > 0:
+        if charset:
             con_info['charset'] = charset
         else:
-            showlog.warning('charset 未填写，将设置为默认值：utf8')
-            con_info['charset'] = 'utf8'
+            con_info['charset'] = default_charset
 
         return con_info
 
 
 def con_mysql(
         host: str,
         username: str,
         password: str,
         db_name: str = None,
         port: int = 3306,
         charset: str = 'utf8',
-        ssc: bool = False
+        ssc: bool = False,
+        silence: bool = silence_default,
+        auto_reconnect: bool = True,
+        reconnect_wait: int = 5
 ):
     """
-    此函数为有提示信息的Mysql数据库连接函数的优化，内部预定义了连接的默认字符设置
+    执行连接数据库
     当连接失败时，将倒计时5秒后重连，直到连接成功
-    此函数有运行提示
+    包含重试机制
     :param host:
     :param db_name:
     :param username:
     :param password:
     :param port: 默认端口为3306
     :param charset: 默认字符集为utf8
     :param ssc: 默认不使用流式游标
+    :param silence: 静默模式
+    :param auto_reconnect: 自动重连
+    :param reconnect_wait: 重连等待时间，单位为秒，默认为5秒
     :return:(con, cur)
     """
     while True:
         try:
-            showlog.info('User [%s] are trying to connect to the database [%s] ...' % (username, db_name))
+            if not silence:
+                showlog.info(f'User [{username}] are trying to connect to the database [{db_name}] ...')
             con = pymysql.connect(
                 host=host,
                 db=db_name,
                 user=username,
                 passwd=password,
                 port=port,
                 charset=charset
             )
             if ssc is False:
                 cur = con.cursor()
             else:
                 cur = pymysql.cursors.SSCursor(con)  # 使用流式游标
-            cur.execute('SET NAMES utf8mb4')
-            cur.execute('SET CHARACTER SET utf8mb4')
-            cur.execute('SET character_set_connection=utf8mb4')
-            showlog.info('ok! connection success.')
+            cur.execute(query='SET NAMES utf8mb4')
+            cur.execute(query='SET CHARACTER SET utf8mb4')
+            cur.execute(query='SET character_set_connection=utf8mb4')
+            if not silence:
+                showlog.info('ok! connection success.')
             return con, cur
-        except:
-            showlog.error('Oops, connection failed, Trying to reconnect in 5 seconds ...')
-            time.sleep(5)
-
-
-def con_mysql_silence(
-        host: str,
-        username: str,
-        password: str,
-        db_name: str = None,
-        port: int = 3306,
-        charset: str = 'utf8',
-        ssc: bool = False
-):
-    """
-    此函数为无提示信息的Mysql数据库连接函数的优化，内部预定义了连接的默认字符设置
-    当连接失败时，将倒计时5秒后重连，直到连接成功
-    此函数无运行提示
-    :param host:
-    :param db_name:
-    :param username:
-    :param password:
-    :param port: 默认端口为3306
-    :param charset: 默认字符集为utf8
-    :param ssc: 默认不使用流式游标
-    :return:(con, cur)
-    """
-    while True:
-        try:
-            con = pymysql.connect(
-                host=host,
-                db=db_name,
-                user=username,
-                passwd=password,
-                port=port,
-                charset=charset
-            )
-            if ssc is False:
-                cur = con.cursor()
+        except reconnect_errors:
+            if auto_reconnect:
+                if not silence:
+                    showlog.error(f'Oops, reconnect_errors, Trying to reconnect in {reconnect_wait} seconds ...')
+                time.sleep(reconnect_wait)
             else:
-                cur = pymysql.cursors.SSCursor(con)  # 使用流式游标
-            cur.execute('SET NAMES utf8mb4')
-            cur.execute('SET CHARACTER SET utf8mb4')
-            cur.execute('SET character_set_connection=utf8mb4')
-            return con, cur
+                return
         except:
-            time.sleep(5)
+            if auto_reconnect:
+                if not silence:
+                    showlog.error(f'Oops, connection failed, Trying to reconnect in {reconnect_wait} seconds ...')
+                time.sleep(reconnect_wait)
+            else:
+                return
 
 
 def con2db(
         con_info: dict,
         db_name: str = None,
-        silence: bool = silence_default,  # 默认为非静默模式
-        ssc: bool = False
+        silence: bool = silence_default,
+        ssc: bool = False,
+        auto_reconnect: bool = True,
+        reconnect_wait: int = 5
 ):
     """
     对连接数据库的方法再次优化，此处可以定义所有数据库的连接
+    包含重试机制
     :param con_info:设置连接的具体信息，必须包含：host、username、password，可选包含：port、charset
     :param db_name:设置需要连接的数据库
     :param silence:设置静默模式，为True表示静默，为False表示非静默
     :param ssc: 默认不使用流式游标
+    :param auto_reconnect: 自动重连
+    :param reconnect_wait: 重连等待时间，单位为秒，默认为5秒
     :return:connection，由(con, cur)组成，所以返回的效果是(con, cur)
     """
-    host = con_info.get("host")
-    username = con_info.get("username")
-    password = con_info.get("password")
-    port = con_info.get("port", 3306)
-    charset = con_info.get("charset", "utf8")
-    if silence is True:
-        connection = con_mysql_silence(
-            host=host,
-            db_name=db_name,
-            username=username,
-            password=password,
-            port=port,
-            charset=charset,
-            ssc=ssc
-        )
-        return connection
-    else:
-        connection = con_mysql(
-            host=host,
-            db_name=db_name,
-            username=username,
-            password=password,
-            port=port,
-            charset=charset,
-            ssc=ssc
-        )
-        return connection
+    return con_mysql(
+        host=con_info.get("host"),
+        db_name=db_name,
+        username=con_info.get("username"),
+        password=con_info.get("password"),
+        port=con_info.get("port", 3306),
+        charset=con_info.get("charset", "utf8"),
+        ssc=ssc,
+        silence=silence,
+        auto_reconnect=auto_reconnect,
+        reconnect_wait=reconnect_wait
+    )
 
 
 def _query(
         sql: str,
         cur,
         con=None,
         parameter: tuple = None,
-        operate: bool = False  # 是否为操作
+        operate: bool = False,  # 是否为操作
+        order_dict: bool = True,
+        silence: bool = silence_default
 ):
     """
     查询结果以list(dict)形式输出
+    [不包含重试机制，需要在外部执行重试]
     :param sql:
     :param cur:
     :param con:
     :param parameter: 参数化查询语句避免SQL注入
     :param operate: 为True的时候执行操作（执行commit），为False的时候执行查询数据（不执行commit）
+    :param order_dict: 返回值是否组成有序dict
+    :param silence:设置静默模式，为True表示静默，为False表示非静默
     :return:
     """
-    try:
-        if parameter is None:
-            cur.execute(sql)
-        else:
-            cur.execute(sql, parameter)
-        if operate is False:
-            # 只查询
-            index = cur.description
-            result = list()
-            for res in cur.fetchall():
+    cur.execute(query=sql, args=parameter)
+    if operate is False:
+        # 只查询
+        index = cur.description
+        result = list()
+        for res in cur.fetchall():
+            if order_dict is True:
                 row = OrderedDict()
-                for i in range(len(index)):
-                    row[index[i][0]] = res[i]
-                result.append(row)
-            return result
-        else:
-            # 只操作
-            effect_rows = cur.rowcount
-            con.commit()
-            return effect_rows
-    except Exception as ex:
-        showlog.warning("Oops! there is an error occurred in query:%s , sql: %s ,parameter: %s" % (ex, sql, parameter))
-        return
+            else:
+                row = dict()
+            for i in range(len(index)):
+                row[index[i][0]] = res[i]
+            result.append(row)
+        return result
+    else:
+        # 只操作
+        effect_rows = cur.rowcount
+        con.commit()
+        return effect_rows
 
 
 def query_table_all_data(
         db_name: str,  # 必须为内部参数，防止注入
         tb_name: str,  # 必须为内部参数，防止注入
         con_info: dict = None,  # 若指定，将优先使用
-        env_file_name: str = 'mysql.env',
+        env_file_name: str = env_file_name_default,
         order_col: str = None,  # 需要排序的列，必须为内部参数，防止注入
         order_index: str = "DESC",  # 排序规则，必须为内部参数，防止注入
-        silence: bool = silence_default
+        silence: bool = silence_default,
+        order_dict: bool = True,
+        auto_reconnect: bool = True,
+        reconnect_wait: int = 5
 ):
     """
+    获取表所有数据
+    包含重试机制
+    :param db_name: 必须为内部参数，防止注入
+    :param tb_name: 必须为内部参数，防止注入
+    :param con_info: 若指定，将优先使用
+    :param env_file_name: 自动重连
+    :param order_col: 需要排序的列，必须为内部参数，防止注入
+    :param order_index: 排序规则，必须为内部参数，防止注入
+    :param silence: 静默参数
+    :param order_dict:
+    :param auto_reconnect: 自动重连
+    :param reconnect_wait: 重连等待时间，单位为秒，默认为5秒
     查询某个表的所有数据
     查询结果以list(dict)形式输出
     """
     # ---------------- 固定设置 ----------------
-    if con_info is None:
-        con_info = make_con_info(env_file_name=env_file_name)
-    else:
-        pass
-    # ---------------- 固定设置 ----------------
-    try:
-        con, cur = con2db(
-            con_info=con_info,
-            db_name=db_name,
+    if not con_info:
+        con_info = make_con_info(
+            env_file_name=env_file_name,
             silence=silence
         )
+    con, cur = con2db(
+        con_info=con_info,
+        db_name=db_name,
+        silence=silence,
+        auto_reconnect=auto_reconnect,
+        reconnect_wait=reconnect_wait
+    )  # 已包含重试机制
+    # ---------------- 固定设置 ----------------
+    try:
         if order_col is None:
-            sql = "SELECT * FROM `%s`.`%s`" % (db_name, tb_name)
-            parameter = None
-        else:
-            sql = "SELECT * FROM `%s`.`%s` ORDER BY %s %s" % (db_name, tb_name, order_col, order_index)
-            parameter = None
-        if silence is True:
-            try:
-                res = _query(
-                    cur=cur,
-                    sql=sql,
-                    parameter=parameter
-                )
-                return res
-            except Exception as ex:
-                return
+            sql = f"SELECT * FROM `{db_name}`.`{tb_name}`"
         else:
-            showlog.info("Executing sql：%s ..." % sql)
+            sql = f"SELECT * FROM `{db_name}`.`{tb_name}` ORDER BY `{order_col}` {order_index}"
+
+        if not silence:
+            showlog.info(f"Executing sql：{sql} ...")
+        while True:
             try:
                 res = _query(
                     cur=cur,
                     sql=sql,
-                    parameter=parameter
+                    order_dict=order_dict,
+                    silence=silence
                 )
-                showlog.info("Executing sql success.")
+                if not silence:
+                    showlog.info("Executing sql success.")
                 return res
+            except reconnect_errors:
+                if auto_reconnect:
+                    if not silence:
+                        showlog.error(f'Oops, reconnect_errors, Trying to reconnect in {reconnect_wait} seconds ...')
+                    time.sleep(reconnect_wait)
+                    con, cur = con2db(
+                        con_info=con_info,
+                        db_name=db_name,
+                        silence=silence,
+                        auto_reconnect=auto_reconnect,
+                        reconnect_wait=reconnect_wait
+                    )  # 已包含重试机制
+                else:
+                    return
             except Exception as ex:
-                showlog.warning("Oops! an error occurred, maybe query error. Exception: %s" % ex)
+                if not silence:
+                    showlog.warning(f"Oops! an error occurred, Exception: {ex}")
                 return
     except Exception as ex:
-        showlog.warning("Oops! an error occurred, maybe con2db error. Exception: %s" % ex)
+        if not silence:
+            showlog.warning(f"Oops! an error occurred, Exception: {ex}")
         return
 
 
 def query_by_sql(
-        sql: str,  # 参数用%s表示
-        parameter: tuple = None,  # 参数化查询避免sql注入
+        sql: str,
+        parameter: tuple = None,
         db_name: str = None,
-        con_info: dict = None,  # 若指定，将优先使用
-        env_file_name: str = 'mysql.env',
-        silence: bool = silence_default
+        con_info: dict = None,
+        env_file_name: str = env_file_name_default,
+        silence: bool = silence_default,
+        order_dict: bool = True,
+        auto_reconnect: bool = True,
+        reconnect_wait: int = 5,
+        show_sql: bool = default_show_sql
 ):
     """
     按照sql查询
+    【包含重试机制】
+    :param sql: 参数用%s表示
+    :param parameter: 参数化查询避免sql注入
+    :param db_name:
+    :param con_info: 若指定，将优先使用
+    :param env_file_name:
+    :param silence:
+    :param order_dict:
+    :param auto_reconnect: 自动重连
+    :param reconnect_wait: 重连等待时间，单位为秒，默认为5秒
+    :param show_sql: 是否显示sql，优先级低于silence
+    按照sql查询
     查询结果以list(dict)形式输出
     """
     # ---------------- 固定设置 ----------------
-    if con_info is None:
-        con_info = make_con_info(env_file_name=env_file_name)
-    else:
-        pass
-    # ---------------- 固定设置 ----------------
-    try:
-        con, cur = con2db(
-            con_info=con_info,
-            db_name=db_name,
+    if not con_info:
+        con_info = make_con_info(
+            env_file_name=env_file_name,
             silence=silence
         )
-        if silence is True:
-            try:
-                res = _query(
-                    cur=cur,
-                    sql=sql,
-                    parameter=parameter
-                )
-                return res
-            except Exception as ex:
-                showlog.warning("Oops! an error occurred, maybe query error. Exception: %s" % ex)
-                return
-        else:
-            showlog.info("Executing sql：%s ..." % sql)
+    con, cur = con2db(
+        con_info=con_info,
+        db_name=db_name,
+        silence=silence,
+        auto_reconnect=auto_reconnect,
+        reconnect_wait=reconnect_wait
+    )  # 已包含重试机制
+    # ---------------- 固定设置 ----------------
+    try:
+        if not silence:
+            if show_sql:
+                showlog.info(f"Executing sql：{sql} ...")
+            else:
+                showlog.info(f"Executing sql ...")
+        while True:
             try:
                 res = _query(
                     cur=cur,
                     sql=sql,
-                    parameter=parameter
+                    parameter=parameter,
+                    order_dict=order_dict,
+                    silence=silence
                 )
-                showlog.info("Executing sql success.")
+                if not silence:
+                    showlog.info("Executing sql success.")
                 return res
+            except reconnect_errors:
+                if auto_reconnect:
+                    if not silence:
+                        showlog.error(f'Oops, reconnect_errors, Trying to reconnect in {reconnect_wait} seconds ...')
+                    time.sleep(reconnect_wait)
+                    con, cur = con2db(
+                        con_info=con_info,
+                        db_name=db_name,
+                        silence=silence,
+                        auto_reconnect=auto_reconnect,
+                        reconnect_wait=reconnect_wait
+                    )  # 已包含重试机制
+                else:
+                    return
             except Exception as ex:
-                showlog.warning("Oops! an error occurred, maybe query error. Exception: %s" % ex)
+                if not silence:
+                    showlog.warning("Oops! an error occurred, Exception: %s" % ex)
                 return
     except Exception as ex:
-        showlog.warning("Oops! an error occurred, maybe con2db error. Exception: %s" % ex)
+        if not silence:
+            showlog.warning("Oops! an error occurred, Exception: %s" % ex)
         return
 
 
 def do_by_sql(
-        sql: str,  # 参数用%s表示
-        parameter: tuple = None,  # 参数化查询避免sql注入
+        sql: str,
+        parameter: tuple = None,
         db_name: str = None,
-        con_info: dict = None,  # 若指定，将优先使用
-        env_file_name: str = 'mysql.env',
-        silence: bool = silence_default
+        con_info: dict = None,
+        env_file_name: str = env_file_name_default,
+        silence: bool = silence_default,
+        order_dict: bool = True,
+        auto_reconnect: bool = True,
+        reconnect_wait: int = 5,
+        show_sql: bool = default_show_sql
 ):
     """
     按照sql执行
     查询结果以list(dict)形式输出
+    【包含重试机制】
+    :param sql: 参数用%s表示
+    :param parameter: 参数化查询避免sql注入
+    :param db_name:
+    :param con_info: 若指定，将优先使用
+    :param env_file_name:
+    :param silence:
+    :param order_dict:
+    :param auto_reconnect: 自动重连
+    :param reconnect_wait: 重连等待时间，单位为秒，默认为5秒
+    :param show_sql: 是否显示sql，优先级低于silence
     """
     # ---------------- 固定设置 ----------------
-    if con_info is None:
-        con_info = make_con_info(env_file_name=env_file_name)
-    else:
-        pass
-    # ---------------- 固定设置 ----------------
-    try:
-        con, cur = con2db(
-            con_info=con_info,
-            db_name=db_name,
+    if not con_info:
+        con_info = make_con_info(
+            env_file_name=env_file_name,
             silence=silence
         )
-        if silence is True:
-            try:
-                effect_rows = _query(
-                    sql=sql,
-                    parameter=parameter,
-                    cur=cur,
-                    con=con,
-                    operate=True
-                )
-                return effect_rows
-            except Exception as ex:
-                showlog.warning("Oops! an error occurred, maybe query error. Exception: %s" % ex)
-                return
+    con, cur = con2db(
+        con_info=con_info,
+        db_name=db_name,
+        silence=silence,
+        auto_reconnect=auto_reconnect,
+        reconnect_wait=reconnect_wait
+    )  # 已包含重试机制
+    # ---------------- 固定设置 ----------------
+    if not silence:
+        if show_sql:
+            showlog.info(f"Executing sql：{sql} ...")
         else:
-            showlog.info("Executing sql：%s ..." % sql)
-            try:
-                effect_rows = _query(
-                    sql=sql,
-                    parameter=parameter,
-                    cur=cur,
-                    con=con,
-                    operate=True
-                )
+            showlog.info("Executing sql ...")
+    while True:
+        try:
+            effect_rows = _query(
+                sql=sql,
+                parameter=parameter,
+                cur=cur,
+                con=con,
+                operate=True,
+                order_dict=order_dict,
+                silence=silence
+            )
+            if not silence:
                 showlog.info("Executing sql success.")
-                return effect_rows
-            except Exception as ex:
-                showlog.warning("Oops! an error occurred, maybe query error. Exception: %s" % ex)
+            return effect_rows
+        except reconnect_errors:
+            if auto_reconnect:
+                if not silence:
+                    showlog.error(f'Oops, reconnect_errors, Trying to reconnect in {reconnect_wait} seconds ...')
+                time.sleep(reconnect_wait)
+                con, cur = con2db(
+                    con_info=con_info,
+                    db_name=db_name,
+                    silence=silence,
+                    auto_reconnect=auto_reconnect,
+                    reconnect_wait=reconnect_wait
+                )  # 已包含重试机制
+            else:
                 return
-    except Exception as ex:
-        showlog.warning("Oops! an error occurred, maybe con2db error. Exception: %s" % ex)
-        return
 
 
 def data_bases(
-        con_info: dict = None,  # 若指定，将优先使用
-        env_file_name: str = 'mysql.env',
-        silence: bool = silence_default
+        con_info: dict = None,
+        env_file_name: str = env_file_name_default,
+        silence: bool = silence_default,
+        order_dict: bool = True,
+        auto_reconnect: bool = True,
+        reconnect_wait: int = 5
 ):
     """
     获取MySQL的连接权限范围内的所有db列表
+    【包含重试机制】
+    :param con_info: 若指定，将优先使用
+    :param env_file_name:
+    :param silence:
+    :param order_dict:
+    :param auto_reconnect: 自动重连
+    :param reconnect_wait: 重连等待时间，单位为秒，默认为5秒
     """
     # ---------------- 固定设置 ----------------
-    if con_info is None:
-        con_info = make_con_info(env_file_name=env_file_name)
-    else:
-        pass
-    # ---------------- 固定设置 ----------------
-    try:
-        con, cur = con2db(
-            con_info=con_info,
+    if not con_info:
+        con_info = make_con_info(
+            env_file_name=env_file_name,
             silence=silence
         )
-        sql = "SHOW DATABASES;"
-        if silence is True:
-            try:
-                res = _query(
-                    cur=cur,
-                    sql=sql
-                )
-                inner_db_list = list()
-                for each in res:
-                    for k, v in each.items():
-                        inner_db_list.append(v)
-                return inner_db_list
-            except Exception as ex:
-                showlog.warning("Oops! an error occurred, maybe query error. Exception: %s" % ex)
-                return
-        else:
-            showlog.info("Executing sql：%s ..." % sql)
-            try:
-                res = _query(
-                    cur=cur,
-                    sql=sql
-                )
+    con, cur = con2db(
+        con_info=con_info,
+        silence=silence,
+        auto_reconnect=auto_reconnect,
+        reconnect_wait=reconnect_wait
+    )  # 已包含重试机制
+    # ---------------- 固定设置 ----------------
+    sql = "SHOW DATABASES;"
+    if not silence:
+        showlog.info("Executing sql：%s ..." % sql)
+    while True:
+        try:
+            res = _query(
+                cur=cur,
+                sql=sql,
+                order_dict=order_dict,
+                silence=silence
+            )
+            if not silence:
                 showlog.info("Executing sql success.")
-                inner_db_list = list()
-                for each in res:
-                    for k, v in each.items():
-                        inner_db_list.append(v)
-                return inner_db_list
-            except Exception as ex:
-                showlog.warning("Oops! an error occurred, maybe query error. Exception: %s" % ex)
+            inner_db_list = list()
+            for each in res:
+                for k, v in each.items():
+                    inner_db_list.append(v)
+            return inner_db_list
+        except reconnect_errors:
+            if auto_reconnect:
+                if not silence:
+                    showlog.error(f'Oops, reconnect_errors, Trying to reconnect in {reconnect_wait} seconds ...')
+                time.sleep(reconnect_wait)
+                con, cur = con2db(
+                    con_info=con_info,
+                    silence=silence,
+                    auto_reconnect=auto_reconnect,
+                    reconnect_wait=reconnect_wait
+                )  # 已包含重试机制
+            else:
                 return
-    except Exception as ex:
-        showlog.warning("Oops! an error occurred, maybe con2db error. Exception: %s" % ex)
-        return
+        except Exception as ex:
+            if not silence:
+                showlog.warning("Oops! an error occurred, Exception: %s" % ex)
+            return
 
 
 def tables(
-        db_name: str = None,  # 指定数据库，若不指定，将获取所有
-        con_info: dict = None,  # 若指定，将优先使用
-        env_file_name: str = 'mysql.env',
-        silence: bool = silence_default
+        db_name: str = None,
+        con_info: dict = None,
+        env_file_name: str = env_file_name_default,
+        silence: bool = silence_default,
+        order_dict: bool = True,
+        auto_reconnect: bool = True,
+        reconnect_wait: int = 5
 ):
     """
-        获取所有表，若不指定db_name，将获取所有
+    获取所有表，若不指定db_name，将获取所有
+    【包含重试机制】
+    :param db_name: 指定数据库，若不指定，将获取所有
+    :param con_info: 若指定，将优先使用
+    :param env_file_name:
+    :param silence:
+    :param order_dict:
+    :param auto_reconnect: 自动重连
+    :param reconnect_wait: 重连等待时间，单位为秒，默认为5秒
     """
     # ---------------- 固定设置 ----------------
-    if con_info is None:
-        con_info = make_con_info(env_file_name=env_file_name)
-    else:
-        pass
-    # ---------------- 固定设置 ----------------
-    try:
-        con, cur = con2db(
-            con_info=con_info,
-            db_name=db_name,
+    if not con_info:
+        con_info = make_con_info(
+            env_file_name=env_file_name,
             silence=silence
         )
-        sql = "SHOW TABLES;"
-        if silence is True:
-            try:
-                res = _query(
-                    cur=cur,
-                    sql=sql
-                )
-                table_list = list()
-                for each in res:
-                    for k, v in each.items():
-                        table_list.append(v)
-                return table_list
-            except:
-                return
-        else:
-            showlog.info("Executing sql：%s ..." % sql)
-            try:
-                res = _query(
-                    cur=cur,
-                    sql=sql
-                )
+    con, cur = con2db(
+        con_info=con_info,
+        db_name=db_name,
+        silence=silence,
+        auto_reconnect=auto_reconnect,
+        reconnect_wait=reconnect_wait
+    )  # 已包含重试机制
+    # ---------------- 固定设置 ----------------
+    sql = "SHOW TABLES;"
+    if not silence:
+        showlog.info("Executing sql：%s ..." % sql)
+    while True:
+        try:
+            res = _query(
+                cur=cur,
+                sql=sql,
+                order_dict=order_dict,
+                silence=silence
+            )
+            if not silence:
                 showlog.info("Executing sql success.")
-                table_list = list()
-                for each in res:
-                    for k, v in each.items():
-                        table_list.append(v)
-                return table_list
-            except Exception as ex:
-                showlog.warning("Oops! an error occurred, maybe query error. Exception: %s" % ex)
+            table_list = list()
+            for each in res:
+                for k, v in each.items():
+                    table_list.append(v)
+            return table_list
+        except reconnect_errors:
+            if auto_reconnect:
+                if not silence:
+                    showlog.error(f'Oops, reconnect_errors, Trying to reconnect in {reconnect_wait} seconds ...')
+                time.sleep(reconnect_wait)
+                con, cur = con2db(
+                    con_info=con_info,
+                    db_name=db_name,
+                    silence=silence,
+                    auto_reconnect=auto_reconnect,
+                    reconnect_wait=reconnect_wait
+                )  # 已包含重试机制
+            else:
                 return
-    except Exception as ex:
-        showlog.warning("Oops! an error occurred, maybe con2db error. Exception: %s" % ex)
-        return
+        except Exception as ex:
+            if not silence:
+                showlog.warning("Oops! an error occurred, maybe query error. Exception: %s" % ex)
+            return
 
 
 def tb_info(
         db_name: str,
         tb_name: str,
-        con_info: dict = None,  # 若指定，将优先使用
-        env_file_name: str = 'mysql.env',
-        silence: bool = silence_default
+        con_info: dict = None,
+        env_file_name: str = env_file_name_default,
+        silence: bool = silence_default,
+        auto_reconnect: bool = True,
+        reconnect_wait: int = 5
 ):
     """
     输出表信息，其中：
     COLUMN_NAME：列名
     DATA_TYPE：数据类型
+    【包含重试机制】
+    :param db_name:
+    :param tb_name:
+    :param con_info: 若指定，将优先使用
+    :param env_file_name:
+    :param silence:
+    :param auto_reconnect: 自动重连
+    :param reconnect_wait: 重连等待时间，单位为秒，默认为5秒
     """
     # ---------------- 固定设置 ----------------
-    if con_info is None:
-        con_info = make_con_info(env_file_name=env_file_name)
-    else:
-        pass
+    if not con_info:
+        con_info = make_con_info(
+            env_file_name=env_file_name,
+            silence=silence
+        )
     # ---------------- 固定设置 ----------------
     where_string = "TABLE_SCHEMA='%s' and TABLE_NAME='%s'" % (db_name, tb_name)
     sql = "SELECT * FROM `information_schema`.`COLUMNS` WHERE %s" % where_string
     res = query_by_sql(
         sql=sql,
-        silence=silence,
-        con_info=con_info
+        con_info=con_info,
+        auto_reconnect=auto_reconnect,
+        reconnect_wait=reconnect_wait,
+        silence=silence
     )
     return res
 
 
 def column_list(
         db_name: str,
         tb_name: str,
         con_info: dict = None,  # 若指定，将优先使用
-        env_file_name: str = 'mysql.env',
-        silence: bool = silence_default
+        env_file_name: str = env_file_name_default,
+        silence: bool = silence_default,
+        order_dict: bool = True,
+        auto_reconnect: bool = True,
+        reconnect_wait: int = 5
 ):
+    """
+    【包含重试机制】
+    :param db_name:
+    :param tb_name:
+    :param con_info: 若指定，将优先使用
+    :param env_file_name:
+    :param silence:
+    :param order_dict:
+    :param auto_reconnect: 自动重连
+    :param reconnect_wait: 重连等待时间，单位为秒，默认为5秒
+    """
     # ---------------- 固定设置 ----------------
-    if con_info is None:
-        con_info = make_con_info(env_file_name=env_file_name)
-    else:
-        pass
-    # ---------------- 固定设置 ----------------
-    try:
-        con, cur = con2db(
-            con_info=con_info,
-            db_name=db_name,
+    if not con_info:
+        con_info = make_con_info(
+            env_file_name=env_file_name,
             silence=silence
         )
-        sql1 = """
-        SELECT
-            `COLUMN_NAME` 
-        FROM
-            `information_schema`.`COLUMNS` 
-        WHERE
-            `TABLE_SCHEMA` = %s 
-            AND `TABLE_NAME` = %s;
-        """
-        all_col_dict = _query(
-            cur=cur,
-            sql=sql1,
-            parameter=(db_name, tb_name)
-        )
-        all_col_list = list()
-        for each in all_col_dict:
-            all_col_list.append(each.get("COLUMN_NAME"))
-        sql2 = """
-        SELECT
-            `COLUMN_NAME` 
-        FROM
-            `information_schema`.`KEY_COLUMN_USAGE` 
-        WHERE
-            `TABLE_SCHEMA` = %s 
-            AND `TABLE_NAME` = %s
-        """
-        pk_col_dict = _query(
-            cur=cur,
-            sql=sql2,
-            parameter=(db_name, tb_name)
-        )
-        pk_col_list = list()
-        for each in pk_col_dict:
-            pk_col_list.append(each.get("COLUMN_NAME"))
-        data_col_list = all_col_list.copy()
-        for each in pk_col_list:
-            try:
-                data_col_list.remove(each)
-            except:
-                pass
-        return all_col_list, pk_col_list, data_col_list
-    except Exception as ex:
-        showlog.warning("Oops! an error occurred in column_list, Exception: %s" % ex)
-        return
+    con, cur = con2db(
+        con_info=con_info,
+        db_name=db_name,
+        silence=silence,
+        auto_reconnect=auto_reconnect,
+        reconnect_wait=reconnect_wait
+    )  # 已包含重试机制
+    # ---------------- 固定设置 ----------------
+    while True:
+        try:
+            sql1 = """
+            SELECT
+                `COLUMN_NAME` 
+            FROM
+                `information_schema`.`COLUMNS` 
+            WHERE
+                `TABLE_SCHEMA` = %s 
+                AND `TABLE_NAME` = %s;
+            """
+            all_col_dict = _query(
+                cur=cur,
+                sql=sql1,
+                parameter=(db_name, tb_name),
+                order_dict=order_dict,
+                silence=silence
+            )
+            all_col_list = list()
+            for each in all_col_dict:
+                all_col_list.append(each.get("COLUMN_NAME"))
+            sql2 = """
+            SELECT
+                `COLUMN_NAME` 
+            FROM
+                `information_schema`.`KEY_COLUMN_USAGE` 
+            WHERE
+                `TABLE_SCHEMA` = %s 
+                AND `TABLE_NAME` = %s
+            """
+            pk_col_dict = _query(
+                cur=cur,
+                sql=sql2,
+                parameter=(db_name, tb_name),
+                order_dict=order_dict,
+                silence=silence
+            )
+            pk_col_list = list()
+            for each in pk_col_dict:
+                pk_col_list.append(each.get("COLUMN_NAME"))
+            data_col_list = all_col_list.copy()
+            for each in pk_col_list:
+                try:
+                    data_col_list.remove(each)
+                except:
+                    pass
+            return all_col_list, pk_col_list, data_col_list
+        except reconnect_errors:
+            if auto_reconnect:
+                if not silence:
+                    showlog.error(f'Oops, reconnect_errors, Trying to reconnect in {reconnect_wait} seconds ...')
+                time.sleep(reconnect_wait)
+                con, cur = con2db(
+                    con_info=con_info,
+                    db_name=db_name,
+                    silence=silence,
+                    auto_reconnect=auto_reconnect,
+                    reconnect_wait=reconnect_wait
+                )  # 已包含重试机制
+            else:
+                return
+        except Exception as ex:
+            showlog.warning("Oops! an error occurred in column_list, Exception: %s" % ex)
+            return
 
 
 def query_to_pd(
         sql: str,
+        db_name: str = None,
         parameter=None,
         con_info: dict = None,  # 若指定，将优先使用
-        env_file_name: str = 'mysql.env',
-        silence: bool = silence_default
+        env_file_name: str = env_file_name_default,
+        silence: bool = silence_default,
+        auto_reconnect: bool = True,
+        reconnect_wait: int = 5,
+        show_sql: bool = default_show_sql
 ):
     """
     针对数据量较大的情况，将数据存储到pd中
+    【包含重试机制】
+    :param sql:
+    :param db_name:
+    :param parameter:
+    :param con_info: 若指定，将优先使用
+    :param env_file_name:
+    :param silence:
+    :param auto_reconnect: 自动重连
+    :param reconnect_wait: 重连等待时间，单位为秒，默认为5秒
+    :param show_sql: 是否显示sql，优先级低于silence
     """
     # ---------------- 固定设置 ----------------
-    if con_info is None:
-        con_info = make_con_info(env_file_name=env_file_name)
-    else:
-        pass
-    # ---------------- 固定设置 ----------------
-    try:
-        con, cur = con2db(
-            con_info=con_info,
+    if not con_info:
+        con_info = make_con_info(
+            env_file_name=env_file_name,
             silence=silence
         )
-        if parameter is None:
-            cur.execute(sql)
-        else:
-            cur.execute(sql, parameter)
+    con, cur = con2db(
+        con_info=con_info,
+        db_name=db_name,
+        silence=silence,
+        auto_reconnect=auto_reconnect,
+        reconnect_wait=reconnect_wait
+    )  # 已包含重试机制
+    # ---------------- 固定设置 ----------------
+    try:
+        cur.execute(query=sql, args=parameter)
         index = cur.description
         columns = list()
         for each in index:
             columns.append(each[0])
         result = list()
         p_bar = tqdm(cur.fetchall())
         for res in p_bar:
@@ -661,48 +809,66 @@
         return
 
 
 def information_schema(
         db_name: str,
         table_name: str,
         con_info: dict = None,  # 若指定，将优先使用
-        env_file_name: str = 'mysql.env',
-        silence: bool = silence_default
+        env_file_name: str = env_file_name_default,
+        silence: bool = silence_default,
+        auto_reconnect: bool = True,
+        reconnect_wait: int = 5
 ):
     """
     输出表信息，其中：
     COLUMN_NAME：列名
     DATA_TYPE：数据类型
+    【包含重试机制】
+    :param db_name:
+    :param table_name:
+    :param con_info: 若指定，将优先使用
+    :param env_file_name:
+    :param silence:
+    :param auto_reconnect: 自动重连
+    :param reconnect_wait: 重连等待时间，单位为秒，默认为5秒
     """
     # ---------------- 固定设置 ----------------
-    if con_info is None:
-        con_info = make_con_info(env_file_name=env_file_name)
-    else:
-        pass
+    if not con_info:
+        con_info = make_con_info(
+            env_file_name=env_file_name,
+            silence=silence
+        )
     # ---------------- 固定设置 ----------------
     where_string = "TABLE_SCHEMA='%s' and TABLE_NAME='%s'" % (db_name, table_name)
     sql = "SELECT * FROM `information_schema`.`COLUMNS` WHERE %s;" % where_string
     res = query_by_sql(
         sql=sql,
         con_info=con_info,
+        auto_reconnect=auto_reconnect,
+        reconnect_wait=reconnect_wait,
         silence=silence
     )
     return res
 
 
 def clean_data(
         data_dict_list: list,
         column_info_dict: dict,
         db_name: str,
         tb_name: str,
-        replace_space_to_none: bool = True  # 自动将空值null改为None
+        replace_space_to_none: bool = True,  # 自动将空值null改为None
 ):
     """
     功能性模块
     格式化数据
+    :param data_dict_list:
+    :param column_info_dict:
+    :param db_name:
+    :param tb_name:
+    :param replace_space_to_none:
     """
     data_dict_list_temp = copy.deepcopy(data_dict_list)  # 深度拷贝，不更改源数据
     all_col_list = column_info_dict.get('all_col_list')  # 所有列名
 
     # 按照目标表的结构格式化data_dict_list，去除额外列的数据，只保留预设列的数据
     # step1: 清洗数据
     operate_param_set = set()
@@ -744,256 +910,293 @@
                     each_data_list.append(temp_data)
         data_list.append(tuple(each_data_list))  # 转换为tuple确保不变
     data_list_single = list(set(data_list))  # set去重
     return operate_clause, data_list_single
 
 
 def replace_into(
-        data_dict_list: list,  # 数据[{},{}]
-        db_name: str,  # 数据库名
-        tb_name: str,  # 表名
-        con_info: dict = None,  # 若指定，将优先使用
-        env_file_name: str = 'mysql.env',
-        pk_col_list: list = None,  # 主键列表
-        silence: bool = silence_default
+        data_dict_list: list,
+        db_name: str,
+        tb_name: str,
+        con_info: dict = None,
+        env_file_name: str = env_file_name_default,
+        pk_col_list: list = None,
+        silence: bool = silence_default,
+        auto_reconnect: bool = True,
+        reconnect_wait: int = 5
 ):
     """
     插入和自动更新，注意，这里的更新是先对原来的数据删除，再插入，不适用于局部更新！
+    【包含重试机制】
+    :param data_dict_list: 数据[{},{}]
+    :param db_name: 数据库名
+    :param tb_name: 表名
+    :param con_info: 若指定，将优先使用
+    :param env_file_name:
+    :param pk_col_list: 主键列表
+    :param silence:
+    :param auto_reconnect: 自动重连
+    :param reconnect_wait: 重连等待时间，单位为秒，默认为5秒
     """
     # ---------------- 固定设置 ----------------
-    if con_info is None:
-        con_info = make_con_info(env_file_name=env_file_name)
-    else:
-        pass
+    if not con_info:
+        con_info = make_con_info(
+            env_file_name=env_file_name,
+            silence=silence
+        )
+    con, cur = con2db(
+        con_info=con_info,
+        db_name=db_name,
+        silence=silence,
+        auto_reconnect=auto_reconnect,
+        reconnect_wait=reconnect_wait
+    )  # 已包含重试机制
     # ---------------- 固定设置 ----------------
-    if data_dict_list is None or len(data_dict_list) == 0:
+    if not data_dict_list:
         return True
     else:
         try:
             column_info = column_list(
                 db_name=db_name,
                 tb_name=tb_name,
                 con_info=con_info,
+                auto_reconnect=auto_reconnect,
+                reconnect_wait=reconnect_wait,
                 silence=silence
             )  # 获取列名信息
-            if column_info is not None:  # 若未获取到列名信息，提示错误并退出
+            if column_info:  # 若未获取到列名信息，提示错误并退出
                 all_col_list, pk_col_list_get, data_col_list = column_info  # 获取到列名信息
                 column_info_dict = {
                     'all_col_list': all_col_list,
                     'data_col_list': data_col_list,
                 }
-                if pk_col_list is not None:
+                if pk_col_list:
                     column_info_dict['pk_col_list'] = pk_col_list  # 使用自定义主键列表
                 else:
                     column_info_dict['pk_col_list'] = pk_col_list_get  # 使用数据库中定义的主键列表
 
                 operate_clause, data_list_single = clean_data(
                     column_info_dict=column_info_dict,
                     data_dict_list=data_dict_list,
                     db_name=db_name,
-                    tb_name=tb_name
+                    tb_name=tb_name,
                 )
-                connection = con2db(
-                    con_info=con_info,
-                    db_name=db_name,
-                    silence=silence
-                )  # 连接数据库
-                if connection is not None:
-                    con, cur = connection
+                while True:
                     try:
-                        if silence is False:
+                        if not silence:
                             showlog.info('operating %s data...' % len(data_list_single))
-                        else:
-                            pass
-                        cur.executemany(operate_clause, list(data_list_single))
+                        cur.executemany(query=operate_clause, args=list(data_list_single))
                         con.commit()
-                        if silence is False:
+                        if not silence:
                             showlog.info("operate success.")
-                        else:
-                            pass
                         return True
+                    except reconnect_errors:
+                        if auto_reconnect:
+                            if not silence:
+                                showlog.error(f'Oops, reconnect_errors, Trying to reconnect in {reconnect_wait} seconds ...')
+                            time.sleep(reconnect_wait)
+                            con, cur = con2db(
+                                con_info=con_info,
+                                db_name=db_name,
+                                silence=silence,
+                                auto_reconnect=auto_reconnect,
+                                reconnect_wait=reconnect_wait
+                            )  # 已包含重试机制
+                        else:
+                            return
                     except:
-                        if silence is False:
+                        if not silence:
                             showlog.error("operate failure.operate_clause: %s" % operate_clause)
                             print(operate_clause, list(data_list_single)[0])
-                        else:
-                            pass
                         return False
-                else:
-                    if silence is False:
-                        showlog.warning("Oops! can't get connection.")
-                    else:
-                        pass
-                    return False
             else:
-                if silence is False:
+                if not silence:
                     showlog.warning("Oops! can't get column_info.")
-                else:
-                    pass
                 return False
         except:
-            if silence is False:
+            if not silence:
                 showlog.error("Oops! an error occurred!")
-            else:
-                pass
             return False
 
 
 def insert(
         data_dict_list: list,
         db_name: str,
         tb_name: str,
-        con_info: dict = None,  # 若指定，将优先使用
-        env_file_name: str = 'mysql.env',
-        replace_space_to_none: bool = True,  # 自动将空值null改为None
-        silence: bool = silence_default
+        con_info: dict = None,
+        env_file_name: str = env_file_name_default,
+        replace_space_to_none: bool = True,
+        silence: bool = silence_default,
+        auto_reconnect: bool = True,
+        reconnect_wait: int = 5
 ):
     """
     此模块的功能是插入和自动更新
+    【包含重试机制】
+    :param data_dict_list:
+    :param db_name:
+    :param tb_name:
+    :param con_info: 若指定，将优先使用
+    :param env_file_name:
+    :param replace_space_to_none: 自动将空值null改为None
+    :param silence:
+    :param auto_reconnect: 自动重连
+    :param reconnect_wait: 重连等待时间，单位为秒，默认为5秒
     """
     # ---------------- 固定设置 ----------------
-    if con_info is None:
-        con_info = make_con_info(env_file_name=env_file_name)
-    else:
-        pass
+    if not con_info:
+        con_info = make_con_info(
+            env_file_name=env_file_name,
+            silence=silence
+        )
+    con, cur = con2db(
+        con_info=con_info,
+        db_name=db_name,
+        silence=silence,
+        auto_reconnect=auto_reconnect,
+        reconnect_wait=reconnect_wait
+    )  # 已包含重试机制
     # ---------------- 固定设置 ----------------
     try:
         # 获取列名信息
         column_info = column_list(
             db_name=db_name,
             tb_name=tb_name,
             con_info=con_info,
+            auto_reconnect=auto_reconnect,
+            reconnect_wait=reconnect_wait,
             silence=silence
         )
-        if column_info is not None:  # 若未获取到列名信息，提示错误并退出
+        if column_info:  # 若未获取到列名信息，提示错误并退出
             all_col_list, pk_col_list, data_col_list = column_info  # 获取到列名信息
-            connection = con2db(
-                con_info=con_info,
-                db_name=db_name,
-                silence=silence
-            )  # 连接数据库
-            if connection is not None:
-                con, cur = connection
-                # 按照目标表的结构格式化data_dict_list，去除额外列的数据，只保留预设列的数据
-                insert_param_set = set()
-                for each_data_dict in data_dict_list:  # 遍历数据list里的所有dict
-                    each_data_dict_in = each_data_dict.copy()  # 复制一份避免发生更改dict的错误
-                    for each in each_data_dict_in:  # 遍历单个dict的所有的key
-                        if each in all_col_list:  # 若key在all_col_list中，则收集该key，否则将删除key以及对应的数据，最终得到需要插入数据的列名列表
-                            insert_param_set.add(each)
-                        else:
-                            del each_data_dict[each]
+            # 按照目标表的结构格式化data_dict_list，去除额外列的数据，只保留预设列的数据
+            insert_param_set = set()
+            for each_data_dict in data_dict_list:  # 遍历数据list里的所有dict
+                each_data_dict_in = each_data_dict.copy()  # 复制一份避免发生更改dict的错误
+                for each in each_data_dict_in:  # 遍历单个dict的所有的key
+                    if each in all_col_list:  # 若key在all_col_list中，则收集该key，否则将删除key以及对应的数据，最终得到需要插入数据的列名列表
+                        insert_param_set.add(each)
+                    else:
+                        del each_data_dict[each]
 
-                insert_param_list = list(insert_param_set)  # 生成插入参数list
-                insert_clause_tuple = "`,`".join(insert_param_list)
-                insert_data_arg_list = list()
-                for _ in insert_param_list:
-                    insert_data_arg_list.append("%s")
-                insert_data_tuple = ",".join(insert_data_arg_list)
-                # 生成插入语句模板
-                insert_clause = 'INSERT INTO `%s`.`%s`(`%s`) VALUES(%s)' % \
-                                (db_name, tb_name, insert_clause_tuple, insert_data_tuple)
-
-                # 生成插入数据tuple
-                insert_data_list = list()
-                for each_data_dict in data_dict_list:
-                    each_insert_data_list = list()
-                    for each_data_key in insert_param_list:
-                        if each_data_dict.get(each_data_key) == "":
-                            if replace_space_to_none is True:
-                                each_insert_data_list.append(None)
-                            else:
-                                each_insert_data_list.append("")
+            insert_param_list = list(insert_param_set)  # 生成插入参数list
+            insert_clause_tuple = "`,`".join(insert_param_list)
+            insert_data_arg_list = list()
+            for _ in insert_param_list:
+                insert_data_arg_list.append("%s")
+            insert_data_tuple = ",".join(insert_data_arg_list)
+            # 生成插入语句模板
+            insert_clause = f'INSERT INTO `{db_name}`.`{tb_name}`(`{insert_clause_tuple}`) VALUES({insert_data_tuple})'
+
+            # 生成插入数据tuple
+            insert_data_list = list()
+            for each_data_dict in data_dict_list:
+                each_insert_data_list = list()
+                for each_data_key in insert_param_list:
+                    if each_data_dict.get(each_data_key) == "":
+                        if replace_space_to_none is True:
+                            each_insert_data_list.append(None)
                         else:
-                            each_insert_data_list.append(each_data_dict.get(each_data_key))
-                    insert_data_list.append(tuple(each_insert_data_list))
+                            each_insert_data_list.append("")
+                    else:
+                        each_insert_data_list.append(each_data_dict.get(each_data_key))
+                insert_data_list.append(tuple(each_insert_data_list))
 
-                insert_data_list = set(insert_data_list)  # set去重
+            insert_data_list = set(insert_data_list)  # set去重
 
+            while True:
                 try:
-                    if silence is False:
+                    if not silence:
                         showlog.info('Inserting %s data...' % len(insert_data_list))
-                    else:
-                        pass
-                    cur.executemany(insert_clause, list(insert_data_list))
+                    cur.executemany(query=insert_clause, args=list(insert_data_list))
                     con.commit()
-                    if silence is False:
+                    if not silence:
                         showlog.info("Insert success.")
-                    else:
-                        pass
                     return True
+                except reconnect_errors:
+                    if auto_reconnect:
+                        if not silence:
+                            showlog.error(f'Oops, reconnect_errors, Trying to reconnect in {reconnect_wait} seconds ...')
+                        time.sleep(reconnect_wait)
+                        con, cur = con2db(
+                            con_info=con_info,
+                            db_name=db_name,
+                            silence=silence,
+                            auto_reconnect=auto_reconnect,
+                            reconnect_wait=reconnect_wait
+                        )  # 已包含重试机制
+                    else:
+                        return
                 except:
-                    if silence is False:
-                        showlog.error("Insert failure.insert_clause: %s" % insert_clause)
+                    if not silence:
+                        showlog.error("Insert failure. insert_clause: %s" % insert_clause)
                         print(insert_clause, list(insert_data_list)[0])
-                    else:
-                        pass
                     return False
-            else:
-                if silence is False:
-                    showlog.warning("Oops! can't get connection.")
-                else:
-                    pass
-                return False
         else:
-            if silence is False:
+            if not silence:
                 showlog.warning("Oops! can't get column_info.")
-            else:
-                pass
             return False
     except:
-        if silence is False:
+        if not silence:
             showlog.error("Oops! an error occurred!")
-        else:
-            return False
+        return False
 
 
 def update(
         data_dict_list: list,
         db_name: str,
         tb_name: str,
         con_info: dict = None,  # 若指定，将优先使用
-        env_file_name: str = 'mysql.env',
+        env_file_name: str = env_file_name_default,
         silence: bool = silence_default,
+        auto_reconnect: bool = True,
+        reconnect_wait: int = 5
 ):
     """
     针对MySQL的数据批量更新方法，不考虑data_dict_list为空或者无数据的情况，仅仅能批量更新，默认where条件是表格的主键，且空值不参与
     先连接目标数据库获取到目标表的结构信息
+    【包含重试机制】
     :param silence:设置上传的时候是否有提示信息
     :param con_info:连接信息
     :param env_file_name:设置连接数据库的信息
     :param db_name:需要上传到的目标数据库名称
     :param tb_name:需要上传到的目标数据表名称
     :param data_dict_list:需要上传的数据列表
+    :param auto_reconnect: 自动重连
+    :param reconnect_wait: 重连等待时间，单位为秒，默认为5秒
     :return:
     """
     # ---------------- 固定设置 ----------------
-    if con_info is None:
-        con_info = make_con_info(env_file_name=env_file_name)
-    else:
-        pass
+    if not con_info:
+        con_info = make_con_info(
+            env_file_name=env_file_name,
+            silence=silence
+        )
+    con, cur = con2db(
+        con_info=con_info,
+        db_name=db_name,
+        silence=silence,
+        auto_reconnect=auto_reconnect,
+        reconnect_wait=reconnect_wait
+    )  # 已包含重试机制
     # ---------------- 固定设置 ----------------
     try:
         # 获取列名信息
         column_info = column_list(
             db_name=db_name,
             tb_name=tb_name,
             con_info=con_info,
+            auto_reconnect=auto_reconnect,
+            reconnect_wait=reconnect_wait,
             silence=silence
         )
         if column_info is not None:  # 若未获取到列名信息，提示错误并推出
             all_col_list, pk_col_list, data_col_list = column_info  # 获取到列名信息
-            connection = con2db(
-                con_info=con_info,
-                db_name=db_name,
-                silence=silence
-            )  # 连接数据库
-            if connection is not None:
-                con, cur = connection
-                # 按照目标表的结构格式化data_dict_list，去除额外列的数据，只保留预设列的数据
+            # 按照目标表的结构格式化data_dict_list，去除额外列的数据，只保留预设列的数据
+            while True:
                 try:
                     for each_data_dict in data_dict_list:  # 遍历数据list里的所有dict
 
                         set_clause_list = list()  # set语句列表
                         for each in each_data_dict:  # 遍历单个dict的所有的key
                             if each in data_col_list:  # 若key在all_col_list中，则收集该key，否则将删除key以及对应的数据，最终得到需要更新的列名列表
                                 if each_data_dict.get(each) == "" or each_data_dict.get(each) is None:
@@ -1020,64 +1223,80 @@
                                     where_clause = "`%s`='%s'" % (each, each_data_dict.get(each).replace("'", "''"))
                                 else:
                                     where_clause = "`%s`=%s" % (each, each_data_dict.get(each))
                                 where_clause_list.append(where_clause)
                         where_string = " AND ".join(where_clause_list)  # 生成where语句完成
 
                         # where_string生成完成
-                        update_clause = 'UPDATE `%s`.`%s` SET %s WHERE %s' % \
-                                        (db_name, tb_name, set_string, where_string)
+                        update_clause = f'UPDATE `{db_name}`.`{tb_name}` SET {set_string} WHERE {where_string}'
                         # print(update_clause)
-                        cur.execute(update_clause)
-                    con.commit()
-                    return 1
-                except:
-                    if silence is False:
-                        showlog.error("Update failure with update_clause: %s" % update_clause)
+                        cur.execute(query=update_clause)
+                    return con.commit()
+                except reconnect_errors:
+                    if auto_reconnect:
+                        if not silence:
+                            showlog.error(f'Oops, reconnect_errors, Trying to reconnect in {reconnect_wait} seconds ...')
+                        time.sleep(reconnect_wait)
+                        con, cur = con2db(
+                            con_info=con_info,
+                            db_name=db_name,
+                            silence=silence,
+                            auto_reconnect=auto_reconnect,
+                            reconnect_wait=reconnect_wait
+                        )  # 已包含重试机制
                     else:
                         return
-            else:
-                if silence is False:
-                    showlog.warning("Oops! can't get connection.")
-                else:
+                except:
+                    if not silence:
+                        showlog.error("Update failure with update_clause: %s" % update_clause)
                     return
         else:
-            if silence is False:
+            if not silence:
                 showlog.warning("Oops! can't get column_info.")
-            else:
-                return
+            return
     except:
-        if silence is False:
+        if not silence:
             showlog.error("Oops! an error occurred!")
-        else:
-            return
+        return
 
 
 def show_create_table(
         db_name: str,
         tb_name: str,
         con_info: dict = None,  # 若指定，将优先使用
-        env_file_name: str = 'mysql.env',
-        silence: bool = silence_default
+        env_file_name: str = env_file_name_default,
+        silence: bool = silence_default,
+        auto_reconnect: bool = True,
+        reconnect_wait: int = 5
 ):
     """
     获取建表语句
+    【包含重试机制】
+    :param db_name:
+    :param tb_name:
+    :param con_info: 若指定，将优先使用
+    :param env_file_name:
+    :param silence:
+    :param auto_reconnect: 自动重连
+    :param reconnect_wait: 重连等待时间，单位为秒，默认为5秒
     """
     # ---------------- 固定设置 ----------------
-    if con_info is None:
-        con_info = make_con_info(env_file_name=env_file_name)
-    else:
-        pass
+    if not con_info:
+        con_info = make_con_info(
+            env_file_name=env_file_name,
+            silence=silence
+        )
     # ---------------- 固定设置 ----------------
     sql = 'SHOW CREATE TABLE `%s`.`%s`;' % (db_name, tb_name)
     res = query_by_sql(
         db_name=db_name,
         sql=sql,
         env_file_name=env_file_name,
         con_info=con_info,
+        auto_reconnect=auto_reconnect,
+        reconnect_wait=reconnect_wait,
         silence=silence
     )
-    if res is None:
-        return None
+    if res:
+        return res[0]['Create Table']
     else:
-        create_table = res[0]['Create Table']
-        return create_table
+        return
```

### Comparing `fastmysql-0.0.9/fastmysql.egg-info/PKG-INFO` & `fastmysql-0.1.0/fastmysql.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 Metadata-Version: 2.1
 Name: fastmysql
-Version: 0.0.9
+Version: 0.1.0
 Summary: make it easy to use pymysql
 Home-page: https://gitee.com/ZeroSeeker/fastmysql
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # fastmysql
 ![](https://img.shields.io/badge/Python-3.8.6-green.svg)
 
 #### 介绍
 简单快速的使用mysql
 
@@ -23,27 +19,36 @@
 软件架构说明
 
 
 #### 安装教程
 
 1.  pip安装
 ```shell script
-pip install fastmysql
+pip3 install fastmysql
 ```
 2.  pip安装（使用淘宝镜像加速）
 ```shell script
-pip install fastmysql -i https://mirrors.aliyun.com/pypi/simple
+pip3 install fastmysql -i https://mirrors.aliyun.com/pypi/simple
 ```
 
 #### 使用说明
 
 1.  demo
 ```python
 import fastmysql
-query_res = fastmysql.query_table_all_data(db_name='test', tb_name='test')
+query_res = fastmysql.query_table_all_data(
+    db_name='test', 
+    tb_name='test'
+)
+
+# 获取建表语句
+res = fastmysql.show_create_table(
+    db_name='test',
+    tb_name='test'
+)
 ```
 
 2.  防止sql注入：
 写法
 
 cursor.execute('insert into user (name,password) value (?,?)',(name,password))
 　　或者
@@ -53,7 +58,9 @@
 
 cursor.execute('insert into user (name,password) value (?,?)'%(name,password))
 　　这种写法是直接将参数拼接到sql语句中，这样数据库就容易被sql注入攻击，比如
 
 cursor.execute('select * from user where user=%s and password=%s'%(name,password))
 　　要是name和password都等于'a or 1=1'，那么这个语句会把整个user表都查询出来
 
+3.  默认环境
+- 默认使用的环境文件为：mysql.env
```

