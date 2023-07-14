# Comparing `tmp/rstyleslice-1.4.4.tar.gz` & `tmp/rstyleslice-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rstyleslice-1.4.4.tar", last modified: Sun Jul  9 06:54:50 2023, max compression
+gzip compressed data, was "rstyleslice-1.4.5.tar", last modified: Fri Jul 14 17:43:07 2023, max compression
```

## Comparing `rstyleslice-1.4.4.tar` & `rstyleslice-1.4.5.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0    10953 2023-07-09 05:47:26.599959 rstyleslice-1.4.4/LICENSE
--rw-r--r--   0        0        0     2916 2023-07-09 05:44:41.558583 rstyleslice-1.4.4/README.md
--rw-r--r--   0        0        0      595 2023-07-09 06:54:44.459762 rstyleslice-1.4.4/pyproject.toml
--rw-r--r--   0        0        0       31 2023-04-10 04:03:01.139197 rstyleslice-1.4.4/rstyleslice/__init__.py
--rw-r--r--   0        0        0     5794 2023-04-25 13:10:59.200573 rstyleslice-1.4.4/rstyleslice/docs/index.md
--rw-r--r--   0        0        0     3265 1970-01-01 00:00:00.000000 rstyleslice-1.4.4/PKG-INFO
+-rw-r--r--   0        0        0    11036 2023-07-14 17:01:09.599742 rstyleslice-1.4.5/LICENSE
+-rw-r--r--   0        0        0     2894 2023-07-14 16:01:58.187221 rstyleslice-1.4.5/README.md
+-rw-r--r--   0        0        0      560 2023-07-14 17:43:06.838290 rstyleslice-1.4.5/pyproject.toml
+-rw-r--r--   0        0        0       25 2023-07-13 08:31:53.164510 rstyleslice-1.4.5/rstyleslice/__init__.py
+-rw-r--r--   0        0        0     2956 2023-07-14 17:14:22.785588 rstyleslice-1.4.5/rstyleslice/_core.py
+-rw-r--r--   0        0        0     5794 2023-04-25 13:10:59.200573 rstyleslice-1.4.5/rstyleslice/docs/index.md
+-rw-r--r--   0        0        0     3190 1970-01-01 00:00:00.000000 rstyleslice-1.4.5/PKG-INFO
```

### Comparing `rstyleslice-1.4.4/LICENSE` & `rstyleslice-1.4.5/LICENSE`

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

### Comparing `rstyleslice-1.4.4/README.md` & `rstyleslice-1.4.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -6,31 +6,35 @@
 | -------------------------------------- | -------------------------------------------------------------------------- | -------------------------------------------------------------------------- |
 | **索引**                         | 从 0 开始（0 表示第 1 个元素）<br /><br />-1 表示倒数第 1 个元素（相同点） | 从 1 开始（1 表示第 1 个元素）<br /><br />-1 表示倒数第 1 个元素（相同点） |
 | **切片**                         | 左闭右开区间，例如：<br />[3: 5] 表示提取第 4、5 这 2 个元素               | 双闭区间，例如：<br />[3: 5] 表示提取第 3、4、5 这 3 个元素                |
 | **从右往**<br />**左切片** | step（步长）为负值，例如：<br />[9: 1: -1] 表示提取第 9~3 这 7 个元素      | step（步长）始终为正值，例如：<br />[9: 1: 1] 表示提取第 9~1 这 9 个元素   |
 
 切片格式为  [start: stop: step]  ，start 表示从哪条开始，stop 表示到哪条停止，step 表示步长。当  step>=2  时表示间隔式切片。
 
-# 安装与教程
+# 关于作者
+
+作者：lcctoor.com
 
-安装：`pip install rstyleslice`
+域名：lcctoor.com
+
+邮箱：lcctoor@outlook.com
 
