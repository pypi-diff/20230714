# Comparing `tmp/coolmongo-1.3.5.tar.gz` & `tmp/coolmongo-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolmongo-1.3.5.tar", last modified: Sun Jul  9 06:52:08 2023, max compression
+gzip compressed data, was "coolmongo-1.3.6.tar", last modified: Fri Jul 14 17:40:25 2023, max compression
```

## Comparing `coolmongo-1.3.5.tar` & `coolmongo-1.3.6.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0    10955 2023-07-09 05:47:26.656963 coolmongo-1.3.5/LICENSE
--rw-r--r--   0        0        0     4606 2023-07-09 05:44:41.568778 coolmongo-1.3.5/README.md
--rw-r--r--   0        0        0       29 2023-04-10 03:54:46.072863 coolmongo-1.3.5/coolmongo/__init__.py
--rw-r--r--   0        0        0    18005 2023-05-25 16:58:30.727299 coolmongo-1.3.5/coolmongo/docs/index.md
--rw-r--r--   0        0        0      597 2023-07-09 06:52:03.799347 coolmongo-1.3.5/pyproject.toml
--rw-r--r--   0        0        0     4904 1970-01-01 00:00:00.000000 coolmongo-1.3.5/PKG-INFO
+-rw-r--r--   0        0        0    11038 2023-07-14 17:01:09.577742 coolmongo-1.3.6/LICENSE
+-rw-r--r--   0        0        0     4586 2023-07-14 16:01:09.190077 coolmongo-1.3.6/README.md
+-rw-r--r--   0        0        0    11357 2022-11-17 21:35:25.000000 coolmongo-1.3.6/coolmongo/Dependent Packages/pymongo/LICENSE
+-rw-r--r--   0        0        0      165 2023-06-13 11:57:21.279654 coolmongo-1.3.6/coolmongo/__init__.py
+-rw-r--r--   0        0        0    20966 2023-07-14 17:20:50.294699 coolmongo-1.3.6/coolmongo/_core.py
+-rw-r--r--   0        0        0    18005 2023-07-13 01:34:06.574194 coolmongo-1.3.6/coolmongo/docs/index.md
+-rw-r--r--   0        0        0      571 2023-07-14 17:40:24.794458 coolmongo-1.3.6/pyproject.toml
+-rw-r--r--   0        0        0     4854 1970-01-01 00:00:00.000000 coolmongo-1.3.6/PKG-INFO
```

### Comparing `coolmongo-1.3.5/LICENSE` & `coolmongo-1.3.6/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -170,18 +170,22 @@
       on Your own behalf and on Your sole responsibility, not on behalf
       of any other Contributor, and only if You agree to indemnify,
       defend, and hold each Contributor harmless for any liability
       incurred by, or claims asserted against, such Contributor by reason
       of your accepting any such warranty or additional liability.
 
    END OF TERMS AND CONDITIONS
-   
+
 
    Copyright [2023] [lcctoor.com]
 
+   author: lcctoor.com
+   domain-name: lcctoor.com
+   email: lcctoor@outlook.com
+
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
```

### Comparing `coolmongo-1.3.5/README.md` & `coolmongo-1.3.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 # 项目描述
 
-史上最优雅的 MongoDB ORM 。
+全球最优雅的 MongoDB ORM 。
 
-# 安装与教程
+# 关于作者
+
+作者：lcctoor.com
 
-安装：`pip install coolmongo`
+域名：lcctoor.com
+
+邮箱：lcctoor@outlook.com
 
-[教程](https://github.com/lcctoor/lccpy/blob/main/packages/coolmongo/coolmongo/docs/index.md)
+[主页](https://lcctoor.github.io/me/) \| [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) \| [Python交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) \| [捐赠](https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg)
 
 # Bug提交、功能提议
 
 您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) 与我联系。
 
-# 关于作者
-
-作者：lcctoor.com
+# 安装
 
-邮箱：lcctoor@outlook.com
+```
+pip install coolmongo
+```
 
-[主页](https://lcctoor.github.io/me/) | [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) | [Python交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) | [捐赠](https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg)
+# [教程](https://lcctoor.github.io/lccpy/?doc=coolmongo)
 
 # 教程预览
 
 #### 导入
 
 ```python
 from pymongo import MongoClient
```

### Comparing `coolmongo-1.3.5/coolmongo/docs/index.md` & `coolmongo-1.3.6/coolmongo/docs/index.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # 项目描述
 
-史上最优雅的 MongoDB ORM 。
+全球最优雅的 MongoDB ORM 。
 
-本文将以最简洁的方式向你介绍核心知识，而不会让你被繁琐的概念所淹没。
+本文将以最简洁的方式向你介绍核心知识，而不会让你被繁琐的术语所淹没。
 
 # 安装
 
 ```cpp
 pip install coolmongo
 ```
```

### Comparing `coolmongo-1.3.5/pyproject.toml` & `coolmongo-1.3.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "coolmongo"
-version = "1.3.5"
-description = "史上最优雅的 MongoDB ORM"
-dependencies = ["lccpy >=1.4.7.1"]
+version = "1.3.6"
+description = "全球最优雅的 MongoDB ORM"
+dependencies = ["pymongo"]
 keywords = ["coolmongo", "pymongo", "mongodb", "orm"]
 
 readme = "README.md"
 authors = [{name = "lcctoor.com", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
 
 [project.urls]
-HomePage = "https://github.com/lcctoor/lccpy/tree/main/packages/coolmongo#readme"
+HomePage = "https://lcctoor.github.io/lccpy/?package=coolmongo"
```

### Comparing `coolmongo-1.3.5/PKG-INFO` & `coolmongo-1.3.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 Metadata-Version: 2.1
 Name: coolmongo
-Version: 1.3.5
-Summary: 史上最优雅的 MongoDB ORM
+Version: 1.3.6
+Summary: 全球最优雅的 MongoDB ORM
 Keywords: coolmongo,pymongo,mongodb,orm
 Author-email: "lcctoor.com" <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: lccpy >=1.4.7.1
-Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/coolmongo#readme
+Requires-Dist: pymongo
+Project-URL: HomePage, https://lcctoor.github.io/lccpy/?package=coolmongo
 
 # 项目描述
 
-史上最优雅的 MongoDB ORM 。
+全球最优雅的 MongoDB ORM 。
 
-# 安装与教程
+# 关于作者
+
+作者：lcctoor.com
 
-安装：`pip install coolmongo`
+域名：lcctoor.com
+
+邮箱：lcctoor@outlook.com
 
-[教程](https://github.com/lcctoor/lccpy/blob/main/packages/coolmongo/coolmongo/docs/index.md)
+[主页](https://lcctoor.github.io/me/) \| [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) \| [Python交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) \| [捐赠](https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg)
 
 # Bug提交、功能提议
 
 您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) 与我联系。
 
-# 关于作者
-
-作者：lcctoor.com
+# 安装
 
-邮箱：lcctoor@outlook.com
+```
+pip install coolmongo
+```
 
-[主页](https://lcctoor.github.io/me/) | [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) | [Python交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) | [捐赠](https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg)
+# [教程](https://lcctoor.github.io/lccpy/?doc=coolmongo)
 
 # 教程预览
 
 #### 导入
 
 ```python
 from pymongo import MongoClient
```

