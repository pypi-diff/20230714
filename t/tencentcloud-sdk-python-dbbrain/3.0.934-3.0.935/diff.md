# Comparing `tmp/tencentcloud-sdk-python-dbbrain-3.0.934.tar.gz` & `tmp/tencentcloud-sdk-python-dbbrain-3.0.935.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dbbrain-3.0.934.tar", last modified: Thu Jul 13 00:20:26 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dbbrain-3.0.935.tar", last modified: Fri Jul 14 00:22:00 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dbbrain-3.0.934.tar` & `tencentcloud-sdk-python-dbbrain-3.0.935.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:20:26.000000 tencentcloud-sdk-python-dbbrain-3.0.934/
--rw-r--r--   0 root         (0) root         (0)     1014 2023-07-13 00:20:26.000000 tencentcloud-sdk-python-dbbrain-3.0.934/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:20:26.000000 tencentcloud-sdk-python-dbbrain-3.0.934/tencentcloud_sdk_python_dbbrain.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 00:20:26.000000 tencentcloud-sdk-python-dbbrain-3.0.934/tencentcloud_sdk_python_dbbrain.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      663 2023-07-13 00:20:26.000000 tencentcloud-sdk-python-dbbrain-3.0.934/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-13 00:20:26.000000 tencentcloud-sdk-python-dbbrain-3.0.934/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-13 00:20:26.000000 tencentcloud-sdk-python-dbbrain-3.0.934/tencentcloud_sdk_python_dbbrain.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:20:26.000000 tencentcloud-sdk-python-dbbrain-3.0.934/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-13 00:20:26.000000 tencentcloud-sdk-python-dbbrain-3.0.934/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:20:26.000000 tencentcloud-sdk-python-dbbrain-3.0.934/tencentcloud/dbbrain/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:20:26.000000 tencentcloud-sdk-python-dbbrain-3.0.934/tencentcloud/dbbrain/v20210527/
--rw-r--r--   0 root         (0) root         (0)    53256 2023-07-13 00:20:26.000000 tencentcloud-sdk-python-dbbrain-3.0.934/tencentcloud/dbbrain/v20210527/dbbrain_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:20:26.000000 tencentcloud-sdk-python-dbbrain-3.0.934/tencentcloud/dbbrain/v20210527/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2058 2023-07-13 00:20:26.000000 tencentcloud-sdk-python-dbbrain-3.0.934/tencentcloud/dbbrain/v20210527/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   325442 2023-07-13 00:20:26.000000 tencentcloud-sdk-python-dbbrain-3.0.934/tencentcloud/dbbrain/v20210527/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:20:26.000000 tencentcloud-sdk-python-dbbrain-3.0.934/tencentcloud/dbbrain/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:20:26.000000 tencentcloud-sdk-python-dbbrain-3.0.934/tencentcloud/dbbrain/v20191016/
--rw-r--r--   0 root         (0) root         (0)    27659 2023-07-13 00:20:26.000000 tencentcloud-sdk-python-dbbrain-3.0.934/tencentcloud/dbbrain/v20191016/dbbrain_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:20:26.000000 tencentcloud-sdk-python-dbbrain-3.0.934/tencentcloud/dbbrain/v20191016/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1567 2023-07-13 00:20:26.000000 tencentcloud-sdk-python-dbbrain-3.0.934/tencentcloud/dbbrain/v20191016/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   183920 2023-07-13 00:20:26.000000 tencentcloud-sdk-python-dbbrain-3.0.934/tencentcloud/dbbrain/v20191016/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-13 00:20:26.000000 tencentcloud-sdk-python-dbbrain-3.0.934/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-13 00:20:26.000000 tencentcloud-sdk-python-dbbrain-3.0.934/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      749 2023-07-13 00:20:26.000000 tencentcloud-sdk-python-dbbrain-3.0.934/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:22:00.000000 tencentcloud-sdk-python-dbbrain-3.0.935/
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-07-14 00:22:00.000000 tencentcloud-sdk-python-dbbrain-3.0.935/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:22:00.000000 tencentcloud-sdk-python-dbbrain-3.0.935/tencentcloud_sdk_python_dbbrain.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 00:22:00.000000 tencentcloud-sdk-python-dbbrain-3.0.935/tencentcloud_sdk_python_dbbrain.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      663 2023-07-14 00:22:00.000000 tencentcloud-sdk-python-dbbrain-3.0.935/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-14 00:22:00.000000 tencentcloud-sdk-python-dbbrain-3.0.935/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-14 00:22:00.000000 tencentcloud-sdk-python-dbbrain-3.0.935/tencentcloud_sdk_python_dbbrain.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:22:00.000000 tencentcloud-sdk-python-dbbrain-3.0.935/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-14 00:22:00.000000 tencentcloud-sdk-python-dbbrain-3.0.935/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:22:00.000000 tencentcloud-sdk-python-dbbrain-3.0.935/tencentcloud/dbbrain/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:22:00.000000 tencentcloud-sdk-python-dbbrain-3.0.935/tencentcloud/dbbrain/v20210527/
+-rw-r--r--   0 root         (0) root         (0)    53256 2023-07-14 00:22:00.000000 tencentcloud-sdk-python-dbbrain-3.0.935/tencentcloud/dbbrain/v20210527/dbbrain_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:22:00.000000 tencentcloud-sdk-python-dbbrain-3.0.935/tencentcloud/dbbrain/v20210527/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2023-07-14 00:22:00.000000 tencentcloud-sdk-python-dbbrain-3.0.935/tencentcloud/dbbrain/v20210527/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   325476 2023-07-14 00:22:00.000000 tencentcloud-sdk-python-dbbrain-3.0.935/tencentcloud/dbbrain/v20210527/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:22:00.000000 tencentcloud-sdk-python-dbbrain-3.0.935/tencentcloud/dbbrain/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:22:00.000000 tencentcloud-sdk-python-dbbrain-3.0.935/tencentcloud/dbbrain/v20191016/
+-rw-r--r--   0 root         (0) root         (0)    27659 2023-07-14 00:22:00.000000 tencentcloud-sdk-python-dbbrain-3.0.935/tencentcloud/dbbrain/v20191016/dbbrain_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:22:00.000000 tencentcloud-sdk-python-dbbrain-3.0.935/tencentcloud/dbbrain/v20191016/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-07-14 00:22:00.000000 tencentcloud-sdk-python-dbbrain-3.0.935/tencentcloud/dbbrain/v20191016/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   183920 2023-07-14 00:22:00.000000 tencentcloud-sdk-python-dbbrain-3.0.935/tencentcloud/dbbrain/v20191016/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-14 00:22:00.000000 tencentcloud-sdk-python-dbbrain-3.0.935/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-14 00:22:00.000000 tencentcloud-sdk-python-dbbrain-3.0.935/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      749 2023-07-14 00:22:00.000000 tencentcloud-sdk-python-dbbrain-3.0.935/README.rst
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.934/setup.py` & `tencentcloud-sdk-python-dbbrain-3.0.935/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.934/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-dbbrain-3.0.935/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.934/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dbbrain-3.0.935/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dbbrain
-Version: 3.0.934
+Version: 3.0.935
 Summary: Tencent Cloud Dbbrain SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.934/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dbbrain-3.0.935/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.934/tencentcloud/dbbrain/v20210527/dbbrain_client.py` & `tencentcloud-sdk-python-dbbrain-3.0.935/tencentcloud/dbbrain/v20210527/dbbrain_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.934/tencentcloud/dbbrain/v20210527/errorcodes.py` & `tencentcloud-sdk-python-dbbrain-3.0.935/tencentcloud/dbbrain/v20210527/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.934/tencentcloud/dbbrain/v20210527/models.py` & `tencentcloud-sdk-python-dbbrain-3.0.935/tencentcloud/dbbrain/v20210527/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -731,15 +731,15 @@
 class CloseAuditServiceRequest(AbstractModel):
     """CloseAuditService请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Product: 服务产品类型，支持值包括： "dcdb" - 云数据库 Tdsql， "mariadb" - 云数据库 MariaDB for MariaDB。
+        :param _Product: 服务产品类型，支持值包括： "dcdb" - 云数据库 Tdsql， "mariadb" - 云数据库 MariaDB。
         :type Product: str
         :param _NodeRequestType: 与Product保持一致。如："dcdb" ,"mariadb"。
         :type NodeRequestType: str
         :param _InstanceId: 实例Id。
         :type InstanceId: str
         """
         self._Product = None
