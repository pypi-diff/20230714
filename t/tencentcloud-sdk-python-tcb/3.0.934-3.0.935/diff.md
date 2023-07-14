# Comparing `tmp/tencentcloud-sdk-python-tcb-3.0.934.tar.gz` & `tmp/tencentcloud-sdk-python-tcb-3.0.935.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tcb-3.0.934.tar", last modified: Thu Jul 13 00:33:51 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tcb-3.0.935.tar", last modified: Fri Jul 14 00:38:55 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tcb-3.0.934.tar` & `tencentcloud-sdk-python-tcb-3.0.935.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:33:51.000000 tencentcloud-sdk-python-tcb-3.0.934/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-13 00:33:51.000000 tencentcloud-sdk-python-tcb-3.0.934/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:33:51.000000 tencentcloud-sdk-python-tcb-3.0.934/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-13 00:33:51.000000 tencentcloud-sdk-python-tcb-3.0.934/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:33:51.000000 tencentcloud-sdk-python-tcb-3.0.934/tencentcloud/tcb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:33:51.000000 tencentcloud-sdk-python-tcb-3.0.934/tencentcloud/tcb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:33:51.000000 tencentcloud-sdk-python-tcb-3.0.934/tencentcloud/tcb/v20180608/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:33:51.000000 tencentcloud-sdk-python-tcb-3.0.934/tencentcloud/tcb/v20180608/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4156 2023-07-13 00:33:51.000000 tencentcloud-sdk-python-tcb-3.0.934/tencentcloud/tcb/v20180608/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    83901 2023-07-13 00:33:51.000000 tencentcloud-sdk-python-tcb-3.0.934/tencentcloud/tcb/v20180608/tcb_client.py
--rw-r--r--   0 root         (0) root         (0)   549856 2023-07-13 00:33:51.000000 tencentcloud-sdk-python-tcb-3.0.934/tencentcloud/tcb/v20180608/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-13 00:33:51.000000 tencentcloud-sdk-python-tcb-3.0.934/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:33:51.000000 tencentcloud-sdk-python-tcb-3.0.934/tencentcloud_sdk_python_tcb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 00:33:51.000000 tencentcloud-sdk-python-tcb-3.0.934/tencentcloud_sdk_python_tcb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-13 00:33:51.000000 tencentcloud-sdk-python-tcb-3.0.934/tencentcloud_sdk_python_tcb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-13 00:33:51.000000 tencentcloud-sdk-python-tcb-3.0.934/tencentcloud_sdk_python_tcb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-13 00:33:51.000000 tencentcloud-sdk-python-tcb-3.0.934/tencentcloud_sdk_python_tcb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-13 00:33:51.000000 tencentcloud-sdk-python-tcb-3.0.934/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-13 00:33:51.000000 tencentcloud-sdk-python-tcb-3.0.934/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:38:55.000000 tencentcloud-sdk-python-tcb-3.0.935/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-14 00:38:54.000000 tencentcloud-sdk-python-tcb-3.0.935/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:38:55.000000 tencentcloud-sdk-python-tcb-3.0.935/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-14 00:38:54.000000 tencentcloud-sdk-python-tcb-3.0.935/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:38:55.000000 tencentcloud-sdk-python-tcb-3.0.935/tencentcloud/tcb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:38:54.000000 tencentcloud-sdk-python-tcb-3.0.935/tencentcloud/tcb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:38:55.000000 tencentcloud-sdk-python-tcb-3.0.935/tencentcloud/tcb/v20180608/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:38:54.000000 tencentcloud-sdk-python-tcb-3.0.935/tencentcloud/tcb/v20180608/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4156 2023-07-14 00:38:54.000000 tencentcloud-sdk-python-tcb-3.0.935/tencentcloud/tcb/v20180608/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    83901 2023-07-14 00:38:54.000000 tencentcloud-sdk-python-tcb-3.0.935/tencentcloud/tcb/v20180608/tcb_client.py
+-rw-r--r--   0 root         (0) root         (0)   549868 2023-07-14 00:38:54.000000 tencentcloud-sdk-python-tcb-3.0.935/tencentcloud/tcb/v20180608/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-14 00:38:55.000000 tencentcloud-sdk-python-tcb-3.0.935/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:38:55.000000 tencentcloud-sdk-python-tcb-3.0.935/tencentcloud_sdk_python_tcb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 00:38:55.000000 tencentcloud-sdk-python-tcb-3.0.935/tencentcloud_sdk_python_tcb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-14 00:38:55.000000 tencentcloud-sdk-python-tcb-3.0.935/tencentcloud_sdk_python_tcb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 00:38:55.000000 tencentcloud-sdk-python-tcb-3.0.935/tencentcloud_sdk_python_tcb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-14 00:38:55.000000 tencentcloud-sdk-python-tcb-3.0.935/tencentcloud_sdk_python_tcb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 00:38:55.000000 tencentcloud-sdk-python-tcb-3.0.935/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-14 00:38:54.000000 tencentcloud-sdk-python-tcb-3.0.935/README.rst
```

### Comparing `tencentcloud-sdk-python-tcb-3.0.934/setup.py` & `tencentcloud-sdk-python-tcb-3.0.935/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcb-3.0.934/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tcb-3.0.935/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tcb-3.0.934/tencentcloud/tcb/v20180608/errorcodes.py` & `tencentcloud-sdk-python-tcb-3.0.935/tencentcloud/tcb/v20180608/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcb-3.0.934/tencentcloud/tcb/v20180608/tcb_client.py` & `tencentcloud-sdk-python-tcb-3.0.935/tencentcloud/tcb/v20180608/tcb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcb-3.0.934/tencentcloud/tcb/v20180608/models.py` & `tencentcloud-sdk-python-tcb-3.0.935/tencentcloud/tcb/v20180608/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -8862,17 +8862,17 @@
         :param _DockerfilePath: Dockefile的路径
 注意：此字段可能返回 null，表示取不到有效值。
         :type DockerfilePath: str
         :param _BuildDir: DockerBuild的目录
 注意：此字段可能返回 null，表示取不到有效值。
         :type BuildDir: str
         :param _Cpu: 请使用CPUSize
