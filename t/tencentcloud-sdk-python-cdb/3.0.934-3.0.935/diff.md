# Comparing `tmp/tencentcloud-sdk-python-cdb-3.0.934.tar.gz` & `tmp/tencentcloud-sdk-python-cdb-3.0.935.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdb-3.0.934.tar", last modified: Thu Jul 13 00:17:16 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdb-3.0.935.tar", last modified: Fri Jul 14 00:18:51 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cdb-3.0.934.tar` & `tencentcloud-sdk-python-cdb-3.0.935.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:17:16.000000 tencentcloud-sdk-python-cdb-3.0.934/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-13 00:17:16.000000 tencentcloud-sdk-python-cdb-3.0.934/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:17:16.000000 tencentcloud-sdk-python-cdb-3.0.934/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-13 00:17:16.000000 tencentcloud-sdk-python-cdb-3.0.934/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:17:16.000000 tencentcloud-sdk-python-cdb-3.0.934/tencentcloud/cdb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:17:16.000000 tencentcloud-sdk-python-cdb-3.0.934/tencentcloud/cdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:17:16.000000 tencentcloud-sdk-python-cdb-3.0.934/tencentcloud/cdb/v20170320/
--rw-r--r--   0 root         (0) root         (0)   151510 2023-07-13 00:17:16.000000 tencentcloud-sdk-python-cdb-3.0.934/tencentcloud/cdb/v20170320/cdb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:17:16.000000 tencentcloud-sdk-python-cdb-3.0.934/tencentcloud/cdb/v20170320/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19147 2023-07-13 00:17:16.000000 tencentcloud-sdk-python-cdb-3.0.934/tencentcloud/cdb/v20170320/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   834924 2023-07-13 00:17:16.000000 tencentcloud-sdk-python-cdb-3.0.934/tencentcloud/cdb/v20170320/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-13 00:17:16.000000 tencentcloud-sdk-python-cdb-3.0.934/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:17:16.000000 tencentcloud-sdk-python-cdb-3.0.934/tencentcloud_sdk_python_cdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 00:17:16.000000 tencentcloud-sdk-python-cdb-3.0.934/tencentcloud_sdk_python_cdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-13 00:17:16.000000 tencentcloud-sdk-python-cdb-3.0.934/tencentcloud_sdk_python_cdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-13 00:17:16.000000 tencentcloud-sdk-python-cdb-3.0.934/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-13 00:17:16.000000 tencentcloud-sdk-python-cdb-3.0.934/tencentcloud_sdk_python_cdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-13 00:17:16.000000 tencentcloud-sdk-python-cdb-3.0.934/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-13 00:17:16.000000 tencentcloud-sdk-python-cdb-3.0.934/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:18:51.000000 tencentcloud-sdk-python-cdb-3.0.935/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-14 00:18:51.000000 tencentcloud-sdk-python-cdb-3.0.935/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:18:51.000000 tencentcloud-sdk-python-cdb-3.0.935/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-14 00:18:51.000000 tencentcloud-sdk-python-cdb-3.0.935/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:18:51.000000 tencentcloud-sdk-python-cdb-3.0.935/tencentcloud/cdb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:18:51.000000 tencentcloud-sdk-python-cdb-3.0.935/tencentcloud/cdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:18:51.000000 tencentcloud-sdk-python-cdb-3.0.935/tencentcloud/cdb/v20170320/
+-rw-r--r--   0 root         (0) root         (0)   152421 2023-07-14 00:18:51.000000 tencentcloud-sdk-python-cdb-3.0.935/tencentcloud/cdb/v20170320/cdb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 00:18:51.000000 tencentcloud-sdk-python-cdb-3.0.935/tencentcloud/cdb/v20170320/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19678 2023-07-14 00:18:51.000000 tencentcloud-sdk-python-cdb-3.0.935/tencentcloud/cdb/v20170320/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   846341 2023-07-14 00:18:51.000000 tencentcloud-sdk-python-cdb-3.0.935/tencentcloud/cdb/v20170320/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-14 00:18:51.000000 tencentcloud-sdk-python-cdb-3.0.935/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:18:51.000000 tencentcloud-sdk-python-cdb-3.0.935/tencentcloud_sdk_python_cdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 00:18:51.000000 tencentcloud-sdk-python-cdb-3.0.935/tencentcloud_sdk_python_cdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-14 00:18:51.000000 tencentcloud-sdk-python-cdb-3.0.935/tencentcloud_sdk_python_cdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 00:18:51.000000 tencentcloud-sdk-python-cdb-3.0.935/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-14 00:18:51.000000 tencentcloud-sdk-python-cdb-3.0.935/tencentcloud_sdk_python_cdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 00:18:51.000000 tencentcloud-sdk-python-cdb-3.0.935/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-14 00:18:51.000000 tencentcloud-sdk-python-cdb-3.0.935/README.rst
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.934/setup.py` & `tencentcloud-sdk-python-cdb-3.0.935/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.934/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdb-3.0.935/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cdb-3.0.934/tencentcloud/cdb/v20170320/cdb_client.py` & `tencentcloud-sdk-python-cdb-3.0.935/tencentcloud/cdb/v20170320/cdb_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -892,14 +892,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeAuditLogs(self, request):
+        """本接口(DescribeAuditLogs)用于查询数据库审计日志。
+
+        :param request: Request instance for DescribeAuditLogs.
+        :type request: :class:`tencentcloud.cdb.v20170320.models.DescribeAuditLogsRequest`
+        :rtype: :class:`tencentcloud.cdb.v20170320.models.DescribeAuditLogsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeAuditLogs", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeAuditLogsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeAuditPolicies(self, request):
         """本接口(DescribeAuditPolicies)用于查询云数据库实例的审计策略。
 
         :param request: Request instance for DescribeAuditPolicies.
         :type request: :class:`tencentcloud.cdb.v20170320.models.DescribeAuditPoliciesRequest`
         :rtype: :class:`tencentcloud.cdb.v20170320.models.DescribeAuditPoliciesResponse`
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.934/tencentcloud/cdb/v20170320/errorcodes.py` & `tencentcloud-sdk-python-cdb-3.0.935/tencentcloud/cdb/v20170320/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,17 @@
 
 # 执行的权限修改操作非法。您可以参照产品文档，了解当前实例支持哪些权限修改操作，如有疑问，请您咨询客服进行处理。
 FAILEDOPERATION_PRIVILEGEDATAILLEGAL = 'FailedOperation.PrivilegeDataIllegal'
 
 # 数据库代理状态异常。
 FAILEDOPERATION_PROXYGROUPSTATUSERROR = 'FailedOperation.ProxyGroupStatusError'
 
