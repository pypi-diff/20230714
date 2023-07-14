# Comparing `tmp/tencentcloud-sdk-python-domain-3.0.934.tar.gz` & `tmp/tencentcloud-sdk-python-domain-3.0.935.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-domain-3.0.934.tar", last modified: Thu Jul 13 00:21:00 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-domain-3.0.935.tar", last modified: Fri Jul 14 00:22:32 2023, max compression
```

## Comparing `tencentcloud-sdk-python-domain-3.0.934.tar` & `tencentcloud-sdk-python-domain-3.0.935.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:21:00.000000 tencentcloud-sdk-python-domain-3.0.934/
--rw-r--r--   0 root         (0) root         (0)     1012 2023-07-13 00:21:00.000000 tencentcloud-sdk-python-domain-3.0.934/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:21:00.000000 tencentcloud-sdk-python-domain-3.0.934/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-13 00:21:00.000000 tencentcloud-sdk-python-domain-3.0.934/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:21:00.000000 tencentcloud-sdk-python-domain-3.0.934/tencentcloud/domain/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:21:00.000000 tencentcloud-sdk-python-domain-3.0.934/tencentcloud/domain/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:21:00.000000 tencentcloud-sdk-python-domain-3.0.934/tencentcloud/domain/v20180808/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:21:00.000000 tencentcloud-sdk-python-domain-3.0.934/tencentcloud/domain/v20180808/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8787 2023-07-13 00:21:00.000000 tencentcloud-sdk-python-domain-3.0.934/tencentcloud/domain/v20180808/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    25103 2023-07-13 00:21:00.000000 tencentcloud-sdk-python-domain-3.0.934/tencentcloud/domain/v20180808/domain_client.py
--rw-r--r--   0 root         (0) root         (0)   120145 2023-07-13 00:21:00.000000 tencentcloud-sdk-python-domain-3.0.934/tencentcloud/domain/v20180808/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-13 00:21:00.000000 tencentcloud-sdk-python-domain-3.0.934/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:21:00.000000 tencentcloud-sdk-python-domain-3.0.934/tencentcloud_sdk_python_domain.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 00:21:00.000000 tencentcloud-sdk-python-domain-3.0.934/tencentcloud_sdk_python_domain.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-07-13 00:21:00.000000 tencentcloud-sdk-python-domain-3.0.934/tencentcloud_sdk_python_domain.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-13 00:21:00.000000 tencentcloud-sdk-python-domain-3.0.934/tencentcloud_sdk_python_domain.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-13 00:21:00.000000 tencentcloud-sdk-python-domain-3.0.934/tencentcloud_sdk_python_domain.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-13 00:21:00.000000 tencentcloud-sdk-python-domain-3.0.934/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-07-13 00:21:00.000000 tencentcloud-sdk-python-domain-3.0.934/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:22:32.000000 tencentcloud-sdk-python-domain-3.0.935/
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-07-14 00:22:32.000000 tencentcloud-sdk-python-domain-3.0.935/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:22:32.000000 tencentcloud-sdk-python-domain-3.0.935/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-14 00:22:32.000000 tencentcloud-sdk-python-domain-3.0.935/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:22:32.000000 tencentcloud-sdk-python-domain-3.0.935/tencentcloud/domain/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:22:32.000000 tencentcloud-sdk-python-domain-3.0.935/tencentcloud/domain/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:22:32.000000 tencentcloud-sdk-python-domain-3.0.935/tencentcloud/domain/v20180808/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:22:32.000000 tencentcloud-sdk-python-domain-3.0.935/tencentcloud/domain/v20180808/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8787 2023-07-14 00:22:32.000000 tencentcloud-sdk-python-domain-3.0.935/tencentcloud/domain/v20180808/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    25103 2023-07-14 00:22:32.000000 tencentcloud-sdk-python-domain-3.0.935/tencentcloud/domain/v20180808/domain_client.py
+-rw-r--r--   0 root         (0) root         (0)   121267 2023-07-14 00:22:32.000000 tencentcloud-sdk-python-domain-3.0.935/tencentcloud/domain/v20180808/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-14 00:22:32.000000 tencentcloud-sdk-python-domain-3.0.935/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:22:32.000000 tencentcloud-sdk-python-domain-3.0.935/tencentcloud_sdk_python_domain.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 00:22:32.000000 tencentcloud-sdk-python-domain-3.0.935/tencentcloud_sdk_python_domain.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-07-14 00:22:32.000000 tencentcloud-sdk-python-domain-3.0.935/tencentcloud_sdk_python_domain.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-14 00:22:32.000000 tencentcloud-sdk-python-domain-3.0.935/tencentcloud_sdk_python_domain.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-14 00:22:32.000000 tencentcloud-sdk-python-domain-3.0.935/tencentcloud_sdk_python_domain.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-14 00:22:32.000000 tencentcloud-sdk-python-domain-3.0.935/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-14 00:22:32.000000 tencentcloud-sdk-python-domain-3.0.935/README.rst
```

### Comparing `tencentcloud-sdk-python-domain-3.0.934/setup.py` & `tencentcloud-sdk-python-domain-3.0.935/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-domain-3.0.934/tencentcloud/__init__.py` & `tencentcloud-sdk-python-domain-3.0.935/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-domain-3.0.934/tencentcloud/domain/v20180808/errorcodes.py` & `tencentcloud-sdk-python-domain-3.0.935/tencentcloud/domain/v20180808/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-domain-3.0.934/tencentcloud/domain/v20180808/domain_client.py` & `tencentcloud-sdk-python-domain-3.0.935/tencentcloud/domain/v20180808/domain_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-domain-3.0.934/tencentcloud/domain/v20180808/models.py` & `tencentcloud-sdk-python-domain-3.0.935/tencentcloud/domain/v20180808/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,14 +215,42 @@
         :param _OriginImgUrl: 原始照片地址
 注意：此字段可能返回 null，表示取不到有效值。
         :type OriginImgUrl: str
         :param _RegistrantCertificateCode: 联系人证件号码。
 注意：此字段可能返回 null，表示取不到有效值。
         :type RegistrantCertificateCode: str
         :param _RegistrantCertificateType: 联系人证件类型。
