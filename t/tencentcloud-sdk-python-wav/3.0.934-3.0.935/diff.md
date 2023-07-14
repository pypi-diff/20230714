# Comparing `tmp/tencentcloud-sdk-python-wav-3.0.934.tar.gz` & `tmp/tencentcloud-sdk-python-wav-3.0.935.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-wav-3.0.934.tar", last modified: Thu Jul 13 00:38:30 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-wav-3.0.935.tar", last modified: Fri Jul 14 00:46:00 2023, max compression
```

## Comparing `tencentcloud-sdk-python-wav-3.0.934.tar` & `tencentcloud-sdk-python-wav-3.0.935.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:38:30.000000 tencentcloud-sdk-python-wav-3.0.934/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-13 00:38:29.000000 tencentcloud-sdk-python-wav-3.0.934/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:38:30.000000 tencentcloud-sdk-python-wav-3.0.934/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-13 00:38:29.000000 tencentcloud-sdk-python-wav-3.0.934/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:38:30.000000 tencentcloud-sdk-python-wav-3.0.934/tencentcloud/wav/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:38:29.000000 tencentcloud-sdk-python-wav-3.0.934/tencentcloud/wav/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:38:30.000000 tencentcloud-sdk-python-wav-3.0.934/tencentcloud/wav/v20210129/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:38:29.000000 tencentcloud-sdk-python-wav-3.0.934/tencentcloud/wav/v20210129/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1771 2023-07-13 00:38:29.000000 tencentcloud-sdk-python-wav-3.0.934/tencentcloud/wav/v20210129/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   224775 2023-07-13 00:38:29.000000 tencentcloud-sdk-python-wav-3.0.934/tencentcloud/wav/v20210129/models.py
--rw-r--r--   0 root         (0) root         (0)    25908 2023-07-13 00:38:29.000000 tencentcloud-sdk-python-wav-3.0.934/tencentcloud/wav/v20210129/wav_client.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-13 00:38:30.000000 tencentcloud-sdk-python-wav-3.0.934/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:38:30.000000 tencentcloud-sdk-python-wav-3.0.934/tencentcloud_sdk_python_wav.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 00:38:30.000000 tencentcloud-sdk-python-wav-3.0.934/tencentcloud_sdk_python_wav.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-13 00:38:30.000000 tencentcloud-sdk-python-wav-3.0.934/tencentcloud_sdk_python_wav.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-13 00:38:30.000000 tencentcloud-sdk-python-wav-3.0.934/tencentcloud_sdk_python_wav.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-13 00:38:30.000000 tencentcloud-sdk-python-wav-3.0.934/tencentcloud_sdk_python_wav.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-13 00:38:30.000000 tencentcloud-sdk-python-wav-3.0.934/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-13 00:38:29.000000 tencentcloud-sdk-python-wav-3.0.934/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:46:00.000000 tencentcloud-sdk-python-wav-3.0.935/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-14 00:46:00.000000 tencentcloud-sdk-python-wav-3.0.935/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:46:00.000000 tencentcloud-sdk-python-wav-3.0.935/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-14 00:46:00.000000 tencentcloud-sdk-python-wav-3.0.935/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:46:00.000000 tencentcloud-sdk-python-wav-3.0.935/tencentcloud/wav/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:46:00.000000 tencentcloud-sdk-python-wav-3.0.935/tencentcloud/wav/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:46:00.000000 tencentcloud-sdk-python-wav-3.0.935/tencentcloud/wav/v20210129/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:46:00.000000 tencentcloud-sdk-python-wav-3.0.935/tencentcloud/wav/v20210129/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1771 2023-07-14 00:46:00.000000 tencentcloud-sdk-python-wav-3.0.935/tencentcloud/wav/v20210129/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   229073 2023-07-14 00:46:00.000000 tencentcloud-sdk-python-wav-3.0.935/tencentcloud/wav/v20210129/models.py
+-rw-r--r--   0 root         (0) root         (0)    25908 2023-07-14 00:46:00.000000 tencentcloud-sdk-python-wav-3.0.935/tencentcloud/wav/v20210129/wav_client.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-14 00:46:00.000000 tencentcloud-sdk-python-wav-3.0.935/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:46:00.000000 tencentcloud-sdk-python-wav-3.0.935/tencentcloud_sdk_python_wav.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 00:46:00.000000 tencentcloud-sdk-python-wav-3.0.935/tencentcloud_sdk_python_wav.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-14 00:46:00.000000 tencentcloud-sdk-python-wav-3.0.935/tencentcloud_sdk_python_wav.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 00:46:00.000000 tencentcloud-sdk-python-wav-3.0.935/tencentcloud_sdk_python_wav.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-14 00:46:00.000000 tencentcloud-sdk-python-wav-3.0.935/tencentcloud_sdk_python_wav.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 00:46:00.000000 tencentcloud-sdk-python-wav-3.0.935/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-14 00:46:00.000000 tencentcloud-sdk-python-wav-3.0.935/README.rst
```

### Comparing `tencentcloud-sdk-python-wav-3.0.934/setup.py` & `tencentcloud-sdk-python-wav-3.0.935/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wav-3.0.934/tencentcloud/__init__.py` & `tencentcloud-sdk-python-wav-3.0.935/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-wav-3.0.934/tencentcloud/wav/v20210129/errorcodes.py` & `tencentcloud-sdk-python-wav-3.0.935/tencentcloud/wav/v20210129/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wav-3.0.934/tencentcloud/wav/v20210129/models.py` & `tencentcloud-sdk-python-wav-3.0.935/tencentcloud/wav/v20210129/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -2672,14 +2672,41 @@
         :type NextFollowTime: int
         :param _EnterpriseTags: 已为该客户添加的企业标签信息
 注意：此字段可能返回 null，表示取不到有效值。
         :type EnterpriseTags: list of EnterpriseTag
         :param _ChannelTags: 已为该客户添加的渠道标签信息
 注意：此字段可能返回 null，表示取不到有效值。
         :type ChannelTags: list of ChannelTag