+# 查询审计任务失败。
+FAILEDOPERATION_QUERYAUDITTASKFAILERROR = 'FailedOperation.QueryAuditTaskFailError'
+
 # 查询日志失败。
 FAILEDOPERATION_QUERYLOGERROR = 'FailedOperation.QueryLogError'
 
 # 代理创建中或则已存在，请勿重复创建。
 FAILEDOPERATION_REPEATCREATEPROXYERROR = 'FailedOperation.RepeatCreateProxyError'
 
 # 后台请求服务异常，请您联系客服解决。
@@ -139,14 +142,17 @@
 
 # 删除审计日志错误。
 INTERNALERROR_AUDITDELETELOGFILEERROR = 'InternalError.AuditDeleteLogFileError'
 
 # 审计内部服务错误。
 INTERNALERROR_AUDITDELETEPOLICYERROR = 'InternalError.AuditDeletePolicyError'
 
+# 查询审计日志错误。
+INTERNALERROR_AUDITDESCRIBELOGERROR = 'InternalError.AuditDescribeLogError'
+
 # 审计内部服务错误。
 INTERNALERROR_AUDITERROR = 'InternalError.AuditError'
 
 # 修改审计状态失败。
 INTERNALERROR_AUDITMODIFYSTATUSERROR = 'InternalError.AuditModifyStatusError'
 
 # 审计服务内部异常。
@@ -487,14 +493,23 @@
 
 # 代理节点超限。
 OPERATIONDENIED_PROXYNODECOUNTLIMITERROR = 'OperationDenied.ProxyNodeCountLimitError'
 
 # 数据库代理升级任务中，不允许该操作。
 OPERATIONDENIED_PROXYUPGRADETASKSTATUSERROR = 'OperationDenied.ProxyUpgradeTaskStatusError'
 
