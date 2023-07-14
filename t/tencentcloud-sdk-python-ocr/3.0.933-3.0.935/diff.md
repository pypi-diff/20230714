# Comparing `tmp/tencentcloud-sdk-python-ocr-3.0.933.tar.gz` & `tmp/tencentcloud-sdk-python-ocr-3.0.935.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.933.tar", last modified: Wed Jul 12 00:34:40 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.935.tar", last modified: Fri Jul 14 00:35:28 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ocr-3.0.933.tar` & `tencentcloud-sdk-python-ocr-3.0.935.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:34:40.000000 tencentcloud-sdk-python-ocr-3.0.933/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-12 00:34:40.000000 tencentcloud-sdk-python-ocr-3.0.933/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:34:40.000000 tencentcloud-sdk-python-ocr-3.0.933/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-12 00:34:40.000000 tencentcloud-sdk-python-ocr-3.0.933/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:34:40.000000 tencentcloud-sdk-python-ocr-3.0.933/tencentcloud/ocr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:34:40.000000 tencentcloud-sdk-python-ocr-3.0.933/tencentcloud/ocr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:34:40.000000 tencentcloud-sdk-python-ocr-3.0.933/tencentcloud/ocr/v20181119/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:34:40.000000 tencentcloud-sdk-python-ocr-3.0.933/tencentcloud/ocr/v20181119/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5894 2023-07-12 00:34:40.000000 tencentcloud-sdk-python-ocr-3.0.933/tencentcloud/ocr/v20181119/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   115258 2023-07-12 00:34:40.000000 tencentcloud-sdk-python-ocr-3.0.933/tencentcloud/ocr/v20181119/ocr_client.py
--rw-r--r--   0 root         (0) root         (0)   816358 2023-07-12 00:34:40.000000 tencentcloud-sdk-python-ocr-3.0.933/tencentcloud/ocr/v20181119/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:34:40.000000 tencentcloud-sdk-python-ocr-3.0.933/tencentcloud_sdk_python_ocr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 00:34:40.000000 tencentcloud-sdk-python-ocr-3.0.933/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-12 00:34:40.000000 tencentcloud-sdk-python-ocr-3.0.933/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-12 00:34:40.000000 tencentcloud-sdk-python-ocr-3.0.933/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-12 00:34:40.000000 tencentcloud-sdk-python-ocr-3.0.933/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-12 00:34:40.000000 tencentcloud-sdk-python-ocr-3.0.933/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-12 00:34:40.000000 tencentcloud-sdk-python-ocr-3.0.933/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-12 00:34:40.000000 tencentcloud-sdk-python-ocr-3.0.933/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:35:28.000000 tencentcloud-sdk-python-ocr-3.0.935/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-14 00:35:28.000000 tencentcloud-sdk-python-ocr-3.0.935/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:35:28.000000 tencentcloud-sdk-python-ocr-3.0.935/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-14 00:35:28.000000 tencentcloud-sdk-python-ocr-3.0.935/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:35:28.000000 tencentcloud-sdk-python-ocr-3.0.935/tencentcloud/ocr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:35:28.000000 tencentcloud-sdk-python-ocr-3.0.935/tencentcloud/ocr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:35:28.000000 tencentcloud-sdk-python-ocr-3.0.935/tencentcloud/ocr/v20181119/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:35:28.000000 tencentcloud-sdk-python-ocr-3.0.935/tencentcloud/ocr/v20181119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5894 2023-07-14 00:35:28.000000 tencentcloud-sdk-python-ocr-3.0.935/tencentcloud/ocr/v20181119/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   115238 2023-07-14 00:35:28.000000 tencentcloud-sdk-python-ocr-3.0.935/tencentcloud/ocr/v20181119/ocr_client.py
+-rw-r--r--   0 root         (0) root         (0)   816278 2023-07-14 00:35:28.000000 tencentcloud-sdk-python-ocr-3.0.935/tencentcloud/ocr/v20181119/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:35:28.000000 tencentcloud-sdk-python-ocr-3.0.935/tencentcloud_sdk_python_ocr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 00:35:28.000000 tencentcloud-sdk-python-ocr-3.0.935/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-14 00:35:28.000000 tencentcloud-sdk-python-ocr-3.0.935/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 00:35:28.000000 tencentcloud-sdk-python-ocr-3.0.935/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-14 00:35:28.000000 tencentcloud-sdk-python-ocr-3.0.935/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-14 00:35:28.000000 tencentcloud-sdk-python-ocr-3.0.935/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 00:35:28.000000 tencentcloud-sdk-python-ocr-3.0.935/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-14 00:35:28.000000 tencentcloud-sdk-python-ocr-3.0.935/README.rst
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.933/setup.py` & `tencentcloud-sdk-python-ocr-3.0.935/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.933/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ocr-3.0.935/tencentcloud/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.933'
+__version__ = '3.0.935'
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.933/tencentcloud/ocr/v20181119/errorcodes.py` & `tencentcloud-sdk-python-ocr-3.0.935/tencentcloud/ocr/v20181119/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.933/tencentcloud/ocr/v20181119/ocr_client.py` & `tencentcloud-sdk-python-ocr-3.0.935/tencentcloud/ocr/v20181119/ocr_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -860,15 +860,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def HKIDCardOCR(self, request):
-        """本接口支持中国香港身份证人像面中关键字段的识别，包括中文姓名、英文姓名、姓名电码、出生日期、性别、证件符号、首次签发日期、最近领用日期、身份证号、是否是永久性居民身份证；具备防伪识别、人像照片裁剪等扩展功能。
+        """本接口支持中国香港身份证人像面中关键字段的识别，包括中文姓名、英文姓名、姓名电码、出生日期、性别、证件符号、首次签发日期、最近领用日期、身份证号、是否是永久性居民身份证；具备人像照片裁剪等扩展功能。
 
         默认接口请求频率限制：5次/秒。
 
         :param request: Request instance for HKIDCardOCR.
         :type request: :class:`tencentcloud.ocr.v20181119.models.HKIDCardOCRRequest`
         :rtype: :class:`tencentcloud.ocr.v20181119.models.HKIDCardOCRResponse`
 