+        :param _LeadId: 关联线索id
+        :type LeadId: int
+        :param _WxId: 客户微信id
+        :type WxId: str
+        :param _Position: 顾问职位
+        :type Position: str
+        :param _IsBindWx: 是否关联微信 1 是 0 否
+        :type IsBindWx: int
+        :param _IsInvalid: 是否无效
+        :type IsInvalid: int
+        :param _InvalidType: 无效类型
+        :type InvalidType: str
+        :param _InvalidTypeName: 无效类型名称
+        :type InvalidTypeName: str
+        :param _InvalidTime: 无效时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InvalidTime: int
+        :param _InvalidRemark: 由顾问手动输入的无效原因文字
+        :type InvalidRemark: str
+        :param _IsLose: 线索是否战败
+        :type IsLose: int
+        :param _LoseType: 战败类型
+        :type LoseType: str
+        :param _LoseTypeName: 战败类型名称
+        :type LoseTypeName: str
+        :param _LoseRemark: 战败申请原因
+        :type LoseRemark: str
         """
         self._CustomerId = None
         self._DealerCode = None
         self._UnionId = None
         self._CreateTime = None
         self._UserName = None
         self._Gender = None
@@ -2712,14 +2739,27 @@
         self._OrgIdList = None
         self._Introducer = None
         self._IntroducerPhone = None
         self._FollowTime = None
         self._NextFollowTime = None
         self._EnterpriseTags = None
         self._ChannelTags = None
+        self._LeadId = None
+        self._WxId = None
+        self._Position = None
+        self._IsBindWx = None
+        self._IsInvalid = None
+        self._InvalidType = None
+        self._InvalidTypeName = None
+        self._InvalidTime = None
+        self._InvalidRemark = None
+        self._IsLose = None
+        self._LoseType = None
+        self._LoseTypeName = None
+        self._LoseRemark = None
 
     @property
     def CustomerId(self):
         return self._CustomerId
 
     @CustomerId.setter
     def CustomerId(self, CustomerId):
@@ -3025,14 +3065,118 @@
     def ChannelTags(self):
         return self._ChannelTags
 
     @ChannelTags.setter
     def ChannelTags(self, ChannelTags):
         self._ChannelTags = ChannelTags
 
+    @property
+    def LeadId(self):
+        return self._LeadId
+
+    @LeadId.setter
+    def LeadId(self, LeadId):
+        self._LeadId = LeadId
+
+    @property
+    def WxId(self):
+        return self._WxId
+
+    @WxId.setter
+    def WxId(self, WxId):
+        self._WxId = WxId
+
+    @property
+    def Position(self):
+        return self._Position
+
+    @Position.setter
+    def Position(self, Position):
+        self._Position = Position
+
+    @property
+    def IsBindWx(self):
+        return self._IsBindWx
+
+    @IsBindWx.setter
+    def IsBindWx(self, IsBindWx):
+        self._IsBindWx = IsBindWx
+
+    @property
+    def IsInvalid(self):
+        return self._IsInvalid
+
+    @IsInvalid.setter
+    def IsInvalid(self, IsInvalid):
+        self._IsInvalid = IsInvalid
+
+    @property
+    def InvalidType(self):
+        return self._InvalidType
+
+    @InvalidType.setter
+    def InvalidType(self, InvalidType):
+        self._InvalidType = InvalidType
+
+    @property
+    def InvalidTypeName(self):
+        return self._InvalidTypeName
+
+    @InvalidTypeName.setter
+    def InvalidTypeName(self, InvalidTypeName):
+        self._InvalidTypeName = InvalidTypeName
+
+    @property
+    def InvalidTime(self):
+        return self._InvalidTime
+
+    @InvalidTime.setter
+    def InvalidTime(self, InvalidTime):
+        self._InvalidTime = InvalidTime
+
+    @property
+    def InvalidRemark(self):
+        return self._InvalidRemark
+
+    @InvalidRemark.setter
+    def InvalidRemark(self, InvalidRemark):
+        self._InvalidRemark = InvalidRemark
+
+    @property
+    def IsLose(self):
+        return self._IsLose
+
+    @IsLose.setter
+    def IsLose(self, IsLose):
+        self._IsLose = IsLose
+
+    @property
+    def LoseType(self):
+        return self._LoseType
+
+    @LoseType.setter
+    def LoseType(self, LoseType):
+        self._LoseType = LoseType
+
+    @property
+    def LoseTypeName(self):
+        return self._LoseTypeName
+
+    @LoseTypeName.setter
+    def LoseTypeName(self, LoseTypeName):
+        self._LoseTypeName = LoseTypeName
+
+    @property
+    def LoseRemark(self):
+        return self._LoseRemark
+
+    @LoseRemark.setter
+    def LoseRemark(self, LoseRemark):
+        self._LoseRemark = LoseRemark
+
 
     def _deserialize(self, params):
         self._CustomerId = params.get("CustomerId")
         self._DealerCode = params.get("DealerCode")
         self._UnionId = params.get("UnionId")
         self._CreateTime = params.get("CreateTime")
         self._UserName = params.get("UserName")
@@ -3083,14 +3227,27 @@
                 self._EnterpriseTags.append(obj)
         if params.get("ChannelTags") is not None:
             self._ChannelTags = []
             for item in params.get("ChannelTags"):
                 obj = ChannelTag()
                 obj._deserialize(item)
                 self._ChannelTags.append(obj)
+        self._LeadId = params.get("LeadId")
+        self._WxId = params.get("WxId")
+        self._Position = params.get("Position")
+        self._IsBindWx = params.get("IsBindWx")
+        self._IsInvalid = params.get("IsInvalid")
+        self._InvalidType = params.get("InvalidType")
+        self._InvalidTypeName = params.get("InvalidTypeName")
+        self._InvalidTime = params.get("InvalidTime")
+        self._InvalidRemark = params.get("InvalidRemark")
+        self._IsLose = params.get("IsLose")
+        self._LoseType = params.get("LoseType")
+        self._LoseTypeName = params.get("LoseTypeName")
+        self._LoseRemark = params.get("LoseRemark")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-wav-3.0.934/tencentcloud/wav/v20210129/wav_client.py` & `tencentcloud-sdk-python-wav-3.0.935/tencentcloud/wav/v20210129/wav_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wav-3.0.934/tencentcloud_sdk_python_wav.egg-info/PKG-INFO` & `tencentcloud-sdk-python-wav-3.0.935/tencentcloud_sdk_python_wav.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-wav
-Version: 3.0.934
+Version: 3.0.935
 Summary: Tencent Cloud Wav SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-wav-3.0.934/PKG-INFO` & `tencentcloud-sdk-python-wav-3.0.935/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-wav
-Version: 3.0.934
+Version: 3.0.935
 Summary: Tencent Cloud Wav SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-wav-3.0.934/README.rst` & `tencentcloud-sdk-python-wav-3.0.935/README.rst`

 * *Files identical despite different names*

