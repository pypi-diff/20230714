# Comparing `tmp/longmao-open-sdk-python-0.1.5.tar.gz` & `tmp/longmao-open-sdk-python-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longmao-open-sdk-python-0.1.5.tar", last modified: Tue Nov 15 11:51:56 2022, max compression
+gzip compressed data, was "longmao-open-sdk-python-0.1.6.tar", last modified: Fri Jul 14 11:49:02 2023, max compression
```

## Comparing `longmao-open-sdk-python-0.1.5.tar` & `longmao-open-sdk-python-0.1.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 nayuan     (501) staff       (20)        0 2022-11-15 11:51:56.277496 longmao-open-sdk-python-0.1.5/
--rw-r--r--   0 nayuan     (501) staff       (20)    11357 2022-09-03 11:18:36.000000 longmao-open-sdk-python-0.1.5/LICENSE
--rw-r--r--   0 nayuan     (501) staff       (20)     2644 2022-11-15 11:51:56.277364 longmao-open-sdk-python-0.1.5/PKG-INFO
--rw-r--r--   0 nayuan     (501) staff       (20)     1911 2022-09-03 11:18:36.000000 longmao-open-sdk-python-0.1.5/README.rst
-drwxr-xr-x   0 nayuan     (501) staff       (20)        0 2022-11-15 11:51:56.272944 longmao-open-sdk-python-0.1.5/longmao/
--rw-r--r--   0 nayuan     (501) staff       (20)      125 2022-11-15 11:51:54.000000 longmao-open-sdk-python-0.1.5/longmao/__init__.py
-drwxr-xr-x   0 nayuan     (501) staff       (20)        0 2022-11-15 11:51:56.273269 longmao-open-sdk-python-0.1.5/longmao/api/
--rw-r--r--   0 nayuan     (501) staff       (20)      963 2022-09-03 11:18:36.000000 longmao-open-sdk-python-0.1.5/longmao/api/Api.py
--rw-r--r--   0 nayuan     (501) staff       (20)       69 2022-09-03 11:18:36.000000 longmao-open-sdk-python-0.1.5/longmao/api/__init__.py
-drwxr-xr-x   0 nayuan     (501) staff       (20)        0 2022-11-15 11:51:56.273961 longmao-open-sdk-python-0.1.5/longmao/api/tags/
--rw-r--r--   0 nayuan     (501) staff       (20)     2218 2022-11-15 11:38:25.000000 longmao-open-sdk-python-0.1.5/longmao/api/tags/ApiTagsTencentPush.py
--rw-r--r--   0 nayuan     (501) staff       (20)     1036 2022-09-04 13:11:51.000000 longmao-open-sdk-python-0.1.5/longmao/api/tags/ApiTagsUploadCsv.py
--rw-r--r--   0 nayuan     (501) staff       (20)       69 2022-09-03 11:18:36.000000 longmao-open-sdk-python-0.1.5/longmao/api/tags/__init__.py
-drwxr-xr-x   0 nayuan     (501) staff       (20)        0 2022-11-15 11:51:56.274662 longmao-open-sdk-python-0.1.5/longmao/core/
--rw-r--r--   0 nayuan     (501) staff       (20)     1182 2022-09-03 11:18:36.000000 longmao-open-sdk-python-0.1.5/longmao/core/DefaultLongMaoClient.py
--rw-r--r--   0 nayuan     (501) staff       (20)     1779 2022-09-04 13:34:39.000000 longmao-open-sdk-python-0.1.5/longmao/core/LongMaoClientConfig.py
--rw-r--r--   0 nayuan     (501) staff       (20)       69 2022-09-03 11:18:36.000000 longmao-open-sdk-python-0.1.5/longmao/core/__init__.py
-drwxr-xr-x   0 nayuan     (501) staff       (20)        0 2022-11-15 11:51:56.275170 longmao-open-sdk-python-0.1.5/longmao/core/exception/
--rw-r--r--   0 nayuan     (501) staff       (20)      505 2022-09-03 11:18:36.000000 longmao-open-sdk-python-0.1.5/longmao/core/exception/Exception.py
--rw-r--r--   0 nayuan     (501) staff       (20)       69 2022-09-03 11:18:36.000000 longmao-open-sdk-python-0.1.5/longmao/core/exception/__init__.py
-drwxr-xr-x   0 nayuan     (501) staff       (20)        0 2022-11-15 11:51:56.275705 longmao-open-sdk-python-0.1.5/longmao/core/http/
--rw-r--r--   0 nayuan     (501) staff       (20)      673 2022-09-03 11:18:36.000000 longmao-open-sdk-python-0.1.5/longmao/core/http/FileItem.py
--rw-r--r--   0 nayuan     (501) staff       (20)     7109 2022-09-03 11:18:36.000000 longmao-open-sdk-python-0.1.5/longmao/core/http/HttpRequest.py
--rw-r--r--   0 nayuan     (501) staff       (20)       69 2022-09-03 11:18:36.000000 longmao-open-sdk-python-0.1.5/longmao/core/http/__init__.py
-drwxr-xr-x   0 nayuan     (501) staff       (20)        0 2022-11-15 11:51:56.276488 longmao-open-sdk-python-0.1.5/longmao/core/utils/
--rw-r--r--   0 nayuan     (501) staff       (20)     1969 2022-09-03 11:18:36.000000 longmao-open-sdk-python-0.1.5/longmao/core/utils/CommonUtils.py
--rw-r--r--   0 nayuan     (501) staff       (20)      253 2022-09-03 11:18:36.000000 longmao-open-sdk-python-0.1.5/longmao/core/utils/Constants.py
--rw-r--r--   0 nayuan     (501) staff       (20)      436 2022-09-03 11:18:36.000000 longmao-open-sdk-python-0.1.5/longmao/core/utils/SignatureUtils.py
--rw-r--r--   0 nayuan     (501) staff       (20)      299 2022-09-03 11:18:36.000000 longmao-open-sdk-python-0.1.5/longmao/core/utils/StringUtils.py
--rw-r--r--   0 nayuan     (501) staff       (20)       69 2022-09-03 11:18:36.000000 longmao-open-sdk-python-0.1.5/longmao/core/utils/__init__.py
-drwxr-xr-x   0 nayuan     (501) staff       (20)        0 2022-11-15 11:51:56.277189 longmao-open-sdk-python-0.1.5/longmao_open_sdk_python.egg-info/
--rw-r--r--   0 nayuan     (501) staff       (20)     2644 2022-11-15 11:51:56.000000 longmao-open-sdk-python-0.1.5/longmao_open_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 nayuan     (501) staff       (20)      859 2022-11-15 11:51:56.000000 longmao-open-sdk-python-0.1.5/longmao_open_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 nayuan     (501) staff       (20)        1 2022-11-15 11:51:56.000000 longmao-open-sdk-python-0.1.5/longmao_open_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 nayuan     (501) staff       (20)        9 2022-11-15 11:51:56.000000 longmao-open-sdk-python-0.1.5/longmao_open_sdk_python.egg-info/requires.txt
--rw-r--r--   0 nayuan     (501) staff       (20)        8 2022-11-15 11:51:56.000000 longmao-open-sdk-python-0.1.5/longmao_open_sdk_python.egg-info/top_level.txt
--rw-r--r--   0 nayuan     (501) staff       (20)       38 2022-11-15 11:51:56.277546 longmao-open-sdk-python-0.1.5/setup.cfg
--rw-r--r--   0 nayuan     (501) staff       (20)     2243 2022-09-03 11:18:36.000000 longmao-open-sdk-python-0.1.5/setup.py
+drwxr-xr-x   0 nayuan     (501) staff       (20)        0 2023-07-14 11:49:02.211923 longmao-open-sdk-python-0.1.6/
+-rw-r--r--   0 nayuan     (501) staff       (20)    11357 2022-09-03 11:18:36.000000 longmao-open-sdk-python-0.1.6/LICENSE
+-rw-r--r--   0 nayuan     (501) staff       (20)     2654 2023-07-14 11:49:02.211793 longmao-open-sdk-python-0.1.6/PKG-INFO
+-rw-r--r--   0 nayuan     (501) staff       (20)     1911 2022-09-03 11:18:36.000000 longmao-open-sdk-python-0.1.6/README.rst
+drwxr-xr-x   0 nayuan     (501) staff       (20)        0 2023-07-14 11:49:02.207675 longmao-open-sdk-python-0.1.6/longmao/
+-rw-r--r--   0 nayuan     (501) staff       (20)      125 2023-07-13 09:03:25.000000 longmao-open-sdk-python-0.1.6/longmao/__init__.py
+drwxr-xr-x   0 nayuan     (501) staff       (20)        0 2023-07-14 11:49:02.208090 longmao-open-sdk-python-0.1.6/longmao/api/
+-rw-r--r--   0 nayuan     (501) staff       (20)      963 2022-09-03 11:18:36.000000 longmao-open-sdk-python-0.1.6/longmao/api/Api.py
+-rw-r--r--   0 nayuan     (501) staff       (20)       69 2022-09-03 11:18:36.000000 longmao-open-sdk-python-0.1.6/longmao/api/__init__.py
+drwxr-xr-x   0 nayuan     (501) staff       (20)        0 2023-07-14 11:49:02.208779 longmao-open-sdk-python-0.1.6/longmao/api/tags/
+-rw-r--r--   0 nayuan     (501) staff       (20)      738 2023-07-14 11:35:22.000000 longmao-open-sdk-python-0.1.6/longmao/api/tags/ApiTagsDeleteCsv.py
+-rw-r--r--   0 nayuan     (501) staff       (20)     1036 2022-09-04 13:11:51.000000 longmao-open-sdk-python-0.1.6/longmao/api/tags/ApiTagsUploadCsv.py
+-rw-r--r--   0 nayuan     (501) staff       (20)       69 2022-09-03 11:18:36.000000 longmao-open-sdk-python-0.1.6/longmao/api/tags/__init__.py
+drwxr-xr-x   0 nayuan     (501) staff       (20)        0 2023-07-14 11:49:02.209521 longmao-open-sdk-python-0.1.6/longmao/core/
+-rw-r--r--   0 nayuan     (501) staff       (20)     1182 2023-07-13 09:03:25.000000 longmao-open-sdk-python-0.1.6/longmao/core/DefaultLongMaoClient.py
+-rw-r--r--   0 nayuan     (501) staff       (20)     1778 2023-07-13 09:03:25.000000 longmao-open-sdk-python-0.1.6/longmao/core/LongMaoClientConfig.py
+-rw-r--r--   0 nayuan     (501) staff       (20)       69 2022-09-03 11:18:36.000000 longmao-open-sdk-python-0.1.6/longmao/core/__init__.py
+drwxr-xr-x   0 nayuan     (501) staff       (20)        0 2023-07-14 11:49:02.209793 longmao-open-sdk-python-0.1.6/longmao/core/exception/
+-rw-r--r--   0 nayuan     (501) staff       (20)      505 2022-09-03 11:18:36.000000 longmao-open-sdk-python-0.1.6/longmao/core/exception/Exception.py
+-rw-r--r--   0 nayuan     (501) staff       (20)       69 2022-09-03 11:18:36.000000 longmao-open-sdk-python-0.1.6/longmao/core/exception/__init__.py
+drwxr-xr-x   0 nayuan     (501) staff       (20)        0 2023-07-14 11:49:02.210260 longmao-open-sdk-python-0.1.6/longmao/core/http/
+-rw-r--r--   0 nayuan     (501) staff       (20)      673 2022-09-03 11:18:36.000000 longmao-open-sdk-python-0.1.6/longmao/core/http/FileItem.py
+-rw-r--r--   0 nayuan     (501) staff       (20)     7109 2022-09-03 11:18:36.000000 longmao-open-sdk-python-0.1.6/longmao/core/http/HttpRequest.py
+-rw-r--r--   0 nayuan     (501) staff       (20)       69 2022-09-03 11:18:36.000000 longmao-open-sdk-python-0.1.6/longmao/core/http/__init__.py
+drwxr-xr-x   0 nayuan     (501) staff       (20)        0 2023-07-14 11:49:02.211000 longmao-open-sdk-python-0.1.6/longmao/core/utils/
+-rw-r--r--   0 nayuan     (501) staff       (20)     1969 2022-09-03 11:18:36.000000 longmao-open-sdk-python-0.1.6/longmao/core/utils/CommonUtils.py
+-rw-r--r--   0 nayuan     (501) staff       (20)      253 2022-09-03 11:18:36.000000 longmao-open-sdk-python-0.1.6/longmao/core/utils/Constants.py
+-rw-r--r--   0 nayuan     (501) staff       (20)      436 2022-09-03 11:18:36.000000 longmao-open-sdk-python-0.1.6/longmao/core/utils/SignatureUtils.py
+-rw-r--r--   0 nayuan     (501) staff       (20)      299 2022-09-03 11:18:36.000000 longmao-open-sdk-python-0.1.6/longmao/core/utils/StringUtils.py
+-rw-r--r--   0 nayuan     (501) staff       (20)       69 2022-09-03 11:18:36.000000 longmao-open-sdk-python-0.1.6/longmao/core/utils/__init__.py
+drwxr-xr-x   0 nayuan     (501) staff       (20)        0 2023-07-14 11:49:02.211613 longmao-open-sdk-python-0.1.6/longmao_open_sdk_python.egg-info/
+-rw-r--r--   0 nayuan     (501) staff       (20)     2654 2023-07-14 11:49:02.000000 longmao-open-sdk-python-0.1.6/longmao_open_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 nayuan     (501) staff       (20)      857 2023-07-14 11:49:02.000000 longmao-open-sdk-python-0.1.6/longmao_open_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 nayuan     (501) staff       (20)        1 2023-07-14 11:49:02.000000 longmao-open-sdk-python-0.1.6/longmao_open_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 nayuan     (501) staff       (20)        9 2023-07-14 11:49:02.000000 longmao-open-sdk-python-0.1.6/longmao_open_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 nayuan     (501) staff       (20)        8 2023-07-14 11:49:02.000000 longmao-open-sdk-python-0.1.6/longmao_open_sdk_python.egg-info/top_level.txt
+-rw-r--r--   0 nayuan     (501) staff       (20)       38 2023-07-14 11:49:02.211954 longmao-open-sdk-python-0.1.6/setup.cfg
+-rw-r--r--   0 nayuan     (501) staff       (20)     2253 2023-07-13 09:02:12.000000 longmao-open-sdk-python-0.1.6/setup.py
```

### Comparing `longmao-open-sdk-python-0.1.5/LICENSE` & `longmao-open-sdk-python-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `longmao-open-sdk-python-0.1.5/PKG-INFO` & `longmao-open-sdk-python-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: longmao-open-sdk-python
-Version: 0.1.5
+Version: 0.1.6
 Summary: The official LongMao SDK for Python.
 Home-page: https://github.com/nayuan/longmao-open-sdk-python
 Author: nayuan
-Author-email: nayuan@vip.qq.com
+Author-email: haojunsheng@longmaosoft.com
 License: Apache
 Keywords: longmao,open,sdk
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.6
```