-        :type Cpu: int
+        :type Cpu: float
         :param _Mem: 请使用MemSize
-        :type Mem: int
+        :type Mem: float
         :param _MinNum: 副本最小值
         :type MinNum: int
         :param _MaxNum: 副本最大值
         :type MaxNum: int
         :param _PolicyType: 策略类型
         :type PolicyType: str
         :param _PolicyThreshold: 策略阈值
@@ -10174,15 +10174,15 @@
         :param _Period: 统计周期(单位秒), 当时间区间为1天内, 统计周期为5分钟; 当时间区间选择为1天以上, 15天以下, 统计周期为1小时; 当时间区间选择为15天以上, 180天以下, 统计周期为1天.
         :type Period: int
         :param _Values: 有效的监控数据, 每个有效监控数据的上报时间可以从时间数组中的对应位置上获取到.
         :type Values: list of int
         :param _Time: 时间数据, 标识监控数据Values中的点是哪个时间段上报的.
         :type Time: list of int
         :param _NewValues: 有效的监控数据, 每个有效监控数据的上报时间可以从时间数组中的对应位置上获取到.
-        :type NewValues: float
+        :type NewValues: list of float
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._StartTime = None
         self._EndTime = None
         self._MetricName = None
         self._Period = None
```

### Comparing `tencentcloud-sdk-python-tcb-3.0.934/tencentcloud_sdk_python_tcb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tcb-3.0.935/tencentcloud_sdk_python_tcb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcb
-Version: 3.0.934
+Version: 3.0.935
 Summary: Tencent Cloud Tcb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcb-3.0.934/PKG-INFO` & `tencentcloud-sdk-python-tcb-3.0.935/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcb
-Version: 3.0.934
+Version: 3.0.935
 Summary: Tencent Cloud Tcb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcb-3.0.934/README.rst` & `tencentcloud-sdk-python-tcb-3.0.935/README.rst`

 * *Files identical despite different names*

