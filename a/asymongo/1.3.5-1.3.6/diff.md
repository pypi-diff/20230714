# Comparing `tmp/asymongo-1.3.5.tar.gz` & `tmp/asymongo-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asymongo-1.3.5.tar", last modified: Sun Jul  9 06:50:25 2023, max compression
+gzip compressed data, was "asymongo-1.3.6.tar", last modified: Fri Jul 14 17:40:46 2023, max compression
```

## Comparing `asymongo-1.3.5.tar` & `asymongo-1.3.6.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0    10955 2023-07-09 05:47:26.664960 asymongo-1.3.5/LICENSE
--rw-r--r--   0        0        0     4744 2023-07-09 05:44:41.576785 asymongo-1.3.5/README.md
--rw-r--r--   0        0        0       28 2023-04-10 03:40:07.519027 asymongo-1.3.5/asymongo/__init__.py
--rw-r--r--   0        0        0    16892 2023-04-25 13:09:33.999319 asymongo-1.3.5/asymongo/docs/index.md
--rw-r--r--   0        0        0      594 2023-07-09 06:49:31.623756 asymongo-1.3.5/pyproject.toml
--rw-r--r--   0        0        0     5034 1970-01-01 00:00:00.000000 asymongo-1.3.5/PKG-INFO
+-rw-r--r--   0        0        0    11038 2023-07-14 17:01:09.592746 asymongo-1.3.6/LICENSE
+-rw-r--r--   0        0        0     4725 2023-07-14 16:02:32.343243 asymongo-1.3.6/README.md
+-rw-r--r--   0        0        0    11357 2022-10-25 20:46:40.000000 asymongo-1.3.6/asymongo/Dependent Packages/motor/LICENSE
+-rw-r--r--   0        0        0      165 2023-06-13 11:57:21.300071 asymongo-1.3.6/asymongo/__init__.py
+-rw-r--r--   0        0        0    20548 2023-07-14 17:14:22.800337 asymongo-1.3.6/asymongo/_core.py
+-rw-r--r--   0        0        0    16892 2023-04-25 13:09:33.999319 asymongo-1.3.6/asymongo/docs/index.md
+-rw-r--r--   0        0        0      566 2023-07-14 17:40:46.602391 asymongo-1.3.6/pyproject.toml
+-rw-r--r--   0        0        0     4983 1970-01-01 00:00:00.000000 asymongo-1.3.6/PKG-INFO
```

### Comparing `asymongo-1.3.5/LICENSE` & `asymongo-1.3.6/LICENSE`

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

### Comparing `asymongo-1.3.5/README.md` & `asymongo-1.3.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 # 项目描述
 
 异步的 MongoDB ORM 。
 
-# 安装与教程
+# 关于作者
+
+作者：lcctoor.com
 
-安装：`pip install asymongo`
+域名：lcctoor.com
+
+邮箱：lcctoor@outlook.com
 
-[教程](https://github.com/lcctoor/lccpy/blob/main/packages/asymongo/asymongo/docs/index.md)
+[主页](https://lcctoor.github.io/me/) \| [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) \| [Python交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) \| [捐赠](https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg)
 
 # Bug提交、功能提议
 
 您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) 与我联系。
 
-# 关于作者
-
-作者：lcctoor.com
+# 安装
 
-邮箱：lcctoor@outlook.com
+```
+pip install asymongo
+```
 
-[主页](https://lcctoor.github.io/me/) | [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) | [Python交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) | [捐赠](https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg)
+# [教程](https://lcctoor.github.io/lccpy/?doc=asymongo)
 
 # 教程预览
 
 #### 导入
 
 ```python
 from motor.motor_asyncio import AsyncIOMotorClient as MongoClient
```

### Comparing `asymongo-1.3.5/asymongo/docs/index.md` & `asymongo-1.3.6/asymongo/docs/index.md`

 * *Files identical despite different names*

### Comparing `asymongo-1.3.5/pyproject.toml` & `asymongo-1.3.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "asymongo"
-version = "1.3.5"
+version = "1.3.6"
 description = "异步的 MongoDB ORM"
-dependencies = ["lccpy >=1.4.7.1"]
+dependencies = ["motor"]
 keywords = ["asymongo", "motor", "mongodb", "pymongo", "orm"]
 
 readme = "README.md"
 authors = [{name = "lcctoor.com", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
 
 [project.urls]
-HomePage = "https://github.com/lcctoor/lccpy/tree/main/packages/asymongo#readme"
+HomePage = "https://lcctoor.github.io/lccpy/?package=asymongo"
```

### Comparing `asymongo-1.3.5/PKG-INFO` & `asymongo-1.3.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 Metadata-Version: 2.1
 Name: asymongo
-Version: 1.3.5
+Version: 1.3.6
 Summary: 异步的 MongoDB ORM
 Keywords: asymongo,motor,mongodb,pymongo,orm
 Author-email: "lcctoor.com" <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: lccpy >=1.4.7.1
-Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/asymongo#readme
+Requires-Dist: motor
+Project-URL: HomePage, https://lcctoor.github.io/lccpy/?package=asymongo
 
 # 项目描述
 
 异步的 MongoDB ORM 。
 
-# 安装与教程
+# 关于作者
+
+作者：lcctoor.com
 
-安装：`pip install asymongo`
+域名：lcctoor.com
+
+邮箱：lcctoor@outlook.com
 
-[教程](https://github.com/lcctoor/lccpy/blob/main/packages/asymongo/asymongo/docs/index.md)
+[主页](https://lcctoor.github.io/me/) \| [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) \| [Python交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) \| [捐赠](https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg)
 
 # Bug提交、功能提议
 
 您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) 与我联系。
 
-# 关于作者
-
-作者：lcctoor.com
+# 安装
 
-邮箱：lcctoor@outlook.com
+```
+pip install asymongo
+```
 
-[主页](https://lcctoor.github.io/me/) | [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) | [Python交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) | [捐赠](https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg)
+# [教程](https://lcctoor.github.io/lccpy/?doc=asymongo)
 
 # 教程预览
 
 #### 导入
 
 ```python
 from motor.motor_asyncio import AsyncIOMotorClient as MongoClient
```

