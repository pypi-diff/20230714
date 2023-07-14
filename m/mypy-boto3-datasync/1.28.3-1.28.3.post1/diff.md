# Comparing `tmp/mypy-boto3-datasync-1.28.3.tar.gz` & `tmp/mypy-boto3-datasync-1.28.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-datasync-1.28.3.tar", last modified: Thu Jul 13 19:49:12 2023, max compression
+gzip compressed data, was "mypy-boto3-datasync-1.28.3.post1.tar", last modified: Fri Jul 14 16:17:59 2023, max compression
```

## Comparing `mypy-boto3-datasync-1.28.3.tar` & `mypy-boto3-datasync-1.28.3.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:12.653227 mypy-boto3-datasync-1.28.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-13 19:47:08.000000 mypy-boto3-datasync-1.28.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20467 2023-07-13 19:49:12.653227 mypy-boto3-datasync-1.28.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18978 2023-07-13 19:47:08.000000 mypy-boto3-datasync-1.28.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:12.653227 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-13 19:47:08.000000 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-13 19:47:08.000000 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-13 19:47:08.000000 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45373 2023-07-13 19:47:09.000000 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    45301 2023-07-13 19:47:09.000000 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12831 2023-07-13 19:47:09.000000 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-07-13 19:47:09.000000 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-07-13 19:47:09.000000 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9901 2023-07-13 19:47:09.000000 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:47:08.000000 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    55168 2023-07-13 19:47:11.000000 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    55107 2023-07-13 19:47:10.000000 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 19:47:08.000000 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:12.653227 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20467 2023-07-13 19:49:12.000000 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-13 19:49:12.000000 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:12.000000 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:12.000000 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-13 19:49:12.000000 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-13 19:49:12.000000 mypy-boto3-datasync-1.28.3/mypy_boto3_datasync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 19:49:12.653227 mypy-boto3-datasync-1.28.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-13 19:47:08.000000 mypy-boto3-datasync-1.28.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:59.895360 mypy-boto3-datasync-1.28.3.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-14 16:15:31.000000 mypy-boto3-datasync-1.28.3.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21307 2023-07-14 16:17:59.895360 mypy-boto3-datasync-1.28.3.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19812 2023-07-14 16:15:31.000000 mypy-boto3-datasync-1.28.3.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:59.891360 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-14 16:15:31.000000 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-14 16:15:31.000000 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-14 16:15:31.000000 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45897 2023-07-14 16:15:32.000000 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45825 2023-07-14 16:15:32.000000 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12831 2023-07-14 16:15:33.000000 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-07-14 16:15:33.000000 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-07-14 16:15:32.000000 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-07-14 16:15:32.000000 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:15:31.000000 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    59781 2023-07-14 16:15:34.000000 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59720 2023-07-14 16:15:33.000000 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-14 16:15:31.000000 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:59.895360 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21307 2023-07-14 16:17:59.000000 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-14 16:17:59.000000 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:17:59.000000 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:17:59.000000 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-14 16:17:59.000000 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-14 16:17:59.000000 mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 16:17:59.895360 mypy-boto3-datasync-1.28.3.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-14 16:15:31.000000 mypy-boto3-datasync-1.28.3.post1/setup.py
```

### Comparing `mypy-boto3-datasync-1.28.3/LICENSE` & `mypy-boto3-datasync-1.28.3.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datasync-1.28.3/PKG-INFO` & `mypy-boto3-datasync-1.28.3.post1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-datasync
-Version: 1.28.3
-Summary: Type annotations for boto3.DataSync 1.28.3 service generated with mypy-boto3-builder 7.14.6
+Version: 1.28.3.post1
+Summary: Type annotations for boto3.DataSync 1.28.3 service generated with mypy-boto3-builder 7.14.7
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -47,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.6](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.7](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-datasync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/).
 
 See how it helps to find and fix potential bugs:
 
@@ -391,155 +391,170 @@
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_datasync.type_defs import (
     CredentialsTypeDef,
     DiscoveryServerConfigurationTypeDef,
     TagListEntryTypeDef,
-    AddStorageSystemResponseTypeDef,
-    AgentListEntryTypeDef,
+    AddStorageSystemResponseOutputTypeDef,
+    AgentListEntryOutputTypeDef,
     CancelTaskExecutionRequestRequestTypeDef,
-    CapacityTypeDef,
-    CreateAgentResponseTypeDef,
+    CapacityOutputTypeDef,
+    CreateAgentResponseOutputTypeDef,
     Ec2ConfigTypeDef,
-    CreateLocationEfsResponseTypeDef,
-    CreateLocationFsxLustreResponseTypeDef,
-    CreateLocationFsxOntapResponseTypeDef,
-    CreateLocationFsxOpenZfsResponseTypeDef,
-    CreateLocationFsxWindowsResponseTypeDef,
+    CreateLocationEfsResponseOutputTypeDef,
+    CreateLocationFsxLustreResponseOutputTypeDef,
+    CreateLocationFsxOntapResponseOutputTypeDef,
+    CreateLocationFsxOpenZfsResponseOutputTypeDef,
+    CreateLocationFsxWindowsResponseOutputTypeDef,
     HdfsNameNodeTypeDef,
     QopConfigurationTypeDef,
-    CreateLocationHdfsResponseTypeDef,
+    CreateLocationHdfsResponseOutputTypeDef,
     NfsMountOptionsTypeDef,
     OnPremConfigTypeDef,
-    CreateLocationNfsResponseTypeDef,
-    CreateLocationObjectStorageResponseTypeDef,
+    CreateLocationNfsResponseOutputTypeDef,
+    CreateLocationObjectStorageResponseOutputTypeDef,
     S3ConfigTypeDef,
-    CreateLocationS3ResponseTypeDef,
+    CreateLocationS3ResponseOutputTypeDef,
     SmbMountOptionsTypeDef,
-    CreateLocationSmbResponseTypeDef,
+    CreateLocationSmbResponseOutputTypeDef,
     FilterRuleTypeDef,
     OptionsTypeDef,
     TaskScheduleTypeDef,
-    CreateTaskResponseTypeDef,
+    CreateTaskResponseOutputTypeDef,
     DeleteAgentRequestRequestTypeDef,
     DeleteLocationRequestRequestTypeDef,
     DeleteTaskRequestRequestTypeDef,
     DescribeAgentRequestRequestTypeDef,
-    PrivateLinkConfigTypeDef,
+    PrivateLinkConfigOutputTypeDef,
     DescribeDiscoveryJobRequestRequestTypeDef,
-    DescribeDiscoveryJobResponseTypeDef,
+    DescribeDiscoveryJobResponseOutputTypeDef,
     DescribeLocationEfsRequestRequestTypeDef,
+    Ec2ConfigOutputTypeDef,
     DescribeLocationFsxLustreRequestRequestTypeDef,
-    DescribeLocationFsxLustreResponseTypeDef,
+    DescribeLocationFsxLustreResponseOutputTypeDef,
     DescribeLocationFsxOntapRequestRequestTypeDef,
     DescribeLocationFsxOpenZfsRequestRequestTypeDef,
     DescribeLocationFsxWindowsRequestRequestTypeDef,
-    DescribeLocationFsxWindowsResponseTypeDef,
+    DescribeLocationFsxWindowsResponseOutputTypeDef,
     DescribeLocationHdfsRequestRequestTypeDef,
+    HdfsNameNodeOutputTypeDef,
+    QopConfigurationOutputTypeDef,
     DescribeLocationNfsRequestRequestTypeDef,
+    NfsMountOptionsOutputTypeDef,
+    OnPremConfigOutputTypeDef,
     DescribeLocationObjectStorageRequestRequestTypeDef,
-    DescribeLocationObjectStorageResponseTypeDef,
+    DescribeLocationObjectStorageResponseOutputTypeDef,
     DescribeLocationS3RequestRequestTypeDef,
+    S3ConfigOutputTypeDef,
     DescribeLocationSmbRequestRequestTypeDef,
+    SmbMountOptionsOutputTypeDef,
     DescribeStorageSystemRequestRequestTypeDef,
     DescribeStorageSystemResourceMetricsRequestDescribeStorageSystemResourceMetricsPaginateTypeDef,
     DescribeStorageSystemResourceMetricsRequestRequestTypeDef,
     DescribeStorageSystemResourcesRequestRequestTypeDef,
+    DiscoveryServerConfigurationOutputTypeDef,
     DescribeTaskExecutionRequestRequestTypeDef,
-    TaskExecutionResultDetailTypeDef,
+    FilterRuleOutputTypeDef,
+    OptionsOutputTypeDef,
+    TaskExecutionResultDetailOutputTypeDef,
     DescribeTaskRequestRequestTypeDef,
-    DiscoveryJobListEntryTypeDef,
+    TaskScheduleOutputTypeDef,
+    DiscoveryJobListEntryOutputTypeDef,
     GenerateRecommendationsRequestRequestTypeDef,
-    IOPSTypeDef,
-    LatencyTypeDef,
+    IOPSOutputTypeDef,
+    LatencyOutputTypeDef,
     ListAgentsRequestListAgentsPaginateTypeDef,
     ListAgentsRequestRequestTypeDef,
     ListDiscoveryJobsRequestListDiscoveryJobsPaginateTypeDef,
     ListDiscoveryJobsRequestRequestTypeDef,
     LocationFilterTypeDef,
-    LocationListEntryTypeDef,
+    LocationListEntryOutputTypeDef,
     ListStorageSystemsRequestListStorageSystemsPaginateTypeDef,
     ListStorageSystemsRequestRequestTypeDef,
-    StorageSystemListEntryTypeDef,
+    StorageSystemListEntryOutputTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagListEntryOutputTypeDef,
     ListTaskExecutionsRequestListTaskExecutionsPaginateTypeDef,
     ListTaskExecutionsRequestRequestTypeDef,
-    TaskExecutionListEntryTypeDef,
+    TaskExecutionListEntryOutputTypeDef,
     TaskFilterTypeDef,
-    TaskListEntryTypeDef,
-    MaxP95PerformanceTypeDef,
-    RecommendationTypeDef,
-    ThroughputTypeDef,
+    TaskListEntryOutputTypeDef,
+    MaxP95PerformanceOutputTypeDef,
+    RecommendationOutputTypeDef,
+    ThroughputOutputTypeDef,
     PaginatorConfigTypeDef,
     RemoveStorageSystemRequestRequestTypeDef,
     ResponseMetadataTypeDef,
-    StartDiscoveryJobResponseTypeDef,
-    StartTaskExecutionResponseTypeDef,
+    StartDiscoveryJobResponseOutputTypeDef,
+    StartTaskExecutionResponseOutputTypeDef,
     StopDiscoveryJobRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAgentRequestRequestTypeDef,
     UpdateDiscoveryJobRequestRequestTypeDef,
     UpdateLocationObjectStorageRequestRequestTypeDef,
-    DescribeStorageSystemResponseTypeDef,
     UpdateStorageSystemRequestRequestTypeDef,
     AddStorageSystemRequestRequestTypeDef,
     CreateAgentRequestRequestTypeDef,
     CreateLocationFsxLustreRequestRequestTypeDef,
     CreateLocationFsxWindowsRequestRequestTypeDef,
     CreateLocationObjectStorageRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     StartDiscoveryJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    ListAgentsResponseTypeDef,
+    ListAgentsResponseOutputTypeDef,
     CreateLocationEfsRequestRequestTypeDef,
-    DescribeLocationEfsResponseTypeDef,
     CreateLocationHdfsRequestRequestTypeDef,
-    DescribeLocationHdfsResponseTypeDef,
     UpdateLocationHdfsRequestRequestTypeDef,
     FsxProtocolNfsTypeDef,
     CreateLocationNfsRequestRequestTypeDef,
-    DescribeLocationNfsResponseTypeDef,
     UpdateLocationNfsRequestRequestTypeDef,
     CreateLocationS3RequestRequestTypeDef,
-    DescribeLocationS3ResponseTypeDef,
     CreateLocationSmbRequestRequestTypeDef,
-    DescribeLocationSmbResponseTypeDef,
     FsxProtocolSmbTypeDef,
     UpdateLocationSmbRequestRequestTypeDef,
     StartTaskExecutionRequestRequestTypeDef,
     UpdateTaskExecutionRequestRequestTypeDef,
     CreateTaskRequestRequestTypeDef,
-    DescribeTaskResponseTypeDef,
     UpdateTaskRequestRequestTypeDef,
-    DescribeAgentResponseTypeDef,
-    DescribeTaskExecutionResponseTypeDef,
-    ListDiscoveryJobsResponseTypeDef,
+    DescribeAgentResponseOutputTypeDef,
+    DescribeLocationEfsResponseOutputTypeDef,
+    DescribeLocationHdfsResponseOutputTypeDef,
+    FsxProtocolNfsOutputTypeDef,
+    DescribeLocationNfsResponseOutputTypeDef,
+    DescribeLocationS3ResponseOutputTypeDef,
+    DescribeLocationSmbResponseOutputTypeDef,
+    FsxProtocolSmbOutputTypeDef,
+    DescribeStorageSystemResponseOutputTypeDef,
+    DescribeTaskExecutionResponseOutputTypeDef,
+    DescribeTaskResponseOutputTypeDef,
+    ListDiscoveryJobsResponseOutputTypeDef,
     ListLocationsRequestListLocationsPaginateTypeDef,
     ListLocationsRequestRequestTypeDef,
-    ListLocationsResponseTypeDef,
-    ListStorageSystemsResponseTypeDef,
-    ListTaskExecutionsResponseTypeDef,
+    ListLocationsResponseOutputTypeDef,
+    ListStorageSystemsResponseOutputTypeDef,
+    ListTagsForResourceResponseOutputTypeDef,
+    ListTaskExecutionsResponseOutputTypeDef,
     ListTasksRequestListTasksPaginateTypeDef,
     ListTasksRequestRequestTypeDef,
-    ListTasksResponseTypeDef,
-    NetAppONTAPClusterTypeDef,
-    NetAppONTAPSVMTypeDef,
-    NetAppONTAPVolumeTypeDef,
-    P95MetricsTypeDef,
+    ListTasksResponseOutputTypeDef,
+    NetAppONTAPClusterOutputTypeDef,
+    NetAppONTAPSVMOutputTypeDef,
+    NetAppONTAPVolumeOutputTypeDef,
+    P95MetricsOutputTypeDef,
     FsxProtocolTypeDef,
-    ResourceDetailsTypeDef,
-    ResourceMetricsTypeDef,
+    FsxProtocolOutputTypeDef,
+    ResourceDetailsOutputTypeDef,
+    ResourceMetricsOutputTypeDef,
     CreateLocationFsxOntapRequestRequestTypeDef,
     CreateLocationFsxOpenZfsRequestRequestTypeDef,
-    DescribeLocationFsxOntapResponseTypeDef,
-    DescribeLocationFsxOpenZfsResponseTypeDef,
-    DescribeStorageSystemResourcesResponseTypeDef,
-    DescribeStorageSystemResourceMetricsResponseTypeDef,
+    DescribeLocationFsxOntapResponseOutputTypeDef,
+    DescribeLocationFsxOpenZfsResponseOutputTypeDef,
+    DescribeStorageSystemResourcesResponseOutputTypeDef,
+    DescribeStorageSystemResourceMetricsResponseOutputTypeDef,
 )
 
 
 def get_structure() -> CredentialsTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-datasync-1.28.3/README.md` & `mypy-boto3-datasync-1.28.3.post1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.6](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.7](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-datasync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/).
 
 See how it helps to find and fix potential bugs:
 
@@ -359,155 +359,170 @@
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_datasync.type_defs import (
     CredentialsTypeDef,
     DiscoveryServerConfigurationTypeDef,
     TagListEntryTypeDef,
-    AddStorageSystemResponseTypeDef,
-    AgentListEntryTypeDef,
+    AddStorageSystemResponseOutputTypeDef,
+    AgentListEntryOutputTypeDef,
     CancelTaskExecutionRequestRequestTypeDef,
-    CapacityTypeDef,
-    CreateAgentResponseTypeDef,
+    CapacityOutputTypeDef,
+    CreateAgentResponseOutputTypeDef,
     Ec2ConfigTypeDef,
-    CreateLocationEfsResponseTypeDef,
-    CreateLocationFsxLustreResponseTypeDef,
-    CreateLocationFsxOntapResponseTypeDef,
-    CreateLocationFsxOpenZfsResponseTypeDef,
-    CreateLocationFsxWindowsResponseTypeDef,
+    CreateLocationEfsResponseOutputTypeDef,
+    CreateLocationFsxLustreResponseOutputTypeDef,
+    CreateLocationFsxOntapResponseOutputTypeDef,
+    CreateLocationFsxOpenZfsResponseOutputTypeDef,
+    CreateLocationFsxWindowsResponseOutputTypeDef,
     HdfsNameNodeTypeDef,
     QopConfigurationTypeDef,
-    CreateLocationHdfsResponseTypeDef,
+    CreateLocationHdfsResponseOutputTypeDef,
     NfsMountOptionsTypeDef,
     OnPremConfigTypeDef,
-    CreateLocationNfsResponseTypeDef,
-    CreateLocationObjectStorageResponseTypeDef,
+    CreateLocationNfsResponseOutputTypeDef,
+    CreateLocationObjectStorageResponseOutputTypeDef,
     S3ConfigTypeDef,
-    CreateLocationS3ResponseTypeDef,
+    CreateLocationS3ResponseOutputTypeDef,
     SmbMountOptionsTypeDef,
-    CreateLocationSmbResponseTypeDef,
+    CreateLocationSmbResponseOutputTypeDef,
     FilterRuleTypeDef,
     OptionsTypeDef,
     TaskScheduleTypeDef,
-    CreateTaskResponseTypeDef,
+    CreateTaskResponseOutputTypeDef,
     DeleteAgentRequestRequestTypeDef,
     DeleteLocationRequestRequestTypeDef,
     DeleteTaskRequestRequestTypeDef,
     DescribeAgentRequestRequestTypeDef,
-    PrivateLinkConfigTypeDef,
+    PrivateLinkConfigOutputTypeDef,
     DescribeDiscoveryJobRequestRequestTypeDef,
-    DescribeDiscoveryJobResponseTypeDef,
+    DescribeDiscoveryJobResponseOutputTypeDef,
     DescribeLocationEfsRequestRequestTypeDef,
+    Ec2ConfigOutputTypeDef,
     DescribeLocationFsxLustreRequestRequestTypeDef,
-    DescribeLocationFsxLustreResponseTypeDef,
+    DescribeLocationFsxLustreResponseOutputTypeDef,
     DescribeLocationFsxOntapRequestRequestTypeDef,
     DescribeLocationFsxOpenZfsRequestRequestTypeDef,
     DescribeLocationFsxWindowsRequestRequestTypeDef,
-    DescribeLocationFsxWindowsResponseTypeDef,
+    DescribeLocationFsxWindowsResponseOutputTypeDef,
     DescribeLocationHdfsRequestRequestTypeDef,
+    HdfsNameNodeOutputTypeDef,
+    QopConfigurationOutputTypeDef,
     DescribeLocationNfsRequestRequestTypeDef,
+    NfsMountOptionsOutputTypeDef,
+    OnPremConfigOutputTypeDef,
     DescribeLocationObjectStorageRequestRequestTypeDef,
-    DescribeLocationObjectStorageResponseTypeDef,
+    DescribeLocationObjectStorageResponseOutputTypeDef,
     DescribeLocationS3RequestRequestTypeDef,
+    S3ConfigOutputTypeDef,
     DescribeLocationSmbRequestRequestTypeDef,
+    SmbMountOptionsOutputTypeDef,
     DescribeStorageSystemRequestRequestTypeDef,
     DescribeStorageSystemResourceMetricsRequestDescribeStorageSystemResourceMetricsPaginateTypeDef,
     DescribeStorageSystemResourceMetricsRequestRequestTypeDef,
     DescribeStorageSystemResourcesRequestRequestTypeDef,
+    DiscoveryServerConfigurationOutputTypeDef,
     DescribeTaskExecutionRequestRequestTypeDef,
-    TaskExecutionResultDetailTypeDef,
+    FilterRuleOutputTypeDef,
+    OptionsOutputTypeDef,
+    TaskExecutionResultDetailOutputTypeDef,
     DescribeTaskRequestRequestTypeDef,
-    DiscoveryJobListEntryTypeDef,
+    TaskScheduleOutputTypeDef,
+    DiscoveryJobListEntryOutputTypeDef,
     GenerateRecommendationsRequestRequestTypeDef,
-    IOPSTypeDef,
-    LatencyTypeDef,
+    IOPSOutputTypeDef,
+    LatencyOutputTypeDef,
     ListAgentsRequestListAgentsPaginateTypeDef,
     ListAgentsRequestRequestTypeDef,
     ListDiscoveryJobsRequestListDiscoveryJobsPaginateTypeDef,
     ListDiscoveryJobsRequestRequestTypeDef,
     LocationFilterTypeDef,
-    LocationListEntryTypeDef,
+    LocationListEntryOutputTypeDef,
     ListStorageSystemsRequestListStorageSystemsPaginateTypeDef,
     ListStorageSystemsRequestRequestTypeDef,
-    StorageSystemListEntryTypeDef,
+    StorageSystemListEntryOutputTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagListEntryOutputTypeDef,
     ListTaskExecutionsRequestListTaskExecutionsPaginateTypeDef,
     ListTaskExecutionsRequestRequestTypeDef,
-    TaskExecutionListEntryTypeDef,
+    TaskExecutionListEntryOutputTypeDef,
     TaskFilterTypeDef,
-    TaskListEntryTypeDef,
-    MaxP95PerformanceTypeDef,
-    RecommendationTypeDef,
-    ThroughputTypeDef,
+    TaskListEntryOutputTypeDef,
+    MaxP95PerformanceOutputTypeDef,
+    RecommendationOutputTypeDef,
+    ThroughputOutputTypeDef,
     PaginatorConfigTypeDef,
     RemoveStorageSystemRequestRequestTypeDef,
     ResponseMetadataTypeDef,
-    StartDiscoveryJobResponseTypeDef,
-    StartTaskExecutionResponseTypeDef,
+    StartDiscoveryJobResponseOutputTypeDef,
+    StartTaskExecutionResponseOutputTypeDef,
     StopDiscoveryJobRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAgentRequestRequestTypeDef,
     UpdateDiscoveryJobRequestRequestTypeDef,
     UpdateLocationObjectStorageRequestRequestTypeDef,
-    DescribeStorageSystemResponseTypeDef,
     UpdateStorageSystemRequestRequestTypeDef,
     AddStorageSystemRequestRequestTypeDef,
     CreateAgentRequestRequestTypeDef,
     CreateLocationFsxLustreRequestRequestTypeDef,
     CreateLocationFsxWindowsRequestRequestTypeDef,
     CreateLocationObjectStorageRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     StartDiscoveryJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    ListAgentsResponseTypeDef,
+    ListAgentsResponseOutputTypeDef,
     CreateLocationEfsRequestRequestTypeDef,
-    DescribeLocationEfsResponseTypeDef,
     CreateLocationHdfsRequestRequestTypeDef,
-    DescribeLocationHdfsResponseTypeDef,
     UpdateLocationHdfsRequestRequestTypeDef,
     FsxProtocolNfsTypeDef,
     CreateLocationNfsRequestRequestTypeDef,
-    DescribeLocationNfsResponseTypeDef,
     UpdateLocationNfsRequestRequestTypeDef,
     CreateLocationS3RequestRequestTypeDef,
-    DescribeLocationS3ResponseTypeDef,
     CreateLocationSmbRequestRequestTypeDef,
-    DescribeLocationSmbResponseTypeDef,
     FsxProtocolSmbTypeDef,
     UpdateLocationSmbRequestRequestTypeDef,
     StartTaskExecutionRequestRequestTypeDef,
     UpdateTaskExecutionRequestRequestTypeDef,
     CreateTaskRequestRequestTypeDef,
-    DescribeTaskResponseTypeDef,
     UpdateTaskRequestRequestTypeDef,
-    DescribeAgentResponseTypeDef,
-    DescribeTaskExecutionResponseTypeDef,
-    ListDiscoveryJobsResponseTypeDef,
+    DescribeAgentResponseOutputTypeDef,
+    DescribeLocationEfsResponseOutputTypeDef,
+    DescribeLocationHdfsResponseOutputTypeDef,
+    FsxProtocolNfsOutputTypeDef,
+    DescribeLocationNfsResponseOutputTypeDef,
+    DescribeLocationS3ResponseOutputTypeDef,
+    DescribeLocationSmbResponseOutputTypeDef,
+    FsxProtocolSmbOutputTypeDef,
+    DescribeStorageSystemResponseOutputTypeDef,
+    DescribeTaskExecutionResponseOutputTypeDef,
+    DescribeTaskResponseOutputTypeDef,
+    ListDiscoveryJobsResponseOutputTypeDef,
     ListLocationsRequestListLocationsPaginateTypeDef,
     ListLocationsRequestRequestTypeDef,
-    ListLocationsResponseTypeDef,
-    ListStorageSystemsResponseTypeDef,
-    ListTaskExecutionsResponseTypeDef,
+    ListLocationsResponseOutputTypeDef,
+    ListStorageSystemsResponseOutputTypeDef,
+    ListTagsForResourceResponseOutputTypeDef,
+    ListTaskExecutionsResponseOutputTypeDef,
     ListTasksRequestListTasksPaginateTypeDef,
     ListTasksRequestRequestTypeDef,
-    ListTasksResponseTypeDef,
-    NetAppONTAPClusterTypeDef,
-    NetAppONTAPSVMTypeDef,
-    NetAppONTAPVolumeTypeDef,
-    P95MetricsTypeDef,
+    ListTasksResponseOutputTypeDef,
+    NetAppONTAPClusterOutputTypeDef,
+    NetAppONTAPSVMOutputTypeDef,
+    NetAppONTAPVolumeOutputTypeDef,
+    P95MetricsOutputTypeDef,
     FsxProtocolTypeDef,
-    ResourceDetailsTypeDef,
-    ResourceMetricsTypeDef,
+    FsxProtocolOutputTypeDef,
+    ResourceDetailsOutputTypeDef,
+    ResourceMetricsOutputTypeDef,
     CreateLocationFsxOntapRequestRequestTypeDef,
     CreateLocationFsxOpenZfsRequestRequestTypeDef,
-    DescribeLocationFsxOntapResponseTypeDef,
-    DescribeLocationFsxOpenZfsResponseTypeDef,
-    DescribeStorageSystemResourcesResponseTypeDef,
-    DescribeStorageSystemResourceMetricsResponseTypeDef,
+    DescribeLocationFsxOntapResponseOutputTypeDef,
+    DescribeLocationFsxOpenZfsResponseOutputTypeDef,
+    DescribeStorageSystemResourcesResponseOutputTypeDef,
+    DescribeStorageSystemResourceMetricsResponseOutputTypeDef,
 )
 
 
 def get_structure() -> CredentialsTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/__init__.py` & `mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/__init__.pyi` & `mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/__main__.py` & `mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DataSync 1.28.3\nVersion:         1.28.3\nBuilder version:"
