# Comparing `tmp/tencentcloud-sdk-python-asr-3.0.934.tar.gz` & `tmp/tencentcloud-sdk-python-asr-3.0.935.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-asr-3.0.934.tar", last modified: Thu Jul 13 00:15:04 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-asr-3.0.935.tar", last modified: Fri Jul 14 00:16:40 2023, max compression
```

## Comparing `tencentcloud-sdk-python-asr-3.0.934.tar` & `tencentcloud-sdk-python-asr-3.0.935.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:15:04.000000 tencentcloud-sdk-python-asr-3.0.934/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-13 00:15:04.000000 tencentcloud-sdk-python-asr-3.0.934/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:15:04.000000 tencentcloud-sdk-python-asr-3.0.934/tencentcloud_sdk_python_asr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 00:15:04.000000 tencentcloud-sdk-python-asr-3.0.934/tencentcloud_sdk_python_asr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-13 00:15:04.000000 tencentcloud-sdk-python-asr-3.0.934/tencentcloud_sdk_python_asr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-13 00:15:04.000000 tencentcloud-sdk-python-asr-3.0.934/tencentcloud_sdk_python_asr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-13 00:15:04.000000 tencentcloud-sdk-python-asr-3.0.934/tencentcloud_sdk_python_asr.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:15:04.000000 tencentcloud-sdk-python-asr-3.0.934/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:15:04.000000 tencentcloud-sdk-python-asr-3.0.934/tencentcloud/asr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:15:04.000000 tencentcloud-sdk-python-asr-3.0.934/tencentcloud/asr/v20190614/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:15:04.000000 tencentcloud-sdk-python-asr-3.0.934/tencentcloud/asr/v20190614/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29291 2023-07-13 00:15:04.000000 tencentcloud-sdk-python-asr-3.0.934/tencentcloud/asr/v20190614/asr_client.py
--rw-r--r--   0 root         (0) root         (0)     7371 2023-07-13 00:15:04.000000 tencentcloud-sdk-python-asr-3.0.934/tencentcloud/asr/v20190614/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   110887 2023-07-13 00:15:04.000000 tencentcloud-sdk-python-asr-3.0.934/tencentcloud/asr/v20190614/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:15:04.000000 tencentcloud-sdk-python-asr-3.0.934/tencentcloud/asr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-13 00:15:04.000000 tencentcloud-sdk-python-asr-3.0.934/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-13 00:15:04.000000 tencentcloud-sdk-python-asr-3.0.934/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-13 00:15:04.000000 tencentcloud-sdk-python-asr-3.0.934/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-13 00:15:04.000000 tencentcloud-sdk-python-asr-3.0.934/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:16:40.000000 tencentcloud-sdk-python-asr-3.0.935/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-14 00:16:40.000000 tencentcloud-sdk-python-asr-3.0.935/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:16:40.000000 tencentcloud-sdk-python-asr-3.0.935/tencentcloud_sdk_python_asr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 00:16:40.000000 tencentcloud-sdk-python-asr-3.0.935/tencentcloud_sdk_python_asr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-14 00:16:40.000000 tencentcloud-sdk-python-asr-3.0.935/tencentcloud_sdk_python_asr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 00:16:40.000000 tencentcloud-sdk-python-asr-3.0.935/tencentcloud_sdk_python_asr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-14 00:16:40.000000 tencentcloud-sdk-python-asr-3.0.935/tencentcloud_sdk_python_asr.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:16:40.000000 tencentcloud-sdk-python-asr-3.0.935/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:16:40.000000 tencentcloud-sdk-python-asr-3.0.935/tencentcloud/asr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:16:40.000000 tencentcloud-sdk-python-asr-3.0.935/tencentcloud/asr/v20190614/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:16:40.000000 tencentcloud-sdk-python-asr-3.0.935/tencentcloud/asr/v20190614/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29291 2023-07-14 00:16:40.000000 tencentcloud-sdk-python-asr-3.0.935/tencentcloud/asr/v20190614/asr_client.py
+-rw-r--r--   0 root         (0) root         (0)     7371 2023-07-14 00:16:40.000000 tencentcloud-sdk-python-asr-3.0.935/tencentcloud/asr/v20190614/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   110960 2023-07-14 00:16:40.000000 tencentcloud-sdk-python-asr-3.0.935/tencentcloud/asr/v20190614/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:16:40.000000 tencentcloud-sdk-python-asr-3.0.935/tencentcloud/asr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-14 00:16:40.000000 tencentcloud-sdk-python-asr-3.0.935/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-14 00:16:40.000000 tencentcloud-sdk-python-asr-3.0.935/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 00:16:40.000000 tencentcloud-sdk-python-asr-3.0.935/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-14 00:16:40.000000 tencentcloud-sdk-python-asr-3.0.935/README.rst
```

### Comparing `tencentcloud-sdk-python-asr-3.0.934/setup.py` & `tencentcloud-sdk-python-asr-3.0.935/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.934/tencentcloud_sdk_python_asr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-asr-3.0.935/tencentcloud_sdk_python_asr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-asr
-Version: 3.0.934
+Version: 3.0.935
 Summary: Tencent Cloud Asr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-asr-3.0.934/tencentcloud/asr/v20190614/asr_client.py` & `tencentcloud-sdk-python-asr-3.0.935/tencentcloud/asr/v20190614/asr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.934/tencentcloud/asr/v20190614/errorcodes.py` & `tencentcloud-sdk-python-asr-3.0.935/tencentcloud/asr/v20190614/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.934/tencentcloud/asr/v20190614/models.py` & `tencentcloud-sdk-python-asr-3.0.935/tencentcloud/asr/v20190614/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -605,15 +605,15 @@
 • 16k_th：泰语；
 • 16k_pt：葡萄牙语；
 • 16k_tr：土耳其语；
 • 16k_zh_dialect：多方言，支持23种方言（上海话、四川话、武汉话、贵阳话、昆明话、西安话、郑州话、太原话、兰州话、银川话、西宁话、南京话、合肥话、南昌话、长沙话、苏州话、杭州话、济南话、天津话、石家庄话、黑龙江话、吉林话、辽宁话）；
         :type EngineModelType: str
         :param _ChannelNum: 识别声道数。1：单声道（非电话场景，直接选择单声道即可，忽略音频声道数）；2：双声道（仅支持8k_zh电话场景，双声道应分别对应通话双方）。注意：双声道的电话音频已物理分离说话人，无需再开启说话人分离功能。
         :type ChannelNum: int
