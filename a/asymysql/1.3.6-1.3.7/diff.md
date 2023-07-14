# Comparing `tmp/asymysql-1.3.6.tar.gz` & `tmp/asymysql-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asymysql-1.3.6.tar", last modified: Fri Jul 14 17:40:35 2023, max compression
+gzip compressed data, was "asymysql-1.3.7.tar", last modified: Fri Jul 14 18:47:29 2023, max compression
```

## Comparing `asymysql-1.3.6.tar` & `asymysql-1.3.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11038 2023-07-14 17:01:09.592746 asymysql-1.3.6/LICENSE
--rw-r--r--   0        0        0     4380 2023-07-14 16:02:17.215282 asymysql-1.3.6/README.md
--rw-r--r--   0        0        0     1070 2022-05-08 19:03:55.000000 asymysql-1.3.6/asymysql/Dependent Packages/aiomysql/LICENSE
--rw-r--r--   0        0        0       86 2023-06-13 11:57:21.290462 asymysql-1.3.6/asymysql/__init__.py
--rw-r--r--   0        0        0    22840 2023-07-14 17:14:22.804339 asymysql-1.3.6/asymysql/_core.py
--rw-r--r--   0        0        0    18330 2023-07-10 14:06:26.043080 asymysql-1.3.6/asymysql/docs/index.md
--rw-r--r--   0        0        0      568 2023-07-14 17:40:35.485931 asymysql-1.3.6/pyproject.toml
--rw-r--r--   0        0        0     4620 1970-01-01 00:00:00.000000 asymysql-1.3.6/PKG-INFO
+-rw-r--r--   0        0        0    11038 2023-07-14 17:01:09.592746 asymysql-1.3.7/LICENSE
+-rw-r--r--   0        0        0     4380 2023-07-14 16:02:17.215282 asymysql-1.3.7/README.md
+-rw-r--r--   0        0        0     1070 2022-05-08 19:03:55.000000 asymysql-1.3.7/asymysql/Dependent Packages/aiomysql/LICENSE
+-rw-r--r--   0        0        0       86 2023-06-13 11:57:21.290462 asymysql-1.3.7/asymysql/__init__.py
+-rw-r--r--   0        0        0    22840 2023-07-14 17:14:22.804339 asymysql-1.3.7/asymysql/_core.py
+-rw-r--r--   0        0        0    18330 2023-07-10 14:06:26.043080 asymysql-1.3.7/asymysql/docs/index.md
+-rw-r--r--   0        0        0      589 2023-07-14 18:47:29.179717 asymysql-1.3.7/pyproject.toml
+-rw-r--r--   0        0        0     4665 1970-01-01 00:00:00.000000 asymysql-1.3.7/PKG-INFO
```

### Comparing `asymysql-1.3.6/LICENSE` & `asymysql-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `asymysql-1.3.6/README.md` & `asymysql-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `asymysql-1.3.6/asymysql/Dependent Packages/aiomysql/LICENSE` & `asymysql-1.3.7/asymysql/Dependent Packages/aiomysql/LICENSE`

 * *Files identical despite different names*

### Comparing `asymysql-1.3.6/asymysql/_core.py` & `asymysql-1.3.7/asymysql/_core.py`

 * *Files identical despite different names*

### Comparing `asymysql-1.3.6/asymysql/docs/index.md` & `asymysql-1.3.7/asymysql/docs/index.md`

 * *Files identical despite different names*

### Comparing `asymysql-1.3.6/pyproject.toml` & `asymysql-1.3.7/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "asymysql"
-version = "1.3.6"
+version = "1.3.7"
 description = "异步的 mysql ORM"
-dependencies = ["aiomysql"]
+dependencies = ["aiomysql", "vtype", "coolfunc"]
 keywords = ["asymysql", "aiomysql", "mysql", "pymysql", "orm"]
 
 readme = "README.md"
 authors = [{name = "lcctoor.com", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
```

### Comparing `asymysql-1.3.6/PKG-INFO` & `asymysql-1.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: asymysql
-Version: 1.3.6
+Version: 1.3.7
 Summary: 异步的 mysql ORM
 Keywords: asymysql,aiomysql,mysql,pymysql,orm
 Author-email: "lcctoor.com" <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: aiomysql
+Requires-Dist: vtype
+Requires-Dist: coolfunc
 Project-URL: HomePage, https://lcctoor.github.io/lccpy/?package=asymysql
 
 # 项目描述
 
 异步的 mysql ORM 。
 
 # 关于作者
```