@@ -2670,15 +2670,15 @@
 class DescribeAuditInstanceListRequest(AbstractModel):
     """DescribeAuditInstanceList请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Product: 服务产品类型，支持值包括： "dcdb" - 云数据库 Tdsql， "mariadb" - 云数据库 MariaDB for MariaDB。
+        :param _Product: 服务产品类型，支持值包括： "dcdb" - 云数据库 Tdsql， "mariadb" - 云数据库 MariaDB。
         :type Product: str
         :param _NodeRequestType: 与Product保持一致。如："dcdb" ,"mariadb"。
         :type NodeRequestType: str
         :param _AuditSwitch: 审计状态标识，0-未开通审计；1-已开通审计，默认为0。
         :type AuditSwitch: int
         :param _Offset: 偏移量，默认为0。
         :type Offset: int
@@ -8431,23 +8431,23 @@
 class ModifyAuditServiceRequest(AbstractModel):
     """ModifyAuditService请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Product: 服务产品类型，支持值包括： "dcdb" - 云数据库 Tdsql， "mariadb" - 云数据库 MariaDB for MariaDB。
+        :param _Product: 服务产品类型，支持值包括： "dcdb" - 云数据库 Tdsql， "mariadb" - 云数据库 MariaDB。
         :type Product: str
         :param _NodeRequestType: 与Product保持一致。如："dcdb" ,"mariadb"。
         :type NodeRequestType: str
         :param _InstanceId: 实例ID。
         :type InstanceId: str
