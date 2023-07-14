# Comparing `tmp/ir_digit-1.0.0.tar.gz` & `tmp/ir_digit-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ir_digit-1.0.0.tar", last modified: Thu Jul 13 10:07:35 2023, max compression
+gzip compressed data, was "ir_digit-1.1.1.tar", last modified: Fri Jul 14 06:40:34 2023, max compression
```

## Comparing `ir_digit-1.0.0.tar` & `ir_digit-1.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 10:07:35.328215 ir_digit-1.0.0/
--rw-rw-rw-   0        0        0     1091 2023-03-24 06:34:05.000000 ir_digit-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       32 2023-03-28 12:17:48.000000 ir_digit-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0      506 2023-07-13 10:07:35.325153 ir_digit-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      161 2023-03-27 07:07:49.000000 ir_digit-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 10:07:35.305707 ir_digit-1.0.0/digit/
--rw-rw-rw-   0        0        0      244 2023-06-30 08:41:10.000000 ir_digit-1.0.0/digit/__init__.py
--rw-rw-rw-   0        0        0     3536 2023-07-07 06:05:06.000000 ir_digit-1.0.0/digit/base_data.py
--rw-rw-rw-   0        0        0     1786 2023-06-01 06:11:19.000000 ir_digit-1.0.0/digit/child_base_data.py
--rw-rw-rw-   0        0        0     3206 2023-07-07 06:26:49.000000 ir_digit-1.0.0/digit/core.py
--rw-rw-rw-   0        0        0     7225 2023-07-07 06:11:22.000000 ir_digit-1.0.0/digit/data.py
--rw-rw-rw-   0        0        0     4987 2023-06-01 08:52:58.000000 ir_digit-1.0.0/digit/download.py
--rw-rw-rw-   0        0        0      252 2023-06-01 09:12:08.000000 ir_digit-1.0.0/digit/info.json
--rw-rw-rw-   0        0        0     2155 2023-07-13 09:55:44.000000 ir_digit-1.0.0/digit/info.py
--rw-rw-rw-   0        0        0     4894 2023-06-30 03:59:09.000000 ir_digit-1.0.0/digit/query.py
--rw-rw-rw-   0        0        0     2937 2023-07-13 07:20:47.000000 ir_digit-1.0.0/digit/scripts.py
--rw-rw-rw-   0        0        0     2315 2023-07-13 09:53:29.000000 ir_digit-1.0.0/digit/setting.py
-drwxrwxrwx   0        0        0        0 2023-07-13 10:07:35.322604 ir_digit-1.0.0/ir_digit.egg-info/
--rw-rw-rw-   0        0        0      506 2023-07-13 10:07:34.000000 ir_digit-1.0.0/ir_digit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      419 2023-07-13 10:07:35.000000 ir_digit-1.0.0/ir_digit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 10:07:34.000000 ir_digit-1.0.0/ir_digit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-13 10:07:34.000000 ir_digit-1.0.0/ir_digit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 10:07:34.000000 ir_digit-1.0.0/ir_digit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-13 10:07:34.000000 ir_digit-1.0.0/ir_digit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 10:07:35.329228 ir_digit-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      940 2023-07-13 10:07:18.000000 ir_digit-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 06:40:34.598250 ir_digit-1.1.1/
+-rw-rw-rw-   0        0        0     1091 2023-03-24 06:34:05.000000 ir_digit-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0       32 2023-03-28 12:17:48.000000 ir_digit-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      516 2023-07-14 06:40:34.594251 ir_digit-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      161 2023-03-27 07:07:49.000000 ir_digit-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 06:40:34.574250 ir_digit-1.1.1/digit/
+-rw-rw-rw-   0        0        0      244 2023-06-30 08:41:10.000000 ir_digit-1.1.1/digit/__init__.py
+-rw-rw-rw-   0        0        0     3536 2023-07-07 06:05:06.000000 ir_digit-1.1.1/digit/base_data.py
+-rw-rw-rw-   0        0        0     1786 2023-06-01 06:11:19.000000 ir_digit-1.1.1/digit/child_base_data.py
+-rw-rw-rw-   0        0        0     3206 2023-07-07 06:26:49.000000 ir_digit-1.1.1/digit/core.py
+-rw-rw-rw-   0        0        0     7223 2023-07-13 12:35:06.000000 ir_digit-1.1.1/digit/data.py
+-rw-rw-rw-   0        0        0     4985 2023-07-13 12:22:34.000000 ir_digit-1.1.1/digit/download.py
+-rw-rw-rw-   0        0        0      252 2023-06-01 09:12:08.000000 ir_digit-1.1.1/digit/info.json
+-rw-rw-rw-   0        0        0     2143 2023-07-13 12:28:13.000000 ir_digit-1.1.1/digit/info.py
+-rw-rw-rw-   0        0        0     4899 2023-07-13 12:22:10.000000 ir_digit-1.1.1/digit/query.py
+-rw-rw-rw-   0        0        0     2937 2023-07-13 07:20:47.000000 ir_digit-1.1.1/digit/scripts.py
+-rw-rw-rw-   0        0        0     2315 2023-07-13 09:53:29.000000 ir_digit-1.1.1/digit/setting.py
+drwxrwxrwx   0        0        0        0 2023-07-14 06:40:34.590253 ir_digit-1.1.1/ir_digit.egg-info/
+-rw-rw-rw-   0        0        0      516 2023-07-14 06:40:33.000000 ir_digit-1.1.1/ir_digit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      419 2023-07-14 06:40:34.000000 ir_digit-1.1.1/ir_digit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 06:40:33.000000 ir_digit-1.1.1/ir_digit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-14 06:40:33.000000 ir_digit-1.1.1/ir_digit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       48 2023-07-14 06:40:33.000000 ir_digit-1.1.1/ir_digit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-14 06:40:33.000000 ir_digit-1.1.1/ir_digit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 06:40:34.598250 ir_digit-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      968 2023-07-14 06:40:29.000000 ir_digit-1.1.1/setup.py
```

### Comparing `ir_digit-1.0.0/LICENSE` & `ir_digit-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ir_digit-1.0.0/digit/base_data.py` & `ir_digit-1.1.1/digit/base_data.py`

 * *Files identical despite different names*

### Comparing `ir_digit-1.0.0/digit/child_base_data.py` & `ir_digit-1.1.1/digit/child_base_data.py`

 * *Files identical despite different names*

### Comparing `ir_digit-1.0.0/digit/core.py` & `ir_digit-1.1.1/digit/core.py`

 * *Files identical despite different names*

### Comparing `ir_digit-1.0.0/digit/data.py` & `ir_digit-1.1.1/digit/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
             if config[field] not in category.get(field):
                 errors.append(f"字段{field}的值为{config[field]},不在规定类型的数字代号范围中:{list(category.get(field).keys())}")
 
     return errors
 
 
 
