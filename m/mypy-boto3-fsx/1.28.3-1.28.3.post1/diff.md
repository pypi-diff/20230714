# Comparing `tmp/mypy-boto3-fsx-1.28.3.tar.gz` & `tmp/mypy-boto3-fsx-1.28.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-fsx-1.28.3.tar", last modified: Thu Jul 13 19:49:12 2023, max compression
+gzip compressed data, was "mypy-boto3-fsx-1.28.3.post1.tar", last modified: Fri Jul 14 16:17:59 2023, max compression
```

## Comparing `mypy-boto3-fsx-1.28.3.tar` & `mypy-boto3-fsx-1.28.3.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:12.653227 mypy-boto3-fsx-1.28.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-13 19:48:05.000000 mypy-boto3-fsx-1.28.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22284 2023-07-13 19:49:12.649227 mypy-boto3-fsx-1.28.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20815 2023-07-13 19:48:05.000000 mypy-boto3-fsx-1.28.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:12.645227 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-13 19:48:05.000000 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-13 19:48:05.000000 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-13 19:48:05.000000 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38786 2023-07-13 19:48:06.000000 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    38733 2023-07-13 19:48:06.000000 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15330 2023-07-13 19:48:06.000000 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15328 2023-07-13 19:48:06.000000 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-07-13 19:48:06.000000 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-07-13 19:48:06.000000 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:48:05.000000 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    79886 2023-07-13 19:48:08.000000 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    79797 2023-07-13 19:48:07.000000 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 19:48:05.000000 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:12.649227 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22284 2023-07-13 19:49:12.000000 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-13 19:49:12.000000 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:12.000000 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:12.000000 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-13 19:49:12.000000 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 19:49:12.000000 mypy-boto3-fsx-1.28.3/mypy_boto3_fsx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 19:49:12.653227 mypy-boto3-fsx-1.28.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-13 19:48:05.000000 mypy-boto3-fsx-1.28.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:59.895360 mypy-boto3-fsx-1.28.3.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-14 16:16:37.000000 mypy-boto3-fsx-1.28.3.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23371 2023-07-14 16:17:59.895360 mypy-boto3-fsx-1.28.3.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21896 2023-07-14 16:16:37.000000 mypy-boto3-fsx-1.28.3.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:59.891360 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-14 16:16:37.000000 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-14 16:16:37.000000 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-14 16:16:37.000000 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39254 2023-07-14 16:16:37.000000 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39201 2023-07-14 16:16:37.000000 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15330 2023-07-14 16:16:38.000000 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15328 2023-07-14 16:16:38.000000 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-07-14 16:16:37.000000 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-07-14 16:16:37.000000 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:16:37.000000 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    85904 2023-07-14 16:16:40.000000 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85811 2023-07-14 16:16:39.000000 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-14 16:16:37.000000 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:59.895360 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23371 2023-07-14 16:17:59.000000 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-14 16:17:59.000000 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:17:59.000000 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:17:59.000000 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-14 16:17:59.000000 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-14 16:17:59.000000 mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 16:17:59.895360 mypy-boto3-fsx-1.28.3.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-14 16:16:37.000000 mypy-boto3-fsx-1.28.3.post1/setup.py
```

### Comparing `mypy-boto3-fsx-1.28.3/LICENSE` & `mypy-boto3-fsx-1.28.3.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.28.3/PKG-INFO` & `mypy-boto3-fsx-1.28.3.post1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-fsx
-Version: 1.28.3
-Summary: Type annotations for boto3.FSx 1.28.3 service generated with mypy-boto3-builder 7.14.6
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 fsx type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-fsx"></a>
 
 # mypy-boto3-fsx
 
 [![PyPI - mypy-boto3-fsx](https://img.shields.io/pypi/v/mypy-boto3-fsx.svg?color=blue)](https://pypi.org/project/mypy-boto3-fsx)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fsx.svg?color=blue)](https://pypi.org/project/mypy-boto3-fsx)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/)
@@ -47,15 +15,15 @@
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
 [mypy-boto3-fsx docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/).
 
 See how it helps to find and fix potential bugs:
 
@@ -393,199 +361,214 @@
 ### Typed dictionaries
 
 `mypy_boto3_fsx.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_fsx.type_defs import (
-    ActiveDirectoryBackupAttributesTypeDef,
-    AdministrativeActionFailureDetailsTypeDef,
-    AliasTypeDef,
+    ActiveDirectoryBackupAttributesOutputTypeDef,
+    AdministrativeActionFailureDetailsOutputTypeDef,
+    AliasOutputTypeDef,
     AssociateFileSystemAliasesRequestRequestTypeDef,
+    AutoExportPolicyOutputTypeDef,
     AutoExportPolicyTypeDef,
+    AutoImportPolicyOutputTypeDef,
     AutoImportPolicyTypeDef,
+    AutocommitPeriodOutputTypeDef,
     AutocommitPeriodTypeDef,
-    BackupFailureDetailsTypeDef,
-    TagTypeDef,
+    BackupFailureDetailsOutputTypeDef,
+    TagOutputTypeDef,
     CancelDataRepositoryTaskRequestRequestTypeDef,
-    CancelDataRepositoryTaskResponseTypeDef,
+    CancelDataRepositoryTaskResponseOutputTypeDef,
+    CompletionReportOutputTypeDef,
     CompletionReportTypeDef,
+    TagTypeDef,
     FileCacheLustreMetadataConfigurationTypeDef,
-    CreateFileSystemFromBackupResponseTypeDef,
+    CreateFileSystemFromBackupResponseOutputTypeDef,
     LustreLogCreateConfigurationTypeDef,
     LustreRootSquashConfigurationTypeDef,
     DiskIopsConfigurationTypeDef,
-    CreateFileSystemResponseTypeDef,
+    CreateFileSystemResponseOutputTypeDef,
     SelfManagedActiveDirectoryConfigurationTypeDef,
     WindowsAuditLogCreateConfigurationTypeDef,
     TieringPolicyTypeDef,
     CreateOpenZFSOriginSnapshotConfigurationTypeDef,
     OpenZFSUserOrGroupQuotaTypeDef,
-    DataRepositoryFailureDetailsTypeDef,
-    DataRepositoryTaskFailureDetailsTypeDef,
+    DataRepositoryFailureDetailsOutputTypeDef,
+    DataRepositoryTaskFailureDetailsOutputTypeDef,
     DataRepositoryTaskFilterTypeDef,
-    DataRepositoryTaskStatusTypeDef,
+    DataRepositoryTaskStatusOutputTypeDef,
     DeleteBackupRequestRequestTypeDef,
-    DeleteBackupResponseTypeDef,
+    DeleteBackupResponseOutputTypeDef,
     DeleteDataRepositoryAssociationRequestRequestTypeDef,
-    DeleteDataRepositoryAssociationResponseTypeDef,
+    DeleteDataRepositoryAssociationResponseOutputTypeDef,
     DeleteFileCacheRequestRequestTypeDef,
-    DeleteFileCacheResponseTypeDef,
+    DeleteFileCacheResponseOutputTypeDef,
     DeleteSnapshotRequestRequestTypeDef,
-    DeleteSnapshotResponseTypeDef,
+    DeleteSnapshotResponseOutputTypeDef,
     DeleteStorageVirtualMachineRequestRequestTypeDef,
-    DeleteStorageVirtualMachineResponseTypeDef,
+    DeleteStorageVirtualMachineResponseOutputTypeDef,
     DeleteVolumeOpenZFSConfigurationTypeDef,
     FilterTypeDef,
     DescribeFileCachesRequestRequestTypeDef,
     DescribeFileSystemAliasesRequestRequestTypeDef,
     DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef,
     DescribeFileSystemsRequestRequestTypeDef,
-    DescribeFileSystemsResponseTypeDef,
+    DescribeFileSystemsResponseOutputTypeDef,
     SnapshotFilterTypeDef,
     StorageVirtualMachineFilterTypeDef,
     VolumeFilterTypeDef,
     DisassociateFileSystemAliasesRequestRequestTypeDef,
-    FileCacheFailureDetailsTypeDef,
+    DiskIopsConfigurationOutputTypeDef,
+    FileCacheFailureDetailsOutputTypeDef,
     FileCacheNFSConfigurationTypeDef,
-    LustreLogConfigurationTypeDef,
-    FileSystemEndpointTypeDef,
-    FileSystemFailureDetailsTypeDef,
-    LifecycleTransitionReasonTypeDef,
+    FileCacheLustreMetadataConfigurationOutputTypeDef,
+    LustreLogConfigurationOutputTypeDef,
+    FileSystemEndpointOutputTypeDef,
+    FileSystemFailureDetailsOutputTypeDef,
+    LifecycleTransitionReasonOutputTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    LustreRootSquashConfigurationOutputTypeDef,
+    TieringPolicyOutputTypeDef,
+    OpenZFSClientConfigurationOutputTypeDef,
     OpenZFSClientConfigurationTypeDef,
-    OpenZFSOriginSnapshotConfigurationTypeDef,
+    OpenZFSOriginSnapshotConfigurationOutputTypeDef,
+    OpenZFSUserOrGroupQuotaOutputTypeDef,
     PaginatorConfigTypeDef,
     ReleaseFileSystemNfsV3LocksRequestRequestTypeDef,
-    ReleaseFileSystemNfsV3LocksResponseTypeDef,
+    ReleaseFileSystemNfsV3LocksResponseOutputTypeDef,
     ResponseMetadataTypeDef,
     RestoreVolumeFromSnapshotRequestRequestTypeDef,
-    RestoreVolumeFromSnapshotResponseTypeDef,
+    RestoreVolumeFromSnapshotResponseOutputTypeDef,
+    RetentionPeriodOutputTypeDef,
     RetentionPeriodTypeDef,
-    SelfManagedActiveDirectoryAttributesTypeDef,
+    SelfManagedActiveDirectoryAttributesOutputTypeDef,
     SelfManagedActiveDirectoryConfigurationUpdatesTypeDef,
-    SvmEndpointTypeDef,
+    SvmEndpointOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFileCacheLustreConfigurationTypeDef,
-    UpdateFileSystemResponseTypeDef,
+    UpdateFileSystemResponseOutputTypeDef,
     UpdateSnapshotRequestRequestTypeDef,
-    WindowsAuditLogConfigurationTypeDef,
-    AssociateFileSystemAliasesResponseTypeDef,
-    DescribeFileSystemAliasesResponseTypeDef,
-    DisassociateFileSystemAliasesResponseTypeDef,
-    NFSDataRepositoryConfigurationTypeDef,
+    WindowsAuditLogConfigurationOutputTypeDef,
+    AssociateFileSystemAliasesResponseOutputTypeDef,
+    DescribeFileSystemAliasesResponseOutputTypeDef,
+    DisassociateFileSystemAliasesResponseOutputTypeDef,
+    NFSDataRepositoryConfigurationOutputTypeDef,
+    S3DataRepositoryConfigurationOutputTypeDef,
     S3DataRepositoryConfigurationTypeDef,
+    DeleteFileSystemLustreResponseOutputTypeDef,
+    DeleteFileSystemOpenZFSResponseOutputTypeDef,
+    DeleteFileSystemWindowsResponseOutputTypeDef,
+    DeleteVolumeOntapResponseOutputTypeDef,
+    ListTagsForResourceResponseOutputTypeDef,
     CopyBackupRequestRequestTypeDef,
     CreateBackupRequestRequestTypeDef,
+    CreateDataRepositoryTaskRequestRequestTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     DeleteFileSystemLustreConfigurationTypeDef,
-    DeleteFileSystemLustreResponseTypeDef,
     DeleteFileSystemOpenZFSConfigurationTypeDef,
-    DeleteFileSystemOpenZFSResponseTypeDef,
     DeleteFileSystemWindowsConfigurationTypeDef,
-    DeleteFileSystemWindowsResponseTypeDef,
     DeleteVolumeOntapConfigurationTypeDef,
-    DeleteVolumeOntapResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    CreateDataRepositoryTaskRequestRequestTypeDef,
     CreateFileCacheLustreConfigurationTypeDef,
     CreateFileSystemLustreConfigurationTypeDef,
     UpdateFileSystemLustreConfigurationTypeDef,
     CreateFileSystemOntapConfigurationTypeDef,
-    OpenZFSFileSystemConfigurationTypeDef,
     UpdateFileSystemOntapConfigurationTypeDef,
     UpdateFileSystemOpenZFSConfigurationTypeDef,
     CreateSvmActiveDirectoryConfigurationTypeDef,
     CreateFileSystemWindowsConfigurationTypeDef,
-    DataRepositoryConfigurationTypeDef,
+    DataRepositoryConfigurationOutputTypeDef,
     DescribeDataRepositoryTasksRequestRequestTypeDef,
-    DataRepositoryTaskTypeDef,
+    DataRepositoryTaskOutputTypeDef,
     DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
     DescribeBackupsRequestRequestTypeDef,
     DescribeDataRepositoryAssociationsRequestRequestTypeDef,
     DescribeSnapshotsRequestRequestTypeDef,
     DescribeStorageVirtualMachinesRequestDescribeStorageVirtualMachinesPaginateTypeDef,
     DescribeStorageVirtualMachinesRequestRequestTypeDef,
     DescribeVolumesRequestDescribeVolumesPaginateTypeDef,
     DescribeVolumesRequestRequestTypeDef,
+    OpenZFSFileSystemConfigurationOutputTypeDef,
     FileCacheDataRepositoryAssociationTypeDef,
-    FileCacheLustreConfigurationTypeDef,
-    FileSystemEndpointsTypeDef,
-    SnapshotTypeDef,
+    FileCacheLustreConfigurationOutputTypeDef,
+    FileSystemEndpointsOutputTypeDef,
+    SnapshotOutputTypeDef,
+    OpenZFSNfsExportOutputTypeDef,
     OpenZFSNfsExportTypeDef,
+    SnaplockRetentionPeriodOutputTypeDef,
     SnaplockRetentionPeriodTypeDef,
-    SvmActiveDirectoryConfigurationTypeDef,
+    SvmActiveDirectoryConfigurationOutputTypeDef,
     UpdateFileSystemWindowsConfigurationTypeDef,
     UpdateSvmActiveDirectoryConfigurationTypeDef,
-    SvmEndpointsTypeDef,
+    SvmEndpointsOutputTypeDef,
     UpdateFileCacheRequestRequestTypeDef,
-    WindowsFileSystemConfigurationTypeDef,
+    WindowsFileSystemConfigurationOutputTypeDef,
+    DataRepositoryAssociationOutputTypeDef,
     CreateDataRepositoryAssociationRequestRequestTypeDef,
-    DataRepositoryAssociationTypeDef,
     UpdateDataRepositoryAssociationRequestRequestTypeDef,
+    DeleteFileSystemResponseOutputTypeDef,
+    DeleteVolumeResponseOutputTypeDef,
     DeleteFileSystemRequestRequestTypeDef,
-    DeleteFileSystemResponseTypeDef,
     DeleteVolumeRequestRequestTypeDef,
-    DeleteVolumeResponseTypeDef,
     CreateStorageVirtualMachineRequestRequestTypeDef,
-    LustreFileSystemConfigurationTypeDef,
-    CreateDataRepositoryTaskResponseTypeDef,
-    DescribeDataRepositoryTasksResponseTypeDef,
+    LustreFileSystemConfigurationOutputTypeDef,
+    CreateDataRepositoryTaskResponseOutputTypeDef,
+    DescribeDataRepositoryTasksResponseOutputTypeDef,
     CreateFileCacheRequestRequestTypeDef,
-    FileCacheCreatingTypeDef,
-    FileCacheTypeDef,
-    OntapFileSystemConfigurationTypeDef,
-    CreateSnapshotResponseTypeDef,
-    DescribeSnapshotsResponseTypeDef,
-    UpdateSnapshotResponseTypeDef,
+    FileCacheCreatingOutputTypeDef,
+    FileCacheOutputTypeDef,
+    OntapFileSystemConfigurationOutputTypeDef,
+    CreateSnapshotResponseOutputTypeDef,
+    DescribeSnapshotsResponseOutputTypeDef,
+    UpdateSnapshotResponseOutputTypeDef,
+    OpenZFSVolumeConfigurationOutputTypeDef,
     CreateOpenZFSVolumeConfigurationTypeDef,
     OpenZFSCreateRootVolumeConfigurationTypeDef,
-    OpenZFSVolumeConfigurationTypeDef,
     UpdateOpenZFSVolumeConfigurationTypeDef,
+    SnaplockConfigurationOutputTypeDef,
     CreateSnaplockConfigurationTypeDef,
-    SnaplockConfigurationTypeDef,
     UpdateSnaplockConfigurationTypeDef,
     UpdateFileSystemRequestRequestTypeDef,
     UpdateStorageVirtualMachineRequestRequestTypeDef,
-    StorageVirtualMachineTypeDef,
-    CreateDataRepositoryAssociationResponseTypeDef,
-    DescribeDataRepositoryAssociationsResponseTypeDef,
-    UpdateDataRepositoryAssociationResponseTypeDef,
-    CreateFileCacheResponseTypeDef,
-    DescribeFileCachesResponseTypeDef,
-    UpdateFileCacheResponseTypeDef,
-    FileSystemTypeDef,
+    StorageVirtualMachineOutputTypeDef,
+    CreateDataRepositoryAssociationResponseOutputTypeDef,
+    DescribeDataRepositoryAssociationsResponseOutputTypeDef,
+    UpdateDataRepositoryAssociationResponseOutputTypeDef,
+    CreateFileCacheResponseOutputTypeDef,
+    DescribeFileCachesResponseOutputTypeDef,
+    UpdateFileCacheResponseOutputTypeDef,
+    FileSystemOutputTypeDef,
     CreateFileSystemOpenZFSConfigurationTypeDef,
+    OntapVolumeConfigurationOutputTypeDef,
     CreateOntapVolumeConfigurationTypeDef,
-    OntapVolumeConfigurationTypeDef,
     UpdateOntapVolumeConfigurationTypeDef,
-    CreateStorageVirtualMachineResponseTypeDef,
-    DescribeStorageVirtualMachinesResponseTypeDef,
-    UpdateStorageVirtualMachineResponseTypeDef,
+    CreateStorageVirtualMachineResponseOutputTypeDef,
+    DescribeStorageVirtualMachinesResponseOutputTypeDef,
+    UpdateStorageVirtualMachineResponseOutputTypeDef,
     CreateFileSystemFromBackupRequestRequestTypeDef,
     CreateFileSystemRequestRequestTypeDef,
+    VolumeOutputTypeDef,
     CreateVolumeFromBackupRequestRequestTypeDef,
     CreateVolumeRequestRequestTypeDef,
-    VolumeTypeDef,
     UpdateVolumeRequestRequestTypeDef,
-    AdministrativeActionTypeDef,
-    BackupTypeDef,
-    CreateVolumeFromBackupResponseTypeDef,
-    CreateVolumeResponseTypeDef,
-    DescribeVolumesResponseTypeDef,
-    UpdateVolumeResponseTypeDef,
-    CopyBackupResponseTypeDef,
-    CreateBackupResponseTypeDef,
-    DescribeBackupsResponseTypeDef,
+    AdministrativeActionOutputTypeDef,
+    BackupOutputTypeDef,
+    CreateVolumeFromBackupResponseOutputTypeDef,
+    CreateVolumeResponseOutputTypeDef,
+    DescribeVolumesResponseOutputTypeDef,
+    UpdateVolumeResponseOutputTypeDef,
+    CopyBackupResponseOutputTypeDef,
+    CreateBackupResponseOutputTypeDef,
+    DescribeBackupsResponseOutputTypeDef,
 )
 
 
-def get_structure() -> ActiveDirectoryBackupAttributesTypeDef:
+def get_structure() -> ActiveDirectoryBackupAttributesOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-fsx-1.28.3/README.md` & `mypy-boto3-fsx-1.28.3.post1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-fsx
+Version: 1.28.3.post1
+Summary: Type annotations for boto3.FSx 1.28.3 service generated with mypy-boto3-builder 7.14.7
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 fsx type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-fsx"></a>
 
 # mypy-boto3-fsx
 
 [![PyPI - mypy-boto3-fsx](https://img.shields.io/pypi/v/mypy-boto3-fsx.svg?color=blue)](https://pypi.org/project/mypy-boto3-fsx)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fsx.svg?color=blue)](https://pypi.org/project/mypy-boto3-fsx)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/)
@@ -15,15 +47,15 @@
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
 [mypy-boto3-fsx docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/).
 
 See how it helps to find and fix potential bugs:
 
@@ -361,199 +393,214 @@
 ### Typed dictionaries
 
 `mypy_boto3_fsx.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_fsx.type_defs import (
-    ActiveDirectoryBackupAttributesTypeDef,
-    AdministrativeActionFailureDetailsTypeDef,
-    AliasTypeDef,
+    ActiveDirectoryBackupAttributesOutputTypeDef,
+    AdministrativeActionFailureDetailsOutputTypeDef,
+    AliasOutputTypeDef,
     AssociateFileSystemAliasesRequestRequestTypeDef,
+    AutoExportPolicyOutputTypeDef,
     AutoExportPolicyTypeDef,
+    AutoImportPolicyOutputTypeDef,
     AutoImportPolicyTypeDef,
+    AutocommitPeriodOutputTypeDef,
     AutocommitPeriodTypeDef,
-    BackupFailureDetailsTypeDef,
-    TagTypeDef,
+    BackupFailureDetailsOutputTypeDef,
+    TagOutputTypeDef,
     CancelDataRepositoryTaskRequestRequestTypeDef,
-    CancelDataRepositoryTaskResponseTypeDef,
+    CancelDataRepositoryTaskResponseOutputTypeDef,
+    CompletionReportOutputTypeDef,
     CompletionReportTypeDef,
+    TagTypeDef,
     FileCacheLustreMetadataConfigurationTypeDef,
-    CreateFileSystemFromBackupResponseTypeDef,
+    CreateFileSystemFromBackupResponseOutputTypeDef,
     LustreLogCreateConfigurationTypeDef,
     LustreRootSquashConfigurationTypeDef,
     DiskIopsConfigurationTypeDef,
-    CreateFileSystemResponseTypeDef,
+    CreateFileSystemResponseOutputTypeDef,
     SelfManagedActiveDirectoryConfigurationTypeDef,
     WindowsAuditLogCreateConfigurationTypeDef,
     TieringPolicyTypeDef,
     CreateOpenZFSOriginSnapshotConfigurationTypeDef,
     OpenZFSUserOrGroupQuotaTypeDef,
-    DataRepositoryFailureDetailsTypeDef,
-    DataRepositoryTaskFailureDetailsTypeDef,
+    DataRepositoryFailureDetailsOutputTypeDef,
+    DataRepositoryTaskFailureDetailsOutputTypeDef,
     DataRepositoryTaskFilterTypeDef,
-    DataRepositoryTaskStatusTypeDef,
+    DataRepositoryTaskStatusOutputTypeDef,
     DeleteBackupRequestRequestTypeDef,
-    DeleteBackupResponseTypeDef,
+    DeleteBackupResponseOutputTypeDef,
     DeleteDataRepositoryAssociationRequestRequestTypeDef,
-    DeleteDataRepositoryAssociationResponseTypeDef,
+    DeleteDataRepositoryAssociationResponseOutputTypeDef,
     DeleteFileCacheRequestRequestTypeDef,
-    DeleteFileCacheResponseTypeDef,
+    DeleteFileCacheResponseOutputTypeDef,
     DeleteSnapshotRequestRequestTypeDef,
-    DeleteSnapshotResponseTypeDef,
+    DeleteSnapshotResponseOutputTypeDef,
     DeleteStorageVirtualMachineRequestRequestTypeDef,
-    DeleteStorageVirtualMachineResponseTypeDef,
+    DeleteStorageVirtualMachineResponseOutputTypeDef,
     DeleteVolumeOpenZFSConfigurationTypeDef,
     FilterTypeDef,
     DescribeFileCachesRequestRequestTypeDef,
     DescribeFileSystemAliasesRequestRequestTypeDef,
     DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef,
     DescribeFileSystemsRequestRequestTypeDef,
-    DescribeFileSystemsResponseTypeDef,
+    DescribeFileSystemsResponseOutputTypeDef,
     SnapshotFilterTypeDef,
     StorageVirtualMachineFilterTypeDef,
     VolumeFilterTypeDef,
     DisassociateFileSystemAliasesRequestRequestTypeDef,
-    FileCacheFailureDetailsTypeDef,
+    DiskIopsConfigurationOutputTypeDef,
+    FileCacheFailureDetailsOutputTypeDef,
     FileCacheNFSConfigurationTypeDef,
-    LustreLogConfigurationTypeDef,
-    FileSystemEndpointTypeDef,
-    FileSystemFailureDetailsTypeDef,
-    LifecycleTransitionReasonTypeDef,
+    FileCacheLustreMetadataConfigurationOutputTypeDef,
+    LustreLogConfigurationOutputTypeDef,
+    FileSystemEndpointOutputTypeDef,
+    FileSystemFailureDetailsOutputTypeDef,
+    LifecycleTransitionReasonOutputTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    LustreRootSquashConfigurationOutputTypeDef,
+    TieringPolicyOutputTypeDef,
+    OpenZFSClientConfigurationOutputTypeDef,
     OpenZFSClientConfigurationTypeDef,
-    OpenZFSOriginSnapshotConfigurationTypeDef,
+    OpenZFSOriginSnapshotConfigurationOutputTypeDef,
+    OpenZFSUserOrGroupQuotaOutputTypeDef,
     PaginatorConfigTypeDef,
     ReleaseFileSystemNfsV3LocksRequestRequestTypeDef,
-    ReleaseFileSystemNfsV3LocksResponseTypeDef,
+    ReleaseFileSystemNfsV3LocksResponseOutputTypeDef,
     ResponseMetadataTypeDef,
     RestoreVolumeFromSnapshotRequestRequestTypeDef,
-    RestoreVolumeFromSnapshotResponseTypeDef,
+    RestoreVolumeFromSnapshotResponseOutputTypeDef,
+    RetentionPeriodOutputTypeDef,
     RetentionPeriodTypeDef,
-    SelfManagedActiveDirectoryAttributesTypeDef,
+    SelfManagedActiveDirectoryAttributesOutputTypeDef,
     SelfManagedActiveDirectoryConfigurationUpdatesTypeDef,
-    SvmEndpointTypeDef,
+    SvmEndpointOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFileCacheLustreConfigurationTypeDef,
-    UpdateFileSystemResponseTypeDef,
+    UpdateFileSystemResponseOutputTypeDef,
     UpdateSnapshotRequestRequestTypeDef,
-    WindowsAuditLogConfigurationTypeDef,
-    AssociateFileSystemAliasesResponseTypeDef,
-    DescribeFileSystemAliasesResponseTypeDef,
-    DisassociateFileSystemAliasesResponseTypeDef,
-    NFSDataRepositoryConfigurationTypeDef,
+    WindowsAuditLogConfigurationOutputTypeDef,
+    AssociateFileSystemAliasesResponseOutputTypeDef,
+    DescribeFileSystemAliasesResponseOutputTypeDef,
+    DisassociateFileSystemAliasesResponseOutputTypeDef,
+    NFSDataRepositoryConfigurationOutputTypeDef,
+    S3DataRepositoryConfigurationOutputTypeDef,
     S3DataRepositoryConfigurationTypeDef,
+    DeleteFileSystemLustreResponseOutputTypeDef,
+    DeleteFileSystemOpenZFSResponseOutputTypeDef,
+    DeleteFileSystemWindowsResponseOutputTypeDef,
+    DeleteVolumeOntapResponseOutputTypeDef,
+    ListTagsForResourceResponseOutputTypeDef,
     CopyBackupRequestRequestTypeDef,
     CreateBackupRequestRequestTypeDef,
+    CreateDataRepositoryTaskRequestRequestTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     DeleteFileSystemLustreConfigurationTypeDef,
-    DeleteFileSystemLustreResponseTypeDef,
     DeleteFileSystemOpenZFSConfigurationTypeDef,
-    DeleteFileSystemOpenZFSResponseTypeDef,
     DeleteFileSystemWindowsConfigurationTypeDef,
-    DeleteFileSystemWindowsResponseTypeDef,
     DeleteVolumeOntapConfigurationTypeDef,
-    DeleteVolumeOntapResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    CreateDataRepositoryTaskRequestRequestTypeDef,
     CreateFileCacheLustreConfigurationTypeDef,
     CreateFileSystemLustreConfigurationTypeDef,
     UpdateFileSystemLustreConfigurationTypeDef,
     CreateFileSystemOntapConfigurationTypeDef,
-    OpenZFSFileSystemConfigurationTypeDef,
     UpdateFileSystemOntapConfigurationTypeDef,
     UpdateFileSystemOpenZFSConfigurationTypeDef,
     CreateSvmActiveDirectoryConfigurationTypeDef,
     CreateFileSystemWindowsConfigurationTypeDef,
-    DataRepositoryConfigurationTypeDef,
+    DataRepositoryConfigurationOutputTypeDef,
     DescribeDataRepositoryTasksRequestRequestTypeDef,
-    DataRepositoryTaskTypeDef,
+    DataRepositoryTaskOutputTypeDef,
     DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
     DescribeBackupsRequestRequestTypeDef,
     DescribeDataRepositoryAssociationsRequestRequestTypeDef,
     DescribeSnapshotsRequestRequestTypeDef,
     DescribeStorageVirtualMachinesRequestDescribeStorageVirtualMachinesPaginateTypeDef,
     DescribeStorageVirtualMachinesRequestRequestTypeDef,
     DescribeVolumesRequestDescribeVolumesPaginateTypeDef,
     DescribeVolumesRequestRequestTypeDef,
+    OpenZFSFileSystemConfigurationOutputTypeDef,
     FileCacheDataRepositoryAssociationTypeDef,
-    FileCacheLustreConfigurationTypeDef,
-    FileSystemEndpointsTypeDef,
-    SnapshotTypeDef,
+    FileCacheLustreConfigurationOutputTypeDef,
+    FileSystemEndpointsOutputTypeDef,
+    SnapshotOutputTypeDef,
+    OpenZFSNfsExportOutputTypeDef,
     OpenZFSNfsExportTypeDef,
+    SnaplockRetentionPeriodOutputTypeDef,
     SnaplockRetentionPeriodTypeDef,
-    SvmActiveDirectoryConfigurationTypeDef,
+    SvmActiveDirectoryConfigurationOutputTypeDef,
     UpdateFileSystemWindowsConfigurationTypeDef,
     UpdateSvmActiveDirectoryConfigurationTypeDef,
-    SvmEndpointsTypeDef,
+    SvmEndpointsOutputTypeDef,
     UpdateFileCacheRequestRequestTypeDef,
-    WindowsFileSystemConfigurationTypeDef,
+    WindowsFileSystemConfigurationOutputTypeDef,
+    DataRepositoryAssociationOutputTypeDef,
     CreateDataRepositoryAssociationRequestRequestTypeDef,
-    DataRepositoryAssociationTypeDef,
     UpdateDataRepositoryAssociationRequestRequestTypeDef,
+    DeleteFileSystemResponseOutputTypeDef,
+    DeleteVolumeResponseOutputTypeDef,
     DeleteFileSystemRequestRequestTypeDef,
-    DeleteFileSystemResponseTypeDef,
     DeleteVolumeRequestRequestTypeDef,
-    DeleteVolumeResponseTypeDef,
     CreateStorageVirtualMachineRequestRequestTypeDef,
-    LustreFileSystemConfigurationTypeDef,
-    CreateDataRepositoryTaskResponseTypeDef,
-    DescribeDataRepositoryTasksResponseTypeDef,
+    LustreFileSystemConfigurationOutputTypeDef,
+    CreateDataRepositoryTaskResponseOutputTypeDef,
+    DescribeDataRepositoryTasksResponseOutputTypeDef,
     CreateFileCacheRequestRequestTypeDef,
-    FileCacheCreatingTypeDef,
-    FileCacheTypeDef,
-    OntapFileSystemConfigurationTypeDef,
-    CreateSnapshotResponseTypeDef,
-    DescribeSnapshotsResponseTypeDef,
-    UpdateSnapshotResponseTypeDef,
+    FileCacheCreatingOutputTypeDef,
+    FileCacheOutputTypeDef,
+    OntapFileSystemConfigurationOutputTypeDef,
+    CreateSnapshotResponseOutputTypeDef,
+    DescribeSnapshotsResponseOutputTypeDef,
+    UpdateSnapshotResponseOutputTypeDef,
+    OpenZFSVolumeConfigurationOutputTypeDef,
     CreateOpenZFSVolumeConfigurationTypeDef,
     OpenZFSCreateRootVolumeConfigurationTypeDef,
-    OpenZFSVolumeConfigurationTypeDef,
     UpdateOpenZFSVolumeConfigurationTypeDef,
+    SnaplockConfigurationOutputTypeDef,
     CreateSnaplockConfigurationTypeDef,
-    SnaplockConfigurationTypeDef,
     UpdateSnaplockConfigurationTypeDef,
     UpdateFileSystemRequestRequestTypeDef,
     UpdateStorageVirtualMachineRequestRequestTypeDef,
-    StorageVirtualMachineTypeDef,
-    CreateDataRepositoryAssociationResponseTypeDef,
-    DescribeDataRepositoryAssociationsResponseTypeDef,
-    UpdateDataRepositoryAssociationResponseTypeDef,
-    CreateFileCacheResponseTypeDef,
-    DescribeFileCachesResponseTypeDef,
-    UpdateFileCacheResponseTypeDef,
-    FileSystemTypeDef,
+    StorageVirtualMachineOutputTypeDef,
+    CreateDataRepositoryAssociationResponseOutputTypeDef,
+    DescribeDataRepositoryAssociationsResponseOutputTypeDef,
+    UpdateDataRepositoryAssociationResponseOutputTypeDef,
+    CreateFileCacheResponseOutputTypeDef,
+    DescribeFileCachesResponseOutputTypeDef,
+    UpdateFileCacheResponseOutputTypeDef,
+    FileSystemOutputTypeDef,
     CreateFileSystemOpenZFSConfigurationTypeDef,
+    OntapVolumeConfigurationOutputTypeDef,
     CreateOntapVolumeConfigurationTypeDef,
-    OntapVolumeConfigurationTypeDef,
     UpdateOntapVolumeConfigurationTypeDef,
-    CreateStorageVirtualMachineResponseTypeDef,
-    DescribeStorageVirtualMachinesResponseTypeDef,
-    UpdateStorageVirtualMachineResponseTypeDef,
+    CreateStorageVirtualMachineResponseOutputTypeDef,
+    DescribeStorageVirtualMachinesResponseOutputTypeDef,
+    UpdateStorageVirtualMachineResponseOutputTypeDef,
     CreateFileSystemFromBackupRequestRequestTypeDef,
     CreateFileSystemRequestRequestTypeDef,
+    VolumeOutputTypeDef,
     CreateVolumeFromBackupRequestRequestTypeDef,
     CreateVolumeRequestRequestTypeDef,
-    VolumeTypeDef,
     UpdateVolumeRequestRequestTypeDef,
-    AdministrativeActionTypeDef,
-    BackupTypeDef,
-    CreateVolumeFromBackupResponseTypeDef,
-    CreateVolumeResponseTypeDef,
-    DescribeVolumesResponseTypeDef,
-    UpdateVolumeResponseTypeDef,
-    CopyBackupResponseTypeDef,
-    CreateBackupResponseTypeDef,
-    DescribeBackupsResponseTypeDef,
+    AdministrativeActionOutputTypeDef,
+    BackupOutputTypeDef,
+    CreateVolumeFromBackupResponseOutputTypeDef,
+    CreateVolumeResponseOutputTypeDef,
+    DescribeVolumesResponseOutputTypeDef,
+    UpdateVolumeResponseOutputTypeDef,
+    CopyBackupResponseOutputTypeDef,
+    CreateBackupResponseOutputTypeDef,
+    DescribeBackupsResponseOutputTypeDef,
 )
 
 
-def get_structure() -> ActiveDirectoryBackupAttributesTypeDef:
+def get_structure() -> ActiveDirectoryBackupAttributesOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/__init__.py` & `mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/__init__.pyi` & `mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/__main__.py` & `mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.FSx 1.28.3\nVersion:         1.28.3\nBuilder version:"
-        " 7.14.6\nDocs:           "
+        "Type annotations for boto3.FSx 1.28.3\nVersion:         1.28.3.post1\nBuilder version:"
+        " 7.14.7\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx\nOther"
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

### Comparing `mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/client.py` & `mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,82 +30,82 @@
     DescribeBackupsPaginator,
     DescribeFileSystemsPaginator,
     DescribeStorageVirtualMachinesPaginator,
     DescribeVolumesPaginator,
     ListTagsForResourcePaginator,
 )
 from .type_defs import (
-    AssociateFileSystemAliasesResponseTypeDef,
-    CancelDataRepositoryTaskResponseTypeDef,
+    AssociateFileSystemAliasesResponseOutputTypeDef,
+    CancelDataRepositoryTaskResponseOutputTypeDef,
     CompletionReportTypeDef,
-    CopyBackupResponseTypeDef,
-    CreateBackupResponseTypeDef,
-    CreateDataRepositoryAssociationResponseTypeDef,
-    CreateDataRepositoryTaskResponseTypeDef,
+    CopyBackupResponseOutputTypeDef,
+    CreateBackupResponseOutputTypeDef,
+    CreateDataRepositoryAssociationResponseOutputTypeDef,
+    CreateDataRepositoryTaskResponseOutputTypeDef,
     CreateFileCacheLustreConfigurationTypeDef,
-    CreateFileCacheResponseTypeDef,
-    CreateFileSystemFromBackupResponseTypeDef,
+    CreateFileCacheResponseOutputTypeDef,
+    CreateFileSystemFromBackupResponseOutputTypeDef,
     CreateFileSystemLustreConfigurationTypeDef,
     CreateFileSystemOntapConfigurationTypeDef,
     CreateFileSystemOpenZFSConfigurationTypeDef,
-    CreateFileSystemResponseTypeDef,
+    CreateFileSystemResponseOutputTypeDef,
     CreateFileSystemWindowsConfigurationTypeDef,
     CreateOntapVolumeConfigurationTypeDef,
     CreateOpenZFSVolumeConfigurationTypeDef,
-    CreateSnapshotResponseTypeDef,
-    CreateStorageVirtualMachineResponseTypeDef,
+    CreateSnapshotResponseOutputTypeDef,
+    CreateStorageVirtualMachineResponseOutputTypeDef,
     CreateSvmActiveDirectoryConfigurationTypeDef,
-    CreateVolumeFromBackupResponseTypeDef,
-    CreateVolumeResponseTypeDef,
+    CreateVolumeFromBackupResponseOutputTypeDef,
+    CreateVolumeResponseOutputTypeDef,
     DataRepositoryTaskFilterTypeDef,
-    DeleteBackupResponseTypeDef,
-    DeleteDataRepositoryAssociationResponseTypeDef,
-    DeleteFileCacheResponseTypeDef,
+    DeleteBackupResponseOutputTypeDef,
+    DeleteDataRepositoryAssociationResponseOutputTypeDef,
+    DeleteFileCacheResponseOutputTypeDef,
     DeleteFileSystemLustreConfigurationTypeDef,
     DeleteFileSystemOpenZFSConfigurationTypeDef,
-    DeleteFileSystemResponseTypeDef,
+    DeleteFileSystemResponseOutputTypeDef,
     DeleteFileSystemWindowsConfigurationTypeDef,
-    DeleteSnapshotResponseTypeDef,
-    DeleteStorageVirtualMachineResponseTypeDef,
+    DeleteSnapshotResponseOutputTypeDef,
+    DeleteStorageVirtualMachineResponseOutputTypeDef,
     DeleteVolumeOntapConfigurationTypeDef,
     DeleteVolumeOpenZFSConfigurationTypeDef,
-    DeleteVolumeResponseTypeDef,
-    DescribeBackupsResponseTypeDef,
-    DescribeDataRepositoryAssociationsResponseTypeDef,
-    DescribeDataRepositoryTasksResponseTypeDef,
-    DescribeFileCachesResponseTypeDef,
-    DescribeFileSystemAliasesResponseTypeDef,
-    DescribeFileSystemsResponseTypeDef,
-    DescribeSnapshotsResponseTypeDef,
-    DescribeStorageVirtualMachinesResponseTypeDef,
-    DescribeVolumesResponseTypeDef,
-    DisassociateFileSystemAliasesResponseTypeDef,
+    DeleteVolumeResponseOutputTypeDef,
+    DescribeBackupsResponseOutputTypeDef,
+    DescribeDataRepositoryAssociationsResponseOutputTypeDef,
+    DescribeDataRepositoryTasksResponseOutputTypeDef,
+    DescribeFileCachesResponseOutputTypeDef,
+    DescribeFileSystemAliasesResponseOutputTypeDef,
+    DescribeFileSystemsResponseOutputTypeDef,
+    DescribeSnapshotsResponseOutputTypeDef,
+    DescribeStorageVirtualMachinesResponseOutputTypeDef,
+    DescribeVolumesResponseOutputTypeDef,
+    DisassociateFileSystemAliasesResponseOutputTypeDef,
     FileCacheDataRepositoryAssociationTypeDef,
     FilterTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ReleaseFileSystemNfsV3LocksResponseTypeDef,
-    RestoreVolumeFromSnapshotResponseTypeDef,
+    ListTagsForResourceResponseOutputTypeDef,
+    ReleaseFileSystemNfsV3LocksResponseOutputTypeDef,
+    RestoreVolumeFromSnapshotResponseOutputTypeDef,
     S3DataRepositoryConfigurationTypeDef,
     SnapshotFilterTypeDef,
     StorageVirtualMachineFilterTypeDef,
     TagTypeDef,
-    UpdateDataRepositoryAssociationResponseTypeDef,
+    UpdateDataRepositoryAssociationResponseOutputTypeDef,
     UpdateFileCacheLustreConfigurationTypeDef,
-    UpdateFileCacheResponseTypeDef,
+    UpdateFileCacheResponseOutputTypeDef,
     UpdateFileSystemLustreConfigurationTypeDef,
     UpdateFileSystemOntapConfigurationTypeDef,
     UpdateFileSystemOpenZFSConfigurationTypeDef,
-    UpdateFileSystemResponseTypeDef,
+    UpdateFileSystemResponseOutputTypeDef,
     UpdateFileSystemWindowsConfigurationTypeDef,
     UpdateOntapVolumeConfigurationTypeDef,
     UpdateOpenZFSVolumeConfigurationTypeDef,
-    UpdateSnapshotResponseTypeDef,
-    UpdateStorageVirtualMachineResponseTypeDef,
+    UpdateSnapshotResponseOutputTypeDef,
+    UpdateStorageVirtualMachineResponseOutputTypeDef,
     UpdateSvmActiveDirectoryConfigurationTypeDef,
-    UpdateVolumeResponseTypeDef,
+    UpdateVolumeResponseOutputTypeDef,
     VolumeFilterTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -176,15 +176,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#exceptions)
         """
 
     def associate_file_system_aliases(
         self, *, FileSystemId: str, Aliases: Sequence[str], ClientRequestToken: str = ...
-    ) -> AssociateFileSystemAliasesResponseTypeDef:
+    ) -> AssociateFileSystemAliasesResponseOutputTypeDef:
         """
         Use this action to associate one or more Domain Name Server (DNS) aliases with
         an existing Amazon FSx for Windows File Server file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.associate_file_system_aliases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#associate_file_system_aliases)
         """
@@ -195,15 +195,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#can_paginate)
         """
 
     def cancel_data_repository_task(
         self, *, TaskId: str
-    ) -> CancelDataRepositoryTaskResponseTypeDef:
+    ) -> CancelDataRepositoryTaskResponseOutputTypeDef:
         """
         Cancels an existing Amazon FSx for Lustre data repository task if that task is
         in either the `PENDING` or `EXECUTING` state.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.cancel_data_repository_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#cancel_data_repository_task)
         """
@@ -221,15 +221,15 @@
         *,
         SourceBackupId: str,
         ClientRequestToken: str = ...,
         SourceRegion: str = ...,
         KmsKeyId: str = ...,
         CopyTags: bool = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CopyBackupResponseTypeDef:
+    ) -> CopyBackupResponseOutputTypeDef:
         """
         Copies an existing backup within the same Amazon Web Services account to another
         Amazon Web Services Region (cross-Region copy) or within the same Amazon Web
         Services Region (in-Region copy).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.copy_backup)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#copy_backup)
@@ -238,15 +238,15 @@
     def create_backup(
         self,
         *,
         FileSystemId: str = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         VolumeId: str = ...
-    ) -> CreateBackupResponseTypeDef:
+    ) -> CreateBackupResponseOutputTypeDef:
         """
         Creates a backup of an existing Amazon FSx for Windows File Server file system,
         Amazon FSx for Lustre file system, Amazon FSx for NetApp ONTAP volume, or Amazon
         FSx for OpenZFS file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_backup)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_backup)
