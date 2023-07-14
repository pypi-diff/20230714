# Comparing `tmp/coolmongo-1.3.6.tar.gz` & `tmp/coolmongo-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolmongo-1.3.6.tar", last modified: Fri Jul 14 17:40:25 2023, max compression
+gzip compressed data, was "coolmongo-1.3.7.tar", last modified: Fri Jul 14 18:47:19 2023, max compression
```

## Comparing `coolmongo-1.3.6.tar` & `coolmongo-1.3.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11038 2023-07-14 17:01:09.577742 coolmongo-1.3.6/LICENSE
--rw-r--r--   0        0        0     4586 2023-07-14 16:01:09.190077 coolmongo-1.3.6/README.md
--rw-r--r--   0        0        0    11357 2022-11-17 21:35:25.000000 coolmongo-1.3.6/coolmongo/Dependent Packages/pymongo/LICENSE
--rw-r--r--   0        0        0      165 2023-06-13 11:57:21.279654 coolmongo-1.3.6/coolmongo/__init__.py
--rw-r--r--   0        0        0    20966 2023-07-14 17:20:50.294699 coolmongo-1.3.6/coolmongo/_core.py
--rw-r--r--   0        0        0    18005 2023-07-13 01:34:06.574194 coolmongo-1.3.6/coolmongo/docs/index.md
--rw-r--r--   0        0        0      571 2023-07-14 17:40:24.794458 coolmongo-1.3.6/pyproject.toml
--rw-r--r--   0        0        0     4854 1970-01-01 00:00:00.000000 coolmongo-1.3.6/PKG-INFO
+-rw-r--r--   0        0        0    11038 2023-07-14 17:01:09.577742 coolmongo-1.3.7/LICENSE
+-rw-r--r--   0        0        0     4586 2023-07-14 16:01:09.190077 coolmongo-1.3.7/README.md
+-rw-r--r--   0        0        0    11357 2022-11-17 21:35:25.000000 coolmongo-1.3.7/coolmongo/Dependent Packages/pymongo/LICENSE
+-rw-r--r--   0        0        0      165 2023-06-13 11:57:21.279654 coolmongo-1.3.7/coolmongo/__init__.py
+-rw-r--r--   0        0        0    20966 2023-07-14 17:20:50.294699 coolmongo-1.3.7/coolmongo/_core.py
+-rw-r--r--   0        0        0    18005 2023-07-13 01:34:06.574194 coolmongo-1.3.7/coolmongo/docs/index.md
+-rw-r--r--   0        0        0      580 2023-07-14 18:47:19.418088 coolmongo-1.3.7/pyproject.toml
+-rw-r--r--   0        0        0     4875 1970-01-01 00:00:00.000000 coolmongo-1.3.7/PKG-INFO
```

### Comparing `coolmongo-1.3.6/LICENSE` & `coolmongo-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `coolmongo-1.3.6/README.md` & `coolmongo-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `coolmongo-1.3.6/coolmongo/Dependent Packages/pymongo/LICENSE` & `coolmongo-1.3.7/coolmongo/Dependent Packages/pymongo/LICENSE`

 * *Files identical despite different names*

### Comparing `coolmongo-1.3.6/coolmongo/_core.py` & `coolmongo-1.3.7/coolmongo/_core.py`

 * *Files identical despite different names*

### Comparing `coolmongo-1.3.6/coolmongo/docs/index.md` & `coolmongo-1.3.7/coolmongo/docs/index.md`

 * *Files identical despite different names*

### Comparing `coolmongo-1.3.6/PKG-INFO` & `coolmongo-1.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: coolmongo
-Version: 1.3.6
+Version: 1.3.7
 Summary: 全球最优雅的 MongoDB ORM
 Keywords: coolmongo,pymongo,mongodb,orm
 Author-email: "lcctoor.com" <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: pymongo
+Requires-Dist: vtype
 Project-URL: HomePage, https://lcctoor.github.io/lccpy/?package=coolmongo
 
 # 项目描述
 
 全球最优雅的 MongoDB ORM 。
 
 # 关于作者
```