-class Data():
+class Data:
 
     def __init__(self):
         self.info = Information()
         self.qd = QueryDigit()
         self.data_id = ""
         self.DD = "" # 存放加载的数据类
```

### Comparing `ir_digit-1.0.0/digit/download.py` & `ir_digit-1.1.1/digit/download.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 from .query import QueryDigit
 import shutil
 import git
 import stat
 
 
-class Download():
+class Download:
     """
     downlaod 主要就是repo下载
     初始化时检查是否存在对应的文件目录
     不存在则创建
     """
 
     def __init__(self):
```

### Comparing `ir_digit-1.0.0/digit/info.py` & `ir_digit-1.1.1/digit/info.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import sys
 import os
 
 """
-加载info文件， 其中包括api_token和data的字典，如果已经缓存，则data字典中有对应data的data_id和data_name，
+加载info文件， 其中包括api_token和data的字典，如果已经缓存，则data字典中有对应data的data_id，
 """
 
 
 
 class Information:
     def __init__(self):
         if getattr(sys, 'frozen', None): # 确保在不同环境下都能加载正确的文件路径， 无论是打包后的执行文件还是为打包的python脚本
```

### Comparing `ir_digit-1.0.0/digit/query.py` & `ir_digit-1.1.1/digit/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import requests
 from .setting import INTERFACE_PATH,DATA_STORAGE_TYPE, DATA_DATA_TYPE, DATA_LANGUAGE, DATA_TASK_TYPE
 import time
 from .info import Information
 import pprint
 
-class QueryDigit():
+class QueryDigit:
 
     def __init__(self, api_token=Information().get_api_token()):
         self.api_token = api_token
         self.queryset = ""
         self.api_path = INTERFACE_PATH
         self.api_types = ['data', 'card', 'user', 'account', 'websetting','dataid']
 
@@ -100,15 +100,15 @@
             print("\t".join(briefs))
             for resource in self.queryset:
                 print("\t".join([resource[i] for i in briefs]))
 
     """
     已经写好获取两种类型的数据函数，下面是用户请求，选择是否输出details"""
 
-    def get_resources(self, api_type: str, id=None, detail=False):
+    def get_resources(self, api_type: str="data", id=None, detail=False):
         if id:
             if not self._get_single_resource(api_type=api_type, id=id):
                 print(self.errors[0])
                 return self.queryset
         else:
             if not self._get_all_resources(api_type=api_type):
                 print(self.errors[0])
```

### Comparing `ir_digit-1.0.0/digit/scripts.py` & `ir_digit-1.1.1/digit/scripts.py`

 * *Files identical despite different names*

### Comparing `ir_digit-1.0.0/digit/setting.py` & `ir_digit-1.1.1/digit/setting.py`

 * *Files identical despite different names*

### Comparing `ir_digit-1.0.0/setup.py` & `ir_digit-1.1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import setuptools
 
 
 setuptools.setup(
     name="ir_digit",
-    version="1.0.0",
+    version="1.1.1",
     author="FKLiu",
     author_email="fkliu001@outlook.com",
     description="digit package",
     long_description="digit package 与 digit web 配套使用，下载其digit web中的数据资源并在本地运行",
     long_description_content_type="text",
-    url="https://pypi.org/project/ir-digit/",
+    url="https://master--ir-digit-redocs.netlify.app/",
     packages=setuptools.find_packages(),
     include_package_data=True,
     install_requires = [
         "gitpython",
         "numpy",
         "pandas",
         "matplotlib",
-        "seaborn"
+        "seaborn",
+        "jieba"
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
```

