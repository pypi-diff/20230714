# Comparing `tmp/tencentcloud-sdk-python-tke-3.0.934.tar.gz` & `tmp/tencentcloud-sdk-python-tke-3.0.935.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tke-3.0.934.tar", last modified: Thu Jul 13 00:36:06 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tke-3.0.935.tar", last modified: Fri Jul 14 00:41:02 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tke-3.0.934.tar` & `tencentcloud-sdk-python-tke-3.0.935.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:36:06.000000 tencentcloud-sdk-python-tke-3.0.934/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-13 00:36:06.000000 tencentcloud-sdk-python-tke-3.0.934/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:36:06.000000 tencentcloud-sdk-python-tke-3.0.934/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:36:06.000000 tencentcloud-sdk-python-tke-3.0.934/tencentcloud/tke/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:36:06.000000 tencentcloud-sdk-python-tke-3.0.934/tencentcloud/tke/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:36:06.000000 tencentcloud-sdk-python-tke-3.0.934/tencentcloud/tke/v20180525/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:36:06.000000 tencentcloud-sdk-python-tke-3.0.934/tencentcloud/tke/v20180525/__init__.py
--rw-r--r--   0 root         (0) root         (0)   190375 2023-07-13 00:36:06.000000 tencentcloud-sdk-python-tke-3.0.934/tencentcloud/tke/v20180525/tke_client.py
--rw-r--r--   0 root         (0) root         (0)    19591 2023-07-13 00:36:06.000000 tencentcloud-sdk-python-tke-3.0.934/tencentcloud/tke/v20180525/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)  1059069 2023-07-13 00:36:06.000000 tencentcloud-sdk-python-tke-3.0.934/tencentcloud/tke/v20180525/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-13 00:36:06.000000 tencentcloud-sdk-python-tke-3.0.934/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-13 00:36:06.000000 tencentcloud-sdk-python-tke-3.0.934/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-13 00:36:06.000000 tencentcloud-sdk-python-tke-3.0.934/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-13 00:36:06.000000 tencentcloud-sdk-python-tke-3.0.934/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:36:06.000000 tencentcloud-sdk-python-tke-3.0.934/tencentcloud_sdk_python_tke.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 00:36:06.000000 tencentcloud-sdk-python-tke-3.0.934/tencentcloud_sdk_python_tke.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-13 00:36:06.000000 tencentcloud-sdk-python-tke-3.0.934/tencentcloud_sdk_python_tke.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-13 00:36:06.000000 tencentcloud-sdk-python-tke-3.0.934/tencentcloud_sdk_python_tke.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-13 00:36:06.000000 tencentcloud-sdk-python-tke-3.0.934/tencentcloud_sdk_python_tke.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:41:02.000000 tencentcloud-sdk-python-tke-3.0.935/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-14 00:41:02.000000 tencentcloud-sdk-python-tke-3.0.935/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:41:02.000000 tencentcloud-sdk-python-tke-3.0.935/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:41:02.000000 tencentcloud-sdk-python-tke-3.0.935/tencentcloud/tke/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:41:02.000000 tencentcloud-sdk-python-tke-3.0.935/tencentcloud/tke/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:41:02.000000 tencentcloud-sdk-python-tke-3.0.935/tencentcloud/tke/v20180525/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:41:02.000000 tencentcloud-sdk-python-tke-3.0.935/tencentcloud/tke/v20180525/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   190375 2023-07-14 00:41:02.000000 tencentcloud-sdk-python-tke-3.0.935/tencentcloud/tke/v20180525/tke_client.py
+-rw-r--r--   0 root         (0) root         (0)    19591 2023-07-14 00:41:02.000000 tencentcloud-sdk-python-tke-3.0.935/tencentcloud/tke/v20180525/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)  1059069 2023-07-14 00:41:02.000000 tencentcloud-sdk-python-tke-3.0.935/tencentcloud/tke/v20180525/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-14 00:41:02.000000 tencentcloud-sdk-python-tke-3.0.935/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-14 00:41:02.000000 tencentcloud-sdk-python-tke-3.0.935/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 00:41:02.000000 tencentcloud-sdk-python-tke-3.0.935/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-14 00:41:02.000000 tencentcloud-sdk-python-tke-3.0.935/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:41:02.000000 tencentcloud-sdk-python-tke-3.0.935/tencentcloud_sdk_python_tke.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 00:41:02.000000 tencentcloud-sdk-python-tke-3.0.935/tencentcloud_sdk_python_tke.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-14 00:41:02.000000 tencentcloud-sdk-python-tke-3.0.935/tencentcloud_sdk_python_tke.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 00:41:02.000000 tencentcloud-sdk-python-tke-3.0.935/tencentcloud_sdk_python_tke.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-14 00:41:02.000000 tencentcloud-sdk-python-tke-3.0.935/tencentcloud_sdk_python_tke.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-tke-3.0.934/setup.py` & `tencentcloud-sdk-python-tke-3.0.935/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.934/tencentcloud/tke/v20180525/tke_client.py` & `tencentcloud-sdk-python-tke-3.0.935/tencentcloud/tke/v20180525/tke_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.934/tencentcloud/tke/v20180525/errorcodes.py` & `tencentcloud-sdk-python-tke-3.0.935/tencentcloud/tke/v20180525/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.934/tencentcloud/tke/v20180525/models.py` & `tencentcloud-sdk-python-tke-3.0.935/tencentcloud/tke/v20180525/models.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5079,18 +5079,18 @@
 class CreateClusterRequest(AbstractModel):
     """CreateCluster请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _ClusterCIDRSettings: 集群容器网络配置信息
-        :type ClusterCIDRSettings: :class:`tencentcloud.tke.v20180525.models.ClusterCIDRSettings`
         :param _ClusterType: 集群类型，托管集群：MANAGED_CLUSTER，独立集群：INDEPENDENT_CLUSTER。
         :type ClusterType: str
+        :param _ClusterCIDRSettings: 集群容器网络配置信息
+        :type ClusterCIDRSettings: :class:`tencentcloud.tke.v20180525.models.ClusterCIDRSettings`
         :param _RunInstancesForNode: CVM创建透传参数，json化字符串格式，详见[CVM创建实例](https://cloud.tencent.com/document/product/213/15730)接口。总机型(包括地域)数量不超过10个，相同机型(地域)购买多台机器可以通过设置参数中RunInstances中InstanceCount来实现。
         :type RunInstancesForNode: list of RunInstancesForNode
         :param _ClusterBasicSettings: 集群的基本配置信息
         :type ClusterBasicSettings: :class:`tencentcloud.tke.v20180525.models.ClusterBasicSettings`
         :param _ClusterAdvancedSettings: 集群高级配置信息
         :type ClusterAdvancedSettings: :class:`tencentcloud.tke.v20180525.models.ClusterAdvancedSettings`
         :param _InstanceAdvancedSettings: 节点高级配置信息
@@ -5098,41 +5098,41 @@
         :param _ExistedInstancesForNode: 已存在实例的配置信息。所有实例必须在同一个VPC中，最大数量不超过100，不支持添加竞价实例。
         :type ExistedInstancesForNode: list of ExistedInstancesForNode
         :param _InstanceDataDiskMountSettings: CVM类型和其对应的数据盘挂载配置信息
         :type InstanceDataDiskMountSettings: list of InstanceDataDiskMountSetting
         :param _ExtensionAddons: 需要安装的扩展组件信息
         :type ExtensionAddons: list of ExtensionAddon
         """
