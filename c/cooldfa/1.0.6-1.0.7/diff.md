# Comparing `tmp/cooldfa-1.0.6.tar.gz` & `tmp/cooldfa-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cooldfa-1.0.6.tar", last modified: Sun Jul  9 06:51:37 2023, max compression
+gzip compressed data, was "cooldfa-1.0.7.tar", last modified: Fri Jul 14 17:37:35 2023, max compression
```

## Comparing `cooldfa-1.0.6.tar` & `cooldfa-1.0.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    10953 2023-07-09 05:47:26.657966 cooldfa-1.0.6/LICENSE
--rw-r--r--   0        0        0     1514 2023-07-09 05:44:41.573781 cooldfa-1.0.6/README.md
--rw-r--r--   0        0        0       39 2023-04-03 14:28:11.266714 cooldfa-1.0.6/cooldfa/__init__.py
--rw-r--r--   0        0        0     3663 2023-07-09 05:47:26.657966 cooldfa-1.0.6/cooldfa/_cooldfa.py
--rw-r--r--   0        0        0   478756 2023-04-30 19:24:41.305728 cooldfa-1.0.6/cooldfa/_words/others.json
--rw-r--r--   0        0        0    23188 2023-04-30 19:24:41.308762 cooldfa-1.0.6/cooldfa/_words/politics.json
--rw-r--r--   0        0        0    10325 2023-04-30 19:24:41.311777 cooldfa-1.0.6/cooldfa/_words/sex.json
--rw-r--r--   0        0        0   262857 2023-04-30 19:24:41.330728 cooldfa-1.0.6/cooldfa/_words/url.json
--rw-r--r--   0        0        0     4015 2023-04-30 19:24:41.331729 cooldfa-1.0.6/cooldfa/_words/violence.json
--rw-r--r--   0        0        0      561 2023-07-09 06:51:29.375709 cooldfa-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     1833 1970-01-01 00:00:00.000000 cooldfa-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11036 2023-07-14 17:01:09.603744 cooldfa-1.0.7/LICENSE
+-rw-r--r--   0        0        0     1541 2023-07-14 14:42:06.504365 cooldfa-1.0.7/README.md
+-rw-r--r--   0        0        0       39 2023-04-03 14:28:11.266714 cooldfa-1.0.7/cooldfa/__init__.py
+-rw-r--r--   0        0        0     3690 2023-07-14 17:14:22.805335 cooldfa-1.0.7/cooldfa/_cooldfa.py
+-rw-r--r--   0        0        0   478756 2023-04-30 19:24:41.305728 cooldfa-1.0.7/cooldfa/_words/others.json
+-rw-r--r--   0        0        0    23188 2023-04-30 19:24:41.308762 cooldfa-1.0.7/cooldfa/_words/politics.json
+-rw-r--r--   0        0        0    10325 2023-04-30 19:24:41.311777 cooldfa-1.0.7/cooldfa/_words/sex.json
+-rw-r--r--   0        0        0   262857 2023-04-30 19:24:41.330728 cooldfa-1.0.7/cooldfa/_words/url.json
+-rw-r--r--   0        0        0     4015 2023-04-30 19:24:41.331729 cooldfa-1.0.7/cooldfa/_words/violence.json
+-rw-r--r--   0        0        0      543 2023-07-14 17:37:34.560278 cooldfa-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1840 1970-01-01 00:00:00.000000 cooldfa-1.0.7/PKG-INFO
```

### Comparing `cooldfa-1.0.6/LICENSE` & `cooldfa-1.0.7/LICENSE`

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

### Comparing `cooldfa-1.0.6/README.md` & `cooldfa-1.0.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # 项目描述
 
 基于 DFA 算法的敏感词检测器。
 
-# 安装
+# 关于作者
 
-```
-pip install cooldfa
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
+pip install cooldfa
+```
 
 # 教程
 
 #### 导入
 
 ```python
 from cooldfa import dfa
```

### Comparing `cooldfa-1.0.6/cooldfa/_cooldfa.py` & `cooldfa-1.0.7/cooldfa/_cooldfa.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,20 @@
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
 from json import loads
 from pathlib import Path
-from typing import Any
 
 
 # 预置忽略词
 preset_ignore_words = set('''
     `-_=~!@#$%^&*()+[ ]\\{}|;\',./:"<>?·！￥…（）—【】、；‘：“，。《》？
     ～＆＠＃”’〝〞＂＇´﹞﹝＞＜«»‹›〔〕〈〉』『〗〖｝｛」「］［︵︷︹︿︽﹁﹃︻︗＼｜／︘︼﹄﹂︾﹀︺︸︶＿﹏﹍﹎
     \n\r \t¦¡\xad¨ˊ¯￣﹋﹉﹊ˋ︴¿ˇ\u3000
```

### Comparing `cooldfa-1.0.6/cooldfa/_words/others.json` & `cooldfa-1.0.7/cooldfa/_words/others.json`

 * *Files identical despite different names*

### Comparing `cooldfa-1.0.6/cooldfa/_words/politics.json` & `cooldfa-1.0.7/cooldfa/_words/politics.json`

 * *Files identical despite different names*

### Comparing `cooldfa-1.0.6/cooldfa/_words/sex.json` & `cooldfa-1.0.7/cooldfa/_words/sex.json`

 * *Files identical despite different names*

### Comparing `cooldfa-1.0.6/cooldfa/_words/url.json` & `cooldfa-1.0.7/cooldfa/_words/url.json`

 * *Files identical despite different names*

### Comparing `cooldfa-1.0.6/cooldfa/_words/violence.json` & `cooldfa-1.0.7/cooldfa/_words/violence.json`

 * *Files identical despite different names*

### Comparing `cooldfa-1.0.6/pyproject.toml` & `cooldfa-1.0.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "cooldfa"
-version = "1.0.6"
+version = "1.0.7"
 description = "基于 DFA 算法的敏感词检测器"
 dependencies = []
 keywords = ["cooldfa", "dfa"]
 
 readme = "README.md"
 authors = [{name = "lcctoor.com", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.10"
 
 [project.urls]
-HomePage = "https://github.com/lcctoor/lccpy/tree/main/packages/cooldfa#readme"
+HomePage = "https://lcctoor.github.io/lccpy/?package=cooldfa"
```

### Comparing `cooldfa-1.0.6/PKG-INFO` & `cooldfa-1.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 Metadata-Version: 2.1
 Name: cooldfa
-Version: 1.0.6
+Version: 1.0.7
 Summary: 基于 DFA 算法的敏感词检测器
 Keywords: cooldfa,dfa
 Author-email: "lcctoor.com" <lcctoor@outlook.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/cooldfa#readme
+Project-URL: HomePage, https://lcctoor.github.io/lccpy/?package=cooldfa
 
 # 项目描述
 
 基于 DFA 算法的敏感词检测器。
 
-# 安装
+# 关于作者
 
-```
-pip install cooldfa
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
+pip install cooldfa
+```
 
 # 教程
 
 #### 导入
 
 ```python
 from cooldfa import dfa
```