@@ -259,15 +259,15 @@
         DataRepositoryPath: str,
         FileSystemPath: str = ...,
         BatchImportMetaDataOnCreate: bool = ...,
         ImportedFileChunkSize: int = ...,
         S3: S3DataRepositoryConfigurationTypeDef = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateDataRepositoryAssociationResponseTypeDef:
+    ) -> CreateDataRepositoryAssociationResponseOutputTypeDef:
         """
         Creates an Amazon FSx for Lustre data repository association (DRA).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_data_repository_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_data_repository_association)
         """
 
@@ -277,15 +277,15 @@
         Type: DataRepositoryTaskTypeType,
         FileSystemId: str,
         Report: CompletionReportTypeDef,
         Paths: Sequence[str] = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         CapacityToRelease: int = ...
-    ) -> CreateDataRepositoryTaskResponseTypeDef:
+    ) -> CreateDataRepositoryTaskResponseOutputTypeDef:
         """
         Creates an Amazon FSx for Lustre data repository task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_data_repository_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_data_repository_task)
         """
 
@@ -299,15 +299,15 @@
         ClientRequestToken: str = ...,
         SecurityGroupIds: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         CopyTagsToDataRepositoryAssociations: bool = ...,
         KmsKeyId: str = ...,
         LustreConfiguration: CreateFileCacheLustreConfigurationTypeDef = ...,
         DataRepositoryAssociations: Sequence[FileCacheDataRepositoryAssociationTypeDef] = ...
-    ) -> CreateFileCacheResponseTypeDef:
+    ) -> CreateFileCacheResponseOutputTypeDef:
         """
         Creates a new Amazon File Cache resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_file_cache)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_file_cache)
         """
 
@@ -323,15 +323,15 @@
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
         WindowsConfiguration: CreateFileSystemWindowsConfigurationTypeDef = ...,
         LustreConfiguration: CreateFileSystemLustreConfigurationTypeDef = ...,
         OntapConfiguration: CreateFileSystemOntapConfigurationTypeDef = ...,
         FileSystemTypeVersion: str = ...,
         OpenZFSConfiguration: CreateFileSystemOpenZFSConfigurationTypeDef = ...
-    ) -> CreateFileSystemResponseTypeDef:
+    ) -> CreateFileSystemResponseOutputTypeDef:
         """
         Creates a new, empty Amazon FSx file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_file_system)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_file_system)
         """
 
@@ -346,15 +346,15 @@
         WindowsConfiguration: CreateFileSystemWindowsConfigurationTypeDef = ...,
         LustreConfiguration: CreateFileSystemLustreConfigurationTypeDef = ...,
         StorageType: StorageTypeType = ...,
         KmsKeyId: str = ...,
         FileSystemTypeVersion: str = ...,
         OpenZFSConfiguration: CreateFileSystemOpenZFSConfigurationTypeDef = ...,
         StorageCapacity: int = ...
-    ) -> CreateFileSystemFromBackupResponseTypeDef:
+    ) -> CreateFileSystemFromBackupResponseOutputTypeDef:
         """
         Creates a new Amazon FSx for Lustre, Amazon FSx for Windows File Server, or
         Amazon FSx for OpenZFS file system from an existing Amazon FSx backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_file_system_from_backup)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_file_system_from_backup)
         """
@@ -362,15 +362,15 @@
     def create_snapshot(
         self,
         *,
         Name: str,
         VolumeId: str,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateSnapshotResponseTypeDef:
+    ) -> CreateSnapshotResponseOutputTypeDef:
         """
         Creates a snapshot of an existing Amazon FSx for OpenZFS volume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_snapshot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_snapshot)
         """
 
@@ -380,15 +380,15 @@
         FileSystemId: str,
         Name: str,
         ActiveDirectoryConfiguration: CreateSvmActiveDirectoryConfigurationTypeDef = ...,
         ClientRequestToken: str = ...,
         SvmAdminPassword: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         RootVolumeSecurityStyle: StorageVirtualMachineRootVolumeSecurityStyleType = ...
-    ) -> CreateStorageVirtualMachineResponseTypeDef:
+    ) -> CreateStorageVirtualMachineResponseOutputTypeDef:
         """
         Creates a storage virtual machine (SVM) for an Amazon FSx for ONTAP file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_storage_virtual_machine)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_storage_virtual_machine)
         """
 
@@ -397,15 +397,15 @@
         *,
         VolumeType: VolumeTypeType,
         Name: str,
         ClientRequestToken: str = ...,
         OntapConfiguration: CreateOntapVolumeConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         OpenZFSConfiguration: CreateOpenZFSVolumeConfigurationTypeDef = ...
-    ) -> CreateVolumeResponseTypeDef:
+    ) -> CreateVolumeResponseOutputTypeDef:
         """
         Creates an FSx for ONTAP or Amazon FSx for OpenZFS storage volume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_volume)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_volume)
         """
 
@@ -413,50 +413,50 @@
         self,
         *,
         BackupId: str,
         Name: str,
         ClientRequestToken: str = ...,
         OntapConfiguration: CreateOntapVolumeConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateVolumeFromBackupResponseTypeDef:
+    ) -> CreateVolumeFromBackupResponseOutputTypeDef:
         """
         Creates a new Amazon FSx for NetApp ONTAP volume from an existing Amazon FSx
         volume backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_volume_from_backup)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_volume_from_backup)
         """
 
     def delete_backup(
         self, *, BackupId: str, ClientRequestToken: str = ...
-    ) -> DeleteBackupResponseTypeDef:
+    ) -> DeleteBackupResponseOutputTypeDef:
         """
         Deletes an Amazon FSx backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.delete_backup)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#delete_backup)
         """
 
     def delete_data_repository_association(
         self,
         *,
         AssociationId: str,
         ClientRequestToken: str = ...,
         DeleteDataInFileSystem: bool = ...
-    ) -> DeleteDataRepositoryAssociationResponseTypeDef:
+    ) -> DeleteDataRepositoryAssociationResponseOutputTypeDef:
         """
         Deletes a data repository association on an Amazon FSx for Lustre file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.delete_data_repository_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#delete_data_repository_association)
         """
 
     def delete_file_cache(
         self, *, FileCacheId: str, ClientRequestToken: str = ...
-    ) -> DeleteFileCacheResponseTypeDef:
+    ) -> DeleteFileCacheResponseOutputTypeDef:
         """
         Deletes an Amazon File Cache resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.delete_file_cache)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#delete_file_cache)
         """
 
@@ -464,65 +464,65 @@
         self,
         *,
         FileSystemId: str,
         ClientRequestToken: str = ...,
         WindowsConfiguration: DeleteFileSystemWindowsConfigurationTypeDef = ...,
         LustreConfiguration: DeleteFileSystemLustreConfigurationTypeDef = ...,
         OpenZFSConfiguration: DeleteFileSystemOpenZFSConfigurationTypeDef = ...
-    ) -> DeleteFileSystemResponseTypeDef:
+    ) -> DeleteFileSystemResponseOutputTypeDef:
         """
         Deletes a file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.delete_file_system)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#delete_file_system)
         """
 
     def delete_snapshot(
         self, *, SnapshotId: str, ClientRequestToken: str = ...
-    ) -> DeleteSnapshotResponseTypeDef:
+    ) -> DeleteSnapshotResponseOutputTypeDef:
         """
         Deletes an Amazon FSx for OpenZFS snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.delete_snapshot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#delete_snapshot)
         """
 
     def delete_storage_virtual_machine(
         self, *, StorageVirtualMachineId: str, ClientRequestToken: str = ...
-    ) -> DeleteStorageVirtualMachineResponseTypeDef:
+    ) -> DeleteStorageVirtualMachineResponseOutputTypeDef:
         """
         Deletes an existing Amazon FSx for ONTAP storage virtual machine (SVM).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.delete_storage_virtual_machine)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#delete_storage_virtual_machine)
         """
 
     def delete_volume(
         self,
         *,
         VolumeId: str,
         ClientRequestToken: str = ...,
         OntapConfiguration: DeleteVolumeOntapConfigurationTypeDef = ...,
         OpenZFSConfiguration: DeleteVolumeOpenZFSConfigurationTypeDef = ...
-    ) -> DeleteVolumeResponseTypeDef:
+    ) -> DeleteVolumeResponseOutputTypeDef:
         """
         Deletes an Amazon FSx for NetApp ONTAP or Amazon FSx for OpenZFS volume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.delete_volume)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#delete_volume)
         """
 
     def describe_backups(
         self,
         *,
         BackupIds: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> DescribeBackupsResponseTypeDef:
+    ) -> DescribeBackupsResponseOutputTypeDef:
         """
         Returns the description of a specific Amazon FSx backup, if a `BackupIds` value
         is provided for that backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_backups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#describe_backups)
         """
@@ -530,15 +530,15 @@
     def describe_data_repository_associations(
         self,
         *,
         AssociationIds: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> DescribeDataRepositoryAssociationsResponseTypeDef:
+    ) -> DescribeDataRepositoryAssociationsResponseOutputTypeDef:
         """
         Returns the description of specific Amazon FSx for Lustre or Amazon File Cache
         data repository associations, if one or more `AssociationIds` values are
         provided in the request, or if filters are used in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_data_repository_associations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#describe_data_repository_associations)
@@ -547,27 +547,27 @@
     def describe_data_repository_tasks(
         self,
         *,
         TaskIds: Sequence[str] = ...,
         Filters: Sequence[DataRepositoryTaskFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> DescribeDataRepositoryTasksResponseTypeDef:
+    ) -> DescribeDataRepositoryTasksResponseOutputTypeDef:
         """
         Returns the description of specific Amazon FSx for Lustre or Amazon File Cache
         data repository tasks, if one or more `TaskIds` values are provided in the
         request, or if filters are used in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_data_repository_tasks)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#describe_data_repository_tasks)
         """
 
     def describe_file_caches(
         self, *, FileCacheIds: Sequence[str] = ..., MaxResults: int = ..., NextToken: str = ...
-    ) -> DescribeFileCachesResponseTypeDef:
+    ) -> DescribeFileCachesResponseOutputTypeDef:
         """
         Returns the description of a specific Amazon File Cache resource, if a
         `FileCacheIds` value is provided for that cache.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_file_caches)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#describe_file_caches)
         """
@@ -575,26 +575,26 @@
     def describe_file_system_aliases(
         self,
         *,
         FileSystemId: str,
         ClientRequestToken: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> DescribeFileSystemAliasesResponseTypeDef:
+    ) -> DescribeFileSystemAliasesResponseOutputTypeDef:
         """
         Returns the DNS aliases that are associated with the specified Amazon FSx for
         Windows File Server file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_file_system_aliases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#describe_file_system_aliases)
         """
 
     def describe_file_systems(
         self, *, FileSystemIds: Sequence[str] = ..., MaxResults: int = ..., NextToken: str = ...
-    ) -> DescribeFileSystemsResponseTypeDef:
+    ) -> DescribeFileSystemsResponseOutputTypeDef:
         """
         Returns the description of specific Amazon FSx file systems, if a
         `FileSystemIds` value is provided for that file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_file_systems)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#describe_file_systems)
         """
@@ -602,15 +602,15 @@
     def describe_snapshots(
         self,
         *,
         SnapshotIds: Sequence[str] = ...,
         Filters: Sequence[SnapshotFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> DescribeSnapshotsResponseTypeDef:
+    ) -> DescribeSnapshotsResponseOutputTypeDef:
         """
         Returns the description of specific Amazon FSx for OpenZFS snapshots, if a
         `SnapshotIds` value is provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_snapshots)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#describe_snapshots)
         """
@@ -618,15 +618,15 @@
     def describe_storage_virtual_machines(
         self,
         *,
         StorageVirtualMachineIds: Sequence[str] = ...,
         Filters: Sequence[StorageVirtualMachineFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> DescribeStorageVirtualMachinesResponseTypeDef:
+    ) -> DescribeStorageVirtualMachinesResponseOutputTypeDef:
         """
         Describes one or more Amazon FSx for NetApp ONTAP storage virtual machines
         (SVMs).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_storage_virtual_machines)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#describe_storage_virtual_machines)
         """
@@ -634,26 +634,26 @@
     def describe_volumes(
         self,
         *,
         VolumeIds: Sequence[str] = ...,
         Filters: Sequence[VolumeFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> DescribeVolumesResponseTypeDef:
+    ) -> DescribeVolumesResponseOutputTypeDef:
         """
         Describes one or more Amazon FSx for NetApp ONTAP or Amazon FSx for OpenZFS
         volumes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_volumes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#describe_volumes)
         """
 
     def disassociate_file_system_aliases(
         self, *, FileSystemId: str, Aliases: Sequence[str], ClientRequestToken: str = ...
-    ) -> DisassociateFileSystemAliasesResponseTypeDef:
+    ) -> DisassociateFileSystemAliasesResponseOutputTypeDef:
         """
         Use this action to disassociate, or remove, one or more Domain Name Service
         (DNS) aliases from an Amazon FSx for Windows File Server file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.disassociate_file_system_aliases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#disassociate_file_system_aliases)
         """
@@ -670,40 +670,40 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#generate_presigned_url)
         """
 
     def list_tags_for_resource(
         self, *, ResourceARN: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListTagsForResourceResponseTypeDef:
+    ) -> ListTagsForResourceResponseOutputTypeDef:
         """
         Lists tags for Amazon FSx resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#list_tags_for_resource)
         """
 
     def release_file_system_nfs_v3_locks(
         self, *, FileSystemId: str, ClientRequestToken: str = ...
-    ) -> ReleaseFileSystemNfsV3LocksResponseTypeDef:
+    ) -> ReleaseFileSystemNfsV3LocksResponseOutputTypeDef:
         """
         Releases the file system lock from an Amazon FSx for OpenZFS file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.release_file_system_nfs_v3_locks)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#release_file_system_nfs_v3_locks)
         """
 
     def restore_volume_from_snapshot(
         self,
         *,
         VolumeId: str,
         SnapshotId: str,
         ClientRequestToken: str = ...,
         Options: Sequence[RestoreOpenZFSVolumeOptionType] = ...
-    ) -> RestoreVolumeFromSnapshotResponseTypeDef:
+    ) -> RestoreVolumeFromSnapshotResponseOutputTypeDef:
         """
         Returns an Amazon FSx for OpenZFS volume to the state saved by the specified
         snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.restore_volume_from_snapshot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#restore_volume_from_snapshot)
         """
@@ -727,30 +727,30 @@
     def update_data_repository_association(
         self,
         *,
         AssociationId: str,
         ClientRequestToken: str = ...,
         ImportedFileChunkSize: int = ...,
         S3: S3DataRepositoryConfigurationTypeDef = ...
-    ) -> UpdateDataRepositoryAssociationResponseTypeDef:
+    ) -> UpdateDataRepositoryAssociationResponseOutputTypeDef:
         """
         Updates the configuration of an existing data repository association on an
         Amazon FSx for Lustre file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.update_data_repository_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#update_data_repository_association)
         """
 
     def update_file_cache(
         self,
         *,
         FileCacheId: str,
         ClientRequestToken: str = ...,
         LustreConfiguration: UpdateFileCacheLustreConfigurationTypeDef = ...
-    ) -> UpdateFileCacheResponseTypeDef:
+    ) -> UpdateFileCacheResponseOutputTypeDef:
         """
         Updates the configuration of an existing Amazon File Cache resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.update_file_cache)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#update_file_cache)
         """
 
@@ -760,41 +760,41 @@
         FileSystemId: str,
         ClientRequestToken: str = ...,
         StorageCapacity: int = ...,
         WindowsConfiguration: UpdateFileSystemWindowsConfigurationTypeDef = ...,
         LustreConfiguration: UpdateFileSystemLustreConfigurationTypeDef = ...,
         OntapConfiguration: UpdateFileSystemOntapConfigurationTypeDef = ...,
         OpenZFSConfiguration: UpdateFileSystemOpenZFSConfigurationTypeDef = ...
-    ) -> UpdateFileSystemResponseTypeDef:
+    ) -> UpdateFileSystemResponseOutputTypeDef:
         """
         Use this operation to update the configuration of an existing Amazon FSx file
         system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.update_file_system)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#update_file_system)
         """
 
     def update_snapshot(
         self, *, Name: str, SnapshotId: str, ClientRequestToken: str = ...
-    ) -> UpdateSnapshotResponseTypeDef:
+    ) -> UpdateSnapshotResponseOutputTypeDef:
         """
         Updates the name of an Amazon FSx for OpenZFS snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.update_snapshot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#update_snapshot)
         """
 
     def update_storage_virtual_machine(
         self,
         *,
         StorageVirtualMachineId: str,
         ActiveDirectoryConfiguration: UpdateSvmActiveDirectoryConfigurationTypeDef = ...,
         ClientRequestToken: str = ...,
         SvmAdminPassword: str = ...
-    ) -> UpdateStorageVirtualMachineResponseTypeDef:
+    ) -> UpdateStorageVirtualMachineResponseOutputTypeDef:
         """
         Updates an FSx for ONTAP storage virtual machine (SVM).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.update_storage_virtual_machine)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#update_storage_virtual_machine)
         """
 
@@ -802,15 +802,15 @@
         self,
         *,
         VolumeId: str,
         ClientRequestToken: str = ...,
         OntapConfiguration: UpdateOntapVolumeConfigurationTypeDef = ...,
         Name: str = ...,
         OpenZFSConfiguration: UpdateOpenZFSVolumeConfigurationTypeDef = ...
-    ) -> UpdateVolumeResponseTypeDef:
+    ) -> UpdateVolumeResponseOutputTypeDef:
         """
         Updates the configuration of an Amazon FSx for NetApp ONTAP or Amazon FSx for
         OpenZFS volume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.update_volume)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#update_volume)
         """
```

### Comparing `mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/client.pyi` & `mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -30,82 +30,82 @@
     DescribeBackupsPaginator,
     DescribeFileSystemsPaginator,
     DescribeStorageVirtualMachinesPaginator,
     DescribeVolumesPaginator,
     ListTagsForResourcePaginator,
 )
 from .type_defs import (
-    AssociateFileSystemAliasesResponseTypeDef,
-    CancelDataRepositoryTaskResponseTypeDef,
+    AssociateFileSystemAliasesResponseOutputTypeDef,
+    CancelDataRepositoryTaskResponseOutputTypeDef,
     CompletionReportTypeDef,
-    CopyBackupResponseTypeDef,
-    CreateBackupResponseTypeDef,
-    CreateDataRepositoryAssociationResponseTypeDef,
-    CreateDataRepositoryTaskResponseTypeDef,
+    CopyBackupResponseOutputTypeDef,
+    CreateBackupResponseOutputTypeDef,
+    CreateDataRepositoryAssociationResponseOutputTypeDef,
+    CreateDataRepositoryTaskResponseOutputTypeDef,
     CreateFileCacheLustreConfigurationTypeDef,
-    CreateFileCacheResponseTypeDef,
-    CreateFileSystemFromBackupResponseTypeDef,
+    CreateFileCacheResponseOutputTypeDef,
+    CreateFileSystemFromBackupResponseOutputTypeDef,
     CreateFileSystemLustreConfigurationTypeDef,
     CreateFileSystemOntapConfigurationTypeDef,
     CreateFileSystemOpenZFSConfigurationTypeDef,
-    CreateFileSystemResponseTypeDef,
+    CreateFileSystemResponseOutputTypeDef,
     CreateFileSystemWindowsConfigurationTypeDef,
     CreateOntapVolumeConfigurationTypeDef,
     CreateOpenZFSVolumeConfigurationTypeDef,
-    CreateSnapshotResponseTypeDef,
-    CreateStorageVirtualMachineResponseTypeDef,
+    CreateSnapshotResponseOutputTypeDef,
+    CreateStorageVirtualMachineResponseOutputTypeDef,
     CreateSvmActiveDirectoryConfigurationTypeDef,
-    CreateVolumeFromBackupResponseTypeDef,
-    CreateVolumeResponseTypeDef,
+    CreateVolumeFromBackupResponseOutputTypeDef,
+    CreateVolumeResponseOutputTypeDef,
     DataRepositoryTaskFilterTypeDef,
-    DeleteBackupResponseTypeDef,
-    DeleteDataRepositoryAssociationResponseTypeDef,
-    DeleteFileCacheResponseTypeDef,
+    DeleteBackupResponseOutputTypeDef,
+    DeleteDataRepositoryAssociationResponseOutputTypeDef,
+    DeleteFileCacheResponseOutputTypeDef,
     DeleteFileSystemLustreConfigurationTypeDef,
     DeleteFileSystemOpenZFSConfigurationTypeDef,
-    DeleteFileSystemResponseTypeDef,
+    DeleteFileSystemResponseOutputTypeDef,
     DeleteFileSystemWindowsConfigurationTypeDef,
-    DeleteSnapshotResponseTypeDef,
-    DeleteStorageVirtualMachineResponseTypeDef,
+    DeleteSnapshotResponseOutputTypeDef,
+    DeleteStorageVirtualMachineResponseOutputTypeDef,
     DeleteVolumeOntapConfigurationTypeDef,
     DeleteVolumeOpenZFSConfigurationTypeDef,
-    DeleteVolumeResponseTypeDef,
-    DescribeBackupsResponseTypeDef,
-    DescribeDataRepositoryAssociationsResponseTypeDef,
-    DescribeDataRepositoryTasksResponseTypeDef,
-    DescribeFileCachesResponseTypeDef,
-    DescribeFileSystemAliasesResponseTypeDef,
-    DescribeFileSystemsResponseTypeDef,
-    DescribeSnapshotsResponseTypeDef,
-    DescribeStorageVirtualMachinesResponseTypeDef,
-    DescribeVolumesResponseTypeDef,
-    DisassociateFileSystemAliasesResponseTypeDef,
+    DeleteVolumeResponseOutputTypeDef,
+    DescribeBackupsResponseOutputTypeDef,
+    DescribeDataRepositoryAssociationsResponseOutputTypeDef,
+    DescribeDataRepositoryTasksResponseOutputTypeDef,
+    DescribeFileCachesResponseOutputTypeDef,
+    DescribeFileSystemAliasesResponseOutputTypeDef,
+    DescribeFileSystemsResponseOutputTypeDef,
+    DescribeSnapshotsResponseOutputTypeDef,
+    DescribeStorageVirtualMachinesResponseOutputTypeDef,
+    DescribeVolumesResponseOutputTypeDef,
+    DisassociateFileSystemAliasesResponseOutputTypeDef,
     FileCacheDataRepositoryAssociationTypeDef,
     FilterTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ReleaseFileSystemNfsV3LocksResponseTypeDef,
-    RestoreVolumeFromSnapshotResponseTypeDef,
+    ListTagsForResourceResponseOutputTypeDef,
+    ReleaseFileSystemNfsV3LocksResponseOutputTypeDef,
+    RestoreVolumeFromSnapshotResponseOutputTypeDef,
     S3DataRepositoryConfigurationTypeDef,
     SnapshotFilterTypeDef,
     StorageVirtualMachineFilterTypeDef,
     TagTypeDef,
-    UpdateDataRepositoryAssociationResponseTypeDef,
+    UpdateDataRepositoryAssociationResponseOutputTypeDef,
     UpdateFileCacheLustreConfigurationTypeDef,
-    UpdateFileCacheResponseTypeDef,
+    UpdateFileCacheResponseOutputTypeDef,
     UpdateFileSystemLustreConfigurationTypeDef,
     UpdateFileSystemOntapConfigurationTypeDef,
     UpdateFileSystemOpenZFSConfigurationTypeDef,
-    UpdateFileSystemResponseTypeDef,
+    UpdateFileSystemResponseOutputTypeDef,
     UpdateFileSystemWindowsConfigurationTypeDef,
     UpdateOntapVolumeConfigurationTypeDef,
     UpdateOpenZFSVolumeConfigurationTypeDef,
-    UpdateSnapshotResponseTypeDef,
-    UpdateStorageVirtualMachineResponseTypeDef,
+    UpdateSnapshotResponseOutputTypeDef,
+    UpdateStorageVirtualMachineResponseOutputTypeDef,
     UpdateSvmActiveDirectoryConfigurationTypeDef,
-    UpdateVolumeResponseTypeDef,
+    UpdateVolumeResponseOutputTypeDef,
     VolumeFilterTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -171,15 +171,15 @@
         FSxClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#exceptions)
         """
     def associate_file_system_aliases(
         self, *, FileSystemId: str, Aliases: Sequence[str], ClientRequestToken: str = ...
-    ) -> AssociateFileSystemAliasesResponseTypeDef:
+    ) -> AssociateFileSystemAliasesResponseOutputTypeDef:
         """
         Use this action to associate one or more Domain Name Server (DNS) aliases with
         an existing Amazon FSx for Windows File Server file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.associate_file_system_aliases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#associate_file_system_aliases)
         """
@@ -188,15 +188,15 @@
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#can_paginate)
         """
     def cancel_data_repository_task(
         self, *, TaskId: str
-    ) -> CancelDataRepositoryTaskResponseTypeDef:
+    ) -> CancelDataRepositoryTaskResponseOutputTypeDef:
         """
         Cancels an existing Amazon FSx for Lustre data repository task if that task is
         in either the `PENDING` or `EXECUTING` state.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.cancel_data_repository_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#cancel_data_repository_task)
         """
@@ -212,15 +212,15 @@
         *,
         SourceBackupId: str,
         ClientRequestToken: str = ...,
         SourceRegion: str = ...,
         KmsKeyId: str = ...,
         CopyTags: bool = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CopyBackupResponseTypeDef:
+    ) -> CopyBackupResponseOutputTypeDef:
         """
         Copies an existing backup within the same Amazon Web Services account to another
         Amazon Web Services Region (cross-Region copy) or within the same Amazon Web
         Services Region (in-Region copy).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.copy_backup)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#copy_backup)
@@ -228,15 +228,15 @@
     def create_backup(
         self,
         *,
         FileSystemId: str = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         VolumeId: str = ...
-    ) -> CreateBackupResponseTypeDef:
+    ) -> CreateBackupResponseOutputTypeDef:
         """
         Creates a backup of an existing Amazon FSx for Windows File Server file system,
         Amazon FSx for Lustre file system, Amazon FSx for NetApp ONTAP volume, or Amazon
         FSx for OpenZFS file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_backup)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_backup)
@@ -248,15 +248,15 @@
         DataRepositoryPath: str,
         FileSystemPath: str = ...,
         BatchImportMetaDataOnCreate: bool = ...,
         ImportedFileChunkSize: int = ...,
         S3: S3DataRepositoryConfigurationTypeDef = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateDataRepositoryAssociationResponseTypeDef:
