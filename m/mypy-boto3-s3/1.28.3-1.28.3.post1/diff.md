# Comparing `tmp/mypy-boto3-s3-1.28.3.tar.gz` & `tmp/mypy-boto3-s3-1.28.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-s3-1.28.3.tar", last modified: Thu Jul 13 19:49:15 2023, max compression
+gzip compressed data, was "mypy-boto3-s3-1.28.3.post1.tar", last modified: Fri Jul 14 16:18:03 2023, max compression
```

## Comparing `mypy-boto3-s3-1.28.3.tar` & `mypy-boto3-s3-1.28.3.post1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:15.173303 mypy-boto3-s3-1.28.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-13 19:48:29.000000 mypy-boto3-s3-1.28.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    34064 2023-07-13 19:49:15.169303 mypy-boto3-s3-1.28.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    32599 2023-07-13 19:48:29.000000 mypy-boto3-s3-1.28.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:15.157302 mypy-boto3-s3-1.28.3/mypy_boto3_s3/
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-13 19:48:29.000000 mypy-boto3-s3-1.28.3/mypy_boto3_s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-13 19:48:29.000000 mypy-boto3-s3-1.28.3/mypy_boto3_s3/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-13 19:48:29.000000 mypy-boto3-s3-1.28.3/mypy_boto3_s3/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    83859 2023-07-13 19:48:30.000000 mypy-boto3-s3-1.28.3/mypy_boto3_s3/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    83740 2023-07-13 19:48:29.000000 mypy-boto3-s3-1.28.3/mypy_boto3_s3/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16604 2023-07-13 19:48:32.000000 mypy-boto3-s3-1.28.3/mypy_boto3_s3/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    16602 2023-07-13 19:48:32.000000 mypy-boto3-s3-1.28.3/mypy_boto3_s3/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-07-13 19:48:31.000000 mypy-boto3-s3-1.28.3/mypy_boto3_s3/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-07-13 19:48:31.000000 mypy-boto3-s3-1.28.3/mypy_boto3_s3/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:48:29.000000 mypy-boto3-s3-1.28.3/mypy_boto3_s3/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   117751 2023-07-13 19:48:31.000000 mypy-boto3-s3-1.28.3/mypy_boto3_s3/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)   117535 2023-07-13 19:48:31.000000 mypy-boto3-s3-1.28.3/mypy_boto3_s3/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   178932 2023-07-13 19:48:37.000000 mypy-boto3-s3-1.28.3/mypy_boto3_s3/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   178660 2023-07-13 19:48:34.000000 mypy-boto3-s3-1.28.3/mypy_boto3_s3/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 19:48:29.000000 mypy-boto3-s3-1.28.3/mypy_boto3_s3/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-07-13 19:48:31.000000 mypy-boto3-s3-1.28.3/mypy_boto3_s3/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-07-13 19:48:31.000000 mypy-boto3-s3-1.28.3/mypy_boto3_s3/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:49:15.169303 mypy-boto3-s3-1.28.3/mypy_boto3_s3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    34064 2023-07-13 19:49:15.000000 mypy-boto3-s3-1.28.3/mypy_boto3_s3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-13 19:49:15.000000 mypy-boto3-s3-1.28.3/mypy_boto3_s3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:15.000000 mypy-boto3-s3-1.28.3/mypy_boto3_s3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:49:15.000000 mypy-boto3-s3-1.28.3/mypy_boto3_s3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-13 19:49:15.000000 mypy-boto3-s3-1.28.3/mypy_boto3_s3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-13 19:49:15.000000 mypy-boto3-s3-1.28.3/mypy_boto3_s3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 19:49:15.173303 mypy-boto3-s3-1.28.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-13 19:48:29.000000 mypy-boto3-s3-1.28.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:18:03.011732 mypy-boto3-s3-1.28.3.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-14 16:17:04.000000 mypy-boto3-s3-1.28.3.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    37496 2023-07-14 16:18:03.011732 mypy-boto3-s3-1.28.3.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    36025 2023-07-14 16:17:04.000000 mypy-boto3-s3-1.28.3.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:18:03.003731 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-14 16:17:04.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-14 16:17:04.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-14 16:17:04.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84515 2023-07-14 16:17:05.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84396 2023-07-14 16:17:05.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16604 2023-07-14 16:17:08.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16602 2023-07-14 16:17:08.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7386 2023-07-14 16:17:07.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-07-14 16:17:07.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:04.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   118063 2023-07-14 16:17:07.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)   117847 2023-07-14 16:17:06.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   206191 2023-07-14 16:17:13.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   205879 2023-07-14 16:17:11.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-14 16:17:04.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-07-14 16:17:07.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-07-14 16:17:07.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:18:03.011732 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    37496 2023-07-14 16:18:02.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-14 16:18:02.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:18:02.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:18:02.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-14 16:18:02.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-14 16:18:02.000000 mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 16:18:03.011732 mypy-boto3-s3-1.28.3.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-14 16:17:04.000000 mypy-boto3-s3-1.28.3.post1/setup.py
```

### Comparing `mypy-boto3-s3-1.28.3/LICENSE` & `mypy-boto3-s3-1.28.3.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.28.3/PKG-INFO` & `mypy-boto3-s3-1.28.3.post1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-s3
-Version: 1.28.3
-Summary: Type annotations for boto3.S3 1.28.3 service generated with mypy-boto3-builder 7.14.6
+Version: 1.28.3.post1
+Summary: Type annotations for boto3.S3 1.28.3 service generated with mypy-boto3-builder 7.14.7
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/
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
 [mypy-boto3-s3 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/).
 
 See how it helps to find and fix potential bugs:
 
@@ -551,53 +551,61 @@
 ### Typed dictionaries
 
 `mypy_boto3_s3.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_s3.type_defs import (
+    AbortIncompleteMultipartUploadOutputTypeDef,
     AbortIncompleteMultipartUploadTypeDef,
-    AbortMultipartUploadOutputTypeDef,
+    AbortMultipartUploadOutputOutputTypeDef,
     AbortMultipartUploadRequestMultipartUploadAbortTypeDef,
     AbortMultipartUploadRequestRequestTypeDef,
     AccelerateConfigurationTypeDef,
     OwnerTypeDef,
+    AccessControlTranslationOutputTypeDef,
     AccessControlTranslationTypeDef,
+    TagOutputTypeDef,
     TagTypeDef,
+    AnalyticsS3BucketDestinationOutputTypeDef,
     AnalyticsS3BucketDestinationTypeDef,
     CopySourceTypeDef,
     BucketDownloadFileRequestTypeDef,
     BucketDownloadFileobjRequestTypeDef,
-    BucketTypeDef,
+    BucketOutputTypeDef,
     BucketUploadFileRequestTypeDef,
     BucketUploadFileobjRequestTypeDef,
     CORSRuleTypeDef,
+    CORSRuleOutputTypeDef,
     CSVInputTypeDef,
     CSVOutputTypeDef,
-    ChecksumTypeDef,
+    ChecksumOutputTypeDef,
     ClientDownloadFileRequestTypeDef,
     ClientDownloadFileobjRequestTypeDef,
     ClientGeneratePresignedPostRequestTypeDef,
     ClientUploadFileRequestTypeDef,
     ClientUploadFileobjRequestTypeDef,
+    CloudFunctionConfigurationOutputTypeDef,
     CloudFunctionConfigurationTypeDef,
-    CommonPrefixTypeDef,
-    CompleteMultipartUploadOutputTypeDef,
+    CommonPrefixOutputTypeDef,
+    CompleteMultipartUploadOutputOutputTypeDef,
     CompletedPartTypeDef,
+    ConditionOutputTypeDef,
     ConditionTypeDef,
-    CopyObjectResultTypeDef,
+    CopyObjectResultOutputTypeDef,
     CopyObjectRequestObjectCopyFromTypeDef,
     CopyObjectRequestObjectSummaryCopyFromTypeDef,
-    CopyPartResultTypeDef,
+    CopyPartResultOutputTypeDef,
     CreateBucketConfigurationTypeDef,
-    CreateBucketOutputTypeDef,
-    CreateMultipartUploadOutputTypeDef,
+    CreateBucketOutputOutputTypeDef,
+    CreateMultipartUploadOutputOutputTypeDef,
     CreateMultipartUploadRequestObjectInitiateMultipartUploadTypeDef,
     CreateMultipartUploadRequestObjectSummaryInitiateMultipartUploadTypeDef,
     CreateMultipartUploadRequestRequestTypeDef,
+    DefaultRetentionOutputTypeDef,
     DefaultRetentionTypeDef,
     DeleteBucketAnalyticsConfigurationRequestRequestTypeDef,
     DeleteBucketCorsRequestBucketCorsDeleteTypeDef,
     DeleteBucketCorsRequestRequestTypeDef,
     DeleteBucketEncryptionRequestRequestTypeDef,
     DeleteBucketIntelligentTieringConfigurationRequestRequestTypeDef,
     DeleteBucketInventoryConfigurationRequestRequestTypeDef,
@@ -611,97 +619,113 @@
     DeleteBucketReplicationRequestRequestTypeDef,
     DeleteBucketRequestBucketDeleteTypeDef,
     DeleteBucketRequestRequestTypeDef,
     DeleteBucketTaggingRequestBucketTaggingDeleteTypeDef,
     DeleteBucketTaggingRequestRequestTypeDef,
     DeleteBucketWebsiteRequestBucketWebsiteDeleteTypeDef,
     DeleteBucketWebsiteRequestRequestTypeDef,
+    OwnerOutputTypeDef,
+    DeleteMarkerReplicationOutputTypeDef,
     DeleteMarkerReplicationTypeDef,
-    DeleteObjectOutputTypeDef,
+    DeleteObjectOutputOutputTypeDef,
     DeleteObjectRequestObjectDeleteTypeDef,
     DeleteObjectRequestObjectSummaryDeleteTypeDef,
     DeleteObjectRequestObjectVersionDeleteTypeDef,
     DeleteObjectRequestRequestTypeDef,
-    DeleteObjectTaggingOutputTypeDef,
+    DeleteObjectTaggingOutputOutputTypeDef,
     DeleteObjectTaggingRequestRequestTypeDef,
-    DeletedObjectTypeDef,
-    ErrorTypeDef,
+    DeletedObjectOutputTypeDef,
+    ErrorOutputTypeDef,
     DeletePublicAccessBlockRequestRequestTypeDef,
     ObjectIdentifierTypeDef,
+    EncryptionConfigurationOutputTypeDef,
     EncryptionConfigurationTypeDef,
     EmptyResponseMetadataTypeDef,
     EncryptionTypeDef,
+    ErrorDocumentOutputTypeDef,
     ErrorDocumentResponseMetadataTypeDef,
     ErrorDocumentTypeDef,
+    ExistingObjectReplicationOutputTypeDef,
     ExistingObjectReplicationTypeDef,
+    FilterRuleOutputTypeDef,
     FilterRuleTypeDef,
-    GetBucketAccelerateConfigurationOutputTypeDef,
+    GetBucketAccelerateConfigurationOutputOutputTypeDef,
     GetBucketAccelerateConfigurationRequestRequestTypeDef,
     GetBucketAclRequestRequestTypeDef,
     GetBucketAnalyticsConfigurationRequestRequestTypeDef,
     GetBucketCorsRequestRequestTypeDef,
     GetBucketEncryptionRequestRequestTypeDef,
     GetBucketIntelligentTieringConfigurationRequestRequestTypeDef,
     GetBucketInventoryConfigurationRequestRequestTypeDef,
     GetBucketLifecycleConfigurationRequestRequestTypeDef,
     GetBucketLifecycleRequestRequestTypeDef,
-    GetBucketLocationOutputTypeDef,
+    GetBucketLocationOutputOutputTypeDef,
     GetBucketLocationRequestRequestTypeDef,
     GetBucketLoggingRequestRequestTypeDef,
     GetBucketMetricsConfigurationRequestRequestTypeDef,
     GetBucketNotificationConfigurationRequestRequestTypeDef,
     GetBucketOwnershipControlsRequestRequestTypeDef,
-    GetBucketPolicyOutputTypeDef,
+    GetBucketPolicyOutputOutputTypeDef,
     GetBucketPolicyRequestRequestTypeDef,
-    PolicyStatusTypeDef,
+    PolicyStatusOutputTypeDef,
     GetBucketPolicyStatusRequestRequestTypeDef,
     GetBucketReplicationRequestRequestTypeDef,
-    GetBucketRequestPaymentOutputTypeDef,
+    GetBucketRequestPaymentOutputOutputTypeDef,
     GetBucketRequestPaymentRequestRequestTypeDef,
     GetBucketTaggingRequestRequestTypeDef,
-    GetBucketVersioningOutputTypeDef,
+    GetBucketVersioningOutputOutputTypeDef,
     GetBucketVersioningRequestRequestTypeDef,
-    IndexDocumentTypeDef,
-    RedirectAllRequestsToTypeDef,
+    IndexDocumentOutputTypeDef,
+    RedirectAllRequestsToOutputTypeDef,
     GetBucketWebsiteRequestRequestTypeDef,
     GetObjectAclRequestRequestTypeDef,
-    ObjectPartTypeDef,
+    ObjectPartOutputTypeDef,
     GetObjectAttributesRequestRequestTypeDef,
-    ObjectLockLegalHoldTypeDef,
+    ObjectLockLegalHoldOutputTypeDef,
     GetObjectLegalHoldRequestRequestTypeDef,
     GetObjectLockConfigurationRequestRequestTypeDef,
-    GetObjectOutputTypeDef,
+    GetObjectOutputOutputTypeDef,
     GetObjectRequestObjectGetTypeDef,
     GetObjectRequestObjectSummaryGetTypeDef,
     GetObjectRequestObjectVersionGetTypeDef,
     GetObjectRequestRequestTypeDef,
-    ObjectLockRetentionTypeDef,
+    ObjectLockRetentionOutputTypeDef,
     GetObjectRetentionRequestRequestTypeDef,
     GetObjectTaggingRequestRequestTypeDef,
-    GetObjectTorrentOutputTypeDef,
+    GetObjectTorrentOutputOutputTypeDef,
     GetObjectTorrentRequestRequestTypeDef,
-    PublicAccessBlockConfigurationTypeDef,
+    PublicAccessBlockConfigurationOutputTypeDef,
     GetPublicAccessBlockRequestRequestTypeDef,
     GlacierJobParametersTypeDef,
+    GranteeOutputTypeDef,
     GranteeTypeDef,
     WaiterConfigTypeDef,
     HeadBucketRequestRequestTypeDef,
-    HeadObjectOutputTypeDef,
+    HeadObjectOutputOutputTypeDef,
     HeadObjectRequestObjectVersionHeadTypeDef,
     HeadObjectRequestRequestTypeDef,
     IndexDocumentResponseMetadataTypeDef,
+    IndexDocumentTypeDef,
+    InitiatorOutputTypeDef,
     InitiatorResponseMetadataTypeDef,
-    InitiatorTypeDef,
     JSONInputTypeDef,
+    TieringOutputTypeDef,
     TieringTypeDef,
+    InventoryFilterOutputTypeDef,
+    InventoryScheduleOutputTypeDef,
     InventoryFilterTypeDef,
     InventoryScheduleTypeDef,
+    SSEKMSOutputTypeDef,
     SSEKMSTypeDef,
     JSONOutputTypeDef,
+    LifecycleExpirationOutputTypeDef,
     LifecycleExpirationTypeDef,
+    NoncurrentVersionExpirationOutputTypeDef,
+    NoncurrentVersionTransitionOutputTypeDef,
+    TransitionOutputTypeDef,
     NoncurrentVersionExpirationTypeDef,
     NoncurrentVersionTransitionTypeDef,
     TransitionTypeDef,
     ListBucketAnalyticsConfigurationsRequestRequestTypeDef,
     ListBucketIntelligentTieringConfigurationsRequestRequestTypeDef,
     ListBucketInventoryConfigurationsRequestRequestTypeDef,
     ListBucketMetricsConfigurationsRequestRequestTypeDef,
@@ -709,229 +733,283 @@
     ListMultipartUploadsRequestRequestTypeDef,
     ListObjectVersionsRequestListObjectVersionsPaginateTypeDef,
     ListObjectVersionsRequestRequestTypeDef,
     ListObjectsRequestListObjectsPaginateTypeDef,
     ListObjectsRequestRequestTypeDef,
     ListObjectsV2RequestListObjectsV2PaginateTypeDef,
     ListObjectsV2RequestRequestTypeDef,
-    PartTypeDef,
+    PartOutputTypeDef,
     ListPartsRequestListPartsPaginateTypeDef,
     ListPartsRequestRequestTypeDef,
     MetadataEntryTypeDef,
+    ReplicationTimeValueOutputTypeDef,
     ReplicationTimeValueTypeDef,
+    QueueConfigurationDeprecatedOutputTypeDef,
+    TopicConfigurationDeprecatedOutputTypeDef,
     QueueConfigurationDeprecatedTypeDef,
     TopicConfigurationDeprecatedTypeDef,
     ObjectDownloadFileRequestTypeDef,
     ObjectDownloadFileobjRequestTypeDef,
-    RestoreStatusTypeDef,
+    ObjectLockLegalHoldTypeDef,
+    ObjectLockRetentionTypeDef,
+    RestoreStatusOutputTypeDef,
     ObjectUploadFileRequestTypeDef,
     ObjectUploadFileobjRequestTypeDef,
     OwnerResponseMetadataTypeDef,
+    OwnershipControlsRuleOutputTypeDef,
     OwnershipControlsRuleTypeDef,
     PaginatorConfigTypeDef,
-    ProgressTypeDef,
+    ProgressOutputTypeDef,
+    PublicAccessBlockConfigurationTypeDef,
     PutBucketPolicyRequestBucketPolicyPutTypeDef,
     PutBucketPolicyRequestRequestTypeDef,
     RequestPaymentConfigurationTypeDef,
     PutBucketVersioningRequestBucketVersioningEnableTypeDef,
     VersioningConfigurationTypeDef,
     PutBucketVersioningRequestBucketVersioningSuspendTypeDef,
-    PutObjectAclOutputTypeDef,
-    PutObjectLegalHoldOutputTypeDef,
-    PutObjectLockConfigurationOutputTypeDef,
-    PutObjectOutputTypeDef,
+    PutObjectAclOutputOutputTypeDef,
+    PutObjectLegalHoldOutputOutputTypeDef,
+    PutObjectLockConfigurationOutputOutputTypeDef,
+    PutObjectOutputOutputTypeDef,
     PutObjectRequestBucketPutObjectTypeDef,
     PutObjectRequestObjectPutTypeDef,
     PutObjectRequestObjectSummaryPutTypeDef,
     PutObjectRequestRequestTypeDef,
-    PutObjectRetentionOutputTypeDef,
-    PutObjectTaggingOutputTypeDef,
-    RecordsEventTypeDef,
+    PutObjectRetentionOutputOutputTypeDef,
+    PutObjectTaggingOutputOutputTypeDef,
+    RecordsEventOutputTypeDef,
     RedirectAllRequestsToResponseMetadataTypeDef,
+    RedirectAllRequestsToTypeDef,
+    RedirectOutputTypeDef,
     RedirectTypeDef,
+    ReplicaModificationsOutputTypeDef,
     ReplicaModificationsTypeDef,
     RequestProgressTypeDef,
     ResponseMetadataTypeDef,
-    RestoreObjectOutputTypeDef,
+    RestoreObjectOutputOutputTypeDef,
     RestoreStatusResponseMetadataTypeDef,
     ScanRangeTypeDef,
+    ServerSideEncryptionByDefaultOutputTypeDef,
     ServerSideEncryptionByDefaultTypeDef,
+    SseKmsEncryptedObjectsOutputTypeDef,
     SseKmsEncryptedObjectsTypeDef,
-    StatsTypeDef,
-    UploadPartOutputTypeDef,
+    StatsOutputTypeDef,
+    UploadPartOutputOutputTypeDef,
     UploadPartRequestMultipartUploadPartUploadTypeDef,
     UploadPartRequestRequestTypeDef,
     WriteGetObjectResponseRequestRequestTypeDef,
     PutBucketAccelerateConfigurationRequestRequestTypeDef,
-    DeleteMarkerEntryTypeDef,
+    AnalyticsAndOperatorOutputTypeDef,
+    GetBucketTaggingOutputOutputTypeDef,
+    GetObjectTaggingOutputOutputTypeDef,
+    IntelligentTieringAndOperatorOutputTypeDef,
+    LifecycleRuleAndOperatorOutputTypeDef,
+    MetricsAndOperatorOutputTypeDef,
+    ReplicationRuleAndOperatorOutputTypeDef,
     AnalyticsAndOperatorTypeDef,
-    GetBucketTaggingOutputTypeDef,
-    GetObjectTaggingOutputTypeDef,
     IntelligentTieringAndOperatorTypeDef,
     LifecycleRuleAndOperatorTypeDef,
     MetricsAndOperatorTypeDef,
     ReplicationRuleAndOperatorTypeDef,
     TaggingTypeDef,
+    AnalyticsExportDestinationOutputTypeDef,
     AnalyticsExportDestinationTypeDef,
     BucketCopyRequestTypeDef,
     ClientCopyRequestTypeDef,
     CopyObjectRequestRequestTypeDef,
     ObjectCopyRequestTypeDef,
     UploadPartCopyRequestMultipartUploadPartCopyFromTypeDef,
     UploadPartCopyRequestRequestTypeDef,
-    ListBucketsOutputTypeDef,
     CORSConfigurationTypeDef,
-    GetBucketCorsOutputTypeDef,
+    GetBucketCorsOutputOutputTypeDef,
     CompletedMultipartUploadTypeDef,
-    CopyObjectOutputTypeDef,
-    UploadPartCopyOutputTypeDef,
+    CopyObjectOutputOutputTypeDef,
+    UploadPartCopyOutputOutputTypeDef,
     CreateBucketRequestBucketCreateTypeDef,
     CreateBucketRequestRequestTypeDef,
     CreateBucketRequestServiceResourceCreateBucketTypeDef,
+    ObjectLockRuleOutputTypeDef,
     ObjectLockRuleTypeDef,
-    DeleteObjectsOutputTypeDef,
+    DeleteMarkerEntryOutputTypeDef,
+    ListBucketsOutputOutputTypeDef,
+    DeleteObjectsOutputOutputTypeDef,
     DeleteTypeDef,
+    S3KeyFilterOutputTypeDef,
     S3KeyFilterTypeDef,
-    GetBucketPolicyStatusOutputTypeDef,
-    GetObjectAttributesPartsTypeDef,
-    GetObjectLegalHoldOutputTypeDef,
-    PutObjectLegalHoldRequestRequestTypeDef,
-    GetObjectRetentionOutputTypeDef,
-    PutObjectRetentionRequestRequestTypeDef,
-    GetPublicAccessBlockOutputTypeDef,
-    PutPublicAccessBlockRequestRequestTypeDef,
+    GetBucketPolicyStatusOutputOutputTypeDef,
+    GetObjectAttributesPartsOutputTypeDef,
+    GetObjectLegalHoldOutputOutputTypeDef,
+    GetObjectRetentionOutputOutputTypeDef,
+    GetPublicAccessBlockOutputOutputTypeDef,
+    GrantOutputTypeDef,
+    TargetGrantOutputTypeDef,
     GrantTypeDef,
     TargetGrantTypeDef,
     HeadBucketRequestBucketExistsWaitTypeDef,
     HeadBucketRequestBucketNotExistsWaitTypeDef,
     HeadObjectRequestObjectExistsWaitTypeDef,
     HeadObjectRequestObjectNotExistsWaitTypeDef,
-    MultipartUploadTypeDef,
+    MultipartUploadOutputTypeDef,
     InputSerializationTypeDef,
+    InventoryEncryptionOutputTypeDef,
     InventoryEncryptionTypeDef,
     OutputSerializationTypeDef,
+    RuleOutputTypeDef,
     RuleTypeDef,
-    ListPartsOutputTypeDef,
+    ListPartsOutputOutputTypeDef,
+    MetricsOutputTypeDef,
+    ReplicationTimeOutputTypeDef,
     MetricsTypeDef,
     ReplicationTimeTypeDef,
-    NotificationConfigurationDeprecatedResponseMetadataTypeDef,
+    NotificationConfigurationDeprecatedOutputTypeDef,
     NotificationConfigurationDeprecatedTypeDef,
-    ObjectTypeDef,
-    ObjectVersionTypeDef,
+    PutObjectLegalHoldRequestRequestTypeDef,
+    PutObjectRetentionRequestRequestTypeDef,
+    ObjectOutputTypeDef,
+    ObjectVersionOutputTypeDef,
+    OwnershipControlsOutputTypeDef,
     OwnershipControlsTypeDef,
-    ProgressEventTypeDef,
+    ProgressEventOutputTypeDef,
+    PutPublicAccessBlockRequestRequestTypeDef,
     PutBucketRequestPaymentRequestBucketRequestPaymentPutTypeDef,
     PutBucketRequestPaymentRequestRequestTypeDef,
     PutBucketVersioningRequestBucketVersioningPutTypeDef,
     PutBucketVersioningRequestRequestTypeDef,
+    RoutingRuleOutputTypeDef,
     RoutingRuleTypeDef,
+    ServerSideEncryptionRuleOutputTypeDef,
     ServerSideEncryptionRuleTypeDef,
+    SourceSelectionCriteriaOutputTypeDef,
     SourceSelectionCriteriaTypeDef,
-    StatsEventTypeDef,
+    StatsEventOutputTypeDef,
+    AnalyticsFilterOutputTypeDef,
+    IntelligentTieringFilterOutputTypeDef,
+    LifecycleRuleFilterOutputTypeDef,
+    MetricsFilterOutputTypeDef,
+    ReplicationRuleFilterOutputTypeDef,
     AnalyticsFilterTypeDef,
     IntelligentTieringFilterTypeDef,
     LifecycleRuleFilterTypeDef,
     MetricsFilterTypeDef,
     ReplicationRuleFilterTypeDef,
     PutBucketTaggingRequestBucketTaggingPutTypeDef,
     PutBucketTaggingRequestRequestTypeDef,
     PutObjectTaggingRequestRequestTypeDef,
+    StorageClassAnalysisDataExportOutputTypeDef,
     StorageClassAnalysisDataExportTypeDef,
     PutBucketCorsRequestBucketCorsPutTypeDef,
     PutBucketCorsRequestRequestTypeDef,
     CompleteMultipartUploadRequestMultipartUploadCompleteTypeDef,
     CompleteMultipartUploadRequestRequestTypeDef,
+    ObjectLockConfigurationOutputTypeDef,
     ObjectLockConfigurationTypeDef,
     DeleteObjectsRequestBucketDeleteObjectsTypeDef,
     DeleteObjectsRequestRequestTypeDef,
+    NotificationConfigurationFilterOutputTypeDef,
     NotificationConfigurationFilterTypeDef,
-    GetObjectAttributesOutputTypeDef,
+    GetObjectAttributesOutputOutputTypeDef,
+    GetBucketAclOutputOutputTypeDef,
+    GetObjectAclOutputOutputTypeDef,
+    LoggingEnabledOutputTypeDef,
+    LoggingEnabledResponseMetadataTypeDef,
     AccessControlPolicyTypeDef,
-    GetBucketAclOutputTypeDef,
-    GetObjectAclOutputTypeDef,
     S3LocationTypeDef,
-    LoggingEnabledResponseMetadataTypeDef,
     LoggingEnabledTypeDef,
-    ListMultipartUploadsOutputTypeDef,
+    ListMultipartUploadsOutputOutputTypeDef,
+    InventoryS3BucketDestinationOutputTypeDef,
     InventoryS3BucketDestinationTypeDef,
     SelectObjectContentRequestRequestTypeDef,
     SelectParametersTypeDef,
-    GetBucketLifecycleOutputTypeDef,
+    GetBucketLifecycleOutputOutputTypeDef,
     LifecycleConfigurationTypeDef,
+    DestinationOutputTypeDef,
     DestinationTypeDef,
     PutBucketNotificationRequestRequestTypeDef,
-    ListObjectsOutputTypeDef,
-    ListObjectsV2OutputTypeDef,
-    ListObjectVersionsOutputTypeDef,
-    GetBucketOwnershipControlsOutputTypeDef,
+    ListObjectsOutputOutputTypeDef,
+    ListObjectsV2OutputOutputTypeDef,
+    ListObjectVersionsOutputOutputTypeDef,
+    GetBucketOwnershipControlsOutputOutputTypeDef,
     PutBucketOwnershipControlsRequestRequestTypeDef,
-    GetBucketWebsiteOutputTypeDef,
+    GetBucketWebsiteOutputOutputTypeDef,
     WebsiteConfigurationTypeDef,
+    ServerSideEncryptionConfigurationOutputTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
-    SelectObjectContentEventStreamTypeDef,
+    SelectObjectContentEventStreamOutputTypeDef,
+    IntelligentTieringConfigurationOutputTypeDef,
+    LifecycleRuleOutputTypeDef,
+    MetricsConfigurationOutputTypeDef,
     IntelligentTieringConfigurationTypeDef,
     LifecycleRuleTypeDef,
     MetricsConfigurationTypeDef,
+    StorageClassAnalysisOutputTypeDef,
     StorageClassAnalysisTypeDef,
-    GetObjectLockConfigurationOutputTypeDef,
+    GetObjectLockConfigurationOutputOutputTypeDef,
     PutObjectLockConfigurationRequestRequestTypeDef,
+    LambdaFunctionConfigurationOutputTypeDef,
+    QueueConfigurationOutputTypeDef,
+    TopicConfigurationOutputTypeDef,
     LambdaFunctionConfigurationTypeDef,
     QueueConfigurationTypeDef,
     TopicConfigurationTypeDef,
+    GetBucketLoggingOutputOutputTypeDef,
     PutBucketAclRequestBucketAclPutTypeDef,
     PutBucketAclRequestRequestTypeDef,
     PutObjectAclRequestObjectAclPutTypeDef,
     PutObjectAclRequestRequestTypeDef,
     OutputLocationTypeDef,
     BucketLoggingStatusTypeDef,
-    GetBucketLoggingOutputTypeDef,
+    InventoryDestinationOutputTypeDef,
     InventoryDestinationTypeDef,
     PutBucketLifecycleRequestBucketLifecyclePutTypeDef,
     PutBucketLifecycleRequestRequestTypeDef,
+    ReplicationRuleOutputTypeDef,
     ReplicationRuleTypeDef,
     PutBucketWebsiteRequestBucketWebsitePutTypeDef,
     PutBucketWebsiteRequestRequestTypeDef,
-    GetBucketEncryptionOutputTypeDef,
+    GetBucketEncryptionOutputOutputTypeDef,
     PutBucketEncryptionRequestRequestTypeDef,
-    SelectObjectContentOutputTypeDef,
-    GetBucketIntelligentTieringConfigurationOutputTypeDef,
-    ListBucketIntelligentTieringConfigurationsOutputTypeDef,
+    SelectObjectContentOutputOutputTypeDef,
+    GetBucketIntelligentTieringConfigurationOutputOutputTypeDef,
+    ListBucketIntelligentTieringConfigurationsOutputOutputTypeDef,
+    GetBucketLifecycleConfigurationOutputOutputTypeDef,
+    GetBucketMetricsConfigurationOutputOutputTypeDef,
+    ListBucketMetricsConfigurationsOutputOutputTypeDef,
     PutBucketIntelligentTieringConfigurationRequestRequestTypeDef,
     BucketLifecycleConfigurationTypeDef,
-    GetBucketLifecycleConfigurationOutputTypeDef,
-    GetBucketMetricsConfigurationOutputTypeDef,
-    ListBucketMetricsConfigurationsOutputTypeDef,
     PutBucketMetricsConfigurationRequestRequestTypeDef,
+    AnalyticsConfigurationOutputTypeDef,
     AnalyticsConfigurationTypeDef,
-    NotificationConfigurationResponseMetadataTypeDef,
+    NotificationConfigurationOutputTypeDef,
     NotificationConfigurationTypeDef,
     RestoreRequestTypeDef,
     PutBucketLoggingRequestBucketLoggingPutTypeDef,
     PutBucketLoggingRequestRequestTypeDef,
+    InventoryConfigurationOutputTypeDef,
     InventoryConfigurationTypeDef,
+    ReplicationConfigurationOutputTypeDef,
     ReplicationConfigurationTypeDef,
     PutBucketLifecycleConfigurationRequestBucketLifecycleConfigurationPutTypeDef,
     PutBucketLifecycleConfigurationRequestRequestTypeDef,
-    GetBucketAnalyticsConfigurationOutputTypeDef,
-    ListBucketAnalyticsConfigurationsOutputTypeDef,
+    GetBucketAnalyticsConfigurationOutputOutputTypeDef,
+    ListBucketAnalyticsConfigurationsOutputOutputTypeDef,
     PutBucketAnalyticsConfigurationRequestRequestTypeDef,
     PutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef,
     PutBucketNotificationConfigurationRequestRequestTypeDef,
     RestoreObjectRequestObjectRestoreObjectTypeDef,
     RestoreObjectRequestObjectSummaryRestoreObjectTypeDef,
     RestoreObjectRequestRequestTypeDef,
-    GetBucketInventoryConfigurationOutputTypeDef,
-    ListBucketInventoryConfigurationsOutputTypeDef,
+    GetBucketInventoryConfigurationOutputOutputTypeDef,
+    ListBucketInventoryConfigurationsOutputOutputTypeDef,
     PutBucketInventoryConfigurationRequestRequestTypeDef,
-    GetBucketReplicationOutputTypeDef,
+    GetBucketReplicationOutputOutputTypeDef,
     PutBucketReplicationRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AbortIncompleteMultipartUploadTypeDef:
+def get_structure() -> AbortIncompleteMultipartUploadOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-s3-1.28.3/README.md` & `mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-s3
+Version: 1.28.3.post1
+Summary: Type annotations for boto3.S3 1.28.3 service generated with mypy-boto3-builder 7.14.7
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 s3 type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-s3"></a>
 
 # mypy-boto3-s3
 
 [![PyPI - mypy-boto3-s3](https://img.shields.io/pypi/v/mypy-boto3-s3.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/)
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
 [mypy-boto3-s3 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/).
 
 See how it helps to find and fix potential bugs:
 
@@ -519,53 +551,61 @@
 ### Typed dictionaries
 
 `mypy_boto3_s3.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_s3.type_defs import (
+    AbortIncompleteMultipartUploadOutputTypeDef,
     AbortIncompleteMultipartUploadTypeDef,
-    AbortMultipartUploadOutputTypeDef,
+    AbortMultipartUploadOutputOutputTypeDef,
     AbortMultipartUploadRequestMultipartUploadAbortTypeDef,
     AbortMultipartUploadRequestRequestTypeDef,
     AccelerateConfigurationTypeDef,
     OwnerTypeDef,
+    AccessControlTranslationOutputTypeDef,
     AccessControlTranslationTypeDef,
+    TagOutputTypeDef,
     TagTypeDef,
+    AnalyticsS3BucketDestinationOutputTypeDef,
     AnalyticsS3BucketDestinationTypeDef,
     CopySourceTypeDef,
     BucketDownloadFileRequestTypeDef,
     BucketDownloadFileobjRequestTypeDef,
-    BucketTypeDef,
+    BucketOutputTypeDef,
     BucketUploadFileRequestTypeDef,
     BucketUploadFileobjRequestTypeDef,
     CORSRuleTypeDef,
+    CORSRuleOutputTypeDef,
     CSVInputTypeDef,
     CSVOutputTypeDef,
-    ChecksumTypeDef,
+    ChecksumOutputTypeDef,
     ClientDownloadFileRequestTypeDef,
     ClientDownloadFileobjRequestTypeDef,
     ClientGeneratePresignedPostRequestTypeDef,
     ClientUploadFileRequestTypeDef,
     ClientUploadFileobjRequestTypeDef,
+    CloudFunctionConfigurationOutputTypeDef,
     CloudFunctionConfigurationTypeDef,
-    CommonPrefixTypeDef,
-    CompleteMultipartUploadOutputTypeDef,
+    CommonPrefixOutputTypeDef,
+    CompleteMultipartUploadOutputOutputTypeDef,
     CompletedPartTypeDef,
+    ConditionOutputTypeDef,
     ConditionTypeDef,
-    CopyObjectResultTypeDef,
+    CopyObjectResultOutputTypeDef,
     CopyObjectRequestObjectCopyFromTypeDef,
     CopyObjectRequestObjectSummaryCopyFromTypeDef,
-    CopyPartResultTypeDef,
+    CopyPartResultOutputTypeDef,
     CreateBucketConfigurationTypeDef,
-    CreateBucketOutputTypeDef,
-    CreateMultipartUploadOutputTypeDef,
+    CreateBucketOutputOutputTypeDef,
+    CreateMultipartUploadOutputOutputTypeDef,
     CreateMultipartUploadRequestObjectInitiateMultipartUploadTypeDef,
     CreateMultipartUploadRequestObjectSummaryInitiateMultipartUploadTypeDef,
     CreateMultipartUploadRequestRequestTypeDef,
+    DefaultRetentionOutputTypeDef,
     DefaultRetentionTypeDef,
     DeleteBucketAnalyticsConfigurationRequestRequestTypeDef,
     DeleteBucketCorsRequestBucketCorsDeleteTypeDef,
     DeleteBucketCorsRequestRequestTypeDef,
     DeleteBucketEncryptionRequestRequestTypeDef,
     DeleteBucketIntelligentTieringConfigurationRequestRequestTypeDef,
     DeleteBucketInventoryConfigurationRequestRequestTypeDef,
@@ -579,97 +619,113 @@
     DeleteBucketReplicationRequestRequestTypeDef,
     DeleteBucketRequestBucketDeleteTypeDef,
     DeleteBucketRequestRequestTypeDef,
     DeleteBucketTaggingRequestBucketTaggingDeleteTypeDef,
     DeleteBucketTaggingRequestRequestTypeDef,
     DeleteBucketWebsiteRequestBucketWebsiteDeleteTypeDef,
     DeleteBucketWebsiteRequestRequestTypeDef,
+    OwnerOutputTypeDef,
+    DeleteMarkerReplicationOutputTypeDef,
     DeleteMarkerReplicationTypeDef,
-    DeleteObjectOutputTypeDef,
+    DeleteObjectOutputOutputTypeDef,
     DeleteObjectRequestObjectDeleteTypeDef,
     DeleteObjectRequestObjectSummaryDeleteTypeDef,
     DeleteObjectRequestObjectVersionDeleteTypeDef,
     DeleteObjectRequestRequestTypeDef,
-    DeleteObjectTaggingOutputTypeDef,
+    DeleteObjectTaggingOutputOutputTypeDef,
     DeleteObjectTaggingRequestRequestTypeDef,
-    DeletedObjectTypeDef,
-    ErrorTypeDef,
+    DeletedObjectOutputTypeDef,
+    ErrorOutputTypeDef,
     DeletePublicAccessBlockRequestRequestTypeDef,
     ObjectIdentifierTypeDef,
+    EncryptionConfigurationOutputTypeDef,
     EncryptionConfigurationTypeDef,
     EmptyResponseMetadataTypeDef,
     EncryptionTypeDef,
+    ErrorDocumentOutputTypeDef,
     ErrorDocumentResponseMetadataTypeDef,
     ErrorDocumentTypeDef,
+    ExistingObjectReplicationOutputTypeDef,
     ExistingObjectReplicationTypeDef,
+    FilterRuleOutputTypeDef,
     FilterRuleTypeDef,
-    GetBucketAccelerateConfigurationOutputTypeDef,
+    GetBucketAccelerateConfigurationOutputOutputTypeDef,
     GetBucketAccelerateConfigurationRequestRequestTypeDef,
     GetBucketAclRequestRequestTypeDef,
     GetBucketAnalyticsConfigurationRequestRequestTypeDef,
     GetBucketCorsRequestRequestTypeDef,
     GetBucketEncryptionRequestRequestTypeDef,
     GetBucketIntelligentTieringConfigurationRequestRequestTypeDef,
     GetBucketInventoryConfigurationRequestRequestTypeDef,
     GetBucketLifecycleConfigurationRequestRequestTypeDef,
     GetBucketLifecycleRequestRequestTypeDef,
-    GetBucketLocationOutputTypeDef,
+    GetBucketLocationOutputOutputTypeDef,
     GetBucketLocationRequestRequestTypeDef,
     GetBucketLoggingRequestRequestTypeDef,
     GetBucketMetricsConfigurationRequestRequestTypeDef,
     GetBucketNotificationConfigurationRequestRequestTypeDef,
     GetBucketOwnershipControlsRequestRequestTypeDef,
-    GetBucketPolicyOutputTypeDef,
+    GetBucketPolicyOutputOutputTypeDef,
     GetBucketPolicyRequestRequestTypeDef,
-    PolicyStatusTypeDef,
+    PolicyStatusOutputTypeDef,
     GetBucketPolicyStatusRequestRequestTypeDef,
     GetBucketReplicationRequestRequestTypeDef,
-    GetBucketRequestPaymentOutputTypeDef,
+    GetBucketRequestPaymentOutputOutputTypeDef,
     GetBucketRequestPaymentRequestRequestTypeDef,
     GetBucketTaggingRequestRequestTypeDef,
-    GetBucketVersioningOutputTypeDef,
+    GetBucketVersioningOutputOutputTypeDef,
     GetBucketVersioningRequestRequestTypeDef,
-    IndexDocumentTypeDef,
-    RedirectAllRequestsToTypeDef,
+    IndexDocumentOutputTypeDef,
+    RedirectAllRequestsToOutputTypeDef,
     GetBucketWebsiteRequestRequestTypeDef,
     GetObjectAclRequestRequestTypeDef,
-    ObjectPartTypeDef,
+    ObjectPartOutputTypeDef,
     GetObjectAttributesRequestRequestTypeDef,
-    ObjectLockLegalHoldTypeDef,
+    ObjectLockLegalHoldOutputTypeDef,
     GetObjectLegalHoldRequestRequestTypeDef,
     GetObjectLockConfigurationRequestRequestTypeDef,
-    GetObjectOutputTypeDef,
+    GetObjectOutputOutputTypeDef,
     GetObjectRequestObjectGetTypeDef,
     GetObjectRequestObjectSummaryGetTypeDef,
     GetObjectRequestObjectVersionGetTypeDef,
     GetObjectRequestRequestTypeDef,
-    ObjectLockRetentionTypeDef,
+    ObjectLockRetentionOutputTypeDef,
     GetObjectRetentionRequestRequestTypeDef,
     GetObjectTaggingRequestRequestTypeDef,
-    GetObjectTorrentOutputTypeDef,
+    GetObjectTorrentOutputOutputTypeDef,
     GetObjectTorrentRequestRequestTypeDef,
-    PublicAccessBlockConfigurationTypeDef,
+    PublicAccessBlockConfigurationOutputTypeDef,
     GetPublicAccessBlockRequestRequestTypeDef,
     GlacierJobParametersTypeDef,
+    GranteeOutputTypeDef,
     GranteeTypeDef,
     WaiterConfigTypeDef,
     HeadBucketRequestRequestTypeDef,
-    HeadObjectOutputTypeDef,
+    HeadObjectOutputOutputTypeDef,
     HeadObjectRequestObjectVersionHeadTypeDef,
     HeadObjectRequestRequestTypeDef,
     IndexDocumentResponseMetadataTypeDef,
+    IndexDocumentTypeDef,
+    InitiatorOutputTypeDef,
     InitiatorResponseMetadataTypeDef,
-    InitiatorTypeDef,
     JSONInputTypeDef,
+    TieringOutputTypeDef,
     TieringTypeDef,
+    InventoryFilterOutputTypeDef,
+    InventoryScheduleOutputTypeDef,
     InventoryFilterTypeDef,
     InventoryScheduleTypeDef,
+    SSEKMSOutputTypeDef,
     SSEKMSTypeDef,
     JSONOutputTypeDef,
+    LifecycleExpirationOutputTypeDef,
     LifecycleExpirationTypeDef,
+    NoncurrentVersionExpirationOutputTypeDef,
+    NoncurrentVersionTransitionOutputTypeDef,
+    TransitionOutputTypeDef,
     NoncurrentVersionExpirationTypeDef,
     NoncurrentVersionTransitionTypeDef,
     TransitionTypeDef,
     ListBucketAnalyticsConfigurationsRequestRequestTypeDef,
     ListBucketIntelligentTieringConfigurationsRequestRequestTypeDef,
     ListBucketInventoryConfigurationsRequestRequestTypeDef,
     ListBucketMetricsConfigurationsRequestRequestTypeDef,
@@ -677,229 +733,283 @@
     ListMultipartUploadsRequestRequestTypeDef,
     ListObjectVersionsRequestListObjectVersionsPaginateTypeDef,
     ListObjectVersionsRequestRequestTypeDef,
     ListObjectsRequestListObjectsPaginateTypeDef,
     ListObjectsRequestRequestTypeDef,
     ListObjectsV2RequestListObjectsV2PaginateTypeDef,
     ListObjectsV2RequestRequestTypeDef,
-    PartTypeDef,
+    PartOutputTypeDef,
     ListPartsRequestListPartsPaginateTypeDef,
     ListPartsRequestRequestTypeDef,
     MetadataEntryTypeDef,
+    ReplicationTimeValueOutputTypeDef,
     ReplicationTimeValueTypeDef,
+    QueueConfigurationDeprecatedOutputTypeDef,
+    TopicConfigurationDeprecatedOutputTypeDef,
     QueueConfigurationDeprecatedTypeDef,
     TopicConfigurationDeprecatedTypeDef,
     ObjectDownloadFileRequestTypeDef,
     ObjectDownloadFileobjRequestTypeDef,
-    RestoreStatusTypeDef,
+    ObjectLockLegalHoldTypeDef,
+    ObjectLockRetentionTypeDef,
+    RestoreStatusOutputTypeDef,
     ObjectUploadFileRequestTypeDef,
     ObjectUploadFileobjRequestTypeDef,
     OwnerResponseMetadataTypeDef,
+    OwnershipControlsRuleOutputTypeDef,
     OwnershipControlsRuleTypeDef,
     PaginatorConfigTypeDef,
-    ProgressTypeDef,
+    ProgressOutputTypeDef,
+    PublicAccessBlockConfigurationTypeDef,
     PutBucketPolicyRequestBucketPolicyPutTypeDef,
     PutBucketPolicyRequestRequestTypeDef,
     RequestPaymentConfigurationTypeDef,
     PutBucketVersioningRequestBucketVersioningEnableTypeDef,
     VersioningConfigurationTypeDef,
     PutBucketVersioningRequestBucketVersioningSuspendTypeDef,
-    PutObjectAclOutputTypeDef,
-    PutObjectLegalHoldOutputTypeDef,
-    PutObjectLockConfigurationOutputTypeDef,
-    PutObjectOutputTypeDef,
+    PutObjectAclOutputOutputTypeDef,
+    PutObjectLegalHoldOutputOutputTypeDef,
+    PutObjectLockConfigurationOutputOutputTypeDef,
+    PutObjectOutputOutputTypeDef,
     PutObjectRequestBucketPutObjectTypeDef,
     PutObjectRequestObjectPutTypeDef,
     PutObjectRequestObjectSummaryPutTypeDef,
     PutObjectRequestRequestTypeDef,
-    PutObjectRetentionOutputTypeDef,
-    PutObjectTaggingOutputTypeDef,
-    RecordsEventTypeDef,
+    PutObjectRetentionOutputOutputTypeDef,
+    PutObjectTaggingOutputOutputTypeDef,
+    RecordsEventOutputTypeDef,
     RedirectAllRequestsToResponseMetadataTypeDef,
+    RedirectAllRequestsToTypeDef,
+    RedirectOutputTypeDef,
     RedirectTypeDef,
+    ReplicaModificationsOutputTypeDef,
     ReplicaModificationsTypeDef,
     RequestProgressTypeDef,
     ResponseMetadataTypeDef,
-    RestoreObjectOutputTypeDef,
+    RestoreObjectOutputOutputTypeDef,
     RestoreStatusResponseMetadataTypeDef,
     ScanRangeTypeDef,
+    ServerSideEncryptionByDefaultOutputTypeDef,
     ServerSideEncryptionByDefaultTypeDef,
+    SseKmsEncryptedObjectsOutputTypeDef,
     SseKmsEncryptedObjectsTypeDef,
-    StatsTypeDef,
-    UploadPartOutputTypeDef,
+    StatsOutputTypeDef,
+    UploadPartOutputOutputTypeDef,
     UploadPartRequestMultipartUploadPartUploadTypeDef,
     UploadPartRequestRequestTypeDef,
     WriteGetObjectResponseRequestRequestTypeDef,
     PutBucketAccelerateConfigurationRequestRequestTypeDef,
-    DeleteMarkerEntryTypeDef,
+    AnalyticsAndOperatorOutputTypeDef,
+    GetBucketTaggingOutputOutputTypeDef,
+    GetObjectTaggingOutputOutputTypeDef,
+    IntelligentTieringAndOperatorOutputTypeDef,
+    LifecycleRuleAndOperatorOutputTypeDef,
+    MetricsAndOperatorOutputTypeDef,
+    ReplicationRuleAndOperatorOutputTypeDef,
     AnalyticsAndOperatorTypeDef,
-    GetBucketTaggingOutputTypeDef,
-    GetObjectTaggingOutputTypeDef,
     IntelligentTieringAndOperatorTypeDef,
     LifecycleRuleAndOperatorTypeDef,
     MetricsAndOperatorTypeDef,
     ReplicationRuleAndOperatorTypeDef,
     TaggingTypeDef,
+    AnalyticsExportDestinationOutputTypeDef,
     AnalyticsExportDestinationTypeDef,
     BucketCopyRequestTypeDef,
     ClientCopyRequestTypeDef,
     CopyObjectRequestRequestTypeDef,
     ObjectCopyRequestTypeDef,
     UploadPartCopyRequestMultipartUploadPartCopyFromTypeDef,
     UploadPartCopyRequestRequestTypeDef,
-    ListBucketsOutputTypeDef,
     CORSConfigurationTypeDef,
-    GetBucketCorsOutputTypeDef,
+    GetBucketCorsOutputOutputTypeDef,
     CompletedMultipartUploadTypeDef,
-    CopyObjectOutputTypeDef,
-    UploadPartCopyOutputTypeDef,
+    CopyObjectOutputOutputTypeDef,
+    UploadPartCopyOutputOutputTypeDef,
     CreateBucketRequestBucketCreateTypeDef,
     CreateBucketRequestRequestTypeDef,
     CreateBucketRequestServiceResourceCreateBucketTypeDef,
+    ObjectLockRuleOutputTypeDef,
     ObjectLockRuleTypeDef,
-    DeleteObjectsOutputTypeDef,
+    DeleteMarkerEntryOutputTypeDef,
+    ListBucketsOutputOutputTypeDef,
+    DeleteObjectsOutputOutputTypeDef,
     DeleteTypeDef,
+    S3KeyFilterOutputTypeDef,
     S3KeyFilterTypeDef,
-    GetBucketPolicyStatusOutputTypeDef,
-    GetObjectAttributesPartsTypeDef,
-    GetObjectLegalHoldOutputTypeDef,
-    PutObjectLegalHoldRequestRequestTypeDef,
-    GetObjectRetentionOutputTypeDef,
-    PutObjectRetentionRequestRequestTypeDef,
-    GetPublicAccessBlockOutputTypeDef,
-    PutPublicAccessBlockRequestRequestTypeDef,
+    GetBucketPolicyStatusOutputOutputTypeDef,
+    GetObjectAttributesPartsOutputTypeDef,
+    GetObjectLegalHoldOutputOutputTypeDef,
+    GetObjectRetentionOutputOutputTypeDef,
+    GetPublicAccessBlockOutputOutputTypeDef,
+    GrantOutputTypeDef,
+    TargetGrantOutputTypeDef,
     GrantTypeDef,
     TargetGrantTypeDef,
     HeadBucketRequestBucketExistsWaitTypeDef,
     HeadBucketRequestBucketNotExistsWaitTypeDef,
     HeadObjectRequestObjectExistsWaitTypeDef,
     HeadObjectRequestObjectNotExistsWaitTypeDef,
-    MultipartUploadTypeDef,
+    MultipartUploadOutputTypeDef,
     InputSerializationTypeDef,
+    InventoryEncryptionOutputTypeDef,
     InventoryEncryptionTypeDef,
     OutputSerializationTypeDef,
+    RuleOutputTypeDef,
     RuleTypeDef,
-    ListPartsOutputTypeDef,
+    ListPartsOutputOutputTypeDef,
+    MetricsOutputTypeDef,
+    ReplicationTimeOutputTypeDef,
     MetricsTypeDef,
     ReplicationTimeTypeDef,
-    NotificationConfigurationDeprecatedResponseMetadataTypeDef,
+    NotificationConfigurationDeprecatedOutputTypeDef,
     NotificationConfigurationDeprecatedTypeDef,
-    ObjectTypeDef,
-    ObjectVersionTypeDef,
+    PutObjectLegalHoldRequestRequestTypeDef,
+    PutObjectRetentionRequestRequestTypeDef,
+    ObjectOutputTypeDef,
+    ObjectVersionOutputTypeDef,
+    OwnershipControlsOutputTypeDef,
     OwnershipControlsTypeDef,
-    ProgressEventTypeDef,
+    ProgressEventOutputTypeDef,
+    PutPublicAccessBlockRequestRequestTypeDef,
     PutBucketRequestPaymentRequestBucketRequestPaymentPutTypeDef,
     PutBucketRequestPaymentRequestRequestTypeDef,
     PutBucketVersioningRequestBucketVersioningPutTypeDef,
     PutBucketVersioningRequestRequestTypeDef,
+    RoutingRuleOutputTypeDef,
     RoutingRuleTypeDef,
+    ServerSideEncryptionRuleOutputTypeDef,
     ServerSideEncryptionRuleTypeDef,
+    SourceSelectionCriteriaOutputTypeDef,
     SourceSelectionCriteriaTypeDef,
-    StatsEventTypeDef,
+    StatsEventOutputTypeDef,
+    AnalyticsFilterOutputTypeDef,
+    IntelligentTieringFilterOutputTypeDef,
+    LifecycleRuleFilterOutputTypeDef,
+    MetricsFilterOutputTypeDef,
+    ReplicationRuleFilterOutputTypeDef,
     AnalyticsFilterTypeDef,
     IntelligentTieringFilterTypeDef,
     LifecycleRuleFilterTypeDef,
     MetricsFilterTypeDef,
     ReplicationRuleFilterTypeDef,
     PutBucketTaggingRequestBucketTaggingPutTypeDef,
     PutBucketTaggingRequestRequestTypeDef,
     PutObjectTaggingRequestRequestTypeDef,
+    StorageClassAnalysisDataExportOutputTypeDef,
     StorageClassAnalysisDataExportTypeDef,
     PutBucketCorsRequestBucketCorsPutTypeDef,
     PutBucketCorsRequestRequestTypeDef,
     CompleteMultipartUploadRequestMultipartUploadCompleteTypeDef,
     CompleteMultipartUploadRequestRequestTypeDef,
+    ObjectLockConfigurationOutputTypeDef,
     ObjectLockConfigurationTypeDef,
     DeleteObjectsRequestBucketDeleteObjectsTypeDef,
     DeleteObjectsRequestRequestTypeDef,
+    NotificationConfigurationFilterOutputTypeDef,
     NotificationConfigurationFilterTypeDef,
-    GetObjectAttributesOutputTypeDef,
+    GetObjectAttributesOutputOutputTypeDef,
+    GetBucketAclOutputOutputTypeDef,
+    GetObjectAclOutputOutputTypeDef,
+    LoggingEnabledOutputTypeDef,
+    LoggingEnabledResponseMetadataTypeDef,
     AccessControlPolicyTypeDef,
-    GetBucketAclOutputTypeDef,
-    GetObjectAclOutputTypeDef,
     S3LocationTypeDef,
-    LoggingEnabledResponseMetadataTypeDef,
     LoggingEnabledTypeDef,
-    ListMultipartUploadsOutputTypeDef,
+    ListMultipartUploadsOutputOutputTypeDef,
+    InventoryS3BucketDestinationOutputTypeDef,
     InventoryS3BucketDestinationTypeDef,
     SelectObjectContentRequestRequestTypeDef,
     SelectParametersTypeDef,
-    GetBucketLifecycleOutputTypeDef,
+    GetBucketLifecycleOutputOutputTypeDef,
     LifecycleConfigurationTypeDef,
+    DestinationOutputTypeDef,
     DestinationTypeDef,
     PutBucketNotificationRequestRequestTypeDef,
-    ListObjectsOutputTypeDef,
-    ListObjectsV2OutputTypeDef,
-    ListObjectVersionsOutputTypeDef,
-    GetBucketOwnershipControlsOutputTypeDef,
+    ListObjectsOutputOutputTypeDef,
+    ListObjectsV2OutputOutputTypeDef,
+    ListObjectVersionsOutputOutputTypeDef,
+    GetBucketOwnershipControlsOutputOutputTypeDef,
     PutBucketOwnershipControlsRequestRequestTypeDef,
-    GetBucketWebsiteOutputTypeDef,
+    GetBucketWebsiteOutputOutputTypeDef,
     WebsiteConfigurationTypeDef,
+    ServerSideEncryptionConfigurationOutputTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
-    SelectObjectContentEventStreamTypeDef,
+    SelectObjectContentEventStreamOutputTypeDef,
+    IntelligentTieringConfigurationOutputTypeDef,
+    LifecycleRuleOutputTypeDef,
+    MetricsConfigurationOutputTypeDef,
     IntelligentTieringConfigurationTypeDef,
     LifecycleRuleTypeDef,
     MetricsConfigurationTypeDef,
+    StorageClassAnalysisOutputTypeDef,
     StorageClassAnalysisTypeDef,
-    GetObjectLockConfigurationOutputTypeDef,
+    GetObjectLockConfigurationOutputOutputTypeDef,
     PutObjectLockConfigurationRequestRequestTypeDef,
+    LambdaFunctionConfigurationOutputTypeDef,
+    QueueConfigurationOutputTypeDef,
+    TopicConfigurationOutputTypeDef,
     LambdaFunctionConfigurationTypeDef,
     QueueConfigurationTypeDef,
     TopicConfigurationTypeDef,
+    GetBucketLoggingOutputOutputTypeDef,
     PutBucketAclRequestBucketAclPutTypeDef,
     PutBucketAclRequestRequestTypeDef,
     PutObjectAclRequestObjectAclPutTypeDef,
     PutObjectAclRequestRequestTypeDef,
     OutputLocationTypeDef,
     BucketLoggingStatusTypeDef,
-    GetBucketLoggingOutputTypeDef,
+    InventoryDestinationOutputTypeDef,
     InventoryDestinationTypeDef,
     PutBucketLifecycleRequestBucketLifecyclePutTypeDef,
     PutBucketLifecycleRequestRequestTypeDef,
+    ReplicationRuleOutputTypeDef,
     ReplicationRuleTypeDef,
     PutBucketWebsiteRequestBucketWebsitePutTypeDef,
     PutBucketWebsiteRequestRequestTypeDef,
-    GetBucketEncryptionOutputTypeDef,
+    GetBucketEncryptionOutputOutputTypeDef,
     PutBucketEncryptionRequestRequestTypeDef,
-    SelectObjectContentOutputTypeDef,
-    GetBucketIntelligentTieringConfigurationOutputTypeDef,
-    ListBucketIntelligentTieringConfigurationsOutputTypeDef,
+    SelectObjectContentOutputOutputTypeDef,
+    GetBucketIntelligentTieringConfigurationOutputOutputTypeDef,
+    ListBucketIntelligentTieringConfigurationsOutputOutputTypeDef,
+    GetBucketLifecycleConfigurationOutputOutputTypeDef,
+    GetBucketMetricsConfigurationOutputOutputTypeDef,
+    ListBucketMetricsConfigurationsOutputOutputTypeDef,
     PutBucketIntelligentTieringConfigurationRequestRequestTypeDef,
     BucketLifecycleConfigurationTypeDef,
-    GetBucketLifecycleConfigurationOutputTypeDef,
-    GetBucketMetricsConfigurationOutputTypeDef,
-    ListBucketMetricsConfigurationsOutputTypeDef,
     PutBucketMetricsConfigurationRequestRequestTypeDef,
+    AnalyticsConfigurationOutputTypeDef,
     AnalyticsConfigurationTypeDef,
-    NotificationConfigurationResponseMetadataTypeDef,
+    NotificationConfigurationOutputTypeDef,
     NotificationConfigurationTypeDef,
     RestoreRequestTypeDef,
     PutBucketLoggingRequestBucketLoggingPutTypeDef,
     PutBucketLoggingRequestRequestTypeDef,
+    InventoryConfigurationOutputTypeDef,
     InventoryConfigurationTypeDef,
+    ReplicationConfigurationOutputTypeDef,
     ReplicationConfigurationTypeDef,
     PutBucketLifecycleConfigurationRequestBucketLifecycleConfigurationPutTypeDef,
     PutBucketLifecycleConfigurationRequestRequestTypeDef,
-    GetBucketAnalyticsConfigurationOutputTypeDef,
-    ListBucketAnalyticsConfigurationsOutputTypeDef,
+    GetBucketAnalyticsConfigurationOutputOutputTypeDef,
+    ListBucketAnalyticsConfigurationsOutputOutputTypeDef,
     PutBucketAnalyticsConfigurationRequestRequestTypeDef,
     PutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef,
     PutBucketNotificationConfigurationRequestRequestTypeDef,
     RestoreObjectRequestObjectRestoreObjectTypeDef,
     RestoreObjectRequestObjectSummaryRestoreObjectTypeDef,
     RestoreObjectRequestRequestTypeDef,
-    GetBucketInventoryConfigurationOutputTypeDef,
-    ListBucketInventoryConfigurationsOutputTypeDef,
+    GetBucketInventoryConfigurationOutputOutputTypeDef,
+    ListBucketInventoryConfigurationsOutputOutputTypeDef,
     PutBucketInventoryConfigurationRequestRequestTypeDef,
-    GetBucketReplicationOutputTypeDef,
+    GetBucketReplicationOutputOutputTypeDef,
     PutBucketReplicationRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AbortIncompleteMultipartUploadTypeDef:
+def get_structure() -> AbortIncompleteMultipartUploadOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-s3-1.28.3/mypy_boto3_s3/__init__.py` & `mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.28.3/mypy_boto3_s3/__init__.pyi` & `mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.28.3/mypy_boto3_s3/__main__.py` & `mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.S3 1.28.3\nVersion:         1.28.3\nBuilder version:"
-        " 7.14.6\nDocs:           "
+        "Type annotations for boto3.S3 1.28.3\nVersion:         1.28.3.post1\nBuilder version:"
+        " 7.14.7\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3\nOther"
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

### Comparing `mypy-boto3-s3-1.28.3/mypy_boto3_s3/client.py` & `mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,105 +39,105 @@
     ListMultipartUploadsPaginator,
     ListObjectsPaginator,
     ListObjectsV2Paginator,
     ListObjectVersionsPaginator,
     ListPartsPaginator,
 )
 from .type_defs import (
-    AbortMultipartUploadOutputTypeDef,
+    AbortMultipartUploadOutputOutputTypeDef,
     AccelerateConfigurationTypeDef,
     AccessControlPolicyTypeDef,
     AnalyticsConfigurationTypeDef,
     BucketLifecycleConfigurationTypeDef,
     BucketLoggingStatusTypeDef,
     CompletedMultipartUploadTypeDef,
-    CompleteMultipartUploadOutputTypeDef,
-    CopyObjectOutputTypeDef,
+    CompleteMultipartUploadOutputOutputTypeDef,
+    CopyObjectOutputOutputTypeDef,
     CopySourceTypeDef,
     CORSConfigurationTypeDef,
     CreateBucketConfigurationTypeDef,
-    CreateBucketOutputTypeDef,
-    CreateMultipartUploadOutputTypeDef,
-    DeleteObjectOutputTypeDef,
-    DeleteObjectsOutputTypeDef,
-    DeleteObjectTaggingOutputTypeDef,
+    CreateBucketOutputOutputTypeDef,
+    CreateMultipartUploadOutputOutputTypeDef,
+    DeleteObjectOutputOutputTypeDef,
+    DeleteObjectsOutputOutputTypeDef,
+    DeleteObjectTaggingOutputOutputTypeDef,
     DeleteTypeDef,
     EmptyResponseMetadataTypeDef,
-    GetBucketAccelerateConfigurationOutputTypeDef,
-    GetBucketAclOutputTypeDef,
-    GetBucketAnalyticsConfigurationOutputTypeDef,
-    GetBucketCorsOutputTypeDef,
-    GetBucketEncryptionOutputTypeDef,
-    GetBucketIntelligentTieringConfigurationOutputTypeDef,
-    GetBucketInventoryConfigurationOutputTypeDef,
-    GetBucketLifecycleConfigurationOutputTypeDef,
-    GetBucketLifecycleOutputTypeDef,
-    GetBucketLocationOutputTypeDef,
-    GetBucketLoggingOutputTypeDef,
-    GetBucketMetricsConfigurationOutputTypeDef,
-    GetBucketOwnershipControlsOutputTypeDef,
-    GetBucketPolicyOutputTypeDef,
-    GetBucketPolicyStatusOutputTypeDef,
-    GetBucketReplicationOutputTypeDef,
-    GetBucketRequestPaymentOutputTypeDef,
-    GetBucketTaggingOutputTypeDef,
-    GetBucketVersioningOutputTypeDef,
-    GetBucketWebsiteOutputTypeDef,
-    GetObjectAclOutputTypeDef,
-    GetObjectAttributesOutputTypeDef,
-    GetObjectLegalHoldOutputTypeDef,
-    GetObjectLockConfigurationOutputTypeDef,
-    GetObjectOutputTypeDef,
-    GetObjectRetentionOutputTypeDef,
-    GetObjectTaggingOutputTypeDef,
-    GetObjectTorrentOutputTypeDef,
-    GetPublicAccessBlockOutputTypeDef,
-    HeadObjectOutputTypeDef,
+    GetBucketAccelerateConfigurationOutputOutputTypeDef,
+    GetBucketAclOutputOutputTypeDef,
+    GetBucketAnalyticsConfigurationOutputOutputTypeDef,
+    GetBucketCorsOutputOutputTypeDef,
+    GetBucketEncryptionOutputOutputTypeDef,
+    GetBucketIntelligentTieringConfigurationOutputOutputTypeDef,
+    GetBucketInventoryConfigurationOutputOutputTypeDef,
+    GetBucketLifecycleConfigurationOutputOutputTypeDef,
+    GetBucketLifecycleOutputOutputTypeDef,
+    GetBucketLocationOutputOutputTypeDef,
+    GetBucketLoggingOutputOutputTypeDef,
+    GetBucketMetricsConfigurationOutputOutputTypeDef,
+    GetBucketOwnershipControlsOutputOutputTypeDef,
+    GetBucketPolicyOutputOutputTypeDef,
+    GetBucketPolicyStatusOutputOutputTypeDef,
+    GetBucketReplicationOutputOutputTypeDef,
+    GetBucketRequestPaymentOutputOutputTypeDef,
+    GetBucketTaggingOutputOutputTypeDef,
+    GetBucketVersioningOutputOutputTypeDef,
+    GetBucketWebsiteOutputOutputTypeDef,
+    GetObjectAclOutputOutputTypeDef,
+    GetObjectAttributesOutputOutputTypeDef,
+    GetObjectLegalHoldOutputOutputTypeDef,
+    GetObjectLockConfigurationOutputOutputTypeDef,
+    GetObjectOutputOutputTypeDef,
+    GetObjectRetentionOutputOutputTypeDef,
+    GetObjectTaggingOutputOutputTypeDef,
+    GetObjectTorrentOutputOutputTypeDef,
+    GetPublicAccessBlockOutputOutputTypeDef,
+    HeadObjectOutputOutputTypeDef,
     InputSerializationTypeDef,
     IntelligentTieringConfigurationTypeDef,
     InventoryConfigurationTypeDef,
     LifecycleConfigurationTypeDef,
-    ListBucketAnalyticsConfigurationsOutputTypeDef,
-    ListBucketIntelligentTieringConfigurationsOutputTypeDef,
-    ListBucketInventoryConfigurationsOutputTypeDef,
-    ListBucketMetricsConfigurationsOutputTypeDef,
-    ListBucketsOutputTypeDef,
-    ListMultipartUploadsOutputTypeDef,
-    ListObjectsOutputTypeDef,
-    ListObjectsV2OutputTypeDef,
-    ListObjectVersionsOutputTypeDef,
-    ListPartsOutputTypeDef,
+    ListBucketAnalyticsConfigurationsOutputOutputTypeDef,
+    ListBucketIntelligentTieringConfigurationsOutputOutputTypeDef,
+    ListBucketInventoryConfigurationsOutputOutputTypeDef,
+    ListBucketMetricsConfigurationsOutputOutputTypeDef,
+    ListBucketsOutputOutputTypeDef,
+    ListMultipartUploadsOutputOutputTypeDef,
+    ListObjectsOutputOutputTypeDef,
+    ListObjectsV2OutputOutputTypeDef,
+    ListObjectVersionsOutputOutputTypeDef,
+    ListPartsOutputOutputTypeDef,
     MetricsConfigurationTypeDef,
-    NotificationConfigurationDeprecatedResponseMetadataTypeDef,
+    NotificationConfigurationDeprecatedOutputTypeDef,
     NotificationConfigurationDeprecatedTypeDef,
-    NotificationConfigurationResponseMetadataTypeDef,
+    NotificationConfigurationOutputTypeDef,
     NotificationConfigurationTypeDef,
     ObjectLockConfigurationTypeDef,
     ObjectLockLegalHoldTypeDef,
     ObjectLockRetentionTypeDef,
     OutputSerializationTypeDef,
     OwnershipControlsTypeDef,
     PublicAccessBlockConfigurationTypeDef,
-    PutObjectAclOutputTypeDef,
-    PutObjectLegalHoldOutputTypeDef,
-    PutObjectLockConfigurationOutputTypeDef,
-    PutObjectOutputTypeDef,
-    PutObjectRetentionOutputTypeDef,
-    PutObjectTaggingOutputTypeDef,
+    PutObjectAclOutputOutputTypeDef,
+    PutObjectLegalHoldOutputOutputTypeDef,
+    PutObjectLockConfigurationOutputOutputTypeDef,
+    PutObjectOutputOutputTypeDef,
+    PutObjectRetentionOutputOutputTypeDef,
+    PutObjectTaggingOutputOutputTypeDef,
     ReplicationConfigurationTypeDef,
     RequestPaymentConfigurationTypeDef,
     RequestProgressTypeDef,
-    RestoreObjectOutputTypeDef,
+    RestoreObjectOutputOutputTypeDef,
     RestoreRequestTypeDef,
     ScanRangeTypeDef,
-    SelectObjectContentOutputTypeDef,
+    SelectObjectContentOutputOutputTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     TaggingTypeDef,
-    UploadPartCopyOutputTypeDef,
-    UploadPartOutputTypeDef,
+    UploadPartCopyOutputOutputTypeDef,
+    UploadPartOutputOutputTypeDef,
     VersioningConfigurationTypeDef,
     WebsiteConfigurationTypeDef,
 )
 from .waiter import (
     BucketExistsWaiter,
     BucketNotExistsWaiter,
     ObjectExistsWaiter,
@@ -194,15 +194,15 @@
         self,
         *,
         Bucket: str,
         Key: str,
         UploadId: str,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...
-    ) -> AbortMultipartUploadOutputTypeDef:
+    ) -> AbortMultipartUploadOutputOutputTypeDef:
         """
         This action aborts a multipart upload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.abort_multipart_upload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#abort_multipart_upload)
         """
 
@@ -234,15 +234,15 @@
         ChecksumSHA1: str = ...,
         ChecksumSHA256: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...
-    ) -> CompleteMultipartUploadOutputTypeDef:
+    ) -> CompleteMultipartUploadOutputOutputTypeDef:
         """
         Completes a multipart upload by assembling previously uploaded parts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.complete_multipart_upload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#complete_multipart_upload)
         """
 
@@ -303,15 +303,15 @@
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: Union[datetime, str] = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...,
         ExpectedSourceBucketOwner: str = ...
-    ) -> CopyObjectOutputTypeDef:
+    ) -> CopyObjectOutputOutputTypeDef:
         """
         Creates a copy of an object that is already stored in Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.copy_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#copy_object)
         """
 
@@ -324,15 +324,15 @@
         GrantFullControl: str = ...,
         GrantRead: str = ...,
         GrantReadACP: str = ...,
         GrantWrite: str = ...,
         GrantWriteACP: str = ...,
         ObjectLockEnabledForBucket: bool = ...,
         ObjectOwnership: ObjectOwnershipType = ...
-    ) -> CreateBucketOutputTypeDef:
+    ) -> CreateBucketOutputOutputTypeDef:
         """
         Creates a new S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.create_bucket)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#create_bucket)
         """
 
@@ -365,15 +365,15 @@
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: Union[datetime, str] = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...
-    ) -> CreateMultipartUploadOutputTypeDef:
+    ) -> CreateMultipartUploadOutputOutputTypeDef:
         """
         This action initiates a multipart upload and returns an upload ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.create_multipart_upload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#create_multipart_upload)
         """
 
@@ -518,26 +518,26 @@
         Bucket: str,
         Key: str,
         MFA: str = ...,
         VersionId: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...
-    ) -> DeleteObjectOutputTypeDef:
+    ) -> DeleteObjectOutputOutputTypeDef:
         """
         Removes the null version (if there is one) of an object and inserts a delete
         marker, which becomes the latest version of the object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.delete_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#delete_object)
         """
 
     def delete_object_tagging(
         self, *, Bucket: str, Key: str, VersionId: str = ..., ExpectedBucketOwner: str = ...
-    ) -> DeleteObjectTaggingOutputTypeDef:
+    ) -> DeleteObjectTaggingOutputOutputTypeDef:
         """
         Removes the entire tag set from the specified object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.delete_object_tagging)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#delete_object_tagging)
         """
 
@@ -547,15 +547,15 @@
         Bucket: str,
         Delete: DeleteTypeDef,
         MFA: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...
-    ) -> DeleteObjectsOutputTypeDef:
+    ) -> DeleteObjectsOutputOutputTypeDef:
         """
         This action enables you to delete multiple objects from a bucket using a single
         HTTP request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.delete_objects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#delete_objects)
         """
@@ -633,235 +633,235 @@
 
     def get_bucket_accelerate_configuration(
         self,
         *,
         Bucket: str,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...
-    ) -> GetBucketAccelerateConfigurationOutputTypeDef:
+    ) -> GetBucketAccelerateConfigurationOutputOutputTypeDef:
         """
         This implementation of the GET action uses the `accelerate` subresource to
         return the Transfer Acceleration state of a bucket, which is either `Enabled` or
         `Suspended`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_accelerate_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_accelerate_configuration)
         """
 
     def get_bucket_acl(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketAclOutputTypeDef:
+    ) -> GetBucketAclOutputOutputTypeDef:
         """
         This implementation of the `GET` action uses the `acl` subresource to return the
         access control list (ACL) of a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_acl)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_acl)
         """
 
     def get_bucket_analytics_configuration(
         self, *, Bucket: str, Id: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketAnalyticsConfigurationOutputTypeDef:
+    ) -> GetBucketAnalyticsConfigurationOutputOutputTypeDef:
         """
         This implementation of the GET action returns an analytics configuration
         (identified by the analytics configuration ID) from the bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_analytics_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_analytics_configuration)
         """
 
     def get_bucket_cors(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketCorsOutputTypeDef:
+    ) -> GetBucketCorsOutputOutputTypeDef:
         """
         Returns the Cross-Origin Resource Sharing (CORS) configuration information set
         for the bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_cors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_cors)
         """
 
     def get_bucket_encryption(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketEncryptionOutputTypeDef:
+    ) -> GetBucketEncryptionOutputOutputTypeDef:
         """
         Returns the default encryption configuration for an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_encryption)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_encryption)
         """
 
     def get_bucket_intelligent_tiering_configuration(
         self, *, Bucket: str, Id: str
-    ) -> GetBucketIntelligentTieringConfigurationOutputTypeDef:
+    ) -> GetBucketIntelligentTieringConfigurationOutputOutputTypeDef:
         """
         Gets the S3 Intelligent-Tiering configuration from the specified bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_intelligent_tiering_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_intelligent_tiering_configuration)
         """
 
     def get_bucket_inventory_configuration(
         self, *, Bucket: str, Id: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketInventoryConfigurationOutputTypeDef:
+    ) -> GetBucketInventoryConfigurationOutputOutputTypeDef:
         """
         Returns an inventory configuration (identified by the inventory configuration
         ID) from the bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_inventory_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_inventory_configuration)
         """
 
     def get_bucket_lifecycle(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketLifecycleOutputTypeDef:
+    ) -> GetBucketLifecycleOutputOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_lifecycle)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_lifecycle)
         """
 
     def get_bucket_lifecycle_configuration(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketLifecycleConfigurationOutputTypeDef:
+    ) -> GetBucketLifecycleConfigurationOutputOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_lifecycle_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_lifecycle_configuration)
         """
 
     def get_bucket_location(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketLocationOutputTypeDef:
+    ) -> GetBucketLocationOutputOutputTypeDef:
         """
         Returns the Region the bucket resides in.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_location)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_location)
         """
 
     def get_bucket_logging(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketLoggingOutputTypeDef:
+    ) -> GetBucketLoggingOutputOutputTypeDef:
         """
         Returns the logging status of a bucket and the permissions users have to view
         and modify that status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_logging)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_logging)
         """
 
     def get_bucket_metrics_configuration(
         self, *, Bucket: str, Id: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketMetricsConfigurationOutputTypeDef:
+    ) -> GetBucketMetricsConfigurationOutputOutputTypeDef:
         """
         Gets a metrics configuration (specified by the metrics configuration ID) from
         the bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_metrics_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_metrics_configuration)
         """
 
     def get_bucket_notification(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> NotificationConfigurationDeprecatedResponseMetadataTypeDef:
+    ) -> NotificationConfigurationDeprecatedOutputTypeDef:
         """
         No longer used, see
         [GetBucketNotificationConfiguration](https://docs.aws.amazon.com/AmazonS3/latest/API/API_GetBucketNotificationConfiguration.html)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_notification)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_notification)
         """
 
     def get_bucket_notification_configuration(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> NotificationConfigurationResponseMetadataTypeDef:
+    ) -> NotificationConfigurationOutputTypeDef:
         """
         Returns the notification configuration of a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_notification_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_notification_configuration)
         """
 
     def get_bucket_ownership_controls(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketOwnershipControlsOutputTypeDef:
+    ) -> GetBucketOwnershipControlsOutputOutputTypeDef:
         """
         Retrieves `OwnershipControls` for an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_ownership_controls)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_ownership_controls)
         """
 
     def get_bucket_policy(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketPolicyOutputTypeDef:
+    ) -> GetBucketPolicyOutputOutputTypeDef:
         """
         Returns the policy of a specified bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_policy)
         """
 
     def get_bucket_policy_status(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketPolicyStatusOutputTypeDef:
+    ) -> GetBucketPolicyStatusOutputOutputTypeDef:
         """
         Retrieves the policy status for an Amazon S3 bucket, indicating whether the
         bucket is public.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_policy_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_policy_status)
         """
 
     def get_bucket_replication(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketReplicationOutputTypeDef:
+    ) -> GetBucketReplicationOutputOutputTypeDef:
         """
         Returns the replication configuration of a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_replication)
         """
 
     def get_bucket_request_payment(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketRequestPaymentOutputTypeDef:
+    ) -> GetBucketRequestPaymentOutputOutputTypeDef:
         """
         Returns the request payment configuration of a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_request_payment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_request_payment)
         """
 
     def get_bucket_tagging(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketTaggingOutputTypeDef:
+    ) -> GetBucketTaggingOutputOutputTypeDef:
         """
         Returns the tag set associated with the bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_tagging)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_tagging)
         """
 
     def get_bucket_versioning(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketVersioningOutputTypeDef:
+    ) -> GetBucketVersioningOutputOutputTypeDef:
         """
         Returns the versioning state of a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_versioning)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_versioning)
         """
 
     def get_bucket_website(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketWebsiteOutputTypeDef:
+    ) -> GetBucketWebsiteOutputOutputTypeDef:
         """
         Returns the website configuration for a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_website)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_website)
         """
 
@@ -885,15 +885,15 @@
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumMode: Literal["ENABLED"] = ...
-    ) -> GetObjectOutputTypeDef:
+    ) -> GetObjectOutputOutputTypeDef:
         """
         Retrieves objects from Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_object)
         """
 
@@ -901,15 +901,15 @@
         self,
         *,
         Bucket: str,
         Key: str,
         VersionId: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...
-    ) -> GetObjectAclOutputTypeDef:
+    ) -> GetObjectAclOutputOutputTypeDef:
         """
         Returns the access control list (ACL) of an object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_acl)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_object_acl)
         """
 
@@ -923,15 +923,15 @@
         MaxParts: int = ...,
         PartNumberMarker: int = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...
-    ) -> GetObjectAttributesOutputTypeDef:
+    ) -> GetObjectAttributesOutputOutputTypeDef:
         """
         Retrieves all the metadata from an object without returning the object itself.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_object_attributes)
         """
 
@@ -939,25 +939,25 @@
         self,
         *,
         Bucket: str,
         Key: str,
         VersionId: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...
-    ) -> GetObjectLegalHoldOutputTypeDef:
+    ) -> GetObjectLegalHoldOutputOutputTypeDef:
         """
         Gets an object's current legal hold status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_legal_hold)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_object_legal_hold)
         """
 
     def get_object_lock_configuration(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetObjectLockConfigurationOutputTypeDef:
+    ) -> GetObjectLockConfigurationOutputOutputTypeDef:
         """
         Gets the Object Lock configuration for a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_lock_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_object_lock_configuration)
         """
 
@@ -965,15 +965,15 @@
         self,
         *,
         Bucket: str,
         Key: str,
         VersionId: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...
-    ) -> GetObjectRetentionOutputTypeDef:
+    ) -> GetObjectRetentionOutputOutputTypeDef:
         """
         Retrieves an object's retention settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_retention)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_object_retention)
         """
 
@@ -981,40 +981,40 @@
         self,
         *,
         Bucket: str,
         Key: str,
         VersionId: str = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...
-    ) -> GetObjectTaggingOutputTypeDef:
+    ) -> GetObjectTaggingOutputOutputTypeDef:
         """
         Returns the tag-set of an object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_tagging)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_object_tagging)
         """
 
     def get_object_torrent(
         self,
         *,
         Bucket: str,
         Key: str,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...
-    ) -> GetObjectTorrentOutputTypeDef:
+    ) -> GetObjectTorrentOutputOutputTypeDef:
         """
         Returns torrent files from a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_torrent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_object_torrent)
         """
 
     def get_public_access_block(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetPublicAccessBlockOutputTypeDef:
+    ) -> GetPublicAccessBlockOutputOutputTypeDef:
         """
         Retrieves the `PublicAccessBlock` configuration for an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_public_access_block)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_public_access_block)
         """
 
@@ -1043,64 +1043,64 @@
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumMode: Literal["ENABLED"] = ...
-    ) -> HeadObjectOutputTypeDef:
+    ) -> HeadObjectOutputOutputTypeDef:
         """
         The `HEAD` action retrieves metadata from an object without returning the object
         itself.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.head_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#head_object)
         """
 
     def list_bucket_analytics_configurations(
         self, *, Bucket: str, ContinuationToken: str = ..., ExpectedBucketOwner: str = ...
-    ) -> ListBucketAnalyticsConfigurationsOutputTypeDef:
+    ) -> ListBucketAnalyticsConfigurationsOutputOutputTypeDef:
         """
         Lists the analytics configurations for the bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_bucket_analytics_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_bucket_analytics_configurations)
         """
 
     def list_bucket_intelligent_tiering_configurations(
         self, *, Bucket: str, ContinuationToken: str = ...
-    ) -> ListBucketIntelligentTieringConfigurationsOutputTypeDef:
+    ) -> ListBucketIntelligentTieringConfigurationsOutputOutputTypeDef:
         """
         Lists the S3 Intelligent-Tiering configuration from the specified bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_bucket_intelligent_tiering_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_bucket_intelligent_tiering_configurations)
         """
 
     def list_bucket_inventory_configurations(
         self, *, Bucket: str, ContinuationToken: str = ..., ExpectedBucketOwner: str = ...
-    ) -> ListBucketInventoryConfigurationsOutputTypeDef:
+    ) -> ListBucketInventoryConfigurationsOutputOutputTypeDef:
         """
         Returns a list of inventory configurations for the bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_bucket_inventory_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_bucket_inventory_configurations)
         """
 
     def list_bucket_metrics_configurations(
         self, *, Bucket: str, ContinuationToken: str = ..., ExpectedBucketOwner: str = ...
-    ) -> ListBucketMetricsConfigurationsOutputTypeDef:
+    ) -> ListBucketMetricsConfigurationsOutputOutputTypeDef:
         """
         Lists the metrics configurations for the bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_bucket_metrics_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_bucket_metrics_configurations)
         """
 
-    def list_buckets(self) -> ListBucketsOutputTypeDef:
+    def list_buckets(self) -> ListBucketsOutputOutputTypeDef:
         """
         Returns a list of all buckets owned by the authenticated sender of the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_buckets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_buckets)
         """
 
@@ -1112,15 +1112,15 @@
         EncodingType: Literal["url"] = ...,
         KeyMarker: str = ...,
         MaxUploads: int = ...,
         Prefix: str = ...,
         UploadIdMarker: str = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...
-    ) -> ListMultipartUploadsOutputTypeDef:
+    ) -> ListMultipartUploadsOutputOutputTypeDef:
         """
         This action lists in-progress multipart uploads.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_multipart_uploads)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_multipart_uploads)
         """
 
@@ -1133,15 +1133,15 @@
         KeyMarker: str = ...,
         MaxKeys: int = ...,
         Prefix: str = ...,
         VersionIdMarker: str = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...
-    ) -> ListObjectVersionsOutputTypeDef:
+    ) -> ListObjectVersionsOutputOutputTypeDef:
         """
         Returns metadata about all versions of the objects in a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_object_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_object_versions)
         """
 
@@ -1153,15 +1153,15 @@
         EncodingType: Literal["url"] = ...,
         Marker: str = ...,
         MaxKeys: int = ...,
         Prefix: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...
-    ) -> ListObjectsOutputTypeDef:
+    ) -> ListObjectsOutputOutputTypeDef:
         """
         Returns some or all (up to 1,000) of the objects in a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_objects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_objects)
         """
 
@@ -1175,15 +1175,15 @@
         Prefix: str = ...,
         ContinuationToken: str = ...,
         FetchOwner: bool = ...,
         StartAfter: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...
-    ) -> ListObjectsV2OutputTypeDef:
+    ) -> ListObjectsV2OutputOutputTypeDef:
         """
         Returns some or all (up to 1,000) of the objects in a bucket with each request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_objects_v2)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_objects_v2)
         """
 
@@ -1196,15 +1196,15 @@
         MaxParts: int = ...,
         PartNumberMarker: int = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...
-    ) -> ListPartsOutputTypeDef:
+    ) -> ListPartsOutputOutputTypeDef:
         """
         Lists the parts that have been uploaded for a specific multipart upload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_parts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_parts)
         """
 
@@ -1562,15 +1562,15 @@
         BucketKeyEnabled: bool = ...,
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: Union[datetime, str] = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...
-    ) -> PutObjectOutputTypeDef:
+    ) -> PutObjectOutputOutputTypeDef:
         """
         Adds an object to a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#put_object)
         """
 
@@ -1586,15 +1586,15 @@
         GrantRead: str = ...,
         GrantReadACP: str = ...,
         GrantWrite: str = ...,
         GrantWriteACP: str = ...,
         RequestPayer: Literal["requester"] = ...,
         VersionId: str = ...,
         ExpectedBucketOwner: str = ...
-    ) -> PutObjectAclOutputTypeDef:
+    ) -> PutObjectAclOutputOutputTypeDef:
         """
         Uses the `acl` subresource to set the access control list (ACL) permissions for
         a new or existing object in an S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_object_acl)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#put_object_acl)
         """
@@ -1606,15 +1606,15 @@
         Key: str,
         LegalHold: ObjectLockLegalHoldTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         VersionId: str = ...,
         ContentMD5: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...
-    ) -> PutObjectLegalHoldOutputTypeDef:
+    ) -> PutObjectLegalHoldOutputOutputTypeDef:
         """
         Applies a legal hold configuration to the specified object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_object_legal_hold)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#put_object_legal_hold)
         """
 
@@ -1624,15 +1624,15 @@
         Bucket: str,
         ObjectLockConfiguration: ObjectLockConfigurationTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         Token: str = ...,
         ContentMD5: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...
-    ) -> PutObjectLockConfigurationOutputTypeDef:
+    ) -> PutObjectLockConfigurationOutputOutputTypeDef:
         """
         Places an Object Lock configuration on the specified bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_object_lock_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#put_object_lock_configuration)
         """
 
@@ -1644,15 +1644,15 @@
         Retention: ObjectLockRetentionTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         VersionId: str = ...,
         BypassGovernanceRetention: bool = ...,
         ContentMD5: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...
-    ) -> PutObjectRetentionOutputTypeDef:
+    ) -> PutObjectRetentionOutputOutputTypeDef:
         """
         Places an Object Retention configuration on an object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_object_retention)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#put_object_retention)
         """
 
@@ -1663,15 +1663,15 @@
         Key: str,
         Tagging: TaggingTypeDef,
         VersionId: str = ...,
         ContentMD5: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...
-    ) -> PutObjectTaggingOutputTypeDef:
+    ) -> PutObjectTaggingOutputOutputTypeDef:
         """
         Sets the supplied tag-set to an object that already exists in a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_object_tagging)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#put_object_tagging)
         """
 
@@ -1698,15 +1698,15 @@
         Bucket: str,
         Key: str,
         VersionId: str = ...,
         RestoreRequest: RestoreRequestTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...
-    ) -> RestoreObjectOutputTypeDef:
+    ) -> RestoreObjectOutputOutputTypeDef:
         """
         Restores an archived copy of an object back into Amazon S3 This action is not
         supported by Amazon S3 on Outposts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.restore_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#restore_object)
         """
@@ -1722,15 +1722,15 @@
         OutputSerialization: OutputSerializationTypeDef,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestProgress: RequestProgressTypeDef = ...,
         ScanRange: ScanRangeTypeDef = ...,
         ExpectedBucketOwner: str = ...
-    ) -> SelectObjectContentOutputTypeDef:
+    ) -> SelectObjectContentOutputOutputTypeDef:
         """
         This action filters the contents of an Amazon S3 object based on a simple
         structured query language (SQL) statement.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.select_object_content)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#select_object_content)
         """
@@ -1783,15 +1783,15 @@
         ChecksumSHA1: str = ...,
         ChecksumSHA256: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...
-    ) -> UploadPartOutputTypeDef:
+    ) -> UploadPartOutputOutputTypeDef:
         """
         Uploads a part in a multipart upload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.upload_part)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#upload_part)
         """
 
@@ -1813,15 +1813,15 @@
         SSECustomerKeyMD5: str = ...,
         CopySourceSSECustomerAlgorithm: str = ...,
         CopySourceSSECustomerKey: str = ...,
         CopySourceSSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         ExpectedSourceBucketOwner: str = ...
-    ) -> UploadPartCopyOutputTypeDef:
+    ) -> UploadPartCopyOutputOutputTypeDef:
         """
         Uploads a part by copying data from an existing object as data source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.upload_part_copy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#upload_part_copy)
         """
```

### Comparing `mypy-boto3-s3-1.28.3/mypy_boto3_s3/client.pyi` & `mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/client.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -39,105 +39,105 @@
     ListMultipartUploadsPaginator,
     ListObjectsPaginator,
     ListObjectsV2Paginator,
     ListObjectVersionsPaginator,
     ListPartsPaginator,
 )
 from .type_defs import (
-    AbortMultipartUploadOutputTypeDef,
+    AbortMultipartUploadOutputOutputTypeDef,
     AccelerateConfigurationTypeDef,
     AccessControlPolicyTypeDef,
     AnalyticsConfigurationTypeDef,
     BucketLifecycleConfigurationTypeDef,
     BucketLoggingStatusTypeDef,
     CompletedMultipartUploadTypeDef,
-    CompleteMultipartUploadOutputTypeDef,
-    CopyObjectOutputTypeDef,
+    CompleteMultipartUploadOutputOutputTypeDef,
+    CopyObjectOutputOutputTypeDef,
     CopySourceTypeDef,
     CORSConfigurationTypeDef,
     CreateBucketConfigurationTypeDef,
-    CreateBucketOutputTypeDef,
-    CreateMultipartUploadOutputTypeDef,
-    DeleteObjectOutputTypeDef,
-    DeleteObjectsOutputTypeDef,
-    DeleteObjectTaggingOutputTypeDef,
+    CreateBucketOutputOutputTypeDef,
+    CreateMultipartUploadOutputOutputTypeDef,
+    DeleteObjectOutputOutputTypeDef,
+    DeleteObjectsOutputOutputTypeDef,
+    DeleteObjectTaggingOutputOutputTypeDef,
     DeleteTypeDef,
     EmptyResponseMetadataTypeDef,
-    GetBucketAccelerateConfigurationOutputTypeDef,
-    GetBucketAclOutputTypeDef,
-    GetBucketAnalyticsConfigurationOutputTypeDef,
-    GetBucketCorsOutputTypeDef,
-    GetBucketEncryptionOutputTypeDef,
-    GetBucketIntelligentTieringConfigurationOutputTypeDef,
-    GetBucketInventoryConfigurationOutputTypeDef,
-    GetBucketLifecycleConfigurationOutputTypeDef,
-    GetBucketLifecycleOutputTypeDef,
-    GetBucketLocationOutputTypeDef,
-    GetBucketLoggingOutputTypeDef,
-    GetBucketMetricsConfigurationOutputTypeDef,
-    GetBucketOwnershipControlsOutputTypeDef,
-    GetBucketPolicyOutputTypeDef,
-    GetBucketPolicyStatusOutputTypeDef,
-    GetBucketReplicationOutputTypeDef,
-    GetBucketRequestPaymentOutputTypeDef,
-    GetBucketTaggingOutputTypeDef,
-    GetBucketVersioningOutputTypeDef,
-    GetBucketWebsiteOutputTypeDef,
-    GetObjectAclOutputTypeDef,
-    GetObjectAttributesOutputTypeDef,
-    GetObjectLegalHoldOutputTypeDef,
-    GetObjectLockConfigurationOutputTypeDef,
-    GetObjectOutputTypeDef,
-    GetObjectRetentionOutputTypeDef,
-    GetObjectTaggingOutputTypeDef,
-    GetObjectTorrentOutputTypeDef,
-    GetPublicAccessBlockOutputTypeDef,
-    HeadObjectOutputTypeDef,
+    GetBucketAccelerateConfigurationOutputOutputTypeDef,
+    GetBucketAclOutputOutputTypeDef,
+    GetBucketAnalyticsConfigurationOutputOutputTypeDef,
+    GetBucketCorsOutputOutputTypeDef,
+    GetBucketEncryptionOutputOutputTypeDef,
+    GetBucketIntelligentTieringConfigurationOutputOutputTypeDef,
+    GetBucketInventoryConfigurationOutputOutputTypeDef,
+    GetBucketLifecycleConfigurationOutputOutputTypeDef,
+    GetBucketLifecycleOutputOutputTypeDef,
+    GetBucketLocationOutputOutputTypeDef,
+    GetBucketLoggingOutputOutputTypeDef,
+    GetBucketMetricsConfigurationOutputOutputTypeDef,
+    GetBucketOwnershipControlsOutputOutputTypeDef,
+    GetBucketPolicyOutputOutputTypeDef,
+    GetBucketPolicyStatusOutputOutputTypeDef,
+    GetBucketReplicationOutputOutputTypeDef,
+    GetBucketRequestPaymentOutputOutputTypeDef,
+    GetBucketTaggingOutputOutputTypeDef,
+    GetBucketVersioningOutputOutputTypeDef,
+    GetBucketWebsiteOutputOutputTypeDef,
+    GetObjectAclOutputOutputTypeDef,
+    GetObjectAttributesOutputOutputTypeDef,
+    GetObjectLegalHoldOutputOutputTypeDef,
+    GetObjectLockConfigurationOutputOutputTypeDef,
+    GetObjectOutputOutputTypeDef,
+    GetObjectRetentionOutputOutputTypeDef,
+    GetObjectTaggingOutputOutputTypeDef,
+    GetObjectTorrentOutputOutputTypeDef,
+    GetPublicAccessBlockOutputOutputTypeDef,
+    HeadObjectOutputOutputTypeDef,
     InputSerializationTypeDef,
     IntelligentTieringConfigurationTypeDef,
     InventoryConfigurationTypeDef,
     LifecycleConfigurationTypeDef,
-    ListBucketAnalyticsConfigurationsOutputTypeDef,
-    ListBucketIntelligentTieringConfigurationsOutputTypeDef,
-    ListBucketInventoryConfigurationsOutputTypeDef,
-    ListBucketMetricsConfigurationsOutputTypeDef,
-    ListBucketsOutputTypeDef,
-    ListMultipartUploadsOutputTypeDef,
-    ListObjectsOutputTypeDef,
-    ListObjectsV2OutputTypeDef,
-    ListObjectVersionsOutputTypeDef,
-    ListPartsOutputTypeDef,
+    ListBucketAnalyticsConfigurationsOutputOutputTypeDef,
+    ListBucketIntelligentTieringConfigurationsOutputOutputTypeDef,
+    ListBucketInventoryConfigurationsOutputOutputTypeDef,
+    ListBucketMetricsConfigurationsOutputOutputTypeDef,
+    ListBucketsOutputOutputTypeDef,
+    ListMultipartUploadsOutputOutputTypeDef,
+    ListObjectsOutputOutputTypeDef,
+    ListObjectsV2OutputOutputTypeDef,
+    ListObjectVersionsOutputOutputTypeDef,
+    ListPartsOutputOutputTypeDef,
     MetricsConfigurationTypeDef,
-    NotificationConfigurationDeprecatedResponseMetadataTypeDef,
+    NotificationConfigurationDeprecatedOutputTypeDef,
     NotificationConfigurationDeprecatedTypeDef,
-    NotificationConfigurationResponseMetadataTypeDef,
+    NotificationConfigurationOutputTypeDef,
     NotificationConfigurationTypeDef,
     ObjectLockConfigurationTypeDef,
     ObjectLockLegalHoldTypeDef,
     ObjectLockRetentionTypeDef,
     OutputSerializationTypeDef,
     OwnershipControlsTypeDef,
     PublicAccessBlockConfigurationTypeDef,
-    PutObjectAclOutputTypeDef,
-    PutObjectLegalHoldOutputTypeDef,
-    PutObjectLockConfigurationOutputTypeDef,
-    PutObjectOutputTypeDef,
-    PutObjectRetentionOutputTypeDef,
-    PutObjectTaggingOutputTypeDef,
+    PutObjectAclOutputOutputTypeDef,
+    PutObjectLegalHoldOutputOutputTypeDef,
+    PutObjectLockConfigurationOutputOutputTypeDef,
+    PutObjectOutputOutputTypeDef,
+    PutObjectRetentionOutputOutputTypeDef,
+    PutObjectTaggingOutputOutputTypeDef,
     ReplicationConfigurationTypeDef,
     RequestPaymentConfigurationTypeDef,
     RequestProgressTypeDef,
-    RestoreObjectOutputTypeDef,
+    RestoreObjectOutputOutputTypeDef,
     RestoreRequestTypeDef,
     ScanRangeTypeDef,
-    SelectObjectContentOutputTypeDef,
+    SelectObjectContentOutputOutputTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     TaggingTypeDef,
-    UploadPartCopyOutputTypeDef,
-    UploadPartOutputTypeDef,
+    UploadPartCopyOutputOutputTypeDef,
+    UploadPartOutputOutputTypeDef,
     VersioningConfigurationTypeDef,
     WebsiteConfigurationTypeDef,
 )
 from .waiter import (
     BucketExistsWaiter,
     BucketNotExistsWaiter,
     ObjectExistsWaiter,
@@ -189,15 +189,15 @@
         self,
         *,
         Bucket: str,
         Key: str,
         UploadId: str,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...
-    ) -> AbortMultipartUploadOutputTypeDef:
+    ) -> AbortMultipartUploadOutputOutputTypeDef:
         """
         This action aborts a multipart upload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.abort_multipart_upload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#abort_multipart_upload)
         """
     def can_paginate(self, operation_name: str) -> bool:
@@ -226,15 +226,15 @@
         ChecksumSHA1: str = ...,
         ChecksumSHA256: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...
-    ) -> CompleteMultipartUploadOutputTypeDef:
+    ) -> CompleteMultipartUploadOutputOutputTypeDef:
         """
         Completes a multipart upload by assembling previously uploaded parts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.complete_multipart_upload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#complete_multipart_upload)
         """
     def copy(
@@ -293,15 +293,15 @@
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: Union[datetime, str] = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...,
         ExpectedSourceBucketOwner: str = ...
-    ) -> CopyObjectOutputTypeDef:
+    ) -> CopyObjectOutputOutputTypeDef:
         """
         Creates a copy of an object that is already stored in Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.copy_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#copy_object)
         """
     def create_bucket(
@@ -313,15 +313,15 @@
         GrantFullControl: str = ...,
         GrantRead: str = ...,
         GrantReadACP: str = ...,
         GrantWrite: str = ...,
         GrantWriteACP: str = ...,
         ObjectLockEnabledForBucket: bool = ...,
         ObjectOwnership: ObjectOwnershipType = ...
-    ) -> CreateBucketOutputTypeDef:
+    ) -> CreateBucketOutputOutputTypeDef:
         """
         Creates a new S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.create_bucket)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#create_bucket)
         """
     def create_multipart_upload(
@@ -353,15 +353,15 @@
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: Union[datetime, str] = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...
-    ) -> CreateMultipartUploadOutputTypeDef:
+    ) -> CreateMultipartUploadOutputOutputTypeDef:
         """
         This action initiates a multipart upload and returns an upload ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.create_multipart_upload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#create_multipart_upload)
         """
     def delete_bucket(
@@ -492,25 +492,25 @@
         Bucket: str,
         Key: str,
         MFA: str = ...,
         VersionId: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...
-    ) -> DeleteObjectOutputTypeDef:
+    ) -> DeleteObjectOutputOutputTypeDef:
         """
         Removes the null version (if there is one) of an object and inserts a delete
         marker, which becomes the latest version of the object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.delete_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#delete_object)
         """
     def delete_object_tagging(
         self, *, Bucket: str, Key: str, VersionId: str = ..., ExpectedBucketOwner: str = ...
-    ) -> DeleteObjectTaggingOutputTypeDef:
+    ) -> DeleteObjectTaggingOutputOutputTypeDef:
         """
         Removes the entire tag set from the specified object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.delete_object_tagging)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#delete_object_tagging)
         """
     def delete_objects(
@@ -519,15 +519,15 @@
         Bucket: str,
         Delete: DeleteTypeDef,
         MFA: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...
-    ) -> DeleteObjectsOutputTypeDef:
+    ) -> DeleteObjectsOutputOutputTypeDef:
         """
         This action enables you to delete multiple objects from a bucket using a single
         HTTP request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.delete_objects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#delete_objects)
         """
@@ -599,214 +599,214 @@
         """
     def get_bucket_accelerate_configuration(
         self,
         *,
         Bucket: str,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...
-    ) -> GetBucketAccelerateConfigurationOutputTypeDef:
+    ) -> GetBucketAccelerateConfigurationOutputOutputTypeDef:
         """
         This implementation of the GET action uses the `accelerate` subresource to
         return the Transfer Acceleration state of a bucket, which is either `Enabled` or
         `Suspended`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_accelerate_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_accelerate_configuration)
         """
     def get_bucket_acl(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketAclOutputTypeDef:
+    ) -> GetBucketAclOutputOutputTypeDef:
         """
         This implementation of the `GET` action uses the `acl` subresource to return the
         access control list (ACL) of a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_acl)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_acl)
         """
     def get_bucket_analytics_configuration(
         self, *, Bucket: str, Id: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketAnalyticsConfigurationOutputTypeDef:
+    ) -> GetBucketAnalyticsConfigurationOutputOutputTypeDef:
         """
         This implementation of the GET action returns an analytics configuration
         (identified by the analytics configuration ID) from the bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_analytics_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_analytics_configuration)
         """
     def get_bucket_cors(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketCorsOutputTypeDef:
+    ) -> GetBucketCorsOutputOutputTypeDef:
         """
         Returns the Cross-Origin Resource Sharing (CORS) configuration information set
         for the bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_cors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_cors)
         """
     def get_bucket_encryption(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketEncryptionOutputTypeDef:
+    ) -> GetBucketEncryptionOutputOutputTypeDef:
         """
         Returns the default encryption configuration for an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_encryption)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_encryption)
         """
     def get_bucket_intelligent_tiering_configuration(
         self, *, Bucket: str, Id: str
-    ) -> GetBucketIntelligentTieringConfigurationOutputTypeDef:
+    ) -> GetBucketIntelligentTieringConfigurationOutputOutputTypeDef:
         """
         Gets the S3 Intelligent-Tiering configuration from the specified bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_intelligent_tiering_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_intelligent_tiering_configuration)
         """
     def get_bucket_inventory_configuration(
         self, *, Bucket: str, Id: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketInventoryConfigurationOutputTypeDef:
+    ) -> GetBucketInventoryConfigurationOutputOutputTypeDef:
         """
         Returns an inventory configuration (identified by the inventory configuration
         ID) from the bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_inventory_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_inventory_configuration)
         """
     def get_bucket_lifecycle(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketLifecycleOutputTypeDef:
+    ) -> GetBucketLifecycleOutputOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_lifecycle)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_lifecycle)
         """
     def get_bucket_lifecycle_configuration(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketLifecycleConfigurationOutputTypeDef:
+    ) -> GetBucketLifecycleConfigurationOutputOutputTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_lifecycle_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_lifecycle_configuration)
         """
     def get_bucket_location(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketLocationOutputTypeDef:
+    ) -> GetBucketLocationOutputOutputTypeDef:
         """
         Returns the Region the bucket resides in.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_location)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_location)
         """
     def get_bucket_logging(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketLoggingOutputTypeDef:
+    ) -> GetBucketLoggingOutputOutputTypeDef:
         """
         Returns the logging status of a bucket and the permissions users have to view
         and modify that status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_logging)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_logging)
         """
     def get_bucket_metrics_configuration(
         self, *, Bucket: str, Id: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketMetricsConfigurationOutputTypeDef:
+    ) -> GetBucketMetricsConfigurationOutputOutputTypeDef:
         """
         Gets a metrics configuration (specified by the metrics configuration ID) from
         the bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_metrics_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_metrics_configuration)
         """
     def get_bucket_notification(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> NotificationConfigurationDeprecatedResponseMetadataTypeDef:
+    ) -> NotificationConfigurationDeprecatedOutputTypeDef:
         """
         No longer used, see
         [GetBucketNotificationConfiguration](https://docs.aws.amazon.com/AmazonS3/latest/API/API_GetBucketNotificationConfiguration.html)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_notification)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_notification)
         """
     def get_bucket_notification_configuration(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> NotificationConfigurationResponseMetadataTypeDef:
+    ) -> NotificationConfigurationOutputTypeDef:
         """
         Returns the notification configuration of a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_notification_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_notification_configuration)
         """
     def get_bucket_ownership_controls(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketOwnershipControlsOutputTypeDef:
+    ) -> GetBucketOwnershipControlsOutputOutputTypeDef:
         """
         Retrieves `OwnershipControls` for an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_ownership_controls)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_ownership_controls)
         """
     def get_bucket_policy(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketPolicyOutputTypeDef:
+    ) -> GetBucketPolicyOutputOutputTypeDef:
         """
         Returns the policy of a specified bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_policy)
         """
     def get_bucket_policy_status(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketPolicyStatusOutputTypeDef:
+    ) -> GetBucketPolicyStatusOutputOutputTypeDef:
         """
         Retrieves the policy status for an Amazon S3 bucket, indicating whether the
         bucket is public.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_policy_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_policy_status)
         """
     def get_bucket_replication(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketReplicationOutputTypeDef:
+    ) -> GetBucketReplicationOutputOutputTypeDef:
         """
         Returns the replication configuration of a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_replication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_replication)
         """
     def get_bucket_request_payment(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketRequestPaymentOutputTypeDef:
+    ) -> GetBucketRequestPaymentOutputOutputTypeDef:
         """
         Returns the request payment configuration of a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_request_payment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_request_payment)
         """
     def get_bucket_tagging(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketTaggingOutputTypeDef:
+    ) -> GetBucketTaggingOutputOutputTypeDef:
         """
         Returns the tag set associated with the bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_tagging)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_tagging)
         """
     def get_bucket_versioning(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketVersioningOutputTypeDef:
+    ) -> GetBucketVersioningOutputOutputTypeDef:
         """
         Returns the versioning state of a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_versioning)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_versioning)
         """
     def get_bucket_website(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetBucketWebsiteOutputTypeDef:
+    ) -> GetBucketWebsiteOutputOutputTypeDef:
         """
         Returns the website configuration for a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_bucket_website)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_bucket_website)
         """
     def get_object(
@@ -829,30 +829,30 @@
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumMode: Literal["ENABLED"] = ...
-    ) -> GetObjectOutputTypeDef:
+    ) -> GetObjectOutputOutputTypeDef:
         """
         Retrieves objects from Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_object)
         """
     def get_object_acl(
         self,
         *,
         Bucket: str,
         Key: str,
         VersionId: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...
-    ) -> GetObjectAclOutputTypeDef:
+    ) -> GetObjectAclOutputOutputTypeDef:
         """
         Returns the access control list (ACL) of an object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_acl)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_object_acl)
         """
     def get_object_attributes(
@@ -865,92 +865,92 @@
         MaxParts: int = ...,
         PartNumberMarker: int = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...
-    ) -> GetObjectAttributesOutputTypeDef:
+    ) -> GetObjectAttributesOutputOutputTypeDef:
         """
         Retrieves all the metadata from an object without returning the object itself.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_object_attributes)
         """
     def get_object_legal_hold(
         self,
         *,
         Bucket: str,
         Key: str,
         VersionId: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...
-    ) -> GetObjectLegalHoldOutputTypeDef:
+    ) -> GetObjectLegalHoldOutputOutputTypeDef:
         """
         Gets an object's current legal hold status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_legal_hold)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_object_legal_hold)
         """
     def get_object_lock_configuration(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetObjectLockConfigurationOutputTypeDef:
+    ) -> GetObjectLockConfigurationOutputOutputTypeDef:
         """
         Gets the Object Lock configuration for a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_lock_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_object_lock_configuration)
         """
     def get_object_retention(
         self,
         *,
         Bucket: str,
         Key: str,
         VersionId: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...
-    ) -> GetObjectRetentionOutputTypeDef:
+    ) -> GetObjectRetentionOutputOutputTypeDef:
         """
         Retrieves an object's retention settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_retention)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_object_retention)
         """
     def get_object_tagging(
         self,
         *,
         Bucket: str,
         Key: str,
         VersionId: str = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...
-    ) -> GetObjectTaggingOutputTypeDef:
+    ) -> GetObjectTaggingOutputOutputTypeDef:
         """
         Returns the tag-set of an object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_tagging)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_object_tagging)
         """
     def get_object_torrent(
         self,
         *,
         Bucket: str,
         Key: str,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...
-    ) -> GetObjectTorrentOutputTypeDef:
+    ) -> GetObjectTorrentOutputOutputTypeDef:
         """
         Returns torrent files from a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_object_torrent)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_object_torrent)
         """
     def get_public_access_block(
         self, *, Bucket: str, ExpectedBucketOwner: str = ...
-    ) -> GetPublicAccessBlockOutputTypeDef:
+    ) -> GetPublicAccessBlockOutputOutputTypeDef:
         """
         Retrieves the `PublicAccessBlock` configuration for an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.get_public_access_block)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#get_public_access_block)
         """
     def head_bucket(
@@ -977,59 +977,59 @@
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumMode: Literal["ENABLED"] = ...
-    ) -> HeadObjectOutputTypeDef:
+    ) -> HeadObjectOutputOutputTypeDef:
         """
         The `HEAD` action retrieves metadata from an object without returning the object
         itself.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.head_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#head_object)
         """
     def list_bucket_analytics_configurations(
         self, *, Bucket: str, ContinuationToken: str = ..., ExpectedBucketOwner: str = ...
-    ) -> ListBucketAnalyticsConfigurationsOutputTypeDef:
+    ) -> ListBucketAnalyticsConfigurationsOutputOutputTypeDef:
         """
         Lists the analytics configurations for the bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_bucket_analytics_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_bucket_analytics_configurations)
         """
     def list_bucket_intelligent_tiering_configurations(
         self, *, Bucket: str, ContinuationToken: str = ...
-    ) -> ListBucketIntelligentTieringConfigurationsOutputTypeDef:
+    ) -> ListBucketIntelligentTieringConfigurationsOutputOutputTypeDef:
         """
         Lists the S3 Intelligent-Tiering configuration from the specified bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_bucket_intelligent_tiering_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_bucket_intelligent_tiering_configurations)
         """
     def list_bucket_inventory_configurations(
         self, *, Bucket: str, ContinuationToken: str = ..., ExpectedBucketOwner: str = ...
-    ) -> ListBucketInventoryConfigurationsOutputTypeDef:
+    ) -> ListBucketInventoryConfigurationsOutputOutputTypeDef:
         """
         Returns a list of inventory configurations for the bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_bucket_inventory_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_bucket_inventory_configurations)
         """
     def list_bucket_metrics_configurations(
         self, *, Bucket: str, ContinuationToken: str = ..., ExpectedBucketOwner: str = ...
-    ) -> ListBucketMetricsConfigurationsOutputTypeDef:
+    ) -> ListBucketMetricsConfigurationsOutputOutputTypeDef:
         """
         Lists the metrics configurations for the bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_bucket_metrics_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_bucket_metrics_configurations)
         """
-    def list_buckets(self) -> ListBucketsOutputTypeDef:
+    def list_buckets(self) -> ListBucketsOutputOutputTypeDef:
         """
         Returns a list of all buckets owned by the authenticated sender of the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_buckets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_buckets)
         """
     def list_multipart_uploads(
@@ -1040,15 +1040,15 @@
         EncodingType: Literal["url"] = ...,
         KeyMarker: str = ...,
         MaxUploads: int = ...,
         Prefix: str = ...,
         UploadIdMarker: str = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...
-    ) -> ListMultipartUploadsOutputTypeDef:
+    ) -> ListMultipartUploadsOutputOutputTypeDef:
         """
         This action lists in-progress multipart uploads.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_multipart_uploads)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_multipart_uploads)
         """
     def list_object_versions(
@@ -1060,15 +1060,15 @@
         KeyMarker: str = ...,
         MaxKeys: int = ...,
         Prefix: str = ...,
         VersionIdMarker: str = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...
-    ) -> ListObjectVersionsOutputTypeDef:
+    ) -> ListObjectVersionsOutputOutputTypeDef:
         """
         Returns metadata about all versions of the objects in a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_object_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_object_versions)
         """
     def list_objects(
@@ -1079,15 +1079,15 @@
         EncodingType: Literal["url"] = ...,
         Marker: str = ...,
         MaxKeys: int = ...,
         Prefix: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...
-    ) -> ListObjectsOutputTypeDef:
+    ) -> ListObjectsOutputOutputTypeDef:
         """
         Returns some or all (up to 1,000) of the objects in a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_objects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_objects)
         """
     def list_objects_v2(
@@ -1100,15 +1100,15 @@
         Prefix: str = ...,
         ContinuationToken: str = ...,
         FetchOwner: bool = ...,
         StartAfter: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...
-    ) -> ListObjectsV2OutputTypeDef:
+    ) -> ListObjectsV2OutputOutputTypeDef:
         """
         Returns some or all (up to 1,000) of the objects in a bucket with each request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_objects_v2)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_objects_v2)
         """
     def list_parts(
@@ -1120,15 +1120,15 @@
         MaxParts: int = ...,
         PartNumberMarker: int = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...
-    ) -> ListPartsOutputTypeDef:
+    ) -> ListPartsOutputOutputTypeDef:
         """
         Lists the parts that have been uploaded for a specific multipart upload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.list_parts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#list_parts)
         """
     def put_bucket_accelerate_configuration(
@@ -1465,15 +1465,15 @@
         BucketKeyEnabled: bool = ...,
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: Union[datetime, str] = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...
-    ) -> PutObjectOutputTypeDef:
+    ) -> PutObjectOutputOutputTypeDef:
         """
         Adds an object to a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#put_object)
         """
     def put_object_acl(
@@ -1488,15 +1488,15 @@
         GrantRead: str = ...,
         GrantReadACP: str = ...,
         GrantWrite: str = ...,
         GrantWriteACP: str = ...,
         RequestPayer: Literal["requester"] = ...,
         VersionId: str = ...,
         ExpectedBucketOwner: str = ...
-    ) -> PutObjectAclOutputTypeDef:
+    ) -> PutObjectAclOutputOutputTypeDef:
         """
         Uses the `acl` subresource to set the access control list (ACL) permissions for
         a new or existing object in an S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_object_acl)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#put_object_acl)
         """
@@ -1507,15 +1507,15 @@
         Key: str,
         LegalHold: ObjectLockLegalHoldTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         VersionId: str = ...,
         ContentMD5: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...
-    ) -> PutObjectLegalHoldOutputTypeDef:
+    ) -> PutObjectLegalHoldOutputOutputTypeDef:
         """
         Applies a legal hold configuration to the specified object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_object_legal_hold)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#put_object_legal_hold)
         """
     def put_object_lock_configuration(
@@ -1524,15 +1524,15 @@
         Bucket: str,
         ObjectLockConfiguration: ObjectLockConfigurationTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         Token: str = ...,
         ContentMD5: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...
-    ) -> PutObjectLockConfigurationOutputTypeDef:
+    ) -> PutObjectLockConfigurationOutputOutputTypeDef:
         """
         Places an Object Lock configuration on the specified bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_object_lock_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#put_object_lock_configuration)
         """
     def put_object_retention(
@@ -1543,15 +1543,15 @@
         Retention: ObjectLockRetentionTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         VersionId: str = ...,
         BypassGovernanceRetention: bool = ...,
         ContentMD5: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...
-    ) -> PutObjectRetentionOutputTypeDef:
+    ) -> PutObjectRetentionOutputOutputTypeDef:
         """
         Places an Object Retention configuration on an object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_object_retention)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#put_object_retention)
         """
     def put_object_tagging(
@@ -1561,15 +1561,15 @@
         Key: str,
         Tagging: TaggingTypeDef,
         VersionId: str = ...,
         ContentMD5: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...
-    ) -> PutObjectTaggingOutputTypeDef:
+    ) -> PutObjectTaggingOutputOutputTypeDef:
         """
         Sets the supplied tag-set to an object that already exists in a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.put_object_tagging)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#put_object_tagging)
         """
     def put_public_access_block(
@@ -1594,15 +1594,15 @@
         Bucket: str,
         Key: str,
         VersionId: str = ...,
         RestoreRequest: RestoreRequestTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...
-    ) -> RestoreObjectOutputTypeDef:
+    ) -> RestoreObjectOutputOutputTypeDef:
         """
         Restores an archived copy of an object back into Amazon S3 This action is not
         supported by Amazon S3 on Outposts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.restore_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#restore_object)
         """
@@ -1617,15 +1617,15 @@
         OutputSerialization: OutputSerializationTypeDef,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestProgress: RequestProgressTypeDef = ...,
         ScanRange: ScanRangeTypeDef = ...,
         ExpectedBucketOwner: str = ...
-    ) -> SelectObjectContentOutputTypeDef:
+    ) -> SelectObjectContentOutputOutputTypeDef:
         """
         This action filters the contents of an Amazon S3 object based on a simple
         structured query language (SQL) statement.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.select_object_content)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#select_object_content)
         """
@@ -1675,15 +1675,15 @@
         ChecksumSHA1: str = ...,
         ChecksumSHA256: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...
-    ) -> UploadPartOutputTypeDef:
+    ) -> UploadPartOutputOutputTypeDef:
         """
         Uploads a part in a multipart upload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.upload_part)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#upload_part)
         """
     def upload_part_copy(
@@ -1704,15 +1704,15 @@
         SSECustomerKeyMD5: str = ...,
         CopySourceSSECustomerAlgorithm: str = ...,
         CopySourceSSECustomerKey: str = ...,
         CopySourceSSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         ExpectedSourceBucketOwner: str = ...
-    ) -> UploadPartCopyOutputTypeDef:
+    ) -> UploadPartCopyOutputOutputTypeDef:
         """
         Uploads a part by copying data from an existing object as data source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.upload_part_copy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/client/#upload_part_copy)
         """
     def write_get_object_response(
```

### Comparing `mypy-boto3-s3-1.28.3/mypy_boto3_s3/literals.py` & `mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.28.3/mypy_boto3_s3/literals.pyi` & `mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.28.3/mypy_boto3_s3/paginator.py` & `mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 """
 import sys
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
-    ListMultipartUploadsOutputTypeDef,
-    ListObjectsOutputTypeDef,
-    ListObjectsV2OutputTypeDef,
-    ListObjectVersionsOutputTypeDef,
-    ListPartsOutputTypeDef,
+    ListMultipartUploadsOutputOutputTypeDef,
+    ListObjectsOutputOutputTypeDef,
+    ListObjectsV2OutputOutputTypeDef,
+    ListObjectVersionsOutputOutputTypeDef,
+    ListPartsOutputOutputTypeDef,
     PaginatorConfigTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -78,15 +78,15 @@
         Bucket: str,
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListMultipartUploadsOutputTypeDef]:
+    ) -> _PageIterator[ListMultipartUploadsOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListMultipartUploads.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listmultipartuploadspaginator)
         """
 
 
 class ListObjectVersionsPaginator(Paginator):
@@ -102,15 +102,15 @@
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListObjectVersionsOutputTypeDef]:
+    ) -> _PageIterator[ListObjectVersionsOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjectVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listobjectversionspaginator)
         """
 
 
 class ListObjectsPaginator(Paginator):
@@ -126,15 +126,15 @@
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListObjectsOutputTypeDef]:
+    ) -> _PageIterator[ListObjectsOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listobjectspaginator)
         """
 
 
 class ListObjectsV2Paginator(Paginator):
@@ -152,15 +152,15 @@
         Prefix: str = ...,
         FetchOwner: bool = ...,
         StartAfter: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListObjectsV2OutputTypeDef]:
+    ) -> _PageIterator[ListObjectsV2OutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjectsV2.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listobjectsv2paginator)
         """
 
 
 class ListPartsPaginator(Paginator):
@@ -177,12 +177,12 @@
         UploadId: str,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListPartsOutputTypeDef]:
+    ) -> _PageIterator[ListPartsOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListParts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listpartspaginator)
         """
```

### Comparing `mypy-boto3-s3-1.28.3/mypy_boto3_s3/paginator.pyi` & `mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 """
 import sys
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
-    ListMultipartUploadsOutputTypeDef,
-    ListObjectsOutputTypeDef,
-    ListObjectsV2OutputTypeDef,
-    ListObjectVersionsOutputTypeDef,
-    ListPartsOutputTypeDef,
+    ListMultipartUploadsOutputOutputTypeDef,
+    ListObjectsOutputOutputTypeDef,
+    ListObjectsV2OutputOutputTypeDef,
+    ListObjectVersionsOutputOutputTypeDef,
+    ListPartsOutputOutputTypeDef,
     PaginatorConfigTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -74,15 +74,15 @@
         Bucket: str,
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListMultipartUploadsOutputTypeDef]:
+    ) -> _PageIterator[ListMultipartUploadsOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListMultipartUploads.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listmultipartuploadspaginator)
         """
 
 class ListObjectVersionsPaginator(Paginator):
     """
@@ -97,15 +97,15 @@
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         ExpectedBucketOwner: str = ...,
         RequestPayer: Literal["requester"] = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListObjectVersionsOutputTypeDef]:
+    ) -> _PageIterator[ListObjectVersionsOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjectVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listobjectversionspaginator)
         """
 
 class ListObjectsPaginator(Paginator):
     """
@@ -120,15 +120,15 @@
         Delimiter: str = ...,
         EncodingType: Literal["url"] = ...,
         Prefix: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListObjectsOutputTypeDef]:
+    ) -> _PageIterator[ListObjectsOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listobjectspaginator)
         """
 
 class ListObjectsV2Paginator(Paginator):
     """
@@ -145,15 +145,15 @@
         Prefix: str = ...,
         FetchOwner: bool = ...,
         StartAfter: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         OptionalObjectAttributes: Sequence[Literal["RestoreStatus"]] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListObjectsV2OutputTypeDef]:
+    ) -> _PageIterator[ListObjectsV2OutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjectsV2.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listobjectsv2paginator)
         """
 
 class ListPartsPaginator(Paginator):
     """
@@ -169,12 +169,12 @@
         UploadId: str,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListPartsOutputTypeDef]:
+    ) -> _PageIterator[ListPartsOutputOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListParts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/paginators/#listpartspaginator)
         """
```

### Comparing `mypy-boto3-s3-1.28.3/mypy_boto3_s3/service_resource.py` & `mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/service_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,55 +60,55 @@
     PayerType,
     ReplicationStatusType,
     ServerSideEncryptionType,
     StorageClassType,
     TaggingDirectiveType,
 )
 from .type_defs import (
-    AbortMultipartUploadOutputTypeDef,
+    AbortMultipartUploadOutputOutputTypeDef,
     AccessControlPolicyTypeDef,
     BucketLifecycleConfigurationTypeDef,
     BucketLoggingStatusTypeDef,
     CompletedMultipartUploadTypeDef,
-    CopyObjectOutputTypeDef,
+    CopyObjectOutputOutputTypeDef,
     CopySourceTypeDef,
     CORSConfigurationTypeDef,
-    CORSRuleTypeDef,
+    CORSRuleOutputTypeDef,
     CreateBucketConfigurationTypeDef,
-    CreateBucketOutputTypeDef,
-    DeleteObjectOutputTypeDef,
-    DeleteObjectsOutputTypeDef,
+    CreateBucketOutputOutputTypeDef,
+    DeleteObjectOutputOutputTypeDef,
+    DeleteObjectsOutputOutputTypeDef,
     DeleteTypeDef,
     ErrorDocumentResponseMetadataTypeDef,
-    GetObjectOutputTypeDef,
-    GrantTypeDef,
-    HeadObjectOutputTypeDef,
+    GetObjectOutputOutputTypeDef,
+    GrantOutputTypeDef,
+    HeadObjectOutputOutputTypeDef,
     IndexDocumentResponseMetadataTypeDef,
     InitiatorResponseMetadataTypeDef,
-    LambdaFunctionConfigurationTypeDef,
+    LambdaFunctionConfigurationOutputTypeDef,
     LifecycleConfigurationTypeDef,
-    LifecycleRuleTypeDef,
+    LifecycleRuleOutputTypeDef,
     LoggingEnabledResponseMetadataTypeDef,
     NotificationConfigurationTypeDef,
     OwnerResponseMetadataTypeDef,
-    PutObjectAclOutputTypeDef,
-    PutObjectOutputTypeDef,
-    QueueConfigurationTypeDef,
+    PutObjectAclOutputOutputTypeDef,
+    PutObjectOutputOutputTypeDef,
+    QueueConfigurationOutputTypeDef,
     RedirectAllRequestsToResponseMetadataTypeDef,
     RequestPaymentConfigurationTypeDef,
-    RestoreObjectOutputTypeDef,
+    RestoreObjectOutputOutputTypeDef,
     RestoreRequestTypeDef,
     RestoreStatusResponseMetadataTypeDef,
-    RoutingRuleTypeDef,
-    RuleTypeDef,
+    RoutingRuleOutputTypeDef,
+    RuleOutputTypeDef,
     TaggingTypeDef,
-    TagTypeDef,
-    TopicConfigurationTypeDef,
-    UploadPartCopyOutputTypeDef,
-    UploadPartOutputTypeDef,
+    TagOutputTypeDef,
+    TopicConfigurationOutputTypeDef,
+    UploadPartCopyOutputOutputTypeDef,
+    UploadPartOutputOutputTypeDef,
     VersioningConfigurationTypeDef,
     WebsiteConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -268,15 +268,15 @@
         self,
         *,
         MFA: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...
-    ) -> List[DeleteObjectsOutputTypeDef]:
+    ) -> List[DeleteObjectsOutputOutputTypeDef]:
         """
         Batch method.
         """
 
     def limit(self, count: int) -> "BucketObjectVersionsCollection":
         """
         Return at most this many ObjectVersions.
@@ -324,15 +324,15 @@
         self,
         *,
         MFA: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...
-    ) -> List[DeleteObjectsOutputTypeDef]:
+    ) -> List[DeleteObjectsOutputOutputTypeDef]:
         """
         Batch method.
         """
 
     def limit(self, count: int) -> "BucketObjectsCollection":
         """
         Return at most this many ObjectSummarys.
@@ -399,15 +399,15 @@
 class BucketAcl(ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketAcl)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketacl)
     """
 
     owner: OwnerResponseMetadataTypeDef
-    grants: List[GrantTypeDef]
+    grants: List[GrantOutputTypeDef]
     bucket_name: str
 
     def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketAcl.Bucket)
@@ -466,15 +466,15 @@
 
 class BucketCors(ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketCors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketcors)
     """
 
-    cors_rules: List[CORSRuleTypeDef]
+    cors_rules: List[CORSRuleOutputTypeDef]
     bucket_name: str
 
     def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketCors.Bucket)
@@ -535,15 +535,15 @@
 
 class BucketLifecycle(ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketLifecycle)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketlifecycle)
     """
 
-    rules: List[RuleTypeDef]
+    rules: List[RuleOutputTypeDef]
     bucket_name: str
 
     def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLifecycle.Bucket)
@@ -604,15 +604,15 @@
 
 class BucketLifecycleConfiguration(ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketLifecycleConfiguration)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketlifecycleconfiguration)
     """
 
-    rules: List[LifecycleRuleTypeDef]
+    rules: List[LifecycleRuleOutputTypeDef]
     bucket_name: str
 
     def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLifecycleConfiguration.Bucket)
@@ -736,17 +736,17 @@
 
 class BucketNotification(ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketNotification)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketnotification)
     """
 
-    topic_configurations: List[TopicConfigurationTypeDef]
-    queue_configurations: List[QueueConfigurationTypeDef]
-    lambda_function_configurations: List[LambdaFunctionConfigurationTypeDef]
+    topic_configurations: List[TopicConfigurationOutputTypeDef]
+    queue_configurations: List[QueueConfigurationOutputTypeDef]
+    lambda_function_configurations: List[LambdaFunctionConfigurationOutputTypeDef]
     event_bridge_configuration: Dict[str, Any]
     bucket_name: str
 
     def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
@@ -932,15 +932,15 @@
 
 class BucketTagging(ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketTagging)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#buckettagging)
     """
 
-    tag_set: List[TagTypeDef]
+    tag_set: List[TagOutputTypeDef]
     bucket_name: str
 
     def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketTagging.Bucket)
@@ -1095,15 +1095,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketWebsite)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketwebsite)
     """
 
     redirect_all_requests_to: RedirectAllRequestsToResponseMetadataTypeDef
     index_document: IndexDocumentResponseMetadataTypeDef
     error_document: ErrorDocumentResponseMetadataTypeDef
-    routing_rules: List[RoutingRuleTypeDef]
+    routing_rules: List[RoutingRuleOutputTypeDef]
     bucket_name: str
 
     def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketWebsite.Bucket)
@@ -1203,15 +1203,15 @@
         SSECustomerKeyMD5: str = ...,
         CopySourceSSECustomerAlgorithm: str = ...,
         CopySourceSSECustomerKey: str = ...,
         CopySourceSSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         ExpectedSourceBucketOwner: str = ...
-    ) -> UploadPartCopyOutputTypeDef:
+    ) -> UploadPartCopyOutputOutputTypeDef:
         """
         Uploads a part by copying data from an existing object as data source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.MultipartUploadPart.copy_from)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#multipartuploadpartcopy_from-method)
         """
 
@@ -1235,15 +1235,15 @@
         ChecksumSHA1: str = ...,
         ChecksumSHA256: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...
-    ) -> UploadPartOutputTypeDef:
+    ) -> UploadPartOutputOutputTypeDef:
         """
         Uploads a part in a multipart upload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.MultipartUploadPart.upload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#multipartuploadpartupload-method)
         """
 
@@ -1254,15 +1254,15 @@
 class ObjectAcl(ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.ObjectAcl)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectacl)
     """
 
     owner: OwnerResponseMetadataTypeDef
-    grants: List[GrantTypeDef]
+    grants: List[GrantOutputTypeDef]
     request_charged: Literal["requester"]
     bucket_name: str
     object_key: str
 
     def Object(self) -> "_Object":
         """
         Creates a Object resource.
@@ -1298,15 +1298,15 @@
         GrantRead: str = ...,
         GrantReadACP: str = ...,
         GrantWrite: str = ...,
         GrantWriteACP: str = ...,
         RequestPayer: Literal["requester"] = ...,
         VersionId: str = ...,
         ExpectedBucketOwner: str = ...
-    ) -> PutObjectAclOutputTypeDef:
+    ) -> PutObjectAclOutputOutputTypeDef:
         """
         Uses the `acl` subresource to set the access control list (ACL) permissions for
         a new or existing object in an S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectAcl.put)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectaclput-method)
         """
@@ -1355,15 +1355,15 @@
     def delete(
         self,
         *,
         MFA: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...
-    ) -> DeleteObjectOutputTypeDef:
+    ) -> DeleteObjectOutputOutputTypeDef:
         """
         Removes the null version (if there is one) of an object and inserts a delete
         marker, which becomes the latest version of the object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectVersion.delete)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectversiondelete-method)
         """
@@ -1385,15 +1385,15 @@
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumMode: Literal["ENABLED"] = ...
-    ) -> GetObjectOutputTypeDef:
+    ) -> GetObjectOutputOutputTypeDef:
         """
         Retrieves objects from Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectVersion.get)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectversionget-method)
         """
 
@@ -1416,15 +1416,15 @@
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumMode: Literal["ENABLED"] = ...
-    ) -> HeadObjectOutputTypeDef:
+    ) -> HeadObjectOutputOutputTypeDef:
         """
         The `HEAD` action retrieves metadata from an object without returning the object
         itself.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectVersion.head)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectversionhead-method)
         """
@@ -1465,15 +1465,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.MultipartUpload.Part)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#multipartuploadpart-method)
         """
 
     def abort(
         self, *, RequestPayer: Literal["requester"] = ..., ExpectedBucketOwner: str = ...
-    ) -> AbortMultipartUploadOutputTypeDef:
+    ) -> AbortMultipartUploadOutputOutputTypeDef:
         """
         This action aborts a multipart upload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.MultipartUpload.abort)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#multipartuploadabort-method)
         """
 
@@ -1638,15 +1638,15 @@
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: Union[datetime, str] = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...,
         ExpectedSourceBucketOwner: str = ...
-    ) -> CopyObjectOutputTypeDef:
+    ) -> CopyObjectOutputOutputTypeDef:
         """
         Creates a copy of an object that is already stored in Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.copy_from)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectcopy_from-method)
         """
 
@@ -1654,15 +1654,15 @@
         self,
         *,
         MFA: str = ...,
         VersionId: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...
-    ) -> DeleteObjectOutputTypeDef:
+    ) -> DeleteObjectOutputOutputTypeDef:
         """
         Removes the null version (if there is one) of an object and inserts a delete
         marker, which becomes the latest version of the object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.delete)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectdelete-method)
         """
@@ -1713,15 +1713,15 @@
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumMode: Literal["ENABLED"] = ...
-    ) -> GetObjectOutputTypeDef:
+    ) -> GetObjectOutputOutputTypeDef:
         """
         Retrieves objects from Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.get)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectget-method)
         """
 
@@ -1815,15 +1815,15 @@
         BucketKeyEnabled: bool = ...,
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: Union[datetime, str] = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...
-    ) -> PutObjectOutputTypeDef:
+    ) -> PutObjectOutputOutputTypeDef:
         """
         Adds an object to a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.put)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectput-method)
         """
 
@@ -1840,15 +1840,15 @@
         self,
         *,
         VersionId: str = ...,
         RestoreRequest: RestoreRequestTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...
-    ) -> RestoreObjectOutputTypeDef:
+    ) -> RestoreObjectOutputOutputTypeDef:
         """
         Restores an archived copy of an object back into Amazon S3 This action is not
         supported by Amazon S3 on Outposts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.restore_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectrestore_object-method)
         """
@@ -1995,15 +1995,15 @@
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: Union[datetime, str] = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...,
         ExpectedSourceBucketOwner: str = ...
-    ) -> CopyObjectOutputTypeDef:
+    ) -> CopyObjectOutputOutputTypeDef:
         """
         Creates a copy of an object that is already stored in Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.copy_from)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectsummarycopy_from-method)
         """
 
@@ -2011,15 +2011,15 @@
         self,
         *,
         MFA: str = ...,
         VersionId: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...
-    ) -> DeleteObjectOutputTypeDef:
+    ) -> DeleteObjectOutputOutputTypeDef:
         """
         Removes the null version (if there is one) of an object and inserts a delete
         marker, which becomes the latest version of the object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.delete)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectsummarydelete-method)
         """
@@ -2042,15 +2042,15 @@
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumMode: Literal["ENABLED"] = ...
-    ) -> GetObjectOutputTypeDef:
+    ) -> GetObjectOutputOutputTypeDef:
         """
         Retrieves objects from Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.get)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectsummaryget-method)
         """
 
@@ -2144,15 +2144,15 @@
         BucketKeyEnabled: bool = ...,
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: Union[datetime, str] = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...
-    ) -> PutObjectOutputTypeDef:
+    ) -> PutObjectOutputOutputTypeDef:
         """
         Adds an object to a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.put)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectsummaryput-method)
         """
 
@@ -2160,15 +2160,15 @@
         self,
         *,
         VersionId: str = ...,
         RestoreRequest: RestoreRequestTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...
-    ) -> RestoreObjectOutputTypeDef:
+    ) -> RestoreObjectOutputOutputTypeDef:
         """
         Restores an archived copy of an object back into Amazon S3 This action is not
         supported by Amazon S3 on Outposts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.restore_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectsummaryrestore_object-method)
         """
@@ -2325,15 +2325,15 @@
         GrantFullControl: str = ...,
         GrantRead: str = ...,
         GrantReadACP: str = ...,
         GrantWrite: str = ...,
         GrantWriteACP: str = ...,
         ObjectLockEnabledForBucket: bool = ...,
         ObjectOwnership: ObjectOwnershipType = ...
-    ) -> CreateBucketOutputTypeDef:
+    ) -> CreateBucketOutputOutputTypeDef:
         """
         Creates a new S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.create)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketcreate-method)
         """
 
@@ -2350,15 +2350,15 @@
         *,
         Delete: DeleteTypeDef,
         MFA: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...
-    ) -> DeleteObjectsOutputTypeDef:
+    ) -> DeleteObjectsOutputOutputTypeDef:
         """
         This action enables you to delete multiple objects from a bucket using a single
         HTTP request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.delete_objects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketdelete_objects-method)
         """
```

### Comparing `mypy-boto3-s3-1.28.3/mypy_boto3_s3/service_resource.pyi` & `mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/service_resource.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -60,55 +60,55 @@
     PayerType,
     ReplicationStatusType,
     ServerSideEncryptionType,
     StorageClassType,
     TaggingDirectiveType,
 )
 from .type_defs import (
-    AbortMultipartUploadOutputTypeDef,
+    AbortMultipartUploadOutputOutputTypeDef,
     AccessControlPolicyTypeDef,
     BucketLifecycleConfigurationTypeDef,
     BucketLoggingStatusTypeDef,
     CompletedMultipartUploadTypeDef,
-    CopyObjectOutputTypeDef,
+    CopyObjectOutputOutputTypeDef,
     CopySourceTypeDef,
     CORSConfigurationTypeDef,
-    CORSRuleTypeDef,
+    CORSRuleOutputTypeDef,
     CreateBucketConfigurationTypeDef,
-    CreateBucketOutputTypeDef,
-    DeleteObjectOutputTypeDef,
-    DeleteObjectsOutputTypeDef,
+    CreateBucketOutputOutputTypeDef,
+    DeleteObjectOutputOutputTypeDef,
+    DeleteObjectsOutputOutputTypeDef,
     DeleteTypeDef,
     ErrorDocumentResponseMetadataTypeDef,
-    GetObjectOutputTypeDef,
-    GrantTypeDef,
-    HeadObjectOutputTypeDef,
+    GetObjectOutputOutputTypeDef,
+    GrantOutputTypeDef,
+    HeadObjectOutputOutputTypeDef,
     IndexDocumentResponseMetadataTypeDef,
     InitiatorResponseMetadataTypeDef,
-    LambdaFunctionConfigurationTypeDef,
+    LambdaFunctionConfigurationOutputTypeDef,
     LifecycleConfigurationTypeDef,
-    LifecycleRuleTypeDef,
+    LifecycleRuleOutputTypeDef,
     LoggingEnabledResponseMetadataTypeDef,
     NotificationConfigurationTypeDef,
     OwnerResponseMetadataTypeDef,
-    PutObjectAclOutputTypeDef,
-    PutObjectOutputTypeDef,
-    QueueConfigurationTypeDef,
+    PutObjectAclOutputOutputTypeDef,
+    PutObjectOutputOutputTypeDef,
+    QueueConfigurationOutputTypeDef,
     RedirectAllRequestsToResponseMetadataTypeDef,
     RequestPaymentConfigurationTypeDef,
-    RestoreObjectOutputTypeDef,
+    RestoreObjectOutputOutputTypeDef,
     RestoreRequestTypeDef,
     RestoreStatusResponseMetadataTypeDef,
-    RoutingRuleTypeDef,
-    RuleTypeDef,
+    RoutingRuleOutputTypeDef,
+    RuleOutputTypeDef,
     TaggingTypeDef,
-    TagTypeDef,
-    TopicConfigurationTypeDef,
-    UploadPartCopyOutputTypeDef,
-    UploadPartOutputTypeDef,
+    TagOutputTypeDef,
+    TopicConfigurationOutputTypeDef,
+    UploadPartCopyOutputOutputTypeDef,
+    UploadPartOutputOutputTypeDef,
     VersioningConfigurationTypeDef,
     WebsiteConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -252,15 +252,15 @@
         self,
         *,
         MFA: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...
-    ) -> List[DeleteObjectsOutputTypeDef]:
+    ) -> List[DeleteObjectsOutputOutputTypeDef]:
         """
         Batch method.
         """
     def limit(self, count: int) -> "BucketObjectVersionsCollection":
         """
         Return at most this many ObjectVersions.
         """
@@ -301,15 +301,15 @@
         self,
         *,
         MFA: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...
-    ) -> List[DeleteObjectsOutputTypeDef]:
+    ) -> List[DeleteObjectsOutputOutputTypeDef]:
         """
         Batch method.
         """
     def limit(self, count: int) -> "BucketObjectsCollection":
         """
         Return at most this many ObjectSummarys.
         """
@@ -365,15 +365,15 @@
 class BucketAcl(ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketAcl)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketacl)
     """
 
     owner: OwnerResponseMetadataTypeDef
-    grants: List[GrantTypeDef]
+    grants: List[GrantOutputTypeDef]
     bucket_name: str
 
     def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketAcl.Bucket)
@@ -426,15 +426,15 @@
 
 class BucketCors(ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketCors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketcors)
     """
 
-    cors_rules: List[CORSRuleTypeDef]
+    cors_rules: List[CORSRuleOutputTypeDef]
     bucket_name: str
 
     def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketCors.Bucket)
@@ -488,15 +488,15 @@
 
 class BucketLifecycle(ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketLifecycle)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketlifecycle)
     """
 
-    rules: List[RuleTypeDef]
+    rules: List[RuleOutputTypeDef]
     bucket_name: str
 
     def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLifecycle.Bucket)
@@ -550,15 +550,15 @@
 
 class BucketLifecycleConfiguration(ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketLifecycleConfiguration)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketlifecycleconfiguration)
     """
 
-    rules: List[LifecycleRuleTypeDef]
+    rules: List[LifecycleRuleOutputTypeDef]
     bucket_name: str
 
     def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketLifecycleConfiguration.Bucket)
@@ -669,17 +669,17 @@
 
 class BucketNotification(ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketNotification)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketnotification)
     """
 
-    topic_configurations: List[TopicConfigurationTypeDef]
-    queue_configurations: List[QueueConfigurationTypeDef]
-    lambda_function_configurations: List[LambdaFunctionConfigurationTypeDef]
+    topic_configurations: List[TopicConfigurationOutputTypeDef]
+    queue_configurations: List[QueueConfigurationOutputTypeDef]
+    lambda_function_configurations: List[LambdaFunctionConfigurationOutputTypeDef]
     event_bridge_configuration: Dict[str, Any]
     bucket_name: str
 
     def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
@@ -846,15 +846,15 @@
 
 class BucketTagging(ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketTagging)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#buckettagging)
     """
 
-    tag_set: List[TagTypeDef]
+    tag_set: List[TagOutputTypeDef]
     bucket_name: str
 
     def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketTagging.Bucket)
@@ -994,15 +994,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.BucketWebsite)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketwebsite)
     """
 
     redirect_all_requests_to: RedirectAllRequestsToResponseMetadataTypeDef
     index_document: IndexDocumentResponseMetadataTypeDef
     error_document: ErrorDocumentResponseMetadataTypeDef
-    routing_rules: List[RoutingRuleTypeDef]
+    routing_rules: List[RoutingRuleOutputTypeDef]
     bucket_name: str
 
     def Bucket(self) -> "_Bucket":
         """
         Creates a Bucket resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.BucketWebsite.Bucket)
@@ -1094,15 +1094,15 @@
         SSECustomerKeyMD5: str = ...,
         CopySourceSSECustomerAlgorithm: str = ...,
         CopySourceSSECustomerKey: str = ...,
         CopySourceSSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...,
         ExpectedSourceBucketOwner: str = ...
-    ) -> UploadPartCopyOutputTypeDef:
+    ) -> UploadPartCopyOutputOutputTypeDef:
         """
         Uploads a part by copying data from an existing object as data source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.MultipartUploadPart.copy_from)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#multipartuploadpartcopy_from-method)
         """
     def get_available_subresources(self) -> Sequence[str]:
@@ -1124,15 +1124,15 @@
         ChecksumSHA1: str = ...,
         ChecksumSHA256: str = ...,
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         ExpectedBucketOwner: str = ...
-    ) -> UploadPartOutputTypeDef:
+    ) -> UploadPartOutputOutputTypeDef:
         """
         Uploads a part in a multipart upload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.MultipartUploadPart.upload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#multipartuploadpartupload-method)
         """
 
@@ -1141,15 +1141,15 @@
 class ObjectAcl(ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ServiceResource.ObjectAcl)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectacl)
     """
 
     owner: OwnerResponseMetadataTypeDef
-    grants: List[GrantTypeDef]
+    grants: List[GrantOutputTypeDef]
     request_charged: Literal["requester"]
     bucket_name: str
     object_key: str
 
     def Object(self) -> "_Object":
         """
         Creates a Object resource.
@@ -1182,15 +1182,15 @@
         GrantRead: str = ...,
         GrantReadACP: str = ...,
         GrantWrite: str = ...,
         GrantWriteACP: str = ...,
         RequestPayer: Literal["requester"] = ...,
         VersionId: str = ...,
         ExpectedBucketOwner: str = ...
-    ) -> PutObjectAclOutputTypeDef:
+    ) -> PutObjectAclOutputOutputTypeDef:
         """
         Uses the `acl` subresource to set the access control list (ACL) permissions for
         a new or existing object in an S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectAcl.put)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectaclput-method)
         """
@@ -1235,15 +1235,15 @@
     def delete(
         self,
         *,
         MFA: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...
-    ) -> DeleteObjectOutputTypeDef:
+    ) -> DeleteObjectOutputOutputTypeDef:
         """
         Removes the null version (if there is one) of an object and inserts a delete
         marker, which becomes the latest version of the object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectVersion.delete)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectversiondelete-method)
         """
@@ -1264,15 +1264,15 @@
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumMode: Literal["ENABLED"] = ...
-    ) -> GetObjectOutputTypeDef:
+    ) -> GetObjectOutputOutputTypeDef:
         """
         Retrieves objects from Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectVersion.get)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectversionget-method)
         """
     def get_available_subresources(self) -> Sequence[str]:
@@ -1293,15 +1293,15 @@
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumMode: Literal["ENABLED"] = ...
-    ) -> HeadObjectOutputTypeDef:
+    ) -> HeadObjectOutputOutputTypeDef:
         """
         The `HEAD` action retrieves metadata from an object without returning the object
         itself.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectVersion.head)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectversionhead-method)
         """
@@ -1338,15 +1338,15 @@
         Creates a MultipartUploadPart resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.MultipartUpload.Part)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#multipartuploadpart-method)
         """
     def abort(
         self, *, RequestPayer: Literal["requester"] = ..., ExpectedBucketOwner: str = ...
-    ) -> AbortMultipartUploadOutputTypeDef:
+    ) -> AbortMultipartUploadOutputOutputTypeDef:
         """
         This action aborts a multipart upload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.MultipartUpload.abort)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#multipartuploadabort-method)
         """
     def complete(
@@ -1502,30 +1502,30 @@
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: Union[datetime, str] = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...,
         ExpectedSourceBucketOwner: str = ...
-    ) -> CopyObjectOutputTypeDef:
+    ) -> CopyObjectOutputOutputTypeDef:
         """
         Creates a copy of an object that is already stored in Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.copy_from)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectcopy_from-method)
         """
     def delete(
         self,
         *,
         MFA: str = ...,
         VersionId: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...
-    ) -> DeleteObjectOutputTypeDef:
+    ) -> DeleteObjectOutputOutputTypeDef:
         """
         Removes the null version (if there is one) of an object and inserts a delete
         marker, which becomes the latest version of the object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.delete)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectdelete-method)
         """
@@ -1573,15 +1573,15 @@
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumMode: Literal["ENABLED"] = ...
-    ) -> GetObjectOutputTypeDef:
+    ) -> GetObjectOutputOutputTypeDef:
         """
         Retrieves objects from Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.get)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectget-method)
         """
     def get_available_subresources(self) -> Sequence[str]:
@@ -1671,15 +1671,15 @@
         BucketKeyEnabled: bool = ...,
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: Union[datetime, str] = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...
-    ) -> PutObjectOutputTypeDef:
+    ) -> PutObjectOutputOutputTypeDef:
         """
         Adds an object to a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.put)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectput-method)
         """
     def reload(self) -> None:
@@ -1694,15 +1694,15 @@
         self,
         *,
         VersionId: str = ...,
         RestoreRequest: RestoreRequestTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...
-    ) -> RestoreObjectOutputTypeDef:
+    ) -> RestoreObjectOutputOutputTypeDef:
         """
         Restores an archived copy of an object back into Amazon S3 This action is not
         supported by Amazon S3 on Outposts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Object.restore_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectrestore_object-method)
         """
@@ -1838,30 +1838,30 @@
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: Union[datetime, str] = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...,
         ExpectedSourceBucketOwner: str = ...
-    ) -> CopyObjectOutputTypeDef:
+    ) -> CopyObjectOutputOutputTypeDef:
         """
         Creates a copy of an object that is already stored in Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.copy_from)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectsummarycopy_from-method)
         """
     def delete(
         self,
         *,
         MFA: str = ...,
         VersionId: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...
-    ) -> DeleteObjectOutputTypeDef:
+    ) -> DeleteObjectOutputOutputTypeDef:
         """
         Removes the null version (if there is one) of an object and inserts a delete
         marker, which becomes the latest version of the object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.delete)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectsummarydelete-method)
         """
@@ -1883,15 +1883,15 @@
         SSECustomerAlgorithm: str = ...,
         SSECustomerKey: str = ...,
         SSECustomerKeyMD5: str = ...,
         RequestPayer: Literal["requester"] = ...,
         PartNumber: int = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumMode: Literal["ENABLED"] = ...
-    ) -> GetObjectOutputTypeDef:
+    ) -> GetObjectOutputOutputTypeDef:
         """
         Retrieves objects from Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.get)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectsummaryget-method)
         """
     def get_available_subresources(self) -> Sequence[str]:
@@ -1981,30 +1981,30 @@
         BucketKeyEnabled: bool = ...,
         RequestPayer: Literal["requester"] = ...,
         Tagging: str = ...,
         ObjectLockMode: ObjectLockModeType = ...,
         ObjectLockRetainUntilDate: Union[datetime, str] = ...,
         ObjectLockLegalHoldStatus: ObjectLockLegalHoldStatusType = ...,
         ExpectedBucketOwner: str = ...
-    ) -> PutObjectOutputTypeDef:
+    ) -> PutObjectOutputOutputTypeDef:
         """
         Adds an object to a bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.put)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectsummaryput-method)
         """
     def restore_object(
         self,
         *,
         VersionId: str = ...,
         RestoreRequest: RestoreRequestTypeDef = ...,
         RequestPayer: Literal["requester"] = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...,
         ExpectedBucketOwner: str = ...
-    ) -> RestoreObjectOutputTypeDef:
+    ) -> RestoreObjectOutputOutputTypeDef:
         """
         Restores an archived copy of an object back into Amazon S3 This action is not
         supported by Amazon S3 on Outposts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.ObjectSummary.restore_object)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#objectsummaryrestore_object-method)
         """
@@ -2144,15 +2144,15 @@
         GrantFullControl: str = ...,
         GrantRead: str = ...,
         GrantReadACP: str = ...,
         GrantWrite: str = ...,
         GrantWriteACP: str = ...,
         ObjectLockEnabledForBucket: bool = ...,
         ObjectOwnership: ObjectOwnershipType = ...
-    ) -> CreateBucketOutputTypeDef:
+    ) -> CreateBucketOutputOutputTypeDef:
         """
         Creates a new S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.create)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketcreate-method)
         """
     def delete(self, *, ExpectedBucketOwner: str = ...) -> None:
@@ -2167,15 +2167,15 @@
         *,
         Delete: DeleteTypeDef,
         MFA: str = ...,
         RequestPayer: Literal["requester"] = ...,
         BypassGovernanceRetention: bool = ...,
         ExpectedBucketOwner: str = ...,
         ChecksumAlgorithm: ChecksumAlgorithmType = ...
-    ) -> DeleteObjectsOutputTypeDef:
+    ) -> DeleteObjectsOutputOutputTypeDef:
         """
         This action enables you to delete multiple objects from a bucket using a single
         HTTP request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Bucket.delete_objects)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/service_resource/#bucketdelete_objects-method)
         """
```

### Comparing `mypy-boto3-s3-1.28.3/mypy_boto3_s3/type_defs.py` & `mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for s3 service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_s3.type_defs import AbortIncompleteMultipartUploadTypeDef
+    from mypy_boto3_s3.type_defs import AbortIncompleteMultipartUploadOutputTypeDef
 
-    data: AbortIncompleteMultipartUploadTypeDef = {...}
+    data: AbortIncompleteMultipartUploadOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Callable, Dict, List, Mapping, Sequence, Union
 
 from boto3.s3.transfer import TransferConfig
@@ -77,53 +77,61 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AbortIncompleteMultipartUploadOutputTypeDef",
     "AbortIncompleteMultipartUploadTypeDef",
-    "AbortMultipartUploadOutputTypeDef",
+    "AbortMultipartUploadOutputOutputTypeDef",
     "AbortMultipartUploadRequestMultipartUploadAbortTypeDef",
     "AbortMultipartUploadRequestRequestTypeDef",
     "AccelerateConfigurationTypeDef",
     "OwnerTypeDef",
+    "AccessControlTranslationOutputTypeDef",
     "AccessControlTranslationTypeDef",
+    "TagOutputTypeDef",
     "TagTypeDef",
+    "AnalyticsS3BucketDestinationOutputTypeDef",
     "AnalyticsS3BucketDestinationTypeDef",
     "CopySourceTypeDef",
     "BucketDownloadFileRequestTypeDef",
     "BucketDownloadFileobjRequestTypeDef",
-    "BucketTypeDef",
+    "BucketOutputTypeDef",
     "BucketUploadFileRequestTypeDef",
     "BucketUploadFileobjRequestTypeDef",
     "CORSRuleTypeDef",
+    "CORSRuleOutputTypeDef",
     "CSVInputTypeDef",
     "CSVOutputTypeDef",
-    "ChecksumTypeDef",
+    "ChecksumOutputTypeDef",
     "ClientDownloadFileRequestTypeDef",
     "ClientDownloadFileobjRequestTypeDef",
     "ClientGeneratePresignedPostRequestTypeDef",
     "ClientUploadFileRequestTypeDef",
     "ClientUploadFileobjRequestTypeDef",
+    "CloudFunctionConfigurationOutputTypeDef",
     "CloudFunctionConfigurationTypeDef",
-    "CommonPrefixTypeDef",
-    "CompleteMultipartUploadOutputTypeDef",
+    "CommonPrefixOutputTypeDef",
+    "CompleteMultipartUploadOutputOutputTypeDef",
     "CompletedPartTypeDef",
+    "ConditionOutputTypeDef",
     "ConditionTypeDef",
-    "CopyObjectResultTypeDef",
+    "CopyObjectResultOutputTypeDef",
     "CopyObjectRequestObjectCopyFromTypeDef",
     "CopyObjectRequestObjectSummaryCopyFromTypeDef",
-    "CopyPartResultTypeDef",
+    "CopyPartResultOutputTypeDef",
     "CreateBucketConfigurationTypeDef",
-    "CreateBucketOutputTypeDef",
-    "CreateMultipartUploadOutputTypeDef",
+    "CreateBucketOutputOutputTypeDef",
+    "CreateMultipartUploadOutputOutputTypeDef",
     "CreateMultipartUploadRequestObjectInitiateMultipartUploadTypeDef",
     "CreateMultipartUploadRequestObjectSummaryInitiateMultipartUploadTypeDef",
     "CreateMultipartUploadRequestRequestTypeDef",
+    "DefaultRetentionOutputTypeDef",
     "DefaultRetentionTypeDef",
     "DeleteBucketAnalyticsConfigurationRequestRequestTypeDef",
     "DeleteBucketCorsRequestBucketCorsDeleteTypeDef",
     "DeleteBucketCorsRequestRequestTypeDef",
     "DeleteBucketEncryptionRequestRequestTypeDef",
     "DeleteBucketIntelligentTieringConfigurationRequestRequestTypeDef",
     "DeleteBucketInventoryConfigurationRequestRequestTypeDef",
@@ -137,97 +145,113 @@
     "DeleteBucketReplicationRequestRequestTypeDef",
     "DeleteBucketRequestBucketDeleteTypeDef",
     "DeleteBucketRequestRequestTypeDef",
     "DeleteBucketTaggingRequestBucketTaggingDeleteTypeDef",
     "DeleteBucketTaggingRequestRequestTypeDef",
     "DeleteBucketWebsiteRequestBucketWebsiteDeleteTypeDef",
     "DeleteBucketWebsiteRequestRequestTypeDef",
+    "OwnerOutputTypeDef",
+    "DeleteMarkerReplicationOutputTypeDef",
     "DeleteMarkerReplicationTypeDef",
-    "DeleteObjectOutputTypeDef",
+    "DeleteObjectOutputOutputTypeDef",
     "DeleteObjectRequestObjectDeleteTypeDef",
     "DeleteObjectRequestObjectSummaryDeleteTypeDef",
     "DeleteObjectRequestObjectVersionDeleteTypeDef",
     "DeleteObjectRequestRequestTypeDef",
-    "DeleteObjectTaggingOutputTypeDef",
+    "DeleteObjectTaggingOutputOutputTypeDef",
     "DeleteObjectTaggingRequestRequestTypeDef",
-    "DeletedObjectTypeDef",
-    "ErrorTypeDef",
+    "DeletedObjectOutputTypeDef",
+    "ErrorOutputTypeDef",
     "DeletePublicAccessBlockRequestRequestTypeDef",
     "ObjectIdentifierTypeDef",
+    "EncryptionConfigurationOutputTypeDef",
     "EncryptionConfigurationTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EncryptionTypeDef",
+    "ErrorDocumentOutputTypeDef",
     "ErrorDocumentResponseMetadataTypeDef",
     "ErrorDocumentTypeDef",
+    "ExistingObjectReplicationOutputTypeDef",
     "ExistingObjectReplicationTypeDef",
+    "FilterRuleOutputTypeDef",
     "FilterRuleTypeDef",
-    "GetBucketAccelerateConfigurationOutputTypeDef",
+    "GetBucketAccelerateConfigurationOutputOutputTypeDef",
     "GetBucketAccelerateConfigurationRequestRequestTypeDef",
     "GetBucketAclRequestRequestTypeDef",
     "GetBucketAnalyticsConfigurationRequestRequestTypeDef",
     "GetBucketCorsRequestRequestTypeDef",
     "GetBucketEncryptionRequestRequestTypeDef",
     "GetBucketIntelligentTieringConfigurationRequestRequestTypeDef",
     "GetBucketInventoryConfigurationRequestRequestTypeDef",
     "GetBucketLifecycleConfigurationRequestRequestTypeDef",
     "GetBucketLifecycleRequestRequestTypeDef",
-    "GetBucketLocationOutputTypeDef",
+    "GetBucketLocationOutputOutputTypeDef",
     "GetBucketLocationRequestRequestTypeDef",
     "GetBucketLoggingRequestRequestTypeDef",
     "GetBucketMetricsConfigurationRequestRequestTypeDef",
     "GetBucketNotificationConfigurationRequestRequestTypeDef",
     "GetBucketOwnershipControlsRequestRequestTypeDef",
-    "GetBucketPolicyOutputTypeDef",
+    "GetBucketPolicyOutputOutputTypeDef",
     "GetBucketPolicyRequestRequestTypeDef",
-    "PolicyStatusTypeDef",
+    "PolicyStatusOutputTypeDef",
     "GetBucketPolicyStatusRequestRequestTypeDef",
     "GetBucketReplicationRequestRequestTypeDef",
-    "GetBucketRequestPaymentOutputTypeDef",
+    "GetBucketRequestPaymentOutputOutputTypeDef",
     "GetBucketRequestPaymentRequestRequestTypeDef",
     "GetBucketTaggingRequestRequestTypeDef",
-    "GetBucketVersioningOutputTypeDef",
+    "GetBucketVersioningOutputOutputTypeDef",
     "GetBucketVersioningRequestRequestTypeDef",
-    "IndexDocumentTypeDef",
-    "RedirectAllRequestsToTypeDef",
+    "IndexDocumentOutputTypeDef",
+    "RedirectAllRequestsToOutputTypeDef",
     "GetBucketWebsiteRequestRequestTypeDef",
     "GetObjectAclRequestRequestTypeDef",
-    "ObjectPartTypeDef",
+    "ObjectPartOutputTypeDef",
     "GetObjectAttributesRequestRequestTypeDef",
-    "ObjectLockLegalHoldTypeDef",
+    "ObjectLockLegalHoldOutputTypeDef",
     "GetObjectLegalHoldRequestRequestTypeDef",
     "GetObjectLockConfigurationRequestRequestTypeDef",
-    "GetObjectOutputTypeDef",
+    "GetObjectOutputOutputTypeDef",
     "GetObjectRequestObjectGetTypeDef",
     "GetObjectRequestObjectSummaryGetTypeDef",
     "GetObjectRequestObjectVersionGetTypeDef",
     "GetObjectRequestRequestTypeDef",
-    "ObjectLockRetentionTypeDef",
+    "ObjectLockRetentionOutputTypeDef",
     "GetObjectRetentionRequestRequestTypeDef",
     "GetObjectTaggingRequestRequestTypeDef",
-    "GetObjectTorrentOutputTypeDef",
+    "GetObjectTorrentOutputOutputTypeDef",
     "GetObjectTorrentRequestRequestTypeDef",
-    "PublicAccessBlockConfigurationTypeDef",
+    "PublicAccessBlockConfigurationOutputTypeDef",
     "GetPublicAccessBlockRequestRequestTypeDef",
     "GlacierJobParametersTypeDef",
+    "GranteeOutputTypeDef",
     "GranteeTypeDef",
     "WaiterConfigTypeDef",
     "HeadBucketRequestRequestTypeDef",
-    "HeadObjectOutputTypeDef",
+    "HeadObjectOutputOutputTypeDef",
     "HeadObjectRequestObjectVersionHeadTypeDef",
     "HeadObjectRequestRequestTypeDef",
     "IndexDocumentResponseMetadataTypeDef",
+    "IndexDocumentTypeDef",
+    "InitiatorOutputTypeDef",
     "InitiatorResponseMetadataTypeDef",
-    "InitiatorTypeDef",
     "JSONInputTypeDef",
+    "TieringOutputTypeDef",
     "TieringTypeDef",
+    "InventoryFilterOutputTypeDef",
+    "InventoryScheduleOutputTypeDef",
     "InventoryFilterTypeDef",
     "InventoryScheduleTypeDef",
+    "SSEKMSOutputTypeDef",
     "SSEKMSTypeDef",
     "JSONOutputTypeDef",
+    "LifecycleExpirationOutputTypeDef",
     "LifecycleExpirationTypeDef",
+    "NoncurrentVersionExpirationOutputTypeDef",
+    "NoncurrentVersionTransitionOutputTypeDef",
+    "TransitionOutputTypeDef",
     "NoncurrentVersionExpirationTypeDef",
     "NoncurrentVersionTransitionTypeDef",
     "TransitionTypeDef",
     "ListBucketAnalyticsConfigurationsRequestRequestTypeDef",
     "ListBucketIntelligentTieringConfigurationsRequestRequestTypeDef",
     "ListBucketInventoryConfigurationsRequestRequestTypeDef",
     "ListBucketMetricsConfigurationsRequestRequestTypeDef",
@@ -235,236 +259,298 @@
     "ListMultipartUploadsRequestRequestTypeDef",
     "ListObjectVersionsRequestListObjectVersionsPaginateTypeDef",
     "ListObjectVersionsRequestRequestTypeDef",
     "ListObjectsRequestListObjectsPaginateTypeDef",
     "ListObjectsRequestRequestTypeDef",
     "ListObjectsV2RequestListObjectsV2PaginateTypeDef",
     "ListObjectsV2RequestRequestTypeDef",
-    "PartTypeDef",
+    "PartOutputTypeDef",
     "ListPartsRequestListPartsPaginateTypeDef",
     "ListPartsRequestRequestTypeDef",
     "MetadataEntryTypeDef",
+    "ReplicationTimeValueOutputTypeDef",
     "ReplicationTimeValueTypeDef",
+    "QueueConfigurationDeprecatedOutputTypeDef",
+    "TopicConfigurationDeprecatedOutputTypeDef",
     "QueueConfigurationDeprecatedTypeDef",
     "TopicConfigurationDeprecatedTypeDef",
     "ObjectDownloadFileRequestTypeDef",
     "ObjectDownloadFileobjRequestTypeDef",
-    "RestoreStatusTypeDef",
+    "ObjectLockLegalHoldTypeDef",
+    "ObjectLockRetentionTypeDef",
+    "RestoreStatusOutputTypeDef",
     "ObjectUploadFileRequestTypeDef",
     "ObjectUploadFileobjRequestTypeDef",
     "OwnerResponseMetadataTypeDef",
+    "OwnershipControlsRuleOutputTypeDef",
     "OwnershipControlsRuleTypeDef",
     "PaginatorConfigTypeDef",
-    "ProgressTypeDef",
+    "ProgressOutputTypeDef",
+    "PublicAccessBlockConfigurationTypeDef",
     "PutBucketPolicyRequestBucketPolicyPutTypeDef",
     "PutBucketPolicyRequestRequestTypeDef",
     "RequestPaymentConfigurationTypeDef",
     "PutBucketVersioningRequestBucketVersioningEnableTypeDef",
     "VersioningConfigurationTypeDef",
     "PutBucketVersioningRequestBucketVersioningSuspendTypeDef",
-    "PutObjectAclOutputTypeDef",
-    "PutObjectLegalHoldOutputTypeDef",
-    "PutObjectLockConfigurationOutputTypeDef",
-    "PutObjectOutputTypeDef",
+    "PutObjectAclOutputOutputTypeDef",
+    "PutObjectLegalHoldOutputOutputTypeDef",
+    "PutObjectLockConfigurationOutputOutputTypeDef",
+    "PutObjectOutputOutputTypeDef",
     "PutObjectRequestBucketPutObjectTypeDef",
     "PutObjectRequestObjectPutTypeDef",
     "PutObjectRequestObjectSummaryPutTypeDef",
     "PutObjectRequestRequestTypeDef",
-    "PutObjectRetentionOutputTypeDef",
-    "PutObjectTaggingOutputTypeDef",
-    "RecordsEventTypeDef",
+    "PutObjectRetentionOutputOutputTypeDef",
+    "PutObjectTaggingOutputOutputTypeDef",
+    "RecordsEventOutputTypeDef",
     "RedirectAllRequestsToResponseMetadataTypeDef",
+    "RedirectAllRequestsToTypeDef",
+    "RedirectOutputTypeDef",
     "RedirectTypeDef",
+    "ReplicaModificationsOutputTypeDef",
     "ReplicaModificationsTypeDef",
     "RequestProgressTypeDef",
     "ResponseMetadataTypeDef",
-    "RestoreObjectOutputTypeDef",
+    "RestoreObjectOutputOutputTypeDef",
     "RestoreStatusResponseMetadataTypeDef",
     "ScanRangeTypeDef",
+    "ServerSideEncryptionByDefaultOutputTypeDef",
     "ServerSideEncryptionByDefaultTypeDef",
+    "SseKmsEncryptedObjectsOutputTypeDef",
     "SseKmsEncryptedObjectsTypeDef",
-    "StatsTypeDef",
-    "UploadPartOutputTypeDef",
+    "StatsOutputTypeDef",
+    "UploadPartOutputOutputTypeDef",
     "UploadPartRequestMultipartUploadPartUploadTypeDef",
     "UploadPartRequestRequestTypeDef",
     "WriteGetObjectResponseRequestRequestTypeDef",
     "PutBucketAccelerateConfigurationRequestRequestTypeDef",
-    "DeleteMarkerEntryTypeDef",
+    "AnalyticsAndOperatorOutputTypeDef",
+    "GetBucketTaggingOutputOutputTypeDef",
+    "GetObjectTaggingOutputOutputTypeDef",
+    "IntelligentTieringAndOperatorOutputTypeDef",
+    "LifecycleRuleAndOperatorOutputTypeDef",
+    "MetricsAndOperatorOutputTypeDef",
+    "ReplicationRuleAndOperatorOutputTypeDef",
     "AnalyticsAndOperatorTypeDef",
-    "GetBucketTaggingOutputTypeDef",
-    "GetObjectTaggingOutputTypeDef",
     "IntelligentTieringAndOperatorTypeDef",
     "LifecycleRuleAndOperatorTypeDef",
     "MetricsAndOperatorTypeDef",
     "ReplicationRuleAndOperatorTypeDef",
     "TaggingTypeDef",
+    "AnalyticsExportDestinationOutputTypeDef",
     "AnalyticsExportDestinationTypeDef",
     "BucketCopyRequestTypeDef",
     "ClientCopyRequestTypeDef",
     "CopyObjectRequestRequestTypeDef",
     "ObjectCopyRequestTypeDef",
     "UploadPartCopyRequestMultipartUploadPartCopyFromTypeDef",
     "UploadPartCopyRequestRequestTypeDef",
-    "ListBucketsOutputTypeDef",
     "CORSConfigurationTypeDef",
-    "GetBucketCorsOutputTypeDef",
+    "GetBucketCorsOutputOutputTypeDef",
     "CompletedMultipartUploadTypeDef",
-    "CopyObjectOutputTypeDef",
-    "UploadPartCopyOutputTypeDef",
+    "CopyObjectOutputOutputTypeDef",
+    "UploadPartCopyOutputOutputTypeDef",
     "CreateBucketRequestBucketCreateTypeDef",
     "CreateBucketRequestRequestTypeDef",
     "CreateBucketRequestServiceResourceCreateBucketTypeDef",
+    "ObjectLockRuleOutputTypeDef",
     "ObjectLockRuleTypeDef",
-    "DeleteObjectsOutputTypeDef",
+    "DeleteMarkerEntryOutputTypeDef",
+    "ListBucketsOutputOutputTypeDef",
+    "DeleteObjectsOutputOutputTypeDef",
     "DeleteTypeDef",
+    "S3KeyFilterOutputTypeDef",
     "S3KeyFilterTypeDef",
-    "GetBucketPolicyStatusOutputTypeDef",
-    "GetObjectAttributesPartsTypeDef",
-    "GetObjectLegalHoldOutputTypeDef",
-    "PutObjectLegalHoldRequestRequestTypeDef",
-    "GetObjectRetentionOutputTypeDef",
-    "PutObjectRetentionRequestRequestTypeDef",
-    "GetPublicAccessBlockOutputTypeDef",
-    "PutPublicAccessBlockRequestRequestTypeDef",
+    "GetBucketPolicyStatusOutputOutputTypeDef",
+    "GetObjectAttributesPartsOutputTypeDef",
+    "GetObjectLegalHoldOutputOutputTypeDef",
+    "GetObjectRetentionOutputOutputTypeDef",
+    "GetPublicAccessBlockOutputOutputTypeDef",
+    "GrantOutputTypeDef",
+    "TargetGrantOutputTypeDef",
     "GrantTypeDef",
     "TargetGrantTypeDef",
     "HeadBucketRequestBucketExistsWaitTypeDef",
     "HeadBucketRequestBucketNotExistsWaitTypeDef",
     "HeadObjectRequestObjectExistsWaitTypeDef",
     "HeadObjectRequestObjectNotExistsWaitTypeDef",
-    "MultipartUploadTypeDef",
+    "MultipartUploadOutputTypeDef",
     "InputSerializationTypeDef",
+    "InventoryEncryptionOutputTypeDef",
     "InventoryEncryptionTypeDef",
     "OutputSerializationTypeDef",
+    "RuleOutputTypeDef",
     "RuleTypeDef",
-    "ListPartsOutputTypeDef",
+    "ListPartsOutputOutputTypeDef",
+    "MetricsOutputTypeDef",
+    "ReplicationTimeOutputTypeDef",
     "MetricsTypeDef",
     "ReplicationTimeTypeDef",
-    "NotificationConfigurationDeprecatedResponseMetadataTypeDef",
+    "NotificationConfigurationDeprecatedOutputTypeDef",
     "NotificationConfigurationDeprecatedTypeDef",
-    "ObjectTypeDef",
-    "ObjectVersionTypeDef",
+    "PutObjectLegalHoldRequestRequestTypeDef",
+    "PutObjectRetentionRequestRequestTypeDef",
+    "ObjectOutputTypeDef",
+    "ObjectVersionOutputTypeDef",
+    "OwnershipControlsOutputTypeDef",
     "OwnershipControlsTypeDef",
-    "ProgressEventTypeDef",
+    "ProgressEventOutputTypeDef",
+    "PutPublicAccessBlockRequestRequestTypeDef",
     "PutBucketRequestPaymentRequestBucketRequestPaymentPutTypeDef",
     "PutBucketRequestPaymentRequestRequestTypeDef",
     "PutBucketVersioningRequestBucketVersioningPutTypeDef",
     "PutBucketVersioningRequestRequestTypeDef",
+    "RoutingRuleOutputTypeDef",
     "RoutingRuleTypeDef",
+    "ServerSideEncryptionRuleOutputTypeDef",
     "ServerSideEncryptionRuleTypeDef",
+    "SourceSelectionCriteriaOutputTypeDef",
     "SourceSelectionCriteriaTypeDef",
-    "StatsEventTypeDef",
+    "StatsEventOutputTypeDef",
+    "AnalyticsFilterOutputTypeDef",
+    "IntelligentTieringFilterOutputTypeDef",
+    "LifecycleRuleFilterOutputTypeDef",
+    "MetricsFilterOutputTypeDef",
+    "ReplicationRuleFilterOutputTypeDef",
     "AnalyticsFilterTypeDef",
     "IntelligentTieringFilterTypeDef",
     "LifecycleRuleFilterTypeDef",
     "MetricsFilterTypeDef",
     "ReplicationRuleFilterTypeDef",
     "PutBucketTaggingRequestBucketTaggingPutTypeDef",
     "PutBucketTaggingRequestRequestTypeDef",
     "PutObjectTaggingRequestRequestTypeDef",
+    "StorageClassAnalysisDataExportOutputTypeDef",
     "StorageClassAnalysisDataExportTypeDef",
     "PutBucketCorsRequestBucketCorsPutTypeDef",
     "PutBucketCorsRequestRequestTypeDef",
     "CompleteMultipartUploadRequestMultipartUploadCompleteTypeDef",
     "CompleteMultipartUploadRequestRequestTypeDef",
+    "ObjectLockConfigurationOutputTypeDef",
     "ObjectLockConfigurationTypeDef",
     "DeleteObjectsRequestBucketDeleteObjectsTypeDef",
     "DeleteObjectsRequestRequestTypeDef",
+    "NotificationConfigurationFilterOutputTypeDef",
     "NotificationConfigurationFilterTypeDef",
-    "GetObjectAttributesOutputTypeDef",
+    "GetObjectAttributesOutputOutputTypeDef",
+    "GetBucketAclOutputOutputTypeDef",
+    "GetObjectAclOutputOutputTypeDef",
+    "LoggingEnabledOutputTypeDef",
+    "LoggingEnabledResponseMetadataTypeDef",
     "AccessControlPolicyTypeDef",
-    "GetBucketAclOutputTypeDef",
-    "GetObjectAclOutputTypeDef",
     "S3LocationTypeDef",
-    "LoggingEnabledResponseMetadataTypeDef",
     "LoggingEnabledTypeDef",
-    "ListMultipartUploadsOutputTypeDef",
+    "ListMultipartUploadsOutputOutputTypeDef",
+    "InventoryS3BucketDestinationOutputTypeDef",
     "InventoryS3BucketDestinationTypeDef",
     "SelectObjectContentRequestRequestTypeDef",
     "SelectParametersTypeDef",
-    "GetBucketLifecycleOutputTypeDef",
+    "GetBucketLifecycleOutputOutputTypeDef",
     "LifecycleConfigurationTypeDef",
+    "DestinationOutputTypeDef",
     "DestinationTypeDef",
     "PutBucketNotificationRequestRequestTypeDef",
-    "ListObjectsOutputTypeDef",
-    "ListObjectsV2OutputTypeDef",
-    "ListObjectVersionsOutputTypeDef",
-    "GetBucketOwnershipControlsOutputTypeDef",
+    "ListObjectsOutputOutputTypeDef",
+    "ListObjectsV2OutputOutputTypeDef",
+    "ListObjectVersionsOutputOutputTypeDef",
+    "GetBucketOwnershipControlsOutputOutputTypeDef",
     "PutBucketOwnershipControlsRequestRequestTypeDef",
-    "GetBucketWebsiteOutputTypeDef",
+    "GetBucketWebsiteOutputOutputTypeDef",
     "WebsiteConfigurationTypeDef",
+    "ServerSideEncryptionConfigurationOutputTypeDef",
     "ServerSideEncryptionConfigurationTypeDef",
-    "SelectObjectContentEventStreamTypeDef",
+    "SelectObjectContentEventStreamOutputTypeDef",
+    "IntelligentTieringConfigurationOutputTypeDef",
+    "LifecycleRuleOutputTypeDef",
+    "MetricsConfigurationOutputTypeDef",
     "IntelligentTieringConfigurationTypeDef",
     "LifecycleRuleTypeDef",
     "MetricsConfigurationTypeDef",
+    "StorageClassAnalysisOutputTypeDef",
     "StorageClassAnalysisTypeDef",
-    "GetObjectLockConfigurationOutputTypeDef",
+    "GetObjectLockConfigurationOutputOutputTypeDef",
     "PutObjectLockConfigurationRequestRequestTypeDef",
+    "LambdaFunctionConfigurationOutputTypeDef",
+    "QueueConfigurationOutputTypeDef",
+    "TopicConfigurationOutputTypeDef",
     "LambdaFunctionConfigurationTypeDef",
     "QueueConfigurationTypeDef",
     "TopicConfigurationTypeDef",
+    "GetBucketLoggingOutputOutputTypeDef",
     "PutBucketAclRequestBucketAclPutTypeDef",
     "PutBucketAclRequestRequestTypeDef",
     "PutObjectAclRequestObjectAclPutTypeDef",
     "PutObjectAclRequestRequestTypeDef",
     "OutputLocationTypeDef",
     "BucketLoggingStatusTypeDef",
-    "GetBucketLoggingOutputTypeDef",
+    "InventoryDestinationOutputTypeDef",
     "InventoryDestinationTypeDef",
     "PutBucketLifecycleRequestBucketLifecyclePutTypeDef",
     "PutBucketLifecycleRequestRequestTypeDef",
+    "ReplicationRuleOutputTypeDef",
     "ReplicationRuleTypeDef",
     "PutBucketWebsiteRequestBucketWebsitePutTypeDef",
     "PutBucketWebsiteRequestRequestTypeDef",
-    "GetBucketEncryptionOutputTypeDef",
+    "GetBucketEncryptionOutputOutputTypeDef",
     "PutBucketEncryptionRequestRequestTypeDef",
-    "SelectObjectContentOutputTypeDef",
-    "GetBucketIntelligentTieringConfigurationOutputTypeDef",
-    "ListBucketIntelligentTieringConfigurationsOutputTypeDef",
+    "SelectObjectContentOutputOutputTypeDef",
+    "GetBucketIntelligentTieringConfigurationOutputOutputTypeDef",
+    "ListBucketIntelligentTieringConfigurationsOutputOutputTypeDef",
+    "GetBucketLifecycleConfigurationOutputOutputTypeDef",
+    "GetBucketMetricsConfigurationOutputOutputTypeDef",
+    "ListBucketMetricsConfigurationsOutputOutputTypeDef",
     "PutBucketIntelligentTieringConfigurationRequestRequestTypeDef",
     "BucketLifecycleConfigurationTypeDef",
-    "GetBucketLifecycleConfigurationOutputTypeDef",
-    "GetBucketMetricsConfigurationOutputTypeDef",
-    "ListBucketMetricsConfigurationsOutputTypeDef",
     "PutBucketMetricsConfigurationRequestRequestTypeDef",
+    "AnalyticsConfigurationOutputTypeDef",
     "AnalyticsConfigurationTypeDef",
-    "NotificationConfigurationResponseMetadataTypeDef",
+    "NotificationConfigurationOutputTypeDef",
     "NotificationConfigurationTypeDef",
     "RestoreRequestTypeDef",
     "PutBucketLoggingRequestBucketLoggingPutTypeDef",
     "PutBucketLoggingRequestRequestTypeDef",
+    "InventoryConfigurationOutputTypeDef",
     "InventoryConfigurationTypeDef",
+    "ReplicationConfigurationOutputTypeDef",
     "ReplicationConfigurationTypeDef",
     "PutBucketLifecycleConfigurationRequestBucketLifecycleConfigurationPutTypeDef",
     "PutBucketLifecycleConfigurationRequestRequestTypeDef",
-    "GetBucketAnalyticsConfigurationOutputTypeDef",
-    "ListBucketAnalyticsConfigurationsOutputTypeDef",
+    "GetBucketAnalyticsConfigurationOutputOutputTypeDef",
+    "ListBucketAnalyticsConfigurationsOutputOutputTypeDef",
     "PutBucketAnalyticsConfigurationRequestRequestTypeDef",
     "PutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef",
     "PutBucketNotificationConfigurationRequestRequestTypeDef",
     "RestoreObjectRequestObjectRestoreObjectTypeDef",
     "RestoreObjectRequestObjectSummaryRestoreObjectTypeDef",
     "RestoreObjectRequestRequestTypeDef",
-    "GetBucketInventoryConfigurationOutputTypeDef",
-    "ListBucketInventoryConfigurationsOutputTypeDef",
+    "GetBucketInventoryConfigurationOutputOutputTypeDef",
+    "ListBucketInventoryConfigurationsOutputOutputTypeDef",
     "PutBucketInventoryConfigurationRequestRequestTypeDef",
-    "GetBucketReplicationOutputTypeDef",
+    "GetBucketReplicationOutputOutputTypeDef",
     "PutBucketReplicationRequestRequestTypeDef",
 )
 
+AbortIncompleteMultipartUploadOutputTypeDef = TypedDict(
+    "AbortIncompleteMultipartUploadOutputTypeDef",
+    {
+        "DaysAfterInitiation": int,
+    },
+)
+
 AbortIncompleteMultipartUploadTypeDef = TypedDict(
     "AbortIncompleteMultipartUploadTypeDef",
     {
         "DaysAfterInitiation": int,
     },
+    total=False,
 )
 
-AbortMultipartUploadOutputTypeDef = TypedDict(
-    "AbortMultipartUploadOutputTypeDef",
+AbortMultipartUploadOutputOutputTypeDef = TypedDict(
+    "AbortMultipartUploadOutputOutputTypeDef",
     {
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AbortMultipartUploadRequestMultipartUploadAbortTypeDef = TypedDict(
@@ -511,41 +597,80 @@
 
 OwnerTypeDef = TypedDict(
     "OwnerTypeDef",
     {
         "DisplayName": str,
         "ID": str,
     },
+    total=False,
+)
+
+AccessControlTranslationOutputTypeDef = TypedDict(
+    "AccessControlTranslationOutputTypeDef",
+    {
+        "Owner": Literal["Destination"],
+    },
 )
 
 AccessControlTranslationTypeDef = TypedDict(
     "AccessControlTranslationTypeDef",
     {
         "Owner": Literal["Destination"],
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-AnalyticsS3BucketDestinationTypeDef = TypedDict(
-    "AnalyticsS3BucketDestinationTypeDef",
+AnalyticsS3BucketDestinationOutputTypeDef = TypedDict(
+    "AnalyticsS3BucketDestinationOutputTypeDef",
     {
         "Format": Literal["CSV"],
         "BucketAccountId": str,
         "Bucket": str,
         "Prefix": str,
     },
 )
 
+_RequiredAnalyticsS3BucketDestinationTypeDef = TypedDict(
+    "_RequiredAnalyticsS3BucketDestinationTypeDef",
+    {
+        "Format": Literal["CSV"],
+        "Bucket": str,
+    },
+)
+_OptionalAnalyticsS3BucketDestinationTypeDef = TypedDict(
+    "_OptionalAnalyticsS3BucketDestinationTypeDef",
+    {
+        "BucketAccountId": str,
+        "Prefix": str,
+    },
+    total=False,
+)
+
+
+class AnalyticsS3BucketDestinationTypeDef(
+    _RequiredAnalyticsS3BucketDestinationTypeDef, _OptionalAnalyticsS3BucketDestinationTypeDef
+):
+    pass
+
+
 _RequiredCopySourceTypeDef = TypedDict(
     "_RequiredCopySourceTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
 )
@@ -606,16 +731,16 @@
 
 class BucketDownloadFileobjRequestTypeDef(
     _RequiredBucketDownloadFileobjRequestTypeDef, _OptionalBucketDownloadFileobjRequestTypeDef
 ):
     pass
 
 
-BucketTypeDef = TypedDict(
-    "BucketTypeDef",
+BucketOutputTypeDef = TypedDict(
+    "BucketOutputTypeDef",
     {
         "Name": str,
         "CreationDate": datetime,
     },
 )
 
 _RequiredBucketUploadFileRequestTypeDef = TypedDict(
@@ -662,16 +787,39 @@
 
 class BucketUploadFileobjRequestTypeDef(
     _RequiredBucketUploadFileobjRequestTypeDef, _OptionalBucketUploadFileobjRequestTypeDef
 ):
     pass
 
 
-CORSRuleTypeDef = TypedDict(
-    "CORSRuleTypeDef",
+_RequiredCORSRuleTypeDef = TypedDict(
+    "_RequiredCORSRuleTypeDef",
+    {
+        "AllowedMethods": Sequence[str],
+        "AllowedOrigins": Sequence[str],
+    },
+)
+_OptionalCORSRuleTypeDef = TypedDict(
+    "_OptionalCORSRuleTypeDef",
+    {
+        "ID": str,
+        "AllowedHeaders": Sequence[str],
+        "ExposeHeaders": Sequence[str],
+        "MaxAgeSeconds": int,
+    },
+    total=False,
+)
+
+
+class CORSRuleTypeDef(_RequiredCORSRuleTypeDef, _OptionalCORSRuleTypeDef):
+    pass
+
+
+CORSRuleOutputTypeDef = TypedDict(
+    "CORSRuleOutputTypeDef",
     {
         "ID": str,
         "AllowedHeaders": List[str],
         "AllowedMethods": List[str],
         "AllowedOrigins": List[str],
         "ExposeHeaders": List[str],
         "MaxAgeSeconds": int,
@@ -700,16 +848,16 @@
         "RecordDelimiter": str,
         "FieldDelimiter": str,
         "QuoteCharacter": str,
     },
     total=False,
 )
 
-ChecksumTypeDef = TypedDict(
-    "ChecksumTypeDef",
+ChecksumOutputTypeDef = TypedDict(
+    "ChecksumOutputTypeDef",
     {
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
         "ChecksumSHA256": str,
     },
 )
@@ -835,34 +983,46 @@
 
 class ClientUploadFileobjRequestTypeDef(
     _RequiredClientUploadFileobjRequestTypeDef, _OptionalClientUploadFileobjRequestTypeDef
 ):
     pass
 
 
+CloudFunctionConfigurationOutputTypeDef = TypedDict(
+    "CloudFunctionConfigurationOutputTypeDef",
+    {
+        "Id": str,
+        "Event": EventType,
+        "Events": List[EventType],
+        "CloudFunction": str,
+        "InvocationRole": str,
+    },
+)
+
 CloudFunctionConfigurationTypeDef = TypedDict(
     "CloudFunctionConfigurationTypeDef",
     {
         "Id": str,
         "Event": EventType,
-        "Events": List[EventType],
+        "Events": Sequence[EventType],
         "CloudFunction": str,
         "InvocationRole": str,
     },
+    total=False,
 )
 
-CommonPrefixTypeDef = TypedDict(
-    "CommonPrefixTypeDef",
+CommonPrefixOutputTypeDef = TypedDict(
+    "CommonPrefixOutputTypeDef",
     {
         "Prefix": str,
     },
 )
 
-CompleteMultipartUploadOutputTypeDef = TypedDict(
-    "CompleteMultipartUploadOutputTypeDef",
+CompleteMultipartUploadOutputOutputTypeDef = TypedDict(
+    "CompleteMultipartUploadOutputOutputTypeDef",
     {
         "Location": str,
         "Bucket": str,
         "Key": str,
         "Expiration": str,
         "ETag": str,
         "ChecksumCRC32": str,
@@ -887,24 +1047,33 @@
         "ChecksumSHA1": str,
         "ChecksumSHA256": str,
         "PartNumber": int,
     },
     total=False,
 )
 
+ConditionOutputTypeDef = TypedDict(
+    "ConditionOutputTypeDef",
+    {
+        "HttpErrorCodeReturnedEquals": str,
+        "KeyPrefixEquals": str,
+    },
+)
+
 ConditionTypeDef = TypedDict(
     "ConditionTypeDef",
     {
         "HttpErrorCodeReturnedEquals": str,
         "KeyPrefixEquals": str,
     },
+    total=False,
 )
 
-CopyObjectResultTypeDef = TypedDict(
-    "CopyObjectResultTypeDef",
+CopyObjectResultOutputTypeDef = TypedDict(
+    "CopyObjectResultOutputTypeDef",
     {
         "ETag": str,
         "LastModified": datetime,
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
         "ChecksumSHA256": str,
@@ -1024,16 +1193,16 @@
 class CopyObjectRequestObjectSummaryCopyFromTypeDef(
     _RequiredCopyObjectRequestObjectSummaryCopyFromTypeDef,
     _OptionalCopyObjectRequestObjectSummaryCopyFromTypeDef,
 ):
     pass
 
 
-CopyPartResultTypeDef = TypedDict(
-    "CopyPartResultTypeDef",
+CopyPartResultOutputTypeDef = TypedDict(
+    "CopyPartResultOutputTypeDef",
     {
         "ETag": str,
         "LastModified": datetime,
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
         "ChecksumSHA256": str,
@@ -1044,24 +1213,24 @@
     "CreateBucketConfigurationTypeDef",
     {
         "LocationConstraint": BucketLocationConstraintType,
     },
     total=False,
 )
 
-CreateBucketOutputTypeDef = TypedDict(
-    "CreateBucketOutputTypeDef",
+CreateBucketOutputOutputTypeDef = TypedDict(
+    "CreateBucketOutputOutputTypeDef",
     {
         "Location": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateMultipartUploadOutputTypeDef = TypedDict(
-    "CreateMultipartUploadOutputTypeDef",
+CreateMultipartUploadOutputOutputTypeDef = TypedDict(
+    "CreateMultipartUploadOutputOutputTypeDef",
     {
         "AbortDate": datetime,
         "AbortRuleId": str,
         "Bucket": str,
         "Key": str,
         "UploadId": str,
         "ServerSideEncryption": ServerSideEncryptionType,
@@ -1192,21 +1361,31 @@
 class CreateMultipartUploadRequestRequestTypeDef(
     _RequiredCreateMultipartUploadRequestRequestTypeDef,
     _OptionalCreateMultipartUploadRequestRequestTypeDef,
 ):
     pass
 
 
+DefaultRetentionOutputTypeDef = TypedDict(
+    "DefaultRetentionOutputTypeDef",
+    {
+        "Mode": ObjectLockRetentionModeType,
+        "Days": int,
+        "Years": int,
+    },
+)
+
 DefaultRetentionTypeDef = TypedDict(
     "DefaultRetentionTypeDef",
     {
         "Mode": ObjectLockRetentionModeType,
         "Days": int,
         "Years": int,
     },
+    total=False,
 )
 
 _RequiredDeleteBucketAnalyticsConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteBucketAnalyticsConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
         "Id": str,
@@ -1530,23 +1709,39 @@
 class DeleteBucketWebsiteRequestRequestTypeDef(
     _RequiredDeleteBucketWebsiteRequestRequestTypeDef,
     _OptionalDeleteBucketWebsiteRequestRequestTypeDef,
 ):
     pass
 
 
+OwnerOutputTypeDef = TypedDict(
+    "OwnerOutputTypeDef",
+    {
+        "DisplayName": str,
+        "ID": str,
+    },
+)
+
+DeleteMarkerReplicationOutputTypeDef = TypedDict(
+    "DeleteMarkerReplicationOutputTypeDef",
+    {
+        "Status": DeleteMarkerReplicationStatusType,
+    },
+)
+
 DeleteMarkerReplicationTypeDef = TypedDict(
     "DeleteMarkerReplicationTypeDef",
     {
         "Status": DeleteMarkerReplicationStatusType,
     },
+    total=False,
 )
 
-DeleteObjectOutputTypeDef = TypedDict(
-    "DeleteObjectOutputTypeDef",
+DeleteObjectOutputOutputTypeDef = TypedDict(
+    "DeleteObjectOutputOutputTypeDef",
     {
         "DeleteMarker": bool,
         "VersionId": str,
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1608,16 +1803,16 @@
 
 class DeleteObjectRequestRequestTypeDef(
     _RequiredDeleteObjectRequestRequestTypeDef, _OptionalDeleteObjectRequestRequestTypeDef
 ):
     pass
 
 
-DeleteObjectTaggingOutputTypeDef = TypedDict(
-    "DeleteObjectTaggingOutputTypeDef",
+DeleteObjectTaggingOutputOutputTypeDef = TypedDict(
+    "DeleteObjectTaggingOutputOutputTypeDef",
     {
         "VersionId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDeleteObjectTaggingRequestRequestTypeDef = TypedDict(
@@ -1640,26 +1835,26 @@
 class DeleteObjectTaggingRequestRequestTypeDef(
     _RequiredDeleteObjectTaggingRequestRequestTypeDef,
     _OptionalDeleteObjectTaggingRequestRequestTypeDef,
 ):
     pass
 
 
-DeletedObjectTypeDef = TypedDict(
-    "DeletedObjectTypeDef",
+DeletedObjectOutputTypeDef = TypedDict(
+    "DeletedObjectOutputTypeDef",
     {
         "Key": str,
         "VersionId": str,
         "DeleteMarker": bool,
         "DeleteMarkerVersionId": str,
     },
 )
 
-ErrorTypeDef = TypedDict(
-    "ErrorTypeDef",
+ErrorOutputTypeDef = TypedDict(
+    "ErrorOutputTypeDef",
     {
         "Key": str,
         "VersionId": str,
         "Code": str,
         "Message": str,
     },
 )
@@ -1701,19 +1896,27 @@
 )
 
 
 class ObjectIdentifierTypeDef(_RequiredObjectIdentifierTypeDef, _OptionalObjectIdentifierTypeDef):
     pass
 
 
+EncryptionConfigurationOutputTypeDef = TypedDict(
+    "EncryptionConfigurationOutputTypeDef",
+    {
+        "ReplicaKmsKeyID": str,
+    },
+)
+
 EncryptionConfigurationTypeDef = TypedDict(
     "EncryptionConfigurationTypeDef",
     {
         "ReplicaKmsKeyID": str,
     },
+    total=False,
 )
 
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1735,14 +1938,21 @@
 )
 
 
 class EncryptionTypeDef(_RequiredEncryptionTypeDef, _OptionalEncryptionTypeDef):
     pass
 
 
+ErrorDocumentOutputTypeDef = TypedDict(
+    "ErrorDocumentOutputTypeDef",
+    {
+        "Key": str,
+    },
+)
+
 ErrorDocumentResponseMetadataTypeDef = TypedDict(
     "ErrorDocumentResponseMetadataTypeDef",
     {
         "Key": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1750,31 +1960,47 @@
 ErrorDocumentTypeDef = TypedDict(
     "ErrorDocumentTypeDef",
     {
         "Key": str,
     },
 )
 
+ExistingObjectReplicationOutputTypeDef = TypedDict(
+    "ExistingObjectReplicationOutputTypeDef",
+    {
+        "Status": ExistingObjectReplicationStatusType,
+    },
+)
+
 ExistingObjectReplicationTypeDef = TypedDict(
     "ExistingObjectReplicationTypeDef",
     {
         "Status": ExistingObjectReplicationStatusType,
     },
 )
 
+FilterRuleOutputTypeDef = TypedDict(
+    "FilterRuleOutputTypeDef",
+    {
+        "Name": FilterRuleNameType,
+        "Value": str,
+    },
+)
+
 FilterRuleTypeDef = TypedDict(
     "FilterRuleTypeDef",
     {
         "Name": FilterRuleNameType,
         "Value": str,
     },
+    total=False,
 )
 
-GetBucketAccelerateConfigurationOutputTypeDef = TypedDict(
-    "GetBucketAccelerateConfigurationOutputTypeDef",
+GetBucketAccelerateConfigurationOutputOutputTypeDef = TypedDict(
+    "GetBucketAccelerateConfigurationOutputOutputTypeDef",
     {
         "Status": BucketAccelerateStatusType,
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1959,16 +2185,16 @@
 class GetBucketLifecycleRequestRequestTypeDef(
     _RequiredGetBucketLifecycleRequestRequestTypeDef,
     _OptionalGetBucketLifecycleRequestRequestTypeDef,
 ):
     pass
 
 
-GetBucketLocationOutputTypeDef = TypedDict(
-    "GetBucketLocationOutputTypeDef",
+GetBucketLocationOutputOutputTypeDef = TypedDict(
+    "GetBucketLocationOutputOutputTypeDef",
     {
         "LocationConstraint": BucketLocationConstraintType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetBucketLocationRequestRequestTypeDef = TypedDict(
@@ -2076,16 +2302,16 @@
 class GetBucketOwnershipControlsRequestRequestTypeDef(
     _RequiredGetBucketOwnershipControlsRequestRequestTypeDef,
     _OptionalGetBucketOwnershipControlsRequestRequestTypeDef,
 ):
     pass
 
 
-GetBucketPolicyOutputTypeDef = TypedDict(
-    "GetBucketPolicyOutputTypeDef",
+GetBucketPolicyOutputOutputTypeDef = TypedDict(
+    "GetBucketPolicyOutputOutputTypeDef",
     {
         "Policy": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetBucketPolicyRequestRequestTypeDef = TypedDict(
@@ -2105,16 +2331,16 @@
 
 class GetBucketPolicyRequestRequestTypeDef(
     _RequiredGetBucketPolicyRequestRequestTypeDef, _OptionalGetBucketPolicyRequestRequestTypeDef
 ):
     pass
 
 
-PolicyStatusTypeDef = TypedDict(
-    "PolicyStatusTypeDef",
+PolicyStatusOutputTypeDef = TypedDict(
+    "PolicyStatusOutputTypeDef",
     {
         "IsPublic": bool,
     },
 )
 
 _RequiredGetBucketPolicyStatusRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketPolicyStatusRequestRequestTypeDef",
@@ -2156,16 +2382,16 @@
 class GetBucketReplicationRequestRequestTypeDef(
     _RequiredGetBucketReplicationRequestRequestTypeDef,
     _OptionalGetBucketReplicationRequestRequestTypeDef,
 ):
     pass
 
 
-GetBucketRequestPaymentOutputTypeDef = TypedDict(
-    "GetBucketRequestPaymentOutputTypeDef",
+GetBucketRequestPaymentOutputOutputTypeDef = TypedDict(
+    "GetBucketRequestPaymentOutputOutputTypeDef",
     {
         "Payer": PayerType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetBucketRequestPaymentRequestRequestTypeDef = TypedDict(
@@ -2207,16 +2433,16 @@
 
 class GetBucketTaggingRequestRequestTypeDef(
     _RequiredGetBucketTaggingRequestRequestTypeDef, _OptionalGetBucketTaggingRequestRequestTypeDef
 ):
     pass
 
 
-GetBucketVersioningOutputTypeDef = TypedDict(
-    "GetBucketVersioningOutputTypeDef",
+GetBucketVersioningOutputOutputTypeDef = TypedDict(
+    "GetBucketVersioningOutputOutputTypeDef",
     {
         "Status": BucketVersioningStatusType,
         "MFADelete": MFADeleteStatusType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -2238,23 +2464,23 @@
 class GetBucketVersioningRequestRequestTypeDef(
     _RequiredGetBucketVersioningRequestRequestTypeDef,
     _OptionalGetBucketVersioningRequestRequestTypeDef,
 ):
     pass
 
 
-IndexDocumentTypeDef = TypedDict(
-    "IndexDocumentTypeDef",
+IndexDocumentOutputTypeDef = TypedDict(
+    "IndexDocumentOutputTypeDef",
     {
         "Suffix": str,
     },
 )
 
-RedirectAllRequestsToTypeDef = TypedDict(
-    "RedirectAllRequestsToTypeDef",
+RedirectAllRequestsToOutputTypeDef = TypedDict(
+    "RedirectAllRequestsToOutputTypeDef",
     {
         "HostName": str,
         "Protocol": ProtocolType,
     },
 )
 
 _RequiredGetBucketWebsiteRequestRequestTypeDef = TypedDict(
@@ -2298,16 +2524,16 @@
 
 class GetObjectAclRequestRequestTypeDef(
     _RequiredGetObjectAclRequestRequestTypeDef, _OptionalGetObjectAclRequestRequestTypeDef
 ):
     pass
 
 
-ObjectPartTypeDef = TypedDict(
-    "ObjectPartTypeDef",
+ObjectPartOutputTypeDef = TypedDict(
+    "ObjectPartOutputTypeDef",
     {
         "PartNumber": int,
         "Size": int,
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
         "ChecksumSHA256": str,
@@ -2341,16 +2567,16 @@
 class GetObjectAttributesRequestRequestTypeDef(
     _RequiredGetObjectAttributesRequestRequestTypeDef,
     _OptionalGetObjectAttributesRequestRequestTypeDef,
 ):
     pass
 
 
-ObjectLockLegalHoldTypeDef = TypedDict(
-    "ObjectLockLegalHoldTypeDef",
+ObjectLockLegalHoldOutputTypeDef = TypedDict(
+    "ObjectLockLegalHoldOutputTypeDef",
     {
         "Status": ObjectLockLegalHoldStatusType,
     },
 )
 
 _RequiredGetObjectLegalHoldRequestRequestTypeDef = TypedDict(
     "_RequiredGetObjectLegalHoldRequestRequestTypeDef",
@@ -2395,16 +2621,16 @@
 class GetObjectLockConfigurationRequestRequestTypeDef(
     _RequiredGetObjectLockConfigurationRequestRequestTypeDef,
     _OptionalGetObjectLockConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-GetObjectOutputTypeDef = TypedDict(
-    "GetObjectOutputTypeDef",
+GetObjectOutputOutputTypeDef = TypedDict(
+    "GetObjectOutputOutputTypeDef",
     {
         "Body": StreamingBody,
         "DeleteMarker": bool,
         "AcceptRanges": str,
         "Expiration": str,
         "Restore": str,
         "LastModified": datetime,
@@ -2555,16 +2781,16 @@
 
 class GetObjectRequestRequestTypeDef(
     _RequiredGetObjectRequestRequestTypeDef, _OptionalGetObjectRequestRequestTypeDef
 ):
     pass
 
 
-ObjectLockRetentionTypeDef = TypedDict(
-    "ObjectLockRetentionTypeDef",
+ObjectLockRetentionOutputTypeDef = TypedDict(
+    "ObjectLockRetentionOutputTypeDef",
     {
         "Mode": ObjectLockRetentionModeType,
         "RetainUntilDate": datetime,
     },
 )
 
 _RequiredGetObjectRetentionRequestRequestTypeDef = TypedDict(
@@ -2612,16 +2838,16 @@
 
 class GetObjectTaggingRequestRequestTypeDef(
     _RequiredGetObjectTaggingRequestRequestTypeDef, _OptionalGetObjectTaggingRequestRequestTypeDef
 ):
     pass
 
 
-GetObjectTorrentOutputTypeDef = TypedDict(
-    "GetObjectTorrentOutputTypeDef",
+GetObjectTorrentOutputOutputTypeDef = TypedDict(
+    "GetObjectTorrentOutputOutputTypeDef",
     {
         "Body": StreamingBody,
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -2644,16 +2870,16 @@
 
 class GetObjectTorrentRequestRequestTypeDef(
     _RequiredGetObjectTorrentRequestRequestTypeDef, _OptionalGetObjectTorrentRequestRequestTypeDef
 ):
     pass
 
 
-PublicAccessBlockConfigurationTypeDef = TypedDict(
-    "PublicAccessBlockConfigurationTypeDef",
+PublicAccessBlockConfigurationOutputTypeDef = TypedDict(
+    "PublicAccessBlockConfigurationOutputTypeDef",
     {
         "BlockPublicAcls": bool,
         "IgnorePublicAcls": bool,
         "BlockPublicPolicy": bool,
         "RestrictPublicBuckets": bool,
     },
 )
@@ -2683,25 +2909,47 @@
 GlacierJobParametersTypeDef = TypedDict(
     "GlacierJobParametersTypeDef",
     {
         "Tier": TierType,
     },
 )
 
-GranteeTypeDef = TypedDict(
-    "GranteeTypeDef",
+GranteeOutputTypeDef = TypedDict(
+    "GranteeOutputTypeDef",
     {
         "DisplayName": str,
         "EmailAddress": str,
         "ID": str,
         "Type": TypeType,
         "URI": str,
     },
 )
 
+_RequiredGranteeTypeDef = TypedDict(
+    "_RequiredGranteeTypeDef",
+    {
+        "Type": TypeType,
+    },
+)
+_OptionalGranteeTypeDef = TypedDict(
+    "_OptionalGranteeTypeDef",
+    {
+        "DisplayName": str,
+        "EmailAddress": str,
+        "ID": str,
+        "URI": str,
+    },
+    total=False,
+)
+
+
+class GranteeTypeDef(_RequiredGranteeTypeDef, _OptionalGranteeTypeDef):
+    pass
+
+
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -2724,16 +2972,16 @@
 
 class HeadBucketRequestRequestTypeDef(
     _RequiredHeadBucketRequestRequestTypeDef, _OptionalHeadBucketRequestRequestTypeDef
 ):
     pass
 
 
-HeadObjectOutputTypeDef = TypedDict(
-    "HeadObjectOutputTypeDef",
+HeadObjectOutputOutputTypeDef = TypedDict(
+    "HeadObjectOutputOutputTypeDef",
     {
         "DeleteMarker": bool,
         "AcceptRanges": str,
         "Expiration": str,
         "Restore": str,
         "ArchiveStatus": ArchiveStatusType,
         "LastModified": datetime,
@@ -2826,61 +3074,97 @@
     "IndexDocumentResponseMetadataTypeDef",
     {
         "Suffix": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-InitiatorResponseMetadataTypeDef = TypedDict(
-    "InitiatorResponseMetadataTypeDef",
+IndexDocumentTypeDef = TypedDict(
+    "IndexDocumentTypeDef",
+    {
+        "Suffix": str,
+    },
+)
+
+InitiatorOutputTypeDef = TypedDict(
+    "InitiatorOutputTypeDef",
     {
         "ID": str,
         "DisplayName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-InitiatorTypeDef = TypedDict(
-    "InitiatorTypeDef",
+InitiatorResponseMetadataTypeDef = TypedDict(
+    "InitiatorResponseMetadataTypeDef",
     {
         "ID": str,
         "DisplayName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 JSONInputTypeDef = TypedDict(
     "JSONInputTypeDef",
     {
         "Type": JSONTypeType,
     },
     total=False,
 )
 
+TieringOutputTypeDef = TypedDict(
+    "TieringOutputTypeDef",
+    {
+        "Days": int,
+        "AccessTier": IntelligentTieringAccessTierType,
+    },
+)
+
 TieringTypeDef = TypedDict(
     "TieringTypeDef",
     {
         "Days": int,
         "AccessTier": IntelligentTieringAccessTierType,
     },
 )
 
+InventoryFilterOutputTypeDef = TypedDict(
+    "InventoryFilterOutputTypeDef",
+    {
+        "Prefix": str,
+    },
+)
+
+InventoryScheduleOutputTypeDef = TypedDict(
+    "InventoryScheduleOutputTypeDef",
+    {
+        "Frequency": InventoryFrequencyType,
+    },
+)
+
 InventoryFilterTypeDef = TypedDict(
     "InventoryFilterTypeDef",
     {
         "Prefix": str,
     },
 )
 
 InventoryScheduleTypeDef = TypedDict(
     "InventoryScheduleTypeDef",
     {
         "Frequency": InventoryFrequencyType,
     },
 )
 
+SSEKMSOutputTypeDef = TypedDict(
+    "SSEKMSOutputTypeDef",
+    {
+        "KeyId": str,
+    },
+)
+
 SSEKMSTypeDef = TypedDict(
     "SSEKMSTypeDef",
     {
         "KeyId": str,
     },
 )
 
@@ -2888,47 +3172,86 @@
     "JSONOutputTypeDef",
     {
         "RecordDelimiter": str,
     },
     total=False,
 )
 
+LifecycleExpirationOutputTypeDef = TypedDict(
+    "LifecycleExpirationOutputTypeDef",
+    {
+        "Date": datetime,
+        "Days": int,
+        "ExpiredObjectDeleteMarker": bool,
+    },
+)
+
 LifecycleExpirationTypeDef = TypedDict(
     "LifecycleExpirationTypeDef",
     {
-        "Date": datetime,
+        "Date": Union[datetime, str],
         "Days": int,
         "ExpiredObjectDeleteMarker": bool,
     },
+    total=False,
+)
+
+NoncurrentVersionExpirationOutputTypeDef = TypedDict(
+    "NoncurrentVersionExpirationOutputTypeDef",
+    {
+        "NoncurrentDays": int,
+        "NewerNoncurrentVersions": int,
+    },
+)
+
+NoncurrentVersionTransitionOutputTypeDef = TypedDict(
+    "NoncurrentVersionTransitionOutputTypeDef",
+    {
+        "NoncurrentDays": int,
+        "StorageClass": TransitionStorageClassType,
+        "NewerNoncurrentVersions": int,
+    },
+)
+
+TransitionOutputTypeDef = TypedDict(
+    "TransitionOutputTypeDef",
+    {
+        "Date": datetime,
+        "Days": int,
+        "StorageClass": TransitionStorageClassType,
+    },
 )
 
 NoncurrentVersionExpirationTypeDef = TypedDict(
     "NoncurrentVersionExpirationTypeDef",
     {
         "NoncurrentDays": int,
         "NewerNoncurrentVersions": int,
     },
+    total=False,
 )
 
 NoncurrentVersionTransitionTypeDef = TypedDict(
     "NoncurrentVersionTransitionTypeDef",
     {
         "NoncurrentDays": int,
         "StorageClass": TransitionStorageClassType,
         "NewerNoncurrentVersions": int,
     },
+    total=False,
 )
 
 TransitionTypeDef = TypedDict(
     "TransitionTypeDef",
     {
-        "Date": datetime,
+        "Date": Union[datetime, str],
         "Days": int,
         "StorageClass": TransitionStorageClassType,
     },
+    total=False,
 )
 
 _RequiredListBucketAnalyticsConfigurationsRequestRequestTypeDef = TypedDict(
     "_RequiredListBucketAnalyticsConfigurationsRequestRequestTypeDef",
     {
         "Bucket": str,
     },
@@ -3244,16 +3567,16 @@
 
 class ListObjectsV2RequestRequestTypeDef(
     _RequiredListObjectsV2RequestRequestTypeDef, _OptionalListObjectsV2RequestRequestTypeDef
 ):
     pass
 
 
-PartTypeDef = TypedDict(
-    "PartTypeDef",
+PartOutputTypeDef = TypedDict(
+    "PartOutputTypeDef",
     {
         "PartNumber": int,
         "LastModified": datetime,
         "ETag": str,
         "Size": int,
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
@@ -3325,39 +3648,69 @@
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
+ReplicationTimeValueOutputTypeDef = TypedDict(
+    "ReplicationTimeValueOutputTypeDef",
+    {
+        "Minutes": int,
+    },
+)
+
 ReplicationTimeValueTypeDef = TypedDict(
     "ReplicationTimeValueTypeDef",
     {
         "Minutes": int,
     },
+    total=False,
+)
+
+QueueConfigurationDeprecatedOutputTypeDef = TypedDict(
+    "QueueConfigurationDeprecatedOutputTypeDef",
+    {
+        "Id": str,
+        "Event": EventType,
+        "Events": List[EventType],
+        "Queue": str,
+    },
+)
+
+TopicConfigurationDeprecatedOutputTypeDef = TypedDict(
+    "TopicConfigurationDeprecatedOutputTypeDef",
+    {
+        "Id": str,
+        "Events": List[EventType],
+        "Event": EventType,
+        "Topic": str,
+    },
 )
 
 QueueConfigurationDeprecatedTypeDef = TypedDict(
     "QueueConfigurationDeprecatedTypeDef",
     {
         "Id": str,
         "Event": EventType,
-        "Events": List[EventType],
+        "Events": Sequence[EventType],
         "Queue": str,
     },
+    total=False,
 )
 
 TopicConfigurationDeprecatedTypeDef = TypedDict(
     "TopicConfigurationDeprecatedTypeDef",
     {
         "Id": str,
-        "Events": List[EventType],
+        "Events": Sequence[EventType],
         "Event": EventType,
         "Topic": str,
     },
+    total=False,
 )
 
 _RequiredObjectDownloadFileRequestTypeDef = TypedDict(
     "_RequiredObjectDownloadFileRequestTypeDef",
     {
         "Filename": str,
     },
@@ -3398,16 +3751,33 @@
 
 class ObjectDownloadFileobjRequestTypeDef(
     _RequiredObjectDownloadFileobjRequestTypeDef, _OptionalObjectDownloadFileobjRequestTypeDef
 ):
     pass
 
 
-RestoreStatusTypeDef = TypedDict(
-    "RestoreStatusTypeDef",
+ObjectLockLegalHoldTypeDef = TypedDict(
+    "ObjectLockLegalHoldTypeDef",
+    {
+        "Status": ObjectLockLegalHoldStatusType,
+    },
+    total=False,
+)
+
+ObjectLockRetentionTypeDef = TypedDict(
+    "ObjectLockRetentionTypeDef",
+    {
+        "Mode": ObjectLockRetentionModeType,
+        "RetainUntilDate": Union[datetime, str],
+    },
+    total=False,
+)
+
+RestoreStatusOutputTypeDef = TypedDict(
+    "RestoreStatusOutputTypeDef",
     {
         "IsRestoreInProgress": bool,
         "RestoreExpiryDate": datetime,
     },
 )
 
 _RequiredObjectUploadFileRequestTypeDef = TypedDict(
@@ -3461,14 +3831,21 @@
     {
         "DisplayName": str,
         "ID": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+OwnershipControlsRuleOutputTypeDef = TypedDict(
+    "OwnershipControlsRuleOutputTypeDef",
+    {
+        "ObjectOwnership": ObjectOwnershipType,
+    },
+)
+
 OwnershipControlsRuleTypeDef = TypedDict(
     "OwnershipControlsRuleTypeDef",
     {
         "ObjectOwnership": ObjectOwnershipType,
     },
 )
 
@@ -3478,23 +3855,34 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-ProgressTypeDef = TypedDict(
-    "ProgressTypeDef",
+ProgressOutputTypeDef = TypedDict(
+    "ProgressOutputTypeDef",
     {
         "BytesScanned": int,
         "BytesProcessed": int,
         "BytesReturned": int,
     },
 )
 
+PublicAccessBlockConfigurationTypeDef = TypedDict(
+    "PublicAccessBlockConfigurationTypeDef",
+    {
+        "BlockPublicAcls": bool,
+        "IgnorePublicAcls": bool,
+        "BlockPublicPolicy": bool,
+        "RestrictPublicBuckets": bool,
+    },
+    total=False,
+)
+
 _RequiredPutBucketPolicyRequestBucketPolicyPutTypeDef = TypedDict(
     "_RequiredPutBucketPolicyRequestBucketPolicyPutTypeDef",
     {
         "Policy": str,
     },
 )
 _OptionalPutBucketPolicyRequestBucketPolicyPutTypeDef = TypedDict(
@@ -3571,40 +3959,40 @@
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "MFA": str,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-PutObjectAclOutputTypeDef = TypedDict(
-    "PutObjectAclOutputTypeDef",
+PutObjectAclOutputOutputTypeDef = TypedDict(
+    "PutObjectAclOutputOutputTypeDef",
     {
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutObjectLegalHoldOutputTypeDef = TypedDict(
-    "PutObjectLegalHoldOutputTypeDef",
+PutObjectLegalHoldOutputOutputTypeDef = TypedDict(
+    "PutObjectLegalHoldOutputOutputTypeDef",
     {
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutObjectLockConfigurationOutputTypeDef = TypedDict(
-    "PutObjectLockConfigurationOutputTypeDef",
+PutObjectLockConfigurationOutputOutputTypeDef = TypedDict(
+    "PutObjectLockConfigurationOutputOutputTypeDef",
     {
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutObjectOutputTypeDef = TypedDict(
-    "PutObjectOutputTypeDef",
+PutObjectOutputOutputTypeDef = TypedDict(
+    "PutObjectOutputOutputTypeDef",
     {
         "Expiration": str,
         "ETag": str,
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
         "ChecksumSHA256": str,
@@ -3811,55 +4199,95 @@
 
 class PutObjectRequestRequestTypeDef(
     _RequiredPutObjectRequestRequestTypeDef, _OptionalPutObjectRequestRequestTypeDef
 ):
     pass
 
 
-PutObjectRetentionOutputTypeDef = TypedDict(
-    "PutObjectRetentionOutputTypeDef",
+PutObjectRetentionOutputOutputTypeDef = TypedDict(
+    "PutObjectRetentionOutputOutputTypeDef",
     {
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutObjectTaggingOutputTypeDef = TypedDict(
-    "PutObjectTaggingOutputTypeDef",
+PutObjectTaggingOutputOutputTypeDef = TypedDict(
+    "PutObjectTaggingOutputOutputTypeDef",
     {
         "VersionId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RecordsEventTypeDef = TypedDict(
-    "RecordsEventTypeDef",
+RecordsEventOutputTypeDef = TypedDict(
+    "RecordsEventOutputTypeDef",
     {
         "Payload": bytes,
     },
 )
 
 RedirectAllRequestsToResponseMetadataTypeDef = TypedDict(
     "RedirectAllRequestsToResponseMetadataTypeDef",
     {
         "HostName": str,
         "Protocol": ProtocolType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredRedirectAllRequestsToTypeDef = TypedDict(
+    "_RequiredRedirectAllRequestsToTypeDef",
+    {
+        "HostName": str,
+    },
+)
+_OptionalRedirectAllRequestsToTypeDef = TypedDict(
+    "_OptionalRedirectAllRequestsToTypeDef",
+    {
+        "Protocol": ProtocolType,
+    },
+    total=False,
+)
+
+
+class RedirectAllRequestsToTypeDef(
+    _RequiredRedirectAllRequestsToTypeDef, _OptionalRedirectAllRequestsToTypeDef
+):
+    pass
+
+
+RedirectOutputTypeDef = TypedDict(
+    "RedirectOutputTypeDef",
+    {
+        "HostName": str,
+        "HttpRedirectCode": str,
+        "Protocol": ProtocolType,
+        "ReplaceKeyPrefixWith": str,
+        "ReplaceKeyWith": str,
+    },
+)
+
 RedirectTypeDef = TypedDict(
     "RedirectTypeDef",
     {
         "HostName": str,
         "HttpRedirectCode": str,
         "Protocol": ProtocolType,
         "ReplaceKeyPrefixWith": str,
         "ReplaceKeyWith": str,
     },
+    total=False,
+)
+
+ReplicaModificationsOutputTypeDef = TypedDict(
+    "ReplicaModificationsOutputTypeDef",
+    {
+        "Status": ReplicaModificationsStatusType,
+    },
 )
 
 ReplicaModificationsTypeDef = TypedDict(
     "ReplicaModificationsTypeDef",
     {
         "Status": ReplicaModificationsStatusType,
     },
@@ -3880,16 +4308,16 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-RestoreObjectOutputTypeDef = TypedDict(
-    "RestoreObjectOutputTypeDef",
+RestoreObjectOutputOutputTypeDef = TypedDict(
+    "RestoreObjectOutputOutputTypeDef",
     {
         "RequestCharged": Literal["requester"],
         "RestoreOutputPath": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -3907,40 +4335,68 @@
     {
         "Start": int,
         "End": int,
     },
     total=False,
 )
 
-ServerSideEncryptionByDefaultTypeDef = TypedDict(
-    "ServerSideEncryptionByDefaultTypeDef",
+ServerSideEncryptionByDefaultOutputTypeDef = TypedDict(
+    "ServerSideEncryptionByDefaultOutputTypeDef",
     {
         "SSEAlgorithm": ServerSideEncryptionType,
         "KMSMasterKeyID": str,
     },
 )
 
+_RequiredServerSideEncryptionByDefaultTypeDef = TypedDict(
+    "_RequiredServerSideEncryptionByDefaultTypeDef",
+    {
+        "SSEAlgorithm": ServerSideEncryptionType,
+    },
+)
+_OptionalServerSideEncryptionByDefaultTypeDef = TypedDict(
+    "_OptionalServerSideEncryptionByDefaultTypeDef",
+    {
+        "KMSMasterKeyID": str,
+    },
+    total=False,
+)
+
+
+class ServerSideEncryptionByDefaultTypeDef(
+    _RequiredServerSideEncryptionByDefaultTypeDef, _OptionalServerSideEncryptionByDefaultTypeDef
+):
+    pass
+
+
+SseKmsEncryptedObjectsOutputTypeDef = TypedDict(
+    "SseKmsEncryptedObjectsOutputTypeDef",
+    {
+        "Status": SseKmsEncryptedObjectsStatusType,
+    },
+)
+
 SseKmsEncryptedObjectsTypeDef = TypedDict(
     "SseKmsEncryptedObjectsTypeDef",
     {
         "Status": SseKmsEncryptedObjectsStatusType,
     },
 )
 
-StatsTypeDef = TypedDict(
-    "StatsTypeDef",
+StatsOutputTypeDef = TypedDict(
+    "StatsOutputTypeDef",
     {
         "BytesScanned": int,
         "BytesProcessed": int,
         "BytesReturned": int,
     },
 )
 
-UploadPartOutputTypeDef = TypedDict(
-    "UploadPartOutputTypeDef",
+UploadPartOutputOutputTypeDef = TypedDict(
+    "UploadPartOutputOutputTypeDef",
     {
         "ServerSideEncryption": ServerSideEncryptionType,
         "ETag": str,
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
         "ChecksumSHA256": str,
@@ -4089,92 +4545,136 @@
 class PutBucketAccelerateConfigurationRequestRequestTypeDef(
     _RequiredPutBucketAccelerateConfigurationRequestRequestTypeDef,
     _OptionalPutBucketAccelerateConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-DeleteMarkerEntryTypeDef = TypedDict(
-    "DeleteMarkerEntryTypeDef",
+AnalyticsAndOperatorOutputTypeDef = TypedDict(
+    "AnalyticsAndOperatorOutputTypeDef",
+    {
+        "Prefix": str,
+        "Tags": List[TagOutputTypeDef],
+    },
+)
+
+GetBucketTaggingOutputOutputTypeDef = TypedDict(
+    "GetBucketTaggingOutputOutputTypeDef",
+    {
+        "TagSet": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetObjectTaggingOutputOutputTypeDef = TypedDict(
+    "GetObjectTaggingOutputOutputTypeDef",
     {
-        "Owner": OwnerTypeDef,
-        "Key": str,
         "VersionId": str,
-        "IsLatest": bool,
-        "LastModified": datetime,
+        "TagSet": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-AnalyticsAndOperatorTypeDef = TypedDict(
-    "AnalyticsAndOperatorTypeDef",
+IntelligentTieringAndOperatorOutputTypeDef = TypedDict(
+    "IntelligentTieringAndOperatorOutputTypeDef",
     {
         "Prefix": str,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
     },
 )
 
-GetBucketTaggingOutputTypeDef = TypedDict(
-    "GetBucketTaggingOutputTypeDef",
+LifecycleRuleAndOperatorOutputTypeDef = TypedDict(
+    "LifecycleRuleAndOperatorOutputTypeDef",
     {
-        "TagSet": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Prefix": str,
+        "Tags": List[TagOutputTypeDef],
+        "ObjectSizeGreaterThan": int,
+        "ObjectSizeLessThan": int,
     },
 )
 
-GetObjectTaggingOutputTypeDef = TypedDict(
-    "GetObjectTaggingOutputTypeDef",
+MetricsAndOperatorOutputTypeDef = TypedDict(
+    "MetricsAndOperatorOutputTypeDef",
     {
-        "VersionId": str,
-        "TagSet": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Prefix": str,
+        "Tags": List[TagOutputTypeDef],
+        "AccessPointArn": str,
     },
 )
 
+ReplicationRuleAndOperatorOutputTypeDef = TypedDict(
+    "ReplicationRuleAndOperatorOutputTypeDef",
+    {
+        "Prefix": str,
+        "Tags": List[TagOutputTypeDef],
+    },
+)
+
+AnalyticsAndOperatorTypeDef = TypedDict(
+    "AnalyticsAndOperatorTypeDef",
+    {
+        "Prefix": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
 IntelligentTieringAndOperatorTypeDef = TypedDict(
     "IntelligentTieringAndOperatorTypeDef",
     {
         "Prefix": str,
-        "Tags": List[TagTypeDef],
+        "Tags": Sequence[TagTypeDef],
     },
+    total=False,
 )
 
 LifecycleRuleAndOperatorTypeDef = TypedDict(
     "LifecycleRuleAndOperatorTypeDef",
     {
         "Prefix": str,
-        "Tags": List[TagTypeDef],
+        "Tags": Sequence[TagTypeDef],
         "ObjectSizeGreaterThan": int,
         "ObjectSizeLessThan": int,
     },
+    total=False,
 )
 
 MetricsAndOperatorTypeDef = TypedDict(
     "MetricsAndOperatorTypeDef",
     {
         "Prefix": str,
-        "Tags": List[TagTypeDef],
+        "Tags": Sequence[TagTypeDef],
         "AccessPointArn": str,
     },
+    total=False,
 )
 
 ReplicationRuleAndOperatorTypeDef = TypedDict(
     "ReplicationRuleAndOperatorTypeDef",
     {
         "Prefix": str,
-        "Tags": List[TagTypeDef],
+        "Tags": Sequence[TagTypeDef],
     },
+    total=False,
 )
 
 TaggingTypeDef = TypedDict(
     "TaggingTypeDef",
     {
         "TagSet": Sequence[TagTypeDef],
     },
 )
 
+AnalyticsExportDestinationOutputTypeDef = TypedDict(
+    "AnalyticsExportDestinationOutputTypeDef",
+    {
+        "S3BucketDestination": AnalyticsS3BucketDestinationOutputTypeDef,
+    },
+)
+
 AnalyticsExportDestinationTypeDef = TypedDict(
     "AnalyticsExportDestinationTypeDef",
     {
         "S3BucketDestination": AnalyticsS3BucketDestinationTypeDef,
     },
 )
 
@@ -4382,69 +4882,60 @@
 
 class UploadPartCopyRequestRequestTypeDef(
     _RequiredUploadPartCopyRequestRequestTypeDef, _OptionalUploadPartCopyRequestRequestTypeDef
 ):
     pass
 
 
-ListBucketsOutputTypeDef = TypedDict(
-    "ListBucketsOutputTypeDef",
-    {
-        "Buckets": List[BucketTypeDef],
-        "Owner": OwnerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CORSConfigurationTypeDef = TypedDict(
     "CORSConfigurationTypeDef",
     {
         "CORSRules": Sequence[CORSRuleTypeDef],
     },
 )
 
-GetBucketCorsOutputTypeDef = TypedDict(
-    "GetBucketCorsOutputTypeDef",
+GetBucketCorsOutputOutputTypeDef = TypedDict(
+    "GetBucketCorsOutputOutputTypeDef",
     {
-        "CORSRules": List[CORSRuleTypeDef],
+        "CORSRules": List[CORSRuleOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CompletedMultipartUploadTypeDef = TypedDict(
     "CompletedMultipartUploadTypeDef",
     {
         "Parts": Sequence[CompletedPartTypeDef],
     },
     total=False,
 )
 
-CopyObjectOutputTypeDef = TypedDict(
-    "CopyObjectOutputTypeDef",
+CopyObjectOutputOutputTypeDef = TypedDict(
+    "CopyObjectOutputOutputTypeDef",
     {
-        "CopyObjectResult": CopyObjectResultTypeDef,
+        "CopyObjectResult": CopyObjectResultOutputTypeDef,
         "Expiration": str,
         "CopySourceVersionId": str,
         "VersionId": str,
         "ServerSideEncryption": ServerSideEncryptionType,
         "SSECustomerAlgorithm": str,
         "SSECustomerKeyMD5": str,
         "SSEKMSKeyId": str,
         "SSEKMSEncryptionContext": str,
         "BucketKeyEnabled": bool,
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UploadPartCopyOutputTypeDef = TypedDict(
-    "UploadPartCopyOutputTypeDef",
+UploadPartCopyOutputOutputTypeDef = TypedDict(
+    "UploadPartCopyOutputOutputTypeDef",
     {
         "CopySourceVersionId": str,
-        "CopyPartResult": CopyPartResultTypeDef,
+        "CopyPartResult": CopyPartResultOutputTypeDef,
         "ServerSideEncryption": ServerSideEncryptionType,
         "SSECustomerAlgorithm": str,
         "SSECustomerKeyMD5": str,
         "SSEKMSKeyId": str,
         "BucketKeyEnabled": bool,
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -4522,27 +5013,55 @@
 class CreateBucketRequestServiceResourceCreateBucketTypeDef(
     _RequiredCreateBucketRequestServiceResourceCreateBucketTypeDef,
     _OptionalCreateBucketRequestServiceResourceCreateBucketTypeDef,
 ):
     pass
 
 
+ObjectLockRuleOutputTypeDef = TypedDict(
+    "ObjectLockRuleOutputTypeDef",
+    {
+        "DefaultRetention": DefaultRetentionOutputTypeDef,
+    },
+)
+
 ObjectLockRuleTypeDef = TypedDict(
     "ObjectLockRuleTypeDef",
     {
         "DefaultRetention": DefaultRetentionTypeDef,
     },
+    total=False,
 )
 
-DeleteObjectsOutputTypeDef = TypedDict(
-    "DeleteObjectsOutputTypeDef",
+DeleteMarkerEntryOutputTypeDef = TypedDict(
+    "DeleteMarkerEntryOutputTypeDef",
     {
-        "Deleted": List[DeletedObjectTypeDef],
+        "Owner": OwnerOutputTypeDef,
+        "Key": str,
+        "VersionId": str,
+        "IsLatest": bool,
+        "LastModified": datetime,
+    },
+)
+
+ListBucketsOutputOutputTypeDef = TypedDict(
+    "ListBucketsOutputOutputTypeDef",
+    {
+        "Buckets": List[BucketOutputTypeDef],
+        "Owner": OwnerOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DeleteObjectsOutputOutputTypeDef = TypedDict(
+    "DeleteObjectsOutputOutputTypeDef",
+    {
+        "Deleted": List[DeletedObjectOutputTypeDef],
         "RequestCharged": Literal["requester"],
-        "Errors": List[ErrorTypeDef],
+        "Errors": List[ErrorOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDeleteTypeDef = TypedDict(
     "_RequiredDeleteTypeDef",
     {
@@ -4558,161 +5077,105 @@
 )
 
 
 class DeleteTypeDef(_RequiredDeleteTypeDef, _OptionalDeleteTypeDef):
     pass
 
 
+S3KeyFilterOutputTypeDef = TypedDict(
+    "S3KeyFilterOutputTypeDef",
+    {
+        "FilterRules": List[FilterRuleOutputTypeDef],
+    },
+)
+
 S3KeyFilterTypeDef = TypedDict(
     "S3KeyFilterTypeDef",
     {
-        "FilterRules": List[FilterRuleTypeDef],
+        "FilterRules": Sequence[FilterRuleTypeDef],
     },
+    total=False,
 )
 
-GetBucketPolicyStatusOutputTypeDef = TypedDict(
-    "GetBucketPolicyStatusOutputTypeDef",
+GetBucketPolicyStatusOutputOutputTypeDef = TypedDict(
+    "GetBucketPolicyStatusOutputOutputTypeDef",
     {
-        "PolicyStatus": PolicyStatusTypeDef,
+        "PolicyStatus": PolicyStatusOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetObjectAttributesPartsTypeDef = TypedDict(
-    "GetObjectAttributesPartsTypeDef",
+GetObjectAttributesPartsOutputTypeDef = TypedDict(
+    "GetObjectAttributesPartsOutputTypeDef",
     {
         "TotalPartsCount": int,
         "PartNumberMarker": int,
         "NextPartNumberMarker": int,
         "MaxParts": int,
         "IsTruncated": bool,
-        "Parts": List[ObjectPartTypeDef],
+        "Parts": List[ObjectPartOutputTypeDef],
     },
 )
 
-GetObjectLegalHoldOutputTypeDef = TypedDict(
-    "GetObjectLegalHoldOutputTypeDef",
+GetObjectLegalHoldOutputOutputTypeDef = TypedDict(
+    "GetObjectLegalHoldOutputOutputTypeDef",
     {
-        "LegalHold": ObjectLockLegalHoldTypeDef,
+        "LegalHold": ObjectLockLegalHoldOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredPutObjectLegalHoldRequestRequestTypeDef = TypedDict(
-    "_RequiredPutObjectLegalHoldRequestRequestTypeDef",
-    {
-        "Bucket": str,
-        "Key": str,
-    },
-)
-_OptionalPutObjectLegalHoldRequestRequestTypeDef = TypedDict(
-    "_OptionalPutObjectLegalHoldRequestRequestTypeDef",
-    {
-        "LegalHold": ObjectLockLegalHoldTypeDef,
-        "RequestPayer": Literal["requester"],
-        "VersionId": str,
-        "ContentMD5": str,
-        "ChecksumAlgorithm": ChecksumAlgorithmType,
-        "ExpectedBucketOwner": str,
-    },
-    total=False,
-)
-
-
-class PutObjectLegalHoldRequestRequestTypeDef(
-    _RequiredPutObjectLegalHoldRequestRequestTypeDef,
-    _OptionalPutObjectLegalHoldRequestRequestTypeDef,
-):
-    pass
-
-
-GetObjectRetentionOutputTypeDef = TypedDict(
-    "GetObjectRetentionOutputTypeDef",
+GetObjectRetentionOutputOutputTypeDef = TypedDict(
+    "GetObjectRetentionOutputOutputTypeDef",
     {
-        "Retention": ObjectLockRetentionTypeDef,
+        "Retention": ObjectLockRetentionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredPutObjectRetentionRequestRequestTypeDef = TypedDict(
-    "_RequiredPutObjectRetentionRequestRequestTypeDef",
-    {
-        "Bucket": str,
-        "Key": str,
-    },
-)
-_OptionalPutObjectRetentionRequestRequestTypeDef = TypedDict(
-    "_OptionalPutObjectRetentionRequestRequestTypeDef",
+GetPublicAccessBlockOutputOutputTypeDef = TypedDict(
+    "GetPublicAccessBlockOutputOutputTypeDef",
     {
-        "Retention": ObjectLockRetentionTypeDef,
-        "RequestPayer": Literal["requester"],
-        "VersionId": str,
-        "BypassGovernanceRetention": bool,
-        "ContentMD5": str,
-        "ChecksumAlgorithm": ChecksumAlgorithmType,
-        "ExpectedBucketOwner": str,
-    },
-    total=False,
-)
-
-
-class PutObjectRetentionRequestRequestTypeDef(
-    _RequiredPutObjectRetentionRequestRequestTypeDef,
-    _OptionalPutObjectRetentionRequestRequestTypeDef,
-):
-    pass
-
-
-GetPublicAccessBlockOutputTypeDef = TypedDict(
-    "GetPublicAccessBlockOutputTypeDef",
-    {
-        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
+        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredPutPublicAccessBlockRequestRequestTypeDef = TypedDict(
-    "_RequiredPutPublicAccessBlockRequestRequestTypeDef",
+GrantOutputTypeDef = TypedDict(
+    "GrantOutputTypeDef",
     {
-        "Bucket": str,
-        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
+        "Grantee": GranteeOutputTypeDef,
+        "Permission": PermissionType,
     },
 )
-_OptionalPutPublicAccessBlockRequestRequestTypeDef = TypedDict(
-    "_OptionalPutPublicAccessBlockRequestRequestTypeDef",
+
+TargetGrantOutputTypeDef = TypedDict(
+    "TargetGrantOutputTypeDef",
     {
-        "ContentMD5": str,
-        "ChecksumAlgorithm": ChecksumAlgorithmType,
-        "ExpectedBucketOwner": str,
+        "Grantee": GranteeOutputTypeDef,
+        "Permission": BucketLogsPermissionType,
     },
-    total=False,
 )
 
-
-class PutPublicAccessBlockRequestRequestTypeDef(
-    _RequiredPutPublicAccessBlockRequestRequestTypeDef,
-    _OptionalPutPublicAccessBlockRequestRequestTypeDef,
-):
-    pass
-
-
 GrantTypeDef = TypedDict(
     "GrantTypeDef",
     {
         "Grantee": GranteeTypeDef,
         "Permission": PermissionType,
     },
+    total=False,
 )
 
 TargetGrantTypeDef = TypedDict(
     "TargetGrantTypeDef",
     {
         "Grantee": GranteeTypeDef,
         "Permission": BucketLogsPermissionType,
     },
+    total=False,
 )
 
 _RequiredHeadBucketRequestBucketExistsWaitTypeDef = TypedDict(
     "_RequiredHeadBucketRequestBucketExistsWaitTypeDef",
     {
         "Bucket": str,
     },
@@ -4825,23 +5288,23 @@
 class HeadObjectRequestObjectNotExistsWaitTypeDef(
     _RequiredHeadObjectRequestObjectNotExistsWaitTypeDef,
     _OptionalHeadObjectRequestObjectNotExistsWaitTypeDef,
 ):
     pass
 
 
-MultipartUploadTypeDef = TypedDict(
-    "MultipartUploadTypeDef",
+MultipartUploadOutputTypeDef = TypedDict(
+    "MultipartUploadOutputTypeDef",
     {
         "UploadId": str,
         "Key": str,
         "Initiated": datetime,
         "StorageClass": StorageClassType,
-        "Owner": OwnerTypeDef,
-        "Initiator": InitiatorTypeDef,
+        "Owner": OwnerOutputTypeDef,
+        "Initiator": InitiatorOutputTypeDef,
         "ChecksumAlgorithm": ChecksumAlgorithmType,
     },
 )
 
 InputSerializationTypeDef = TypedDict(
     "InputSerializationTypeDef",
     {
@@ -4849,147 +5312,297 @@
         "CompressionType": CompressionTypeType,
         "JSON": JSONInputTypeDef,
         "Parquet": Mapping[str, Any],
     },
     total=False,
 )
 
+InventoryEncryptionOutputTypeDef = TypedDict(
+    "InventoryEncryptionOutputTypeDef",
+    {
+        "SSES3": Dict[str, Any],
+        "SSEKMS": SSEKMSOutputTypeDef,
+    },
+)
+
 InventoryEncryptionTypeDef = TypedDict(
     "InventoryEncryptionTypeDef",
     {
-        "SSES3": Dict[str, Any],
+        "SSES3": Mapping[str, Any],
         "SSEKMS": SSEKMSTypeDef,
     },
+    total=False,
 )
 
 OutputSerializationTypeDef = TypedDict(
     "OutputSerializationTypeDef",
     {
         "CSV": CSVOutputTypeDef,
         "JSON": JSONOutputTypeDef,
     },
     total=False,
 )
 
-RuleTypeDef = TypedDict(
-    "RuleTypeDef",
+RuleOutputTypeDef = TypedDict(
+    "RuleOutputTypeDef",
     {
-        "Expiration": LifecycleExpirationTypeDef,
+        "Expiration": LifecycleExpirationOutputTypeDef,
         "ID": str,
         "Prefix": str,
         "Status": ExpirationStatusType,
+        "Transition": TransitionOutputTypeDef,
+        "NoncurrentVersionTransition": NoncurrentVersionTransitionOutputTypeDef,
+        "NoncurrentVersionExpiration": NoncurrentVersionExpirationOutputTypeDef,
+        "AbortIncompleteMultipartUpload": AbortIncompleteMultipartUploadOutputTypeDef,
+    },
+)
+
+_RequiredRuleTypeDef = TypedDict(
+    "_RequiredRuleTypeDef",
+    {
+        "Prefix": str,
+        "Status": ExpirationStatusType,
+    },
+)
+_OptionalRuleTypeDef = TypedDict(
+    "_OptionalRuleTypeDef",
+    {
+        "Expiration": LifecycleExpirationTypeDef,
+        "ID": str,
         "Transition": TransitionTypeDef,
         "NoncurrentVersionTransition": NoncurrentVersionTransitionTypeDef,
         "NoncurrentVersionExpiration": NoncurrentVersionExpirationTypeDef,
         "AbortIncompleteMultipartUpload": AbortIncompleteMultipartUploadTypeDef,
     },
+    total=False,
 )
 
-ListPartsOutputTypeDef = TypedDict(
-    "ListPartsOutputTypeDef",
+
+class RuleTypeDef(_RequiredRuleTypeDef, _OptionalRuleTypeDef):
+    pass
+
+
+ListPartsOutputOutputTypeDef = TypedDict(
+    "ListPartsOutputOutputTypeDef",
     {
         "AbortDate": datetime,
         "AbortRuleId": str,
         "Bucket": str,
         "Key": str,
         "UploadId": str,
         "PartNumberMarker": int,
         "NextPartNumberMarker": int,
         "MaxParts": int,
         "IsTruncated": bool,
-        "Parts": List[PartTypeDef],
-        "Initiator": InitiatorTypeDef,
-        "Owner": OwnerTypeDef,
+        "Parts": List[PartOutputTypeDef],
+        "Initiator": InitiatorOutputTypeDef,
+        "Owner": OwnerOutputTypeDef,
         "StorageClass": StorageClassType,
         "RequestCharged": Literal["requester"],
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-MetricsTypeDef = TypedDict(
-    "MetricsTypeDef",
+MetricsOutputTypeDef = TypedDict(
+    "MetricsOutputTypeDef",
+    {
+        "Status": MetricsStatusType,
+        "EventThreshold": ReplicationTimeValueOutputTypeDef,
+    },
+)
+
+ReplicationTimeOutputTypeDef = TypedDict(
+    "ReplicationTimeOutputTypeDef",
+    {
+        "Status": ReplicationTimeStatusType,
+        "Time": ReplicationTimeValueOutputTypeDef,
+    },
+)
+
+_RequiredMetricsTypeDef = TypedDict(
+    "_RequiredMetricsTypeDef",
     {
         "Status": MetricsStatusType,
+    },
+)
+_OptionalMetricsTypeDef = TypedDict(
+    "_OptionalMetricsTypeDef",
+    {
         "EventThreshold": ReplicationTimeValueTypeDef,
     },
+    total=False,
 )
 
+
+class MetricsTypeDef(_RequiredMetricsTypeDef, _OptionalMetricsTypeDef):
+    pass
+
+
 ReplicationTimeTypeDef = TypedDict(
     "ReplicationTimeTypeDef",
     {
         "Status": ReplicationTimeStatusType,
         "Time": ReplicationTimeValueTypeDef,
     },
 )
 
-NotificationConfigurationDeprecatedResponseMetadataTypeDef = TypedDict(
-    "NotificationConfigurationDeprecatedResponseMetadataTypeDef",
+NotificationConfigurationDeprecatedOutputTypeDef = TypedDict(
+    "NotificationConfigurationDeprecatedOutputTypeDef",
     {
-        "TopicConfiguration": TopicConfigurationDeprecatedTypeDef,
-        "QueueConfiguration": QueueConfigurationDeprecatedTypeDef,
-        "CloudFunctionConfiguration": CloudFunctionConfigurationTypeDef,
+        "TopicConfiguration": TopicConfigurationDeprecatedOutputTypeDef,
+        "QueueConfiguration": QueueConfigurationDeprecatedOutputTypeDef,
+        "CloudFunctionConfiguration": CloudFunctionConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 NotificationConfigurationDeprecatedTypeDef = TypedDict(
     "NotificationConfigurationDeprecatedTypeDef",
     {
         "TopicConfiguration": TopicConfigurationDeprecatedTypeDef,
         "QueueConfiguration": QueueConfigurationDeprecatedTypeDef,
         "CloudFunctionConfiguration": CloudFunctionConfigurationTypeDef,
     },
     total=False,
 )
 
-ObjectTypeDef = TypedDict(
-    "ObjectTypeDef",
+_RequiredPutObjectLegalHoldRequestRequestTypeDef = TypedDict(
+    "_RequiredPutObjectLegalHoldRequestRequestTypeDef",
+    {
+        "Bucket": str,
+        "Key": str,
+    },
+)
+_OptionalPutObjectLegalHoldRequestRequestTypeDef = TypedDict(
+    "_OptionalPutObjectLegalHoldRequestRequestTypeDef",
+    {
+        "LegalHold": ObjectLockLegalHoldTypeDef,
+        "RequestPayer": Literal["requester"],
+        "VersionId": str,
+        "ContentMD5": str,
+        "ChecksumAlgorithm": ChecksumAlgorithmType,
+        "ExpectedBucketOwner": str,
+    },
+    total=False,
+)
+
+
+class PutObjectLegalHoldRequestRequestTypeDef(
+    _RequiredPutObjectLegalHoldRequestRequestTypeDef,
+    _OptionalPutObjectLegalHoldRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredPutObjectRetentionRequestRequestTypeDef = TypedDict(
+    "_RequiredPutObjectRetentionRequestRequestTypeDef",
+    {
+        "Bucket": str,
+        "Key": str,
+    },
+)
+_OptionalPutObjectRetentionRequestRequestTypeDef = TypedDict(
+    "_OptionalPutObjectRetentionRequestRequestTypeDef",
+    {
+        "Retention": ObjectLockRetentionTypeDef,
+        "RequestPayer": Literal["requester"],
+        "VersionId": str,
+        "BypassGovernanceRetention": bool,
+        "ContentMD5": str,
+        "ChecksumAlgorithm": ChecksumAlgorithmType,
+        "ExpectedBucketOwner": str,
+    },
+    total=False,
+)
+
+
+class PutObjectRetentionRequestRequestTypeDef(
+    _RequiredPutObjectRetentionRequestRequestTypeDef,
+    _OptionalPutObjectRetentionRequestRequestTypeDef,
+):
+    pass
+
+
+ObjectOutputTypeDef = TypedDict(
+    "ObjectOutputTypeDef",
     {
         "Key": str,
         "LastModified": datetime,
         "ETag": str,
         "ChecksumAlgorithm": List[ChecksumAlgorithmType],
         "Size": int,
         "StorageClass": ObjectStorageClassType,
-        "Owner": OwnerTypeDef,
-        "RestoreStatus": RestoreStatusTypeDef,
+        "Owner": OwnerOutputTypeDef,
+        "RestoreStatus": RestoreStatusOutputTypeDef,
     },
 )
 
-ObjectVersionTypeDef = TypedDict(
-    "ObjectVersionTypeDef",
+ObjectVersionOutputTypeDef = TypedDict(
+    "ObjectVersionOutputTypeDef",
     {
         "ETag": str,
         "ChecksumAlgorithm": List[ChecksumAlgorithmType],
         "Size": int,
         "StorageClass": Literal["STANDARD"],
         "Key": str,
         "VersionId": str,
         "IsLatest": bool,
         "LastModified": datetime,
-        "Owner": OwnerTypeDef,
-        "RestoreStatus": RestoreStatusTypeDef,
+        "Owner": OwnerOutputTypeDef,
+        "RestoreStatus": RestoreStatusOutputTypeDef,
+    },
+)
+
+OwnershipControlsOutputTypeDef = TypedDict(
+    "OwnershipControlsOutputTypeDef",
+    {
+        "Rules": List[OwnershipControlsRuleOutputTypeDef],
     },
 )
 
 OwnershipControlsTypeDef = TypedDict(
     "OwnershipControlsTypeDef",
     {
-        "Rules": List[OwnershipControlsRuleTypeDef],
+        "Rules": Sequence[OwnershipControlsRuleTypeDef],
     },
 )
 
-ProgressEventTypeDef = TypedDict(
-    "ProgressEventTypeDef",
+ProgressEventOutputTypeDef = TypedDict(
+    "ProgressEventOutputTypeDef",
     {
-        "Details": ProgressTypeDef,
+        "Details": ProgressOutputTypeDef,
     },
 )
 
+_RequiredPutPublicAccessBlockRequestRequestTypeDef = TypedDict(
+    "_RequiredPutPublicAccessBlockRequestRequestTypeDef",
+    {
+        "Bucket": str,
+        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
+    },
+)
+_OptionalPutPublicAccessBlockRequestRequestTypeDef = TypedDict(
+    "_OptionalPutPublicAccessBlockRequestRequestTypeDef",
+    {
+        "ContentMD5": str,
+        "ChecksumAlgorithm": ChecksumAlgorithmType,
+        "ExpectedBucketOwner": str,
+    },
+    total=False,
+)
+
+
+class PutPublicAccessBlockRequestRequestTypeDef(
+    _RequiredPutPublicAccessBlockRequestRequestTypeDef,
+    _OptionalPutPublicAccessBlockRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredPutBucketRequestPaymentRequestBucketRequestPaymentPutTypeDef = TypedDict(
     "_RequiredPutBucketRequestPaymentRequestBucketRequestPaymentPutTypeDef",
     {
         "RequestPaymentConfiguration": RequestPaymentConfigurationTypeDef,
     },
 )
 _OptionalPutBucketRequestPaymentRequestBucketRequestPaymentPutTypeDef = TypedDict(
@@ -5078,91 +5691,181 @@
 class PutBucketVersioningRequestRequestTypeDef(
     _RequiredPutBucketVersioningRequestRequestTypeDef,
     _OptionalPutBucketVersioningRequestRequestTypeDef,
 ):
     pass
 
 
-RoutingRuleTypeDef = TypedDict(
-    "RoutingRuleTypeDef",
+RoutingRuleOutputTypeDef = TypedDict(
+    "RoutingRuleOutputTypeDef",
+    {
+        "Condition": ConditionOutputTypeDef,
+        "Redirect": RedirectOutputTypeDef,
+    },
+)
+
+_RequiredRoutingRuleTypeDef = TypedDict(
+    "_RequiredRoutingRuleTypeDef",
     {
-        "Condition": ConditionTypeDef,
         "Redirect": RedirectTypeDef,
     },
 )
+_OptionalRoutingRuleTypeDef = TypedDict(
+    "_OptionalRoutingRuleTypeDef",
+    {
+        "Condition": ConditionTypeDef,
+    },
+    total=False,
+)
+
+
+class RoutingRuleTypeDef(_RequiredRoutingRuleTypeDef, _OptionalRoutingRuleTypeDef):
+    pass
+
+
+ServerSideEncryptionRuleOutputTypeDef = TypedDict(
+    "ServerSideEncryptionRuleOutputTypeDef",
+    {
+        "ApplyServerSideEncryptionByDefault": ServerSideEncryptionByDefaultOutputTypeDef,
+        "BucketKeyEnabled": bool,
+    },
+)
 
 ServerSideEncryptionRuleTypeDef = TypedDict(
     "ServerSideEncryptionRuleTypeDef",
     {
         "ApplyServerSideEncryptionByDefault": ServerSideEncryptionByDefaultTypeDef,
         "BucketKeyEnabled": bool,
     },
+    total=False,
+)
+
+SourceSelectionCriteriaOutputTypeDef = TypedDict(
+    "SourceSelectionCriteriaOutputTypeDef",
+    {
+        "SseKmsEncryptedObjects": SseKmsEncryptedObjectsOutputTypeDef,
+        "ReplicaModifications": ReplicaModificationsOutputTypeDef,
+    },
 )
 
 SourceSelectionCriteriaTypeDef = TypedDict(
     "SourceSelectionCriteriaTypeDef",
     {
         "SseKmsEncryptedObjects": SseKmsEncryptedObjectsTypeDef,
         "ReplicaModifications": ReplicaModificationsTypeDef,
     },
+    total=False,
+)
+
+StatsEventOutputTypeDef = TypedDict(
+    "StatsEventOutputTypeDef",
+    {
+        "Details": StatsOutputTypeDef,
+    },
+)
+
+AnalyticsFilterOutputTypeDef = TypedDict(
+    "AnalyticsFilterOutputTypeDef",
+    {
+        "Prefix": str,
+        "Tag": TagOutputTypeDef,
+        "And": AnalyticsAndOperatorOutputTypeDef,
+    },
 )
 
-StatsEventTypeDef = TypedDict(
-    "StatsEventTypeDef",
+IntelligentTieringFilterOutputTypeDef = TypedDict(
+    "IntelligentTieringFilterOutputTypeDef",
     {
-        "Details": StatsTypeDef,
+        "Prefix": str,
+        "Tag": TagOutputTypeDef,
+        "And": IntelligentTieringAndOperatorOutputTypeDef,
+    },
+)
+
+LifecycleRuleFilterOutputTypeDef = TypedDict(
+    "LifecycleRuleFilterOutputTypeDef",
+    {
+        "Prefix": str,
+        "Tag": TagOutputTypeDef,
+        "ObjectSizeGreaterThan": int,
+        "ObjectSizeLessThan": int,
+        "And": LifecycleRuleAndOperatorOutputTypeDef,
+    },
+)
+
+MetricsFilterOutputTypeDef = TypedDict(
+    "MetricsFilterOutputTypeDef",
+    {
+        "Prefix": str,
+        "Tag": TagOutputTypeDef,
+        "AccessPointArn": str,
+        "And": MetricsAndOperatorOutputTypeDef,
+    },
+)
+
+ReplicationRuleFilterOutputTypeDef = TypedDict(
+    "ReplicationRuleFilterOutputTypeDef",
+    {
+        "Prefix": str,
+        "Tag": TagOutputTypeDef,
+        "And": ReplicationRuleAndOperatorOutputTypeDef,
     },
 )
 
 AnalyticsFilterTypeDef = TypedDict(
     "AnalyticsFilterTypeDef",
     {
         "Prefix": str,
         "Tag": TagTypeDef,
         "And": AnalyticsAndOperatorTypeDef,
     },
+    total=False,
 )
 
 IntelligentTieringFilterTypeDef = TypedDict(
     "IntelligentTieringFilterTypeDef",
     {
         "Prefix": str,
         "Tag": TagTypeDef,
         "And": IntelligentTieringAndOperatorTypeDef,
     },
+    total=False,
 )
 
 LifecycleRuleFilterTypeDef = TypedDict(
     "LifecycleRuleFilterTypeDef",
     {
         "Prefix": str,
         "Tag": TagTypeDef,
         "ObjectSizeGreaterThan": int,
         "ObjectSizeLessThan": int,
         "And": LifecycleRuleAndOperatorTypeDef,
     },
+    total=False,
 )
 
 MetricsFilterTypeDef = TypedDict(
     "MetricsFilterTypeDef",
     {
         "Prefix": str,
         "Tag": TagTypeDef,
         "AccessPointArn": str,
         "And": MetricsAndOperatorTypeDef,
     },
+    total=False,
 )
 
 ReplicationRuleFilterTypeDef = TypedDict(
     "ReplicationRuleFilterTypeDef",
     {
         "Prefix": str,
         "Tag": TagTypeDef,
         "And": ReplicationRuleAndOperatorTypeDef,
     },
+    total=False,
 )
 
 _RequiredPutBucketTaggingRequestBucketTaggingPutTypeDef = TypedDict(
     "_RequiredPutBucketTaggingRequestBucketTaggingPutTypeDef",
     {
         "Tagging": TaggingTypeDef,
     },
@@ -5230,14 +5933,22 @@
 
 class PutObjectTaggingRequestRequestTypeDef(
     _RequiredPutObjectTaggingRequestRequestTypeDef, _OptionalPutObjectTaggingRequestRequestTypeDef
 ):
     pass
 
 
+StorageClassAnalysisDataExportOutputTypeDef = TypedDict(
+    "StorageClassAnalysisDataExportOutputTypeDef",
+    {
+        "OutputSchemaVersion": Literal["V_1"],
+        "Destination": AnalyticsExportDestinationOutputTypeDef,
+    },
+)
+
 StorageClassAnalysisDataExportTypeDef = TypedDict(
     "StorageClassAnalysisDataExportTypeDef",
     {
         "OutputSchemaVersion": Literal["V_1"],
         "Destination": AnalyticsExportDestinationTypeDef,
     },
 )
@@ -5334,20 +6045,29 @@
 class CompleteMultipartUploadRequestRequestTypeDef(
     _RequiredCompleteMultipartUploadRequestRequestTypeDef,
     _OptionalCompleteMultipartUploadRequestRequestTypeDef,
 ):
     pass
 
 
+ObjectLockConfigurationOutputTypeDef = TypedDict(
+    "ObjectLockConfigurationOutputTypeDef",
+    {
+        "ObjectLockEnabled": Literal["Enabled"],
+        "Rule": ObjectLockRuleOutputTypeDef,
+    },
+)
+
 ObjectLockConfigurationTypeDef = TypedDict(
     "ObjectLockConfigurationTypeDef",
     {
         "ObjectLockEnabled": Literal["Enabled"],
         "Rule": ObjectLockRuleTypeDef,
     },
+    total=False,
 )
 
 _RequiredDeleteObjectsRequestBucketDeleteObjectsTypeDef = TypedDict(
     "_RequiredDeleteObjectsRequestBucketDeleteObjectsTypeDef",
     {
         "Delete": DeleteTypeDef,
     },
@@ -5394,65 +6114,92 @@
 
 class DeleteObjectsRequestRequestTypeDef(
     _RequiredDeleteObjectsRequestRequestTypeDef, _OptionalDeleteObjectsRequestRequestTypeDef
 ):
     pass
 
 
+NotificationConfigurationFilterOutputTypeDef = TypedDict(
+    "NotificationConfigurationFilterOutputTypeDef",
+    {
+        "Key": S3KeyFilterOutputTypeDef,
+    },
+)
+
 NotificationConfigurationFilterTypeDef = TypedDict(
     "NotificationConfigurationFilterTypeDef",
     {
         "Key": S3KeyFilterTypeDef,
     },
+    total=False,
 )
 
-GetObjectAttributesOutputTypeDef = TypedDict(
-    "GetObjectAttributesOutputTypeDef",
+GetObjectAttributesOutputOutputTypeDef = TypedDict(
+    "GetObjectAttributesOutputOutputTypeDef",
     {
         "DeleteMarker": bool,
         "LastModified": datetime,
         "VersionId": str,
         "RequestCharged": Literal["requester"],
         "ETag": str,
-        "Checksum": ChecksumTypeDef,
-        "ObjectParts": GetObjectAttributesPartsTypeDef,
+        "Checksum": ChecksumOutputTypeDef,
+        "ObjectParts": GetObjectAttributesPartsOutputTypeDef,
         "StorageClass": StorageClassType,
         "ObjectSize": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-AccessControlPolicyTypeDef = TypedDict(
-    "AccessControlPolicyTypeDef",
+GetBucketAclOutputOutputTypeDef = TypedDict(
+    "GetBucketAclOutputOutputTypeDef",
     {
-        "Grants": Sequence[GrantTypeDef],
-        "Owner": OwnerTypeDef,
+        "Owner": OwnerOutputTypeDef,
+        "Grants": List[GrantOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-GetBucketAclOutputTypeDef = TypedDict(
-    "GetBucketAclOutputTypeDef",
+GetObjectAclOutputOutputTypeDef = TypedDict(
+    "GetObjectAclOutputOutputTypeDef",
     {
-        "Owner": OwnerTypeDef,
-        "Grants": List[GrantTypeDef],
+        "Owner": OwnerOutputTypeDef,
+        "Grants": List[GrantOutputTypeDef],
+        "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetObjectAclOutputTypeDef = TypedDict(
-    "GetObjectAclOutputTypeDef",
+LoggingEnabledOutputTypeDef = TypedDict(
+    "LoggingEnabledOutputTypeDef",
     {
-        "Owner": OwnerTypeDef,
-        "Grants": List[GrantTypeDef],
-        "RequestCharged": Literal["requester"],
+        "TargetBucket": str,
+        "TargetGrants": List[TargetGrantOutputTypeDef],
+        "TargetPrefix": str,
+    },
+)
+
+LoggingEnabledResponseMetadataTypeDef = TypedDict(
+    "LoggingEnabledResponseMetadataTypeDef",
+    {
+        "TargetBucket": str,
+        "TargetGrants": List[TargetGrantOutputTypeDef],
+        "TargetPrefix": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+AccessControlPolicyTypeDef = TypedDict(
+    "AccessControlPolicyTypeDef",
+    {
+        "Grants": Sequence[GrantTypeDef],
+        "Owner": OwnerTypeDef,
+    },
+    total=False,
+)
+
 _RequiredS3LocationTypeDef = TypedDict(
     "_RequiredS3LocationTypeDef",
     {
         "BucketName": str,
         "Prefix": str,
     },
 )
@@ -5470,64 +6217,89 @@
 )
 
 
 class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
     pass
 
 
-LoggingEnabledResponseMetadataTypeDef = TypedDict(
-    "LoggingEnabledResponseMetadataTypeDef",
+_RequiredLoggingEnabledTypeDef = TypedDict(
+    "_RequiredLoggingEnabledTypeDef",
     {
         "TargetBucket": str,
-        "TargetGrants": List[TargetGrantTypeDef],
         "TargetPrefix": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-
-LoggingEnabledTypeDef = TypedDict(
-    "LoggingEnabledTypeDef",
+_OptionalLoggingEnabledTypeDef = TypedDict(
+    "_OptionalLoggingEnabledTypeDef",
     {
-        "TargetBucket": str,
-        "TargetGrants": List[TargetGrantTypeDef],
-        "TargetPrefix": str,
+        "TargetGrants": Sequence[TargetGrantTypeDef],
     },
+    total=False,
 )
 
-ListMultipartUploadsOutputTypeDef = TypedDict(
-    "ListMultipartUploadsOutputTypeDef",
+
+class LoggingEnabledTypeDef(_RequiredLoggingEnabledTypeDef, _OptionalLoggingEnabledTypeDef):
+    pass
+
+
+ListMultipartUploadsOutputOutputTypeDef = TypedDict(
+    "ListMultipartUploadsOutputOutputTypeDef",
     {
         "Bucket": str,
         "KeyMarker": str,
         "UploadIdMarker": str,
         "NextKeyMarker": str,
         "Prefix": str,
         "Delimiter": str,
         "NextUploadIdMarker": str,
         "MaxUploads": int,
         "IsTruncated": bool,
-        "Uploads": List[MultipartUploadTypeDef],
-        "CommonPrefixes": List[CommonPrefixTypeDef],
+        "Uploads": List[MultipartUploadOutputTypeDef],
+        "CommonPrefixes": List[CommonPrefixOutputTypeDef],
         "EncodingType": Literal["url"],
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-InventoryS3BucketDestinationTypeDef = TypedDict(
-    "InventoryS3BucketDestinationTypeDef",
+InventoryS3BucketDestinationOutputTypeDef = TypedDict(
+    "InventoryS3BucketDestinationOutputTypeDef",
     {
         "AccountId": str,
         "Bucket": str,
         "Format": InventoryFormatType,
         "Prefix": str,
+        "Encryption": InventoryEncryptionOutputTypeDef,
+    },
+)
+
+_RequiredInventoryS3BucketDestinationTypeDef = TypedDict(
+    "_RequiredInventoryS3BucketDestinationTypeDef",
+    {
+        "Bucket": str,
+        "Format": InventoryFormatType,
+    },
+)
+_OptionalInventoryS3BucketDestinationTypeDef = TypedDict(
+    "_OptionalInventoryS3BucketDestinationTypeDef",
+    {
+        "AccountId": str,
+        "Prefix": str,
         "Encryption": InventoryEncryptionTypeDef,
     },
+    total=False,
 )
 
+
+class InventoryS3BucketDestinationTypeDef(
+    _RequiredInventoryS3BucketDestinationTypeDef, _OptionalInventoryS3BucketDestinationTypeDef
+):
+    pass
+
+
 _RequiredSelectObjectContentRequestRequestTypeDef = TypedDict(
     "_RequiredSelectObjectContentRequestRequestTypeDef",
     {
         "Bucket": str,
         "Key": str,
         "Expression": str,
         "ExpressionType": Literal["SQL"],
@@ -5562,42 +6334,66 @@
         "InputSerialization": InputSerializationTypeDef,
         "ExpressionType": Literal["SQL"],
         "Expression": str,
         "OutputSerialization": OutputSerializationTypeDef,
     },
 )
 
-GetBucketLifecycleOutputTypeDef = TypedDict(
-    "GetBucketLifecycleOutputTypeDef",
+GetBucketLifecycleOutputOutputTypeDef = TypedDict(
+    "GetBucketLifecycleOutputOutputTypeDef",
     {
-        "Rules": List[RuleTypeDef],
+        "Rules": List[RuleOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LifecycleConfigurationTypeDef = TypedDict(
     "LifecycleConfigurationTypeDef",
     {
         "Rules": Sequence[RuleTypeDef],
     },
 )
 
-DestinationTypeDef = TypedDict(
-    "DestinationTypeDef",
+DestinationOutputTypeDef = TypedDict(
+    "DestinationOutputTypeDef",
+    {
+        "Bucket": str,
+        "Account": str,
+        "StorageClass": StorageClassType,
+        "AccessControlTranslation": AccessControlTranslationOutputTypeDef,
+        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
+        "ReplicationTime": ReplicationTimeOutputTypeDef,
+        "Metrics": MetricsOutputTypeDef,
+    },
+)
+
+_RequiredDestinationTypeDef = TypedDict(
+    "_RequiredDestinationTypeDef",
     {
         "Bucket": str,
+    },
+)
+_OptionalDestinationTypeDef = TypedDict(
+    "_OptionalDestinationTypeDef",
+    {
         "Account": str,
         "StorageClass": StorageClassType,
         "AccessControlTranslation": AccessControlTranslationTypeDef,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
         "ReplicationTime": ReplicationTimeTypeDef,
         "Metrics": MetricsTypeDef,
     },
+    total=False,
 )
 
+
+class DestinationTypeDef(_RequiredDestinationTypeDef, _OptionalDestinationTypeDef):
+    pass
+
+
 _RequiredPutBucketNotificationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketNotificationRequestRequestTypeDef",
     {
         "Bucket": str,
         "NotificationConfiguration": NotificationConfigurationDeprecatedTypeDef,
     },
 )
@@ -5614,77 +6410,77 @@
 class PutBucketNotificationRequestRequestTypeDef(
     _RequiredPutBucketNotificationRequestRequestTypeDef,
     _OptionalPutBucketNotificationRequestRequestTypeDef,
 ):
     pass
 
 
-ListObjectsOutputTypeDef = TypedDict(
-    "ListObjectsOutputTypeDef",
+ListObjectsOutputOutputTypeDef = TypedDict(
+    "ListObjectsOutputOutputTypeDef",
     {
         "IsTruncated": bool,
         "Marker": str,
         "NextMarker": str,
-        "Contents": List[ObjectTypeDef],
+        "Contents": List[ObjectOutputTypeDef],
         "Name": str,
         "Prefix": str,
         "Delimiter": str,
         "MaxKeys": int,
-        "CommonPrefixes": List[CommonPrefixTypeDef],
+        "CommonPrefixes": List[CommonPrefixOutputTypeDef],
         "EncodingType": Literal["url"],
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListObjectsV2OutputTypeDef = TypedDict(
-    "ListObjectsV2OutputTypeDef",
+ListObjectsV2OutputOutputTypeDef = TypedDict(
+    "ListObjectsV2OutputOutputTypeDef",
     {
         "IsTruncated": bool,
-        "Contents": List[ObjectTypeDef],
+        "Contents": List[ObjectOutputTypeDef],
         "Name": str,
         "Prefix": str,
         "Delimiter": str,
         "MaxKeys": int,
-        "CommonPrefixes": List[CommonPrefixTypeDef],
+        "CommonPrefixes": List[CommonPrefixOutputTypeDef],
         "EncodingType": Literal["url"],
         "KeyCount": int,
         "ContinuationToken": str,
         "NextContinuationToken": str,
         "StartAfter": str,
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListObjectVersionsOutputTypeDef = TypedDict(
-    "ListObjectVersionsOutputTypeDef",
+ListObjectVersionsOutputOutputTypeDef = TypedDict(
+    "ListObjectVersionsOutputOutputTypeDef",
     {
         "IsTruncated": bool,
         "KeyMarker": str,
         "VersionIdMarker": str,
         "NextKeyMarker": str,
         "NextVersionIdMarker": str,
-        "Versions": List[ObjectVersionTypeDef],
-        "DeleteMarkers": List[DeleteMarkerEntryTypeDef],
+        "Versions": List[ObjectVersionOutputTypeDef],
+        "DeleteMarkers": List[DeleteMarkerEntryOutputTypeDef],
         "Name": str,
         "Prefix": str,
         "Delimiter": str,
         "MaxKeys": int,
-        "CommonPrefixes": List[CommonPrefixTypeDef],
+        "CommonPrefixes": List[CommonPrefixOutputTypeDef],
         "EncodingType": Literal["url"],
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetBucketOwnershipControlsOutputTypeDef = TypedDict(
-    "GetBucketOwnershipControlsOutputTypeDef",
+GetBucketOwnershipControlsOutputOutputTypeDef = TypedDict(
+    "GetBucketOwnershipControlsOutputOutputTypeDef",
     {
-        "OwnershipControls": OwnershipControlsTypeDef,
+        "OwnershipControls": OwnershipControlsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutBucketOwnershipControlsRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketOwnershipControlsRequestRequestTypeDef",
     {
@@ -5705,21 +6501,21 @@
 class PutBucketOwnershipControlsRequestRequestTypeDef(
     _RequiredPutBucketOwnershipControlsRequestRequestTypeDef,
     _OptionalPutBucketOwnershipControlsRequestRequestTypeDef,
 ):
     pass
 
 
-GetBucketWebsiteOutputTypeDef = TypedDict(
-    "GetBucketWebsiteOutputTypeDef",
+GetBucketWebsiteOutputOutputTypeDef = TypedDict(
+    "GetBucketWebsiteOutputOutputTypeDef",
     {
-        "RedirectAllRequestsTo": RedirectAllRequestsToTypeDef,
-        "IndexDocument": IndexDocumentTypeDef,
-        "ErrorDocument": ErrorDocumentTypeDef,
-        "RoutingRules": List[RoutingRuleTypeDef],
+        "RedirectAllRequestsTo": RedirectAllRequestsToOutputTypeDef,
+        "IndexDocument": IndexDocumentOutputTypeDef,
+        "ErrorDocument": ErrorDocumentOutputTypeDef,
+        "RoutingRules": List[RoutingRuleOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 WebsiteConfigurationTypeDef = TypedDict(
     "WebsiteConfigurationTypeDef",
     {
@@ -5727,76 +6523,161 @@
         "IndexDocument": IndexDocumentTypeDef,
         "RedirectAllRequestsTo": RedirectAllRequestsToTypeDef,
         "RoutingRules": Sequence[RoutingRuleTypeDef],
     },
     total=False,
 )
 
+ServerSideEncryptionConfigurationOutputTypeDef = TypedDict(
+    "ServerSideEncryptionConfigurationOutputTypeDef",
+    {
+        "Rules": List[ServerSideEncryptionRuleOutputTypeDef],
+    },
+)
+
 ServerSideEncryptionConfigurationTypeDef = TypedDict(
     "ServerSideEncryptionConfigurationTypeDef",
     {
-        "Rules": List[ServerSideEncryptionRuleTypeDef],
+        "Rules": Sequence[ServerSideEncryptionRuleTypeDef],
     },
 )
 
-SelectObjectContentEventStreamTypeDef = TypedDict(
-    "SelectObjectContentEventStreamTypeDef",
+SelectObjectContentEventStreamOutputTypeDef = TypedDict(
+    "SelectObjectContentEventStreamOutputTypeDef",
     {
-        "Records": RecordsEventTypeDef,
-        "Stats": StatsEventTypeDef,
-        "Progress": ProgressEventTypeDef,
+        "Records": RecordsEventOutputTypeDef,
+        "Stats": StatsEventOutputTypeDef,
+        "Progress": ProgressEventOutputTypeDef,
         "Cont": Dict[str, Any],
         "End": Dict[str, Any],
     },
 )
 
-IntelligentTieringConfigurationTypeDef = TypedDict(
-    "IntelligentTieringConfigurationTypeDef",
+IntelligentTieringConfigurationOutputTypeDef = TypedDict(
+    "IntelligentTieringConfigurationOutputTypeDef",
     {
         "Id": str,
-        "Filter": IntelligentTieringFilterTypeDef,
+        "Filter": IntelligentTieringFilterOutputTypeDef,
         "Status": IntelligentTieringStatusType,
-        "Tierings": List[TieringTypeDef],
+        "Tierings": List[TieringOutputTypeDef],
     },
 )
 
-LifecycleRuleTypeDef = TypedDict(
-    "LifecycleRuleTypeDef",
+LifecycleRuleOutputTypeDef = TypedDict(
+    "LifecycleRuleOutputTypeDef",
+    {
+        "Expiration": LifecycleExpirationOutputTypeDef,
+        "ID": str,
+        "Prefix": str,
+        "Filter": LifecycleRuleFilterOutputTypeDef,
+        "Status": ExpirationStatusType,
+        "Transitions": List[TransitionOutputTypeDef],
+        "NoncurrentVersionTransitions": List[NoncurrentVersionTransitionOutputTypeDef],
+        "NoncurrentVersionExpiration": NoncurrentVersionExpirationOutputTypeDef,
+        "AbortIncompleteMultipartUpload": AbortIncompleteMultipartUploadOutputTypeDef,
+    },
+)
+
+MetricsConfigurationOutputTypeDef = TypedDict(
+    "MetricsConfigurationOutputTypeDef",
+    {
+        "Id": str,
+        "Filter": MetricsFilterOutputTypeDef,
+    },
+)
+
+_RequiredIntelligentTieringConfigurationTypeDef = TypedDict(
+    "_RequiredIntelligentTieringConfigurationTypeDef",
+    {
+        "Id": str,
+        "Status": IntelligentTieringStatusType,
+        "Tierings": Sequence[TieringTypeDef],
+    },
+)
+_OptionalIntelligentTieringConfigurationTypeDef = TypedDict(
+    "_OptionalIntelligentTieringConfigurationTypeDef",
+    {
+        "Filter": IntelligentTieringFilterTypeDef,
+    },
+    total=False,
+)
+
+
+class IntelligentTieringConfigurationTypeDef(
+    _RequiredIntelligentTieringConfigurationTypeDef, _OptionalIntelligentTieringConfigurationTypeDef
+):
+    pass
+
+
+_RequiredLifecycleRuleTypeDef = TypedDict(
+    "_RequiredLifecycleRuleTypeDef",
+    {
+        "Status": ExpirationStatusType,
+    },
+)
+_OptionalLifecycleRuleTypeDef = TypedDict(
+    "_OptionalLifecycleRuleTypeDef",
     {
         "Expiration": LifecycleExpirationTypeDef,
         "ID": str,
         "Prefix": str,
         "Filter": LifecycleRuleFilterTypeDef,
-        "Status": ExpirationStatusType,
-        "Transitions": List[TransitionTypeDef],
-        "NoncurrentVersionTransitions": List[NoncurrentVersionTransitionTypeDef],
+        "Transitions": Sequence[TransitionTypeDef],
+        "NoncurrentVersionTransitions": Sequence[NoncurrentVersionTransitionTypeDef],
         "NoncurrentVersionExpiration": NoncurrentVersionExpirationTypeDef,
         "AbortIncompleteMultipartUpload": AbortIncompleteMultipartUploadTypeDef,
     },
+    total=False,
 )
 
-MetricsConfigurationTypeDef = TypedDict(
-    "MetricsConfigurationTypeDef",
+
+class LifecycleRuleTypeDef(_RequiredLifecycleRuleTypeDef, _OptionalLifecycleRuleTypeDef):
+    pass
+
+
+_RequiredMetricsConfigurationTypeDef = TypedDict(
+    "_RequiredMetricsConfigurationTypeDef",
     {
         "Id": str,
+    },
+)
+_OptionalMetricsConfigurationTypeDef = TypedDict(
+    "_OptionalMetricsConfigurationTypeDef",
+    {
         "Filter": MetricsFilterTypeDef,
     },
+    total=False,
+)
+
+
+class MetricsConfigurationTypeDef(
+    _RequiredMetricsConfigurationTypeDef, _OptionalMetricsConfigurationTypeDef
+):
+    pass
+
+
+StorageClassAnalysisOutputTypeDef = TypedDict(
+    "StorageClassAnalysisOutputTypeDef",
+    {
+        "DataExport": StorageClassAnalysisDataExportOutputTypeDef,
+    },
 )
 
 StorageClassAnalysisTypeDef = TypedDict(
     "StorageClassAnalysisTypeDef",
     {
         "DataExport": StorageClassAnalysisDataExportTypeDef,
     },
+    total=False,
 )
 
-GetObjectLockConfigurationOutputTypeDef = TypedDict(
-    "GetObjectLockConfigurationOutputTypeDef",
+GetObjectLockConfigurationOutputOutputTypeDef = TypedDict(
+    "GetObjectLockConfigurationOutputOutputTypeDef",
     {
-        "ObjectLockConfiguration": ObjectLockConfigurationTypeDef,
+        "ObjectLockConfiguration": ObjectLockConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutObjectLockConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutObjectLockConfigurationRequestRequestTypeDef",
     {
@@ -5820,42 +6701,119 @@
 class PutObjectLockConfigurationRequestRequestTypeDef(
     _RequiredPutObjectLockConfigurationRequestRequestTypeDef,
     _OptionalPutObjectLockConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-LambdaFunctionConfigurationTypeDef = TypedDict(
-    "LambdaFunctionConfigurationTypeDef",
+LambdaFunctionConfigurationOutputTypeDef = TypedDict(
+    "LambdaFunctionConfigurationOutputTypeDef",
     {
         "Id": str,
         "LambdaFunctionArn": str,
         "Events": List[EventType],
-        "Filter": NotificationConfigurationFilterTypeDef,
+        "Filter": NotificationConfigurationFilterOutputTypeDef,
     },
 )
 
-QueueConfigurationTypeDef = TypedDict(
-    "QueueConfigurationTypeDef",
+QueueConfigurationOutputTypeDef = TypedDict(
+    "QueueConfigurationOutputTypeDef",
     {
         "Id": str,
         "QueueArn": str,
         "Events": List[EventType],
-        "Filter": NotificationConfigurationFilterTypeDef,
+        "Filter": NotificationConfigurationFilterOutputTypeDef,
     },
 )
 
-TopicConfigurationTypeDef = TypedDict(
-    "TopicConfigurationTypeDef",
+TopicConfigurationOutputTypeDef = TypedDict(
+    "TopicConfigurationOutputTypeDef",
     {
         "Id": str,
         "TopicArn": str,
         "Events": List[EventType],
+        "Filter": NotificationConfigurationFilterOutputTypeDef,
+    },
+)
+
+_RequiredLambdaFunctionConfigurationTypeDef = TypedDict(
+    "_RequiredLambdaFunctionConfigurationTypeDef",
+    {
+        "LambdaFunctionArn": str,
+        "Events": Sequence[EventType],
+    },
+)
+_OptionalLambdaFunctionConfigurationTypeDef = TypedDict(
+    "_OptionalLambdaFunctionConfigurationTypeDef",
+    {
+        "Id": str,
         "Filter": NotificationConfigurationFilterTypeDef,
     },
+    total=False,
+)
+
+
+class LambdaFunctionConfigurationTypeDef(
+    _RequiredLambdaFunctionConfigurationTypeDef, _OptionalLambdaFunctionConfigurationTypeDef
+):
+    pass
+
+
+_RequiredQueueConfigurationTypeDef = TypedDict(
+    "_RequiredQueueConfigurationTypeDef",
+    {
+        "QueueArn": str,
+        "Events": Sequence[EventType],
+    },
+)
+_OptionalQueueConfigurationTypeDef = TypedDict(
+    "_OptionalQueueConfigurationTypeDef",
+    {
+        "Id": str,
+        "Filter": NotificationConfigurationFilterTypeDef,
+    },
+    total=False,
+)
+
+
+class QueueConfigurationTypeDef(
+    _RequiredQueueConfigurationTypeDef, _OptionalQueueConfigurationTypeDef
+):
+    pass
+
+
+_RequiredTopicConfigurationTypeDef = TypedDict(
+    "_RequiredTopicConfigurationTypeDef",
+    {
+        "TopicArn": str,
+        "Events": Sequence[EventType],
+    },
+)
+_OptionalTopicConfigurationTypeDef = TypedDict(
+    "_OptionalTopicConfigurationTypeDef",
+    {
+        "Id": str,
+        "Filter": NotificationConfigurationFilterTypeDef,
+    },
+    total=False,
+)
+
+
+class TopicConfigurationTypeDef(
+    _RequiredTopicConfigurationTypeDef, _OptionalTopicConfigurationTypeDef
+):
+    pass
+
+
+GetBucketLoggingOutputOutputTypeDef = TypedDict(
+    "GetBucketLoggingOutputOutputTypeDef",
+    {
+        "LoggingEnabled": LoggingEnabledOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
 )
 
 PutBucketAclRequestBucketAclPutTypeDef = TypedDict(
     "PutBucketAclRequestBucketAclPutTypeDef",
     {
         "ACL": BucketCannedACLType,
         "AccessControlPolicy": AccessControlPolicyTypeDef,
@@ -5961,19 +6919,18 @@
     "BucketLoggingStatusTypeDef",
     {
         "LoggingEnabled": LoggingEnabledTypeDef,
     },
     total=False,
 )
 
-GetBucketLoggingOutputTypeDef = TypedDict(
-    "GetBucketLoggingOutputTypeDef",
+InventoryDestinationOutputTypeDef = TypedDict(
+    "InventoryDestinationOutputTypeDef",
     {
-        "LoggingEnabled": LoggingEnabledTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "S3BucketDestination": InventoryS3BucketDestinationOutputTypeDef,
     },
 )
 
 InventoryDestinationTypeDef = TypedDict(
     "InventoryDestinationTypeDef",
     {
         "S3BucketDestination": InventoryS3BucketDestinationTypeDef,
@@ -6010,29 +6967,55 @@
 class PutBucketLifecycleRequestRequestTypeDef(
     _RequiredPutBucketLifecycleRequestRequestTypeDef,
     _OptionalPutBucketLifecycleRequestRequestTypeDef,
 ):
     pass
 
 
-ReplicationRuleTypeDef = TypedDict(
-    "ReplicationRuleTypeDef",
+ReplicationRuleOutputTypeDef = TypedDict(
+    "ReplicationRuleOutputTypeDef",
     {
         "ID": str,
         "Priority": int,
         "Prefix": str,
-        "Filter": ReplicationRuleFilterTypeDef,
+        "Filter": ReplicationRuleFilterOutputTypeDef,
         "Status": ReplicationRuleStatusType,
+        "SourceSelectionCriteria": SourceSelectionCriteriaOutputTypeDef,
+        "ExistingObjectReplication": ExistingObjectReplicationOutputTypeDef,
+        "Destination": DestinationOutputTypeDef,
+        "DeleteMarkerReplication": DeleteMarkerReplicationOutputTypeDef,
+    },
+)
+
+_RequiredReplicationRuleTypeDef = TypedDict(
+    "_RequiredReplicationRuleTypeDef",
+    {
+        "Status": ReplicationRuleStatusType,
+        "Destination": DestinationTypeDef,
+    },
+)
+_OptionalReplicationRuleTypeDef = TypedDict(
+    "_OptionalReplicationRuleTypeDef",
+    {
+        "ID": str,
+        "Priority": int,
+        "Prefix": str,
+        "Filter": ReplicationRuleFilterTypeDef,
         "SourceSelectionCriteria": SourceSelectionCriteriaTypeDef,
         "ExistingObjectReplication": ExistingObjectReplicationTypeDef,
-        "Destination": DestinationTypeDef,
         "DeleteMarkerReplication": DeleteMarkerReplicationTypeDef,
     },
+    total=False,
 )
 
+
+class ReplicationRuleTypeDef(_RequiredReplicationRuleTypeDef, _OptionalReplicationRuleTypeDef):
+    pass
+
+
 _RequiredPutBucketWebsiteRequestBucketWebsitePutTypeDef = TypedDict(
     "_RequiredPutBucketWebsiteRequestBucketWebsitePutTypeDef",
     {
         "WebsiteConfiguration": WebsiteConfigurationTypeDef,
     },
 )
 _OptionalPutBucketWebsiteRequestBucketWebsitePutTypeDef = TypedDict(
@@ -6071,18 +7054,18 @@
 
 class PutBucketWebsiteRequestRequestTypeDef(
     _RequiredPutBucketWebsiteRequestRequestTypeDef, _OptionalPutBucketWebsiteRequestRequestTypeDef
 ):
     pass
 
 
-GetBucketEncryptionOutputTypeDef = TypedDict(
-    "GetBucketEncryptionOutputTypeDef",
+GetBucketEncryptionOutputOutputTypeDef = TypedDict(
+    "GetBucketEncryptionOutputOutputTypeDef",
     {
-        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
+        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutBucketEncryptionRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketEncryptionRequestRequestTypeDef",
     {
@@ -6104,81 +7087,81 @@
 class PutBucketEncryptionRequestRequestTypeDef(
     _RequiredPutBucketEncryptionRequestRequestTypeDef,
     _OptionalPutBucketEncryptionRequestRequestTypeDef,
 ):
     pass
 
 
-SelectObjectContentOutputTypeDef = TypedDict(
-    "SelectObjectContentOutputTypeDef",
+SelectObjectContentOutputOutputTypeDef = TypedDict(
+    "SelectObjectContentOutputOutputTypeDef",
     {
-        "Payload": "EventStream[SelectObjectContentEventStreamTypeDef]",
+        "Payload": "EventStream[SelectObjectContentEventStreamOutputTypeDef]",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetBucketIntelligentTieringConfigurationOutputTypeDef = TypedDict(
-    "GetBucketIntelligentTieringConfigurationOutputTypeDef",
+GetBucketIntelligentTieringConfigurationOutputOutputTypeDef = TypedDict(
+    "GetBucketIntelligentTieringConfigurationOutputOutputTypeDef",
     {
-        "IntelligentTieringConfiguration": IntelligentTieringConfigurationTypeDef,
+        "IntelligentTieringConfiguration": IntelligentTieringConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListBucketIntelligentTieringConfigurationsOutputTypeDef = TypedDict(
-    "ListBucketIntelligentTieringConfigurationsOutputTypeDef",
+ListBucketIntelligentTieringConfigurationsOutputOutputTypeDef = TypedDict(
+    "ListBucketIntelligentTieringConfigurationsOutputOutputTypeDef",
     {
         "IsTruncated": bool,
         "ContinuationToken": str,
         "NextContinuationToken": str,
-        "IntelligentTieringConfigurationList": List[IntelligentTieringConfigurationTypeDef],
+        "IntelligentTieringConfigurationList": List[IntelligentTieringConfigurationOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutBucketIntelligentTieringConfigurationRequestRequestTypeDef = TypedDict(
-    "PutBucketIntelligentTieringConfigurationRequestRequestTypeDef",
+GetBucketLifecycleConfigurationOutputOutputTypeDef = TypedDict(
+    "GetBucketLifecycleConfigurationOutputOutputTypeDef",
     {
-        "Bucket": str,
-        "Id": str,
-        "IntelligentTieringConfiguration": IntelligentTieringConfigurationTypeDef,
+        "Rules": List[LifecycleRuleOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-BucketLifecycleConfigurationTypeDef = TypedDict(
-    "BucketLifecycleConfigurationTypeDef",
+GetBucketMetricsConfigurationOutputOutputTypeDef = TypedDict(
+    "GetBucketMetricsConfigurationOutputOutputTypeDef",
     {
-        "Rules": Sequence[LifecycleRuleTypeDef],
+        "MetricsConfiguration": MetricsConfigurationOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetBucketLifecycleConfigurationOutputTypeDef = TypedDict(
-    "GetBucketLifecycleConfigurationOutputTypeDef",
+ListBucketMetricsConfigurationsOutputOutputTypeDef = TypedDict(
+    "ListBucketMetricsConfigurationsOutputOutputTypeDef",
     {
-        "Rules": List[LifecycleRuleTypeDef],
+        "IsTruncated": bool,
+        "ContinuationToken": str,
+        "NextContinuationToken": str,
+        "MetricsConfigurationList": List[MetricsConfigurationOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetBucketMetricsConfigurationOutputTypeDef = TypedDict(
-    "GetBucketMetricsConfigurationOutputTypeDef",
+PutBucketIntelligentTieringConfigurationRequestRequestTypeDef = TypedDict(
+    "PutBucketIntelligentTieringConfigurationRequestRequestTypeDef",
     {
-        "MetricsConfiguration": MetricsConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Bucket": str,
+        "Id": str,
+        "IntelligentTieringConfiguration": IntelligentTieringConfigurationTypeDef,
     },
 )
 
-ListBucketMetricsConfigurationsOutputTypeDef = TypedDict(
-    "ListBucketMetricsConfigurationsOutputTypeDef",
+BucketLifecycleConfigurationTypeDef = TypedDict(
+    "BucketLifecycleConfigurationTypeDef",
     {
-        "IsTruncated": bool,
-        "ContinuationToken": str,
-        "NextContinuationToken": str,
-        "MetricsConfigurationList": List[MetricsConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Rules": Sequence[LifecycleRuleTypeDef],
     },
 )
 
 _RequiredPutBucketMetricsConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketMetricsConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -6198,29 +7181,51 @@
 class PutBucketMetricsConfigurationRequestRequestTypeDef(
     _RequiredPutBucketMetricsConfigurationRequestRequestTypeDef,
     _OptionalPutBucketMetricsConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-AnalyticsConfigurationTypeDef = TypedDict(
-    "AnalyticsConfigurationTypeDef",
+AnalyticsConfigurationOutputTypeDef = TypedDict(
+    "AnalyticsConfigurationOutputTypeDef",
+    {
+        "Id": str,
+        "Filter": AnalyticsFilterOutputTypeDef,
+        "StorageClassAnalysis": StorageClassAnalysisOutputTypeDef,
+    },
+)
+
+_RequiredAnalyticsConfigurationTypeDef = TypedDict(
+    "_RequiredAnalyticsConfigurationTypeDef",
     {
         "Id": str,
-        "Filter": AnalyticsFilterTypeDef,
         "StorageClassAnalysis": StorageClassAnalysisTypeDef,
     },
 )
+_OptionalAnalyticsConfigurationTypeDef = TypedDict(
+    "_OptionalAnalyticsConfigurationTypeDef",
+    {
+        "Filter": AnalyticsFilterTypeDef,
+    },
+    total=False,
+)
+
+
+class AnalyticsConfigurationTypeDef(
+    _RequiredAnalyticsConfigurationTypeDef, _OptionalAnalyticsConfigurationTypeDef
+):
+    pass
 
-NotificationConfigurationResponseMetadataTypeDef = TypedDict(
-    "NotificationConfigurationResponseMetadataTypeDef",
+
+NotificationConfigurationOutputTypeDef = TypedDict(
+    "NotificationConfigurationOutputTypeDef",
     {
-        "TopicConfigurations": List[TopicConfigurationTypeDef],
-        "QueueConfigurations": List[QueueConfigurationTypeDef],
-        "LambdaFunctionConfigurations": List[LambdaFunctionConfigurationTypeDef],
+        "TopicConfigurations": List[TopicConfigurationOutputTypeDef],
+        "QueueConfigurations": List[QueueConfigurationOutputTypeDef],
+        "LambdaFunctionConfigurations": List[LambdaFunctionConfigurationOutputTypeDef],
         "EventBridgeConfiguration": Dict[str, Any],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 NotificationConfigurationTypeDef = TypedDict(
     "NotificationConfigurationTypeDef",
@@ -6289,32 +7294,66 @@
 
 class PutBucketLoggingRequestRequestTypeDef(
     _RequiredPutBucketLoggingRequestRequestTypeDef, _OptionalPutBucketLoggingRequestRequestTypeDef
 ):
     pass
 
 
-InventoryConfigurationTypeDef = TypedDict(
-    "InventoryConfigurationTypeDef",
+InventoryConfigurationOutputTypeDef = TypedDict(
+    "InventoryConfigurationOutputTypeDef",
     {
-        "Destination": InventoryDestinationTypeDef,
+        "Destination": InventoryDestinationOutputTypeDef,
         "IsEnabled": bool,
-        "Filter": InventoryFilterTypeDef,
+        "Filter": InventoryFilterOutputTypeDef,
         "Id": str,
         "IncludedObjectVersions": InventoryIncludedObjectVersionsType,
         "OptionalFields": List[InventoryOptionalFieldType],
+        "Schedule": InventoryScheduleOutputTypeDef,
+    },
+)
+
+_RequiredInventoryConfigurationTypeDef = TypedDict(
+    "_RequiredInventoryConfigurationTypeDef",
+    {
+        "Destination": InventoryDestinationTypeDef,
+        "IsEnabled": bool,
+        "Id": str,
+        "IncludedObjectVersions": InventoryIncludedObjectVersionsType,
         "Schedule": InventoryScheduleTypeDef,
     },
 )
+_OptionalInventoryConfigurationTypeDef = TypedDict(
+    "_OptionalInventoryConfigurationTypeDef",
+    {
+        "Filter": InventoryFilterTypeDef,
+        "OptionalFields": Sequence[InventoryOptionalFieldType],
+    },
+    total=False,
+)
+
+
+class InventoryConfigurationTypeDef(
+    _RequiredInventoryConfigurationTypeDef, _OptionalInventoryConfigurationTypeDef
+):
+    pass
+
+
+ReplicationConfigurationOutputTypeDef = TypedDict(
+    "ReplicationConfigurationOutputTypeDef",
+    {
+        "Role": str,
+        "Rules": List[ReplicationRuleOutputTypeDef],
+    },
+)
 
 ReplicationConfigurationTypeDef = TypedDict(
     "ReplicationConfigurationTypeDef",
     {
         "Role": str,
-        "Rules": List[ReplicationRuleTypeDef],
+        "Rules": Sequence[ReplicationRuleTypeDef],
     },
 )
 
 PutBucketLifecycleConfigurationRequestBucketLifecycleConfigurationPutTypeDef = TypedDict(
     "PutBucketLifecycleConfigurationRequestBucketLifecycleConfigurationPutTypeDef",
     {
         "ChecksumAlgorithm": ChecksumAlgorithmType,
@@ -6344,29 +7383,29 @@
 class PutBucketLifecycleConfigurationRequestRequestTypeDef(
     _RequiredPutBucketLifecycleConfigurationRequestRequestTypeDef,
     _OptionalPutBucketLifecycleConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-GetBucketAnalyticsConfigurationOutputTypeDef = TypedDict(
-    "GetBucketAnalyticsConfigurationOutputTypeDef",
+GetBucketAnalyticsConfigurationOutputOutputTypeDef = TypedDict(
+    "GetBucketAnalyticsConfigurationOutputOutputTypeDef",
     {
-        "AnalyticsConfiguration": AnalyticsConfigurationTypeDef,
+        "AnalyticsConfiguration": AnalyticsConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListBucketAnalyticsConfigurationsOutputTypeDef = TypedDict(
-    "ListBucketAnalyticsConfigurationsOutputTypeDef",
+ListBucketAnalyticsConfigurationsOutputOutputTypeDef = TypedDict(
+    "ListBucketAnalyticsConfigurationsOutputOutputTypeDef",
     {
         "IsTruncated": bool,
         "ContinuationToken": str,
         "NextContinuationToken": str,
-        "AnalyticsConfigurationList": List[AnalyticsConfigurationTypeDef],
+        "AnalyticsConfigurationList": List[AnalyticsConfigurationOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutBucketAnalyticsConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketAnalyticsConfigurationRequestRequestTypeDef",
     {
@@ -6484,27 +7523,27 @@
 
 class RestoreObjectRequestRequestTypeDef(
     _RequiredRestoreObjectRequestRequestTypeDef, _OptionalRestoreObjectRequestRequestTypeDef
 ):
     pass
 
 
-GetBucketInventoryConfigurationOutputTypeDef = TypedDict(
-    "GetBucketInventoryConfigurationOutputTypeDef",
+GetBucketInventoryConfigurationOutputOutputTypeDef = TypedDict(
+    "GetBucketInventoryConfigurationOutputOutputTypeDef",
     {
-        "InventoryConfiguration": InventoryConfigurationTypeDef,
+        "InventoryConfiguration": InventoryConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListBucketInventoryConfigurationsOutputTypeDef = TypedDict(
-    "ListBucketInventoryConfigurationsOutputTypeDef",
+ListBucketInventoryConfigurationsOutputOutputTypeDef = TypedDict(
+    "ListBucketInventoryConfigurationsOutputOutputTypeDef",
     {
         "ContinuationToken": str,
-        "InventoryConfigurationList": List[InventoryConfigurationTypeDef],
+        "InventoryConfigurationList": List[InventoryConfigurationOutputTypeDef],
         "IsTruncated": bool,
         "NextContinuationToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutBucketInventoryConfigurationRequestRequestTypeDef = TypedDict(
@@ -6527,18 +7566,18 @@
 class PutBucketInventoryConfigurationRequestRequestTypeDef(
     _RequiredPutBucketInventoryConfigurationRequestRequestTypeDef,
     _OptionalPutBucketInventoryConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-GetBucketReplicationOutputTypeDef = TypedDict(
-    "GetBucketReplicationOutputTypeDef",
+GetBucketReplicationOutputOutputTypeDef = TypedDict(
+    "GetBucketReplicationOutputOutputTypeDef",
     {
-        "ReplicationConfiguration": ReplicationConfigurationTypeDef,
+        "ReplicationConfiguration": ReplicationConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutBucketReplicationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketReplicationRequestRequestTypeDef",
     {
```

### Comparing `mypy-boto3-s3-1.28.3/mypy_boto3_s3/type_defs.pyi` & `mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for s3 service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_s3.type_defs import AbortIncompleteMultipartUploadTypeDef
+    from mypy_boto3_s3.type_defs import AbortIncompleteMultipartUploadOutputTypeDef
 
-    data: AbortIncompleteMultipartUploadTypeDef = {...}
+    data: AbortIncompleteMultipartUploadOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Callable, Dict, List, Mapping, Sequence, Union
 
 from boto3.s3.transfer import TransferConfig
@@ -76,53 +76,61 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AbortIncompleteMultipartUploadOutputTypeDef",
     "AbortIncompleteMultipartUploadTypeDef",
-    "AbortMultipartUploadOutputTypeDef",
+    "AbortMultipartUploadOutputOutputTypeDef",
     "AbortMultipartUploadRequestMultipartUploadAbortTypeDef",
     "AbortMultipartUploadRequestRequestTypeDef",
     "AccelerateConfigurationTypeDef",
     "OwnerTypeDef",
+    "AccessControlTranslationOutputTypeDef",
     "AccessControlTranslationTypeDef",
+    "TagOutputTypeDef",
     "TagTypeDef",
+    "AnalyticsS3BucketDestinationOutputTypeDef",
     "AnalyticsS3BucketDestinationTypeDef",
     "CopySourceTypeDef",
     "BucketDownloadFileRequestTypeDef",
     "BucketDownloadFileobjRequestTypeDef",
-    "BucketTypeDef",
+    "BucketOutputTypeDef",
     "BucketUploadFileRequestTypeDef",
     "BucketUploadFileobjRequestTypeDef",
     "CORSRuleTypeDef",
+    "CORSRuleOutputTypeDef",
     "CSVInputTypeDef",
     "CSVOutputTypeDef",
-    "ChecksumTypeDef",
+    "ChecksumOutputTypeDef",
     "ClientDownloadFileRequestTypeDef",
     "ClientDownloadFileobjRequestTypeDef",
     "ClientGeneratePresignedPostRequestTypeDef",
     "ClientUploadFileRequestTypeDef",
     "ClientUploadFileobjRequestTypeDef",
+    "CloudFunctionConfigurationOutputTypeDef",
     "CloudFunctionConfigurationTypeDef",
-    "CommonPrefixTypeDef",
-    "CompleteMultipartUploadOutputTypeDef",
+    "CommonPrefixOutputTypeDef",
+    "CompleteMultipartUploadOutputOutputTypeDef",
     "CompletedPartTypeDef",
+    "ConditionOutputTypeDef",
     "ConditionTypeDef",
-    "CopyObjectResultTypeDef",
+    "CopyObjectResultOutputTypeDef",
     "CopyObjectRequestObjectCopyFromTypeDef",
     "CopyObjectRequestObjectSummaryCopyFromTypeDef",
-    "CopyPartResultTypeDef",
+    "CopyPartResultOutputTypeDef",
     "CreateBucketConfigurationTypeDef",
-    "CreateBucketOutputTypeDef",
-    "CreateMultipartUploadOutputTypeDef",
+    "CreateBucketOutputOutputTypeDef",
+    "CreateMultipartUploadOutputOutputTypeDef",
     "CreateMultipartUploadRequestObjectInitiateMultipartUploadTypeDef",
     "CreateMultipartUploadRequestObjectSummaryInitiateMultipartUploadTypeDef",
     "CreateMultipartUploadRequestRequestTypeDef",
+    "DefaultRetentionOutputTypeDef",
     "DefaultRetentionTypeDef",
     "DeleteBucketAnalyticsConfigurationRequestRequestTypeDef",
     "DeleteBucketCorsRequestBucketCorsDeleteTypeDef",
     "DeleteBucketCorsRequestRequestTypeDef",
     "DeleteBucketEncryptionRequestRequestTypeDef",
     "DeleteBucketIntelligentTieringConfigurationRequestRequestTypeDef",
     "DeleteBucketInventoryConfigurationRequestRequestTypeDef",
@@ -136,97 +144,113 @@
     "DeleteBucketReplicationRequestRequestTypeDef",
     "DeleteBucketRequestBucketDeleteTypeDef",
     "DeleteBucketRequestRequestTypeDef",
     "DeleteBucketTaggingRequestBucketTaggingDeleteTypeDef",
     "DeleteBucketTaggingRequestRequestTypeDef",
     "DeleteBucketWebsiteRequestBucketWebsiteDeleteTypeDef",
     "DeleteBucketWebsiteRequestRequestTypeDef",
+    "OwnerOutputTypeDef",
+    "DeleteMarkerReplicationOutputTypeDef",
     "DeleteMarkerReplicationTypeDef",
-    "DeleteObjectOutputTypeDef",
+    "DeleteObjectOutputOutputTypeDef",
     "DeleteObjectRequestObjectDeleteTypeDef",
     "DeleteObjectRequestObjectSummaryDeleteTypeDef",
     "DeleteObjectRequestObjectVersionDeleteTypeDef",
     "DeleteObjectRequestRequestTypeDef",
-    "DeleteObjectTaggingOutputTypeDef",
+    "DeleteObjectTaggingOutputOutputTypeDef",
     "DeleteObjectTaggingRequestRequestTypeDef",
-    "DeletedObjectTypeDef",
-    "ErrorTypeDef",
+    "DeletedObjectOutputTypeDef",
+    "ErrorOutputTypeDef",
     "DeletePublicAccessBlockRequestRequestTypeDef",
     "ObjectIdentifierTypeDef",
+    "EncryptionConfigurationOutputTypeDef",
     "EncryptionConfigurationTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EncryptionTypeDef",
+    "ErrorDocumentOutputTypeDef",
     "ErrorDocumentResponseMetadataTypeDef",
     "ErrorDocumentTypeDef",
+    "ExistingObjectReplicationOutputTypeDef",
     "ExistingObjectReplicationTypeDef",
+    "FilterRuleOutputTypeDef",
     "FilterRuleTypeDef",
-    "GetBucketAccelerateConfigurationOutputTypeDef",
+    "GetBucketAccelerateConfigurationOutputOutputTypeDef",
     "GetBucketAccelerateConfigurationRequestRequestTypeDef",
     "GetBucketAclRequestRequestTypeDef",
     "GetBucketAnalyticsConfigurationRequestRequestTypeDef",
     "GetBucketCorsRequestRequestTypeDef",
     "GetBucketEncryptionRequestRequestTypeDef",
     "GetBucketIntelligentTieringConfigurationRequestRequestTypeDef",
     "GetBucketInventoryConfigurationRequestRequestTypeDef",
     "GetBucketLifecycleConfigurationRequestRequestTypeDef",
     "GetBucketLifecycleRequestRequestTypeDef",
-    "GetBucketLocationOutputTypeDef",
+    "GetBucketLocationOutputOutputTypeDef",
     "GetBucketLocationRequestRequestTypeDef",
     "GetBucketLoggingRequestRequestTypeDef",
     "GetBucketMetricsConfigurationRequestRequestTypeDef",
     "GetBucketNotificationConfigurationRequestRequestTypeDef",
     "GetBucketOwnershipControlsRequestRequestTypeDef",
-    "GetBucketPolicyOutputTypeDef",
+    "GetBucketPolicyOutputOutputTypeDef",
     "GetBucketPolicyRequestRequestTypeDef",
-    "PolicyStatusTypeDef",
+    "PolicyStatusOutputTypeDef",
     "GetBucketPolicyStatusRequestRequestTypeDef",
     "GetBucketReplicationRequestRequestTypeDef",
-    "GetBucketRequestPaymentOutputTypeDef",
+    "GetBucketRequestPaymentOutputOutputTypeDef",
     "GetBucketRequestPaymentRequestRequestTypeDef",
     "GetBucketTaggingRequestRequestTypeDef",
-    "GetBucketVersioningOutputTypeDef",
+    "GetBucketVersioningOutputOutputTypeDef",
     "GetBucketVersioningRequestRequestTypeDef",
-    "IndexDocumentTypeDef",
-    "RedirectAllRequestsToTypeDef",
+    "IndexDocumentOutputTypeDef",
+    "RedirectAllRequestsToOutputTypeDef",
     "GetBucketWebsiteRequestRequestTypeDef",
     "GetObjectAclRequestRequestTypeDef",
-    "ObjectPartTypeDef",
+    "ObjectPartOutputTypeDef",
     "GetObjectAttributesRequestRequestTypeDef",
-    "ObjectLockLegalHoldTypeDef",
+    "ObjectLockLegalHoldOutputTypeDef",
     "GetObjectLegalHoldRequestRequestTypeDef",
     "GetObjectLockConfigurationRequestRequestTypeDef",
-    "GetObjectOutputTypeDef",
+    "GetObjectOutputOutputTypeDef",
     "GetObjectRequestObjectGetTypeDef",
     "GetObjectRequestObjectSummaryGetTypeDef",
     "GetObjectRequestObjectVersionGetTypeDef",
     "GetObjectRequestRequestTypeDef",
-    "ObjectLockRetentionTypeDef",
+    "ObjectLockRetentionOutputTypeDef",
     "GetObjectRetentionRequestRequestTypeDef",
     "GetObjectTaggingRequestRequestTypeDef",
-    "GetObjectTorrentOutputTypeDef",
+    "GetObjectTorrentOutputOutputTypeDef",
     "GetObjectTorrentRequestRequestTypeDef",
-    "PublicAccessBlockConfigurationTypeDef",
+    "PublicAccessBlockConfigurationOutputTypeDef",
     "GetPublicAccessBlockRequestRequestTypeDef",
     "GlacierJobParametersTypeDef",
+    "GranteeOutputTypeDef",
     "GranteeTypeDef",
     "WaiterConfigTypeDef",
     "HeadBucketRequestRequestTypeDef",
-    "HeadObjectOutputTypeDef",
+    "HeadObjectOutputOutputTypeDef",
     "HeadObjectRequestObjectVersionHeadTypeDef",
     "HeadObjectRequestRequestTypeDef",
     "IndexDocumentResponseMetadataTypeDef",
+    "IndexDocumentTypeDef",
+    "InitiatorOutputTypeDef",
     "InitiatorResponseMetadataTypeDef",
-    "InitiatorTypeDef",
     "JSONInputTypeDef",
+    "TieringOutputTypeDef",
     "TieringTypeDef",
+    "InventoryFilterOutputTypeDef",
+    "InventoryScheduleOutputTypeDef",
     "InventoryFilterTypeDef",
     "InventoryScheduleTypeDef",
+    "SSEKMSOutputTypeDef",
     "SSEKMSTypeDef",
     "JSONOutputTypeDef",
+    "LifecycleExpirationOutputTypeDef",
     "LifecycleExpirationTypeDef",
+    "NoncurrentVersionExpirationOutputTypeDef",
+    "NoncurrentVersionTransitionOutputTypeDef",
+    "TransitionOutputTypeDef",
     "NoncurrentVersionExpirationTypeDef",
     "NoncurrentVersionTransitionTypeDef",
     "TransitionTypeDef",
     "ListBucketAnalyticsConfigurationsRequestRequestTypeDef",
     "ListBucketIntelligentTieringConfigurationsRequestRequestTypeDef",
     "ListBucketInventoryConfigurationsRequestRequestTypeDef",
     "ListBucketMetricsConfigurationsRequestRequestTypeDef",
@@ -234,236 +258,298 @@
     "ListMultipartUploadsRequestRequestTypeDef",
     "ListObjectVersionsRequestListObjectVersionsPaginateTypeDef",
     "ListObjectVersionsRequestRequestTypeDef",
     "ListObjectsRequestListObjectsPaginateTypeDef",
     "ListObjectsRequestRequestTypeDef",
     "ListObjectsV2RequestListObjectsV2PaginateTypeDef",
     "ListObjectsV2RequestRequestTypeDef",
-    "PartTypeDef",
+    "PartOutputTypeDef",
     "ListPartsRequestListPartsPaginateTypeDef",
     "ListPartsRequestRequestTypeDef",
     "MetadataEntryTypeDef",
+    "ReplicationTimeValueOutputTypeDef",
     "ReplicationTimeValueTypeDef",
+    "QueueConfigurationDeprecatedOutputTypeDef",
+    "TopicConfigurationDeprecatedOutputTypeDef",
     "QueueConfigurationDeprecatedTypeDef",
     "TopicConfigurationDeprecatedTypeDef",
     "ObjectDownloadFileRequestTypeDef",
     "ObjectDownloadFileobjRequestTypeDef",
-    "RestoreStatusTypeDef",
+    "ObjectLockLegalHoldTypeDef",
+    "ObjectLockRetentionTypeDef",
+    "RestoreStatusOutputTypeDef",
     "ObjectUploadFileRequestTypeDef",
     "ObjectUploadFileobjRequestTypeDef",
     "OwnerResponseMetadataTypeDef",
+    "OwnershipControlsRuleOutputTypeDef",
     "OwnershipControlsRuleTypeDef",
     "PaginatorConfigTypeDef",
-    "ProgressTypeDef",
+    "ProgressOutputTypeDef",
+    "PublicAccessBlockConfigurationTypeDef",
     "PutBucketPolicyRequestBucketPolicyPutTypeDef",
     "PutBucketPolicyRequestRequestTypeDef",
     "RequestPaymentConfigurationTypeDef",
     "PutBucketVersioningRequestBucketVersioningEnableTypeDef",
     "VersioningConfigurationTypeDef",
     "PutBucketVersioningRequestBucketVersioningSuspendTypeDef",
-    "PutObjectAclOutputTypeDef",
-    "PutObjectLegalHoldOutputTypeDef",
-    "PutObjectLockConfigurationOutputTypeDef",
-    "PutObjectOutputTypeDef",
+    "PutObjectAclOutputOutputTypeDef",
+    "PutObjectLegalHoldOutputOutputTypeDef",
+    "PutObjectLockConfigurationOutputOutputTypeDef",
+    "PutObjectOutputOutputTypeDef",
     "PutObjectRequestBucketPutObjectTypeDef",
     "PutObjectRequestObjectPutTypeDef",
     "PutObjectRequestObjectSummaryPutTypeDef",
     "PutObjectRequestRequestTypeDef",
-    "PutObjectRetentionOutputTypeDef",
-    "PutObjectTaggingOutputTypeDef",
-    "RecordsEventTypeDef",
+    "PutObjectRetentionOutputOutputTypeDef",
+    "PutObjectTaggingOutputOutputTypeDef",
+    "RecordsEventOutputTypeDef",
     "RedirectAllRequestsToResponseMetadataTypeDef",
+    "RedirectAllRequestsToTypeDef",
+    "RedirectOutputTypeDef",
     "RedirectTypeDef",
+    "ReplicaModificationsOutputTypeDef",
     "ReplicaModificationsTypeDef",
     "RequestProgressTypeDef",
     "ResponseMetadataTypeDef",
-    "RestoreObjectOutputTypeDef",
+    "RestoreObjectOutputOutputTypeDef",
     "RestoreStatusResponseMetadataTypeDef",
     "ScanRangeTypeDef",
+    "ServerSideEncryptionByDefaultOutputTypeDef",
     "ServerSideEncryptionByDefaultTypeDef",
+    "SseKmsEncryptedObjectsOutputTypeDef",
     "SseKmsEncryptedObjectsTypeDef",
-    "StatsTypeDef",
-    "UploadPartOutputTypeDef",
+    "StatsOutputTypeDef",
+    "UploadPartOutputOutputTypeDef",
     "UploadPartRequestMultipartUploadPartUploadTypeDef",
     "UploadPartRequestRequestTypeDef",
     "WriteGetObjectResponseRequestRequestTypeDef",
     "PutBucketAccelerateConfigurationRequestRequestTypeDef",
-    "DeleteMarkerEntryTypeDef",
+    "AnalyticsAndOperatorOutputTypeDef",
+    "GetBucketTaggingOutputOutputTypeDef",
+    "GetObjectTaggingOutputOutputTypeDef",
+    "IntelligentTieringAndOperatorOutputTypeDef",
+    "LifecycleRuleAndOperatorOutputTypeDef",
+    "MetricsAndOperatorOutputTypeDef",
+    "ReplicationRuleAndOperatorOutputTypeDef",
     "AnalyticsAndOperatorTypeDef",
-    "GetBucketTaggingOutputTypeDef",
-    "GetObjectTaggingOutputTypeDef",
     "IntelligentTieringAndOperatorTypeDef",
     "LifecycleRuleAndOperatorTypeDef",
     "MetricsAndOperatorTypeDef",
     "ReplicationRuleAndOperatorTypeDef",
     "TaggingTypeDef",
+    "AnalyticsExportDestinationOutputTypeDef",
     "AnalyticsExportDestinationTypeDef",
     "BucketCopyRequestTypeDef",
     "ClientCopyRequestTypeDef",
     "CopyObjectRequestRequestTypeDef",
     "ObjectCopyRequestTypeDef",
     "UploadPartCopyRequestMultipartUploadPartCopyFromTypeDef",
     "UploadPartCopyRequestRequestTypeDef",
-    "ListBucketsOutputTypeDef",
     "CORSConfigurationTypeDef",
-    "GetBucketCorsOutputTypeDef",
+    "GetBucketCorsOutputOutputTypeDef",
     "CompletedMultipartUploadTypeDef",
-    "CopyObjectOutputTypeDef",
-    "UploadPartCopyOutputTypeDef",
+    "CopyObjectOutputOutputTypeDef",
+    "UploadPartCopyOutputOutputTypeDef",
     "CreateBucketRequestBucketCreateTypeDef",
     "CreateBucketRequestRequestTypeDef",
     "CreateBucketRequestServiceResourceCreateBucketTypeDef",
+    "ObjectLockRuleOutputTypeDef",
     "ObjectLockRuleTypeDef",
-    "DeleteObjectsOutputTypeDef",
+    "DeleteMarkerEntryOutputTypeDef",
+    "ListBucketsOutputOutputTypeDef",
+    "DeleteObjectsOutputOutputTypeDef",
     "DeleteTypeDef",
+    "S3KeyFilterOutputTypeDef",
     "S3KeyFilterTypeDef",
-    "GetBucketPolicyStatusOutputTypeDef",
-    "GetObjectAttributesPartsTypeDef",
-    "GetObjectLegalHoldOutputTypeDef",
-    "PutObjectLegalHoldRequestRequestTypeDef",
-    "GetObjectRetentionOutputTypeDef",
-    "PutObjectRetentionRequestRequestTypeDef",
-    "GetPublicAccessBlockOutputTypeDef",
-    "PutPublicAccessBlockRequestRequestTypeDef",
+    "GetBucketPolicyStatusOutputOutputTypeDef",
+    "GetObjectAttributesPartsOutputTypeDef",
+    "GetObjectLegalHoldOutputOutputTypeDef",
+    "GetObjectRetentionOutputOutputTypeDef",
+    "GetPublicAccessBlockOutputOutputTypeDef",
+    "GrantOutputTypeDef",
+    "TargetGrantOutputTypeDef",
     "GrantTypeDef",
     "TargetGrantTypeDef",
     "HeadBucketRequestBucketExistsWaitTypeDef",
     "HeadBucketRequestBucketNotExistsWaitTypeDef",
     "HeadObjectRequestObjectExistsWaitTypeDef",
     "HeadObjectRequestObjectNotExistsWaitTypeDef",
-    "MultipartUploadTypeDef",
+    "MultipartUploadOutputTypeDef",
     "InputSerializationTypeDef",
+    "InventoryEncryptionOutputTypeDef",
     "InventoryEncryptionTypeDef",
     "OutputSerializationTypeDef",
+    "RuleOutputTypeDef",
     "RuleTypeDef",
-    "ListPartsOutputTypeDef",
+    "ListPartsOutputOutputTypeDef",
+    "MetricsOutputTypeDef",
+    "ReplicationTimeOutputTypeDef",
     "MetricsTypeDef",
     "ReplicationTimeTypeDef",
-    "NotificationConfigurationDeprecatedResponseMetadataTypeDef",
+    "NotificationConfigurationDeprecatedOutputTypeDef",
     "NotificationConfigurationDeprecatedTypeDef",
-    "ObjectTypeDef",
-    "ObjectVersionTypeDef",
+    "PutObjectLegalHoldRequestRequestTypeDef",
+    "PutObjectRetentionRequestRequestTypeDef",
+    "ObjectOutputTypeDef",
+    "ObjectVersionOutputTypeDef",
+    "OwnershipControlsOutputTypeDef",
     "OwnershipControlsTypeDef",
-    "ProgressEventTypeDef",
+    "ProgressEventOutputTypeDef",
+    "PutPublicAccessBlockRequestRequestTypeDef",
     "PutBucketRequestPaymentRequestBucketRequestPaymentPutTypeDef",
     "PutBucketRequestPaymentRequestRequestTypeDef",
     "PutBucketVersioningRequestBucketVersioningPutTypeDef",
     "PutBucketVersioningRequestRequestTypeDef",
+    "RoutingRuleOutputTypeDef",
     "RoutingRuleTypeDef",
+    "ServerSideEncryptionRuleOutputTypeDef",
     "ServerSideEncryptionRuleTypeDef",
+    "SourceSelectionCriteriaOutputTypeDef",
     "SourceSelectionCriteriaTypeDef",
-    "StatsEventTypeDef",
+    "StatsEventOutputTypeDef",
+    "AnalyticsFilterOutputTypeDef",
+    "IntelligentTieringFilterOutputTypeDef",
+    "LifecycleRuleFilterOutputTypeDef",
+    "MetricsFilterOutputTypeDef",
+    "ReplicationRuleFilterOutputTypeDef",
     "AnalyticsFilterTypeDef",
     "IntelligentTieringFilterTypeDef",
     "LifecycleRuleFilterTypeDef",
     "MetricsFilterTypeDef",
     "ReplicationRuleFilterTypeDef",
     "PutBucketTaggingRequestBucketTaggingPutTypeDef",
     "PutBucketTaggingRequestRequestTypeDef",
     "PutObjectTaggingRequestRequestTypeDef",
+    "StorageClassAnalysisDataExportOutputTypeDef",
     "StorageClassAnalysisDataExportTypeDef",
     "PutBucketCorsRequestBucketCorsPutTypeDef",
     "PutBucketCorsRequestRequestTypeDef",
     "CompleteMultipartUploadRequestMultipartUploadCompleteTypeDef",
     "CompleteMultipartUploadRequestRequestTypeDef",
+    "ObjectLockConfigurationOutputTypeDef",
     "ObjectLockConfigurationTypeDef",
     "DeleteObjectsRequestBucketDeleteObjectsTypeDef",
     "DeleteObjectsRequestRequestTypeDef",
+    "NotificationConfigurationFilterOutputTypeDef",
     "NotificationConfigurationFilterTypeDef",
-    "GetObjectAttributesOutputTypeDef",
+    "GetObjectAttributesOutputOutputTypeDef",
+    "GetBucketAclOutputOutputTypeDef",
+    "GetObjectAclOutputOutputTypeDef",
+    "LoggingEnabledOutputTypeDef",
+    "LoggingEnabledResponseMetadataTypeDef",
     "AccessControlPolicyTypeDef",
-    "GetBucketAclOutputTypeDef",
-    "GetObjectAclOutputTypeDef",
     "S3LocationTypeDef",
-    "LoggingEnabledResponseMetadataTypeDef",
     "LoggingEnabledTypeDef",
-    "ListMultipartUploadsOutputTypeDef",
+    "ListMultipartUploadsOutputOutputTypeDef",
+    "InventoryS3BucketDestinationOutputTypeDef",
     "InventoryS3BucketDestinationTypeDef",
     "SelectObjectContentRequestRequestTypeDef",
     "SelectParametersTypeDef",
-    "GetBucketLifecycleOutputTypeDef",
+    "GetBucketLifecycleOutputOutputTypeDef",
     "LifecycleConfigurationTypeDef",
+    "DestinationOutputTypeDef",
     "DestinationTypeDef",
     "PutBucketNotificationRequestRequestTypeDef",
-    "ListObjectsOutputTypeDef",
-    "ListObjectsV2OutputTypeDef",
-    "ListObjectVersionsOutputTypeDef",
-    "GetBucketOwnershipControlsOutputTypeDef",
+    "ListObjectsOutputOutputTypeDef",
+    "ListObjectsV2OutputOutputTypeDef",
+    "ListObjectVersionsOutputOutputTypeDef",
+    "GetBucketOwnershipControlsOutputOutputTypeDef",
     "PutBucketOwnershipControlsRequestRequestTypeDef",
-    "GetBucketWebsiteOutputTypeDef",
+    "GetBucketWebsiteOutputOutputTypeDef",
     "WebsiteConfigurationTypeDef",
+    "ServerSideEncryptionConfigurationOutputTypeDef",
     "ServerSideEncryptionConfigurationTypeDef",
-    "SelectObjectContentEventStreamTypeDef",
+    "SelectObjectContentEventStreamOutputTypeDef",
+    "IntelligentTieringConfigurationOutputTypeDef",
+    "LifecycleRuleOutputTypeDef",
+    "MetricsConfigurationOutputTypeDef",
     "IntelligentTieringConfigurationTypeDef",
     "LifecycleRuleTypeDef",
     "MetricsConfigurationTypeDef",
+    "StorageClassAnalysisOutputTypeDef",
     "StorageClassAnalysisTypeDef",
-    "GetObjectLockConfigurationOutputTypeDef",
+    "GetObjectLockConfigurationOutputOutputTypeDef",
     "PutObjectLockConfigurationRequestRequestTypeDef",
+    "LambdaFunctionConfigurationOutputTypeDef",
+    "QueueConfigurationOutputTypeDef",
+    "TopicConfigurationOutputTypeDef",
     "LambdaFunctionConfigurationTypeDef",
     "QueueConfigurationTypeDef",
     "TopicConfigurationTypeDef",
+    "GetBucketLoggingOutputOutputTypeDef",
     "PutBucketAclRequestBucketAclPutTypeDef",
     "PutBucketAclRequestRequestTypeDef",
     "PutObjectAclRequestObjectAclPutTypeDef",
     "PutObjectAclRequestRequestTypeDef",
     "OutputLocationTypeDef",
     "BucketLoggingStatusTypeDef",
-    "GetBucketLoggingOutputTypeDef",
+    "InventoryDestinationOutputTypeDef",
     "InventoryDestinationTypeDef",
     "PutBucketLifecycleRequestBucketLifecyclePutTypeDef",
     "PutBucketLifecycleRequestRequestTypeDef",
+    "ReplicationRuleOutputTypeDef",
     "ReplicationRuleTypeDef",
     "PutBucketWebsiteRequestBucketWebsitePutTypeDef",
     "PutBucketWebsiteRequestRequestTypeDef",
-    "GetBucketEncryptionOutputTypeDef",
+    "GetBucketEncryptionOutputOutputTypeDef",
     "PutBucketEncryptionRequestRequestTypeDef",
-    "SelectObjectContentOutputTypeDef",
-    "GetBucketIntelligentTieringConfigurationOutputTypeDef",
-    "ListBucketIntelligentTieringConfigurationsOutputTypeDef",
+    "SelectObjectContentOutputOutputTypeDef",
+    "GetBucketIntelligentTieringConfigurationOutputOutputTypeDef",
+    "ListBucketIntelligentTieringConfigurationsOutputOutputTypeDef",
+    "GetBucketLifecycleConfigurationOutputOutputTypeDef",
+    "GetBucketMetricsConfigurationOutputOutputTypeDef",
+    "ListBucketMetricsConfigurationsOutputOutputTypeDef",
     "PutBucketIntelligentTieringConfigurationRequestRequestTypeDef",
     "BucketLifecycleConfigurationTypeDef",
-    "GetBucketLifecycleConfigurationOutputTypeDef",
-    "GetBucketMetricsConfigurationOutputTypeDef",
-    "ListBucketMetricsConfigurationsOutputTypeDef",
     "PutBucketMetricsConfigurationRequestRequestTypeDef",
+    "AnalyticsConfigurationOutputTypeDef",
     "AnalyticsConfigurationTypeDef",
-    "NotificationConfigurationResponseMetadataTypeDef",
+    "NotificationConfigurationOutputTypeDef",
     "NotificationConfigurationTypeDef",
     "RestoreRequestTypeDef",
     "PutBucketLoggingRequestBucketLoggingPutTypeDef",
     "PutBucketLoggingRequestRequestTypeDef",
+    "InventoryConfigurationOutputTypeDef",
     "InventoryConfigurationTypeDef",
+    "ReplicationConfigurationOutputTypeDef",
     "ReplicationConfigurationTypeDef",
     "PutBucketLifecycleConfigurationRequestBucketLifecycleConfigurationPutTypeDef",
     "PutBucketLifecycleConfigurationRequestRequestTypeDef",
-    "GetBucketAnalyticsConfigurationOutputTypeDef",
-    "ListBucketAnalyticsConfigurationsOutputTypeDef",
+    "GetBucketAnalyticsConfigurationOutputOutputTypeDef",
+    "ListBucketAnalyticsConfigurationsOutputOutputTypeDef",
     "PutBucketAnalyticsConfigurationRequestRequestTypeDef",
     "PutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef",
     "PutBucketNotificationConfigurationRequestRequestTypeDef",
     "RestoreObjectRequestObjectRestoreObjectTypeDef",
     "RestoreObjectRequestObjectSummaryRestoreObjectTypeDef",
     "RestoreObjectRequestRequestTypeDef",
-    "GetBucketInventoryConfigurationOutputTypeDef",
-    "ListBucketInventoryConfigurationsOutputTypeDef",
+    "GetBucketInventoryConfigurationOutputOutputTypeDef",
+    "ListBucketInventoryConfigurationsOutputOutputTypeDef",
     "PutBucketInventoryConfigurationRequestRequestTypeDef",
-    "GetBucketReplicationOutputTypeDef",
+    "GetBucketReplicationOutputOutputTypeDef",
     "PutBucketReplicationRequestRequestTypeDef",
 )
 
+AbortIncompleteMultipartUploadOutputTypeDef = TypedDict(
+    "AbortIncompleteMultipartUploadOutputTypeDef",
+    {
+        "DaysAfterInitiation": int,
+    },
+)
+
 AbortIncompleteMultipartUploadTypeDef = TypedDict(
     "AbortIncompleteMultipartUploadTypeDef",
     {
         "DaysAfterInitiation": int,
     },
+    total=False,
 )
 
-AbortMultipartUploadOutputTypeDef = TypedDict(
-    "AbortMultipartUploadOutputTypeDef",
+AbortMultipartUploadOutputOutputTypeDef = TypedDict(
+    "AbortMultipartUploadOutputOutputTypeDef",
     {
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AbortMultipartUploadRequestMultipartUploadAbortTypeDef = TypedDict(
@@ -508,41 +594,78 @@
 
 OwnerTypeDef = TypedDict(
     "OwnerTypeDef",
     {
         "DisplayName": str,
         "ID": str,
     },
+    total=False,
+)
+
+AccessControlTranslationOutputTypeDef = TypedDict(
+    "AccessControlTranslationOutputTypeDef",
+    {
+        "Owner": Literal["Destination"],
+    },
 )
 
 AccessControlTranslationTypeDef = TypedDict(
     "AccessControlTranslationTypeDef",
     {
         "Owner": Literal["Destination"],
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-AnalyticsS3BucketDestinationTypeDef = TypedDict(
-    "AnalyticsS3BucketDestinationTypeDef",
+AnalyticsS3BucketDestinationOutputTypeDef = TypedDict(
+    "AnalyticsS3BucketDestinationOutputTypeDef",
     {
         "Format": Literal["CSV"],
         "BucketAccountId": str,
         "Bucket": str,
         "Prefix": str,
     },
 )
 
+_RequiredAnalyticsS3BucketDestinationTypeDef = TypedDict(
+    "_RequiredAnalyticsS3BucketDestinationTypeDef",
+    {
+        "Format": Literal["CSV"],
+        "Bucket": str,
+    },
+)
+_OptionalAnalyticsS3BucketDestinationTypeDef = TypedDict(
+    "_OptionalAnalyticsS3BucketDestinationTypeDef",
+    {
+        "BucketAccountId": str,
+        "Prefix": str,
+    },
+    total=False,
+)
+
+class AnalyticsS3BucketDestinationTypeDef(
+    _RequiredAnalyticsS3BucketDestinationTypeDef, _OptionalAnalyticsS3BucketDestinationTypeDef
+):
+    pass
+
 _RequiredCopySourceTypeDef = TypedDict(
     "_RequiredCopySourceTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
 )
@@ -597,16 +720,16 @@
 )
 
 class BucketDownloadFileobjRequestTypeDef(
     _RequiredBucketDownloadFileobjRequestTypeDef, _OptionalBucketDownloadFileobjRequestTypeDef
 ):
     pass
 
-BucketTypeDef = TypedDict(
-    "BucketTypeDef",
+BucketOutputTypeDef = TypedDict(
+    "BucketOutputTypeDef",
     {
         "Name": str,
         "CreationDate": datetime,
     },
 )
 
 _RequiredBucketUploadFileRequestTypeDef = TypedDict(
@@ -649,16 +772,37 @@
 )
 
 class BucketUploadFileobjRequestTypeDef(
     _RequiredBucketUploadFileobjRequestTypeDef, _OptionalBucketUploadFileobjRequestTypeDef
 ):
     pass
 
-CORSRuleTypeDef = TypedDict(
-    "CORSRuleTypeDef",
+_RequiredCORSRuleTypeDef = TypedDict(
+    "_RequiredCORSRuleTypeDef",
+    {
+        "AllowedMethods": Sequence[str],
+        "AllowedOrigins": Sequence[str],
+    },
+)
+_OptionalCORSRuleTypeDef = TypedDict(
+    "_OptionalCORSRuleTypeDef",
+    {
+        "ID": str,
+        "AllowedHeaders": Sequence[str],
+        "ExposeHeaders": Sequence[str],
+        "MaxAgeSeconds": int,
+    },
+    total=False,
+)
+
+class CORSRuleTypeDef(_RequiredCORSRuleTypeDef, _OptionalCORSRuleTypeDef):
+    pass
+
+CORSRuleOutputTypeDef = TypedDict(
+    "CORSRuleOutputTypeDef",
     {
         "ID": str,
         "AllowedHeaders": List[str],
         "AllowedMethods": List[str],
         "AllowedOrigins": List[str],
         "ExposeHeaders": List[str],
         "MaxAgeSeconds": int,
@@ -687,16 +831,16 @@
         "RecordDelimiter": str,
         "FieldDelimiter": str,
         "QuoteCharacter": str,
     },
     total=False,
 )
 
-ChecksumTypeDef = TypedDict(
-    "ChecksumTypeDef",
+ChecksumOutputTypeDef = TypedDict(
+    "ChecksumOutputTypeDef",
     {
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
         "ChecksumSHA256": str,
     },
 )
@@ -812,34 +956,46 @@
 )
 
 class ClientUploadFileobjRequestTypeDef(
     _RequiredClientUploadFileobjRequestTypeDef, _OptionalClientUploadFileobjRequestTypeDef
 ):
     pass
 
+CloudFunctionConfigurationOutputTypeDef = TypedDict(
+    "CloudFunctionConfigurationOutputTypeDef",
+    {
+        "Id": str,
+        "Event": EventType,
+        "Events": List[EventType],
+        "CloudFunction": str,
+        "InvocationRole": str,
+    },
+)
+
 CloudFunctionConfigurationTypeDef = TypedDict(
     "CloudFunctionConfigurationTypeDef",
     {
         "Id": str,
         "Event": EventType,
-        "Events": List[EventType],
+        "Events": Sequence[EventType],
         "CloudFunction": str,
         "InvocationRole": str,
     },
+    total=False,
 )
 
-CommonPrefixTypeDef = TypedDict(
-    "CommonPrefixTypeDef",
+CommonPrefixOutputTypeDef = TypedDict(
+    "CommonPrefixOutputTypeDef",
     {
         "Prefix": str,
     },
 )
 
-CompleteMultipartUploadOutputTypeDef = TypedDict(
-    "CompleteMultipartUploadOutputTypeDef",
+CompleteMultipartUploadOutputOutputTypeDef = TypedDict(
+    "CompleteMultipartUploadOutputOutputTypeDef",
     {
         "Location": str,
         "Bucket": str,
         "Key": str,
         "Expiration": str,
         "ETag": str,
         "ChecksumCRC32": str,
@@ -864,24 +1020,33 @@
         "ChecksumSHA1": str,
         "ChecksumSHA256": str,
         "PartNumber": int,
     },
     total=False,
 )
 
+ConditionOutputTypeDef = TypedDict(
+    "ConditionOutputTypeDef",
+    {
+        "HttpErrorCodeReturnedEquals": str,
+        "KeyPrefixEquals": str,
+    },
+)
+
 ConditionTypeDef = TypedDict(
     "ConditionTypeDef",
     {
         "HttpErrorCodeReturnedEquals": str,
         "KeyPrefixEquals": str,
     },
+    total=False,
 )
 
-CopyObjectResultTypeDef = TypedDict(
-    "CopyObjectResultTypeDef",
+CopyObjectResultOutputTypeDef = TypedDict(
+    "CopyObjectResultOutputTypeDef",
     {
         "ETag": str,
         "LastModified": datetime,
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
         "ChecksumSHA256": str,
@@ -997,16 +1162,16 @@
 
 class CopyObjectRequestObjectSummaryCopyFromTypeDef(
     _RequiredCopyObjectRequestObjectSummaryCopyFromTypeDef,
     _OptionalCopyObjectRequestObjectSummaryCopyFromTypeDef,
 ):
     pass
 
-CopyPartResultTypeDef = TypedDict(
-    "CopyPartResultTypeDef",
+CopyPartResultOutputTypeDef = TypedDict(
+    "CopyPartResultOutputTypeDef",
     {
         "ETag": str,
         "LastModified": datetime,
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
         "ChecksumSHA256": str,
@@ -1017,24 +1182,24 @@
     "CreateBucketConfigurationTypeDef",
     {
         "LocationConstraint": BucketLocationConstraintType,
     },
     total=False,
 )
 
-CreateBucketOutputTypeDef = TypedDict(
-    "CreateBucketOutputTypeDef",
+CreateBucketOutputOutputTypeDef = TypedDict(
+    "CreateBucketOutputOutputTypeDef",
     {
         "Location": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateMultipartUploadOutputTypeDef = TypedDict(
-    "CreateMultipartUploadOutputTypeDef",
+CreateMultipartUploadOutputOutputTypeDef = TypedDict(
+    "CreateMultipartUploadOutputOutputTypeDef",
     {
         "AbortDate": datetime,
         "AbortRuleId": str,
         "Bucket": str,
         "Key": str,
         "UploadId": str,
         "ServerSideEncryption": ServerSideEncryptionType,
@@ -1163,21 +1328,31 @@
 
 class CreateMultipartUploadRequestRequestTypeDef(
     _RequiredCreateMultipartUploadRequestRequestTypeDef,
     _OptionalCreateMultipartUploadRequestRequestTypeDef,
 ):
     pass
 
+DefaultRetentionOutputTypeDef = TypedDict(
+    "DefaultRetentionOutputTypeDef",
+    {
+        "Mode": ObjectLockRetentionModeType,
+        "Days": int,
+        "Years": int,
+    },
+)
+
 DefaultRetentionTypeDef = TypedDict(
     "DefaultRetentionTypeDef",
     {
         "Mode": ObjectLockRetentionModeType,
         "Days": int,
         "Years": int,
     },
+    total=False,
 )
 
 _RequiredDeleteBucketAnalyticsConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteBucketAnalyticsConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
         "Id": str,
@@ -1477,23 +1652,39 @@
 
 class DeleteBucketWebsiteRequestRequestTypeDef(
     _RequiredDeleteBucketWebsiteRequestRequestTypeDef,
     _OptionalDeleteBucketWebsiteRequestRequestTypeDef,
 ):
     pass
 
+OwnerOutputTypeDef = TypedDict(
+    "OwnerOutputTypeDef",
+    {
+        "DisplayName": str,
+        "ID": str,
+    },
+)
+
+DeleteMarkerReplicationOutputTypeDef = TypedDict(
+    "DeleteMarkerReplicationOutputTypeDef",
+    {
+        "Status": DeleteMarkerReplicationStatusType,
+    },
+)
+
 DeleteMarkerReplicationTypeDef = TypedDict(
     "DeleteMarkerReplicationTypeDef",
     {
         "Status": DeleteMarkerReplicationStatusType,
     },
+    total=False,
 )
 
-DeleteObjectOutputTypeDef = TypedDict(
-    "DeleteObjectOutputTypeDef",
+DeleteObjectOutputOutputTypeDef = TypedDict(
+    "DeleteObjectOutputOutputTypeDef",
     {
         "DeleteMarker": bool,
         "VersionId": str,
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1553,16 +1744,16 @@
 )
 
 class DeleteObjectRequestRequestTypeDef(
     _RequiredDeleteObjectRequestRequestTypeDef, _OptionalDeleteObjectRequestRequestTypeDef
 ):
     pass
 
-DeleteObjectTaggingOutputTypeDef = TypedDict(
-    "DeleteObjectTaggingOutputTypeDef",
+DeleteObjectTaggingOutputOutputTypeDef = TypedDict(
+    "DeleteObjectTaggingOutputOutputTypeDef",
     {
         "VersionId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDeleteObjectTaggingRequestRequestTypeDef = TypedDict(
@@ -1583,26 +1774,26 @@
 
 class DeleteObjectTaggingRequestRequestTypeDef(
     _RequiredDeleteObjectTaggingRequestRequestTypeDef,
     _OptionalDeleteObjectTaggingRequestRequestTypeDef,
 ):
     pass
 
-DeletedObjectTypeDef = TypedDict(
-    "DeletedObjectTypeDef",
+DeletedObjectOutputTypeDef = TypedDict(
+    "DeletedObjectOutputTypeDef",
     {
         "Key": str,
         "VersionId": str,
         "DeleteMarker": bool,
         "DeleteMarkerVersionId": str,
     },
 )
 
-ErrorTypeDef = TypedDict(
-    "ErrorTypeDef",
+ErrorOutputTypeDef = TypedDict(
+    "ErrorOutputTypeDef",
     {
         "Key": str,
         "VersionId": str,
         "Code": str,
         "Message": str,
     },
 )
@@ -1640,19 +1831,27 @@
     },
     total=False,
 )
 
 class ObjectIdentifierTypeDef(_RequiredObjectIdentifierTypeDef, _OptionalObjectIdentifierTypeDef):
     pass
 
+EncryptionConfigurationOutputTypeDef = TypedDict(
+    "EncryptionConfigurationOutputTypeDef",
+    {
+        "ReplicaKmsKeyID": str,
+    },
+)
+
 EncryptionConfigurationTypeDef = TypedDict(
     "EncryptionConfigurationTypeDef",
     {
         "ReplicaKmsKeyID": str,
     },
+    total=False,
 )
 
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1672,14 +1871,21 @@
     },
     total=False,
 )
 
 class EncryptionTypeDef(_RequiredEncryptionTypeDef, _OptionalEncryptionTypeDef):
     pass
 
+ErrorDocumentOutputTypeDef = TypedDict(
+    "ErrorDocumentOutputTypeDef",
+    {
+        "Key": str,
+    },
+)
+
 ErrorDocumentResponseMetadataTypeDef = TypedDict(
     "ErrorDocumentResponseMetadataTypeDef",
     {
         "Key": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1687,31 +1893,47 @@
 ErrorDocumentTypeDef = TypedDict(
     "ErrorDocumentTypeDef",
     {
         "Key": str,
     },
 )
 
+ExistingObjectReplicationOutputTypeDef = TypedDict(
+    "ExistingObjectReplicationOutputTypeDef",
+    {
+        "Status": ExistingObjectReplicationStatusType,
+    },
+)
+
 ExistingObjectReplicationTypeDef = TypedDict(
     "ExistingObjectReplicationTypeDef",
     {
         "Status": ExistingObjectReplicationStatusType,
     },
 )
 
+FilterRuleOutputTypeDef = TypedDict(
+    "FilterRuleOutputTypeDef",
+    {
+        "Name": FilterRuleNameType,
+        "Value": str,
+    },
+)
+
 FilterRuleTypeDef = TypedDict(
     "FilterRuleTypeDef",
     {
         "Name": FilterRuleNameType,
         "Value": str,
     },
+    total=False,
 )
 
-GetBucketAccelerateConfigurationOutputTypeDef = TypedDict(
-    "GetBucketAccelerateConfigurationOutputTypeDef",
+GetBucketAccelerateConfigurationOutputOutputTypeDef = TypedDict(
+    "GetBucketAccelerateConfigurationOutputOutputTypeDef",
     {
         "Status": BucketAccelerateStatusType,
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1880,16 +2102,16 @@
 
 class GetBucketLifecycleRequestRequestTypeDef(
     _RequiredGetBucketLifecycleRequestRequestTypeDef,
     _OptionalGetBucketLifecycleRequestRequestTypeDef,
 ):
     pass
 
-GetBucketLocationOutputTypeDef = TypedDict(
-    "GetBucketLocationOutputTypeDef",
+GetBucketLocationOutputOutputTypeDef = TypedDict(
+    "GetBucketLocationOutputOutputTypeDef",
     {
         "LocationConstraint": BucketLocationConstraintType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetBucketLocationRequestRequestTypeDef = TypedDict(
@@ -1987,16 +2209,16 @@
 
 class GetBucketOwnershipControlsRequestRequestTypeDef(
     _RequiredGetBucketOwnershipControlsRequestRequestTypeDef,
     _OptionalGetBucketOwnershipControlsRequestRequestTypeDef,
 ):
     pass
 
-GetBucketPolicyOutputTypeDef = TypedDict(
-    "GetBucketPolicyOutputTypeDef",
+GetBucketPolicyOutputOutputTypeDef = TypedDict(
+    "GetBucketPolicyOutputOutputTypeDef",
     {
         "Policy": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetBucketPolicyRequestRequestTypeDef = TypedDict(
@@ -2014,16 +2236,16 @@
 )
 
 class GetBucketPolicyRequestRequestTypeDef(
     _RequiredGetBucketPolicyRequestRequestTypeDef, _OptionalGetBucketPolicyRequestRequestTypeDef
 ):
     pass
 
-PolicyStatusTypeDef = TypedDict(
-    "PolicyStatusTypeDef",
+PolicyStatusOutputTypeDef = TypedDict(
+    "PolicyStatusOutputTypeDef",
     {
         "IsPublic": bool,
     },
 )
 
 _RequiredGetBucketPolicyStatusRequestRequestTypeDef = TypedDict(
     "_RequiredGetBucketPolicyStatusRequestRequestTypeDef",
@@ -2061,16 +2283,16 @@
 
 class GetBucketReplicationRequestRequestTypeDef(
     _RequiredGetBucketReplicationRequestRequestTypeDef,
     _OptionalGetBucketReplicationRequestRequestTypeDef,
 ):
     pass
 
-GetBucketRequestPaymentOutputTypeDef = TypedDict(
-    "GetBucketRequestPaymentOutputTypeDef",
+GetBucketRequestPaymentOutputOutputTypeDef = TypedDict(
+    "GetBucketRequestPaymentOutputOutputTypeDef",
     {
         "Payer": PayerType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetBucketRequestPaymentRequestRequestTypeDef = TypedDict(
@@ -2108,16 +2330,16 @@
 )
 
 class GetBucketTaggingRequestRequestTypeDef(
     _RequiredGetBucketTaggingRequestRequestTypeDef, _OptionalGetBucketTaggingRequestRequestTypeDef
 ):
     pass
 
-GetBucketVersioningOutputTypeDef = TypedDict(
-    "GetBucketVersioningOutputTypeDef",
+GetBucketVersioningOutputOutputTypeDef = TypedDict(
+    "GetBucketVersioningOutputOutputTypeDef",
     {
         "Status": BucketVersioningStatusType,
         "MFADelete": MFADeleteStatusType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -2137,23 +2359,23 @@
 
 class GetBucketVersioningRequestRequestTypeDef(
     _RequiredGetBucketVersioningRequestRequestTypeDef,
     _OptionalGetBucketVersioningRequestRequestTypeDef,
 ):
     pass
 
-IndexDocumentTypeDef = TypedDict(
-    "IndexDocumentTypeDef",
+IndexDocumentOutputTypeDef = TypedDict(
+    "IndexDocumentOutputTypeDef",
     {
         "Suffix": str,
     },
 )
 
-RedirectAllRequestsToTypeDef = TypedDict(
-    "RedirectAllRequestsToTypeDef",
+RedirectAllRequestsToOutputTypeDef = TypedDict(
+    "RedirectAllRequestsToOutputTypeDef",
     {
         "HostName": str,
         "Protocol": ProtocolType,
     },
 )
 
 _RequiredGetBucketWebsiteRequestRequestTypeDef = TypedDict(
@@ -2193,16 +2415,16 @@
 )
 
 class GetObjectAclRequestRequestTypeDef(
     _RequiredGetObjectAclRequestRequestTypeDef, _OptionalGetObjectAclRequestRequestTypeDef
 ):
     pass
 
-ObjectPartTypeDef = TypedDict(
-    "ObjectPartTypeDef",
+ObjectPartOutputTypeDef = TypedDict(
+    "ObjectPartOutputTypeDef",
     {
         "PartNumber": int,
         "Size": int,
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
         "ChecksumSHA256": str,
@@ -2234,16 +2456,16 @@
 
 class GetObjectAttributesRequestRequestTypeDef(
     _RequiredGetObjectAttributesRequestRequestTypeDef,
     _OptionalGetObjectAttributesRequestRequestTypeDef,
 ):
     pass
 
-ObjectLockLegalHoldTypeDef = TypedDict(
-    "ObjectLockLegalHoldTypeDef",
+ObjectLockLegalHoldOutputTypeDef = TypedDict(
+    "ObjectLockLegalHoldOutputTypeDef",
     {
         "Status": ObjectLockLegalHoldStatusType,
     },
 )
 
 _RequiredGetObjectLegalHoldRequestRequestTypeDef = TypedDict(
     "_RequiredGetObjectLegalHoldRequestRequestTypeDef",
@@ -2284,16 +2506,16 @@
 
 class GetObjectLockConfigurationRequestRequestTypeDef(
     _RequiredGetObjectLockConfigurationRequestRequestTypeDef,
     _OptionalGetObjectLockConfigurationRequestRequestTypeDef,
 ):
     pass
 
-GetObjectOutputTypeDef = TypedDict(
-    "GetObjectOutputTypeDef",
+GetObjectOutputOutputTypeDef = TypedDict(
+    "GetObjectOutputOutputTypeDef",
     {
         "Body": StreamingBody,
         "DeleteMarker": bool,
         "AcceptRanges": str,
         "Expiration": str,
         "Restore": str,
         "LastModified": datetime,
@@ -2442,16 +2664,16 @@
 )
 
 class GetObjectRequestRequestTypeDef(
     _RequiredGetObjectRequestRequestTypeDef, _OptionalGetObjectRequestRequestTypeDef
 ):
     pass
 
-ObjectLockRetentionTypeDef = TypedDict(
-    "ObjectLockRetentionTypeDef",
+ObjectLockRetentionOutputTypeDef = TypedDict(
+    "ObjectLockRetentionOutputTypeDef",
     {
         "Mode": ObjectLockRetentionModeType,
         "RetainUntilDate": datetime,
     },
 )
 
 _RequiredGetObjectRetentionRequestRequestTypeDef = TypedDict(
@@ -2495,16 +2717,16 @@
 )
 
 class GetObjectTaggingRequestRequestTypeDef(
     _RequiredGetObjectTaggingRequestRequestTypeDef, _OptionalGetObjectTaggingRequestRequestTypeDef
 ):
     pass
 
-GetObjectTorrentOutputTypeDef = TypedDict(
-    "GetObjectTorrentOutputTypeDef",
+GetObjectTorrentOutputOutputTypeDef = TypedDict(
+    "GetObjectTorrentOutputOutputTypeDef",
     {
         "Body": StreamingBody,
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -2525,16 +2747,16 @@
 )
 
 class GetObjectTorrentRequestRequestTypeDef(
     _RequiredGetObjectTorrentRequestRequestTypeDef, _OptionalGetObjectTorrentRequestRequestTypeDef
 ):
     pass
 
-PublicAccessBlockConfigurationTypeDef = TypedDict(
-    "PublicAccessBlockConfigurationTypeDef",
+PublicAccessBlockConfigurationOutputTypeDef = TypedDict(
+    "PublicAccessBlockConfigurationOutputTypeDef",
     {
         "BlockPublicAcls": bool,
         "IgnorePublicAcls": bool,
         "BlockPublicPolicy": bool,
         "RestrictPublicBuckets": bool,
     },
 )
@@ -2562,25 +2784,45 @@
 GlacierJobParametersTypeDef = TypedDict(
     "GlacierJobParametersTypeDef",
     {
         "Tier": TierType,
     },
 )
 
-GranteeTypeDef = TypedDict(
-    "GranteeTypeDef",
+GranteeOutputTypeDef = TypedDict(
+    "GranteeOutputTypeDef",
     {
         "DisplayName": str,
         "EmailAddress": str,
         "ID": str,
         "Type": TypeType,
         "URI": str,
     },
 )
 
+_RequiredGranteeTypeDef = TypedDict(
+    "_RequiredGranteeTypeDef",
+    {
+        "Type": TypeType,
+    },
+)
+_OptionalGranteeTypeDef = TypedDict(
+    "_OptionalGranteeTypeDef",
+    {
+        "DisplayName": str,
+        "EmailAddress": str,
+        "ID": str,
+        "URI": str,
+    },
+    total=False,
+)
+
+class GranteeTypeDef(_RequiredGranteeTypeDef, _OptionalGranteeTypeDef):
+    pass
+
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -2601,16 +2843,16 @@
 )
 
 class HeadBucketRequestRequestTypeDef(
     _RequiredHeadBucketRequestRequestTypeDef, _OptionalHeadBucketRequestRequestTypeDef
 ):
     pass
 
-HeadObjectOutputTypeDef = TypedDict(
-    "HeadObjectOutputTypeDef",
+HeadObjectOutputOutputTypeDef = TypedDict(
+    "HeadObjectOutputOutputTypeDef",
     {
         "DeleteMarker": bool,
         "AcceptRanges": str,
         "Expiration": str,
         "Restore": str,
         "ArchiveStatus": ArchiveStatusType,
         "LastModified": datetime,
@@ -2701,61 +2943,97 @@
     "IndexDocumentResponseMetadataTypeDef",
     {
         "Suffix": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-InitiatorResponseMetadataTypeDef = TypedDict(
-    "InitiatorResponseMetadataTypeDef",
+IndexDocumentTypeDef = TypedDict(
+    "IndexDocumentTypeDef",
+    {
+        "Suffix": str,
+    },
+)
+
+InitiatorOutputTypeDef = TypedDict(
+    "InitiatorOutputTypeDef",
     {
         "ID": str,
         "DisplayName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-InitiatorTypeDef = TypedDict(
-    "InitiatorTypeDef",
+InitiatorResponseMetadataTypeDef = TypedDict(
+    "InitiatorResponseMetadataTypeDef",
     {
         "ID": str,
         "DisplayName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 JSONInputTypeDef = TypedDict(
     "JSONInputTypeDef",
     {
         "Type": JSONTypeType,
     },
     total=False,
 )
 
+TieringOutputTypeDef = TypedDict(
+    "TieringOutputTypeDef",
+    {
+        "Days": int,
+        "AccessTier": IntelligentTieringAccessTierType,
+    },
+)
+
 TieringTypeDef = TypedDict(
     "TieringTypeDef",
     {
         "Days": int,
         "AccessTier": IntelligentTieringAccessTierType,
     },
 )
 
+InventoryFilterOutputTypeDef = TypedDict(
+    "InventoryFilterOutputTypeDef",
+    {
+        "Prefix": str,
+    },
+)
+
+InventoryScheduleOutputTypeDef = TypedDict(
+    "InventoryScheduleOutputTypeDef",
+    {
+        "Frequency": InventoryFrequencyType,
+    },
+)
+
 InventoryFilterTypeDef = TypedDict(
     "InventoryFilterTypeDef",
     {
         "Prefix": str,
     },
 )
 
 InventoryScheduleTypeDef = TypedDict(
     "InventoryScheduleTypeDef",
     {
         "Frequency": InventoryFrequencyType,
     },
 )
 
+SSEKMSOutputTypeDef = TypedDict(
+    "SSEKMSOutputTypeDef",
+    {
+        "KeyId": str,
+    },
+)
+
 SSEKMSTypeDef = TypedDict(
     "SSEKMSTypeDef",
     {
         "KeyId": str,
     },
 )
 
@@ -2763,47 +3041,86 @@
     "JSONOutputTypeDef",
     {
         "RecordDelimiter": str,
     },
     total=False,
 )
 
+LifecycleExpirationOutputTypeDef = TypedDict(
+    "LifecycleExpirationOutputTypeDef",
+    {
+        "Date": datetime,
+        "Days": int,
+        "ExpiredObjectDeleteMarker": bool,
+    },
+)
+
 LifecycleExpirationTypeDef = TypedDict(
     "LifecycleExpirationTypeDef",
     {
-        "Date": datetime,
+        "Date": Union[datetime, str],
         "Days": int,
         "ExpiredObjectDeleteMarker": bool,
     },
+    total=False,
+)
+
+NoncurrentVersionExpirationOutputTypeDef = TypedDict(
+    "NoncurrentVersionExpirationOutputTypeDef",
+    {
+        "NoncurrentDays": int,
+        "NewerNoncurrentVersions": int,
+    },
+)
+
+NoncurrentVersionTransitionOutputTypeDef = TypedDict(
+    "NoncurrentVersionTransitionOutputTypeDef",
+    {
+        "NoncurrentDays": int,
+        "StorageClass": TransitionStorageClassType,
+        "NewerNoncurrentVersions": int,
+    },
+)
+
+TransitionOutputTypeDef = TypedDict(
+    "TransitionOutputTypeDef",
+    {
+        "Date": datetime,
+        "Days": int,
+        "StorageClass": TransitionStorageClassType,
+    },
 )
 
 NoncurrentVersionExpirationTypeDef = TypedDict(
     "NoncurrentVersionExpirationTypeDef",
     {
         "NoncurrentDays": int,
         "NewerNoncurrentVersions": int,
     },
+    total=False,
 )
 
 NoncurrentVersionTransitionTypeDef = TypedDict(
     "NoncurrentVersionTransitionTypeDef",
     {
         "NoncurrentDays": int,
         "StorageClass": TransitionStorageClassType,
         "NewerNoncurrentVersions": int,
     },
+    total=False,
 )
 
 TransitionTypeDef = TypedDict(
     "TransitionTypeDef",
     {
-        "Date": datetime,
+        "Date": Union[datetime, str],
         "Days": int,
         "StorageClass": TransitionStorageClassType,
     },
+    total=False,
 )
 
 _RequiredListBucketAnalyticsConfigurationsRequestRequestTypeDef = TypedDict(
     "_RequiredListBucketAnalyticsConfigurationsRequestRequestTypeDef",
     {
         "Bucket": str,
     },
@@ -3095,16 +3412,16 @@
 )
 
 class ListObjectsV2RequestRequestTypeDef(
     _RequiredListObjectsV2RequestRequestTypeDef, _OptionalListObjectsV2RequestRequestTypeDef
 ):
     pass
 
-PartTypeDef = TypedDict(
-    "PartTypeDef",
+PartOutputTypeDef = TypedDict(
+    "PartOutputTypeDef",
     {
         "PartNumber": int,
         "LastModified": datetime,
         "ETag": str,
         "Size": int,
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
@@ -3172,39 +3489,69 @@
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
+ReplicationTimeValueOutputTypeDef = TypedDict(
+    "ReplicationTimeValueOutputTypeDef",
+    {
+        "Minutes": int,
+    },
+)
+
 ReplicationTimeValueTypeDef = TypedDict(
     "ReplicationTimeValueTypeDef",
     {
         "Minutes": int,
     },
+    total=False,
+)
+
+QueueConfigurationDeprecatedOutputTypeDef = TypedDict(
+    "QueueConfigurationDeprecatedOutputTypeDef",
+    {
+        "Id": str,
+        "Event": EventType,
+        "Events": List[EventType],
+        "Queue": str,
+    },
+)
+
+TopicConfigurationDeprecatedOutputTypeDef = TypedDict(
+    "TopicConfigurationDeprecatedOutputTypeDef",
+    {
+        "Id": str,
+        "Events": List[EventType],
+        "Event": EventType,
+        "Topic": str,
+    },
 )
 
 QueueConfigurationDeprecatedTypeDef = TypedDict(
     "QueueConfigurationDeprecatedTypeDef",
     {
         "Id": str,
         "Event": EventType,
-        "Events": List[EventType],
+        "Events": Sequence[EventType],
         "Queue": str,
     },
+    total=False,
 )
 
 TopicConfigurationDeprecatedTypeDef = TypedDict(
     "TopicConfigurationDeprecatedTypeDef",
     {
         "Id": str,
-        "Events": List[EventType],
+        "Events": Sequence[EventType],
         "Event": EventType,
         "Topic": str,
     },
+    total=False,
 )
 
 _RequiredObjectDownloadFileRequestTypeDef = TypedDict(
     "_RequiredObjectDownloadFileRequestTypeDef",
     {
         "Filename": str,
     },
@@ -3241,16 +3588,33 @@
 )
 
 class ObjectDownloadFileobjRequestTypeDef(
     _RequiredObjectDownloadFileobjRequestTypeDef, _OptionalObjectDownloadFileobjRequestTypeDef
 ):
     pass
 
-RestoreStatusTypeDef = TypedDict(
-    "RestoreStatusTypeDef",
+ObjectLockLegalHoldTypeDef = TypedDict(
+    "ObjectLockLegalHoldTypeDef",
+    {
+        "Status": ObjectLockLegalHoldStatusType,
+    },
+    total=False,
+)
+
+ObjectLockRetentionTypeDef = TypedDict(
+    "ObjectLockRetentionTypeDef",
+    {
+        "Mode": ObjectLockRetentionModeType,
+        "RetainUntilDate": Union[datetime, str],
+    },
+    total=False,
+)
+
+RestoreStatusOutputTypeDef = TypedDict(
+    "RestoreStatusOutputTypeDef",
     {
         "IsRestoreInProgress": bool,
         "RestoreExpiryDate": datetime,
     },
 )
 
 _RequiredObjectUploadFileRequestTypeDef = TypedDict(
@@ -3300,14 +3664,21 @@
     {
         "DisplayName": str,
         "ID": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+OwnershipControlsRuleOutputTypeDef = TypedDict(
+    "OwnershipControlsRuleOutputTypeDef",
+    {
+        "ObjectOwnership": ObjectOwnershipType,
+    },
+)
+
 OwnershipControlsRuleTypeDef = TypedDict(
     "OwnershipControlsRuleTypeDef",
     {
         "ObjectOwnership": ObjectOwnershipType,
     },
 )
 
@@ -3317,23 +3688,34 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-ProgressTypeDef = TypedDict(
-    "ProgressTypeDef",
+ProgressOutputTypeDef = TypedDict(
+    "ProgressOutputTypeDef",
     {
         "BytesScanned": int,
         "BytesProcessed": int,
         "BytesReturned": int,
     },
 )
 
+PublicAccessBlockConfigurationTypeDef = TypedDict(
+    "PublicAccessBlockConfigurationTypeDef",
+    {
+        "BlockPublicAcls": bool,
+        "IgnorePublicAcls": bool,
+        "BlockPublicPolicy": bool,
+        "RestrictPublicBuckets": bool,
+    },
+    total=False,
+)
+
 _RequiredPutBucketPolicyRequestBucketPolicyPutTypeDef = TypedDict(
     "_RequiredPutBucketPolicyRequestBucketPolicyPutTypeDef",
     {
         "Policy": str,
     },
 )
 _OptionalPutBucketPolicyRequestBucketPolicyPutTypeDef = TypedDict(
@@ -3406,40 +3788,40 @@
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "MFA": str,
         "ExpectedBucketOwner": str,
     },
     total=False,
 )
 
-PutObjectAclOutputTypeDef = TypedDict(
-    "PutObjectAclOutputTypeDef",
+PutObjectAclOutputOutputTypeDef = TypedDict(
+    "PutObjectAclOutputOutputTypeDef",
     {
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutObjectLegalHoldOutputTypeDef = TypedDict(
-    "PutObjectLegalHoldOutputTypeDef",
+PutObjectLegalHoldOutputOutputTypeDef = TypedDict(
+    "PutObjectLegalHoldOutputOutputTypeDef",
     {
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutObjectLockConfigurationOutputTypeDef = TypedDict(
-    "PutObjectLockConfigurationOutputTypeDef",
+PutObjectLockConfigurationOutputOutputTypeDef = TypedDict(
+    "PutObjectLockConfigurationOutputOutputTypeDef",
     {
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutObjectOutputTypeDef = TypedDict(
-    "PutObjectOutputTypeDef",
+PutObjectOutputOutputTypeDef = TypedDict(
+    "PutObjectOutputOutputTypeDef",
     {
         "Expiration": str,
         "ETag": str,
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
         "ChecksumSHA256": str,
@@ -3642,55 +4024,93 @@
 )
 
 class PutObjectRequestRequestTypeDef(
     _RequiredPutObjectRequestRequestTypeDef, _OptionalPutObjectRequestRequestTypeDef
 ):
     pass
 
-PutObjectRetentionOutputTypeDef = TypedDict(
-    "PutObjectRetentionOutputTypeDef",
+PutObjectRetentionOutputOutputTypeDef = TypedDict(
+    "PutObjectRetentionOutputOutputTypeDef",
     {
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutObjectTaggingOutputTypeDef = TypedDict(
-    "PutObjectTaggingOutputTypeDef",
+PutObjectTaggingOutputOutputTypeDef = TypedDict(
+    "PutObjectTaggingOutputOutputTypeDef",
     {
         "VersionId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RecordsEventTypeDef = TypedDict(
-    "RecordsEventTypeDef",
+RecordsEventOutputTypeDef = TypedDict(
+    "RecordsEventOutputTypeDef",
     {
         "Payload": bytes,
     },
 )
 
 RedirectAllRequestsToResponseMetadataTypeDef = TypedDict(
     "RedirectAllRequestsToResponseMetadataTypeDef",
     {
         "HostName": str,
         "Protocol": ProtocolType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredRedirectAllRequestsToTypeDef = TypedDict(
+    "_RequiredRedirectAllRequestsToTypeDef",
+    {
+        "HostName": str,
+    },
+)
+_OptionalRedirectAllRequestsToTypeDef = TypedDict(
+    "_OptionalRedirectAllRequestsToTypeDef",
+    {
+        "Protocol": ProtocolType,
+    },
+    total=False,
+)
+
+class RedirectAllRequestsToTypeDef(
+    _RequiredRedirectAllRequestsToTypeDef, _OptionalRedirectAllRequestsToTypeDef
+):
+    pass
+
+RedirectOutputTypeDef = TypedDict(
+    "RedirectOutputTypeDef",
+    {
+        "HostName": str,
+        "HttpRedirectCode": str,
+        "Protocol": ProtocolType,
+        "ReplaceKeyPrefixWith": str,
+        "ReplaceKeyWith": str,
+    },
+)
+
 RedirectTypeDef = TypedDict(
     "RedirectTypeDef",
     {
         "HostName": str,
         "HttpRedirectCode": str,
         "Protocol": ProtocolType,
         "ReplaceKeyPrefixWith": str,
         "ReplaceKeyWith": str,
     },
+    total=False,
+)
+
+ReplicaModificationsOutputTypeDef = TypedDict(
+    "ReplicaModificationsOutputTypeDef",
+    {
+        "Status": ReplicaModificationsStatusType,
+    },
 )
 
 ReplicaModificationsTypeDef = TypedDict(
     "ReplicaModificationsTypeDef",
     {
         "Status": ReplicaModificationsStatusType,
     },
@@ -3711,16 +4131,16 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-RestoreObjectOutputTypeDef = TypedDict(
-    "RestoreObjectOutputTypeDef",
+RestoreObjectOutputOutputTypeDef = TypedDict(
+    "RestoreObjectOutputOutputTypeDef",
     {
         "RequestCharged": Literal["requester"],
         "RestoreOutputPath": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -3738,40 +4158,66 @@
     {
         "Start": int,
         "End": int,
     },
     total=False,
 )
 
-ServerSideEncryptionByDefaultTypeDef = TypedDict(
-    "ServerSideEncryptionByDefaultTypeDef",
+ServerSideEncryptionByDefaultOutputTypeDef = TypedDict(
+    "ServerSideEncryptionByDefaultOutputTypeDef",
+    {
+        "SSEAlgorithm": ServerSideEncryptionType,
+        "KMSMasterKeyID": str,
+    },
+)
+
+_RequiredServerSideEncryptionByDefaultTypeDef = TypedDict(
+    "_RequiredServerSideEncryptionByDefaultTypeDef",
     {
         "SSEAlgorithm": ServerSideEncryptionType,
+    },
+)
+_OptionalServerSideEncryptionByDefaultTypeDef = TypedDict(
+    "_OptionalServerSideEncryptionByDefaultTypeDef",
+    {
         "KMSMasterKeyID": str,
     },
+    total=False,
+)
+
+class ServerSideEncryptionByDefaultTypeDef(
+    _RequiredServerSideEncryptionByDefaultTypeDef, _OptionalServerSideEncryptionByDefaultTypeDef
+):
+    pass
+
+SseKmsEncryptedObjectsOutputTypeDef = TypedDict(
+    "SseKmsEncryptedObjectsOutputTypeDef",
+    {
+        "Status": SseKmsEncryptedObjectsStatusType,
+    },
 )
 
 SseKmsEncryptedObjectsTypeDef = TypedDict(
     "SseKmsEncryptedObjectsTypeDef",
     {
         "Status": SseKmsEncryptedObjectsStatusType,
     },
 )
 
-StatsTypeDef = TypedDict(
-    "StatsTypeDef",
+StatsOutputTypeDef = TypedDict(
+    "StatsOutputTypeDef",
     {
         "BytesScanned": int,
         "BytesProcessed": int,
         "BytesReturned": int,
     },
 )
 
-UploadPartOutputTypeDef = TypedDict(
-    "UploadPartOutputTypeDef",
+UploadPartOutputOutputTypeDef = TypedDict(
+    "UploadPartOutputOutputTypeDef",
     {
         "ServerSideEncryption": ServerSideEncryptionType,
         "ETag": str,
         "ChecksumCRC32": str,
         "ChecksumCRC32C": str,
         "ChecksumSHA1": str,
         "ChecksumSHA256": str,
@@ -3914,92 +4360,136 @@
 
 class PutBucketAccelerateConfigurationRequestRequestTypeDef(
     _RequiredPutBucketAccelerateConfigurationRequestRequestTypeDef,
     _OptionalPutBucketAccelerateConfigurationRequestRequestTypeDef,
 ):
     pass
 
-DeleteMarkerEntryTypeDef = TypedDict(
-    "DeleteMarkerEntryTypeDef",
+AnalyticsAndOperatorOutputTypeDef = TypedDict(
+    "AnalyticsAndOperatorOutputTypeDef",
+    {
+        "Prefix": str,
+        "Tags": List[TagOutputTypeDef],
+    },
+)
+
+GetBucketTaggingOutputOutputTypeDef = TypedDict(
+    "GetBucketTaggingOutputOutputTypeDef",
+    {
+        "TagSet": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetObjectTaggingOutputOutputTypeDef = TypedDict(
+    "GetObjectTaggingOutputOutputTypeDef",
     {
-        "Owner": OwnerTypeDef,
-        "Key": str,
         "VersionId": str,
-        "IsLatest": bool,
-        "LastModified": datetime,
+        "TagSet": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-AnalyticsAndOperatorTypeDef = TypedDict(
-    "AnalyticsAndOperatorTypeDef",
+IntelligentTieringAndOperatorOutputTypeDef = TypedDict(
+    "IntelligentTieringAndOperatorOutputTypeDef",
     {
         "Prefix": str,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
     },
 )
 
-GetBucketTaggingOutputTypeDef = TypedDict(
-    "GetBucketTaggingOutputTypeDef",
+LifecycleRuleAndOperatorOutputTypeDef = TypedDict(
+    "LifecycleRuleAndOperatorOutputTypeDef",
     {
-        "TagSet": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Prefix": str,
+        "Tags": List[TagOutputTypeDef],
+        "ObjectSizeGreaterThan": int,
+        "ObjectSizeLessThan": int,
     },
 )
 
-GetObjectTaggingOutputTypeDef = TypedDict(
-    "GetObjectTaggingOutputTypeDef",
+MetricsAndOperatorOutputTypeDef = TypedDict(
+    "MetricsAndOperatorOutputTypeDef",
     {
-        "VersionId": str,
-        "TagSet": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Prefix": str,
+        "Tags": List[TagOutputTypeDef],
+        "AccessPointArn": str,
+    },
+)
+
+ReplicationRuleAndOperatorOutputTypeDef = TypedDict(
+    "ReplicationRuleAndOperatorOutputTypeDef",
+    {
+        "Prefix": str,
+        "Tags": List[TagOutputTypeDef],
+    },
+)
+
+AnalyticsAndOperatorTypeDef = TypedDict(
+    "AnalyticsAndOperatorTypeDef",
+    {
+        "Prefix": str,
+        "Tags": Sequence[TagTypeDef],
     },
+    total=False,
 )
 
 IntelligentTieringAndOperatorTypeDef = TypedDict(
     "IntelligentTieringAndOperatorTypeDef",
     {
         "Prefix": str,
-        "Tags": List[TagTypeDef],
+        "Tags": Sequence[TagTypeDef],
     },
+    total=False,
 )
 
 LifecycleRuleAndOperatorTypeDef = TypedDict(
     "LifecycleRuleAndOperatorTypeDef",
     {
         "Prefix": str,
-        "Tags": List[TagTypeDef],
+        "Tags": Sequence[TagTypeDef],
         "ObjectSizeGreaterThan": int,
         "ObjectSizeLessThan": int,
     },
+    total=False,
 )
 
 MetricsAndOperatorTypeDef = TypedDict(
     "MetricsAndOperatorTypeDef",
     {
         "Prefix": str,
-        "Tags": List[TagTypeDef],
+        "Tags": Sequence[TagTypeDef],
         "AccessPointArn": str,
     },
+    total=False,
 )
 
 ReplicationRuleAndOperatorTypeDef = TypedDict(
     "ReplicationRuleAndOperatorTypeDef",
     {
         "Prefix": str,
-        "Tags": List[TagTypeDef],
+        "Tags": Sequence[TagTypeDef],
     },
+    total=False,
 )
 
 TaggingTypeDef = TypedDict(
     "TaggingTypeDef",
     {
         "TagSet": Sequence[TagTypeDef],
     },
 )
 
+AnalyticsExportDestinationOutputTypeDef = TypedDict(
+    "AnalyticsExportDestinationOutputTypeDef",
+    {
+        "S3BucketDestination": AnalyticsS3BucketDestinationOutputTypeDef,
+    },
+)
+
 AnalyticsExportDestinationTypeDef = TypedDict(
     "AnalyticsExportDestinationTypeDef",
     {
         "S3BucketDestination": AnalyticsS3BucketDestinationTypeDef,
     },
 )
 
@@ -4195,69 +4685,60 @@
 )
 
 class UploadPartCopyRequestRequestTypeDef(
     _RequiredUploadPartCopyRequestRequestTypeDef, _OptionalUploadPartCopyRequestRequestTypeDef
 ):
     pass
 
-ListBucketsOutputTypeDef = TypedDict(
-    "ListBucketsOutputTypeDef",
-    {
-        "Buckets": List[BucketTypeDef],
-        "Owner": OwnerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CORSConfigurationTypeDef = TypedDict(
     "CORSConfigurationTypeDef",
     {
         "CORSRules": Sequence[CORSRuleTypeDef],
     },
 )
 
-GetBucketCorsOutputTypeDef = TypedDict(
-    "GetBucketCorsOutputTypeDef",
+GetBucketCorsOutputOutputTypeDef = TypedDict(
+    "GetBucketCorsOutputOutputTypeDef",
     {
-        "CORSRules": List[CORSRuleTypeDef],
+        "CORSRules": List[CORSRuleOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CompletedMultipartUploadTypeDef = TypedDict(
     "CompletedMultipartUploadTypeDef",
     {
         "Parts": Sequence[CompletedPartTypeDef],
     },
     total=False,
 )
 
-CopyObjectOutputTypeDef = TypedDict(
-    "CopyObjectOutputTypeDef",
+CopyObjectOutputOutputTypeDef = TypedDict(
+    "CopyObjectOutputOutputTypeDef",
     {
-        "CopyObjectResult": CopyObjectResultTypeDef,
+        "CopyObjectResult": CopyObjectResultOutputTypeDef,
         "Expiration": str,
         "CopySourceVersionId": str,
         "VersionId": str,
         "ServerSideEncryption": ServerSideEncryptionType,
         "SSECustomerAlgorithm": str,
         "SSECustomerKeyMD5": str,
         "SSEKMSKeyId": str,
         "SSEKMSEncryptionContext": str,
         "BucketKeyEnabled": bool,
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UploadPartCopyOutputTypeDef = TypedDict(
-    "UploadPartCopyOutputTypeDef",
+UploadPartCopyOutputOutputTypeDef = TypedDict(
+    "UploadPartCopyOutputOutputTypeDef",
     {
         "CopySourceVersionId": str,
-        "CopyPartResult": CopyPartResultTypeDef,
+        "CopyPartResult": CopyPartResultOutputTypeDef,
         "ServerSideEncryption": ServerSideEncryptionType,
         "SSECustomerAlgorithm": str,
         "SSECustomerKeyMD5": str,
         "SSEKMSKeyId": str,
         "BucketKeyEnabled": bool,
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -4331,27 +4812,55 @@
 
 class CreateBucketRequestServiceResourceCreateBucketTypeDef(
     _RequiredCreateBucketRequestServiceResourceCreateBucketTypeDef,
     _OptionalCreateBucketRequestServiceResourceCreateBucketTypeDef,
 ):
     pass
 
+ObjectLockRuleOutputTypeDef = TypedDict(
+    "ObjectLockRuleOutputTypeDef",
+    {
+        "DefaultRetention": DefaultRetentionOutputTypeDef,
+    },
+)
+
 ObjectLockRuleTypeDef = TypedDict(
     "ObjectLockRuleTypeDef",
     {
         "DefaultRetention": DefaultRetentionTypeDef,
     },
+    total=False,
 )
 
-DeleteObjectsOutputTypeDef = TypedDict(
-    "DeleteObjectsOutputTypeDef",
+DeleteMarkerEntryOutputTypeDef = TypedDict(
+    "DeleteMarkerEntryOutputTypeDef",
     {
-        "Deleted": List[DeletedObjectTypeDef],
+        "Owner": OwnerOutputTypeDef,
+        "Key": str,
+        "VersionId": str,
+        "IsLatest": bool,
+        "LastModified": datetime,
+    },
+)
+
+ListBucketsOutputOutputTypeDef = TypedDict(
+    "ListBucketsOutputOutputTypeDef",
+    {
+        "Buckets": List[BucketOutputTypeDef],
+        "Owner": OwnerOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DeleteObjectsOutputOutputTypeDef = TypedDict(
+    "DeleteObjectsOutputOutputTypeDef",
+    {
+        "Deleted": List[DeletedObjectOutputTypeDef],
         "RequestCharged": Literal["requester"],
-        "Errors": List[ErrorTypeDef],
+        "Errors": List[ErrorOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDeleteTypeDef = TypedDict(
     "_RequiredDeleteTypeDef",
     {
@@ -4365,155 +4874,105 @@
     },
     total=False,
 )
 
 class DeleteTypeDef(_RequiredDeleteTypeDef, _OptionalDeleteTypeDef):
     pass
 
+S3KeyFilterOutputTypeDef = TypedDict(
+    "S3KeyFilterOutputTypeDef",
+    {
+        "FilterRules": List[FilterRuleOutputTypeDef],
+    },
+)
+
 S3KeyFilterTypeDef = TypedDict(
     "S3KeyFilterTypeDef",
     {
-        "FilterRules": List[FilterRuleTypeDef],
+        "FilterRules": Sequence[FilterRuleTypeDef],
     },
+    total=False,
 )
 
-GetBucketPolicyStatusOutputTypeDef = TypedDict(
-    "GetBucketPolicyStatusOutputTypeDef",
+GetBucketPolicyStatusOutputOutputTypeDef = TypedDict(
+    "GetBucketPolicyStatusOutputOutputTypeDef",
     {
-        "PolicyStatus": PolicyStatusTypeDef,
+        "PolicyStatus": PolicyStatusOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetObjectAttributesPartsTypeDef = TypedDict(
-    "GetObjectAttributesPartsTypeDef",
+GetObjectAttributesPartsOutputTypeDef = TypedDict(
+    "GetObjectAttributesPartsOutputTypeDef",
     {
         "TotalPartsCount": int,
         "PartNumberMarker": int,
         "NextPartNumberMarker": int,
         "MaxParts": int,
         "IsTruncated": bool,
-        "Parts": List[ObjectPartTypeDef],
+        "Parts": List[ObjectPartOutputTypeDef],
     },
 )
 
-GetObjectLegalHoldOutputTypeDef = TypedDict(
-    "GetObjectLegalHoldOutputTypeDef",
+GetObjectLegalHoldOutputOutputTypeDef = TypedDict(
+    "GetObjectLegalHoldOutputOutputTypeDef",
     {
-        "LegalHold": ObjectLockLegalHoldTypeDef,
+        "LegalHold": ObjectLockLegalHoldOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredPutObjectLegalHoldRequestRequestTypeDef = TypedDict(
-    "_RequiredPutObjectLegalHoldRequestRequestTypeDef",
-    {
-        "Bucket": str,
-        "Key": str,
-    },
-)
-_OptionalPutObjectLegalHoldRequestRequestTypeDef = TypedDict(
-    "_OptionalPutObjectLegalHoldRequestRequestTypeDef",
-    {
-        "LegalHold": ObjectLockLegalHoldTypeDef,
-        "RequestPayer": Literal["requester"],
-        "VersionId": str,
-        "ContentMD5": str,
-        "ChecksumAlgorithm": ChecksumAlgorithmType,
-        "ExpectedBucketOwner": str,
-    },
-    total=False,
-)
-
-class PutObjectLegalHoldRequestRequestTypeDef(
-    _RequiredPutObjectLegalHoldRequestRequestTypeDef,
-    _OptionalPutObjectLegalHoldRequestRequestTypeDef,
-):
-    pass
-
-GetObjectRetentionOutputTypeDef = TypedDict(
-    "GetObjectRetentionOutputTypeDef",
+GetObjectRetentionOutputOutputTypeDef = TypedDict(
+    "GetObjectRetentionOutputOutputTypeDef",
     {
-        "Retention": ObjectLockRetentionTypeDef,
+        "Retention": ObjectLockRetentionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredPutObjectRetentionRequestRequestTypeDef = TypedDict(
-    "_RequiredPutObjectRetentionRequestRequestTypeDef",
-    {
-        "Bucket": str,
-        "Key": str,
-    },
-)
-_OptionalPutObjectRetentionRequestRequestTypeDef = TypedDict(
-    "_OptionalPutObjectRetentionRequestRequestTypeDef",
+GetPublicAccessBlockOutputOutputTypeDef = TypedDict(
+    "GetPublicAccessBlockOutputOutputTypeDef",
     {
-        "Retention": ObjectLockRetentionTypeDef,
-        "RequestPayer": Literal["requester"],
-        "VersionId": str,
-        "BypassGovernanceRetention": bool,
-        "ContentMD5": str,
-        "ChecksumAlgorithm": ChecksumAlgorithmType,
-        "ExpectedBucketOwner": str,
-    },
-    total=False,
-)
-
-class PutObjectRetentionRequestRequestTypeDef(
-    _RequiredPutObjectRetentionRequestRequestTypeDef,
-    _OptionalPutObjectRetentionRequestRequestTypeDef,
-):
-    pass
-
-GetPublicAccessBlockOutputTypeDef = TypedDict(
-    "GetPublicAccessBlockOutputTypeDef",
-    {
-        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
+        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredPutPublicAccessBlockRequestRequestTypeDef = TypedDict(
-    "_RequiredPutPublicAccessBlockRequestRequestTypeDef",
+GrantOutputTypeDef = TypedDict(
+    "GrantOutputTypeDef",
     {
-        "Bucket": str,
-        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
+        "Grantee": GranteeOutputTypeDef,
+        "Permission": PermissionType,
     },
 )
-_OptionalPutPublicAccessBlockRequestRequestTypeDef = TypedDict(
-    "_OptionalPutPublicAccessBlockRequestRequestTypeDef",
+
+TargetGrantOutputTypeDef = TypedDict(
+    "TargetGrantOutputTypeDef",
     {
-        "ContentMD5": str,
-        "ChecksumAlgorithm": ChecksumAlgorithmType,
-        "ExpectedBucketOwner": str,
+        "Grantee": GranteeOutputTypeDef,
+        "Permission": BucketLogsPermissionType,
     },
-    total=False,
 )
 
-class PutPublicAccessBlockRequestRequestTypeDef(
-    _RequiredPutPublicAccessBlockRequestRequestTypeDef,
-    _OptionalPutPublicAccessBlockRequestRequestTypeDef,
-):
-    pass
-
 GrantTypeDef = TypedDict(
     "GrantTypeDef",
     {
         "Grantee": GranteeTypeDef,
         "Permission": PermissionType,
     },
+    total=False,
 )
 
 TargetGrantTypeDef = TypedDict(
     "TargetGrantTypeDef",
     {
         "Grantee": GranteeTypeDef,
         "Permission": BucketLogsPermissionType,
     },
+    total=False,
 )
 
 _RequiredHeadBucketRequestBucketExistsWaitTypeDef = TypedDict(
     "_RequiredHeadBucketRequestBucketExistsWaitTypeDef",
     {
         "Bucket": str,
     },
@@ -4618,23 +5077,23 @@
 
 class HeadObjectRequestObjectNotExistsWaitTypeDef(
     _RequiredHeadObjectRequestObjectNotExistsWaitTypeDef,
     _OptionalHeadObjectRequestObjectNotExistsWaitTypeDef,
 ):
     pass
 
-MultipartUploadTypeDef = TypedDict(
-    "MultipartUploadTypeDef",
+MultipartUploadOutputTypeDef = TypedDict(
+    "MultipartUploadOutputTypeDef",
     {
         "UploadId": str,
         "Key": str,
         "Initiated": datetime,
         "StorageClass": StorageClassType,
-        "Owner": OwnerTypeDef,
-        "Initiator": InitiatorTypeDef,
+        "Owner": OwnerOutputTypeDef,
+        "Initiator": InitiatorOutputTypeDef,
         "ChecksumAlgorithm": ChecksumAlgorithmType,
     },
 )
 
 InputSerializationTypeDef = TypedDict(
     "InputSerializationTypeDef",
     {
@@ -4642,147 +5101,287 @@
         "CompressionType": CompressionTypeType,
         "JSON": JSONInputTypeDef,
         "Parquet": Mapping[str, Any],
     },
     total=False,
 )
 
+InventoryEncryptionOutputTypeDef = TypedDict(
+    "InventoryEncryptionOutputTypeDef",
+    {
+        "SSES3": Dict[str, Any],
+        "SSEKMS": SSEKMSOutputTypeDef,
+    },
+)
+
 InventoryEncryptionTypeDef = TypedDict(
     "InventoryEncryptionTypeDef",
     {
-        "SSES3": Dict[str, Any],
+        "SSES3": Mapping[str, Any],
         "SSEKMS": SSEKMSTypeDef,
     },
+    total=False,
 )
 
 OutputSerializationTypeDef = TypedDict(
     "OutputSerializationTypeDef",
     {
         "CSV": CSVOutputTypeDef,
         "JSON": JSONOutputTypeDef,
     },
     total=False,
 )
 
-RuleTypeDef = TypedDict(
-    "RuleTypeDef",
+RuleOutputTypeDef = TypedDict(
+    "RuleOutputTypeDef",
     {
-        "Expiration": LifecycleExpirationTypeDef,
+        "Expiration": LifecycleExpirationOutputTypeDef,
         "ID": str,
         "Prefix": str,
         "Status": ExpirationStatusType,
+        "Transition": TransitionOutputTypeDef,
+        "NoncurrentVersionTransition": NoncurrentVersionTransitionOutputTypeDef,
+        "NoncurrentVersionExpiration": NoncurrentVersionExpirationOutputTypeDef,
+        "AbortIncompleteMultipartUpload": AbortIncompleteMultipartUploadOutputTypeDef,
+    },
+)
+
+_RequiredRuleTypeDef = TypedDict(
+    "_RequiredRuleTypeDef",
+    {
+        "Prefix": str,
+        "Status": ExpirationStatusType,
+    },
+)
+_OptionalRuleTypeDef = TypedDict(
+    "_OptionalRuleTypeDef",
+    {
+        "Expiration": LifecycleExpirationTypeDef,
+        "ID": str,
         "Transition": TransitionTypeDef,
         "NoncurrentVersionTransition": NoncurrentVersionTransitionTypeDef,
         "NoncurrentVersionExpiration": NoncurrentVersionExpirationTypeDef,
         "AbortIncompleteMultipartUpload": AbortIncompleteMultipartUploadTypeDef,
     },
+    total=False,
 )
 
-ListPartsOutputTypeDef = TypedDict(
-    "ListPartsOutputTypeDef",
+class RuleTypeDef(_RequiredRuleTypeDef, _OptionalRuleTypeDef):
+    pass
+
+ListPartsOutputOutputTypeDef = TypedDict(
+    "ListPartsOutputOutputTypeDef",
     {
         "AbortDate": datetime,
         "AbortRuleId": str,
         "Bucket": str,
         "Key": str,
         "UploadId": str,
         "PartNumberMarker": int,
         "NextPartNumberMarker": int,
         "MaxParts": int,
         "IsTruncated": bool,
-        "Parts": List[PartTypeDef],
-        "Initiator": InitiatorTypeDef,
-        "Owner": OwnerTypeDef,
+        "Parts": List[PartOutputTypeDef],
+        "Initiator": InitiatorOutputTypeDef,
+        "Owner": OwnerOutputTypeDef,
         "StorageClass": StorageClassType,
         "RequestCharged": Literal["requester"],
         "ChecksumAlgorithm": ChecksumAlgorithmType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-MetricsTypeDef = TypedDict(
-    "MetricsTypeDef",
+MetricsOutputTypeDef = TypedDict(
+    "MetricsOutputTypeDef",
     {
         "Status": MetricsStatusType,
+        "EventThreshold": ReplicationTimeValueOutputTypeDef,
+    },
+)
+
+ReplicationTimeOutputTypeDef = TypedDict(
+    "ReplicationTimeOutputTypeDef",
+    {
+        "Status": ReplicationTimeStatusType,
+        "Time": ReplicationTimeValueOutputTypeDef,
+    },
+)
+
+_RequiredMetricsTypeDef = TypedDict(
+    "_RequiredMetricsTypeDef",
+    {
+        "Status": MetricsStatusType,
+    },
+)
+_OptionalMetricsTypeDef = TypedDict(
+    "_OptionalMetricsTypeDef",
+    {
         "EventThreshold": ReplicationTimeValueTypeDef,
     },
+    total=False,
 )
 
+class MetricsTypeDef(_RequiredMetricsTypeDef, _OptionalMetricsTypeDef):
+    pass
+
 ReplicationTimeTypeDef = TypedDict(
     "ReplicationTimeTypeDef",
     {
         "Status": ReplicationTimeStatusType,
         "Time": ReplicationTimeValueTypeDef,
     },
 )
 
-NotificationConfigurationDeprecatedResponseMetadataTypeDef = TypedDict(
-    "NotificationConfigurationDeprecatedResponseMetadataTypeDef",
+NotificationConfigurationDeprecatedOutputTypeDef = TypedDict(
+    "NotificationConfigurationDeprecatedOutputTypeDef",
     {
-        "TopicConfiguration": TopicConfigurationDeprecatedTypeDef,
-        "QueueConfiguration": QueueConfigurationDeprecatedTypeDef,
-        "CloudFunctionConfiguration": CloudFunctionConfigurationTypeDef,
+        "TopicConfiguration": TopicConfigurationDeprecatedOutputTypeDef,
+        "QueueConfiguration": QueueConfigurationDeprecatedOutputTypeDef,
+        "CloudFunctionConfiguration": CloudFunctionConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 NotificationConfigurationDeprecatedTypeDef = TypedDict(
     "NotificationConfigurationDeprecatedTypeDef",
     {
         "TopicConfiguration": TopicConfigurationDeprecatedTypeDef,
         "QueueConfiguration": QueueConfigurationDeprecatedTypeDef,
         "CloudFunctionConfiguration": CloudFunctionConfigurationTypeDef,
     },
     total=False,
 )
 
-ObjectTypeDef = TypedDict(
-    "ObjectTypeDef",
+_RequiredPutObjectLegalHoldRequestRequestTypeDef = TypedDict(
+    "_RequiredPutObjectLegalHoldRequestRequestTypeDef",
+    {
+        "Bucket": str,
+        "Key": str,
+    },
+)
+_OptionalPutObjectLegalHoldRequestRequestTypeDef = TypedDict(
+    "_OptionalPutObjectLegalHoldRequestRequestTypeDef",
+    {
+        "LegalHold": ObjectLockLegalHoldTypeDef,
+        "RequestPayer": Literal["requester"],
+        "VersionId": str,
+        "ContentMD5": str,
+        "ChecksumAlgorithm": ChecksumAlgorithmType,
+        "ExpectedBucketOwner": str,
+    },
+    total=False,
+)
+
+class PutObjectLegalHoldRequestRequestTypeDef(
+    _RequiredPutObjectLegalHoldRequestRequestTypeDef,
+    _OptionalPutObjectLegalHoldRequestRequestTypeDef,
+):
+    pass
+
+_RequiredPutObjectRetentionRequestRequestTypeDef = TypedDict(
+    "_RequiredPutObjectRetentionRequestRequestTypeDef",
+    {
+        "Bucket": str,
+        "Key": str,
+    },
+)
+_OptionalPutObjectRetentionRequestRequestTypeDef = TypedDict(
+    "_OptionalPutObjectRetentionRequestRequestTypeDef",
+    {
+        "Retention": ObjectLockRetentionTypeDef,
+        "RequestPayer": Literal["requester"],
+        "VersionId": str,
+        "BypassGovernanceRetention": bool,
+        "ContentMD5": str,
+        "ChecksumAlgorithm": ChecksumAlgorithmType,
+        "ExpectedBucketOwner": str,
+    },
+    total=False,
+)
+
+class PutObjectRetentionRequestRequestTypeDef(
+    _RequiredPutObjectRetentionRequestRequestTypeDef,
+    _OptionalPutObjectRetentionRequestRequestTypeDef,
+):
+    pass
+
+ObjectOutputTypeDef = TypedDict(
+    "ObjectOutputTypeDef",
     {
         "Key": str,
         "LastModified": datetime,
         "ETag": str,
         "ChecksumAlgorithm": List[ChecksumAlgorithmType],
         "Size": int,
         "StorageClass": ObjectStorageClassType,
-        "Owner": OwnerTypeDef,
-        "RestoreStatus": RestoreStatusTypeDef,
+        "Owner": OwnerOutputTypeDef,
+        "RestoreStatus": RestoreStatusOutputTypeDef,
     },
 )
 
-ObjectVersionTypeDef = TypedDict(
-    "ObjectVersionTypeDef",
+ObjectVersionOutputTypeDef = TypedDict(
+    "ObjectVersionOutputTypeDef",
     {
         "ETag": str,
         "ChecksumAlgorithm": List[ChecksumAlgorithmType],
         "Size": int,
         "StorageClass": Literal["STANDARD"],
         "Key": str,
         "VersionId": str,
         "IsLatest": bool,
         "LastModified": datetime,
-        "Owner": OwnerTypeDef,
-        "RestoreStatus": RestoreStatusTypeDef,
+        "Owner": OwnerOutputTypeDef,
+        "RestoreStatus": RestoreStatusOutputTypeDef,
+    },
+)
+
+OwnershipControlsOutputTypeDef = TypedDict(
+    "OwnershipControlsOutputTypeDef",
+    {
+        "Rules": List[OwnershipControlsRuleOutputTypeDef],
     },
 )
 
 OwnershipControlsTypeDef = TypedDict(
     "OwnershipControlsTypeDef",
     {
-        "Rules": List[OwnershipControlsRuleTypeDef],
+        "Rules": Sequence[OwnershipControlsRuleTypeDef],
     },
 )
 
-ProgressEventTypeDef = TypedDict(
-    "ProgressEventTypeDef",
+ProgressEventOutputTypeDef = TypedDict(
+    "ProgressEventOutputTypeDef",
+    {
+        "Details": ProgressOutputTypeDef,
+    },
+)
+
+_RequiredPutPublicAccessBlockRequestRequestTypeDef = TypedDict(
+    "_RequiredPutPublicAccessBlockRequestRequestTypeDef",
+    {
+        "Bucket": str,
+        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
+    },
+)
+_OptionalPutPublicAccessBlockRequestRequestTypeDef = TypedDict(
+    "_OptionalPutPublicAccessBlockRequestRequestTypeDef",
     {
-        "Details": ProgressTypeDef,
+        "ContentMD5": str,
+        "ChecksumAlgorithm": ChecksumAlgorithmType,
+        "ExpectedBucketOwner": str,
     },
+    total=False,
 )
 
+class PutPublicAccessBlockRequestRequestTypeDef(
+    _RequiredPutPublicAccessBlockRequestRequestTypeDef,
+    _OptionalPutPublicAccessBlockRequestRequestTypeDef,
+):
+    pass
+
 _RequiredPutBucketRequestPaymentRequestBucketRequestPaymentPutTypeDef = TypedDict(
     "_RequiredPutBucketRequestPaymentRequestBucketRequestPaymentPutTypeDef",
     {
         "RequestPaymentConfiguration": RequestPaymentConfigurationTypeDef,
     },
 )
 _OptionalPutBucketRequestPaymentRequestBucketRequestPaymentPutTypeDef = TypedDict(
@@ -4863,91 +5462,179 @@
 
 class PutBucketVersioningRequestRequestTypeDef(
     _RequiredPutBucketVersioningRequestRequestTypeDef,
     _OptionalPutBucketVersioningRequestRequestTypeDef,
 ):
     pass
 
-RoutingRuleTypeDef = TypedDict(
-    "RoutingRuleTypeDef",
+RoutingRuleOutputTypeDef = TypedDict(
+    "RoutingRuleOutputTypeDef",
+    {
+        "Condition": ConditionOutputTypeDef,
+        "Redirect": RedirectOutputTypeDef,
+    },
+)
+
+_RequiredRoutingRuleTypeDef = TypedDict(
+    "_RequiredRoutingRuleTypeDef",
     {
-        "Condition": ConditionTypeDef,
         "Redirect": RedirectTypeDef,
     },
 )
+_OptionalRoutingRuleTypeDef = TypedDict(
+    "_OptionalRoutingRuleTypeDef",
+    {
+        "Condition": ConditionTypeDef,
+    },
+    total=False,
+)
+
+class RoutingRuleTypeDef(_RequiredRoutingRuleTypeDef, _OptionalRoutingRuleTypeDef):
+    pass
+
+ServerSideEncryptionRuleOutputTypeDef = TypedDict(
+    "ServerSideEncryptionRuleOutputTypeDef",
+    {
+        "ApplyServerSideEncryptionByDefault": ServerSideEncryptionByDefaultOutputTypeDef,
+        "BucketKeyEnabled": bool,
+    },
+)
 
 ServerSideEncryptionRuleTypeDef = TypedDict(
     "ServerSideEncryptionRuleTypeDef",
     {
         "ApplyServerSideEncryptionByDefault": ServerSideEncryptionByDefaultTypeDef,
         "BucketKeyEnabled": bool,
     },
+    total=False,
+)
+
+SourceSelectionCriteriaOutputTypeDef = TypedDict(
+    "SourceSelectionCriteriaOutputTypeDef",
+    {
+        "SseKmsEncryptedObjects": SseKmsEncryptedObjectsOutputTypeDef,
+        "ReplicaModifications": ReplicaModificationsOutputTypeDef,
+    },
 )
 
 SourceSelectionCriteriaTypeDef = TypedDict(
     "SourceSelectionCriteriaTypeDef",
     {
         "SseKmsEncryptedObjects": SseKmsEncryptedObjectsTypeDef,
         "ReplicaModifications": ReplicaModificationsTypeDef,
     },
+    total=False,
+)
+
+StatsEventOutputTypeDef = TypedDict(
+    "StatsEventOutputTypeDef",
+    {
+        "Details": StatsOutputTypeDef,
+    },
+)
+
+AnalyticsFilterOutputTypeDef = TypedDict(
+    "AnalyticsFilterOutputTypeDef",
+    {
+        "Prefix": str,
+        "Tag": TagOutputTypeDef,
+        "And": AnalyticsAndOperatorOutputTypeDef,
+    },
+)
+
+IntelligentTieringFilterOutputTypeDef = TypedDict(
+    "IntelligentTieringFilterOutputTypeDef",
+    {
+        "Prefix": str,
+        "Tag": TagOutputTypeDef,
+        "And": IntelligentTieringAndOperatorOutputTypeDef,
+    },
+)
+
+LifecycleRuleFilterOutputTypeDef = TypedDict(
+    "LifecycleRuleFilterOutputTypeDef",
+    {
+        "Prefix": str,
+        "Tag": TagOutputTypeDef,
+        "ObjectSizeGreaterThan": int,
+        "ObjectSizeLessThan": int,
+        "And": LifecycleRuleAndOperatorOutputTypeDef,
+    },
+)
+
+MetricsFilterOutputTypeDef = TypedDict(
+    "MetricsFilterOutputTypeDef",
+    {
+        "Prefix": str,
+        "Tag": TagOutputTypeDef,
+        "AccessPointArn": str,
+        "And": MetricsAndOperatorOutputTypeDef,
+    },
 )
 
-StatsEventTypeDef = TypedDict(
-    "StatsEventTypeDef",
+ReplicationRuleFilterOutputTypeDef = TypedDict(
+    "ReplicationRuleFilterOutputTypeDef",
     {
-        "Details": StatsTypeDef,
+        "Prefix": str,
+        "Tag": TagOutputTypeDef,
+        "And": ReplicationRuleAndOperatorOutputTypeDef,
     },
 )
 
 AnalyticsFilterTypeDef = TypedDict(
     "AnalyticsFilterTypeDef",
     {
         "Prefix": str,
         "Tag": TagTypeDef,
         "And": AnalyticsAndOperatorTypeDef,
     },
+    total=False,
 )
 
 IntelligentTieringFilterTypeDef = TypedDict(
     "IntelligentTieringFilterTypeDef",
     {
         "Prefix": str,
         "Tag": TagTypeDef,
         "And": IntelligentTieringAndOperatorTypeDef,
     },
+    total=False,
 )
 
 LifecycleRuleFilterTypeDef = TypedDict(
     "LifecycleRuleFilterTypeDef",
     {
         "Prefix": str,
         "Tag": TagTypeDef,
         "ObjectSizeGreaterThan": int,
         "ObjectSizeLessThan": int,
         "And": LifecycleRuleAndOperatorTypeDef,
     },
+    total=False,
 )
 
 MetricsFilterTypeDef = TypedDict(
     "MetricsFilterTypeDef",
     {
         "Prefix": str,
         "Tag": TagTypeDef,
         "AccessPointArn": str,
         "And": MetricsAndOperatorTypeDef,
     },
+    total=False,
 )
 
 ReplicationRuleFilterTypeDef = TypedDict(
     "ReplicationRuleFilterTypeDef",
     {
         "Prefix": str,
         "Tag": TagTypeDef,
         "And": ReplicationRuleAndOperatorTypeDef,
     },
+    total=False,
 )
 
 _RequiredPutBucketTaggingRequestBucketTaggingPutTypeDef = TypedDict(
     "_RequiredPutBucketTaggingRequestBucketTaggingPutTypeDef",
     {
         "Tagging": TaggingTypeDef,
     },
@@ -5009,14 +5696,22 @@
 )
 
 class PutObjectTaggingRequestRequestTypeDef(
     _RequiredPutObjectTaggingRequestRequestTypeDef, _OptionalPutObjectTaggingRequestRequestTypeDef
 ):
     pass
 
+StorageClassAnalysisDataExportOutputTypeDef = TypedDict(
+    "StorageClassAnalysisDataExportOutputTypeDef",
+    {
+        "OutputSchemaVersion": Literal["V_1"],
+        "Destination": AnalyticsExportDestinationOutputTypeDef,
+    },
+)
+
 StorageClassAnalysisDataExportTypeDef = TypedDict(
     "StorageClassAnalysisDataExportTypeDef",
     {
         "OutputSchemaVersion": Literal["V_1"],
         "Destination": AnalyticsExportDestinationTypeDef,
     },
 )
@@ -5107,20 +5802,29 @@
 
 class CompleteMultipartUploadRequestRequestTypeDef(
     _RequiredCompleteMultipartUploadRequestRequestTypeDef,
     _OptionalCompleteMultipartUploadRequestRequestTypeDef,
 ):
     pass
 
+ObjectLockConfigurationOutputTypeDef = TypedDict(
+    "ObjectLockConfigurationOutputTypeDef",
+    {
+        "ObjectLockEnabled": Literal["Enabled"],
+        "Rule": ObjectLockRuleOutputTypeDef,
+    },
+)
+
 ObjectLockConfigurationTypeDef = TypedDict(
     "ObjectLockConfigurationTypeDef",
     {
         "ObjectLockEnabled": Literal["Enabled"],
         "Rule": ObjectLockRuleTypeDef,
     },
+    total=False,
 )
 
 _RequiredDeleteObjectsRequestBucketDeleteObjectsTypeDef = TypedDict(
     "_RequiredDeleteObjectsRequestBucketDeleteObjectsTypeDef",
     {
         "Delete": DeleteTypeDef,
     },
@@ -5163,65 +5867,92 @@
 )
 
 class DeleteObjectsRequestRequestTypeDef(
     _RequiredDeleteObjectsRequestRequestTypeDef, _OptionalDeleteObjectsRequestRequestTypeDef
 ):
     pass
 
+NotificationConfigurationFilterOutputTypeDef = TypedDict(
+    "NotificationConfigurationFilterOutputTypeDef",
+    {
+        "Key": S3KeyFilterOutputTypeDef,
+    },
+)
+
 NotificationConfigurationFilterTypeDef = TypedDict(
     "NotificationConfigurationFilterTypeDef",
     {
         "Key": S3KeyFilterTypeDef,
     },
+    total=False,
 )
 
-GetObjectAttributesOutputTypeDef = TypedDict(
-    "GetObjectAttributesOutputTypeDef",
+GetObjectAttributesOutputOutputTypeDef = TypedDict(
+    "GetObjectAttributesOutputOutputTypeDef",
     {
         "DeleteMarker": bool,
         "LastModified": datetime,
         "VersionId": str,
         "RequestCharged": Literal["requester"],
         "ETag": str,
-        "Checksum": ChecksumTypeDef,
-        "ObjectParts": GetObjectAttributesPartsTypeDef,
+        "Checksum": ChecksumOutputTypeDef,
+        "ObjectParts": GetObjectAttributesPartsOutputTypeDef,
         "StorageClass": StorageClassType,
         "ObjectSize": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-AccessControlPolicyTypeDef = TypedDict(
-    "AccessControlPolicyTypeDef",
+GetBucketAclOutputOutputTypeDef = TypedDict(
+    "GetBucketAclOutputOutputTypeDef",
     {
-        "Grants": Sequence[GrantTypeDef],
-        "Owner": OwnerTypeDef,
+        "Owner": OwnerOutputTypeDef,
+        "Grants": List[GrantOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-GetBucketAclOutputTypeDef = TypedDict(
-    "GetBucketAclOutputTypeDef",
+GetObjectAclOutputOutputTypeDef = TypedDict(
+    "GetObjectAclOutputOutputTypeDef",
     {
-        "Owner": OwnerTypeDef,
-        "Grants": List[GrantTypeDef],
+        "Owner": OwnerOutputTypeDef,
+        "Grants": List[GrantOutputTypeDef],
+        "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetObjectAclOutputTypeDef = TypedDict(
-    "GetObjectAclOutputTypeDef",
+LoggingEnabledOutputTypeDef = TypedDict(
+    "LoggingEnabledOutputTypeDef",
     {
-        "Owner": OwnerTypeDef,
-        "Grants": List[GrantTypeDef],
-        "RequestCharged": Literal["requester"],
+        "TargetBucket": str,
+        "TargetGrants": List[TargetGrantOutputTypeDef],
+        "TargetPrefix": str,
+    },
+)
+
+LoggingEnabledResponseMetadataTypeDef = TypedDict(
+    "LoggingEnabledResponseMetadataTypeDef",
+    {
+        "TargetBucket": str,
+        "TargetGrants": List[TargetGrantOutputTypeDef],
+        "TargetPrefix": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+AccessControlPolicyTypeDef = TypedDict(
+    "AccessControlPolicyTypeDef",
+    {
+        "Grants": Sequence[GrantTypeDef],
+        "Owner": OwnerTypeDef,
+    },
+    total=False,
+)
+
 _RequiredS3LocationTypeDef = TypedDict(
     "_RequiredS3LocationTypeDef",
     {
         "BucketName": str,
         "Prefix": str,
     },
 )
@@ -5237,64 +5968,85 @@
     },
     total=False,
 )
 
 class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
     pass
 
-LoggingEnabledResponseMetadataTypeDef = TypedDict(
-    "LoggingEnabledResponseMetadataTypeDef",
+_RequiredLoggingEnabledTypeDef = TypedDict(
+    "_RequiredLoggingEnabledTypeDef",
     {
         "TargetBucket": str,
-        "TargetGrants": List[TargetGrantTypeDef],
         "TargetPrefix": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-
-LoggingEnabledTypeDef = TypedDict(
-    "LoggingEnabledTypeDef",
+_OptionalLoggingEnabledTypeDef = TypedDict(
+    "_OptionalLoggingEnabledTypeDef",
     {
-        "TargetBucket": str,
-        "TargetGrants": List[TargetGrantTypeDef],
-        "TargetPrefix": str,
+        "TargetGrants": Sequence[TargetGrantTypeDef],
     },
+    total=False,
 )
 
-ListMultipartUploadsOutputTypeDef = TypedDict(
-    "ListMultipartUploadsOutputTypeDef",
+class LoggingEnabledTypeDef(_RequiredLoggingEnabledTypeDef, _OptionalLoggingEnabledTypeDef):
+    pass
+
+ListMultipartUploadsOutputOutputTypeDef = TypedDict(
+    "ListMultipartUploadsOutputOutputTypeDef",
     {
         "Bucket": str,
         "KeyMarker": str,
         "UploadIdMarker": str,
         "NextKeyMarker": str,
         "Prefix": str,
         "Delimiter": str,
         "NextUploadIdMarker": str,
         "MaxUploads": int,
         "IsTruncated": bool,
-        "Uploads": List[MultipartUploadTypeDef],
-        "CommonPrefixes": List[CommonPrefixTypeDef],
+        "Uploads": List[MultipartUploadOutputTypeDef],
+        "CommonPrefixes": List[CommonPrefixOutputTypeDef],
         "EncodingType": Literal["url"],
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-InventoryS3BucketDestinationTypeDef = TypedDict(
-    "InventoryS3BucketDestinationTypeDef",
+InventoryS3BucketDestinationOutputTypeDef = TypedDict(
+    "InventoryS3BucketDestinationOutputTypeDef",
     {
         "AccountId": str,
         "Bucket": str,
         "Format": InventoryFormatType,
         "Prefix": str,
+        "Encryption": InventoryEncryptionOutputTypeDef,
+    },
+)
+
+_RequiredInventoryS3BucketDestinationTypeDef = TypedDict(
+    "_RequiredInventoryS3BucketDestinationTypeDef",
+    {
+        "Bucket": str,
+        "Format": InventoryFormatType,
+    },
+)
+_OptionalInventoryS3BucketDestinationTypeDef = TypedDict(
+    "_OptionalInventoryS3BucketDestinationTypeDef",
+    {
+        "AccountId": str,
+        "Prefix": str,
         "Encryption": InventoryEncryptionTypeDef,
     },
+    total=False,
 )
 
+class InventoryS3BucketDestinationTypeDef(
+    _RequiredInventoryS3BucketDestinationTypeDef, _OptionalInventoryS3BucketDestinationTypeDef
+):
+    pass
+
 _RequiredSelectObjectContentRequestRequestTypeDef = TypedDict(
     "_RequiredSelectObjectContentRequestRequestTypeDef",
     {
         "Bucket": str,
         "Key": str,
         "Expression": str,
         "ExpressionType": Literal["SQL"],
@@ -5327,42 +6079,64 @@
         "InputSerialization": InputSerializationTypeDef,
         "ExpressionType": Literal["SQL"],
         "Expression": str,
         "OutputSerialization": OutputSerializationTypeDef,
     },
 )
 
-GetBucketLifecycleOutputTypeDef = TypedDict(
-    "GetBucketLifecycleOutputTypeDef",
+GetBucketLifecycleOutputOutputTypeDef = TypedDict(
+    "GetBucketLifecycleOutputOutputTypeDef",
     {
-        "Rules": List[RuleTypeDef],
+        "Rules": List[RuleOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LifecycleConfigurationTypeDef = TypedDict(
     "LifecycleConfigurationTypeDef",
     {
         "Rules": Sequence[RuleTypeDef],
     },
 )
 
-DestinationTypeDef = TypedDict(
-    "DestinationTypeDef",
+DestinationOutputTypeDef = TypedDict(
+    "DestinationOutputTypeDef",
     {
         "Bucket": str,
         "Account": str,
         "StorageClass": StorageClassType,
+        "AccessControlTranslation": AccessControlTranslationOutputTypeDef,
+        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
+        "ReplicationTime": ReplicationTimeOutputTypeDef,
+        "Metrics": MetricsOutputTypeDef,
+    },
+)
+
+_RequiredDestinationTypeDef = TypedDict(
+    "_RequiredDestinationTypeDef",
+    {
+        "Bucket": str,
+    },
+)
+_OptionalDestinationTypeDef = TypedDict(
+    "_OptionalDestinationTypeDef",
+    {
+        "Account": str,
+        "StorageClass": StorageClassType,
         "AccessControlTranslation": AccessControlTranslationTypeDef,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
         "ReplicationTime": ReplicationTimeTypeDef,
         "Metrics": MetricsTypeDef,
     },
+    total=False,
 )
 
+class DestinationTypeDef(_RequiredDestinationTypeDef, _OptionalDestinationTypeDef):
+    pass
+
 _RequiredPutBucketNotificationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketNotificationRequestRequestTypeDef",
     {
         "Bucket": str,
         "NotificationConfiguration": NotificationConfigurationDeprecatedTypeDef,
     },
 )
@@ -5377,77 +6151,77 @@
 
 class PutBucketNotificationRequestRequestTypeDef(
     _RequiredPutBucketNotificationRequestRequestTypeDef,
     _OptionalPutBucketNotificationRequestRequestTypeDef,
 ):
     pass
 
-ListObjectsOutputTypeDef = TypedDict(
-    "ListObjectsOutputTypeDef",
+ListObjectsOutputOutputTypeDef = TypedDict(
+    "ListObjectsOutputOutputTypeDef",
     {
         "IsTruncated": bool,
         "Marker": str,
         "NextMarker": str,
-        "Contents": List[ObjectTypeDef],
+        "Contents": List[ObjectOutputTypeDef],
         "Name": str,
         "Prefix": str,
         "Delimiter": str,
         "MaxKeys": int,
-        "CommonPrefixes": List[CommonPrefixTypeDef],
+        "CommonPrefixes": List[CommonPrefixOutputTypeDef],
         "EncodingType": Literal["url"],
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListObjectsV2OutputTypeDef = TypedDict(
-    "ListObjectsV2OutputTypeDef",
+ListObjectsV2OutputOutputTypeDef = TypedDict(
+    "ListObjectsV2OutputOutputTypeDef",
     {
         "IsTruncated": bool,
-        "Contents": List[ObjectTypeDef],
+        "Contents": List[ObjectOutputTypeDef],
         "Name": str,
         "Prefix": str,
         "Delimiter": str,
         "MaxKeys": int,
-        "CommonPrefixes": List[CommonPrefixTypeDef],
+        "CommonPrefixes": List[CommonPrefixOutputTypeDef],
         "EncodingType": Literal["url"],
         "KeyCount": int,
         "ContinuationToken": str,
         "NextContinuationToken": str,
         "StartAfter": str,
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListObjectVersionsOutputTypeDef = TypedDict(
-    "ListObjectVersionsOutputTypeDef",
+ListObjectVersionsOutputOutputTypeDef = TypedDict(
+    "ListObjectVersionsOutputOutputTypeDef",
     {
         "IsTruncated": bool,
         "KeyMarker": str,
         "VersionIdMarker": str,
         "NextKeyMarker": str,
         "NextVersionIdMarker": str,
-        "Versions": List[ObjectVersionTypeDef],
-        "DeleteMarkers": List[DeleteMarkerEntryTypeDef],
+        "Versions": List[ObjectVersionOutputTypeDef],
+        "DeleteMarkers": List[DeleteMarkerEntryOutputTypeDef],
         "Name": str,
         "Prefix": str,
         "Delimiter": str,
         "MaxKeys": int,
-        "CommonPrefixes": List[CommonPrefixTypeDef],
+        "CommonPrefixes": List[CommonPrefixOutputTypeDef],
         "EncodingType": Literal["url"],
         "RequestCharged": Literal["requester"],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetBucketOwnershipControlsOutputTypeDef = TypedDict(
-    "GetBucketOwnershipControlsOutputTypeDef",
+GetBucketOwnershipControlsOutputOutputTypeDef = TypedDict(
+    "GetBucketOwnershipControlsOutputOutputTypeDef",
     {
-        "OwnershipControls": OwnershipControlsTypeDef,
+        "OwnershipControls": OwnershipControlsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutBucketOwnershipControlsRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketOwnershipControlsRequestRequestTypeDef",
     {
@@ -5466,21 +6240,21 @@
 
 class PutBucketOwnershipControlsRequestRequestTypeDef(
     _RequiredPutBucketOwnershipControlsRequestRequestTypeDef,
     _OptionalPutBucketOwnershipControlsRequestRequestTypeDef,
 ):
     pass
 
-GetBucketWebsiteOutputTypeDef = TypedDict(
-    "GetBucketWebsiteOutputTypeDef",
+GetBucketWebsiteOutputOutputTypeDef = TypedDict(
+    "GetBucketWebsiteOutputOutputTypeDef",
     {
-        "RedirectAllRequestsTo": RedirectAllRequestsToTypeDef,
-        "IndexDocument": IndexDocumentTypeDef,
-        "ErrorDocument": ErrorDocumentTypeDef,
-        "RoutingRules": List[RoutingRuleTypeDef],
+        "RedirectAllRequestsTo": RedirectAllRequestsToOutputTypeDef,
+        "IndexDocument": IndexDocumentOutputTypeDef,
+        "ErrorDocument": ErrorDocumentOutputTypeDef,
+        "RoutingRules": List[RoutingRuleOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 WebsiteConfigurationTypeDef = TypedDict(
     "WebsiteConfigurationTypeDef",
     {
@@ -5488,76 +6262,155 @@
         "IndexDocument": IndexDocumentTypeDef,
         "RedirectAllRequestsTo": RedirectAllRequestsToTypeDef,
         "RoutingRules": Sequence[RoutingRuleTypeDef],
     },
     total=False,
 )
 
+ServerSideEncryptionConfigurationOutputTypeDef = TypedDict(
+    "ServerSideEncryptionConfigurationOutputTypeDef",
+    {
+        "Rules": List[ServerSideEncryptionRuleOutputTypeDef],
+    },
+)
+
 ServerSideEncryptionConfigurationTypeDef = TypedDict(
     "ServerSideEncryptionConfigurationTypeDef",
     {
-        "Rules": List[ServerSideEncryptionRuleTypeDef],
+        "Rules": Sequence[ServerSideEncryptionRuleTypeDef],
     },
 )
 
-SelectObjectContentEventStreamTypeDef = TypedDict(
-    "SelectObjectContentEventStreamTypeDef",
+SelectObjectContentEventStreamOutputTypeDef = TypedDict(
+    "SelectObjectContentEventStreamOutputTypeDef",
     {
-        "Records": RecordsEventTypeDef,
-        "Stats": StatsEventTypeDef,
-        "Progress": ProgressEventTypeDef,
+        "Records": RecordsEventOutputTypeDef,
+        "Stats": StatsEventOutputTypeDef,
+        "Progress": ProgressEventOutputTypeDef,
         "Cont": Dict[str, Any],
         "End": Dict[str, Any],
     },
 )
 
-IntelligentTieringConfigurationTypeDef = TypedDict(
-    "IntelligentTieringConfigurationTypeDef",
+IntelligentTieringConfigurationOutputTypeDef = TypedDict(
+    "IntelligentTieringConfigurationOutputTypeDef",
     {
         "Id": str,
-        "Filter": IntelligentTieringFilterTypeDef,
+        "Filter": IntelligentTieringFilterOutputTypeDef,
         "Status": IntelligentTieringStatusType,
-        "Tierings": List[TieringTypeDef],
+        "Tierings": List[TieringOutputTypeDef],
     },
 )
 
-LifecycleRuleTypeDef = TypedDict(
-    "LifecycleRuleTypeDef",
+LifecycleRuleOutputTypeDef = TypedDict(
+    "LifecycleRuleOutputTypeDef",
+    {
+        "Expiration": LifecycleExpirationOutputTypeDef,
+        "ID": str,
+        "Prefix": str,
+        "Filter": LifecycleRuleFilterOutputTypeDef,
+        "Status": ExpirationStatusType,
+        "Transitions": List[TransitionOutputTypeDef],
+        "NoncurrentVersionTransitions": List[NoncurrentVersionTransitionOutputTypeDef],
+        "NoncurrentVersionExpiration": NoncurrentVersionExpirationOutputTypeDef,
+        "AbortIncompleteMultipartUpload": AbortIncompleteMultipartUploadOutputTypeDef,
+    },
+)
+
+MetricsConfigurationOutputTypeDef = TypedDict(
+    "MetricsConfigurationOutputTypeDef",
+    {
+        "Id": str,
+        "Filter": MetricsFilterOutputTypeDef,
+    },
+)
+
+_RequiredIntelligentTieringConfigurationTypeDef = TypedDict(
+    "_RequiredIntelligentTieringConfigurationTypeDef",
+    {
+        "Id": str,
+        "Status": IntelligentTieringStatusType,
+        "Tierings": Sequence[TieringTypeDef],
+    },
+)
+_OptionalIntelligentTieringConfigurationTypeDef = TypedDict(
+    "_OptionalIntelligentTieringConfigurationTypeDef",
+    {
+        "Filter": IntelligentTieringFilterTypeDef,
+    },
+    total=False,
+)
+
+class IntelligentTieringConfigurationTypeDef(
+    _RequiredIntelligentTieringConfigurationTypeDef, _OptionalIntelligentTieringConfigurationTypeDef
+):
+    pass
+
+_RequiredLifecycleRuleTypeDef = TypedDict(
+    "_RequiredLifecycleRuleTypeDef",
+    {
+        "Status": ExpirationStatusType,
+    },
+)
+_OptionalLifecycleRuleTypeDef = TypedDict(
+    "_OptionalLifecycleRuleTypeDef",
     {
         "Expiration": LifecycleExpirationTypeDef,
         "ID": str,
         "Prefix": str,
         "Filter": LifecycleRuleFilterTypeDef,
-        "Status": ExpirationStatusType,
-        "Transitions": List[TransitionTypeDef],
-        "NoncurrentVersionTransitions": List[NoncurrentVersionTransitionTypeDef],
+        "Transitions": Sequence[TransitionTypeDef],
+        "NoncurrentVersionTransitions": Sequence[NoncurrentVersionTransitionTypeDef],
         "NoncurrentVersionExpiration": NoncurrentVersionExpirationTypeDef,
         "AbortIncompleteMultipartUpload": AbortIncompleteMultipartUploadTypeDef,
     },
+    total=False,
 )
 
-MetricsConfigurationTypeDef = TypedDict(
-    "MetricsConfigurationTypeDef",
+class LifecycleRuleTypeDef(_RequiredLifecycleRuleTypeDef, _OptionalLifecycleRuleTypeDef):
+    pass
+
+_RequiredMetricsConfigurationTypeDef = TypedDict(
+    "_RequiredMetricsConfigurationTypeDef",
     {
         "Id": str,
+    },
+)
+_OptionalMetricsConfigurationTypeDef = TypedDict(
+    "_OptionalMetricsConfigurationTypeDef",
+    {
         "Filter": MetricsFilterTypeDef,
     },
+    total=False,
+)
+
+class MetricsConfigurationTypeDef(
+    _RequiredMetricsConfigurationTypeDef, _OptionalMetricsConfigurationTypeDef
+):
+    pass
+
+StorageClassAnalysisOutputTypeDef = TypedDict(
+    "StorageClassAnalysisOutputTypeDef",
+    {
+        "DataExport": StorageClassAnalysisDataExportOutputTypeDef,
+    },
 )
 
 StorageClassAnalysisTypeDef = TypedDict(
     "StorageClassAnalysisTypeDef",
     {
         "DataExport": StorageClassAnalysisDataExportTypeDef,
     },
+    total=False,
 )
 
-GetObjectLockConfigurationOutputTypeDef = TypedDict(
-    "GetObjectLockConfigurationOutputTypeDef",
+GetObjectLockConfigurationOutputOutputTypeDef = TypedDict(
+    "GetObjectLockConfigurationOutputOutputTypeDef",
     {
-        "ObjectLockConfiguration": ObjectLockConfigurationTypeDef,
+        "ObjectLockConfiguration": ObjectLockConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutObjectLockConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutObjectLockConfigurationRequestRequestTypeDef",
     {
@@ -5579,42 +6432,113 @@
 
 class PutObjectLockConfigurationRequestRequestTypeDef(
     _RequiredPutObjectLockConfigurationRequestRequestTypeDef,
     _OptionalPutObjectLockConfigurationRequestRequestTypeDef,
 ):
     pass
 
-LambdaFunctionConfigurationTypeDef = TypedDict(
-    "LambdaFunctionConfigurationTypeDef",
+LambdaFunctionConfigurationOutputTypeDef = TypedDict(
+    "LambdaFunctionConfigurationOutputTypeDef",
     {
         "Id": str,
         "LambdaFunctionArn": str,
         "Events": List[EventType],
-        "Filter": NotificationConfigurationFilterTypeDef,
+        "Filter": NotificationConfigurationFilterOutputTypeDef,
     },
 )
 
-QueueConfigurationTypeDef = TypedDict(
-    "QueueConfigurationTypeDef",
+QueueConfigurationOutputTypeDef = TypedDict(
+    "QueueConfigurationOutputTypeDef",
     {
         "Id": str,
         "QueueArn": str,
         "Events": List[EventType],
-        "Filter": NotificationConfigurationFilterTypeDef,
+        "Filter": NotificationConfigurationFilterOutputTypeDef,
     },
 )
 
-TopicConfigurationTypeDef = TypedDict(
-    "TopicConfigurationTypeDef",
+TopicConfigurationOutputTypeDef = TypedDict(
+    "TopicConfigurationOutputTypeDef",
     {
         "Id": str,
         "TopicArn": str,
         "Events": List[EventType],
+        "Filter": NotificationConfigurationFilterOutputTypeDef,
+    },
+)
+
+_RequiredLambdaFunctionConfigurationTypeDef = TypedDict(
+    "_RequiredLambdaFunctionConfigurationTypeDef",
+    {
+        "LambdaFunctionArn": str,
+        "Events": Sequence[EventType],
+    },
+)
+_OptionalLambdaFunctionConfigurationTypeDef = TypedDict(
+    "_OptionalLambdaFunctionConfigurationTypeDef",
+    {
+        "Id": str,
+        "Filter": NotificationConfigurationFilterTypeDef,
+    },
+    total=False,
+)
+
+class LambdaFunctionConfigurationTypeDef(
+    _RequiredLambdaFunctionConfigurationTypeDef, _OptionalLambdaFunctionConfigurationTypeDef
+):
+    pass
+
+_RequiredQueueConfigurationTypeDef = TypedDict(
+    "_RequiredQueueConfigurationTypeDef",
+    {
+        "QueueArn": str,
+        "Events": Sequence[EventType],
+    },
+)
+_OptionalQueueConfigurationTypeDef = TypedDict(
+    "_OptionalQueueConfigurationTypeDef",
+    {
+        "Id": str,
+        "Filter": NotificationConfigurationFilterTypeDef,
+    },
+    total=False,
+)
+
+class QueueConfigurationTypeDef(
+    _RequiredQueueConfigurationTypeDef, _OptionalQueueConfigurationTypeDef
+):
+    pass
+
+_RequiredTopicConfigurationTypeDef = TypedDict(
+    "_RequiredTopicConfigurationTypeDef",
+    {
+        "TopicArn": str,
+        "Events": Sequence[EventType],
+    },
+)
+_OptionalTopicConfigurationTypeDef = TypedDict(
+    "_OptionalTopicConfigurationTypeDef",
+    {
+        "Id": str,
         "Filter": NotificationConfigurationFilterTypeDef,
     },
+    total=False,
+)
+
+class TopicConfigurationTypeDef(
+    _RequiredTopicConfigurationTypeDef, _OptionalTopicConfigurationTypeDef
+):
+    pass
+
+GetBucketLoggingOutputOutputTypeDef = TypedDict(
+    "GetBucketLoggingOutputOutputTypeDef",
+    {
+        "LoggingEnabled": LoggingEnabledOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
 )
 
 PutBucketAclRequestBucketAclPutTypeDef = TypedDict(
     "PutBucketAclRequestBucketAclPutTypeDef",
     {
         "ACL": BucketCannedACLType,
         "AccessControlPolicy": AccessControlPolicyTypeDef,
@@ -5716,19 +6640,18 @@
     "BucketLoggingStatusTypeDef",
     {
         "LoggingEnabled": LoggingEnabledTypeDef,
     },
     total=False,
 )
 
-GetBucketLoggingOutputTypeDef = TypedDict(
-    "GetBucketLoggingOutputTypeDef",
+InventoryDestinationOutputTypeDef = TypedDict(
+    "InventoryDestinationOutputTypeDef",
     {
-        "LoggingEnabled": LoggingEnabledTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "S3BucketDestination": InventoryS3BucketDestinationOutputTypeDef,
     },
 )
 
 InventoryDestinationTypeDef = TypedDict(
     "InventoryDestinationTypeDef",
     {
         "S3BucketDestination": InventoryS3BucketDestinationTypeDef,
@@ -5763,29 +6686,53 @@
 
 class PutBucketLifecycleRequestRequestTypeDef(
     _RequiredPutBucketLifecycleRequestRequestTypeDef,
     _OptionalPutBucketLifecycleRequestRequestTypeDef,
 ):
     pass
 
-ReplicationRuleTypeDef = TypedDict(
-    "ReplicationRuleTypeDef",
+ReplicationRuleOutputTypeDef = TypedDict(
+    "ReplicationRuleOutputTypeDef",
     {
         "ID": str,
         "Priority": int,
         "Prefix": str,
-        "Filter": ReplicationRuleFilterTypeDef,
+        "Filter": ReplicationRuleFilterOutputTypeDef,
+        "Status": ReplicationRuleStatusType,
+        "SourceSelectionCriteria": SourceSelectionCriteriaOutputTypeDef,
+        "ExistingObjectReplication": ExistingObjectReplicationOutputTypeDef,
+        "Destination": DestinationOutputTypeDef,
+        "DeleteMarkerReplication": DeleteMarkerReplicationOutputTypeDef,
+    },
+)
+
+_RequiredReplicationRuleTypeDef = TypedDict(
+    "_RequiredReplicationRuleTypeDef",
+    {
         "Status": ReplicationRuleStatusType,
+        "Destination": DestinationTypeDef,
+    },
+)
+_OptionalReplicationRuleTypeDef = TypedDict(
+    "_OptionalReplicationRuleTypeDef",
+    {
+        "ID": str,
+        "Priority": int,
+        "Prefix": str,
+        "Filter": ReplicationRuleFilterTypeDef,
         "SourceSelectionCriteria": SourceSelectionCriteriaTypeDef,
         "ExistingObjectReplication": ExistingObjectReplicationTypeDef,
-        "Destination": DestinationTypeDef,
         "DeleteMarkerReplication": DeleteMarkerReplicationTypeDef,
     },
+    total=False,
 )
 
+class ReplicationRuleTypeDef(_RequiredReplicationRuleTypeDef, _OptionalReplicationRuleTypeDef):
+    pass
+
 _RequiredPutBucketWebsiteRequestBucketWebsitePutTypeDef = TypedDict(
     "_RequiredPutBucketWebsiteRequestBucketWebsitePutTypeDef",
     {
         "WebsiteConfiguration": WebsiteConfigurationTypeDef,
     },
 )
 _OptionalPutBucketWebsiteRequestBucketWebsitePutTypeDef = TypedDict(
@@ -5820,18 +6767,18 @@
 )
 
 class PutBucketWebsiteRequestRequestTypeDef(
     _RequiredPutBucketWebsiteRequestRequestTypeDef, _OptionalPutBucketWebsiteRequestRequestTypeDef
 ):
     pass
 
-GetBucketEncryptionOutputTypeDef = TypedDict(
-    "GetBucketEncryptionOutputTypeDef",
+GetBucketEncryptionOutputOutputTypeDef = TypedDict(
+    "GetBucketEncryptionOutputOutputTypeDef",
     {
-        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
+        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutBucketEncryptionRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketEncryptionRequestRequestTypeDef",
     {
@@ -5851,81 +6798,81 @@
 
 class PutBucketEncryptionRequestRequestTypeDef(
     _RequiredPutBucketEncryptionRequestRequestTypeDef,
     _OptionalPutBucketEncryptionRequestRequestTypeDef,
 ):
     pass
 
-SelectObjectContentOutputTypeDef = TypedDict(
-    "SelectObjectContentOutputTypeDef",
+SelectObjectContentOutputOutputTypeDef = TypedDict(
+    "SelectObjectContentOutputOutputTypeDef",
     {
-        "Payload": "EventStream[SelectObjectContentEventStreamTypeDef]",
+        "Payload": "EventStream[SelectObjectContentEventStreamOutputTypeDef]",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetBucketIntelligentTieringConfigurationOutputTypeDef = TypedDict(
-    "GetBucketIntelligentTieringConfigurationOutputTypeDef",
+GetBucketIntelligentTieringConfigurationOutputOutputTypeDef = TypedDict(
+    "GetBucketIntelligentTieringConfigurationOutputOutputTypeDef",
     {
-        "IntelligentTieringConfiguration": IntelligentTieringConfigurationTypeDef,
+        "IntelligentTieringConfiguration": IntelligentTieringConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListBucketIntelligentTieringConfigurationsOutputTypeDef = TypedDict(
-    "ListBucketIntelligentTieringConfigurationsOutputTypeDef",
+ListBucketIntelligentTieringConfigurationsOutputOutputTypeDef = TypedDict(
+    "ListBucketIntelligentTieringConfigurationsOutputOutputTypeDef",
     {
         "IsTruncated": bool,
         "ContinuationToken": str,
         "NextContinuationToken": str,
-        "IntelligentTieringConfigurationList": List[IntelligentTieringConfigurationTypeDef],
+        "IntelligentTieringConfigurationList": List[IntelligentTieringConfigurationOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutBucketIntelligentTieringConfigurationRequestRequestTypeDef = TypedDict(
-    "PutBucketIntelligentTieringConfigurationRequestRequestTypeDef",
+GetBucketLifecycleConfigurationOutputOutputTypeDef = TypedDict(
+    "GetBucketLifecycleConfigurationOutputOutputTypeDef",
     {
-        "Bucket": str,
-        "Id": str,
-        "IntelligentTieringConfiguration": IntelligentTieringConfigurationTypeDef,
+        "Rules": List[LifecycleRuleOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-BucketLifecycleConfigurationTypeDef = TypedDict(
-    "BucketLifecycleConfigurationTypeDef",
+GetBucketMetricsConfigurationOutputOutputTypeDef = TypedDict(
+    "GetBucketMetricsConfigurationOutputOutputTypeDef",
     {
-        "Rules": Sequence[LifecycleRuleTypeDef],
+        "MetricsConfiguration": MetricsConfigurationOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetBucketLifecycleConfigurationOutputTypeDef = TypedDict(
-    "GetBucketLifecycleConfigurationOutputTypeDef",
+ListBucketMetricsConfigurationsOutputOutputTypeDef = TypedDict(
+    "ListBucketMetricsConfigurationsOutputOutputTypeDef",
     {
-        "Rules": List[LifecycleRuleTypeDef],
+        "IsTruncated": bool,
+        "ContinuationToken": str,
+        "NextContinuationToken": str,
+        "MetricsConfigurationList": List[MetricsConfigurationOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetBucketMetricsConfigurationOutputTypeDef = TypedDict(
-    "GetBucketMetricsConfigurationOutputTypeDef",
+PutBucketIntelligentTieringConfigurationRequestRequestTypeDef = TypedDict(
+    "PutBucketIntelligentTieringConfigurationRequestRequestTypeDef",
     {
-        "MetricsConfiguration": MetricsConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Bucket": str,
+        "Id": str,
+        "IntelligentTieringConfiguration": IntelligentTieringConfigurationTypeDef,
     },
 )
 
-ListBucketMetricsConfigurationsOutputTypeDef = TypedDict(
-    "ListBucketMetricsConfigurationsOutputTypeDef",
+BucketLifecycleConfigurationTypeDef = TypedDict(
+    "BucketLifecycleConfigurationTypeDef",
     {
-        "IsTruncated": bool,
-        "ContinuationToken": str,
-        "NextContinuationToken": str,
-        "MetricsConfigurationList": List[MetricsConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Rules": Sequence[LifecycleRuleTypeDef],
     },
 )
 
 _RequiredPutBucketMetricsConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketMetricsConfigurationRequestRequestTypeDef",
     {
         "Bucket": str,
@@ -5943,29 +6890,49 @@
 
 class PutBucketMetricsConfigurationRequestRequestTypeDef(
     _RequiredPutBucketMetricsConfigurationRequestRequestTypeDef,
     _OptionalPutBucketMetricsConfigurationRequestRequestTypeDef,
 ):
     pass
 
-AnalyticsConfigurationTypeDef = TypedDict(
-    "AnalyticsConfigurationTypeDef",
+AnalyticsConfigurationOutputTypeDef = TypedDict(
+    "AnalyticsConfigurationOutputTypeDef",
+    {
+        "Id": str,
+        "Filter": AnalyticsFilterOutputTypeDef,
+        "StorageClassAnalysis": StorageClassAnalysisOutputTypeDef,
+    },
+)
+
+_RequiredAnalyticsConfigurationTypeDef = TypedDict(
+    "_RequiredAnalyticsConfigurationTypeDef",
     {
         "Id": str,
-        "Filter": AnalyticsFilterTypeDef,
         "StorageClassAnalysis": StorageClassAnalysisTypeDef,
     },
 )
+_OptionalAnalyticsConfigurationTypeDef = TypedDict(
+    "_OptionalAnalyticsConfigurationTypeDef",
+    {
+        "Filter": AnalyticsFilterTypeDef,
+    },
+    total=False,
+)
 
-NotificationConfigurationResponseMetadataTypeDef = TypedDict(
-    "NotificationConfigurationResponseMetadataTypeDef",
+class AnalyticsConfigurationTypeDef(
+    _RequiredAnalyticsConfigurationTypeDef, _OptionalAnalyticsConfigurationTypeDef
+):
+    pass
+
+NotificationConfigurationOutputTypeDef = TypedDict(
+    "NotificationConfigurationOutputTypeDef",
     {
-        "TopicConfigurations": List[TopicConfigurationTypeDef],
-        "QueueConfigurations": List[QueueConfigurationTypeDef],
-        "LambdaFunctionConfigurations": List[LambdaFunctionConfigurationTypeDef],
+        "TopicConfigurations": List[TopicConfigurationOutputTypeDef],
+        "QueueConfigurations": List[QueueConfigurationOutputTypeDef],
+        "LambdaFunctionConfigurations": List[LambdaFunctionConfigurationOutputTypeDef],
         "EventBridgeConfiguration": Dict[str, Any],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 NotificationConfigurationTypeDef = TypedDict(
     "NotificationConfigurationTypeDef",
@@ -6030,32 +6997,64 @@
 )
 
 class PutBucketLoggingRequestRequestTypeDef(
     _RequiredPutBucketLoggingRequestRequestTypeDef, _OptionalPutBucketLoggingRequestRequestTypeDef
 ):
     pass
 
-InventoryConfigurationTypeDef = TypedDict(
-    "InventoryConfigurationTypeDef",
+InventoryConfigurationOutputTypeDef = TypedDict(
+    "InventoryConfigurationOutputTypeDef",
     {
-        "Destination": InventoryDestinationTypeDef,
+        "Destination": InventoryDestinationOutputTypeDef,
         "IsEnabled": bool,
-        "Filter": InventoryFilterTypeDef,
+        "Filter": InventoryFilterOutputTypeDef,
         "Id": str,
         "IncludedObjectVersions": InventoryIncludedObjectVersionsType,
         "OptionalFields": List[InventoryOptionalFieldType],
+        "Schedule": InventoryScheduleOutputTypeDef,
+    },
+)
+
+_RequiredInventoryConfigurationTypeDef = TypedDict(
+    "_RequiredInventoryConfigurationTypeDef",
+    {
+        "Destination": InventoryDestinationTypeDef,
+        "IsEnabled": bool,
+        "Id": str,
+        "IncludedObjectVersions": InventoryIncludedObjectVersionsType,
         "Schedule": InventoryScheduleTypeDef,
     },
 )
+_OptionalInventoryConfigurationTypeDef = TypedDict(
+    "_OptionalInventoryConfigurationTypeDef",
+    {
+        "Filter": InventoryFilterTypeDef,
+        "OptionalFields": Sequence[InventoryOptionalFieldType],
+    },
+    total=False,
+)
+
+class InventoryConfigurationTypeDef(
+    _RequiredInventoryConfigurationTypeDef, _OptionalInventoryConfigurationTypeDef
+):
+    pass
+
+ReplicationConfigurationOutputTypeDef = TypedDict(
+    "ReplicationConfigurationOutputTypeDef",
+    {
+        "Role": str,
+        "Rules": List[ReplicationRuleOutputTypeDef],
+    },
+)
 
 ReplicationConfigurationTypeDef = TypedDict(
     "ReplicationConfigurationTypeDef",
     {
         "Role": str,
-        "Rules": List[ReplicationRuleTypeDef],
+        "Rules": Sequence[ReplicationRuleTypeDef],
     },
 )
 
 PutBucketLifecycleConfigurationRequestBucketLifecycleConfigurationPutTypeDef = TypedDict(
     "PutBucketLifecycleConfigurationRequestBucketLifecycleConfigurationPutTypeDef",
     {
         "ChecksumAlgorithm": ChecksumAlgorithmType,
@@ -6083,29 +7082,29 @@
 
 class PutBucketLifecycleConfigurationRequestRequestTypeDef(
     _RequiredPutBucketLifecycleConfigurationRequestRequestTypeDef,
     _OptionalPutBucketLifecycleConfigurationRequestRequestTypeDef,
 ):
     pass
 
-GetBucketAnalyticsConfigurationOutputTypeDef = TypedDict(
-    "GetBucketAnalyticsConfigurationOutputTypeDef",
+GetBucketAnalyticsConfigurationOutputOutputTypeDef = TypedDict(
+    "GetBucketAnalyticsConfigurationOutputOutputTypeDef",
     {
-        "AnalyticsConfiguration": AnalyticsConfigurationTypeDef,
+        "AnalyticsConfiguration": AnalyticsConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListBucketAnalyticsConfigurationsOutputTypeDef = TypedDict(
-    "ListBucketAnalyticsConfigurationsOutputTypeDef",
+ListBucketAnalyticsConfigurationsOutputOutputTypeDef = TypedDict(
+    "ListBucketAnalyticsConfigurationsOutputOutputTypeDef",
     {
         "IsTruncated": bool,
         "ContinuationToken": str,
         "NextContinuationToken": str,
-        "AnalyticsConfigurationList": List[AnalyticsConfigurationTypeDef],
+        "AnalyticsConfigurationList": List[AnalyticsConfigurationOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutBucketAnalyticsConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketAnalyticsConfigurationRequestRequestTypeDef",
     {
@@ -6215,27 +7214,27 @@
 )
 
 class RestoreObjectRequestRequestTypeDef(
     _RequiredRestoreObjectRequestRequestTypeDef, _OptionalRestoreObjectRequestRequestTypeDef
 ):
     pass
 
-GetBucketInventoryConfigurationOutputTypeDef = TypedDict(
-    "GetBucketInventoryConfigurationOutputTypeDef",
+GetBucketInventoryConfigurationOutputOutputTypeDef = TypedDict(
+    "GetBucketInventoryConfigurationOutputOutputTypeDef",
     {
-        "InventoryConfiguration": InventoryConfigurationTypeDef,
+        "InventoryConfiguration": InventoryConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListBucketInventoryConfigurationsOutputTypeDef = TypedDict(
-    "ListBucketInventoryConfigurationsOutputTypeDef",
+ListBucketInventoryConfigurationsOutputOutputTypeDef = TypedDict(
+    "ListBucketInventoryConfigurationsOutputOutputTypeDef",
     {
         "ContinuationToken": str,
-        "InventoryConfigurationList": List[InventoryConfigurationTypeDef],
+        "InventoryConfigurationList": List[InventoryConfigurationOutputTypeDef],
         "IsTruncated": bool,
         "NextContinuationToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutBucketInventoryConfigurationRequestRequestTypeDef = TypedDict(
@@ -6256,18 +7255,18 @@
 
 class PutBucketInventoryConfigurationRequestRequestTypeDef(
     _RequiredPutBucketInventoryConfigurationRequestRequestTypeDef,
     _OptionalPutBucketInventoryConfigurationRequestRequestTypeDef,
 ):
     pass
 
-GetBucketReplicationOutputTypeDef = TypedDict(
-    "GetBucketReplicationOutputTypeDef",
+GetBucketReplicationOutputOutputTypeDef = TypedDict(
+    "GetBucketReplicationOutputOutputTypeDef",
     {
-        "ReplicationConfiguration": ReplicationConfigurationTypeDef,
+        "ReplicationConfiguration": ReplicationConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutBucketReplicationRequestRequestTypeDef = TypedDict(
     "_RequiredPutBucketReplicationRequestRequestTypeDef",
     {
```

### Comparing `mypy-boto3-s3-1.28.3/mypy_boto3_s3/waiter.py` & `mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.28.3/mypy_boto3_s3/waiter.pyi` & `mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.28.3/mypy_boto3_s3.egg-info/PKG-INFO` & `mypy-boto3-s3-1.28.3.post1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-s3
-Version: 1.28.3
-Summary: Type annotations for boto3.S3 1.28.3 service generated with mypy-boto3-builder 7.14.6
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 s3 type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-s3"></a>
 
 # mypy-boto3-s3
 
 [![PyPI - mypy-boto3-s3](https://img.shields.io/pypi/v/mypy-boto3-s3.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/)
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
 [mypy-boto3-s3 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3/).
 
 See how it helps to find and fix potential bugs:
 
@@ -551,53 +519,61 @@
 ### Typed dictionaries
 
 `mypy_boto3_s3.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_s3.type_defs import (
+    AbortIncompleteMultipartUploadOutputTypeDef,
     AbortIncompleteMultipartUploadTypeDef,
-    AbortMultipartUploadOutputTypeDef,
+    AbortMultipartUploadOutputOutputTypeDef,
     AbortMultipartUploadRequestMultipartUploadAbortTypeDef,
     AbortMultipartUploadRequestRequestTypeDef,
     AccelerateConfigurationTypeDef,
     OwnerTypeDef,
+    AccessControlTranslationOutputTypeDef,
     AccessControlTranslationTypeDef,
+    TagOutputTypeDef,
     TagTypeDef,
+    AnalyticsS3BucketDestinationOutputTypeDef,
     AnalyticsS3BucketDestinationTypeDef,
     CopySourceTypeDef,
     BucketDownloadFileRequestTypeDef,
     BucketDownloadFileobjRequestTypeDef,
-    BucketTypeDef,
+    BucketOutputTypeDef,
     BucketUploadFileRequestTypeDef,
     BucketUploadFileobjRequestTypeDef,
     CORSRuleTypeDef,
+    CORSRuleOutputTypeDef,
     CSVInputTypeDef,
     CSVOutputTypeDef,
-    ChecksumTypeDef,
+    ChecksumOutputTypeDef,
     ClientDownloadFileRequestTypeDef,
     ClientDownloadFileobjRequestTypeDef,
     ClientGeneratePresignedPostRequestTypeDef,
     ClientUploadFileRequestTypeDef,
     ClientUploadFileobjRequestTypeDef,
+    CloudFunctionConfigurationOutputTypeDef,
     CloudFunctionConfigurationTypeDef,
-    CommonPrefixTypeDef,
-    CompleteMultipartUploadOutputTypeDef,
+    CommonPrefixOutputTypeDef,
+    CompleteMultipartUploadOutputOutputTypeDef,
     CompletedPartTypeDef,
+    ConditionOutputTypeDef,
     ConditionTypeDef,
-    CopyObjectResultTypeDef,
+    CopyObjectResultOutputTypeDef,
     CopyObjectRequestObjectCopyFromTypeDef,
     CopyObjectRequestObjectSummaryCopyFromTypeDef,
-    CopyPartResultTypeDef,
+    CopyPartResultOutputTypeDef,
     CreateBucketConfigurationTypeDef,
-    CreateBucketOutputTypeDef,
-    CreateMultipartUploadOutputTypeDef,
+    CreateBucketOutputOutputTypeDef,
+    CreateMultipartUploadOutputOutputTypeDef,
     CreateMultipartUploadRequestObjectInitiateMultipartUploadTypeDef,
     CreateMultipartUploadRequestObjectSummaryInitiateMultipartUploadTypeDef,
     CreateMultipartUploadRequestRequestTypeDef,
+    DefaultRetentionOutputTypeDef,
     DefaultRetentionTypeDef,
     DeleteBucketAnalyticsConfigurationRequestRequestTypeDef,
     DeleteBucketCorsRequestBucketCorsDeleteTypeDef,
     DeleteBucketCorsRequestRequestTypeDef,
     DeleteBucketEncryptionRequestRequestTypeDef,
     DeleteBucketIntelligentTieringConfigurationRequestRequestTypeDef,
     DeleteBucketInventoryConfigurationRequestRequestTypeDef,
@@ -611,97 +587,113 @@
     DeleteBucketReplicationRequestRequestTypeDef,
     DeleteBucketRequestBucketDeleteTypeDef,
     DeleteBucketRequestRequestTypeDef,
     DeleteBucketTaggingRequestBucketTaggingDeleteTypeDef,
     DeleteBucketTaggingRequestRequestTypeDef,
     DeleteBucketWebsiteRequestBucketWebsiteDeleteTypeDef,
     DeleteBucketWebsiteRequestRequestTypeDef,
+    OwnerOutputTypeDef,
+    DeleteMarkerReplicationOutputTypeDef,
     DeleteMarkerReplicationTypeDef,
-    DeleteObjectOutputTypeDef,
+    DeleteObjectOutputOutputTypeDef,
     DeleteObjectRequestObjectDeleteTypeDef,
     DeleteObjectRequestObjectSummaryDeleteTypeDef,
     DeleteObjectRequestObjectVersionDeleteTypeDef,
     DeleteObjectRequestRequestTypeDef,
-    DeleteObjectTaggingOutputTypeDef,
+    DeleteObjectTaggingOutputOutputTypeDef,
     DeleteObjectTaggingRequestRequestTypeDef,
-    DeletedObjectTypeDef,
-    ErrorTypeDef,
+    DeletedObjectOutputTypeDef,
+    ErrorOutputTypeDef,
     DeletePublicAccessBlockRequestRequestTypeDef,
     ObjectIdentifierTypeDef,
+    EncryptionConfigurationOutputTypeDef,
     EncryptionConfigurationTypeDef,
     EmptyResponseMetadataTypeDef,
     EncryptionTypeDef,
+    ErrorDocumentOutputTypeDef,
     ErrorDocumentResponseMetadataTypeDef,
     ErrorDocumentTypeDef,
+    ExistingObjectReplicationOutputTypeDef,
     ExistingObjectReplicationTypeDef,
+    FilterRuleOutputTypeDef,
     FilterRuleTypeDef,
-    GetBucketAccelerateConfigurationOutputTypeDef,
+    GetBucketAccelerateConfigurationOutputOutputTypeDef,
     GetBucketAccelerateConfigurationRequestRequestTypeDef,
     GetBucketAclRequestRequestTypeDef,
     GetBucketAnalyticsConfigurationRequestRequestTypeDef,
     GetBucketCorsRequestRequestTypeDef,
     GetBucketEncryptionRequestRequestTypeDef,
     GetBucketIntelligentTieringConfigurationRequestRequestTypeDef,
     GetBucketInventoryConfigurationRequestRequestTypeDef,
     GetBucketLifecycleConfigurationRequestRequestTypeDef,
     GetBucketLifecycleRequestRequestTypeDef,
-    GetBucketLocationOutputTypeDef,
+    GetBucketLocationOutputOutputTypeDef,
     GetBucketLocationRequestRequestTypeDef,
     GetBucketLoggingRequestRequestTypeDef,
     GetBucketMetricsConfigurationRequestRequestTypeDef,
     GetBucketNotificationConfigurationRequestRequestTypeDef,
     GetBucketOwnershipControlsRequestRequestTypeDef,
-    GetBucketPolicyOutputTypeDef,
+    GetBucketPolicyOutputOutputTypeDef,
     GetBucketPolicyRequestRequestTypeDef,
-    PolicyStatusTypeDef,
+    PolicyStatusOutputTypeDef,
     GetBucketPolicyStatusRequestRequestTypeDef,
     GetBucketReplicationRequestRequestTypeDef,
-    GetBucketRequestPaymentOutputTypeDef,
+    GetBucketRequestPaymentOutputOutputTypeDef,
     GetBucketRequestPaymentRequestRequestTypeDef,
     GetBucketTaggingRequestRequestTypeDef,
-    GetBucketVersioningOutputTypeDef,
+    GetBucketVersioningOutputOutputTypeDef,
     GetBucketVersioningRequestRequestTypeDef,
-    IndexDocumentTypeDef,
-    RedirectAllRequestsToTypeDef,
+    IndexDocumentOutputTypeDef,
+    RedirectAllRequestsToOutputTypeDef,
     GetBucketWebsiteRequestRequestTypeDef,
     GetObjectAclRequestRequestTypeDef,
-    ObjectPartTypeDef,
+    ObjectPartOutputTypeDef,
     GetObjectAttributesRequestRequestTypeDef,
-    ObjectLockLegalHoldTypeDef,
+    ObjectLockLegalHoldOutputTypeDef,
     GetObjectLegalHoldRequestRequestTypeDef,
     GetObjectLockConfigurationRequestRequestTypeDef,
-    GetObjectOutputTypeDef,
+    GetObjectOutputOutputTypeDef,
     GetObjectRequestObjectGetTypeDef,
     GetObjectRequestObjectSummaryGetTypeDef,
     GetObjectRequestObjectVersionGetTypeDef,
     GetObjectRequestRequestTypeDef,
-    ObjectLockRetentionTypeDef,
+    ObjectLockRetentionOutputTypeDef,
     GetObjectRetentionRequestRequestTypeDef,
     GetObjectTaggingRequestRequestTypeDef,
-    GetObjectTorrentOutputTypeDef,
+    GetObjectTorrentOutputOutputTypeDef,
     GetObjectTorrentRequestRequestTypeDef,
-    PublicAccessBlockConfigurationTypeDef,
+    PublicAccessBlockConfigurationOutputTypeDef,
     GetPublicAccessBlockRequestRequestTypeDef,
     GlacierJobParametersTypeDef,
+    GranteeOutputTypeDef,
     GranteeTypeDef,
     WaiterConfigTypeDef,
     HeadBucketRequestRequestTypeDef,
-    HeadObjectOutputTypeDef,
+    HeadObjectOutputOutputTypeDef,
     HeadObjectRequestObjectVersionHeadTypeDef,
     HeadObjectRequestRequestTypeDef,
     IndexDocumentResponseMetadataTypeDef,
+    IndexDocumentTypeDef,
+    InitiatorOutputTypeDef,
     InitiatorResponseMetadataTypeDef,
-    InitiatorTypeDef,
     JSONInputTypeDef,
+    TieringOutputTypeDef,
     TieringTypeDef,
+    InventoryFilterOutputTypeDef,
+    InventoryScheduleOutputTypeDef,
     InventoryFilterTypeDef,
     InventoryScheduleTypeDef,
+    SSEKMSOutputTypeDef,
     SSEKMSTypeDef,
     JSONOutputTypeDef,
+    LifecycleExpirationOutputTypeDef,
     LifecycleExpirationTypeDef,
+    NoncurrentVersionExpirationOutputTypeDef,
+    NoncurrentVersionTransitionOutputTypeDef,
+    TransitionOutputTypeDef,
     NoncurrentVersionExpirationTypeDef,
     NoncurrentVersionTransitionTypeDef,
     TransitionTypeDef,
     ListBucketAnalyticsConfigurationsRequestRequestTypeDef,
     ListBucketIntelligentTieringConfigurationsRequestRequestTypeDef,
     ListBucketInventoryConfigurationsRequestRequestTypeDef,
     ListBucketMetricsConfigurationsRequestRequestTypeDef,
@@ -709,229 +701,283 @@
     ListMultipartUploadsRequestRequestTypeDef,
     ListObjectVersionsRequestListObjectVersionsPaginateTypeDef,
     ListObjectVersionsRequestRequestTypeDef,
     ListObjectsRequestListObjectsPaginateTypeDef,
     ListObjectsRequestRequestTypeDef,
     ListObjectsV2RequestListObjectsV2PaginateTypeDef,
     ListObjectsV2RequestRequestTypeDef,
-    PartTypeDef,
+    PartOutputTypeDef,
     ListPartsRequestListPartsPaginateTypeDef,
     ListPartsRequestRequestTypeDef,
     MetadataEntryTypeDef,
+    ReplicationTimeValueOutputTypeDef,
     ReplicationTimeValueTypeDef,
+    QueueConfigurationDeprecatedOutputTypeDef,
+    TopicConfigurationDeprecatedOutputTypeDef,
     QueueConfigurationDeprecatedTypeDef,
     TopicConfigurationDeprecatedTypeDef,
     ObjectDownloadFileRequestTypeDef,
     ObjectDownloadFileobjRequestTypeDef,
-    RestoreStatusTypeDef,
+    ObjectLockLegalHoldTypeDef,
+    ObjectLockRetentionTypeDef,
+    RestoreStatusOutputTypeDef,
     ObjectUploadFileRequestTypeDef,
     ObjectUploadFileobjRequestTypeDef,
     OwnerResponseMetadataTypeDef,
+    OwnershipControlsRuleOutputTypeDef,
     OwnershipControlsRuleTypeDef,
     PaginatorConfigTypeDef,
-    ProgressTypeDef,
+    ProgressOutputTypeDef,
+    PublicAccessBlockConfigurationTypeDef,
     PutBucketPolicyRequestBucketPolicyPutTypeDef,
     PutBucketPolicyRequestRequestTypeDef,
     RequestPaymentConfigurationTypeDef,
     PutBucketVersioningRequestBucketVersioningEnableTypeDef,
     VersioningConfigurationTypeDef,
     PutBucketVersioningRequestBucketVersioningSuspendTypeDef,
-    PutObjectAclOutputTypeDef,
-    PutObjectLegalHoldOutputTypeDef,
-    PutObjectLockConfigurationOutputTypeDef,
-    PutObjectOutputTypeDef,
+    PutObjectAclOutputOutputTypeDef,
+    PutObjectLegalHoldOutputOutputTypeDef,
+    PutObjectLockConfigurationOutputOutputTypeDef,
+    PutObjectOutputOutputTypeDef,
     PutObjectRequestBucketPutObjectTypeDef,
     PutObjectRequestObjectPutTypeDef,
     PutObjectRequestObjectSummaryPutTypeDef,
     PutObjectRequestRequestTypeDef,
-    PutObjectRetentionOutputTypeDef,
-    PutObjectTaggingOutputTypeDef,
-    RecordsEventTypeDef,
+    PutObjectRetentionOutputOutputTypeDef,
+    PutObjectTaggingOutputOutputTypeDef,
+    RecordsEventOutputTypeDef,
     RedirectAllRequestsToResponseMetadataTypeDef,
+    RedirectAllRequestsToTypeDef,
+    RedirectOutputTypeDef,
     RedirectTypeDef,
+    ReplicaModificationsOutputTypeDef,
     ReplicaModificationsTypeDef,
     RequestProgressTypeDef,
     ResponseMetadataTypeDef,
-    RestoreObjectOutputTypeDef,
+    RestoreObjectOutputOutputTypeDef,
     RestoreStatusResponseMetadataTypeDef,
     ScanRangeTypeDef,
+    ServerSideEncryptionByDefaultOutputTypeDef,
     ServerSideEncryptionByDefaultTypeDef,
+    SseKmsEncryptedObjectsOutputTypeDef,
     SseKmsEncryptedObjectsTypeDef,
-    StatsTypeDef,
-    UploadPartOutputTypeDef,
+    StatsOutputTypeDef,
+    UploadPartOutputOutputTypeDef,
     UploadPartRequestMultipartUploadPartUploadTypeDef,
     UploadPartRequestRequestTypeDef,
     WriteGetObjectResponseRequestRequestTypeDef,
     PutBucketAccelerateConfigurationRequestRequestTypeDef,
-    DeleteMarkerEntryTypeDef,
+    AnalyticsAndOperatorOutputTypeDef,
+    GetBucketTaggingOutputOutputTypeDef,
+    GetObjectTaggingOutputOutputTypeDef,
+    IntelligentTieringAndOperatorOutputTypeDef,
+    LifecycleRuleAndOperatorOutputTypeDef,
+    MetricsAndOperatorOutputTypeDef,
+    ReplicationRuleAndOperatorOutputTypeDef,
     AnalyticsAndOperatorTypeDef,
-    GetBucketTaggingOutputTypeDef,
-    GetObjectTaggingOutputTypeDef,
     IntelligentTieringAndOperatorTypeDef,
     LifecycleRuleAndOperatorTypeDef,
     MetricsAndOperatorTypeDef,
     ReplicationRuleAndOperatorTypeDef,
     TaggingTypeDef,
+    AnalyticsExportDestinationOutputTypeDef,
     AnalyticsExportDestinationTypeDef,
     BucketCopyRequestTypeDef,
     ClientCopyRequestTypeDef,
     CopyObjectRequestRequestTypeDef,
     ObjectCopyRequestTypeDef,
     UploadPartCopyRequestMultipartUploadPartCopyFromTypeDef,
     UploadPartCopyRequestRequestTypeDef,
-    ListBucketsOutputTypeDef,
     CORSConfigurationTypeDef,
-    GetBucketCorsOutputTypeDef,
+    GetBucketCorsOutputOutputTypeDef,
     CompletedMultipartUploadTypeDef,
-    CopyObjectOutputTypeDef,
-    UploadPartCopyOutputTypeDef,
+    CopyObjectOutputOutputTypeDef,
+    UploadPartCopyOutputOutputTypeDef,
     CreateBucketRequestBucketCreateTypeDef,
     CreateBucketRequestRequestTypeDef,
     CreateBucketRequestServiceResourceCreateBucketTypeDef,
+    ObjectLockRuleOutputTypeDef,
     ObjectLockRuleTypeDef,
-    DeleteObjectsOutputTypeDef,
+    DeleteMarkerEntryOutputTypeDef,
+    ListBucketsOutputOutputTypeDef,
+    DeleteObjectsOutputOutputTypeDef,
     DeleteTypeDef,
+    S3KeyFilterOutputTypeDef,
     S3KeyFilterTypeDef,
-    GetBucketPolicyStatusOutputTypeDef,
-    GetObjectAttributesPartsTypeDef,
-    GetObjectLegalHoldOutputTypeDef,
-    PutObjectLegalHoldRequestRequestTypeDef,
-    GetObjectRetentionOutputTypeDef,
-    PutObjectRetentionRequestRequestTypeDef,
-    GetPublicAccessBlockOutputTypeDef,
-    PutPublicAccessBlockRequestRequestTypeDef,
+    GetBucketPolicyStatusOutputOutputTypeDef,
+    GetObjectAttributesPartsOutputTypeDef,
+    GetObjectLegalHoldOutputOutputTypeDef,
+    GetObjectRetentionOutputOutputTypeDef,
+    GetPublicAccessBlockOutputOutputTypeDef,
+    GrantOutputTypeDef,
+    TargetGrantOutputTypeDef,
     GrantTypeDef,
     TargetGrantTypeDef,
     HeadBucketRequestBucketExistsWaitTypeDef,
     HeadBucketRequestBucketNotExistsWaitTypeDef,
     HeadObjectRequestObjectExistsWaitTypeDef,
     HeadObjectRequestObjectNotExistsWaitTypeDef,
-    MultipartUploadTypeDef,
+    MultipartUploadOutputTypeDef,
     InputSerializationTypeDef,
+    InventoryEncryptionOutputTypeDef,
     InventoryEncryptionTypeDef,
     OutputSerializationTypeDef,
+    RuleOutputTypeDef,
     RuleTypeDef,
-    ListPartsOutputTypeDef,
+    ListPartsOutputOutputTypeDef,
+    MetricsOutputTypeDef,
+    ReplicationTimeOutputTypeDef,
     MetricsTypeDef,
     ReplicationTimeTypeDef,
-    NotificationConfigurationDeprecatedResponseMetadataTypeDef,
+    NotificationConfigurationDeprecatedOutputTypeDef,
     NotificationConfigurationDeprecatedTypeDef,
-    ObjectTypeDef,
-    ObjectVersionTypeDef,
+    PutObjectLegalHoldRequestRequestTypeDef,
+    PutObjectRetentionRequestRequestTypeDef,
+    ObjectOutputTypeDef,
+    ObjectVersionOutputTypeDef,
+    OwnershipControlsOutputTypeDef,
     OwnershipControlsTypeDef,
-    ProgressEventTypeDef,
+    ProgressEventOutputTypeDef,
+    PutPublicAccessBlockRequestRequestTypeDef,
     PutBucketRequestPaymentRequestBucketRequestPaymentPutTypeDef,
     PutBucketRequestPaymentRequestRequestTypeDef,
     PutBucketVersioningRequestBucketVersioningPutTypeDef,
     PutBucketVersioningRequestRequestTypeDef,
+    RoutingRuleOutputTypeDef,
     RoutingRuleTypeDef,
+    ServerSideEncryptionRuleOutputTypeDef,
     ServerSideEncryptionRuleTypeDef,
+    SourceSelectionCriteriaOutputTypeDef,
     SourceSelectionCriteriaTypeDef,
-    StatsEventTypeDef,
+    StatsEventOutputTypeDef,
+    AnalyticsFilterOutputTypeDef,
+    IntelligentTieringFilterOutputTypeDef,
+    LifecycleRuleFilterOutputTypeDef,
+    MetricsFilterOutputTypeDef,
+    ReplicationRuleFilterOutputTypeDef,
     AnalyticsFilterTypeDef,
     IntelligentTieringFilterTypeDef,
     LifecycleRuleFilterTypeDef,
     MetricsFilterTypeDef,
     ReplicationRuleFilterTypeDef,
     PutBucketTaggingRequestBucketTaggingPutTypeDef,
     PutBucketTaggingRequestRequestTypeDef,
     PutObjectTaggingRequestRequestTypeDef,
+    StorageClassAnalysisDataExportOutputTypeDef,
     StorageClassAnalysisDataExportTypeDef,
     PutBucketCorsRequestBucketCorsPutTypeDef,
     PutBucketCorsRequestRequestTypeDef,
     CompleteMultipartUploadRequestMultipartUploadCompleteTypeDef,
     CompleteMultipartUploadRequestRequestTypeDef,
+    ObjectLockConfigurationOutputTypeDef,
     ObjectLockConfigurationTypeDef,
     DeleteObjectsRequestBucketDeleteObjectsTypeDef,
     DeleteObjectsRequestRequestTypeDef,
+    NotificationConfigurationFilterOutputTypeDef,
     NotificationConfigurationFilterTypeDef,
-    GetObjectAttributesOutputTypeDef,
+    GetObjectAttributesOutputOutputTypeDef,
+    GetBucketAclOutputOutputTypeDef,
+    GetObjectAclOutputOutputTypeDef,
+    LoggingEnabledOutputTypeDef,
+    LoggingEnabledResponseMetadataTypeDef,
     AccessControlPolicyTypeDef,
-    GetBucketAclOutputTypeDef,
-    GetObjectAclOutputTypeDef,
     S3LocationTypeDef,
-    LoggingEnabledResponseMetadataTypeDef,
     LoggingEnabledTypeDef,
-    ListMultipartUploadsOutputTypeDef,
+    ListMultipartUploadsOutputOutputTypeDef,
+    InventoryS3BucketDestinationOutputTypeDef,
     InventoryS3BucketDestinationTypeDef,
     SelectObjectContentRequestRequestTypeDef,
     SelectParametersTypeDef,
-    GetBucketLifecycleOutputTypeDef,
+    GetBucketLifecycleOutputOutputTypeDef,
     LifecycleConfigurationTypeDef,
+    DestinationOutputTypeDef,
     DestinationTypeDef,
     PutBucketNotificationRequestRequestTypeDef,
-    ListObjectsOutputTypeDef,
-    ListObjectsV2OutputTypeDef,
-    ListObjectVersionsOutputTypeDef,
-    GetBucketOwnershipControlsOutputTypeDef,
+    ListObjectsOutputOutputTypeDef,
+    ListObjectsV2OutputOutputTypeDef,
+    ListObjectVersionsOutputOutputTypeDef,
+    GetBucketOwnershipControlsOutputOutputTypeDef,
     PutBucketOwnershipControlsRequestRequestTypeDef,
-    GetBucketWebsiteOutputTypeDef,
+    GetBucketWebsiteOutputOutputTypeDef,
     WebsiteConfigurationTypeDef,
+    ServerSideEncryptionConfigurationOutputTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
-    SelectObjectContentEventStreamTypeDef,
+    SelectObjectContentEventStreamOutputTypeDef,
+    IntelligentTieringConfigurationOutputTypeDef,
+    LifecycleRuleOutputTypeDef,
+    MetricsConfigurationOutputTypeDef,
     IntelligentTieringConfigurationTypeDef,
     LifecycleRuleTypeDef,
     MetricsConfigurationTypeDef,
+    StorageClassAnalysisOutputTypeDef,
     StorageClassAnalysisTypeDef,
-    GetObjectLockConfigurationOutputTypeDef,
+    GetObjectLockConfigurationOutputOutputTypeDef,
     PutObjectLockConfigurationRequestRequestTypeDef,
+    LambdaFunctionConfigurationOutputTypeDef,
+    QueueConfigurationOutputTypeDef,
+    TopicConfigurationOutputTypeDef,
     LambdaFunctionConfigurationTypeDef,
     QueueConfigurationTypeDef,
     TopicConfigurationTypeDef,
+    GetBucketLoggingOutputOutputTypeDef,
     PutBucketAclRequestBucketAclPutTypeDef,
     PutBucketAclRequestRequestTypeDef,
     PutObjectAclRequestObjectAclPutTypeDef,
     PutObjectAclRequestRequestTypeDef,
     OutputLocationTypeDef,
     BucketLoggingStatusTypeDef,
-    GetBucketLoggingOutputTypeDef,
+    InventoryDestinationOutputTypeDef,
     InventoryDestinationTypeDef,
     PutBucketLifecycleRequestBucketLifecyclePutTypeDef,
     PutBucketLifecycleRequestRequestTypeDef,
+    ReplicationRuleOutputTypeDef,
     ReplicationRuleTypeDef,
     PutBucketWebsiteRequestBucketWebsitePutTypeDef,
     PutBucketWebsiteRequestRequestTypeDef,
-    GetBucketEncryptionOutputTypeDef,
+    GetBucketEncryptionOutputOutputTypeDef,
     PutBucketEncryptionRequestRequestTypeDef,
-    SelectObjectContentOutputTypeDef,
-    GetBucketIntelligentTieringConfigurationOutputTypeDef,
-    ListBucketIntelligentTieringConfigurationsOutputTypeDef,
+    SelectObjectContentOutputOutputTypeDef,
+    GetBucketIntelligentTieringConfigurationOutputOutputTypeDef,
+    ListBucketIntelligentTieringConfigurationsOutputOutputTypeDef,
+    GetBucketLifecycleConfigurationOutputOutputTypeDef,
+    GetBucketMetricsConfigurationOutputOutputTypeDef,
+    ListBucketMetricsConfigurationsOutputOutputTypeDef,
     PutBucketIntelligentTieringConfigurationRequestRequestTypeDef,
     BucketLifecycleConfigurationTypeDef,
-    GetBucketLifecycleConfigurationOutputTypeDef,
-    GetBucketMetricsConfigurationOutputTypeDef,
-    ListBucketMetricsConfigurationsOutputTypeDef,
     PutBucketMetricsConfigurationRequestRequestTypeDef,
+    AnalyticsConfigurationOutputTypeDef,
     AnalyticsConfigurationTypeDef,
-    NotificationConfigurationResponseMetadataTypeDef,
+    NotificationConfigurationOutputTypeDef,
     NotificationConfigurationTypeDef,
     RestoreRequestTypeDef,
     PutBucketLoggingRequestBucketLoggingPutTypeDef,
     PutBucketLoggingRequestRequestTypeDef,
+    InventoryConfigurationOutputTypeDef,
     InventoryConfigurationTypeDef,
+    ReplicationConfigurationOutputTypeDef,
     ReplicationConfigurationTypeDef,
     PutBucketLifecycleConfigurationRequestBucketLifecycleConfigurationPutTypeDef,
     PutBucketLifecycleConfigurationRequestRequestTypeDef,
-    GetBucketAnalyticsConfigurationOutputTypeDef,
-    ListBucketAnalyticsConfigurationsOutputTypeDef,
+    GetBucketAnalyticsConfigurationOutputOutputTypeDef,
+    ListBucketAnalyticsConfigurationsOutputOutputTypeDef,
     PutBucketAnalyticsConfigurationRequestRequestTypeDef,
     PutBucketNotificationConfigurationRequestBucketNotificationPutTypeDef,
     PutBucketNotificationConfigurationRequestRequestTypeDef,
     RestoreObjectRequestObjectRestoreObjectTypeDef,
     RestoreObjectRequestObjectSummaryRestoreObjectTypeDef,
     RestoreObjectRequestRequestTypeDef,
-    GetBucketInventoryConfigurationOutputTypeDef,
-    ListBucketInventoryConfigurationsOutputTypeDef,
+    GetBucketInventoryConfigurationOutputOutputTypeDef,
+    ListBucketInventoryConfigurationsOutputOutputTypeDef,
     PutBucketInventoryConfigurationRequestRequestTypeDef,
-    GetBucketReplicationOutputTypeDef,
+    GetBucketReplicationOutputOutputTypeDef,
     PutBucketReplicationRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AbortIncompleteMultipartUploadTypeDef:
+def get_structure() -> AbortIncompleteMultipartUploadOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-s3-1.28.3/mypy_boto3_s3.egg-info/SOURCES.txt` & `mypy-boto3-s3-1.28.3.post1/mypy_boto3_s3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3-1.28.3/setup.py` & `mypy-boto3-s3-1.28.3.post1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-s3",
-    version="1.28.3",
+    version="1.28.3.post1",
     packages=["mypy_boto3_s3"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.S3 1.28.3 service generated with mypy-boto3-builder 7.14.6"
+        "Type annotations for boto3.S3 1.28.3 service generated with mypy-boto3-builder 7.14.7"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

