# Comparing `tmp/tencentcloud-sdk-python-apigateway-3.0.934.tar.gz` & `tmp/tencentcloud-sdk-python-apigateway-3.0.935.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-apigateway-3.0.934.tar", last modified: Thu Jul 13 00:14:53 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-apigateway-3.0.935.tar", last modified: Fri Jul 14 00:16:30 2023, max compression
```

## Comparing `tencentcloud-sdk-python-apigateway-3.0.934.tar` & `tencentcloud-sdk-python-apigateway-3.0.935.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:14:53.000000 tencentcloud-sdk-python-apigateway-3.0.934/
--rw-r--r--   0 root         (0) root         (0)     1020 2023-07-13 00:14:53.000000 tencentcloud-sdk-python-apigateway-3.0.934/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:14:53.000000 tencentcloud-sdk-python-apigateway-3.0.934/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:14:53.000000 tencentcloud-sdk-python-apigateway-3.0.934/tencentcloud/apigateway/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:14:53.000000 tencentcloud-sdk-python-apigateway-3.0.934/tencentcloud/apigateway/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:14:53.000000 tencentcloud-sdk-python-apigateway-3.0.934/tencentcloud/apigateway/v20180808/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:14:53.000000 tencentcloud-sdk-python-apigateway-3.0.934/tencentcloud/apigateway/v20180808/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21433 2023-07-13 00:14:53.000000 tencentcloud-sdk-python-apigateway-3.0.934/tencentcloud/apigateway/v20180808/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   648251 2023-07-13 00:14:53.000000 tencentcloud-sdk-python-apigateway-3.0.934/tencentcloud/apigateway/v20180808/models.py
--rw-r--r--   0 root         (0) root         (0)    96004 2023-07-13 00:14:53.000000 tencentcloud-sdk-python-apigateway-3.0.934/tencentcloud/apigateway/v20180808/apigateway_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-13 00:14:53.000000 tencentcloud-sdk-python-apigateway-3.0.934/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-13 00:14:53.000000 tencentcloud-sdk-python-apigateway-3.0.934/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1694 2023-07-13 00:14:53.000000 tencentcloud-sdk-python-apigateway-3.0.934/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:14:53.000000 tencentcloud-sdk-python-apigateway-3.0.934/tencentcloud_sdk_python_apigateway.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 00:14:53.000000 tencentcloud-sdk-python-apigateway-3.0.934/tencentcloud_sdk_python_apigateway.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      515 2023-07-13 00:14:53.000000 tencentcloud-sdk-python-apigateway-3.0.934/tencentcloud_sdk_python_apigateway.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-07-13 00:14:53.000000 tencentcloud-sdk-python-apigateway-3.0.934/tencentcloud_sdk_python_apigateway.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-13 00:14:53.000000 tencentcloud-sdk-python-apigateway-3.0.934/tencentcloud_sdk_python_apigateway.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      758 2023-07-13 00:14:53.000000 tencentcloud-sdk-python-apigateway-3.0.934/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:16:30.000000 tencentcloud-sdk-python-apigateway-3.0.935/
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-07-14 00:16:30.000000 tencentcloud-sdk-python-apigateway-3.0.935/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:16:30.000000 tencentcloud-sdk-python-apigateway-3.0.935/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:16:30.000000 tencentcloud-sdk-python-apigateway-3.0.935/tencentcloud/apigateway/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:16:30.000000 tencentcloud-sdk-python-apigateway-3.0.935/tencentcloud/apigateway/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:16:30.000000 tencentcloud-sdk-python-apigateway-3.0.935/tencentcloud/apigateway/v20180808/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:16:30.000000 tencentcloud-sdk-python-apigateway-3.0.935/tencentcloud/apigateway/v20180808/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21433 2023-07-14 00:16:30.000000 tencentcloud-sdk-python-apigateway-3.0.935/tencentcloud/apigateway/v20180808/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   648251 2023-07-14 00:16:30.000000 tencentcloud-sdk-python-apigateway-3.0.935/tencentcloud/apigateway/v20180808/models.py
+-rw-r--r--   0 root         (0) root         (0)    96105 2023-07-14 00:16:30.000000 tencentcloud-sdk-python-apigateway-3.0.935/tencentcloud/apigateway/v20180808/apigateway_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-14 00:16:30.000000 tencentcloud-sdk-python-apigateway-3.0.935/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-14 00:16:30.000000 tencentcloud-sdk-python-apigateway-3.0.935/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-07-14 00:16:30.000000 tencentcloud-sdk-python-apigateway-3.0.935/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:16:30.000000 tencentcloud-sdk-python-apigateway-3.0.935/tencentcloud_sdk_python_apigateway.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 00:16:30.000000 tencentcloud-sdk-python-apigateway-3.0.935/tencentcloud_sdk_python_apigateway.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      515 2023-07-14 00:16:30.000000 tencentcloud-sdk-python-apigateway-3.0.935/tencentcloud_sdk_python_apigateway.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-07-14 00:16:30.000000 tencentcloud-sdk-python-apigateway-3.0.935/tencentcloud_sdk_python_apigateway.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-14 00:16:30.000000 tencentcloud-sdk-python-apigateway-3.0.935/tencentcloud_sdk_python_apigateway.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      758 2023-07-14 00:16:30.000000 tencentcloud-sdk-python-apigateway-3.0.935/README.rst
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.934/setup.py` & `tencentcloud-sdk-python-apigateway-3.0.935/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apigateway-3.0.934/tencentcloud/apigateway/v20180808/errorcodes.py` & `tencentcloud-sdk-python-apigateway-3.0.935/tencentcloud/apigateway/v20180808/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apigateway-3.0.934/tencentcloud/apigateway/v20180808/models.py` & `tencentcloud-sdk-python-apigateway-3.0.935/tencentcloud/apigateway/v20180808/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -733,15 +733,15 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class ApiEnvironmentStrategyStataus(AbstractModel):
+class ApiEnvironmentStrategyStatus(AbstractModel):
     """API绑定策略列表
 
     """
 
     def __init__(self):
         r"""
         :param _TotalCount: API绑定的限流策略数量。
@@ -7789,15 +7789,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param _Result: api绑定策略详情
 注意：此字段可能返回 null，表示取不到有效值。
-        :type Result: :class:`tencentcloud.apigateway.v20180808.models.ApiEnvironmentStrategyStataus`
+        :type Result: :class:`tencentcloud.apigateway.v20180808.models.ApiEnvironmentStrategyStatus`
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._Result = None
         self._RequestId = None
 
     @property
@@ -7815,15 +7815,15 @@
     @RequestId.setter
     def RequestId(self, RequestId):
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         if params.get("Result") is not None:
-            self._Result = ApiEnvironmentStrategyStataus()
+            self._Result = ApiEnvironmentStrategyStatus()
             self._Result._deserialize(params.get("Result"))
         self._RequestId = params.get("RequestId")
 
 
 class DescribeApiForApiAppRequest(AbstractModel):
     """DescribeApiForApiApp请求参数结构体
 
