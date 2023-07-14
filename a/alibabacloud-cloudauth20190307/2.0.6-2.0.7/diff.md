# Comparing `tmp/alibabacloud_cloudauth20190307-2.0.6.tar.gz` & `tmp/alibabacloud_cloudauth20190307-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cloudauth20190307-2.0.6.tar", last modified: Thu May 18 02:56:41 2023, max compression
+gzip compressed data, was "dist/alibabacloud_cloudauth20190307-2.0.7.tar", last modified: Fri Jul 14 01:44:38 2023, max compression
```

## Comparing `alibabacloud_cloudauth20190307-2.0.6.tar` & `alibabacloud_cloudauth20190307-2.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 02:56:41.000000 alibabacloud_cloudauth20190307-2.0.6/
--rw-r--r--   0 root         (0) root         (0)      756 2023-05-18 02:56:41.000000 alibabacloud_cloudauth20190307-2.0.6/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-18 02:56:41.000000 alibabacloud_cloudauth20190307-2.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-18 02:56:41.000000 alibabacloud_cloudauth20190307-2.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2370 2023-05-18 02:56:41.000000 alibabacloud_cloudauth20190307-2.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1040 2023-05-18 02:56:41.000000 alibabacloud_cloudauth20190307-2.0.6/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1125 2023-05-18 02:56:41.000000 alibabacloud_cloudauth20190307-2.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 02:56:41.000000 alibabacloud_cloudauth20190307-2.0.6/alibabacloud_cloudauth20190307/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-18 02:56:41.000000 alibabacloud_cloudauth20190307-2.0.6/alibabacloud_cloudauth20190307/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77649 2023-05-18 02:56:41.000000 alibabacloud_cloudauth20190307-2.0.6/alibabacloud_cloudauth20190307/client.py
--rw-r--r--   0 root         (0) root         (0)   129400 2023-05-18 02:56:41.000000 alibabacloud_cloudauth20190307-2.0.6/alibabacloud_cloudauth20190307/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 02:56:41.000000 alibabacloud_cloudauth20190307-2.0.6/alibabacloud_cloudauth20190307.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2370 2023-05-18 02:56:41.000000 alibabacloud_cloudauth20190307-2.0.6/alibabacloud_cloudauth20190307.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      468 2023-05-18 02:56:41.000000 alibabacloud_cloudauth20190307-2.0.6/alibabacloud_cloudauth20190307.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 02:56:41.000000 alibabacloud_cloudauth20190307-2.0.6/alibabacloud_cloudauth20190307.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      315 2023-05-18 02:56:41.000000 alibabacloud_cloudauth20190307-2.0.6/alibabacloud_cloudauth20190307.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-05-18 02:56:41.000000 alibabacloud_cloudauth20190307-2.0.6/alibabacloud_cloudauth20190307.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-18 02:56:41.000000 alibabacloud_cloudauth20190307-2.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2837 2023-05-18 02:56:41.000000 alibabacloud_cloudauth20190307-2.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:44:38.000000 alibabacloud_cloudauth20190307-2.0.7/
+-rw-r--r--   0 root         (0) root         (0)      801 2023-07-14 01:44:37.000000 alibabacloud_cloudauth20190307-2.0.7/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-14 01:44:37.000000 alibabacloud_cloudauth20190307-2.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-14 01:44:37.000000 alibabacloud_cloudauth20190307-2.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2370 2023-07-14 01:44:38.000000 alibabacloud_cloudauth20190307-2.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-07-14 01:44:37.000000 alibabacloud_cloudauth20190307-2.0.7/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-07-14 01:44:37.000000 alibabacloud_cloudauth20190307-2.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:44:38.000000 alibabacloud_cloudauth20190307-2.0.7/alibabacloud_cloudauth20190307/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-14 01:44:37.000000 alibabacloud_cloudauth20190307-2.0.7/alibabacloud_cloudauth20190307/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77649 2023-07-14 01:44:37.000000 alibabacloud_cloudauth20190307-2.0.7/alibabacloud_cloudauth20190307/client.py
+-rw-r--r--   0 root         (0) root         (0)   129660 2023-07-14 01:44:37.000000 alibabacloud_cloudauth20190307-2.0.7/alibabacloud_cloudauth20190307/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:44:38.000000 alibabacloud_cloudauth20190307-2.0.7/alibabacloud_cloudauth20190307.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2370 2023-07-14 01:44:37.000000 alibabacloud_cloudauth20190307-2.0.7/alibabacloud_cloudauth20190307.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      468 2023-07-14 01:44:37.000000 alibabacloud_cloudauth20190307-2.0.7/alibabacloud_cloudauth20190307.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 01:44:37.000000 alibabacloud_cloudauth20190307-2.0.7/alibabacloud_cloudauth20190307.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      315 2023-07-14 01:44:37.000000 alibabacloud_cloudauth20190307-2.0.7/alibabacloud_cloudauth20190307.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-07-14 01:44:37.000000 alibabacloud_cloudauth20190307-2.0.7/alibabacloud_cloudauth20190307.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-14 01:44:38.000000 alibabacloud_cloudauth20190307-2.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2837 2023-07-14 01:44:37.000000 alibabacloud_cloudauth20190307-2.0.7/setup.py
```

### Comparing `alibabacloud_cloudauth20190307-2.0.6/ChangeLog.md` & `alibabacloud_cloudauth20190307-2.0.7/ChangeLog.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-05-18 Version: 2.0.6
+- For 2019-03-07.
+
 2022-11-02 Version: 2.0.5
 - For 2019-03-07.
 
 2022-10-17 Version: 2.0.4
 - For 2019-03-07.
 
 2022-06-29 Version: 2.0.3