-        " 7.14.6\nDocs:           "
+        "Type annotations for boto3.DataSync 1.28.3\nVersion:         1.28.3.post1\nBuilder"
+        " version: 7.14.7\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.3")
+    print("1.28.3.post1")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/client.py` & `mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/client.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -34,94 +34,90 @@
     ListLocationsPaginator,
     ListStorageSystemsPaginator,
     ListTagsForResourcePaginator,
     ListTaskExecutionsPaginator,
     ListTasksPaginator,
 )
 from .type_defs import (
-    AddStorageSystemResponseTypeDef,
-    CreateAgentResponseTypeDef,
-    CreateLocationEfsResponseTypeDef,
-    CreateLocationFsxLustreResponseTypeDef,
-    CreateLocationFsxOntapResponseTypeDef,
-    CreateLocationFsxOpenZfsResponseTypeDef,
-    CreateLocationFsxWindowsResponseTypeDef,
-    CreateLocationHdfsResponseTypeDef,
-    CreateLocationNfsResponseTypeDef,
-    CreateLocationObjectStorageResponseTypeDef,
-    CreateLocationS3ResponseTypeDef,
-    CreateLocationSmbResponseTypeDef,
-    CreateTaskResponseTypeDef,
+    AddStorageSystemResponseOutputTypeDef,
+    CreateAgentResponseOutputTypeDef,
+    CreateLocationEfsResponseOutputTypeDef,
+    CreateLocationFsxLustreResponseOutputTypeDef,
+    CreateLocationFsxOntapResponseOutputTypeDef,
+    CreateLocationFsxOpenZfsResponseOutputTypeDef,
+    CreateLocationFsxWindowsResponseOutputTypeDef,
+    CreateLocationHdfsResponseOutputTypeDef,
+    CreateLocationNfsResponseOutputTypeDef,
+    CreateLocationObjectStorageResponseOutputTypeDef,
+    CreateLocationS3ResponseOutputTypeDef,
+    CreateLocationSmbResponseOutputTypeDef,
+    CreateTaskResponseOutputTypeDef,
     CredentialsTypeDef,
-    DescribeAgentResponseTypeDef,
-    DescribeDiscoveryJobResponseTypeDef,
-    DescribeLocationEfsResponseTypeDef,
-    DescribeLocationFsxLustreResponseTypeDef,
-    DescribeLocationFsxOntapResponseTypeDef,
-    DescribeLocationFsxOpenZfsResponseTypeDef,
-    DescribeLocationFsxWindowsResponseTypeDef,
-    DescribeLocationHdfsResponseTypeDef,
-    DescribeLocationNfsResponseTypeDef,
-    DescribeLocationObjectStorageResponseTypeDef,
-    DescribeLocationS3ResponseTypeDef,
-    DescribeLocationSmbResponseTypeDef,
-    DescribeStorageSystemResourceMetricsResponseTypeDef,
-    DescribeStorageSystemResourcesResponseTypeDef,
-    DescribeStorageSystemResponseTypeDef,
-    DescribeTaskExecutionResponseTypeDef,
-    DescribeTaskResponseTypeDef,
+    DescribeAgentResponseOutputTypeDef,
+    DescribeDiscoveryJobResponseOutputTypeDef,
+    DescribeLocationEfsResponseOutputTypeDef,
+    DescribeLocationFsxLustreResponseOutputTypeDef,
+    DescribeLocationFsxOntapResponseOutputTypeDef,
+    DescribeLocationFsxOpenZfsResponseOutputTypeDef,
+    DescribeLocationFsxWindowsResponseOutputTypeDef,
+    DescribeLocationHdfsResponseOutputTypeDef,
+    DescribeLocationNfsResponseOutputTypeDef,
+    DescribeLocationObjectStorageResponseOutputTypeDef,
+    DescribeLocationS3ResponseOutputTypeDef,
+    DescribeLocationSmbResponseOutputTypeDef,
+    DescribeStorageSystemResourceMetricsResponseOutputTypeDef,
+    DescribeStorageSystemResourcesResponseOutputTypeDef,
+    DescribeStorageSystemResponseOutputTypeDef,
+    DescribeTaskExecutionResponseOutputTypeDef,
+    DescribeTaskResponseOutputTypeDef,
     DiscoveryServerConfigurationTypeDef,
     Ec2ConfigTypeDef,
     FilterRuleTypeDef,
     FsxProtocolTypeDef,
     HdfsNameNodeTypeDef,
-    ListAgentsResponseTypeDef,
-    ListDiscoveryJobsResponseTypeDef,
-    ListLocationsResponseTypeDef,
-    ListStorageSystemsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTaskExecutionsResponseTypeDef,
-    ListTasksResponseTypeDef,
+    ListAgentsResponseOutputTypeDef,
+    ListDiscoveryJobsResponseOutputTypeDef,
+    ListLocationsResponseOutputTypeDef,
+    ListStorageSystemsResponseOutputTypeDef,
+    ListTagsForResourceResponseOutputTypeDef,
+    ListTaskExecutionsResponseOutputTypeDef,
+    ListTasksResponseOutputTypeDef,
     LocationFilterTypeDef,
     NfsMountOptionsTypeDef,
     OnPremConfigTypeDef,
     OptionsTypeDef,
     QopConfigurationTypeDef,
     S3ConfigTypeDef,
     SmbMountOptionsTypeDef,
-    StartDiscoveryJobResponseTypeDef,
-    StartTaskExecutionResponseTypeDef,
+    StartDiscoveryJobResponseOutputTypeDef,
+    StartTaskExecutionResponseOutputTypeDef,
     TagListEntryTypeDef,
     TaskFilterTypeDef,
     TaskScheduleTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("DataSyncClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     InternalException: Type[BotocoreClientError]
     InvalidRequestException: Type[BotocoreClientError]
 
-
 class DataSyncClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/)
     """
 
     meta: ClientMeta
@@ -130,162 +126,151 @@
     def exceptions(self) -> Exceptions:
         """
         DataSyncClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#exceptions)
         """
-
     def add_storage_system(
         self,
         *,
         ServerConfiguration: DiscoveryServerConfigurationTypeDef,
         SystemType: Literal["NetAppONTAP"],
         AgentArns: Sequence[str],
         ClientToken: str,
         Credentials: CredentialsTypeDef,
         CloudWatchLogGroupArn: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         Name: str = ...
-    ) -> AddStorageSystemResponseTypeDef:
+    ) -> AddStorageSystemResponseOutputTypeDef:
         """
         Creates an Amazon Web Services resource for an on-premises storage system that
         you want DataSync Discovery to collect information about.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.add_storage_system)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#add_storage_system)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#can_paginate)
         """
-
     def cancel_task_execution(self, *, TaskExecutionArn: str) -> Dict[str, Any]:
         """
         Stops an DataSync task execution that's in progress.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.cancel_task_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#cancel_task_execution)
         """
-
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#close)
         """
-
     def create_agent(
         self,
         *,
         ActivationKey: str,
         AgentName: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         VpcEndpointId: str = ...,
         SubnetArns: Sequence[str] = ...,
         SecurityGroupArns: Sequence[str] = ...
-    ) -> CreateAgentResponseTypeDef:
+    ) -> CreateAgentResponseOutputTypeDef:
         """
         Activates an DataSync agent that you've deployed in your storage environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_agent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_agent)
         """
-
     def create_location_efs(
         self,
         *,
         EfsFilesystemArn: str,
         Ec2Config: Ec2ConfigTypeDef,
         Subdirectory: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         AccessPointArn: str = ...,
         FileSystemAccessRoleArn: str = ...,
         InTransitEncryption: EfsInTransitEncryptionType = ...
-    ) -> CreateLocationEfsResponseTypeDef:
+    ) -> CreateLocationEfsResponseOutputTypeDef:
         """
         Creates an endpoint for an Amazon EFS file system that DataSync can access for a
         transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_efs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_efs)
         """
-
     def create_location_fsx_lustre(
         self,
         *,
         FsxFilesystemArn: str,
         SecurityGroupArns: Sequence[str],
         Subdirectory: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
-    ) -> CreateLocationFsxLustreResponseTypeDef:
+    ) -> CreateLocationFsxLustreResponseOutputTypeDef:
         """
         Creates an endpoint for an Amazon FSx for Lustre file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_fsx_lustre)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_fsx_lustre)
         """
-
     def create_location_fsx_ontap(
         self,
         *,
         Protocol: FsxProtocolTypeDef,
         SecurityGroupArns: Sequence[str],
         StorageVirtualMachineArn: str,
         Subdirectory: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
-    ) -> CreateLocationFsxOntapResponseTypeDef:
+    ) -> CreateLocationFsxOntapResponseOutputTypeDef:
         """
         Creates an endpoint for an Amazon FSx for NetApp ONTAP file system that DataSync
         can access for a transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_fsx_ontap)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_fsx_ontap)
         """
-
     def create_location_fsx_open_zfs(
         self,
         *,
         FsxFilesystemArn: str,
         Protocol: FsxProtocolTypeDef,
         SecurityGroupArns: Sequence[str],
         Subdirectory: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
-    ) -> CreateLocationFsxOpenZfsResponseTypeDef:
+    ) -> CreateLocationFsxOpenZfsResponseOutputTypeDef:
         """
         Creates an endpoint for an Amazon FSx for OpenZFS file system that DataSync can
         access for a transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_fsx_open_zfs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_fsx_open_zfs)
         """
-
     def create_location_fsx_windows(
         self,
         *,
         FsxFilesystemArn: str,
         SecurityGroupArns: Sequence[str],
         User: str,
         Password: str,
         Subdirectory: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         Domain: str = ...
-    ) -> CreateLocationFsxWindowsResponseTypeDef:
+    ) -> CreateLocationFsxWindowsResponseOutputTypeDef:
         """
         Creates an endpoint for an Amazon FSx for Windows File Server file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_fsx_windows)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_fsx_windows)
         """
-
     def create_location_hdfs(
         self,
         *,
         NameNodes: Sequence[HdfsNameNodeTypeDef],
         AuthenticationType: HdfsAuthenticationTypeType,
         AgentArns: Sequence[str],
         Subdirectory: str = ...,
@@ -294,516 +279,481 @@
         KmsKeyProviderUri: str = ...,
         QopConfiguration: QopConfigurationTypeDef = ...,
         SimpleUser: str = ...,
         KerberosPrincipal: str = ...,
         KerberosKeytab: Union[str, bytes, IO[Any], StreamingBody] = ...,
         KerberosKrb5Conf: Union[str, bytes, IO[Any], StreamingBody] = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
-    ) -> CreateLocationHdfsResponseTypeDef:
+    ) -> CreateLocationHdfsResponseOutputTypeDef:
         """
         Creates an endpoint for a Hadoop Distributed File System (HDFS).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_hdfs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_hdfs)
         """
-
     def create_location_nfs(
         self,
         *,
         Subdirectory: str,
         ServerHostname: str,
         OnPremConfig: OnPremConfigTypeDef,
         MountOptions: NfsMountOptionsTypeDef = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
-    ) -> CreateLocationNfsResponseTypeDef:
+    ) -> CreateLocationNfsResponseOutputTypeDef:
         """
         Defines a file system on a Network File System (NFS) server that can be read
         from or written to.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_nfs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_nfs)
         """
-
     def create_location_object_storage(
         self,
         *,
         ServerHostname: str,
         BucketName: str,
         AgentArns: Sequence[str],
         ServerPort: int = ...,
         ServerProtocol: ObjectStorageServerProtocolType = ...,
         Subdirectory: str = ...,
         AccessKey: str = ...,
         SecretKey: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         ServerCertificate: Union[str, bytes, IO[Any], StreamingBody] = ...
-    ) -> CreateLocationObjectStorageResponseTypeDef:
+    ) -> CreateLocationObjectStorageResponseOutputTypeDef:
         """
         Creates an endpoint for an object storage system that DataSync can access for a
         transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_object_storage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_object_storage)
         """
-
     def create_location_s3(
         self,
         *,
         S3BucketArn: str,
         S3Config: S3ConfigTypeDef,
         Subdirectory: str = ...,
         S3StorageClass: S3StorageClassType = ...,
         AgentArns: Sequence[str] = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
-    ) -> CreateLocationS3ResponseTypeDef:
+    ) -> CreateLocationS3ResponseOutputTypeDef:
         """
         A *location* is an endpoint for an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_s3)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_s3)
         """
-
     def create_location_smb(
         self,
         *,
         Subdirectory: str,
         ServerHostname: str,
         User: str,
         Password: str,
         AgentArns: Sequence[str],
         Domain: str = ...,
         MountOptions: SmbMountOptionsTypeDef = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
-    ) -> CreateLocationSmbResponseTypeDef:
+    ) -> CreateLocationSmbResponseOutputTypeDef:
         """
         Creates an endpoint for a Server Message Block (SMB) file server that DataSync
         can access for a transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_smb)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_smb)
         """
-
     def create_task(
         self,
         *,
         SourceLocationArn: str,
         DestinationLocationArn: str,
         CloudWatchLogGroupArn: str = ...,
         Name: str = ...,
         Options: OptionsTypeDef = ...,
         Excludes: Sequence[FilterRuleTypeDef] = ...,
         Schedule: TaskScheduleTypeDef = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         Includes: Sequence[FilterRuleTypeDef] = ...
-    ) -> CreateTaskResponseTypeDef:
+    ) -> CreateTaskResponseOutputTypeDef:
         """
         Configures a task, which defines where and how DataSync transfers your data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_task)
         """
-
     def delete_agent(self, *, AgentArn: str) -> Dict[str, Any]:
         """
         Deletes an agent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.delete_agent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#delete_agent)
         """
-
     def delete_location(self, *, LocationArn: str) -> Dict[str, Any]:
         """
         Deletes the configuration of a location used by DataSync.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.delete_location)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#delete_location)
         """
-
     def delete_task(self, *, TaskArn: str) -> Dict[str, Any]:
         """
         Deletes an DataSync task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.delete_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#delete_task)
         """
-
-    def describe_agent(self, *, AgentArn: str) -> DescribeAgentResponseTypeDef:
+    def describe_agent(self, *, AgentArn: str) -> DescribeAgentResponseOutputTypeDef:
         """
         Returns metadata about an DataSync agent, such as its name, endpoint type, and
         status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_agent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_agent)
         """
-
     def describe_discovery_job(
         self, *, DiscoveryJobArn: str
-    ) -> DescribeDiscoveryJobResponseTypeDef:
+    ) -> DescribeDiscoveryJobResponseOutputTypeDef:
         """
         Returns information about a DataSync discovery job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_discovery_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_discovery_job)
         """
-
-    def describe_location_efs(self, *, LocationArn: str) -> DescribeLocationEfsResponseTypeDef:
+    def describe_location_efs(
+        self, *, LocationArn: str
+    ) -> DescribeLocationEfsResponseOutputTypeDef:
         """
         Returns metadata about your DataSync location for an Amazon EFS file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_efs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_efs)
         """
-
     def describe_location_fsx_lustre(
         self, *, LocationArn: str
-    ) -> DescribeLocationFsxLustreResponseTypeDef:
+    ) -> DescribeLocationFsxLustreResponseOutputTypeDef:
         """
         Provides details about how an DataSync location for an Amazon FSx for Lustre
         file system is configured.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_fsx_lustre)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_fsx_lustre)
         """
-
     def describe_location_fsx_ontap(
         self, *, LocationArn: str
-    ) -> DescribeLocationFsxOntapResponseTypeDef:
+    ) -> DescribeLocationFsxOntapResponseOutputTypeDef:
         """
         Provides details about how an DataSync location for an Amazon FSx for NetApp
         ONTAP file system is configured.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_fsx_ontap)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_fsx_ontap)
         """
-
     def describe_location_fsx_open_zfs(
         self, *, LocationArn: str
-    ) -> DescribeLocationFsxOpenZfsResponseTypeDef:
+    ) -> DescribeLocationFsxOpenZfsResponseOutputTypeDef:
         """
         Provides details about how an DataSync location for an Amazon FSx for OpenZFS
         file system is configured.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_fsx_open_zfs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_fsx_open_zfs)
         """
-
     def describe_location_fsx_windows(
         self, *, LocationArn: str
-    ) -> DescribeLocationFsxWindowsResponseTypeDef:
+    ) -> DescribeLocationFsxWindowsResponseOutputTypeDef:
         """
         Returns metadata about an Amazon FSx for Windows File Server location, such as
         information about its path.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_fsx_windows)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_fsx_windows)
         """
-
-    def describe_location_hdfs(self, *, LocationArn: str) -> DescribeLocationHdfsResponseTypeDef:
+    def describe_location_hdfs(
+        self, *, LocationArn: str
+    ) -> DescribeLocationHdfsResponseOutputTypeDef:
         """
         Returns metadata, such as the authentication information about the Hadoop
         Distributed File System (HDFS) location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_hdfs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_hdfs)
         """
-
-    def describe_location_nfs(self, *, LocationArn: str) -> DescribeLocationNfsResponseTypeDef:
+    def describe_location_nfs(
+        self, *, LocationArn: str
+    ) -> DescribeLocationNfsResponseOutputTypeDef:
         """
         Returns metadata, such as the path information, about an NFS location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_nfs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_nfs)
         """
-
     def describe_location_object_storage(
         self, *, LocationArn: str
-    ) -> DescribeLocationObjectStorageResponseTypeDef:
+    ) -> DescribeLocationObjectStorageResponseOutputTypeDef:
         """
         Returns metadata about your DataSync location for an object storage system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_object_storage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_object_storage)
         """
-
-    def describe_location_s3(self, *, LocationArn: str) -> DescribeLocationS3ResponseTypeDef:
+    def describe_location_s3(self, *, LocationArn: str) -> DescribeLocationS3ResponseOutputTypeDef:
         """
         Returns metadata, such as bucket name, about an Amazon S3 bucket location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_s3)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_s3)
         """
-
-    def describe_location_smb(self, *, LocationArn: str) -> DescribeLocationSmbResponseTypeDef:
+    def describe_location_smb(
+        self, *, LocationArn: str
+    ) -> DescribeLocationSmbResponseOutputTypeDef:
         """
         Returns metadata, such as the path and user information about an SMB location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_smb)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_smb)
         """
-
     def describe_storage_system(
         self, *, StorageSystemArn: str
-    ) -> DescribeStorageSystemResponseTypeDef:
+    ) -> DescribeStorageSystemResponseOutputTypeDef:
         """
         Returns information about an on-premises storage system that you're using with
         DataSync Discovery.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_storage_system)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_storage_system)
         """
-
     def describe_storage_system_resource_metrics(
         self,
         *,
         DiscoveryJobArn: str,
         ResourceType: DiscoveryResourceTypeType,
         ResourceId: str,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> DescribeStorageSystemResourceMetricsResponseTypeDef:
+    ) -> DescribeStorageSystemResourceMetricsResponseOutputTypeDef:
         """
         Returns information, including performance data and capacity usage, which
         DataSync Discovery collects about a specific resource in your-premises storage
         system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_storage_system_resource_metrics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_storage_system_resource_metrics)
         """
-
     def describe_storage_system_resources(
         self,
         *,
         DiscoveryJobArn: str,
         ResourceType: DiscoveryResourceTypeType,
         ResourceIds: Sequence[str] = ...,
         Filter: Mapping[Literal["SVM"], Sequence[str]] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> DescribeStorageSystemResourcesResponseTypeDef:
+    ) -> DescribeStorageSystemResourcesResponseOutputTypeDef:
         """
         Returns information that DataSync Discovery collects about resources in your on-
         premises storage system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_storage_system_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_storage_system_resources)
         """
-
-    def describe_task(self, *, TaskArn: str) -> DescribeTaskResponseTypeDef:
+    def describe_task(self, *, TaskArn: str) -> DescribeTaskResponseOutputTypeDef:
         """
         Returns metadata about a task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_task)
         """
-
     def describe_task_execution(
         self, *, TaskExecutionArn: str
-    ) -> DescribeTaskExecutionResponseTypeDef:
+    ) -> DescribeTaskExecutionResponseOutputTypeDef:
         """
         Returns detailed metadata about a task that is being executed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_task_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_task_execution)
         """
-
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#generate_presigned_url)
         """
-
     def generate_recommendations(
         self,
         *,
         DiscoveryJobArn: str,
         ResourceIds: Sequence[str],
         ResourceType: DiscoveryResourceTypeType
     ) -> Dict[str, Any]:
         """
         Creates recommendations about where to migrate your data to in Amazon Web
         Services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.generate_recommendations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#generate_recommendations)
         """
-
     def list_agents(
         self, *, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListAgentsResponseTypeDef:
+    ) -> ListAgentsResponseOutputTypeDef:
         """
         Returns a list of DataSync agents that belong to an Amazon Web Services account
         in the Amazon Web Services Region specified in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_agents)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#list_agents)
         """
-
     def list_discovery_jobs(
         self, *, StorageSystemArn: str = ..., MaxResults: int = ..., NextToken: str = ...
-    ) -> ListDiscoveryJobsResponseTypeDef:
+    ) -> ListDiscoveryJobsResponseOutputTypeDef:
         """
         Provides a list of the existing discovery jobs in the Amazon Web Services Region
         and Amazon Web Services account where you're using DataSync Discovery.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_discovery_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#list_discovery_jobs)
         """
-
     def list_locations(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
         Filters: Sequence[LocationFilterTypeDef] = ...
-    ) -> ListLocationsResponseTypeDef:
+    ) -> ListLocationsResponseOutputTypeDef:
         """
         Returns a list of source and destination locations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_locations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#list_locations)
         """
-
     def list_storage_systems(
         self, *, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListStorageSystemsResponseTypeDef:
+    ) -> ListStorageSystemsResponseOutputTypeDef:
         """
         Lists the on-premises storage systems that you're using with DataSync Discovery.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_storage_systems)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#list_storage_systems)
         """
-
     def list_tags_for_resource(
         self, *, ResourceArn: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListTagsForResourceResponseTypeDef:
+    ) -> ListTagsForResourceResponseOutputTypeDef:
         """
         Returns all the tags associated with an Amazon Web Services resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#list_tags_for_resource)
         """
-
     def list_task_executions(
         self, *, TaskArn: str = ..., MaxResults: int = ..., NextToken: str = ...
-    ) -> ListTaskExecutionsResponseTypeDef:
+    ) -> ListTaskExecutionsResponseOutputTypeDef:
         """
         Returns a list of executed tasks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_task_executions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#list_task_executions)
         """
-
     def list_tasks(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
         Filters: Sequence[TaskFilterTypeDef] = ...
-    ) -> ListTasksResponseTypeDef:
+    ) -> ListTasksResponseOutputTypeDef:
         """
         Returns a list of the DataSync tasks you created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_tasks)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#list_tasks)
         """
-
     def remove_storage_system(self, *, StorageSystemArn: str) -> Dict[str, Any]:
         """
         Permanently removes a storage system resource from DataSync Discovery, including
         the associated discovery jobs, collected data, and recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.remove_storage_system)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#remove_storage_system)
         """
-
     def start_discovery_job(
         self,
         *,
         StorageSystemArn: str,
         CollectionDurationMinutes: int,
         ClientToken: str,
         Tags: Sequence[TagListEntryTypeDef] = ...
-    ) -> StartDiscoveryJobResponseTypeDef:
+    ) -> StartDiscoveryJobResponseOutputTypeDef:
         """
         Runs a DataSync discovery job on your on-premises storage system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.start_discovery_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#start_discovery_job)
         """
-
     def start_task_execution(
         self,
         *,
         TaskArn: str,
         OverrideOptions: OptionsTypeDef = ...,
         Includes: Sequence[FilterRuleTypeDef] = ...,
         Excludes: Sequence[FilterRuleTypeDef] = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
-    ) -> StartTaskExecutionResponseTypeDef:
+    ) -> StartTaskExecutionResponseOutputTypeDef:
         """
         Starts an DataSync task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.start_task_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#start_task_execution)
         """
-
     def stop_discovery_job(self, *, DiscoveryJobArn: str) -> Dict[str, Any]:
         """
         Stops a running DataSync discovery job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.stop_discovery_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#stop_discovery_job)
         """
-
     def tag_resource(
         self, *, ResourceArn: str, Tags: Sequence[TagListEntryTypeDef]
     ) -> Dict[str, Any]:
         """
         Applies a *tag* to an Amazon Web Services resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#tag_resource)
         """
-
     def untag_resource(self, *, ResourceArn: str, Keys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes tags from an Amazon Web Services resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#untag_resource)
         """
-
     def update_agent(self, *, AgentArn: str, Name: str = ...) -> Dict[str, Any]:
         """
         Updates the name of an agent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_agent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#update_agent)
         """
-
     def update_discovery_job(
         self, *, DiscoveryJobArn: str, CollectionDurationMinutes: int
     ) -> Dict[str, Any]:
         """
         Edits a DataSync discovery job configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_discovery_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#update_discovery_job)
         """