-        :param _LogExpireDay: 日志保存总时长，只能是7,30,90,180,365,1095,1825
+        :param _LogExpireDay: 日志保存总时长，只能是7,30,90,180,365,1095,1825。
         :type LogExpireDay: int
-        :param _HotLogExpireDay: 高频日志保存时长，只能是7,30,90,180,365,1095,1825
+        :param _HotLogExpireDay: 高频日志保存时长，只能是7,30,90,180,365,1095,1825。
         :type HotLogExpireDay: int
         """
         self._Product = None
         self._NodeRequestType = None
         self._InstanceId = None
         self._LogExpireDay = None
         self._HotLogExpireDay = None
@@ -9084,23 +9084,23 @@
 class OpenAuditServiceRequest(AbstractModel):
     """OpenAuditService请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Product: 与Product保持一致。如："dcdb" ,"mariadb"。
+        :param _Product: 服务产品类型，支持值包括： "dcdb" - 云数据库 Tdsql， "mariadb" - 云数据库 MariaDB。
         :type Product: str
         :param _NodeRequestType: 与Product保持一致。如："dcdb" ,"mariadb"。
         :type NodeRequestType: str
-        :param _InstanceId: 实例ID
+        :param _InstanceId: 实例ID。
         :type InstanceId: str
-        :param _LogExpireDay: 日志保存总时长，只能是7,30,90,180,365,1095,1825
+        :param _LogExpireDay: 日志保存总时长，只能是7,30,90,180,365,1095,1825。
         :type LogExpireDay: int
-        :param _HotLogExpireDay: 高频日志保存时长，只能是7,30,90,180,365,1095,1825
+        :param _HotLogExpireDay: 高频日志保存时长，只能是7,30,90,180,365,1095,1825。
         :type HotLogExpireDay: int
         """
         self._Product = None
         self._NodeRequestType = None
         self._InstanceId = None
         self._LogExpireDay = None
         self._HotLogExpireDay = None
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.934/tencentcloud/dbbrain/v20191016/dbbrain_client.py` & `tencentcloud-sdk-python-dbbrain-3.0.935/tencentcloud/dbbrain/v20191016/dbbrain_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.934/tencentcloud/dbbrain/v20191016/errorcodes.py` & `tencentcloud-sdk-python-dbbrain-3.0.935/tencentcloud/dbbrain/v20191016/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.934/tencentcloud/dbbrain/v20191016/models.py` & `tencentcloud-sdk-python-dbbrain-3.0.935/tencentcloud/dbbrain/v20191016/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.934/PKG-INFO` & `tencentcloud-sdk-python-dbbrain-3.0.935/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dbbrain
-Version: 3.0.934
+Version: 3.0.935
 Summary: Tencent Cloud Dbbrain SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.934/README.rst` & `tencentcloud-sdk-python-dbbrain-3.0.935/README.rst`

 * *Files identical despite different names*