```

### Comparing `alibabacloud_cloudauth20190307-2.0.6/LICENSE` & `alibabacloud_cloudauth20190307-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth20190307-2.0.6/PKG-INFO` & `alibabacloud_cloudauth20190307-2.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cloudauth20190307
-Version: 2.0.6
+Version: 2.0.7
 Summary: Alibaba Cloud ID Verification (20190307) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloudauth20190307-2.0.6/README-CN.md` & `alibabacloud_cloudauth20190307-2.0.7/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth20190307-2.0.6/README.md` & `alibabacloud_cloudauth20190307-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth20190307-2.0.6/alibabacloud_cloudauth20190307/client.py` & `alibabacloud_cloudauth20190307-2.0.7/alibabacloud_cloudauth20190307/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth20190307-2.0.6/alibabacloud_cloudauth20190307/models.py` & `alibabacloud_cloudauth20190307-2.0.7/alibabacloud_cloudauth20190307/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1384,20 +1384,22 @@
             self.scene_id = m.get('SceneId')
         return self
 
 
 class DescribeFaceVerifyResponseBodyResultObject(TeaModel):
     def __init__(
         self,
+        device_risk: str = None,
         device_token: str = None,
         identity_info: str = None,
         material_info: str = None,
         passed: str = None,
         sub_code: str = None,
     ):
+        self.device_risk = device_risk
         self.device_token = device_token
         self.identity_info = identity_info
         self.material_info = material_info
         self.passed = passed
         self.sub_code = sub_code
 
     def validate(self):
@@ -1405,28 +1407,32 @@
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.device_risk is not None:
+            result['DeviceRisk'] = self.device_risk
         if self.device_token is not None:
             result['DeviceToken'] = self.device_token
         if self.identity_info is not None:
             result['IdentityInfo'] = self.identity_info
         if self.material_info is not None:
             result['MaterialInfo'] = self.material_info
         if self.passed is not None:
             result['Passed'] = self.passed
         if self.sub_code is not None:
             result['SubCode'] = self.sub_code
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('DeviceRisk') is not None:
+            self.device_risk = m.get('DeviceRisk')
         if m.get('DeviceToken') is not None:
             self.device_token = m.get('DeviceToken')
         if m.get('IdentityInfo') is not None:
             self.identity_info = m.get('IdentityInfo')
         if m.get('MaterialInfo') is not None:
             self.material_info = m.get('MaterialInfo')
         if m.get('Passed') is not None:
```

### Comparing `alibabacloud_cloudauth20190307-2.0.6/alibabacloud_cloudauth20190307.egg-info/PKG-INFO` & `alibabacloud_cloudauth20190307-2.0.7/alibabacloud_cloudauth20190307.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cloudauth20190307
-Version: 2.0.6
+Version: 2.0.7
 Summary: Alibaba Cloud ID Verification (20190307) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloudauth20190307-2.0.6/setup.py` & `alibabacloud_cloudauth20190307-2.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cloudauth20190307.
 
-Created on 18/05/2023
+Created on 14/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cloudauth20190307"
 NAME = "alibabacloud_cloudauth20190307" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ID Verification (20190307) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_util>=0.3.9, <1.0.0",
     "alibabacloud_oss_sdk>=0.1.0, <1.0.0",
     "alibabacloud_openplatform20191219>=2.0.0, <3.0.0",
     "alibabacloud_oss_util>=0.0.5, <1.0.0",
     "alibabacloud_tea_fileform>=0.0.3, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
```

