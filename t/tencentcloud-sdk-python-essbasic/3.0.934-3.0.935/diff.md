# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.934.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.935.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.934.tar", last modified: Thu Jul 13 00:22:17 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.935.tar", last modified: Fri Jul 14 00:30:29 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.934.tar` & `tencentcloud-sdk-python-essbasic-3.0.935.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/
--rw-r--r--   0 root         (0) root         (0)     1016 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/essbasic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/essbasic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16662 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    53839 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)   383583 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/essbasic/v20210526/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5392 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    53845 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/essbasic/v20201222/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)   270905 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      678 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-13 00:22:17.000000 tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/essbasic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16662 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    53839 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)   383862 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/essbasic/v20210526/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    53845 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/essbasic/v20201222/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)   270905 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      678 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-14 00:30:29.000000 tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.934/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.935/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/essbasic/v20210526/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1226,25 +1226,25 @@
 
     def __init__(self):
         r"""
         :param _Agent: 渠道应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _EmbedType: WEB嵌入资源类型。
 CREATE_SEAL: 创建印章
-CREATE_TEMPLATE：创建模版
-MODIFY_TEMPLATE：修改模版
-PREVIEW_TEMPLATE：预览模版
+CREATE_TEMPLATE：创建模板
+MODIFY_TEMPLATE：修改模板
+PREVIEW_TEMPLATE：预览模板
 PREVIEW_FLOW：预览合同文档
 PREVIEW_FLOW_DETAIL：预览合同详情
 PREVIEW_SEAL_LIST：预览印章列表
 PREVIEW_SEAL_DETAIL：预览印章详情
 EXTEND_SERVICE：扩展服务
         :type EmbedType: str
         :param _BusinessId: WEB嵌入的业务资源ID
-EmbedType取值MODIFY_TEMPLATE，PREVIEW_TEMPLATE时必填，取值为模版id
+EmbedType取值MODIFY_TEMPLATE，PREVIEW_TEMPLATE时必填，取值为模板id
 PREVIEW_FLOW，PREVIEW_FLOW_DETAIL时必填，取值为合同id
 PREVIEW_SEAL_DETAIL，必填，取值为印章id
         :type BusinessId: str
         :param _HiddenComponents: 是否隐藏控件，只有预览模板时生效
         :type HiddenComponents: bool
         :param _Operator: 渠道操作者信息
         :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
@@ -5574,23 +5574,23 @@
 
     """
 
     def __init__(self):
         r"""
         :param _CanEditFlow: 是否允许修改合同信息，true-是，false-否
         :type CanEditFlow: bool
-        :param _HideShowFlowName: 是否允许发起合同弹窗隐藏合同名称
+        :param _HideShowFlowName: 是否允许发起合同弹窗隐藏合同名称，true-允许，false-不允许
         :type HideShowFlowName: bool
-        :param _HideShowFlowType: 是否允许发起合同弹窗隐藏合同类型
+        :param _HideShowFlowType: 是否允许发起合同弹窗隐藏合同类型，true-允许，false-不允许
         :type HideShowFlowType: bool
-        :param _HideShowDeadline: 是否允许发起合同弹窗隐藏合同到期时间
+        :param _HideShowDeadline: 是否允许发起合同弹窗隐藏合同到期时间，true-允许，false-不允许
         :type HideShowDeadline: bool
-        :param _CanSkipAddApprover: 是否允许发起合同步骤跳过指定签署方步骤
+        :param _CanSkipAddApprover: 是否允许发起合同步骤跳过指定签署方步骤，true-允许，false-不允许
         :type CanSkipAddApprover: bool
-        :param _CustomCreateFlowDescription: 定制化发起合同页合同描述信息
+        :param _CustomCreateFlowDescription: 定制化发起合同弹窗的描述信息，描述信息最长500
         :type CustomCreateFlowDescription: str
         """
         self._CanEditFlow = None
         self._HideShowFlowName = None
         self._HideShowFlowType = None
         self._HideShowDeadline = None
         self._CanSkipAddApprover = None
@@ -7710,16 +7710,16 @@
         :param _ApproverSignTypes: 签署人签署合同时的认证方式
 1-人脸认证 2-签署密码 3-运营商三要素(默认为1,2)
         :type ApproverSignTypes: list of int
         :param _SignId: 签署ID
 - 发起流程时系统自动补充
 - 创建签署链接时，可以通过查询详情接口获得签署人的SignId，然后可传入此值为该签署人创建签署链接，无需再传姓名、手机号、证件号等其他信息
         :type SignId: str
-        :param _NotifyType: SMS: 短信; NONE: 不发信息
-默认为SMS(该字段对子客无效)
+        :param _NotifyType: SMS: 短信(需确保“电子签短信通知签署方”功能是开启状态才能生效); NONE: 不发信息
+默认为SMS(签署方为子客时该字段不生效)
         :type NotifyType: str
         """
         self._Name = None
         self._IdCardType = None
         self._IdCardNumber = None
         self._Mobile = None
         self._OrganizationName = None
@@ -8781,15 +8781,15 @@
         :param _ComponentId: 表单域或控件的ID，跟ComponentName二选一，不能全为空；
 CreateFlowsByTemplates 接口不使用此字段。
 注意：此字段可能返回 null，表示取不到有效值。
         :type ComponentId: str
         :param _ComponentName: 控件的名字，跟ComponentId二选一，不能全为空
 注意：此字段可能返回 null，表示取不到有效值。
         :type ComponentName: str
-        :param _LockComponentValue: 是否锁定模版控件值，锁定后无法修改（用于嵌入式发起合同）
+        :param _LockComponentValue: 是否锁定模版控件值，锁定后无法修改（用于嵌入式发起合同），true-锁定，false-不锁定
 注意：此字段可能返回 null，表示取不到有效值。
         :type LockComponentValue: bool
         """
         self._ComponentValue = None
         self._ComponentId = None
         self._ComponentName = None
         self._LockComponentValue = None
@@ -9340,15 +9340,15 @@
         r"""
         :param _AppId: 腾讯电子签颁发给第三方应用平台的应用ID
 注意：此字段可能返回 null，表示取不到有效值。
         :type AppId: str
         :param _TemplateId: 第三方应用平台模板库模板唯一标识
 注意：此字段可能返回 null，表示取不到有效值。
         :type TemplateId: str
-        :param _OperateResult: 描述模版可见性更改的结果，和参数中Available无关，全部成功-"all-success",部分成功-"part-success", 全部失败-"fail"失败的会在FailMessageList中展示。
+        :param _OperateResult: 描述模板可见性更改的结果，和参数中Available无关，全部成功-"all-success",部分成功-"part-success", 全部失败-"fail"失败的会在FailMessageList中展示。
 注意：此字段可能返回 null，表示取不到有效值。
         :type OperateResult: str
         :param _AuthTag: 模板可见性, 全部可见-"all", 部分可见-"part"
 注意：此字段可能返回 null，表示取不到有效值。
         :type AuthTag: str
         :param _ProxyOrganizationOpenIds: 合作企业方第三方机构唯一标识数据
 注意：此字段可能返回 null，表示取不到有效值。
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-essbasic-3.0.934/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.935/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.934
+Version: 3.0.935
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.934/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.935/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.934/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.935/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.934
+Version: 3.0.935
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