### Comparing `longmao-open-sdk-python-0.1.5/README.rst` & `longmao-open-sdk-python-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `longmao-open-sdk-python-0.1.5/longmao/api/Api.py` & `longmao-open-sdk-python-0.1.6/longmao/api/Api.py`

 * *Files identical despite different names*

### Comparing `longmao-open-sdk-python-0.1.5/longmao/api/tags/ApiTagsUploadCsv.py` & `longmao-open-sdk-python-0.1.6/longmao/api/tags/ApiTagsUploadCsv.py`

 * *Files identical despite different names*

### Comparing `longmao-open-sdk-python-0.1.5/longmao/core/DefaultLongMaoClient.py` & `longmao-open-sdk-python-0.1.6/longmao/core/DefaultLongMaoClient.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     """
     执行接口请求
     """
     def execute(self, api):
         headers = {
             "Cache-Control": "no-cache",
             "Connection": "Keep-Alive",
-            "User-Agent": "longmao-open-sdk-python/0.1.0 " + platform.platform() + ' ' + platform.python_version()
+            "User-Agent": "longmao-open-sdk-python/0.1.6 " + platform.platform() + ' ' + platform.python_version()
         }
         url = self._config.server_url + '?' + api.get_url_params(self._config)
 
         file = api.get_file()
         if not file:
             headers['Content-type'] = 'application/json;charset=' + self._config.charset
             result = requests.post(url, headers=headers, data=json.dumps(api.get_params()))
```

### Comparing `longmao-open-sdk-python-0.1.5/longmao/core/LongMaoClientConfig.py` & `longmao-open-sdk-python-0.1.6/longmao/core/LongMaoClientConfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         # 龙猫数据开放平台网关地址
         self._server_url = "https://api.service.longmaosoft.com/gateway.do"
         # 请求字符集，默认utf-8
         self._charset = 'utf-8'
         # 请求响应报文格式
         self._format = 'JSON'
         # 请求读取超时，单位秒，默认15s
-        self._timeout = 15
+        self._timeout = 5
 
     @property
     def domain(self):
         return self._server_url
 
     @domain.setter
     def domain(self, value):
```

### Comparing `longmao-open-sdk-python-0.1.5/longmao/core/http/FileItem.py` & `longmao-open-sdk-python-0.1.6/longmao/core/http/FileItem.py`

 * *Files identical despite different names*

### Comparing `longmao-open-sdk-python-0.1.5/longmao/core/http/HttpRequest.py` & `longmao-open-sdk-python-0.1.6/longmao/core/http/HttpRequest.py`

 * *Files identical despite different names*

### Comparing `longmao-open-sdk-python-0.1.5/longmao/core/utils/CommonUtils.py` & `longmao-open-sdk-python-0.1.6/longmao/core/utils/CommonUtils.py`

 * *Files identical despite different names*

### Comparing `longmao-open-sdk-python-0.1.5/longmao_open_sdk_python.egg-info/PKG-INFO` & `longmao-open-sdk-python-0.1.6/longmao_open_sdk_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: longmao-open-sdk-python
-Version: 0.1.5
+Version: 0.1.6
 Summary: The official LongMao SDK for Python.
 Home-page: https://github.com/nayuan/longmao-open-sdk-python
 Author: nayuan
-Author-email: nayuan@vip.qq.com
+Author-email: haojunsheng@longmaosoft.com
 License: Apache
 Keywords: longmao,open,sdk
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.6
```

### Comparing `longmao-open-sdk-python-0.1.5/longmao_open_sdk_python.egg-info/SOURCES.txt` & `longmao-open-sdk-python-0.1.6/longmao_open_sdk_python.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 LICENSE
 README.rst
 setup.py
 longmao/__init__.py
 longmao/api/Api.py
 longmao/api/__init__.py
-longmao/api/tags/ApiTagsTencentPush.py
+longmao/api/tags/ApiTagsDeleteCsv.py
 longmao/api/tags/ApiTagsUploadCsv.py
 longmao/api/tags/__init__.py
 longmao/core/DefaultLongMaoClient.py
 longmao/core/LongMaoClientConfig.py
 longmao/core/__init__.py
 longmao/core/exception/Exception.py
 longmao/core/exception/__init__.py
```

### Comparing `longmao-open-sdk-python-0.1.5/setup.py` & `longmao-open-sdk-python-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 Created on 2020-01-01
 @author: nayuan
 """
 PACKAGE = "longmao"
 NAME = "longmao-open-sdk-python"
 DESCRIPTION = "The official LongMao SDK for Python."
 AUTHOR = "nayuan"
-AUTHOR_EMAIL = "nayuan@vip.qq.com"
+AUTHOR_EMAIL = "haojunsheng@longmaosoft.com"
 URL = "https://github.com/nayuan/longmao-open-sdk-python"
 
 TOPDIR = os.path.dirname(__file__) or "."
 VERSION = __import__(PACKAGE).__version__
 
 desc_file = codecs.open("README.rst", 'r', 'utf-8')
 try:
```

