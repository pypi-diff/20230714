# Comparing `tmp/encrypt256-1.8.4.tar.gz` & `tmp/encrypt256-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encrypt256-1.8.4.tar", last modified: Sun Jul  9 06:53:09 2023, max compression
+gzip compressed data, was "encrypt256-1.8.5.tar", last modified: Fri Jul 14 17:39:46 2023, max compression
```

## Comparing `encrypt256-1.8.4.tar` & `encrypt256-1.8.5.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0    10953 2023-07-09 05:47:26.656963 encrypt256-1.8.4/LICENSE
--rw-r--r--   0        0        0     1884 2023-07-09 05:44:41.563781 encrypt256-1.8.4/README.md
--rw-r--r--   0        0        0       30 2023-04-10 04:00:30.884575 encrypt256-1.8.4/encrypt256.py
--rw-r--r--   0        0        0      618 2023-07-09 06:53:05.135943 encrypt256-1.8.4/pyproject.toml
--rw-r--r--   0        0        0     2261 1970-01-01 00:00:00.000000 encrypt256-1.8.4/PKG-INFO
+-rw-r--r--   0        0        0    11036 2023-07-14 17:01:09.603744 encrypt256-1.8.5/LICENSE
+-rw-r--r--   0        0        0     1911 2023-07-14 14:42:06.504365 encrypt256-1.8.5/README.md
+-rw-r--r--   0        0        0     2926 2023-01-27 23:35:02.000000 encrypt256-1.8.5/encrypt256/Dependent Packages/pycryptodome/LICENSE
+-rw-r--r--   0        0        0       29 2023-06-13 11:40:05.743411 encrypt256-1.8.5/encrypt256/__init__.py
+-rw-r--r--   0        0        0     5194 2023-07-14 17:14:22.805335 encrypt256-1.8.5/encrypt256/_core.py
+-rw-r--r--   0        0        0      599 2023-07-14 17:39:45.817379 encrypt256-1.8.5/pyproject.toml
+-rw-r--r--   0        0        0     2267 1970-01-01 00:00:00.000000 encrypt256-1.8.5/PKG-INFO
```

### Comparing `encrypt256-1.8.4/LICENSE` & `encrypt256-1.8.5/LICENSE`

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

### Comparing `encrypt256-1.8.4/README.md` & `encrypt256-1.8.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -4,31 +4,33 @@
 
 1、底层加密算法为 AES-CBC-256。
 
 2、加密时，会自动创建随机 salt、随机 iv、原始明文的校验值，并把校验值添加到密文中。
 
 3、解密时，会自动根据校验值校验“解密得到的明文”与“原始明文”是否一致。
 
-# 安装
+# 关于作者
 
-```
-pip install encrypt256
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
+pip install encrypt256
+```
 
 # 教程
 
 #### 导入
 
 ```python
 from encrypt256 import Encrypt256
```

### Comparing `encrypt256-1.8.4/pyproject.toml` & `encrypt256-1.8.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "encrypt256"
-version = "1.8.4"
+version = "1.8.5"
 description = "str 型和 bytes 型数据加密器"
-dependencies = ["lccpy >=1.4.7"]
+dependencies = ["pycryptodome"]
 keywords = ["encrypt256", "encrypt", "AES", "pycryptodome", "Crypto"]
 
 readme = "README.md"
 authors = [{name = "lcctoor.com", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
 
 [project.urls]
-HomePage = "https://github.com/lcctoor/lccpy/tree/main/packages/encrypt256#readme"
+HomePage = "https://lcctoor.github.io/lccpy/?package=encrypt256"
```

### Comparing `encrypt256-1.8.4/PKG-INFO` & `encrypt256-1.8.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 Metadata-Version: 2.1
 Name: encrypt256
-Version: 1.8.4
+Version: 1.8.5
 Summary: str 型和 bytes 型数据加密器
 Keywords: encrypt256,encrypt,AES,pycryptodome,Crypto
 Author-email: "lcctoor.com" <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: lccpy >=1.4.7
-Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/encrypt256#readme
+Requires-Dist: pycryptodome
+Project-URL: HomePage, https://lcctoor.github.io/lccpy/?package=encrypt256
 
 # 项目描述
 
 str 型和 bytes 型数据加密器。
 
 1、底层加密算法为 AES-CBC-256。
 
 2、加密时，会自动创建随机 salt、随机 iv、原始明文的校验值，并把校验值添加到密文中。
 
 3、解密时，会自动根据校验值校验“解密得到的明文”与“原始明文”是否一致。
 
-# 安装
+# 关于作者
 
-```
-pip install encrypt256
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
+pip install encrypt256
+```
 
 # 教程
 
 #### 导入
 
 ```python
 from encrypt256 import Encrypt256
```