@@ -2313,15 +2313,15 @@
     def VehicleLicenseOCR(self, request):
         """本接口支持行驶证主页和副页所有字段的自动定位与识别。
 
         行驶证主页：车牌号码、车辆类型、所有人、住址、使用性质、品牌型号、识别代码、发动机号、注册日期、发证日期、发证单位。
 
         行驶证副页：号牌号码、档案编号、核定载人数、总质量、整备质量、核定载质量、外廓尺寸、准牵引总质量、备注、检验记录。
 
-        另外，本接口还支持复印件、翻拍和PS告警功能。
+        另外，本接口还支持复印件、翻拍告警功能。
 
         默认接口请求频率限制：10次/秒。
 
         :param request: Request instance for VehicleLicenseOCR.
         :type request: :class:`tencentcloud.ocr.v20181119.models.VehicleLicenseOCRRequest`
         :rtype: :class:`tencentcloud.ocr.v20181119.models.VehicleLicenseOCRResponse`
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.933/tencentcloud/ocr/v20181119/models.py` & `tencentcloud-sdk-python-ocr-3.0.935/tencentcloud/ocr/v20181119/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5837,18 +5837,17 @@
 1：假；
 2：真。
 注意：此字段可能返回 null，表示取不到有效值。
         :type FakeDetectResult: int
         :param _HeadImage: 人像照片Base64后的结果
 注意：此字段可能返回 null，表示取不到有效值。
         :type HeadImage: str
-        :param _WarningCode: 多重告警码，当身份证是翻拍、复印、PS件时返回对应告警码。
+        :param _WarningCode: 多重告警码，当身份证是翻拍、复印件时返回对应告警码。
 -9102：证照复印件告警
 -9103：证照翻拍告警
--9104：证照PS告警
         :type WarningCode: list of int
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._CnName = None
         self._EnName = None
         self._TelexCode = None
@@ -25206,21 +25205,19 @@
         :type FrontInfo: :class:`tencentcloud.ocr.v20181119.models.TextVehicleFront`
         :param _BackInfo: 行驶证副页正面的识别结果，CardSide 为 BACK。
 注意：此字段可能返回 null，表示取不到有效值。
         :type BackInfo: :class:`tencentcloud.ocr.v20181119.models.TextVehicleBack`
         :param _RecognizeWarnCode: Code 告警码列表和释义：
 -9102 复印件告警
 -9103 翻拍件告警
--9106 ps告警
 注：告警码可以同时存在多个
         :type RecognizeWarnCode: list of int
         :param _RecognizeWarnMsg: 告警码说明：
 WARN_DRIVER_LICENSE_COPY_CARD 复印件告警
 WARN_DRIVER_LICENSE_SCREENED_CARD 翻拍件告警
-WARN_DRIVER_LICENSE_PS_CARD ps告警
 注：告警信息可以同时存在多个
         :type RecognizeWarnMsg: list of str
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._FrontInfo = None
         self._BackInfo = None
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.933/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.935/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.933
+Version: 3.0.935
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.933/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.935/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.933
+Version: 3.0.935
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.933/README.rst` & `tencentcloud-sdk-python-ocr-3.0.935/README.rst`

 * *Files identical despite different names*

