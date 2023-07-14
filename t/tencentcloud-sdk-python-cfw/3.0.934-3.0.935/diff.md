# Comparing `tmp/tencentcloud-sdk-python-cfw-3.0.934.tar.gz` & `tmp/tencentcloud-sdk-python-cfw-3.0.935.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cfw-3.0.934.tar", last modified: Thu Jul 13 00:17:56 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cfw-3.0.935.tar", last modified: Fri Jul 14 00:19:30 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cfw-3.0.934.tar` & `tencentcloud-sdk-python-cfw-3.0.935.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:17:56.000000 tencentcloud-sdk-python-cfw-3.0.934/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:17:56.000000 tencentcloud-sdk-python-cfw-3.0.934/tencentcloud_sdk_python_cfw.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 00:17:56.000000 tencentcloud-sdk-python-cfw-3.0.934/tencentcloud_sdk_python_cfw.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-13 00:17:56.000000 tencentcloud-sdk-python-cfw-3.0.934/tencentcloud_sdk_python_cfw.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-13 00:17:56.000000 tencentcloud-sdk-python-cfw-3.0.934/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-13 00:17:56.000000 tencentcloud-sdk-python-cfw-3.0.934/tencentcloud_sdk_python_cfw.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-13 00:17:56.000000 tencentcloud-sdk-python-cfw-3.0.934/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:17:56.000000 tencentcloud-sdk-python-cfw-3.0.934/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:17:56.000000 tencentcloud-sdk-python-cfw-3.0.934/tencentcloud/cfw/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:17:56.000000 tencentcloud-sdk-python-cfw-3.0.934/tencentcloud/cfw/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:17:56.000000 tencentcloud-sdk-python-cfw-3.0.934/tencentcloud/cfw/v20190904/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:17:56.000000 tencentcloud-sdk-python-cfw-3.0.934/tencentcloud/cfw/v20190904/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1836 2023-07-13 00:17:56.000000 tencentcloud-sdk-python-cfw-3.0.934/tencentcloud/cfw/v20190904/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   356341 2023-07-13 00:17:56.000000 tencentcloud-sdk-python-cfw-3.0.934/tencentcloud/cfw/v20190904/models.py
--rw-r--r--   0 root         (0) root         (0)    67446 2023-07-13 00:17:56.000000 tencentcloud-sdk-python-cfw-3.0.934/tencentcloud/cfw/v20190904/cfw_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-13 00:17:56.000000 tencentcloud-sdk-python-cfw-3.0.934/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-13 00:17:56.000000 tencentcloud-sdk-python-cfw-3.0.934/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-13 00:17:56.000000 tencentcloud-sdk-python-cfw-3.0.934/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-13 00:17:56.000000 tencentcloud-sdk-python-cfw-3.0.934/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:19:30.000000 tencentcloud-sdk-python-cfw-3.0.935/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:19:30.000000 tencentcloud-sdk-python-cfw-3.0.935/tencentcloud_sdk_python_cfw.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 00:19:30.000000 tencentcloud-sdk-python-cfw-3.0.935/tencentcloud_sdk_python_cfw.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-14 00:19:30.000000 tencentcloud-sdk-python-cfw-3.0.935/tencentcloud_sdk_python_cfw.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 00:19:30.000000 tencentcloud-sdk-python-cfw-3.0.935/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-14 00:19:30.000000 tencentcloud-sdk-python-cfw-3.0.935/tencentcloud_sdk_python_cfw.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-14 00:19:30.000000 tencentcloud-sdk-python-cfw-3.0.935/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:19:30.000000 tencentcloud-sdk-python-cfw-3.0.935/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:19:30.000000 tencentcloud-sdk-python-cfw-3.0.935/tencentcloud/cfw/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:19:30.000000 tencentcloud-sdk-python-cfw-3.0.935/tencentcloud/cfw/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:19:30.000000 tencentcloud-sdk-python-cfw-3.0.935/tencentcloud/cfw/v20190904/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:19:30.000000 tencentcloud-sdk-python-cfw-3.0.935/tencentcloud/cfw/v20190904/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-07-14 00:19:30.000000 tencentcloud-sdk-python-cfw-3.0.935/tencentcloud/cfw/v20190904/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   360649 2023-07-14 00:19:30.000000 tencentcloud-sdk-python-cfw-3.0.935/tencentcloud/cfw/v20190904/models.py
+-rw-r--r--   0 root         (0) root         (0)    69236 2023-07-14 00:19:30.000000 tencentcloud-sdk-python-cfw-3.0.935/tencentcloud/cfw/v20190904/cfw_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-14 00:19:30.000000 tencentcloud-sdk-python-cfw-3.0.935/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-14 00:19:30.000000 tencentcloud-sdk-python-cfw-3.0.935/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 00:19:30.000000 tencentcloud-sdk-python-cfw-3.0.935/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-14 00:19:30.000000 tencentcloud-sdk-python-cfw-3.0.935/README.rst
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.934/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cfw-3.0.935/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfw
-Version: 3.0.934
+Version: 3.0.935
 Summary: Tencent Cloud Cfw SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.934/setup.py` & `tencentcloud-sdk-python-cfw-3.0.935/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfw-3.0.934/tencentcloud/cfw/v20190904/errorcodes.py` & `tencentcloud-sdk-python-cfw-3.0.935/tencentcloud/cfw/v20190904/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfw-3.0.934/tencentcloud/cfw/v20190904/models.py` & `tencentcloud-sdk-python-cfw-3.0.935/tencentcloud/cfw/v20190904/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1479,14 +1479,122 @@
 
     def _deserialize(self, params):
         self._Status = params.get("Status")
         self._Info = params.get("Info")
         self._RequestId = params.get("RequestId")
 
 
