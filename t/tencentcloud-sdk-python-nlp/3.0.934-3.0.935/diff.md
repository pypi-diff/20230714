# Comparing `tmp/tencentcloud-sdk-python-nlp-3.0.934.tar.gz` & `tmp/tencentcloud-sdk-python-nlp-3.0.935.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-nlp-3.0.934.tar", last modified: Thu Jul 13 00:27:00 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-nlp-3.0.935.tar", last modified: Fri Jul 14 00:35:13 2023, max compression
```

## Comparing `tencentcloud-sdk-python-nlp-3.0.934.tar` & `tencentcloud-sdk-python-nlp-3.0.935.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:27:00.000000 tencentcloud-sdk-python-nlp-3.0.934/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-13 00:27:00.000000 tencentcloud-sdk-python-nlp-3.0.934/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:27:00.000000 tencentcloud-sdk-python-nlp-3.0.934/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-13 00:27:00.000000 tencentcloud-sdk-python-nlp-3.0.934/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:27:00.000000 tencentcloud-sdk-python-nlp-3.0.934/tencentcloud/nlp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:27:00.000000 tencentcloud-sdk-python-nlp-3.0.934/tencentcloud/nlp/v20190408/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:27:00.000000 tencentcloud-sdk-python-nlp-3.0.934/tencentcloud/nlp/v20190408/__init__.py
--rw-r--r--   0 root         (0) root         (0)    49107 2023-07-13 00:27:00.000000 tencentcloud-sdk-python-nlp-3.0.934/tencentcloud/nlp/v20190408/nlp_client.py
--rw-r--r--   0 root         (0) root         (0)     6090 2023-07-13 00:27:00.000000 tencentcloud-sdk-python-nlp-3.0.934/tencentcloud/nlp/v20190408/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   134218 2023-07-13 00:27:00.000000 tencentcloud-sdk-python-nlp-3.0.934/tencentcloud/nlp/v20190408/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:27:00.000000 tencentcloud-sdk-python-nlp-3.0.934/tencentcloud/nlp/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-13 00:27:00.000000 tencentcloud-sdk-python-nlp-3.0.934/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:27:00.000000 tencentcloud-sdk-python-nlp-3.0.934/tencentcloud_sdk_python_nlp.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 00:27:00.000000 tencentcloud-sdk-python-nlp-3.0.934/tencentcloud_sdk_python_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-13 00:27:00.000000 tencentcloud-sdk-python-nlp-3.0.934/tencentcloud_sdk_python_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-13 00:27:00.000000 tencentcloud-sdk-python-nlp-3.0.934/tencentcloud_sdk_python_nlp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-13 00:27:00.000000 tencentcloud-sdk-python-nlp-3.0.934/tencentcloud_sdk_python_nlp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-13 00:27:00.000000 tencentcloud-sdk-python-nlp-3.0.934/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-13 00:27:00.000000 tencentcloud-sdk-python-nlp-3.0.934/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:35:13.000000 tencentcloud-sdk-python-nlp-3.0.935/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-14 00:35:13.000000 tencentcloud-sdk-python-nlp-3.0.935/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:35:13.000000 tencentcloud-sdk-python-nlp-3.0.935/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-14 00:35:13.000000 tencentcloud-sdk-python-nlp-3.0.935/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:35:13.000000 tencentcloud-sdk-python-nlp-3.0.935/tencentcloud/nlp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:35:13.000000 tencentcloud-sdk-python-nlp-3.0.935/tencentcloud/nlp/v20190408/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:35:13.000000 tencentcloud-sdk-python-nlp-3.0.935/tencentcloud/nlp/v20190408/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    49107 2023-07-14 00:35:13.000000 tencentcloud-sdk-python-nlp-3.0.935/tencentcloud/nlp/v20190408/nlp_client.py
+-rw-r--r--   0 root         (0) root         (0)     6090 2023-07-14 00:35:13.000000 tencentcloud-sdk-python-nlp-3.0.935/tencentcloud/nlp/v20190408/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   134541 2023-07-14 00:35:13.000000 tencentcloud-sdk-python-nlp-3.0.935/tencentcloud/nlp/v20190408/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:35:13.000000 tencentcloud-sdk-python-nlp-3.0.935/tencentcloud/nlp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-14 00:35:13.000000 tencentcloud-sdk-python-nlp-3.0.935/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:35:13.000000 tencentcloud-sdk-python-nlp-3.0.935/tencentcloud_sdk_python_nlp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 00:35:13.000000 tencentcloud-sdk-python-nlp-3.0.935/tencentcloud_sdk_python_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-14 00:35:13.000000 tencentcloud-sdk-python-nlp-3.0.935/tencentcloud_sdk_python_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 00:35:13.000000 tencentcloud-sdk-python-nlp-3.0.935/tencentcloud_sdk_python_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-14 00:35:13.000000 tencentcloud-sdk-python-nlp-3.0.935/tencentcloud_sdk_python_nlp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 00:35:13.000000 tencentcloud-sdk-python-nlp-3.0.935/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-14 00:35:13.000000 tencentcloud-sdk-python-nlp-3.0.935/README.rst
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.934/setup.py` & `tencentcloud-sdk-python-nlp-3.0.935/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-nlp-3.0.934/tencentcloud/__init__.py` & `tencentcloud-sdk-python-nlp-3.0.935/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-nlp-3.0.934/tencentcloud/nlp/v20190408/nlp_client.py` & `tencentcloud-sdk-python-nlp-3.0.935/tencentcloud/nlp/v20190408/nlp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-nlp-3.0.934/tencentcloud/nlp/v20190408/errorcodes.py` & `tencentcloud-sdk-python-nlp-3.0.935/tencentcloud/nlp/v20190408/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-nlp-3.0.934/tencentcloud/nlp/v20190408/models.py` & `tencentcloud-sdk-python-nlp-3.0.935/tencentcloud/nlp/v20190408/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -704,19 +704,19 @@
 class ClassifyContentResponse(AbstractModel):
     """ClassifyContent返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _FirstClassification: 一级分类。分类详情见附录-三级分类体系表。
+        :param _FirstClassification: 一级分类。（请参见附录[三级分类体系表](https://cloud.tencent.com/document/product/271/94286)）
         :type FirstClassification: :class:`tencentcloud.nlp.v20190408.models.Category`
-        :param _SecondClassification: 二级分类。分类详情见附录-三级分类体系表。
+        :param _SecondClassification: 二级分类。（请参见附录[三级分类体系表](https://cloud.tencent.com/document/product/271/94286)）
         :type SecondClassification: :class:`tencentcloud.nlp.v20190408.models.Category`
-        :param _ThirdClassification: 三级分类。分类详情见附录-三级分类体系表。
+        :param _ThirdClassification: 三级分类。（请参见附录[三级分类体系表](https://cloud.tencent.com/document/product/271/94286)）
 注意：此字段可能返回 null，表示取不到有效值。
         :type ThirdClassification: :class:`tencentcloud.nlp.v20190408.models.Category`
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._FirstClassification = None
         self._SecondClassification = None
@@ -3029,20 +3029,19 @@
 
     """
 
     def __init__(self):
         r"""
         :param _NormalText: 输入文本正则化的结果。（包括对英文文本中的开头和实体进行大写等）
         :type NormalText: str
-        :param _BasicParticiples: 基础粒度分词和词性标注的结果。（词性表请参见附录）
-
+        :param _BasicParticiples: 基础粒度分词和词性标注的结果。（请参见附录[词性表](https://cloud.tencent.com/document/product/271/36460)）
         :type BasicParticiples: list of BasicParticiple
-        :param _CompoundParticiples: 复合粒度分词和词性标注的结果。（词性表请参见附录）
+        :param _CompoundParticiples: 复合粒度分词和词性标注的结果。（请参见附录[词性表](https://cloud.tencent.com/document/product/271/36460)）
         :type CompoundParticiples: list of CompoundParticiple
-        :param _Entities: 实体识别结果。（实体类型数据请参见附录）
+        :param _Entities: 实体识别结果。（请参见附录[实体类型数据](https://cloud.tencent.com/document/product/271/90592)）
 
         :type Entities: list of Entity
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._NormalText = None
         self._BasicParticiples = None
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.934/tencentcloud_sdk_python_nlp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-nlp-3.0.935/tencentcloud_sdk_python_nlp.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-nlp
-Version: 3.0.934
+Version: 3.0.935
 Summary: Tencent Cloud Nlp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.934/PKG-INFO` & `tencentcloud-sdk-python-nlp-3.0.935/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-nlp
-Version: 3.0.934
+Version: 3.0.935
 Summary: Tencent Cloud Nlp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.934/README.rst` & `tencentcloud-sdk-python-nlp-3.0.935/README.rst`

 * *Files identical despite different names*

