# Comparing `tmp/asymysql-1.3.5.tar.gz` & `tmp/asymysql-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asymysql-1.3.5.tar", last modified: Sun Jul  9 06:50:50 2023, max compression
+gzip compressed data, was "asymysql-1.3.6.tar", last modified: Fri Jul 14 17:40:35 2023, max compression
```

## Comparing `asymysql-1.3.5.tar` & `asymysql-1.3.6.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0    10955 2023-07-09 05:47:26.657966 asymysql-1.3.5/LICENSE
--rw-r--r--   0        0        0     4399 2023-07-09 05:44:41.576785 asymysql-1.3.5/README.md
--rw-r--r--   0        0        0       28 2023-04-10 03:48:57.281686 asymysql-1.3.5/asymysql/__init__.py
--rw-r--r--   0        0        0    18318 2023-06-14 09:12:35.228575 asymysql-1.3.5/asymysql/docs/index.md
--rw-r--r--   0        0        0      593 2023-07-09 06:50:40.631134 asymysql-1.3.5/pyproject.toml
--rw-r--r--   0        0        0     4668 1970-01-01 00:00:00.000000 asymysql-1.3.5/PKG-INFO
+-rw-r--r--   0        0        0    11038 2023-07-14 17:01:09.592746 asymysql-1.3.6/LICENSE
+-rw-r--r--   0        0        0     4380 2023-07-14 16:02:17.215282 asymysql-1.3.6/README.md
+-rw-r--r--   0        0        0     1070 2022-05-08 19:03:55.000000 asymysql-1.3.6/asymysql/Dependent Packages/aiomysql/LICENSE
+-rw-r--r--   0        0        0       86 2023-06-13 11:57:21.290462 asymysql-1.3.6/asymysql/__init__.py
+-rw-r--r--   0        0        0    22840 2023-07-14 17:14:22.804339 asymysql-1.3.6/asymysql/_core.py
+-rw-r--r--   0        0        0    18330 2023-07-10 14:06:26.043080 asymysql-1.3.6/asymysql/docs/index.md
+-rw-r--r--   0        0        0      568 2023-07-14 17:40:35.485931 asymysql-1.3.6/pyproject.toml
+-rw-r--r--   0        0        0     4620 1970-01-01 00:00:00.000000 asymysql-1.3.6/PKG-INFO
```

### Comparing `asymysql-1.3.5/LICENSE` & `asymysql-1.3.6/LICENSE`

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

### Comparing `asymysql-1.3.5/README.md` & `asymysql-1.3.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 # 项目描述
 
 异步的 mysql ORM 。
 
-# 安装与教程
+# 关于作者
+
+作者：lcctoor.com
 
-安装：`pip install asymysql`
+域名：lcctoor.com
+
+邮箱：lcctoor@outlook.com
 
-[教程](https://github.com/lcctoor/lccpy/blob/main/packages/asymysql/asymysql/docs/index.md)
+[主页](https://lcctoor.github.io/me/) \| [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) \| [Python交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) \| [捐赠](https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg)
 
 # Bug提交、功能提议
 
 您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) 与我联系。
 
-# 关于作者
-
-作者：lcctoor.com
+# 安装
 
-邮箱：lcctoor@outlook.com
+```
+pip install asymysql
+```
 
-[主页](https://lcctoor.github.io/me/) | [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) | [Python交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) | [捐赠](https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg)
+# [教程](https://lcctoor.github.io/lccpy/?doc=asymysql)
 
 # 教程预览
 
 #### 导入
 
 ```python
 from aiomysql import connect
```

### Comparing `asymysql-1.3.5/asymysql/docs/index.md` & `asymysql-1.3.6/asymysql/docs/index.md`

 * *Files 1% similar despite different names*

```diff
@@ -310,15 +310,15 @@
 await _[:]  # 切片
 ```
 
 注：无论过滤器多复杂，ORM都不会访问数据库，只有在最后切片时，ORM才会访问数据库。
 
 # 排序
 
-对所有年龄>12的数据，优先按年龄降序，其次按姓名升序，排序后返回第2\~4条数据：
+对所有年级为“高一”的数据，优先按年龄降序，其次按姓名升序，排序后返回第2\~4条数据：
 
 ```python
 await sheet[mc.年级=='高一'].order(年龄=False, 姓名=True)[2:4]
 ```
 
 有趣的，以下两行代码的返回结果相同：
```

### Comparing `asymysql-1.3.5/PKG-INFO` & `asymysql-1.3.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 Metadata-Version: 2.1
 Name: asymysql
-Version: 1.3.5
+Version: 1.3.6
 Summary: 异步的 mysql ORM
 Keywords: asymysql,aiomysql,mysql,pymysql,orm
 Author-email: "lcctoor.com" <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: lccpy >=1.4.7.1
-Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/asymysql#readme
+Requires-Dist: aiomysql
+Project-URL: HomePage, https://lcctoor.github.io/lccpy/?package=asymysql
 
 # 项目描述
 
 异步的 mysql ORM 。
 
-# 安装与教程
+# 关于作者
+
+作者：lcctoor.com
 
-安装：`pip install asymysql`
+域名：lcctoor.com
+
+邮箱：lcctoor@outlook.com
 
-[教程](https://github.com/lcctoor/lccpy/blob/main/packages/asymysql/asymysql/docs/index.md)
+[主页](https://lcctoor.github.io/me/) \| [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) \| [Python交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) \| [捐赠](https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg)
 
 # Bug提交、功能提议
 
 您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) 与我联系。
 
-# 关于作者
-
-作者：lcctoor.com
+# 安装
 
-邮箱：lcctoor@outlook.com
+```
+pip install asymysql
+```
 
-[主页](https://lcctoor.github.io/me/) | [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) | [Python交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) | [捐赠](https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg)
+# [教程](https://lcctoor.github.io/lccpy/?doc=asymysql)
 
 # 教程预览
 
 #### 导入
 
 ```python
 from aiomysql import connect
```