@@ -9426,15 +9426,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param _Result: 符合条件的策略列表。
 注意：此字段可能返回 null，表示取不到有效值。
-        :type Result: :class:`tencentcloud.apigateway.v20180808.models.IPStrategysStatus`
+        :type Result: :class:`tencentcloud.apigateway.v20180808.models.IPStrategiesStatus`
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._Result = None
         self._RequestId = None
 
     @property
@@ -9452,15 +9452,15 @@
     @RequestId.setter
     def RequestId(self, RequestId):
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         if params.get("Result") is not None:
-            self._Result = IPStrategysStatus()
+            self._Result = IPStrategiesStatus()
             self._Result._deserialize(params.get("Result"))
         self._RequestId = params.get("RequestId")
 
 
 class DescribeLogSearchRequest(AbstractModel):
     """DescribeLogSearch请求参数结构体
 
@@ -13268,14 +13268,66 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class IPStrategiesStatus(AbstractModel):
+    """策略列表
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TotalCount: 策略数量。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TotalCount: int
+        :param _StrategySet: 策略列表。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type StrategySet: list of IPStrategy
+        """
+        self._TotalCount = None
+        self._StrategySet = None
+
+    @property
+    def TotalCount(self):
+        return self._TotalCount
+
+    @TotalCount.setter
+    def TotalCount(self, TotalCount):
+        self._TotalCount = TotalCount
+
+    @property
+    def StrategySet(self):
+        return self._StrategySet
+
+    @StrategySet.setter
+    def StrategySet(self, StrategySet):
+        self._StrategySet = StrategySet
+
+
+    def _deserialize(self, params):
+        self._TotalCount = params.get("TotalCount")
+        if params.get("StrategySet") is not None:
+            self._StrategySet = []
+            for item in params.get("StrategySet"):
+                obj = IPStrategy()
+                obj._deserialize(item)
+                self._StrategySet.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class IPStrategy(AbstractModel):
     """ip策略
 
     """
 
     def __init__(self):
         r"""