-
     def update_location_hdfs(
         self,
         *,
         LocationArn: str,
         Subdirectory: str = ...,
         NameNodes: Sequence[HdfsNameNodeTypeDef] = ...,
         BlockSize: int = ...,
@@ -820,15 +770,14 @@
         """
         Updates some parameters of a previously created location for a Hadoop
         Distributed File System cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_location_hdfs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#update_location_hdfs)
         """
-
     def update_location_nfs(
         self,
         *,
         LocationArn: str,
         Subdirectory: str = ...,
         OnPremConfig: OnPremConfigTypeDef = ...,
         MountOptions: NfsMountOptionsTypeDef = ...
@@ -836,15 +785,14 @@
         """
         Updates some of the parameters of a previously created location for Network File
         System (NFS) access.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_location_nfs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#update_location_nfs)
         """
-
     def update_location_object_storage(
         self,
         *,
         LocationArn: str,
         ServerPort: int = ...,
         ServerProtocol: ObjectStorageServerProtocolType = ...,
         Subdirectory: str = ...,
@@ -856,15 +804,14 @@
         """
         Updates some parameters of an existing object storage location that DataSync
         accesses for a transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_location_object_storage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#update_location_object_storage)
         """
-
     def update_location_smb(
         self,
         *,
         LocationArn: str,
         Subdirectory: str = ...,
         User: str = ...,
         Domain: str = ...,
@@ -875,15 +822,14 @@
         """
         Updates some of the parameters of a previously created location for Server
         Message Block (SMB) file system access.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_location_smb)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#update_location_smb)
         """
-
     def update_storage_system(
         self,
         *,
         StorageSystemArn: str,
         ServerConfiguration: DiscoveryServerConfigurationTypeDef = ...,
         AgentArns: Sequence[str] = ...,
         Name: str = ...,
@@ -893,15 +839,14 @@
         """
         Modifies some configurations of an on-premises storage system resource that
         you're using with DataSync Discovery.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_storage_system)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#update_storage_system)
         """
-
     def update_task(
         self,
         *,
         TaskArn: str,
         Options: OptionsTypeDef = ...,
         Excludes: Sequence[FilterRuleTypeDef] = ...,
         Schedule: TaskScheduleTypeDef = ...,
@@ -911,83 +856,74 @@
     ) -> Dict[str, Any]:
         """
         Updates the metadata associated with a task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#update_task)
         """
-
     def update_task_execution(
         self, *, TaskExecutionArn: str, Options: OptionsTypeDef
     ) -> Dict[str, Any]:
         """
         Modifies a running DataSync task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_task_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#update_task_execution)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_storage_system_resource_metrics"]
     ) -> DescribeStorageSystemResourceMetricsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_agents"]) -> ListAgentsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_discovery_jobs"]
     ) -> ListDiscoveryJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_locations"]) -> ListLocationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_storage_systems"]
     ) -> ListStorageSystemsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_tags_for_resource"]
     ) -> ListTagsForResourcePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_task_executions"]
     ) -> ListTaskExecutionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_tasks"]) -> ListTasksPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/client.pyi` & `mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -34,90 +34,94 @@
     ListLocationsPaginator,
     ListStorageSystemsPaginator,
     ListTagsForResourcePaginator,
     ListTaskExecutionsPaginator,
     ListTasksPaginator,
 )
 from .type_defs import (
-    AddStorageSystemResponseTypeDef,
-    CreateAgentResponseTypeDef,
-    CreateLocationEfsResponseTypeDef,
-    CreateLocationFsxLustreResponseTypeDef,
-    CreateLocationFsxOntapResponseTypeDef,
-    CreateLocationFsxOpenZfsResponseTypeDef,
-    CreateLocationFsxWindowsResponseTypeDef,
-    CreateLocationHdfsResponseTypeDef,
-    CreateLocationNfsResponseTypeDef,
-    CreateLocationObjectStorageResponseTypeDef,
-    CreateLocationS3ResponseTypeDef,
-    CreateLocationSmbResponseTypeDef,
-    CreateTaskResponseTypeDef,
+    AddStorageSystemResponseOutputTypeDef,
+    CreateAgentResponseOutputTypeDef,
+    CreateLocationEfsResponseOutputTypeDef,
+    CreateLocationFsxLustreResponseOutputTypeDef,
+    CreateLocationFsxOntapResponseOutputTypeDef,
+    CreateLocationFsxOpenZfsResponseOutputTypeDef,
+    CreateLocationFsxWindowsResponseOutputTypeDef,
+    CreateLocationHdfsResponseOutputTypeDef,
+    CreateLocationNfsResponseOutputTypeDef,
+    CreateLocationObjectStorageResponseOutputTypeDef,
+    CreateLocationS3ResponseOutputTypeDef,
+    CreateLocationSmbResponseOutputTypeDef,
+    CreateTaskResponseOutputTypeDef,
     CredentialsTypeDef,
-    DescribeAgentResponseTypeDef,
-    DescribeDiscoveryJobResponseTypeDef,
-    DescribeLocationEfsResponseTypeDef,
-    DescribeLocationFsxLustreResponseTypeDef,
-    DescribeLocationFsxOntapResponseTypeDef,
-    DescribeLocationFsxOpenZfsResponseTypeDef,
-    DescribeLocationFsxWindowsResponseTypeDef,
-    DescribeLocationHdfsResponseTypeDef,
-    DescribeLocationNfsResponseTypeDef,
-    DescribeLocationObjectStorageResponseTypeDef,
-    DescribeLocationS3ResponseTypeDef,
-    DescribeLocationSmbResponseTypeDef,
-    DescribeStorageSystemResourceMetricsResponseTypeDef,
-    DescribeStorageSystemResourcesResponseTypeDef,
-    DescribeStorageSystemResponseTypeDef,
-    DescribeTaskExecutionResponseTypeDef,
-    DescribeTaskResponseTypeDef,
+    DescribeAgentResponseOutputTypeDef,
+    DescribeDiscoveryJobResponseOutputTypeDef,
+    DescribeLocationEfsResponseOutputTypeDef,
+    DescribeLocationFsxLustreResponseOutputTypeDef,
+    DescribeLocationFsxOntapResponseOutputTypeDef,
+    DescribeLocationFsxOpenZfsResponseOutputTypeDef,
+    DescribeLocationFsxWindowsResponseOutputTypeDef,
+    DescribeLocationHdfsResponseOutputTypeDef,
+    DescribeLocationNfsResponseOutputTypeDef,
+    DescribeLocationObjectStorageResponseOutputTypeDef,
+    DescribeLocationS3ResponseOutputTypeDef,
+    DescribeLocationSmbResponseOutputTypeDef,
+    DescribeStorageSystemResourceMetricsResponseOutputTypeDef,
+    DescribeStorageSystemResourcesResponseOutputTypeDef,
+    DescribeStorageSystemResponseOutputTypeDef,
+    DescribeTaskExecutionResponseOutputTypeDef,
+    DescribeTaskResponseOutputTypeDef,
     DiscoveryServerConfigurationTypeDef,
     Ec2ConfigTypeDef,
     FilterRuleTypeDef,
     FsxProtocolTypeDef,
     HdfsNameNodeTypeDef,
-    ListAgentsResponseTypeDef,
-    ListDiscoveryJobsResponseTypeDef,
-    ListLocationsResponseTypeDef,
-    ListStorageSystemsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTaskExecutionsResponseTypeDef,
-    ListTasksResponseTypeDef,
+    ListAgentsResponseOutputTypeDef,
+    ListDiscoveryJobsResponseOutputTypeDef,
+    ListLocationsResponseOutputTypeDef,
+    ListStorageSystemsResponseOutputTypeDef,
+    ListTagsForResourceResponseOutputTypeDef,
+    ListTaskExecutionsResponseOutputTypeDef,
+    ListTasksResponseOutputTypeDef,
     LocationFilterTypeDef,
     NfsMountOptionsTypeDef,
     OnPremConfigTypeDef,
     OptionsTypeDef,
     QopConfigurationTypeDef,
     S3ConfigTypeDef,
     SmbMountOptionsTypeDef,
-    StartDiscoveryJobResponseTypeDef,
-    StartTaskExecutionResponseTypeDef,
+    StartDiscoveryJobResponseOutputTypeDef,
+    StartTaskExecutionResponseOutputTypeDef,
     TagListEntryTypeDef,
     TaskFilterTypeDef,
     TaskScheduleTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("DataSyncClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     InternalException: Type[BotocoreClientError]
     InvalidRequestException: Type[BotocoreClientError]
 
+
 class DataSyncClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/)
     """
 
     meta: ClientMeta
@@ -126,151 +130,162 @@
     def exceptions(self) -> Exceptions:
         """
         DataSyncClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#exceptions)
         """
+
     def add_storage_system(
         self,
         *,
         ServerConfiguration: DiscoveryServerConfigurationTypeDef,
         SystemType: Literal["NetAppONTAP"],
         AgentArns: Sequence[str],
         ClientToken: str,
         Credentials: CredentialsTypeDef,
         CloudWatchLogGroupArn: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         Name: str = ...
-    ) -> AddStorageSystemResponseTypeDef:
+    ) -> AddStorageSystemResponseOutputTypeDef:
         """
         Creates an Amazon Web Services resource for an on-premises storage system that
         you want DataSync Discovery to collect information about.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.add_storage_system)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#add_storage_system)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#can_paginate)
         """
+
     def cancel_task_execution(self, *, TaskExecutionArn: str) -> Dict[str, Any]:
         """
         Stops an DataSync task execution that's in progress.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.cancel_task_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#cancel_task_execution)
         """
+
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#close)
         """
+
     def create_agent(
         self,
         *,
         ActivationKey: str,
         AgentName: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         VpcEndpointId: str = ...,
         SubnetArns: Sequence[str] = ...,
         SecurityGroupArns: Sequence[str] = ...
-    ) -> CreateAgentResponseTypeDef:
+    ) -> CreateAgentResponseOutputTypeDef:
         """
         Activates an DataSync agent that you've deployed in your storage environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_agent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_agent)
         """
+
     def create_location_efs(
         self,
         *,
         EfsFilesystemArn: str,
         Ec2Config: Ec2ConfigTypeDef,
         Subdirectory: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         AccessPointArn: str = ...,
         FileSystemAccessRoleArn: str = ...,
         InTransitEncryption: EfsInTransitEncryptionType = ...
-    ) -> CreateLocationEfsResponseTypeDef:
+    ) -> CreateLocationEfsResponseOutputTypeDef:
         """
         Creates an endpoint for an Amazon EFS file system that DataSync can access for a
         transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_efs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_efs)
         """
+
     def create_location_fsx_lustre(
         self,
         *,
         FsxFilesystemArn: str,
         SecurityGroupArns: Sequence[str],
         Subdirectory: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
-    ) -> CreateLocationFsxLustreResponseTypeDef:
+    ) -> CreateLocationFsxLustreResponseOutputTypeDef:
         """
         Creates an endpoint for an Amazon FSx for Lustre file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_fsx_lustre)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_fsx_lustre)
         """
+
     def create_location_fsx_ontap(
         self,
         *,
         Protocol: FsxProtocolTypeDef,
         SecurityGroupArns: Sequence[str],
         StorageVirtualMachineArn: str,
         Subdirectory: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
-    ) -> CreateLocationFsxOntapResponseTypeDef:
+    ) -> CreateLocationFsxOntapResponseOutputTypeDef:
         """
         Creates an endpoint for an Amazon FSx for NetApp ONTAP file system that DataSync
         can access for a transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_fsx_ontap)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_fsx_ontap)
         """
+
     def create_location_fsx_open_zfs(
         self,
         *,
         FsxFilesystemArn: str,
         Protocol: FsxProtocolTypeDef,
         SecurityGroupArns: Sequence[str],
         Subdirectory: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
-    ) -> CreateLocationFsxOpenZfsResponseTypeDef:
+    ) -> CreateLocationFsxOpenZfsResponseOutputTypeDef:
         """
         Creates an endpoint for an Amazon FSx for OpenZFS file system that DataSync can
         access for a transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_fsx_open_zfs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_fsx_open_zfs)
         """
+
     def create_location_fsx_windows(
         self,
         *,
         FsxFilesystemArn: str,
         SecurityGroupArns: Sequence[str],
         User: str,
         Password: str,
         Subdirectory: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         Domain: str = ...
-    ) -> CreateLocationFsxWindowsResponseTypeDef:
+    ) -> CreateLocationFsxWindowsResponseOutputTypeDef:
         """
         Creates an endpoint for an Amazon FSx for Windows File Server file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_fsx_windows)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_fsx_windows)
         """
+
     def create_location_hdfs(
         self,
         *,
         NameNodes: Sequence[HdfsNameNodeTypeDef],
         AuthenticationType: HdfsAuthenticationTypeType,
         AgentArns: Sequence[str],
         Subdirectory: str = ...,
@@ -279,473 +294,524 @@
         KmsKeyProviderUri: str = ...,
         QopConfiguration: QopConfigurationTypeDef = ...,
         SimpleUser: str = ...,
         KerberosPrincipal: str = ...,
         KerberosKeytab: Union[str, bytes, IO[Any], StreamingBody] = ...,
         KerberosKrb5Conf: Union[str, bytes, IO[Any], StreamingBody] = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
-    ) -> CreateLocationHdfsResponseTypeDef:
+    ) -> CreateLocationHdfsResponseOutputTypeDef:
         """
         Creates an endpoint for a Hadoop Distributed File System (HDFS).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_hdfs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_hdfs)
         """
+
     def create_location_nfs(
         self,
         *,
         Subdirectory: str,
         ServerHostname: str,
         OnPremConfig: OnPremConfigTypeDef,
         MountOptions: NfsMountOptionsTypeDef = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
-    ) -> CreateLocationNfsResponseTypeDef:
+    ) -> CreateLocationNfsResponseOutputTypeDef:
         """
         Defines a file system on a Network File System (NFS) server that can be read
         from or written to.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_nfs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_nfs)
         """
+
     def create_location_object_storage(
         self,
         *,
         ServerHostname: str,
         BucketName: str,
         AgentArns: Sequence[str],
         ServerPort: int = ...,
         ServerProtocol: ObjectStorageServerProtocolType = ...,
         Subdirectory: str = ...,
         AccessKey: str = ...,
         SecretKey: str = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         ServerCertificate: Union[str, bytes, IO[Any], StreamingBody] = ...
-    ) -> CreateLocationObjectStorageResponseTypeDef:
+    ) -> CreateLocationObjectStorageResponseOutputTypeDef:
         """
         Creates an endpoint for an object storage system that DataSync can access for a
         transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_object_storage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_object_storage)
         """
+
     def create_location_s3(
         self,
         *,
         S3BucketArn: str,
         S3Config: S3ConfigTypeDef,
         Subdirectory: str = ...,
         S3StorageClass: S3StorageClassType = ...,
         AgentArns: Sequence[str] = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
-    ) -> CreateLocationS3ResponseTypeDef:
+    ) -> CreateLocationS3ResponseOutputTypeDef:
         """
         A *location* is an endpoint for an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_s3)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_s3)
         """
+
     def create_location_smb(
         self,
         *,
         Subdirectory: str,
         ServerHostname: str,
         User: str,
         Password: str,
         AgentArns: Sequence[str],
         Domain: str = ...,
         MountOptions: SmbMountOptionsTypeDef = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
-    ) -> CreateLocationSmbResponseTypeDef:
+    ) -> CreateLocationSmbResponseOutputTypeDef:
         """
         Creates an endpoint for a Server Message Block (SMB) file server that DataSync
         can access for a transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_location_smb)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_location_smb)
         """
+
     def create_task(
         self,
         *,
         SourceLocationArn: str,
         DestinationLocationArn: str,
         CloudWatchLogGroupArn: str = ...,
         Name: str = ...,
         Options: OptionsTypeDef = ...,
         Excludes: Sequence[FilterRuleTypeDef] = ...,
         Schedule: TaskScheduleTypeDef = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         Includes: Sequence[FilterRuleTypeDef] = ...
-    ) -> CreateTaskResponseTypeDef:
+    ) -> CreateTaskResponseOutputTypeDef:
         """
         Configures a task, which defines where and how DataSync transfers your data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_task)
         """
+
     def delete_agent(self, *, AgentArn: str) -> Dict[str, Any]:
         """
         Deletes an agent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.delete_agent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#delete_agent)
         """
+
     def delete_location(self, *, LocationArn: str) -> Dict[str, Any]:
         """
         Deletes the configuration of a location used by DataSync.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.delete_location)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#delete_location)
         """
+
     def delete_task(self, *, TaskArn: str) -> Dict[str, Any]:
         """
         Deletes an DataSync task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.delete_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#delete_task)
         """
-    def describe_agent(self, *, AgentArn: str) -> DescribeAgentResponseTypeDef:
+
+    def describe_agent(self, *, AgentArn: str) -> DescribeAgentResponseOutputTypeDef:
         """
         Returns metadata about an DataSync agent, such as its name, endpoint type, and
         status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_agent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_agent)
         """
+
     def describe_discovery_job(
         self, *, DiscoveryJobArn: str
-    ) -> DescribeDiscoveryJobResponseTypeDef:
+    ) -> DescribeDiscoveryJobResponseOutputTypeDef:
         """
         Returns information about a DataSync discovery job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_discovery_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_discovery_job)
         """
-    def describe_location_efs(self, *, LocationArn: str) -> DescribeLocationEfsResponseTypeDef:
+
+    def describe_location_efs(
+        self, *, LocationArn: str
+    ) -> DescribeLocationEfsResponseOutputTypeDef:
         """
         Returns metadata about your DataSync location for an Amazon EFS file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_efs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_efs)
         """
+
     def describe_location_fsx_lustre(
         self, *, LocationArn: str
-    ) -> DescribeLocationFsxLustreResponseTypeDef:
+    ) -> DescribeLocationFsxLustreResponseOutputTypeDef:
         """
         Provides details about how an DataSync location for an Amazon FSx for Lustre
         file system is configured.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_fsx_lustre)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_fsx_lustre)
         """
+
     def describe_location_fsx_ontap(
         self, *, LocationArn: str
-    ) -> DescribeLocationFsxOntapResponseTypeDef:
+    ) -> DescribeLocationFsxOntapResponseOutputTypeDef:
         """
         Provides details about how an DataSync location for an Amazon FSx for NetApp
         ONTAP file system is configured.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_fsx_ontap)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_fsx_ontap)
         """
+
     def describe_location_fsx_open_zfs(
         self, *, LocationArn: str
-    ) -> DescribeLocationFsxOpenZfsResponseTypeDef:
+    ) -> DescribeLocationFsxOpenZfsResponseOutputTypeDef:
         """
         Provides details about how an DataSync location for an Amazon FSx for OpenZFS
         file system is configured.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_fsx_open_zfs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_fsx_open_zfs)
         """
+
     def describe_location_fsx_windows(
         self, *, LocationArn: str
-    ) -> DescribeLocationFsxWindowsResponseTypeDef:
+    ) -> DescribeLocationFsxWindowsResponseOutputTypeDef:
         """
         Returns metadata about an Amazon FSx for Windows File Server location, such as
         information about its path.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_fsx_windows)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_fsx_windows)
         """
-    def describe_location_hdfs(self, *, LocationArn: str) -> DescribeLocationHdfsResponseTypeDef:
+
+    def describe_location_hdfs(
+        self, *, LocationArn: str
+    ) -> DescribeLocationHdfsResponseOutputTypeDef:
         """
         Returns metadata, such as the authentication information about the Hadoop
         Distributed File System (HDFS) location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_hdfs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_hdfs)
         """
-    def describe_location_nfs(self, *, LocationArn: str) -> DescribeLocationNfsResponseTypeDef:
+
+    def describe_location_nfs(
+        self, *, LocationArn: str
+    ) -> DescribeLocationNfsResponseOutputTypeDef:
         """
         Returns metadata, such as the path information, about an NFS location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_nfs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_nfs)
         """
+
     def describe_location_object_storage(
         self, *, LocationArn: str
-    ) -> DescribeLocationObjectStorageResponseTypeDef:
+    ) -> DescribeLocationObjectStorageResponseOutputTypeDef:
         """
         Returns metadata about your DataSync location for an object storage system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_object_storage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_object_storage)
         """
-    def describe_location_s3(self, *, LocationArn: str) -> DescribeLocationS3ResponseTypeDef:
+
+    def describe_location_s3(self, *, LocationArn: str) -> DescribeLocationS3ResponseOutputTypeDef:
         """
         Returns metadata, such as bucket name, about an Amazon S3 bucket location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_s3)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_s3)
         """
-    def describe_location_smb(self, *, LocationArn: str) -> DescribeLocationSmbResponseTypeDef:
+
+    def describe_location_smb(
+        self, *, LocationArn: str
+    ) -> DescribeLocationSmbResponseOutputTypeDef:
         """
         Returns metadata, such as the path and user information about an SMB location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_location_smb)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_location_smb)
         """
+
     def describe_storage_system(
         self, *, StorageSystemArn: str
-    ) -> DescribeStorageSystemResponseTypeDef:
+    ) -> DescribeStorageSystemResponseOutputTypeDef:
         """
         Returns information about an on-premises storage system that you're using with
         DataSync Discovery.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_storage_system)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_storage_system)
         """
+
     def describe_storage_system_resource_metrics(
         self,
         *,
         DiscoveryJobArn: str,
         ResourceType: DiscoveryResourceTypeType,
         ResourceId: str,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> DescribeStorageSystemResourceMetricsResponseTypeDef:
+    ) -> DescribeStorageSystemResourceMetricsResponseOutputTypeDef:
         """
         Returns information, including performance data and capacity usage, which
         DataSync Discovery collects about a specific resource in your-premises storage
         system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_storage_system_resource_metrics)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_storage_system_resource_metrics)
         """
+
     def describe_storage_system_resources(
         self,
         *,
         DiscoveryJobArn: str,
         ResourceType: DiscoveryResourceTypeType,
         ResourceIds: Sequence[str] = ...,
         Filter: Mapping[Literal["SVM"], Sequence[str]] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> DescribeStorageSystemResourcesResponseTypeDef:
+    ) -> DescribeStorageSystemResourcesResponseOutputTypeDef:
         """
         Returns information that DataSync Discovery collects about resources in your on-
         premises storage system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_storage_system_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_storage_system_resources)
         """
-    def describe_task(self, *, TaskArn: str) -> DescribeTaskResponseTypeDef:
+
+    def describe_task(self, *, TaskArn: str) -> DescribeTaskResponseOutputTypeDef:
         """
         Returns metadata about a task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_task)
         """
+
     def describe_task_execution(
         self, *, TaskExecutionArn: str
-    ) -> DescribeTaskExecutionResponseTypeDef:
+    ) -> DescribeTaskExecutionResponseOutputTypeDef:
         """
         Returns detailed metadata about a task that is being executed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_task_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_task_execution)
         """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#generate_presigned_url)
         """
+
     def generate_recommendations(
         self,
         *,
         DiscoveryJobArn: str,
         ResourceIds: Sequence[str],
         ResourceType: DiscoveryResourceTypeType
     ) -> Dict[str, Any]:
         """
         Creates recommendations about where to migrate your data to in Amazon Web
         Services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.generate_recommendations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#generate_recommendations)
         """
+
     def list_agents(
         self, *, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListAgentsResponseTypeDef:
+    ) -> ListAgentsResponseOutputTypeDef:
         """
         Returns a list of DataSync agents that belong to an Amazon Web Services account
         in the Amazon Web Services Region specified in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_agents)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#list_agents)
         """
+
     def list_discovery_jobs(
         self, *, StorageSystemArn: str = ..., MaxResults: int = ..., NextToken: str = ...
-    ) -> ListDiscoveryJobsResponseTypeDef:
+    ) -> ListDiscoveryJobsResponseOutputTypeDef:
         """
         Provides a list of the existing discovery jobs in the Amazon Web Services Region
         and Amazon Web Services account where you're using DataSync Discovery.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_discovery_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#list_discovery_jobs)
         """
+
     def list_locations(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
         Filters: Sequence[LocationFilterTypeDef] = ...
-    ) -> ListLocationsResponseTypeDef:
+    ) -> ListLocationsResponseOutputTypeDef:
         """
         Returns a list of source and destination locations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_locations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#list_locations)
         """
+
     def list_storage_systems(
         self, *, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListStorageSystemsResponseTypeDef:
+    ) -> ListStorageSystemsResponseOutputTypeDef:
         """
         Lists the on-premises storage systems that you're using with DataSync Discovery.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_storage_systems)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#list_storage_systems)
         """
+
     def list_tags_for_resource(
         self, *, ResourceArn: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListTagsForResourceResponseTypeDef:
+    ) -> ListTagsForResourceResponseOutputTypeDef:
         """
         Returns all the tags associated with an Amazon Web Services resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#list_tags_for_resource)
         """
+
     def list_task_executions(
         self, *, TaskArn: str = ..., MaxResults: int = ..., NextToken: str = ...
-    ) -> ListTaskExecutionsResponseTypeDef:
+    ) -> ListTaskExecutionsResponseOutputTypeDef:
         """
         Returns a list of executed tasks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_task_executions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#list_task_executions)
         """
+
     def list_tasks(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
         Filters: Sequence[TaskFilterTypeDef] = ...
-    ) -> ListTasksResponseTypeDef:
+    ) -> ListTasksResponseOutputTypeDef:
         """
         Returns a list of the DataSync tasks you created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.list_tasks)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#list_tasks)
         """
+
     def remove_storage_system(self, *, StorageSystemArn: str) -> Dict[str, Any]:
         """
         Permanently removes a storage system resource from DataSync Discovery, including
         the associated discovery jobs, collected data, and recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.remove_storage_system)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#remove_storage_system)
         """
+
     def start_discovery_job(
         self,
         *,
         StorageSystemArn: str,
         CollectionDurationMinutes: int,
         ClientToken: str,
         Tags: Sequence[TagListEntryTypeDef] = ...
-    ) -> StartDiscoveryJobResponseTypeDef:
+    ) -> StartDiscoveryJobResponseOutputTypeDef:
         """
         Runs a DataSync discovery job on your on-premises storage system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.start_discovery_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#start_discovery_job)
         """
+
     def start_task_execution(
         self,
         *,
         TaskArn: str,
         OverrideOptions: OptionsTypeDef = ...,
         Includes: Sequence[FilterRuleTypeDef] = ...,
         Excludes: Sequence[FilterRuleTypeDef] = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...
-    ) -> StartTaskExecutionResponseTypeDef:
+    ) -> StartTaskExecutionResponseOutputTypeDef:
         """
         Starts an DataSync task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.start_task_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#start_task_execution)
         """
+
     def stop_discovery_job(self, *, DiscoveryJobArn: str) -> Dict[str, Any]:
         """
         Stops a running DataSync discovery job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.stop_discovery_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#stop_discovery_job)
         """
+
     def tag_resource(
         self, *, ResourceArn: str, Tags: Sequence[TagListEntryTypeDef]
     ) -> Dict[str, Any]:
         """
         Applies a *tag* to an Amazon Web Services resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#tag_resource)
         """
+
     def untag_resource(self, *, ResourceArn: str, Keys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes tags from an Amazon Web Services resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#untag_resource)
         """
+
     def update_agent(self, *, AgentArn: str, Name: str = ...) -> Dict[str, Any]:
         """
         Updates the name of an agent.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_agent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#update_agent)
         """
+
     def update_discovery_job(
         self, *, DiscoveryJobArn: str, CollectionDurationMinutes: int
     ) -> Dict[str, Any]:
         """
         Edits a DataSync discovery job configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_discovery_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#update_discovery_job)
         """
+
     def update_location_hdfs(
         self,
         *,
         LocationArn: str,
         Subdirectory: str = ...,
         NameNodes: Sequence[HdfsNameNodeTypeDef] = ...,
         BlockSize: int = ...,
@@ -762,14 +828,15 @@
         """
         Updates some parameters of a previously created location for a Hadoop
         Distributed File System cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_location_hdfs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#update_location_hdfs)
         """
+
     def update_location_nfs(
         self,
         *,
         LocationArn: str,
         Subdirectory: str = ...,
         OnPremConfig: OnPremConfigTypeDef = ...,
         MountOptions: NfsMountOptionsTypeDef = ...
@@ -777,14 +844,15 @@
         """
         Updates some of the parameters of a previously created location for Network File
         System (NFS) access.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_location_nfs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#update_location_nfs)
         """
+
     def update_location_object_storage(
         self,
         *,
         LocationArn: str,
         ServerPort: int = ...,
         ServerProtocol: ObjectStorageServerProtocolType = ...,
         Subdirectory: str = ...,
@@ -796,14 +864,15 @@
         """
         Updates some parameters of an existing object storage location that DataSync
         accesses for a transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_location_object_storage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#update_location_object_storage)
         """
+
     def update_location_smb(
         self,
         *,
         LocationArn: str,
         Subdirectory: str = ...,
         User: str = ...,
         Domain: str = ...,
@@ -814,14 +883,15 @@
         """
         Updates some of the parameters of a previously created location for Server
         Message Block (SMB) file system access.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_location_smb)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#update_location_smb)
         """
+
     def update_storage_system(
         self,
         *,
         StorageSystemArn: str,
         ServerConfiguration: DiscoveryServerConfigurationTypeDef = ...,
         AgentArns: Sequence[str] = ...,
         Name: str = ...,
@@ -831,14 +901,15 @@
         """
         Modifies some configurations of an on-premises storage system resource that
         you're using with DataSync Discovery.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_storage_system)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#update_storage_system)
         """
+
     def update_task(
         self,
         *,
         TaskArn: str,
         Options: OptionsTypeDef = ...,
         Excludes: Sequence[FilterRuleTypeDef] = ...,
         Schedule: TaskScheduleTypeDef = ...,
@@ -848,74 +919,83 @@
     ) -> Dict[str, Any]:
         """
         Updates the metadata associated with a task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#update_task)
         """
+
     def update_task_execution(
         self, *, TaskExecutionArn: str, Options: OptionsTypeDef
     ) -> Dict[str, Any]:
         """
         Modifies a running DataSync task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_task_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#update_task_execution)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_storage_system_resource_metrics"]
     ) -> DescribeStorageSystemResourceMetricsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_agents"]) -> ListAgentsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_discovery_jobs"]
     ) -> ListDiscoveryJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_locations"]) -> ListLocationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_storage_systems"]
     ) -> ListStorageSystemsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_tags_for_resource"]
     ) -> ListTagsForResourcePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_task_executions"]
     ) -> ListTaskExecutionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_tasks"]) -> ListTasksPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/literals.py` & `mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/literals.pyi` & `mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/paginator.py` & `mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,22 +36,22 @@
 from datetime import datetime
 from typing import Generic, Iterator, Sequence, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import DiscoveryResourceTypeType
 from .type_defs import (
-    DescribeStorageSystemResourceMetricsResponseTypeDef,
-    ListAgentsResponseTypeDef,
-    ListDiscoveryJobsResponseTypeDef,
-    ListLocationsResponseTypeDef,
-    ListStorageSystemsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTaskExecutionsResponseTypeDef,
-    ListTasksResponseTypeDef,
+    DescribeStorageSystemResourceMetricsResponseOutputTypeDef,
+    ListAgentsResponseOutputTypeDef,
+    ListDiscoveryJobsResponseOutputTypeDef,
+    ListLocationsResponseOutputTypeDef,
+    ListStorageSystemsResponseOutputTypeDef,
+    ListTagsForResourceResponseOutputTypeDef,
+    ListTaskExecutionsResponseOutputTypeDef,
+    ListTasksResponseOutputTypeDef,
     LocationFilterTypeDef,
     PaginatorConfigTypeDef,
     TaskFilterTypeDef,
 )
 
 __all__ = (
     "DescribeStorageSystemResourceMetricsPaginator",
@@ -86,45 +86,45 @@
         *,
         DiscoveryJobArn: str,
         ResourceType: DiscoveryResourceTypeType,
         ResourceId: str,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeStorageSystemResourceMetricsResponseTypeDef]:
+    ) -> _PageIterator[DescribeStorageSystemResourceMetricsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.DescribeStorageSystemResourceMetrics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#describestoragesystemresourcemetricspaginator)
         """
 
 
 class ListAgentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListAgents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listagentspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListAgentsResponseTypeDef]:
+    ) -> _PageIterator[ListAgentsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListAgents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listagentspaginator)
         """
 
 
 class ListDiscoveryJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListDiscoveryJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listdiscoveryjobspaginator)
     """
 
     def paginate(
         self, *, StorageSystemArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListDiscoveryJobsResponseTypeDef]:
+    ) -> _PageIterator[ListDiscoveryJobsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListDiscoveryJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listdiscoveryjobspaginator)
         """
 
 
 class ListLocationsPaginator(Paginator):
@@ -134,60 +134,60 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[LocationFilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListLocationsResponseTypeDef]:
+    ) -> _PageIterator[ListLocationsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListLocations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listlocationspaginator)
         """
 
 
 class ListStorageSystemsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListStorageSystems)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#liststoragesystemspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListStorageSystemsResponseTypeDef]:
+    ) -> _PageIterator[ListStorageSystemsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListStorageSystems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#liststoragesystemspaginator)
         """
 
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
         self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
+    ) -> _PageIterator[ListTagsForResourceResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listtagsforresourcepaginator)
         """
 
 
 class ListTaskExecutionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListTaskExecutions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listtaskexecutionspaginator)
     """
 
     def paginate(
         self, *, TaskArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListTaskExecutionsResponseTypeDef]:
+    ) -> _PageIterator[ListTaskExecutionsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListTaskExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listtaskexecutionspaginator)
         """
 
 
 class ListTasksPaginator(Paginator):
@@ -197,12 +197,12 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[TaskFilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListTasksResponseTypeDef]:
+    ) -> _PageIterator[ListTasksResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listtaskspaginator)
         """
```

### Comparing `mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/paginator.pyi` & `mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/paginator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -36,22 +36,22 @@
 from datetime import datetime
 from typing import Generic, Iterator, Sequence, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import DiscoveryResourceTypeType
 from .type_defs import (
-    DescribeStorageSystemResourceMetricsResponseTypeDef,
-    ListAgentsResponseTypeDef,
-    ListDiscoveryJobsResponseTypeDef,
-    ListLocationsResponseTypeDef,
-    ListStorageSystemsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTaskExecutionsResponseTypeDef,
-    ListTasksResponseTypeDef,
+    DescribeStorageSystemResourceMetricsResponseOutputTypeDef,
+    ListAgentsResponseOutputTypeDef,
+    ListDiscoveryJobsResponseOutputTypeDef,
+    ListLocationsResponseOutputTypeDef,
+    ListStorageSystemsResponseOutputTypeDef,
+    ListTagsForResourceResponseOutputTypeDef,
+    ListTaskExecutionsResponseOutputTypeDef,
+    ListTasksResponseOutputTypeDef,
     LocationFilterTypeDef,
     PaginatorConfigTypeDef,
     TaskFilterTypeDef,
 )
 
 __all__ = (
     "DescribeStorageSystemResourceMetricsPaginator",
@@ -83,43 +83,43 @@
         *,
         DiscoveryJobArn: str,
         ResourceType: DiscoveryResourceTypeType,
         ResourceId: str,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeStorageSystemResourceMetricsResponseTypeDef]:
+    ) -> _PageIterator[DescribeStorageSystemResourceMetricsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.DescribeStorageSystemResourceMetrics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#describestoragesystemresourcemetricspaginator)
         """
 
 class ListAgentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListAgents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listagentspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListAgentsResponseTypeDef]:
+    ) -> _PageIterator[ListAgentsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListAgents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listagentspaginator)
         """
 
 class ListDiscoveryJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListDiscoveryJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listdiscoveryjobspaginator)
     """
 
     def paginate(
         self, *, StorageSystemArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListDiscoveryJobsResponseTypeDef]:
+    ) -> _PageIterator[ListDiscoveryJobsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListDiscoveryJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listdiscoveryjobspaginator)
         """
 
 class ListLocationsPaginator(Paginator):
     """
@@ -128,57 +128,57 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[LocationFilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListLocationsResponseTypeDef]:
+    ) -> _PageIterator[ListLocationsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListLocations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listlocationspaginator)
         """
 
 class ListStorageSystemsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListStorageSystems)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#liststoragesystemspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListStorageSystemsResponseTypeDef]:
+    ) -> _PageIterator[ListStorageSystemsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListStorageSystems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#liststoragesystemspaginator)
         """
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
         self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
+    ) -> _PageIterator[ListTagsForResourceResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listtagsforresourcepaginator)
         """
 
 class ListTaskExecutionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListTaskExecutions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listtaskexecutionspaginator)
     """
 
     def paginate(
         self, *, TaskArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListTaskExecutionsResponseTypeDef]:
+    ) -> _PageIterator[ListTaskExecutionsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListTaskExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listtaskexecutionspaginator)
         """
 
 class ListTasksPaginator(Paginator):
     """
@@ -187,12 +187,12 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[TaskFilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListTasksResponseTypeDef]:
+    ) -> _PageIterator[ListTasksResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Paginator.ListTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/paginators/#listtaskspaginator)
         """
```

### Comparing `mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/type_defs.py` & `mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -59,160 +59,174 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CredentialsTypeDef",
     "DiscoveryServerConfigurationTypeDef",
     "TagListEntryTypeDef",
-    "AddStorageSystemResponseTypeDef",
-    "AgentListEntryTypeDef",
+    "AddStorageSystemResponseOutputTypeDef",
+    "AgentListEntryOutputTypeDef",
     "CancelTaskExecutionRequestRequestTypeDef",
-    "CapacityTypeDef",
-    "CreateAgentResponseTypeDef",
+    "CapacityOutputTypeDef",
+    "CreateAgentResponseOutputTypeDef",
     "Ec2ConfigTypeDef",
-    "CreateLocationEfsResponseTypeDef",
-    "CreateLocationFsxLustreResponseTypeDef",
-    "CreateLocationFsxOntapResponseTypeDef",
-    "CreateLocationFsxOpenZfsResponseTypeDef",
-    "CreateLocationFsxWindowsResponseTypeDef",
+    "CreateLocationEfsResponseOutputTypeDef",
+    "CreateLocationFsxLustreResponseOutputTypeDef",
+    "CreateLocationFsxOntapResponseOutputTypeDef",
+    "CreateLocationFsxOpenZfsResponseOutputTypeDef",
+    "CreateLocationFsxWindowsResponseOutputTypeDef",
     "HdfsNameNodeTypeDef",
     "QopConfigurationTypeDef",
-    "CreateLocationHdfsResponseTypeDef",
+    "CreateLocationHdfsResponseOutputTypeDef",
     "NfsMountOptionsTypeDef",
     "OnPremConfigTypeDef",
-    "CreateLocationNfsResponseTypeDef",
-    "CreateLocationObjectStorageResponseTypeDef",
+    "CreateLocationNfsResponseOutputTypeDef",
+    "CreateLocationObjectStorageResponseOutputTypeDef",
     "S3ConfigTypeDef",
-    "CreateLocationS3ResponseTypeDef",
+    "CreateLocationS3ResponseOutputTypeDef",
     "SmbMountOptionsTypeDef",
-    "CreateLocationSmbResponseTypeDef",
+    "CreateLocationSmbResponseOutputTypeDef",
     "FilterRuleTypeDef",
     "OptionsTypeDef",
     "TaskScheduleTypeDef",
-    "CreateTaskResponseTypeDef",
+    "CreateTaskResponseOutputTypeDef",
     "DeleteAgentRequestRequestTypeDef",
     "DeleteLocationRequestRequestTypeDef",
     "DeleteTaskRequestRequestTypeDef",
     "DescribeAgentRequestRequestTypeDef",
-    "PrivateLinkConfigTypeDef",
+    "PrivateLinkConfigOutputTypeDef",
     "DescribeDiscoveryJobRequestRequestTypeDef",
-    "DescribeDiscoveryJobResponseTypeDef",
+    "DescribeDiscoveryJobResponseOutputTypeDef",
     "DescribeLocationEfsRequestRequestTypeDef",
+    "Ec2ConfigOutputTypeDef",
     "DescribeLocationFsxLustreRequestRequestTypeDef",
-    "DescribeLocationFsxLustreResponseTypeDef",
+    "DescribeLocationFsxLustreResponseOutputTypeDef",
     "DescribeLocationFsxOntapRequestRequestTypeDef",
     "DescribeLocationFsxOpenZfsRequestRequestTypeDef",
     "DescribeLocationFsxWindowsRequestRequestTypeDef",
-    "DescribeLocationFsxWindowsResponseTypeDef",
+    "DescribeLocationFsxWindowsResponseOutputTypeDef",
     "DescribeLocationHdfsRequestRequestTypeDef",
+    "HdfsNameNodeOutputTypeDef",
+    "QopConfigurationOutputTypeDef",
     "DescribeLocationNfsRequestRequestTypeDef",
+    "NfsMountOptionsOutputTypeDef",
+    "OnPremConfigOutputTypeDef",
     "DescribeLocationObjectStorageRequestRequestTypeDef",
-    "DescribeLocationObjectStorageResponseTypeDef",
+    "DescribeLocationObjectStorageResponseOutputTypeDef",
     "DescribeLocationS3RequestRequestTypeDef",
+    "S3ConfigOutputTypeDef",
     "DescribeLocationSmbRequestRequestTypeDef",
+    "SmbMountOptionsOutputTypeDef",
     "DescribeStorageSystemRequestRequestTypeDef",
     "DescribeStorageSystemResourceMetricsRequestDescribeStorageSystemResourceMetricsPaginateTypeDef",
     "DescribeStorageSystemResourceMetricsRequestRequestTypeDef",
     "DescribeStorageSystemResourcesRequestRequestTypeDef",
+    "DiscoveryServerConfigurationOutputTypeDef",
     "DescribeTaskExecutionRequestRequestTypeDef",
-    "TaskExecutionResultDetailTypeDef",
+    "FilterRuleOutputTypeDef",
+    "OptionsOutputTypeDef",
+    "TaskExecutionResultDetailOutputTypeDef",
     "DescribeTaskRequestRequestTypeDef",
-    "DiscoveryJobListEntryTypeDef",
+    "TaskScheduleOutputTypeDef",
+    "DiscoveryJobListEntryOutputTypeDef",
     "GenerateRecommendationsRequestRequestTypeDef",
-    "IOPSTypeDef",
-    "LatencyTypeDef",
+    "IOPSOutputTypeDef",
+    "LatencyOutputTypeDef",
     "ListAgentsRequestListAgentsPaginateTypeDef",
     "ListAgentsRequestRequestTypeDef",
     "ListDiscoveryJobsRequestListDiscoveryJobsPaginateTypeDef",
     "ListDiscoveryJobsRequestRequestTypeDef",
     "LocationFilterTypeDef",
-    "LocationListEntryTypeDef",
+    "LocationListEntryOutputTypeDef",
     "ListStorageSystemsRequestListStorageSystemsPaginateTypeDef",
     "ListStorageSystemsRequestRequestTypeDef",
-    "StorageSystemListEntryTypeDef",
+    "StorageSystemListEntryOutputTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagListEntryOutputTypeDef",
     "ListTaskExecutionsRequestListTaskExecutionsPaginateTypeDef",
     "ListTaskExecutionsRequestRequestTypeDef",
-    "TaskExecutionListEntryTypeDef",
+    "TaskExecutionListEntryOutputTypeDef",
     "TaskFilterTypeDef",
-    "TaskListEntryTypeDef",
-    "MaxP95PerformanceTypeDef",
-    "RecommendationTypeDef",
-    "ThroughputTypeDef",
+    "TaskListEntryOutputTypeDef",
+    "MaxP95PerformanceOutputTypeDef",
+    "RecommendationOutputTypeDef",
+    "ThroughputOutputTypeDef",
     "PaginatorConfigTypeDef",
     "RemoveStorageSystemRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
-    "StartDiscoveryJobResponseTypeDef",
-    "StartTaskExecutionResponseTypeDef",
+    "StartDiscoveryJobResponseOutputTypeDef",
+    "StartTaskExecutionResponseOutputTypeDef",
     "StopDiscoveryJobRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAgentRequestRequestTypeDef",
     "UpdateDiscoveryJobRequestRequestTypeDef",
     "UpdateLocationObjectStorageRequestRequestTypeDef",
-    "DescribeStorageSystemResponseTypeDef",
     "UpdateStorageSystemRequestRequestTypeDef",
     "AddStorageSystemRequestRequestTypeDef",
     "CreateAgentRequestRequestTypeDef",
     "CreateLocationFsxLustreRequestRequestTypeDef",
     "CreateLocationFsxWindowsRequestRequestTypeDef",
     "CreateLocationObjectStorageRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "StartDiscoveryJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "ListAgentsResponseTypeDef",
+    "ListAgentsResponseOutputTypeDef",
     "CreateLocationEfsRequestRequestTypeDef",
-    "DescribeLocationEfsResponseTypeDef",
     "CreateLocationHdfsRequestRequestTypeDef",
-    "DescribeLocationHdfsResponseTypeDef",
     "UpdateLocationHdfsRequestRequestTypeDef",
     "FsxProtocolNfsTypeDef",
     "CreateLocationNfsRequestRequestTypeDef",
-    "DescribeLocationNfsResponseTypeDef",
     "UpdateLocationNfsRequestRequestTypeDef",
     "CreateLocationS3RequestRequestTypeDef",
-    "DescribeLocationS3ResponseTypeDef",
     "CreateLocationSmbRequestRequestTypeDef",
-    "DescribeLocationSmbResponseTypeDef",
     "FsxProtocolSmbTypeDef",
     "UpdateLocationSmbRequestRequestTypeDef",
     "StartTaskExecutionRequestRequestTypeDef",
     "UpdateTaskExecutionRequestRequestTypeDef",
     "CreateTaskRequestRequestTypeDef",
-    "DescribeTaskResponseTypeDef",
     "UpdateTaskRequestRequestTypeDef",
-    "DescribeAgentResponseTypeDef",
-    "DescribeTaskExecutionResponseTypeDef",
-    "ListDiscoveryJobsResponseTypeDef",
+    "DescribeAgentResponseOutputTypeDef",
+    "DescribeLocationEfsResponseOutputTypeDef",
+    "DescribeLocationHdfsResponseOutputTypeDef",
+    "FsxProtocolNfsOutputTypeDef",
+    "DescribeLocationNfsResponseOutputTypeDef",
+    "DescribeLocationS3ResponseOutputTypeDef",
+    "DescribeLocationSmbResponseOutputTypeDef",
+    "FsxProtocolSmbOutputTypeDef",
+    "DescribeStorageSystemResponseOutputTypeDef",
+    "DescribeTaskExecutionResponseOutputTypeDef",
+    "DescribeTaskResponseOutputTypeDef",
+    "ListDiscoveryJobsResponseOutputTypeDef",
     "ListLocationsRequestListLocationsPaginateTypeDef",
     "ListLocationsRequestRequestTypeDef",
-    "ListLocationsResponseTypeDef",
-    "ListStorageSystemsResponseTypeDef",
-    "ListTaskExecutionsResponseTypeDef",
+    "ListLocationsResponseOutputTypeDef",
+    "ListStorageSystemsResponseOutputTypeDef",
+    "ListTagsForResourceResponseOutputTypeDef",
+    "ListTaskExecutionsResponseOutputTypeDef",
     "ListTasksRequestListTasksPaginateTypeDef",
     "ListTasksRequestRequestTypeDef",
-    "ListTasksResponseTypeDef",
-    "NetAppONTAPClusterTypeDef",
-    "NetAppONTAPSVMTypeDef",
-    "NetAppONTAPVolumeTypeDef",
-    "P95MetricsTypeDef",
+    "ListTasksResponseOutputTypeDef",
+    "NetAppONTAPClusterOutputTypeDef",
+    "NetAppONTAPSVMOutputTypeDef",
+    "NetAppONTAPVolumeOutputTypeDef",
+    "P95MetricsOutputTypeDef",
     "FsxProtocolTypeDef",
-    "ResourceDetailsTypeDef",
-    "ResourceMetricsTypeDef",
+    "FsxProtocolOutputTypeDef",
+    "ResourceDetailsOutputTypeDef",
+    "ResourceMetricsOutputTypeDef",
     "CreateLocationFsxOntapRequestRequestTypeDef",
     "CreateLocationFsxOpenZfsRequestRequestTypeDef",