+# 查询审计日志失败。
+OPERATIONDENIED_QUERYAUDITLOGSERROR = 'OperationDenied.QueryAuditLogsError'
+
+# 资源未找到。
+OPERATIONDENIED_RESOURCENOTFOUNDERROR = 'OperationDenied.ResourceNotFoundError'
+
+# 资源未找到。
+OPERATIONDENIED_RESOURCENOTFUNDERROR = 'OperationDenied.ResourceNotFundError'
+
 # 结果集超过限制，请缩小检索范围。
 OPERATIONDENIED_RESULTOVERLIMIT = 'OperationDenied.ResultOverLimit'
 
 # 腾讯云子账号权限不足，不允许执行当前操作。
 OPERATIONDENIED_SUBACCOUNTOPERATIONDENIED = 'OperationDenied.SubAccountOperationDenied'
 
 # 该实例暂不支持退款。
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.934/tencentcloud/cdb/v20170320/models.py` & `tencentcloud-sdk-python-cdb-3.0.935/tencentcloud/cdb/v20170320/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1101,14 +1101,257 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class AuditLog(AbstractModel):
+    """审计日志详细信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _AffectRows: 影响行数。
+        :type AffectRows: int
+        :param _ErrCode: 错误码。
+        :type ErrCode: int
+        :param _SqlType: SQL 类型。
+        :type SqlType: str
+        :param _PolicyName: 审计策略名称，逐步下线。
+        :type PolicyName: str
+        :param _DBName: 数据库名称。
+        :type DBName: str
+        :param _Sql: SQL 语句。
+        :type Sql: str
+        :param _Host: 客户端地址。
+        :type Host: str
+        :param _User: 用户名。
+        :type User: str
+        :param _ExecTime: 执行时间，微秒。
+        :type ExecTime: int
+        :param _Timestamp: 时间。
+        :type Timestamp: str
+        :param _SentRows: 返回行数。
+        :type SentRows: int
+        :param _ThreadId: 线程ID。
+        :type ThreadId: int
+        :param _CheckRows: 扫描行数。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CheckRows: int
+        :param _CpuTime: cpu执行时间，微秒。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CpuTime: float
+        :param _IoWaitTime: IO等待时间，微秒。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IoWaitTime: int
+        :param _LockWaitTime: 锁等待时间，微秒。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LockWaitTime: int
+        :param _NsTime: 开始时间，与timestamp构成一个精确到纳秒的时间。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type NsTime: int
+        :param _TrxLivingTime: 事物持续时间，微秒。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TrxLivingTime: int
+        """
+        self._AffectRows = None
+        self._ErrCode = None
+        self._SqlType = None
+        self._PolicyName = None
+        self._DBName = None
+        self._Sql = None
+        self._Host = None
+        self._User = None
+        self._ExecTime = None
+        self._Timestamp = None
+        self._SentRows = None
+        self._ThreadId = None
+        self._CheckRows = None
+        self._CpuTime = None
+        self._IoWaitTime = None
+        self._LockWaitTime = None
+        self._NsTime = None
+        self._TrxLivingTime = None
+
+    @property
+    def AffectRows(self):
+        return self._AffectRows
+
+    @AffectRows.setter
+    def AffectRows(self, AffectRows):
+        self._AffectRows = AffectRows
+
+    @property
+    def ErrCode(self):
+        return self._ErrCode
+
+    @ErrCode.setter
+    def ErrCode(self, ErrCode):
+        self._ErrCode = ErrCode
+
+    @property
+    def SqlType(self):
+        return self._SqlType
+
+    @SqlType.setter
+    def SqlType(self, SqlType):
+        self._SqlType = SqlType
+
+    @property
+    def PolicyName(self):
+        return self._PolicyName
+
+    @PolicyName.setter
+    def PolicyName(self, PolicyName):
+        self._PolicyName = PolicyName
+
+    @property
+    def DBName(self):
+        return self._DBName
+
+    @DBName.setter
+    def DBName(self, DBName):
+        self._DBName = DBName
+
+    @property
+    def Sql(self):
+        return self._Sql
+
+    @Sql.setter
+    def Sql(self, Sql):
+        self._Sql = Sql
+
+    @property
+    def Host(self):
+        return self._Host
+
+    @Host.setter
+    def Host(self, Host):
+        self._Host = Host
+
+    @property
+    def User(self):
+        return self._User
+
+    @User.setter
+    def User(self, User):
+        self._User = User
+
+    @property
+    def ExecTime(self):
+        return self._ExecTime
+
+    @ExecTime.setter
+    def ExecTime(self, ExecTime):
+        self._ExecTime = ExecTime
+
+    @property
+    def Timestamp(self):
+        return self._Timestamp
+
+    @Timestamp.setter
+    def Timestamp(self, Timestamp):
+        self._Timestamp = Timestamp
+
+    @property
+    def SentRows(self):
+        return self._SentRows
+
+    @SentRows.setter
+    def SentRows(self, SentRows):
+        self._SentRows = SentRows
+
+    @property
+    def ThreadId(self):
+        return self._ThreadId
+
+    @ThreadId.setter
+    def ThreadId(self, ThreadId):
+        self._ThreadId = ThreadId
+
+    @property
+    def CheckRows(self):
+        return self._CheckRows
+
+    @CheckRows.setter
+    def CheckRows(self, CheckRows):
+        self._CheckRows = CheckRows
+
+    @property
+    def CpuTime(self):
+        return self._CpuTime
+
+    @CpuTime.setter
+    def CpuTime(self, CpuTime):
+        self._CpuTime = CpuTime
+
+    @property
+    def IoWaitTime(self):
+        return self._IoWaitTime
+
+    @IoWaitTime.setter
+    def IoWaitTime(self, IoWaitTime):
+        self._IoWaitTime = IoWaitTime
+
+    @property
+    def LockWaitTime(self):
+        return self._LockWaitTime
+
+    @LockWaitTime.setter
+    def LockWaitTime(self, LockWaitTime):
+        self._LockWaitTime = LockWaitTime
+
+    @property
+    def NsTime(self):
+        return self._NsTime
+
+    @NsTime.setter
+    def NsTime(self, NsTime):
+        self._NsTime = NsTime
+
+    @property
+    def TrxLivingTime(self):
+        return self._TrxLivingTime
+
+    @TrxLivingTime.setter
+    def TrxLivingTime(self, TrxLivingTime):
+        self._TrxLivingTime = TrxLivingTime
+
+
+    def _deserialize(self, params):
+        self._AffectRows = params.get("AffectRows")
+        self._ErrCode = params.get("ErrCode")
+        self._SqlType = params.get("SqlType")
+        self._PolicyName = params.get("PolicyName")
+        self._DBName = params.get("DBName")
+        self._Sql = params.get("Sql")
+        self._Host = params.get("Host")
+        self._User = params.get("User")
+        self._ExecTime = params.get("ExecTime")
+        self._Timestamp = params.get("Timestamp")
+        self._SentRows = params.get("SentRows")
+        self._ThreadId = params.get("ThreadId")
+        self._CheckRows = params.get("CheckRows")
+        self._CpuTime = params.get("CpuTime")
+        self._IoWaitTime = params.get("IoWaitTime")
+        self._LockWaitTime = params.get("LockWaitTime")
+        self._NsTime = params.get("NsTime")
+        self._TrxLivingTime = params.get("TrxLivingTime")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class AuditLogAggregationResult(AbstractModel):
     """审计日志分析结果
 
     """
 
     def __init__(self):
         r"""
@@ -8581,14 +8824,194 @@
             for item in params.get("Items"):
                 obj = AuditLogFile()
                 obj._deserialize(item)
                 self._Items.append(obj)
         self._RequestId = params.get("RequestId")
 
 
+class DescribeAuditLogsRequest(AbstractModel):
+    """DescribeAuditLogs请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _InstanceId: 实例 ID。
+        :type InstanceId: str
+        :param _StartTime: 开始时间。
+        :type StartTime: str
+        :param _EndTime: 结束时间。
+        :type EndTime: str
+        :param _Limit: 分页参数，单次返回的数据条数。默认值为100，最大值为100。
+        :type Limit: int
+        :param _Offset: 分页偏移量。
+        :type Offset: int
+        :param _Order: 排序方式。支持值包括："ASC" - 升序，"DESC" - 降序。
+        :type Order: str
+        :param _OrderBy: 排序字段。支持值包括：
+"timestamp" - 时间戳；
+"affectRows" - 影响行数；
+"execTime" - 执行时间。
+        :type OrderBy: str
+        :param _LogFilter: 过滤条件。可按设置的过滤条件过滤日志。
+        :type LogFilter: list of InstanceAuditLogFilters
+        """
+        self._InstanceId = None
+        self._StartTime = None
+        self._EndTime = None
+        self._Limit = None
+        self._Offset = None
+        self._Order = None
+        self._OrderBy = None
+        self._LogFilter = None
+
+    @property
+    def InstanceId(self):
+        return self._InstanceId
+
+    @InstanceId.setter
+    def InstanceId(self, InstanceId):
+        self._InstanceId = InstanceId
+
+    @property
+    def StartTime(self):
+        return self._StartTime
+
+    @StartTime.setter
+    def StartTime(self, StartTime):
+        self._StartTime = StartTime
+
+    @property
+    def EndTime(self):
+        return self._EndTime
+
+    @EndTime.setter
+    def EndTime(self, EndTime):
+        self._EndTime = EndTime
+
+    @property
+    def Limit(self):
+        return self._Limit
+
+    @Limit.setter
+    def Limit(self, Limit):
+        self._Limit = Limit
+
+    @property
+    def Offset(self):
+        return self._Offset
+
+    @Offset.setter
+    def Offset(self, Offset):
+        self._Offset = Offset
+
+    @property
+    def Order(self):
+        return self._Order
+
+    @Order.setter
+    def Order(self, Order):
+        self._Order = Order
+
+    @property
+    def OrderBy(self):
+        return self._OrderBy
+
+    @OrderBy.setter
+    def OrderBy(self, OrderBy):
+        self._OrderBy = OrderBy
+
+    @property
+    def LogFilter(self):
+        return self._LogFilter
+
+    @LogFilter.setter
+    def LogFilter(self, LogFilter):
+        self._LogFilter = LogFilter
+
+
+    def _deserialize(self, params):
+        self._InstanceId = params.get("InstanceId")
+        self._StartTime = params.get("StartTime")
+        self._EndTime = params.get("EndTime")
+        self._Limit = params.get("Limit")
+        self._Offset = params.get("Offset")
+        self._Order = params.get("Order")
+        self._OrderBy = params.get("OrderBy")
+        if params.get("LogFilter") is not None:
+            self._LogFilter = []
+            for item in params.get("LogFilter"):
+                obj = InstanceAuditLogFilters()
+                obj._deserialize(item)
+                self._LogFilter.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeAuditLogsResponse(AbstractModel):
+    """DescribeAuditLogs返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TotalCount: 符合条件的审计日志条数。
+        :type TotalCount: int
+        :param _Items: 审计日志详情。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Items: list of AuditLog
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._TotalCount = None
+        self._Items = None
+        self._RequestId = None
+
+    @property
+    def TotalCount(self):
+        return self._TotalCount
+
+    @TotalCount.setter
+    def TotalCount(self, TotalCount):
+        self._TotalCount = TotalCount
+
+    @property
+    def Items(self):
+        return self._Items
+
+    @Items.setter
+    def Items(self, Items):
+        self._Items = Items
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._TotalCount = params.get("TotalCount")
+        if params.get("Items") is not None:
+            self._Items = []
+            for item in params.get("Items"):
+                obj = AuditLog()
+                obj._deserialize(item)
+                self._Items.append(obj)
+        self._RequestId = params.get("RequestId")
+
+
 class DescribeAuditPoliciesRequest(AbstractModel):
     """DescribeAuditPolicies请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.934/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdb-3.0.935/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdb
-Version: 3.0.934
+Version: 3.0.935
 Summary: Tencent Cloud Cdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.934/PKG-INFO` & `tencentcloud-sdk-python-cdb-3.0.935/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdb
-Version: 3.0.934
+Version: 3.0.935
 Summary: Tencent Cloud Cdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.934/README.rst` & `tencentcloud-sdk-python-cdb-3.0.935/README.rst`

 * *Files identical despite different names*

