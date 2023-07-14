# Comparing `tmp/tencentcloud-sdk-python-cfs-3.0.934.tar.gz` & `tmp/tencentcloud-sdk-python-cfs-3.0.935.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cfs-3.0.934.tar", last modified: Thu Jul 13 00:17:51 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cfs-3.0.935.tar", last modified: Fri Jul 14 00:19:24 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cfs-3.0.934.tar` & `tencentcloud-sdk-python-cfs-3.0.935.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:17:51.000000 tencentcloud-sdk-python-cfs-3.0.934/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-13 00:17:51.000000 tencentcloud-sdk-python-cfs-3.0.934/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:17:51.000000 tencentcloud-sdk-python-cfs-3.0.934/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-13 00:17:51.000000 tencentcloud-sdk-python-cfs-3.0.934/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:17:51.000000 tencentcloud-sdk-python-cfs-3.0.934/tencentcloud/cfs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:17:51.000000 tencentcloud-sdk-python-cfs-3.0.934/tencentcloud/cfs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:17:51.000000 tencentcloud-sdk-python-cfs-3.0.934/tencentcloud/cfs/v20190719/
--rw-r--r--   0 root         (0) root         (0)    39796 2023-07-13 00:17:51.000000 tencentcloud-sdk-python-cfs-3.0.934/tencentcloud/cfs/v20190719/cfs_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:17:51.000000 tencentcloud-sdk-python-cfs-3.0.934/tencentcloud/cfs/v20190719/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15890 2023-07-13 00:17:51.000000 tencentcloud-sdk-python-cfs-3.0.934/tencentcloud/cfs/v20190719/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   193136 2023-07-13 00:17:51.000000 tencentcloud-sdk-python-cfs-3.0.934/tencentcloud/cfs/v20190719/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-13 00:17:51.000000 tencentcloud-sdk-python-cfs-3.0.934/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:17:51.000000 tencentcloud-sdk-python-cfs-3.0.934/tencentcloud_sdk_python_cfs.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 00:17:51.000000 tencentcloud-sdk-python-cfs-3.0.934/tencentcloud_sdk_python_cfs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-13 00:17:51.000000 tencentcloud-sdk-python-cfs-3.0.934/tencentcloud_sdk_python_cfs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-13 00:17:51.000000 tencentcloud-sdk-python-cfs-3.0.934/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-13 00:17:51.000000 tencentcloud-sdk-python-cfs-3.0.934/tencentcloud_sdk_python_cfs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-13 00:17:51.000000 tencentcloud-sdk-python-cfs-3.0.934/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-13 00:17:51.000000 tencentcloud-sdk-python-cfs-3.0.934/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:19:24.000000 tencentcloud-sdk-python-cfs-3.0.935/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-14 00:19:24.000000 tencentcloud-sdk-python-cfs-3.0.935/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:19:24.000000 tencentcloud-sdk-python-cfs-3.0.935/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-14 00:19:24.000000 tencentcloud-sdk-python-cfs-3.0.935/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:19:24.000000 tencentcloud-sdk-python-cfs-3.0.935/tencentcloud/cfs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:19:24.000000 tencentcloud-sdk-python-cfs-3.0.935/tencentcloud/cfs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:19:24.000000 tencentcloud-sdk-python-cfs-3.0.935/tencentcloud/cfs/v20190719/
+-rw-r--r--   0 root         (0) root         (0)    39879 2023-07-14 00:19:24.000000 tencentcloud-sdk-python-cfs-3.0.935/tencentcloud/cfs/v20190719/cfs_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:19:24.000000 tencentcloud-sdk-python-cfs-3.0.935/tencentcloud/cfs/v20190719/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15890 2023-07-14 00:19:24.000000 tencentcloud-sdk-python-cfs-3.0.935/tencentcloud/cfs/v20190719/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   194257 2023-07-14 00:19:24.000000 tencentcloud-sdk-python-cfs-3.0.935/tencentcloud/cfs/v20190719/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-14 00:19:24.000000 tencentcloud-sdk-python-cfs-3.0.935/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:19:24.000000 tencentcloud-sdk-python-cfs-3.0.935/tencentcloud_sdk_python_cfs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 00:19:24.000000 tencentcloud-sdk-python-cfs-3.0.935/tencentcloud_sdk_python_cfs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-14 00:19:24.000000 tencentcloud-sdk-python-cfs-3.0.935/tencentcloud_sdk_python_cfs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 00:19:24.000000 tencentcloud-sdk-python-cfs-3.0.935/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-14 00:19:24.000000 tencentcloud-sdk-python-cfs-3.0.935/tencentcloud_sdk_python_cfs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 00:19:24.000000 tencentcloud-sdk-python-cfs-3.0.935/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-14 00:19:24.000000 tencentcloud-sdk-python-cfs-3.0.935/README.rst
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.934/setup.py` & `tencentcloud-sdk-python-cfs-3.0.935/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfs-3.0.934/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cfs-3.0.935/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cfs-3.0.934/tencentcloud/cfs/v20190719/cfs_client.py` & `tencentcloud-sdk-python-cfs-3.0.935/tencentcloud/cfs/v20190719/cfs_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -671,15 +671,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeUserQuota(self, request):
-        """查询文件系统配额
+        """查询文件系统配额（仅部分Turbo实例能使用，若需要调用请提交工单与我们联系）
 
         :param request: Request instance for DescribeUserQuota.
         :type request: :class:`tencentcloud.cfs.v20190719.models.DescribeUserQuotaRequest`
         :rtype: :class:`tencentcloud.cfs.v20190719.models.DescribeUserQuotaResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.934/tencentcloud/cfs/v20190719/errorcodes.py` & `tencentcloud-sdk-python-cfs-3.0.935/tencentcloud/cfs/v20190719/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfs-3.0.934/tencentcloud/cfs/v20190719/models.py` & `tencentcloud-sdk-python-cfs-3.0.935/tencentcloud/cfs/v20190719/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,19 +33,19 @@
         :type CreationTime: str
         :param _FileSystemNums: 关联的文件系统个数
         :type FileSystemNums: int
         :param _DayOfWeek: 快照定期备份在一星期哪一天，该参数与DayOfMonth,IntervalDays互斥
         :type DayOfWeek: str
         :param _Hour: 快照定期备份在一天的哪一小时
         :type Hour: str
-        :param _IsActivated: 是否激活定期快照功能
+        :param _IsActivated: 是否激活定期快照功能,1代表已激活，0代表未激活
         :type IsActivated: int
         :param _NextActiveTime: 下一次触发快照时间
         :type NextActiveTime: str
-        :param _Status: 快照策略状态
+        :param _Status: 快照策略状态，1代表快照策略状态正常。这里只有一种状态
         :type Status: str
         :param _AppId: 帐号ID
         :type AppId: int
         :param _AliveDays: 保留时间
         :type AliveDays: int
         :param _RegionName: 地域
         :type RegionName: str
@@ -53,15 +53,15 @@
         :type FileSystems: list of FileSystemByPolicy
         :param _DayOfMonth: 快照定期备份在一个月的某个时间；该参数与DayOfWeek,IntervalDays互斥
 注意：此字段可能返回 null，表示取不到有效值。
         :type DayOfMonth: str
         :param _IntervalDays: 快照定期间隔天数，1-365 天；该参数与DayOfMonth,DayOfWeek互斥
 注意：此字段可能返回 null，表示取不到有效值。
         :type IntervalDays: int
-        :param _CrossRegionsAliveDays: 跨地域复制的快照保留时间
+        :param _CrossRegionsAliveDays: 跨地域复制的快照保留时间，单位天
         :type CrossRegionsAliveDays: int
         """
         self._AutoSnapshotPolicyId = None
         self._PolicyName = None
         self._CreationTime = None
         self._FileSystemNums = None
         self._DayOfWeek = None
@@ -648,21 +648,21 @@
 class CreateAutoSnapshotPolicyRequest(AbstractModel):
     """CreateAutoSnapshotPolicy请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Hour: 快照重复时间点
+        :param _Hour: 快照重复时间点,0-23
         :type Hour: str
         :param _PolicyName: 策略名称
         :type PolicyName: str
-        :param _DayOfWeek: 快照重复日期，星期一到星期日
+        :param _DayOfWeek: 快照重复日期，星期一到星期日。 1代表星期一、7代表星期天
         :type DayOfWeek: str
-        :param _AliveDays: 快照保留时长
+        :param _AliveDays: 快照保留时长，单位天
         :type AliveDays: int
         :param _DayOfMonth: 快照按月重复，每月1-31号，选择一天，每月将在这一天自动创建快照。
         :type DayOfMonth: str
         :param _IntervalDays: 间隔天数
         :type IntervalDays: int
         """
         self._Hour = None
@@ -3594,15 +3594,15 @@
         :type FileSystemId: str
         :param _Filters: 过滤条件。
 <br><li>UserType - Array of String - 是否必填：否 -（过滤条件）按配额类型过滤。(Uid| Gid )
 <br><li>UserId - Array of String - 是否必填：否 -（过滤条件）按UID/GID过滤。
         :type Filters: list of Filter
         :param _Offset: Offset 分页码
         :type Offset: int
-        :param _Limit: Limit 页面大小
+        :param _Limit: Limit 页面大小，可填范围为大于0的整数
         :type Limit: int
         """
         self._FileSystemId = None
         self._Filters = None
         self._Offset = None
         self._Limit = None
 
@@ -3720,19 +3720,19 @@
 
     def __init__(self):
         r"""
         :param _CreationToken: 文件系统名称
         :type CreationToken: str
         :param _FileSystemId: 文件系统ID
         :type FileSystemId: str
-        :param _SizeByte: 文件系统大小
+        :param _SizeByte: 文件系统大小，单位Byte
         :type SizeByte: int
-        :param _StorageType: 存储类型
+        :param _StorageType: 存储类型，HP：通用性能型；SD：通用标准型；TP:turbo性能型；TB：turbo标准型；THP：吞吐型
         :type StorageType: str
-        :param _TotalSnapshotSize: 快照总大小
+        :param _TotalSnapshotSize: 快照总大小，单位GiB
         :type TotalSnapshotSize: int
         :param _CreationTime: 文件系统创建时间
         :type CreationTime: str
         :param _ZoneId: 文件系统所在区ID
         :type ZoneId: int
         """
         self._CreationToken = None
@@ -3928,47 +3928,49 @@
 - creating:创建中
 - mounting:挂载中
 - create_failed:创建失败
 - available:可使用
 - unserviced:停服中
 - upgrading:升级中
         :type LifeCycleState: str
-        :param _SizeByte: 文件系统已使用容量
+        :param _SizeByte: 文件系统已使用容量,单位Byte
         :type SizeByte: int
-        :param _SizeLimit: 文件系统最大空间限制
+        :param _SizeLimit: 文件系统最大空间限制,GiB
         :type SizeLimit: int
         :param _ZoneId: 区域 ID
         :type ZoneId: int
         :param _Zone: 区域名称
         :type Zone: str
-        :param _Protocol: 文件系统协议类型
+        :param _Protocol: 文件系统协议类型, 支持 NFS,CIFS,TURBO
         :type Protocol: str
-        :param _StorageType: 文件系统存储类型
+        :param _StorageType: 存储类型，HP：通用性能型；SD：通用标准型；TP:turbo性能型；TB：turbo标准型；THP：吞吐型
         :type StorageType: str
         :param _StorageResourcePkg: 文件系统绑定的预付费存储包
         :type StorageResourcePkg: str
         :param _BandwidthResourcePkg: 文件系统绑定的预付费带宽包（暂未支持）
         :type BandwidthResourcePkg: str
         :param _PGroup: 文件系统绑定权限组信息
         :type PGroup: :class:`tencentcloud.cfs.v20190719.models.PGroup`
         :param _FsName: 用户自定义名称
         :type FsName: str
-        :param _Encrypted: 文件系统是否加密
+        :param _Encrypted: 文件系统是否加密,true：代表加密，false：非加密
         :type Encrypted: bool
         :param _KmsKeyId: 加密所使用的密钥，可以为密钥的 ID 或者 ARN
         :type KmsKeyId: str
         :param _AppId: 应用ID
         :type AppId: int
-        :param _BandwidthLimit: 文件系统吞吐上限，吞吐上限是根据文件系统当前已使用存储量、绑定的存储资源包以及吞吐资源包一同确定
+        :param _BandwidthLimit: 文件系统吞吐上限，吞吐上限是根据文件系统当前已使用存储量、绑定的存储资源包以及吞吐资源包一同确定. 单位MiB/s
         :type BandwidthLimit: float
         :param _Capacity: 文件系统总容量
         :type Capacity: int
         :param _Tags: 文件系统标签列表
         :type Tags: list of TagInfo
         :param _TieringState: 文件系统生命周期管理状态
+NotAvailable：不可用
+Available:可用
         :type TieringState: str
         :param _TieringDetail: 分层存储详情
 注意：此字段可能返回 null，表示取不到有效值。
         :type TieringDetail: :class:`tencentcloud.cfs.v20190719.models.TieringDetailInfo`
         """
         self._CreationTime = None
         self._CreationToken = None
@@ -5361,38 +5363,38 @@
         r"""
         :param _CreationTime: 创建快照时间
         :type CreationTime: str
         :param _SnapshotName: 快照名称
         :type SnapshotName: str
         :param _SnapshotId: 快照ID
         :type SnapshotId: str
-        :param _Status: 快照状态
+        :param _Status: 快照状态，createing-创建中；available-运行中；deleting-删除中；rollbacking-new 创建新文件系统中；create-failed 创建失败
         :type Status: str
         :param _RegionName: 地域名称
         :type RegionName: str
         :param _FileSystemId: 文件系统ID
         :type FileSystemId: str
         :param _Size: 快照大小
         :type Size: int
         :param _AliveDay: 保留时长天
         :type AliveDay: int
-        :param _Percent: 快照进度
+        :param _Percent: 快照进度百分比，1表示1%
         :type Percent: int
         :param _AppId: 帐号ID
         :type AppId: int
         :param _DeleteTime: 快照删除时间
         :type DeleteTime: str
         :param _FsName: 文件系统名称
         :type FsName: str
         :param _Tags: 快照标签
         :type Tags: list of TagInfo
-        :param _SnapshotType: 快照类型
+        :param _SnapshotType: 快照类型, general为通用系列快照，turbo为Turbo系列快照
 注意：此字段可能返回 null，表示取不到有效值。
         :type SnapshotType: str
-        :param _SnapshotTime: 实际快照时间，这里主要是为了标识跨地域复制快照的时间快照时间
+        :param _SnapshotTime: 实际快照时间，反应快照对应文件系统某个时刻的数据。
 注意：此字段可能返回 null，表示取不到有效值。
         :type SnapshotTime: str
         """
         self._CreationTime = None
         self._SnapshotName = None
         self._SnapshotId = None
         self._Status = None
@@ -5564,22 +5566,30 @@
     """快照操作日志
 
     """
 
     def __init__(self):
         r"""
         :param _Action: 操作类型
+CreateCfsSnapshot：创建快照
+DeleteCfsSnapshot：删除快照
+CreateCfsFileSystem：创建文件系统
+UpdateCfsSnapshotAttribute：更新快照
         :type Action: str
         :param _ActionTime: 操作时间
         :type ActionTime: str
         :param _ActionName: 操作名称
+CreateCfsSnapshot
+DeleteCfsSnapshot
+CreateCfsFileSystem
+UpdateCfsSnapshotAttribute
         :type ActionName: str
-        :param _Operator: 操作者
+        :param _Operator: 操作者uin
         :type Operator: str
-        :param _Result: 结果
+        :param _Result: 1-任务进行中；2-任务成功；3-任务失败
         :type Result: int
         """
         self._Action = None
         self._ActionTime = None
         self._ActionName = None
         self._Operator = None
         self._Result = None
@@ -5948,21 +5958,21 @@
 
     def __init__(self):
         r"""
         :param _AutoSnapshotPolicyId: 快照策略ID
         :type AutoSnapshotPolicyId: str
         :param _PolicyName: 快照策略名称
         :type PolicyName: str
-        :param _DayOfWeek: 快照定期备份在一星期哪一天
+        :param _DayOfWeek: 快照定期备份，按照星期一到星期日。 1代表星期一，7代表星期日
         :type DayOfWeek: str
         :param _Hour: 快照定期备份在一天的哪一小时
         :type Hour: str
         :param _AliveDays: 快照保留日期
         :type AliveDays: int
-        :param _IsActivated: 是否激活定期快照功能
+        :param _IsActivated: 是否激活定期快照功能；1代表激活，0代表未激活
         :type IsActivated: int
         :param _DayOfMonth: 定期快照在每月的第几天创建快照，该参数与DayOfWeek互斥
         :type DayOfMonth: str
         :param _IntervalDays: 间隔天数定期执行快照，该参数与DayOfWeek,DayOfMonth 互斥
         :type IntervalDays: int
         """
         self._AutoSnapshotPolicyId = None
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.934/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cfs-3.0.935/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfs
-Version: 3.0.934
+Version: 3.0.935
 Summary: Tencent Cloud Cfs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.934/PKG-INFO` & `tencentcloud-sdk-python-cfs-3.0.935/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfs
-Version: 3.0.934
+Version: 3.0.935
 Summary: Tencent Cloud Cfs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.934/README.rst` & `tencentcloud-sdk-python-cfs-3.0.935/README.rst`

 * *Files identical despite different names*