+    ) -> CreateDataRepositoryAssociationResponseOutputTypeDef:
         """
         Creates an Amazon FSx for Lustre data repository association (DRA).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_data_repository_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_data_repository_association)
         """
     def create_data_repository_task(
@@ -265,15 +265,15 @@
         Type: DataRepositoryTaskTypeType,
         FileSystemId: str,
         Report: CompletionReportTypeDef,
         Paths: Sequence[str] = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         CapacityToRelease: int = ...
-    ) -> CreateDataRepositoryTaskResponseTypeDef:
+    ) -> CreateDataRepositoryTaskResponseOutputTypeDef:
         """
         Creates an Amazon FSx for Lustre data repository task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_data_repository_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_data_repository_task)
         """
     def create_file_cache(
@@ -286,15 +286,15 @@
         ClientRequestToken: str = ...,
         SecurityGroupIds: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         CopyTagsToDataRepositoryAssociations: bool = ...,
         KmsKeyId: str = ...,
         LustreConfiguration: CreateFileCacheLustreConfigurationTypeDef = ...,
         DataRepositoryAssociations: Sequence[FileCacheDataRepositoryAssociationTypeDef] = ...
-    ) -> CreateFileCacheResponseTypeDef:
+    ) -> CreateFileCacheResponseOutputTypeDef:
         """
         Creates a new Amazon File Cache resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_file_cache)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_file_cache)
         """
     def create_file_system(
@@ -309,15 +309,15 @@
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
         WindowsConfiguration: CreateFileSystemWindowsConfigurationTypeDef = ...,
         LustreConfiguration: CreateFileSystemLustreConfigurationTypeDef = ...,
         OntapConfiguration: CreateFileSystemOntapConfigurationTypeDef = ...,
         FileSystemTypeVersion: str = ...,
         OpenZFSConfiguration: CreateFileSystemOpenZFSConfigurationTypeDef = ...
-    ) -> CreateFileSystemResponseTypeDef:
+    ) -> CreateFileSystemResponseOutputTypeDef:
         """
         Creates a new, empty Amazon FSx file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_file_system)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_file_system)
         """
     def create_file_system_from_backup(
@@ -331,30 +331,30 @@
         WindowsConfiguration: CreateFileSystemWindowsConfigurationTypeDef = ...,
         LustreConfiguration: CreateFileSystemLustreConfigurationTypeDef = ...,
         StorageType: StorageTypeType = ...,
         KmsKeyId: str = ...,
         FileSystemTypeVersion: str = ...,
         OpenZFSConfiguration: CreateFileSystemOpenZFSConfigurationTypeDef = ...,
         StorageCapacity: int = ...
-    ) -> CreateFileSystemFromBackupResponseTypeDef:
+    ) -> CreateFileSystemFromBackupResponseOutputTypeDef:
         """
         Creates a new Amazon FSx for Lustre, Amazon FSx for Windows File Server, or
         Amazon FSx for OpenZFS file system from an existing Amazon FSx backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_file_system_from_backup)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_file_system_from_backup)
         """
     def create_snapshot(
         self,
         *,
         Name: str,
         VolumeId: str,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateSnapshotResponseTypeDef:
+    ) -> CreateSnapshotResponseOutputTypeDef:
         """
         Creates a snapshot of an existing Amazon FSx for OpenZFS volume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_snapshot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_snapshot)
         """
     def create_storage_virtual_machine(
@@ -363,15 +363,15 @@
         FileSystemId: str,
         Name: str,
         ActiveDirectoryConfiguration: CreateSvmActiveDirectoryConfigurationTypeDef = ...,
         ClientRequestToken: str = ...,
         SvmAdminPassword: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         RootVolumeSecurityStyle: StorageVirtualMachineRootVolumeSecurityStyleType = ...
-    ) -> CreateStorageVirtualMachineResponseTypeDef:
+    ) -> CreateStorageVirtualMachineResponseOutputTypeDef:
         """
         Creates a storage virtual machine (SVM) for an Amazon FSx for ONTAP file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_storage_virtual_machine)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_storage_virtual_machine)
         """
     def create_volume(
@@ -379,138 +379,138 @@
         *,
         VolumeType: VolumeTypeType,
         Name: str,
         ClientRequestToken: str = ...,
         OntapConfiguration: CreateOntapVolumeConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         OpenZFSConfiguration: CreateOpenZFSVolumeConfigurationTypeDef = ...
-    ) -> CreateVolumeResponseTypeDef:
+    ) -> CreateVolumeResponseOutputTypeDef:
         """
         Creates an FSx for ONTAP or Amazon FSx for OpenZFS storage volume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_volume)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_volume)
         """
     def create_volume_from_backup(
         self,
         *,
         BackupId: str,
         Name: str,
         ClientRequestToken: str = ...,
         OntapConfiguration: CreateOntapVolumeConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateVolumeFromBackupResponseTypeDef:
+    ) -> CreateVolumeFromBackupResponseOutputTypeDef:
         """
         Creates a new Amazon FSx for NetApp ONTAP volume from an existing Amazon FSx
         volume backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_volume_from_backup)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#create_volume_from_backup)
         """
     def delete_backup(
         self, *, BackupId: str, ClientRequestToken: str = ...
-    ) -> DeleteBackupResponseTypeDef:
+    ) -> DeleteBackupResponseOutputTypeDef:
         """
         Deletes an Amazon FSx backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.delete_backup)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#delete_backup)
         """
     def delete_data_repository_association(
         self,
         *,
         AssociationId: str,
         ClientRequestToken: str = ...,
         DeleteDataInFileSystem: bool = ...
-    ) -> DeleteDataRepositoryAssociationResponseTypeDef:
+    ) -> DeleteDataRepositoryAssociationResponseOutputTypeDef:
         """
         Deletes a data repository association on an Amazon FSx for Lustre file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.delete_data_repository_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#delete_data_repository_association)
         """
     def delete_file_cache(
         self, *, FileCacheId: str, ClientRequestToken: str = ...
-    ) -> DeleteFileCacheResponseTypeDef:
+    ) -> DeleteFileCacheResponseOutputTypeDef:
         """
         Deletes an Amazon File Cache resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.delete_file_cache)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#delete_file_cache)
         """
     def delete_file_system(
         self,
         *,
         FileSystemId: str,
         ClientRequestToken: str = ...,
         WindowsConfiguration: DeleteFileSystemWindowsConfigurationTypeDef = ...,
         LustreConfiguration: DeleteFileSystemLustreConfigurationTypeDef = ...,
         OpenZFSConfiguration: DeleteFileSystemOpenZFSConfigurationTypeDef = ...
-    ) -> DeleteFileSystemResponseTypeDef:
+    ) -> DeleteFileSystemResponseOutputTypeDef:
         """
         Deletes a file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.delete_file_system)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#delete_file_system)
         """
     def delete_snapshot(
         self, *, SnapshotId: str, ClientRequestToken: str = ...
-    ) -> DeleteSnapshotResponseTypeDef:
+    ) -> DeleteSnapshotResponseOutputTypeDef:
         """
         Deletes an Amazon FSx for OpenZFS snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.delete_snapshot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#delete_snapshot)
         """
     def delete_storage_virtual_machine(
         self, *, StorageVirtualMachineId: str, ClientRequestToken: str = ...
-    ) -> DeleteStorageVirtualMachineResponseTypeDef:
+    ) -> DeleteStorageVirtualMachineResponseOutputTypeDef:
         """
         Deletes an existing Amazon FSx for ONTAP storage virtual machine (SVM).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.delete_storage_virtual_machine)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#delete_storage_virtual_machine)
         """
     def delete_volume(
         self,
         *,
         VolumeId: str,
         ClientRequestToken: str = ...,
         OntapConfiguration: DeleteVolumeOntapConfigurationTypeDef = ...,
         OpenZFSConfiguration: DeleteVolumeOpenZFSConfigurationTypeDef = ...
-    ) -> DeleteVolumeResponseTypeDef:
+    ) -> DeleteVolumeResponseOutputTypeDef:
         """
         Deletes an Amazon FSx for NetApp ONTAP or Amazon FSx for OpenZFS volume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.delete_volume)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#delete_volume)
         """
     def describe_backups(
         self,
         *,
         BackupIds: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> DescribeBackupsResponseTypeDef:
+    ) -> DescribeBackupsResponseOutputTypeDef:
         """
         Returns the description of a specific Amazon FSx backup, if a `BackupIds` value
         is provided for that backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_backups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#describe_backups)
         """
     def describe_data_repository_associations(
         self,
         *,
         AssociationIds: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> DescribeDataRepositoryAssociationsResponseTypeDef:
+    ) -> DescribeDataRepositoryAssociationsResponseOutputTypeDef:
         """
         Returns the description of specific Amazon FSx for Lustre or Amazon File Cache
         data repository associations, if one or more `AssociationIds` values are
         provided in the request, or if filters are used in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_data_repository_associations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#describe_data_repository_associations)
@@ -518,106 +518,106 @@
     def describe_data_repository_tasks(
         self,
         *,
         TaskIds: Sequence[str] = ...,
         Filters: Sequence[DataRepositoryTaskFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> DescribeDataRepositoryTasksResponseTypeDef:
+    ) -> DescribeDataRepositoryTasksResponseOutputTypeDef:
         """
         Returns the description of specific Amazon FSx for Lustre or Amazon File Cache
         data repository tasks, if one or more `TaskIds` values are provided in the
         request, or if filters are used in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_data_repository_tasks)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#describe_data_repository_tasks)
         """
     def describe_file_caches(
         self, *, FileCacheIds: Sequence[str] = ..., MaxResults: int = ..., NextToken: str = ...
-    ) -> DescribeFileCachesResponseTypeDef:
+    ) -> DescribeFileCachesResponseOutputTypeDef:
         """
         Returns the description of a specific Amazon File Cache resource, if a
         `FileCacheIds` value is provided for that cache.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_file_caches)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#describe_file_caches)
         """
     def describe_file_system_aliases(
         self,
         *,
         FileSystemId: str,
         ClientRequestToken: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> DescribeFileSystemAliasesResponseTypeDef:
+    ) -> DescribeFileSystemAliasesResponseOutputTypeDef:
         """
         Returns the DNS aliases that are associated with the specified Amazon FSx for
         Windows File Server file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_file_system_aliases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#describe_file_system_aliases)
         """
     def describe_file_systems(
         self, *, FileSystemIds: Sequence[str] = ..., MaxResults: int = ..., NextToken: str = ...
-    ) -> DescribeFileSystemsResponseTypeDef:
+    ) -> DescribeFileSystemsResponseOutputTypeDef:
         """
         Returns the description of specific Amazon FSx file systems, if a
         `FileSystemIds` value is provided for that file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_file_systems)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#describe_file_systems)
         """
     def describe_snapshots(
         self,
         *,
         SnapshotIds: Sequence[str] = ...,
         Filters: Sequence[SnapshotFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> DescribeSnapshotsResponseTypeDef:
+    ) -> DescribeSnapshotsResponseOutputTypeDef:
         """
         Returns the description of specific Amazon FSx for OpenZFS snapshots, if a
         `SnapshotIds` value is provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_snapshots)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#describe_snapshots)
         """
     def describe_storage_virtual_machines(
         self,
         *,
         StorageVirtualMachineIds: Sequence[str] = ...,
         Filters: Sequence[StorageVirtualMachineFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> DescribeStorageVirtualMachinesResponseTypeDef:
+    ) -> DescribeStorageVirtualMachinesResponseOutputTypeDef:
         """
         Describes one or more Amazon FSx for NetApp ONTAP storage virtual machines
         (SVMs).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_storage_virtual_machines)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#describe_storage_virtual_machines)
         """
     def describe_volumes(
         self,
         *,
         VolumeIds: Sequence[str] = ...,
         Filters: Sequence[VolumeFilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
-    ) -> DescribeVolumesResponseTypeDef:
+    ) -> DescribeVolumesResponseOutputTypeDef:
         """
         Describes one or more Amazon FSx for NetApp ONTAP or Amazon FSx for OpenZFS
         volumes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_volumes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#describe_volumes)
         """
     def disassociate_file_system_aliases(
         self, *, FileSystemId: str, Aliases: Sequence[str], ClientRequestToken: str = ...
-    ) -> DisassociateFileSystemAliasesResponseTypeDef:
+    ) -> DisassociateFileSystemAliasesResponseOutputTypeDef:
         """
         Use this action to disassociate, or remove, one or more Domain Name Service
         (DNS) aliases from an Amazon FSx for Windows File Server file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.disassociate_file_system_aliases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#disassociate_file_system_aliases)
         """
@@ -632,38 +632,38 @@
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#generate_presigned_url)
         """
     def list_tags_for_resource(
         self, *, ResourceARN: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListTagsForResourceResponseTypeDef:
+    ) -> ListTagsForResourceResponseOutputTypeDef:
         """
         Lists tags for Amazon FSx resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#list_tags_for_resource)
         """
     def release_file_system_nfs_v3_locks(
         self, *, FileSystemId: str, ClientRequestToken: str = ...
-    ) -> ReleaseFileSystemNfsV3LocksResponseTypeDef:
+    ) -> ReleaseFileSystemNfsV3LocksResponseOutputTypeDef:
         """
         Releases the file system lock from an Amazon FSx for OpenZFS file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.release_file_system_nfs_v3_locks)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#release_file_system_nfs_v3_locks)
         """
     def restore_volume_from_snapshot(
         self,
         *,
         VolumeId: str,
         SnapshotId: str,
         ClientRequestToken: str = ...,
         Options: Sequence[RestoreOpenZFSVolumeOptionType] = ...
-    ) -> RestoreVolumeFromSnapshotResponseTypeDef:
+    ) -> RestoreVolumeFromSnapshotResponseOutputTypeDef:
         """
         Returns an Amazon FSx for OpenZFS volume to the state saved by the specified
         snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.restore_volume_from_snapshot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#restore_volume_from_snapshot)
         """
@@ -684,29 +684,29 @@
     def update_data_repository_association(
         self,
         *,
         AssociationId: str,
         ClientRequestToken: str = ...,
         ImportedFileChunkSize: int = ...,
         S3: S3DataRepositoryConfigurationTypeDef = ...
-    ) -> UpdateDataRepositoryAssociationResponseTypeDef:
+    ) -> UpdateDataRepositoryAssociationResponseOutputTypeDef:
         """
         Updates the configuration of an existing data repository association on an
         Amazon FSx for Lustre file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.update_data_repository_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#update_data_repository_association)
         """
     def update_file_cache(
         self,
         *,
         FileCacheId: str,
         ClientRequestToken: str = ...,
         LustreConfiguration: UpdateFileCacheLustreConfigurationTypeDef = ...
-    ) -> UpdateFileCacheResponseTypeDef:
+    ) -> UpdateFileCacheResponseOutputTypeDef:
         """
         Updates the configuration of an existing Amazon File Cache resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.update_file_cache)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#update_file_cache)
         """
     def update_file_system(
@@ -715,54 +715,54 @@
         FileSystemId: str,
         ClientRequestToken: str = ...,
         StorageCapacity: int = ...,
         WindowsConfiguration: UpdateFileSystemWindowsConfigurationTypeDef = ...,
         LustreConfiguration: UpdateFileSystemLustreConfigurationTypeDef = ...,
         OntapConfiguration: UpdateFileSystemOntapConfigurationTypeDef = ...,
         OpenZFSConfiguration: UpdateFileSystemOpenZFSConfigurationTypeDef = ...
-    ) -> UpdateFileSystemResponseTypeDef:
+    ) -> UpdateFileSystemResponseOutputTypeDef:
         """
         Use this operation to update the configuration of an existing Amazon FSx file
         system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.update_file_system)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#update_file_system)
         """
     def update_snapshot(
         self, *, Name: str, SnapshotId: str, ClientRequestToken: str = ...
-    ) -> UpdateSnapshotResponseTypeDef:
+    ) -> UpdateSnapshotResponseOutputTypeDef:
         """
         Updates the name of an Amazon FSx for OpenZFS snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.update_snapshot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#update_snapshot)
         """
     def update_storage_virtual_machine(
         self,
         *,
         StorageVirtualMachineId: str,
         ActiveDirectoryConfiguration: UpdateSvmActiveDirectoryConfigurationTypeDef = ...,
         ClientRequestToken: str = ...,
         SvmAdminPassword: str = ...
-    ) -> UpdateStorageVirtualMachineResponseTypeDef:
+    ) -> UpdateStorageVirtualMachineResponseOutputTypeDef:
         """
         Updates an FSx for ONTAP storage virtual machine (SVM).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.update_storage_virtual_machine)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#update_storage_virtual_machine)
         """
     def update_volume(
         self,
         *,
         VolumeId: str,
         ClientRequestToken: str = ...,
         OntapConfiguration: UpdateOntapVolumeConfigurationTypeDef = ...,
         Name: str = ...,
         OpenZFSConfiguration: UpdateOpenZFSVolumeConfigurationTypeDef = ...
-    ) -> UpdateVolumeResponseTypeDef:
+    ) -> UpdateVolumeResponseOutputTypeDef:
         """
         Updates the configuration of an Amazon FSx for NetApp ONTAP or Amazon FSx for
         OpenZFS volume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.update_volume)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/client/#update_volume)
         """
```

### Comparing `mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/literals.py` & `mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/literals.pyi` & `mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/paginator.py` & `mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,20 +28,20 @@
     ```
 """
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
-    DescribeBackupsResponseTypeDef,
-    DescribeFileSystemsResponseTypeDef,
-    DescribeStorageVirtualMachinesResponseTypeDef,
-    DescribeVolumesResponseTypeDef,
+    DescribeBackupsResponseOutputTypeDef,
+    DescribeFileSystemsResponseOutputTypeDef,
+    DescribeStorageVirtualMachinesResponseOutputTypeDef,
+    DescribeVolumesResponseOutputTypeDef,
     FilterTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    ListTagsForResourceResponseOutputTypeDef,
     PaginatorConfigTypeDef,
     StorageVirtualMachineFilterTypeDef,
     VolumeFilterTypeDef,
 )
 
 __all__ = (
     "DescribeBackupsPaginator",
@@ -70,15 +70,15 @@
 
     def paginate(
         self,
         *,
         BackupIds: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeBackupsResponseTypeDef]:
+    ) -> _PageIterator[DescribeBackupsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeBackups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/paginators/#describebackupspaginator)
         """
 
 
 class DescribeFileSystemsPaginator(Paginator):
@@ -88,15 +88,15 @@
     """
 
     def paginate(
         self,
         *,
         FileSystemIds: Sequence[str] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeFileSystemsResponseTypeDef]:
+    ) -> _PageIterator[DescribeFileSystemsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeFileSystems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/paginators/#describefilesystemspaginator)
         """
 
 
 class DescribeStorageVirtualMachinesPaginator(Paginator):
@@ -107,15 +107,15 @@
 
     def paginate(
         self,
         *,
         StorageVirtualMachineIds: Sequence[str] = ...,
         Filters: Sequence[StorageVirtualMachineFilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeStorageVirtualMachinesResponseTypeDef]:
+    ) -> _PageIterator[DescribeStorageVirtualMachinesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeStorageVirtualMachines.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/paginators/#describestoragevirtualmachinespaginator)
         """
 
 
 class DescribeVolumesPaginator(Paginator):
@@ -126,27 +126,27 @@
 
     def paginate(
         self,
         *,
         VolumeIds: Sequence[str] = ...,
         Filters: Sequence[VolumeFilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeVolumesResponseTypeDef]:
+    ) -> _PageIterator[DescribeVolumesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeVolumes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/paginators/#describevolumespaginator)
         """
 
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
         self, *, ResourceARN: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
+    ) -> _PageIterator[ListTagsForResourceResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/paginator.pyi` & `mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -28,20 +28,20 @@
     ```
 """
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
-    DescribeBackupsResponseTypeDef,
-    DescribeFileSystemsResponseTypeDef,
-    DescribeStorageVirtualMachinesResponseTypeDef,
-    DescribeVolumesResponseTypeDef,
+    DescribeBackupsResponseOutputTypeDef,
+    DescribeFileSystemsResponseOutputTypeDef,
+    DescribeStorageVirtualMachinesResponseOutputTypeDef,
+    DescribeVolumesResponseOutputTypeDef,
     FilterTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    ListTagsForResourceResponseOutputTypeDef,
     PaginatorConfigTypeDef,
     StorageVirtualMachineFilterTypeDef,
     VolumeFilterTypeDef,
 )
 
 __all__ = (
     "DescribeBackupsPaginator",
@@ -67,15 +67,15 @@
 
     def paginate(
         self,
         *,
         BackupIds: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeBackupsResponseTypeDef]:
+    ) -> _PageIterator[DescribeBackupsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeBackups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/paginators/#describebackupspaginator)
         """
 
 class DescribeFileSystemsPaginator(Paginator):
     """
@@ -84,15 +84,15 @@
     """
 
     def paginate(
         self,
         *,
         FileSystemIds: Sequence[str] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeFileSystemsResponseTypeDef]:
+    ) -> _PageIterator[DescribeFileSystemsResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeFileSystems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/paginators/#describefilesystemspaginator)
         """
 
 class DescribeStorageVirtualMachinesPaginator(Paginator):
     """
@@ -102,15 +102,15 @@
 
     def paginate(
         self,
         *,
         StorageVirtualMachineIds: Sequence[str] = ...,
         Filters: Sequence[StorageVirtualMachineFilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeStorageVirtualMachinesResponseTypeDef]:
+    ) -> _PageIterator[DescribeStorageVirtualMachinesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeStorageVirtualMachines.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/paginators/#describestoragevirtualmachinespaginator)
         """
 
 class DescribeVolumesPaginator(Paginator):
     """
@@ -120,26 +120,26 @@
 
     def paginate(
         self,
         *,
         VolumeIds: Sequence[str] = ...,
         Filters: Sequence[VolumeFilterTypeDef] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[DescribeVolumesResponseTypeDef]:
+    ) -> _PageIterator[DescribeVolumesResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeVolumes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/paginators/#describevolumespaginator)
         """
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
         self, *, ResourceARN: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
+    ) -> _PageIterator[ListTagsForResourceResponseOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/type_defs.py` & `mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for fsx service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_fsx.type_defs import ActiveDirectoryBackupAttributesTypeDef
+    from mypy_boto3_fsx.type_defs import ActiveDirectoryBackupAttributesOutputTypeDef
 
-    data: ActiveDirectoryBackupAttributesTypeDef = {...}
+    data: ActiveDirectoryBackupAttributesOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Sequence
 
 from .literals import (
@@ -73,215 +73,230 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "ActiveDirectoryBackupAttributesTypeDef",
-    "AdministrativeActionFailureDetailsTypeDef",
-    "AliasTypeDef",
+    "ActiveDirectoryBackupAttributesOutputTypeDef",
+    "AdministrativeActionFailureDetailsOutputTypeDef",
+    "AliasOutputTypeDef",
     "AssociateFileSystemAliasesRequestRequestTypeDef",
+    "AutoExportPolicyOutputTypeDef",
     "AutoExportPolicyTypeDef",
+    "AutoImportPolicyOutputTypeDef",
     "AutoImportPolicyTypeDef",
+    "AutocommitPeriodOutputTypeDef",
     "AutocommitPeriodTypeDef",
-    "BackupFailureDetailsTypeDef",
-    "TagTypeDef",
+    "BackupFailureDetailsOutputTypeDef",
+    "TagOutputTypeDef",
     "CancelDataRepositoryTaskRequestRequestTypeDef",
-    "CancelDataRepositoryTaskResponseTypeDef",
+    "CancelDataRepositoryTaskResponseOutputTypeDef",
+    "CompletionReportOutputTypeDef",
     "CompletionReportTypeDef",
+    "TagTypeDef",
     "FileCacheLustreMetadataConfigurationTypeDef",
-    "CreateFileSystemFromBackupResponseTypeDef",
+    "CreateFileSystemFromBackupResponseOutputTypeDef",
     "LustreLogCreateConfigurationTypeDef",
     "LustreRootSquashConfigurationTypeDef",
     "DiskIopsConfigurationTypeDef",
-    "CreateFileSystemResponseTypeDef",
+    "CreateFileSystemResponseOutputTypeDef",
     "SelfManagedActiveDirectoryConfigurationTypeDef",
     "WindowsAuditLogCreateConfigurationTypeDef",
     "TieringPolicyTypeDef",
     "CreateOpenZFSOriginSnapshotConfigurationTypeDef",
     "OpenZFSUserOrGroupQuotaTypeDef",
-    "DataRepositoryFailureDetailsTypeDef",
-    "DataRepositoryTaskFailureDetailsTypeDef",
+    "DataRepositoryFailureDetailsOutputTypeDef",
+    "DataRepositoryTaskFailureDetailsOutputTypeDef",
     "DataRepositoryTaskFilterTypeDef",
-    "DataRepositoryTaskStatusTypeDef",
+    "DataRepositoryTaskStatusOutputTypeDef",
     "DeleteBackupRequestRequestTypeDef",
-    "DeleteBackupResponseTypeDef",
+    "DeleteBackupResponseOutputTypeDef",
     "DeleteDataRepositoryAssociationRequestRequestTypeDef",
-    "DeleteDataRepositoryAssociationResponseTypeDef",
+    "DeleteDataRepositoryAssociationResponseOutputTypeDef",
     "DeleteFileCacheRequestRequestTypeDef",
-    "DeleteFileCacheResponseTypeDef",
+    "DeleteFileCacheResponseOutputTypeDef",
     "DeleteSnapshotRequestRequestTypeDef",
-    "DeleteSnapshotResponseTypeDef",
+    "DeleteSnapshotResponseOutputTypeDef",
     "DeleteStorageVirtualMachineRequestRequestTypeDef",
-    "DeleteStorageVirtualMachineResponseTypeDef",
+    "DeleteStorageVirtualMachineResponseOutputTypeDef",
     "DeleteVolumeOpenZFSConfigurationTypeDef",
     "FilterTypeDef",
     "DescribeFileCachesRequestRequestTypeDef",
     "DescribeFileSystemAliasesRequestRequestTypeDef",
     "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
     "DescribeFileSystemsRequestRequestTypeDef",
-    "DescribeFileSystemsResponseTypeDef",
+    "DescribeFileSystemsResponseOutputTypeDef",
     "SnapshotFilterTypeDef",
     "StorageVirtualMachineFilterTypeDef",
     "VolumeFilterTypeDef",
     "DisassociateFileSystemAliasesRequestRequestTypeDef",
-    "FileCacheFailureDetailsTypeDef",
+    "DiskIopsConfigurationOutputTypeDef",
+    "FileCacheFailureDetailsOutputTypeDef",
     "FileCacheNFSConfigurationTypeDef",
-    "LustreLogConfigurationTypeDef",
-    "FileSystemEndpointTypeDef",
-    "FileSystemFailureDetailsTypeDef",
-    "LifecycleTransitionReasonTypeDef",
+    "FileCacheLustreMetadataConfigurationOutputTypeDef",
+    "LustreLogConfigurationOutputTypeDef",
+    "FileSystemEndpointOutputTypeDef",
+    "FileSystemFailureDetailsOutputTypeDef",
+    "LifecycleTransitionReasonOutputTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "LustreRootSquashConfigurationOutputTypeDef",
+    "TieringPolicyOutputTypeDef",
+    "OpenZFSClientConfigurationOutputTypeDef",
     "OpenZFSClientConfigurationTypeDef",
-    "OpenZFSOriginSnapshotConfigurationTypeDef",
+    "OpenZFSOriginSnapshotConfigurationOutputTypeDef",
+    "OpenZFSUserOrGroupQuotaOutputTypeDef",
     "PaginatorConfigTypeDef",
     "ReleaseFileSystemNfsV3LocksRequestRequestTypeDef",
-    "ReleaseFileSystemNfsV3LocksResponseTypeDef",
+    "ReleaseFileSystemNfsV3LocksResponseOutputTypeDef",
     "ResponseMetadataTypeDef",
     "RestoreVolumeFromSnapshotRequestRequestTypeDef",
-    "RestoreVolumeFromSnapshotResponseTypeDef",
+    "RestoreVolumeFromSnapshotResponseOutputTypeDef",
+    "RetentionPeriodOutputTypeDef",
     "RetentionPeriodTypeDef",
-    "SelfManagedActiveDirectoryAttributesTypeDef",
+    "SelfManagedActiveDirectoryAttributesOutputTypeDef",
     "SelfManagedActiveDirectoryConfigurationUpdatesTypeDef",
-    "SvmEndpointTypeDef",
+    "SvmEndpointOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFileCacheLustreConfigurationTypeDef",
-    "UpdateFileSystemResponseTypeDef",
+    "UpdateFileSystemResponseOutputTypeDef",
     "UpdateSnapshotRequestRequestTypeDef",
-    "WindowsAuditLogConfigurationTypeDef",
-    "AssociateFileSystemAliasesResponseTypeDef",
-    "DescribeFileSystemAliasesResponseTypeDef",
-    "DisassociateFileSystemAliasesResponseTypeDef",
-    "NFSDataRepositoryConfigurationTypeDef",
+    "WindowsAuditLogConfigurationOutputTypeDef",
+    "AssociateFileSystemAliasesResponseOutputTypeDef",
+    "DescribeFileSystemAliasesResponseOutputTypeDef",
+    "DisassociateFileSystemAliasesResponseOutputTypeDef",
+    "NFSDataRepositoryConfigurationOutputTypeDef",
+    "S3DataRepositoryConfigurationOutputTypeDef",
     "S3DataRepositoryConfigurationTypeDef",
+    "DeleteFileSystemLustreResponseOutputTypeDef",
+    "DeleteFileSystemOpenZFSResponseOutputTypeDef",
+    "DeleteFileSystemWindowsResponseOutputTypeDef",
+    "DeleteVolumeOntapResponseOutputTypeDef",
+    "ListTagsForResourceResponseOutputTypeDef",
     "CopyBackupRequestRequestTypeDef",
     "CreateBackupRequestRequestTypeDef",
+    "CreateDataRepositoryTaskRequestRequestTypeDef",
     "CreateSnapshotRequestRequestTypeDef",
     "DeleteFileSystemLustreConfigurationTypeDef",
-    "DeleteFileSystemLustreResponseTypeDef",
     "DeleteFileSystemOpenZFSConfigurationTypeDef",
-    "DeleteFileSystemOpenZFSResponseTypeDef",
     "DeleteFileSystemWindowsConfigurationTypeDef",
-    "DeleteFileSystemWindowsResponseTypeDef",
     "DeleteVolumeOntapConfigurationTypeDef",
-    "DeleteVolumeOntapResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "CreateDataRepositoryTaskRequestRequestTypeDef",
     "CreateFileCacheLustreConfigurationTypeDef",
     "CreateFileSystemLustreConfigurationTypeDef",
     "UpdateFileSystemLustreConfigurationTypeDef",
     "CreateFileSystemOntapConfigurationTypeDef",
-    "OpenZFSFileSystemConfigurationTypeDef",
     "UpdateFileSystemOntapConfigurationTypeDef",
     "UpdateFileSystemOpenZFSConfigurationTypeDef",
     "CreateSvmActiveDirectoryConfigurationTypeDef",
     "CreateFileSystemWindowsConfigurationTypeDef",
-    "DataRepositoryConfigurationTypeDef",
+    "DataRepositoryConfigurationOutputTypeDef",
     "DescribeDataRepositoryTasksRequestRequestTypeDef",
-    "DataRepositoryTaskTypeDef",
+    "DataRepositoryTaskOutputTypeDef",
     "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
     "DescribeBackupsRequestRequestTypeDef",
     "DescribeDataRepositoryAssociationsRequestRequestTypeDef",
     "DescribeSnapshotsRequestRequestTypeDef",
     "DescribeStorageVirtualMachinesRequestDescribeStorageVirtualMachinesPaginateTypeDef",
     "DescribeStorageVirtualMachinesRequestRequestTypeDef",
     "DescribeVolumesRequestDescribeVolumesPaginateTypeDef",
     "DescribeVolumesRequestRequestTypeDef",
+    "OpenZFSFileSystemConfigurationOutputTypeDef",
     "FileCacheDataRepositoryAssociationTypeDef",
-    "FileCacheLustreConfigurationTypeDef",
-    "FileSystemEndpointsTypeDef",
-    "SnapshotTypeDef",
+    "FileCacheLustreConfigurationOutputTypeDef",
+    "FileSystemEndpointsOutputTypeDef",
+    "SnapshotOutputTypeDef",
+    "OpenZFSNfsExportOutputTypeDef",
     "OpenZFSNfsExportTypeDef",
+    "SnaplockRetentionPeriodOutputTypeDef",
     "SnaplockRetentionPeriodTypeDef",
-    "SvmActiveDirectoryConfigurationTypeDef",
+    "SvmActiveDirectoryConfigurationOutputTypeDef",
     "UpdateFileSystemWindowsConfigurationTypeDef",
     "UpdateSvmActiveDirectoryConfigurationTypeDef",
-    "SvmEndpointsTypeDef",
+    "SvmEndpointsOutputTypeDef",
     "UpdateFileCacheRequestRequestTypeDef",
-    "WindowsFileSystemConfigurationTypeDef",
+    "WindowsFileSystemConfigurationOutputTypeDef",
+    "DataRepositoryAssociationOutputTypeDef",
     "CreateDataRepositoryAssociationRequestRequestTypeDef",
-    "DataRepositoryAssociationTypeDef",
     "UpdateDataRepositoryAssociationRequestRequestTypeDef",
+    "DeleteFileSystemResponseOutputTypeDef",
+    "DeleteVolumeResponseOutputTypeDef",
     "DeleteFileSystemRequestRequestTypeDef",
-    "DeleteFileSystemResponseTypeDef",
     "DeleteVolumeRequestRequestTypeDef",
-    "DeleteVolumeResponseTypeDef",
     "CreateStorageVirtualMachineRequestRequestTypeDef",
-    "LustreFileSystemConfigurationTypeDef",
-    "CreateDataRepositoryTaskResponseTypeDef",
-    "DescribeDataRepositoryTasksResponseTypeDef",
+    "LustreFileSystemConfigurationOutputTypeDef",
+    "CreateDataRepositoryTaskResponseOutputTypeDef",
+    "DescribeDataRepositoryTasksResponseOutputTypeDef",
     "CreateFileCacheRequestRequestTypeDef",
-    "FileCacheCreatingTypeDef",
-    "FileCacheTypeDef",
-    "OntapFileSystemConfigurationTypeDef",
-    "CreateSnapshotResponseTypeDef",
-    "DescribeSnapshotsResponseTypeDef",
-    "UpdateSnapshotResponseTypeDef",
+    "FileCacheCreatingOutputTypeDef",
+    "FileCacheOutputTypeDef",
+    "OntapFileSystemConfigurationOutputTypeDef",
+    "CreateSnapshotResponseOutputTypeDef",
+    "DescribeSnapshotsResponseOutputTypeDef",
+    "UpdateSnapshotResponseOutputTypeDef",
+    "OpenZFSVolumeConfigurationOutputTypeDef",
     "CreateOpenZFSVolumeConfigurationTypeDef",
     "OpenZFSCreateRootVolumeConfigurationTypeDef",
-    "OpenZFSVolumeConfigurationTypeDef",
     "UpdateOpenZFSVolumeConfigurationTypeDef",
+    "SnaplockConfigurationOutputTypeDef",
     "CreateSnaplockConfigurationTypeDef",
-    "SnaplockConfigurationTypeDef",
     "UpdateSnaplockConfigurationTypeDef",
     "UpdateFileSystemRequestRequestTypeDef",
     "UpdateStorageVirtualMachineRequestRequestTypeDef",
-    "StorageVirtualMachineTypeDef",
-    "CreateDataRepositoryAssociationResponseTypeDef",
-    "DescribeDataRepositoryAssociationsResponseTypeDef",
-    "UpdateDataRepositoryAssociationResponseTypeDef",
-    "CreateFileCacheResponseTypeDef",
-    "DescribeFileCachesResponseTypeDef",
-    "UpdateFileCacheResponseTypeDef",
-    "FileSystemTypeDef",
+    "StorageVirtualMachineOutputTypeDef",
+    "CreateDataRepositoryAssociationResponseOutputTypeDef",
+    "DescribeDataRepositoryAssociationsResponseOutputTypeDef",
+    "UpdateDataRepositoryAssociationResponseOutputTypeDef",
+    "CreateFileCacheResponseOutputTypeDef",
+    "DescribeFileCachesResponseOutputTypeDef",
+    "UpdateFileCacheResponseOutputTypeDef",
+    "FileSystemOutputTypeDef",
     "CreateFileSystemOpenZFSConfigurationTypeDef",
+    "OntapVolumeConfigurationOutputTypeDef",
     "CreateOntapVolumeConfigurationTypeDef",
-    "OntapVolumeConfigurationTypeDef",
     "UpdateOntapVolumeConfigurationTypeDef",
-    "CreateStorageVirtualMachineResponseTypeDef",
-    "DescribeStorageVirtualMachinesResponseTypeDef",
-    "UpdateStorageVirtualMachineResponseTypeDef",
+    "CreateStorageVirtualMachineResponseOutputTypeDef",
+    "DescribeStorageVirtualMachinesResponseOutputTypeDef",
+    "UpdateStorageVirtualMachineResponseOutputTypeDef",
     "CreateFileSystemFromBackupRequestRequestTypeDef",
     "CreateFileSystemRequestRequestTypeDef",
+    "VolumeOutputTypeDef",
     "CreateVolumeFromBackupRequestRequestTypeDef",
     "CreateVolumeRequestRequestTypeDef",
-    "VolumeTypeDef",
     "UpdateVolumeRequestRequestTypeDef",
-    "AdministrativeActionTypeDef",
-    "BackupTypeDef",
-    "CreateVolumeFromBackupResponseTypeDef",
-    "CreateVolumeResponseTypeDef",
-    "DescribeVolumesResponseTypeDef",
-    "UpdateVolumeResponseTypeDef",
-    "CopyBackupResponseTypeDef",
-    "CreateBackupResponseTypeDef",
-    "DescribeBackupsResponseTypeDef",
+    "AdministrativeActionOutputTypeDef",
+    "BackupOutputTypeDef",
+    "CreateVolumeFromBackupResponseOutputTypeDef",
+    "CreateVolumeResponseOutputTypeDef",
+    "DescribeVolumesResponseOutputTypeDef",
+    "UpdateVolumeResponseOutputTypeDef",
+    "CopyBackupResponseOutputTypeDef",
+    "CreateBackupResponseOutputTypeDef",
+    "DescribeBackupsResponseOutputTypeDef",
 )
 
-ActiveDirectoryBackupAttributesTypeDef = TypedDict(
-    "ActiveDirectoryBackupAttributesTypeDef",
+ActiveDirectoryBackupAttributesOutputTypeDef = TypedDict(
+    "ActiveDirectoryBackupAttributesOutputTypeDef",
     {
         "DomainName": str,
         "ActiveDirectoryId": str,
         "ResourceARN": str,
     },
 )
 
-AdministrativeActionFailureDetailsTypeDef = TypedDict(
-    "AdministrativeActionFailureDetailsTypeDef",
+AdministrativeActionFailureDetailsOutputTypeDef = TypedDict(
+    "AdministrativeActionFailureDetailsOutputTypeDef",
     {
         "Message": str,
     },
 )
 
-AliasTypeDef = TypedDict(
-    "AliasTypeDef",
+AliasOutputTypeDef = TypedDict(
+    "AliasOutputTypeDef",
     {
         "Name": str,
         "Lifecycle": AliasLifecycleType,
     },
 )
 
 _RequiredAssociateFileSystemAliasesRequestRequestTypeDef = TypedDict(
@@ -303,69 +318,112 @@
 class AssociateFileSystemAliasesRequestRequestTypeDef(
     _RequiredAssociateFileSystemAliasesRequestRequestTypeDef,
     _OptionalAssociateFileSystemAliasesRequestRequestTypeDef,
 ):
     pass
 
 
+AutoExportPolicyOutputTypeDef = TypedDict(
+    "AutoExportPolicyOutputTypeDef",
+    {
+        "Events": List[EventTypeType],
+    },
+)
+
 AutoExportPolicyTypeDef = TypedDict(
     "AutoExportPolicyTypeDef",
     {
         "Events": Sequence[EventTypeType],
     },
     total=False,
 )
 
+AutoImportPolicyOutputTypeDef = TypedDict(
+    "AutoImportPolicyOutputTypeDef",
+    {
+        "Events": List[EventTypeType],
+    },
+)
+
 AutoImportPolicyTypeDef = TypedDict(
     "AutoImportPolicyTypeDef",
     {
         "Events": Sequence[EventTypeType],
     },
     total=False,
 )
 
-AutocommitPeriodTypeDef = TypedDict(
-    "AutocommitPeriodTypeDef",
+AutocommitPeriodOutputTypeDef = TypedDict(
+    "AutocommitPeriodOutputTypeDef",
     {
         "Type": AutocommitPeriodTypeType,
         "Value": int,
     },
 )
 
-BackupFailureDetailsTypeDef = TypedDict(
-    "BackupFailureDetailsTypeDef",
+_RequiredAutocommitPeriodTypeDef = TypedDict(
+    "_RequiredAutocommitPeriodTypeDef",
+    {
+        "Type": AutocommitPeriodTypeType,
+    },
+)
+_OptionalAutocommitPeriodTypeDef = TypedDict(
+    "_OptionalAutocommitPeriodTypeDef",
+    {
+        "Value": int,
+    },
+    total=False,
+)
+
+
+class AutocommitPeriodTypeDef(_RequiredAutocommitPeriodTypeDef, _OptionalAutocommitPeriodTypeDef):
+    pass
+
+
+BackupFailureDetailsOutputTypeDef = TypedDict(
+    "BackupFailureDetailsOutputTypeDef",
     {
         "Message": str,
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
 CancelDataRepositoryTaskRequestRequestTypeDef = TypedDict(
     "CancelDataRepositoryTaskRequestRequestTypeDef",
     {
         "TaskId": str,
     },
 )
 
-CancelDataRepositoryTaskResponseTypeDef = TypedDict(
-    "CancelDataRepositoryTaskResponseTypeDef",
+CancelDataRepositoryTaskResponseOutputTypeDef = TypedDict(
+    "CancelDataRepositoryTaskResponseOutputTypeDef",
     {
         "Lifecycle": DataRepositoryTaskLifecycleType,
         "TaskId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CompletionReportOutputTypeDef = TypedDict(
+    "CompletionReportOutputTypeDef",
+    {
+        "Enabled": bool,
+        "Path": str,
+        "Format": Literal["REPORT_CSV_20191124"],
+        "Scope": Literal["FAILED_FILES_ONLY"],
+    },
+)
+
 _RequiredCompletionReportTypeDef = TypedDict(
     "_RequiredCompletionReportTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalCompletionReportTypeDef = TypedDict(
@@ -379,25 +437,33 @@
 )
 
 
 class CompletionReportTypeDef(_RequiredCompletionReportTypeDef, _OptionalCompletionReportTypeDef):
     pass
 
 
+TagTypeDef = TypedDict(
+    "TagTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 FileCacheLustreMetadataConfigurationTypeDef = TypedDict(
     "FileCacheLustreMetadataConfigurationTypeDef",
     {
         "StorageCapacity": int,
     },
 )
 
-CreateFileSystemFromBackupResponseTypeDef = TypedDict(
-    "CreateFileSystemFromBackupResponseTypeDef",
+CreateFileSystemFromBackupResponseOutputTypeDef = TypedDict(
+    "CreateFileSystemFromBackupResponseOutputTypeDef",
     {
-        "FileSystem": "FileSystemTypeDef",
+        "FileSystem": "FileSystemOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredLustreLogCreateConfigurationTypeDef = TypedDict(
     "_RequiredLustreLogCreateConfigurationTypeDef",
     {
@@ -419,30 +485,32 @@
     pass
 
 
 LustreRootSquashConfigurationTypeDef = TypedDict(
     "LustreRootSquashConfigurationTypeDef",
     {
         "RootSquash": str,
-        "NoSquashNids": List[str],
+        "NoSquashNids": Sequence[str],
     },
+    total=False,
 )
 
 DiskIopsConfigurationTypeDef = TypedDict(
     "DiskIopsConfigurationTypeDef",
     {
         "Mode": DiskIopsConfigurationModeType,
         "Iops": int,
     },
+    total=False,
 )
 
-CreateFileSystemResponseTypeDef = TypedDict(
-    "CreateFileSystemResponseTypeDef",
+CreateFileSystemResponseOutputTypeDef = TypedDict(
+    "CreateFileSystemResponseOutputTypeDef",
     {
-        "FileSystem": "FileSystemTypeDef",
+        "FileSystem": "FileSystemOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSelfManagedActiveDirectoryConfigurationTypeDef = TypedDict(
     "_RequiredSelfManagedActiveDirectoryConfigurationTypeDef",
     {
@@ -494,14 +562,15 @@
 
 TieringPolicyTypeDef = TypedDict(
     "TieringPolicyTypeDef",
     {
         "CoolingPeriod": int,
         "Name": TieringPolicyNameType,
     },
+    total=False,
 )
 
 CreateOpenZFSOriginSnapshotConfigurationTypeDef = TypedDict(
     "CreateOpenZFSOriginSnapshotConfigurationTypeDef",
     {
         "SnapshotARN": str,
         "CopyStrategy": OpenZFSCopyStrategyType,
@@ -513,39 +582,39 @@
     {
         "Type": OpenZFSQuotaTypeType,
         "Id": int,
         "StorageCapacityQuotaGiB": int,
     },
 )
 
-DataRepositoryFailureDetailsTypeDef = TypedDict(
-    "DataRepositoryFailureDetailsTypeDef",
+DataRepositoryFailureDetailsOutputTypeDef = TypedDict(
+    "DataRepositoryFailureDetailsOutputTypeDef",
     {
         "Message": str,
     },
 )
 
-DataRepositoryTaskFailureDetailsTypeDef = TypedDict(
-    "DataRepositoryTaskFailureDetailsTypeDef",
+DataRepositoryTaskFailureDetailsOutputTypeDef = TypedDict(
+    "DataRepositoryTaskFailureDetailsOutputTypeDef",
     {
         "Message": str,
     },
 )
 
 DataRepositoryTaskFilterTypeDef = TypedDict(
     "DataRepositoryTaskFilterTypeDef",
     {
         "Name": DataRepositoryTaskFilterNameType,
         "Values": Sequence[str],
     },
     total=False,
 )
 
-DataRepositoryTaskStatusTypeDef = TypedDict(
-    "DataRepositoryTaskStatusTypeDef",
+DataRepositoryTaskStatusOutputTypeDef = TypedDict(
+    "DataRepositoryTaskStatusOutputTypeDef",
     {
         "TotalCount": int,
         "SucceededCount": int,
         "FailedCount": int,
         "LastUpdatedTime": datetime,
         "ReleasedCapacity": int,
     },
@@ -568,16 +637,16 @@
 
 class DeleteBackupRequestRequestTypeDef(
     _RequiredDeleteBackupRequestRequestTypeDef, _OptionalDeleteBackupRequestRequestTypeDef
 ):
     pass
 
 
-DeleteBackupResponseTypeDef = TypedDict(
-    "DeleteBackupResponseTypeDef",
+DeleteBackupResponseOutputTypeDef = TypedDict(
+    "DeleteBackupResponseOutputTypeDef",
     {
         "BackupId": str,
         "Lifecycle": BackupLifecycleType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -600,16 +669,16 @@
 class DeleteDataRepositoryAssociationRequestRequestTypeDef(
     _RequiredDeleteDataRepositoryAssociationRequestRequestTypeDef,
     _OptionalDeleteDataRepositoryAssociationRequestRequestTypeDef,
 ):
     pass
 
 
-DeleteDataRepositoryAssociationResponseTypeDef = TypedDict(
-    "DeleteDataRepositoryAssociationResponseTypeDef",
+DeleteDataRepositoryAssociationResponseOutputTypeDef = TypedDict(
+    "DeleteDataRepositoryAssociationResponseOutputTypeDef",
     {
         "AssociationId": str,
         "Lifecycle": DataRepositoryLifecycleType,
         "DeleteDataInFileSystem": bool,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -631,16 +700,16 @@
 
 class DeleteFileCacheRequestRequestTypeDef(
     _RequiredDeleteFileCacheRequestRequestTypeDef, _OptionalDeleteFileCacheRequestRequestTypeDef
 ):
     pass
 
 
-DeleteFileCacheResponseTypeDef = TypedDict(
-    "DeleteFileCacheResponseTypeDef",
+DeleteFileCacheResponseOutputTypeDef = TypedDict(
+    "DeleteFileCacheResponseOutputTypeDef",
     {
         "FileCacheId": str,
         "Lifecycle": FileCacheLifecycleType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -661,16 +730,16 @@
 
 class DeleteSnapshotRequestRequestTypeDef(
     _RequiredDeleteSnapshotRequestRequestTypeDef, _OptionalDeleteSnapshotRequestRequestTypeDef
 ):
     pass
 
 
-DeleteSnapshotResponseTypeDef = TypedDict(
-    "DeleteSnapshotResponseTypeDef",
+DeleteSnapshotResponseOutputTypeDef = TypedDict(
+    "DeleteSnapshotResponseOutputTypeDef",
     {
         "SnapshotId": str,
         "Lifecycle": SnapshotLifecycleType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -692,16 +761,16 @@
 class DeleteStorageVirtualMachineRequestRequestTypeDef(
     _RequiredDeleteStorageVirtualMachineRequestRequestTypeDef,
     _OptionalDeleteStorageVirtualMachineRequestRequestTypeDef,
 ):
     pass
 
 
-DeleteStorageVirtualMachineResponseTypeDef = TypedDict(
-    "DeleteStorageVirtualMachineResponseTypeDef",
+DeleteStorageVirtualMachineResponseOutputTypeDef = TypedDict(
+    "DeleteStorageVirtualMachineResponseOutputTypeDef",
     {
         "StorageVirtualMachineId": str,
         "Lifecycle": StorageVirtualMachineLifecycleType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -771,18 +840,18 @@
         "FileSystemIds": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeFileSystemsResponseTypeDef = TypedDict(
-    "DescribeFileSystemsResponseTypeDef",
+DescribeFileSystemsResponseOutputTypeDef = TypedDict(
+    "DescribeFileSystemsResponseOutputTypeDef",
     {
-        "FileSystems": List["FileSystemTypeDef"],
+        "FileSystems": List["FileSystemOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SnapshotFilterTypeDef = TypedDict(
     "SnapshotFilterTypeDef",
@@ -830,16 +899,24 @@
 class DisassociateFileSystemAliasesRequestRequestTypeDef(
     _RequiredDisassociateFileSystemAliasesRequestRequestTypeDef,
     _OptionalDisassociateFileSystemAliasesRequestRequestTypeDef,
 ):
     pass
 
 
-FileCacheFailureDetailsTypeDef = TypedDict(
-    "FileCacheFailureDetailsTypeDef",
+DiskIopsConfigurationOutputTypeDef = TypedDict(
+    "DiskIopsConfigurationOutputTypeDef",
+    {
+        "Mode": DiskIopsConfigurationModeType,
+        "Iops": int,
+    },
+)
+
+FileCacheFailureDetailsOutputTypeDef = TypedDict(
+    "FileCacheFailureDetailsOutputTypeDef",
     {
         "Message": str,
     },
 )
 
 _RequiredFileCacheNFSConfigurationTypeDef = TypedDict(
     "_RequiredFileCacheNFSConfigurationTypeDef",
@@ -858,39 +935,46 @@
 
 class FileCacheNFSConfigurationTypeDef(
     _RequiredFileCacheNFSConfigurationTypeDef, _OptionalFileCacheNFSConfigurationTypeDef
 ):
     pass
 
 
-LustreLogConfigurationTypeDef = TypedDict(
-    "LustreLogConfigurationTypeDef",
+FileCacheLustreMetadataConfigurationOutputTypeDef = TypedDict(
+    "FileCacheLustreMetadataConfigurationOutputTypeDef",
+    {
+        "StorageCapacity": int,
+    },
+)
+
+LustreLogConfigurationOutputTypeDef = TypedDict(
+    "LustreLogConfigurationOutputTypeDef",
     {
         "Level": LustreAccessAuditLogLevelType,
         "Destination": str,
     },
 )
 
-FileSystemEndpointTypeDef = TypedDict(
-    "FileSystemEndpointTypeDef",
+FileSystemEndpointOutputTypeDef = TypedDict(
+    "FileSystemEndpointOutputTypeDef",
     {
         "DNSName": str,
         "IpAddresses": List[str],
     },
 )
 
-FileSystemFailureDetailsTypeDef = TypedDict(
-    "FileSystemFailureDetailsTypeDef",
+FileSystemFailureDetailsOutputTypeDef = TypedDict(
+    "FileSystemFailureDetailsOutputTypeDef",
     {
         "Message": str,
     },
 )
 
-LifecycleTransitionReasonTypeDef = TypedDict(
-    "LifecycleTransitionReasonTypeDef",
+LifecycleTransitionReasonOutputTypeDef = TypedDict(
+    "LifecycleTransitionReasonOutputTypeDef",
     {
         "Message": str,
     },
 )
 
 _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
@@ -933,30 +1017,63 @@
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
 
+LustreRootSquashConfigurationOutputTypeDef = TypedDict(
+    "LustreRootSquashConfigurationOutputTypeDef",
+    {
+        "RootSquash": str,
+        "NoSquashNids": List[str],
+    },
+)
+
+TieringPolicyOutputTypeDef = TypedDict(
+    "TieringPolicyOutputTypeDef",
+    {
+        "CoolingPeriod": int,
+        "Name": TieringPolicyNameType,
+    },
+)
+
+OpenZFSClientConfigurationOutputTypeDef = TypedDict(
+    "OpenZFSClientConfigurationOutputTypeDef",
+    {
+        "Clients": str,
+        "Options": List[str],
+    },
+)
+
 OpenZFSClientConfigurationTypeDef = TypedDict(
     "OpenZFSClientConfigurationTypeDef",
     {
         "Clients": str,
-        "Options": List[str],
+        "Options": Sequence[str],
     },
 )
 
-OpenZFSOriginSnapshotConfigurationTypeDef = TypedDict(
-    "OpenZFSOriginSnapshotConfigurationTypeDef",
+OpenZFSOriginSnapshotConfigurationOutputTypeDef = TypedDict(
+    "OpenZFSOriginSnapshotConfigurationOutputTypeDef",
     {
         "SnapshotARN": str,
         "CopyStrategy": OpenZFSCopyStrategyType,
     },
 )
 
+OpenZFSUserOrGroupQuotaOutputTypeDef = TypedDict(
+    "OpenZFSUserOrGroupQuotaOutputTypeDef",
+    {
+        "Type": OpenZFSQuotaTypeType,
+        "Id": int,
+        "StorageCapacityQuotaGiB": int,
+    },
+)
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -981,18 +1098,18 @@
 class ReleaseFileSystemNfsV3LocksRequestRequestTypeDef(
     _RequiredReleaseFileSystemNfsV3LocksRequestRequestTypeDef,
     _OptionalReleaseFileSystemNfsV3LocksRequestRequestTypeDef,
 ):
     pass
 
 
-ReleaseFileSystemNfsV3LocksResponseTypeDef = TypedDict(
-    "ReleaseFileSystemNfsV3LocksResponseTypeDef",
+ReleaseFileSystemNfsV3LocksResponseOutputTypeDef = TypedDict(
+    "ReleaseFileSystemNfsV3LocksResponseOutputTypeDef",
     {
-        "FileSystem": "FileSystemTypeDef",
+        "FileSystem": "FileSystemOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
@@ -1024,34 +1141,53 @@
 class RestoreVolumeFromSnapshotRequestRequestTypeDef(
     _RequiredRestoreVolumeFromSnapshotRequestRequestTypeDef,
     _OptionalRestoreVolumeFromSnapshotRequestRequestTypeDef,
 ):
     pass
 
 
-RestoreVolumeFromSnapshotResponseTypeDef = TypedDict(
-    "RestoreVolumeFromSnapshotResponseTypeDef",
+RestoreVolumeFromSnapshotResponseOutputTypeDef = TypedDict(
+    "RestoreVolumeFromSnapshotResponseOutputTypeDef",
     {
         "VolumeId": str,
         "Lifecycle": VolumeLifecycleType,
-        "AdministrativeActions": List["AdministrativeActionTypeDef"],
+        "AdministrativeActions": List["AdministrativeActionOutputTypeDef"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RetentionPeriodTypeDef = TypedDict(
-    "RetentionPeriodTypeDef",
+RetentionPeriodOutputTypeDef = TypedDict(
+    "RetentionPeriodOutputTypeDef",
+    {
+        "Type": RetentionPeriodTypeType,
+        "Value": int,
+    },
+)
+
+_RequiredRetentionPeriodTypeDef = TypedDict(
+    "_RequiredRetentionPeriodTypeDef",
     {
         "Type": RetentionPeriodTypeType,
+    },
+)
+_OptionalRetentionPeriodTypeDef = TypedDict(
+    "_OptionalRetentionPeriodTypeDef",
+    {
         "Value": int,
     },
+    total=False,
 )
 
-SelfManagedActiveDirectoryAttributesTypeDef = TypedDict(
-    "SelfManagedActiveDirectoryAttributesTypeDef",
+
+class RetentionPeriodTypeDef(_RequiredRetentionPeriodTypeDef, _OptionalRetentionPeriodTypeDef):
+    pass
+
+
+SelfManagedActiveDirectoryAttributesOutputTypeDef = TypedDict(
+    "SelfManagedActiveDirectoryAttributesOutputTypeDef",
     {
         "DomainName": str,
         "OrganizationalUnitDistinguishedName": str,
         "FileSystemAdministratorsGroup": str,
         "UserName": str,
         "DnsIps": List[str],
     },
@@ -1066,16 +1202,16 @@
         "DomainName": str,
         "OrganizationalUnitDistinguishedName": str,
         "FileSystemAdministratorsGroup": str,
     },
     total=False,
 )
 
-SvmEndpointTypeDef = TypedDict(
-    "SvmEndpointTypeDef",
+SvmEndpointOutputTypeDef = TypedDict(
+    "SvmEndpointOutputTypeDef",
     {
         "DNSName": str,
         "IpAddresses": List[str],
     },
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
@@ -1090,18 +1226,18 @@
     "UpdateFileCacheLustreConfigurationTypeDef",
     {
         "WeeklyMaintenanceStartTime": str,
     },
     total=False,
 )
 
-UpdateFileSystemResponseTypeDef = TypedDict(
-    "UpdateFileSystemResponseTypeDef",
+UpdateFileSystemResponseOutputTypeDef = TypedDict(
+    "UpdateFileSystemResponseOutputTypeDef",
     {
-        "FileSystem": "FileSystemTypeDef",
+        "FileSystem": "FileSystemOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSnapshotRequestRequestTypeDef",
     {
@@ -1120,66 +1256,115 @@
 
 class UpdateSnapshotRequestRequestTypeDef(
     _RequiredUpdateSnapshotRequestRequestTypeDef, _OptionalUpdateSnapshotRequestRequestTypeDef
 ):
     pass
 
 
-WindowsAuditLogConfigurationTypeDef = TypedDict(
-    "WindowsAuditLogConfigurationTypeDef",
+WindowsAuditLogConfigurationOutputTypeDef = TypedDict(
+    "WindowsAuditLogConfigurationOutputTypeDef",
     {
         "FileAccessAuditLogLevel": WindowsAccessAuditLogLevelType,
         "FileShareAccessAuditLogLevel": WindowsAccessAuditLogLevelType,
         "AuditLogDestination": str,
     },
 )
 
-AssociateFileSystemAliasesResponseTypeDef = TypedDict(
-    "AssociateFileSystemAliasesResponseTypeDef",
+AssociateFileSystemAliasesResponseOutputTypeDef = TypedDict(
+    "AssociateFileSystemAliasesResponseOutputTypeDef",
     {
-        "Aliases": List[AliasTypeDef],
+        "Aliases": List[AliasOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeFileSystemAliasesResponseTypeDef = TypedDict(
-    "DescribeFileSystemAliasesResponseTypeDef",
+DescribeFileSystemAliasesResponseOutputTypeDef = TypedDict(
+    "DescribeFileSystemAliasesResponseOutputTypeDef",
     {
-        "Aliases": List[AliasTypeDef],
+        "Aliases": List[AliasOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DisassociateFileSystemAliasesResponseTypeDef = TypedDict(
-    "DisassociateFileSystemAliasesResponseTypeDef",
+DisassociateFileSystemAliasesResponseOutputTypeDef = TypedDict(
+    "DisassociateFileSystemAliasesResponseOutputTypeDef",
     {
-        "Aliases": List[AliasTypeDef],
+        "Aliases": List[AliasOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-NFSDataRepositoryConfigurationTypeDef = TypedDict(
-    "NFSDataRepositoryConfigurationTypeDef",
+NFSDataRepositoryConfigurationOutputTypeDef = TypedDict(
+    "NFSDataRepositoryConfigurationOutputTypeDef",
     {
         "Version": Literal["NFS3"],
         "DnsIps": List[str],
-        "AutoExportPolicy": AutoExportPolicyTypeDef,
+        "AutoExportPolicy": AutoExportPolicyOutputTypeDef,
+    },
+)
+
+S3DataRepositoryConfigurationOutputTypeDef = TypedDict(
+    "S3DataRepositoryConfigurationOutputTypeDef",
+    {
+        "AutoImportPolicy": AutoImportPolicyOutputTypeDef,
+        "AutoExportPolicy": AutoExportPolicyOutputTypeDef,
     },
 )
 
 S3DataRepositoryConfigurationTypeDef = TypedDict(
     "S3DataRepositoryConfigurationTypeDef",
     {
         "AutoImportPolicy": AutoImportPolicyTypeDef,
         "AutoExportPolicy": AutoExportPolicyTypeDef,
     },
     total=False,
 )
 
+DeleteFileSystemLustreResponseOutputTypeDef = TypedDict(
+    "DeleteFileSystemLustreResponseOutputTypeDef",
+    {
+        "FinalBackupId": str,
+        "FinalBackupTags": List[TagOutputTypeDef],
+    },
+)
+
+DeleteFileSystemOpenZFSResponseOutputTypeDef = TypedDict(
+    "DeleteFileSystemOpenZFSResponseOutputTypeDef",
+    {
+        "FinalBackupId": str,
+        "FinalBackupTags": List[TagOutputTypeDef],
+    },
+)
+
+DeleteFileSystemWindowsResponseOutputTypeDef = TypedDict(
+    "DeleteFileSystemWindowsResponseOutputTypeDef",
+    {
+        "FinalBackupId": str,
+        "FinalBackupTags": List[TagOutputTypeDef],
+    },
+)
+
+DeleteVolumeOntapResponseOutputTypeDef = TypedDict(
+    "DeleteVolumeOntapResponseOutputTypeDef",
+    {
+        "FinalBackupId": str,
+        "FinalBackupTags": List[TagOutputTypeDef],
+    },
+)
+
+ListTagsForResourceResponseOutputTypeDef = TypedDict(
+    "ListTagsForResourceResponseOutputTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCopyBackupRequestRequestTypeDef = TypedDict(
     "_RequiredCopyBackupRequestRequestTypeDef",
     {
         "SourceBackupId": str,
     },
 )
 _OptionalCopyBackupRequestRequestTypeDef = TypedDict(
@@ -1208,14 +1393,41 @@
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
         "VolumeId": str,
     },
     total=False,
 )
 
+_RequiredCreateDataRepositoryTaskRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDataRepositoryTaskRequestRequestTypeDef",
+    {
+        "Type": DataRepositoryTaskTypeType,
+        "FileSystemId": str,
+        "Report": CompletionReportTypeDef,
+    },
+)
+_OptionalCreateDataRepositoryTaskRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDataRepositoryTaskRequestRequestTypeDef",
+    {
+        "Paths": Sequence[str],
+        "ClientRequestToken": str,
+        "Tags": Sequence[TagTypeDef],
+        "CapacityToRelease": int,
+    },
+    total=False,
+)
+
+
+class CreateDataRepositoryTaskRequestRequestTypeDef(
+    _RequiredCreateDataRepositoryTaskRequestRequestTypeDef,
+    _OptionalCreateDataRepositoryTaskRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredCreateSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSnapshotRequestRequestTypeDef",
     {
         "Name": str,
         "VolumeId": str,
     },
 )
@@ -1240,119 +1452,51 @@
     {
         "SkipFinalBackup": bool,
         "FinalBackupTags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-DeleteFileSystemLustreResponseTypeDef = TypedDict(
-    "DeleteFileSystemLustreResponseTypeDef",
-    {
-        "FinalBackupId": str,
-        "FinalBackupTags": List[TagTypeDef],
-    },
-)
-
 DeleteFileSystemOpenZFSConfigurationTypeDef = TypedDict(
     "DeleteFileSystemOpenZFSConfigurationTypeDef",
     {
         "SkipFinalBackup": bool,
         "FinalBackupTags": Sequence[TagTypeDef],
         "Options": Sequence[Literal["DELETE_CHILD_VOLUMES_AND_SNAPSHOTS"]],
     },
     total=False,
 )
 
-DeleteFileSystemOpenZFSResponseTypeDef = TypedDict(
-    "DeleteFileSystemOpenZFSResponseTypeDef",
-    {
-        "FinalBackupId": str,
-        "FinalBackupTags": List[TagTypeDef],
-    },
-)
-
 DeleteFileSystemWindowsConfigurationTypeDef = TypedDict(
     "DeleteFileSystemWindowsConfigurationTypeDef",
     {
         "SkipFinalBackup": bool,
         "FinalBackupTags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-DeleteFileSystemWindowsResponseTypeDef = TypedDict(
-    "DeleteFileSystemWindowsResponseTypeDef",
-    {
-        "FinalBackupId": str,
-        "FinalBackupTags": List[TagTypeDef],
-    },
-)
-
 DeleteVolumeOntapConfigurationTypeDef = TypedDict(
     "DeleteVolumeOntapConfigurationTypeDef",
     {
         "SkipFinalBackup": bool,
         "FinalBackupTags": Sequence[TagTypeDef],
         "BypassSnaplockEnterpriseRetention": bool,
     },
     total=False,
 )
 
-DeleteVolumeOntapResponseTypeDef = TypedDict(
-    "DeleteVolumeOntapResponseTypeDef",
-    {
-        "FinalBackupId": str,
-        "FinalBackupTags": List[TagTypeDef],
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-_RequiredCreateDataRepositoryTaskRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDataRepositoryTaskRequestRequestTypeDef",
-    {
-        "Type": DataRepositoryTaskTypeType,
-        "FileSystemId": str,
-        "Report": CompletionReportTypeDef,
-    },
-)
-_OptionalCreateDataRepositoryTaskRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDataRepositoryTaskRequestRequestTypeDef",
-    {
-        "Paths": Sequence[str],
-        "ClientRequestToken": str,
-        "Tags": Sequence[TagTypeDef],
-        "CapacityToRelease": int,
-    },
-    total=False,
-)
-
-
-class CreateDataRepositoryTaskRequestRequestTypeDef(
-    _RequiredCreateDataRepositoryTaskRequestRequestTypeDef,
-    _OptionalCreateDataRepositoryTaskRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredCreateFileCacheLustreConfigurationTypeDef = TypedDict(
     "_RequiredCreateFileCacheLustreConfigurationTypeDef",
     {
         "PerUnitStorageThroughput": int,
         "DeploymentType": Literal["CACHE_1"],
         "MetadataConfiguration": FileCacheLustreMetadataConfigurationTypeDef,
     },
@@ -1434,29 +1578,14 @@
 class CreateFileSystemOntapConfigurationTypeDef(
     _RequiredCreateFileSystemOntapConfigurationTypeDef,
     _OptionalCreateFileSystemOntapConfigurationTypeDef,
 ):
     pass
 
 
-OpenZFSFileSystemConfigurationTypeDef = TypedDict(
-    "OpenZFSFileSystemConfigurationTypeDef",
-    {
-        "AutomaticBackupRetentionDays": int,
-        "CopyTagsToBackups": bool,
-        "CopyTagsToVolumes": bool,
-        "DailyAutomaticBackupStartTime": str,
-        "DeploymentType": OpenZFSDeploymentTypeType,
-        "ThroughputCapacity": int,
-        "WeeklyMaintenanceStartTime": str,
-        "DiskIopsConfiguration": DiskIopsConfigurationTypeDef,
-        "RootVolumeId": str,
-    },
-)
-
 UpdateFileSystemOntapConfigurationTypeDef = TypedDict(
     "UpdateFileSystemOntapConfigurationTypeDef",
     {
         "AutomaticBackupRetentionDays": int,
         "DailyAutomaticBackupStartTime": str,
         "FsxAdminPassword": str,
         "WeeklyMaintenanceStartTime": str,
@@ -1531,53 +1660,53 @@
 class CreateFileSystemWindowsConfigurationTypeDef(
     _RequiredCreateFileSystemWindowsConfigurationTypeDef,
     _OptionalCreateFileSystemWindowsConfigurationTypeDef,
 ):
     pass
 
 
-DataRepositoryConfigurationTypeDef = TypedDict(
-    "DataRepositoryConfigurationTypeDef",
+DataRepositoryConfigurationOutputTypeDef = TypedDict(
+    "DataRepositoryConfigurationOutputTypeDef",
     {
         "Lifecycle": DataRepositoryLifecycleType,
         "ImportPath": str,
         "ExportPath": str,
         "ImportedFileChunkSize": int,
         "AutoImportPolicy": AutoImportPolicyTypeType,
-        "FailureDetails": DataRepositoryFailureDetailsTypeDef,
+        "FailureDetails": DataRepositoryFailureDetailsOutputTypeDef,
     },
 )
 
 DescribeDataRepositoryTasksRequestRequestTypeDef = TypedDict(
     "DescribeDataRepositoryTasksRequestRequestTypeDef",
     {
         "TaskIds": Sequence[str],
         "Filters": Sequence[DataRepositoryTaskFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DataRepositoryTaskTypeDef = TypedDict(
-    "DataRepositoryTaskTypeDef",
+DataRepositoryTaskOutputTypeDef = TypedDict(
+    "DataRepositoryTaskOutputTypeDef",
     {
         "TaskId": str,
         "Lifecycle": DataRepositoryTaskLifecycleType,
         "Type": DataRepositoryTaskTypeType,
         "CreationTime": datetime,
         "StartTime": datetime,
         "EndTime": datetime,
         "ResourceARN": str,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "FileSystemId": str,
         "Paths": List[str],
-        "FailureDetails": DataRepositoryTaskFailureDetailsTypeDef,
-        "Status": DataRepositoryTaskStatusTypeDef,
-        "Report": CompletionReportTypeDef,
+        "FailureDetails": DataRepositoryTaskFailureDetailsOutputTypeDef,
+        "Status": DataRepositoryTaskStatusOutputTypeDef,
+        "Report": CompletionReportOutputTypeDef,
         "CapacityToRelease": int,
         "FileCacheId": str,
     },
 )
 
 DescribeBackupsRequestDescribeBackupsPaginateTypeDef = TypedDict(
     "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
@@ -1660,14 +1789,29 @@
         "Filters": Sequence[VolumeFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+OpenZFSFileSystemConfigurationOutputTypeDef = TypedDict(
+    "OpenZFSFileSystemConfigurationOutputTypeDef",
+    {
+        "AutomaticBackupRetentionDays": int,
+        "CopyTagsToBackups": bool,
+        "CopyTagsToVolumes": bool,
+        "DailyAutomaticBackupStartTime": str,
+        "DeploymentType": OpenZFSDeploymentTypeType,
+        "ThroughputCapacity": int,
+        "WeeklyMaintenanceStartTime": str,
+        "DiskIopsConfiguration": DiskIopsConfigurationOutputTypeDef,
+        "RootVolumeId": str,
+    },
+)
+
 _RequiredFileCacheDataRepositoryAssociationTypeDef = TypedDict(
     "_RequiredFileCacheDataRepositoryAssociationTypeDef",
     {
         "FileCachePath": str,
         "DataRepositoryPath": str,
     },
 )
@@ -1684,70 +1828,88 @@
 class FileCacheDataRepositoryAssociationTypeDef(
     _RequiredFileCacheDataRepositoryAssociationTypeDef,
     _OptionalFileCacheDataRepositoryAssociationTypeDef,
 ):
     pass
 
 
-FileCacheLustreConfigurationTypeDef = TypedDict(
-    "FileCacheLustreConfigurationTypeDef",
+FileCacheLustreConfigurationOutputTypeDef = TypedDict(
+    "FileCacheLustreConfigurationOutputTypeDef",
     {
         "PerUnitStorageThroughput": int,
         "DeploymentType": Literal["CACHE_1"],
         "MountName": str,
         "WeeklyMaintenanceStartTime": str,
-        "MetadataConfiguration": FileCacheLustreMetadataConfigurationTypeDef,
-        "LogConfiguration": LustreLogConfigurationTypeDef,
+        "MetadataConfiguration": FileCacheLustreMetadataConfigurationOutputTypeDef,
+        "LogConfiguration": LustreLogConfigurationOutputTypeDef,
     },
 )
 
-FileSystemEndpointsTypeDef = TypedDict(
-    "FileSystemEndpointsTypeDef",
+FileSystemEndpointsOutputTypeDef = TypedDict(
+    "FileSystemEndpointsOutputTypeDef",
     {
-        "Intercluster": FileSystemEndpointTypeDef,
-        "Management": FileSystemEndpointTypeDef,
+        "Intercluster": FileSystemEndpointOutputTypeDef,
+        "Management": FileSystemEndpointOutputTypeDef,
     },
 )
 
-SnapshotTypeDef = TypedDict(
-    "SnapshotTypeDef",
+SnapshotOutputTypeDef = TypedDict(
+    "SnapshotOutputTypeDef",
     {
         "ResourceARN": str,
         "SnapshotId": str,
         "Name": str,
         "VolumeId": str,
         "CreationTime": datetime,
         "Lifecycle": SnapshotLifecycleType,
-        "LifecycleTransitionReason": LifecycleTransitionReasonTypeDef,
-        "Tags": List[TagTypeDef],
-        "AdministrativeActions": List["AdministrativeActionTypeDef"],
+        "LifecycleTransitionReason": LifecycleTransitionReasonOutputTypeDef,
+        "Tags": List[TagOutputTypeDef],
+        "AdministrativeActions": List["AdministrativeActionOutputTypeDef"],
+    },
+)
+
+OpenZFSNfsExportOutputTypeDef = TypedDict(
+    "OpenZFSNfsExportOutputTypeDef",
+    {
+        "ClientConfigurations": List[OpenZFSClientConfigurationOutputTypeDef],
     },
 )
 
 OpenZFSNfsExportTypeDef = TypedDict(
     "OpenZFSNfsExportTypeDef",
     {
-        "ClientConfigurations": List[OpenZFSClientConfigurationTypeDef],
+        "ClientConfigurations": Sequence[OpenZFSClientConfigurationTypeDef],
+    },
+)
+
+SnaplockRetentionPeriodOutputTypeDef = TypedDict(
+    "SnaplockRetentionPeriodOutputTypeDef",
+    {
+        "DefaultRetention": RetentionPeriodOutputTypeDef,
+        "MinimumRetention": RetentionPeriodOutputTypeDef,
+        "MaximumRetention": RetentionPeriodOutputTypeDef,
     },
 )
 
 SnaplockRetentionPeriodTypeDef = TypedDict(
     "SnaplockRetentionPeriodTypeDef",
     {
         "DefaultRetention": RetentionPeriodTypeDef,
         "MinimumRetention": RetentionPeriodTypeDef,
         "MaximumRetention": RetentionPeriodTypeDef,
     },
 )
 
-SvmActiveDirectoryConfigurationTypeDef = TypedDict(
-    "SvmActiveDirectoryConfigurationTypeDef",
+SvmActiveDirectoryConfigurationOutputTypeDef = TypedDict(
+    "SvmActiveDirectoryConfigurationOutputTypeDef",
     {
         "NetBiosName": str,
-        "SelfManagedActiveDirectoryConfiguration": SelfManagedActiveDirectoryAttributesTypeDef,
+        "SelfManagedActiveDirectoryConfiguration": (
+            SelfManagedActiveDirectoryAttributesOutputTypeDef
+        ),
     },
 )
 
 UpdateFileSystemWindowsConfigurationTypeDef = TypedDict(
     "UpdateFileSystemWindowsConfigurationTypeDef",
     {
         "WeeklyMaintenanceStartTime": str,
@@ -1769,21 +1931,21 @@
             SelfManagedActiveDirectoryConfigurationUpdatesTypeDef
         ),
         "NetBiosName": str,
     },
     total=False,
 )
 
-SvmEndpointsTypeDef = TypedDict(
-    "SvmEndpointsTypeDef",
+SvmEndpointsOutputTypeDef = TypedDict(
+    "SvmEndpointsOutputTypeDef",
     {
-        "Iscsi": SvmEndpointTypeDef,
-        "Management": SvmEndpointTypeDef,
-        "Nfs": SvmEndpointTypeDef,
-        "Smb": SvmEndpointTypeDef,
+        "Iscsi": SvmEndpointOutputTypeDef,
+        "Management": SvmEndpointOutputTypeDef,
+        "Nfs": SvmEndpointOutputTypeDef,
+        "Smb": SvmEndpointOutputTypeDef,
     },
 )
 
 _RequiredUpdateFileCacheRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFileCacheRequestRequestTypeDef",
     {
         "FileCacheId": str,
@@ -1801,31 +1963,55 @@
 
 class UpdateFileCacheRequestRequestTypeDef(
     _RequiredUpdateFileCacheRequestRequestTypeDef, _OptionalUpdateFileCacheRequestRequestTypeDef
 ):
     pass
 
 
-WindowsFileSystemConfigurationTypeDef = TypedDict(
-    "WindowsFileSystemConfigurationTypeDef",
+WindowsFileSystemConfigurationOutputTypeDef = TypedDict(
+    "WindowsFileSystemConfigurationOutputTypeDef",
     {
         "ActiveDirectoryId": str,
-        "SelfManagedActiveDirectoryConfiguration": SelfManagedActiveDirectoryAttributesTypeDef,
+        "SelfManagedActiveDirectoryConfiguration": (
+            SelfManagedActiveDirectoryAttributesOutputTypeDef
+        ),
         "DeploymentType": WindowsDeploymentTypeType,
         "RemoteAdministrationEndpoint": str,
         "PreferredSubnetId": str,
         "PreferredFileServerIp": str,
         "ThroughputCapacity": int,
         "MaintenanceOperationsInProgress": List[FileSystemMaintenanceOperationType],
         "WeeklyMaintenanceStartTime": str,
         "DailyAutomaticBackupStartTime": str,
         "AutomaticBackupRetentionDays": int,
         "CopyTagsToBackups": bool,
-        "Aliases": List[AliasTypeDef],
-        "AuditLogConfiguration": WindowsAuditLogConfigurationTypeDef,
+        "Aliases": List[AliasOutputTypeDef],
+        "AuditLogConfiguration": WindowsAuditLogConfigurationOutputTypeDef,
+    },
+)
+
+DataRepositoryAssociationOutputTypeDef = TypedDict(
+    "DataRepositoryAssociationOutputTypeDef",
+    {
+        "AssociationId": str,
+        "ResourceARN": str,
+        "FileSystemId": str,
+        "Lifecycle": DataRepositoryLifecycleType,
+        "FailureDetails": DataRepositoryFailureDetailsOutputTypeDef,
+        "FileSystemPath": str,
+        "DataRepositoryPath": str,
+        "BatchImportMetaDataOnCreate": bool,
+        "ImportedFileChunkSize": int,
+        "S3": S3DataRepositoryConfigurationOutputTypeDef,
+        "Tags": List[TagOutputTypeDef],
+        "CreationTime": datetime,
+        "FileCacheId": str,
+        "FileCachePath": str,
+        "DataRepositorySubdirectories": List[str],
+        "NFS": NFSDataRepositoryConfigurationOutputTypeDef,
     },
 )
 
 _RequiredCreateDataRepositoryAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataRepositoryAssociationRequestRequestTypeDef",
     {
         "FileSystemId": str,
@@ -1849,36 +2035,14 @@
 class CreateDataRepositoryAssociationRequestRequestTypeDef(
     _RequiredCreateDataRepositoryAssociationRequestRequestTypeDef,
     _OptionalCreateDataRepositoryAssociationRequestRequestTypeDef,
 ):
     pass
 
 
-DataRepositoryAssociationTypeDef = TypedDict(
-    "DataRepositoryAssociationTypeDef",
-    {
-        "AssociationId": str,
-        "ResourceARN": str,
-        "FileSystemId": str,
-        "Lifecycle": DataRepositoryLifecycleType,
-        "FailureDetails": DataRepositoryFailureDetailsTypeDef,
-        "FileSystemPath": str,
-        "DataRepositoryPath": str,
-        "BatchImportMetaDataOnCreate": bool,
-        "ImportedFileChunkSize": int,
-        "S3": S3DataRepositoryConfigurationTypeDef,
-        "Tags": List[TagTypeDef],
-        "CreationTime": datetime,
-        "FileCacheId": str,
-        "FileCachePath": str,
-        "DataRepositorySubdirectories": List[str],
-        "NFS": NFSDataRepositoryConfigurationTypeDef,
-    },
-)
-
 _RequiredUpdateDataRepositoryAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDataRepositoryAssociationRequestRequestTypeDef",
     {
         "AssociationId": str,
     },
 )
 _OptionalUpdateDataRepositoryAssociationRequestRequestTypeDef = TypedDict(
@@ -1895,14 +2059,36 @@
 class UpdateDataRepositoryAssociationRequestRequestTypeDef(
     _RequiredUpdateDataRepositoryAssociationRequestRequestTypeDef,
     _OptionalUpdateDataRepositoryAssociationRequestRequestTypeDef,
 ):
     pass
 
 
+DeleteFileSystemResponseOutputTypeDef = TypedDict(
+    "DeleteFileSystemResponseOutputTypeDef",
+    {
+        "FileSystemId": str,
+        "Lifecycle": FileSystemLifecycleType,
+        "WindowsResponse": DeleteFileSystemWindowsResponseOutputTypeDef,
+        "LustreResponse": DeleteFileSystemLustreResponseOutputTypeDef,
+        "OpenZFSResponse": DeleteFileSystemOpenZFSResponseOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DeleteVolumeResponseOutputTypeDef = TypedDict(
+    "DeleteVolumeResponseOutputTypeDef",
+    {
+        "VolumeId": str,
+        "Lifecycle": VolumeLifecycleType,
+        "OntapResponse": DeleteVolumeOntapResponseOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteFileSystemRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteFileSystemRequestRequestTypeDef",
     {
         "FileSystemId": str,
     },
 )
 _OptionalDeleteFileSystemRequestRequestTypeDef = TypedDict(
@@ -1919,26 +2105,14 @@
 
 class DeleteFileSystemRequestRequestTypeDef(
     _RequiredDeleteFileSystemRequestRequestTypeDef, _OptionalDeleteFileSystemRequestRequestTypeDef
 ):
     pass
 
 
-DeleteFileSystemResponseTypeDef = TypedDict(
-    "DeleteFileSystemResponseTypeDef",
-    {
-        "FileSystemId": str,
-        "Lifecycle": FileSystemLifecycleType,
-        "WindowsResponse": DeleteFileSystemWindowsResponseTypeDef,
-        "LustreResponse": DeleteFileSystemLustreResponseTypeDef,
-        "OpenZFSResponse": DeleteFileSystemOpenZFSResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteVolumeRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteVolumeRequestRequestTypeDef",
     {
         "VolumeId": str,
     },
 )
 _OptionalDeleteVolumeRequestRequestTypeDef = TypedDict(
@@ -1954,24 +2128,14 @@
 
 class DeleteVolumeRequestRequestTypeDef(
     _RequiredDeleteVolumeRequestRequestTypeDef, _OptionalDeleteVolumeRequestRequestTypeDef
 ):
     pass
 
 
-DeleteVolumeResponseTypeDef = TypedDict(
-    "DeleteVolumeResponseTypeDef",
-    {
-        "VolumeId": str,
-        "Lifecycle": VolumeLifecycleType,
-        "OntapResponse": DeleteVolumeOntapResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateStorageVirtualMachineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStorageVirtualMachineRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "Name": str,
     },
 )
@@ -1991,44 +2155,44 @@
 class CreateStorageVirtualMachineRequestRequestTypeDef(
     _RequiredCreateStorageVirtualMachineRequestRequestTypeDef,
     _OptionalCreateStorageVirtualMachineRequestRequestTypeDef,
 ):
     pass
 
 
-LustreFileSystemConfigurationTypeDef = TypedDict(
-    "LustreFileSystemConfigurationTypeDef",
+LustreFileSystemConfigurationOutputTypeDef = TypedDict(
+    "LustreFileSystemConfigurationOutputTypeDef",
     {
         "WeeklyMaintenanceStartTime": str,
-        "DataRepositoryConfiguration": DataRepositoryConfigurationTypeDef,
+        "DataRepositoryConfiguration": DataRepositoryConfigurationOutputTypeDef,
         "DeploymentType": LustreDeploymentTypeType,
         "PerUnitStorageThroughput": int,
         "MountName": str,
         "DailyAutomaticBackupStartTime": str,
         "AutomaticBackupRetentionDays": int,
         "CopyTagsToBackups": bool,
         "DriveCacheType": DriveCacheTypeType,
         "DataCompressionType": DataCompressionTypeType,
-        "LogConfiguration": LustreLogConfigurationTypeDef,
-        "RootSquashConfiguration": LustreRootSquashConfigurationTypeDef,
+        "LogConfiguration": LustreLogConfigurationOutputTypeDef,
+        "RootSquashConfiguration": LustreRootSquashConfigurationOutputTypeDef,
     },
 )
 
-CreateDataRepositoryTaskResponseTypeDef = TypedDict(
-    "CreateDataRepositoryTaskResponseTypeDef",
+CreateDataRepositoryTaskResponseOutputTypeDef = TypedDict(
+    "CreateDataRepositoryTaskResponseOutputTypeDef",
     {
-        "DataRepositoryTask": DataRepositoryTaskTypeDef,
+        "DataRepositoryTask": DataRepositoryTaskOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeDataRepositoryTasksResponseTypeDef = TypedDict(
-    "DescribeDataRepositoryTasksResponseTypeDef",
+DescribeDataRepositoryTasksResponseOutputTypeDef = TypedDict(
+    "DescribeDataRepositoryTasksResponseOutputTypeDef",
     {
-        "DataRepositoryTasks": List[DataRepositoryTaskTypeDef],
+        "DataRepositoryTasks": List[DataRepositoryTaskOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateFileCacheRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFileCacheRequestRequestTypeDef",
@@ -2056,102 +2220,122 @@
 
 class CreateFileCacheRequestRequestTypeDef(
     _RequiredCreateFileCacheRequestRequestTypeDef, _OptionalCreateFileCacheRequestRequestTypeDef
 ):
     pass
 
 
-FileCacheCreatingTypeDef = TypedDict(
-    "FileCacheCreatingTypeDef",
+FileCacheCreatingOutputTypeDef = TypedDict(
+    "FileCacheCreatingOutputTypeDef",
     {
         "OwnerId": str,
         "CreationTime": datetime,
         "FileCacheId": str,
         "FileCacheType": Literal["LUSTRE"],
         "FileCacheTypeVersion": str,
         "Lifecycle": FileCacheLifecycleType,
-        "FailureDetails": FileCacheFailureDetailsTypeDef,
+        "FailureDetails": FileCacheFailureDetailsOutputTypeDef,
         "StorageCapacity": int,
         "VpcId": str,
         "SubnetIds": List[str],
         "NetworkInterfaceIds": List[str],
         "DNSName": str,
         "KmsKeyId": str,
         "ResourceARN": str,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "CopyTagsToDataRepositoryAssociations": bool,
-        "LustreConfiguration": FileCacheLustreConfigurationTypeDef,
+        "LustreConfiguration": FileCacheLustreConfigurationOutputTypeDef,
         "DataRepositoryAssociationIds": List[str],
     },
 )
 
-FileCacheTypeDef = TypedDict(
-    "FileCacheTypeDef",
+FileCacheOutputTypeDef = TypedDict(
+    "FileCacheOutputTypeDef",
     {
         "OwnerId": str,
         "CreationTime": datetime,
         "FileCacheId": str,
         "FileCacheType": Literal["LUSTRE"],
         "FileCacheTypeVersion": str,
         "Lifecycle": FileCacheLifecycleType,
-        "FailureDetails": FileCacheFailureDetailsTypeDef,
+        "FailureDetails": FileCacheFailureDetailsOutputTypeDef,
         "StorageCapacity": int,
         "VpcId": str,
         "SubnetIds": List[str],
         "NetworkInterfaceIds": List[str],
         "DNSName": str,
         "KmsKeyId": str,
         "ResourceARN": str,
-        "LustreConfiguration": FileCacheLustreConfigurationTypeDef,
+        "LustreConfiguration": FileCacheLustreConfigurationOutputTypeDef,
         "DataRepositoryAssociationIds": List[str],
     },
 )
 
-OntapFileSystemConfigurationTypeDef = TypedDict(
-    "OntapFileSystemConfigurationTypeDef",
+OntapFileSystemConfigurationOutputTypeDef = TypedDict(
+    "OntapFileSystemConfigurationOutputTypeDef",
     {
         "AutomaticBackupRetentionDays": int,
         "DailyAutomaticBackupStartTime": str,
         "DeploymentType": OntapDeploymentTypeType,
         "EndpointIpAddressRange": str,
-        "Endpoints": FileSystemEndpointsTypeDef,
-        "DiskIopsConfiguration": DiskIopsConfigurationTypeDef,
+        "Endpoints": FileSystemEndpointsOutputTypeDef,
+        "DiskIopsConfiguration": DiskIopsConfigurationOutputTypeDef,
         "PreferredSubnetId": str,
         "RouteTableIds": List[str],
         "ThroughputCapacity": int,
         "WeeklyMaintenanceStartTime": str,
         "FsxAdminPassword": str,
     },
 )
 
-CreateSnapshotResponseTypeDef = TypedDict(
-    "CreateSnapshotResponseTypeDef",
+CreateSnapshotResponseOutputTypeDef = TypedDict(
+    "CreateSnapshotResponseOutputTypeDef",
     {
-        "Snapshot": SnapshotTypeDef,
+        "Snapshot": SnapshotOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeSnapshotsResponseTypeDef = TypedDict(
-    "DescribeSnapshotsResponseTypeDef",
+DescribeSnapshotsResponseOutputTypeDef = TypedDict(
+    "DescribeSnapshotsResponseOutputTypeDef",
     {
-        "Snapshots": List[SnapshotTypeDef],
+        "Snapshots": List[SnapshotOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateSnapshotResponseTypeDef = TypedDict(
-    "UpdateSnapshotResponseTypeDef",
+UpdateSnapshotResponseOutputTypeDef = TypedDict(
+    "UpdateSnapshotResponseOutputTypeDef",
     {
-        "Snapshot": SnapshotTypeDef,
+        "Snapshot": SnapshotOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+OpenZFSVolumeConfigurationOutputTypeDef = TypedDict(
+    "OpenZFSVolumeConfigurationOutputTypeDef",
+    {
+        "ParentVolumeId": str,
+        "VolumePath": str,
+        "StorageCapacityReservationGiB": int,
+        "StorageCapacityQuotaGiB": int,
+        "RecordSizeKiB": int,
+        "DataCompressionType": OpenZFSDataCompressionTypeType,
+        "CopyTagsToSnapshots": bool,
+        "OriginSnapshot": OpenZFSOriginSnapshotConfigurationOutputTypeDef,
+        "ReadOnly": bool,
+        "NfsExports": List[OpenZFSNfsExportOutputTypeDef],
+        "UserAndGroupQuotas": List[OpenZFSUserOrGroupQuotaOutputTypeDef],
+        "RestoreToSnapshot": str,
+        "DeleteIntermediateSnaphots": bool,
+        "DeleteClonedVolumes": bool,
+    },
+)
+
 _RequiredCreateOpenZFSVolumeConfigurationTypeDef = TypedDict(
     "_RequiredCreateOpenZFSVolumeConfigurationTypeDef",
     {
         "ParentVolumeId": str,
     },
 )
 _OptionalCreateOpenZFSVolumeConfigurationTypeDef = TypedDict(
@@ -2187,48 +2371,40 @@
         "UserAndGroupQuotas": Sequence[OpenZFSUserOrGroupQuotaTypeDef],
         "CopyTagsToSnapshots": bool,
         "ReadOnly": bool,
     },
     total=False,
 )
 
-OpenZFSVolumeConfigurationTypeDef = TypedDict(
-    "OpenZFSVolumeConfigurationTypeDef",
-    {
-        "ParentVolumeId": str,
-        "VolumePath": str,
-        "StorageCapacityReservationGiB": int,
-        "StorageCapacityQuotaGiB": int,
-        "RecordSizeKiB": int,
-        "DataCompressionType": OpenZFSDataCompressionTypeType,
-        "CopyTagsToSnapshots": bool,
-        "OriginSnapshot": OpenZFSOriginSnapshotConfigurationTypeDef,
-        "ReadOnly": bool,
-        "NfsExports": List[OpenZFSNfsExportTypeDef],
-        "UserAndGroupQuotas": List[OpenZFSUserOrGroupQuotaTypeDef],
-        "RestoreToSnapshot": str,
-        "DeleteIntermediateSnaphots": bool,
-        "DeleteClonedVolumes": bool,
-    },
-)
-
 UpdateOpenZFSVolumeConfigurationTypeDef = TypedDict(
     "UpdateOpenZFSVolumeConfigurationTypeDef",
     {
         "StorageCapacityReservationGiB": int,
         "StorageCapacityQuotaGiB": int,
         "RecordSizeKiB": int,
         "DataCompressionType": OpenZFSDataCompressionTypeType,
         "NfsExports": Sequence[OpenZFSNfsExportTypeDef],
         "UserAndGroupQuotas": Sequence[OpenZFSUserOrGroupQuotaTypeDef],
         "ReadOnly": bool,
     },
     total=False,
 )
 
+SnaplockConfigurationOutputTypeDef = TypedDict(
+    "SnaplockConfigurationOutputTypeDef",
+    {
+        "AuditLogVolume": bool,
+        "AutocommitPeriod": AutocommitPeriodOutputTypeDef,
+        "PrivilegedDelete": PrivilegedDeleteType,
+        "RetentionPeriod": SnaplockRetentionPeriodOutputTypeDef,
+        "SnaplockType": SnaplockTypeType,
+        "VolumeAppendModeEnabled": bool,
+    },
+)
+
 _RequiredCreateSnaplockConfigurationTypeDef = TypedDict(
     "_RequiredCreateSnaplockConfigurationTypeDef",
     {
         "SnaplockType": SnaplockTypeType,
     },
 )
 _OptionalCreateSnaplockConfigurationTypeDef = TypedDict(
@@ -2246,26 +2422,14 @@
 
 class CreateSnaplockConfigurationTypeDef(
     _RequiredCreateSnaplockConfigurationTypeDef, _OptionalCreateSnaplockConfigurationTypeDef
 ):
     pass
 
 
-SnaplockConfigurationTypeDef = TypedDict(
-    "SnaplockConfigurationTypeDef",
-    {
-        "AuditLogVolume": bool,
-        "AutocommitPeriod": AutocommitPeriodTypeDef,
-        "PrivilegedDelete": PrivilegedDeleteType,
-        "RetentionPeriod": SnaplockRetentionPeriodTypeDef,
-        "SnaplockType": SnaplockTypeType,
-        "VolumeAppendModeEnabled": bool,
-    },
-)
-
 UpdateSnaplockConfigurationTypeDef = TypedDict(
     "UpdateSnaplockConfigurationTypeDef",
     {
         "AuditLogVolume": bool,
         "AutocommitPeriod": AutocommitPeriodTypeDef,
         "PrivilegedDelete": PrivilegedDeleteType,
         "RetentionPeriod": SnaplockRetentionPeriodTypeDef,
@@ -2320,107 +2484,107 @@
 class UpdateStorageVirtualMachineRequestRequestTypeDef(
     _RequiredUpdateStorageVirtualMachineRequestRequestTypeDef,
     _OptionalUpdateStorageVirtualMachineRequestRequestTypeDef,
 ):
     pass
 
 
-StorageVirtualMachineTypeDef = TypedDict(
-    "StorageVirtualMachineTypeDef",
+StorageVirtualMachineOutputTypeDef = TypedDict(
+    "StorageVirtualMachineOutputTypeDef",
     {
-        "ActiveDirectoryConfiguration": SvmActiveDirectoryConfigurationTypeDef,
+        "ActiveDirectoryConfiguration": SvmActiveDirectoryConfigurationOutputTypeDef,
         "CreationTime": datetime,
-        "Endpoints": SvmEndpointsTypeDef,
+        "Endpoints": SvmEndpointsOutputTypeDef,
         "FileSystemId": str,
         "Lifecycle": StorageVirtualMachineLifecycleType,
         "Name": str,
         "ResourceARN": str,
         "StorageVirtualMachineId": str,
         "Subtype": StorageVirtualMachineSubtypeType,
         "UUID": str,
-        "Tags": List[TagTypeDef],
-        "LifecycleTransitionReason": LifecycleTransitionReasonTypeDef,
+        "Tags": List[TagOutputTypeDef],
+        "LifecycleTransitionReason": LifecycleTransitionReasonOutputTypeDef,
         "RootVolumeSecurityStyle": StorageVirtualMachineRootVolumeSecurityStyleType,
     },
 )
 
-CreateDataRepositoryAssociationResponseTypeDef = TypedDict(
-    "CreateDataRepositoryAssociationResponseTypeDef",
+CreateDataRepositoryAssociationResponseOutputTypeDef = TypedDict(
+    "CreateDataRepositoryAssociationResponseOutputTypeDef",
     {
-        "Association": DataRepositoryAssociationTypeDef,
+        "Association": DataRepositoryAssociationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeDataRepositoryAssociationsResponseTypeDef = TypedDict(
-    "DescribeDataRepositoryAssociationsResponseTypeDef",
+DescribeDataRepositoryAssociationsResponseOutputTypeDef = TypedDict(
+    "DescribeDataRepositoryAssociationsResponseOutputTypeDef",
     {
-        "Associations": List[DataRepositoryAssociationTypeDef],
+        "Associations": List[DataRepositoryAssociationOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateDataRepositoryAssociationResponseTypeDef = TypedDict(
-    "UpdateDataRepositoryAssociationResponseTypeDef",
+UpdateDataRepositoryAssociationResponseOutputTypeDef = TypedDict(
+    "UpdateDataRepositoryAssociationResponseOutputTypeDef",
     {
-        "Association": DataRepositoryAssociationTypeDef,
+        "Association": DataRepositoryAssociationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateFileCacheResponseTypeDef = TypedDict(
-    "CreateFileCacheResponseTypeDef",
+CreateFileCacheResponseOutputTypeDef = TypedDict(
+    "CreateFileCacheResponseOutputTypeDef",
     {
-        "FileCache": FileCacheCreatingTypeDef,
+        "FileCache": FileCacheCreatingOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeFileCachesResponseTypeDef = TypedDict(
-    "DescribeFileCachesResponseTypeDef",
+DescribeFileCachesResponseOutputTypeDef = TypedDict(
+    "DescribeFileCachesResponseOutputTypeDef",
     {
-        "FileCaches": List[FileCacheTypeDef],
+        "FileCaches": List[FileCacheOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateFileCacheResponseTypeDef = TypedDict(
-    "UpdateFileCacheResponseTypeDef",
+UpdateFileCacheResponseOutputTypeDef = TypedDict(
+    "UpdateFileCacheResponseOutputTypeDef",
     {
-        "FileCache": FileCacheTypeDef,
+        "FileCache": FileCacheOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-FileSystemTypeDef = TypedDict(
-    "FileSystemTypeDef",
+FileSystemOutputTypeDef = TypedDict(
+    "FileSystemOutputTypeDef",
     {
         "OwnerId": str,
         "CreationTime": datetime,
         "FileSystemId": str,
         "FileSystemType": FileSystemTypeType,
         "Lifecycle": FileSystemLifecycleType,
-        "FailureDetails": FileSystemFailureDetailsTypeDef,
+        "FailureDetails": FileSystemFailureDetailsOutputTypeDef,
         "StorageCapacity": int,
         "StorageType": StorageTypeType,
         "VpcId": str,
         "SubnetIds": List[str],
         "NetworkInterfaceIds": List[str],
         "DNSName": str,
         "KmsKeyId": str,
         "ResourceARN": str,
-        "Tags": List[TagTypeDef],
-        "WindowsConfiguration": WindowsFileSystemConfigurationTypeDef,
-        "LustreConfiguration": LustreFileSystemConfigurationTypeDef,
-        "AdministrativeActions": List["AdministrativeActionTypeDef"],
-        "OntapConfiguration": OntapFileSystemConfigurationTypeDef,
+        "Tags": List[TagOutputTypeDef],
+        "WindowsConfiguration": WindowsFileSystemConfigurationOutputTypeDef,
+        "LustreConfiguration": LustreFileSystemConfigurationOutputTypeDef,
+        "AdministrativeActions": List["AdministrativeActionOutputTypeDef"],
+        "OntapConfiguration": OntapFileSystemConfigurationOutputTypeDef,
         "FileSystemTypeVersion": str,
-        "OpenZFSConfiguration": OpenZFSFileSystemConfigurationTypeDef,
+        "OpenZFSConfiguration": OpenZFSFileSystemConfigurationOutputTypeDef,
     },
 )
 
 _RequiredCreateFileSystemOpenZFSConfigurationTypeDef = TypedDict(
     "_RequiredCreateFileSystemOpenZFSConfigurationTypeDef",
     {
         "DeploymentType": OpenZFSDeploymentTypeType,
@@ -2445,14 +2609,33 @@
 class CreateFileSystemOpenZFSConfigurationTypeDef(
     _RequiredCreateFileSystemOpenZFSConfigurationTypeDef,
     _OptionalCreateFileSystemOpenZFSConfigurationTypeDef,
 ):
     pass
 
 
+OntapVolumeConfigurationOutputTypeDef = TypedDict(
+    "OntapVolumeConfigurationOutputTypeDef",
+    {
+        "FlexCacheEndpointType": FlexCacheEndpointTypeType,
+        "JunctionPath": str,
+        "SecurityStyle": SecurityStyleType,
+        "SizeInMegabytes": int,
+        "StorageEfficiencyEnabled": bool,
+        "StorageVirtualMachineId": str,
+        "StorageVirtualMachineRoot": bool,
+        "TieringPolicy": TieringPolicyOutputTypeDef,
+        "UUID": str,
+        "OntapVolumeType": OntapVolumeTypeType,
+        "SnapshotPolicy": str,
+        "CopyTagsToBackups": bool,
+        "SnaplockConfiguration": SnaplockConfigurationOutputTypeDef,
+    },
+)
+
 _RequiredCreateOntapVolumeConfigurationTypeDef = TypedDict(
     "_RequiredCreateOntapVolumeConfigurationTypeDef",
     {
         "SizeInMegabytes": int,
         "StorageVirtualMachineId": str,
     },
 )
@@ -2474,33 +2657,14 @@
 
 class CreateOntapVolumeConfigurationTypeDef(
     _RequiredCreateOntapVolumeConfigurationTypeDef, _OptionalCreateOntapVolumeConfigurationTypeDef
 ):
     pass
 
 
-OntapVolumeConfigurationTypeDef = TypedDict(
-    "OntapVolumeConfigurationTypeDef",
-    {
-        "FlexCacheEndpointType": FlexCacheEndpointTypeType,
-        "JunctionPath": str,
-        "SecurityStyle": SecurityStyleType,
-        "SizeInMegabytes": int,
-        "StorageEfficiencyEnabled": bool,
-        "StorageVirtualMachineId": str,
-        "StorageVirtualMachineRoot": bool,
-        "TieringPolicy": TieringPolicyTypeDef,
-        "UUID": str,
-        "OntapVolumeType": OntapVolumeTypeType,
-        "SnapshotPolicy": str,
-        "CopyTagsToBackups": bool,
-        "SnaplockConfiguration": SnaplockConfigurationTypeDef,
-    },
-)
-
 UpdateOntapVolumeConfigurationTypeDef = TypedDict(
     "UpdateOntapVolumeConfigurationTypeDef",
     {
         "JunctionPath": str,
         "SecurityStyle": SecurityStyleType,
         "SizeInMegabytes": int,
         "StorageEfficiencyEnabled": bool,
@@ -2508,35 +2672,35 @@
         "SnapshotPolicy": str,
         "CopyTagsToBackups": bool,
         "SnaplockConfiguration": UpdateSnaplockConfigurationTypeDef,
     },
     total=False,
 )
 
-CreateStorageVirtualMachineResponseTypeDef = TypedDict(
-    "CreateStorageVirtualMachineResponseTypeDef",
+CreateStorageVirtualMachineResponseOutputTypeDef = TypedDict(
+    "CreateStorageVirtualMachineResponseOutputTypeDef",
     {
-        "StorageVirtualMachine": StorageVirtualMachineTypeDef,
+        "StorageVirtualMachine": StorageVirtualMachineOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeStorageVirtualMachinesResponseTypeDef = TypedDict(
-    "DescribeStorageVirtualMachinesResponseTypeDef",
+DescribeStorageVirtualMachinesResponseOutputTypeDef = TypedDict(
+    "DescribeStorageVirtualMachinesResponseOutputTypeDef",
     {
-        "StorageVirtualMachines": List[StorageVirtualMachineTypeDef],
+        "StorageVirtualMachines": List[StorageVirtualMachineOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateStorageVirtualMachineResponseTypeDef = TypedDict(
-    "UpdateStorageVirtualMachineResponseTypeDef",
+UpdateStorageVirtualMachineResponseOutputTypeDef = TypedDict(
+    "UpdateStorageVirtualMachineResponseOutputTypeDef",
     {
-        "StorageVirtualMachine": StorageVirtualMachineTypeDef,
+        "StorageVirtualMachine": StorageVirtualMachineOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateFileSystemFromBackupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFileSystemFromBackupRequestRequestTypeDef",
     {
@@ -2597,14 +2761,32 @@
 
 class CreateFileSystemRequestRequestTypeDef(
     _RequiredCreateFileSystemRequestRequestTypeDef, _OptionalCreateFileSystemRequestRequestTypeDef
 ):
     pass
 
 
+VolumeOutputTypeDef = TypedDict(
+    "VolumeOutputTypeDef",
+    {
+        "CreationTime": datetime,
+        "FileSystemId": str,
+        "Lifecycle": VolumeLifecycleType,
+        "Name": str,
+        "OntapConfiguration": OntapVolumeConfigurationOutputTypeDef,
+        "ResourceARN": str,
+        "Tags": List[TagOutputTypeDef],
+        "VolumeId": str,
+        "VolumeType": VolumeTypeType,
+        "LifecycleTransitionReason": LifecycleTransitionReasonOutputTypeDef,
+        "AdministrativeActions": List[Dict[str, Any]],
+        "OpenZFSConfiguration": OpenZFSVolumeConfigurationOutputTypeDef,
+    },
+)
+
 _RequiredCreateVolumeFromBackupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVolumeFromBackupRequestRequestTypeDef",
     {
         "BackupId": str,
         "Name": str,
     },
 )
@@ -2647,32 +2829,14 @@
 
 class CreateVolumeRequestRequestTypeDef(
     _RequiredCreateVolumeRequestRequestTypeDef, _OptionalCreateVolumeRequestRequestTypeDef
 ):
     pass
 
 
-VolumeTypeDef = TypedDict(
-    "VolumeTypeDef",
-    {
-        "CreationTime": datetime,
-        "FileSystemId": str,
-        "Lifecycle": VolumeLifecycleType,
-        "Name": str,
-        "OntapConfiguration": OntapVolumeConfigurationTypeDef,
-        "ResourceARN": str,
-        "Tags": List[TagTypeDef],
-        "VolumeId": str,
-        "VolumeType": VolumeTypeType,
-        "LifecycleTransitionReason": LifecycleTransitionReasonTypeDef,
-        "AdministrativeActions": List[Dict[str, Any]],
-        "OpenZFSConfiguration": OpenZFSVolumeConfigurationTypeDef,
-    },
-)
-
 _RequiredUpdateVolumeRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateVolumeRequestRequestTypeDef",
     {
         "VolumeId": str,
     },
 )
 _OptionalUpdateVolumeRequestRequestTypeDef = TypedDict(
@@ -2689,100 +2853,100 @@
 
 class UpdateVolumeRequestRequestTypeDef(
     _RequiredUpdateVolumeRequestRequestTypeDef, _OptionalUpdateVolumeRequestRequestTypeDef
 ):
     pass
 
 
-AdministrativeActionTypeDef = TypedDict(
-    "AdministrativeActionTypeDef",
+AdministrativeActionOutputTypeDef = TypedDict(
+    "AdministrativeActionOutputTypeDef",
     {
         "AdministrativeActionType": AdministrativeActionTypeType,
         "ProgressPercent": int,
         "RequestTime": datetime,
         "Status": StatusType,
         "TargetFileSystemValues": Dict[str, Any],
-        "FailureDetails": AdministrativeActionFailureDetailsTypeDef,
+        "FailureDetails": AdministrativeActionFailureDetailsOutputTypeDef,
         "TargetVolumeValues": Dict[str, Any],
         "TargetSnapshotValues": Dict[str, Any],
     },
 )
 
-BackupTypeDef = TypedDict(
-    "BackupTypeDef",
+BackupOutputTypeDef = TypedDict(
+    "BackupOutputTypeDef",
     {
         "BackupId": str,
         "Lifecycle": BackupLifecycleType,
-        "FailureDetails": BackupFailureDetailsTypeDef,
+        "FailureDetails": BackupFailureDetailsOutputTypeDef,
         "Type": BackupTypeType,
         "ProgressPercent": int,
         "CreationTime": datetime,
         "KmsKeyId": str,
         "ResourceARN": str,
-        "Tags": List[TagTypeDef],
-        "FileSystem": "FileSystemTypeDef",
-        "DirectoryInformation": ActiveDirectoryBackupAttributesTypeDef,
+        "Tags": List[TagOutputTypeDef],
+        "FileSystem": "FileSystemOutputTypeDef",
+        "DirectoryInformation": ActiveDirectoryBackupAttributesOutputTypeDef,
         "OwnerId": str,
         "SourceBackupId": str,
         "SourceBackupRegion": str,
         "ResourceType": ResourceTypeType,
-        "Volume": VolumeTypeDef,
+        "Volume": VolumeOutputTypeDef,
     },
 )
 
-CreateVolumeFromBackupResponseTypeDef = TypedDict(
-    "CreateVolumeFromBackupResponseTypeDef",
+CreateVolumeFromBackupResponseOutputTypeDef = TypedDict(
+    "CreateVolumeFromBackupResponseOutputTypeDef",
     {
-        "Volume": VolumeTypeDef,
+        "Volume": VolumeOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateVolumeResponseTypeDef = TypedDict(
-    "CreateVolumeResponseTypeDef",
+CreateVolumeResponseOutputTypeDef = TypedDict(
+    "CreateVolumeResponseOutputTypeDef",
     {
-        "Volume": VolumeTypeDef,
+        "Volume": VolumeOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeVolumesResponseTypeDef = TypedDict(
-    "DescribeVolumesResponseTypeDef",
+DescribeVolumesResponseOutputTypeDef = TypedDict(
+    "DescribeVolumesResponseOutputTypeDef",
     {
-        "Volumes": List[VolumeTypeDef],
+        "Volumes": List[VolumeOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateVolumeResponseTypeDef = TypedDict(
-    "UpdateVolumeResponseTypeDef",
+UpdateVolumeResponseOutputTypeDef = TypedDict(
+    "UpdateVolumeResponseOutputTypeDef",
     {
-        "Volume": VolumeTypeDef,
+        "Volume": VolumeOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CopyBackupResponseTypeDef = TypedDict(
-    "CopyBackupResponseTypeDef",
+CopyBackupResponseOutputTypeDef = TypedDict(
+    "CopyBackupResponseOutputTypeDef",
     {
-        "Backup": BackupTypeDef,
+        "Backup": BackupOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateBackupResponseTypeDef = TypedDict(
-    "CreateBackupResponseTypeDef",
+CreateBackupResponseOutputTypeDef = TypedDict(
+    "CreateBackupResponseOutputTypeDef",
     {
-        "Backup": BackupTypeDef,
+        "Backup": BackupOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeBackupsResponseTypeDef = TypedDict(
-    "DescribeBackupsResponseTypeDef",
+DescribeBackupsResponseOutputTypeDef = TypedDict(
+    "DescribeBackupsResponseOutputTypeDef",
     {
-        "Backups": List[BackupTypeDef],
+        "Backups": List[BackupOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-fsx-1.28.3/mypy_boto3_fsx/type_defs.pyi` & `mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for fsx service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_fsx.type_defs import ActiveDirectoryBackupAttributesTypeDef
+    from mypy_boto3_fsx.type_defs import ActiveDirectoryBackupAttributesOutputTypeDef
 
-    data: ActiveDirectoryBackupAttributesTypeDef = {...}
+    data: ActiveDirectoryBackupAttributesOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Sequence
 
 from .literals import (
@@ -72,215 +72,230 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "ActiveDirectoryBackupAttributesTypeDef",
-    "AdministrativeActionFailureDetailsTypeDef",
-    "AliasTypeDef",
+    "ActiveDirectoryBackupAttributesOutputTypeDef",
+    "AdministrativeActionFailureDetailsOutputTypeDef",
+    "AliasOutputTypeDef",
     "AssociateFileSystemAliasesRequestRequestTypeDef",
+    "AutoExportPolicyOutputTypeDef",
     "AutoExportPolicyTypeDef",
+    "AutoImportPolicyOutputTypeDef",
     "AutoImportPolicyTypeDef",
+    "AutocommitPeriodOutputTypeDef",
     "AutocommitPeriodTypeDef",
-    "BackupFailureDetailsTypeDef",
-    "TagTypeDef",
+    "BackupFailureDetailsOutputTypeDef",
+    "TagOutputTypeDef",
     "CancelDataRepositoryTaskRequestRequestTypeDef",
-    "CancelDataRepositoryTaskResponseTypeDef",
+    "CancelDataRepositoryTaskResponseOutputTypeDef",
+    "CompletionReportOutputTypeDef",
     "CompletionReportTypeDef",
+    "TagTypeDef",
     "FileCacheLustreMetadataConfigurationTypeDef",
-    "CreateFileSystemFromBackupResponseTypeDef",
+    "CreateFileSystemFromBackupResponseOutputTypeDef",
     "LustreLogCreateConfigurationTypeDef",
     "LustreRootSquashConfigurationTypeDef",
     "DiskIopsConfigurationTypeDef",
-    "CreateFileSystemResponseTypeDef",
+    "CreateFileSystemResponseOutputTypeDef",
     "SelfManagedActiveDirectoryConfigurationTypeDef",
     "WindowsAuditLogCreateConfigurationTypeDef",
     "TieringPolicyTypeDef",
     "CreateOpenZFSOriginSnapshotConfigurationTypeDef",
     "OpenZFSUserOrGroupQuotaTypeDef",
-    "DataRepositoryFailureDetailsTypeDef",
-    "DataRepositoryTaskFailureDetailsTypeDef",
+    "DataRepositoryFailureDetailsOutputTypeDef",
+    "DataRepositoryTaskFailureDetailsOutputTypeDef",
     "DataRepositoryTaskFilterTypeDef",
-    "DataRepositoryTaskStatusTypeDef",
+    "DataRepositoryTaskStatusOutputTypeDef",
     "DeleteBackupRequestRequestTypeDef",
-    "DeleteBackupResponseTypeDef",
+    "DeleteBackupResponseOutputTypeDef",
     "DeleteDataRepositoryAssociationRequestRequestTypeDef",
-    "DeleteDataRepositoryAssociationResponseTypeDef",
+    "DeleteDataRepositoryAssociationResponseOutputTypeDef",
     "DeleteFileCacheRequestRequestTypeDef",
-    "DeleteFileCacheResponseTypeDef",
+    "DeleteFileCacheResponseOutputTypeDef",
     "DeleteSnapshotRequestRequestTypeDef",
-    "DeleteSnapshotResponseTypeDef",
+    "DeleteSnapshotResponseOutputTypeDef",
     "DeleteStorageVirtualMachineRequestRequestTypeDef",
-    "DeleteStorageVirtualMachineResponseTypeDef",
+    "DeleteStorageVirtualMachineResponseOutputTypeDef",
     "DeleteVolumeOpenZFSConfigurationTypeDef",
     "FilterTypeDef",
     "DescribeFileCachesRequestRequestTypeDef",
     "DescribeFileSystemAliasesRequestRequestTypeDef",
     "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
     "DescribeFileSystemsRequestRequestTypeDef",
-    "DescribeFileSystemsResponseTypeDef",
+    "DescribeFileSystemsResponseOutputTypeDef",
     "SnapshotFilterTypeDef",
     "StorageVirtualMachineFilterTypeDef",
     "VolumeFilterTypeDef",
     "DisassociateFileSystemAliasesRequestRequestTypeDef",
-    "FileCacheFailureDetailsTypeDef",
+    "DiskIopsConfigurationOutputTypeDef",
+    "FileCacheFailureDetailsOutputTypeDef",
     "FileCacheNFSConfigurationTypeDef",
-    "LustreLogConfigurationTypeDef",
-    "FileSystemEndpointTypeDef",
-    "FileSystemFailureDetailsTypeDef",
-    "LifecycleTransitionReasonTypeDef",
+    "FileCacheLustreMetadataConfigurationOutputTypeDef",
+    "LustreLogConfigurationOutputTypeDef",
+    "FileSystemEndpointOutputTypeDef",
+    "FileSystemFailureDetailsOutputTypeDef",
+    "LifecycleTransitionReasonOutputTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "LustreRootSquashConfigurationOutputTypeDef",
+    "TieringPolicyOutputTypeDef",
+    "OpenZFSClientConfigurationOutputTypeDef",
     "OpenZFSClientConfigurationTypeDef",
-    "OpenZFSOriginSnapshotConfigurationTypeDef",
+    "OpenZFSOriginSnapshotConfigurationOutputTypeDef",
+    "OpenZFSUserOrGroupQuotaOutputTypeDef",
     "PaginatorConfigTypeDef",
     "ReleaseFileSystemNfsV3LocksRequestRequestTypeDef",
-    "ReleaseFileSystemNfsV3LocksResponseTypeDef",
+    "ReleaseFileSystemNfsV3LocksResponseOutputTypeDef",
     "ResponseMetadataTypeDef",
     "RestoreVolumeFromSnapshotRequestRequestTypeDef",
-    "RestoreVolumeFromSnapshotResponseTypeDef",
+    "RestoreVolumeFromSnapshotResponseOutputTypeDef",
+    "RetentionPeriodOutputTypeDef",
     "RetentionPeriodTypeDef",
-    "SelfManagedActiveDirectoryAttributesTypeDef",
+    "SelfManagedActiveDirectoryAttributesOutputTypeDef",
     "SelfManagedActiveDirectoryConfigurationUpdatesTypeDef",
-    "SvmEndpointTypeDef",
+    "SvmEndpointOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFileCacheLustreConfigurationTypeDef",
-    "UpdateFileSystemResponseTypeDef",
+    "UpdateFileSystemResponseOutputTypeDef",
     "UpdateSnapshotRequestRequestTypeDef",
-    "WindowsAuditLogConfigurationTypeDef",
-    "AssociateFileSystemAliasesResponseTypeDef",
-    "DescribeFileSystemAliasesResponseTypeDef",
-    "DisassociateFileSystemAliasesResponseTypeDef",
-    "NFSDataRepositoryConfigurationTypeDef",
+    "WindowsAuditLogConfigurationOutputTypeDef",
+    "AssociateFileSystemAliasesResponseOutputTypeDef",
+    "DescribeFileSystemAliasesResponseOutputTypeDef",
+    "DisassociateFileSystemAliasesResponseOutputTypeDef",
+    "NFSDataRepositoryConfigurationOutputTypeDef",
+    "S3DataRepositoryConfigurationOutputTypeDef",
     "S3DataRepositoryConfigurationTypeDef",
+    "DeleteFileSystemLustreResponseOutputTypeDef",
+    "DeleteFileSystemOpenZFSResponseOutputTypeDef",
+    "DeleteFileSystemWindowsResponseOutputTypeDef",
+    "DeleteVolumeOntapResponseOutputTypeDef",
+    "ListTagsForResourceResponseOutputTypeDef",
     "CopyBackupRequestRequestTypeDef",
     "CreateBackupRequestRequestTypeDef",
+    "CreateDataRepositoryTaskRequestRequestTypeDef",
     "CreateSnapshotRequestRequestTypeDef",
     "DeleteFileSystemLustreConfigurationTypeDef",
-    "DeleteFileSystemLustreResponseTypeDef",
     "DeleteFileSystemOpenZFSConfigurationTypeDef",
-    "DeleteFileSystemOpenZFSResponseTypeDef",
     "DeleteFileSystemWindowsConfigurationTypeDef",
-    "DeleteFileSystemWindowsResponseTypeDef",
     "DeleteVolumeOntapConfigurationTypeDef",
-    "DeleteVolumeOntapResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "CreateDataRepositoryTaskRequestRequestTypeDef",
     "CreateFileCacheLustreConfigurationTypeDef",
     "CreateFileSystemLustreConfigurationTypeDef",
     "UpdateFileSystemLustreConfigurationTypeDef",
     "CreateFileSystemOntapConfigurationTypeDef",
-    "OpenZFSFileSystemConfigurationTypeDef",
     "UpdateFileSystemOntapConfigurationTypeDef",
     "UpdateFileSystemOpenZFSConfigurationTypeDef",
     "CreateSvmActiveDirectoryConfigurationTypeDef",
     "CreateFileSystemWindowsConfigurationTypeDef",
-    "DataRepositoryConfigurationTypeDef",
+    "DataRepositoryConfigurationOutputTypeDef",
     "DescribeDataRepositoryTasksRequestRequestTypeDef",
-    "DataRepositoryTaskTypeDef",
+    "DataRepositoryTaskOutputTypeDef",
     "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
     "DescribeBackupsRequestRequestTypeDef",
     "DescribeDataRepositoryAssociationsRequestRequestTypeDef",
     "DescribeSnapshotsRequestRequestTypeDef",
     "DescribeStorageVirtualMachinesRequestDescribeStorageVirtualMachinesPaginateTypeDef",
     "DescribeStorageVirtualMachinesRequestRequestTypeDef",
     "DescribeVolumesRequestDescribeVolumesPaginateTypeDef",
     "DescribeVolumesRequestRequestTypeDef",
+    "OpenZFSFileSystemConfigurationOutputTypeDef",
     "FileCacheDataRepositoryAssociationTypeDef",
-    "FileCacheLustreConfigurationTypeDef",
-    "FileSystemEndpointsTypeDef",
-    "SnapshotTypeDef",
+    "FileCacheLustreConfigurationOutputTypeDef",
+    "FileSystemEndpointsOutputTypeDef",
+    "SnapshotOutputTypeDef",
+    "OpenZFSNfsExportOutputTypeDef",
     "OpenZFSNfsExportTypeDef",
+    "SnaplockRetentionPeriodOutputTypeDef",
     "SnaplockRetentionPeriodTypeDef",
-    "SvmActiveDirectoryConfigurationTypeDef",
+    "SvmActiveDirectoryConfigurationOutputTypeDef",
     "UpdateFileSystemWindowsConfigurationTypeDef",
     "UpdateSvmActiveDirectoryConfigurationTypeDef",
-    "SvmEndpointsTypeDef",
+    "SvmEndpointsOutputTypeDef",
     "UpdateFileCacheRequestRequestTypeDef",
-    "WindowsFileSystemConfigurationTypeDef",
+    "WindowsFileSystemConfigurationOutputTypeDef",
+    "DataRepositoryAssociationOutputTypeDef",
     "CreateDataRepositoryAssociationRequestRequestTypeDef",
-    "DataRepositoryAssociationTypeDef",
     "UpdateDataRepositoryAssociationRequestRequestTypeDef",
+    "DeleteFileSystemResponseOutputTypeDef",
+    "DeleteVolumeResponseOutputTypeDef",
     "DeleteFileSystemRequestRequestTypeDef",
-    "DeleteFileSystemResponseTypeDef",
     "DeleteVolumeRequestRequestTypeDef",
-    "DeleteVolumeResponseTypeDef",
     "CreateStorageVirtualMachineRequestRequestTypeDef",
-    "LustreFileSystemConfigurationTypeDef",
-    "CreateDataRepositoryTaskResponseTypeDef",
-    "DescribeDataRepositoryTasksResponseTypeDef",
+    "LustreFileSystemConfigurationOutputTypeDef",
+    "CreateDataRepositoryTaskResponseOutputTypeDef",
+    "DescribeDataRepositoryTasksResponseOutputTypeDef",
     "CreateFileCacheRequestRequestTypeDef",
-    "FileCacheCreatingTypeDef",
-    "FileCacheTypeDef",
-    "OntapFileSystemConfigurationTypeDef",
-    "CreateSnapshotResponseTypeDef",
-    "DescribeSnapshotsResponseTypeDef",
-    "UpdateSnapshotResponseTypeDef",
+    "FileCacheCreatingOutputTypeDef",
+    "FileCacheOutputTypeDef",
+    "OntapFileSystemConfigurationOutputTypeDef",
+    "CreateSnapshotResponseOutputTypeDef",
+    "DescribeSnapshotsResponseOutputTypeDef",
+    "UpdateSnapshotResponseOutputTypeDef",
+    "OpenZFSVolumeConfigurationOutputTypeDef",
     "CreateOpenZFSVolumeConfigurationTypeDef",
     "OpenZFSCreateRootVolumeConfigurationTypeDef",
-    "OpenZFSVolumeConfigurationTypeDef",
     "UpdateOpenZFSVolumeConfigurationTypeDef",
+    "SnaplockConfigurationOutputTypeDef",
     "CreateSnaplockConfigurationTypeDef",
-    "SnaplockConfigurationTypeDef",
     "UpdateSnaplockConfigurationTypeDef",
     "UpdateFileSystemRequestRequestTypeDef",
     "UpdateStorageVirtualMachineRequestRequestTypeDef",
-    "StorageVirtualMachineTypeDef",
-    "CreateDataRepositoryAssociationResponseTypeDef",
-    "DescribeDataRepositoryAssociationsResponseTypeDef",
-    "UpdateDataRepositoryAssociationResponseTypeDef",
-    "CreateFileCacheResponseTypeDef",
-    "DescribeFileCachesResponseTypeDef",
-    "UpdateFileCacheResponseTypeDef",
-    "FileSystemTypeDef",
+    "StorageVirtualMachineOutputTypeDef",
+    "CreateDataRepositoryAssociationResponseOutputTypeDef",
+    "DescribeDataRepositoryAssociationsResponseOutputTypeDef",
+    "UpdateDataRepositoryAssociationResponseOutputTypeDef",
+    "CreateFileCacheResponseOutputTypeDef",
+    "DescribeFileCachesResponseOutputTypeDef",
+    "UpdateFileCacheResponseOutputTypeDef",
+    "FileSystemOutputTypeDef",
     "CreateFileSystemOpenZFSConfigurationTypeDef",
+    "OntapVolumeConfigurationOutputTypeDef",
     "CreateOntapVolumeConfigurationTypeDef",
-    "OntapVolumeConfigurationTypeDef",
     "UpdateOntapVolumeConfigurationTypeDef",
-    "CreateStorageVirtualMachineResponseTypeDef",
-    "DescribeStorageVirtualMachinesResponseTypeDef",
-    "UpdateStorageVirtualMachineResponseTypeDef",
+    "CreateStorageVirtualMachineResponseOutputTypeDef",
+    "DescribeStorageVirtualMachinesResponseOutputTypeDef",
+    "UpdateStorageVirtualMachineResponseOutputTypeDef",
     "CreateFileSystemFromBackupRequestRequestTypeDef",
     "CreateFileSystemRequestRequestTypeDef",
+    "VolumeOutputTypeDef",
     "CreateVolumeFromBackupRequestRequestTypeDef",
     "CreateVolumeRequestRequestTypeDef",
-    "VolumeTypeDef",
     "UpdateVolumeRequestRequestTypeDef",
-    "AdministrativeActionTypeDef",
-    "BackupTypeDef",
-    "CreateVolumeFromBackupResponseTypeDef",
-    "CreateVolumeResponseTypeDef",
-    "DescribeVolumesResponseTypeDef",
-    "UpdateVolumeResponseTypeDef",
-    "CopyBackupResponseTypeDef",
-    "CreateBackupResponseTypeDef",
-    "DescribeBackupsResponseTypeDef",
+    "AdministrativeActionOutputTypeDef",
+    "BackupOutputTypeDef",
+    "CreateVolumeFromBackupResponseOutputTypeDef",
+    "CreateVolumeResponseOutputTypeDef",
+    "DescribeVolumesResponseOutputTypeDef",
+    "UpdateVolumeResponseOutputTypeDef",
+    "CopyBackupResponseOutputTypeDef",
+    "CreateBackupResponseOutputTypeDef",
+    "DescribeBackupsResponseOutputTypeDef",
 )
 
-ActiveDirectoryBackupAttributesTypeDef = TypedDict(
-    "ActiveDirectoryBackupAttributesTypeDef",
+ActiveDirectoryBackupAttributesOutputTypeDef = TypedDict(
+    "ActiveDirectoryBackupAttributesOutputTypeDef",
     {
         "DomainName": str,
         "ActiveDirectoryId": str,
         "ResourceARN": str,
     },
 )
 
-AdministrativeActionFailureDetailsTypeDef = TypedDict(
-    "AdministrativeActionFailureDetailsTypeDef",
+AdministrativeActionFailureDetailsOutputTypeDef = TypedDict(
+    "AdministrativeActionFailureDetailsOutputTypeDef",
     {
         "Message": str,
     },
 )
 
-AliasTypeDef = TypedDict(
-    "AliasTypeDef",
+AliasOutputTypeDef = TypedDict(
+    "AliasOutputTypeDef",
     {
         "Name": str,
         "Lifecycle": AliasLifecycleType,
     },
 )
 
 _RequiredAssociateFileSystemAliasesRequestRequestTypeDef = TypedDict(
@@ -300,69 +315,110 @@
 
 class AssociateFileSystemAliasesRequestRequestTypeDef(
     _RequiredAssociateFileSystemAliasesRequestRequestTypeDef,
     _OptionalAssociateFileSystemAliasesRequestRequestTypeDef,
 ):
     pass
 
+AutoExportPolicyOutputTypeDef = TypedDict(
+    "AutoExportPolicyOutputTypeDef",
+    {
+        "Events": List[EventTypeType],
+    },
+)
+
 AutoExportPolicyTypeDef = TypedDict(
     "AutoExportPolicyTypeDef",
     {
         "Events": Sequence[EventTypeType],
     },
     total=False,
 )
 
+AutoImportPolicyOutputTypeDef = TypedDict(
+    "AutoImportPolicyOutputTypeDef",
+    {
+        "Events": List[EventTypeType],
+    },
+)
+
 AutoImportPolicyTypeDef = TypedDict(
     "AutoImportPolicyTypeDef",
     {
         "Events": Sequence[EventTypeType],
     },
     total=False,
 )
 
-AutocommitPeriodTypeDef = TypedDict(
-    "AutocommitPeriodTypeDef",
+AutocommitPeriodOutputTypeDef = TypedDict(
+    "AutocommitPeriodOutputTypeDef",
     {
         "Type": AutocommitPeriodTypeType,
         "Value": int,
     },
 )
 
-BackupFailureDetailsTypeDef = TypedDict(
-    "BackupFailureDetailsTypeDef",
+_RequiredAutocommitPeriodTypeDef = TypedDict(
+    "_RequiredAutocommitPeriodTypeDef",
+    {
+        "Type": AutocommitPeriodTypeType,
+    },
+)
+_OptionalAutocommitPeriodTypeDef = TypedDict(
+    "_OptionalAutocommitPeriodTypeDef",
+    {
+        "Value": int,
+    },
+    total=False,
+)
+
+class AutocommitPeriodTypeDef(_RequiredAutocommitPeriodTypeDef, _OptionalAutocommitPeriodTypeDef):
+    pass
+
+BackupFailureDetailsOutputTypeDef = TypedDict(
+    "BackupFailureDetailsOutputTypeDef",
     {
         "Message": str,
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
 CancelDataRepositoryTaskRequestRequestTypeDef = TypedDict(
     "CancelDataRepositoryTaskRequestRequestTypeDef",
     {
         "TaskId": str,
     },
 )
 
-CancelDataRepositoryTaskResponseTypeDef = TypedDict(
-    "CancelDataRepositoryTaskResponseTypeDef",
+CancelDataRepositoryTaskResponseOutputTypeDef = TypedDict(
+    "CancelDataRepositoryTaskResponseOutputTypeDef",
     {
         "Lifecycle": DataRepositoryTaskLifecycleType,
         "TaskId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CompletionReportOutputTypeDef = TypedDict(
+    "CompletionReportOutputTypeDef",
+    {
+        "Enabled": bool,
+        "Path": str,
+        "Format": Literal["REPORT_CSV_20191124"],
+        "Scope": Literal["FAILED_FILES_ONLY"],
+    },
+)
+
 _RequiredCompletionReportTypeDef = TypedDict(
     "_RequiredCompletionReportTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalCompletionReportTypeDef = TypedDict(
@@ -374,25 +430,33 @@
     },
     total=False,
 )
 
 class CompletionReportTypeDef(_RequiredCompletionReportTypeDef, _OptionalCompletionReportTypeDef):
     pass
 
+TagTypeDef = TypedDict(
+    "TagTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 FileCacheLustreMetadataConfigurationTypeDef = TypedDict(
     "FileCacheLustreMetadataConfigurationTypeDef",
     {
         "StorageCapacity": int,
     },
 )
 
-CreateFileSystemFromBackupResponseTypeDef = TypedDict(
-    "CreateFileSystemFromBackupResponseTypeDef",
+CreateFileSystemFromBackupResponseOutputTypeDef = TypedDict(
+    "CreateFileSystemFromBackupResponseOutputTypeDef",
     {
-        "FileSystem": "FileSystemTypeDef",
+        "FileSystem": "FileSystemOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredLustreLogCreateConfigurationTypeDef = TypedDict(
     "_RequiredLustreLogCreateConfigurationTypeDef",
     {
@@ -412,30 +476,32 @@
 ):
     pass
 
 LustreRootSquashConfigurationTypeDef = TypedDict(
     "LustreRootSquashConfigurationTypeDef",
     {
         "RootSquash": str,
-        "NoSquashNids": List[str],
+        "NoSquashNids": Sequence[str],
     },
+    total=False,
 )
 
 DiskIopsConfigurationTypeDef = TypedDict(
     "DiskIopsConfigurationTypeDef",
     {
         "Mode": DiskIopsConfigurationModeType,
         "Iops": int,
     },
+    total=False,
 )
 
-CreateFileSystemResponseTypeDef = TypedDict(
-    "CreateFileSystemResponseTypeDef",
+CreateFileSystemResponseOutputTypeDef = TypedDict(
+    "CreateFileSystemResponseOutputTypeDef",
     {
-        "FileSystem": "FileSystemTypeDef",
+        "FileSystem": "FileSystemOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSelfManagedActiveDirectoryConfigurationTypeDef = TypedDict(
     "_RequiredSelfManagedActiveDirectoryConfigurationTypeDef",
     {
@@ -483,14 +549,15 @@
 
 TieringPolicyTypeDef = TypedDict(
     "TieringPolicyTypeDef",
     {
         "CoolingPeriod": int,
         "Name": TieringPolicyNameType,
     },
+    total=False,
 )
 
 CreateOpenZFSOriginSnapshotConfigurationTypeDef = TypedDict(
     "CreateOpenZFSOriginSnapshotConfigurationTypeDef",
     {
         "SnapshotARN": str,
         "CopyStrategy": OpenZFSCopyStrategyType,
@@ -502,39 +569,39 @@
     {
         "Type": OpenZFSQuotaTypeType,
         "Id": int,
         "StorageCapacityQuotaGiB": int,
     },
 )
 
-DataRepositoryFailureDetailsTypeDef = TypedDict(
-    "DataRepositoryFailureDetailsTypeDef",
+DataRepositoryFailureDetailsOutputTypeDef = TypedDict(
+    "DataRepositoryFailureDetailsOutputTypeDef",
     {
         "Message": str,
     },
 )
 
-DataRepositoryTaskFailureDetailsTypeDef = TypedDict(
-    "DataRepositoryTaskFailureDetailsTypeDef",
+DataRepositoryTaskFailureDetailsOutputTypeDef = TypedDict(
+    "DataRepositoryTaskFailureDetailsOutputTypeDef",
     {
         "Message": str,
     },
 )
 
 DataRepositoryTaskFilterTypeDef = TypedDict(
     "DataRepositoryTaskFilterTypeDef",
     {
         "Name": DataRepositoryTaskFilterNameType,
         "Values": Sequence[str],
     },
     total=False,
 )
 
-DataRepositoryTaskStatusTypeDef = TypedDict(
-    "DataRepositoryTaskStatusTypeDef",
+DataRepositoryTaskStatusOutputTypeDef = TypedDict(
+    "DataRepositoryTaskStatusOutputTypeDef",
     {
         "TotalCount": int,
         "SucceededCount": int,
         "FailedCount": int,
         "LastUpdatedTime": datetime,
         "ReleasedCapacity": int,
     },
@@ -555,16 +622,16 @@
 )
 
 class DeleteBackupRequestRequestTypeDef(
     _RequiredDeleteBackupRequestRequestTypeDef, _OptionalDeleteBackupRequestRequestTypeDef
 ):
     pass
 
-DeleteBackupResponseTypeDef = TypedDict(
-    "DeleteBackupResponseTypeDef",
+DeleteBackupResponseOutputTypeDef = TypedDict(
+    "DeleteBackupResponseOutputTypeDef",
     {
         "BackupId": str,
         "Lifecycle": BackupLifecycleType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -585,16 +652,16 @@
 
 class DeleteDataRepositoryAssociationRequestRequestTypeDef(
     _RequiredDeleteDataRepositoryAssociationRequestRequestTypeDef,
     _OptionalDeleteDataRepositoryAssociationRequestRequestTypeDef,
 ):
     pass
 
-DeleteDataRepositoryAssociationResponseTypeDef = TypedDict(
-    "DeleteDataRepositoryAssociationResponseTypeDef",
+DeleteDataRepositoryAssociationResponseOutputTypeDef = TypedDict(
+    "DeleteDataRepositoryAssociationResponseOutputTypeDef",
     {
         "AssociationId": str,
         "Lifecycle": DataRepositoryLifecycleType,
         "DeleteDataInFileSystem": bool,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -614,16 +681,16 @@
 )
 
 class DeleteFileCacheRequestRequestTypeDef(
     _RequiredDeleteFileCacheRequestRequestTypeDef, _OptionalDeleteFileCacheRequestRequestTypeDef
 ):
     pass
 
-DeleteFileCacheResponseTypeDef = TypedDict(
-    "DeleteFileCacheResponseTypeDef",
+DeleteFileCacheResponseOutputTypeDef = TypedDict(
+    "DeleteFileCacheResponseOutputTypeDef",
     {
         "FileCacheId": str,
         "Lifecycle": FileCacheLifecycleType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -642,16 +709,16 @@
 )
 
 class DeleteSnapshotRequestRequestTypeDef(
     _RequiredDeleteSnapshotRequestRequestTypeDef, _OptionalDeleteSnapshotRequestRequestTypeDef
 ):
     pass
 
-DeleteSnapshotResponseTypeDef = TypedDict(
-    "DeleteSnapshotResponseTypeDef",
+DeleteSnapshotResponseOutputTypeDef = TypedDict(
+    "DeleteSnapshotResponseOutputTypeDef",
     {
         "SnapshotId": str,
         "Lifecycle": SnapshotLifecycleType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -671,16 +738,16 @@
 
 class DeleteStorageVirtualMachineRequestRequestTypeDef(
     _RequiredDeleteStorageVirtualMachineRequestRequestTypeDef,
     _OptionalDeleteStorageVirtualMachineRequestRequestTypeDef,
 ):
     pass
 
-DeleteStorageVirtualMachineResponseTypeDef = TypedDict(
-    "DeleteStorageVirtualMachineResponseTypeDef",
+DeleteStorageVirtualMachineResponseOutputTypeDef = TypedDict(
+    "DeleteStorageVirtualMachineResponseOutputTypeDef",
     {
         "StorageVirtualMachineId": str,
         "Lifecycle": StorageVirtualMachineLifecycleType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -748,18 +815,18 @@
         "FileSystemIds": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeFileSystemsResponseTypeDef = TypedDict(
-    "DescribeFileSystemsResponseTypeDef",
+DescribeFileSystemsResponseOutputTypeDef = TypedDict(
+    "DescribeFileSystemsResponseOutputTypeDef",
     {
-        "FileSystems": List["FileSystemTypeDef"],
+        "FileSystems": List["FileSystemOutputTypeDef"],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SnapshotFilterTypeDef = TypedDict(
     "SnapshotFilterTypeDef",
@@ -805,16 +872,24 @@
 
 class DisassociateFileSystemAliasesRequestRequestTypeDef(
     _RequiredDisassociateFileSystemAliasesRequestRequestTypeDef,
     _OptionalDisassociateFileSystemAliasesRequestRequestTypeDef,
 ):
     pass
 
-FileCacheFailureDetailsTypeDef = TypedDict(
-    "FileCacheFailureDetailsTypeDef",
+DiskIopsConfigurationOutputTypeDef = TypedDict(
+    "DiskIopsConfigurationOutputTypeDef",
+    {
+        "Mode": DiskIopsConfigurationModeType,
+        "Iops": int,
+    },
+)
+
+FileCacheFailureDetailsOutputTypeDef = TypedDict(
+    "FileCacheFailureDetailsOutputTypeDef",
     {
         "Message": str,
     },
 )
 
 _RequiredFileCacheNFSConfigurationTypeDef = TypedDict(
     "_RequiredFileCacheNFSConfigurationTypeDef",
@@ -831,39 +906,46 @@
 )
 
 class FileCacheNFSConfigurationTypeDef(
     _RequiredFileCacheNFSConfigurationTypeDef, _OptionalFileCacheNFSConfigurationTypeDef
 ):
     pass
 
-LustreLogConfigurationTypeDef = TypedDict(
-    "LustreLogConfigurationTypeDef",
+FileCacheLustreMetadataConfigurationOutputTypeDef = TypedDict(
+    "FileCacheLustreMetadataConfigurationOutputTypeDef",
+    {
+        "StorageCapacity": int,
+    },
+)
+
+LustreLogConfigurationOutputTypeDef = TypedDict(
+    "LustreLogConfigurationOutputTypeDef",
     {
         "Level": LustreAccessAuditLogLevelType,
         "Destination": str,
     },
 )
 
-FileSystemEndpointTypeDef = TypedDict(
-    "FileSystemEndpointTypeDef",
+FileSystemEndpointOutputTypeDef = TypedDict(
+    "FileSystemEndpointOutputTypeDef",
     {
         "DNSName": str,
         "IpAddresses": List[str],
     },
 )
 
-FileSystemFailureDetailsTypeDef = TypedDict(
-    "FileSystemFailureDetailsTypeDef",
+FileSystemFailureDetailsOutputTypeDef = TypedDict(
+    "FileSystemFailureDetailsOutputTypeDef",
     {
         "Message": str,
     },
 )
 
-LifecycleTransitionReasonTypeDef = TypedDict(
-    "LifecycleTransitionReasonTypeDef",
+LifecycleTransitionReasonOutputTypeDef = TypedDict(
+    "LifecycleTransitionReasonOutputTypeDef",
     {
         "Message": str,
     },
 )
 
 _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
@@ -902,30 +984,63 @@
 
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
+LustreRootSquashConfigurationOutputTypeDef = TypedDict(
+    "LustreRootSquashConfigurationOutputTypeDef",
+    {
+        "RootSquash": str,
+        "NoSquashNids": List[str],
+    },
+)
+
+TieringPolicyOutputTypeDef = TypedDict(
+    "TieringPolicyOutputTypeDef",
+    {
+        "CoolingPeriod": int,
+        "Name": TieringPolicyNameType,
+    },
+)
+
+OpenZFSClientConfigurationOutputTypeDef = TypedDict(
+    "OpenZFSClientConfigurationOutputTypeDef",
+    {
+        "Clients": str,
+        "Options": List[str],
+    },
+)
+
 OpenZFSClientConfigurationTypeDef = TypedDict(
     "OpenZFSClientConfigurationTypeDef",
     {
         "Clients": str,
-        "Options": List[str],
+        "Options": Sequence[str],
     },
 )
 
-OpenZFSOriginSnapshotConfigurationTypeDef = TypedDict(
-    "OpenZFSOriginSnapshotConfigurationTypeDef",
+OpenZFSOriginSnapshotConfigurationOutputTypeDef = TypedDict(
+    "OpenZFSOriginSnapshotConfigurationOutputTypeDef",
     {
         "SnapshotARN": str,
         "CopyStrategy": OpenZFSCopyStrategyType,
     },
 )
 
+OpenZFSUserOrGroupQuotaOutputTypeDef = TypedDict(
+    "OpenZFSUserOrGroupQuotaOutputTypeDef",
+    {
+        "Type": OpenZFSQuotaTypeType,
+        "Id": int,
+        "StorageCapacityQuotaGiB": int,
+    },
+)
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -948,18 +1063,18 @@
 
 class ReleaseFileSystemNfsV3LocksRequestRequestTypeDef(
     _RequiredReleaseFileSystemNfsV3LocksRequestRequestTypeDef,
     _OptionalReleaseFileSystemNfsV3LocksRequestRequestTypeDef,
 ):
     pass
 
-ReleaseFileSystemNfsV3LocksResponseTypeDef = TypedDict(
-    "ReleaseFileSystemNfsV3LocksResponseTypeDef",
+ReleaseFileSystemNfsV3LocksResponseOutputTypeDef = TypedDict(
+    "ReleaseFileSystemNfsV3LocksResponseOutputTypeDef",
     {
-        "FileSystem": "FileSystemTypeDef",
+        "FileSystem": "FileSystemOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
@@ -989,34 +1104,51 @@
 
 class RestoreVolumeFromSnapshotRequestRequestTypeDef(
     _RequiredRestoreVolumeFromSnapshotRequestRequestTypeDef,
     _OptionalRestoreVolumeFromSnapshotRequestRequestTypeDef,
 ):
     pass
 
-RestoreVolumeFromSnapshotResponseTypeDef = TypedDict(
-    "RestoreVolumeFromSnapshotResponseTypeDef",
+RestoreVolumeFromSnapshotResponseOutputTypeDef = TypedDict(
+    "RestoreVolumeFromSnapshotResponseOutputTypeDef",
     {
         "VolumeId": str,
         "Lifecycle": VolumeLifecycleType,
-        "AdministrativeActions": List["AdministrativeActionTypeDef"],
+        "AdministrativeActions": List["AdministrativeActionOutputTypeDef"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RetentionPeriodTypeDef = TypedDict(
-    "RetentionPeriodTypeDef",
+RetentionPeriodOutputTypeDef = TypedDict(
+    "RetentionPeriodOutputTypeDef",
     {
         "Type": RetentionPeriodTypeType,
         "Value": int,
     },
 )
 
-SelfManagedActiveDirectoryAttributesTypeDef = TypedDict(
-    "SelfManagedActiveDirectoryAttributesTypeDef",
+_RequiredRetentionPeriodTypeDef = TypedDict(
+    "_RequiredRetentionPeriodTypeDef",
+    {
+        "Type": RetentionPeriodTypeType,
+    },
+)
+_OptionalRetentionPeriodTypeDef = TypedDict(
+    "_OptionalRetentionPeriodTypeDef",
+    {
+        "Value": int,
+    },
+    total=False,
+)
+
+class RetentionPeriodTypeDef(_RequiredRetentionPeriodTypeDef, _OptionalRetentionPeriodTypeDef):
+    pass
+
+SelfManagedActiveDirectoryAttributesOutputTypeDef = TypedDict(
+    "SelfManagedActiveDirectoryAttributesOutputTypeDef",
     {
         "DomainName": str,
         "OrganizationalUnitDistinguishedName": str,
         "FileSystemAdministratorsGroup": str,
         "UserName": str,
         "DnsIps": List[str],
     },
@@ -1031,16 +1163,16 @@
         "DomainName": str,
         "OrganizationalUnitDistinguishedName": str,
         "FileSystemAdministratorsGroup": str,
     },
     total=False,
 )
 
-SvmEndpointTypeDef = TypedDict(
-    "SvmEndpointTypeDef",
+SvmEndpointOutputTypeDef = TypedDict(
+    "SvmEndpointOutputTypeDef",
     {
         "DNSName": str,
         "IpAddresses": List[str],
     },
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
@@ -1055,18 +1187,18 @@
     "UpdateFileCacheLustreConfigurationTypeDef",
     {
         "WeeklyMaintenanceStartTime": str,
     },
     total=False,
 )
 
-UpdateFileSystemResponseTypeDef = TypedDict(
-    "UpdateFileSystemResponseTypeDef",
+UpdateFileSystemResponseOutputTypeDef = TypedDict(
+    "UpdateFileSystemResponseOutputTypeDef",
     {
-        "FileSystem": "FileSystemTypeDef",
+        "FileSystem": "FileSystemOutputTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSnapshotRequestRequestTypeDef",
     {
@@ -1083,66 +1215,115 @@
 )
 
 class UpdateSnapshotRequestRequestTypeDef(
     _RequiredUpdateSnapshotRequestRequestTypeDef, _OptionalUpdateSnapshotRequestRequestTypeDef
 ):
     pass
 
-WindowsAuditLogConfigurationTypeDef = TypedDict(
-    "WindowsAuditLogConfigurationTypeDef",
+WindowsAuditLogConfigurationOutputTypeDef = TypedDict(
+    "WindowsAuditLogConfigurationOutputTypeDef",
     {
         "FileAccessAuditLogLevel": WindowsAccessAuditLogLevelType,
         "FileShareAccessAuditLogLevel": WindowsAccessAuditLogLevelType,
         "AuditLogDestination": str,
     },
 )
 
-AssociateFileSystemAliasesResponseTypeDef = TypedDict(
-    "AssociateFileSystemAliasesResponseTypeDef",
+AssociateFileSystemAliasesResponseOutputTypeDef = TypedDict(
+    "AssociateFileSystemAliasesResponseOutputTypeDef",
     {
-        "Aliases": List[AliasTypeDef],
+        "Aliases": List[AliasOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeFileSystemAliasesResponseTypeDef = TypedDict(
-    "DescribeFileSystemAliasesResponseTypeDef",
+DescribeFileSystemAliasesResponseOutputTypeDef = TypedDict(
+    "DescribeFileSystemAliasesResponseOutputTypeDef",
     {
-        "Aliases": List[AliasTypeDef],
+        "Aliases": List[AliasOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DisassociateFileSystemAliasesResponseTypeDef = TypedDict(
-    "DisassociateFileSystemAliasesResponseTypeDef",
+DisassociateFileSystemAliasesResponseOutputTypeDef = TypedDict(
+    "DisassociateFileSystemAliasesResponseOutputTypeDef",
     {
-        "Aliases": List[AliasTypeDef],
+        "Aliases": List[AliasOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-NFSDataRepositoryConfigurationTypeDef = TypedDict(
-    "NFSDataRepositoryConfigurationTypeDef",
+NFSDataRepositoryConfigurationOutputTypeDef = TypedDict(
+    "NFSDataRepositoryConfigurationOutputTypeDef",
     {
         "Version": Literal["NFS3"],
         "DnsIps": List[str],
-        "AutoExportPolicy": AutoExportPolicyTypeDef,
+        "AutoExportPolicy": AutoExportPolicyOutputTypeDef,
+    },
+)
+
+S3DataRepositoryConfigurationOutputTypeDef = TypedDict(
+    "S3DataRepositoryConfigurationOutputTypeDef",
+    {
+        "AutoImportPolicy": AutoImportPolicyOutputTypeDef,
+        "AutoExportPolicy": AutoExportPolicyOutputTypeDef,
     },
 )
 
 S3DataRepositoryConfigurationTypeDef = TypedDict(
     "S3DataRepositoryConfigurationTypeDef",
     {
         "AutoImportPolicy": AutoImportPolicyTypeDef,
         "AutoExportPolicy": AutoExportPolicyTypeDef,
     },
     total=False,
 )
 
+DeleteFileSystemLustreResponseOutputTypeDef = TypedDict(
+    "DeleteFileSystemLustreResponseOutputTypeDef",
+    {
+        "FinalBackupId": str,
+        "FinalBackupTags": List[TagOutputTypeDef],
+    },
+)
+
+DeleteFileSystemOpenZFSResponseOutputTypeDef = TypedDict(
+    "DeleteFileSystemOpenZFSResponseOutputTypeDef",
+    {
+        "FinalBackupId": str,
+        "FinalBackupTags": List[TagOutputTypeDef],
+    },
+)
+
+DeleteFileSystemWindowsResponseOutputTypeDef = TypedDict(
+    "DeleteFileSystemWindowsResponseOutputTypeDef",
+    {
+        "FinalBackupId": str,
+        "FinalBackupTags": List[TagOutputTypeDef],
+    },
+)
+
+DeleteVolumeOntapResponseOutputTypeDef = TypedDict(
+    "DeleteVolumeOntapResponseOutputTypeDef",
+    {
+        "FinalBackupId": str,
+        "FinalBackupTags": List[TagOutputTypeDef],
+    },
+)
+
+ListTagsForResourceResponseOutputTypeDef = TypedDict(
+    "ListTagsForResourceResponseOutputTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCopyBackupRequestRequestTypeDef = TypedDict(
     "_RequiredCopyBackupRequestRequestTypeDef",
     {
         "SourceBackupId": str,
     },
 )
 _OptionalCopyBackupRequestRequestTypeDef = TypedDict(
@@ -1169,14 +1350,39 @@
         "ClientRequestToken": str,
         "Tags": Sequence[TagTypeDef],
         "VolumeId": str,
     },
     total=False,
 )
 
+_RequiredCreateDataRepositoryTaskRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDataRepositoryTaskRequestRequestTypeDef",
+    {
+        "Type": DataRepositoryTaskTypeType,
+        "FileSystemId": str,
+        "Report": CompletionReportTypeDef,
+    },
+)
+_OptionalCreateDataRepositoryTaskRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDataRepositoryTaskRequestRequestTypeDef",
+    {
+        "Paths": Sequence[str],
+        "ClientRequestToken": str,
+        "Tags": Sequence[TagTypeDef],
+        "CapacityToRelease": int,
+    },
+    total=False,
+)
+
+class CreateDataRepositoryTaskRequestRequestTypeDef(
+    _RequiredCreateDataRepositoryTaskRequestRequestTypeDef,
+    _OptionalCreateDataRepositoryTaskRequestRequestTypeDef,
+):
+    pass
+
 _RequiredCreateSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSnapshotRequestRequestTypeDef",
     {
         "Name": str,
         "VolumeId": str,
     },
 )
@@ -1199,117 +1405,51 @@
     {
         "SkipFinalBackup": bool,
         "FinalBackupTags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-DeleteFileSystemLustreResponseTypeDef = TypedDict(
-    "DeleteFileSystemLustreResponseTypeDef",
-    {
-        "FinalBackupId": str,
-        "FinalBackupTags": List[TagTypeDef],
-    },
-)
-
 DeleteFileSystemOpenZFSConfigurationTypeDef = TypedDict(
     "DeleteFileSystemOpenZFSConfigurationTypeDef",
     {
         "SkipFinalBackup": bool,
         "FinalBackupTags": Sequence[TagTypeDef],
         "Options": Sequence[Literal["DELETE_CHILD_VOLUMES_AND_SNAPSHOTS"]],
     },
     total=False,
 )
 
-DeleteFileSystemOpenZFSResponseTypeDef = TypedDict(
-    "DeleteFileSystemOpenZFSResponseTypeDef",
-    {
-        "FinalBackupId": str,
-        "FinalBackupTags": List[TagTypeDef],
-    },
-)
-
 DeleteFileSystemWindowsConfigurationTypeDef = TypedDict(
     "DeleteFileSystemWindowsConfigurationTypeDef",
     {
         "SkipFinalBackup": bool,
         "FinalBackupTags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-DeleteFileSystemWindowsResponseTypeDef = TypedDict(
-    "DeleteFileSystemWindowsResponseTypeDef",
-    {
-        "FinalBackupId": str,
-        "FinalBackupTags": List[TagTypeDef],
-    },
-)
-
 DeleteVolumeOntapConfigurationTypeDef = TypedDict(
     "DeleteVolumeOntapConfigurationTypeDef",
     {
         "SkipFinalBackup": bool,
         "FinalBackupTags": Sequence[TagTypeDef],
         "BypassSnaplockEnterpriseRetention": bool,
     },
     total=False,
 )
 
-DeleteVolumeOntapResponseTypeDef = TypedDict(
-    "DeleteVolumeOntapResponseTypeDef",
-    {
-        "FinalBackupId": str,
-        "FinalBackupTags": List[TagTypeDef],
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-_RequiredCreateDataRepositoryTaskRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDataRepositoryTaskRequestRequestTypeDef",
-    {
-        "Type": DataRepositoryTaskTypeType,
-        "FileSystemId": str,
-        "Report": CompletionReportTypeDef,
-    },
-)
-_OptionalCreateDataRepositoryTaskRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDataRepositoryTaskRequestRequestTypeDef",
-    {
-        "Paths": Sequence[str],
-        "ClientRequestToken": str,
-        "Tags": Sequence[TagTypeDef],
-        "CapacityToRelease": int,
-    },
-    total=False,
-)
-
-class CreateDataRepositoryTaskRequestRequestTypeDef(
-    _RequiredCreateDataRepositoryTaskRequestRequestTypeDef,
-    _OptionalCreateDataRepositoryTaskRequestRequestTypeDef,
-):
-    pass
-
 _RequiredCreateFileCacheLustreConfigurationTypeDef = TypedDict(
     "_RequiredCreateFileCacheLustreConfigurationTypeDef",
     {
         "PerUnitStorageThroughput": int,
         "DeploymentType": Literal["CACHE_1"],
         "MetadataConfiguration": FileCacheLustreMetadataConfigurationTypeDef,
     },
@@ -1387,29 +1527,14 @@
 
 class CreateFileSystemOntapConfigurationTypeDef(
     _RequiredCreateFileSystemOntapConfigurationTypeDef,
     _OptionalCreateFileSystemOntapConfigurationTypeDef,
 ):
     pass
 
-OpenZFSFileSystemConfigurationTypeDef = TypedDict(
-    "OpenZFSFileSystemConfigurationTypeDef",
-    {
-        "AutomaticBackupRetentionDays": int,
-        "CopyTagsToBackups": bool,
-        "CopyTagsToVolumes": bool,
-        "DailyAutomaticBackupStartTime": str,
-        "DeploymentType": OpenZFSDeploymentTypeType,
-        "ThroughputCapacity": int,
-        "WeeklyMaintenanceStartTime": str,
-        "DiskIopsConfiguration": DiskIopsConfigurationTypeDef,
-        "RootVolumeId": str,
-    },
-)
-
 UpdateFileSystemOntapConfigurationTypeDef = TypedDict(
     "UpdateFileSystemOntapConfigurationTypeDef",
     {
         "AutomaticBackupRetentionDays": int,
         "DailyAutomaticBackupStartTime": str,
         "FsxAdminPassword": str,
         "WeeklyMaintenanceStartTime": str,
@@ -1480,53 +1605,53 @@
 
 class CreateFileSystemWindowsConfigurationTypeDef(
     _RequiredCreateFileSystemWindowsConfigurationTypeDef,
     _OptionalCreateFileSystemWindowsConfigurationTypeDef,
 ):
     pass
 
-DataRepositoryConfigurationTypeDef = TypedDict(
-    "DataRepositoryConfigurationTypeDef",
+DataRepositoryConfigurationOutputTypeDef = TypedDict(
+    "DataRepositoryConfigurationOutputTypeDef",
     {
         "Lifecycle": DataRepositoryLifecycleType,
         "ImportPath": str,
         "ExportPath": str,
         "ImportedFileChunkSize": int,
         "AutoImportPolicy": AutoImportPolicyTypeType,
-        "FailureDetails": DataRepositoryFailureDetailsTypeDef,
+        "FailureDetails": DataRepositoryFailureDetailsOutputTypeDef,
     },
 )
 
 DescribeDataRepositoryTasksRequestRequestTypeDef = TypedDict(
     "DescribeDataRepositoryTasksRequestRequestTypeDef",
     {
         "TaskIds": Sequence[str],
         "Filters": Sequence[DataRepositoryTaskFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DataRepositoryTaskTypeDef = TypedDict(
-    "DataRepositoryTaskTypeDef",
+DataRepositoryTaskOutputTypeDef = TypedDict(
+    "DataRepositoryTaskOutputTypeDef",
     {
         "TaskId": str,
         "Lifecycle": DataRepositoryTaskLifecycleType,
         "Type": DataRepositoryTaskTypeType,
         "CreationTime": datetime,
         "StartTime": datetime,
         "EndTime": datetime,
         "ResourceARN": str,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "FileSystemId": str,
         "Paths": List[str],
-        "FailureDetails": DataRepositoryTaskFailureDetailsTypeDef,
-        "Status": DataRepositoryTaskStatusTypeDef,
-        "Report": CompletionReportTypeDef,
+        "FailureDetails": DataRepositoryTaskFailureDetailsOutputTypeDef,
+        "Status": DataRepositoryTaskStatusOutputTypeDef,
+        "Report": CompletionReportOutputTypeDef,
         "CapacityToRelease": int,
         "FileCacheId": str,
     },
 )
 
 DescribeBackupsRequestDescribeBackupsPaginateTypeDef = TypedDict(
     "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
@@ -1609,14 +1734,29 @@
         "Filters": Sequence[VolumeFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+OpenZFSFileSystemConfigurationOutputTypeDef = TypedDict(
+    "OpenZFSFileSystemConfigurationOutputTypeDef",
+    {
+        "AutomaticBackupRetentionDays": int,
+        "CopyTagsToBackups": bool,
+        "CopyTagsToVolumes": bool,
+        "DailyAutomaticBackupStartTime": str,
+        "DeploymentType": OpenZFSDeploymentTypeType,
+        "ThroughputCapacity": int,
+        "WeeklyMaintenanceStartTime": str,
+        "DiskIopsConfiguration": DiskIopsConfigurationOutputTypeDef,
+        "RootVolumeId": str,
+    },
+)
+
 _RequiredFileCacheDataRepositoryAssociationTypeDef = TypedDict(
     "_RequiredFileCacheDataRepositoryAssociationTypeDef",
     {
         "FileCachePath": str,
         "DataRepositoryPath": str,
     },
 )
@@ -1631,70 +1771,88 @@
 
 class FileCacheDataRepositoryAssociationTypeDef(
     _RequiredFileCacheDataRepositoryAssociationTypeDef,
     _OptionalFileCacheDataRepositoryAssociationTypeDef,
 ):
     pass
 
-FileCacheLustreConfigurationTypeDef = TypedDict(
-    "FileCacheLustreConfigurationTypeDef",
+FileCacheLustreConfigurationOutputTypeDef = TypedDict(
+    "FileCacheLustreConfigurationOutputTypeDef",
     {
         "PerUnitStorageThroughput": int,
         "DeploymentType": Literal["CACHE_1"],
         "MountName": str,
         "WeeklyMaintenanceStartTime": str,
-        "MetadataConfiguration": FileCacheLustreMetadataConfigurationTypeDef,
-        "LogConfiguration": LustreLogConfigurationTypeDef,
+        "MetadataConfiguration": FileCacheLustreMetadataConfigurationOutputTypeDef,
+        "LogConfiguration": LustreLogConfigurationOutputTypeDef,
     },
 )
 
-FileSystemEndpointsTypeDef = TypedDict(
-    "FileSystemEndpointsTypeDef",
+FileSystemEndpointsOutputTypeDef = TypedDict(
+    "FileSystemEndpointsOutputTypeDef",
     {
-        "Intercluster": FileSystemEndpointTypeDef,
-        "Management": FileSystemEndpointTypeDef,
+        "Intercluster": FileSystemEndpointOutputTypeDef,
+        "Management": FileSystemEndpointOutputTypeDef,
     },
 )
 
-SnapshotTypeDef = TypedDict(
-    "SnapshotTypeDef",
+SnapshotOutputTypeDef = TypedDict(
+    "SnapshotOutputTypeDef",
     {
         "ResourceARN": str,
         "SnapshotId": str,
         "Name": str,
         "VolumeId": str,
         "CreationTime": datetime,
         "Lifecycle": SnapshotLifecycleType,
-        "LifecycleTransitionReason": LifecycleTransitionReasonTypeDef,
-        "Tags": List[TagTypeDef],
-        "AdministrativeActions": List["AdministrativeActionTypeDef"],
+        "LifecycleTransitionReason": LifecycleTransitionReasonOutputTypeDef,
+        "Tags": List[TagOutputTypeDef],
+        "AdministrativeActions": List["AdministrativeActionOutputTypeDef"],
+    },
+)
+
+OpenZFSNfsExportOutputTypeDef = TypedDict(
+    "OpenZFSNfsExportOutputTypeDef",
+    {
+        "ClientConfigurations": List[OpenZFSClientConfigurationOutputTypeDef],
     },
 )
 
 OpenZFSNfsExportTypeDef = TypedDict(
     "OpenZFSNfsExportTypeDef",
     {
-        "ClientConfigurations": List[OpenZFSClientConfigurationTypeDef],
+        "ClientConfigurations": Sequence[OpenZFSClientConfigurationTypeDef],
+    },
+)
+
+SnaplockRetentionPeriodOutputTypeDef = TypedDict(
+    "SnaplockRetentionPeriodOutputTypeDef",
+    {
+        "DefaultRetention": RetentionPeriodOutputTypeDef,
+        "MinimumRetention": RetentionPeriodOutputTypeDef,
+        "MaximumRetention": RetentionPeriodOutputTypeDef,
     },
 )
 
 SnaplockRetentionPeriodTypeDef = TypedDict(
     "SnaplockRetentionPeriodTypeDef",
     {
         "DefaultRetention": RetentionPeriodTypeDef,
         "MinimumRetention": RetentionPeriodTypeDef,
         "MaximumRetention": RetentionPeriodTypeDef,
     },
 )
 
-SvmActiveDirectoryConfigurationTypeDef = TypedDict(
-    "SvmActiveDirectoryConfigurationTypeDef",
+SvmActiveDirectoryConfigurationOutputTypeDef = TypedDict(
+    "SvmActiveDirectoryConfigurationOutputTypeDef",
     {
         "NetBiosName": str,
-        "SelfManagedActiveDirectoryConfiguration": SelfManagedActiveDirectoryAttributesTypeDef,
+        "SelfManagedActiveDirectoryConfiguration": (
+            SelfManagedActiveDirectoryAttributesOutputTypeDef
+        ),
     },
 )
 
 UpdateFileSystemWindowsConfigurationTypeDef = TypedDict(
     "UpdateFileSystemWindowsConfigurationTypeDef",
     {
         "WeeklyMaintenanceStartTime": str,
@@ -1716,21 +1874,21 @@
             SelfManagedActiveDirectoryConfigurationUpdatesTypeDef
         ),
         "NetBiosName": str,
     },
     total=False,
 )
 
-SvmEndpointsTypeDef = TypedDict(
-    "SvmEndpointsTypeDef",
+SvmEndpointsOutputTypeDef = TypedDict(
+    "SvmEndpointsOutputTypeDef",
     {
-        "Iscsi": SvmEndpointTypeDef,
-        "Management": SvmEndpointTypeDef,
-        "Nfs": SvmEndpointTypeDef,
-        "Smb": SvmEndpointTypeDef,
+        "Iscsi": SvmEndpointOutputTypeDef,
+        "Management": SvmEndpointOutputTypeDef,
+        "Nfs": SvmEndpointOutputTypeDef,
+        "Smb": SvmEndpointOutputTypeDef,
     },
 )
 
 _RequiredUpdateFileCacheRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFileCacheRequestRequestTypeDef",
     {
         "FileCacheId": str,
@@ -1746,31 +1904,55 @@
 )
 
 class UpdateFileCacheRequestRequestTypeDef(
     _RequiredUpdateFileCacheRequestRequestTypeDef, _OptionalUpdateFileCacheRequestRequestTypeDef
 ):
     pass
 
-WindowsFileSystemConfigurationTypeDef = TypedDict(
-    "WindowsFileSystemConfigurationTypeDef",
+WindowsFileSystemConfigurationOutputTypeDef = TypedDict(
+    "WindowsFileSystemConfigurationOutputTypeDef",
     {
         "ActiveDirectoryId": str,
-        "SelfManagedActiveDirectoryConfiguration": SelfManagedActiveDirectoryAttributesTypeDef,
+        "SelfManagedActiveDirectoryConfiguration": (
+            SelfManagedActiveDirectoryAttributesOutputTypeDef
+        ),
         "DeploymentType": WindowsDeploymentTypeType,
         "RemoteAdministrationEndpoint": str,
         "PreferredSubnetId": str,
         "PreferredFileServerIp": str,
         "ThroughputCapacity": int,
         "MaintenanceOperationsInProgress": List[FileSystemMaintenanceOperationType],
         "WeeklyMaintenanceStartTime": str,
         "DailyAutomaticBackupStartTime": str,
         "AutomaticBackupRetentionDays": int,
         "CopyTagsToBackups": bool,
-        "Aliases": List[AliasTypeDef],
-        "AuditLogConfiguration": WindowsAuditLogConfigurationTypeDef,
+        "Aliases": List[AliasOutputTypeDef],
+        "AuditLogConfiguration": WindowsAuditLogConfigurationOutputTypeDef,
+    },
+)
+
+DataRepositoryAssociationOutputTypeDef = TypedDict(
+    "DataRepositoryAssociationOutputTypeDef",
+    {
+        "AssociationId": str,
+        "ResourceARN": str,
+        "FileSystemId": str,
+        "Lifecycle": DataRepositoryLifecycleType,
+        "FailureDetails": DataRepositoryFailureDetailsOutputTypeDef,
+        "FileSystemPath": str,
+        "DataRepositoryPath": str,
+        "BatchImportMetaDataOnCreate": bool,
+        "ImportedFileChunkSize": int,
+        "S3": S3DataRepositoryConfigurationOutputTypeDef,
+        "Tags": List[TagOutputTypeDef],
+        "CreationTime": datetime,
+        "FileCacheId": str,
+        "FileCachePath": str,
+        "DataRepositorySubdirectories": List[str],
+        "NFS": NFSDataRepositoryConfigurationOutputTypeDef,
     },
 )
 
 _RequiredCreateDataRepositoryAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataRepositoryAssociationRequestRequestTypeDef",
     {
         "FileSystemId": str,
@@ -1792,36 +1974,14 @@
 
 class CreateDataRepositoryAssociationRequestRequestTypeDef(
     _RequiredCreateDataRepositoryAssociationRequestRequestTypeDef,
     _OptionalCreateDataRepositoryAssociationRequestRequestTypeDef,
 ):
     pass
 
-DataRepositoryAssociationTypeDef = TypedDict(
-    "DataRepositoryAssociationTypeDef",
-    {
-        "AssociationId": str,
-        "ResourceARN": str,
-        "FileSystemId": str,
-        "Lifecycle": DataRepositoryLifecycleType,
-        "FailureDetails": DataRepositoryFailureDetailsTypeDef,
-        "FileSystemPath": str,
-        "DataRepositoryPath": str,
-        "BatchImportMetaDataOnCreate": bool,
-        "ImportedFileChunkSize": int,
-        "S3": S3DataRepositoryConfigurationTypeDef,
-        "Tags": List[TagTypeDef],
-        "CreationTime": datetime,
-        "FileCacheId": str,
-        "FileCachePath": str,
-        "DataRepositorySubdirectories": List[str],
-        "NFS": NFSDataRepositoryConfigurationTypeDef,
-    },
-)
-
 _RequiredUpdateDataRepositoryAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDataRepositoryAssociationRequestRequestTypeDef",
     {
         "AssociationId": str,
     },
 )
 _OptionalUpdateDataRepositoryAssociationRequestRequestTypeDef = TypedDict(
@@ -1836,14 +1996,36 @@
 
 class UpdateDataRepositoryAssociationRequestRequestTypeDef(
     _RequiredUpdateDataRepositoryAssociationRequestRequestTypeDef,
     _OptionalUpdateDataRepositoryAssociationRequestRequestTypeDef,
 ):
     pass
 
+DeleteFileSystemResponseOutputTypeDef = TypedDict(
+    "DeleteFileSystemResponseOutputTypeDef",
+    {
+        "FileSystemId": str,
+        "Lifecycle": FileSystemLifecycleType,
+        "WindowsResponse": DeleteFileSystemWindowsResponseOutputTypeDef,
+        "LustreResponse": DeleteFileSystemLustreResponseOutputTypeDef,
+        "OpenZFSResponse": DeleteFileSystemOpenZFSResponseOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DeleteVolumeResponseOutputTypeDef = TypedDict(
+    "DeleteVolumeResponseOutputTypeDef",
+    {
+        "VolumeId": str,
+        "Lifecycle": VolumeLifecycleType,
+        "OntapResponse": DeleteVolumeOntapResponseOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDeleteFileSystemRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteFileSystemRequestRequestTypeDef",
     {
         "FileSystemId": str,
     },
 )
 _OptionalDeleteFileSystemRequestRequestTypeDef = TypedDict(
@@ -1858,26 +2040,14 @@
 )
 
 class DeleteFileSystemRequestRequestTypeDef(
     _RequiredDeleteFileSystemRequestRequestTypeDef, _OptionalDeleteFileSystemRequestRequestTypeDef
 ):
     pass
 
-DeleteFileSystemResponseTypeDef = TypedDict(
-    "DeleteFileSystemResponseTypeDef",
-    {
-        "FileSystemId": str,
-        "Lifecycle": FileSystemLifecycleType,
-        "WindowsResponse": DeleteFileSystemWindowsResponseTypeDef,
-        "LustreResponse": DeleteFileSystemLustreResponseTypeDef,
-        "OpenZFSResponse": DeleteFileSystemOpenZFSResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteVolumeRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteVolumeRequestRequestTypeDef",
     {
         "VolumeId": str,
     },
 )
 _OptionalDeleteVolumeRequestRequestTypeDef = TypedDict(
@@ -1891,24 +2061,14 @@
 )
 
 class DeleteVolumeRequestRequestTypeDef(
     _RequiredDeleteVolumeRequestRequestTypeDef, _OptionalDeleteVolumeRequestRequestTypeDef
 ):
     pass
 
-DeleteVolumeResponseTypeDef = TypedDict(
-    "DeleteVolumeResponseTypeDef",
-    {
-        "VolumeId": str,
-        "Lifecycle": VolumeLifecycleType,
-        "OntapResponse": DeleteVolumeOntapResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateStorageVirtualMachineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStorageVirtualMachineRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "Name": str,
     },
 )
@@ -1926,44 +2086,44 @@
 
 class CreateStorageVirtualMachineRequestRequestTypeDef(
     _RequiredCreateStorageVirtualMachineRequestRequestTypeDef,
     _OptionalCreateStorageVirtualMachineRequestRequestTypeDef,
 ):
     pass
 
-LustreFileSystemConfigurationTypeDef = TypedDict(
-    "LustreFileSystemConfigurationTypeDef",
+LustreFileSystemConfigurationOutputTypeDef = TypedDict(
+    "LustreFileSystemConfigurationOutputTypeDef",
     {
         "WeeklyMaintenanceStartTime": str,
-        "DataRepositoryConfiguration": DataRepositoryConfigurationTypeDef,
+        "DataRepositoryConfiguration": DataRepositoryConfigurationOutputTypeDef,
         "DeploymentType": LustreDeploymentTypeType,
         "PerUnitStorageThroughput": int,
         "MountName": str,
         "DailyAutomaticBackupStartTime": str,
         "AutomaticBackupRetentionDays": int,
         "CopyTagsToBackups": bool,
         "DriveCacheType": DriveCacheTypeType,
         "DataCompressionType": DataCompressionTypeType,
-        "LogConfiguration": LustreLogConfigurationTypeDef,
-        "RootSquashConfiguration": LustreRootSquashConfigurationTypeDef,
+        "LogConfiguration": LustreLogConfigurationOutputTypeDef,
+        "RootSquashConfiguration": LustreRootSquashConfigurationOutputTypeDef,
     },
 )
 
-CreateDataRepositoryTaskResponseTypeDef = TypedDict(
-    "CreateDataRepositoryTaskResponseTypeDef",
+CreateDataRepositoryTaskResponseOutputTypeDef = TypedDict(
+    "CreateDataRepositoryTaskResponseOutputTypeDef",
     {
-        "DataRepositoryTask": DataRepositoryTaskTypeDef,
+        "DataRepositoryTask": DataRepositoryTaskOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeDataRepositoryTasksResponseTypeDef = TypedDict(
-    "DescribeDataRepositoryTasksResponseTypeDef",
+DescribeDataRepositoryTasksResponseOutputTypeDef = TypedDict(
+    "DescribeDataRepositoryTasksResponseOutputTypeDef",
     {
-        "DataRepositoryTasks": List[DataRepositoryTaskTypeDef],
+        "DataRepositoryTasks": List[DataRepositoryTaskOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateFileCacheRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFileCacheRequestRequestTypeDef",
@@ -1989,102 +2149,122 @@
 )
 
 class CreateFileCacheRequestRequestTypeDef(
     _RequiredCreateFileCacheRequestRequestTypeDef, _OptionalCreateFileCacheRequestRequestTypeDef
 ):
     pass
 
-FileCacheCreatingTypeDef = TypedDict(
-    "FileCacheCreatingTypeDef",
+FileCacheCreatingOutputTypeDef = TypedDict(
+    "FileCacheCreatingOutputTypeDef",
     {
         "OwnerId": str,
         "CreationTime": datetime,
         "FileCacheId": str,
         "FileCacheType": Literal["LUSTRE"],
         "FileCacheTypeVersion": str,
         "Lifecycle": FileCacheLifecycleType,
-        "FailureDetails": FileCacheFailureDetailsTypeDef,
+        "FailureDetails": FileCacheFailureDetailsOutputTypeDef,
         "StorageCapacity": int,
         "VpcId": str,
         "SubnetIds": List[str],
         "NetworkInterfaceIds": List[str],
         "DNSName": str,
         "KmsKeyId": str,
         "ResourceARN": str,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "CopyTagsToDataRepositoryAssociations": bool,
-        "LustreConfiguration": FileCacheLustreConfigurationTypeDef,
+        "LustreConfiguration": FileCacheLustreConfigurationOutputTypeDef,
         "DataRepositoryAssociationIds": List[str],
     },
 )
 
-FileCacheTypeDef = TypedDict(
-    "FileCacheTypeDef",
+FileCacheOutputTypeDef = TypedDict(
+    "FileCacheOutputTypeDef",
     {
         "OwnerId": str,
         "CreationTime": datetime,
         "FileCacheId": str,
         "FileCacheType": Literal["LUSTRE"],
         "FileCacheTypeVersion": str,
         "Lifecycle": FileCacheLifecycleType,
-        "FailureDetails": FileCacheFailureDetailsTypeDef,
+        "FailureDetails": FileCacheFailureDetailsOutputTypeDef,
         "StorageCapacity": int,
         "VpcId": str,
         "SubnetIds": List[str],
         "NetworkInterfaceIds": List[str],
         "DNSName": str,
         "KmsKeyId": str,
         "ResourceARN": str,
-        "LustreConfiguration": FileCacheLustreConfigurationTypeDef,
+        "LustreConfiguration": FileCacheLustreConfigurationOutputTypeDef,
         "DataRepositoryAssociationIds": List[str],
     },
 )
 
-OntapFileSystemConfigurationTypeDef = TypedDict(
-    "OntapFileSystemConfigurationTypeDef",
+OntapFileSystemConfigurationOutputTypeDef = TypedDict(
+    "OntapFileSystemConfigurationOutputTypeDef",
     {
         "AutomaticBackupRetentionDays": int,
         "DailyAutomaticBackupStartTime": str,
         "DeploymentType": OntapDeploymentTypeType,
         "EndpointIpAddressRange": str,
-        "Endpoints": FileSystemEndpointsTypeDef,
-        "DiskIopsConfiguration": DiskIopsConfigurationTypeDef,
+        "Endpoints": FileSystemEndpointsOutputTypeDef,
+        "DiskIopsConfiguration": DiskIopsConfigurationOutputTypeDef,
         "PreferredSubnetId": str,
         "RouteTableIds": List[str],
         "ThroughputCapacity": int,
         "WeeklyMaintenanceStartTime": str,
         "FsxAdminPassword": str,
     },
 )
 
-CreateSnapshotResponseTypeDef = TypedDict(
-    "CreateSnapshotResponseTypeDef",
+CreateSnapshotResponseOutputTypeDef = TypedDict(
+    "CreateSnapshotResponseOutputTypeDef",
     {
-        "Snapshot": SnapshotTypeDef,
+        "Snapshot": SnapshotOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeSnapshotsResponseTypeDef = TypedDict(
-    "DescribeSnapshotsResponseTypeDef",
+DescribeSnapshotsResponseOutputTypeDef = TypedDict(
+    "DescribeSnapshotsResponseOutputTypeDef",
     {
-        "Snapshots": List[SnapshotTypeDef],
+        "Snapshots": List[SnapshotOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateSnapshotResponseTypeDef = TypedDict(
-    "UpdateSnapshotResponseTypeDef",
+UpdateSnapshotResponseOutputTypeDef = TypedDict(
+    "UpdateSnapshotResponseOutputTypeDef",
     {
-        "Snapshot": SnapshotTypeDef,
+        "Snapshot": SnapshotOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+OpenZFSVolumeConfigurationOutputTypeDef = TypedDict(
+    "OpenZFSVolumeConfigurationOutputTypeDef",
+    {
+        "ParentVolumeId": str,
+        "VolumePath": str,
+        "StorageCapacityReservationGiB": int,
+        "StorageCapacityQuotaGiB": int,
+        "RecordSizeKiB": int,
+        "DataCompressionType": OpenZFSDataCompressionTypeType,
+        "CopyTagsToSnapshots": bool,
+        "OriginSnapshot": OpenZFSOriginSnapshotConfigurationOutputTypeDef,
+        "ReadOnly": bool,
+        "NfsExports": List[OpenZFSNfsExportOutputTypeDef],
+        "UserAndGroupQuotas": List[OpenZFSUserOrGroupQuotaOutputTypeDef],
+        "RestoreToSnapshot": str,
+        "DeleteIntermediateSnaphots": bool,
+        "DeleteClonedVolumes": bool,
+    },
+)
+
 _RequiredCreateOpenZFSVolumeConfigurationTypeDef = TypedDict(
     "_RequiredCreateOpenZFSVolumeConfigurationTypeDef",
     {
         "ParentVolumeId": str,
     },
 )
 _OptionalCreateOpenZFSVolumeConfigurationTypeDef = TypedDict(
@@ -2118,48 +2298,40 @@
         "UserAndGroupQuotas": Sequence[OpenZFSUserOrGroupQuotaTypeDef],
         "CopyTagsToSnapshots": bool,
         "ReadOnly": bool,
     },
     total=False,
 )
 
-OpenZFSVolumeConfigurationTypeDef = TypedDict(
-    "OpenZFSVolumeConfigurationTypeDef",
-    {
-        "ParentVolumeId": str,
-        "VolumePath": str,
-        "StorageCapacityReservationGiB": int,
-        "StorageCapacityQuotaGiB": int,
-        "RecordSizeKiB": int,
-        "DataCompressionType": OpenZFSDataCompressionTypeType,
-        "CopyTagsToSnapshots": bool,
-        "OriginSnapshot": OpenZFSOriginSnapshotConfigurationTypeDef,
-        "ReadOnly": bool,
-        "NfsExports": List[OpenZFSNfsExportTypeDef],
-        "UserAndGroupQuotas": List[OpenZFSUserOrGroupQuotaTypeDef],
-        "RestoreToSnapshot": str,
-        "DeleteIntermediateSnaphots": bool,
-        "DeleteClonedVolumes": bool,
-    },
-)
-
 UpdateOpenZFSVolumeConfigurationTypeDef = TypedDict(
     "UpdateOpenZFSVolumeConfigurationTypeDef",
     {
         "StorageCapacityReservationGiB": int,
         "StorageCapacityQuotaGiB": int,
         "RecordSizeKiB": int,
         "DataCompressionType": OpenZFSDataCompressionTypeType,
         "NfsExports": Sequence[OpenZFSNfsExportTypeDef],
         "UserAndGroupQuotas": Sequence[OpenZFSUserOrGroupQuotaTypeDef],
         "ReadOnly": bool,
     },
     total=False,
 )
 
+SnaplockConfigurationOutputTypeDef = TypedDict(
+    "SnaplockConfigurationOutputTypeDef",
+    {
+        "AuditLogVolume": bool,
+        "AutocommitPeriod": AutocommitPeriodOutputTypeDef,
+        "PrivilegedDelete": PrivilegedDeleteType,
+        "RetentionPeriod": SnaplockRetentionPeriodOutputTypeDef,
+        "SnaplockType": SnaplockTypeType,
+        "VolumeAppendModeEnabled": bool,
+    },
+)
+
 _RequiredCreateSnaplockConfigurationTypeDef = TypedDict(
     "_RequiredCreateSnaplockConfigurationTypeDef",
     {
         "SnaplockType": SnaplockTypeType,
     },
 )
 _OptionalCreateSnaplockConfigurationTypeDef = TypedDict(
@@ -2175,26 +2347,14 @@
 )
 
 class CreateSnaplockConfigurationTypeDef(
     _RequiredCreateSnaplockConfigurationTypeDef, _OptionalCreateSnaplockConfigurationTypeDef
 ):
     pass
 
-SnaplockConfigurationTypeDef = TypedDict(
-    "SnaplockConfigurationTypeDef",
-    {
-        "AuditLogVolume": bool,
-        "AutocommitPeriod": AutocommitPeriodTypeDef,
-        "PrivilegedDelete": PrivilegedDeleteType,
-        "RetentionPeriod": SnaplockRetentionPeriodTypeDef,
-        "SnaplockType": SnaplockTypeType,
-        "VolumeAppendModeEnabled": bool,
-    },
-)
-
 UpdateSnaplockConfigurationTypeDef = TypedDict(
     "UpdateSnaplockConfigurationTypeDef",
     {
         "AuditLogVolume": bool,
         "AutocommitPeriod": AutocommitPeriodTypeDef,
         "PrivilegedDelete": PrivilegedDeleteType,
         "RetentionPeriod": SnaplockRetentionPeriodTypeDef,
@@ -2245,107 +2405,107 @@
 
 class UpdateStorageVirtualMachineRequestRequestTypeDef(
     _RequiredUpdateStorageVirtualMachineRequestRequestTypeDef,
     _OptionalUpdateStorageVirtualMachineRequestRequestTypeDef,
 ):
     pass
 
-StorageVirtualMachineTypeDef = TypedDict(
-    "StorageVirtualMachineTypeDef",
+StorageVirtualMachineOutputTypeDef = TypedDict(
+    "StorageVirtualMachineOutputTypeDef",
     {
-        "ActiveDirectoryConfiguration": SvmActiveDirectoryConfigurationTypeDef,
+        "ActiveDirectoryConfiguration": SvmActiveDirectoryConfigurationOutputTypeDef,
         "CreationTime": datetime,
-        "Endpoints": SvmEndpointsTypeDef,
+        "Endpoints": SvmEndpointsOutputTypeDef,
         "FileSystemId": str,
         "Lifecycle": StorageVirtualMachineLifecycleType,
         "Name": str,
         "ResourceARN": str,
         "StorageVirtualMachineId": str,
         "Subtype": StorageVirtualMachineSubtypeType,
         "UUID": str,
-        "Tags": List[TagTypeDef],
-        "LifecycleTransitionReason": LifecycleTransitionReasonTypeDef,
+        "Tags": List[TagOutputTypeDef],
+        "LifecycleTransitionReason": LifecycleTransitionReasonOutputTypeDef,
         "RootVolumeSecurityStyle": StorageVirtualMachineRootVolumeSecurityStyleType,
     },
 )
 
-CreateDataRepositoryAssociationResponseTypeDef = TypedDict(
-    "CreateDataRepositoryAssociationResponseTypeDef",
+CreateDataRepositoryAssociationResponseOutputTypeDef = TypedDict(
+    "CreateDataRepositoryAssociationResponseOutputTypeDef",
     {
-        "Association": DataRepositoryAssociationTypeDef,
+        "Association": DataRepositoryAssociationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeDataRepositoryAssociationsResponseTypeDef = TypedDict(
-    "DescribeDataRepositoryAssociationsResponseTypeDef",
+DescribeDataRepositoryAssociationsResponseOutputTypeDef = TypedDict(
+    "DescribeDataRepositoryAssociationsResponseOutputTypeDef",
     {
-        "Associations": List[DataRepositoryAssociationTypeDef],
+        "Associations": List[DataRepositoryAssociationOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateDataRepositoryAssociationResponseTypeDef = TypedDict(
-    "UpdateDataRepositoryAssociationResponseTypeDef",
+UpdateDataRepositoryAssociationResponseOutputTypeDef = TypedDict(
+    "UpdateDataRepositoryAssociationResponseOutputTypeDef",
     {
-        "Association": DataRepositoryAssociationTypeDef,
+        "Association": DataRepositoryAssociationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateFileCacheResponseTypeDef = TypedDict(
-    "CreateFileCacheResponseTypeDef",
+CreateFileCacheResponseOutputTypeDef = TypedDict(
+    "CreateFileCacheResponseOutputTypeDef",
     {
-        "FileCache": FileCacheCreatingTypeDef,
+        "FileCache": FileCacheCreatingOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeFileCachesResponseTypeDef = TypedDict(
-    "DescribeFileCachesResponseTypeDef",
+DescribeFileCachesResponseOutputTypeDef = TypedDict(
+    "DescribeFileCachesResponseOutputTypeDef",
     {
-        "FileCaches": List[FileCacheTypeDef],
+        "FileCaches": List[FileCacheOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateFileCacheResponseTypeDef = TypedDict(
-    "UpdateFileCacheResponseTypeDef",
+UpdateFileCacheResponseOutputTypeDef = TypedDict(
+    "UpdateFileCacheResponseOutputTypeDef",
     {
-        "FileCache": FileCacheTypeDef,
+        "FileCache": FileCacheOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-FileSystemTypeDef = TypedDict(
-    "FileSystemTypeDef",
+FileSystemOutputTypeDef = TypedDict(
+    "FileSystemOutputTypeDef",
     {
         "OwnerId": str,
         "CreationTime": datetime,
         "FileSystemId": str,
         "FileSystemType": FileSystemTypeType,
         "Lifecycle": FileSystemLifecycleType,
-        "FailureDetails": FileSystemFailureDetailsTypeDef,
+        "FailureDetails": FileSystemFailureDetailsOutputTypeDef,
         "StorageCapacity": int,
         "StorageType": StorageTypeType,
         "VpcId": str,
         "SubnetIds": List[str],
         "NetworkInterfaceIds": List[str],
         "DNSName": str,
         "KmsKeyId": str,
         "ResourceARN": str,
-        "Tags": List[TagTypeDef],
-        "WindowsConfiguration": WindowsFileSystemConfigurationTypeDef,
-        "LustreConfiguration": LustreFileSystemConfigurationTypeDef,
-        "AdministrativeActions": List["AdministrativeActionTypeDef"],
-        "OntapConfiguration": OntapFileSystemConfigurationTypeDef,
+        "Tags": List[TagOutputTypeDef],
+        "WindowsConfiguration": WindowsFileSystemConfigurationOutputTypeDef,
+        "LustreConfiguration": LustreFileSystemConfigurationOutputTypeDef,
+        "AdministrativeActions": List["AdministrativeActionOutputTypeDef"],
+        "OntapConfiguration": OntapFileSystemConfigurationOutputTypeDef,
         "FileSystemTypeVersion": str,
-        "OpenZFSConfiguration": OpenZFSFileSystemConfigurationTypeDef,
+        "OpenZFSConfiguration": OpenZFSFileSystemConfigurationOutputTypeDef,
     },
 )
 
 _RequiredCreateFileSystemOpenZFSConfigurationTypeDef = TypedDict(
     "_RequiredCreateFileSystemOpenZFSConfigurationTypeDef",
     {
         "DeploymentType": OpenZFSDeploymentTypeType,
@@ -2368,14 +2528,33 @@
 
 class CreateFileSystemOpenZFSConfigurationTypeDef(
     _RequiredCreateFileSystemOpenZFSConfigurationTypeDef,
     _OptionalCreateFileSystemOpenZFSConfigurationTypeDef,
 ):
     pass
 
+OntapVolumeConfigurationOutputTypeDef = TypedDict(
+    "OntapVolumeConfigurationOutputTypeDef",
+    {
+        "FlexCacheEndpointType": FlexCacheEndpointTypeType,
+        "JunctionPath": str,
+        "SecurityStyle": SecurityStyleType,
+        "SizeInMegabytes": int,
+        "StorageEfficiencyEnabled": bool,
+        "StorageVirtualMachineId": str,
+        "StorageVirtualMachineRoot": bool,
+        "TieringPolicy": TieringPolicyOutputTypeDef,
+        "UUID": str,
+        "OntapVolumeType": OntapVolumeTypeType,
+        "SnapshotPolicy": str,
+        "CopyTagsToBackups": bool,
+        "SnaplockConfiguration": SnaplockConfigurationOutputTypeDef,
+    },
+)
+
 _RequiredCreateOntapVolumeConfigurationTypeDef = TypedDict(
     "_RequiredCreateOntapVolumeConfigurationTypeDef",
     {
         "SizeInMegabytes": int,
         "StorageVirtualMachineId": str,
     },
 )
@@ -2395,33 +2574,14 @@
 )
 
 class CreateOntapVolumeConfigurationTypeDef(
     _RequiredCreateOntapVolumeConfigurationTypeDef, _OptionalCreateOntapVolumeConfigurationTypeDef
 ):
     pass
 
-OntapVolumeConfigurationTypeDef = TypedDict(
-    "OntapVolumeConfigurationTypeDef",
-    {
-        "FlexCacheEndpointType": FlexCacheEndpointTypeType,
-        "JunctionPath": str,
-        "SecurityStyle": SecurityStyleType,
-        "SizeInMegabytes": int,
-        "StorageEfficiencyEnabled": bool,
-        "StorageVirtualMachineId": str,
-        "StorageVirtualMachineRoot": bool,
-        "TieringPolicy": TieringPolicyTypeDef,
-        "UUID": str,
-        "OntapVolumeType": OntapVolumeTypeType,
-        "SnapshotPolicy": str,
-        "CopyTagsToBackups": bool,
-        "SnaplockConfiguration": SnaplockConfigurationTypeDef,
-    },
-)
-
 UpdateOntapVolumeConfigurationTypeDef = TypedDict(
     "UpdateOntapVolumeConfigurationTypeDef",
     {
         "JunctionPath": str,
         "SecurityStyle": SecurityStyleType,
         "SizeInMegabytes": int,
         "StorageEfficiencyEnabled": bool,
@@ -2429,35 +2589,35 @@
         "SnapshotPolicy": str,
         "CopyTagsToBackups": bool,
         "SnaplockConfiguration": UpdateSnaplockConfigurationTypeDef,
     },
     total=False,
 )
 
-CreateStorageVirtualMachineResponseTypeDef = TypedDict(
-    "CreateStorageVirtualMachineResponseTypeDef",
+CreateStorageVirtualMachineResponseOutputTypeDef = TypedDict(
+    "CreateStorageVirtualMachineResponseOutputTypeDef",
     {
-        "StorageVirtualMachine": StorageVirtualMachineTypeDef,
+        "StorageVirtualMachine": StorageVirtualMachineOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeStorageVirtualMachinesResponseTypeDef = TypedDict(
-    "DescribeStorageVirtualMachinesResponseTypeDef",
+DescribeStorageVirtualMachinesResponseOutputTypeDef = TypedDict(
+    "DescribeStorageVirtualMachinesResponseOutputTypeDef",
     {
-        "StorageVirtualMachines": List[StorageVirtualMachineTypeDef],
+        "StorageVirtualMachines": List[StorageVirtualMachineOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateStorageVirtualMachineResponseTypeDef = TypedDict(
-    "UpdateStorageVirtualMachineResponseTypeDef",
+UpdateStorageVirtualMachineResponseOutputTypeDef = TypedDict(
+    "UpdateStorageVirtualMachineResponseOutputTypeDef",
     {
-        "StorageVirtualMachine": StorageVirtualMachineTypeDef,
+        "StorageVirtualMachine": StorageVirtualMachineOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateFileSystemFromBackupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFileSystemFromBackupRequestRequestTypeDef",
     {
@@ -2514,14 +2674,32 @@
 )
 
 class CreateFileSystemRequestRequestTypeDef(
     _RequiredCreateFileSystemRequestRequestTypeDef, _OptionalCreateFileSystemRequestRequestTypeDef
 ):
     pass
 
+VolumeOutputTypeDef = TypedDict(
+    "VolumeOutputTypeDef",
+    {
+        "CreationTime": datetime,
+        "FileSystemId": str,
+        "Lifecycle": VolumeLifecycleType,
+        "Name": str,
+        "OntapConfiguration": OntapVolumeConfigurationOutputTypeDef,
+        "ResourceARN": str,
+        "Tags": List[TagOutputTypeDef],
+        "VolumeId": str,
+        "VolumeType": VolumeTypeType,
+        "LifecycleTransitionReason": LifecycleTransitionReasonOutputTypeDef,
+        "AdministrativeActions": List[Dict[str, Any]],
+        "OpenZFSConfiguration": OpenZFSVolumeConfigurationOutputTypeDef,
+    },
+)
+
 _RequiredCreateVolumeFromBackupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVolumeFromBackupRequestRequestTypeDef",
     {
         "BackupId": str,
         "Name": str,
     },
 )
@@ -2560,32 +2738,14 @@
 )
 
 class CreateVolumeRequestRequestTypeDef(
     _RequiredCreateVolumeRequestRequestTypeDef, _OptionalCreateVolumeRequestRequestTypeDef
 ):
     pass
 
-VolumeTypeDef = TypedDict(
-    "VolumeTypeDef",
-    {
-        "CreationTime": datetime,
-        "FileSystemId": str,
-        "Lifecycle": VolumeLifecycleType,
-        "Name": str,
-        "OntapConfiguration": OntapVolumeConfigurationTypeDef,
-        "ResourceARN": str,
-        "Tags": List[TagTypeDef],
-        "VolumeId": str,
-        "VolumeType": VolumeTypeType,
-        "LifecycleTransitionReason": LifecycleTransitionReasonTypeDef,
-        "AdministrativeActions": List[Dict[str, Any]],
-        "OpenZFSConfiguration": OpenZFSVolumeConfigurationTypeDef,
-    },
-)
-
 _RequiredUpdateVolumeRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateVolumeRequestRequestTypeDef",
     {
         "VolumeId": str,
     },
 )
 _OptionalUpdateVolumeRequestRequestTypeDef = TypedDict(
@@ -2600,100 +2760,100 @@
 )
 
 class UpdateVolumeRequestRequestTypeDef(
     _RequiredUpdateVolumeRequestRequestTypeDef, _OptionalUpdateVolumeRequestRequestTypeDef
 ):
     pass
 
-AdministrativeActionTypeDef = TypedDict(
-    "AdministrativeActionTypeDef",
+AdministrativeActionOutputTypeDef = TypedDict(
+    "AdministrativeActionOutputTypeDef",
     {
         "AdministrativeActionType": AdministrativeActionTypeType,
         "ProgressPercent": int,
         "RequestTime": datetime,
         "Status": StatusType,
         "TargetFileSystemValues": Dict[str, Any],
-        "FailureDetails": AdministrativeActionFailureDetailsTypeDef,
+        "FailureDetails": AdministrativeActionFailureDetailsOutputTypeDef,
         "TargetVolumeValues": Dict[str, Any],
         "TargetSnapshotValues": Dict[str, Any],
     },
 )
 
-BackupTypeDef = TypedDict(
-    "BackupTypeDef",
+BackupOutputTypeDef = TypedDict(
+    "BackupOutputTypeDef",
     {
         "BackupId": str,
         "Lifecycle": BackupLifecycleType,
-        "FailureDetails": BackupFailureDetailsTypeDef,
+        "FailureDetails": BackupFailureDetailsOutputTypeDef,
         "Type": BackupTypeType,
         "ProgressPercent": int,
         "CreationTime": datetime,
         "KmsKeyId": str,
         "ResourceARN": str,
-        "Tags": List[TagTypeDef],
-        "FileSystem": "FileSystemTypeDef",
-        "DirectoryInformation": ActiveDirectoryBackupAttributesTypeDef,
+        "Tags": List[TagOutputTypeDef],
+        "FileSystem": "FileSystemOutputTypeDef",
+        "DirectoryInformation": ActiveDirectoryBackupAttributesOutputTypeDef,
         "OwnerId": str,
         "SourceBackupId": str,
         "SourceBackupRegion": str,
         "ResourceType": ResourceTypeType,
-        "Volume": VolumeTypeDef,
+        "Volume": VolumeOutputTypeDef,
     },
 )
 
-CreateVolumeFromBackupResponseTypeDef = TypedDict(
-    "CreateVolumeFromBackupResponseTypeDef",
+CreateVolumeFromBackupResponseOutputTypeDef = TypedDict(
+    "CreateVolumeFromBackupResponseOutputTypeDef",
     {
-        "Volume": VolumeTypeDef,
+        "Volume": VolumeOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateVolumeResponseTypeDef = TypedDict(
-    "CreateVolumeResponseTypeDef",
+CreateVolumeResponseOutputTypeDef = TypedDict(
+    "CreateVolumeResponseOutputTypeDef",
     {
-        "Volume": VolumeTypeDef,
+        "Volume": VolumeOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeVolumesResponseTypeDef = TypedDict(
-    "DescribeVolumesResponseTypeDef",
+DescribeVolumesResponseOutputTypeDef = TypedDict(
+    "DescribeVolumesResponseOutputTypeDef",
     {
-        "Volumes": List[VolumeTypeDef],
+        "Volumes": List[VolumeOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateVolumeResponseTypeDef = TypedDict(
-    "UpdateVolumeResponseTypeDef",
+UpdateVolumeResponseOutputTypeDef = TypedDict(
+    "UpdateVolumeResponseOutputTypeDef",
     {
-        "Volume": VolumeTypeDef,
+        "Volume": VolumeOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CopyBackupResponseTypeDef = TypedDict(
-    "CopyBackupResponseTypeDef",
+CopyBackupResponseOutputTypeDef = TypedDict(
+    "CopyBackupResponseOutputTypeDef",
     {
-        "Backup": BackupTypeDef,
+        "Backup": BackupOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateBackupResponseTypeDef = TypedDict(
-    "CreateBackupResponseTypeDef",
+CreateBackupResponseOutputTypeDef = TypedDict(
+    "CreateBackupResponseOutputTypeDef",
     {
-        "Backup": BackupTypeDef,
+        "Backup": BackupOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeBackupsResponseTypeDef = TypedDict(
-    "DescribeBackupsResponseTypeDef",
+DescribeBackupsResponseOutputTypeDef = TypedDict(
+    "DescribeBackupsResponseOutputTypeDef",
     {
-        "Backups": List[BackupTypeDef],
+        "Backups": List[BackupOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-fsx-1.28.3/mypy_boto3_fsx.egg-info/PKG-INFO` & `mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-fsx
-Version: 1.28.3
-Summary: Type annotations for boto3.FSx 1.28.3 service generated with mypy-boto3-builder 7.14.6
+Version: 1.28.3.post1
+Summary: Type annotations for boto3.FSx 1.28.3 service generated with mypy-boto3-builder 7.14.7
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/
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
 [mypy-boto3-fsx docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/).
 
 See how it helps to find and fix potential bugs:
 
@@ -393,199 +393,214 @@
 ### Typed dictionaries
 
 `mypy_boto3_fsx.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_fsx.type_defs import (
-    ActiveDirectoryBackupAttributesTypeDef,
-    AdministrativeActionFailureDetailsTypeDef,
-    AliasTypeDef,
+    ActiveDirectoryBackupAttributesOutputTypeDef,
+    AdministrativeActionFailureDetailsOutputTypeDef,
+    AliasOutputTypeDef,
     AssociateFileSystemAliasesRequestRequestTypeDef,
+    AutoExportPolicyOutputTypeDef,
     AutoExportPolicyTypeDef,
+    AutoImportPolicyOutputTypeDef,
     AutoImportPolicyTypeDef,
+    AutocommitPeriodOutputTypeDef,
     AutocommitPeriodTypeDef,
-    BackupFailureDetailsTypeDef,
-    TagTypeDef,
+    BackupFailureDetailsOutputTypeDef,
+    TagOutputTypeDef,
     CancelDataRepositoryTaskRequestRequestTypeDef,
-    CancelDataRepositoryTaskResponseTypeDef,
+    CancelDataRepositoryTaskResponseOutputTypeDef,
+    CompletionReportOutputTypeDef,
     CompletionReportTypeDef,
+    TagTypeDef,
     FileCacheLustreMetadataConfigurationTypeDef,
-    CreateFileSystemFromBackupResponseTypeDef,
+    CreateFileSystemFromBackupResponseOutputTypeDef,
     LustreLogCreateConfigurationTypeDef,
     LustreRootSquashConfigurationTypeDef,
     DiskIopsConfigurationTypeDef,
-    CreateFileSystemResponseTypeDef,
+    CreateFileSystemResponseOutputTypeDef,
     SelfManagedActiveDirectoryConfigurationTypeDef,
     WindowsAuditLogCreateConfigurationTypeDef,
     TieringPolicyTypeDef,
     CreateOpenZFSOriginSnapshotConfigurationTypeDef,
     OpenZFSUserOrGroupQuotaTypeDef,
-    DataRepositoryFailureDetailsTypeDef,
-    DataRepositoryTaskFailureDetailsTypeDef,
+    DataRepositoryFailureDetailsOutputTypeDef,
+    DataRepositoryTaskFailureDetailsOutputTypeDef,
     DataRepositoryTaskFilterTypeDef,
-    DataRepositoryTaskStatusTypeDef,
+    DataRepositoryTaskStatusOutputTypeDef,
     DeleteBackupRequestRequestTypeDef,
-    DeleteBackupResponseTypeDef,
+    DeleteBackupResponseOutputTypeDef,
     DeleteDataRepositoryAssociationRequestRequestTypeDef,
-    DeleteDataRepositoryAssociationResponseTypeDef,
+    DeleteDataRepositoryAssociationResponseOutputTypeDef,
     DeleteFileCacheRequestRequestTypeDef,
-    DeleteFileCacheResponseTypeDef,
+    DeleteFileCacheResponseOutputTypeDef,
     DeleteSnapshotRequestRequestTypeDef,
-    DeleteSnapshotResponseTypeDef,
+    DeleteSnapshotResponseOutputTypeDef,
     DeleteStorageVirtualMachineRequestRequestTypeDef,
-    DeleteStorageVirtualMachineResponseTypeDef,
+    DeleteStorageVirtualMachineResponseOutputTypeDef,
     DeleteVolumeOpenZFSConfigurationTypeDef,
     FilterTypeDef,
     DescribeFileCachesRequestRequestTypeDef,
     DescribeFileSystemAliasesRequestRequestTypeDef,
     DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef,
     DescribeFileSystemsRequestRequestTypeDef,
-    DescribeFileSystemsResponseTypeDef,
+    DescribeFileSystemsResponseOutputTypeDef,
     SnapshotFilterTypeDef,
     StorageVirtualMachineFilterTypeDef,
     VolumeFilterTypeDef,
     DisassociateFileSystemAliasesRequestRequestTypeDef,
-    FileCacheFailureDetailsTypeDef,
+    DiskIopsConfigurationOutputTypeDef,
+    FileCacheFailureDetailsOutputTypeDef,
     FileCacheNFSConfigurationTypeDef,
-    LustreLogConfigurationTypeDef,
-    FileSystemEndpointTypeDef,
-    FileSystemFailureDetailsTypeDef,
-    LifecycleTransitionReasonTypeDef,
+    FileCacheLustreMetadataConfigurationOutputTypeDef,
+    LustreLogConfigurationOutputTypeDef,
+    FileSystemEndpointOutputTypeDef,
+    FileSystemFailureDetailsOutputTypeDef,
+    LifecycleTransitionReasonOutputTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    LustreRootSquashConfigurationOutputTypeDef,
+    TieringPolicyOutputTypeDef,
+    OpenZFSClientConfigurationOutputTypeDef,
     OpenZFSClientConfigurationTypeDef,
-    OpenZFSOriginSnapshotConfigurationTypeDef,
+    OpenZFSOriginSnapshotConfigurationOutputTypeDef,
+    OpenZFSUserOrGroupQuotaOutputTypeDef,
     PaginatorConfigTypeDef,
     ReleaseFileSystemNfsV3LocksRequestRequestTypeDef,
-    ReleaseFileSystemNfsV3LocksResponseTypeDef,
+    ReleaseFileSystemNfsV3LocksResponseOutputTypeDef,
     ResponseMetadataTypeDef,
     RestoreVolumeFromSnapshotRequestRequestTypeDef,
-    RestoreVolumeFromSnapshotResponseTypeDef,
+    RestoreVolumeFromSnapshotResponseOutputTypeDef,
+    RetentionPeriodOutputTypeDef,
     RetentionPeriodTypeDef,
-    SelfManagedActiveDirectoryAttributesTypeDef,
+    SelfManagedActiveDirectoryAttributesOutputTypeDef,
     SelfManagedActiveDirectoryConfigurationUpdatesTypeDef,
-    SvmEndpointTypeDef,
+    SvmEndpointOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFileCacheLustreConfigurationTypeDef,
-    UpdateFileSystemResponseTypeDef,
+    UpdateFileSystemResponseOutputTypeDef,
     UpdateSnapshotRequestRequestTypeDef,
-    WindowsAuditLogConfigurationTypeDef,
-    AssociateFileSystemAliasesResponseTypeDef,
-    DescribeFileSystemAliasesResponseTypeDef,
-    DisassociateFileSystemAliasesResponseTypeDef,
-    NFSDataRepositoryConfigurationTypeDef,
+    WindowsAuditLogConfigurationOutputTypeDef,
+    AssociateFileSystemAliasesResponseOutputTypeDef,
+    DescribeFileSystemAliasesResponseOutputTypeDef,
+    DisassociateFileSystemAliasesResponseOutputTypeDef,
+    NFSDataRepositoryConfigurationOutputTypeDef,
+    S3DataRepositoryConfigurationOutputTypeDef,
     S3DataRepositoryConfigurationTypeDef,
+    DeleteFileSystemLustreResponseOutputTypeDef,
+    DeleteFileSystemOpenZFSResponseOutputTypeDef,
+    DeleteFileSystemWindowsResponseOutputTypeDef,
+    DeleteVolumeOntapResponseOutputTypeDef,
+    ListTagsForResourceResponseOutputTypeDef,
     CopyBackupRequestRequestTypeDef,
     CreateBackupRequestRequestTypeDef,
+    CreateDataRepositoryTaskRequestRequestTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     DeleteFileSystemLustreConfigurationTypeDef,
-    DeleteFileSystemLustreResponseTypeDef,
     DeleteFileSystemOpenZFSConfigurationTypeDef,
-    DeleteFileSystemOpenZFSResponseTypeDef,
     DeleteFileSystemWindowsConfigurationTypeDef,
-    DeleteFileSystemWindowsResponseTypeDef,
     DeleteVolumeOntapConfigurationTypeDef,
-    DeleteVolumeOntapResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    CreateDataRepositoryTaskRequestRequestTypeDef,
     CreateFileCacheLustreConfigurationTypeDef,
     CreateFileSystemLustreConfigurationTypeDef,
     UpdateFileSystemLustreConfigurationTypeDef,
     CreateFileSystemOntapConfigurationTypeDef,
-    OpenZFSFileSystemConfigurationTypeDef,
     UpdateFileSystemOntapConfigurationTypeDef,
     UpdateFileSystemOpenZFSConfigurationTypeDef,
     CreateSvmActiveDirectoryConfigurationTypeDef,
     CreateFileSystemWindowsConfigurationTypeDef,
-    DataRepositoryConfigurationTypeDef,
+    DataRepositoryConfigurationOutputTypeDef,
     DescribeDataRepositoryTasksRequestRequestTypeDef,
-    DataRepositoryTaskTypeDef,
+    DataRepositoryTaskOutputTypeDef,
     DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
     DescribeBackupsRequestRequestTypeDef,
     DescribeDataRepositoryAssociationsRequestRequestTypeDef,
     DescribeSnapshotsRequestRequestTypeDef,
     DescribeStorageVirtualMachinesRequestDescribeStorageVirtualMachinesPaginateTypeDef,
     DescribeStorageVirtualMachinesRequestRequestTypeDef,
     DescribeVolumesRequestDescribeVolumesPaginateTypeDef,
     DescribeVolumesRequestRequestTypeDef,
+    OpenZFSFileSystemConfigurationOutputTypeDef,
     FileCacheDataRepositoryAssociationTypeDef,
-    FileCacheLustreConfigurationTypeDef,
-    FileSystemEndpointsTypeDef,
-    SnapshotTypeDef,
+    FileCacheLustreConfigurationOutputTypeDef,
+    FileSystemEndpointsOutputTypeDef,
+    SnapshotOutputTypeDef,
+    OpenZFSNfsExportOutputTypeDef,
     OpenZFSNfsExportTypeDef,
+    SnaplockRetentionPeriodOutputTypeDef,
     SnaplockRetentionPeriodTypeDef,
-    SvmActiveDirectoryConfigurationTypeDef,
+    SvmActiveDirectoryConfigurationOutputTypeDef,
     UpdateFileSystemWindowsConfigurationTypeDef,
     UpdateSvmActiveDirectoryConfigurationTypeDef,
-    SvmEndpointsTypeDef,
+    SvmEndpointsOutputTypeDef,
     UpdateFileCacheRequestRequestTypeDef,
-    WindowsFileSystemConfigurationTypeDef,
+    WindowsFileSystemConfigurationOutputTypeDef,
+    DataRepositoryAssociationOutputTypeDef,
     CreateDataRepositoryAssociationRequestRequestTypeDef,
-    DataRepositoryAssociationTypeDef,
     UpdateDataRepositoryAssociationRequestRequestTypeDef,
+    DeleteFileSystemResponseOutputTypeDef,
+    DeleteVolumeResponseOutputTypeDef,
     DeleteFileSystemRequestRequestTypeDef,
-    DeleteFileSystemResponseTypeDef,
     DeleteVolumeRequestRequestTypeDef,
-    DeleteVolumeResponseTypeDef,
     CreateStorageVirtualMachineRequestRequestTypeDef,
-    LustreFileSystemConfigurationTypeDef,
-    CreateDataRepositoryTaskResponseTypeDef,
-    DescribeDataRepositoryTasksResponseTypeDef,
+    LustreFileSystemConfigurationOutputTypeDef,
+    CreateDataRepositoryTaskResponseOutputTypeDef,
+    DescribeDataRepositoryTasksResponseOutputTypeDef,
     CreateFileCacheRequestRequestTypeDef,
-    FileCacheCreatingTypeDef,
-    FileCacheTypeDef,
-    OntapFileSystemConfigurationTypeDef,
-    CreateSnapshotResponseTypeDef,
-    DescribeSnapshotsResponseTypeDef,
-    UpdateSnapshotResponseTypeDef,
+    FileCacheCreatingOutputTypeDef,
+    FileCacheOutputTypeDef,
+    OntapFileSystemConfigurationOutputTypeDef,
+    CreateSnapshotResponseOutputTypeDef,
+    DescribeSnapshotsResponseOutputTypeDef,
+    UpdateSnapshotResponseOutputTypeDef,
+    OpenZFSVolumeConfigurationOutputTypeDef,
     CreateOpenZFSVolumeConfigurationTypeDef,
     OpenZFSCreateRootVolumeConfigurationTypeDef,
-    OpenZFSVolumeConfigurationTypeDef,
     UpdateOpenZFSVolumeConfigurationTypeDef,
+    SnaplockConfigurationOutputTypeDef,
     CreateSnaplockConfigurationTypeDef,
-    SnaplockConfigurationTypeDef,
     UpdateSnaplockConfigurationTypeDef,
     UpdateFileSystemRequestRequestTypeDef,
     UpdateStorageVirtualMachineRequestRequestTypeDef,
-    StorageVirtualMachineTypeDef,
-    CreateDataRepositoryAssociationResponseTypeDef,
-    DescribeDataRepositoryAssociationsResponseTypeDef,
-    UpdateDataRepositoryAssociationResponseTypeDef,
-    CreateFileCacheResponseTypeDef,
-    DescribeFileCachesResponseTypeDef,
-    UpdateFileCacheResponseTypeDef,
-    FileSystemTypeDef,
+    StorageVirtualMachineOutputTypeDef,
+    CreateDataRepositoryAssociationResponseOutputTypeDef,
+    DescribeDataRepositoryAssociationsResponseOutputTypeDef,
+    UpdateDataRepositoryAssociationResponseOutputTypeDef,
+    CreateFileCacheResponseOutputTypeDef,
+    DescribeFileCachesResponseOutputTypeDef,
+    UpdateFileCacheResponseOutputTypeDef,
+    FileSystemOutputTypeDef,
     CreateFileSystemOpenZFSConfigurationTypeDef,
+    OntapVolumeConfigurationOutputTypeDef,
     CreateOntapVolumeConfigurationTypeDef,
-    OntapVolumeConfigurationTypeDef,
     UpdateOntapVolumeConfigurationTypeDef,
-    CreateStorageVirtualMachineResponseTypeDef,
-    DescribeStorageVirtualMachinesResponseTypeDef,
-    UpdateStorageVirtualMachineResponseTypeDef,
+    CreateStorageVirtualMachineResponseOutputTypeDef,
+    DescribeStorageVirtualMachinesResponseOutputTypeDef,
+    UpdateStorageVirtualMachineResponseOutputTypeDef,
     CreateFileSystemFromBackupRequestRequestTypeDef,
     CreateFileSystemRequestRequestTypeDef,
+    VolumeOutputTypeDef,
     CreateVolumeFromBackupRequestRequestTypeDef,
     CreateVolumeRequestRequestTypeDef,
-    VolumeTypeDef,
     UpdateVolumeRequestRequestTypeDef,
-    AdministrativeActionTypeDef,
-    BackupTypeDef,
-    CreateVolumeFromBackupResponseTypeDef,
-    CreateVolumeResponseTypeDef,
-    DescribeVolumesResponseTypeDef,
-    UpdateVolumeResponseTypeDef,
-    CopyBackupResponseTypeDef,
-    CreateBackupResponseTypeDef,
-    DescribeBackupsResponseTypeDef,
+    AdministrativeActionOutputTypeDef,
+    BackupOutputTypeDef,
+    CreateVolumeFromBackupResponseOutputTypeDef,
+    CreateVolumeResponseOutputTypeDef,
+    DescribeVolumesResponseOutputTypeDef,
+    UpdateVolumeResponseOutputTypeDef,
+    CopyBackupResponseOutputTypeDef,
+    CreateBackupResponseOutputTypeDef,
+    DescribeBackupsResponseOutputTypeDef,
 )
 
 
-def get_structure() -> ActiveDirectoryBackupAttributesTypeDef:
+def get_structure() -> ActiveDirectoryBackupAttributesOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-fsx-1.28.3/mypy_boto3_fsx.egg-info/SOURCES.txt` & `mypy-boto3-fsx-1.28.3.post1/mypy_boto3_fsx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.28.3/setup.py` & `mypy-boto3-fsx-1.28.3.post1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-fsx",
-    version="1.28.3",
+    version="1.28.3.post1",
     packages=["mypy_boto3_fsx"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.FSx 1.28.3 service generated with mypy-boto3-builder 7.14.6"
+        "Type annotations for boto3.FSx 1.28.3 service generated with mypy-boto3-builder 7.14.7"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

