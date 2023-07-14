# Comparing `tmp/coolapi-1.0.2.tar.gz` & `tmp/coolapi-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolapi-1.0.2.tar", last modified: Sun Jul  9 06:51:13 2023, max compression
+gzip compressed data, was "coolapi-1.0.3.tar", last modified: Fri Jul 14 17:41:10 2023, max compression
```

## Comparing `coolapi-1.0.2.tar` & `coolapi-1.0.3.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0    10953 2023-07-09 05:47:26.657966 coolapi-1.0.2/LICENSE
--rw-r--r--   0        0        0     4726 2023-07-09 05:44:41.573781 coolapi-1.0.2/README.md
--rw-r--r--   0        0        0       27 2023-06-12 17:15:32.722578 coolapi-1.0.2/coolapi.py
--rw-r--r--   0        0        0      621 2023-07-09 06:51:05.798923 coolapi-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     5011 1970-01-01 00:00:00.000000 coolapi-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11036 2023-07-14 17:01:09.603744 coolapi-1.0.3/LICENSE
+-rw-r--r--   0        0        0     4753 2023-07-14 14:41:56.896108 coolapi-1.0.3/README.md
+-rw-r--r--   0        0        0    11358 2023-05-14 02:53:10.000000 coolapi-1.0.3/coolapi/Dependent Packages/tornado/LICENSE
+-rw-r--r--   0        0        0       40 2023-05-28 06:10:27.855895 coolapi-1.0.3/coolapi/__init__.py
+-rw-r--r--   0        0        0     1721 2023-07-14 17:14:22.794781 coolapi-1.0.3/coolapi/_core.py
+-rw-r--r--   0        0        0      597 2023-07-14 17:41:10.084495 coolapi-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5012 1970-01-01 00:00:00.000000 coolapi-1.0.3/PKG-INFO
```

### Comparing `coolapi-1.0.2/LICENSE` & `coolapi-1.0.3/LICENSE`

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

### Comparing `coolapi-1.0.2/README.md` & `coolapi-1.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # 项目描述
 
 简单好用的异步 web 框架。
 
-# 安装
+# 关于作者
 
-```
-pip install coolapi
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
+pip install coolapi
+```
 
 # 教程
 
 #### 导入
 
 ```python
 import asyncio
```

### Comparing `coolapi-1.0.2/pyproject.toml` & `coolapi-1.0.3/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "coolapi"
-version = "1.0.2"
+version = "1.0.3"
 description = "简单好用的异步 web 框架"
-dependencies = ["lccpy >=1.4.7"]
+dependencies = ["tornado"]
 keywords = ["coolapi", "tornado", "flask", "fastapi", "django", "aiohttp", "web"]
 
 readme = "README.md"
 authors = [{name = "lcctoor.com", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
 
 [project.urls]
-HomePage = "https://github.com/lcctoor/lccpy/tree/main/packages/coolapi#readme"
+HomePage = "https://lcctoor.github.io/lccpy/?package=coolapi"
```

### Comparing `coolapi-1.0.2/PKG-INFO` & `coolapi-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 Metadata-Version: 2.1
 Name: coolapi
-Version: 1.0.2
+Version: 1.0.3
 Summary: 简单好用的异步 web 框架
 Keywords: coolapi,tornado,flask,fastapi,django,aiohttp,web
 Author-email: "lcctoor.com" <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: lccpy >=1.4.7
-Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/coolapi#readme
+Requires-Dist: tornado
+Project-URL: HomePage, https://lcctoor.github.io/lccpy/?package=coolapi
 
 # 项目描述
 
 简单好用的异步 web 框架。
 
-# 安装
+# 关于作者
 
-```
-pip install coolapi
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
+pip install coolapi
+```
 
 # 教程
 
 #### 导入
 
 ```python
 import asyncio
```