-    "DescribeLocationFsxOntapResponseTypeDef",
-    "DescribeLocationFsxOpenZfsResponseTypeDef",
-    "DescribeStorageSystemResourcesResponseTypeDef",
-    "DescribeStorageSystemResourceMetricsResponseTypeDef",
+    "DescribeLocationFsxOntapResponseOutputTypeDef",
+    "DescribeLocationFsxOpenZfsResponseOutputTypeDef",
+    "DescribeStorageSystemResourcesResponseOutputTypeDef",
+    "DescribeStorageSystemResourceMetricsResponseOutputTypeDef",
 )
 
 CredentialsTypeDef = TypedDict(
     "CredentialsTypeDef",
     {
         "Username": str,
         "Password": str,
@@ -229,123 +243,119 @@
     "_OptionalDiscoveryServerConfigurationTypeDef",
     {
         "ServerPort": int,
     },
     total=False,
 )
 
-
 class DiscoveryServerConfigurationTypeDef(
     _RequiredDiscoveryServerConfigurationTypeDef, _OptionalDiscoveryServerConfigurationTypeDef
 ):
     pass
 
-
 _RequiredTagListEntryTypeDef = TypedDict(
     "_RequiredTagListEntryTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalTagListEntryTypeDef = TypedDict(
     "_OptionalTagListEntryTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-
 class TagListEntryTypeDef(_RequiredTagListEntryTypeDef, _OptionalTagListEntryTypeDef):
     pass
 
-
-AddStorageSystemResponseTypeDef = TypedDict(
-    "AddStorageSystemResponseTypeDef",
+AddStorageSystemResponseOutputTypeDef = TypedDict(
+    "AddStorageSystemResponseOutputTypeDef",
     {
         "StorageSystemArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-AgentListEntryTypeDef = TypedDict(
-    "AgentListEntryTypeDef",
+AgentListEntryOutputTypeDef = TypedDict(
+    "AgentListEntryOutputTypeDef",
     {
         "AgentArn": str,
         "Name": str,
         "Status": AgentStatusType,
     },
 )
 
 CancelTaskExecutionRequestRequestTypeDef = TypedDict(
     "CancelTaskExecutionRequestRequestTypeDef",
     {
         "TaskExecutionArn": str,
     },
 )
 
-CapacityTypeDef = TypedDict(
-    "CapacityTypeDef",
+CapacityOutputTypeDef = TypedDict(
+    "CapacityOutputTypeDef",
     {
         "Used": int,
         "Provisioned": int,
         "LogicalUsed": int,
     },
 )
 
-CreateAgentResponseTypeDef = TypedDict(
-    "CreateAgentResponseTypeDef",
+CreateAgentResponseOutputTypeDef = TypedDict(
+    "CreateAgentResponseOutputTypeDef",
     {
         "AgentArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 Ec2ConfigTypeDef = TypedDict(
     "Ec2ConfigTypeDef",
     {
         "SubnetArn": str,
         "SecurityGroupArns": Sequence[str],
     },
 )
 
-CreateLocationEfsResponseTypeDef = TypedDict(
-    "CreateLocationEfsResponseTypeDef",
+CreateLocationEfsResponseOutputTypeDef = TypedDict(
+    "CreateLocationEfsResponseOutputTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateLocationFsxLustreResponseTypeDef = TypedDict(
-    "CreateLocationFsxLustreResponseTypeDef",
+CreateLocationFsxLustreResponseOutputTypeDef = TypedDict(
+    "CreateLocationFsxLustreResponseOutputTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateLocationFsxOntapResponseTypeDef = TypedDict(
-    "CreateLocationFsxOntapResponseTypeDef",
+CreateLocationFsxOntapResponseOutputTypeDef = TypedDict(
+    "CreateLocationFsxOntapResponseOutputTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateLocationFsxOpenZfsResponseTypeDef = TypedDict(
-    "CreateLocationFsxOpenZfsResponseTypeDef",
+CreateLocationFsxOpenZfsResponseOutputTypeDef = TypedDict(
+    "CreateLocationFsxOpenZfsResponseOutputTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateLocationFsxWindowsResponseTypeDef = TypedDict(
-    "CreateLocationFsxWindowsResponseTypeDef",
+CreateLocationFsxWindowsResponseOutputTypeDef = TypedDict(
+    "CreateLocationFsxWindowsResponseOutputTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 HdfsNameNodeTypeDef = TypedDict(
@@ -361,16 +371,16 @@
     {
         "RpcProtection": HdfsRpcProtectionType,
         "DataTransferProtection": HdfsDataTransferProtectionType,
     },
     total=False,
 )
 
-CreateLocationHdfsResponseTypeDef = TypedDict(
-    "CreateLocationHdfsResponseTypeDef",
+CreateLocationHdfsResponseOutputTypeDef = TypedDict(
+    "CreateLocationHdfsResponseOutputTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 NfsMountOptionsTypeDef = TypedDict(
@@ -384,55 +394,55 @@
 OnPremConfigTypeDef = TypedDict(
     "OnPremConfigTypeDef",
     {
         "AgentArns": Sequence[str],
     },
 )
 
-CreateLocationNfsResponseTypeDef = TypedDict(
-    "CreateLocationNfsResponseTypeDef",
+CreateLocationNfsResponseOutputTypeDef = TypedDict(
+    "CreateLocationNfsResponseOutputTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateLocationObjectStorageResponseTypeDef = TypedDict(
-    "CreateLocationObjectStorageResponseTypeDef",
+CreateLocationObjectStorageResponseOutputTypeDef = TypedDict(
+    "CreateLocationObjectStorageResponseOutputTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 S3ConfigTypeDef = TypedDict(
     "S3ConfigTypeDef",
     {
         "BucketAccessRoleArn": str,
     },
 )
 
-CreateLocationS3ResponseTypeDef = TypedDict(
-    "CreateLocationS3ResponseTypeDef",
+CreateLocationS3ResponseOutputTypeDef = TypedDict(
+    "CreateLocationS3ResponseOutputTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SmbMountOptionsTypeDef = TypedDict(
     "SmbMountOptionsTypeDef",
     {
         "Version": SmbVersionType,
     },
     total=False,
 )
 
-CreateLocationSmbResponseTypeDef = TypedDict(
-    "CreateLocationSmbResponseTypeDef",
+CreateLocationSmbResponseOutputTypeDef = TypedDict(
+    "CreateLocationSmbResponseOutputTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FilterRuleTypeDef = TypedDict(
@@ -469,16 +479,16 @@
 TaskScheduleTypeDef = TypedDict(
     "TaskScheduleTypeDef",
     {
         "ScheduleExpression": str,
     },
 )
 
-CreateTaskResponseTypeDef = TypedDict(
-    "CreateTaskResponseTypeDef",
+CreateTaskResponseOutputTypeDef = TypedDict(
+    "CreateTaskResponseOutputTypeDef",
     {
         "TaskArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteAgentRequestRequestTypeDef = TypedDict(
@@ -505,16 +515,16 @@
 DescribeAgentRequestRequestTypeDef = TypedDict(
     "DescribeAgentRequestRequestTypeDef",
     {
         "AgentArn": str,
     },
 )
 
-PrivateLinkConfigTypeDef = TypedDict(
-    "PrivateLinkConfigTypeDef",
+PrivateLinkConfigOutputTypeDef = TypedDict(
+    "PrivateLinkConfigOutputTypeDef",
     {
         "VpcEndpointId": str,
         "PrivateLinkEndpoint": str,
         "SubnetArns": List[str],
         "SecurityGroupArns": List[str],
     },
 )
@@ -522,16 +532,16 @@
 DescribeDiscoveryJobRequestRequestTypeDef = TypedDict(
     "DescribeDiscoveryJobRequestRequestTypeDef",
     {
         "DiscoveryJobArn": str,
     },
 )
 
-DescribeDiscoveryJobResponseTypeDef = TypedDict(
-    "DescribeDiscoveryJobResponseTypeDef",
+DescribeDiscoveryJobResponseOutputTypeDef = TypedDict(
+    "DescribeDiscoveryJobResponseOutputTypeDef",
     {
         "StorageSystemArn": str,
         "DiscoveryJobArn": str,
         "CollectionDurationMinutes": int,
         "Status": DiscoveryJobStatusType,
         "JobStartTime": datetime,
         "JobEndTime": datetime,
@@ -542,23 +552,31 @@
 DescribeLocationEfsRequestRequestTypeDef = TypedDict(
     "DescribeLocationEfsRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
+Ec2ConfigOutputTypeDef = TypedDict(
+    "Ec2ConfigOutputTypeDef",
+    {
+        "SubnetArn": str,
+        "SecurityGroupArns": List[str],
+    },
+)
+
 DescribeLocationFsxLustreRequestRequestTypeDef = TypedDict(
     "DescribeLocationFsxLustreRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
-DescribeLocationFsxLustreResponseTypeDef = TypedDict(
-    "DescribeLocationFsxLustreResponseTypeDef",
+DescribeLocationFsxLustreResponseOutputTypeDef = TypedDict(
+    "DescribeLocationFsxLustreResponseOutputTypeDef",
     {
         "LocationArn": str,
         "LocationUri": str,
         "SecurityGroupArns": List[str],
         "CreationTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -581,16 +599,16 @@
 DescribeLocationFsxWindowsRequestRequestTypeDef = TypedDict(
     "DescribeLocationFsxWindowsRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
-DescribeLocationFsxWindowsResponseTypeDef = TypedDict(
-    "DescribeLocationFsxWindowsResponseTypeDef",
+DescribeLocationFsxWindowsResponseOutputTypeDef = TypedDict(
+    "DescribeLocationFsxWindowsResponseOutputTypeDef",
     {
         "LocationArn": str,
         "LocationUri": str,
         "SecurityGroupArns": List[str],
         "CreationTime": datetime,
         "User": str,
         "Domain": str,
@@ -601,30 +619,60 @@
 DescribeLocationHdfsRequestRequestTypeDef = TypedDict(
     "DescribeLocationHdfsRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
+HdfsNameNodeOutputTypeDef = TypedDict(
+    "HdfsNameNodeOutputTypeDef",
+    {
+        "Hostname": str,
+        "Port": int,
+    },
+)
+
+QopConfigurationOutputTypeDef = TypedDict(
+    "QopConfigurationOutputTypeDef",
+    {
+        "RpcProtection": HdfsRpcProtectionType,
+        "DataTransferProtection": HdfsDataTransferProtectionType,
+    },
+)
+
 DescribeLocationNfsRequestRequestTypeDef = TypedDict(
     "DescribeLocationNfsRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
+NfsMountOptionsOutputTypeDef = TypedDict(
+    "NfsMountOptionsOutputTypeDef",
+    {
+        "Version": NfsVersionType,
+    },
+)
+
+OnPremConfigOutputTypeDef = TypedDict(
+    "OnPremConfigOutputTypeDef",
+    {
+        "AgentArns": List[str],
+    },
+)
+
 DescribeLocationObjectStorageRequestRequestTypeDef = TypedDict(
     "DescribeLocationObjectStorageRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
-DescribeLocationObjectStorageResponseTypeDef = TypedDict(
-    "DescribeLocationObjectStorageResponseTypeDef",
+DescribeLocationObjectStorageResponseOutputTypeDef = TypedDict(
+    "DescribeLocationObjectStorageResponseOutputTypeDef",
     {
         "LocationArn": str,
         "LocationUri": str,
         "AccessKey": str,
         "ServerPort": int,
         "ServerProtocol": ObjectStorageServerProtocolType,
         "AgentArns": List[str],
@@ -637,21 +685,35 @@
 DescribeLocationS3RequestRequestTypeDef = TypedDict(
     "DescribeLocationS3RequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
+S3ConfigOutputTypeDef = TypedDict(
+    "S3ConfigOutputTypeDef",
+    {
+        "BucketAccessRoleArn": str,
+    },
+)
+
 DescribeLocationSmbRequestRequestTypeDef = TypedDict(
     "DescribeLocationSmbRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
+SmbMountOptionsOutputTypeDef = TypedDict(
+    "SmbMountOptionsOutputTypeDef",
+    {
+        "Version": SmbVersionType,
+    },
+)
+
 DescribeStorageSystemRequestRequestTypeDef = TypedDict(
     "DescribeStorageSystemRequestRequestTypeDef",
     {
         "StorageSystemArn": str,
     },
 )
 
@@ -669,22 +731,20 @@
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class DescribeStorageSystemResourceMetricsRequestDescribeStorageSystemResourceMetricsPaginateTypeDef(
     _RequiredDescribeStorageSystemResourceMetricsRequestDescribeStorageSystemResourceMetricsPaginateTypeDef,
     _OptionalDescribeStorageSystemResourceMetricsRequestDescribeStorageSystemResourceMetricsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeStorageSystemResourceMetricsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeStorageSystemResourceMetricsRequestRequestTypeDef",
     {
         "DiscoveryJobArn": str,
         "ResourceType": DiscoveryResourceTypeType,
         "ResourceId": str,
     },
@@ -696,22 +756,20 @@
         "EndTime": Union[datetime, str],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeStorageSystemResourceMetricsRequestRequestTypeDef(
     _RequiredDescribeStorageSystemResourceMetricsRequestRequestTypeDef,
     _OptionalDescribeStorageSystemResourceMetricsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeStorageSystemResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeStorageSystemResourcesRequestRequestTypeDef",
     {
         "DiscoveryJobArn": str,
         "ResourceType": DiscoveryResourceTypeType,
     },
 )
@@ -722,31 +780,66 @@
         "Filter": Mapping[Literal["SVM"], Sequence[str]],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeStorageSystemResourcesRequestRequestTypeDef(
     _RequiredDescribeStorageSystemResourcesRequestRequestTypeDef,
     _OptionalDescribeStorageSystemResourcesRequestRequestTypeDef,
 ):
     pass
 
+DiscoveryServerConfigurationOutputTypeDef = TypedDict(
+    "DiscoveryServerConfigurationOutputTypeDef",
+    {
+        "ServerHostname": str,
+        "ServerPort": int,
+    },
+)
 
 DescribeTaskExecutionRequestRequestTypeDef = TypedDict(
     "DescribeTaskExecutionRequestRequestTypeDef",
     {
         "TaskExecutionArn": str,
     },
 )
 
-TaskExecutionResultDetailTypeDef = TypedDict(
-    "TaskExecutionResultDetailTypeDef",
+FilterRuleOutputTypeDef = TypedDict(
+    "FilterRuleOutputTypeDef",
+    {
+        "FilterType": Literal["SIMPLE_PATTERN"],
+        "Value": str,
+    },
+)
+
+OptionsOutputTypeDef = TypedDict(
+    "OptionsOutputTypeDef",
+    {
+        "VerifyMode": VerifyModeType,
+        "OverwriteMode": OverwriteModeType,
+        "Atime": AtimeType,
+        "Mtime": MtimeType,
+        "Uid": UidType,
+        "Gid": GidType,
+        "PreserveDeletedFiles": PreserveDeletedFilesType,
+        "PreserveDevices": PreserveDevicesType,
+        "PosixPermissions": PosixPermissionsType,
+        "BytesPerSecond": int,
+        "TaskQueueing": TaskQueueingType,
+        "LogLevel": LogLevelType,
+        "TransferMode": TransferModeType,
+        "SecurityDescriptorCopyFlags": SmbSecurityDescriptorCopyFlagsType,
+        "ObjectTags": ObjectTagsType,
+    },
+)
+
+TaskExecutionResultDetailOutputTypeDef = TypedDict(
+    "TaskExecutionResultDetailOutputTypeDef",
     {
         "PrepareDuration": int,
         "PrepareStatus": PhaseStatusType,
         "TotalDuration": int,
         "TransferDuration": int,
         "TransferStatus": PhaseStatusType,
         "VerifyDuration": int,
@@ -759,16 +852,23 @@
 DescribeTaskRequestRequestTypeDef = TypedDict(
     "DescribeTaskRequestRequestTypeDef",
     {
         "TaskArn": str,
     },
 )
 
-DiscoveryJobListEntryTypeDef = TypedDict(
-    "DiscoveryJobListEntryTypeDef",
+TaskScheduleOutputTypeDef = TypedDict(
+    "TaskScheduleOutputTypeDef",
+    {
+        "ScheduleExpression": str,
+    },
+)
+
+DiscoveryJobListEntryOutputTypeDef = TypedDict(
+    "DiscoveryJobListEntryOutputTypeDef",
     {
         "DiscoveryJobArn": str,
         "Status": DiscoveryJobStatusType,
     },
 )
 
 GenerateRecommendationsRequestRequestTypeDef = TypedDict(
@@ -776,26 +876,26 @@
     {
         "DiscoveryJobArn": str,
         "ResourceIds": Sequence[str],
         "ResourceType": DiscoveryResourceTypeType,
     },
 )
 
-IOPSTypeDef = TypedDict(
-    "IOPSTypeDef",
+IOPSOutputTypeDef = TypedDict(
+    "IOPSOutputTypeDef",
     {
         "Read": float,
         "Write": float,
         "Other": float,
         "Total": float,
     },
 )
 
-LatencyTypeDef = TypedDict(
-    "LatencyTypeDef",
+LatencyOutputTypeDef = TypedDict(
+    "LatencyOutputTypeDef",
     {
         "Read": float,
         "Write": float,
         "Other": float,
     },
 )
 
@@ -840,16 +940,16 @@
     {
         "Name": LocationFilterNameType,
         "Values": Sequence[str],
         "Operator": OperatorType,
     },
 )
 
-LocationListEntryTypeDef = TypedDict(
-    "LocationListEntryTypeDef",
+LocationListEntryOutputTypeDef = TypedDict(
+    "LocationListEntryOutputTypeDef",
     {
         "LocationArn": str,
         "LocationUri": str,
     },
 )
 
 ListStorageSystemsRequestListStorageSystemsPaginateTypeDef = TypedDict(
@@ -865,16 +965,16 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-StorageSystemListEntryTypeDef = TypedDict(
-    "StorageSystemListEntryTypeDef",
+StorageSystemListEntryOutputTypeDef = TypedDict(
+    "StorageSystemListEntryOutputTypeDef",
     {
         "StorageSystemArn": str,
         "Name": str,
     },
 )
 
 _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
@@ -887,22 +987,20 @@
     "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
     _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
 ):
     pass
 
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -910,21 +1008,27 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
+TagListEntryOutputTypeDef = TypedDict(
+    "TagListEntryOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
 
 ListTaskExecutionsRequestListTaskExecutionsPaginateTypeDef = TypedDict(
     "ListTaskExecutionsRequestListTaskExecutionsPaginateTypeDef",
     {
         "TaskArn": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
@@ -937,16 +1041,16 @@
         "TaskArn": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-TaskExecutionListEntryTypeDef = TypedDict(
-    "TaskExecutionListEntryTypeDef",
+TaskExecutionListEntryOutputTypeDef = TypedDict(
+    "TaskExecutionListEntryOutputTypeDef",
     {
         "TaskExecutionArn": str,
         "Status": TaskExecutionStatusType,
     },
 )
 
 TaskFilterTypeDef = TypedDict(
@@ -954,25 +1058,25 @@
     {
         "Name": TaskFilterNameType,
         "Values": Sequence[str],
         "Operator": OperatorType,
     },
 )
 
-TaskListEntryTypeDef = TypedDict(
-    "TaskListEntryTypeDef",
+TaskListEntryOutputTypeDef = TypedDict(
+    "TaskListEntryOutputTypeDef",
     {
         "TaskArn": str,
         "Status": TaskStatusType,
         "Name": str,
     },
 )
 
-MaxP95PerformanceTypeDef = TypedDict(
-    "MaxP95PerformanceTypeDef",
+MaxP95PerformanceOutputTypeDef = TypedDict(
+    "MaxP95PerformanceOutputTypeDef",
     {
         "IopsRead": float,
         "IopsWrite": float,
         "IopsOther": float,
         "IopsTotal": float,
         "ThroughputRead": float,
         "ThroughputWrite": float,
@@ -980,25 +1084,25 @@
         "ThroughputTotal": float,
         "LatencyRead": float,
         "LatencyWrite": float,
         "LatencyOther": float,
     },
 )
 
-RecommendationTypeDef = TypedDict(
-    "RecommendationTypeDef",
+RecommendationOutputTypeDef = TypedDict(
+    "RecommendationOutputTypeDef",
     {
         "StorageType": str,
         "StorageConfiguration": Dict[str, str],
         "EstimatedMonthlyStorageCost": str,
     },
 )
 
-ThroughputTypeDef = TypedDict(
-    "ThroughputTypeDef",
+ThroughputOutputTypeDef = TypedDict(
+    "ThroughputOutputTypeDef",
     {
         "Read": float,
         "Write": float,
         "Other": float,
         "Total": float,
     },
 )
@@ -1027,24 +1131,24 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-StartDiscoveryJobResponseTypeDef = TypedDict(
-    "StartDiscoveryJobResponseTypeDef",
+StartDiscoveryJobResponseOutputTypeDef = TypedDict(
+    "StartDiscoveryJobResponseOutputTypeDef",
     {
         "DiscoveryJobArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartTaskExecutionResponseTypeDef = TypedDict(
-    "StartTaskExecutionResponseTypeDef",
+StartTaskExecutionResponseOutputTypeDef = TypedDict(
+    "StartTaskExecutionResponseOutputTypeDef",
     {
         "TaskExecutionArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopDiscoveryJobRequestRequestTypeDef = TypedDict(
@@ -1072,21 +1176,19 @@
     "_OptionalUpdateAgentRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-
 class UpdateAgentRequestRequestTypeDef(
     _RequiredUpdateAgentRequestRequestTypeDef, _OptionalUpdateAgentRequestRequestTypeDef
 ):
     pass
 
-
 UpdateDiscoveryJobRequestRequestTypeDef = TypedDict(
     "UpdateDiscoveryJobRequestRequestTypeDef",
     {
         "DiscoveryJobArn": str,
         "CollectionDurationMinutes": int,
     },
 )
@@ -1107,39 +1209,20 @@
         "SecretKey": str,
         "AgentArns": Sequence[str],
         "ServerCertificate": Union[str, bytes, IO[Any], StreamingBody],
     },
     total=False,
 )
 
-
 class UpdateLocationObjectStorageRequestRequestTypeDef(
     _RequiredUpdateLocationObjectStorageRequestRequestTypeDef,
     _OptionalUpdateLocationObjectStorageRequestRequestTypeDef,
 ):
     pass
 
-
-DescribeStorageSystemResponseTypeDef = TypedDict(
-    "DescribeStorageSystemResponseTypeDef",
-    {
-        "StorageSystemArn": str,
-        "ServerConfiguration": DiscoveryServerConfigurationTypeDef,
-        "SystemType": Literal["NetAppONTAP"],
-        "AgentArns": List[str],
-        "Name": str,
-        "ErrorMessage": str,
-        "ConnectivityStatus": StorageSystemConnectivityStatusType,
-        "CloudWatchLogGroupArn": str,
-        "CreationTime": datetime,
-        "SecretsManagerArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateStorageSystemRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStorageSystemRequestRequestTypeDef",
     {
         "StorageSystemArn": str,
     },
 )
 _OptionalUpdateStorageSystemRequestRequestTypeDef = TypedDict(
@@ -1150,22 +1233,20 @@
         "Name": str,
         "CloudWatchLogGroupArn": str,
         "Credentials": CredentialsTypeDef,
     },
     total=False,
 )
 
-
 class UpdateStorageSystemRequestRequestTypeDef(
     _RequiredUpdateStorageSystemRequestRequestTypeDef,
     _OptionalUpdateStorageSystemRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredAddStorageSystemRequestRequestTypeDef = TypedDict(
     "_RequiredAddStorageSystemRequestRequestTypeDef",
     {
         "ServerConfiguration": DiscoveryServerConfigurationTypeDef,
         "SystemType": Literal["NetAppONTAP"],
         "AgentArns": Sequence[str],
         "ClientToken": str,
@@ -1178,21 +1259,19 @@
         "CloudWatchLogGroupArn": str,
         "Tags": Sequence[TagListEntryTypeDef],
         "Name": str,
     },
     total=False,
 )
 
-
 class AddStorageSystemRequestRequestTypeDef(
     _RequiredAddStorageSystemRequestRequestTypeDef, _OptionalAddStorageSystemRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateAgentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAgentRequestRequestTypeDef",
     {
         "ActivationKey": str,
     },
 )
 _OptionalCreateAgentRequestRequestTypeDef = TypedDict(
@@ -1203,21 +1282,19 @@
         "VpcEndpointId": str,
         "SubnetArns": Sequence[str],
         "SecurityGroupArns": Sequence[str],
     },
     total=False,
 )
 
-
 class CreateAgentRequestRequestTypeDef(
     _RequiredCreateAgentRequestRequestTypeDef, _OptionalCreateAgentRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateLocationFsxLustreRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLocationFsxLustreRequestRequestTypeDef",
     {
         "FsxFilesystemArn": str,
         "SecurityGroupArns": Sequence[str],
     },
 )
@@ -1226,22 +1303,20 @@
     {
         "Subdirectory": str,
         "Tags": Sequence[TagListEntryTypeDef],
     },
     total=False,
 )
 
-
 class CreateLocationFsxLustreRequestRequestTypeDef(
     _RequiredCreateLocationFsxLustreRequestRequestTypeDef,
     _OptionalCreateLocationFsxLustreRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateLocationFsxWindowsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLocationFsxWindowsRequestRequestTypeDef",
     {
         "FsxFilesystemArn": str,
         "SecurityGroupArns": Sequence[str],
         "User": str,
         "Password": str,
@@ -1253,22 +1328,20 @@
         "Subdirectory": str,
         "Tags": Sequence[TagListEntryTypeDef],
         "Domain": str,
     },
     total=False,
 )
 
-
 class CreateLocationFsxWindowsRequestRequestTypeDef(
     _RequiredCreateLocationFsxWindowsRequestRequestTypeDef,
     _OptionalCreateLocationFsxWindowsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateLocationObjectStorageRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLocationObjectStorageRequestRequestTypeDef",
     {
         "ServerHostname": str,
         "BucketName": str,
         "AgentArns": Sequence[str],
     },
@@ -1283,31 +1356,20 @@
         "SecretKey": str,
         "Tags": Sequence[TagListEntryTypeDef],
         "ServerCertificate": Union[str, bytes, IO[Any], StreamingBody],
     },
     total=False,
 )
 
-
 class CreateLocationObjectStorageRequestRequestTypeDef(
     _RequiredCreateLocationObjectStorageRequestRequestTypeDef,
     _OptionalCreateLocationObjectStorageRequestRequestTypeDef,
 ):
     pass
 
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagListEntryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStartDiscoveryJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartDiscoveryJobRequestRequestTypeDef",
     {
         "StorageSystemArn": str,
         "CollectionDurationMinutes": int,
         "ClientToken": str,
     },
@@ -1316,33 +1378,31 @@
     "_OptionalStartDiscoveryJobRequestRequestTypeDef",
     {
         "Tags": Sequence[TagListEntryTypeDef],
     },
     total=False,
 )
 
-
 class StartDiscoveryJobRequestRequestTypeDef(
     _RequiredStartDiscoveryJobRequestRequestTypeDef, _OptionalStartDiscoveryJobRequestRequestTypeDef
 ):
     pass
 
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagListEntryTypeDef],
     },
 )
 
-ListAgentsResponseTypeDef = TypedDict(
-    "ListAgentsResponseTypeDef",
+ListAgentsResponseOutputTypeDef = TypedDict(
+    "ListAgentsResponseOutputTypeDef",
     {
-        "Agents": List[AgentListEntryTypeDef],
+        "Agents": List[AgentListEntryOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateLocationEfsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLocationEfsRequestRequestTypeDef",
@@ -1359,35 +1419,19 @@
         "AccessPointArn": str,
         "FileSystemAccessRoleArn": str,
         "InTransitEncryption": EfsInTransitEncryptionType,
     },
     total=False,
 )
 
-
 class CreateLocationEfsRequestRequestTypeDef(
     _RequiredCreateLocationEfsRequestRequestTypeDef, _OptionalCreateLocationEfsRequestRequestTypeDef
 ):
     pass
 
-
-DescribeLocationEfsResponseTypeDef = TypedDict(
-    "DescribeLocationEfsResponseTypeDef",
-    {
-        "LocationArn": str,
-        "LocationUri": str,
-        "Ec2Config": Ec2ConfigTypeDef,
-        "CreationTime": datetime,
-        "AccessPointArn": str,
-        "FileSystemAccessRoleArn": str,
-        "InTransitEncryption": EfsInTransitEncryptionType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateLocationHdfsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLocationHdfsRequestRequestTypeDef",
     {
         "NameNodes": Sequence[HdfsNameNodeTypeDef],
         "AuthenticationType": HdfsAuthenticationTypeType,
         "AgentArns": Sequence[str],
     },
@@ -1405,41 +1449,20 @@
         "KerberosKeytab": Union[str, bytes, IO[Any], StreamingBody],
         "KerberosKrb5Conf": Union[str, bytes, IO[Any], StreamingBody],
         "Tags": Sequence[TagListEntryTypeDef],
     },
     total=False,
 )
 
-
 class CreateLocationHdfsRequestRequestTypeDef(
     _RequiredCreateLocationHdfsRequestRequestTypeDef,
     _OptionalCreateLocationHdfsRequestRequestTypeDef,
 ):
     pass
 
-
-DescribeLocationHdfsResponseTypeDef = TypedDict(
-    "DescribeLocationHdfsResponseTypeDef",
-    {
-        "LocationArn": str,
-        "LocationUri": str,
-        "NameNodes": List[HdfsNameNodeTypeDef],
-        "BlockSize": int,
-        "ReplicationFactor": int,
-        "KmsKeyProviderUri": str,
-        "QopConfiguration": QopConfigurationTypeDef,
-        "AuthenticationType": HdfsAuthenticationTypeType,
-        "SimpleUser": str,
-        "KerberosPrincipal": str,
-        "AgentArns": List[str],
-        "CreationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateLocationHdfsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLocationHdfsRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 _OptionalUpdateLocationHdfsRequestRequestTypeDef = TypedDict(
@@ -1457,22 +1480,20 @@
         "KerberosKeytab": Union[str, bytes, IO[Any], StreamingBody],
         "KerberosKrb5Conf": Union[str, bytes, IO[Any], StreamingBody],
         "AgentArns": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdateLocationHdfsRequestRequestTypeDef(
     _RequiredUpdateLocationHdfsRequestRequestTypeDef,
     _OptionalUpdateLocationHdfsRequestRequestTypeDef,
 ):
     pass
 
-
 FsxProtocolNfsTypeDef = TypedDict(
     "FsxProtocolNfsTypeDef",
     {
         "MountOptions": NfsMountOptionsTypeDef,
     },
     total=False,
 )
@@ -1490,33 +1511,19 @@
     {
         "MountOptions": NfsMountOptionsTypeDef,
         "Tags": Sequence[TagListEntryTypeDef],
     },
     total=False,
 )
 
-
 class CreateLocationNfsRequestRequestTypeDef(
     _RequiredCreateLocationNfsRequestRequestTypeDef, _OptionalCreateLocationNfsRequestRequestTypeDef
 ):
     pass
 
-
-DescribeLocationNfsResponseTypeDef = TypedDict(
-    "DescribeLocationNfsResponseTypeDef",
-    {
-        "LocationArn": str,
-        "LocationUri": str,
-        "OnPremConfig": OnPremConfigTypeDef,
-        "MountOptions": NfsMountOptionsTypeDef,
-        "CreationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateLocationNfsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLocationNfsRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 _OptionalUpdateLocationNfsRequestRequestTypeDef = TypedDict(
@@ -1525,21 +1532,19 @@
         "Subdirectory": str,
         "OnPremConfig": OnPremConfigTypeDef,
         "MountOptions": NfsMountOptionsTypeDef,
     },
     total=False,
 )
 
-
 class UpdateLocationNfsRequestRequestTypeDef(
     _RequiredUpdateLocationNfsRequestRequestTypeDef, _OptionalUpdateLocationNfsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateLocationS3RequestRequestTypeDef = TypedDict(
     "_RequiredCreateLocationS3RequestRequestTypeDef",
     {
         "S3BucketArn": str,
         "S3Config": S3ConfigTypeDef,
     },
 )
@@ -1550,34 +1555,19 @@
         "S3StorageClass": S3StorageClassType,
         "AgentArns": Sequence[str],
         "Tags": Sequence[TagListEntryTypeDef],
     },
     total=False,
 )
 
-
 class CreateLocationS3RequestRequestTypeDef(
     _RequiredCreateLocationS3RequestRequestTypeDef, _OptionalCreateLocationS3RequestRequestTypeDef
 ):
     pass
 
-
-DescribeLocationS3ResponseTypeDef = TypedDict(
-    "DescribeLocationS3ResponseTypeDef",
-    {
-        "LocationArn": str,
-        "LocationUri": str,
-        "S3StorageClass": S3StorageClassType,
-        "S3Config": S3ConfigTypeDef,
-        "AgentArns": List[str],
-        "CreationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateLocationSmbRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLocationSmbRequestRequestTypeDef",
     {
         "Subdirectory": str,
         "ServerHostname": str,
         "User": str,
         "Password": str,
@@ -1590,35 +1580,19 @@
         "Domain": str,
         "MountOptions": SmbMountOptionsTypeDef,
         "Tags": Sequence[TagListEntryTypeDef],
     },
     total=False,
 )
 
-
 class CreateLocationSmbRequestRequestTypeDef(
     _RequiredCreateLocationSmbRequestRequestTypeDef, _OptionalCreateLocationSmbRequestRequestTypeDef
 ):
     pass
 
-
-DescribeLocationSmbResponseTypeDef = TypedDict(
-    "DescribeLocationSmbResponseTypeDef",
-    {
-        "LocationArn": str,
-        "LocationUri": str,
-        "AgentArns": List[str],
-        "User": str,
-        "Domain": str,
-        "MountOptions": SmbMountOptionsTypeDef,
-        "CreationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredFsxProtocolSmbTypeDef = TypedDict(
     "_RequiredFsxProtocolSmbTypeDef",
     {
         "Password": str,
         "User": str,
     },
 )
@@ -1627,19 +1601,17 @@
     {
         "Domain": str,
         "MountOptions": SmbMountOptionsTypeDef,
     },
     total=False,
 )
 
-
 class FsxProtocolSmbTypeDef(_RequiredFsxProtocolSmbTypeDef, _OptionalFsxProtocolSmbTypeDef):
     pass
 
-
 _RequiredUpdateLocationSmbRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLocationSmbRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 _OptionalUpdateLocationSmbRequestRequestTypeDef = TypedDict(
@@ -1651,21 +1623,19 @@
         "Password": str,
         "AgentArns": Sequence[str],
         "MountOptions": SmbMountOptionsTypeDef,
     },
     total=False,
 )
 
-
 class UpdateLocationSmbRequestRequestTypeDef(
     _RequiredUpdateLocationSmbRequestRequestTypeDef, _OptionalUpdateLocationSmbRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredStartTaskExecutionRequestRequestTypeDef = TypedDict(
     "_RequiredStartTaskExecutionRequestRequestTypeDef",
     {
         "TaskArn": str,
     },
 )
 _OptionalStartTaskExecutionRequestRequestTypeDef = TypedDict(
@@ -1675,22 +1645,20 @@
         "Includes": Sequence[FilterRuleTypeDef],
         "Excludes": Sequence[FilterRuleTypeDef],
         "Tags": Sequence[TagListEntryTypeDef],
     },
     total=False,
 )
 
-
 class StartTaskExecutionRequestRequestTypeDef(
     _RequiredStartTaskExecutionRequestRequestTypeDef,
     _OptionalStartTaskExecutionRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateTaskExecutionRequestRequestTypeDef = TypedDict(
     "UpdateTaskExecutionRequestRequestTypeDef",
     {
         "TaskExecutionArn": str,
         "Options": OptionsTypeDef,
     },
 )
@@ -1712,44 +1680,19 @@
         "Schedule": TaskScheduleTypeDef,
         "Tags": Sequence[TagListEntryTypeDef],
         "Includes": Sequence[FilterRuleTypeDef],
     },
     total=False,
 )
 
-
 class CreateTaskRequestRequestTypeDef(
     _RequiredCreateTaskRequestRequestTypeDef, _OptionalCreateTaskRequestRequestTypeDef
 ):
     pass
 
-
-DescribeTaskResponseTypeDef = TypedDict(
-    "DescribeTaskResponseTypeDef",
-    {
-        "TaskArn": str,
-        "Status": TaskStatusType,
-        "Name": str,
-        "CurrentTaskExecutionArn": str,
-        "SourceLocationArn": str,
-        "DestinationLocationArn": str,
-        "CloudWatchLogGroupArn": str,
-        "SourceNetworkInterfaceArns": List[str],
-        "DestinationNetworkInterfaceArns": List[str],
-        "Options": OptionsTypeDef,
-        "Excludes": List[FilterRuleTypeDef],
-        "Schedule": TaskScheduleTypeDef,
-        "ErrorCode": str,
-        "ErrorDetail": str,
-        "CreationTime": datetime,
-        "Includes": List[FilterRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateTaskRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTaskRequestRequestTypeDef",
     {
         "TaskArn": str,
     },
 )
 _OptionalUpdateTaskRequestRequestTypeDef = TypedDict(
@@ -1761,59 +1704,186 @@
         "Name": str,
         "CloudWatchLogGroupArn": str,
         "Includes": Sequence[FilterRuleTypeDef],
     },
     total=False,
 )
 
-
 class UpdateTaskRequestRequestTypeDef(
     _RequiredUpdateTaskRequestRequestTypeDef, _OptionalUpdateTaskRequestRequestTypeDef
 ):
     pass
 
-
-DescribeAgentResponseTypeDef = TypedDict(
-    "DescribeAgentResponseTypeDef",
+DescribeAgentResponseOutputTypeDef = TypedDict(
+    "DescribeAgentResponseOutputTypeDef",
     {
         "AgentArn": str,
         "Name": str,
         "Status": AgentStatusType,
         "LastConnectionTime": datetime,
         "CreationTime": datetime,
         "EndpointType": EndpointTypeType,
-        "PrivateLinkConfig": PrivateLinkConfigTypeDef,
+        "PrivateLinkConfig": PrivateLinkConfigOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeLocationEfsResponseOutputTypeDef = TypedDict(
+    "DescribeLocationEfsResponseOutputTypeDef",
+    {
+        "LocationArn": str,
+        "LocationUri": str,
+        "Ec2Config": Ec2ConfigOutputTypeDef,
+        "CreationTime": datetime,
+        "AccessPointArn": str,
+        "FileSystemAccessRoleArn": str,
+        "InTransitEncryption": EfsInTransitEncryptionType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeLocationHdfsResponseOutputTypeDef = TypedDict(
+    "DescribeLocationHdfsResponseOutputTypeDef",
+    {
+        "LocationArn": str,
+        "LocationUri": str,
+        "NameNodes": List[HdfsNameNodeOutputTypeDef],
+        "BlockSize": int,
+        "ReplicationFactor": int,
+        "KmsKeyProviderUri": str,
+        "QopConfiguration": QopConfigurationOutputTypeDef,
+        "AuthenticationType": HdfsAuthenticationTypeType,
+        "SimpleUser": str,
+        "KerberosPrincipal": str,
+        "AgentArns": List[str],
+        "CreationTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+FsxProtocolNfsOutputTypeDef = TypedDict(
+    "FsxProtocolNfsOutputTypeDef",
+    {
+        "MountOptions": NfsMountOptionsOutputTypeDef,
+    },
+)
+
+DescribeLocationNfsResponseOutputTypeDef = TypedDict(
+    "DescribeLocationNfsResponseOutputTypeDef",
+    {
+        "LocationArn": str,
+        "LocationUri": str,
+        "OnPremConfig": OnPremConfigOutputTypeDef,
+        "MountOptions": NfsMountOptionsOutputTypeDef,
+        "CreationTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeLocationS3ResponseOutputTypeDef = TypedDict(
+    "DescribeLocationS3ResponseOutputTypeDef",
+    {
+        "LocationArn": str,
+        "LocationUri": str,
+        "S3StorageClass": S3StorageClassType,
+        "S3Config": S3ConfigOutputTypeDef,
+        "AgentArns": List[str],
+        "CreationTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeLocationSmbResponseOutputTypeDef = TypedDict(
+    "DescribeLocationSmbResponseOutputTypeDef",
+    {
+        "LocationArn": str,
+        "LocationUri": str,
+        "AgentArns": List[str],
+        "User": str,
+        "Domain": str,
+        "MountOptions": SmbMountOptionsOutputTypeDef,
+        "CreationTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeTaskExecutionResponseTypeDef = TypedDict(
-    "DescribeTaskExecutionResponseTypeDef",
+FsxProtocolSmbOutputTypeDef = TypedDict(
+    "FsxProtocolSmbOutputTypeDef",
+    {
+        "Domain": str,
+        "MountOptions": SmbMountOptionsOutputTypeDef,
+        "Password": str,
+        "User": str,
+    },
+)
+
+DescribeStorageSystemResponseOutputTypeDef = TypedDict(
+    "DescribeStorageSystemResponseOutputTypeDef",
+    {
+        "StorageSystemArn": str,
+        "ServerConfiguration": DiscoveryServerConfigurationOutputTypeDef,
+        "SystemType": Literal["NetAppONTAP"],
+        "AgentArns": List[str],
+        "Name": str,
+        "ErrorMessage": str,
+        "ConnectivityStatus": StorageSystemConnectivityStatusType,
+        "CloudWatchLogGroupArn": str,
+        "CreationTime": datetime,
+        "SecretsManagerArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeTaskExecutionResponseOutputTypeDef = TypedDict(
+    "DescribeTaskExecutionResponseOutputTypeDef",
     {
         "TaskExecutionArn": str,
         "Status": TaskExecutionStatusType,
-        "Options": OptionsTypeDef,
-        "Excludes": List[FilterRuleTypeDef],
-        "Includes": List[FilterRuleTypeDef],
+        "Options": OptionsOutputTypeDef,
+        "Excludes": List[FilterRuleOutputTypeDef],
+        "Includes": List[FilterRuleOutputTypeDef],
         "StartTime": datetime,
         "EstimatedFilesToTransfer": int,
         "EstimatedBytesToTransfer": int,
         "FilesTransferred": int,
         "BytesWritten": int,
         "BytesTransferred": int,
-        "Result": TaskExecutionResultDetailTypeDef,
+        "Result": TaskExecutionResultDetailOutputTypeDef,
         "BytesCompressed": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListDiscoveryJobsResponseTypeDef = TypedDict(
-    "ListDiscoveryJobsResponseTypeDef",
+DescribeTaskResponseOutputTypeDef = TypedDict(
+    "DescribeTaskResponseOutputTypeDef",
     {
-        "DiscoveryJobs": List[DiscoveryJobListEntryTypeDef],
+        "TaskArn": str,
+        "Status": TaskStatusType,
+        "Name": str,
+        "CurrentTaskExecutionArn": str,
+        "SourceLocationArn": str,
+        "DestinationLocationArn": str,
+        "CloudWatchLogGroupArn": str,
+        "SourceNetworkInterfaceArns": List[str],
+        "DestinationNetworkInterfaceArns": List[str],
+        "Options": OptionsOutputTypeDef,
+        "Excludes": List[FilterRuleOutputTypeDef],
+        "Schedule": TaskScheduleOutputTypeDef,
+        "ErrorCode": str,
+        "ErrorDetail": str,
+        "CreationTime": datetime,
+        "Includes": List[FilterRuleOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListDiscoveryJobsResponseOutputTypeDef = TypedDict(
+    "ListDiscoveryJobsResponseOutputTypeDef",
+    {
+        "DiscoveryJobs": List[DiscoveryJobListEntryOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLocationsRequestListLocationsPaginateTypeDef = TypedDict(
     "ListLocationsRequestListLocationsPaginateTypeDef",
@@ -1830,36 +1900,45 @@
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[LocationFilterTypeDef],
     },
     total=False,
 )
 
-ListLocationsResponseTypeDef = TypedDict(
-    "ListLocationsResponseTypeDef",
+ListLocationsResponseOutputTypeDef = TypedDict(
+    "ListLocationsResponseOutputTypeDef",
+    {
+        "Locations": List[LocationListEntryOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListStorageSystemsResponseOutputTypeDef = TypedDict(
+    "ListStorageSystemsResponseOutputTypeDef",
     {
-        "Locations": List[LocationListEntryTypeDef],
+        "StorageSystems": List[StorageSystemListEntryOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListStorageSystemsResponseTypeDef = TypedDict(
-    "ListStorageSystemsResponseTypeDef",
+ListTagsForResourceResponseOutputTypeDef = TypedDict(
+    "ListTagsForResourceResponseOutputTypeDef",
     {
-        "StorageSystems": List[StorageSystemListEntryTypeDef],
+        "Tags": List[TagListEntryOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTaskExecutionsResponseTypeDef = TypedDict(
-    "ListTaskExecutionsResponseTypeDef",
+ListTaskExecutionsResponseOutputTypeDef = TypedDict(
+    "ListTaskExecutionsResponseOutputTypeDef",
     {
-        "TaskExecutions": List[TaskExecutionListEntryTypeDef],
+        "TaskExecutions": List[TaskExecutionListEntryOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTasksRequestListTasksPaginateTypeDef = TypedDict(
     "ListTasksRequestListTasksPaginateTypeDef",
@@ -1876,114 +1955,122 @@
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[TaskFilterTypeDef],
     },
     total=False,
 )
 
-ListTasksResponseTypeDef = TypedDict(
-    "ListTasksResponseTypeDef",
+ListTasksResponseOutputTypeDef = TypedDict(
+    "ListTasksResponseOutputTypeDef",
     {
-        "Tasks": List[TaskListEntryTypeDef],
+        "Tasks": List[TaskListEntryOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-NetAppONTAPClusterTypeDef = TypedDict(
-    "NetAppONTAPClusterTypeDef",
+NetAppONTAPClusterOutputTypeDef = TypedDict(
+    "NetAppONTAPClusterOutputTypeDef",
     {
         "CifsShareCount": int,
         "NfsExportedVolumes": int,
         "ResourceId": str,
         "ClusterName": str,
-        "MaxP95Performance": MaxP95PerformanceTypeDef,
+        "MaxP95Performance": MaxP95PerformanceOutputTypeDef,
         "ClusterBlockStorageSize": int,
         "ClusterBlockStorageUsed": int,
         "ClusterBlockStorageLogicalUsed": int,
-        "Recommendations": List[RecommendationTypeDef],
+        "Recommendations": List[RecommendationOutputTypeDef],
         "RecommendationStatus": RecommendationStatusType,
         "LunCount": int,
     },
 )
 
-NetAppONTAPSVMTypeDef = TypedDict(
-    "NetAppONTAPSVMTypeDef",
+NetAppONTAPSVMOutputTypeDef = TypedDict(
+    "NetAppONTAPSVMOutputTypeDef",
     {
         "ClusterUuid": str,
         "ResourceId": str,
         "SvmName": str,
         "CifsShareCount": int,
         "EnabledProtocols": List[str],
         "TotalCapacityUsed": int,
         "TotalCapacityProvisioned": int,
         "TotalLogicalCapacityUsed": int,
-        "MaxP95Performance": MaxP95PerformanceTypeDef,
-        "Recommendations": List[RecommendationTypeDef],
+        "MaxP95Performance": MaxP95PerformanceOutputTypeDef,
+        "Recommendations": List[RecommendationOutputTypeDef],
         "NfsExportedVolumes": int,
         "RecommendationStatus": RecommendationStatusType,
         "TotalSnapshotCapacityUsed": int,
         "LunCount": int,
     },
 )
 
-NetAppONTAPVolumeTypeDef = TypedDict(
-    "NetAppONTAPVolumeTypeDef",
+NetAppONTAPVolumeOutputTypeDef = TypedDict(
+    "NetAppONTAPVolumeOutputTypeDef",
     {
         "VolumeName": str,
         "ResourceId": str,
         "CifsShareCount": int,
         "SecurityStyle": str,
         "SvmUuid": str,
         "SvmName": str,
         "CapacityUsed": int,
         "CapacityProvisioned": int,
         "LogicalCapacityUsed": int,
         "NfsExported": bool,
         "SnapshotCapacityUsed": int,
-        "MaxP95Performance": MaxP95PerformanceTypeDef,
-        "Recommendations": List[RecommendationTypeDef],
+        "MaxP95Performance": MaxP95PerformanceOutputTypeDef,
+        "Recommendations": List[RecommendationOutputTypeDef],
         "RecommendationStatus": RecommendationStatusType,
         "LunCount": int,
     },
 )
 
-P95MetricsTypeDef = TypedDict(
-    "P95MetricsTypeDef",
+P95MetricsOutputTypeDef = TypedDict(
+    "P95MetricsOutputTypeDef",
     {
-        "IOPS": IOPSTypeDef,
-        "Throughput": ThroughputTypeDef,
-        "Latency": LatencyTypeDef,
+        "IOPS": IOPSOutputTypeDef,
+        "Throughput": ThroughputOutputTypeDef,
+        "Latency": LatencyOutputTypeDef,
     },
 )
 
 FsxProtocolTypeDef = TypedDict(
     "FsxProtocolTypeDef",
     {
         "NFS": FsxProtocolNfsTypeDef,
         "SMB": FsxProtocolSmbTypeDef,
     },
     total=False,
 )
 
-ResourceDetailsTypeDef = TypedDict(
-    "ResourceDetailsTypeDef",
+FsxProtocolOutputTypeDef = TypedDict(
+    "FsxProtocolOutputTypeDef",
     {
-        "NetAppONTAPSVMs": List[NetAppONTAPSVMTypeDef],
-        "NetAppONTAPVolumes": List[NetAppONTAPVolumeTypeDef],
-        "NetAppONTAPClusters": List[NetAppONTAPClusterTypeDef],
+        "NFS": FsxProtocolNfsOutputTypeDef,
+        "SMB": FsxProtocolSmbOutputTypeDef,
     },
 )
 
-ResourceMetricsTypeDef = TypedDict(
-    "ResourceMetricsTypeDef",
+ResourceDetailsOutputTypeDef = TypedDict(
+    "ResourceDetailsOutputTypeDef",
+    {
+        "NetAppONTAPSVMs": List[NetAppONTAPSVMOutputTypeDef],
+        "NetAppONTAPVolumes": List[NetAppONTAPVolumeOutputTypeDef],
+        "NetAppONTAPClusters": List[NetAppONTAPClusterOutputTypeDef],
+    },
+)
+
+ResourceMetricsOutputTypeDef = TypedDict(
+    "ResourceMetricsOutputTypeDef",
     {
         "Timestamp": datetime,
-        "P95Metrics": P95MetricsTypeDef,
-        "Capacity": CapacityTypeDef,
+        "P95Metrics": P95MetricsOutputTypeDef,
+        "Capacity": CapacityOutputTypeDef,
         "ResourceId": str,
         "ResourceType": DiscoveryResourceTypeType,
     },
 )
 
 _RequiredCreateLocationFsxOntapRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLocationFsxOntapRequestRequestTypeDef",
@@ -1998,22 +2085,20 @@
     {
         "Subdirectory": str,
         "Tags": Sequence[TagListEntryTypeDef],
     },
     total=False,
 )
 
-
 class CreateLocationFsxOntapRequestRequestTypeDef(
     _RequiredCreateLocationFsxOntapRequestRequestTypeDef,
     _OptionalCreateLocationFsxOntapRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateLocationFsxOpenZfsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLocationFsxOpenZfsRequestRequestTypeDef",
     {
         "FsxFilesystemArn": str,
         "Protocol": FsxProtocolTypeDef,
         "SecurityGroupArns": Sequence[str],
     },
@@ -2023,58 +2108,56 @@
     {
         "Subdirectory": str,
         "Tags": Sequence[TagListEntryTypeDef],
     },
     total=False,
 )
 
-
 class CreateLocationFsxOpenZfsRequestRequestTypeDef(
     _RequiredCreateLocationFsxOpenZfsRequestRequestTypeDef,
     _OptionalCreateLocationFsxOpenZfsRequestRequestTypeDef,
 ):
     pass
 
-
-DescribeLocationFsxOntapResponseTypeDef = TypedDict(
-    "DescribeLocationFsxOntapResponseTypeDef",
+DescribeLocationFsxOntapResponseOutputTypeDef = TypedDict(
+    "DescribeLocationFsxOntapResponseOutputTypeDef",
     {
         "CreationTime": datetime,
         "LocationArn": str,
         "LocationUri": str,
-        "Protocol": FsxProtocolTypeDef,
+        "Protocol": FsxProtocolOutputTypeDef,
         "SecurityGroupArns": List[str],
         "StorageVirtualMachineArn": str,
         "FsxFilesystemArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeLocationFsxOpenZfsResponseTypeDef = TypedDict(
-    "DescribeLocationFsxOpenZfsResponseTypeDef",
+DescribeLocationFsxOpenZfsResponseOutputTypeDef = TypedDict(
+    "DescribeLocationFsxOpenZfsResponseOutputTypeDef",
     {
         "LocationArn": str,
         "LocationUri": str,
         "SecurityGroupArns": List[str],
-        "Protocol": FsxProtocolTypeDef,
+        "Protocol": FsxProtocolOutputTypeDef,
         "CreationTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeStorageSystemResourcesResponseTypeDef = TypedDict(
-    "DescribeStorageSystemResourcesResponseTypeDef",
+DescribeStorageSystemResourcesResponseOutputTypeDef = TypedDict(
+    "DescribeStorageSystemResourcesResponseOutputTypeDef",
     {
-        "ResourceDetails": ResourceDetailsTypeDef,
+        "ResourceDetails": ResourceDetailsOutputTypeDef,
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeStorageSystemResourceMetricsResponseTypeDef = TypedDict(
-    "DescribeStorageSystemResourceMetricsResponseTypeDef",
+DescribeStorageSystemResourceMetricsResponseOutputTypeDef = TypedDict(
+    "DescribeStorageSystemResourceMetricsResponseOutputTypeDef",
     {
-        "Metrics": List[ResourceMetricsTypeDef],
+        "Metrics": List[ResourceMetricsOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-datasync-1.28.3/mypy_boto3_datasync/type_defs.pyi` & `mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync/type_defs.py`

 * *Files 11% similar despite different names*

```diff
@@ -59,159 +59,175 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "CredentialsTypeDef",
     "DiscoveryServerConfigurationTypeDef",
     "TagListEntryTypeDef",
-    "AddStorageSystemResponseTypeDef",
-    "AgentListEntryTypeDef",
+    "AddStorageSystemResponseOutputTypeDef",
+    "AgentListEntryOutputTypeDef",
     "CancelTaskExecutionRequestRequestTypeDef",
-    "CapacityTypeDef",
-    "CreateAgentResponseTypeDef",
+    "CapacityOutputTypeDef",
+    "CreateAgentResponseOutputTypeDef",
     "Ec2ConfigTypeDef",
-    "CreateLocationEfsResponseTypeDef",
-    "CreateLocationFsxLustreResponseTypeDef",
-    "CreateLocationFsxOntapResponseTypeDef",
-    "CreateLocationFsxOpenZfsResponseTypeDef",
-    "CreateLocationFsxWindowsResponseTypeDef",
+    "CreateLocationEfsResponseOutputTypeDef",
+    "CreateLocationFsxLustreResponseOutputTypeDef",
+    "CreateLocationFsxOntapResponseOutputTypeDef",
+    "CreateLocationFsxOpenZfsResponseOutputTypeDef",
+    "CreateLocationFsxWindowsResponseOutputTypeDef",
     "HdfsNameNodeTypeDef",
     "QopConfigurationTypeDef",
-    "CreateLocationHdfsResponseTypeDef",
+    "CreateLocationHdfsResponseOutputTypeDef",
     "NfsMountOptionsTypeDef",
     "OnPremConfigTypeDef",
-    "CreateLocationNfsResponseTypeDef",
-    "CreateLocationObjectStorageResponseTypeDef",
+    "CreateLocationNfsResponseOutputTypeDef",
+    "CreateLocationObjectStorageResponseOutputTypeDef",
     "S3ConfigTypeDef",
-    "CreateLocationS3ResponseTypeDef",
+    "CreateLocationS3ResponseOutputTypeDef",
     "SmbMountOptionsTypeDef",
-    "CreateLocationSmbResponseTypeDef",
+    "CreateLocationSmbResponseOutputTypeDef",
     "FilterRuleTypeDef",
     "OptionsTypeDef",
     "TaskScheduleTypeDef",
-    "CreateTaskResponseTypeDef",
+    "CreateTaskResponseOutputTypeDef",
     "DeleteAgentRequestRequestTypeDef",
     "DeleteLocationRequestRequestTypeDef",
     "DeleteTaskRequestRequestTypeDef",
     "DescribeAgentRequestRequestTypeDef",
-    "PrivateLinkConfigTypeDef",
+    "PrivateLinkConfigOutputTypeDef",
     "DescribeDiscoveryJobRequestRequestTypeDef",
-    "DescribeDiscoveryJobResponseTypeDef",
+    "DescribeDiscoveryJobResponseOutputTypeDef",
     "DescribeLocationEfsRequestRequestTypeDef",
+    "Ec2ConfigOutputTypeDef",
     "DescribeLocationFsxLustreRequestRequestTypeDef",
-    "DescribeLocationFsxLustreResponseTypeDef",
+    "DescribeLocationFsxLustreResponseOutputTypeDef",
     "DescribeLocationFsxOntapRequestRequestTypeDef",
     "DescribeLocationFsxOpenZfsRequestRequestTypeDef",
     "DescribeLocationFsxWindowsRequestRequestTypeDef",
-    "DescribeLocationFsxWindowsResponseTypeDef",
+    "DescribeLocationFsxWindowsResponseOutputTypeDef",
     "DescribeLocationHdfsRequestRequestTypeDef",
+    "HdfsNameNodeOutputTypeDef",
+    "QopConfigurationOutputTypeDef",
     "DescribeLocationNfsRequestRequestTypeDef",
+    "NfsMountOptionsOutputTypeDef",
+    "OnPremConfigOutputTypeDef",
     "DescribeLocationObjectStorageRequestRequestTypeDef",
-    "DescribeLocationObjectStorageResponseTypeDef",
+    "DescribeLocationObjectStorageResponseOutputTypeDef",
     "DescribeLocationS3RequestRequestTypeDef",
+    "S3ConfigOutputTypeDef",
     "DescribeLocationSmbRequestRequestTypeDef",
+    "SmbMountOptionsOutputTypeDef",
     "DescribeStorageSystemRequestRequestTypeDef",
     "DescribeStorageSystemResourceMetricsRequestDescribeStorageSystemResourceMetricsPaginateTypeDef",
     "DescribeStorageSystemResourceMetricsRequestRequestTypeDef",
     "DescribeStorageSystemResourcesRequestRequestTypeDef",
+    "DiscoveryServerConfigurationOutputTypeDef",
     "DescribeTaskExecutionRequestRequestTypeDef",
-    "TaskExecutionResultDetailTypeDef",
+    "FilterRuleOutputTypeDef",
+    "OptionsOutputTypeDef",
+    "TaskExecutionResultDetailOutputTypeDef",
     "DescribeTaskRequestRequestTypeDef",
-    "DiscoveryJobListEntryTypeDef",
+    "TaskScheduleOutputTypeDef",
+    "DiscoveryJobListEntryOutputTypeDef",
     "GenerateRecommendationsRequestRequestTypeDef",
-    "IOPSTypeDef",
-    "LatencyTypeDef",
+    "IOPSOutputTypeDef",
+    "LatencyOutputTypeDef",
     "ListAgentsRequestListAgentsPaginateTypeDef",
     "ListAgentsRequestRequestTypeDef",
     "ListDiscoveryJobsRequestListDiscoveryJobsPaginateTypeDef",
     "ListDiscoveryJobsRequestRequestTypeDef",
     "LocationFilterTypeDef",
-    "LocationListEntryTypeDef",
+    "LocationListEntryOutputTypeDef",
     "ListStorageSystemsRequestListStorageSystemsPaginateTypeDef",
     "ListStorageSystemsRequestRequestTypeDef",
-    "StorageSystemListEntryTypeDef",
+    "StorageSystemListEntryOutputTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagListEntryOutputTypeDef",
     "ListTaskExecutionsRequestListTaskExecutionsPaginateTypeDef",
     "ListTaskExecutionsRequestRequestTypeDef",
-    "TaskExecutionListEntryTypeDef",
+    "TaskExecutionListEntryOutputTypeDef",
     "TaskFilterTypeDef",
-    "TaskListEntryTypeDef",
-    "MaxP95PerformanceTypeDef",
-    "RecommendationTypeDef",
-    "ThroughputTypeDef",
+    "TaskListEntryOutputTypeDef",
+    "MaxP95PerformanceOutputTypeDef",
+    "RecommendationOutputTypeDef",
+    "ThroughputOutputTypeDef",
     "PaginatorConfigTypeDef",
     "RemoveStorageSystemRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
-    "StartDiscoveryJobResponseTypeDef",
-    "StartTaskExecutionResponseTypeDef",
+    "StartDiscoveryJobResponseOutputTypeDef",
+    "StartTaskExecutionResponseOutputTypeDef",
     "StopDiscoveryJobRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAgentRequestRequestTypeDef",
     "UpdateDiscoveryJobRequestRequestTypeDef",
     "UpdateLocationObjectStorageRequestRequestTypeDef",
-    "DescribeStorageSystemResponseTypeDef",
     "UpdateStorageSystemRequestRequestTypeDef",
     "AddStorageSystemRequestRequestTypeDef",
     "CreateAgentRequestRequestTypeDef",
     "CreateLocationFsxLustreRequestRequestTypeDef",
     "CreateLocationFsxWindowsRequestRequestTypeDef",
     "CreateLocationObjectStorageRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "StartDiscoveryJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "ListAgentsResponseTypeDef",
+    "ListAgentsResponseOutputTypeDef",
     "CreateLocationEfsRequestRequestTypeDef",
-    "DescribeLocationEfsResponseTypeDef",
     "CreateLocationHdfsRequestRequestTypeDef",
-    "DescribeLocationHdfsResponseTypeDef",
     "UpdateLocationHdfsRequestRequestTypeDef",
     "FsxProtocolNfsTypeDef",
     "CreateLocationNfsRequestRequestTypeDef",
-    "DescribeLocationNfsResponseTypeDef",
     "UpdateLocationNfsRequestRequestTypeDef",
     "CreateLocationS3RequestRequestTypeDef",
-    "DescribeLocationS3ResponseTypeDef",
     "CreateLocationSmbRequestRequestTypeDef",
-    "DescribeLocationSmbResponseTypeDef",
     "FsxProtocolSmbTypeDef",
     "UpdateLocationSmbRequestRequestTypeDef",
     "StartTaskExecutionRequestRequestTypeDef",
     "UpdateTaskExecutionRequestRequestTypeDef",
     "CreateTaskRequestRequestTypeDef",
-    "DescribeTaskResponseTypeDef",
     "UpdateTaskRequestRequestTypeDef",
-    "DescribeAgentResponseTypeDef",
-    "DescribeTaskExecutionResponseTypeDef",
-    "ListDiscoveryJobsResponseTypeDef",
+    "DescribeAgentResponseOutputTypeDef",
+    "DescribeLocationEfsResponseOutputTypeDef",
+    "DescribeLocationHdfsResponseOutputTypeDef",
+    "FsxProtocolNfsOutputTypeDef",
+    "DescribeLocationNfsResponseOutputTypeDef",
+    "DescribeLocationS3ResponseOutputTypeDef",
+    "DescribeLocationSmbResponseOutputTypeDef",
+    "FsxProtocolSmbOutputTypeDef",
+    "DescribeStorageSystemResponseOutputTypeDef",
+    "DescribeTaskExecutionResponseOutputTypeDef",
+    "DescribeTaskResponseOutputTypeDef",
+    "ListDiscoveryJobsResponseOutputTypeDef",
     "ListLocationsRequestListLocationsPaginateTypeDef",
     "ListLocationsRequestRequestTypeDef",
-    "ListLocationsResponseTypeDef",
-    "ListStorageSystemsResponseTypeDef",
-    "ListTaskExecutionsResponseTypeDef",
+    "ListLocationsResponseOutputTypeDef",
+    "ListStorageSystemsResponseOutputTypeDef",
+    "ListTagsForResourceResponseOutputTypeDef",
+    "ListTaskExecutionsResponseOutputTypeDef",
     "ListTasksRequestListTasksPaginateTypeDef",
     "ListTasksRequestRequestTypeDef",
-    "ListTasksResponseTypeDef",
-    "NetAppONTAPClusterTypeDef",
-    "NetAppONTAPSVMTypeDef",
-    "NetAppONTAPVolumeTypeDef",
-    "P95MetricsTypeDef",
+    "ListTasksResponseOutputTypeDef",
+    "NetAppONTAPClusterOutputTypeDef",
+    "NetAppONTAPSVMOutputTypeDef",
+    "NetAppONTAPVolumeOutputTypeDef",
+    "P95MetricsOutputTypeDef",
     "FsxProtocolTypeDef",
-    "ResourceDetailsTypeDef",
-    "ResourceMetricsTypeDef",
+    "FsxProtocolOutputTypeDef",
+    "ResourceDetailsOutputTypeDef",
+    "ResourceMetricsOutputTypeDef",
     "CreateLocationFsxOntapRequestRequestTypeDef",
     "CreateLocationFsxOpenZfsRequestRequestTypeDef",
-    "DescribeLocationFsxOntapResponseTypeDef",
-    "DescribeLocationFsxOpenZfsResponseTypeDef",
-    "DescribeStorageSystemResourcesResponseTypeDef",
-    "DescribeStorageSystemResourceMetricsResponseTypeDef",
+    "DescribeLocationFsxOntapResponseOutputTypeDef",
+    "DescribeLocationFsxOpenZfsResponseOutputTypeDef",
+    "DescribeStorageSystemResourcesResponseOutputTypeDef",
+    "DescribeStorageSystemResourceMetricsResponseOutputTypeDef",
 )
 
 CredentialsTypeDef = TypedDict(
     "CredentialsTypeDef",
     {
         "Username": str,
         "Password": str,
@@ -228,119 +244,123 @@
     "_OptionalDiscoveryServerConfigurationTypeDef",
     {
         "ServerPort": int,
     },
     total=False,
 )
 
+
 class DiscoveryServerConfigurationTypeDef(
     _RequiredDiscoveryServerConfigurationTypeDef, _OptionalDiscoveryServerConfigurationTypeDef
 ):
     pass
 
+
 _RequiredTagListEntryTypeDef = TypedDict(
     "_RequiredTagListEntryTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalTagListEntryTypeDef = TypedDict(
     "_OptionalTagListEntryTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
+
 class TagListEntryTypeDef(_RequiredTagListEntryTypeDef, _OptionalTagListEntryTypeDef):
     pass
 
-AddStorageSystemResponseTypeDef = TypedDict(
-    "AddStorageSystemResponseTypeDef",
+
+AddStorageSystemResponseOutputTypeDef = TypedDict(
+    "AddStorageSystemResponseOutputTypeDef",
     {
         "StorageSystemArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-AgentListEntryTypeDef = TypedDict(
-    "AgentListEntryTypeDef",
+AgentListEntryOutputTypeDef = TypedDict(
+    "AgentListEntryOutputTypeDef",
     {
         "AgentArn": str,
         "Name": str,
         "Status": AgentStatusType,
     },
 )
 
 CancelTaskExecutionRequestRequestTypeDef = TypedDict(
     "CancelTaskExecutionRequestRequestTypeDef",
     {
         "TaskExecutionArn": str,
     },
 )
 
-CapacityTypeDef = TypedDict(
-    "CapacityTypeDef",
+CapacityOutputTypeDef = TypedDict(
+    "CapacityOutputTypeDef",
     {
         "Used": int,
         "Provisioned": int,
         "LogicalUsed": int,
     },
 )
 
-CreateAgentResponseTypeDef = TypedDict(
-    "CreateAgentResponseTypeDef",
+CreateAgentResponseOutputTypeDef = TypedDict(
+    "CreateAgentResponseOutputTypeDef",
     {
         "AgentArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 Ec2ConfigTypeDef = TypedDict(
     "Ec2ConfigTypeDef",
     {
         "SubnetArn": str,
         "SecurityGroupArns": Sequence[str],
     },
 )
 
-CreateLocationEfsResponseTypeDef = TypedDict(
-    "CreateLocationEfsResponseTypeDef",
+CreateLocationEfsResponseOutputTypeDef = TypedDict(
+    "CreateLocationEfsResponseOutputTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateLocationFsxLustreResponseTypeDef = TypedDict(
-    "CreateLocationFsxLustreResponseTypeDef",
+CreateLocationFsxLustreResponseOutputTypeDef = TypedDict(
+    "CreateLocationFsxLustreResponseOutputTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateLocationFsxOntapResponseTypeDef = TypedDict(
-    "CreateLocationFsxOntapResponseTypeDef",
+CreateLocationFsxOntapResponseOutputTypeDef = TypedDict(
+    "CreateLocationFsxOntapResponseOutputTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateLocationFsxOpenZfsResponseTypeDef = TypedDict(
-    "CreateLocationFsxOpenZfsResponseTypeDef",
+CreateLocationFsxOpenZfsResponseOutputTypeDef = TypedDict(
+    "CreateLocationFsxOpenZfsResponseOutputTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateLocationFsxWindowsResponseTypeDef = TypedDict(
-    "CreateLocationFsxWindowsResponseTypeDef",
+CreateLocationFsxWindowsResponseOutputTypeDef = TypedDict(
+    "CreateLocationFsxWindowsResponseOutputTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 HdfsNameNodeTypeDef = TypedDict(
@@ -356,16 +376,16 @@
     {
         "RpcProtection": HdfsRpcProtectionType,
         "DataTransferProtection": HdfsDataTransferProtectionType,
     },
     total=False,
 )
 
-CreateLocationHdfsResponseTypeDef = TypedDict(
-    "CreateLocationHdfsResponseTypeDef",
+CreateLocationHdfsResponseOutputTypeDef = TypedDict(
+    "CreateLocationHdfsResponseOutputTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 NfsMountOptionsTypeDef = TypedDict(
@@ -379,55 +399,55 @@
 OnPremConfigTypeDef = TypedDict(
     "OnPremConfigTypeDef",
     {
         "AgentArns": Sequence[str],
     },
 )
 
-CreateLocationNfsResponseTypeDef = TypedDict(
-    "CreateLocationNfsResponseTypeDef",
+CreateLocationNfsResponseOutputTypeDef = TypedDict(
+    "CreateLocationNfsResponseOutputTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateLocationObjectStorageResponseTypeDef = TypedDict(
-    "CreateLocationObjectStorageResponseTypeDef",
+CreateLocationObjectStorageResponseOutputTypeDef = TypedDict(
+    "CreateLocationObjectStorageResponseOutputTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 S3ConfigTypeDef = TypedDict(
     "S3ConfigTypeDef",
     {
         "BucketAccessRoleArn": str,
     },
 )
 
-CreateLocationS3ResponseTypeDef = TypedDict(
-    "CreateLocationS3ResponseTypeDef",
+CreateLocationS3ResponseOutputTypeDef = TypedDict(
+    "CreateLocationS3ResponseOutputTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SmbMountOptionsTypeDef = TypedDict(
     "SmbMountOptionsTypeDef",
     {
         "Version": SmbVersionType,
     },
     total=False,
 )
 
-CreateLocationSmbResponseTypeDef = TypedDict(
-    "CreateLocationSmbResponseTypeDef",
+CreateLocationSmbResponseOutputTypeDef = TypedDict(
+    "CreateLocationSmbResponseOutputTypeDef",
     {
         "LocationArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FilterRuleTypeDef = TypedDict(
@@ -464,16 +484,16 @@
 TaskScheduleTypeDef = TypedDict(
     "TaskScheduleTypeDef",
     {
         "ScheduleExpression": str,
     },
 )
 
-CreateTaskResponseTypeDef = TypedDict(
-    "CreateTaskResponseTypeDef",
+CreateTaskResponseOutputTypeDef = TypedDict(
+    "CreateTaskResponseOutputTypeDef",
     {
         "TaskArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteAgentRequestRequestTypeDef = TypedDict(
@@ -500,16 +520,16 @@
 DescribeAgentRequestRequestTypeDef = TypedDict(
     "DescribeAgentRequestRequestTypeDef",
     {
         "AgentArn": str,
     },
 )
 
-PrivateLinkConfigTypeDef = TypedDict(
-    "PrivateLinkConfigTypeDef",
+PrivateLinkConfigOutputTypeDef = TypedDict(
+    "PrivateLinkConfigOutputTypeDef",
     {
         "VpcEndpointId": str,
         "PrivateLinkEndpoint": str,
         "SubnetArns": List[str],
         "SecurityGroupArns": List[str],
     },
 )
@@ -517,16 +537,16 @@
 DescribeDiscoveryJobRequestRequestTypeDef = TypedDict(
     "DescribeDiscoveryJobRequestRequestTypeDef",
     {
         "DiscoveryJobArn": str,
     },
 )
 
-DescribeDiscoveryJobResponseTypeDef = TypedDict(
-    "DescribeDiscoveryJobResponseTypeDef",
+DescribeDiscoveryJobResponseOutputTypeDef = TypedDict(
+    "DescribeDiscoveryJobResponseOutputTypeDef",
     {
         "StorageSystemArn": str,
         "DiscoveryJobArn": str,
         "CollectionDurationMinutes": int,
         "Status": DiscoveryJobStatusType,
         "JobStartTime": datetime,
         "JobEndTime": datetime,
@@ -537,23 +557,31 @@
 DescribeLocationEfsRequestRequestTypeDef = TypedDict(
     "DescribeLocationEfsRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
+Ec2ConfigOutputTypeDef = TypedDict(
+    "Ec2ConfigOutputTypeDef",
+    {
+        "SubnetArn": str,
+        "SecurityGroupArns": List[str],
+    },
+)
+
 DescribeLocationFsxLustreRequestRequestTypeDef = TypedDict(
     "DescribeLocationFsxLustreRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
-DescribeLocationFsxLustreResponseTypeDef = TypedDict(
-    "DescribeLocationFsxLustreResponseTypeDef",
+DescribeLocationFsxLustreResponseOutputTypeDef = TypedDict(
+    "DescribeLocationFsxLustreResponseOutputTypeDef",
     {
         "LocationArn": str,
         "LocationUri": str,
         "SecurityGroupArns": List[str],
         "CreationTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -576,16 +604,16 @@
 DescribeLocationFsxWindowsRequestRequestTypeDef = TypedDict(
     "DescribeLocationFsxWindowsRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
-DescribeLocationFsxWindowsResponseTypeDef = TypedDict(
-    "DescribeLocationFsxWindowsResponseTypeDef",
+DescribeLocationFsxWindowsResponseOutputTypeDef = TypedDict(
+    "DescribeLocationFsxWindowsResponseOutputTypeDef",
     {
         "LocationArn": str,
         "LocationUri": str,
         "SecurityGroupArns": List[str],
         "CreationTime": datetime,
         "User": str,
         "Domain": str,
@@ -596,30 +624,60 @@
 DescribeLocationHdfsRequestRequestTypeDef = TypedDict(
     "DescribeLocationHdfsRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
+HdfsNameNodeOutputTypeDef = TypedDict(
+    "HdfsNameNodeOutputTypeDef",
+    {
+        "Hostname": str,
+        "Port": int,
+    },
+)
+
+QopConfigurationOutputTypeDef = TypedDict(
+    "QopConfigurationOutputTypeDef",
+    {
+        "RpcProtection": HdfsRpcProtectionType,
+        "DataTransferProtection": HdfsDataTransferProtectionType,
+    },
+)
+
 DescribeLocationNfsRequestRequestTypeDef = TypedDict(
     "DescribeLocationNfsRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
+NfsMountOptionsOutputTypeDef = TypedDict(
+    "NfsMountOptionsOutputTypeDef",
+    {
+        "Version": NfsVersionType,
+    },
+)
+
+OnPremConfigOutputTypeDef = TypedDict(
+    "OnPremConfigOutputTypeDef",
+    {
+        "AgentArns": List[str],
+    },
+)
+
 DescribeLocationObjectStorageRequestRequestTypeDef = TypedDict(
     "DescribeLocationObjectStorageRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
-DescribeLocationObjectStorageResponseTypeDef = TypedDict(
-    "DescribeLocationObjectStorageResponseTypeDef",
+DescribeLocationObjectStorageResponseOutputTypeDef = TypedDict(
+    "DescribeLocationObjectStorageResponseOutputTypeDef",
     {
         "LocationArn": str,
         "LocationUri": str,
         "AccessKey": str,
         "ServerPort": int,
         "ServerProtocol": ObjectStorageServerProtocolType,
         "AgentArns": List[str],
@@ -632,21 +690,35 @@
 DescribeLocationS3RequestRequestTypeDef = TypedDict(
     "DescribeLocationS3RequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
+S3ConfigOutputTypeDef = TypedDict(
+    "S3ConfigOutputTypeDef",
+    {
+        "BucketAccessRoleArn": str,
+    },
+)
+
 DescribeLocationSmbRequestRequestTypeDef = TypedDict(
     "DescribeLocationSmbRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 
+SmbMountOptionsOutputTypeDef = TypedDict(
+    "SmbMountOptionsOutputTypeDef",
+    {
+        "Version": SmbVersionType,
+    },
+)
+
 DescribeStorageSystemRequestRequestTypeDef = TypedDict(
     "DescribeStorageSystemRequestRequestTypeDef",
     {
         "StorageSystemArn": str,
     },
 )
 
@@ -664,20 +736,22 @@
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class DescribeStorageSystemResourceMetricsRequestDescribeStorageSystemResourceMetricsPaginateTypeDef(
     _RequiredDescribeStorageSystemResourceMetricsRequestDescribeStorageSystemResourceMetricsPaginateTypeDef,
     _OptionalDescribeStorageSystemResourceMetricsRequestDescribeStorageSystemResourceMetricsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeStorageSystemResourceMetricsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeStorageSystemResourceMetricsRequestRequestTypeDef",
     {
         "DiscoveryJobArn": str,
         "ResourceType": DiscoveryResourceTypeType,
         "ResourceId": str,
     },
@@ -689,20 +763,22 @@
         "EndTime": Union[datetime, str],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeStorageSystemResourceMetricsRequestRequestTypeDef(
     _RequiredDescribeStorageSystemResourceMetricsRequestRequestTypeDef,
     _OptionalDescribeStorageSystemResourceMetricsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeStorageSystemResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeStorageSystemResourcesRequestRequestTypeDef",
     {
         "DiscoveryJobArn": str,
         "ResourceType": DiscoveryResourceTypeType,
     },
 )
@@ -713,29 +789,68 @@
         "Filter": Mapping[Literal["SVM"], Sequence[str]],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeStorageSystemResourcesRequestRequestTypeDef(
     _RequiredDescribeStorageSystemResourcesRequestRequestTypeDef,
     _OptionalDescribeStorageSystemResourcesRequestRequestTypeDef,
 ):
     pass
 
+
+DiscoveryServerConfigurationOutputTypeDef = TypedDict(
+    "DiscoveryServerConfigurationOutputTypeDef",
+    {
+        "ServerHostname": str,
+        "ServerPort": int,
+    },
+)
+
 DescribeTaskExecutionRequestRequestTypeDef = TypedDict(
     "DescribeTaskExecutionRequestRequestTypeDef",
     {
         "TaskExecutionArn": str,
     },
 )
 
-TaskExecutionResultDetailTypeDef = TypedDict(
-    "TaskExecutionResultDetailTypeDef",
+FilterRuleOutputTypeDef = TypedDict(
+    "FilterRuleOutputTypeDef",
+    {
+        "FilterType": Literal["SIMPLE_PATTERN"],
+        "Value": str,
+    },
+)
+
+OptionsOutputTypeDef = TypedDict(
+    "OptionsOutputTypeDef",
+    {
+        "VerifyMode": VerifyModeType,
+        "OverwriteMode": OverwriteModeType,
+        "Atime": AtimeType,
+        "Mtime": MtimeType,
+        "Uid": UidType,
+        "Gid": GidType,
+        "PreserveDeletedFiles": PreserveDeletedFilesType,
+        "PreserveDevices": PreserveDevicesType,
+        "PosixPermissions": PosixPermissionsType,
+        "BytesPerSecond": int,
+        "TaskQueueing": TaskQueueingType,
+        "LogLevel": LogLevelType,
+        "TransferMode": TransferModeType,
+        "SecurityDescriptorCopyFlags": SmbSecurityDescriptorCopyFlagsType,
+        "ObjectTags": ObjectTagsType,
+    },
+)
+
+TaskExecutionResultDetailOutputTypeDef = TypedDict(
+    "TaskExecutionResultDetailOutputTypeDef",
     {
         "PrepareDuration": int,
         "PrepareStatus": PhaseStatusType,
         "TotalDuration": int,
         "TransferDuration": int,
         "TransferStatus": PhaseStatusType,
         "VerifyDuration": int,
@@ -748,16 +863,23 @@
 DescribeTaskRequestRequestTypeDef = TypedDict(
     "DescribeTaskRequestRequestTypeDef",
     {
         "TaskArn": str,
     },
 )
 
-DiscoveryJobListEntryTypeDef = TypedDict(
-    "DiscoveryJobListEntryTypeDef",
+TaskScheduleOutputTypeDef = TypedDict(
+    "TaskScheduleOutputTypeDef",
+    {
+        "ScheduleExpression": str,
+    },
+)
+
+DiscoveryJobListEntryOutputTypeDef = TypedDict(
+    "DiscoveryJobListEntryOutputTypeDef",
     {
         "DiscoveryJobArn": str,
         "Status": DiscoveryJobStatusType,
     },
 )
 
 GenerateRecommendationsRequestRequestTypeDef = TypedDict(
@@ -765,26 +887,26 @@
     {
         "DiscoveryJobArn": str,
         "ResourceIds": Sequence[str],
         "ResourceType": DiscoveryResourceTypeType,
     },
 )
 
-IOPSTypeDef = TypedDict(
-    "IOPSTypeDef",
+IOPSOutputTypeDef = TypedDict(
+    "IOPSOutputTypeDef",
     {
         "Read": float,
         "Write": float,
         "Other": float,
         "Total": float,
     },
 )
 
-LatencyTypeDef = TypedDict(
-    "LatencyTypeDef",
+LatencyOutputTypeDef = TypedDict(
+    "LatencyOutputTypeDef",
     {
         "Read": float,
         "Write": float,
         "Other": float,
     },
 )
 
@@ -829,16 +951,16 @@
     {
         "Name": LocationFilterNameType,
         "Values": Sequence[str],
         "Operator": OperatorType,
     },
 )
 
-LocationListEntryTypeDef = TypedDict(
-    "LocationListEntryTypeDef",
+LocationListEntryOutputTypeDef = TypedDict(
+    "LocationListEntryOutputTypeDef",
     {
         "LocationArn": str,
         "LocationUri": str,
     },
 )
 
 ListStorageSystemsRequestListStorageSystemsPaginateTypeDef = TypedDict(
@@ -854,16 +976,16 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-StorageSystemListEntryTypeDef = TypedDict(
-    "StorageSystemListEntryTypeDef",
+StorageSystemListEntryOutputTypeDef = TypedDict(
+    "StorageSystemListEntryOutputTypeDef",
     {
         "StorageSystemArn": str,
         "Name": str,
     },
 )
 
 _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
@@ -876,20 +998,22 @@
     "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
     _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
 ):
     pass
 
+
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -897,20 +1021,30 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
+
+TagListEntryOutputTypeDef = TypedDict(
+    "TagListEntryOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 ListTaskExecutionsRequestListTaskExecutionsPaginateTypeDef = TypedDict(
     "ListTaskExecutionsRequestListTaskExecutionsPaginateTypeDef",
     {
         "TaskArn": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -922,16 +1056,16 @@
         "TaskArn": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-TaskExecutionListEntryTypeDef = TypedDict(
-    "TaskExecutionListEntryTypeDef",
+TaskExecutionListEntryOutputTypeDef = TypedDict(
+    "TaskExecutionListEntryOutputTypeDef",
     {
         "TaskExecutionArn": str,
         "Status": TaskExecutionStatusType,
     },
 )
 
 TaskFilterTypeDef = TypedDict(
@@ -939,25 +1073,25 @@
     {
         "Name": TaskFilterNameType,
         "Values": Sequence[str],
         "Operator": OperatorType,
     },
 )
 
-TaskListEntryTypeDef = TypedDict(
-    "TaskListEntryTypeDef",
+TaskListEntryOutputTypeDef = TypedDict(
+    "TaskListEntryOutputTypeDef",
     {
         "TaskArn": str,
         "Status": TaskStatusType,
         "Name": str,
     },
 )
 
-MaxP95PerformanceTypeDef = TypedDict(
-    "MaxP95PerformanceTypeDef",
+MaxP95PerformanceOutputTypeDef = TypedDict(
+    "MaxP95PerformanceOutputTypeDef",
     {
         "IopsRead": float,
         "IopsWrite": float,
         "IopsOther": float,
         "IopsTotal": float,
         "ThroughputRead": float,
         "ThroughputWrite": float,
@@ -965,25 +1099,25 @@
         "ThroughputTotal": float,
         "LatencyRead": float,
         "LatencyWrite": float,
         "LatencyOther": float,
     },
 )
 
-RecommendationTypeDef = TypedDict(
-    "RecommendationTypeDef",
+RecommendationOutputTypeDef = TypedDict(
+    "RecommendationOutputTypeDef",
     {
         "StorageType": str,
         "StorageConfiguration": Dict[str, str],
         "EstimatedMonthlyStorageCost": str,
     },
 )
 
-ThroughputTypeDef = TypedDict(
-    "ThroughputTypeDef",
+ThroughputOutputTypeDef = TypedDict(
+    "ThroughputOutputTypeDef",
     {
         "Read": float,
         "Write": float,
         "Other": float,
         "Total": float,
     },
 )
@@ -1012,24 +1146,24 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-StartDiscoveryJobResponseTypeDef = TypedDict(
-    "StartDiscoveryJobResponseTypeDef",
+StartDiscoveryJobResponseOutputTypeDef = TypedDict(
+    "StartDiscoveryJobResponseOutputTypeDef",
     {
         "DiscoveryJobArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartTaskExecutionResponseTypeDef = TypedDict(
-    "StartTaskExecutionResponseTypeDef",
+StartTaskExecutionResponseOutputTypeDef = TypedDict(
+    "StartTaskExecutionResponseOutputTypeDef",
     {
         "TaskExecutionArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopDiscoveryJobRequestRequestTypeDef = TypedDict(
@@ -1057,19 +1191,21 @@
     "_OptionalUpdateAgentRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
+
 class UpdateAgentRequestRequestTypeDef(
     _RequiredUpdateAgentRequestRequestTypeDef, _OptionalUpdateAgentRequestRequestTypeDef
 ):
     pass
 
+
 UpdateDiscoveryJobRequestRequestTypeDef = TypedDict(
     "UpdateDiscoveryJobRequestRequestTypeDef",
     {
         "DiscoveryJobArn": str,
         "CollectionDurationMinutes": int,
     },
 )
@@ -1090,36 +1226,21 @@
         "SecretKey": str,
         "AgentArns": Sequence[str],
         "ServerCertificate": Union[str, bytes, IO[Any], StreamingBody],
     },
     total=False,
 )
 
+
 class UpdateLocationObjectStorageRequestRequestTypeDef(
     _RequiredUpdateLocationObjectStorageRequestRequestTypeDef,
     _OptionalUpdateLocationObjectStorageRequestRequestTypeDef,
 ):
     pass
 
-DescribeStorageSystemResponseTypeDef = TypedDict(
-    "DescribeStorageSystemResponseTypeDef",
-    {
-        "StorageSystemArn": str,
-        "ServerConfiguration": DiscoveryServerConfigurationTypeDef,
-        "SystemType": Literal["NetAppONTAP"],
-        "AgentArns": List[str],
-        "Name": str,
-        "ErrorMessage": str,
-        "ConnectivityStatus": StorageSystemConnectivityStatusType,
-        "CloudWatchLogGroupArn": str,
-        "CreationTime": datetime,
-        "SecretsManagerArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredUpdateStorageSystemRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStorageSystemRequestRequestTypeDef",
     {
         "StorageSystemArn": str,
     },
 )
@@ -1131,20 +1252,22 @@
         "Name": str,
         "CloudWatchLogGroupArn": str,
         "Credentials": CredentialsTypeDef,
     },
     total=False,
 )
 
+
 class UpdateStorageSystemRequestRequestTypeDef(
     _RequiredUpdateStorageSystemRequestRequestTypeDef,
     _OptionalUpdateStorageSystemRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredAddStorageSystemRequestRequestTypeDef = TypedDict(
     "_RequiredAddStorageSystemRequestRequestTypeDef",
     {
         "ServerConfiguration": DiscoveryServerConfigurationTypeDef,
         "SystemType": Literal["NetAppONTAP"],
         "AgentArns": Sequence[str],
         "ClientToken": str,
@@ -1157,19 +1280,21 @@
         "CloudWatchLogGroupArn": str,
         "Tags": Sequence[TagListEntryTypeDef],
         "Name": str,
     },
     total=False,
 )
 
+
 class AddStorageSystemRequestRequestTypeDef(
     _RequiredAddStorageSystemRequestRequestTypeDef, _OptionalAddStorageSystemRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateAgentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAgentRequestRequestTypeDef",
     {
         "ActivationKey": str,
     },
 )
 _OptionalCreateAgentRequestRequestTypeDef = TypedDict(
@@ -1180,19 +1305,21 @@
         "VpcEndpointId": str,
         "SubnetArns": Sequence[str],
         "SecurityGroupArns": Sequence[str],
     },
     total=False,
 )
 
+
 class CreateAgentRequestRequestTypeDef(
     _RequiredCreateAgentRequestRequestTypeDef, _OptionalCreateAgentRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateLocationFsxLustreRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLocationFsxLustreRequestRequestTypeDef",
     {
         "FsxFilesystemArn": str,
         "SecurityGroupArns": Sequence[str],
     },
 )
@@ -1201,20 +1328,22 @@
     {
         "Subdirectory": str,
         "Tags": Sequence[TagListEntryTypeDef],
     },
     total=False,
 )
 
+
 class CreateLocationFsxLustreRequestRequestTypeDef(
     _RequiredCreateLocationFsxLustreRequestRequestTypeDef,
     _OptionalCreateLocationFsxLustreRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateLocationFsxWindowsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLocationFsxWindowsRequestRequestTypeDef",
     {
         "FsxFilesystemArn": str,
         "SecurityGroupArns": Sequence[str],
         "User": str,
         "Password": str,
@@ -1226,20 +1355,22 @@
         "Subdirectory": str,
         "Tags": Sequence[TagListEntryTypeDef],
         "Domain": str,
     },
     total=False,
 )
 
+
 class CreateLocationFsxWindowsRequestRequestTypeDef(
     _RequiredCreateLocationFsxWindowsRequestRequestTypeDef,
     _OptionalCreateLocationFsxWindowsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateLocationObjectStorageRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLocationObjectStorageRequestRequestTypeDef",
     {
         "ServerHostname": str,
         "BucketName": str,
         "AgentArns": Sequence[str],
     },
@@ -1254,28 +1385,21 @@
         "SecretKey": str,
         "Tags": Sequence[TagListEntryTypeDef],
         "ServerCertificate": Union[str, bytes, IO[Any], StreamingBody],
     },
     total=False,
 )
 
+
 class CreateLocationObjectStorageRequestRequestTypeDef(
     _RequiredCreateLocationObjectStorageRequestRequestTypeDef,
     _OptionalCreateLocationObjectStorageRequestRequestTypeDef,
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagListEntryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredStartDiscoveryJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartDiscoveryJobRequestRequestTypeDef",
     {
         "StorageSystemArn": str,
         "CollectionDurationMinutes": int,
         "ClientToken": str,
@@ -1285,31 +1409,33 @@
     "_OptionalStartDiscoveryJobRequestRequestTypeDef",
     {
         "Tags": Sequence[TagListEntryTypeDef],
     },
     total=False,
 )
 
+
 class StartDiscoveryJobRequestRequestTypeDef(
     _RequiredStartDiscoveryJobRequestRequestTypeDef, _OptionalStartDiscoveryJobRequestRequestTypeDef
 ):
     pass
 
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagListEntryTypeDef],
     },
 )
 
-ListAgentsResponseTypeDef = TypedDict(
-    "ListAgentsResponseTypeDef",
+ListAgentsResponseOutputTypeDef = TypedDict(
+    "ListAgentsResponseOutputTypeDef",
     {
-        "Agents": List[AgentListEntryTypeDef],
+        "Agents": List[AgentListEntryOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateLocationEfsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLocationEfsRequestRequestTypeDef",
@@ -1326,32 +1452,20 @@
         "AccessPointArn": str,
         "FileSystemAccessRoleArn": str,
         "InTransitEncryption": EfsInTransitEncryptionType,
     },
     total=False,
 )
 
+
 class CreateLocationEfsRequestRequestTypeDef(
     _RequiredCreateLocationEfsRequestRequestTypeDef, _OptionalCreateLocationEfsRequestRequestTypeDef
 ):
     pass
 
-DescribeLocationEfsResponseTypeDef = TypedDict(
-    "DescribeLocationEfsResponseTypeDef",
-    {
-        "LocationArn": str,
-        "LocationUri": str,
-        "Ec2Config": Ec2ConfigTypeDef,
-        "CreationTime": datetime,
-        "AccessPointArn": str,
-        "FileSystemAccessRoleArn": str,
-        "InTransitEncryption": EfsInTransitEncryptionType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredCreateLocationHdfsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLocationHdfsRequestRequestTypeDef",
     {
         "NameNodes": Sequence[HdfsNameNodeTypeDef],
         "AuthenticationType": HdfsAuthenticationTypeType,
         "AgentArns": Sequence[str],
@@ -1370,38 +1484,21 @@
         "KerberosKeytab": Union[str, bytes, IO[Any], StreamingBody],
         "KerberosKrb5Conf": Union[str, bytes, IO[Any], StreamingBody],
         "Tags": Sequence[TagListEntryTypeDef],
     },
     total=False,
 )
 
+
 class CreateLocationHdfsRequestRequestTypeDef(
     _RequiredCreateLocationHdfsRequestRequestTypeDef,
     _OptionalCreateLocationHdfsRequestRequestTypeDef,
 ):
     pass
 
-DescribeLocationHdfsResponseTypeDef = TypedDict(
-    "DescribeLocationHdfsResponseTypeDef",
-    {
-        "LocationArn": str,
-        "LocationUri": str,
-        "NameNodes": List[HdfsNameNodeTypeDef],
-        "BlockSize": int,
-        "ReplicationFactor": int,
-        "KmsKeyProviderUri": str,
-        "QopConfiguration": QopConfigurationTypeDef,
-        "AuthenticationType": HdfsAuthenticationTypeType,
-        "SimpleUser": str,
-        "KerberosPrincipal": str,
-        "AgentArns": List[str],
-        "CreationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredUpdateLocationHdfsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLocationHdfsRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
@@ -1420,20 +1517,22 @@
         "KerberosKeytab": Union[str, bytes, IO[Any], StreamingBody],
         "KerberosKrb5Conf": Union[str, bytes, IO[Any], StreamingBody],
         "AgentArns": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdateLocationHdfsRequestRequestTypeDef(
     _RequiredUpdateLocationHdfsRequestRequestTypeDef,
     _OptionalUpdateLocationHdfsRequestRequestTypeDef,
 ):
     pass
 
+
 FsxProtocolNfsTypeDef = TypedDict(
     "FsxProtocolNfsTypeDef",
     {
         "MountOptions": NfsMountOptionsTypeDef,
     },
     total=False,
 )
@@ -1451,30 +1550,20 @@
     {
         "MountOptions": NfsMountOptionsTypeDef,
         "Tags": Sequence[TagListEntryTypeDef],
     },
     total=False,
 )
 
+
 class CreateLocationNfsRequestRequestTypeDef(
     _RequiredCreateLocationNfsRequestRequestTypeDef, _OptionalCreateLocationNfsRequestRequestTypeDef
 ):
     pass
 
-DescribeLocationNfsResponseTypeDef = TypedDict(
-    "DescribeLocationNfsResponseTypeDef",
-    {
-        "LocationArn": str,
-        "LocationUri": str,
-        "OnPremConfig": OnPremConfigTypeDef,
-        "MountOptions": NfsMountOptionsTypeDef,
-        "CreationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredUpdateLocationNfsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLocationNfsRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
@@ -1484,19 +1573,21 @@
         "Subdirectory": str,
         "OnPremConfig": OnPremConfigTypeDef,
         "MountOptions": NfsMountOptionsTypeDef,
     },
     total=False,
 )
 
+
 class UpdateLocationNfsRequestRequestTypeDef(
     _RequiredUpdateLocationNfsRequestRequestTypeDef, _OptionalUpdateLocationNfsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateLocationS3RequestRequestTypeDef = TypedDict(
     "_RequiredCreateLocationS3RequestRequestTypeDef",
     {
         "S3BucketArn": str,
         "S3Config": S3ConfigTypeDef,
     },
 )
@@ -1507,31 +1598,20 @@
         "S3StorageClass": S3StorageClassType,
         "AgentArns": Sequence[str],
         "Tags": Sequence[TagListEntryTypeDef],
     },
     total=False,
 )
 
+
 class CreateLocationS3RequestRequestTypeDef(
     _RequiredCreateLocationS3RequestRequestTypeDef, _OptionalCreateLocationS3RequestRequestTypeDef
 ):
     pass
 
-DescribeLocationS3ResponseTypeDef = TypedDict(
-    "DescribeLocationS3ResponseTypeDef",
-    {
-        "LocationArn": str,
-        "LocationUri": str,
-        "S3StorageClass": S3StorageClassType,
-        "S3Config": S3ConfigTypeDef,
-        "AgentArns": List[str],
-        "CreationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredCreateLocationSmbRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLocationSmbRequestRequestTypeDef",
     {
         "Subdirectory": str,
         "ServerHostname": str,
         "User": str,
@@ -1545,32 +1625,20 @@
         "Domain": str,
         "MountOptions": SmbMountOptionsTypeDef,
         "Tags": Sequence[TagListEntryTypeDef],
     },
     total=False,
 )
 
+
 class CreateLocationSmbRequestRequestTypeDef(
     _RequiredCreateLocationSmbRequestRequestTypeDef, _OptionalCreateLocationSmbRequestRequestTypeDef
 ):
     pass
 
-DescribeLocationSmbResponseTypeDef = TypedDict(
-    "DescribeLocationSmbResponseTypeDef",
-    {
-        "LocationArn": str,
-        "LocationUri": str,
-        "AgentArns": List[str],
-        "User": str,
-        "Domain": str,
-        "MountOptions": SmbMountOptionsTypeDef,
-        "CreationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredFsxProtocolSmbTypeDef = TypedDict(
     "_RequiredFsxProtocolSmbTypeDef",
     {
         "Password": str,
         "User": str,
     },
@@ -1580,17 +1648,19 @@
     {
         "Domain": str,
         "MountOptions": SmbMountOptionsTypeDef,
     },
     total=False,
 )
 
+
 class FsxProtocolSmbTypeDef(_RequiredFsxProtocolSmbTypeDef, _OptionalFsxProtocolSmbTypeDef):
     pass
 
+
 _RequiredUpdateLocationSmbRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLocationSmbRequestRequestTypeDef",
     {
         "LocationArn": str,
     },
 )
 _OptionalUpdateLocationSmbRequestRequestTypeDef = TypedDict(
@@ -1602,19 +1672,21 @@
         "Password": str,
         "AgentArns": Sequence[str],
         "MountOptions": SmbMountOptionsTypeDef,
     },
     total=False,
 )
 
+
 class UpdateLocationSmbRequestRequestTypeDef(
     _RequiredUpdateLocationSmbRequestRequestTypeDef, _OptionalUpdateLocationSmbRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredStartTaskExecutionRequestRequestTypeDef = TypedDict(
     "_RequiredStartTaskExecutionRequestRequestTypeDef",
     {
         "TaskArn": str,
     },
 )
 _OptionalStartTaskExecutionRequestRequestTypeDef = TypedDict(
@@ -1624,20 +1696,22 @@
         "Includes": Sequence[FilterRuleTypeDef],
         "Excludes": Sequence[FilterRuleTypeDef],
         "Tags": Sequence[TagListEntryTypeDef],
     },
     total=False,
 )
 
+
 class StartTaskExecutionRequestRequestTypeDef(
     _RequiredStartTaskExecutionRequestRequestTypeDef,
     _OptionalStartTaskExecutionRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateTaskExecutionRequestRequestTypeDef = TypedDict(
     "UpdateTaskExecutionRequestRequestTypeDef",
     {
         "TaskExecutionArn": str,
         "Options": OptionsTypeDef,
     },
 )
@@ -1659,41 +1733,20 @@
         "Schedule": TaskScheduleTypeDef,
         "Tags": Sequence[TagListEntryTypeDef],
         "Includes": Sequence[FilterRuleTypeDef],
     },
     total=False,
 )
 
+
 class CreateTaskRequestRequestTypeDef(
     _RequiredCreateTaskRequestRequestTypeDef, _OptionalCreateTaskRequestRequestTypeDef
 ):
     pass
 
-DescribeTaskResponseTypeDef = TypedDict(
-    "DescribeTaskResponseTypeDef",
-    {
-        "TaskArn": str,
-        "Status": TaskStatusType,
-        "Name": str,
-        "CurrentTaskExecutionArn": str,
-        "SourceLocationArn": str,
-        "DestinationLocationArn": str,
-        "CloudWatchLogGroupArn": str,
-        "SourceNetworkInterfaceArns": List[str],
-        "DestinationNetworkInterfaceArns": List[str],
-        "Options": OptionsTypeDef,
-        "Excludes": List[FilterRuleTypeDef],
-        "Schedule": TaskScheduleTypeDef,
-        "ErrorCode": str,
-        "ErrorDetail": str,
-        "CreationTime": datetime,
-        "Includes": List[FilterRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredUpdateTaskRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTaskRequestRequestTypeDef",
     {
         "TaskArn": str,
     },
 )
@@ -1706,57 +1759,188 @@
         "Name": str,
         "CloudWatchLogGroupArn": str,
         "Includes": Sequence[FilterRuleTypeDef],
     },
     total=False,
 )
 
+
 class UpdateTaskRequestRequestTypeDef(
     _RequiredUpdateTaskRequestRequestTypeDef, _OptionalUpdateTaskRequestRequestTypeDef
 ):
     pass
 
-DescribeAgentResponseTypeDef = TypedDict(
-    "DescribeAgentResponseTypeDef",
+
+DescribeAgentResponseOutputTypeDef = TypedDict(
+    "DescribeAgentResponseOutputTypeDef",
     {
         "AgentArn": str,
         "Name": str,
         "Status": AgentStatusType,
         "LastConnectionTime": datetime,
         "CreationTime": datetime,
         "EndpointType": EndpointTypeType,
-        "PrivateLinkConfig": PrivateLinkConfigTypeDef,
+        "PrivateLinkConfig": PrivateLinkConfigOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeLocationEfsResponseOutputTypeDef = TypedDict(
+    "DescribeLocationEfsResponseOutputTypeDef",
+    {
+        "LocationArn": str,
+        "LocationUri": str,
+        "Ec2Config": Ec2ConfigOutputTypeDef,
+        "CreationTime": datetime,
+        "AccessPointArn": str,
+        "FileSystemAccessRoleArn": str,
+        "InTransitEncryption": EfsInTransitEncryptionType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeLocationHdfsResponseOutputTypeDef = TypedDict(
+    "DescribeLocationHdfsResponseOutputTypeDef",
+    {
+        "LocationArn": str,
+        "LocationUri": str,
+        "NameNodes": List[HdfsNameNodeOutputTypeDef],
+        "BlockSize": int,
+        "ReplicationFactor": int,
+        "KmsKeyProviderUri": str,
+        "QopConfiguration": QopConfigurationOutputTypeDef,
+        "AuthenticationType": HdfsAuthenticationTypeType,
+        "SimpleUser": str,
+        "KerberosPrincipal": str,
+        "AgentArns": List[str],
+        "CreationTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+FsxProtocolNfsOutputTypeDef = TypedDict(
+    "FsxProtocolNfsOutputTypeDef",
+    {
+        "MountOptions": NfsMountOptionsOutputTypeDef,
+    },
+)
+
+DescribeLocationNfsResponseOutputTypeDef = TypedDict(
+    "DescribeLocationNfsResponseOutputTypeDef",
+    {
+        "LocationArn": str,
+        "LocationUri": str,
+        "OnPremConfig": OnPremConfigOutputTypeDef,
+        "MountOptions": NfsMountOptionsOutputTypeDef,
+        "CreationTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeLocationS3ResponseOutputTypeDef = TypedDict(
+    "DescribeLocationS3ResponseOutputTypeDef",
+    {
+        "LocationArn": str,
+        "LocationUri": str,
+        "S3StorageClass": S3StorageClassType,
+        "S3Config": S3ConfigOutputTypeDef,
+        "AgentArns": List[str],
+        "CreationTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeLocationSmbResponseOutputTypeDef = TypedDict(
+    "DescribeLocationSmbResponseOutputTypeDef",
+    {
+        "LocationArn": str,
+        "LocationUri": str,
+        "AgentArns": List[str],
+        "User": str,
+        "Domain": str,
+        "MountOptions": SmbMountOptionsOutputTypeDef,
+        "CreationTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+FsxProtocolSmbOutputTypeDef = TypedDict(
+    "FsxProtocolSmbOutputTypeDef",
+    {
+        "Domain": str,
+        "MountOptions": SmbMountOptionsOutputTypeDef,
+        "Password": str,
+        "User": str,
+    },
+)
+
+DescribeStorageSystemResponseOutputTypeDef = TypedDict(
+    "DescribeStorageSystemResponseOutputTypeDef",
+    {
+        "StorageSystemArn": str,
+        "ServerConfiguration": DiscoveryServerConfigurationOutputTypeDef,
+        "SystemType": Literal["NetAppONTAP"],
+        "AgentArns": List[str],
+        "Name": str,
+        "ErrorMessage": str,
+        "ConnectivityStatus": StorageSystemConnectivityStatusType,
+        "CloudWatchLogGroupArn": str,
+        "CreationTime": datetime,
+        "SecretsManagerArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeTaskExecutionResponseTypeDef = TypedDict(
-    "DescribeTaskExecutionResponseTypeDef",
+DescribeTaskExecutionResponseOutputTypeDef = TypedDict(
+    "DescribeTaskExecutionResponseOutputTypeDef",
     {
         "TaskExecutionArn": str,
         "Status": TaskExecutionStatusType,
-        "Options": OptionsTypeDef,
-        "Excludes": List[FilterRuleTypeDef],
-        "Includes": List[FilterRuleTypeDef],
+        "Options": OptionsOutputTypeDef,
+        "Excludes": List[FilterRuleOutputTypeDef],
+        "Includes": List[FilterRuleOutputTypeDef],
         "StartTime": datetime,
         "EstimatedFilesToTransfer": int,
         "EstimatedBytesToTransfer": int,
         "FilesTransferred": int,
         "BytesWritten": int,
         "BytesTransferred": int,
-        "Result": TaskExecutionResultDetailTypeDef,
+        "Result": TaskExecutionResultDetailOutputTypeDef,
         "BytesCompressed": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListDiscoveryJobsResponseTypeDef = TypedDict(
-    "ListDiscoveryJobsResponseTypeDef",
+DescribeTaskResponseOutputTypeDef = TypedDict(
+    "DescribeTaskResponseOutputTypeDef",
+    {
+        "TaskArn": str,
+        "Status": TaskStatusType,
+        "Name": str,
+        "CurrentTaskExecutionArn": str,
+        "SourceLocationArn": str,
+        "DestinationLocationArn": str,
+        "CloudWatchLogGroupArn": str,
+        "SourceNetworkInterfaceArns": List[str],
+        "DestinationNetworkInterfaceArns": List[str],
+        "Options": OptionsOutputTypeDef,
+        "Excludes": List[FilterRuleOutputTypeDef],
+        "Schedule": TaskScheduleOutputTypeDef,
+        "ErrorCode": str,
+        "ErrorDetail": str,
+        "CreationTime": datetime,
+        "Includes": List[FilterRuleOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListDiscoveryJobsResponseOutputTypeDef = TypedDict(
+    "ListDiscoveryJobsResponseOutputTypeDef",
     {
-        "DiscoveryJobs": List[DiscoveryJobListEntryTypeDef],
+        "DiscoveryJobs": List[DiscoveryJobListEntryOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLocationsRequestListLocationsPaginateTypeDef = TypedDict(
     "ListLocationsRequestListLocationsPaginateTypeDef",
@@ -1773,36 +1957,45 @@
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[LocationFilterTypeDef],
     },
     total=False,
 )
 
-ListLocationsResponseTypeDef = TypedDict(
-    "ListLocationsResponseTypeDef",
+ListLocationsResponseOutputTypeDef = TypedDict(
+    "ListLocationsResponseOutputTypeDef",
+    {
+        "Locations": List[LocationListEntryOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListStorageSystemsResponseOutputTypeDef = TypedDict(
+    "ListStorageSystemsResponseOutputTypeDef",
     {
-        "Locations": List[LocationListEntryTypeDef],
+        "StorageSystems": List[StorageSystemListEntryOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListStorageSystemsResponseTypeDef = TypedDict(
-    "ListStorageSystemsResponseTypeDef",
+ListTagsForResourceResponseOutputTypeDef = TypedDict(
+    "ListTagsForResourceResponseOutputTypeDef",
     {
-        "StorageSystems": List[StorageSystemListEntryTypeDef],
+        "Tags": List[TagListEntryOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTaskExecutionsResponseTypeDef = TypedDict(
-    "ListTaskExecutionsResponseTypeDef",
+ListTaskExecutionsResponseOutputTypeDef = TypedDict(
+    "ListTaskExecutionsResponseOutputTypeDef",
     {
-        "TaskExecutions": List[TaskExecutionListEntryTypeDef],
+        "TaskExecutions": List[TaskExecutionListEntryOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTasksRequestListTasksPaginateTypeDef = TypedDict(
     "ListTasksRequestListTasksPaginateTypeDef",
@@ -1819,114 +2012,122 @@
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[TaskFilterTypeDef],
     },
     total=False,
 )
 
-ListTasksResponseTypeDef = TypedDict(
-    "ListTasksResponseTypeDef",
+ListTasksResponseOutputTypeDef = TypedDict(
+    "ListTasksResponseOutputTypeDef",
     {
-        "Tasks": List[TaskListEntryTypeDef],
+        "Tasks": List[TaskListEntryOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-NetAppONTAPClusterTypeDef = TypedDict(
-    "NetAppONTAPClusterTypeDef",
+NetAppONTAPClusterOutputTypeDef = TypedDict(
+    "NetAppONTAPClusterOutputTypeDef",
     {
         "CifsShareCount": int,
         "NfsExportedVolumes": int,
         "ResourceId": str,
         "ClusterName": str,
-        "MaxP95Performance": MaxP95PerformanceTypeDef,
+        "MaxP95Performance": MaxP95PerformanceOutputTypeDef,
         "ClusterBlockStorageSize": int,
         "ClusterBlockStorageUsed": int,
         "ClusterBlockStorageLogicalUsed": int,
-        "Recommendations": List[RecommendationTypeDef],
+        "Recommendations": List[RecommendationOutputTypeDef],
         "RecommendationStatus": RecommendationStatusType,
         "LunCount": int,
     },
 )
 
-NetAppONTAPSVMTypeDef = TypedDict(
-    "NetAppONTAPSVMTypeDef",
+NetAppONTAPSVMOutputTypeDef = TypedDict(
+    "NetAppONTAPSVMOutputTypeDef",
     {
         "ClusterUuid": str,
         "ResourceId": str,
         "SvmName": str,
         "CifsShareCount": int,
         "EnabledProtocols": List[str],
         "TotalCapacityUsed": int,
         "TotalCapacityProvisioned": int,
         "TotalLogicalCapacityUsed": int,
-        "MaxP95Performance": MaxP95PerformanceTypeDef,
-        "Recommendations": List[RecommendationTypeDef],
+        "MaxP95Performance": MaxP95PerformanceOutputTypeDef,
+        "Recommendations": List[RecommendationOutputTypeDef],
         "NfsExportedVolumes": int,
         "RecommendationStatus": RecommendationStatusType,
         "TotalSnapshotCapacityUsed": int,
         "LunCount": int,
     },
 )
 
-NetAppONTAPVolumeTypeDef = TypedDict(
-    "NetAppONTAPVolumeTypeDef",
+NetAppONTAPVolumeOutputTypeDef = TypedDict(
+    "NetAppONTAPVolumeOutputTypeDef",
     {
         "VolumeName": str,
         "ResourceId": str,
         "CifsShareCount": int,
         "SecurityStyle": str,
         "SvmUuid": str,
         "SvmName": str,
         "CapacityUsed": int,
         "CapacityProvisioned": int,
         "LogicalCapacityUsed": int,
         "NfsExported": bool,
         "SnapshotCapacityUsed": int,
-        "MaxP95Performance": MaxP95PerformanceTypeDef,
-        "Recommendations": List[RecommendationTypeDef],
+        "MaxP95Performance": MaxP95PerformanceOutputTypeDef,
+        "Recommendations": List[RecommendationOutputTypeDef],
         "RecommendationStatus": RecommendationStatusType,
         "LunCount": int,
     },
 )
 
-P95MetricsTypeDef = TypedDict(
-    "P95MetricsTypeDef",
+P95MetricsOutputTypeDef = TypedDict(
+    "P95MetricsOutputTypeDef",
     {
-        "IOPS": IOPSTypeDef,
-        "Throughput": ThroughputTypeDef,
-        "Latency": LatencyTypeDef,
+        "IOPS": IOPSOutputTypeDef,
+        "Throughput": ThroughputOutputTypeDef,
+        "Latency": LatencyOutputTypeDef,
     },
 )
 
 FsxProtocolTypeDef = TypedDict(
     "FsxProtocolTypeDef",
     {
         "NFS": FsxProtocolNfsTypeDef,
         "SMB": FsxProtocolSmbTypeDef,
     },
     total=False,
 )
 
-ResourceDetailsTypeDef = TypedDict(
-    "ResourceDetailsTypeDef",
+FsxProtocolOutputTypeDef = TypedDict(
+    "FsxProtocolOutputTypeDef",
     {
-        "NetAppONTAPSVMs": List[NetAppONTAPSVMTypeDef],
-        "NetAppONTAPVolumes": List[NetAppONTAPVolumeTypeDef],
-        "NetAppONTAPClusters": List[NetAppONTAPClusterTypeDef],
+        "NFS": FsxProtocolNfsOutputTypeDef,
+        "SMB": FsxProtocolSmbOutputTypeDef,
     },
 )
 
-ResourceMetricsTypeDef = TypedDict(
-    "ResourceMetricsTypeDef",
+ResourceDetailsOutputTypeDef = TypedDict(
+    "ResourceDetailsOutputTypeDef",
+    {
+        "NetAppONTAPSVMs": List[NetAppONTAPSVMOutputTypeDef],
+        "NetAppONTAPVolumes": List[NetAppONTAPVolumeOutputTypeDef],
+        "NetAppONTAPClusters": List[NetAppONTAPClusterOutputTypeDef],
+    },
+)
+
+ResourceMetricsOutputTypeDef = TypedDict(
+    "ResourceMetricsOutputTypeDef",
     {
         "Timestamp": datetime,
-        "P95Metrics": P95MetricsTypeDef,
-        "Capacity": CapacityTypeDef,
+        "P95Metrics": P95MetricsOutputTypeDef,
+        "Capacity": CapacityOutputTypeDef,
         "ResourceId": str,
         "ResourceType": DiscoveryResourceTypeType,
     },
 )
 
 _RequiredCreateLocationFsxOntapRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLocationFsxOntapRequestRequestTypeDef",
@@ -1941,20 +2142,22 @@
     {
         "Subdirectory": str,
         "Tags": Sequence[TagListEntryTypeDef],
     },
     total=False,
 )
 
+
 class CreateLocationFsxOntapRequestRequestTypeDef(
     _RequiredCreateLocationFsxOntapRequestRequestTypeDef,
     _OptionalCreateLocationFsxOntapRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateLocationFsxOpenZfsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLocationFsxOpenZfsRequestRequestTypeDef",
     {
         "FsxFilesystemArn": str,
         "Protocol": FsxProtocolTypeDef,
         "SecurityGroupArns": Sequence[str],
     },
@@ -1964,56 +2167,58 @@
     {
         "Subdirectory": str,
         "Tags": Sequence[TagListEntryTypeDef],
     },
     total=False,
 )
 
+
 class CreateLocationFsxOpenZfsRequestRequestTypeDef(
     _RequiredCreateLocationFsxOpenZfsRequestRequestTypeDef,
     _OptionalCreateLocationFsxOpenZfsRequestRequestTypeDef,
 ):
     pass
 
-DescribeLocationFsxOntapResponseTypeDef = TypedDict(
-    "DescribeLocationFsxOntapResponseTypeDef",
+
+DescribeLocationFsxOntapResponseOutputTypeDef = TypedDict(
+    "DescribeLocationFsxOntapResponseOutputTypeDef",
     {
         "CreationTime": datetime,
         "LocationArn": str,
         "LocationUri": str,
-        "Protocol": FsxProtocolTypeDef,
+        "Protocol": FsxProtocolOutputTypeDef,
         "SecurityGroupArns": List[str],
         "StorageVirtualMachineArn": str,
         "FsxFilesystemArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeLocationFsxOpenZfsResponseTypeDef = TypedDict(
-    "DescribeLocationFsxOpenZfsResponseTypeDef",
+DescribeLocationFsxOpenZfsResponseOutputTypeDef = TypedDict(
+    "DescribeLocationFsxOpenZfsResponseOutputTypeDef",
     {
         "LocationArn": str,
         "LocationUri": str,
         "SecurityGroupArns": List[str],
-        "Protocol": FsxProtocolTypeDef,
+        "Protocol": FsxProtocolOutputTypeDef,
         "CreationTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeStorageSystemResourcesResponseTypeDef = TypedDict(
-    "DescribeStorageSystemResourcesResponseTypeDef",
+DescribeStorageSystemResourcesResponseOutputTypeDef = TypedDict(
+    "DescribeStorageSystemResourcesResponseOutputTypeDef",
     {
-        "ResourceDetails": ResourceDetailsTypeDef,
+        "ResourceDetails": ResourceDetailsOutputTypeDef,
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeStorageSystemResourceMetricsResponseTypeDef = TypedDict(
-    "DescribeStorageSystemResourceMetricsResponseTypeDef",
+DescribeStorageSystemResourceMetricsResponseOutputTypeDef = TypedDict(
+    "DescribeStorageSystemResourceMetricsResponseOutputTypeDef",
     {
-        "Metrics": List[ResourceMetricsTypeDef],
+        "Metrics": List[ResourceMetricsOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-datasync-1.28.3/mypy_boto3_datasync.egg-info/PKG-INFO` & `mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-datasync
-Version: 1.28.3
-Summary: Type annotations for boto3.DataSync 1.28.3 service generated with mypy-boto3-builder 7.14.6
+Version: 1.28.3.post1
+Summary: Type annotations for boto3.DataSync 1.28.3 service generated with mypy-boto3-builder 7.14.7
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -47,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.6](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.7](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-datasync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/).
 
 See how it helps to find and fix potential bugs:
 
@@ -391,155 +391,170 @@
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_datasync.type_defs import (
     CredentialsTypeDef,
     DiscoveryServerConfigurationTypeDef,
     TagListEntryTypeDef,
-    AddStorageSystemResponseTypeDef,
-    AgentListEntryTypeDef,
+    AddStorageSystemResponseOutputTypeDef,
+    AgentListEntryOutputTypeDef,
     CancelTaskExecutionRequestRequestTypeDef,
-    CapacityTypeDef,
-    CreateAgentResponseTypeDef,
+    CapacityOutputTypeDef,
+    CreateAgentResponseOutputTypeDef,
     Ec2ConfigTypeDef,
-    CreateLocationEfsResponseTypeDef,
-    CreateLocationFsxLustreResponseTypeDef,
-    CreateLocationFsxOntapResponseTypeDef,
-    CreateLocationFsxOpenZfsResponseTypeDef,
-    CreateLocationFsxWindowsResponseTypeDef,
+    CreateLocationEfsResponseOutputTypeDef,
+    CreateLocationFsxLustreResponseOutputTypeDef,
+    CreateLocationFsxOntapResponseOutputTypeDef,
+    CreateLocationFsxOpenZfsResponseOutputTypeDef,
+    CreateLocationFsxWindowsResponseOutputTypeDef,
     HdfsNameNodeTypeDef,
     QopConfigurationTypeDef,
-    CreateLocationHdfsResponseTypeDef,
+    CreateLocationHdfsResponseOutputTypeDef,
     NfsMountOptionsTypeDef,
     OnPremConfigTypeDef,
-    CreateLocationNfsResponseTypeDef,
-    CreateLocationObjectStorageResponseTypeDef,
+    CreateLocationNfsResponseOutputTypeDef,
+    CreateLocationObjectStorageResponseOutputTypeDef,
     S3ConfigTypeDef,
-    CreateLocationS3ResponseTypeDef,
+    CreateLocationS3ResponseOutputTypeDef,
     SmbMountOptionsTypeDef,
-    CreateLocationSmbResponseTypeDef,
+    CreateLocationSmbResponseOutputTypeDef,
     FilterRuleTypeDef,
     OptionsTypeDef,
     TaskScheduleTypeDef,
-    CreateTaskResponseTypeDef,
+    CreateTaskResponseOutputTypeDef,
     DeleteAgentRequestRequestTypeDef,
     DeleteLocationRequestRequestTypeDef,
     DeleteTaskRequestRequestTypeDef,
     DescribeAgentRequestRequestTypeDef,
-    PrivateLinkConfigTypeDef,
+    PrivateLinkConfigOutputTypeDef,
     DescribeDiscoveryJobRequestRequestTypeDef,
-    DescribeDiscoveryJobResponseTypeDef,
+    DescribeDiscoveryJobResponseOutputTypeDef,
     DescribeLocationEfsRequestRequestTypeDef,
+    Ec2ConfigOutputTypeDef,
     DescribeLocationFsxLustreRequestRequestTypeDef,
-    DescribeLocationFsxLustreResponseTypeDef,
+    DescribeLocationFsxLustreResponseOutputTypeDef,
     DescribeLocationFsxOntapRequestRequestTypeDef,
     DescribeLocationFsxOpenZfsRequestRequestTypeDef,
     DescribeLocationFsxWindowsRequestRequestTypeDef,
-    DescribeLocationFsxWindowsResponseTypeDef,
+    DescribeLocationFsxWindowsResponseOutputTypeDef,
     DescribeLocationHdfsRequestRequestTypeDef,
+    HdfsNameNodeOutputTypeDef,
+    QopConfigurationOutputTypeDef,
     DescribeLocationNfsRequestRequestTypeDef,
+    NfsMountOptionsOutputTypeDef,
+    OnPremConfigOutputTypeDef,
     DescribeLocationObjectStorageRequestRequestTypeDef,
-    DescribeLocationObjectStorageResponseTypeDef,
+    DescribeLocationObjectStorageResponseOutputTypeDef,
     DescribeLocationS3RequestRequestTypeDef,
+    S3ConfigOutputTypeDef,
     DescribeLocationSmbRequestRequestTypeDef,
+    SmbMountOptionsOutputTypeDef,
     DescribeStorageSystemRequestRequestTypeDef,
     DescribeStorageSystemResourceMetricsRequestDescribeStorageSystemResourceMetricsPaginateTypeDef,
     DescribeStorageSystemResourceMetricsRequestRequestTypeDef,
     DescribeStorageSystemResourcesRequestRequestTypeDef,
+    DiscoveryServerConfigurationOutputTypeDef,
     DescribeTaskExecutionRequestRequestTypeDef,
-    TaskExecutionResultDetailTypeDef,
+    FilterRuleOutputTypeDef,
+    OptionsOutputTypeDef,
+    TaskExecutionResultDetailOutputTypeDef,
     DescribeTaskRequestRequestTypeDef,
-    DiscoveryJobListEntryTypeDef,
+    TaskScheduleOutputTypeDef,
+    DiscoveryJobListEntryOutputTypeDef,
     GenerateRecommendationsRequestRequestTypeDef,
-    IOPSTypeDef,
-    LatencyTypeDef,
+    IOPSOutputTypeDef,
+    LatencyOutputTypeDef,
     ListAgentsRequestListAgentsPaginateTypeDef,
     ListAgentsRequestRequestTypeDef,
     ListDiscoveryJobsRequestListDiscoveryJobsPaginateTypeDef,
     ListDiscoveryJobsRequestRequestTypeDef,
     LocationFilterTypeDef,
-    LocationListEntryTypeDef,
+    LocationListEntryOutputTypeDef,
     ListStorageSystemsRequestListStorageSystemsPaginateTypeDef,
     ListStorageSystemsRequestRequestTypeDef,
-    StorageSystemListEntryTypeDef,
+    StorageSystemListEntryOutputTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagListEntryOutputTypeDef,
     ListTaskExecutionsRequestListTaskExecutionsPaginateTypeDef,
     ListTaskExecutionsRequestRequestTypeDef,
-    TaskExecutionListEntryTypeDef,
+    TaskExecutionListEntryOutputTypeDef,
     TaskFilterTypeDef,
-    TaskListEntryTypeDef,
-    MaxP95PerformanceTypeDef,
-    RecommendationTypeDef,
-    ThroughputTypeDef,
+    TaskListEntryOutputTypeDef,
+    MaxP95PerformanceOutputTypeDef,
+    RecommendationOutputTypeDef,
+    ThroughputOutputTypeDef,
     PaginatorConfigTypeDef,
     RemoveStorageSystemRequestRequestTypeDef,
     ResponseMetadataTypeDef,
-    StartDiscoveryJobResponseTypeDef,
-    StartTaskExecutionResponseTypeDef,
+    StartDiscoveryJobResponseOutputTypeDef,
+    StartTaskExecutionResponseOutputTypeDef,
     StopDiscoveryJobRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAgentRequestRequestTypeDef,
     UpdateDiscoveryJobRequestRequestTypeDef,
     UpdateLocationObjectStorageRequestRequestTypeDef,
-    DescribeStorageSystemResponseTypeDef,
     UpdateStorageSystemRequestRequestTypeDef,
     AddStorageSystemRequestRequestTypeDef,
     CreateAgentRequestRequestTypeDef,
     CreateLocationFsxLustreRequestRequestTypeDef,
     CreateLocationFsxWindowsRequestRequestTypeDef,
     CreateLocationObjectStorageRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     StartDiscoveryJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    ListAgentsResponseTypeDef,
+    ListAgentsResponseOutputTypeDef,
     CreateLocationEfsRequestRequestTypeDef,
-    DescribeLocationEfsResponseTypeDef,
     CreateLocationHdfsRequestRequestTypeDef,
-    DescribeLocationHdfsResponseTypeDef,
     UpdateLocationHdfsRequestRequestTypeDef,
     FsxProtocolNfsTypeDef,
     CreateLocationNfsRequestRequestTypeDef,
-    DescribeLocationNfsResponseTypeDef,
     UpdateLocationNfsRequestRequestTypeDef,
     CreateLocationS3RequestRequestTypeDef,
-    DescribeLocationS3ResponseTypeDef,
     CreateLocationSmbRequestRequestTypeDef,
-    DescribeLocationSmbResponseTypeDef,
     FsxProtocolSmbTypeDef,
     UpdateLocationSmbRequestRequestTypeDef,
     StartTaskExecutionRequestRequestTypeDef,
     UpdateTaskExecutionRequestRequestTypeDef,
     CreateTaskRequestRequestTypeDef,
-    DescribeTaskResponseTypeDef,
     UpdateTaskRequestRequestTypeDef,
-    DescribeAgentResponseTypeDef,
-    DescribeTaskExecutionResponseTypeDef,
-    ListDiscoveryJobsResponseTypeDef,
+    DescribeAgentResponseOutputTypeDef,
+    DescribeLocationEfsResponseOutputTypeDef,
+    DescribeLocationHdfsResponseOutputTypeDef,
+    FsxProtocolNfsOutputTypeDef,
+    DescribeLocationNfsResponseOutputTypeDef,
+    DescribeLocationS3ResponseOutputTypeDef,
+    DescribeLocationSmbResponseOutputTypeDef,
+    FsxProtocolSmbOutputTypeDef,
+    DescribeStorageSystemResponseOutputTypeDef,
+    DescribeTaskExecutionResponseOutputTypeDef,
+    DescribeTaskResponseOutputTypeDef,
+    ListDiscoveryJobsResponseOutputTypeDef,
     ListLocationsRequestListLocationsPaginateTypeDef,
     ListLocationsRequestRequestTypeDef,
-    ListLocationsResponseTypeDef,
-    ListStorageSystemsResponseTypeDef,
-    ListTaskExecutionsResponseTypeDef,
+    ListLocationsResponseOutputTypeDef,
+    ListStorageSystemsResponseOutputTypeDef,
+    ListTagsForResourceResponseOutputTypeDef,
+    ListTaskExecutionsResponseOutputTypeDef,
     ListTasksRequestListTasksPaginateTypeDef,
     ListTasksRequestRequestTypeDef,
-    ListTasksResponseTypeDef,
-    NetAppONTAPClusterTypeDef,
-    NetAppONTAPSVMTypeDef,
-    NetAppONTAPVolumeTypeDef,
-    P95MetricsTypeDef,
+    ListTasksResponseOutputTypeDef,
+    NetAppONTAPClusterOutputTypeDef,
+    NetAppONTAPSVMOutputTypeDef,
+    NetAppONTAPVolumeOutputTypeDef,
+    P95MetricsOutputTypeDef,
     FsxProtocolTypeDef,
-    ResourceDetailsTypeDef,
-    ResourceMetricsTypeDef,
+    FsxProtocolOutputTypeDef,
+    ResourceDetailsOutputTypeDef,
+    ResourceMetricsOutputTypeDef,
     CreateLocationFsxOntapRequestRequestTypeDef,
     CreateLocationFsxOpenZfsRequestRequestTypeDef,
-    DescribeLocationFsxOntapResponseTypeDef,
-    DescribeLocationFsxOpenZfsResponseTypeDef,
-    DescribeStorageSystemResourcesResponseTypeDef,
-    DescribeStorageSystemResourceMetricsResponseTypeDef,
+    DescribeLocationFsxOntapResponseOutputTypeDef,
+    DescribeLocationFsxOpenZfsResponseOutputTypeDef,
+    DescribeStorageSystemResourcesResponseOutputTypeDef,
+    DescribeStorageSystemResourceMetricsResponseOutputTypeDef,
 )
 
 
 def get_structure() -> CredentialsTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-datasync-1.28.3/mypy_boto3_datasync.egg-info/SOURCES.txt` & `mypy-boto3-datasync-1.28.3.post1/mypy_boto3_datasync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datasync-1.28.3/setup.py` & `mypy-boto3-datasync-1.28.3.post1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-datasync",
-    version="1.28.3",
+    version="1.28.3.post1",
     packages=["mypy_boto3_datasync"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.DataSync 1.28.3 service generated with mypy-boto3-builder"
-        " 7.14.6"
+        " 7.14.7"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

