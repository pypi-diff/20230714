# Comparing `tmp/envname-1.0.3.tar.gz` & `tmp/envname-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "envname-1.0.3.tar", last modified: Sun Jul  9 06:53:28 2023, max compression
+gzip compressed data, was "envname-1.0.4.tar", last modified: Fri Jul 14 17:43:26 2023, max compression
```

## Comparing `envname-1.0.3.tar` & `envname-1.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    10953 2023-07-09 05:47:26.637967 envname-1.0.3/LICENSE
--rw-r--r--   0        0        0     1533 2023-07-09 05:44:41.566784 envname-1.0.3/README.md
--rw-r--r--   0        0        0      647 2023-07-09 05:47:26.638963 envname-1.0.3/envname/__init__.py
--rw-r--r--   0        0        0      102 2023-05-01 17:24:53.385434 envname-1.0.3/envname/_envname.py
--rw-r--r--   0        0        0      585 2023-07-09 06:53:23.550155 envname-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1831 1970-01-01 00:00:00.000000 envname-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11036 2023-07-14 17:01:09.596759 envname-1.0.4/LICENSE
+-rw-r--r--   0        0        0     1560 2023-07-14 14:42:06.488996 envname-1.0.4/README.md
+-rw-r--r--   0        0        0      698 2023-07-14 17:14:22.784588 envname-1.0.4/envname/__init__.py
+-rw-r--r--   0        0        0      102 2023-05-01 17:24:53.385434 envname-1.0.4/envname/_envname.py
+-rw-r--r--   0        0        0      567 2023-07-14 17:43:25.877677 envname-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1838 1970-01-01 00:00:00.000000 envname-1.0.4/PKG-INFO
```

### Comparing `envname-1.0.3/LICENSE` & `envname-1.0.4/LICENSE`

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

### Comparing `envname-1.0.3/README.md` & `envname-1.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # 项目描述
 
 为运行环境设置名称。
 
 有时候，对于某些功能，我们也许希望在不同的环境上采用不同的方案。以访问数据库为例：当程序在外网运行时，须通过数据库公网ip访问；而当程序在内网运行时，为了提高性能，我们可以通过数据库内网ip访问。
 
-# 安装
+# 关于作者
 
-```
-pip install envname
-```
+作者：lcctoor.com
 
-# Bug提交、功能提议
+域名：lcctoor.com
 
-您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) 与我联系。
+邮箱：lcctoor@outlook.com
 
-# 关于作者
+[主页](https://lcctoor.github.io/me/) \| [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) \| [Python交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) \| [捐赠](https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg)
 
-作者：lcctoor.com
+# Bug提交、功能提议
 
-邮箱：lcctoor@outlook.com
+您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) 与我联系。
 
-[主页](https://lcctoor.github.io/me/) | [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) | [Python交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) | [捐赠](https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg)
+# 安装
+
+```
+pip install envname
+```
 
 # 教程
 
 #### 创建环境名称
 
 （cmd）：
```

### Comparing `envname-1.0.3/pyproject.toml` & `envname-1.0.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "envname"
-version = "1.0.3"
+version = "1.0.4"
 description = "为运行环境设置名称"
 dependencies = []
 keywords = []
 
 readme = "README.md"
 authors = [{name = "lcctoor.com", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
 
 [project.scripts]
 envname = "envname:_parsecmd"
 
 [project.urls]
-HomePage = "https://github.com/lcctoor/lccpy/tree/main/packages/envname#readme"
+HomePage = "https://lcctoor.github.io/lccpy/?package=envname"
```

### Comparing `envname-1.0.3/PKG-INFO` & `envname-1.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 Metadata-Version: 2.1
 Name: envname
-Version: 1.0.3
+Version: 1.0.4
 Summary: 为运行环境设置名称
 Keywords: 
 Author-email: "lcctoor.com" <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/envname#readme
+Project-URL: HomePage, https://lcctoor.github.io/lccpy/?package=envname
 
 # 项目描述
 
 为运行环境设置名称。
 
 有时候，对于某些功能，我们也许希望在不同的环境上采用不同的方案。以访问数据库为例：当程序在外网运行时，须通过数据库公网ip访问；而当程序在内网运行时，为了提高性能，我们可以通过数据库内网ip访问。
 
-# 安装
+# 关于作者
 
-```
-pip install envname
-```
+作者：lcctoor.com
 
-# Bug提交、功能提议
+域名：lcctoor.com
 
-您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) 与我联系。
+邮箱：lcctoor@outlook.com
 
-# 关于作者
+[主页](https://lcctoor.github.io/me/) \| [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) \| [Python交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) \| [捐赠](https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg)
 
-作者：lcctoor.com
+# Bug提交、功能提议
 
-邮箱：lcctoor@outlook.com
+您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) 与我联系。
 
-[主页](https://lcctoor.github.io/me/) | [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) | [Python交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) | [捐赠](https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg)
+# 安装
+
+```
+pip install envname
+```
 
 # 教程
 
 #### 创建环境名称
 
 （cmd）：
```