-        :param _ResTextFormat: 识别结果返回形式。0： 识别结果文本(含分段时间戳)； 1：词级别粒度的[详细识别结果](https://cloud.tencent.com/document/api/1093/37824#SentenceDetail)(不含标点，含语速值)；2：词级别粒度的详细识别结果（包含标点、语速值）；3: 标点符号分段，包含每段时间戳，特别适用于字幕场景（包含词级时间、标点、语速值）。4：【付费功能】将对ASR结果按照语义分段，并展示词级别粒度的详细识别结果,目前仅支持中文引擎（注意：如果开启后付费，将[自动计费](https://cloud.tencent.com/document/product/1093/35686)）
+        :param _ResTextFormat: 识别结果返回形式。0： 识别结果文本(含分段时间戳)； 1：词级别粒度的[详细识别结果](https://cloud.tencent.com/document/api/1093/37824#SentenceDetail)(不含标点，含语速值)；2：词级别粒度的详细识别结果（包含标点、语速值）；3: 标点符号分段，包含每段时间戳，特别适用于字幕场景（包含词级时间、标点、语速值）。4：【增值付费功能】对识别结果按照语义分段，并展示词级别粒度的详细识别结果，仅支持8k_zh、16k_zh引擎，需购买对应资源包使用（注意：如果账号后付费功能开启并使用此功能，将[自动计费](https://cloud.tencent.com/document/product/1093/35686)）
         :type ResTextFormat: int
         :param _SourceType: 语音数据来源。0：语音 URL；1：语音数据（post body）。
         :type SourceType: int
         :param _SpeakerDiarization: 是否开启说话人分离，0：不开启，1：开启(仅支持8k_zh/16k_zh，ChannelNum=1时可用)，默认值为 0。
 注意：8k电话场景建议使用双声道来区分通话双方，设置ChannelNum=2即可，不用开启说话人分离，如果设置了ChannelNum=1，后台会先转码成单声道，说话人分离结果可能产生偏差。
         :type SpeakerDiarization: int
         :param _SpeakerNumber: 说话人分离人数（需配合开启说话人分离使用），取值范围：0-10，0代表自动分离（目前仅支持≤6个人），1-10代表指定说话人数分离。默认值为 0。
```

### Comparing `tencentcloud-sdk-python-asr-3.0.934/tencentcloud/__init__.py` & `tencentcloud-sdk-python-asr-3.0.935/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-asr-3.0.934/PKG-INFO` & `tencentcloud-sdk-python-asr-3.0.935/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-asr
-Version: 3.0.934
+Version: 3.0.935
 Summary: Tencent Cloud Asr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-asr-3.0.934/README.rst` & `tencentcloud-sdk-python-asr-3.0.935/README.rst`

 * *Files identical despite different names*

