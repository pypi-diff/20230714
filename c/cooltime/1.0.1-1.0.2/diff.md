# Comparing `tmp/cooltime-1.0.1.tar.gz` & `tmp/cooltime-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cooltime-1.0.1.tar", last modified: Sun Jul  9 06:52:50 2023, max compression
+gzip compressed data, was "cooltime-1.0.2.tar", last modified: Fri Jul 14 17:40:59 2023, max compression
```

## Comparing `cooltime-1.0.1.tar` & `cooltime-1.0.2.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0    10953 2023-07-09 05:47:26.656963 cooltime-1.0.1/LICENSE
--rw-r--r--   0        0        0     3511 2023-07-09 05:44:41.566784 cooltime-1.0.1/README.md
--rw-r--r--   0        0        0       28 2023-06-25 08:04:00.811074 cooltime-1.0.1/cooltime.py
--rw-r--r--   0        0        0      559 2023-07-09 06:52:44.343597 cooltime-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3818 1970-01-01 00:00:00.000000 cooltime-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11036 2023-07-14 17:01:09.603744 cooltime-1.0.2/LICENSE
+-rw-r--r--   0        0        0     3547 2023-07-14 14:42:06.504365 cooltime-1.0.2/README.md
+-rw-r--r--   0        0        0       27 2023-06-25 08:02:23.228282 cooltime-1.0.2/cooltime/__init__.py
+-rw-r--r--   0        0        0     2823 2023-07-14 17:14:22.805335 cooltime-1.0.2/cooltime/_core.py
+-rw-r--r--   0        0        0      533 2023-07-14 17:40:59.535325 cooltime-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3812 1970-01-01 00:00:00.000000 cooltime-1.0.2/PKG-INFO
```

### Comparing `cooltime-1.0.1/LICENSE` & `cooltime-1.0.2/LICENSE`

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

### Comparing `cooltime-1.0.1/README.md` & `cooltime-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # 项目描述
 
-人性化的时间模块。
+全球最人性化的时间模块。
 
-# 安装
+# 关于作者
 
-```
-pip install cooltime
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
+pip install cooltime
+```
 
 # 教程
 
 #### 导入
 
 ```python
 from cooltime import cooltime
```

### Comparing `cooltime-1.0.1/pyproject.toml` & `cooltime-1.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "cooltime"
-version = "1.0.1"
-description = "人性化的时间模块"
-dependencies = ["lccpy >=1.4.7.1"]
+version = "1.0.2"
+description = "全球最人性化的时间模块"
+dependencies = []
 keywords = ["cooltime"]
 
 readme = "README.md"
 authors = [{name = "lcctoor.com", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
 
 [project.urls]
-HomePage = "https://github.com/lcctoor/lccpy/tree/main/packages/cooltime#readme"
+HomePage = "https://lcctoor.github.io/lccpy/?package=cooltime"
```

### Comparing `cooltime-1.0.1/PKG-INFO` & `cooltime-1.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 Metadata-Version: 2.1
 Name: cooltime
-Version: 1.0.1
-Summary: 人性化的时间模块
+Version: 1.0.2
+Summary: 全球最人性化的时间模块
 Keywords: cooltime
 Author-email: "lcctoor.com" <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: lccpy >=1.4.7.1
-Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/cooltime#readme
+Project-URL: HomePage, https://lcctoor.github.io/lccpy/?package=cooltime
 
 # 项目描述
 
-人性化的时间模块。
+全球最人性化的时间模块。
 
-# 安装
+# 关于作者
 
-```
-pip install cooltime
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
+pip install cooltime
+```
 
 # 教程
 
 #### 导入
 
 ```python
 from cooltime import cooltime
```

