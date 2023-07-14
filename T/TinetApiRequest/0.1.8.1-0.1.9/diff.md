# Comparing `tmp/TinetApiRequest-0.1.8.1.tar.gz` & `tmp/TinetApiRequest-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\TinetApiRequest-0.1.8.1.tar", last modified: Tue Jul 11 08:53:27 2023, max compression
+gzip compressed data, was "dist\TinetApiRequest-0.1.9.tar", last modified: Fri Jul 14 02:57:09 2023, max compression
```

## Comparing `TinetApiRequest-0.1.8.1.tar` & `TinetApiRequest-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 08:53:27.000000 TinetApiRequest-0.1.8.1/
--rw-rw-rw-   0        0        0      274 2023-07-11 08:53:27.000000 TinetApiRequest-0.1.8.1/PKG-INFO
--rw-rw-rw-   0        0        0     3690 2023-06-28 10:50:15.000000 TinetApiRequest-0.1.8.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 08:53:27.000000 TinetApiRequest-0.1.8.1/TinetApiRequest.egg-info/
--rw-rw-rw-   0        0        0      274 2023-07-11 08:53:27.000000 TinetApiRequest-0.1.8.1/TinetApiRequest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-07-11 08:53:27.000000 TinetApiRequest-0.1.8.1/TinetApiRequest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 08:53:27.000000 TinetApiRequest-0.1.8.1/TinetApiRequest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      188 2023-07-11 08:53:27.000000 TinetApiRequest-0.1.8.1/TinetApiRequest.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-11 08:53:27.000000 TinetApiRequest-0.1.8.1/TinetApiRequest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 08:53:27.000000 TinetApiRequest-0.1.8.1/setup.cfg
--rw-rw-rw-   0        0        0      655 2023-07-10 10:07:01.000000 TinetApiRequest-0.1.8.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 08:53:27.000000 TinetApiRequest-0.1.8.1/tinet/
--rw-rw-rw-   0        0        0    20907 2023-07-11 08:07:55.000000 TinetApiRequest-0.1.8.1/tinet/APIRequest.py
--rw-rw-rw-   0        0        0     6911 2023-06-28 10:40:40.000000 TinetApiRequest-0.1.8.1/tinet/ApiConfig.py
--rw-rw-rw-   0        0        0     1082 2023-07-11 08:50:04.000000 TinetApiRequest-0.1.8.1/tinet/LogUtil.py
--rw-rw-rw-   0        0        0     2658 2023-07-11 08:50:04.000000 TinetApiRequest-0.1.8.1/tinet/RequestUtil.py
--rw-rw-rw-   0        0        0     2958 2023-07-11 08:50:04.000000 TinetApiRequest-0.1.8.1/tinet/SignUtil.py
--rw-rw-rw-   0        0        0     7314 2023-06-13 08:06:01.000000 TinetApiRequest-0.1.8.1/tinet/YamlUtil.py
--rw-rw-rw-   0        0        0      164 2023-06-09 08:49:02.000000 TinetApiRequest-0.1.8.1/tinet/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 02:57:09.000000 TinetApiRequest-0.1.9/
+-rw-rw-rw-   0        0        0      272 2023-07-14 02:57:09.000000 TinetApiRequest-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3690 2023-06-28 10:50:15.000000 TinetApiRequest-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 02:57:09.000000 TinetApiRequest-0.1.9/TinetApiRequest.egg-info/
+-rw-rw-rw-   0        0        0      272 2023-07-14 02:57:09.000000 TinetApiRequest-0.1.9/TinetApiRequest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-07-14 02:57:09.000000 TinetApiRequest-0.1.9/TinetApiRequest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 02:57:09.000000 TinetApiRequest-0.1.9/TinetApiRequest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      188 2023-07-14 02:57:09.000000 TinetApiRequest-0.1.9/TinetApiRequest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-14 02:57:09.000000 TinetApiRequest-0.1.9/TinetApiRequest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 02:57:09.000000 TinetApiRequest-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      653 2023-07-14 02:56:37.000000 TinetApiRequest-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 02:57:09.000000 TinetApiRequest-0.1.9/tinet/
+-rw-rw-rw-   0        0        0    21866 2023-07-14 02:51:06.000000 TinetApiRequest-0.1.9/tinet/APIRequest.py
+-rw-rw-rw-   0        0        0     6911 2023-06-28 10:40:40.000000 TinetApiRequest-0.1.9/tinet/ApiConfig.py
+-rw-rw-rw-   0        0        0     1082 2023-07-11 08:50:04.000000 TinetApiRequest-0.1.9/tinet/LogUtil.py
+-rw-rw-rw-   0        0        0     2658 2023-07-11 08:50:04.000000 TinetApiRequest-0.1.9/tinet/RequestUtil.py
+-rw-rw-rw-   0        0        0     2958 2023-07-11 08:50:04.000000 TinetApiRequest-0.1.9/tinet/SignUtil.py
+-rw-rw-rw-   0        0        0     7314 2023-06-13 08:06:01.000000 TinetApiRequest-0.1.9/tinet/YamlUtil.py
+-rw-rw-rw-   0        0        0      164 2023-06-09 08:49:02.000000 TinetApiRequest-0.1.9/tinet/__init__.py
```

### Comparing `TinetApiRequest-0.1.8.1/README.md` & `TinetApiRequest-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-0.1.8.1/setup.py` & `TinetApiRequest-0.1.9/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 BASE_DIR = Path(__file__).parent
 with open(Path(BASE_DIR, "requirements.txt"), "r") as file:
     required_packages = [ln.strip() for ln in file.readlines()]
 
 # Define our package
 setup(
     name="TinetApiRequest",
-    version="0.1.8.1",
+    version="0.1.9",
     description="天润接口测试库",
     author="天润-测试",
     author_email="zhupeng@ti-net.com.cn",
     url="https://www.ti-net.com.cn/",
     python_requires=">=3.7",
     packages=find_namespace_packages(),
     install_requires=[required_packages],
```

### Comparing `TinetApiRequest-0.1.8.1/tinet/APIRequest.py` & `TinetApiRequest-0.1.9/tinet/APIRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """
 接口测试核心类
 """
 import json
 import time
+from urllib.parse import urlparse
+
 import pytest
 import allure
 import jsonpath
 from requests_toolbelt import MultipartEncoder
 from tinet.LogUtil import log
 from tinet.RequestUtil import HttpClient
 from tinet.SignUtil import SignUtil
@@ -70,32 +72,38 @@
                     raise Exception(f"commonPath路径未配置,请检查配置文件")
                 # 执行当前用例 格式化为json 间隔4个空格
                 log.info(f"执行当前用例name: {testcase.get('name')}, id: {testcase.get('id')}")
                 allure.attach(f"{json.dumps(testcase, indent=4, ensure_ascii=False)}", name=f"执行当前用例name: {testcase.get('name')}, id: {testcase.get('id')}",
                               attachment_type=allure.attachment_type.TEXT)
                 # 1. 先看看参数中是否有需要替换的参数
                 repParameter = self.replaceParameterAttr(dataSaveBean, testcase.get('parameter'))
+                repApi = self.replaceParameterAttr(dataSaveBean, testcase.get('api'))
                 # 2. 判断鉴权方式 authType 返回请求地址
-                requestParameter, requestUrl = self.authType(testcase.get('authType'), testcase.get('api'), testcase.get('method'), repParameter)
+                requestParameter, requestUrl = self.authType(testcase.get('authType'), repApi, testcase.get('method'), repParameter)
                 # 3. 判断请求 requestType
-                dataRequestParameter, jsonRequestParameter, requestType = self.requestType(testcase.get('requestType'), requestParameter)
+                dataRequestParameter, jsonRequestParameter, paramsData, requestType = self.requestType(testcase.get('requestType'), requestParameter)
                 # 4. 开始请求
                 log.info(f"开始请求地址: {requestUrl} ")
                 allure.attach(f"{requestUrl}", name=f"开始请求地址", attachment_type=allure.attachment_type.TEXT)
                 log.info(f"开始请求方式: {testcase.get('method')}")
                 allure.attach(f"{testcase.get('method')}", name=f"开始请求方式", attachment_type=allure.attachment_type.TEXT)
-                log.info(f"开始请求参数dataRequestParameter: {dataRequestParameter}")
-                allure.attach(f"{dataRequestParameter}", name=f"开始请求参数dataRequestParameter", attachment_type=allure.attachment_type.TEXT)
-                log.info(f"开始请求参数jsonRequestParameter: {jsonRequestParameter}")
-                allure.attach(f"{jsonRequestParameter}", name=f"开始请求参数jsonRequestParameter", attachment_type=allure.attachment_type.TEXT)
+                if dataRequestParameter is not None:
+                    log.info(f"开始请求参数dataRequestParameter: {dataRequestParameter}")
+                    allure.attach(f"{dataRequestParameter}", name=f"开始请求参数dataRequestParameter", attachment_type=allure.attachment_type.TEXT)
+                if jsonRequestParameter is not None:
+                    log.info(f"开始请求参数jsonRequestParameter: {jsonRequestParameter}")
+                    allure.attach(f"{jsonRequestParameter}", name=f"开始请求参数jsonRequestParameter", attachment_type=allure.attachment_type.TEXT)
+                if paramsData is not None:
+                    log.info(f"开始请求参数paramsData: {paramsData}")
+                    allure.attach(f"{paramsData}", name=f"开始请求参数paramsDatar", attachment_type=allure.attachment_type.TEXT)
                 # form-data请求 需要处理一下header
                 headers = testcase.get('headers')
                 if dataRequestParameter is not None and requestType.lower() == 'form-data':
                     headers['Content-Type'] = dataRequestParameter.content_type
-                response = request.request(method=testcase.get('method'), url=requestUrl, data=dataRequestParameter, json=jsonRequestParameter, headers=headers)
+                response = request.request(method=testcase.get('method'), url=requestUrl, data=dataRequestParameter, json=jsonRequestParameter, params=paramsData, headers=headers)
                 try:  # 当返回不是 json 返回text
                     log.info(f"当前用例response: {json.dumps(response.json(), indent=4, ensure_ascii=False)}")
                     allure.attach(f"{json.dumps(response.json(), indent=4, ensure_ascii=False)}", name=f"当前用例response",
                                   attachment_type=allure.attachment_type.TEXT)
                 except:
                     log.info(f"当前用例response: {json.dumps(response.text, indent=4, ensure_ascii=False)}")
                     allure.attach(f"{json.dumps(response.text, indent=4, ensure_ascii=False)}", name=f"当前用例response",
@@ -229,14 +237,15 @@
         return repParameter
 
     # 判断请求方式 requestType
     def requestType(self, requestType, data):
         # 判断是否为空
         jsonRequestParameter = None
         dataRequestParameter = None
+        paramsData = None
         if requestType is None:
             log.info(f"请求方式为空: {requestType} ,默认走json请求")
             allure.attach(f"{requestType}", name=f"请求方式为空,默认走json请求", attachment_type=allure.attachment_type.TEXT)
             jsonRequestParameter = data
         elif requestType.lower() == "json":
             # 进行json请求
             log.info(f"请求方式为JSON: {requestType}")
@@ -245,30 +254,31 @@
         elif requestType.lower() == "form-data":
             # 进行form请求
             log.info(f"请求方式为FORM: {requestType}")
             allure.attach(f"{requestType}", name=f"请求方式为FORM", attachment_type=allure.attachment_type.TEXT)
             dataRequestParameter = MultipartEncoder(fields=data)
         elif requestType == "PARAMS":
             # 进行PARAMS请求
-            pass
+            log.info(f"请求方式为PARAMS: {requestType}")
+            allure.attach(f"{requestType}", name=f"请求方式为PARAMS", attachment_type=allure.attachment_type.TEXT)
+            paramsData = data
         elif requestType == "DATA":
             # 进行DATA请求
             log.info(f"请求方式为DATA: {requestType}")
             allure.attach(f"{requestType}", name=f"请求方式为DATA", attachment_type=allure.attachment_type.TEXT)
             dataRequestParameter = data
-            pass
         else:
             log.error("请求方式不支持")
             allure.attach(f"请求方式不支持", name=f"请求方式不支持", attachment_type=allure.attachment_type.TEXT)
-        return dataRequestParameter, jsonRequestParameter, requestType
+        return dataRequestParameter, jsonRequestParameter, paramsData, requestType
 
     # 判断鉴权方式 authType
     def authType(self, authType, url, method, parameter):
         # 判断baseurl 是否为None
-        if self.baseUrl is None:
+        if self.baseUrl is None or self.isValidUrl(url):
             requestUrl = url
         else:
             requestUrl = self.baseUrl + url
         requestParameter = None
         if authType == "SIGN":
             # 进行签名
             requestUrl = SignUtil.signature(apiUrlPath=requestUrl, method=method, params=parameter, access_key_id=self.AccessKeyId, access_key_secret=self.AccessKeySecret)
@@ -329,7 +339,14 @@
         :param type:
         :return:
         """
         if type == 'stop':
             assert ass, tips
         elif type == 'continue':
             pytest.assume(ass, tips)
+
+    def isValidUrl(self, url):
+        try:
+            result = urlparse(url)
+            return all([result.scheme, result.netloc])
+        except ValueError:
+            return False
```

### Comparing `TinetApiRequest-0.1.8.1/tinet/ApiConfig.py` & `TinetApiRequest-0.1.9/tinet/ApiConfig.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-0.1.8.1/tinet/LogUtil.py` & `TinetApiRequest-0.1.9/tinet/LogUtil.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-0.1.8.1/tinet/RequestUtil.py` & `TinetApiRequest-0.1.9/tinet/RequestUtil.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-0.1.8.1/tinet/SignUtil.py` & `TinetApiRequest-0.1.9/tinet/SignUtil.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-0.1.8.1/tinet/YamlUtil.py` & `TinetApiRequest-0.1.9/tinet/YamlUtil.py`

 * *Files identical despite different names*

