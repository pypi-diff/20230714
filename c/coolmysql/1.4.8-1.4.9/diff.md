# Comparing `tmp/coolmysql-1.4.8.tar.gz` & `tmp/coolmysql-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolmysql-1.4.8.tar", last modified: Sun Jul  9 06:52:29 2023, max compression
+gzip compressed data, was "coolmysql-1.4.9.tar", last modified: Fri Jul 14 17:40:13 2023, max compression
```

## Comparing `coolmysql-1.4.8.tar` & `coolmysql-1.4.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    10955 2023-07-09 05:47:26.656963 coolmysql-1.4.8/LICENSE
--rw-r--r--   0        0        0     3833 2023-07-09 05:44:41.571802 coolmysql-1.4.8/README.md
--rw-r--r--   0        0        0     1070 2013-11-27 14:43:24.000000 coolmysql-1.4.8/coolmysql/Dependent Packages/pymysql/LICENSE
--rw-r--r--   0        0        0       86 2023-06-13 11:57:21.279654 coolmysql-1.4.8/coolmysql/__init__.py
--rw-r--r--   0        0        0    23082 2023-07-09 06:02:16.006639 coolmysql-1.4.8/coolmysql/_core.py
--rw-r--r--   0        0        0    18748 2023-06-14 09:13:53.682433 coolmysql-1.4.8/coolmysql/docs/index.md
--rw-r--r--   0        0        0      597 2023-07-09 06:52:25.076919 coolmysql-1.4.8/pyproject.toml
--rw-r--r--   0        0        0     4126 1970-01-01 00:00:00.000000 coolmysql-1.4.8/PKG-INFO
+-rw-r--r--   0        0        0    11038 2023-07-14 17:01:35.003848 coolmysql-1.4.9/LICENSE
+-rw-r--r--   0        0        0     3813 2023-07-14 16:00:04.111500 coolmysql-1.4.9/README.md
+-rw-r--r--   0        0        0     1070 2013-11-27 14:43:24.000000 coolmysql-1.4.9/coolmysql/Dependent Packages/pymysql/LICENSE
+-rw-r--r--   0        0        0       86 2023-06-13 11:57:21.279654 coolmysql-1.4.9/coolmysql/__init__.py
+-rw-r--r--   0        0        0    23133 2023-07-14 17:14:22.805335 coolmysql-1.4.9/coolmysql/_core.py
+-rw-r--r--   0        0        0    18760 2023-07-13 01:34:06.580190 coolmysql-1.4.9/coolmysql/docs/index.md
+-rw-r--r--   0        0        0      579 2023-07-14 17:40:12.808422 coolmysql-1.4.9/pyproject.toml
+-rw-r--r--   0        0        0     4084 1970-01-01 00:00:00.000000 coolmysql-1.4.9/PKG-INFO
```

### Comparing `coolmysql-1.4.8/LICENSE` & `coolmysql-1.4.9/LICENSE`

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

### Comparing `coolmysql-1.4.8/README.md` & `coolmysql-1.4.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 # 项目描述
 
-史上最优雅的 mysql ORM 。
+全球最优雅的 mysql ORM 。
 
-# 安装与教程
+# 关于作者
+
+作者：lcctoor.com
 
-安装：`pip install coolmysql`
+域名：lcctoor.com
+
+邮箱：lcctoor@outlook.com
 
-[教程](https://github.com/lcctoor/lccpy/blob/main/packages/coolmysql/coolmysql/docs/index.md)
+[主页](https://lcctoor.github.io/me/) \| [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) \| [Python交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) \| [捐赠](https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg)
 
 # Bug提交、功能提议
 
 您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) 与我联系。
 
-# 关于作者
-
-作者：lcctoor.com
+# 安装
 
-邮箱：lcctoor@outlook.com
+```
+pip install coolmysql
+```
 
-[主页](https://lcctoor.github.io/me/) | [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) | [Python交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) | [捐赠](https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg)
+# [教程](https://lcctoor.github.io/lccpy/?doc=coolmysql)
 
 # 教程预览
 
 #### 导入
 
 ```python
 from pymysql import connect
```

### Comparing `coolmysql-1.4.8/coolmysql/Dependent Packages/pymysql/LICENSE` & `coolmysql-1.4.9/coolmysql/Dependent Packages/pymysql/LICENSE`

 * *Files identical despite different names*

### Comparing `coolmysql-1.4.8/coolmysql/_core.py` & `coolmysql-1.4.9/coolmysql/_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 '''
 Copyright [2023] [lcctoor.com]
+
 license: Apache License, Version 2.0
+
+author: lcctoor.com
+domain-name: lcctoor.com
 email: lcctoor@outlook.com
 '''
 
 from copy import deepcopy
 from collections import deque
 from pymysql import connect  # 代码提示
 from pymysql.cursors import DictCursor
```

### Comparing `coolmysql-1.4.8/coolmysql/docs/index.md` & `coolmysql-1.4.9/coolmysql/docs/index.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # 项目描述
 
-史上最优雅的 mysql ORM 。
+全球最优雅的 mysql ORM 。
 
-本文将以最简洁的方式向你介绍核心知识，而不会让你被繁琐的概念所淹没。
+本文将以最简洁的方式向你介绍核心知识，而不会让你被繁琐的术语所淹没。
 
 # 安装
 
 ```cpp
 pip install coolmysql
 ```
 
@@ -269,15 +269,15 @@
 _[:]  # 切片
 ```
 
 注：无论过滤器多复杂，ORM都不会访问数据库，只有在最后切片时，ORM才会访问数据库。
 
 # 排序
 
-对所有年龄>12的数据，优先按年龄降序，其次按姓名升序，排序后返回第2\~4条数据：
+对所有年级为“高一”的数据，优先按年龄降序，其次按姓名升序，排序后返回第2\~4条数据：
 
 ```python
 sheet[mc.年级=='高一'].order(年龄=False, 姓名=True)[2:4]
 ```
 
 有趣的，以下两行代码的返回结果相同：
```

### Comparing `coolmysql-1.4.8/PKG-INFO` & `coolmysql-1.4.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 Metadata-Version: 2.1
 Name: coolmysql
-Version: 1.4.8
-Summary: 史上最优雅的 mysql ORM
+Version: 1.4.9
+Summary: 全球最优雅的 mysql ORM
 Keywords: coolmysql,pymysql,mysql,aiomysql,orm
 Author-email: "lcctoor.com" <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: pymysql
-Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/coolmysql#readme
+Project-URL: HomePage, https://lcctoor.github.io/lccpy/?package=coolmysql
 
 # 项目描述
 
-史上最优雅的 mysql ORM 。
+全球最优雅的 mysql ORM 。
 
-# 安装与教程
+# 关于作者
+
+作者：lcctoor.com
 
-安装：`pip install coolmysql`
+域名：lcctoor.com
+
+邮箱：lcctoor@outlook.com
 
-[教程](https://github.com/lcctoor/lccpy/blob/main/packages/coolmysql/coolmysql/docs/index.md)
+[主页](https://lcctoor.github.io/me/) \| [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) \| [Python交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) \| [捐赠](https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg)
 
 # Bug提交、功能提议
 
 您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) 与我联系。
 
-# 关于作者
-
-作者：lcctoor.com
+# 安装
 
-邮箱：lcctoor@outlook.com
+```
+pip install coolmysql
+```
 
-[主页](https://lcctoor.github.io/me/) | [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) | [Python交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) | [捐赠](https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg)
+# [教程](https://lcctoor.github.io/lccpy/?doc=coolmysql)
 
 # 教程预览
 
 #### 导入
 
 ```python
 from pymysql import connect
```

