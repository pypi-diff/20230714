# Comparing `tmp/increment-1.3.4.tar.gz` & `tmp/increment-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "increment-1.3.4.tar", last modified: Sun Jul  9 06:53:47 2023, max compression
+gzip compressed data, was "increment-1.3.5.tar", last modified: Fri Jul 14 17:39:32 2023, max compression
```

## Comparing `increment-1.3.4.tar` & `increment-1.3.5.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0    10953 2023-07-09 05:47:26.656963 increment-1.3.4/LICENSE
--rw-r--r--   0        0        0     1218 2023-07-09 05:44:41.558583 increment-1.3.4/README.md
--rw-r--r--   0        0        0       29 2023-04-10 04:01:47.110396 increment-1.3.4/increment.py
--rw-r--r--   0        0        0      610 2023-07-09 06:53:41.700858 increment-1.3.4/pyproject.toml
--rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 increment-1.3.4/PKG-INFO
+-rw-r--r--   0        0        0    11036 2023-07-14 17:01:09.603744 increment-1.3.5/LICENSE
+-rw-r--r--   0        0        0     1245 2023-07-14 14:42:06.504365 increment-1.3.5/README.md
+-rw-r--r--   0        0        0       30 2023-06-25 03:07:54.283832 increment-1.3.5/increment/__init__.py
+-rw-r--r--   0        0        0     1639 2023-07-14 17:14:22.805335 increment-1.3.5/increment/_core.py
+-rw-r--r--   0        0        0      577 2023-07-14 17:39:32.243960 increment-1.3.5/pyproject.toml
+-rw-r--r--   0        0        0     1586 1970-01-01 00:00:00.000000 increment-1.3.5/PKG-INFO
```

### Comparing `increment-1.3.4/LICENSE` & `increment-1.3.5/LICENSE`

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

### Comparing `increment-1.3.4/README.md` & `increment-1.3.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # 项目描述
 
 分布式主键生成器，支持多机器|多进程|多线程并发生成。
 
-# 安装
+# 关于作者
 
-```
-pip install increment
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
+pip install increment
+```
 
 # 教程
 
 #### 导入
 
 ```python
 from increment import incrementer
```

### Comparing `increment-1.3.4/pyproject.toml` & `increment-1.3.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "increment"
-version = "1.3.4"
+version = "1.3.5"
 description = "分布式主键生成器，支持多机器|多进程|多线程并发生成"
-dependencies = ["lccpy >=1.4.7"]
+dependencies = []
 keywords = ["increment"]
 
 readme = "README.md"
 authors = [{name = "lcctoor.com", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
 
 [project.urls]
-HomePage = "https://github.com/lcctoor/lccpy/tree/main/packages/increment#readme"
+HomePage = "https://lcctoor.github.io/lccpy/?package=increment"
```

### Comparing `increment-1.3.4/PKG-INFO` & `increment-1.3.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 Metadata-Version: 2.1
 Name: increment
-Version: 1.3.4
+Version: 1.3.5
 Summary: 分布式主键生成器，支持多机器|多进程|多线程并发生成
 Keywords: increment
 Author-email: "lcctoor.com" <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: lccpy >=1.4.7
-Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/increment#readme
+Project-URL: HomePage, https://lcctoor.github.io/lccpy/?package=increment
 
 # 项目描述
 
 分布式主键生成器，支持多机器|多进程|多线程并发生成。
 
-# 安装
+# 关于作者
 
-```
-pip install increment
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
+pip install increment
+```
 
 # 教程
 
 #### 导入
 
 ```python
 from increment import incrementer
```

