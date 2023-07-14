# Comparing `tmp/tencentcloud-sdk-python-lcic-3.0.934.tar.gz` & `tmp/tencentcloud-sdk-python-lcic-3.0.935.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-lcic-3.0.934.tar", last modified: Thu Jul 13 00:25:17 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-lcic-3.0.935.tar", last modified: Fri Jul 14 00:33:27 2023, max compression
```

## Comparing `tencentcloud-sdk-python-lcic-3.0.934.tar` & `tencentcloud-sdk-python-lcic-3.0.935.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:25:17.000000 tencentcloud-sdk-python-lcic-3.0.934/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-13 00:25:16.000000 tencentcloud-sdk-python-lcic-3.0.934/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:25:17.000000 tencentcloud-sdk-python-lcic-3.0.934/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-13 00:25:16.000000 tencentcloud-sdk-python-lcic-3.0.934/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:25:17.000000 tencentcloud-sdk-python-lcic-3.0.934/tencentcloud/lcic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:25:17.000000 tencentcloud-sdk-python-lcic-3.0.934/tencentcloud/lcic/v20220817/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:25:16.000000 tencentcloud-sdk-python-lcic-3.0.934/tencentcloud/lcic/v20220817/__init__.py
--rw-r--r--   0 root         (0) root         (0)    48649 2023-07-13 00:25:16.000000 tencentcloud-sdk-python-lcic-3.0.934/tencentcloud/lcic/v20220817/lcic_client.py
--rw-r--r--   0 root         (0) root         (0)     4414 2023-07-13 00:25:16.000000 tencentcloud-sdk-python-lcic-3.0.934/tencentcloud/lcic/v20220817/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   229346 2023-07-13 00:25:16.000000 tencentcloud-sdk-python-lcic-3.0.934/tencentcloud/lcic/v20220817/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:25:16.000000 tencentcloud-sdk-python-lcic-3.0.934/tencentcloud/lcic/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-13 00:25:17.000000 tencentcloud-sdk-python-lcic-3.0.934/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:25:17.000000 tencentcloud-sdk-python-lcic-3.0.934/tencentcloud_sdk_python_lcic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 00:25:17.000000 tencentcloud-sdk-python-lcic-3.0.934/tencentcloud_sdk_python_lcic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-13 00:25:17.000000 tencentcloud-sdk-python-lcic-3.0.934/tencentcloud_sdk_python_lcic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-13 00:25:17.000000 tencentcloud-sdk-python-lcic-3.0.934/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-13 00:25:17.000000 tencentcloud-sdk-python-lcic-3.0.934/tencentcloud_sdk_python_lcic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-13 00:25:17.000000 tencentcloud-sdk-python-lcic-3.0.934/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-13 00:25:16.000000 tencentcloud-sdk-python-lcic-3.0.934/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:33:27.000000 tencentcloud-sdk-python-lcic-3.0.935/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-14 00:33:26.000000 tencentcloud-sdk-python-lcic-3.0.935/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:33:27.000000 tencentcloud-sdk-python-lcic-3.0.935/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-14 00:33:26.000000 tencentcloud-sdk-python-lcic-3.0.935/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:33:27.000000 tencentcloud-sdk-python-lcic-3.0.935/tencentcloud/lcic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:33:27.000000 tencentcloud-sdk-python-lcic-3.0.935/tencentcloud/lcic/v20220817/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:33:26.000000 tencentcloud-sdk-python-lcic-3.0.935/tencentcloud/lcic/v20220817/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    48649 2023-07-14 00:33:26.000000 tencentcloud-sdk-python-lcic-3.0.935/tencentcloud/lcic/v20220817/lcic_client.py
+-rw-r--r--   0 root         (0) root         (0)     4414 2023-07-14 00:33:26.000000 tencentcloud-sdk-python-lcic-3.0.935/tencentcloud/lcic/v20220817/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   229644 2023-07-14 00:33:26.000000 tencentcloud-sdk-python-lcic-3.0.935/tencentcloud/lcic/v20220817/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:33:26.000000 tencentcloud-sdk-python-lcic-3.0.935/tencentcloud/lcic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-14 00:33:27.000000 tencentcloud-sdk-python-lcic-3.0.935/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:33:27.000000 tencentcloud-sdk-python-lcic-3.0.935/tencentcloud_sdk_python_lcic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 00:33:27.000000 tencentcloud-sdk-python-lcic-3.0.935/tencentcloud_sdk_python_lcic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-14 00:33:27.000000 tencentcloud-sdk-python-lcic-3.0.935/tencentcloud_sdk_python_lcic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-14 00:33:27.000000 tencentcloud-sdk-python-lcic-3.0.935/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-14 00:33:27.000000 tencentcloud-sdk-python-lcic-3.0.935/tencentcloud_sdk_python_lcic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-14 00:33:27.000000 tencentcloud-sdk-python-lcic-3.0.935/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-14 00:33:26.000000 tencentcloud-sdk-python-lcic-3.0.935/README.rst
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.934/setup.py` & `tencentcloud-sdk-python-lcic-3.0.935/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.934/tencentcloud/__init__.py` & `tencentcloud-sdk-python-lcic-3.0.935/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-lcic-3.0.934/tencentcloud/lcic/v20220817/lcic_client.py` & `tencentcloud-sdk-python-lcic-3.0.935/tencentcloud/lcic/v20220817/lcic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.934/tencentcloud/lcic/v20220817/errorcodes.py` & `tencentcloud-sdk-python-lcic-3.0.935/tencentcloud/lcic/v20220817/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.934/tencentcloud/lcic/v20220817/models.py` & `tencentcloud-sdk-python-lcic-3.0.935/tencentcloud/lcic/v20220817/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2919,14 +2919,16 @@
         :type DocumentType: str
         :param _DocumentSize: 文档大小，单位：字节
         :type DocumentSize: int
         :param _UpdateTime: 更新的UNIX时间戳
         :type UpdateTime: int
         :param _Pages: 课件页数
         :type Pages: int