-[教程](https://github.com/lcctoor/lccpy/blob/main/packages/rstyleslice/rstyleslice/docs/index.md)
+[主页](https://lcctoor.github.io/me/) \| [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) \| [Python交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) \| [捐赠](https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg)
 
 # Bug提交、功能提议
 
 您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) 与我联系。
 
-# 关于作者
-
-作者：lcctoor.com
+# 安装
 
-邮箱：lcctoor@outlook.com
+```
+pip install rstyleslice
+```
 
-[主页](https://lcctoor.github.io/me/) | [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) | [Python交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) | [捐赠](https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg)
+# [教程](https://lcctoor.github.io/lccpy/?doc=rstyleslice)
 
 # 教程预览
 
 #### 导入
 
 ```python
 from rstyleslice import rslice
```

### Comparing `rstyleslice-1.4.4/pyproject.toml` & `rstyleslice-1.4.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "rstyleslice"
-version = "1.4.4"
+version = "1.4.5"
 description = "一套符合直觉的索引和切片语法"
-dependencies = ["lccpy >=1.4.7.1"]
+dependencies = []
 keywords = ["rstyleslice", "slice"]
 
 readme = "README.md"
 authors = [{name = "lcctoor.com", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
 
 [project.urls]
-HomePage = "https://github.com/lcctoor/lccpy/tree/main/packages/rstyleslice#readme"
+HomePage = "https://lcctoor.github.io/lccpy/?package=rstyleslice"
```

### Comparing `rstyleslice-1.4.4/rstyleslice/docs/index.md` & `rstyleslice-1.4.5/rstyleslice/docs/index.md`

 * *Files identical despite different names*

### Comparing `rstyleslice-1.4.4/PKG-INFO` & `rstyleslice-1.4.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 Metadata-Version: 2.1
 Name: rstyleslice
-Version: 1.4.4
+Version: 1.4.5
 Summary: 一套符合直觉的索引和切片语法
 Keywords: rstyleslice,slice
 Author-email: "lcctoor.com" <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: lccpy >=1.4.7.1
-Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/rstyleslice#readme
+Project-URL: HomePage, https://lcctoor.github.io/lccpy/?package=rstyleslice
 
 # 项目描述
 
 一套符合直觉的索引和切片语法。
 
 |                                        | **Python**                                                           | **rstyleslice**                                                      |
 | -------------------------------------- | -------------------------------------------------------------------------- | -------------------------------------------------------------------------- |
 | **索引**                         | 从 0 开始（0 表示第 1 个元素）<br /><br />-1 表示倒数第 1 个元素（相同点） | 从 1 开始（1 表示第 1 个元素）<br /><br />-1 表示倒数第 1 个元素（相同点） |
 | **切片**                         | 左闭右开区间，例如：<br />[3: 5] 表示提取第 4、5 这 2 个元素               | 双闭区间，例如：<br />[3: 5] 表示提取第 3、4、5 这 3 个元素                |
 | **从右往**<br />**左切片** | step（步长）为负值，例如：<br />[9: 1: -1] 表示提取第 9~3 这 7 个元素      | step（步长）始终为正值，例如：<br />[9: 1: 1] 表示提取第 9~1 这 9 个元素   |
 
 切片格式为  [start: stop: step]  ，start 表示从哪条开始，stop 表示到哪条停止，step 表示步长。当  step>=2  时表示间隔式切片。
 
-# 安装与教程
+# 关于作者
+
+作者：lcctoor.com
 
-安装：`pip install rstyleslice`
+域名：lcctoor.com
+
+邮箱：lcctoor@outlook.com
 
-[教程](https://github.com/lcctoor/lccpy/blob/main/packages/rstyleslice/rstyleslice/docs/index.md)
+[主页](https://lcctoor.github.io/me/) \| [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) \| [Python交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) \| [捐赠](https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg)
 
 # Bug提交、功能提议
 
 您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) 与我联系。
 
-# 关于作者
-
-作者：lcctoor.com
+# 安装
 
-邮箱：lcctoor@outlook.com
+```
+pip install rstyleslice
+```
 
-[主页](https://lcctoor.github.io/me/) | [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) | [Python交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) | [捐赠](https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg)
+# [教程](https://lcctoor.github.io/lccpy/?doc=rstyleslice)
 
 # 教程预览
 
 #### 导入
 
 ```python
 from rstyleslice import rslice
```

