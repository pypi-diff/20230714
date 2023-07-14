# Comparing `tmp/df2mysql-0.0.2.tar.gz` & `tmp/df2mysql-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "df2mysql-0.0.2.tar", last modified: Fri Jul 14 09:12:33 2023, max compression
+gzip compressed data, was "df2mysql-0.0.3.tar", last modified: Fri Jul 14 09:18:14 2023, max compression
```

## Comparing `df2mysql-0.0.2.tar` & `df2mysql-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 09:12:33.490831 df2mysql-0.0.2/
--rw-rw-rw-   0        0        0     1056 2023-07-14 08:46:20.000000 df2mysql-0.0.2/LICENSE
--rw-rw-rw-   0        0        0        0 2023-07-14 08:47:12.000000 df2mysql-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3085 2023-07-14 09:12:33.488838 df2mysql-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1706 2023-07-14 08:41:15.000000 df2mysql-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 09:12:33.413040 df2mysql-0.0.2/df2mysql/
--rw-rw-rw-   0        0        0       29 2023-07-14 09:06:44.000000 df2mysql-0.0.2/df2mysql/__init__.py
--rw-rw-rw-   0        0        0     8733 2023-02-20 07:52:23.000000 df2mysql-0.0.2/df2mysql/database.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:12:33.486842 df2mysql-0.0.2/df2mysql.egg-info/
--rw-rw-rw-   0        0        0     3085 2023-07-14 09:12:33.000000 df2mysql-0.0.2/df2mysql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-07-14 09:12:33.000000 df2mysql-0.0.2/df2mysql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 09:12:33.000000 df2mysql-0.0.2/df2mysql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-14 09:01:30.000000 df2mysql-0.0.2/df2mysql.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       15 2023-07-14 09:12:33.000000 df2mysql-0.0.2/df2mysql.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-14 09:12:33.000000 df2mysql-0.0.2/df2mysql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1427 2023-07-14 09:12:16.000000 df2mysql-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-14 09:12:33.490831 df2mysql-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1577 2023-07-14 09:12:20.000000 df2mysql-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:18:14.912637 df2mysql-0.0.3/
+-rw-rw-rw-   0        0        0     1056 2023-07-14 08:46:20.000000 df2mysql-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-07-14 08:47:12.000000 df2mysql-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3085 2023-07-14 09:18:14.910642 df2mysql-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1706 2023-07-14 08:41:15.000000 df2mysql-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 09:18:14.860774 df2mysql-0.0.3/df2mysql/
+-rw-rw-rw-   0        0        0       32 2023-07-14 09:15:46.000000 df2mysql-0.0.3/df2mysql/__init__.py
+-rw-rw-rw-   0        0        0     8733 2023-02-20 07:52:23.000000 df2mysql-0.0.3/df2mysql/database.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:18:14.909644 df2mysql-0.0.3/df2mysql.egg-info/
+-rw-rw-rw-   0        0        0     3085 2023-07-14 09:18:14.000000 df2mysql-0.0.3/df2mysql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-07-14 09:18:14.000000 df2mysql-0.0.3/df2mysql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 09:18:14.000000 df2mysql-0.0.3/df2mysql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-14 09:01:30.000000 df2mysql-0.0.3/df2mysql.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       15 2023-07-14 09:18:14.000000 df2mysql-0.0.3/df2mysql.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-14 09:18:14.000000 df2mysql-0.0.3/df2mysql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1427 2023-07-14 09:17:28.000000 df2mysql-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-14 09:18:14.912637 df2mysql-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1577 2023-07-14 09:17:24.000000 df2mysql-0.0.3/setup.py
```

### Comparing `df2mysql-0.0.2/LICENSE` & `df2mysql-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `df2mysql-0.0.2/PKG-INFO` & `df2mysql-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: df2mysql
-Version: 0.0.2
+Version: 0.0.3
 Summary: 提供了一组方法，用于与 Microsoft SQL Server 数据库进行交互。允许执行各种操作，如连接到 SQL Server、创建和删除数据库、创建和删除表、添加和删除列、插入和检索数据等。
 Home-page: https://github.com/ng-fukgin/df2mysql
 Author: wfj
 Author-email: wfj <wfj.0000@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/ng-fukgin/df2mysql
 Project-URL: repository, https://github.com/ng-fukgin/df2mysql
```

### Comparing `df2mysql-0.0.2/README.md` & `df2mysql-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `df2mysql-0.0.2/df2mysql/database.py` & `df2mysql-0.0.3/df2mysql/database.py`

 * *Files identical despite different names*

### Comparing `df2mysql-0.0.2/df2mysql.egg-info/PKG-INFO` & `df2mysql-0.0.3/df2mysql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: df2mysql
-Version: 0.0.2
+Version: 0.0.3
 Summary: 提供了一组方法，用于与 Microsoft SQL Server 数据库进行交互。允许执行各种操作，如连接到 SQL Server、创建和删除数据库、创建和删除表、添加和删除列、插入和检索数据等。
 Home-page: https://github.com/ng-fukgin/df2mysql
 Author: wfj
 Author-email: wfj <wfj.0000@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/ng-fukgin/df2mysql
 Project-URL: repository, https://github.com/ng-fukgin/df2mysql
```

### Comparing `df2mysql-0.0.2/pyproject.toml` & `df2mysql-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "df2mysql"
-version = "0.0.2"
+version = "0.0.3"
 description = "提供了一组方法，用于与 Microsoft SQL Server 数据库进行交互。允许执行各种操作，如连接到 SQL Server、创建和删除数据库、创建和删除表、添加和删除列、插入和检索数据等。"
 readme = "README.md"
 authors = [{ name = "wfj", email = "wfj.0000@gmail.com" }]
 keywords = ["df2mysql", "Microsoft SQL Server", "数据库交互", "数据库连接", "数据库操作", "数据库管理"]
 license = { text = "MIT" }
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `df2mysql-0.0.2/setup.py` & `df2mysql-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='df2mysql',
-    version='0.0.2',
+    version='0.0.3',
     author='wfj',
     author_email='wfj.0000@gmail.com',
     description='提供了一组方法，用于与 Microsoft SQL Server 数据库进行交互。允许执行各种操作，如连接到 SQL Server、创建和删除数据库、创建和删除表、添加和删除列、插入和检索数据等。',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/ng-fukgin/df2mysql',
     classifiers=[
```