+        :param _Preview: 课件预览地址
+        :type Preview: str
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._DocumentId = None
         self._DocumentUrl = None
         self._DocumentName = None
         self._Owner = None
@@ -2937,14 +2939,15 @@
         self._TranscodeProgress = None
         self._TranscodeState = None
         self._TranscodeInfo = None
         self._DocumentType = None
         self._DocumentSize = None
         self._UpdateTime = None
         self._Pages = None
+        self._Preview = None
         self._RequestId = None
 
     @property
     def DocumentId(self):
         return self._DocumentId
 
     @DocumentId.setter
@@ -3060,14 +3063,22 @@
         return self._Pages
 
     @Pages.setter
     def Pages(self, Pages):
         self._Pages = Pages
 
     @property
+    def Preview(self):
+        return self._Preview
+
+    @Preview.setter
+    def Preview(self, Preview):
+        self._Preview = Preview
+
+    @property
     def RequestId(self):
         return self._RequestId
 
     @RequestId.setter
     def RequestId(self, RequestId):
         self._RequestId = RequestId
 
@@ -3084,14 +3095,15 @@
         self._TranscodeProgress = params.get("TranscodeProgress")
         self._TranscodeState = params.get("TranscodeState")
         self._TranscodeInfo = params.get("TranscodeInfo")
         self._DocumentType = params.get("DocumentType")
         self._DocumentSize = params.get("DocumentSize")
         self._UpdateTime = params.get("UpdateTime")
         self._Pages = params.get("Pages")
+        self._Preview = params.get("Preview")
         self._RequestId = params.get("RequestId")
 
 
 class DescribeDocumentsByRoomRequest(AbstractModel):
     """DescribeDocumentsByRoom请求参数结构体
 
     """
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.934/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-lcic-3.0.935/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lcic
-Version: 3.0.934
+Version: 3.0.935
 Summary: Tencent Cloud Lcic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.934/PKG-INFO` & `tencentcloud-sdk-python-lcic-3.0.935/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lcic
-Version: 3.0.934
+Version: 3.0.935
 Summary: Tencent Cloud Lcic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.934/README.rst` & `tencentcloud-sdk-python-lcic-3.0.935/README.rst`

 * *Files identical despite different names*