-        self._ClusterCIDRSettings = None
         self._ClusterType = None
+        self._ClusterCIDRSettings = None
         self._RunInstancesForNode = None
         self._ClusterBasicSettings = None
         self._ClusterAdvancedSettings = None
         self._InstanceAdvancedSettings = None
         self._ExistedInstancesForNode = None
         self._InstanceDataDiskMountSettings = None
         self._ExtensionAddons = None
 
     @property
-    def ClusterCIDRSettings(self):
-        return self._ClusterCIDRSettings
-
-    @ClusterCIDRSettings.setter
-    def ClusterCIDRSettings(self, ClusterCIDRSettings):
-        self._ClusterCIDRSettings = ClusterCIDRSettings
-
-    @property
     def ClusterType(self):
         return self._ClusterType
 
     @ClusterType.setter
     def ClusterType(self, ClusterType):
         self._ClusterType = ClusterType
 
     @property
+    def ClusterCIDRSettings(self):
+        return self._ClusterCIDRSettings
+
+    @ClusterCIDRSettings.setter
+    def ClusterCIDRSettings(self, ClusterCIDRSettings):
+        self._ClusterCIDRSettings = ClusterCIDRSettings
+
+    @property
     def RunInstancesForNode(self):
         return self._RunInstancesForNode
 
     @RunInstancesForNode.setter
     def RunInstancesForNode(self, RunInstancesForNode):
         self._RunInstancesForNode = RunInstancesForNode
 
@@ -5182,18 +5182,18 @@
 
     @ExtensionAddons.setter
     def ExtensionAddons(self, ExtensionAddons):
         self._ExtensionAddons = ExtensionAddons
 
 
     def _deserialize(self, params):
+        self._ClusterType = params.get("ClusterType")
         if params.get("ClusterCIDRSettings") is not None:
             self._ClusterCIDRSettings = ClusterCIDRSettings()
             self._ClusterCIDRSettings._deserialize(params.get("ClusterCIDRSettings"))
-        self._ClusterType = params.get("ClusterType")
         if params.get("RunInstancesForNode") is not None:
             self._RunInstancesForNode = []
             for item in params.get("RunInstancesForNode"):
                 obj = RunInstancesForNode()
                 obj._deserialize(item)
                 self._RunInstancesForNode.append(obj)
         if params.get("ClusterBasicSettings") is not None:
```

### Comparing `tencentcloud-sdk-python-tke-3.0.934/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tke-3.0.935/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tke-3.0.934/PKG-INFO` & `tencentcloud-sdk-python-tke-3.0.935/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tke
-Version: 3.0.934
+Version: 3.0.935
 Summary: Tencent Cloud Tke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tke-3.0.934/README.rst` & `tencentcloud-sdk-python-tke-3.0.935/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.934/tencentcloud_sdk_python_tke.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tke-3.0.935/tencentcloud_sdk_python_tke.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tke
-Version: 3.0.934
+Version: 3.0.935
 Summary: Tencent Cloud Tke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