@@ -13565,66 +13617,14 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class IPStrategysStatus(AbstractModel):
-    """策略列表
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _TotalCount: 策略数量。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type TotalCount: int
-        :param _StrategySet: 策略列表。
-注意：此字段可能返回 null，表示取不到有效值。
-        :type StrategySet: list of IPStrategy
-        """
-        self._TotalCount = None
-        self._StrategySet = None
-
-    @property
-    def TotalCount(self):
-        return self._TotalCount
-
-    @TotalCount.setter
-    def TotalCount(self, TotalCount):
-        self._TotalCount = TotalCount
-
-    @property
-    def StrategySet(self):
-        return self._StrategySet
-
-    @StrategySet.setter
-    def StrategySet(self, StrategySet):
-        self._StrategySet = StrategySet
-
-
-    def _deserialize(self, params):
-        self._TotalCount = params.get("TotalCount")
-        if params.get("StrategySet") is not None:
-            self._StrategySet = []
-            for item in params.get("StrategySet"):
-                obj = IPStrategy()
-                obj._deserialize(item)
-                self._StrategySet.append(obj)
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class ImportOpenApiRequest(AbstractModel):
     """ImportOpenApi请求参数结构体
 
     """
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.934/tencentcloud/apigateway/v20180808/apigateway_client.py` & `tencentcloud-sdk-python-apigateway-3.0.935/tencentcloud/apigateway/v20180808/apigateway_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1093,15 +1093,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeIPStrategysStatus(self, request):
-        """本接口（DescribeIPStrategysStatus）用于查询服务IP策略列表。
+        """本接口（DescribeIPStrategysStatus）用于查询服务IP策略列表，因为接口名拼写错误，已不推荐使用，请优先使用DescribeIPStrategiesStatus接口。
 
         :param request: Request instance for DescribeIPStrategysStatus.
         :type request: :class:`tencentcloud.apigateway.v20180808.models.DescribeIPStrategysStatusRequest`
         :rtype: :class:`tencentcloud.apigateway.v20180808.models.DescribeIPStrategysStatusResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.934/tencentcloud/__init__.py` & `tencentcloud-sdk-python-apigateway-3.0.935/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.934'
+__version__ = '3.0.935'
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.934/PKG-INFO` & `tencentcloud-sdk-python-apigateway-3.0.935/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-apigateway
-Version: 3.0.934
+Version: 3.0.935
 Summary: Tencent Cloud Apigateway SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.934/tencentcloud_sdk_python_apigateway.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-apigateway-3.0.935/tencentcloud_sdk_python_apigateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apigateway-3.0.934/tencentcloud_sdk_python_apigateway.egg-info/PKG-INFO` & `tencentcloud-sdk-python-apigateway-3.0.935/tencentcloud_sdk_python_apigateway.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-apigateway
-Version: 3.0.934
+Version: 3.0.935
 Summary: Tencent Cloud Apigateway SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-apigateway-3.0.934/README.rst` & `tencentcloud-sdk-python-apigateway-3.0.935/README.rst`

 * *Files identical despite different names*