+SFZ: 身份证。
+HZ: 护照。
+TXZ: 中国港澳居民来往内地通行证。
+TWSFZ: 中国台湾居民来往大陆通行证。
+GWSFZ: 外国人永久居留身份证。
+ORG: 组织机构代码证
+YYZZ: 工商营业执照。
+TYDMZ: 统一社会信用代码证书。
+BDDH: 部队代号
+JDXKZ: 军队单位对外有偿服务许可证。
+SYZS: 事业单位法定代表人证书。
+GWCZDJZ: 外国企业常驻代表机构登记证。
+STDJZ: 社会团体法定代表人登记证书。
+ZJDJZ: 宗教活动场所登记证。
+MBDJZ: 民办非企业单位登记证书。
+JJDJZ: 基金会法定代表人登记证书。
+LSXKZ: 律师事务所执业许可证。
+GWZHDJZ: 外国在华文化中心登记证。
+GWLYDJZ: 外国政府旅游部门常驻代表机构批准登记证。
+SFXKZ: 司法鉴定许可证
+GWJGZJ: 外国机构证件。
+SHFWJGZ: 社会服务机构登记证书。
+MBXXXKZ: 民办学校办学许可证。
+YLJGXKZ: 医疗机构执业许可证。
+GAJZZ: 中国港澳居住证。
+TWJZZ: 中国台湾居住证。
+QTTYDM: 其他-统一社会信用代码证书。
+GZJGZY: 公证机构执业证。
 注意：此字段可能返回 null，表示取不到有效值。
         :type RegistrantCertificateType: str
         :param _RegistrantImgUrl: 联系人证件照片地址。
 注意：此字段可能返回 null，表示取不到有效值。
         :type RegistrantImgUrl: str
         """
         self._CertificateCode = None
@@ -1906,15 +1934,15 @@
         r"""
         :param _Type: 0：所有类型  1：手机  2：邮箱，默认0
         :type Type: int
         :param _Offset: 偏移量，默认为0
         :type Offset: int
         :param _Limit: 返回数量，默认为20，取值范围[1,200]
         :type Limit: int
-        :param _Code: 手机或者邮箱精确搜索
+        :param _Code: 手机或者邮箱，用于精确搜索
         :type Code: str
         """
         self._Type = None
         self._Offset = None
         self._Limit = None
         self._Code = None
 
@@ -2031,15 +2059,15 @@
         :type Offset: int
         :param _Limit: 返回数量，默认为20，最大值为100。
         :type Limit: int
         :param _Type: 用户注册类型，默认:all , 个人：I ,企业: E
         :type Type: str
         :param _Status: 认证状态：未实名审核:NotUpload, 实名审核中:InAudit，已实名审核:Approved，实名审核失败:Reject，更新手机邮箱:NotVerified。
         :type Status: str
-        :param _Keyword: 域名所有者筛选
+        :param _Keyword: 关键字，用于域名所有者筛选
         :type Keyword: str
         """
         self._Offset = None
         self._Limit = None
         self._Type = None
         self._Status = None
         self._Keyword = None
```

### Comparing `tencentcloud-sdk-python-domain-3.0.934/tencentcloud_sdk_python_domain.egg-info/PKG-INFO` & `tencentcloud-sdk-python-domain-3.0.935/tencentcloud_sdk_python_domain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-domain
-Version: 3.0.934
+Version: 3.0.935
 Summary: Tencent Cloud Domain SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-domain-3.0.934/PKG-INFO` & `tencentcloud-sdk-python-domain-3.0.935/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-domain
-Version: 3.0.934
+Version: 3.0.935
 Summary: Tencent Cloud Domain SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-domain-3.0.934/README.rst` & `tencentcloud-sdk-python-domain-3.0.935/README.rst`

 * *Files identical despite different names*

