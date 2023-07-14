# Comparing `tmp/tencentcloud-sdk-python-region-3.0.934.tar.gz` & `tmp/tencentcloud-sdk-python-region-3.0.935.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-region-3.0.934.tar", last modified: Thu Jul 13 00:31:28 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-region-3.0.935.tar", last modified: Fri Jul 14 00:36:26 2023, max compression
```

## Comparing `tencentcloud-sdk-python-region-3.0.934.tar` & `tencentcloud-sdk-python-region-3.0.935.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:31:28.000000 tencentcloud-sdk-python-region-3.0.934/
--rw-r--r--   0 root         (0) root         (0)     1012 2023-07-13 00:31:28.000000 tencentcloud-sdk-python-region-3.0.934/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:31:28.000000 tencentcloud-sdk-python-region-3.0.934/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-13 00:31:28.000000 tencentcloud-sdk-python-region-3.0.934/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:31:28.000000 tencentcloud-sdk-python-region-3.0.934/tencentcloud/region/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:31:28.000000 tencentcloud-sdk-python-region-3.0.934/tencentcloud/region/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:31:28.000000 tencentcloud-sdk-python-region-3.0.934/tencentcloud/region/v20220627/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:31:28.000000 tencentcloud-sdk-python-region-3.0.934/tencentcloud/region/v20220627/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3744 2023-07-13 00:31:28.000000 tencentcloud-sdk-python-region-3.0.934/tencentcloud/region/v20220627/region_client.py
--rw-r--r--   0 root         (0) root         (0)      866 2023-07-13 00:31:28.000000 tencentcloud-sdk-python-region-3.0.934/tencentcloud/region/v20220627/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    18296 2023-07-13 00:31:28.000000 tencentcloud-sdk-python-region-3.0.934/tencentcloud/region/v20220627/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-13 00:31:28.000000 tencentcloud-sdk-python-region-3.0.934/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:31:28.000000 tencentcloud-sdk-python-region-3.0.934/tencentcloud_sdk_python_region.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 00:31:28.000000 tencentcloud-sdk-python-region-3.0.934/tencentcloud_sdk_python_region.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-07-13 00:31:28.000000 tencentcloud-sdk-python-region-3.0.934/tencentcloud_sdk_python_region.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-13 00:31:28.000000 tencentcloud-sdk-python-region-3.0.934/tencentcloud_sdk_python_region.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-13 00:31:28.000000 tencentcloud-sdk-python-region-3.0.934/tencentcloud_sdk_python_region.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-13 00:31:28.000000 tencentcloud-sdk-python-region-3.0.934/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-07-13 00:31:28.000000 tencentcloud-sdk-python-region-3.0.934/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:36:26.000000 tencentcloud-sdk-python-region-3.0.935/
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-07-14 00:36:26.000000 tencentcloud-sdk-python-region-3.0.935/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:36:26.000000 tencentcloud-sdk-python-region-3.0.935/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-14 00:36:26.000000 tencentcloud-sdk-python-region-3.0.935/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:36:26.000000 tencentcloud-sdk-python-region-3.0.935/tencentcloud/region/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:36:26.000000 tencentcloud-sdk-python-region-3.0.935/tencentcloud/region/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:36:26.000000 tencentcloud-sdk-python-region-3.0.935/tencentcloud/region/v20220627/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:36:26.000000 tencentcloud-sdk-python-region-3.0.935/tencentcloud/region/v20220627/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3744 2023-07-14 00:36:26.000000 tencentcloud-sdk-python-region-3.0.935/tencentcloud/region/v20220627/region_client.py
+-rw-r--r--   0 root         (0) root         (0)      866 2023-07-14 00:36:26.000000 tencentcloud-sdk-python-region-3.0.935/tencentcloud/region/v20220627/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    18296 2023-07-14 00:36:26.000000 tencentcloud-sdk-python-region-3.0.935/tencentcloud/region/v20220627/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-14 00:36:26.000000 tencentcloud-sdk-python-region-3.0.935/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:36:26.000000 tencentcloud-sdk-python-region-3.0.935/tencentcloud_sdk_python_region.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 00:36:26.000000 tencentcloud-sdk-python-region-3.0.935/tencentcloud_sdk_python_region.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-07-14 00:36:26.000000 tencentcloud-sdk-python-region-3.0.935/tencentcloud_sdk_python_region.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-14 00:36:26.000000 tencentcloud-sdk-python-region-3.0.935/tencentcloud_sdk_python_region.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-14 00:36:26.000000 tencentcloud-sdk-python-region-3.0.935/tencentcloud_sdk_python_region.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-14 00:36:26.000000 tencentcloud-sdk-python-region-3.0.935/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-14 00:36:26.000000 tencentcloud-sdk-python-region-3.0.935/README.rst
```

### Comparing `tencentcloud-sdk-python-region-3.0.934/setup.py` & `tencentcloud-sdk-python-region-3.0.935/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-region-3.0.934/tencentcloud/__init__.py` & `tencentcloud-sdk-python-region-3.0.935/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-region-3.0.934/tencentcloud/region/v20220627/region_client.py` & `tencentcloud-sdk-python-region-3.0.935/tencentcloud/region/v20220627/region_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-region-3.0.934/tencentcloud/region/v20220627/errorcodes.py` & `tencentcloud-sdk-python-region-3.0.935/tencentcloud/region/v20220627/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-region-3.0.934/tencentcloud/region/v20220627/models.py` & `tencentcloud-sdk-python-region-3.0.935/tencentcloud/region/v20220627/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-region-3.0.934/tencentcloud_sdk_python_region.egg-info/PKG-INFO` & `tencentcloud-sdk-python-region-3.0.935/tencentcloud_sdk_python_region.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-region
-Version: 3.0.934
+Version: 3.0.935
 Summary: Tencent Cloud Region SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-region-3.0.934/PKG-INFO` & `tencentcloud-sdk-python-region-3.0.935/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-region
-Version: 3.0.934
+Version: 3.0.935
 Summary: Tencent Cloud Region SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-region-3.0.934/README.rst` & `tencentcloud-sdk-python-region-3.0.935/README.rst`

 * *Files identical despite different names*