+class CreateAddressTemplateRequest(AbstractModel):
+    """CreateAddressTemplate请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Name: 模板名称
+        :type Name: str
+        :param _Detail: 模板描述
+        :type Detail: str
+        :param _IpString: Type为1，ip模板eg：1.1.1.1,2.2.2.2；
+Type为5，域名模板eg：www.qq.com,www.tencent.com
+        :type IpString: str
+        :param _Type: 1 ip模板
+5 域名模板
+        :type Type: int
+        """
+        self._Name = None
+        self._Detail = None
+        self._IpString = None
+        self._Type = None
+
+    @property
+    def Name(self):
+        return self._Name
+
+    @Name.setter
+    def Name(self, Name):
+        self._Name = Name
+
+    @property
+    def Detail(self):
+        return self._Detail
+
+    @Detail.setter
+    def Detail(self, Detail):
+        self._Detail = Detail
+
+    @property
+    def IpString(self):
+        return self._IpString
+
+    @IpString.setter
+    def IpString(self, IpString):
+        self._IpString = IpString
+
+    @property
+    def Type(self):
+        return self._Type
+
+    @Type.setter
+    def Type(self, Type):
+        self._Type = Type
+
+
+    def _deserialize(self, params):
+        self._Name = params.get("Name")
+        self._Detail = params.get("Detail")
+        self._IpString = params.get("IpString")
+        self._Type = params.get("Type")
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
+class CreateAddressTemplateResponse(AbstractModel):
+    """CreateAddressTemplate返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Status: 创建结果,0成功
+        :type Status: int
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Status = None
+        self._RequestId = None
+
+    @property
+    def Status(self):
+        return self._Status
+
+    @Status.setter
+    def Status(self, Status):
+        self._Status = Status
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._Status = params.get("Status")
+        self._RequestId = params.get("RequestId")
+
+
 class CreateChooseVpcsRequest(AbstractModel):
     """CreateChooseVpcs请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -2566,14 +2674,84 @@
 
     def _deserialize(self, params):
         self._Status = params.get("Status")
         self._Info = params.get("Info")
         self._RequestId = params.get("RequestId")
 
 
+class DeleteAddressTemplateRequest(AbstractModel):
+    """DeleteAddressTemplate请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Uuid: 模板id
+        :type Uuid: str
+        """
+        self._Uuid = None
+
+    @property
+    def Uuid(self):
+        return self._Uuid
+
+    @Uuid.setter
+    def Uuid(self, Uuid):
+        self._Uuid = Uuid
+
+
+    def _deserialize(self, params):
+        self._Uuid = params.get("Uuid")
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
+class DeleteAddressTemplateResponse(AbstractModel):
+    """DeleteAddressTemplate返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Status: 删除结果,0成功
+        :type Status: int
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Status = None
+        self._RequestId = None
+
+    @property
+    def Status(self):
+        return self._Status
+
+    @Status.setter
+    def Status(self, Status):
+        self._Status = Status
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._Status = params.get("Status")
+        self._RequestId = params.get("RequestId")
+
+
 class DeleteAllAccessControlRuleRequest(AbstractModel):
     """DeleteAllAccessControlRule请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.934/tencentcloud/cfw/v20190904/cfw_client.py` & `tencentcloud-sdk-python-cfw-3.0.935/tencentcloud/cfw/v20190904/cfw_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def CreateAddressTemplate(self, request):
+        """创建地址模板规则
+
+        :param request: Request instance for CreateAddressTemplate.
+        :type request: :class:`tencentcloud.cfw.v20190904.models.CreateAddressTemplateRequest`
+        :rtype: :class:`tencentcloud.cfw.v20190904.models.CreateAddressTemplateResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateAddressTemplate", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateAddressTemplateResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def CreateChooseVpcs(self, request):
         """创建、选择vpc
 
         :param request: Request instance for CreateChooseVpcs.
         :type request: :class:`tencentcloud.cfw.v20190904.models.CreateChooseVpcsRequest`
         :rtype: :class:`tencentcloud.cfw.v20190904.models.CreateChooseVpcsResponse`
 
@@ -250,14 +273,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DeleteAddressTemplate(self, request):
+        """删除地址模板规则
+
+        :param request: Request instance for DeleteAddressTemplate.
+        :type request: :class:`tencentcloud.cfw.v20190904.models.DeleteAddressTemplateRequest`
+        :rtype: :class:`tencentcloud.cfw.v20190904.models.DeleteAddressTemplateResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteAddressTemplate", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteAddressTemplateResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def DeleteAllAccessControlRule(self, request):
         """全部删除规则
 
         :param request: Request instance for DeleteAllAccessControlRule.
         :type request: :class:`tencentcloud.cfw.v20190904.models.DeleteAllAccessControlRuleRequest`
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.934/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cfw-3.0.935/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cfw-3.0.934/PKG-INFO` & `tencentcloud-sdk-python-cfw-3.0.935/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfw
-Version: 3.0.934
+Version: 3.0.935
 Summary: Tencent Cloud Cfw SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.934/README.rst` & `tencentcloud-sdk-python-cfw-3.0.935/README.rst`

 * *Files identical despite different names*

